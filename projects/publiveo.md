# PubliVeo — video into multichannel content

| | |
|---|---|
| **Sector** | Own products and platforms |
| **Period** | 2026-05-15 → 2026-06-12 |
| **Commits** | 230 |
| **Languages** | TypeScript 73%, Python 25%, CSS 2%, Mako 0% |
| **Source code** | private repository — read access on request |

## What it is

A SaaS platform that turns a recorded video into content ready to publish on the creator's social channels, with no manual editing. It is the project with the longest history in the portfolio, at 230 commits. The pipeline runs from upload to transcription, clip suggestions with a score per segment, and copy generation adapted to each channel (LinkedIn, Instagram, YouTube and blog), each with a native preview of the platform's format and version history. On top of the pipeline sits a complete product layer: Supabase authentication, a profile with nickname, a public page per creator, a credits system and Stripe checkout. The repository shows deliberate engineering practice: design specs versioned before implementation, technical plans per phase, and a recorded refactor of a monolithic 1005-line page into separate panels.

## Repository composition

222 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `PDF-BLOG` | 2 | 2099 KB |
| `frontend` | 113 | 1007 KB |
| `docs` | 25 | 534 KB |
| `backend` | 76 | 262 KB |
| `(raiz)` | 5 | 99 KB |
| `.github` | 1 | 0 KB |

---

[← back to index](../README.md)
