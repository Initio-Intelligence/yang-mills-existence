# Energy, sources and the two integrated patches

## 4.35 Actual Wilson energy normalization and an averaged raw norm

The earlier same-exterior obstruction does not prevent a normalized estimate under the actual Wilson exterior law. The following theorem supplies that estimate for local energies and their weighted collections. Its complete proof, including the required even-block chessboard inequality, is in [Wilson normalization of local energy budgets](../energy_budgets.md), §§2–7. It uses only exact finite-lattice integrals and the numerical N2-F trajectory.

Write n=T/a, V=n⁴, d_A=N²−1, and let β_K mean the **bare** literal P2 coefficient at cutoff depth K. It is not the terminal effective coefficient. For each positive fine link b let S_b be the sum of its six unnormalized Wilson plaquette actions. There are constants κ,C>0, independent of K,T and the weights, such that

\[
 \log\mu_{n,\beta_K}
       \exp\!\left(\kappa\beta_K\sum_b w_bS_b\right)
       \le C\sum_bw_b,\qquad 0\le w_b\le1.
 \tag{4.223; P: actual normalized weighted-energy theorem}
\]

The constants depend only on the specified N2-F data and N,L,γ,g_*. The theorem applies on every compatible torus. It neither rescales the literal physical source by a⁴ nor identifies a renormalized insertion with a positive bare-energy budget.

**Proof of the actual normalization.** Put z(β)=∫e^{−βs(U)}dU. An identity chart, the exact relation s(U)=‖U−I‖²_HS/2 and the positive gap away from I give z(β) comparable to (1+β)⁻ᵈᴬᐟ². A spanning-tree gauge change leaves precisely 3V+1 free group coordinates. Restricting those coordinates to radius c(1+β)⁻¹ᐟ² costs exp(−CV)(1+β)⁻ᵈᴬ⁽³ⱽ⁺¹⁾ᐟ², while the restricted action costs only exp(−CV).

For the upper bound, select an exactly integrable plaquette forest. In dimension j, first retain wrapping (1,μ) plaquettes indexed by a tree on the n^{j−1} transverse vertices, then all open direction-1 plaquette chains, then recursively a forest in the first-coordinate-zero slice. Integrate wrapping tree leaves before the open chains. Every leaf or terminal chain variable gives exactly z(β), by Haar invariance, independently of the remaining coefficients. The count is r_j=(j−1)n^j−j+1, hence r_4=3V−3. Omitted plaquettes are nonnegative. Therefore

\[
 \begin{aligned}
 e^{-CV}(1+\beta)^{-d_A(3V+1)/2}
       &\le Z_n(\beta)\le z(\beta)^{3V-3},\\
 0\le\log\frac{Z_n((1-s)\beta)}{Z_n(\beta)}
       &\le C_{N,s}V+2d_A\log(1+\beta),
       \qquad 0<s<1.
 \end{aligned}
 \tag{4.224; P: exact forest/tree-gauge bounds}
\]

No discarded torus constraint is treated as an independent plaquette. Four free group degrees separate the two counts. N2-F (i)–(iii) imply β_K≤2N[g_*⁻²+K(b₀log L+C_rγ²)], while n≥2L^K. Thus the right side divided by V is uniformly bounded.

To localize this estimate, use site-plane reflection positivity with tangential boundary links shared and integrated once. Every plaquette lies in one closed half or in the boundary, so the reflected quadratic form is the integral of a squared modulus. For blocks of fine side b=L² and K≥2, the number of blocks per direction is even and a full link star fits strictly inside each block. Its disseminated copies have disjoint plaquette sets; their total action is at most S. The chessboard inequality holds for every even block count: normalize a finite list of observables by their fully disseminated expectations, take a maximizing coloring, and repeatedly reflect a maximizing half to double a run of equal slices. This produces a homogeneous maximizing coloring, whose normalized expectation is one. It proves the generalized inequality without a power-of-two assumption. The partition ratio then gives μ(e^{sβ_KS_b})≤e^{C_s} uniformly. K=0,1 follow from the bounded coefficient and compact action.

For arbitrary weights, partition positive links into the finitely many orientation/residue classes modulo 2b. Each class fits a translated canonical block array. Jensen controls a fractional weight, the generalized chessboard inequality handles the class, and Hölder combines the finitely many classes. Choosing κ smaller by that fixed number proves (4.223). All reflected observables are the actual star actions with the correct inverse-link convention. ∎

This argument resolves the averaged form of the ordinary-frustration counterexample in §4.23. Let W_b be the minimum of S_b over the active link with its exterior fixed. Then W_b is a literal gauge-invariant reflected star observable and 0≤W_b≤S_b. Under the actual exterior marginal,

\[
 \mu_{n,\beta_K}\{\beta_KW_b\ge u\}
      \le\min\{1,e^{C_s-su}\},\qquad u\ge0.
 \tag{4.225; P: true exterior-law suppression}
\]

There is also a direct SU(N) frustration estimate. If F_i, i=1,2,3, are the three opposite-plane-pair star forces, D=Σ_i|F_i|², P=|Σ_iF_i|² and ℓ=ΔS_b, define h_b=β(D−P/3) and r_b=βD−ℓ/3 with the Lie metric used in §4.23. Put A_i equal to each pair of unitary staples, A=Σ_iA_i and M=max_U ReTr(UA)=6N−W_b. Projection onto the Lie algebra and the three-vector variance identity give

\[
 0\le h_b
   =\frac\beta3\sum_{i<j}|F_i-F_j|^2
   \le4\beta W_b\le4\beta S_b,
 \qquad |r_b|\le4\beta S_b+2d_A.
 \tag{4.226; P}
\]

Indeed Σ_{i<j}|F_i−F_j|²≤3Σ_i‖A_i‖²_HS−‖A‖²_HS≤36N−M²/N=12W_b−W_b²/N. The exact compact-field estimate on ΔS_b proves the second inequality. Consequently h_b and |r_b| have uniform local exponential moments under the Wilson law. Their essential suprema at fixed exteriors can still grow with β_K. No marked ℓ² susceptibility or connected decay estimate follows merely from these one-root moments.

