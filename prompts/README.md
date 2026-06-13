# 🎨 คลังรวม Prompt ออกแบบเชิงพาณิชย์และกราฟิก (June 13, 2026)

รวบรวมเทมเพลตและตัวอย่างพฤติกรรมการเขียน Prompt สำหรับสร้างรูปภาพโฆษณาสินค้า, แสตนดี้ร้านอาหาร, โปสเตอร์ภาพยนตร์ และโลโก้ตัวอักษรภาษาไทย ที่ได้เรียนรู้และพัฒนาปรับปรุงในวันนี้

---

## 1. 🛒 ป้ายโปรโมชันแฟลชเซลล์ E-commerce (Flash Sale Badge Ads)
เน้นการโชว์ตัวผลิตภัณฑ์คู่กับป้ายราคาโปรโมชันที่มีคอนทราสต์สูง สไตล์แบนเนอร์ TikTok / Shopee

### เทมเพลตตัวแปรหลัก
*   **PRODUCT_CATEGORY**: ประเภทของสินค้า
*   **HERO_PRODUCT_DETAILS**: รายละเอียดของแพ็กเกจจิ้ง แสงเงาสตูดิโอ และส่วนประกอบตกแต่งรอบๆ
*   **MAIN_CLAIM_TEXT**: ข้อความโปรโมตหลัก
*   **PRICE_DETAILS**: รายละเอียดราคา (ราคาโปรโมชัน จากราคาปกติ)
*   **BADGE_COLOR_THEME**: โทนสีและเอฟเฟกต์ของป้ายราคา
*   **BADGE_SHAPE_STYLE**: รูปทรงของป้ายราคา
*   **PROMOTION_TAG**: แท็กหัวข้อย่อยโปรโมชันด้านบนสุด

### ตัวอย่างที่ 1: หม้อสแตนเลสสองหูพร้อมชั้นนึ่ง (อ้างอิงจากไฟล์ `IMG_3434.JPG`)
```text
- PRODUCT_CATEGORY: หม้อสแตนเลสสองหูพร้อมชั้นนึ่ง
- HERO_PRODUCT_DETAILS: Brushed stainless steel double-handle cooking pot with a stackable steamer tier. The pot features dual curved black bakelite side handles. The top is covered with a clear brownish-tinted tempered glass lid with a polished stainless steel rim and a shiny steel knob. Professional studio lighting highlighting clean metallic reflections and brushed metal texture details. A dramatic, elegant swirl of white hot cooking steam rising from behind. At the base, fresh whole food ingredients like garlic, red chili, lemongrass, and green herbs are arranged artfully.
- MAIN_CLAIM_TEXT: หม้อสุกี้อเนกประสงค์ ร้อนไว ทนทาน นึ่งต้มครบในใบเดียว
- PRICE_DETAILS: 399.- จากราคาปกติ 790.-
- BADGE_COLOR_THEME: Saturated fiery red and metallic gold panels with glowing bright white 3D neon inner gradients.
- BADGE_SHAPE_STYLE: Modern Rounded Shield (ป้ายรูปทรงโล่โค้งมนซ้อนทับกันเป็นเลเยอร์ดูทันสมัยและน่าเชื่อถือ)
- PROMOTION_TAG: แข็งแรงทนทาน การันตีคุณภาพ!
- BACKGROUND_COLOR: Solid black
```

### ตัวอย่างที่ 2: โกโก้ปั่นเข้มข้นภูเขาไฟ (อ้างอิงจากไฟล์ `โกโก้ปั่นเข้มข้น (Cocoa Smoothie) .jpeg`)
```text
- PRODUCT_CATEGORY: โกโก้ปั่นเข้มข้นวิปครีมภูเขาไฟ
- HERO_PRODUCT_DETAILS: Rich dark cocoa smoothie in a tall faceted glass covered in cold condensation droplets, crowned with a perfect swirl of whipped cream dusted with dark cocoa powder. The glass sits in a dynamic glossy chocolate syrup splash. Floating around are chocolate chunks, whole cocoa beans, and ice cubes. Solid clean white background. High-end food styling lighting.
- MAIN_CLAIM_TEXT: โกโก้ปั่นเข้มข้น ดับร้อน เคี้ยวเพลิน หวานมันสะใจ
- PRICE_DETAILS: 59.- จากราคาปกติ 89.-
- BADGE_COLOR_THEME: Warm chocolate brown and golden yellow panels with glowing yellow 3D neon inner gradients.
- BADGE_SHAPE_STYLE: Rounded Hexagon (ป้ายทรงหกเหลี่ยมโค้งมนดูนำสายตา)
- PROMOTION_TAG: เมนูขายดีอันดับ 1!
- BACKGROUND_COLOR: Solid white
```

