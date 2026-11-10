# Reconstruction and older Schur responses

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

**Conditional coordinates.** Clause (2″) in [Retained coordinates](retained_coordinates.md) specifies all variables integrated, including the completed preparation stages and auxiliary gauge variables. On a relocated bond the log Jacobian is combined with the Haar density ratio.

## 3. S5, part 1: what a stopped preparation has integrated

Notation: the R step acts at scale b (called k in LFR I); h = b − N; stage n+1 (0 ≤ n < N) treats scale j = h+n. Z is the union of eligible components; "component" means one component X of Z.

### 3.1 Source facts

**SF1** (LFR I p.180, source). (1.18): "U_k^{(n)} = U_k^{(n)}(V) = U(𝔹_k^{(n)}, V)"; (1.19)–(1.20): "The corresponding functions are defined by the gauge fields V restricted to Ω_k^c, and by M_{𝔹_k(Z)}(Q_k^{s*}V_k) restricted to Z∩Ω_k, thus U^{(n)}_{k,Z} = U^{(n)}_{k,Z}(V) = U(𝔹_k^{(n)}(Z), (M^·(Q_k^{s*}V_k)↾_{Z∩Ω_k}, V↾_{Z∩Ω_k^c}))". So the localized backgrounds depend only on fields **inside Z**.

**SF2** (p.181, source). (1.22): "χ_k^{(0)} = χ({|U^{(0)}_{k,Z}(∂p) − 1| < (1 − β½)ε_h(L^{k−h}η)² for p ∈ Ω_h∖Ω_{h+1}})"; "In components with the function 1 − χ_k^{(0)} we have introduced new large fields, therefore they do not satisfy the condition (ii), and we exclude them from the region Z. They are not changed by the subsequent operations, and we treat them in the same way as the remaining large field regions."

**SF3** (p.182, source). "We integrate with respect to the variables A_j, V_j localized in Z_{j+1}∖Z″_{j+1}. It is a part of the operation 𝕋^{(j)}(Z_{j+1}), and we have to consider the following integral ∫dA_j↾_{Z_{j+1}∩Ω_{j+1}}χ(Z_{j+1}∩Ω_{j+1})exp[−½⟨A_j, C*Δ^{(j)}_{Λ_{j+1}}CA_j⟩]·∫dV_j↾_{Ω^c_{j+1}∖Z″_{j+1}}δ(V̄_jV_{j+1}^{−1})ζ(Ω^c_{j+1})χ_k^{(n)}exp A_k^{(n)} (1.25)"; "The function χ_k^{(n+1)} does not depend on integration variables"; "Using the Faddeev–Popov procedure we introduce the gauge fixing terms (1.5), (1.6) on this set"; (1.26)–(1.27): "V_Z^{(j)} = M^j(U_{k,Z}^{(j+1−h)}), χ′_j = χ({|V_j(b)(V_Z^{(j)}conditional)^{−1} − 1| < 2δ′_j for b ∈ (Ω^c_{j+1}∖Z″_{j+1})^{(j)*}})".

**SF4** (p.183, source). (1.28), and: "Let us notice that all the characteristic functions introduced above depend on the field variables localized in the corresponding components of the large field region Z_k. This is an important part of the inductive assumption for the effective density, more precisely for the operation 𝕋_k(Z_k). It is also clear how this operation has been changed by the above decompositions, but we will not attempt to give a systematic description of all possible cases; there are too many of them".

**SF5** (pp.187–188, source). (1.53): "V′_j = V_j(V^{(j)})^{−1}, V^{(j)} = M^j(U_k^{(n+1)}), B′_j = (1/i)log V′_j" — the fluctuation is taken relative to the **global** background; (1.55): "χ′^{(j)} = χ({|B_j(b)| < δ′_j for b ∈ (Ω^c_{j+1}∖Z″_{j+1})^{(j)*}}). We exclude from Z the components with the large field function 1 − χ′^{(j)}. In these components we have to localize the dependence on the field V in the characteristic functions (1.27)"; (1.58): "V^{(j)} = exp i ℍ_Z^{(j)} V_Z^{(j)}, where ℍ_Z^{(j)} … is an analytic function of the configuration U_k^{(n+1)} restricted to Z, and on (Ω^c_{j+1}∖Z″_j)^{(j)} it is bounded by O(1)exp(−R_j)ε_j"; "Now we make the change of variables (1.22) [III], with ℍ_Z^{(j)} instead of ℍ_{1,Ax}, for the bonds belonging to (Ω^c_{j+1}∖Z″_{j+1})^{(j)*}, or rather to the components of this set with the large field function 1 − χ′^{(j)}. This change of variables transforms the function χ′_j(1 − χ′^{(j)}) into χ({|exp ig_jB_j(b) − 1| < 2δ′_j for b ∈ (…)^{(j)*}})(1 − χ′^{(j)}) (1.59), which has the required property, in fact it does not depend at all on the background fields. The change of variables gives also the usual new terms in the action."

**SF6** ([III] pp.251–252, source). (1.22): "A(b) = (1/ig₀) log exp ig₀A′(b) exp(−ig(A′conditional)ℍ_{1,Ax}conditional)"; "g is a C^∞-function defined on the Lie algebra 𝔤, 0 ≤ g(A′) ≤ 1, g(A′) = 0 on {A′ : |A′| ≤ 4/3 g₀^{−1}δ₀}, g(A′) = 1 on {A′ : |exp ig₀A′ − 1| ≥ 5/3 δ₀}"; (1.24): the Jacobians "can be exponentiated … and they yield the expression Σ_{b∈S₁*} Tr log[1 + ∂/∂A(b)(−(1/g₀)g(A(b))ℍ_{1,Ax}(b) + (1/g₀)𝐅(…))]"; "we obtain a new expression V^{(0)}(S₁, A, ℍ_{1,Ax}) … The dependence on ℍ_{1,Ax} is analytic, and the expressions are small".

**SF7** (LFR I pp.188–189, source). (1.60)–(1.62): the stage integral has "the form of the fluctuation field integral in (3.25) [III]"; "the integration in (1.60) is localized in the large field region Z, therefore the integral contributes to the boundary terms only"; "ℂ_k^{(n+1)} = log(the ∫ in (1.60)) + A(1/(g_k^{(n+1)}(·))² − 1/(g_k^{(n)}(·))², U_k^{(n+1)}), 𝔹_k^{(n+1)} = 𝔹_k^{(n)} + ℂ_k^{(n+1)}".

**SF8** (p.191, source). "Finally let us remark that if in a component of Z we finish the integrations for some n, because some new large field has been introduced, then we leave the new terms 𝔹_k^{(n)} as a part of all boundary terms, and it is easy to generalize the definition of the spaces in such a case for the next steps." On the same page: "we have to prove that if 𝕌 is an element of the space Ũ_k^{(n+1)c}(X, α̃₀, α̃₁), then exp iηℍ_k^{(n)}(g_jCB_j − hD̃(g_jCB_j))𝕌 is an element of the space Ũ_k^{(n)c}(X, α̃₀, α̃₁) … The proof is almost identical to the proof of a similar statement … and we will not repeat it."

**SF9** (p.192, source). (1.70): "|ℂ_k^{(n)}(X,(𝕌,𝕁))| ≤ C₀ exp(−(1+3β)κ d_m(X))"; "L₀^{2N₀} ≤ (1/3)^{N₀}L(L+1)(N₀+1)^{β₀}R_k < L(L+1)N₀^{−1}R_k"; (1.71)–(1.72): after the N integrations "𝕋″^{(j)}(Z″_{j+1}) = ∫dV_j↾_{Z″_{j+1}}δ(V̄_jV_{j+1}^{−1})".

**SF10** (p.193, source). (1.75) χ_{k,Λ}, "The restriction introduced by this function is on the field V_k↾_{Z∩Λ^c} only"; and: "All the above transformations preserve the k-th density ρ_k, they change only the representation of this density. … Now we define the next operation, which changes the density. The equality sign is replaced by the equivalence sign … The next operation is an integration of this term with respect to the field variables V_k over the domain Λ."

**SF11** (p.194, source). "We obtain a new expression, which we consider as a function of all field variables V_k, but independent of V_k↾Λ"; (1.76): "χ_k(Ω_k^{∼4})χ_{k,Λ}∫dV_h↾_{Z_h}χ_h(Ω_h∩Z_h)𝕋_h(Z_h)∫dV″↾_{𝔹″_k∩(Λ∩Z_h^c)}χ″_k exp A″_k … In fact the first integral, over the region Z_h, is left unchanged in the following discussion."

