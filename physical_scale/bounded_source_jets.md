# Bounded source jets and uniform integrability

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

## 1. Result and scope

The finite-volume mixed-kernel calculation left a specific alternative to raw-variable
equicontinuity: retain a larger joint state on which the actual kernel
compositions and source probes converge together. The companion
mixed kernel composition constructs that state for bounded
probes. This paper supplies the source-jet and component-mass interface.

There are two useful conclusions. First, a complete mass-weighted
canonical cumulant is continuous in a finite list of joint moment
coordinates, even at zero component mass. Total-variation convergence
on a common raw reference space is unnecessary for this passage.
Second, finite source jets and their logarithms pass through the
limiting conditional kernels with all incoming higher vertices and
outer conditional means retained. An explicit uniform-integrability
criterion extends the statement to unbounded probes.

The original compact energy reserve verifies that criterion for
dimensionless microscopic energy representatives. The physical
dimension-four factors and the prescribed running normalization remain
explicit. This result closes the bounded-source composition interface;
it does not supply the recent-separated physical estimate ER.7 or
the spatial matching estimates of M04–M07.

## 2. The positive moment cone

Fix labeled insertions \(f_1,\ldots,f_m\), with positive bounds
\(r_i\). Write \(r_I=\prod_{i\in I}r_i\) and \(r_\varnothing=1\).
The functions and their underlying spaces may vary with the cutoff.
For a finite positive measure \(\mu\), put
\[
 v_I=\mu\!\left(\prod_{i\in I}f_i\right),
 \qquad v_\varnothing=\mu(1).
 \tag{BJ.1}
\]
If \(|f_i|\le r_i\), then
\[
 v_\varnothing\ge0,\qquad |v_I|\le r_Iv_\varnothing.
 \tag{BJ.2}
\]
Complex insertions are allowed; the underlying measure is positive.
It suffices to work on the closed convex cone defined by (BJ.2),
which contains every actual moment vector. Additional positivity
relations are retained when a representing measure is needed.

For \(v_\varnothing>0\), define
\[
 \mathcal C_m(v)=
 \sum_{\pi\in\Pi_m}
 (-1)^{|\pi|-1}(|\pi|-1)!\,
 v_\varnothing^{\,1-|\pi|}
       \prod_{B\in\pi}v_B .
 \tag{BJ.3}
\]
This is the mass times the normalized conditional cumulant. Define
\(\mathcal C_m(0)=0\). Zero bounds \(r_i=0\) can be removed separately:
every term containing that insertion is then identically zero.

Let
\[
 B_m=\sum_{\pi\in\Pi_m}(|\pi|-1)!,
 \qquad
 L_m=\sum_{\pi\in\Pi_m}
       (2|\pi|-1)(|\pi|-1)!.
 \tag{BJ.4}
\]
Counting ordered set partitions by their block-size compositions gives
\[
 B_m\le 2^{m-1}m!,\qquad L_m\le 2^m m!.
 \tag{BJ.5}
\]
Indeed, \(\sum_r r!S(m,r)\) is at most \(m!\) times the
\(2^{m-1}\) compositions of \(m\); the exact contribution for a
composition \((n_1,\ldots,n_r)\) is
\(m!/(n_1!\cdots n_r!)\). Also
\((2r-1)(r-1)!\le2r!\).

### Theorem BJ.1 — continuity through zero mass using joint moments

For any two vectors \(v,w\) satisfying (BJ.2),
\[
 |\mathcal C_m(v)|\le B_m r_{[m]}v_\varnothing,
 \tag{BJ.6}
\]
and
\[
 |\mathcal C_m(v)-\mathcal C_m(w)|
 \le L_m r_{[m]}
       \max_{I\subseteq[m]}
             \frac{|v_I-w_I|}{r_I}.
 \tag{BJ.7}
\]
Thus the complete coefficient is continuous on the closed cone,
including its zero-mass vertex. The two vectors need not arise from
measures on the same raw space.

