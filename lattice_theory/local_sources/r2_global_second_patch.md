# Second Wilson integration on all real exterior data

## 1. Definitions, normalization and the completed theorem

**Status: P for the fixed finite patch specified here; full R2 remains O.** This note extends the regular second-integration theorem in [Inherited interactions in the second integration](r2_second_integration.md) to every real exterior configuration. It retains the actual first-layer marginal and its source readout. Its constants are uniform in the exterior, the lattice spacing and the torus, but the number of integrated links is bounded by seven. No assertion about arbitrary renormalization histories is made.

Let G=SU(N), N≥2, with normalized Haar measure and normalized trace tr=Tr/N. For a plaquette matrix P, use the nonnegative normalized action a(P). Its relation to the literal Wilson conventions is

\[
 a(P)=1-\operatorname{Re}\operatorname{tr}P\in[0,2],\qquad
 s(P)=Na(P),\qquad \tau=N\beta_a,\qquad z_p=Nj_p.
 \tag{G2.1; P: normalization}
\]

The matrix norm below is the normalized Hilbert–Schmidt norm, so that ‖P−I‖²=2a(P) on G. We consider a four-dimensional periodic lattice with at least three sites per side. This includes the finest lattice of every compatible torus in the question when K≥1. The two-site periodic lattice is excluded because two distinct links can then share more than one plaquette.

Start with a plaquette-disjoint first family of integrated links: no plaquette contains two of them. Choose a retained link e. Let b₁,…,b_d be the members of that first family sharing a plaquette with e. The periodic size condition implies that each shares exactly one plaquette; thus 0≤d≤6. The patch F consists of e and these d links. Its affected plaquettes P(F) have cardinality M=6+5d. There are 6−d plaquettes containing only e from F, five containing only each b_i, and one shared by e and each b_i. All other links are fixed at their arbitrary real exterior values v.

Write U_F for the internal links and define the exact joint kernel, its minimum energy, and its flat comparison:

\[
 \begin{split}
 S_v(U_F)&=\sum_{p\in P(F)}a(P_p(U_F;v)),\\
 m(v)&=\min_{U_F\in G^{d+1}}S_v(U_F)\in[0,2M],\\
 Z_v(\tau,\mathbf z)&=\int_{G^{d+1}}
   \exp\!\left[-\tau S_v(U_F)+\sum_{p\in P(F)}z_pa(P_p(U_F;v))\right]dU_F.
 \end{split}
 \tag{G2.2; P: exact definitions}
\]

The flat kernel Z₀ is this same integral with all exterior links equal to the identity. Source labels stay attached to the same plaquettes. Let D=(d+1)(N²−1) and ν=D/2. Define the deterministic flat vacuum L, the source-zero energy cost Γ, and the flat-subtracted source logarithm Φ by

\[
 \begin{split}
 L_\tau(\mathbf z)&=\log\frac{Z_0(\tau,\mathbf z)}{Z_0(\tau,\mathbf0)},\\
 \Gamma_\tau(v)&=\log\frac{Z_0(\tau,\mathbf0)}{Z_v(\tau,\mathbf0)},\\
 \Phi_\tau(\mathbf z;v)&=\log\frac{Z_v(\tau,\mathbf z)}{Z_v(\tau,\mathbf0)}-L_\tau(\mathbf z).
 \end{split}
 \tag{G2.3; P: exact definitions; analytic logarithms normalized at zero}
\]

**Theorem 1.1 — P.** There exist τ_*≥1, r_*>0 and C<∞, depending only on N and the bounded patch types d=0,…,6, such that for every real exterior v, every τ≥τ_* and every complex source array with ‖z‖₁≤r_*,

\[
 \frac12\tau m(v)\le\Gamma_\tau(v)\le2\tau m(v),\qquad
 |\Phi_\tau(\mathbf z;v)|\le C m(v)\|\mathbf z\|_1.
 \tag{G2.4; P}
\]

The logarithms are holomorphic on the larger source ball ‖z‖₁<2r_*. Their branches vanish at zero. Consequently the source retains a definite part of the actual patch energy suppression:

\[
 \left|e^{-L_\tau(\mathbf z)}
       \frac{Z_v(\tau,\mathbf z)}{Z_0(\tau,\mathbf0)}\right|
 \le\exp\!\left[-\left(\frac\tau2-C\|\mathbf z\|_1\right)m(v)\right].
 \tag{G2.5; P}
\]