All bare clover directions admit the same actual majorant. Let J be the six-by-six symmetric matrix on independent antisymmetric pairs, so J_AB=4j^{μνρσ} in the ordered-index convention. The negative clover matrix is a Gram matrix and the four-plaquette average gives

\[
 |J:Q(x)|\le\frac{\|J\|_{\rm op}}4
          \sum_{b\ \mathrm{incident\ on}\ x}S_b,
 \quad
 \log\mu_{n,\beta_K}
  e^{\kappa\beta_K\sum_xw_x|J_x:Q(x)|}
       \le2C\sum_xw_x
 \quad(0\le w_x\le1,\ \|J_x\|_{\rm op}\le1).
 \tag{4.227; P}
\]

Every touching plaquette occurs twice among the eight incident stars, which fixes the factor. This controls bare tensors under the actual law; it is not their running tensor normalization or a collision prescription.

**A complete-kernel transport consequence.** For any complete normalized positive history kernel Q(dv|U), let μ̄=μQ and let ν_F be the signed pushforward of Fμ. Disintegration gives dν_F/dμ̄=E[F|v]. Therefore every p≥1 satisfies

\[
 \left\|\frac{d\nu_F}{d\bar\mu}\right\|_{L^p(\bar\mu)}
       \le\|F\|_{L^p(\mu)},\qquad
 |\nu_F|\le Q(|F|\mu),\qquad
 \int e^{\kappa\mathbb E[B\mid v]}d\bar\mu
       \le\mu(e^{\kappa B})\quad(B\ge0).
 \tag{4.228; P}
\]

For B_D=β_K(a/ℓ₀)⁴Σ_{start(b)∈D}S_b, where D is a union of physical cells, (4.223) gives μ(e^{κB_D})≤exp(4C|D|). Literal packets bounded by powers of B_D thus have a physical-cell factorial majorant which survives every complete positive pushforward. Rare label masses remain inside μ̄; they are never inverted independently.

This supplies a rigorous **averaged raw norm** for packets with that proved majorant. It does not identify the complete vacuum-subtracted physical source with B_D. Nor does it make point evaluation or complex-field differentiation continuous on an arbitrary real Lᵖ space. Conversion from a raw old kernel to an analytic current activity, and normalization after separately conditioning on a prescribed future event, remain distinct operations. These are the precise limitations to retain when using the new normalization theorem in R1/R2.

## 4.36 Global SU(N) first integration and spatial scalar source contacts

The first actual conditional integration is controlled on every real exterior for every SU(N), including small conditional masses. The full proof is in [Scalar-source bounds for a Wilson link in SU(N)](r1_su_n_global_star.md), §§2–7. The more explicit SU(2) spatial and field-contact calculation is in [Spatial sources and field-dependent contacts](r1_spatial_source_integration.md), §§2–7.

At a positive link orient its six plaquettes as s(UV_i), with real staples V_i∈SU(N). Use the literal P2 coefficient β and literal plaquette source values z_i. Define

\[
 \begin{aligned}
 Z_\beta(v;z)&=\int_{SU(N)}
     e^{-\sum_{i=1}^6(\beta-z_i)s(UV_i)}dU,\qquad
 W(v)=\min_U\sum_{i=1}^6s(UV_i),\\
 \Gamma_\beta(v)&=\log Z_\beta(0;0)-\log Z_\beta(v;0),\\
 L_\beta(z)&=\log\frac{Z_\beta(0;z)}{Z_\beta(0;0)},\qquad
 \Phi_\beta(z;v)=\log\frac{Z_\beta(v;z)}{Z_\beta(v;0)}-L_\beta(z).
 \end{aligned}
 \tag{4.229; P: actual source, mass and deterministic flat vacuum}
\]

Here 0 means all staples equal I. The logarithmic branches start at z=0; their uniform domain is proved below.

**Theorem (P).** For every β_min>0, there are c,C,δ>0 depending only on N,β_min such that, for every β≥β_min and every real v,

\[
 c\beta W(v)\le\Gamma_\beta(v)\le\beta W(v),\qquad
 |\Phi_\beta(z;v)|\le CW(v)\|z\|_1
       \quad(\|z\|_1<\delta).
 \tag{4.230; P: global first-star energy and source estimate}
\]

The source logarithm is holomorphic on that fixed physical-source ball. Its m-th derivative is bounded by m!C^{m+1}W(v) times the product of the directional supremum norms, for every m≥1. The constants do not depend on the exterior, coupling above β_min, lattice or torus.

**Proof.** Generalized Hölder bounds the star integral by the flat integral. Equality forces the six normalized factors e^{−βs(UV_i)} to coincide; their equal Haar integrals and their values at U=V_i⁻¹ then imply V_1=⋯=V_6. Thus Γ≥0 with exactly the same zero set as W.

For the sharp upper bound choose a minimizing U_* and put B=U_*Σ_iV_i. With respect to the central flat law proportional to exp(6β ReTr Q), its mean is m(6β)I, where 0<m(t)≤1 for t>0. Jensen gives Z_β(v;0)/Z_β(0;0)≥exp[−βm(6β)W], hence Γ≤βW. The positivity of m follows by differentiating the Haar log moment generating function of ReTr U: its mean is zero at t=0 and its derivative is a strictly positive variance.

Near the common-staple locus use relative coordinates V_1⁻¹V_i=e^{X_i}, X_1=0. The actual minimum obeys W comparable to Σ_i‖X_i‖². The fixed-dimensional holomorphic Laplace theorem of §4.37 gives Γ=βW+O(W) uniformly for large β, with all coefficient derivatives on a common regular domain. For bounded β, right Haar invariance of ∫exp[t ReTr(Ue^{εX})]dU gives the exact Ward covariance E_t[(ReTr UX)(ReTr UY)]=m(t)⟨X,Y⟩/t. Consequently

\[
 \left.\frac{d^2}{d\varepsilon^2}
 \Gamma_\beta(e^{\varepsilon X_1},\ldots,e^{\varepsilon X_6})
       \right|_{\varepsilon=0}
    =\beta m(6\beta)\sum_i\|X_i-\bar X\|^2,
 \qquad \bar X=\tfrac16\sum_iX_i.
 \tag{4.231; P: nonzero transverse bounded-coupling Hessian}
\]

