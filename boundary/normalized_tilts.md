# Normalized tilts, local cumulants and summable induction

**Composed-response hypothesis (CR).** Each complete boundary conclusion below assumes the displayed native-chart and spatial response estimates for the actual iterated reconstruction, with the prescribed earlier innovations and raw variables fixed, uniformly over the admitted histories. A sufficient estimate for the latent contribution is (A.8) in [Conditional-law estimates and the continuum application](../continuum/conditional_to_continuum.md), refined for the anchored exterior derivative in PG.18–PG.20. The two endpoint bounds concern the identical Wilson-subtracted primitive, its actual cutoff and its independently extended current. A direct minimizing-field derivative alone does not establish this hypothesis. The application to every required original Wilson history remains open. Complete boundary estimates and their C06/C08 applications in this chapter are conditional on CR and the other displayed source, AF, domain and support assumptions. Exact density identities and abstract inequalities retain their individually stated hypotheses.

In the projective density formulation, a sufficient comparison is
\[
 \sup_{\zeta,x,a}\left|
 \log\frac{W_\zeta(x,a)W_0(x,a_*)}
               {W_0(x,a)W_\zeta(x,a_*)}
 \right|\le\delta_r<\pi/2,
\]
on the stipulated chart with the required uniform rates and actual fixed support. The composed ordinary response is the unresolved input in its derivation. The exact partial-gauge transport and the surviving fixed-exterior derivative are given in the chapter [Gauge covariance of partial integrals and exterior scores](../continuum/partial_gauge_transport.md), equations PG.2–PG.6 and the subsequent anchored-score criterion.

**Scale convention.** The Ward estimate uses the evaluation age $n-b$. When $b\le n<j$, one also needs decay in the forcing age $j-n$. The latter response for the actual composed field, with earlier innovations fixed, is conditional on CR. The two-age interpolation SR.12–SR.24 is used here in place of the one-age calculation of OR.19.

The analytic and numerical lemmas imply the complete boundary estimates under CR and the compatibility conditions in §8.

## 1. Fixed fibers and the actual normalization

Fix the admitted history, the unintegrated real raw tuple, and a branch of every hard selector. Write these data as x. Let A_x be the actual common support of the coordinates a integrated by a stopped prefix. All identities below are on this fiber. Neither x nor a is analytically continued merely because an external native parameter z is complexified.

Let nu_x be a positive probability on A_x. Suppose an ordinary normalized kernel mu_z has a density satisfying

\[
  \mu_z1=1,\qquad |d\mu_z(a)|\le M_0\,d\nu_x(a),
  \qquad M_0\ge1.
  \tag{RT.1}
\]

The same nu_x must work for every z on the common working chart. Uniform scalar operator norms alone are not substituted for (RT.1).

Let V_z(a) be the additional, literal interaction. A scalar c_z(x), independent of every coordinate integrated on this fiber, can be removed from its normalized tilt. Put D_z=V_z-c_z and assume

\[
  \sup_{z,a\in A_x}|D_z(a)|\le\delta,
  \qquad u=e^\delta-1,
  \qquad M_0u<1.
  \tag{RT.2}
\]

This assumption concerns the complete action oscillation. It does not require each inherited term to possess a larger analytic radius.

## 2. Nonvanishing and a common positive reference after a full tilt

**Lemma RT.1.** For real 0<=t<=1, define

\[
 Z_t(z)=\mu_z(e^{tD_z}),\qquad
 \mu_{t,z}F={\mu_z(e^{tD_z}F)\over Z_t(z)}.
 \tag{RT.3}
\]

Then, uniformly in t and z,

\[
 |Z_t-1|\le M_0u,
 \qquad |Z_t|\ge1-M_0u,
 \qquad
 |d\mu_{t,z}|\le M\,d\nu_x,
 \quad
 M={M_0e^\delta\over1-M_0u}.
 \tag{RT.4}
\]

For a fixed upper bound on M_0 and sufficiently small delta,

\[
 {M\over M_0}\le1+C\delta.
 \tag{RT.5}
\]

**Proof.** Subtract mu_z(1)=1 inside Z_t. The exponential series gives |e^{tD}-1|<=u, so (RT.1) gives the first two inequalities. Applying (RT.1) to the numerator density gives the third. The last claim follows by expanding, or directly bounding, e^delta/(1-M_0(e^delta-1)) on a fixed small interval. This proves the claim for the actual complex kernel; no Gaussian replacement is involved.

