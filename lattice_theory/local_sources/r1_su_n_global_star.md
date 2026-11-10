# Scalar-source bounds for a Wilson link in SU(N)

**Status: proved finite integration theorem; full R1 remains open.**

## 1. Target, relationship to the companion notes, and scope

This note proves an actual, uniformly normalized first integration of six independently sourced Wilson plaquettes for every fixed SU(N), N≥2. The exterior links may be arbitrary real group elements. The coupling may be any β≥β_min>0. After subtracting the same source-dependent flat-star vacuum, the remaining source logarithm is bounded by the actual minimum star energy. The source-free effective action controls that minimum energy uniformly. Consequently a sufficiently small physical source preserves the first-layer large-field suppression, with constants independent of the torus and of the number of integrated links.

The exact object is a compact one-link integral, not a substitute independent-link model: every Wilson plaquette containing that link enters with its actual staple and actual source value. A family of links with no common plaquette gives the corresponding exact first-layer statement by conditional factorization.

The proof uses the fixed-patch, jointly holomorphic Laplace theorem already proved in [Inherited interactions in the second integration](r2_second_integration.md), §§5–7, only in its d=0 case. In that case the integration manifold is SU(N), its flat phase is 6a(U), and its flat Hessian is 6 times the identity. Section 3 below states precisely the consequences used and verifies this dictionary. No multiscale admission theorem, inherited-source bound, or unproved R1/R2 conclusion is assumed. The bounded-coupling part of the result is proved here by an exact Haar Ward identity, and the nonregular real exteriors are included by Hölder's inequality, compactness, and a direct flat lower bound.

The companion note [Spatial sources and field-dependent contacts](r1_spatial_source_integration.md) supplies a closed SU(2) formula, its fixed complex regular domain, exact contact coefficients, and an example showing why a source disk proportional to the coupling cannot cover all real exteriors. The present note extends the global real-exterior conclusion to every SU(N) and every β≥β_min. The second-patch theorem of [Inherited interactions in the second integration](r2_second_integration.md) treats an actual inherited interaction on a regular exterior domain; it is not silently extended here to all compulsory histories.

All displays below are proved statements, tagged **P**, except the final explicitly open obligation. Constants may depend on N and β_min. They never depend on a, T, a particular exterior configuration, or the number of disjoint stars.

## 2. Definitions and the global theorem

Use precisely the preamble's Wilson plaquette, with its literal coupling and physical scalar source:

\[
 s(P)=N-\operatorname{Re}\operatorname{Tr}P
      =\tfrac12\|P-I\|_{\rm HS}^2,\qquad
 0\le s(P)\le2N,\qquad \beta=\beta_a,\quad z_i=j^{(0)}(x_{p_i}).
 \tag{G1; P}
\]

At a link, orient the six incident plaquettes so that their actions are s(UV_i), with the actual exterior staples V_i∈SU(N). Inversion does not change s. Set v=(V_1,…,V_6), and let 0 denote the flat choice V_i=I. Define

\[
 \begin{aligned}
 Z_\beta(v;z)&=\int_{SU(N)}
   \exp\!\left[-\sum_{i=1}^6(\beta-z_i)s(UV_i)\right]dU,\\
 W(v)&=\min_{U\in SU(N)}\sum_{i=1}^6s(UV_i),\\
 \Gamma_\beta(v)&=\log Z_\beta(0;0)-\log Z_\beta(v;0),\\
 L_\beta(z)&=\log\frac{Z_\beta(0;z)}{Z_\beta(0;0)},\\
 \Phi_\beta(z;v)&=\log\frac{Z_\beta(v;z)}{Z_\beta(v;0)}-L_\beta(z).
 \end{aligned}
 \tag{G2; P: definitions of actual integrals and their normalized logarithms}
\]

The source logarithms use the branch equal to zero at z=0; its existence on the domain stated below is part of the proof. In particular the full mass Z_β(v;0), which may be very small, remains in the normalization. No lower bound independent of v and β is substituted for it.

**Theorem 2.1 (P: global first-integration source admission).** Fix N≥2 and β_min>0. There exist δ>0 and finite constants c,C>0, depending only on N and β_min, such that the following assertions hold for every β≥β_min and every real v∈SU(N)^6:

