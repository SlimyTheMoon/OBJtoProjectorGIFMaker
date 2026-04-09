# OBJtoProjectorGIFMaker

A browser-based holo-projector GIF generator for `.OBJ` models. Drop in a 3D object, tweak the holographic projector effects, and export a looping animated GIF.

## Features

- Upload a `.OBJ` file and visualize it in a futuristic holographic projector scene
- Choose holo style presets: Deep Space, Alert, Tactical, Archival, or a custom color
- Select projector base style: Cylindrical, Octagonal, or Portable
- Toggle visual effects: flat projection, HUD overlay, ambient dust, attenuation, cinematic bloom, signal glitch, scan ring, wireframe
- Customize HUD text and dynamic data placeholders
- Record a 6-second looping GIF from the rendered scene

## Usage

1. Open `index.html` in a modern browser.
2. Upload your `.OBJ` model using the sidebar upload control.
3. Adjust hologram style, projector base, and effect toggles.
4. Press `Record 6s Loop` to generate and download the GIF.

> If the browser blocks local file access, run a simple local server in the repository folder:
>
> ```bash
> python -m http.server 8000
> ```
>
> Then open `http://localhost:8000`.

## Supported Input

- `.obj` files only (OBJ model loader is built into the page)

## Technology

- `HTML`, `CSS`, `JavaScript`
- `Three.js` for 3D rendering
- `OBJLoader` and `OrbitControls`
- `EffectComposer` with `UnrealBloomPass` for glows
- `gif.js` for GIF export
- `Tailwind CSS` for layout and styling
- `Phosphor Icons` for UI icons

## Project Files

- `index.html` — main app UI, rendering logic, and export workflow
- `LICENSE.md` — project license (GNU GPL v2)
- `README.md` — project overview and usage

## License

This project is licensed under the GNU General Public License v2 (GPLv2). See `LICENSE.md` for details.

