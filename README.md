# OBJtoProjectorGIFMaker

A browser-based utility that converts `.OBJ` models into a stylized holographic projector scene and exports a looping GIF.

## Description

`OBJtoProjectorGIFMaker` is a single-file web app built with Three.js and GIF.js. It loads OBJ geometry, wraps it in a futuristic holographic environment, and lets you export an animated hologram clip without any build setup.

## Key Features

- Real-time `.OBJ` model preview in a sci-fi projector display
- Multiple holo color themes and custom color input
- Selectable projector base styles: cylindrical, octagonal, or portable
- Toggleable holographic effects: flat projection, HUD overlay, dust particles, attenuation, bloom, glitch, scan ring, wireframe
- Editable HUD text with dynamic placeholders
- Generate a 6-second looping GIF from the rendered scene

## Quick Start

1. Open `index.html` in a modern browser.
2. Upload your `.OBJ` file from the sidebar.
3. Customize the holo style and projector appearance.
4. Enable or disable visual effects.
5. Click `Record 6s Loop` to render and save the GIF.

## Recommended Setup

For best results, run a local HTTP server instead of opening the file directly.

```powershell
python -m http.server 8000
```

Open the app at:

```text
http://localhost:8000
```

## Supported File Types

- `.obj` only

## Project Structure

- `index.html` — main application UI, 3D scene, controls, and GIF export logic
- `LICENSE.md` — license text (GNU GPL v2)
- `README.md` — project documentation

## Technologies Used

- `Three.js` for 3D rendering and scene management
- `OBJLoader` for loading geometry
- `OrbitControls` for camera control
- `EffectComposer` + `UnrealBloomPass` for lighting and bloom effects
- `gif.js` for GIF capture and export
- `Tailwind CSS` for styling
- `Phosphor Icons` for iconography

## Notes

- The app runs entirely in the browser and does not require a server-side component.
- Large OBJ files may reduce performance during rendering or GIF export.

## License

This project is licensed under the GNU General Public License version 2 (GPLv2). See `LICENSE.md` for details.