**Proof.** For a partition with \(r\) blocks, (BJ.2) bounds its
mass-weighted monomial by \(r_{[m]}v_\varnothing\), proving (BJ.6).
For (BJ.7), use the segment \(v(t)=(1-t)v+tw\), which stays in
the cone. Wherever its mass is positive, differentiation of the
partition monomial gives \(r\) moment derivatives and \(r-1\)
mass derivatives. If
\[
 d(v,w)=\max_I |v_I-w_I|/r_I,
\]
their total absolute value is at most
\((2r-1)r_{[m]}d(v,w)\): every apparent negative power of
\(v_\varnothing(t)\) is cancelled by the other moment bounds
in (BJ.2). Integrate over the segment and sum the partition
coefficients. At a zero-mass endpoint use (BJ.6) to pass to
the endpoint. If both masses vanish, both vectors are zero.
\(\square\)

This strengthens the mode of convergence available in the earlier
MW lemma. It does not assert that weak convergence of each raw
multiplier separately suffices: the joint product moment coordinates
in (BJ.1) must actually converge together.

## 3. Passing complete canonical coefficients

Let \(K\) be a compact metrizable joint probe space. Suppose the
coordinates \(v_I\) are continuous on \(K\), satisfy (BJ.2),
and \(v_\varnothing\le M\). Let \(\rho_n\) be laws on \(K\)
converging weakly to \(\rho\). Then, for every continuous bounded
probe \(a\),
\[
 \int a\,\mathcal C_m(v)\,d\rho_n
 \longrightarrow
 \int a\,\mathcal C_m(v)\,d\rho.
 \tag{BJ.8}
\]
Theorem BJ.1 proves that the integrand is continuous and bounded.
The same conclusion holds jointly for any finite polynomial in these
complete coefficients and other retained bounded coordinates.
One countable joint algebra handles all fixed orders on a single
subsequence.

If the expression is divided by one global normalization \(Z_n\),
it is enough that \(Z_n\to Z>0\). No lower bound on every individual
component mass is needed. At fixed terminal volume the normalized
joint-law construction already incorporates \(Z_n\); when an
unnormalized presentation is used, H2S.14a supplies its stated
finite-volume lower bound. That lower bound is not promoted to a
positive constant uniform in an expanding terminal volume.

### Exact application to the source component grouping

