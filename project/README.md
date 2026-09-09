# Term Project (25%)

**Proposal due:** TBD · **Report + presentation:** TBD

The project is where learning outcome **Ö04** is assessed: design an end-to-end
optimization solution to a real computer-engineering problem under realistic
constraints, and communicate it in a written report and an oral presentation.

## Requirements from the syllabus

1. Model a real problem (decision variables, objective, constraints) — **Ö01**.
2. Implement the solution method; use modern tooling where appropriate — **Ö02**.
3. Either prove optimality (duality / KKT) **or** measure heuristic quality with a
   proper experiment design: equal computational budget, multiple random seeds,
   statistical distributions — **Ö03**.
4. Written report + oral presentation — **Ö04**, **P07**.

## Candidate topics

| Domain | Problem | Method family |
|--------|---------|---------------|
| ML | Sparse model selection / LASSO path at scale | Proximal, FISTA |
| ML | Hyperparameter or architecture search | Bayesian opt / metaheuristic |
| Networks | Traffic engineering, multi-commodity flow routing | LP / min-cost flow |
| Networks | Base-station or server placement | Integer programming |
| VLSI | Gate sizing | Geometric programming (convex, provable) |
| VLSI | Standard-cell placement | Simulated annealing / GA |
| Resources | Job-shop or course scheduling | MIP + branch and bound |
| Portfolio | Risk-constrained allocation | QP / SOCP |

A strong project picks a problem with **both** a convex formulation (provable
optimum) and a heuristic approach, then quantifies the gap between them.

## Structure

```
project/
├── README.md      this file
├── proposal.md    problem, data, method, evaluation plan
├── report/        final written report
├── src/           implementation
├── data/
└── results/       figures, tables, raw experiment output
```

## Checklist

- [ ] Topic chosen and approved by the instructor
- [ ] Proposal written
- [ ] Problem formulated mathematically
- [ ] Baseline implemented
- [ ] Main method implemented
- [ ] Experiments run (equal budget, ≥30 seeds if stochastic)
- [ ] Optimality certificate or honest statistical comparison
- [ ] Report written
- [ ] Presentation slides prepared
- [ ] Rehearsed
