MEILIEX MINI APP V2 — ตรงกับ Preview ล่าสุด

วิธีอัปโหลด GitHub Pages
1. แตกไฟล์ ZIP
2. เปิด Repository mbot-mini-app
3. ลบไฟล์เวอร์ชันเก่า
4. อัปโหลดไฟล์ทั้งหมดที่อยู่ภายในโฟลเดอร์นี้
5. กด Commit changes และรอ 1–3 นาที

การเปลี่ยนรูปกิจกรรม
- ใช้รูปขนาด 1:1
- ตั้งชื่อ activity.png
- วางตำแหน่งเดียวกับ index.html

การแก้สถานะ
- เปิด index.html และค้นหา const streamers
- คนกำลังไลฟ์ใช้ live:true
- คนออฟไลน์ใช้ live:false

หมายเหตุ
- communityLinks ยังต้องใส่ลิงก์ Telegram จริง
- สถานะยังเป็นระบบแก้ไขเอง จนกว่าจะเชื่อม Twitch API
TWITCH LIVE STATUS
- เชื่อมต่อ API: https://meiliex-live-status-api.worker7889.workers.dev/
- ตรวจสอบสถานะทันทีเมื่อเปิดหน้า และอัปเดตทุก 60 วินาที
- Client Secret เก็บใน Cloudflare Worker เท่านั้น ห้ามใส่ใน index.html
- หาก API ติดต่อไม่ได้ หน้าเว็บจะเก็บสถานะล่าสุดไว้และแสดง "เชื่อมต่อไม่ได้"
