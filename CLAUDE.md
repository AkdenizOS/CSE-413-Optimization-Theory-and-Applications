# CSE 413 — Working Notes for AI Sessions

Course repository for Optimization Theory and Applications (Akdeniz University,
Computer Engineering, semester 7). Read [`docs/syllabus.md`](docs/syllabus.md) for
what the course covers and [`docs/resource-map.md`](docs/resource-map.md) for which
book covers which week.

## What this repo is for

Studying. The deliverables are understanding, working from-scratch implementations,
assignments, and a term project — not a production system.

## Conventions

- **Language:** English for everything committed — READMEs, notes, code, comments.
  Turkish appears only where the source is Turkish (syllabus quotes, glossary,
  Turkish reference books).
- **Week folders:** `weeks/NN-topic-slug/` with `README.md` (goals, reading, tasks,
  checklist), `notes.md` (personal notes taken during/after lecture), and `code/`.
- **Shared code:** anything reused by two or more weeks moves to `src/optlib/`.
  One-off experiments stay in the week's `code/`.
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
