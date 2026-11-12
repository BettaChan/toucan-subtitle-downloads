# Toucan Subtitle

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Русский](README.ru.md) · [ไทย](README.th.md)

Toucan Subtitle เป็นแอปเดสก์ท็อปสำหรับถอดเสียงจากไฟล์เสียงและวิดีโอบนเครื่องด้วย Whisper และแปลคำบรรยายผ่านบริการที่คุณตั้งค่าได้

## ดาวน์โหลดและติดตั้ง

หลังเผยแพร่ ให้เลือกแพ็กเกจที่ตรงกับระบบของคุณใน [GitHub Releases](https://github.com/BettaChan/toucan-subtitle-downloads/releases)

| OS | Package | Steps |
| --- | --- | --- |
| macOS 13 ขึ้นไป ชิป Apple | DMG / ZIP | เปิด DMG หรือแตกไฟล์ ZIP แล้วย้ายแอปไปยังโฟลเดอร์ Applications |
| Windows x64 | EXE | เรียกใช้ตัวติดตั้ง แล้วเปิดแอปจากเมนู Start |
| Windows x64 | ZIP | แตกไฟล์ ZIP ทั้งหมด แล้วเรียกใช้ `大嘴鸟字幕.exe` |

หากไม่มี Visual C++ x64 Runtime ให้ติดตั้งหรือซ่อมแซมจาก [Microsoft](https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist)

## เริ่มถอดเสียง

ดาวน์โหลดโมเดล Whisper ในการตั้งค่า เพิ่มไฟล์เสียงหรือวิดีโอในพื้นที่ทำงาน แล้วเริ่มถอดเสียง หากต้องการแปล ให้เลือกบริการและภาษาเป้าหมาย บริการระยะไกลจะได้รับข้อความคำบรรยายที่ส่งไปแปล

## ตรวจสอบไฟล์ดาวน์โหลด

เปรียบเทียบค่า SHA-256 ของไฟล์กับค่าของชื่อไฟล์เดียวกันในรุ่นบน GitHub [SHA256SUMS.txt](SHA256SUMS.txt)

- macOS: `shasum -a 256 <filename>`
- Windows PowerShell: `Get-FileHash -Algorithm SHA256 <filename>`

## การสนับสนุนและสัญญาอนุญาต

แจ้งเวอร์ชันแอป เวอร์ชันระบบปฏิบัติการ ขั้นตอนที่ทำให้เกิดปัญหา และข้อความข้อผิดพลาดใน [Issues](https://github.com/BettaChan/toucan-subtitle-downloads/issues) ดูสัญญาอนุญาตของส่วนประกอบอื่นได้ในเมนูวิธีใช้ → เกี่ยวกับ

## 1.2.02 · รุ่นเตรียมเผยแพร่

อัปเดตเครื่องมือถอดเสียง FFmpeg / FFprobe เป็น 8.1.3 และลดขนาดส่วนประกอบที่รวมมา พร้อมแนบซอร์สโค้ดของเครื่องมือถอดเสียงและไลบรารีเล่นสื่อของ Electron สร้าง NumPy 2.5.2 สำหรับ Windows จากซอร์สโค้ดและใช้ Visual C++ x64 Runtime ของระบบ แพ็กเกจสี่ไฟล์และซอร์สโค้ดสองไฟล์ผ่านการดาวน์โหลดและตรวจสอบ SHA-256 แพ็กเกจ Windows ทั้งสองผ่านการทดสอบเปิดแอป ตรวจจับเสียงพูดแบบออฟไลน์ และถอดเสียงจริง แอป macOS ลงนามแบบ ad hoc และยังไม่ผ่านการรับรองจาก Apple ส่วนแพ็กเกจ Windows ยังไม่ได้ลงนาม

[Windows x64](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43328309404) · [macOS / FFmpeg](https://github.com/BettaChan/toucan-subtitle-downloads/actions/runs/43330776354)
