# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Adesudu/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Adesudu/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original chess engine in at most 4,096 bytes of Python, written for make.fun's tiny-chess-01 bounty. It plays the house gauntlet through the env: 8 games against alpha-beta engines from depth-2 to 2M nodes, rated by Elo against their anchors.

The engine (`main.py`, packed from the readable `engine_src.py` with the kit's `makefun compress`) is a 0x88 board with negamax alpha-beta search, quiescence on captures, a transposition table, MVV-LVA + killer move ordering, piece-square evaluation, and iterative deepening on a fixed node budget — fully deterministic, no clock, no randomness.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=qq4pkark&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
