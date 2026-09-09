# Week 5 — Unconstrained Optimization I: Gradient Descent

> Syllabus (TR): *Kısıtsız optimizasyon I: gradyan iniş, adım seçimi (Armijo/geri izleme), yakınsama hızları ve koşul sayısı*

## Goals
- Implement gradient descent with a principled step-size rule.
- Prove/observe convergence rates and connect them to the condition number.

## Key concepts
- Descent direction; steepest descent in a general norm.
- Exact line search vs. backtracking (Armijo) line search: parameters `α ∈ (0, 0.5)`, `β ∈ (0,1)`.
- Wolfe conditions (sufficient decrease + curvature).
- Convergence: linear rate `((κ−1)/(κ+1))²` for quadratics; `L`-smoothness and `μ`-strong convexity.
- Why ill-conditioning (`κ ≫ 1`) makes GD zig-zag.

## Reading
- Nocedal & Wright — Ch. 3 (line search methods)
- Boyd & Vandenberghe — Ch. 9.1-9.3
- Boyd slides — Section 9 "Unconstrained minimization"

## Implement
- [ ] `gradient_descent` with fixed step, exact line search, and backtracking.
- [ ] Rosenbrock and ill-conditioned quadratics as test problems.
- [ ] Convergence plot: `log(f(x_k) − p*)` vs. `k` for several `κ`.

## Checklist
- [ ] Notes written
- [ ] Observed linear rate matches the theoretical bound
- [ ] Backtracking implemented without any library helper
