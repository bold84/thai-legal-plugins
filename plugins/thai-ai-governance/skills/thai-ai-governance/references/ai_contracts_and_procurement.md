# ai_contracts_and_procurement.md — ข้อสัญญา AI และการจัดซื้อของรัฐ/CII

อ่านไฟล์นี้เมื่อซื้อ/ขาย AI ตรวจผู้ขาย ข้อสัญญา no-training/ความรับผิด หรือเสนอรัฐ/CII

ข้อมูล ณ 9 ตุลาคม 2569 (2026) — ข้อสัญญาเป็น **ข้อเสนอให้ต่อรอง** ไม่ใช่ตัวบท สัญญาควบคุม/localisation [D11] เป็น **ร่าง — ยังไม่มีผลใช้บังคับ** และมีขอบเขตรัฐ/CII ไม่ใช่ AI ทุก B2B ตรวจข้อสัญญาไม่เป็นธรรม [L6]/คลาวด์ [L11] วันนี้ รหัส/URL ใน `key_sections.md`

---

## สารบัญ
1. การเลือกผู้ขายและ annex
2. ข้อสัญญาสองภาษา
3. ความถูกต้องและการจำกัดความรับผิด
4. การจัดซื้อรัฐ/CII
5. เกณฑ์ก่อนลงนาม

## 1. การเลือกผู้ขายและ annex

ขอรุ่นบริการ/โมเดล ผู้รับช่วง data flow (inference/training/log/backup/support) สิทธิ no-training/retention ผลทดสอบ security/incident/change contacts [G4–G6, G12] “enterprise” ไม่พิสูจน์ว่าข้อมูลอยู่ไทย

| Annex | เนื้อหาที่ต้องตกลง |
|---|---|
| AI scope | งาน/รุ่น ภาษา ผู้ใช้ intended use และ prohibited use; ผู้รับผิดชอบ human oversight |
| Data schedule | input/output/RAG/embeddings/log/feedback วัตถุประสงค์ ผู้เข้าถึง/ผู้รับช่วง ที่ตั้งและ retention |
| Test/acceptance | ชุดทดสอบมีสิทธิ เกณฑ์รับตามงาน ผลเสียสำคัญ re-test เมื่อเปลี่ยนและ remedy เมื่อไม่ผ่าน |
| Operations | SLA version/change notice rollback incident escalation export/exit และสิ่งที่ต้องคงหลังจบ |

DPA/โอน: `thai-pdpa`; IP: `thai-copyright-software`; สัญญาทั่วไป/ลงนาม: `thai-contract-master` ให้ annex AI สอดคล้องทั้งสัญญา

## 2. ข้อสัญญาสองภาษา

### 2.1 ใช้ข้อมูลเฉพาะบริการ / ไม่ใช้ฝึก

```text
ผู้ให้บริการและผู้รับช่วงจะใช้ข้อมูลของลูกค้า อินพุต ผลลัพธ์ ข้อมูล RAG
embeddings และ feedback เฉพาะเพื่อให้บริการที่กำหนดในเอกสารขอบเขตงาน
ห้ามนำไปฝึก ปรับแต่ง ประเมิน หรือพัฒนาโมเดลเพื่อประโยชน์อื่น หรือใช้ร่วมกับ
ลูกค้ารายอื่น เว้นแต่ได้รับอนุมัติเป็นหนังสือล่วงหน้าตามขั้นตอนที่ตกลง
log เพื่อความปลอดภัยใช้ได้เฉพาะขอบเขตและระยะเก็บใน Data Schedule
ผู้ให้บริการต้องกำหนดหน้าที่เดียวกันแก่ผู้รับช่วงและแสดงหลักฐานการตั้งค่า

The Provider and its subprocessors shall use Customer Data, inputs, outputs,
RAG data, embeddings and feedback solely to deliver the Services specified
in the Statement of Work. They shall not use such data to train, fine-tune,
evaluate or develop models for other purposes or for other customers without
prior written approval under the agreed process. Security logs may be used
only within the scope and retention period in the Data Schedule.
The Provider shall impose equivalent obligations on subprocessors and provide
evidence of the relevant settings.
```