In the relative chart the displayed quadratic form is at least Σ_i‖X_i‖²/6. It therefore proves the lower comparison uniformly on each compact positive β interval near W=0. Away from that locus strict Hölder and compactness give the same comparison for bounded β. At large β use Z_v≤e^{−βW} and Z_flat≥cβ⁻ᵈᴬᐟ²: if W is bounded below, the logarithmic loss is eventually at most βW/2. Choosing the large-β threshold first and the bounded-β chart afterwards avoids circular constants. This proves the energy comparison.

For source holomorphy, the actual normalized conditional expectation M(z)=E_v exp(Σ_i z_i s_i) satisfies |M−1|≤e^{2N‖z‖₁}−1. A fixed doubled source disk keeps it and its flat counterpart within distance 1/2 of one, uniformly in β and v. Near W=0, the regular coefficient derivatives give |Φ|≤CW‖z‖₁ for large β. On a bounded β interval, the actual compact integral is jointly holomorphic in a fixed relative-staple chart and that source disk. Φ vanishes at the flat chart, and color conjugation kills its first field derivative; uniform Taylor/Cauchy estimates give |Φ|≤C‖X‖²‖z‖₁≤CW‖z‖₁. Away from W=0 the elementary logarithmic bound is sufficient because W is bounded below. Cauchy on the doubled source disk supplies every higher source derivative. ∎

N2-F permits β_min=2Nγ⁻², since its g_0≤γ. Thus this whole first-star theorem needs no strengthened trajectory assumption. For sufficiently small source,

\[
 \left|\frac{Z_\beta(v;z)}{Z_\beta(0;z)}\right|
    \le e^{-[c\beta-C\|z\|_1]W(v)}.
 \tag{4.232; P: paid first-integration bound}
\]

For a plaquette-disjoint set I of integrated links, conditioning on all other links factorizes exactly. Every integrated star contributes its deterministic L_β(z_b), its actual e^{−Γ_β(v_b)} and its actual e^{Φ_β(z_b;v_b)}. The unintegrated plaquettes keep their original sources. If |z_p|≤r with r fixed sufficiently small, the modulus of the retained integrand, after these deterministic star factors are removed, is bounded by exp[−(β/2)Σ_{p∈P_ext}s_p−(cβ/2)Σ_{b∈I}W(v_b)]. Additional nonnegative weights depending only on retained links can be included. Inner constraints or interactions depending on integrated links change this conditional law and require their own proof.

**Spatial and field-valued information in SU(2).** Use normalized a_i=1−q·v_i, τ=2β and normalized source z_i=2j_i for this paragraph. Put t_i=τ−z_i=τw_i, s=Σ_iw_i, a_ij=1−v_i·v_j, A=Σ_{i<j}w_iw_j a_ij, r=√(s²−2A) and W=s−r. The square root is the branch near six. The exact Haar integral is

\[
 Z_b(t\mid v)=e^{-\sum_i t_i}I\!\left(
    \sqrt{(\sum_i t_iv_i)\cdot(\sum_i t_iv_i)}\right),\qquad
 I(\kappa)=\sum_{n\ge0}\frac{(\kappa^2/4)^n}{n!(n+1)!}.
 \tag{4.233; P}
\]

On a fixed complex regular field domain, the sector expansion of this exact integral gives

\[
 \Gamma_\tau(w,a)
   =\tau W+\frac32\log(r/s)+W B_\tau(w,a),\qquad
 B_\tau(w,a)=\frac{3}{8\tau sr}+O(\tau^{-2}).
 \tag{4.234; P on the stated joint regular domain}
\]

All source and field derivatives have fixed-margin Cauchy bounds. On complex fields the majorant is Σ|a_ij|, not a possibly cancelling complex W. On the real regular slice, let r_0=|Σv_i|, n=Σv_i/r_0, ω_i=1−n·v_i and u_i=v_i−(n·v_i)n. Then Σ_iω_i=W_0=6−r_0, Σ_iu_i=0 and Σ|u_i|²≤2W_0. For directions f,g on the six plaquettes the leading second source contact is (τr_0)⁻¹(Σ_i(f_i−f̄)u_i)·(Σ_j(g_j−ḡ)u_j). Homogeneity of the classical and determinant terms gives the sharper complete bound

\[
 |K_{fg}|\le CW_0\left[
   \frac{{\rm osc}(f){\rm osc}(g)}\tau
   +\frac{\|f\|_\infty{\rm osc}(g)+\|g\|_\infty{\rm osc}(f)}{\tau^2}
   +\frac{\|f\|_\infty\|g\|_\infty}{\tau^3}\right].
 \tag{4.235; P: actual first-patch spatial two-jet bound}
\]

For a smooth profile, osc(f)≤Ca‖∇f‖∞. Even a common constant source has a nonzero field-valued contact after the flat vacuum is removed:

\[
 K_{\mathbf1\mathbf1}
    =-\frac{W_0}{8r_0\tau^3}+O(W_0\tau^{-4}).
 \tag{4.236; P on real regular exteriors}
\]

It cannot be discarded as an identity counterterm. This explicitly identifies a term that the later source induction must carry and project.

The fixed absolute source radius in (4.230) is substantive. A proportional radius cτ cannot cover every real exterior. In SU(2), the realizable six staples ±e₀,±e₁,±e₂ have cancelling sum and Haar conditional law. Varying one plaquette source produces the factor I(z)I(6τ)/I(6τ−z). Its numerator has an imaginary zero of modulus less than four, as follows directly from the displayed series, uniformly in τ. The regular cτ disk and the all-real fixed disk are therefore genuinely different statements. Neither the global real source estimate nor its exact first-layer extension alone proves the complex-field admission required by the full mixed history construction.

## 4.37 An actual second integration with its inherited interaction retained

