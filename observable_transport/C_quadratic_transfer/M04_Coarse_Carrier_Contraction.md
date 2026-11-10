# Coarse covering contracts the actual volume-plus-tree carrier size

This note resolves a geometric part of the next uniform-depth question. It uses the stated carrier weight, proves a deterministic weighted pushforward estimate, and separates it from the number of fine anchors and from Gaussian or interaction losses. It does not alter TC, NC, TR, TS, or the original M-03 norm.

## 1. The exact size convention

Annex Y, Section 1, (M.2), defines
\[
 n_h(X)=|X|+\mathsf t_h(X),\qquad
 w_h(X)=e^{\kappa n_h(X)} ,
 \tag{CC.1}
\]
where \(\mathsf t_h(X)\) is the number of edges of a shortest connected subgraph of the current block graph containing \(X\). The graph is the homogeneous periodic cubic block graph in the application here. Sizes are in its current units, not microscopic-link counts. Full determining footprints and insertion anchors belong to \(X\).

If \(X\ne\varnothing\) is already connected, a spanning tree has \(|X|-1\) edges, and no connected graph containing \(X\) can have fewer. Thus
\[
 n_h(X)=2|X|-1\quad\hbox{for connected }X.
 \tag{CC.2}
\]
For a general nonempty \(X\), a shortest connected subgraph may be chosen to be a tree \(T\), with \(\mathsf t_h(X)\) edges. The tree is used below to estimate a cover. It need not be declared an additional set of field dependencies.

This is distinct from silently substituting the source's continuum tree-length convention for the specified norm. CMP109 p.257 and CMP116 (1.26), (1.33)--(1.36) describe native tree supports, but their conversion to the actual physical block graph still has to be retained in a coefficient construction. The present lemma starts with those full physical supports already specified.

## 2. A one-step cover bound

Let \(\pi_L\) be an aligned partition into blocks of side \(L\), with each fine block assigned to one parent block. Write
\[
 {\cal C}_L X=\{\pi_L x:x\in X\},\qquad
 F_{L,c}(X)=({\cal C}_LX)^{+c},
 \tag{CC.3}
\]
where the superscript is a sup-norm graph dilation by the integer \(c\ge0\) in the new block units. All additional incidence conventions and fixed constraint/gauge/readout collars must be included in \(c\). In particular, if a convention counts every closed-cell contact rather than using the parent assignment, its extra one-block incidence is included here.

### Lemma CC.1

In dimension \(d\), set
\[
 A_c=2^{d+1}(2c+1)^d .
 \tag{CC.4}
\]
For every nonempty finite carrier \(X\),
\[
 n_{Lh}(F_{L,c}(X))
 \le A_c\left(1+\frac{2\mathsf t_h(X)}{L}\right)
 \le A_c+\frac{2A_c}{L}n_h(X).
 \tag{CC.5}
\]
If \(X\) is connected, the stronger estimate is
\[
 n_{Lh}(F_{L,c}(X))
 \le A_c+\frac{A_c}{L}n_h(X).
 \tag{CC.6}
\]

**Proof.** Traverse each edge of a shortest connecting tree \(T\) twice. The resulting walk has length \(2\mathsf t_h(X)\). Split it into walks of at most \(L\) fine edges. There are at most \(1+2\mathsf t_h(X)/L\) pieces. Each piece has coordinate range at most \(L\) in every direction, so it meets at most \(2^d\) aligned parent blocks. Consequently
\[
 |{\cal C}_LT|
 \le 2^d\left(1+\frac{2\mathsf t_h(X)}{L}\right).
 \tag{CC.7}
\]
The image of a connected nearest-neighbor walk is connected: a fine edge maps either to one coarse vertex or to a coarse edge. Its \(c\)-dilation remains connected. That dilation has at most \((2c+1)^d|{\cal C}_LT|\) vertices and contains \(F_{L,c}(X)\). Monotonicity of cardinality and of the shortest connecting-tree length therefore bounds its \(n\)-size by twice that number minus one. This proves the first inequality in CC.5, with harmless room in the displayed constant. The general second inequality uses \(\mathsf t_h(X)\le n_h(X)\). For connected \(X\), use \(2\mathsf t_h(X)=n_h(X)-1\), giving CC.6. \(\square\)

The proof also covers periodic carriers that wrap around the torus. Each short piece of the tree walk can be lifted to the covering lattice, and reduction modulo the coarse torus cannot increase the number of blocks it visits. A one-block or otherwise small final torus only reduces that count. No global nonwrapping representative of \(T\) is required.

A strictly multiplicative contraction without an additive constant is false even for a singleton and \(c=0\): its size stays one. With \(c>0\), a singleton acquires a fixed neighborhood. Large \(L\) gives one-step affine contraction if the actual \(c\) satisfies \(2A_c<L\) (or \(A_c<L\) for connected carriers). The source's fixed localization constants need not satisfy that relation. It must not be assumed just because all of them are fixed.

## 3. Repeated fixed collars can be grouped without an age-dependent collar

