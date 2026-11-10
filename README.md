# 📖 คู่มือการนำเว็บ One-Page นี้ขึ้น GitHub Pages

โฟลเดอร์นี้ประกอบด้วยหน้าเว็บคู่มือการใช้งาน **"ระบบขอข้อมูลและรายงาน โรงพยาบาลบุรีรัมย์"** ที่พร้อมสำหรับนำขึ้น **GitHub Pages** ได้ทันทีโดยไม่ต้องตั้งค่าเซิร์ฟเวอร์ใดๆ

---

## 📂 โครงสร้างไฟล์ในโฟลเดอร์นี้
* `index.html` — หน้าเว็บหลัก One-Page ดีไซน์แบบ Responsive รองรับทั้งคอมพิวเตอร์และมือถือ
* `images/` — รูปภาพประกอบจริงที่แคปเจอร์จากระบบ:
  * `step-intranet.png` — ภาพหน้าจออินทราเน็ต รพ. (แสดงตำแหน่งเมนู ขอข้อมูล/รายงาน)
  * `step-login.png` — ภาพหน้าจอเข้าสู่ระบบด้วยรหัส PM

---

## 🚀 ขั้นตอนการนำขึ้น GitHub Pages (ภายใน 2 นาที)

### ขั้นตอนที่ 1: สร้าง Repository บน GitHub
1. เข้าเว็บไซต์ [github.com](https://github.com/) และเข้าสู่ระบบ
2. กดปุ่มเครื่องหมาย **+** มุมขวาบน แล้วเลือก **New repository**
3. ตั้งชื่อ Repository เช่น: `brh-report-guide` (หรือชื่ออื่นที่ต้องการ)
4. เลือกเป็น **Public** *(จำเป็นสำหรับ GitHub Pages แผนฟรี)*
5. ไม่ต้องติ๊ก Add README file แล้วกดปุ่ม **Create repository**

---

### ขั้นตอนที่ 2: อัปโหลดไฟล์ขึ้น GitHub

สามารถเลือกทำได้ 2 วิธีตามสะดวกครับ:

#### วิธี A: ลากไฟล์วางผ่านหน้าเว็บ GitHub (ง่ายที่สุด)
1. ในหน้า Repository ที่เพิ่งสร้าง จะมีข้อความว่า *“…or upload an existing file”* ให้คลิกคำว่า **upload an existing file**
2. ลากไฟล์ `index.html` และโฟลเดอร์ `images` ทั้งหมดในโฟลเดอร์นี้ไปปล่อยลงในหน้าเว็บ
3. ด้านล่างพิมพ์ข้อความ เช่น `Initial commit` แล้วกด **Commit changes**

#### วิธี B: ใช้คำสั่ง Git ผ่าน Terminal / PowerShell
เปิด PowerShell ในโฟลเดอร์ `brh-guide` แล้วรันคำสั่ง:
```bash
git init
git add .
git commit -m "feat: initial brh report guide page"
git branch -M main
git remote add origin https://github.com/<username>/brh-report-guide.git
git push -u origin main
```
*(เปลี่ยน `<username>` เป็นชื่อผู้ใช้ GitHub ของคุณ)*

---

### ขั้นตอนที่ 3: เปิดใช้งาน GitHub Pages
1. ในหน้า Repository ของคุณ ให้คลิกที่แท็บ **Settings** (เมนูรูปฟันเฟืองด้านบน)
2. ที่แถบเมนูด้านซ้ายมือ ให้คลิกเลือก **Pages**
3. ในส่วนของ **Build and deployment**:
   * **Source:** เลือกเป็น `Deploy from a branch`
   * **Branch:** เลือก `main` (หรือ `master`) และช่องข้างๆ เลือกเป็น `/ (root)`
   * กดปุ่ม **Save**
4. รอประมาณ 1–2 นาที รีเฟรชหน้าจอจะเห็นกล่องสีเขียวแสดง URL ของเว็บไซต์ เช่น:
   ```
   https://<username>.github.io/brh-report-guide/
   ```

---

🎉 **เสร็จเรียบร้อย!** สามารถนำลิงก์ที่ได้ไปแชร์ในไลน์กลุ่มโรงพยาบาล แปะในหน้าอินทราเน็ต หรือส่งให้เจ้าหน้าที่เปิดดูคู่มือได้ทันทีครับ!
