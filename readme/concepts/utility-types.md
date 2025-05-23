# ประเภทยูทิลิตี้

ประเภทยูทิลิตี้กำหนดประเภทของยูทิลิตี้ที่คุณต้องการวัดและวิเคราะห์ ซึ่งโดยทั่วไปจะเป็น:

* ไฟฟ้า
* น้ำ
* ก๊าซ
* น้ำเย็น
* ขยะ ฯลฯ...

คุณสามารถเพิ่มประเภทยูทิลิตี้เหล่านี้ลงในระบบ แต่ละประเภทยูทิลิตี้สามารถวัดได้ในหน่วยที่แตกต่างกัน คุณสามารถกำหนดหน่วยที่แตกต่างกันสำหรับแต่ละประเภทยูทิลิตี้ ตัวอย่างเช่น ไฟฟ้าสามารถบันทึกได้ในหน่วย kWh หรือ mWh หรือ BTU

#### หน่วย

ภายในแต่ละประเภทยูทิลิตี้ คุณจำเป็นต้องกำหนดหน่วยที่เป็นไปได้ที่สามารถวัดได้ สำหรับแต่ละหน่วย - คุณต้องให้ชื่อและปัจจัยการแปลง ปัจจัยการแปลงคือตัวคูณเพื่อแปลงหน่วยนั้นเป็นหน่วยฐาน

คุณสามารถกำหนดหน่วยฐานโดยการให้ปัจจัยการแปลงเป็นหนึ่ง

ตัวอย่างเช่น หากคุณเก็บปริมาณน้ำ คุณอาจต้องการกำหนดหน่วยต่อไปนี้:

* ลิตร
* แกลลอนสหรัฐ
* แกลลอนอิมพีเรียล

หากเราเลือกลิตรเป็นหน่วยฐาน แล้วปัจจัยการแปลงต่อไปนี้สามารถใช้ได้:

* ลิตร - 1
* แกลลอนสหรัฐ - 3.785
* แกลลอนอิมพีเรียล - 4.546

หากเราต้องการเลือกแกลลอนสหรัฐเป็นหน่วยฐาน ปัจจัยการแปลงต่อไปนี้สามารถใช้ได้:

* ลิตร - 0.2642 (1/3.785)
* แกลลอนสหรัฐ - 1
* แกลลอนอิมพีเรียล - 1.20095

###