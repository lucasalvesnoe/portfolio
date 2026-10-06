# CCA-F Trainer — certification exam prep

| | |
|---|---|
| **Sector** | Own products and platforms |
| **Period** | 2026-06-11 → 2026-06-24 |
| **Commits** | 44 |
| **Languages** | TypeScript 74%, Python 24%, CSS 2%, JavaScript 0% |
| **Source code** | private repository — read access on request |

## What it is

A study app for the Claude Certified Architect – Foundations certification. It has a bank of 271 bilingual PT-BR/EN questions with instant language switching inside the quiz, in three modes: review with per-question feedback, timed, and a full 60-question mock exam in 110 minutes with a scaled score from 100 to 1000, as in the real exam. Each question has an interactive AI tutor that explains why each wrong option is wrong and ties it back to the domain, and the API key belongs to the user (BYOK), held only in the browser tab and never on the server. Multi-user, with Clerk login and email verification, progress synced across devices via Upstash Redis keyed per user, plus gamification with XP, levels, streaks and achievements.

## Declared dependencies

Extracted from the repository manifests.

```
@anthropic-ai/sdk · @supabase/ssr · @supabase/supabase-js · @upstash/ratelimit ·
@upstash/redis · @vercel/analytics · @vercel/speed-insights · canvas-confetti · lucide-react
· next · react · react-dom · zod
```

## Repository composition

97 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `data` | 2 | 939 KB |
| `(raiz)` | 13 | 313 KB |
| `src` | 73 | 300 KB |
| `scripts` | 7 | 90 KB |
| `docs` | 2 | 14 KB |

---

[← back to index](../README.md)
