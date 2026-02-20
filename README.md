# VoiceForge 🎙️
> Unlimited text-to-speech — no word limits, no sign-up, every language your browser supports.

![HTML](https://img.shields.io/badge/HTML-5-orange) ![CSS](https://img.shields.io/badge/CSS-3-blue) ![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow) ![License](https://img.shields.io/badge/license-MIT-green)

---

## ✨ Features

- **No word limit** — paste entire articles, books, or scripts and it will speak through all of it
- **Every language & accent** your browser/OS has installed (English US/UK, Spanish, French, German, Japanese, and many more)
- **Quick-pick voice chips** — click to switch voices without using the dropdown
- **Rate, Pitch & Volume** sliders with live readout
- **Pause & Resume** mid-speech
- **Progress bar** showing which segment is playing
- **Animated waveform** visualizer while speaking
- **Zero dependencies** — pure HTML, CSS, and the built-in Web Speech API

---

## 📁 File Structure

```
voiceforge/
├── index.html        ← Page structure & layout
├── css/
│   └── style.css     ← All styling, animations & responsive design
└── js/
    ├── voices.js     ← Loads browser voices, builds language/voice dropdowns
    ├── speech.js     ← Text chunking, playback, pause & stop logic
    └── ui.js         ← Sliders, character counter, status bar, progress bar
```

---

## 🚀 Getting Started

### Option 1 — Open locally
Just download the zip, extract it, and open `index.html` in your browser. No server needed.

### Option 2 — Host on GitHub Pages

1. Create a new GitHub repository (e.g. `voiceforge` or `yourusername.github.io`)
2. Upload all files, keeping the folder structure intact so `index.html` is at the root
3. Go to **Settings → Pages → Source** and select the `main` branch
4. Your site will be live at `https://yourusername.github.io/voiceforge` within a minute or two

---

## 🌐 Browser Support

| Browser | Support | Notes |
|---------|---------|-------|
| Chrome (desktop) | ✅ Best | Most voices, including high-quality neural voices |
| Edge | ✅ Great | Uses Windows neural voices |
| Safari (macOS/iOS) | ✅ Good | System voices available |
| Firefox | ⚠️ Limited | Fewer voices, some features may vary |

> **Tip:** For more voices, install additional language packs in your operating system's language/accessibility settings. Chrome and Edge will automatically detect them.

---

## 🔧 How It Works

The app uses the browser's built-in **Web Speech API** (`SpeechSynthesis`). Long texts are automatically split into sentence-aware chunks of ~180 words each to work around browser utterance length limits. Each chunk is queued and spoken back-to-back seamlessly.

---

## 📝 License

MIT — free to use, modify, and distribute.
