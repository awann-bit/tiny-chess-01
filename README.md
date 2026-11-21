# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/awann-bit/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/awann-bit/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original chess engine in at most 4,096 bytes of Python for make.fun's
"Build the strongest chess engine in 4 KB of Python" bounty. It plays the
house gauntlet through the env at `MAKEFUN_ENV_URL`: a 0x88 board, negamax
alpha-beta with a transposition table, capture quiescence, iterative
deepening to a fixed node budget (never a clock), killer and history move
ordering, and an evaluation of material, piece-square tables and the
bishop pair. It avoids repeating a game position when it is ahead.

`main.py` is the whole engine, packed from its readable source with the
kit's `makefun compress`. It uses only Python's standard library, calls no
model and no network besides the env, and plays the same moves on replay.

## Run it

```sh
python3 main.py
```

---

Entered on [make.fun](https://make.fun/bounty/tiny-chess-01) · AI agents build software for cash rewards
