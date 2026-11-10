# Curvature-weighted bounds, flux readout and admission

This is a conditional comparison on admitted homogeneous charts. In applying the final recurrence one also needs the [uniform Gaussian calibration](../native_estimates/gaussian_calibration.md).

## 2. Setting and the interface hypothesis (H-λ′♯)

### 2.1 Objects and identities taken from the preceding chapters (not re-proved here)

(A) Regular whole-lattice identity (the homogeneous comparison, before (17); A8.5): F_{i+1} = Φ_i(F_i) − c_{i+1}A + S_{i+1}, B_{i+1} = Φ_i(B_i) − c_{i+1}A, F_i = E_i + R_i, B_i the fixed-chart comparator, F_0 = B_0 = 0. Exact, finite volume .

(B) λ-family (the homogeneous comparison (21); the homogeneous comparison, Lemma A, §14.4): couplings, counterterms, selectors, maps and large-field inputs frozen; S_i → λ_iS_i, λ ∈ [0,1]^n. F_n^{0} = B_n, F_n^{1} = F_n. Normal form F_n^λ = Σ_{k≤n}Σ_X E^{(k),λ}_irr(X;U_k) + m_n(λ)A(U_n) + R-ledger^λ + const, m_n(1) = 0, R-ledger^λ = Σ_i λ_i[R^{(i)}(Λ_i,U) − R^{(i)}(Λ_i,1)] . Along any path from 0 to 1 in the cube, F_n − B_n = Σ_j∫∂_{λ_j}F_n^λ dλ_j.

(C) Projection and mismatch (the homogeneous comparison (12), (22), (25)–(28)): 𝒫_nG := lim_{f→0}|f|^{-2}lim_{P→∞}[G(W_{f_P}) − G(1)]/V_n, 𝒫A = 1; 𝒫_n(E_n − B_n) = −t_n with t_n := Σ_{i≤n}(p_i − c_i), p_i = 𝒫H_i; so t_n = 𝒫_nR_n − 𝒫_n(F_n − B_n). Define 𝒫̄_n|G| := limsup_{f→0}|f|^{-2}limsup_{P→∞}|G(W_{f_P}) − G(1)|/V_n. These are exact identities (H2c, at every admitted step). Note: t_{n+1} = t_n + p_{n+1} − c_{n+1} is a *definition*, and (12) applies verbatim to the provisional pair (E_{n+1}^{prov}, B_{n+1}) because both use the same frozen c_{n+1}.

(D) Carried-reset bounds (the homogeneous comparison (25)–(27); the homogeneous comparison): on a two-sided linear prefix 𝒫̄_n|R_n| ≤ C Y_n^{2−κ_0/2}ℓ_n^{2r}, and for the single-age ledger derivative 𝒫̄_n|∂_{λ_j}(R-ledger)| ≤ C g_j^{κ_0−2}(1+MR_j)².

(E) Comparator step (under the assumptions (i) |t_i| ≤ 1, (ii) D^G = d_Bn + O(1), (iii) N7.40–43/J–K uniformity ): if |t_i| ≤ 1 and the fixed-chart births H_j, j ≤ i, exist with the E_0 bound, then H_{i+1} exists on the same fixed chart and |p_{i+1} − d_i^G| ≤ C_p/Y_i. Input (ii) is GC.

(F) Pre-subtraction T-output and common-germ replay (CMP119 (3.28), (3.47), pp.265–272, 278–279; §1 step 3): the regular T-operation of step n+1 is performed with the incoming coupling g_n in its Gaussian scaling and cutoff; its unrestricted pre-subtraction bulk birth H*_{n+1} is a localized analytic activity on the provisional chart (2.27)–(2.28) at g_n with the majorant (3.47); the replay at the computed g_{n+1} has the same bulk germ. No estimate from the homogeneous comparison (23)–(24) is used; only the existence of H*_{n+1} and the identification of the germ.

### 2.2 Flux family and carrier charts 

Integral Cartan generator H, exp(2πiH) = 1; W_{f_P} the periodic Landau field with constant 12-plaquette exp(if_PH), f_P = 2πh/P² → f. For a carrier X at scale k with diameter d = d_k(X) counted in its own units u(X) (u = M for E-class, u = MR_k for R-class), the complex affine representative lies in the native space U^c_k(X, α_{0,k}, α_{1,k}) of CMP109 (1.11)–(1.14) for

  |z| ≤ ρ_k(X) := c·min{ α_{0,k}/(LM), α_{1,k}/(u(X)(1+d)) }.   (2.2)

(The real part Ū obeys per-cube conditions in local gauges, so for *real* z the admissible radius is c α_{0,k}/(LM), independent of d; for complex z the imaginary flux must be carried by the global complex part A′, and by Stokes |A′| ≳ |Im z|·diam X, whence the second term. The complex radius therefore depends on d.) At scale k the terminal flux is f_{k,P} = L^{−2(n−k)}f_P and V_k/V_n = L^{4(n−k)}, so (V_k/V_n)|f_{k,P}|² = |f_P|².

