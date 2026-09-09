# Week 2 — Mathematical Foundations

> Syllabus (TR): *Matematiksel temeller: normlar, gradyan, Taylor açılımı, karesel formlar; dışbükeyliğe ilk bakış; sayısal hesaplama ortamı*

## Goals
- Fluency with norms, inner products, gradients, Hessians, and quadratic forms.
- Use the first- and second-order Taylor expansion as the basis of every local method.
- First look at convexity; recognize positive (semi)definite matrices.

## Key concepts
- Norms: `‖x‖₁`, `‖x‖₂`, `‖x‖∞`; dual norms; norm balls.
- Gradient `∇f`, Hessian `∇²f`, Jacobian; directional derivative.
- Taylor: `f(x+p) ≈ f(x) + ∇f(x)ᵀp + ½ pᵀ∇²f(x) p`.
- Quadratic form `½xᵀQx − bᵀx`; `Q ≻ 0` ⇒ unique minimizer `x* = Q⁻¹b`.
- Condition number `κ(Q) = λ_max/λ_min` — this predicts gradient descent's speed in Week 5.
- Convex set / convex function, first-order and second-order conditions.

## Reading
- Nocedal & Wright — Ch. 2 (fundamentals of unconstrained optimization), Appendix A
- Boyd & Vandenberghe — Appendix A, Ch. 2.1-2.2, Ch. 3.1
- Pınar, *Dışbükeylik ve Optimizasyon* — early chapters (TR)

## Implement
- [ ] Numerical gradient (finite differences) and check it against an analytic gradient.
- [ ] Eigen-decomposition of a quadratic form; plot level sets for varying `κ`.
- [ ] Norm-ball visualizer for p = 1, 2, ∞.

## Checklist
- [ ] Notes written
- [ ] Gradient checker works (relative error < 1e-6)
- [ ] Can state the second-order condition for convexity from memory
