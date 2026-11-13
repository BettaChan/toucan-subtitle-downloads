# Toucan Subtitle · 大嘴鸟字幕

[![Official website: toucansub.app](https://img.shields.io/badge/Official%20website-toucansub.app-0969da?style=for-the-badge)](https://toucansub.app/)

**Local Whisper GUI for macOS & Windows**

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

Toucan Subtitle is a desktop app that transcribes audio and video locally with Whisper and can translate subtitles through a service you configure.

## Download and install

Download the [latest release](https://github.com/BettaChan/toucan-subtitle-downloads/releases/latest) or visit the [official download page](https://toucansub.app/en/downloads.html#platforms). [Changelog](CHANGELOG.md) · [1.2.03 SHA-256](https://github.com/BettaChan/toucan-subtitle-downloads/releases/download/v1.2.03/SHA256SUMS-ToucanSubtitle-1.2.03.txt)

| Platform | Package | Installation |
| --- | --- | --- |
| macOS 13 or later, Apple silicon | DMG / ZIP | Open the DMG or extract the ZIP, then move the app to Applications. |
| Windows x64 | EXE | Run the installer, then open the app from the Start menu. |
| Windows x64 | ZIP | Extract the whole archive, then run `大嘴鸟字幕.exe` from the extracted folder. |

If Windows reports a missing Visual C++ x64 runtime, install or repair it from [Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist).

## Get started

1. Open Settings → Speech Transcription and download a Whisper model.
2. Add audio or video to the workspace and start transcription.
3. For translation, configure a provider and target language. A remote provider receives the subtitle text you send for translation.

## Verify a download

Compare the file’s SHA-256 with the value listed for its exact name in the Release. If you downloaded every file named in `SHA256SUMS-ToucanSubtitle-1.2.03.txt`, put the files and checksum list in one directory.

- macOS: `shasum -a 256 <filename>`, or `shasum -a 256 -c SHA256SUMS-ToucanSubtitle-1.2.03.txt` for the full set.
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`.

## Support and licensing

Use [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) to report the app version, OS version, steps to reproduce, and error text. Review screenshots and logs for local paths, subtitle text, accounts, or keys before posting.

In the app, open Help → About → Third-Party Licenses. Releases include source, build instructions, and notices for the transcription FFmpeg tools and the Electron playback library.