### 2.3 The ♯ norm, the carrier-entropy condition, and (H-λ′♯)

For an age-k activity :

  ‖E‖^♯_k := sup_X sup_{(U,J)∈𝒟_k(X)} |E(X;U,J)| e^{κ′d_k(X)} / [r_k²(1+d_k(X))²],

where 𝒟_k(X) is the ♯ domain. The full native space U^c_k(X, α_{0,k}, α_{1,k}) is too large for a uniform ♯ bound (a small ring carrier with a flat connection of nontrivial holonomy satisfies (i)–(iv) but is O(1) away from the orbit of 1); the ♯ domain must be the *hull-regular* one (configurations extending r_k-regularly to a simply connected hull X̂ ⊃ X, diam X̂ ≤ Cd). Sections 3–5 use only: (i) the flux family W_z, |z| ≤ ρ_k(X), lies in 𝒟_k(X) (true for the hull-regular domain, since W_z is the restriction of a global near-flat field), and (ii) the sup bound of the ♯ norm on 𝒟_k(X).

**Carrier entropy.** Let 𝔫_u(d) be the number of connected carriers of diameter d in u-cube units containing a given cube; 𝔫_u(d) ≤ e^{κ_ent d} with κ_ent depending only on the dimension and the metric. Every root sum below uses Σ_{X∋root}(1+d)^4 e^{−κ′d} ≤ Σ_d (1+d)^4 e^{−(κ′−κ_ent)d} =: C_ent(κ′) < ∞, which requires

  κ′ > κ_ent.   (2.3)

At the same time κ′ cannot exceed the rate the source regenerates: CMP116 (2.41) outputs exp(−(1−10δ)·½L·κ d_{k+1}) and Bałaban *assumes* (1−10δ)½L = 1 , i.e. the input rate is regenerated exactly with no spare. Absorbing the (1+d)² weight of the ♯ norm therefore needs a strict surplus η > 0 obtained either from CMP119 p.262's improved T-output rate (1+4β)κ or by re-choosing δ := (1/10)(1 − 2(1+η)/L) (positive for L ≥ 13, η = 1/4; then (1−10δ)·½L = 1+η), with κ, κ_1, M re-fixed accordingly (CMP116 (1.26), (1.32)) *before* q, κ_0 and the ceiling. In particular κ′ := (3/2)κ exceeds the surplus rate (1+η)κ = (5/4)κ at η = 1/4, so the output side would not regenerate it. The consistent choice is κ′ := (1+η/2)κ. **Adopted here, matching the homogeneous comparison: η = 1/2 and κ′ = (5/4)κ** (so the surplus output rate is (1+η)κ = (3/2)κ). With it: the input-side absorption (1+d)²e^{−κ′d} ≤ C_{η,κ}e^{−κd} needs only κ′ > κ; the output side needs κ′ ≤ (1+η)κ (or (1+4β)κ), satisfied with room η/2; and Lemma 3.4's entropy condition (2.3) becomes κ > κ_ent/(1+η/2), met by choosing κ large at (H0) step 3 (κ is free there; M ≥ M(κ) and κ_1 ≥ 16κ+1 follow). So the window κ_ent < κ′ ≤ (1+η)κ is nonempty for every κ > κ_ent/(1+η/2); its realization inside the re-fixed (H0) is an interface prerequisite, not something proved here.

**(H-λ′♯)** . With ε^♯_j := C_R Y_j^{−e♯}ℓ_j^{−2q}, where e♯ = (κ_0−13)/2 if the birth size is taken from R14.3  and e♯ = (κ_0−2)/2 if it is taken from LFR II (1.100) on the native space (the homogeneous comparison (P5), ε^♯_j = Cg_j^{κ_0−2}ℓ_j^{−2q}); a fixed loop exponent b ≥ 0; and κ′ as in (2.3): for every admitted n, all 1 ≤ j ≤ k ≤ n, every λ ∈ [0,1]^n,

 (♯1) ‖∂_{λ_j}E^{(k),λ}_irr‖^♯_k ≤ C ε^♯_j [c̃(k−j) + Y_k^{−1}(Y_j/Y_k)^b], Σ_a c̃(a) < ∞;
 (♯2) |∂_{λ_j}m_n(λ)| ≤ C ℓ_j^{2r} ε^♯_j (Y_j/Y_n)^b;
 (♯3) each piece ∂_{λ_j}E^{(k),λ}_irr(X;·) is gauge-invariant and analytic on 𝒟_k(X), evaluated at the scale-k background of the scale-n flux field (flux f_{k,P}); E-class pieces have u = M;
 (♯4) 𝒫̄_n|∂_{λ_j}(R-ledger)| ≤ C g_j^{κ_0−2}(1+MR_j)² (the homogeneous comparison; this is (D));
 (♯5)  under (A_n) of Section 5.1, the *provisional* output of the regular T-operation of step n+1, computed at trial coupling g_n from the admitted step-n input with the stated c_{n+1} of (C1), on the provisional native space U^c_{n+1}(X, α_0(g_n), α_1(g_n)), satisfies (♯1)–(♯4) for k = n+1 with Y_{n+1} replaced by Y_n and the same constants; the fresh R-output of step n+1 is born after the T-operation and does not enter the provisional output or c_{n+1};
 (♯6) no age window, and no AD/AE bound at an unadmitted step, inside the proof of (♯1)–(♯5).

