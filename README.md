# VOID RAID

A neon arcade space shooter. Hold the line, wipe the fleet, survive the raid.

Single-file HTML5 game. No libraries, no assets, no build step. Open `index.html` and play.

## Play

Open `index.html` in any modern browser, or deploy with GitHub Pages.

## Controls

### Desktop

- **A / D** or **Arrow keys** — move
- **Mouse** — aim / move
- **Space** or **Click** — fire
- **ESC** or **P** — pause

### Mobile / Tablet

- **Drag** — move
- **Hold** — fire
- **II** button — pause

Works in portrait and landscape. Safe-area insets are respected on notched devices.

## Features

- Grid enemy waves with escalating speed, fire rate, and hit points
- Player bullets and enemy fire with AABB collision
- Lives, score, and high score (`localStorage`)
- Power-ups: Rapid Fire (`R`) and Shield (`S`)
- Particle explosions, screen shake, starfield parallax
- Web Audio API SFX (shoot, explosion, hit, power-up)
- Pause menu: Resume / Restart / Sound toggle / Title
- Auto-pause on tab hide and window blur
- Object pooling for bullets and particles
- 60 FPS `requestAnimationFrame` loop, responsive fullscreen canvas

## Tech stack

- Vanilla JavaScript (ES6)
- HTML5 Canvas 2D
- Web Audio API
- CSS (inline)

No npm, no bundler, no CDNs, no external images or audio.

## Deploy on GitHub Pages

1. Create a repository and push this project (keep `index.html` at the repo root).
2. GitHub → **Settings** → **Pages**.
3. Source: **Deploy from a branch**.
4. Branch: `main` (or `master`), folder: `/ (root)`.
5. Save. The game is live at `https://<user>.github.io/<repo>/`.

Local preview: double-click `index.html` or run any static server from this folder.

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.
