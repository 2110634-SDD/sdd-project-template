# Milestone 1: Foundations – Problem Understanding & High-Level Design

Milestone นี้มุ่งเน้นการทำความเข้าใจปัญหาและการออกแบบระบบในระดับแนวคิด  
นิสิตจะต้องแสดงให้เห็นว่าเข้าใจ **บริบทของระบบ (system context)**  
**ผู้ใช้งาน (actors)** และ **ความสามารถหลักของระบบ (use cases)**  
ก่อนจะเข้าสู่การออกแบบเชิงสถาปัตยกรรมใน milestone ถัดไป

---

## วัตถุประสงค์ของ Milestone

เมื่อจบ Milestone 1 นิสิตควรสามารถ:

- อธิบายปัญหาและขอบเขตของระบบได้อย่างชัดเจน
- ระบุผู้ใช้งานหลัก (actors) และความสัมพันธ์กับระบบ
- สร้าง Use Case Model ที่สอดคล้องกับปัญหา
- เขียน Fully Dressed Use Case Descriptions สำหรับ use case หลัก
- ออกแบบระบบในระดับแนวคิด (conceptual level) โดยไม่ลงรายละเอียด implementation

---

## สิ่งที่ต้องส่ง (Deliverables)

ให้ส่งไฟล์ต่อไปนี้ใน repository:

```
milestone1/
├── INSTRUCTIONS.md (ห้ามแก้ไข - contract สำหรับ milestone1)
├── README.md
├── concrete-quality-attribute-scenarios.md
├── STUDENT_SUMMARY.md
├── use-case-descriptions/
│   ├── README.md
│   ├── UC01-<name>.md
│   ├── ...
│   └── UC*-<name>.md
└── diagrams/
    ├── README.md
    ├── use-case-diagram.png
    ├── use-case-diagram.puml
    ├── conceptual-class-diagram.png
    ├── conceptual-class-diagram.puml
    ├── system-context.png
    └── system-context.puml
```

> หมายเหตุ:  
> ไฟล์ `README.md` นี้มีไว้เพื่ออธิบาย milestone  
> ส่วนรายละเอียดการออกแบบให้เขียนในไฟล์ตามที่กำหนด
> Template บางไฟล์จะมีส่วนที่เป็นคำอธิบายจากอาจารย์ ให้แก้ไขเฉพาะส่วนที่ระบุว่า [Student Fill In]

---

## รายละเอียดของแต่ละ Deliverable

### 1. Use Case Diagram

- แสดง system boundary อย่างชัดเจน
- ระบุ actors ที่เกี่ยวข้องกับระบบ
- แสดง use case ในระดับ *user goal*
- ใช้สัญลักษณ์ตามมาตรฐาน UML

ไฟล์:  
- `diagrams/use-case-diagram.png`
- `diagrams/use-case-diagram.puml`

---

### 2. Use Case Descriptions

ไฟล์:  
- `use-case-descriptions/README.md`
  - สรุป

- `use-case-descriptions/UC*-<name>.md`

เนื้อหาที่ต้องมี:
- Fully Dressed Use Case Descriptions
- เลือกอย่างน้อย **2 use case หลัก**
- แต่ละ use case แยกเป็นไฟล์แยกกัน `UC*-<name>.md` ต้องมีองค์ประกอบให้ครบถ้วนตามบริบทของ use case นั้น:
  - Primary Actor
  - Stakeholders & Secondary Actors
  - Preconditions
  - Main Flows
  - Alternative / Exception / Extension Flows
  - Postconditions

> ❗ **ไม่ต้องอธิบายขั้นตอนการคิดหรือ process**  
> ให้ใส่เฉพาะผลลัพธ์สุดท้ายของ use case modeling

---

### 3. Conceptual Model

ไฟล์:  
- `diagrams/conceptual-class-diagram.png`
- `diagrams/conceptual-class-diagram.puml`
- `diagrams/README.md`

