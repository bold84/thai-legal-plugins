# templates.md — แม่แบบแจ้งเนื้อหา คำขอข้อมูล log และข้อสัญญา

อ่านไฟล์นี้เมื่อร่างเอกสารปฏิบัติหลังตรวจฐานกฎหมายแล้ว · ข้อมูล ณ 9 ตุลาคม 2569 (2026) · **แบบร่างเพื่อปรับใช้ ไม่ใช่แบบราชการหรือคำรับรองผล** · ช่องวงเล็บเป็นข้อมูลเฉพาะงาน ไม่ใช่ข้อความกฎหมาย · หลักกฎหมายเป็น (สรุปสาระ) ตาม `key_sections.md`

---

## สารบัญ

1. หนังสือแจ้งและตอบผู้ร้อง
2. ลิขสิทธิ์และคำโต้แย้ง
3. ทะเบียนคำขอและหนังสือตอบรัฐ
4. โครงนโยบาย log
5. เช็กลิสต์ ETDA และ scoping memo
6. ข้อสัญญาผู้ขายให้รัฐ/CII

## 1. หนังสือแจ้งและตอบผู้ร้อง

สำหรับช่องร้องเรียน ม.15/ประกาศ MDES 2565 ข้อ 6 ต้องเติมเอกสารประกอบและใช้ตามองค์ประกอบ ไม่ใช้แทนแบบคำสั่งเจ้าหน้าที่ตามประกาศ

```text
เรื่อง: ขอระงับการเผยแพร่/นำข้อมูลออก — เลขรับเรื่อง [หมายเลข]
ถึง [ชื่อและช่องติดต่อผู้ให้บริการ/ตัวแทน]

ผู้ร้อง: [ชื่อ ที่อยู่ โทรศัพท์/อีเมล]
ผู้แทนและหลักฐานอำนาจ (ถ้ามี): [รายละเอียด]
ผู้ให้บริการที่ร้องเรียน: [ชื่อ ที่อยู่ ช่องติดต่อ]
ข้อมูล/URL/data ID: [ตำแหน่งเฉพาะที่ระบุได้]
ข้อเท็จจริง: [เนื้อหา เวลา เหตุและหลักฐานที่เกี่ยวข้อง]
ฐานที่กล่าวอ้าง: [มาตรา/ข้อและเหตุเข้าองค์ประกอบ ไม่ใช้เพียงชื่อกฎหมาย]
ความเสียหาย: [ลักษณะและความเกี่ยวข้องของผู้ร้อง]
สิ่งที่ขอ: [รายการและขอบเขตการระงับ/นำออก]
เอกสารประกอบ: [รายการ]
ข้าพเจ้ารับรองว่าข้อความที่แจ้งเป็นความจริง
[ลายมือชื่อ/ลายมือชื่ออิเล็กทรอนิกส์] [วันที่]

Subject: Request to suppress dissemination/remove content — [case ID]
To: [provider/representative and verified contact]
Complainant: [name, address, phone/email]
Representative and authority, if any: [details]
Provider complained against: [name, address and contact]
Content and exact location: [URL/data ID]
Facts and evidence: [content, dates, context and supporting material]
Alleged legal basis: [provision and facts satisfying it]
Harm and complainant's connection: [details]
Requested action and scope: [specific items]
Attachments: [list]
I certify that the statements in this notice are true.
[Signature/electronic signature] [date]
```

```text
ตอบรับ: ได้รับเรื่อง [ID] เมื่อ [วันเวลา/เขตเวลา] เกี่ยวกับ [รายการ]
สถานะ: [กำลังตรวจข้อมูล/ระงับแล้ว/ขอข้อมูลที่ขาดโดยระบุรายการ]
การดำเนินการนี้ไม่เป็นการวินิจฉัยความรับผิดหรือรับรองสิทธิของคู่กรณี
ช่องทางติดตาม: [ผู้รับผิดชอบ/ช่องทาง]

Acknowledgment: We received case [ID] at [date/time/timezone] concerning [items].
Status: [reviewing/suppressed/requesting the specifically listed missing details].
This action is not a determination of liability or an endorsement of either party's rights.
Case contact: [responsible contact].
```

อย่ารอคำตอบอัตโนมัติแทนการดำเนินการทันทีเมื่อเงื่อนไขกฎหมายครบ และอย่าส่งข้อมูลส่วนตัวผู้ร้องเกินสิ่งที่ขั้นตอนกฎหมายเรียกโดยไม่ประเมินกับ `thai-pdpa`