This is an estimate of the exact two-stage kernel, since integrating the d leaves first and then e is exactly the same joint integral by Fubini. Section 4 identifies the inherited source and its second vacuum subtraction explicitly. The theorem includes nonregular and frustrated real exteriors. Its source radius there is a fixed absolute physical radius; it does not assert a radius proportional to τ or a complex continuation of those nonregular exterior fields.

The proof has two regimes. Small m permits a source-independent exact change of internal variables that turns every plaquette defect into a small coefficient of the same flat star. Its size is controlled by m, so the proved regular Laplace expansion applies. Away from small m, uniform upper Hessian bounds at an arbitrary compact minimum and a fixed absolute source disk suffice. No positive lower Hessian at a frustrated minimum is needed.

## 2. An exact acyclic normal form at a minimizing configuration

**Lemma 2.1 — P.** For every real exterior choose any minimizing internal configuration U_F^*. There is a product-Haar-preserving transformation of the internal variables, independent of the source array, which writes every affected plaquette action in the following form:

\[
 \widetilde S_{\mathbf B}(Q,Q_1,\ldots,Q_d)
 =\sum_{p\in H}a(QB_p)
  +\sum_{i=1}^d\sum_{p\in A_i}a(Q_iB_p)
  +\sum_{i=1}^d a(QQ_i^{-1}B_{s_i}).
 \tag{G2.6; P}
\]

Here H is the set of 6−d hub-only plaquettes, A_i the five leaf-only plaquettes of b_i, and s_i its one shared plaquette. Each B_p is a unitary conjugate of the original minimizing plaquette P_p(U_F^*;v), or of its inverse. At the transformed identity configuration the phase is at its minimum, and

\[
 \widetilde S_{\mathbf B}(\mathbf1)=\sum_p a(B_p)=m(v),
 \qquad
 \min_{Q,Q_1,\ldots,Q_d}\widetilde S_{\mathbf B}=m(v).
 \tag{G2.7; P}
\]

The equality holds plaquette by plaquette with all original labels, and therefore also holds with arbitrary independent real or complex coefficients multiplying those actions.

**Proof.** Denote the hub by U and leaf i by V_i. Cyclicity of trace and a(P)=a(P⁻¹) allow each shared plaquette to be written as a(U A V_i^σ B), where σ is either +1 or −1 and A,B are products of exterior links. Put U=Q U^* and V_i=R_i V_i^*. These translations preserve Haar measure. For σ=+1 define T_i=U^*A and P^*=U^*A V_i^*B. For σ=−1 define T_i=U^*A V_i^{*-1} and P^*=T_iB. In both cases the shared plaquette has the exact form

\[
 a(UAV_i^\sigma B)
 =a(QT_iR_i^\sigma T_i^{-1}P^*)
 =a(QQ_i^{-1}P^*),
 \qquad Q_i=(T_iR_i^\sigma T_i^{-1})^{-1}.
 \tag{G2.8; P}
\]

Conjugation and inversion preserve Haar measure on a compact group. These changes can be made independently for the d leaves because no plaquette contains two leaves and each leaf has exactly one shared plaquette. This is where the acyclic star geometry is used.

Before rebasing, write each leaf-only plaquette as a(V_iC_p) using cyclicity and, when required, inversion. After rebasing it becomes a(R_iD_p), with D_p=V_i^*C_p. Since R_i=T_i⁻¹Q_i^−σT_i, cyclicity gives a(Q_i^−σ T_iD_pT_i⁻¹). If σ=−1 this already has the required form. If σ=+1, inversion followed by cyclicity changes it to a(Q_i(T_iD_pT_i⁻¹)⁻¹). Thus its B_p is respectively T_iD_pT_i⁻¹ or its inverse. It is a conjugate, or inverse conjugate, of the original minimizing plaquette. A hub-only plaquette is similarly a(U C_p)=a(Q U^*C_p), with B_p=U^*C_p. The shared coefficient is exactly P^* in (G2.8).

At Q=Q_i=I the original internal links are precisely U_F^*. Every term therefore has the original minimizing action. Product Haar invariance and bijectivity preserve the whole integral and its minimum. This proves all assertions. ∎

