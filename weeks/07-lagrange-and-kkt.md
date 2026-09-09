# Week 7 — Lagrange Multipliers and KKT Conditions

> Syllabus (TR): *Lagrange çarpanları ve KKT koşulları: eniyilik sertifikaları, dualite bağlantısı; su doldurma problemi*

**Builds on:** [Week 4 · Linear Programming II: Duality and Sensitivity](04-lp-duality-and-sensitivity.md) · [Week 5 · Unconstrained Optimization I: Gradient Descent](05-unconstrained-gradient-descent.md)
**Leads to:** [Week 8 · Convex Optimization I: Sets, Functions, Problem Hierarchy](08-convex-optimization-theory.md) · [Week 9 · Convex Optimization II: CVXPY and Disciplined Convex Programming](09-convex-optimization-cvxpy.md)

## Goals
- Write the Lagrangian and dual function for a constrained problem.
- State and apply the KKT conditions as an optimality certificate.
- Solve the water-filling problem analytically.

## Key concepts
- Lagrangian `L(x,λ,ν) = f₀(x) + Σλᵢfᵢ(x) + Σνᵢhᵢ(x)`; dual function `g(λ,ν) = inf_x L`.
- Weak duality always; strong duality under Slater's condition.
- Duality gap; the dual is *always* concave, even for non-convex primal.
- KKT: stationarity, primal feasibility, dual feasibility, complementary slackness.
- Water-filling: `x_i* = max(0, 1/ν − α_i)` — the canonical closed-form KKT example.
- Sensitivity: `λ*` = shadow price of constraint `i` (same idea as [Week 4](04-lp-duality-and-sensitivity.md)).

## Reading

- [Boyd — Ch. 5 (duality), especially 5.5 (optimality conditions)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=229)
- [Nocedal & Wright — Ch. 12 (theory of constrained optimization)](../resources/books/nocedal-wright-numerical-optimization.pdf#page=323)
- Pınar, *Dışbükeylik ve Optimizasyon* (TR) — "Lagrange Eştersliği", "Optimallik Koşulları"; 122 solved exercises

## Implement
- [ ] Water-filling: closed-form bisection on `ν` vs. CVXPY solution.
- [ ] KKT residual checker: given `(x, λ, ν)`, report violation of each of the 4 conditions.
- [ ] Dual function plot for a small problem; visualize the duality gap.

## Checklist
- [ ] Notes written
- [ ] KKT checker validates solutions from Weeks 3-6
- [ ] Can derive water-filling on paper without notes

## My notes

<!-- Lecture: what was actually covered. -->

<!-- Derivations worked out by hand. -->

<!-- Questions to ask the instructor. -->

<!-- Exam-worthy: formulas, conditions, algorithm steps. -->
