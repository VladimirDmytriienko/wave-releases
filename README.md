# wave — downloads

Local-first macOS AI transcription app. Record audio, capture your screen,
drop a file — get speech-to-text powered by [whisper.cpp][w] entirely on your
Mac. Nothing leaves the device.

This repo hosts the **downloadable builds only**. The source lives in a
separate private repository.

## Download

Grab the latest `.dmg` from the [**Releases**](../../releases/latest) page.

- **Apple Silicon (arm64)** only — M1 / M2 / M3 / M4.
- Requires macOS 12+.

## Install

1. Open the `.dmg` and drag **wave** into **Applications**.
2. First launch: the app is not notarized, so macOS Gatekeeper will warn
   "wave can't be opened because it is from an unidentified developer".
   Fix it once: **right-click wave.app → Open → Open**, or
   **System Settings → Privacy & Security → Open Anyway**.
3. In the app, open **Settings → Models** and download a Whisper model
   (Turbo is the recommended balance).

### Transcription needs ffmpeg

Recording and playback work out of the box. Transcription decodes audio via
`ffmpeg` — install it once:

```bash
brew install ffmpeg
```

## Features

- 🎙️ Audio recording — mic, system audio, or both
- 🖥️ Screen recording — multi-display picker with live previews
- 📂 Import MP3 / M4A / WAV / OGG / FLAC / MP4 / MOV / WEBM / MKV
- ✍️ On-device Whisper transcription (Turbo / Large v3 / Medium / Small / …)
- 🌍 Auto-detect or pin English / Ukrainian / Russian (+ 96 more)
- 👥 Lightweight speaker diarization
- 🎬 Video viewer with synced transcript + subtitle overlay
- 💾 Export TXT / Markdown / SRT / JSON
- ⌘K command palette · 🪟 mini floating recorder
- 🗑️ Built-in uninstall wizard

## License

MIT.

[w]: https://github.com/ggerganov/whisper.cpp
