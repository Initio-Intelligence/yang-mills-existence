# External branches attached to a single holed ancestor

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

**Conditional single-record statement.** The branch expansion uses (M-loc-s), (Res-H), (Id-T), (Collar), (T-box), (T-sep), and PA1–PA5. (Res-H) for data-form records still requires (BV-Lip). Two distinct records can meet through an unpaid common hole; no proof that their connected cluster pays the crossing is given.

## 2. The obstruction, stated precisely, and why Cauchy in s cannot cure it

Fix a T step k → K = k+1 and an ancestor ρ in (FT★) at grid G_j ([Retained sigma-fields and conditional expectations] §4.2): carrier X, holes H, paid set P, w_ρ ≤ We^{−κδ_j(P)}. Following [II] p.8 and [III] p.276, its T-step pieces are obtained by deforming the propagators of the step with parameters s_t on the proper-scale cubes t outside X₀ (X₀ = the 𝐃_k-cover of X; s ≡ 1 on X₀) and expanding

 f(s) := G_ρ(Ψ(z;s)) − G_ρ(0),  P(Y₀) := ∫_{[0,1]^{Y₀}} ∂_s^{Y₀} f(s_{Y₀}, 0) ds,  f(1) = Σ_{Y₀} P(Y₀),  (2.1)

where z is the fluctuation of the step (supported in Λ_{k+1}), Ψ(z;s) is the s-deformed (composite) response of the background at the moving labels of ρ, and G_ρ is ρ as a function of that response ([Local deformation of propagators and the minimizer] §6.1: G_X(A) = 𝐁^{(j)}(X; exp(iξA)U, J′(U,J,A))). Summing the source's first-order terms (3.6)–(3.7) of [I] over the cubes □ and integrating over t gives exactly (2.1) for each s (partition of unity and the fundamental theorem of calculus; deduction). Call this identification **(Id-T)**; its status is in §11.

The source bounds each piece by Cauchy on the polydisc |s_t| ≤ e^{κ₁}: |P(Y₀)| ≤ sup|f|·(e^{κ₁}−1)^{−|Y₀|}. Without the reading (R-T1)(ii), which is not used here, the cubes of Y₀ may sit anywhere on the surface of a hole Q ⊂ X₀ ([Native-tag admission, trajectory weights and the obstruction to propagation] §4.1, source p.276), and two things fail ([Native-tag admission, trajectory weights and the obstruction to propagation] §4.4): the *format* (an arm on the far side of Q makes δ_K(P̂ ∪ Ŷ₀) ≥ D̂(Q), unpaid by e^{−κ₁|Y₀|}) and the *entropy* (Σ_{Y₀ ⊂ surface}(e^{κ₁}−1)^{−|Y₀|} = exp(≈e^{−κ₁}S(Q)), S(Q) ≍ R_b^{d−1}).

