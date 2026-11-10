# Actual regular action and admitted reference

**Current status:** This regular-sector identification remains in force. Parts I–III supply the additional current-link, magnetic, source/coarea, and regulator comparisons required for the regular mean metric. Mixed conditional boundaries remain outside its scope.

**Scope:** The intrinsic regular coefficient functions of the source construction, with their whole-lattice versions and compatible finite-volume localizations. Boundary terms remain in the boundary ledger. All running couplings, block averages, fluctuation maps, characteristic functions, and actual counterterm numbers are frozen throughout the comparison. The quantitative AF trajectory remains a standing premise; this module does not prove N2-F.

This module addresses the remaining identity A7.58. The reference constructed here performs pure regular fluctuation integrals, with the **actual frozen counterterms**. Its admission on a fixed complex domain is proved together with the smallness of the difference from the actual action. It is not assumed in advance, and it is not identified with the counterfactual model obtained by removing large-field operations and recomputing its coupling trajectory.

The proof uses the regular analytic estimates established in [Appendix F](observable_appendix_f.md) (A7), the full density version of the marked operator, and the actual unmarked source bounds for regular reset births. It distinguishes an exact equality on physical minimizing fields from the construction of a new compatible intrinsic analytic extension. Agreement on a thin physical section is not used as a uniqueness theorem for arbitrary preexisting extensions.

### 1. Source bookkeeping: what is absorbed and what is retained

Write the actual vacuum-subtracted regular potential as

\[
F_k=E_k+R_k.
\tag{A8.1}
\]

Here \(E_k\) is the fully renormalized regular expression in CMP119 (2.25), and \(R_k\) is the birth sum (2.30). The vacuum scalars are kept separately. Neither symbol denotes a boundary term.

The absorption described immediately before CMP119 (3.26) concerns the old-\(R\) **fluctuation expressions** in the exponent of the fluctuation integral. The terms \(R^{(j)}(U_{k+1})-R^{(j)}(1)\) already carried outside that integral remain in the classical birth sum. Denoting the fluctuation expression arising from old \(R\) by part of \(E\) therefore does not remove the old classical \(R\)-carriers.

This distinction gives an exact invariant ledger. Let \(\mathcal C_k\) denote classical restriction of an extensive action to the next minimizing field, with the current-unit density reassignment included. Define \(\Phi_k(H)\) as the logarithm of the complete frozen regular integral **relative to its leading Wilson factor at the step coupling \(g_k\)**, and then subtract its flat value. Thus, if \(\mathcal I_k^{\mathrm{phys}}(H)\) includes the leading input Wilson action,

\[
\Phi_k(H)=\mathcal V\!\left[\log\mathcal I_k^{\mathrm{phys}}(H)
+x_k\mathcal W_{k+1}\right],\qquad x_k=g_k^{-2}.
\tag{A8.2a}
\]

The frozen vacuum prefactors are tracked outside this relative potential. The later rewrite from \(g_k\) to the prescribed \(g_{k+1}\) is precisely the separate counterterm subtraction in (A8.5); it is not performed twice. In particular \(\Phi_k(0)\) contains no term of size \(x_k\mathcal W\). Define

\[
V_k=\Phi_k(0),\qquad
Q_k(H)=\Phi_k(H)-\mathcal C_kH-V_k.
\tag{A8.2}
\]

Apart from the extracted leading Wilson factor and vacuum scalar, the integral defining \(\Phi_k\) retains its Gaussian normalization, gauge-fixing factors, Jacobians, and the complete classical contribution \(\mathcal C_kH\) of the additional potential. Thus \(Q_k(0)=0\). The map is a map of local **action densities**: in current-unit density norms its classical part contains the four-dimensional block multiplicity. It is not an operation on one point root with that multiplicity omitted.

Let \(R_k^{\mathrm{old}}\) be the part absorbed into the regular fluctuation expression in the source's chosen split. The second interpolation term in (3.26), after removing its value at the flat field, is

\[
J_k=Q_k(E_k+R_k)-Q_k(E_k+R_k^{\mathrm{old}}).
\tag{A8.3}
\]

Its regular coefficients are the \(R''^{(k+1)}\) terms described on printed p.279; the remaining coefficients are assigned to the boundary term. The new regular birth is

\[
H_k^{\mathrm{reg}}=V_k+Q_k(E_k+R_k^{\mathrm{old}}).
\tag{A8.4}
\]

Let \(c_k\mathcal W_{k+1}\) be the actual coupling counterterm subtracted from this birth. The number \(c_k\) is fixed data in the present comparison. Let \(S_{k+1}\) be the new regular contribution of the subsequent reset operation, after vacuum subtraction. LFR II (1.98)–(1.101) identifies this contribution and gives its analytic birth estimate; coefficients touching the retained large-field region belong to the boundary ledger.

The source identities then give

\[
\begin{aligned}
E_{k+1}&=\mathcal C_kE_k+H_k^{\mathrm{reg}}-c_k\mathcal W_{k+1},\\
R_{k+1}&=\mathcal C_kR_k+J_k+S_{k+1},\\
F_{k+1}&=\Phi_k(F_k)-c_k\mathcal W_{k+1}+S_{k+1}.
\end{aligned}
\tag{A8.5}
\]

