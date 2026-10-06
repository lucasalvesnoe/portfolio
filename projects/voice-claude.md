# Claudinho — voice interface for Claude Code

| | |
|---|---|
| **Sector** | Agents, infrastructure and tooling |
| **Source code** | private repository — read access on request |

## What it is

Portuguese-language voice interface for Claude Code — speak and the agent runs commands, edits files and executes scripts, without losing any tool along the way. In version 1.6 the Claude Agent SDK is the single brain: its structured stream (text, tool call, reasoning, result) is rendered cleanly in an xterm.js terminal, instead of running a second `claude` process in a PTY — which guarantees a single session and makes the TTS read only the prose of the reply, never the tool noise. It works without a headset, because echo cancellation uses macOS's `VoiceProcessingIO`, the same AEC as Siri and FaceTime. Local transcription with whisper.cpp, neural TTS, and a native dark interface.

---

[← back to index](../README.md)
