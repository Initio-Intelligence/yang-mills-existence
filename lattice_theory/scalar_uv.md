# Scalar ultraviolet coefficients and three-point functions

## 1. Scope, conventions, and the obstruction this calculation resolves

This note proves the complete separated-point Gaussian coefficient calculation for the dimension-four scalar curvature square. It also identifies the first nonzero *formal perturbative* Yang–Mills OPE coefficient from a checked primary source. It does not assert that the nonperturbative Wilson lattice measures have these asymptotics, or that a pure phase inherits them. Those are separate estimates, stated precisely below.

Use \(d_A=N^2-1\), real Lie algebra components normalized by Hermitian generators \(\operatorname{Tr}(T^aT^b)=\tfrac12\delta^{ab}\), and independent two-form indices \(I=(\mu,\nu)\) with \(\mu<\nu\). Let \(q>0\). The free gauge potential has Feynman-gauge covariance

\[
\langle A_\mu^a(x)A_\nu^b(y)\rangle_0
=q\,\delta^{ab}\delta_{\mu\nu}D(x-y),\qquad
D(z)=\frac{1}{4\pi^2|z|^2},\qquad
F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a.
\tag{UV.1; P: definition}
\]

The curvature correlators are independent of the pure-gradient part of a covariant-gauge propagator. All formulas below concern distinct insertion points; distributional contact terms on diagonals are excluded. The scalar conventions are

\[
S(x)=\sum_{a=1}^{d_A}\sum_{\mu<\nu}:F_{\mu\nu}^a(x)^2:,
\qquad
\mathcal F(x)=\sum_{a,\mu,\nu}:F_{\mu\nu}^a(x)^2:=2S(x).
\tag{UV.2; P: definition}
\]

Thus, with an ordered sum over Lorentz indices, \(\operatorname{Tr}F_{\mu\nu}F_{\mu\nu}=S\) in the Hermitian component convention, and \(2\operatorname{Tr}F_{\mu\nu}F_{\mu\nu}=\mathcal F\). These equalities must not be confused with an anti-Hermitian matrix convention, in which a minus sign accompanies the matrix trace.

The essential correction is that the Gaussian connected scalar three-point coefficient is zero. A nonzero Yang–Mills three-point coefficient must be established at the first interaction order. Consequently, an error estimate merely tending to zero relative to the Gaussian scale does not suffice for R6.

## 2. Exact Gaussian coefficient theorem and proof

**Theorem UV.1 (P).** At distinct points, the fields in (UV.1)–(UV.2) satisfy

\[
\langle S(x)S(y)\rangle_{0,c}
=\frac{12d_Aq^2}{\pi^4|x-y|^8},
\qquad
\langle\mathcal F(x)\mathcal F(y)\rangle_{0,c}
=\frac{48d_Aq^2}{\pi^4|x-y|^8}.
\tag{UV.3; P}
\]

Every odd connected correlator of \(S\), of order at least three, vanishes at separated points. In particular,

\[
\langle S(x_1)S(x_2)S(x_3)\rangle_{0,c}
=\langle\mathcal F(x_1)\mathcal F(x_2)\mathcal F(x_3)\rangle_{0,c}=0.
\tag{UV.4; P}
\]

This assertion is about the scalar contraction; it does not assert vanishing for arbitrary tensor contractions of three curvature-square operators.

**Proof.** For \(z\ne0\), put \(n=z/|z|\), \(I(z)=\mathbf1-2n\otimes n\), and let \(R(z)=\Lambda^2I(z)\) act on the six-dimensional real two-form space with orthonormal basis indexed by \(\mu<\nu\). Direct differentiation gives

\[
\partial_\mu\partial_\rho D(z)
=-\frac{\delta_{\mu\rho}}{2\pi^2|z|^4}
+\frac{2z_\mu z_\rho}{\pi^2|z|^6},
\quad
\langle F_{\mu\nu}^a(x)F_{\rho\sigma}^b(y)\rangle_0
=\delta^{ab}\frac{q}{\pi^2|z|^4}
\bigl(I_{\mu\rho}I_{\nu\sigma}-I_{\mu\sigma}I_{\nu\rho}\bigr).
\tag{UV.5; P}
\]