The minimizing configuration is selected at source zero and every rebase and conjugation is then held fixed during source variations. No derivative of a minimizer, measurable selection of a minimizer, or global uniqueness of that minimizer is used. All estimates below are pointwise in the exterior and depend only on m(v). The function m is continuous, because it is the minimum over a fixed compact set of a jointly continuous function.

**Corollary 2.2 — P.** There are ε₀>0 and C<∞ depending only on N such that, whenever m(v)≤ε₀, all normal-form coefficients have principal logarithms b_p∈su(N) and

\[
 B_p=e^{b_p},\qquad
 \|\mathbf b\|^2:=\sum_p\|b_p\|^2\le C m(v).
 \tag{G2.9; P}
\]

If m(v)=0, the entire kernel including every independent source equals its flat counterpart.

**Proof.** The identity ‖B_p−I‖²=2a(B_p), nonnegativity, and (G2.7) put every B_p in a fixed identity neighborhood for ε₀ small. The principal matrix logarithm is analytic there with a uniform Lipschitz bound in the normalized Hilbert–Schmidt norm. Shrinking ε₀ with N ensures that the sum of the principal eigenangles has absolute value below 2π; it is therefore zero, so b_p is traceless as well as anti-Hermitian. Summing ‖b_p‖²≤C‖B_p−I‖² gives (G2.9). If m=0, every a(B_p) vanishes, hence every B_p=I. Formula (G2.6), with its unchanged source labels, is then exactly the flat phase. ∎

For completeness, the flat phase appearing in this normal form is the one used in the regular second-integration theorem:

\[
 S_{\rm flat}(Q,Q_1,\ldots,Q_d)
 =(6-d)a(Q)+\sum_{i=1}^d\bigl[5a(Q_i)+a(QQ_i^{-1})\bigr].
 \tag{G2.10; P}
\]

Its Hessian at the identity is N²−1 copies of 6I−Adj(star_d), in an orthonormal Lie-algebra basis for −tr(XY). Its smallest eigenvalue is at least 6−√6. The normalized Hilbert–Schmidt triangle inequality gives a(Q)≤2a(Q_i)+2a(QQ_i⁻¹), and a(QQ_i⁻¹)≤2a(Q)+2a(Q_i). Consequently

\[
 \frac12\left[a(Q)+\sum_i a(Q_i)\right]
 \le S_{\rm flat}(Q,Q_1,\ldots,Q_d)
 \le12\left[a(Q)+\sum_i a(Q_i)\right].
 \tag{G2.11; P}
\]

For d≤5 the lower bound already follows from the singleton terms. For d=6, use one of the six shared terms with the first triangle inequality and retain the remaining five-unit leaf weights; the coefficient 1/2 is then valid for the hub and every leaf. The upper bound follows by summing the second triangle inequality. These facts verify a unique flat minimum, a positive local Hessian, and a uniform gap away from its identity neighborhood for every patch type, including d=6.

## 3. Proof of the all-real partition and source bounds

### 3.1 Verification of the regular coefficient family

We apply the finite compact-patch Laplace module proved in §§5–7 of [Inherited interactions in the second integration](r2_second_integration.md), with the coefficient tuple b from (G2.9) as its parameters. Here is the verification, including the analytic facts needed for this application. Extend a to SL(N,C) as a^hol(P)=1−[tr(P)+tr(P⁻¹)]/2. In (G2.6) replace B_p by e^{b_p}, and give the plaquette terms independent weights w_p near one. The resulting phase S_{w,b} is holomorphic in the finite tuple (w,b). At b=0 and real positive w near one it has the same unique minimum Q=1 and a uniformly positive Hessian. The fixed flat gap and uniform C² perturbation bound persist for small real b. The implicit-function theorem therefore gives a unique nearby minimum and a holomorphic critical point Q_*(w,b) on a fixed complex neighborhood.

For real parameters, translate each integration variable by its component of Q_*. Haar invariance gives an exact centered integral. Both sides are holomorphic in (w,b), so the identity extends to complex parameters by the identity theorem on the real form. The centered action F_{w,b} has value and first derivative zero at the identity. Its difference from S_flat is uniformly O(‖w−1‖+‖b‖) in C². Taylor's formula near the identity and the compact positive gap elsewhere give the global estimate

