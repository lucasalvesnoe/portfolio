# Image generation lab with locked identity

| | |
|---|---|
| **Sector** | Agents, infrastructure and tooling |
| **Source code** | private repository — read access on request |

## What it is

An image generation lab with consistent identity, running on a GPU rented by the hour. The work does not happen in ComfyUI: there are three local screens of its own, one for the cast and the creation workbench, one for following GPU hydration byte by byte, and one for the GPU marketplace with the history of rental rounds. The core technical problem is locking a character's identity across generations, which is what separates a pretty image from a usable character; the secondary one is economic — spinning up a GPU on demand, loading the models, working and tearing it down before the hour turns into dead cost. Internal use.

---

[← back to index](../README.md)
