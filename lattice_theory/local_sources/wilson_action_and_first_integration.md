# Wilson action lower bounds and the first SU(2) integration

## 1. Target, conventions, and status

**Status.** R2 is **O** for the complete Yang–Mills construction. This note proves an actual Wilson-measure obstruction to one proposed preintegration domination argument, then states exactly where a valid complete-history argument must instead be applied. It does not count Ward-score concentration, a conditional scalar innovation estimate, or an abstract normalization implication as a proof of R2.

The lattice is the four-dimensional periodic lattice with n sites in each direction, n≥2. The group is SU(N), N≥2, with normalized product Haar measure. Write V=n⁴ for the number of lattice sites; there are 4V positive-orientation links and 6V plaquettes. The Wilson action and partition function are

\[
s_p(U)=N-\operatorname{Re}\operatorname{Tr}U_p,\qquad
S(U)=\sum_p s_p(U),\qquad
Z(\beta)=\int e^{-\beta S(U)}\,dU,\qquad
d\mu_\beta=Z(\beta)^{-1}e^{-\beta S}\,dU.
\tag{R2.1; P: definitions}
\]

The scalar source in [Lattice conventions and hypotheses](../lattice_conventions.md) is the literal coupling shift. For the constant negative source j=−t, t>0,

\[
\frac{Z_\beta[-t]}{Z_\beta[0]}
=\frac{Z(\beta+t)}{Z(\beta)}
=\mu_\beta(e^{-tS}).
\tag{R2.2; P}
\]

No physical normalization factor is silently attached to this mark. A source for βS is a different mark and must carry that factor in its budget.

At physical spacing a=L^{-K}ℓ₀ and fixed compatible physical torus T, one has n=T/a, N_T=(T/ℓ₀)⁴, and V=N_TL^{4K}. The sole permitted numerical interface N2-F implies the bare bound β_a≤C(K+1), for all sufficiently large K and with a fixed C depending on the selected trajectory. The finite-lattice theorems below do not need N2-F; it is used only when comparing the lower bound with the physical volume.

R2 asks for normalized estimates on the **complete renormalized physical source** after every compulsory old integration, retained survivor mass, selector, constraint and future continuation has been included. There are at least two sufficient strategies:

1. Prove a local fractional comparison for the actual complete positive patch kernel σ_D, with mass t_D=σ_D1, allocated raw reserve ε_D, and the actual outer marginal λ.
2. Prove the actual complex marked-pressure estimate on a fixed source domain, extract the deterministic source-local vacuum on that same domain, and use the literal reflected source factors in the chessboard inequality.

The first strategy has the concrete sufficient target

\[
\int \varepsilon_D^\theta t_D^{\,1-\theta}\,d\lambda
\le e^{C|D|}\int t_D\,d\lambda,\qquad 0<\theta<1.
\tag{R2.3; O: actual complete-patch comparison}
\]

The second strategy is the conditional theorem of §4.27, in [Regular jet transport, pressure and coupling windows](regular_jets.md). Neither a raw component upper bound nor a normalization of the newly appended reference measure proves either strategy.

A **fully unreduced positive lift** retains the original fine field U as well as any later auxiliary variables and all complementary history flags. Its marginal in U is exactly μ_β. By contrast, an **already reduced representation** has actually performed the regular fine-field integrations and retains their effective activities, their extracted vacuum terms, the current fields, and any still-explicit compulsory old fields. These two representations have the same integrated partition function, but their possible pointwise domination bounds are different. Section 3 proves why this distinction is indispensable.

Labels: **P** is proved here, **L** is a checked primary-source assertion in its stated scope, **C** is an application conditional on an explicit unproved input, and **O** is a remaining physical estimate. No interface besides N2-F is assumed. All source-free Balaban formulas used in the table of §5 are checked against the printed pages.

**Related results.** [Pressure and scalar contact terms](../pressure_contacts.md) adds an actual SU(N) plateau variance lower bound, proving the necessity of a divergent quadratic source contact, and a conditional scalar two-jet route using ultraviolet covariance, macroscopic smeared control and prescribed-contact matching without imposing clustering. [Cross-shell Gaussian source transport and local vacuum](cross_shell_gaussian_source.md) proves the full flat Gaussian local-vacuum and active-cell normalization theorem with all cross-shell terms. [Raw core sources in the large-field operation](../raw_core.md) identifies an actual strict-core connected R vacuum. Complete interacting locality, boundary readouts and normalization still prevent full R2.

## 2. An unconditional lower bound on the actual Wilson action

Use the bi-invariant Lie metric −Tr(T_A T_B)=δ_AB, with T_A anti-Hermitian and traceless. Put d_A=N²−1 and C_F=d_A/N. For a link b let X_b^A be the left-invariant derivative, let S_b=Σ_{p∋b}s_p be its six-plaquette star, and define

\[
P_b=\sum_A(X_b^AS)^2,\qquad
\ell_b=\sum_A(X_b^A)^2S.
\tag{R2.4; P: definitions}
\]