The removed scalar is still present in the unnormalized action:

\[
 \mu_z(e^{V_z})=e^{c_z}Z_1(z).
 \tag{RT.6}
\]

Its derivatives must be retained in the outer action. Only its cancellation from the normalized conditional kernel has been used.

## 3. Exact moving-normalizer response

Differentiation of the quotient in (RT.3) gives

\[
 {d\over dt}\mu_{t,z}F
 =\mu_{t,z}(FD_z)-\mu_{t,z}F\,\mu_{t,z}D_z
 =\operatorname{Cov}_{\mu_{t,z}}(F,D_z).
 \tag{RT.7}
\]

The covariance is algebraic and is well defined for the normalized complex functional. The second term is the response of the moving mass. Consequently

\[
 (\mu_{1,z}-\mu_{0,z})F
 =\int_0^1\operatorname{Cov}_{\mu_{t,z}}(F,D_z)\,dt.
 \tag{RT.8}
\]

An equally useful exact formula, obtained without differentiating, is

\[
 (\mu_{1,z}-\mu_z)F
 ={\mu_z(Fv_z)-\mu_zF\,\mu_zv_z\over1+\mu_zv_z},
 \qquad v_z=e^{D_z}-1.
 \tag{RT.9}
\]

In particular constants are annihilated exactly. A bound on the first numerator term in (RT.9) is not a bound on the whole normalized response unless the second is included.

### 3.1 Positive analytic families, with raw supremum in the required place

Suppose nonnegative weights w_G, independent of z and a, satisfy

\[
 \sum_Gw_G\sup_z|F_G(z,a)|\le K
 \quad\hbox{for every }a\in A_x.
 \tag{RT.10}
\]

Then

\[
 \sum_Gw_G\sup_z|\mu_{t,z}F_G|\le MK,
 \tag{RT.11}
\]

and

\[
 \sum_Gw_G\sup_z
 |(\mu_{1,z}-\mu_{0,z})F_G|
 \le(M+M^2)\delta K.
 \tag{RT.12}
\]

**Proof.** For (RT.11), dominate every integrand by M nu_x, take the analytic supremum inside its positive integral, and apply Tonelli to (RT.10). For the first covariance term in (RT.7), the same calculation gives M delta K. For the product of expectations, apply (RT.11) to the F_G factor and |mu_tD|<=M delta to the other. Integrate over t. All labels can be placed in one measurable union, with absent terms set equal to zero. The outer supremum in x is taken only after these inequalities have been proved for each x.

Thus arbitrary bounded measurable dependence on old raw coordinates is allowed. Analyticity in those raw variables has not been assumed.

### 3.2 Marked perturbations and new spatial roots

If D= sum_e D_e, apply (RT.7) before taking absolute values and retain the label e in each covariance term. For every finite subcatalog the identity is exact. Absolute convergence permits passage to the full catalog. This identifies the positive records that a physical-root estimate must pay:

\[
 (G,e)\longmapsto
 \mu_t(F_GD_e)-\mu_tF_G\,\mu_tD_e.
 \tag{RT.13}
\]

Both terms carry the same marked record e. A root on the added part of e must be paid by the two-endpoint majorant of e. A root on G can use its old rooted norm. An unrooted bound for D does not by itself prove the new-root sum. This is the precise interface with the companion rooted-interaction proof.

## 4. Absolute action smallness requires only an anchored difference

Choose any a_* in the actual nonempty support A_x. No assumption that zero belongs to that support is necessary. Define

\[
 D_z(a)=V_z(a)-V_z(a_*).
 \tag{RT.14}
\]

All contributions independent of a cancel. If V= sum_G V_G, the required bound is therefore on

\[
 \sum_G\sup_z|V_G(z,a)-V_G(z,a_*)|,
 \tag{RT.15}
\]

not on the full volume sum of |V_G|. A term with explicit raw dependence can be charged to an actually used raw slot. A term with native-only dependence must first be differenced through the actual native map; its response records then have an actual forcing endpoint. Counting every old fine cell in the final component would not establish (RT.15).

Suppose the proved root conversion for an incoming catalog gives

