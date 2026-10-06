# Incremental modernisation of a legacy municipal system

| | |
|---|---|
| **Client** | State capital municipal government |
| **Sector** | Public sector |
| **Source code** | private repository — read access on request |

## What it is

Proof that a production system can be modernised without a big-bang rewrite. The target is a municipal project-approval system: Angular 8 from 2019, running in production. The repository contains the client's two original systems, the complete reverse engineering carried out on them, and a slice rebuilt in Angular 22 that genuinely runs — side by side with the legacy system, against the same server. One command brings up the three services: the legacy system inside a `node:12.13.1` container, the same `FROM` as the original Dockerfile, so nothing from 2019 is installed on anyone's machine; the new slice; and an API simulator with Swagger. Both sides write to the same log file, and it is this request-level equivalence — not visual similarity of the screens — that supports the argument. The documentation numbers the reverse-engineering findings and marks, for each, the level of confidence and what is still unknown.

---

[← back to index](../README.md)
