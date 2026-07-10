# SkyWheels

**Fancy flying cars.** A kid-friendly 3D browser game — drive the city, race through a mountain tunnel, soar over the big bridge, and fly whenever you want.

[![Play Live](https://img.shields.io/badge/▶_Play_Live-SkyWheels-7ad7ff?style=for-the-badge&logo=googlechrome&logoColor=white)](https://luvbuniz.github.io/skywheels/)
[![GitHub](https://img.shields.io/badge/GitHub-luvbuniz%2Fskywheels-181717?style=for-the-badge&logo=github)](https://github.com/luvbuniz/skywheels)
[![Made with Three.js](https://img.shields.io/badge/Three.js-0.160-black?style=for-the-badge&logo=threedotjs&logoColor=white)](https://threejs.org/)

---

## ▶ Play now

**Live game:** [https://luvbuniz.github.io/skywheels/](https://luvbuniz.github.io/skywheels/)

No install. Open the link in Chrome, Edge, or Firefox and hit **START DRIVING**.

---

## About

**SkyWheels** is a free, browser-based driving and flying game. You pilot a super-fancy sports car through:

| Area | What you’ll find |
|------|------------------|
| **City** | Roads, tall buildings, street lights, glowing plaza |
| **Mountain** | Climbing road, rocky peaks, snowy top |
| **Bridge** | Big span over a gorge with towers & cables |
| **Tunnel** | Lit tunnel road through the mountain |
| **Sky** | Other fancy cars flying all around you |

Your car can **drive on roads** and **fly into the air**. Other traffic drives the city and mountain routes while flying cars cruise overhead. There’s a **rear-view mirror**, a **minimap**, and first-person or chase camera modes.

Built as a fun project for kids (and grown-ups who still love cool cars).

---

## Controls

| Key | Action |
|-----|--------|
| **W / ↑** | Gas |
| **S / ↓** | Brake / reverse |
| **A D / ← →** | Steer |
| **Space** | Fly up |
| **Shift** | Fly down |
| **C** | Look behind you |
| **V** | Switch camera (driver’s seat / chase) |
| **R** | Reset if you get stuck |

There’s always a **rear-view mirror** in the top-right and a **minimap** at the bottom.

---

## Features

- First-person driver’s seat + optional chase camera  
- Always-on rear-view mirror  
- Fancy sports cars (chrome, spoilers, underglow, headlights)  
- AI traffic on roads + flying cars in the sky  
- City · mountain · bridge · tunnel world  
- Speedometer, altitude, drive/fly mode badge  
- Runs entirely in the browser (Three.js)

---

## Run locally

Clone or download this repo, then open `index.html` in a modern browser.

If the 3D world stays blank (some browsers block modules from `file://`), use a tiny local server:

```bash
# from this folder
npx --yes serve .
```

Then open the URL it prints (often `http://localhost:3000`).

---

## Project layout

```
skywheels/
├── index.html   # Full game (HTML + CSS + Three.js)
└── README.md    # This file
```

No build step, no npm install for players — just static files.

---

## Tech

- [Three.js](https://threejs.org/) r160 (CDN)
- Vanilla JavaScript (ES modules)
- Hosted with [GitHub Pages](https://pages.github.com/)

---

## Links

| | |
|---|---|
| **Play live** | [luvbuniz.github.io/skywheels](https://luvbuniz.github.io/skywheels/) |
| **Source code** | [github.com/luvbuniz/skywheels](https://github.com/luvbuniz/skywheels) |
| **Author** | [luvbuniz](https://github.com/luvbuniz) |

---

## License

Made for fun. Free to play, share, and remix.
