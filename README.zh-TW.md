# 大嘴鳥字幕

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

大嘴鳥字幕是一款桌面應用程式，使用 Whisper 在本機將音訊和影片轉寫成字幕，也可透過您設定的服務翻譯字幕。

## 下載與安裝

發佈後可從 [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases) 取得對應版本。請下載符合您系統的檔案。

| OS | Package | Steps |
| --- | --- | --- |
| macOS 13 或更新版本，Apple 晶片 | DMG / ZIP | 開啟 DMG 或解壓縮 ZIP，將應用程式移至「應用程式」。 |
| Windows x64 | EXE | 執行安裝程式，再從「開始」功能表開啟。 |
| Windows x64 | ZIP | 完整解壓縮後執行 `大嘴鸟字幕.exe`。 |

若系統提示缺少 Visual C++ x64 執行階段，請從 [Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist) 安裝或修復。

## 開始轉寫

在設定中下載 Whisper 模型，將音訊或影片加入工作區，再開始轉寫。如需翻譯，請選擇服務和目標語言。遠端服務會收到送交翻譯的字幕文字。

## 校驗下載

依檔名比對 Release 提供的 SHA-256。 [SHA256SUMS.txt](SHA256SUMS.txt)

- macOS: `shasum -a 256 <filename>`
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`

## 支援與授權

可在 [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) 回報應用程式版本、系統版本、重現步驟和錯誤訊息。應用程式的「說明 → 關於」提供第三方授權。

## 1.2.02 · 發佈候選

更新了轉寫工具 FFmpeg / FFprobe 8.1.3，精簡了執行環境，並隨 Release 提供轉寫工具和 Electron 播放程式庫的對應原始碼。Windows 重新建置 NumPy 2.5.2，使用系統的 Visual C++ x64。四份安裝包和兩份原始碼包皆通過下載和 SHA-256 校驗。Windows 安裝版與免安裝版另通過啟動、離線語音偵測及實際轉寫。macOS 為臨時簽署，尚未取得 Apple 公證。Windows 套件尚未簽署。

[Windows x64](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43328309404) · [macOS / FFmpeg](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43330776354)
