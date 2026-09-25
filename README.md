# MiMo TTS Reader

**Product — browser text-to-speech for content, learning, and accessibility.**

Design or clone a voice, generate natural speech, download WAV/MP3 — no install. Built to show how far a single-page app can go on a modern TTS API.

https://github.com/user-attachments/assets/5bd1c4ec-60b7-4899-a73b-d29ac71049c5

**[Live Demo →](https://47096.github.io/mimo-reader/)**

---

## Why this product

Teams need voiceover without a studio. This app turns **text + a voice choice** into audio you can ship — with **design** (describe a voice) and **clone** (upload a sample) in one place. I kept it **client-side** so the workflow stays fast and the mental model stays simple.

## Use cases

| Use | What you get |
|-----|----------------|
| **Podcast / YouTube** | Intros, outros, ads — or your own cloned host voice |
| **Marketing** | Brand voice for social, explainers, decks |
| **Accessibility** | Listen to long text (dyslexia, vision, audio-first) |
| **E-learning** | Consistent narration for courses |
| **Localization** | Accents/styles for different audiences |

## Features

- **100+ preset voices** (6 categories)
- **Voice design** — editable descriptions
- **Voice clone** — file or mic
- **WAV / MP3 download**
- Dark/light theme · responsive · `⌘+Enter` generate · non-blocking generation

## Getting started

1. Open **[the live app](https://47096.github.io/mimo-reader/)**  
2. **Settings** → add your [MiMo TTS](https://platform.xiaomimimo.com/docs/en-US/welcome) API key  
3. Text → pick a voice → **Generate**  

### Voice design
Mode → voice (search/filter) → text → Generate → download.

### Voice clone
Mode → upload or record → text → Generate → download.

### Preview
Play icon on any voice · edit description · **Random** for new descriptions.

---

## API (MiMo TTS v2.5)

| Model | Use |
|-------|-----|
| `mimo-v2.5-tts-voicedesign` | Custom voices from description |
| `mimo-v2.5-tts-voiceclone` | Clone from audio sample |
| `mimo-v2.5-tts` | Preset voices / dialect tags |

| Region | Endpoint |
|--------|----------|
| Singapore | `https://token-plan-sgp.xiaomimimo.com/v1/chat/completions` |
| China | `https://token-plan-cn.xiaomimimo.com/v1/chat/completions` |
| Standard | `https://api.xiaomimimo.com/v1/chat/completions` |

**Privacy:** your API key stays in the browser (Settings). Text/audio go to the TTS provider you configure — this app has no backend of its own.

### Platform credits (optional)

I use **MiMo Open Platform**. Invite link if you want signup credit: code **`RRJPZE`** → [Sign up](https://platform.xiaomimimo.com?ref=RRJPZE) ($2 credit + 10% off first plan).

![MiMo invite](images/RRJPZE.png)

## Tech

Single-page **HTML/CSS/JS** · MiMo TTS (OpenAI-compatible) · Web Audio · lamejs (MP3) · JetBrains Mono  

**Browsers:** Chrome 90+ · Firefox 88+ · Safari 14+ · Edge 90+

| Shortcut | Action |
|----------|--------|
| `⌘+Enter` | Generate |
| `Escape` | Cancel |
| `Space` | Play / pause |

## Family

- [`hanna`](https://github.com/47096/hanna) — Chrome TTS extension (karaoke highlight, clone)
- [`lux-tts`](https://github.com/47096/lux-tts) — Colab voice-clone **demo**
- [`mimo-storyteller`](https://github.com/47096/mimo-storyteller) — multi-character audio stories

## License

MIT · [datafying](https://datafying.co/)
