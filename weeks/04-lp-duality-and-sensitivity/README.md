# Week 4 — Linear Programming II: Duality and Sensitivity

> Syllabus (TR): *Doğrusal programlama II: dualite, gölge fiyatlar, tamamlayıcı gevşeklik ve duyarlılık analizi*

## Goals
- Construct the dual of any LP mechanically.
- Interpret dual variables as shadow prices.
- Use complementary slackness as an optimality certificate.

## Key concepts
- Primal-dual pair; weak duality `dᵀy ≤ cᵀx`; strong duality for feasible LPs.
- Complementary slackness: `y_i (a_iᵀx − b_i) = 0` — the certificate you will reuse in Week 7.
- Shadow price = rate of change of `p*` per unit of resource `b_i`.
- Sensitivity/ranging: how far can `c` or `b` move before the basis changes.
- Dual simplex; farkas lemma / certificates of infeasibility.

## Reading
- Winston — Ch. 5 (sensitivity analysis: applied approach), Ch. 6 (sensitivity analysis and duality)
- Pınar, *Doğrusal Optimizasyondan Çıkış* (TR) — "Eşterslik" (duality), "İkili Seçenek Teoremleri" (theorems of alternatives)
- Boyd & Vandenberghe — Ch. 5.1-5.2 (LP duality as a special case)
- Boyd slides — Section 5 "Duality" (`bv_cvxslides.pdf`, p. 2815+ of text)

## Implement
- [ ] Automatic primal → dual transformer for LPs in any form.
- [ ] Extract shadow prices from your Week-3 simplex tableau and verify against SciPy duals.
- [ ] Sensitivity report: allowable ranges for `c` and `b`.

## Checklist
- [ ] Notes written
- [ ] Verified `cᵀx* = bᵀy*` numerically
- [ ] Can explain a shadow price to a non-technical person