## 2. ลิขสิทธิ์และคำโต้แย้ง

Notice ม.43/6 ให้ใช้ช่องผู้ร้อง/งาน/ตำแหน่ง/คำรับรอง/ลายมือชื่อ โดยเพิ่ม **งานอันมีลิขสิทธิ์และหลักฐานสิทธิ การใช้ที่กล่าวว่าละเมิด และการพิจารณาข้อยกเว้น** แยกจาก ม.15; ใช้ `thai-copyright-software` ตรวจเงื่อนไข safe harbour ก่อนส่ง

```text
คำโต้แย้งลิขสิทธิ์ตาม ม.43/7 — [case ID]
ผู้ใช้: [ชื่อ/ชื่อนิติบุคคล ที่อยู่ โทรศัพท์ อีเมล]
รายการที่ถูกนำออก/ระงับและตำแหน่งก่อนดำเนินการ: [URL/data ID/link]
คำชี้แจงว่าดำเนินการโดยผิดพลาด/ผิดหลง: [ข้อเท็จจริงและหลักฐาน]
[ลายมือชื่อ/ลายมือชื่ออิเล็กทรอนิกส์] [วันที่]

Copyright counter-notice under section 43/7 — [case ID]
User: [name/entity, address, phone, email]
Removed/disabled material and its previous location: [URL/data ID/link]
Explanation of error or misidentification: [facts and supporting evidence]
[Signature/electronic signature] [date]

สำหรับผู้ให้บริการ: ตรวจความครบ ส่งสำเนาแก่เจ้าของสิทธิโดยเร็ว และแจ้ง
การคืนเมื่อพ้น 30 วันนับแต่รับคำโต้แย้ง โดยคืนภายใน 15 วันถัดไป
เว้นได้รับแจ้งพร้อมหลักฐานการยื่นฟ้องผู้ใช้; ตรวจฐานอื่นที่ยังห้ามเผยแพร่
Provider use: Check completeness, promptly forward to the owner and explain
restoration after 30 days from receipt, within the following 15 days,
unless notified with evidence of a filed suit against the user.
Check any independent legal restriction before restoring.
```

คำโต้แย้งทั่วไปเกี่ยวกับเงื่อนไขแพลตฟอร์มใช้รูปแบบข้อมูลผู้ใช้/รายการ/เหตุผล/หลักฐานเดียวกันได้ แต่ต้องเปลี่ยนชื่อและฐาน **ห้ามเรียกทุกคำโต้แย้งว่า ม.43/7 หรือให้สิทธิคืนอัตโนมัติแก่ lane ศาล/CCA**

## 3. ทะเบียนคำขอและหนังสือตอบรัฐ

```text
ทะเบียนคำขอรัฐ / Government request register
Case ID | Received time/timezone | Agency/case/document reference
Verified official/appointment/contact-back evidence
Legal basis | Requested action: preservation/disclosure/access/removal
Data type: traffic/user identification/content | Accounts/URLs | Time range
Court authorization required? | Order and scope | Confidentiality constraint
Legal deadline and trigger | Extension request/approval (if any)
Legal reviewer | Approver | Technical executor | Independent checker
Decision and reasons | Questions/narrowing sent | Hold scope/review/release basis
Export manifest/checksum | Secure delivery | Recipient | Receipt
User notice: permitted/prohibited/not appropriate, with reasons
Completion time | Remaining obligations | Evidence location/access restrictions
```

```text
ถึง [หน่วยงาน/เจ้าหน้าที่] อ้างถึง [หนังสือ/คดี]
ได้รับคำขอเมื่อ [วันเวลา] เกี่ยวกับ [ชุดข้อมูล/การกระทำ]
[ยืนยันส่วนที่ดำเนินการได้พร้อมรายการ/ช่วงเวลา]
ส่วน [รายการ] ขอให้ยืนยัน [อำนาจ/คำสั่งศาลเมื่อจำเป็น/ขอบเขต/ระบบรับ]
[ขออนุญาตขยายเวลาพร้อมเหตุและวันที่ หากฐานกฎหมายอนุญาต]
การขอความชัดเจนไม่ถือเป็นการหยุดหรือขยายกำหนดเวลาโดยฝ่ายเดียว
ข้อมูลจะส่งผ่าน [ช่องทางที่ตกลง] ให้ [ผู้รับที่ตรวจตัวตนแล้ว]
[ผู้มีอำนาจลงนาม/ช่องทางประสาน]

To: [agency/official], reference [document/case]
Received at [date/time], concerning [data/action].
[Identify the lawful, clear portion and action taken or scheduled.]
For [items], please confirm [authority/necessary court order/scope/receiving system].
[Request an authorized extension with reasons and proposed date, if permitted.]
This clarification request does not unilaterally suspend or extend the deadline.
Delivery will use [agreed secure method] to [verified recipient].
[Authorized signatory/contact]
```

