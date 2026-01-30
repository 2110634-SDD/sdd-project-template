# STUDENT_SUMMARY.md  
Milestone 1 – Problem Understanding & High-Level Design

> **วัตถุประสงค์ของเอกสารนี้**  
> เอกสารนี้ใช้เพื่ออธิบายความเข้าใจในปัญหาและเหตุผลเบื้องหลังการออกแบบในระดับแนวคิด
> เน้นอธิบาย *เหตุผลในการตัดสินใจ (why)* ไม่ใช่รายละเอียดการ implement (how)

---

## 1. Problem Understanding & Scope

**ปัญหาที่ระบบพยายามแก้ไข**  
(อธิบายปัญหาหลักจากมุมมองของผู้ใช้ ไม่ต้องเล่าฉากหลังยาว)

> …

**ผู้ใช้หลักของระบบ (Primary users)**  
(ระบุว่าผู้ใช้หลักคือใคร และมีบทบาทอย่างไร)

> …

**ขอบเขตที่ไม่ครอบคลุม (Out of scope)**  
(ระบุอย่างน้อย 1 ประเด็นที่ตั้งใจ “ไม่ทำ” ในระบบนี้ เพื่อให้ขอบเขตชัดเจน)

> …

---

## 2. Key Use Cases

เลือก **2–3 use cases ที่สำคัญที่สุด** สำหรับระบบนี้  
(use case ที่ถ้าระบบล้ม จะส่งผลกระทบสูง)

สำหรับแต่ละ use case ให้อธิบาย:
- เป้าหมายของผู้ใช้คืออะไร
- เหตุผลที่ use case นี้ถือว่าสำคัญต่อระบบ

**Use Case 1:** `<ชื่อ use case>`  
- เหตุผลที่เป็น use case หลัก:  
  > …

**Use Case 2:** `<ชื่อ use case>`  
- เหตุผลที่เป็น use case หลัก:  
  > …

*(ถ้ามี)*  
**Use Case 3:** `<ชื่อ use case>`  
- เหตุผลที่เป็น use case หลัก:  
  > …

---

## 3. Quality Attribute Drivers

ระบุ **1–3 quality attributes** ที่มีผลต่อการตัดสินใจออกแบบระบบมากที่สุด  
(เช่น Performance, Availability, Security, Maintainability ฯลฯ)

สำหรับแต่ละ quality attribute ให้ระบุ:
- เหตุผลว่าทำไมจึงสำคัญกับระบบนี้
- อ้างอิง concrete quality attribute scenario ที่เขียนไว้
- trade-off ที่ยอมรับจากการเลือกคุณลักษณะนี้

**Quality Attribute 1:** `<ชื่อ quality attribute>`  
- เหตุผลที่สำคัญ:  
  > …
- Scenario ที่เกี่ยวข้อง:  
  > …
- Trade-off ที่ยอมรับ:  
  > …

**Quality Attribute 2 (ถ้ามี):** `<ชื่อ quality attribute>`  
- เหตุผลที่สำคัญ:  
  > …
- Scenario ที่เกี่ยวข้อง:  
  > …
- Trade-off ที่ยอมรับ:  
  > …

---

## 4. Conceptual Design Decisions

อธิบายแนวคิดในการออกแบบเชิงแนวคิด (conceptual design)  
โดยอ้างอิงจาก **conceptual class diagram** และกระบวนการ Streamlined Object Modeling

ให้เน้นอธิบาย:
- domain หลักของระบบถูกแบ่งเป็นแนวคิดใหญ่อะไรบ้าง
- class ใดเป็น class หลัก และทำหน้าที่อะไร
- เหตุผลในการกำหนดความรับผิดชอบให้กับ class เหล่านี้

**Class หลัก 1:** `<ชื่อ class>`  
- บทบาทตาม collaboration pattern:  
  > …
- ความรับผิดชอบหลัก (responsibility):  
  > …
- ความสัมพันธ์ที่สำคัญกับ class อื่น:  
  > …

**Class หลัก 2:** `<ชื่อ class>`  
- บทบาทตาม collaboration pattern:  
  > …
- ความรับผิดชอบหลัก (responsibility):  
  > …
- ความสัมพันธ์ที่สำคัญกับ class อื่น:  
  > …

*(ถ้ามี)*  
**Class หลัก 3:** `<ชื่อ class>`  
- บทบาทตาม collaboration pattern:  
  > …
- ความรับผิดชอบหลัก (responsibility):  
  > …
- ความสัมพันธ์ที่สำคัญกับ class อื่น:  
  > …

---

## 5. Modeling Process Reflection

ส่วนนี้ใช้เพื่อสะท้อนว่าได้ใช้กระบวนการ modeling ตามที่เรียนมาอย่างไร  
ไม่ต้องเขียนเป็นขั้นตอนละเอียด แต่ให้เห็นการตัดสินใจและเหตุผล

### Use Case Modeling
(สะท้อนการสร้างและปรับ use case model)

- ระบุ actor และ goal อย่างไร
- มี use case ใดที่รวม แยก หรือตัดออก พร้อมเหตุผล
- มี assumption ใดที่ใช้ในการออกแบบ

> - …
> - …
> - …

### Conceptual Modeling (Streamlined Object Modeling)
(สะท้อนการสร้าง conceptual class diagram)

- collaboration patterns ที่เลือกใช้
- จุดที่ตัดสินใจยากหรือไม่แน่ใจ
- แนวคิดหรือ class ที่ตั้งใจไม่ model และเหตุผล

> - …
> - …
> - …

---

## 6. Architectural Direction & Open Questions

อธิบายแนวทาง architecture ในระดับสูง  
(ยังไม่ต้องระบุ container, technology หรือ framework)

- แนวคิด architecture ที่คิดว่าเหมาะสมกับระบบ
- quality attributes ที่มีผลต่อแนวคิดนี้

> …

**ประเด็นหรือความเสี่ยงที่ต้องพิสูจน์ใน Milestone 2**  
(ระบุ 2–3 ข้อ)

- …
- …
- …

---

## References to Artefacts

ระบุไฟล์หรือ link ของ artefact ที่เกี่ยวข้อง  
(ไม่ต้องแปะ diagram ซ้ำในเอกสารนี้)

- Use case diagram:  
- Use case descriptions:  
- Conceptual class diagram:  
- C4 Context diagram:  

---
