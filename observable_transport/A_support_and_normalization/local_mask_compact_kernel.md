# Exact compact regular kernels with local integration masks

## Result and scope

This note proves a local-mask extension of the compact-product theorem
CP.1. The mask selects integrated independent free coordinates from one
fixed pre-integration chart. All masks, including changes of integrated
rank, use one padded product probability space. The theorem retains the
actual exterior force and proves exact compatible direct and kernel
records. In particular, a change of the physical support is a kernel
current even if the padded reference probability is unchanged.

The large retained energy produced when a coordinate of size P is
activated or deactivated is not estimated by a small-interaction norm.
It is removed by an exact retained-only subtraction separately in each
normalized conditional. Its contribution to the outer history mass
remains present.

The action assumptions below are primitive gradient/coefficient
assumptions, independent of the mark and of the normalized output.
They are proved explicitly for a finite-range quadratic or analytic
primitive action. The actual current Gaussian and the already verified
full-carrier ordinary primitives fit the same calculation. A completed
inherited B activity with a component interior omitted from its
physical carrier is not supplied by this theorem.

This is an explicitly amended state interface: the integration mask is
a local primitive coordinate. It is not a proof for the specified
derived-domain footprint convention disproved by GO. The source
application is at fixed Ω in a common chart before the Λ-dependent
exterior relocation. Pullback to the old relocated retained filing and
changes of Ω are separate operations.

## 1. One fixed chart and all masks

Let J be a finite set of independent current free-coordinate blocks.
Their dimensions are bounded by a fixed d*, and at most n* of
these current blocks occur in one physical block, with n* fixed.
This is the one-step current layer, not the possibly extensive
list of inherited old coordinates; those remain in p.
Each coordinate and every
raw parameter has its actual physical footprint. For simplicity write
i for a coordinate with a fixed source-size footprint; replacing i by
that full footprint everywhere gives the same statements.

Fix source unit norm balls B_i and external radii

\[
 0<r_i\le r_*,\qquad r_*\le C gP,\qquad P\ge1 .
 \tag{MP.1}
\]

The first broad-cutoff convention r=P is not included in the
smallness conclusion below. The literal later cutoff of CMP119
(3.15)--(3.16) has the form (MP.1).

The retained state is \(\xi=(p,a,m)\), where p contains all other
retained raw and payload parameters, a_i is a padded possible exterior
value, and \(m_i\in\{0,1\}\) is an independent local integration mask.
It does not denote a derived rectangular hull flag. At actual source
states only the source-admitted masks occur; the normalized family
will be defined on every mask.

One may either restrict \(|a_i|\le AP\), with A fixed, or choose
once and for all a local smooth saturation \(A_i(a_i)\), identity
on that range, such that

\[
 |A_i(a_i)|\le C_A P,\qquad
 |A_i(a_i)|\le C_A|a_i|,\qquad
 \|D A_i\|\le C_A .
 \tag{MP.2}
\]

The latter gives an ambient extension on all Euclidean a. Write
\(\bar a_i=A_i(a_i)\); without an extension, \(\bar a_i=a_i\).
Set

\[
 \pi(du)=\bigotimes_{i\in J}
       |B_i|^{-1}{\bf1}_{B_i}(u_i)\,du_i ,
 \qquad
 c_{m,i}=(1-m_i)\bar a_i,\qquad
 \eta_{m,i}=m_i r_i u_i ,
\]

\[
 x_m(u)=c_m+\eta_m .
 \tag{MP.3}
\]

An inactive coordinate has the deterministic physical value \(\bar a_i\).
Its dummy u_i remains in π, but no observable is assigned a spurious
fluctuation or variance there.

Let \(\mathcal L(x;p)\) be the complete log density in the common
independent-coordinate chart, before selecting an integration subset.
It has no further m dependence. Let \(\chi(p,x)\) be the same
reconstruction used for every mark. Retained-only normalization factors
are denoted \(C_m(p,a)\ge0\), without any size assumption.
At active source data this factor is positive. At other data,
(MP.5)--(MP.6) specify the chosen positive extension; no
cancellation of a zero source factor is asserted.