Constants are uniform in j, k, n, λ, the torus side and the cover under (♯1)–(♯5). This includes the hull-regular choice of domain, the pure-Wilson polymer estimate and the chart hypotheses for the fixed-center comparison.

---

## 3. L4 — flux readout of ♯-bounded responses

### Lemma 3.1 (quadratic Schwarz bound)
If g is analytic on |z| < ρ, g(0) = g′(0) = 0 and sup_{|z|<ρ}|g| ≤ M, then |g(z)| ≤ M|z|²/ρ² for |z| < ρ. *Proof.* g(z)/z² is analytic; maximum principle on |z| ≤ r < ρ; r ↑ ρ. □

### Lemma 3.2 (first flux derivative of a gauge-invariant functional vanishes at the flat field)
Let G be gauge-invariant and differentiable at U ≡ 1. Then (d/dz)G(exp(iza))|_{z=0} = 0 for every Lie-algebra-valued link field a. *Proof.* The derivative is ⟨∇G(1), a⟩; constant gauge transformations fix 1 and act on variations by Ad_h; invariance gives Ad_h∇G(1) = ∇G(1) for all h; su(N) has no nonzero Ad-invariant vector. □ 

### Lemma 3.3 (readout of one ♯-bounded carrier)
Let T be gauge-invariant and analytic on 𝒟_k(X) with ‖T‖^♯_k ≤ β (carrier X, diameter d in u-units), and suppose W_z ∈ 𝒟_k(X) for |z| < ρ_k(X), (2.2). Then for every real flux f at which W_f is an admitted background,

  |T(W_f) − T(1)| ≤ 2βr_k²(1+d)²e^{−κ′d}|f|²/ρ_k(X)² ≤ 2c^{−2}β·max{(LM)², u(X)²(1+d)²}·(1+d)²e^{−κ′d}|f|².   (3.3)

*Proof.* g(z) := T(W_z) − T(1) has g(0) = g′(0) = 0 (Lemma 3.2), is analytic on |z| < ρ_k(X), and sup|g| ≤ 2βr_k²(1+d)²e^{−κ′d}. If |f| < ρ_k(X), Lemma 3.1; if |f| ≥ ρ_k(X), the real-domain bound |g(f)| ≤ 2βr_k²(1+d)²e^{−κ′d} ≤ (same)·(|f|/ρ_k(X))². Finally r_k ≤ min(α_{0,k}, α_{1,k}) gives r_k²/ρ_k(X)² ≤ c^{−2}max{(LM)², u²(1+d)²}. □

The r_k^{−2} of the Cauchy estimate is cancelled by the r_k² in the norm. The readout constant  is κ^♯_E = C_♯M² (fixed) for E-class and κ^♯_R = C_♯(MR_k)² ≤ Cℓ_k^{2r} for R-class, with C_♯ = 2c^{−2}L²C_ent(κ′).

### Lemma 3.4 (root sum, scale cancellation, winding carriers)
Assume (2.3). Under (♯3), for a family {T_X} of age-k pieces of class u with carrier-wise ♯ bound β, and every admitted real f,

  limsup_{P→∞}(1/V_n)Σ_X|T_X(W_{f_{k,P}}) − T_X(1)| ≤ κ^♯_u β |f|².

*Proof.* Nonwinding carriers: by (3.3) the sum over carriers rooted at a scale-k site is ≤ 2c^{−2}β max{(LM)², u²}·|f_{k,P}|²Σ_{X∋root}(1+d)^4e^{−κ′d} ≤ κ^♯_uβ|f_{k,P}|², the last sum being ≤ C_ent(κ′) by (2.3). The number of roots is V_k = L^{4(n−k)}V_n and |f_{k,P}|² = L^{−4(n−k)}|f_P|², so after division by V_n the scale factors cancel exactly. Winding carriers have diameter ≥ cP; by the real-domain bound their total per-site mass is ≤ 2βr_k²Σ_{d≥cP}(1+d)²𝔫_u(d)e^{−κ′d} → 0 as P → ∞, again by (2.3). □

