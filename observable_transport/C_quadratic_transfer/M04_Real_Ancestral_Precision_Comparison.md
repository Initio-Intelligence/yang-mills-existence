# A summable real comparison of the actual birth-scale precision

This note addresses the real primitive-matrix part of UD.19. It keeps one ordinary birth-scale precision, including its constraint-force correction and the actual averaged soft gauge, while changing its background along a homogeneous admitted ancestor chain. The matrices are transported into one fixed birth frame before they are compared. The resulting operator and finite-marginal trace bounds are uniform in the age of the birth.

The statement concerns the untruncated Gaussian coefficient of the actual source normal form. It does not identify a Gaussian comparison with the complete interacting conditional law. It does not construct a common complex outside-parameter family, prove raw carrier support for the transporting gauges, or establish a uniform-depth marked or density induction.

## 1. The chain, the fixed operator, and the normalization

Work in four dimensions. Fix a microscopic spacing \(\eta\), an integer blocking factor \(L>1\), and a finite homogeneous torus. Put \(h_j=L^j\eta\). Let \(b\) be a birth step: its ordinary transformation integrates a field at spacing \(h_b\), subject to its one-step average at spacing \(h_{b+1}\). All domains through the finite chain considered here are the full homogeneous domains. In particular, there are no changing holes, old boundary components, or changing free-coordinate lists in the assertion below.

Consider actual real source-admitted fields \(V_j\), for \(b+1\le j\le N\), and their minimal microscopic configurations

\[
 F_j=U_j(V_j).
 \tag{AP.1}
\]

Admissibility means the hypotheses of the source variational construction and its ordinary P/Q-regular comparison hold at every listed step. In the representatives used by that construction,

\[
 V_j=\exp(iB_j)M^jF_{j+1},\qquad
 \|B_j\|_\infty\le C_L\epsilon_j,
 \quad \epsilon_j=g_jp_0(g_j),
 \qquad b+1\le j<N.
 \tag{AP.2}
\]

This is the homogeneous specialization of CMP119, printed pp.266--267, (3.10)--(3.14). It precedes the R split. We assume a fixed sufficiently small weak-coupling ceiling for all the listed fields. We do not assert that an arbitrary-depth density induction has already produced such a chain.

An important exact nesting fact is

\[
 F_j=U_{b+1}(M^{b+1}F_j)
       =U_b(M^bF_j)
 \quad\hbox{as minimal orbits},\qquad j\ge b+1.
 \tag{AP.3}
\]

Indeed, the literal iterated average makes the tangent kernel of either finer constraint on the right a subspace of the \(j\)-constraint tangent. Hence the interior critical field \(F_j\) is critical on that finer fiber. Its stronger coarser-scale regularity also places it in the birth regular class. The uniqueness of the regular critical orbit in CMP102, printed p.279, Theorem 1, then identifies it with the indicated birth minimum. This argument does not assume that the entire broader birth-regular admissible set lies in the stricter \(j\)-regular class. Thus each \(F_j\) is an actual critical background for the **same birth-b ordinary problem**, with its own target \(M^{b+1}F_j\). Merely being a regular arbitrary field would not suffice for the gauge-null assertion used below.

Let \(\mathcal F_b\) be the actual birth-b independent bond list: the ordinary nonexceptional bonds, with one distinguished \(b_0(c)\) removed for each next coarse bond. It is fixed throughout this note. The complete linearized one-step constraint is solved by \(C_b(F)\); it is the identity on \(\mathcal F_b\). This is the source exceptional-bond solve, not an arbitrary right inverse. Its range is the linearized zero-average subspace. Its stencil and both its norm and the inverse exceptional coefficient have bounds depending on fixed \(L\), not on \(b\), the volume, or \(\eta/h_b\). See CMP99 p.428, (3.156)--(3.158), and CMP109 pp.267--268.

All quadratic matrices below use the dimensionless **birth coordinates** \(z\): the physical birth-link displacement starts as \(g_b C_b(F)z\), and the classical action carries its original factor \(g_b^{-2}\). The birth lattice is rescaled to unit spacing when matrix norms are taken. No later \(g_j\) or \(h_j\) is substituted into this normalization.

