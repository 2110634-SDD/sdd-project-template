# Milestone 1: Problem Understanding & High-Level Design

> ไฟล์นี้ใช้เป็นคำอธิบายโครงสร้างและเนื้อหาของ Milestone 1  
> เพื่อช่วยให้ผู้อ่านเข้าใจว่าเอกสารแต่ละส่วนอยู่ที่ใดและควรอ่านอย่างไร  
> **ไม่ต้องอธิบายเหตุผลเชิงการออกแบบในไฟล์นี้**

---

## Overview [Student Fill In]

Milestone 1 มุ่งเน้นการทำความเข้าใจปัญหาและการออกแบบระบบในระดับแนวคิด  
โครงงานนี้เกี่ยวข้องกับปัญหาเกี่ยวกับ:  
- (อธิบายปัญหาโดยสรุป 2–3 บรรทัด)
- กลุ่มผู้ใช้งานหลักของระบบคือใคร
- เป้าหมายหลักของระบบในภาพรวม

---

## Contents

ส่วนนี้อธิบายว่าเอกสารและ diagram แต่ละชุดใน Milestone 1 มีหน้าที่อะไร

### 1. Use Case Modeling

- `diagrams/use-case-diagram.png`  
  Use case diagram แสดงขอบเขตของระบบ ผู้ใช้งานหลัก (actors)  
  และความสามารถของระบบในระดับ user goal

- `use-case-descriptions/`  
  โฟลเดอร์นี้ประกอบด้วย fully dressed use case descriptions  
  ของ use case หลักที่ระบบรองรับ โดยแยกเป็นไฟล์ตามแต่ละ use case

---

### 2. Conceptual Design

- `diagrams/conceptual-class-diagram.png`  
  Conceptual class diagram แสดงโครงสร้างเชิงแนวคิดของ domain  
  และความสัมพันธ์ระหว่าง conceptual classes ที่สำคัญ

- `diagrams/README.md`  
  คำอธิบายความหมายของ diagram และ conceptual classes  
  เพื่อช่วยให้เข้าใจ domain model ได้ชัดเจนขึ้น

---

### 3. Quality Attributes

- `concrete-quality-attribute-scenarios.md`  
  ระบุ quality attributes ที่สำคัญของระบบ  
  พร้อม concrete quality attribute scenarios ในระดับที่สามารถทดสอบและวัดผลได้

---

### 4. System Context

- `diagrams/system-context.png`  
  C4 context diagram แสดงภาพรวมของระบบ  
  ผู้ใช้งาน และระบบภายนอกที่เกี่ยวข้อง

---

## How to Read This Milestone

แนะนำให้ผู้อ่านเอกสาร Milestone 1 ตามลำดับดังนี้:

1. Use case diagram เพื่อเข้าใจขอบเขตของระบบและ actors
2. Use case descriptions เพื่อเข้าใจความสามารถหลักของระบบ
3. Conceptual class diagram เพื่อเข้าใจ domain model
4. Quality attribute scenarios เพื่อเข้าใจความคาดหวังเชิงคุณภาพของระบบ
5. System context diagram เพื่อเห็นภาพรวมของระบบใน environment จริง

---

## Notes

- ไฟล์นี้อธิบายเฉพาะ **ว่าเอกสารแต่ละส่วนคืออะไร**
- เหตุผลในการตัดสินใจทางการออกแบบ  
  (เช่น ทำไมเลือก use case นี้ หรือออกแบบ domain แบบนี้)  
  ให้เขียนไว้ใน `STUDENT_SUMMARY.md`
