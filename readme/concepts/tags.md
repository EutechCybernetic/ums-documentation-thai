# แท็ก

แท็กเป็นคุณสมบัติที่มีประโยชน์ในการจัดระเบียบและจัดแคตตาล็อกข้อมูลการใช้งานสาธารณูปโภคในทางที่แตกต่างกันและเป็นการกำหนดเอง คุณสามารถใช้แท็กหลายตัวกับเมตร, เมตรเสมือนหรือกลุ่มเมตร คุณจึงสามารถวิเคราะห์ข้อมูลการใช้งานตามแท็ก ทุกเมตรที่มีแท็กเดียวกันจะมีข้อมูลการใช้งานรวมกัน เช่น หากมีผู้เช่าหลายคนในอาคารและแต่ละคนมีเมตรหลายตัว คุณสามารถใช้แท็กเมตรหรือกลุ่มเมตรที่แตกต่างกันด้วยชื่อผู้เช่า แล้ววิเคราะห์ข้อมูลการใช้งานตามชื่อผู้เช่า

เพื่อให้มีโครงสร้างและรับรองว่าข้อมูลสะอาด คุณต้องกำหนดแท็กของคุณล่วงหน้า

คุณเริ่มต้นด้วยการกำหนด 'ประเภทแท็ก' - เช่น 'ผู้เช่า' คุณจึงสามารถกำหนดรายการหลายรายการภายใต้แท็ก 'ผู้เช่า' คุณสามารถเพิ่มแท็กสำหรับแต่ละผู้เช่า - 'ACME', 'Blueberry Electronics', 'Verper Stationary' ฯลฯ..

สิ่งที่ทำให้แท็กน่าสนใจมากขึ้นคือพวกเขาสามารถปฏิบัติตามโครงสร้างต้นไม้แบบลำดับชั้น

#### ต้นไม้แท็ก

คุณสามารถกำหนดแท็กที่มีแท็กแม่และแท็กลูก คุณสามารถสร้างแท็กและแท็กย่อยและแท็กย่อยย่อยและคงทำต่อไป ข้อดีของสิ่งนี้คือเมื่อคุณต้องการวิเคราะห์ข้อมูลการใช้งานสำหรับแท็ก มันจะรวมแท็กย่อยทั้งหมด (หรือแท็กลูก) ด้วย เช่น หากผู้เช่า 'Sunbucks Coffee' มีร้าน 2 แห่งในอาคารพาณิชย์ คุณสามารถกำหนดโครงสร้างแท็กสำหรับผู้เช่าดังนี้:

* ผู้เช่า
  * อาหารและเครื่องดื่ม
    * Sunbucks Coffee
      * ชั้นล่าง
      * ชั้น 3
    * Don Pepe

คุณจึงสามารถใช้แท็กเมตรเป็น `ผู้เช่า/อาหารและเครื่องดื่ม/Sunbucks Coffee/ชั้นล่าง` หรือ `ผู้เช่า/อาหารและเครื่องดื่ม/Sunbucks Coffee/ชั้น 3`.

คุณสามารถวิเคราะห์ข้อมูลสำหรับแต่ละเมตร หรือหากคุณเลือกวิเคราะห์ข้อมูลสำหรับ `ผู้เช่า/อาหารและเครื่องดื่ม/Sunbucks Coffee` ข้อมูลจาก `ชั้นล่าง` และ `ชั้น 3` จะถูกรวมอย่างอัตโนมัติ

หากคุณวิเคราะห์ข้อมูลสำหรับแท็ก `ผู้เช่า/อาหารและเครื่องดื่ม` มันจะรวมข้อมูลการใช้งานจากเมตรที่มีแท็ก `Don Pepe` ด้วย

การมีโครงสร้างแบบต้นไม้ช่วยให้คุณสามารถแยกและวิเคราะห์ข้อมูลแบบเดี่ยวหรือเป็นกลุ่ม