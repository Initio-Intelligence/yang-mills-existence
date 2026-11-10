# Direct boundary score and Hessian tests

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

## 1. Results and precise status

This note establishes five results without assuming C05, C06, an interacting spectral gap, or an identity between covariance and an inverse Hessian.

1. It gives the exact first and second derivatives of the actual fixed-support partial integral and of its normalized insertion. The formulas retain the moving denominator, every old mass that remains inside a later integration, and the covariance of the complete score.
2. It proves a positive-law derivative estimate using oscillations of the actual logarithmic density. It extends to weakly coupled components by a proved heat-bath comparison estimate. No differentiability in an integrated old raw variable is required.
3. It verifies the direct logarithmic-density response of the pure constrained Gaussian/Schur/coarea part of an eligible stopped prefix, using the actual old cutoffs and native coordinate counts. Arbitrary positive factors depending only on the fixed raw coordinates may be included in its reference measure. Such factors change the expectation; they do not create an explicit current score.
4. It proves the exact nonlinear normalized-integration estimate needed by the proposed running-tail induction: after the transported linear part is retained, the remaining logarithm is quadratic in the incoming relative interaction. The quadratic term is the moving-normalizer covariance, explicitly paid. An AF-summable quadratic recurrence closes with a uniform superlogarithmic tail.
5. It proves the derivative readout from a complete projective density bound on the actual analytic chart. This yields the C06/C08 first-current and weighted second-current inputs once the genuine root-localization load has been established.

The complete all-history C05 conclusion is not asserted by these statements alone. The outstanding source matching is the incident sum of **all** archived relative activities in a literal stopped prefix, including native-only remote responses and any raw argument that really moves. The companion density and root calculations address this matching. An old label saying that C05 is complete is not used as a premise here.

The argument below is stronger than merely observing that a covariance term is missing: it identifies a route which can pay that term without C05, and proves the nonlinear estimate which makes the running-tail bootstrap noncircular.

## 2. Fixed support and the literal density

Let \(z=(z_i)_{i\in I}\) denote the current free coordinates. Fix all earlier retained raw coordinates \(x\), the geometry, and the selector/history branch. Let \(a\in\mathcal A_x\) be precisely the old free coordinates actually integrated by the partial operation. After the source's actual exceptional-coordinate elimination and failed-selector relocation, write its density as

\[
 T_zF=\int_{\mathcal A_x}p(z,a;x)F(z,a;x)\,dm_x(a),
 \qquad \tau(z)=T_z1,\qquad \Pi_zF=\frac{T_zF}{\tau(z)}.
 \tag{DB.1}
\]

The measure \(m_x\), including fixed selectors, is independent of \(z\). On its positive support the complete logarithmic density is \(L(z,a)=\log p(z,a;x)\). A common positive raw factor may instead be placed in \(m_x\); this is an exact change of notation, not deletion of that factor. Assume the differentiations below are justified by common-support domination. The finite-cutoff analytic source chart supplies this for its actual smooth native factors; no raw differentiability is assumed for an arbitrary bounded test \(F\).

The fixed-support assertion is the one in LFR I (1.25), (1.29), (1.55), (1.59), (1.60), printed pp.182, 187–189. The free coordinates are the independent coordinates after solving the linear averaging constraints, CMP119 p.249. In particular, varying a native parameter does not mean putting an arbitrary old raw test function at a complex value of its raw argument.

If a proposed coordinate change moves an old raw argument, its response must be retained. The safe formula is \(M(\Phi_z(a,x))\), not (M(a,x)). No arbitrary raw analyticity follows from native analyticity. A genuinely moving support also requires its actual transport and Jacobian before (DB.1) can be used.

### 2.1 Ordered masses stay at their actual locations

For an earlier kernel \(K_z(u,da)\), write

\[
 K_z(u,da)=\tau_z(u)\Pi_z(u,da).
 \tag{DB.2}
\]

If \(u\) is integrated later, the later density contains the factor \(\tau_z(u)\). It is not a scalar that can be moved outside that integration. For two successive integrations,

\[
 \int r_z(u)\int k_z(u,a)F(u,a)\,da\,du
 =\int r_z(u)\tau_z(u)\Pi_{z,u}F\,du.
 \tag{DB.3}
\]

The correct outer normalized law is proportional to \(r_z(u)\tau_z(u)\). Replacing it by the independently normalized law proportional only to \(r_z(u)\) changes the answer.

This also identifies the outer score:

\[
 \partial_i\log\{r_z(u)\tau_z(u)\}
 =\partial_i\log r_z(u)+\Pi_{z,u}(\partial_i\log k_z).
 \tag{DB.4}
\]

Its second derivative contains the conditional score covariance below. Thus normalization cannot remove a response just by changing the order in which the same integral is written.

## 3. Exact derivative identities

All covariances are bilinear covariances under the displayed law. On the real slice these are ordinary positive-probability covariances. Complex versions use the same algebra with the normalized complex functional.

Set \(S_i=L_i\) and \(T_{ij}=L_{ij}\). Direct quotient differentiation gives

\[
 \partial_i\Pi F=\Pi F_i+\operatorname{Cov}_{\Pi}(F,S_i),
 \tag{DB.5}
\]

