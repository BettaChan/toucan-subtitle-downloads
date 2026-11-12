# 大嘴鸟字幕

大嘴鸟字幕是一款桌面应用，可在本机用 Whisper 将音视频转写为字幕，并按设置调用翻译服务。

## 下载与安装

版本附件发布后可从 [GitHub Releases](https://github.com/BettaChan/dazui-subtitle-downloads/releases) 获取。[版本记录](CHANGELOG.md) · [1.2.02 SHA-256](SHA256SUMS.txt)

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

把安装包与对应版本的 `SHA256SUMS.txt` 放在同一个目录，对照文件名和 SHA-256 值。

- macOS 可运行 `shasum -a 256 -c SHA256SUMS.txt`。如果只下载了一个安装包，可运行 `shasum -a 256 <文件名>` 并对照该行。
- Windows PowerShell 可运行 `Get-FileHash -Algorithm SHA256 <文件名>` 并对照该行。

## 反馈与许可

可在 [Issues](https://github.com/BettaChan/dazui-subtitle-downloads/issues) 提交应用版本、系统版本、复现步骤和报错文字。请先检查截图和日志中的本地路径、字幕、账号或密钥。

应用及第三方组件的许可可从「帮助 → 关于 → 第三方许可」查看。转写 FFmpeg 的对应源码与构建资料随版本提供。
