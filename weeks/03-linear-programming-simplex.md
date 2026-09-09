# Week 3 — Linear Programming I: Geometry and the Simplex Method

> Syllabus (TR): *Doğrusal programlama I: geometri, köşe noktaları ve simpleks yöntemi; tablo simpleksinin gerçeklenmesi*

**Builds on:** [Week 2 · Mathematical Foundations](02-mathematical-foundations.md)
**Leads to:** [Week 4 · Linear Programming II: Duality and Sensitivity](04-lp-duality-and-sensitivity.md) · [Week 12 · Discrete Optimization I: Integer Programming](12-integer-programming.md) · [Week 13 · Discrete Optimization II: Dynamic Programming and Network Optimization](13-dynamic-programming-and-networks.md)

## Goals
- LP standard form and its geometry (polyhedra, vertices, extreme points).
- Understand why an optimal LP solution can always be found at a vertex.
- Implement tableau simplex from scratch.

## Key concepts
- Standard form: `min cᵀx s.t. Ax = b, x ≥ 0`; slack/surplus variables.
- Polyhedron, vertex ↔ basic feasible solution (BFS); basis `B`, nonbasis `N`.
- Reduced costs `c̄ = c_N − c_Bᵀ B⁻¹ N`; entering / leaving variable; ratio test.
- Degeneracy, cycling, Bland's rule; two-phase / Big-M for finding an initial BFS.
- Complexity note: simplex is exponential worst-case, fast in practice.

## Reading

- [Winston — Ch. 3 (introduction to linear programming)](../resources/books/winston-operations-research.pdf#page=65)
- [Winston — Ch. 4 (the simplex algorithm)](../resources/books/winston-operations-research.pdf#page=143)
- [Nocedal & Wright — Ch. 13 (LP: the simplex method)](../resources/books/nocedal-wright-numerical-optimization.pdf#page=374)
- Pınar, *Doğrusal Optimizasyondan Çıkış* (TR) — "Çokyüzlüler", "Simpleks Yöntemi"

## Implement
- [ ] Tableau simplex (`src/optlib/simplex.py`): pivoting, ratio test, Bland's rule.
- [ ] Two-phase method for an initial BFS.
- [ ] Cross-check against `scipy.optimize.linprog` on random LPs.

## Checklist
- [ ] Notes written
- [ ] Simplex matches SciPy on 100 random feasible LPs
- [ ] Can trace a full tableau iteration by hand

## My notes

<!-- Lecture: what was actually covered. -->

<!-- Derivations worked out by hand. -->

<!-- Questions to ask the instructor. -->

<!-- Exam-worthy: formulas, conditions, algorithm steps. -->
