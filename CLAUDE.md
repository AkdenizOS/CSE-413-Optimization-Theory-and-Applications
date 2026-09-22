# CSE 413 — Working Notes for AI Sessions

Course repository for Optimization Theory and Applications (Akdeniz University,
Computer Engineering, semester 7). Read [`course-info.md`](course-info.md) for
what the course covers and its [Resource Map](course-info.md#resource-map--which-source-covers-which-week)
section for which book covers which week. [`README.md`](README.md) has the layout.

## What this repo is for

Studying. The deliverables are understanding, working from-scratch implementations,
assignments, and a term project — not a production system.

## Conventions

- **Language:** English for everything committed — READMEs, notes, code, comments.
  Turkish appears only where the source is Turkish (syllabus quotes, glossary,
  Turkish reference books).
- **Week notes:** one file per week, `weeks/NN-topic-slug.md`, holding goals,
  reading, tasks, checklist and, below the shared plan, one
  `## Notes — <Name> (<term>)` section per person. Scratch code for that
  week goes in `code/week-NN/`.
- **Where other files go:** exam papers flat in `exams/`; someone's own assignments
  and project in `assignments/<term>-<person>/`; slides and handouts the instructor
  issued in a given term in `resources/<term>/`. A folder exists only once it holds
  two or more files.
- **Links:** plain Markdown links, never `[[wikilinks]]` — Markdown links show up in
  Obsidian's graph and backlinks *and* still work on GitHub. Book citations link to
  the exact page (`...pdf#page=N`); offsets are Boyd +14, Nocedal +19, Winston +16.
- **Shared code:** anything reused by two or more weeks moves to `src/optlib/`.
  One-off experiments stay in the week's `code/week-NN/`.
- **Every implementation is verified** against a reference solver (SciPy, CVXPY,
  PuLP/CBC, NetworkX, PyTorch). An unverified implementation is not done.
- **Stochastic methods take an explicit seed.** Comparisons use equal evaluation
  budgets and multiple seeds — this is graded (outcome Ö03).

## Do not

- Do not add solver wrappers that hide the from-scratch requirement. The point of
  the course is implementing simplex, Newton, branch-and-bound, etc. by hand; the
  library is the *check*, not the answer.
- Do not fill in TBD dates or grades. Those come from the instructor.
- Do not create placeholder modules in `src/optlib/` before the week that needs them.

## Environment

```bash
source .venv/bin/activate
```

Dependencies in `requirements.txt`.
