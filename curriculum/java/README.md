# Java Track

**Best for:** AP CS A, school courses, and learning static types and OOP properly.

## Setup (macOS)

Full setup rules live in `claude.md` -> Environment Setup. The student types every command.

**Which JDK?** Two doors, same language:

- **Eclipse Temurin (OpenJDK) — the default.** Free, open source, no licence question.
  `brew install --cask temurin@21`, or download from <https://adoptium.net>.
- **Oracle JDK** — Oracle's build, from
  <https://www.oracle.com/java/technologies/downloads/>. Free for personal and development
  use under Oracle's current terms, but those terms have changed before. Temurin avoids the
  question; pick Oracle only if the school requires it.

Use **JDK 21** (long-term support) unless the school pins another version.

```bash
brew install --cask temurin@21
java --version                          # verify
/usr/libexec/java_home -V               # list every installed JDK
export JAVA_HOME=$(/usr/libexec/java_home -v 21)

brew install --cask intellij-idea-ce    # free IntelliJ Community Edition
java Hello.java                         # run a single file, no compile step needed
```

- Maven and Gradle wait until Stage 9. `java File.java` carries the student through every
  data structure in this roadmap.

## Courses that fit

Princeton Algorithms I & II and Berkeley CS61B are both Java-based and map straight onto
Stages 4-7. See `curriculum/resources.md`.

## Tools introduced by stage

| Stage | Tool |
|---|---|
| 0 | JDK, IntelliJ, `java File.java` |
| 3 | JUnit 5, the IntelliJ debugger, `git` |
| 5 | the Collections framework |
| 9 | Maven or Gradle, a real project layout |

## Stage mapping and Java specifics

- **Stage 1** — `public static void main`, explicit types, `Scanner` for input, braces and
  semicolons, `System.out.println`.
- **Stage 2** — fixed-size arrays vs `ArrayList`; `String` is immutable, use
  `StringBuilder` in loops; `HashMap`, `HashSet`; 2D arrays `int[][]`.
- **Stage 3** — JUnit, exceptions and `try`/`catch`, reading a stack trace.
- **Stage 4** — `Arrays.sort`, `Collections.sort`, `Comparator`, `compareTo`.
- **Stage 5** — `Deque` / `ArrayDeque` for stacks and queues, `LinkedList`, a hand-written
  `Node` class; `interface` vs `class` lands naturally here (ADT vs implementation).
- **Stage 6** — recursion depth, `PriorityQueue`, generics `<T>`.
- **Stage 7** — `Map<Integer, List<Integer>>` adjacency lists, `PriorityQueue` for Dijkstra.
- **Stage 8** — `long` overflow, `int` is 32-bit, `BigInteger` when needed.
- **OOP** (classes, fields, constructors, `static`, inheritance, interfaces,
  encapsulation) is required for AP CS A. Teach it across Stages 3-5 as the data structures
  give it a reason to exist. Do not teach inheritance before the student has felt the need.

## Gotchas to teach explicitly

- `==` compares references for objects; use `.equals()` for `String`
- Integer division truncates; `int` overflow is silent
- Arrays have `.length`, `String` has `.length()`, lists have `.size()`
- `null` and the `NullPointerException`
- Autoboxing surprises with `Integer` caching
