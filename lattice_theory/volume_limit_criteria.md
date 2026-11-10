# Infinite-volume criteria for local distributions

Labels: **(P)** proved here, **(L)** proved in the literature with citation, **(C)** conditional on a precisely stated hypothesis, **(O)** open. "The source construction" is the original Wilson-source construction; its pages are cited as printed pages of the [source estimates](source_estimates/README.md). Other locators refer to the following notes in this collection: [ND] = [Nonlinear dispersion and unequal spatial weights](block_and_transfer/conditional_estimates/nonlinear_dispersion_and_unequal_spatial_weights.tex); [PW] = [Physical Wilson contacts and local conditional subtraction](block_and_transfer/conditional_estimates/physical_wilson_contacts_and_local_conditional_subtraction.tex); [OS] = [Ordinary spectral estimates and mixed current transfer](block_and_transfer/conditional_estimates/ordinary_spectral_estimates_and_mixed_current_transfer.tex); [SR] = [Spatial reduction and uniform-source holonomy means](block_and_transfer/conditional_estimates/spatial_reduction_and_uniform_source_holonomy_means.tex).

**Conventions.** Torus T = (R/TZ)^4 with lattice spacing a, Wilson measure dmu = Z^-1 exp(−beta S) dHaar, S = sum_p s(U_p), 0 <= s <= s_max, beta = beta_a on the asymptotically free trajectory (volume-independent by construction). p_{a,T} = Vol(T)^-1 log Z_{a,T}. Reference torus T_* of side t_* (fixed, compatible), T = qT_*, n = t_*/a, M = q^4. For a source J coupled to a local gauge-invariant lattice observable, Z_{a,T}[J] and p_{a,T}[J] are the sourced partition function and pressure.

---

## 1. The precise theorem needed for item 6

**Theorem 6 (target).** Let O_1, ..., O_r be the renormalized gauge-invariant local observables of the construction (the smeared action density Tr F^2 or the H family of the source construction), with volume-independent local counterterms. There exist a Schwartz-type norm ||.||_s, constants C, beta_0 and a cell size l_c, all independent of a and T, such that for every compatible torus T with side >= 2 l_c and all test functions f_1, ..., f_m:

  (U)  |< O_{i_1}(f_1) ... O_{i_m}(f_m) >_{a,T}|  <=  C^m (m!)^{beta_0} prod_j ||f_j||_s .

Given (U), the following are consequences:

(a) **Compactness (P, elementary).** For each fixed m the set {S_m^{a,T}} is bounded in the dual of a Banach space of test functions; by Banach–Alaoglu and a diagonal argument over m there are sequences a_j -> 0, T_j -> infinity along which all S_m^{a_j,T_j} converge weakly to tempered distributions S_m. (Weak-* compactness of bounded sets in the dual of a separable space.) Joint subsequences in (a,T) are taken; no interchange of limits is needed, see Section 6.

(b) **Properties that pass to the limit (P, elementary).** Symmetry (E3) and reflection positivity (E2) are finite systems of linear equalities / inequalities among finitely many S_m tested on finitely many test functions, hence closed under weak convergence; RP with respect to the reflection in the plane x_0 = 0 holds at every (a,T) for lattice site-planes (Osterwalder–Seiler), and the limit inherits it. Invariance under translations by a_j Z^4 for all j gives invariance under a dense subgroup; continuity of translations on tempered distributions gives invariance under R^4. Hypercubic symmetry passes. Full O(4) covariance is item 7, not addressed here.

