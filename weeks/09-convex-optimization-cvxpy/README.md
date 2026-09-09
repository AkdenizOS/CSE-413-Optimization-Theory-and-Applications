# Week 9 — Convex Optimization II: CVXPY and Disciplined Convex Programming

> Syllabus (TR): *Dışbükey optimizasyon II: CVXPY ile disiplinli dışbükey programlama, dual değişkenlerin okunması, uygulama galerisi*

## Goals
- Express problems in DCP form and get them accepted by CVXPY.
- Read and interpret dual variables returned by the solver.
- Build a personal gallery of solved application problems.

## Key concepts
- DCP ruleset: expressions built from atoms with known curvature and monotonicity.
- Why `cp.square(x)/y` fails but `cp.quad_over_lin(x, y)` works.
- Solvers: ECOS, SCS, CLARABEL, OSQP — which for which cone.
- `constraint.dual_value` ↔ the `λ*` from Week 7.
- Applications: regularized regression (LASSO, ridge), SVM, portfolio optimization, robust LP, Chebyshev center, minimum-volume ellipsoid.

## Reading
- Boyd & Vandenberghe — Ch. 4, Ch. 6 (approximation and fitting), Ch. 7 (statistical estimation), Ch. 8 (geometric problems)
- Pınar, *Dışbükeylik ve Optimizasyon* (TR) — "Disiplinli Dışbükey Programlama" (DCP in Turkish), "Matris Değişkenli Problemler"
- CVXPY docs: https://www.cvxpy.org/
- Additional exercises: https://github.com/cvxgrp/cvxbook_additional_exercises

## Implement
- [ ] LASSO regularization path; compare with `sklearn`.
- [ ] SVM primal and dual in CVXPY; verify KKT/complementary slackness on the support vectors.
- [ ] Reproduce your Week-7 water-filling solution in CVXPY and match the dual variable.
- [ ] Fix 3 deliberately DCP-invalid formulations.

## Checklist
- [ ] Notes written
- [ ] Dual values match hand-derived KKT multipliers
- [ ] Gallery has ≥4 working application scripts in `code/`