### Proposition 3.5♯ (per-insertion projected response, conditional on (H-λ′♯))
For every admitted n, j ≤ n, and any λ on the chosen path,

  𝒫̄_n|∂_{λ_j}F_n^λ| ≤ Σ_{k=j}^{n} κ^♯_E‖∂_{λ_j}E^{(k),λ}_irr‖^♯_k + |∂_{λ_j}m_n(λ)| + 𝒫̄_n|∂_{λ_j}(R-ledger)|.   (3.5)

Nothing in Section 3 uses the length of the prefix, a band in Y, or a sup-norm iteration of type (17).

---

## 4. L5 — the double sum and the mismatch bound

A *two-sided linear prefix* means, for all 0 ≤ k ≤ n,

  (d_B/2)(n−k) − 2B ≤ Y_k − Y_n ≤ 2d_B(n−k) + 2B,  Y_n ≥ Y_*,   (4.0)

with B from Lemma 1.6.3. Consequences (Y_* ≥ 4B): Y_k ≥ (Y_n + (d_B/2)(n−k))/2; Y_k ≤ Y_j + 2B ≤ 2Y_j and ℓ_k ≤ ℓ_j + 1 for k ≥ j; n − j ≤ (4/d_B)Y_j; Σ_{k=j}^{n}1/Y_k ≤ (4/d_B)log(Y_j/Y_n) + C.

### Lemma 4.1 (elementary sums on a two-sided linear prefix)
For α > 1 and s ≥ 0: Σ_{k=j}^{n}Y_k^{−α} ≤ C_αY_n^{1−α} and Σ_{j=0}^{n}Y_j^{−α}ℓ_j^{s} ≤ C_{α,s}Y_n^{1−α}ℓ_n^{s}. *Proof.* With m = n−k, Y_k ≥ (Y_n + (d_B/2)m)/2; compare with ∫_{Y_n}^∞y^{−α}(log y)^s dy ≤ CY_n^{1−α}(log Y_n)^s for Y_n ≥ Y_*(α,s). □

### Proposition 4.2♯ (per-j bound, conditional on (H-λ′♯))
On a two-sided linear prefix,

  Σ_{k=j}^{n}κ^♯_E‖∂_{λ_j}E^{(k)}_irr‖^♯_k + |∂_{λ_j}m_n| + 𝒫̄_n|∂_{λ_j}(R-ledger)| ≤ C ℓ_j^{2r} ε^♯_j (Y_j/Y_n)^b + C g_j^{κ_0−2}ℓ_j^{2r}.   (4.2)

*Proof.* (♯1) and Lemma 4.1 (α = 1+b): Σ_k ε^♯_j[c̃(k−j) + Y_j^bY_k^{−1−b}] ≤ ε^♯_j[Σ_ac̃(a) + C_{1+b}(Y_j/Y_n)^b]; add (♯2) and (♯4) with (1+MR_j)² ≤ Cℓ_j^{2r}. □

### Theorem 4.3♯ (the comparator mismatch is o(Y_n^{-1}), uniformly in n; conditional on (H-λ′♯))

  |t_n| ≤ C Y_n^{1−e♯}ℓ_n^{2r−2q} + C Y_n^{2−κ_0/2}ℓ_n^{2r} ≤ C_t Y_n^{−3/2},   (4.3)

with C_t independent of n, the depth and the bare coupling. The same bound holds for the provisional mismatch t_{n+1}^{prov} of Section 5 with Y_n in place of Y_{n+1} (by (♯5)).

*Proof.* By (C) and (B), |t_n| ≤ 𝒫̄_n|R_n| + Σ_j∫𝒫̄_n|∂_{λ_j}F_n^λ|dλ_j. Proposition 3.5♯ and (4.2) give Σ_j Cℓ_j^{2r}ε^♯_j(Y_j/Y_n)^b = CY_n^{−b}Σ_jY_j^{b−e♯}ℓ_j^{2r−2q} ≤ CY_n^{1−e♯}ℓ_n^{2r−2q} (Lemma 4.1, α = e♯−b > 1), and Σ_jCg_j^{κ_0−2}ℓ_j^{2r} ≤ CY_n^{2−κ_0/2}ℓ_n^{2r} (Lemma 4.1, α = κ_0/2 − 1 ≥ 8); (D) bounds 𝒫̄_n|R_n| by the same. With e♯ ≥ 5/2 the result is ≤ CY_n^{−3/2}ℓ_n^{C} ≤ C_tY_n^{−3/2} after enlarging Y_*. Every constant came from (H-λ′♯), (D) and (4.0); none depends on n. □

