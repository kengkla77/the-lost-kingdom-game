# 🏰 The Lost Kingdom - Interactive Visual Novel

> เกมแนว "Choose Your Own Adventure" บนเว็บ ที่สร้างด้วย **HTML, HTMX และ Tailwind CSS** มอบประสบการณ์ระดับ Cinematic โดยไม่ต้องใช้ JavaScript Framework หนักๆ

![Game Screenshot](https://github.com/kengkla77/the-lost-kingdom-game/blob/main/index.png?raw=true)


## 🎮 ลองเล่น (Demo)
👉 **[กดที่นี่เพื่อเข้าสู่โลกแห่งจินตนาการ](https://kengkla77.github.io/the-lost-kingdom-game/)**

---

## ✨ เกี่ยวกับโปรเจค (About)
โปรเจคนี้สร้างขึ้นเพื่อทดสอบแนวคิด **"Modern Web without Complexity"** โดยการใช้เทคโนโลยีเว็บมาตรฐานเพื่อสร้างเกมที่มีการโต้ตอบสูง (Interactive) และสวยงาม:

* **Cinematic Experience:** การเปลี่ยนฉากที่นุ่มนวลเหมือนภาพยนตร์
* **No Page Reloads:** เล่นต่อเนื่องไม่มีสะดุดเหมือนแอปพลิเคชัน (SPA feel)
* **Mobile First:** ออกแบบมาให้เล่นบนมือถือได้อย่างสมบูรณ์แบบ

## 🛠️ Tech Stack (ใช้อะไรสร้างบ้าง?)
โปรเจคนี้พิสูจน์ว่า **"แค่ HTML ก็อลังการได้"** ด้วย Stack นี้:

* **[HTMX](https://htmx.org/):** พระเอกของงาน! ใช้จัดการ Logic การเปลี่ยนฉาก โหลด HTML Fragments มาแสดงผลโดยไม่ต้องเขียน Fetch API เอง
* **[Tailwind CSS](https://tailwindcss.com/):** จัดการความสวยงาม Layout และ Responsive Design (ผ่าน CDN)
* **[View Transitions API](https://developer.mozilla.org/en-US/docs/Web/API/View_Transitions_API):** ฟีเจอร์ใหม่ของ Browser ที่ทำให้การสลับหน้าจอมีการ Cross-fade แบบเนียนกริบ (Native Browser Animation)
* **HTML5:** โครงสร้างหลักที่เรียบง่าย

## 📂 โครงสร้างไฟล์ (File Structure)
เราใช้เทคนิค **Fragment-based** คือแยกฉากแต่ละฉากเป็นไฟล์ HTML ย่อยๆ

```text
my-visual-novel/
├── index.html           # 🎭 เวทีหลัก (Main Stage) และ Script ควบคุม Animation
├── README.md            # 📄 เอกสารอธิบายโปรเจค
└── scenes/              # 🎬 บทละครแต่ละฉาก (HTML Fragments)
    ├── start.html       # ฉากเริ่มต้น
    ├── forest.html      # ฉากป่า
    ├── castle.html      # ฉากปราสาท
    ├── ...              # ฉากย่อยและฉากจบต่างๆ
    └── end-xxx.html     # ฉากจบแต่ละแบบ
```
## 🚀 วิธีรันโปรเจคในเครื่อง (How to Run Locally)
เนื่องจากโปรเจคนี้ใช้ HTMX ในการดึงไฟล์ (AJAX) คุณไม่สามารถเปิดไฟล์ index.html ตรงๆ ได้ (Browser จะบล็อกเนื่องจาก CORS Policy)

Clone Repo:
```
git clone (https://github.com/kengkla77/the-lost-kingdom-game.git)
```
## เปิดด้วย Live Server (แนะนำ):
* ติดตั้ง Extension "Live Server" ใน VS Code
* คลิกขวาที่ไฟล์ index.html แล้วเลือก Open with Live Server

## 🏆 ฟีเจอร์เด่น (Key Features)
* Dynamic Content Loading: โหลดเฉพาะเนื้อหาใหม่ ไม่ต้องโหลดหน้าเว็บใหม่ทั้งหน้า

* Responsive Design: ปุ่มกดและตัวหนังสือปรับขนาดอัตโนมัติตามหน้าจอมือถือ/แท็บเล็ต/คอมพิวเตอร์

* Fallback Images: ระบบป้องกันรูปภาพแตก หากโหลดรูปไม่ได้จะมีพื้นหลัง Gradient สวยๆ ขึ้นมาแทนที่

* Immersive UI: ใช้ Font ตระกูล Serif (Cinzel, Lora) และ Dark Mode เพื่อสร้างบรรยากาศ

## 📜 License
โปรเจคนี้เป็น Open Source สามารถนำไปศึกษาหรือต่อยอดได้ตามสบาย! Images courtesy of Unsplash.

Created with ❤️ by kengkla