These equalities hold for the regular whole-lattice coefficient functions. In a carrier with boundaries, localization restricts their interior coefficients and assigns all remaining terms to the existing boundary ledger, exactly as in CMP119 (3.43)–(3.47). Equation (A8.5) is not an assertion that those boundary terms vanish.

The last line is independent of the old/recent split. Repeating an absorption changes the two intermediate ledgers, but leaves their sum unchanged. Consequently one does not need to invert the historical absorptions individually.

### 2. Matching the actual regular cutoff

The regular integral can be matched without replacing the cutoff by a source-dependent one. CMP119 (3.16) introduces the fluctuation-only characteristic functions. On the regular region, the preceding background-dependent characteristic factor equals one by (3.17)–(3.19); (3.20) identifies the resulting regular integration region. Thus its remaining cutoff is the fixed function of the fluctuation coordinates used in (3.25) and (3.28).

Use that **same function** in \(\Phi_k\) and in the reference below. Its fluctuation radius is a fixed multiple of the source polylogarithmic cutoff. It is even in the fluctuation variables and is independent of the inserted action parameter. No cutoff derivative is dropped from the comparison.

The fixed-domain analytic estimates do not require a different numerical cutoff radius. On the actual cutoff,

\[
\|B'\|\le Cg_kr_{\chi,k},\qquad
r_{\chi,k}\le C(\log x_k)^{p_0},\qquad x_k=g_k^{-2}.
\tag{A8.6}
\]

At a sufficiently weak fixed endpoint, this is smaller than the fixed complex margin in the source's small-field construction. The independent-current maps and the rooted localizations from A7 therefore apply. The source regular proof already treats characteristic functions of the fluctuation coordinates; its estimates require this smallness and Gaussian coercivity, rather than equality to one particular published cutoff constant.

If one instead compares with a reference using another cutoff, the corresponding normalized logarithmic difference must be retained. A local cutoff difference is supported in a Gaussian tail and is treated as a separate rare birth using the localized cutoff expansion, such as CMP119 (3.32). That optional comparison is unnecessary here. Background-dependent boundary cutoffs that survive outside the regular region remain in Gate 3.

### 3. The action space and the actual counterterm projection

Use the concrete intrinsic local families from A7, now with the local-potential norm

\[
\|H\|_{k,r,\kappa}^{\mathrm{pot}}
=\sup_{\Delta}\sum_{X\ni\Delta}
 e^{\kappa n_k(X)}\sup_{\mathscr D_k(X;r)}|H_X|.
\tag{A8.7}
\]

The potentials are vacuum-subtracted. Their scalar vacuum contributions are stored separately. The analytic domains use normalized relative connections and independent currents; the fine-link count never replaces a normalized potential norm. A fixed source reserve \(\kappa_{\mathrm{total}}\) pays the density reassignment, localizer extensions, support moments, and the marked norm exponent \(\kappa\), as in A7.27–A7.29a and A7.49a.

For the critical projection in this section use the **source's whole-lattice curvature functional**, denoted \(\Pi_\infty\). It is the quadratic constant-curvature coefficient per unit current volume. It acts on the full covariant density, after summing its localized terms, and has the matching embedding \(\iota_k\). Write \(P_k=\iota_k\Pi_\infty\).

The source Ward and Euclidean identities, CMP119 (3.49)–(3.67), identify the scalar invariant coefficient with the counterterm used in (2.24)–(2.25). With the matching normalization of \(\mathcal W_k\), they give

\[
\Pi_\infty\mathcal W_k=1,\qquad
\Pi_\infty\mathcal C_k H=\Pi_\infty H,\qquad
\mathcal C_k\iota_k=\iota_{k+1}+\mathcal R_{\mathrm{cl},k},\quad
\Pi_\infty\mathcal R_{\mathrm{cl},k}=0.
\tag{A8.8}
\]

Only the critical jet is reproduced exactly. The localized embedding can have the stable descendant \(\mathcal R_{\mathrm{cl},k}\), whose fixed-domain operator norm is bounded by a fixed \(C_{\mathrm{cl}}\). An exact identity of embedded functions is not required.

There are two projection realizations in this proof. For the translation-covariant reference \(B\), \(\Pi_\infty\) is its constant critical coefficient, reduced by the source symmetries to the scalar Wilson channel. Its complementary sector is the one used in (A8.16)–(A8.17).

For a general reset or difference density, retain the **entire 21-component coefficient profile** \(\mathbf\Pi_k H(z)\) over current density roots, with the supremum norm in \(z\). Its classical critical operation is the source block/hat average, of norm one. A zero spatial average of this profile does not make it stable. The propagator (A8.18) and the radius estimate (A8.24) use this full profile realization, exactly as in N7.45–N7.49. All stable estimates for an arbitrary profile refer to the kernel of this profile projection, not the kernel of its global average.

When applying \(\Pi_\infty\) to the difference identity involving \(R\) and \(\delta\), it means the bounded spatial average of their critical profiles. The actual regular reset grids have compatible power-of-\(L\) periods; on a finite compatible torus use its average, and on the whole lattice use the common period of the finite collection of birth grids. Averaging has norm at most one. The covariant density \(E_k\), and the constructed reference \(B_k\), have constant profiles.

