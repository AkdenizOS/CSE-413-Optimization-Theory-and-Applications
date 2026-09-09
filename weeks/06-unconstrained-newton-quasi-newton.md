# Week 6 — Unconstrained Optimization II: Newton and Quasi-Newton

> Syllabus (TR): *Kısıtsız optimizasyon II: Newton yöntemi, quasi-Newton (BFGS, L-BFGS), Gauss–Newton; yöntem seçim rehberi*

**Builds on:** [Week 5 · Unconstrained Optimization I: Gradient Descent](05-unconstrained-gradient-descent.md)
**Leads to:** [Week 10 · Stochastic Gradient Methods](10-stochastic-gradient-methods.md)

## Goals
- Implement Newton's method with the Newton decrement as stopping criterion.
- Implement BFGS and L-BFGS; understand the secant condition.
- Build a decision rule: which method for which problem.

## Key concepts
- Newton step `Δx_nt = −∇²f(x)⁻¹∇f(x)`; affine invariance; quadratic local convergence.
- Newton decrement `λ(x)² = ∇f ᵀ ∇²f⁻¹ ∇f`; stop when `λ²/2 ≤ ε`.
- Damped Newton phase vs. pure Newton phase.
- Secant equation `B_{k+1} s_k = y_k`; BFGS update; L-BFGS two-loop recursion (memory `m`).
- Gauss-Newton and Levenberg-Marquardt for nonlinear least squares.
- Method selection: cheap Hessian → Newton; large `n` → L-BFGS; residual structure → Gauss-Newton.

## Reading

- [Nocedal & Wright — Ch. 6 (quasi-Newton methods)](../resources/books/nocedal-wright-numerical-optimization.pdf#page=154)
- [Nocedal & Wright — Ch. 7 (large-scale unconstrained optimization, L-BFGS)](../resources/books/nocedal-wright-numerical-optimization.pdf#page=183)
- [Nocedal & Wright — Ch. 10 (least-squares problems)](../resources/books/nocedal-wright-numerical-optimization.pdf#page=264)
- [Boyd — Ch. 9.5 (Newton's method)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=498)

## Implement
- [ ] Newton with backtracking; report the two convergence phases.
- [ ] BFGS from scratch; L-BFGS two-loop recursion.
- [ ] Gauss-Newton on a curve-fitting problem.
- [ ] Benchmark table: iterations, function evals, wall time vs. `scipy.optimize.minimize`.

## Checklist
- [ ] Notes written
- [ ] Quadratic convergence observed (error squares each step near `x*`)
- [ ] Method-selection guide written in `notes.md`

---

Your own notes for this week go in `terms/<your-term>/notes/week-06.md`, not here.
This file is the shared plan — improve it if the course changes, but keep it general.
