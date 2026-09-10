# Snapshot pack 2026-08-31 → 2026-09-09

One Excel + one JSON per calendar day the pipeline was actually launched.
Newest dated folder that day is the source. Missing layers are omitted, not invented.

**Glossary / formulas:** `GLOSSARY_AND_FORMULAS.docx` — Word companion covering constants, identities, mix scores, projected-total construction, field glossary, physics vs chosen scales, and which layers existed on which day.

| Date | Contract | Games | Projected total | Ump/C/pen | Lineups | Mix/physics |
|---|---|---|---|---|---|---|
| 2026-08-31 | 70.0.0 | 12 | no | no | no | yes |
| 2026-09-01 | 80.0.0 | 15 | no | no | no | yes |
| 2026-09-02 | 80.0.0 | 15 | no | no | yes | yes |
| 2026-09-03 | 80.0.0 | 9 | no | no | yes | yes |
| 2026-09-04 | 80.0.0 | 16 | no | no | yes | yes |
| 2026-09-05 | 80.0.0 | 15 | no | no | yes | yes |
| 2026-09-06 | — | — | no run | no run | no run | no run |
| 2026-09-07 | 80.0.0 | 11 | no | no | yes | yes |
| 2026-09-08 | 90.0.0 | 15 | yes | yes | yes | yes |
| 2026-09-09 | 90.0.0 | 15 | yes | yes | yes | yes |

## Excel
- `COVERAGE` tab: what this run actually had.
- `Slate` tab: one row per matchup.
- One tab per game: scoreboard, air, carry-if-hit, each arm (schedule/acclimation + season profile + per-pitch mix from the dashboard cards), nines, HP/catchers, bullpen, plugged recipe.

## JSON
Condensed transfer object: environment, projection, market, umpire, catchers, bullpen, lineups, pitchers (mix + profile + per-pitch break/speed/command/pickup/rain/gust + Statcast deltas). No glossary, no artifact hashes.

## Known gaps
- 2026-09-06: no collect.
- Through 2026-09-07: no generative `projected_total`, no Covers HP, no Savant framing, no bullpen intel, no DK/SAO overlay. Mix + physics + (from 9/2) lineups are present.
- 2026-08-31 (V70): no lineups section.
- 2026-09-08 onward (V90): full stack.
