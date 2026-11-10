# Flat ordinary innovations have a uniform native gap at every depth

This note proves the flat linear statement needed for the explicit old-A part of a finite restored history. It uses the exact scale normalization of curvature averaging, followed by the already proved fixed-L block Poincare inequality. The result concerns the Gaussian Hessian at the flat reference and its exact Schur marginals. It does not infer the same complete-law convexity for a nonlinear history or differentiate an integrated hard-cutoff completion.

## 1. Curvature averaging is an L² contraction in four dimensions

Let a be a dimensionless oriented bond angle on the fine unit lattice. At the identity, the source raw coarse average is a linear one-form average \mathcal Q_1. Its difference from Balaban's gauge-corrected new average is an endpoint gradient; taking a plaquette circulation removes that difference.

For a coarse plaquette based at y in the positive μν plane, discrete Stokes and the translated-path formula CMP98 (125) give

\[
 (d\mathcal Q_1a)_{p_y^{\mu\nu}}
 =L^{-d}\sum_{x\in B(y)}
   \sum_{r,s=0}^{L-1}(da)_{p_{x+r e_\mu+s e_\nu}^{\mu\nu}}
 =:(\mathcal Q_2 da)_{p_y^{\mu\nu}}.
 \tag{IG.1}
\]

The four translated paths form the boundary of the L by L rectangle based at x. Their internal edges cancel. The L factor converting the normalized physical-one-form Q of (125) into raw output angles is included here; its omission would give the wrong dimensional scaling.

The positive kernel \mathcal Q_2 has row sum L². For a fixed fine μν plaquette there are exactly L² starting pairs (r,s); each corresponding x belongs to exactly one coarse block. Consequently its column sum is L^{2-d}. The Schur test gives

\[
 \|\mathcal Q_2\|_{\ell^2\to\ell^2}
 \le\sqrt{L^2 L^{2-d}}=L^{(4-d)/2}.
 \tag{IG.2}
\]

All norms here use counting measure and dimensionless plaquette angles at their respective scales. In d=4,

\[
 \|d\mathcal Q_1a\|_2\le\|da\|_2,
 \qquad
 \|d\mathcal Q_{1,0:j}a\|_2\le\|da\|_2.
 \tag{IG.3}
\]

The second estimate follows by composition with no constant per scale. It also holds after restricting output plaquettes: the positive row and column sums only decrease. Reference parallel transports are trivial in this flat statement; no uncontrolled absolute value of a nonflat matrix product is being used.

## 2. The coarse constrained minimum dominates coarse curvature

Let H_j b be the derivative of the actual regular minimizing field with respect to a j-scale current bond perturbation b, with all older mixed raw determining data held fixed. Work at the flat reference, on the physical quotient. Its quadratic Wilson action is

\[
 q_j(b)=\tfrac12\|dH_jb\|_2^2,
 \tag{IG.4}
\]

up to the fixed trace/coupling convention. The original microscopic field and current perturbation use the corresponding dimensionless normalizations; running couplings comparable on the fixed first-reset window change only a fixed constant.

The literal current readout of H_jb is b on the active footprint. Therefore (IG.3) gives

\[
 q_j(b)\ge c\|d_jb\|_2^2.
 \tag{IG.5}
\]

For a mixed domain, the following interface conditions are part of this assertion. The perturbation b is supported in the ordinary active region Ω_{j+1}. The fixed-L averaging/Poincare halo of that region lies inside Ω_j by the source's R M1 separation. On this halo every j-readout is a literal prescribed current entry. Those outside the active Ω_{j+1} portion belong to the held Γ_j data and have zero variation. Extend b by precisely that zero readout on this halo when forming boundary plaquettes. PM's exact chronological determination gives the required equality with the average of H_jb there. No assertion about a global j-readout across an older lower-grid interface is needed. In particular one must not extend b by zero across an averaging footprint whose older raw constraints are actually varying.

Under these conditions, output restriction in (IG.3) proves (IG.5) for all the current plaquettes needed in the local Poincare argument. An older fine constraint can only shrink the fine minimizing fiber; it cannot lower its action below the curvature energy of its specified current readout.

## 3. The actual free-coordinate precision has a uniform flat gap

Let Q_j be the next one-step linear average on the j lattice, and let C_j be the source exceptional-bond elimination map. Thus Q_jC_j z=0 and C_j z keeps every independent free coordinate z unchanged. Let τ_av,j be the actual symmetrized contour gauge map of CMP109 (0.11), not a substituted single tree-path map.

The fixed-L block argument PG.1, applied at this native scale, gives

\[
 \|b\|_2^2\le C_L\{\|d_jb\|_2^2+
                         \|\tau_{\rm av,j}b\|_2^2\},
 \qquad Q_jb=0.
 \tag{IG.6}
\]

Combining (IG.5), the original positive soft-gauge quadratic and (IG.6),

