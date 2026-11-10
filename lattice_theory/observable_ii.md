# Direct continuum principal trace in all 21 channels

**Status.** This note evaluates the continuum principal part of the complete uniform-source Gaussian trace used in the fixed-block matching argument. It proves its sign in every one of the 21 curvature-bilinear directions. The calculation is for an arbitrary fixed compact simple Lie algebra, with its invariant form and coupling convention stated explicitly. Passing from this principal part to the actual frozen lattice coefficient requires the separate T9/N9 Schur and finite-part argument; that passage is not obtained by naming a continuum anomalous dimension.

The resulting two nonzero rates agree with the dimension-four values in Ferretti–Heise–Zarembo, hep-th/0404187v3, equations (6)–(7), after converting their canonical field strength to the geometric curvature. The derivation here does not extend a large-\(N\) spin chain by assumption.

### 1. Background, source, and conventions

Choose a fixed Cartan color \(H\) and a real constant spatial two-form \(F\). Work in one charged adjoint root space, absorbing its real charge into \(F\). With \(\pi_\mu=-iD_\mu\), use

\[
[\pi_\mu,\pi_\nu]=-iF_{\mu\nu},\qquad
M(F)=\pi^2I_4-2iF.
\tag{U9.1}
\]

This is the background Feynman-gauge quadratic vector precision. The antisymmetric real matrix \(F\) makes \(-iF\) Hermitian. Gauge fixing is held independent of the uniform insertion source.

Let \(f=(F_{12},F_{13},F_{14},F_{23},F_{24},F_{34})\), and let
\(J\in\operatorname{Sym}^2(\Lambda^2\mathbb R^4)\). Normalize the source as

\[
H_J(F)=\tfrac12 f^TJf.
\tag{U9.2}
\]

For \(J=I_6\), this is the usual \(\tfrac14\sum_{\mu,\nu}F_{\mu\nu}^2\). Extend \(J_{\mu\nu,\rho\sigma}\) antisymmetrically in each pair from its \(\mu<\nu,\rho<\sigma\) entries.

The global uniform tensor source is stationary on a constant commuting background, as proved in T9. Its Hessian has two terms: the square of the linearized curvature with coefficient \(J\), and the curvature times the second variation of the connection commutator. In a midpoint covariant symbol they give

\[
\begin{aligned}
(M_{J,0})_{\nu\sigma}(p)
 &=\sum_{\mu,\rho}J_{\mu\nu,\rho\sigma}p_\mu p_\rho,\\
(M_{J,1})_{\nu\sigma}(F)
 &=-\frac i2\sum_{\mu,\rho}J_{\mu\nu,\rho\sigma}F_{\mu\rho}
   -i(JF)_{\nu\sigma}.
\end{aligned}
\tag{U9.3}
\]

Here \((JF)_{\nu\sigma}=\sum_{\rho<\eta}J_{\nu\sigma,\rho\eta}F_{\rho\eta}\). The first term on the second line is the ordering correction in \(\pi_\mu\pi_\rho\); the second is the nonlinear curvature variation. For \(J=I_6\), the source Hessian symbol is
\(p^2I-pp^T-\tfrac32iF\), precisely the Wilson/Yang–Mills Hessian before adding the fixed gauge-fixing form. This check fixes its sign and factor.

There is no source derivative of the ghost determinant in this calculation: the background and the gauge-fixing map are fixed under the uniform tensor variation. The physical quotient formulation in N9 accounts for the same fact without choosing a different quotient for different sources.

### 2. The magnetic inverse through quadratic curvature order

For the commutator convention (U9.1), the covariant symbol product is

\[
a\star b
=ab-\frac i2F_{\alpha\beta}
(\partial_\alpha a)(\partial_\beta b)
-\frac18F_{\alpha\beta}F_{\gamma\eta}
(\partial_\alpha\partial_\gamma a)
(\partial_\beta\partial_\eta b)+O(F^3).
\tag{U9.4}
\]

Repeated spatial indices are summed. Solving
\((p^2I-2iF)\star C=I\) by homogeneous degree in \(F\) gives

\[
\begin{aligned}
C_0(p)&=p^{-2}I,\\
C_1(p,F)&=2iF\,p^{-4},\\
C_2(p,F)&=-4F^2p^{-6}
-\tfrac12|F|_{\mathrm F}^2I\,p^{-6}
+2|Fp|^2I\,p^{-8}.
\end{aligned}
\tag{U9.5}
\]

