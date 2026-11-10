# A stopped sequence with a positive weak endpoint

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

**Gaussian calibration hypothesis (GC).** For the signed Gaussian increments of the actual stationary source section in its thermodynamic normalization, assume $\sum_{k<n}d_k^G=d_Bn+\vartheta_n$ with $d_B>0$ and $\sup_n|\vartheta_n|\le B_G$. The coupling and stopping conclusions use this calibration and the specified source readout and replay. A physical continuum limit also requires the stated uniform normalization and full-law hierarchy estimates.

## Stopped-sequence application and the stated B05 test

Assume the **actual** source-free Wilson recursion has been proved through every admitted stopped prefix, with its infinite-volume coupling readout and finite-torus replay identified. Assume its Gaussian calibration and all-depth error give a bounded-coboundary corrected inverse coupling with a uniformly positive decrement while the physical inverse coupling is at least one fixed large ceiling \(Y_{\min}\).

Then one can construct an actual cofinal sequence of bare Wilson coefficients and cubic lattices whose terminal inverse couplings stay in a fixed compact subset of \((Y_{\min},\infty)\). A subsequence has a strictly positive weak terminal coupling. No continuity across the rounded \(R_j\)-grid changes and no shooting at a prescribed integer depth are needed for this conclusion.

The actual-map inputs are now supplied at the retained causal-source and original Gaussian-calibration scope by [Homogeneous feedback and the causal Wilson recursion](causal_coupling_recursion.md), (BP.17), (BP.20), and (BP.22)–(BP.31), together with [The driven homogeneous coupling endpoint](driven_coupling_endpoint.md), (DE1), and the causal-source compatibility conditions. Thus the stopped sequence below is an application of those results. The hypotheses are repeated in Section 1 so the numerical theorem is standalone; a numerical recurrence without the actual-map/replay identification would not suffice.

The original B05 statement is stronger: it asks for one coherent bare Wilson set satisfying the **chosen finite physical normalization at \(\ell_0\)**, with compatibility across cutoff depths. A subsequential, emergent scalar endpoint is not automatically that prescribed normalization or a compatible limit of full effective states. Section 8 states the precise remaining distinction.

## 1. Actual-map assumptions and the corrected coordinate

Use the retained source convention
\[
 Y_j=g_j^{-2},\qquad
 \beta_{W,0}=Y_0/N.
 \tag{PE.1}
\]
Fix the source group, odd block factor \(L\), all static grid/decay/chart constants, and a common admitted lower ceiling \(Y_{\min}\) for \(Y\).

The hypothesis is an **actual, causal** recursion on every prefix for which \(Y_j\ge Y_{\min}\), including a provisional next output computed from that admitted input:
\[
 Y_{j+1}=Y_j-d_j^G-e_j,\qquad
 \left|\sum_{i=0}^{j-1}(d_i^G-d_B)\right|\le Q,
 \qquad
 |e_j|\le A/Y_j,
 \tag{PE.2}
\]
with fixed \(d_B>0,A,Q<\infty\). A different quantified error suffices if it is uniformly smaller than \(d_B/2\) on this ceiling. The constants must be independent of total prefix length, bare coupling and finite volume in the stated source readout/replay convention.

At the stated source and calibration scope, (PE.2) is the consequence (BP.23)–(BP.28) of the two stated B03 analytic gates. The source scheme and exponent choices are fixed once before the final weak ceiling. The outgoing scalar is the actual homogeneous infinite-volume projector, and finite cubic lattices use the same scalar prescription in the retained replay convention.

Put
\[
 q_j=\sum_{i<j}(d_i^G-d_B),\qquad
 Z_j=Y_j+q_j .
\]
Then
\[
 |q_j|\le Q,\quad q_0=0,\qquad
 Z_{j+1}=Z_j-d_B-e_j.
 \tag{PE.3}
\]
Choose \(Y_{\min}\) large enough that \(A/Y_{\min}\le d_B/4\), and set, for example,
\[
 d_-=\frac34d_B,\qquad d_+=\frac54d_B .
\]
Every admitted step then obeys
\[
 d_-\le Z_j-Z_{j+1}\le d_+.
 \tag{PE.4}
\]
No sign is asserted for the individual uncorrected decrement \(Y_j-Y_{j+1}\). That is why stopping is first done in \(Z\).

