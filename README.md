# RoomKit

A single-file 3D interior-design editor that runs in the browser (HTML + Three.js, no build step).

## Features
- Free-form floor plan: draw rooms and walls in 2D, typed lengths, snapping, vertex/wall dragging
- Floor-plan underlay: import an image, calibrate scale, trace over it
- Doors and windows embedded in walls, slidable along them
- 13 furniture types with materials/textures, collision detection and wall snapping
- Import GLB models, export GLB (single item or whole scene)
- Export Rhino `.3dm` (millimetres, Z up, layers: walls / floors / doors & windows / furniture; meshes, not NURBS). Revit 2022+ can import `.3dm` as reference geometry. Falls back to `.obj` if the rhino3dm WebAssembly library cannot be loaded.
- Image to 3D model (only works inside Claude, uses the page `sample` capability)
- Undo/redo, autosave (localStorage + IndexedDB), JSON import/export
- Views: 3D perspective, top, 2D plan

## Run
Open `index.html` in a browser (needs internet for the Three.js CDN), or enable GitHub Pages
(Settings -> Pages -> Deploy from branch -> `main` / root).
