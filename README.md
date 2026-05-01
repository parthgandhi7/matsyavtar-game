# Matsyavatar - The Great Deluge

A mobile-friendly HTML5 Canvas game where you guide Matsya (fish) while towing Manu's boat through storm obstacles.

## Theme manifest (visual-only customization)

Visual assets are now controlled by `assets/theme-default.json`. You can replace look-and-feel without touching game logic in `index.html`.

- Manifest keys:
  - `water`
  - `land`
  - `obstacles.whirlpool`
  - `obstacles.debris`
  - `obstacles.prop`
  - `decals` (Matsya + boat SVG paths)
- Typical per-asset params:
  - `texture` path
  - `tint`
  - `scale`
  - `animationSpeed`
  - `blendMode` (reserved for effect styling)

### Replace visuals safely

1. Put replacement textures/SVGs in `assets/`.
2. Edit file paths/colors/scales in `assets/theme-default.json`.
3. Reload the page.

If a manifest file or asset fails to load, the game falls back to procedural/material defaults in code and shows load status/errors in the start screen (`statusText`).

## Run locally

Just open `index.html` in your browser.

## Deploy on GitHub Pages

1. Push this repository to GitHub.
2. In repo settings, open **Pages**.
3. Set source to `Deploy from a branch`.
4. Choose `main` (or your branch) and `/ (root)`.
5. Save. GitHub will host `index.html` automatically.
