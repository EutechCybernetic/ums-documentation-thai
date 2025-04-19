# กระบวนการดำเนินการที่ซับซ้อน

กระบวนการดำเนินการที่ซับซ้อนนี้เหมือนกับกระบวนการดำเนินการง่าย ยกเว้นขั้นตอนเพิ่มเติมหนึ่งขั้นตอนที่สำคัญ: การทำแผนที่เมตรไปยังสถานที่

* กำหนดค่า Meters ดูที่ [configuring-meters.md](../getting-started/configuring-the-application/configuring-meters.md "mention")
* ตั้งค่าการรวมเข้ากับ meters
* ตั้งค่า tags, virtual meters หรือ meter groups ตามต้องการ (ดูที่ [configuring-virtual-meters.md](../getting-started/configuring-the-application/configuring-virtual-meters.md "mention"), [configuring-meter-groups.md](../getting-started/configuring-the-application/configuring-meter-groups.md "mention"), [configuring-tags.md](../getting-started/configuring-the-application/configuring-tags.md "mention"))
* ทำแผนที่ Meters ไปยังสถานที่
* ตั้งค่าแดชบอร์ดของคุณ



## ทำไมฉันต้องทำแผนที่เมตรไปยังสถานที่

เมื่อคุณมีเมตรและเมตรย่อย การบริโภคสำหรับสถานที่อาจจะทำให้เกิดความสับสน เพราะยังรวมเมตรย่อย ที่ค่าของมันอาจจะถูกคำนวณเข้าไปในเมตรหลักแล้ว

ตัวอย่างเช่น ถ้าเมตรหลักคือแผงกระจาย และเมตรย่อยคือเมตรสาธารณูปโภคภายในชั้น แผงกระจายจะรวมการบริโภคของเมตรย่อยแล้ว

ดังนั้น ถ้าทั้งสองต่อกับสถานที่เดียวกัน มันจะนับการบริโภคบางส่วนสองครั้ง



วิธีแก้ไขคือ ทำเครื่องหมายแผงกระจายเป็นเมตรหลักสำหรับสถานที่

สำหรับทุกสถานที่ที่คุณต้องการติดตามการบริโภคและมีเมตรย่อย คุณสามารถทำเครื่องหมายหนึ่งในเมตรเป็นเมตรหลักสำหรับสถานที่นั้น

{% hint style="info" %}
เมตรหลักโดยทั่วไปจะเป็นแผงกระจายที่สถานที่นั้น
{% endhint %}

คุณยังสามารถทำแผนที่ virtual meter หรือ meter group

ดังนั้น ถ้ามีเมตรหลักมากกว่าหนึ่งในสถานที่ - คุณสามารถสร้าง virtual meter หรือ meter group สำหรับมัน แล้วทำแผนที่กลุ่มหรือ virtual meter เป็นเมตรหลักสำหรับสถานที่



ดูที่ [marking-the-main-meter.md](../getting-started/configuring-the-application/marking-the-main-meter.md "mention") ส่วนสำหรับข้อมูลเพิ่มเติมเกี่ยวกับการทำแผนที่เมตรไปยังสถานที่.