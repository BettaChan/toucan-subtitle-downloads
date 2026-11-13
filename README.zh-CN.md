# 大嘴鸟字幕

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

大嘴鸟字幕是一款桌面应用，可在本机用 Whisper 将音视频转写为字幕，并按设置调用翻译服务。

## 下载与安装

从 [GitHub 最新正式版](https://github.com/BettaChan/toucan-subtitle-downloads/releases/latest) 或[官网下载页](https://toucansub.app/downloads.html#platforms)选择安装包。[版本记录](CHANGELOG.md) · [1.2.03 SHA-256](https://github.com/BettaChan/toucan-subtitle-downloads/releases/download/v1.2.03/SHA256SUMS-ToucanSubtitle-1.2.03.txt)

| 平台 | 包 | 安装方法 |
| --- | --- | --- |
| macOS 13 或更新版本，Apple 芯片 | DMG / ZIP | 打开 DMG 或解压 ZIP，把「大嘴鸟字幕」移到「应用程序」。 |
| Windows x64 | EXE | 运行安装程序，完成后从开始菜单打开。 |
| Windows x64 | ZIP | 完整解压后，运行目录里的「大嘴鸟字幕.exe」。 |

Windows 若提示缺少 Visual C++ x64 运行库，可从[微软官方页面](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist)安装或修复。

## 开始转写

1. 打开应用，在「设置 → 语音转写」选择并下载 Whisper 模型。
2. 把音频或视频添加到工作台，开始转写。
3. 如需翻译，在设置中配置翻译服务和目标语言。使用远程翻译服务时，字幕文本会发送给你选定的服务。

## 校验安装包

请按文件名对照对应 Release 中的 SHA-256。下载了 `SHA256SUMS-ToucanSubtitle-1.2.03.txt` 列出的所有文件时，可把文件与校验清单放在同一目录批量核对。

- macOS 可运行 `shasum -a 256 -c SHA256SUMS-ToucanSubtitle-1.2.03.txt`。如果只下载了一个安装包，可运行 `shasum -a 256 <文件名>` 并对照该行。
- Windows PowerShell 可运行 `Get-FileHash -Algorithm SHA256 <文件名>` 并对照该行。

## 反馈与许可

可在 [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) 提交应用版本、系统版本、复现步骤和报错文字。请先检查截图和日志中的本地路径、字幕、账号或密钥。

应用及第三方组件的许可可从「帮助 → 关于 → 第三方许可」查看。转写 FFmpeg 和 Electron 播放库的对应源码、构建资料及许可随版本提供。

## 1.2.02 · 发布候选

- 转写工具改用独立构建的 FFmpeg / FFprobe 8.1.3，采用 LGPL 2.1 或更新版本。
- 精简了随包运行库。Mac DMG / ZIP 约 258.4 / 293.7 MiB，Windows EXE / ZIP 约 144.9 / 200.8 MiB。
- 「帮助 → 关于」加入应用授权、第三方许可入口和手动检查更新。
- Windows 从源码重建 NumPy 2.5.2，使用微软 Visual C++ x64 系统运行库，保留 OpenBLAS 许可与引擎诊断。
- 两个平台的归档通过本地完整性检查。macOS 应用通过本地启动测试，采用 ad-hoc 签名，尚无 Apple 公证。Windows 包未签名，安装、启动和实际转写待复测。
- 随 Release 提供转写 FFmpeg 和 Electron 播放库各自的对应源码。

四份新版安装包和两份 FFmpeg 源码包均通过本地 SHA-256 校验。
