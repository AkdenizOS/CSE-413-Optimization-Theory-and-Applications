# Week 14 — Metaheuristics and VLSI Applications

> Syllabus (TR): *Metasezgisel yöntemler ve VLSI uygulamaları: benzetimli tavlama, genetik algoritmalar, parçacık sürüsü, yapay arı kolonisi (ABC); yerleşim ve kapı boyutlandırma*

## Goals
- Implement SA, GA, PSO, and ABC from scratch.
- Design an *honest* experiment when optimality cannot be proven (course outcome Ö03).
- Apply a metaheuristic to VLSI placement and gate sizing.

## Key concepts
- Exploration vs. exploitation; no-free-lunch theorem.
- Simulated annealing: Metropolis criterion, cooling schedule, acceptance ratio.
- Genetic algorithms: encoding, selection (tournament/roulette), crossover, mutation, elitism.
- PSO: velocity update, inertia weight `w`, cognitive `c₁` / social `c₂` coefficients.
- ABC (Karaboğa): employed / onlooker / scout bees, limit parameter, fitness-proportional selection.
- Experimental protocol: **equal budget** (same #evaluations), **multiple seeds** (≥30 runs), report median/IQR and a statistical test — not a single lucky run.
- VLSI: placement as quadratic/nonconvex assignment; gate sizing as a geometric program (convex! — see Boyd Ch. 4.5).

## Reading
- Karaboğa, *Yapay Zeka Optimizasyon Algoritmaları* (TR) — primary source for ABC
- Boyd & Vandenberghe — Ch. 4.5 (geometric programming), Ch. 8; slides "Geometric programming"
- Boyd et al., *Digital circuit optimization via geometric programming* (2005)

## Implement
- [ ] SA, GA, PSO, ABC behind one common `optimize(f, bounds, budget, seed)` interface.
- [ ] Benchmark suite: Rastrigin, Ackley, Rosenbrock, Griewank.
- [ ] Equal-budget comparison, 30 seeds, boxplots + Wilcoxon signed-rank test.
- [ ] VLSI: gate sizing as a GP in CVXPY (provably optimal) vs. a metaheuristic — quantify the gap.

## Checklist
- [ ] Notes written
- [ ] Comparison uses equal budget and ≥30 seeds
- [ ] Gate sizing GP solution beats or matches the heuristic, and I can say why
