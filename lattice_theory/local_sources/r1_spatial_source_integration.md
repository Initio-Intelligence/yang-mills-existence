# Spatial sources and field-dependent contacts

## 1. Result, scope and the remaining complete-history gap

This note studies the R1 spatial source-integration estimate. It proves a new actual finite-lattice transition for the scalar source: exact SU(2) integration of one link, or of a plaquette-disjoint family of links, with six independently varying incident plaquette couplings. The source is evaluated on the original plaquettes. A deterministic flat-star subtraction is made, and the resulting interaction is kept as a function of the actual exterior links.

The result applies to an explicit complex regular exterior domain. It gives the local classical term, the fluctuation determinant term, the complete source-dependent remainder, and the first two spatial-source jets. The leading field-valued two-source contact has an exact transverse Gram form and annihilates the constant source direction. Consequently it carries two source oscillations; the next determinant contact carries at least one. The residual scalar constant-source response has the stronger inverse-coupling powers dictated by the exact integral.

These are uniform estimates for a genuine inherited interaction, not for a chosen comparison observable. The constants are independent of the torus and lattice spacing, and the complex field domain is explicit. No N-interface beyond N2-F is assumed; in fact the finite-lattice proofs here do not need N2-F.

**Full R1 remains O.** This note does not claim repeated admission of every inherited E/R/B term, a construction of a sourced minimizer, or normalized estimates for compulsory histories. The exact next conditional measure contains the inherited source-free interaction derived below. Replacing that measure by the original Wilson one-link law would change the problem. Section 8 states what the new local theorem closes and what it leaves open.

The source-free LFR operator bounds are recalled first. LFR II (1.65), p.375, admits the source-free reconstructed effective action in the stated complex domain. Equations (1.73)–(1.75), p.380, compare its complex extension with the same real old component mass. None of these source-free or conditional results automatically bounds the new physical source readout. They are not counted again here.

Labels are **P** for a proved statement with its displayed hypotheses, **L** for a checked primary assertion in its stated scope, **C** for an actual-theory application conditional on an explicitly unverified premise, and **O** for an outstanding proposition. Every display is labelled. The new one-link calculations below are P results derived directly from compact-group integration; no sourced Balaban theorem is imported.

## 2. Exact integration with six independent plaquette sources

Work on a four-dimensional periodic SU(2) lattice with distinct occurrences of the six plaquettes incident on a chosen positive link b. The compatible lattices in the program have this property. Use normalized plaquette action a_p=1−ReTr(U_p)/2. The literal P2 action is s_p=2a_p; consequently its coefficient is τ=2β_a and its scalar source on a plaquette is z_p=2j^{(0)}(x_p).

After conditioning on every link except b, write the six incident traces as ReTr(UV_i), where V_i are the oriented three-link staples. Let q∈S³ be the quaternion for U and v_i∈S³ the quaternion for V_i⁻¹. Then the six plaquette actions are a_i=1−q·v_i. For six possibly complex coefficients t_i set

\[
 T=\sum_{i=1}^6t_i,\qquad
 s_t=\sum_{i=1}^6t_iv_i,\qquad
 R^2=s_t\cdot s_t,
 \qquad
 a_{ij}=1-v_i\cdot v_j
       =1-\tfrac12\operatorname{Tr}(V_iV_j^{-1}).
 \tag{S1.1; P: definitions and exact SU(2) identities}
\]

The dot product is bilinear, not sesquilinear, when variables are complexified. Define the entire even function

\[
 I(\kappa)=\int_{S^3}e^{\kappa q_0}\,dq
 =\frac2\pi\int_{-1}^1e^{\kappa u}(1-u^2)^{1/2}\,du
 =\sum_{n\ge0}\frac{(\kappa^2/4)^n}{n!(n+1)!}.
 \tag{S1.2; P}
\]

The normalization gives I(0)=1. To obtain the series, the odd moments vanish by symmetry; substituting u² in the even moments gives the beta integral, and hence the stated coefficient. Rotational invariance gives the same series with κ² replaced by s_t·s_t. The identity initially holds for real s_t and extends to every complex s_t by polynomial identity in each homogeneous degree and normal convergence. Thus no square-root branch is needed for the following exact integral:

\[
 Z_b(t\mid v)
 :=\int_{S^3}\exp\!\left[-\sum_it_i(1-q\cdot v_i)\right]dq
 =e^{-T}I(R),
 \qquad
 R^2=T^2-2\sum_{i<j}t_it_j a_{ij}.
 \tag{S1.3; P}
\]

All original exterior fields remain in a_{ij}. These loop traces are gauge invariant: all staples have the same endpoints, and the relative products transform by conjugation. The formula is not evaluated on a newly selected reference field.

Start at t_i=τ>0 and insert the original source Σ_i z_i a_i, so t_i=τ−z_i. Write t_i=τw_i, s(w)=Σ_iw_i, and

\[
 A(w,a)=\sum_{i<j}w_iw_j a_{ij},\quad
 r(w,a)=\sqrt{s(w)^2-2A(w,a)},\quad
 W(w,a)=s(w)-r(w,a).
 \tag{S1.4; P: definitions on the regular branch specified in §3}
\]

