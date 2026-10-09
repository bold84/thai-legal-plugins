# templates.md — แม่แบบงาน PDPA (Privacy Notice, DPA, ภาคผนวกโอนข้อมูล, DSAR, แจ้งเหตุละเมิด, ROPA, TIA)

อ่านไฟล์นี้เมื่อร่างเอกสาร · [....] เป็นช่องข้อมูลที่ต้องเติมก่อนส่ง ไม่ใช่ข้อเท็จจริงสมมติให้รับรอง · ข้อสัญญาเป็นข้อเสนอ (การวิเคราะห์/แนวปฏิบัติ) ไม่ใช่ตัวบทคัดลอก · ชื่อเต็ม/วันที่/URL ใน `key_sections.md` · ข้อมูล ณ 9 ตุลาคม 2569 (2026)

---

## สารบัญ
1. Privacy Notice (ม.23)
2. DPA สองภาษา (ม.40 ว.3)
3. ภาคผนวกโอนข้อมูลข้ามพรมแดน (ม.28/29)
4. จดหมายตอบ DSAR
5. แบบแจ้งเหตุละเมิด
6. ตาราง ROPA
7. สรุป TIA — โปรไฟล์กฎหมายไทย

---

## 1. Privacy Notice (ม.23)

ตรวจครบหกรายการ ม.23 ก่อน/ขณะเก็บเว้นรู้แล้ว; แหล่งอื่นใช้ ม.25/เงื่อนไขครั้งแรก ไม่ใช่ 30 วันทุกกรณี Notice ไม่ใช่ consent ถ้าต้องยินยอมให้ทำแบบแยกตาม ม.19/20/26

```text
ประกาศความเป็นส่วนตัว / Privacy Notice — ฉบับ [....] วันที่ / Date [....]
ผู้ควบคุม [ชื่อ/ช่องทาง]; ตัวแทนไทย [ถ้ามี]; DPO [ถ้ามี/ช่องทาง]
Controller [name/contact]; Thai representative [if any]; DPO [if any/contact].
เราเก็บ [ประเภทข้อมูล] จาก [ท่าน/แหล่งอื่น] เพื่อ [วัตถุประสงค์รายกิจกรรม]
โดยใช้ฐาน [ม.24(..)/ม.26(..)/consent] และเก็บ [ระยะเวลาหรือเกณฑ์ที่กำหนดได้]
We collect [data] from [you/other sources] for [each purpose], on [basis],
and retain it for [period or determinable criteria].
ท่าน [ต้อง/ไม่ต้อง] ให้ข้อมูลตาม [กฎหมาย/สัญญา/เพื่อเข้าทำสัญญา]; หากไม่ให้ [ผล]
Providing [data] is [required/optional] under [law/contract]; not providing it means [effect].
เราเปิดเผยแก่ [ประเภทผู้รับ]; โอนไป [ประเทศ/ผู้รับ/เครื่องมือ/มาตรการ]
We disclose to [recipient categories] and transfer to [countries/recipients] under [safeguards].
ท่านขอถอนยินยอม เข้าถึง/สำเนา/ที่มา โอนย้าย คัดค้าน ลบ ระงับ แก้ไข และร้องเรียน
ตามเงื่อนไขกฎหมายได้ที่ [ช่องทางตรง/ไปรษณีย์/อิเล็กทรอนิกส์] การถอนง่ายเท่าให้
You may exercise the applicable rights to withdraw consent, access/copies/sources,
portability, object, erase, restrict, rectify and complain through [channels].
Withdrawal is as easy as giving consent and does not affect prior lawful processing.
คำขอเข้าถึงตอบภายใน 30 วัน ขยายไม่เกินอีก 30 วันตามเงื่อนไขโดยแจ้งเหตุผล
สิทธิอื่นใช้เกณฑ์เฉพาะ ไม่ใช่ทุกคำขอ 30 วัน ติดต่อ/ร้องเรียน สคส. [ช่องทางปัจจุบัน]
Access requests are completed within 30 days, with a reasoned extension of up to
30 days where permitted. Other rights have their own rules. PDPC complaints: [current channel].
```

