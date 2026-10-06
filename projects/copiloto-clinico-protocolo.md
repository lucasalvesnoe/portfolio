# Clinical copilot for protocol adherence

| | |
|---|---|
| **Client** | Clinic network |
| **Sector** | Healthcare |
| **Period** | 2026-06-06 → 2026-09-22 |
| **Commits** | 22 |
| **Languages** | TypeScript 99%, HTML 1% |
| **Source code** | private repository — read access on request |

## What it is

Manifest V3 Chrome extension that injects the clinical copilot into a clinic network's electronic health record (EHR), without the EHR vendor having to integrate anything. The content script reads the consultation open on screen, sends it to the PACK RAG backend and returns a protocol-adherence analysis. The product detail that defines the project is the gate: the "Registrar" (Save) button stays locked until the doctor has reviewed the suggested actions — the AI never writes to the record on its own. The engine runs in three modes: question and answer, clinical-note generation, and gap analysis of the written note against the PACK. React 19 + TypeScript + Vite with `@crxjs/vite-plugin`, and two build targets — the CRX for Chrome and an EHR simulation that runs without Chrome, so the interface can be validated without depending on the client's environment.

## Declared dependencies

Extracted from the repository manifests.

```
@vitejs/plugin-react · react · react-dom
```

---

[← back to index](../README.md)
