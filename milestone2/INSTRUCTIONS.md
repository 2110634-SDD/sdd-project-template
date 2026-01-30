# Milestone 2: Architectural Checkpoint – The Walking Skeleton  
**(Live Demo: สัปดาห์ที่ 13)**

Milestone นี้มีเป้าหมายเพื่อ **พิสูจน์ว่าสถาปัตยกรรมที่ออกแบบไว้สามารถทำงานได้จริง**  
ผ่านการพัฒนาฟังก์ชันหลัก 1 ฟังก์ชันให้ทำงานได้ครบวงจร (End-to-End)

แนวคิดสำคัญของ Milestone นี้คือ **Walking Skeleton**  
ระบบต้อง “เดินได้” ทั้งระบบ แม้จะยังทำได้เพียง use case เดียว

---

## วัตถุประสงค์ของ Milestone

เมื่อจบ Milestone 2 นิสิตควรสามารถ:

- แสดงให้เห็นว่าสถาปัตยกรรมระดับสูงที่ออกแบบไว้สามารถนำไปใช้จริงได้
- เชื่อมโยงระบบตั้งแต่ Client → Backend → Persistence → Client ได้ครบวงจร
- แสดงโครงสร้างโค้ดที่สะท้อนการตัดสินใจเชิงออกแบบ (architectural decisions)
- ใช้ CI/CD Pipeline เพื่อยืนยันคุณภาพพื้นฐานของระบบโดยอัตโนมัติ
- อธิบายการออกแบบเชิงลึกของ use case ที่นำมาทำ demo ได้อย่างเป็นระบบ

---

## สิ่งที่ต้องส่ง (Deliverables)

### 1. Live Demo (ในชั้นเรียน)

- สาธิต **1 Use Case หลัก** ให้ทำงานได้ครบ End-to-End  
  (เช่น Mobile App → Backend → Database → Mobile App)
- ระบบต้องสามารถ build และรันได้จริง

---

### 2. Source Code พร้อม CI/CD Pipeline

- Source code ของระบบ (ภาษาหรือ framework ใดก็ได้)
- ต้องมี CI/CD Pipeline ที่ทำงานอัตโนมัติ เช่น:
  - `.gitlab-ci.yml`  
  - หรือไฟล์ใน `.github/workflows/`
- Pipeline ต้องอย่างน้อย:
  - Build ได้สำเร็จ
  - รัน test หรือ static check บางอย่างได้

---

### 3. เอกสารในโฟลเดอร์ `milestone2/`

#### โครงสร้างไฟล์ที่กำหนด (Required Structure)

เพื่อให้การตรวจและการประเมินผลเป็นไปในแนวทางเดียวกัน  
นิสิตต้องจัดโครงสร้างไฟล์ภายใน `milestone2/` ดังนี้:

```
milestone2/
├── README.md
├── detailed-design.md
├── diagrams/
│   ├── sequence-diagram.png
│   ├── refined-class-diagram.png
│   ├── sequence-diagram.puml        
│   └── refined-class-diagram.puml   
```

**ข้อกำหนดสำคัญ**

* Diagram ทั้งหมดที่อ้างอิงใน `detailed-design.md` **ต้องอยู่ภายใต้โฟลเดอร์ `milestone2/diagrams/`**
* Diagram ทุกภาพควรมีไฟล์ต้นฉบับในรูปแบบ `.puml` เพื่อให้สามารถตรวจสอบและปรับปรุงได้
* ชื่อไฟล์สามารถแตกต่างได้เล็กน้อย แต่ต้องสื่อความหมายชัดเจนและอ้างอิงถูกต้องในเอกสาร

---

### 4. Detailed Design Document

ไฟล์:

* `milestone2/detailed-design.md`

เนื้อหาที่ต้องมี:

#### 4.1 Selected Use Case

* ระบุ use case ที่เลือกมาทำ Walking Skeleton
* เชื่อมโยงกับ use case จาก Milestone 1