แนบตาราง `purpose | data | basis | mandatory/effect | retention | recipients/transfers` ไม่ใช้คำว่า “เพื่อพัฒนาบริการ” ครอบคลุม training ที่ไม่แจ้ง; หาก GDPR ใช้ เพิ่มรายละเอียดตามระบอบนั้น ไม่ส่ง notice ไทยแทนฉบับ EU โดยไม่ตรวจ

## 2. DPA สองภาษา (ม.40 วรรคสาม)

ม.40 บังคับข้อตกลง แต่ไม่ได้แจกแจงข้อสัญญาเท่ากับ GDPR Art.28 ทุกข้อ รายการ sub-processor/audit/SLA/liability เป็นข้อเสนอให้หน้าที่ทำได้จริง เติมภาคผนวกและลงนามก่อนประมวลผล

```text
ข้อตกลงประมวลผลข้อมูล / Data Processing Agreement — วันที่ / Date [....]
ผู้ควบคุม / Controller [....] กับผู้ประมวลผล / Processor [....]
ประกอบสัญญา / Underlying agreement [....]; ผู้ติดต่อเหตุ/สิทธิ / Contacts [....]

1. ขอบเขต: ผู้ประมวลผลทำตามคำสั่งที่บันทึกไว้และภาคผนวก 1 เท่านั้น ไม่ใช้เพื่อตน
หรือฝึกโมเดล/ทำ analytics นอกคำสั่ง หากคำสั่งขัดกฎหมายให้แจ้งทันทีและไม่ทำส่วนที่มิชอบ
Scope: Process only on documented instructions and Annex 1, not for own purposes,
model training or analytics outside instructions. Flag unlawful instructions promptly
and do not carry out the unlawful part.

2. ความลับ/ความปลอดภัย: ผูกพันผู้เข้าถึงให้รักษาลับ จำกัดสิทธิเท่าที่จำเป็น และใช้
มาตรการภาคผนวก 2 ไม่ต่ำกว่าประกาศความปลอดภัย พ.ศ.2565 ข้อ 4; ทบทวนตามความเสี่ยง
Confidentiality/security: Bind authorised personnel to confidentiality, restrict access
to need-to-know, and apply Annex 2 measures no lower than clause 4 of the 2022
PDPC security notification. Review measures as risks change.

3. แจ้งเหตุ: แจ้งผู้ควบคุมโดยไม่ชักช้าภายใน 72 ชั่วโมงนับทราบเท่าที่ทำได้ โดยแจ้ง
เบื้องต้นภายใน [SLA ที่สั้นกว่าตามตกลง] ผ่าน [ช่องทาง] พร้อมลักษณะ ข้อมูล/จำนวน
ผู้ติดต่อ ผลกระทบและมาตรการเท่าที่ทราบ ส่งข้อมูลเพิ่มโดยไม่รอสอบสวนเสร็จ
Breach: Notify the Controller without undue delay and within 72 hours of awareness
where feasible, with an initial alert within [agreed shorter SLA] via [channel].
Provide known nature, data/numbers, contact, effects and measures; promptly supplement
missing details without waiting for a final investigation.

4. สิทธิ/หลักฐาน: ส่งคำขอแก่ผู้ควบคุมในโอกาสแรกและภายใน [SLA] ไม่ตอบแทนเว้นมอบหมาย
ช่วยค้น ตัดข้อมูลผู้อื่น แก้ ลบ ระงับ และแจ้งเหตุให้ทันแต่ละกำหนด; ทำ ROPA ที่ต้องทำ
Rights/evidence: Forward requests at the first opportunity and within [SLA]; respond
only if authorised. Assist search, third-party redaction, rectification, erasure,
restriction and breach duties within the applicable deadlines; keep required ROPA.

5. ผู้ประมวลผลช่วง: ใช้เฉพาะ [รายชื่อ/อนุญาตทั่วไปพร้อมแจ้งก่อนและสิทธิคัดค้านตามตกลง]
ผูกพันหน้าที่คุ้มครองเทียบเท่าและรับผิดตาม [ขอบเขต]; ไม่ส่งต่อก่อนอนุมัติ/เครื่องมือครบ
Sub-processors: Use only [named approvals/general authorisation with agreed prior
notice and objection]. Impose equivalent protection and [agreed responsibility];
do not transfer before authorisation and the required transfer arrangements are in place.

6. โอน/คำขอรัฐ: เฉพาะ flow ประเทศและผู้รับในภาคผนวก 3 รวม support/โอนต่อ ตรวจความชอบ
คำขอรัฐ แจ้งเท่าที่กฎหมายอนุญาต พิจารณาโต้แย้งเมื่อมีเหตุ และเปิดเผยเฉพาะจำเป็น
Transfers/public authorities: Use only Annex 3 flows, countries and recipients,
including support/onward transfers. Review requests, notify where lawful, challenge
where warranted and available, and disclose only what is necessary.

7. ตรวจสอบ/สิ้นสุด: ให้หลักฐานมาตรการและ audit ตาม [วิธี/ขอบเขต] เมื่อสิ้นสุดให้
คืน/ลบตามทางเลือกผู้ควบคุมภายใน [กำหนดสัญญา] รวมสำรอง และยืนยันเป็นหนังสือ
หากกฎหมายบังคับเก็บ ให้ระบุกฎหมาย/ส่วน/ระยะเวลา แยกและห้ามใช้อย่างอื่นจนลบ
Audit/exit: Provide compliance evidence and audits under [procedure/scope]. At exit,
return or delete at the Controller's choice within [contractual period], including
backups, and confirm in writing. Identify mandatory legal retention, isolate that data,
and prohibit other use until deletion.

8. ความรับผิด/ลำดับ: ข้อตกลงชดใช้ระหว่างคู่สัญญา [....] ไม่ตัดสิทธิเจ้าของข้อมูล
หรืออำนาจหน่วยงาน DPA เหนือสัญญาหลักเรื่องข้อมูลแต่ไม่ลดหน้าที่กฎหมาย/ข้อสัญญาโอน
Liability/priority: Inter-party indemnities [....] do not restrict data-subject rights
or authorities' powers. This DPA prevails on data matters, without reducing mandatory
law or the applicable transfer clauses. Governing law/forum/language: [....].

ภาคผนวก / Annexes:
1 purpose/processing/data/subjects/duration/instructions; 2 TOMs/access/backup;
3 flow/country/recipient/role/tool/onward; 4 authorised sub-processors/contacts.
ลงนามผู้มีอำนาจ / Authorised signatures: Controller [....] Processor [....]
```