**Lemma 2.1 (P): pointwise force and Laplacian identities.** For every configuration and every b,

\[
P_b\le12S_b,\qquad
\ell_b=C_F(6N-S_b).
\tag{R2.5; P}
\]

**Proof.** If b belongs to p, cyclically transport its Lie generator to the base of the plaquette. Inverse occurrences are treated using Re Tr(V⁻¹)=Re Tr(V). The squared gradient norm is therefore the squared norm of the Lie-algebra projection of V−I, where V is a unitary conjugate of U_p or U_p⁻¹. Bessel's inequality in the real Hilbert–Schmidt metric gives

\[
\sum_A(X_b^As_p)^2
\le\|V-I\|_{\mathrm{HS}}^2
=2\bigl(N-\operatorname{Re}\operatorname{Tr}V\bigr)
=2s_p.
\tag{R2.6; P}
\]

There are six incident plaquettes. Cauchy–Schwarz for their six gradient vectors proves the first inequality of (R2.5).

The Casimir matrix Σ_A T_A² commutes with SU(N), hence is scalar. Its trace is −d_A, so it equals −C_FI. Differentiating the real trace of a plaquette twice in its one occurrence of b therefore gives Δ_bs_p=C_F Re Tr U_p. Summing the six contributions proves the second identity. Periodic coincidences of other links when n=2 do not cause the active link to occur twice in a plaquette, so this case is included. ∎

**Theorem 2.2 (P): a volume-uniform action lower bound, also conditionally at each link.** For every β>0 and every exterior configuration,

\[
\mathbb E_{\mu_\beta}[S_b\mid U_{b^c}]
\ge\frac{6d_A}{12\beta+C_F}.
\tag{R2.7; P}
\]

Consequently,

\[
\mathbb E_{\mu_\beta}S
\ge\frac{6d_A}{12\beta+C_F}\,V.
\tag{R2.8; P}
\]

**Proof.** The conditional one-link law is a smooth strictly positive density on the compact group. Haar integration by parts gives

\[
\beta\,\mathbb E[P_b\mid U_{b^c}]
=\mathbb E[\ell_b\mid U_{b^c}]
=C_F\left(6N-\mathbb E[S_b\mid U_{b^c}]\right).
\tag{R2.9; P}
\]

Combine this with P_b≤12S_b. Rearrangement gives
(12β+C_F)E(S_b|U_{b^c})≥6NC_F=6d_A, proving (R2.7). Average over the exterior and sum over the 4V links. Every plaquette belongs to exactly four stars, so Σ_bS_b=4S. This proves (R2.8). ∎

No asymptotic expansion, small-field restriction, plaquette-moment import or coupling-flow derivative has been used. This bound is not claimed sharp. Its order V/β is enough to detect the necessary vacuum subtraction.

**Corollary 2.3 (P): a finite negative scalar source has a divergent unrenormalized pressure response.** For every t>0,

\[
\log\frac{Z(\beta+t)}{Z(\beta)}
\le
-\frac{d_A V}{2}
 \log\!\left(1+\frac{12t}{12\beta+C_F}\right)
\le
-\frac{6d_A t\,V}{12(\beta+t)+C_F}.
\tag{R2.10; P}
\]

**Proof.** At finite lattice size Z is positive and differentiable on the real axis, with ∂_β log Z=−E_βS. Integrate (R2.8) from β to β+t. The second inequality uses log(1+x)≥x/(1+x), x≥0. ∎

For a fixed physical torus on the N2-F bare trajectory, define