## 2. The actual constrained precision and the averaged gauge

### 2.1 The force terms are part of the matrix

In the source notation, the classical birth quadratic form is

\[
 \langle B,\Delta_b(F)B\rangle
 =\langle B,(QG_1Q^*)^{-1}B\rangle-a\langle B,B\rangle
       -2\langle H_1\widetilde D_b^{(2)}(B),J(F)\rangle.
 \tag{AP.4}
\]

This is CMP99 p.428, (3.156), with the birth index substituted for the source index. The polynomial \(\widetilde D_b^{(2)}\) is the literal quadratic correction from linearizing the next nonlinear average. Moreover, \(G_1,H_1\) already include the earlier constraint-force correction from (3.127)--(3.138), printed pp.421--423. Neither correction is discarded. In particular, (AP.4) is not replaced by a bare Maxwell quadratic or by the square of a prolongation alone.

At the critical orbit (AP.3), its restriction to the exact constraint tangent is the Hessian of the constrained classical action. Gauge invariance on that fiber implies that the Hessian annihilates every center-fixed infinitesimal gauge direction, including its cross pairings with other tangent vectors. This statement uses the complete force correction. It would generally be false for the unconstrained second derivative with its multiplier term omitted.

### 2.2 The complete nonlinear average is differentiated

For a birth field \(V\), write

\[
 w_x(V)=V(y,x),\qquad x\in B(y),\quad y\in T^{(b+1)},
 \tag{AP.5}
\]

where \(V(y,x)\) is the **full nonlinear group average of the contour transports** defined in CMP109 p.253, (0.11). The source soft term is a fixed positive multiple of
\(\sum_x[1-\operatorname{Re}\operatorname{tr}w_x(V)]\); see p.254, (0.14).

The source chooses the ordinary saddle representative with \(G(V_*)=0\), as stated on p.265 after (2.2). Since its summands are nonnegative on the compact group, this means

\[
 w_x(V_*)=I\quad\hbox{for every sampled }x.
 \tag{AP.6}
\]

It does not say that every individual contour entering the average is the identity. Those individual contour derivatives and all derivatives of the nonlinear group average must remain in the quadratic coefficient.

Define the relative linear sampler by

\[
 \tau_V(B)_x={1\over i}{d\over dt}
   \Log\!\left[w_x(e^{itB}V)w_x(V)^{-1}\right]_{t=0}.
 \tag{AP.7}
\]

At a canonical representative (AP.6), this is exactly the linear coefficient used in CMP109 p.266 before (2.5): the paper explicitly expands the same relative averaged variable. Thus the soft quadratic is \(c_{\rm gf}\|\tau_{V_*}B\|^2\), with the fixed coefficient \(c_{\rm gf}>0\) determined by the source trace convention. No derivative of an individual contour has been substituted for the derivative of its nonlinear average.

There is no additional second-derivative term in this soft Hessian. For a real curve \(w(t)\) with \(w(0)=I\), write \(w(t)=\exp[i(tT+t^2R+O(t^3))]\). The real trace of the term linear in \(R\) vanishes, so the second derivative of \(1-\operatorname{Re}\operatorname{tr}w(t)\) is the fixed trace norm of \(T\). Equivalently, the outer soft potential is critical at the identity. This is also the degree-two/degree-at-least-three separation in source (2.5).

For an arbitrary real regular representative \(F\), put \(V=M^bF\) and define the transported coefficient extension

\[
 K_b^{\rm rel}(F)
 =C_b(F)^*\{\Delta_b(F)+c_{\rm gf}\tau_V^*\tau_V\}C_b(F).
 \tag{AP.8}
\]

At (AP.6) this is the actual complete source precision. Away from that section it is the relative extension in (AP.7), not the Hessian of the absolute soft functional at a noncanonical field.

### 2.3 Exact covariance and canonicalization

Let \(u\) be a real microscopic gauge transformation, restricted to the birth vertices for the induced coarse action. Let \(T_b(u)\) act on free birth coordinates by \(\operatorname{Ad}_{u(e_-)}\). Endpoint covariance gives