Choose a fixed threshold
\[
 Z_*>Y_{\min}+Q+d_+ .
 \tag{PE.5}
\]
Its excess can be increased to meet any finite list of native/source ceiling tolerances. The choice is independent of the bare cutoff.

## 2. The last admitted corrected stopping point

For an actual trajectory starting at \(Y_0\to\infty\), let \(K\) be the last index with \(Z_K\ge Z_*\), stopping when the provisional next output satisfies \(Z_{K+1}<Z_*\).

This stopping time exists and is finite. Until the crossing,
\[
 Y_j=Z_j-q_j\ge Z_*-Q>Y_{\min},
\]
so every required input is admitted. The next output is computed by the actual provisional recursion; (PE.5) even keeps its physical inverse coupling above \(Y_{\min}\), although that extra output need not be used in the final sequence. The positive decrement in (PE.4) forces a crossing in finitely many steps.

At the stop,
\[
 Z_*\le Z_K<Z_*+d_+,
 \qquad
 Z_*-Q\le Y_K<Z_*+d_++Q.
 \tag{PE.6}
\]
In particular
\[
 (Z_*+d_++Q)^{-1/2}
 < g_K\le (Z_*-Q)^{-1/2}.
 \tag{PE.7}
\]
Both endpoints are fixed positive numbers, and the upper one lies below all chosen weak-coupling ceilings.

Moreover
\[
 \frac{Y_0-Z_*-d_+}{d_+}<K
 \le\frac{Y_0-Z_*}{d_-}.
 \tag{PE.8}
\]
Thus \(K\to\infty\) with \(Y_0\).

If the uncorrected coordinate itself has the positive decrement, take \(Q=0\). Then (PE.6) reduces to the usual fixed interval of width \(d_+\). The bounded-coboundary formulation is the one relevant to the currently retained Gaussian calibration.

## 3. Recovering the literal terminal suffix inequality

The bounded correction gives useful all-pair inequalities immediately:
\[
 d_-(k-j)-2Q
 \le Y_j-Y_k
 \le d_+(k-j)+2Q,\qquad j<k\le K.
 \tag{PE.9}
\]
For the exact no-additive-slack terminal inequality printed in CMP109 (0.31), make a bounded final trimming, as in the accepted B02 construction.

