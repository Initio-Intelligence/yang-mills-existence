# Structured cluster rates and two-layer geometry

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

**Local-chart hypotheses.** In every application use (A8′) in the structured form 3′ and 4′, F(4′) on (Avg), (Sm3′), (Par-g_Z′), and (Lay-W), with $M_W\mid M_1$ and $M_1\ge6M_W$. In particular the per-potential rate must satisfy $\kappa_1/2\ge\sqrt d(1+3\beta)\kappa/(1-3\delta)$. The bound on the joint terminal law requires the action estimate and item 4′.

## 2. CMP96 (2.59): the definitive reading, and Lemma 2.1′

**Reading.** The condition printed in [P2] is
\[
\tfrac14\alpha\delta_0RM>2d\log c_0(\tfrac12\alpha)+1,\qquad c_0(\tfrac12\alpha)=\coth(\alpha\delta_0/4).
\tag{2.59}
\]
* [N] is right that the construction quoted ½α: Local deformation of propagators and the minimizer S5, The one-sided collar estimate l.194/l.285 (where the misquote is labelled source), and the collar estimate item 4.
* The printed thresholds are (finite comparison, d = 4):

| α | role | δ₀ = 1 | δ₀ = ¼ |
|---|---|---|---|
| ½ | true package | 141.4 | 229.8 |
| ¼ | (Geo-α) | 371.1 | 548.3 |
| ⅛ | s-variant | 919.3 | 1274.1 |

