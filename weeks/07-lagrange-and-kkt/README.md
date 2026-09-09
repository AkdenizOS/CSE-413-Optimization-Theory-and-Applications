# Week 7 — Lagrange Multipliers and KKT Conditions

> Syllabus (TR): *Lagrange çarpanları ve KKT koşulları: eniyilik sertifikaları, dualite bağlantısı; su doldurma problemi*

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
- Sensitivity: `λ*` = shadow price of constraint `i` (same idea as Week 4).

## Reading
- Boyd & Vandenberghe — Ch. 5 (all), especially 5.5 (optimality conditions) and Example 5.2 (water-filling)
- Nocedal & Wright — Ch. 12 (theory of constrained optimization)

## Implement
- [ ] Water-filling: closed-form bisection on `ν` vs. CVXPY solution.
- [ ] KKT residual checker: given `(x, λ, ν)`, report violation of each of the 4 conditions.
- [ ] Dual function plot for a small problem; visualize the duality gap.

## Checklist
- [ ] Notes written
- [ ] KKT checker validates solutions from Weeks 3-6
- [ ] Can derive water-filling on paper without notes