\[
 q_j(C_jz)+c_{\rm gf}\|\tau_{\rm av,j}C_jz\|_2^2
 \ge c_L\|C_jz\|_2^2\ge c_L\|z\|_2^2.
 \tag{IG.7}
\]

Hence the flat source ordinary free precision K_j obeys

\[
 \boxed{\qquad K_j\ge c_L I,\qquad
     \|K_j^{-1}\|_{2\to2}\le C_L.\qquad}
 \tag{IG.8}
\]

The constant is independent of j, N, the total volume and the number of old components, subject to the stated admitted footprint conditions. This does not require estimating a sequence of prolongations by C^j. The scale-critical curvature contraction gives the needed lower bound in one step.

At the flat reference the ambient Wilson force vanishes, so there is no omitted constraint-multiplier Hessian in this particular statement. For a nonflat source reference, the actual current and constraint-curvature contribution must be restored; IG.8 does not by itself control it.

If only a subset D_j of the j-th free coordinates is left explicit, its **untruncated** marginal precision is the exact Schur complement S_j. Since K_j≥c_LI,

\[
 z_{D_j}^{\mathsf T}S_jz_{D_j}
   =\inf_{z_{D_j^c}}z^{\mathsf T}K_jz
   \ge c_L\|z_{D_j}\|_2^2.
 \tag{IG.9}
\]

The same gap therefore holds for every such retained first or later ordinary marginal. Its actual cutoff completion is retained separately; it is not claimed to equal one.

## 4. Nested Gaussian innovations are independent before masks

There is an exact abstract statement behind the flat source bookkeeping. Let \mathcal F_0⊃\mathcal F_1⊃⋯⊃\mathcal F_m be linear readout sigma-algebras of one Gaussian physical field, with fixed terminal data imposed. Write P_i for the corresponding energy-orthogonal conditional-mean projections. Then

\[
 P_iP_{i+1}=P_{i+1},\qquad
 Y_i=(P_i-P_{i+1})A
 \tag{IG.10}
\]

are mutually orthogonal in the Gaussian covariance geometry and are independent centered Gaussians, independent of the final retained readout. This follows either from zero cross covariance or the exact successive Schur square completion NE.6.

The ordinary mixed readouts are nested: a next mixed determining list is obtained by retaining older raw entries and averaging the current active ones. The actual free innovation has zero next average. Thus the flat ordinary A_j coordinates are linear coordinates on these successive increments, with their actual conditional mean removed. A source preparatory integration has the same conclusion whenever its stated new readout is obtained from the preceding one by the exact next averaging identity; that nesting must be checked for the particular restored B_j list.

The source normalized gauge variables can be added as independent Gaussian coordinates in their exact small-w parameterization. Center-fixed gauge changes preserve the next readout. They do not change the physical projection argument and must not be removed as if they were absent.

Consequently, on one correctly identified restored history, the untruncated Gaussian reference is block diagonal in its explicit ordinary innovation blocks and the remaining physical determining block. Each ordinary block has the gap (IG.8), including any retained marginal. A separate physical B/V_h block need not have that same Euclidean gap; the R^9 test estimate must not be mistaken for an operator bound there.

After imposing the original good masks, independence generally disappears. If those Gaussian masks are centered convex, the covariance bounds survive by CR.12. When integrated good masks are retained as Gaussian completion factors, GC.4–GC.6 shows that their convexity also preserves the reference bound. None of these facts establishes a small old-A derivative for the completed nonlinear action.

## 5. Consequence for a prospective perturbative derivative budget

Suppose a complete perturbation W on a finite admitted chart has total value budget A_*, and suppose its explicit ordinary innovation dependence has verified first/second real derivative bounds

\[
 |\partial_a W|\le C A_*/P_{\min},\qquad
 |\partial_a\partial_bW|\le C A_*/P_{\min}^2.
 \tag{IG.11}
\]

These may follow from a legitimate analytic tube with smooth switches separately controlled, but are **not** supplied by the bounded boundary term alone; GC.1–GC.3 explains the issue.

For D explicit ordinary coordinates, the block-diagonal gap gives

\[
 \|K_A^{-1/2}\nabla_AW\|^2
       \le C D A_*^2/P_{\min}^2,
 \qquad
 \|K_A^{-1/2}W_{AA}K_A^{-1/2}\|
       \le C D A_*/P_{\min}^2.
 \tag{IG.12}
\]

For D=O(R^5 log^4 R), A_*=O(R^6 times fixed logarithms), and P_min=p1(g), the first numerator is R^17 times fixed logarithms. The literal hierarchy 2p1−9r0>p0>p1 implies p1>9r0. With r0≥r and R comparable to (log g^{-2})^r, both bounds in IG.12 tend to zero. No R^9 inverse factor is needed on these explicit innovation coordinates.

This verifies the exponent arithmetic and the Gaussian metric for that proposed route. It leaves the actual derivative hypothesis, the physical U/J-slot pullback, nonlinear mask enclosures and full completion comparison as source obligations. In particular it does not turn the general boundary-analyticity gate into a proved theorem.
