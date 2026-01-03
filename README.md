# CS460 – Computer Graphics

Coursework repository for **CS460: Computer Graphics** at the University of Massachusetts Boston (Fall 2022).

These projects explore interactive, browser-based 3D graphics and visualizations using WebGL and Three.js — covering transformations, camera controls, materials, texture mapping, lighting, and animation.

---

## Course Information

| | |
|---|---|
| **University** | University of Massachusetts Boston |
| **Course** | CS460 – Computer Graphics |
| **Term** | Fall 2022 |
| **Prerequisites** | CS 310, Math 260 |
| **Course Site** | [cs460.org](https://cs460.org) |

---

## Live Demos

All assignments are hosted via GitHub Pages:

| Assignment | Demo Link |
|------------|-----------|
| Assignment 01 | [View Demo](https://dathrika13.github.io/cs460student/01/index.html) |
| Assignment 02 | [View Demo](https://dathrika13.github.io/cs460student/02/index.html) |
| Assignment 03 | [View Demo](https://dathrika13.github.io/cs460student/03/index.html) |
| Assignment 04 | [View Demo](https://dathrika13.github.io/cs460student/04/index.html) |
| Assignment 05 | [View Demo](https://dathrika13.github.io/cs460student/05/index.html) |
| Assignment 06 | [View Demo](https://dathrika13.github.io/cs460student/06/index.html) |
| Assignment 07 | [View Demo](https://dathrika13.github.io/cs460student/07/index.html) |
| Assignment 08 | [View Demo](https://dathrika13.github.io/cs460student/08/index.html) |
| Assignment 09 | [View Demo](https://dathrika13.github.io/cs460student/09/index.html) |
| **Final Project** | [**3D Interactive City**](https://dathrika13.github.io/cs460student/3dCityProject/) |

---

## Final Project: 3D Interactive City

A fully animated 3D city scene built with Three.js featuring:

- Multiple imported OBJ models (buildings, vehicles, terrain)
- Skybox environment and textured surfaces
- Animated cars driving along roads
- Helicopter flying across the scene
- Interactive robots that walk and navigate obstacles
- Real-time controls via dat.GUI

> **Note:** Video textures require running via a local web server rather than opening files directly.

---

## Tech Stack

| Technology | Usage |
|------------|-------|
| JavaScript | Core programming language |
| WebGL | Hardware-accelerated 3D rendering |
| Three.js | 3D graphics library |
| OBJ/MTL Loaders | 3D model importing |
| dat.GUI | Interactive runtime controls |

---

## Running Locally

Some browsers block textures, video, and audio when opened via `file://`. Use a local server instead.

### Python
```bash
python3 -m http.server 8000
```

### Node.js
```bash
npx http-server -p 8000
```

Then navigate to:
```
http://localhost:8000/01/index.html
http://localhost:8000/3dCityProject/
```

---

## Repository Structure

```
cs460student/
├── 01/ - 09/           # Course assignments
├── 3dCityProject/      # Final project
└── README.md
```

> Keep assets inside their respective folders to ensure GitHub Pages loads them correctly.

---

## References

- [Three.js Documentation](https://threejs.org/docs/)
- [CS460 Course Site](https://cs460.org)
