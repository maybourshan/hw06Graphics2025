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
🏆 Challenge Completed!
Final Score: X
Shots: Y
Hits: Z
Accuracy: P%

markdown
Copy
Edit
- On timeout before 50 pts: “⏱ Time’s Up!” + same stats alert  
- Start/stop button for Challenge  

✔️ **Rich UI**  
- Power bar  
- Game mode menu (Free Shoot / Challenge)  
- Combo popup animations  
- On-screen display of:
- Shots
- Makes
- Accuracy %
- Current Score & High Score
- Timer / Clock
- Animated messages  
- Real-time stats  

✔️ **Graphics & Sound Effects**  
- 5-layer colored ball trail  
- Firework effects on perfect makes  
- Three sound types:
- ✅ Ball hit rim/ground
- ✅ Success cheer
- ✅ Failure boo  

## Advanced Features

Based on the current implementation, the following optional bonus features are fully supported:

- 🎯 **Multiple Hoops**  
  Both left and right rims are present, with each shot automatically targeting the nearest hoop.

- 🟡 **Swish Detection**  
  Perfect “swish” shots (no contact with rim or backboard) trigger a “SWISH!” notification and fireworks effect.

- 🔥 **Combo System**  
  Consecutive made shots increase a combo counter, awarding extra bonus points and displaying a dynamic combo message.

- ⏱️ **Time Challenge**  
  A 60-second timed mode with countdown display, win/lose alerts, and automatic reset at round end.

- 🔊 **Sound Effects**  
  Three distinct audio cues for makes (`cheer.wav`), misses (`boo.wav`), and ball impacts (`basketball.wav`).

- ✨ **Ball Trail Effect**  
  A fading, five-layer trail follows the ball’s flight path, adding visual flair to each shot.

- 🌬️ **Advanced Physics**  
  Realistic gravity, energy loss on bounces, precise rim/backboard collisions, and motion damping ensure authentic behavior.

- 🎮 **Game Modes**  
  Toggle between Free Shoot (live clock) and Timed Challenge modes via on-screen buttons.

- 🏆 **Leaderboard**  
  High score tracking using `localStorage`, with the top score displayed on the HUD.

🚀 **External Assets**  
- `basketball.png` – Ball texture  
- `wood_floor.jpg` – Court floor  
- `cheer.wav` – Success sound  
- `boo.wav` – Failure sound  
- `basketball.wav` – Impact sound  
- `Droid Serif` – Font for timer & text  


✨ **Summary**

This project meets all HW06 requirements and extends them significantly. The combination of graphics, physics, controls, design, and challenge makes for a complete and engaging game experience.

