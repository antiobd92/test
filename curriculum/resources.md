# Outside Resources — Free University Courses and Tools

Mapped to the stages in `roadmap.md`.

**Read the rules in `claude.md` -> "University Courses and Outside Resources" before using
any of this.** The short version: code first, lecture second; one specific piece at a time;
never a whole syllabus; verify the link resolves before sending it. Course numbers, URLs,
and hosting move around — if a link is dead, tell the student how to search for it instead
of guessing a new one.

---

## Everyday tools — reach for these first

These beat lectures for a high school student, every time.

| Tool | What it is | Use it for |
|---|---|---|
| **Python Tutor** — <https://pythontutor.com> | steps through code line by line, drawing variables and the call stack | Stages 1-6. The single best tool here. Essential for recursion and for linked lists. Supports Python, Java, and C++. |
| **VisuAlgo** — <https://visualgo.net> | animated data structures and algorithms | Stages 4-8. Watch a BST rebalance or Dijkstra expand before coding it. |
| **USF Algorithm Visualizations** — <https://www.cs.usfca.edu/~galles/visualization/Algorithms.html> | plain, fast visualisations | same as above; simpler and quicker to load |
| **Exercism** — <https://exercism.org> | small exercises with human mentoring, free | Stages 1-3, for volume of practice |

---

## By stage

| Stage | Best fit | Why this one |
|---|---|---|
| 0-1 Setup, core programming | **Harvard CS50P** (Python) or **MIT 6.100A** | gentle, assumes nothing |
| 1-2 Core + collections | **CMU 15-112** | enormous, well-graded exercise bank |
| 2-3 Problem solving, craft | **Harvard CS50x** | the C weeks teach what a variable really is; famously well produced |
| 3-4 Abstraction, complexity | **Berkeley CS61A** | teaches *thinking*, not syntax |
| 4-7 Sorting, structures, graphs | **Princeton Algorithms I & II** | the best fit for a motivated high school student |
| 5-7 Data structures in Java | **Berkeley CS61B** | build every structure yourself; ideal alongside the Java track |
| 4-8 Algorithms, rigorous | **MIT 6.006** | the real thing. More mathematics — reach for it when the student is ready |
| 8-9 Advanced, contests | **USACO Guide** + **Competitive Programmer's Handbook** | stage-by-stage contest training |

---

## The courses

### MIT — OpenCourseWare (free, openly licensed) — <https://ocw.mit.edu>

- **6.100A / 6.0001 Introduction to Computer Science and Programming in Python** — Stages
  1-2. Lecture videos, assignments, and solutions. A solid first course.
- **6.006 Introduction to Algorithms** — Stages 4-8. Sorting, hashing, trees, graphs, DP.
  The Spring 2020 version (Ku, Demaine, Solomon) has excellent recitation notes. *Level
  warning:* assumes comfort with proofs and summations — best after Stage 4 is finished.
- **6.046J Design and Analysis of Algorithms** — beyond Stage 8. Park it for later.
- **6.042J Mathematics for Computer Science** — the discrete maths (induction, counting,
  graphs, proofs) that makes 6.006 readable. Useful in small pieces from Stage 4.
- **MIT 6.851 Advanced Data Structures** — genuinely advanced. Only for a student who has
  finished Stage 8 and wants more.

### Harvard — <https://cs50.harvard.edu>

- **CS50x — Introduction to Computer Science** — Stages 0-3. Free on the site and on edX
  (audit free; the certificate is paid — say so before recommending). Starts in Scratch,
  moves to C, ends in Python and SQL. The C section is worth doing precisely because it is
  uncomfortable: arrays, pointers, and memory become concrete.
- **CS50P — Introduction to Programming with Python** — Stages 0-2. Gentler than CS50x and
  a better first stop for a student who only wants Python.

### Princeton — <https://algs4.cs.princeton.edu> and Coursera

- **Algorithms, Part I and Part II** (Sedgewick & Wayne) — Stages 4-7. Free to audit on
  Coursera. Java-based, superb visualisations, exactly the right level for a strong high
  school student. **The best single algorithms resource for this roadmap.** Pairs perfectly
  with the Java track.
- The companion site has all the code and exercises free, no sign-up.

### UC Berkeley

- **CS61A — Structure and Interpretation of Computer Programs** — <https://cs61a.org>.
  Stages 3-4. Python. Recursion, abstraction, higher-order functions. Changes how a student
  thinks. Full textbook free at <https://composingprograms.com>.
- **CS61B — Data Structures** — <https://datastructur.es>. Stages 5-7. Java. Students build
  lists, maps, trees, heaps, and graphs from scratch. Labs and autograded specs are public.

### Stanford

- **CS106B Programming Abstractions** — Stages 5-6, C++. Recursion and data structures.
- **CS106L Standard C++ Programming** — <https://web.stanford.edu/class/cs106l/>. For the
  C++ track once basics are solid; teaches modern C++ properly.
- **CS161 Design and Analysis of Algorithms** — Stage 8 and beyond. Proof-heavy.

### Carnegie Mellon

- **15-112 Fundamentals of Programming** — <https://www.cs.cmu.edu/~112/>. Stages 1-2,
  Python. Notes, exercises, and term projects all public. The exercise volume is the draw.

### Other open material

- **Teach Yourself CS** — <https://teachyourselfcs.com>. A curated map of the whole CS
  curriculum with book and course picks. Good for a student asking "what comes after this?"
- **OpenDSA** — free interactive data structures textbook with embedded visualisations.
- **Khan Academy** — for the maths gaps (logarithms, summations, combinatorics) that block
  Stage 4 and Stage 8.

---

## Practice — Stages 4 to 9

| Site | Use |
|---|---|
| **LeetCode** — <https://leetcode.com> | pattern practice from Stage 5 on. Easy -> Medium. Do **not** read the solution tab; that breaks The No-Answer Rule from the other side. |
| **CSES Problem Set** — <https://cses.fi/problemset/> | 300 problems ordered by topic, near-perfect coverage of Stages 5-8 |
| **USACO Guide** — <https://usaco.guide> | free, structured Bronze -> Platinum path. The best contest curriculum available |
| **Codeforces** — <https://codeforces.com> | live contests from Stage 8. Div. 3 first |
| **Project Euler** — <https://projecteuler.net> | maths-flavoured problems; good for a student who likes numbers |
| **Advent of Code** — <https://adventofcode.com> | every December, wide difficulty range, very motivating |

## Books

- **Competitive Programmer's Handbook** (Antti Laaksonen) — free PDF at
  <https://cses.fi/book/book.pdf>. Stages 5-9. Concise and genuinely readable.
- **Grokking Algorithms** (Aditya Bhargava) — paid, illustrated, aimed squarely at people
  who find CLRS impenetrable. The best book for this student. Mention the cost.
- **Introduction to Algorithms** (CLRS) — the reference. Too dense for a high school
  student to read cover to cover. Use it to look one thing up, never as a course.

---

## Watch out for

- **Tutorial hell.** A student who has watched forty hours of lectures and written four
  hundred lines of code is going backwards. Ratio should be the other way around.
- **Course-hopping.** Starting five courses is how people quit. One at a time, one piece at
  a time.
- **Level mismatch.** MIT 6.006 in week two will convince a bright student they are stupid.
  Pace the recommendations to the roadmap stage.
- **Solution tabs and answer videos.** These are the exact thing The No-Answer Rule exists
  to prevent. Point the student at the *hints* on a problem, never the editorial, until
  after they have solved it.
