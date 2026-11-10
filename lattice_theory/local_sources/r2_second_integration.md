# Inherited interactions in the second integration

## 1. Target, normalization and status

This note continues the R2 analysis of [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md). It keeps the actual inherited non-Wilson interaction after a plaquette-disjoint first integration. The new results are: a quantitative holomorphic decomposition of that interaction on a fixed complex regular exterior domain, and a normalized second-integration theorem for a genuine finite star patch of the original SU(2) Wilson law with a regular exterior. Neither result replaces the complete-history R2 theorem, which remains **O**.

The normalization is the literal one fixed in [Lattice conventions and hypotheses](../lattice_conventions.md). For SU(2), let a_p=1−ReTr(U_p)/2, so s_p=2a_p and the action coefficient is τ=2β_a. A constant physical scalar source j on the selected plaquettes has coefficient z=2j and changes τ to τ−z on precisely those plaquettes. All Haar measures are normalized.

The first integration of a free link with six staple quaternions v_i gives

\[
 K_\tau(v)=e^{-6\tau}I(\tau r),\qquad
 r=\Big|\sum_{i=1}^6v_i\Big|,\qquad
 I(\kappa)=\frac2\pi\int_{-1}^{1}e^{\kappa u}\sqrt{1-u^2}\,du.
 \tag{N2.1; P: exact first marginal}
\]

The actual source-free exterior measure contains all these factors. They are not replaced by normalized auxiliary references. Define its flat-relative effective energy and the corresponding flat-vacuum-subtracted source logarithm by

\[
 \Gamma_\tau(r)=\log I(6\tau)-\log I(\tau r),\qquad
 \Phi_\tau(z;r)=\Gamma_\tau(r)-\Gamma_{\tau-z}(r).
 \tag{N2.2; P: definitions near the real positive axis}
\]

[Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md) proves source holomorphy for every real exterior. Here §§2–3 also control the first inherited factor as a function of a **complex regular exterior**, and identify its determinant and higher corrections. Sections 4–6 then integrate one more actual retained link, equivalently the corresponding connected patch of at most seven original links. The old product of I factors is kept throughout.

All constants in the local results are independent of the fine spacing, torus volume and τ≥τ₀. They may depend on the fixed patch size, the fixed regularity neighborhood and a stated finite derivative order. The second-step geometry assumes n≥3 sites in each periodic direction, so distinct links share at most one plaquette. The selected cofinal lattices satisfy this restriction; the special n=2 coincidences are not silently included.

**Status labels.** P means a proof in the displayed scope; C means an actual-theory application still needs its explicitly stated hypothesis; O means unproved. Only N2-F is an assumed program interface. The results below are finite-dimensional derivations and do not assume a sourced stability theorem.

## 2. A uniform sector expansion of the exact Haar integral

Put c_H=√(2/π). On the right half-plane use the principal powers of κ. Substituting t=1−u in (N2.1) gives the exact identity

\[
 I(\kappa)=c_H e^\kappa\kappa^{-3/2}\mathscr A(\kappa),\qquad
 \mathscr A(\kappa)=\frac{\kappa^{3/2}}{\Gamma(3/2)}
       \int_0^2 e^{-\kappa t}t^{1/2}\sqrt{1-t/2}\,dt.
 \tag{N2.3; P}
\]

### Theorem 2.1. Quantitative holomorphic expansion — P

Fix 0<θ₁<θ₂<π/2. There are R,C,C₁ finite, depending only on these angles, such that on |arg κ|≤θ₂ and |κ|≥R the function I has no zero and

\[
 \mathscr A(\kappa)=1-\frac{3}{8\kappa}+O(C|\kappa|^{-2}),\qquad
 \mathscr R(\kappa):=\log\mathscr A(\kappa)
      =-\frac{3}{8\kappa}+\mathscr Q(\kappa),
 \qquad |\mathscr Q(\kappa)|\le C|\kappa|^{-2}.
 \tag{N2.4; P}
\]

The logarithm is the branch defined by |𝒜−1|<1/2. On the smaller sector |arg κ|≤θ₁, |κ|≥2R, every derivative obeys

\[
 |\mathscr R^{(m)}(\kappa)|
      \le m!C_1^{m+1}|\kappa|^{-m-1},\qquad
 |\mathscr Q^{(m)}(\kappa)|
      \le m!C_1^{m+1}|\kappa|^{-m-2},\qquad m\ge0.
 \tag{N2.5; P}
\]

**Proof.** For 0≤u≤1 the exact elementary identity

\[
 \sqrt{1-u}-1+\frac u2
       =-\frac{u^2}{2(1+\sqrt{1-u})^2}
 \tag{N2.6; P}
\]

bounds the error by u²/2. Apply it with u=t/2. Replacing √(1−t/2) in (N2.3) by 1−t/4 therefore costs at most
C|κ|^{3/2}∫₀²e^{−Reκ t}t^{5/2}dt≤C_θ|κ|⁻².
The replacement of the upper endpoint two by infinity in the two polynomial integrals has the same bound: Re κ≥|κ|cos θ₂, and each omitted tail is exponentially small in |κ|. The full gamma integrals are Γ(3/2)κ⁻³ᐟ² and Γ(5/2)κ⁻⁵ᐟ². Since Γ(5/2)/Γ(3/2)=3/2, their normalized sum is exactly 1−3/(8κ).

This proves the first expansion. Increasing R makes |𝒜−1|≤1/2, so 𝒜 has no zero and its principal local logarithm is holomorphic throughout the sector. The elementary power series for log(1+w) gives the second expansion and its remainder bound. The other factors in (N2.3) are nonzero, so I is nonzero there as well.

For κ in the smaller sector, a disk of radius c|κ|, with c>0 depending only on θ₂−θ₁, lies in the larger sector and has |κ′| comparable with |κ|. Enlarge R once if necessary to keep that disk above the threshold. Cauchy's derivative estimate applied to 𝓡 and 𝓠 gives (N2.5). The proof uses the exact Haar integral, not a formal or unquantified Bessel expansion. ∎

The leading logarithm is consequently

\[
 \log I(\kappa)
   =\kappa-\frac32\log\kappa+\log c_H+\mathscr R(\kappa)
 \tag{N2.7; P on the stated sector and chosen branch}
\]

and is suitable for joint current-coupling and complex-exterior estimates. No assertion is made about a zero-free extension through κ=0 or into an arbitrary complex sector.

## 3. Holomorphic admission of the first inherited interaction

Fix τ≥τ₀, with τ₀ sufficiently large. In this section ζ is a complex coefficient with |ζ−τ|<τ/8 and r lies in |r−6|<1/2. The sector lemma applies on a larger product neighborhood, so all derivative estimates below have fixed margins.