At a=0, take r=s. Define the deterministic flat-star logarithmic subtraction and the actual subtracted conditional logarithm by

\[
 \begin{aligned}
 L_\tau(z)&=\sum_i z_i+\log I\!\left(6\tau-\sum_i z_i\right)-\log I(6\tau),\\
 \Phi_\tau(z;a)&=\log\mathbb E_{\tau,v}
        \exp\!\left(\sum_i z_i a_i\right)-L_\tau(z),\\
 \Gamma_\tau(w,a)&=\log I(\tau s(w))-\log I(\tau r(w,a)).
 \end{aligned}
 \tag{S1.5; P: definitions near zero source}
\]

For the real source-zero conditional law, expectation here uses its actual density proportional to exp(τq·Σ_iv_i), with normalized Haar measure. At complex exterior values, the logarithms are the holomorphic branches constructed below. The exact relation is

\[
 \Phi_\tau(z;a)=\Gamma_\tau(\mathbf1,a)
                    -\Gamma_\tau(\mathbf1-z/\tau,a),
 \qquad \Phi_\tau(0;a)=0.
 \tag{S1.6; P}
\]

The subtraction L_τ depends only on the six source values and τ. It is not the conditional mean at the physical exterior. It is invariant under permutations of those six source values, and it is the same flat reference for every star. Its eventual assembly into a common cell vacuum prescription is not claimed here.

## 3. A complex regular domain and a proved sector estimate

Choose fixed numerical ε_w,ε_a>0 sufficiently small; for example ε_w=1/16 and ε_a=1/10 can be decreased once if necessary. Regard the fifteen a_{ij} initially as independent complex variables and set

\[
 \mathcal D=\{\max_i|w_i-1|<\varepsilon_w,
                \ \mathcal A:=\sum_{i<j}|a_{ij}|<\varepsilon_a\}.
 \tag{S1.7; P: definition}
\]

On this domain |s| is bounded above and below by positive numerical constants, |2A/s²| is uniformly small, and the branch r=s(1−2A/s²)^{1/2} is holomorphic. In particular

\[
 |s|+|r|\le C,\quad |s|,|r|\ge c>0,\quad
 |\arg s|,|\arg r|<\pi/12,\qquad
 W=\frac{2A}{s+r},\quad |W|\le C\mathcal A.
 \tag{S1.8; P}
\]

The holomorphic extension to independent a variables is only a device for bounds. On actual complex staple matrices, use their literal trace values in (S1.1); no independence of those physical traces is asserted.

This domain has a direct regular-field meaning. If the six incident plaquette matrices P_i=UV_i belong, in one common base-point gauge, to a sufficiently small SL(2,C) neighborhood of I, then V_iV_j⁻¹ is conjugate to P_iP_j⁻¹. Hence |a_{ij}|≤C max_l‖P_l−I‖². One elementary proof uses det(I+B)=1+Tr B+det B in dimension two: for P=I+B∈SL(2,C), Tr B=−det B, so |1−Tr P/2|≤C‖B‖². The relative plaquette matrix differs from I by O(max_l‖P_l−I‖). Thus an ordinary fixed small regular plaquette domain lies in (S1.7). This does not assert that a later mixed reconstruction automatically stays there.

### Lemma 3.1. Sector asymptotics with a quantitative analytic remainder — P

There exist κ₀,C>0 such that on |arg κ|≤π/3 and |κ|≥κ₀,

\[
 I(\kappa)=\sqrt{\frac2\pi}\,e^\kappa\kappa^{-3/2}A_0(\kappa),
 \qquad
 A_0(\kappa)=1-\frac3{8\kappa}+O(|\kappa|^{-2}),
 \qquad |A_0-1|<\frac12.
 \tag{S1.9; P}
\]

The branches use the principal logarithm in the right half-plane. The function χ=log A₀ is analytic there at these large moduli. On the smaller sector |arg κ|≤π/6, |κ|≥2κ₀, its derivatives obey

\[
 |\chi^{(n)}(\kappa)|\le n!C^{n+1}|\kappa|^{-n-1},\qquad
 \left|\left(\chi(\kappa)+\frac3{8\kappa}\right)^{(n)}\right|
       \le n!C^{n+1}|\kappa|^{-n-2}
 \quad(n\ge0).
 \tag{S1.10; P}
\]

**Proof.** Substitute u=1−q₀ in the Haar integral (S1.2). After extracting e^κ, the integral becomes (2√2/π)∫₀²e⁻κu u^{1/2}√(1−u/2)du. The full half-line gamma integral for the constant term is Γ(3/2)κ⁻³ᐟ². The linear term −u/4 gives −3/(8κ) relative to it. The exact identity

\[
 \sqrt{1-v}-1+\frac v2
 =-\frac{v^2}{2(1+\sqrt{1-v})^2},\qquad 0\le v\le1,
 \tag{S1.11; P}
\]

