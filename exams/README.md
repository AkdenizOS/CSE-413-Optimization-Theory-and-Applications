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
down the pattern. See [CSE 435's exam analysis](https://github.com/AkdenizOS/CSE-435-Formal-Languages-and-Automata-/blob/main/exams/README.md)
for what that looks like — its midterm shape has not changed since 2020.

## Midterm (30% in Fall 2026–2027)

**Date:** not independently confirmed here; the Lab countdown uses 4 November 2026,
10:30. **Written syllabus scope:** weeks 1–7; week 8 assessment;
**one handwritten A4 formula sheet allowed**.
The [instructor's current syllabus](../resources/2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Syllabus.pdf#page=1)
sets 30%; the general department syllabus's 25% is not the current term's weight.
Duration, calculator policy and exact question format remain unconfirmed.

### Exam guidance and scope

- In the instructor's message shared by Efe, the guidance is covered material,
  simple calculations, and what the methods are used for. This does not specify
  a question count or guarantee any particular topic.
- A classmate reports decks 1–5 were taught and Newton from deck 6 was discussed
  with calculations. How much of deck 6 was completed is uncertain.
- The classmate's “simplex will definitely appear” is a peer prediction, not a
  direct instructor guarantee. Prioritize simplex for practice without calling
  it a confirmed exam question.
- Course resources include decks 1–6, syllabus and Lab01–02. Deck 7 and
  Lab03–06 notebooks are unavailable; deck 6 names a full Week06_Lab notebook which was not supplied.
- The syllabus includes W7. The messages do not establish that it was taught;
  keep KKT/water-filling/barrier as scope-dependent review, not excluded topics.

### Preparation route

No prior optimization study is assumed. Start with the [instructor-aligned study guide](midterm-review.md) and the
[interactive review](https://akdenizos.org/lab/cse-413/midterm-review.html).
For every method: learn the concept, follow a worked example, then close the
solution and reproduce the calculation. Explain what the result means. Reading
time estimates do not include all the time needed to learn and practise.

| Priority | Material | Practice |
|----------|----------|----------|
| Core | W1 modeling | Variables, objective, constraints, feasible/infeasible/unbounded, local/global |
| Core | W2 foundations | Norms; gradient/Hessian; small Taylor model; definiteness and convexity |
| Core | W3 simplex | Job-mix standard form, two pivots, ratio tests, optimal point and slack |
| Core | W4 duality/sensitivity | Build the dual; complementary slackness; shadow prices and valid ranges |
| Core | W5 GD | Three scalar updates; one 2-D update; simple backtracking; scaling and stopping |
| Review basic examples | W6 Newton | Slope/bend update, square-root iterations, negative curvature; BFGS/L-BFGS purpose |
| Confirm coverage | W7 | KKT, water-filling, barrier; not established as taught by the shared messages |
| Extension | Textbook detail | Big-M/two-phase, detailed dual simplex/Farkas, Wolfe/Goldstein, decrement, BFGS matrix update, Gauss–Newton/LM |

### Must be able to do by hand first

- [ ] Formulate a small LP and classify the variables and feasible set.
- [ ] Compute norms, a gradient and Hessian; distinguish a minimum from a saddle.
- [ ] Run the job-mix simplex pivots and read the optimum and unused resources.
- [ ] Recognize both `c_j − z_j` (W3) and the opposite-sign z-row (W4).
- [ ] Construct the dual and obtain prices using complementary slackness.
- [ ] Use a shadow price only within its range and interpret a purchase decision.
- [ ] Calculate three GD steps and a backtracking accept/reject sequence.
- [ ] Explain rescaling, gradient checking and practical stopping rules.
- [ ] Calculate two scalar Newton steps; check curvature and domain.
- [ ] Explain why BFGS uses gradient differences and L-BFGS saves memory.

After these, revisit the full syllabus topics and the extended
[formula sheet](https://akdenizos.org/lab/cse-413/formula-sheet.html).
The old EXAMPLE paper is a broad self-study mock. Its 90-minute duration,
calculator permission and closed-notes instructions are invented practice
conditions, not actual exam policy; the current syllabus allows the A4 sheet.

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