\[
 \begin{split}
 \partial_i\partial_j\Pi F={}&\Pi F_{ij}
 +\operatorname{Cov}_{\Pi}(F_i,S_j)
 +\operatorname{Cov}_{\Pi}(F_j,S_i)\\
 &+\operatorname{Cov}_{\Pi}(F,T_{ij})
 +\kappa_{3,\Pi}(F,S_i,S_j).
 \end{split}
 \tag{DB.6}
\]

Here \(\kappa_3(X,Y,Z)=\Pi[(X-\Pi X)(Y-\Pi Y)(Z-\Pi Z)]\). Every term is required. In particular, a first-derivative estimate for \(F\) alone is not an estimate for the derivative of \(\Pi F\).

For the mass,

\[
 \partial_i\log\tau=\Pi S_i,
 \qquad
 \partial_i\partial_j\log\tau
 =\Pi T_{ij}+\operatorname{Cov}_{\Pi}(S_i,S_j).
 \tag{DB.7}
\]

The normalized logarithmic score is \(S_i-\Pi S_i\). Its appearance is exactly the denominator response. Formula (DB.7) applies to an arbitrary positive finite-dimensional density; neither Gaussianity nor convexity is involved.

### 3.1 A literal interaction relative to a moving reference

Let \(p_t=p_0e^{tV}\), let \(\Pi_t\) normalize this same density on the same support, and define

\[
 B(z)=\log\int p_0(z,a)e^{V(z,a)}\,dm
       -\log\int p_0(z,a)\,dm.
 \tag{DB.8}
\]

Write \(S_i=(\log p_0)_i\), \(T_{ij}=(\log p_0)_{ij}\). Then

\[
 B_i=\Pi_1V_i+(\Pi_1-\Pi_0)S_i,
 \tag{DB.9}
\]

\[
 \begin{split}
 B_{ij}={}&\Pi_1V_{ij}+(\Pi_1-\Pi_0)T_{ij}\\
 &+\operatorname{Cov}_{\Pi_1}(S_i+V_i,S_j+V_j)
  -\operatorname{Cov}_{\Pi_0}(S_i,S_j).
 \end{split}
 \tag{DB.10}
\]

The common reference can have order-one or larger scores. Their two covariances cannot be bounded separately and then called a small interaction response without paying the resulting reference-size term.

There is a useful exact interpolation which keeps the small interaction factor explicit. Put \(S_i(t)=S_i+tV_i\), \(T_{ij}(t)=T_{ij}+tV_{ij}\). Then

\[
 B_i=\int_0^1\left\{\Pi_tV_i+
              \operatorname{Cov}_{\Pi_t}(V,S_i(t))\right\}dt,
 \tag{DB.11}
\]

\[
 \begin{split}
 B_{ij}=\int_0^1\{&\Pi_tV_{ij}
 +\operatorname{Cov}_{\Pi_t}(V,T_{ij}(t))\\
 &+\operatorname{Cov}_{\Pi_t}(V_i,S_j(t))
 +\operatorname{Cov}_{\Pi_t}(V_j,S_i(t))\\
 &+\kappa_{3,\Pi_t}(V,S_i(t),S_j(t))\}\,dt.
 \end{split}
 \tag{DB.12}
\]

Proof: differentiate \(\log Z_t\) in \(z\) and then in \(t\); use \(\partial_t\Pi_tF=\Pi_t\partial_tF+\operatorname{Cov}_{\Pi_t}(F,V)\). The derivative of a covariance is its two differentiated arguments plus the third cumulant. Integrating in \(t\) proves the result. This proof never inserts an independently normalized comparison law.

### 3.2 Schur differentiation is a coefficient calculation

Let the actual constrained precision be

\[
 K=\begin{pmatrix}A&B\\B^{\mathsf T}&C\end{pmatrix},
 \quad G=A^{-1},\quad S=C-B^{\mathsf T}GB,
 \quad E=\binom{-GB}{I}.
 \tag{DB.13}
\]

The constrained background-current term is part of \(K\). For fixed retained \(a\), \(KEa=(0,Sa)\), and

\[
 S_i=E^{\mathsf T}K_iE.
 \tag{DB.14}
\]

In this subsection only, \(S_i\) denotes the derivative of the Schur matrix. Put \(R_i=(K_iE)_I\). Since \(E_i=(-GR_i,0)^{\mathsf T}\),

\[
 S_{ij}=E^{\mathsf T}K_{ij}E
      -R_i^{\mathsf T}GR_j-R_j^{\mathsf T}GR_i.
 \tag{DB.15}
\]

Consequently the retained exponent \(q=-a^{\mathsf T}Sa/2\) satisfies

\[
 q_i=-\tfrac12(Ea)^{\mathsf T}K_i(Ea),
 \quad
 q_{ij}=-\tfrac12(Ea)^{\mathsf T}K_{ij}(Ea)
          +(R_i a)^{\mathsf T}G(R_j a).
 \tag{DB.16}
\]

The final term is indispensable. The Gaussian determinant, wherever the source assigns it, has

\[
 (\log\det A)_i=\operatorname{Tr}(GA_i),\qquad
 (\log\det A)_{ij}
 =\operatorname{Tr}(GA_{ij}-GA_jGA_i).
 \tag{DB.17}
\]

