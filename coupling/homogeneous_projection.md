# The homogeneous projection: curvature response and Gaussian comparison

**Hypotheses.** All comparisons are in the homogeneous regular sector on the indicated real-centered charts. The assertion $D_n^G=d_B n+O(1)$ in the setting below is the Gaussian calibration hypothesis, not a consequence of the logarithmic coefficient.

### 19.1 Setting

- **Model.** The source-free Wilson recursion for 4D SU(N) lattice gauge theory in Bałaban's RG (CMP109, CMP116, CMP119, LFR I/II), in the J0/C-01 representation, restricted to the homogeneous regular sector.
- **Coupling.** Y_i = g_i^{−2}, in the published convention: weight exp(−A/g²), A = Σ_p[1 − Re tr U_p], tr 1 = 1.
- **Decrement.** c_{i+1} := Y_i − Y_{i+1}, the pre-R bulk projection of the T-output (convention (C1), §14.4).
- **Gaussian comparison.** d_i^G is the Gaussian decrement, D_n^G := Σ_{i<n}d_i^G = d_B n + O(1), and d_B := 2N²·11 log L/(24π²) > 0.
- **Corrected coordinate.** y_i := Y_i + (D_i^G − d_B i) and u_i := 1/y_i.
- **Shorthand.** ℓ_k := log Y_k and r_k := min(α_{0,k}, α_{1,k}) ≍ g_kℓ_k^q.

### 19.2 Theorem

Fix the parameters as in 19.3. Let Y_0 ≥ Y_* + D, and let K be the first index with Y_K < Y_*.

- Every step 0 ≤ i < K is admitted.
- |c_{i+1} − d_i^G| ≤ C_c/Y_i.
- With u^{UV}_m := u_{K−m}, for 0 ≤ m < K:
```
u^{UV}_{m+1} = u^{UV}_m − d_B (u^{UV}_m)² + r_m ,   |r_m| ≤ A (u^{UV}_m)³ .
```
- A is uniform in K, Y_0, the volume and the history. r_m may depend on the whole trajectory.
- B-04 (Annex S, Theorem 1.1) applies pathwise. It gives u^{UV}_m = [d_B(m+κ)]^{−1} + O(log(1+m/κ)/(m+κ)²).

### 19.3 Parameter order

1. **Source constants.**
   - L odd ≥ 13 and β = 1/4.
   - η = 1/2 and δ = (1/10)(1 − 3/L).
   - κ large, with κ′ = (5/4)κ greater than the rooted M-cube entropy.
   - κ_1 ≥ 16κ + 1; M ≥ M(κ) with δ_0M ≥ κ.
   - E_0, ε_1, A_0, p0 ≥ 5r and r.
   - Grids R_j = L^{m_j}.
   - α′ := CMP109's absolute α_0, α_1.
2. **q.** An integer q > p0, with q_0 = q_1 = q.
3. **b.** b := (4/d_B)C_Γ. It does not depend on κ0.
4. **κ0.** κ0 ≥ max{8, 2b+5}. This implies κ0 > 4.
5. **Ceiling.** Y_* large. It absorbs:
   - γ(κ0);
   - (U2): C_{κ0}g⁴ ≤ R_1;
   - the log thresholds of (2.7)–(2.8);
   - the renewal condition ρ_kC log ℓ_k ≤ ½min{1, 1 − L^{−(1−θ′)}};
   - the cross-tree smallness Σ_kC(log ℓ_k)σ^{cr}_k ≤ ½;
   - |m|/Y ≤ β/10;
   - Proposition H on the doubled radius, 8g̃P ≤ ε_ana;
   - the H-cut thresholds Π = γ_2A_1²ℓ^{2p0} ≥ Π_*;
   - B-04's interval;

6. **Y_0.**

### 20.1 Theorem HC-W by an elliptic (Bochner–Neumann) argument, with no reflected diffusion

**Setting.**
- 𝒳 = ⊕_{i∈I}ℝ^{n_i} (finite). D = Π_iD_i, each D_i a bounded convex body with nonempty interior.
- H real and C³ on an open neighbourhood N of D̄. μ = Z^{−1}1_D e^{−H}dx.
- W = diag(w_iI_{n_i}) with w_i > 0, and Sym(WH″W^{−1}) ≥ λ > 0 on N.

**Claim (HC5).** For f, g ∈ C¹(N): |Cov_μ(f,g)| ≤ λ^{−1}‖W∇f‖_{L²(μ)}‖W^{−1}∇g‖_{L²(μ)}.