**SF12** (pp.196–197, (source)). A tree gauge δ_{T₀}(V′) is introduced in (1.76) by Faddeev–Popov; (1.82): "χ′ = χ({|B′conditional| < δ′_k for b ∈ 𝔹₀})", "we exclude from Z the components with the large field function 1 − χ′"; (1.88): a decomposition over subsets P of (Ω″_{h+1})^c∩Ω_h on the fields V_h, "We have new large fields in components with nonempty sets P, so we exclude these components from Z."

**SF13** (p.200, source). "the remaining components, for which the integral operations have many forms, varying from the old 𝕋-operations to the integrals as in (1.76), but with some large field characteristic functions, through the intermediate operations described above. These operations are denoted by 𝕋″_k."

**SF14** (p.179, source). (1.10)–(1.11): the prepared regions Z″_k, …, Z″_{k−N₀+1} are "separated by one layer of M-cubes" at their own scales; "Z″_j = (Ω_j^{∼5})^c∩Z for j = k−N₀, …, h+1; Z″_j = Z_j for j = h, …, 1".

### 3.2 Proposition BK (the forms of a stopped component)

Let X be a component of the eligible union at the R step of scale b. After the R step it is in exactly one of the following states. "Integrated" means: integrated by the source at this R step, hence not in 𝒢★ afterwards. Stage i+1−h integrates the pair 𝔰_i := (A_i↾Z_{i+1}∩Ω_{i+1}∩X, V_i↾(Ω^c_{i+1}∖Z″_{i+1})∩X).

| Form | Stopped at | Integrated at this R step | Retained internal variables, and their coordinates | New selector | Determining set in X afterwards |
|---|---|---|---|---|---|
| **F0** | (1.22) or (1.23) | nothing | all of 𝕋_b(X), as before | 1−χ^{(0)}, or χ^{(0)}(1−χ^{(1)}): functions of U_{b,Z}^{(0)}, U_{b,Z}^{(1)} | 𝔹_b |
| **F(n,1)** | 1−χ_b^{(n+1)} of (1.24) | 𝔰_h, …, 𝔰_{h+n−1} | everything else of 𝕋_b(X), original coordinates | function of U_{b,Z}^{(n+1)} | 𝔹_b^{(n)} |
| **F(n,2)** | 1−χ′_j of (1.27) | same | same; V_j in the Faddeev–Popov gauge-fixed representation ((1.5), (1.6) inserted) | function of V_j and V_Z^{(j)} | 𝔹_b^{(n)} |
| **F(n,3)** | the complement in (1.28) | same | same as F(n,2) | function of A_j | 𝔹_b^{(n)} |
| **F(n,4)** | 1−χ′^{(j)} of (1.55) | same | A_j original; the stage field in the **relocated free coordinate** B_j of (1.59); the rest original | (1.59): function of B_j alone | 𝔹_b^{(n)} with the datum V_j = 𝔳(B_j; M^j(U^{(n+1)})) (see §3.4) |
| **FΛ** | 1−χ_{b,Λ} of (1.75) | 𝔰_h, …, 𝔰_{b−1} | the deep factor χ_h𝕋_h(Z_h) and the raw fields on 𝔹″_b∩X | function of V_b↾Z∩Λ^c | 𝔹″_b |
| **F′** | 1−χ′ of (1.82) | 𝔰_h, …, 𝔰_{b−1} | deep factor; the old V_b↾Λ and the other V″ on 𝔹″_b∩Λ∩Z_h^c, in the tree-gauge coordinates V′ of (1.81); the **new** V_b↾Λ is a fresh variable with flat density (SF11) | function of B′ | 𝔹″_b |
| **F_P** | P ≠ ∅ in (1.88) | same | same as F′ | function of V_h near (Ω″_{h+1})^c | 𝔹″_b |

Survivors of all tests go on to LFR II and become first-class (everything integrated) or second-class (tags: all N stages integrated, the variables of (1.76) retained from birth, [Det] F5–F6).

*Proof.* The order of operations is SF2, SF3–SF5, SF10–SF12. A component leaves Z at its first failed decomposition and is "not changed by the subsequent operations" (SF2). The integrations 𝔰_i are performed stage by stage, each a partial evaluation of the integral operation 𝕋^{(i)}(Z_{i+1}) (SF3, SF7), and their logarithms ℂ^{(i)} remain boundary terms in stopped components (SF8). In F(n,2)–F(n,4) the gauge fixing has been inserted before the failing decomposition (SF3). In F(n,4) the stage variables have been re-expressed through B_j ((1.53)) and then relocated (SF5); the selector becomes (1.59). In F′, F_P the Λ-integration has been applied (SF10–SF11) and its variables are the operation's own integration variables (SF13: "integrals as in (1.76), but with some large field characteristic functions"). □ Hypotheses: source input for each formula used; **additional assumption** for exhaustiveness, because the source says it "will not attempt to give a systematic description of all possible cases" (SF4), and for F′, F_P because (1.82), (1.88) were read in in the source only.

**Corollary BK1 (selectors are frozen) (deduction; given BK and (Collar)).** At every T step k ≥ b the selectors of all eight forms are independent of the current coordinates z. *Proof.* Each is a function of internal variables of X and of the localized backgrounds U_{b,Z}^{(·)}, which depend on fields inside Z only (SF1, SF4). X ⊂ Z_k ⊂ Ω_{k+1}^c, so V_k↾X and all older fields in X are retained raw variables of the T step ([III] (3.15): the integration "∫dV_k↾_{Ω^c_{k+1}}" stays outside the fluctuation integral, source). In F(n,4) this holds only because the retained coordinate is the relocated one: in the unrelocated coordinate the selector χ′_j(1−χ′^{(j)}) depends on ℍ_Z^{(j)}, hence on the global background, hence on z. □

**Corollary BK2 (no tag is partially integrated) additional assumption.** The stages integrate only variables of scales ≥ h in Z_{i+1}∖Z″_{i+1}; older tags inside X were born at scales ≤ h (a second-class component is a new large-field region, LFR II p.378, so its creation breaks eligibility (ii) for N steps) and lie in the deep factor 𝕋_h(Z_h), which is "left unchanged" (SF11). So [Cons] premise R2 (Cons) is unaffected. The argument assumes Z_h ⊂ Z″_{h+1} on the geometry beyond (1.11).

### 3.3 The amendment to DN-1

DN-1 (2) reads: "A T step integrates exactly its current free coordinates. An R step integrates exactly the internal variables of its successful components, including every older operation they contain." By Prop. BK the second sentence is false for every component that enters the preparation and is not first-class. Proposed replacement:

> **(2′) Integrated data.** A T step integrates exactly its current free coordinates. An R step integrates (a) all internal variables of its first-class components, including every older operation they contain; conditional in every component that enters the preparation of LFR I §1, whatever its later fate, the variables 𝔰_i = (A_i↾Z_{i+1}∩Ω_{i+1}, V_i↾Ω^c_{i+1}∖Z″_{i+1}) of each **completed** preparatory stage (LFR I (1.25), (1.60)); (c) nothing else. **Coordinates.** Retained variables are carried in the coordinates in which the source leaves them: after a failed fluctuation test (LFR I (1.55)) the relocated coordinate of (1.59); after a T step the relocated exterior fluctuation of [III] (3.22); after (1.76) the tree-gauge coordinates of (1.81). A component stopped after the Λ-integration keeps the old V_b↾Λ as a retained internal variable; the new V_b↾Λ is a fresh variable.

Why the coordinate clause is part of the *law*: two coordinates related by a map that depends on the current field generate different σ-fields after that field is integrated ((1.59): the map is B_j^{old} = R_ℍ(B_j^{new}) with ℍ a function of the global background). ★ ("retained ⇔ not yet integrated by the main-line representation") selects the source's coordinate; Cor. BK1 shows that it is also the only one of the two for which [Cons] §1.1's sentence "the selectors of all retained operations do not depend on z" is true.