หมายเหตุ: ผู้ให้บริการที่นำข้อมูลของลูกค้าไปฝึก/เฟรชโมเดลของตนเองเพื่อวัตถุประสงค์ของตน เปลี่ยนสถานะเป็นผู้ควบคุมข้อมูลส่วนบุคคลอีกรายหนึ่ง (แนวปฏิบัติ AI สคส. v1.0 บทสรุปผู้บริหาร ข้อ 2 [G12]; PDPA ม.6 นิยามตามอำนาจตัดสินใจ; ม.40(1) ผู้ประมวลผลผูกพันตามคำสั่ง [L2])

นิยามให้ครอบคลุม telemetry/human review; จำกัด fraud/security ไม่เปิดทาง training ซ่อน การอนุมัติไม่แทนฐาน PDPA/สิทธิภายนอก

### 2.2 ความลับและการคืน/ลบ

```text
ข้อมูล โมเดล prompt เอกสารและผลลัพธ์ที่ระบุเป็นความลับจะเข้าถึงได้เฉพาะ
ผู้จำเป็นเพื่อบริการ ห้ามใส่ในเครื่องมือภายนอกที่ไม่ได้อนุมัติ
เมื่อสิ้นสุด ให้คืน/ลบตาม Data Schedule รวมผู้รับช่วงและสำเนาสำรอง
หากกฎหมายหรือ legal hold กำหนดให้เก็บ ให้แยกเก็บ จำกัดการใช้ และแจ้งฐาน
เท่าที่กฎหมายอนุญาต พร้อมหลักฐานการปฏิบัติหลังพ้นเหตุให้เก็บ

Confidential data, models, prompts, documentation and outputs may be accessed
only by persons who need them to provide the Services, and shall not be
submitted to unapproved external tools. On termination, return or deletion,
including subprocessor copies and backups, shall follow the Data Schedule.
Data required by law or a legal hold shall be segregated and its use restricted.
The legal basis shall be notified to the extent permitted by law, with evidence
of completion when the retention requirement ends.
```

### 2.3 สิทธิในผลลัพธ์และส่วนเดิม

```text
คู่สัญญาจะแยกสิทธิในทรัพย์สินเดิม โมเดล/ซอฟต์แวร์ที่ให้บริการ ข้อมูลลูกค้า
และผลลัพธ์ตาม IP Schedule ผู้ให้บริการให้/โอนสิทธิในผลลัพธ์เท่าที่มีสิทธิ
ให้ได้ตามกฎหมาย โดยไม่รับรองว่าผลลัพธ์ AI ทุกชิ้นเกิดลิขสิทธิ์หรือเป็นเอกสิทธิ์
ภาระตรวจสิทธิบุคคลภายนอก การป้องกันคดี และการเยียวยาเป็นไปตาม [ข้อที่ตกลง]

The IP Schedule shall distinguish background IP, service models/software,
Customer Data and outputs. The Provider shall grant or assign output rights
only to the extent it lawfully holds and may grant them. This does not represent
that every AI output is copyrightable or exclusive. Third-party rights review,
defence and remedies shall be governed by [agreed provisions].
```

“ลูกค้าเป็นเจ้าของทั้งหมด” ไม่แก้ training rights/ใบหน้า/เสียง ให้สกิล IP ตรวจสิทธิและ remedy

### 2.4 ความโปร่งใสและกำกับโดยมนุษย์

```text
ผู้ให้บริการจัดข้อมูลข้อจำกัด intended use รุ่นและวิธีระบุเนื้อหา AI ที่ตกลง
ลูกค้ารับผิดชอบการตรวจ/อนุมัติในงาน [ระบุ] และการเปิดเผยต่อผู้ใช้/เผยแพร่
ตามหน้าที่ที่ใช้กับตน คู่สัญญาร่วมทดสอบว่าป้ายและ metadata คงอยู่หลังแปลงไฟล์
และแก้การเปิดเผยที่ผิด ไม่ลบหรือหลบเครื่องหมายโดยขัดหน้าที่ที่ใช้จริง

The Provider shall supply the agreed limitations, intended-use information,
version details and AI-content identification methods. The Customer shall
perform review/approval for [specified tasks] and disclosures applicable to its
use or publication. The parties shall test label and metadata preservation after
transformation and correct inaccurate disclosures. Neither party shall remove
or bypass markers contrary to applicable obligations.
```