**Step 1: smooth product approximation.**
- Choose smooth, uniformly convex D_i^ε with D_i ⊂ D_i^ε ⊂ D_i + B_ε (mollify the gauge function of D_i and add ε|x|²). Put D^ε := Π_iD_i^ε ⊂ N for ε small, and μ_ε := Z_ε^{−1}1_{D^ε}e^{−H}dx.
- ∂D^ε = ∪_iF_i with faces F_i := ∂D_i^ε × Π_{l≠i}D̄_l^ε. The corner set Σ := ∪_{i<l}(F_i ∩ F_l) has (dim − 1)-measure zero.
- On the relative interior of F_i the outward normal is block-pure: n = (0, …, ν_i(x_i), …, 0).
- Write L := Δ − ∇H·∇. It is symmetric on L²(μ_ε) with the Neumann form ∫∇u·∇v dμ_ε.

**Step 2: the Neumann problem and regularity.**
- Let g̃ := g − μ_εg. The form ∫∇u·∇v dμ_ε is coercive on mean-zero H¹(D^ε): Poincaré on a bounded convex domain, and e^{−H} is bounded above and below on D̄^ε. Lax–Milgram gives a unique mean-zero u ∈ H¹ with ∫∇u·∇v dμ_ε = −∫g̃ v dμ_ε for all v ∈ H¹. Equivalently, Lu = g̃ weakly with natural Neumann condition. Write ‖·‖ for L²(μ_ε).
- **Interior and smooth faces.** u ∈ H²_loc(D^ε) ∩ H²_loc near the relative interior of each face, by the standard interior and boundary H² regularity for divergence-form operators ∇·(e^{−H}∇u) with C¹ coefficients and Neumann condition (Gilbarg–Trudinger Theorem 8.8 and its Neumann analogue). If g ∈ C¹, then u is C² away from Σ.
- **Corners.** Near a point of Σ, use block-wise Fermi (boundary-normal) coordinates x_i ↦ (s_i, t_i), where t_i is the signed distance to ∂D_i^ε. These act on separate blocks, so their product straightens every face meeting at the point simultaneously into {t_i = 0}. The metric is block-diagonal.
- **Even reflection.** Reflect evenly in each t_i. The Neumann condition is the natural one, so the reflected u is a weak solution across {t_i = 0} of a divergence-form equation. Its coefficients are the reflected metric and e^{−H}, which are Lipschitz. Interior H² regularity for Lipschitz divergence-form coefficients (GT 8.8) gives **u ∈ H²(D^ε)**.

**Step 3: a core.** Let 𝒞_N be the set of v ∈ C^∞(D̄^ε) with ∂_nv = 0 on every face.
- **Density.** 𝒞_N is dense in the H²-Neumann class: apply a partition of unity whose cutoffs are even in every t_i near faces, so ∂_n(cutoff) = 0. Near Σ, mollify the evenly reflected function with a kernel that is even in each t_i. The result is smooth, even in every t_i, so it satisfies ∂_{t_i} = 0 at t_i = 0. That is the exact Neumann condition, because Fermi coordinates are orthogonal at the boundary. The mollified functions converge in H².
- **Identity (B), for v ∈ 𝒞_N.** Write L_{W^{−2}}v := e^{H}∇·(e^{−H}W^{−2}∇v) = Σ_iw_i^{−2}(Δ_iv − ∇_iH·∇_iv). Then
  ```
  ∫(L_{W^{−2}}v)(Lv)dμ_ε = Σ_jw_j^{−2}∫|∇∂_jv|²dμ_ε + ∫⟨W^{−1}∇v, Sym(W^{−1}H″W)W^{−1}∇v⟩dμ_ε + Σ_iw_i^{−2}∫_{F_i}S_i(∇_iv,∇_iv)e^{−H}dσ/Z_ε .   (B)
  ```
  Here S_i ≥ 0 is the shape operator of ∂D_i^ε.