\[
 c\beta W(v)\le\Gamma_\beta(v)\le\beta W(v).
 \tag{G3; P}
\]

The function Φ_β is holomorphic in the six independent complex source values on the fixed physical-source ball ∥z∥₁<δ, and

\[
 |\Phi_\beta(z;v)|\le C W(v)\|z\|_1,\qquad
 |D^m\Phi_\beta(0;v)[f^1,\ldots,f^m]|
   \le m!C^{m+1}W(v)\prod_{r=1}^m\|f^r\|_\infty
 \quad(m\ge1).
 \tag{G4; P}
\]

Consequently the flat-normalized actual kernel satisfies

\[
 \left|\frac{Z_\beta(v;z)}{Z_\beta(0;z)}\right|
    =|e^{-\Gamma_\beta(v)+\Phi_\beta(z;v)}|
    \le\exp\{-[c\beta-C\|z\|_1]W(v)\}.
 \tag{G5; P}
\]

For a fixed smaller source ball with C∥z∥₁≤cβ_min/2 this retains at least cβW(v)/2 of the effective energy. The theorem asserts a fixed absolute source radius at arbitrary real exteriors. It makes no assertion of a radius proportional to β there; that stronger assertion already fails in the explicit SU(2) example in the companion note.

## 3. The checked regular-neighborhood input

Haar invariance replaces U by UV_1 and hence replaces the staples by V_1^{-1}V_i. On a fixed regular neighborhood put V_1^{-1}V_i=e^{X_i}, X_1=0. The real X_i belong to su(N); the complex continuation belongs to sl(N,ℂ). The holomorphic Wilson function is

\[
 s^{\rm hol}(P)=N-\tfrac12\operatorname{Tr}(P+P^{-1}),\qquad
 \phi_{w,X}(U)=\sum_{i=1}^6w_i s^{\rm hol}(Ue^{X_i}).
 \tag{G6; P}
\]

It agrees with (G1) on SU(N). At X=0 and w near 1 its critical point is I and, in the metric ⟨A,B⟩=−Tr(AB) on su(N), its Hessian is (Σ_iw_i)I. The flat real phase has a unique minimum and a strictly positive gap outside any fixed identity neighborhood. Thus the implicit-function, holomorphic Haar-centering, coercivity, and Laplace arguments of [Inherited interactions in the second integration](r2_second_integration.md), §§5.1, 6.1 and 7.1–7.2, apply to this one-link integral with d=0. The conversion from that note is a=s/N and τ=Nβ; its normalized source is Nz, so w=1−z/β in both conventions.

For completeness, the exact conclusion needed here is the following. On fixed complex neighborhoods ∥X∥<ε, ∥w−1∥∞<ε, and a fixed sector about the positive β axis with |β|≥B, let

\[
 \Gamma_\beta(w,X)=
    \log\int e^{-\beta\phi_{w,0}(U)}dU
       -\log\int e^{-\beta\phi_{w,X}(U)}dU.
 \tag{G7; P}
\]

With branches continued from the real flat integral, the proved regular-patch theorem gives

\[
 \Gamma_\beta(w,X)=\beta F(w,X)+D(w,X)+E_\beta(w,X),
 \qquad
 |F|+|D|\le C\|X\|^2,\qquad
 |E_\beta|\le C\|X\|^2/|\beta|.
 \tag{G8; P: fixed-patch Laplace theorem with the preceding dictionary}
\]

The estimates hold also for fixed-margin w derivatives. For real regular fields and w=1, F(1,X)=W(v). The determinant term D has degree zero in w, and F has degree one.

The field-quadratic factors in (G8) are essential. They follow because each scalar term is invariant under simultaneous color conjugation, vanishes at X=0, and has zero first X derivative there: an invariant linear form on sl(N,ℂ) vanishes. Uniform holomorphic bounds then give the quadratic factor by Taylor's formula. The basic Laplace remainder is O(β^{-1}); centering the compact integral is exact, the even Haar Jacobian and odd cubic phase cancel its possible β^{-1/2} term, and the fixed-domain Cauchy estimate preserves the color-invariant quadratic vanishing. These are the proved steps in the cited internal lemma, rather than an assumed asymptotic expansion without parameter control.

