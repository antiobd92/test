# Roadmap — Stage 0 to Stage 9

Language-neutral. Concepts live here once; syntax lives in `curriculum/<lang>/README.md`.

**Rule:** do not start a stage until the previous stage's **Gate** passes. The Gate is a
task the student completes alone, from a blank file, with no hints.

Rough pace for a high school student doing 3 sessions a week: Stages 0-3 in a term,
Stages 4-6 in the next, Stages 7-9 over the following year. Slower is fine. Skipping is not.

---

## Stage 0 — Setup and First Program

Get a working loop of: write code -> run it -> read the output or the error.

- Install the language toolchain and an editor; run a program from the terminal
- `print` / output, comments, saving and re-running a file
- Reading an error message: what line, what kind, what to do
- Terminal basics: `cd`, `ls`, running a file by path

**Gate:** from a blank file, write a program that prints three lines, deliberately break it,
read the error aloud, and fix it.

**Project:** a program that prints a small ASCII picture or a personalised greeting banner.

---

## Stage 1 — Core Programming

The imperative core. Every later stage assumes total fluency here.

- Variables, assignment, and the idea of a name pointing at a value
- Types: integer, float, string, boolean. Type errors and conversion
- Arithmetic, integer division, modulo (`%` is used constantly later — teach it properly)
- Input from the user; converting input to numbers
- Conditionals: `if` / `else if` / `else`, comparison and boolean operators
- Loops: `while`, `for`, counters, accumulators, `break` / `continue`
- Functions: parameters, return values, scope, why we split code up
- Tracing code by hand on paper (teach this early; it pays back forever)

**Gate:** write a number-guessing game with input validation and a replay loop, from blank.

**Project:** a text calculator, a quiz game, or a unit converter with a menu.

---

## Stage 2 — Collections and Strings

- Arrays / lists: index, length, iterate, append, remove, off-by-one errors
- Strings as sequences: slicing, searching, splitting, joining, building up
- 2D grids: nested loops, row/column, printing a grid
- Key-value maps (dict / HashMap / map): lookup, insert, iterate
- Sets: membership and dedupe
- Choosing the right container for a job
- File reading and writing (line by line)

**Gate:** read a file of words and report the 5 most frequent, from blank.

**Project:** a gradebook, a text-adventure map, or tic-tac-toe on a 2D grid.

---

## Stage 3 — Problem Solving and Craft

The stage most courses skip. Do not skip it.

- Decomposition: turning a vague problem into named functions
- Reading a problem statement: inputs, outputs, constraints, edge cases
- Debugging on purpose: print-tracing, then the real debugger, breakpoints, stepping
- Writing test cases before the code; the empty / one-element / huge cases
- Naming, small functions, avoiding copy-paste
- Version control basics: `git init`, `add`, `commit`, reading `git log`

**Gate:** given a buggy 60-line program they have never seen, find and fix three bugs and
explain each one.

**Project:** take an earlier project, add tests, split it into functions, commit the history.

---

## Stage 4 — Complexity, Searching and Sorting

Where "programming" becomes "computer science".

- Counting operations; growth rates; Big-O notation (O(1), O(log n), O(n), O(n log n), O(n^2))
- Best / average / worst case; space complexity
- Linear search; binary search on a sorted array (and its off-by-one traps)
- Quadratic sorts by hand: selection, insertion, bubble — trace them on paper
- Merge sort and quicksort: divide and conquer, recursion tree, why n log n
- Stability, in-place, and using the language's built-in sort with a custom key/comparator

**Gate:** implement binary search and insertion sort from blank, then state and justify the
Big-O of each.

**Project:** a benchmark harness that times their sorts against the built-in one on growing
inputs and plots or prints the curve.

---

## Stage 5 — Linear Data Structures

Build each one from scratch first, *then* use the library version.

- Abstract data type vs implementation (the interface is the promise, the code is the how)
- Dynamic arrays: how append is amortised O(1)
- Stack: push/pop, call stack, bracket matching, undo
- Queue and deque: BFS ordering, sliding windows, ring buffers
- Singly and doubly linked lists: nodes, pointers/references, insert, delete, reverse
- Hash tables: hash function, buckets, collisions, why lookup is ~O(1)
- Two pointers and the sliding window pattern

