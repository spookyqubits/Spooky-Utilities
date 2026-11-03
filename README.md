# Spooky Utilities · SpookyQubits

A separate collection of visual learning utilities alongside [Ghosts and Gates](https://spookyqubits.github.io/Ghosts_and_Gates/) and [Spooky Signals](https://spookyqubits.github.io/SpookySignals/).

## Utilities

- **Bloch Sphere** — `games/bloch-sphere/`: compare one, two, or three independent one-qubit preparations under X, Y, Z, H, S, and T. Includes camera dragging, a progress scrubber, and measurement probabilities. Previously previewed with the working name “Block Sphere.”
- **Ghost Numbers** — `games/ghost-numbers/`: learn complex-number coordinates, addition, rotation, and scaling through six missions and Free Play. Includes a draggable 3D presentation of the plane and a square-on Flat View.

Both are playable previews, designed for phones and usable on larger screens. Multiple Bloch-sphere ghosts represent independent preparations, not an entangled register. Complex-plane points represent numbers, not complete qubit states. Animation paths are teaching representations, not physical trajectories. Learning gains have not been evaluated.

## Run and host

This is a static collection. No database, accounts, analytics, advertising, external scripts, or external fonts are needed. The public files are:

```text
index.html
utilities.css
assets/ghost.svg
games/bloch-sphere/index.html
games/ghost-numbers/index.html
source/bloch-sphere.html
source/ghost-numbers.html
downloads/spooky-utilities-offline.zip
```

Serve the directory with `python3 -m http.server 8080`, or open `index.html`. Individual game pages also work offline. Progress is stored in this browser when local storage is available; storage can be unavailable for local files or in private browsing.

Publish the root of `main` with GitHub Pages. `.nojekyll` is included. The intended collection address is `https://spookyqubits.github.io/Spooky-Utilities/`.

The `source/` directory contains the editable game fragments. The `games/` pages are self-contained standalone exports of those fragments, with a navigation header and a browser-local persistence bridge. Re-export a changed fragment when updating its standalone page.

The local source/build project is `Logo-Website/spooky-utilities-playground`. It builds the explicit public file set and an upload ZIP; unrelated workspace files are excluded.

Prepared for SpookyQubits, 3 November 2026. Original mathematical and educational sources remain credited inside Ghost Numbers.