Fix \(0<a<d_-\), for example \(a=d_-/2\). Let \(S_i=Y_0-Y_i\), and let \(K'\) be the **last** maximizer of
\[
 S_i-ai,\qquad 0\le i\le K.
 \tag{PE.10}
\]
Then
\[
 0\le K-K'\le J_0:=
 \left\lceil\frac{2Q}{d_--a}\right\rceil .
 \tag{PE.11}
\]
Indeed maximality gives \(S_K-S_{K'}\le a(K-K')\), while (PE.9) bounds the left side below by \(d_-(K-K')-2Q\).

For every \(j\le K'\),
\[
 a(K'-j)\le Y_j-Y_{K'}
       \le D(K'-j),\qquad D=d_++2Q,
 \tag{PE.12}
\]
where the upper inequality for positive integer age absorbs \(2Q\) into \(D\); at age zero it is exact. The lower inequality is precisely the maximality condition in (PE.10).

Trimming changes the terminal compact interval by only a fixed amount:
\[
 Y_-:=Z_*-Q\le Y_{K'}\le
 Y_+:=Z_*+d_+(J_0+1)+Q.
 \tag{PE.13}
\]
The retained causal trajectory before \(K'\) is unchanged. Also \(K'\to\infty\).

With \(\epsilon=L^{-K'}\), (PE.12) is the printed source terminal envelope, with constants \(a/\log L\) and \(D/\log L\):
\[
 Y_{K'}+\frac a{\log L}
       \log[(L^j\epsilon)^{-1}]
 \le Y_j
 \le
 Y_{K'}+\frac D{\log L}
       \log[(L^j\epsilon)^{-1}].
 \tag{PE.14}
\]
This does not assert positive single-step drift of raw \(Y_j\).

The all-pair bound (PE.9), together with a large fixed \(Y_{\min}\), also gives the source pairwise coupling/profile comparisons. For example \(Y_j\ge Y_k-2Q\) makes \(g_j/g_k\le1+\beta_0\) at a sufficiently large ceiling, while
\(Y_j/Y_k\le1+(d_++2Q)(k-j)/Y_k\)
controls the reverse ratio. For any fixed profile exponent \(p\),
\[
 \left(\frac{\log Y_j}{\log Y_k}\right)^p
 \le
 \left(1+\frac{D(k-j)}{Y_k}\right)^{p/\log Y_k}
\]
in the direction \(Y_j\ge Y_k\), with the bounded opposite-direction slack absorbed by the chosen ceiling. Taking \(Y_{\min}\) large after the finite list of exponents makes the required exponent at most the source tolerance \(\beta_0\).

For the rounded radii \(R_j\), CMP119 (2.9), p.256, permits the fixed \(L\) rounding factor. The preceding logarithmic comparisons give its two inequalities. In particular possible small raw-coupling reversals do not require assuming all \(R_j\) are equal.

## 4. One bare prescription and a cofinal physical mesh

Choose any deterministic unbounded bare sequence, for example
\[
 Y_{0,n}=Y_{\min}+n.
 \tag{PE.15}
\]
For each \(n\), use the **actual same source prescription** to generate its trajectory and compute the stops \(K_n,K_n'\). If strictly increasing depths are convenient, retain the deterministic subsequence obtained by taking the next \(n\) for which \(K_n'\) exceeds its preceding chosen value. Equation (PE.8) ensures this procedure never stops.

Define
\[
 a_n=\ell_0L^{-K_n'},\qquad
 h_{j,n}=\ell_0L^{j-K_n'},\qquad
 \beta_{W,n}=Y_{0,n}/N .
 \tag{PE.16}
\]
Then \(a_n\to0\), and the final retained scale is exactly \(\ell_0\). These are genuine bare Wilson coefficients, not independently postulated sequences of effective couplings.

The source lower/upper slopes give the logarithmic bare order
\[
 c_1K_n'\le Y_{0,n}\le c_2K_n'+C,
\]
so
\[
 \beta_{W,n}\asymp\log(\ell_0/a_n).
 \tag{PE.17}
\]
This is an additional useful property absent from the B02 short-window witness.

Under the sharper error in (PE.2), sum the actual recurrence to obtain
\[
 Y_{0,n}
 =d_BK_n'+Y_{K_n'}+q_{K_n'}
                   +\sum_{j<K_n'}e_j.
\]
Using (PE.12),
\[
 \sum_{j<K_n'}\frac1{Y_j}
 \le \frac1{Y_-}
    +\frac1a\log\left(1+\frac{aK_n'}{Y_-}\right).
\]
Consequently
\[
 \beta_{W,n}
 =
 \frac{d_B}{N\log L}\log(\ell_0/a_n)
 +O(\log\log(\ell_0/a_n))+O(1),
 \tag{PE.18}
\]
with the fixed terminal interval absorbed in the last constant. This is conditional on the actual all-depth recurrence, not a new proof of its coefficient.

## 5. Original cubic geometry works at a fixed positive endpoint

Keep exactly the fixed divisors and odd-\(L\) centered partitions of the accepted B02 geometry. Write \(M=L^u\), \(M_2=L^v\), with the source's once-selected compatible fixed divisors understood. Let
\[
 R_j=L^{r_j},\qquad
 R_j\le C_R[\log Y_j]^{r}
 \tag{PE.19}
\]
with the source rounding factor included in \(C_R\). The equality convention at a rounding threshold is the actual source convention, not a new one.

At age \(s=K_n'-j\), (PE.12)–(PE.13) give
\[
 Y_j\le Y_++Ds.
\]
Hence
\[
 \sup_{n,j\le K_n'}
       L^{j-K_n'}R_j
 \le C_R\sup_{s\ge0}
     L^{-s}[\log(Y_++Ds)]^r
 =:C_{\rm geom}<\infty .
 \tag{PE.20}
\]
The supremum is finite because an exponential dominates every power of a logarithm. Thus the physical sizes of **all** old \(MR_j\) and \(LM_2R_j\) tiles are bounded by one fixed multiple of \(\ell_0\), uniformly in the bare depth. They need not be equal.

Choose a fixed integer \(H_0\) such that every such tile exponent
\[
 j-K_n'+r_j+\max(u,1+v)
\]
is at most \(H_0-q\), where \(q\) is fixed with \(L^q\) larger than the source's finite halo/component multipliers. Every elementary and earlier compatible grid then divides the cubic period
\[
 T_n=2L^{H_n}\ell_0,\qquad H_n\ge H_0.
 \tag{PE.21}
\]
The \(100MR_j\) component rectangles and their finitely many fixed enlargements fit as neighborhoods. They do not impose new independent period divisors.

Any choice \(H_n\to\infty\) above this fixed bound is cofinal. In particular one may take
\[
 H_n=\max\{H_0,\lfloor\theta\log_L(2+K_n')\rfloor\},
 \qquad 0<\theta<\frac14.
 \tag{PE.22}
\]
Then \(T_n\to\infty\) and the terminal lattice volume satisfies
\[
 V_{{\rm term},n}=(T_n/\ell_0)^4
 \le C(2+K_n')^{4\theta}=o(K_n').
 \tag{PE.23}
\]
This optional slow-volume property is a geometric fact only; it does not imply an interacting terminal estimate.

The common centered origin and odd \(L\) give the same site-reflection planes as B02. Explicitly,
\[
 T_n/(2h_{j,n})=L^{H_n+K_n'-j}\in\mathbb N.
\]
The fixed half-\(\ell_0\) translation used in the accepted construction identifies all center lattices with the corresponding \(h_{j,n}\mathbb Z^4\). Every compact physical support eventually fits inside the cubic torus.

Finally the compact Wilson reserve obeys
\[
 \frac{\log(1+\beta_{W,n})}{T_n/a_n}
 \le
 \frac{C\log(2+K_n')}{2L^{H_n+K_n'}}
 \longrightarrow0.
 \tag{PE.24}
\]
Thus the actual logarithmic bare order is compatible with this geometry and its microscopic compact-moment reserve.

All statements in this section concern original cubic tori. No rectangular extension of the full source-free RG theorem is used. The infinite-volume coupling readout is performed at each finite prefix in the retained B02 convention of [The Wilson trajectory on intervals admitting mature resets](../coupling/finite_window.md) before choosing the finite torus large enough to replay that prefix.

## 6. A positive terminal subsequence and fixed physical offsets

By (PE.13), extract a subsequence with
\[
 Y_{K_n'}\longrightarrow Y_\infty\in[Y_-,Y_+],
 \qquad
 g_{K_n'}\longrightarrow
 g_\infty=Y_\infty^{-1/2}>0 .
 \tag{PE.25}
\]
The upper bound on \(g_\infty\) remains below all fixed weak-coupling ceilings.

For every fixed ultraviolet offset \(s\ge0\), the actual couplings at the fixed physical mesh \(\ell_0L^{-s}\) lie in the compact interval
\[
 Y_{K_n'}+as\le
 Y_{K_n'-s}\le
 Y_{K_n'}+Ds .
\]
A countable diagonal subsequence therefore yields
\[
 \widehat Y_s=\lim_nY_{K_n'-s},
 \qquad
 Y_\infty+as\le\widehat Y_s\le Y_\infty+Ds .
 \tag{PE.26}
\]
This is a compatible numerical suffix array drawn from the same finite Wilson trajectories. It is not a new independently selected sequence of finite effective trajectories.

For each fixed offset the rounded radius and the finitely many integer source parameters have only finitely many possible values in this compact range. A further diagonal can make those discrete labels eventually constant at every fixed offset. At a rounding threshold, the constant label can be a one-sided limiting label; its equality with the canonical label computed from \(\widehat Y_s\) requires a closed-graph or chart-matching check. Numeric convergence does not prove that check.

In particular (PE.26) alone does not prove that the limiting suffix array solves the full history-dependent Wilson map. Bounds on an error term pass to subsequences as inequalities. Its exact dependence on the infinite incoming effective state requires convergence and compatibility of that state.

## 7. What continuity has been avoided, and what has not

The construction uses no continuity of \(Y_0\mapsto Y_{K}(Y_0)\) across a rounded \(R_j\) transition. It never asks a prescribed integer-depth trajectory to land at a specified \(Y_*\). It follows each actual trajectory until a common corrected threshold is crossed and then selects a subsequence.

It also does not compare conditional mean laws from unrelated reset decompositions or replace the full E/R/boundary state by the scalar \(Y\). The native projection may depend on that whole state; its all-depth estimate is part of the hypothesis, and its limiting-state continuity is a separate issue.

A sufficient full-state compatibility statement would be the following. At every fixed physical offset and fixed finite spatial region, the actual effective coefficients, positive history kernels and normalized marginal laws admit a common topology in which:

1. the local coefficient families are compact on their genuine admitted charts;
2. contributions from incoming births beyond \(m\) additional ultraviolet levels have a uniform tail tending to zero as \(m\to\infty\), in the same norm used to pass the actual projection and normalization;
3. on each retained discrete grid/selector chart, the finite-window source transformations pass to limits, with either closed-graph control at threshold labels or an exact invariance identifying the different decompositions.

Then extract the full states, pass the finite-window identities, and use the uniform tail to obtain an exact limiting RG/history identity. This is a precise sufficient interface. A scalar recurrence and a diagonal array do not establish its three statements. C05/C08 provide several of their uniform scalar-law ingredients, but neither proves arbitrary transported-mark compactness or the full physical field normalization.

## 8. Comparison with the stated B05 normalization

The following conclusions must be distinguished.

| Assertion | Status under the actual-map assumptions (PE.2) |
|---|---|
| One deterministic cofinal set of genuine bare Wilson coefficients and original cubic tori, with every used source prefix below all weak-coupling ceilings | Proved by (PE.5)–(PE.24), using the fixed B02 source constants and replay convention. |
| A terminal coupling bounded away from zero and a subsequential positive scalar endpoint at scale \(\ell_0\) | Proved by (PE.13), (PE.25). |
| A fixed-offset numerical array extracted from those same trajectories, with the source terminal AF envelope | Proved by (PE.26). |
| A prescribed numerical value \(g_{\rm phys}\) at \(\ell_0\) chosen before the construction | Not proved: \(g_\infty\) is an emergent subsequential value in a compact interval. |
| Compatibility of the complete effective states and actual normalized history maps across cutoffs | Requires the full-state convergence/tail/threshold statement in Section 7, not just scalar diagonalization. |
| Identification with the program's chosen physical observable normalization, and the renormalized continuum fields | Still requires the corresponding B05/F05/M07 matching statements. |

If the physical construction permits choosing **some** sufficiently small positive renormalization condition after extraction, (PE.25) removes the need to shoot to a preassigned scalar endpoint. That is potentially useful for an existence proof. It must be stated as that choice; it does not meet a requirement for a prescribed normalization.

Changing the physical unit or selecting an integer RG offset does not by itself prove equality with an arbitrary prescribed coupling. Such an identification needs the relevant scale/normalization theorem. Likewise a limiting positive \(g_\infty\) is not by itself a proof of nontrivial continuum Yang–Mills fields.

The substantive gain is therefore exact and conditional: **once the actual all-depth B03 stopped-prefix estimate is established, cofinal original-lattice geometry and a positive weak subsequential endpoint need no separate shooting continuity argument.** The remaining B05 question is the specified physical normalization and full-state compatibility, rather than the elementary existence of an admissible numerical stopping sequence.