\[
D_a(t)=\frac{6d_A t\,V}{12(\beta_a+t)+C_F}.
\quad\text{Then}\quad
\frac{D_a(t)}{N_T}
\ge c_t\frac{L^{4K}}{K+1}\longrightarrow\infty.
\tag{R2.11; P from N2-F's bare growth}
\]

Here c_t>0 depends on the fixed trajectory, t and the construction constants, never on K. Finitely many initial depths can be excluded from this asymptotic lower bound without affecting its conclusion.

### 2.4 The same lower bound for a cell-supported smooth source

The preceding obstruction does not depend on using a source spread over the whole torus. Let 0≤f≤1 be a fixed smooth function supported with margin inside one physical cell, and suppose f=1 on a nonempty smaller cube. Set F_f=Σ_pf(x_p)s_p, where x_p is the literal source anchor in P2. Let B_f(a) be any set of fine links whose six incident plaquette anchors all lie in the plateau f=1.

**Proposition 2.4 (P).** For all β,t>0,

\[
\log\mu_\beta(e^{-tF_f})
\le
-\frac{d_A|B_f(a)|}{8}
 \log\!\left(1+\frac{12t}{12\beta+C_F}\right)
\le
-\frac{3d_A t\,|B_f(a)|}{2[12(\beta+t)+C_F]}.
\tag{R2.12; P}
\]

**Proof.** Along the interpolation with Wilson coefficient β+uf(x_p), 0≤u≤t, every star based at b∈B_f(a) has the common coefficient β+u. Conditioning on its exterior therefore gives exactly the same one-link integration-by-parts argument as Theorem 2.2, even though couplings elsewhere are inhomogeneous. Moreover Σ_{b∈B_f(a)}S_b≤4F_f, because every counted plaquette has f=1 and belongs to at most four stars. Hence
E_uF_f≥(3d_A|B_f(a)|/2)/(12(β+u)+C_F).
Integrate ∂_u log Z(β+uf)=−E_uF_f. ∎

For a fixed plateau of positive physical volume, |B_f(a)|≥c_f a⁻⁴ for all sufficiently fine lattices. Choose t≤r₀/‖f‖_{C⁵,ℓ₀}; then −tf is an allowed cell-supported source. Along N2-F, the positive number on the right of (R2.12), with its minus sign removed, grows at least as c_{f,t}a⁻⁴/(K+1). All geometric restrictions on the source class are respected.

## 3. A complete obstruction to preintegration domination by physical volume and bad records

Let f be either the constant function 1 or the cell-supported function in §2.4, and fix t>0 within the admitted source radius. Write D_a(t,f)>0 for the corresponding lower bound on −log μ_{β_a}(e^{-tF_f}) from (R2.10) or (R2.12). Let C_a(−tf) be any real deterministic source subtraction with the desired bounded renormalized pressure,

\[
\left|
 \log\mu_{\beta_a}(e^{-tF_f})-C_a(-tf)
\right|
\le B\,N_T,
\tag{R2.13; P: hypothesis of the obstruction theorem}
\]

where B is independent of a. The original N1-S cell sum Σ_cL_a(j|_c), if delivered, has this property. A local estimate with the number of active cells in place of N_T is even stronger and is also covered.

**Theorem 3.1 (P): necessary counterterm growth and failure of an unreduced pointwise history budget.** Under (R2.13),

\[
-C_a(-tf)\ge D_a(t,f)-BN_T.
\tag{R2.14; P}
\]

Let μ̂_a be any complete positive history lift with original-field marginal μ_{β_a}. Let H_a≥0 be its bad-record count or another proposed history budget. Suppose the fully small-field branch has the elementary support property

\[
\widehat\mu_a\{H_a=0,\ F_f<\varepsilon\}>0
\quad\text{for every }\varepsilon>0.
\tag{R2.15; P: explicit support hypothesis}
\]

Then the original-field source factor with its deterministic subtraction satisfies

\[
\operatorname*{ess\,sup}_{H_a=0}
 \log\!\left(e^{-tF_f-C_a(-tf)}\right)
=-C_a(-tf)
\ge D_a(t,f)-BN_T.
\tag{R2.16; P}
\]

In particular, along the asymptotically free bare trajectory at fixed physical T, there are no finite a-independent constants C and s such that

\[
\left|e^{-tF_f(U)-C_a(-tf)}\right|
\le e^{CN_T+sH_a}
\quad \widehat\mu_a\text{-almost everywhere for every }a.
\tag{R2.17; P: impossibility of this proposed bound}
\]

**Proof.** Rearrange (R2.13) and use log μ(e^{-tF_f})≤−D_a(t,f) to obtain (R2.14). Since F_f≥0, the logarithm in (R2.16) is everywhere at most −C_a. On each positive-measure set in (R2.15), it is at least −C_a−tε. Let ε decrease to zero to prove the essential-supremum identity.

If (R2.17) held, the essential supremum on H_a=0 would be at most CN_T. Equations (R2.11) and (R2.12) make D_a(t,f)/N_T diverge as a tends to zero. This contradicts (R2.16). The failure occurs on positive-measure sets for every sufficiently small a, not merely at the single flat configuration. ∎

**Why the support hypothesis applies to the proposed unreduced small-field lift.** At the flat original field U_b=I, the physical source F_f vanishes. Choosing the all-small branch gives no bad records. The source-free small-field selectors use strict positive thresholds; the explicit factors in LFR I (1.3)–(1.5), (1.7)–(1.9), printed p.178, are explicit. Their arguments vanish at the identity configuration with zero fluctuation coordinates. For each fixed finite cutoff there are finitely many such conditions, and the regular charts are continuous near that configuration. A sufficiently small neighborhood therefore stays inside the same all-small branch and has arbitrarily small F_f. Product Haar measure and the finite Wilson density are strictly positive there. Normalized gauge/reference variables may be integrated in their corresponding admitted neighborhoods, or are absent when no reset is executed. This gives (R2.15) for a budget that counts only genuinely bad records.

More abstractly, the proof of Theorem 3.1 only needs the displayed support property. If a proposed lift does not have it, that proposal must identify its additional positive fine-scale budget and show how that budget is paid. Calling it a bad-history count does not establish such a payment.

**Interpretation.** This is not a counterexample to R2, N1-S, or a complex marked-pressure estimate after regular integrations. It disproves a particular proposed argument: retaining all original fine variables, subtracting the full deterministic vacuum, and then asserting a pointwise bound that costs only physical volume plus old bad-record count. The missing small-field vacuum cancellation has an ultraviolet-divergent size even for an allowed single-cell scalar source.

The obstruction also identifies the valid place to seek a raw count estimate. First perform the regular integrations that produce and subtract their own vacuum terms. Keep the resulting regular and boundary source activities as effective functions, with their actual analytic norms. Only the still-explicit compulsory old fields can then be bounded by their own paid coordinate counts. Reopening those already integrated activities as all original fine variables reintroduces the obstruction.

All references to a “complete old source envelope” in an R2 proof must therefore specify the represented stage and its variables. A fully unreduced original-field factor and a partially reduced source activity are not interchangeable pointwise.

## 4. Exact SU(2) integration of the predictable scalar source

The preceding obstruction says that regular vacuum cancellation must occur before a physical-volume domination. This section performs one such integration exactly. It identifies the exterior-dependent source interaction rather than discarding it.

### 4.1 Actual one-link law and its exterior loop energy

Use normalized SU(2) plaquette action a_p=1−½Re Tr U_p and coefficient τ>0. The literal P2 convention is s_p=2a_p and τ=2β_a; a constant physical scalar source j on a star is z=2j in the notation below, so τ−z=2(β_a−j). Fix one free link U. Rewrite the six incident plaquette traces as Re Tr(UV_i), where each V_i∈SU(2) is an oriented three-link staple determined by the exterior. In unit-quaternion coordinates q∈S³ for U, choose v_i for V_i⁻¹. Then a_p=1−q·v_i. Set

\[
r=\left|\sum_{i=1}^{6}v_i\right|\in[0,6],
\qquad W=6-r,\qquad
A_b=\sum_{p\ni b}a_p=6-r u,
\qquad
u=q\cdot\frac{\sum_i v_i}{r}\quad(r>0).
\tag{R2.18; P: definitions}
\]

At r=0, A_b=6 is constant. The normalized conditional law of q is proportional to e^{τru}dq. Write

\[
I(\kappa)=\int_{S^3}e^{\kappa u}\,dq
=\frac2\pi\int_{-1}^{1}e^{\kappa u}(1-u^2)^{1/2}\,du.
\tag{R2.19; P}
\]

The second equality is the normalized first-coordinate marginal of Haar measure on S³. No special-function asymptotic is needed.

The exterior interaction W is gauge invariant and is an explicit bounded local loop energy:

\[
W
=\frac{\sum_{i<j}|v_i-v_j|^2}{6+r}
=\frac{2}{6+r}\sum_{i<j}
 \left[1-\tfrac12\operatorname{Re}\operatorname{Tr}(V_iV_j^{-1})\right].
\tag{R2.20; P}
\]

Indeed, 36−r²=Σ_{i<j}|v_i−v_j|², and the quaternion inner product equals the normalized trace of the corresponding relative product. Each V_iV_j⁻¹ is a closed path of length at most six, after any cancellations. All staples have the same endpoints, so their common gauge transformation preserves r and conjugates the relative loops. W vanishes when the six staples coincide. It is not a deterministic vacuum value.

For a scalar star source zA_b, define the deterministic **flat-star** logarithmic vacuum and the remaining conditional logarithm by

\[
L_\tau(z)=\log\mathbb E_{\tau,6}e^{zA_b},
\qquad
\Phi_\tau(z;r)
=\log\mathbb E_{\tau,r}e^{zA_b}-L_\tau(z).
\tag{R2.21; P: definitions near }z=0
\]

At real z with τ−z>0, these are ordinary real logarithms of strictly positive conditional integrals. Complex logarithms below are the analytic branches equal to zero at z=0. Explicitly,

\[
L_\tau(z)=6z+\log I(6(\tau-z))-\log I(6\tau),
\quad
\Phi_\tau(z;r)
=\log I((\tau-z)r)-\log I(\tau r)
-\log I(6(\tau-z))+\log I(6\tau).
\tag{R2.22; P}
\]

### 4.2 A uniform Gamma estimate and the global real theorem

Let κ=τr and X=κ(1−u); set X=0 at κ=0. The star action is A_b=W+X/τ. For κ>0, substitution x=κ(1−u) in (R2.19) shows that the density of X, relative to a Gamma(3/2,1) density, is proportional to the decreasing function
(2−x/κ)^{1/2}1_{[0,2κ]}(x). If φ is increasing and h decreasing, then
2Cov(φ(G),h(G))=E[(φ(G)−φ(G′))(h(G)−h(G′))]≤0.
Consequently X is stochastically dominated by G∼Gamma(3/2,1). In particular,

\[
M(\kappa):=\mathbb E_\kappa X\le\frac32,\qquad
\mathbb E_\kappa X^2\le\frac{15}{4},\qquad
\mathbb E_\kappa e^{qX}\le(1-q)^{-3/2}\quad(0\le q<1).
\tag{R2.23; P}
\]

**Theorem 4.1 (P): global real predictable-source transport.** For every τ>0, every exterior (including r=0), and every real z with |z|≤τ/2,

\[
\left|\Phi_\tau(z;r)-zW\right|
\le\frac72\,\frac{|z|}{\tau}\,W.
\tag{R2.24; P}
\]

Thus the flat-vacuum subtraction leaves the actual exterior loop interaction zW, with a relative O(τ⁻¹) correction, uniformly over every fixed exterior.

**Proof.** For κ>0, differentiation of M(κ)=κ(1−E_\kappa u) gives

\[
M'(\kappa)
=\frac{M(\kappa)-\operatorname{Var}_\kappa(X)}{\kappa},
\qquad
|M'(\kappa)|\le\frac{21}{4\kappa}.
\tag{R2.25; P}
\]

Here ∂_κE_\kappa u=Var_\kappa(u), which follows by differentiating the compact integral. The Gamma bounds imply the inequality.

For real coefficient α>0,

\[
\mathbb E_{\alpha,r}A_b-\mathbb E_{\alpha,6}A_b
=W+\frac{M(\alpha r)-M(6\alpha)}{\alpha}.
\tag{R2.26; P}
\]

If r≤3, then W≥3 and the last numerator has modulus at most 3/2, so the remainder is at most W/(2α). If 3≤r≤6, integrate (R2.25) from αr to 6α to bound the numerator by (21/4)log(6/r)≤(7/4)W. Thus in every case the remainder in (R2.26) is at most 7W/(4α).

The derivative of Φ_\tau(z;r) in real z is (R2.26) with α=τ−z. Integrate from 0 to z, in either direction. Since α≥τ−|z|≥τ/2, (R2.24) follows. ∎

### 4.3 Uniform complex source neighborhood and every scalar source derivative

The real result also has a direct complex extension, without invoking an asymptotic expansion of I.

**Theorem 4.2 (P): a complete one-link complex source theorem.** There are numerical δ,C,C_* >0, independent of τ, exterior and torus, such that Φ_\tau is holomorphic for |z|<δτ and

\[
|\Phi_\tau(z;r)-zW|
\le C\frac{|z|}{\tau}W,\qquad
|\Phi_\tau'(0;r)-W|\le C\frac{W}{\tau},
\qquad
|\Phi_\tau^{(m)}(0;r)|
\le m!C_*^m W\tau^{-m}\quad(m\ge2).
\tag{R2.27; P}
\]

**Proof.** Put t=z/τ and, for real κ≥0, define G_κ(t)=E_κe^{tX} and ψ_κ(t)=log G_κ(t). Choose a numerical δ₀>0 so small that (1−δ₀)^{-3/2}−1≤1/4. Equation (R2.23) gives

\[
|G_\kappa(t)-1|
\le \mathbb E_\kappa(e^{|t|X}-1)\le\frac14
\quad(|t|\le\delta_0),
\qquad
|\psi_\kappa(t)|\le C|t|.
\tag{R2.28; P}
\]

The second estimate follows from
|G_κ(t)−1|≤|t|E[Xe^{δ₀X}]
and the Gamma exponential moment, followed by the logarithm estimate on the disk |G−1|≤1/4. Thus every required logarithm has a uniform analytic branch.

For κ>0, let

\[
\widetilde M_\kappa(t)
=(1-t)\frac{\mathbb E_\kappa[Xe^{tX}]}{G_\kappa(t)}.
\tag{R2.29; P}
\]

This is holomorphic and uniformly bounded on |t|≤δ₀, by the same exponential moments and denominator bound. Cauchy's estimate on the smaller disk implies
|\widetilde M_κ(t)−M(κ)|≤C|t| for |t|≤δ₀/2.

The exact integral identity
G_κ(t)=e^{tκ}I((1−t)κ)/I(κ) gives

\[
\partial_\kappa\psi_\kappa(t)
=\frac{M(\kappa)-\widetilde M_\kappa(t)}{\kappa},
\qquad
|\partial_r\psi_{\tau r}(t)|
\le C\frac{|t|}{r}\quad(r>0,\ |t|\le\delta_0/2).
\tag{R2.30; P}
\]

The identity can also be obtained by direct differentiation under the finite integral. The expression for \widetilde M is exactly the analytically tilted version of M; no positive-measure interpretation is assigned to its complex values.

Since A_b=W+X/τ,

\[
\Phi_\tau(z;r)
=zW+\psi_{\tau r}(z/\tau)-\psi_{6\tau}(z/\tau).
\tag{R2.31; P}
\]

For r≥3, integrate (R2.30) from r to 6 and use log(6/r)≤W/3. For r≤3, use (R2.28) twice and W≥3. Both cases give the first bound in (R2.27), with one fixed δ<δ₀/2. The formula at r=0 follows from X=0 and continuity. Cauchy's estimate for the analytic remainder Φ−zW on a smaller circle of radius proportional to τ proves the derivative bounds. ∎

These constants are uniform at every exterior. The theorem controls a real physical conditional logarithm and its genuine complex source extension, not an artificially normalized old survivor component.

### 4.4 Exact first decimation and the limit of the theorem

Let I be a set of free links with no plaquette containing two of them. Their star plaquette sets are disjoint, and the original Wilson law factorizes in those links after conditioning on the complement. For constant source z on their incident stars, the flat-vacuum-subtracted conditional generating function is therefore exactly

\[
\exp\!\left\{\sum_{b\in I}\Phi_\tau(z;r_b)\right\},
\quad
\left|\sum_{b\in I}[\Phi_\tau(z;r_b)-zW_b]\right|
\le C\frac{|z|}{\tau}\sum_{b\in I}W_b
\quad(|z|<\delta\tau).
\tag{R2.32; P}
\]

Different star sources can be used independently, with the corresponding sum of |z_b|W_b/τ. Smooth-profile differences within a star remain literal additional source terms; their bounded first-layer treatment is in §4.24 of [Geometry, ultraviolet coefficients and conditional innovations](conditional_innovations.md) and is not suppressed here.

After integrating these free links, the **source-free** marginal of the exterior is

\[
d\mu_{\tau,\mathrm{ext}}
\propto
e^{-\tau\sum_{p:\,p\cap I=\varnothing}a_p}
 \prod_{b\in I}\left[e^{-6\tau}I(\tau r_b)\right]
 \prod_{e\notin I}dU_e.
\tag{R2.33; P}
\]

The new terms log I(τr_b) are non-Wilson effective interactions. Therefore the one-link Gamma proof cannot simply be repeated for the next color or next RG layer. Its conditional link law is now affected by these actual inherited interactions. Keeping their source derivatives, decomposing their vacuum/field parts, and bounding them on the correct subsequent domains is the missing transition to the complete R1/R2 induction.

Equation (R2.32) is nonetheless a genuine first integration theorem for the predictable source: its exterior term has been identified as a local gauge-invariant loop energy, and its complete scalar source derivatives are controlled. It is stronger than merely bounding a centered conditional innovation. It is not a proof of R2 across arbitrary ultraviolet depth.

## 5. The exact stage at which a complete domination may be sought

The source-free construction itself distinguishes three different kinds of integrated terms. In B119, printed p.259, the paragraph preceding (2.24) states that E is the regular action, with both vacuum and coupling renormalizations; R is generated by the R-operations, with vacuum renormalization only; B contains terms localized near large-field regions and is not renormalized. Equation (2.25) on that page explicitly subtracts both the regular vacuum and the Wilson coefficient from E. Printed p.262 explains that the running constant is obtained by subtracting the one-step small-field vacuum expressions from the initial constant. These are **L** statements about the source-free construction. A source-dependent version is additional work.

The final LFR II representation is equally explicit about survivor masses. On printed p.391, (1.103) first factors out the product of T′_k(Y_i)1, and only then applies the normalized operators to the boundary exponential. Its explanation of “normalized” means that an operator applied to a function independent of its integration variables equals that function. It does not mean T′_k(Y_i)1 is a numerical constant. Equation (1.104), and the explanation on printed p.392, leave these masses as multiplicative functions of the current fields restricted to Y_i. Contributions of previous large-field regions are contained in those functions and in the new boundary terms. These are **L** statements in the original source-free hypotheses.

Thus a mathematically meaningful complete source envelope has to specify the following stages.

| Stage | Variables or terms retained | Required source operation | What is not justified by the source-free formula |
|---|---|---|---|
| Before regular integration | Original fine fluctuations and literal primitive source | Perform the actual marked regular integral | A pointwise physical-volume bound after subtracting its divergent vacuum; §3 disproves that shortcut |
| Regular effective action | E activities, their Wilson projection, and their local vacuum | Bound all inherited marked activities on the actual determining-field domains and extract their source-dependent vacuum | Replacing every old field by a newly introduced minimizer |
| Erasable R components | Connected activities produced by summing the erasable domains | Perform the marked connected expansion and its R-vacuum extraction | Paying every fine component by its raw smallness and assuming the remaining global pressure costs only physical volume |
| Compulsory survivors | Actual positive kernels, old payload, masses T′_k(Y_i)1, selectors, constraints and B activities | Carry the old source through the same complete kernels and estimate with the true exterior marginal | Declaring a survivor mass constant, replacing it by a newly normalized auxiliary reference mass, or suppressing B terms |
| Terminal representation | Renormalized E/R/B terms, surviving fields and masses, local vacuum already extracted | Prove the complex upper bound and the common-vacuum real lower bound | An upper bound divided by an unrelated normalization |

The raw geometry tilt of main §4.3 concerns the actual positive operator before an old integration, at a fixed localized component. LFR II (1.79), printed p.383, retains its explicit geometry costs together with the suppression factors; the later combinatorial estimates spend these factors. Such a local tilt is useful. It does not itself prove the extensive estimate needed after all ultraviolet components are summed.

### 5.1 A rigorous warning about summing local reserves

The distinction between local component smallness and a physical-volume pressure bound has a simple exact model.

**Proposition 5.1 (P): fixed local exponential tilts need not have a physical-volume global cost.** Fix L>1 and an integer N_T≥1. Let M_K=N_TL^{4K}, let B_1,…,B_{M_K} be independent Bernoulli variables with parameter p_K=exp(−2[log(K+2)]²), and put H_K=Σ_iB_i. For every fixed s>0, an individual occupied-component mass with the tilt e^s obeys the arbitrarily small bound

\[
p_Ke^s\le \varepsilon_K:=e^{-[\log(K+2)]^2}
\quad\text{for all sufficiently large }K.
\tag{R2.34; P}
\]

Nevertheless,

\[
\frac1{N_T}\log\mathbb E e^{sH_K}
=L^{4K}\log\!\left(1+p_K(e^s-1)\right)
\longrightarrow\infty.
\tag{R2.35; P}
\]

**Proof.** The first assertion is immediate once [log(K+2)]²≥s. Independence gives the exact formula in (R2.35). For sufficiently large K, p_K(e^s−1)≤1, so log(1+x)≥x/2 gives the lower bound
½(e^s−1)exp(4K log L−2[log(K+2)]²), which diverges. ∎

This is a counterexample to the proposed inference, not to a Yang–Mills estimate. It shows precisely why reopening every already erased fine-scale component and applying a raw count tilt may recreate a divergent local vacuum. In this example the correct source-dependent subtraction is the deterministic sum M_K log(1+p_K(e^s−1)); local component suppression alone did not subtract it.

A valid source proof must therefore finish both kinds of vacuum extraction before claiming a physical-volume bound: the regular E extraction and the connected erased-R extraction. Source-free extraction followed by a source tilt of every original record is not the same operation. The source dependence of the new vacuum is part of the theorem to be proved.

### 5.2 What the exact SU(2) seed supplies at that stage

For any completion of the exterior by a free link q, the exact star decomposition gives

\[
0\le W=6-r\le A_b(q).
\tag{R2.36; P}
\]

If a genuine regular determining field supplies such a completion, the remainder Φ−zW in §4 is consequently bounded by its actual star curvature energy. The expression (R2.20) also identifies the finite-loop, gauge-invariant readout whose regular derivatives must be estimated. This is a concrete first inherited source term, rather than an unspecified conditional mean.

The conclusion remains tied to the field and scale supplying the completion. A small-curvature estimate at one determining scale does not bound every historical readout on every domain. In particular, the subsequent law (R2.33) must enter the next conditional integral unchanged. The local loop term zW, its analytic remainder, the newly generated unmarked log I terms, and any older E/R/B terms all belong in that next integral.

## 6. The exact remaining R2 proposition

The following statement fixes the kernel whose normalization remains to be controlled. It is deliberately stricter than “the new reference field is normalized.”

Fix the cutoff a, a compatible torus, a complete history geometry, and a connected patch D of physical cells carrying the selected source. Start with the actual source-free positive construction. Perform those regular integrations and erased-component connected expansions that have already been completed, retaining their vacuum subtraction and effective E/R/B activities. Include every compulsory old integration incident on D and every subsequent constraint, selector, boundary factor and continuation that is needed to interpret the inherited physical source. Denote the remaining positive inner kernel by σ_D(ξ,dζ); ξ is its actual exterior and ζ includes all still-explicit old variables. Denote the actual outside positive measure by λ_D(dξ). Define

\[
t_D(\xi)=\int \sigma_D(\xi,d\zeta),
\qquad
Z_D=\int t_D(\xi)\,\lambda_D(d\xi)>0,
\qquad
d\mathbb P_D(\xi,\zeta)
=Z_D^{-1}\lambda_D(d\xi)\sigma_D(\xi,d\zeta).
\tag{R2.37; P: definitions of the actual complete law}
\]

These objects must be obtained from the physical integrand. A replacement of λ_D by product Haar measure, of t_D by a fresh reference mass, or of an old source readout by a new minimizer produces a different statement.

Let Q_D≥0 be a majorant for the complete physical source packet after the preceding vacuum cancellations and counterterm projections. In particular it must include the inherited old source, the predictable exterior terms such as W in §4, and the applicable E/R/B source activities. Let ε_D(ξ)>0 be the actual once-owned reserve retained by the same proof. It may depend on the admitted exterior geometry; it must not be reused independently for multiple pieces of the same packet.

**Proposition 6.1 (C): exact normalization implication.** Suppose there are fixed s>0 and θ∈(0,1), independent of cutoff, torus and history, such that the actual complete kernel satisfies both

\[
\int e^{sQ_D(\xi,\zeta)}\,
     \sigma_D(\xi,d\zeta)
\le \varepsilon_D(\xi),
\tag{R2.38; O: complete physical packet bound}
\]

and

\[
\int \varepsilon_D(\xi)^\theta
          t_D(\xi)^{1-\theta}\,\lambda_D(d\xi)
\le e^{C|D|}Z_D.
\tag{R2.39; O: complete exterior fractional comparison}
\]

Then

\[
\mathbb E_{\mathbb P_D}e^{\theta sQ_D}
\le e^{C|D|},
\qquad
\mathbb E_{\mathbb P_D}Q_D^m
\le m!(\theta s)^{-m}e^{C|D|}
\quad(m\ge0).
\tag{R2.40; C on (R2.38)–(R2.39)}
\]

**Proof.** For each fixed ξ, Hölder's inequality for the unnormalized positive measure σ_D gives
σ_D(e^{θsQ_D})≤[σ_D(e^{sQ_D})]^θ[σ_D1]^{1−θ}.
Insert (R2.38), integrate using exactly λ_D, and divide exactly once by Z_D. This proves the exponential bound. The inequality x^m≤m!u⁻ᵐe^{ux}, x≥0 and u>0, proves the moment bound. ∎

The proposition is elementary; its two physical hypotheses are not established by this note. Local raw geometry tilts verify only a particular part of (R2.38), before all inherited source activities are included. They do not verify (R2.39). Conditional centering of a new scalar score verifies neither the predictable-source part of (R2.38) nor the exterior comparison.

### 6.1 The alternative that avoids individual inverse survivor masses

It is not necessary to insist on (R2.39) if the entire marked pressure can be controlled before local normalization. The alternative has the following exact target.

For every compatible torus, every cutoff and every real or complex source in one fixed admitted source neighborhood, derive from the unchanged complete construction a representation

\[
Z_{a,T}[j]
=e^{V_{a,T}+C_{a,T}[j]}\,\mathfrak Z_{a,T}[j],
\qquad C_{a,T}[0]=0,
\tag{R2.41; O: actual marked representation with one vacuum recipe}
\]

where V is the common source-free vacuum, C is the deterministic source-dependent vacuum generated by that same recipe, and the entire terminal remainder satisfies

\[
|\mathfrak Z_{a,T}[j]|
\le e^{c_+N_T},
\qquad
\mathfrak Z_{a,T}[0]\ge e^{-c_-N_T},
\tag{R2.42; O: complete complex upper and common-vacuum lower estimates}
\]

with constants independent of a,T,j. The complex upper estimate must retain all survivor masses and all previous source activities; it is not a pointwise estimate on the fully unreduced original fine field.

For an active-cell conclusion, the same C must have the source-local decomposition and reflection covariance required in N1-S, on the same complex neighborhood, and the actual reflected source factors must satisfy the required chessboard inequality. Main §4.27 proves the implication once these inputs are available. The equality of source branches, the source-local subtraction, and the complex-domain bounds are part of those inputs. A bound on real j alone is not a holomorphic source estimate, and a deterministic subtraction fitted separately to each torus is not a cell-local counterterm recipe.

This route deals directly with the two vacuum problems identified above. It performs the regular and erased-R source extractions inside the actual integration instead of charging every unintegrated fine field or every original erased component to a global raw count. It also permits compulsory survivor masses to stay unnormalized until the final ratio. It still requires quantitative bounds on the same old source and boundary activities; avoiding a local inverse mass does not eliminate their source dependence.

### 6.2 The first unproved transition after the new theorem

The first genuinely new conditional integral after §4 has the exact marginal (R2.33). A next-link integral is therefore of the form

\[
\int_{SU(2)}
e^{-\tau\sum_{\text{remaining }p\ni e}a_p(U_e)}
\prod_{b:\,r_b\text{ depends on }U_e}
 I\!\left(\tau r_b(U_e)\right)
\,
\exp\!\left\{
 \sum_b\Phi_\tau(z_b;r_b(U_e))

\right\}\,dU_e,
\tag{R2.43; P: form of the next actual integral}
\]

up to factors independent of U_e. This is the literal next integral after the first decimation of the original Wilson law. Source-free constants e^{-6τ} cancel from this displayed dependence. The new product of I factors and the source functions Φ are correlated functions of the same next variable. After further layers, both the additional source-free effective factors and every inherited source activity must also be retained; they are not asserted to be covered by the displayed first-step product.

The needed theorem is a uniform decomposition of this actual integral, and its constrained Balaban analogue, into a deterministic local source vacuum, the correctly projected marginal source, and a remainder with the prescribed E/R/B norm and geometric reserve. Such a theorem must remain true after every repetition and every compulsory large-field history. It must control the full marked packet once, not a sequence of newly centered scores with their predictable parts discarded.

Neither the Gamma calculation nor the scalar N2-F recurrence supplies that theorem. This is the minimal concrete analytical transition still missing on the sequential-integration route. In the full construction it is precisely the inherited-activity transition described by R1, together with the complete normalization or complex pressure estimate in (R2.39) or (R2.42).

