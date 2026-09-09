# Week 11 — Optimization in Machine Learning and Deep Learning

> Syllabus (TR): *Makine öğrenmesi ve derin öğrenmede optimizasyon: deneysel risk minimizasyonu, geri yayılım = otomatik türev, eğitim reçeteleri, model sıkıştırma*

## Goals
- Frame learning as empirical risk minimization (ERM).
- See backpropagation as reverse-mode automatic differentiation, and implement a tiny autodiff engine.
- Know practical training recipes and compression as a constrained optimization problem.

## Key concepts
- ERM: `min_θ (1/n) Σ ℓ(f_θ(xᵢ), yᵢ) + λR(θ)`; generalization vs. optimization error.
- Computational graph; forward mode vs. reverse mode AD; why reverse mode is cheap for `ℝⁿ → ℝ`.
- Backprop = chain rule over the graph in reverse topological order.
- Non-convexity of deep nets: saddle points, flat minima, batch norm's effect on the loss landscape.
- Training recipes: initialization, warmup, gradient clipping, weight decay vs. L2.
- Model compression: pruning (ℓ0/ℓ1 relaxation), quantization (as integer programming), distillation.

## Reading

- [Nocedal & Wright — Ch. 8 (calculating derivatives = automatic differentiation)](../../resources/books/nocedal-wright-numerical-optimization.pdf#page=212)
- Goodfellow et al., *Deep Learning* — Ch. 8 (optimization for training deep models)
- PyTorch autograd docs

## Implement
- [ ] Micro-autograd: scalar `Value` class with `+`, `*`, `tanh`, and `.backward()`.
- [ ] Train a 2-layer MLP with it; verify gradients against PyTorch.
- [ ] Magnitude pruning experiment: accuracy vs. sparsity curve.

## Checklist
- [ ] Notes written
- [ ] Autograd gradients match PyTorch to 1e-6
- [ ] Can explain why reverse-mode AD costs ~2× the forward pass