The real field norm and the actual minimum energy are comparable in this chart. Indeed, if U_* is any minimizer and P_i=U_*V_i, then each s(P_i)≤W and

\[
 \|V_1^{-1}V_i-I\|_{\rm HS}
   =\|P_1^{-1}P_i-I\|_{\rm HS}
   \le\sqrt{2s(P_1)}+\sqrt{2s(P_i)}.
 \tag{G9; P}
\]

For W small this places all relative staples in the logarithm chart and gives ∥X∥²≤CW. Conversely, choosing U=V_1^{-1} in the minimization gives W≤C∥X∥². In particular a sufficiently small fixed W-neighborhood lies inside the regular chart; every real configuration outside that neighborhood has W≥w_0>0.

For β≥B, (G8) and (G9) imply, uniformly in that real regular neighborhood,

\[
 |\Gamma_\beta(v)-\beta W(v)|\le CW(v),\qquad
 |\Phi_\beta(z;v)|\le CW(v)\|z\|_1
       \quad(\|z\|_\infty<c_0\beta).
 \tag{G10; P}
\]

For the second assertion use exactly Φ_β(z;v)=Γ_β(1,X)−Γ_β(1−z/β,X), and apply the fixed-margin w derivative bounds in (G8). The corresponding complex-exterior bound uses ∥X∥²; W(v) is used only on the real slice. This distinction prevents cancellation among complex curvature components from invalidating the estimate.

## 4. Exact positivity, sharp upper bound, and the bounded-coupling Hessian

Write H(U)=Re Tr U and let μ_t be normalized Haar measure tilted by e^{tH(U)}. Set

