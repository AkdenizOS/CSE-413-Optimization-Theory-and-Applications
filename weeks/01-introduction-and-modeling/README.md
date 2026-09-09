# Week 1 — Introduction to Optimization: Modeling

> Syllabus (TR): *Optimizasyona giriş: modelleme, karar değişkenleri, amaç fonksiyonu, kısıtlar; mühendislikte optimizasyon problemleri*

## Goals
- Translate a verbal engineering problem into `min f(x) s.t. x ∈ C`.
- Identify decision variables, objective, constraints, and feasible set.
- Classify a problem: continuous vs. discrete, convex vs. non-convex, network-structured.

## Key concepts
- Standard form of an optimization problem; feasible set, optimal value `p*`, optimal point `x*`.
- Local vs. global optimum; infeasible and unbounded problems.
- Why problem *structure* (not size) decides solvability.
- Taxonomy: LP, QP, SOCP, SDP, convex, IP/MIP, DP, heuristic-only.

## Reading
- Boyd & Vandenberghe, *Convex Optimization* — Ch. 1 (`resources/books/boyd-vandenberghe-convex-optimization.pdf`)
- Boyd slides — Section 1 "Introduction" (`resources/slides/bv_cvxslides.pdf`, p. 6+)
- Winston, *Operations Research* — Ch. 1-2 (modeling, intro to LP)

## Implement (Python, from scratch)
- [ ] Set up the environment (`requirements.txt`), verify `numpy`, `scipy`, `matplotlib`.
- [ ] Model + solve the Boyd illumination problem (lamp powers) by brute force / least squares, and compare.
- [ ] Plot a 2-variable feasible region and level curves of the objective.

## Checklist
- [ ] Lecture attended / slides read
- [ ] Notes written in `notes.md`
- [ ] Code committed under `code/`
- [ ] Self-test: can I write down the standard form of 3 problems from my own field?
