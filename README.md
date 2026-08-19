# Cokiry for macOS

> Fast, private, on-device neural text-to-speech for macOS powered by Kokoro-82M.

[![macOS 15+](https://img.shields.io/badge/macOS-15%2B-black?logo=apple)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-Apple%20Silicon%20%7C%20Intel-blue)](https://github.com)
[![Engine](https://img.shields.io/badge/TTS-Kokoro--82M-orange)](https://github.com/hexgrad/kokoro)

Cokiry is a native macOS speech utility that reads highlighted text across any application via a global shortcut or directly inside its built-in document reader (EPUB, PDF, Markdown, TXT). 

Everything runs locally on your machine: no telemetry, no cloud dependencies, and zero monthly API subscriptions.

---

## Key Features

- **100% Local Neural TTS:** Powered by Kokoro-82M running via ONNX Runtime with zero cloud calls.
- **Global Selection Reader:** Highlight text in any application (Safari, Slack, Xcode, Notes) and trigger instant playback via hotkey or the macOS Services menu (`Read with Cokiry`).
- **Built-in Document Reader:** Open TXT, Markdown, PDF, and EPUB files with real-time sentence-by-sentence highlight and progress tracking.
- **Pure-Swift G2P:** Built-in grapheme-to-phoneme lexicons with stress assignment and number expansion—zero Python runtime overhead.
- **Audio Export:** Export synthesized audio directly to `.wav` files.
- **Lightweight Menu Bar Utility:** Quick voice switching, speed adjustment, and playback controls always within reach.

---

## Download & Installation

1. Download the latest `Cokiry.dmg` from the [Releases](https://github.com/<your-org>/<your-repo>/releases/latest) page.
2. Open the DMG and drag **Cokiry.app** into your `/Applications` folder.
3. Launch the app and grant **Accessibility** permissions when prompted to enable reading highlighted text across other apps.

> **Note on macOS Gatekeeper:**  
> If macOS alerts that the developer cannot be verified, right-click `Cokiry.app` in `/Applications` and select **Open**, or run:
> ```bash
> xattr -cr /Applications/Cokiry.app
> ```

---

## Pricing & Licensing

Cokiry provides a permanent free tier with an optional one-time Pro upgrade:

| Feature | Free Tier | Pro ($19.99 One-Time) |
| :--- | :--- | :--- |
| **Character Limit** | 5,000 characters / session | **Unlimited** |
| **Local Inference** | Full Speed | Full Speed |
| **Speed Control** | Presets (0.5×, 1.0×, 1.5×, 2.0×) | **Continuous fine-tuned slider** |
| **Reader Fonts** | Default system font | **Custom typography** |
| **Save to Audio** | — | **Export full documents to `.wav`** |

*License keys are sold via Paddle and activated directly inside the app.*

---

## System Requirements

- **OS:** macOS 15.0 or later
- **Architecture:** Apple Silicon (M1/M2/M3/M4) or Intel x86_64
- **RAM:** Minimum 8 GB (16 GB recommended for multi-tasking)

---

## Feedback & Bug Reports

Found an issue with voice generation, pronunciation, or document rendering? Please open an issue via [GitHub Issues](https://github.com/<your-org>/<your-repo>/issues).

---

## Third-Party Licenses & Attribution

Cokiry is distributed as proprietary software and incorporates components under the following permissive open-source licenses:

- **Kokoro-82M** (Apache-2.0) — Model weights & voices by [@hexgrad](https://github.com/hexgrad/kokoro)
- **Misaki G2P** (Apache-2.0) — Grapheme-to-phoneme lexicon data by [@hexgrad](https://github.com/hexgrad/misaki)
- **ONNX Runtime** (MIT) — Inference runtime by Microsoft