bounds the remaining integrand by Cu². Its integral is O((Re κ)⁻⁷ᐟ²), hence gives O(|κ|⁻²) after multiplication by κ^{3/2}. The tails of the constant and linear gamma integrals beyond u=2 are exponentially small uniformly in this sector. The normalization constant is (2√2/π)Γ(3/2)=√(2/π). This proves (S1.9), and increasing κ₀ gives |A₀−1|<1/2. The logarithm then has χ=−3/(8κ)+O(|κ|⁻²). A disk of a fixed small fraction of |κ| around an inner-sector point stays in the outer sector with comparable modulus. Cauchy's formula gives both derivative bounds. ∎

This proof is also the sector lemma of [Inherited interactions in the second integration](r2_second_integration.md), Theorem 2.1, derived from the same elementary Haar integral. It uses no unproved Bessel asymptotic. In particular it proves the required zero-free statement rather than assuming a logarithm exists.

Choose τ₀ so large that τs and τr lie in the inner domain of this lemma for every (w,a)∈D and real τ≥τ₀. The same remains true on a fixed relative complex neighborhood of each such τ, after reducing its radius once. All logarithms in (S1.5) are therefore holomorphic on this common source/field domain.

## 4. Exact regular interaction and joint source/field admission

### Theorem 4.1. Spatial-source one-link admission — P

For τ≥τ₀ and (w,a) in the fixed domain D of §3, the actual flat-subtracted effective interaction has the exact decomposition

\[
 \Gamma_\tau(w,a)=\tau W(w,a)+D(w,a)+E_\tau(w,a),\qquad
 D(w,a)=\frac32\log\frac{r(w,a)}{s(w)},\qquad
 E_\tau=\chi(\tau s)-\chi(\tau r).
 \tag{S1.12; P}
\]

All three terms are holomorphic in the physical source and the loop variables. The remainder has the exact factorization and estimate

\[
 E_\tau=W B_\tau,\qquad
 B_\tau(w,a)=\tau\int_0^1
      \chi'\!\left(\tau[r+t(s-r)]\right)dt,
 \qquad
 B_\tau=\frac3{8\tau s r}+O(\tau^{-2}),
 \qquad |E_\tau|\le C\mathcal A/\tau.
 \tag{S1.13; P}
\]

The estimates are uniform in the lattice spacing, torus and actual exterior satisfying D. On any fixed smaller domain, for m,n≥0, the mixed coefficient derivatives of E obey

\[
 \begin{aligned}
 \|D_w^m E_\tau\|&\le m!C^{m+1}\tau^{-1}\mathcal A,\\
 \|D_a^n D_w^m E_\tau\|&\le n!m!C^{n+m+1}\tau^{-1}
                                      &&(n\ge1).
 \end{aligned}
 \tag{S1.14; P}
\]

The w directions use the maximum norm on C⁶ and the a directions the sum norm on C¹⁵. A fixed further τ derivative costs a corresponding factor τ⁻¹ with Cauchy factorials. In particular physical source derivatives of order m in z=τ(1−w) cost τ⁻ᵐ in (S1.14).

**Proof.** Substitute the sector factorization (S1.9) in the definition of Γ. The constants and powers of τ cancel between the two logarithms, giving (S1.12). The fundamental theorem of calculus along the segment from τr to τs gives (S1.13). That segment remains in the sector with modulus comparable to τ. Equation (S1.10) bounds χ' by Cτ⁻², so B is O(τ⁻¹). Using χ'=3/(8κ²)+O(κ⁻³) and integrating its leading term gives 3/(8τsr); the remainder is O(τ⁻²). Together with |W|≤C A this proves the value estimate.

Cauchy's formula on fixed smaller polydisks gives the derivative bounds. More explicitly, apply one Cauchy variable to a sum of m w directions with radii proportional to 1/m, and similarly for n a directions. The factor m^m is bounded by e^m m!, and n^n by e^n n!, so the displayed constants absorb polarization. For derivatives in w alone, the a variables remain fixed and the bound C A/τ persists on the whole w polydisk. Once an a derivative is taken, no factor A is claimed. The relative complex τ disk constructed in §3 gives the additional τ-derivative powers. ∎

The formula does not discard the classical interaction τW or the fluctuation determinant D. Both are present in the next actual exterior law. The residual E is an admitted bounded analytic local interaction after those two pieces are displayed explicitly. It has an inverse-coupling gain, vanishes at a=0, and retains every original source slot.

### Corollary 4.2. Complete source derivatives on a regular exterior — P

There are fixed δ,C>0 such that for max_i|z_i|<δτ and actual exterior values in a fixed smaller regular domain,

\[
 |\Phi_\tau(z;a)|\le C\mathcal A\max_i|z_i|,
 \qquad
 \|D_z^m\Phi_\tau(0;a)\|
       \le m!C^{m+1}\tau^{1-m}\mathcal A\quad(m\ge1).
 \tag{S1.15; P}
\]

The determinant contribution separately has derivative bound m!C^{m+1}τ⁻ᵐ A, and the E contribution has m!C^{m+1}τ⁻ᵐ⁻¹ A. Mixed exterior-field derivatives follow by (S1.14) and the corresponding fixed-domain Cauchy estimates for W and D.

