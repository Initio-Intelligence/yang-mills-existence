# Actual normalized R references and complex marginal transfer

**Annex AE.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Target and result

This chapter concerns the normalized R contour. The statement asks for a simultaneous current-coordinate contour for every actual localized R pullback, including its marginal transfer, the independently extended current, and the denominators in the source construction.

**C-03 is proved at the stated source J0/C-01 scope.** The completed theorem, incorporated in full in Section 10, gives the actual regular R activities a simultaneous native contour containing their full real regular current support. On that contour the transferred, vacuum-subtracted R activity has the bound \(C_Rg_k^{\kappa_0-11}e^{-\kappa_*d_k(Y)}\), with explicit current, native-background, independently extended-current and preparation derivative radii. The five-power primitive-radius loss and the source's six-power old-scale summation loss are both retained.

The shared quantitative map-domain theorem is proved in Theorem E14.3. Section 10 checks its outputs against every domain input of the R proof, then uses the actual R source prescription and its Ward identities. No analytic continuation from the physical graph \(J=J(U)\) is asserted. The true denominators are already included in the completed source R norm; a separate proof below bounds the actual fresh reference in complex total variation and explains its cancellation mechanism.

The auxiliary complex axial-gauge lemma and the optional repeated-reference norm bound retain their explicit premises. They are not needed to claim an uncontrolled bound along an entire marked history. The final theorem does not establish boundary estimates, action/Hessian smallness, arbitrary transported-mark regularity, or history-interface bounds. Status: **L** is a primary source result in its stated scope; **P** is proved here; **C** is an implication whose extra hypotheses remain explicit.

### 2. Primary domains and the actual reference

#### 2.1 Primitive R and prepared R are different domain statements — L

CMP119, pp.259–260, (2.27)–(2.31), gives the primitive R activities the same localized analytic and gauge-invariance properties as the primitive E activities, with

\[
 |R_X^{(j)}(U,J)|\le g_j^{\kappa_0}e^{-\kappa d_j(X)},\qquad
 \alpha_{0,j}=C_0g_j\ell_j^{q_0},\quad
 \alpha_{1,j}=C_1g_j\ell_j^{q_1},\quad
 \ell_j=\log g_j^{-2}.
 \tag{R14.1}
\]

The primitive domain is the regular space from CMP109, (1.10)–(1.16). It is not, by definition, the complete multiscale boundary domain introduced later in CMP119, (2.34)–(2.39). CMP109 p.262 defines the primitive domain as a union of **complex** gauge orbits. Its conditions include a real regular representative, a small complex relative field with a first-difference bound, a current bound, and regularity of reconstructed configurations.

