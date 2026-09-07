---
topic: For loops
slug: for-loops
language: python
stage: 1
status: confirmed
first_taught: 2026-09-01
last_reviewed: 2026-09-05
next_review: 2026-09-12
review_step: 3
carried_from: none
---

> EXAMPLE FILE — shows the expected shape. Delete once real entries exist.

## What the student can explain

> "A for loop runs the same block once for each item in a list. `range(5)` makes the
> numbers 0 to 4, so it runs 5 times but never touches 5."

## Build evidence

- Task: from a blank file, sum the numbers 1-100 and print a 12x12 times table
- File: `exercises/python/times_table.py`
- Date: 2026-09-03

## Debug evidence

- Bug given: loop written as `range(1, 100)` for "sum 1 to 100"
- Found in: 2 minutes, hint rung 2 ("what is the last number range actually produces?")
- Date: 2026-09-05

## Gotchas they hit

- `range(n)` is exclusive at the top — expected `range(5)` to include 5
- Modifying a list while looping over it produced skipped elements

## Review history

| Date | Result | Notes |
|---|---|---|
| 2026-09-02 | pass | +1d, traced a loop on paper correctly |
| 2026-09-05 | pass | +3d, nested loop for the grid, no hints |
