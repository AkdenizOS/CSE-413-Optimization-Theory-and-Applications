# Week 3 — Linear Programming I: Geometry and the Simplex Method

> Syllabus (TR): *Doğrusal programlama I: geometri, köşe noktaları ve simpleks yöntemi; tablo simpleksinin gerçeklenmesi*

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
- Winston, *Operations Research* — Ch. 3 (LP intro), Ch. 4 (simplex)
- Nocedal & Wright — Ch. 13 (LP: the simplex method)
- Pınar, *Doğrusal Optimizasyondan Çıkış* (TR) — "Çokyüzlüler", "Simpleks Yöntemi"
- Taha, *Yöneylem Araştırması* — LP chapters

## Implement
- [ ] Tableau simplex (`src/optlib/simplex.py`): pivoting, ratio test, Bland's rule.
- [ ] Two-phase method for an initial BFS.
- [ ] Cross-check against `scipy.optimize.linprog` on random LPs.

## Checklist
- [ ] Notes written
- [ ] Simplex matches SciPy on 100 random feasible LPs
- [ ] Can trace a full tableau iteration by hand