Consider a sequence
\[
 X_{j+1}=F_{L,c_j}(X_j),\qquad 0\le c_j\le c,
 \tag{CC.8}
\]
on a nested aligned block hierarchy. Put
\[
 c_\infty=\left\lceil\frac{cL}{L-1}\right\rceil+1 .
 \tag{CC.9}
\]
The final \(+1\) is retained as a uniform alignment allowance. It is not multiplied by the number of steps.

### Lemma CC.2

For every available integer \(N\ge1\),
\[
 X_N\subset({\cal C}_{L^N}X_0)^{+c_\infty},
 \tag{CC.10}
\]
and, with \(A_\infty=A_{c_\infty}\),
\[
 n_{h_N}(X_N)
 \le A_\infty+
        \frac{2A_\infty}{L^N}n_{h_0}(X_0).
 \tag{CC.11}
\]
For connected \(X_0\), replace \(2A_\infty\) by \(A_\infty\) in the second term.

**Proof.** Use coordinates in the covering lattice. A point produced by successive dilation choices has a fine ancestor \(x\in X_0\) and integer displacement vectors \(a_j\) with \(|a_j|_\infty\le c\). Unrolling the nested floor maps shows that its final position differs from the assigned \(L^N\)-parent of \(x\) by a displacement bounded by
\[
 c\sum_{r=0}^{N-1}L^{-r}
\]
before the last integer rounding. This is at most \(cL/(L-1)\). Fixed offsets for centered odd-\(L\) blocks are included in the common nested parent map and cancel in this comparison. CC.9 therefore bounds the final integer displacement. This proves CC.10. The argument is coordinatewise and remains valid after taking residues on any compatible periodic torus.

Apply the proof of Lemma CC.1 to the original connecting-tree walk, now splitting it into pieces of length \(L^N\), and then take its single \(c_\infty\)-dilation. This gives CC.11. In particular no constant in CC.11 grows with \(N\). \(\square\)

Choose once a block-grouping depth \(q\) such that
\[
 \vartheta:=2A_\infty L^{-q}<1.
 \tag{CC.12}
\]
This is possible for every fixed finite \(c\) and \(L>1\), including when the ordinary buffer is larger than \(L\). Each group of \(q\) blockings then satisfies
\[
 n_{\rm out}\le\vartheta n_{\rm in}+A_\infty.
 \tag{CC.13}
\]
The constants and \(q\) are fixed. This assertion does not permit an unspecified collar depending on the accumulated depth; that would violate the hypothesis \(c_j\le c\).

For a forest, apply the estimate to each connected component and multiply its component weights. The additive term is paid per component. It does not join previously disconnected components or waive the true connector length.

## 4. Deterministic weighted pushforward, before anchor summation

Let nonnegative numbers \(a_X\) be indexed by old carriers, and let a deterministic grouped cover send \(X\) to \(F(X)\). Preserve all labels, or aggregate them exactly as
\[
 b_Y=\sum_{X:F(X)=Y}a_X .
\]
If CC.13 holds, then
\[
 \sum_Y e^{\kappa n(Y)}b_Y
 \le e^{\kappa A_\infty}
       \sum_Xe^{\kappa\vartheta n(X)}a_X .
 \tag{CC.14}
\]
Equivalently, each column of this nonnegative pushforward matrix satisfies
\[
 \frac{\sum_Y e^{\kappa n(Y)}
                   {\bf1}_{F(X)=Y}}
      {e^{\kappa n(X)}}
 \le
 e^{\kappa A_\infty}
 e^{-\kappa(1-\vartheta)n(X)}.
 \tag{CC.15}
\]
This is a genuine positive spatial gain for large carriers, at the **same** rate \(\kappa\).

The additive constant is a small-carrier floor, not a geometric exponential loss at every time. For example put
\[
 B_*=\frac{A_\infty}{1-\vartheta},\qquad
 s(X)=(n(X)-B_*)_+ .
\]
Then CC.13 implies
\[
 s(F(X))\le\vartheta s(X),\qquad
 e^{\kappa s(X)}\le e^{\kappa n(X)}
                  \le e^{\kappa B_*}e^{\kappa s(X)}.
 \tag{CC.16}
\]
These equivalences are used once at the ends of a deterministic transport lineage. They are not an assertion that the reduced weight is a replacement polymer-algebra norm: its multiplication rules would need separate accounting. Alternatively one may retain the exact original weight ratios, which telescope, and use CC.11 directly.

This addresses the repeated fixed geometric conversion in CA.6 and TC.9: bounding each cover by \(C_{\rm cov}n(X)\) and dividing the rate by \(C_{\rm cov}\) at every step is unnecessary for the cover operation itself. It does not prove that every other step of the analytic construction preserves that rate.

## 5. A precise small-substitution consequence

Here is the algebraic consequence for an analytic coefficient when its actual supported substitution has already been constructed. This statement does not supply such a substitution from numerical sensitivity alone.

