# Auto Rally (Retro Auto-Rickshaw Racing Game)

A high-performance pseudo-3D HTML5 Canvas racing game engineered to run **100% offline in flight mode on phones, tablets, and laptops**. Features 3-lap racing, coin pickups, obstacle avoidance, cutting chai nitro boosts, persistent leaderboards, and synthesized retro sound effects.

---

## 🌟 Key Features

1. **Complete Flight-Mode Autonomy:**
   - Zero external assets or CDNs. Runs offline as an installable PWA (`manifest.json`, `sw.js`).
   - Pure canvas vector graphics and Web Audio API synthesized audio.

2. **60-FPS Perspective Canvas Track Engine:**
   - Dynamic curved looping track with animated road stripes, curbs, and sunset horizon.
   - Vector-rendered Indian auto-rickshaw sprite with steering tilt and exhaust particles.

3. **Dual Control Scheme:**
   - **Desktop:** Keyboard Arrows (<kbd>▲</kbd> <kbd>▼</kbd> <kbd>◀</kbd> <kbd>▶</kbd>) or <kbd>W</kbd><kbd>A</kbd><kbd>S</kbd><kbd>D</kbd>.
   - **Mobile:** On-screen thumb buttons (Steer ◀, Steer ▶, 🛑 Brake, ⚡ Gas).

4. **Game Items & Power-ups:**
   - 🪙 **Gold Coins:** +50 points and score counter.
   - ⚡ **Cutting Chai / Nitro Boost:** 4 seconds of super speed and engine roar.
   - 🚧 **Obstacles:** Road barriers and potholes with fair collision recovery.

5. **3-Lap Race & Persistent Leaderboard:**
   - Real-time HUD showing Coins (`🪙 24`), Current Lap (`Lap 2/3`), and Race Timer (`0:48`).
   - Personal best lap and race records survive device restarts via `localStorage`.

6. **Synthesized Retro Audio:**
   - Engine acceleration rumble, chimes, crash thumps, and fanfare generated in real time with audio oscillators.
   - One-click master mute toggle button.

---

## 📂 Project Structure

```
auto-rally/
├── index.html     # Game viewport and HUD markup
├── prompts.md     # Development prompt logs
├── README.md      # Game manual & verification
├── manifest.json  # PWA installation manifest
├── sw.js          # Service worker for offline cache
├── css/
│   └── style.css  # Arcade HUD and mobile touch styling
└── js/
    ├── audio.js   # Pure Web Audio API synthesized sound
    ├── game.js    # Canvas rendering, physics, and lap tracking
    └── app.js     # Input bindings and HUD loop
```

---

## 🚀 How to Play

Double-click `index.html` or open in any mobile or desktop browser:
```
index.html
```

---

*Authored by Soubhagya for Bharat Space Education Research Centre (BSERC) Internship — Week 2 Submission.*
