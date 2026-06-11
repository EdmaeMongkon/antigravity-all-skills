# Antigravity Skills Backup (`antigravity-all-skills`)

คลังเก็บข้อมูลระบบความรู้ (Skills Backup) และการตั้งค่าของ Antigravity CLI สำหรับการย้ายไปใช้งานในเครื่องใหม่

## 📂 รายละเอียดไฟล์ใน Repository
- **`skills/`**: โฟลเดอร์ที่รวบรวม Skills ทั้งหมด 88 รายการ (ขนาดประมาณ 5.6MB)
  - **AEC / BIM Stack**: Blender Core API, Bonsai (BlenderBIM), IfcOpenShell, Sverchok, Clash Detection, QTO (Quantity Takeoff), 2D Drawings, MEP, Materials, etc.
  - **Web & Animation**: HyperFrames (CLI, Media, Registry), Anime.js, GSAP, CSS Animations, Lottie, Tailwind CSS, Three.js, WebGL, TypeGPU, WAAPI (Web Animations API)
- **`skills-lock.json`**: ไฟล์ระบุแหล่งที่มาและ Hash ของแต่ละ Skill ที่ดาวน์โหลดมาจากภายนอก
- **`.mcp.json`**: ไฟล์การตั้งค่า Model Context Protocol (MCP) สำหรับเชื่อมต่อเครื่องมือภายนอก (เช่น Blender MCP Server)

---

## 🚀 วิธีนำไปใช้งานในเครื่องคอมพิวเตอร์เครื่องใหม่ (Restore Guide)

ทำตามขั้นตอนด้านล่างนี้เพื่อนำข้อมูลความรู้ทั้งหมดไปติดตั้งและใช้งานบนเครื่องใหม่:

### ขั้นตอนที่ 1: เตรียมสภาพแวดล้อมระบบ (Prerequisites)
ติดตั้งเครื่องมือพื้นฐานที่จำเป็นบนเครื่องใหม่:
1. **Node.js** (เวอร์ชัน 18 ขึ้นไป): [ดาวน์โหลดที่นี่](https://nodejs.org/)
2. **Git**: ติดตั้งผ่าน Xcode Command Line Tools (macOS) หรือดาวน์โหลดตัวติดตั้งสำหรับ OS ของคุณ
3. **uv (Python package manager)**:
   * **macOS / Linux**: `curl -LsSf https://astral.sh/uv/install.sh | sh`
   * **Windows**: `powershell -c "irm https://astral.sh/uv/install.ps1 | iex"`

---

### ขั้นตอนที่ 2: ติดตั้ง Antigravity CLI
เปิด Terminal บนเครื่องใหม่แล้วติดตั้ง CLI ของ Antigravity (หรือติดตั้งระบบ Agent ของคุณ)

---

### ขั้นตอนที่ 3: ดึงข้อมูลความรู้ (Clone Repository)
ดาวน์โหลดโฟลเดอร์นี้ลงเครื่องใหม่ผ่านคำสั่ง Git:
```bash
git clone https://github.com/EdmaeMongkon/antigravity-all-skills.git
```

---

### ขั้นตอนที่ 4: คัดลอก Skills ไปยังโฟลเดอร์ระบบของเครื่องใหม่

ในระบบ macOS/Linux ปกติ Antigravity จะค้นหา Skills ในโฟลเดอร์ `~/.agents/skills/`

ให้ทำการสร้างโฟลเดอร์ปลายทางแล้วคัดลอกไฟล์ความรู้ทั้งหมดไปวาง:

```bash
# 1. สร้างโฟลเดอร์ปลายทางบนเครื่องใหม่ (หากยังไม่มี)
mkdir -p ~/.agents/skills

# 2. คัดลอก Skills ทั้งหมดเข้าไปในระบบ
cp -r antigravity-all-skills/skills/* ~/.agents/skills/

# 3. คัดลอกไฟล์ lock และตั้งค่าไปไว้ในโฟลเดอร์ผู้ใช้
cp antigravity-all-skills/skills-lock.json ~/
cp antigravity-all-skills/.mcp.json ~/
```

---

## 🛠️ รายการ Skills ทั้งหมดในคลังนี้ (88 ตัว)
ความรู้และกฎการเขียนโค้ดที่ระบบ Agent ของคุณสามารถเรียกใช้ได้ทันที ได้แก่:
1. **AEC / BIM Workflow Orchestrator**
2. **Blender Scripting & Addon Development** (Core, GPU, Runtime, Materials, Mesh, Modifiers, Nodes, Operators, Panels, Properties, Rendering)
3. **Bonsai BIM Authoring** (Project, Drawing, Modeling, QTO, Clash, BCF, Spatial Hierarchy, Classifications)
4. **IfcOpenShell (IFC Python SDK)** (Creation, Geometry, Materials, MEP, Profiles, Relationships, Sequence/4D, Validation)
5. **Sverchok (Visual Programming)** (Parametric Design, Topologic, Custom Nodes, SNLite Scripting, Sockets, Data Nesting)
6. **HyperFrames & Video Assets** (Remotion transition, TTS Voiceover, Audio Beat Sync, Whispers/Captions)
7. **Animation Libraries** (GSAP, Anime.js, Lottie, WAAPI, Three.js, TypeGPU)
