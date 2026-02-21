# 📚🤜💥🏛️ The Luchabrarian Version 15.0

> *A top-down action game where you are a librarian, the library is haunted, and Book Genres are your only weapon. Built entirely with HTML, CSS, and JavaScript — no engines, no libraries (the code kind) *

---

## 🏛️ What Is This Game?

Imagine your library has a ghost problem. Not a *FRIENDLY* ghost problem. A *swarming, teleporting, exploding, shape-shifting* ghost problem. Your job? Keep shelving books anyway. 😝📖👻

You're the **LUCHABRARIAN** ➡️ part librarian, part luchador, 100% done with these ghosts. Dash around the library floor, scoop up scattered books, deliver them to the correct shelves, and survive long enough to file everything before chaos wins.

It's Pac-Man meets library science... With lore. And a trash can specifically for *BANANA PEELS*. 🍌🗑️ (CUE **HOLLABACK GIRL** by Gwen Stefani... iykyk 💅🔉🎶📢 )

---

## ✨ Features

- 🗺️ **Top-down action gameplay** — free movement across a full library floor
- 📚 **12 book categories** — Romance, Science, Horror, Sci-Fi, Manga, Forbidden, Mystery, Fantasy, History, Music, Art, Tablets, and... the Trash can (we are at a library of course!)
- 👻 **10 unique ghost types** — each with its own terrifying personality (see below)
- ⚡ **7 power-ups** — from Speed Boosts to Time Freeze to Auto-Sort
- 🎯 **4 difficulty modes** — Easy, Medium, Hard, and Endless (for people who hate themselves a little)
- 🥊 **3 combat moves** — Dash/Parry, Throw Book, and a 3-book Charge Attack
- 🏆 **Achievement system** — slide-in notifications for milestones
- 🗺️ **Mini-map** — because the library is big and the ghosts are fast
- 📱 **Fully responsive** — scales to any screen size (I think 😅)

---

## 🕹️ Controls

| Action | Key |
|---|---|
| Move | Arrow Keys |
| Dash / Parry | `Space` |
| Throw Book | `Enter` |
| Charge Attack (needs 3 books) | `Space Bar` |
| Toggle Mini-Map | `M` |
| Pause | `Esc` |

> 💡 **Pro tip:** A perfectly timed Dash *parries* ghost attacks. The Luchabrarian didn't go to library school to get hurt.

---

## 👻 Ghost Roster

These aren't your friendly neighborhood ghosts. Each one has a different strategy for making your shift miserable:

| Ghost | Behavior | Threat Level |
|---|---|---|
| 👻 Normal | Chases you. Classic. | ⭐ |
| 💨 Fast | Chases you, but faster. Great. | ⭐⭐ |
| 🪨 Tank | Slow but takes 2 hits to banish | ⭐⭐ |
| ✨ Teleporter | Blinks around the room. Rude. | ⭐⭐⭐ |
| 💥 Bomber | Rushes in and explodes. Dramatic. | ⭐⭐⭐ |
| 🔮 Ranged | Keeps its distance and shoots projectiles | ⭐⭐⭐ |
| 🪲 Swarm | Dies and splits into 3 mini-ghosts | ⭐⭐⭐ |
| 📕 Mimic | Disguises itself as a book on the floor. EVIL. | ⭐⭐⭐⭐ |
| 🔮 Possessor | Takes over a shelf and corrupts it | ⭐⭐⭐⭐ |
| 👑 Boss | Slow, giant, takes 3 hits, deeply unpleasant | ⭐⭐⭐⭐⭐ |

---

## ⚡ Power-Up Guide

Glowing pickups appear throughout the library. Grab them before the ghosts do:

| Power-Up | Effect | Duration |
|---|---|---|
| ⚡ Speed Boost | Move faster | 8 sec |
| 📚 Multi-Carry | Carry more books at once | 12 sec |
| 🛡️ Ghost Repel | Ghosts keep their distance | 6 sec |
| ⏸️ Time Freeze | All ghosts freeze | 5 sec |
| 🎯 Auto-Sort | Books automatically file themselves | 10 sec |
| 💰 Double Points | All filings worth 2x | 15 sec |
| ➕ Health Restore | Instantly heals 40 HP | Instant |

---

## 🎚️ Difficulty Modes

| Mode | Time Limit | Notes |
|---|---|---|
| 😌 Easy | 120 sec | Ghosts arrive late, health regenerates |
| 😤 Medium | 90 sec | Balanced chaos |
| 😰 Hard | 60 sec | No health regen. No mercy. |
| ♾️ Endless | No limit | Waves escalate forever. Good luck. |

---

## 🧠 What I Learned Building This

This is a full-featured game built with nothing but the tools baked into every web browser. Here's what went into it:

### 🏗️ HTML — *The Blueprint*
A single canvas element and a wrapping div. The whole game renders onto one blank drawing board: minimal HTML, maximum game.

### 🎨 CSS — *The Atmosphere*
Mostly handling the background, the CRT scanline effect is overlaid on the entire screen, and making sure the canvas scales to fill any device. Those subtle horizontal lines you see? That's CSS making a browser game feel like an old arcade cabinet. 🕹️

### 🧠 JavaScript — *Everything Else*
This is where the real work lives. Key concepts used include:

- **Object-oriented thinking** — each ghost, book, shelf, and power-up is its own data structure with its own properties and behaviors
- **Game state management** — juggling menus, gameplay, pause, and game-over screens without them fighting each other
- **Delta time physics** — movement uses real elapsed milliseconds so the game runs at the same speed on a fast laptop and a slow one
- **Collision detection** — every book pickup, ghost touch, projectile hit, and parry window is calculated with bounding-box math
- **Enemy AI** — each ghost type has its own decision-making: the Ranged ghost *maintains distance*, the Mimic sits still until you get too close, the Bomber *speeds up* when it's about to explode
- **Combo & scoring systems** — tracking chains, timeouts, multipliers, and floating score popups
- **A mini-map** — scaling the full game world down to a 120×120 pixel overview in real time

### 🖼️ The Canvas API — *The Paintbrush*
Every sprite, every glow effect, every shelf label, every ghost is drawn with `fillRect`, `arc`, and `fillText`. Zero image files. The eerie glow around haunted shelves? Radial gradients. The ghost animations? Sine waves applied to coordinates. Learning to make art with math is one of the most satisfying things you can discover as a developer. ✨

---

## 📁 Project Structure

```
the-luchabrarian/
└── index.html    ← ~13,000 lines of pure determination 🥵🥵🥵
```

One file. No `package.json` staring at you with quiet judgment. Just open it and play. 🎮

---

## 🚀 How To Run It

1. Download `index.html`
2. Open it in any modern browser
3. Choose your difficulty
4. Try not to let the Mimic ghost fool you

Or play it live at: `https://oscaram007.github.io/luchabrarian15.0/`

---

## 📚 About This Project

As a library employee, I think about organization, information systems, and how people navigate complexity every single day. This project started as a question: *what if the stakes of getting the filing wrong were… ghosts?*

It grew from a simple concept into a full action game with enemy AI, power-up systems, achievements, and a combo chain. The Forbidden books shelf is real. The Trash can is real. The feeling of triumphantly ***YEETING*** 😎🙌 a book at a ghost and watching it explode? That's new, but honestly, it should be an option at the reference desk. 📕💥

This represents weeks of reading documentation 📖, reverse-engineering how other games handle AI, a frankly embarrassing amount of time tweaking ghost glow effects, and the slow, deeply satisfying process of building something complex out of very simple pieces.

---

## 🛠️ Built With

- Pure **HTML5**
- Pure **CSS3**
- Pure **JavaScript** (ES6+)
- The browser's built-in **Canvas 2D API**
- The **Press Start 2P** font (via Google Fonts — the one external thing, and worth every byte)
- Zero game engines 💪

---

## 🗺️ What's Next?

We'll see... 👀

---

## 📜📄 Copyright & License

**Copyright © 2026 by Oscar A. Martinez**

All rights reserved. This software, source code, documentation, and associated materials (collectively, "the Work") are protected under the copyright laws of the United States and international copyright treaties.

### Restrictions

No part of this Work may be reproduced, modified, adapted, distributed, publicly displayed, performed, or transmitted in any form or by any means—including but not limited to electronic, mechanical, digital reproduction, version control systems, code repositories, or cloud storage—without the prior written permission of the author, except as expressly permitted below or under applicable copyright law.

### Permitted Uses

Brief code snippets may be quoted in reviews, tutorials, academic papers, or other noncommercial commentary for purposes of illustration, critique, or education, provided proper attribution is given.

### Prohibited Actions

The following are strictly prohibited without explicit written authorization:

- ❌ Copying, forking, or cloning this code for redistribution
- ❌ Incorporating this code into other projects, whether open-source or proprietary
- ❌ Reverse engineering, decompiling, or disassembling any compiled portions
- ❌ Removing or altering copyright notices, attribution, or licensing information
- ❌ Commercial use, sublicensing, or sale of this Work or derivatives thereof

**Any unauthorized use, reproduction, or distribution of this Work may result in civil and criminal liability under applicable law. The moral rights of the author have been asserted.**

---

*Made with curiosity, late nights, and a deep personal respect for anyone who has ever worked a library reference desk. You are the real Luchabrarians. 😊🏆*