The first inherited non-Wilson factor is no longer merely an unestimated next kernel. A genuine second integration, with its old source function and mass intact, has been proved on a fixed complex regular domain for every SU(N). See R2 Second Integration, §§4–7, for the full finite-patch geometry and parameter estimates.

Take a plaquette-disjoint first set I and one retained link e. Assume n≥3, so a distinct old link shares at most one plaquette with e. There are d≤6 adjacent old links b_i. Their union F={e,b_1,…,b_d} has at most seven free links and 6+5d≤36 affected plaquettes. Other previously integrated factors do not depend on these free variables and stay in the actual outer measure. Use a=s/N, τ=Nβ and normalized scalar sources z_p=Nj_p. The exact joint patch integral and its flat phase are

\[
 Z_v(\zeta)=\int_{SU(N)^F}e^{-\zeta S_v(U_F)}dU_F,
 \qquad
 S_0(U,V_1,\ldots,V_d)
   =(6-d)a(U)+\sum_{i=1}^d[5a(V_i)+a(UV_i^{-1})].
 \tag{4.237; P: exact two-stage patch and its flat exterior}
\]

The leaf inversions needed to write this expression preserve Haar measure. In SU(2), integrating the leaves first gives exactly e^{−6dζ}∫e^{−ζS_e^rem(q;v)}Π_i I(ζr_i(q;v))dq. These are the same old I factors, and their r_i are the same functions of the next link. For general SU(N), Fubini identifies the same joint integral with its exact first-link compact integrals without requiring a closed formula.

The Hilbert–Schmidt triangle inequality gives ½Σ_{b∈F}a(U_b)≤S_0≤12Σ_{b∈F}a(U_b). In Lie coordinates orthonormal for the normalized metric −tr(XY), its Hessian is N²−1 copies of 6I−Adj(star_d), whose lower eigenvalue is at least 6−√6. Hence it has a unique flat minimum and a fixed global gap. For boundary links in a small fixed identity chart, the analytic implicit-function theorem gives a critical point U_*(v), a positive real Hessian on the real slice and the unique real minimum. Set 𝓔(v)=S_v(U_*(v)). Its complex continuation is defined on the same fixed chart; |𝓔(v)|≤C‖v‖².

**The holomorphic integration argument.** For real v, Haar invariance centers the integral at U_*(v). Both sides of that equality are holomorphic in the boundary Lie coordinates, so the identity theorem extends it to complex v. This avoids claiming that a complex translation preserves the real Haar contour. In the unchanged real integration variable Q define F_v(Q)=S_v(U_*(v)Q)−𝓔(v). Its value and first derivative at Q=I vanish. A local Taylor estimate and compactness away from I give |F_v(Q)−S_0(Q)|≤C‖v‖dist(Q,I)². A sufficiently small fixed complex v chart therefore ensures Re(ζF_v)≥c|ζ|dist(Q,I)² throughout a fixed right ζ sector.

The centered local Haar density is even in exponential coordinates. Expanding the phase through cubic order, the odd cubic term integrates to zero against the complex even Gaussian. Quartic terms and the square of the cubic term give a relative O(|ζ|⁻¹) remainder; the global tail is exponentially small by the just-proved coercivity. The same estimate on a larger complex parameter domain supplies all Cauchy derivatives. Thus, for |ζ| sufficiently large,

\[
 Z_v(\zeta)=e^{-\zeta\mathcal E(v)}\zeta^{-\nu}
       \mathcal A(v)e^{\varrho(v,\zeta)},\qquad
 \nu=\frac{(d+1)(N^2-1)}2,
 \quad 0<c\le|\mathcal A(v)|\le C,
 \quad |\varrho(v,\zeta)|\le C/|\zeta|.
 \tag{4.238; P: jointly holomorphic exact factorization}
\]

Increasing the coefficient threshold makes the normalized relative error less than 1/2, proving nonvanishing and the logarithmic branch. Global color conjugation kills the first exterior derivative at the flat chart. Therefore Δϱ(v,ζ)=ϱ(v,ζ)−ϱ(0,ζ) has every m-th ζ derivative bounded by m!C^{m+1}‖v‖²|ζ|⁻ᵐ⁻¹. This proves the field-quadratic improvement, including its complex-domain margins; it is not an unquantified stationary-phase approximation.

**The normalized second-source theorem.** Subtract the same flat-patch vacuum on every exterior,
L_{τ,F}(z)=log[Z_0(τ−z)/Z_0(τ)]. For |z|<cτ and v in the proved complex regular chart, the actual remaining logarithm is

\[
 \begin{aligned}
 \mathcal P_{\tau,F}(z;v)
   &:=\log\frac{Z_v(\tau-z)}{Z_v(\tau)}-L_{\tau,F}(z)\\
   &=z\mathcal E(v)+\Delta\varrho(v,\tau-z)-\Delta\varrho(v,\tau),\\
 |\mathcal P_{\tau,F}(z;v)-z\mathcal E(v)|
   &\le C|z|\|v\|^2\tau^{-2},\\
 |\partial_z^m(\mathcal P_{\tau,F}-z\mathcal E)|_{z=0}
   &\le m!C^{m+1}\|v\|^2\tau^{-m-1},\qquad m\ge1.
 \end{aligned}
 \tag{4.239; P: actual repeated regular integration}
\]

Both the determinant term and the fluctuation-count term cancel exactly. For any positive outer law λ supported on this real regular chart, with all its factors genuinely independent of U_F, integrate e^{𝓟} against Z_v(τ)λ(dv)/∫Z_v(τ)dλ. Its modulus is at most exp(C|z|δ²). The numerator and denominator use exactly the same outer law and full patch mass. Inner selectors or old factors depending on U_F cannot be moved to λ to claim this estimate.

The old source is exactly the one treated by this theorem. Let μ_red be the actual next-link law after the d first-link integrations, and let Φ_i be their inherited flat-subtracted source functions. Its source is Ψ=zS_e^rem+Σ_iΦ_i. Exact Fubini gives