These are exact coefficient identities, not formulas for interacting covariance. Moreover, integrating over a cutoff set gives the full Gaussian Schur expression **times its actual truncated-Gaussian probability**. If the cutoff is present, the derivatives of that probability remain unless the source has already assigned and estimated them elsewhere. The covariance of a truncated Gaussian is not in general \(A^{-1}\).

## 4. Positivity pays the covariance without a spectral theorem

For a real random vector \(X\), define a deterministic centered radius \(q_X\) by choosing any constant vector \(c_X\) and requiring \(\|X-c_X\|\le q_X\) pointwise. Then, for unit test vectors (u,v),

\[
 \operatorname{Var}(u\cdot X)\le q_X^2,
 \qquad
 |\operatorname{Cov}(u\cdot X,v\cdot Y)|\le q_Xq_Y.
 \tag{DB.18}
\]

The first inequality follows by subtracting the mean from a square about \(c_X\); the second is Cauchy–Schwarz. For a scalar, one may use half its oscillation as \(q_X\).

Suppose \(L=c(z)+\widetilde L(z,a)\), with

\[
 |\widetilde L_i|\le d_i,\qquad
 \|\widetilde L_{ij}\|\le h_{ij},\qquad
 \|\widetilde L_i-c_i^*\|\le q_i
 \tag{DB.19}
\]

for constants \(c_i^*\) that may depend on \(z\), but not on \(a\). For \(F=\log\tau-c\), (DB.7) and (DB.18) give

\[
 \|F_i\|\le d_i,\qquad
 \|F_{ij}\|\le h_{ij}+q_iq_j.
 \tag{DB.20}
\]

Therefore a sufficient physical weighted second-current estimate is

\[
 \sup_i\sum_j e^{\gamma\rho(i,j)}h_{ij}\le H P^{-2},
 \qquad
 \sup_i q_i\sum_j e^{\gamma\rho(i,j)}q_j\le Q P^{-2}.
 \tag{DB.21}
\]

The result is \(\|F''\|_\gamma\le(H+Q)P^{-2}\). The actual scalar \(c(z)\) is estimated separately; it cannot be deleted from the unsubtracted native theorem.

For (DB.12), suppose on every interpolating positive law that the centered radii of \(V,S_i(t),T_{ij}(t),V_i\) are respectively bounded by \(v,q_i,h_{ij},r_i\), and \(\|V_i\|\le d_i\), \(\|V_{ij}\|\le e_{ij}\). Since

\[
 |\kappa_3(V,X,Y)|
 \le 2v\sqrt{\operatorname{Var}(X)\operatorname{Var}(Y)},
 \tag{DB.22}
\]

the exact relative response satisfies

\[
 \|B_i\|\le d_i+vq_i,
 \qquad
 \|B_{ij}\|\le e_{ij}+vh_{ij}+r_iq_j+q_ir_j+2vq_iq_j.
 \tag{DB.23}
\]

This estimate retains a factor from the relative interaction in each response term. It needs no regularity in \(a\). A total oscillation \(v\) that grows with the number of components is not a uniform estimate; in that situation use the component comparison below or a proved connected expansion.

## 5. Coupled components: a complete heat-bath proof

This section supplies a real alternative to complex cluster expansion for first and second derivatives. It allows arbitrary positive internal component laws, including nonsmooth old tests and large internal masses.

Let \(\mathcal V\) be a finite component set and

\[
 d\nu(a)=Z^{-1}\prod_{v\in\mathcal V}d\mu_v(a_v)
      \exp\Bigl\{\sum_e V_e(a_{I_e})\Bigr\}.
 \tag{DB.24}
\]

All common external current/native parameters are fixed here. Interactions spanning two components stay in the displayed exponential. The reference factors may share fixed external parameters; they may not depend on another component's integrated coordinate.

For a bounded scalar \(f\), let \(\delta_vf\) be its oscillation when only \(a_v\) changes. Let \(P_v\) be the conditional expectation over \(a_v\). Define the influence matrix

\[
 C_{vu}=\sup_{a,b:\ a_w=b_w\ (w\ne u)}
    \|\nu_v(\cdot\mid a_{-v})-\nu_v(\cdot\mid b_{-v})\|_{\rm TV},
 \quad C_{vv}=0,
 \tag{DB.25}
\]

where total variation has the convention \(\sup_A|\mu(A)-\nu(A)|\).

### Theorem DB.1

If \(\sup_v\sum_uC_{vu}<1\), then for bounded real functions

\[
 |\operatorname{Cov}_\nu(f,g)|
 \le\frac14\sum_{u,v}(\delta_uf)
       [(I-C)^{-1}]_{uv}(\delta_vg).
 \tag{DB.26}
\]

**Proof.** For \(u\ne v\), comparison of two conditional integrals gives

\[
 \delta_u(P_vf)\le\delta_uf+C_{vu}\delta_vf,
 \qquad \delta_v(P_vf)=0.
 \tag{DB.27}
\]

The bounded generator \(\mathcal L=\sum_v(P_v-I)\) defines the continuous-time random-scan heat-bath semigroup \(P_t\). Each \(P_v\) is self-adjoint in \(L^2(\nu)\). The positive semigroup comparison obtained by iterating (DB.27) is