For clarity, the four derivative terms in the last covariance are
\(-\delta_{\nu\sigma}\partial_\mu\partial_\rho D
+\delta_{\nu\rho}\partial_\mu\partial_\sigma D
+\delta_{\mu\sigma}\partial_\nu\partial_\rho D
-\delta_{\mu\rho}\partial_\nu\partial_\sigma D\), multiplied by \(q\delta^{ab}\).
This establishes both the factor and the sign in (UV.5). Thus the one-color covariance matrix on independent two-form components is

\[
C(z)=\frac{q}{\pi^2|z|^4}R(z),
\qquad R(z)^{\mathsf T}=R(z),\qquad R(z)^2=\mathbf1,
\qquad \operatorname{tr}_{\Lambda^2}\mathbf1=6.
\tag{UV.6; P}
\]

Wick contraction supplies two ways to join the two quadratic vertices. Color conservation along the connected graph gives one factor \(d_A\). Therefore

\[
\kappa_2(S(x),S(y))
=2d_A\operatorname{tr}_{\Lambda^2}\bigl(C(x-y)C(y-x)\bigr)
=2d_A\frac{q^2}{\pi^4|x-y|^8}\,6.
\tag{UV.7; P}
\]

This proves (UV.3). For the three vertices the connected contractions form one triangle, and there are eight choices of the two half-edges at the vertices:

\[
\kappa_3(S(x_1),S(x_2),S(x_3))
=8d_A\operatorname{tr}_{\Lambda^2}(C_{12}C_{23}C_{31}),
\qquad C_{ij}=C(x_i-x_j).
\tag{UV.8; P}
\]

Let \(J=*\) be the Euclidean Hodge operator on two-forms. It satisfies \(J^2=\mathbf1\). For any orthogonal map \(M\) on \(\mathbb R^4\), the definition of the Hodge operator by the oriented volume form gives

\[
J(\Lambda^2M)=\det(M)(\Lambda^2M)J.
\tag{UV.9; P}
\]

Each \(I(z)\) is a reflection and has determinant \(-1\). Hence \(JC(z)J=-C(z)\). Conjugating a product of \(n\) such covariance matrices by \(J\) changes it by \((-1)^n\). For odd \(n\), invariance of trace under conjugation consequently gives

\[
\operatorname{tr}_{\Lambda^2}(C_{i_1i_2}\cdots C_{i_ni_1})
=\operatorname{tr}_{\Lambda^2}\bigl(JC_{i_1i_2}\cdots C_{i_ni_1}J\bigr)
=-\operatorname{tr}_{\Lambda^2}(C_{i_1i_2}\cdots C_{i_ni_1})=0.
\tag{UV.10; P}
\]

At any order \(n\ge2\), a connected Wick graph of quadratic vertices is a cycle. Summing cycles yields the explicit identity

\[
\kappa_n(S(x_1),\ldots,S(x_n))
=2^{n-1}d_A
\sum_{\sigma\in\mathfrak S(\{2,\ldots,n\})}
\operatorname{tr}_{\Lambda^2}
\bigl(C_{1,\sigma(2)}C_{\sigma(2),\sigma(3)}
\cdots C_{\sigma(n),1}\bigr).
\tag{UV.11; P}
\]

For \(n=2\) it has the coefficient \(2\), and for \(n=3\) the two reverse cycles give the coefficient \(8\) in (UV.8). Each trace in (UV.11) vanishes for odd \(n\). This proves the theorem. Normal ordering removes self-contractions; no assertion here assigns values to contact distributions on the diagonals. \(\square\)

**Corollary UV.2 (P).** If \(f_1,f_2,f_3\) are smooth test functions with pairwise disjoint compact supports, the Gaussian mixed third derivative of the connected scalar generating functional is zero. Subtracting any counterterm supported on coincident insertion points cannot change this conclusion.

**Proof.** The smeared connected third derivative is the integral of (UV.4). A contact distribution has support in a union of partial diagonals, disjoint from the product of the three supports. \(\square\)

## 3. The first interaction coefficient: what is established perturbatively

