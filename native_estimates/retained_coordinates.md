# Retained coordinates, Haar factors and Schur kernels

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

## 2. Proposition BK, clause (2′), Proposition LAW

### 2.1 The source order of operations (source input; images)

Each stage n+1 (scale j = h+n) runs as follows.
1. The integral (1.25) is set up: "∫dA_j↾_{Z_{j+1}∩Ω_{j+1}}χ(Z_{j+1}∩Ω_{j+1})exp[−½⟨A_j,C*Δ^{(j)}_{Λ_{j+1}}CA_j⟩]·∫dV_j↾_{Ω^c_{j+1}∖Z″_{j+1}}δ(V̄_jV_{j+1}^{−1})…" (p.182).
2. Decomposition χ_k^{(n+1)}, which "does not depend on integration variables". Failing components are excluded.
3. "Using the Faddeev–Popov procedure we introduce the gauge fixing terms (1.5), (1.6) on the whole integration region" (p.182).
4. Decomposition χ′_j of (1.27), "under the integral (1.25)" (p.183). Failing components are excluded.
5. Decomposition (1.28) on χ_□^{(j)}. Failing components are excluded.
6. Proof of (1.29) (pp.183–187).
7. Only then: "Now let us come back to the integral (1.25) … We introduce the fluctuation field V′_j … (1.53) … we linearize the expressions in the δ-functions, we remove the δ-functions using the operator C, and finally we perform the scaling transformation" (p.187).
8. Decomposition χ′^{(j)} of (1.55), "in the obtained integral". Failing components are relocated by "(1.22) [III], with ℍ_Z^{(j)} instead of ℍ_{1,Ax}" and acquire (1.59) (p.188).
9. The passing components' integral (1.60); output ℂ^{(n+1)} (1.62).

After the N stages come (1.75) (p.193), the Λ-integration (pp.193–194), the tree gauge and (1.82) (p.196), and (1.88) (p.197). Failing components are excluded at each test. p.200: the remaining components have "many forms, varying from the old 𝕋-operations to the integrals as in (1.76) … These operations are denoted by 𝕋″_k".

So F(n,1)–F(n,3) fail at steps 2, 4, 5, before step 7. **V_j is raw in them.** In F(n,2) and F(n,3) it is the Faddeev–Popov representative (§2.4 (iv)). This settles the derivation's stated doubt. LFR II: a search in the source for "exclud", "large field function" and "decomposition of unity" finds only the class split after (1.70) (p.378) and a smooth localization partition (p.360). So the eight forms and the two classes are exhaustive **relative to the displayed tests**: source input for LFR I, source input for LFR II. SF4's "we will not attempt to give a systematic description of all possible cases" refers to the shapes of 𝕋_k inside a component (nested older operations), not to further tests.

F′ and F_P (pp.195–198, images): V″ = V′V₀ on Λ₀ = Λ∩Ω″^{∼2}_{h+1}, V₀ = M_{𝔹₀}(U₀), U₀ = U_{k,Z}(V_Λ). By Proposition 1 (p.194), V_Λ is a function of V_k↾Z∩Λ^c only. In the deep part, "The field V″ is equal to V_h on (Ω″^{∼2}_{h+1})^c∩□^{∼4}" ((1.92), p.198). The gauge change u₀ of (1.86) is a function of U₀. All of these are built from data inside the component, so **F′ and F_P have frozen data** source input. [Reconstruction and older Schur responses]'s table entry for F′ ("tree-gauge coordinates V′ of (1.81)") holds on Λ₀; deeper in, the coordinate is raw V_h. This does not change any conclusion.

The paragraph on p.191 says the insertion statement's proof "is almost identical to the proof of a similar statement for the configurations U_k^{(n)}, given in (44)–(52)". The interpretation of "(44)–(52)" is LFR I's own (1.44)–(1.52): the real-configuration proof on pp.186–187 that χ_k^{(n)} = 1. That is additional assumption. [RC] also has equations (1.44)–(1.52), but they are gauge-fixing estimates.

### 2.2 Lemma S (the relocated selectors are background-free)

Work on one free bond with V_jV_Z^{−1} = e^{ig_jB^{old}}e^{iℍ} and B^{old} = R_ℍ(B^{new}), so that e^{ig_jB^{old}} = e^{ig_jB^{new}}e^{−iγ(g_jB^{new})ℍ}. Here γ = 0 for |X| ≤ (4/3)δ′_j and γ = 1 for |e^{iX}−1| ≥ (5/3)δ′_j (SF6). Take any Ad-invariant norm with |e^{iX}−1| ≤ |X|, and assume |ℍ| ≤ δ′_j/3.

1. *Failure indicator.* For every threshold θ ≤ δ′_j: |g_jB^{old}| < θ ⇔ |g_jB^{new}| < θ. This covers (1.55) with B scaled or unscaled.
2. *First factor of (1.59).* χ′_j = χ(|V_jV_Z^{−1} − 1| < 2δ′_j) equals χ(|e^{ig_jB^{new}} − 1| < 2δ′_j).

Hence the product χ′_j(1−χ′^{(j)}) is a function of B^{new} alone. This is LFR I's "(1.59) … does not depend at all on the background fields".

