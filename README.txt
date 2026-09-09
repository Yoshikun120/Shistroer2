SHI STORE - REAL VERSION

Supabase Project:
https://xybgzgjjefdongycvfms.supabase.co

ระบบที่เชื่อมจริง:
- สมัคร/เข้าสู่ระบบด้วย Supabase Auth
- โปรไฟล์ + ที่อยู่จัดส่ง
- สินค้า/หมวดหมู่/สต็อก
- ตะกร้า + checkout ผ่าน RPC create_order (ราคา/สต็อกตรวจฝั่งฐานข้อมูล)
- Wallet
- เติมเงินด้วยบัญชี/QR + อัปโหลดสลิป
- แอดมินอนุมัติ/ปฏิเสธเติมเงิน
- ถอนเงิน + แอดมินอนุมัติ/ปฏิเสธ (ปฏิเสธแล้วคืนเงิน)
- ประวัติธุรกรรม
- คำสั่งซื้อ + สถานะ + เลขพัสดุ
- จัดการสินค้า/บัญชีรับเงิน/แบนเนอร์
- Storage แยก QR, สลิป, รูปสินค้า
- RLS

ความปลอดภัย:
ไฟล์นี้ใช้ publishable key เท่านั้น ห้ามนำ service_role key มาใส่ใน frontend

สิ่งที่ต้องทำก่อนเปิดใช้งานจริง:
1) สมัครบัญชีผู้ใช้ผ่านหน้าเว็บ
2) นำ UUID ของบัญชีที่จะเป็นแอดมินไปเพิ่มใน public.admin_roles
   SQL:
   insert into public.admin_roles(user_id) values ('USER_UUID_HERE');
3) ตั้งค่า Supabase Auth URL / redirect ให้ตรงกับโดเมนที่จะใช้
4) อัปโหลดโฟลเดอร์นี้ขึ้น GitHub Pages / Cloudflare Pages / โฮสต์ static ใดก็ได้
5) ถ้าต้องการใช้โดเมนของตัวเอง ให้ชี้ DNS ไปยังโฮสต์ที่เลือก

เพลงพื้นหลัง:
ssstik.io_1788973689173.mp3