\[
 |F_{w,\mathbf b}(Q)-S_{\rm flat}(Q)|
 \le C(\|w-\mathbf1\|+\|\mathbf b\|)
                 \sum_{\ell\in F}a(Q_\ell).
 \tag{G2.12; P}
\]

Thus Re(ζF_{w,b}) dominates a positive multiple of |ζ|Σa(Q_ℓ) on a fixed right sector, after the parameter neighborhoods are made small. This controls the whole real compact integration manifold, including the region outside the local chart.

In an identity exponential chart the centered action is its positive quadratic form plus a homogeneous cubic polynomial and an O(|x|⁴) remainder. The Haar density is analytic, positive at zero, and even. Integrate on a symmetric small coordinate ball. The cubic first correction integrates to zero against the even complex Gaussian. The remaining errors are bounded by a slightly weakened Gaussian times a fixed sum of |x|², |ζ||x|⁴ and |ζ|²|x|⁶. Their integrals are O(|ζ|⁻¹) relative to the leading Gaussian integral. The complement has an exponential bound from (G2.12). This proves a uniform holomorphic expansion with a relative error smaller than 1/2 when |ζ| is large. Taking its logarithm is therefore justified. Cauchy's inequalities on larger fixed parameter neighborhoods and coefficient sectors give all derivatives used below. This is the same argument as the companion module, and none of its hypotheses has been inferred from the smallness of a source.

In particular, for real τ≥τ_reg and fixed complex neighborhoods of w=1 and b=0,

\[
 Z_\tau(w,\mathbf b)
 =e^{-\tau E(w,\mathbf b)}\tau^{-\nu}
                 A(w,\mathbf b)e^{\rho(w,\mathbf b,\tau)},\qquad
 |\rho(w,\mathbf b,\tau)|\le C/\tau,\qquad |A(w,\mathbf b)|\ge c>0.
 \tag{G2.13; P}
\]

All logarithms are continued from the real flat point. Set D(w,b)=log A(w,b)−log A(w,0) and R(w,b,τ)=ρ(w,b,τ)−ρ(w,0,τ). Simultaneously conjugating every b_p and every internal variable leaves the phase and Haar integral invariant. The critical energy, Gaussian determinant and logarithmic remainder inherit this invariance. Each first b derivative at zero is therefore an invariant linear functional on a copy of sl(N,C), and is zero: sl(N,C) has no nonzero functional invariant under all SU(N) conjugations. Since E(w,0)=D(w,0)=R(w,0,τ)=0, Taylor's formula and the fixed-domain Cauchy bounds imply

\[
 |E(w,\mathbf b)|+|D(w,\mathbf b)|\le C\|\mathbf b\|^2,\qquad
 |R(w,\mathbf b,\tau)|\le C\|\mathbf b\|^2/\tau.
 \tag{G2.14; P}
\]

The same bounds hold for first w derivatives on a smaller fixed neighborhood. The companion proof also gives higher derivatives, but only the first are needed here. This verifies the module for the normal-form coefficients themselves; it is not necessary to realize an arbitrary independent tuple B_p as the boundary links of a new lattice.

Choose ε₀ in Corollary 2.2 smaller if needed so that every tuple produced by m≤ε₀ lies in that inner parameter neighborhood. The critical energy at w=1 is exactly m, since the transformed identity is a global minimum. Substitution into (G2.13) gives

\[
 \Gamma_\tau(v)=\tau m(v)-D(\mathbf1,\mathbf b)
                                  -R(\mathbf1,\mathbf b,\tau),
 \qquad |\Gamma_\tau(v)-\tau m(v)|\le C_{\rm reg}m(v)
 \quad(m(v)\le\varepsilon_0).
 \tag{G2.15; P}
\]

For sources put w=1−z/τ. Taking the exact source ratio and subtracting the flat ratio yields

\[
 \begin{split}
 \Phi_\tau(\mathbf z;v)
 &=\tau[E(\mathbf1,\mathbf b)-E(\mathbf1-\mathbf z/\tau,\mathbf b)]\\
 &\quad+D(\mathbf1-\mathbf z/\tau,\mathbf b)-D(\mathbf1,\mathbf b)\\
 &\quad+R(\mathbf1-\mathbf z/\tau,\mathbf b,\tau)-R(\mathbf1,\mathbf b,\tau).
 \end{split}
 \tag{G2.16; P on the small-minimum-energy domain}
\]

