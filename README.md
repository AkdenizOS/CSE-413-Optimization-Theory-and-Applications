# CSE 413 — Optimization Theory and Applications

Akdeniz University, Faculty of Engineering, Computer Engineering (English)
Semester 7 · 4 credits · 6 ECTS · Elective · Language: English

**Instructor:** Arş. Gör. Dr. Taha Yiğit Alkan — [avesis](https://avesis.akdeniz.edu.tr/yigitalkan) · yigitalkan@akdeniz.edu.tr

This repository is my working environment for the course: weekly notes, from-scratch
Python implementations, assignments, exam prep, and the term project.

## Course goal

Model engineering problems as mathematical optimization problems, recognize their
structure (convexity, discreteness, network structure), pick a matching solution
method, and either **prove** the solution is optimal or **honestly measure** its
quality when a proof is impossible. Every method is implemented from scratch in Python.

## Weekly plan

| # | Topic | Folder |
|---|-------|--------|
| 1 | Introduction to optimization: modeling | [weeks/01](weeks/01-introduction-and-modeling.md) |
| 2 | Mathematical foundations: norms, gradient, Taylor, convexity | [weeks/02](weeks/02-mathematical-foundations.md) |
| 3 | Linear programming I: geometry and simplex | [weeks/03](weeks/03-linear-programming-simplex.md) |
| 4 | Linear programming II: duality and sensitivity | [weeks/04](weeks/04-lp-duality-and-sensitivity.md) |
| 5 | Unconstrained I: gradient descent, line search | [weeks/05](weeks/05-unconstrained-gradient-descent.md) |
| 6 | Unconstrained II: Newton, BFGS, L-BFGS, Gauss-Newton | [weeks/06](weeks/06-unconstrained-newton-quasi-newton.md) |
| 7 | Lagrange multipliers and KKT conditions | [weeks/07](weeks/07-lagrange-and-kkt.md) |
| 8 | Convex optimization I: sets, functions, hierarchy | [weeks/08](weeks/08-convex-optimization-theory.md) |
| 9 | Convex optimization II: CVXPY and DCP | [weeks/09](weeks/09-convex-optimization-cvxpy.md) |
| 10 | Stochastic gradient methods: SGD, momentum, Adam, ISTA | [weeks/10](weeks/10-stochastic-gradient-methods.md) |
| 11 | Optimization in ML and deep learning | [weeks/11](weeks/11-optimization-in-ml-and-dl.md) |
| 12 | Discrete I: integer programming, branch and bound | [weeks/12](weeks/12-integer-programming.md) |
| 13 | Discrete II: dynamic programming and networks | [weeks/13](weeks/13-dynamic-programming-and-networks.md) |
| 14 | Metaheuristics and VLSI applications | [weeks/14](weeks/14-metaheuristics-and-vlsi.md) |

## Grading

| Component | Count | Weight |
|-----------|-------|--------|
| Midterm | 1 | 25% |
| Assignments | 4 | 10% |
| Term project | 1 | 25% |
| Final exam | 1 | 40% |

Tracked in [docs/grading.md](docs/grading.md).

## Repository layout

```
docs/            Syllabus summary, grading tracker, resource map, glossary
weeks/NN-*.md    One note per week: goals, reading, tasks, my notes
weeks/code/      Per-week scratch code
src/optlib/      From-scratch implementations reused across weeks
assignments/     hw-01 .. hw-04
project/         Term project (25%)
exams/           Midterm and final preparation
notebooks/       Exploratory Jupyter notebooks
resources/       Syllabus PDF, textbooks, papers, slide decks
```

Each week note links to the weeks it builds on and leads to, so Obsidian's graph
view shows the actual dependency chain — simplex (week 3) feeding branch-and-bound
(week 12) and max-flow (week 13), duality (week 4) feeding KKT (week 7), and so on.

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Learning outcomes

- **Ö01** Model a problem; analyze its structure; justify the chosen method.
- **Ö02** Explain and implement core algorithms from scratch; use SciPy, CVXPY, PuLP/CBC, PyTorch.
- **Ö03** Certify optimality via duality/KKT; where impossible, measure heuristic performance with a proper experiment design (equal budget, multiple seeds, statistics).
- **Ö04** Apply optimization to ML, network routing, and VLSI design; deliver an end-to-end term project with a written report and oral presentation.