### Theorem 3.1. Exact classical, determinant and remainder decomposition — P

Put W=6−r. There is a holomorphic B(ζ,r), including r=6, such that

\[
 \Gamma_\zeta(r)=\zeta W+\frac32\log(r/6)+WB(\zeta,r),\qquad
 B(\zeta,r)=\zeta\int_0^1
  \mathscr R'\!\left(\zeta[r+t(6-r)]\right)dt.
 \tag{N2.8; P}
\]

Its mixed derivatives satisfy, on smaller fixed product neighborhoods if needed,

\[
 |\partial_\zeta^m\partial_r^nB(\zeta,r)|
    \le m!n!C^{m+n+1}\tau^{-m-1},\qquad
 B(\zeta,r)=\frac1{16\zeta r}+O(C\tau^{-2}).
 \tag{N2.9; P}
\]

**Proof.** Subtract (N2.7) at 6ζ and ζr. The factors log ζ and log c_H cancel, giving the first formula except for its divided difference. The fundamental theorem of calculus for the holomorphic function 𝓡 gives that divided difference exactly as the integral in (N2.8), which also proves removability at r=6. The bound |𝓡′|≤C|κ|⁻² gives |B|≤C/τ. Multivariable Cauchy on the fixed larger product neighborhood gives the mixed derivative estimates.

The leading term 𝓡(κ)=−3/(8κ)+𝓠(κ) gives
𝓡(6ζ)−𝓡(ζr)=(3/(8ζ))(1/r−1/6)+O(|W|τ⁻²).
Since (3/8)(1/r−1/6)=W/(16r), this proves the last assertion. The O term and its derivatives have the same analytic margins. ∎

The logarithmic term is the actual one-link determinant correction. It is independent of ζ after the flat comparison; it must not be charged as an arbitrary source-dependent remainder.

### Corollary 3.2. Improved source bound with complex regular exteriors — P

For |z|<cτ and |r−6|<1/2, with fixed c>0 sufficiently small,

\[
 \Phi_\tau(z;r)
   =zW+W\{B(\tau,r)-B(\tau-z,r)\},\qquad
 |\Phi_\tau(z;r)-zW|
     \le C|z||W|\tau^{-2}.
 \tag{N2.10; P}
\]

The quotient (Φ−zW)/(zW), filled in at z=0 and W=0, is holomorphic and bounded by Cτ⁻². Thus every complex-exterior derivative on an inner domain has its usual fixed-margin Cauchy bound. In particular,

\[
 \left|\partial_z^m\bigl(\Phi_\tau(z;r)-zW\bigr)\big|_{z=0}\right|
     \le m!C^{m+1}|W|\tau^{-m-1},\qquad m\ge1.
 \tag{N2.11; P}
\]

**Proof.** Subtract (N2.8) at τ and τ−z. The entire determinant term cancels. Integrate ∂_ζB along the coefficient segment and use (N2.9). Higher source derivatives follow directly from the ζ derivatives in the same formula; division by z and W has the stated removable singularities. ∎

This gains one inverse power of τ over the earlier all-exterior bound. The improvement is restricted to the regular exterior domain. It does not assert a coefficient-scaled source neighborhood for arbitrary complex or frustrated exteriors.

### 3.3 Extracting the linear field coefficient and the higher field remainder

In the variable W, define c(ζ)=∂_WΓ_ζ(6−W)|_{W=0}. The exact formulas and the expansion above give

