# Changelog · 版本记录

[简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

## 1.2.05 · 2026-11-15

- The first-run wizard follows the system language and guides users through setup checks, Whisper model preparation, and the choice of transcription or translation.
- 首次启动向导跟随系统语言，引导用户检查环境、准备 Whisper 模型，并选择仅转写或转写并翻译。

[Release / 发布附件](https://github.com/BettaChan/toucan-subtitle-downloads/releases/tag/v1.2.05) · [SHA-256](https://github.com/BettaChan/toucan-subtitle-downloads/releases/download/v1.2.05/SHA256SUMS-ToucanSubtitle-1.2.05.txt)

## 1.2.04 · 2026-11-13

- Added background update checks at startup and localized the macOS app name and Windows installer.
- 新增启动时后台检查更新，macOS 应用名称与 Windows 安装界面随系统语言显示。

[Release / 发布附件](https://github.com/BettaChan/toucan-subtitle-downloads/releases/tag/v1.2.04) · [SHA-256](https://github.com/BettaChan/toucan-subtitle-downloads/releases/download/v1.2.04/SHA256SUMS-ToucanSubtitle-1.2.04.txt)

## 1.2.03 · 2026-11-13

- Added a recovery guide for Whisper downloads, with HF-Mirror retry and links to model files on ModelScope.
- Added offline import for downloaded Whisper model folders.
- 新增 Whisper 下载失败引导、HF-Mirror 重试、魔搭模型文件入口和离线模型导入。

[Release / 发布附件](https://github.com/BettaChan/toucan-subtitle-downloads/releases/tag/v1.2.03) · [SHA-256](https://github.com/BettaChan/toucan-subtitle-downloads/releases/download/v1.2.03/SHA256SUMS-ToucanSubtitle-1.2.03.txt)

## 1.2.02

- Uses a standalone FFmpeg / FFprobe 8.1.3 build for transcription under LGPL 2.1 or later.
- Slimmed the bundled runtimes. The macOS DMG / ZIP are about 258.4 / 293.7 MiB. The Windows EXE / ZIP are about 144.9 / 200.8 MiB.
- Added app and third-party licenses and a manual Check for Updates under Help → About.
- Rebuilt NumPy 2.5.2 from source for Windows. It uses Microsoft's system Visual C++ x64 runtime. OpenBLAS notices and the engine diagnostic are included.
- Both platforms passed local archive integrity checks. The macOS app passed a local startup test and is ad-hoc signed, with Apple notarization pending. The Windows packages are unsigned and await native installation, startup, and transcription retesting.
- The Release includes corresponding source for the transcription tools and for Electron's FFmpeg playback library.
- Local SHA-256 verification passed for the four current packages and both FFmpeg source archives.
