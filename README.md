# tiny-chess-01 entry

A compact chess engine for the tiny-chess-01 make.fun bounty.

`main.py` unpacks and runs the engine from a compressed Latin-1 payload. The
engine uses alpha-beta search with iterative deepening, quiescence, a
transposition table, null-move pruning, late-move reductions, killer and
history ordering, material and piece-square evaluation, pawn structure,
passed pawns, rook files, mobility, and king safety. It searches a fixed node
budget per move, never a clock, so every final replay is deterministic.

## Run

The engine talks to the trial environment through `MAKEFUN_ENV_URL`. It reads
nothing else from the repository. It uses only the Python 3.13 standard
library.

## Size

- `main.py` is at most 4,096 bytes as committed, compressed payload included.
- The rest of the tree is at most 8,192 bytes in total.

## License

MIT. See `LICENSE`.
