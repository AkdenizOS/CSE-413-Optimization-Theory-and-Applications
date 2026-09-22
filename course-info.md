# CSE 413 — Syllabus Summary

Source: [`resources/CSE413-syllabus.pdf`](resources/CSE413-syllabus.pdf) (official, Turkish).
This is an English summary; the PDF is authoritative.
The instructor's own English syllabus for 2026-2027 Fall is
[`resources/2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Syllabus.pdf`](resources/2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Syllabus.pdf).

## Course identity

| Field                    | Value                                                                |
| ------------------------ | -------------------------------------------------------------------- |
| Code                     | CSE 413                                                              |
| Title                    | Optimization Theory and Applications                                 |
| Semester                 | 7                                                                    |
| T+U                      | 4                                                                    |
| Credits                  | 4                                                                    |
| ECTS                     | 6                                                                    |
| Type                     | Elective                                                             |
| Level                    | Faculty                                                              |
| Language                 | English                                                              |
| Delivery                 | Formal education (örgün öğretim)                                     |
| Prerequisite             | None                                                                 |
| Internship               | None                                                                 |
| Coordinator / Instructor | Arş. Gör. Dr. Taha Yiğit Alkan                                       |
| Contact                  | yigitalkan@akdeniz.edu.tr · https://avesis.akdeniz.edu.tr/yigitalkan |

## Aim

Give students the ability to model engineering problems as mathematical optimization
problems, recognize the problem's structure (convexity, discreteness, network
structure), and choose and apply a matching solution method.

The course covers linear programming and duality, gradient-based and Newton-type
methods, Lagrange/KKT conditions, convex optimization, stochastic gradient methods,
integer programming, dynamic programming, network optimization, and metaheuristics —
each with its theoretical foundation. **All methods are implemented from scratch in
Python** and applied to current computer-engineering problems such as machine
learning, network routing, resource allocation, and VLSI design.

By the end, the student should be able to model a problem, select the right solver,
prove the optimality of the solution obtained, or — when a proof is not possible —
measure solution quality with honest statistical methods.

## Course structure (content distribution)

| Area | % |
|------|---|
| Mathematics and basic sciences | 30 |
| Engineering sciences | 40 |
| Engineering design | 20 |
| Field knowledge | 10 |

## Learning outcomes

- **Ö01** — Models engineering problems as mathematical optimization problems with decision variables, an objective function, and constraints; analyzes the problem's structure (convexity, discreteness, network structure) and selects a suitable solution method with justification.
- **Ö02** — Explains the core optimization algorithms (simplex, gradient descent, Newton, branch and bound, dynamic programming, metaheuristics) with their theoretical foundations; implements them from scratch in Python and uses modern software tools (SciPy, CVXPY, PuLP/CBC, PyTorch) effectively.
- **Ö03** — Certifies the optimality of a solution using duality and KKT conditions and performs sensitivity analysis; where an optimality proof is not possible, measures and interprets heuristic performance through experiment design (equal budget, multiple seeds, statistical distributions).
- **Ö04** — Applies optimization techniques to computer-engineering problems such as machine learning, network routing, and VLSI design; designs an end-to-end solution under realistic constraints in the term project and communicates the results in a written report and an oral presentation.

## Program outcome contributions

| | P01 | P02 | P03 | P04 | P05 | P06 | P07 |
|---|---|---|---|---|---|---|---|
| **All** | 5 | 5 | 4 | 5 | 4 | 3 | 3 |
| Ö01 | 5 | 5 | | | | | |
| Ö02 | 4 | | | 5 | | | |
| Ö03 | 4 | 3 | | | 5 | | |
| Ö04 | | 4 | 4 | 3 | | 3 | 4 |

Contribution level: 1 = very low … 5 = very high.

## Assessment

| Component | Count | Weight |
|-----------|-------|--------|
| Midterm | 1 | 25% |
| Quiz | 0 | 0% |
| Assignments / seminar | 4 | 10% |
| Attendance | 0 | 0% |
| Practice | 0 | 0% |
| Term project | 1 | 25% |
| Final exam | 1 | 40% |

