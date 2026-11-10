# Geometry, ultraviolet coefficients and conditional innovations

## 4.19 Exact geometry sign and the raw-to-rescaled cutoff dictionary

This subsection resolves two finite algebraic ambiguities in R0. It does not supply a marked nonlinear surface estimate. The working identities are derived from the incoming density, and the difference from the printed B119 notation is recorded explicitly.

#### 4.19.1 The geometry increment has a determined sign

**Proposition (P).** Write \(A(q,U)=\sum_pq(p)a_p(U)\), \(X=g_k^{-2}\), \(d(p)=q(p)-X\), and \(H=E_k+R_k+B_k\). The old fluctuation arguments of \(B_k\) are held fixed in this notation. The incoming effective exponent in B119 (2.23), p.258, is \(\mathcal A_q(U)=-A(q,U)+H(U)-E_k^{\rm vac}\). For the reconstructed field \(\mathcal U(A)\) and extracted field \(U_+\), its exact difference is

\[
\begin{aligned}
\mathcal A_q(\mathcal U(A))-\mathcal A_q(U_+)
={}&-X\{A(1,\mathcal U(A))-A(1,U_+)\}\\
&+H(\mathcal U(A))-H(U_+)\\
&-\{A(d,\mathcal U(A))-A(d,U_+)\}.
\end{aligned}
\tag{4.117; P}
\]

Consequently, when the Gaussian and \(P^{(k)}\) are obtained by expanding the uniform-coefficient Wilson action, the geometry term in (4.3) is

\[
G_{\rm geom}(A)
=-A(g_k(\cdot)^{-2}-g_k^{-2},\mathcal U(A))
 +A(g_k(\cdot)^{-2}-g_k^{-2},U_+).
\tag{4.118; P}
\]

**Proof.** Substitute \(q=X+d\), use linearity of \(A\) in its first argument, and subtract the exponent at \(U_+\). The vacuum constant cancels. All Jacobians and the uniform-coefficient gauge/Wilson expansion belong to the same constant-\(X\) calculation and cannot change the coefficient of \(d\). This proves both identities.

**Primary-text check and explicit correction.** B109 (2.12) and the paragraph immediately following it, p.268, define \(P^{(k)}\) from the expansion of \(-g_k^{-2}A\) and the measure, excluding the old-action difference in braces. B119 p.267 identifies its expansion with that construction. The continuation of B119 (3.15), p.268, visibly prints the *positive* increment with the argument \(g_k(\cdot)^{-2}-g_k^{-2}\). With the definitions just checked, that pair of signs is inconsistent with (2.23); it must be reversed to obtain the incoming density. Equivalently one could reverse the coefficient difference itself. This paper uses (4.118), derived above. It is not an unreported alternative definition of \(P^{(k)}\).

This correction preserves every absolute bound on the isolated geometry increment and its localization support, since it changes only its overall sign. It does not license replacing an exact density by a norm estimate. The marked identities in §4.2 already used the full incoming exponent, and therefore need no change.

#### 4.19.2 The explicit later LFR cutoff fixes the rescaled radius

