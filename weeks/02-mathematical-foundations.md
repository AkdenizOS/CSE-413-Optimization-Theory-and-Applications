# Week 2 — Mathematical Foundations

> Syllabus (TR): *Matematiksel temeller: normlar, gradyan, Taylor açılımı, karesel formlar; dışbükeyliğe ilk bakış; sayısal hesaplama ortamı*

**Builds on:** [Week 1 · Introduction to Optimization: Modeling](01-introduction-and-modeling.md)
**Leads to:** [Week 3 · Linear Programming I: Geometry and the Simplex Method](03-linear-programming-simplex.md) · [Week 5 · Unconstrained Optimization I: Gradient Descent](05-unconstrained-gradient-descent.md) · [Week 8 · Convex Optimization I: Sets, Functions, Problem Hierarchy](08-convex-optimization-theory.md)

## Goals
- Fluency with norms, inner products, gradients, Hessians, and quadratic forms.
- Use the first- and second-order Taylor expansion as the basis of every local method.
- First look at convexity; recognize positive (semi)definite matrices.

## Key concepts
- Norms: `‖x‖₁`, `‖x‖₂`, `‖x‖∞`; dual norms; norm balls.
- Gradient `∇f`, Hessian `∇²f`, Jacobian; directional derivative.
- Taylor: `f(x+p) ≈ f(x) + ∇f(x)ᵀp + ½ pᵀ∇²f(x) p`.
- Quadratic form `½xᵀQx − bᵀx`; `Q ≻ 0` ⇒ unique minimizer `x* = Q⁻¹b`.
- Condition number `κ(Q) = λ_max/λ_min` — this predicts gradient descent's speed in [Week 5](05-unconstrained-gradient-descent.md).
- Convex set / convex function, first-order and second-order conditions.

## Reading

- [Nocedal & Wright — Ch. 2 (fundamentals of unconstrained optimization)](../resources/books/nocedal-wright-numerical-optimization.pdf#page=29)
- [Boyd — App. A.1 (norms), A.4 (derivatives), A.5 (linear algebra)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=647)
- [Boyd — Ch. 2.1 (affine and convex sets)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=35) · [Ch. 3.1 (basic properties)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=81)
- [Winston — Ch. 2 (basic linear algebra)](../resources/books/winston-operations-research.pdf#page=27)
- Pınar, *Dışbükeylik ve Optimizasyon* (TR) — "Dışbükey Kümeler", "Dışbükey Fonksiyonlar"

## Implement
- [ ] Numerical gradient (finite differences) and check it against an analytic gradient.
- [ ] Eigen-decomposition of a quadratic form; plot level sets for varying `κ`.
- [ ] Norm-ball visualizer for p = 1, 2, ∞.

## Checklist
- [ ] Notes written
- [ ] Gradient checker works (relative error < 1e-6)
- [ ] Can state the second-order condition for convexity from memory

## My notes

<!-- Lecture: what was actually covered. -->

<!-- Derivations worked out by hand. -->

<!-- Questions to ask the instructor. -->

<!-- Exam-worthy: formulas, conditions, algorithm steps. -->
