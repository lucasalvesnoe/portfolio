# EducAI — civil servant training portal

| | |
|---|---|
| **Client** | Public sector — civil servant training |
| **Sector** | Public sector |
| **Period** | 2026-03-11 → 2026-06-16 |
| **Commits** | 101 |
| **Languages** | TypeScript 68%, HTML 23%, JavaScript 5%, Python 3% |
| **Source code** | private repository — read access on request |

## What it is

A training portal for public servants, and the project with the largest history in the collection: 101 commits. Standalone Angular with Supabase, organised into `core` (route guards, authentication interceptor, models, services) and `features` by domain. The catalogue of courses and learning paths is just the surface: it also has AI content generation, a study copilot, a prompt studio so the administrator can tune prompts without touching code, PDF certificate issuing (jsPDF), gamification with a leaderboard, an events area, spreadsheet export, user management, a persisted audit trail, and HeyGen and Higgsfield integration for avatar video. Authentication has two paths (Supabase and direct Postgres), and billing runs through AbacatePay.

## Declared dependencies

Extracted from the repository manifests.

```
@angular/common · @angular/compiler · @angular/core · @angular/forms · @angular/platform-
browser · @angular/router · @supabase/supabase-js · cors · dotenv · express · jspdf · rxjs ·
tslib · xlsx
```

## Repository composition

277 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `Docs` | 29 | 12433 KB |
| `educai-backend` | 91 | 5358 KB |
| `test-screenshots` | 33 | 3182 KB |
| `public` | 6 | 1829 KB |
| `src` | 60 | 858 KB |
| `Arquitetura` | 7 | 387 KB |
| `(raiz)` | 18 | 360 KB |
| `poc-catalogo-v2` | 18 | 190 KB |
| `scripts` | 10 | 81 KB |
| `netlify` | 1 | 16 KB |
| `.vscode` | 4 | 2 KB |

---

[← back to index](../README.md)
