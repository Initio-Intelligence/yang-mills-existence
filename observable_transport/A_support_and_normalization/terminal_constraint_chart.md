# The terminal average constraints have a polynomial local section

This note constructs a section for the fixed terminal average map on the promoted raw list. It leaves the terminal deltas exact and accounts for their coarea factor. It concerns the actual first-reset prepared geometry, where the old finest cells lie strictly inside the core which is integrated out. It does not identify the full restored density, its positive energy, or all of its cutoff completions.

## 1. Only the last logarithmically many scales meet a terminal footprint

Put `n=k−N_0+1`, with `N_0=1+O(log_L R)`, as in LFR I printed pp.191–192. The n-scale MR_n cubes have current physical size M. Let C be the next-grid cover of all earlier ancestors. The quiet construction and the definitions of the final inner region and prepared core imply the safe inclusion

\[
 C+B_{4M}\subset\Lambda.
 \tag{TQ.1}
\]

Every earlier old region `Z_j`, j≤n−1, lies in C. This is an inclusion of parallel sets, not an assertion that erosion commutes with arbitrary unions. The source derivation is recorded in the terminal-footprint lemma of the support analysis: CMP119 (3.5), the eight-layer cover, LFR I (1.10), (1.73), and the one-M enlargement defining Λ.

The full two-block footprint of a current average, including a crossing bond, has fixed current diameter. Choose the source M larger than that diameter and the additional fixed interface constants. A terminal average on `Y\Lambda` then cannot see promoted cells at levels below `k−N_0`, up to a fixed collar index. Consequently all its nontrivial variable dependence lies in at most

\[
 m\le N_0+C_L=O(\log R)
 \tag{TQ.2}
\]

ordinary scale changes. The arbitrary early depth N=R remains inside Λ and is absent from this terminal inversion. A fixed logarithmic enlargement of the exposed collar changes (TQ.2) by at most another `O(log log R)`.

The retained outer entries are held fixed. A terminal constraint that is already determined wholly by those entries is redundant and is not counted as a new constraint. The nonredundant constraints have their actual variable two-block footprints in the available collar. This is the same incidence convention as the ordinary source constraint solve.

## 2. One exceptional bond gives an exact one-step section

For each oriented coarse bond c choose the actual exceptional fine bond b_0(c) of CMP119 (1.14)–(1.15). It crosses the common face of the two averaging blocks of c. The averaging footprint of c contains b_0(c), but contains no b_0(c′) for a distinct coarse bond c′: such a bond crosses a different pair of blocks, whereas all the remaining averaging paths stay inside the two blocks of c. Internal axial tree bonds are not among these face-crossing exceptional bonds.

Freeze every other fine entry at a real regular baseline W_*. In local Lie coordinates the one-step average at c is an analytic function of the single exceptional entry. At a flat baseline, (125) and the factor L in (122) of CMP98 give

\[
 D_{b_0(c)}\log\mathcal M(W)_c=L^{1-d}I.
 \tag{TQ.3}
\]

Indeed b_0(c) is traversed by L starting points of the translated path, each with the raw-angle weight `L^{-d}`. The actual regular-baseline derivative differs from (TQ.3) by `O(C_L ε)`, in a local block gauge. The source real regularity ceiling can be chosen small compared with this fixed L-dependent number. Therefore its inverse has norm at most a fixed C_L, uniformly in the number of blocks and in the absolute scale.

The analytic implicit-function theorem, or the explicit exceptional-bond construction of the source, yields an exact section

\[
 w_c\longmapsto W_{b_0(c)}(w_c),\qquad
 \mathcal M(W(w))_c=w_c,
 \tag{TQ.4}
\]

on a fixed small relative group ball. It leaves the other fine entries unchanged. Its first derivative and its inverse-coordinate Jacobian have fixed L-dependent bounds, and it has a fixed holomorphic radius in relative angles. Different c can be solved simultaneously because their exceptional entries are distinct and the dependence just described is diagonal across c.

This construction is a section of the actual nonlinear average. It is not the linear replacement `QCA=0`. It is also not a claim that the Haar/coarea determinant is one.

