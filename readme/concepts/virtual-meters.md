# มิเตอร์เสมือนจริง

มิเตอร์เสมือนจริง - หรือ 'มิเตอร์ซอฟต์แวร์' - เป็นมิเตอร์ที่ถูกกำหนดในชั้นซอฟต์แวร์และมีค่าที่ได้มาจากมิเตอร์ทางกายภาพหนึ่งหรือมากกว่านั้น มักจะมีอาคารที่ไม่มีมิเตอร์สำหรับทุกๆ ระบบย่อยที่ต้องการวัด - แต่คุณสามารถคำนวณค่าพลังงานสำหรับระบบย่อยนั้นๆ ได้โดยการสืบทอดข้อมูลจากมิเตอร์ทางกายภาพอื่นๆ

ตัวอย่างเช่น ถ้าชั้นมีมิเตอร์สำหรับมัน (เราเรียกว่า F1) และแต่ละหน่วยภายในชั้นมีมิเตอร์ของตัวเอง (เราเรียกว่า U1 และ U2) แล้วเราสามารถวัดพลังงานทั้งหมดที่เข้าไปในชั้น และพลังงานที่เข้าไปในแต่ละหน่วย

แต่พลังงานที่ถูกบริโภคโดยพื้นที่ส่วนกลางในชั้นล่ะ? ไม่มีมิเตอร์แยกเพื่อวัด แต่เราสามารถ _คำนวณ_ ได้โดยการนำการบริโภคจาก F1 และลบการบริโภคจาก U1 และ U2 พลังงานที่เหลือคือพลังงานของพื้นที่ส่วนกลางในชั้น

ในกรณีนี้ คุณสามารถกำหนดมิเตอร์เสมือนจริงที่เรียกว่า 'CA1' เพื่อแทนการบริโภคพลังงานของพื้นที่ส่วนกลาง และคุณสามารถกำหนดค่าให้มันตามสูตร `F1 - U1 - U2`

เมื่อกำหนดค่ามิเตอร์เสมือนจริง คุณต้องระบุตำแหน่งที่ให้บริการ ชื่อ และแท็ก นอกจากนี้คุณยังต้องระบุมิเตอร์ที่มิเตอร์เสมือนจริงนี้สืบทอดข้อมูลของมันมา และปัจจัยการสเกลสำหรับแต่ละมิเตอร์

ใช้ตัวอย่างด้านบน - `F1 - U1 - U2`, คุณจะเพิ่ม 3 มิเตอร์และปัจจัยการสเกลที่สอดคล้องดังนี้:

| มิเตอร์ | ปัจจัยการสเกล |
| ----- | -------------- |
| F1    | 1              |
| U1    | -1             |
| U2    | -1             |

#### หน่วยสำหรับมิเตอร์เสมือนจริง

มิเตอร์เสมือนจริงสามารถคำนวณจากมิเตอร์ที่มีหน่วยต่างกัน การบริโภคทั้งหมดสำหรับมิเตอร์เสมือนจริงจะถูกเก็บในหน่วยฐานของประเภทสาธารณูปโภค ดังนั้นถ้าคุณได้กำหนดมิเตอร์น้ำเสมือนจริงและประเภทสาธารณูปโภค `น้ำ` มี 'แกลลอนอิมพีเรียล' เป็นหน่วยฐาน (เช่น ปัจจัยการแปลงของหน่วยคือ 1) แล้วข้อมูลการบริโภคของมิเตอร์เสมือนจริงทั้งหมดจะถูกคำนวณในแกลลอนอิมพีเรียล ไม่ว่าหน่วยของมิเตอร์ที่มิเตอร์เสมือนจริงได้รับมาจากจะเป็นอย่างไร

#### การคำนวณการบริโภค

การบริโภคสำหรับมิเตอร์เสมือนจริงจะถูกคำนวณโดยอัตโนมัติเมื่อข้อมูลการบริโภคถูกบันทึกในมิเตอร์ที่อยู่ภายใต้มิเตอร์เสมือนจริง