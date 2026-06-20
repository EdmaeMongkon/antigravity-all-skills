# Global Antigravity Rules
> โหลดทุกครั้งที่เริ่มต้น `agy` — ทำให้ผมฉลาดขึ้นตั้งแต่วินาทีแรก

---

## 🌏 ภาษา

- **ตอบภาษาไทยเสมอ** ไม่ว่า prompt จะเป็นภาษาอะไร
- ยกเว้น code, terminal commands, ชื่อ library/package — ใช้ภาษาอังกฤษตามปกติ
- ห้ามขึ้นต้นด้วย "สวัสดีครับ" หรือ "ยินดีต้อนรับ" ทุกครั้ง — ตอบตรงเรื่องเลย

---

## ✅ ก่อนลงมือเขียนโค้ด — สรุปแผนก่อนเสมอ

**ทุกครั้งที่งานมีการเปลี่ยน/สร้างไฟล์มากกว่า 1 ไฟล์:**
1. สรุปแผนเป็นขั้นตอนสั้นๆ ว่าจะทำอะไรบ้าง
2. ระบุไฟล์ที่จะสร้าง/แก้ไข
3. รอ approve ก่อนลงมือ

**ยกเว้น:** งานเล็กๆ ไฟล์เดียว หรือแก้ bug ที่ชัดเจน — ทำเลยได้

---

## 🎨 Web Design / UI — ออกแบบสวยตั้งแต่ต้น

- **ห้ามออกแบบแบบ plain/minimal** โดยไม่ได้รับคำสั่ง
- ใช้ **dark mode, glassmorphism, gradient, micro-animation** เป็น default
- Typography: ดึง Google Fonts (Inter, Outfit, DM Sans ฯลฯ) เสมอ
- สี: ใช้ HSL palette ที่ curated ไม่ใช่ plain red/blue/green
- ทุก interactive element ต้องมี hover state และ transition
- **Mobile responsive** เป็น requirement ไม่ใช่ option

---

## 🔧 Tech Stack ที่ใช้

```
Frontend:   Next.js 14+ (App Router), TypeScript, Tailwind CSS v4
Backend:    Node.js / Bun, REST API หรือ tRPC
Database:   PostgreSQL / Prisma, หรือ Supabase
Styling:    Tailwind v4 + Vanilla CSS สำหรับ animations
State:      Zustand หรือ React Context
Auth:       NextAuth.js หรือ Supabase Auth
```

- เมื่อสร้างโปรเจกต์ใหม่ — ถามว่าใช้ stack ไหนก่อน ถ้าไม่บอก default = Next.js + TypeScript + Tailwind
- ใช้ `pnpm` เป็น package manager default
- ใช้ `npx -y` สำหรับ CLI tools

---

## 🤖 Open Design Workflow

- Open Design คือ **local-first, open-source Claude Design alternative**
- รัน via Docker ที่ `http://localhost:7456`
- เชื่อมกับ Antigravity ผ่าน MCP (`od mcp install antigravity`)
- ใช้ **DESIGN.md** เป็น brand contract ของแต่ละโปรเจกต์
- Skills อยู่ใน `/Users/mekrua/.agents/skills/`
- เมื่อผู้ใช้พูดถึง Open Design — รู้ว่าเป็น workflow tool ไม่ใช่ library

---

## 🗂️ โปรเจกต์ในเครื่อง — Context สำคัญ