## 4. โครงนโยบาย log

```text
นโยบายเก็บข้อมูลจราจร / Traffic-data retention policy
1. ขอบเขตบริการและประเภทตามประกาศ MDES 2564 พร้อมเหตุผล
2. Schedule ต่อชุดข้อมูล:
   field | purpose/legal basis | source | accountable owner | storage location
   start event | minimum period | deletion event | access | integrity/time controls
3. Traffic data: ไม่น้อยกว่า 90 วันจากเข้าสู่ระบบ ตาม ม.26/ประกาศที่ใช้
4. User identification: เก็บข้อมูลจำเป็นตั้งแต่เริ่มใช้และอย่างน้อย 90 วันหลังสิ้นสุด
5. Extended retention: เฉพาะคำสั่งที่ตรวจแล้ว ระบุช่วง/ราย/คราวและเพดานที่ใช้
6. Legal hold: ฐาน/ผู้สั่ง/ชุดข้อมูล/วันเริ่ม/ผู้รับผิดชอบ/ทบทวน/เหตุปลด
7. การรับคำขอ การอนุมัติ ส่งออก manifest/checksum และบันทึกการส่งมอบ
8. ป้องกันแก้ไข/สูญหาย การอ้างอิงเวลา สิทธิ admin และผู้รับจ้างเก็บ log
9. PDPA: notice/base/minimisation/transfers ผ่าน thai-pdpa
10. การลบ ตรวจการลบ ข้อยกเว้น hold และหลักฐานทบทวนนโยบาย

Content retention is separate from statutory traffic-data retention.
Preservation does not itself authorize disclosure. The 2-year ceiling is not
an instruction to retain all customer content for 2 years.
```

## 5. เช็กลิสต์ ETDA และ scoping memo

```text
DPS scoping / Notification preparation — ไม่ใช่แบบราชการ
[ ] ผู้ประกอบธุรกิจ/คู่สัญญาจริงและประเทศ
[ ] แผนภาพฟังก์ชัน private/public ผู้ใช้และคู่ธุรกรรม
[ ] นิยาม ม.3 ข้อยกเว้น ม.4 และกรณีแจ้งโดยย่อพร้อมเหตุผล
[ ] รายได้บริการในไทย AMAU และวิธีคำนวณที่ตรวจย้อนกลับได้
[ ] ประเภท/รายชื่อเฉพาะ และหน้าที่ ม.16–23 ที่ใช้
[ ] ผู้ประสานงานไทย/หนังสือแต่งตั้งเมื่อเกี่ยวข้อง
[ ] ข้อมูล ม.12 เอกสารอำนาจ ช่องทางบริการ ประเภทผู้ใช้ และข้อร้องเรียน
[ ] ใช้แบบในระบบ ETDA ฉบับปัจจุบัน เก็บใบรับ/คำสั่งแก้ไข
[ ] รายงานประจำปีตามปีบัญชีจริงและทะเบียนเปลี่ยนข้อมูล/เงื่อนไข
[ ] ช่องร้องเรียน การเยียวยา ranking/terms version และ exit plan
[ ] เจ้าของงาน หลักฐาน compliance และ trigger ประเมินเมื่อเพิ่มฟีเจอร์
Conclusion: in scope/out of scope/conditional, separately for each function.
Missing facts: [specific items]. Basis/source/date: [verified provisions/URLs].
```

## 6. ข้อสัญญาผู้ขายให้รัฐ/CII

ใช้หลังทราบ CII/ชั้นข้อมูล/ข้อควบคุมจริง ตรวจทั้งสองภาษากับ `thai-contract-master`; ไม่รับรองว่าข้อความนี้ครบ TOR ทุกหน่วยงาน และไม่ใส่หน้าที่ตามกฎหมายของลูกค้าให้ผู้ขายรับทั้งหมดโดยไม่แจกแจง