The Frobenius norm is \(|F|_{\mathrm F}^2=\sum_{\mu,\nu}F_{\mu\nu}^2=2|f|^2\).
At first order the magnetic derivative term vanishes because
\(F_{\alpha\beta}p_\alpha p_\beta=0\). At second order the spin product gives \(-4F^2p^{-6}\). The second derivative in the star product gives the two remaining scalar terms. Thus the orbital and spin responses are both present.

For the logarithmic coefficient of the source trace, one may integrate the ordinary product \(CM_J\). On a periodic momentum cell the trace of a star product equals the trace of the ordinary product. Equivalently, on a continuum annulus the difference is a total momentum derivative; a homogeneous degree \(-4\) total derivative has equal boundary flux at the two radii and contributes no logarithm. The quadratic logarithmic angular coefficient is therefore

\[
\mathcal L_J(F)
=\operatorname{Av}_{n\in S^3}
\operatorname{Tr}_{\mathbb R^4}
\bigl(C_2(n,F)M_{J,0}(n)+C_1(n,F)M_{J,1}(F)\bigr).
\tag{U9.6}
\]

There is no principal \(M_{J,2}\) term for the dimension-four continuum source. The retained lattice remainder has such a term of order \(O(1)\); its trace is integrable and is kept in the N9 finite part.

### 3. Perform the spherical contraction explicitly

Define the symmetric contraction of \(J\), the positive matrix \(A\), and the antisymmetric contraction \(K_F\) by

\[
B_{\nu\sigma}=\sum_\mu J_{\mu\nu,\mu\sigma},\qquad
A=F^TF=-F^2,\qquad
(K_F)_{\nu\sigma}=\sum_{\mu,\rho}
J_{\mu\nu,\rho\sigma}F_{\mu\rho}.
\tag{U9.7}
\]

The elementary spherical moments in four dimensions are

\[
\operatorname{Av}n_\alpha n_\beta=\frac{\delta_{\alpha\beta}}4,
\qquad
\operatorname{Av}n_\alpha n_\beta n_\gamma n_\eta
=\frac{\delta_{\alpha\beta}\delta_{\gamma\eta}
+\delta_{\alpha\gamma}\delta_{\beta\eta}
+\delta_{\alpha\eta}\delta_{\beta\gamma}}{24}.
\tag{U9.8}
\]

In particular
\(\operatorname{Av}M_{J,0}=B/4\),
\(\operatorname{Tr}M_{J,0}(n)=n^TBn\), and
\(\operatorname{Av}(n^TAn)(n^TBn)
=(\operatorname{Tr}A\operatorname{Tr}B+2\operatorname{Tr}AB)/24\).
Substitution into (U9.6) gives the completely explicit quadratic form

\[
\boxed{
\mathcal L_J(F)
=\frac76\operatorname{Tr}(AB)
-\frac1{24}|F|_{\mathrm F}^2\operatorname{Tr}B
+\operatorname{Tr}(FK_F)+2\operatorname{Tr}(F(JF)).
}
\tag{U9.9}
\]

As a small direct check, take diagonal \(J\), write \(J_{ij}=J_{ij,ij}\), and set \(F_{12}=1\), with other independent components zero. Then

\[
\mathcal L_J(F)
=-\frac{23}{6}J_{12}-\frac16J_{34}
+J_{13}+J_{14}+J_{23}+J_{24}.
\tag{U9.10}
\]

The scalar choice gives zero exactly.

### 4. All 21 directions and the signs

Use the orthogonal continuum decomposition into scalar, pseudoscalar, stress, and Weyl source tensors, of dimensions \(1,1,9,10\). This is a decomposition of the 21-dimensional source space. It does not impose a Bianchi identity on the curvature bilinears themselves.

The pseudoscalar source is \(J=c*\). Its contraction \(B\) is zero and \(K_F=-2JF\), so (U9.3) vanishes identically and \(\mathcal L_J=0\).

The other 20 source tensors obey the algebraic first-Bianchi symmetry. Contracting that identity with \(F\) gives \(K_F=JF\). Hence, on those tensors,

\[
\mathcal L_J(F)
=\frac76\operatorname{Tr}(AB)
-\frac1{24}|F|_{\mathrm F}^2\operatorname{Tr}B
-6f^TJf.
\tag{U9.11}
\]

For \(J=cI_6\), \(B=3cI_4\), and the first two terms cancel the last one. For a stress source induced by a trace-free symmetric metric tensor \(h\), one has \(B=2h\), \(\operatorname{Tr}B=0\), and \(\operatorname{Tr}(Ah)=f^TJf\). For a Weyl source, \(B=0\). Therefore

