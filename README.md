# 🎮 Exercise 6 – Interactive Basketball Shooting Game with Physics

**Semester:** Spring 2025  
**Course:** Computer Graphics  
**Student Name:** May Bourshan  

---

## 🏀 Overview

This project expands Exercise 5 (HW05) into a complete 3D basketball shooting game.  
The system includes full player control, realistic physics, animations, scoring, multiple game modes, effects, and an interactive UI.

---

## ✅ How to Run

1. Clone or download the project files  
2. Open `index.html` in a modern browser  
3. *(If using local fonts or textures, run via a local server like Live Server in VS Code)*

---

## 🎮 Controls

- **Arrow keys** – Move on court  
- **W / S** – Adjust shot power  
- **Spacebar** – Shoot  
- **R** – Reset ball  
- **O** – Toggle Orbit camera  
- **1** – Top-down view  
- **2** – Behind scoreboard view  
- **3** – Classic angled view (default)  
- **4** – Sideline view  

You can switch between **Free Shoot** and **Timed Challenge** modes anytime using on-screen buttons – even during gameplay.

---

## 🎯 Implemented Features

### ✔️ Physics-Based Basketball Movement
- Real gravity (−9.8)  
- Parabolic trajectory based on velocity vector  
- Shot power affects speed  
- Bounces with gradual energy loss  
- Collision with walls and floor  
- Natural deceleration and stop  
- Precise collision detection with **rim and backboard**

### ✔️ Interactive Controls
- Smooth movement via arrow keys  
- Power bar adjustment  
- Shooting with spacebar  
- Auto-aim towards nearest hoop  
- Quick reset using “R”  
- Orbit camera toggle  

### ✔️ Rotation Animation
- Ball rotates in motion  
- Rotation axis based on movement vector  
- Spin speed depends on shot power  

### ✔️ Advanced Scoring System
- Real-time score updates  
- Success rate percentage  
- Tracks shots and hits  
- High Score saved in `localStorage`  
- Animated feedback messages:  
  - 🟡 “SWISH!” – perfect shot (no rim/backboard contact)  
  - 🟢 “SHOT MADE!” – regular make  
  - 🔴 “MISSED SHOT” – miss  

### ✔️ Combo System
- Streaks of successful shots earn bonuses:  
  - 2 hits → “COMBO x1! +1 Bonus”  
  - 3 hits → “COMBO x2! +2 Bonus”  
  - etc.  
- Resets on a miss  
- Shows animated combo bonus on screen  

### ✔️ SWISH + Fireworks 🎆
- Detects no-contact shots (swish)  
- Triggers fireworks from the rim + “SWISH!” message  

### ✔️ Timed Challenge Mode
- HUD shows timer or clock  
- **Free Shoot**: live clock  
- **Challenge**: 60-second countdown  
- Default mode: Free Shoot  
- Mode switch resets stats  
- High Score remains saved  
- Goal: 50 points in 60 seconds  
- On success: 🎉 message + alert with:  
  🏆 Challenge Completed  
  Final Score, Attempts, Hits, Accuracy  
- On timeout: ⏱ Time’s Up! + same alert  

---

## 🎨 Graphics & Sounds

- 5-layer colorful ball trail  
- Fireworks effect on perfect swishes  
- Three distinct sound effects:  
  - ✅ Ball collision (rim, ground, or backboard)  
  - ✅ Success cheer  
  - ✅ Missed shot “boo”

---

## 📸 Screenshots / Video

Below are visual highlights of the game:

🖼️ ![Game UI Overview](shttps://www.youtube.com/watch?v=vS3HTB0j_Hw&feature=youtu.be)

🎬 **[Watch Swish Shot (MP4)](https://www.youtube.com/watch?v=vE5b3hfhDQI&feature=youtu.be)**  
A short clip demonstrating a perfect "Swish" shot with no rim contact, combo bonus, fireworks animation, and score update.

🎬 **[Watch Full Gameplay (MP4)](https://www.youtube.com/watch?v=vS3HTB0j_Hw&feature=youtu.be)**   
A full 60-second recording demonstrating the main gameplay features:
- 🏀 Basketball being moved around the court using arrow keys  
- 🎯 Shot power adjustment using W/S keys  
- 🔄 Shooting mechanics with spacebar  
- ✅ Successful shot with real-time score update  
- 🌀 Ball rotation animation during movement and flight  
- 📊 Full UI: score, combo, statistics, timer, and controls  
- ⏱️ Switching to Timed Challenge mode and breaking the **local high score**  
- 🎉 Combo streak 
- 🔁 Missed shots and automatic reset of combo  


## ⚠️ Known Issues

- In rare edge cases, minor misalignment in rim collisions may occur  
  *(Resolved using multiple invisible cylinders to simulate the rim)*

---

## 📁 External Assets

- `basketball.png` – Ball texture  
- `wood_floor.jpg` – Court texture  
- `cheer.wav` – Success sound  
- `boo.wav` – Miss sound  
- `basketball.wav` – Impact sound  
- `Droid Serif` – UI font  
- `Helvetiker` – Font for 3D text (TextGeometry)


---

## 📝 Notes  
All logic, animations, and visual effects were custom-built using raw Three.js – with no external game engines.  
Key systems such as the scoreboard, ball physics, combo handling, fireworks, and dynamic UI were developed entirely from scratch.