## Weekly topics

1. Introduction to optimization: modeling, decision variables, objective function, constraints; optimization problems in engineering.
2. Mathematical foundations: norms, gradient, Taylor expansion, quadratic forms; first look at convexity; the numerical computing environment.
3. Linear programming I: geometry, vertices, and the simplex method; implementing tableau simplex.
4. Linear programming II: duality, shadow prices, complementary slackness, and sensitivity analysis.
5. Unconstrained optimization I: gradient descent, step selection (Armijo/backtracking), convergence rates, and the condition number.
6. Unconstrained optimization II: Newton's method, quasi-Newton (BFGS, L-BFGS), Gauss-Newton; a method-selection guide.
7. Lagrange multipliers and KKT conditions: optimality certificates, connection to duality; the water-filling problem.
8. Convex optimization I: convex sets and functions; the problem hierarchy.
9. Convex optimization II: disciplined convex programming with CVXPY, reading dual variables, an application gallery.
10. Stochastic gradient methods: SGD, momentum, Adam, learning-rate schedules, proximal methods / ISTA.
11. Optimization in machine learning and deep learning: empirical risk minimization, backpropagation = automatic differentiation, training recipes, model compression.
12. Discrete optimization I — integer programming: modeling techniques (big-M, either/or), LP relaxation, branch and bound, cutting planes.
13. Discrete optimization II — dynamic programming and network optimization: Bellman's principle, Dijkstra, Bellman-Ford, A*, max-flow / min-cut.
14. Metaheuristics and VLSI applications: simulated annealing, genetic algorithms, particle swarm, artificial bee colony (ABC); placement and gate sizing.

## References

- Boyd, S., & Vandenberghe, L. (2004). *Convex optimization*. Cambridge University Press. https://web.stanford.edu/~boyd/cvxbook/
- Karaboğa, D. (2014). *Yapay zeka optimizasyon algoritmaları* (updated ed.). Nobel Akademik Yayıncılık.
- Nocedal, J., & Wright, S. J. (2006). *Numerical optimization* (2nd ed.). Springer.
- Pınar, M. Ç. (2020). *Dışbükeylik ve optimizasyon: Ders notları*. Bilkent University. https://www.ie.bilkent.edu.tr/~mustafap/pubs/kitapconvopt-toc.pdf
- Pınar, M. Ç. (2020). *Doğrusal optimizasyondan çıkış: Ders notları*. Seçkin Yayıncılık.
- Taha, H. A. (2018). *Yöneylem araştırması* (6th ed., trans. Ş. A. Baray & Ş. Esnaf). Literatür Yayıncılık.
- Winston, W. L. (2004). *Operations research: Applications and algorithms* (4th ed.). Brooks/Cole.

## Grading Tracker

| Component | Count | Weight | Status | Grade |
|-----------|-------|--------|--------|-------|
| Midterm (Ara Sınav) | 1 | 25% | — | — |
| Assignments (Ödev) | 4 | 10% | 0/4 | — |
| Term project (Dönem Ödevi / Proje) | 1 | 25% | — | — |
| Final (Yarıyıl Sonu Sınavı) | 1 | 40% | — | — |
| **Total** | | **100%** | | |

### Assignments

| # | Topic | Assigned | Due | Status | Grade |
|---|-------|----------|-----|--------|-------|
| 1 | TBD | | | not started | |
| 2 | TBD | | | not started | |
| 3 | TBD | | | not started | |
| 4 | TBD | | | not started | |

### Key dates

| Event | Date |
|-------|------|
| Semester start | TBD |
| Midterm | TBD |
| Project proposal due | TBD |
| Project report + presentation | TBD |
| Final exam | TBD |

### Expected workload (ECTS 6 = 168 hours)