\[
 \sup_{x,a,a_*}\sum_G\sup_z
 |V_G(z,a)-V_G(z,a_*)|
 \le d_r A_{r-1},\qquad d_r\le C g_r^{-u}\ell_r^D.
 \tag{RT.16}
\]

Then the additional actual-law tilt in a scale-r prefix has delta<=d_r A_{r-1}. This is a use of the incoming capacity only. The output capacity A_r or any current-stage marginal is not assumed.

## 5. A quantitative tail from the stipulated AF profile

Write T_r=g_r^{-2} and ell_r=log T_r. Use the admitted two-sided AF profile only through the lower bound

\[
 T_b\ge c_{\rm AF}[T_r+(r-b)]\quad(b\le r).
 \tag{RT.17}
\]

Assume T_r is above a common fixed threshold. Let

\[
 f_b\le C_f(\log T_b)^d
                  e^{-c_0(\log T_b)^p},\qquad p>1.
 \tag{RT.18}
\]

**Lemma RT.2.** For each 0<c_1<c_0, after increasing the common threshold,

\[
 F_r:=\sum_{b\le r}f_b
 \le C_1 e^{-c_1\ell_r^p}.
 \tag{RT.19}
\]

The constants are independent of the ultraviolet starting scale, cutoff depth and admitted history. The same conclusion holds after multiplying f_b by any fixed power of log T_b.

**Proof.** The function u -> (log u)^d exp[-c_0(log u)^p] is decreasing for large u. Apply (RT.17), compare the sum to an integral, and change variables t=log u. Apart from a fixed factor and the first summand, the result is bounded by

\[
 \int_{\log(c_{\rm AF}T_r)}^\infty
       t^d e^{t-c_0t^p}\,dt.
 \tag{RT.20}
\]

For large t, the derivative of H(t)=c_0t^p-t-d log t is at least (c_0p/2)t^{p-1}. Thus, if s=log(c_AF T_r), the integral is at most

\[
 {2\over c_0p}s^{d+1-p}e^{s-c_0s^p}.
 \tag{RT.21}
\]

Here s=ell_r+O(1). The terms s, log s and O(ell_r^{p-1}) are absorbed by (c_0-c_1)ell_r^p. This proves (RT.19). Notice the factor e^t in (RT.20): it accounts for the number of scales and cannot be discarded. The strict assumption p>1 is what absorbs it.

### 5.1 Conditional monotone-radius variant: not a source premise

The constants in the comparison R_r~ell_r^p must not be used independently on opposite sides of a close exponent budget. The following mathematical variant would be available under the ADDITIONAL premise b<=r implies R_b>=R_r. The retained two-sided AF envelope does not establish that premise, and this variant is not used in the main proof. Section 6.2 gives a repair that needs no monotonicity of rounded radii.

**Lemma RT.2a.** Suppose R_b>=c_R(log T_b)^p with p>1, the radii have the just stated monotonicity, (RT.17) holds, and

\[
 f_b\le C g_b^{-v}(1+\ell_b)^d e^{-a_0R_b}.
 \tag{RT.21a}
\]

For every 0<a_1<a_0, uniformly in the cutoff depth,

\[
 F_r=\sum_{b\le r}f_b\le C_{a_1}e^{-a_1R_r}.
 \tag{RT.21b}
\]

**Proof.** If R_b<=s, then T_b<=exp[(s/c_R)^{1/p}]. Equation (RT.17) therefore bounds the number of possible b by C exp[C s^{1/p}]. The extra factor g_b^{-v}(1+ell_b)^d on the shell q<=R_b<q+1 is at most C(q+1)^{d/p} exp[C_v(q+1)^{1/p}]. By monotonicity only shells q>=floor(R_r) occur. Consequently

