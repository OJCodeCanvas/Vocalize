# Vocalize
Free, browser-based speech-to-text transcription. No sign-ups, no API keys, no limits.

```markdown
# Vocalize — Free Speech to Text

A completely free, browser-based transcription tool. No API keys, no sign-ups, no limits. Open the page, hit record, speak — text appears instantly.

> **100% client-side.** No data leaves your browser. No server. No subscriptions.

![GitHub release](https://img.shields.io/badge/version-1.0.0-amber?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![No API Key](https://img.shields.io/badge/no_API_key-required-red?style=flat-square)

---

## Features

- **Live mic transcription** — real-time speech-to-text as you speak
- **30+ languages** — English, Spanish, French, Japanese, Arabic, Hindi, and more
- **Continuous mode** — keeps listening until you stop
- **Timestamps** — toggle `[HH:MM:SS]` markers per segment
- **Fully editable output** — click to correct before copying
- **Copy to clipboard** — one click, paste anywhere
- **Download as `.txt`** — plain text export
- **Download as `.srt`** — subtitle file with proper timing
- **Audio file playback** — drop MP3/WAV, play through speakers, transcribe via mic
- **Live waveform visualizer** — see audio levels while recording
- **Keyboard shortcut** — `Ctrl + Shift + M` to toggle recording
- **Timer & word count** — always visible

---

## Quick Start

### Option 1 — Just open it
```
Double-click index.html in Chrome/Edge/Brave
```

### Option 2 — Local server (recommended)
```bash
python -m http.server 8000
# Then open http://localhost:8000
```

---

## Browser Support

| Browser | Status |
|---------|--------|
| Chrome | ✅ Full support |
| Edge | ✅ Full support |
| Brave | ✅ Full support |
| Firefox | ❌ No Speech Recognition API |
| Safari | ❌ No Speech Recognition API |

> The Web Speech Recognition API may require internet the first time to download the language model. After that it works offline in most cases.

---

## How It Works

Uses the browser's built-in **Web Speech API**. Everything runs locally:

1. Microphone audio captured via `getUserMedia`
2. Browser's speech engine processes it in real-time
3. Results appear in an editable text area
4. Export to clipboard, `.txt`, or `.srt`

**No server. No API keys. No data collection.**

---

## File Structure

```
vocalize/
├── index.html
├── README.md
└── LICENSE
```

---

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Shift + M` | Start / Stop recording |

---

## Limitations

- **Browser-dependent** — only Chromium-based browsers
- **Audio files** — must play through speakers and be picked up by mic (no direct file-to-text in the browser)
- **Accuracy** — depends on mic quality, background noise, and pronunciation
- **Long sessions** — may need manual restarts due to browser memory management

---

## For Direct Audio File Transcription

If you need to transcribe audio files directly (not through mic), check out these free offline tools:

- [Whisper.cpp](https://github.com/ggerganov/whisper.cpp) — Run Whisper locally
- [Buzz](https://github.com/chidiwilliams/buzz) — GUI for Whisper, transcribe files offline
- [WhisperDesktop](https://github.com/Const-me/Whisper) — Windows GUI for Whisper

---

## License

MIT — use it, modify it, share it. No restrictions.
```