Every birth in the **fully renormalized** regular density has its actual curvature coefficient subtracted. Classical restriction preserves that coefficient in four dimensions. Therefore

\[
\boxed{\Pi_\infty E_k=0.}
\tag{A8.9}
\]

This does not say \(\Pi H_X=0\) for each polymer. It does not apply to the temporary expression denoted by \(E_k+R_k^{\mathrm{old}}\) inside the fluctuation integral. Using either of those statements would invalidate the argument.

#### 3.1 Physical jet versus independent-current extension

The source definition of the counterterm is a physical minimizing-field derivative. In the intrinsic extension, the same coefficient is obtained by the affine connection test with independent \(J=0\). At the flat field the minimizing linear response reproduces an affine constant-curvature connection up to a linear gauge change; the physical current has no linear term on that affine test. The difference in the second-order field response contributes through the first differential of the activity, which vanishes by constant color invariance. Thus the quadratic coefficients agree. This is the local version of the source Ward calculation used to identify its counterterm.

There is no assertion that an arbitrary cutoff-affine test on a finite torus has zero physical current in its cutoff annulus. Nor is arbitrary off-section analytic uniqueness used. The exact identity (A8.9) is imposed on the source whole-lattice coefficient families and their physical curvature functional.

#### 3.2 Finite volumes

The coefficient construction has a compatible whole-lattice version. Nonwrapping interior coefficients agree with it by locality; CMP119, printed pp.278–279, states the interior-coefficient identification used in the regular construction. The finite-volume remainder consists of localized families with a support spanning the chosen periodic boundary or reaching the cutoff annulus. Keep these in an additional large-support sector rather than assigning them a fictitious zero physical jet.

This sector is controlled directly by its exponential support weight. If a step ends on a torus admitting the source root patch, an old wrapping support has at least a fixed multiple of the old torus diameter in block units. Its coarse cover has a smaller block footprint. The unused weight therefore pays the engineering factor:

\[
L^4e^{-\tau(n_k(X)-n_{k+1}(\overline X))}\le q_{\mathrm{wrap}}<1
\tag{A8.10}
\]

after the fixed source choices. A descendant retains the original protected support, so the same sector does not produce a new nonwrapping bulk coefficient. The ordinary localizer extension decay pays distant output roots as in A7.49a. These terms can be included in the stable norm used below. This avoids an inverse-mesh cost from a sawtooth direction and avoids multiplying an uncontrolled fixed-volume error by an inverse shrinking radius.

The argument does not apply an extra RG step after the finite torus has ceased to admit the source block geometry. It gives uniform bounds over the admitted finite volumes and ultraviolet cutoffs.

### 4. Source estimates used in the comparison

The following are the established regular analytic inputs, now stated in action-density form.

**Fixed-domain bare birth.** On one fixed domain of radius \(b\),

\[
\|(1-P_{k+1})V_k\|_{*,k+1}\le C_V.
\tag{A8.11}
\]

The bare integral contains the Gaussian determinant and the fixed Wilson/Jacobian remainder. Its local expansion is the source regular expansion with the old additional potential set to zero. The bound is uniform in the original mesh, scale, and admitted volume. Field-independent powers of \(g_k\) are vacuum scalars, not part of this norm.

**Uniform potential admission.** For every fixed bound \(R_B<\infty\), choose the endpoint sufficiently weak. Every invariant intrinsic potential \(B\) with fixed-domain norm at most \(2R_B\) then supplies an admitted frozen regular kernel on the enlarged fixed background domain. Indeed its fluctuation difference has local-potential norm at most
\(C g_kr_{\chi,k}\|B\|\), by the base-preserving pair map and whole-composition Cauchy estimate. This is the quantity that enters the source cluster-admissibility neighborhood. A fixed bound on the background potential itself need not tend to zero.

**Derivative and nonlinear remainder.** On a common admitted chart, differentiation of the actual finite-dimensional integral gives

\[
D\Phi_k(B)[H]
=\mathcal V\,\mathcal T_k^B H
=:\mathcal L_k^B H,
\tag{A8.12}
\]

where \(\mathcal V f=f-f(1,0)\). The density reassignment is included. The normalized denominator is present. The actual counterterm is outside \(\Phi_k\) and is not differentiated.

The rooted expansion, summed over density roots with its spatial reserve, gives

\[
\|D Q_k(B)[H]\|_{k+1,b,\kappa}^{\mathrm{pot}}
\le \epsilon_k\|H\|_{k,b,\kappa}^{\mathrm{pot}},
\qquad \epsilon_k\le Cg_kr_{\chi,k},
\tag{A8.13}
\]

uniformly for \(B\) in the fixed ball. This is the density version of A7.26. Summing the roots costs the current block factor already included in \(\mathcal L_k^B\), not an original-fine-mesh factor.

For an additional potential \(\delta\) on the current narrow chart, with small local norm, define

\[
\mathcal N_k(B,\delta)
=\Phi_k(B+\delta)-\Phi_k(B)-\mathcal L_k^B\delta.
\tag{A8.14}
\]