**Gate:** implement a stack and a linked list from blank, including `reverse`, and explain
when a linked list beats an array.

**Project:** a browser-history simulator (back/forward with two stacks) or an LRU cache.

---

## Stage 6 — Recursion and Trees

- Recursion: base case, recursive case, the call stack, stack overflow
- Recursion vs iteration; converting between them
- Classic recursions: factorial, Fibonacci, sum of list, string reversal, Towers of Hanoi
- Memoisation (the door into dynamic programming)
- Backtracking: N-Queens, permutations, subsets, maze solving
- Binary trees: nodes, height, depth, leaves
- Traversals: preorder, inorder, postorder, level-order (BFS with a queue)
- Binary search trees: insert, search, delete; why balance matters (AVL / red-black at
  concept level only)
- Heaps and priority queues; heapsort
- Tries for prefix problems

**Gate:** from blank, write a BST with insert and search plus all four traversals, and solve
one backtracking problem.

**Project:** an autocomplete over a word list (trie), or an expression evaluator (tree).

---

## Stage 7 — Graphs

- Modelling problems as graphs: vertices, edges, directed, weighted
- Representations: adjacency list vs adjacency matrix, and the trade-off
- BFS: shortest path in an unweighted graph, level order, flood fill
- DFS: recursive and stack-based; connected components; cycle detection
- Topological sort and dependency ordering
- Dijkstra's algorithm with a priority queue
- Union-Find (disjoint set) with path compression
- Minimum spanning trees: Kruskal and Prim
- Grid problems as graphs (islands, shortest path in a maze)

**Gate:** from blank, BFS shortest path on a grid, and explain when to reach for BFS vs DFS
vs Dijkstra.

**Project:** a route finder on a real map or campus grid, or a course-prerequisite planner.

---

## Stage 8 — Advanced Algorithms

- Greedy algorithms: interval scheduling, coin change — and how to know greed fails
- Dynamic programming: state, transition, base case
  - 1D: climbing stairs, house robber, longest increasing subsequence
  - 2D: grid paths, edit distance, longest common subsequence, 0/1 knapsack
  - Top-down memoisation vs bottom-up tabulation; space optimisation
- Bit manipulation: masks, shifts, XOR tricks, subset enumeration
- Advanced two pointers, prefix sums, difference arrays
- String algorithms: KMP, rolling hash, palindrome techniques
- Range queries: Fenwick tree (BIT) and segment tree
- Amortised analysis; picking the right structure under a constraint

**Gate:** from blank, solve a 2D DP problem and explain the state and transition in words
before writing any code.

**Project:** a solver for a real puzzle (Sudoku, word ladder, scheduling) with a written
complexity analysis.

---

## Stage 9 — Practice, Contests, Real Software

- Pattern recognition: mapping a new problem onto a known technique
- Timed practice: LeetCode easy -> medium -> hard; Codeforces Div 3/2; USACO Bronze -> Silver
- Reading and writing an editorial: explaining a solution clearly is its own skill
- Contest technique: reading fast, brute force first, testing edge cases, when to move on
- Beyond algorithms: an API, a database, a small web or game project, a real repo with
  branches, issues, and a README

**Gate:** solve an unseen medium problem in 45 minutes and explain the approach out loud
before coding.

**Project:** something the student actually wants to exist, shipped and shown to a person.

---

## Progress Table

Update the status as gates pass. Keep dates absolute.

| Stage | Name | Status | Gate passed |
|---|---|---|---|
| 0 | Setup and First Program | not started | |
| 1 | Core Programming | not started | |
| 2 | Collections and Strings | not started | |
| 3 | Problem Solving and Craft | not started | |
| 4 | Complexity, Searching, Sorting | not started | |
| 5 | Linear Data Structures | not started | |
| 6 | Recursion and Trees | not started | |
| 7 | Graphs | not started | |
| 8 | Advanced Algorithms | not started | |
| 9 | Practice and Contests | not started | |