\[
 \delta(P_tf)\le e^{-t(I-C^{\mathsf T})}\delta(f)
 \tag{DB.28}
\]

componentwise. It can be proved first for a product of the individual Poisson update semigroups, then by the finite-dimensional Trotter product formula. Equivalently, the upper Dini derivatives of the oscillations satisfy the corresponding linear cooperative differential inequality. Since the row norm of \(C\) is less than one, the sum of these oscillations decays exponentially. Thus \(P_tf\to\nu f\) uniformly for bounded \(f\) of finite coordinate oscillation.

Reversibility and conditional expectation give

\[
 -\langle\mathcal L h,g\rangle_\nu
 =\sum_v\nu\bigl[\operatorname{Cov}_{\nu_v(\cdot\mid a_{-v})}(h,g)\bigr].
 \tag{DB.29}
\]

Integrate the derivative of \(\nu[(P_tf)g]\) from zero to infinity. Conditional covariance is at most \(\delta_v(P_tf)\delta_vg/4\), by the scalar version of (DB.18). Hence

\[
 |\operatorname{Cov}_\nu(f,g)|
 \le\frac14\int_0^\infty
       \delta(f)^{\mathsf T}e^{-t(I-C)}\delta(g)\,dt,
 \tag{DB.30}
\]

which is (DB.26). No differential operator in an internal variable, and no internal convexity, has been used. Truncation extends the inequality whenever its displayed right side remains finite. \(\square\)

### 5.1 A direct sufficient influence bound

If two conditional densities differ by a log tilt \(\Delta\) whose oscillation is \(r\), their total variation is at most \(\tanh(r/4)\). For completeness, put \(X=e^\Delta\in[a,b]\). Convexity of \(x\mapsto|x-m|\) gives

\[
 \frac{\mathbb E|X-m|}{2m}
 \le\frac{(b-m)(m-a)}{m(b-a)},\qquad m=\mathbb EX.
\]

The maximum over \(m\in[a,b]\) occurs at \(m=\sqrt{ab}\), giving 

\[
 \frac{\sqrt b-\sqrt a}{\sqrt b+\sqrt a}
 =\tanh\bigl(\tfrac14\log(b/a)\bigr).
 \tag{DB.31}
\]

Consequently, with \(v_e=\|V_e\|_\infty\),

\[
 C_{vu}\le\tanh\Bigl(\sum_{e:\ u,v\in I_e}v_e\Bigr)
          \le\sum_{e:\ u,v\in I_e}v_e.
 \tag{DB.32}
\]

Indeed a mixed finite difference in \(a_v,a_u\) of one \(V_e\) has size at most \(4v_e\). The constants in (DB.32) use the total-variation convention specified above.

### 5.2 Exact weighted block readout

Choose one physical current-mesh anchor \(x_v\) for each component. All distances below are in one common ambient current lattice, not a quotient that collapses a component and not a union of unconverted native counting measures. For a scalar or rectangular matrix \(M\), define the weighted Schur norm using both row and column sums,

\[
 \|M\|_\gamma=\max\left\{
 \sup_a\sum_b e^{\gamma\rho(x_a,x_b)}|M_{ab}|,
 \sup_b\sum_a e^{\gamma\rho(x_a,x_b)}|M_{ab}|\right\}.
 \tag{DB.33}
\]

For a current index, \(x_i\) is its bond site. This norm is submultiplicative, including rectangular products: the triangle inequality for the physical metric gives the exponential weight inequality, and Tonelli gives each row and column bound.

Let \(L\) be the full logarithmic density before normalization, including all factors actually depending on \(z\). Define

\[
 Q_{vi}=\sup_{a,b:\ a_w=b_w\ (w\ne v)}
                \|L_i(a)-L_i(b)\|,
 \qquad H_{ij}=\sup_a\|L_{ij}(a)\|.
 \tag{DB.34}
\]

For every pair of unit current block directions, (DB.26) gives

\[
 \|\operatorname{Cov}_\nu(L_i,L_j)\|_{\rm op}
 \le\tfrac14[Q^{\mathsf T}(I-C)^{-1}Q]_{ij}.
 \tag{DB.35}
\]

If \(\|C\|_\gamma\le\kappa<1\), \(\|Q\|_\gamma\le q/P\), and \(\|H\|_\gamma\le h/P^2\), then the exact mass Hessian satisfies

\[
 \left\|D_z^2\log Z\right\|_\gamma
 \le\frac1{P^2}\left\{h+\frac{q^2}{4(1-\kappa)}\right\}.
 \tag{DB.36}
\]

Pure scalar contributions can be split from \(L\) and then included with their actual derivatives. The first derivative is bounded by the actual supremum score or a separately proved centered-score plus scalar bound.

Equation (DB.36) is noncircular. To apply it to the source, however, one must prove (DB.34) for the complete current dependence and (DB.32) for the actual cross-component interactions. Smallness of the final reduced Hessian cannot be used to prove these hypotheses. Choosing an anchor also costs the diameter of its component when converting source support-distance bounds to (DB.33).

## 6. Actual source input that is available independently

### 6.1 Pure stopped-prefix response, with old raw masses retained

