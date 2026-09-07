# Curriculum

## How it works

- `roadmap.md` is the spine: Stages 0-9, **language-neutral**. A concept is defined once.
- `resources.md` maps free university courses (MIT, Harvard, Princeton, Berkeley, Stanford,
  CMU) and practice sites onto those stages. Reinforcement only — never a substitute for
  the student writing code.
- `<lang>/README.md` holds the syntax, tooling, and gotchas for one language, plus how the
  roadmap stages map onto it.
- A stage is finished when its **Gate** passes: the student completes the gate task alone,
  from a blank file, with no hints.

## Order of operations for a new topic

1. Concept, in plain English, with an analogy and a hand-traced example on paper.
2. Syntax in the student's current language.
3. Student writes it from a blank file.
4. Student debugs a broken version you supply.
5. Topic goes into `knowledge/<lang>/` with the right status (see `knowledge/README.md`).

## Multi-language

Concepts are learned once, syntax per language. When a known concept appears in a new
language, teach only the delta and the gotchas — do not re-teach the idea. Record the new
file with `carried_from:` in its frontmatter.

## Adding a language

1. `curriculum/<lang>/README.md` (copy the shape of `python/README.md`)
2. `knowledge/<lang>/` and `exercises/<lang>/`
3. Add it to `student/profile.md`