**Effect on proposition.** None at the level of ρ_k: "All the above transformations preserve the k-th density ρ_k" (SF10). For the path law, clause conditional only moves variables from "retained" to "integrated at the R step"; no proposition conditions on prefix-stage variables of a stopped component (H-03 and Annex BI concern successful components; C-02–C-04 are pointwise in the retained data). The cited estimate is taken as a hypothesis.  it is (d) to that extent.

### 3.4 Proposition LAW (where the current enters a stopped component)

Fix a T step k ≥ b and a stopped component X ⊂ Z_k. Write the T-step log-density of z at frozen 𝔣 as in [Cons] §1.1. Then:

1. *F0, F(n,1–3), FΛ, F′, F_P.* Every datum of the determining set inside X and every slot is frozen. The component contributes to the z-dependence only through (i) records of the global action whose carriers reach X, including the stage outputs ℂ^{(i)} with the bound (1.70) — these are S1a records; (ii) the Schur forms of its unintegrated ordinary operations — S4; (iii) for F(n,2–3), the Faddeev–Popov factors (1.5)–(1.6), which are functions of the frozen V_j. **S5 is empty in these forms.** deduction given BK.
2. *F(n,4).* On the stage bonds the datum of the determining set is not frozen. With Y := M^j(U^{[X]}) (the average of the global background built *without* the stage datum of X, i.e. U_k^{(n+1)} at birth), e^{iH} := Y V_Z^{−1} (SF5, (1.58)), γ the bump of SF6 and R_H(b) := (1/ig_j) log(e^{ig_jb}e^{−iγ(b)H}), the datum is
 V_j = 𝔳(B_j; Y) := exp i[g_jC R_H(B_j) − hD̃(g_jC R_H(B_j))]·Y,
 where B_j is the frozen relocated coordinate. On a free bond this is e^{ig_jB_j}e^{i(1−γ(B_j))H}V_Z: frozen where γ = 1, and equal to e^{ig_jB_j}Y — rigidly attached to the moving background — where γ = 0. In addition the density carries the factor exp Σ_u j(B_j(u); H_u), j(b;H) := log det D_bR_H(b). deduction from SF5–SF6, given the form (1.53) of the stage parametrization; the formula on free bonds is exact, on eliminated bonds it is the constraint solution (additional assumption, not written out by the source).
3. Consequently, with v^{ref} the stage data at the reference point z = 0,
 B̃_k = [the sectors of [Cons] §1.3 evaluated with stage data frozen at v^{ref}] + Θ^{J} + Θ^{A},
 Θ^{J}(z) := Σ_{X of form F(n,4)} Σ_{u} [j(B_j(u); H_u(z)) − j(B_j(u); H_u(0))], Θ^{A}(z) := Σ_ρ [F_ρ^{mov}(z) − F_ρ^{frz}(z)],
 where ρ runs over **all** records of the exponent (Wilson cells, E, R, B, S4, S6, tag densities, and the local gauge-fixing terms of the stage) and mov/frz means evaluated with stage data v(z), resp. v^{ref}. No logarithm of an integral over a retained variable occurs. deduction given items 1–2.

Θ^{J} + Θ^{A} is the sector S5. It is what the source calls "the usual new terms in the action" (SF5) and what [III] calls V^{(k)}(S_{k+1}, A_k, ℍ^{(k)}) for the relocation of a T step ("All terms of the previous action contribute to it", [III] p.269, (source)): the old relocation of a T step, seen from later steps, is the same object, and the source books it as B-terms. S5 is therefore **not** a new kind of sector; it is S1d at an old birth, inside a stopped component.

**Reading (MC) additional assumption.** When several components are in form F(n,4), The interpretation of the relocation field of X is defined through the background U^{[X]} that contains the (moving) stage data of the other components. The source defines ℍ_Z^{(j)} "in each component of Z separately" and does not discuss this. Lemma MD below shows that the reading is harmless: the mutual influence is a contraction.

## 4. The common tool: the current reconstruction as a holomorphic family

### 4.1 Setting and inputs

Fix the T step k → K = k+1, frozen data 𝔣, a real point ζ₀ of the support, and the polydisc D_r(ζ₀). Let 𝔅 be the determining set left by the last R step (it contains the prefix sets of Prop. BK inside stopped components), d := d_𝔅 the scaled distance [P2] (2.46) of 𝔅, E₀ the set of bonds of 𝔅 carrying current data, and 𝔛₄ the set of components of form F(n,4), with stage bonds S_X and stage scale j_X.

- **(H1) geometry.** 𝔅, and for each X ∈ 𝔛₄ the set 𝔅^{[X]} (stage datum of X removed, i.e. the (n+1)-structure in X), are of [V]-type and satisfy (Geo) of [The one-sided collar estimate] §6. Inside prepared regions the layers are one M-cube wide (SF14), so there (Geo) reads **(Geo-PF): ¼δ₀M > 2d log c₀(¼) + 1 and δ₀M ≥ 16 log L** — a condition on M alone (≈ δ₀M > 70.7 at δ₀ = 1), not on RM. The source uses the same mechanism: LFR I p.200 source: "exp(−δ(L^{−(k−m)}8MR_m + ⋯)) ≤ exp(−4δ(m−k₀)M) … can be made arbitrarily small for M large enough". Hypotheses: additional assumption for [V]-type (as (P9-ms) in [Native-tag admission, trajectory weights and the obstruction to propagation]); (Geo-PF) is a new parameter condition.
- **(H2) regular real base.** For real ζ₀ the configuration W₀ := U(𝔅, 𝔡(ζ₀)) is a real critical configuration in the class where (K♯), (Small) of [The one-sided collar estimate] hold. In prepared regions the source allows the enhancement L₀^{2N₀} ≤ L(L+1)R_b/N₀ (SF9, (1.24)); so (Small) there needs g_bℓ_b^{p₀}R_b small. Hypotheses: assumed input; additional assumption.
- **(H3)** [Source operators for the deformed reconstruction] P9♮ with (Conv-CR), [The one-sided collar estimate] Corollary HD and the main inequality of CT♯ at rate λ₁ := δ₀/4, and (Fr-Lip) of [Native-tag admission, trajectory weights and the obstruction to propagation] §2.1, for 𝔅 and each 𝔅^{[X]}. Hypotheses: conditional in those notes.
- **(H4) current data (E0).** The moving data on E₀ are V_k(ζ)(c) = exp i[g_kCA − hD̃(g_kCA)](c)·V^{(k)}source input, A = (a^{ext}, ζ), with a^{ext} the frozen exterior fluctuation and V^{(k)} frozen ([III] (3.15), source: "U_k(exp i[g_kCA_k − hD̃(g_kCA_k)]V^{(k)})"). The log-move B₀(ζ)(c) := (1/i)log(V_k(ζ)(c)V_k(ζ₀)(c)^{−1}) is holomorphic, |B₀| ≤ C_Cg_kr, and ∂_iB₀(c) = 0 unless d(source input; x_i) ≤ r_C, where |∂_iB₀(c)| ≤ C_Cg_k. Hypotheses: source input for block-locality of C ([P] p.428: "the operator C is almost local, a value (CB)(b) depends on B restricted to several blocks surrounding the bond b"); additional assumption for D̃.
- **(H5) stage map (St-loc).** 𝔳(b;Y) of Prop. LAW is holomorphic in Y near real admissible Y, real on real, block-local, and |log(𝔳(b;Y)𝔳(b;Y′)^{−1})source input| ≤ C_loc sup_{c′∈blk(c)}|log(Y(c′)Y′(c′)^{−1})|. Hypotheses: deduction on free bonds, where 𝔳 = e^{ig_jb}e^{i(1−γconditional)H}V_Z and H = (1/i)log(YV_Z^{−1}) (a Lipschitz function of Y with constant ≤ 2 for small arguments); additional assumption on eliminated bonds.
- **(H6) separation (Sep).** θ_sep := sup_X Σ_{X′≠X} e^{−(δ₀/8)d(X,X′)} ≤ 1/(2C_*), with C_* := C_locC_M(1+C_a)K_CTe^{λ₁c_blk}. Hypotheses: holds below a coupling ceiling, because distinct components of the large-field region are at distance ≥ MR_bh_b ((c\*) [Retained sigma-fields and conditional expectations] §4.1) and their number within distance t grows polynomially.
- **(H7) averages (Av-Lip).** For a block bond c of scale j: |log(M^j((e^{iη𝓗}W)^{u})(c)M^j(W)(c)^{−1})| ≤ C_M sup_{blk(c)}[h_j|𝓗| + h_j²|∇𝓗| + |u−1|] for small arguments. Hypotheses: (d) (the standard property of the averaging maps; assumed).
- **(Ceil)** 4C_*C_Cg_kr ≤ min(r₉, r_CT).

