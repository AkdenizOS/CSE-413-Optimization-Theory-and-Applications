# Week 10 — Stochastic Gradient Methods

> Syllabus (TR): *Stokastik gradyan yöntemleri: SGD, momentum, Adam, öğrenme oranı çizelgeleri, proksimal yöntemler/ISTA*

## Goals
- Implement SGD and its main variants from scratch.
- Understand why noise changes the convergence story vs. Weeks 5-6.
- Implement a proximal method (ISTA/FISTA) for nonsmooth regularizers.

## Key concepts
- Finite-sum objective `f(x) = (1/n) Σ fᵢ(x)`; minibatch gradient as an unbiased estimator.
- SGD convergence `O(1/√k)`; why a decaying step size is required (Robbins–Monro).
- Momentum / heavy ball; Nesterov acceleration.
- Adaptive methods: AdaGrad, RMSProp, Adam (bias correction), AdamW.
- Learning-rate schedules: step decay, cosine, warmup.
- Proximal operator `prox_{th}(v)`; soft-thresholding; ISTA and FISTA for `‖x‖₁`.

## Reading

- [Nocedal & Wright — Ch. 7 (large-scale optimization)](../../resources/books/nocedal-wright-numerical-optimization.pdf#page=183)
- Kingma & Ba, *Adam* (2014); Beck & Teboulle, *FISTA* (2009)
- Boyd, Stanford EE364b — subgradient and proximal method notes

## Implement
- [ ] SGD, momentum, Nesterov, AdaGrad, RMSProp, Adam — one common interface.
- [ ] Logistic regression on a real dataset; compare optimizers on equal budget.
- [ ] ISTA + FISTA for LASSO; compare against the CVXPY solution from Week 9.

## Checklist
- [ ] Notes written
- [ ] Fair comparison: same seeds, same epoch budget, multiple runs
- [ ] Can explain Adam's bias correction term
