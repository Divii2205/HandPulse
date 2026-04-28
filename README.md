
# HandConnect

A simple, single-page static project containing `index.html` that serves as the starting point for the HandConnect web interface.

## Summary

- Lightweight static prototype; no build tools required.
- Single entry point: `index.html`.

## Features

- Minimal, easy to edit HTML for quick prototyping.
- Ready to serve locally or deploy to static hosts.

## Simulation

- This project includes a browser-based hand-interaction simulation used to prototype gesture-driven UI and visualizations.
- The simulation typically reads webcam input (with user permission), runs hand detection/pose estimation, and renders visual feedback on the page.
- Purpose: validate interaction flows, test gestures, and iterate on UX without backend dependencies.

## Main Technologies (examples)

- MediaPipe Hands — real-time hand tracking and landmarks (commonly used for fast, accurate hand detection).
- Plain JavaScript + DOM/CSS — for UI wiring, event handling, and lightweight interactions.

## Getting Started

1. Open `index.html` directly in your browser for a quick preview.
2. Or serve locally with Python or a static server:

```bash
python -m http.server 8000
# or
npx http-server -p 8000
```

Then open http://localhost:8000 in your browser. If the simulation uses the webcam, grant camera permission when prompted.

## Development

- Edit `index.html` to update the UI, simulation wiring, or to swap libraries (e.g., switch MediaPipe for TensorFlow.js).
- Add library-specific scripts or assets as needed; no build step is required for pure client-side prototypes.