B119 p.265 defines \(\delta_k=g_k(A_1/A_0)p_0(g_k)\). Page 267 rescales the fluctuation by \(A'_k=g_kA_k\), whereas the new partition (3.16), p.268, prints a threshold \(\delta_k\) next to \(A_k\). The later explicit list of the actual characteristic functions, LFR I (1.7)–(1.9), p.178, distinguishes the raw group difference from the free rescaled field. In particular (1.9) is the restriction \(\sup_b|A_j(b)|<g_j^{-1}\delta_j\).

**Working dictionary (L/P).** We adopt the explicit LFR I convention: the linearized raw coordinate is \(B=g_kA\), and the small free-field radius is

\[
\chi_{\delta_k}(g_kA)
=\boldsymbol1_{\{\lVert A\rVert<R_k^{\rm fl}\}},
\qquad
R_k^{\rm fl}:=\frac{\delta_k}{g_k}
=\frac{A_1}{A_0}p_0(g_k).
\tag{4.119; P; cutoff identification L: LFR I (1.9), p.178}
\]

Here \(R_k^{\rm fl}\) is a fluctuation radius, distinct from the localization length \(R_k\). Thus a formula retaining \(\delta_k\) as the raw radius must put \(g_kA_k\), rather than \(A_k\), inside that particular norm. We do not identify the two literally different printed thresholds. The raw nonlinear group selectors in LFR I (1.7)–(1.8) remain their exact group selectors; they are not replaced by (4.119).

For a free block of dimension \(d\), \(dB=g_k^d\,dA\). In distributions, with Euclidean radius and outward unit normal \(n\), the chain rule and radial interpolation give

\[
\begin{aligned}
\nabla_A\boldsymbol1_{\{|g_kA|<\delta_k\}}
 &=-n(A)\,\delta_{\rm D}(|A|-R_k^{\rm fl}),\\
\frac{d}{dt}\int w(A)
 \boldsymbol1_{\{|tA|<R_k^{\rm fl}\}}\,dA
 &=-\frac{R_k^{\rm fl}}{t^2}
 \int_{|A|=R_k^{\rm fl}/t}w(A)\,dS_A,
 \qquad t>0 .
\end{aligned}
\tag{4.120; P}
\]

For disjoint coordinate blocks, the derivative of their product cutoff is the sum of these terms with all other indicators retained. The same argument works for overlapping faces whose intersections have zero surface measure. Coincident or redundant constraints are merged, or differentiated through one common smooth approximation. The first formula follows from \(g_k\delta_{\rm D}(g_kr-\delta_k)=\delta_{\rm D}(r-\delta_k/g_k)\); the second follows by differentiating the moving radius \(R_k^{\rm fl}/t\). Approximation of indicators by smooth radial functions proves the distributional statements for integrable smooth weights, and the coarea formula gives the boundary integrals. Gaussian weights satisfy the required domination. The bulk factor \(g_k^d\) cancels for the dimensionless radial flux, or for the numerator expressed with the \(A\)-coordinate derivative and its chain-rule factor. In contrast, a bare raw surface-to-volume ratio \(dS_B/dB\) scales as \(g_k^{-1}\). These are different quantities.

For completeness, let \(F\) be an orientation-preserving \(C^1\) coordinate diffeomorphism, \(\Omega\) a domain with piecewise \(C^1\) boundary, \(J=\det DF>0\), and \(v,w\) smooth with compact support in the chart. The exact nonlinear pullback is

\[
\int v(a)\cdot\nabla_a\boldsymbol1_\Omega(F(a))\,w(a)\,da
=-\int_{\partial\Omega}
 n(b)\cdot DF(F^{-1}b)v(F^{-1}b)\,
 \frac{w(F^{-1}b)}{J(F^{-1}b)}\,dS_b .
\tag{4.121; P}
\]

Apply the distributional chain rule, change variables \(b=F(a)\), and use \(\nabla_b\boldsymbol1_\Omega=-n\,dS_{\partial\Omega}\). Corners have zero surface measure; the same formula holds by smooth approximation. For \(F(a)=g_ka\), it agrees with (4.120) and the \(g_k^{d-1}\) surface Jacobian. For the nonlinear constraint-straightening or boundary-localizing maps, it records the full cofactor weight and normal displacement. Bounds on these weights must still be proved on their actual charts. Freezing the chart during source differentiation leaves no additional source derivative of \(F\).

**Consequence and limit.** The complete centered Gaussian surface theorem of §4.12 now uses the explicit logarithmic radius \(R_k^{\rm fl}\), with the covariance normalization specified there; the raw/rescaled ambiguity is removed for this application. The sign question and the surface-Jacobian calculation are closed. Nonlinear group selectors, retained large-field conditioning, common coupling normalization, and marked bounds through the boundary coordinate maps remain separate substantive tasks.

#### 4.19.3 The discrete gauge average must also be normalized

There is a second finite normalization discrepancy on the checked LFR I p.201. Formula (1.100) places \(1/N_i\) before its gauge-coordinate sum, whereas the paragraph below states \(N_i=1/(2^d d!)\) when describing the average over the \(2^d d!\) coordinate permutations and sign reversals. Taken together literally, these two reciprocal conventions do not give an average.

We use explicit normalized weights. If \(\mathcal H\) is that finite symmetry group and \(G_\theta\) the graph associated to \(\theta\), define

\[
w_G=\frac{\#\{\theta\in\mathcal H:G_\theta=G\}}{|\mathcal H|},
\qquad \sum_Gw_G=1,\qquad
\mathcal R_{\rm av}\rho=\sum_Gw_G\mathcal R_G\rho,
\qquad
\int\mathcal R_{\rm av}\rho=\int\rho .
\tag{4.121a; P}
\]

**Proof.** For each fixed graph and admitted exterior, the new reference quotient in (1.100) integrates to one in its new variables. Integrating the reset therefore leaves the old mass unchanged. Sum this identity with the nonnegative weights \(w_G\); their sum is one. Repeated images of a graph are automatically handled by the multiplicity in \(w_G\). This is also the normalization required by LFR I (1.102) on the same page.

Thus, if the sum is over all elements of \(\mathcal H\) and the displayed reciprocal factor \(1/N_i\) is retained, its \(N_i\) must mean \(|\mathcal H|=2^d d!\). If \(N_i\) instead denotes the reciprocal cardinality as in the prose, the multiplier is \(N_i\). All positive-lift arguments below use the explicit \(w_G\), rather than the inconsistent combination of the two printed conventions.

## 4.20 The scalar ultraviolet coefficient: Gaussian cancellation and the first interaction target

This subsection closes the separated-point Gaussian coefficient calculation and fixes the first nonzero *formal perturbative* scalar-channel target. It does not identify that coefficient in the nonperturbative Wilson continuum limit. In particular, the Gaussian scalar three-point coefficient is zero, so R6 requires an error smaller than the first interaction term.

#### 4.20.1 Exact two-form covariance and all connected scalar cycles

Use Hermitian generators with \(\operatorname{Tr}(T^aT^b)=\delta^{ab}/2\), \(d_A=N^2-1\), and independent two-form indices \(\mu<\nu\). The free potential and scalar conventions are

\[
\begin{gathered}
\langle A_\mu^a(x)A_\nu^b(y)\rangle_0
=q\,\delta^{ab}\delta_{\mu\nu}D(x-y),
\qquad D(z)=\frac1{4\pi^2|z|^2},\qquad q>0,\\
F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a,\qquad
S(x)=\sum_{a,\mu<\nu}:F_{\mu\nu}^a(x)^2:,\qquad
\mathcal F(x)=2S(x).
\end{gathered}
\tag{4.122; P: definitions}
\]

Here \(\mathcal F=2\operatorname{Tr}F_{\mu\nu}F_{\mu\nu}\) with an ordered Lorentz-index sum and Hermitian component matrices. For anti-Hermitian curvature matrices the corresponding trace has the opposite sign. A pure-gradient change of gauge covariance cancels when the two curls are taken. The formulas below specify kernels at pairwise distinct points and do not prescribe contact extensions.

**Proposition (P).** On this separated configuration space,

\[
\langle S(x)S(y)\rangle_{0,c}
=\frac{12d_Aq^2}{\pi^4|x-y|^8},
\qquad
\kappa_{2m+1}(S(x_1),\ldots,S(x_{2m+1}))=0
\quad(m\ge1).
\tag{4.123; P}
\]

**Proof.** Put \(I(z)=1-2\widehat z\otimes\widehat z\) and \(R(z)=\Lambda^2I(z)\), acting on the six independent two-form components. Differentiate \(D\):
\(\partial_\mu\partial_\rho D=-\delta_{\mu\rho}/(2\pi^2|z|^4)+2z_\mu z_\rho/(\pi^2|z|^6)\).
The four curl terms are
\(-\delta_{\nu\sigma}\partial_\mu\partial_\rho D+
\delta_{\nu\rho}\partial_\mu\partial_\sigma D+
\delta_{\mu\sigma}\partial_\nu\partial_\rho D-
\delta_{\mu\rho}\partial_\nu\partial_\sigma D\).
Substitution gives the one-color curvature covariance

\[
\begin{aligned}
C_{\mu\nu,\rho\sigma}(z)
&=\frac{q}{\pi^2|z|^4}
 (I_{\mu\rho}I_{\nu\sigma}-I_{\mu\sigma}I_{\nu\rho}),\\
C(z)&=\frac{q}{\pi^2|z|^4}R(z),
\qquad R(z)^{\mathsf T}=R(z),\quad R(z)^2=1 .
\end{aligned}
\tag{4.124; P}
\]

Wick contraction at two quadratic vertices gives
\(2d_A\operatorname{tr}_{\Lambda^2}(C(x-y)C(y-x))\). The trace of the identity on this space is six, proving the first formula in (4.123).

Every connected Wick graph of \(m\ge2\) normal-ordered quadratic vertices is a cycle. The color is constant around that cycle. Counting the two half-edge choices at each vertex and the reverse orientation gives

\[
\kappa_m(S(x_1),\ldots,S(x_m))
=2^{m-1}d_A\!
\sum_{\sigma\in\mathfrak S(\{2,\ldots,m\})}
\operatorname{tr}_{\Lambda^2}
 (C_{1,\sigma(2)}C_{\sigma(2),\sigma(3)}
 \cdots C_{\sigma(m),1}),
\quad C_{ij}=C(x_i-x_j).
\tag{4.125; P}
\]

For \(m=2\) the coefficient is two; for \(m=3\) the two reverse cycles yield \(8d_A\operatorname{tr}(C_{12}C_{23}C_{31})\).

Let \(J=*\) be the Euclidean Hodge star on two-forms. Its definition through the oriented volume form implies \(J^2=1\) and
\(J\Lambda^2M=\det(M)\Lambda^2M J\) for an orthogonal \(M\). Each \(I(z)\) reverses orientation, hence \(JC(z)J=-C(z)\). Consequently

\[
\operatorname{tr}(C_1\cdots C_m)
=\operatorname{tr}(JC_1\cdots C_mJ)
=(-1)^m\operatorname{tr}(C_1\cdots C_m).
\tag{4.126; P}
\]

Every odd-cycle trace is zero. Formula (4.125) proves the second assertion of (4.123).

This cancellation does not make the scalar composite Gaussian. At four collinear points \(x_i=(i-1)te\), with \(|e|=1\), every covariance has the same reflection factor \(R\), and \(\operatorname{tr}R^4=6\). The three unoriented cycle denominators are \(81t^{16}\), \(256t^{16}\), and \(20736t^{16}\). Therefore

\[
\langle S(0)S(te)S(2te)S(3te)\rangle_{0,c}
=\frac{96d_Aq^4}{\pi^8t^{16}}
 \left(\frac1{81}+\frac1{256}+\frac1{20736}\right)
=\frac{169d_Aq^4}{108\pi^8t^{16}}>0.
\tag{4.127; P}
\]

The requested nonzero scalar *three*-point coefficient is thus a stronger specific test than non-Gaussianity of this quadratic free composite.

#### 4.20.2 The checked formal interaction coefficient

Write \(u=g_{\rm YM}\) for the conventional coupling and \(g_{\rm tH}=\sqrt N\,u\). Canonically normalized curvature is \(F=dA+u[A,A]\); its free covariance has \(q=1\). The formal one-loop coefficient is \(b_u=11N/(48\pi^2)\), namely \(\mu\,du/d\mu=-b_u u^3+O_{\rm formal}(u^5)\).

**Checked import (L, formal perturbation theory only).** Becchetti–Bochicchio, JHEP 03 (2019) 088, [arXiv:1810.08527](https://arxiv.org/abs/1810.08527), (3.4)–(3.7), printed pp.9–10, give, with \(N_f=0\), the noncontact coefficient \(C_{\mathcal F\mathcal F}^{\mathcal F}=4b_u u^2/(\pi^2|x|^4)+O_{\rm formal}(u^4)\). Since \(\mathcal F=2S\), this becomes

\[
C_{SS}^{S}(x)
=\frac{2b_u u^2}{\pi^2|x|^4}
 +O_{\rm formal}(u^4),\qquad x\ne0 .
\tag{4.128; L, with P normalization conversion}
\]

The source's leading delta-function contact coefficient is separate. It is not a separated scalar three-point contribution.

The normalization can also be checked from Zoller–Chetyrkin, JHEP 12 (2012) 119, [arXiv:1209.1516v3](https://arxiv.org/abs/1209.1516), (4.24), p.15. For \(O_1=-\mathcal F/4\), \(a_s=u^2/(4\pi^2)\), it gives
\(C_1^{GG}=-1+a_s[-49N/36-(11N/12)\log(\mu^2/Q^2)]+O_{\rm formal}(a_s^2)\).
Changing to \(\mathcal F\) multiplies the coefficient by \(-4\). The inverse Fourier transform needed for its noncontact logarithm is

\[
\begin{aligned}
\int\frac{d^4p}{(2\pi)^4}e^{ipx}
 \left(\frac{\mu^2}{p^2}\right)^\alpha
&=\frac{\mu^{2\alpha}\Gamma(2-\alpha)}
 {4^\alpha\pi^2\Gamma(\alpha)}
 (x^2)^{\alpha-2},\qquad x\ne0,\\
\mathcal F^{-1}\!\left[\log\frac{\mu^2}{p^2}\right](x)
&=\frac1{\pi^2|x|^4}.
\end{aligned}
\tag{4.129; P}
\]

For \(0<\operatorname{Re}\alpha<2\), represent \((p^2)^{-\alpha}\) by its Gamma integral and perform the Gaussian Fourier integral; the change of variable \(|x|^2/(4t)\) gives the first line. Analytic continuation and differentiation at \(\alpha=0\) give the second line. Choices of extension at \(x=0\) affect only contacts. Multiplying by \((11N/3)a_s\) gives \(4b_u u^2/(\pi^2|x|^4)\), independently checking the sign and factors in (4.128).

#### 4.20.3 A nonzero formal hierarchical three-point coefficient

Let a bar mean normalized spherical averaging in \(\omega\in S^3\), and let \([\,\cdot\,]_{u^2}\) extract the formal coefficient of \(u^2\). Then

\[
\lim_{r\downarrow0}r^4
\left[\overline{
\langle S(r\omega)S(0)S(y)\rangle_c}\right]_{u^2}
=\frac{24b_ud_A}{\pi^6|y|^8}
=\frac{11N(N^2-1)}{2\pi^8|y|^8},
\qquad y\ne0 .
\tag{4.130; P within the formal OPE, using (4.128)}
\]

**Proof in that scope.** Multiply the scalar OPE coefficient \(2b_u/(\pi^2r^4)\) by the Gaussian two-point coefficient \(12d_A/(\pi^4|y|^8)\). The identity channel vanishes in the connected triple. There is no nonconstant local gauge-invariant operator of engineering dimension below four in pure \(SU(N)\) Yang–Mills theory: a single curvature has zero trace, and derivatives cannot lower dimension. At dimension four, spherical averaging removes the nonscalar irreducible tensor coefficients, and parity excludes the pseudoscalar. Derivative descendants and higher-dimensional operators carry positive additional powers of \(r\). In the formal gauge-invariant OPE, equation-of-motion and BRST-exact terms give only contact contributions to these separated insertions. This identifies the scalar channel and proves (4.130).

No summation of an infinite perturbative series or nonperturbative exchange of limits is claimed. A finite field change \(S\mapsto(1+O(u^2))S\) cannot alter this first nonzero coefficient, because the order-zero triple vanishes. The scalar hierarchical coefficient also does not determine the complete triangle kernel without further Ward identities; no conformal three-point ansatz is assumed here.

#### 4.20.4 Literal P2 matching and the one-loop normalization correction

For a smooth anti-Hermitian connection with curvature \(\mathscr G=iT^aG^a\), expand its plaquette holonomy. Tracelessness removes the linear trace and gives

\[
s_{p_{\mu\nu}(x)}
=-\frac{a^4}{2}\operatorname{Tr}\mathscr G_{\mu\nu}(x)^2+o(a^4)
=\frac{a^4}{4}\sum_a(G_{\mu\nu}^a(x))^2+o(a^4).
\tag{4.131; P: classical expansion}
\]

Only the leading term is used; a lower-vertex evaluation need not have an \(a^6\) next error. With \(G=uF(A,u)\), the P2 action has continuum coefficient \(\beta_a u^2/4\) multiplying \(S\). The canonical action is \(\frac12\int S\). Hence the exact convention conversion is

\[
\beta_a=\frac2{u^2}=\frac{2N}{g_0^2},
\qquad
u^2=\frac{g_0^2}{N},\qquad
g_0=g_{\rm tH},\qquad
O_{\rm match}^{(0)}=\frac{u^2}{4}S
=\frac{g_0^2}{4N}S.
\tag{4.132; P: classical/formal matching}
\]

\(O_{\rm match}^{(0)}\) is a formal canonical matching symbol, not an established continuum limit of the bare lattice field. With ordered Lorentz summation it equals \(-\operatorname{Tr}\mathscr G^2/4\). Thus the positive P2 scalar has the sign displayed here; the anti-Hermitian matrix-trace scalar by itself has the opposite three-point sign. Equations (4.123) and (4.130) now give

\[
\begin{aligned}
\langle O_{\rm match}^{(0)}(x)O_{\rm match}^{(0)}(0)\rangle_c
&=\frac{3(N^2-1)}{4N^2\pi^4}
 \frac{g_0^4}{|x|^8}+O_{\rm formal}(g_0^6),\\
\lim_{r\downarrow0}r^4
\left[\overline{\langle
O_{\rm match}^{(0)}(r\omega)
O_{\rm match}^{(0)}(0)
O_{\rm match}^{(0)}(y)\rangle_c}\right]_{g_0^8}
&=\frac{11(N^2-1)}{128N^3\pi^8|y|^8}.
\end{aligned}
\tag{4.133; P: formal conversions}
\]

For the second line, the three factors \(u^2/4\) multiply the order-\(u^2\) coefficient, producing \(11Nd_Au^8/(128\pi^8)=11d_Ag_0^8/(128N^3\pi^8)\). It begins at order \(g_0^8\), rather than the vanishing Gaussian order \(g_0^6\).

The same conversion fixes the provisional one-loop normalization in the preamble:

\[
x=g_0^{-2}=\frac1N u^{-2},
\qquad
\frac{dx}{d\log\mu}
=\frac{2b_u}{N}+O_{\rm formal}(x^{-1})
=\frac{11}{24\pi^2}+O_{\rm formal}(x^{-1}).
\tag{4.134; P: conversion of the formal one-loop import}
\]

Thus, with the *literal P2 action*, the formal decrement in \(x\) under coarse-graining by \(L\) is \(-11\log L/(24\pi^2)\). The value \(11N/(24\pi^2)\) belongs to \(u^{-2}\). This supplies the normalization content of ICR-N1-1; it is not a derivation of N2-F's nonperturbative remainder or a silent change to its verbatim statement.

#### 4.20.5 The comparison still needed, at the correct order

Let \(u_\epsilon\) be the conventional running coupling at scale \(\epsilon\). After constructing the actual scalar field normalization \(Z_{\epsilon,a}\), denote by \(\Phi_{\epsilon,a,T}\) the rescaled distribution \(\epsilon^4 Z_{\epsilon,a}O_a^{(0)}(x_*+\epsilon x)\) normalized to the canonical \(S\) convention. Its connected distributions \(G^{(m)}_{\epsilon,a,T}\), on compact subsets \(Q\) of separated configurations, must satisfy a bound of the form

\[
\begin{aligned}
|\langle G^{(2)}_{\epsilon,a,T}-K_2,f\rangle|
&\le\delta_{2,Q}(\epsilon,a/\epsilon,\epsilon/T)\,p_Q(f),\\
|\langle G^{(3)}_{\epsilon,a,T}-u_\epsilon^2K_3,f\rangle|
&\le u_\epsilon^2
 \delta_{3,Q}(\epsilon,a/\epsilon,\epsilon/T)\,p_Q(f),
\qquad \delta_{m,Q}\longrightarrow0 .
\end{aligned}
\tag{4.135; O: sufficient uniform nonperturbative comparison}
\]

Here \(K_2\) is (4.123) with \(q=1\); \(K_3\) must have the specified nonzero scalar hierarchical coefficient (4.130). It suffices instead to formulate the second line directly on separated, spherically projected hierarchical test families if that is the coefficient chosen for P1. A full triangle-kernel target requires its own identification. All estimates include the normalized history sum and the actual field matching. Torus harmonic modes, lattice errors and cutoff removal are not covered by the continuum Gaussian computation.

**Sharpness of the order (P).** Both \(G_\epsilon^{(3)}=0\) and \(G_\epsilon^{(3)}=u_\epsilon^2K_3\) obey a Gaussian \(o(1)\) comparison. Only an \(o(u_\epsilon^2)\) remainder distinguishes the first interaction coefficient. This follows immediately by dividing the second line of (4.135) by \(u_\epsilon^2\).

For phase transfer the sufficient central criterion of §4.11.3 must have the corresponding strength:

\[
\|\mathscr C_2^\epsilon-K_2 I\|\longrightarrow0,\qquad
\|u_\epsilon^{-2}\mathscr C_3^\epsilon-K_3 I\|
\longrightarrow0 .
\tag{4.136; C: sufficient phasewise estimate; O for the YM application}
\]

The fibres of \(\mathscr C_m^\epsilon\) are phasewise *connected* correlations. The essential-supremum and countable-density proof in §4.11.3 then applies. A mixed-state connected coefficient alone does not prove this estimate.

Finally, a contact distribution supported on partial diagonals annihilates a product of test functions with pairwise disjoint supports. It therefore cannot repair the Gaussian zero or change a separated coefficient. This is a support argument: the product support does not meet any diagonal. Locality only to a fixed physical cell is weaker and can still affect distinct points within that cell. R4 must establish the actual contact support needed here.

## 4.21 Complete reference cancellation and boundary dressing of surviving histories

There are two different normalization questions. A normalized auxiliary reference can be changed without changing a completely integrated original payload. A compulsory survivor's old mass is a factor in the physical marginal and cannot be removed by that identity. This subsection proves the first statement for the unreduced positive construction and controls a specified bounded boundary interaction in the second.

#### 4.21.1 The positive lift and cancellation against every original payload

Keep the original fine variables \(\omega_0\), all old variables of still unperformed integrations, and all selector, coordinate-gauge and original gauge-orbit labels. An original payload is evaluated at the retained \(\omega_0\), including those orbit coordinates. At finite cutoff, normalize the original positive measure by its finite partition function. An executed reset in LFR I (1.100), p.201, has the lifted form \(d\sigma_{h,v}(\omega)\,q_{h,v}(du)\), where the new reference \(q_{h,v}\) is its own numerator divided by its integral. The old integration variables \(\omega\) are retained as latent variables, rather than identified with the new \(u\). Any old variable on which the reference depends is included in the conditioning data \(v\).

The gauge average uses the normalized weights (4.121a). Every rejected selector branch is retained as the identity branch. The last small/large split is explicitly a decomposition of unity on LFR II p.378. The raw block map in B119 (3.1), p.264, is also normalized: integrating the new field against normalized Haar integrates its block delta function to one. Preliminary integrations and coordinate changes may be left undone in this lifted description. Extracted vacuum scalars are restored, so that the entire un-subtracted positive density is being transported.

These facts realize the complete finite construction as normalized forward kernels on the enlarged space. The assertion concerns complete positive operations, not individual signed connected activities or a single resummed survivor factor. The backward continuation with all later flags and all terminal outputs integrated is one.

**Theorem (P).** Vary only selected normalized references, keeping the original input law and all other prescriptions fixed. Let \(L_n(z)\) be the likelihood of the resulting forward history law relative to its base law. For real admissible \(z\), and every integrable payload \(F(\omega_0)\) of the original fine variables,

\[
\mathbb E_0[L_n(z)\mid\omega_0]=1,\qquad
\mathbb E_0[F(\omega_0)L_n(z)]
=\mathbb E_0 F(\omega_0).
\tag{4.137; P}
\]

**Proof.** Each executed reference likelihood has conditional expectation one before that reset. For identity, selector and unchanged block transitions its likelihood is one; a selector is not conditioned on a prescribed future outcome. Iterating conditional expectation over all later normalized kernels proves the first identity. For nonnegative \(F\), Tonelli proves the second. Apply it to the positive and negative parts of an integrable real \(F\), or to the real and imaginary parts. It also proves integrability under the changed law since \(\mathbb E_0[|F|L_n(z)]=\mathbb E_0|F|\).

For a holomorphic reference deformation the same identities hold wherever the finite construction admits \(L^1\) analytic continuation. Differentiation then shows that every globally summed coefficient with positive auxiliary-reference order has zero integral against an original payload. Finite-lattice Wilson and clover payloads are bounded, and the finite reference disks supplied by the denominator bounds justify this step. In particular, mixed derivatives with an original source generating factor also vanish if their auxiliary-reference order is positive.

No uniform accumulated square-cost is required for this exact cancellation. It justifies keeping all references at zero source in the exact raw marked partition identities. It does not make the individual extracted activities or counterterms reference independent, and it gives no bound on their absolute norms. The original source remains a payload of the initial positive law, whose normalized correlations are precisely the difficult objects to control.

#### 4.21.2 What the likelihood bound gains from complete flag summation

For affine reference changes \(X_j\mapsto X_j+u_jz\), let \(b_j=u_j^2D_j^2/X_j^2\), with the actual centered-energy constants of (4.110)–(4.111). The next executed component and slope may depend on the past. If \(\sum_j b_j\le B\) on every path, then complete summation over later flags gives

\[
\mathbb E_0|L_n(z)|^2\le e^{C|z|^2B},\qquad
\|L_n^{(m)}(0)\|_2\le m!(C_1\sqrt B)^m,
\qquad |z|\sqrt B\le c.
\tag{4.138; P, with the stated deterministic budget}
\]

**Proof.** Conditional reference means are one and conditional second moments are bounded by \(e^{C|z|^2b_j}\). Hence
\(|L_j|^2\exp(-C|z|^2\sum_{i\le j}b_i)\) is a supermartingale. Its expectation gives the first inequality, and Banach-valued Cauchy on a circle of radius \(c_1/\sqrt B\) gives the second. If \(B=0\), the likelihood is one. A final marginal likelihood is \(\mathbb E_0[L_n(z)\mid V]\), so conditional-expectation contraction gives the same bound.

This proves that *summed* future flags do not create the conditioning obstruction for the auxiliary sector. Prescribing one future sector and normalizing inside it would change the law and is not covered. No uniform physical-cell estimate for \(B\) is asserted: all affected components, including their fine-scale multiplicity, must enter it.

#### 4.21.3 A boundary comparison valid even under prescribed future flags

Use the literal unresummed boundary family of B119 (2.40)–(2.42), p.261. At a fixed generation \(j\), let \(D\) contain \(n_j(D)\) localization cubes, including every cube incident to an active link. Let \(B_D^{(j)}\) be the sum of that family's terms which depend on active variables in \(D\). The checked inductive bound is \(|B^{(j)}(X)|\le B_0e^{-\kappa d_j(X)}\).

Let \(Q\) be any probability measure supported on the admitted real variables; it may already contain compulsory flags, old masses, constraints and an arbitrary nonnegative later weight. Then

\[
e^{-c_Bn_j(D)}
\le\frac{e^{B_D^{(j)}}}{Qe^{B_D^{(j)}}}
\le e^{c_Bn_j(D)},\qquad
c_B=2B_0C_\kappa,\qquad
C_\kappa=\sup_\square\sum_{X\ni\square}
 e^{-\kappa d_j(X)}<\infty .
\tag{4.139; P, using the checked bound (2.42)}
\]

**Proof of the rooted sum and comparison.** The localization domains in B109 p.257 are connected unions of cubes, and \(d_j\) is the rescaled length of a shortest tree meeting them. A connected set of \(n\) cubes containing a specified cube has at most \((2d)^{2(n-1)}\) possibilities: encode a canonical spanning tree by its depth-first nearest-neighbor walk. This count also holds on a compatible torus.

A tree of length \(\ell\) can meet at most \(c_d(1+\ell)\) unit cubes. Traverse the tree in length \(2\ell\), mark points at arclength intervals at most one, and cover by unit balls centered at those points; each ball meets only a dimensional number of cubes. Thus \(d_j(X)\ge n/c_d-1\). It follows that

\[
C_\kappa\le
\sum_{n\ge1}(2d)^{2(n-1)}
\exp\{-\kappa\max(0,n/c_d-1)\}<\infty
\tag{4.140; P}
\]

for the sufficiently large fixed decay parameter in the construction. Summing first over active cubes yields
\(\operatorname{osc}B_D^{(j)}\le2B_0C_\kappa n_j(D)\).
For any real \(B\) with oscillation at most \(M\), both \(e^B\) and its expectation lie between \(e^{\inf B}\) and \(e^{\sup B}\), so \(e^{-M}\le e^B/Qe^B\le e^M\). This proves (4.139), independently of every other factor in \(Q\).

Consequently removal of this *specified bounded boundary interaction* costs at most \(e^{c_Bn_j(D)}\) in any nonnegative expectation, including an exponential history moment. No survivor is deleted. If a fixed physical cell contains \(L^{4(K-j)}\) fine localization cubes, that multiplicity is retained; no dimension-four renormalization weight is inferred from (4.139).

#### 4.21.4 The actual survivor mass and the remaining conditioned continuation

LFR II (1.103), p.391, writes the survivor contribution, before its final boundary logarithm, as

\[
\left(\prod_i t_i(v)\right)
\left[\bigotimes_i\mu_{i,v}\right]e^{B(v,\omega)},
\qquad
t_i(v)=T'_k(Y_i;v)1,\qquad
\mu_{i,v}=t_i(v)^{-1}T'_k(Y_i;v).
\tag{4.141; L/P: probability notation for the exact factorization}
\]

Zero-mass sectors can be discarded from this disintegration. Page 392 explicitly leaves the \(t_i\) as functions of the new field \(V_k|_{Y_i}\), multiplying the subsequent density. Their upper bounds do not give a lower comparison or control their variation relative to their local average.

For the *resummed* boundary in (1.103), the exact oscillation cost is
\(2\sum_{X:\,B'^{(k)}(X)\ {\rm depends\ on\ the\ active\ old\ variables}}\|B'^{(k)}(X)\|_\infty\).
The estimate (1.99) uses its relative tree metric with the fixed survivor family. It cannot be replaced silently by the ordinary \(d_j\) in (4.140). The text on p.391 expressly explains that survivor domains are fixed in that particular cluster expansion; their geometry is not being summed.

To state what is still missing, let \(Q\) be a current positive reference, \(h\ge0\) its actual future continuation after a local event or nonconstant payoff has been retained, and \(0<Qh<\infty\). If \(Qe^{sV}\le M\), then for \(0<\theta<1\),

\[
Q^H(du)=\frac{h(u)}{Qh}\,Q(du),\qquad
Q^He^{\theta sV}
\le M^\theta
\frac{\|h\|_{L^{1/(1-\theta)}(Q)}}{Qh}.
\tag{4.142; P}
\]

Hölder with exponents \(1/\theta\) and \(1/(1-\theta)\) proves this formula. Thus a uniform local reverse-Hölder comparison for this *actual* continuation, or an appropriate averaged comparison such as (4.81), would close this normalization step. It is not proved here.

The first unboundedly deep factors to be controlled are the retained old operation \(T_k''(Z_k)\) and, after replacement, the compulsory masses \(t_i(V_k)\) with their selectors and constraints. A finite-energy bound for the terminal Wilson action does not estimate those factors. Equation (4.137) removes auxiliary-reference motion from globally integrated original payloads; it does not remove these masses from a local physical-source estimate. R2 therefore remains open.

## 4.22 The universal coupling family and its complete old-activity response

The universal coefficient in the source-free complete expansion is defined by the regular small-field construction. This fact reduces its parameter problem, while leaving the marked R/B response in the full density intact. On the original fixed background domains, one can also prove a derivative bound with respect to the *entire* old regular-activity family. Couplings in this subsection use Balaban's normalization; their identification with the preamble's running parameter still requires the dictionary in §2.1 and R0.

#### 4.22.1 Identification of the universal coefficient

**Checked definitions (L).** B119 (2.24)–(2.25), p.259, define

\[
\begin{aligned}
g_{j-1}(y)^{-2}
&=g_j(y)^{-2}+\beta_j(g_{j-1})\phi_j(y),\\
E_k(U_k)
&=\sum_{j=1}^k\left[
E^{(j)}(\Lambda_j,g_{j-1},U_k)
-E^{(j)}(\Lambda_j,g_{j-1},1)
-\beta_j(g_{j-1})A(\phi_j,U_k)\right].
\end{aligned}
\tag{4.143; L: B119 (2.24)–(2.25), p.259}
\]

The preceding paragraph assigns vacuum and coupling subtraction to E, vacuum subtraction alone to R, and no subtraction to B. Following (3.47), p.278, an interior fresh regular activity supported in \(\Lambda_{k+1}\) is identified with its whole-lattice counterpart. Page 279 takes those terms as \(E^{(k+1)}\), sends the other carriers to B, and performs the new Wilson subtraction on the regular part.

**Reduction proposition (P).** The coherent-family problem for this source-free universal \(\beta_j\) reduces to the whole-lattice regular construction with the prescribed cutoffs. No separate universal beta function is needed for each large-field history.

**Proof.** The first coefficient is the whole-lattice regular Wilson projection. Suppose the old E activities and their coefficients have that identification. The interior-carrier identity just cited identifies the new E activities with their whole-lattice values; the remaining terms are allocated to B or R by the prescribed decomposition. The new subtraction on p.279 is performed on the identified E family. Induction proves the claim. Absolute convergence and linearity of the Wilson projection also make an unchanged summed activity independent of its particular localization repartition.

This does not imply a zero source derivative of R or B, or a zero Wilson projection for their jets in the separately frozen scheme. Earlier *regular* couplings remain suppressed arguments of \(\beta_j(g_{j-1})\), as B109 p.298 explicitly records. They are part of the reduced problem.

#### 4.22.2 A complete old-family derivative on the original fixed domains

Fix the current coupling and cutoff of B109–B116. Let \(\mathscr H_k\) be the space of all old regular localized activities, with their linear vacuum and Wilson extractions, obeying the gauge and lattice covariance identities. Its norm is the maximum over old generations of the exponentially weighted supremum on the fixed absolute domains \(U_j^c(X,\alpha_0,\alpha_1)\) of B109 p.263. Let \(\Psi_k(g,H)\) be the freshly generated non-Gaussian regular family. The freshly added Gaussian determinant is independent of the old-activity input \(H\).

The old-age localizer sums in B116 (1.26)–(1.36), pp.8–9, are included in this map. Lemma 3, (2.38), p.20, has a prefactor \(C_3\epsilon_1\), with
\(C_3=2(L+2)^4O(1)\,2E_0C_1\alpha_4^{-1}\alpha_6^{-1}M^q e^{C_2\kappa_1}\).
The final connected summation (2.39)–(2.41), pp.20–21, keeps that linear \(E_0\epsilon_1\) majorant. Reserving a fixed amount of carrier decay gives

\[
\|\Psi_k(g,H)\|_\kappa
\le C_{\rm sf}E_0\epsilon_1
\quad\text{for }\|H\|_{\mathscr H_k}\le E_0.
\tag{4.144; P from the checked B116 majorants}
\]

For the estimates below fix the construction's smallness parameters so that the same connected expansion is admitted up to \(2E_0\), with upper bound \(2C_{\rm sf}E_0\epsilon_1\). All inverse field margins in \(C_1,\alpha_4^{-1},\alpha_6^{-1}\) remain in \(C_{\rm sf}\). No coupling-dependent radius is substituted for those fixed constants.

Complex auxiliary perturbations of the old activities are legitimate on this ball. Before the logarithm their coefficients enter entire exponential factors; the connected expansion is absolutely convergent under the same absolute potential majorant and defines its holomorphic logarithm. Gauge/covariance restrictions and the prescribed subtractions are linear and are retained. Thus the uniform output bound holds on the complex auxiliary ball, with every old generation included.

**Proposition (P, in this fixed-domain scheme).** For \(\|H\|\le E_0\),

\[
\begin{aligned}
\|D_H\Psi_k(g,H)[h]\|_\kappa
&\le4C_{\rm sf}\epsilon_1\|h\|_{\mathscr H_k},\\
\|D_H^2\Psi_k(g,H)[h_1,h_2]\|_\kappa
&\le32C_{\rm sf}\epsilon_1E_0^{-1}
 \|h_1\|_{\mathscr H_k}\|h_2\|_{\mathscr H_k}.
\end{aligned}
\tag{4.145; P}
\]

**Proof.** Apply Cauchy to \(H+zh\) on \(|z|=E_0/(2\|h\|)\). The input norm is at most \(3E_0/2\), and the enlarged bound (4.144) gives the first inequality. For the mixed derivative use radii \(E_0/(4\|h_i\|)\). Their inverse product times \(2C_{\rm sf}E_0\epsilon_1\) gives the second inequality. Zero directions are immediate. The reserved carrier decay justifies differentiation and summation in the output norm.

The Wilson extraction \(\mathcal P_k\), B109 (1.20)–(1.22), p.264, uses two background derivatives and a second spatial moment. If \(\alpha\) is the smaller fixed available background margin, field Cauchy and the exponentially convergent moment sum give

\[
|\mathcal P_kF|
\le C_{\rm mom}\alpha^{-2}\|F\|_\kappa,\qquad
|D_H\beta_{k+1}(g,H)[h]|
\le4C_{\rm mom}\alpha^{-2}C_{\rm sf}\epsilon_1\|h\|.
\tag{4.146; P}
\]

These are uniform old-family response bounds within the original admitted geometry. They do not extend that geometry to every torus, and they are not yet total bare-coupling derivatives.

#### 4.22.3 Why a direct shrinking-radius estimate fails, and the two obligations it creates

The actual B119 domains have \(\alpha_{i,j}=C_i g_j(\log g_j^{-2})^{q_i}\), (2.28), p.259. A shrinking margin cannot be removed from (4.146). For example, if \(\epsilon_j\asymp g_j(\log g_j^{-2})^p\) and \(\rho_j\asymp g_j(\log g_j^{-2})^q\), then

\[
\epsilon_j\rho_j^{-2}
\asymp g_j^{-1}(\log g_j^{-2})^{p-2q},
\qquad g_j\downarrow0.
\tag{4.147; P}
\]

This is unbounded for any fixed logarithmic exponents, even before the other inverse radii in \(C_{\rm sf}\) are included. Hence (4.145) does not automatically give a projected contraction in the prescribed B119 family.

This calculation creates two precise obligations. **CT-domain** requires the actual whole-lattice B119 regular activities, with their consistently rescaled cutoffs, to admit the fixed-domain old-family perturbations above, or requires a closed replacement in the actual radius-weighted norms. **CT-derivative** requires control of the current-coupling derivatives \(\partial_g\Psi_k,\partial_g^2\Psi_k,D_H\partial_g\Psi_k\) for that *same* family, including its moving-cutoff surfaces and old interactions. A different analytic-cutoff scheme requires an explicit comparison. Section 4.25 resolves both obligations for the universal regular E family by constructing its fixed-domain extension and an exact holomorphic dilation of its real cutoff integral. The corrected cutoff convention and the sufficient weak-coupling interval remain explicit. This does not extend an arbitrary incoming R/B family.

The exact two-jet ledger shows why both tasks matter. Put \(X_{B,k}(s)=g_k(s)^{-2}\), \(u_k=X_{B,k}'(0)\), \(v_k=X_{B,k}''(0)\), and \(H^{<k}=(H_1,\ldots,H_k)\). For a locally twice differentiable rerun,

\[
\begin{aligned}
g_k'&=-\tfrac12g_k^3u_k,\qquad
g_k''=\tfrac34g_k^5u_k^2-\tfrac12g_k^3v_k,\\
H_{k+1}'&=\Psi_g g_k'+D_H\Psi[H^{<k\prime}],\\
H_{k+1}''
&=\Psi_{gg}(g_k')^2+\Psi_g g_k''
 +2D_H\Psi_g[H^{<k\prime}]g_k'\\
&\quad+D_H^2\Psi[H^{<k\prime},H^{<k\prime}]
 +D_H\Psi[H^{<k\prime\prime}].
\end{aligned}
\tag{4.148; P: chain-rule identities, not bounds on the unknown jets}
\]

Here current partial derivatives include the cutoff if the adapted prescription moves it. The unknown \(u_k\) is retained; replacing \(g_k'\) by a bounded multiple of \(g_k^3\) before proving the coupled estimate would assume the desired conclusion.

The numerical tail itself is strong enough for a finite-jet surface calculation. For a logarithmic rescaled cutoff and fixed \(p\ge1\), all fixed \(m,n,Q\ge0\) satisfy

\[
g^{-m}(1+\log g^{-2})^n
e^{-cA^2(\log g^{-2})^{2p}}
\le C_{m,n,Q}g^Q,\qquad 0<g\le\gamma<1.
\tag{4.149; P}
\]

Indeed, set \(t=\log g^{-2}\); after division by \(g^Q\), a polynomial in \(t\) multiplies \(\exp((m+Q)t/2-cA^2t^{2p})\), which is bounded. The Gaussian tails in B116 (2.22), (2.26), pp.16–17, have this form after the logarithmic-threshold substitution. This estimate pays a specified finite list of losses only after the complete localized surface calculation has produced them. It is not that calculation.

The fixed-domain old-family derivatives proved here are completed by the current/mixed derivative theorem in §4.25. The coherent regular two-jet feedback is then proved in §4.26 conditional on the exact running-coordinate dictionary R0-reg. A uniform bare-source disk for the entire construction and the complete marked E/R/B induction remain open.

## 4.23 Uniform Ward scores, complete-history transfer, and an actual exterior obstruction

The ordinary-susceptibility formulation in [Ordinary susceptibility and the structure factor](../ordinary_susceptibility.tex) treats a force-frustration observable, of engineering dimension six on smooth fields. Its ordinary-susceptibility target and complex-source input are explicitly incomplete. The estimates below are proved directly under the original Wilson law; none of its imported interfaces is assumed. They give a complete auxiliary theorem, with constants valid for every compatible torus. They do not replace the dimension-four source estimates required by N1-S.

Fix a finite four-dimensional periodic lattice with at least two sites in each direction. This includes every compatible torus in the common preamble. Use the positive-orientation link set, normalized product Haar measure, and the actual Wilson law with any real coupling β>0. For this section only, fix the Lie-algebra metric by −Tr(T_A T_B)=δ_AB on anti-Hermitian generators. Thus the fundamental Casimir is C_F=(N²−1)/N. A different fixed metric changes the explicit constants, but does not change any uniformity assertion.

For a link b let X_b^A denote the left-invariant derivative, and define

\[
 F_b^A=X_b^A S,\qquad P_b=\sum_A(F_b^A)^2,
 \qquad \ell_b=\sum_A(X_b^A)^2S,
 \qquad t_b=\frac13(\ell_b-\beta P_b).
 \tag{4.150; P: definitions}
\]

Put A_N=6(N²−1). For real deterministic marks f write t_f=∑_b f_b t_b and M_f=∑_b f_b².

#### 4.23.1 Uniform conditional score moments and arbitrary-mark variance — P

For every β>0, every finite compatible torus, and every link b, the following bounds hold. They also hold conditionally on **every fixed configuration of the other links**, with the usual continuous one-link Gibbs density:

\[
 \mathbb E[(\beta P_b)^m\mid U_{b^c}]
 \le A_N^m m!\quad(m=0,1,2,\ldots),\qquad
 \mathbb E[t_b\mid U_{b^c}]=0.
 \tag{4.151; P}
\]

Consequently,

\[
 \mathbb E[e^{\lambda|t_b|}\mid U_{b^c}]
 \le\frac{e^{\lambda A_N/3}}{1-\lambda A_N/3}
 \quad(0\le\lambda<3/A_N),
 \qquad
 \operatorname{Var}_{\mu_\beta}(t_f)
 \le380(N^2-1)^2 M_f.
 \tag{4.152; P}
\]

The variance statement permits marks of arbitrary sign and arbitrary lattice-scale oscillation. Its constant is independent of β, lattice spacing, torus side, support size, and the mark.

**Proof.** Hold every link other than b fixed. By cyclicity of the trace and Re Tr(V⁻¹)=Re Tr(V), the six plaquettes incident on b give a one-link action

\[
 S_b(U_b)=6N-\operatorname{ReTr}(U_b A_b),
 \qquad A_b=\sum_{i=1}^{6} V_i,
 \qquad V_i\in\mathrm{SU}(N),\quad\|A_b\|_{\mathrm{op}}\le6.
 \tag{4.153; P}
\]

All remaining terms in S are constant during this conditional integration. The Casimir identity and the one-link geodesic Hessian give

\[
 |\ell_b|=|C_F\operatorname{ReTr}(U_b A_b)|\le A_N,
 \qquad
 |\operatorname{Hess}_b S(\xi,\xi)|
 =|\operatorname{ReTr}(\xi^2 U_b A_b)|
 \le6\|\xi\|^2.
 \tag{4.154; P}
\]

For the last inequality, −ξ² is positive semidefinite and its trace is the squared norm of ξ. Left-invariant vector fields are divergence-free for Haar measure. Integration of the divergence of P_b^{m−1}∇_bS times e^{−βS_b} therefore gives, for m≥1,

\[
 \begin{aligned}
 \beta\mathbb E[P_b^m\mid U_{b^c}]
 &=\mathbb E[\ell_b P_b^{m-1}
 +(m-1)P_b^{m-2}\nabla_bS\cdot\nabla_bP_b\mid U_{b^c}]\\
 &\le[A_N+12(m-1)]\mathbb E[P_b^{m-1}\mid U_{b^c}]\\
 &\le A_N m\,\mathbb E[P_b^{m-1}\mid U_{b^c}].
 \end{aligned}
 \tag{4.155; P}
\]

At m=1 the term multiplied by m−1 is omitted; no negative power is used. Here ∇S·∇P=2 Hess S(∇S,∇S), and A_N≥18≥12 for N≥2. Induction proves the moment bound. The same divergence identity at m=1 proves the conditional centering of t_b. Summing the nonnegative moment series proves

\[
 \mathbb E[e^{s\beta P_b}\mid U_{b^c}]\le(1-A_Ns)^{-1}
 \quad(0\le s<A_N^{-1}),\qquad
 \mathbb E[t_b^2\mid U_{b^c}]\le\frac59 A_N^2.
 \tag{4.156; P}
\]

The exponential bound in (4.152) follows from 3|t_b|≤A_N+βP_b.

For the variance estimate, compact-group integration by parts yields, for every smooth G,

\[
 \mathbb E_{\mu_\beta}[t_bG]
 =-\frac13\mathbb E_{\mu_\beta}[\nabla_bS\cdot\nabla_bG].
 \tag{4.157; P}
\]

The observable t_c depends only on the links of plaquettes containing c. Hence E(t_bt_c)=0 if b and c do not belong to a common plaquette. Including b itself, at most 19 links can belong to a plaquette containing b: one root link and three other links for each of six plaquettes. Periodic coincidences can only reduce this count. By Cauchy–Schwarz, (4.156), and 2|f_bf_c|≤f_b²+f_c²,

\[
 \begin{aligned}
 \operatorname{Var}_{\mu_\beta}(t_f)
 &\le\frac59 A_N^2\sum_{b\sim c}|f_bf_c|\\
 &\le\frac{95}{9}A_N^2\sum_bf_b^2
 =380(N^2-1)^2 M_f.
 \end{aligned}
 \tag{4.158; P}
\]

The adjacency relation is symmetric and includes the diagonal. Every integration is finite-dimensional, every integrand is smooth, and the conditional density is strictly positive. This completes the proof. ∎

#### 4.23.2 A global real Bernstein bound — P

Put B_N=2A_N/3=4(N²−1). Let q≤19 be the number of colors in a proper coloring of the graph in which distinct links are adjacent when they share a plaquette. For every real s satisfying qB_N|s|‖f‖∞<1,

\[
 \log\mathbb E_{\mu_\beta}e^{s t_f}
 \le\frac{qB_N^2s^2 M_f}{1-qB_N|s|\|f\|_\infty}.
 \tag{4.159; P}
\]

In particular, for u>0 and a nonzero mark f,

\[
 \mu_\beta\{|t_f|\ge u\}
 \le2\exp\left[-\frac{u^2}{4qB_N^2M_f+2qB_N\|f\|_\infty u}\right].
 \tag{4.160; P}
\]

**Proof.** From (4.151), 3|t_b|≤A_N+βP_b, and (x+y)^m≤2^{m−1}(x^m+y^m), one obtains E(|t_b|^m|U_{b^c})≤B_N^m m! for m≥1. Conditional centering removes the first-order term. Thus, for real z with B_N|z|<1,

\[
 \mathbb E[e^{zt_b}\mid U_{b^c}]
 \le\exp\left(\frac{B_N^2z^2}{1-B_N|z|}\right).
 \tag{4.161; P}
\]

Each graph vertex has degree at most 18, so greedy coloring uses at most 19 colors. Conditional on the complement of one color class C, no plaquette contains two free links. The Wilson action is a sum of one-link actions in those free links, its conditional law factorizes, and each t_b with b∈C depends only on its own free link and the fixed complement. The conditional product of (4.161), followed by averaging over the complement, therefore gives the same exponential bound with ∑_{b∈C}f_b². Hölder's inequality with exponent q applied to the q color sums proves (4.159). No unconditional independence of colors is used.

For the upper tail use Chernoff's inequality with s=u/(2qB_N²M_f+qB_N‖f‖∞u), and apply the same bound to −t_f for the lower tail. Substitution gives (4.160). ∎

**Scope.** Pair covariance has the displayed contact property because the score is a divergence in one link. The proof does not assert independence at separated links, finite-range higher cumulants, or the N1-S generating-functional bound for ordinary coupling and clover sources. §4.23.2 is a real-source bound for this particular score; a uniform zero-free complex disc is not inferred from it.

#### 4.23.3 Frustration remains after the Ward score is removed

Partition the six coordinate planes into the three matchings {12,34}, {13,24}, and {14,23}, and write S=S₁+S₂+S₃ accordingly. For a fixed link b each matching contributes the two incident plaquettes in one plane. Define

\[
 F_{b,i}=\nabla_bS_i,\quad F_b=\sum_{i=1}^3F_{b,i},\quad
 D_b=\sum_{i=1}^3|F_{b,i}|^2,\quad
 r_b=\beta D_b-\frac13\ell_b,\quad
 h_b=\beta\left(D_b-\frac13P_b\right).
 \tag{4.162; P: definitions}
\]

These are the ordinary and frustration observables of [Ordinary susceptibility and the structure factor](../ordinary_susceptibility.tex). The following exact identities require none of its imported moment estimates:

\[
 h_b=\frac\beta3\sum_{1\le i<j\le3}|F_{b,i}-F_{b,j}|^2\ge0,
 \qquad r_b=h_b-t_b,
 \qquad \mathbb E[r_b\mid U_{b^c}]=\mathbb E[h_b\mid U_{b^c}].
 \tag{4.163; P}
\]

The first equality follows by expanding the three squares. The second follows from the definitions. The last follows from §4.23.1’s exact conditional centering.

**Proposition (P): equivalence of the two susceptibility targets.**

Let Σ_r and Σ_h be the suprema, over nonzero real marks f on a fixed finite torus, of Var(r_f)/M_f and Var(h_f)/M_f, respectively. Then

\[
 |\sqrt{\Sigma_r}-\sqrt{\Sigma_h}|
 \le\sqrt{380}\,(N^2-1).
 \tag{4.164; P}
\]

**Proof.** Center (4.163), sum against f, and use the triangle inequality in L²(μ_β), together with §4.23.1:

\[
 \left|\sqrt{\operatorname{Var}(r_f)}-
 \sqrt{\operatorname{Var}(h_f)}\right|
 \le\sqrt{\operatorname{Var}(t_f)}
 \le\sqrt{380}\,(N^2-1)\sqrt{M_f}.
 \tag{4.165; P}
\]

Take suprema after dividing by √M_f, once in each direction. ∎

Thus the ordinary-susceptibility target is equivalent, up to explicit changes of constants, to controlling the frustration susceptibility. This reduction does not require the imported plaquette moment estimate I1 or the imported contact-error estimate of that formulation. It does not prove either target. The possible growth of the frustration covariance remains the entire noncontact problem.

**Counterexample (P): a uniform same-exterior ordinary variance bound is false.**

For SU(2), on every periodic lattice with at least three sites in each direction, there is a fixed exterior configuration for one link b such that its conditional Wilson law is Haar for every β>0 and

\[
 t_b=0,\qquad
 \mathbb E[r_b\mid U_{b^c}]=12\beta,
 \qquad
 \operatorname{Var}(r_b\mid U_{b^c})=16\beta^2.
 \tag{4.166; P}
\]

For each fixed β, the conditional variance is at least 8β² on an open set of exterior configurations of strictly positive Wilson probability. Hence no bound independent of β can hold for almost every exterior uniformly in β.

**Proof.** Take b=(0,1). Set all transverse links equal to I. The six opposite parallel links (±e_ν,1), ν=2,3,4, are distinct when each side has at least three sites. Choose them so that the two staples in the 12-plane are +I,+I, those in the 13-plane are −I,−I, and those in the 14-plane are +I,−I. Set all other links except b to I. Since −I is central in SU(2), orientation inversion does not alter these signs. The three staple sums are 2I, −2I, and 0. Their total is zero.

Writing q(U)=Re Tr U for the free link, the three portions of the action that depend on it are 4−2q(U), 4+2q(U), and 4. Their sum is the constant 12, so the conditional Gibbs density in U is exactly Haar. Also

\[
 F_{b,1}=-2\nabla q,\qquad F_{b,2}=2\nabla q,\qquad
 F_{b,3}=0,\qquad F_b=0,\quad P_b=\ell_b=0,
 \quad D_b=8|\nabla q|^2.
 \tag{4.167; P}
\]

Parametrize SU(2) by U=u₀I+i∑_{j=1}³u_jσ_j with ∑_{j=0}³u_j²=1. The chosen Lie metric has the orthonormal basis T_j=iσ_j/√2. Thus X_jq=−√2u_j and

\[
 D_b=16(1-u_0^2),\qquad r_b=h_b=16\beta(1-u_0^2).
 \tag{4.168; P}
\]

Normalized Haar measure is the uniform measure on the unit three-sphere. Its coordinate moments are E(u₀²)=1/4 and E(u₀⁴)=1/8. These follow from rotational symmetry and the identity ∑u_j²=1, or directly from the corresponding spherical integral. Therefore E D_b=12 and Var(D_b)=16, proving (4.166).

For fixed β, conditional partition functions and conditional first and second moments are continuous functions of the exterior links: the integrands are continuous on a compact product of groups, and the conditional partition function is strictly positive. A sufficiently small open neighborhood of this exterior consequently has conditional variance at least 8β². The marginal Wilson density is strictly positive everywhere, so this open set has positive probability. ∎

**What the counterexample does and does not settle.** It rules out a proposed proof that first obtains a β-uniform ordinary-source estimate at every fixed exterior and then averages the exterior. It also shows why the total-force score theorem cannot be silently substituted for an ordinary-source theorem: the score vanishes identically in this example while ordinary-source fluctuations grow quadratically in β. It does not disprove the averaged ordinary-susceptibility target, nor the complete-patch fractional comparison of actual R2. The exterior just constructed may be very rare. A valid averaged argument must pay for that rarity with the actual exterior or survivor mass; that is precisely the missing work.

#### 4.23.4 Transfer through complete histories and the survivor-mass distinction

**Exact transfer for the retained original score.**

The unsummed positive representation keeps the original fine field ω₀, each old integration variable, every selector label, the coordinate-gauge label, and the original gauge orbit. At an executed reset, the numerator and its own denominator in LFR I (1.100), p. 201, form a probability kernel in the new auxiliary variable. The coordinate-gauge average on that page has normalized total weight. The displayed identity (1.102) is the resulting preservation of the integrated density. The block constraint in B119 (3.1), p. 264, likewise integrates to one in its new Haar variable.

The algebra can be made independent of the number and positions of executed resets. Write K_j(dh_j|ω₀,h₁,…,h_{j−1}) for the complete one-step transition on all fields and flags, before an optional signed cluster expansion. It has total mass one because it retains all branches, normalized gauge choices, and normalized auxiliary references. Restoring extracted vacuum scalars gives the probability lift

\[
 d\widehat\mu_\beta(\omega_0,h_1,\ldots,h_m)
 =d\mu_\beta(\omega_0)\prod_{j=1}^{m}
 K_j(dh_j\mid\omega_0,h_{<j}),
 \qquad K_j1=1.
 \tag{4.169; P, for the complete positive lift}
\]

Unexecuted operations may be padded by identity kernels, so a finite cutoff gives a fixed finite m. Integrating successively from the final variable to the first gives

\[
 \widehat\mu_\beta\bigl[F(\omega_0)\bigr]=\mu_\beta[F]
 \quad\text{for every integrable }F.
 \tag{4.170; P}
\]

In particular, the estimates of §§4.23.1–4.23.2 hold with the retained original score t_f(ω₀) under this complete history law, with their original constants. Compulsory history branches cause no loss in this statement, because they are not removed or conditioned on; every eventual flag is summed. This is a theorem for the original Wilson-score payload in an exact lift. It is not a claim that the native coarse-field score equals that payload, or that an arbitrary incomplete RG history has the same normalization.

Changing normalized auxiliary references changes the conditional history kernels but leaves (4.170) unchanged. It therefore cannot, by itself, produce a bound on the frustration payload h_f that was not already known under μ_β.

**Conditioning introduces an extra term.**

For any positive C¹ weight H with 0<μ_β(H)<∞, let μ_β^H=Hμ_β/μ_β(H). Direct integration by parts gives

\[
 \mathbb E_{\mu_\beta^H}[t_bG]
 =-\frac13\mathbb E_{\mu_\beta^H}[\nabla_bS\cdot\nabla_bG]
 -\frac{1}{3\mu_\beta(H)}
 \mathbb E_{\mu_\beta}[G\nabla_bS\cdot\nabla_bH].
 \tag{4.171; P}
\]

This formula follows by applying (4.157) to HG and expanding its derivative. If H is independent of U_b, the correction vanishes. For a general continuation it does not. Characteristic-function selectors require a weak or boundary version of the same calculation; their derivative cannot simply be discarded. Thus a conditional Ward estimate cannot be invoked under an actual retained continuation without accounting for that continuation's dependence on the active variables.

**The checked LFR II normalization.**

On p. 380, LFR II (1.73)–(1.75) separates the positive real operation from a small complex correction σ. In the notation of that paper, its proved quotient estimate is

\[
 \left|\frac{T'_k(X,(U,J))F}{T'_k(X,(U,J))1}\right|
 \le e^{3\sup|\sigma|}\sup|F|.
 \tag{4.172; L: LFR II (1.75), p. 380}
\]

The primary text immediately before this estimate says the underlying positive mass may be very small. Its parameter J is a background perturbation in that construction; no identification of it with an arbitrary position-dependent coupling source j is licensed by (4.172).

The later representation (1.103), p. 391, factors the operation algebraically as

\[
 \left(\prod_i t_i(v)\right)
 \left(\bigotimes_i\mu_{i,v}\right)e^{B(v,\omega)},
 \qquad
 t_i(v)=T'_k(Y_i;v)1,\qquad
 \mu_{i,v}=t_i(v)^{-1}T'_k(Y_i;v).
 \tag{4.173; L/P: LFR II (1.103), p. 391}
\]

The normalized kernels act on the boundary exponential, while the factors t_i(v) remain. On p. 392 the paper explicitly identifies those masses as functions of the new field V_k restricted to Y_i, multiplying the effective density. They are not constants that cancel in a subsequent integration over v. They form part of the actual continuation weight H in a calculation such as (4.171).

The same page-391 discussion notes that the survivor domains are fixed in the indicated boundary expansion; their summation is not being controlled by that particular cluster argument. Neither the quotient estimate (4.172), the exact global identity (4.170), nor a moment estimate for a normalized reference measure supplies a lower comparison, a reverse-Hölder estimate, or a complete-patch fractional estimate for these actual multiplying masses. The counterexample of §4.23.3 additionally prevents replacing that task by an exterior-uniform estimate for the ordinary frustration observable.

The final small/large split on LFR II p.378 is a condition on the new field’s curvature, through the displayed decomposition of unity for χ_k. It is not a freely resampled event under a normalized auxiliary Gaussian. Thus the new reference alone cannot make an arbitrary retained exterior satisfy the small-field alternative. The estimates proved here retain the original fine-field payload and all flags. R2 remains an averaged physical-source problem.

## 4.24 Conditional scalar innovations for the actual SU(2) Wilson law

The next theorem proves a uniform conditional analytic bound for the fluctuating part of a scalar Wilson insertion. Its proof is direct and includes a one-link Gamma domination. It concerns the actual Wilson law with arbitrary fixed exterior.

Use \(a_p=1-\tfrac12\operatorname{Re}\operatorname{Tr}U_p\), and write the \(SU(2)\) law as \(d\mu_\tau\propto e^{-\tau\sum_pa_p}dU\), \(\tau>0\). In literal P2, \(s_p=2a_p\) and \(\tau=2\beta_a\). Choose a set \(I\) of free links such that no plaquette contains two of them, and condition on all other links; call this exterior sigma-field \(\mathcal E\). The torus has at least two sites in each direction, which includes every compatible torus; each link has the usual six incident plaquettes. No regularity or unfrustrated-boundary assumption is made.

For a real scalar profile \(f\), set \(J_f=\tau\sum_p f(x_p)a_p\), take the initial site of each free link as its anchor \(x_b\), and put

\[
\omega_b(f)=\max_{p\ni b}|f(x_p)-f(x_b)|,
\qquad
A_b(f)=|f(x_b)|+24\tau\,\omega_b(f),
\qquad
Y_f=J_f-\mathbb E[J_f\mid\mathcal E].
\tag{4.174; P: definitions}
\]

**Theorem (P).** There are numerical \(r_*,C,C_* >0\), independent of \(\tau\), the exterior, the torus, the number of free links, and the number of profiles, with the following properties. For any finite family \(f_i\), put \(s_b(z)=\sum_i|z_i|A_b(f_i)\). On the domain \(\max_bs_b(z)<r_*\), the conditional generating function has its analytic logarithm at zero and

\[
\left|\log\mathbb E\!\left[
 e^{\sum_i z_iY_{f_i}}\mid\mathcal E\right]\right|
\le C\sum_{b\in I}s_b(z)^2.
\tag{4.175; P}
\]

For \(m\ge2\), its conditional cumulants satisfy

\[
|\kappa(J_{f_1},\ldots,J_{f_m}\mid\mathcal E)|
\le C\,m!\,C_*^m
 \sum_{b\in I}\prod_{i=1}^m A_b(f_i).
\tag{4.176; P}
\]

In particular,

\[
\operatorname{Var}_{\mu_\tau}(Y_f)
=\mathbb E\operatorname{Var}(J_f\mid\mathcal E)
\le\frac{21}{2}\sum_{b\in I}A_b(f)^2.
\tag{4.177; P}
\]

The right sides may be restricted to links whose incident plaquettes meet the corresponding source supports. For scalar \(C^1\) profiles, \(\omega_b(f)\le Ca\|\nabla f\|_\infty\), so the relevant profile norm is \(\|f\|_\infty+C\tau a\|\nabla f\|_\infty\). On an N2-F bare trajectory, \(\tau a\) is bounded: asymptotically \(\tau=O(K+\log(K+1))\), whereas \(a=L^{-K}\ell_0\), and any finitely many admitted initial depths only change the bound. This observation uses only the stated bare asymptotic; it does not identify any running Balaban map.

**Proof.** Identify \(SU(2)\) with the unit quaternions \(q\in S^3\). Every incident plaquette has the form \(a_p=1-q\cdot v_p\) for an exterior-determined unit quaternion \(v_p\), after the appropriate orientation convention. Set \(S_b=\sum_{p\ni b}v_p\), \(\varrho_b=|S_b|\), and \(\kappa_b=\tau \varrho_b\). The conditional link law is proportional to \(e^{\tau q\cdot S_b}dq\). The free links are conditionally independent because no plaquette contains two of them.

If \(\varrho_b>0\), put \(u=q\cdot S_b/\varrho_b\) and \(X_b=\kappa_b(1-u)\); if \(\varrho_b=0\), put \(X_b=0\). The marginal Haar density of \(u\) is proportional to \((1-u^2)^{1/2}\) on \([-1,1]\). Substitution \(x=\kappa_b(1-u)\) shows that the density of \(X_b\), relative to a Gamma\((3/2,1)\) density, is proportional to

\[
h_{\kappa_b}(x)=(2-x/\kappa_b)^{1/2}
 1_{[0,2\kappa_b]}(x),
\tag{4.178; P}
\]

a nonnegative decreasing function. For an increasing \(\phi\),
\(2\operatorname{Cov}(\phi(G),h(G))=
\mathbb E[(\phi(G)-\phi(G'))(h(G)-h(G'))]\le0\).
Thus \(X_b\) is stochastically dominated by \(G\sim\mathrm{Gamma}(3/2,1)\). In particular \(\mathbb EX_b\le3/2\), \(\mathbb Ee^{tX_b}\le(1-t)^{-3/2}\) for \(0\le t<1\), uniformly in every exterior.

Let \(Z_b(f)\) be the centered contribution of the six-plaquette star to \(J_f\). The star action equals \(6-\varrho_b+X_b/\tau\). Split \(f(x_p)=f(x_b)+[f(x_p)-f(x_b)]\). The centered constant part is \(f(x_b)(X_b-\mathbb EX_b)\). Since \(0\le a_p\le2\), the remaining term has absolute value at most \(24\tau\omega_b(f)\) after centering. Therefore

\[
|Z_b(f)|\le A_b(f)(X_b+3/2).
\tag{4.179; P}
\]

For \(Z_b(z)=\sum_i z_iZ_b(f_i)\), its conditional mean is zero and \(|Z_b(z)|\le s_b(z)(X_b+3/2)\). Put
\(C_0=\tfrac12\mathbb E[(G+3/2)^2e^{(G+3/2)/4}]<\infty\).
Taylor's inequality \(|e^w-1-w|\le\tfrac12|w|^2e^{|w|}\) and stochastic domination give

\[
\left|\mathbb E[e^{Z_b(z)}\mid\mathcal E]-1\right|
\le C_0s_b(z)^2 \qquad (s_b(z)\le1/4).
\tag{4.180; P}
\]

Choose \(r_*\le1/4\) with \(C_0r_*^2\le1/4\). Each factor is zero-free there and its logarithm is bounded by \(2C_0s_b^2\). Conditional independence gives (4.175) by adding these actual logarithms.

For (4.176), apply multivariable Cauchy to a single-link logarithm on radii \(r_*/(mA_b(f_i))\); directions with zero \(A_b\) contribute zero. The coefficient bound is \(Cr_*^2(m/r_*)^m\prod_iA_b(f_i)\). Since \(m^m\le e^m m!\), this has the stated form. Sum over the independent links. Repeated observables receive distinct labels. Finally \(\mathbb E(G+3/2)^2=21/2\), so (4.179) bounds each conditional variance by \((21/2)A_b^2\). Independence and the zero conditional mean prove (4.177). ∎

**Scope of the gain.** This proves cutoff-uniform first-layer scalar-score innovation estimates, all conditional orders, and a fixed conditional complex source neighborhood. The bounds retain the actual original Wilson action and arbitrary exterior. No reflection positivity, spectral gap, convexity, common background saddle, or source-free partition estimate was assumed. For the ordinary P2 insertion \(\sum f s_p\), divide \(Y_f\) by \(\beta_a\).

**What remains after conditioning.** The exact variance decomposition is

\[
\operatorname{Var}(J_f)
=\mathbb E\operatorname{Var}(J_f\mid\mathcal E)
 +\operatorname{Var}(\mathbb E[J_f\mid\mathcal E]).
\tag{4.181; P}
\]

Only the first term has been bounded. Even with a constant profile on a star, its conditional mean contains \(\tau(6-\varrho_b)\), the exterior frustration floor. It is a nonconstant function of the physical exterior. It cannot be thrown away as a scalar source-only vacuum counterterm. The theorem also does not claim an extensive all-order *unconditional* cumulant bound: averaging the conditional logarithms is not taking the logarithm of the averaged generating function. Iterating to the next RG scale requires control of the predictable effective interaction and every inherited source member. That is exactly where the remaining R1/R2 work lies.