(c) **OS reconstruction without clustering (L).** Osterwalder–Schrader, CMP 42 (1975) 281–305, Theorem (E0', E1, E2, E3 => Wightman theory): the reconstruction from Schwinger functions satisfying temperedness with the linear growth condition E0', Euclidean covariance E1, reflection positivity E2 and symmetry E3 yields a Hilbert space, a positive-energy representation of the Poincaré group, and Wightman fields; the cluster property E4 is equivalent to uniqueness of the vacuum and is **not** needed for the reconstruction. (OS II, Sections II and IV, and OS I CMP 31 (1973), Remark 3 p. 89; the source construction records exactly this subset implication at printed p. 488.) The exponent beta_0 and the norm in (U) must be matched to the E0' condition of OS II when the final statement is written; the chessboard route below produces beta_0 = 1 with a C^5-type norm summed over cells, which is of the E0' form, but the identification of the index must be checked against OS II's statement (flagged in Section 6).

(d) **Pure phases (L, as read in the source construction; primary text not verified here).** Driessler–Summers, Helv. Phys. Acta 59 (1986) 331–348, Theorem 2.3: for a Hermitian scalar Wightman field with possibly degenerate vacuum, under a generalized energy bound for test functions with compact Fourier support, the central decomposition of the vacuum state has, almost everywhere, Wightman components satisfying clustering and vacuum uniqueness; Poincaré covariance of the components is the subject of Driessler–Summers, Ann. IHP 43 (1985) 147–166 (absence of spontaneous breaking of the Lorentz group). The source construction reads the 1986 theorem at printed p. 467 (§69.3) and applies it at printed p. 488 (§74), supplying the energy-bound hypothesis from its own (EP5)/(SC3). The hypotheses as stated there are not checked here against the original and must be before anything is claimed.

So: **existence does not require uniqueness of the infinite-volume limit nor the cluster property**, provided (i) the limit points satisfy E0'–E3, (ii) the energy-bound hypothesis of Driessler–Summers holds, and (iii) a separate argument shows that some component is non-trivial. Point (iii) is genuinely open and is discussed in Section 6: the decomposition theorem is silent on triviality; a component can be a constant field or a generalized free field.

**What item 6 therefore requires is (U) uniform in a AND T.** Everything else in this item is standard once (U) holds.

---

## 2. The reduction chain

### 2.1 Chessboard estimate on the torus (L)

Partition T into cells of side l_c with an even number n_T of cells per direction, cell faces on lattice site-planes. The Wilson measure is reflection positive with respect to every lattice site-plane and every mid-plane in every coordinate direction (Osterwalder–Seiler, Ann. Phys. 110 (1978) 440–471, Theorem on RP for the Wilson action; plaquettes lying in the reflection plane are split as e^{−beta s/2} e^{−beta s/2}). For functions F_c each measurable with respect to links strictly inside cell c (margin from faces), the multiple-reflection (chessboard) estimate reads

  (CB)  |< prod_c F_c >_{a,T}|  <=  prod_c < prod_{c'} theta_{c->c'} F_c >_{a,T}^{1/n_T^4},

where theta_{c->c'} is the composition of face reflections carrying c to c' (with complex conjugation in odd cells). Reference: Fröhlich–Israel–Lieb–Simon, CMP 62 (1978) 1–34, Theorem 2.2 and the torus version in Glimm–Jaffe, *Quantum Physics*, 2nd ed., Theorem 10.5.4 (multiple reflection bounds) and the chessboard estimate of Section 10.5. For F_c = exp(J_c . O) with J_c a source supported in c, the replicated expectation is a ratio of partition functions:

  (CB')  < prod_{c'} theta F_c >_{a,T} = Z_{a,T}[W J_c] / Z_{a,T}[0] = exp( Vol(T) ( p_{a,T}[W J_c] − p_{a,T}[0] ) ),

with W J_c the source reflected (and conjugated in odd cells) into all cells. This is the first inequality in (S95) of the source construction, printed p. 619. **Status: (L).** Nothing here depends on a or T except the requirement n_T even and the margin.

### 2.2 RP subadditivity across tori (P, using L)

**Lemma 2.2.** For T = qT_* and any cell-replicated source W J (including J = 0):

  Z_{a,T}[W J]  <=  Z_{a,T_*}[W J]^{q^4},   equivalently   p_{a,T}[W J]  <=  p_{a,T_*}[W J].

*Proof.* Fix direction 1. Let n_* (even) be the number of cells of T_* per direction. The Wilson measure with the replicated source on the torus T_1 x Sigma (Sigma the transverse three-torus, any sides) has a positive, self-adjoint, trace-class transfer operator in direction 1 (Lüscher 1977; Osterwalder–Seiler 1978; [PW, Lemma 8.1] proves positivity and trace class for the pure Wilson case with gauge projection: T = M_b C_beta M_b with C_beta a positive-definite convolution kernel). The source term is a sum of cell-local terms; the transfer operator across one cell period is an operator A, and the reflection-plus-conjugation structure of W J makes the next cell's operator A^*. Hence Z_{T_1 x Sigma}[W J] = Tr( (A A^*)^{n_1/2} ) with n_1 the number of cells in direction 1 (n_1 even). With mu_i >= 0 the eigenvalues of the positive trace-class operator P = (A A^*)^{n_*/2},

  Tr P^q = sum_i mu_i^q  <=  ( sum_i mu_i )^q = (Tr P)^q,

since (sum mu_i)^q expands into a sum of nonnegative terms containing sum mu_i^q. This gives Z_{(qt_*) x Sigma} <= Z_{t_* x Sigma}^q. Apply it successively in the four directions, each time on the torus obtained so far (RP of the Wilson measure holds on every torus with respect to every coordinate direction): Z_{(qT_*)^4} <= Z_{T_* x (qT_*)^3}^q <= Z_{T_*^2 x (qT_*)^2}^{q^2} <= ... <= Z_{T_*^4}^{q^4}. QED.

For J = 0 this is **p_{a,qT_*} <= p_{a,T_*}** (direction checked: the larger torus has the smaller pressure). It is (SV14) of the source construction, printed p. 633, and the second inequality in (S95). Note the direction of what S94 asks: the **reverse** inequality up to a constant.

### 2.3 Splitting the sourced pressure difference (P)

From (CB), (CB') and Lemma 2.2, for a source J in one cell of T:

  |Z_{a,T}[J]/Z_{a,T}[0]|  <=  ( Z_{a,T}[W J]/Z_{a,T}[0] )^{1/n_T^4}
                           <=  ( Z_{a,T_*}[W J]^{q^4} / Z_{a,T}[0] )^{1/n_T^4}
                            =  exp( l_c^4 [ (p_{a,T_*}[W J] − p_{a,T_*}[0]) + (p_{a,T_*}[0] − p_{a,T}[0]) ] ),

using n_T^4 = Vol(T)/l_c^4. The first bracket is the **reference-torus sourced pressure bound**; the second is **S94** (in its pressure form, [ND, (7.2)] and (SV3)–(SV4) at printed p. 630). This is (S96) of the source construction, printed p. 619. **Status (P)**, given (L) for CB. For m sources in m distinct cells the same argument gives the product of m such factors; for several insertions in one cell their product is the cell insertion.

### 2.4 From sourced bounds to (U) (P, modulo the reference-torus bound)

Suppose, for complex sources with ||J_c||_{C^5} <= r_0 supported in a cell with margin, the reference-torus bound

  (RT)  p_{a,T_*}[W J] − p_{a,T_*}[0]  <=  C_1   uniformly in a,

in the renormalized form of (S92) of the source construction, i.e. with the local counterterm functional L_a(J) (additive over cells with margins, (S93) at printed p. 619) absorbed; and suppose S94. Then for sources J_1, ..., J_m in m cells, lambda_j in the polydisc |lambda_j| <= r_0/||J_j||_{C^5},

  | e^{−L_a(sum_j lambda_j J_j)} Z_{a,T}[sum_j lambda_j J_j] / Z_{a,T}[0] |  <=  exp( m l_c^4 (C_1 + C_0) ).

The multivariable Cauchy estimate gives, for the renormalized connected and full Schwinger functions (derivatives at lambda = 0),

  |S_m(J_1, ..., J_m)|  <=  exp( m l_c^4 (C_1 + C_0) ) prod_j ( ||J_j||_{C^5}/r_0 ),

with an extra k! when k insertions share a cell (one-variable Cauchy of order k). Decomposing an arbitrary test function with a smooth partition of unity subordinate to the cells and summing, |S_m(f_1, ..., f_m)| <= C^m m! prod_j ||f_j||_s with ||f||_s = sum_c ||f chi_c||_{C^5}, which is dominated by a weighted Schwartz norm. This is (U) with beta_0 = 1. **Status: (P)** given (RT) and S94. The m! comes only from coincident cells; the exponent could be improved but is not needed.

**Summary of the chain:**

  (U)  <==  (RT) [small torus, fixed volume, with sources: items 1–2, status (C)]  +  S94 [status: see 2.5–2.6]  +  (CB),(L).

### 2.5 S94 is a pressure comparison, and only one side is missing (P)

With the stability input | log Z_{a,R} − V_{a,R} | <= C_st Vol(R) on both tori (S74–S81 of the source construction, first inequality of (S102)), S94 is equivalent up to 2 C_st to p_{a,T_*} − p_{a,qT_*} <= C ((SV3)–(SV4), printed p. 630; [ND, (7.2)]). By Lemma 2.2 the difference is >= 0. So S94 is exactly: **the pressure does not drop by more than O(1) when the torus is enlarged**, uniformly in a.

### 2.6 The reduction of S94 to a one-sided stability statement at a fixed physical scale (P given hypotheses)

This reduction is referred to below as (iv). Let l_0 be a fixed physical length (small enough that the running coupling g(l_0) is small), L the block ratio, K = log_L(l_0/a) the number of RG steps from spacing a to spacing l_0; K depends on a, not on T.

**Hypothesis UB(T_*).** There is a number E_vac(a) (depending on a, g_0(a), l_0, L, not on the torus) and C_+ (independent of a) with

  log Z_{a,T_*}  <=  − Vol(T_*) E_vac(a) + C_+ Vol(T_*).

**Hypothesis LB(T).** With the same E_vac(a) and C_− independent of a and T, for every compatible T >= T_*:

  log Z_{a,T}  >=  − Vol(T) E_vac(a) − C_− Vol(T).

**Proposition 2.6 (P).** UB(T_*) and LB(T) imply S94 with C_0 = C_+ + C_− + 2C_st, and moreover |p_{a,T} + E_vac(a)| <= C_+ + C_− for every T >= T_*.

*Proof.* p_{a,T_*} − p_{a,T} <= (−E_vac + C_+) − (−E_vac − C_−). The two-sided statement for T follows from Lemma 2.2: p_{a,T} <= p_{a,T_*} <= −E_vac + C_+. QED.

Two remarks that sharpen (iv). First, **no bound on the large torus from above is needed** (that direction is free by RP). Second, **no bound on the small torus from below is needed**. So the volume-uniform input is a *lower* bound on Z_{a,T}, and a lower bound on a positive integral can be obtained by restricting the domain of integration. This is where the large-field problem disappears from the volume-uniform part:

**Proposition 2.7 (P): LB(T) follows from a small-field-only statement.** Let the block-spin RG be implemented as in Balaban (block averaging with positive kernels, fluctuation integrations at scales l_1 < ... < l_K). Insert at each step k the characteristic function chi_k of the small-field event for the fluctuation field (and, at the last step, chi_K for the coarse field U_K). Since every factor of the integrand (Boltzmann weights, Haar measures, averaging kernels) is nonnegative,

  Z_{a,T}  >=  Z^{sf}_{a,T} := integral with all chi_k inserted = ∫ dU_K chi_K(U_K) rho^{sf}_{K,T}(U_K).

Suppose (hypothesis SF below) that on {chi_K = 1}

  rho^{sf}_{K,T}(U_K)  >=  exp( − Vol(T) E_vac(a) − g_K^{−2} S_K(U_K) − C Vol(T) l_0^{−4} ),

with S_K a nonnegative local action at spacing l_0 (Wilson-like with coupling g_K = g(l_0), or any nonnegative local functional) and C independent of a, T. Then, restricting to the Haar-set B = {U_K : every link within delta of 1} ∩ {chi_K = 1}, on which S_K(U_K) <= C' delta^2 Vol(T) l_0^{−4} and whose Haar measure is >= exp(−C'' Vol(T) l_0^{−4}) (a product of 4 Vol(T)/l_0^4 link balls, each of fixed Haar volume),

  Z_{a,T}  >=  exp( − Vol(T) E_vac(a) − [C + C' delta^2 g_K^{−2} + C''] Vol(T) l_0^{−4} ),

which is LB(T) with C_− = (C + C' delta^2 g_K^{−2} + C'') l_0^{−4}. QED.

This is the "elementary pointwise-density argument" of (iv): at spacing l_0 the degrees of freedom per unit physical volume are bounded (4 dim G / l_0^4) and the coarse variables are compact, so the crude lower bound is extensive with an a-independent constant. No seam argument is needed, and no mass gap: compactness of the group plays the role that the mass mu-bar = 1 plays in the final step of Dimock's scalar treatment (arXiv:1304.0705, Section 2, "The mass mu-bar_N = mu-bar = 1 will enable us to control the final integral").

**Hypothesis SF (the exact remaining volume-uniform input).** Stated in Section 3 as Theorem A. It is a statement about the *small-field sector only* of Balaban's RG, run K steps on an arbitrary torus, with volume-independent vacuum-energy extraction.

**Hypothesis UB(T_*)** is Balaban's ultraviolet stability on a fixed torus (upper half), with E_vac(a) the small-field counterterm. Stated in Section 3 as Theorem B. It uses the large-field R-operation, but only at fixed volume T_*, which is the published setting.

### 2.7 Volume-independence of E_vac(a) from locality (P for the Gaussian part and for the wrapping sum; C for the nonlinear local coefficients)

In a block-spin scheme the constant term extracted at step k is of the form Vol(T) e_k^{(T)} with e_k^{(T)} = (Vol^{-1}) [ log of a Gaussian normalization on T + the field-independent part of the local effective action on T ].

(a) **Gaussian part (P, in the source construction).** For a finite-range matrix on a periodic lattice with uniform singular-value bounds, log |det| has a convergent walk expansion whose density at a root is a sum over closed walks within distance 2kR of the root ((V6.7)–(V6.8), printed p. 815), and rooted walks of length < n/(4R) lift injectively between the tori of n and qn cells, so the densities agree except for terms of order rho^{n/4R} ((V6.9)–(V6.10), printed p. 815; here n = t_*/l_k in current-scale cells). Hence e_k^{(T_*)} − e_k^{(T)} = O(l_k^{−4} e^{−c t_*/l_k}) for the Gaussian part.

(b) **Nonlinear local coefficients (C).** The field-independent part of the effective action at step k is a sum over polymers X of local activities; activities of polymers that do not wrap either torus are equal on the two tori when the local recipe is natural under copying ([OS, Proposition 8.1]: exact conjugacy of all copied typed factors). Wrapping polymers at scale l_k on T_* have total weight <= C Vol(T_*) l_k^{−4} e^{−c t_*/l_k} if the activities decay exponentially in the polymer tree length. That decay is the cluster-expansion output.

(c) **Summing the wrapping defects (P).** Define E_vac(a) := sum_{k<=K} e_k^{(infinite volume)} (or the T_*-values; the difference is the same sum). Then, with l_k = L^k a <= l_0 <= t_*/2 and x_k = t_*/l_k >= 2,

  sum_{k<=K} l_k^{−4} e^{−c t_*/l_k} = t_*^{−4} sum_k x_k^4 e^{−c x_k} <= t_*^{−4} sum_{j>=0} (2L^j)^4 e^{−2c L^j} = C(L,c) t_*^{−4},

uniformly in a (the sequence x_k is geometric, so the sum is dominated by a convergent series independent of where it starts). Thus the torus-dependence of the extracted vacuum energy is O(t_*^{−4}) per unit volume, which is admissible in S94. **Note:** in the one-sided scheme of Proposition 2.6 one may simply *define* E_vac(a) by the T_* recursion and verify LB(T) with that definition; then only the wrapping polymers on T (side >= t_*) enter, and they are controlled by the same sum.

(d) **Zero modes and holonomies.** Flat coarse fields with nontrivial holonomy around the cycles of T are coarse-field configurations U_K at spacing l_0 with trivial plaquettes; they are integrated with Haar measure in the crude step of Proposition 2.7 and never enter E_vac(a). On T_* they are among the configurations handled by Balaban's large-field analysis at fixed volume. The massless global modes of the continuum theory contribute at most O(log Vol) to log Z (a finite-dimensional sector), which is negligible against Vol. The fluctuation integrals at step k are nondegenerate because block averaging supplies an effective mass of order l_k^{−1} (Dimock 1108.1335, remark after (343): "the averaging operator a_k Q_k^T Q_k supplies an effective mass"); this is what makes the fluctuation covariances exponentially decaying at scale l_k and is the mechanism behind (a)–(c).

### 2.8 Where (iv) would break, if it breaks

The chain 2.6–2.7 is correct as a reduction. It breaks only if **Theorem A (Section 3) fails**, i.e. if Balaban's small-field cluster expansion at a fixed step K cannot be made uniform in the torus size, or if its vacuum-energy extraction is intrinsically volume-dependent beyond wrapping tails. The explicit scalar analogue is volume-uniform (Dimock 1108.1335 Theorem 1: "for all M, N", counterterms depending on N only; 1304.0705 Corollary 1: constant "independent of M, N"). But the primary statements in Bałaban's gauge papers are not verified here (Section 7), so Theorem A remains **(C)**.

---

## 3. The exact remaining lemmas, as theorems with hypotheses

**Theorem A (volume-uniform small-field RG to a fixed physical scale; status (C)).** Fix L >= 2, a physical scale l_0, and a block-spin transformation of Balaban type (gauge-covariant block averaging with positive kernels, axial-type gauge fixing inside blocks, fluctuation integration). Let g_0(a) run on the asymptotically free trajectory normalized so that g(l_0) = g_K is a fixed small number. There exist constants C, c, delta_0 > 0 and, for each a, a number E_vac(a), such that for every compatible torus T of side >= 2 l_0 and K = log_L(l_0/a):

(A1) [positivity] Z_{a,T} >= ∫ dU_K chi_K(U_K) rho^{sf}_{K,T}(U_K), where rho^{sf}_{K,T} is the density obtained by inserting the small-field characteristic functions chi_1, ..., chi_K at every step (trivial from positivity of the integrand, once the transformation is fixed);

(A2) [small-field lower bound, uniform in T] on {chi_K = 1}: rho^{sf}_{K,T}(U_K) >= exp(−Vol(T) E_vac(a) − g_K^{−2} S_K(U_K) − C Vol(T) l_0^{−4}), with S_K >= 0 a local functional at spacing l_0 bounded by C' Vol(T) l_0^{−4} when all links of U_K are within delta_0 of the identity;

(A3) [volume-independence] E_vac(a) does not depend on T.

Correspondence with Balaban: (A2) is the output of "Renormalization group approach to lattice gauge field theories I" (CMP 109 (1987) 249–301: generation of the localized effective actions in the small-field approximation, coupling renormalization, running coupling recursion) together with "II. Cluster expansions" (CMP 116 (1988) 1–22: the fluctuation-integral cluster expansion, Lemma 2 (1.41)–(1.43), activity and connected bounds (2.38)–(2.41), as located in the source construction, printed p. 620). The source construction, §32.5 (printed p. 213), already states bounds of exactly this type at a "fixed retained resolution" citing [8, Theorem 1] = "Large field renormalization II" (CMP 122 (1989) 355–392) Theorem 1, but on a fixed torus. What must be checked in the primary text: that the constants in CMP 109/116 are independent of the number of blocks (the torus side), and that the vacuum-energy extraction (the field-independent term of the effective action) is defined by a recursion that does not see the torus size except through wrapping polymers. Both are properties a cluster expansion is designed to have; the scalar model version is explicit (Dimock 1108.1335 Theorem 1; 1304.0705 Theorem 2 and Corollary 1).

**Theorem B (fixed-volume upper stability with the small-field counterterm; status (L) modulo scope check).** For the fixed reference torus T_* (side t_* small enough that Balaban's hypotheses on the running couplings hold on T_*), log Z_{a,T_*} <= −Vol(T_*) E_vac(a) + C_+ Vol(T_*) uniformly in a, with the same E_vac(a) as in Theorem A. This is the upper half of Balaban's ultraviolet stability (LFR II Theorem 1, whose abstract states that the paper "completes the proof of ultraviolet stability for four-dimensional pure gauge field theories, as formulated in Theorem 1"; the zbMATH review adds that the main theorem assumes effective couplings in an interval ]0, gamma] with gamma small). Scope to check: (i) Balaban's E_vac is the accumulated small-field vacuum energy (it is, in the scheme: the large-field terms are bounded relative to it); (ii) his theorem runs all K(a) steps, so his counterterm is sum_{k<=K(a)} e_k, which differs from the Theorem A counterterm sum_{k<=K} e_k by sum_{K<k<=K(a)} e_k = O(l_0^{−4}) (vacuum energy generated between scales l_0 and t_*), an a-independent constant; (iii) the torus T_* must be in the range of his theorem. Alternatively run only K steps on T_* and use his step-K representation with large fields at fixed volume.

**Corollary (P).** Theorems A and B imply S94 (Proposition 2.6), hence, with the reference-torus sourced bound (RT), the uniform bound (U) (Section 2.4), hence item 6 up to the standard OS/Driessler–Summers steps and the non-triviality question. **Item 6 therefore reduces to: Theorem A (volume-uniform small-field RG, no observables, no large fields) + Theorem B (published, fixed volume) + (RT) (items 1–2 with observables, fixed volume T_*) + item 7.**

The form of stability needed, answering (iv) precisely: an **integrated, one-sided** form suffices. Pointwise two-sided bounds on the full density rho_K on the large torus are not needed; what is needed is a pointwise *lower* bound on the small-field-restricted density on the small-field set (A2), and an *integrated upper* bound on the fixed small torus (Theorem B).

---

## 4. What the source construction already contains for each node

| Node | Material in the source construction | Status |
|---|---|---|
| (CB) chessboard, (CB') replicated partition functions | (S95) first inequality, printed p. 619; §10 "matching partition powers and chessboard moments" | (L) |
| RP subadditivity Z_T <= Z_{T_*}^{q^4} | (S95) second inequality, printed p. 619; (SV14), printed p. 633; transfer operator positivity [PW, Lemma 8.1]; sign of the pressure difference [ND, §7.3] | (P) here, (L) for transfer-matrix positivity |
| Splitting (S96) and transfer of source bounds with a common normalizer | (S96)–(S99), printed pp. 619–620: "The only cross-volume renormalization input is the source-zero estimate (S94)" | (P) |
| Reference-torus sourced bound (RT) | (S92)–(S93), printed p. 618: e^{−L(J)} Z[J]/Z[0] <= e^{C Vol}, ||J||_{C^5} < r_0, constants uniform in cutoff and in compatible volume with a lower period bound; L strictly local, additive over separated supports (S93) | (C): rests on the imported source theorem S74–S81 of the source construction, itself conditional on items 1–2 |
| S94 <=> pressure comparison | (SV3)–(SV4), printed p. 630; [ND, (7.2)] | (P) |
| Elementary gluing bound O(beta a^{−3}/t_*) | (SV5)–(SV9), printed pp. 631–632; [ND, (7.3)] | (P), insufficient |
| Transfer-matrix bound O(a^{−3} log beta) | [PW, Theorem 8.2, (8.11)]; covering argument [PW, (8.7)–(8.10)] | (P), insufficient |
| Energy–entropy identity for the seam | (SV12), printed p. 632; [PW, (8.15)–(8.17)] | (P), diagnostic |
| Equivalent targets: (SV11) signed boundary integral, (SV16)/(9.2) normalized trace, (9.6) two-copy overlap, I_m information bound | printed pp. 632–633; [PW, §9]; [SR, App. A, (49)–(51)] | (P) equivalences; targets open |
| Gaussian torus comparison HC | §111: finite-range inverse/determinant expansions (V6.5)–(V6.10), printed pp. 814–815; ledger of leaves, printed pp. 826–827 | (P) for the Gaussian leaf |
| Exact local-factor conjugacy and root-counted defect identity | [OS, Prop. 8.1 and (45)–(51)] | (P) algebra; the induction bound on E_k open |
| Fixed-resolution density bounds and entropy argument | §32.5 (123)–(126), printed pp. 213–214; §32.2 projective limits and RP of limits (116), printed p. 212 | (C) on [8, Thm 1]; fixed torus |
| OS reconstruction without clustering; Driessler–Summers | §69.3, printed p. 467; §74, printed p. 488 (SC3), conditional scalar sector | (L) as read; (C) hypotheses (D1),(SP2),(SC1) |
| Statement that S94 is "the infrared problem in disguise" | Summary of open problems in the source construction | Disputed here: see Section 2.6 |

**How the approach of the source construction relates to (iv).** The source construction pursues S94 by exact naturality of *every* coefficient of the full nonlinear and large-field (R) histories on the two tori (§89.22.2, §111.8 "three routes", and [OS, §8.4]). Proposition 2.7 shows this is more than S94 needs: on the large torus only the small-field sector is required (lower bound by positivity), and the large-field sector is needed only on the fixed small torus, where it is Balaban's published setting. The "regular/R vacuum births" leaf and "complete nonlinear and R sensitivity" leaf of the source construction (printed p. 826) are thereby removed from the volume-uniform part. The remaining leaf is the nonlinear small-field one ("finite nonlinear Gaussian readout", "uniform weighted derivative/density bounds for every actual inherited readout"), which is Theorem A.

**Is any of SV11, SV16, (9.6), I_m implied by (iv)?** Yes, all of them, a posteriori: Theorems A+B give S94 in the form p_{a,T_*} − p_{a,qT_*} <= C for every q and every rectangular enlargement family; [PW, (9.1)] then gives log R_{a,Sigma} <= (q/(q−1)) t_* A C, i.e. (9.2) = (SV16); (9.5) gives (9.6); (SV11) is identical to S94 by (SV5)+(SV10); and − log P_m <= 2 I_m ([SR, (50)]) is an *upper* bound on the purity by information, not needed. None of them is a route *to* (iv); they are consequences.

---

## 5. Alternatives, and why they do or do not help

**5.1 Why the elementary gluing bound costs a^{−3} (P).** Same-variable gluing identity (SV5): Z_T/Z_{T_*}^M = E_{mu_0} e^{−beta Delta S}, mu_0 = mu_{T_*}^{⊗M}. A rewired plaquette p contains exactly one link of a neighbouring independent block. Under mu_0 that block is separately gauge invariant; a gauge transformation h at the endpoint of the open bond multiplies that link by h and no other link of p, so E_{mu_0} Tr(U_1 U_2 U_3 U_4) = ∫ dh E Tr(U_1 U_2 U_3 h U_4) = 0 (Haar average of a nontrivial irreducible representation vanishes). Hence E_{mu_0} s(U_p^{big}) = 1 for every rewired plaquette while E s(U_p^{per}) = s-bar = O(1/beta). Jensen gives G_{a,q} := M log Z_{T_*} − log Z_T <= beta E_{mu_0} Delta S = beta N_seam (1 − s-bar) with N_seam = M(12 n^3 − 6 n^2), i.e. p_{T_*} − p_T <= 12 beta/(t_* a^3). The relative-entropy identity (SV12) G = beta E_{mu_0} Delta S − D(mu_0 || mu_1) shows the real reason: the product measure is UV-divergently far from the true measure at the seam (D ~ beta N_seam up to a^{−3} log beta by [PW, (8.16)]), and S94 is the O(Vol) difference of two O(a^{−3})-sized terms. Any bound that treats the two terms separately must fail; only a local-counterterm (renormalization-group) accounting can exhibit the cancellation. This is why (iv) is the right shape.

**5.2 Why the transfer-matrix bound has a^{−3} log beta (P).** (8.9)–(8.11): the covering argument lower-bounds the top eigenvalue by the mass of one product cell of radius r ~ beta^{−1/2} per spatial link, giving log Tr(K/||K||) <= E_Sigma [C + (m/2) log(1+beta)] with E_Sigma = 3A/a^3 spatial links. This counts beta^{m/2} "states" per fine link — the entropy of the lattice variables at the resolution set by beta — instead of the physical count of thermally occupied states, which should be e^{O(A t_*^{−3})}. The missing cancellation is again the vacuum-energy subtraction, now in the time direction.

**5.3 Finite-temperature free energy.** (SV16)/(9.2) is log Tr e^{−t_* (H − E_0)} <= C t_* A: finiteness of the vacuum-subtracted free-energy density at temperature 1/t_*, uniformly in a. This is S94 for the enlargement of the time side and needs the same ingredient: the vacuum counterterm of the time-periodic box equals that of the reference box up to O(1). No independent route; same lemma.

**5.4 Correlation inequalities.** Griffiths/GKS and FKG inequalities for the Wilson action are available for abelian groups (U(1), Z_N) and are not available for SU(N): the character-expansion coefficients of the Boltzmann weight are nonnegative, but the duplicate-variable argument needs nonnegativity of all Fourier coefficients of products of gauge-variant link monomials, which fails. Even where monotonicity of the pressure in the volume holds, it gives the sign already known from RP, not an O(1) bound. Does not help.

**5.5 Faria da Veiga–O'Carroll (L, arXiv:2205.07376v2).** Theorems 1–2 and (23): z_l^{Lambda_r} <= Z^u <= z_u^{Lambda_r} with Lambda_r the number of retained lattice bonds and z_l, z_u single-bond partition functions sharing the singular factor (a^{(d−4)/2}/g)^{delta_N} but with different O(1) constants c_l < c_u; the scaled free energy per retained bond lies in [c_l, c_u] (their (27)); the thermodynamic limit is taken first, then a -> 0, both subsequentially (their Theorem 3). The window c_u − c_l per lattice bond is O(a^{−4}) per unit physical volume; S94 needs O(1). They do not match, because the upper bound deletes plaquette interactions and the lower bound uses a global quadratic majorant of the action: neither sees the interaction between neighbouring bonds, which is where the a^{−4} log(1/a) running vacuum energy lives. This agrees with §92.7 of the source construction (printed p. 634).

**Conclusion of Section 5:** none of the alternatives avoids the RG; (iv) with Theorems A and B is the only route identified here, and it is how Dimock's scalar stability is proven uniformly in the volume.

---

## 6. Pitfalls and open questions

**6.1 Interchange of a -> 0 and T -> infinity.** Not an issue for existence: (U) is uniform in (a,T) jointly, so one extracts a joint diagonal subsequence (a_j, T_j). Different orders may give different limit points; existence needs one. The counterterms are volume-independent (E_vac(a) cancels in normalized expectations; L_a(J) is local, (S93)), and the bare trajectory g_0(a) is fixed in the ultraviolet, independent of T — this is essential and holds in the source construction ((SV19)–(SV20) there show that a T-dependent retuning would cost O(a^{−4}|delta beta|)).

**6.2 Subsequential limits suffice** for the Clay existence statement (Jaffe–Witten ask for a theory; uniqueness is not required), provided every property is verified for the limit of the chosen subsequence. Clustering is obtained inside a pure component rather than for the limit itself.

**6.3 Renormalization conditions.** They must be imposed on the reference torus T_* or in the UV, never on the large torus (whose running coupling at scale T is not small). In the (iv) scheme they are: g(l_0) fixed; observable normalization by the local counterterm L_a fixed by small-torus data.

**6.4 Could a pure component be trivial? Yes, a priori.** Driessler–Summers give components with unique vacuum; nothing prevents a component from being a constant field or a generalized free field (GFF). Two usable facts: (i) **(P)** if almost every component were a constant c_xi, the mixture's two-point function would be constant in the separation, so any non-constant connected two-point function excludes this ((SC1) argument of the source construction, printed p. 488). (ii) **(P)** if every component is a mean-zero Gaussian field with two-point function S_2^xi, then for real f the mixture's fourth cumulant is kappa_4(phi(f)) = 3 Var_nu( S_2^xi(f,f) ) >= 0. Hence **a strictly negative fourth cumulant for one real test function excludes a decomposition into mean-zero GFFs**. Caveat: a mixture of Gaussians with *different means* can have negative kappa_4, so the criterion must be applied to components with equal one-point functions (e.g. after showing the one-point function is the same in all components by a symmetry or a uniform short-distance law). A nonzero mixture fourth cumulant alone does not exclude a GFF mixture; (NG4)–(NG9) of the source construction are needed for that. Non-triviality is item E7 and remains **(O)**.

**6.5 Energy-bound hypothesis of Driessler–Summers.** The source construction derives it from a small-ball source insertion bound ((EP5), (SC3) at printed p. 488); that bound is itself conditional on the source theorem. **(C)**.

**6.6 OS growth exponent.** Section 2.4 gives beta_0 = 1 with a cell-summed C^5 norm; OS II's E0' must be checked for the admissible exponent and norm index. This is expected to be within E0', but it is not derived here from the OS II text. **(flag)**

**6.7 The observable family.** (U) must hold for the whole gauge-invariant family required by Jaffe–Witten, not only the action density; the chessboard argument is observable-agnostic once (RT) holds for each observable with a local counterterm. C-odd operators and winding loops are outside the scalar sector (§33 of the source construction, printed p. 215).

**6.8 Volume uniformity of Balaban's small-field expansion** is the single open mathematical point of this item (Theorem A). Specific things that could hide a volume dependence and must be ruled out in the primary text: (a) gauge fixing of the coarse field (should be unnecessary: integrate U_K with Haar); (b) the constant term of the Gaussian normalization on the torus (controlled by 2.7(a)); (c) the choice of small-field thresholds p_k (uniform); (d) the minimizer/background construction on the torus (local by exponential decay of the response). No indication that any of these is volume-dependent has been found.

---

## 7. Primary sources to check, with the specific statement

1. Bałaban, "Large field renormalization II", CMP 122 (1989) 355–392: **Theorem 1** — exact form of the stability bound, the torus setting (is the side a free parameter?), the definition of the vacuum counterterm, the coupling interval ]0, gamma]. Needed for Theorem B and to decide whether Theorem A is already contained.
2. Bałaban, "Renormalization group approach to lattice gauge field theories I", CMP 109 (1987) 249–301: the setup section (lattice T_eps and torus), the effective-action theorem, the running-coupling recursion (3.24)–(3.42), and whether the constants depend on the lattice size. Needed for Theorem A (A2), (A3).
3. Bałaban, "... II. Cluster expansions", CMP 116 (1988) 1–22: Lemma 2 (1.41)–(1.43) and the bounds (2.38)–(2.41): are the activity bounds and tree-decay constants independent of the number of blocks? Needed for Theorem A and 2.7(b).
4. Bałaban, "Convergent renormalization expansions for lattice gauge theories", CMP 119 (1988) 243–285: the density representation (2.18)–(2.23), (2.30) and the vacuum convention before Theorem 1. Needed to identify E_vac(a) with the small-field recursion.
5. Dimock, arXiv:1108.1335 (Theorem 1, "for all M, N"; (259)–(260) counterterm recursion independent of M; remark after (343) on the effective mass) and arXiv:1304.0705 (Theorem 2, Corollary 1: eta independent of M, N; Section 2 on using the mass for the last step). These are the explicit volume-uniform templates.
6. Osterwalder–Seiler, Ann. Phys. 110 (1978) 440–471: RP for both reflection types and positivity of the transfer matrix (used in 2.1–2.2).
7. Fröhlich–Israel–Lieb–Simon, CMP 62 (1978) 1–34, Theorem 2.2; Glimm–Jaffe, Quantum Physics, Theorem 10.5.4 and Section 10.5 (chessboard estimates on a torus).
8. Osterwalder–Schrader, CMP 42 (1975) 281–305: Theorem E0'–E3 => Wightman; the exact statement of E0' (exponent and norm index) for 6.6.
9. Driessler–Summers, Helv. Phys. Acta 59 (1986) 331–348, Theorem 2.3 and Section III pp. 335–343; Ann. IHP 43 (1985) 147–166 for Poincaré covariance of components. Not verified here; hypotheses must be confirmed.
10. Faria da Veiga–O'Carroll, arXiv:2205.07376v2, Theorems 1–3, (23), (27)–(28): the constants c_l, c_u do not match.
