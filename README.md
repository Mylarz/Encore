<div align="center">

  <h1>Encore</h1>

  <p>
    <strong>An Android music player for your offline library, with karaoke-style synced lyrics.</strong>
  </p>

  <p>
    <img src="https://img.shields.io/badge/License-GPLv3-6366f1?style=for-the-badge&logo=gnu&logoColor=white&labelColor=1e1e2e" alt="License: GPLv3" />
    <img src="https://img.shields.io/badge/Platform-Android%208.0%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white&labelColor=1e1e2e" alt="Android 8.0+" />
  </p>

</div>

---

## About

**Encore** is an open-source Android music player built around local files and word-by-word synced lyrics. It is currently built on top of the [YumaPlayer](https://github.com/MuwMx/YumaPlayer) codebase (GPL-3.0), which itself builds on ArchiveTune, Metrolist and SimpMusic. Encore is its own project and is not affiliated with YumaPlayer or its author.

No subscriptions, no ads, no telemetry.

> Encore is in early development. A lot of the code and some internal names still come from YumaPlayer and are being reworked step by step.

---

## Features (inherited base)

- **Local playback:** FLAC, MP3, AAC, OGG and WAV files stored on your device.
- **Synced lyrics:** line-by-line and word-by-word display, from `.lrc` files, embedded tags, or online providers (LRCLIB, Kugou, BetterLyrics, SimpMusic, Unison, YouLyPlus).
- **Audio engine:** Media3 (ExoPlayer), dual-deck crossfade, 5-band equalizer, loudness normalization, tempo and pitch adjustment, sleep timer.
- **Streaming sources:** optional YouTube Music and Spotify browsing, inherited from the base project.
- **Theming:** dynamic colors extracted from the current artwork.

---

## Building from source

```bash
git clone https://github.com/Mylarz/Encore.git
cd Encore
./gradlew assembleRelease
# Built APK: app/build/outputs/apk/release/
```

Prerequisites: Android Studio with AGP 9.x support, JDK 21, Android SDK 37 (compileSdk/targetSdk 37, minSdk 26).

---

## Documentation

These docs were inherited from YumaPlayer and still use its naming:

- [Architecture Overview](docs/architecture/ARCHITECTURE.md)
- [Architectural Decision Records](docs/architecture/DECISIONS.md)
- [Design System Specification](docs/design/YDS.md)
- [Coding Standards](docs/development/YUMA_RULES.md)

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Acknowledgments

Encore builds on the work of the open-source community:

- **[YumaPlayer](https://github.com/MuwMx/YumaPlayer)** by MuwMix, the direct base of this project.
- **[ArchiveTune](https://github.com/rukamori/ArchiveTune)**, playback foundations and settings base.
- **[Meld](https://github.com/FrancescoGrazioso/Meld)**, Spotify hybrid integration.
- **[Mochy Music](https://github.com/realidkroo/Mochy-Music)**, UI themes and components.
- **[Stash](https://github.com/rawnaldclark/Stash)**, lossless FLAC pipeline inspiration.
- **[Metrolist](https://github.com/mostafaalagamy/Metrolist)** and **[SimpMusic](https://github.com/maxrave-dev/SimpMusic)**, lyrics parsing and interface ideas.
- **[PixelPlayer](https://github.com/theovilardo/PixelPlayer)**, swipe kinematics and queue structure.
- **[LRCLIB](https://lrclib.net/)** and **[BetterLyrics](https://better-lyrics.boidu.dev/)**, open synced lyrics databases.

---

## License

Encore is free software licensed under the **GNU General Public License v3.0**. You may copy, modify and redistribute it as long as you keep the copyright notices and distribute derivative works under the same license.

Encore is an independent third-party client and is not affiliated with, endorsed by, or sponsored by Google LLC, YouTube Music, or Spotify AB.
