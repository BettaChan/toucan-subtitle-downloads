# Changelog · 版本记录

[简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

## 1.2.02 · Release candidate

- Uses a standalone FFmpeg / FFprobe 8.1.3 build for transcription under LGPL 2.1 or later.
- Slimmed the bundled runtimes. The macOS DMG / ZIP are about 258.4 / 293.7 MiB. The Windows EXE / ZIP are about 144.9 / 200.8 MiB.
- Added app and third-party licenses and a manual Check for Updates under Help → About.
- Rebuilt NumPy 2.5.2 from source for Windows. It uses Microsoft's system Visual C++ x64 runtime. OpenBLAS notices and the engine diagnostic are included.
- Both platforms passed local archive integrity checks. The macOS app passed a local startup test and is ad-hoc signed, with Apple notarization pending. The Windows packages are unsigned and await native installation, startup, and transcription retesting.
- The Release includes corresponding source for the transcription tools and for Electron's FFmpeg playback library.
- Local SHA-256 verification passed for the four current packages and both FFmpeg source archives.
