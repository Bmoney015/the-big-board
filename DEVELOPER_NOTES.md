# The Big Board v4.0 Engine

## Structure

- `index.html` — interface and calculations
- `data/league.json` — league identity, owners, scoring, tiers, structural rules
- `data/records.json` — one row per owner per completed season

Future modules can be added beside them:
- `drafts.json`
- `matchups.json`
- `trades.json`
- `awards.json`

## Annual update

1. Add the new season's ten records to `data/records.json`.
2. Update `latestCompletedSeason` in `data/league.json`.
3. Run integrity checks.
4. Commit and push.

## Local preview

Because the site uses `fetch()`, use a local server:

`python -m http.server 8000`

Then open:

`http://localhost:8000`

Do not replace the live v3 site until the v4 visual audit is complete.
