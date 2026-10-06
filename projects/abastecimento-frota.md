# DIRECTFUEL — external fleet refuelling

| | |
|---|---|
| **Client** | Road transport group |
| **Sector** | Transport and logistics |
| **Period** | 2026-07-28 → 2026-07-31 |
| **Commits** | 25 |
| **Languages** | TypeScript 92%, JavaScript 4%, Rich Text Format 2%, Shell 1% |
| **Source code** | private repository — read access on request |

## What it is

MVP for managing external fleet refuelling, built for a 60-day pilot at a road transport group and presented to the client under the DIRECTFUEL brand. Three roles share one workflow: the driver requests fuel from their phone, the pump attendant confirms at the pump, and the manager audits on the dashboard. It includes an anti-fraud rule engine and mandatory photo evidence, but the constraint that shaped the architecture is a different one: roadside fuel stations have no signal, so the operation is fully offline and syncs later. The stack uses Postgres in Docker Compose, Prisma for schema and seed, and JWT authentication with a PIN for the driver. No seed password has a default value in the code: the seed fails unless the environment variables are set with the required minimum length.

## Declared dependencies

Extracted from the repository manifests.

```
@prisma/client · prisma · tsx
```

## Repository composition

112 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `docs` | 6 | 5057 KB |
| `(raiz)` | 15 | 525 KB |
| `apps` | 75 | 457 KB |
| `packages` | 8 | 33 KB |
| `prisma` | 5 | 30 KB |
| `tests` | 2 | 17 KB |
| `scripts` | 1 | 3 KB |

---

[← back to index](../README.md)
