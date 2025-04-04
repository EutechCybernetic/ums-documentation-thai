# กระบวนการดำเนินการที่ซับซ้อน

กระบวนการดำเนินการที่ซับซ้อนนั้นเหมือนกับกระบวนการดำเนินการที่ง่าย ยกเว้นขั้นตอนหลักที่เพิ่มเติมขึ้นมาคือ: การทำแผนที่เมตรไปยังสถานที่

* กำหนดค่าเมตร ดู [configuring-meters.md](../getting-started/configuring-the-application/configuring-meters.md "mention")
* ตั้งค่าการรวมเมตร
* ตั้งค่าแท็ก, เมตรเสมือน หรือกลุ่มเมตร (ดู [configuring-virtual-meters.md](../getting-started/configuring-the-application/configuring-virtual-meters.md "mention"), [configuring-meter-groups.md](../getting-started/configuring-the-application/configuring-meter-groups.md "mention"), [configuring-tags.md](../getting-started/configuring-the-application/configuring-tags.md "mention"))
* ทำแผนที่เมตรไปยังสถานที่
* ตั้งค่าแดชบอร์ดของคุณ



## ทำไมฉันต้องทำแผนที่เมตรไปยังสถานที่

เมื่อคุณมีเมตรและเมตรย่อย การบริโภคสำหรับสถานที่อาจทำให้เกิดความสับสน เนื่องจากยังรวมเมตรย่อย ที่มีค่าที่ได้รับการคำนวณล่วงหน้าในเมตรหลัก

ตัวอย่างเช่น ถ้าเมตรหลักคือแผงกระจายและเมตรย่อยคือเมตรสาธารณูปโภคภายในชั้น แผงกระจายจะรวมการบริโภคของเมตรย่อยแล้ว

ดังนั้น ถ้าทั้งสองต่อกับสถานที่เดียวกัน จะทำให้การนับบางส่วนของการบริโภคซ้ำซ้อน



วิธีแก้ปัญหาคือทำเครื่องหมายแผงกระจายเป็นเมตรหลักสำหรับสถานที่

สำหรับทุกสถานที่ที่คุณต้องการติดตามการบริโภคและมีเมตรย่อย คุณสามารถทำเครื่องหมายหนึ่งในเมตรเป็นเมตรหลักสำหรับสถานที่นั้น

{% hint style="info" %}
เมตรหลักโดยทั่วไปจะเป็นแผงกระจายที่สถานที่นั้น
{% endhint %}

คุณยังสามารถทำแผนที่เมตรเสมือนหรือกลุ่มเมตร

ดังนั้น ถ้ามีเมตรหลักมากกว่าหนึ่งในสถานที่ - คุณสามารถสร้างเมตรเสมือนหรือกลุ่มเมตรสำหรับมันแล้วทำแผนที่กลุ่มหรือเมตรเสมือนเป็นเมตรหลักสำหรับสถานที่



ดูส่วน [marking-the-main-meter.md](../getting-started/configuring-the-application/marking-the-main-meter.md "mention") สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการทำแผนที่เมตรไปยังสถานที่.