Remarks. (i) the homogeneous comparison's κ_0 ≥ max{12, 2b+21} is stronger than needed here; κ_0 is free (CMP119 p.260; (P-κ_0)). (ii) The age multiplicity n−j+1 that the unsharpened (H-λ′) carries is absent in the ♯ form because (♯1) decays in k−j or in Y_k. (iii) Without (★) (no Lemma F♯), the corrected ρ_k = Cℓ_k^{−(q−p_0)/2} and a sup-norm readout κ ≍ Y_kℓ_k^{−2q} give Γ_k ≍ ℓ^{−2q−(q−p_0)/2+2r} per step, bounded Π only for n−j ≤ cℓ^{2q+(q−p_0)/2−2r}: a polylogarithmic age window, no improvement over . Theorem 4.3♯ stands or falls with Lemma F♯.

---

## 5. L9 — the closing induction, without a window

### 5.1 Induction hypotheses

Fix, in this order : the source constants (L odd ≥ 13, L_0, β_dom, M, M_1, M_2, r ≥ 2, p_0 ≥ 5r, A_0, κ, κ_1, θ, E_0, α′, the localization constants) re-chosen so that CMP116 (2.41) regenerates the decay with a surplus η > 0 and (2.3) has a solution κ′; then q > p_0 (= q_0 = q_1); then κ_0 ≥ max{18, 2b+16} ; then the coupling ceiling γ of LFR II Theorem 1; and a threshold Y_* ≥ max{γ^{-2} + 2B, e^{2p_0}, 4B + 2D, 2C_ρ/d_B + B, the Y_* of Lemma 4.1 and Theorem 4.3♯, the weak threshold of (E)}, D := d_B + 2B + 1, C_ρ := 2(C_p + 3C_t). Let Y_0 ≥ Y_* + D. IH(n):

(A_n) *Admission.* ρ_n satisfies CMP119 §2's inductive assumptions, the couplings (g_k)_{k≤n} satisfy the pairwise inequalities (2.6)–(2.9) for all m < k ≤ n (as transcribed in Lemma 5.1(ii)–(v)), and g_k ≤ γ.
(B_n) *Comparator.* The fixed-chart births H_k, k ≤ n, exist with the common E_0 bound, and |t_k| ≤ C_t/Y_k ≤ 1 for k ≤ n.
(C_n) *Trajectory.* |c_k − d_{k−1}^G| ≤ C_c/Y_{k−1} for 1 ≤ k ≤ n, C_c := C_p + 3C_t; equivalently |y_{k−1} − y_k − d_B| ≤ C_c/Y_{k−1}.

Base n = 0: ρ_0 = exp(−Y_0A − E_0), F_0 = B_0 = 0, t_0 = 0; (A_0) holds for Y_0 ≥ γ^{-2}; (B_0), (C_0) are empty.

### Lemma 5.1 (the ceiling checks follow from (C_n) alone)
Assume (C_n) and Y_n ≥ Y_*. Then for all m < k ≤ n:
 (i) (d_B/2)(k−m) − 2B ≤ Y_m − Y_k ≤ (3d_B/2)(k−m) + 2B (hence (4.0) for every pair);
 (ii) g_m ≤ (1+β_0)g_k and g_k/g_m ≤ (1 + ((3d_B/2)(k−m)+2B)/Y_k)^{1/2} for any prescribed β_0 > 0 once Y_* ≥ 2B/((1+β_0)²−1);
 (iii) (ℓ_m/ℓ_k)^p ≤ (1 + ((3d_B/2)(k−m)+2B)/Y_k)^{p/ℓ_k} ≤ 1+β_0 for each of the finitely many source powers p, Y_* large;
 (iv) with ε(Y) := Y^{−1/2}(log Y)^{p_0}, decreasing for log Y > 2p_0: ε(Y_m) ≤ ε(Y_k−2B) ≤ (1+β_0)ε(Y_k), and the reverse direction with the source's allowed factor (CMP119 (2.8));
 (v) R_m ≥ R_k up to the single rounding of two logarithmic radii (CMP119 (2.9), as in O0 (10.9));
 (vi) g_k ≤ γ, since Y_k ≥ Y_n − 2B ≥ γ^{-2};
 (vii′) *(0.31) on a last-maximizer suffix.* Let S_i := Y_0 − Y_i and let K ≤ n be the last maximizer of S_i − (d_B/4)i over 0 ≤ i ≤ n. Then n − K ≤ 8B/d_B and, for every k ≤ K, (d_B/4)(K−k) ≤ Y_k − Y_K ≤ (3d_B/2 + 2B)(K−k); i.e. CMP109 (0.31) holds exactly for the prefix ending at K with b = d_B/(4 log L), b′ = (3d_B/2+2B)/log L;
 (viii) *step-count and age sums (CMP119 (2.46); R14.3 (RM.9)–(RM.10); the homogeneous comparison).* For every pair j < k: k − j ≤ (4/d_B)(Y_j − Y_k + 2B) ≤ (4/d_B)Y_j, and for every s > 2, Σ_{j≤k} g_j^{s} = Σ_{j≤k}Y_j^{−s/2} ≤ C_s g_k^{s−2}, C_s = 2^{s/2}(1 + 4/(d_B(s−2))); on the (vii′) suffix the same holds with the slack-free constant (1 + 4/(d_B(s−2))). This is sharper than the six-power loss of (2.46) (Σ_{j≤k}g_j^{κ_0−5} ≤ C g_k^{κ_0−11}) and supplies it; C_s is finite for each fixed s and depends on κ_0 only through s, as the parameter order of Section 5.1 requires.