The literal source formula is
\[
 \left(\prod_i\tau_i\right)
       \left[\left(\prod_i\Pi_i\right)F\right]
   =\left(\prod_iT'_i\right)F,\qquad
 \tau_i=T'_i1,\quad \Pi_i=\tau_i^{-1}T'_i.
 \tag{BJ.9}
\]
These are LFR II (1.103)–(1.104), and FK.9–FK.10.
The operations are kept in their actual chronological order.
Product factorization is used only for the disjoint component
family for which the source gives it.

For real source-free data each \(T'_i\) is a positive finite
measure operation. For bounded insertions, retain the moments
of the complete product measure in (BJ.9), including every unused
mass. A positive common interaction factor, if present in the
complete unlocalized branch, can be included in that same
measure. This preserves (BJ.2).

For the literal canonical components of LFR II (1.71), the
source's bound (1.89), printed p.387, gives
\[
 0\le\tau_i\le
 \exp[-2(1+\beta_0)^{-1}p_0(g_k)]\le1.
 \tag{BJ.9a}
\]
Here \(\beta_0\) is the source's fixed comparison parameter,
not the Wilson coefficient. The source allows both component
classes in (1.71), and (1.103) identifies the retained
second-class multiplier with this same \(T'_i1\).
Thus the mass of the complete disjoint product in (BJ.9)
is at most one. Its bounded product moments can be included
directly in the joint state.

If a positive interaction factor is moved into that measure,
its actual scalar value bound must also be retained. On a
fixed active-cost, geometry and finite-volume truncation,
the finite native-root count and the source value bounds
supply the stated finite bound for such a bounded interaction.
Explicitly, for a real scalar \(B'\),
\[
 \mu^{B'}(1)
   =\left(\prod_iT'_i\right)e^{B'}
   \le e^{\sup B'}\prod_i(T'_i1).
 \tag{BJ.9b}
\]
The bound is used only on the truncation where the complete
\(\sup B'\) has its proved finite native-volume bound.
This is not a blanket envelope for every unnormalized mixed
branch density. No common cross-cutoff Haar/coarea density
is asserted.

Equation (BJ.8) now passes each complete mass-retaining coefficient.
It does not pass an isolated normalized logarithm after its
outside mass has been discarded. It also does not multiply
separately extracted weak limits of the \(\tau_i\): the complete
product moments are part of the joint state from the start.

## 4. Exact finite jets under the limiting kernels

Use distinct labels even when two insertions are the same observable.
Let \(\varepsilon_i^2=0\), with commuting nilpotent variables, and
write the actual conditional moment jet at a cut \(s\) as
\[
 Z_s(\varepsilon)=
 \sum_{I\subseteq[m]}\varepsilon_I M_{I,s},
 \qquad M_{\varnothing,s}=1 .
 \tag{BJ.10}
\]
For bounded insertions the coefficients are bounded physical probes.
The joint kernel construction includes their products and every
actual normalized kernel pullback. If \(P_{t,s}\) is the limiting
backward kernel between two retained cuts, its exact prelimit
source identity passes to
\[
 Z_t=P_{t,s}Z_s.
 \tag{BJ.11}
\]
The finite logarithm is a polynomial in the \(M_{I,s}\):
\[
 H_s=\log Z_s,\qquad
 [\varepsilon_I]H_s
   =\sum_{\pi\in\Pi(I)}
       (-1)^{|\pi|-1}(|\pi|-1)!
                  \prod_{B\in\pi}M_{B,s}.
 \tag{BJ.12}
\]
All those products belong to the jointly retained algebra. Hence
\[
 H_t=\log P_{t,s}e^{H_s}.
 \tag{BJ.13}
\]
This is the complete finite-jet transformation, with every incoming
higher vertex. It needs no common zero-free disk for a complex
exponential source.

For a chain of cuts, the Feller kernels of the companion construction
satisfy their actual composition identities. Consequently the
right side of (BJ.11) is independent of how a fixed finite chain is
parenthesized. The logarithmic jets inherit that compatibility.
Restriction from \(m+1\) labels to \(m\) commutes with every operation.
The outer marginal identity
\[
 \int M_{I,t}\,d\rho_t
     =\int M_{I,s}\,d\rho_s
 \tag{BJ.14}
\]
passes at the same time. In particular the full second cumulant
retains both the averaged conditional covariance and the covariance
of conditional means. No within-sector covariance is substituted
for their sum.

The scalar formula is elementary; the substantive requirement is
the simultaneous joint-state and kernel construction. Separate
weak-* limits of the coefficient functions do not justify (BJ.12).

## 5. A uniform-integrability theorem for unbounded probes

Here the probability space and the sigma-field may vary with \(n\).
Let \(\mathcal G\) be a sigma-field in an actual positive full law,
and denote the conditional cumulant by
\(\kappa_{\mathcal G}(X_1,\ldots,X_m)\).

### Lemma BJ.2 — complete conditional-cumulant moment bound

For \(q\ge1\),
\[
 \|\kappa_{\mathcal G}(X_1,\ldots,X_m)\|_{L^q}
 \le B_m\prod_{i=1}^m\|X_i\|_{L^{qm}}.
 \tag{BJ.15}
\]
The bound is uniform in the cut and its actual conditional masses.

**Proof.** For each partition \(\pi\), apply Holder to its block
moments with exponents \(m/|B|\):
\[
 \left\|\prod_{B\in\pi}
       \mathbb E[X_B\mid\mathcal G]\right\|_q
 \le
 \prod_{B\in\pi}
       \|\mathbb E[X_B\mid\mathcal G]\|_{qm/|B|}
 \le
 \prod_{i=1}^m\|X_i\|_{qm}.
 \tag{BJ.16}
\]
The second inequality uses conditional-expectation contraction and
Holder within each block. Sum the absolute partition coefficients.
\(\square\)

Multilinearity gives the corresponding stability bound. If
\(\|X_i\|_{qm},\|Y_i\|_{qm}\le A_i\), then
\[
 \|\kappa_{\mathcal G}(X)-\kappa_{\mathcal G}(Y)\|_q
 \le B_m\sum_{j=1}^m
       \|X_j-Y_j\|_{qm}\prod_{i\ne j}A_i.
 \tag{BJ.17}
\]
This follows by replacing the arguments one at a time.

For a \(\mathcal G\)-measurable event \(A\) and \(q>1\),
\[
 \left|\mathbb E[
       \mathbf1_A\kappa_{\mathcal G}(X)]\right|
 \le \mathbb P(A)^{1-1/q}
       B_m\prod_i\|X_i\|_{qm}.
 \tag{BJ.18}
\]
Its probability is that of the normalized full law. It cannot be
replaced by a component mass already cancelled from a posterior.

### Theorem BJ.3 — removing bounded source truncations

Suppose that, for each required fixed order \(m\), the actual
insertions satisfy a cutoff-uniform \(L^{m+\delta}\) bound for
some \(\delta>0\). Retain a countable set of truncation levels
in the joint probe construction. Then all order-\(m\) conditional
moment and cumulant identities pass to the joint limit in the
integrated sense, with the bounded truncations removed.

If identities are required in \(L^q\), replace \(m+\delta\) by
\(qm+\delta\). If all fixed orders have these bounds, the same
countable construction handles all orders and cuts.

**Proof.** With \(X^{[R]}\) the radial clipping at \(R\),
\[
 \|X-X^{[R]}\|_p
 \le R^{-\delta/p}
       \|X\|_{p+\delta}^{\,1+\delta/p}.
 \tag{BJ.19}
\]
This tends to zero uniformly in the cutoff. Conditional moment
products obey the same telescoping estimate as (BJ.16), and
(BJ.17) handles cumulants. Thus the bounded truncations are
Cauchy in the required integrated norm, uniformly over cuts.
Their joint limiting laws inherit the same bounds by lower
semicontinuity, or directly by applying the bounds to successive
bounded truncations. The limiting kernels preserve their
marginals and are contractions in these \(L^p\) spaces.
Pass first at fixed \(R\), then let \(R\to\infty\).
This proves the identities and their compatibility.
\(\square\)

The theorem concerns genuine joint moment bounds. A bound only on
the probability of the geometry, or a pointwise compactness
statement for a raw multiplier, does not supply its hypothesis.
In particular a signed bound on separated smeared correlations
must not be silently promoted to pointwise absolute moments.

## 6. Actual application supplied by the compact Wilson reserve

For the centered fixed microscopic representatives of CS.1, set
\[
 X_{\alpha,a}(x)
   =a^4\left[
       \beta_a\widetilde q_{\alpha,a}(x)
       -\mu_a(\beta_a\widetilde q_{\alpha,a}(x))
       \right].
 \tag{BJ.20}
\]
The fixed finite F01 clovers, their scalar repair, and the original
normalized compact energy reserve give
\[
 \|X_{\alpha,a}(x)\|_p\le Cp,\qquad p\ge1,
 \tag{BJ.21}
\]
uniformly along the admitted sequence. This is exactly CS.2 with
its displayed physical factor multiplied through; the microscopic
insertion has not been replaced by a current-scale stencil.

For any fixed countable collection of such microscopic probes and
actual cuts, BJ.3 applies at every order. Furthermore
\[
 \|\kappa_{\mathcal G}
       (X_{\alpha_1,a}(x_1),\ldots,X_{\alpha_m,a}(x_m))\|_q
 \le C_1^m(m!)^2q^m .
 \tag{BJ.22}
\]
Indeed (BJ.15) gives \(B_m(Cqm)^m\), and
\(m^m\le e^m m!\). This is a fixed factorial budget for the
complete conditional logarithmic jet in an averaged value norm.
It is uniform in the number and type of source-free operations.
Reality and any exact finite reflection/tensor identities included
in the generating probes pass with the same joint construction.

These variables are dimensionless microscopic representatives.
Restoring the physical field multiplies the \(m\)-point coefficient
by \(a^{-4m}\). For the prescribed F01 fields an additional
\((\|Z_a\|/\beta_a)^m\) budget remains after the identity-budget
reduction in physical normalization. Neither factor
is paid by (BJ.22). The actual spatial matching and recent-separated
estimate remain necessary.

## 7. What is closed and what is still required

Together with the companion kernel construction, the results close
the following specific interfaces:

1. Joint bounded archived probes and normalized kernel compositions
   have a common enlarged-state realization.
2. Complete mass-retaining canonical cumulants pass through that
   limit without an individual lower component mass or a common raw
   total-variation reference.
3. The full finite source jet, its conditional logarithm, higher
   vertices and outer marginal identities pass compatibly at every
   fixed order.
4. The original compact moment reserve permits actual removal of
   truncations for dimensionless microscopic energy representatives.

The enlarged state includes predictive archive information. Its
kernel need not be a function of naked active raw coordinates alone.
Hard selector labels retained as coordinates are not thereby
identified with recomputation of every canonical limiting selector.
The full physically normalized ER.7 bound, the actual seven-channel
mixing estimates and all remaining frozen existence requirements
retain their separate status.
