# Intelligent public data platform

| | |
|---|---|
| **Client** | State research and statistics institute |
| **Sector** | Public sector |
| **Period** | 2026-02-12 → 2026-06-08 |
| **Commits** | 26 |
| **Languages** | HTML 84%, JavaScript 12%, CSS 3% |
| **Source code** | private repository — read access on request |

## What it is

A platform for accessing state public data, built for a state research institute and delivered as a PoC for handoff to the client's Azure team. It brings together, in a single portal, embedded Power BI dashboards, an AI assistant with local RAG and a fallback to EvaGPT, and bespoke analytical modules — a geospatial module, with a map and comparison between municipalities, and Curadoria IA (AI curation). It has role-based access control (client and admin), with different screens per role, and an admin panel that monitors usage. The repository includes the architecture documentation and an explicit list of what must change before going to production — a real backend, vector RAG and JWT authentication in place of the PoC's mock.

## Repository composition

39 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `(raiz)` | 27 | 728 KB |
| `docs` | 10 | 86 KB |
| `.netlify` | 2 | 0 KB |

---

[← back to index](../README.md)
