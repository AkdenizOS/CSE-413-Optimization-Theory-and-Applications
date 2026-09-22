# Exams

Past papers sit in this folder as `<year>-<type>.pdf`. Below: what has been
collected so far, then the midterm and final preparation checklists.

## Past papers

No papers from previous cohorts have been collected for this course yet.

[`EXAMPLE/`](EXAMPLE/) holds a self-study practice midterm covering weeks 1-7:
[`midterm.pdf`](EXAMPLE/midterm.pdf) and its [answer key](EXAMPLE/midterm-answers.pdf).
It was not issued by the instructor and says nothing about the real exam's format.
The `.html` files next to the PDFs are the editable sources; re-export with Chrome's
print-to-PDF.

### Adding a paper

Name it after the academic year it was sat, directly in this folder:

```
exams/2026-2027-midterm.pdf
exams/2026-2027-final.pdf
```

Use `2026-2027-final-answered-<surname>.pdf` when it is somebody's graded answers rather
than a blank paper. Exam papers live here regardless of whose they are — they are
study material, and this is where anyone preparing for an exam looks. Only work
you produced yourself goes elsewhere: assignments and the project under
`assignments/<term>-<you>/`, notes in your own section of each week file.

Once a few years have accumulated, the useful thing is to read them all and write
down the pattern. See [CSE 435's exam analysis](https://github.com/AkdenizOS/CSE-435-Formal-Languages-and-Automata-/blob/main/docs/exam-patterns.md)
for what that looks like — its midterm shape has not changed since 2020.

## Midterm (25%)

**Date:** TBD · **Scope:** TBD (expect weeks 1-7)

### Likely scope

| Week | Topic | Confidence |
|------|-------|-----------|
| 1 | Modeling, problem classification | high |
| 2 | Norms, gradient, Taylor, quadratic forms, convexity basics | high |
| 3 | LP geometry, simplex tableau by hand | high |
| 4 | Duality, shadow prices, complementary slackness, sensitivity | high |
| 5 | Gradient descent, backtracking, convergence rate, condition number | high |
| 6 | Newton, BFGS, L-BFGS, Gauss-Newton | medium |
| 7 | Lagrange, KKT, water-filling | medium |

### Must be able to do by hand

- [ ] Convert any LP to standard form and build its dual.
- [ ] Run 2-3 simplex pivots on a tableau, including the ratio test.
- [ ] State complementary slackness and use it to verify a candidate solution.
- [ ] Write the backtracking line search algorithm.
- [ ] Derive the Newton step and the Newton decrement.
- [ ] Write all four KKT conditions and apply them to a small problem.
- [ ] Derive water-filling.

### Study log
<!-- What was reviewed and when. -->

### Practice problems
<!-- Links to worked exercises in weeks/*/ and the textbooks. -->

## Final Exam (40%)

**Date:** TBD · **Scope:** TBD (expect comprehensive, weeks 1-14)

### Likely scope

Everything from the midterm, plus:

| Week | Topic |
|------|-------|
| 8 | Convex sets/functions, convexity-preserving operations, LP/QP/SOCP/SDP hierarchy |
| 9 | DCP rules, CVXPY formulation, reading dual variables |
| 10 | SGD, momentum, Adam, learning-rate schedules, ISTA/FISTA |
| 11 | ERM, backprop as reverse-mode AD, training recipes, compression |
| 12 | Big-M modeling, LP relaxation, branch and bound, cutting planes |
| 13 | Bellman's principle, Dijkstra/Bellman-Ford/A*, max-flow min-cut |
| 14 | SA, GA, PSO, ABC; experiment design; VLSI gate sizing as a GP |

### Must be able to do by hand

- [ ] Prove a set or function is convex using the standard operations.
- [ ] Classify a problem into LP / QP / SOCP / SDP.
- [ ] Explain why a given CVXPY expression violates DCP and fix it.
- [ ] Write the Adam update including bias correction.
- [ ] Model a logical condition with big-M binaries.
- [ ] Run a branch-and-bound tree on a small knapsack.
- [ ] Trace Dijkstra and Bellman-Ford; extract a min-cut from a residual graph.
- [ ] Describe SA, GA, PSO, and ABC operators and their control parameters.
- [ ] Design a fair comparison between a heuristic and an exact method.

### Study log
