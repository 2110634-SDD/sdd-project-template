# Milestone 0: Team & Project Setup

## วัตถุประสงค์ (Objective)

Milestone 0 มีเป้าหมายเพื่อเตรียมความพร้อมของทีมและสภาพแวดล้อมของโครงงานให้พร้อมสำหรับการทำงานตลอดภาคการศึกษา โดยเน้นที่

* การทำงานเป็นทีม
* การใช้ Git / GitHub เป็นเครื่องมือทำงานร่วมกัน
* ความเข้าใจในกติกาและกระบวนการของรายวิชา

> **หมายเหตุ:** Milestone นี้เป็นเงื่อนไขเบื้องต้นสำหรับการทำ milestone ถัดไป การตรวจจะดำเนินการด้วยระบบ **autograding 100%**

---

## งานที่นิสิตต้องทำ (Tasks)

> ส่วนนี้เป็น **คำสั่งเริ่มต้นของ assignment** สำหรับประกาศใน LMS โดยอธิบายขั้นตอนตั้งแต่รับงาน (accept assignment) จนถึงการส่ง Milestone 0
> ครอบคลุมทั้งกรณี **ยังไม่สร้างทีม** และ **สร้างทีมไปแล้ว**

---

### ภาพรวมขั้นตอนทั้งหมด (Overview)

1. Accept assignment บน GitHub Classroom
2. เข้าร่วมทีม (หรือสร้างทีม หากยังไม่มี)
3. Clone repository ลงเครื่อง
4. ตั้งค่า Git identity (name / email)
5. แก้ไขไฟล์ `TEAM.md` (แต่ละคนแก้ด้วย commit ของตนเอง)
6. Commit และ push ขึ้น GitHub
7. Pull เพื่อตรวจสอบว่า repo อยู่ในสถานะล่าสุด
8. ตรวจสอบความเรียบร้อย และถือว่าเป็นการส่ง Milestone 0

รายละเอียดของแต่ละขั้นตอนอธิบายอยู่ในหัวข้อ Submission Workflow ด้านล่าง

---

## Submission Workflow (Milestone 0)

> ส่วนนี้อธิบาย **ลำดับขั้นตอนมาตรฐาน** ตั้งแต่เริ่มรับงานบน GitHub Classroom จนถึงการส่ง Milestone 0
> นิสิตทุกคนควรทำตามลำดับนี้เพื่อลดปัญหาและให้การตรวจด้วย autograding เป็นไปอย่างถูกต้อง 

---

### Step 0: ตั้งค่า Git identity (ต้องทำก่อน commit ครั้งแรก)

สมาชิกทุกคนต้องตั้งค่า git name และ email ของตนเอง (หากเคยตั้งค่าแล้ว สามารถข้ามขั้นตอนนี้ได้)

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

ตรวจสอบค่าที่ตั้งไว้:

```bash
git config --global --list
```

> Email ที่ตั้งตรงนี้ ต้องตรงกับค่า `Commit Email` ที่จะกรอกใน `TEAM.md`

---

### Step 1: Accept Assignment ผ่าน myCourseVille (ทุกคนต้องทำ)

* เข้า myCourseVille และเปิดรายวิชานี้
* ไปที่ assignment: **Milestone 0**
* คลิกลิงก์ GitHub Classroom ที่แนบไว้ใน myCourseVille
* กด **Accept Assignment**
* ระบบจะพาไปขั้นตอนเลือกทีมหรือสร้างทีม

---

### Step 2: เลือกทีม หรือสร้างทีมใหม่

* หากมีทีมอยู่แล้ว → เลือกทีมที่มีอยู่
* หากยังไม่มีทีม → ตัวแทนกลุ่มสร้างทีมใหม่

  * ตั้งชื่อทีมเป็นภาษาอังกฤษ (ห้ามใช้ภาษาไทย)

> การสร้างหรือเข้าร่วมทีมจะเกิดขึ้นในขั้นตอน Accept Assignment เท่านั้น

---

### Step 3: สมาชิกทุกคนเข้าร่วมทีมให้ครบ

* สมาชิกที่ยังไม่ได้อยู่ในทีม:

  * เข้า link assignment เดิมอีกครั้ง
  * เลือกทีมที่ตัวแทนสร้างไว้
* ตรวจสอบว่าเห็น repository ของทีมใน GitHub account ของตนเองแล้ว

---

### Step 4: Repository ของทีมถูกสร้างและตั้งค่าเป็น private

