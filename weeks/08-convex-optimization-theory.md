# Week 8 — Convex Optimization I: Sets, Functions, Problem Hierarchy

> Syllabus (TR): *Dışbükey optimizasyon I: dışbükey kümeler ve fonksiyonlar; problem hiyerarşisi*

**Builds on:** [Week 2 · Mathematical Foundations](02-mathematical-foundations.md) · [Week 7 · Lagrange Multipliers and KKT Conditions](07-lagrange-and-kkt.md)
**Leads to:** [Week 9 · Convex Optimization II: CVXPY and Disciplined Convex Programming](09-convex-optimization-cvxpy.md) · [Week 14 · Metaheuristics and VLSI Applications](14-metaheuristics-and-vlsi.md)

## Goals
- Prove convexity of sets and functions using the standard toolbox.
- Place a problem in the hierarchy LP ⊂ QP ⊂ SOCP ⊂ SDP.

## Key concepts
- Convex sets: hyperplanes, halfspaces, norm balls, polyhedra, PSD cone, second-order cone.
- Operations preserving convexity: intersection, affine maps, perspective, linear-fractional.
- Convex functions: first-/second-order conditions, epigraph, sublevel sets, Jensen.
- Convexity-preserving operations: nonneg. weighted sum, composition rules, pointwise max/sup, partial minimization.
- Quasiconvexity.
- Hierarchy: LP → QP → QCQP → SOCP → SDP; each is a special case of the next.

## Reading

- [Boyd — Ch. 2 (convex sets)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=35)
- [Boyd — Ch. 3 (convex functions)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=81)
- [Boyd — Ch. 4 (convex optimization problems)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=141)
- Boyd slides — Sections 2, 3, 4
- Pınar, *Dışbükeylik ve Optimizasyon* (TR) — "Dışbükey Kümeler/Fonksiyonlar/Optimizasyon", "Konik Optimizasyon"; 92 worked examples

## Implement
- [ ] Convexity checker for a quadratic (eigenvalue test) and a sampled numerical check (`f(θx+(1−θ)y) ≤ θf(x)+(1−θ)f(y)`).
- [ ] Reformulate 3 problems (e.g. ℓ∞ regression, robust LP, max-volume ellipsoid) into their canonical class.

## Checklist
- [ ] Notes written
- [ ] Can classify a given problem into LP/QP/SOCP/SDP on sight
- [ ] Worked ≥5 exercises from `resources/books/boyd-vandenberghe-convex-optimization.pdf` Ch. 2-4

## My notes

<!-- Lecture: what was actually covered. -->

<!-- Derivations worked out by hand. -->

<!-- Questions to ask the instructor. -->

<!-- Exam-worthy: formulas, conditions, algorithm steps. -->
