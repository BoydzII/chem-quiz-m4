# ⚗️ คลังโจทย์เคมี ม.4 (Chemistry Grade 10 Question Bank)

เว็บแอปพลิเคชันแบบ **Single-file HTML** สำหรับสร้างแบบฝึกหัดเคมี ม.4, ตรวจคำตอบแบบละเอียด 7 ขั้นตอน (Scaffolding Engine), บันทึกสถิติลงเครื่อง และส่งออกเป็นเอกสาร PDF

---

## 🚀 ฟีเจอร์หลัก
- **Single-file Architecture**: ไฟล์เดียว (`index.html`) ทำงานได้ทันที ไม่ต้องติดตั้งโปรแกรมหรือพึ่งพาเซิร์ฟเวอร์ภายนอก
- **7-Step Scaffolding Engine**: แสดงวิธีทำและเฉลยละเอียด 7 ขั้น (วิเคราะห์โจทย์, สิ่งที่กำหนด, หลักการ/สูตร, จัดรูปสมการ, แทนค่า, คำนวณ, สรุปคำตอบ)
- **Stoichiometry & Mole Engine**: สุ่มตัวเลขและสารเคมีอัตโนมัติ คำตอบเลขสวย คิดง่ายตามหลักเคมี
- **Offline First**: บันทึกสถานะการทำแบบฝึกหัดลงใน `localStorage` อัตโนมัติ ป้องกันข้อมูลสูญหาย
- **Cloud Sync Ready**: รองรับการเชื่อมต่อ Google Sheets ผ่าน Google Apps Script สำหรับห้องเรียน

---

## 📂 โครงสร้างบทเรียนเคมี ม.4
1. ความปลอดภัยและทักษะในปฏิบัติการเคมี
2. อะตอมและตารางธาตุ
3. พันธะเคมี
4. โมลและสูตรเคมี
5. สารละลาย
6. ปริมาณสารสัมพันธ์

---

## 🌐 วิธีนำขึ้น GitHub & GitHub Pages (เปิดเป็นเว็บไซต์ฟรี)

### วิธีที่ 1: ผ่านหน้าเว็บ GitHub (ง่ายที่สุด ไม่ต้องพิมพ์คำสั่ง)
1. ไปที่ [github.com/new](https://github.com/new) เพื่อสร้าง Repository ใหม่ (ตั้งชื่อเช่น `chem-quiz-m4` และเลือกเป็น **Public**)
2. กด **uploading an existing file** แล้วลากไฟล์ `index.html` ขึ้นไป แล้วกด **Commit changes**
3. ไปที่เมนู **Settings** > **Pages**
4. ในส่วน **Branch** เลือก `main` หรือ `master` โฟลเดอร์ `/ (root)` แล้วกด **Save**
5. รอ 1-2 นาที คุณจะได้ลิงก์เว็บไซต์ เช่น `https://<username>.github.io/chem-quiz-m4/` ส่งให้นักเรียนเปิดใช้งานได้ทันที!

---

### วิธีที่ 2: ผ่าน Git / GitHub CLI ในเครื่อง
เปิด PowerShell ในโฟลเดอร์นี้ แล้วรัน:
```bash
# 1. ล็อกอิน GitHub (ถ้ายังไม่ได้ล็อกอิน)
gh auth login

# 2. สร้าง repository และ push ขึ้น GitHub
gh repo create chem-quiz-m4 --public --source=. --push

# 3. เปิดใช้งาน GitHub Pages
gh repo edit --enable-pages --pages-branch main
```