*Proof.* (1) On the plateau γ = 0, R_ℍ(b) = b. If γ(gb) ≠ 0 then |gb| > (4/3)δ′, so |gR_ℍ(b)| ≥ |gb| − |ℍ| > δ′ ≥ θ and |gb| > θ. (2) Where γ = 1, V_jV_Z^{−1} = e^{igB^{new}} exactly. Where γ < 1, |e^{igB^{new}} − 1| < (5/3)δ′. Then |e^{igB^{new}}−1| < (5/3)δ′ < 2δ′. For the other quantity, use |WW′−1| ≤ |W−1| + |W′−1| (unitary W, W′; ℍ is real at birth) and |e^{iX}−1| ≤ |X|. This gives |e^{igB^{new}}e^{i(1−γ)ℍ}−1| < (5/3)δ′ + δ′/3 = 2δ′. So both indicators are 1. □

Lemma S is what Cor. BK1 needs in form F(n,4). It is also what [Cons] §1.1 / [Retained sigma-fields and conditional expectations] needs for "the selectors of all retained operations do not depend on z" (§3, item C-07).

### 2.3 Proposition LAW: two corrections

**E1 (Haar factor).** On a relocated bond, the density of the new variable is σ(g_jR_ℍconditional)·|det D_bR_ℍ(b)|, where σ is the Haar density in exponential coordinates. [Reconstruction and older Schur responses] item 2 keeps only j = log det D_bR_ℍ. On the plateau γ = 1 the map is a right translation by the constant e^{−iℍ}, so

 σ(gR_ℍconditional)|det D_bR_ℍ(b)| = σ(gb)

exactly. Then m(b;ℍ) := j(b;ℍ) + log σ(gR_ℍconditional) − log σ(gb) vanishes there, while j alone does not. On γ = 0 both vanish. So the true S5-J record is m, supported on the transition shell (4/3)δ′ < |gb| < (5/3)δ′-ish. It obeys the bounds of (J-a) with the same form, because log σ is analytic with derivative O(|gb|) = O(δ′).

Status deduction. This is [Rd] Lemma 2.2 ("the chart is a Haar-preserving reparametrization") applied on the plateau. **Repair:** replace j by m in Prop. LAW items 2–3, in Prop. J and in the budget. No estimate changes.

**E6 (what Y is at birth; status of (MC)).** At birth, LFR I (1.53)/(1.58) uses V^{(j)} = M^j(U_k^{(n+1)}) with U_k^{(n+1)} = U(𝔹_k^{(n+1)}, V) (source input; p.187). In 𝔹^{(n+1)}, every component still in Z at stage n+1 carries the (n+1)-structure. So for all components that fail (1.55) at the same stage, the stage data are absent, not "moving" as reading (MC) has it.