\[
 w_x(V^u)=u(y)w_x(V)u(x)^{-1},
\]
\[
 \tau_{V^u}(T_{\rm full}(u)B)_x
       =\operatorname{Ad}_{u(y)}\tau_V(B)_x.
 \tag{AP.9}
\]

The identity follows by differentiating the **whole** relative product in (AP.7). The exact nonlinear coarse constraint is endpoint-covariant too. Linearizing it and using uniqueness of the exceptional solve gives

\[
 C_b(F^u)T_b(u)=T_{\rm full}(u)C_b(F).
 \tag{AP.10}
\]

The complete classical constrained Hessian is covariant; its propagator and force covariance are also written explicitly in CMP99 pp.395--396, (3.28)--(3.34). Consequently

\[
 K_b^{\rm rel}(F^u)=T_b(u)K_b^{\rm rel}(F)T_b(u)^*.
 \tag{AP.11}
\]

This agrees with the actual fluctuation covariance statement CMP109 p.269, (2.16). It transports the constraint subspace, its independent coordinates, and the soft coefficient together.

For completeness, any \(V=M^bF\) has an exact birth canonicalization: choose \(r_b(y)=I\) at the next centers and \(r_b(x)=w_x(V)\) elsewhere in each birth block. Then \(w_x(V^{r_b})=I\), and the next average is unchanged. Lift this birth-site gauge consistently to the microscopic field. Equation (AP.11) shows that \(K_b^{\rm rel}(F)\) is orthogonally equivalent to the actual source precision at that canonical representative. We do **not** independently canonicalize successive chain fields before applying the source comparison (AP.2), which might change that comparison. Canonicalization is used only to identify the coefficient and its positive gap.

## 3. A uniform analytic matrix estimate in birth units

For a relative microscopic potential \(A\), use the exact homogeneous specialization of CMP99 (3.37)--(3.38):

\[
 \|A\|_{\mathcal R_b(F)}=
 \max\{h_b\|A\|_\infty,
        h_b^2\|\nabla_F A\|_\infty,
        h_b^3\|D_F^*D_F A\|_\infty\}.
 \tag{AP.12}
\]

The source's compatible covariant derivative conventions are used in this expression. All homogeneous lower-level inequalities are weaker than the birth-level ones. Local real regularity is the source condition (3.35)--(3.36), not a global weak-link gauge assumption.

For a matrix on free birth bonds, define the two-sided weighted block norm

\[
 \|M\|_\rho=\max\left\{
 \sup_e\sum_f e^{\rho d_b(e,f)}\|M_{ef}\|,
 \sup_f\sum_e e^{\rho d_b(e,f)}\|M_{ef}\|
 \right\}.
 \tag{AP.13}
\]

Here \(d_b\) is distance in unit birth-lattice coordinates. Pointwise real adjoint gauges are isometries for this norm and for the ordinary operator norm.

### Lemma AP.1: source analytic bound

There are \(\alpha_*,\rho,m,M>0\), independent of the birth index, the microscopic mesh, and the volume, such that the following hold on the source regular class with a sufficiently small fixed ceiling.

1. The coefficient (AP.8) has a holomorphic extension for
   \(F_A=e^{i\eta A}F\), \(\|A\|_{\mathcal R_b(F)}<\alpha_*\), and
   \(\sup\|K_b^{\rm rel}(F_A)\|_\rho\le M\).
2. On a real critical orbit (AP.3), \(mI\le K_b^{\rm rel}(F)\le MI\).
3. For \(\|A\|_{\mathcal R_b(F)}\le\alpha_*/2\),

\[
 \|K_b^{\rm rel}(e^{i\eta A}F)-K_b^{\rm rel}(F)\|_\rho
       \le C\|A\|_{\mathcal R_b(F)}.
 \tag{AP.14}
\]

**Proof.** The scale normalization is the source's unit-lattice one in CMP99 Section E, pp.427--428. The relevant analytic neighborhood is (3.37)--(3.38), not a microscopic link sup norm with an index-dependent radius. Theorem 3.4, p.400, gives analytic propagators with the same regularity and kernel bounds as the real operators. The force-corrected versions are given by the explicit uniformly convergent series (3.130) and (3.138); the smallness estimate for their additional coefficient is (3.136)--(3.137). The text on p.423 makes the constants depend only on fixed \(d,L\). The extra third-derivative condition in (3.38) is retained precisely to control this force coefficient.

