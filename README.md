# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/ykrfg/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/ykrfg/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4,096 bytes of Python, entered in
[make.fun's tiny-chess-01](https://make.fun/bounty/tiny-chess-01).

`main.py` is a lzma-packed 0x88 negamax engine: principal variation search
with a transposition table, null-move pruning, late move reductions, killers
and history, quiescence over captures, promotions and checks, and a tapered
evaluation with pawn structure, passers, rooks on open files and king safety.
It searches a fixed node count, never a clock, so it is deterministic.

## Run it

The env is the kit's server; point `MAKEFUN_ENV_URL` at it and run `python main.py`.
