# A conditional composition interface for origin-preserving path currents

This note identifies the additional input needed to compose the amended DP path-current interface with one more normalized kernel. It proves an algebraic and normed composition lemma under explicit primitive support, path-admission and reserve hypotheses. It does not supply those hypotheses for an actual third Yang–Mills step.

## 1. What must be retained from the old step

Let F(v) be the old conditional microscopic field, represented by connected physical carrier tags. Keep its occurrence-level primitive representation and the origin labels
\[
 {\cal O}=\{M,0,\ldots,k-1\}.
\]
The label M is the microscopic readout; each other label records one actual normalized-kernel occurrence. Extra explicitly subtracted fields, if present, can keep their own labels.

For an admitted real analytic path gamma(theta) in the old retained variables, write
\[
 j_r[F;\gamma](\theta),\qquad r\in{\cal O},
\]
for the weak current obtained by differentiating the factors owned by r, before changing their integration coordinates. The required old primitive certificate is:

1. The original scalar, each normalized density and its denominator, the actual cutoff faces, and their exact coordinate maps are kept in one value/first-jet registry.
2. For every path used in the composition, the actual joint boundary argument applies in its own latent variables. The field is absolutely continuous along that path and
\[
 \frac{d}{d\theta}F(\gamma(\theta))
       =\sum_{r\in{\cal O}}j_r[F;\gamma](\theta)
       \quad\hbox{for almost every theta}.
 \tag{PC.1}
\]
3. Each normalized kernel's own jet annihilates the constant test. Every origin annihilates a constant microscopic mark.
4. Positive primitive envelopes dominate the path jets by the absolute supported velocity of the actual path, with the required energy grade. The signed current itself need not be a globally defined covector at every retained field.

The new paths in Item 2 are a substantive enlargement of the stored elementary-path list. They cannot be omitted.

### Why elementary finite-current values are not the needed chain-rule input

The next reconstruction will produce
\[
 \gamma_a(\theta)=\Psi_{w(\theta)}(a),
 \tag{PC.2}
\]
at fixed next free coordinate a. This generally changes many old links. It can remain in a cutoff-tie stratum for an interval, even when the ambient exceptional set has zero volume.

For example, the Lipschitz function f(x,y)=|x-y| is constant on the analytic path (theta,theta). At a point of that path its two positive coordinate difference quotients are both one, so they cannot be inserted as components of a linear differential to obtain the zero path derivative. This elementary example concerns the chain-rule inference, not a new Yang–Mills obstruction.

DP avoids that inference by treating the actual path and its spatial latent variables jointly. When boundary sheets coincide jointly on that spacetime chart, their derivatives along that path and its spatial transport agree. At the remaining path times, ties have zero boundary measure, except on a null set of times. This argument can be reapplied to (PC.2) if its actual reconstruction and boundary hypotheses are proved. Merely retaining the numbers \(J_{d,t}^{r,\mathrm{path}}\) on elementary paths does not retain this primitive admission or tie calculation.

## 2. The next normalized kernel and the precise assumptions

Let
\[
 p_w(da)=\frac{N_w(da)}{Z_w},\qquad Z_w=N_w(1)>0,
 \qquad F^+(w)=\int p_w(da)\,F(\Psi_w(a)).
 \tag{PC.3}
\]
This is the fixed actual next kernel at zero microscopic source. It is independent of the observable F in this linear transport theorem. Its density N, all measure/coarea factors, its moving domains, its full inherited unmarked mass factors and its own denominator are retained. An inherited mass belongs to the new density when that is its actual occurrence there. Higher source-dependent kernels would require separate source-jet bookkeeping; they are not silently treated as a fixed linear operator here.

For every buffered elementary new path w(theta), assume the following.

**P1 — actual lifted-path admission.** The reconstruction is analytic on the needed real and coefficient tubes. Every lifted path (PC.2) met by the new kernel is admitted for the old primitive path certificate, including its boundary traces and a local parameter collar. The old cutoffs and the new cutoff admit the joint shape/product rule on the actual independent latent variables. No delta constraint between old and new slots is inferred after the exceptional variables have been eliminated.

**P2 — a common normalized first-jet family.** The old primitive factors and the new kernel have one component-compatible pullback family, with the full triangular coordinate change and its Lie/divergence terms. Each occurrence's physical origin is assigned before any change of variables or cancellation. Numerator and denominator jets for each conditional are identical occurrences of its own normalization construction. In particular,
\[
 p_{w,s}(1)=1,\qquad \dot p_{w,s}^{\,new}(1)=0.
 \tag{PC.4}
\]
These identities must hold in the continued component family where normalization and coefficient extraction are performed. P2 does not assert that a completed moving-cutoff normalizer is an analytic local coefficient.

**P3 — supported primitive transfer and joint reserves.** The actual reconstruction velocity, old positive root envelopes, new signed kernel response, and all normalization terms have physical carrier certificates. Their coefficientwise integrals satisfy the three positive transfer bounds stated in Section 4. These are joint energy/velocity and normalized response bounds, not consequences of numerical covariance decay alone.

