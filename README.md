# OBJtoProjectorGIFMaker

A single-page browser app that turns `.OBJ` models into stylized holographic projector scenes and exports animated GIFs.

## Overview

`OBJtoProjectorGIFMaker` renders a 3D object inside a futuristic holo-projector interface. Users can upload an OBJ file, customize the projector appearance, enable holographic effects, and record a looping GIF directly from the browser.

## Features

- Upload `.OBJ` models and preview them in real time
- Hologram color presets plus custom color selection
- Choose projector base style: cylindrical, octagonal, or portable
- Visual effect toggles: flat projection, HUD overlay, dust, attenuation, bloom, glitch, scan ring, wireframe
- Custom HUD text with dynamic placeholders
- Export a 6-second looping GIF using the in-app recorder

## How to Use

1. Open `index.html` in a modern browser.
2. Upload a `.OBJ` file using the sidebar control.
3. Adjust the holo style, projector style, and visual effect toggles.
4. Press `Record 6s Loop` to generate a GIF.
5. Download the result from the GIF modal.

### Local Hosting

For the best experience, serve the project with a local HTTP server instead of opening the file directly.

```powershell
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Supported Input

- `.OBJ` files only

## Built With

- `HTML`, `CSS`, `JavaScript`
- `Three.js` (3D scene, OBJLoader, OrbitControls)
- `EffectComposer`, `RenderPass`, `UnrealBloomPass`
- `gif.js` for GIF export
- Tailwind CSS for UI styling
- Phosphor Icons for interface icons

## Files

- `index.html` — application UI, rendering logic, and export workflow
- `LICENSE.md` — license text (GNU GPL v2)
- `README.md` — project documentation

## License

This project is licensed under the GNU General Public License version 2 (GPLv2). See `LICENSE.md` for full details.

