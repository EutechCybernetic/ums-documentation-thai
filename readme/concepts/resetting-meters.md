# การตั้งค่ามิเตอร์ใหม่

สำหรับมิเตอร์ที่บันทึกการอ่านแบบสะสม, การตั้งค่ามิเตอร์ใหม่จะเกิดขึ้นโดยอัตโนมัติ

หากการอ่านครั้งล่าสุดน้อยกว่าครั้งก่อนหน้า, จะมีช่องว่างชั่วคราวในค่าพลังงานในเวลาที่การตั้งค่าใหม่

ต่อมา, เมื่อการอ่านครั้งถัดไปเข้ามา - จะถูกคำนวณตามการอ่านครั้งก่อนหน้าที่ถูกส่ง



โปรดทราบว่า การอ่านที่เป็น '0' (ศูนย์) จะถูกลบออกอย่างเงียบ ๆ และถูกจัดการเป็นข้อผิดพลาดในการสื่อสารหรือข้อผิดพลาดในการรวมเข้าด้วยกัน ดังนั้นหากมีการบันทึกการอ่านในขณะที่ตั้งค่าใหม่, มันจะไม่ถูกใช้จนกว่าการอ่านครั้งถัดไปจะถูกส่ง