# การตั้งค่ามิเตอร์ใหม่

สำหรับมิเตอร์ที่บันทึกการอ่านค่าสะสม, การตั้งค่ามิเตอร์ใหม่จะเกิดขึ้นโดยอัตโนมัติ

หากการอ่านค่าล่าสุดน้อยกว่าค่าก่อนหน้านี้, จะมีช่องว่างชั่วคราวในค่าพลังงานในเวลาที่ทำการตั้งค่าใหม่

ต่อมา, เมื่อมีการอ่านค่าถัดไปเข้ามา - ค่านี้จะถูกคำนวณขึ้นมาจากการอ่านค่าก่อนหน้าที่ถูกส่ง

โปรดทราบว่า การอ่านค่าที่เป็น '0' (ศูนย์) จะถูกละทิ้งอย่างเงียบ ๆ และถือว่าเป็นข้อผิดพลาดในการสื่อสารหรือข้อผิดพลาดในการรวมข้อมูล ดังนั้นหากมีการบันทึกการอ่านค่าในขณะที่ทำการตั้งค่าใหม่, ค่านี้จะไม่ถูกใช้จนกว่าการอ่านค่าถัดไปจะถูกส่งมา