The unnormalized source conditional is

\[
 C_m(p,a)
 \int_{\prod_{m_i=1}r_iB_i}
     e^{\mathcal L(x;p)}F(\chi(p,x))\prod_{m_i=1}dx_i ,
 \qquad x_i=\bar a_i\quad(m_i=0).
 \tag{MP.4}
\]

Every nonconstant Haar, coarea, old density or action factor belongs
to \(\mathcal L\); it is not placed in \(C_m\).

## 2. Exact baseline subtraction and rank normalization

Define

\[
 H_\xi(u)
   =\mathcal L(c_m+\eta_m;p)-\mathcal L(c_m;p),
 \qquad
 \nu_\xi(du)
   =\frac{e^{H_\xi(u)}\pi(du)}{\pi(e^{H_\xi})}.
 \tag{MP.5}
\]

The physical normalized kernel is

\[
 q_\xi=(u\mapsto\chi(p,x_m(u)))_*\nu_\xi .
 \tag{MP.6}
\]

Equations (MP.5)--(MP.6) are exact. Indeed the unnormalized denominator
in (MP.4) is

\[
 C_m(p,a)\,e^{\mathcal L(c_m;p)}
 \prod_{m_i=1}r_i^{d_i}|B_i|\;
 \pi(e^{H_\xi}) .
 \tag{MP.7}
\]

The first three factors cancel with precisely the same factors in
the numerator. They need not be small or comparable for two masks.
They remain in the source outer/history mass.

If no coordinate is integrated, \(H_\xi=0\) and q is the point
mass at the actual reconstructed retained field. This is a positive
kernel, with no zero-normalizer convention needed. Rank changes
require no comparison of Lebesgue measures of different dimensions.

There is also an exact outer-mass decomposition on active data:

\[
 \log Z_m^{\rm source}
 =\log C_m+\mathcal L(c_m;p)
   +\sum_i m_i(d_i\log r_i+\log|B_i|)
   +\log\pi(e^{H_\xi}).
 \tag{MP.7a}
\]

The last term has the small connected carrier expansion of CP.1,
with local-mask differences controlled by (MP.14) below. The
possibly large retained baseline retains the original primitive
carriers of \(\mathcal L\), and the product-volume term is an
explicit one-site mask term. Neither is declared a small
interaction. Any nonlocal dependence in \(C_m\) stays exposed.

For the actual quadratic density
\(\mathcal L_2=-x^*K(p)x/2\), symmetry gives

\[
 H_{2,\xi}
 =-\eta_m^*K(p)c_m-\tfrac12\eta_m^*K(p)\eta_m .
 \tag{MP.8}
\]

Thus the exterior force is exactly \(-K_{IO}\bar a_O\).
The omitted term \(-c_m^*Kc_m/2\) is retained-only and is
accounted for in (MP.7). A mask flip can change that term by
O(P²); no O(P²) interaction is introduced into (MP.8).

## 3. Primitive assumptions which imply small mask interactions

Suppose the common log density has actual connected coefficient
carriers

\[
 \mathcal L(x;p)
    =\sum_\alpha \ell_\alpha(x_{S_\alpha};p_{X_\alpha}),
 \qquad S_\alpha\subset X_\alpha .
 \tag{MP.9}
\]

The carrier includes every raw dependency and reconstruction
footprint. It is not the storage label of a nonlocal coefficient.
In the finite-range case (MP.9) is just the explicit local
stencil decomposition of the primitive action. No localization
of a normalized output is assumed.

On the common box \(|x_i|\le C_A P+r_*\), put

\[
 d_\alpha
   =\sum_{i\in S_\alpha}\sup\|\partial_{x_i}\ell_\alpha\|,
 \qquad
 e_\alpha
   =\sum_{i,j\in S_\alpha}
             \sup\|\partial_{x_i}\partial_{x_j}\ell_\alpha\|.
 \tag{MP.10}
\]

Let \(d_{\alpha,p}\) be the corresponding sum of actual normalized
raw-parameter finite differences of \(\nabla_x\ell_\alpha\),
divided by their parameter where required. Each direction carries
its full footprint. These may be real finite-difference bounds;
no old-payload complex tube is inferred.