---

## 2. 🍲 แสตนดี้ตั้งโต๊ะ / ตั้งพื้นโปรโมตเมนูอาหาร (Catering Display Stand)
ออกแบบขึ้นรูปแสตนดี้โชว์เมนูอาหารบนพื้นหลังสีขาวสะอาดยื่นออกมาเห็นฐานชัดเจน เพื่อความสะดวกในการตัดต่อใช้งานจริง

### ตัวอย่างที่ 1: ชุดหม้อไฟต้มยำทะเลเดือด (แนวปะทุร้อนแรงภูเขาไฟ)
```text
BRAND_NAME: หม้อเดือดภูเขาไฟ
MAIN_TITLE: ชุดหม้อไฟเดือดจัด
SUBTITLE: ซุปเข้มข้น เครื่องแน่นเต็มหม้อ
SUPPORTING_PHRASES: น้ำซุปเข้ม | เนื้อแน่น | ผักสด
FOOD_CATEGORY: Hotpot promotion set
THEME_DIRECTION: hot and bold volcano hotpot style
COLOR_PALETTE: lava red, soup orange, dark charcoal, fresh green, warm white
FEATURED_PRODUCT: หม้อไฟต้มยำทะเลเดือด
SUPPORTING_PRODUCTS: กุ้งแม่น้ำ, หมึกสด, ลูกชิ้นปลา, เห็ดรวม, ผักสด
ADD_ONS: น้ำจิ้มซีฟู้ด, เส้นแก้ว, ไข่ไก่
SELLING_POINTS: ซุปหอมจัด, ซีฟู้ดสด, เครื่องแน่น, กินได้หลายคน, คุ้มทุกหม้อ
PROMOTION_INFO: เซ็ตหม้อไฟ 299 บาท
DISPLAY_MATERIAL: floor-standing KT board display stand
LANGUAGE_MODE: THAI
```

### ตัวอย่างที่ 2: โกโก้ปั่นวิปครีมภูเขาไฟ (ป้ายตั้งโต๊ะคาเฟ่)
```text
BRAND_NAME: โกโก้ภูเขาไฟ (Volcano Cocoa)
MAIN_TITLE: โกโก้ปั่นภูเขาไฟเข้มข้น
SUBTITLE: เข้มข้นสะใจ วิปครีมล้นแก้ว โรยผงโกโก้เน้นๆ
SUPPORTING_PHRASES: โกโก้นำเข้าแท้ | วิปครีมนุ่มละมุน | เย็นชื่นใจดับร้อน
FOOD_CATEGORY: Cocoa smoothie drink promotion
THEME_DIRECTION: rich and bold chocolate volcano style with icy splash
COLOR_PALETTE: chocolate brown, cream white, ice blue, golden brown, dark charcoal
FEATURED_PRODUCT: โกโก้ปั่นภูเขาไฟวิปครีมล้น (Volcano Cocoa Smoothie)
SUPPORTING_PRODUCTS: ช็อกโกแลตชิ้นพรีเมียม (Premium chocolate chunks), เมล็ดโกโก้คั่ว (Roasted cocoa beans), น้ำแข็งใสสะอาด (Pure ice cubes)
ADD_ONS: ซอสช็อกโกแลตเข้มข้น (Rich chocolate syrup splash), ผงโกโก้โรยหน้า (Extra cocoa powder)
SELLING_POINTS: โกโก้เกรดพรีเมียม, หวานมันกลมกล่อม, วิปครีมแท้, ปั่นเนื้อละเอียด, อร่อยเต็มแก้ว
PROMOTION_INFO: พิเศษเพียง 59 บาท จากปกติ 89.-
DISPLAY_MATERIAL: tabletop mini KT board display card
LANGUAGE_MODE: THAI
```

---

