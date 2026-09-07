---
topic: Off-by-one in loop bounds
slug: off-by-one
language: python
stage: 1
opened: 2026-09-03
status: open
resolved: none
clean_successes: 1
related_knowledge: knowledge/python/1-for-loops.md
---

> EXAMPLE FILE — shows the expected shape. Delete once real entries exist.

## Symptom

Writes `range(1, n)` when the problem needs 1..n inclusive, and `range(len(a))` vs
`range(len(a) - 1)` gets picked by guessing rather than reasoning. Happened in the sum
exercise, the times table, and again in the list-reverse exercise.

## Suspected root cause

Not really about `range`. The student is not tracing the **last** iteration before running
the code. Root cause is likely a missing habit: hand-tracing boundary cases.

## Attempts

| # | Date | Approach tried | What happened |
|---|---|---|---|
| 1 | 2026-09-03 | restated the rule "stop is exclusive" | worked that day, gone next session |
| 2 | 2026-09-05 | had them write out the first and last value on paper before coding | correct on the first try, no hints |

## Clean successes

| # | Date | Task | Unaided? |
|---|---|---|---|
| 1 | 2026-09-05 | times table 1-12 inclusive | yes |

## Resolution

<pending — needs 2 more clean successes in a later session>