It is a new local analytic potential on the next narrow chart, and

\[
\|\mathcal N_k(B,\delta)\|_{k+1,\mathrm{narrow},\kappa}^{\mathrm{pot}}
\le C\|\delta\|_{k,\mathrm{narrow},\kappa}^{\mathrm{pot}\,2}.
\tag{A8.15}
\]

For precision, this follows from the source local-potential analytic neighborhood, not a global partition-function lower bound. Introduce \(z\delta\) into the frozen exponent. The connected local expansion is analytic for \(|z|\le c/\|\delta\|_{\mathrm{pot}}\). Coefficientwise Cauchy, with the same support reserve, bounds the sum of the terms of degree at least two by (A8.15). The classical part is linear and has canceled from (A8.14). The complex chart remains the narrow one; no continuation of \(\delta\) to the fixed radius is used.

#### 4.1 Classical and linear propagation estimates

For the covariant reference sector, the stable classical bound A7.36 can be turned into an equivalent one-step norm. The corresponding profilewise norm is used when the general-profile propagator is invoked later. Choose \(\omega\in(0,1)\) larger than its asymptotic classical contraction rate, and set, for the stable family,

\[
\|r\|_{*,k}
=\sup_{n\ge0}\omega^{-n}
 \|\mathcal C_{k+n-1}\cdots\mathcal C_k r\|_{k+n,b,\kappa}^{\mathrm{pot}}.
\tag{A8.16}
\]

For a finite horizon the supremum is truncated at its endpoint. A7.36 and the finitely many preceding steps give uniform equivalence to the original norm, and

\[
\|\mathcal C_k r\|_{*,k+1}\le\omega\|r\|_{*,k}.
\tag{A8.17}
\]

The support-tail sector in §3.2 is included in this stable norm. Add the bounded critical norm to obtain \(\|B\|_*\).

For a sequence of admitted fixed-domain kernels, Gate 2, N7.40–N7.49, gives the full action-density propagator bound

\[
\|\mathcal L_{k-1}^{B_{k-1}}\cdots\mathcal L_j^{B_j}\|
\le C\left(\frac{x_j}{x_k}\right)^{p_b}.
\tag{A8.18}
\]

It uses the \(O(g^2)\) critical and reverse blocks, stable contraction, and the AF scale bounds. It holds for arbitrary profiles, including the reset-grid profiles. It is not the still stronger common point-root normalization sought in Gate 2. The derivative estimate is uniform over the fixed potential ball: the flat-law cumulant proof uses the fixed-domain derivatives and the same unused source potential reserve.

### 5. Choose the actual shrinking radii

The source cutoff and source analytic radii can be made compatible explicitly. With \(p_0\) the fixed cutoff power in CMP119, choose the exponents in its (2.28), for example, with

\[
q_1=p_0+2,\qquad q_0=p_0+4,
\tag{A8.19}
\]

and choose the constants in the source hierarchy before fixing the weak endpoint. Take a fixed small multiple of the smaller allowed reference/relative/current radius:

\[
r_k=c_r g_k(\log x_k)^{q_1}.
\tag{A8.20}
\]

The larger real-reference and independent-current radius can contain this common inner ball. If the source convention requires additional fixed factors between its amplitudes, include them in \(c_r\). All logarithmic powers are fixed; the smallness conditions on the absolute source radii hold at a sufficiently weak endpoint because \(g(\log g^{-2})^q\to0\) for every fixed \(q\). The reset hierarchy also permits this choice: the analytic continuation estimate immediately before LFR II (1.73), printed p.379, bounds its additional exponent by \(g_k\) times a fixed product of powers of \(R_k\), \(p_1(g_k)\), and \(q_0(g_k)\). Increasing the fixed logarithmic exponents therefore still gives a vanishing error at weak coupling. It does not introduce a factor of the form \(\alpha_{1,k}^2/g_k^2\) that would reverse this conclusion.

Use the route's standing two-sided AF premise, with constants \(c_-,c_+>0\) such that

\[
c_-\le x_k-x_{k+1}\le c_+.
\tag{A8.21}
\]

Consequently, after increasing the weak endpoint \(x_*\),

\[
\frac{r_{k+1}}{r_k}\le2,\qquad
\frac{g_kr_{\chi,k}}{r_k}
\le C(\log x_k)^{-2},\qquad r_k\le b.
\tag{A8.22}
\]

Choose \(L\) so that there is \(\theta\) satisfying

\[
2<\theta L,\qquad c_{\mathrm{an}}\theta<1.
\tag{A8.23}
\]

These are fixed choices. A birth at radius \(r_j\) follows the ramp
\(r_{j,t+1}=\min\{b,\theta Lr_{j,t}\}\).
It contains the current narrow chart at every age. Its independent current has the additional old-unit factor \(L^{-3}\), so no cubed-radius convention is needed.

During its \(O(\log x_j)\) maturation interval, (A8.21) gives \(x_{j+t}\ge x_j/2\) for sufficiently weak coupling. Thus the birth fluctuation-to-radius estimate remains valid throughout the ramp. A7.41–A7.45 now yields a fixed exponent \(v\) such that a narrow birth at scale \(j\) can be propagated to any later scale with the estimate

