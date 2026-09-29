# Voxel Portal

Pick an object and watch a cloud of cubes rebuild itself into it, live, inside a floating portal.

- A loose cluster of cubes sits between two iridescent frames and trails your mouse like liquid.
- Choose one of 25 objects and press **Transform**: the cubes tighten, lift into a spinning vortex, then peel off one by one and build the object from the bottom up, taking on its colours mid-flight.
- Desktop shows the picker beside the portal; phones get a bottom sheet with a sideways-scrolling row of objects so the portal stays in view.

## Run locally

It's plain HTML, CSS and JavaScript with no build step. Serve the folder with any static server:

```bash
python3 -m http.server 4181
```

Then open http://localhost:4181.

## Files

- `index.html`: the page (object picker, Transform button, layout for desktop and mobile)
- `portal.html`: the 3D scene, built with [three.js](https://threejs.org): grid walls, frames, the cube cluster, the object models and the transform animation
- `assets/`: the object icons