Write \(u=g_{\rm YM}\) for the conventional canonical Yang–Mills coupling and \(g_{\rm tH}=\sqrt N\,u\). The canonical action is \(\tfrac14\int \mathcal F\), with \(F=dA+u[A,A]\), so the free covariance parameter in §2 is \(q=1\). In pure \(SU(N)\) Yang–Mills theory the standard formal one-loop beta function is

\[
\mu\frac{du}{d\mu}=-b_u u^3+O_{\rm formal}(u^5),
\quad b_u=\frac{11N}{48\pi^2};
\qquad
\mu\frac{dg_{\rm tH}}{d\mu}
=-\beta_{\rm tH}g_{\rm tH}^3+O_{\rm formal}(g_{\rm tH}^5),
\quad \beta_{\rm tH}=\frac{11}{48\pi^2}.
\tag{UV.12; L: formal one-loop coefficient and P: change of variable}
\]

**Checked import UV-L1 (L, perturbative scope).** Becchetti and Bochicchio, *OPE and a low-energy theorem in QCD-like theories*, JHEP 03 (2019) 088, [arXiv:1810.08527](https://arxiv.org/pdf/1810.08527), printed pp.9–10, (3.4)–(3.7), use \(\mathcal F=2\operatorname{Tr}F^2\) and \(g_{\rm tH}^2=Nu^2\). Setting their \(N_f=0\), their scalar OPE coefficient at nonzero separation is

\[
C_{\mathcal F\mathcal F}^{\mathcal F}(x)
=\frac{4\beta_{\rm tH}g_{\rm tH}^2}{\pi^2|x|^4}
+O_{\rm formal}(g_{\rm tH}^4)
=\frac{4b_u u^2}{\pi^2|x|^4}+O_{\rm formal}(u^4).
\tag{UV.13; L}
\]

Their (3.6) separately includes a leading \(4\delta^{(4)}(x)\). This contact term is absent at separated points and cannot provide the nonzero triple required by R6. Their (3.5) gives the leading two-point coefficient \(48d_A/\pi^4\), independently reproduced by Theorem UV.1.

The momentum-space primary calculation is Zoller and Chetyrkin, *OPE of the energy-momentum tensor correlator in massless QCD*, JHEP 12 (2012) 119, [arXiv:1209.1516v3](https://arxiv.org/pdf/1209.1516), printed p.15, (4.24). Its \(O_1=-\mathcal F/4\), \(a_s=u^2/(4\pi^2)\), \(C_A=N\), \(l_{\mu q}=\log(\mu^2/Q^2)\) give, for \(N_f=0\),

\[
C_1^{GG}(Q)
=-1+a_s\left(-\frac{49}{36}N-\frac{11}{12}N\,l_{\mu q}\right)
+O_{\rm formal}(a_s^2).
\tag{UV.14; L}
\]

Changing from \(O_1\) to \(\mathcal F=-4O_1\) multiplies this OPE coefficient by \(-4\). The momentum-independent terms are contact terms. The inverse Fourier transform of the remaining logarithm verifies (UV.13), including its sign:

\[
\mathcal F^{-1}\!\left[\log\frac{\mu^2}{p^2}\right](x)
=\frac{1}{\pi^2|x|^4}\quad(x\ne0),
\qquad
\frac{11N}{3}a_s\,\frac{1}{\pi^2|x|^4}
=\frac{4b_u u^2}{\pi^2|x|^4}.
\tag{UV.15; P: Fourier transform and normalization conversion}
\]

To prove the transform, differentiate at \(\alpha=0\) the analytically continued Riesz-kernel identity

\[
\int\frac{d^4p}{(2\pi)^4}e^{ip\cdot x}
\left(\frac{\mu^2}{p^2}\right)^\alpha
=
\frac{\mu^{2\alpha}\Gamma(2-\alpha)}
{4^\alpha\pi^2\Gamma(\alpha)}
(x^2)^{\alpha-2}\quad(x\ne0).
\tag{UV.16; P}
\]

Its coefficient of \(\alpha\) is \((\pi^2|x|^4)^{-1}\); choices of extension at \(x=0\) alter only contact terms.

**Theorem UV.3 (P within the formal perturbative OPE, using UV-L1).** Let \([\cdot]_{u^2}\) denote coefficient extraction in the formal canonical-coupling expansion. Let the bar denote normalized spherical averaging over \(x=\varepsilon\omega\), \(\omega\in S^3\), and fix \(y\ne0\). The scalar dimension-four OPE channel gives

\[
\lim_{\varepsilon\downarrow0}
\varepsilon^4
\left[\overline{
\langle S(\varepsilon\omega)S(0)S(y)\rangle_{c}
}\right]_{u^2}
=\frac{24b_ud_A}{\pi^6|y|^8}
=\frac{11N(N^2-1)}{2\pi^8|y|^8}.
\tag{UV.17; P in formal perturbation theory}
\]

For \(\mathcal F=2S\), the corresponding coefficient is eight times larger:

\[
\lim_{\varepsilon\downarrow0}
\varepsilon^4
\left[\overline{
\langle\mathcal F(\varepsilon\omega)\mathcal F(0)\mathcal F(y)\rangle_{c}
}\right]_{u^2}
=\frac{192b_ud_A}{\pi^6|y|^8}
=\frac{44N(N^2-1)}{\pi^8|y|^8}.
\tag{UV.18; P in formal perturbation theory}
\]

**Proof.** Since \(S=\mathcal F/2\), the coefficient of \(S\) in the OPE \(SS\) is half of (UV.13), namely \(2b_u u^2/(\pi^2|x|^4)\). Multiply it by the Gaussian two-point function \(12d_A/(\pi^4|y|^8)\). There are no gauge-invariant operators of positive dimension below four in pure Yang–Mills theory. The identity contributes nothing to this connected triple. At dimension four, spherical averaging kills non-scalar irreducible tensor coefficients, while parity excludes the pseudoscalar. Derivative descendants and higher-dimensional terms have extra positive powers of \(\varepsilon\) after multiplication by \(\varepsilon^4\). BRST-exact and equation-of-motion terms do not contribute to separated gauge-invariant correlators. Thus the displayed scalar OPE channel gives precisely (UV.17). The factor of eight proves (UV.18). This is coefficient extraction in the renormalized formal OPE; it is not an exchange of a nonperturbative ultraviolet limit with an infinite perturbative series. \(\square\)

The nonzero coefficient (UV.17) is unaffected by a finite multiplicative field change \(S\mapsto(1+O(u^2))S\) or a coupling change \(u\mapsto u+O(u^3)\): both would first change a nonzero triple at order \(u^4\), because the order-zero triple vanishes.

**Conditional all-triangle formula (C).** If the order-\(u^2\) separated scalar triple satisfies the homogeneous conformal-primary Ward identities of dimension four, its unique three-point form and (UV.17) imply

\[
\langle S(x_1)S(x_2)S(x_3)\rangle_c
=\frac{11N(N^2-1)}{2\pi^8}
\frac{u^2}{|x_{12}|^4|x_{23}|^4|x_{31}|^4}
+O_{\rm formal}(u^4).
\tag{UV.19; C: stated conformal Ward hypothesis}
\]

This note does not replace that Ward-identity verification by an appeal to scale invariance. Bochicchio and Pallante, [arXiv:2402.16490v1](https://arxiv.org/pdf/2402.16490), printed pp.28–30, (6.11), (6.15), (6.24), use the corresponding conformal form and recover \(N_3/N_2=4\beta_{\rm tH}g_{\rm tH}^2/\pi^2\); their (6.11) is explicitly introduced as an ansatz. The unconditional new algebra here is Theorem UV.1; the imported one-loop scalar-channel coefficient is (UV.13); the full nonperturbative version of either (UV.17) or (UV.19) remains open.

## 4. Conversion to the literal P2 scalar source and beta-function variable

The P2 action uses the unnormalized fundamental trace. This changes the usual relation between the parameter called \(g_0\) in P2 and the conventional Yang–Mills coupling \(u\).

**Proposition UV.4 (P, classical and formal normalization).** Let a smooth continuum anti-Hermitian connection have curvature \(\mathscr G=iT^aG^a\), and use its link holonomies. Then

\[
s_{p_{\mu\nu}(x)}
=-\frac{a^4}{2}\operatorname{Tr}\mathscr G_{\mu\nu}(x)^2+o(a^4)
=\frac{a^4}{4}\sum_aG_{\mu\nu}^a(x)^2+o(a^4),
\qquad
O_a^{(0)}\longrightarrow\frac14\sum_{\mu<\nu,a}(G_{\mu\nu}^a)^2 .
\tag{UV.20; P: classical expansion}
\]

At a lower-vertex evaluation point the error need not start at \(a^6\); the leading equality is all that is used. With the canonical rescaling \(G=uF(A,u)\), matching the quadratic and interacting action to \(\tfrac14\int\mathcal F=\tfrac12\int S\) gives

\[
\frac{\beta_a}{4}u^2=\frac12,
\qquad
\beta_a=\frac2{u^2}=\frac{2N}{g_0^2},
\qquad
u^2=\frac{g_0^2}{N},
\qquad
g_0=g_{\rm tH},
\qquad
O_{\rm match}^{(0)}=\frac{u^2}{4}S
=\frac{g_0^2}{4N}S.
\tag{UV.21; P}
\]

The symbol \(O_{\rm match}^{(0)}\) denotes this formal canonical matching, not an already proved renormalized continuum limit of the bare lattice observable.

**Proof.** In the plaquette holonomy \(U_p=\mathbf1+a^2\mathscr G+O(a^3)\), the linear trace vanishes. The first real trace correction is \(a^4\operatorname{Tr}\mathscr G^2/2\). The trace convention gives \(\operatorname{Tr}\mathscr G^2=-\tfrac12\sum_a(G^a)^2\), proving (UV.20). Comparing the coefficient of \(\sum_{\mu<\nu,a}F^2\) proves (UV.21). \(\square\)

Consequently the formal P2 scalar two-point coefficient is

\[
\langle O_{\rm match}^{(0)}(x)O_{\rm match}^{(0)}(0)\rangle_c
=\frac{3(N^2-1)}{4N^2\pi^4}
\frac{g_0^4}{|x|^8}+O_{\rm formal}(g_0^6).
\tag{UV.22; P: conversion of UV.3}
\]

Its free third connected coefficient is zero. The first nonzero scalar-channel hierarchical coefficient is

\[
\lim_{r\downarrow0}r^4
\left[
\overline{\langle
O_{\rm match}^{(0)}(r\omega)
O_{\rm match}^{(0)}(0)
O_{\rm match}^{(0)}(y)
\rangle_c}
\right]_{g_0^8}
=\frac{11(N^2-1)}{128N^3\pi^8|y|^8}.
\tag{UV.23; P: formal conversion of UV.17}
\]

Indeed, three scalar marks contribute \((u^2/4)^3=u^6/64\), and (UV.17) supplies \(11Nd_Au^2/(2\pi^8)\). Their product is \(11Nd_Au^8/(128\pi^8)=11d_Ag_0^8/(128N^3\pi^8)\). Replacing the bare symbol by an actual running coupling and relating the lattice scalar to the canonically renormalized \(S\) requires the matching and running field-normalization theorem; (UV.22)–(UV.23) do not supply it.

There is also an exact normalization consequence for the provisional expected coefficient in N2-F. With the literal P2 action and the canonical convention just checked,

\[
x=g_0^{-2}=\frac1N u^{-2},
\qquad
\frac{dx}{d\log\mu}
=\frac{2b_u}{N}+O_{\rm formal}(x^{-1})
=\frac{11}{24\pi^2}+O_{\rm formal}(x^{-1}).
\tag{UV.24; P: conversion of the one-loop import}
\]

Thus coarse-graining by \(L\) gives the formal decrement \(-11\log L/(24\pi^2)\) in this \(x\). The value \(11N/(24\pi^2)\) belongs instead to \(u^{-2}\). This is the normalization clarification ICR-N1-1 of [lattice_conventions.md](lattice_conventions.md); it is not a new assumption about the actual N2-F remainder. If P2 were changed to the conventional normalized-plaquette Wilson action, the parameter conversion would change with it.

## 5. The exact nonperturbative comparison and phase transfer still required

The Gaussian theorem lives on \(\mathbb R^4\). Finite periodic volume, harmonic-mode conventions, lattice differentiation, and the actual Wilson interaction introduce errors. Their vanishing at the required rate is not part of Theorem UV.1.

To specify that rate, let \(u_\varepsilon\) be the conventional running coupling at physical scale \(\varepsilon\), tending to zero along the asymptotically free trajectory. Suppose that the full renormalization has identified a scalar normalization \(Z_{\varepsilon,a}\) for which

\[
\Phi_{\varepsilon,a,T}(x)
=\varepsilon^4 Z_{\varepsilon,a}
O_a^{(0)}(x_*+\varepsilon x)
\tag{UV.25; C: definition once actual field matching is constructed}
\]

has the canonical ultraviolet normalization \(S\) used above. The notation denotes rescaled distributions, not assumed pointwise fields. In particular, \(Z_{\varepsilon,a}\) includes the conversion \(4N/g_0^2\) at tree level and the actual running/matching factors; its cutoff dependence must be derived.

**Residual UV-R1 (O).** Prove, for each compact set \(Q\) of separated rescaled configurations, a fixed test seminorm \(p_Q\) and uniform estimates

\[
\begin{aligned}
\left|\langle G^{(2)}_{\varepsilon,a,T}-K_2,f\rangle\right|
&\le \delta_{2,Q}(\varepsilon,a/\varepsilon,\varepsilon/T)\,p_Q(f),\\
\left|\langle G^{(3)}_{\varepsilon,a,T}
-u_\varepsilon^2K_3,f\rangle\right|
&\le u_\varepsilon^2
\delta_{3,Q}(\varepsilon,a/\varepsilon,\varepsilon/T)\,p_Q(f),
\end{aligned}
\qquad
\delta_{m,Q}\longrightarrow0,
\tag{UV.26; O}
\]

where \(G^{(m)}\) are the connected correlators of (UV.25), \(K_2\) is (UV.3) with \(q=1\), and \(K_3\) has the nonzero scalar hierarchical coefficient (UV.17). One can replace the second line by a suitably smeared, spherically projected hierarchy estimate that directly targets (UV.17); a general all-triangle formula is not necessary for a *specified hierarchical coefficient*. If the target instead specifies the full triangle kernel, its perturbative identification must also be completed.

The limit in (UV.26) includes \(a/\varepsilon\to0\) and \(\varepsilon/T\to0\) on the selected cofinal family. Uniformity must include all small-field and retained/erased large-field histories after normalization, field/source Taylor remainders, local contact subtractions, boundary terms, and the actual source-renormalization factors. A formal series, a bound on \(\log Z\), and a Gaussian approximation with a bare \(o(1)\) error each leave this estimate unproved.

**Proposition UV.5 (P, sharpness of the required order).** An \(o(1)\) error at canonical three-point scale cannot establish the nonzero first interaction coefficient. An \(o(u_\varepsilon^2)\) error can.

**Proof.** Since the Gaussian target is zero, both \(G^{(3)}_\varepsilon=0\) and \(G^{(3)}_\varepsilon=u_\varepsilon^2K_3\), for any fixed nonzero test distribution \(K_3\), satisfy \(G^{(3)}_\varepsilon=o(1)\). Thus that information does not distinguish them. Dividing the second line of (UV.26) by \(u_\varepsilon^2\) instead gives convergence to the specified \(K_3\), which has a nonzero evaluation on an appropriate separated scalar-channel test family by (UV.17). \(\square\)

The sequential hierarchy can be stated without an unproved all-triangle formula. At fixed small \(h>0\), first establish the ultraviolet limit in the separated configuration \((h\omega,0,y)\); then take the spherical scalar projection and \(h\downarrow0\). The coefficient required is

\[
\lim_{h\downarrow0}h^4
\lim_{\varepsilon\downarrow0}
\frac{
\overline{G^{(3)}_{\varepsilon}(h\omega,0,y)}
}{u_\varepsilon^2}
=\frac{11N(N^2-1)}{2\pi^8|y|^8}.
\tag{UV.27; O: nonperturbative hierarchical target}
\]

Formula (UV.27) must be formulated with separated smearing unless smooth off-diagonal kernels have independently been proved. A simultaneous limit in \(h\) and \(\varepsilon\) requires additional uniform control over the two scales. No interchange is implicit here.

**Residual UV-R2 (O).** Transfer the two-point and first interaction coefficient to a selected pure component. In the existing phase decomposition, let \(\mathscr C_m^\varepsilon\) denote the central multiplication operators whose fibers are the *phasewise connected* correlators of the appropriately scaled fields. A sufficient strengthening of the central criterion of the phase-decomposition argument is

\[
\|\mathscr C_2^\varepsilon-K_2\mathbf1\|\longrightarrow0,
\qquad
\|u_\varepsilon^{-2}\mathscr C_3^\varepsilon-K_3\mathbf1\|
\longrightarrow0,
\tag{UV.28; C: sufficient phasewise comparison; O for the YM construction}
\]

uniformly in the relevant separated-test seminorms. The same assertion may be imposed only on the chosen scalar hierarchical test family if that is the specified target. Essential-supremum norm convergence yields the same law in almost every component; a countable dense test and scale family gives one common full-measure set, with distributional continuity extending the result. This is the direct-integral argument of the phase-decomposition step, with the indispensable factor \(u_\varepsilon^{-2}\).

For completeness, the need to control connected fibers follows algebraically from the law of total cumulance. For a mixture \(\rho=\int\rho_\alpha\,d\mu(\alpha)\), write \(m_\alpha(X)=\rho_\alpha(X)\). Then

\[
\begin{aligned}
\kappa_{3,\rho}(X,Y,Z)
={}&\int\kappa_{3,\rho_\alpha}(X,Y,Z)\,d\mu(\alpha)
+\kappa_{3,\mu}(m_\alpha(X),m_\alpha(Y),m_\alpha(Z))\\
&+\operatorname{Cov}_{\mu}
\bigl(m_\alpha(X),\kappa_{2,\rho_\alpha}(Y,Z)\bigr)
+\operatorname{Cov}_{\mu}
\bigl(m_\alpha(Y),\kappa_{2,\rho_\alpha}(X,Z)\bigr)\\
&+\operatorname{Cov}_{\mu}
\bigl(m_\alpha(Z),\kappa_{2,\rho_\alpha}(X,Y)\bigr).
\end{aligned}
\tag{UV.29; P}
\]

Expanding both sides into first, second, and third moments proves the identity. Hence a nonzero mixed-state triple alone does not identify a pure-component triple. Either (UV.28) or a direct phase-selection argument with the same interaction-order precision is needed.

Finally, contact invisibility means locality on partial diagonals. A functional local only to a fixed physical cell can have mixed derivatives at distinct points within that cell. Such cell locality alone does not justify ignoring its contribution to these coefficients. The revised contact-renormalization theorem must provide the actual support statement used in Corollary UV.2.

## 6. The free scalar is not a Gaussian field: a nonzero four-point check

**Corollary UV.6 (P).** Let \(t>0\), \(e\) be a unit vector, and \(x_i=(i-1)te\), \(i=1,2,3,4\). The connected free scalar four-point function is strictly positive; explicitly,

\[
\langle S(0)S(te)S(2te)S(3te)\rangle_{0,c}
=\frac{169}{108}\,
\frac{(N^2-1)q^4}{\pi^8t^{16}}.
\tag{UV.30; P}
\]

**Proof.** All six pair covariances have the same two-form reflection \(R=\Lambda^2(\mathbf1-2e\otimes e)\), multiplied by the positive number \(q/(\pi^2|x_i-x_j|^4)\). Since \(R^4=\mathbf1\), every four-cycle trace is \(6\). The six oriented cycles in (UV.11) form three reverse pairs. Their scalar denominators, after extracting \(t^{16}\), are \(81\), \(256\), and \(20736\). Thus

\[
\kappa_4
=\frac{96d_Aq^4}{\pi^8t^{16}}
\left(\frac1{81}+\frac1{256}+\frac1{20736}\right)
=\frac{169d_Aq^4}{108\pi^8t^{16}}.
\tag{UV.31; P}
\]

This proves the claim. \(\square\)

The free Maxwell *potential* is Gaussian, while its scalar curvature-square field is a quadratic composite and has nonzero connected four-point functions. Therefore the odd-cycle cancellation does not make \(S\) Gaussian. It also does not discharge P1's stipulated nonzero *interacting scalar three-point coefficient*; that remains the order-\(u^2\) target in (UV.17), with its nonperturbative and phasewise versions (UV.26)–(UV.28).