**Proof.** W and D vanish at a=0 and are bounded by C A on the common w domain. Their w derivatives have the same bound with fixed Cauchy factorials. Use the exact difference (S1.6), integrating its first w derivative along the line segment, and then use D_z=−τ⁻¹D_w for all positive orders. The value estimate uses τ≥1. The E estimate is (S1.14). ∎

**Complex-domain qualification.** On a complex exterior the quantity A=Σ|a_{ij}|, not |W(1,a)|, is the coefficient majorant. Distinct a_{ij} can cancel in their unweighted sum while an independently weighted derivative remains nonzero. On the real SU(2) slice all a_{ij}≥0, and the comparison with W used in §5 is valid. No such positivity is asserted on the complex slice.

## 5. Exact field-valued two-source contacts and source freezing

For real SU(2) staples in the regular domain, put r₀=|Σ_iv_i|, W₀=6−r₀, n=(Σ_iv_i)/r₀, c_i=n·v_i and u_i=v_i−c_i n. These are exterior quantities; r₀≥3 after the fixed choice in §3. Define ω_i=1−c_i. Then

\[
 \omega_i\ge0,\qquad \sum_i\omega_i=W_0,\qquad
 \sum_i u_i=0,\qquad
 \sum_i|u_i|^2\le2W_0,\qquad
 \sum_{i<j}a_{ij}=\frac{6+r_0}{2}W_0\le6W_0.
 \tag{S1.16; P}
\]

The first identities follow by summing c_i=n·v_i. The perpendicular norm is 1−c_i²=(1−c_i)(1+c_i)≤2ω_i. The last equality follows from r₀²=36−2Σ_{i<j}a_{ij}.

For a six-component source direction f let F=max_i|f_i|, f̄=Σ_if_i/6 and osc(f)=max_i|f_i−f̄|. Define the first and mixed second logarithmic source coefficients

\[
 K_f=D_z\Phi_\tau(0;a)[f],\qquad
 K_{fg}=D_z^2\Phi_\tau(0;a)[f,g].
 \tag{S1.17; P: definitions}
\]

### Theorem 5.1. Constant-mode cancellation and spatial two-jet bounds — P

With G=max_i|g_i|, the actual first coefficient satisfies

\[
 K_f=\sum_i f_i\omega_i
       -\frac{3}{2\tau r_0}\sum_i(f_i-\bar f)\omega_i
       +\mathcal E_f,
 \qquad |\mathcal E_f|\le C W_0 F\tau^{-2}.
 \tag{S1.18; P}
\]

Consequently

\[
 |K_f-\bar f W_0|
 \le C W_0\{\operatorname{osc}(f)
       +\tau^{-1}\operatorname{osc}(f)+\tau^{-2}F\}.
 \tag{S1.19; P}
\]

The leading second coefficient is an explicit field-valued contact:

\[
 K_{fg}
 =\frac1{\tau r_0}
       \left(\sum_i(f_i-\bar f)u_i\right)\!\cdot\!
       \left(\sum_j(g_j-\bar g)u_j\right)
       -\tau^{-2}D_w^2D(\mathbf1,a)[f,g]
       +\mathcal E_{fg},
 \qquad |\mathcal E_{fg}|\le C W_0FG\tau^{-3}.
 \tag{S1.20; P}
\]

In particular,

\[
 |K_{fg}|
 \le C W_0\left\{
 \frac{\operatorname{osc}(f)\operatorname{osc}(g)}\tau
 +\frac{F\operatorname{osc}(g)+G\operatorname{osc}(f)}{\tau^2}
 +\frac{FG}{\tau^3}\right\}.
 \tag{S1.21; P}
\]

For real f=g the displayed leading term in (S1.20) is nonnegative. It vanishes if either source is constant on the star. The determinant term vanishes if both are constant. These cancellations are exact, not estimates inferred from smallness of the unmarked activity.

**Proof.** Differentiate W=s−r in the independent w variables at w=1. The first derivative in direction f is Σ_i f_i(1−c_i). The derivative of D=(3/2)log(r/s) is (3/2)[(Σ_if_ic_i)/r₀−(Σ_if_i)/6]. Since Σ_i(f_i−f̄)=0 and Σ_ic_i=r₀, this equals −(3/(2r₀))Σ_i(f_i−f̄)ω_i. Formula (S1.6) supplies the factor τ⁻¹ for this determinant derivative; the remainder derivative is bounded by (S1.14), another τ⁻¹ from z=τ(1−w). This proves (S1.18). Positivity of the ω_i and their sum prove (S1.19).

The bilinear second derivative of r is

\[
 D_w^2r(\mathbf1,a)[f,g]
 =\frac1{r_0}\sum_{i,j}f_i g_j
               (v_i\cdot v_j-c_ic_j)
 =\frac1{r_0}
      \left(\sum_i f_i u_i\right)\!\cdot\!
      \left(\sum_j g_j u_j\right).
 \tag{S1.22; P}
\]