- **Proof of (B).** Gauss–Green on the Lipschitz domain D^ε with C¹ vector fields.
  - **First integration.** ∫(L_{W^{−2}}v)(Lv)dμ = −∫⟨W^{−2}∇v, ∇(Lv)⟩dμ + ∫_∂(Lv)⟨W^{−2}∇v, n⟩. The boundary term vanishes: on F_i, ⟨W^{−2}∇v, n⟩ = w_i^{−2}⟨∇_iv, ν_i⟩ = 0. **This is where block-pure normals and block-scalar W are used.**
  - **Commutator.** ∂_j(Lv) = L(∂_jv) − Σ_kH″_{jk}∂_kv, so −∫⟨W^{−2}∇v, ∇Lv⟩ = −Σ_jw_j^{−2}∫∂_jv L∂_jv + ∫⟨W^{−2}∇v, H″∇v⟩.
  - **Second integration.** −∫∂_jv L∂_jv = ∫|∇∂_jv|² − ∫_∂∂_jv ∂_n∂_jv.
  - **Boundary integrand.** On F_i it is B := ⟨W^{−2}∇v, ∇²v n⟩. Write ∇²v n = ∇⟨∇v, n⟩ − (Dn)^T∇v, with n extended as ν_i(x_i), a function of x_i alone.
    - The vector W^{−2}∇v is tangent to F_i: its block-i part w_i^{−2}∇_iv is ⊥ ν_i, and the other blocks are tangent. Since ⟨∇v,n⟩ ≡ 0 on F_i, the first term contributes zero.
    - Dn = 0 ⊕ ⋯ ⊕ S_i ⊕ ⋯ ⊕ 0 is block-diagonal and acts only on block i. On block i, W^{−2} is the scalar w_i^{−2}, so **W^{−2} commutes with Dn**.
    - Hence B = −w_i^{−2}S_i(∇_iv,∇_iv) ≤ 0, and its sign enters (B) as the positive last term.
  - Finally, ∫⟨W^{−2}∇v, H″∇v⟩ = ∫⟨W^{−1}∇v, (W^{−1}H″W)W^{−1}∇v⟩, and Sym(W^{−1}H″W) = Sym(WH″W^{−1}) for symmetric H″.
- **Extension to u.** Both sides of (B) are continuous in the H² norm: the left side and the bulk terms involve derivatives of order ≤ 2, and the face term involves traces of ∇v ∈ H^{1/2}. So (B) holds for u by density.

**Step 4: the estimate.**
- (B) with the last two terms dropped or bounded below gives ∫(L_{W^{−2}}u)(Lu)dμ_ε ≥ λ‖W^{−1}∇u‖².
- One integration by parts (H² × H¹; boundary term zero by Neumann and block-purity, as in Step 3) gives ∫(L_{W^{−2}}u)g̃ dμ_ε = −∫⟨W^{−2}∇u, ∇g⟩dμ_ε.
- Hence λ‖W^{−1}∇u‖² ≤ ‖W^{−1}∇u‖‖W^{−1}∇g‖, i.e. ‖W^{−1}∇u‖ ≤ λ^{−1}‖W^{−1}∇g‖.
- Then Cov_{μ_ε}(f,g) = ∫f g̃ dμ_ε = ∫f Lu dμ_ε = −∫⟨∇f, ∇u⟩dμ_ε. Integration by parts with the Neumann condition, no boundary term.
- So |Cov_{μ_ε}(f,g)| ≤ ‖W∇f‖‖W^{−1}∇u‖ ≤ λ^{−1}‖W∇f‖_{L²(μ_ε)}‖W^{−1}∇g‖_{L²(μ_ε)}.

**Step 5: ε → 0.**
- 1_{D^ε} → 1_{D̄} pointwise, and ∂D has Lebesgue measure zero (D convex with interior). With f, g, ∇f, ∇g, e^{−H} bounded on N, dominated convergence gives Z_ε → Z, Cov_{μ_ε}(f,g) → Cov_μ(f,g), and the weighted norms converge.
- λ is uniform in ε because the gap holds on N ⊃ D^ε. (HC5) follows. □

**Application to the comparator.**
- **Domain.** D = Π_b{|a_b| ≤ P}, a product over the finitely many independent bonds of Lie-algebra norm balls. These are convex bodies; the matrix-norm ball need not be smooth, which Step 1 handles.
- **Interaction.** H = H_{τ,0} is real-analytic on N := Π_b{|a_b| < 2P} ⊂ {g̃‖a‖ < ε_ana}. Proposition H's margin 4g̃·2P ≤ ε_ana holds below the ceiling.
- **Gap.** (HC22) applies on N with λ ≥ m/2 (§15.10, 18.2).
- **Weights.** The weights of J-C, W_b = e^{αd(b,U_A)}, are block-scalar: one scalar per bond block.
- So HC-W holds for the comparator **without the reflected diffusion.**
- The raw-moment bound (HT20)–(HT26) also used the diffusion (Itô with reflection). Its replacement is the same Bochner argument applied to v = |W_xA|^{p/2}-type test functions. Alternatively, and more simply, the Gaussian moment bound follows from HC-W itself via the standard Herbst/Poincaré argument applied to the Lipschitz functions A ↦ |W_xA|. I record this as a **gap**: written in outline only, not in full.

**Imports now used.** Lax–Milgram, Poincaré, H² regularity for divergence-form equations with Lipschitz coefficients, and even reflection. These are textbook elliptic facts (Gilbarg–Trudinger Ch. 8). No probabilistic import remains in HC-W.

