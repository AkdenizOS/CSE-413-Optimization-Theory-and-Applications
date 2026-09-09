# Resource Map — Which Source Covers Which Week

The course syllabus is the instructor's own synthesis; no single book covers it.
The Boyd slides in `resources/slides/` are the **standard Stanford EE364a deck**
(11 chapters: intro, convex sets, convex functions, convex problems, duality,
approximation & fitting, statistical estimation, geometric problems, unconstrained
minimization, equality-constrained minimization, interior-point methods).
They cover roughly weeks 2 and 5-9 only — the LP/simplex, integer programming,
dynamic programming, network, SGD/deep-learning, and metaheuristics weeks come
from the other sources below.

| Week | Topic | Primary source |
|------|-------|----------------|
| 1 | Modeling | Boyd Ch. 1 · Winston Ch. 1-2 |
| 2 | Math foundations | Nocedal Ch. 2 + App. A · Boyd App. A, 2.1, 3.1 |
| 3 | LP, simplex | Winston Ch. 3-4 · Pınar *Doğrusal Optimizasyondan Çıkış* · Taha |
| 4 | LP duality, sensitivity | Winston Ch. 6 · Boyd 5.1-5.2 |
| 5 | Gradient descent | Nocedal Ch. 3 · Boyd Ch. 9.1-9.3 |
| 6 | Newton, quasi-Newton | Nocedal Ch. 6, 7, 10 · Boyd Ch. 9.5 |
| 7 | Lagrange, KKT | Boyd Ch. 5 · Nocedal Ch. 12 |
| 8 | Convex theory | Boyd Ch. 2-4 · Pınar *Dışbükeylik ve Optimizasyon* |
| 9 | CVXPY / DCP | Boyd Ch. 4, 6, 7, 8 · CVXPY docs · cvxbook additional exercises |
| 10 | SGD, Adam, ISTA | Nocedal Ch. 7 · Adam (2014), FISTA (2009) papers |
| 11 | ML/DL optimization | Nocedal Ch. 8 (autodiff) · Goodfellow Ch. 8 · PyTorch docs |
| 12 | Integer programming | Winston Ch. 9 · Taha |
| 13 | DP and networks | Winston Ch. 8, 18-19 · Taha |
| 14 | Metaheuristics, VLSI | Karaboğa · Boyd Ch. 4.5 (geometric programming) |

## Files in this repository

| File | Source |
|------|--------|
| `resources/syllabus/CSE413-syllabus.pdf` | Official Akdeniz University course syllabus |
| `resources/books/boyd-vandenberghe-convex-optimization.pdf` | Boyd & Vandenberghe (2004), free at [stanford.edu/~boyd/cvxbook](https://web.stanford.edu/~boyd/cvxbook/) |
| `resources/books/nocedal-wright-numerical-optimization.pdf` | Nocedal & Wright (2006), Springer |
| `resources/books/winston-operations-research.pdf` | Winston (2004), Brooks/Cole |
| `resources/books/pinar-disbukeylik-ve-optimizasyon.pdf` | Pınar (2020), Bilkent lecture notes (TR) |
| `resources/books/pinar-dogrusal-optimizasyondan-cikis.pdf` | Pınar (2020), Seçkin (TR) |
| `resources/slides/bv_cvxslides.pdf` | Boyd/Vandenberghe/Nobel, 2024 revision |
| `resources/slides/bv_cvxslides_original.pdf` | Boyd/Vandenberghe, 2016 original |

## Not in this repository

- Karaboğa, D. (2014). *Yapay Zeka Optimizasyon Algoritmaları*. Nobel Akademik Yayıncılık. — needed for week 14 (ABC).
- Taha, H. A. (2018). *Yöneylem Araştırması* (6th ed., TR translation). Literatür Yayıncılık.

## Useful links

- Boyd cvxbook additional exercises: https://github.com/cvxgrp/cvxbook_additional_exercises
- CVXPY: https://www.cvxpy.org/
- Stanford EE364a lectures: https://web.stanford.edu/class/ee364a/
- SciPy optimize: https://docs.scipy.org/doc/scipy/reference/optimize.html
- PuLP: https://coin-or.github.io/pulp/
