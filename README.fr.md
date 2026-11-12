# Toucan Subtitle

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

Toucan Subtitle transcrit les fichiers audio et vidéo en local avec Whisper et peut traduire les sous-titres via un service que vous configurez.

## Téléchargement et installation

Après publication, récupérez le paquet adapté à votre système dans [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases).

| OS | Package | Steps |
| --- | --- | --- |
| macOS 13 ou version ultérieure, puce Apple | DMG / ZIP | Ouvrez le DMG ou décompressez le ZIP, puis placez l’application dans Applications. |
| Windows x64 | EXE | Lancez le programme d’installation, puis ouvrez l’application depuis le menu Démarrer. |
| Windows x64 | ZIP | Décompressez entièrement le ZIP et lancez `大嘴鸟字幕.exe`. |

Si l’environnement d’exécution Visual C++ x64 manque, installez-le ou réparez-le depuis [Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist).

## Première transcription

Dans les paramètres, téléchargez un modèle Whisper. Ajoutez un fichier audio ou vidéo à l’espace de travail et lancez la transcription. Pour traduire, choisissez un service et une langue cible. Un service distant reçoit le texte transmis pour traduction.

## Vérification du téléchargement

Comparez le SHA-256 du fichier à celui indiqué sous le même nom dans la version GitHub. [SHA256SUMS.txt](SHA256SUMS.txt)

- macOS: `shasum -a 256 <filename>`
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`

## Assistance et licences

Utilisez [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) pour signaler la version de l’application, la version du système, les étapes de reproduction et le message d’erreur. Consultez les licences tierces dans « Aide → À propos ».

## 1.2.02 · Version candidate

Les outils de transcription FFmpeg / FFprobe passent à la version 8.1.3, et les composants embarqués occupent moins de place. Les sources des outils de transcription et de la bibliothèque de lecture Electron sont jointes à la version. Sous Windows, NumPy 2.5.2 a été recompilé et utilise Visual C++ x64 installé sur le système. Les quatre paquets et les deux archives source ont passé les contrôles de téléchargement et de SHA-256. Les deux paquets Windows ont également passé les tests de démarrage, de détection vocale hors ligne et de transcription. L’application macOS porte une signature ad hoc et n’est pas encore notariée par Apple. Les paquets Windows ne sont pas signés.

[Windows x64](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43328309404) · [macOS / FFmpeg](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43330776354)
