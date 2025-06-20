🎮 Exercise 6 – Interactive Basketball Shooting Game with Physics

**Semester:** Spring 2025  
**Course:** Computer Graphics  
**Student Name:** May Bourshan

🏀 **General Description**

This project extends Exercise 5 (HW05) to create a full basketball shooting game on a 3D court. The system includes full controls, realistic physics, animations, scoring, different game modes, effects, and an interactive UI.

✅ **How to Run**

1. Open `index.html` in a modern browser.  
2. If you use local fonts or textures, run a local server (e.g., Live Server in VS Code).

**Controls:**
- **Arrow keys** – Move on court  
- **W / S** – Adjust shot power  
- **Spacebar** – Shoot  
- **R** – Reset ball  
- **O** – Toggle Orbit camera  
- **1** – Top-down view  
- **2** – Behind scoreboard view  
- **3** – Classic angled view (default)  
- **4** – Sideline view  

🎯 **Implemented Features**

✔️ **Physics-Based Basketball Movement**  
- Real gravity (−9.8)  
- Parabolic trajectory using velocity vector  
- Shot power affects horizontal & vertical speed  
- Bounces off ground with gradual energy loss  
- Collision with court walls/edges  
- Backboard collision with impact sound  
- Deceleration on bounce  
- Stop movement when velocity is near zero  
- Precise rim collision detection  

✔️ **Interactive Controls**  
- Smooth motion with arrow keys  
- Power bar adjustment  
- Spacebar shoot  
- Auto-aim toward nearest hoop  
- Quick reset with “R”  
- Orbit toggle  

✔️ **Rotation Animation**  
- Ball rotates along flight path  
- Rotation axis computed from movement vector  
- Spin speed proportional to shot power  

✔️ **Advanced Scoring System**  
- Immediate score updates  
- Success percentage meter  
- Track shots & makes  
- High Score in `localStorage`  
- Colorful animated messages:  
  - 🟡 “SWISH!” – perfect no-contact shot  
  - 🟢 “SHOT MADE!” – normal make  
  - 🔴 “MISSED SHOT” – miss  

✔️ **Combo System**  
- Consecutive makes earn bonus:  
  1st = 2 pts, 2nd = 3 pts, 3rd = 4 pts, …  
- Combo resets on miss  
- Visual “COMBO x2! +1 Bonus” mid-screen  

✔️ **SWISH + Fireworks 🎆**  
- Detect no-contact shot  
- Display “SWISH!” + fireworks from rim  

✔️ **Timed Challenge Mode**  
- Scoreboard shows clock or timer  
- **Free Shoot**: current time  
- **Challenge**: 60 s countdown  
- Default: Free Shoot  
- Mode switch resets all stats (score, shots, combo)  
- High Score preserved across sessions  
- Goal: reach 50 pts in 60 s  
- On success: animated “🎉 You won the challenge!” + `alert` with:
