# Interactive Demos — Immersive Lecture

เด็คเดโมสำหรับสอนวิชา Interactive / Immersive Media
หน้าเดียวจบ (`index.html`) ไม่มี build step · เวทีคงที่ 1920×1080 ย่อ-ขยายตามหน้าจอ

**เปิดดูออนไลน์:** https://ginomcclay28.github.io/Interactive-Demos/

## 14 เดโม

| # | เดโม | อินพุต |
|---|------|--------|
| 01 | Particle Field — ผลัก · ดูดเก็บ · ปล่อยระเบิด | เมาส์ |
| 02 | Pointer Spray — พ่นสีเป็นหางยาว | เมาส์ |
| 03 | Live Camera Tracking — Body / Skeleton / Hand / Face | กล้อง |
| 04 | Speech → Physics — พูดแล้วคำร่วงเป็นวัตถุ | ไมค์ |
| 05 | Waterfall Silhouette — น้ำตกแหวกรอบตัวคน | กล้อง / เมาส์ |
| 06 | Fish School — ลากไล่ปลา · คลิกโปรยอาหาร | เมาส์ |
| 07 | Foggy Mirror — โบกมือเช็ดฝ้า | กล้อง / เมาส์ |
| 08 | Pin Art Wall — ผนังเข็มพินอาร์ต | กล้อง / เมาส์ |
| 09 | Ripple Pool — ผิวน้ำกระเพื่อมจริง | เมาส์ |
| 10 | Aurora Flow Field — ริบบิ้นแสงไหลตาม noise field | เมาส์ |
| 11 | Magnetic Sand — ผงเหล็กเรียงตามสนามแม่เหล็ก | เมาส์ |
| 12 | Kaleidoscope Paint — วาดเส้นเดียวได้ลายมันดาลา | เมาส์ |
| 13 | Cloth & Rope — ผ้า verlet ที่ลากและฉีกได้ | เมาส์ |
| 14 | Audio Reactive Forest — เสียงทำให้ป่าแสงโต | ไมค์ |

ทุกเดโมมีแผง **⚙ CONFIG** มุมซ้ายบน กดพับ/กางได้ ปรับค่าสดระหว่างสอน

## คีย์ลัด

| คีย์ | ทำอะไร |
|------|--------|
| `←` `→` | เปลี่ยนสไลด์ |
| `1`–`9` · `0` | ข้ามไปเดโม 1–10 |
| `H` | กลับหน้า Home |
| `F` | เต็มจอ |

## เปิดในเครื่อง

เดโมที่ใช้กล้อง/ไมค์ (03, 04, 05, 07, 08, 14) เบราว์เซอร์บล็อกบน `file://`
ต้องเสิร์ฟผ่าน localhost:

```
ดับเบิลคลิก START_LECTURE.bat
```

จะเปิด `http://localhost:8777/index.html` ให้เอง (ใช้ Python หรือ Node ตัวไหนก็ได้ที่มีในเครื่อง)
บน GitHub Pages ใช้ได้เลยเพราะเป็น HTTPS

ใช้ Chrome หรือ Edge — Speech Recognition (เดโม 04) ยังไม่รองรับใน Firefox/Safari

## หมายเหตุ

- เดโม 03 โหลดโมเดล MediaPipe จาก CDN ต้องต่อเน็ต
- เดโม 05 / 08 ถ้าโหลดโมเดลแยกร่างคนไม่ได้ จะถอยไปใช้โหมด "จับพื้นหลัง" อัตโนมัติ
- ตัวนับผู้เข้าชมใช้ `page-views-api.ratneshc.com` (ยอดรวมทุกเครื่อง ตัวเดียวกับเด็ค Immersive-Theme-Park)
  ถ้า API ล่มจะถอยไปใช้ป้าย hits.sh แล้วค่อย localStorage — ถ้าตกมาถึงขั้นสุดท้ายจริง ๆ ป้ายใต้ตัวเลขจะเขียนว่า “เครื่องนี้” ให้เห็นชัด
