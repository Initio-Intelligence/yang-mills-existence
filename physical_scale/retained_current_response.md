# Response to exterior current coordinates

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

## Assumptions and conclusions

This note proves a fixed-history response theorem under the complete conditional C05/C06/C08 estimates. It estimates the **new normalized-kernel current**, not only an inner conditional moment. It supplies a usable smooth-current part of M04/M06 and an exact interface for the outer covariance in H05.

The varying retained coordinates are only the exterior part of the **same current fluctuation field** as the integrated coordinates. They are not the older raw fields, a geometry label, a selector, or a completed component's arbitrary retained data. The canonical source representation, all conditional normalizers, and every nonconstant-in-the-inner-field term remain unchanged.

In particular the absolute physical-carrier marked numerator required by M04, support/selector currents, and the full outer retained-data law remain separate obligations.

## 1. The exact current-coordinate set

Write \(I\) for the current free bonds integrated in the regular interior, and \(O\) for the other current free bonds in the same chart. In the source indexing,
\[
 O=(\Omega_{k+1}\cap\Lambda_{k+1}^{\,c})^{(k)*}
 \quad\hbox{within the same independent-coordinate convention}.
 \tag{RC.1}
\]
CMP119, printed p.270, after (3.25), specifies this split. In particular \(O\) lies inside the new \(\Omega_{k+1}\) shield. It is not the complement of \(I\) in the union of all historical raw coordinates.

The older raw group slots are fixed as well as the old adjoint slots. CMP119 (2.19)–(2.22) places the old operations in \(Z_k\); a surviving completed raw \(V_b\)-slot lies in its owned component \(H_b\subset Z_k\). The new substitution (3.15) changes the current \(V_k\) only in \(\Omega_{k+1}\), while the measure on \(\Omega_{k+1}^{c}\) remains an outer factor. The ordinary four-layer cover separates that set from \(Z_k\) and the stored owned halos. The actual \(C,h\), averaging, nodal and exceptional-bond conventions have only their fixed admitted stencil enlargements, included in the positive remaining collar CE18. Thus an \(I\)- or \(O\)-direction in (RC.1) changes no surviving old raw group slot. AD17.1 by itself states only the older-adjoint assertion; this support argument supplies the required raw-group bridge.

Keep the geometry, coupling, older real raw coordinates, and admitted native background fixed. Before the exterior relocation, write \(t=(z,y)\), with \(z=t_I\), \(y=t_O\). The exact analytic constrained substitution is
\[
 U_k\!\left(\exp i[g_kCt-hD(g_kCt)]V^{(k)}\right),
 \tag{RC.2}
\]
CMP119 (3.15), pp.267–268; see AD17.4–AD17.5 of the C05 estimates. The older \(A_j,\ j<k\), are fixed arguments of that substitution.

These are physical constrained-current variations at fixed coarse datum. In the source constraint notation, let \(q=g_kCt\), \(a=q-hD(q)\), and \(\Phi(a)=Qa+N(a)\). The exact identities \(QC=0\), \(Qh=I\), and \(D(q)=N(a)\) give
\[
 \Phi(a)=Qq-D(q)+N(a)=0
\]
for every full admitted \(t=(z,y)\). Thus varying \(y\) in (RC.1) leaves the prescribed coarse \(V_{k+1}\), its background \(U_{k+1}\), and the current precision \(K\) fixed. The nonlocal response of the reconstructed finer field is retained in \(W^{\rm pre}\); it is not confused with the finite raw-slot support padding above.

On an active fiber the inner conditional law is
\[
 \nu_y(dz)=Z(y)^{-1}{\bf1}_{D}(z)
 \exp H(z,y)\,dz,
 \qquad
 H(z,y)=-\frac12z^TK_{II}z-z^TK_{IO}y+W^{\rm pre}(z,y).
 \tag{RC.3}
\]
Here \(D\) is the literal C07 product of symmetric convex independent-bond balls. Its radii do not vary with \(y\) on this fixed geometry/coupling chart. \(K=C^*\Delta C\) is the actual full constrained precision at the fixed native background.

Every term with a nonzero \(z\)-gradient is included in \(W^{\rm pre}\). Factors depending only on \(y\), including applicable selector factors, exterior Gaussian/coarea factors and the exterior Jacobian after relocation, may be placed in the outer marginal. They cancel from (RC.3), and only there. No term is declared outer merely because it is small or geometrically near a boundary.

