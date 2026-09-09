# CSE 413 — Syllabus Summary

Source: [`resources/syllabus/CSE413-syllabus.pdf`](../resources/syllabus/CSE413-syllabus.pdf) (official, Turkish).
This is an English summary; the PDF is authoritative.

## Course identity

| Field | Value |
|-------|-------|
| Code | CSE 413 |
| Title | Optimization Theory and Applications |
| Semester | 7 |
| T+U | 4 |
| Credits | 4 |
| ECTS | 6 |
| Type | Elective |
| Level | Faculty |
| Language | English |
| Delivery | Formal education (örgün öğretim) |
| Prerequisite | None |
| Internship | None |
| Coordinator / Instructor | Arş. Gör. Dr. Taha Yiğit Alkan |
| Contact | yigitalkan@akdeniz.edu.tr · https://avesis.akdeniz.edu.tr/yigitalkan |

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