For the pure part of the literal LFR I (1.60) density, the actual constrained matrices are \(K_j=C_j^*\Delta^{(j)}C_j\), with the correct principal/Schur restrictions. On the source chart, CMP99 Section B, especially (3.59), (3.61), (3.63)–(3.65), controls the operator perturbation by the small native displacement. Its Sections D–E supply the local free-coordinate and principal-inverse constructions. The same comparison includes the background-current term in (3.156).

At fixed real free variables,

\[
 L_{{\rm pure},i}
 =-\tfrac12\sum_j a_j^{\mathsf T}(K_j)_i a_j
     +(\log J)_i+\text{actual cross-force responses},
 \tag{DB.37}
\]

and \(L_{{\rm pure},ij}\) contains the corresponding second coefficient derivatives. For Schur pieces use (DB.16), not just the first term. The actual cutoff gives \(\|a_j\|_\infty\le CP_j\); consequently the quadratic score carries \(P_j^2\), not a universal constant.

For an eligible attempted component at scale \(r\), the source componentwise geometry gives, on each strip's own \(j\)-mesh,

\[
 D_j(P)\le C(1+LMR_{j+1})^4,
 \qquad N_r\le C\ell_r^{p_N}.
 \tag{DB.38}
\]

This is the LFR I p.177 eligibility clause and pp.192,198 preparation construction, as recovered explicitly in the geometry notes. It must not be replaced by a current-scale bounding box subdivided into \(j\)-cells. The prepared complex displacement is \(\widehat\alpha_r\le Cg_r\ell_r^A\), with fixed \(A\), including the top-band polynomial enhancement.

The operator perturbation estimate therefore gives the **modulus**, not only the imaginary-part, bound