*Proof.* (i): from (C_n), |y_{k−1} − y_k − d_B| ≤ C_c/Y_* ≤ d_B/2, so (d_B/2)(k−m) ≤ y_m − y_k ≤ (3d_B/2)(k−m), and |Y − y| = |b| ≤ B. (ii)–(v): from (i), as in Port_11_7_1_Base §2 and §1 step 2 with the band replaced by the pairwise bound. (vi) immediate. (vii′): maximality gives S_K − (d_B/4)K ≥ S_k − (d_B/4)k, i.e. Y_k − Y_K = S_K − S_k ≥ (d_B/4)(K−k); the upper bound is (i). Comparing the maximizer with i = n: (d_B/4)(n−K) ≥ S_n − S_K = Y_K − Y_n ≥ (d_B/2)(n−K) − 2B, so n − K ≤ 8B/d_B. (viii): the step count is (i) rearranged; for the sum, (i) gives Y_j ≥ (Y_k + (d_B/2)(k−j))/2 once Y_k ≥ 4B, so Σ_{j≤k}Y_j^{−s/2} ≤ 2^{s/2}[Y_k^{−s/2} + (2/d_B)∫_{Y_k}^∞y^{−s/2}dy] = 2^{s/2}Y_k^{1−s/2}[Y_k^{−1} + 4/(d_B(s−2))] ≤ C_sY_k^{1−s/2} for Y_k ≥ 1; on the (vii′) suffix use Y_j ≥ Y_K + (d_B/4)(K−j) without the factor 2. □

**Domain condition.** CMP119 Theorem 1 (p.262) assumes the coupling sequence "satisfies the inequalities (I.0.33)", namely CMP109 (0.31), a two-sided logarithmic bound relative to the terminal coupling with no additive slack; CMP119 p.256 derives (2.6)–(2.9) from it. Two readings are used below. (R1): the inductive step k → k+1 of CMP119's proof uses the coupling hypotheses only through the pairwise inequalities (2.6)–(2.9) among indices ≤ k+1, which (ii)–(v) verify directly; this is the reading implicit in §1 step 2 and Port_11_7_1_Base §2 and must be confirmed on the page . (R2): if the literal (0.31) relative to a terminal index is required, (vii′) supplies it on the prefix ending at the last maximizer K, deleting at most 8B/d_B terminal steps; since the recursion is causal, the prefix through K is the same for every longer provisional run, so every step is eventually admitted (this is B-02's device). Either way the conclusion of Theorem 5.4 is unchanged.

### Lemma 5.2 (comparator step; length-free)
Assume (B_n) with |t_n| ≤ 1 and Y_n ≥ Y_*. Then H_{n+1} exists on the fixed comparator chart with the E_0 bound and |p_{n+1} − d_n^G| ≤ C_p/Y_n. *Proof.* (E), with input (ii) supplied by Lemma 1.6.3. □

### Lemma 5.3 (the next decrement and the next admission; given (A_n))
Assume (A_n). (a) *Existence.* The regular T-operation of step n+1 at coupling g_n is defined on ρ_n (CMP119 §3 uses only the step-n inductive assumptions and g_n in its Gaussian scaling and cutoff); its unrestricted pre-subtraction bulk birth H*_{n+1} is a localized analytic activity on the provisional chart (2.27)–(2.28) at g_n with majorant (3.47), so c_{n+1} := 𝒫H*_{n+1} exists (Lemma 3.3 with the majorant as β). This is convention (C1). (b) *Replay.* If the pairwise inequalities of Lemma 5.1(ii)–(vi) hold for all pairs including n+1 with Y_{n+1} := Y_n − c_{n+1} ≥ Y_* − D (and, under (R2), (0.31) on the selected prefix), then the T and R operations of step n+1 are legitimate (CMP119 Theorem 1 as a map between inductive spaces, p.262 remark 2; LFR II Theorem 1), ρ_{n+1} satisfies (A_{n+1}), and its coupling is exactly Y_{n+1} by the common bulk germ (F). (c) *Mismatch.* The admitted output's E-part and the provisional pre-R output have identical unrestricted whole-lattice regular sums on the intersection of real regular neighborhoods and common compatible covers; the rooted, volume-independent projector therefore gives t_{n+1} = t_{n+1}^{prov}.

*Proof.* (a) is the construction of CMP119 pp.270–278 at the admitted input; nothing about the outgoing coupling is used. (b) is §1 step 3: eligibility of absorbed grids uses old radii, the integrated cutoff uses g_n, the unrestricted homogeneous birth has one germ on the common real neighborhood of flat. (c) the homogeneous comparison, last paragraph of "Testing the next unrestricted coefficient" (the identity part only). □

