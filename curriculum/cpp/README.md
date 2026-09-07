# C++ Track

**Best for:** competitive programming (USACO, Codeforces, IOI) and understanding memory.

Do not make C++ a first language unless the student is aiming at contests.

## Setup (macOS)

Full setup rules live in `claude.md` -> Environment Setup. The student types every command.

```bash
xcode-select --install                  # Apple's clang, reachable as g++. Enough for Stages 0-8
g++ --version                           # will say "Apple clang" — that is expected
brew install --cask visual-studio-code  # then add the C/C++ extension

# build and run, with the sanitizers on — they catch the bugs beginners actually write
g++ -std=c++17 -O2 -Wall -fsanitize=address,undefined main.cpp -o main && ./main
```

- **Real GNU GCC** (what most contest judges run): `brew install gcc`, then call the
  versioned binary, e.g. `g++-14`. Only worth it once the student enters contests.
- **There is no standard C++ package manager.** Say so plainly. The standard library covers
  every stage in this roadmap. (`vcpkg` and Conan exist; the student does not need them.)

## Courses that fit

Stanford CS106B for abstractions, CS106L for modern C++, and the USACO Guide plus the
Competitive Programmer's Handbook for contests. See `curriculum/resources.md`.

## Tools introduced by stage

| Stage | Tool |
|---|---|
| 0 | `g++`, a one-line build-and-run command |
| 3 | `gdb` or `lldb`, `-fsanitize=address,undefined`, `git` |
| 4 | `<chrono>` for timing |
| 9 | contest template, fast I/O, stress testing against a brute force |

## Stage mapping and C++ specifics

- **Stage 1** — `#include <iostream>`, `cin` / `cout`, explicit types, `int main()`.
- **Stage 2** — `std::vector` (teach this, not raw arrays), `std::string`, `std::map`,
  `std::unordered_map`, `std::set`, 2D as `vector<vector<int>>`.
- **Stage 3** — sanitizers, `assert`, reading a segfault, a debugger.
- **Stage 4** — `std::sort` with a lambda comparator, `lower_bound` after hand-writing
  binary search, `-O2` and why timings change.
- **Stage 5** — `stack`, `queue`, `deque`, `list`; pointers and references; a hand-written
  linked list is where pointers finally click.
- **Stage 6** — recursion depth and the stack, `priority_queue`, structs.
- **Stage 7** — `vector<vector<int>>` adjacency lists, `priority_queue` with `greater<>`.
- **Stage 8** — bit tricks (`__builtin_popcount`), `long long` overflow, segment trees and
  Fenwick trees, contest-speed I/O (`ios::sync_with_stdio(false)`).

## Gotchas to teach explicitly

- Undefined behaviour is real: out-of-bounds may "work" and then not
- `int` overflow at ~2.1 billion; use `long long`
- Uninitialised variables hold garbage
- Pass by value vs reference (`vector<int>` copies are expensive)
- Iterator invalidation when modifying a container mid-loop
- Integer division truncates toward zero for negatives
