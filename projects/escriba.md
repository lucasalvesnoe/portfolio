# Escriba — meetings recorded and transcribed on the Mac itself

| | |
|---|---|
| **Sector** | Agents, infrastructure and tooling |
| **Period** | 2026-08-10 → 2026-08-30 |
| **Commits** | 32 |
| **Languages** | Python 50%, Swift 21%, JavaScript 18%, CSS 8% |
| **Source code** | private repository — read access on request |

## What it is

Records, transcribes and summarises meetings on the Mac with no bot joining the call, no virtual audio driver and no audio leaving the machine. It works with anything that makes a sound (Teams, Meet, Zoom, WhatsApp, Discord, FaceTime, browser video) because it captures system audio via ScreenCaptureKit rather than any specific app's API. The microphone is captured in parallel on a separate track with AVAudioEngine, and it is these two distinct tracks that provide speaker separation, without statistical diarisation. Transcription runs locally, live, with Metal-accelerated whisper.cpp. At the end, the Claude CLI generates a summary, memory and index in Markdown. Python with Swift components for the native macOS APIs.

## Repository composition

59 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `docs` | 11 | 432 KB |
| `escriba` | 25 | 190 KB |
| `web` | 8 | 114 KB |
| `(raiz)` | 5 | 98 KB |
| `native` | 8 | 85 KB |
| `tools` | 1 | 7 KB |
| `bin` | 1 | 0 KB |

---

[← back to index](../README.md)
