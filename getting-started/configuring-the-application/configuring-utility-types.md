# การกำหนดค่า Utility Types

คุณสามารถกำหนดค่า Utility Types หลายรูปแบบในแอปพลิเคชัน

ไปที่ส่วน Configuration แล้วไปที่แท็บ 'Meter Types' เพื่อกำหนดค่า Utility Types ต่างๆ

{% hint style="info" %}
เราใช้คำว่า 'meter type' และ 'utility type' แทนกัน&#x20;
{% endhint %}

ที่นี่คุณสามารถดู Utility Types ที่มีอยู่แล้ว แก้ไข และเพิ่มประเภทใหม่

คลิกที่ปุ่ม 'Add Item' ที่มุมขวาบนเพื่อเพิ่ม Utility Type ใหม่

คุณสามารถคลิกที่ปุ่ม 'edit' ที่อยู่ใต้ Utility Type เพื่อแก้ไขคุณสมบัติ

คุณยังสามารถลบ Utility Types ได้โดยคลิกที่ไอคอนลบ (ถังขยะ)

{% hint style="warning" %}
การลบเหมือนกับเพชร คือตลอดไป กรุณาอย่าลบ Utility Types นอกจากคุณได้สร้างมันขึ้นมาโดยไม่ได้ตั้งใจ&#x20;
{% endhint %}



## การกำหนดค่า Utility Types

ไม่ว่าคุณจะเพิ่ม Utility Type ใหม่หรือแก้ไขที่มีอยู่แล้ว หน้าตาของอินเทอร์เฟซที่ใช้ทำงานนั้นคล้ายกัน

คุณมีตัวเลือกในการระบุหน่วยที่รองรับสำหรับ Utility Type นี้

การกำหนดค่าหน่วยเป็นสิ่งสำคัญ คุณจำเป็นต้องมีอย่างน้อยหนึ่งหน่วยสำหรับแต่ละ Utility Type



## การเข้าใจ Units

แต่ละ Utility Type สามารถรองรับหน่วยหลายหน่วยที่ใช้บันทึกการบริโภค

สำหรับไฟฟ้า - อาจเป็น `mWh` หรือ `kWh`

สำหรับน้ำเย็น อาจเป็น `mWh` หรือ `btu`

สำหรับการบริโภคขยะ อาจเป็น \`kg\`

สำหรับน้ำ อาจเป็นลิตรหรือแกลลอน

แต่ละ Utility Type มี **base unit** หนึ่งหน่วย

แล้วหน่วยอื่นๆ จะถูกกำหนดค่าตามหน่วยพื้นฐาน

แต่ละหน่วยถูกกำหนดค่าด้วย _conversion factor_ ที่กำหนดว่ามันสามารถแปลงเป็นหน่วยพื้นฐานได้อย่างไร

หน่วยพื้นฐานมี conversion factor เป็น 1 เสมอ

{% hint style="info" %}
วิธีที่คุณกำหนดหน่วยพื้นฐานคือโดยการกำหนดหน่วยใหม่และให้ conversion factor เป็น 1 ซึ่งจะทำให้มันกลายเป็นหน่วยพื้นฐานของคุณ
{% endhint %}

{% hint style="info" %}
คุณสามารถมีหน่วยพื้นฐานหลายหน่วยได้หรือไม่ โดยการกำหนดหน่วยหลายหน่วยและให้ conversion factor เป็น 1 จริงๆ แล้วคุณสามารถทำได้ แต่มันจะไม่มีประโยชน์อะไร
{% endhint %}



หน่วยพื้นฐานเป็นสิ่งสำคัญ - โดยค่าเริ่มต้น ข้อมูลทั้งหมดจะถูกแปลงเป็นหน่วยพื้นฐานเมื่อบันทึกและหน่วยเริ่มต้นสำหรับการรายงานจะเป็นหน่วยพื้นฐาน