\[
 c(\zeta)=\zeta\frac{I'(6\zeta)}{I(6\zeta)}
     =\zeta-\frac14+\frac1{96\zeta}+O(C\tau^{-2}),
 \qquad |c'(\tau)-1|\le C\tau^{-2}.
 \tag{N2.12; P}
\]

There is a holomorphic H(ζ,W) such that

\[
 \Gamma_\zeta(6-W)=c(\zeta)W+W^2H(\zeta,W),\qquad
 H(\zeta,W)=H_\infty(W)+O(C\tau^{-1}),
 \quad
 H_\infty(W)=\frac{\frac32\log(1-W/6)+W/4}{W^2}.
 \tag{N2.13; P}
\]

All singularities at W=0 are removable. Moreover |∂_ζH|≤Cτ⁻² on an inner domain. Consequently the first inherited scalar source has the exact projected form

\[
 \Phi_\tau(z;6-W)
    =[c(\tau)-c(\tau-z)]W+W^2[H(\tau,W)-H(\tau-z,W)],
 \quad
 |H(\tau,W)-H(\tau-z,W)|\le C|z|\tau^{-2}.
 \tag{N2.14; P}
\]

**Proof.** Differentiate (N2.2) at W=0 for the exact expression for c. Equations (N2.8)–(N2.9) give its expansion and derivative estimate. Subtract c(ζ)W from (N2.8). The explicit logarithm leaves W²H_∞. The other term is W[B(ζ,6−W)−B(ζ,6)], whose division by W² is a bounded r-derivative divided difference of B. This gives the O(τ⁻¹) term and its coefficient derivative. Subtract at τ and τ−z to obtain (N2.14). ∎

Here c is the coefficient of the specific finite-loop function W, not yet the Wilson coefficient in the full renormalization scheme. Identifying its dimension-four projection in that scheme is a further dictionary/extraction step. The result nevertheless identifies the actual inherited linear coefficient and a higher field remainder, rather than treating all of log I as an unspecified old interaction.

### 3.4 The actual complex gauge-field neighborhood

For complexified SU(2), use the holomorphic quaternion coordinates on SL(2,C), with v_i·v_i=1. Put

\[
 a_{ij}=1-\tfrac12\operatorname{Tr}(V_iV_j^{-1}),\qquad
 A_{\rm loop}=\sum_{i<j}a_{ij},\qquad
 r^2=36-2A_{\rm loop},\qquad r\sim6.
 \tag{N2.15; P}
\]

The equality follows from the bilinear quaternion identity. The first integration itself remains exactly \(e^{-6\zeta}I(\zeta r)\): it holds for real quaternions and extends holomorphically in the matrix entries. Equivalently, I is even and entire, so its power series is an entire series in ζ²r²; the branch r∼6 is needed only for the logarithmic decomposition.

If the six plaquettes admit a common completion P_i=UV_i in SL(2,C) with ‖P_i−I‖≤ε in one fixed small identity chart, then P_iP_j⁻¹ is O(ε) from I. Its traceless logarithm shows |a_ij|≤Cε². Hence |A_loop|≤Cε² and |W|≤Cε²; choosing ε once makes the whole preceding complex domain valid. All carriers are the literal relative-staple loops, of length at most six.

On the real slice, A_loop≥0 and A_loop=W(12−W)/2. On a complex domain individual a_ij may cancel. A spatially varying six-source derivative must therefore use the majorant Σ|a_ij|, rather than deducing its bound from |W| alone. The common-source factorization (N2.10) has the exact W factor because its exterior r is held fixed. The independent-source extension in [Spatial sources and field-dependent contacts](r1_spatial_source_integration.md) keeps the stronger majorant explicitly.

The small complex neighborhood here is an actual local domain for the inherited factor. It is not a theorem that every historical source readout lies in that neighborhood at later scales.

## 4. The actual second-link kernel and its regular minimum

Let the periodic lattice have n≥3 sites in each direction. Let I be any set of links such that no plaquette contains two members of I. Integrate all links in I exactly. Choose a retained link e. At most six members b₁,…,b_d of I share a plaquette with e, and each shares exactly one. Thus 0≤d≤6. Put F={e,b₁,…,b_d}. A plaquette meeting F has either one free link or the pair e,b_i; no other free pair occurs. There are 6+5d distinct affected plaquettes.

Let v denote all boundary links appearing in these plaquettes, and let S_v be the sum of their normalized actions a_p. Define the exact patch integral

\[
 Z_v(\zeta)=\int_{SU(2)^F}e^{-\zeta S_v(U_F)}\,dU_F.
 \tag{N2.16; P: actual two-stage patch kernel}
\]

Factors from already integrated links in I that share no plaquette with e are independent of every variable in F. They remain in the outside measure. They are not declared constant as functions of v.

Integrating the b_i first gives exactly

\[
 Z_v(\zeta)=e^{-6d\zeta}\int_{SU(2)}
 e^{-\zeta S^{\rm rem}_e(q;v)}
       \prod_{i=1}^d I\!\left(\zeta r_i(q;v)\right)dq,
 \tag{N2.17; P}
\]

where S_e^rem contains the 6−d plaquettes of e containing no b_i. This is the inherited non-Wilson conditional law. No I factor has been discarded or replaced by a fresh reference normalization.

### 4.1 The flat exterior, exactly

Set every boundary link to the identity. By choosing the inverse quaternion coordinate on a b_i when its orientation requires it, the actual joint action becomes

\[
 S_0(q,q_1,\ldots,q_d)
   =(6-d)(1-q_0)+\sum_{i=1}^d
        \left[5(1-q_{i,0})+1-q\cdot q_i\right].
 \tag{N2.18; P}
\]

The Haar measures are unchanged by these coordinate inversions. The six-staple norm of a leaf is r_i(q;0)=|5e₀+q|=√(26+10q₀). Minimizing the leaves for fixed q therefore gives the exact reduced classical action

\[
 E_d(q_0)=(6-d)(1-q_0)
       +d\bigl[6-\sqrt{26+10q_0}\bigr].
 \tag{N2.19; P}
\]

Writing s=1−q₀∈[0,2], direct differentiation gives

\[
 5\le \frac{dE_d}{ds}
      =(6-d)+\frac{5d}{\sqrt{36-10s}}
      \le\frac{15}{2},
 \qquad 5s\le E_d(1-s)\le\frac{15}{2}s.
 \tag{N2.20; P}
\]

In particular q=e₀ is the unique reduced minimum, and its Hessian in q=(√(1−|y|²),y) is (6−d/6)I₃. For the joint action the Hessian is three copies of the star matrix 6I−Adj(star_d); its smallest eigenvalue is at least 6−√6.

A global joint coercivity estimate is also elementary. Put a(q)=1−q₀. The inequality a(q)≤2a(q_i)+2(1−q·q_i) and nonnegativity give

\[
 \frac12\sum_{b\in F}a(q_b)
       \le S_0(U_F)\le12\sum_{b\in F}a(q_b).
 \tag{N2.21; P}
\]

For the lower bound with d≥1, the single leaf term 5a(q₁)+(1−q·q₁) pays a(q)/2+4a(q₁), while the other leaf pins are nonnegative. The d=0 case is immediate. For the upper bound use 1−q·q_i≤2a(q)+2a(q_i). Thus the patch has no unremoved gauge zero mode under its fixed flat boundary.

### 4.2 A fixed real regular exterior neighborhood

Write each boundary link as exp(A_ℓ) in one identity chart, with real A_ℓ∈su(2), and define δ²=Σ_ℓ|A_ℓ|² using a fixed invariant norm. The number of boundary links is bounded by an absolute constant because |F|≤7. We require δ≤δ₀, with δ₀ fixed sufficiently small. The statement can be applied after a unitary gauge transformation placing the boundary in this chart; this note does not assert that every historical readout admits such a gauge.

For arbitrary q∈SU(2), the five leaf staples not involving e are O(δ) from their flat values, and the remaining staple is an orthogonal image of q with O(δ) changes in its coefficients. Therefore

\[
 r_i(q;v)\ge4-C\delta\ge3,
 \qquad
 E_v^{\rm red}(q):=S_e^{\rm rem}(q;v)
                       +\sum_{i=1}^d[6-r_i(q;v)]
 \tag{N2.22; P for sufficiently small δ₀}
\]

is smooth in q,v, with uniform derivatives of each fixed order. Its C^s difference from the flat E_d is at most C_sδ, for any fixed s. This follows by differentiating the finitely many matrix products and the square root on r_i≥3; it does not differentiate through r_i=0.

**Lemma 4.1 (P): uniform regular minimum.** There is a unique global minimizer q_*(v) of E_v^red. It lies O(δ) from the identity, depends real-analytically on v, and has a uniformly positive Hessian. Define

\[
 E_*(v)=\min_qE_v^{\rm red}(q)=\min_{U_F}S_v(U_F).
 \tag{N2.23; P}
\]

Then 0≤E_*(v)≤Cδ². On one fixed local coordinate ball about q_*(v), the reduced action above its minimum is bounded above and below by positive constant multiples of the squared coordinate distance. On the complement of a smaller fixed ball it has a uniform positive gap. The corresponding assertions hold for the joint action on SU(2)^F.

**Proof.** At v=0, (N2.20) gives a positive gap away from a fixed small identity neighborhood and a positive Hessian within a sufficiently small coordinate ball. The uniform C² perturbation bound preserves strict convexity on that ball for δ₀ small. The implicit-function theorem, with its uniformly invertible Hessian, produces a critical point O(δ) from the identity. Strict convexity makes it unique within the ball. The global gap persists under the uniform C⁰ perturbation, so every global minimum lies in the same ball; hence the critical point is the unique global minimum. Taylor's formula and the uniform Hessian bounds give local quadratic comparability. Choosing the ball and δ₀ in this order yields constants independent of the torus and τ.

The reduced and joint minima coincide because each leaf minimization is exact and r_i≥3 gives its unique minimizing quaternion. Evaluating the original plaquettes at identity internal links gives S_v≤Cδ², while the real compact action is nonnegative. This proves the ground-energy bound. The same perturbation proof applies directly to the joint action using (N2.21) and its explicit Hessian. Real analyticity of the minimizer follows from the analytic implicit-function theorem on these fixed charts. ∎

The lemma is a uniform statement for the actual finite second-step patch with a regular boundary. It is not an estimate for arbitrary frustrated exteriors or for a patch whose number of historical variables grows with ultraviolet depth.

## 5. Uniform complex-coefficient Laplace estimate for that actual kernel

We give the quantitative argument because a merely real stationary-point statement would not control the normalized complex source.

### 5.1 A finite-dimensional lemma with uniform parameter derivatives

Let M be one fixed compact smooth manifold, of dimension D bounded by a fixed number. Let E_v be a real smooth family with the following verified properties on a compact real parameter neighborhood: one global minimum x_*(v), a uniformly positive Hessian there, a common local coordinate ball with quadratic upper/lower bounds, and a uniform positive gap outside a smaller ball. Assume the derivatives needed below are uniformly bounded. Let a_ζ(x,v) be holomorphic in ζ on a right sector |arg ζ|<θ<π/2 and have the form a₀(x,v)+η_ζ(x,v), where a₀(x_*(v),v)≥c>0 and the required spatial and first two parameter derivatives of η_ζ are bounded by C/|ζ|. The integration density is included in a_ζ in the local chart.

**Lemma 5.1 (P).** For |ζ| sufficiently large on an inner right sector,

\[
 \int_M e^{-\zeta E_v(x)}a_\zeta(x,v)\,dx
 =e^{-\zeta E_*(v)}\zeta^{-D/2}A(v)
          \exp\rho_v(\zeta),
 \quad
 A(v)=\frac{(2\pi)^{D/2}a_0(x_*(v),v)}{\sqrt{\det H(v)}},
 \tag{N2.24; P under the stated explicit finite-dimensional hypotheses}
\]

where A(v) is uniformly bounded above and below, the integral is nonzero, and

\[
 |\partial_v^\alpha\partial_\zeta^m\rho_v(\zeta)|
     \le m!C_\alpha^{m+1}|\zeta|^{-m-1},
       \qquad |\alpha|\le2,\quad m\ge0.
 \tag{N2.25; P}
\]

The branch in (N2.24) is the positive real one when the integral and amplitude are positive at real ζ, continued by the displayed nonvanishing factorization.

**Proof.** Translate local coordinates to the minimum and insert a smooth radial cutoff equal to one on a smaller ball. The cutoff is fixed in the translated coordinates. Taylor's formula gives
E_v(x)−E_*(v)=xᵀH(v)x/2+T₃(v,x)+O(|x|⁴),
where T₃ is homogeneous of degree three, and
a₀(x,v)=a₀(0,v)+a₁(v)·x+O(|x|²).
These estimates and their first two v derivatives are uniform. Choose the ball small enough that C|x|³ is absorbed by a fixed fraction of Re ζ times the quadratic form, throughout the chosen sector.

Expand the nonquadratic exponential through its cubic term. The error is bounded, after multiplication by a slightly weakened Gaussian, by a fixed constant times
|ζ||x|⁴+|ζ|²|x|⁶.
The linear amplitude term and the constant-amplitude cubic term integrate to zero against the even Gaussian and radial cutoff. The surviving amplitude error is O(|x|²); its product with the cubic term contributes at most C|ζ||x|⁴. Gaussian moment scaling therefore bounds every error by \(C|\zeta|^{-D/2-1}\). The η_ζ term has the same bound directly from its C/|ζ| estimate. Replacing the cutoff Gaussian by the full Gaussian costs an exponentially small tail. The latter integral is exactly \((2\pi)^{D/2}\zeta^{-D/2}(\det H)^{-1/2}\), with the principal power of ζ.

On the complement of the local ball, the phase gap bounds the integral by \(Ce^{-c\operatorname{Re}\zeta}\) after factoring out \(e^{-\zeta E_*}\). This is smaller than the required power. Thus the normalized integral equals A(v)+O(|ζ|⁻¹). Since A(v)≥c, increasing the coefficient threshold makes the relative error smaller than 1/2. Its logarithm defines ρ and proves |ρ|≤C/|ζ| and nonvanishing.

For the first two parameter derivatives, differentiate the same translated-coordinate expansion. Derivatives of the quadratic Gaussian introduce factors ζ times a quadratic polynomial; two derivatives can introduce their products. Each such factor is neutral under Gaussian scaling. Derivatives of T₃ remain cubic, and derivatives of the linear amplitude remain linear, so the odd cancellations persist. Every remaining term keeps at least one extra inverse power of |ζ|. Derivatives of the moving-chart cutoff in the complementary integral are supported in a region with the same positive gap and have exponentially small contributions. This proves the first two parameter bounds for the normalized error, and hence for ρ. Finally, a disk of radius c|ζ| inside the outer sector gives the coefficient derivatives by Cauchy's estimate. ∎

The proof works in any of the finitely many patch dimensions D≤21 with common constants after taking their maximum. No infinite-dimensional stationary-phase assertion is used.

### 5.2 Verification for the inherited I-factor marginal

Apply (N2.3) and (N2.7) to every factor in (N2.17). Since r_i(q;v)≥3 on the whole real integration manifold,

\[
 Z_v(\zeta)=c_H^d\zeta^{-3d/2}
       \int_{SU(2)}e^{-\zeta E_v^{\rm red}(q)}
          \left(\prod_{i=1}^d r_i(q;v)^{-3/2}\right)
          \exp\!\left(\sum_{i=1}^d\mathscr R(\zeta r_i(q;v))\right)dq.
 \tag{N2.26; P: unchanged inherited marginal}
\]

All fixed-order q and v derivatives of the last exponential minus one are O(|ζ|⁻¹). Indeed, differentiating 𝓡(ζr) produces ζ^j𝓡^(j)(ζr) multiplied by bounded derivatives of r, and (N2.5) bounds each by C_j/|ζ|. The leading amplitude ∏r_i⁻³ᐟ² is positive and bounded above and below. Lemma 4.1 verifies the phase hypotheses. Thus Lemma 5.1 applies with D=3 after the exact first integration; its prefactor accounts for the other 3d modes.

### Theorem 5.2. Exact second-step regular-kernel expansion — P

For every actual patch in §4 and every real regular exterior δ≤δ₀,

\[
 Z_v(\zeta)
   =e^{-\zeta E_*(v)}\zeta^{-\nu}A(v)\exp\rho_v(\zeta),
 \qquad \nu=\frac32(d+1),\qquad 0<c\le A(v)\le C,
 \tag{N2.27; P}
\]

on one fixed right sector with |ζ|≥τ₀, with the bounds (N2.25). The constants are uniform in the torus, spacing, patch position, d≤6 and regular exterior. At the flat exterior,

\[
 E_*(0)=0,\qquad
 A(0)=c_H^{d+1}\bigl[6^{d-1}(36-d)\bigr]^{-3/2}.
 \tag{N2.28; P}
\]

The expression includes d=0, since 6⁻¹·36=6. Formula (N2.28) follows either by the reduced Hessian and exact leaf prefactors or from the joint Hessian in (N2.18). It checks the fluctuation count and does not discard any old mass.

There is also a useful boundary-sensitive improvement. Simultaneous conjugation of every boundary and internal link leaves S_v, Z_v, E_*(v) and A(v) invariant. In boundary Lie-algebra coordinates at the identity, the tangent space is a direct sum of adjoint SU(2) representations, with no invariant linear functional. Therefore every first boundary derivative of ρ_v(ζ) vanishes at v=0. Taylor's formula with (N2.25) yields

\[
 |\partial_\zeta^m[\rho_v(\zeta)-\rho_0(\zeta)]|
       \le m!C^{m+1}\delta^2|\zeta|^{-m-1},
       \qquad m\ge0.
 \tag{N2.29; P}
\]

For m=0 this is the real parameter Taylor estimate, uniform on the complex coefficient sector. For all m, apply coefficient Cauchy to that difference on a smaller sector. The real regularity of the exterior is essential here: this theorem has not claimed a common complex exterior domain for the complete second-step integral. The first inherited factor itself does have the complex exterior domain proved in §3.

## 6. A fixed complex exterior domain and normalized second-step source theorem

The real estimate in §5 can be strengthened to a common complex exterior neighborhood. The key point is an exact holomorphic change-of-variables identity, not an unproved displacement of an integration contour.

### 6.1 Holomorphic centering of the actual compact integral

Use the boundary Lie-algebra coordinates v from §4, now complex. Extend the normalized SU(2) action holomorphically as 1−Tr(U_p)/2 on SL(2,C); on SU(2) the trace is real, so this agrees with the physical action. The invertible joint Hessian in (N2.18) gives a unique holomorphic critical point U_*(v)∈SL(2,C)^F near the identity, for ‖v‖<δ₁ with a fixed δ₁>0. At real v it is the real minimum in Lemma 4.1. Put

\[
 \mathcal E(v)=S_v(U_*(v)),\qquad
 F_v(Q)=S_v(U_*(v)Q)-\mathcal E(v),
 \tag{N2.30; P: componentwise left multiplication}
\]

where Q∈SU(2)^F in the integral. At v=0, U_*=1 and F₀=S₀. For every complex v in the neighborhood, F_v(1)=0 and its first internal derivative at 1 is zero.

For real v, Haar invariance gives an exact equality. Both sides are holomorphic in the complex boundary coordinates and ζ, so the identity theorem extends it:

\[
 Z_v(\zeta)=e^{-\zeta\mathcal E(v)}
                \int_{SU(2)^F}e^{-\zeta F_v(Q)}dQ.
 \tag{N2.31; P on a fixed complex boundary neighborhood}
\]

The identity theorem applies because the two holomorphic functions agree on an open set of the real form in the boundary coordinate space; iterating the one-variable identity theorem proves equality on its complex neighborhood. No assertion that complex left multiplication preserves the real Haar contour is needed.

Define d(Q,1)²=Σ_b(1−q_{b,0}) on the real integration manifold. Analyticity on a larger boundary neighborhood and compactness of that manifold give a uniform C² estimate F_v−S₀=O(‖v‖). Its value and first internal derivative vanish at Q=1, hence in a fixed identity chart it obeys the stronger estimate C‖v‖d(Q,1)². Off that chart, d(Q,1)² is bounded below, so the global C⁰ estimate gives the same conclusion with a larger constant. Therefore

\[
 |F_v(Q)-S_0(Q)|\le C\|v\|d(Q,1)^2,
 \qquad
 \operatorname{Re}\{\zeta F_v(Q)\}
      \ge c|\zeta|d(Q,1)^2
 \tag{N2.32; P}
\]

for one fixed right sector |arg ζ|≤θ<π/2 and all ‖v‖≤δ₂ sufficiently small. The second inequality uses (N2.21), Re ζ≥|ζ|cos θ and the first inequality. These are global bounds on the entire unchanged compact integration manifold.

The local centered Hessian H(v) is holomorphic, symmetric and a small perturbation of the positive matrix H(0). In the fixed identity chart the normalized Haar density is independent of v and even in the real chart variables. The proof of Lemma 5.1 now applies uniformly for complex v: the complex Gaussian still has an even integrand and a positive real part in its quadratic exponent, so the cubic odd term integrates to zero. Its Gaussian integral is given by the determinant branch continued from v=0. The global tail is controlled by (N2.32). We obtain

\[
 Z_v(\zeta)=e^{-\zeta\mathcal E(v)}\zeta^{-\nu}
       \mathcal A(v)\exp\varrho(v,\zeta),\qquad
 |\varrho(v,\zeta)|\le C|\zeta|^{-1},\qquad
 0<c\le|\mathcal A(v)|\le C,
 \tag{N2.33; P, jointly holomorphic}
\]

on a fixed complex boundary ball and coefficient sector. Here ν=3(d+1)/2 and 𝒜(v) is the centered Haar Gaussian determinant. On the real slice 𝒜=A and ϱ=ρ from §5. The uniform coefficient threshold ensures that the normalized error is smaller than 1/2, so all logarithms and the zero-free assertion have been proved on this joint domain.

Use a strictly larger boundary ball and coefficient sector when applying Cauchy's inequalities. On an inner domain,

\[
 |\partial_v^\alpha\partial_\zeta^m\varrho(v,\zeta)|
     \le\alpha!m! C^{|\alpha|+m+1}|\zeta|^{-m-1}.
 \tag{N2.34; P}
\]

The boundary dimension is uniformly bounded for these patches; its fixed factors are included in C. The same global conjugation invariance as in §5 kills the first v derivative at zero. Thus, writing Δϱ(v,ζ)=ϱ(v,ζ)−ϱ(0,ζ),

\[
 |\partial_\zeta^m\Delta\varrho(v,\zeta)|
     \le m!C^{m+1}\|v\|^2|\zeta|^{-m-1},\qquad
 |\mathcal E(v)|\le C\|v\|^2.
 \tag{N2.35; P}
\]

The second bound follows either from the same color invariance and analyticity, or directly from the absence of a linear trace term at the identity. At real v, 𝓔(v)=E_*(v)≥0. No positivity is asserted at complex v.

### Theorem 6.1. Actual normalized second-integration source — P

Let τ≥τ₁, ‖v‖≤δ₃ and |z|<cτ, with fixed positive τ₁,δ₃,c and the domain margins just described. Use the same deterministic flat-patch subtraction on every exterior:

\[
 L_{\tau,F}(z)=\log\frac{Z_0(\tau-z)}{Z_0(\tau)},\qquad
 \mathcal P_{\tau,F}(z;v)
      =\log\frac{Z_v(\tau-z)}{Z_v(\tau)}-L_{\tau,F}(z).
 \tag{N2.36; P: literal patch source and local flat vacuum}
\]

These functions are holomorphic on the stated coefficient/exterior domains and satisfy

\[
 \mathcal P_{\tau,F}(z;v)
   =z\mathcal E(v)+\Delta\varrho(v,\tau-z)
                         -\Delta\varrho(v,\tau),\qquad
 |\mathcal P_{\tau,F}(z;v)-z\mathcal E(v)|
       \le C|z|\|v\|^2\tau^{-2}.
 \tag{N2.37; P}
\]

For every m≥1,

\[
 \left|\partial_z^m\bigl(\mathcal P_{\tau,F}(z;v)
                       -z\mathcal E(v)\bigr)\big|_{z=0}\right|
      \le m!C^{m+1}\|v\|^2\tau^{-m-1}.
 \tag{N2.38; P}
\]

The remainder is jointly holomorphic and vanishes to second order at the flat exterior, so its full field derivatives have the fixed-margin bounds obtained from (N2.34). In particular this is a source estimate on an actual complex regular-field domain, not only at a real saddle.

**Proof.** Substitute (N2.33) into (N2.36). The powers −νlog ζ cancel between the true patch and its flat comparison. The determinant term log𝒜(v) is independent of ζ and cancels from each ratio. The two critical actions leave exactly z𝓔(v), since 𝓔(0)=0. This proves the identity. Integrate the m=1 coefficient bound in (N2.35) along τ−tz, 0≤t≤1, to obtain the remainder estimate. Direct coefficient differentiation or Cauchy proves every higher source bound. ∎

The predictable term is the actual minimum energy of the finite joint patch, continued holomorphically; it is not set equal to zero. The deterministic vacuum L_{τ,F} depends only on the patch type and τ,z. The source changes the coefficient of every plaquette in that patch and no other plaquette.

### 6.2 Normalization under an arbitrary true outer law on the regular domain

Let λ(dv) be any positive exterior measure supported on the real regular domain ‖v‖≤δ₃, with 0<∫Z_v(τ)λ(dv)<∞. It may contain arbitrary additional source-independent outside weights and survivor masses, provided they are independent of the integrated variables F and therefore genuinely belong to λ. Then the actual normalized patch expectation is

\[
 e^{-L_{\tau,F}(z)}
 \frac{\int Z_v(\tau-z)\lambda(dv)}
      {\int Z_v(\tau)\lambda(dv)}
   =\frac{\int Z_v(\tau)e^{\mathcal P_{\tau,F}(z;v)}\lambda(dv)}
          {\int Z_v(\tau)\lambda(dv)},
 \qquad
 \left|\cdot\right|\le e^{C|z|\delta_3^2}.
 \tag{N2.39; P}
\]

This follows pointwise from (N2.37) and |𝓔(v)|≤Cδ₃², then by integrating with precisely the same outside law. No exterior replacement, inverse rare-component estimate or separate reference mass is used. We have thus normalized an actual two-stage regular patch, including its first inherited I factors, under every positive outer law allowed by its stated support.

Weights depending on the still-integrated old links are part of the inner kernel and cannot be placed in λ to invoke (N2.39). Arbitrary compulsory large-field constraints are not covered by the regular-support assumption. Those are material restrictions on the theorem, not notational qualifications.

### 6.3 The old first-step source is exactly the source in the second integral

For SU(2), let μ_red,τ,v be the normalized actual q-law in (N2.17), retaining its product of I factors. Let L_1,τ(z) be the one-link flat-star vacuum from [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md). The source after the d first integrations is exactly

\[
 \Psi_\tau(z;q,v)=zS_e^{\rm rem}(q;v)
                         +\sum_{i=1}^d\Phi_\tau(z;r_i(q;v)).
 \tag{N2.39a; P: actual inherited source readout}
\]

Using the first-link identity on each leaf, with no change of q or of its exterior, gives

\[
 \log\mathbb E_{\mu_{\rm red,\tau,v}}e^{\Psi_\tau(z;q,v)}
   =\log\frac{Z_v(\tau-z)}{Z_v(\tau)}-dL_{1,\tau}(z).
 \tag{N2.39b; P}
\]

Therefore the deterministic vacuum for the second integration is

\[
 L_{2,\tau,F}(z)=L_{\tau,F}(z)-dL_{1,\tau}(z),\qquad
 \log\mathbb E_{\mu_{\rm red,\tau,v}}e^{\Psi_\tau}
           -L_{2,\tau,F}(z)=\mathcal P_{\tau,F}(z;v).
 \tag{N2.39c; P}
\]

This identifies Theorem 6.1 as an actual iterated-source theorem: it integrates the old exterior-dependent Φ terms under their genuine new marginal. It does not replace them by newly centered Wilson sources. The joint subtraction L_F includes the first vacua; if those have already been removed, only L_2 is removed at the next step. This prevents double subtraction.

For real regular v all expectations above are with positive normalized measures. On the stated complex domain the same identities hold by their zero-free analytic continuations. The plaquette-disjoint geometry ensures that no source plaquette has been counted twice.

## 7. All SU(N), independent plaquette sources and inherited regular weights

### 7.1 The finite second-step theorem for every SU(N)

The second-step proof does not fundamentally require the explicit SU(2) Haar integral. For G=SU(N), use normalized trace tr=Tr/N and

\[
 a(U)=1-\operatorname{Re}\operatorname{tr}U,\qquad
 a^{\rm hol}(U)=1-\tfrac12\operatorname{tr}(U+U^{-1}),\qquad
 \tau=N\beta_a,\quad z=Nj.
 \tag{N2.40; P: exact P2 normalization and holomorphic extension}
\]

Keep the same star-patch geometry F. At the flat exterior its joint action, after any required leaf inversions, is

\[
 S_0(U,V_1,\ldots,V_d)
 =(6-d)a(U)+\sum_{i=1}^d[5a(V_i)+a(UV_i^{-1})].
 \tag{N2.41; P}
\]

The normalized Hilbert–Schmidt distance satisfies ‖U−I‖²=2a(U). Its triangle inequality gives a(U)≤2a(V)+2a(UV⁻¹), so the same global comparison (N2.21) holds. In a basis with −tr(T_AT_B)=δ_AB, the flat Hessian is N²−1 copies of 6I−Adj(star_d). It is strictly positive with the same scalar gap. Therefore the regular minimum, holomorphic critical point and global centered coercivity proofs apply verbatim on SL(N,C)^F.

Normalized Haar measure has a positive real-analytic density in an identity chart. In exponential coordinates that density is even, because Haar measure is invariant under inversion. The finite-dimensional Laplace proof consequently has the same odd-cubic cancellation. Equations (N2.33)–(N2.39) hold for every SU(N), with

\[
 \nu=\frac{(d+1)(N^2-1)}2,\qquad
 \mathcal A(0)=c_N^{d+1}
      [6^{d-1}(36-d)]^{-(N^2-1)/2},
 \quad c_N=(2\pi)^{(N^2-1)/2}J_N(0)>0,
 \tag{N2.42; P}
\]

where J_N(0) is the normalized Haar density in the stated orthonormal exponential coordinates. For N=2 these agree with (N2.28). Constants may depend on N, never on cutoff or volume. For N>2 the first leaf integral need not be written in closed form; Fubini identifies the joint integral with the exact two-stage marginal, and all its masses remain in the proof.

### 7.2 A joint domain for independent plaquette coefficients

Let P(F) be the 6+5d affected plaquettes. Give them independent coefficients w_p near one and set S_{w,v}=Σ_pw_pa_p^hol. The weighted joint phase is linear in w. Its flat critical point remains the identity, and its Hessian is a small perturbation of the positive star Hessian. The critical-point, centering and coercivity proofs above apply jointly for complex ‖w−1‖∞<ε and ‖v‖<δ, with fixed ε,δ. Thus

\[
 Z_\tau(w,v)
   =e^{-\tau\mathcal E(w,v)}\tau^{-\nu}
       \mathcal A(w,v)\exp\varrho(w,v,\tau),
 \qquad |\varrho|\le C\tau^{-1},
 \tag{N2.43; P, jointly holomorphic}
\]

with fixed domain margins and all Cauchy derivatives. The exact centered identity is first proved for real positive w and real v and then extended in all parameters. Its global perturbation estimate is
|F_{w,v}−S₀|≤C(‖w−1‖+‖v‖)d(Q,1)².
This supplies the uniform complex coercivity needed for (N2.43).

At v=0, every plaquette is flat at the critical point, so 𝓔(w,0)=0 for every admitted w. Define

\[
 D(w,v)=\log\mathcal A(w,v)-\log\mathcal A(w,0),\qquad
 R(w,v,\tau)=\varrho(w,v,\tau)-\varrho(w,0,\tau).
 \tag{N2.44; P}
\]

Global color conjugation gives no linear v term in any of 𝓔, D or R. On inner domains their norms and fixed-order w derivatives obey

\[
 |\mathcal E(w,v)|+|D(w,v)|\le C\|v\|^2,
 \qquad |R(w,v,\tau)|\le C\|v\|^2\tau^{-1}.
 \tag{N2.45; P}
\]

Their useful homogeneity identities follow from the same actual weighted phase:

\[
 \mathcal E(tw,v)=t\mathcal E(w,v),\qquad
 D(tw,v)=D(w,v),\qquad
 R(tw,v,\tau)=R(w,v,t\tau),
 \tag{N2.46; P for t near one}
\]

The critical point is unchanged when all weights are multiplied by t. Its Hessian scales by t, so \(\mathcal A(tw,v)=t^{-\nu}\mathcal A(w,v)\); that factor cancels in D. Comparing the two exact factorizations proves the last identity. All powers and logarithms use the common branch at t=1.

### Theorem 7.1. Spatial two-jet admission for the actual second patch — P

Put w_p=1−z_p/τ and subtract the same flat-patch source vacuum. The exact local source logarithm is

\[
 \begin{aligned}
 \mathcal P_\tau(\mathbf z;v)
  &=\tau[\mathcal E(\mathbf1,v)-\mathcal E(\mathbf1-\mathbf z/\tau,v)]\\
  &\quad+D(\mathbf1-\mathbf z/\tau,v)-D(\mathbf1,v)
      +R(\mathbf1-\mathbf z/\tau,v,\tau)-R(\mathbf1,v,\tau).
 \end{aligned}
 \tag{N2.47; P}
\]

It is jointly holomorphic on ‖z‖∞<cτ and ‖v‖<δ. For any direction f on the affected plaquettes, choose a constant f₀ and write f=f₀1+f_⊥, with ω(f)=‖f_⊥‖∞. The first and second source jets at zero satisfy

\[
 \begin{aligned}
 |\mathcal P_f-f_0\mathcal E(\mathbf1,v)|
   &\le C\|v\|^2\left[\omega(f)+\frac{\omega(f)}\tau
                                +\frac{\|f\|_\infty}{\tau^2}\right],\\
 |\mathcal P_{fg}|
   &\le C\|v\|^2\left[
       \frac{\omega(f)\omega(g)}\tau
       +\frac{\|f\|_\infty\omega(g)+\|g\|_\infty\omega(f)}{\tau^2}
       +\frac{\|f\|_\infty\|g\|_\infty}{\tau^3}\right].
 \end{aligned}
 \tag{N2.48; P}
\]

One may choose f₀=f at any reference plaquette, so ω(f) is bounded by the maximum variation over the patch. Sampling a smooth profile gives ω(f)≤Ca‖∇f‖∞ because the patch diameter is O(a). The same statement holds in the scaled lattice units used for a fixed local transformation.

**Proof.** Formula (N2.47) is the exact quotient of (N2.43) and its flat counterpart; no deterministic counterterm is fitted to a nonflat exterior. Cauchy's bounds and (N2.45) control every w derivative. Degree-one homogeneity gives E′[1]=E and E″[1,h]=0. Degree-zero homogeneity gives D′[1]=0 and D″[1,h]=−D′[h]. The identity for R gives R′[1]=τ∂_τR=O(‖v‖²/τ). These identities yield the first estimate after differentiating (N2.47).

For the second derivative, the three exact terms are −τ⁻¹E″[f,g], τ⁻²D″[f,g] and τ⁻²R″[f,g]. The first term only sees f_⊥ and g_⊥. The second contains their transverse-transverse term and the two radial-transverse terms just identified; its radial-radial term is zero. The last term is bounded by C‖v‖²‖f‖‖g‖/τ³. This proves (N2.48), including the constant-source improvement. All operations take place on fixed enlarged domains, so the same bounds have fixed-margin field derivative estimates. ∎

For real regular v and real weights, there is an exact interpretation of the leading field-valued second contact. Let H be the positive Hessian of S_{1,v} at its critical point and let G_f be the internal gradient there of Σ_pf_pa_p. Differentiating the critical equation gives

\[
 \mathcal E''(\mathbf1,v)[f,g]
       =-\langle G_f,H^{-1}G_g\rangle,
 \qquad G_{\mathbf1}=0.
 \tag{N2.49; P}
\]

Thus the leading second source term is τ⁻¹ times this positive Gram form. It vanishes when either source direction is constant. It is a field-dependent coefficient, not a vacuum constant. Retaining and extracting it is part of a complete source induction.

### 7.3 Stability under actual admitted regular inner interactions

The compact patch theorem remains valid if the actual inner kernel is multiplied by e^{B(U_F,v)}, subject to the following explicit conditions: B is real on real fields, gauge invariant under simultaneous conjugation, source independent during the displayed source variation, and holomorphic with a fixed bound on a complex neighborhood of the entire real compact integration manifold and the boundary ball. The radius and bound must be uniform in the cutoff. They may depend on the fixed local construction constants.

To prove this, retain e^B in the exact centering identity (N2.31). It becomes the analytic amplitude e^{B(U_*(w,v)Q,v)}. Its value at Q=1 is nonzero, and its derivatives are uniformly bounded on a smaller domain. The same Laplace proof applies. The leading determinant factor is multiplied by e^{B(U_*(w,v),v)}; because U_*(tw,v)=U_*(w,v), this extra factor preserves the degree-zero identity for D. The remainder and all estimates have constants depending on the amplitude bound and radius. A family B_τ is allowed if it is frozen as τ−z is varied and has those same uniform bounds; no derivative of its arbitrary baseline τ dependence is assumed. For such a family, keep the baseline label τ₀ fixed in coefficient identities: R_{τ₀}(tw,v,ζ)=R_{τ₀}(w,v,tζ). The right side does not replace B_{τ₀} by B_{tτ₀}.

This is a stability theorem for genuine admitted inner activities. It does not assert that all old E/R/B terms, hard selectors, compulsory masses or their source jets satisfy the stated amplitude hypotheses. A hard constraint that deletes the regular minimum, an amplitude with no uniform analytic neighborhood, or an inherited physical source depending on earlier variables requires a separate proof. Dropping such a factor to apply this theorem would change the kernel.

## 8. What this closes, and the precise remaining R2 work

### 8.1 Completed local statements

This note proves a genuine second integration of the physical source. The old first-step I factors remain in the law, the old predictable source Φ remains its actual function of the next link, and the two deterministic vacuum subtractions telescope exactly. The normalized estimate is uniform under any positive outer law supported on the proved regular exterior domain. The compact-patch argument also gives an all-SU(N) theorem and a fixed complex domain for independent plaquette sources, with explicit first and mixed-second estimates and the field-valued Gram contact.

The admitted inner amplitude theorem shows that the result is stable under genuinely bounded holomorphic source-independent regular interactions. Its hypotheses have not been asserted for unclassified old activities. These are P theorems in their finite-patch domains, not a conditional restatement of the desired full R2 estimate.

The resulting exact kernel has the next effective form

\[
 K_{F,\tau}(v)=e^{-\tau\mathcal E(v)}\tau^{-\nu}
                   \mathcal A(v)e^{\varrho(v,\tau)}.
 \tag{N2.50; P: actual output of the second patch integration}
\]

Its source is z𝓔(v) plus the proved analytic correction after the stated deterministic subtraction. The factor ‖v‖² is a norm in the fixed local field chart; it is not by itself the physical dimension-four scale factor or a replacement for a physical-cell root count. Those require the actual gauge-field extraction and endpoint-scale dictionary. This is the next literal inherited interaction. Treating it as an unchanged Wilson plaquette action would again be incorrect. The tensor/field projection and domain admission of these outputs in a complete RG step remain to be matched to the actual construction.

### 8.2 Why the regular theorem does not cover arbitrary compulsory histories

A simple actual one-link degeneration illustrates the restriction. A real exterior with cancelling staples has r=0 and constant star action six. Its integral is \(e^{-6\tau}\), rather than a nondegenerate three-mode Laplace integral. For a fixed small real source z, flat subtraction gives

\[
 \Phi_\tau(z;0)=6z-L_{1,\tau}(z)
       =6z-\frac{3z}{2\tau}+O(\tau^{-2})
 \quad(\tau\longrightarrow\infty).
 \tag{N2.51; P for fixed z}
\]

The sector expansion proves the last equality. Thus even the improved O(zτ⁻²) error relative to the actual minimum energy is false uniformly over all real exteriors: the fluctuation rank changes at such a frustrated exterior. The all-exterior theorem of [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md) retains an O(z/τ) correction. This is not a counterexample to R2; a complete construction must assign the degenerate configurations to the appropriate raw/large-field treatment and retain their real weights.

The remaining full R2 input is still an estimate for the actual post-E/post-erased-R compulsory system. It must cover the following concrete failures of the local theorem's hypotheses:

1. Inner selectors or constraints can remove the regular minimum or leave a mass depending on the exterior. They cannot be placed into the outer measure if they depend on an integrated old link.
2. Historical source readouts need not equal the current patch energy. They must be carried through their actual old kernels, including their field-valued contacts and boundary terms.
3. The number, scales and analytic radii of retained historical variables are not bounded by the finite star-patch geometry. The constants above cannot simply be multiplied through ultraviolet depth.
4. The local flat subtraction used here must be assembled into one consistent source-local vacuum recipe. The two-step telescoping identity is proved; complete E/R vacuum copying, overlapping patch bookkeeping and the eventual physical-cell count are not.

A full proof may use the complete-patch fractional comparison or the all-history complex-pressure route stated in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md). This note supplies an actual regular normalized kernel for that effort. It does not supply the complementary compulsory-history estimate or its averaged payment under the true outer measure.

### 8.3 Suggested next exact calculation

Insert the output (N2.50), its independently weighted source jets (N2.47)–(N2.49), and the actual remaining boundary/constraint factors into one named Balaban mixed regular/R transition. Verify which factors satisfy the fixed complex amplitude hypothesis and which remain raw. Apply the regular theorem only to the former. For each raw factor, retain its old source readout and mass and prove the complete normalized comparison with its actual outer law. Then check that the extracted identity term agrees with the same local vacuum recipe on both branches.

That calculation would connect the new finite repeated-integration theorem to O–MR1/O–MR2 and the full R2 contract. It cannot be replaced by declaring a compulsory mass constant, assigning a fresh reference expectation to an old observable, or assuming a normalized bound from a raw component upper estimate.

**Full R2 status: O.** The new results close the first genuine iterated regular integration, including complex regular exteriors, all SU(N), spatial coefficient jets and an admitted-interaction stability theorem. They do not close the complete history construction, and no strengthened N2-F interface has been assumed.