Because W=s−r, the classical contribution to D_z²Φ is −τ⁻¹D_w²W=τ⁻¹D_w²r. The identity Σ_iu_i=0 permits replacing f_i by f_i−f̄ and g_i by g_i−ḡ. By Cauchy–Schwarz and (S1.16), each transverse sum has norm at most √(12W₀) osc(f), respectively √(12W₀) osc(g). This bounds the first term of (S1.20).

For the determinant, D(cw,a)=D(w,a) for c near one. Differentiating this homogeneity identity gives

\[
 D_wD(\mathbf1,a)[\mathbf1]=0,\qquad
 D_w^2D(\mathbf1,a)[\mathbf1,h]
       =-D_wD(\mathbf1,a)[h],\qquad
 D_w^2D(\mathbf1,a)[\mathbf1,\mathbf1]=0.
 \tag{S1.23; P}
\]

Split f=f̄1+(f−f̄1), and similarly g. The fixed-domain bounds for D and its derivatives are C A. Equations (S1.23) remove the constant/constant part and bound the other three terms by C A[F osc(g)+G osc(f)+osc(f)osc(g)]. The last summand is absorbed into the first two using osc(f)≤2F. On the real slice A≤6W₀. Finally, (S1.14) bounds −τ⁻²D_w²E by CW₀FGτ⁻³. This proves (S1.20)–(S1.21). ∎

On the complex exterior domain the same derivation and bounds hold with C A in place of CW₀, with the bilinear algebraic continuation of the leading term, and without a positivity assertion. The cancellation in the constant direction follows from homogeneity and survives complex continuation.

### Corollary 5.2. The literal slowly varying scalar source — P

Let f_i=f(x_{p_i}) and g_i=g(x_{p_i}) use the six literal P2 plaquette anchors. All these points lie at distance at most Ca from the chosen link. Thus osc(f)≤Ca‖∇f‖∞ and osc(g)≤Ca‖∇g‖∞. The actual second coefficient obeys

\[
 |K_{fg}|\le C W_0\left\{
 \frac{a^2}\tau\|\nabla f\|_\infty\|\nabla g\|_\infty
 +\frac a{\tau^2}
       (\|f\|_\infty\|\nabla g\|_\infty
        +\|g\|_\infty\|\nabla f\|_\infty)
 +\frac1{\tau^3}\|f\|_\infty\|g\|_\infty\right\}.
 \tag{S1.24; P}
\]

Physical P2 derivatives multiply f_i and g_i by two, which changes only the explicit fixed constant. The estimate uses C¹ regularity, hence is compatible with the stated C⁵ class. It retains the actual lower-vertex placements rather than silently symmetrizing them.

The first two terms are derivative-source artifacts at this transition. The final constant-source term is an actual field-dependent contact of order τ⁻³. It is not a source-only vacuum constant and must remain in the subsequent source recursion or be extracted into its field-valued contact prescription. No such extraction is assumed merely from the estimate.

### 5.3 A nonzero constant-source field contact is already generated

The leading term of (S1.13) gives, at fixed actual exterior and w=1,

\[
 \Gamma_\tau(\mathbf1,a)
 =\tau W_0+\frac32\log(r_0/6)
      +\frac{W_0}{16\tau r_0}+O(W_0\tau^{-2}).
 \tag{S1.25; P on the real regular slice, with analytic remainder}
\]

For a common source z_i=z, (S1.6) becomes Γ_τ−Γ_{τ−z}. The analytic τ remainder estimates from §3 justify differentiating (S1.25), and hence

\[
 K_{\mathbf1}=W_0-\frac{W_0}{16r_0\tau^2}
                      +O(W_0\tau^{-3}),\qquad
 K_{\mathbf1,\mathbf1}=-\frac{W_0}{8r_0\tau^3}
                      +O(W_0\tau^{-4}).
 \tag{S1.26; P}
\]

For a nonflat regular exterior W₀>0, the second coefficient is nonzero for sufficiently large τ. The flat-star vacuum has already been subtracted. Thus this is a concrete nonzero field-dependent two-source coefficient in the actual Wilson integration. It cannot be removed by declaring the source dependence to consist only of a source-only vacuum and an unchanged linear source. A scheme may place it in a nonlinear scalar coupling shift or retain it as a local contact activity, but must keep and bound it. Its τ⁻³ size is favorable; its existence is not a failure of renormalizability or a counterexample to N1-S.

## 6. A whole first layer, its exact exterior law and the physical root count

Let I be any family of free links such that no plaquette contains two of them. Their incident plaquette sets are disjoint. Given the complement, the original Wilson law therefore factorizes over I, and the preceding calculation applies simultaneously with independent star source arrays z_b.

Let P_ext be the plaquettes incident to no link in I. The exact source-free exterior measure is

\[
 d\mu_{\tau,\mathrm{ext}}
 =\frac1{Z_\tau[0]}
   \exp\!\left(-\tau\sum_{p\in P_{\mathrm{ext}}}a_p\right)
   \prod_{b\in I}\left[e^{-6\tau}I(\tau r_b)\right]
   \prod_{e\notin I}dU_e.
 \tag{S1.27; P}
\]

Its normalization follows by the exact original link integrations, not by assigning unit mass to a rare component. For an arbitrary scalar source on all plaquettes, the exact identity is