The first-weight derivative bounds, (G2.9), and integration on the straight segment between the two weight arrays prove |Φ|≤C_reg m‖z‖₁, as long as that segment lies in the inner weight neighborhood. A fixed disk ‖z‖₁≤2r_* satisfies this for all sufficiently large τ. The coordinate change and the tuple b remain fixed throughout this computation.

### 3.2 Uniform partition bounds away from small minimum energy

For arbitrary real v, the action S_v has uniformly bounded second derivatives on the compact group G^{d+1}: it is a sum of at most 36 fixed-length Wilson words with unitary exterior coefficients. Choose any minimum U_F^*. Its first derivative is zero. Uniform Taylor bounds in a translated identity chart therefore imply S_v(U_F^* exp X)≤m(v)+C‖X‖² for ‖X‖ below a fixed radius. The normalized Haar measure of a ball of radius cτ⁻¹ᐟ² is at least c'τ⁻ν. Integrating on this ball gives the lower bound below. The upper bound uses S_v≥m and total Haar mass one:

\[
 c_1\tau^{-\nu}e^{-\tau m(v)}
 \le Z_v(\tau,\mathbf0)\le e^{-\tau m(v)}
 \qquad(\tau\ge1).
 \tag{G2.17; P}
\]

This argument uses an upper bound on the Hessian, which holds at every compact minimum, including degenerate ones. It requires neither uniqueness nor a lower Hessian bound at an arbitrary exterior.

At the flat exterior the proved regular Laplace expansion, with its nonzero Gaussian determinant, gives c₀τ⁻ν≤Z₀(τ,0)≤C₀τ⁻ν for τ≥τ_reg. Combining these estimates gives

\[
 \tau m(v)-\nu\log\tau-C_{\rm gap}
 \le \Gamma_\tau(v)\le\tau m(v)+C_{\rm gap},
 \tag{G2.18; P}
\]

where C_gap can be chosen to dominate both −log c₀ and log(C₀/c₁), as well as zero. Take the largest such constant and ν_max over the seven patch types. There exists τ_* such that for every τ≥τ_*,

\[
 \tau\ge 2C_{\rm reg},\qquad
 \nu_{\max}\log\tau+C_{\rm gap}\le\frac{\varepsilon_0\tau}{2}.
 \tag{G2.19; P: an admissible threshold choice}
\]

Increase τ_* also to meet τ_reg and the inner weight-neighborhood requirement after (G2.16). If m≤ε₀, (G2.15) proves the first inequality of Theorem 1.1 with the claimed upper bound. If m≥ε₀, (G2.18)–(G2.19) do so. In the case m=0 the exact flat-kernel identity of Corollary 2.2 applies. This proves the energy estimate for all real exteriors.

### 3.3 A fixed absolute source disk at every real exterior

Let μ_{v,τ} be the normalized positive patch measure at source zero, and write G_v(z)=Z_v(τ,z)/Z_v(τ,0). Since every a_p lies in [0,2], the exponential series gives the following bound uniformly in τ and v:

\[
 |G_v(\mathbf z)-1|
 \le e^{2\|\mathbf z\|_1}-1.
 \tag{G2.20; P}
\]

Choose r_*=1/32 in normalized source units. On ‖z‖₁<2r_*=1/16, the right side is less than 1/4. Thus G_v has a single holomorphic logarithm vanishing at zero on this whole ball. The logarithm power series also gives |log G_v(z)|≤4‖z‖₁; the same applies to G₀. Consequently |Φ|≤8‖z‖₁ there, which is at most (8/ε₀)m(v)‖z‖₁ when m≥ε₀. When m≤ε₀, (G2.16) gives the sharper energy-charged estimate. The branches in the two proofs agree at zero and hence agree everywhere on their common disk.

This proves the source estimate of Theorem 1.1, with C=max(C_reg,8/ε₀) after enlargement if needed. All constants and thresholds depend only on N and the finite patch types. The source reserve (G2.5) follows from the exact identity exp(−L)Z_v/Z₀=exp(−Γ+Φ). ∎

## 4. The inherited source, source jets and the exact remaining scope

### 4.1 All source derivatives and the common-source refinement

