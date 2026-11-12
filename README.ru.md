# Toucan Subtitle

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

Toucan Subtitle — настольное приложение для локальной расшифровки аудио и видео с помощью Whisper. Субтитры можно переводить через настроенный вами сервис.

## Загрузка и установка

После публикации выберите пакет для своей системы в [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases).

| OS | Package | Steps |
| --- | --- | --- |
| macOS 13 или новее, чип Apple | DMG / ZIP | Откройте DMG или распакуйте ZIP и переместите приложение в папку «Программы». |
| Windows x64 | EXE | Запустите установщик, затем откройте приложение из меню «Пуск». |
| Windows x64 | ZIP | Распакуйте ZIP целиком и запустите `大嘴鸟字幕.exe`. |

Если отсутствует среда выполнения Visual C++ x64, установите или восстановите её с сайта [Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist).

## Первая расшифровка

Загрузите модель Whisper в настройках, добавьте аудио или видео в рабочую область и запустите расшифровку. Для перевода выберите сервис и язык. Удалённый сервис получит текст субтитров, отправленный на перевод.

## Проверка загрузки

Сравните SHA-256 файла со значением для того же имени в выпуске GitHub. [SHA256SUMS.txt](SHA256SUMS.txt)

- macOS: `shasum -a 256 <filename>`
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`

## Поддержка и лицензии

В [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) укажите версии приложения и ОС, шаги для воспроизведения и сообщение об ошибке. Лицензии сторонних компонентов доступны в разделе «Справка → О программе».

## 1.2.02 · Кандидат на выпуск

FFmpeg / FFprobe для расшифровки обновлены до версии 8.1.3, а размер компонентов уменьшен. К выпуску приложен исходный код инструментов расшифровки и библиотеки воспроизведения Electron. NumPy 2.5.2 для Windows собран из исходников и использует системную среду выполнения Visual C++ x64. Четыре пакета и два архива исходников прошли проверку загрузки и SHA-256. Оба пакета Windows также прошли проверку запуска, автономного обнаружения речи и расшифровки. Приложение для macOS имеет подпись ad hoc и пока не нотарифицировано Apple. Пакеты Windows не подписаны.

[Windows x64](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43328309404) · [macOS / FFmpeg](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43330776354)
