# Week 4 — Linear Programming II: Duality and Sensitivity

> Syllabus (TR): *Doğrusal programlama II: dualite, gölge fiyatlar, tamamlayıcı gevşeklik ve duyarlılık analizi*

**Builds on:** [Week 3 · Linear Programming I: Geometry and the Simplex Method](03-linear-programming-simplex.md)
**Leads to:** [Week 7 · Lagrange Multipliers and KKT Conditions](07-lagrange-and-kkt.md) · [Week 13 · Discrete Optimization II: Dynamic Programming and Network Optimization](13-dynamic-programming-and-networks.md)

## Goals
- Construct the dual of any LP mechanically.
- Interpret dual variables as shadow prices.
- Use complementary slackness as an optimality certificate.

## Key concepts
- Primal-dual pair; weak duality `dᵀy ≤ cᵀx`; strong duality for feasible LPs.
- Complementary slackness: `y_i (a_iᵀx − b_i) = 0` — the certificate you will reuse in [Week 7](07-lagrange-and-kkt.md).
- Shadow price = rate of change of `p*` per unit of resource `b_i`.
- Sensitivity/ranging: how far can `c` or `b` move before the basis changes.
- Dual simplex; farkas lemma / certificates of infeasibility.

## Reading

- [Winston — Ch. 5 (sensitivity analysis: an applied approach)](../resources/books/winston-operations-research.pdf#page=243)
- [Winston — Ch. 6 (sensitivity analysis and duality)](../resources/books/winston-operations-research.pdf#page=278)
- [Boyd — Ch. 5.1 (the Lagrange dual function)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=229) · [5.2 (the dual problem)](../resources/books/boyd-vandenberghe-convex-optimization.pdf#page=237)
- Pınar, *Doğrusal Optimizasyondan Çıkış* (TR) — "Eşterslik", "İkili Seçenek Teoremleri"

## Implement
- [ ] Automatic primal → dual transformer for LPs in any form.
- [ ] Extract shadow prices from your [Week 3](03-linear-programming-simplex.md) simplex tableau and verify against SciPy duals.
- [ ] Sensitivity report: allowable ranges for `c` and `b`.

## Checklist
- [ ] Notes written
- [ ] Verified `cᵀx* = bᵀy*` numerically
- [ ] Can explain a shadow price to a non-technical person

## My notes

<!-- Lecture: what was actually covered. -->

<!-- Derivations worked out by hand. -->

<!-- Questions to ask the instructor. -->

<!-- Exam-worthy: formulas, conditions, algorithm steps. -->
