# Week 8 — Convex Optimization I: Sets, Functions, Problem Hierarchy

> Syllabus (TR): *Dışbükey optimizasyon I: dışbükey kümeler ve fonksiyonlar; problem hiyerarşisi*

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
- Boyd & Vandenberghe — Ch. 2 (convex sets), Ch. 3 (convex functions), Ch. 4 (convex problems)
- Boyd slides — Sections 2, 3, 4
- Pınar, *Dışbükeylik ve Optimizasyon* (TR) — "Dışbükey Kümeler", "Dışbükey Fonksiyonlar", "Dışbükey Optimizasyon", "Konik Optimizasyon"; 92 worked examples

## Implement
- [ ] Convexity checker for a quadratic (eigenvalue test) and a sampled numerical check (`f(θx+(1−θ)y) ≤ θf(x)+(1−θ)f(y)`).
- [ ] Reformulate 3 problems (e.g. ℓ∞ regression, robust LP, max-volume ellipsoid) into their canonical class.

## Checklist
- [ ] Notes written
- [ ] Can classify a given problem into LP/QP/SOCP/SDP on sight
- [ ] Worked ≥5 exercises from `resources/books/boyd-vandenberghe-convex-optimization.pdf` Ch. 2-4