เนื้อหา:
- Diagram เป็น artifact หลักสำหรับ conceptual model
- คำอธิบายความหมายของแต่ละคลาส (สั้น ๆ) ให้เขียนแยกใน `diagrams/README.md`
- ใน diagram ไม่ต้องใส่ข้อความอธิบายเป็นประโยค
- แสดง conceptual classes ที่สำคัญในระบบ
- ความสัมพันธ์ระหว่าง classes (association, aggregation, etc.)
- ใส่ multiplicity ระหว่าง class ให้ถูกต้อง
- ใส่ stereotype ของแต่ละคลาสจาก collaboration pattern ที่เลือกใช้ เช่น <<role>>, <<transaction>>, <<follow-up transaction>> เป็นต้น
- มี core attributes ที่ define identity / meaning ของคลาส (ไม่ต้องใส่ datatype, technical field, foreign key, list ยาวๆ แบบ ER diagram)
- ไม่ต้องมี method หรือ implementation detail

อาจแนบ diagram เพิ่มได้ถ้าจำเป็น

---

### 4. Concrete Quality Attribute Scenarios

ไฟล์:  
- `concrete-quality-attribute-scenarios.md`

เนื้อหา:
- ระบุ quality attributes ที่สำคัญของระบบ (เช่น usability, performance, security)
- เขียน concrete quality attribute scenario ของแต่ละ quality attributes อธิบายในระดับ *ความคาดหวังเชิงพฤติกรรมของระบบ* ที่ *testable*, *measurable*
- ยังไม่จำเป็นต้องผูกกับ solution หรือ technology

---

### 5. C4 Diagram (Context Level Only)

ไฟล์:
- `diagrams/system-context.png`
- `diagrams/system-context.puml`

เนื้อหา:
- Context Diagram: แสดงระบบในมุมมองภาพรวมและระบบภายนอก
- System boundary ชัด
- Trace ได้กับ use cases
- ไม่ต้องทำ Container / Component diagram ใน milestone นี้

---

## สิ่งที่ **ไม่ควรทำ** ใน Milestone นี้

- ไม่ออกแบบเชิง implementation
- ไม่ระบุภาษา programming หรือ framework
- ไม่เขียน pseudo-code
- ไม่ออกแบบ database schema เชิงเทคนิค

---

## การนำเสนอ (Presentation)

ในวันนำเสนอ นิสิตต้องสามารถอธิบาย:

- ที่มาของ use cases
- เหตุผลในการเลือก use case หลัก
- การเชื่อมโยงระหว่าง problem → use case → conceptual model

> ขั้นตอนการทำ (process) ให้แสดงใน presentation  
> เอกสารที่ส่งควรเป็น **design artifact ที่สะอาดและพร้อมใช้งาน**
> เอกสารที่ส่งเป็นเกณฑ์หลักในการประเมิน
> การนำเสนอใช้เพื่ออธิบายเหตุผลและตรวจสอบความเข้าใจของทีม

---

## เกณฑ์การประเมินโดยสังเขป

- ความชัดเจนของ problem understanding
- ความสมเหตุสมผลของ use case model
- คุณภาพของ use case descriptions
- ความสอดคล้องระหว่างเอกสารแต่ละชิ้น
- การใช้ notation และคำศัพท์อย่างถูกต้อง

รายละเอียดคะแนนดูได้จาก `PROJECT_SPEC.md`

---

## Autograding (Informational)
บางส่วนของ milestone นี้จะถูกตรวจด้วย script อัตโนมัติ
เช่น โครงสร้างไฟล์และการตั้งชื่อ

---

## หมายเหตุเพิ่มเติม

Milestone นี้เป็นพื้นฐานสำคัญสำหรับ Milestone 2  
หากการออกแบบระดับแนวคิดยังไม่ชัด จะส่งผลต่อการออกแบบสถาปัตยกรรมในลำดับถัดไป