**But the doubling is not forced.** The printed condition is only a sufficient condition chosen by Bałaban; the next line of his proof keeps a spare factor \(e^{-\frac14\alpha\delta_0RM\max(|j-j'|-1,0)}\) that the conclusion does not use.

> **Lemma 2.1′ — deduction, on the printed (2.58).** Let 0 < α < 1 and
> \[
> \tfrac12\alpha\delta_0RM>2d\log c_0(\tfrac12\alpha)+1. \tag{2.59′}
> \]
> Then (2.60)–(2.63) of [P2] hold with the same \(c_1(\alpha)=12c_0^d(\frac12\alpha)\).
> *Proof.* (2.60) is the geometric fact behind (2.57); it does not use (2.59). For (2.61), put \(q:=e^{-\frac12\alpha\delta_0RM}c_0^{2d}\). By (2.59′), \(q<e^{-1}\). In (2.58),
> \[
> \sum_{m\ge m_0}e^{-\frac12\alpha\delta_0mRM}c_0^{d(2m+1)}=c_0^d\frac{q^{m_0}}{1-q}\le\frac{e}{1-e^{-1}}\,c_0^de^{-|j-j'|},\qquad m_0=\max(|j-j'|-1,0).
> \]
> Summing over \(j'\in\mathbb Z\) gives at most \(\frac{e}{1-e^{-1}}\coth\frac12\,c_0^d=9.31\,c_0^d<12c_0^d\). (2.62) is (2.61) iterated. (2.63) is (2.62) with the triangle inequality (2.54). \(\square\)
> finite comparison evaluates the one-sided sum (j′ ≥ 0) at equality in (2.59′): 6.59 c₀^d.

**Consequence.** Two options are equally rigorous.
1. Cite (2.59) as printed. The thresholds are 141.4, 371.1 and 919.3 at δ₀ = 1.
2. Cite Lemma 2.1′. the collar estimate's numbers 70.7 and 459.7 stand. (Geo-α) becomes δ₀LM₁ > 185.5 (274.2 at δ₀ = ¼), and (Geo-PF) of the conditional-coordinate convention stays at ≈ 70.7.

Either way only constants fixed right after d, L are affected. [N]'s §0 item 5, its finding 4 and the walk-block conditions item 3 ("thresholds double") should read: "double if (2.59) is cited as printed; unchanged with Lemma 2.1′". The one-sided collar estimate's label "(c)" on the misquote should be corrected.

## 3. Lemma F

### 3.1 F(1): the axial representative leaves [P]'s complex domain

The claim is intrinsic, not an artefact of the decomposition. For any factorisation \(\mathbf U^{\rm ax}(b)=\tilde U'\tilde U\) with \(\tilde U\) unitary, \(\tilde U'\tilde U'^*=\mathbf U^{\rm ax}\mathbf U^{{\rm ax}*}\). So the non-unitary size of \(\tilde U'\) is fixed by \(\mathbf U^{\rm ax}\).

Take two adjacent blocks of side l, axial contours "x first, then y" from each block's root, and the roots joined by the coarse contour.
* For blocks adjacent along the **first** contour direction, the loops are thin and the ratio stays O(1): 1.3 → 1.7.
* For blocks adjacent along the **second** direction, the loop encloses an area of about \(l^2/2\). The ratio |Im A^ax| / (α₁/l) on the crossing bonds is 1.2, 4.7, 11.9, 26.2, 55.0 for l = 4, 8, 16, 32, 64.

So the claim holds for the bonds transverse to the first contour direction, which is all a counterexample needs.

A single block does not exhibit growth, because inside a block the transverse bonds carry only a 1 × y strip of flux. The "block boundary" qualifier in [N] is essential.

### 3.2 F(2)–(3): covariance and the repaired definition, deduction given the algebraic form of the operators

* Every primitive is either an explicit polynomial expression in U and U⁻¹ (with the complex-bilinear transpose replacing the adjoint), an inverse of one, or a convergent series of such. The block averaging is also covariant, provided its log/exp series stay convergent after conjugation.
* So \(X(U^u)=R(u)X(U)R(u)^{-1}\) holds wherever both sides are given by convergent expressions.
* The deformed fixed-point equation transforms covariantly, and the small solution at (𝐔, 𝐉) with transported datum is holomorphic on Dec♯'s domain.
* At real configurations, \(u_{\mathbf U}\) is unitary and both definitions agree. So the repaired definition (F(3)) is the analytic continuation of the source's object from the real points. That is the point that matters, and it is correct.

Two precisions:
* *Convergence after conjugation.* Conjugating by a non-unitary frame enlarges norms by at most ‖Ad u‖ ≤ 2 (under F(4)). Every series used in F(2) must therefore be applied on domains shrunk by a factor 2. (Sm4) already contains this factor 2.
* *Lemma D.* Lemma D's "invariant in modulus under gauge changes" is false for complex gauge transformations. It is not needed:
  * \(\tilde B={\rm Ad}(u_{\mathbf U}^{-1})B_b(\mathbf U)\) is the datum in the original frame.
  * Computing it in the (2.38)/(1.65) gauge w, which is **G-valued** since (2.38) is a statement about the real factor U, changes it by a unitary conjugation.
  * So Lemma D's bound holds for \(\tilde B\) directly.

### 3.3 F(4): the frame bound — **not deduction; conditional on (Avg)**

[RD] Definition 2.5 item 1 defines the frame hierarchically:
\[
u_{\mathbf U}(x)=u_{\mathbf U}(y)\,(M^j\mathbf U)(y,x),\qquad x\in B(y)\cap T^{(j)},\ y\in T^{(j+1)},
\]
with contour variables of the **averaged configurations** \(M^j\mathbf U\), j ≥ 1.

[N]'s proof bounds \(|\log v|\) by \(\sum|\eta A'|\) along a fine-lattice contour, i.e. as if \(u_{\mathbf U}\) were a product of links of \(\mathbf U\). That is true only for the level-0 segment. The level-j segments need a bound on the non-unitary part of \(M^j(U'U)\) relative to \(M^j(U)\). That is exactly what (Avg) supplies.

> **Lemma F(4′) — conditional on (Avg) and [I] (0.11).** Let \(C_A\) be the Lipschitz constant, in the scaled variable, of the averaging maps on the ball \(|a|<\frac12r_*\) (by Cauchy, \(C_A\le2\sup|M|/r_*\)). Assume \(a^{\rm dat}_0+a^{\mathbb G}_1\le\frac12r_*\) (a coupling ceiling). Then \(|\log v(x)|\le2dLC_A\,a^{\mathbb G}_1\), and \(\|{\rm Ad}(u_{\mathbf U}^{\pm1})\|\le2\) under
> \[
> \textbf{(Sm3′)}\qquad4dLC_A\,a^{\mathbb G}_1\le\log2.
> \]
> *Proof.* Compute in the G-valued gauge w of (2.38) (Lemma N), where \(U^w=e^{i\eta A}\) and \(\mathbf U^w=e^{i\eta a}\) with \(|a|\le a_0^{\rm dat}+a_1^{\mathbb G}\) in scaled units.
> * At each level j, (Avg) gives \(|\log M^j(\mathbf U^w)(c)M^j(U^w)(c)^{-1}|\le C_AL^j\eta|A'|_{\rm scaled}\).
> * The level-j contour has at most \(dL\) level-j links. Summing over levels geometrically gives \(\le2dLC_Aa^{\mathbb G}_1\).
> * The unitary part of the frame is the axial frame of the real factor, conjugated by w. It does not affect ‖Ad‖. \(\square\)

**Two bookkeeping slips in [N] §2.4(4).**
* For (T), \(a^{\mathbb G}_1\) already contains \((1+\beta)\), and the displayed bound multiplies by \((1+\beta)\) again.
* The ceiling (Sm3) omits the corresponding factor.

The frame estimate is conditional on (Avg), which enters Dec♯ through both (Sm3′) and (Sm4).

**scope on Lemma F: holds with the modification F(4′).**

## 4. (Lay-W) and the two-layer geometry of [P] §C

### 4.1 What §C requires of the layers

The following is read in the source (§1), labelled (d) where Interpret.
1. Corollary 3.6 handles a local problem only when the whole local domain lies in **one** (3.35)-class cube, i.e. one gauge with the index-j bound on all of □̃⁵ (p.408: "Ω′₀ ⊂ □ for a cube □ of the class"; p.409: "□̃⁵ is contained in one of the cubes for which this condition holds").
2. The (3.35) class, and its CMP119/LFR I counterparts (2.38), (1.65), (1.67), (1.69), consists by definition of cubes inside **two consecutive layers**, indexed by the finer one (p.396; [III] p.261; [IV] pp.190–191).
3. The local sequence of a walk cube is Bałaban's two-level one inside □̃⁴ (p.408). The operator identity \(\Delta'_aG'_0=I-R'\) (3.88) requires the local level structure to agree with the global one on supp h_□ ⊂ □.

So the containment §C actually uses is
**(2L) □̃⁵ of every walk cube lies in two consecutive layers**, and the walk cube itself in the two layers its local sequence carries. This is additional assumption as a reading, as [N] says.

If □̃⁵ meets the finer layer, the index drops by one and the regularity constant changes by a factor L. That is harmless. What is not harmless is meeting an **unbounded** number of layers, because the single-gauge bound then degrades by \(L^{p-1}\) with p unbounded.

Consider the following layer geometry:
* the exact maximal domains of [III] p.256 in 1D, Ω_n aligned to the global L^nM₁ grid;
* the box boundary at **every** offset on the M₁ grid modulo L^NM₁;
* walk cubes on the global big-block lattice with a block in their own layer.

[N]'s model fixes one alignment, which makes layers up to twice their minimal width. Mine includes the minimal-width cases.

| L | M₁/M_W = 1 | 2 | 3 | 4 | 5 | **6** | 8 |
|---|---|---|---|---|---|---|---|
| 3 | 6 | 6 | 6 | 6 | 3 | **2** | 2 |
| 5 | 6 | 6 | 6 | 6 | 3 | **2** | 2 |
| 13 | 6 | 6 | 6 | 3 | 3 | **2** | 2 |

(Maximum number of layers met by a 5-neighbourhood, N = 4 levels.) Two further results:
* The walk cube itself never meets more than 2 layers. So (2L) for □̃⁵, not the local–global agreement on □, is the binding condition.
* At M₁ = M_W the maximum is 4, 5, 6, 7 for N = 2, 3, 4, 5, for L = 3 and L = 13. It grows with depth.

Analytic form. In level-m units the finer layers have total width \(<M_1L/(L-1)\), while □̃⁵ reaches \(6M_W\) beyond its own layer. So for \(M_1<6M_W(L-1)/L\) a 5-neighbourhood near the outer boundary of its layer crosses **all** finer layers and leaves the box. Conversely, \(M_1\ge6M_W\) keeps it within its own layer and one neighbour, because the finer neighbour is ≥ M₁ wide in level-m units and the coarser one ≥ L²M₁.

**scope: (Lay-W) M_W | M₁, M₁ ≥ 6M_W is a correct sufficient condition. Some condition M₁ ≥ c·M_W with c > (L−1)/L·6 is necessary for (2L).** The formula gives the arithmetic deduction; that (2L) is the containment §C needs is additional assumption.

General form, for any admissible sequence:
> **(Lay-W\*)** Every layer that has a coarser neighbour is at least \(6LM_W\) wide in its own level units.

This holds trivially for main-sequence layers (\(2MR\)) and for Z″ layers (M in level units, since \(M\ge160L^3M_W\)). On box collars it is exactly (Lay-W).

* **The source makes it.**
  * [II] p.3 (source): walk domains are unions of cubes of π_k(1), "of the size M₁".
  * [III] p.245: M₁ is "the size of large cubes for which all the theorems of the previous papers … are valid", and the box collars are 2M₁ wide (p.256).
  * The source's own thin-collar uses therefore rest on the same identification: [III] (3.6)–(3.8) and (3.17)–(3.19) on \(\mathbf B_k(\square^{\sim4})\), and [LFR II] (1.161). For [III] (3.6)–(3.8) and (3.17)–(3.19) this would give R = L in [P2] (2.2), and §C's (2L) fails.
  * (Lay-W) is therefore a **re-reading of the source's constants**: CMP119's M₁ must be at least 6× the [P] big block actually used in §C. [P] Theorem 3.1's threshold (its own "M₁", p.397) bounds M_W from below only, so the re-reading is consistent.
  * B-02's base note (N0 l.218) already makes the analogous separation for CMP102 (1), with native M_v, R_v, M₁ a multiple of M_v and LM₁ > R_vM_v.
* **Local deformation of propagators and the minimizer, Domains of the representation-defined derivatives, T′♯, C-05's ST/Prop. N chain.** These work on the main sequence, with layers ≥ 2MR ≥ 6LM₁ in level units. Domains of the representation-defined derivatives §4 says so explicitly: "layer j−1 has thickness ≥ ML^{j−1}ξ". **Unaffected**, whichever block is called the walk block. The "d, L, M₁" in Local deformation of propagators and the minimizer (W-ms) and Source operators for the deformed reconstruction Theorem S should read "d, L, M_W"; this is cosmetic.
* **CT♯ (The one-sided collar estimate).** Its consumer table covers [III] (3.6)–(3.8), (3.17)–(3.19) and the R^loc "complex (3.19)". All are box problems with M₁-collars, and The one-sided collar estimate's (d) note at l.229 records that the local set occupies a thin strip. For these consumers, (K♯) is applied to sequences that violate (2L) under the identification.
  * Repair: add (Lay-W), and read (Geo) with RM = LM₁.
  * With these, CT♯'s conclusions for these consumers stand at their previous level. **Without them, they rest on an unproved extension of §C.**
  * The same applies to Native-tag admission, trajectory weights and the obstruction to propagation's H′♯ / Corollary HD on old determining sets with M₁-collars (the single-ancestor condition item 1: "(Geo) thresholds for old sets fall on M and M₁").
  * R-01's (190) half (the representation convention) is affected only through these consumers. Same repair.
* **[N] / Dec♯.** (Lay-W) is among Dec♯'s hypotheses. Fine.

None of this breaks a result. It adds one lower bound on a free constant fixed right after d, L, M_W, at every use of (K♯)/(W-ms) on thin-collar sequences.

## 5. Lemma N

**Holds**, at deduction given source input, with the junction at additional assumption, as [N] states.

* **(T).** The box lies in Ω_{k+1} with margin (B5). (2.38)'s top-level clause gives one G-valued gauge on every CM-cube with the level-(k+1) bound. Every [P] class cube of the box sequence has size \(\le12M_W\le CM\) in top units, so it lies in such a cube.
  * The level weights \((L^m\eta)^{-p}\) increase toward finer levels, so the top-level bounds imply (3.35) at every index, and (3.37) and the 𝐉-bound in every layer (monotonicity, deduction).
  * Class cubes of index 0 that stick out of the box are harmless, by [P] p.396: "these regularity conditions do not impose any constraints on U outside the domain Ω₀". additional assumption
* **(R).** (1.65)/(1.67)/(1.69) are two-layer gauge classes of size CML^mη, with level-m bounds on the layers (Ω″_m∖Ω″_{m+1}) and (Ω_m∖Ω_{m+1}). The level-k clause with c = 3 holds on all of Ω_k ∩ X, which contains the B_k(Z)-collar. The factors are bounded by \(\Theta_0=3L_0^{2N_0}\).
  * A 12M_W class cube of index m lies in a CML^m class cube of the same index, provided it can be placed inside Ω″_m. That holds because Ω″_m contains all coarser layers, which are thick.
  * Whether the combined Z″/collar set is an admissible sequence at the junction remains additional assumption, exactly as [N] §7 item 5 says. [IV] p.180 itself only asserts "(1.13) admissible".
* **(3.36)/(3.38).** They are not implied: no space contains second-derivative bounds on A or A′. They are not needed:
  * Theorem 3.4 and Corollaries 3.5–3.6 use (3.35) and (3.37) only (p.396).
  * (3.36) is used at (3.117), to make the error of the non-invariant quadratic form small through J = J(U), and at p.422 for \(H^*J\). With independent 𝐉 and the right form (S-calc♯) (the representation convention: "a definition … no use of symmetry … allowed"), both uses are replaced by the 𝐉-bound of item 3.
  * [N] mentions only the second use. The first is covered by the same convention. source input; additional assumption
* **Small inconsistency.** §2.3 "Consequence" writes Lemma L's ceiling with \(a_0^{\mathbb G}/12\). (Sm1) writes \(a_0^{\mathbb G}\). (Sm1) is the stronger condition, so keep it.

## 6. Theorem Dec♯

**Holds with stated modification, conditional.**.

1. **Domain (item 1).** This is Lemma N; see §5.
2. **Admissibility.** (G-adm) gives (2.1)–(2.2) with \((M,R)=(M_W,LM_1/M_W)\). Only RM = LM₁ enters (2.59) or (2.59′). Whether R = LM₁/M_W ≥ 6L is "big enough" for every use of R in [P2]/[P] beyond Lemma 2.1 and (2L) is additional assumption. [N] §7 item 6 says so.
3. **(Tile), W0(e).** Checked:
   * Bałaban's d in level-m units dominates the π_k tile count for m ≤ k. For the level-(k+1) region of (T) this costs a factor L.
   * Walk domains have diameter ≤ 20M_WL^{k+1} assumed input. So \(M\ge160L^3M_W\) for (T).
   * \(\kappa_{\max}^{\mathbb G}=\delta_0M/(2^{d+6}L^{2+(t-k)})\); Δ_* = 3^d − 1; b₀ = 12.23.
4. **Existence, holomorphy and bounds (item 2).** These come from Source operators for the deformed reconstruction Theorem S with \(\hat B\) and The one-sided collar estimate's (D1)–(D3), as for M♯ in C-05. The proof assumes them (shared premises (U1)–(U6)).
5. **Vanishing (item 4).** With s = 0 off R ∪ T, every walk term meeting a tile outside R ∪ T carries a factor 0, so P(s) splits by *-components (Local deformation of propagators and the minimizer Theorem W(2)).
   * If the component of R misses the datum support, the unique small solution on core(R) is the solution with datum 0, which is 0.
   * The Möbius terms with T non-connected to R vanish because their derivatives act on a component that does not reach core(R).
   * The datum at a collar point depends only on 𝐔 in that point's top block, which lies inside its π_k tile by (Par-c). So Φ_T depends on (𝐔, 𝐉) only through R ∪ T.
   * Correct (deduction; given Theorem W). [N]'s toy is consistent with this.
6. **The uniform tiling** is Bałaban's own (LFR II p.372, Y₀ ∈ D_k, c).

**Modifications.**
* Status should read "conditional on (U1)–(U6), (S-calc♯), (Avg) **through (Sm3′) and (Sm4)**".
* (Sm3) should be replaced by (Sm3′).
* (Lay-W) and (2L) are additional assumption as the reading of §C's needs.

## 7. Theorem A8′

### 7.1 Items 1, 2, 5 — hold at [N]'s level

* **Item 1.** The identification at real configurations uses (1.56) source input and [V] Theorem 1 / Proposition 9 conditional. The datum bound 44d²B₃ε_k is (p.188).
* **Item 2.** This is Dec♯(4) for \(\mathbb G_Z\). The datum lies in \(\mathcal L_Z\subset Z\cap\Omega_k\):
  * where Q^{s*}-data are used (on Z∩Ω_k), the top-level averages agree, so the datum is non-zero only in the B_k(Z)-collar;
  * on Z∩Ω^c_k the component uses the global data, so the datum is 0.

  This is source input; additional assumption, as stated.
* **Item 5.** Labels are unchanged; the chart only reparametrises.

### 7.2 Item 3: the coarsening index m = k

(1.63) (p.189) takes the minimal m with \(X\subset\Omega^c_{m+1}\), with \(\Omega_{k+1}=\emptyset\).
* X contains a tube meeting \(\mathcal L_Z\subset\Omega_k\), so \(X\not\subset\Omega^c_k\) and m ≥ k. Hence m = k.
* The other conditions of (1.63) hold: \(X\cap(Z_{j+1}\setminus Z''_{j+1})\ne\emptyset\) via b ∈ 𝔅_Z, and X ∈ D_k after coarsening.

### 7.3 Item 4: the rate gap — **does not follow as written; repaired**

[N] item 3 lumps everything into \(|W_Z(X)|\le\varepsilon_Ze^{-(1-5\delta)\kappa d_k(X)}\). Item 4 then claims (1.70) for the resulting ℂ-terms, \(|\cdot|\le C\varepsilon_Ze^{-(1+3\beta)\kappa d_k(X)}\). That rate is **higher** than the input rate by the factor \((1+3\beta)/(1-5\delta)\approx1.84\) at β = ¼ (finite comparison.

The first-order contribution of a potential to the cluster expansion is localised on its own domain with its own size. So no expansion can turn \(e^{-(1-5\delta)\kappa d}\) into \(e^{-(1+3\beta)\kappa d}\) for large d. The prefactor ε_Z cannot help either: it is fixed, while d_k(X) ranges up to the volume of the component.

How does the source get (1+3β)κ for its own terms? Not stated on pp.189–192. The natural mechanism is the coarsening gain (native scale j′ < m gives a factor \(L^{m-j'}\) in linear size). That gain is **absent** for W_Z: X is already a D_k domain, at m = k. [N]'s (Clu-R), "accepts additional potentials bounded by ε times the source bounds (with κ → (1−3δ)κ) and yields … (1.70) multiplied by O(ε)", thus asserts a rate gain that the source supplies at most for its own coarsened terms. As a reading it is stronger than anything on the page.

**Repair.** Keep the structure that [N]'s own proof produces, and do not lump the rates. Put \(c_T:=(1+3\beta)\kappa/(1-3\delta)\). For a source domain Y of (S9-R), write \(d^\flat_k(Y)\) for the scale-k linear size of the smallest D_k domain containing Y, and \(\mathfrak b_V(Y):=C_Vp(g_j)^2|Y|^2e^{-(1-2\delta)\kappa d(Y)}\) for its source bound.

> **Item 3′ — conditional on Dec♯, (S9-R), (Geo-Z).** Assume in addition
> \[
> \tfrac12\kappa_1\ \ge\ \sqrt d\,c_T=\sqrt d\,(1+3\beta)\kappa/(1-3\delta),\qquad \kappa_1\ge4(1+b_0).
> \]
> Then \(\mathscr V_Z=\sum_Y\sum_XW_Z(X;Y)\), with X ∈ D_k as in [N] item 3 (index m = k). Each \(W_Z(X;Y)\) has [N]'s locality, analyticity, covariance and vanishing properties, and
> \[
> \sum_X|W_Z(X;Y)|\,e^{c_T\,(d_k(X)-d^\flat_k(Y))}\ \le\ \hat x_Y e^{\hat x_Y}\,\mathfrak b_V(Y),\qquad \hat x_Y:=C\,|Y^*|\,\ell_k^q\,(g_k/g_j)\,e^{c_T(\sqrt d+1)}e^{-\frac14\kappa_1n_Z}.
> \]
> *Proof.* [N]'s own inequality gives \(d_k(X)\le d^\flat_k(Y)+1+\sqrt d\sum_i(|T_i|+1)\). Then
> \[
> e^{c_T(d_k(X)-d^\flat_k(Y))}\le e^{c_T}\prod_ie^{c_T\sqrt d}e^{\frac12\kappa_1|T_i|}.
> \]
> The tube sums with weight \(e^{\frac12\kappa_1|T|}\) are bounded by (3.1♯) \(\le eA_Ze^{-\frac14\kappa_1n_Z}\). The power-series step of [AU] §4.2 with \(\rho_H=\frac12g_j\) gives \(\hat x_Ye^{\hat x_Y}\). \(\square\)
> **(Clu-R′) — additional assumption.** The source's estimation of (1.60) ([IV] pp.189–192) yields (1.70) for the ℂ-terms generated by the source potentials V(Y). It then also yields (1.70), with C₀ replaced by \(C\sup_Y\hat x_Ye^{\hat x_Y}\), for the ℂ-terms generated by additional potentials satisfying item 3′ with \(c_T\ge(1+3\beta)\kappa/(1-3\delta)\).
> *Why this is the right reading.* Enlarging a term from \(Y^\flat\) to X costs \(e^{-c_T(d_k(X)-d^\flat_k(Y))}\), which is faster than any rate the output needs, so the enlargement is free. What remains is the source's own rate for Y. The reading claims nothing about W_Z beyond what the source claims for V(Y).
> **Item 4′.** Under (Clu-R′) and **(Par-g_Z′)** \(C\sup_Y\hat x_Ye^{\hat x_Y}\le g_j^{\kappa_0+2}\), the conclusion of [N] item 4 holds: (1.70) with \(C_0\to Cg_j^{\kappa_0+2}\le g_j^{\kappa_0}C_0\). (Par-g_Z′) is a coupling ceiling of the same type as (Par-g_Z), since \(n_Z\gtrsim R_k\).

[N]'s lumped bound remains true. It is just not the form that (1.70) can be checked against.

**A doubt about the source, recorded rather than resolved additional assumption.** For source potentials of native scale k meeting 𝔅_Z (B^{(k)}-terms with large D_k domains), the source's own (1.70) at (1+3β)κ has no visible coarsening gain either. Any form of (Clu-R) inherits whatever the source does there. A8′ in the repaired form is no worse than the source.

### 7.4 (Geo-Z) — additional assumption, better supported than [N] says, with one misattribution

* [N]'s j ≤ k−2 argument cites [III] p.256 for dist(Ω^c_{k−1}, Ω_k) ≥ 2MR_{k−1}. The quoted sentence is about ∂Ω_j and ∂Λ_j of the **same** index.
* The Euclidean reading is instead supported by:
  * [IV] p.177 (source): "Each renormalization step adds at least ten layers of MR_k-cubes". Layers of cubes are Euclidean thickenings.
  * (1.57)'s exponent, which is a sum of exactly such layer widths: 10MR_i per intermediate step and MR_k at step k.
* Bałaban's d dominates the Euclidean T^{(k)} distance. So a large d alone would *not* imply a long Euclidean tube. The p.177 sentence is what closes that.
* [N]'s \(c_Z=2/L^2\) is conservative. Keep (Geo-Z) at additional assumption, citing p.177 and (1.57).

### 7.5 "With Dec♯ the amendment needs CT♯ for none of its new uses", conditional

* [RD]'s uses U1–U4 are covered:
  * U1, U2: Lemma 3.2(1)–(2) and Lemma 4.1, via (3.1♯) with the real datum or with Lemma D;
  * U3: real local minimiser, same mechanism;
  * U4: \(\mathbb H^{(j)}_Z\) via A8′ item 2.
* U5 is the source's own (3.6)–(3.8), (3.22). It is not new and still uses CT♯ or (P-190), now with (Lay-W) (§4.3).
* The rate (CD-T) delivers per unit collar distance is about \(\frac14\kappa_1L/M\le\delta_0/(2^{d+8}L^2)\). That is far below the source's δ. It suffices because every consumer needs only \(e^{-cR}\) with some c > 0 and absorbs \(\hat B^2\) by a ceiling (Par-g′).
* Dec♯ and CT♯ both rest on (U1)–(U3), i.e. [P] Theorems 3.1–3.3 and 3.7–3.10. "No CT♯" does not mean "no shared source premise".

**scope on A8′: holds with the modification 3′/4′ and the condition ½κ₁ ≥ √d(1+3β)κ/(1−3δ).**

## 8. Order of constants, and B-02

**Order.** The order is
d, L → M_W (≥ [P]'s threshold) → M₁ ((Lay-W), (Geo-α) or its Lemma 2.1′ form, B-02's LM₁ > R_vM_v) → M₂ = L²M₁ → κ (Bałaban's localisation decay) → κ₁ → M → C₀, C₁ → g-ceilings.
* **κ₁ is bounded below** by 4(1+b₀) = 52.9 (d = 4, uniform tiling) and by \(2\sqrt d(1+3\beta)\kappa/(1-3\delta)\) (Lemma W and A8′ 3′).
* **κ₁ is bounded above only** by \(\kappa^{\mathbb G}_{\max}=\delta_0M/(2^{d+6}L^3)\), and M is chosen after κ₁.
* M has further lower bounds only: \(160L^3M_W\), \((L+8)M_2\), and C-05's \(2^{d+6}L^2\kappa_C/\delta_0\) for its own decoupling parameter.
* κ is a source constant fixed before M ([III] p.260: κ₀ "can be chosen arbitrarily large, similarly as κ, if the other parameters are fixed properly"). Nothing bounds κ by M or κ₁.
* All ceilings (Sm1), (Sm2), (Sm3′), (Sm4), (Par-g), (Par-g_Z′) involve g last.
* **No circularity.**

**Numbers.** [N] §4, its finite comparison and the walk-block conditions item 7 use κ₁ = 52.9. For d = 4, β = ¼, the second lower bound \(7\kappa\) dominates as soon as κ > 7.6 (finite comparison:

| κ | κ₁ ≥ | δ₀M ≥ (L = 2) | δ₀M ≥ (L = 13) | log B̂ ≥ |
|---|---|---|---|---|
| 5 | 52.9 | 4.3·10⁵ | 1.2·10⁸ | 847 |
| 10 | 70 | 5.7·10⁵ | 1.6·10⁸ | 1120 |
| 20 | 140 | 1.2·10⁶ | 3.2·10⁸ | 2240 |
| 33 | 231 | 1.9·10⁶ | 5.2·10⁸ | 3696 |

Even at κ = 33, M = 13⁸ = 8.2·10⁸ works for δ₀ ≥ 0.64. These are constants only, but the recorded "M ≥ 1.2·10⁸/δ₀" and "log B̂ ≥ 847" are lower bounds valid only for κ ≤ 7.6.

**Parameter constraints for B-02.**
* The B-02 base note (Port l.7) fixes the native \(M_v,R_v\) and "a sufficiently large L-power M₁ divisible by M_v with LM₁ > R_vM_v", then \(M_2\), then "M = L^u sufficiently larger". N0 l.218 explicitly warns against "reusing the same letter for two block constants".
* So (Lay-W), (Geo-α) / Lemma 2.1′, (Tile) and the κ₁-driven bound on M are **compatible**: all are lower bounds on constants that B-02 leaves free ("sufficiently large").
* There is no identified upper bound on M₁, M or κ₁ in B-02's evidence. The order of constants is specified above; no upper bound on M₁ or M appears.
* B-02's re-verification needs only to add the new lower bounds and the divisibility M_W | M₁.

## 9. Prop. 5.3′ and TC Theorem 5.1 for the final construction

**Prop. 5.3′, conditional.**
* The R^loc label reads data within \((L+8)LM_2R_{n+1}\le LMR_{n+1}\) (Par-M).
* The (A8) label reads only data in the eligible component, a cube of side 100MR_n. That includes all earlier preparatory stages, since \(U^{(n+1)}_{k,Z}\) is built from data in Z ((1.20), source).
* Eligibility needs only a bounded exploration and N steps of history ([IV] p.177).
* (A5′)/(A8′) change no label, so item 2 is right.
* The cumulative range is a geometric sum by (G5).

**Theorem 5.1.** It is an implication from its inputs, and as such it holds as written. Here is which inputs depend on the construction, and how the amendment affects them:

| Input | Depends on the construction? | Under 𝒞^fin |
|---|---|---|
| (FP) | yes | Prop. 5.3′ conditional |
| (C1) / (Cov) | yes | Amended rules covariant with odd L and common centre planes ([AU] §3.4, c\*). The **localised new terms** must also be covariant, because the R′ kernels of LFR II (1.100)–(1.102) are built from the effective densities. This needs covariant choices of 𝒟, h_□ (Dec♯ item 3). It is achievable: reflections through big-block centre planes map big-block vertices to vertices. Not "unchanged", as [N]'s Lemma 1.1 row says, but holds. deduction; additional assumption |
| Lemma 1.1 | via kernel covariance | as for (C1) |
| Lemma 4.1 (RP of the lift) | via the structure of the lift | Unchanged: the charts are deterministic and Haar-preserving, and the labels are deterministic. deduction given TC |
| (J_U) = (T_U) + (M)/(RD)/(S)/(G-R) | yes, through the inductive bounds on the effective action and the large-field factors | Holds to the extent the amended action satisfies the source's inductive bounds, i.e. conditional on [RD] Theorem 4.5 and **A8′ item 4′** (§7.3). Per-cube factors: on R^loc-flagged cubes, \(t^2\to(t-2\eta)^2\ge t^2/4\). This lowers the per-cube **lower** bound, so the constant that changes is TM §4.4's \(C_{\rm fat}\to4C_{\rm fat}\), not \(C_\square\) or \(C_1\) as [N] writes. The net effect θ → θ/4 is the same. |
| (G1), (G4), (G5), (G6) | geometric | unchanged |
| (G2), (G3) | label structure | Unchanged in form. (G3) is helped: the preparatory failure label is component-local. |
| FILS chessboard | no | external theorem |

TC §1.4's per-tile condition \(2p_0>dr+1\) is unchanged, since only constants move.