Put λ := δ₀/8 and K₁ := K_CTC_C(1+2C_*).

### 4.2 Lemma MD (moving stage data) conditional

Under (H1)–(H7), (Ceil): for every real ζ₀ there is a unique family v(ζ) = (v_X(ζ))_{X∈𝔛₄}, holomorphic on D_r(ζ₀), with v_X(ζ) = 𝔳_X(b_X; M^{j_X}(U(𝔅^{[X]}, 𝔡₀(ζ), v_{X′≠X}(ζ)))) and v(ζ₀) the actual stage data. Its log-move β_X(ζ) := (1/i)log(v_X(ζ)v_X(ζ₀)^{−1}) satisfies, for every stage bond c and every i,
 |β(ζ)source input| ≤ 2C_*C_Cg_kr e^{−λd(source input; E₀)}, |∂_iβ(ζ)source input| ≤ 2C_*C_Cg_k e^{λr_C}e^{−λd(source input; x_i)}.
On the real slice v(ζ) is the actual stage data.

*Proof.* Let ‖β‖_w := sup_c e^{w(c)}|β(c)| with w := λd(·,E₀). For given β in the ball ‖β‖_w ≤ 2C_*C_Cg_kr define Φ_X(β) as the log-move of the right-hand side. For the set 𝔅^{[X]} at its real critical base (H2), the data move is (B₀(ζ), β_{X′}, X′ ≠ X); by (Ceil) it is < r_CT. By (H3) the reconstruction is (e^{iη𝓗^{[X]}}W₀^{[X]})^{ũ}, 𝓗^{[X]} holomorphic in the data. Apply the main inequality of CT♯ along the segment from 0 to the datum (𝓗(0) = 0), separately to each part of the datum: for the part B₀ with the weight w; for the part β_{X′} with the weight w̃ := w + (λ₁−λ)d(·,X′), which is λ₁-Lipschitz and equals w on X′. This gives, at a block y,
 e^{w(y)}[h|𝓗^{[X]}| + h²|∇𝓗^{[X]}|](y) ≤ K_CT[C_Cg_kr + Σ_{X′≠X}e^{−(λ₁−λ)d(y,X′)}‖β_{X′}‖_w].
By (Fr-Lip), (H7), (H5) and the definition of C_* (the factor e^{λ₁c_blk} pays the weight over one block),
 ‖Φ_X(β)‖_w ≤ C_*[C_Cg_kr + θ_sep‖β‖_w] ≤ 2C_*C_Cg_kr, ‖Φ(β) − Φ(β′)‖_w ≤ C_*θ_sep‖β − β′‖_w ≤ ½‖β − β′‖_w,
the Lipschitz bound by the same inequality applied to the difference of two data (CT♯ is a bound on the derivative at every base point). So Φ is a contraction of the ball; the Picard iterates starting from β = 0 are holomorphic in ζ and converge uniformly, so the fixed point is holomorphic. For real ζ every object is real and the actual stage data satisfy the equation by Prop. LAW item 2 and reading (MC); they lie in the ball because the real-slice move obeys the same a priori bound (continuity argument along the segment from ζ₀). The derivative bound follows by differentiating the fixed-point equation and repeating the estimate with the weight λd(·,x_i), using ∂_iB₀(c) = 0 for d(source input; x_i) > r_C. □

The least checked step is the multi-component coupling; for a single F(n,4) component the lemma is one application of HD.

### 4.3 Theorem CR conditional

Assume (H1)–(H7), (Ceil). Let B(ζ) := (B₀(ζ), β(ζ)) be the total data move on 𝔅 relative to ζ₀, and 𝓗(ζ) := 𝓗_{W₀}(B(ζ)), ũ(ζ) the response and frame map of P9♮ at the base W₀. Then on D_r(ζ₀):

- **(CR1)** 𝓗, ũ are holomorphic, real on real ζ, 𝓗(ζ₀) = 0, ũ(ζ₀) = 1, and for real ζ the current background is U(𝔅,𝔡(ζ)) = (e^{iη𝓗(ζ)}W₀)^{ũ(ζ)}.
- **(CR2)** For every block y of layer n: [h_n|𝓗| + h_n²|∇𝓗| + h_n³|D*D𝓗|](y) ≤ K₁g_kr e^{−λd(y,E₀)}, and |log ũ(ζ)(x)| ≤ C_aK₁e^{λc_blk}g_kr e^{−λd(x,E₀)}.
- **(CR3)** [h_n|∂_i𝓗| + h_n²|∇∂_i𝓗| + h_n³|D*D∂_i𝓗|](y) ≤ K₁e^{λr_C}g_k e^{−λd(y,x_i)}, and |∂_i log ũ(ζ)(x)| ≤ C_aK₁e^{λ(r_C+c_blk)}g_k e^{−λd(x,x_i)}.
- **(CR4) collar ratio.** Suppose the layerwise reserve satisfies ρ(n) ≥ (β/8)α_{∧,n}, α_{∧,n} ≥ α_{∧,k}/(C_AF√(1+k−n)), and g_kr ≤ c_rα_{∧,k} ((Res-pat), AF and the radius premise G5 of [Cons]; additional assumption). For a set 𝒪 of old sites with d(y,E₀) ≥ max(D_𝒪, k−n(y)−1), put ε_𝒪 := C₅e^{−λD_𝒪/2}, C₅ := (8/β)C_AFc_r(1+C_a)K₁e^{λc_blk}·sup_m√(1+m)e^{−λ(m−1)/2}. Then the matched norms of 𝓗(ζ) and of log ũ(ζ) at y ∈ 𝒪 are ≤ ε_𝒪ρ(n(y)). For 𝒪 = Z_k one has D_𝒪 = D_k − 2, D_k = 8LR_{k+1} ((Collar), (c\*) [Deep retained tags and boundary rotations] §2.1).

*Proof.* (CR1): P9♮ item 1 and minimal-orbit uniqueness, exactly as in [Native-tag admission, trajectory weights and the obstruction to propagation] Theorem H′ step (i), with the data B(ζ) holomorphic by (H4) and Lemma MD and |B|_∞ < min(r₉,r_CT) by (Ceil). (CR2): the weighted main inequality of CT♯ integrated along the segment, with weight λd(·,E₀): ‖B‖_w ≤ C_Cg_kr(1+2C_*) by Lemma MD; then (Fr-Lip). (CR3): the same inequality applied to the datum ∂_iB with weight λd(·,x_i). (CR4): arithmetic, as in [Native-tag admission, trajectory weights and the obstruction to propagation] Theorem H′ step (ii), using max(deduction; a′) ≥ (a+a′)/2. □

**What is new relative to [Native-tag admission, trajectory weights and the obstruction to propagation].** [Native-tag admission, trajectory weights and the obstruction to propagation] §2.5 item 4(i) already used "HD for the current-step set B_k" to control the data map of a tag. Theorem CR states that step as a theorem in its own right, in weighted form, for the determining set actually left by the R step (prefix sets included), and with moving stage data. With 𝔛₄ = ∅ it is a restatement.

### 4.4 Lemma A-cur (admission of records of the current background) conditional

Let ρ be a record of the form F_ρ(ζ;a) = 𝔈_ρ(U(𝔅,𝔡(ζ)); a) with carrier X_ρ and frozen real slots a at sites Σ_ρ ⊂ X_ρ, such that: **(Cov)** 𝔈_ρ(W^g; g·a) = 𝔈_ρ(W;a) for real gauges; **(Dom)** 𝔈_ρ(·;a) is holomorphic and bounded by w_ρ (after subtraction of a constant) on the native ball of layerwise radius 2ρ(n) about every real admitted W₀↾X_ρ, uniformly in a; **(HSA)** there is 𝔊_a(W,l), holomorphic for W in the ball of radius ρ(n) and |l(x)| < ϱ(x), bounded by w_ρ, with 𝔊_a(W,l) = 𝔈_ρ(W; e^{l}·a) at real arguments. Assume Theorem CR and **(Res)**: the reserves ρ̂(x) := min(ρ(n(x)), ϱ(x)) satisfy ρ̂(x) ≥ ĉα_{∧,n(x)} for x ∈ X_ρ (ĉ = β/8 without slots; ĉ = c_Iβ/(8Λ₀²) for ordinary slots, by [Deep retained tags and boundary rotations] Lemma I and Cor. 5.1(i)), α_{∧,n} ≥ α_{∧,k}/(C_AF√(1+k−n)), g_kr ≤ c_rα_{∧,k}, and C₆ := (1/ĉ)C_AFc_r(1+C_a)K₁e^{λc_blk}sup_m√(1+m)e^{−λ(m−1)/2} ≤ ½. Then

