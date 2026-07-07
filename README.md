# 🎯 Box Knockdown — Carnival Arcade Game

A fun, physics-based 3D carnival-style "can knockdown" arcade game built entirely with **Three.js** and vanilla JavaScript — no build tools, no backend, no installation. Just open `index.html` and play.

![Platform](https://img.shields.io/badge/platform-Web-blue)
![Engine](https://img.shields.io/badge/engine-Three.js-black)
![License](https://img.shields.io/badge/license-MIT-green)
![Made with](https://img.shields.io/badge/made%20with-JavaScript-yellow)

---

## 🕹️ About

Box Knockdown is a mobile-friendly, desktop-friendly, single-page arcade game where players throw balls to knock down stacks of cans, crates, and neon boxes across **20 levels** spread over 5 themed stages, each introducing new mechanics and increasing difficulty.

| Stage | Levels | Theme |
|-------|--------|-------|
| 1 | 1–4 | **Warm-Up Alley** – simple, growing stacks |
| 2 | 5–8 | **Double Trouble Row** – multiple stacks at once |
| 3 | 9–12 | **Shaky Platforms** – stacks on moving platforms |
| 4 | 13–16 | **Windy Boulevard** – wind gusts and swinging obstacles |
| 5 | 17–20 | **The Grand Carousel** – rotating trick formations |

---

## ✨ Features

- 🎮 **Physics-based gameplay** — custom lightweight physics for satisfying falling, bouncing, and chain-reaction collisions
- 🌪️ **Dynamic level mechanics** — moving platforms, wind gusts, swinging obstacles, and rotating carousel formations
- 🎱 **Four ball types** with distinct behavior:
  - ⚫ Heavy — high knockdown force, low bounce
  - 🟢 Bouncy — high restitution, chains multiple hits
  - 🔴 Explosive — detonates on impact for area damage
  - 🔵 Fast — flat, high-speed trajectory
- 📦 **Three box skins** — metal cans, wooden crates, glowing neon boxes
- 👆 **Swipe/drag-to-aim controls** with a live trajectory preview and power meter — works with mouse, trackpad, or touch
- 🏆 **Scoring system** — points for accuracy, speed, and boxes knocked down, with a 1–3 star rating per level
- 🪙 **Coins, daily bonus, and a session leaderboard**
- 🔊 **Procedurally generated audio** — arcade sound effects and background music synthesized live via the Web Audio API (no audio files to download)
- 📱 **Responsive & mobile-optimized** — automatically reduces render quality on phones for smooth performance, with a friendly fallback message on unsupported devices/browsers
- 🌐 **Fully offline-capable** after the first load (aside from the CDN-hosted engine/fonts)

---

## 🚀 Getting Started

### Play instantly
Simply open [`index.html`](./index.html) in any modern browser:

```bash
git clone https://github.com/<your-username>/box-knockdown.git
cd box-knockdown
open index.html      # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

Or just double-click the file in your file explorer.

> **Note:** An internet connection is required the first time you open the game, since it loads [Three.js](https://threejs.org/) and Google Fonts from public CDNs. After that, gameplay works fully offline.

### Host it online
Since this is a static single-file game, it can be deployed anywhere for free:

- **GitHub Pages** — enable Pages on this repo (Settings → Pages → deploy from `main` branch) and it will be live at `https://<your-username>.github.io/box-knockdown/`
- **Netlify / Vercel** — drag-and-drop deploy, zero configuration
- **Any static web host** — just upload `index.html`

---

## 🎮 How to Play

| Action | Control |
|---|---|
| Aim | Click/touch and drag |
| Set power | Drag distance (further = more power) |
| Throw | Release |
| Switch ball type | Tap a ball icon at the bottom of the screen |
| Pause | Tap the pause button (top right) |

**Tip:** This is a click-and-*drag* (slingshot-style) control, not a single click/tap — pull back and release, like a real toss.

---

## 🛠️ Tech Stack

- [Three.js](https://threejs.org/) (r128) — 3D rendering
- Vanilla JavaScript (ES6) — game logic, custom physics engine, UI
- Web Audio API — procedural sound effects & music
- HTML5 / CSS3 — UI, theming, and layout
- No build step, no dependencies to install, no backend

---

## 📁 Project Structure

```
box-knockdown/
├── index.html      # Entire game — markup, styles, and game logic
└── README.md        # This file
```

The whole game intentionally lives in a single self-contained HTML file for maximum portability — no bundler, package manager, or server required.

---

## ⚠️ Known Limitations

- Coins, unlocked levels, and leaderboard scores are stored **in-memory only** for the current browser session — they reset on page reload since no backend/database is included.
- Physics is a simplified arcade-style model (sphere/AABB approximations tuned for fun, satisfying gameplay) rather than a full rigid-body physics engine.

---

## 🤝 Contributing

Contributions, bug reports, and feature ideas are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes
4. Open a pull request

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE).

---

## 🙌 Acknowledgements

- [Three.js](https://threejs.org/) for the 3D rendering engine
- [Google Fonts](https://fonts.google.com/) — *Bangers* and *Baloo 2* for the carnival typography
