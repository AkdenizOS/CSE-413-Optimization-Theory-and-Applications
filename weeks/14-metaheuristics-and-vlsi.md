# Week 14 — Metaheuristics and VLSI Applications

> Syllabus (TR): *Metasezgisel yöntemler ve VLSI uygulamaları: benzetimli tavlama, genetik algoritmalar, parçacık sürüsü, yapay arı kolonisi (ABC); yerleşim ve kapı boyutlandırma*

**Builds on:** [Week 8 · Convex Optimization I: Sets, Functions, Problem Hierarchy](08-convex-optimization-theory.md) · [Week 9 · Convex Optimization II: CVXPY and Disciplined Convex Programming](09-convex-optimization-cvxpy.md)

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

- Karaboga (2005), TR06 — [original ABC paper](../resources/papers/karaboga-2005-abc-tr06.pdf)
- [ABC pseudocode](../resources/papers/karaboga-abc-pseudocode.pdf) — implement from this
- [ABC step-by-step trace](../resources/papers/karaboga-abc-step-by-step.pdf) — debug against this
- [Boyd — Ch. 4.5 (geometric programming) — gate sizing is a GP](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=174)
- Karaboga & Basturk (2007), J. Global Optimization 39(3) — paywalled, get via the university's Springer subscription

## Implement
- [ ] SA, GA, PSO, ABC behind one common `optimize(f, bounds, budget, seed)` interface.
- [ ] Benchmark suite: Rastrigin, Ackley, Rosenbrock, Griewank.
- [ ] Equal-budget comparison, 30 seeds, boxplots + Wilcoxon signed-rank test.
- [ ] VLSI: gate sizing as a GP in CVXPY (provably optimal) vs. a metaheuristic — quantify the gap.

## Checklist
- [ ] Notes written
- [ ] Comparison uses equal budget and ≥30 seeds
- [ ] Gate sizing GP solution beats or matches the heuristic, and I can say why

---

Your own notes for this week go in `terms/<your-term>/notes/week-14.md`, not here.
This file is the shared plan — improve it if the course changes, but keep it general.