หาก GDPR ใช้ เติม Art.28(3) ให้ครบและตรวจว่า SLA ไทย/สัญญาไม่ลด “without undue delay” ของ Art.33(2)/SCC การทำให้นิรนามเพื่อใช้เองต้องมีคำสั่ง/ฐานก่อนและไม่แทนหน้าที่ return/delete ในชุด GDPR อัตโนมัติ

## 3. ภาคผนวกโอนข้อมูล (ม.28–29)

ไม่ใช่ SCC/MCC ตัวเต็ม: ต้องแนบต้นฉบับที่เลือกจริง EU SCC ข้อ 2 ห้ามแก้สาระนอกตัวเลือก/ภาคผนวกหรือเพิ่มขัดกัน; ASEAN MCC อนุญาตปรับตามเงื่อนไขต้นแบบ/กฎหมาย แต่ยังต้องครบประกาศ ม.29 ข้อ 9–11 และบังคับสิทธิ/เยียวยาได้

```text
การโอน / Transfer [ผู้ส่ง/ผู้รับ/role/countries/data/purpose/duration/onward]
เครื่องมือ / Tool [ม.28 เหตุและหลักฐาน / BCR รับรองไทย / สัญญาเข้าเกณฑ์ ม.29]
หากใช้ต้นแบบ: [EU SCC Module และ annex / ASEAN MCC Module และตัวเลือก]

A1 ภาคผนวกนี้เสริมเครื่องมือที่แนบ ไม่แก้ EU SCC หรือลดความคุ้มครอง หากขัดกัน
เครื่องมือบังคับที่เกี่ยวข้องใช้ก่อน; หน้าที่ไทยและ EU ที่ใช้จริงต้องครบแยก
This addendum supplements the attached tool without modifying EU SCCs or reducing
protection. Applicable mandatory transfer terms prevail; meet both regimes where applicable.

A2 ผู้รับคุ้มครองสิทธิเจ้าของข้อมูลที่ PDPA ใช้และเยียวยาที่บังคับได้ตาม [ข้อที่ระบุ]
ตั้งผู้ติดต่อ/รับร้องเรียน [....] และยอมรับการกำกับ/ศาลตามเครื่องมือ ไม่จำกัดเฉพาะสัญชาติไทย
The Recipient ensures enforceable rights and effective remedies for subjects covered
by PDPA, under [clauses], with [contact/complaint route] and the applicable jurisdiction.

A3 แจ้งเหตุแก่ผู้ส่งไม่ชักช้าภายใน 72 ชั่วโมงนับทราบเท่าที่ทำได้ตามหน้าที่ที่ใช้
ผู้รับ controller ที่ผู้ส่ง controller ตรวจข้อยกเว้นไม่มีความเสี่ยง; ไม่ลดหน้าที่ SCC
Notify the Sender without undue delay and within 72 hours of awareness where feasible
under the applicable duties. Controller-to-controller notification is subject to the
applicable no-risk exception; this does not reduce SCC obligations.

A4 โอนต่อเฉพาะ [เงื่อนไข/ผู้รับ/ประเทศ]; จำกัด purpose/ข้อมูลและผูกพันคุ้มครองต่อเนื่อง
ให้ทางเลือกเจ้าของตามประกาศข้อ 11; review คำขอรัฐ แจ้งเมื่อกฎหมายอนุญาต เปิดเผยขั้นต่ำ
Onward transfers only under [conditions/recipients/countries], with purpose limitation,
continuous protection and subject choices required by clause 11. Review public-authority
requests, notify where lawful and minimise disclosure.

A5 มาตรการเสริม/หลักฐาน [....]; ทบทวนเมื่อ [vendor/law/flow เปลี่ยน]; หากทำการคุ้มครอง
ที่บังคับไม่ได้ ให้แจ้งผู้ส่งและระงับ/สิ้นสุดตามเครื่องมือ ไม่ใช้ consent เหมารวม
Supplementary measures/evidence [....]; review on [changes]. If required protection
cannot be maintained, notify and suspend/terminate as required by the tool.
```