1. F_ρ(·;a) extends holomorphically to 𝒮_r, with |F_ρ − const| ≤ w_ρ there;
2. sup_a|∂_iF_ρ(ζ;a)| ≤ (w_ρ/r)C_Ae^{−(λ/2)d(x_i,X_ρ)} on D_{r/2}(ζ₀), C_A := 4C₆e^{λr_C};
3. the constants depend on none of: the volume, k, the history, the number, sizes, ages, forms or positions of components, the frozen data.

*Proof.* [Native-tag admission, trajectory weights and the obstruction to propagation] Theorem H′ steps (i)–(iii) with 𝒰 := U(𝔅,·): F_ext(ζ) := 𝔊_a(e^{iη𝓗(ζ)}W₀, −log ũ(ζ)) is holomorphic by (CR1), lies in the domain by (CR4), equals F on the real slice by (Cov) and (CR1). For the derivative, ∂_iF_ext = D_W𝔊·∂_iW^L + D_l𝔊·∂_il; Cauchy in each factor with radius ρ̂(x)/2 (the point lies within ρ̂/2 of the base by (CR2), (Res)) and (CR3) give ≤ 2w_ρ max_x[(1+C_a)K₁e^{λ(r_C+c_blk)}g_ke^{−λd(x,x_i)}/(ρ̂(x)/2)], and g_k/ρ̂(x) ≤ (1/r)(1/ĉ)C_AFc_r√(1+k−n(x)); d(x,x_i) ≥ max(d(x_i,X_ρ), k−n(x)−1) for x ∈ X_ρ ((c\*) [Multiscale incidence and logarithmic jets] T3 via [Deep retained tags and boundary rotations] Cor. 5.1) absorbs the square root in half of the exponent. Gluing over ζ₀ is [Deep retained tags and boundary rotations] Lemma 2.2. □

To pass to the metrics of Theorem C one needs **(Met)**: d_𝔅 ≥ c_metd_g − c′ on the sites considered ([Boundary estimate b] Lemma G1, assumed input; (d) inside prepared regions), and d_g ≥ d^{(b)}. Then (Loc★) holds at rate ν := c_metλ/2.

### 4.5 Lemma Δ (difference records)

Let 𝔊 be holomorphic and bounded by w on the ball of radius 2ρ (in a norm ‖·‖) about a point p₀. Let p₁(ζ), p₂(ζ) be holomorphic with ‖p_a(ζ) − p₀‖ ≤ ρ/2, ‖p₁ − p₂‖ ≤ ερ, ‖∂_ip_a‖ ≤ (ρ/r)τ_i, ‖∂_i(p₁−p₂)‖ ≤ (ρ/r)ετ_i. Then G := 𝔊∘p₁ − 𝔊∘p₂ satisfies |G| ≤ εw and |∂_iG| ≤ 3ε(w/r)τ_i.

*Proof.* ∂_iG = D𝔊(p₁)[∂_i(p₁−p₂)] + (D𝔊(p₁) − D𝔊(p₂))[∂_ip₂]. Every point q of the segment [p₂,p₁] is within ρ/2 of p₀, so the ball of radius 3ρ/2 about q lies in the domain; Cauchy gives ‖D𝔊(q)‖ ≤ w/ρ and ‖D²𝔊(q)‖ ≤ 2w/ρ². So |∂_iG| ≤ (w/ρ)(ρ/r)ετ_i + (2w/ρ²)(ερ)(ρ/r)τ_i = 3ε(w/r)τ_i. The value bound is the mean-value inequality. □

## 5. S5, part 2: the per-record inputs

### 5.1 Proposition J (the Jacobian records; PF.12–15 and PF.3) 

**(J-a) Single-bond estimates.** Let Ψ(X,Y) := (1/i)log(e^{iX}e^{iY}) on 𝔤^c×𝔤^c, analytic for |X|,|Y| ≤ ¼, with Ψ(X,0) = X. Let γ be a C^∞ function of the invariant |X|² = tr X² with γ = 0 for |X| ≤ (4/3)δ′, γ = 1 for |X| ≥ (5/3)δ′, |Dγ| ≤ C_γ/δ′ (as a function of X = g b). For real b with |gb| ≤ 6δ′ ≤ ¼ and complex H with |H| ≤ 2c₀δ′ (c₀ ≤ 1/(16C_Ψ(1+C_γ)), δ′ ≤ 1) put R_H(b) := g^{−1}Ψ(gb, −γ(gb)H). Then
 ‖D_bR_H(b) − 1‖ ≤ C_Ψ(1+C_γ)|H|/δ′ ≤ ¼, j(b;H) := log det D_bR_H(b) is holomorphic in H, |j| ≤ 2 dim𝔤·C_Ψ(1+C_γ)|H|/δ′, and for |H| ≤ c₀δ′: |D_Hj[v]| ≤ C_j|v|/δ′, C_j := 4 dim𝔤·C_Ψ(1+C_γ).
*Proof.* D_bR_H = D_XΨ(gb,Y) + D_YΨ(gb,Y)·(−H ⊗ g^{−1}D_b[γ(gb)]), Y = −γH. By Cauchy on the bidisc, ‖D_XΨ(X,Y) − 1‖ ≤ C_Ψ|Y| (it vanishes at Y = 0) and ‖D_YΨ‖ ≤ C_Ψ; and |g^{−1}D_b[γ(gb)]| ≤ C_γ/δ′. For fixed real b, γ(gb) and its derivative are numbers, so D_bR_H is an analytic function of H; the logarithm of the determinant converges because ‖D_bR_H − 1‖ ≤ ¼ (|Tr log(1+E)| ≤ 2 dim𝔤‖E‖ for ‖E‖ ≤ ½), and |D_Hj| follows by Cauchy from the ball |H| ≤ 2c₀δ′ to the ball |H| ≤ c₀δ′. □ These are (PF.12), (PF.14), (PF.15). : on SU(2) the three ratios are ≈ 6.0, 5.7, 5.5 for δ′ ≤ 0.1 (and the estimates fail for δ′ of order 1, where |gb| leaves the principal branch — the hypothesis 6δ′ ≤ ¼ is needed).

**(J-b) The record conditional.** For X ∈ 𝔛₄ and a stage bond u, H_u(ζ) := (1/i)log(Y_u(ζ)V_{Z,u}^{−1}) with Y(ζ) := M^{j}(U(𝔅^{[X]},·)) along the family of Lemma MD. Assume **(H-real)**: |H_u| ≤ ½c₀δ′_j at every real point of the support, at every step k ≥ b. Then F_{J,u}(ζ) := j(B_j(u); H_u(ζ)) − j(B_j(u); H_u(0)) is holomorphic on 𝒮_r and
 sup_𝔣|∂_iF_{J,u}(ζ)| ≤ (w^J_u/r) e^{−λd(u,x_i)}, w^J_u := r·C_jC_M(1+C_a)K₁e^{λ(r_C+c_blk)}·g_k/δ′_j,
provided C_M(1+C_a)K₁e^{λc_blk}g_kr e^{−λ(D_k−2)} ≤ ½c₀δ′_j (a ceiling).
*Proof.* By (H7), (Fr-Lip) and Theorem CR applied to 𝔅^{[X]}, |H_u(ζ) − H_u(ζ₀)| ≤ C_M(1+C_a)K₁e^{λc_blk}g_kr e^{−λd(u,E₀)} and |∂_iH_u| ≤ C_M(1+C_a)K₁e^{λ(r_C+c_blk)}g_k e^{−λd(u,x_i)}; with (H-real) and the ceiling, |H_u(ζ)| ≤ c₀δ′_j; compose with (J-a). □

