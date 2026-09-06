# Knowledge — what the student can actually do

One file per **topic per language**. This folder is the honest record. If a topic is not in
here with `status: confirmed`, the student does not know it yet — no matter how many times
it was explained.

## File naming

`knowledge/<language>/<stage>-<topic-slug>.md`

Examples: `python/1-for-loops.md`, `java/5-linked-list.md`, `cpp/7-bfs.md`

## Status ladder

| Status | Meaning |
|---|---|
| `learning` | introduced, in progress. This is the frontier. |
| `shaky` | passed once, failed a later review. Needs another pass. |
| `confirmed` | passed the 3-Way Check **and** at least one spaced review. |

## The 3-Way Check — required for `confirmed`

All three, in one session, unaided:

1. **Explain** — describes it in their own words, no jargon parroting
2. **Build** — writes working code using it from a **blank file**
3. **Debug** — finds and fixes the bug in a broken version you supply

Record the evidence in the file. "We covered it" is not evidence.

## Spaced review

`next_review` ladder: **+1d -> +3d -> +7d -> +21d -> +60d -> done**

- Pass a review: advance one rung, set the new `next_review`, log it.
- Fail a review: status drops to `shaky`, ladder resets to `+1d`. Two fails -> open a
  struggle file.

At the start of every session, check this folder for reviews due today or overdue.

## Carried-over concepts

When a confirmed concept reappears in a new language, set `carried_from: <language>` and
teach only the syntax delta. The Explain check is waived; **Build and Debug still apply**
in the new language.

Copy `_template.md` to start a file.