\[
 \frac{Z_\tau[z]}{Z_\tau[0]}
 =\exp\!\left(\sum_{b\in I}L_\tau(z_b)\right)
   \mathbb E_{\mu_{\tau,\mathrm{ext}}}
    \exp\!\left\{\sum_{p\in P_{\mathrm{ext}}}z_pa_p
                    +\sum_{b\in I}\Phi_\tau(z_b;a_b)\right\}.
 \tag{S1.28; P}
\]

This first integrates the actual source and extracts its deterministic local vacuum. The unintegrated exterior source is still present. No claim of a physical-volume bound for the entire right side is made from the one-layer formula alone.

The source-free effective action in (S1.27) contains Γ_τ(1,a_b), up to the deterministic flat-star constants. Consequently the next integral must contain its classical W term, determinant log(r/6) term and E remainder. It is not another unchanged Wilson conditional law. The joint-source coefficients (S1.18)–(S1.24) belong inside that next integral.

### Proposition 6.1. Regular background root count after the first vacuum extraction — P

Let a be the fine spacing and h≥a a fixed determining scale. Suppose the actual exterior admits a common completion U_* on I for which every star plaquette satisfies, in a common local gauge,

\[
 \|P_i(U_*)-I\|\le\varepsilon(a/h)^2.
 \tag{S1.29; P: explicit regular-completion hypothesis}
\]

The completion is used only to estimate the exterior loop invariants, not to replace the integrated source. On the real slice W_b is the minimum of the star action over its free link, so W_b≤Σ_{p∋b}a_p(U_*). On the complex slice the trace argument of §3 gives the analogous absolute-loop bound. Thus on a core D, with its fixed star collar,

\[
 \mathcal A_b\le C\varepsilon^2(a/h)^4,\qquad
 \sum_{b\in I\cap D}\mathcal A_b
           \le C\varepsilon^2\operatorname{Vol}(D^+)h^{-4}.
 \tag{S1.30; P}
\]

Here D⁺ is enlarged by a fixed number of fine spacings. The constants are independent of a,h and the torus. The same conclusion holds with W_b on the real slice.

**Proof.** For SU(2), a_p=‖P_p−I‖²_HS/4, and (S1.29) gives the real bound. More generally, the relative star loops are conjugate to products P_iP_j⁻¹, with matrix deviation O(ε(a/h)²); the SL(2,C) trace identity of §3 gives the complex a_{ij} bound. There are a fixed number of loops in each star and at most C Vol(D⁺)a⁻⁴ positive links. Multiplication cancels the fine factor a⁻⁴ against (a/h)⁴, proving (S1.30). ∎

Together with (S1.15), this yields an actual analytic first-layer source remainder bounded by Cε² Vol(D⁺)h⁻⁴ max|z|, after its explicit flat vacuum extraction. Combining it with (S1.24) gives the same determining-block count for the second source coefficient, multiplied by

\[
 C\left\{
 \frac{a^2}\tau\|\nabla f\|_\infty\|\nabla g\|_\infty
 +\frac a{\tau^2}(\|f\|_\infty\|\nabla g\|_\infty
                 +\|g\|_\infty\|\nabla f\|_\infty)
 +\frac{\|f\|_\infty\|g\|_\infty}{\tau^3}\right\}.
 \tag{S1.31; P: factor multiplying the bound in S1.30}
\]

The count is Vol(D⁺)h⁻⁴, not a falsely replaced Gaussian rank. Its proof uses the actual curvature scaling of the retained regular background and the exact already-integrated source. If a later history has several determining scales, each record must keep its own h and its own regular-completion proof. No uniform mixed-layer ownership theorem is inferred from (S1.30).

The one-star vacuum L_τ is local in its six source values and covariant under permutations of the star. Reflection or translation sends the entire formula for I to the corresponding formula for the transformed free-link set. A fixed chosen decimation set need not itself have every reflection symmetry. A compatible full prescription or an explicit symmetrization of the construction remains necessary before asserting the final reflected field algebra or a cell-grid counterterm theorem.

## 7. The first spatial-source transition on every real exterior

The larger regular-domain source radius proportional to τ cannot be extended to every real exterior. A smaller fixed physical-source radius is enough for the following uniform, actual first-layer theorem.

### Theorem 7.1. Full one-star spatial-source envelope and energy reserve — P

There exist fixed δ_*,C,τ₀>0 such that for every τ≥τ₀ and every real SU(2) exterior, the logarithm Φ_τ has a holomorphic branch on Σ_i|z_i|<δ_* and

\[
 |\Phi_\tau(z;v)|\le C W_0\sum_i|z_i|,
 \qquad
 \|D_z^m\Phi_\tau(0;v)\|
       \le m!C^{m+1}W_0\quad(m\ge1).
 \tag{S1.32; P}
\]

Here W₀=6−|Σ_iv_i|∈[0,6], and the direction norms are the maximum norms on the six source values. In addition the source-free exterior interaction obeys, for τ≥1,

\[
 \frac\tau4 W_0\le
 \Gamma_\tau(\mathbf1,v)
       =\log I(6\tau)-\log I(\tau r_0)
 \le\tau W_0.
 \tag{S1.33; P}
\]