## 3. Descend only through the terminal collar

At the terminal level prescribe the nearby target averages and leave all other target entries at their baseline values. A nonredundant terminal c is not already a fixed raw current entry of the master shell. By the aligned incidence convention its adjacent averaging blocks then lie in the finer complement inside Y. Its chosen exceptional descendant is either an actual variable entry of a lower master shell, in which case stop on that branch, or lies again in the finer complement, in which case continue the same one-step construction. The terminal-footprint bound ensures that every branch stops within m levels. No leaf is a fixed exterior variable. This recursive version avoids changing a master entry that was already prescribed at a coarser level. Other coarse readouts stay fixed by the unique-exceptional-bond footprint property in Section 2.

Apply (TQ.4) backward on these branches. At each stage, only the actual exceptional entries needed for that stage change. Their averaging footprints and the nested selected exceptional positions lie in a fixed current enlargement of the original terminal footprint: the physical widths add as `Σ_{j≤k} L^{j-k}`, not as m current block widths. The margin (TQ.1) contains this enlargement and keeps it away from all older finer cells.

Let W_j(w) denote the resulting consistent fields on the intermediate grids. They satisfy their literal chronological identities

\[
 \mathcal M_j(W_j(w))=W_{j+1}(w).
 \tag{TQ.5}
\]

Assign these values to the promoted master entries of native level at least k−m in this collar. Leave the earlier master entries and all fixed exterior data unchanged. All coarser redundant readouts are assigned by (TQ.5). The exact determination lemma PM.1 then gives a section S of the terminal readout Φ:

\[
 \Phi(S(w))=w.
 \tag{TQ.6}
\]

The temporary uniformly finer description used to form W_j is only a deterministic device for defining S. None of its unused coordinates is made an integration variable or charged as an independent rank. The actual section takes values in the same promoted raw list.

Choose C_L≥2 also to dominate the local analytic estimates in Section 2. A direct induction gives a sufficient complex domain and derivative estimate

\[
 \|w-w_*\|_{\rm rel}<c_L C_L^{-m},\qquad
 \|S(w)-S(w_*)\|_{\rm rel}
        \le C_L^m\|w-w_*\|_{\rm rel}.
 \tag{TQ.7}
\]

Since m=O(log R), both the inverse radius and the Lipschitz constant are a fixed power of R, with an additional fixed log R power if the optional collar has been enlarged. In particular, at the actual reference point

\[
 A=D\Phi(0),\qquad R_0=DS(0),\qquad
 AR_0=I,\qquad \|R_0\|\le\operatorname{poly}(R).
 \tag{TQ.8}
\]

The norm is the maximum native-coordinate norm. Conversion to the finite Euclidean norm costs at most a power of the actual dimension D. Every constant remains polynomial. This is why a crude exceptional-bond section suffices here even though it would be unacceptable over the full N=R depth.

## 4. An exact chart of the nonlinear terminal fiber

The following finite-dimensional consequence records what is needed for coarea. Work in small real Lie coordinates of the promoted entries, about the actual reference U_0, and translate the terminal value to zero. Suppose Φ is analytic on a radius ρ_0 with a known second-derivative bound M_2. The primitive maps of WA provide polynomial reciprocal radii and polynomial derivative bounds; a direct logarithmic-depth construction also gives such bounds for this terminal map.

Let `K_0=1+||A||+||R_0||`, and use the splitting

\[
 x=\xi+R_0 b,
 \qquad \xi\in\ker A.
 \tag{TQ.9}
\]

The exact constraint `Φ(x)=0` becomes

\[
 b=-[\Phi(\xi+R_0b)-A(\xi+R_0b)].
 \tag{TQ.10}
\]

On `||ξ||≤ρ`, with

\[
 \rho\le c\min\{\rho_0/K_0,\,(M_2K_0^2)^{-1}\},
 \tag{TQ.11}
\]

this is a contraction on `||b||≤C M_2||ξ||²`. It has a unique analytic solution b(ξ), and

\[
 \Phi(\xi+R_0b(\xi))=0,
 \qquad
 \|R_0b(\xi)\|\le C\|R_0\|M_2\|\xi\|^2.
 \tag{TQ.12}
\]

