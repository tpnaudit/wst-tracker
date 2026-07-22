# WST Audit Tracker

ทะเบียนงบสอบบัญชีสำหรับ WST — เว็บแอปไฟล์เดียว (index.html)

- ข้อมูลเก็บใน localStorage ของเบราว์เซอร์ และ sync ข้ามเครื่องผ่าน repo ส่วนตัว `tpnaudit/wst-audit-data` (ไฟล์ `data.enc.json`, เข้ารหัส AES-256-GCM ด้วย PIN)
- โครงสร้าง/ฟีเจอร์เหมือน audit-tracker ของ TPN แต่ข้อมูลแยกกันคนละชุด (localStorage key ขึ้นต้น `wst...`)
- ตั้ง sync: กุญแจ (PAT) ถูกเข้ารหัสด้วย PIN ฝังใน `sync-token.enc.js` — เปิดลิงก์ + ใส่ PIN ครั้งเดียวต่อเครื่อง
