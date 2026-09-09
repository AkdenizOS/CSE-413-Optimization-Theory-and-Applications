# Week 12 — Discrete Optimization I: Integer Programming

> Syllabus (TR): *Ayrık optimizasyon I — Tamsayılı programlama: modelleme teknikleri (büyük-M, ya-ya da), LP gevşetmesi, dal-sınır, kesme düzlemleri*

## Goals
- Model logical conditions with binary variables.
- Implement branch-and-bound on top of your Week-3 LP solver.
- Understand LP relaxation quality and cutting planes.

## Key concepts
- Binary modeling: big-M, either/or, if-then, fixed charge, indicator constraints.
- LP relaxation gives a bound; integrality gap.
- Branch and bound: branching variable selection, node bounding, pruning, incumbent.
- Cutting planes: Gomory cuts, cover inequalities; branch-and-cut.
- Classic problems: knapsack, set cover, assignment, TSP, facility location, bin packing.
- NP-hardness — this is where "prove optimality" starts getting expensive.

## Reading
- Winston — Ch. 9 (integer programming)
- Taha, *Yöneylem Araştırması* — integer programming chapter (TR)

## Implement
- [ ] Branch-and-bound for binary IPs using your simplex from Week 3.
- [ ] Knapsack: DP vs. B&B vs. LP relaxation bound.
- [ ] One Gomory cut round; measure gap reduction.
- [ ] Model + solve a real instance with PuLP/CBC; compare node counts.

## Checklist
- [ ] Notes written
- [ ] B&B returns provably optimal solutions on ≥20 random instances
- [ ] Can write a big-M constraint correctly without looking it up
