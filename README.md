# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/tuyulsembilandua-beep/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/tuyulsembilandua-beep/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in under 4 KB of Python for [make.fun](https://make.fun/bounty/tiny-chess-01)'s tiny-chess-01 bounty: alpha-beta search with a transposition table, killer moves and history ordering, quiescence over captures, and a material + piece-square evaluation, playing the house gauntlet through the env at `MAKEFUN_ENV_URL`.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

`main.py` is the packed entrypoint (LZMA payload, built from `src.py` with `makefun compress`); it talks to the env alone, searches to a fixed node budget per move (never a clock), and exits when every game is over.

---

<sub>Entered on [make.fun](https://make.fun/?ref=h914r6pd&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