The coarse inverse in (AP.4) obeys the exponential unit-lattice kernel bound (3.132), for \(G_1\) as well as \(G\). Its scale factors are not suppressed by notation: before rescaling, that kernel has the source factors \(h_b^{-2}h_b^{-d}\), its input potential is the link angle divided by \(h_b\), and the two kernel sums carry their coarse cell measures. The resulting angle quadratic scales as \(h_b^{d-4}=1\) in the present dimension. Rescaling the birth lattice to unit spacing therefore gives the asserted dimensionless matrix bound uniformly in \(\eta/h_b\). Its complex continuation follows by the same perturbation series: analytic variation of \(QG_1Q^*\) is bounded in the unit weighted matrix norm, and its real inverse has the uniform bound (3.132); a fixed smaller complex radius permits inverse Neumann expansion. The local term \(\widetilde D_b^{(2)}\) has a fixed unit-block stencil and uniformly bounded coefficients, while \(H_1^*J\) has the corresponding dimensionless bound by (3.133), (3.136)--(3.137). This supplies the complete force part of (AP.4), not merely the uncorrected propagator.

The one-step maps \(C_b\) and \(\tau\) have fixed-L stencils. They are analytic on the fixed small-diameter contour tube. The relative birth readout \(M^b(e^{i\eta A}F)(M^bF)^{-1}\) is bounded by \(C\|A\|_{\mathcal R_b}\) uniformly in the number of microscopic averages. Here is the scale accounting in that assertion. If \(\|A\|_{\mathcal R_b}\le\alpha\), then at an intermediate spacing \(\ell_s=L^s\eta\le h_b\) the relative angle satisfies the bootstrap bound \(C\alpha\ell_s/h_b\). The corresponding background plaquette ceiling is \(C\alpha_0(\ell_s/h_b)^2\). After factoring the explicit angle scaling \(\ell_s/h_b\), the main averaging row is one. The error words in WA.1--WA.8 and WA.13, from the source positive averaging kernels, are therefore bounded by a product of factors
\[
 1+C\alpha_0L^{-2(b-s)}+C\alpha L^{-(b-s)}.
\]
Both exponent sums are bounded independently of \(b\), closing the bootstrap on a fixed smaller \(\alpha\)-ball. The inverse gauge products in CMP98 (104)--(108) have the same summable relative-angle sizes. This is a fixed analytic radius in birth units, with no factor \(C^b\). Hence the exceptional inverses and the full nonlinear averaged sampler remain uniformly analytic. Exponential kernel bounds, followed by the convergent sum over the unit lattice with a smaller positive rate \(\rho\), give the upper bound in (AP.13). This proves assertion 1.

For assertion 2, CMP99 p.428 after (3.158) gives a uniform positive gap on the axial constrained free space. At a critical orbit the full classical constrained form is gauge-null, as explained after (AP.4). Decompose any constrained tangent field into its fixed-L axial projection and a center-fixed gauge direction. Both the projection and its inverse reconstruction have fixed-L bounds. At the canonical section, \(\tau D\phi=-\phi\) on center-fixed gauge variables, up to the harmless orientation convention. Thus the norm of the full tangent is bounded by a fixed constant times the axial norm plus \(\|\tau B\|\). The source axial gap and the positive soft quadratic imply a gap for their sum. Since \(C_b\) retains every independent entry, \(\|C_bz\|\ge\|z\|\). Equation (AP.11) transfers this gap to arbitrary real representatives. The upper bound was already proved in assertion 1.

Finally apply the Banach-valued Cauchy estimate to
\(t\mapsto K_b^{\rm rel}(e^{i\eta tA}F)\) on the disk of radius proportional to \(\alpha_*/\|A\|_{\mathcal R_b}\). The bound in assertion 1 gives (AP.14). Analytic stars here mean the source analytic transpose continuation; on the real class they are the ordinary adjoints. ∎

## 4. Direct ancestor comparison, without multiplying step inverses

