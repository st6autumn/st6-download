<div align="center">

# 🍂 st6.download

### Video & Music Downloader

**Download videos and music from 9+ platforms with a beautiful animated UI.**

[![Version](https://img.shields.io/badge/version-2.9.2-orange?style=for-the-badge)](https://github.com/st6autumn/st6-download/releases/latest)
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

## 🎬 Supported Platforms

### Video
| Platform | Quality | Subtitles | Thumbnails |
|----------|---------|-----------|------------|
| **YouTube** | Up to 4K | ✅ English (burn-in) | ✅ |
| **TikTok** | Best available | ❌ | ✅ Embedded |
| **Instagram** | Best available | ❌ | ✅ |
| **Twitter/X** | Best available | ❌ | ✅ |
| **Other URLs** | Auto-detected | ✅ English (burn-in) | ✅ |

### Music
| Platform | Formats | Cover Art | Method |
|----------|---------|-----------|--------|
| **Spotify** | MP3 / WAV / FLAC | ✅ Embedded | via spotdl |
| **SoundCloud** | MP3 / WAV / FLAC | ✅ Embedded | Direct stream |
| **Apple Music** | MP3 / WAV / FLAC | ✅ Embedded | via spotdl |
| **Tidal** | MP3 / WAV / FLAC | ✅ Embedded | via spotdl |

### "Other" URL Extraction
For streaming sites that aren't directly supported (anime sites, movie sites, etc.), st6.download uses a built-in browser-based extraction engine:
- 🔍 Follows up to **5 levels** of nested iframes
- 🖱️ Automatically clicks play buttons & server selectors
- 🎭 Anti-bot detection (spoofs Chrome, hides webdriver)
- 📡 Intercepts XHR/fetch AJAX responses for hidden stream URLs
- 🔄 Re-encodes to **H.264 MP4** for editing software compatibility
- 📺 Smart title extraction from page metadata & URL patterns

---

## 🎨 Themes

st6.download features **6 fully animated canvas themes**, each with unique particle effects, colour palettes, and vibes:

| Theme | Description |
|-------|-------------|
| 🍂 **Autumn** | Warm sand-coloured waves with falling leaves that land, sit, and sink into the water |
| 🌿 **Forest** | Dark old-growth trees with volumetric fog, sparse fireflies, near-black mood |
| ❄️ **Snow** | Icy blue waves with unique per-flake snowflakes that dissolve on contact |
| ✨ **Aurora** | Dark night sky with 80 stars and 6 aurora curtains with wave distortion |
| 🔥 **Fire** | 60 fire particle blobs, 40 embers, and heat haze distortion |
| 🌑 **Mono** | Black & white with grid lines, drifting orbs, and a brightness slider |

Each theme responds to the **Colour Hue** slider, letting you shift the entire palette within the theme's range.

---

## ✨ Features

### Core
- 📥 **One-click downloads** — paste a URL, pick a format, hit download
- 🎵 **Video & Music modes** — toggle between platforms with a smooth pill switch
- 📋 **Queue system** — queue multiple downloads, they process automatically
- ⏸ **Pause/Resume** — freeze downloads mid-progress and resume exactly where you left off
- 🔤 **Subtitle burn-in** — downloads and burns English subtitles directly into the video
- 📂 **Auto-open folder** — optionally opens the save folder when done
- 🖼️ **Thumbnail embedding** — all audio downloads include cover art

### UI
- 🎨 **6 animated themes** with canvas particle effects
- 🌈 **Colour Hue slider** for fine-tuning each theme
- ⚙️ **Settings panel** with 4 tabs (System, General, Appearance, Features)
- 📋 **Download history** with click-to-reload
- 📖 **First-run tutorial** with step-by-step guided tour
- 💬 **Themed tooltips** that match the dark UI
- 🔔 **Windows notifications** on download complete
- 🖱️ **Drag & drop** URLs from your browser
- 🔔 **Update popup** — centered modal with changelog, progress bar, one-click install

### Technical
- 🔄 **Auto-updates** — checks GitHub for new versions, downloads and installs the `.exe` automatically
- 🔒 **No source code exposed** — updates are distributed as compiled installers
- 🧹 **Failed download cleanup** — partial files are automatically deleted
- 🍪 **Cookie support** — for Instagram and sites requiring authentication
- 🎯 **Smart filename cleaning** — removes hashtags, @mentions, junk characters from filenames
- 📡 **Binary management** — downloads and manages yt-dlp, ffmpeg, and spotdl automatically
- 🗑️ **Uninstall** — clean removal from Settings → System

---

## 📦 Installation

### Quick Start
1. **[Download the latest release](https://github.com/st6autumn/st6-download/releases/latest)**
2. Run the installer
3. Open st6.download
4. Click **⬇ Download All Dependencies** in Settings → System (one-time setup)
5. Start downloading!

### Spotify / Apple Music / Tidal Setup
These platforms require free Spotify API credentials (takes 2 minutes):
1. Go to [developer.spotify.com/dashboard](https://developer.spotify.com/dashboard)
2. Create an app → set redirect URI to `https://localhost:8888/callback`
3. Copy Client ID and Client Secret into Settings → General

### Instagram Setup
Instagram requires cookies for authentication:
1. Install the [Get cookies.txt LOCALLY](https://chromewebstore.google.com/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc) Chrome extension
2. Go to instagram.com while logged in
3. Export cookies → browse the file in Settings → General

---

## 🔄 Auto-Updates

st6.download checks for updates automatically on startup. When a new version is available:
1. A popup appears center-screen showing the new version and formatted changelog
2. Click **"Install Update"** to download the new installer with a progress bar
3. Click **"Install & Restart"** to apply

You can also manually check via **Settings → System → Check for Updates**.

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
| Frontend | 2,387 lines |
| Backend | 1,834 lines |
| Themes | 6 animated |
| Platforms | 9 supported |
| Settings tabs | 4 (System, General, Appearance, Features) |
| Canvas particles | Leaves, snowflakes, fireflies, embers, aurora curtains, orbs |

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
