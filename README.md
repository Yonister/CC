# ⚔️ Card Tower

เกม Roguelike Deck-Builder บนเว็บ เล่นได้ทั้งมือถือและคอม

## 🎮 เล่นเกม

เล่นออนไลน์ได้ที่: `https://<your-username>.github.io/<repo-name>/`
(ลิงก์จะอัปเดตหลัง deploy ผ่าน GitHub Pages)

## ✨ Features

- 4 Class: Warrior, Mage, Rogue, Paladin — แต่ละอาชีพมีการ์ดและ Skill Tree เฉพาะตัว
- Skill Tree ปรับระดับได้ Lv1-5 ต่อ skill
- ระบบ Fusion ผสมการ์ด 2 ใบเป็นใบใหม่ที่แรงขึ้น (ทำได้ที่จุดพัก)
- ระบบธาตุ (Fire/Ice/Lightning/Physical) มีจุดอ่อนของศัตรู
- Boss พร้อม Phase 2 และ Ability เฉพาะตัว
- Online Leaderboard (ผ่าน Firebase) — แข่งกันว่าใครไปได้ไกลที่สุด

## 🛠️ Setup สำหรับ Online Leaderboard

ไฟล์นี้มี Firebase integration พร้อมใช้ แต่ต้องตั้งค่า config ก่อน:

1. สร้าง Firebase project ฟรีที่ https://console.firebase.google.com
2. เปิด Firestore Database (เลือก "Start in test mode")
3. ไปที่ Project Settings > Your apps > Web เพื่อสร้าง config
4. แก้ไฟล์ `index.html` หาตัวแปร `FIREBASE_CONFIG` แทนที่ `null` ด้วย config ที่ได้
5. Commit + push ขึ้น GitHub อีกครั้ง

ถ้าไม่ตั้งค่า Firebase เกมยังเล่นได้ปกติ แต่ Leaderboard จะเก็บแค่ในเครื่อง (localStorage) ไม่ sync กับคนอื่น

## 📱 วิธีเล่น

เปิดลิงก์ผ่านเบราว์เซอร์มือถือหรือคอมพิวเตอร์ได้เลย ไม่ต้องติดตั้งอะไร