```text
1. ขอบเขตและความรับผิดร่วม
คู่สัญญาจะระบุระบบ ข้อมูล ระดับข้อมูล และมาตรฐานที่ใช้ในภาคผนวกความปลอดภัย
พร้อมตารางความรับผิดลูกค้า/ผู้ให้บริการ/ผู้รับจ้างช่วง การจ้างภายนอกไม่ยกเลิก
หน้าที่กฎหมายของผู้มีหน้าที่โดยตรง
Scope and shared responsibility
The security schedule shall identify systems, data, classification and applicable
standards, and allocate customer/provider/subcontractor controls. Outsourcing
does not displace either party's direct statutory obligations.

2. การแจ้งเหตุและความร่วมมือ
ผู้ให้บริการแจ้งเหตุที่กระทบบริการหรือข้อมูลในขอบเขตผ่านช่องทาง [ระบุ] ภายใน
[ระบุเวลาสัญญา/เหตุเริ่มที่ตกลง] พร้อมข้อมูลที่ทราบ มาตรการและการเพิ่มเติม
ลูกค้ารับผิดชอบรายงานหน่วยงานตามกฎหมายของตน โดยผู้ให้บริการช่วยเก็บหลักฐาน
และให้ข้อมูลที่จำเป็น กำหนดเวลาสัญญาไม่แทนหรือขยายเวลาตามกฎหมาย
Incident notice and cooperation
The provider shall notify in-scope incidents through [channel] within [agreed
period and trigger], describing known facts, response and updates. The customer
retains its statutory reporting duties; the provider shall preserve relevant
evidence and supply necessary information. Contract timing does not replace
or extend statutory deadlines.

3. สิทธิและการเข้าถึง
จำกัดผู้เข้าถึงตามหน้าที่ บันทึก privileged access และใช้กระบวนการอนุมัติ
การเข้าถึงจากภายนอก การตอบคำขอรัฐต้องตรวจฐานและขอบเขต ไม่ส่งข้อมูลหรือ
กุญแจของลูกค้ารายอื่น; แจ้งลูกค้าเมื่อกฎหมายและคำสั่งอนุญาต
Access and government requests
Access shall be role-limited; privileged and remote access shall be approved
and logged. Government requests require verification of authority and scope.
Other customers' data or keys shall not be disclosed. The customer shall be
notified where permitted by applicable law and orders.

4. ตรวจสอบและผู้รับจ้างช่วง
จัดหลักฐานข้อควบคุม/การตรวจตามขอบเขต ให้สิทธิตรวจที่สมเหตุสมผลโดยรักษา
ความลับและข้อมูลรายอื่น แจ้งการเปลี่ยนผู้รับจ้างช่วงที่เกี่ยวข้องตามขั้นตอน
ที่ตกลง และส่งต่อข้อควบคุมที่จำเป็นโดยผู้ให้บริการยังรับผิดตามสัญญา
Assurance and subcontractors
Provide in-scope control/audit evidence and reasonable audit rights subject to
confidentiality and other customers' rights. Relevant subcontractor changes
shall follow the agreed notice procedure. Required controls shall flow down,
without relieving the provider of its contractual responsibilities.

5. คืนข้อมูลและสิ้นสุดบริการ
กำหนดรูปแบบ/เวลาส่งออก การช่วยย้าย backup และการลบที่ตรวจได้ในภาคผนวก
แยกข้อมูลที่กฎหมาย/คำสั่งบังคับเก็บ พร้อมจำกัดการใช้และแจ้งเหตุไม่ลบเมื่อทำได้
Exit and deletion
The schedule shall define export format/timing, migration support, backups
and verifiable deletion. Legally required retention or preservation shall be
identified separately, with restricted use and permitted explanation of any
non-deletion. No unrestricted indefinite retention right is granted.
```

---

## หลักการ

ปรับข้อมูลและฐานก่อนส่ง; แยกแบบภายในจากแบบราชการ; ใช้เวลาเฉพาะ lane; ภาษาไทย/อังกฤษต้องมีผลสอดคล้องกัน; ห้ามแม่แบบให้สิทธิเปิดเผย ลบ หรือคืนเนื้อหาเกินอำนาจที่ตรวจแล้ว
