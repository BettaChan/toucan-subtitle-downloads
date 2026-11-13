# Toucan Subtitle

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

Toucan Subtitle은 Whisper를 사용해 오디오와 동영상을 기기에서 직접 전사하는 데스크톱 앱입니다. 사용자가 설정한 서비스로 자막을 번역할 수도 있습니다.

## 다운로드 및 설치

공개 후 [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases)에서 시스템에 맞는 패키지를 받으세요.

| OS | Package | Steps |
| --- | --- | --- |
| macOS 13 이상, Apple Silicon | DMG / ZIP | DMG를 열거나 ZIP을 푼 다음 앱을 응용 프로그램 폴더로 옮기세요. |
| Windows x64 | EXE | 설치 프로그램을 실행한 다음 시작 메뉴에서 앱을 여세요. |
| Windows x64 | ZIP | ZIP의 압축을 모두 풀고 `大嘴鸟字幕.exe`를 실행하세요. |

Visual C++ x64 런타임이 없다는 메시지가 표시되면 [Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist)에서 설치하거나 복구하세요.

## 전사 시작하기

설정에서 Whisper 모델을 다운로드합니다. 작업 공간에 오디오나 동영상을 추가하고 전사를 시작합니다. 번역하려면 서비스와 대상 언어를 선택하세요. 원격 서비스에는 번역할 자막 텍스트가 전송됩니다.

## 다운로드 확인

파일의 SHA-256을 계산하고 GitHub 릴리스에서 같은 이름으로 표시된 값과 비교하세요. [SHA256SUMS.txt](SHA256SUMS.txt)

- macOS: `shasum -a 256 <filename>`
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`

## 지원 및 라이선스

[Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues)에 앱과 운영체제 버전, 재현 단계, 오류 메시지를 적어 주세요. 타사 라이선스는 도움말의 정보 화면에서 확인할 수 있습니다.

## 1.2.02 · 릴리스 후보

전사용 FFmpeg / FFprobe를 8.1.3으로 업데이트하고 포함된 런타임의 용량을 줄였습니다. 전사 도구와 Electron 재생 라이브러리의 소스 코드를 릴리스에 첨부했습니다. Windows용 NumPy 2.5.2는 소스에서 다시 빌드했으며 시스템의 Visual C++ x64 런타임을 사용합니다. 도움말의 정보 화면에서 수동으로 업데이트를 확인할 수 있습니다. 최신 패키지 4개와 소스 아카이브 2개의 SHA-256을 로컬에서 검증했습니다. macOS 앱은 로컬 실행 테스트를 통과했습니다. 새 Windows 패키지의 설치, 실행 및 전사는 재시험을 기다리고 있습니다. macOS 앱에는 애드혹 서명이 적용되었으며 Apple 공증은 아직 받지 않았습니다. Windows 패키지는 서명되지 않았습니다.
