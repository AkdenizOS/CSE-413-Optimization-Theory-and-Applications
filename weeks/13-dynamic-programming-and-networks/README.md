# Week 13 — Discrete Optimization II: Dynamic Programming and Network Optimization

> Syllabus (TR): *Ayrık optimizasyon II — Dinamik programlama ve ağ optimizasyonu: Bellman ilkesi, Dijkstra, Bellman–Ford, A*, en büyük akış–en küçük kesit*

## Goals
- Apply Bellman's principle of optimality to decompose problems.
- Implement the core shortest-path and max-flow algorithms.
- See LP duality reappear as max-flow / min-cut.

## Key concepts
- Principle of optimality; state, stage, transition, value function.
- Bellman equation; forward vs. backward recursion; memoization vs. tabulation.
- Dijkstra (nonnegative weights, `O(E log V)`); Bellman-Ford (negative edges, cycle detection); A* (admissible + consistent heuristic).
- Max-flow: Ford-Fulkerson, Edmonds-Karp, Dinic; residual graph, augmenting path.
- Max-flow min-cut theorem = LP strong duality on the flow LP (link back to Week 4).
- Min-cost flow; network simplex; total unimodularity ⇒ LP relaxation is integral.

## Reading
- Winston — Ch. 8 (network models), Ch. 18-19 (deterministic dynamic programming)
- Winston — Ch. 7 (transportation, assignment, transshipment)
- Pınar, *Doğrusal Optimizasyondan Çıkış* (TR) — "Ağ Problemleri", "Çizge Kuramı", "En Kısa Yol Problemi", "Atama Problemi"

## Implement
- [ ] DP: knapsack, longest common subsequence, and one routing problem.
- [ ] Dijkstra, Bellman-Ford, A* on the same graph; compare nodes expanded.
- [ ] Edmonds-Karp max-flow; extract the min-cut and verify `max-flow = min-cut`.
- [ ] Formulate max-flow as an LP, solve with Week-3 simplex, and confirm the same value.

## Checklist
- [ ] Notes written
- [ ] Min-cut extracted correctly from the final residual graph
- [ ] Can explain why total unimodularity makes the LP relaxation exact