\[
\|\mathcal L_{k-1}^{B_{k-1}}\cdots\mathcal L_j^{B_j}f\|
\le Cx_j^v
       \left(\frac{x_j}{x_k}\right)^{p_b}
       \|f\|_{j,r_j,\kappa}^{\mathrm{pot}}.
\tag{A8.24}
\]

Before maturation the fixed factor \((KL^4)^{k-j}\) is at most the full reserved maturation cost. After maturation apply (A8.18). Therefore (A8.24) does not assume the existence of a future kernel beyond a finite endpoint.

### 6. Actual rare inputs and the old regular \(R\) sum

LFR II (1.100) gives the new regular reset activity a factor \(e^{-p_0(g_k)}\) with ordinary tree decay. The comparison uses the activities produced by the actual operation, with their values frozen. Their possible dependence on earlier data is not differentiated. For any prescribed fixed \(Q\), the weak endpoint can be chosen so that

\[
\|S_{k+1}\|_{k+1,r_{k+1},\kappa}^{\mathrm{pot}}
\le C_Qx_{k+1}^{-Q}.
\tag{A8.25}
\]

The normalized domain and density conversion are those in A7.46–A7.52. In particular the source \(d_j\) is the fixed-\(M\)-block metric, not a metric assigning size one to an entire \(MR_j\)-cube. The birth-root multiplicity \(\lambda^{-4}\) is canceled by the vacuum-subtracted quadratic gain \(\lambda^4\). With the selectable \(\kappa_0\) in CMP119 (2.31), these estimates also give

\[
\|R_k\|_{k,r_k,\kappa}^{\mathrm{pot}}
\le C_Qx_k^{-Q}.
\tag{A8.26}
\]

These are estimates for the actual regular \(R\)-coefficients. Boundary coefficients and the masses of unresolved operations are not included in (A8.25) or (A8.26).

### 7. Define the reference without assuming its admission

On a fixed finite horizon, set \(B_0=0\), as appropriate to the vacuum-subtracted bare Wilson action, and recursively define

\[
\boxed{
B_{k+1}=\Phi_k(B_k)-c_k\mathcal W_{k+1}.
}
\tag{A8.27}
\]

This is a pure regular fluctuation recurrence, using the actual prescribed couplings, actual fluctuation cutoff, and actual counterterms. There is no fresh reset vertex in its integrand. It is a concrete nonautonomous reference, not an arbitrary admitted potential.

At each finite step, (A8.27) is defined as soon as \(B_k\) is in the admitted fixed ball. The proof below establishes this admission inductively. It is not assumed for the entire horizon.

Define the action difference on physical fields by

\[
\delta_k=F_k-B_k.
\tag{A8.28}
\]

Subtracting (A8.27) from the last line of (A8.5), with the same frozen \(c_k\), gives the exact recursion

\[
\boxed{
\delta_{k+1}
=\mathcal L_k^{B_k}\delta_k
 +\mathcal N_k(B_k,\delta_k)+S_{k+1}.
}
\tag{A8.29}
\]

No derivative of the coupling trajectory or of the counterterm occurs. The nonlinear term is defined on the narrow chart by (A8.14), with the bound (A8.15).

#### 7.1 Exact birth tags

Equation (A8.29) is also an explicit tagged representation. Every \(S_j\) receives its actual birth label. Every nonlinear remainder is expanded by the convergent local connected expansion in \(\delta\); its terms contain at least two previous difference factors. They can be assigned either their full ordered birth list or the step at which that connected term is formed. Propagate each resulting birth only by the pure linear operator \(\mathcal L^{B}\).

For finite horizons and cutoffs this is an exact algebraic identity. Absolute convergence follows from the local-potential neighborhood and the norm estimates below, so regrouping by birth or by the first occurrence of a reset vertex is permitted. Repeated absorption into the source's \(E\)-ledger cannot erase these tags: absorption has already disappeared from the total identity (A8.5).

The reference counterterm numbers are held fixed while tags are varied. Thus the tagged identity is not a counterfactual recalculation of the counterterms, and does not introduce an unrecorded response through them.

### 8. Uniform nonlinear difference bound

Let \(a_k\) denote the sum of the current norms of the concrete birth pieces representing \(\delta_k\), each on its own ramp domain. Because every such domain contains the current narrow chart,

\[
\|\delta_k\|_{k,\mathrm{narrow},\kappa}^{\mathrm{pot}}
\le a_k.
\tag{A8.30}
\]

If the reference is admitted through the preceding steps, (A8.15), (A8.24), and exact Duhamel expansion of (A8.29) imply

\[
a_k\le C\sum_{j<k}
 x_{j+1}^{v}
 \left(\frac{x_{j+1}}{x_k}\right)^{p_b}
 \bigl(a_j^2+C_Qx_{j+1}^{-Q}\bigr).
\tag{A8.31}
\]

The fixed adjacent-scale ratios are absorbed in \(C\). For any \(s>1\), (A8.21) gives
\(\sum_{j<k}x_j^{-s}\le C_sx_k^{1-s}\).
Consequently, under the inductive bound \(a_j\le D x_j^{-q}\),