For \(\nu_0>0\) and b>0 define

\[
 \begin{split}
 \epsilon_0&=
 \sup_y\sum_{\alpha:y\in X_\alpha}
 e^{\nu_0(|X_\alpha|+\mathsf t(X_\alpha))+b|X_\alpha|}
          r_*d_\alpha,\\
 \epsilon_a&=
 \sup_y\sum_{\alpha:y\in X_\alpha}
 e^{\nu_0(|X_\alpha|+\mathsf t(X_\alpha))+b|X_\alpha|}
          C_A r_*e_\alpha,\\
 \epsilon_p&=
 \sup_y\sum_{\alpha:y\in X_\alpha}
 e^{\nu_0(|X_\alpha|+\mathsf t(X_\alpha))+b|X_\alpha|}
          r_*d_{\alpha,p}.
 \end{split}
 \tag{MP.11}
\]

Only \(\epsilon_0\) must be below the fixed compact-product
convergence threshold. The other two quantities are exposed
current budgets.

For each primitive define, exactly,

\[
 h_{\alpha,\xi}(u)
 =\ell_\alpha(c_m+\eta_m;p)-\ell_\alpha(c_m;p).
 \tag{MP.12}
\]

The path \(c_m+t\eta_m\) stays in the same box. The fundamental
theorem of calculus gives

\[
 |h_{\alpha,\xi}|\le r_*d_\alpha ,
 \qquad
 h_{\alpha,\xi}=0
       \quad\hbox{if }m_i=0\hbox{ for all }i\in S_\alpha.
 \tag{MP.13}
\]

Every h has the same actual carrier X, now also containing the
local mask bits it reads. This is a constructive localization
identity.

If \(m^{(j)}\) flips one bit j, then

\[
 \Delta_j h_\alpha=0\quad(j\notin S_\alpha),
 \qquad
 |\Delta_j h_\alpha|\le2r_*d_\alpha,
 \qquad
 \sum_j|\Delta_j h_\alpha|
       \le2|S_\alpha|r_*d_\alpha .
 \tag{MP.14}
\]

There is no P² factor in this difference. Losing half the b
reserve pays \(|S_\alpha|\), so the summed mask-current
interaction budget is at most \(C_b\epsilon_0\).

For a retained endpoint, differentiation of the exact difference
gives

\[
 \nabla_{a_j}h_\alpha
 =(1-m_j)D A_j(a_j)^*
   [\partial_{x_j}\ell_\alpha(c_m+\eta_m;p)
        -\partial_{x_j}\ell_\alpha(c_m;p)] .
 \tag{MP.15}
\]

The summed bound is \(C_A r_*e_\alpha\).
Integrating (MP.15) along a unit finite-difference path proves
the same bound for actual divided differences, including through
the smooth saturation. Raw-parameter differences obey
\(|\delta_p h_\alpha|\le r_*d_{\alpha,p}\), since the
retained baseline is differentiated as well.

Thus (MP.11) proves value and all these density-current
budgets before any normalized kernel or mark is considered.

### Explicit quadratic and local analytic examples

For a true coefficient family \(K=\sum_\alpha K_\alpha(p)\)
with endpoints and raw footprints in X, set
\(k_\alpha=\sum_{i,j}\|(K_\alpha)_{ij}\|\).
Then

\[
 d_\alpha\le C P k_\alpha,\qquad
 e_\alpha\le Ck_\alpha,\qquad
 d_{\alpha,p}\le CP k_{\alpha,p}.
 \tag{MP.16}
\]

Consequently the value budget is \(O(r_*P)\), the exterior
endpoint-density current budget \(O(r_*)\), and the raw
coefficient-current budget \(O(r_*P)\) times its actual
coefficient budget. With \(r_*\le CgP\), these are
O(gP²), O(gP), and the exposed coefficient-current analogue.
No gap or small conditional Gaussian mean is needed for this
compact integral.

For a finite-range analytic primitive remainder with gradient
O(gP²) and Hessian O(gP), its contributions are
O(g²P³) and O(g²P²). Haar and exceptional-coordinate
logarithms with gradient O(g) give O(g²P).
Bounded stencil incidence proves the carrier sums directly.
These are actual derivative calculations on the common
primitive chart, not assumptions about a transported mark.

