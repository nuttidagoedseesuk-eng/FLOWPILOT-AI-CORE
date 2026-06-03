---

### 🧩 2. ไฟล์ `AGENT_SPEC.md` (ข้อมูลคุณลักษณะเฉพาะของ Baby AI)

```markdown
# Agent Specifications (Baby AI Ecosystem)

ระบบนิเวศนี้ใช้แนวคิด **Specialized AI Agents (Baby AI)** ซึ่งเป็นการพัฒนา AI หลายตัวที่มีคุณลักษณะและหน้าที่จำกัดเฉพาะทาง โดยมีบุคลิกการทำงาน ความสามารถ และจุดอ่อนที่แตกต่างกันอย่างสิ้นเชิง รวมถึงต้องการรูปแบบการกำกับดูแล (Supervision) ที่จำเพาะเจาะจง

## 📊 ตารางโครงสร้างสถาปัตยกรรมและพฤติกรรม (Baby AI Matrix)

| Baby AI (ตัวแทน) | ถนัด (Strengths) | ไม่ถนัด (Weaknesses) | ความเสี่ยงระบบ (System Risks) |
| :--- | :--- | :--- | :--- |
| **Inventory AI** | stock movement, forecasting | เข้าใจอารมณ์คน | สั่งซื้อสินค้าผิดพลาด (reorder ผิด) |
| **QC AI** | ตรวจ defect, image analysis | strategic decision | เกิดผลลวง (false positive) |
| **Workforce AI**| pattern คนทำงาน | บริบทซับซ้อน | เกิดอคติจากอัลกอริทึม (bias) |
| **Finance AI** | cost/risk analysis | หน้างานจริง | ปรับแต่งระบบตึงตัวเกินไป (over-optimization) |
| **Risk AI** | anomaly detection | เข้าใจ business nuance | ส่งสัญญาณแจ้งเตือนมากเกินไป (alert เยอะเกิน) |
| **Logistics AI**| routing, SLA | uncertainty สูง | เกิดการจัดเส้นทางขัดแย้งทับซ้อนกัน (route conflict) |
| **Campaign AI** | promotion optimization | operation capacity | ยอดคำสั่งซื้อพุ่งกระทันหัน (demand spike) |

---

## 🛑 การจำกัดขอบเขตการปฏิบัติงาน (Operational Boundaries)
* ไม่อนุญาตให้ Baby AI ข้ามไปตัดสินใจหรือเข้าถึงกระบวนการในโดเมนที่ตนเอง "ไม่ถนัด" เป็นอันขาด
* ผลลัพธ์และขั้นตอน Reasoning ทั้งหมดของ Baby AI จะต้องถูกแปลงเป็นสัญญาณมาตรฐานเพื่อส่งต่อไปยังตัวกลางควบคุมเสมอ