\[
a_k\le C_1x_k^{1+v-Q}
      +C_2D^2x_k^{1+v-2q},
\tag{A8.32}
\]

provided \(Q-v-p_b>1\) and \(2q-v-p_b>1\).

Choose once

\[
q>v+p_b+3,\qquad
Q>q+v+p_b+3.
\tag{A8.33}
\]

Then choose a fixed \(D\) larger than the linear forcing constant and increase \(x_*\) until

\[
C_1x_*^{1+v-Q+q}\le D/4,\qquad
C_2D^2x_*^{1+v-q}\le D/4.
\tag{A8.34}
\]

The right side of (A8.32) is at most \((D/2)x_k^{-q}\), leaving strict slack. Also choose \(x_*\) so that \(Dx_*^{-q}\) lies inside the local-potential neighborhood required by (A8.15).

Thus the difference bound closes uniformly at any finite horizon:

\[
\boxed{a_k\le D x_k^{-q}.}
\tag{A8.35}
\]

The exponent can be chosen as large as a fixed application requires. Its size is paid by the source rare-birth estimate and the selectable source power, not by an age-dependent exponent. The radius cost is the one fixed power \(v\).

### 9. Simultaneously prove the reference is admitted

The only potential circularity is that the linear estimates used in §8 require admitted \(B_k\). Resolve it by a finite-horizon first-exit induction with strict margins.

The counterterm identity (A8.9), together with (A8.1) and (A8.28), gives

\[
\Pi_\infty B_k
=\Pi_\infty R_k-\Pi_\infty\delta_k.
\tag{A8.36}
\]

A curvature extraction on the radius-\(r_k\) chart costs two inverse radii, with a fixed polynomial support moment. The latter is paid by the spatial reserve. From (A8.20), (A8.26), and (A8.35),

\[
|\Pi_\infty B_k|
\le Cr_k^{-2}\bigl(C_Qx_k^{-Q}+Dx_k^{-q}\bigr)
\le C(D+C_Q)x_k^{1-q}.
\tag{A8.37}
\]

Choose the endpoint so that this is at most \(1/4\). This bounds the critical sector without assuming that the actual counterterms equal the canonical pure-theory counterterms.

For the stable sector apply \(1-P_{k+1}\) to (A8.27). The counterterm disappears, and (A8.8) retains a bounded stable descendant of the old critical coefficient. Equation (A8.2) gives

\[
\begin{aligned}
\|(1-P_{k+1})B_{k+1}\|_*
&\le\omega\|(1-P_k)B_k\|_*+C_V
 +C_{\mathrm{cl}}|\Pi_\infty B_k|
 +\epsilon_k\|B_k\|_*.
\end{aligned}
\tag{A8.38}
\]

Here (A8.13) was integrated along \(tB_k\), \(0\le t\le1\). Define

\[
R_s=\frac{4(C_V+C_{\mathrm{cl}}+1)}{1-\omega},\qquad R_B=R_s+1,
\tag{A8.39}
\]

and use the source admission neighborhood corresponding to \(2R_B\). Choose the endpoint so that
\(\epsilon_k\le(1-\omega)/8\).
If the old stable norm is at most \(R_s\) and the critical norm at most one, (A8.38) is strictly smaller than \(R_s\), by a fixed positive margin. The added \(C_{\mathrm{cl}}\) in (A8.39) pays the stable classical descendant. Equation (A8.37) gives the stronger next critical bound \(1/4\).

The induction order is important:

1. At step zero, \(B_0=\delta_0=0\); the source bare action supplies the base case.
2. Assuming the previous references are admitted, construct \(B_{k+1}\) from the admitted integral at \(B_k\). This does not yet use a kernel at \(B_{k+1}\).
3. Construct the narrow analytic extension of \(\delta_{k+1}\) by (A8.29). The estimates in §8 use only earlier admitted kernels and give their strict bound at \(k+1\).
4. The physical equality in (A8.28) follows from the source identity (A8.5). It identifies the physical curvature coefficient, so (A8.36)–(A8.37) bound the newly constructed reference's critical part.
5. The stable estimate (A8.38) bounds its remaining part. Thus \(B_{k+1}\) is admitted before the next integral is taken.

Every constant is chosen before the finite horizon. Increasing the horizon therefore does not change the bounds. This closes both the analytic admission and the nonlinear difference estimate; neither is used as an unproved global premise for the other.

### 10. The actual identification and its analytic meaning

Combining (A8.1), (A8.28), and the completed bootstrap gives

\[
\boxed{
E_k=B_k+\Delta E_k,\qquad
\Delta E_k:=\delta_k-R_k.
}
\tag{A8.40}
\]

On the physical minimizing section this is the **actual regular action**, with the actual counterterms and cutoff. The new intrinsic extension on the common narrow chart is defined by the right-hand side. It is local and gauge invariant because every map and localized coefficient used to construct it has those properties. Its bound is

\[
\|\Delta E_k\|_{k,r_k,\kappa}^{\mathrm{pot}}
\le C_qx_k^{-q},\qquad
\|B_k\|_{k,b,\kappa}^{\mathrm{pot}}\le R_B,
\tag{A8.41}
\]

