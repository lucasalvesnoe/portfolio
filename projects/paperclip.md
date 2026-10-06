# AIsquad — a team of agents on top of company context

| | |
|---|---|
| **Sector** | Agents, infrastructure and tooling |
| **Code files** | 942 |
| **Lines of code** | 195,443 |
| **Extensions** | `.ts` ×646, `.tsx` ×163, `.sql` ×41, `.py` ×40, `.sh` ×30 |
| **Source code** | not versioned on GitHub — available on request |

## What it is

AIsquad is a team of AI agents that works on the company's real context: project folders, email, Teams and the CRM. It runs entirely on the local machine, on top of Paperclip, and talks through Telegram. It is the largest system in the portfolio: 942 files and about 195k lines, not counting the vendored upstream. The architectural decision that defines everything is the boundary between disk and agent. Collection and filtering are deterministic and never call a model: scripts read the local Teams v2 cache, the Mail.app and Outlook stores, meetings and the CRM, filter by project and write a `digest.md` in that project's folder. Only then does an agent read the digest, and only then are tokens spent. Everything before the boundary costs nothing, so every filter lives before it, never after. There are six collection plugins (local context; local mail with no Azure or Graph API; local Teams; escriba, which turns a recorded meeting into an issue with action items; read-only HubSpot; and a knowledge graph over the folders), plus six deterministic work modules: an archivist that sweeps for evidence to close issues, a reconciler that checks open issues against deal stage, finance for commission and cash-flow forecasting, an auditor with an append-only incident table and fixed vocabulary, a watcher on token consumption and tier, and an audit of the workspaces. The interface is Telegram with its own Mini App (board, agent profile, consumption). The repository is published as a template: real client data, billing and the agents' instructions are kept out by `.gitignore`, and no secret goes into a file. Keys and tokens live in the macOS Keychain, and the config stores only the item name, never the value. A missing key makes the script fail immediately, saying which one, instead of carrying on with `undefined` and breaking three functions later.

## Structure

```
arquivista/
auditor/
conciliador/
contexto/
docs/
financeiro/
intelliway-hq/
miniapp/
paperclip-plugin-contexto-local/
paperclip-plugin-escriba/
paperclip-plugin-graph/
paperclip-plugin-hubspot/
paperclip-plugin-mail-local/
paperclip-plugin-teams-local/
quota/
skills-lucas/
telegram/
tools/
wireguard-air/
```

---

[← back to index](../README.md)