Consequently the actual star factor, with its flat vacuum removed, satisfies

\[
 \left|e^{-\Gamma_\tau(\mathbf1,v)+\Phi_\tau(z;v)}\right|
 \le \exp\!\left[-\left(\frac\tau4-C\sum_i|z_i|\right)W_0\right].
 \tag{S1.34; P}
\]

The constants do not depend on the torus, exterior, spacing or τ. A plaquette-disjoint family obeys the product of these pointwise bounds, under any nonnegative additional weight depending only on the retained exterior.

**Proof of the source bound.** Every real plaquette action a_i lies in [0,2]. For the actual conditional law and for its flat reference,

\[
 \left|\mathbb E e^{\sum_i z_i a_i}-1\right|
 \le e^{2\sum_i|z_i|}-1.
 \tag{S1.35; P}
\]

Choose δ_* so small that the right side is at most 1/2. Both logarithms therefore exist on the same fixed source ball, and their difference is bounded by CΣ_i|z_i|, uniformly in every real exterior and τ.

For the exteriors with Σ_{i<j}a_{ij}<ε_a/4, reduce δ_* once so that |z_i|/τ remains in the smaller regular w domain. Corollary 4.2 gives |Φ|≤C(Σa_{ij})Σ|z_i|≤CW₀Σ|z_i|. For the remaining exteriors, Σa_{ij}≥ε_a/4, while Σa_{ij}=W₀(6+r₀)/2≤6W₀. Hence W₀≥ε_a/24, and the crude logarithm bound has the required form after enlarging the fixed C. The branches agree near zero and hence throughout their common connected source ball. Multivariate Cauchy with radii proportional to δ_*/m, followed by m^m≤e^m m!, gives the derivative bound.

**Proof of the energy bound.** Write M(κ)=E_κ[κ(1−u)] for the actual axial quaternion law proportional to e^{κu}. The density of X=κ(1−u) relative to Gamma(3/2,1) is proportional to √(2−X/κ)1_{[0,2κ]}(X), a decreasing function. The elementary covariance identity for an increasing and a decreasing function shows M(κ)≤3/2. Therefore I'(κ)/I(κ)=1−M(κ)/κ≥1−3/(2κ). Also 0≤I'/I≤1 for κ≥0, by the symmetric real Haar integral and |u|≤1.

For r₀≥3, integrate these bounds from τr₀ to 6τ to obtain Γ≥τW₀−(3/2)log(6/r₀)≥(τ−1/2)W₀≥τW₀/2. If r₀≤3, monotonicity gives Γ≥log I(6τ)−log I(3τ)≥3τ−(3/2)log2≥(3/2)τ for τ≥1. Since W₀≤6, this is at least τW₀/4. The upper bound follows by integrating I'/I≤1. This also covers r₀=0 by continuity. Equation (S1.34) follows from (S1.32), and the product assertion follows from conditional factorization. ∎

This theorem is a complete first-layer scalar spatial-source estimate on all real exteriors. On a regular exterior it improves to the analytic field estimates and inverse-coupling contact powers of §§4–5. On a genuinely nonregular exterior, (S1.34) retains a positive part of the actual inherited action as a reserve. It does not replace a sum over many fine anchors by a physical-volume constant; the remaining integration and local vacuum extraction are still necessary.

### Proposition 7.2. A proportional source radius fails on an actual frustrated exterior — P

There are real exterior staples for which the logarithm of the one-star generating function with independent plaquette sources has a zero at a source of bounded size, uniformly as τ tends to infinity. Hence no domain max_i|z_i|<δτ with fixed δ>0 can hold for all real exteriors.

**Proof.** Choose six staple quaternions v_i equal to ±e₀, ±e₁ and ±e₂. Their sum is zero, so the source-zero free-link law is exactly Haar. Such staples can be realized by assigning independently the six parallel exterior links at x±ν, ν≠μ, and setting the transverse links to identity on a sufficiently large compatible torus. Insert a source z on the first plaquette only, with v₁=e₀. Its actual conditional generating function is e^zI(z). Its flat-star-subtracted exponential is

\[
 e^{\Phi_\tau(z,0,\ldots,0)}
       =\frac{I(z)I(6\tau)}{I(6\tau-z)}.
 \tag{S1.36; P near zero source, with meromorphic continuation}
\]

The entire function I(iy) is real for real y. Its alternating series in (S1.2) gives I(0)=1 and I(4i)<−1/45<0: the sum through n=4 is −1/45, and the remaining alternating tail begins negative with decreasing magnitudes. Thus I(iy₀)=0 for some 0<y₀<4. For sufficiently large τ, the denominator I(6τ−iy₀) is nonzero by Lemma 3.1. The zero at z=iy₀ obstructs a single holomorphic logarithm on any proportional disk eventually containing it. ∎

This does not obstruct a fixed small physical-source radius, which Theorem 7.1 proves. It explains why regular complex admission and real large-field treatment must keep their distinct domains. Nor does it contradict a theorem about the generating function without its logarithm: a generating function can be holomorphic at its zeros.

