# VoiceInput

**English** · [繁體中文](README.zh-Hant.md) · [日本語](README.ja.md)

**Offline voice input for Mac and Windows** — press a hotkey, speak, and the text appears right at your cursor, in any app. On-device Whisper, **60+ languages**, **100% offline** — your voice never leaves your computer. Best-in-class accuracy for **Chinese, Japanese & Korean**.

This repo hosts the **public releases**.

## Download

Get the latest build from **[Releases](../../releases)**:

| Platform | File | Notes |
|---|---|---|
| macOS | `VoiceInput-x.y.zip` | Model downloaded on first run (~574 MB) |
| Windows | `VoiceInput-x.y.z-setup.exe` | Models bundled — works offline right after install |

## Install — macOS

1. Download and unzip → drag **VoiceInput.app** to your Applications folder
2. Open it (signed with Apple Developer ID & notarized — no Gatekeeper warnings)
3. Follow the first-run guide: download the model, grant **Microphone** and **Accessibility**
4. In any app, press the hotkey, speak, and the text is inserted at your cursor

## Install — Windows

1. Run `VoiceInput-x.y.z-setup.exe` — no administrator rights needed
2. VoiceInput lives in the notification area; tap **Left Ctrl** to start speaking, tap again to finish
3. Right-click the tray icon for settings, file transcription and licensing

Nothing else to install: the recognition model and every required library are included.
GPU acceleration uses **Vulkan**, which ships with your graphics driver — NVIDIA, AMD and Intel
are all covered by the same build. Without a Vulkan-capable driver it falls back to the CPU,
which still works but is much slower.

> The Windows build is **not code-signed yet**, so SmartScreen shows a warning on first run.
> Choose *More info → Run anyway*. Signing is planned for a later release.

## Requirements

| | macOS | Windows |
|---|---|---|
| OS | macOS 14 or later | Windows 10 or later (64-bit) |
| Recommended | Apple Silicon (M-series) | Any GPU with an up-to-date driver |
| Disk space | ~600 MB for the model | ~700 MB |

## Features

- On-device Whisper (large-v3-turbo) — accurate across 60+ languages
- 100% offline & private — nothing is uploaded
- Inserts into any app · CJK typography polish (CJK↔Latin spacing, punctuation, simplified/traditional)
- Automatic punctuation restoration for Chinese
- Custom dictionary · learns from your edits · two-language quick switch
- Transcribe audio/video files to text or SRT subtitles
- Interface in Traditional Chinese, Simplified Chinese, Japanese and English

One license covers **both Mac and Windows** — the device count is shared across platforms.

---

© 2026 momosoft · Powered by Whisper, running entirely on-device
