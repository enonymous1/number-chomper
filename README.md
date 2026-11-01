# Number Chomper

A playable, single-file web game. Move the Chomper around a 6×5 number grid and chomp only the numbers that match the rule at the top. Clear the board to advance to the next level.

No build step, no backend, no dependencies to install. Just open `index.html` in a browser.

## How to play

- **Goal:** chomp every number that matches the current rule, and nothing else.
- **Rules rotate** between Multiples, Factors, Primes, Greater/Less Than, and Even/Odd.
- **Lives:** you start with 3 Chompers. Chomping a wrong number, or letting a Gobbler catch you, costs one.
- **Levels:** clearing a board advances a level. Higher levels add more, faster Gobblers and larger numbers.

## Gobblers

- **Wanderer** — wanders the board, but is still hungry.
- **Scribbler** — rewrites numbers it steps on.
- **Hunter** — hunts you down.

## Controls

- Arrow keys / WASD — move
- Space — chomp
- P — pause (also pauses automatically when the tab hides)
- Touch — swipe the board to move, tap to chomp, or use the on-screen D-pad and CHOMP button

## Scoring

- +10 per correct chomp
- Streaks build a bonus
- Clearing a level pays 100 + 10 per level

## Sound

Synthesized in-browser sound effects, with a mute toggle. No audio files are needed.

## High scores

The top-8 high score table is kept for the current browser session only. Scores reset when the page is closed — this is a static page with no server or account storage.

## Run it

Open `index.html` directly, or serve the folder:

```sh
python3 -m http.server 8000
```

then open http://localhost:8000/

## Publish it with GitHub Pages

1. Push this repo to GitHub.
2. Settings → Pages → Build and deployment → Source: Deploy from a branch.
3. Branch: `main`, folder: `/ (root)`.
4. Save — the site will be served from `index.html`.

## License

MIT — see [LICENSE](LICENSE).