after adjusting the freely chosen source exponents. This is the required replacement for A7.58. The fixed-domain bulk reference is the concrete recurrence (A8.27), and its admission has been proved, not postulated.

The action actually appearing in the next regular kernel is \(E_k+R_k=B_k+\delta_k\). Consequently its difference from the admitted fixed-domain reference has the narrow analytic norm (A8.35). A7.53–A7.57 and H7-A now apply with this **identified** difference. They no longer require an unidentified pure-versus-final-action correction.

The original independently chosen source extension of \(E_k\) away from physical minimizing fields need not equal the new extension. Such an equality is unnecessary. The new extension agrees with the physical action, has the intrinsic locality required by subsequent kernels, and preserves the source physical curvature coefficient. This is the extension used in the marked induction.

### 11. Vacuum scalars and history weights

All displayed action maps use the quotient by field-independent constants. For a finite carrier restore the scalar discarded by \(\mathcal V\) at each step:

\[
\zeta_{k+1}
=\zeta_k+
\left[\log\mathcal I_k(F_k)-\log\mathcal I_k(B_k)\right]_{(U,J)=(1,0)}
+\zeta_{k+1}^{\mathrm{reset}},
\tag{A8.42}
\]

with the source's prescribed vacuum-counterterm convention included in the last two terms. This equality is an exact scalar ledger; no uniform bound on an extensive global partition-function ratio is used in the local estimates.

For a fixed normalized regular conditional operator, the scalar cancels. If it depends on a carrier or a history, its factor remains in that carrier's contribution to the joint positive law. The comparison does not drop it from history probabilities or from conditional means. Those weights remain part of Gate 3.

### 12. A fixed-domain bound for the Gaussian cutoff score

This supplementary estimate is useful for the scalar one-loop normalization calculation in Gate 2. It concerns the actual frozen Gaussian cutoff and includes its normalization.

Let \(M(U,J)\) be the constrained Gaussian precision, with source current-coordinate dimension \(n\), and let \(D_p=pD_1\) be the even fluctuation domain. The fixed complex background domain is chosen so that the source covariance bounds and a uniform positive real-part bound persist. Put

\[
Z_p(M)=\int_{D_p}e^{-A^TM A/2}\,dA,\qquad
\mathcal B_p(M)=p\partial_p\log Z_p(M).
\tag{A8.43}
\]

For real positive precision, integration by parts in the actual domain gives

\[
\mathbb E_{p,M}[A^TM A]=n-\mathcal B_p(M).
\tag{A8.44}
\]

For a product of balls the score on the right is the sum of the normalized boundary integrals of \(A\cdot n\). For a smooth cutoff it is the corresponding integral with one differentiated cutoff. The identity is analytic in the admitted background and remains valid there by its convergent Gaussian cluster representation. It is not an uncut integration-by-parts identity applied to a truncated measure.

Write the normalized Gaussian cutoff contribution as
\(\log(Z_p/Z_\infty)\).
The Gaussian version of the source local expansion, used explicitly for CMP119 (3.32), expands this logarithm into connected local coefficients. Its derivative with respect to a local cutoff radius has at least one boundary factor. Such a factor is supported where a local fluctuation reaches size \(p\), and its Gaussian estimate has the form \(C p^m e^{-c p^2}\). Connecting derivatives and any fixed number of background derivatives add fixed polynomial moments; the covariance decay pays their connected spatial tree. The calculation is coefficientwise in the logarithmic expansion, so it does not estimate the inverse of an extensive partition function.

If a cutoff factor occupies an \(MR_k\)-cube, its finite-coordinate multiplicity and spatial weight can be bounded by a polynomial times \(\exp(C_\kappa R_k^4)\). Therefore the local density family of the score satisfies, on a fixed smaller background domain,