| Activity | Count | Hours each | Total |
|----------|-------|-----------|-------|
| Lectures | 14 | 3 | 42 |
| Outside-class study | 14 | 3 | 42 |
| Assignments | 4 | 8 | 32 |
| Midterm prep | 1 | 12 | 12 |
| Project | 1 | 20 | 20 |
| Final prep | 1 | 20 | 20 |
| **Total** | | | **168** |

## Resource Map — Which Source Covers Which Week

Every chapter number below was verified against the actual PDF in `resources/`,
not quoted from memory. Where a syllabus reference is not obtainable, a free
substitute is named.

### What the slide deck actually is

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

### Week → source

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
| 14 | Metaheuristics, VLSI | Karaboga TR06 + pseudocode (`resources/papers/`) · Boyd Ch. 4.5 (geometric programming) |

### Files in this repository

| File | Source | Verified contents |
|------|--------|-------------------|
| `CSE413-syllabus.pdf` | Official Akdeniz University syllabus | 14 weeks, outcomes Ö01-Ö04, grading, references |
| `2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Syllabus.pdf` | Instructor, 2026-2027 Fall | Term syllabus (English), 2 pp. |
| `2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Week_01.pdf` | Instructor, 2026-2027 Fall | Week 1 lecture slides — introduction and problem formulation, 21 pp. |
| `books/boyd-vandenberghe-convex-optimization.pdf` | Boyd & Vandenberghe (2004) — free at [stanford.edu/~boyd/cvxbook](https://web.stanford.edu/~boyd/cvxbook/) | Ch. 1-11 |
| `books/nocedal-wright-numerical-optimization.pdf` | Nocedal & Wright (2006), Springer | 19 chapters; 2 unconstrained fundamentals, 3 line search, 6 quasi-Newton, 7 large-scale, 8 derivatives, 10 least squares, 12 constrained theory, 13 simplex |
| `books/winston-operations-research.pdf` | Winston (2004), Brooks/Cole | 24 chapters; 3 LP, 4 simplex, 5-6 sensitivity/duality, 7 transportation, 8 networks, 9 integer programming, 18 deterministic DP |
| `books/pinar-disbukeylik-ve-optimizasyon.pdf` | Pınar (2020), Seçkin — 290 pp. (TR) | Convex sets/functions/optimization, Lagrange & Fenchel duality, conic optimization, optimality conditions, matrix-variable problems, DCP. **92 examples, 122 solved exercises** |
| `books/pinar-dogrusal-optimizasyondan-cikis.pdf` | Pınar (2019), Seçkin — 259 pp. (TR) | Polyhedra, duality, Lagrange method, theorems of alternatives, assignment, network problems, graph theory, simplex, interior point, shortest path. **17 applications, 61 exercises** |
| `papers/karaboga-2005-abc-tr06.pdf` | Karaboga (2005), Technical Report TR06, Erciyes Üniversitesi | The original ABC paper, 10 pp. |
| `papers/karaboga-abc-pseudocode.pdf` | abc.erciyes.edu.tr | Detailed ABC pseudocode, 2 pp. |
| `papers/karaboga-abc-step-by-step.pdf` | abc.erciyes.edu.tr | Worked step-by-step ABC trace, 5 pp. |
| `slides/bv_cvxslides.pdf` | Boyd/Vandenberghe/Nobel, 2024 revision | 11 sections, 402 pp. |
| `slides/bv_cvxslides_original.pdf` | Boyd/Vandenberghe, 2016 | same deck, older |

### Missing syllabus references and what to use instead

**Karaboğa, D. (2014). *Yapay zeka optimizasyon algoritmaları*. Nobel Akademik.**
Needed for week 14 (ABC). Turkish print book, not available online — buy or borrow
from the library. Covered instead by the three papers now in `resources/papers/`,
downloaded from Karaboğa's own site: the original TR06 report, the detailed
pseudocode, and a step-by-step worked trace. That is enough to implement ABC.

**Karaboga & Basturk (2007). *A powerful and efficient algorithm for numerical
function optimization: artificial bee colony (ABC) algorithm*. J. Global
Optimization 39(3), 459-471.** DOI [10.1007/s10898-007-9149-x](https://doi.org/10.1007/s10898-007-9149-x).
Paywalled at Springer, and the author has not self-archived it. Akdeniz University
has a Springer subscription — download it from campus network or through the
library proxy. Content-wise it is the journal version of TR06 plus benchmark
comparisons against GA, PSO and DE, so TR06 covers the algorithm itself.

ABC reference implementations (Python, Rust, C#, Delphi):
https://github.com/artificialbeecolony

For SA, GA and PSO the original papers are all free: Kirkpatrick et al. (1983,
*Science*), Holland (1975) / Goldberg (1989), Kennedy & Eberhart (1995, ICNN).

**Taha, H. A. (2018). *Yöneylem araştırması* (TR translation). Literatür.**
Not obtainable, and **not needed** — Winston is the same kind of OR textbook and
covers every topic the syllabus cites Taha for (LP, integer programming, networks,
DP), and Pınar *Doğrusal* covers the same ground in Turkish with solved exercises.
Skip it.

### Useful links

- Boyd cvxbook additional exercises: https://github.com/cvxgrp/cvxbook_additional_exercises
- CVXPY: https://www.cvxpy.org/
- Stanford EE364a: https://web.stanford.edu/class/ee364a/
- Karaboğa's ABC page: https://abc.erciyes.edu.tr/
- SciPy optimize: https://docs.scipy.org/doc/scipy/reference/optimize.html
- PuLP: https://coin-or.github.io/pulp/

## Glossary — Turkish ↔ English

Lectures and exams are in English, but the syllabus and two of the reference books
are Turkish. This maps the terms between them.

| Turkish | English |
|---------|---------|
| eniyileme / optimizasyon | optimization |
| amaç fonksiyonu | objective function |
| karar değişkeni | decision variable |
| kısıt | constraint |
| olurlu bölge / uygun küme | feasible region / feasible set |
| eniyilik | optimality |
| eniyilik sertifikası | optimality certificate |
| dışbükey | convex |
| içbükey | concave |
| dışbükey küme | convex set |
| doğrusal programlama | linear programming |
| simpleks yöntemi | simplex method |
| köşe noktası | vertex / extreme point |
| temel olurlu çözüm | basic feasible solution (BFS) |
| dualite / ikilik | duality |
| gölge fiyat | shadow price |
| tamamlayıcı gevşeklik | complementary slackness |
| duyarlılık analizi | sensitivity analysis |
| gevşetme | relaxation |
| kısıtsız optimizasyon | unconstrained optimization |
| gradyan iniş | gradient descent |
| geri izleme (adım arama) | backtracking line search |
| yakınsama hızı | convergence rate |
| koşul sayısı | condition number |
| karesel form | quadratic form |
| Lagrange çarpanı | Lagrange multiplier |
| su doldurma | water-filling |
| stokastik gradyan | stochastic gradient |
| öğrenme oranı | learning rate |
| geri yayılım | backpropagation |
| otomatik türev | automatic differentiation |
| deneysel risk minimizasyonu | empirical risk minimization |
| model sıkıştırma | model compression |
| tamsayılı programlama | integer programming |
| dal-sınır | branch and bound |
| kesme düzlemi | cutting plane |
| dinamik programlama | dynamic programming |
| en kısa yol | shortest path |
| en büyük akış | maximum flow |
| en küçük kesit | minimum cut |
| ağ optimizasyonu | network optimization |
| metasezgisel | metaheuristic |
| benzetimli tavlama | simulated annealing |
| genetik algoritma | genetic algorithm |
| parçacık sürüsü optimizasyonu | particle swarm optimization |
| yapay arı kolonisi | artificial bee colony (ABC) |
| tümdevre (VLSI) tasarımı | VLSI design |
| kapı boyutlandırma | gate sizing |
| yerleşim | placement |
