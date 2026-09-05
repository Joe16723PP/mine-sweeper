# Minesweeper

A single-file Minesweeper game in `index.html`. No build step, no dependencies — open the file or serve the folder.

The first click is always safe. Clear every safe square without hitting a mine.

## Features

- **Easy / Medium / Hard** — 9×9 (10 mines), 12×12 (24), 14×14 (40)
- **Classic or Race** — Race counts down (90 / 150 / 210 seconds)
- **English and Thai** — language choice is saved
- **Light and dark theme** — follows the system on the first visit, then remembers your pick
- **Hints** — up to 3 guaranteed moves per game
- **Score** — shown on the game-over modal, with round stats and a scoring guide below the board

## How to play

- Click a square to reveal it. Right-click, or use **Flag**, to mark a mine.
- Click a number when the flags around it match that number to clear the rest.
- The face button starts a new game.

## Scoring

The score appears only when the game ends.

| Action | Points |
| --- | --- |
| Cleared safe square | +10 |
| Correct flag | +20 |
| Wrong flag | −15 |
| Unused hint | +30 |
| Each second left on a clear | +8 |

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8777
```

Then visit [http://127.0.0.1:8777/](http://127.0.0.1:8777/).

## Deploy

This is a static site. Publish the repo root (the folder that contains `index.html`) with no build command.

Free hosts that work well:

- [GitHub Pages](https://pages.github.com/)
- [Cloudflare Pages](https://pages.cloudflare.com/)
- [Netlify](https://www.netlify.com/)
- [Vercel](https://vercel.com/)