\[
 J(t)=\int e^{tH(U)}dU,\qquad
 m(t)=\frac{J'(t)}{NJ(t)},\qquad
 \mathbb E_{\mu_t}U=m(t)I,\qquad
 m'(t)=\operatorname{Var}_{\mu_t}(H)/N>0.
 \tag{G11; P}
\]

Conjugation invariance makes the matrix expectation scalar, and inversion makes it real. Haar expectation of U is zero, so m(0)=0. The real continuous function H is nonconstant, and the tilted density is strictly positive, proving the strict variance assertion. Thus 0<m(t)<1 for t>0.

Hölder's inequality applied to the six positive functions f_i(U)=e^{-βs(UV_i)} gives Z_β(v;0)≤Z_β(0;0), because their sixth-power integrals are identical by Haar invariance. Equality forces the six normalized sixth powers to coincide. They have the same integral, so f_i=f_j everywhere. At U=V_i^{-1} this says s(V_i^{-1}V_j)=0 and hence V_i=V_j. Therefore

\[
 \Gamma_\beta(v)\ge0,\qquad
 \Gamma_\beta(v)=0\ \Longleftrightarrow\ W(v)=0
    \ \Longleftrightarrow\ V_1=\cdots=V_6
       \quad(\beta>0).
 \tag{G12; P}
\]

There is also a sharp upper bound valid without any regularity assumption. Choose a minimizer U_*, put B=U_*Σ_iV_i, and change U=QU_* in the star integral. Since Re Tr B=6N−W,

\[
 \frac{Z_\beta(v;0)}{Z_\beta(0;0)}
  =\mathbb E_{\mu_{6\beta}}
       e^{\beta\operatorname{Re}\operatorname{Tr}(Q(B-6I))}
  \ge e^{-\beta m(6\beta)W(v)},\qquad
 \Gamma_\beta(v)\le\beta m(6\beta)W(v)\le\beta W(v).
 \tag{G13; P}
\]

The inequality is Jensen's inequality. No positivity or special polar form of the matrix B is required.

For the lower bound near common staples at bounded β, we calculate the exact transverse Hessian. For X∈su(N), right invariance of Haar measure makes ∫e^{t Re Tr(Ue^{εX})}dU independent of ε. Its second derivative at zero, together with (G11), yields

\[
 \mathbb E_{\mu_t}\operatorname{Re}\operatorname{Tr}(UX)=0,\qquad
 \mathbb E_{\mu_t}
   [(\operatorname{Re}\operatorname{Tr}(UX))
    (\operatorname{Re}\operatorname{Tr}(UY))]
       =\frac{m(t)}t\langle X,Y\rangle,
 \qquad \langle X,Y\rangle=-\operatorname{Tr}(XY).
 \tag{G14; P}
\]

The second identity follows first for X=Y and then by polarization. In detail, the second derivative before polarization is
t E Re Tr(UX²)+t² E(Re Tr UX)²=0, and the first expectation is −m(t)∥X∥².

Apply this identity at t=6β to the second derivative of log Z_β(e^{εX_1},…,e^{εX_6};0). If X̄=Σ_iX_i/6, the result is

\[
 \left.\frac{d^2}{d\varepsilon^2}
   \Gamma_\beta(e^{\varepsilon X_1},\ldots,e^{\varepsilon X_6})
       \right|_{\varepsilon=0}
     =\beta m(6\beta)\sum_{i=1}^6\|X_i-\bar X\|^2.
 \tag{G15; P}
\]

Indeed the direct second derivative of the phase contributes −βm(6β)Σ_i∥X_i∥² to log Z, and its variance contributes βm(6β)∥Σ_iX_i∥²/6. The sign reverses for Γ. The first derivative vanishes.

The actual minimization has the same transverse quadratic form: minimizing the quadratic phase ½Σ_i∥A+X_i∥² over A gives A=−X̄. The regular implicit-function theorem therefore gives

\[
 \begin{aligned}
 \Gamma_\beta(e^{X_1},\ldots,e^{X_6})
   &=\frac{\beta m(6\beta)}2
       \sum_i\|X_i-\bar X\|^2+O_{\beta_{\min},B}(\|X\|^3),\\
 W(e^{X_1},\ldots,e^{X_6})
   &=\frac12\sum_i\|X_i-\bar X\|^2+O(\|X\|^3)
       \qquad(\beta\in[\beta_{\min},B]).
 \end{aligned}
 \tag{G16; P}
\]

Here ∥X∥²=Σ_i∥X_i∥². In the relative chart X_1=0, the quadratic form Σ_i∥X_i−X̄∥² is at least ∥X∥²/6. On every fixed compact positive β interval, m(6β) has a positive lower bound and the Taylor remainders are uniform. Hence, after choosing a small chart depending on that interval, Γ_β(v)≥cβW(v). This is a genuine positive quadratic coefficient; strict positivity away from W=0 alone would not have justified a uniform ratio as W tends to zero.

## 5. Completion of the global energy comparison

First fix the regular chart in §3, and choose w_0>0 such that W≤w_0 implies membership in a smaller chart. For all sufficiently large β, (G10) gives Γ_β≥βW/2 on this set.

For its complement we need only two direct integral estimates. The star action is at least W. In a fixed exponential chart about I, the flat phase 6s(e^A) is at most C∥A∥², and normalized Haar density is bounded below. Integration over ∥A∥≤cβ^{-1/2} gives, with d_A=N²−1,

\[
 Z_\beta(v;0)\le e^{-\beta W(v)},\qquad
 Z_\beta(0;0)\ge c_1\beta^{-d_A/2}\quad(\beta\ge1),\qquad
 \Gamma_\beta(v)\ge\beta W(v)-\frac{d_A}{2}\log\beta-C_1.
 \tag{G17; P}
\]

Because W≥w_0 on this complement, the last two losses are at most βW/2 once β exceeds a fixed B. Thus Γ_β≥βW/2 for every real exterior and every β≥B.

It remains to treat β∈[β_min,B]. The precise bounded-coupling Hessian (G16) gives Γ_β≥c_2βW uniformly when W≤w_1, for a sufficiently small w_1>0. On the compact set β∈[β_min,B], v∈SU(N)^6, W(v)≥w_1, the continuous ratio Γ_β(v)/(βW(v)) is strictly positive by (G12). It has a positive minimum c_3. Combining these three regions yields the lower inequality in (G3), with c=min(1/2,c_2,c_3). The upper inequality is the exact Jensen bound (G13).

There is no circular choice of constants: choose the original regular chart and w_0 first, then B for the large-β argument, then the smaller w_1 for the compact interval. The large-β proof continues to use the original w_0. Neither B nor either chart depends on the exterior or on the lattice size.

## 6. A fixed physical-source disk on every real exterior

This proof retains the actual conditional law, including its full mass. With respect to the probability density e^{-βΣ_is(UV_i)}/Z_β(v;0), put M_β(z;v)=E exp(Σ_iz_is(UV_i)). The boundedness in (G1) gives

\[
 |M_\beta(z;v)-1|\le e^{2N\|z\|_1}-1.
 \tag{G18; P}
\]

Choose δ_0>0 with e^{4Nδ_0}−1<1/2. Then M_β(z;v), and its flat counterpart, lie in the disk |M−1|<1/2 for ∥z∥₁<2δ_0, for all β>0 and all real v. Their logarithms are single-valued and uniformly bounded there. More precisely,

\[
 |\log M_\beta(z;v)|+|\log M_\beta(z;0)|
      \le C_N\|z\|_1.
 \tag{G19; P}
\]

This elementary zero-free argument alone gives a constant bound; it does not yet give the energy factor W. We establish that factor near W=0 and then use the crude bound only where W is bounded below.

For β≥B and regular v, (G10) supplies |Φ_β|≤CW∥z∥₁ on a fixed source disk, after decreasing δ_0 if necessary. For β∈[β_min,B], choose a small fixed complex relative-staple chart X. The flat denominator Z_β(0;0) has a positive minimum on this compact β interval. The flat source ratios on ∥z∥₁<2δ_0 are bounded away from zero by (G18). Uniform continuity of the compact integrals in X therefore supplies a fixed smaller complex X-neighborhood on which the actual ratios and their logarithms are jointly holomorphic in z and X, with uniform bounds.

For every such z, Φ_β(z;0)=0. Simultaneous color conjugation of X leaves Φ_β invariant. Its linear derivative in any one X_i at X=0 is consequently an invariant linear form on sl(N,ℂ), and it vanishes. To see the last assertion directly, invariance implies that the linear form vanishes on every commutator; those commutators span sl(N,ℂ). Uniform Taylor estimates in X, followed by a source Cauchy estimate on the doubled disk and the identity Φ_β(0;X)=0, give

\[
 |\Phi_\beta(z;X)|\le C\|X\|^2\|z\|_1
       \quad(\beta\in[\beta_{\min},B])
 \tag{G20; P}
\]

on fixed smaller domains. For real fields in this chart, (G9) replaces ∥X∥² by CW. Choose w_2>0 small enough that W<w_2 places the real exterior in the required chart for both β ranges. Thus the desired energy-sensitive estimate holds when W<w_2. If W≥w_2, subtract the two logarithms in (G19) and use 1≤W/w_2. This proves the first assertion of (G4) everywhere, uniformly for β≥β_min.

For its derivative assertion use a fixed six-dimensional source polydisc contained in ∥z∥₁<δ. Coordinate Cauchy estimates give factorial bounds, and the at most 6^m terms in an m-linear directional derivative are absorbed in C^{m+1}. This proves the stated estimate for every m≥1. Inserting the first bound of (G4) and the lower bound of (G3) into the exact identity in (G5) completes Theorem 2.1. ∎

The argument gives analyticity in the physical source at every real exterior. Only the regular portion supplies a uniform complex field neighborhood. Source analyticity and field analyticity are distinct requirements; the theorem does not replace one by the other.

## 7. The exact first layer, its vacuum, and its retained energy

Let I be any set of lattice links such that no plaquette contains two members of I. Condition on all links outside I. Every incident plaquette then belongs to exactly one integrated star, and each staple is a function only of retained links. Denote by P_ext the plaquettes containing no member of I. Exact conditional integration gives

\[
 \begin{aligned}
 Z_{\Lambda,\beta}[z]
  &=[Z_\beta(0;0)]^{|I|}
      e^{\sum_{b\in I}L_\beta(z_b)}\\
  &\quad\times\int
      e^{-\sum_{p\in P_{\rm ext}}(\beta-z_p)s_p}
      \prod_{b\in I}
        e^{-\Gamma_\beta(v_b)+\Phi_\beta(z_b;v_b)}
           \prod_{e\notin I}dU_e .
 \end{aligned}
 \tag{G21; P: exact full-mass first-layer identity}
\]

The six entries of z_b are the source values of that star's actual plaquettes. No common-source replacement is made. The formula works on every compatible torus and for every allowed choice of I; possible coincidences among retained staple links do not affect conditional factorization.

The vacuum L_β(z_b) is deterministic, analytic on the fixed source disk, invariant under permutations of the six entries, and independent of the exterior and the torus. Scalar lattice reflections merely permute its literal plaquette-indexed arguments. This assertion does not silently identify that array transformation with reflection of a lower-vertex-sampled continuum profile; the latter requires the separately specified source-anchor convention. This is a proved single-star local vacuum. It is not yet the all-scale cell functional L_a required by N1-S(ii).

Choose r>0 so that 6r<δ, 6Cr≤cβ_min/2, and r≤β_min/2. If |z_p|≤r, then the modulus of the retained integrand in (G21) is bounded by

\[
 \exp\!\left[-\frac\beta2\sum_{p\in P_{\rm ext}}s_p
              -\frac{c\beta}2\sum_{b\in I}W(v_b)\right].
 \tag{G22; P}
\]

This is an actual paid energy bound after the entire first layer, valid at all real retained configurations. Any additional nonnegative factor depending only on the retained links can multiply both sides before integration. A factor depending on one of the integrated links changes its conditional law and is not covered by this assertion.

Along the allowed trajectory, N2-F gives g_0≤γ and hence β_a=2Ng_0^{-2}≥2Nγ^{-2}. Thus one may take β_min=2Nγ^{-2} in this first-layer theorem. No strengthening of N2-F and no smaller terminal-coupling hypothesis is needed for (G21)–(G22). The tensor/clover sector and the old source already carried through later transformations remain separate obligations.

## 8. The next actual transition and the remaining R1 boundary

The first-layer estimate does not make the next conditional law Wilson. For a retained link c, let I_c be the old stars whose staples depend on c. Up to the factors already independent of U_c, the next exact kernel is

\[
 \mathcal K_{c,\beta}[z](v)=\int_{SU(N)}
   e^{-\sum_{p\in P_{\rm ext}:\,c\in p}(\beta-z_p)s_p(U_c,v)}
   \prod_{b\in I_c}
      e^{-\Gamma_\beta(v_b(U_c,v))
          +\Phi_\beta(z_b;v_b(U_c,v))}\,dU_c.
 \tag{G23; P: exact next conditional kernel}
\]

Its normalization is the full value K_{c,β}[0](v). Each old Φ is the same inherited function of U_c that was created by (G21). Replacing these terms by fresh centered plaquette marks would change the kernel. The regular finite-patch result in [Inherited interactions in the second integration](r2_second_integration.md) does integrate this sort of inherited source by reopening its actual finite joint patch. The resulting regular theorem has a fixed dimension, a fixed positive Hessian gap, and a fixed complex exterior domain.

**Open requirement (O–R1–global-history):** prove that the actual source-carrying constrained transformations and R/B histories admit the required marked analytic norm uniformly in their length, while retaining their original source readouts, compulsory-event masses, gauge constraints, and endpoint layers. One must identify and subtract the complete identity and dimension-four projections of the resulting field-valued contacts, and then prove the claimed uniform remainder bounds on the same histories and analytic domains. The real bound (G22) does not itself supply those complex norm or projection statements. The next kernel (G23) locates where an iteration begins; Balaban's actual constrained block transition requires its own checked correspondence.

The theorem is nevertheless stronger than a bare bounded-observable estimate. It divides by the actual mass, subtracts a concrete local source vacuum, preserves the actual six independent source values, and produces an energy-sensitive bound at every real exterior. The bound is uniform for all β≥β_min, rather than only asymptotically large β. Its large-β regular part uses the proved fixed-patch Laplace theorem; its bounded-β part uses an explicitly positive transverse Haar-Ward coefficient. Exact Hölder and Jensen estimates control the zero set and the sharp upper energy comparison, while the nonregular region retains a positive energy lower bound. These ingredients also yield an exact torus-independent first-layer suppression theorem with no small-field assumption on retained configurations.

What remains is the uniform multiscale propagation of this information, not the existence of the first local source logarithm or the handling of its small conditional mass. No conclusion in this note labels full R1, full R2, N1-S, or the Yang–Mills existence target as proved. The result is a concrete completed component to be combined with the separate first inherited regular-patch theorem and the Gaussian locality work.