**Status of (H-real).** At the birth step it is the source's (1.57)–(1.58), source: "bounded by O(1)exp(−R_j)ε_j. This bound is very small, smaller than any positive power of g_j". At later steps the global background has changed; the same bound follows from CT♯ item 3 for the localized set 𝔹^{(n+1)}(Z) (the two minimisers have the same data inside Z and differ by a boundary datum of size O(ε) on the 2M₁-collar, at distance ≥ 10M(R_{j+1}+⋯+R_{b−1}) + MR_b from the stage bonds, (1.57)). This remains an assumption: **conditional; additional assumption**.

**Format for Theorem C.** Birth j (the stage scale), carrier the one 𝒢_j-cube containing u, anchor that cube (it lies in the grade-j layer (Ω^c_{j+1}∖Z″_j)^{(j)} of 𝔅^{(n)}, (1.16), source), weight w^J_u, rooted norm W_j^{J} ≤ dM^d dim𝔤·w^J. Since g_k/δ′_j = g_k/(g_jA₁p₁(g_j)) ≤ C_AF√(1+k−j)/(A₁p₁(g_j)), W_j^J ≤ C r√(1+k−j)/p₁(g_j); the square root is absorbed by Γ_j ([Hidden components] Rem. 4.4(3)). The anchors lie in Z_k, so [Retained sigma-fields and conditional expectations] Cor. C-col gives the collar factor. The count C(MR_b)⁴L^{4(b−t)} of (PF.16) is not paid by hand: it is the anchor sum of Theorem C, paid by (Geo) — which must be read with the thin prepared layers ([Hidden components] Rem. 4.4(2): at most N₀ of them, cost e^{C₀} ≤ L^{dN₀}e^{γN₀}, polynomial in R_b).

The smallness of H is **not** used for the bound; the finite-cutoff construction factor e^{−c_JR_b} of (PF.17) is replaced by the collar factor of the current step, which is what the completion test asks for.

### 5.2 Proposition AD (the action difference; PF.19–22) conditional

Let ρ be any record of the exponent that satisfies the hypotheses of Lemma A-cur (or, for slot-free explicit records, the direct estimates of §§6–7), with weight w_ρ and rate λ/2. Let F_ρ^{mov}, F_ρ^{frz} be its values with stage data v(ζ), resp. v^{ref} = v(0). Then G_ρ := F_ρ^{mov} − F_ρ^{frz} is holomorphic on 𝒮_r and
 sup_𝔣|∂_iG_ρ| ≤ 3ε_PF (w_ρ/r) C_A e^{−(λ/4)d(x_i,X_ρ)}, ε_PF := C_Δ(1+P_k/r) e^{−λ(D_k−2)/4},
uniformly in the frozen data, the number and forms of stopped components and the volume.

*Proof.* Take the base W₀^{frz} := U(𝔅, 𝔡₀(ζ₀), v^{ref}). Relative to it the frz family has data move (B₀(ζ), 0) and the mov family (B₀(ζ), β^{ref}(ζ)), β^{ref} := log(v(ζ)(v^{ref})^{−1}) = β(ζ) + β(ζ₀ ← 0). By Lemma MD along the real segment from 0 to ζ₀ (|z_{0,i}| ≤ P_k) and [Deep retained tags and boundary rotations] (Sites), |β^{ref}source input| ≤ 2C_*C_CC_Σg_k(r+P_k)e^{−(λ/2)d(source input; E₀)}. *Values.* By the main inequality of CT♯ integrated along the segment in the β-direction, the two responses differ at a block y by ≤ K_CT sup_c e^{−λ₁d(y,c)}|β^{ref}source input| in matched units, the sup over stage bonds c. Since λ₁ ≥ λ/2, d(y,c) + d(source input; E₀) ≥ d(y,E₀) and d(source input; E₀) ≥ D_k − 2 for c ∈ Z_k, this is ≤ 2K_CTC_*C_CC_Σg_k(r+P_k)e^{−(λ/2)max(D_k−2, d(y,E₀))} — small at **every** y, near the current support as well as inside Z_k. Dividing by the reserve at layer n(y) and using d(y,E₀) ≥ k−n(y)−1 as in (CR4), the difference is ≤ ε_PFρ̂(y) with C_Δ := (2/ĉ)C_AFc_rK_CTC_*C_CC_Σ(1+C_a)e^{λc_blk}sup_m√(1+m)e^{−(λ/4)(m−1)}. *Derivatives.* ∂_i(𝓗^{mov} − 𝓗^{frz}) = D𝓗(B₀,β^{ref})[(0,∂_iβ)] + (D𝓗(B₀,β^{ref}) − D𝓗(B₀,0))[(∂_iB₀,0)]. First term: the datum ∂_iβ lives on stage bonds, where |∂_iβ(c)| ≤ 2C_*C_Ce^{λr_C}g_ke^{−λd(source input; x_i)} (Lemma MD); the weighted inequality with weight λd(·,x_i) gives ≤ Cg_ke^{−λd(y,x_i)}, and the unweighted one with d(source input; x_i) ≥ D_k − 2 gives ≤ Cg_ke^{−λ(D_k−2)}; take the geometric mean. Second term: it is ∫₀¹D²𝓗(B₀,tβ^{ref})[(∂_iB₀,0),(0,β^{ref})]dt; Cauchy in the β-direction on the radius r_CT/2 gives ≤ (2|β^{ref}|_∞/r_CT)·sup|D𝓗[(∂_iB₀,0)]| ≤ (2|β^{ref}|_∞/r_CT)K_CTC_Ce^{λr_C}g_ke^{−λd(y,x_i)}, and |β^{ref}|_∞ ≤ 2C_*C_CC_Σg_k(r+P_k)e^{−(λ/2)(D_k−2)}. Both terms are ≤ ε_PF·K₁e^{λr_C}g_ke^{−(λ/2)d(y,x_i)} in matched units (after enlarging C_Δ by a factor depending on r_CT). The frame maps are treated the same way by (Fr-Lip). Now apply Lemma Δ to 𝔊_a with p₁, p₂ the pairs (W^L, −log ũ) of the two families and τ_i = C_Ae^{−(λ/4)d(x_i,X_ρ)}. □

**Consequences.**
1. Θ^{A} = Σ_ρG_ρ is summed by the *same* summation theorems as the records ρ themselves, record class by record class, with every weight multiplied by 3ε_PF and the rate halved. No hole format, no carrier of its own, no (Col_b) for the failed component.
2. Its budget is ε_PF·𝔖_k^{abs}, where 𝔖_k^{abs} := Σ_bΓ_b[W_b^{Wil} + W_b^{E} + W_b^{R} + W_b^{S1} + W_b^{S4} + W_b^{S6} + m₁s_{*,b}] is the **absolute** budget of all records — including the bulk Wilson cells and the E- and R-records, which C-05 otherwise does not sum. **(Abs)**: these absolute budgets are finite and polynomial in ℓ_k: for Wilson cells by Lemma P of §7 at g_k^{−2} in place of the coefficient difference (W_b^{Wil} ≤ CM⁴(ε_b/g_b + r)r, conditional); for E, R by the absolute layerwise majorants of C-02/C-03 in record format ([Cons] V4 cites them as (E14.51), (RM.13); assumption/(d) — assumed here). Then ε_PF𝔖^{abs}/r² → 0 because R_k ≥ ℓ_k^r with r > 1.
3. The local terms of the stage that depend on the stage data explicitly (the Faddeev–Popov factors (1.6), −g_j^{−2}[1 − Re tr V_j(y,x)]) are local holomorphic functions of v(ζ); their difference records have |∂_i| ≤ Cg_j^{−2}ε_j|∂_iβ| ≤ C(ε_j/g_j)(g_k/g_j)e^{−λd(source input; x_i)} by the trace cancellation of Lemma P and (1.5), i.e. weight ≤ CrP_j√(1+k−j) per site, summed as in §5.1. conditional