\[
 \log\mathbb E_{\mu_{\rm red}}e^\Psi
       =\log\frac{Z_v(\tau-z)}{Z_v(\tau)}-dL_{1,\tau}(z),\qquad
 L_{2,\tau,F}=L_{\tau,F}-dL_{1,\tau},\qquad
 \log\mathbb E_{\mu_{\rm red}}e^\Psi-L_{2,\tau,F}
       =\mathcal P_{\tau,F}.
 \tag{4.240; P: exact inherited-source and vacuum telescoping identity}
\]

The first deterministic vacua are already inside L_F. Only their difference L_2 is removed at the second stage. This rules out double subtraction and makes the result an actual iterated-source theorem.

**Independent spatial coefficients.** Give each affected plaquette weight w_p near one. The same centered proof applies jointly in w and v. The ground energy 𝓔(w,v) has degree one in w; the flat-relative determinant D(w,v) has degree zero; and the flat-relative remainder R obeys R(tw,v,τ)=R(w,v,tτ). All three vanish quadratically in v. Differentiating the exact source quotient at w=1−z/τ gives, for directions f,g and their oscillations on the finite patch,

\[
 |\mathcal P_{fg}|\le C\|v\|^2\left[
  \frac{\omega(f)\omega(g)}\tau
 +\frac{\|f\|_\infty\omega(g)+\|g\|_\infty\omega(f)}{\tau^2}
 +\frac{\|f\|_\infty\|g\|_\infty}{\tau^3}\right],
 \qquad
 -\mathcal E''[f,g]=\langle G_f,H^{-1}G_g\rangle.
 \tag{4.241; P: spatial second-patch contact and its exact leading term}
\]

Here G_f is the gradient of Σ_pf_pa_p at the actual minimizing internal configuration and H its positive Hessian; G_1=0. The leading contact is therefore a field-valued Gram term, with radial cancellation, not an identity term. Smooth sources have ω(f)≤Ca‖∇f‖∞. The exterior norm in this formula is a local chart norm: the physical field-scale conversion and root count still have to be supplied when admitting it to the multiscale norm.

A source-independent inner factor e^B can remain in this theorem if B has a uniform holomorphic bound on a neighborhood of the entire compact inner manifold and the boundary chart, is real on real fields, and is color invariant. It becomes a bounded analytic amplitude in the same proof. If B has a baseline-coupling label, that label is frozen during the source variation. This stability statement cannot be invoked for unclassified old activities or hard constraints without checking those hypotheses.

The output is a new effective interaction 𝓔(v), determinant 𝒜(v), analytic correction ϱ(v,τ), and their actual inherited source functions. These are proved and available for a next local transition. Constants remain uniform for these finitely many patch geometries; no estimate here asserts uniformity as the number of historical variables or gauge constraints grows without bound. That extension is the remaining multiscale obligation.

## 4.38 A local Gaussian vacuum, including a strict source-jet recipe

A global determinant-rank estimate retains the fine-volume divergence and cannot by itself prove a physical-volume locality remainder. The following operator theorem isolates the missing calculation and proves it, including all source orders. Its full proof is Gaussian Source Locality, §§2–4. Its application to a particular factor requires that factor's exact covariance and source dictionary; it is not an additional assumed Yang–Mills interface.

Let h_k=L^ka, 0≤k≤K. Let Γ_k^∞ be symmetric d-component covariance kernels, covariant under simultaneous h_k-grid translations, and suppose

\[
 \|\Gamma_k^\infty(x,y)\|
   \le C_0X_k^{-1}h_k^{-4}e^{-\mu|x-y|_1/h_k},
 \quad X_k\ge X_*>0,\qquad
 \Gamma_k^T(x,y)=\sum_{n\in\mathbb Z^4}
       \Gamma_k^\infty(x,y+nT)\ge0.
 \tag{4.242; C: explicit common-kernel hypotheses for the operator theorem}
\]

The final inequality means positivity as a covariance matrix. The exact common periodization is essential; unrelated exponentially decaying finite-torus matrices need not have it. For a centered Gaussian ξ_k with that covariance, define F_k^T[J]=log E exp[(a⁴/2)Σ_x ξ_k(x)^T J(x)ξ_k(x)], with J a complex symmetric matrix source. All normalizations, including a⁴ and the one half, are part of this definition.

**Theorem (P under (4.242)).** On a fixed small source ball, independent of a,K,T, there is a torus-independent cell functional L_a^G such that

\[
 \sum_{k=0}^KF_k^T[J]
   =\sum_cL_a^G(J|_{c^\delta})+R_{a,T}^G[J],
 \qquad |R_{a,T}^G[J]|
        \le C n_{\rm act}(J)\le CN_T,
 \qquad \delta=\ell_0/16.
 \tag{4.243; P: Gaussian local vacuum and physical-cell remainder}
\]

The functionals are holomorphic on a neighborhood of the closed ball, real on real sources, covariant under cell translations, and zero at zero. Under the exact face-reflection covariance of Γ and its tensor source transformation, they are reflection covariant and have the required chessboard replication property for a source supported at margin ℓ₀/8. The remainder's m-th derivative is bounded by m!C^{m+1} times the active-cell count and the product of directional source norms. The normalized product of these specified Gaussian source factors is e^R and has the corresponding physical-cell bound.

**Proof and counterterm recipe.** Regard Γ as an operator with measure a⁴. The exponential kernel bound gives a uniform Schur bound C/X_k. Choose the source ball so that the half-exponent positive majorant of ΓJ has norm at most 1/4 on a doubled ball. The exact convergent logarithm is then ½Σ_{m≥1}Tr[(ΓJ)^m]/m, also for a degenerate covariance.

Root each trace loop at its first source site. Assign a root on r cell faces weight 2⁻ʳ in each adjacent cell, and weight one to an interior root. The weights sum to one, and a⁴ times their sum in each cell is exactly ℓ₀⁴. They preserve reflection symmetry at lattice sites on faces. Expand each periodized edge into its lifted infinite-kernel paths. Define L_{k,c} by retaining precisely zero-winding loops with all source vertices in c^δ; their kernels and integration recipes are independent of T. Set L_a^G=Σ_kL_{k,c}.

