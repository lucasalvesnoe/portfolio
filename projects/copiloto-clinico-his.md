# MedInsights — clinical copilot on a hospital information system

| | |
|---|---|
| **Client** | Hospital — off-the-shelf hospital management system |
| **Sector** | Healthcare |
| **Period** | 2026-04-16 → 2026-08-11 |
| **Commits** | 10 |
| **Languages** | TypeScript 97%, CSS 2%, JavaScript 1%, HTML 0% |
| **Source code** | private repository — read access on request |

## What it is

A proof of concept of the clinical copilot, demonstrated on top of the interface of an off-the-shelf hospital management system. It analyses the patient record in real time, cross-referencing three sources that are not normally read together: the doctor's written progress notes, the nursing notes and the test history. This produces two kinds of alert: inconsistency, when what the doctor reports contradicts a vital sign measured by nursing, and trend, when a series of test results points to a subtle deterioration that a single reading would not show, such as acute kidney injury under way. It shows the chain of clinical reasoning behind each conclusion, so the doctor can disagree on solid grounds. The side panel pushes the content aside rather than covering it, and has a minimised mode. Generation by Gemini 2.5 Pro.

## Declared dependencies

Taken from the repository's manifests.

```
@anthropic-ai/sdk · @google/genai · react · react-dom
```

---

[← back to index](../README.md)