## 🎬 3. โปสเตอร์ภาพยนตร์คอมเมดี้สไตล์ไทย (Thai Action-Comedy Movie Poster)
การใช้คู่สีจัดจ้าน (High Contrast) และมุมกล้องกว้าง-ต่ำ (Wide and Low angle) พร้อมวัตถุปลิวลอยเพิ่มมิติความตลกโกลาหล

### ตัวอย่างหลัก: พุ่มพวง สู้ฟัด (รถพุ่มพวงขายกับข้าวซิ่งระเบิด)
```text
POSTER_TITLE: พุ่มพวง สู้ฟัด
MAIN_VEHICLE: รถกระบะพุ่มพวงที่มีถุงผักและของสดห้อยเต็มรถ
MAIN_CHARACTERS: ลุงคนขับใจดีแต่ใส่แว่นดำเท่ๆ กับคุณยายที่ถือตะหลิวเตรียมสู้
LOCATION: ถนนลูกรังในชนบทที่มีฝุ่นตลบ
CHAOTIC_ELEMENTS: ลูกมะนาวบิน, ปลาร้าขวด, พริกแห้งกระจาย, ไก่บ้านที่บินหนี
COLOR_MOOD: Earthy Tones with Popping Green and Red
```

---

## 🪐 4. โปสเตอร์ซูเปอร์ฮีโร่แนวรวมดารานักแสดง (Cosmic Superhero Ensemble Poster)
การคอลลาจหน้าตัวละครซ้อนทับกันเป็นมิติ โดยใช้คู่สีแนวอวกาศ (Electric Purple, Neon Blue, Magenta) และเอฟเฟกต์ลำแสงพลังงาน

### พรอมต์หลักในการเจน (Direct Prompt)
```text
An epic cinematic movie poster featuring a collage of powerful superheroes in a dynamic layered montage. At the top center, a legendary hero in high-tech armor looks off-camera with a determined expression. In the background shadow, a giant armored villain looms. Surrounding them are other diverse heroes: a warrior god with a beard, a female cosmic captain, a female spy in black suit, a super soldier at the bottom center. The scene is illuminated by dramatic electric purple, neon blue, and hot magenta cosmic light beams and glowing energy streaks. Starry space galaxy background with nebulas. High-end theatrical release poster aesthetic, detailed faces, realistic cinematic lighting, volumetric lights, 8k resolution.
```

---

## 🏷️ 5. โลโก้ตัวอักษรภาษาไทยเชิงแนวคิด (Conceptual Thai Typographic Logo)
บังคับให้ตัวอักษรภาษาไทยแสดงออกในรูปแบบรูปภาพเวกเตอร์ 2 มิติที่ขยับหรือไหลลื่นตามแนวคิดของแบรนด์ (2D Flat Vector)

### ตัวอย่างที่ 1: คาเฟ่ลับในตรอกซอกซอย ("ซอยไหน")
```text
BRAND_NAME_TH: "ซอยไหน"
TAGLINE_TH: "คาเฟ่ลับ ที่คุณต้องค้นหา"
CONCEPT_SHAPE: A minimalist street sign or a narrow alleyway perspective.
FONT_BEHAVIOR: The Thai letters "ซ-อ-ย-ไ-ห-น" should use forced perspective, looking like they are receding into a distance along a street.
COLOR_PALETTE: Asphalt Grey, Neon Yellow, and White.
```

### ตัวอย่างที่ 2: ร้านผัดกะเพรารสเผ็ดร้อน ("กะเพราเอาอีกแล้ว")
```text
BRAND_NAME_TH: "กะเพราเอาอีกแล้ว"
TAGLINE_TH: "รสจัดจ้าน เผ็ดร้อน หอมกลิ่นกระทะ"
CONCEPT_SHAPE: A stylized minimalist hot iron wok with a dynamic fire flare or a single holy basil leaf.
FONT_BEHAVIOR: The Thai characters "ก-ะ-เ-พ-ร-า-เ-อ-า-อี-ก-แ-ล้-ว" should use organic, lively strokes where the top terminals and vowels curve upward slightly to mimic rising steam or hot flames from a stir-fry wok.
COLOR_PALETTE: Chili Red, Basil Green, Matte Charcoal, and Warm White.
```