The source's mechanism for later stages is (1.60)–(1.62): every action term, including "the usual new terms in the action" of the relocation (p.188), is evaluated at U^{(n)}(exp i[g_jCB_j…]V^{(j)}) inside the integral. The difference from its value at U^{(n+1)} goes into ℂ^{(n+1)}. From stage n+2 onward, X's relocation terms are therefore re-evaluated at backgrounds in which the other stopped components carry their 𝔹^{(·)}-structure, with the data in the 𝔳-form (SF8's "generalize the definition of the spaces"). That is (MC).

Conclusion additional assumption: (MC) is a **representation convention**. It agrees with the source's re-evaluation from stage n+2 onward, and the switch at stage n+1 is absorbed exactly in ℂ^{(n+2)}, or in the first T step if n+1 = N. The alternative convention

 **(MC₀)** Y_X := M^{j_X}(U(𝔅^{[𝔛₄]}, 𝔡₀(ζ))), with the stage data of *all* F(·,4) components removed,

is equally legitimate. It agrees with the birth step for same-stage components. With (MC₀), v(ζ) is explicit: one application of HD for 𝔅^{[𝔛₄]}, then one for 𝔅. Lemma MD's fixed point and (H6)(Sep) are not needed. **One may use (MC₀).**

One remark on (G-T). The relocation terms are action terms (p.188: "new terms in the action"). So in the source's own representation Θ^J and Θ^A sit *inside* the T-step fluctuation integral. (G-T) concerns kernels of 𝕋-operations (S4, S2★), not S5. [Reconstruction and older Schur responses] §8 item 6 lists Θ^{PF}; that is overcautious and harmless additional assumption.

### 2.4 Clause (2″): repaired wording

> **(2″) Integrated data.** A T step integrates exactly its current free coordinates. An R step integrates:
> (a) all internal variables of its first-class components, including every older operation they contain;
> conditional in every component that enters the preparation of LFR I §1, whatever its later fate (first class, second class, or stopped), the variables 𝔰_i = (A_i↾Z_{i+1}∩Ω_{i+1}, V_i↾Ω^c_{i+1}∖Z″_{i+1}) of each completed preparatory stage (LFR I (1.25), (1.60));
> (c) the auxiliary variables the source integrates where it introduces or removes them: the primitive labels it resums (L1), and the gauge-orbit variables of its Faddeev–Popov insertions and removals (LFR I p.182, (1.76); LFR II p.378).
> No other retained field variable is integrated. At its birth step, the internal state of a new second-class component is either retained directly, or averaged under the H-03 posterior π_v and replaced by a copy resampled from π_v given v (Annex BI §8). The two options give the same joint law and the same T-step laws.
> **Coordinates.** Retained variables are carried in the coordinates in which the main-line representation leaves them:
> - literal construction: after a failed fluctuation test (LFR I (1.55)), the relocated coordinate of (1.59); after a T step, the relocated exterior fluctuation of [III] (3.22);
> - local construction (the local-test construction): the local charts of [Rd] (A2) and (A8);
> - after (1.76), the tree-gauge coordinates of (1.81) on Λ₀ and raw V_h deeper in;
> - in F(n,2)–F(n,4), the stage field V_j is the Faddeev–Popov representative.
> A component stopped after the Λ-integration keeps the old V_b↾Λ as a retained internal variable; the new V_b↾Λ is a fresh variable.

Hypotheses: source input for the source facts; (a) that (b) is forced by LFR I p.191.

Three points of the repair:
1. The birth-option sentence must stay. H-03's interface statement is "Annex BI is used in form DN-1 (2), second option (resample)" ([Det] l.277).
2. "(c) nothing else" in (2′) would forbid the integrations that L1 and the gauge restorations perform.
3. The Faddeev–Popov representative is harmless for T-step laws. Everything is invariant under the stage gauge transformations (LFR I p.182: "All the expressions and the functions in (1.25) are invariant …"), so conditioning on V_j and conditioning on its slice representative give the same conditional law of z.

## 4. Theorem CR, Lemma MD, Lemma A-cur, Lemma Δ

### 4.1 Theorem CR conditional on (H1)–(H7), (Ceil), with two amendments

The formula gives (CR2)–(CR3) from the main inequality of CT♯ with weights λd(·,E₀) and λd(·,x_i):
- the B₀ part has weighted norm ≤ C_Cg_kr, resp. ≤ C_Ce^{λr_C}g_k;
- the β part has weighted norm ≤ 2C_*C_Cg_kr, resp. ≤ 2C_*C_Ce^{λr_C}g_k.

Their sum gives K₁ = K_CTC_C(1+2C_*). The D*D row is used at a real critical base only, which is legitimate (E3 of [The one-sided collar estimate]). (CR4) is arithmetic and correct.

Amendments:
- **(Ceil+P).** Prop. AD uses the family along the real segment from 0 to ζ₀, with |z_{0,i}| ≤ P_k. The fixed point and the bound |B|_∞ < min(r₉, r_CT) are needed for data moves of size C_Cg_k(r+P_k). So (Ceil) must read 4C_*C_Cg_k(r+P_k) ≤ min(r₉, r_CT).
- **(Geo-PF) at both thresholds (E5).** CT♯'s (Geo) is CMP 96 (2.59), "½αδ₀RM > 2d log c₀(½α) + 1" source input. Its proof (Lemma 2.1) sums over surface crossings at cost e^{−½αδ₀·(layer width)} each, so the width enters exactly as RM does. Hence one-M-cube prepared layers need δ₀M > 4(2d log coth(δ₀/8)+1), which is 70.7 at δ₀ = 1, for the true package (HD, P9♮). If [Native-tag admission, trajectory weights and the obstruction to propagation] Prop. T2 is applied inside prepared regions, the s-deformed variant needs δ₀M > 16(2d log coth(δ₀/32)+1), which is **459.7** at δ₀ = 1. This is consistent with the source: LFR I p.186 "We choose M large enough, so that δ(M/M₁) ≥ 2" and p.200 "can be made arbitrarily small for M large enough".
- That P9♮ and HD apply to determining sets with thin layers is additional assumption, on the same footing as (P9-ms) in [Native-tag admission, trajectory weights and the obstruction to propagation]. The source asserts admissibility: p.179, "The sequence {Ω″_j} is an admissible sequence".

### 4.2 Lemma MD with modification conditional

The contraction is correct. Each split weight w̃ = w + (λ₁−λ)d(·,X′) is λ₁-Lipschitz and equals w on X′. The cross terms are bounded by θ_sep‖β‖_w.

Two gaps:
1. The contraction step uses *difference* bounds |log M((e^{iη𝓗}W)^u)·M((e^{iη𝓗′}W)^{u′})^{−1}| ≤ C_M sup(h|𝓗−𝓗′| + h²|∇(𝓗−𝓗′)| + |log u − log u′|), and the analogous difference form of (Fr-Lip). (H7) and (Fr-Lip) are stated only from a base. The difference forms follow from analyticity and Cauchy for small arguments additional assumption, but must be listed.
2. The real slice is defined globally by continuing along real segments under (Ceil+P).

With (MC₀) (§2.3) the lemma reduces to two applications of HD. (H6)(Sep) and the contraction disappear.

### 4.3 Lemma A-cur and Lemma Δ — hold

Lemma A-cur is [Native-tag admission, trajectory weights and the obstruction to propagation] Theorem H′ with the current reconstruction; There is no identified error.

Lemma Δ: by Cauchy, ‖D𝔊(q)‖ ≤ (2/3)w/ρ ≤ w/ρ and ‖D²𝔊(q)‖ ≤ (8/9)w/ρ² ≤ 2w/ρ² on the ball of radius 3ρ/2. The constant 3 is right deduction. The "norm" is the sup over sites of matched norm divided by the reserve ρ̂(x), on a finite product domain. Cauchy estimates hold there.

## 5. Propositions J and AD

### 5.1 Prop. J with modification

(J-a): ‖D_bR − 1‖ ≤ C_Ψ(1+C_γ)|ℍ|/δ′, |j| ≤ 2dim𝔤‖E‖, and Cauchy from 2c₀δ′ to c₀δ′ gives C_j = 4dim𝔤C_Ψ(1+C_γ) deduction. With m in place of j (E1) the same bounds hold, with C_j enlarged by sup|D log σ| = O(δ′).

(J-b) is correct given Theorem CR for 𝔅^{[X]}. (H-real) at later steps is now conditional, by Lemma PERS (b) (§6.2). It is the source's own (1.57) mechanism at later times.

### 5.2 Prop. AD conditional

The resulting inequalities are:
- the base W₀^{frz}, and |β^{ref}| ≤ 2C_*C_CC_Σg_k(r+P_k)e^{−(λ/2)d(·,E₀)} under (Ceil+P);
- the values bound, using λ₁ ≥ λ/2, d(y,c)+d(source input; E₀) ≥ d(y,E₀) and d(source input; E₀) ≥ D_k−2;
- the two derivative terms, the second by Cauchy in the β-direction;
- the application of Lemma Δ.

All correct.

**E4.** The S5-A records have rate λ/4 = δ₀/32, so with (Met) the common ν for them is c_metδ₀/32. [Reconstruction and older Schur responses] §8 item 4 says c_metδ₀/16. Its own §11 says /32, which is correct.

**(Abs).** For the E- and R-records, C-02 (Annex AD, Theorem E14.3) and C-03 (Annex AE, Theorem R14.3) already give simultaneous native-background contours with explicit radii and summable majorants. These are proposition, a better source than "assumption/(d)". What remains (d) is that their native radius dominates the reserve ĉα_{∧,n} used in Lemma Δ.

## 6. (Dom-PF): exact statement, what is proved, what is missing

### 6.1 The statement C-05 needs

Fix a T step k ≥ b and a component X stopped at the R step of scale b in form F(n,·). Let ρ be a record whose carrier X_ρ meets X. Such records are:
- the stage outputs ℂ^{(i)}(Y,·), i ≤ n, of LFR I (1.63);
- old E, R, B terms evaluated at U^{(n)};
- R-step outputs crossing X.

The statement needed is:

> **(Dom-PF)_k.** 𝔈_ρ(·;a) is holomorphic and bounded by w_ρ on the native ball of layerwise radius 2ρ_PF(m) about every real background W₀ occurring at step k at a real point of the support. Here m runs over the layers of the prepared structure of X (and the ordinary layers outside X), uniformly in the slots a.

This splits into three parts.
- **(DP1) Birth domain.** LFR I (1.70) (source input; p.192): "each term ℂ_k^{(n)}(X,U_k^{(n)}) can be extended to an analytic function defined on the space Ũ_k^{(n)c}(X,α̃₀,α̃₁) and satisfying |ℂ_k^{(n)}(X,(𝕌,𝕁))| ≤ C₀exp(−(1+3β)κd_m(X))". This rests on the insertion statement (p.191, source): "if 𝕌 is an element of the space Ũ_k^{(n+1)c}(X,α̃₀,α̃₁), then exp iηℍ_k^{(n)}(g_jCB_j − hD̃(g_jCB_j))𝕌 is an element of the space Ũ_k^{(n)c}(X,α̃₀,α̃₁) … we will not repeat it". It also rests on the generalization of the spaces to stopped components "for the next steps" (SF8).
- **(DP2) Persistence.** At every later step, the actual real W₀, restricted to the prepared layers of X, lies in the real part of Ũ_b^{(n)c} with a margin.
- **(DP3) Reserve.** The native ball of radius 2ρ_PF(m) about such a W₀ lies inside Ũ_b^{(n)c}.

**Simplification.** In Theorem CR, Lemma A-cur and Prop. AD, the move of the background at any point of X is collar-small: ≤ K₁g_kr·e^{−λ(D_k−2)}. For records whose carrier lies in Z_k, (DP3) is therefore needed only with a reserve ρ_PF ≥ ℓ_b^{−C}α_{∧,b}, i.e. with a polylogarithmic loss, which the factor e^{−λ(D_k−2)/2} absorbs. For records crossing X and reaching E₀, the reserve near E₀ is the ordinary (Res). So the exact profile (Res-pat-PF) is not needed. The parameter condition q₀, q₁ > p₀ + r + 2 of PF.3 is needed only if one wants the profile.

### 6.2 Lemma PERS (persistence through T steps) — conditional

Let X be as above, and let k ≥ b be a T step before any later R step that processes the large-field component containing X. Let W_X := U(𝔹^{(n)}(X), d_X) be the localized background of LFR I (1.20) built from X's own data. These data are frozen at later steps, by Cor. BK1; in F(n,4) the stage datum takes its value at the real point considered. Assume:

- (HD-loc) [The one-sided collar estimate] Corollary HD / CT♯ item 3 for the localized determining set 𝔹^{(n)}(X), at the real critical base W_X. This presupposes [V]-type and (Geo-PF) additional assumption.
- (Reg-∂) At the real point considered, the datum b_∂ := (1/i)log[M(W₀^{(k)})·M(Q^{s*}V_b)^{−1}] is supported in the 2M₁-layer at ∂X, and |b_∂|_∞ ≤ C_∂ε_b < r_CT. At k = b this is LFR I (1.56)–(1.57) (source input; p.188): "has a support in the boundary layer of the width 2M₁ at the boundary of Z, and is bounded by 44d²B₃ε_k". At k > b it is additional assumption. The data in the layer are frozen raw V_b on Z∩Ω_b, and the global background there is scale-b regular by the multiscale regularity of [V] Thm 1 / [III] (3.12) assumed input.

Then on X:
- W₀^{(k)} = (e^{iη𝓗_∂}W_X)^{u}, with h_m|𝓗_∂| + h_m²|∇𝓗_∂| + h_m³|D*D𝓗_∂| ≤ K_CTC_∂ε_b·e^{−λd(y,∂X)} at every block y of layer m.
- On the stage regions, which lie at distance ≥ D_∂ := 10M(R_{j+1}+…+R_{b−1}) + MR_b from ∂X ((1.57), c), the following hold uniformly in k:
 1. W₀^{(k)} and W₀^{(b)} differ by ≤ 2K_CTC_∂ε_be^{−λD_∂} in matched units;
 2. the relocation field satisfies |ℍ_u| ≤ C_M(1+C_a)K_CTC_∂ε_be^{−λD_∂}. This is (H-real) at all later steps, under the ceiling C_M(1+C_a)K_CTC_∂ε_be^{−λD_∂} ≤ ½c₀δ′_j. Use the same argument with 𝔹^{(n+1)}(X), whose localized background has M^j equal to V_Z;
 3. if W₀^{(b)} satisfies the real conditions of Ũ_b^{(n)c} on the prepared layers with margin m₀ (**(DP-margin)**, additional assumption), then W₀^{(k)} satisfies them with margin m₀ − 2K_CTC_∂ε_be^{−λD_∂}·C. The same holds for the auxiliary reconstructions U_{p,X}(M(W₀)) of (1.65)–(1.69), by CT♯ item 3 at the bases U_{p,X}(M(W_X)).

*Proof.* The global minimizer restricted to X and W_X have the same interior data on 𝔹^{(n)}(X). They differ only through the boundary datum b_∂. This is LFR I (1.56), "U_k^{(n+1)} = (exp iηℍ_{k,Z}^{(n+1)}((1/i)log[M(U_k^{(n+1)})(M(Q_k^{s*}V_k))^{−1}])U_{k,Z}^{(n+1)})^{u^{−1}}" (source input; p.188), used at step k; that its validity uses only minimality and the shared interior data is additional assumption. Apply CT♯ item 3 at the real critical base W_X with S = the boundary layer, and (Fr-Lip) for u. Item 1 is the triangle inequality between steps k and b. Item 2 is the same argument for the (n+1)-structure, followed by (H7). Item 3: the real conditions are continuous in matched norms, and U_{p,X}(M(·)) is a reconstruction from averages, so CT♯ item 3 applies to it. □

Near ∂X the conditions of the space are the ordinary layer conditions (iii) of (1.68). There PERS is not small, but the ordinary multiscale regularity (Reg) applies, as for all S1a records additional assumption.

### 6.3 Lemma INS (the insertion statement) — reduction conditional; additional assumption, not completed

**Claim.** Let (𝕌,𝕁) ∈ Ũ_b^{(n+1)c}(X), and let B_j be real on the stage set S_j with |g_jB_j| < 6δ′_j. Put 𝕌′ := e^{iηℍ^{(n)}(g_jCB_j − hD̃)}𝕌, where ℍ^{(n)} is the response of the reconstruction on 𝔹^{(n)}(X) at the complex base 𝕌 to the datum supported on S_j. Then (𝕌′,𝕁′) ∈ Ũ_b^{(n)c}(X).

**Reduction.**
1. *Response bound.* CT♯ item 2 at the complex base 𝕌 ([The one-sided collar estimate] §5.2, conditional on (K♯) at complex backgrounds, **including K3 = (3.132) at complex backgrounds, which the representation convention lists as not yet checked**) gives h_m|ℍ| + h_m²|∇ℍ| ≤ K_CT·6δ′_je^{−λd(y,S_j)}. This replaces the source's (1.45), which cites B₃.
2. *Entry (A′).* Write 𝕌′ = (e^{iηℍ}U′)U with the same real part U. The entries |A′|, |∇A′| change by at most the bound in step 1. The entries |∂U−1| and the axial-gauge bounds (1.65)/(1.67)/(1.69) on U are unchanged.
3. *Entry |∂𝕌−1|.* This is (1.46)–(1.48) verbatim, with K_CT in place of B₃.
4. *Entries U_{p,X}(M(𝕌′)).* The averages change by at most step 1's bound. CT♯ item 3 at the complex base U_{p,X}(M(𝕌)) then gives a response of ≤ K_CT²·6δ′_je^{−λd/2}.
5. *Entries 𝕁, J_{p,X}.* These need the Δ row (a representation output, available at complex bases) or CT-J (item 6). D*D is not available at complex bases (E3 of [The one-sided collar estimate]).
6. *Margins.* Ũ^{(n+1)c} is stricter than Ũ^{(n)c} at layer m by the term β2^{−|m−j−1|}·(entry). Under (Geo-PF), e^{−λM(|m−j|−1)₊} ≤ 2^{−|m−j−1|}, so the margins absorb steps 2–5 provided

 **(PAR-INS)** C·K_CT²·6δ′_j ≤ β·min_m(α̃_{0,m}, α̃_{1,m}).

 This is a ceiling of the same type as the source's "9B₃(A₁/A₀)(p₁(γ)/p₀(γ))(1+β₀) … can be made arbitrarily small" (p.186, c) and as the collar estimate's A₀ ≥ 80K_CTA₁.

**What is missing, precisely.**
- (i) The entry-by-entry transcription of (1.65)–(1.69). Several L₀-exponents are hard to read at 110 dpi, and The argument assumes them.
- (ii) K3 at complex backgrounds (the representation convention).
- (iii) (DP-margin): that the χ^{(n)}-conditions (1.24) on the localized background imply the real conditions of Ũ^{(n)c} with a margin. The space "is modelled on the definition (1.24)" (p.190, c), but its constants α̃_{0,m} are not ε_m, and the relation is not displayed.
- (iv) Repeated R steps on X's component. This is the existing premise V2-R, not specific to stopped components.

Nothing in Theorem CR, H′ or the Local deformation of propagators and the minimizer/Source operators for the deformed reconstruction chain supplies (DP1). Those results all start from a real base inside the domain and control moves from it. Lemma PERS is the new ingredient for (DP2).

**Status of (Dom-PF):** (1.70) source assumption → reduced to Lemma INS (b on CT♯ at complex bases and (PAR-INS); additional assumption for the transcription and for K3 complex) + (DP-margin) (d) + Lemma PERS (b on HD-loc, (Reg-∂) additional assumption) + a polylogarithmic reserve (deduction; by the collar) + V2-R.

## 7. (OR-K): derivation

### 7.1 The objects

Fix the scale j and one component of Z_{j+1}∩Ω_{j+1}. Let 𝔽 be the free bonds of Ω_{j+1} at scale j, L ⊂ 𝔽 those in Λ_{j+1} (the set Λ̃ of [P] (3.156)), and Z the free bonds of the component. Let K(W) := C*Δ^{(j)}(W)C, with blocks K_{LL}, K_{LZ}, K_{ZL}, K_{ZZ}. The Schur form of [III] (2.21) is

 S(W) := K_{ZZ} − K_{ZL}K_{LL}^{−1}K_{LZ}.

[P] (3.158), image p.428: "(C*Δ_kC)^{−1} = C̃^{(k)}(Λ) = C^{(k)}(Λ)↾_{Λ̃}".

Let d be the distance in scale-j units, c(δ) := sup_r Σ_s e^{−δd(r,s)}, and ‖·‖_x the matched norm on the block x. The complex domain 𝔘 consists of W = e^{iηA′}W₀ with W₀ real satisfying [P] (3.35)–(3.36) and matched norms of A′ ≤ ϱ.

### 7.2 Inputs

- **(SK1-real)** For real W: |K(r,s)| ≤ B₀e^{−δ₀d(r,s)}, and |K_{LL}^{−1}(r,s)| ≤ B₀e^{−δ₀d(r,s)}. Sources (source input; images p.428 and p.432): C^{(k)}(Λ) "is defined by a positive definite operator C*Δ_kC with a lower bound γ₀ > 0 independent of k and U … for C*Δ_kC with an arbitrary configuration U satisfying (3.35), (3.36) … This property, together with a uniform exponential decay of C*Δ_kC implies bounds and uniform exponential decay for C̃^{(k)}(Λ)". Theorem 3.15: "|C^{(k)}(Λ;y,y′)| ≤ B₀e^{−δ₀|y−y′|} … with the constants B₀, δ₀ depending on d and L only".
- **(SK1-K)** K extends holomorphically to 𝔘 with the same kernel bound. Source: [P] Theorem 3.4 (source input; p.400): "the operators G′(U), (Q′(U)G′²(U)Q′*(U))^{−1}, R(U), G(U) extend to configurations U′U for α₁ ≤ a₁ as analytic functions of A. The extended operators satisfy all the inequalities of Theorems 3.1–3.3". This applies to the constituents of Δ_k through (3.156).
- **(SK2) Vertex bound.** For W ∈ 𝔘 and δA′ supported on one block x: |DK(W)[δA′](r,s)| ≤ B₀e^{−δ₀(d(r,x)+d(x,s))}‖δA′‖_x.

### 7.3 Lemma V (vertex bound from structure) — deduction, given (S-struct-K) and (K♯)

Suppose an operator T(W) is built from finitely many operators L_i(W) by sums, products and inverses. Suppose each L_i is local with local W-dependence:

 |DL_i[δA′_x](r,s)| ≤ C·1{d(r,x), d(x,s) ≤ c_loc}‖δA′‖_x.

Suppose every inverse appearing satisfies the kernel bound Be^{−δ₀d} on 𝔘. Then T satisfies (SK2) with constants depending on the expression, at rate δ₀/2^{depth}.

*Proof.* Induction on the expression:
- D(T₁+T₂) = DT₁ + DT₂.
- D(T₁T₂) = (DT₁)T₂ + T₁(DT₂). Convolve: Σ_y e^{−δ(d(r,y)+d(y,x))}e^{−δd(y′…)} ≤ c(δ/2)e^{−(δ/2)(…)}, using the triangle inequality.
- D(T^{−1}) = −T^{−1}(DT)T^{−1}.
- Base case: local operators, e.g. Δ_{U′U} = Δ_U − V′₁(A) with V′₁ "the first order operator" of [P] (3.50)–(3.53) (source input; p.400). □

**(S-struct-K)** additional assumption: C*Δ^{(j)}C is such an expression, via (3.156) ("⟨B,(QG₁Q*)^{−1}B⟩ − a⟨B,B⟩ − 2⟨H₁𝔇^{(2)}(B),J⟩ = ⟨B,Δ_kB⟩", c, p.428) and the definitions of G₁, H₁, R, Q as composites of local operators and the inverses of (K♯). [Source operators for the deformed reconstruction] Prop. W♭ / [Local deformation of propagators and the minimizer] §4.1 classify G₁ and H₁ as composites. So (SK2) is conditional on (K♯) at complex backgrounds, the same input as CT♯, and on (S-struct-K).

This is the background-variation statement "CT-U" of [The one-sided collar estimate] §8.4, carried out for the operator K at primitive level. [The one-sided collar estimate] stopped at P₁(A), the non-local term through R(U′U). In Lemma V, R is itself a composite with an inverse, so the induction handles it, provided R(U) is written as such. That is the content of (S-struct-K).

A second route is to apply Cauchy to each walk term of [P] Theorems 3.9/3.10 ("A term … depends on configuration U restricted to X₀⁵∪…") together with [Source operators for the deformed reconstruction] Prop. W♭ on the complex domain conditional.

### 7.4 Lemma SK — deduction given (SK1-real), (SK1-K), (SK2)

Let c := c(δ₀/4) and suppose 2ϱB₀²c³ ≤ ½. Then on 𝔘:

1. K_{LL}^{−1} exists, is holomorphic, and |K_{LL}^{−1}(r,s)| ≤ 2B₀c·e^{−(δ₀/2)d(r,s)}.
2. S is holomorphic and |S(r,s)| ≤ B_Se^{−(δ₀/4)d(r,s)}, with B_S := B₀ + 2B₀³c³.
3. |DS(W)[δA′](r,s)| ≤ B′_S Σ_x e^{−(δ₀/4)(d(r,x)+d(x,s))}‖δA′‖_x ≤ B′_Sc(δ₀/8)·sup_x e^{−(δ₀/8)(d(r,x)+d(x,s))}‖δA′‖_x, with B′_S := B₀(1+4B₀²c⁴+4B₀⁴c⁸).

*Proof.* Write ‖T‖_δ := max(sup_rΣ_s, sup_sΣ_r)|T(r,s)|e^{δd(r,s)}. This is submultiplicative by the triangle inequality, and a kernel bound Be^{−δ₀d} gives ‖T‖_{δ₀/2} ≤ Bc.

(1) Let W₀ be the real point. By (SK2) integrated along the segment, ‖K(W)−K(W₀)‖_{δ₀/2} ≤ B₀c²·2ϱ. Then K_{LL}(W)^{−1} = Σ_n(−G₀ΔK)^nG₀ converges in ‖·‖_{δ₀/2} with ‖G₀ΔK‖ ≤ ½. Holomorphy follows from uniform convergence.

(2) Use the triangle inequality on the chain r→y→y′→s and split the exponent.

(3) DS = DK_{ZZ} − DK_{ZL}GK_{LZ} − K_{ZL}GDK_{LZ} + K_{ZL}G·DK_{LL}·GK_{LZ}, with G := K_{LL}^{−1}. In each term the chain from r to the vertex at x has total length ≥ d(r,x), and the chain from x to s has length ≥ d(x,s). There are at most four intermediate sums. The last inequality uses Σ_x e^{−(δ₀/8)(d(r,x)+d(x,s))} ≤ c(δ₀/8). □

### 7.5 Consequence

**(OR-K)** holds with δ_S = δ₀/8 and B_S := max(B_S, B′_Sc(δ₀/8)) on the ball of matched radius ϱ. The form with 1/ρ_S in [Reconstruction and older Schur responses] is weaker, since ρ_S ≤ 1.

The required radius is 2ρ_S(n) = (β/4)α_{∧,n} ≤ ϱ = min(α₁, 1/(4B₀²c³)). Call this **(Res-OR)**. It holds for small couplings because α_{∧,n} → 0 and α₁ is absolute additional assumption.

The step from the T-step background at a later scale k > j to the regularity hypotheses (3.35)–(3.36) for the scale-j sequence is additional assumption: finer-layer regularity implies coarser-layer regularity, as in (Res-pat).

Prop. OR then holds conditional on: Lemma SK; (SK1-real) source input; (SK1-K) (source input; Thm 3.4); (S-struct-K) additional assumption with (K♯) at complex backgrounds; (Cov-OR) additional assumption; (Met) additional assumption; (Traj-w) additional assumption; (Res-OR) additional assumption.

**S4 now rests on the printed kernel bounds and on one structural reading, under the structural reading.** It does not need (K♯) alone: (S-struct-K) is genuinely extra. It is the same kind of reading as (S-struct) of [Local deformation of propagators and the minimizer] for the minimiser.

## 8. S6: Proposition Het and Lemma P — hold conditional

- Recursion (AB17.22):.
- Lemma P: ∂_i tr W(∂p) = tr(W(∂p)Y_i) = tr((W(∂p)−1)Y_i) because Y_i ∈ sl(N,ℂ) is traceless. The same holds for W^{−1}. The bound is (ε^♯ + C_Pβ)β_i(η/h)⁴. The BCH constants are additional assumption.
- Plaquette count: 6(Mh_n/η)⁴ in d = 4, which cancels (η/h)⁴. 
- Real slice: s_p is gauge invariant. 
- Support: the arithmetic B_AF = 1.13·2^{0.13} = 1.237 ≤ 5/4 checks; at β₀ = ¼ one gets 1.486. So [Reconstruction and older Schur responses]'s correction of [U17] is right.

## 9. The budget of [Reconstruction and older Schur responses] §8 with corrections

𝔖_k is as in [Reconstruction and older Schur responses] §8 item 4, with three changes:
- W^J computed with m instead of j (E1);
- ν ≤ c_metδ₀/32 for the S5-A term (E4);
- (Geo-PF) at both thresholds if Prop. T2 is used inside prepared regions (E5).

ε_PF𝔖^{abs}/r² → 0 holds: ε_PF ≤ C(1+P_k/r)e^{−λ(D_k−2)/4} with D_k = 8LR_{k+1} superlogarithmic, and 𝔖^{abs} is polylogarithmic.

## 10. The local R-test (requirement: "F(n,4)-type structure at every T step in the bulk")

**The indicated statement does not follow from [Reconstruction and older Schur responses] §10 item 1 (or the conditional-coordinate convention item 4) for the local construction. (E3)**

[Reconstruction and older Schur responses] cites [Rf] (M5); the local-test construction uses [Rd] (A1)–(A10) instead. Under the local construction:

1. **Bulk.** (A2) uses the chart Ã on all starred bonds of Ω_{k+1}. On R-tested bonds it is relative to V_b^{(k)} = M^k(U_{k+1,b}), with box □_b^{∼4}. By (B5), "for b ∈ 𝔅_{k+1} with an endpoint in S^{∼2}_{k+1}, □_b^{∼4} ⊂ Λ^c_{k+1}" ([Rd] Lemma 2.1, text). On the outermost bonds it is relative to the source's localized V^{(k)}_{Λ^c_{k+1}∩Λ_k}, with cutoff 1. Both backgrounds are built from V_{k+1} and older data on Λ^c_{k+1}. These are retained raw at every later step: the next fluctuation lies in Ω_{k+2} ⊂ Λ_{k+1}. **So the postponed exterior datum is frozen at later steps.** The chart is a right translation, so its Jacobian, Haar factor included, is exactly 1 ([Rd] Lemma 2.2, and check H for the plateau). **No S5-type sector arises in the bulk** (deduction; given (A2), (B5)).
2. **Prefix.** (A8): "replace the fluctuation B_j of (1.53) by the fluctuation against the component-local background V_j(b) = e^{ig_jB^Z_j(b)}V^{(j)}_Z(b), V^{(j)}_Z := M^j(U^{(n+1)}_{k,Z}) … in all components … Equivalently: apply the source's own change of variables (1.58)–(1.59) with cutoff 1 in every component before testing" ([Rd] §2.6). In a component failing (1.55), the retained datum e^{ig_jB^Z}V_Z^{(j)} is frozen and the Jacobian is Haar-trivial. **F(n,4) reduces to case 1 of Prop. LAW, and S5 = ∅** (deduction; given (A8)). This is the conditional anticipated in [Reconstruction and older Schur responses] §10 item 2, and it holds.
3. Even under (M5), with g ≡ 1 relative to a moving background, the Jacobian-with-Haar-factor vanishes identically. Only an S5-A-type term would remain. [Reconstruction and older Schur responses]'s "D_bR_H − 1 = O(|H|)" is the E1 error again.

**Consequence.** Under the working construction (the local-test construction stage 1, the local-test construction):
- Props J and AD and Lemma MD are not needed;
- Theorem CR is needed only with 𝔛₄ = ∅, where it restates [Native-tag admission, trajectory weights and the obstruction to propagation]'s (E-data) step;
- the older sectors are S4 and S6, plus (Dom-PF) for the stopped components' records.

Under the literal fallback, Props J and AD (as corrected) cover S5, and the exterior relocation of later T steps is the source's S1d/S1a bookkeeping.

The (A8) terms of *passing* components are integrated into ℂ^{(n+1)}. They are records with a weight-g^{κ₀}-type bound ([Rd] §7.2), covered by (Dom-PF) like the other stage outputs.