## 4. จดหมายตอบคำขอเข้าถึง

ใช้ประกาศ พ.ศ. 2569 ข้อ 6–12; ไม่ส่งหนังสือขอเอกสารเพิ่มเมื่อคำขอครบแล้ว คำขอสิทธิอื่นใช้แบบปรับเหตุ/นาฬิกาเฉพาะ ไม่ถือว่าตัวเลขชุดนี้ใช้ทุก DSAR

```text
(ก) รับคำขอ / Acknowledgement — เลขที่ [....] รับ [วันที่] ช่องทาง [....]
เราได้รับคำขอ [รายละเอียด] และจะตรวจครบ/ตัวตนไม่ชักช้าภายใน 15 วัน
We received [request] and will verify completeness/identity without delay within 15 days.
เฉพาะถ้าไม่ครบ: ต้องเพิ่ม [สิ่งจำเป็น/เหตุผล] ภายใน [วันที่ ให้ไม่น้อยกว่า 10 วัน]
ถือวันรับเมื่อแก้ครบ ไม่แก้ถือทิ้งโดยแจ้ง แต่ท่านยื่นใหม่ได้
Only if incomplete: supply [necessary items/reason] by [date, at least 10 days].
Receipt is when corrected and complete. Otherwise it is abandoned with notice,
without prejudice to a fresh request.

(ข) ขยาย / Extension — คำขอรับครบ [วันที่]; เดิมครบกำหนด [วันที่]
เพราะ [ข้อมูลมาก/เหตุจำเป็น/รายละเอียด] ขยาย [ไม่เกิน 30 วันจากกำหนดแรก]
กำหนดใหม่ [วันที่] ไม่ใช่เหตุขยายอัตโนมัติของทุกคำขอ
Because [volume/necessary reasons], extend by [up to 30 days from the original deadline]
to [date]. This is not an automatic extension for every request.

(ค) ปฏิเสธบางส่วน/ทั้งหมด / Partial/full refusal
ไม่ทำส่วน [....] ตาม [กฎหมาย/ศาล/สิทธิผู้อื่น หรือเหตุในข้อ 8 พร้อมรายละเอียด]
ส่วนที่ส่งได้ [....] ตัดข้อมูลผู้อื่น [วิธี] ท่านร้องเรียน สคส.ได้ผ่าน [ช่องทางปัจจุบัน]
We refuse [part/all] on [specific lawful ground/reasons under clause 8]. We provide
[remainder] with [redaction]. You may complain to PDPC through [current channel].

(ง) ส่งมอบ / Fulfilment
ข้อมูล/ที่มา/รายละเอียดที่ให้ [....] รูปแบบ/ช่องทางปลอดภัย [....]
ค่าธรรมเนียม [ฟรี/อัตราและเหตุที่เข้าเกณฑ์ซึ่งแจ้งแล้ว] ผู้ติดต่อ [....]
Provided data/sources/details [....] via [secure format/channel]. Fee [free/permitted
previously disclosed rate and basis]; contact [....].
```