Suppose every local zero-correction readout on the whole common parameter tube has a remaining product physical-angle polydisc of radius \(r_*>0\), and \(f_X\) is bounded by \(a_X\) on the union of those polydiscs. Thus \(r_*\) is a uniform reserve about each actual readout, not merely the radius of a domain centered at zero whose boundary a readout might approach. Assume also a uniform coordinate-incidence bound of at most \(d_0|X|\) scalar coordinates. The zero-correction readout has full raw support \(F(X)\). Write each correction as an actual connected-carrier series rooted in that support, and assume its summed coefficient norm at rate \(\kappa\), on the same common parameter tube, is at most \(q_*\). Include all coordinate and fixed Lie-chart multiplicities in the assumed constant \(d_0\). For \(q_*<r_*/2\), the multivariable Cauchy series and submultiplicativity of connected unions give
\[
 \sum_{\text{substitution tags }\alpha}
 e^{\kappa n(Y_\alpha)}|[f_X]_\alpha|
 \le
 a_Xe^{\kappa n(F(X))}
       (1-q_*/r_*)^{-d_0|X|}
 \le a_Xe^{\kappa A_\infty}
       e^{(\kappa\vartheta+Cq_*)n(X)} .
 \tag{CC.17}
\]
Each correction carrier meets the zero-correction support or its actual previously attached stencil; its union is the declared physical carrier. No connected-coefficient identity is inferred from a distance bound.

In particular if
\[
 Cq_*\le\tfrac12\kappa(1-\vartheta),
 \tag{CC.18}
\]
the same output rate \(\kappa\) is retained, with another positive fraction of the input spatial exponent still available. This is the column estimate behind the small \(e^{Cq|X|}\) loss in CA.6; the contraction can pay it without a fresh arbitrary fractional loss of \(\kappa\).

On the reduced size in CC.16, the corresponding algebra is
\[
 e^{\kappa s(F(X))}e^{Cq_*n(X)}
 \le e^{Cq_*B_*}
       e^{(\kappa\vartheta+Cq_*)s(X)} .
 \tag{CC.19}
\]
It exposes the remaining bounded-carrier amplitude cost. Geometry does not make the product of these costs finite along infinitely many steps. Summability, relevant-term extraction, or an exact joint comparison is still required.

## 6. Anchored density entropy is a different estimate

For the unpadded deterministic cover/dilation in CC.8, a fixed final block \(b\in X_N\) has some fine ancestor \(x\in X_0\) whose \(L^N\)-parent is within \(c_\infty\) of \(b\). There are at most
\[
 C_d(2c_\infty+3)^d L^{dN}
 \tag{CC.20}
\]
such fine ancestors. Combining this with CC.11 gives the anchored upper bound
\[
 \sup_b\sum_{Y\ni b}e^{\kappa n(Y)}b_Y
 \le C_d(2c_\infty+3)^dL^{dN}e^{\kappa A_\infty}
       \sup_x\sum_{X\ni x}
                  e^{2\kappa A_\infty L^{-N}n(X)}a_X .
 \tag{CC.21}
\]
The tree in the proof of CC.5 is not padded into the deterministic support map here. If a later construction deliberately adds new support, that addition needs its own declared map and anchor estimate.

The factor \(L^{dN}\) cannot be removed for arbitrary unextracted density activities. Put one constant coefficient \(\varepsilon\) on each fine singleton, use \(c=0\), and perform only the parent pushforward. A coarse singleton receives exactly \(L^{dN}\varepsilon\). This example is compatible with positive normalized integration, which leaves constants unchanged. It is a limitation of an unextracted anchored norm, not a counterexample to Yang--Mills.

For \(d=4\), the original vacuum and marginal-action extraction problem therefore remains. The fixed incoming microscopic scalar scaling and the density of possible birth positions must also be kept separate. A column estimate for one specified root is not a bound for the sum of all possible fine roots at one coarse anchor.

## 7. What this settles and what it does not

The positive result is a uniform geometric statement for the actual volume-plus-tree norm. Full ordinary carriers with fixed local stencils have an affine contraction after a fixed number of blockings; skinny carriers, disconnected finite supports and winding periodic supports are included. Fixed collars accumulate to one bounded final collar. This removes a purely geometric reason to divide the available spatial rate by a fixed constant at every depth.

Applying CC.17 to an all-depth construction still requires the common analytic correction registry, its uniform physical tube and a sufficiently small supported coefficient norm. The fixed-third TC construction verifies those inputs only at its stated fixed depth. CC does not establish them for all depths.

Growing nonanalytic Q-reference cores follow the separate CGD recurrence and are paid by their own birth reserves; they are not ordinary fixed collars in CC.8. Gaussian rank/determinant comparisons, old real-domain admission, boundary jets, and exact conditional normalization remain the joint-certificate problem of UD/AP/SG and the later core analysis. Their amplitude costs do not telescope merely because support weights do.

Finally, the repeated bounded-carrier costs in CC.19 and the anchored density factor in CC.21 require the actual source extraction/scaling mechanism. No all-depth M04 or continuum-existence conclusion is asserted.

Source/companion locations: Annex Y Section 1 (M.1)--(M.2); CMP109 p.257 and CMP116 (1.26), (1.33)--(1.36) for the distinct native carrier conventions; CA.6 and TC.9 for the fixed-depth supported substitution; CGD.1--10 for growing-core geometry and the independent anchor issue.
