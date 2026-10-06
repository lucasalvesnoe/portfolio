# DIRECTFUEL — external fleet refuelling

| | |
|---|---|
| **Client** | Road transport group |
| **Sector** | Transport and logistics |
| **Status** | PoC approved; contract in negotiation |
| **Source code** | private repository — read access on request |

## What it is

MVP for managing external fleet refuelling, built for a 60-day pilot at a road transport group and presented to the client under the DIRECTFUEL brand. Three roles share one workflow: the driver requests fuel from their phone, the pump attendant confirms at the pump, and the manager audits on the dashboard. It includes an anti-fraud rule engine and mandatory photo evidence, but the constraint that shaped the architecture is a different one: roadside fuel stations have no signal, so the operation is fully offline and syncs later. The stack uses Postgres in Docker Compose, Prisma for schema and seed, and JWT authentication with a PIN for the driver. No seed password has a default value in the code: the seed fails unless the environment variables are set with the required minimum length.

## Stack

```
@prisma/client · prisma · tsx
```

---

[← back to index](../README.md)
