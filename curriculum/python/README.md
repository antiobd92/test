# Python Track

**Best for:** a first language, and for thinking about algorithms without syntax noise.

## Setup (macOS)

Full setup rules live in `claude.md` -> Environment Setup. The student types every command.

```bash
brew install python@3.13                       # or the current stable
python3 --version                              # verify
which python3                                  # /opt/homebrew/bin/python3 on Apple Silicon
brew install --cask visual-studio-code         # editor, then add the Python extension
python3 hello.py                               # run
```

- Alternative to Homebrew: the official installer at
  <https://www.python.org/downloads/macos/> (includes IDLE, fine for a first week).
- Do not build on the `python3` that ships with macOS — that one belongs to the system.
- **Virtual environments** arrive at Stage 3, when the first third-party package does:
  `python3 -m venv .venv` then `source .venv/bin/activate`, then `pip install ...`.
  Before that they are noise.

## Courses that fit

CS50P, MIT 6.100A, CMU 15-112, Berkeley CS61A. See `curriculum/resources.md` for what to
use at which stage.

## Tools introduced by stage

| Stage | Tool |
|---|---|
| 0 | terminal, `python3 file.py` |
| 3 | `pytest`, VS Code debugger, `git` |
| 4 | `timeit` for benchmarks |
| 9 | virtual environments, `pip`, a real project layout |

## Stage mapping and Python specifics

- **Stage 1** — no braces, indentation *is* the block. f-strings for output. `input()`
  always returns a string; `int(input())` is the fix.
- **Stage 2** — lists, slices, `dict`, `set`, tuples, comprehensions (introduce only after
  plain loops are fluent). List methods: `append`, `pop`, `sort`, `sorted`.
- **Stage 3** — `pytest`, `assert`, type hints as documentation.
- **Stage 4** — `sorted(key=...)`, `list.sort()`, `bisect` after hand-writing binary search.
- **Stage 5** — `collections.deque` for queues, `dict` as the hash table, build the linked
  list with a small `Node` class.
- **Stage 6** — `sys.setrecursionlimit`, `functools.lru_cache` for memoisation, `heapq`.
- **Stage 7** — adjacency list as `dict[node, list[node]]`, `heapq` for Dijkstra.
- **Stage 8** — 2D DP tables as list-of-lists, `int` is arbitrary precision (a real
  advantage here).

## Gotchas to teach explicitly

- Mutable default arguments (`def f(x=[])`) — a classic and confusing bug
- `is` vs `==`
- Integer division `//` vs `/`
- Aliasing: `b = a` copies the reference, not the list. `a[:]` or `copy` to duplicate
- Shallow vs deep copy for 2D grids: `[[0]*n]*m` is a trap; use a comprehension
- Late-binding closures in loops
