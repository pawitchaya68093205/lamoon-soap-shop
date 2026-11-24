# ละมุน — Handmade Soap Shop

เว็บไซต์ตัวอย่างขายสบู่ภาษาไทย มีสินค้า 2 SKU, ตะกร้าสินค้า, แบบฟอร์มข้อมูลจัดส่ง และหน้ารายการเตรียมแพ็กสินค้า/พิมพ์ใบจัดส่ง

## เปิดดูเว็บไซต์
เปิดไฟล์ `index.html` ด้วยเว็บเบราว์เซอร์ได้ทันที

## ไฟล์ในโปรเจกต์
- `index.html` — เว็บไซต์ทั้งหมด (HTML/CSS/JavaScript)
- `products.csv` — ตารางข้อมูลสินค้าเริ่มต้น สามารถนำเข้า Google Sheets ได้

## นำข้อมูลเข้า Google Sheets
1. เปิด Google Sheets แล้วสร้าง Spreadsheet ใหม่
2. เลือก File > Import > Upload แล้วเลือก `products.csv`
3. ตั้งชื่อชีตว่า `Products`
4. แชร์สิทธิ์เป็น General access > Anyone with the link > Viewer
5. คัดลอกลิงก์ Google Sheets เพื่อใช้ส่งงาน

## อัปโหลด GitHub
1. สมัคร/เข้าสู่ระบบ GitHub
2. สร้าง repository ใหม่ ตั้งชื่อ `lamoon-soap-shop`
3. เลือก Public
4. อัปโหลด `index.html`, `products.csv` และ README.md

## Deploy บน Vercel
1. สมัคร/เข้าสู่ระบบ Vercel ด้วย GitHub
2. กด Add New > Project แล้วเลือก repository `lamoon-soap-shop`
3. กด Deploy (ไม่ต้องตั้งค่า Build Command)
4. เมื่อเสร็จแล้วคัดลอกโดเมน `.vercel.app`

## ข้อจำกัดของรุ่นตัวอย่างนี้
- คำสั่งซื้อถูกเก็บใน localStorage ของเบราว์เซอร์ที่ใช้สาธิตเท่านั้น ไม่ได้ส่งเข้าร้านหรือ Google Sheets อัตโนมัติ
- ข้อมูลสินค้าในหน้าเว็บเป็นตัวอย่าง ต้องแก้ในตัวแปร `products` ใน `index.html` ให้ตรงกับชีต หรือพัฒนาการเชื่อม Google Sheets เพิ่มเติม
- ไม่มีระบบชำระเงิน/คำนวณค่าขนส่ง/ตัดสต็อกจริง
- รายการจัดส่งและใบแพ็กพิมพ์ได้จากเบราว์เซอร์

## ปรับสินค้า
แก้รายการใน `index.html` ตรง `const products = [...]` และปรับข้อมูลใน `products.csv` ให้ตรงกัน