CMP109 p.263 supplies a useful sufficient subdomain: conditions (i)–(iii) with sufficiently smaller constants imply condition (iv), by its displayed application of Proposition 9 of CMP102. In particular the reconstructed curvature bound is at most \(2B_3\alpha'_0\) in the source's scale normalization. Thus choosing \(\alpha'_0\le\alpha_0/(4B_3)\), together with the other stated smallness restrictions, leaves a quantitative reconstruction reserve. This fact can simplify an admission proof; it is not itself an admission proof for the current free variables.

After actual R preparation, LFR II p.375, (1.65), gives an analytic map from the new expanded multiscale domain to the old expanded domain defined in LFR I (1.64)–(1.69). The target is contained in the domains of the old E, R and B terms. LFR II p.390, (1.100), then gives the newly generated bulk R activity the complex bound

\[
 |R'^{(k)}(X,(U,J))|
 \le e^{-p_0(g_k)}e^{-\kappa d_k(X)}.
 \tag{R14.2}
\]

These are strong source statements. To use their norms for current-coordinate differentiation one must still map a quantitative contour about every actual cutoff configuration into the stated **input** domain. Openness alone does not give the needed uniform radius.

#### 2.2 The reference is a finite-core Wilson reference — L

Fix one replacement component and one axial graph in LFR I p.201, (1.100). Its fresh reference has the form

\[
 h_v(dV')={\mathbf1}_{D_g}(V')\,\delta_{G_0}(V')
 \exp\{-g^{-2}A(\zeta_0,U_{k,Z}(V'v))\}\,dV',
 \qquad H(v)=\int h_v(dV').
 \tag{R14.3}
\]

Here \(v\) denotes the retained data in the source-admitted complex extension. The core \(\Lambda\) is a rectangular parallelepiped contained in a cube of side \(100M\) in current lattice units. The cutoff (1.101) restricts the fresh coordinates only:

\[
 V'=\exp(igB),\qquad |B(b)|<M_0\varepsilon_k/g,
 \qquad b\in\Lambda\setminus G_0.
 \tag{R14.4}
\]

In particular this integration domain does not move with \(v\). Let \(n_\Lambda\) be the number of free bonds and \(D=\dim\mathfrak g\,n_\Lambda\). Then \(D\le C_G(100M)^4\). This bound concerns the replacement core; the outer component \(Z\) need not have bounded diameter.

Writing \(U_0=U_{k,Z}(v)\) for the reference minimizing field, LFR II p.358, (1.10)–(1.11), proves on its admitted complex domain

\[
 H(v)^{-1}
 =\exp\{g^{-2}A(\zeta_0,U_0)+I(v)-E_k(\Lambda)\},
 \qquad |I(v)|\le C\log M\,|\Lambda|.
 \tag{R14.5}
\]

This is a holomorphic reference logarithm, hence a nonvanishing statement on that domain. It is stronger than a real lower bound. The extensive retained Wilson term in (R14.5) must be cancelled before estimating the normalized kernel.

### 3. Uniform complex norm of the actual fresh R reference

#### 3.1 Explicit source estimates entering the norm — L with their complex scope

The expansion in LFR II pp.356–358, (1.2)–(1.11), after the change (R14.4), is

\[
 g^{-2}\{A(\zeta_0,U_{k,Z}(V'v))-A(\zeta_0,U_0)\}
 =\tfrac12 B^{\mathsf T}K(v)B+L(v,B)+N(v,B).
 \tag{R14.6}
\]

The notation uses a complex symmetric bilinear quadratic form; \(B\) is still integrated over the real Lie-algebra coordinates. Put

\[
 a_k=\alpha_{0,k}+\alpha_{1,k},\qquad
 \lambda_M=\frac{\gamma_0}{2d(100M)^5},\qquad d=4.
 \tag{R14.7}
\]

The comparison of the quadratic form with the zero-background form, followed by the axial Poincaré bound (1.8), gives

\[
 \operatorname{Re}(B^{\mathsf T}K(v)B)\ge\lambda_M|B|^2
 \tag{R14.8}
\]

provided the source's smallness restriction

\[
 C\{M^6R_k a_k+e^{-R_k}\}\le\tfrac12\frac{\gamma_0}{d(100M)^5}
 \tag{R14.9}
\]

holds. For real backgrounds this is (1.7)–(1.9). The paragraph introducing the complex reference on p.358 explicitly retains the preceding bounds with \(\varepsilon_k\) replaced by \(O(a_k)\); applying the absolute-value bound for the quadratic-form error gives (R14.8). A complex quadratic form is not ordered without taking its real part.

The linear term is exponentially small because the full reference minimizer is stationary on the core. The source moves the factor \(\zeta_0\) to \(1-\zeta_0\) in (1.5), and (1.6) gives the real estimate. The same complex estimate has the explicit form

\[
 |L(v,B)|\le b_{L,k}:=
 C_M p_0(g_k)\frac{a_k}{g_k}e^{-R_k}.
 \tag{R14.10}
\]

The harmless constant \(C_M\) includes the displayed \(M_0\), the fixed source constants, and the bound \( |\Lambda|\le(100M)^4\). The cubic-and-higher remainder obeys the source's (1.2) estimate

\[
 |N(v,B)|\le b_{N,k}:=C g_k^{1-\vartheta}|\Lambda|,
 \qquad 0<\vartheta<1,
 \tag{R14.11}
\]

after the fixed logarithmic cutoff has been bounded by the allowed small negative power of \(g_k\). We do not infer this estimate from Gaussian positivity; it is the actual nonlinear reference estimate on the source-admitted domain.

The Haar coordinate Jacobian has the form \(e^{E_k(\Lambda)}J_g(B)dB\), with the source constant normalization absorbed into \(E_k\), \(J_g(0)=1\), and

\[
 |J_g(B)|\le e^{b_{J,k}},\qquad
 b_{J,k}\le C D(M_0\varepsilon_k)^2.
 \tag{R14.12}
\]

This follows directly from the analytic Haar density in exponential coordinates on the fixed compact Lie group. Its logarithm has no linear term and is bounded quadratically on a fixed chart. The \(g_k^D\) and constant Haar-density factors are exactly the factors represented by \(E_k(\Lambda)\).

For fixed admitted construction parameters, (R14.9) holds and \(b_{L,k}+b_{N,k}+b_{J,k}\) is uniformly bounded for sufficiently small \(g_k\). The factors \(g_k\ell_k^q\), and \(e^{-R_k}\) against fixed logarithmic powers, are retained explicitly. Section 8 checks their compatibility with the fixed choice \(q_0=q_1=q>p_0\) used in the actual native contour theorem.

#### 3.2 Actual normalized-reference theorem — P using §3.1

Define the complex measure \(\nu_v=H(v)^{-1}h_v\). On the admitted source domain,

\[
 \nu_v(dB)=
 e^{I(v)}\,{\mathbf1}_{D_g}(B)J_g(B)
 e^{-\frac12B^{\mathsf T}K(v)B-L(v,B)-N(v,B)}\,dB.
 \tag{R14.13}
\]

Its total mass is one, and

\[
 \begin{split}
 \|\nu_v\|_{\mathrm{TV}}
 &\le
 \exp\{C\log M\,|\Lambda|+b_{L,k}+b_{N,k}+b_{J,k}\}
 \left(\frac{2\pi}{\lambda_M}\right)^{D/2}
 \\&\le K_M,
 \qquad K_M\le\exp\{C_G M^4\log(2M)\}
 \le\exp\{C'_G M^5\}.
 \end{split}
 \tag{R14.14}
\]

For the last two bounds, reduce the admitted coupling ceiling so that \(b_{L,k}+b_{N,k}+b_{J,k}\le C_0D\), with fixed \(C_0\). The first bound holds without that additional simplification. Constants may depend on the fixed source parameters and gauge group, but not on the cutoff, the outer volume, or the diameter of \(Z\). Graph averaging is a finite convex average and obeys the same bound.

**Proof.** Multiply (R14.3), expressed in \(B\), by (R14.5). The factors \(e^{-g^{-2}A(\zeta_0,U_0)}\) and \(e^{E_k(\Lambda)}\) cancel exactly. This gives (R14.13). Take the absolute value, use (R14.8)–(R14.12), enlarge the real integration domain to all of \(\mathbb R^D\), and evaluate the Gaussian integral. The core dimension and the explicit \(M^{-5}\) coercivity give the final bounds. The defining integral and (R14.5) give mass one. Uniform Gaussian domination on compact subsets of the admitted domain proves holomorphy as an \(L^1(dB)\)-valued function. \(\square\)

Consequently, for a jointly analytic mark \(F(v,B)\) with a uniform norm on this domain,

\[
 \left|\int F(v,B)\,\nu_v(dB)\right|
 \le K_M\sup_B|F(v,B)|.
 \tag{R14.15}
\]

This is an actual estimate for the full fixed-core fresh reference on the complex reference domain used in (1.10). It is not a termwise estimate for independently localized random-walk expressions. The final R theorem in Section 10 uses the completed source R norm and its verified native contour for those expressions. This reference theorem is also not an estimate for the posterior of an archived history label, and it does not identify the signed polymer expansion with a probability distribution.

### 4. Contour shrink makes the normalization loss arbitrarily small

#### 4.1 Local normalized kernel estimate — P

Suppose an actual source chart contains the complex ball

\[
 v_0+\{w:\|w\|_*<r\},
 \tag{R14.16}
\]

where \(v_0\) is real and \(\nu_{v_0}\) is the positive reference probability measure. Assume (R14.14) throughout this ball. For \(s=\|w\|_*/r<1\),

\[
 \|\nu_{v_0+w}-\nu_{v_0}\|_{\mathrm{TV}}
 \le\frac{K_Ms}{1-s},\qquad
 \|\nu_{v_0+w}\|_{\mathrm{TV}}
 \le1+\frac{K_Ms}{1-s}.
 \tag{R14.17}
\]

In particular the smaller radius

\[
 r_{\delta}=r\frac{\delta}{K_M+\delta}
 \tag{R14.18}
\]

gives the bound \(1+\delta\), for any fixed \(\delta>0\).

**Proof.** Restrict the \(L^1\)-valued analytic function to the complex line in the direction of \(w\). Cauchy's formula bounds every positive Taylor coefficient by \(K_M\); the geometric sum gives the first inequality. Positivity and normalization give \(\|\nu_{v_0}\|_{\mathrm{TV}}=1\). The second inequality and (R14.18) follow. This proof uses one simultaneous direction, so it introduces no factor proportional to the number of retained coordinates. \(\square\)

The same argument for an order-\(m\) derivative in one unit direction gives

\[
 \|D^m\nu_{v_0}[w,\ldots,w]\|_{\mathrm{TV}}
 \le m!K_Mr^{-m}\|w\|_*^m.
 \tag{R14.19}
\]

Mixed derivatives can instead use an explicitly admitted polydisc. No derivative bound is obtained when (R14.16) has not been verified for the coordinates being differentiated.

#### 4.2 Exact local carrier cost — P as an implication

For \(n_X\) fresh reference integrations contributing to one carrier, if the same admitted shrunken contour is stable under their actual substitutions, their norm cost is at most

\[
 (1+\delta)^{n_X}
 =\exp\{n_X\log(1+\delta)\}.
 \tag{R14.20}
\]

If the geometric counting available for that carrier is \(n_X\le a_M d(X)+b_M\), then

\[
 e^{-\kappa d(X)}(1+\delta)^{n_X}
 \le(1+\delta)^{b_M}
 e^{-[\kappa-a_M\log(1+\delta)]d(X)}.
 \tag{R14.21}
\]

Thus any fixed positive carrier-decay reserve can pay this normalization cost by choosing \(\delta\) sufficiently small. The radius loss is the fixed factor in (R14.18).

For one generation of disjoint replacement cores, the number of cores is bounded by the number of current \(M\)-cubes in a connected carrier. This gives the required linear counting bound in that case. For an arbitrarily long prepared history the relevant \(n_X\), the stable common contour, and the counting bound must still be supplied; (R14.21) does not assert them.

### 5. A complex axial-gauge estimate with all path costs

#### 5.1 Finite rectangular lattice lemma — P

Let \(\mathcal Q=\{0,\ldots,r\}^d\), with complex matrix-group links \(U_e\) satisfying

\[
 \|U_e\|,\|U_e^{-1}\|\le e^\delta,
 \qquad\|U_p-I\|\le\epsilon
 \tag{R14.22}
\]

for all oriented links and plaquettes needed below. For each \(x\), let \(P_x\) be the path from the origin to \(x\) that traverses coordinates in the order \(1,\ldots,d\), and set \(g_x=U(P_x)\). We use the convention \(U^g_{xy}=g_xU_{xy}g_y^{-1}\). Then

\[
 \|g_x\|,\|g_x^{-1}\|\le e^{dr\delta},
 \qquad
 \|U^g_e-I\|\le dr\,\epsilon\,e^{(2dr+1)\delta}.
 \tag{R14.23}
\]

For a current transforming at the initial endpoint,

\[
 \|J^g_e\|\le e^{2dr\delta}\|J_e\|.
 \tag{R14.24}
\]

If \(b=dr\epsilon e^{(2dr+1)\delta}\le1/2\), the principal logarithm of \(U^g_e\) is holomorphic and

\[
 \|\log U^g_e\|\le2b.
 \tag{R14.25}
\]

**Proof.** For \(e=(x,x+e_i)\), compare \(P_x\) followed by \(e\) with \(P_{x+e_i}\). Move the last \(e_i\)-step to its ordered position by at most \(dr\) adjacent interchanges. Each interchange crosses one plaquette. The difference of the two path transports is bounded by \(\epsilon e^{(dr+1)\delta}\), because the total path length is at most \(dr+1\). Telescoping all interchanges and multiplying by \(U(P_{x+e_i})^{-1}\) proves (R14.23). Conjugation proves (R14.24). The absolutely convergent logarithm series proves (R14.25). Every map used is holomorphic in the links and their inverses. \(\square\)

At a real compact-group configuration the path transports have norm one. If the complex field is a multiplicative relative perturbation, only the relative complex size contributes to \(\delta\); an arbitrary real pure-gauge part does not create an exponential transport cost.

#### 5.2 What this gives for a marginal R chart — C

Let \(t=k-j\), \(\theta_t=L^{-2t}\), and suppose a particular actual coarse pair has, on a box containing its localized carrier,

\[
 \|U_p-I\|\le Q_k\theta_t,
 \quad \|J\|\le Q_k\theta_t,
 \quad \|U_e^{\pm1}\|\le e^{Q_kL^{-t}}.
 \tag{R14.26}
\]

If the box radius is \(r_X\) and

\[
 dr_XQ_k\theta_t\exp\{(2dr_X+1)Q_kL^{-t}\}\le\tfrac12,
 \tag{R14.26a}
\]

then (R14.23)–(R14.25) give

\[
 \|\log U^g\|+\|J^g\|
 \le C(1+r_X)Q_k\theta_t
 \exp\{C r_X Q_kL^{-t}\}.
 \tag{R14.27}
\]

Suppose additionally that the **joint coarse pullback**, including its independent current, has an admitted ball of radius \(a_j\) in these variables and the primitive bound (R14.1) there. Its first derivative at the zero pair vanishes: global semisimple gauge invariance makes each linear coefficient an invariant linear functional on the complex Lie algebra, hence zero. Applying the second-order Schwarz lemma along a radial line gives, whenever the point and the needed radial chart are admitted,

\[
 \begin{split}
 |R_X^{(j)}(U,J)-R_X^{(j)}(1,0)|
 &\le2g_j^{\kappa_0}e^{-\kappa d_j(X)}
 \min\!\left\{1,
 \left[\frac{C(1+r_X)Q_k}{a_j}
 e^{C r_XQ_kL^{-t}}\right]^2L^{-4t}\right\}.
 \end{split}
 \tag{R14.28}
\]

This displays the four-power marginal factor without treating complex gauge transformations as norm-preserving. If (R14.26a) fails, only the trivial bound \(2g_j^{\kappa_0}e^{-\kappa d_j(X)}\) follows from this argument; the large-carrier estimate must then do the required work. A fixed polynomial in the carrier radius can be paid from a verified carrier-decay reserve. If \(r_X\) grows with age or with a history component, that dependence must remain in the bound until its sum is estimated.

The premise about the **coarse pullback** is essential. The original activity may depend on a fine reconstructed field. Axial-gauging an averaged coarse field does not, by itself, identify that fine field with the required minimizing-field substitution. Nor does the lemma identify a localized independently extended current with the physical current of a localized gauge field. Those are actual map questions, not gauge identities.

### 6. Exact normalization and the marked quotient

For the frozen replacement \(\rho'(u',v)=h_v(u')H(v)^{-1}\int\rho(u,v)\,du\), the transported mark is

\[
 QF(u',v)
 =\frac{\int\rho(u,v)F(u,v)\,du}{\int\rho(u,v)\,du}.
 \tag{R14.29}
\]

The fresh reference cancels from this ratio exactly. Equations (R14.13)–(R14.21) control the fresh reference when it subsequently occurs in a complex integration or coordinate transfer. They do **not** remove the old conditional denominator in (R14.29), or establish holomorphy of an old posterior that contains hard history selectors. Those responses belong to the marked/history estimates and must retain their interface currents.

There are therefore three distinct statements: exact real marked integral preservation; bounded analytic fresh-reference integration on an admitted domain; and spatial/analytic estimates for the old projected mark. The first is already proved by the frozen-R mechanism, the second is proved above in its source scope, and the third is not supplied by either one.

### 7. The quantitative targets and their resolution

Write \(\Phi_{j,k,X}\) for the actual localized current-coordinate substitution, with all preparation variables and the independent current retained. Let \(\mathcal K_k\) be the full actual regular free-coordinate cutoff from C-01/C-07. The required statements are recorded here to make the final verification explicit.

**Admission.** For every \(z_0\in\mathcal K_k\), the simultaneous contour \(\mathfrak D_{k,X}(z_0)\) must be stable under all decoupling parameters used by the localized expression and satisfy

\[
 \Phi_{j,k,X}(\mathfrak D_{k,X}(z_0))
 \subset \mathcal U_{j,X}^{\mathrm{actual}},
 \tag{R14.30}
\]

with an explicit lower bound for its current-coordinate radii. The right-hand side is the regular primitive domain or the actual prepared domain appropriate to that stage. Theorem E14.3 now supplies the actual contour (E14.49), using the full unprimed cutoff \(P_k=\delta_k/g_k\), the actual relative averaging and minimizing maps, and all nonlinear preparation variables. Section 10.6 maps each required R-domain input to that proof and to the exact return of the source R operation to its regular normal form.

**Complex marginal transfer.** A sufficient target is a carrier norm of the form

\[
 \sup_i\sum_{Y\ni i} e^{\gamma\operatorname{diam}Y}
 \sup_{z\in\mathfrak D_{k,Y}(z_0)}
 |V^R_{j,k,Y}(z)|
 \le C\,g_j^{\kappa_0}\ell_j^A\frac{Q_k^2}{a_j^2}.
 \tag{R14.31}
\]

Here the \(L^{-4(k-j)}\) factor has already paid the old-cell multiplicity. The completed proof instead retains the more conservative fixed five-power inverse-radius loss in (RM.6). After the same carrier localization and old-cell cancellation it gives (RM.9)–(RM.10), and hence the explicit uniform holomorphic carrier bound (RM.13). The primitive R exponent can be chosen arbitrarily large, so this verified fixed loss is sufficient for C-03 as stated. The independently extended current, the large-carrier tail, every nonlinear preparation term and the fixed localization losses are included in that proof. Formula (R14.28) remains a separate optional mechanism; it is not used as an unsupported replacement for the actual R marginal calculation.

**Old-scale summation.** The source estimate in CMP119 (2.46) loses **six coupling powers**. Equations (RM.6)–(RM.10) keep this loss after paying the five primitive-radius powers. The admitted current and native external radii are then used after the normally convergent old-scale sum, giving (RM.15). No unproved contour radius or uncancelled \(L^{4(k-j)}\) factor is paid by an appeal to a large coupling exponent.

The source-normal-form support theorem C-07 and the holomorphic reference logarithm alone do not prove these targets. Their resolution uses the additional map-domain proof and the explicit marginal calculation incorporated in Section 10. This distinction matters for the remaining history and marked-coordinate obligations.

### 8. R-side compatibility of larger running analytic exponents

The following inequalities concern the R-side compatibility of the larger running analytic domains. The remaining construction parameters must satisfy their stated restrictions.

LFR I p.198, (1.94), explicitly permits a preparation depth satisfying

\[
 N\le C\ell_k^v,\qquad \tfrac12v\le p_0-p_1-1.
 \tag{R14.32}
\]

LFR II p.384, (1.80), takes the required waiting depth to be \(N=R_j\), with \(R_j\asymp\ell_j^r\). Thus it is sufficient here that

\[
 \tfrac12r<p_0-p_1-1.
 \tag{R14.33}
\]

The rare-history budget on LFR II p.385 has the explicit sufficient inequality

\[
 c\,p_0(g_j)^2\ge C_M R_j^{d+2};
 \tag{R14.34}
\]

the exponent condition \(2p_0>r(d+2)\) makes this true for a sufficiently small coupling ceiling. These two requirements are consistent by choosing the fixed integer \(p_0\) sufficiently large after \(p_1,r\) are fixed.

The complex Wilson cancellation on LFR II p.368, (1.47), costs

\[
 C_Mp_0(g_k)q_1(g_k)R_k^7L^{-N}.
 \tag{R14.35}
\]

For \(N\asymp\ell_k^r\), this tends to zero for every fixed finite \(q_1\). The component variation on p.379, immediately before (1.73), costs

\[
 C_Mg_kR_k^{d+2}p_1(g_k)^2q_0(g_k),
 \tag{R14.36}
\]

which also tends to zero for every fixed finite \(q_0\). The reference coercivity condition (R14.9) has the same property. Here \(q_i(g)\) denotes the source's fixed logarithmic power, with its constant; it is distinct from the integer exponent \(q_i\).

Choosing **equal** analytic exponents \(q_0=q_1=q\) is a convenient safe choice for these inequalities. The displayed bound on p.368 packages \(\alpha_0+\alpha_1\) using \(C_1q_1\), whereas the bound on p.379 packages it using \(C_0q_0\); equal powers allow both with fixed constants. Any necessary fixed ratio between the analytic amplitudes can be imposed through \(C_0,C_1\), without claiming an incompatible asymptotic ordering of the two powers.

Consequently these R inequalities impose no upper bound on a finite common \(q\). If a complete current-map proof produces only a **verified fixed** logarithmic preparation loss \(\ell_k^A\), choosing \(q>p_0+A\) makes

\[
 \frac{g_k\ell_k^q}{g_k\ell_k^{p_0+A}}
 =\ell_k^{q-p_0-A}\longrightarrow\infty,
 \tag{R14.37}
\]

while preserving (R14.9), (R14.35), and (R14.36). The completed native-map proof retains its actual preparation constants and requires one fixed \(q>p_0\). The more general observation (R14.37) is not used to assume that an unexamined map loss is a logarithmic power, or to prove the boundary-domain conditions remaining in C-05.

### 9. References and hypotheses

Primary references are LFR I, pp. 198 and 201, LFR II, pp. 357–360, 368, 374–375, 379, 385 and 390, and CMP119, pp. 255, 257, 259–260 and 276–277.

CMP109, pp. 262–263, states the smaller-domain inclusion and defines the complex gauge orbit.

The reference-kernel proof concerns the actual finite-core Wilson reference, with its actual cutoff, graph, minimizing field, and normalization. Its validity does not depend on replacing the archived history posterior by the fresh reference law. The completed C-03 proof is given below; the supporting lemmas are auxiliary to it.

### 10. Complete R marginal and derivative proof

The following argument gives the R marginal transfer and its derivative bounds on the stated domain.


#### 10.1. Result and scope

The finite Taylor/Ward part of the R transfer loses at most five powers of a verified old primitive analytic radius. Together with the proved **shared actual preparation-domain inclusion**, this gives an explicit conservative old-scale budget. The source's six-power coupling summation loss is retained. No identity theorem on the graph \(J=J(U)\) is used.

Theorem E14.3 in Annex AD now proves that shared native interior contour, using the actual relative averaging and minimizing maps. Section 10.6 below checks each required output against its equations. The R argument uses those map-domain conclusions; it does not assume an E value bound to obtain an R value bound.

Only the source-defined regular R carriers are considered here. CMP119, p.276, treats inherited R as E without the coupling subtraction. Its subsequent localization assigns carriers crossing the multiscale boundary to B. LFR II, p.390, (1.99)–(1.100), makes the same regular-R/boundary separation after the large-field operation. Those B carriers remain C-05; they have not been deleted or relabelled by this supplement.

#### 10.2. The actual joint composition, not a uniqueness assertion

CMP109, pp.275–277, gives the needed source prescription:

1. Before (3.24), replace the external \(J_{k+1}\) independently by \(J\), and replace the background in the prepared operators by the specified local reconstructed field \(U_{k+1}(\square_0,M'(U))\).
2. Immediately after (3.24), interpret the notation \(E(X,U_j)\) as the jointly extended expression with \(J_j\), constructed as in (3.13).
3. In (3.28), transform the external \(J\) and the coarse fluctuation together with the background. The explicit transformations occur inside \(H_k\). They are analytic local functions of the external field.
4. In (3.33)–(3.36), form the actual coarse determining field \(B=B(U,J,z)\), and evaluate the physical minimizing pullback
   \[
   \Phi_{j,X}(B)
   =
   R^{(j)}
   \left(X,U_j(\square_0,e^{iB}),
              J_j(\square_0,e^{iB})\right).
   \tag{RM.1}
   \]
   The independent external \(J\) remains in \(B(U,J,z)\). It is not identified with the physical current of \(U\).

The actual inherited R expression in CMP119 (2.30) is vacuum-subtracted. Accordingly, the expression expanded below is \(\Phi_{j,X}(B)-\Phi_{j,X}(0)\). Its constant coefficient belongs to the separately constructed source-free vacuum scalar. It is neither assigned a false fourth-order scale gain nor silently dropped from the exact action.

The finite Taylor and Ward identities apply to \(\Phi_{j,X}\) as identities in its determining variable \(B\). Substitution of the actual jointly analytic \(B(U,J,z)\) preserves such an identity. CMP109, p.276, explicitly allows the prepared field to be replaced by an arbitrary regular \(A\) satisfying (3.31), because final localization does make such replacements. CMP116, §1, implements that replacement with the actual localized \(H_k(s)\), including (1.17).

This is a prescription for a particular joint analytic extension of the physical transferred expression. A different holomorphic extension agreeing only on \(J=J(U)\) need not agree with it away from that graph. No such equality is asserted here.

#### 10.3. Shared domain inputs with the needed regularity outputs

Fix the source parameters \(L,M,\kappa_1\) and one admitted trajectory. For each current regular carrier \(Y\), let \(\mathcal C_{k,Y}\) be the simultaneous contour (E14.49) in the current fluctuation, native background, independent current and source preparation variables, containing the complete real regular support. The R proof uses the following source-native properties on that contour. Their quantitative verification is recorded in Section 10.6.

- Every actual far and nearby primitive argument is admitted in its regular source domain.
- The primitive insertion radius and the nearby determining-field perturbation radius admit a common lower radius
  \[
  a_j\ge c_*g_j,\qquad 0<a_j\le1,
  \tag{RM.2}
  \]
  with \(c_*>0\) independent of old depth, cutoff, volume and history. For example, a proved \(a_j\ge c\alpha_{0,j}\), with \(\alpha_{0,j}=C_0g_j\ell_j^q\), gives (RM.2) after reducing the coupling ceiling.
- The actual prepared current-scale field satisfies the source's regularity bounds (3.31)–(3.32) with a uniform ceiling \(Q_k\le1\), simultaneously for the complex decoupling parameters. Consequently its old determining field satisfies, with \(\lambda=L^{j-k}\),
  \[
  \|B_j\|\le C Q_k\lambda,\qquad
  \|\partial B_j\|\le C Q_k\lambda^2,\qquad
  \|\partial^2B_j\|\le C Q_k\lambda^{2+\beta},
  \tag{RM.3}
  \]
  for one fixed \(0<\beta<1\). These are precisely the scaling bounds proved in CMP109 (4.16)–(4.18), including the actual averaging operation. The same bounds hold for the source's insertion variations when those are used.
- The source's far-carrier and localization bounds remain valid on the same contour, with their actual preparation factor \(K=B_0e^{16\kappa_1}\), fixed cutoff-multiplier constants, and the exponent reserve used in CMP116. In particular, neither an independent-current substitution nor a decoupling variable is omitted from this inclusion.

These are domain and map-regularity assertions. They do not assume the desired R marginal estimate.

#### 10.4. Finite Taylor/Ward radius budget

The primitive source input is

\[
\sup_{\mathcal D_{j,X}}
|R^{(j)}(X,U,J)|
\le g_j^{\kappa_0}e^{-\kappa d_j(X)}.
\tag{RM.4}
\]

CMP119, p.260, (2.31), gives (RM.4) and explicitly permits \(\kappa_0\) to be arbitrarily large after fixing the other parameters properly. LFR II (1.100) supplies an even smaller newly generated regular R bound. Thus choosing a fixed larger \(\kappa_0\) below is within the source's stated scope.

The coarse Taylor expansion uses orders at most four and the fifth-order integral remainder. On a contour satisfying (RM.2), its order-\(m\) coefficient has a Cauchy cost at most \(m!a_j^{-m}\), for \(m\le5\). The coefficient kernel moment estimates used in the Ward calculation have the same maximum inverse-radius power. This is visible in CMP109 (4.3)–(4.5), where the derivatives of the minimizing map at the vacuum have fixed regular kernel bounds, and in (4.22), whose displayed bound contains \((\alpha_1/\alpha_2)^4\). The fifth remainder is (3.54), with its fifth inverse coarse-radius power.

The remaining constants in these finite-order estimates are fixed spatial kernel moments. They depend on \(L,M,\kappa\) and the admitted propagator constants, but not on the number of fine sites. The exponential kernel sums in the proof of (4.22) are essential for this statement; a pointwise Cauchy coefficient bound followed by an unweighted sum over fine coordinates would not suffice.

The source subsequently differentiates the localized expression in its insertion parameter \(t_\square\), as stated immediately before CMP119 (3.67). This does not require a sixth inverse old activity radius. The nearby and far estimates above are uniform on the reserved complex insertion tube. For \(0\le t_\square\le1\), the disc \(|h|<1\) has \(|t_\square+h|\le2\). The preparation reserve (E14.11) and the whole-path bound (E14.44) admit this disc, with their spare factors. Apply the fixed unit-radius Cauchy formula to the already bounded expression. Thus the \(t_\square\) derivative costs a fixed factor, independent of \(a_j\), old age and cutoff. The localization parameters are kept simultaneous as in CMP116; they are not differentiated by a separate unsupported real argument.

The Ward identities (4.14)–(4.15) are complex algebraic identities for the gauge-invariant function (RM.1). The first derivative vanishes. The quadratic, cubic and quartic terms acquire, respectively, two, one and zero extra old-scale difference factors. By (RM.3), each surviving term has a factor \(\lambda^4\). The explicitly retained Hölder remainders improve this to \(\lambda^{4+\beta}\), and the fifth Taylor remainder has \(\lambda^5\). Therefore, before summing old cells, the native nearby bounds have the conservative form

\[
\begin{split}
|\mathcal R^{\rm marg}_{j,X;k}|
&\le
C_{\rm W}\,g_j^{\kappa_0}
\sum_{m=2}^4 a_j^{-m}Q_k^m\,
\lambda^4 e^{-\kappa' d_j(X)},\\
|\mathcal R^{\rm irr}_{j,X;k}|
&\le
C_{\rm W}\,g_j^{\kappa_0}
\left(
\sum_{m=2}^4a_j^{-m}Q_k^m\,\lambda^{4+\beta}
+a_j^{-5}Q_k^5\,\lambda^5
\right)e^{-\kappa'd_j(X)}.
\end{split}
\tag{RM.5}
\]

Here \(\kappa'<\kappa\) is the fixed source decay reserve after the finite coefficient-moment sums. CMP119, p.283, says to stop the R analysis at its (3.49); there is no coupling subtraction to perform. That is exactly the marginal term retained in (RM.5).

Using (RM.2), \(Q_k\le1\), \(g_j\le1\), and absorbing \(c_*^{-m}\) into a fixed constant gives

\[
|\mathcal R^{\rm marg}_{j,X;k}|
+|\mathcal R^{\rm irr}_{j,X;k}|
\le
C_* g_j^{\kappa_0-5}
\lambda^4e^{-\kappa'd_j(X)}.
\tag{RM.6}
\]

This deliberately weaker bound keeps a single five-power loss. It does not assert the sharper source coefficient is unchanged when the primitive radii run.

Far carriers have instead the source factor \(e^{-c/\lambda}\), or the corresponding large-carrier exponential. Their one primitive Cauchy cost is \(a_j^{-1}\), as in CMP109 (3.15)–(3.17). For any fixed \(N\),
\[
e^{-c/\lambda}\le C_{c,N}\lambda^N,
\tag{RM.7}
\]
so \(N\ge4\) gives the same conservative marginal budget (RM.6), retaining the remaining carrier decay.

#### 10.5. Localization and the six-power sum

The preparations and localization operations are the source's actual ones: CMP116 §1, then CMP119 pp.275–277 for the complete geometry. The current interior terms satisfy the original regular-source conditions; the boundary-crossing terms are precisely the B terms identified there. The decoupling contour is simultaneous, \(|s(\Delta)|\le e^{\kappa_1}\), and its preparation factor is retained in the hypothesis of §10.3.

Applying the source's localization/resummation estimates to (RM.6), at a fixed current carrier \(Y\), cancels the old-cell count \(O(\lambda^{-4})\) against the factor \(\lambda^4\). The localization prefactor is the fixed one from that source construction, of the form
\[
C_{\rm loc}=C_{\rm W}C_1M^{q_{\rm loc}}e^{C_2\kappa_1},
\tag{RM.8}
\]
with its stated fixed-parameter dependence. A fixed reduction to an admitted \(\kappa_*>0\) accounts for the coefficient-moment and preparation decay losses. No cutoff-dependent change of \(M,\kappa_1\), or unproved extra logarithmic loss is hidden in \(C_{\rm loc}\).

Thus the remaining old-scale majorant is
\[
C_{\rm loc}e^{-\kappa_*d_k(Y)}
\sum_{j\le k}g_j^{\kappa_0-5}.
\tag{RM.9}
\]

Use the six-power estimate actually displayed in CMP119 (2.46), under its source trajectory hypotheses. Taking \(\kappa_0-5\ge7\), and imposing the corresponding coupling ceiling, gives

\[
\boxed{
\sup_{\mathcal C_{k,Y}}|\mathcal R^{\rm transferred}_{k,Y}|
\le
C_{\rm loc}\,
g_k^{\kappa_0-11}\,
e^{-\kappa_*d_k(Y)}.
}
\tag{RM.10}
\]

The loss is five inverse-radius powers plus the source's six-power summation loss. No age upper bound is inferred from the wrong direction of CMP119 (2.6). In particular, this proof does not require a new lower inverse-coupling increment in order to absorb an axial-gauge age polynomial.

For a simultaneous scalar-coordinate polydisc with radii \(r_i>0\) contained in the same verified contour, Cauchy gives
\[
|\partial^a\mathcal R^{\rm transferred}_{k,Y}|
\le
a!\,C_{\rm loc}\,
g_k^{\kappa_0-11}
e^{-\kappa_*d_k(Y)}
\prod_i r_i^{-a_i}.
\tag{RM.11}
\]

When the admitted full current ball is \(\|z\|_\infty<2P_k\), every real center with \(\|z\|_\infty\le P_k\) has simultaneous scalar Lie-coordinate radii \(P_k/(2\sqrt{\dim G})\). Native-background balls require the directional convention stated in Theorem R14.3 below; they cannot be interpreted as unrestricted fine-coordinate polydiscs.

#### 10.6. Verification of the domain inputs and the true denominators

The common contour has the explicit form

\[
\begin{split}
 &\|z\|_\infty<2P_k,\qquad
 \|b\|_{{\rm native},k}<c_{\rm ext}\alpha_{0,k},\\
 &\|J-J_{0,k}\|_\infty<c_{\rm ext}\alpha_{0,k},\qquad
 |s(\Delta)|<e^{\kappa_1}.
\end{split}
\tag{RM.12}
\]

Here \(P_k=\delta_k/g_k=A_1\ell_k^{p_0}\) is the full unprimed source cutoff, \(\alpha_{i,k}=C_i g_k\ell_k^q\) with one fixed \(q>p_0\), and \(c_{\rm ext}\) is fixed by (E14.47). The ratio \(C_1/C_0\), the source parameters, and the common small-coupling ceiling are chosen exactly as in Theorem E14.3. In particular they do not depend on later derivative order.

| Required R input | Quantitative verification on (RM.12) |
|---|---|
| Actual real centers and primitive reconstructed-field domains | (E14.26)–(E14.32) establish a strict smaller-basic-domain reserve at the actual centers, using layerwise minimizing-field estimates, the local Wilson-current formula, and the primary reconstructed-domain inclusion. CMP119 (2.30)–(2.31) gives primitive R exactly the same regular analytic and gauge-invariance properties as E. |
| Actual nonlinear preparation, independent current and decoupling variables | The minima (E14.8), with \(K=B_0e^{16\kappa_1}\), admit the actual CMP116 constraint/minimizer maps. Equations (E14.45)–(E14.48) transfer the native external background and independently varied current to every old scale with conservative coefficient \(C_JL^{j-k}\), including gauge-conjugation costs. |
| Whole far insertion path | (E14.39)–(E14.44) first admit the actual unmodified \(Q_j\) input to the fixed absolute map domain, integrate the actual relative-minimizer derivative from zero there, and then compare the whole output with the running primitive radius. No \(Q_j=Q'_j\) identification or assumption of the desired activity-domain conclusion is used. |
| Nearby determining-field radius and the common lower bound (RM.2) | (E14.15b), (E14.24f) and (E14.32) give \(r_{3,j}\ge c_3\alpha_{0,j}\) and \(\alpha_{2,j}=c_2\alpha_{0,j}\), with uniform reserves along the actual Taylor segments. Taking \(a_j\) to be a fixed fraction of their minimum and of the remaining native radius gives \(a_j\ge c_*g_j\) and \(a_j\le1\) after reducing the coupling ceiling. |
| Prepared-field regularity (RM.3) | The actual preparation bounds in Sections 3 and 5.6 of the E note give \(Q_k\le c_Q\alpha_{0,k}\le1\). CMP109 (4.16)–(4.18) then give the displayed determining-field and difference bounds on this jointly admitted domain. The independent current enters through the prescribed actual prepared field as in (RM.1). |
| Fixed insertion differentiation and carrier localization | (E14.11) and (E14.44) give the unit insertion-parameter disc used in Section 10.4 above. The same simultaneous preparation contour is used in CMP116 Lemma 1, so its fixed localization losses apply. The E proof's map admission is used here; its matching coupling subtraction is not imported into R. |

This table checks map-domain assertions rather than appealing solely to the completion label of C-02. The construction hypotheses retained in J0, including the admitted history geometry and source propagator bounds, remain hypotheses of both contour theorems.

The primitive bound (RM.4) concerns the actual completed R activities, including the denominators and preliminary integrations used to create them. LFR II, pp.374–375, (1.63)–(1.65), constructs their joint analytic pullbacks and (1.99)–(1.100) gives the final convergent activity bound. The fresh finite-core normalized reference itself has the separate complex total-variation bound proved in Annex AE, §§2–4. That reference law is not confused with the archived-history posterior.

More precisely, LFR II (1.98)–(1.100) first completes the R operation and then assigns its boundary-intersecting outputs to B. Its remaining regular R activities satisfy the regular primitive domain and (RM.4), after choosing the coupling ceiling so that \(e^{-p_0(g_j)}\le g_j^{\kappa_0}\). This uses the source's logarithmic polynomial \(p_0\) of degree greater than one. Subsequent regular current-coordinate pullback is therefore into the very primitive domain verified in the table. No arbitrary multiscale boundary tuple is asserted to lie in the regular domain. Its estimates remain in C-05.

The true source denominators are thus already included in the completed primitive holomorphic norm being pulled back. The separate normalized-reference estimate verifies their cancellation mechanism and gives a useful mark-integration norm, but the proof does not multiply an uncontrolled number of reference norms along an entire history. It also does not infer an analytic old-history posterior from a fresh reference denominator.

#### 10.7. Completed R contour theorem

##### Theorem R14.3 — actual regular R contour and marginal transfer

Retain the source-free complete RG representation, its admitted geometry, regular and large-field history decomposition, and consistently normalized trajectory as in J0/C-01. Use its actual E/R/B classification. Choose the fixed source parameters and the common running analytic domains as in Theorem E14.3. Choose one fixed \(\kappa_0\ge12\), permissible by CMP119 p.260 after (2.31), and reduce the common coupling ceiling to meet (RM.2), the reference restrictions when that reference is used, and the source summation estimate.

Then every actual vacuum-subtracted localized regular R pullback, including the inherited marginal/coordinate transfer and the new completed R activities, is jointly holomorphic on (RM.12). There are fixed \(C_R<\infty\) and \(\kappa_*>0\), independent of cutoff depth, torus volume, remaining admitted history and subsequent derivative order, such that

\[
\boxed{
\sup_{\mathcal C_{k,Y}}
|\mathcal R_{k,Y}|
\le C_Rg_k^{\kappa_0-11}e^{-\kappa_*d_k(Y)}.
}
\tag{RM.13}
\]

Here \(\mathcal R_{k,Y}\) is the actual source-normal-form R contribution; its vacuum scalar is separated by the exact source prescription (2.30). The old-cell count is paid by the four marginal scale powers before the old-scale sum. The denominators and preparation factors are those of the actual construction.

For a real current center \(\|z_0\|_\infty\le P_k\), take

\[
r_z=c_GP_k,\qquad
r_b=r_J=c_Gc_{\rm ext}\alpha_{0,k}/2,\qquad
r_s=(e^{\kappa_1}-1)/2,
\tag{RM.14}
\]

with the fixed Lie-coordinate factor \(c_G\) from (E14.52). For scalar-coordinate multi-indices \(u,w,t\), and \(m\) native-background derivative directions of norm at most one, one has

\[
\begin{split}
&\left|
\partial_z^u D_{b_1}\cdots D_{b_m}
\partial_J^w\partial_s^t\mathcal R_{k,Y}
\right|\\
&\quad\le
u!w!t!\,e^m m!\,
C_Rg_k^{\kappa_0-11}e^{-\kappa_*d_k(Y)}
r_z^{-|u|}r_b^{-m}r_J^{-|w|}r_s^{-|t|}.
\end{split}
\tag{RM.15}
\]

For raw scalar link-coordinate derivatives of multi-index \(v\), the native first-difference norm instead admits the simultaneous coordinate radius \(\xi r_b\), giving \(v!(\xi r_b)^{-|v|}\) in place of \(e^m m!r_b^{-m}\). If the chosen native norm includes a first-difference Hölder seminorm of exponent \(\beta\), use \(\xi^{1+\beta}r_b\). No second-order or nonlocal projection estimate for arbitrary raw coordinate directions is asserted from a first-difference norm.

**Proof.** Section 10.6 verifies every shared-domain input in Section 10.3 on the same product contour, retaining actual independent-current and nonlinear preparation maps. The exact prescribed joint composition in Section 10.2 permits the finite Taylor/Ward calculation there, with its vacuum subtraction. The kernel-moment bounds and reserved insertion disc give (RM.5)–(RM.7) with at most five inverse primitive-radius powers. The source's carrier localization and old-cell counting give (RM.9); its actual six-power coupling sum gives (RM.10). The newly generated completed R activities obey the stronger primitive bound and fit the same majorant. Enlarge the fixed constant to \(C_R\). Normal convergence gives joint holomorphy and (RM.13). Cauchy on the scalar-coordinate factors and on discs of radius \(r_b/m\) for the \(m\) background directions gives (RM.15), using \(m^m\le e^m m!\). The stated raw-coordinate alternatives follow from the explicit native-norm embedding, exactly as in (E14.52)–(E14.53). \(\square\)

Under the stated construction assumptions, the regular R contour has a uniform holomorphic norm with carrier decay and the indicated preparation losses. Its application to the Wilson representation requires CL. The exponent in the preceding estimate is a sufficient bound.

This theorem does not prove the full source-free construction or its coupling trajectory independently. It does not prove C-04 action/Hessian smallness, C-05 boundary-domain estimates, C-06 conditional coercivity, arbitrary later marked-coordinate transport, or spatial control of archived-history posteriors and selector currents. Those remain distinct obligations, and every such term remains in the complete law. No Yang–Mills existence claim follows from C-03 alone.


---