**What Prop. AD needs that is not proved.**
- **(Dom-PF)** source assumption: that the records crossing or lying in a stopped component (old E, R, B and the stage outputs ℂ^{(i)}) are holomorphic on native balls about the *actual* real backgrounds there, with reserve — i.e. the spaces Ũ_k^{(n)c}(X,α̃₀,α̃₁) of LFR I (1.64)–(1.69), their descending property, and the insertion statement the source declines to prove (SF8: "we will not repeat it"). This is PF.1's content. PF.1 verified the multipliers L₀^{2a} of (1.64)–(1.69); The argument assumes it, and the insertion statement itself is a source assertion. With (Dom-PF), the parameter choice q₀, q₁ > p₀ + r + 2 of (PF.3) is what makes the L₀^{2N₀} ≤ CR_b enhancement fit inside the reserve; it must be on the parameter construction.
- **(St-loc)** on eliminated bonds, **(MC)**, **(H-real)** at later steps, **(Abs)** for E and R.

Proved: the law (Prop. BK, Prop. LAW; source input; deduction, exhaustiveness additional assumption); S5-J per record (deduction; conditional); S5-A per record (conditional on the inputs just listed). Not proved: (Dom-PF); the readings; and — outside this note — the same statements under repeated R steps (a component stopped at b, stopped again at b′ > b: the forms compose, Theorem CR and Lemma MD are insensitive to it, but the composed map requires a separate bound).

## 6. S4: the ordinary older Schur response

### 6.1 The object

For an unreplaced operation 𝕋^{(j)}(Z_{j+1}∩X) the kernel contains ([III] p.258, source): "exp[−½⟨A_j, C*Δ^{(j)}CA_j⟩ + ½⟨A_j, C*Δ^{(j)}CC^{(j)}(Λ_{j+1})C*Δ^{(j)}CA_j⟩] (2.21). More precisely, the quadratic form in the exponential couples only the fields A_j in the same component of Z_{j+1}∩Ω_{j+1}. The other terms of this quadratic form are included into the effective action into 𝔹-terms." Write it as −½Σ_{r,s}a_r^{T}S_j(r,s;U)a_s, the sum over pairs of bonds of the scale-j lattice in one component of Z_{j+1}∩Ω_{j+1}, U the fine background. In the stopped forms the same kernel appears as C*Δ^{(j)}_{Λ_{j+1}}C in (1.25). The retained fields obey |a_r| ≤ C_aP_j: [III] p.267 source: "This implies that |V′_k − 1| < O(1)ε_k on Ω_{k+1} … We define A′_k = (1/i)log V′_k, hence |A′_k| < O(1)ε_k also", then A′ = g_kA, so |A_k| ≤ O(1)ε_k/g_k = O(1)(A₀/A₁)P_k; the relocation changes this by less than δ_k/g_k.

S_j is a fixed function of the fine configuration: the same formula is evaluated at U = U(𝔅,𝔡(ζ)) at every later step (this is erratum AX part 1; the source does not display it, gap (G-T) of §8).

### 6.2 The named input

> **(OR-K).** There are constants B_S, δ_S > 0 and layerwise radii ρ_S(n) ≥ (β/8)α_{∧,n} such that for every j, every admitted history and every real admitted background W₀: S_j(r,s;·) is holomorphic on the native ball of radius 2ρ_S about W₀ (complex perturbations e^{iηA′}W₀, measured in the matched norms h_n|A′| + h_n²|∇A′| on layer n), |S_j(r,s;W)| ≤ B_Se^{−δ_Sd_j(r,s)} there, and for every direction δW
> |D_WS_j(r,s;W)[δW]| ≤ B_S sup_x e^{−δ_S(d_j(r,x)+d_j(x,s))}‖δW(x)‖_{nat}/ρ_S(n(x)),
> where d_j is the distance in units of the scale-j lattice.

Status. For real backgrounds the ingredients are printed: [P] (3.156)–(3.158) (source): "(C*Δ_kC)^{−1} = C^{(k)}(Λ)", "a positive definite operator C*Δ_kC with a lower bound γ₀ > 0 independent of k and U"; Theorem 3.15 (source): "the propagator C^{(k)}(Λ) is given by the formula (3.185), and satisfies the bound |C^{(k)}(Λ;y,y′)| ≤ B₀e^{−δ₀|y−y′|} … This propagator has a convergent random walk expansion of the type described previously"; Theorems 3.9, 3.10 (source): "A term in this expansion, corresponding to a walk ω, depends on configuration U restricted to X₀⁵∪X₁⁵∪…∪X_n⁵". The response bound in (OR-K) is the statement that summing the walk expansion with one vertex differentiated loses nothing but constants; it is the same kind of statement as (K♯) of [The one-sided collar estimate] and should follow from the same package. **This remains an input**, and the uniformity on complex balls for the multiscale geometry {Ω_j} is a reading (additional assumption); the conditional boundary estimates item 1 called the walk expansions "substantial input beyond an entrywise covariance bound" and did not check complex uniformity either. So (OR-K) is **source assumption**: source input; additional assumption. the finite-cutoff construction walk-indexed records (OR17.9) are not needed: Theorem C does not require connected carriers, so the pair (r,s) can be the record.

> **(Cov-OR) additional assumption.** S_j(r,s;W^g) = Ad_{g(r₋)}S_j(r,s;W)Ad_{g(s₋)}^{−1} for real gauges g. (Built from covariant objects; [U17] AS §4.1 argues it from uniqueness of the constraint solution C_j. [III] p.261 (iii) states the corresponding invariance for B-terms, assumed input.)

### 6.3 Proposition OR conditional

Assume Theorem CR, (OR-K), (Cov-OR), (Met), and (Res) of Lemma A-cur with ρ = ρ_S and ϱ = ∞. For a pair (r,s) of an operation of scale j put
 F_{r,s}(ζ;a) := −½⟨Ad_{ũ(ζ)^{−1}(r₋)}a_r, S_j(r,s; e^{iη𝓗(ζ)}W₀) Ad_{ũ(ζ)^{−1}(s₋)}a_s⟩.
Then F_{r,s} is holomorphic on 𝒮_r, equals the actual term of the exponent on the real slice, and
 sup_{|a|≤C_aP_j}|∂_iF_{r,s}(ζ;a)| ≤ (w_{r,s}/r)e^{−ν d^{(j)}(x_i,{r,s})}, w_{r,s} := C_{OR}P_j²e^{−(δ_S/2)d_j(r,s)}, ν := min(c_metλ/2, δ_SM/2),
with C_{OR} = 4C_a²B_S(C_A + 1). In the format of [Hidden components] Theorem C: birth b = j+1 (Remark 1); cubes E_ρ = the two 𝒢_{j+1}-cubes containing r and s; anchor the cube of r; δ_{j+1}(E_ρ) ≤ d_j(r,s)/(LM) + 2√d; since d^{(j+1)} ≤ d^{(j)} the locality bound holds a fortiori in the capped metric of the birth; rooted norm
 W_{j+1}^{S4} := sup_q Σ_{r∈q}Σ_s w_{r,s}e^{θδ_{j+1}} ≤ C(additional assumption; L,M,δ_S,θ)C_{OR}P_j² for θ < δ_SLM/2.
All constants are independent of the volume, k, the history, the frozen data and the walk structure.

*Proof.* Real slice: (CR1) and (Cov-OR). Holomorphy: 𝓗, ũ are holomorphic (CR1); e^{iη𝓗(ζ)}W₀ lies in the ρ_S-ball by (CR4) (collar) or (Res) (elsewhere); Ad_{ũ^{−1}} is entire in log ũ and |Ad_{ũ^{−1}}| ≤ e^{2|log ũ|} ≤ 2. Derivative: three terms. (i) D_WS[∂_iW^L]: by (OR-K) and (CR3), ≤ B_S sup_x e^{−δ_S(d_j(r,x)+d_j(x,s))}K₁e^{λr_C}g_ke^{−λd(x,x_i)}/ρ_S(n(x)). Split δ_S in halves; d_j(r,x)+d_j(x,s) ≥ d_j(r,s); d_j ≥ M d^{(j)} (the capped unit is ≥ Mh_j); (Met); and the reserve arithmetic of Lemma A-cur. This gives ≤ (1/r)B_SC_Ae^{−(δ_S/2)d_j(r,s)}e^{−ν d^{(j)}(x_i,{r,s})}. (ii), (iii) the two rotation terms: |∂_iAd_{ũ^{−1}(r₋)}| ≤ 2|∂_i log ũ(r₋)| ≤ (2/r)·(C_aK₁e^{λ(r_C+c_blk)}g_kr)e^{−λd(r₋,x_i)}, and g_kr is ≤ 1. Multiply by |a_r||a_s| ≤ C_a²P_j² and by 4. Rooted norm: the sum over s of e^{−(δ_S/2−θ/M)d_j(r,s)} over bonds of the scale-j lattice converges; q contains dM^d bonds. □

