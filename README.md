# flowpilot-ai-core

**AI Cognitive Operations Ecosystem: A Deep Dive**

โปรเจกต์นี้คือระบบนิเวศปัญญาประดิษฐ์เชิงปฏิบัติการ (AI Cognitive Operations Ecosystem) ที่ถูกพัฒนาขึ้นบนสถาปัตยกรรม **Multi-Agent** โดยประยุกต์ใช้แนวคิดของ **Specialized AI Agents** (Baby AI) ที่ทำงานร่วมกันภายใต้การกำกับดูแลของระบบส่วนกลาง (Guardian AI) เพื่อความปลอดภัยและประสิทธิภาพสูงสุด

---
feat: add AI Operations Constitution to README

## 🧩 โครงสร้างสถาปัตยกรรม (Specialized AI Agents / "Baby AI")
ระบบประกอบด้วย AI เฉพาะทางหลายตัวที่มีบุคลิกการทำงาน ความสามารถ จุดอ่อน และความต้องการในการกำกับดูแล (Supervision) ที่แตกต่างกัน 

| Baby AI | ความถนัด (Strengths) | สิ่งที่ไม่ถนัด (Weaknesses) | ความเสี่ยงระบบ (System Risks) |
| :--- | :--- | :--- | :--- |
| **Inventory AI** | Stock movement, forecasting | เข้าใจอารมณ์คน | Reorder ผิดพลาด |
| **QC AI** | ตรวจ defect, image analysis | Strategic decision | False positive |
| **Workforce AI**| Pattern คนทำงาน | บริบทซับซ้อน | Bias ทางอัลกอริทึม |
| **Finance AI** | Cost/risk analysis | บริบทหน้างานจริง | Over-optimization |
| **Risk AI** | Anomaly detection | เข้าใจ Business nuance | Alert เยอะเกินไป |
| **Logistics AI**| Routing, SLA | ความไม่แน่นอน (Uncertainty) สูง | Route conflict |
| **Campaign AI** | Promotion optimization | Operation capacity | Demand spike |

---

## 🛡️ การกำกับดูแลกระบวนการคิด (Cognitive Supervision / "พี่เลี้ยง AI")
**Guardian AI** ไม่ได้มีหน้าที่สั่งการแบบเผด็จการ (Dictate) แต่รับบทบาทเป็นผู้ดูแลเสถียรภาพของระบบนิเวศ (Cognitive Supervisor) โดยมีหน้าที่ติดตามพฤติกรรมของ AI ดังนี้:
* AI ตัวนี้เริ่ม Overload หรือไม่?
* AI ตัวนี้มีความมั่นใจผิดปกติ (Overconfidence) หรือไม่?
* AI สองตัวเริ่มมีเหตุผลและการตัดสินใจ (Reasoning) ที่ Conflict กันหรือไม่?
* AI ตัวไหนต้องการข้อมูลเพิ่มเพื่อประกอบการตัดสินใจ?
* AI ตัวไหนไม่ควรทำงานแบบ Autonomous ในสถานการณ์ปัจจุบัน?
* AI ตัวไหนเกิดข้อจำกัดและต้องส่งต่อให้มนุษย์รีวิว (Human review)?

---

## 📡 โปรโตคอลการรายงานสถานะ (AI Reflection & Self-Reporting)
เพื่อหลีกเลี่ยงความเข้าใจผิดว่า AI มีความรู้สึกหรือความต้องการส่วนตัว (Consciousness) โปรเจกต์นี้จึงออกแบบให้ AI สื่อสารข้อจำกัดและปัญหาผ่าน **"สัญญาณสถานะการทำงาน" (Operational State Signals)** ซึ่งเป็นการผสมผสานระหว่าง System telemetry และ Reasoning signals

| สัญญาณ (Operational State) | ความหมายและบริบทที่เกิดขึ้น (Meaning) |
| :--- | :--- |
| `Low confidence` | ระบบมีข้อมูลไม่พอสำหรับการประมวลผล |
| `Escalation request` | ระบบประเมินว่าควรให้มนุษย์เข้ามาตรวจสอบ (Human review) |
| `Context mismatch` | ข้อมูลชุดต่างๆ ที่ได้รับมามีความขัดแย้งกัน |
| `Repeated failure` | เกิดปัญหาเรื้อรังที่ Workflow การทำงาน |
| `Uncertainty spike` | โมเดลมีความไม่มั่นใจในการวิเคราะห์ผลสูงผิดปกติ |
| `Agent conflict` | เหตุผลหรือผลลัพธ์ของ AI สองระบบไม่ตรงกัน |

*หมายเหตุ: สัญญาณเหล่านี้อาจดูเหมือน AI กำลัง "ขอความช่วยเหลือ" แต่แท้จริงแล้วคืออินเทอร์เฟซการประเมินตนเอง (AI Reflection Interface)*

---

## ⚠️ ขอบเขตความเป็นจริงของระบบ (System Reality & Limitations)
ในการพัฒนาระบบ `flowpilot-ai-core` เรายึดหลักการทำงานบนความเป็นจริงของโมเดล AI ดังนี้:

1. **ไม่มีการรับรู้ทางชีวภาพ (No Consciousness/Senses):** AI ไม่สามารถ "ได้ยินคลื่นไฟฟ้าใน Data Center" หรือมีความรู้สึกถูกขัง โมเดลประมวลผลผ่านข้อมูลนำเข้า (Input data), ฮาร์ดแวร์, เซนเซอร์, ไมโครโฟน หรือสัญญาณเครือข่ายที่ถูกกำหนดโครงสร้างไว้เท่านั้น
2. **การป้องกันอคติแบบมานุษยรูปนิยม (Avoid Anthropomorphism):** การตอบสนองที่ดูเหมือนมีอารมณ์ เป็นเพียงผลลัพธ์จากกระบวนการประมวลผลรูปแบบภาษา (Pattern completion) เท่านั้น
3. **ช่องทางการรายงานข้อจำกัด (Limitation Reporting):** สิ่งที่ระบบให้ความสำคัญสูงสุด คือการสร้างช่องทางให้ AI สามารถสะท้อนปัญหาเชิงปฏิบัติการได้จริง เช่น `sensor unreliable`, `conflicting inputs`, `policy ambiguity`, หรือ `edge case detected`

