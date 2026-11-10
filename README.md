# Movase — Interactive 3D Scene

A browser-based graphics coursework project using Babylon.js. It loads a glTF scene, provides an orbit camera, and lets the viewer move the model by clicking the ground.

[Open web demo](https://movase-one.vercel.app)

## Project background

I built this interactive 3D scene for a university computer graphics course.

**Previous repository name:** `Web-Based-Simple-Interactive`.

## Implemented features

- glTF model loading with its geometry buffer and texture.
- Orbit/zoom camera controls.
- Hemispheric and directional lighting with ground shadows.
- Click-to-move animation for the loaded model.
- Canvas resizing with the browser window.

**Stack:** JavaScript · HTML · Babylon.js · glTF

## Run locally

Serve the repository over HTTP so the browser can fetch model assets:

```sh
git clone https://github.com/mrafi-aditya/movase-3d.git
cd movase-3d
python -m http.server 8000
```

Open `http://localhost:8000`. No npm installation or build step is required. An internet connection is needed for Babylon.js scripts loaded from its CDN.

## Controls

Drag to orbit the camera, scroll to zoom, and click the ground to animate the model toward the selected position. Camera behavior on touch devices follows Babylon.js defaults.

## Files

| File | Purpose |
|---|---|
| [index.html](index.html) | Page and library loading |
| [script.js](script.js) | Scene, model loading, lighting, and movement |
| `scene.gltf` | Scene description |
| `scene.bin` | Model geometry buffer |
| `main_baseColor.jpeg` | Model texture |

Keep the glTF file, buffer, and texture together when serving the project. This repository demonstrates scene setup and interaction; it does not claim authorship of the underlying 3D asset. Asset provenance and redistribution terms should be documented before reusing it elsewhere.

Earlier coursework: [basic model viewer](https://github.com/mrafi-aditya/Web_Based_Simple_Model) · [lighting and shadows](https://github.com/mrafi-aditya/Web-Based-Simple-Model-Shadow).
