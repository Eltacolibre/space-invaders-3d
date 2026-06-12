# 🛸 Space Invaders 3D

A neon-retrowave 3D remake of the 1978 arcade classic, built with [Three.js](https://threejs.org/) in a single HTML file. No build step, no dependencies to install — just open and play.

**▶ Play it here: https://eltacolibre.github.io/space-invaders-3d/**

## ✨ Flair & modern effects

- **Voxel invaders** — the classic 2-frame sprite animations, extruded pixel-by-pixel into 3D voxel meshes (squid, crab, octopus — each row worth different points, just like 1978)
- **Unreal bloom post-processing** — everything emissive glows
- **Retrowave grid floor** — custom GLSL shader, scrolling toward the horizon with a magenta-to-cyan gradient
- **Particle explosions** with additive blending and physics (drag + gravity), plus point-light flashes
- **Screen shake** on kills and hits, camera parallax that follows your ship and mouse
- **CRT overlay** — scanlines and vignette for that arcade cabinet feel
- **Synthesized sound** — all SFX generated live with the Web Audio API, including the iconic descending 4-note invader march that speeds up as the fleet thins
- **Bonus UFO** flying saucer worth 100–300 points
- Hi-score persistence, escalating waves, the works

## 🎮 Controls

| Key | Action |
|-----|--------|
| `←` `→` or `A` `D` | Move |
| `Space` | Fire (max 3 shots in flight) |
| `P` | Pause |
| `M` | Mute |
| `Enter` | Start / retry |

## 🚀 Run locally

Serve the folder with any static server, e.g.:

```sh
npx serve .
# or
python -m http.server
```

Then open `http://localhost:8000` (or whatever port your server reports). A server is needed because the game loads Three.js as an ES module from a CDN via an import map.

## 🤖 Credits

Built with [Claude Code](https://claude.com/claude-code). Original game by Tomohiro Nishikado / Taito (1978).
