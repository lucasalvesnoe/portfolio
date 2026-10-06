# Account holder change via WhatsApp with OCR

| | |
|---|---|
| **Client** | State water and sanitation company |
| **Sector** | Public sector |
| **Period** | 2026-05-13 → 2026-06-15 |
| **Commits** | 20 |
| **Languages** | HTML 58%, JavaScript 20%, Python 11%, CSS 11% |
| **Source code** | private repository — read access on request |

## What it is

A conversational chatbot that guides the company's customer through the whole process of changing the account holder on a water account over WhatsApp, without going through a human agent in the usual case. The customer photographs the documents within the conversation itself; the OCR runs on Claude's computer vision and extracts the fields straight from the image, with no fixed template per document type. What the AI extracts never becomes a decision on its own: it lands in an admin panel where an operator reviews, corrects and approves before it takes effect. There are three surfaces on the same backend: the chat that simulates WhatsApp, the customer portal and the review panel. Backend in Python 3.11 with FastAPI and SQLite; the repository also versions the PRD, changelog, schedule and the PoC timeline.

## Repository composition

196 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `docs` | 28 | 22567 KB |
| `frontend` | 156 | 7449 KB |
| `backend` | 9 | 67 KB |
| `(raiz)` | 3 | 2 KB |

---

[← back to index](../README.md)
