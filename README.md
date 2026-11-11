# makefun-tiny-chess

`main.py` (4,088 bytes) is a ChatGPT optimization of the engine in commit `02c20ee`, from https://chatgpt.com/c/6af4731a-0760-83ea-925e-e1aec4444c60. That optimization was not written by the agent that opened this PR. The earlier 4,082-byte engine is still in that commit.

Checked from the unpacked source and local runs: a fixed 100,000-node search (no clock, no randomness), principal variation search, one-ply late-move reductions, repetition and fifty-move handling, a bishop-pair bonus, and a draw score for insufficient material. Python standard library only.

`grade-local` was not run here (no Docker). On one matched practice set against depth-2, depth-3, and depth-4, this file won all 6 games. The previous engine won 4 and drew 2.
