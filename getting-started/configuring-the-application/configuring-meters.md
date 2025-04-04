# การตั้งค่ามิเตอร์

เมื่อคุณได้ตั้งค่าประเภทสาธารณูปโภคของคุณแล้ว คุณสามารถเริ่มเพิ่มและตั้งค่ามิเตอร์ได้

{% hint style="info" %}
ที่นี่ 'มิเตอร์' หมายถึงมิเตอร์ทางกายภาพ - ซึ่งจะบันทึกข้อมูลการใช้งาน
{% endhint %}



ไปที่ส่วน Configuration ในแอปพลิเคชันและใน 'Meters' คุณสามารถเริ่มเพิ่มมิเตอร์ได้



ส่วน Meters จะแสดงรายการของมิเตอร์ทางกายภาพทั้งหมดที่คุณได้ตั้งค่าไว้ คุณสามารถคลิก 'Add Item' ที่ด้านบนเพื่อลงทะเบียนมิเตอร์ใหม่ คุณสามารถแก้ไขแต่ละมิเตอร์โดยคลิกที่ไอคอน 'edit' ที่ด้านขวาของแต่ละมิเตอร์



## การตั้งค่ามิเตอร์

เมื่อเพิ่มมิเตอร์ใหม่ คุณต้องระบุรายละเอียดต่อไปนี้:

1. Meter Name - ชื่อเพื่อช่วยคุณระบุมิเตอร์นี้ คุณสามารถให้ชื่อที่คุณต้องการ แต่จะต้องไม่ซ้ำกัน คุณจะไม่ได้รับอนุญาตให้สร้างมิเตอร์หลายตัวที่มีชื่อเดียวกัน
2. Description - คำอธิบายสั้น ๆ ของมิเตอร์นี้ - เพื่อความสะดวกของคุณเท่านั้น แอปพลิเคชันไม่ได้ใช้ข้อมูลนี้
3. Meter Type - ประเภทของมิเตอร์นี้ - คุณจะเลือกหนึ่งในประเภทสาธารณูปโภคที่คุณได้ตั้งค่าไว้ก่อนหน้านี้ (ตัวอย่าง: พลังงานหรือน้ำหรือขยะ)
4. Unit - หน่วยที่มิเตอร์นี้บันทึกข้อมูล นี่เป็นสิ่งที่สำคัญเพราะเมื่อข้อมูลถูกอัปโหลด/ส่ง/บันทึกสำหรับมิเตอร์นี้ จะถูกสมมุติว่าอยู่ในหน่วยที่คุณระบุที่นี่ ดังนั้นหากหน่วยฐานของคุณคือ 'kwh' แต่มิเตอร์ที่กำลังตั้งค่าใช้ btu ให้ระบุ btu เป็นหน่วย  เมื่อข้อมูลถูกบันทึก มันจะถูกแปลงจาก btu เป็น kwh โดยอัตโนมัติเมื่อข้อมูลถูกรับและเก็บรักษา
5. Serving Location - สถานที่ที่มิเตอร์นี้ให้บริการ เมื่อคุณวิเคราะห์ข้อมูลการใช้งานตามสถานที่ ข้อมูลสถานที่นี้จะถูกใช้เพื่อกำหนดมิเตอร์ที่ให้บริการและสนับสนุนสถานที่เฉพาะ
6. Tags - คุณสามารถใช้แท็กหลายตัวกับมิเตอร์ แท็กจำเป็นต้องถูกกำหนดไว้ล่วงหน้า ดูส่วน [configuring-tags.md](configuring-tags.md "mention") สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการทำงานของแท็ก\
   เพื่อเพิ่มแท็กใหม่ คลิกที่ปุ่ม 'Add Tag' จากนั้นเลือกประเภทแท็ก \
   เมื่อคุณเลือกประเภทแท็ก - คุณจะได้รับรายการของแท็กที่เป็นไปได้สำหรับประเภทแท็กนั้น คุณสามารถเลือกหนึ่งเพื่อนำมาใช้\
   คุณสามารถเลือกแท็กหนึ่งตัวของแต่ละประเภท แต่คุณสามารถเพิ่มประเภทแท็กที่คุณต้องการได้ไม่จำกัด
7. Baselines. คุณสามารถตั้งค่าค่าฐานสำหรับแต่ละค่าฐานที่คุณได้กำหนด ค่าเหล่านี้คือค่าฐานการใช้งานประจำวัน ดูส่วนการตั้งค่าค่าฐานสำหรับข้อมูลเพิ่มเติม
   1. Metadata - คุณสามารถตั้งค่าฟิลด์ที่กำหนดเองต่าง ๆ ภายใต้ส่วน 'metadata' ฟิลด์ที่กำหนดเองถูกกำหนดไว้ภายใต้ส่วนการตั้งค่า metadata ซึ่งอยู่ในส่วน 'Advanced'&#x20;

{% hint style="info" %}
การเปลี่ยนแปลงทั้งหมดจะถูกบันทึกเฉพาะเมื่อคุณกดปุ่ม 'Submit' การแก้ไขของคุณจะไม่ถูกบันทึกจนกว่าคุณจะทำเช่นนั้น
{% endhint %}