### 2.5 เหตุ การตรวจและเปลี่ยนรุ่น

```text
คู่สัญญาแจ้งอีกฝ่ายเมื่อทราบเหตุ AI ที่อาจกระทบบริการ ข้อมูลหรือสิทธิ
ผ่าน [ช่องทาง] ภายใน [เวลาตามสัญญาที่ตกลง] พร้อมข้อเท็จจริงที่มีและการจำกัดผล
โดยไม่รอผลสอบสวนครบ ร่วมเก็บหลักฐานและรายงานเพิ่ม แต่ผู้มีหน้าที่ตามกฎหมาย
ยังต้องประเมิน/แจ้งหน่วยกำกับเอง การแจ้งตามสัญญาไม่แทนกำหนดตามกฎหมาย
ให้ตรวจหลักฐานและ audit ตาม [ขอบเขต/รอบ/เหตุ trigger/ผู้ตรวจ/ความลับ]
การเปลี่ยนโมเดล งานข้อมูล ผู้รับช่วงหรือที่ตั้งสำคัญใช้ change-control process
และให้สิทธิ re-test/rollback/exit ตาม [เงื่อนไขที่ตกลง]

Upon awareness of an AI incident that may affect Services, data or rights,
each party shall notify the other through [channel] within [agreed contractual
period], with available facts and containment actions, without awaiting a final
investigation. The parties shall preserve evidence and provide updates.
Statutory reporting duties remain with the responsible party; contractual
notice does not replace statutory deadlines. Evidence review and audits shall
follow [scope, frequency, triggers, auditor and confidentiality safeguards].
Material changes to models, data use, subprocessors or locations shall follow
change control, with re-testing, rollback and exit rights under [agreed terms].
```

Audit ไม่เปิดข้อมูลลูกค้ารายอื่น/เกินจำเป็น ใช้ secure/independent review โดยไม่ตัดสิทธิสอบเหตุ ไม่ใช้กำหนด PDPA เป็นเส้นตาย AI ทั่วไป

## 3. ความถูกต้องและการจำกัดความรับผิด

**(สรุปสาระ)** พ.ร.บ.ข้อสัญญาที่ไม่เป็นธรรมฯ ม.4 รวมสัญญาสำเร็จรูป ไม่จำกัด B2C; ม.8 ห้ามยกเว้น/จำกัดล่วงหน้าชีวิต ร่างกาย อนามัยจากจงใจ/ประมาท; ม.10 เกณฑ์ความเป็นธรรม [L6] ไม่ยกเว้นทุก AI error

```text
ผลลัพธ์ AI อาจไม่ถูกต้องหรือครบถ้วน ลูกค้าต้องใช้การตรวจตามงานที่ตกลง
ข้อนี้ไม่ลดมาตรฐานและ acceptance criteria ของผู้ให้บริการ ไม่ยกเว้นความรับผิด
ที่กฎหมายห้ามยกเว้น และไม่ตัดสิทธิบุคคลภายนอก

AI outputs may be inaccurate or incomplete. The Customer shall apply the
agreed task-specific review. This clause does not reduce the Provider's agreed
standards or acceptance criteria, exclude liability that cannot lawfully be
excluded, or limit third-party rights.
```

cap/indemnity/insurance ตาม control/หลักฐาน การแบ่งระหว่างคู่สัญญาไม่ผูกผู้เสียหาย/ผู้กำกับ; strict/joint liability ตามร่างยังไม่ใช้

## 4. การจัดซื้อรัฐ/CII