เก็บคำขอ/เอกสาร/ผลไม่น้อยกว่า 2 ปี ปฏิเสธบันทึก ม.39(7); electronic แบบไม่มีสื่อ/ขนส่งโดยตรงฟรี อื่นคิดได้เท่าที่ข้อ 11/บัญชีท้ายอนุญาต ไม่เรียกค่าธรรมเนียมเพื่อกันสิทธิ

## 5. แบบแจ้งเหตุละเมิด

แบบทำงานนี้ไม่ใช่แบบราชการรับรอง ตรวจช่องทางสำนักงานฉบับปัจจุบันก่อนส่ง: ประกาศสำนักงานลง 15 ม.ค. 2568 ใช้ `saraban@pdpc.or.th` และหัวเรื่องที่กำหนด เนื้อหาตามประกาศแจ้งเหตุ พ.ศ. 2565 ข้อ 6/10

```text
ถึง สคส. / To PDPC — [การแจ้งเหตุการละเมิดข้อมูลส่วนบุคคล] [ชื่อผู้ควบคุม]
ผู้ควบคุม/ผู้ติดต่อ/DPO / Controller/contact/DPO [....]
ทราบเหตุ/เกิด/แจ้ง / Awareness/occurrence/notification [วัน-เวลา/time zone]
ลักษณะ/ประเภท / Nature/type [confidentiality/integrity/availability]
ข้อมูล/กลุ่ม/จำนวนที่ทราบ / Data/subjects/known numbers [....]
ผลกระทบ/ความเสี่ยง/หลักฐาน / Effects/risk/evidence [....]
มาตรการทำแล้ว/จะทำ / Measures taken/planned [....]
แจ้งเจ้าของเมื่อเสี่ยงสูง / High-risk subject notice [วิธี/เวลา/method/time]
ข้อมูลยังไม่ครบ/จะเพิ่ม / Missing information/supplement [....]
หากช้า: เหตุ/หลักฐาน/คำขอพิจารณา / If delayed: reasons/evidence/request [....]
```

แจ้งโดยไม่ชักช้าภายใน 72 ชั่วโมงนับทราบเท่าที่ทำได้ เว้นไม่มีความเสี่ยงที่พิสูจน์ได้ การขอยกเว้นผิดแจ้งช้าตามข้อ 7 ต้องแจ้งเร็วและไม่เกิน 15 วันพร้อมเหตุจำเป็น **ไม่ใช่ grace period/อนุญาตให้รอ**

