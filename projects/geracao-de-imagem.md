# Image generation lab with locked identity

| | |
|---|---|
| **Sector** | Agents, infrastructure and tooling |
| **Period** | 2026-09-11 → 2026-09-22 |
| **Commits** | 154 |
| **Languages** | Python 74%, HTML 16%, Shell 5%, CSS 3% |
| **Source code** | private repository — read access on request |

## What it is

An image generation lab with consistent identity, running on a GPU rented by the hour — 154 commits, the second-largest history in the collection. The work does not happen in ComfyUI: there are three local screens of its own, one for the cast and the creation workbench, one for following GPU hydration byte by byte, and one for the GPU marketplace with the history of rental rounds. The core technical problem is locking a character's identity across generations, which is what separates a pretty image from a usable character; the secondary one is economic — spinning up a GPU on demand, loading the models, working and tearing it down before the hour turns into dead cost. Internal use.

## Repository composition

320 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `krea_bot` | 137 | 30821 KB |
| `runpod` | 60 | 1948 KB |
| `workflows-lucas` | 33 | 875 KB |
| `docs` | 25 | 790 KB |
| `(raiz)` | 16 | 309 KB |
| `pod` | 17 | 122 KB |
| `bot` | 20 | 119 KB |
| `anaconda_projects` | 1 | 32 KB |
| `graphify-out` | 9 | 25 KB |
| `workflows` | 1 | 10 KB |
| `.virtual_documents` | 1 | 2 KB |

---

[← back to index](../README.md)
