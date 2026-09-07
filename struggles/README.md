# Struggles — where the student is stuck

A struggle file is a hypothesis about a gap, plus the evidence. It is not a report card.
Say "good, we found the gap" and mean it.

## Folders

- `open/` — active. Work on **at most 2 at a time**.
- `resolved/` — closed. Kept on purpose, for spotting patterns.

## File naming

`<language>-<topic-slug>.md` — e.g. `open/python-off-by-one.md`

## Open a file when any of these happen

- Hint rung 4 reached twice on the same concept
- A confirmed topic fails a spaced review twice
- The student says "I don't get it" about the same thing in two different sessions
- The same bug class appears three times (off-by-one, `==` vs `.equals`, aliasing)

## While it is open

- Start each session with one short question from an open struggle.
- Attack the **root**, not the symptom. Repeated trouble with recursion is often really
  trouble with the call stack, or with tracing code by hand.
- Change the approach between attempts. Repeating the same explanation louder is not a new
  attempt — try a drawing, a paper trace, a physical analogy, a smaller sub-problem.
- Log every attempt with what you tried and what happened.

## Close it

**3 clean successes across at least 2 different sessions.** Then:

1. Move the file to `resolved/` and fill in the resolution section.
2. Create or update the matching `knowledge/<lang>/` entry.
3. Note it in `student/session-log.md`.

## Too many open?

3+ open struggles means the pace is too fast. Stop new material. Back up a stage and
rebuild the foundation. This is a pacing signal, not the student's fault.

## Pattern review

Every ~6 sessions, read `resolved/` end to end. Look for a theme. A theme means an earlier
concept was never solid — go fix that.

Copy `_template.md` to start a file.