Any omitted loop rooted in c has total edge length at least δ; a winding loop has length at least T. Split its exponential decay into two halves. One half pays that physical distance; use the other half in the Schur sums, leaving one closing edge at its pointwise h_k⁻⁴/X_k bound. Thus the per-cell error at scale k is at most C‖J‖∞X_k⁻¹(ℓ₀/h_k)⁴exp[−μℓ₀/(32h_k)]. A source-free root gives zero, so only active cells occur. The numerical sum Σ_{r≥0}L^{4r}e^{−cL^r} is finite. This proves (4.243) with its holomorphic bounds. Affine face reflections preserve the loop recipe and fractional root weights. Since the collar is thinner than the support margin, reflected neighboring copies add no unwanted source inside a cell's collar. Finite-family Cauchy proves every derivative assertion. ∎

There is a stronger identity-valued contact recipe. Supply the actual underlying C⁵ source function, and use the algebra norm Σ_{|α|≤5}ℓ₀^{|α|}sup‖∂^αJ‖/α!. In every nonwinding infinite loop rooted at x, replace its ordered source product by the joint Taylor polynomial through total degree four along J(x+t(y_i−x)). Keep the covariance matrices fixed. The resulting L_a^{G,jet} depends only on source jets through order four at the root, with torus-independent infinite-kernel moments as coefficients. It satisfies

\[
 \sum_{k=0}^KF_k^T[J]
    =\sum_cL_a^{G,\rm jet}(J|_{c^\delta})
            +R_{a,T}^{G,\rm jet}[J],
 \qquad |R_{a,T}^{G,\rm jet}[J]|
       \le C n_{\rm act}(J).
 \tag{4.244; P: strict local source-jet refinement}
\]

To prove it, separate winding loops as before. If D is the total edge length of a nonwinding loop, all displacements from its root are at most D. The fifth derivative of the ordered product is bounded by 5!(D/ℓ₀)⁵ times the m-th power of the C⁵ algebra norm. Its multinomial sum is already included in that norm power; no new growing derivative order is required. Taylor's remainder divides by 5!, and a fixed fraction of the exponential edge reserve pays (D/h_k)⁵. Root counting costs (ℓ₀/h_k)⁴, so the per-cell error is at most Ch_k/ℓ₀. Its scale sum is bounded by L/(L−1). The unchanged source factor at the root again restricts the count to active cells. The finite Taylor terms converge normally on a fixed smaller source ball. The same reflection and Cauchy arguments complete the theorem.

The Gaussian result supplies the local counterterm rather than merely bounding its size. The divergent local trace stays inside L_a^G or L_a^{G,jet}; only the controlled remainder is charged to physical volume. The strict jet form concerns the identity-valued vacuum. Field-valued collision outputs, such as (4.236) and (4.241), remain separate terms.

**Exact application limits.** The source-zero flat constrained matrix, physical curvature pullback, coordinate-volume factors and zero-mode convention must be matched to (4.242). At nonzero background, the covariance may have a different local description and must be handled with its actual domains. More importantly, one physical source coupled to the sum of Gaussian shell fields includes cross-shell terms. Even for independent standard real Gaussians X,Y,

\[
 \log\mathbb E e^{j(X+Y)^2/2}
       =-\tfrac12\log(1-2j)
       \ne-\log(1-j)
       =\log\mathbb E e^{jX^2/2}
           +\log\mathbb E e^{jY^2/2}.
 \tag{4.245; P: exact cross-shell distinction}
\]

Consequently the displayed sum of specified Gaussian factors cannot silently replace the full physical sourced integral. One must transport its actual Schur-complement source kernel and retained-field terms, or admit the cross terms as interactions with the fixed source-zero Gaussian. The present theorem proves the operator locality calculation once that dictionary is supplied; it does not complete the nonlinear E/R/B vacuum or compulsory-history normalization.

## 4.39 Actual inherited source densities through arbitrarily many complete positive steps

Combining §§4.35–4.36 gives a normalized transport theorem beyond a single patch. It controls the actual source density and all its source derivatives through any number of complete positive source-independent marginalizations. The complete proof, exact admissible polydiscs and a counterexample to a stronger inference are in Integrated Raw Source Transport, §§1–4.

Throughout this theorem β=β_K is the literal bare N2-F coefficient on a compatible torus. Let μ_ext be the **actual** source-free exterior marginal after a plaquette-disjoint first layer I. It includes Π_{b∈I}Z_β(v_b;0), every remaining Wilson factor, and its true global normalization. Give the plaquettes independent complex values z_p. Put A(z)=Σ_p|z_p|, r(z)=max_p|z_p|, and let
F_1(z;v)=Σ_{p∈P_ext}z_ps_p(v)+Σ_{b∈I}Φ_β(z_b;v_b), G_1=e^{F_1} and L_I=Σ_bL_β(z_b). The exact first-layer identity is ∫G_1dμ_ext=e^{−L_I}Z[z]/Z[0]. No inherited Φ is replaced by a fresh centered source.

**Theorem (P).** There are fixed r_*,c_*,C_*>0 such that

\[
 \|G_1(z)\|_{L^p(\mu_{\rm ext})}
       \le e^{C_*A(z)/\beta},
 \qquad r(z)<r_*,\quad 1\le p<\infty,
       \quad p\,r(z)<c_*\beta.
 \tag{4.246; P: actual inherited raw-density admission}
\]

For any complete positive probability kernel Q(dw|v), independent of z, let ν=μ_ext Q. The transported density is G_Q=d[(G_1μ_ext)Q]/dν=E[G_1|w], and

\[
 \|G_Q(z)\|_{L^p(\nu)}\le e^{C_*A(z)/\beta},
 \qquad \int G_Q(z)d\nu=e^{-L_I(z)}Z[z]/Z[0],
 \qquad
 \int_H|G_Q(z)|d\nu
    \le\nu(H)^{1-1/p}e^{C_*A(z)/\beta}\quad(p>1).
 \tag{4.247; P: full-mass transport and component bound}
\]

Q may be a composition of arbitrarily many such complete steps and retain every history label. On smaller admitted source domains, G_Q is holomorphic as an Lᵖ-valued function, and differentiation commutes with its transport.

