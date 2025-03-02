# การอ่านค่า, การบริโภค และ ความต้องการ

ดังนั้นเราทราบว่ามิเตอร์สามารถบันทึกข้อมูลการบริโภค และทั้งมิเตอร์เสมือนและกลุ่มมิเตอร์สามารถคำนวณการบริโภคโดยอาศัยมิเตอร์ภายใต้และตัวคูณการปรับขนาดของพวกเขา

ดังนั้นหมายความว่า มิเตอร์ทางกายภาพเท่านั้นที่สามารถ _บันทึก_ การบริโภค สำหรับองค์กรอื่น ๆ การบริโภคจะถูก _คำนวณ_

คุณจะบันทึกการบริโภคสำหรับมิเตอร์ทางกายภาพอย่างไร? มีวิธีหลายวิธี:&#x20;

1. บันทึกการอ่านค่ามิเตอร์
2. บันทึกการบริโภค
3. บันทึกการโหลด/ความต้องการ

### การบันทึกการอ่านค่ามิเตอร์

โดยการบันทึกการอ่านค่ามิเตอร์ - การอ่านค่ามิเตอร์หมายถึงตรงนั้น - การอ่านค่าบนมิเตอร์ทางกายภาพจริง นี่จะเป็นค่าสะสมที่เพิ่มขึ้นเสมอ เมื่อการอ่านค่าถูกบันทึก การบริโภคจะถูกคำนวณเป็นความแตกต่างระหว่างการอ่านค่าปัจจุบันและการอ่านค่าก่อนหน้า

ข้อมูลการบริโภคจะถูกแก้ไขในระหว่างเวลาจากการอ่านค่าล่าสุดถึงการอ่านค่าปัจจุบัน และการเปลี่ยนแปลงในการบริโภคถือว่าเป็นเชิงเส้นในช่วงเวลานี้

เพื่อให้แน่ใจว่ามีความแม่นยำ ตรวจสอบให้แน่ใจว่าช่วงระหว่างการอ่านค่าไม่ยาวเกินไป

การอ่านค่าสามารถบันทึกได้หลายวิธี:

1. API
2. การรวมที่มีอยู่แล้ว
3. ป้อนค่าอ่านด้วยตนเองในอินเทอร์เฟซ

ดูส่วน 'การรวม' สำหรับข้อมูลเพิ่มเติม



### การบันทึกการบริโภค

บางครั้ง มิเตอร์อาจไม่ให้คุณอ่านค่าสะสม ตัวอย่างเช่น ถ้าคุณกำลังบันทึกข้อมูลจากมิเตอร์พลังงาน IoT คุณอาจได้รับการบริโภคจริงสำหรับช่วงเวลาที่กำหนด มันเป็นไปได้ที่จะบันทึกข้อมูลการบริโภคนั้นโดยตรงด้วย สิ่งนี้สามารถทำได้ผ่าน API ของมิเตอร์



### การบันทึกการโหลดหรือความต้องการ

บางครั้งกับมิเตอร์พลังงาน มันอาจให้คุณ _ความต้องการ_ ทันทีปัจจุบัน การบริโภคสามารถคำนวณอัตโนมัติจากความต้องการทันที

เมื่อการอ่านค่าความต้องการถูกบันทึก การบริโภคจะถูกคำนวณสำหรับช่วงระหว่างการอ่านค่าความต้องการสองครั้งโดยการคำนวณ 'พื้นที่ใต้กราฟ' ใช้กฎของ Trapezium โดยสมมติว่าการเติบโตเชิงเส้นในการบริโภคระหว่างการอ่านค่าความต้องการสองครั้ง

การบริโภคนั้นจะถูกแก้ไขในแบบเชิงเส้นตลอดช่วงเวลา