The C05 completed-component reduction is already performed where required by the chosen C01 representation. A projected microscopic observable has to undergo those same conditional expectations before it can be used as an insertion \(F\) below.

## 2. Mixed inner/current-exterior derivative estimate

Let \(\rho\) be the current-lattice bond distance. There exist fixed \(c,C>0\) and a fixed nonnegative matrix \(\mathsf A=(\mathsf A_{ia})_{i\in I,a\in O}\) such that
\[
 \mathsf A_{ia}\ge
 \sup_{(z,y)\ {\rm in\ the\ admitted\ real\ chart}}
       \|D_{z_i}D_{y_a}W^{\rm pre}(z,y)\|,
 \qquad
 \sup_i\sum_a e^{c\rho(i,a)}\mathsf A_{ia}
 +\sup_a\sum_i e^{c\rho(i,a)}\mathsf A_{ia}
 \le C P_k^{-2}.
 \tag{RC.4}
\]
It is enough to replace the right side by the explicit complete C08 perturbation prefactor
\(CP_k^{-2}(K_{B,k}^*+K_{ER,k}+K_{{\rm loc},k})\); these prefactors are uniformly bounded at the common ceiling. There is no use of a full exterior-law Hessian here.

**Proof and source match.** The first current endpoint is in \(I\). Permit the second endpoint to range in \(O\) in the C05 current endpoint calculation CE4–CE22. That calculation uses the map (RC.2), its native row measure and the full current contour before restriction to \(I\). An \(O\)-endpoint satisfies the same current-to-old-region shield as an \(I\)-endpoint, since (RC.1) remains in \(\Omega_{k+1}\). None of the older explicit raw slots is differentiated. The first native directional estimate, the simultaneous remaining current Cauchy contour and the endpoint summation therefore apply without changing a carrier or normalizer.

For the independent E/R and local classical/constraint/Haar sectors, use the same full \(t\)-contour and the sector bounds C8A.8–C8A.9; their arguments precede the \(I/O\) restriction. The contour is a fixed \(cP_k\) simultaneous increment neighborhood about each admitted full real \((z,y)\). It is not an origin-centered Euclidean \(2P_k\) ball asserted to contain every exterior value \(|y|\le C_yP_k\). The original map proof admits these increments because \(g_k(C_y+c)P_k\) fits the fixed native reserve; the real cutoff indicators are not complexified. The local classical sector is the complete remainder after the constrained quadratic and is evaluated at the full actual input. Its shifted lower jets are retained. These are estimates of the actual composed functions, not a change in a literal self coefficient.

The result initially has a pointwise weighted row, uniformly on the common contour. Taking one term gives
\[
 \sup_{z,y}\|D_{z_i}D_{y_a}W^{\rm pre}\|
 \le C P_k^{-2}e^{-2c\rho(i,a)}
\]
after choosing \(2c\) below the proved rate. The four-dimensional shell count proves both row and column bounds in (RC.4) at rate \(c\). Thus no interchange of a supremum and a sum is made.

The smooth cutoff in the later exterior relocation is not being complexified. The source tests that are only functions of the retained coordinates are outer factors on this fixed active fiber. The analytic statement here concerns the \(z\)-dependent pre-relocation exponent. These distinctions are exactly AD17.7–AD17.11 and CMP119 (3.20)–(3.25). \(\square\)

Set
\[
 \mathsf C_{ia}=\|(K_{IO})_{ia}\|+\mathsf A_{ia}.
 \tag{RC.5}
\]
The source precision row gives, at a smaller fixed rate if necessary,
\[
 \sup_i\sum_a e^{c\rho(i,a)}\mathsf C_{ia}
 +\sup_a\sum_i e^{c\rho(i,a)}\mathsf C_{ia}\le C_C.
 \tag{RC.6}
\]
The \(O(1)\) principal term is present. A normalized-kernel derivative in \(y\) need not be small in \(P_k^{-1}\).

## 3. Exact normalized response and its signed-kernel bound

