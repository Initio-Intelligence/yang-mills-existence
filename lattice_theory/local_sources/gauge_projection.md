# Gaussian admission, gauge projection and reconstruction

## 4.6 The checked regular Gaussian sector and fresh scalar admission

#### 4.6.1 Gauge directions and constant-source cancellation

Let \(E\) be the tangent space of the coarse averaging constraint at a constrained Wilson minimum. Let \(K\) be its constrained Wilson Hessian in the actual nonlinear constraint chart, including the \(Da\cdot D^2m\) contribution, \(\mathcal N\) its infinitesimal gauge directions fixing block basepoints, and \(D\) the soft axial-gauge differential in B109 (2.5), pp.265–266. Gauge invariance at a critical orbit gives \(K\mathcal N=0\). The averaged contour is a genuine group element on the real domain and is equivariant at both endpoints, by B109 (0.6), (0.9), (0.11), pp.251–253. Consequently \(D\) on a gauge direction is, up to convention, the adjoint of that contour applied to the gauge parameter at its non-basepoint endpoint. It is an isomorphism on \(\mathcal N\); it is not an average of different adjoint maps.

The decomposition \(E=\mathcal N\oplus\ker D\) diagonalizes the two bilinear forms. Thus for \(H=K+D^*D\),

\[
P=H^{-1}K,\qquad P^2=P,\qquad
\operatorname{Tr}P^m=r=\dim E-\dim\mathcal N,\quad m\ge1.
\tag{4.29; P}
\]

On \(\ker D\), \(H\) and \(K\) coincide; on \(\mathcal N\), \(K\) vanishes. This proves the assertion even though that direct sum need not be orthogonal in the original coordinate metric. A constant physical scalar source coupled to the quadratic Taylor part of \(N\sum a_p\) therefore gives the untruncated Gaussian logarithm

\[
\lambda N\mathcal A(U_0)-\frac r2\log(1-N\lambda/X).
\tag{4.30; P}
\]

It follows by the determinant identity \(\det(I-N\lambda P/X)=(1-N\lambda/X)^r\). Source derivatives of order at least two are field-independent on this physical minimizing family, at fixed geometry. The rank may depend on the geometry. The cutoff and nonlinear mark have not been included in (4.30), and its cancellation is a cancellation of the sum of localized terms, not a termwise zero.

The hard constrained covariance of B99 and the soft gauge covariance above are different coordinate realizations. The comparison requires a common averaging constraint and its common constrained Hessian. B109 p.267 identifies the relevant form with B99 (3.156), using the admitted extension of averaging conventions discussed on pp.253–254. With that dictionary fixed, if \(R\) injects gauge parameters, \(A=DR\), and \(J_D=I-RA^{-1}D\), the unit covariances satisfy

\[
C_{\mathrm{soft}}=J_D C_{\mathrm{hard}}J_D^*
+R(A^*A)^{-1}R^*.
\tag{4.31; P}
\]

To prove it, split a fluctuation into its representative in \(\ker D\) and its gauge coordinate. The Wilson form is unchanged by \(J_D\); the two forms have zero cross term. The independent gauge Gaussian has covariance \((A^*A)^{-1}\). Push both back to the original coordinates. With precision coefficient \(X\), multiply the entire covariance by \(X^{-1}\). The axial maps are bounded within fixed blocks on the admitted domain, so this bridge transfers decay with fixed constants. It does not identify different coarse averaging matrices by name.

#### 4.6.2 Variable sources, full Hessians and the scale of the kernel

For the first plaquette variations \(v_p\) at the constrained minimum, \(\sum_pv_p=0\). With symmetric covariance \(C\), put \(K_{pq}=v_p^TCv_q\). Then

\[
\sum_qK_{pq}=0,\qquad
\Big(\sum_pf_pv_p\Big)^TC\Big(\sum_qg_qv_q\Big)
=-\frac12\sum_{p,q}K_{pq}(f_p-f_q)(g_p-g_q).
\tag{4.32; P}
\]

Expand the differences and use symmetry and the row sum to prove the identity. If plaquettes are omitted, the exact right side has the additional term \(\sum_pr_pf_pg_p\), \(r_p=\sum_qK_{pq}\). Boundary forces cannot be removed using interior stationarity.

The nonlinear constrained minimizing map \(m\) contributes to the complete Hessian:

\[
D^2(a_p\circ m)[u,v]
=D^2a_p[Dm(u),Dm(v)]+Da_p[D^2m(u,v)].
\tag{4.33; P}
\]

The second term must be kept. B102 Proposition 9, pp.305–309, supplies a fixed complex neighborhood and exponential localization of the first derivative. Cauchy's formula applied to that derivative gives an exponential bound in its first endpoint; symmetry of \(D^2m\) gives the same bound in the second endpoint. Taking the smaller bound yields decay in the maximum of the two endpoint distances, which is summable with any fixed polynomial moment after reducing the exponent.

For the current regular core, B99 (3.133), Theorem 3.12, pp.422–423, bounds the lift and its fine derivative, and (3.156)–(3.158), p.428, with Theorem 3.15, (3.187), p.432, bounds the constrained unit covariance. Their convolution has exponential decay. In physical units its curvature covariance and the quadratic vacuum response obey

\[
|\mathcal R_h(p,q)|\le CX^{-1}h^{-4}e^{-cd_T(p,q)/h},\qquad
\sup_p\sum_q a^4(1+d_T(p,q)/h)^5
\tfrac12|\operatorname{Tr}[\mathcal R_h(p,q)\mathcal R_h(q,p)]|
\le CX^{-2}h^{-4}.
\tag{4.34; P in the admitted current regular core}
\]

The proof of the powers is explicit: each curvature has dimension two, giving \(h^{-4}\) in the first kernel; squaring gives \(h^{-8}\), and the rooted fine sum with measure \(a^4\) contributes \(h^4\). Exponential convolution bounds its fifth moment uniformly, including the fine anchors. The additional term in (4.33) has the just-proved two-endpoint localization. The complete quadratic two-mark response therefore has a rooted fifth-moment envelope \(Ch^{-4}(X^{-2}+\epsilon_{\mathrm{bg}}^2X^{-1})\); the second term is the linear-vertex contribution. At the identity background it vanishes. This is a current-shell statement, not a bound for all previously integrated fields or an arbitrary large-field background.

#### 4.6.3 The interacting regular integral

The regular B109 (2.12)–(2.14) / B116 integral has the form
\(\int d\mu_C(B)\,\chi(B)e^{V(B)+sW_f(B)+tW_g(B)}\), with the Haar, Jacobian, constraint, Wilson and old source-free E terms retained in \(V\). Suppose the anchored marked vertices obey (2.7) throughout the common analytic background and decoupling domains, and retain strict Gaussian-domination and cluster margins. Add normalized auxiliary vertices within those margins. The proof of (4.19), followed by coefficient extraction, gives

