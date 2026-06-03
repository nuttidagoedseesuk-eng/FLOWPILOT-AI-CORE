# Agent Specifications (Baby AI Ecosystem)

เอกสารฉบับนี้กำหนดสเปกและสถาปัตยกรรมของ **Specialized AI Agents (Baby AI)** ซึ่งเป็น AI หลายตัวที่ถูกออกแบบให้มีบุคลิกการทำงาน ความสามารถ และจุดอ่อนที่แตกต่างกันอย่างสิ้นเชิง เพื่อการทำงานเฉพาะทางในระบบ Multi-agent สมัยใหม่

## 📊 ตารางวิเคราะห์คุณลักษณะและความเสี่ยง (Agent Matrix)

| ตัวแทน (Baby AI) | ความถนัด (Strengths) | สิ่งที่ไม่ถนัด (Weaknesses) | ความเสี่ยงระบบ (System Risks) |
| :--- | :--- | :--- | :--- |
| **Inventory AI** | Stock movement, forecasting | เข้าใจอารมณ์คน | สั่งสินค้าซ้ำซ้อน / Reorder ผิด |
| **QC AI** | ตรวจ Defect, Image analysis | การตัดสินใจเชิงกลยุทธ์ (Strategic) | เกิดผลลวง (False Positive) |
| **Workforce AI**| ตรวจสอบรูปแบบ (Pattern) คนทำงาน | บริบทหน้างานที่ซับซ้อน | เกิดอคติจากอัลกอริทึม (Bias) |
| **Finance AI** | วิเคราะห์ต้นทุนและความเสี่ยง (Cost/Risk) | บริบทหรือสถานการณ์หน้างานจริง | ปรับแต่งระบบจนตึงตัวเกินไป (Over-optimization) |
| **Risk AI** | ตรวจจับสิ่งผิดปกติ (Anomaly detection) | เข้าใจความละเอียดอ่อนทางธุรกิจ (Business Nuance) | ส่งสัญญาณเตือนมากเกินไป (Alert เยอะเกิน) |
| **Logistics AI**| วางแผนเส้นทาง (Routing), ควบคุม SLA | สภาวะที่มีความไม่แน่นอน (Uncertainty) สูง | เกิดการแย่งหรือทับซ้อนเส้นทาง (Route conflict) |
| **Campaign AI** | บริหารโปรโมชัน (Promotion optimization) | ขีดความสามารถการปฏิบัติการ (Operation capacity) | ยอดซื้อพุ่งกระทันหัน (Demand spike) |

---

## ⚙️ แนวทางการควบคุมขอบเขต (Boundary Enforcement)
* Baby AI แต่ละตัวจะไม่มีสิทธิ์เข้าถึงหรือแก้ไขข้อมูลข้ามสายงาน (Cross-domain) โดยไม่ผ่านการตรวจสอบความถูกต้องของสัญญากลาง
* หากตรวจพบว่าสถานการณ์หน้างานตรงกับ **"สิ่งที่ไม่ถนัด (Weaknesses)"** ระดับสิทธิ์ในการตัดสินใจแบบอัตโนมัติ (Autonomy Level) จะต้องถูกจำกัดลงโดยทันที
* 
