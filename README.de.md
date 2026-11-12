# Toucan Subtitle

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

Toucan Subtitle transkribiert Audio und Video lokal mit Whisper und kann Untertitel über einen von Ihnen eingerichteten Dienst übersetzen.

## Download und Installation

Nach der Veröffentlichung finden Sie die Pakete unter [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases).

| OS | Package | Steps |
| --- | --- | --- |
| macOS 13 oder neuer, Apple-Chip | DMG / ZIP | DMG öffnen oder ZIP entpacken, dann die App in den Ordner „Programme“ verschieben. |
| Windows x64 | EXE | Installationsprogramm ausführen und die App über das Startmenü öffnen. |
| Windows x64 | ZIP | ZIP vollständig entpacken und `大嘴鸟字幕.exe` starten. |

Falls die Visual C++-Laufzeit für x64 fehlt, installieren oder reparieren Sie sie über [Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist).

## Erste Transkription

Laden Sie in den Einstellungen ein Whisper-Modell herunter, fügen Sie Audio oder Video zum Arbeitsbereich hinzu und starten Sie die Transkription. Für Übersetzungen wählen Sie einen Dienst und eine Zielsprache. Ein externer Dienst erhält den übermittelten Untertiteltext.

## Download prüfen

Vergleichen Sie die SHA-256-Prüfsumme mit dem Eintrag für den Dateinamen im Release. [SHA256SUMS.txt](SHA256SUMS.txt)

- macOS: `shasum -a 256 <filename>`
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`

## Support und Lizenzen

Melden Sie Probleme unter [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) mit App- und Systemversion, Schritten zur Reproduktion und Fehlermeldung. Drittanbieterlizenzen finden Sie unter „Hilfe → Über“.

## 1.2.02 · Veröffentlichungskandidat

Aktualisiert FFmpeg / FFprobe für die Transkription auf 8.1.3 und verkleinert die mitgelieferten Laufzeitkomponenten. Der Release enthält den Quellcode der Transkriptionswerkzeuge und der Wiedergabebibliothek von Electron. Unter Windows wurde NumPy 2.5.2 neu gebaut und verwendet die Visual C++-Systemlaufzeit für x64. Vier Programmpakete und zwei Quellarchive wurden heruntergeladen und per SHA-256 geprüft. Beide Windows-Pakete bestanden auch Start-, Offline-Spracherkennungs- und Transkriptionstests. Die macOS-App ist ad hoc signiert und noch nicht von Apple notarisiert. Die Windows-Pakete sind unsigniert.

[Windows x64](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43328309404) · [macOS / FFmpeg](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43330776354)