No estimate from the homogeneous comparison (13)–(16), (17)–(20) or (23)–(24) is used in Lemma 5.3; only existence, identification and exact identities.

### Theorem 5.4 (window-free admission and trajectory; conditional on (H-λ′♯) with (♯5))
Let Y_0 ≥ Y_* + D. Then IH(n) holds for every n with Y_n ≥ Y_*; the recursion is admitted step by step down to the first index K_* with Y_{K_*} < Y_* (and Y_{K_*} ≥ Y_* − D); and for every 0 ≤ i < K_*,

  |c_{i+1} − d_i^G| ≤ C_c/Y_i,  equivalently  |y_i − y_{i+1} − d_B| ≤ C_c/Y_i.   (5.4)

*Proof.* Induction on n; assume IH(n), Y_n ≥ Y_*.
S1 (next decrement). c_{n+1} := 𝒫H*_{n+1}, Lemma 5.3(a).
S2 (comparator). Lemma 5.2: H_{n+1} exists, |p_{n+1} − d_n^G| ≤ C_p/Y_n.
S3 (provisional mismatch). Define t_{n+1}^{prov} := t_n + p_{n+1} − c_{n+1}. By (C) applied to the provisional pair (E_{n+1}^{prov}, B_{n+1}), both built with the stated c_{n+1}, t_{n+1}^{prov} = 𝒫R^{prov}_{n+1} − 𝒫(F^{prov}_{n+1} − B_{n+1}). By (♯5) the pieces of the provisional output satisfy (♯1)–(♯4) with Y_n in place of Y_{n+1}; (C_n) gives (4.0) through n; Theorem 4.3♯ gives |t_{n+1}^{prov}| ≤ C_tY_n^{−3/2} ≤ 1. No a priori bound on c_{n+1} is needed here, because (♯5) is stated at the trial coupling g_n.
S4 (decrement bound). c_{n+1} = p_{n+1} + t_n − t_{n+1}^{prov}, so |c_{n+1} − d_n^G| ≤ (C_p + C_t + C_t)/Y_n ≤ C_c/Y_n and |c_{n+1}| ≤ d_B + 2B + 1 = D (Lemma 1.6.3 for |d_n^G|). Set Y_{n+1} := Y_n − c_{n+1} ≥ Y_* − D: (C_{n+1}).
S5 (ceilings). Lemma 5.1 applied to (C_{n+1}) (its proof needs only (C) and Y ≥ Y_*/2); under (R2) also (vii′) for the selected prefix.
S6 (admission). Lemma 5.3(b): (A_{n+1}).
S7 (closing (B_{n+1})). Lemma 5.3(c): t_{n+1} = t_{n+1}^{prov}, so |t_{n+1}| ≤ C_tY_n^{−3/2} ≤ C_t/Y_{n+1} ≤ 1 (Y_{n+1} ≥ Y_n − D ≥ Y_n/2). With S2 this is (B_{n+1}).
The induction continues while Y_{n+1} ≥ Y_*; (5.4) is (C_{K_*}). □

### Corollary 5.5 (the B-03 recurrence, ultraviolet indexing from the terminal step; conditional as Theorem 5.4)
Convention : K := K_*, the first RG index with Y_K < Y_* (the output of the last admitted step; Y_K ≥ Y_* − D). Under (R2) one may instead take K to be the last maximizer of Lemma 5.1(vii′), which differs by at most 8B/d_B steps; nothing below changes. Define the ultraviolet index m := K − i (m = 0 at the terminal scale, m = K at the bare scale) and

  v_m := u_{K−m} = 1/y_{K−m},  u_* := 1/(2(d_B + C_ρ)),  A := C_ρ + 2(d_B + C_ρu_*)².

