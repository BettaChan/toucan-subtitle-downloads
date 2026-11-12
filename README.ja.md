# Toucan Subtitle

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

Toucan Subtitle は Whisper を使用して音声や動画をローカルで文字起こしするデスクトップアプリです。設定したサービスで字幕を翻訳できます。

## ダウンロードとインストール

公開後、お使いの環境に合ったパッケージを [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases) から取得してください。

| OS | Package | Steps |
| --- | --- | --- |
| macOS 13 以降、Apple シリコン | DMG / ZIP | DMG を開くか ZIP を展開し、アプリを「アプリケーション」に移動します。 |
| Windows x64 | EXE | インストーラーを実行し、スタートメニューからアプリを開きます。 |
| Windows x64 | ZIP | ZIP をすべて展開し、`大嘴鸟字幕.exe` を実行します。 |

Visual C++ x64 ランタイムが見つからない場合は、[Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist) からインストールまたは修復してください。

## 文字起こしを始める

設定で Whisper モデルをダウンロードします。ワークスペースに音声や動画を追加し、文字起こしを開始します。翻訳する場合はサービスと翻訳先の言語を選びます。外部サービスを利用する場合、翻訳対象の字幕テキストが送信されます。

## ダウンロードの確認

ファイル名に対応する SHA-256 の値を GitHub Releases で確認し、計算結果と照合してください。 [SHA256SUMS.txt](SHA256SUMS.txt)

- macOS: `shasum -a 256 <filename>`
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`

## サポートとライセンス

[Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) にアプリと OS のバージョン、再現手順、エラーメッセージを記載してください。第三者ライセンスは「ヘルプ → このアプリについて」で確認できます。

## 1.2.02 · リリース候補

文字起こし用の FFmpeg / FFprobe を 8.1.3 に更新し、同梱コンポーネントを軽量化しました。文字起こしツールと Electron の再生ライブラリのソースコードを公開候補に添付しています。Windows 用の NumPy 2.5.2 を再ビルドし、システムの Visual C++ x64 ランタイムを使用します。パッケージ 4 点とソースアーカイブ 2 点のダウンロードと SHA-256 検証が完了しました。Windows の 2 種類のパッケージは、起動、オフライン音声区間検出、実音声の文字起こしにも合格しました。macOS 版はアドホック署名済みで、Apple の公証は未取得です。Windows 版は未署名です。

[Windows x64](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43328309404) · [macOS / FFmpeg](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43330776354)