**P4 — dominated common path integration.** The same deterministic coefficient envelopes hold over the entire required path, its fixed coefficient/source polydiscs, and the declared boundary/contour families. They justify Fubini, weak differentiation, coefficient extraction and subsequent path integration. Any adaptive radius is specified across that box.

At finite volume, positive continuous normalizers may justify the quotient identity. Uniform estimates in P3 must still come from the actual connected normalization; a local-in-parameter lower bound for an extensive Z is not a quantitative substitute.

## 3. Exact composition and origin ownership

For old r define
\[
 j_r^+[F;w](\theta)
   =\int p_{w(\theta)}(da)\,
                  j_r[F;\gamma_a](\theta).
 \tag{PC.5}
\]
Introduce exactly one new label, with
\[
 j_{new}^+[F;w](\theta)
   =\bigl(\partial_\theta p_{w(\theta)}|_a\bigr)
                     [F(\Psi_{w(\theta)}(a))].
 \tag{PC.6}
\]
The test in (PC.6) is held fixed when differentiating the kernel. All dependence of the new density or denominator, including an earlier mass that occurs inside them, belongs to the new label. It is not reassigned to the old label whose equal-valued mass may occur elsewhere.

### Lemma PC.1 — exact path-origin composition

Under P1–P4, F-plus is locally absolutely continuous on the stated new paths, and
\[
 \frac{d}{d\theta}F^+(w(\theta))
      =\sum_{r\in{\cal O}}j_r^+[F;w](\theta)
                       +j_{new}^+[F;w](\theta)
       \quad\hbox{a.e.}
 \tag{PC.7}
\]
The same identity holds tag by tag in the common value/first-jet family. Integrating each term from zero to t and dividing by t gives finite path records whose sum is the exact normalized finite difference. Every old label is retained, one new kernel label is added, and each label vanishes on a constant microscopic mark.

**Proof.** Apply the actual joint weak product rule from P1 to the old primitive integral and the new density. Terms differentiating old factors give (PC.5) by their original ownership. Terms differentiating the new density, its domain and its denominator give (PC.6). P2's triangular transport identities preserve the sum after the common change of variables, including all boundary fluxes.

The new normalized response is exactly
\[
 \dot p_w[G]
  =Z_w^{-1}\dot N_w[G]
       -p_w[G]\,Z_w^{-1}\dot N_w[1]
  =Z_w^{-1}\dot N_w[G-p_wG].
 \tag{PC.8}
\]
This identity includes the smooth and boundary parts of the signed derivative. For G=1 it vanishes by its own normalization. The old labels vanish on a constant by the old certificate, so their averages (PC.5) vanish as well. A cancellation between distinct origins is not needed.

At the occurrence level one uses the first-jet inverse rule before canceling equal zero-jet masses. This preserves (PC.8) even when an old normalizer and an inherited factor in the new density have equal values and different labels. Common component restriction and exact disjoint-vacuum cancellation then preserve the identity under coefficient extraction. P4 permits the a.e. derivatives to be integrated termwise. The oriented integral also covers negative t. This proves all assertions. ∎

This proof adds no physical branching of origin labels. Repeated latent copies introduced by connected normalization keep their original ownership; they do not create new kernel generations.

## 4. What the quantitative transfer must control

Use old and new positive regulators \(R_X^-(v)\), \(R_Z^+(w)\), with their shifted versions, and physical carrier weights \(w_-(X)\), \(w_+(Z)\). Let the old dimensionless pointwise budgets be represented by numbers \(v_X,j_{r,X}\):
\[
 |h_-^4F_X(v)|\le v_X R_X^-(v),
 \qquad
 |h_-^4j_r[F_X;\gamma](\theta)|
       \le j_{r,X}\,\mathcal V_X[\gamma](\theta).
 \tag{PC.9}
\]
Here \(\mathcal V_X\) is the actual positive primitive velocity/energy envelope. For an elementary path it has the old shifted grade \(3/2\). For a lifted path it must retain the normalized coefficients of \(\partial_\theta\Psi\), their genuine raw footprints and the old energy factor before the next integration.

In particular, those normalized velocity coefficients use the old coordinate normalization. A new physical link step of size \(g_+\) produces ratios \(g_+/g_-\); they are retained in the actual transfer constants, not set to one.

P3 means there are nonnegative matrices \(A_{ZX},B_{ZX},N_{ZX}\) obtained from the actual primitive/component construction, with the following bounds:

* The value pullback and integration of its positive root envelope give \(A_{ZX}R_Z^+\).
* The integral of the supported lifted-path envelope \(\mathcal V_X[\gamma_a]\) gives \(B_{ZX}(\widehat R_Z^+)^{3/2}\), for each old origin with the same matrix B, after the actual sum of new directions.
* The connected new-kernel response to the old value envelope gives \(N_{ZX}(\widehat R_Z^+)^{3/2}\), including its own normalizer response and boundary surfaces.