Thus the terminal delta is imposed exactly. Its linearization is used only to choose the free tangent coordinates; the nonlinear correction is retained. The reciprocal radius in (TQ.11) is a fixed polynomial in R and D. For physical relative angles of size `g·poly(R,P)` this chart has a nonempty fixed margin at sufficiently weak coupling.

## 5. The terminal coarea factor

Let r be the number of independent real terminal constraints and d the promoted raw rank after only those gauges already legitimately removed. The right inverse proves that the smallest nonzero singular value of A is at least `||R_0||^{-1}`; its largest is at most `||A||`. The original finite-dimensional group coarea, expressed in the chart (TQ.9)–(TQ.12), therefore has a constant linear factor whose logarithm is bounded in absolute value by

\[
 C d\log K_0.
 \tag{TQ.13}
\]

On the smaller domain (TQ.11), the derivative with respect to b is

\[
 D_b\Phi(\xi+R_0b(\xi))=I+T(\xi),
 \|T(\xi)\|\le\tfrac12.
 \tag{TQ.14}
\]

Its determinant is retained, and its logarithm has magnitude at most C r. The ordinary Haar densities of the raw entries and the target group coordinates are also retained; in the common small group tube their nonconstant log contribution is at most C d. Consequently the terminal constraint/coarea cost, beyond its explicitly displayed powers of the couplings and fixed group constants, is bounded by

\[
 \boxed{\quad C D\log(R+D+2)+C D.\quad}
 \tag{TQ.15}
\]

If normalized variables `x=g z` are used, their `g^d` Haar/Lebesgue factors and the `g^{-r}` factors from the terminal deltas are written separately and charged once in the original normalization ledger. They are not both included in (TQ.15) and then charged a second time as a box volume. Redundant deltas are removed by their original averaging identities before applying this calculation; they do not contribute additional rank.

This argument supplies a coarea bound on the admitted chart. A delta is never bounded by one. Positive Haar integrations remaining after the exact constraint solve may of course be bounded by their normalized volumes.

## 6. Gauge precision and scope

The section above is cleanest on the full promoted raw group variables with their actual gauge samplers retained. A physical forest gauge can then be imposed using its exact Haar/Faddeev–Popov identity. If such a gauge is imposed first, it must either fix all retained terminal centers or keep the terminal delta in the transformed physical and gauge variables. An average fixed by a delta is not automatically a fixed raw edge of a forest. The virtual-boundary-edge construction is a possible way to prove the terminal-preserving physical chart, but is a separate compatibility step.

Compact normalized gauge directions are not positive Gaussian directions. Soft samplers may instead be written in the exact independent small-w coordinates of MT.13–MT.18, while hard samplers retain their normalized deltas. Removing either kind of variable requires its original identity. This note does not claim that the complete reduced Hessian has already been identified with a particular common Schur complement.

On an actually admitted restored chart, (TQ.15) is the missing quantitative terminal coarea input to a direct finite-volume upper bound such as ER.6. The remaining admission, complete action/completion ledger, positive-energy identification and alternative-test coercivity have to be verified for that same restoration. Their conclusions are not part of the local section theorem.

## Mathematical sources

- CMP119 printed pp.248–250, (1.14)–(1.15), and pp.267–270, (3.15): actual exceptional-bond solve and its full coarea.
- CMP98 printed p.36, (122), (125): the normalized derivative and the exceptional-face coefficient used in (TQ.3).
- LFR I printed pp.191–194, (1.70)–(1.76): N_0, the final M-scale prepared core, and the terminal current restriction on its complement.
- The support analysis's terminal-footprint lemma: the safe inclusion (TQ.1), including crossing-bond footprints and the true MR_j-to-current-scale dictionary.
- [M04 Raw Master Determination](M04_Raw_Master_Determination.md), PM.1 and PM.10–PM.11: exact chronological determination, terminal deltas and the original coordinate/coarea factors.
- [mixed weighted averaging](mixed_weighted_averaging.md): polynomial analytic readout bounds, with the actual inverse axial gauge retained.