* GitHub Classroom จะสร้าง repository ให้โดยอัตโนมัติ
* Repository จะถูกตั้งค่าเป็น **private** ตลอดรายวิชา
* นิสิตไม่ต้องตั้งค่า repository เองในขั้นตอนนี้

---

### Step 5: Clone repository ของทีมลงเครื่อง (ทำครั้งแรก)

สมาชิกทุกคน clone repository ของทีมลง local machine

```bash
git clone <repository-url>
cd <repository-name>
```

### Step 5.5: ไฟล์ .gitignore (มีให้แล้ว)

- Repository นี้มีไฟล์ .gitignore เตรียมไว้ให้แล้ว ห้ามลบหรือแก้ไขไฟล์นี้ 
- ระบบจะตรวจว่ามีไฟล์ .gitignore อยู่ที่ root ของ repository ตลอด Milestone 0
- ไม่จำเป็นต้อง commit หรือแก้ไขไฟล์นี้ใน Milestone 0
หมายเหตุ: Milestone 0 ไม่มีการให้คะแนน และตรวจด้วยระบบ autograding 100%

---

### Step 6: ตัวแทนกลุ่มแก้ไข `TEAM.md` ก่อน

ตัวแทนกลุ่มเป็นผู้เริ่มต้นกรอกข้อมูลในไฟล์ `TEAM.md`

* Team Name
* Project Topic
* Project Description
* ข้อมูลของตนเองในตาราง Team Members

```bash
git add TEAM.md
git commit -m "Add initial team information"
git push origin main
```

> ขั้นตอนนี้ช่วยลดปัญหา merge conflict ในทีม

---

### Step 7: สมาชิกที่เหลือ pull และแก้ไขข้อมูลของตนเอง

สมาชิกคนอื่น ๆ ให้ทำตามขั้นตอนนี้ทีละคน

```bash
git pull origin main
```

* เติมข้อมูลของ **ตนเองเท่านั้น** ในตาราง Team Members

```bash
git add TEAM.md
git commit -m "Add my information to TEAM.md"
git push origin main
```

---

### Step 8: ตรวจสอบความเรียบร้อยของทีม

ก่อนใส่ tag `M0` ให้ทีมตรวจสอบตาม checklist นี้ให้ครบถ้วน

- [ ] Repository เป็น **private**
- [ ] มีไฟล์ `TEAM.md` อยู่ที่ root ของ repository
- [ ] ข้อมูลใน `TEAM.md` กรอกครบถ้วนทุกคน
- [ ] สมาชิกทุกคนมีอย่างน้อย 1 commit ของตนเอง
- [ ] Commit email ของแต่ละคน ตรงกับค่า `Commit Email` ใน `TEAM.md`
- [ ] มีไฟล์ `.gitignore` อยู่ที่ root ของ repository

> Checklist นี้สอดคล้องกับสิ่งที่ระบบ **autograding** ใช้ตรวจใน Milestone 0

---

### Step 9: ใส่ tag `M0` (ทำครั้งเดียวโดยใครก็ได้ในทีม)

เมื่อทีมตรวจสอบเรียบร้อยแล้ว ให้ใส่ tag เพื่อระบุว่าพร้อมส่ง Milestone 0
แนะนำให้ตกลงกันในทีมว่าใครเป็นผู้ใส่ tag

```bash
git tag M0
git push origin M0
```

---

### Step 10: การตรวจด้วย autograding และสถานะใน myCourseVille

* **ไม่ต้องอัปโหลดไฟล์ใด ๆ ใน myCourseVille**
* myCourseVille ใช้สำหรับ:

  * ประกาศ assignment
  * แนบลิงก์ GitHub Classroom
  * แจ้งสถานะ/ผลการตรวจ (ถ้ามี)
* ระบบจะตรวจจาก GitHub repository โดยตรง (autograding 100%)

ผลการตรวจ:

* หาก autograding **ผ่าน** → Milestone 0 เสร็จสมบูรณ์
* หาก autograding **ไม่ผ่าน**:

  * ตรวจสอบ error ที่ระบบรายงาน
  * แก้ไขให้ถูกต้อง
  * commit และ push ใหม่

> ไม่จำเป็นต้องสร้าง tag ใหม่

---

## Autograding Summary (Milestone 0)

ระบบ autograding ตรวจเฉพาะ ความถูกต้องของโครงสร้างและกระบวนการทำงาน ไม่ประเมินคุณภาพแนวคิดหรือการออกแบบเชิงเทคนิคของโครงงาน 
การไม่ผ่านหมายถึงขั้นตอนบางอย่างยังไม่ถูกต้อง ให้แก้ไขและ push ใหม่จนกว่าจะผ่าน