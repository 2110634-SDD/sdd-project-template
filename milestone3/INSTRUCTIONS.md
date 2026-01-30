# Milestone 3: Final Product & Project Portfolio
**Final Demo & Submission**

Milestone นี้เป็นขั้นตอนสุดท้ายของโครงงาน  
มุ่งเน้นการส่งมอบ **ระบบที่สมบูรณ์ในระดับที่เหมาะสมกับรายวิชา**  
พร้อมแสดงคุณภาพของการออกแบบ การพัฒนา และการเรียนรู้ตลอดทั้งโครงงาน

---

## วัตถุประสงค์ของ Milestone

เมื่อจบ Milestone 3 นิสิตควรสามารถ:

- ส่งมอบระบบที่ฟังก์ชันหลักทำงานได้ครบถ้วนและมีความเสถียร
- แสดงให้เห็นว่า Architecture ที่เลือกใน Milestone 2 สามารถรองรับระบบโดยรวมได้
- ปรับปรุงคุณภาพโค้ดและโครงสร้างระบบจาก iteration ก่อนหน้า
- อธิบายเหตุผลเชิงวิศวกรรมซอฟต์แวร์ของการตัดสินใจที่สำคัญ
- สะท้อนการเรียนรู้และประสบการณ์จากโครงงานอย่างมีวิจารณญาณ

---

## แนวคิดหลักของ Milestone นี้

- **Milestone 2:** พิสูจน์ว่า *สถาปัตยกรรมทำงานได้จริง* (Walking Skeleton)
- **Milestone 3:** แสดงว่า *สถาปัตยกรรมนั้นรองรับระบบที่สมบูรณ์ได้*

> Milestone นี้ **ไม่ใช่การเริ่มต้นใหม่**  
> แต่เป็นการ **ขยาย + ปรับปรุง + ทำให้เสร็จสมบูรณ์**

---

## สิ่งที่ต้องส่ง (Deliverables)

### 1. Final Product (Working System)

- ระบบต้องพัฒนาต่อยอดจาก Milestone 2
- ฟังก์ชันหลักของระบบต้องทำงานได้ครบถ้วน
- ระบบต้องสามารถ:
  - build ได้จาก repository
  - run ได้ตามวิธีที่ระบุใน `README.md`

---

### 2. Source Code (Final Version)

- โค้ดทั้งหมดของระบบ
- โครงสร้างสอดคล้องกับ Architecture ที่ออกแบบไว้
- มีการปรับปรุงคุณภาพโค้ดจาก Milestone ก่อนหน้า (refactoring)
- CI/CD Pipeline ต้องยังคงทำงานได้

---

### 3. เอกสารในโฟลเดอร์ `milestone3/`

โครงสร้างที่แนะนำ:

```

milestone3/
├── README.md
├── architecture-summary.md
├── diagrams/
│   ├── c4-container.png
│   ├── c4-container.puml
│   ├── c4-component.png (ถ้ามี)
│   ├── c4-component.puml (ถ้ามี)
│   └── README.md
└── reflection/
    ├── individual-reflection-<student-id>.md

```

#### 3.1 `milestone3/README.md`
- สรุปสถานะสุดท้ายของระบบ
- ระบุ:
  - ระบบทำอะไรได้แล้ว
  - ขอบเขตที่ทำสำเร็จ
  - ข้อจำกัดที่ยังมีอยู่

---

#### 3.2 Architecture Summary

ไฟล์: `architecture-summary.md`

เนื้อหา:
- สรุป Architecture ของระบบโดยรวม
- เชื่อมโยง:
  - Context Diagram
  - Container Diagram
  - โครงสร้างระบบจริง
- อธิบายการเปลี่ยนแปลงจาก Milestone 2 (ถ้ามี)

---

#### 3.3 Diagrams

โฟลเดอร์: `milestone3/diagrams/`

- C4 Container Diagram (จำเป็น)
- C4 Component Diagram (ถ้ามี)
- Diagram ต้องสอดคล้องกับโค้ดจริง
- Diagram ทุกภาพควรมีไฟล์ต้นฉบับในรูปแบบ `.puml` เพื่อให้สามารถตรวจสอบและปรับปรุงได้

ไฟล์ `README.md` ในโฟลเดอร์นี้ควรอธิบาย:
- diagram แต่ละรูปใช้สื่ออะไร
- scope ของ diagram
- สิ่งที่ diagram นี้ *ตั้งใจไม่แสดง*

---

#### 3.4 Individual Reflection

โฟลเดอร์: `milestone3/reflection/`

ไฟล์: `individual-reflection-<student-id>.md`

เนื้อหาที่ต้องมี:
- บทบาทของตนเองในโครงงาน
- สิ่งที่ได้เรียนรู้ด้าน software design & development
- การตัดสินใจที่ยากหรือสำคัญ
- สิ่งที่ทำได้ดี และสิ่งที่ควรทำให้ดีกว่านี้ในอนาคต

> Reflection เป็นรายบุคคล  
> ไม่ใช่สรุปผลงานของทีม

---

### 4. Root README.md (Final Version)

`README.md` ที่ root ของ project ต้อง:

- เป็น entry point สำหรับผู้ใช้งาน / ผู้ตรวจ
- อธิบาย:
  - โครงงานคืออะไร
  - ระบบทำอะไรได้
  - วิธี run ระบบในระดับสูง
  - โครงสร้าง repository โดยสังเขป

---

### 5. Git Tag

- ติดป้าย (Tag) commit สุดท้ายเป็น  
  **`v3.0-final`**

---

## การนำเสนอ (Final Presentation)

ในการนำเสนอ นิสิตต้องสามารถ:

- Demo ระบบในภาพรวม
- อธิบายโครงสร้างและสถาปัตยกรรมของระบบ
- เชื่อมโยงการพัฒนาจาก:
  - Problem → Design → Architecture → Implementation
- สรุปบทเรียนที่ได้จากโครงงาน

---

## สิ่งที่ **ไม่คาดหวัง** ใน Milestone นี้

- ระบบระดับ production
- Feature ครบทุก edge case
- Optimization เชิง performance ขั้นสูง

> สิ่งที่คาดหวังคือ  
> **ระบบที่ออกแบบอย่างมีเหตุผล พัฒนาอย่างเป็นระบบ และอธิบายได้**

---

## เกณฑ์การประเมินโดยสังเขป

รายละเอียดคะแนนดูได้จาก `GRADING_RUBRIC.md`

การประเมินจะพิจารณาจาก:
- ความสมบูรณ์และเสถียรภาพของผลิตภัณฑ์
- คุณภาพของโครงสร้างระบบและโค้ด
- การสะท้อนการเรียนรู้และการนำเสนอ

---

