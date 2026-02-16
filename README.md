# 🌗 Hidden Trigger – Theme Switching Game

## 🎮 Project Overview

This project is a creative JavaScript assignment where **theme switching is not just a visual feature — it becomes the core gameplay mechanic.**

The application starts with `button.html`, where the user must toggle a theme switch 20 times.  
After completing the required toggles, a transition animation runs and the main game (`game.html`) launches automatically.

Inside the game, switching between Light and Dark themes dynamically changes the world, unlocking new paths and hiding others.

---

## 📁 Project Structure

js-grp-assignment/<br>
│<br>
├── button.html → Entry file (must be executed first)<br>
├── game.html → Canvas-based platformer game<br>
├── music.mp3 → Background music<br>
└── README.md


---

# 🚀 How To Run

1. Open `button.html` in your browser.
2. Toggle the switch 20 times.
3. A fade animation will run.
4. The game (`game.html`) will start automatically.

⚠️ Make sure all files are in the same folder.

---

# 🌗 Phase 1 – Entry System (`button.html`)

The project begins with a custom animated theme toggle switch.

### What Happens:

- Each toggle switches between light and dark mode.
- A counter decreases from 20.
- After 20 toggles:
  - A fade animation plays.
  - The page redirects to `game.html`.

### JavaScript Concepts Used:

- `getElementById()` for DOM selection  
- `classList.toggle()` for theme switching  
- Event listener (`change`)  
- Countdown logic  
- `setTimeout()` for delayed redirection  
- Dynamic text updates  

This file acts as a **hidden trigger gate** before entering the main game.

---

# 🎮 Phase 2 – The Game (`game.html`)

The main game is built entirely using:

- HTML5 `<canvas>`
- Vanilla JavaScript
- Custom physics logic
- Real-time rendering with `requestAnimationFrame()`

---

# 🧠 Core Concept: Theme as Gameplay

In this game:

- The player can move left and right.
- The player can jump.
- Every time the player jumps:
  - The theme switches between Light and Dark.
  - Platform visibility changes.
  - Some platforms appear.
  - Some platforms disappear.

This creates a puzzle-platform mechanic where switching themes is necessary to progress.

Theme switching is integrated directly into the game physics and collision logic.

---

# ⚙️ Technical Implementation

## 1️⃣ Game Loop

Uses:

```js
requestAnimationFrame()
To continuously:

Update physics

Check collisions

Render the scene

2️⃣ Physics System
Custom-built physics including:

Gravity

Jump velocity

Horizontal movement

Platform collision detection

Boundary restriction

Death condition

3️⃣ Theme Objects
Two theme configurations are defined:

const L = { ... }  // Light theme
const D = { ... }  // Dark theme
Switching themes changes:

Background gradient

Platform colors

Ghost platform appearance

Player colors

Door design

UI text colors

4️⃣ Conditional Platforms
Platforms are categorized as:

Always visible

Visible only in Light mode

Visible only in Dark mode

The game checks the current theme before allowing collisions.

This is what makes theme switching part of the level design.

✨ Additional Features
Moving platforms (sinusoidal motion)

Breakable platforms

Particle effects on jump and death

Timer display

Best time tracking (session-based)

Restart system (R key)

Win screen overlay

Death animation overlay

Background music with autoplay fallback

🎮 Controls
← →  : Move
Space / ↑ : Jump (Switch Theme)
R : Restart
🏆 Objective
Reach the glowing door at the top platform.

When completed:

Timer stops

"YOU WIN!" screen appears

Best time is recorded for the session

🎯 Learning Outcomes
Through this assignment, I learned:

DOM manipulation and event handling

Managing UI state with JavaScript

Canvas-based rendering

Game loop architecture

Collision detection logic

Physics simulation basics

Using theme switching as a dynamic system instead of a visual-only feature

💡 Key Highlight
Unlike a basic light/dark toggle project, this implementation:

Uses theme switching as a gameplay mechanic

Integrates theme state with physics and collision logic

Combines DOM-based UI with Canvas-based game systems

Demonstrates advanced JavaScript logic beyond simple UI toggling

👨‍💻 Developer
Abdeali Makda
