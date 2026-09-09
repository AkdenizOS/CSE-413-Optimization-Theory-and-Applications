# Resource Map — Which Source Covers Which Week

Every chapter number below was verified against the actual PDF in `resources/`,
not quoted from memory. Where a syllabus reference is not obtainable, a free
substitute is named.

## What the slide deck actually is

`resources/slides/bv_cvxslides.pdf` is the **standard Stanford EE364a deck** by
Boyd, Vandenberghe and Nobel (2024 revision, 402 pages) — not the instructor's own
slides. Its 11 sections are: 1 Introduction · 2 Convex sets · 3 Convex functions ·
4 Convex optimization problems · 5 Duality · 6 Approximation and fitting ·
7 Statistical estimation · 8 Geometric problems · B Numerical linear algebra ·
9 Unconstrained minimization · 10 Equality constrained minimization ·
11 Interior-point methods.

That covers roughly **weeks 2 and 5-9 only**. The LP/simplex, integer programming,
dynamic programming, network, SGD/deep-learning and metaheuristics weeks come from
the other sources. Conversely, interior-point methods (deck section 11) are **not**
in the syllabus.

`bv_cvxslides_original.pdf` is the 2016 edition of the same deck.

## Week → source

| Week | Topic | Primary source (verified) |
|------|-------|---------------------------|
| 1 | Modeling | Boyd Ch. 1 · Winston Ch. 1 (model building) |
| 2 | Math foundations | Nocedal Ch. 2 (fundamentals of unconstrained opt.) · Winston Ch. 2 (linear algebra) · Boyd App. A, 2.1, 3.1 · Pınar *Dışbükeylik* |
| 3 | LP, simplex | Winston Ch. 3 (intro to LP), Ch. 4 (simplex algorithm) · Nocedal Ch. 13 (LP: simplex) · Pınar *Doğrusal* — Çokyüzlüler, Simpleks Yöntemi |
| 4 | LP duality, sensitivity | Winston Ch. 5 (sensitivity applied), Ch. 6 (sensitivity + duality) · Boyd 5.1-5.2 · Pınar *Doğrusal* — Eşterslik, İkili Seçenek Teoremleri |
| 5 | Gradient descent | Nocedal Ch. 3 (line search methods) · Boyd Ch. 9.1-9.3 |
| 6 | Newton, quasi-Newton | Nocedal Ch. 6 (quasi-Newton), Ch. 7 (large-scale), Ch. 10 (least squares) · Boyd Ch. 9.5 |
| 7 | Lagrange, KKT | Boyd Ch. 5 · Nocedal Ch. 12 (theory of constrained opt.) · Pınar *Dışbükeylik* — Lagrange Eştersliği, Optimallik Koşulları |
| 8 | Convex theory | Boyd Ch. 2-4 · Pınar *Dışbükeylik* — Dışbükey Kümeler/Fonksiyonlar/Optimizasyon, Konik Optimizasyon |
| 9 | CVXPY / DCP | Boyd Ch. 4, 6, 7, 8 · Pınar *Dışbükeylik* — **Disiplinli Dışbükey Programlama** (DCP in Turkish) · CVXPY docs |
| 10 | SGD, Adam, ISTA | Nocedal Ch. 7 · Adam (2014), FISTA (2009) papers — **no book covers this** |
| 11 | ML/DL optimization | Nocedal Ch. 8 (calculating derivatives = autodiff) · Goodfellow Ch. 8 · PyTorch docs |
| 12 | Integer programming | Winston Ch. 9 (integer programming) |
| 13 | DP and networks | Winston Ch. 7 (transportation/assignment), Ch. 8 (network models), Ch. 18 (deterministic DP) · Pınar *Doğrusal* — Ağ Problemleri, Çizge Kuramı, En Kısa Yol |
| 14 | Metaheuristics, VLSI | Karaboga TR06 (2005, free) · Boyd Ch. 4.5 (geometric programming) |

## Files in this repository

| File | Source | Verified contents |
|------|--------|-------------------|
| `syllabus/CSE413-syllabus.pdf` | Official Akdeniz University syllabus | 14 weeks, outcomes Ö01-Ö04, grading, references |
| `books/boyd-vandenberghe-convex-optimization.pdf` | Boyd & Vandenberghe (2004) — free at [stanford.edu/~boyd/cvxbook](https://web.stanford.edu/~boyd/cvxbook/) | Ch. 1-11 |
| `books/nocedal-wright-numerical-optimization.pdf` | Nocedal & Wright (2006), Springer | 19 chapters; 2 unconstrained fundamentals, 3 line search, 6 quasi-Newton, 7 large-scale, 8 derivatives, 10 least squares, 12 constrained theory, 13 simplex |
| `books/winston-operations-research.pdf` | Winston (2004), Brooks/Cole | 24 chapters; 3 LP, 4 simplex, 5-6 sensitivity/duality, 7 transportation, 8 networks, 9 integer programming, 18 deterministic DP |
| `books/pinar-disbukeylik-ve-optimizasyon.pdf` | Pınar (2020), Seçkin — 290 pp. (TR) | Convex sets/functions/optimization, Lagrange & Fenchel duality, conic optimization, optimality conditions, matrix-variable problems, DCP. **92 examples, 122 solved exercises** |
| `books/pinar-dogrusal-optimizasyondan-cikis.pdf` | Pınar (2019), Seçkin — 259 pp. (TR) | Polyhedra, duality, Lagrange method, theorems of alternatives, assignment, network problems, graph theory, simplex, interior point, shortest path. **17 applications, 61 exercises** |
| `slides/bv_cvxslides.pdf` | Boyd/Vandenberghe/Nobel, 2024 revision | 11 sections, 402 pp. |
| `slides/bv_cvxslides_original.pdf` | Boyd/Vandenberghe, 2016 | same deck, older |

## Missing syllabus references and what to use instead

**Karaboğa, D. (2014). *Yapay zeka optimizasyon algoritmaları*. Nobel Akademik.**
Needed for week 14 (ABC). Not freely available — Turkish print book, buy or borrow
from the library. Free substitutes that cover ABC completely:

- Karaboga, D. (2005). *An idea based on honey bee swarm for numerical
  optimization*. Technical Report TR06, Erciyes University. The original ABC paper,
  by the same author, free: https://abc.erciyes.edu.tr/
- Karaboga & Basturk (2007). *A powerful and efficient algorithm for numerical
  function optimization: artificial bee colony (ABC) algorithm*. Journal of Global
  Optimization 39(3), 459-471.
- https://abc.erciyes.edu.tr/ also hosts reference implementations and a
  publication list.

For SA, GA and PSO the original papers are all free: Kirkpatrick et al. (1983,
*Science*), Holland (1975) / Goldberg (1989), Kennedy & Eberhart (1995, ICNN).

**Taha, H. A. (2018). *Yöneylem araştırması* (TR translation). Literatür.**
Not obtainable, and **not needed** — Winston is the same kind of OR textbook and
covers every topic the syllabus cites Taha for (LP, integer programming, networks,
DP), and Pınar *Doğrusal* covers the same ground in Turkish with solved exercises.
Skip it.

## Useful links

- Boyd cvxbook additional exercises: https://github.com/cvxgrp/cvxbook_additional_exercises
- CVXPY: https://www.cvxpy.org/
- Stanford EE364a: https://web.stanford.edu/class/ee364a/
- Karaboğa's ABC page: https://abc.erciyes.edu.tr/
- SciPy optimize: https://docs.scipy.org/doc/scipy/reference/optimize.html
- PuLP: https://coin-or.github.io/pulp/
