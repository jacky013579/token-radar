# token-radar

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/jacky013579/token-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/jacky013579/token-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

Token Radar ranks every clean pre-token protocol in DefiLlama's snapshot by an implied value, and shows how to farm each one. The board covers all 40 watchlist protocols plus 138 clean pre-token protocols below the $50M floor — every one that passes the watchlist's own cleanliness rule, not a top-N cut. Implied value is an estimated fully-diluted value at launch, priced like the protocol's live peers: each category's multiple is the median market-cap/TVL of its live-token protocols, shrunk toward the global median and clamped, then adjusted for seven-day growth, age with no token, and chain breadth. Each row carries an eight-step farm plan with costs and times, derived from the protocol's own category, chains, TVL and age. Live-token protocols are set aside with their market caps shown — they price the board, they never join it.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input <snapshot.json|directory>
```

The program reads the sealed snapshot, writes the ranked board to `out/board.json`, the dashboard's data to `out/data.js`, copies `dashboard/` and `screenshots/` to `out/`, and writes `out/dossier.json` with the vendored make.fun library. Node 22 or later, standard library only. Open `out/dashboard/index.html` to use the radar: search, filter by category or chain, watchlist-only, sort by implied value / TVL / growth / age, and open any row for its model breakdown and farm plan.

---

<sub>Entered on [make.fun](https://make.fun/?ref=8tp2j03b&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
