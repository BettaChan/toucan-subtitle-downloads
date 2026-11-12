# 版本记录 · Changelog

## 1.2.02 · 发布候选

- 转写工具改用独立构建的 FFmpeg / FFprobe 8.1.3，采用 LGPL 2.1 或更新版本。
- 精简了随包运行库。Mac DMG / ZIP 约 289.6 / 291.0 MiB，Windows EXE / ZIP 约 145.0 / 200.9 MiB。
- 「帮助 → 关于」加入应用授权与第三方许可入口。
- Windows 从源码重建 NumPy 2.5.2，使用微软 Visual C++ x64 系统运行库，保留 OpenBLAS 许可与引擎诊断。
- 两个平台的归档通过解包和内容一致性检查。Windows 两个新版包在 Windows x64 runner 上通过下载校验、启动、离线 VAD 和真实音频转写。Mac 使用 ad-hoc 签名，尚无 Apple 公证。Windows 未做发行者签名。
- 随 Release 提供转写 FFmpeg 和 Electron 播放库各自的对应源码。

## 1.2.02 · Release candidate (English)

- Uses a standalone FFmpeg / FFprobe 8.1.3 build for transcription under LGPL 2.1 or later.
- Slimmed the bundled runtimes. The macOS DMG / ZIP are about 289.6 / 291.0 MiB. The Windows EXE / ZIP are about 145.0 / 200.9 MiB.
- Added app and third-party licenses under Help → About.
- Rebuilt NumPy 2.5.2 from source for Windows. It uses Microsoft's system Visual C++ x64 runtime. OpenBLAS notices and the engine diagnostic are included.
- Both platforms passed archive integrity checks. The rebuilt Windows installer and portable ZIP passed download checks, startup, offline VAD, and speech transcription on a Windows x64 runner. The macOS build is ad-hoc signed and awaits notarization. The Windows build is unsigned.
- The Release includes corresponding source for the transcription tools and for Electron's FFmpeg playback library.