Let f₁,…,f_q be arbitrary plaquette arrays on P(F). The source logarithm is holomorphic on a fixed absolute ball, is zero at the origin and obeys (G2.4). Multivariable Cauchy estimates therefore give

\[
 \left|\partial_{t_1}\cdots\partial_{t_q}
   \Phi_\tau\!\left(\sum_{i=1}^q t_if_i;v\right)\bigg|_{t=0}\right|
 \le q!\,C_{\rm jet}^{\,q}\,m(v)\prod_{i=1}^q\|f_i\|_1
 \qquad(q\ge1).
 \tag{G2.21; P}
\]

Indeed, if all the norms are nonzero, use radii r_*/(2q‖f_i‖₁) for the q scalar variables. Their polydisc maps into the source ball of radius r_*/2. Cauchy's formula bounds the mixed derivative by C m(r_*/2)(2q/r_*)^q times the product of those norms. The elementary bound q^q≤e^q q! absorbs the remaining factors into C_jet^q. A zero direction makes the derivative zero. Constants are independent of q except for the displayed factorial and exponential factors.

There is a stronger bound when the exterior has small minimum energy and all affected plaquettes receive the same normalized source t. Common scaling of all weights leaves the critical configuration unchanged, scales its energy by the same factor, and changes the determinant by the common factor t_scale^−ν. This cancels in D. The exact expansion also gives R(t_scale w,b,τ)=R(w,b,t_scale τ). Increase τ_* by a fixed factor if necessary so that τ−t remains beyond the Laplace threshold when |t|≤cτ. Then coefficient-sector Cauchy estimates from the proof of (G2.13) give

\[
 \Phi_\tau(t\mathbf1;v)
 =t\,m(v)+R(\mathbf1,\mathbf b,\tau-t)-R(\mathbf1,\mathbf b,\tau),
 \qquad
 |\Phi_\tau(t\mathbf1;v)-t\,m(v)|
       \le C|t|m(v)\tau^{-2}
 \quad(m(v)\le\varepsilon_0,\ |t|\le c\tau).
 \tag{G2.22; P}
\]

on an inner fixed coefficient sector. Here c>0 is independent of the exterior and τ. The same argument gives higher t derivatives of the remainder bounded by q!C^{q+1}m(v)τ^−q−1. This refinement applies whenever the patch minimum is small, even if its original exterior links were far from the identity; the exact normal form supplies the admitted coefficient chart.

### 4.2 Identification with the true first-layer marginal

Partition P(F) into P_rem, the 6−d hub-only plaquettes, and the disjoint six-plaquette sets P_i belonging to the first-integrated leaves. Let K_i(U;z_i) be the exact integral over the leaf V_i with U and v fixed, retaining all its six Wilson terms and their sources. Let K_i^flat(z_i) denote its flat-star version, with U and all exterior links set to I. Define

\[
 L_i(\mathbf z_i)=\log\frac{K_i^{\rm flat}(\mathbf z_i)}
                                  {K_i^{\rm flat}(\mathbf0)},\qquad
 \phi_i(\mathbf z_i;U,v)
  =\log\frac{K_i(U;\mathbf z_i)}{K_i(U;\mathbf0)}-L_i(\mathbf z_i).
 \tag{G2.23; P: literal first-layer source and its flat vacuum}
\]

The same raw bounded-action estimate as (G2.20) makes these logarithms holomorphic on the required absolute source disk for every real U,v. Their presence is mandatory: they are the actual non-Wilson source readouts produced by the first integration.

Let S_rem be the sum of a_p over P_rem. The genuine reduced hub law and its inherited source are

\[
 \begin{split}
 d\mu_{{\rm red},\tau,v}(U)
  &=Z_v(\tau,\mathbf0)^{-1}
       e^{-\tau S_{\rm rem}(U;v)}
          \prod_{i=1}^dK_i(U;\mathbf0)\,dU,\\
 \Psi_\tau(\mathbf z;U,v)
  &=\sum_{p\in P_{\rm rem}}z_pa_p(U;v)
                            +\sum_{i=1}^d\phi_i(\mathbf z_i;U,v).
 \end{split}
 \tag{G2.24; P}
\]

