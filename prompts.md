# Engineering Journey & Prompt History: Auto Rally

This document records the sequence of prompts, architectural design decisions, and testing iterations followed to build the **Autonomous Offline Auto Rally Racing Game** for the BSERC Internship (Week 2, Project 8).

---

## Prompt 1: Perspective Canvas Engine & Vector Rickshaw
> **Prompt:**  
> "I need to build a retro pseudo-3D auto-rickshaw racing game on an HTML5 canvas that friends can pass around and play on their phones on a train with zero network.  
> Requirements:
> 1. Driveable auto-rickshaw on a looping perspective road.
> 2. Dual controls: desktop keyboard (arrows/WASD) and mobile touch overlay.
> 3. Collectible coins, obstacles (potholes, barriers), and nitro chai boost.
> 4. 3-lap race with precision timer and lap counter.
> 5. Best lap and race time saved persistently in LocalStorage.
> 6. Synthesized retro sound effects using Web Audio API with a master mute button."

**Outcome:**  
Implemented `js/game.js` with perspective road rasterization, vector auto-rickshaw rendering, and entity management.

---

## Prompt 2: Synthesized Web Audio Engine
> **Prompt:**  
> "Implement `js/audio.js` with mathematical Web Audio API oscillators for engine rumble, coin pickup, nitro boost, crash bump, and victory fanfare. Zero external MP3 files so it works 100% offline in flight mode."

**Outcome:**  
Engineered `SoundEngine` with pitch-shifting engine audio, frequency ramped sound effects, and mute toggle.

---

## Prompt 3: Touch Overlay & Fair Collision Mechanics
> **Prompt:**  
> "Implement mobile touch clusters (Left, Right, Gas, Brake) with `touch-action: none`. Ensure collision boxes feel fair: obstacles slow the vehicle rather than instantly killing the run, and provide 1.2s invulnerability after collision."

**Outcome:**  
Built intuitive mobile touch controls and fair physics collision windows.