| ตรวจวันนี้ | เตรียมรับร่างในอนาคต |
|---|---|
| ผู้ซื้อรัฐ/CII TOR ชั้นข้อมูล ขั้นตอน/อำนาจอนุมัติ | รายการธุรกิจสัญญาควบคุมเฉพาะบริการรัฐ/CII [D11] |
| log/backup/support/ผู้รับช่วง PDPA/กฎหมายเฉพาะ | กิจกรรม/ข้อมูลที่ให้ AI ประมวลผลในไทย ไม่ใช่ทุกบริษัท |
| คลาวด์/ไซเบอร์วันนี้และ flow-down [L11]; ประกาศ กมช. มาตรฐานการรักษาความมั่นคงปลอดภัยไซเบอร์ระบบคลาวด์ 2567 (ราชกิจจาฯ 43184, ลง 10 ก.ย.2567, มีผล 10 ก.ย.2569) ครอบคลุมผู้ให้บริการคลาวด์สาธารณะ (IaaS/PaaS/SaaS) ที่ให้บริการแก่หน่วยงานของรัฐ/ผู้กำกับ/CII; ระดับผลกระทบ (ข้อ 1.8.2 + ตาราง ข้อ 4): ต่ำ = ISO/IEC 27001 + CSA STAR Level 1; กลาง = CSA STAR Level 2 + ISO/IEC 27701; สูง = ISO/IEC 27017 หรือ CSA STAR Level 2 + ISO/IEC 27018 และ 27701 | ข้อบังคับ/marker/เหตุ/ตัวแทนตามฉบับสุดท้าย |
| acceptance ภาษาไทย security/audit/exit/คนกำกับ | ทบทวนเมื่อกฎหมายเปลี่ยน ไม่รับภาระราคา/เวลาไม่จำกัด |
| พ.ร.บ.การจัดซื้อจัดจ้างและการบริหารพัสดุภาครัฐ 2560: TOR ขอบเขตงาน ราคากลาง วิธีซื้อ/จ้าง | ใช้วิธีซื้อที่ตรง ไม่เหมาสัญญา AI เป็นสัญญาควบคุม [D11] |
| พ.ร.บ.การบริหารงานและการให้บริการภาครัฐผ่านระบบดิจิทัล 2562: ชั้นข้อมูล การเชื่อมโยง บริการดิจิทัล | ร่าง ม.50 ประมวลผลในไทยถ้าฉบับสุดท้ายกำหนด |
| มาตรฐานรัฐบาลดิจิทัล (DGA/DGS): ระดับบริการ/ข้อมูลและความมั่นคงปลอดภัย | ตรวจเลขรุ่น/ขอบเขตมาตรฐานกับ TOR ที่ใช้จริง |
| นโยบาย Cloud First (ครม. 11 ก.ย.2566): ใช้คลาวด์ก่อนทางเลือกอื่น | ไม่แทนข้อกำหนดไซเบอร์/PDPA/การโอนข้อมูล |

มาตรฐานคลาวด์ **ไม่ใช่ localisation ร่าง AI** โฮสต์ไทย/ผู้ขายไทยไม่พิสูจน์ว่า support/training/ผู้รับช่วงอยู่ไทย ส่ง CII/คลาวด์ให้ `thai-tech-platform-law`, โอน/เข้าถึงให้ `thai-pdpa`; ไม่แต่ง TOR ทุกหน่วย

## 5. เกณฑ์ก่อนลงนาม

- scope/รุ่น/งาน และ RACI ตรงทะเบียน; ไม่มี acceptance วัดไม่ได้
- no-training/ผู้รับช่วง/retention ตรงบริการที่ซื้อ; marketing ไม่ขัดสัญญา
- ค่า audit/ทดสอบ/ย้าย/ลบและผู้รับผิดชอบชัด; exit ทำได้และมี fallback
- incident/change channels ใช้งานจริง; ข้อความอังกฤษ/ไทยและลำดับเอกสารตรงกัน
- ไม่มี waiver สิทธิบังคับ และไม่ย้ายหน้าที่หน่วยกำกับให้ vendor จนองค์กรละเลย

---

## หลักการ

- แยกบริการที่ได้จริง ข้อสัญญาปัจจุบัน และเงื่อนไขที่จะทบทวนเมื่อกฎหมายใหม่ออก
- ไม่ให้สิทธิข้อมูล/IP เกินที่มีและไม่อ้าง disclaimer เพื่อหลีกเลี่ยงกฎหมาย
- ให้ทนายตรวจทั้งสัญญาและ annex พร้อมข้อสังเกตจากทนาย
