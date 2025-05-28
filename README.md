# ExpertsStage

A 3D visualization of Stage.glb model using Three.js.

## Features

- 3D model loading with GLTFLoader
- HDRI environment lighting using dancing_hall_1k.hdr
- Orbit controls for interactive camera movement
- Responsive design
- Loading progress indicator

## Usage

Simply open `index.html` in a modern web browser to view the 3D scene.

Note: For security reasons, you might need to serve the files through a local web server to properly load the 3D model and HDRI map.

## Local Development Server

You can use a simple HTTP server to serve the files. For example, with Python:

```bash
# Python 3
python -m http.server

# Python 2
python -m SimpleHTTPServer
```

Or with Node.js:

```bash
npx serve
```

Then open http://localhost:8000 (or the provided URL) in your browser. 