```text
ถึงเจ้าของข้อมูล / To affected subjects — เมื่อ [วัน] เกิด [เหตุ/ข้อมูลที่กระทบ]
อาจเกิด [ผล] เราทำ [มาตรการ/เยียวยา] ท่านควรทำ [คำแนะนำตรงความเสี่ยง]
ติดต่อ [DPO/ชื่อ/สถานที่/วิธี] ได้ที่ [....]
On [date], [incident] affected [data]. Possible effects are [....]. We have taken
[measures/remedies]. Please [risk-specific advice]. Contact [DPO/contact/location/method].

ผู้ประมวลผล → ผู้ควบคุม / Processor to Controller — ทราบ [เวลา]
เหตุ/ข้อมูล/จำนวน/ผล/มาตรการ/ผู้ติดต่อเท่าที่ทราบ [....]; จะเพิ่ม [....]
Awareness [time]; known nature/data/numbers/effects/measures/contact [....]; supplement [....].
```

เสี่ยงสูงแจ้งเจ้าของไม่ชักช้า; รายบุคคลไม่ได้จริงใช้กลุ่ม/สาธารณะตามข้อ 11 โดยไม่เพิ่มเสียหาย Processor แจ้งไม่ชักช้าภายใน 72 ชั่วโมงนับตนทราบเท่าที่ทำได้/เร็วกว่าตาม SLA ไม่รอ controller ยืนยันก่อน

## 6. ตาราง ROPA

controller ม.39(1)–(8) กรอกข้อมูล (3) controller/ตัวแทนไว้ส่วนหัว; DPO/ฐาน/ผู้รับเป็นส่วนเสริมตามงาน ไม่ลืมปฏิเสธ ม.39(7) แม้เข้า SME exemption

```text
ผู้ควบคุม/ตัวแทน/DPO/ผู้จัดทำ/วันที่ [....]
กิจกรรม | (1)ข้อมูล | (2)purpose | (4)retention | (5)สิทธิ/วิธี/เงื่อนไขเข้าถึง
        | (6)ใช้/เปิดเผยยกเว้น consent | (7)คำขอปฏิเสธ/เหตุ | (8)ความปลอดภัย
เสริม: role/base/recipients/countries/tool/sub-processors/owner/review/evidence [....]

processor: processor/ตัวแทน; controller/ตัวแทนที่ทำแทน; DPO/ช่องทาง;
ประเภท/ลักษณะ processing/data/purpose; ประเภทผู้รับต่างประเทศ; ความปลอดภัย
ตามประกาศ ROPA processor พ.ศ.2565 ข้อ 3 — ไม่ใช้ตาราง controller แทนทั้งหมด
```

## 7. สรุป TIA — ประเทศไทย

อ่านโปรไฟล์ `cross_border_transfers_and_tia.md` ข้อ 4–6 ไม่ใช้ template รับรองทั้งประเทศ; แยกตัวบท A แหล่งรอง B และผลต่อ flow/ข้อจำกัด C

```text
การโอน EU/EEA → ผู้รับไทย [....]; tool/module [....]; data/purpose/role/onward [....]
Thailand profile: ไทยไม่อยู่ในบัญชี EU adequacy ที่ตรวจ [วันที่]
law/section | actor/trigger | court before/after | notice/secrecy | redress/limits
             | confidence A/B/C | practice evidence | impact on this flow
กฎหมายที่เกี่ยว: CCA 18–19/26; NIA 6/8; Cybersecurity 60–69;
DSI 24–26; AMLA 38/46; Emergency 5/11/16–17; PDPA 4/พ.ร.ฎ.2566
ข้อมูลผู้รับ: คำขอ/ผล/ช่วงเวลาที่ตรวจ [....] ไม่ใช้ไม่มีคำขอ = ไม่มีความเสี่ยง
measures: technical [....] contractual [....] organisational [....]
plaintext/key/support access [....]; effectiveness/residual risk [....]
decision [โอน/มีเงื่อนไข/ระงับ]; reasons/evidence [....]; approver [....]; review triggers [....]
```

---

## หลักการ
- เติมข้อเท็จจริง/ภาคผนวก ตรวจเครื่องมือและอำนาจลงนาม ไม่ส่งช่องว่างเป็นเอกสารพร้อมใช้
- EU SCC/MCC มีเงื่อนไขการปรับต่างกัน; การเพิ่มข้อไทยห้ามลดความคุ้มครองที่บังคับ
- ตรวจกำหนดและช่องทางราชการก่อนส่ง · ปิดท้ายด้วย "ข้อสังเกตจากทนาย"
