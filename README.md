# UNIVERSE

**Interactive WebGL2 Particle Cosmos**
by Ofir Ben Attar

---

## Overview

**UNIVERSE** is a real-time GPU particle simulation built with **WebGL2**, transform feedback, and GLSL shaders.
It renders large-scale cosmic environments — nebulae, galaxies, vortices, and warp tunnels — driven entirely on the GPU with audio-reactive visuals and cinematic post-processing.

This project is both a technical experiment in high-performance browser graphics and an interactive audiovisual art piece.

---

## Features

### Visual Modes

* **Nebula** — organic curl-noise particle flow
* **Galaxy** — spiral orbital mechanics
* **Black Hole** — accretion gravity well
* **Vortex** — tornado-like column dynamics
* **Warp** — forward hyperspace tunnel

### Rendering & Effects

* WebGL2 Transform Feedback particle simulation
* GPU-driven physics (no CPU particle loops)
* HDR-style bloom with gaussian blur
* Chromatic aberration + film grain
* ACES-style tonemapping
* Background starfield layer

### Interaction

* Mouse attraction / repulsion
* Shockwave bursts (click + release)
* RGB color tuner panel
* Quality scaling (low / medium / high)
* Ambient procedural audio with spectrum analysis
* Camera orbit + zoom

---

## Controls

| Action            | Input                   |
| ----------------- | ----------------------- |
| Rotate camera     | Move mouse              |
| Attract particles | Hold mouse button       |
| Shockwave         | Click + release         |
| Zoom              | Mouse wheel             |
| Switch mode       | Buttons or keys **1–5** |
| Change color      | RGB sliders             |
| Audio volume      | Bottom-right slider     |
| Quality level     | Bottom-left toggle      |

---

## Technical Notes

* **WebGL2 Required**
* Heavy use of:

  * Transform Feedback
  * GLSL noise & curl fields
  * Additive blending
  * Post-processing framebuffers
* Designed for modern desktop GPUs.

Particle counts:

* Low: ~40k
* Medium: ~100k
* High: ~200k

---

## Running the Project

No build step required.

1. Clone the repository:

```bash
git clone https://github.com/yourname/universe.git
```

2. Open the project with a local server (recommended):

```bash
npx serve
```

3. Open the browser and click to begin.

---

## File Structure

```
index.html
 ├─ UI layer
 ├─ GLSL shaders (update, render, stars, post)
 └─ Main WebGL application loop
```

All logic currently lives in a single file for simplicity and portability.

---

## Philosophy

UNIVERSE explores the idea of **precision at scale** — small mathematical rules producing vast emergent structures.
Particles are not individually scripted; instead, fields, forces, and noise generate behavior collectively.

The result is less a simulation of space and more a **synthetic cosmology**.

---

## Performance Tips

* Use Chrome or Edge for best WebGL2 performance.
* Reduce quality level if FPS drops.
* Integrated GPUs may struggle at High mode.

---

## License

Open for experimentation and learning.
Attribution appreciated if used in derivative works.

---

## Credits

Design, code, and concept by **Ofir Ben Attar**.