**What Cauchy cannot see (additional assumption; made precise in §5).** The fluctuation lives in Λ_{k+1}, at distance ≥ the collar from Q. Every term of f that depends on s_t is carried by a chain of walks that passes through t *and ends on the support of z*. An arm on the far side of Q therefore costs the walk decay over a path from Λ_{k+1} around or across Q. Cauchy in s with the root X₀ frozen at s = 1 only counts differentiated cubes; it cannot see the length of a path that runs inside X₀. The cure is to expose that path: represent the response at each label as a sum over clusters with a *small* root (the label's own tile), where Cauchy is harmless, and expand G around the base point. This is the mechanism Bałaban uses for the tag's own term on LFR II p.379 (quoted in §1): "a connection between their localization domains and the set B₀ ∪ (Γ″_k ∩ X^∼), a connection with a proper exponential decay. This allows us to resum".

## 3. Lemma CR (coarse resummation) deduction, and what it settles

**Lemma CR.** Let the fine parameter tiles be grouped into coarse cubes (nested grids), let f be holomorphic on the fine polydisc {|s_t| < e^{κ₁}}, and let C be a finite set of coarse cubes. Then

 Σ_{Y₀ fine: every coarse cube of C is hit, no tile outside C} ∫_{[0,1]^{Y₀}} ∂^{Y₀}f(s_{Y₀},0) ds = Σ_{A⊂C}(−1)^{|C∖A|} f(1 on the fine tiles of A, 0 elsewhere) = ∫_{[0,1]^C}∂_u^C F(u) du,

with F(u) := f(s_t = u_{c(t)}), and therefore |·| ≤ sup_{|s|<e^{κ₁}}|f| · (e^{κ₁}−1)^{−|C|}.

*Proof.* For each coarse cube c apply the interpolation identity in the fine variables of c: Σ_{∅≠B⊂fine(c)}∫∂^B g(s_B,0) = g(1_c) − g(0_c). Taking the product over c ∈ C (the operators act on disjoint variables) gives the Möbius form; it equals the iterated fundamental theorem of calculus for F in the coarse variables. Cauchy for F at u ∈ [0,1]^C on the polydisc of radius e^{κ₁}−1: on it every fine s_t = u_{c(t)} has modulus < e^{κ₁}. □

**Consequence.** The source's resummation "in localization domains Y₀ ∈ 𝐃_k" ([III] p.276) — reading additional assumption: pieces are grouped by the 𝐃_k-cover of X₀ ∪ Y₀ — produces terms bounded by one factor (e^{κ₁}−1)^{−1} per *coarse* cube of Y∖X₀, exactly the single-scale form of [II] (1.24)/(1.30). The fine multiplicity L^{(d−1)(k−n)} of proper-scale cubes along a carrier in old layers (the parenthesis in [Native-tag admission, trajectory weights and the obstruction to propagation] §4.4 item 2; [Local deformation of propagators and the minimizer] §5 remark after Theorem D′) disappears. Sanity check:. What remains of the arm problem after Lemma CR is the coarse one: S(Q) ≍ 2d(D̂(Q)+2)^{d−1} coarse cubes on the surface of a hole that is big in G_K.

## 4. Lemma MS: clusters of the deformed response with small roots conditional

**Setting.** 𝒯 = the proper tiling 𝒯^{(k)} of [Local deformation of propagators and the minimizer] §2 (touch degree ≤ Δ_*), 𝒯_cur = the tiles containing current sites (the support of z). X₀ ⊂ 𝒯 the tiles of the 𝐃_k-cover of X; S := 𝒯∖X₀; 𝔓₁ := {s ∈ ℂ^S: |s_t| < e^{κ₁}}, extended by s ≡ 1 on X₀. A **block** β is a tile of X₀ on which ρ has moving data, with the vector of its labels; R_β := the tiles meeting β^{+(K_d+1)} (K_d = 3 the depth budget of [Local deformation of propagators and the minimizer] (S-struct)); |R_β| ≤ r₀ := Δ_*+1, R_β is ∗-connected and contains β. 𝒴(β) := finite Y ⊃ R_β each of whose ∗-components of Y∖R_β touches R_β.

**Lemma MS.** Assume [Local deformation of propagators and the minimizer] Theorem M(1)–(2) for the composite response Ψ = Ψ^{(j,k)} at deformation exponent κ_M > κ₁+1 (i.e. (W-ms), (S-struct)). Put ρ_u := e^{κ_M−κ₁}. For s ∈ 𝔓₁ and every block β,

 Ψ_β(z;s) = Σ_{Y∈𝒴(β)} ψ_{β,Y}(z;s),  ψ_{β,Y}(z;s) := ∫_{[0,1]^{Y∖R_β}} ∂_u^{Y∖R_β} Ψ_β(z; (u·s)_Y, 0) du  (u ≡ 1 on R_β),

and each ψ_{β,Y} is holomorphic on {‖z‖ < R_z} × 𝔓₁ and satisfies
 (i) it depends on (z,s) only through the z_i with t(i) ∈ Y and the s_t with t ∈ Y∖X₀;
 (ii) it vanishes whenever s_t = 0 for some t ∈ (Y∖R_β)∖X₀;
 (iii) it vanishes identically unless Y ∩ 𝒯_cur ≠ ∅;
 (iv) sup_{𝔓₁}‖ψ_{β,Y}(z;s)‖_∞ ≤ A_β(‖z‖/R_z)(ρ_u − 1)^{−|Y∖R_β|}, A_β = C₁^Ψε_Ψ, R_z = ε_Ψ/g_k ([Local deformation of propagators and the minimizer] Theorem M(4)).

*Proof.* Fix s ∈ 𝔓₁. The function Φ(z,u) := Ψ_β(z; u·s) is defined for |u_t| < ρ_u, because |u_ts_t| < e^{κ_M} (s_t := 1 on X₀); by Theorem M(1) it is holomorphic and bounded by 4B̂₀‖z‖-type bounds (A_β‖z‖/R_z in the normalization of M(4)), and Φ(0,u) = 0. (Dec) of [Local deformation of propagators and the minimizer] Theorem D for Φ in u with root R_β: on the slice u_t = 0 (t ∉ Y) the deformation u·s vanishes at least where u does, so by Theorem M(2) (subordination for every zero pattern) and β ⊂ core(R_β) the value depends only on z, u (and s) in the component Y_{R_β}. [Local deformation of propagators and the minimizer] Theorem D (a) gives Ψ_β(z;s) = Φ(z,1) = Σ_T Φ_T and the Cauchy bound A(ρ_u−1)^{−|T|}; set Y = R_β ∪ T. (i): u = 0 outside Y. (ii): if s_t = 0 for t ∈ Y∖R_β then (u·s)_t = 0 for all u_t and ∂_{u_t} = 0. (iii): by (i) and Φ_T(0) = 0, a ψ that does not depend on z vanishes. Holomorphy in s: Φ_T is an integral over a compact set of a function holomorphic in (z,s,u), with the bound uniform. □

Hypotheses: conditional on Theorem M(1)–(2), i.e. on (W-ms) and (S-struct) of [Local deformation of propagators and the minimizer] (themselves source input; additional assumption there); Theorem D of [Local deformation of propagators and the minimizer] is deduction. Vector-valued (sup-norm) versions of Theorem D are immediate (Cauchy per variable).

## 5. Theorem A (cluster–Taylor bound for the pieces of a big root)

- (H1) G holomorphic on 𝒟 := Π_β {u_β : ‖u_β‖_∞ < ϱ_β}, |G| ≤ K_G.
- (H2) Ψ_β(s) = Σ_{Y∈𝒴(β)} ψ_{β,Y}(s) with ψ_{β,Y} holomorphic on 𝔓₁ satisfying (i)–(iii) of Lemma MS and sup_{𝔓₁}‖ψ_{β,Y}‖ ≤ η_β e^{−a|Y∖R_β|}.
- Pieces P(Y₀) as in (2.1) with f := G∘Ψ − G(0).

A **collection** 𝒞 is a finite nonempty family, with repetitions, of slots (β_i, Y_i), Y_i ∈ 𝒴(β_i), Y_i ∩ 𝒯_cur ≠ ∅; ‖𝒞‖ := Σ_i |Y_i∖R_{β_i}|. Let 𝔆(Y₀) be the set of collections with ⋃_i((Y_i∖R_{β_i})∖X₀) ⊂ Y₀ ⊂ ⋃_i(Y_i∖X₀).

**Theorem A.** Let ρ₁ := e^{κ₁}−1, b ≥ 0, and
 ā_β := (e·2^{r₀}/ϱ_β) η_β Σ_{Y∈𝒴(β), Y∩𝒯_cur≠∅} 2^{|Y|} e^{−(a−b)|Y∖R_β|}.
If ā_β < 1 for all β, then:
 (A1) G∘Ψ is holomorphic on 𝔓₁ and Σ_{Y₀⊂S′}P(Y₀) = f(1_{S′},0) for every finite S′ ⊂ S;
 (A2) P(Y₀) = Σ_{𝒞∈𝔆(Y₀)} P_𝒞, where P_𝒞 is the contribution of the Taylor–cluster term of 𝒞;
 (A3) Σ_{Y₀} ρ₁^{|Y₀|} Σ_{𝒞∈𝔆(Y₀)} |P_𝒞| e^{b‖𝒞‖} ≤ K_G [Π_β(1−ā_β)^{−1} − 1].

*Proof.* Expand G in homogeneous parts per block: G(u) = Σ_{k∈ℕ^𝔅} P_k(u), P_k of degree k_β in u_β, with |P_k(u)| ≤ K_GΠ_β(‖u_β‖/ϱ_β)^{k_β} (Cauchy in the scalars λ_β of G(λ·u)). Let P̌_k be the symmetric multilinear form of P_k (one slot per factor); the polarization inequality gives |P̌_k(h)| ≤ K_GΠ_β(k_β^{k_β}/k_β!)Π_{slots}(‖h‖/ϱ_β) ≤ K_GΠ_β e^{k_β}Π(‖h‖/ϱ_β). Substituting Ψ_β = Σ_Yψ_{β,Y} and expanding multilinearly writes G(Ψ(s)) − G(0) as a sum over collections 𝒞 of T_𝒞(s) := P̌_k(ψ_{β_1,Y_1}(s),…), absolutely and uniformly convergent on 𝔓₁ because Σ_Y sup‖ψ_{β,Y}‖ ≤ ā_βϱ_β/e < ϱ_β/e. This gives (A1) (holomorphy, termwise derivatives, and the interpolation identity of [Local deformation of propagators and the minimizer] Theorem D's proof). (A2): ∂^{Y₀}T_𝒞 at (s_{Y₀},0) vanishes if some t ∈ (Y_i∖R_{β_i})∖X₀ is outside Y₀ (by (ii), ψ_i = 0 there) or some t ∈ Y₀ lies in no Y_i∖X₀ (by (i), no dependence on s_t). (A3): by Leibniz over the slots, ∂^{Y₀}T_𝒞 = Σ_α P̌_k(…, ∂^{α^{−1}(i)}ψ_i, …) over assignments α of the tiles of Y₀ to slots containing them. At s ∈ [0,1]^{Y₀}×0 the polydisc of radius ρ₁ lies in 𝔓₁, so ‖∂^Aψ_i‖ ≤ η_{β_i}e^{−a|Y_i∖R|}ρ₁^{−|A|}. The number of assignments is Π_{t∈Y₀}n_t ≤ Π_i 2^{|Y_i|}. Hence
 ρ₁^{|Y₀|}|P_𝒞| ≤ K_G Π_β e^{k_β} Π_i (η_{β_i}2^{|Y_i|}e^{−a|Y_i∖R_{β_i}|}/ϱ_{β_i}).
For fixed 𝒞 the number of Y₀ with 𝒞 ∈ 𝔆(Y₀) is ≤ Π_i 2^{|R_{β_i}∖X₀|} ≤ 2^{r₀|𝒞|}. Multiply by e^{b‖𝒞‖} = Π_ie^{b|Y_i∖R|} and sum over k and the slots block by block: Σ_{k_β≥0}(ā_β)^{k_β} = (1−ā_β)^{−1}. Remove the empty collection. □

**Two remarks.** (1) Bałaban's factor ρ₁^{−1} per differentiated cube survives in (A3); the cluster weights e^{−a|Y∖R|} come *in addition*. (2) No hole, no root size and no surface count enters (A3): the sum over arm sets has been replaced by a sum over clusters, each rooted at a block and ending on a current tile (by (iii)). Blocks far from 𝒯_cur have small ā_β (Lemma 5.1 below), which is where the collar enters.

**Lemma 5.1′ (cluster count; [Local deformation of propagators and the minimizer] Lemma 5.1 with root size r₀).** Let D_β := min{|Y∖R_β| : Y ∈ 𝒴(β), Y ∩ 𝒯_cur ≠ ∅} and b₀(r₀) := log(2 max(r₀,Δ_*)Δ_*). If a − b − log 2 ≥ b₀(r₀) + θ, θ ≥ 0, then Σ_{Y∈𝒴(β), Y∩𝒯_cur≠∅}2^{|Y|}e^{−(a−b)|Y∖R_β|} ≤ 2^{r₀}·e·e^{−θD_β}.
*Proof.* As in [Local deformation of propagators and the minimizer] Lemma 5.1: Y∖R_β is a union of ∗-connected clusters, each containing one of the ≤ r₀Δ_* tiles touching R_β; the number of ∗-connected sets of m tiles containing a given tile is ≤ Δ_*^{2(m−1)}; extract e^{−θD_β} and bound the product over the touching tiles by exp(2r₀Δ_*e^{−(a−b−log2−θ)}) ≤ e. □

Hence ā_β ≤ C_A (A_β‖z‖/(ϱ_βR_z)) e^{−θD_β}, C_A := e²4^{r₀}, when η_β = A_β‖z‖/R_z.

## 6. Proposition T1♯ (holed T-step format, arm-summed) conditional

### 6.1 Geometry: what a collection costs in the paid tree

Notation of [Native-tag admission, trajectory weights and the obstruction to propagation] §4.2: K = k+1, grids nested, X₀ the G_K-cover of X (it contains the 𝐃_k-cover that serves as Bałaban's root in §§2, 4–5; nothing below depends on the difference), P̂ the G_K-cubes meeting ∪P (interiors), Ŷ₀ the G_K-cubes containing tiles of Y₀, P′ := P̂ ∪ Ŷ₀. Tiles have side ≤ s_k = s_K/L. A block β is **hole-type** if its G_K-cube c_β ∉ P̂ (then c_β meets a hole Q_β, by (a′) of [Native-tag admission, trajectory weights and the obstruction to propagation]) and **paid-type** otherwise.

**(Collar)** (c\*/source as in [Cons] G2): every hole lies in Z_k, at Euclidean distance ≥ 8R_Ks_K from Ω_{k+1} ⊃ the current sites. Put D_col := min over hole-type blocks of D_β; a ∗-chain of m tiles spans ≤ √d s_k m, so D_col ≥ 8LR_K/√d − r₀ − 2. Put c_× := sup_Q √d(1 + D̂(Q))/D_col, D̂(Q) := diam₂(Q)/s_K. By (T-box) and Lemma Traj (T2) of [Native-tag admission, trajectory weights and the obstruction to propagation] (R_b ≤ 2LR_{b+1}), D̂(Q) ≤ 100R_bL^{b−K}+2 ≤ 200R_K + 2, so c_× ≤ 2·10² for d = 4 (crude;  (1)), uniformly in k, b and the age.

**Lemma G (tree cost).** For every Y₀ and 𝒞 ∈ 𝔆(Y₀):
 δ_K(P′) ≤ δ_K(P̂) + C_ℓ‖𝒞‖ + C_r|Y₀|,  C_ℓ := 3√d/L + c_×,  C_r := 2√d/L.

*Proof.* Start from a tree through the cubes of P̂ of length ≤ s_K(δ_K(P̂)+ε). Every cube of Ŷ₀ contains a tile t ∈ Y₀; by 𝔆(Y₀), t lies in Y_i∖X₀ for some slot i. If t ∈ R_{β_i}∖X₀ is in no Y_{i′}∖R_{β_{i′}}, join t to the tile β_i (one touch-step, ≤ 2√d s_k): this is the C_r|Y₀| term, provided β_i is joined to the tree. Otherwise |Y_i∖R_{β_i}| ≥ 1: run through the centres of the ∗-components of Y_i∖R_{β_i}, each joined to β_i within two touch-steps: length ≤ √d s_k(|Y_i∖R| + 2·#components) ≤ 3√d s_k|Y_i∖R|. Join β_i to the tree: 0 if paid-type (β_i lies in a cube of P̂); if hole-type, from β_i to Q_{β_i} (≤ √d s_K), across it (≤ √dD̂ s_K) to a cube of P̂ touching it ((b′) of [Native-tag admission, trajectory weights and the obstruction to propagation]), and since every slot of a hole-type block has |Y_i∖R| ≥ D_β ≥ D_col, this is ≤ c_×|Y_i∖R| s_K. A slot whose only tiles outside X₀ are root tiles of a hole-type block also has |Y_i∖R| ≥ D_col, so its join is covered the same way. Divide by s_K and let ε ↓ 0. □

### 6.2 Statement

**Inputs.**
- (FT★) for ρ at grid G_j, with (T-box), (T-sep), nested grids ([Retained sigma-fields and conditional expectations] §4.1–4.2).
- **(M-loc-s)** = Lemma MS, i.e. [Local deformation of propagators and the minimizer] Theorem M(1)–(2) at exponent κ_M.
- **(Res-H)** ρ, as a function G_ρ of its moving data at the T step, is holomorphic and bounded by w_ρ on the polydisc of per-block radii ϱ_β, uniformly in the frozen data, with the reserve pattern (Res-pat) of [Local deformation of propagators and the minimizer] §6.1 (status §11).
- **(Id-T)** the source's T-step descendants of ρ, summed over □ and t, are the pieces (2.1) on the proper tiling with root X₀; grouped by coarse cover ([III] p.276) (status §11).
- (Collar), Lemma Traj (T2), (Geo)-type layer count T3 of [Multiscale incidence and logarithmic jets] (a ∗-chain from a tile of scale n to a current tile has ≥ k−n+1 tiles).
- Asymptotic-freedom ratio α_{∧,k}/α_{∧,n} ≤ C_AF√(1+k−n) ([Local deformation of propagators and the minimizer] Prop. R).

**Parameter conditions.**
- (PA1) a := log(ρ_u−1) ≥ κ_M − κ₁ − 1 satisfies a − κC_ℓ − log 2 ≥ b₀(r₀) + θ.
- (PA2) κ₁ ≥ κC_r + log 2 (the analogue of the source's own "¼(κ₁−1) ≥ (1−δ)κ").
- (PA4) radius: ‖z‖ ≤ r_A := ϱ_refR_z/(4√2C_AF C_A A), with ϱ_ref := (β/2)α_{∧,k}, A := max_βA_β, C_A := e²4^{r₀} (crude; r₀ ≤ Δ_*+1). This is [Local deformation of propagators and the minimizer] Prop. R's radius with c_⋆ multiplied by a constant depending on d, L only, so (R) holds under the same constraint on (q₀,q₁,C₀,C₁) (with min(q₀,q₁) > p₀ any constant is harmless).
- (PA5) κ(1 − 1/L) ≥ C_P 2^{d+1} + δ_resκ, with C_P the constant defined in the proof of T1♯ (depends on d, L, m₁ only).

**Proposition T1♯.** Under these inputs and conditions, for every ancestor ρ and every z in the source's fluctuation domain with ‖z‖ ≤ r_A:
 (a♯) [= (a′) of [Native-tag admission, trajectory weights and the obstruction to propagation]] every cube of X₀∪Ŷ₀ outside P′ meets a hole of H; (b♯) [= (b′)] every hole of H touches a cube of P′;
 (c♯) Σ_{Y₀} |P(Y₀)| e^{κδ_K(P′(Y₀))} ≤ W e^{C_P2^d} e^{−δ_resκδ_j(P)};
 (d♯) consequently every descendant of ρ (and, after grouping by coarse cover, every descendant term with domain Y) is an (FT★) record at grid G_K with carrier X₀∪Ŷ₀, holes H, paid set P′, rate **κ** (no loss) and constant W′ = We^{C_P2^d}; the factor e^{−δ_resκδ_j(P)} is left for the sum over ancestors with a given descendant, as in [II] p.9;
 (e♯) every nonzero piece contains a slot whose cluster meets 𝒯_cur, so its domain meets Λ_{k+1} (consistent with (R-T1)(ii′) of [Native-tag admission, trajectory weights and the obstruction to propagation]).

*Proof.* By Lemma G, e^{κδ_K(P′)} ≤ e^{κδ_K(P̂)}e^{κC_ℓ‖𝒞‖}e^{κC_r|Y₀|} for 𝒞 ∈ 𝔆(Y₀), and e^{κC_r|Y₀|} ≤ ρ₁^{|Y₀|} by (PA2). Apply Theorem A with b := κC_ℓ (admissible by (PA1) and Lemma 5.1′):

 Σ_{Y₀}|P(Y₀)|e^{κδ_K(P′)} ≤ e^{κδ_K(P̂)} w_ρ [Π_β(1−ā_β)^{−1} − 1]. (6.1)

By [Local deformation of propagators and the minimizer] Prop. R's arithmetic ((Res-pat), the asymptotic-freedom ratio, exponent 2 there), ϱ_βe^{2D_β} ≥ ϱ_ref/(2√2C_AF) for every block. Hence, with Lemma 5.1′ and (PA4),
 ā_β ≤ C_A(A‖z‖/R_z)ϱ_β^{−1}e^{−θD_β} ≤ ½ e^{−(θ−2)D_β} ≤ ½,
so Π(1−ā_β)^{−1} ≤ exp(2Σ_βā_β). Split the blocks.
- *Hole-type blocks.* D_β ≥ max(D_col, k−n−1) by (Collar) and T3 (n the grade of the block). A hole Q is met by at most (D̂(Q)+2)^d G_K-cubes, each holding ≤ L^{d(K−n)} tiles of grade n, so the blocks of one hole contribute ≤ ½(D̂+2)^dΣ_{n≤k}L^{d(K−n)}e^{−(θ−2)max(D_col,k−n−1)} ≤ ½(D̂+2)^d(D_col+2)L^{2d}e^{−(θ−2−d log L)D_col}(1−L^de^{−(θ−2)})^{−1} ≤ 1 by (PA3). The holes of ρ number ≤ m₁3^d|P̂| (each touches a cube of P̂; [Cons] V3), so Σ_{hole-type}ā_β ≤ m₁3^d|P|_j; for one hole the contribution is O(e^{−(θ−2−θ_*)D_col}), i.e. collar-small when θ − 2 > θ_*.
- *Paid-type blocks.* Per π_j-cube of X: in layers n ≥ j at most one block; in layers n < j at most L^{d(j−n)} blocks, with D_β ≥ (k−n−1)₊: Σ ≤ ½Σ_{m≥0}L^{dm}e^{−(θ−2)(m−1)₊} ≤ C(additional assumption; L) since θ − 2 ≥ d log L + 1. So Σ_{paid-type}ā_β ≤ C(additional assumption; L)|P|_j.

Hence Π(1−ā)^{−1} ≤ exp(2Σā_β) ≤ exp(C_P|P|_j) with C_P := 2C(additional assumption; L) + 2m₁3^d; writing |P|_j ≤ 2^d(2δ_j(P)+1) the additive part is C_P2^d. With w_ρ ≤ We^{−κδ_j(P)}, δ_K(P̂) ≤ L^{j−K}δ_j(P) ≤ δ_j(P)/L ([Native-tag admission, trajectory weights and the obstruction to propagation] (c′), first paragraph) and |P|_j ≤ 2^d(2δ_j(P)+1) ([Hidden components] Lemma A3), (6.1) is ≤ We^{C_P2^d}exp(−[κ(1−1/L) − C_P2^{d+1}]δ_j(P)), and (PA5) gives (c♯). (a♯), (b♯) are [Native-tag admission, trajectory weights and the obstruction to propagation] (a′), (b′), which use only nesting (unchanged: P′ ⊃ P̂ and Ŷ₀ is paid). (d♯) is (c♯) read term by term; grouping by coarse cover only sums nonnegative bounds. (e♯) is (iii) of Lemma MS. □

**What T1♯ changes relative to T1 and T1♭.** No reading (R-T1)(ii). No excess factor exp{(1−δ)κΣD̂(Q_C)}: the crossing of a hole is paid by the cluster that makes it (Lemma G). No arm entropy: (6.1) is a sum over clusters rooted at blocks; the hole contributes through its blocks only, each at collar distance from 𝒯_cur. T1♭ (holes small in G_K) is contained (D̂ < D₀ makes c_× smaller). The counter-configuration of [Native-tag admission, trajectory weights and the obstruction to propagation] §4.2 (one arm on the far face) is a legitimate piece; its weight carries the cluster that reaches it, which crosses or goes around Q.

### 6.3 Corollary S2★-T (descendants of the tag's own term) conditional

Let G_v be the z-dependent part of the tag's own term V(Y_v^∼) ([Native-tag admission, trajectory weights and the obstruction to propagation] §2.1 last item: localized in a component of Z^∼, moving data = the boundary-layer data of width 2M₁ at ∂Y₁, LFR II p.373 per [Native-tag admission, trajectory weights and the obstruction to propagation], assumed input), holomorphic on the polydisc of its boundary-layer blocks with |G_v − G_v(0)| ≤ K_v. All its blocks are hole-type. Then its T-step descendants are (FT★) records with exterior the S2★ cube plus Ŷ₀, hole Y_v^∼, and

 Σ_{Y₀}|P_v(Y₀)|e^{κδ_K(P′)} ≤ K_v · 2Σ_β ā_β ≤ C K_v (D̂+2)^d(D_col+2)L^{2d}e^{−(θ−2−d log L)D_col}.

So they join S1b carrying a collar factor. *Status of K_v:* (d) that K_v ≤ C(C_TLR_b)^d s_{*,b} with s_{*,b} the weight of [Native-tag admission, trajectory weights and the obstruction to propagation] Theorem R‴ (integrate R‴'s derivative bound across the polydisc); needs (Res-H) for data-form records, i.e. (BV-Lip). Any K_v polynomial in R_b is absorbed.

## 7. What the summation theorems require, and that they consume T1♯

### 7.1 The requirements, read from the proofs

- **[Hidden components] Theorem C** (no holes): per record (Loc) with exterior E_ρ (no connectivity), anchor in closure{g ≤ b}, and the rooted norm 𝒜_b(ν/2+1) = sup_q Σ_{q_ρ=q} w_ρe^{(ν/2+1)δ_b(E_ρ)} (Step 4 uses Lemma C2, i.e. a tree through E_ρ).
- **[Summation over roots with hidden holes] Theorem C′**: in addition holes with (Att), (H-sep), (Col); (Loc′) with the full carrier. Holes enter only Lemma C3: the nearest point of X_ρ to a site may be in a hole Q, which is then crossed once at cost √dD_Q ≤ (√d/θ)Δ by (Col); the rest of the path runs along a tree through F_ρ (uncontracted δ_b(F_ρ)).
- **[Summation over roots with hidden holes] Prop. B2′**: per-pair weights w(F,H) ≤ We^{−aδ_b(F)}, a − ϑ ≥ κ′_cnt(d); counting through the tree-neighbourhood of F; holes chosen among those touching F.
- **[Retained sigma-fields and conditional expectations] Lemma H**: (FT★)(a)–additional assumption, (T-box), (T-sep); output for C′ + B2′ with rate κ/C_♯.
- **[Retained sigma-fields and conditional expectations] Cor. C-col**, **[Hidden components] Theorem D**, **[Summation over roots with hidden holes] D3′**: the same rooted norms, with collar/age distances of the anchors.

So the summation theorems need (Loc′) and a finite rooted norm; (FT★) is a sufficient *format* that Lemma H and B2′ convert into that norm.

### 7.2 Consumption

T1♯ (d♯) delivers (FT★) at grid G_K with rate κ and constant W′, and leaves (Col_K), (H-sep) and (Att) unchanged (holes unchanged, P′ ⊃ P̂). Lemma H then applies verbatim, and C′, B2′, C-col and Theorem D follow with W_K replaced by W′. The sum over ancestors producing the same descendant uses the reserve e^{−δ_resκδ_j(P)} exactly as the full-tree case ([II] p.9: fix a cube in X, sum over X ∋ it with (1.26), then over the cubes; here over P instead of X, since unpaid cubes are hole cubes and holes are fixed). deduction given T1♯.

**Why a weaker "hole as a free vertex" format would not do.** If δ_b(F) were replaced by the tree length with holes contracted, (i) Lemma C3 would have to cross holes that are not nearest to the site; (Col) bounds D_{Q′} only by d(x,Q′), which along the path grows by the previous crossings, giving a factor (1+√d/θ)^{#holes crossed}; (ii) B2′'s count would pass through a hole vertex of degree N_att(Q) ≍ R^{d−1} at each visit. Both are harmless only if every hole visit carries a weight ≪ 1/N_att(Q) — which is what the clusters of Theorem A carry, and why T1♯ can prove the uncontracted format. (Bałaban's own contracted format d_{k,∪Y_i} in LFR II (1.99) is consumed by him under "there are no summations over these domains, they are fixed", p.391; that is the R-step situation, where the holes are the new tags themselves.)

## 8. The full-tree case of [Multiscale incidence and logarithmic jets] §7: scope

**Claim of [Multiscale incidence and logarithmic jets] §7:** (FT)/(Mon) at T steps for records without declared holes are (c) via [II] (1.24), (1.30)–(1.32) and the sentence "the remaining considerations and bounds are the same as in [I]" ([III] p.276).

**Re-read against p.276 source input and [II] §1.** Three ingredients.
1. *Per-term weight.* (1.24)/(1.30): the old factor e^{−κd_j(X)} is carried unchanged and each new cube is charged e^{−(κ₁−1)}; (1.31)–(1.32) convert to e^{−(1−δ)κd_k(Y) − δκd_j(X)}. source input, as [Multiscale incidence and logarithmic jets] says.
2. *Multiscale cubes.* The s-cubes are proper-scale cubes (p.276), so a carrier bordering a layer of grade n < k has up to L^{(d−1)(k−n)} of them per face of a coarse cube. Read naively, (1.27)'s bound e becomes exp(c e^{−κ₁}L^{(d−1)(k−n)}), not uniform in the age. **Lemma CR (§3) removes this exactly:** after the printed resummation into 𝐃_k-domains, the term with coarse domain Y is bounded by one factor (e^{κ₁}−1)^{−1} per coarse cube of Y∖X₀. deduction, given the reading (d) that "resum in Y₀ ∈ 𝐃_k" groups by coarse cover.
3. *Coarse arms.* For a carrier with no hole every coarse cube of X₀ is paid; the coarse arms are coarse animals attached to the ≤ 3^d|X₀| coarse cubes touching X₀, so their sum is ≤ Π_{c}(1 + Σ_{animals ∋ c}(e^{κ₁}−1)^{−|animal|}) ≤ exp(C_d|X₀|e^{−(κ₁−1−2d log 3)}), absorbed by e^{−δκd_j(X)} since |X₀| ≤ |X|_j ≤ C d_j(X) — the pattern of [II] (1.26)–(1.29).

**scope: sound.** The analysis specific worry — proper-scale s-cubes in old layers next to a carrier that abuts a large-field component — is (i) the fine-multiplicity issue, settled by Lemma CR, and (ii) arms on the carrier's own surface, which is paid because the carrier has no hole. A large-field component that the record merely touches is not a hole of it; arms entering that region are ordinary arms. [Multiscale incidence and logarithmic jets] §7's source stands, with Lemma CR added as the (a) step that "the same as in [I]" leaves implicit; Theorem A (applied with all blocks paid-type) is an independent proof of the same bound.

**How Bałaban handles domains adjacent to large-field regions (source input; for the record).** Three devices, all consistent with the above: (1) LFR II p.379: for the tag's own term, "expand them up to the first order in A′, J … a connection between their localization domains and the set B₀ ∪ (Γ″_k ∩ X^∼), a connection with a proper exponential decay. This allows us to resum" — the mechanism of Theorem A (decay along the connection to the source set, not a per-cube count); (2) LFR II pp.387–388: connectivity defined on X′₀∖⋃Y_i, holes do not connect components; (3) LFR II (1.99) and p.391: linear size d_{k,∪Y_i} with holes not counted, justified because the holes are fixed. None of these is printed for the T step after birth; T1♯ supplies (1) for it, and (2) is the device needed in §12.

## 10. Costs (deduction; arithmetic; constants crude)

- **Deformation exponents.** (PA1)–(PA2): κ_M ≥ κ₁ + 1 + log 2 + κC_ℓ + b₀(r₀) + θ and κ₁ ≥ κC_r + log 2. With the source's own κ₁ ≥ 4κ+1 ([II] (1.32)), C_ℓ ≈ 2·10² (d = 4) gives κ_M ≈ 52κ₁ ( (3)). [Local deformation of propagators and the minimizer] Theorem W allows κ_M ≤ δ₀M/(2^{d+6}L²), so **M must be ≈ 50 times larger** than what Theorem M at κ_M ≈ κ₁ (already used by A1, Route I) requires for the same κ. Order of constants unchanged: d, L → κ → κ₁ → κ_M → M → C₀, C₁ → ceilings (the representation convention, the collar estimate).
- **Coupling ceiling.** Theorem M's domain ε_ℋ ∝ B̂₀^{−2} ∝ e^{−2·2^dκ_M}; the T-step needs ‖B‖ ≲ ε_ℋ, i.e. g·polylog ≲ e^{−32κ_M} for d = 4 instead of e^{−32κ₁}: the window shrinks by a power ≈ 52 in the exponent. Harmless for existence; relevant to B-05 (already "astronomically small", the representation convention).
- **(R).** Holds with c_⋆ multiplied by a constant depending on d, L only (PA4); still a constraint on the free constants of [III] (2.28) only.
- **κ (format rate).** (PA5) adds C_P2^{d+1} to the lower bound on κ(1−1/L); negligible beside Lemma H's κ ≥ C_♯(κ′_cnt+ν/2+1) ([Retained sigma-fields and conditional expectations] Rem. (ii)). The very large C_ℓκ in (PA1) is inherited from that C_♯; improving Lemma H's constant improves (PA1) proportionally.
- **CMP119 (3.44)–(3.47).** Untouched by T1♯ (the pieces are the source's). See §12 for the one issue at that layer.
- **No cost** to the Cauchy/κ₁ bookkeeping of the source: Theorem A keeps the factor (e^{κ₁}−1)^{−1} per differentiated cube.

## 11. Status of the inputs of T1♯

| Input | Content | Status |
|---|---|---|
| (M-loc-s) | Lemma MS | conditional on [Local deformation of propagators and the minimizer] Theorem M(1)–(2) = (W-ms), (S-struct) ([Local deformation of propagators and the minimizer] source input; additional assumption); the local-test construction's [Dec] reading where the old structure is one M₁-cube thick (inside tags) |
| (Res-H) | holed ancestors holomorphic on per-block polydiscs in the moving data, uniformly in frozen data | printed B′-terms: analyticity on Ũ^c_k(X,α̃₀,α̃₁) (source input; LFR II p.390) + (Res-pat) additional assumption as for (2.42); uniformity in hidden data = V2-η of [Native-tag admission, trajectory weights and the obstruction to propagation] §5.1; data-form records (tag's own term): H′♯ + **(BV-Lip)** (open, [Native-tag admission, trajectory weights and the obstruction to propagation] H-5) |
| (Id-T) | source pieces = (2.1) on the proper tiling with root X₀ | (c) single-sequence form [II] pp.4–9; (c) the p.276 sentences; (a) summation over □, t; (d) proper-scale cubes = tiles of 𝒯^{(k)}, wall- vs ∗-connectivity (irrelevant to Theorem A, which bounds P(Y₀) for every Y₀), deformed δH_j := ∂_B of the deformed H_j |
| (Collar), (T-box), (T-sep) | as in [Cons] G2–G3 | source/additional assumption as recorded there |
| Lemma Traj (T2), T3 | R_b ≤ 2LR_{b+1}; tile layer count | deduction given [III] (2.6) ([Native-tag admission, trajectory weights and the obstruction to propagation]); (a) [Multiscale incidence and logarithmic jets] |
| Parameters | (PA1)–(PA5) | constraints on free constants; (a) arithmetic |

**Premise-table line V1-T after this note** ([Native-tag admission, trajectory weights and the obstruction to propagation] §7): *full-tree ancestors* source via [Multiscale incidence and logarithmic jets] §7 + Lemma CR deduction; *holed ancestors, any hole size, including the birth step*: **conditional by Prop. T1♯** on (M-loc-s), (Res-H), (Id-T), (Collar), (T-box), (T-sep), (PA1)–(PA5). The open entries of [Native-tag admission, trajectory weights and the obstruction to propagation] §7 for V1-T are discharged at level conditional.