### 20.2 Repeating CMP116 (2.31)–(2.34) for the comparator cutoff P = A_1ℓ^{p0}

The argument below follows CMP116 pp.17–19.
- In the source, the cutoff complement contributes, per defect bond, the factor exp(−½γ_2ε_1²/g_k²) of (2.26). This comes from the estimate (2.22) with γ_2 small; (2.23) absorbs e^{½γ_2|B|²}-type terms into α_5.
- The canonical source cutoff is ε_1/g_k. Replacing it by P gives exactly H-cut's (Hc3) with u = γ_2/2. The Gaussian absorption (2.23)–(2.25) needs α_5‖C^{(k)}‖ < 1/2. This holds because ‖C^{(k)}‖ ≤ γ_0^{−1} (CMP95 (1.90)) and α_5 contains γ_2 small, independently of P.
- Writing Π := γ_2P², the source's four conditions become:

| Source line | Displayed condition (P in place of ε_1/g_k) | Holds once |
|---|---|---|
| (2.31) | Σ_P exp(−Π M^{−4}\|Z_0\Y_0\|/20)·exp(−Π\|P\|/10) ≤ exp(−M^{−4}\|Z_0\Y_0\|[Π/20 − 4M⁴e^{−Π/10}]) ≤ 1 | Π/20 ≥ 4M⁴e^{−Π/10}, i.e. Π ≥ Π_1(M) |
| (2.32)–(2.33) | Π/20 ≥ 4κ (to beat the d_k(Z_0) exponent), and exp(−Π/20) ≤ ε_2 | Π ≥ max{80κ, 20 log(1/ε_2)} |
| (2.34) | Σ_{Z_0\Y_0}exp(−Π M^{−4}\|Z_0\Y_0\|/20) ≤ exp(e^{−Π/20}M^{−4}\|Z_0\|), and with (2.30) this is ≤ exp(δκd_k(Z_0)) | e^{−Π/20}·24 ≤ δκ, i.e. Π ≥ 20 log(24/(δκ)) |