Use \(F_{j+1}\) as the reference in CMP102 Proposition 9, printed pp.305--309. By (AP.3), it is the exact \(j\)-minimum for the reference data \(M^jF_{j+1}\). The source relative Landau representative therefore gives a real microscopic gauge \(u_j\) such that

\[
 F_j^{u_j}=e^{i\eta A_j}F_{j+1}.
 \tag{AP.15}
\]

Integrate the derivative estimate (190), p.308, along \(tB_j\). Its row measure cancels the \(h_j^{-d}\) factor, and its exponential kernel has a uniform row sum in the homogeneous geometry. Since the relative field vanishes at \(B_j=0\),

\[
 \|A_j\|_\infty\le C\epsilon_jh_j^{-1},\qquad
 \|\nabla_{F_{j+1}}A_j\|_\infty\le C\epsilon_jh_j^{-2},\qquad
 \|D_{F_{j+1}}^*D_{F_{j+1}}A_j\|_\infty
                      \le C\epsilon_jh_j^{-3}.
 \tag{AP.16}
\]

These are the direct variational bounds, not a composition of \(j-b\) inverse maps. In birth units they imply

\[
 \|A_j\|_{\mathcal R_b(F_{j+1})}
       \le C\epsilon_j L^{-(j-b)}.
 \tag{AP.17}
\]

The derivative and third-order entries in fact carry the stronger powers \(L^{-2(j-b)}\) and \(L^{-3(j-b)}\). The background \(F_{j+1}\), regular on its coarser scale, belongs to the required birth-regular class: restrict its local regular gauges to birth patches and use the same scale factors. No global small-link gauge is inferred.

Let \(K_j=K_b^{\rm rel}(F_j)\), and let \(T_j=T_b(u_j)\). Lemma AP.1 and exact covariance give

\[
 \|T_jK_jT_j^*-K_{j+1}\|_\rho
       \le C\epsilon_jL^{-(j-b)}.
 \tag{AP.18}
\]

To telescope, fix **one** birth frame. Set \(O_{b+1}=I\) and
\(O_{j+1}=T_jO_j\), and define

\[
 \widehat K_j=O_j^*K_jO_j.
 \tag{AP.19}
\]

Every \(O_j\) is pointwise orthogonal on the same free birth list. Hence (AP.18) is exactly a bound on \(\widehat K_{j+1}-\widehat K_j\). There is no product of its norm constants and no independent change of the marginal coordinates between consecutive comparisons.

The source coupling inequality CMP119 p.255, (2.6), gives for \(j>b\)