\[
 F_r\le C\sum_{q\ge\lfloor R_r\rfloor}
 (q+1)^{d/p}
 \exp[-a_0q+C'(q+1)^{1/p}].
 \tag{RT.21c}
\]

Choose a_2 strictly between a_1 and a_0. Since 1/p<1, the summand is at most C exp[-a_2q] for sufficiently large q. Its geometric tail is at most C exp[-a_1R_r]. This proves (RT.21b), including the scale-counting and inverse-coupling factors. No ratio C_R/c_R enters the surviving exponent a_1. The source radii are used as printed; no smooth replacement of their rounding is made.

## 6. The noncircular nonlinear bootstrap

The moving-normalizer correction is harmless numerically if it has the following proved recurrence:

\[
 A_r\le\exp\{C\sigma_r+C d_r A_{r-1}\}A_{r-1}+f_r,
 \qquad A_{r_0-1}=0.
 \tag{RT.22}
\]

Here sigma_r is the already paid new-map/count reserve; its sum is small at a sufficiently small common coupling ceiling. The d_r factor can contain a fixed inverse-coupling power, logarithmic powers, and the explicitly paid diameter/creation cost of a local nonlinear atom:

\[
 d_r\le Cg_r^{-u}(1+\ell_r)^D e^{\omega\ell_r^p},
 \qquad 0\le\omega<c_1<c_0.
 \tag{RT.22a}
\]

The positive rate used to read a physical root is selected so that its diameter cost satisfies this strict inequality. An exponential in the component diameter is not called a polynomial. The inverse-coupling and logarithmic factors are absorbed by an arbitrarily small further exponent loss. This statement explicitly does not allow a factor 1+Cg_r ell_r^D to be charged to every old atom at every scale. Such a factor is not AF summable.

**Lemma RT.3.** Define F_r as in (RT.19), and suppose the common ceiling is chosen so that

\[
 C\sum_r\sigma_r+2C\sum_r d_rF_{r-1}\le\log2.
 \tag{RT.23}
\]

Then

\[
 A_r\le2F_r\le2C_1e^{-c_1\ell_r^p}
 \tag{RT.24}
\]

at every scale in every finite history. In particular d_r A_{r-1}->0 uniformly as the common coupling ceiling tends to zero.

**Proof.** Assume (RT.24) through r-1 and unroll (RT.22). Every f_b is multiplied by the exponential of a sub-sum of the nonnegative quantities C sigma_j+C d_j A_{j-1}. The induction hypothesis and (RT.23) bound that exponential by 2, giving A_r<=2F_r. The initial zero capacity starts the induction. By Lemma RT.2 and (RT.22a), both the tail bound and sum_r d_rF_{r-1} are finite and tend to zero at a small common ceiling: a positive exponent c_1-omega remains, and the additional inverse-coupling power is exp[(u/2)ell_r], which it absorbs because p>1. Apply the same sum/integral calculation a second time; no depth-dependent constant occurs.

The proof first takes a finite history, obtains constants independent of its depth, and only then permits arbitrary depth. It does not assume the desired uniform conclusion in order to normalize its next prefix.

### 6.1 Conditional actual-radius version: not used in the application

If its additional monotonicity hypothesis were established, one could use Lemma RT.2a and replace (RT.22a) by

\[
 d_r\le Cg_r^{-u}(1+\ell_r)^D e^{\omega R_r},
 \qquad 0\le\omega<a_1<a_0.
 \tag{RT.24a}
\]

The identical induction proves A_r<=2F_r<=C exp[-a_1R_r], because

\[
 \sum_r d_rF_{r-1}
 \le C\sum_r g_r^{-u}(1+\ell_r)^D
                    e^{-(a_1-\omega)R_r}
\]

is uniformly small by the same shell count. In the application, omega includes BOTH the local cumulant's physical diameter/new-creation cost and the exponent of sigma_r^{-1} used to pay old-root component multiplicity. They are not omitted or described as logarithmic factors.

For example, start from a genuinely paid remote guard exp[-aR_r]. The two source extractions give the fresh exponent a/18 before a reserved creation payment. The count decrement can have exponent a/72. Choose the small positive spatial/footprint rates and the creation payment first, so that their total additional exponent is less than a/144. Then one can choose an incoming exponent strictly between a/48 and a/36, below the remaining fresh exponent and above a/72+a/144. Smaller positive reserves give a strict margin. All inequalities concern the SAME actual R_r. The choice is made before reducing the common coupling ceiling.

This paragraph is a conditional numerical variant. It is not an assertion that the printed coupling assumptions make R_r monotone.

### 6.2 Main reserve choice without rounded-radius monotonicity

The actual source gives c_R ell_r^p<=R_r<=C_R ell_r^p. From the fresh source creation bound, including its fixed inverse-coupling/logarithmic prefactors and a sufficiently small once-reserved creation payment, select c_0>0 so that (RT.18) holds. Choose 0<c_1<c_0 for the running tail in (RT.19). The choice of the small creation/footprint rate is made first so its exponential cost does not exhaust c_0.

Let sigma_r^source be the previously sufficient summable count decrement. Choose a fixed s_0 with 0<s_0<c_1/4 and use the larger auxiliary decrement

\[
 \widehat\sigma_r
 =\max\{\sigma_r^{\mathrm{source}},e^{-s_0\ell_r^p}\}.
 \tag{RT.24b}
\]

It is still summable, with arbitrarily small total at a common weak ceiling, by Lemma RT.2. Increasing this count decrement only strengthens the elementary bound N exp[-sigma N] and the old-count payment. The source primitive/forest inequalities required a lower bound on the available decrement. For their additional factor exp[4 hat-sigma |U|], impose 4 hat-sigma_r below the fixed unused primitive volume/count rate. Impose the total enlarged decrement below the initially reserved count rate as well. Both follow by reducing the common ceiling, so the same weighted source inequalities and positive rate floors remain valid. No source geometric radius, source operation, coupling recursion, or analytic domain has been altered.

Now

\[
 \widehat\sigma_r^{-1}\le e^{s_0\ell_r^p}.
 \tag{RT.24c}
\]

Choose the positive physical-root rate gamma and the small footprint/transport reserve d_* so that

\[
 C_R(C_{\rm diam}\gamma+d_*)<c_1/2.
 \tag{RT.24d}
\]

The full local nonlinear coefficient, INCLUDING old-root incidence and the true diameter cost, then satisfies (RT.22a) with

\[
 \omega=s_0+C_R(C_{\rm diam}\gamma+d_*)<3c_1/4<c_1.
 \tag{RT.24e}
\]

Lemma RT.3 closes the recurrence with sigma replaced by this larger hat-sigma. This is the choice used in the main proof. It works for every finite rounding ratio C_R/c_R and every trajectory satisfying the retained AF envelope; it assumes no sign for an individual beta coefficient and no monotonicity of rounded R_r.

## 7. What the running tail changes in the density proof

A fixed closed-ball estimate A<=A_* yields only d_r A_* for a component with d_r actual endpoint slots. That expression need not be small at arbitrary weak scales. Retaining the creation tail instead gives

\[
 d_r A_{r-1}\le C e^{(u/2)\ell_r}\ell_r^{D'}
          e^{-(c_1-\omega)\ell_r^p}=o(1).
 \tag{RT.25}
\]

Consequently (RT.2) can be imposed uniformly on the existing activity domain. The old completed relative action does not need to be continued to the independently enlarged ordinary-source domain. The ordinary kernel is estimated on its own source domain, and Lemma RT.1 incorporates the exact inherited action on the domain where it is actually controlled.

The dependence of the domination constant on the inherited action is 1+O(d_r A_{r-1}), which is summable over scales. Any constant ordinary-prefix integration cost must still use the original one-time integration capacities; this note does not authorize paying it repeatedly along a lineage.

For all subsequent native Cauchy estimates, use the full normalized quotient. They then automatically include every derivative of its normalizer. Cauchy estimates do not prove the prior spatial/rooted input (RT.13), and the two requirements must not be conflated.

## 8. Exact remaining source interface for a C05 application

The proposed simultaneous induction becomes a C05 proof only when all of the following are proved on the same admitted histories and the same coarsened catalog:

1. The ordinary stopped kernel has the common-positive-reference estimate (RT.1), with older raw variables fixed and selectors already relocated.
2. The literal archived raw masses are either retained as positive native-independent weights or have their genuine map response included. Their names do not make them constant.
3. The anchored incoming action obeys the actual proper-mesh endpoint estimate (RT.16), including native-only responses. This is the key numerical improvement over replacing the tail by A_*.
4. The newly exposed primitive records have the two-endpoint physical-root majorant required by (RT.13), as well as the component-root bound.
5. The coarsening/ownership construction yields (RT.22), with no repeated unsummable loss, and with the unchanged source canonical self kernels.

All components must satisfy the conditions above on the same admitted histories and coarsened catalog. Applying the resulting complete boundary estimate to the Wilson law still requires CR.
