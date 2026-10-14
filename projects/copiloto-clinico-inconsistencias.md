# Clinical inconsistency copilot

| | |
|---|---|
| **Client** | Clinic using a cloud-based EHR |
| **Sector** | Healthcare |
| **Status** | Production-ready (October 2026), clinic pilot starting |
| **Source code** | private repository — read access on request |

## What it is

A clinical copilot for a cloud-based EHR, with a different angle from the protocol-adherence copilot: instead of checking adherence to a protocol, it looks for what does not add up in the clinical reasoning. When a consultation is opened, it reads what has already been written, retrieves the same patient's previous consultations and lists in the sidebar contradictions between records, worsening trends, requested tests that never had an outcome, and management decisions without justification. Each finding carries the excerpt from the patient record that supports it and, where relevant, a button that writes the suggestion back. Prioritisation uses the Manchester Triage System, with the model instructed to emit findings in that order and the sidebar re-sorting them to guarantee it: red for treatment management, orange for medication and tests, yellow for record inconsistencies, green for the rest. The cards are numbered because reading priority from colour alone requires knowing the scale.

## Architecture

```
EHR page (browser)
  └─ Chrome extension (Manifest V3)
       ├─ reads the open consultation + previous consultations
       ├─ de-identifies everything IN THE BROWSER  ← no identifiable data leaves the machine
       └─ HTTPS + per-doctor token
            └─ backend (Node, systemd, nginx)
                 ├─ token check (server stores only hashes), per-token and global rate limits
                 ├─ prompt with the record fenced as data (prompt-injection guard)
                 └─ Amazon Bedrock (Claude), streaming cards back to the sidebar
```

The decisions that define it:

1. **De-identification at the source.** Names, CPF, RG, phone numbers, addresses, dates and record numbers are replaced in the extension before anything is sent. The backend refuses any payload that does not carry the de-identification seal, so a bug in the client fails closed instead of leaking.
2. **Nothing is written without a click.** The doctor sees the exact text that will be written into the record before applying it, and every write goes through the same path into the EHR's editor.
3. **Least-privilege cloud access.** The model runs in the product company's own AWS account. The backend's IAM key can only invoke one model through one inference profile, and only from the backend's own IP: a leaked key does not work anywhere else (verified with the IAM policy simulator).
4. **Logs without patient data.** The backend logs only metadata (token id, card count, latency, token usage). A spending alarm caps surprises on the cloud bill.
5. **Dictation stays on the doctor's screen.** The doctor can dictate the consultation note in Chrome or Edge with live transcription. The text opens in an editable box and is written into the record only after review and a click; it never goes to the model.
6. **Operable by one person.** A runbook covers install, token issuing and revocation, key rotation and an emergency stop under five minutes.

## Quality evidence

1. 180 automated tests, type-check and production build on every pull request.
2. De-identification audited in 5 independent rounds by fresh sessions with no context of the build: 910 curated cases plus more than 20,000 generated fuzz sentences, zero leaks of name, CPF, RG, phone or address.
3. A dedicated security review of the backend stack, with all six findings fixed before release (prompt-injection fencing, write preview, nginx rate limiting, HSTS, systemd hardening).
4. End-to-end smoke test against the production backend: unauthenticated, invalid-token, unsealed and empty requests are rejected; a valid analysis returns its cards in 8 seconds.

## Delivery

The backend, the cloud migration and the security hardening (three sprints of the original plan) were built, reviewed and merged in a single overnight session, with AI-assisted development (Claude Code) and the architect reviewing every decision.

## Stack

```
TypeScript · React · Vite · Chrome Extension Manifest V3 · Node.js · nginx · systemd · Amazon Bedrock (Claude) · AWS IAM · AWS Budgets · GitHub Actions
```

---

[← back to index](../README.md)