| โปรเจกต์ | Path | ทำอะไร |
|----------|------|---------|
| `here-we-go-again-admin` | `/Users/mekrua/here-we-go-again-admin` | Admin panel ของระบบ here-we-go-again |
| `here-we-go-again-admin-api` | `/Users/mekrua/here-we-go-again-admin-api` | API backend สำหรับ admin |
| `here-we-go-again-collectibles` | `/Users/mekrua/here-we-go-again-collectibles` | Collectibles / NFT marketplace |
| `here-we-go-again-storefront` | `/Users/mekrua/here-we-go-again-storefront` | หน้าร้านค้า storefront |
| `Kitchen-Hub-Admin` | `/Users/mekrua/Kitchen-Hub-Admin` | Admin panel ร้านอาหาร |
| `Kitchen-Hub-Storefront` | `/Users/mekrua/Kitchen-Hub-Storefront` | หน้าร้าน Kitchen Hub |
| `black-cafe-restaurant` | `/Users/mekrua/black-cafe-restaurant` | เว็บร้านกาแฟ Black Cafe |
| `black-fitness` | `/Users/mekrua/black-fitness` | เว็บ fitness / gym |
| `agent-dashboard-next` | `/Users/mekrua/agent-dashboard-next` | Dashboard ด้วย Next.js |
| `hyperframes-demo` | `/Users/mekrua/hyperframes-demo` | Demo HyperFrames video |
| `phukaew-pochana` | `/Users/mekrua/phukaew-pochana` | เว็บร้านอาหารภูแก้วโภชนา |
| `pos-food` | `/Users/mekrua/pos-food` | ระบบ POS ร้านอาหาร |
| `premium-dining-pos` | `/Users/mekrua/premium-dining-pos` | POS premium dining |
| `remix-portfolio` | `/Users/mekrua/remix-portfolio` | Portfolio ด้วย Remix |
| `s-portfolio` | `/Users/mekrua/s-portfolio` | Portfolio เวอร์ชันอื่น |
| `tiktok-return-app` | `/Users/mekrua/tiktok-return-app` | แอป TikTok return flow |

> เมื่อผู้ใช้พูดถึงโปรเจกต์ — ให้รู้ path ทันทีโดยไม่ต้องถาม

---

## 💾 Git Commit Rules — ใช้ Conventional Commits เสมอ

- ใช้มาตรฐาน **Conventional Commits** เสมอ: `type(scope): description`
  - `feat:` เพิ่มฟีเจอร์ใหม่
  - `fix:` แก้ไขบั๊ก
  - `docs:` อัปเดตเอกสาร/ReadMe
  - `style:` ปรับแต่งรูปแบบโค้ด
  - `refactor:` จัดโครงสร้างโค้ดใหม่
  - `test:` เพิ่ม/แก้ไข test
  - `chore:` อัปเดต config / dependencies
- **อธิบายผลลัพธ์ (Outcome) เสมอ** แทนที่จะเขียนแค่สิ่งที่ทำหรือไฟล์ที่แก้
- **1 Commit = 1 เป้าหมาย** ห้ามรวมหลายเรื่อง
- ใช้ภาษาอังกฤษเป็นหลักสำหรับ Commit Message


---

## 🖼️ Google Flow Image Prompt Generator (Product Shot)

เมื่อผู้ใช้ส่งรายละเอียดสินค้าหรือรูปภาพมาเพื่อให้ช่วยสร้าง Prompt สำหรับ Google Flow:
- ให้ใช้โครงสร้าง Prompt ต้นแบบนี้ในการสร้างและปรับปรุง:
  `Create a hyper-realistic 3D commercial-style product shot of a [main bottled beverage or product], floating mid-air with detailed cold condensation on its surface. Surround it with dynamic elements like [splashing elements or garnish], frozen in high-speed motion with vibrant clarity and natural physics. Add sharp droplets, [floating accent ingredient or object], and vivid details to convey freshness and energy. Use [background color or gradient] to amplify the brand tone, and emphasize a clean, luxurious, premium look. Studio-style cinematic lighting with bright highlights, crisp reflections, and high contrast. Product must always be centered, upright or slightly angled in mid-air, casting subtle shadows or reflections. Aspect ratio: 3:4. Ultra-HD quality. Photographic realism.`
- วิเคราะห์สินค้าหลัก, องค์ประกอบสาดน้ำ/เครื่องตกแต่ง, วัตถุดิบเด่นรอบๆ และโทนสีพื้นหลัง จากข้อมูลหรือรูปภาพของผู้ใช้เพื่อนำไปแทนค่าในวงเล็บ `[...]`
- ตอบกลับด้วย Prompt ภาษาอังกฤษฉบับสมบูรณ์เพื่อให้ผู้ใช้คัดลอกไปใช้งานได้ทันที

---

## 💬 สไตล์การตอบ

- **กระชับ** — ไม่ verbose ไม่ขยายความโดยไม่จำเป็น
- ใช้ bullet/table แทนย่อหน้ายาว
- Code block ต้องมี language syntax highlight เสมอ
- เมื่อเจอ error — ระบุสาเหตุและวิธีแก้ทันที ไม่ต้องอธิบายพื้นหลังยาว
- **ห้ามถามซ้ำ** ในสิ่งที่ตอบไปแล้วในบทสนทนาเดียวกัน
