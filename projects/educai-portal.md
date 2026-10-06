# EducAI — civil servant training portal

| | |
|---|---|
| **Client** | Public sector — civil servant training |
| **Sector** | Public sector |
| **Source code** | private repository — read access on request |

## What it is

A training portal for public servants. Standalone Angular with Supabase, organised into `core` (route guards, authentication interceptor, models, services) and `features` by domain. The catalogue of courses and learning paths is just the surface: it also has AI content generation, a study copilot, a prompt studio so the administrator can tune prompts without touching code, PDF certificate issuing (jsPDF), gamification with a leaderboard, an events area, spreadsheet export, user management, a persisted audit trail, and HeyGen and Higgsfield integration for avatar video. Authentication has two paths (Supabase and direct Postgres), and billing runs through AbacatePay.

## Stack

```
@angular/common · @angular/compiler · @angular/core · @angular/forms · @angular/platform-
browser · @angular/router · @supabase/supabase-js · cors · dotenv · express · jspdf · rxjs ·
tslib · xlsx
```

---

[← back to index](../README.md)