The value and response coefficients themselves must be supported in Z; an estimate for a globally dependent positive mass is not enough. Each matrix entry retains the actual source, velocity, covariance, reference, gauge, constraint and normalization carriers. The requested weighted column sums are
\[
 \sum_Zw_+(Z)A_{ZX}\le A\,w_-(X),\qquad
 \sum_Zw_+(Z)B_{ZX}\le B\,w_-(X),\qquad
 \sum_Zw_+(Z)N_{ZX}\le N\,w_-(X).
 \tag{PC.10}
\]
Direction incidence and the finite-path supremum are included in these common envelopes. The common shifted new regulator controls every real endpoint and current-parameter value used in the integral.

These assumptions expose a concrete analytic gate. Separate bounds for the old energy and for the reconstruction velocity do not imply their joint conditional bound in the second bullet. Neither does a positive real covariance comparison supply the physical carriers, sharp-domain continuation or connected denominator response in the third bullet. Those must be proved for the actual next law.

### Lemma PC.2 — triangular budget transfer

Set
\[
 V=\sum_Xw_-(X)v_X,\qquad
 J=\sum_r\sum_Xw_-(X)j_{r,X},\qquad
 s_h=(h_+/h_-)^4.
\]
Under PC.10 the next native pointwise value and total origin-current budgets obey
\[
 V^+\le s_h A V,\qquad
 J^+\le s_h(BJ+NV).
 \tag{PC.11}
\]
For each old origin separately,
\[
 J_r^+\le s_hB J_r,\qquad
 J_{new}^+\le s_hNV.
 \tag{PC.12}
\]

**Proof.** Apply the positive primitive bounds to each old value/current tag, sum with the new physical weight, and use the column sums PC.10. No cancellation of different origins is used. Multiplication by \(h_+^4\), instead of \(h_-^4\), gives the displayed factor \(s_h\). P4 bounds the finite path integrals by the same envelopes, so they have the identical estimate. ∎

The constants are the same for every retained old label only when P3 proves that uniformity. It is an assumption to be checked, not a benefit automatically obtained by naming the old labels.

## 5. The depth requirement exposed by the recurrence

For successive steps put \(a_j=s_jA_j\), \(b_j=s_jB_j\), and \(n_j=s_jN_j\). Iteration of the proved triangular inequality gives
\[
 V_m\le V_0\prod_{j=0}^{m-1}a_j,
\]
\[
 J_m\le J_0\prod_{j=0}^{m-1}b_j
  +V_0\sum_{\ell=0}^{m-1}
       n_\ell
       \left(\prod_{j<\ell}a_j\right)
       \left(\prod_{j>\ell}b_j\right).
 \tag{PC.13}
\]
Each summand corresponds to the single kernel-origin label born at step ell. There is no extra factor \(2^m\) from duplicating the old origin list. The products can nevertheless grow rapidly: fixed bounds \(A_j,B_j\le C\) do not give a depth-uniform theorem.

For example, after whatever physical renormalization has actually been proved, bounds \(a_j,b_j\le1+\epsilon_j\) with \(\sum_j\epsilon_j<\infty\), together with \(\sum_j n_j<\infty\), would give a uniform budget through PC.13. If \(n_j\) is merely bounded and the two products are controlled, this formula still permits linear growth in the number of generations. The unrenormalized factor \(s_j=L^4\) is explicit and has not disappeared into a newly inflated incoming budget.

A previously rare component also retains its initial small factor through these linear positive transfer maps. That fact is useful only if the products and accumulated normalization costs in PC.13 are controlled; it does not by itself prevent a finite rare reserve from being exhausted at large depth.

## 6. Consequence and exact outstanding input

The amended current interface is algebraically stable under exact normalized composition once the retained primitive path certificate admits the actual lifted paths and the three supported transfer bounds are proved. Identity cancellation is preserved separately for every kernel occurrence. Linear scalar/identity extraction is compatible: constants generate no kernel current, and a subtracted scalar keeps its explicit extraction-current label.

For an actual third step the work still required is specific:

1. Admit the old nonanalytic cores and their independent latent copies on the new reconstructed paths, including paths lying inside tie strata.
2. Construct the common constrained frames and first-jet occurrence registry for those paths with the actual new inherited density and all normalizers.
3. Prove the joint supported energy–velocity integral and the connected new-kernel response in PC.10, with the true cutoff units, physical coupling ratios and rank costs.

DP and MB prove their own two-level versions; they do not verify these third-step hypotheses. The real ancestral Gaussian comparison can be an input to a future reserve estimate, but is not a replacement for these common complex/interacting and cutoff-support checks. No actual third-step bound, uniform-depth marked recursion, averaged M03 norm or Yang–Mills existence result is claimed here.