- Every condition is a **lower bound on Π = γ_2A_1²ℓ_k^{2p0}**, which tends to ∞ as g → 0. So all hold below a coupling ceiling depending only on (M, κ, δ, ε_2, γ_2).
- No condition involves an upper bound on P other than the analyticity requirement P ≤ ε_1/g (Lemma 1's domain), which holds since g̃P = δ_k → 0. The rest of §2, (2.35)–(2.41), does not involve the cutoff.
- **This confirms Proposition H-cut for the comparator cutoff.** Status: verified line by line against CMP116 (2.31)–(2.34).

###  integration by parts only

**Setting.** As in 20.1: D = Π_iD_i, each D_i a bounded convex body **containing 0**; H ∈ C¹(D̄); μ = Z^{−1}1_De^{−H}dx. Take a block-scalar weight W = diag(w_iI) with 0 < w_i ≤ 1, and assume Sym(WH″W^{−1}) ≥ λ > 0 on D. Put T := tr W², B := ‖W∇H(0)‖, q(A) := |WA|².

**Lemma 22.1.** For p ≥ 2,
```
‖ |WA| ‖_{L^p(μ)} ≤ B/λ + √( (T + (p−2)) / λ ) .
```
For the comparator with W_x = diag(e^{−αd(x,i)}): T_x ≤ C_α uniformly in the volume, B_x ≤ C_αb_0 with b_0 := sup_i|∇_iH(0)| = O(|τ|) (20.3), and |A_x| ≤ |W_xA|. Hence ‖A_x‖_p ≤ C_α(b_0/λ + √(p/λ)). This is (HT26), including the mean, and with **no dependence on the cutoff P or the volume**.

**Proof.**
1. **The vector field.** For ε > 0 put q_ε := q + ε and Ψ := W²A q_ε^{(p−2)/2}e^{−H}. This is C¹ on D̄.
2. **Gauss–Green.** D is a convex, hence Lipschitz, domain, so
   ```
   ∫_D div Ψ dx = ∫_{∂D}⟨Ψ, n⟩dσ .
   ```
   On a face F_i the outward normal is block-pure, n = (…, ν_i, …), where n is defined (σ-a.e., away from the corner set). Then ⟨W²A, n⟩ = w_i²⟨A_i, ν_i⟩ ≥ 0, because D_i is convex and contains 0, so the supporting half-space at A_i ∈ ∂D_i contains 0. Hence the boundary integral is ≥ 0.
3. **Expanding the divergence.**
   ```
   div Ψ = e^{−H}[ T q_ε^{(p−2)/2} + (p−2)q_ε^{(p−4)/2}|W²A|² − ⟨W²A, ∇H⟩q_ε^{(p−2)/2} ] .
   ```
4. **The resulting inequality.** Using |W²A|² ≤ ‖W‖²q ≤ q_ε, step 2 gives
   ```
   E[⟨W²A, ∇H(A)⟩ q_ε^{(p−2)/2}] ≤ (T + (p−2)) E[q_ε^{(p−2)/2}] .
   ```
5. **Lower bound on the left side.** By the mean-value formula along the segment sA ⊂ D (D convex and 0 ∈ D),
   ```
   ⟨W²A, ∇H(A) − ∇H(0)⟩ = ∫_0^1⟨WA, (WH″(sA)W^{−1})WA⟩ds ≥ λ q ,
   ```
   and ⟨W²A, ∇H(0)⟩ ≥ −B q^{1/2}. So the left side is ≥ λE[q·q_ε^{(p−2)/2}] − B·E[q^{1/2}q_ε^{(p−2)/2}].
6. **Conclusion.** Let ε ↓ 0 by monotone convergence and write R_p := ‖|WA|‖_p. Hölder gives
   ```
   λR_p^p ≤ (T + p − 2)R_p^{p−2} + B R_p^{p−1} ,   i.e.   λR_p² ≤ T + p − 2 + B R_p ,
   ```
   and solving the quadratic proves the claim. □

**Remarks.**
- The diffusion's reflection-sign argument (HT21) is replaced by the boundary sign in step 2.
- Only C¹ regularity of H on D̄ and convexity of the factors are used.
- No Poincaré inequality is needed. The mean is included because the bound is on raw moments; (HT25) is reproduced exactly.
- **Item closed.**

###  annihilation of the zero-mean periodic remainder, divisibility, and the true cost

**(a) Divisibility, with no condition on M.**
- An MR_j-cube of the scale-j lattice has physical side ML^{m_j}·L^jη = M·L^{j+m_j}η. That is exactly an M-cube of the scale-(j+m_j) partition.
- Bałaban's localization partitions are nested: an M-cube at scale k+1 is an LM-cube at scale k (CMP116 §2, p.12: "cubes from π_{k+1}, i.e. cubes of size LM in the scale corresponding to T_η").
- So for every k ≥ j + m_j, each M-cube of scale k is a disjoint union of exactly L^{4(k−j−m_j)} period cells (MR_j-cubes). For j ≤ k ≤ j + m_j, each period cell is a union of M-cubes of scale k.
- A grid change only shifts m_j by one. Since all partitions share the origin of the nested family, alignment is automatic.
- The period lattice of the R^{(j)}-structure is therefore the M-cube lattice of scale j + m_j. Its side in scale-k units is
  ```
  π_k := M·L^{(j+m_j)−k} ,
  ```
  which is ≥ M for k ≤ j + m_j and < M afterwards.

**(b) Setup.** By 21.1, every λ_j-descendant's marginal part splits into a scalar Wilson part β̄A, extracted into m, and a zero-mean periodic part
```
𝒯(U) = Σ_{x} c̃(x) Q(F_{(·)}(x)) ,   Σ_{x ∈ period cell} c̃(x) = 0 ,
```
where Q is a quadratic form in the curvature at the activity's own scale, and c̃ is periodic with period cell of side π.

**Lemma 22.2 (annihilation after a_j := m_j).** Let k ≥ j + m_j, and let 𝒯 be evaluated on composite arguments: the averaged background U_{(·)}(V) and the insertion fields of step k, which lie in D^♯ (17.4, 21.2). Then
```
𝒯 = Σ_{X: M-cube of scale k} Σ_{x∈X} c̃(x)[Q(F(x)) − Q(F(x_X))] ,
```
with x_X any fixed point of X. The zero-momentum F² part of each M-cube sum vanishes identically. What remains is a sum of derivative terms of dimension ≥ 5, bounded on D^♯ by
```
|Σ_{x∈X}c̃(x)[Q(F(x)) − Q(F(x_X))]| ≤ C‖c̃‖_∞·π_{(own)}·|X|·sup_X|F||∇F| ,
```
where π_{(own)} is the period in the activity's own units.

*Proof.* Each M-cube X of scale k is a union of whole period cells, by (a). So Σ_{x∈X}c̃(x)Q(F(x_X)) = Q(F(x_X))Σ_{x∈X}c̃(x) = 0. Subtracting this zero gives the identity. The bound follows from Q(F(x)) − Q(F(x_X)) = O(|x − x_X||F||∇F|) and the zero mean of c̃ on each period cell, which allows re-centering inside each period cell, so that |x − x_X| is replaced by a distance ≤ diam(period cell) = π. □

```
c′_{per}(a) ≤ C           for a := k − j ≤ m_j   (marginal: L^{4a} cancelled by the four scale powers of F², no gain),
c′_{per}(a) ≤ C L^{−(1−θ)(a − m_j)}   for a > m_j   (Lemma 22.2: dimension-5, gain from π_k).
```
The insertion fields of step k are smooth on sub-block scales. Their curvature variation over an M-cube is controlled by the regularity conditions (1.12)–(1.13) of the native space, which are part of D^♯. So the same lemma applies to the fluctuation differences: these are monomials with at least one insertion factor (17.3), and the relative gain ρ_k is unaffected.

**Lifetime independent of generation.** The period is a fixed physical length, M·L^{j+m_j}η. Every descendant of R^{(j)}, whatever its generation, sees the same π_k at scale k. So the periodic channel exists only for scales k ∈ [j, j + m_j], and it does not restart with each generation.

**(c) The true cost: logarithmic, not ℓ^{C_per}.**
- **Kernel sum.** The full kernel is c′_j(a) = c′(a) + c′_{per}(a), and
  ```
  Σ_{a≥0}c′_j(a) ≤ Ĉ + C(m_j + 1) + C/(1 − L^{−(1−θ)}) ≤ C log ℓ_j .
  ```
- **Renewal condition** (Lemma R, 14.6(a)): ρ_k·C log ℓ_k ≤ ½ min{1, 1 − L^{−(1−θ′)}}. With ρ_k = Cℓ_k^{p0−q}, this holds below the ceiling **for every integer q > p0**.
- **Decay of c̃_j.** The Neumann series c̃_j = Σ_{m≥1}ρ̄^{m−1}c′_j^{*m} gives
  - c̃_j(a) ≤ 2C for a ≤ m_j;
  - c̃_j(a) ≤ 2CL^{−(1−θ)(a−m_j)/2} for a > m_j, by splitting the convolution at the plateau, since ρ̄C log ℓ ≤ ½.
  - Hence Σ_ac̃_j(a) ≤ C(m_j + 1) ≤ C log ℓ_j.

- So the κ0 condition and b are unchanged, and **the requirement "q > p0 + C_per′" of 21.1 is not needed: q > p0 suffices.**
- **Readout.** The direct readout of the periodic part is P(𝒯) = 0 on compatible tori, whose volume is a union of period cells. This is exact by the zero mean of c̃. The readout of the dimension-5 remainders after a_j is bounded by κ^♯_E times their ♯ size, as for any irrelevant term.

**(d) Hyperoctahedral step (21.1(3)), checked.** The scalar extraction needs the period-averaged quadratic form c̄ on Λ²ℝ⁴ to be a multiple of Σ_{μ<ν}F_{μν}².
- The hyperoctahedral group (signed permutations of the axes) acts on the six components F_{μν}. Its permutations act transitively on the six pairs, and the coordinate reflections flip the sign of F_{μν} for exactly those pairs containing the reflected axis.
- A quadratic form invariant under all sign flips is diagonal in the F_{μν} basis. Each off-diagonal entry F_{μν}F_{ρσ} with {μν} ≠ {ρσ} is odd under the reflection of an axis in one pair but not the other. Note that ε^{μνρσ}F_{μν}F_{ρσ} is of this off-diagonal type and is killed by such reflections.
- Transitivity then forces equal diagonal entries.
- So c̄ = β̄·ΣF². This uses only that G_j contains the hyperoctahedral group about cube centres, which CMP119 (2.32) states.

**Status of fix (α):**
- The divisibility (a), Lemma 22.2, the kernel (c) and the invariant theory (d) are **proved** here, given the source inputs.

### 23.2 Equivariance of the homogeneous-sector R^{(j)} and its descendants

**Groups.**
- G_j is the group of lattice isometries preserving the partition into MR_j-cubes at scale j. It consists of translations by MR_j-cube vectors and the hyperoctahedral group B_d about cube centres.
- By 22.2(a), an MR_j-cube at scale j is an M-cube at scale j + m_j.
- G_k^{blk} denotes the isometries preserving the scale-k block structure and the scale-k M-cube partition π_k.

**Lemma 23.1.**
- (i) R′^{(j)}(rX, rU) = R′^{(j)}(X, U) for all r ∈ G_j.
- (ii) For j ≤ k ≤ j + m_j, G_j ⊂ G_k^{blk}. Consequently every λ_j-descendant at scale k is G_j-covariant, in the summed sense of (N5).

**Proof of (i).** The R-operation is a finite composition of maps, each equivariant under G_j.
- **(E1) Selected sets.** Large-field regions, components, determining sets and partitions of unity are unions of MR_j-cubes. They are selected by cube-wise gauge-invariant thresholds, (N3). So they transform as r·(sets).
- **(E2) Invariant ingredients.** The Wilson action, Haar measure and normalization constants are Euclidean invariant.
- **(E3) Block variables.** The averages U(y,x) = M({U(Γ)}_{Γ∈G(y,x)}) (CMP109 (0.11)) are equivariant under isometries that fix y and preserve the block. This needs (N4), together with the axioms (0.6), conjugation-covariance, and (0.7), permutation invariance. The exponential gauge fixing (0.14) is built from U(y,x), so it is equivariant as well.
- **(E4) Minimizers.** The minimizer is unique on regular data (LFR I Proposition 1; CMP102). Uniqueness forces r·(minimizer of D) = minimizer of r·D.
- **(E5) Axial-gauge trees.** These are the only coordinate-dependent ingredient. LFR I (1.100) and LFR II (1.71) average δ_{rT} over r ∈ B_d with weight 1/(2^d d!). For r_0 ∈ B_d, the map r ↦ r_0r permutes the summands, so the average is B_d-equivariant. Translation covariance holds because the trees are built per cube or component (N1).
- **(E6) Earlier-scale operations.** The operations T_h(Z_h ∩ X) inside (1.71) are covariant by induction on the scale: (2.32) at earlier scales for R, and (2.29)/(2.33) for summed E.
- **(E7) Combinatorial steps.** The Mayer expansion, the exponentiation (1.98), the split by intersection with the large-field region, and the vacuum subtraction R^{(j)}(Λ_j, 1) are functorial on equivariant families indexed by unordered collections of cubes.

So each localized R′^{(j)}(X, ·) is G_j-covariant. Its domains X are unions of MR_j-cubes, which r permutes. □

**Proof of (ii).**
- **Translations.** Translations by period vectors M·L^{j+m_j}η are multiples of the scale-k block size L^kη, and of the scale-k M-cube size, when k ≤ j + m_j.
- **Point group.** For the point group about a period-cell centre c, the period cell is an L^{j+m_j−k}-sided array (L odd) of scale-k M-cubes, each an M-array of scale-k blocks.
  - If M is odd, c is a scale-k block centre.
  - If M is even, c is a vertex of the block grid.
  - In either case, reflections and permutations about c map the block grid and π_k onto themselves, and map block centres to block centres.
- So G_j ⊂ G_k^{blk}. The homogeneous-sector T-step at scale k is equivariant under G_k^{blk}: this is the Euclidean covariance of E (CMP119 (2.29), as an unrestricted sum), together with (E3), (E4) and (E7) at scale k.
- Hence descendants of a G_j-covariant input are G_j-covariant for k ≤ j + m_j. □

###  the self/cross split of the λ_j-descendants

**The problem.** The claim in 22.2 that "the lifetime is independent of generation" assumed that every λ_j-descendant is G_j-covariant. But ∂_{λ_j}E^{(k)} = DΦ_k[S_k]·δ_k, where Φ_k is the scale-k T-step and S_k is the **actual** state at scale k. That state contains the other live R^{(j′)} and, under (C1), their descendants. So DΦ_k[S_k] is equivariant only under the symmetry group of S_k.

**Symmetry of the state (Lemma 24.0).**
- All period lattices have the form M·L^p·ℤ^d with a common origin (22.2(a)), so they are nested.
- A cell of side ML^p is an odd array (L odd) of cells of side ML^{p′}, p′ < p. So the centre of a coarse cell is the centre of a finer cell.
- Hence S_k is invariant under 𝒢^{(k)} := (translations by ML^{P_k}ℤ^d) ⋊ B_d, where P_k := max{j′ + m_{j′} : j′ ≤ k, j′ + m_{j′} ≥ k} is the coarsest live period.
- Since m_{j′} ≤ r log_L ℓ_{j′} + 1 and ℓ_{j′} ≤ ℓ_k + 1 (prefix with slack), P_k ≤ k + C log ℓ_k.
- Grids with j′ + m_{j′} < k are dead at scale k: by Lemma 22.2 their periodic parts are already of dimension 5 and need no covariance.

**Symmetrization.**
- For j ≤ k ≤ j + m_j, G_j ⊂ G_k^{blk} (Lemma 23.1(ii)), and G_j acts on the finite torus as a finite group.
- Define the G_j-symmetrized state S̄_k := |G_j|^{−1} Σ_{r∈G_j} r·S_k. This averages the activities only; the selectors and couplings are frozen and, in the homogeneous regular sector, whole-lattice.
- The inductive spaces are invariant under this average: the bounds, analyticity and gauge invariance are all preserved by convex combination and by r. So S̄_k is an admissible state.
- Φ_k is G_k^{blk}-equivariant: Lemma 23.1(ii) and (E3), (E4), (E7) at scale k. Hence DΦ_k[S̄_k] is G_j-equivariant.

**Split.** Write δ_k = δ_k^{self} + δ_k^{cr}, defined recursively from δ_j := (derivative of the input R^{(j)}), with δ_j^{self} := δ_j:
```
δ_{k+1}^{self} := DΦ_kS̄_k            (for k ≤ j + m_j; afterwards DΦ_k[S_k], no symmetry needed),
δ_{k+1}^{cr}   := DΦ_kS_k + (DΦ_k[S_k] − DΦ_k[S̄_k])(δ^{self}_{≤k}) .
```
- **Self part.** By induction δ^{self}_k is G_j-covariant for k ≤ j + m_j. Its periodic channel has the fixed physical period ML^{j+m_j}, and its lifetime is exactly m_j steps from j, **independently of generation**. This gives the claim of 22.2 for the self part only. The annihilation lemma 22.2 applies after j + m_j.
- **Cross remainder at step k.** By the mean-value formula,
  ```
  (DΦ_k[S_k] − DΦ_k[S̄_k])δ = ∫_0^1 D²Φ_kS̄_k + t(S_k − S̄_k) dt .
  ```
  The second variation is bounded by the ζ-Cauchy argument of Lemma B in two auxiliary complex parameters, with the same relative insertion gain ρ_k (17.3). This gives
  ```
  ‖(DΦ_k[S_k] − DΦ_k[S̄_k])δ‖^♯ ≤ C ρ_k ‖S_k − S̄_k‖_{act} Σ_{i≤k} c′(k−i)‖δ_i‖^♯ ,
  ```
  where ‖·‖_{act} is the activity norm divided by the cluster-expansion budget.
- **Size of S_k − S̄_k.** It vanishes on the G_j-invariant part of S_k. That part includes the whole comparator/Wilson sector, which is fully covariant. So S_k − S̄_k is bounded by twice the R-related content of S_k: the R-ledger terms R^{(j′)}, and the R-descendants inside the E-births under (C1). Per current site:
  - each age j′ contributes O(1)·g_{j′}^{κ0}, by marginal persistence (CMP119 (2.5));
  - the R-descendant part contributes at most (log ℓ)·ε_{j′}r_{j′}², by 22.2(c);
  - summing with (U2) on the prefix with slack gives
  ```
  ‖S_k − S̄_k‖_{act} ≤ C (log ℓ_k) Σ_{j′≤k} g_{j′}^{κ0} ≤ C (log ℓ_k) g_k^{κ0−2} .
  ```
  So the cross source at step k is σ^{cr}_k := Cρ_k(log ℓ_k)g_k^{κ0−2}, times the input.
- **Propagation of the cross part.** δ^{cr} is generated at step k as a 𝒢^{(k)}-covariant object: it is the difference of two maps, each equivariant under 𝒢^{(k)} ∩ G_j. Its periodic channel therefore has period ML^{P_k} and lifetime ≤ P_k − k ≤ C log ℓ_k further steps, after which Lemma 22.2 annihilates it. During propagation it can again meet a coarser state and split. Iterating the decomposition gives a **generation tree**:
  - every cross event at step k costs a factor σ^{cr}_k;
  - every channel, self or cross, has kernel mass ≤ C log ℓ (22.2(c), with m_j replaced by the lifetime ≤ C log ℓ).
- **Summation.** Summing the tree,
  ```
  Σ_k ‖δ_k‖^♯-contributions ≤ C(log ℓ_j)·Σ_{n≥0} ( C(log ℓ)·Σ_{k≥j}σ^{cr}_k )^n · ε^♯_j .
  ```
  With Y_k ≥ ½(Y_n + (d_B/2)(n−k)) for k ≤ n, the inner sum satisfies
  ```
  Σ_{k≤n}σ^{cr}_k ≤ C Σ_{k≤n} ℓ_k^{C}Y_k^{−(κ0−2)/2} ≤ C ℓ_n^{C} Y_n^{1−(κ0−2)/2} = C ℓ_n^C g_n^{κ0−4} .
  ```
  This is **finite, and small below the ceiling, for κ0 > 4.** The geometric series converges once C(log ℓ)Σσ^{cr} ≤ ½, which is a ceiling condition.
- **Conclusion.**
  - The persistent periodic channel costs O(log ℓ_j) for the self part plus O(1)·(small) for all cross generations.
  - (H-λ′♯) holds with ε^♯_j → C(log ℓ_j)ε^♯_j, exactly as stated in 22.2(c).
  - **The κ0 condition κ0 ≥ max{8, 2b+5} already implies κ0 > 4.** b is unchanged and still independent of κ0.