The first line is normalized by the actual joint integral, not by a substituted Wilson law. Multiplication of its integrand by exp Ψ replaces each old kernel K_i(U;0) by its sourced kernel K_i(U;z_i), along with the explicit first flat vacuum. Fubini therefore gives the exact identity

\[
 \mathbb E_{\mu_{{\rm red},\tau,v}}e^{\Psi_\tau}
 =e^{-\sum_iL_i(\mathbf z_i)}
                       \frac{Z_v(\tau,\mathbf z)}{Z_v(\tau,\mathbf0)}.
 \tag{G2.25; P}
\]

Its right side is zero-free on the stated source ball, so its logarithm is the analytic one starting at zero. The deterministic second-step subtraction is precisely

\[
 L_{2,\tau,F}(\mathbf z)=L_\tau(\mathbf z)-\sum_iL_i(\mathbf z_i),
 \qquad
 \log\mathbb E_{\mu_{{\rm red},\tau,v}}e^{\Psi_\tau}
      -L_{2,\tau,F}(\mathbf z)=\Phi_\tau(\mathbf z;v).
 \tag{G2.26; P}
\]

Thus (G2.4), (G2.21) and the energy reserve (G2.5) hold for this actual second integration under every real exterior. None of its inherited masses was removed. The subtraction counts each first vacuum exactly once.

### 4.3 Integration under any positive true outer law

Let λ(dv) be any positive source-independent measure on arbitrary real exteriors, with 0<∫Z_v(τ,0)λ(dv)<∞. Every factor depending on an integrated link must already be in Z_v; factors genuinely independent of F may be included in λ. Put dν_λ(v)=Z_v(τ,0)λ(dv)/∫Z_v(τ,0)λ(dv). Then

\[
 e^{-L_\tau(\mathbf z)}
 \frac{\int Z_v(\tau,\mathbf z)\lambda(dv)}
      {\int Z_v(\tau,\mathbf0)\lambda(dv)}
 =\mathbb E_{\nu_\lambda}e^{\Phi_\tau(\mathbf z;v)},\qquad
 \left|\mathbb E_{\nu_\lambda}e^\Phi\right|
 \le\mathbb E_{\nu_\lambda}e^{C\|\mathbf z\|_1m(v)}
 \le e^{2MC\|\mathbf z\|_1}.
 \tag{G2.27; P}
\]

This removes the regular-support restriction in the companion theorem for these actual finite patches. Its first bound preserves the actual exterior energy variable and the actual exterior law. The final coarser bound is a finite-patch bound and should not be multiplied over all fine-lattice anchors when a physical-volume bound is required.

### 4.4 What has and has not been completed

**Completed — P.** For every SU(N) and every real exterior, the fixed actual second patch has a deterministic flat vacuum, a positive suppression comparable to τ times its minimum energy at sufficiently large τ, a uniform absolute complex source disk, all source jets charged to that energy, and exact compatibility with the inherited first-layer source. The exact transformation to a small coefficient tuple when the minimum energy is small is the step that extends the regular result beyond exteriors whose original links lie in one identity chart.

**Still open — O, full R2.** This does not establish a uniformly admitted representation for arbitrary histories of effective interactions, compulsory large-field selectors, earlier source jets and their actual component masses. A hard internal selector can exclude the minimum used in (G2.17); a general inherited internal activity need not be a uniformly analytic amplitude or reduce to this fixed star phase. Such factors cannot be reassigned to λ if they still depend on F. Iterated integration can also create cyclic interaction graphs and unbounded patch sizes, for which the finite normal form and its dimension-dependent constants here are insufficient.

**Still open — O, assembly into N1-S.** The actual next output is the non-Wilson kernel Z_v, together with Φ and the old exterior masses. A complete argument must admit that kernel at every scale, prove the normalized compulsory-history comparison with all those masses, establish local vacuum copying and its summable errors, and show that the final count is proportional to N_T rather than the number of fine patches. The all-real theorem above does not supply that count or identify the final reference measure and the terminal pointwise upper/lower bounds.

There are no literature imports or assumed coupling-flow statements in this note. Its finite-dimensional analytic module is proved in [Inherited interactions in the second integration](r2_second_integration.md) and verified for the present coefficient family in §3.1; its group identities, geometric restriction and compact-minimum estimates are proved here. It is therefore an independently usable completed module, with its precise finite-patch scope exposed.