**Proof.** The all-real star estimate bounds |Φ_b| by CΣ_{p∋b}|z_p|W_b≤CΣ_{p∋b}|z_p|S_b for every original-field completion. Assign each unintegrated sourced plaquette once to one of its boundary link stars. This gives deterministic nonnegative η_b with |F_1(z;v(U))|≤Σ_bη_bS_b(U), maxη_b≤C_0r(z) and Ση_b≤C_0A(z). Apply (4.223) with w_b=pη_b/(κβ), which is at most one by the stated domain. It yields ∫e^{p|F_1|}dμ_ext≤e^{C_*pA/β}; taking the p-th root proves (4.246). Conditional Jensen proves the norm contraction for every complete Q, and row mass one proves the unchanged total source integral. Hölder proves the component estimate without deleting its old mass. Finite-cutoff analyticity under the same doubled-domain majorant and the Bochner Cauchy formula prove the source-jet claims. ∎

The literal real erased-R operation also contracts this integrated raw norm. Let λ(dv)σ_v(dζ) be its actual finite positive old measure, q_v(du) its normalized fresh reference, and R_0(v,du)=q_v(du)σ_v1. For a raw old jet F_m, put R^{(m)}(v,du)=q_v(du)σ_v(F_m). Conditional Jensen gives

\[
 \left\|\frac{d(\lambda R^{(m)})}{d(\lambda R_0)}
          \right\|_{L^p(\lambda R_0)}
       \le\|F_m\|_{L^p(\lambda\sigma)}.
 \tag{4.247a; P: exact averaged real erased-R contraction}
\]

For the first and mixed second logarithmic input jets, F_1=A_f and F_2=A_fg+A_fA_g. The nonconstant old mass remains on both sides; a zero mass contributes zero. This holds also for a subprobability component and incurs no reciprocal old mass. A signed recent-R difference or complex exterior is not such a positive erasure. To combine it with the actual Wilson admission bound, the old joint law must be the correctly identified complete positive lift of that Wilson law.

Explicitly, for directions f^r with F_r=‖f^r‖∞>0, A_r=Σ_p|f_p^r| and 0<θ<min(r_*/2,c_*β/(2p)), choose the parameter radii θ/(mF_r). Then

\[
 \|D^mG_Q(0)[f^1,\ldots,f^m]\|_{L^p(\nu)}
 \le m!\left(\frac e\theta\right)^m
       e^{C_*\theta n_{\rm eff}/\beta}\prod_rF_r,
 \qquad n_{\rm eff}=\frac1m\sum_r\frac{A_r}{F_r}.
 \tag{4.248; P: all-order exact inherited-density jets}
\]

The estimate m^m≤e^m m! supplies the factorial. A zero direction gives zero. For fixed p, N2-F's β≥2Nγ⁻² permits θ independent of cutoff. The actual same-star contacts and all products generated by exponentiation are retained in these derivatives.

This is a genuine later-transition theorem; it does not require that a literal source be admitted first to a pointwise complex-field norm. Its quantitative limitation is equally concrete. If the source occupies D physical cells, the number of fine plaquette anchors is O(L^{4K}|D^+|). The proved exponential budget is O(rL^{4K}|D^+|/β_K), which is not uniform in K. The initial flat-star vacua have already been subtracted, but subsequent local vacua and nonidentity field projections have not. The factor (a/ℓ₀)⁴ in the separately defined weighted energy budget cannot be assigned to the literal scalar source to hide this loss.

Nor can the integrated norm create a pointwise logarithm on every retained component. An exact probability example makes the distinction explicit. Give an event H probability e^{−2κM}; on it let X=±M with equal probability, and set X=0 off it. The nonnegative energy A=M1_H has E e^{κA}≤2. Marginalizing the sign while retaining H produces G_M(z)=cosh(Mz) on H and one off H. On |z|≤κ/p its Lᵖ norm is at most 2^{1/p}, yet

\[
 G_M\!\left(\frac{\pi i}{2M};H=1\right)=0.
 \tag{4.249; P: integrated admission does not imply a componentwise log disk}
\]

This is an abstract counterexample to that inference, not a Wilson counterexample or a disproof of a summed-history pressure theorem. It shows why the next mixed norm should be formulated directly for densities where possible, and why a prescribed component's logarithm requires additional information.

For ordinary successive Haar integrations, Q is literally the actual conditional marginalization, so the theorem applies directly. For a constrained history construction it must be identified as a complete positive lift with the same source-free marginal. A signed connected-activity expansion is not itself such a probability kernel.

The remaining bridge is specific: prove local identity and full dimension-four source extraction under the actual constrained mixed operator, with a stable analytic regular part and an integrated raw part, and with the physical determining-block count replacing the fine-anchor budget. That bridge includes all generated field-valued contacts and the actual source placements. The transport part (4.246)–(4.248) is completed; the mixed local extraction and its uniform multiscale closure are still O.

## 4.40 The actual second integration on every real exterior

The regular second-patch theorem of §4.37 has an all-real extension. It does not assume that the original exterior links are in an identity chart. The complete proof is R2 Global Second Patch, §§1–4.

Use the same acyclic patch F, with d+1≤7 links and M=6+5d≤36 affected plaquettes, on n≥3. Retain normalized a=s/N, τ=Nβ and independent z_p=Nj_p. Let m(v)=min S_v and Z_v(τ,z)=∫exp[−τS_v+Σ_pz_pa_p]dU_F. Define Γ_τ(v)=log[Z_0(τ,0)/Z_v(τ,0)], L_τ(z)=log[Z_0(τ,z)/Z_0(τ,0)] and Φ_τ(z;v)=log[Z_v(τ,z)/Z_v(τ,0)]−L_τ(z).

**Theorem (P).** There are τ_*(N),C(N)<∞, uniform over the finitely many patch types, such that for every real exterior and τ≥τ_*,

\[
 \tfrac12\tau m(v)\le\Gamma_\tau(v)\le2\tau m(v),
 \qquad
 |\Phi_\tau(z;v)|\le Cm(v)\|z\|_1
       \quad(\|z\|_1\le1/32).
 \tag{4.250; P: actual all-real second-patch theorem}
\]

