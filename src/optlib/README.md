# optlib — From-Scratch Implementations

The syllabus requires every method to be implemented from scratch in Python.
Anything reused across more than one week lives here as a proper module; one-off
experiments stay in `weeks/NN-*/code/`.

Planned modules, added as each week is covered:

| Module | Week | Contents |
|--------|------|----------|
| `simplex.py` | 3, 4, 12, 13 | Tableau simplex, two-phase, duals |
| `linesearch.py` | 5, 6 | Backtracking (Armijo), Wolfe conditions |
| `descent.py` | 5, 6 | Gradient descent, Newton, BFGS, L-BFGS, Gauss-Newton |
| `kkt.py` | 7, 9 | KKT residual checker, duality gap |
| `stochastic.py` | 10, 11 | SGD, momentum, AdaGrad, RMSProp, Adam, ISTA/FISTA |
| `autodiff.py` | 11 | Scalar reverse-mode autodiff engine |
| `branch_bound.py` | 12 | Branch and bound on top of `simplex.py` |
| `graphs.py` | 13 | Dijkstra, Bellman-Ford, A*, Edmonds-Karp |
| `metaheuristics.py` | 14 | SA, GA, PSO, ABC behind one interface |
| `benchmarks.py` | 5, 6, 14 | Rosenbrock, Rastrigin, Ackley, Griewank |

## Rules

- Every implementation is validated against a reference (SciPy, CVXPY, PuLP, NetworkX).
- Stochastic methods take an explicit `seed`; comparisons use equal evaluation budgets.
- No method is added here until it is actually needed by two or more weeks.