For a unit Lie-algebra direction at \(a\in O\), define
\[
 S_a(z,y)=D_{y_a}H(z,y)
 =-z^T(K_{IO})_{\cdot a}+D_{y_a}W^{\rm pre}(z,y),
 \qquad
 \widehat S_a=S_a-\nu_yS_a .
 \tag{RC.7}
\]
Then
\[
 D_{y_a}\nu_y(dz)=\widehat S_a(z,y)\,\nu_y(dz),
 \qquad
 D_{y_a}(\nu_yF)=\nu_y(D_{y_a}F)
                +\operatorname{Cov}_{\nu_y}(F,S_a).
 \tag{RC.8}
\]
Both formulas include the derivative of \(Z(y)\). Any \(z\)-independent contribution to \(S_a\) cancels exactly from \(\widehat S_a\).

Differentiation is justified first for bounded smooth \(F\), on the fixed compact product and an admitted open parameter neighborhood. Sobolev and \(L^p\) extensions follow by the displayed bounds and approximation. They do not require a parameter-dependent change of the product support.

A stronger quantitative statement is
\[
 \|\widehat S_a\|_{L^p(\nu_y)}\le C\sqrt p,\qquad p\ge1,
 \quad\hbox{and hence}\quad
 \|D_{y_a}\nu_y\|_{\rm TV}\le C.
 \tag{RC.9}
\]
Here the total-variation norm denotes the mass of the absolute signed derivative; a convention including a factor \(1/2\) changes only the constant.

**Proof.** Let \(m=\nu_y z\), which lies in the closure of the convex product. The C08 centered coordinate estimate gives
\[
 \|z_i-m_i\|_{L^p(\nu_y)}\le C\sqrt p
\]
uniformly in \(i,y\). By (RC.5),
\[
 \|D_{z_i}S_a(z,y)\|\le\mathsf C_{ia}.
\]
Integrate this derivative on the admitted segment from \(m\) to \(z\) and use Minkowski:
\[
 \|S_a(z,y)-S_a(m,y)\|_p
 \le \sum_i\mathsf C_{ia}\|z_i-m_i\|_p
 \le C\sqrt p.
\]
Centering adds at most a factor two. This proof uses the actual deterministic mixed derivative envelope; it does not infer a kernel response from a Hessian gap alone. \(\square\)

