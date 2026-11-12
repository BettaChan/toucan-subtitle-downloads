# Changelog · 版本记录

[简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

## 1.2.02 · Release candidate

- Uses a standalone FFmpeg / FFprobe 8.1.3 build for transcription under LGPL 2.1 or later.
- Slimmed the bundled runtimes. The macOS DMG / ZIP are about 289.6 / 291.0 MiB. The Windows EXE / ZIP are about 145.0 / 200.9 MiB.
- Added app and third-party licenses under Help → About.
- Rebuilt NumPy 2.5.2 from source for Windows. It uses Microsoft's system Visual C++ x64 runtime. OpenBLAS notices and the engine diagnostic are included.
- Both platforms passed archive integrity checks. The rebuilt Windows installer and portable ZIP passed download checks, startup, offline VAD, and speech transcription on a Windows x64 runner. The macOS build is ad-hoc signed and awaits notarization. The Windows build is unsigned.
- The Release includes corresponding source for the transcription tools and for Electron's FFmpeg playback library.
- Both macOS packages and both FFmpeg source archives passed SHA-256 verification after download from GitHub.
