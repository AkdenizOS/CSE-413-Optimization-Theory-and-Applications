# From the basics to the midterm — concepts and simple calculations

No prior optimization study is assumed. Use alongside the
[interactive study route](https://akdenizos.org/lab/cse-413/midterm-review.html).
This is a study guide, not an instructor-issued exam or question prediction.

## What the evidence supports

The instructor's message shared by Efe emphasizes covered material, simple
calculations and what the methods are used for. A classmate reports decks 1–5
were covered and Newton from deck 6 was discussed with calculations; completion
of deck 6 is uncertain. The classmate's simplex prediction is not an instructor
guarantee. The written syllabus still lists W1–W7, so W7 remains an unresolved
coverage question, not an excluded topic.

The current term's syllabus sets the midterm at **30%** and permits **one
handwritten A4 formula sheet**. Exam duration and calculator permission have not
been verified. The EXAMPLE mock's conditions are practice assumptions.

## Source-to-study map

Page numbers below are physical PDF pages. W4's visible slide numbers skip 18–19;
use PDF page numbers for links.

| Deck | Pages | First-pass target | Existing Lab lesson |
|------|-------|-------------------|---------------------|
| [W1](../resources/2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Week_01.pdf#page=4) | 4–19 | Variables, objective, constraints; local/global; problem classes | modeling |
| [W2](../resources/2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Week_02.pdf#page=4) | 4–17 | Norms, gradient, Jacobian, Hessian, Taylor, positive definiteness | norms-gradients; hessian-convexity |
| W2 | 19–30 | Convexity tests, stable arithmetic, finite differences, conditioning | same lessons; numerical examples already present |
| [W3](../resources/2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Week_03.pdf#page=11) | 11–21 | Job-mix pivots, tableau interpretation, alternative optima/degeneracy | simplex; simplex-special |
| [W4](../resources/2026-2027-fall/27G_CSE413_5013_Optimization_Theory_Week_04.pdf#page=3) | 3–10 | Dual, complementary slackness, shadow price | lp-duality |
| W4 | 12–17 | RHS/objective ranges, simplex vs interior-point, data-center case | lp-sensitivity; study route |
| [W5](../resources/2026-2027-fall/27G_CSE413_5013_OptimizationTheory_Week05.pdf#page=4) | 4–12 | Scalar/2-D GD, step sizes, decrease-only backtracking | study route; gradient-descent |
| W5 | 15–20 | Rescaling, stopping, gradient checking, sensor fitting | study route; gradient-descent |
| [W6](../resources/2026-2027-fall/27G_CSE413_5013_OptimizationTheory_Week06.pdf#page=5) | 5–9, 14 | Scalar Newton, square roots, negative curvature | study route; newton-quasi-newton |
| W6 | 15–21 | Hessian cost, BFGS/L-BFGS purpose, method choice | study route; newton-quasi-newton |

W7 slides and Lab03–06 notebooks are not available in the resource folder. W5/W6 slides name full lab
notebooks, but their numerical datasets and complete experiments cannot be
reconstructed from those references alone.

## How to start from zero

Read the definition and learn the English name of each concept. Follow the
worked solution before expecting yourself to solve a new problem. Then close
the solution, reproduce the calculation on blank paper, and explain each step.
Use the linked full lesson when an idea is unfamiliar. Allow extra time for
paper practice; reading-time estimates are not a complete preparation budget.

## Work these examples on paper

On the first pass, use the checks as worked examples. Then cover them and try
each problem independently. Explain the purpose of each method in two
sentences as well as doing the arithmetic.

1. **Modeling:** maximize `3x1 + 4x2` subject to `x1+x2 ≤ 4`,
   `x1+3x2 ≤ 6`, `x ≥ 0`. Identify variables, parameters and feasible region.
   Check `(3,1)` and its objective.
2. **Foundations:** for `f=x²+xy+2y²` at `(1,2)`, find `f`, gradient and
   Hessian. Is `d=(-1,0)` a descent direction? Compare the Hessian of
   `g=x²+3xy+2y²` at its stationary origin.
3. **Simplex:** maximize `3x1+5x2` subject to `x1≤4`, `2x2≤12`,
   `3x1+2x2≤18`, `x≥0`. Add slacks and run two pivots. For every pivot show
   the reduced cost, eligible ratios and row operations; then read slack.
4. **Dual/prices:** write the preceding LP's dual and derive prices from
   complementary slackness. Would you buy a small amount of memory at 1.2 per
   unit, or accelerator at 0.2 per unit? Keep units and allowable ranges fixed.
5. **Sensitivity:** change memory capacity from 12 to 14, then to 20.
   When does the original shadow-price calculation stop being valid?
6. **Data-center application (W4 PDF p.17):** maximize `30x1+20x2` subject
   to `6x1+2x2≤60`, `3x1+3x2≤45`, `x1≤8`, `x≥0`. Solve with the first
   two constraints binding; check the third and find the resource prices.
7. **GD (W5 pp.6–8):** `(x−1)²`, start 5, step size 0.1, three updates.
   Then `x²+4y²`, start `(2,1)`, step size 0.1, one update. Explain what
   happens with step sizes 0.5 and 1 in the scalar example.
8. **Backtracking (W5 p.12):** `(x−3)²`, start 7, initial step size 1;
   repeatedly halve until the objective strictly decreases. State the
   difference between this slide's test and formal Armijo.
9. **Newton (W6 pp.8–9):** `f=x³/3−3x`, start 2, two updates using
   `x_new=x−f'/f''`. What happens starting at −1? Is zero slope enough?
10. **Method choice:** explain gradient vs Hessian vs learned curvature;
    why L-BFGS saves memory; and why fewer iterations need not mean less time.

### Checks

1. `(3,1)` is feasible, objective 13; continuous-variable LP unless an integer
   restriction is explicitly imposed.
2. `f=11`, gradient `(4,9)`, Hessian `[[2,1],[1,4]]` is PD; `gᵀd=−4`.
   The other Hessian is `[[2,3],[3,4]]`, determinant −1, so the origin is a saddle.
3. Initial slacks `(4,12,18)`. Enter `x2`, leave `s2` (ratios 6, 9);
   enter `x1`, leave `s3` (ratios 4, 2). Optimum `(2,6)`, value 36,
   slack `(2,0,0)`. Final `c_j−z_j` slack entries `(0,−1.5,−1)`.
4. Minimize `4y1+12y2+18y3`, subject to `y1+3y3≥3`,
   `2y2+2y3≥5`, `y≥0`. Prices `(0,1.5,1)` give dual value 36.
   Memory's marginal net gain is 0.3; accelerator's is −0.2.
5. At 14: `(4/3,7)`, value 39. Price 1.5 applies on `[6,18]`;
   at 20 the optimum value is 45, not 48. For nonnegative capacity,
   the value is `12+2.5b2` on `[0,6]`, `18+1.5b2` on `[6,18]`, then 45.
6. `(7.5,7.5)`, value 375, stock slack 0.5. Prices `(2.5,5,0)`;
   `60×2.5+45×5=375`. Purchase decisions also depend on unit costs.
7. Scalar: `5 → 4.2 → 3.56 → 3.048`. Two-dimensional: gradient `(4,8)`,
   new point `(1.6,0.2)`, objective `2.72`. Scalar α=0.5 solves in one
   step; α=1 oscillates `5 → −3 → 5`.
8. α=1 gives −1, objective 16 (unchanged, reject); α=0.5 gives 3,
   objective 0 (accept). Formal Armijo requires a specified amount of decrease,
   not just `f_new < f_old`. Check a stopping rule before trying strict decrease
   at zero gradient.
9. `2 → 7/4 → 97/56 ≈ 1.732143`. Negative start:
   `−1 → −2 → −1.75 → … → −√3`, a local maximum because `f''=2x<0`.
   On `x>0`, `+√3` is the minimum; on all real numbers this cubic is
   unbounded below. The method solves `f'=0`, not `f=0`.
10. GD uses gradient; Newton uses Hessian and a linear solve; BFGS learns
    curvature from gradient differences; L-BFGS stores only a few pairs.
    Dense Hessian/BFGS memory is quadratic in variable count, L-BFGS is `O(mn)`.

## Core material and further study

- The actual W5 deck uses simple scalar/2-D calculations and decrease-only
  backtracking. Armijo is in the syllabus; Wolfe/Goldstein and detailed rate
  proofs are supplementary depth.
- W6 teaches scalar Newton, square-root iterations, curvature risks and the
  BFGS/L-BFGS idea. It does not derive Newton decrement, BFGS matrix updates,
  L-BFGS two-loop recursion, Gauss–Newton or LM.
- W4 compares simplex and interior-point conceptually; it does not teach
  detailed dual-simplex pivots or Farkas proofs. Big-M/two-phase remain extended
  textbook review rather than a confirmed exam task.
- W3 uses `c_j−z_j`; W4 p.3 shows the opposite-sign z-row. Reverse the
  entering/stopping signs accordingly. Shadow prices are the *positive*
  slack entries in the W4 z-row, or the negatives of W3 reduced slack costs.
- W4 p.10's debugging shortcut needs a qualification: dual infeasibility
  alone does not prove primal unboundedness, since both can be infeasible.
- Finish the core calculations, then review the broad W1–W7 syllabus,
  especially any W7 material confirmed as taught. Do not infer that availability
  of a deck establishes full exam coverage.
