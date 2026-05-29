# Budget-Tracker

Mobile-first daily budget tracking web app.

แอปบันทึกรายรับรายจ่ายรายวันแบบ **mobile-first** สำหรับเช็กว่า “วันนี้ใช้เงินตามงบไหม?”

## Project Documents
- Context & Task Tracker: `docs/CONTEXT.md`

## Product Vision (ฉบับสั้น)
- ผู้ใช้ตั้งงบรายวัน
- บันทึกรายรับ/รายจ่ายระหว่างวันได้เร็วที่สุด
- เห็นสรุปทันทีว่า **เหลือ / เกินงบ / ขาดเท่าไหร่**
- ใช้คอมเมนต์จาก TikTok เป็นอินพุตพัฒนาฟีเจอร์ต่อเนื่อง

## MVP v1 (Industry Standard)
1. **Daily Budget Setup**
   - ตั้งงบต่อวัน (บาท)
2. **Quick Transaction Logging**
   - เพิ่มรายการ: ประเภท (รายรับ/รายจ่าย), จำนวนเงิน, หมวดหมู่, โน้ตสั้น, เวลา
3. **Today Summary**
   - รายรับรวม, รายจ่ายรวม, คงเหลือสุทธิ
   - สถานะ: อยู่ในงบ / ใกล้เกิน / เกินงบ
4. **Transaction List**
   - ดูรายการทั้งหมดของวันนี้, ลบ/แก้ไขได้
5. **Basic Insights**
   - สัดส่วนรายจ่ายตามหมวดหมู่ของวันนั้น

## Suggested Tech Stack (Web App)
> เน้นมาตรฐานอุตสาหกรรม, scale ได้, และส่งงานไว

- **Frontend:** Next.js (App Router) + TypeScript + Tailwind CSS
- **UI Components:** shadcn/ui
- **State/Form:** React Hook Form + Zod
- **Backend/API:** Next.js Route Handlers (หรือ tRPC ถ้าต้องการ type-safe end-to-end)
- **Database:** PostgreSQL + Prisma ORM
- **Auth (เผื่อ v1.1):** Clerk หรือ NextAuth
- **Analytics/Event Tracking:** PostHog
- **Hosting:** Vercel
- **Monitoring:** Sentry

## UI/UX Principles (Mobile-First)
1. **1-thumb usage**: ปุ่มหลักอยู่ล่างจอ, เพิ่มรายการได้ใน 1-2 tap
2. **Fast input**: preset หมวดหมู่ + ค่าที่ใช้บ่อย
3. **Readable status**: ใช้สี/ไอคอนชัดเจน (เขียว = อยู่ในงบ, แดง = เกินงบ)
4. **Zero-confusion copy**: ข้อความสั้น ตรง เช่น “เหลืออีก 220 บาท”
5. **Empty state ที่ดี**: ชวนให้เพิ่มรายการแรกทันที

> งานออกแบบ UI wireframe/high-fidelity สามารถทำต่อบน Google Stitch ได้ตามที่ต้องการ แล้วค่อย map กลับมาเป็น components ในโค้ด

## Data Model (เริ่มง่าย แต่ต่อยอดได้)
- `users`
- `daily_budgets` (date, amount)
- `transactions` (type, amount, category, note, happened_at)

## คืนนี้ควรเริ่มยังไง (First 3 Steps)
1. **Define scope ให้แคบมากก่อน**  
   เป้าคืนนี้: ตั้งงบ + เพิ่มรายจ่าย + สรุปคงเหลือวันนี้
2. **วาด flow มือถือก่อนโค้ด**  
   Screen หลัก: Home summary, Add transaction sheet, History list
3. **ตั้งโปรเจกต์ + ลงโครงสร้าง production-ready**  
   - Next.js + TypeScript + Tailwind + Prisma  
   - ตั้งค่า env, migration, basic logging, error boundary

## TikTok Feedback Loop (จุดเด่นไอเดียนี้)
1. ทำคลิปเล่าปัญหา + วิธีคิด product
2. ปิดท้ายด้วยคำถาม: “อยากให้เพิ่มฟีเจอร์อะไร?”
3. รวบรวมคอมเมนต์ใส่ backlog (Notion/Trello)
4. เลือก 1 ฟีเจอร์/สัปดาห์มาทำจริง
5. ทำคลิปอัปเดตว่า “ฟีเจอร์นี้มาจากคอมเมนต์ใคร”

## Definition of Done for MVP
- ผู้ใช้บันทึกรายการรายรับ/รายจ่ายได้จริงบนมือถือ
- เห็นผลรวมรายวันและสถานะงบแบบ real-time
- ไม่ต้องสอนการใช้งานก็เข้าใจได้ทันที