\[
\|\mathcal B_{p_k}\|_{\mathrm{pot},b,\kappa}
+\|\Pi_\infty\mathcal B_{p_k}\|
\le C p_k^m R_k^{m'}
       \exp[-c p_k^2+C_\kappa R_k^4].
\tag{A8.45}
\]

The source choices are \(p_k\asymp(\log x_k)^{p_0}\), \(R_k\asymp(\log x_k)^r\), with \(p_0\ge5r\); see the initial cutoff and partition choices in CMP119. Hence the exponent in (A8.45) is at most \(-c' p_k^2\) at a sufficiently weak endpoint, and, for every fixed \(Q\),

\[
\|\Pi_\infty\mathbb E_{p_k,M}[A^TM A]\|
=\|\Pi_\infty\mathcal B_{p_k}(M)\|
\le C_Q x_k^{-Q}.
\tag{A8.46}
\]

The constant \(n\) has zero curvature projection. Equation (A8.46) establishes rarity of this particular normalized Gaussian boundary score. A Wilson-source calculation must first identify its actual constrained source Hessian, including minimizing-field and normalization responses. When the Gaussian precision contains a gauge-fixing term, the projected identity below supplies the appropriate formula.

#### 12.1 A local linear boundary flux

The same argument applies to a uniformly local matrix insertion, which is useful when the Wilson Hessian differs from the full Gaussian precision by gauge fixing. Let \(P(U,J)\) be independent of the integration variable \(A\), holomorphic on the fixed background domain, and uniformly bounded in a local kernel norm with the required spatial reserve. A one-block finite-range matrix with uniformly bounded analytic coefficients satisfies this condition. For real backgrounds, the divergence theorem gives

\[
\mathbb E_{p,M}[A^T P^T M A]
=\operatorname{Tr}P-\mathcal B_{p,P},\qquad
\mathcal B_{p,P}
=Z_p(M)^{-1}\int_{\partial D_p}
     (PA)\cdot n\,e^{-A^TMA/2}\,d\sigma.
\tag{A8.47}
\]

The transpose is the ordinary transpose on the real fluctuation coordinates; its holomorphic continuation does not conjugate the background. For smooth cutoffs the boundary integral is the corresponding one-differentiated-cutoff expression. When \(P=I\), this is (A8.44).

Each localized flux coefficient has the same required boundary factor as in (A8.45), now multiplied by a bounded local linear function of \(A\). Its Gaussian moments cost a fixed additional power of \(p\) and a finite support enlargement. The local matrix norm of \(P\) and the reserved tree decay sum these enlargements. Background derivatives are controlled on a fixed smaller domain by Cauchy. Consequently

\[
\|\mathcal B_{p_k,P}\|_{\mathrm{pot},b,\kappa}
+\|\Pi_\infty\mathcal B_{p_k,P}\|
\le C_Pp_k^{m_P}R_k^{m'_P}
       e^{-cp_k^2+C_\kappa R_k^4}
\le C_{P,Q}x_k^{-Q}.
\tag{A8.48}
\]

The estimate remains coefficientwise in the connected Gaussian expansion; no inverse-volume or inverse-global-normalization estimate has been introduced.

For example, suppose a verified source gauge decomposition gives local analytic matrices \(K,T\), with \(TK=I\), a symmetric Wilson constrained Hessian \(M_W\) with \(M_WK=0\), and \(M=M_W+\kappa T^TT\). Then \(P=I-KT\) satisfies \(P^TM=M_W\) and \(\operatorname{Tr}P=n-n_g\), where \(n_g\) is the fixed gauge-coordinate dimension. Equations (A8.47)–(A8.48) imply

\[
\|\Pi_\infty\mathbb E_{p_k,M}[A^TM_WA]\|
=\|\Pi_\infty\mathcal B_{p_k,P}\|
\le C_Qx_k^{-Q}.
\tag{A8.49}
\]

Here the constant trace has zero curvature coefficient. The Gaussian boundary argument proves this consequence once the stated gauge factorization and its uniform locality are supplied; it does not equate the Wilson Hessian to the full precision when a gauge-fixing term is present.

### 13. Status and source anchors

The regular identification gap A7.58 is resolved by (A8.27)–(A8.41), on the intrinsic regular source geometry. The proof includes the actual density identity, a concrete frozen-counterterm reference, actual source radius choices, repeated-absorption tags, nonlinear feedback, and the simultaneous fixed-domain admission argument.

The scope does not extend this conclusion to a boundary activity outside the regular source domain. It does not prove common point-root normalization or a two-source separation estimate. It also does not replace the positive history-weight ledger by the vacuum-subtracted regular action.

Primary source anchors used in the identification:

- **CMP119 (1988), 243–285:** (2.23)–(2.31) for the actual regular action, counterterms, shrinking domains, and rare regular activities; (3.16)–(3.20) for the fluctuation-only regular cutoff; (3.25)–(3.28) for the exact normalized split and old/recent absorption; (3.43)–(3.47), printed pp.278–279, for interior coefficient matching and the regular/boundary ledger; (3.49)–(3.67) for the physical curvature functional and its counterterm identity.
- **LFR II, CMP122 (1989), 355–392:** (1.98)–(1.101), particularly (1.100), for the fresh regular reset birth and ordinary source-metric decay. The remaining boundary coefficients are explicitly excluded from that estimate.
- **CMP109 (1987), 249–301**, [DOI](https://doi.org/10.1007/BF01215223): (1.18) for absolute regular analytic domains and uniform local bounds; (1.20)–(1.22) for the curvature projection; (2.1)–(2.13) and the subsequent local analysis for the frozen regular integral. Its (0.11), (0.15)–(0.16), and (2.5) identify the residual contour gauge and the Gaussian gauge-fixing term relevant to §12.1. The theorem's own coupling recurrence is not silently substituted for the actual counterterms in (A8.27).
- **CMP116 (1988), 1–22**, [DOI](https://doi.org/10.1007/BF01239022): the local-potential analytic neighborhood and connected expansions used in the derivative and quadratic remainder bounds.
- **Mechanisms from Appendices F, G and H:** A7.13–A7.26 for the intrinsic pair and source return; A7.33–A7.36 for the classical stable estimate; A7.41–A7.52 for maturation and regular \(R\)-density conversion; N7.40–N7.49 for finite jets and arbitrary-profile mature propagation; H7-A for normalized local-potential interpolation.

The result is an analytic regular-sector comparison. It is not a claim that the complete four-dimensional Yang–Mills existence and mass-gap proof has been obtained.

---