## 4. Normalized carrier theorem for every local mask

### Theorem MP.1

Assume (MP.9)--(MP.11), with \(\epsilon_0\) below the fixed
CP.1 threshold. Then uniformly in the total volume, every mask,
the rank of its integrated set, and all radii satisfying (MP.1):

1. The exact denominator \(\pi(e^{H_\xi})\) has the absolutely
   convergent connected product expansion of CP.1. It is nonzero
   on the corresponding coefficient polydisc.
2. A root whose common-chart pullback \(G_Z(p,x)\) has
   complete physical carrier Z and majorant M_Z on the
   common box has an exact normalized carrier representation
   for \(\nu_\xi[G_Z(p,x_m)]\). For a physical mark this
   is its corresponding contribution to \(q_\xi F\).
   At a smaller physical rate \(\nu>0\), the sum of absolute
   rooted values is bounded by

\[
 C w_\nu(Z)M_Z\exp(C\epsilon_0|Z|).
 \tag{MP.17}
\]

3. The sum over all elementary local mask replacements of the
   absolute kernel-current coefficients is bounded by

\[
 C w_\nu(Z)(1+|Z|)M_Z
       \exp(C\epsilon_0|Z|).
 \tag{MP.18}
\]

   It has a local embedding part present even at zero interaction,
   and a density part with the additional factor
   \(C_b\epsilon_0\). There is no inverse power of r, no inverse
   small-activity factor, and no division by a rare conditional
   mass.
4. Continuous endpoint and raw density currents have the same
   rooted bound with their exposed
   \(\epsilon_a+\epsilon_p\) budget. Changes of the physical
   reconstruction additionally require its actual root-current
   majorants; these are included as separate rooted insertions.
   Direct incoming records are transported separately.
5. Every resulting tagged value and its two records satisfy
   the exact M.10 compatibility identity, with the full carrier
   of the value and records assigned together.

Here an elementary mask coordinate can encode any subset of
the fixed finite number of modes at one physical block. Its
finite number of replacements only changes the fixed constant.
An arbitrary change on many blocks is the exact telescoping
sum of these local replacements; it is not declared a single
local direction.

**Proof of values and localization.** Equations (MP.12)--(MP.14)
give bounded true interactions on one product probability.
Apply CP.1 to these interactions. Their support contains the
mask and endpoint coordinates they actually use. The product
reference and all its dummy factors are independent of the
mask. Each rooted coefficient therefore depends only on its
displayed union carrier, even when the mask changes its
physical integrated rank. The initial factor \(w_\nu(Z)\)
is retained. Connected clusters disjoint from the root cancel
by the exact denominator, with no comparison of the outer
normalizers (MP.7). Use one common registry of primitive and
rooted cluster tags for every mask, including tags whose
activity happens to vanish. Mask changes do not reassign
the identity of a tag.

## 5. Exact physical currents: the embedding is part of J

For clarity use the full physical pushforward convention (MP.6),
which is allowed by the \(\chi_*q\) version of the specified
conditional rule. Put

\[
 \mathcal H(\xi_F,\xi_K)
  =\int F_{\xi_F}(\chi(p_K,x_{m_K}(u)))\,
                  \nu_{\xi_K}(du).
 \tag{MP.19}
\]

