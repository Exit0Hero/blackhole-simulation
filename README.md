# Black Hole Simulation

A stylized, interactive WebGL black hole lensing demo showcasing light bending, halo rings, and an accretion disk built with Three.js.

This repository contains a single-page demo (`index.html`) that runs entirely in the browser. It uses plain ES modules (three.js from UNPKG) and requires no build step.

## Features
- Animated accretion disk with shader-driven turbulence
- Additive glow / corona and halo rings
- Curved light-ray paths to visualize gravitational lensing
- Orbit controls: drag to rotate, scroll to zoom

## Run locally
The easiest way is to open `index.html` in a modern browser. For a better local experience (correct MIME types and module loading), run a simple static server. Examples:

Using Python 3:

```bash
python -m http.server 8000
# then open http://localhost:8000/index.html
```

Using Node (http-server):

```bash
npx http-server -c-1
# then open the printed local address
```

## Live demo (GitHub Pages)
This repository includes a GitHub Actions workflow that publishes the site to GitHub Pages automatically on push to `main`.

Once the workflow completes, the page will be available at:

https://Exit0Hero.github.io/blackhole-simulation/

If you'd like a different owner or custom domain, update the repository `Settings → Pages` or add a `CNAME` file.

## Credits
- Built with Three.js (https://threejs.org)

## License
This project is released under the MIT License — see `LICENSE`.