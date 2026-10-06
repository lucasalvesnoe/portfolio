# Clinical inconsistency copilot

| | |
|---|---|
| **Client** | Clinic using a cloud-based EHR |
| **Sector** | Healthcare |
| **Period** | 2026-09-08 → 2026-09-23 |
| **Commits** | 15 |
| **Languages** | TypeScript 100% |
| **Source code** | private repository — read access on request |

## What it is

A clinical copilot for a cloud-based EHR, with a different angle from the protocol-adherence copilot: instead of checking adherence to a protocol, it looks for what does not add up in the clinical reasoning. When a consultation is opened, it reads what has already been written, retrieves the same patient's previous consultations and lists in the sidebar contradictions between records, worsening trends, requested tests that never had an outcome, and management decisions without justification. Each finding carries the excerpt from the patient record that supports it and, where relevant, a button that writes the suggestion back. Prioritisation uses the Manchester Triage System, with the model instructed to emit findings in that order and the sidebar re-sorting them to guarantee it: red for treatment management, orange for medication and tests, yellow for record inconsistencies, green for the rest. The cards are numbered because reading priority from colour alone requires knowing the scale.

## Declared dependencies

Extracted from the repository manifests.

```
@vitejs/plugin-react · react · react-dom
```

---

[← back to index](../README.md)
