# Still cooking — Stephen Curry career lab

Static, dependency-free career dashboard with linked season selection, three-point volume/accuracy scatterplot, scoring composition, age curve (per game or per 36 minutes), and season comparisons.

Open `index.html`, or serve this directory with `python3 -m http.server 8765`.

## Data

`curry.csv` is the supplied Basketball Reference per-game export. `data.js` contains its 17 season rows (career aggregate excluded). The CSV has an extra quoted wrapper around each row; parse that wrapper before parsing the comma-separated fields. Update both files when refreshing the data.

Basketball Reference profile checked September 22, 2026: https://www.basketball-reference.com/players/c/curryst01.html

- Regular season only; static snapshot, no live feed.
- 2019–20 (five games) is retained in source data but excluded from all charts and selectors. The age curve breaks across that missing season. 2011–12: 26 games.
- The shooting scatterplot uses unconnected dots; accuracy axis spans 36–48%.
- Scoring composition uses rounded per-game makes × shot value, so totals can differ slightly from reported PPG.
- Per-36 scoring uses rounded PPG × 36 / minutes per game. No pace adjustment.
- Three-point attempt share = 3PA / FGA.

## Publish

GitHub Pages serves `main` at the repository root. Push changes to deploy.

https://johnbang-hs.github.io/steph-curry-is-he-playing-well/
