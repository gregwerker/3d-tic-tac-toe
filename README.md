# 3D Tic-Tac-Toe

Four in a row on a 4×4×4 cube you can rotate. Play the computer on Easy, Medium or Hard, in one of four colour themes.

**Play it:** https://gregwerker.github.io/3d-tic-tac-toe/

## How it works

- Everything is in `index.html`: the page, the styles and the JavaScript. It runs entirely in the player's browser. GitHub Pages just serves the file.
- The 3D view uses [three.js](https://threejs.org/) (loaded from a CDN).
- The board has 64 cells and 76 winning lines (rows, columns, verticals, and diagonals in every plane, plus the 4 corner-to-corner diagonals).
- **Computer player:**
  - *Easy* sometimes misses wins and blocks.
  - *Medium* always wins or blocks when it can, and otherwise picks among its top few moves.
  - *Hard* also looks for forced wins (a chain of threats you must keep blocking until it has two at once), defends against yours, and avoids moves that let you set up a double threat.

Your theme, difficulty and score are remembered in your browser.
