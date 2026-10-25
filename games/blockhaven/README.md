# Blockhaven

An original voxel sandbox game that runs in the browser. It is written from scratch: none of its code, textures or data comes from Minecraft or any other game.

## Play

Open `index.html` in a browser, or enable GitHub Pages for this repository and visit `/games/blockhaven/`. It loads Three.js r128 from cdnjs, so it needs an internet connection.

## Controls

| Input | Action |
| --- | --- |
| W A S D | Walk (hold Shift to sprint) |
| Mouse | Look around |
| Space | Jump, or swim up |
| Left click | Break a block (hold to keep digging) |
| Right click | Place the selected block |
| 1 to 9, mouse wheel | Choose a block from the hotbar |
| Middle click | Copy the block you're looking at |
| F | Toggle flying (Space up, Shift down) |
| Esc | Pause |

Phones and tablets get an on-screen joystick and buttons instead.

## How it works

- The world is split into 16 x 16 x 80 block chunks that stream in and out around the player.
- Terrain comes from seeded fractal value noise: hills, snowy mountains, lakes, beaches and forests.
- Each chunk is meshed with hidden-face culling and per-vertex ambient occlusion.
- Textures are pixel art painted procedurally onto a canvas atlas at startup.
- Your world (seed, block edits and position) saves to the browser's localStorage.

## Folders

- `notes/`, `tools/`, `reconstructed/`: workspace for design notes and helper scripts.