\[
\|\mathcal K_{fg}\|_{\kappa'}\le C a_fa_g.
\tag{4.35; P under the displayed regular admission}
\]

Every contributing carrier contains both anchors. B116 (1.9)–(1.10) decouples the nonlinear maps as well as the covariance; (1.11)–(1.21) supplies the analytic domains and (1.23)–(1.25) the carrier Cauchy estimates. These facts specify which localized integral the argument applies to.

For a fresh scalar plaquette the holomorphic extension is exactly
\(a(P)=-\tfrac12\operatorname{tr}[(P-1)^2P^{-1}]\). On a current regular background \(|P_0-1|\le C\eta^2\epsilon_{\mathrm{bg}}\), the lifted fluctuation estimate and the minimizing-map Cauchy bound give, after subtracting the background value,
\(C\eta^4(g_B\epsilon_{\mathrm{bg}}|B|+g_B^2|B|^2)\). Summing the \(\eta^{-4}\) fine anchors in a unit block cancels \(\eta^4\). Thus

\[
a_f\le C\|f\|_\infty(g_B\epsilon_{\mathrm{bg}}+g_B^2).
\tag{4.36; P for fresh regular-bulk scalar marks}
\]

This uses the complex plaquette identity, not a real absolute-value formula used outside its domain.

Finally interpolate from the full regular potential to its Gaussian part and split each marked vertex into its complete quadratic Taylor part and its remainder. In the connected series, the difference contains either an interaction vertex, a marked remainder, or a cutoff-complement vertex. The same analytic coefficient estimate bounds it by
\(C[v a_fa_g+r_fa_g+a_fr_g+r_fr_g+e^{-cR^2}a_fa_g]\), where \(v\) is the potential norm, \(r_i\) the remainder norm and \(R\) the matched regular cutoff. For constant marks, the fixed small fluctuation domain gives \(a_i=O(X^{-1})\), \(r_i=O(\epsilon X^{-1})\), \(v=O(\epsilon)\); (4.30) removes the Gaussian field marginal. The fresh nonvacuum response is therefore \(O(\epsilon X^{-2})\). This estimate retains its stated regular-bulk scope. Extending its cutoff tail to (4.3), or replacing all incoming old jets by fresh plaquettes, would discard terms identified in §4.2.

## 4.7 A local discrete gauge proof of the dimension-four projection

This section proves a local statement on the **actual B109 analytic activity domain**. It is not an assertion that every marked coefficient has already been placed in that domain. Let \(G_X(U,J)\) be analytic, local to a filled carrier collar, termwise invariant under complex gauge transformations, and bounded there by \(a_X\). Write \(D=d_j(X)\), \(\theta=h_j/h_k\), \(\eta=L^{-k}\), \(\xi=L^{-j}\), so \(\eta=\theta\xi\). Assume the physical background on a contractible current-scale chart containing the collar has a logarithmic gauge \(U_\mu(x)=e^{i\eta H_\mu(x)}\) with bounded \(H,\nabla^\eta H\) and physical current. B102 Theorem 1, (9)–(10), p.279, supplies these hypotheses, and a finite-difference \(C^{1,\alpha}\) bound for each fixed \(0<\alpha<1\), on its admitted interior minimizing backgrounds.

#### 4.7.1 Killing the constant connection and the linear activity

First take \(\theta(1+D)\le c_0\), with \(c_0\) inside the fixed chart radius; the complementary case is treated by the endpoint/tail bounds below. Choose an anchor \(x_0\) with a plaquette margin and put \(r=x-x_0\). Use the gauge \(u(x)=\exp(i\sum_\nu r_\nu H_\nu(x_0))\). With \(b=\sum r_\nu H_\nu(x_0)\), the transformed positive link is

\[
U_\mu^u(x)=e^{ib(x)}e^{i\eta H_\mu(x)}
 e^{-i(b(x)+\eta H_\mu(x_0))}.
\tag{4.37; P}
\]

The matrix logarithm divided by \(i\eta\) is uniformly analytic in its arguments, including at \(\eta=0\): the product equals the identity at \(\eta=0\), so its convergent logarithm is divisible by \(\eta\). It vanishes at \(r=0\), \(H_\mu(x)=H_\mu(x_0)\). Finite differences of this analytic formula, on the fixed small chart, give \(\widetilde H_\mu(x_0)=0\), \(|\widetilde H(x)|\le C|r|\), \(|\nabla^\eta\widetilde H|\le C\). Thus in old-scale units \(U^u=e^{i\xi A}\),

\[
\|A\|_\infty\le C\theta^2(1+D),\quad
\|\nabla^\xi A\|_\infty\le C\theta^2,\quad
\|J_j(U^u)\|_\infty\le C\theta^3.
\tag{4.38; P/L}
\]

The current factor is the dimension-three scaling in B109 (3.12), p.272. That paper's current background is named \(U_{k+1}\), so its factor \((L^{j-1}\eta_{\mathrm{B109}})^3\) equals \(\theta^3\) after relabelling the current scale, with \(\eta_{\mathrm{B109}}=L\eta\). B109 (1.8), (3.11), and B102 (10) provide the bound on the current itself. It is not inferred from a coarse auxiliary-domain bound alone.

Consider the independent-variable path \((U_z,J_z)=(e^{i\xi zA},zJ_j(U^u))\). It stays in the admitted domain for \(|z|<c/[\theta^2(1+D)^2]\). To check this, use identity as the real reference configuration in B109 (1.11)–(1.14), p.262, and the elementary plaquette bound
\(\xi^{-2}\|d(e^{i\xi B})-1\|\le C(\|\nabla^\xi B\|+\|B\|^2)\). This bound follows by multiplying the four exponentials, whose constant linear contributions cancel. Conditions (i)–(iii) hold with smaller fixed constants by (4.38); B109 p.263 proves that these imply condition (iv). It is legitimate that \(J_z\ne J_j(U_z)\): the activity is analytic in the independent auxiliary variable.

The differential \(DG_X(1,0)\) vanishes. Each of its link and current components is a linear functional on the simple Lie algebra invariant under common constant conjugation. Such a functional is zero. Cauchy's estimate on the preceding disk, whose radius is \(R\), therefore gives \(|G_X(U,J_j(U))-G_X(1,0)|\le a_X\sum_{n\ge2}R^{-n}\). For \(R\ge2\) this is \(2a_XR^{-2}\); for \(R<2\) use the endpoint supremum bound. Hence

\[
|G_X(U,J_j(U))-G_X(1,0)|
\le C a_X\min\{1,\theta^4(1+D)^4\}.
\tag{4.39; P}
\]

If the carrier is too large for the chart, \(1+D\ge c/\theta\). With \(a_X=a e^{-\kappa D}\), the elementary bound
\(e^{-\kappa D}\mathbf1_{1+D\ge c/\theta}\le C_m\theta^m e^{-\kappa'D}\), \(\kappa'<\kappa\), follows by bounding \((1+D)^me^{-(\kappa-\kappa')D}\). It pays these carriers to any fixed power. Noncontractible holonomies have not been gauged away.

#### 4.7.2 Removing the symmetric first jet exactly on the lattice

Assume the stated Hölder bound on \(\nabla^\eta H\), with \(0<\alpha\le1\); use \(\alpha<1\) for the cited minimizing-background theorem. The analytic gauge formula preserves such a bound. Set \(M_{\mu\nu}=\nabla_\nu^\eta\widetilde H_\mu(x_0)\), \(S=(M+M^T)/2\). Telescoping along coordinate lattice paths gives
\(\widetilde H_\mu(x)=\sum_\nu M_{\mu\nu}r_\nu+R_\mu(x)\), with \(|R|\le C|r|^{1+\alpha}\), \(|\nabla R|\le C|r|^\alpha\). Define

\[
\phi(x)=\tfrac12\sum_{\mu,\nu}S_{\mu\nu}r_\mu r_\nu
-\tfrac\eta2\sum_\mu S_{\mu\mu}r_\mu,\qquad
\nabla_\mu^\eta\phi(x)=\sum_\nu S_{\mu\nu}r_\nu.
\tag{4.40; P}
\]

The last identity is an exact finite difference; omitting the linear correction would leave a lattice error at the anchor. Gauge again by \(e^{i\phi}\). On a cube of radius \(R_0=C\theta(1+D)\), the analytic matrix product gives
\(\widehat H_\mu=\widetilde H_\mu-\nabla_\mu\phi+\mathcal E_\mu\),
\(|\mathcal E|\le CR_0^3\), \(|\nabla\mathcal E|\le CR_0^2\). Indeed its remainder is bounded by
\(C[|\phi|(|\widetilde H|+|\nabla\phi|)+\eta(|\widetilde H|+|\nabla\phi|)^2]\); taking one finite difference has the claimed bound since \(\eta\le R_0\). This calculation uses no continuum interpolation of the lattice connection.

All outgoing links at \(x_0\) after the first gauge are exactly the identity. Thus its anchored plaquette is exactly
\(e^{i\eta^2M_{\nu\mu}}e^{-i\eta^2M_{\mu\nu}}\). The principal Hermitian curvature \(\mathcal F_{\mu\nu}=(i\eta^2)^{-1}\log U_{\mu\nu}(x_0)\) satisfies
\(\mathcal F_{\mu\nu}=M_{\nu\mu}-M_{\mu\nu}+O(\eta^2)\). Both subsequent gauges equal identity at the anchor. With \(z=(x-x_0)/\theta\), put \(A_\mu^{\mathcal F}(z)=-(\theta^2/2)\sum_\nu\mathcal F_{\mu\nu}z_\nu\). The estimates just obtained imply

\[
\|A-A^{\mathcal F}\|_{C^1_\xi}
\le C_\alpha\theta^{2+\alpha}(1+D)^{p_\alpha},\qquad
\|A\|_{C^1_\xi}+\|A^{\mathcal F}\|_{C^1_\xi}
\le C\theta^2(1+D)^p.
\tag{4.41; P}
\]

The exact-plaquette replacement costs \(C\theta^2\eta^2(1+D)\), which is absorbed since \(\eta\le\theta\). The fixed small \(C^1_\xi\)/current ball verified above permits uniform multivariable Cauchy estimates. Taylor expand \(G_X(e^{i\xi A},J)\) to second order. Its linear term vanishes. The mixed \(A,J\) term costs \(a_X\theta^5\operatorname{poly}(D)\), the \(J,J\) and cubic terms cost \(a_X\theta^6\operatorname{poly}(D)\), and replacing \(A\) by \(A^{\mathcal F}\) in the pure quadratic part costs \(a_X\theta^{4+\alpha}\operatorname{poly}(D)\). Constant color conjugation makes each quadratic color form a multiple of the invariant trace form. Consequently

\[
G_X(U,J_j(U))=G_X(1,0)
+\theta^4\sum_{\mu<\nu,\rho<\sigma}
 c_X^{\mu\nu\rho\sigma}\operatorname{Tr}
 (\mathcal F_{\mu\nu}\mathcal F_{\rho\sigma})+\mathcal R_X(U),
\quad
|c_X|\le Ca_X(1+D)^p,\quad
|\mathcal R_X|\le C_\alpha a_X\theta^{4+\alpha}(1+D)^{p_\alpha}.
\tag{4.42; P under the local hypotheses}
\]

If the small Taylor ball is not reached, its failure implies a lower bound on \(\theta\) in terms of a fixed inverse power of \(1+D\). The two endpoint bounds and the bound on the extracted quadratic form then imply (4.42) after enlarging that polynomial. Large or wrapping carriers can instead have projection zero and be paid by their exponential tail. Polynomial factors are absorbed by a fixed smaller carrier exponent.

The output is the full curvature-pair tensor space. A scalar projection is not imposed on each carrier. Covariant averaging of anchoring conventions over the finite lattice symmetry group preserves the bounds. In the convention of the question, the four-plaquette anti-Hermitian clover has \(\widehat F/\eta^2=i\mathcal F+O(\eta^\alpha)\) on this chart; hence its trace pairing has the corresponding minus sign relative to the Hermitian \(\operatorname{Tr}\mathcal F\mathcal F\). The same Hölder estimate makes this replacement an irrelevant error.

**Scope.** This proves the physical-background factor and local tensor projection for an already admitted analytic coefficient. It does not give the full complex-domain norm or localizer-difference bound of the projected remainder in B119's shrinking mixed-scale E/B domains. Those additional norms are exactly what the complete marked induction still requires. The independent-current path used here is not used to extend the physical Gaussian cancellation (4.30) off its stationary family.

## 4.8 Source freezing, contact subtractions and physical Gaussian null families

#### 4.8.1 Variable sources cost one physical length

Let \(\mathcal F_X(f,g;U,J)\) be bilinear in the two tests, depend on them only in a fixed collar of \(X\), and have the explicit analytic source-operator norm
\(\sup_{\mathcal D_X}\sup_{\|f\|_{\infty,X^+},\|g\|_{\infty,X^+}\le1}|\mathcal F_X(f,g)|\le a_j e^{-\kappa D}\).
This is an input norm to verify, not a consequence of the source-free bound. The collar is within distance \(Ch_j(1+D)\) of a chosen anchor \(z_X\). Bilinearity gives the exact freezing identity

\[
\mathcal F_X(f,g)-f(z_X)g(z_X)\mathcal F_X(1,1)
=\mathcal F_X(f-f(z_X),g)
+f(z_X)\mathcal F_X(1,g-g(z_X)).
\tag{4.43; P}
\]

The sup norm of either source difference is bounded by the collar diameter times its gradient. Apply (4.39) to the vacuum-subtracted function in (4.43). After a small carrier-exponent loss the result is bounded by
\(Ca_j e^{-\kappa'D}h_j\theta^4
(\|\nabla f\|_\infty\|g\|_\infty+\|f\|_\infty\|\nabla g\|_\infty)\).
There are \(O(\theta^{-4})\) old anchors per current block. Their sum leaves \(Ca_jh_j\) times the source-gradient norm. Since \(h_j/\ell_0=(h_k/\ell_0)\theta\le\theta\), this is a genuine extra factor \(L^{-(k-j)}\). The field Hölder remainder in (4.42) separately leaves \(L^{-\alpha(k-j)}\). The two gains have different origins. On the actual shrinking domain the field-factor estimate also carries \(\rho_j^{-2}\), as in §4.9. The vacuum source Taylor estimate below has no such field-Cauchy loss.

#### 4.8.2 Contact subtraction directly in the source-operator norm

At the identity set \(B_X(f,g)=\mathcal F_X(f,g;1,0)\). On a lifted source chart define

\[
\mathcal P_{4,X}B_X(f,g)
=\sum_{|\beta|+|\gamma|\le4}
\frac{\partial^\beta f(z_X)\partial^\gamma g(z_X)}
{\beta!\gamma!}
B_X((\,\cdot-z_X)^\beta,(\,\cdot-z_X)^\gamma).
\tag{4.44; P: definition}
\]

Only values of the monomials on the source collar are used. This expression is a distribution supported on the two-source diagonal: both source jets are evaluated at the same point. It may be symmetrized in the tests and in the finite reflection/translation-covariant anchor conventions.

Here is a proof of its remainder that does not infer an absolute fine-grid kernel bound from an operator norm. Put
\(f_t(x)=f(z_X+t(x-z_X))\), define \(g_t\) likewise, and apply one-variable Taylor's theorem through degree four to \(b(t)=B_X(f_t,g_t)\), \(0\le t\le1\). Its Taylor polynomial is (4.44). Every term of \(b^{(5)}\) has five total displacement factors and derivatives of total order five distributed between the two functions. The stated bilinear norm controls these functions separately. Therefore

\[
|B_X(f,g)-\mathcal P_{4,X}B_X(f,g)|
\le Ca_j e^{-\kappa'D}(h_j/\ell_0)^5
 \|f\|_{C^5,\ell_0}\|g\|_{C^5,\ell_0}.
\tag{4.45; P under the explicit local source norm}
\]

In a physical volume \(T^4=N_T\ell_0^4\), the old-anchor count is \(O(N_T(\ell_0/h_j)^4)\). Carrier summation leaves \(Ca_jN_T(h_j/\ell_0)\). If \(\sup_j a_j\le A\), its ultraviolet sum is bounded by \(CAN_T/(1-L^{-1})\). Coefficients of the Taylor polynomial may diverge; they are precisely the subtractions. For a compactly supported test one uses its active anchors rather than the total-volume count. Large carriers outside the source chart are paid by the exponential tail, using a smaller fixed exponent.

The Gaussian bound (4.34) gives a more explicit kernel version. For
\(B_h(f,g)=\sum_{p,q}a^8 f(x_p)g(x_q)K_h(p,q)\), take a fixed smooth cutoff \(\chi(r)\), equal to one near zero and supported in an injective ball of radius \(\ell_0/8\), and put
\(c_{\alpha,h}(p)=\sum_q a^4\chi(r)r^\alpha K_h(p,q)/\alpha!\), \(r=x_q-x_p\), \(|\alpha|\le4\).
The diagonal term is \(\sum_p a^4f(x_p)\sum_\alpha c_{\alpha,h}(p)\partial^\alpha g(x_p)\). Taylor's fifth-order remainder and (4.34) give

\[
|B_h(f,g)-\mathcal C_h(f,g)|
\le C\ell_0^{-5} X^{-2}h
 \|f\|_{L^1_a}\|g\|_{C^5,\ell_0},
\qquad \sum_{j=0}^K h_j\le \ell_0/(1-L^{-1}).
\tag{4.46; P in the checked Gaussian vacuum sector}
\]

Indeed \(\ell_0^{-5}|r|^5\) multiplies the rooted kernel; its sum is \(CX^{-2}h\ell_0^{-5}\), as displayed. Equivalently one may write the coefficient as \(C_{\ell_0}X^{-2}h\), with \(\ell_0\) fixed. On the complement of \(\chi=1\), \(|r|\) is bounded below by a fixed physical length, so the same global fifth-power bound controls the omitted polynomial. Symmetrizing preserves the estimate. This proves (3.3).

#### 4.8.3 A summed Gaussian cancellation must be used at its generation scale

Let \(G_X(B)\) be the constant-source Gaussian local family in coarse coordinates at the scale where it was generated. Suppose its derivatives are absolutely summable on a common chart and \(\sum_XG_X(B)\) is constant there. Then for \(n\ge1\),

\[
\sum_X w(z_X)D_{y_1}\cdots D_{y_n}G_X
=\sum_X[w(z_X)-w(y_1)]D_{y_1}\cdots D_{y_n}G_X.
\tag{4.47; P}
\]

Differentiate the sum identity, multiply it by \(w(y_1)\), and subtract to prove the formula. If the rooted derivative kernels have a uniformly summable first distance moment between \(z_X\) and \(y_1\), measured in generation-scale units, the right side has the extra bound \(Ch_j\|\nabla w\|_\infty\) times that moment. Take \(w=fg\) to combine it with (4.43).

There are two essential hypotheses. Derivatives with respect to much later coarse variables may spread over the later scale and do not give \(h_j\). The null identity holds on the physical constrained-minimizer family; it need not hold for independent auxiliary \(U,J\). B109 (3.3), p.270, and (3.38)–(3.39), p.278, give the physical nesting identity, with their stated gauges and domains. CMP98 (97), in Bałaban, CMP 98 (1985), is the averaging-convention gauge bridge used there. The differentiated generation-scale moment ledger for the complete Gaussian family, including its localizers, is still to be verified. Equation (4.47) records what that verification will buy.

#### 4.8.4 Why a fixed number of source derivatives can suffice at every order

Define the equivalent finite-jet norm
\(\|f\|_{5,\mathrm{alg}}=\sum_{|\alpha|\le5}\ell_0^{|\alpha|}\|\partial^\alpha f\|_\infty/\alpha!\).
Leibniz's rule gives exactly
\(\|fg\|_{5,\mathrm{alg}}\le\|f\|_{5,\mathrm{alg}}\|g\|_{5,\mathrm{alg}}\), and
\(\|f\|_{5,\mathrm{alg}}\le\|f\|_{C^5,\ell_0}\le5!\|f\|_{5,\mathrm{alg}}\).
Thus

\[
\left\|\prod_{i=1}^r f_i\right\|_{C^5,\ell_0}
\le5!\prod_{i=1}^r\|f_i\|_{C^5,\ell_0}.
\tag{4.48; P}
\]

An \(r\)-linear admitted local source activity has the same contact proof: dilate all \(r\) sources together and distribute five derivatives among them. The factorially weighted derivative norm bounds that sum, so the remainder still costs only five total displacement powers.

The following application is conditional on an actual gauge-covariant local collision forest with the usual dimension-four power counting. Colliding \(r\) dimension-four insertions and integrating their \(4(r-1)\) relative coordinates leaves output degree four. A local term with \(q\) source derivatives and field dimension \(\Delta\) must satisfy \(q+\Delta\le4\). In the analytic gauge-invariant SU(N) field class there is no nonidentity polynomial of dimension one, two or three; the dimension-four outputs are curvature-pair tensors. Thus internal field-output contractions multiply source tests without derivatives, while terminal identity terms require Taylor degree at most four. Equation (4.48) and the disjoint mark sets of terminal forest vertices cost at most an exponential in \(r\), rather than an increasing derivative order. This removes a potential regularity obstacle. It does not prove the forest coefficients, their gauge identities, or their fixed factorial growth.

## 4.9 Scale summation, shrinking radii and a precise numerical closure

#### 4.9.1 Numerical consequences of N2-F, without extra differentiability

Put \(b=b_0\log L\). Choose a sufficiently large fixed \(x_*\) so that \(C_r/x_*\le b/2\), \(C_r/x_*^2\le1/2\), and all required small-coupling ceilings are met. This choice is compatible with the existential aim. To justify that it controls the whole trajectory, let \(B=C_r\gamma^2\), \(X_c=\max(\gamma^{-2},2C_r/b)\), and choose \(X_1>\max(x_*,X_c+B)\). The set \(\{x<X_1\}\) is forward invariant: above \(X_c\) the trajectory decreases, and below \(X_c\) its next value is below \(X_c+B\). Thus a terminal \(x_K\ge X_1\) forces every earlier value above \(X_1\). In that range,

\[
b_-=b/2\le x_k-x_{k+1}\le b_+=3b/2,\qquad
x_j\ge x_K+b_-(K-j).
\tag{4.49; P from N2-F}
\]

Consequently \(\sum_jg_j^p(1+|\log g_j|)^q\) is uniformly finite for \(p>2\) and fixed \(q\): compare the decreasing tail with the integral of \(x^{-p/2}(1+\log x)^q\). A useful borderline version, for \(d>1\) and \(x_K>1\), is

\[
\sum_{j=0}^K\frac1{x_j(\log x_j)^d}
\le\frac1{x_K(\log x_K)^d}
+\frac{(\log x_K)^{1-d}}{b_-(d-1)}.
\tag{4.50; P}
\]

Apply the integral comparison on each interval \([x_{j+1},x_j]\) to prove it.

N2-F also gives an actual first-derivative numerical statement. For \(F_k(x)=x-b+r_k(x)\), differentiation of a finite composition along an admitted trajectory gives
\(D(F_{j-1}\circ\cdots\circ F_i)=\prod_{l=i}^{j-1}(1+r_l'(x_l))\).
Since \(|\log(1+t)|\le2|t|\) for \(|t|\le1/2\), and
\(\sum_{l=i}^{j-1}x_l^{-2}\le1/(b_-x_j)\),

\[
e^{-2C_r/(b_-x_j)}
\le D(F_{j-1}\circ\cdots\circ F_i)
\le e^{2C_r/(b_-x_j)}.
\tag{4.51; P}
\]

Identifying this numerical derivative with the Wilson marginal of the complete frozen-map marked theory requires a proof of that identification. The numerical interface does not describe derivatives of all irrelevant and boundary activities. It is only \(C^1\), so no second derivative of \(r_k\) is assumed.

#### 4.9.2 The analytic-radius cost must be retained

The fixed-domain lemma in §4.7 is not a license to use a fixed Cauchy radius in B119. Equation (2.28), p.259, gives radii of the form
\(\alpha_{i,j}=g_j C_i(\log g_j^{-2})^{q_i}\), \(q_i>1\). A safe joint \(C^1(A)\)/current radius is
\(\rho_j=c\min(\alpha_{0,j},\alpha_{1,j})\).
With this radius, the proof of (4.39) gives
\(Ca_j\min(1,\theta^4\operatorname{poly}(D)/\rho_j^2)\).
The quadratic projection costs \(\rho_j^{-2}\), and the cubic remainder costs \(\rho_j^{-3}\). These follow by rescaling the analytic ball in the Cauchy proof; they cannot be omitted.

For the fresh second regular response \(a_{j,2}\le C\epsilon g_j^4\), and a fixed normalized incoming mark, the quadratic cost is bounded by

\[
a_{j,2}\rho_j^{-2}
\le \frac{C\epsilon}{X_j(\log X_j)^{2q}},
\qquad q=\min(q_0,q_1)>1,
\tag{4.52; P for the stated fresh-sector bounds}
\]

after the literal coefficient dictionary is matched. This is summable by (4.50). The analogous crude first-mark estimate \(a_{j,1}\le C\epsilon g_j^2\) would give only \(C\epsilon/(\log X_j)^{2q}\), which is not summable over an arbitrarily long ultraviolet trajectory. The first response therefore needs its sharper structural estimate or the rigorously identified flow derivative (4.51). Equation (4.52) does not by itself control transported first-mark normalization factors.

A fixed number of radius losses does not destroy geometric memory. For \(\rho_j\asymp X_j^{-1/2}(\log X_j)^q\), a matched trajectory with the two drift bounds gives, for \(j\le k\),

\[
(\rho_k/\rho_j)^p
\le C\left(1+\frac{b_+(k-j)}{X_k}\right)^{p/2},
\qquad
L^{-\alpha(k-j)}(\rho_k/\rho_j)^p
\le C_{\alpha',p}L^{-\alpha'(k-j)}
\quad(0<\alpha'<\alpha).
\tag{4.53; P for each fixed p}
\]

The logarithmic ratio is at most one after choosing the fixed lower range sufficiently large; the remaining polynomial is absorbed by the extra exponential decay. Thus a norm weighted by the actual current radius is a viable numerical choice. Whether all the required marked localizer estimates obey that norm is still an analytic question.

#### 4.9.3 The memory inequality that would close the constant scalar sector

B109 (0.28)–(0.30), p.258, gives the actual old-scale factor \(\theta^{4+\alpha}\); anchor counting leaves \(q^{k-j}\), \(q=L^{-\alpha}\). The discussion after (3.54), p.280, supplies a small factor \(C\alpha_2^{-1}\epsilon_1\) for the old-activity fluctuation difference. These do not assert an arbitrary one-step contraction.

Here is a fully specified numerical implication. Let \(A_{j,1},A_{j,2}\ge0\) be consistently normalized nonvacuum carrier amplitudes, \(S_{k,m}=\sum_{1\le j\le k}q^{k-j}A_{j,m}\), \(A_{0,m}=0\). Let \(u_k,v_k\) be the constant scalar first and second Wilson responses, \(u_0\ne0,v_0=0\). Suppose one has proved

\[
\begin{aligned}
A_{k+1,1}&\le C\epsilon(|u_k|/X_k+S_{k,1}),\\
A_{k+1,2}&\le C\{\epsilon(|v_k|/X_k+|u_k|^2/X_k^2+S_{k,2})
+\epsilon |u_k|S_{k,1}/X_k+\epsilon^2S_{k,1}^2\},\\
|u_{k+1}-u_k|&\le P A_{k+1,1},\qquad
|v_{k+1}-v_k|\le P A_{k+1,2},
\qquad X_k-X_{k+1}\ge b_->0,\quad X_k\ge X_*>0.
\end{aligned}
\tag{4.54; C: required analytic-to-numerical system}
\]

The fresh terms have the regular-bulk origin in §4.6; the constant-family projection is B109 (1.22), p.264, (5.10), p.293, and (5.42), p.297. That projection uses the translation-invariant kernel of (5.8). Its second moment is bounded by its exponential norm. In shrinking domains that bound must contain the radius factors, or those factors must already be included in the definition of \(A\) and the verified inequalities. This is why \(P\) in (4.54) is an explicit hypothesis, not an automatic fixed constant imported from the fixed-radius calculation.

For sufficiently small fixed \(\epsilon\), system (4.54) implies

\[
A_{k+1,1}\le H_1\epsilon |u_k|/X_k,\qquad
A_{k+1,2}\le H_2\epsilon |u_k|^2/X_k^2,\qquad
|v_k|\le H_v\epsilon |u_k|^2/X_k.
\tag{4.55; P under (4.54)}
\]

**Proof.** Take \(C\ge1\), \(H_1=H_2=2C\), \(H_v=2PH_2/b_-\), and
\(\delta=2PH_1\epsilon/b_-\le1/4\).
Choose \(\epsilon\) so that \(PH_1\epsilon/X_*\le1/2\),
\(H_1\epsilon/(1-q)\le1\), and
\(H_v\epsilon+(H_1+H_2)\epsilon/(1-q)+H_1^2\epsilon^3/(1-q)^2\le1\).
Assume the estimates through the preceding step. The first update preserves the sign of \(u\) and gives
\(|\log|u_{k+1}/u_k||\le2PH_1\epsilon/X_k\).
Integral comparison gives
\(\sum_{l=i}^{j-1}X_l^{-1}\le b_-^{-1}\log(X_i/X_j)\).
Hence both \(|u_i/u_j|\) and its reciprocal are at most \((X_i/X_j)^\delta\).

For \(j\le k\), divide the old first bound by \(|u_k|/X_k\); the remaining factor is
\((X_{j-1}/X_k)^{\delta-1}\le1\).
The second bound similarly uses \(2\delta-2<0\). Therefore
\(S_{k,1}\le H_1\epsilon |u_k|/[X_k(1-q)]\) and
\(S_{k,2}\le H_2\epsilon |u_k|^2/[X_k^2(1-q)]\).
The update for \(v\) gives
\(|v_k|/|u_k|^2\le PH_2\epsilon X_k^{-2\delta}\sum_{j<k}X_j^{2\delta-2}
\le PH_2\epsilon/[b_-(1-2\delta)X_k]\).
This is the stated \(H_v\) bound. Substitution into the two amplitude inequalities leaves respectively brackets
\(1+H_1\epsilon/(1-q)\) and
\(1+H_v\epsilon+(H_1+H_2)\epsilon/(1-q)+H_1^2\epsilon^3/(1-q)^2\), each at most two. This closes the induction from the zero initial memories. The constants are independent of its length.

This proof settles the numerical system, not its full Yang–Mills premises. The boundary, cutoff-surface, R-localizer and weighted-null-family deficits must appear as additional terms until bounded. Dropping them, or dropping the radius losses, would be precisely the missing proof.

#### 4.9.4 A triangular system compatible with the borderline radius estimate

There is a second useful numerical target, closer to (4.52). Suppose the complete scalar transport can be shown to have
\(u_{k+1}=a_ku_k\),
\(v_{k+1}=a_kv_k+b_ku_k^2\), \(v_0=0\), with
\(|a_k-1|\le C_r/x_k^2\le1/2\) and
\(|b_k|\le B\epsilon/[x_k(\log x_k)^d]\), \(d>1\).
This shared linear coefficient is an additional structural estimate to prove; it is not asserted by N2-F for the marked activities.

Let \(w_k=v_k/u_k^2\). Its exact recursion is
\(w_{k+1}=w_k/a_k+b_k/a_k^2\).
Iteration, the derivative-product estimate (4.51), and \(a_k^{-1}\le2\) give

\[
\frac{|v_K|}{|u_K|^2}
\le 2C_*\sum_{k<K}|b_k|
\le\frac{2C_*B\epsilon}{b_-(d-1)}
(\log x_K)^{1-d},
\qquad
C_*=\exp\{2C_r/(b_-x_*)\}.
\tag{4.55a; P under the stated triangular transport}
\]

The last sum excludes the terminal index and is bounded by the corresponding integral on the decreasing trajectory. Thus the actual borderline radius loss can still fit a uniform second-response bound if the first scalar transport is identified sharply and the complete forcing has the stated rate. This provides a concrete alternative to demanding the stronger fixed-radius rates in (4.54).

## 4.10 From local normalized insertions to a reflection-positive OS hierarchy

#### 4.10.1 The terminal normalization estimate

Let \(D\) contain the active source cells and their fixed collars. Integrate its fine, coarse and history variables conditionally on exterior data \(v\). Let \(W_0(v)\ge0\) be the unmarked mass and \(W_I(v)\) the complete raw renormalized jet; counterterm coefficients in \(W_I\) may have signs. A sufficient local estimate is

\[
W_0(v)\ge c_D w_D(v),\qquad
|W_I(v)|\le C_{I,D}w_D(v),\qquad c_D>0,
\tag{4.56; C: common-exterior comparison}
\]

with the same nonnegative reference \(w_D\), uniformly in cutoff and total volume. Integrating against the positive exterior measure gives \(|Z_I/Z_0|\le C_{I,D}/c_D\). This proves the normalization implication without a total-volume factor.

For affine payloads, a useful sufficient upper estimate is
\(\int K_D e^{sV_D}\le C_Dw_D\), \(|F_i|\le a_iV_D\). With the lower estimate it gives
\(|Z_I/Z_0|\le(C_D/c_D)m!s^{-m}\prod_i a_i\).
For nonlinear renormalized jets one must bound the complete numerator instead. Another sufficient alternative is to finish all old integrations first and prove that the complete terminal log jets are bounded functions of retained coarse fields: their normalized expectations and covariances are then bounded under any terminal probability measure.

A global pressure estimate cannot replace (4.56). For example, take \(N\) independent spins, density \(\rho_N=e^{-2sN}\), \(V=N\), and a local cutoff-dependent mark \(F_N=N\epsilon_1\). Then \(\int\rho_Ne^{sV}=e^{-sN}\), whereas its normalized second moment is \(N^2\). The density has extensive upper and lower bounds. This proves that those bounds and a raw history reserve alone do not imply normalized local insertion bounds.

For a useful hierarchy estimate, require (4.56) for a union of \(q\) active cells with loss at most \(C_0e^{C_1q}\), independent of their separation and total torus size. For \(m\) supported arguments, \(q\le C m\). If the complete raw jet bounds have fixed factorial order \(p\), this yields
\(|S_m(f_1,\ldots,f_m)|\le C^m(m!)^p\prod_i\|f_i\|_{C^5,\ell_0}\)
for such arguments. A fixed smooth partition of unity with bounded overlap extends it to Schwartz tests: for \(M>4\),
\(\sum_c\|\chi_cf\|_{C^5,\ell_0}\le C_M p_{M,5}(f)\), where
\(p_{M,5}(f)=\max_{|\alpha|\le5}\sup_x(1+|x|)^M|\partial^\alpha f(x)|\).
Multilinearity and absolute summation prove the same product bound with \(p_{M,5}\).
No such complete survivor comparison has been proved above.

#### 4.10.2 Product bounds imply the corrected order growth

Suppose the full moment hierarchy has a uniform bound
\(|S_m(f_1,\ldots,f_m)|\le C^m(m!)^p\prod_i p_{M,5}(f_i)\).
If it is connected functions that obey that bound, Proposition 4.13.1 applies to (2.8): for every fixed \(p\ge1\), full moments obey the same factorial power \(p\), with only the exponential constant enlarged. Thus full/connected conversion does not consume an additional factorial power.

Let \(h_\nu\) be the four-dimensional Hermite basis and \(H_{\mathrm{osc}}=1-\Delta+|x|^2\), with eigenvalues \(\lambda_\nu\asymp1+|\nu|\). Fixed weighted Sobolev bounds, or the Hermite raising/lowering identities followed by Sobolev's inequality, give \(p_{M,5}(h_\nu)\le C\lambda_\nu^d\) for a fixed \(d\). Choose a fixed integer \(s>d+4\). For a Schwartz \(F\) in \(4m\) variables its Hermite coefficient is bounded by
\(\|(\bigotimes_{i=1}^mH_{\mathrm{osc},i}^s)F\|_2\prod_i\lambda_{\nu_i}^{-s}\).
The sum over the \(\nu_i\) factorizes, since \(\sum_\nu\lambda_\nu^{d-s}<\infty\). Hence

\[
|S_m(F)|\le C_1^m(m!)^p
 \|(\bigotimes_{i=1}^mH_{\mathrm{osc},i}^s)F\|_2
\le C_2^m(m!)^p\,\nu_{qm}(F),\qquad q=2s+3.
\tag{4.57; P under the product estimate}
\]

For the last inequality, each one-particle power has a fixed finite list of polynomial differential terms of weight/derivative order at most \(2s\). Their tensor product has coefficients bounded by \(C_s^m\) and total order at most \(2sm\). The remaining radial weight is integrable in \(4m\) dimensions: \(\int(1+|x|^2)^{-(2m+1)}dx=\pi^{2m}/(2m)!\). This bounds its \(L^2\) cost by an exponential, without adding a factorial power. Hermite expansion also proves the unique continuous multilinear-to-distribution extension. This argument requires estimates for all Schwartz product tests, or a justified extension to them. Bounds only on separated supports do not automatically supply it.

#### 4.10.3 A local renormalization prescription can preserve reflection positivity

Here is a precise sufficient structural lemma. Suppose the bare normalized measure is reflection positive for its gauge-invariant positive-time observables. Let the renormalization at each finite order be described by a real source map \(\mathscr R(j)\), taking values in the finite observable family, and an identity counterterm \(\mathcal C(j)\), both with zero constant term. Assume they are reflection covariant and additive between source families with disjoint separated supports:
\(\mathscr R(j_++j_-)=\mathscr R(j_+)+\mathscr R(j_-)\),
\(\mathcal C(j_++j_-)=\mathcal C(j_+)+\mathcal C(j_-)\).
An exactly local polynomial in source jets has this property.

Define positive-time renormalized polynomial representatives by taking coefficients of
\(\exp\{\mathcal O(\mathscr R(j_+))-\mathcal C(j_+)\}\).
For a finite list \(F_i\) of such source polynomials, denote the representatives by \(T F_i\). Support locality puts them in the positive-time algebra. Additivity and reflection covariance give

\[
G^{\mathrm{ren}}(F_i,F_j)
=\mu\bigl(\Theta(TF_i)\,TF_j\bigr),\qquad
\sum_{i,j}\overline c_i c_jG^{\mathrm{ren}}(F_i,F_j)
=\mu\!\left(\Theta\!\sum_i c_iTF_i\;\sum_jc_jTF_j\right)\ge0.
\tag{4.58; P under the structural hypotheses}
\]

This is simply bare reflection positivity applied to the transformed polynomial. It works for finite formal jets and includes local field-valued collision counterterms through nonlinear \(\mathscr R\). No positive finite-source measure after arbitrary subtraction is assumed. A counterterm with a merely bounded extensive nonlocal remainder need not have the required additivity; dropping that remainder in a Gram form is not justified.

For Wilson gauge theory the positive transfer-matrix construction is a primary route to bare positivity: Lüscher, *Construction of a selfadjoint, strictly positive transfer matrix for Euclidean lattice gauge theories*, Proposition 1 and §II, DESY 76/54 / CMP 54 (1977), 283–292. Its positive character kernel and the spatial gauge projection give the pure-gauge case used here. On a finite periodic time torus the positivity statement concerns the admissible reflected supports; a thermal trace must not be identified with an infinite-time vacuum expectation. For clover components the finite link slab must stay in its assigned half-space, and the exact tensor reflection law must be respected. The lemma then passes to the limit. The actual consistent local prescription for all marks remains to be constructed.

#### 4.10.4 Compactness and reconstruction

Assume H0–H2. For each \(m\) and finite tensor-index list, choose a countable dense family of Schwartz tests. Equation (2.9), or (4.57), gives a uniform bound on every evaluation. A diagonal subsequence converges on all these countably many evaluations. The same seminorm bound extends the limit uniquely and gives convergence on every test: approximate it in the controlling seminorm, bound both errors uniformly, and then pass to the subsequence limit on the approximant. This proves distributional compactness for the entire compatible hierarchy.

The full moment/connected identities pass to the limit on product tests by finite algebra. Every finite reflected Gram form passes by distributional convergence; nonnegative forms have nonnegative limits. The same applies to reality and permutation symmetry. For any translation or rotation, a defect estimate tending to zero yields the corresponding continuum transformation law. Hypercubic symmetry alone supplies only a finite subgroup and is insufficient for the rotation step.

The corrected reconstruction is the literature input: Osterwalder–Schrader, CMP 42 (1975), 281–305, §IV.1, Theorem \(E'\to R'\), with the subset-of-axioms qualification on p.283 and the reconstruction discussion in §IV.2. The linearly growing distribution order and fixed factorial growth are precisely why (4.57) is included. With E0′, E1, E2 and E3, but without imposing the clustering/unique-vacuum clause, it supplies the relativistic field theory needed before phase decomposition. The finite tensor family uses the stated finite-component extension. We use this theorem, not the invalid uncorrected OS I temperedness argument.

## 4.11 Energy bounds, the phase-decomposition domain and phasewise nontriviality

#### 4.11.1 A concrete Euclidean energy criterion

Assume reconstruction of the full hierarchy. On its positive-time polynomial algebra write
\(G(F,G)=S(\Theta F\,G)\), \([F]\) for the OS vector, and
\([\tau_tF]=e^{-tH}[F]\), \(H\ge0\). For a spatial Schwartz test \(h\), define the separated insertion
\(I^h_{s,t}F=\mathcal O(s,h)\tau_{s+t}F\), \(s,t>0\).
It can be defined by time mollifiers with supports kept apart. The prescribed limiting polynomial matrix elements must exist and agree with the analytic continuation of this same hierarchy. Uniform operator bounds alone would not select a unique mollifier limit.

A sufficient new Yang–Mills estimate is

\[
G(I^h_{s,t}F,I^h_{s,t}F)
\le C^2\wp(h)^2s^{-2u}t^{-2v}G(F,F),
\qquad 0<s,t\le1,
\tag{4.59; O for Yang–Mills}
\]

for fixed \(u,v,C,\wp\), and **every** polynomial vector \(F\), independently of its degree and coefficients. This is a matrix domination of all finite Gram matrices. The two distinguished insertions in the reflected norm are separated by \(2s\). Temporal clover terms must be treated as their actual link-slab insertions, not automatically as multiplication on a single spatial time slice.

**Consequence (P under (4.59) and the stated insertion limits).** The map descends to OS null equivalence classes and defines bounded \(B^h_{s,t}\), with
\(\|B^h_{s,t}\|\le C\wp(h)s^{-u}t^{-v}\).
Translation of the inserted polynomial gives
\(B^h_{s+a,t+b}=e^{-aH}B^h_{s,t}e^{-bH}\).
For the spectral bands \(P_n=\mathbf1_{[n,n+1)}(H)\), set

\[
A_{ij}(h)=e^{sH}P_iB^h_{s,t}P_je^{tH},\qquad
\|A_{ij}(h)\|\le e^2C\wp(h)(1+i)^u(1+j)^v.
\tag{4.60; P}
\]

The compatibility makes \(A_{ij}\) independent of \(s,t\); compare any two pairs through a smaller common pair. Taking \(s=(1+i)^{-1}\), \(t=(1+j)^{-1}\) proves the bound. Energy bands may have infinite rank.

For a spacetime Schwartz test \(f\), smear the form in physical time:
\(\Phi_{ij}(f)=\int_{\mathbb R}e^{irH}A_{ij}(f(r,\cdot))e^{-irH}dr\).
On the two bands, split \(H=i+(H-i)\) and \(H=j+(H-j)\); the residual generators have norm at most one. Integrating by parts \(N\) times in the scalar phase \(e^{ir(i-j)}\) gives

\[
\|\Phi_{ij}(f)\|
\le C_N C\,\mathfrak p_N(f)(1+i)^u(1+j)^v
 (1+|i-j|)^{-N},
\qquad
\mathfrak p_N(f)=\sum_{l=0}^N\int_{\mathbb R}
 \wp(\partial_r^l f(r,\cdot))dr.
\tag{4.61; P}
\]

For \(i=j\), use the integral without parts. All differentiated residual exponentials are bounded by fixed powers of two. This proves the bound directly.

Put \(p=u+v\). The block norms of \(\Phi(f)(1+H)^{-p}\) are bounded by
\(C_N C\mathfrak p_N(f)(1+|i-j|)^{-(N-u)}\), since
\(1+i\le(1+j)(1+|i-j|)\).
For \(N>u+1\) its row and column sums are finite. The operator-valued Schur test on \(\bigoplus_nP_n\mathcal H\) therefore proves

\[
\|\Phi(f)(1+H)^{-p}\|\le C_f,\qquad
\|(1+H)^m\Phi(f)(1+H)^{-(p+m)}\|\le C_{f,m}
\quad(m\ge0).
\tag{4.62; P}
\]

For the second estimate use \(N>u+m+1\). Reality gives the adjoint relation and closability. The weighted estimates give an invariant common smooth-energy domain directly. If an integer exponent is desired, enlarge \(p\). The identification with the reconstructed \(\phi(f)\) follows from the prescribed separated Euclidean polynomial matrix elements and uniqueness of their analytic continuation, not from equality of a vacuum two-point function alone.

This criterion is stronger than individual correlation bounds for a reason. The constant random Gaussian field has factorially bounded, Euclidean-invariant positive moments and \(H=0\), but its multiplication operator is unbounded. Thus ordinary distribution bounds alone cannot imply (4.62).

#### 4.11.2 The closure required by Driessler–Summers

The primary domain is important. In Driessler–Summers, *Decomposition of relativistic quantum field theories into pure phases*, HPA 59 (1986), 331–348, p.333, \(D_1\) allows arbitrary Schwartz tests in all variables of a polynomial vector, not just products of separately smeared tests. Definition 2.1, p.334, requires the closure of \(\phi(f)\) **on \(D_1\)** to satisfy a generalized H-bound.

Here is the needed domain proof. Tempered Wightman continuity makes
\(F_n\mapsto\phi^{\otimes n}(F_n)\Omega\) Hilbert-space continuous. Joint time translation is smooth in Schwartz topology, so \(D_1\subset\bigcap_m\operatorname{Dom}H^m\). If \(G\in C_c^\infty(\mathbb R)\), its inverse Fourier transform is Schwartz; joint time convolution of \(F_n\) therefore gives \(G(H)D_1\subset D_1\).

Let \(\psi\in\operatorname{Dom}(1+H)^p\). Smooth compact energy cutoffs \(G_R(H)\psi\) converge to \(\psi\) in that graph norm. Approximate \(\psi\) in Hilbert norm by vectors \(d_l\in D_1\). For fixed \(R\), \(G_R(H)d_l\) converges to \(G_R(H)\psi\) in graph norm because \((1+H)^pG_R(H)\) is bounded. A diagonal choice proves that \(D_1\) is a graph core for \((1+H)^p\). Equation (4.62) then makes \(\phi(f)d_l\) converge whenever \(d_l\) approaches such a \(\psi\) in energy graph norm. Hence

\[
\operatorname{Dom}(1+H)^p
\subset\operatorname{Dom}\overline{\phi(f)|_{D_1}},\qquad
\overline{\phi(f)|_{D_1}}(1+H)^{-(p+1)}
\text{ is bounded}.
\tag{4.63; P}
\]

Thus \(F_f(E)=(1+E)^{-(p+1)}\) is positive and decreasing and supplies exactly Definition 2.1, in particular on its compact-Fourier-support test class.

Theorem 2.3, pp.335–336, of that paper now supplies pure-phase decomposition for the reconstructed Wightman theory without initial vacuum uniqueness; its finite-component extension and energy-bound transfer are part of the stated result. The other hypotheses are accounted for: the full hierarchy gives Wightman locality, covariance, spectrum and a cyclic invariant vector; countable Schwartz density gives separability; (4.63) supplies the required closure bound. The phase fields inherit the energy estimates. This is the literature import used in Theorem 3.5, not an assumption that every extremal polynomial-algebra state automatically clusters.

#### 4.11.3 A sufficient criterion for the specified ultraviolet law in a phase

Phase decomposition alone does not transfer a connected coefficient of a mixed state to a component with the same value. For example, a non-Gaussian constant random field can have a nonzero mixed-state connected three-point function while each pure component is a deterministic constant field.

A concrete stronger sufficient estimate is available. In the decomposed theory let \(P_{\mathrm{vac}}\) be the direct integral of the one-dimensional phase vacuum projections. For physical spacetime-scaled tests \(f_i^\epsilon\), let
\(M_I(\epsilon)=P_{\mathrm{vac}}\prod_{i\in I}\phi(f_i^\epsilon)P_{\mathrm{vac}}\), with the specified ordering. The weighted energy estimates make these compressed products bounded for each fixed \(\epsilon>0\). Explicitly, after enlarging \(p\) to an integer, telescope the bounded factors
\([(1+H)^{(j-1)p}\phi(f_j)(1+H)^{-jp}]\) and use \(HP_{\mathrm{vac}}=0\). Their decomposability makes \(M_I\) multiplication by the phase vacuum moments. For separated Euclidean times use the actual bounded \(B_{s,t}\) and intervening semigroup kernels. If a more general continued Euclidean test form is used in the ultraviolet criterion, its fixed-\(\epsilon\) boundedness, decomposability and identification must additionally be proved; these do not follow from the physical-time energy bound alone. Define their central connected combinations, for example

\[
\mathcal C_2=M_{12}-M_1M_2,\qquad
\mathcal C_3=M_{123}-M_1M_{23}-M_2M_{13}-M_3M_{12}
+2M_1M_2M_3.
\tag{4.64; P}
\]

Suppose the required asymptotically free normalizations \(q_m(\epsilon)\), \(m=2,3\), and specified limiting distributions \(K_m\) satisfy

\[
\|q_m(\epsilon)\mathcal C_m(\epsilon)
-K_m(f_1,\ldots,f_m)I_{P_{\mathrm{vac}}}\|
\le\delta_m(\epsilon)\,\mathfrak p_m(f_1,\ldots,f_m),
\qquad \delta_m(\epsilon)\longrightarrow0.
\tag{4.65; C: sufficient phasewise ultraviolet estimate}
\]

The norm of a decomposable multiplication operator is the essential supremum of its fibre norm. Thus (4.65) gives the same ultraviolet law in almost every phase. Assume the scaled tests and \(q_m(\epsilon)\) are continuous for \(\epsilon>0\), as in the usual scaling families. Use a countable dense set of tests and scaling parameters to choose one common full-measure set. Distributional continuity and the uniform test seminorm extend it to the stated test class and scaling limit; replacing \(\delta_m\) by a local upper envelope preserves its limit zero. A prescribed nonzero \(K_3\) then supplies the requested non-Gaussian component. A directly proved phase-selection/ultraviolet theorem may replace (4.65); the uniform central estimate is sufficient, not necessary.

Combining §§4.10–4.11 proves Theorem 3.5 under H0–H5. The remaining Yang–Mills estimates are the hypotheses explicitly marked C/O, especially the complete normalized hierarchy, continuum rotations, Gram domination and phasewise ultraviolet law. The functional-analysis implications after those inputs are proved or imported with their stated hypotheses.