In particular a bounded but nonsmooth insertion has a controlled smooth-current kernel response,
\[
 |\operatorname{Cov}_{\nu_y}(F,S_a)|
 \le C\sqrt{p'}\,\|F\|_{L^p(\nu_y)},
 \qquad 1<p<\infty,\quad p'=p/(p-1).
 \tag{RC.10}
\]
This is a value bound at one current direction. Spatial decay requires the actual inner Sobolev information of \(F\), as follows.

## 4. Exponential spatial response, including the conditional mean

Use the C08 scalar covariance kernel
\[
 \mathsf G_{ij}=\frac2{\lambda_0}e^{-\gamma\rho(i,j)}
\]
from C8A.12. Choose \(0<a<\min(\gamma,c)\), and put
\[
 \mathsf T_{ia}=\sum_{j\in I}\mathsf G_{ij}\mathsf C_{ja}.
 \tag{RC.11}
\]
The triangle inequality for \(\rho\) and (RC.6) give fixed weighted row and column bounds for \(\mathsf T\). In particular, at any smaller fixed rate \(a_1<a\),
\[
 \mathsf T_{ia}\le C_Te^{-a_1\rho(i,a)}.
 \tag{RC.12}
\]
All constants are independent of the number of integrated or retained current coordinates.

The covariance inequality applied to (RC.8) proves
\[
 \boxed{
 |D_{y_a}(\nu_yF)-\nu_yD_{y_a}F|
 \le\sum_{i\in I}\mathsf T_{ia}
                    \|\nabla_iF\|_{L^2(\nu_y)} .}
 \tag{RC.13}
\]
Thus an insertion supported on \(X\subset I\) obeys the same bound with \(i\in X\). This is a derivative of the normalized actual expectation; it is not the derivative of a replacement native observable.

The corresponding anchored sum over all same-current exterior directions is finite. At a fixed smaller rate \(a_2<a_1\),
\[
 \sum_{a\in O}e^{a_2d(a,X)}
 |D_{y_a}(\nu_yF)-\nu_yD_{y_a}F|
 \le C\sum_{i\in X}\|\nabla_iF\|_{L^2(\nu_y)}.
 \tag{RC.13a}
\]
Indeed \(d(a,X)\le\rho(a,i)\) for \(i\in X\), and the weighted row of \(\mathsf T\) applies. This controls the physical current-direction sum at fixed older data. It is not a sum over a localized expansion in every retained raw/history coordinate, and it contains no unproved shifted-regulator substitution.

For the coordinate conditional mean,
\[
 \|D_{y_a}m_i\|\le C_Te^{-a_1\rho(i,a)}.
 \tag{RC.14}
\]
The mean itself can still be \(O(P_k)\) near a conditioned boundary. Equations (RC.14) and the C08 profile describe different quantities.

Let \(y(s)\), \(0\le s\le1\), be an admitted real path inside this fixed chart. Integrating (RC.13) yields
\[
 \begin{split}
 |\nu_{y(1)}F_{y(1)}-\nu_{y(0)}F_{y(0)}|
 \le\int_0^1 \Big\{
 &\nu_{y(s)}|\partial_sF_{y(s)}|\\
 &+\sum_{i,a}\mathsf T_{ia}
       \|\nabla_iF_{y(s)}\|_{L^2(\nu_{y(s)})}
       |\dot y_a(s)|\Big\}\,ds .
 \end{split}
 \tag{RC.15}
\]
The Sobolev norm is evaluated along that actual path. An endpoint norm or an unshifted regulator has not been substituted for it. A straight segment may be used when the relevant current balls and the fixed native admission make that segment admissible.

## 5. Pullback through the actual exterior relocation

Let \(a\) denote the retained coordinate after the source change of variables and \(y=\mathcal R(a;H)\) its pre-relocation value. AD17.8–AD17.10 gives exactly
\[
 \widetilde\nu_a=\nu_{\mathcal R(a;H)}.
 \tag{RC.16}
\]
The source map is bond-local in \(a\); its background \(H\) is held fixed in the present derivative. Consequently
\[
 D_{a_b}(\widetilde\nu_a\widetilde F)
 =\widetilde\nu_aD_{a_b}\widetilde F
 +\sum_c D_{a_b}\mathcal R_c(a;H)\,
             \operatorname{Cov}_{\nu_{\mathcal R(a)}}(F,S_c).
 \tag{RC.17}
\]
With the literal bond convention the sum has one bond block; allowing its fixed endpoint stencil changes only a fixed finite multiplicity.

The source relocation has a uniformly bounded real first derivative. Explicitly, its BCH expression is
\[
 \mathcal R_b(a;H)
 =\frac1{ig_k}\log\{\exp(ig_ka_b)\exp[-i\chi_b(a_b)H_b]\}.
\]
The real cutoff has a fixed transition shape at the running dimensionless threshold \(\delta_k\asymp g_kP_k\), so \(\|D_a\chi\|\le Cg_k/\delta_k\). The first-step notation \(\delta_0\) in CMP119 p.252 is the corresponding running threshold, not a fixed absolute radius. The source gives \(|H_b|\le C\varepsilon_k e^{-cR_k}\), with \(\varepsilon_k/\delta_k\) fixed. Differentiating the BCH expression on its fixed absolute logarithm neighborhood therefore gives
\[
 D_a\mathcal R=I+O(|H|/\delta_k+|H|),
\]
and hence
\[
 \|D_a\mathcal R\|\le C_{\mathcal R}
 \tag{RC.18}
\]
with a fixed constant. Equivalently this is the first-derivative bound in the literal local change-of-variables estimate CMP119 (1.21)–(1.24), pp.251–252, transferred by (3.22). For a previously fixed permitted cutoff, the constant includes its fixed dimensionless first derivative.

Therefore (RC.9) and (RC.13) survive the pullback, with constants multiplied by \(C_{\mathcal R}\). The exterior Jacobian has no term in the conditional score: it multiplies numerator and denominator by the same factor. Its full derivative remains in the **outer** marginal.

This is a real first-derivative statement. A generic \(C^\infty\) cutoff does not supply an all-order fixed Gevrey/factorial bound. No arbitrary complex continuation of \(\chi(a)\) or all-order raw-\(a\) analyticity is being claimed.

## 6. Native precision and force variations: the exact additional terms

For a fixed-support admitted native direction \(h\), allow \(K\), \(y\), and \(W\) to vary, keeping the actual coupling, raw slots and geometry fixed. A direction in an independent native-current slot refers to the chosen admitted analytic extension; a physical direction must be an actually admitted physical parameter path. In the original, uncentered free coordinates the score is
\[
 S_h=
 -\frac12 z^T(D_hK_{II})z
 +(D_hb)^Tz+D_hW,
 \qquad
 D_hb=-(D_hK_{IO})y-K_{IO}D_hy .
 \tag{RC.19}
\]
The normalized formula remains
\[
 D_h(\nu F)=\nu D_hF+\operatorname{Cov}_\nu(F,S_h).
 \tag{RC.20}
\]
For an explicit bound one must use the actual source coefficient rows and joint native/current scalar derivatives in
\[
 \|\nabla_iS_h\|_{L^2}
 \le \sum_j\|(D_hK_{II})_{ij}\|
                     \{\|m_j\|+C\}
       +|(D_hb)_i|
       +\|\nabla_iD_hW\|_{L^2}.
 \tag{RC.21}
\]
Then C8A.12 applies directly. The factor
\(\|m_j\|\le C(P_k^{-1}+P_ke^{-cd_O(j)})\) is retained. Native variation is not represented by varying only \(W\) while freezing its Gaussian coefficient.

This section records a quantitative interface in the actual source variables, not a claim that every ambient raw/native direction has already passed the source chart test. C05's admitted native directions may be used with their proved coefficient norms. Arbitrary retained raw directions still need their own map and support comparison.

If the Gaussian is written using its outer Schur scalar, set
\[
 G=K_{II}^{-1},\quad
 S=K_{OO}-K_{OI}GK_{IO},\quad
 \mathcal Ey=(-GK_{IO}y,y).
\]
The exact outer response is
\[
 D_h\!\left[-\frac12y^TSy\right]
 =-(D_hy)^TSy-\frac12(\mathcal Ey)^T(D_hK)(\mathcal Ey).
 \tag{RC.22}
\]
This includes the principal inverse response and concerns only the displayed quadratic scalar. Existing determinant, Gaussian normalization and E/vacuum terms remain once in their actual outer-factor/inner-normalizer allocation, with their derivatives retained; (RC.22) introduces no additional determinant. Recentring \(z\) by its Gaussian mean would move the product cutoff; none of the proofs above makes that change of integration coordinates.

## 7. The outer-law interface is now explicit

Write the full positive disintegration locally as
\[
 \mu(dy,dz)=\pi(dy)\nu_y(dz),
 \qquad
 \pi(dy)\ \propto\ a_{\rm out}(y)\,Z(y)\,dy
 \tag{RC.23}
\]
on a continuous fixed-history chart; other retained variables or discrete histories can remain in the outer parameter. Then
\[
 D_{y_a}\log[a_{\rm out}(y)Z(y)]
 =D_{y_a}\log a_{\rm out}(y)+\nu_y S_a .
 \tag{RC.24}
\]
The conditional centering in (RC.8) has not erased this outer score, the Schur term, the coarea factor, the relocation Jacobian, or the history masses.

More explicitly, (RC.23)–(RC.24) use the pre-relocation coordinate \(y\). In the post-relocation coordinate \(a\), the outer density is
\[
 a_{\rm out}^{\rm pre}(\mathcal R(a))\,
 J_{\mathcal R}(a)\,Z(\mathcal R(a)),
\]
and its logarithmic derivative is \(D\mathcal R\) applied to the pre-relocation outer score plus \(D_a\log J_{\mathcal R}\). The latter cancels only from the conditional score in (RC.17).

For any \(F,G\),
\[
 \operatorname{Cov}_{\mu}(F,G)
 =\mathbb E_\pi\operatorname{Cov}_{\nu_y}(F,G)
  +\operatorname{Cov}_{\pi}(\nu_yF,\nu_yG).
 \tag{RC.25}
\]
Suppose, separately, that the **actual** outer law on the relevant fixed-history current chart has a weighted scalar covariance inequality with kernel \(\mathsf G^{\rm out}\). Equation (RC.13), including any direct retained derivatives, then controls the second term. If \(F,G\) have no direct \(y\)-dependence, the resulting positive kernel on the inner indices is
\[
 \mathsf G^{\rm eff}
 =\mathsf G+\mathsf T\,\mathsf G^{\rm out}\,\mathsf T^{\,T}.
 \tag{RC.26}
\]
For example, use Minkowski in the outer \(L^2\) norm to obtain this formula with
\(\|\nabla_iF\|_{L^2(\mu)}\) and \(\|\nabla_jG\|_{L^2(\mu)}\).
Weighted row norms multiply, so a fixed exponential row bound for the actual outer kernel yields one for (RC.26).

The new result is the bounded, exponentially local \(\mathsf T\). Neither C08 nor this note supplies \(\mathsf G^{\rm out}\) for the full mixture of retained fields and histories. H03's proved mixed-reset posterior inequality has its own erased/retained variables and cannot simply be declared that missing current-field inequality. This is the precise H05/M07 interface.

## 8. Higher jets and the remaining marked numerator

For a finite set \(A\) of distinct derivative labels in an admitted smooth chart, the exact normalized response identity is
\[
 D_A(\nu F)=
 \sum_{B\subseteq A}\ 
 \sum_{\pi\in\mathcal P(A\setminus B)}
 \kappa_\nu\big(D_BF,\ (D_CH)_{C\in\pi}\big).
 \tag{RC.27}
\]
The empty partition means \(\nu D_AF\). This identity follows by repeated differentiation of the same normalized generating function; it includes all normalizer derivatives. It is not a newly proved arbitrary-mark all-order bound.

The C08 cumulant theorem can estimate these terms only with the actual displayed Sobolev norms of \(D_BF\) and every score \(D_CH\). For native/current directions on the existing analytic chart, C05 supplies the \(W\)-part of the scalar jets. Native score insertions also contain the actual \(K\)- and force derivatives displayed in (RC.19), and require their coefficient/Sobolev estimates. For same-current exterior \(y\) at fixed background, \(K\) is fixed and its force score is linear, already covered by (RC.5)–(RC.9). For arbitrary incoming microscopic marks, raw cutoff directions and support-changing histories, those required insertion norms and physical carrier expansions are precisely the uncompleted M04/M06 work.

The stated M04 target is stronger than (RC.13):
\[
 \sum_Z w_{h',\kappa+\delta}(Z)\,r_Z
 \le C(L)\,\mathcal B_{\rm in}(F_k).
 \tag{RC.28}
\]
Here \(r_Z\) is the actual pre-quotient localized marked numerator triple, with direct, previous-current and new kernel-current records, on physical supports and the shifted regulator versions. The new score bound controls one smooth component of the new-current cost. It does not create the localized numerator, identify its scalar coefficient in the F01 basis, or pay an \(e^{\kappa |P|}\) physical interior cost for a residual normalized component.

For changing selectors/support, the relevant exact formula is a difference of normalized measures on a common measurable space. A smooth score with fixed \(D\) cannot represent a genuine on-support jump. The support boundary current has to be estimated from the actual selector geometry and law.

## 9. The usable current-rarity supplement

The companion [Joint current rarity and outer averaging](joint_current_rarity.md) supplies, for any prescribed set \(J\) of admitted current coordinates satisfying \(d_O(i)\ge d_0(a)\) for every \(i\in J\),
\[
 \nu_y\{\|z_i\|\ge aP_k\ \forall i\in J\}
 \le e^{-c_aP_k^2|J|},
 \tag{RC.29}
\]
and the exact outer/insertion versions JR.6–JR.8. Its proof uses full-vector linear-tilt concentration and a finite-dimensional sphere net; no independence of current coordinates is needed.

That result can pay a selector-boundary term only after the actual selector event has been represented by these current-coordinate events, with its multiplicity and mark costs. It is not an inherited-low-margin or unreplaced-sector theorem. In particular an outer event \(A\) retains its factor \(\pi(A)\) when (RC.29) is averaged.

## 10. Exact next bottleneck

At the retained C01/AF/source scope, the following are now concrete outputs:

1. An actual fixed-geometry current score, including its normalizer, with \(L^p\) norm \(C\sqrt p\).
2. An exponentially localized response of exact regular conditional means to same-current exterior data.
3. A real first-derivative pullback through the source exterior relocation.
4. Exact native Gaussian/force and outer marginal score formulas.
5. The composition criterion (RC.26), identifying the additional outer inequality needed for full-law covariance.

The next analytic step for M04 is the Wilson-specific positive **marked numerator** estimate (RC.28), with all physical carrier, raw/selector-current and shifted-regulator costs. For H04/H05 it is the sector and outer retained-law estimate needed to apply (RC.25), including the still-unidentified inherited and unreplaced events. C05's scalar activity norm and C08's conditional moments do not, by themselves, imply either statement.