#### 4.2 Sequence Diagram

* แสดง interaction ระหว่าง:

  * Client
  * Backend components
  * Persistence / External systems (ถ้ามี)
* แสดง flow หลักของ use case ที่นำมาทำ demo
* สอดคล้องกับโค้ดที่พัฒนา

#### 4.3 Refined Class Diagram

* แสดงโครงสร้าง class ที่เกี่ยวข้องกับ use case ที่เลือก
* แสดงความสัมพันธ์ที่สะท้อนการออกแบบจริง
* เริ่มเห็น layer / responsibility ชัดเจนขึ้น
* **ยังไม่จำเป็นต้องครอบคลุมทั้งระบบ**

> หมายเหตุ:
> Diagram ใน Milestone นี้ควรสะท้อน *implementation-oriented design*
> มากกว่า conceptual model ใน Milestone 1 แต่ยังไม่ต้องลงรายละเอียดระดับ low-level ทุกจุด

---

### 5. README.md ของ Milestone 2

ไฟล์:

* `milestone2/README.md`

ควรประกอบด้วย:

* สรุปเป้าหมายของ Milestone นี้
* ระบุ use case ที่เลือกมาทำ demo
* อธิบายภาพรวมของ Walking Skeleton
* Link ไปยัง:

  * `detailed-design.md`
  * diagram ที่สำคัญ
  * path ของ source code ที่เกี่ยวข้องโดยสังเขป

README.md นี้ทำหน้าที่เป็น **entry point สำหรับ reviewer**

---

### 6. Git Tag

* ให้ติดป้าย (tag) commit สุดท้ายของการส่งงานว่า:

```
v2.0-M2
```

---

## สิ่งที่ต้องนำเสนอ (Presentation Focus)

ในการนำเสนอ นิสิตต้องสามารถอธิบาย:

### 1. Live Demo

* สาธิต use case ที่เลือกให้ทำงานได้จริงแบบ End-to-End

### 2. CI/CD Demo

* แสดงผลการทำงานของ CI Pipeline
* เห็นสถานะ build / test ผ่าน (เช่น เครื่องหมายถูกสีเขียว)

### 3. Code Walkthrough

* อธิบายโค้ดในส่วนที่สะท้อนการตัดสินใจเชิงออกแบบ เช่น:

  * การแบ่ง layer
  * การใช้ design pattern
  * การจัด responsibility ของ component

---

## เกณฑ์การประเมิน (15% ของคะแนนรวม)

| รายการประเมิน                                   | น้ำหนัก |
| ----------------------------------------------- | :-----: |
| 1. การทำงานและความสมบูรณ์ของ Walking Skeleton   |   40%   |
| 2. คุณภาพของการออกแบบรายละเอียดและโค้ดเบื้องต้น |   40%   |
| 3. การสาธิตและการอธิบายเชิงเทคนิค               |   20%   |

รายละเอียดเพิ่มเติมดูได้จาก `GRADING_RUBRIC.md`

---

## สิ่งที่ไม่คาดหวังใน Milestone นี้

* ระบบที่ feature ครบถ้วน
* UI ที่สมบูรณ์หรือสวยงาม
* Performance optimization เชิงลึก
* Full test coverage

> เป้าหมายของ Milestone นี้คือ
> **“พิสูจน์โครงสร้างและทิศทางของระบบ” ไม่ใช่ “สร้างระบบเสร็จสมบูรณ์”**

---

## หมายเหตุเพิ่มเติม

Milestone 2 เป็นจุดตรวจสำคัญก่อนเข้าสู่การพัฒนาระบบเต็มรูปแบบใน Milestone 3
ปัญหาด้านโครงสร้างหรือสถาปัตยกรรมที่ไม่ชัดเจนในขั้นนี้
จะส่งผลกระทบอย่างมากต่อความสามารถในการขยายระบบในขั้นถัดไป

```

---