Any actual explicit incoming dependence is in the first copy;
the physical conditional, its support, and its reconstruction
are in the second. For an endpoint pair \(\xi,\xi'\), the
two records are exactly

\[
 B=\frac{\mathcal H(\xi',\xi')-\mathcal H(\xi,\xi')}{t},
 \qquad
 J=\frac{\mathcal H(\xi,\xi')-\mathcal H(\xi,\xi)}{t}.
 \tag{MP.20}
\]

For a discrete mask replacement omit t. Their sum is the
divided difference of the actual output. A bare physical
Wilson insertion independent of the first copy has B=0.

Write \(G=F_\xi\circ\chi_\xi\), \(G'=F_\xi\circ\chi_{\xi'}\)
as functions of the same padded u. The exact kernel record is

\[
 J=\nu_{\xi'}(G'-G)/t
       +(\nu_{\xi'}-\nu_\xi)(G)/t.
 \tag{MP.21}
\]

The first term is a kernel embedding record. It cannot be
renamed a direct insertion record merely because π is fixed.
For a mask flip j and a root of carrier Z it vanishes unless
j lies in Z, and its majorant is \(2M_Z\). Hence its sum
over j is at most \(C|Z|M_Z\). It is estimated by the
one-root CP expansion, giving its part of (MP.18).

For the density part set

\[
 H_s=(1-s)H_\xi+sH_{\xi'},\qquad
 \nu_s=e^{H_s}\pi/\pi(e^{H_s}),\quad 0\le s\le1.
\]

All primitive interactions on this real interpolation obey
the same small bound. Differentiating the same normalized
ratio gives the exact identity

\[
 (\nu_{\xi'}-\nu_\xi)(G)/t
   =\int_0^1
       \operatorname{Cov}_{\nu_s}
           \bigl(G,(H_{\xi'}-H_\xi)/t\bigr)\,ds .
 \tag{MP.22}
\]

The centering in this covariance is the denominator response;
it has not been omitted.

Expand (MP.22) by the same connected product series, with
one distinguished density-current vertex. Components not
joining that vertex to the root cancel exactly in the covariance.
For a mask flip j, (MP.14) places j in its distinguished
vertex carrier. Thus each nonzero current tag joins the
original root to the changed local mask.

Summing over j costs \(|S_\alpha|\) at that vertex and is
paid by the spare b reserve in (MP.11). The usual positive
rooted-tree induction then bounds the sum by

\[
 C w_\nu(Z)M_Z(1+|Z|)
    (C_b\epsilon_0)\exp(C\epsilon_0|Z|).
 \tag{MP.23}
\]

Replacing (MP.14) by (MP.15) or the raw coefficient
difference gives the continuous density-current statement.
All integrals are over a fixed real interval and the same
normalized product probability. No complex Gaussian mean,
different-rank density ratio, or total variation comparison
of singular physical measures is used.

Finally perform (MP.19)--(MP.20) on **each rooted cluster
tag**, keeping its common coefficients and full support.
It gives M.10 for that tag, not only after cancellation in
the summed output. Direct incoming records, embedding
kernel records, and density kernel records are kept
separately. This completes the proof of Theorem MP.1. ∎

## 6. Energy grades and what is needed for averaged M-03

On the product support,

\[
 \sum_{i\in Z}|x_{m,i}(u)|^2
 \le C\sum_{i\in Z}|a_i|^2+C|Z|r_*^2 .
 \tag{MP.24}
\]

The same bound holds for both masks in a local difference.
If the incoming physical root has a genuine envelope

\[
 |G_Z|\le b_Zh^{-4}(1+|Z|)^q
        [R_Z(p,a)+|Z|r_*^2],
 \tag{MP.25}
\]

then r*≤1 at a sufficiently small fixed coupling ceiling
gives a grade-one root majorant
\(Cb_Zh^{-4}(1+|Z|)^{q+1}R_Z\).
The mask embedding record is bounded by the sum of the
two endpoint envelopes. Since the common shifted regulator
is at least one, it also has the required grade 3/2.
No factor P² must be appended to that regulator bound.

For the quadratic action one can additionally keep the
pointwise half-grade density bound. Every term in (MP.8),
and in its one-bit difference, contains at most one
retained value and at least one active factor of size r*.
Thus its density-current coefficient is bounded by

\[
 C r_* k_\alpha
   \left(1+\sum_{i\in X_\alpha}|a_i|^2\right)^{1/2},
 \tag{MP.26}
\]

up to a fixed endpoint-count polynomial. When a raw
parameter changes K, replace \(k_\alpha\) by its actual
coefficient-current majorant in this formula. This yields the
natural root grade \(1+\tfrac12\). Uniform suprema
O(r*P) still provide convergence of the unmarked series.

Spatial slack pays the explicit powers of |Z| in
(MP.17)--(MP.25). Averaged M-03 costs still require the
actual outer moment reserve, or a separately proved
disintegration estimate for the localized coefficients.
The pointwise proof here does not declare such an outer
moment estimate. Likewise it does not improve the
microscopic factor a⁻⁴ to a current factor h⁻⁴.

## 7. Actual regular-source application and its boundary

### 7.1 The common pre-Λ primitive

At a fixed source Ω and fixed coarse/mixed determining data,
the background U, the exceptional embedding C, and the
nonlinear constraint solve are fixed before the current R
split selects Λ. The independent coordinate index set J
is therefore common. The complete log density before the
Λ-dependent relocation can be written as

\[
 \mathcal L_k(x;p)=
 -\tfrac12x^*K_k(p)x+
 W_{\rm classical}(x;p)+W_{\rm measure}(x;p)
 +W_E(x;p)+W_R(x;p)+W_B(x;p).
 \tag{MP.27}
\]

This is the complete C01/C07 identity, with every
background-dependent older density ratio retained in W_B.
For an admitted source mask, bad selectors and the remaining
boundary selectors have their whole footprints in the retained
region. The integrated good cutoff is exactly the product
appearing in (MP.4). Retained-only selector values and source
coarea constants are part of its exterior factor, not
discarded from the joint source law.

The actual Gaussian part has the force (MP.8), even next to
the retained exterior. Its coefficient family is the
primitive source operator family with the common raw
reconstruction, not a covariance inferred just from a
spectral gap. The current primitive operator families
already constructed in GR/CP give (MP.16) with their full
raw footprints. The fixed-range Wilson, soft-gauge, Haar,
and exceptional-coordinate terms give the local derivative
bounds described after (MP.16).

For full-tree ordinary E/R/B families, the already verified
common native tube and actual raw component construction
of BQ/GR supply (MP.9)--(MP.11). Mask substitution and
baseline subtraction introduce no new nonlocal map.
Old endpoint currents can be included only when their
actual real current bounds have been proved; a native
(U,J) analytic domain does not supply them.

In particular, the common-chart Gaussian plus primitive
Wilson/measure kernel is a fully proved concrete subcase
with arbitrary local mask changes. Adding the verified
full-tree ordinary factors obeying (MP.11) preserves the
theorem without any new normalization estimate.
A clean prehistory with no surviving older slots or
completed R components removes the completed-B and
old-payload gates; its inherited bulk E/R bounds retain
their previously stated source-domain dependencies.

### 7.2 What is not silently imported

There are three distinct further applications.

* A completed inherited B operation whose source bound
  omits a whole component interior does not automatically
  satisfy (MP.9)--(MP.11) in full physical carriers.
  Multiplying its value by g does not prove that support
  estimate. Its complete coefficients remain an open input.
* The source relocation after Λ selection changes the
  retained filing by a Λ-dependent map. In the common
  pre-relocation coordinates this map is not needed for
  the exact conditional (MP.4). To return to the relocated
  filing, its full mask/current and raw support costs
  must be proved. They are not absorbed into a supposedly
  common K or into a retained constant.
* This note fixes Ω and its determining chart. It does
  not assign local primitive footprints to the source's
  other derived P/Q domains, replace their hard geometry
  tests, or prove arbitrary old-history current estimates.

The independent local-mask amendment is therefore explicit,
and the result is a genuine normalized integration/rank
theorem for that interface. It repairs the mask-current
part of the narrow compact model; it does not prove
the original M-04 statement.

## Sources and companion proofs

* CMP119 pp.247--253, (1.9), (1.14)--(1.26): one common
  exceptional chart before Λ integration; exact later
  retained relocation.
* CMP119 pp.267--268, (3.15)--(3.16): literal later
  scaled free coordinate and shrinking integration radius.
* C01/C07 and the C05 old-density statement: complete density,
  actual coarea, and retention of old Gaussian responses.
* CP.1: exact compact-product connected/rooted expansion.
* GR and BQ: actual primitive raw reference/component
  families and ordinary full-tree current interactions.
* Annex Y (M.10), (M.30) and its physical pushforward
  option: separately compatible direct/kernel records.
