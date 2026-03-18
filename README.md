<div align="center">

# 🍂 st6.download

### Video & Music Downloader

**Download videos and music from 9+ platforms with a beautiful animated UI.**

[![Version](https://img.shields.io/badge/version-2.10.0-orange?style=for-the-badge)](https://github.com/st6autumn/st6-download/releases/latest)
[![Platform](https://img.shields.io/badge/platform-Windows-blue?style=for-the-badge&logo=windows)](https://github.com/st6autumn/st6-download/releases/latest)
[![Electron](https://img.shields.io/badge/electron-28-47848F?style=for-the-badge&logo=electron)](https://www.electronjs.org/)
[![License](https://img.shields.io/badge/license-Proprietary-red?style=for-the-badge)](LICENSE)

**[⬇ Download Latest Release](https://github.com/st6autumn/st6-download/releases/latest)**

---

*Made by [Autumn](https://linktr.ee/st6.autumn)*

</div>

---

## 📖 About

**st6.download** is a sleek, all-in-one video and music downloader built with Electron. It features a fully animated canvas background with 6 unique themes, a modern dark UI, and support for downloading from all major platforms — no browser extensions, no ads, no bloat.

Everything runs locally on your machine. No accounts required, no data collected, no servers involved.

---

## 🌐 Supported Platforms

| Platform | Video | Music | Notes |
|----------|:-----:|:-----:|-------|
| YouTube | ✅ | ✅ | Resolution picker for 1080p+ |
| TikTok | ✅ | — | |
| Instagram | ✅ | — | Requires cookies.txt |
| Twitter/X | ✅ | — | |
| Spotify | — | ✅ | Requires free API credentials |
| SoundCloud | — | ✅ | Direct download |
| Apple Music | — | ✅ | Via spotdl |
| Tidal | — | ✅ | Via spotdl |
| Other | ✅ | — | Generic extraction for streaming sites |

---

## ✨ Features

### Downloads
- **Video** — MP4 with H.264 re-encode (CRF 18, slow preset)
- **Music** — MP3, WAV, or FLAC with embedded cover art
- **Resolution picker** — choose 1080p, 1440p, 4K, or Best for YouTube
- **Subtitles** — burn English CC directly into the video
- **Queue system** — batch multiple downloads
- **Pause/Resume** — freeze mid-download and pick up where you left off
- **Filename watermark** — ` [🍂 st6]` tag on all downloads
- **URL tracking stripper** — auto-removes utm_*, fbclid, gclid, etc.

### UI & Themes
- **6 animated canvas themes** — Autumn (falling leaves), Forest (fireflies), Snow (dissolving flakes), Aurora (curtains), Fire (embers), Mono (moonlit midnight)
- **12 languages** — English, Spanish, French, German, Portuguese, Japanese, Korean, Chinese, Russian, Arabic, Thai, Hindi
- **Startup animation** — custom splash screen with embedded SFX
- **Close animation** — CRT TV power-down with embedded SFX
- **Rounded window edges** — 18px smooth corners
- **Format-specific colours** — MP4 gold, MP3 coral, WAV teal, FLAC violet
- **3D flip animation** — audio button flips when default format changes
- **Download history** — browse and reopen past downloads
- **Colour hue slider** — shift the palette within each theme

### Settings (4 tabs)
- **System** — updates, dependencies, save folder, uninstall
- **General** — language, audio format, Instagram cookies, Spotify API
- **Appearance** — theme picker, colour hue slider
- **Features** — 11 toggleable features including startup/close animations

---

## 🔄 Auto-Updates

st6.download checks for updates automatically on startup. When a new version is available:
1. A popup appears center-screen showing the new version and formatted changelog
2. Click **"Install Update"** to download the new installer with a progress bar
3. Click **"Install & Restart"** to apply

You can also manually check via **Settings → System → Check for Updates**.

---

## 📥 Instagram Setup

Instagram requires a cookies.txt file for downloads:
1. Install the [Get cookies.txt LOCALLY](https://chromewebstore.google.com/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc) Chrome extension
2. Go to instagram.com while logged in
3. Export cookies → browse the file in Settings → General

---

## 🛠️ Tech Stack

| Component | Purpose |
|-----------|---------|
| [Electron](https://www.electronjs.org/) | Desktop app framework |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | Video downloading engine |
| [FFmpeg](https://ffmpeg.org/) | Video/audio processing & conversion |
| [spotdl](https://github.com/spotDL/spotify-downloader) | Spotify/Apple Music/Tidal downloads |
| HTML5 Canvas | Animated theme backgrounds |

---

## 📊 Stats

| Metric | Value |
|--------|-------|
| Frontend | 3,111 lines |
| Backend | 1,996 lines |
| Languages | 12 |
| Themes | 6 animated |
| Platforms | 9 supported |
| Settings tabs | 4 (System, General, Appearance, Features) |
| Feature toggles | 11 |

---

## 📜 License

© 2025-2026 Autumn. All rights reserved.

This software is proprietary. You may not copy, modify, distribute, or reverse-engineer any part of this application without explicit written permission from the author.

---

## 🙏 Acknowledgments

st6.download is built on top of incredible open-source tools:

- **[yt-dlp](https://github.com/yt-dlp/yt-dlp)** — the backbone of video downloading. A fork of youtube-dl with active development and broad site support.
- **[FFmpeg](https://ffmpeg.org/)** — the Swiss army knife of video/audio processing. Handles conversion, re-encoding, subtitle burn-in, thumbnail embedding, and more.
- **[spotdl](https://github.com/spotDL/spotify-downloader)** — downloads music from Spotify, Apple Music, and Tidal by matching tracks on YouTube Music.
- **[Electron](https://www.electronjs.org/)** — makes it possible to build a native Windows app with web technologies.
- **[electron-builder](https://www.electron.build/)** — packages and distributes the app as a Windows installer.

These projects are maintained by their respective communities and are not affiliated with st6.download.

---

<div align="center">

**[⬇ Download Latest Release](https://github.com/st6autumn/st6-download/releases/latest)**

*st6.download — by [Autumn](https://linktr.ee/st6.autumn) 🍂*

</div>
