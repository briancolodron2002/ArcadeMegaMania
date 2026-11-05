# ArcadeMegaMania

A complete fixed-screen space shooter (shmup) game inspired by the classic **Megamania** for the Atari, built in a **single HTML file** using HTML5 Canvas and vanilla JavaScript — no libraries, no external assets.

## Play

Just open `index.html` in any modern browser (Chrome or Edge recommended).

## Features

- **5 unique enemy types** cycling across waves:
  - Hamburgers
  - Cookies
  - Irons
  - Bow-ties
  - Diamonds

- **Player mechanics**: smooth horizontal movement, up to 2 simultaneous bullets, 3 lives, invulnerability flash on hit

- **Energy bar**: drains completely in ~30 seconds — destroy all enemies before it runs out or lose a life

- **Enemy AI**: zigzag descent pattern, enemies shoot back (1 bullet at a time, aimed loosely at player)

- **AABB collision detection** for all projectiles and enemy bodies

- **Increasing difficulty**: speed scales with each wave

- **Scoring**: 100+ points per enemy (scales with wave), bonus on wave clear

- **8-bit pixel art** sprites drawn entirely via code matrices — no image files

- **Pixel font** rendered via code — no external fonts

- **320x240 internal resolution** scaled to the largest integer multiple that fits the window, centered, with black bars — `image-rendering: pixelated`

- **Web Audio API** sound effects (no audio files):
  - Laser shoot (square wave, descending frequency)
  - Enemy explosion (white noise burst + bass thump)
  - Player death (sawtooth decay)

- **Controls**:
  - Keyboard: Arrow keys or A/D to move, Space to fire, Enter/Space to start/restart
  - Mobile: on-screen buttons (left, right, fire) + drag on canvas

## Screenshots

> Open the game and play — all visuals are rendered dynamically in pure JavaScript.

## Tech Stack

| Layer    | Technology          |
|----------|---------------------|
| Structure | HTML5              |
| Rendering | Canvas 2D API      |
| Logic    | Vanilla JavaScript  |
| Audio    | Web Audio API       |
| Styling  | Vanilla CSS         |

## License

MIT
