# Municipal healthcare systems integration

| | |
|---|---|
| **Client** | Municipal government of a mid-sized municipality |
| **Sector** | Public sector |
| **Source code** | private repository — read access on request |

## What it is

Integration architecture for a municipal government's healthcare systems, as part of the municipality's digital transformation programme. The problem identified in the AS-IS analysis: the citizen app, where appointments are booked, and the healthcare management system, where the consultation is carried out, do not talk to each other — an operator re-keys each booking by hand, with no traceability, and an SMS cancellation frees the slot in the management system but does not return it to the app, leaving idle slots. The proposed design is a mediation layer (anti-corruption layer + API orchestration) that leaves the legacy cores untouched: reading from the app through the REST API it already exposes, with a UUID→CNES mapping resolver (CNES being Brazil's national register of healthcare facilities), and writing to the management system through a new ingestion API. It includes an orchestrator with saga, retry and idempotency, an event bus, a slot reconciler, MDM with a golden record of the citizen, and a natural-language query AI service that is read-only and audited. Sized for ~30k appointments a month.

---

[← back to index](../README.md)
