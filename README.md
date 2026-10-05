# NEXUS — Holographic Display Unit

A single-file, interactive Three.js showcase: a levitating glass cube with a shader-driven hologram on a hex pedestal, over a reflective polished-concrete floor, with neon bloom, particles, and a HUD overlay.

## Features
- Amber neon that shifts to magenta on hover
- Custom GLSL hologram (fresnel, scanlines, flicker) + wireframe overlay
- Reflective floor (`Reflector`) with procedural concrete texture
- Bloom post-processing (`UnrealBloomPass`)
- Auto-orbit camera that pauses while you drag
- 5 swappable specimens

## Controls
| Input | Action |
|-------|--------|
| Click pedestal | Next specimen |
| Drag | Rotate view |
| `1`–`5` | Select specimen |
| `Space` | Toggle auto-orbit |

## Run locally
No build step. Open `index.html` in a modern browser (internet needed for Three.js and Google Fonts via CDN), or serve it:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to GitHub Pages
1. Push this repo to GitHub.
2. Settings → Pages → Source: `main` branch, `/ (root)`.
3. Your site will be live at `https://<username>.github.io/<repo>/`.

## Customize
Edit the `CONFIG` object and `modelDefs` array in `index.html` to change colors, sizes, or specimens.

## Tech
Three.js r160 (ES modules via import map), GLSL shaders, WebGL.

## License
MIT