The source logarithms are holomorphic on the larger ball ‖z‖₁<1/16. Every q-th source derivative is bounded by q!C_jet^q m(v) times the product of the directional ℓ¹ norms. Constants do not depend on the torus, spacing, exterior or coupling above the threshold. The theorem is for this fixed acyclic patch; no uniform growing-patch assertion is included.

**Exact normal form.** Choose any source-zero minimizing internal configuration U_F^*. Translate the hub U=QU^* and each leaf V_i=R_iV_i^*. Cyclicity and inversion write its unique shared plaquette as a(UAV_i^σB), σ=±1. With T_i=U^*A for σ=+1 and T_i=U^*AV_i^{*−1} for σ=−1, the change Q_i=(T_iR_i^σT_i⁻¹)⁻¹ converts that plaquette to a(QQ_i⁻¹B_{s_i}). Every leaf-only plaquette becomes a(Q_iB_p), and every hub-only plaquette becomes a(QB_p). All changes preserve product Haar measure. Each B_p is a conjugate or inverse conjugate of its actual minimizing plaquette. Thus the actual sourced phase becomes

\[
 \widetilde S_B
  =\sum_{p\in H}a(QB_p)
    +\sum_i\sum_{p\in A_i}a(Q_iB_p)
    +\sum_i a(QQ_i^{-1}B_{s_i}),
 \qquad \sum_pa(B_p)=m(v).
 \tag{4.251; P: source-label-preserving acyclic normal form}
\]

All original plaquette labels and their independent coefficients are preserved. The changes are frozen at source zero. A leaf has only one shared plaquette, so no incompatible conjugation is required; this is precisely where acyclicity enters. No global unique or measurable choice of minimizer is needed for a pointwise bound in terms of the continuous function m(v).

If m is sufficiently small, all B_p have principal logarithms b_p∈su(N) with Σ‖b_p‖²≤Cm. The traceless logarithm is ensured by taking the identity chart small enough for the sum of principal eigenangles to be zero. This tuple is an actual small parameter of the same holomorphic flat star phase, even when no original boundary-link chart was available. If m=0, all B_p=I, so the entire independently sourced kernel equals its flat counterpart.

Apply the centered compact Laplace proof of §4.37 to the independent b_p parameters and independent weights w_p. Its hypotheses follow from the same flat Hessian and gap. Global conjugation kills all linear b terms in the energy, determinant difference and remainder. Consequently Γ_τ=τm+O(m), and the exact quotient at w=1−z/τ gives |Φ|≤Cm‖z‖₁, uniformly for small m. This proves the delicate regime without losing a hidden flat holonomy or a fluctuation determinant.

For the complementary regime no lower Hessian or uniqueness is needed. The phase has a uniformly bounded second derivative at every compact minimum. A ball of radius cτ⁻¹ᐟ² around any minimizing configuration gives a lower bound, while S_v≥m gives the upper bound:

\[
 c\tau^{-\nu}e^{-\tau m(v)}
       \le Z_v(\tau,0)\le e^{-\tau m(v)},\qquad
 \tau m(v)-\nu\log\tau-C
       \le\Gamma_\tau(v)\le\tau m(v)+C,
 \quad \nu=\tfrac12(d+1)(N^2-1).
 \tag{4.252; P: arbitrary-minimum compact estimates}
\]

Choose τ_* so that the logarithmic loss is at most τm/2 whenever m exceeds the fixed regular threshold. Together with the small-m estimate this proves the two-sided energy comparison everywhere.

For the source, the true conditional ratio satisfies |Z_v(τ,z)/Z_v(τ,0)−1|≤e^{2‖z‖₁}−1 because 0≤a_p≤2. Hence its logarithm and the flat logarithm exist uniformly on the larger fixed ball. Their difference is O(‖z‖₁), which is charged to m where m is bounded below. The regular normal form handles the remaining region. This proves (4.250) and all jets by Cauchy. ∎

The actual first-layer readouts are retained. If K_i(U;z_i) are the literal old leaf kernels, set φ_i=log[K_i(U;z_i)/K_i(U;0)]−L_i(z_i), with L_i the deterministic flat-star vacuum. The true reduced hub law is proportional to e^{−τS_rem(U)}Π_iK_i(U;0), and its inherited source is Ψ=Σ_{p∈P_rem}z_pa_p+Σ_iφ_i. Exactly as in (4.240), the second subtraction is L_2=L_τ−Σ_iL_i and log E_red e^Ψ−L_2=Φ_τ. This identity now holds on every real exterior, with the all-real bounds just proved.

For any positive source-independent true outer law λ on arbitrary real exteriors, with finite positive zero-source patch mass, put dν_λ=Z_v(τ,0)dλ/∫Z_v(τ,0)dλ. Then

\[
 e^{-L_\tau(z)}
   \frac{\int Z_v(\tau,z)d\lambda}{\int Z_v(\tau,0)d\lambda}
       =\mathbb E_{\nu_\lambda}e^{\Phi_\tau(z;v)},
 \qquad
 \left|\mathbb E_{\nu_\lambda}e^\Phi\right|
       \le\mathbb E_{\nu_\lambda}e^{C\|z\|_1m(v)}
       \le e^{2MC\|z\|_1}.
 \tag{4.253; P: arbitrary-real true-outer normalization}
\]

Factors depending on U_F must already be in the inner kernel. They cannot be assigned to λ to invoke this result. The exact kernel also retains the energy reserve exp[−(τ/2−C‖z‖₁)m]. For small m, a common normalized source t has the sharper Φ_τ(t1;v)=tm+O(|t|m/τ²) on |t|≤cτ, by homogeneity and the same coefficient-sector estimates.

This removes the regular-support restriction for these fixed actual two-stage patches. It does not extend a constant per fine patch to a physical-volume bound. Hard inner selectors can exclude the minimum, later interaction graphs can have cycles, and retained historical variables can grow in number and scale. Their source readouts and local projections must still be controlled in the complete mixed norm. The exact first and second integrations, and the arbitrary complete positive raw transport, are completed inputs to that remaining step.
