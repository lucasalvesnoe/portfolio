# Escriba — meetings recorded and transcribed on the Mac itself

| | |
|---|---|
| **Sector** | Agents, infrastructure and tooling |
| **Source code** | private repository — read access on request |

## What it is

Records, transcribes and summarises meetings on the Mac with no bot joining the call, no virtual audio driver and no audio leaving the machine. It works with anything that makes a sound (Teams, Meet, Zoom, WhatsApp, Discord, FaceTime, browser video) because it captures system audio via ScreenCaptureKit rather than any specific app's API. The microphone is captured in parallel on a separate track with AVAudioEngine, and it is these two distinct tracks that provide speaker separation, without statistical diarisation. Transcription runs locally, live, with Metal-accelerated whisper.cpp. At the end, the Claude CLI generates a summary, memory and index in Markdown. Python with Swift components for the native macOS APIs.

---

[← back to index](../README.md)