\[
 \begin{split}
 \sup_a|L_{\rm pure}(\zeta,a)-L_{\rm pure}(0,a)|
 &\le C\widehat\alpha_r\sum_{j=h}^{t}D_j(P)(1+P_j)^2
     +C g_r^{-u}\ell_r^B e^{-cR_r}\\
 &\le Cg_r\ell_r^{A'}+C g_r^{-u}\ell_r^B e^{-cR_r}.
 \end{split}
 \tag{DB.39}
\]

Any genuinely parameter-only quadratic factor can be kept separately before this estimate. Actual cross forces are bounded using their real cutoff endpoints and their native coefficient rows; no invented off-minimum linear force is introduced. Coarea and local determinant responses use their trace rows. The failed-relocation term in (DB.39) is the actual source displacement and Jacobian contribution, with its scale factors retained.

If \(M(a,x)\ge0\) is an arbitrary measurable factor whose raw arguments are unchanged by \(\zeta\), then multiplying the literal density by \(M\) does **not** change (DB.39). It changes the positive reference measure. Thus (DB.39), and the normalized analytic consequences of Section 8, hold with this factor present, irrespective of its internal correlations, size, or raw regularity. This is a useful genuine extension of the pure-kernel estimate. It is not valid for \(M(\Phi_\zeta(a,x))\) unless that pullback is independently controlled.

LFR II pp.391–392 identifies the completed canonical masses \(T'_k(Y)1\) as functions of the new retained raw field on \(Y\) and states that they do not participate in subsequent ordinary transformations. On the fixed-raw part of that source interface they have zero explicit score. Their influence on an integral remains through its actual positive law. A later moving-raw interface must still be checked rather than inferred from this statement.

### 6.2 Completed canonical components

LFR II p.379, following (1.72), identifies the only native-dependent factors of the completed canonical operation as the constrained quadratic and the component-self term \(V(X^-)\). It explicitly includes boundary terms from all earlier renormalization steps in the latter. Its native deformation creates a decaying connection to the deformation support, and the text bounds the resummed deformation by the same small expression as the quadratic deformation. Equations (1.73)–(1.75), p.380, compare with the positive real operation **before** normalization.

Thus, on that actual completed source chart, the density has a pointwise form

\[
 p_\zeta(a)=p_0(a)e^{c(\zeta)+\sigma(\zeta,a)},
 \qquad \sup_{\zeta,a}|\sigma(\zeta,a)|\le\delta_r=o(1).
 \tag{DB.40}
\]

Native Cauchy estimates of \(\sigma\), followed by the genuine current-map composition, give centered score and second-score estimates for this completed operation. This is a source input independent of C05; it does not automatically identify a failed stopped prefix with a conditional fiber of that completed operation.

### 6.3 The precise remaining preintegration question

LFR I pp.191–192 and (1.70) give analytic bounds for the resummed newly created \(C^{(n)}\) terms and discuss the \(g_j\) factor in the top-band fluctuation differences. These statements cannot by themselves be read as a bound on the logarithmic density of every arbitrary stopped interacting kernel with all archived completed terms still unintegrated.

For the direct real route, the needed replacement is only a complete score bound such as (DB.34), or the projective bound (DB.40) on the existing chart. The proposed running-tail induction can supply the archived relative part of that bound without requiring an enlarged analytic radius for an arbitrary inherited relative atom. The next section proves exactly what that proposal gives once the actual incidence sum has been verified.

## 7. The small-relative-tilt induction, with the covariance paid

Let \(\Pi\) be the exact ordinary normalized partial operation on a common analytic chart, with \(\Pi1=1\) and \(\|\Pi\|\le M\). All ordinary masses stay in their literal positions. Let the complete incoming relative interaction be \(R\), on that same chart, with \(\|R\|\le a\), where

\[
 u:=M(e^a-1)<1.
 \tag{DB.41}
\]

No additional radius is imposed on \(R\). Then

\[
 \Psi_\Pi(R):=\log\Pi e^R,
 \qquad |\Psi_\Pi(R)|\le-\log(1-u),
 \tag{DB.42}
\]

and the exact tilted normalized operation has

\[
 \|\Pi_R\|\le\frac{Me^a}{1-u},
 \qquad
 \|\Pi_R-\Pi\|
 \le\frac{M(1+M)(e^a-1)}{1-u}.
 \tag{DB.43}
\]

**Proof.** \(\Pi e^R=1+\Pi(e^R-1)\), so its distance from one is at most \(u\). The series branch of the logarithm yields (DB.42). The first bound in (DB.43) is the quotient bound. For the second use

\[
 (\Pi_R-\Pi)F
 =\frac{\Pi[(e^R-1)F]-\Pi F\,\Pi(e^R-1)}{\Pi e^R}.
 \tag{DB.44}
\]

In particular, the moving normalizer is present in its numerator.

The Fréchet derivatives in the relative interaction are exact:

\[
 D\Psi_\Pi(R)[F]=\Pi_RF,
 \qquad
 D^2\Psi_\Pi(R)[F,G]
 =\Pi_R(FG)-\Pi_RF\,\Pi_RG.
 \tag{DB.45}
\]

Consequently, for \(a\) below a fixed \(M\)-dependent ceiling,

\[
 \Psi_\Pi(R)=\Pi R+\mathcal N_\Pi(R),
 \qquad
 |\mathcal N_\Pi(R)|\le C_M a^2.
 \tag{DB.46}
\]

Indeed the covariance functional in (DB.45) has norm at most \(M_a+M_a^2\), where \(M_a=Me^a/(1-u)\), and integral Taylor remainder proves (DB.46). The linear term is the actual normalized transport, with its dependence on the external current. It is not replaced by a current-independent expectation. The normalizer covariance is exactly the quadratic term which the induction must pay.

### 7.1 Projective archived tilt

**Conditional sufficient estimate, stronger than the main application.**
If the incident archived relative catalog obeys

\[
 \sup_{\zeta,a}\sum_{G:\,\mathrm{participating}}|R_G(\zeta,a)|
 \le K_r,\qquad K_r\le C\ell_r^D A_{r-1},
 \tag{DB.47}
\]

then its contribution to the projective density difference about any fixed positive anchor \(a_*\) is at most \(4K_r\):

\[
 \begin{split}
 \sigma_R(\zeta,a)={}&R(\zeta,a)-R(0,a)\\
 &-R(\zeta,a_*)+R(0,a_*),
 \qquad |\sigma_R|\le4K_r.
 \end{split}
 \tag{DB.48}
\]

This uses only the existing activity-value chart. It needs no arbitrarily larger inherited chart and no analytic extension of an old raw argument. A term independent of all integrated variables is scalar for this operation and can be factored with its mass; its actual external derivatives remain in the scalar decomposition.

Equation (DB.47) is not claimed as a full-value incident-catalog theorem
for the actual source histories. An atom can have a tiny native response
into a component while its unchanged full value has no summable
component incidence. Counting such full values, or copying an incoming
atom over fictitious fine subdivisions, would not prove (DB.47).

The main boundary-induction application instead estimates the complete
anchored differences
\[
 \sup_{a_{\rm ext},a_P}
 \sum_G\sup_{\zeta\in\mathcal D^+}
 |R_G(\zeta,a_P)-R_G(\zeta,a_P^*)|
 \le Cg_r^{-u}(1+\ell_r)^D A_{r-1}.
\]
This is the actual proper-slot/forcing-leaf statement RL.11, combined
with the fixed-fiber identities in the stopped-density and normalized-tilt
notes. It includes a fixed inverse-coupling cost, which the running AF
tail pays. No bound on the full values of every remotely participating
atom is substituted. Native-only differences retain their actual map
response and graded row before a new component root is assigned.
Terms using variables integrated in distinct components remain cross
interactions for the joint integral.

### 7.2 A genuinely noncircular recurrence lemma

Let the bare relative catalog be zero. Suppose the already verified linear transport accounting and source geometry reduce the remaining positive-norm recurrence to

\[
 A_r\le(1+C\ell_r^D A_{r-1})A_{r-1}+f_r,
 \qquad A_{r_0-1}=0.
 \tag{DB.49}
\]

The quadratic term is exactly of the size in (DB.46) or (DB.43) after (DB.47). Define \(F_r=\sum_{b=r_0}^r f_b\). If

\[
 2C\sum_{b=r_0}^r\ell_b^D F_{b-1}\le\log2
 \quad\hbox{for every }r,
 \tag{DB.50}
\]

then \(A_r\le2F_r\), uniformly in the starting cutoff \(r_0\).

**Proof.** Assume the conclusion at earlier indices. Unfold (DB.49):

\[
 A_r\le\sum_{b=r_0}^r f_b
     \prod_{s=b+1}^r(1+C\ell_s^D A_{s-1})
 \le F_r\exp\left(2C\sum_{s=r_0}^r\ell_s^D F_{s-1}\right)
 \le2F_r.
 \tag{DB.51}
\]

This is an induction on a finite cutoff. The proposed bound is never used at the very step where it is being proved.

On the retained AF trajectory \(t_b=g_b^{-2}\), \(t_b\ge t_r+a(r-b)\), a fresh envelope of the form

\[
 f_b\le C t_b^u\ell_b^A e^{-c\ell_b^p},\qquad p>1,
 \tag{DB.52}
\]

has a summable tail. For every fixed \(0<c'<c\), at sufficiently large \(t_r\), comparison with the integral in \(s=t_b\) gives

\[
 F_r\le C' e^{-c'\ell_r^p},\qquad
 \sum_{b\le r}\ell_b^D F_{b-1}\le C''e^{-c''\ell_r^p}
 \tag{DB.53}
\]

for any fixed further rate loss \(0<c''<c'\), after changing the constants. To see this, set \(v=\log s\) in the comparison integral; its exponent is 

\[
 (u+1)v+A\log v-cv^p.
\]

Since \(p>1\), every fixed linear or logarithmic loss is absorbed by an arbitrarily small fixed loss in \(c\). The second tail comparison is identical. One common ceiling therefore enforces (DB.50), and (DB.47) tends uniformly to zero.

There is an essential qualification. A factor \(1+Cg_r\ell_r^D\) charged to every old atom at every ordinary UV step is not AF summable: the comparison integral contains \(\int^\infty s^{-1/2}(\log s)^Dds\). The ordinary source operator costs must therefore be paid by the existing one-time direct-use marks, genuine coarsening, or another proved contraction. The relative extra factor in (DB.49) is summable. This note does not turn an unproved repeated linear transport into (DB.49).

## 8. Derivative consequences of the complete projective bound

Suppose the literal fixed-support density has

\[
 p_\zeta(a)=p_0(a)e^{c(\zeta)+\sigma(\zeta,a)},
 \qquad \sup_{\zeta\in\mathcal D^+,a}|\sigma(\zeta,a)|\le\delta<\log2.
 \tag{DB.54}
\]

The common positive reference is \(\mu_0=p_0/\int p_0\). The exact mass identity is

\[
 \log\tau(\zeta)-\log\tau(0)
 =c(\zeta)+F(\zeta),\qquad
 F(\zeta)=\log\mu_0e^{\sigma(\zeta)}.
 \tag{DB.55}
\]

The scalar \(c\) cancels from normalized insertions but remains in mass and native derivatives. The series branch gives

\[
 |F|\le A(\delta):=-\log(2-e^\delta).
 \tag{DB.56}
\]

There is also pointwise domination of the normalized complex measure,

\[
 |d\Pi_\zeta|\le e^{2\delta}\sec\delta\,d\mu_0,
 \qquad \|\Pi_\zeta\|\le\sec\delta.
 \tag{DB.57}
\]

The first bound uses the numerator/denominator real amplitudes; the second uses the phase cone against the density's own absolute value. Neither introduces a factor for each internal stage. If (DB.54) holds before averaging, it holds on any literal fixed measurable conditional fiber on which the same factorization remains valid.

Suppose around every real point of the full current cutoff support the analytic chart contains a simultaneous increment polydisc of radius \(p=cP\), in the actual source block norm. Then scalar Cauchy and a two-direction phase alignment give

\[
 \sup_i\|D_iF\|\le A(\delta)/p,
 \qquad
 \sup_i\sum_j\|D_iD_jF\|_{\rm op}
 \le 4d_* A(\delta)/p^2.
 \tag{DB.58}
\]

For the second inequality, fix a coordinate of the first block. Choose a unit vector in every second block which aligns the scalar row; apply Cauchy to \(F(z+se_{i,\alpha}+tv)\) with \(|s|,|t|<p/2\). Sum the \(d_*\) first-block coordinates. The dimension is the fixed Lie-algebra block dimension, not the number of lattice sites.

### 8.1 Physical spatial weights

An unweighted scalar bound does not itself give a physical weighted row. A sufficient localization is a genuine normally convergent scalar decomposition \(F=\sum_\Gamma F_\Gamma\) on the same chart, with support \(S_\Gamma\), physical diameter at most \(L_\Gamma\), and

\[
 \sup_i\sum_{\Gamma:\ i\in S_\Gamma}
     e^{\lambda L_\Gamma}\sup_{\mathcal D^+}|F_\Gamma|
 \le K.
 \tag{DB.59}
\]

Then, for \(0\le\gamma\le\lambda\),

\[
 \sup_i\|D_iF\|\le K/p,
 \qquad
 \sup_i\sum_j e^{\gamma\rho(i,j)}
          \|D_iD_jF\|_{\rm op}
 \le4d_*K/p^2.
 \tag{DB.60}
\]

Apply (DB.58) separately to each supported term, pay \(e^{\gamma L_\Gamma}\), and sum. A pointwise positive version also follows by applying the same common Cauchy contours before taking the sum; no exchange of \(\sup\sum\) and \(\sum\sup\) is allowed.

For a complete projective density one can construct these terms without differentiating any raw test: truncate the actual current-to-native map outside \(H^{+n}\), prove the common-chart tail of the **complete** \(\sigma\), and telescope \(F\) at those truncations. If

\[
 \sup_a|\sigma(z,a)-\sigma(z^{[n]},a)|
 \le T\delta e^{-\mu n},
 \tag{DB.61}
\]

then interpolation of the same logarithmic densities gives a scalar tail at most \(C_\delta T\delta e^{-\mu n}\), with support diameter \(\operatorname{diam}H+2n\). Every physical diameter and present-component density must still be paid. A covariance entry bound or an unweighted native operator bound does not establish (DB.61).

### 8.2 C06/C08 interface

If the resulting complete boundary family has \(K=O(1)\), (DB.60) gives precisely

\[
 |D_iW_B(0)|\le C/P_k,\qquad
 \sup_z\sup_i\sum_j e^{\gamma\rho_k(i,j)}
       \|D_iD_jW_B(z)\|\le C/P_k^2.
 \tag{DB.62}
\]

The first condition must be supplied; it is not a consequence of the Hessian condition. On the four-dimensional current lattice, an entrywise supremum produces a fixed symmetric majorant at a smaller rate:

\[
 A^B_{ij}:=\sup_z\|D_iD_jW_B(z)\|
 \le CP_k^{-2}e^{-\gamma\rho_k(i,j)},
\]
\[
 \sup_i\sum_j e^{\gamma\rho_k(i,j)/2}A^B_{ij}
 \le CP_k^{-2}\sum_{n\ge0}(n+1)^3e^{-\gamma n/2}.
 \tag{DB.63}
\]

This is a rate-loss argument. It does not interchange a supremum and an endpoint sum. The source principal Gaussian gap, retained exterior force, regular E/R bounds, and local constrained classical/measure bounds then enter the conditional C06/C08 proofs exactly as written in CA.3, CA.9–CA.10 and C8A.5–C8A.10. The interacting covariance of C08 is obtained later from its scalar Neumann argument; it has not been assumed here.

The common analytic chart and (DB.59), with a positive spatial reserve, also yield the four-dimensional all-current estimate with \((m!)^5\) and divided tree weight, as in the quasilocal-kernel theorem Q21–Q23. A real first/second derivative theorem alone does not establish this all-order conclusion or the unsubtracted native clause [FC.5](primitive_estimates/complete_boundary_estimate.md). Those require the genuine common current/native radii and the scalar \(c\) decomposition in (DB.55).

## 9. analysis decomposition for the boundary-induction integration

| Item | Status in this note | What remains for the complete source application |
|---|---|---|
| Literal normalized first/second derivatives | Proved, DB.5–DB.12 | Match every exact density factor and fixed support |
| Schur and determinant coefficient derivatives | Proved, DB.14–DB.17 | Retain source allocation and actual cutoff response |
| Positive-law covariance from scores | Proved, DB.18–DB.23 | Prove complete current score envelopes |
| Real coupled-component covariance | Proved, DB.26–DB.36 | Verify actual influence and score loads on one physical metric |
| Pure prefix plus arbitrary fixed-raw positive factors | Source coefficient estimate plus proof, DB.37–DB.39 | Confirm eligibility and no moving raw argument in each use |
| Completed canonical projective response | Published pointwise source input, DB.40 | Match its actual current/native pullback |
| Small relative tilt and quadratic normalizer remainder | Proved, DB.41–DB.46 | Verify total incoming incident sum DB.47 |
| Running-tail nonlinear bootstrap | Proved, DB.49–DB.53 | Establish the actual positive recurrence and one-time linear transport accounting |
| First/second current and native analytic readout | Proved implication, DB.54–DB.63 | Complete joint chart, spatial root load, and unsubtracted scalar decomposition |

In particular, neither the pure-kernel estimate nor positivity of the real density establishes the whole stopped interacting law by itself. The running-tail proposal addresses exactly the missing inherited relative contribution. Its acceptance turns on actual source incidence and transport, not on a presumed covariance theorem.

## Sources

- Bałaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP **119** (1988), pp.249–250, 258, 260–262, 269–270.
- Bałaban, *Propagators for Lattice Gauge Theories in a Background Field*, CMP **99** (1985), Sections B and E, especially (3.59), (3.61), (3.63)–(3.65), (3.156), and Theorem 3.15.
- Bałaban, *Large Field Renormalization I*, CMP **122** (1989), pp.177–179, 182, 187–192, 198.
- Bałaban, *Large Field Renormalization II*, CMP **122** (1989), pp.373–380, 390–392, especially (1.66)–(1.75), (1.103)–(1.104).
- [A phase cone for a partially integrated prefix](primitive_estimates/prefix_phase.md), especially P2, P8–P13, P18 and its explicit interaction qualification.
- [Current endpoint estimates for boundary activities](current_endpoints.md), CE4–CE6 and CE11–CE13; used for the stated source-map and coefficient interface, not its claimed complete positive recurrence.
- [Physical root sums and exact rebasing](primitive_estimates/component_roots.md), F1–F21; the complete-relative-density route and its explicit actual-model limitations.
- [Heterogeneous constrained precision and coercivity](heterogeneous_coercivity.md) and [Regular conditional covariance, moments and cumulants](conditional_probability.md); used as conditional endpoint tests, particularly C8A.5 and C8A.7.
- Quasilocal Normalized Kernels, Q1–Q31; used only for its proved analytic/root implications and stated hypotheses.
