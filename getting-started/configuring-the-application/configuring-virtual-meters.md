# การกำหนดค่าเมตรเสมือน

การกำหนดค่าเมตรเสมือนเหมือนกับการกำหนดค่าเมตรทางกายภาพ ยกเว้นว่ามีการกำหนดค่าเพิ่มเติมสำหรับสูตรของเมตรเสมือน

สูตรถูกกำหนดโดยการเลือกเมตรทางกายภาพหนึ่งหรือหลายตัว และใช้ปัจจัยการปรับขนาดกับแต่ละเมตร (ปัจจัยการปรับขนาดสามารถเป็นลบหรือเป็นส่วนหนึ่ง)

ดังนั้น ถ้าคุณต้องการกำหนดเมตรเสมือนเป็นผลรวมของเมตร A และ B และลบด้วยเมตร C, คุณจะต้องเพิ่มเมตรและปัจจัยการปรับขนาดดังต่อไปนี้:

| เมตร | ปัจจัยการปรับขนาด |
| ----- | -------------- |
| A     | 1              |
| B     | 1              |
| C     | -1             |

สิ่งนี้จะทำให้ได้สูตร `Ax1 + Bx1  + Cx-1` ที่ถูกนำไปใช้สำหรับเมตรเสมือนนั้น