# Tiny Chess Engine — make.fun tiny-chess-01

Original 0x88 chess engine in a single `main.py` (<= 4096 bytes, lzma payload).

- Negamax + alpha-beta, quiescence with check evasions
- Transposition table, killer-move ordering, repetition-aware search
- Material + piece-square evaluation, bishop-pair bonus
- Fixed 50,000 nodes/move — fully deterministic, no clock, no model calls
- Python 3.13 standard library only; talks HTTP to the make.fun env

Local practice trials (kit env server): Elo ~1174 mean over 3 trials
(1364 / 1451 / 708), above the 1154 final-entry floor.
