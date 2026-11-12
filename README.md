# 大嘴鸟字幕 · Toucan Subtitle

[中文](#中文) · [English](#english)

## 中文

大嘴鸟字幕是一款桌面应用，可在本机用 Whisper 将音视频转写为字幕，并按设置调用翻译服务。

### 下载与安装

版本附件发布后可从 [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases) 获取。[版本记录](CHANGELOG.md) · [1.2.02 SHA-256](SHA256SUMS.txt)

| 平台 | 包 | 安装方法 |
| --- | --- | --- |
| macOS 13 或更新版本，Apple 芯片 | DMG / ZIP | 打开 DMG 或解压 ZIP，把「大嘴鸟字幕」移到「应用程序」。 |
| Windows x64 | EXE | 运行安装程序，完成后从开始菜单打开。 |
| Windows x64 | ZIP | 完整解压后，运行目录里的「大嘴鸟字幕.exe」。 |

Windows 若提示缺少 Visual C++ x64 运行库，可从[微软官方页面](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist)安装或修复。

### 开始转写

1. 打开应用，在「设置 → 语音转写」选择并下载 Whisper 模型。
2. 把音频或视频添加到工作台，开始转写。
3. 如需翻译，在设置中配置翻译服务和目标语言。使用远程翻译服务时，字幕文本会发送给你选定的服务。

### 校验安装包

请按文件名对照对应 Release 中的 SHA-256。下载了 `SHA256SUMS.txt` 列出的所有文件时，可把文件与校验清单放在同一目录批量核对。

- macOS 可运行 `shasum -a 256 -c SHA256SUMS.txt`。如果只下载了一个安装包，可运行 `shasum -a 256 <文件名>` 并对照该行。
- Windows PowerShell 可运行 `Get-FileHash -Algorithm SHA256 <文件名>` 并对照该行。

### 反馈与许可

可在 [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) 提交应用版本、系统版本、复现步骤和报错文字。请先检查截图和日志中的本地路径、字幕、账号或密钥。

应用及第三方组件的许可可从「帮助 → 关于 → 第三方许可」查看。转写 FFmpeg 和 Electron 播放库的对应源码、构建资料及许可随版本提供。

## English

Toucan Subtitle is a desktop app that transcribes audio and video locally with Whisper and can translate subtitles through a service you configure.

### Download and install

After publication, get versioned packages from [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases). [Changelog](CHANGELOG.md) · [1.2.02 SHA-256](SHA256SUMS.txt)

| Platform | Package | Installation |
| --- | --- | --- |
| macOS 13 or later, Apple silicon | DMG / ZIP | Open the DMG or extract the ZIP, then move the app to Applications. |
| Windows x64 | EXE | Run the installer, then open the app from the Start menu. |
| Windows x64 | ZIP | Extract the whole archive, then run `大嘴鸟字幕.exe` from the extracted folder. |

If Windows reports a missing Visual C++ x64 runtime, install or repair it from [Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist).

### Get started

1. Open Settings → Speech Transcription and download a Whisper model.
2. Add audio or video to the workspace and start transcription.
3. For translation, configure a provider and target language. A remote provider receives the subtitle text you send for translation.

### Verify a download

Compare the file’s SHA-256 with the value listed for its exact name in the Release. If you downloaded every file named in `SHA256SUMS.txt`, put the files and checksum list in one directory.

- macOS: `shasum -a 256 <filename>`, or `shasum -a 256 -c SHA256SUMS.txt` for the full set.
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`.

### Support and licensing

Use [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) to report the app version, OS version, steps to reproduce, and error text. Review screenshots and logs for local paths, subtitle text, accounts, or keys before posting.

In the app, open Help → About → Third-Party Licenses. Releases include source, build instructions, and notices for the transcription FFmpeg tools and the Electron playback library.