**Remarks.**
1. *Anchor.* Theorem C wants an anchor cube meeting closure{g ≤ b}. The fields A_j live in Z_{j+1}∩Ω_{j+1} = Ω_{j+1}∩Λ_{j+1}^c, which is in the layer of grade j+1 of the later history. So the records are declared with birth b = j+1 on the grid 𝒢_{j+1}; this costs a factor L^d in the number of bonds per anchor cube and nothing else. deduction for the bookkeeping, additional assumption for the grade.
2. *Collar.* All anchors lie in Z_k, so [Retained sigma-fields and conditional expectations] Cor. C-col applies: the S4 entry of the budget is e^{−νD_k/(8Θ′)}Σ_bΓ_bW_b^{S4}, finite and → 0 under (Traj-w) ([Native-tag admission, trajectory weights and the obstruction to propagation] §3) because W_b^{S4} ∝ P_{b−1}².
3. *Uniformity in frozen data.* The sup over a uses only the selector bound |a| ≤ C_aP_j; the background enters through W₀, any real admitted one.
4. *Stopped forms.* In forms F(n,1–4) the unintegrated Schur forms of the stage and of the deeper operations are of this type, on the prefix determining set; (OR-K) must then hold for the prefix geometry (thin layers: (Geo-PF)). In F(n,4), additionally, the form −½⟨B_j, C*Δ^{(j)}CB_j⟩ of (1.60) is part of the Wilson action evaluated at moving data, not a kernel factor; it is in Θ^A.
5. *What replaced what.* AD17.3 (nodal interpolation at the two old slots) → the explicit Ad-rotation, entire in the frame map; (OR17.10) → (OR-K); "L^{4a} old-root count with Γ > 4log L + log 2 + 2" → Theorem C with (Geo); the factor e^{−c_GMR_k} of (OR17.11) → Cor. C-col.

## 7. S6: the heterogeneous Wilson coefficient

### 7.1 The object and the recursion

[III] (2.24) (source): 1/g_j²(x) = 1/g_{j−1}²(x) ∓ β_j(g_{j−1})φ_j(x) with "φ_j ∈ C₀^∞(Λ_j), φ_j = 1 on Λ_j^{∼−1}. Thus g_j(x) = g_j on the last domain." With w_l := g_l^{−2}, the homogeneous recursion is the same with φ ≡ 1, so
After an R step the coefficient is reset to g_k^{−2} on the replaced region ((c\*) LFR II p.365, re-read in [Native-tag admission, trajectory weights and the obstruction to propagation] §5); this only removes support. The term of the exponent is F^{het}(z) = −Σ_pΔw(x(p))[s_p(U(z)) − s_p(U(0))], s_p(U) = 1 − Re tr U(∂p), sum over fine plaquettes ([III] (3.15), source: "A(1/g_k²(·) − 1/g_k², U_k(exp i[g_kCA_k − hD̃(g_kCA_k)]V^{(k)})) − A(1/g_k²(·) − 1/g_k², U_{k+1})"; the source treats it as a boundary term with the parameter t, [III] p.271, (source)).

**Size.** Π_n := sup{|Δw(x)| : x of grade n}. Two bounds: (i) crude, as in (AB17.23): Π_n ≤ Cg_k^{−2}(1+k−n+log ℓ_k)^{b_φ}, using only |w_{l−1} − w_l| ≤ w_{l−1} + w_l and AF comparison ((Traj-w)-type, additional assumption); (ii) under **(β-bd)** |w_{l−1} − w_l| = |β_l(g_{l−1})| ≤ C_β (the one-loop recursion; an export of B-03/B-05, additional assumption): Π_n ≤ C_β·#{l ≤ k : φ_l ≢ 1 at grade n} ≤ C_β(k − n + c_φ). Either suffices.

### 7.2 Lemma P (plaquettes; curvature-square cancellation)

Let W₀ be a unitary configuration with |W₀(∂p) − 1| ≤ ε^♯(η/h)² on the fine plaquettes p of a cell, η the fine spacing, h the mesh of the layer. Let W(ζ)(b) = e^{iηA(ζ)(b)}W₀(b) with A holomorphic in ζ, 𝔤^c-valued, h|A| + h²|∇_{W₀}A| ≤ β ≤ 1 and h|∂_iA| + h²|∇_{W₀}∂_iA| ≤ β_i. Then for each p: |W(∂p) − W₀(∂p)| ≤ C_P(η/h)²β; with Y_i := W(∂p)^{−1}∂_iW(∂p) ∈ 𝔤^c: |Y_i| ≤ C_P(η/h)²β_i; and
 ∂_i tr W(∂p) = tr((W(∂p) − 1)Y_i), |∂_i tr W(∂p)^{±1}| ≤ N C_P(η/h)⁴(ε^♯ + C_Pβ)β_i.
*Proof.* W(∂p) is a product of four factors e^{±iηA(b)}W₀(b)^{±1}. Moving the exponentials to one end by conjugation with the (unitary) W₀-transports gives W(∂p) = e^{iX_p}W₀(∂p) with X_p = η²(∇_{W₀}×A)(p) + O(η²|A|²) + O(η|A|·|W₀(∂p) − 1|) (BCH for four small elements); each term is ≤ C(η/h)²(β + β² + βε^♯(η/h)). The same for the ζ-derivative. Y_i is in 𝔤^c because W(∂p) ∈ G^c, hence traceless, so tr(W(∂p)Y_i) = tr((W(∂p) − 1)Y_i). □ : the identity holds to 10^{−9}, and |tr P(t) − tr P(0)| ≤ 0.98(εβ′ + β′²) with β′ = |P(t) − P(0)| on SU(2) with complex perturbations.

### 7.3 Proposition Het conditional

Assume Theorem CR and **(Reg)**: at every real point, W₀ satisfies |W₀(∂p) − 1| ≤ ε_n^♯(η/h_n)² on layer n ≥ 1, ε_n^♯ ≤ C_regε_n (times the prefix enhancement of (H2) inside prepared regions) ((c\*) [V] Theorem 1 / [III] p.267 (3.12), which the source states on the image for the current layer: "|U_{k+1}(∂p) − 1| < 2B₃L²(1+β₀)ε_k(L^{−1}η)²"; additional assumption for old layers). For a 𝒢_n-cube c of grade n meeting supp Δw put
 F_c(ζ) := Σ_{p⊂c}Δw(x(p))·½[tr W^L(ζ)(∂p) + tr W^L(ζ)(∂p)^{−1} − (same at ζ = 0)], W^L(ζ) := e^{iη𝓗(ζ)}W₀.
Then F_c is holomorphic on 𝒮_r, Σ_cF_c = F^{het} on the real slice (s_p is gauge invariant, (CR1)), and with d = 4
 |∂_iF_c(ζ)| ≤ (w_c/r)e^{−λd(source input; x_i)}, w_c := r·6M⁴N C_P Π_n(ε_n^♯ + C_PK₁g_kr)K₁e^{λr_C}g_k.
No slots occur, so the bound is trivially uniform in the frozen data. Format: birth n, carrier {c}, anchor c, one record per cube; W_n^{S6} = w_c. With (β-bd): W_n^{S6} ≤ C r(k−n+c_φ)(ε_n + g_kr)g_k; with the crude bound: ≤ C r(ε_n/g_k + r)·polylog. The entry of the budget is e^{−νD_het/(8Θ′)}Σ_nΓ_nW_n^{S6}.

*Proof.* Lemma P with A = 𝓗(ζ), β = K₁g_kr, β_i = K₁e^{λr_C}g_ke^{−λd(source input; x_i)} from (CR2)–(CR3); the number of fine plaquettes in c is 6(Mh_n/η)⁴, which cancels (η/h_n)⁴. □

This is BC15.1 and the last display of [U17] AW §5.4, with the tangent decay supplied by CT♯ instead of [V] (190). The same computation with g_k^{−2} in place of Δw gives the absolute Wilson budget used in (Abs): W_n^{Wil} ≤ 6M⁴NC_P g_n^{−2}(ε_n^♯ + C_PK₁g_kr)K₁e^{λr_C}g_k r (no collar factor, cells everywhere).