\[
\boxed{
\mathcal L_J(F)=
\begin{cases}
0,&J\text{ scalar or pseudoscalar},\\
-\dfrac{22}{3}H_J(F),&J\text{ stress},\\
-12H_J(F),&J\text{ Weyl}.
\end{cases}
}
\tag{U9.12}
\]

Parity gives equal coefficients on the two five-dimensional chiral Weyl representations. The calculation thus controls the entire ten-dimensional Weyl space, including its three distinct lattice-symmetry subspaces. The nine stress components likewise include both lattice stress subspaces.

The radial momentum integral supplies
\(\operatorname{area}(S^3)/(2\pi)^4=1/(8\pi^2)\), and the Gaussian prefactor contributes \(1/2\). Restoring color, the sum of squared adjoint charges is

\[
\sum_{\alpha\text{ adjoint charges}}\alpha(H)^2
=C_A\langle H,H\rangle.
\tag{U9.13}
\]

This is the invariant-form identity
\(f^{acd}f^{bcd}=C_A\delta^{ab}\). Neutral Cartan modes contribute zero to the curvature response. It holds for every fixed compact simple Lie algebra. There is no planar approximation or omitted trace mixing: the source has two curvature factors and its invariant color bilinear is the fixed form.

In canonical continuum coupling units the principal mean generator is consequently

\[
\boxed{
\mathcal G_{\mathrm{cont}}
=-b\,P_{\mathrm{stress}}
-\frac{18}{11}b\,P_{\mathrm{Weyl}},
\qquad b=\frac{11C_A}{24\pi^2}>0.
}
\tag{U9.14}
\]

Its scalar and pseudoscalar coefficients are zero. In a different Wilson trace/coupling convention, the fixed conversion multiplies \(b\) and the observable coefficient by the same factor. The ratios \(0,0,1,18/11\), and all signs, are unchanged. In the route's actual convention, \(b\) denotes the correspondingly converted one-loop coefficient of the inverse-coupling flow.

### 5. Check the inverse-coupling normalization in the same calculation

One can check the normalization of \(b\) without importing an unrelated beta-function convention. Add a source-independent mass \(\mu^2\) to the background Feynman vector and ghost operators, and set \(d=p^2+\mu^2\). The scalar orbital curvature term of their inverses is

\[
C^{\mathrm{sc}}_2
=-\tfrac12|F|_{\mathrm F}^2d^{-3}
+2|Fp|^2d^{-4}.
\tag{U9.15}
\]

For the mass derivative of the one-loop effective action
\(\tfrac12\operatorname{Tr}\log M-\operatorname{Tr}\log(-D^2)\), the vector and ghost traces combine, after angular averaging, into

\[
|F|_{\mathrm F}^2
\left(\frac32d^{-3}+\frac12p^2d^{-4}\right).
\tag{U9.16}
\]

The convergent radial integrals are

\[
\int\frac{d^4p}{(2\pi)^4}(p^2+\mu^2)^{-3}
=\frac1{32\pi^2\mu^2},\qquad
\int\frac{d^4p}{(2\pi)^4}
\frac{p^2}{(p^2+\mu^2)^4}
=\frac1{48\pi^2\mu^2}.
\tag{U9.17}
\]

Their combination is \(11|F|_{\mathrm F}^2/(192\pi^2\mu^2)\). Divide by the classical action density \(|F|_{\mathrm F}^2/4\), sum color charges, and integrate with respect to \(\mu^2\). The coefficient of \(\log\mu\) in the inverse coupling is exactly \(11C_A/(24\pi^2)\), as used in (U9.14). This is a one-loop normalization check; the standing nonperturbative trajectory premise remains separate.

### 6. Relation to the actual mean-growth calculation

The principal sign alone is not enough to choose a large block parameter in the presence of an uncontrolled block-dependent remainder. N9 instead uses one fixed admitted \(L\), an exact constrained Gaussian Schur identity, and bounded finite parts of the retained action. Its required identity has the form

\[
G_k^{\mathrm f}
=(\log L)\mathcal G_{\mathrm{cont}}
+\mathcal F_k-\mathcal F_{k+1}
+\text{controlled cutoff and finite-volume terms}.
\tag{U9.18}
\]

When that identity and \(\sup_k\|\mathcal F_k\|<\infty\) are justified for the actual source shapes, the finite terms are removed by a bounded coordinate change \(I+g_k^2\mathcal F_k\). The change of running coupling and the already proved amplitude remainder then cost only a summable series. U9 supplies the definite nonpositive principal matrix for that argument. The current completion ledger states whether the separate lattice matching steps have been established.

---
