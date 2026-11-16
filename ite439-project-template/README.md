# <ชื่อแอป>

> ITE-439 Mobile Application Development · ภาคเรียนที่ 2/2569 · กลุ่ม gNN
>
> **Lead: แก้ทุกช่องที่อยู่ใน `< >` ให้ครบ แล้วลบบรรทัดนี้ทิ้ง**

## ปัญหาและผู้ใช้

- **ปัญหาที่แก้**: <เขียน 1–2 ประโยค>
- **ผู้ใช้หลัก**: <ใคร ใช้ตอนไหน>
- **หัวข้อโครงงาน**: <เลขและชื่อหัวข้อจากรายการของรายวิชา>

## สมาชิกและบทบาท

| ชื่อ-สกุล | รหัสนักศึกษา | GitHub | บทบาทหลัก |
| --- | --- | --- | --- |
| | | @ | Lead / Integrator |
| | | @ | UI Developer |
| | | @ | Data Developer |
| | | @ | QA & AI Log Owner |

บทบาทหมุนเวียนได้ตามช่วงงาน แต่ทุกคนต้องมี commit และ Pull Request ของตัวเอง

## ฟีเจอร์หลัก

| ฟีเจอร์ | ระดับ | สถานะ |
| --- | --- | --- |
| <เช่น ดูรายการและรายละเอียด> | Core | ยังไม่เริ่ม |
| <เช่น ฟอร์มที่ตรวจค่าก่อนบันทึก> | Core | ยังไม่เริ่ม |
| <เช่น เชื่อม REST API> | Core | ยังไม่เริ่ม |
| <เช่น เก็บข้อมูลถาวร Local DB / Firestore> | Core | ยังไม่เริ่ม |
| <งานต่อยอด> | Stretch | ยังไม่เริ่ม |

## วิธีรันแอป

```bash
git clone <ลิงก์ repo นี้>
cd <ชื่อ repo>
flutter pub get
flutter run
```

- Flutter version ที่กลุ่มใช้: <ผลจาก `flutter --version`>
- ไฟล์ที่ต้องขอจาก Lead ก่อนรัน (ไม่อยู่ใน repo เพราะเป็นความลับ): <เช่น `google-services.json` — ถ้าไม่มีให้เขียนว่า "ไม่มี">

## โครงสร้างโค้ด

```text
lib/
├── main.dart
├── ui/        หน้าจอและ widget
├── logic/     state (Provider) และกฎของแอป
└── data/      model, service / API, local DB
assets/mock/   mock JSON จาก Design Pack (R2)
```

## วิธีทำงานร่วมกัน

1. ก่อนเริ่มงาน: `git switch main` แล้ว `git pull`
2. แตก branch ของงานตัวเอง: `git switch -c feature/<ชื่อ>-<งาน>` เช่น `feature/ann-login-ui`
3. commit เป็นช่วงๆ แล้ว `git push -u origin feature/<ชื่อ>-<งาน>`
4. เปิด Pull Request บน GitHub ให้เพื่อนอย่างน้อย 1 คนรีวิว
5. Lead กด Merge แล้วทุกคน `git pull` main

## ส่งงาน (Tag)

| รอบส่ง | Tag | ลิงก์ที่ส่งใน Teams |
| --- | --- | --- |
| Midterm | `midterm` | `<ลิงก์ repo>/tree/midterm` |
| API Check-in | `api-checkin` | `<ลิงก์ repo>/tree/api-checkin` |
| Final | `final` | `<ลิงก์ repo>/tree/final` |

ปัก tag ที่ commit ที่ส่ง: `git tag midterm` แล้ว `git push origin midterm`

## เอกสารในโครงงาน

- [HANDOFF.md](HANDOFF.md) — สถานะงาน สิ่งที่ยังไม่เสร็จ และวิธี build APK
- [AI_LOG.md](AI_LOG.md) — บันทึกการใช้ AI ของสมาชิกทุกคน