\[
 {g_j\over\sqrt{1+\beta'g_j^2(j-b)}}\le g_b
       \le(1+\beta_0)g_j.
 \tag{AP.20}
\]

On the fixed weak ceiling this implies
\(g_j/g_b\le C\sqrt{1+j-b}\) and
\(p_0(g_j)\le C p_0(g_b)\). Consequently

\[
 \sum_{j=b+1}^{N-1}\epsilon_jL^{-(j-b)}
 \le C\epsilon_b\sum_{n\ge1}\sqrt{1+n}L^{-n}
 \le C_L\epsilon_b.
 \tag{AP.21}
\]

No monotonicity of \(g_j\), positive beta-function lower speed, or short-age restriction is used.

### Theorem AP.2: summable actual real precision increments

Under the explicit homogeneous chain assumptions of Section 1,

\[
 \sum_{j=b+1}^{N-1}
   \|\widehat K_{j+1}-\widehat K_j\|_\rho
       \le C_L\epsilon_b,
 \qquad mI\le\widehat K_j\le MI.
 \tag{AP.22}
\]

In particular, with \(K_*=\widehat K_{b+1}\),

\[
 \sum_j\left\|
 K_*^{-1/2}(\widehat K_{j+1}-\widehat K_j)K_*^{-1/2}
 \right\|_{\rm op}\le C_L\epsilon_b.
 \tag{AP.23}
\]

The constants are independent of the age \(N-b\), the volume, and the mesh ratio \(\eta/h_b\). They apply to the full force-corrected precision in the real, transported averaged-gauge birth coordinates.

## 5. One finite-marginal Gaussian certificate

Fix any set \(I\) of birth free bonds, retaining the entire Lie algebra fiber on each selected bond. Let \(P_I\) be its projection **after** the common transport (AP.19), and let its real rank be \(r_I\). Define

\[
 \Sigma_j=P_I\widehat K_j^{-1}P_I^*,\qquad
 \Sigma_*=P_IK_*^{-1}P_I^*.
 \tag{AP.24}
\]

The upper and lower bounds in (AP.22) give uniform positive bounds for all these covariances. Put
\(E_j=K_*^{-1/2}(\widehat K_j-K_*)K_*^{-1/2}\) and
\(J_I=K_*^{-1/2}P_I^*\Sigma_*^{-1/2}\). Then \(J_I^*J_I=I\), and exactly

\[
 \Sigma_*^{-1/2}\Sigma_j\Sigma_*^{-1/2}
       =J_I^*(I+E_j)^{-1}J_I.
 \tag{AP.25}
\]

For a sufficiently small birth weak ceiling, \(\|E_j\|\le C\epsilon_b<1/4\). The resolvent identity, (AP.23), and compression by the isometry \(J_I\) imply

\[
 \sum_j\left\|
 \Sigma_*^{-1/2}(\Sigma_{j+1}-\Sigma_j)\Sigma_*^{-1/2}
 \right\|_{\rm op}\le C_L\epsilon_b,
\]
\[
 \sum_j\left\|
 \Sigma_*^{-1/2}(\Sigma_{j+1}-\Sigma_j)\Sigma_*^{-1/2}
 \right\|_1\le C_Lr_I\epsilon_b.
 \tag{AP.26}
\]

The rank is its actual rank; it has not been replaced by the size of the final coarse core. Applying UD.1 once to the total covariance difference yields

\[
 p_{\Sigma_N}(x)\le p_{\Sigma_*}(x)
       \exp\{C_Lr_I\epsilon_b+
              C_L\epsilon_b|\Sigma_*^{-1/2}x|^2\}.
 \tag{AP.27}
\]

The same matrix \(\Sigma_N\) generates both its inverse quadratic and its determinant. Thus the real primitive Gaussian comparison spends one \(O(\epsilon_b)\) energy fraction and one \(O(r_I\epsilon_b)\) determinant cost, independently of age. A born cutoff remains an insertion in this comparison; no repeated removal or renormalization of that cutoff is asserted. Conditional means from fixing additional exterior free coordinates are not bounded by (AP.27).

## 6. What the coupling and action normalization do, and do not, say

The per-ancestor bound can be displayed without hiding its coupling ratio:

\[
 C\epsilon_jL^{-(j-b)}
 =C g_b\,{g_j\over g_b}\,p_0(g_j)L^{-(j-b)}.
 \tag{AP.28}
\]

Equation (AP.20) is what makes this sum finite relative to the birth smallness \(g_bp_0(g_b)\). The precision itself always used the birth action normalization \(g_b^{-2}\) and birth angle \(g_bz\). If the same physical birth displacement were instead parametrized as \(g_jw\), its old action quadratic would be

\[
 {1\over2}\left({g_j\over g_b}\right)^2
       \langle w,K_b w\rangle.
 \tag{AP.29}
\]

That factor cannot be discarded, and this rewritten coordinate is not the native j-th innovation. The theorem also does not replace the inherited classical action by a bare current-scale Wilson action or absorb the source interaction/counterterm corrections into (AP.4).

### A covariant single-direction corollary

Fix one terminal coarse bond and one Lie generator of norm one. Vary its link by the normalized physical displacement \(\exp(i g_N tT)\), within the same native homogeneous coefficient tube, and denote the resulting minimum by \(F_N(t)\). Use the source relative Landau representation with reference \(F_N(0)\):
\[
 F_N(t)^{u(t)}=e^{i\eta A(t)}F_N(0),\qquad A(0)=0.
\]
Proposition 9 and (190), now for this single input direction, give
\[
 \|\dot A(0)\|_{\mathcal R_b(F_N(0))}
       \le Cg_NL^{-(N-b)}.
 \tag{AP.30}
\]
Define \(K^{\rm cov}(t)=K_b^{\rm rel}(e^{i\eta A(t)}F_N(0))\), and take any fixed birth marginal in this co-moving frame. Lemma AP.1 and the same inverse/compression calculation as (AP.25) imply
\[
 \|\dot K^{\rm cov}(0)\|_\rho
 +\|\Sigma(0)^{-1/2}\dot\Sigma(0)\Sigma(0)^{-1/2}\|_{\rm op}
       \le Cg_NL^{-(N-b)}.
 \tag{AP.31}
\]
The corresponding relative trace norm is at most \(Cr_Ig_NL^{-(N-b)}\). The normalized birth-background link displacement, by contrast, satisfies the single-direction bound
\[
 {1\over g_b}\left\|
 {d\over dt}\Log\!\left[
 M^b(e^{i\eta A(t)}F_N(0))(M^bF_N(0))^{-1}
 \right]_{t=0}\right\|_\infty
 \le C\,{g_N\over g_b}L^{-(N-b)}.
 \tag{AP.32}
\]

These are covariant directional estimates in the explicitly moving Landau frame. Differentiating the transport back to a fixed canonical birth representative adds the derivative of its field-dependent adjoint gauge and is not controlled here. Nor does a single-direction operator bound imply a bound on the sum over all terminal directions of the trace norms. The canonical raw-current and absolute-carrier derivative ledgers therefore remain outside this corollary.

There is one exact invariant-domain consequence. Let \(D_I\) be a fixed measurable product of adjoint-invariant norm balls or annuli in the selected full Lie fibers. Its centered Gaussian probability is unchanged by each pointwise adjoint transport, so its actual real single-direction derivative equals the derivative in the co-moving frame. With \(p=p_{\Sigma(0)}\) and \(\delta_N=Cg_NL^{-(N-b)}\), differentiation of the same normalized marginal gives
\[
 \left|{d\over dt}\Pr_{\Sigma(t)}(D_I)\big|_{t=0}\right|
 \le \delta_N\int_{D_I}
       \left(r_I+|\Sigma(0)^{-1/2}x|^2\right)p(x)\,dx.
 \tag{AP.33}
\]
Indeed its score is
\(-\tfrac12\operatorname{Tr}(\Sigma^{-1}\dot\Sigma)
+\tfrac12x^{T}\Sigma^{-1}\dot\Sigma\Sigma^{-1}x\).
The adjoint transport derivative cancels because the entire event is invariant. A reserved Gaussian tail may be applied to the integral in (AP.33); no rare probability is divided out. This observation does not apply to moving Q centers, a noninvariant mark, the interacting density, or a sum of canonical carrier currents.

## 7. The remaining uniform-depth gate

Theorem AP.2 closes a real matrix comparison for the specified admitted chain. It is stronger than numerical plaquette attenuation: it uses the complete source analytic coefficient tube, the actual force-corrected operator, the exact soft-gauge Hessian, both spectral bounds, and one composed birth-space transport.

The following part of UD.19 is still unproved. One needs a **single restriction-consistent complex physical-carrier family** for this transported birth marginal, with a bound analogous to (AP.26) uniformly on the enlarged outside-parameter polydiscs, and with the summed first raw-current bound. Its precision and determinant must come from the same covariance, its disconnected components must agree with the unmarked family, and its real endpoint must retain the actual old domains and reconstruction.

The real Landau gauges \(u_j\) and the birth canonicalizations in this proof are field-dependent. Their pointwise adjoint action is isometric, but this proves neither raw locality nor a bound on their retained derivatives. Weighted matrix-entry decay in (AP.22) is not a connected physical-carrier representation of their dependence on all ancestor data. Nor does this argument control the interaction, cutoff-core frame, or relevant/vacuum extraction budgets accumulated by the complete nonlinear density. Those issues cannot be removed by simply citing the convergent real matrix sum.

## Primary sources

The source statements used above are in Balaban, CMP99 (1985), printed pp.395--400, 421--423, 427--428; CMP102 (1985), printed pp.305--309, especially Proposition 9 and (190); CMP109 (1987), printed pp.253--254 and 265--269; and CMP119 (1988), printed p.255 (2.6) and pp.266--267 (3.10)--(3.14). The CMP102 comparison pages are those used in the UD analysis. The source-defined matrix coefficients are kept distinct from the new relative-extension and alignment argument proved here.