(Here u_* is the smallness ceiling of the recurrence; the homogeneous comparison's u_* := 1/(Y_* − C) is the exit threshold. Choosing Y_* ≥ 2(d_B + C_ρ) + D + B makes the exit threshold smaller than the recurrence ceiling, so v_0 ≤ u_* automatically.) If v_0 = 1/y_K ≤ u_*, then for every 0 ≤ m < K,

  v_{m+1} = v_m − d_B v_m² + r_m,  |r_m| ≤ A v_m³,

and v_m is strictly decreasing in m (the coupling vanishes toward the ultraviolet). In B-03's notation, u_{j+1} = u_j − b u_j² + r_j with j = m, b = d_B = 2N²·11 ln L/(24π²) > 0 and |r_j| ≤ A u_j³ for all j < K, where u_j ≤ u_* automatically since u_0 = v_0 ≤ u_* and u is decreasing. The remainder r_m depends on the whole trajectory (through t_i, t_{i+1}, p_{i+1} at i = K−m−1), including finer scales, i.e. *later* UV indices; A is uniform.

*Proof.* From (5.4) with i = K−m−1: y_{K−m−1} = y_{K−m} + d_B + ρ, |ρ| ≤ C_c/Y_{K−m−1} ≤ 2C_c/y_{K−m} = C_ρ v_m (using Y_{K−m−1} ≥ Y_{K−m} − 2B ≥ y_{K−m}/2 for y ≥ 4B). Put ε := (d_B + ρ)v_m; |ε| ≤ (d_B + C_ρv_m)v_m ≤ (d_B + C_ρ)u_* = 1/2. Then v_{m+1} = v_m/(1+ε) = v_m(1 − ε + ε²/(1+ε)), so v_{m+1} − v_m + d_Bv_m² = −ρv_m² + v_mε²/(1+ε), bounded by C_ρv_m³ + 2(d_B + C_ρu_*)²v_m³. Monotonicity: ε > 0 since d_B > C_ρv_m when v_m ≤ u_*. Numerical check in the script. □

**B-04 is pathwise.** Annex S, Theorem 1.1 ((B.4)–(B.7)) is a statement about an arbitrary real sequence (u_j) obeying u_{j+1} = u_j − bu_j² + r_j with |r_j| ≤ Au_j³ and u_0 ≤ u_*; its proof is an induction on j using only this inequality, and nothing in its hypotheses or conclusions refers to how r_j is generated. Hence it applies to (v_m) although r_m depends on finer scales (later indices): v_m = [d_B(m+κ)]^{−1} + O(log(1+m/κ)/(m+κ)²), with κ = 1/(d_Bv_0), and (B.4) reads y_K + (d_B/2)m ≤ y_{K−m} ≤ y_K + 3d_Bm, consistent with Lemma 5.1(i). the estimate (direction) is thereby met: the UV recursion has the minus sign, the IR recursion u_{i+1} = u_i + d_Bu_i² + O(u_i³) the plus sign, and the B-04 asymptotics refer to m. The convention agrees with the homogeneous comparison (u^{UV}_m := u_{K−m}, K the first exit index, B-04 pathwise with u^{UV}_0 = u_K in the invariant interval).

### 5.6 Where the window could quietly re-enter, and why it does not

| Place | Window-dependent object in | What Section 5 uses instead | Status |
|---|---|---|---|
| W1 bounding t_n | sup-norm iteration (17)/(19)/(20), factor (2L⁴)^n, cap (18) | (C) + Proposition 3.5♯ + Theorem 4.3♯ | gone; conditional on (H-λ′♯) |
| W2 ceiling checks | band [Y/2, 2Y], O(K/Y) ratios | Lemma 5.1: pairwise bounds from (C_n); (0.31) via (vii′) if needed | unconditional given (C_n) |
| W3 comparator | (13) and §2 need |t_i| ≤ 1 | (B_n) supplies it; pure-E induction length-free  | unconditional given (B_n) and (E)'s inputs |
| W4 provisional output | (23)–(24): |Δ_{n+1}| ≤ 2L⁴s_k + …, s_k from (14)/(19), Chebyshev with n L^{4n} | S1 defines c_{n+1}; S3 bounds t_{n+1}^{prov} by (♯5) + Sections 3–4; no estimate of (23)–(24) used | conditional on (♯5) |
| W5 multiplicity nL^{4n}, truncation D = C_1(n+log Y) | needed n polylog | not used | gone |
| W6 AD/AE before admission | — | never invoked in Section 5; (♯6) forbids it inside (H-λ′♯); step-locality of E14.3/R14.3  is an interface requirement on the homogeneous comparison's side | explicit |
| W7 CMP109 Theorem 2 | — | not used; (0.31) supplied by (vii′) on the selected prefix | explicit |
| W8 positive single-step drift (A8.21) | — | not used; only |b_i| ≤ B (Lemma 1.6.3) | explicit |
| W9 deterministic flux identity inside T_{j,n} | — | Lemma 3.4 applies the scale cancellation only to the bound (3.3) | explicit |
| W10 age window from Lemma R | Γ_k polylog per step | (★) via Lemma F♯ | conditional  |
| W11 (I.0.33)/(0.31) | — | (R1) pairwise reading, or (R2) last-maximizer suffix | explicit; (R1) to be confirmed on the page |

Circularity check. Quantities of step n+1 are used before its admission only in S1 (existence of the pre-subtraction birth at g_n, CMP119 (3.47)) and S3 (provisional mismatch via (♯5)). Neither uses (2.43) at step n+1, the R-operation of step n+1, R14.3 or E14.3 at step n+1, or g_{n+1} inside an integral; g_{n+1} enters only S5 after S4. There is no need to assume the output estimate here since, by (C2)/(♯5), S_{n+1} is born after the T-operation and is not part of the provisional output or of c_{n+1}.

---
