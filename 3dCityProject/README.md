# 3D Interactive City

A browser-based 3D interactive city scene built with Three.js and WebGL, featuring dynamic animations, interactive elements, and a fully explorable environment.

**[Live Demo](https://dathrika13.github.io/cs460student/3dCityProject/)**

---

## Overview

This project renders a 3D city environment complete with buildings, vehicles, terrain, and interactive robots. Users can navigate the scene, spawn objects, and control animations through an intuitive interface.

## Features

- **Immersive Environment** — Skybox backdrop with textured ground plane representing city roads
- **3D Models** — Buildings, trees, stadium, helicopter, cars, and mountains loaded via OBJ/MTL
- **Interactive Robots** — Click to spawn robots that walk and navigate around obstacles
- **Animated Elements** — Cars drive along roads, helicopter flies across the scene
- **Dynamic Lighting** — Procedurally generated street lights throughout the city

## Tech Stack

| Technology | Purpose |
|------------|---------|
| Three.js (r104) | 3D rendering engine |
| WebGL | Hardware-accelerated graphics |
| TrackballControls | Camera navigation |
| OBJLoader / MTLLoader | 3D model importing |
| dat.gui | Runtime UI controls |

## Controls

| Input | Action |
|-------|--------|
| Mouse drag | Rotate camera |
| Scroll wheel | Zoom in/out |
| Right-click drag | Pan view |
| Shift + Click | Spawn robot at location |

### GUI Options
- `walk` — Start robot walking behavior
- `AnimateCity` — Trigger vehicle and helicopter animations

## Getting Started

### Prerequisites
A local web server is required. Opening `index.html` directly via `file://` may cause asset loading issues.

### Option 1: Python Server
```bash
cd project-root
python3 -m http.server 8000
```
Then navigate to `http://localhost:8000/3dCityProject/index.html`

### Option 2: VS Code Live Server
1. Install the **Live Server** extension
2. Right-click `index.html` → **Open with Live Server**

## Project Structure

```
3dCityProject/
├── index.html              # Main entry point
├── helper.js               # Procedural mesh helpers
├── robot.js                # Robot creation & animation
├── lights.js               # Street light objects
├── signal.js               # Signal/utility logic
├── Models/                 # Car models & textures
├── UH60/                   # Helicopter model
├── everest/                # Mountain terrain
├── apartment01-03/         # Building models
├── Stadium/                # Stadium model
├── amphitheater/           # Amphitheater model
└── textures/               # Road, brick, skybox textures
```

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Blank screen | Check console for errors; ensure dat.gui loads before main script |
| `dat is not defined` | Add dat.gui CDN before your scripts |
| `geometry.setAttribute` error | Three.js r104 uses `addAttribute()` instead |
| `allRobots is not defined` | Add `window.allRobots = all_robots;` after array declaration |
| 404 errors on assets | Verify exact file paths and case sensitivity |

## Deployment

This project deploys seamlessly to GitHub Pages as static HTML/JS.

**Notes:**
- Use relative paths for all assets
- Maintain consistent file/folder casing (GitHub Pages is case-sensitive)
- Verify asset paths after any structural changes

## Credits

- [Three.js](https://threejs.org/) — 3D library and example loaders
- Third-party OBJ models and textures used for educational purposes

## License

This project is for educational purposes.
