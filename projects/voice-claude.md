# Claudinho — voice interface for Claude Code

| | |
|---|---|
| **Sector** | Agents, infrastructure and tooling |
| **Period** | 2026-06-03 → 2026-06-04 |
| **Commits** | 9 |
| **Languages** | Python 56%, HTML 37%, Swift 4%, Shell 3% |
| **Source code** | private repository — read access on request |

## What it is

Portuguese-language voice interface for Claude Code — speak and the agent runs commands, edits files and executes scripts, without losing any tool along the way. In version 1.6 the Claude Agent SDK is the single brain: its structured stream (text, tool call, reasoning, result) is rendered cleanly in an xterm.js terminal, instead of running a second `claude` process in a PTY — which guarantees a single session and makes the TTS read only the prose of the reply, never the tool noise. It works without a headset, because echo cancellation uses macOS's `VoiceProcessingIO`, the same AEC as Siri and FaceTime. Local transcription with whisper.cpp, neural TTS, and a native dark interface.

## Repository composition

16 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `(raiz)` | 15 | 119 KB |
| `ui` | 1 | 51 KB |

---

[← back to index](../README.md)
