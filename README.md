# SkyWheels

**Fancy flying cars.** A kid-friendly 3D browser game — drive the city, take the big bridge **over** the mountain, watch for animals, and stay out of the spooky cave!

[![Play Live](https://img.shields.io/badge/▶_Play_Live-SkyWheels-7ad7ff?style=for-the-badge&logo=googlechrome&logoColor=white)](https://luvbuniz.github.io/skywheels/)
[![GitHub](https://img.shields.io/badge/GitHub-luvbuniz%2Fskywheels-181717?style=for-the-badge&logo=github)](https://github.com/luvbuniz/skywheels)
[![Made with Three.js](https://img.shields.io/badge/Three.js-0.160-black?style=for-the-badge&logo=threedotjs&logoColor=white)](https://threejs.org/)

---

## ▶ Play now

**Live game:** [https://luvbuniz.github.io/skywheels/](https://luvbuniz.github.io/skywheels/)

### 📱 Tablet install (offline + local save)

1. Open the live link **once while online** (hotspot is fine) so the tablet downloads the game  
2. **iPad (Safari):** Share → **Add to Home Screen**  
3. **Android (Chrome):** Menu ⋮ → **Add to Home screen** / **Install app**  
4. Open from the **SkyWheels** home-screen icon anytime  

After that first load, the game can run **offline** (no internet needed).

**Local save:** Progress is saved on **each tablet separately** (car position, fuel, gas cans, walking).  
Kids do not share or overwrite each other’s saves.

---

## About

**SkyWheels** is a free browser driving & flying game. You pilot a fancy sports car through a neon city, over a giant mountain bridge, past animals in the countryside, and (if you dare) near a dangerous cave.

| Area | What you’ll find |
|------|------------------|
| **City** | Roads, buildings, lights, plaza — crash = game over |
| **Mountain** | Solid rock peaks — **no road through it** |
| **Bridge** | Huge bridge that goes **over** the mountain |
| **Cave** | Spikes, crystals, lava & bats that can crash you |
| **Animals** | Deer, sheep, cows, dogs, birds, bats |
| **Traffic** | Other fancy cars on roads, on the bridge, and in the sky |

### Rules
- Hit a **building**, **mountain**, **other car**, **animal**, **cave hazard**, or the **monster** → **GAME OVER**
- You **cannot drive through** solid things
- **Enter buildings only through doors** (press **E** while walking)
- **Fuel** runs out — fill at the gas station or with a gas can
- Use the **control sign** on the right while you play

### New places
| Place | Where / how |
|-------|-------------|
| **Airport** | East of the city — park, get out (**F**), walk in the **door** (**E**) |
| **Gas station** | West of the city — park at pumps + **E** to fill · shop door for **gas cans** |
| **Monster cave** | Far northwest — purple on minimap — monster chases you! |

### Animals & people
Deer, sheep, cows, dogs, **foxes**, lots of **birds**, bats, and **people walking on sidewalks**.

---

## Controls

### 📱 Touch (tablet / phone)

Touch controls switch on automatically on touch devices (and on the first touch anywhere):

| Control | Action |
|---------|--------|
| **Left side of screen** | A big circle appears under your finger — push **up to GO**, sideways to steer, down to brake/reverse |
| **Drag anywhere else** | Look around (snaps back in the car) |
| **⬆️ FLY / ⬇️ DOWN** | Hold to fly up / come down |
| **🛑 STOP** | Hold to stop the car |
| **🚶 WALK** | Get out of / back into the car |
| **⛽ USE** | Doors, gas pump, buy/use gas can |

While walking, a **glowing blue arrow** marks your parked car so you can always find your way back.

### ⌨️ Keyboard

Always shown on the in-game control sign (right side):

| Key | Action |
|-----|--------|
| **W / ↑** | Gas |
| **S / ↓** | Brake / reverse |
| **A D / ← →** | Steer |
| **Space** | Fly up (in car) |
| **Shift** | Fly down |
| **F** | Get out of / into car |
| **E** | Open door · gas pump · buy/use gas can |
| **C** | Look behind you |
| **V** | Camera: behind car (default) / close-up |
| **R** | Restart after crash |

Default camera is **behind your car** so you can see your fancy car in front of you. Rear-view mirror is always on.

---

## Features

- Engine & flying sound effects (Web Audio)
- Crash sound + game over screen
- Solid collisions (no ghosting through walls)
- Bridge path over the mountain
- Animals that roam and can crash you
- Hazard cave with spikes, crystals, lava, bats
- AI traffic on city roads, bridge, and sky
- Controls panel always visible while playing
- Minimap + speed + altitude HUD

---

## Run locally

```bash
npx --yes serve .
```

Or open `index.html` in a modern browser.

---

## Links

| | |
|---|---|
| **Play live** | [luvbuniz.github.io/skywheels](https://luvbuniz.github.io/skywheels/) |
| **Source** | [github.com/luvbuniz/skywheels](https://github.com/luvbuniz/skywheels) |
| **Author** | [luvbuniz](https://github.com/luvbuniz) |

## License

Made for fun. Free to play, share, and remix.
