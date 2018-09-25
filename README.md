# ระบบแจ้งซ่อมครุภัณฑ์

เป็นระบบบริหารงานพัสดุและครุภัณฑ์ รวมกับ ระบบแจ้งซ่อม เหมาะสำหรับใช้งานภายในองค์กร โดยจะเป็นการแจ้งซ่อมพัสดุภายใน ที่ต้องมีการลงทะเบียนอุปกรณ์ก่อน
และผู้แจ้งซ่อมต้องเป็นสมาชิกเท่านั้น เช่น อุปกรณ์คอมพิวเตอร์ภายในสำนักงาน หรือ หอพัก ห้องพัก โรงแรม

รายละเอียดเพิ่มเติม https://www.kotchasan.com/index.php?module=knowledge&id=100

## ความต้องการของระบบ

- PHP 5.3 ขึ้นไป
- ext-mbstring
- PDO Mysql

## การติดตั้งและการอัปเกรด

1.  ให้อัปโหลดโค้ดทั้งหมดจากที่ดาวน์โหลด ขึ้นไปบน Server
2.  ในกรณีที่มีการติดตั้งใหม่ ให้เรียกตัวติดตั้ง http://domain.tld/install/ และดำเนินการตามขั้นตอนการติดตั้งจนกว่าจะเสร็จสิ้น
3.  ลบไดเร็คทอรี่ install/ ออก
4.  ในกรณีเป็นการอัปเกรด สามารถนำไฟล์ทั้งหมดไปแทนที่ไฟล์เดิม ยกเว้นไดเร็คทอรี่ install/ และให้ดำเนินการต่อไปนี้ที่ฐานข้อมูล

เปิดตาราง `xxx_user` (xxx คือ prefix ของตาราง) ด้วย phpMyAdmin คอลัมน์ `password` ให้เพิ่มความยาวตัวอักษรเป็น 50 ตัวอักษร
และคอลัมน์ `fb` ให้เปลี่ยนชื่อเป็น `social`

## การใช้งาน

- เข้าระบบเป็นผู้ดูแลระบบ : `admin@localhost` และ Password : `admin`
- เข้าระบบเป็นช่างซ่อม : `demo@localhost` และ Password : `demo`
- เข้าระบบเป็นช่างซ่อม : `demo2@localhost` และ Password : `demo`

## ข้อตกลงการนำไปใช้งาน

- สามารถนำไปใช้งานส่วนตัวได้
- สามารถพัฒนาต่อยอดได้
- มีข้อสงสัยสามารถสอบถามได้ที่บอร์ดของคชสาร https://www.kotchasan.com
- ต้องการให้ผู้เขียนพัฒนาเพิ่มเติม ติดต่อผู้เขียนได้โดยตรง (อาจมีค่าใช้จ่าย)
- ผู้เขียนไม่รับผิดชอบข้อผิดพลาดใดๆในการใช้งาน
- ห้ามขาย ถ้าต้องการนำไปพัฒนาต่อเพื่อขายให้ติดต่อผู้เขียนก่อน (เพื่อบริจาค)

## หากต้องการสนับสนุนผู้เขียน สามารถบริจาคช่วยเหลือค่า Server ได้ที่

```
ธนาคาร กสิกรไทย สาขากาญจนบุรี
เลขที่บัญชี 221-2-78341-5
ชื่อบัญชี กรกฎ วิริยะ
```