## 8. Exact next kernel, source verification and construction

### 8.1 The first remaining inherited kernel is explicit

Choose a further link c outside the first free family I, and condition on the exterior of c in the measure (S1.27). Let I_c consist of first-layer stars whose exterior loop functions depend on U_c. Let S_{c,ext} be the sum of remaining original plaquettes containing c, and V_{c,ext}[z] their original source. After the already extracted first-layer flat vacua, the exact next unnormalized source kernel is

\[
 \begin{aligned}
 \mathcal K_{c,v}[z]
 =\int_{SU(2)}&
  e^{-\tau S_{c,\mathrm{ext}}(U_c,v)+V_{c,\mathrm{ext}}[z](U_c,v)}\\
 &\times\prod_{b\in I_c}
  \left[e^{-6\tau}I(\tau r_b(U_c,v))
       e^{\Phi_{\tau,b}(z_b;a_b(U_c,v))}\right]dU_c .
 \end{aligned}
 \tag{S1.37; P: actual next conditional kernel}
\]

Source-independent factors not depending on U_c may be placed outside the integral. Every factor displayed here must remain inside. The old source values z_b still refer to their original plaquettes. A current coarse source substituted for them would require a proved freezing or projection error, not a change of notation.

One may reopen the first-layer free links inside this kernel and regard it as a finite joint Wilson patch; that is an exact Fubini identity. It is a useful next calculation. To turn it into a complete R1 induction, the analytic bounds, constant count, vacuum locality, retained constraints and source contacts must remain uniform as the patches, scale histories and determining layers grow. A proof for a fixed patch is not already that uniform theorem.

The corresponding Balaban transition retains still more structure: old R kernels and nonconstant masses, selector branches, constrained Gaussian coordinates, background reconstruction and boundary localizations. The needed O–MR1 decomposition in [Tensor quadratic admission and the marked transition](tensor_quadratic_admission.md), §4.4, concerns those actual outputs. The present note supplies an actual spatial-source seed and its full first-layer estimates; it does not identify unconstrained link decimation with Balaban's constrained block transformation.

### 8.2 What has been closed in this local calculation

| Item | Result established here | Scope retained |
|---|---|---|
| Six independent scalar weights | Exact conditional integral and deterministic flat-star vacuum | Actual SU(2) one-link law; source positions unchanged |
| Regular complex admission | Fixed loop-variable domain, radius proportional to τ in the source, full mixed derivative bounds | Requires the explicit regular loop domain; no new sourced minimizer assertion |
| Spatial first and second jets | Exact leading field contact, constant-mode cancellations and source-gradient gains | Local source arrays on the actual star; higher subsequent interactions retained |
| Field-valued constant-source contact | Nonzero coefficient −W₀/(8r₀τ³)+O(W₀τ⁻⁴) | Cannot be discarded as a vacuum constant; nonlinear scalar/source contact bookkeeping is needed |
| First-layer regular root count | A source remainder count Vol(D⁺)h⁻⁴ after the actual local vacuum is removed | Each record must supply its own regular completion and determining scale |
| Every real exterior | Fixed physical-source disk, all-order derivatives and domination by the actual inherited W energy | Extra weights may depend on the retained exterior only; a new weight depending on the integrated link changes the conditional law |
| Large-field analytic-radius distinction | Actual frustrated exterior has a bounded complex-source zero | Rules out only a radius proportional to τ on every exterior, not a fixed small physical-source radius |

Theorem 7.1 is not the preintegration bound disproved in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md), §3: its original link has really been integrated, and its flat-star vacuum has really been subtracted. Conversely, it does not bound the remaining exterior integral merely because each conditional factor has a useful bound. A complete construction must integrate or expand those remaining interactions, extract both regular and erased-R source vacua, and normalize compulsory histories under the same final measure.

### 8.3 Checked sources and remaining proof status

The finite-lattice results (S1.1)–(S1.37) are direct proofs. The sector estimate is also derived in [Inherited interactions in the second integration](r2_second_integration.md), Theorem 2.1; no external special-function theorem is being assumed. The earlier fixed-background tensor and regular-map results are not needed to derive this scalar SU(2) seed.

The primary statements used for the scope discussion in §1 are:

| Primary source | Location | What it says and does not say |
|---|---|---|
| Balaban, Large Field Renormalization II, CMP122 (1989), 355–392 | (1.65), printed p.375 | The source-free reconstructed field maps into the inductive analyticity domain after the preliminary integrations. This does not prove bounds for a new inherited physical source readout. |
| Same paper | (1.73)–(1.75), printed p.380 | The complex component is compared to the same real positive old mass, which may be very small. The insertion bound requires its actual supremum; the old mass is not a uniform lower constant. |

The first complete theorem in this sequence remains open: **R1: O**. The remaining estimate is an invariant admission and projection theorem for the repeated actual kernels, including the mixed E/R/B history inputs. The first local kernel that must now be admitted in this direct route is explicitly (S1.37). The complete normalized R2 estimate remains a separate requirement. No additional assumption has been appended to N2-F, and none of these local results is relabelled as full N1-S.
