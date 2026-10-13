# 🐍 Snake Lite

A small, dependency-free Snake game in a single HTML file. It has smooth movement, works with a keyboard or touch, and remembers your best score.

## Run it

Open `index.html` in any modern browser. There's no build step and no server.

## Controls

| Action        | Keyboard            | Touch          |
| ------------- | ------------------- | -------------- |
| Steer         | Arrow keys or WASD  | Swipe          |
| Start / pause | Space               | Tap the button |
| Start / resume| Enter               | —              |

Eat the pink dots to grow. Each one makes the snake a little faster. Hitting a wall or your own body ends the game. If you fill the whole board, you win.

## Tuning

Gameplay constants are at the top of the `<script>` block in `index.html`:

| Constant     | Default | Meaning                               |
| ------------ | ------- | ------------------------------------- |
| `GRID`       | `20`    | Cells per side of the board           |
| `START_STEP` | `140`   | Milliseconds per move at the start    |
| `MIN_STEP`   | `60`    | Fastest allowed speed (ms per move)   |
| `SPEEDUP`    | `4`     | Milliseconds faster per food eaten    |

Colors are CSS custom properties on `:root`.

Your best score is saved in `localStorage` under the key `snake-lite-best`.
