# Tensor admission and fixed-order contact estimates

## 4.29 Full tensor quadratic admission at a fixed regular background

The complete proof is given in [Tensor quadratic admission and the marked transition](tensor_quadratic_admission.md), §§2–3. It proves a genuinely tensor statement, using all 21 components and the actual nonlinear constraint chart. The result concerns one averaging scale and one fixed source-free regular background. It does not construct a displaced sourced minimum or a mixed-scale history.

Let the fine spacing be η, the averaging scale be h≥η, and the background obey B99 (3.35)–(3.36). Normalize the trace as tr=Tr/N. Let H be the constrained Hessian of the unit-coefficient Wilson action and H_J the constrained Hessian of the clover action with a symmetric six-by-six coefficient field J. The P2 conversion is J_AB=4N j^{μνρσ} when the clover action is written using tr. Then on the actual constrained tangent space,

\[
 h^{-2}\|A\|_2^2+\|DA\|_2^2\le C\langle A,HA\rangle,
 \qquad
 |\langle A,H_JA\rangle|\le C\|J\|_\infty\langle A,HA\rangle.
 \tag{4.211; P under the stated fixed-background L hypotheses}
\]

The proof retains the small term in the untraced plaquette derivative. The exact source force has the form D*B_J+R_J, with R_J curvature-small; it is not silently replaced by a pure covariant divergence. Applying the B99 nonlinear constraint jet and the adjoint lift bounds controls the constraint-curvature contribution by C‖J‖∞εh⁻²‖A‖². Positivity of the source-free constrained form then proves the relative estimate. No derivative of J is required.

Here X denotes the coefficient of the normalized-trace quadratic form XH−H_J; at the bare scale X_B=2N²x in P2. For complex J, set B_J=H⁻¹ᐟ²H_JH⁻¹ᐟ². The inverse and determinant logarithm are holomorphic for C‖J‖∞<X. If D_fl is the actual dimension of the Gaussian tangent space, the source derivatives obey

\[
 \left|D^m\!\left[-\frac12\operatorname{Tr}
       \log(I-X^{-1}B_J)\right]_{J=0}[J_1,\ldots,J_m]\right|
 \le \frac{D_{\rm fl}}2(m-1)! (C/X)^m
                     \prod_i\|J_i\|_\infty.
 \tag{4.212; P}
\]

The proof uses the convergent matrix logarithm and all ordered multilinear products, without a commutativity assumption. The same force decomposition bounds the added source-force square in a centered Gaussian by C‖J‖∞²ε²X⁻¹Vh⁻⁴ on a one-scale core of physical volume V. At a noncritical background, a pre-existing Wilson force creates a separate cross term; that term is not estimated by this source-force-square bound.

The coordinate factor D_fl in (4.212) has not been replaced by N_T. Localizing and subtracting this sourced Gaussian vacuum, comparing its actual domains, and controlling the inherited fields are residual R1 problems. B116 p.21 supplies a source-free Gaussian local family with its printed bound; its reference to CMP 102, pp.255–275, formula (63), does not by itself prove a sourced Gaussian extension.

## 4.30 One fixed analytic disk for every regular constant-scalar derivative

The analysis in [Tensor channels, scalar derivatives and contact regularity](regular_tensor_channels.md), §2, upgrades the coherent regular two-jet implication of §4.26 to every scalar order. This is a theorem about the admitted regular activity recursion. Its physical application retains exactly the running-coordinate identification R0-reg; that identification is not inferred from the numerical N2-F.

Consider the exact regular recursion with unprojected fresh activities H, fixed Gaussian family G and bounded fixed Wilson projection P_k:

\[
 H_{k+1}=G_{k+1}+\Phi_k(X_k,H_{\le k}),\qquad
 X_{k+1}=X_k-P_kH_{k+1},\qquad X_0=X_0^0+\lambda.
 \tag{4.213; P: definition of the regular analytic recursion}
\]

Suppose on fixed relative-X neighborhoods of the baseline and a fixed old-family ball that ‖∂_XΦ_k‖≤A h_k and ‖D_HΦ_k‖≤q<1, where h_k is nondecreasing, h_k≤h_* and Σ_kh_k≤B uniformly in ultraviolet depth. Write C_H=A/(1−q), L=‖P‖C_H and M=exp(LB). A radius smaller than both σX_*/(4M) and b/(4C_Hh_*M) keeps every iterate strictly within those neighborhoods. For every m≥1,

\[
 |\partial_\lambda^m X_k(0)|\le m!Mr^{1-m},\qquad
 \|\partial_\lambda^m H_{k+1}(0)\|
       \le m!C_Hh_kMr^{1-m}.
 \tag{4.214; P for the stated analytic iteration; C for its R0-reg physical application}
\]

The proof constructs the entire disk inductively. If D_k=max_{i≤k}|X_i−X_i⁰|, the old-family derivative bound and monotonicity give ‖δH_{k+1}‖≤C_Hh_kD_k and D_{k+1}≤(1+Lh_k)D_k. Thus D_k≤M|λ| and the old-family displacement stays below b/4. Holomorphic composition and Cauchy finish the proof. There is no unsupported continuation of a germ and no assumption on r_k''.

For the regular CT family of §4.25, h_k may be taken as A g_k³(log g_k⁻²)^p and q_k≤Cθ(g_k). A sufficiently weak terminal choice makes q<1 and h_k monotone, and positive drift gives a cutoff-independent sum of h_k. Section 4.28 explains how the numerical weak interval is achieved; R0-reg still has to identify the corresponding physical running coordinate.

Pure log-g vacuum normalizations are accounted for separately. Their fine-volume sum is not bounded by (4.214). Neither a complex disk for regular activities nor a fixed-background determinant disk asserts a zero-free domain for the complete sourced partition function. Spatial sources, tensor marginal coefficients, recent-R, boundary and compulsory-history inputs remain outside this regular conclusion.

## 4.31 The full tensor space, its hypercubic channels and its exact lattice artifact

The complete algebraic proofs are in [Tensor channels, scalar derivatives and contact regularity](regular_tensor_channels.md), §§3–5. They distinguish finite-dimensional kinematics and actual renormalization estimates.

The stated pair symmetries give Sym²(Λ²R⁴), of dimension 21. There is no further algebraic Bianchi quotient: one-color local Abelian curvatures give matrices −vvᵀ for arbitrary v∈R⁶, and those matrices span the full symmetric space. Hodge decomposition gives dimensions 1+1+9+5+5, consisting of scalar, pseudoscalar, symmetric traceless stress and two further five-dimensional pieces. Under the full signed-permutation group H₄, including reflections, this representation is multiplicity-free with sector dimensions

\[
 21=1_{\rm scalar}+1_{\rm pseudo}
       +3_{\rm stress,diag}+6_{\rm stress,off}
       +2_{\rm W,diag}+2_{\rm W,disjoint}+6_{\rm W,shared}.
 \tag{4.215; P}
\]

The proof decomposes the coordinate sign-change characters into diagonal, disjoint-pair and shared-index orbits, then decomposes their stabilizer actions. Consequently an H₄-covariant linear marginal map is Σ_sm_sΠ_s for seven orthogonal projectors. Covariance does not bound these seven numbers or make the different sectors equal. Identity mixing is extracted separately. The seven-scalar conclusion concerns the 21-dimensional marginal space after one scalar representative has been selected. On the literal 22-dimensional bare source space, Wilson scalar plus clover tensor, the two trivial scalar copies allow a 2×2 scalar block in addition to the six other sector coefficients. Reducing that block to a marginal scalar and an irrelevant artifact requires the actual artifact control; the smooth-field identity alone does not perform that reduction.

For one clover let P_i, i=1,…,4, be its consistently based plaquettes, H_i=(P_i+P_i†)/2, B_i=(P_i−P_i†)/2, A_i the traceless part of B_i, and Fhat=Σ_iA_i/4. With S_sym=Σ_is(P_i)/4, the exact identity is

\[
 S_{\rm sym}+\frac12\operatorname{Tr}\widehat F^2
 =\frac18\sum_i\|I-H_i\|_{\rm HS}^2
  +\frac1{8N}\sum_i|\operatorname{Tr}B_i|^2
  +\frac18\sum_i\|A_i-\widehat F\|_{\rm HS}^2\ge0.
 \tag{4.216; P on the real unitary slice}
\]

It follows that |J:Q|≤2‖J‖opΣ_AS_sym,A at a site, and Σ_x,A S_sym,A=Σ_ps_p on a torus. Here J_AB=4j^{μνρσ} when the trace is Tr; the normalized-trace convention of §4.29 has an additional N. This proves a full bare tensor energy budget on compact fields, without asserting that every later effective source has the same pointwise bound.

The holomorphic identity replaces daggers by inverses and norm squares by the corresponding trace polynomials. On a common small identity chart it is bounded by C(δ⁴+η²), where δ bounds the plaquette deviations and η bounds the differences between the four clover skew parts. Smooth fields with δ=O(a²), η=O(a³) give an O(a⁶) artifact. This conclusion requires those regularity hypotheses and is not a quantum large-field estimate.

For a lower-vertex source f the exact scalar matching also contains Σ_p[f(x_p)−fbar_p]s_p, where fbar_p is the average over the four vertices. This is generally O(a∇f) before renormalization, with a nonzero first derivative term. The literal source-placement defect must be controlled or the reflection-covariant convention changed explicitly under ICR-N1-2.

If the actual seven marginal coefficients satisfy |m_{k,s}−1|≤C/X_k with drift X_k−X_{k+1}∈[d,D] and a sufficiently weak ceiling, their products and inverses are at most 2(X_j/X_k)^{2C/d}. This is a proved implication; the estimate on the actual m_{k,s} remains open. Combined with a single geometric age gain after unrolling the history, polynomial transport of m source slots costs only one fixed additional factorial power. Spending that loss again at every RG step would not prove R3. The full argument proves the exact memory estimate and the common factorial-weighted jet algebra, while retaining the unproved primitive and ownership inputs.

## 4.32 A necessary vacuum divergence and the failure of a preintegration shortcut

The analysis in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md), §§2–3, proves the following finite-lattice statements directly for the actual Wilson measure. Let V=n⁴, n≥2, d_A=N²−1, C_F=d_A/N and β>0. With the Lie metric −Tr(T_AT_B)=δ_AB, let S_b be the six-plaquette star of a link, P_b its squared action gradient and ℓ_b its action Laplacian. The exact identities and conditional Haar integration by parts give

\[
 P_b\le12S_b,\qquad \ell_b=C_F(6N-S_b),\qquad
 \mathbb E_\beta S\ge\frac{6d_A}{12\beta+C_F}\,V.
 \tag{4.217; P}
\]

The proof uses Bessel's inequality for the single-plaquette gradient, the fundamental Casimir and βE(P_b|exterior)=E(ℓ_b|exterior). It does not assume a plaquette expansion or uniform regularity of the exterior.

For a smooth cell-supported profile 0≤f≤1 with a plateau f=1, let B_f(a) be fine links whose entire incident source labels lie in that plateau. Conditional integration by parts remains valid along the inhomogeneous coefficient β+uf. Thus

\[
 \log\mu_\beta\!\left(e^{-t\sum_pf(x_p)s_p}\right)
 \le-\frac{d_A|B_f(a)|}{8}
          \log\!\left(1+\frac{12t}{12\beta+C_F}\right),\qquad t>0.
 \tag{4.218; P}
\]

Choose t so that −tf belongs to the specified source class. At fixed physical plateau |B_f(a)| is of order a⁻⁴, while N2-F gives β_a=O(K+1). Therefore any deterministic subtraction C_a[−tf] producing bounded renormalized pressure must have −C_a[−tf] growing at least as ca⁻⁴/(K+1)−CN_T.

On a fully unreduced history lift, near the flat all-small field the bare source tends to zero and a budget counting only bad records is zero. Every fixed-cutoff such neighborhood has positive measure. Consequently the renormalized original-field exponential cannot have a pointwise upper bound exp(CN_T+sH_bad) with cutoff-independent C,s. The full argument states and proves the exact support hypothesis, essential-supremum assertion and contradiction. This is an obstruction to that particular envelope, not a counterexample to an integrated sourced stability theorem.

There is a second staging requirement. Erased large-field components generate connected R activities with their own vacuum terms; one must subtract those marked vacuum terms too. A local rare-component estimate does not imply a physical-volume cost for a tilt of every fine-scale record. Proposition 5.1 of [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md) gives an exact independent-Bernoulli counterexample with superpolynomially small single-site masses and ultraviolet-divergent global log moment. This refutes that inference without claiming Bernoulli independence for Yang–Mills.

Accordingly, any complete raw-count argument used here must occur after both regular E integration/vacuum extraction and erased-R connected integration/vacuum extraction. It then concerns only genuine compulsory surviving kernels, with all masses, constraints and old readouts retained. The integrated pressure criterion of §4.27 remains a possible route; it does not assert the false preintegration pointwise bound.

## 4.33 An exact SU(2) first integration, including its predictable exterior term

The analysis in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md), §4, supplies complete real and complex proofs. Use normalized SU(2) plaquette action a_p=1−ReTr(U_p)/2 and τ=2β_a, so the literal action is unchanged. Given the exterior of one link, its six staples correspond to unit quaternions v_i. Put r=|Σ_iv_i|, W=6−r, κ=τr and X=κ(1−u), where u is the quaternion coordinate along the staple sum. Then the star action is W+X/τ, with X=0 at r=0.

The tilted Haar density makes X stochastically dominated by Gamma(3/2,1). The conditional mean M(κ) satisfies M≤3/2, EX²≤15/4 and |M'|≤21/(4κ). In addition, the exterior term is the explicit gauge-invariant loop energy

\[
 W=\frac{\sum_{i<j}|v_i-v_j|^2}{6+r}
   =\frac{2}{6+r}\sum_{i<j}
         \left[1-\tfrac12\operatorname{ReTr}(V_iV_j^{-1})\right].
 \tag{4.219; P}
\]

Subtract the deterministic conditional logarithm for a flat star r=6. Denote the remaining logarithm for source z times the actual star action by Φ_τ(z;r). There exist numerical δ,C,C_* independent of τ, torus and real exterior such that

\[
 |\Phi_\tau(z;r)-zW|\le C|z|W/\tau
       \quad(|z|<\delta\tau),\qquad
 |\Phi_\tau^{(m)}(0;r)|\le m!C_*^mW\tau^{-m}quad(m\ge2).
 \tag{4.220; P}
\]

The first derivative differs from W by at most CW/τ. On the larger real interval |z|≤τ/2 the first bound holds with C=7/2.

For completeness, the complex argument works directly with G_κ(t)=E_κexp(tX). Gamma domination makes |G_κ−1|≤1/4 on a uniform disk. Its logarithm ψ_κ is therefore single valued there. The tilted mean (1−t)E_κ[Xexp(tX)]/G_κ(t) is uniformly bounded and differs from M(κ) by O(|t|). Exact differentiation gives |∂_rψ_{τr}(t)|≤C|t|/r. Integrate from r to 6 for r≥3; for r≤3 use W≥3 and the direct logarithm bound. The identity Φ_τ=zW+ψ_{τr}(z/τ)−ψ_{6τ}(z/τ) proves (4.220), including r=0. Cauchy yields all derivatives.

A set of links with no common plaquette can be integrated simultaneously, since their conditional laws factorize. The resulting source-free exterior law contains the actual factors exp(−6τ)I(τr_b), where I(κ) is the normalized Haar integral of exp(κu). Thus the next law contains log I interactions and is not a Wilson one-link law. The theorem identifies and bounds the first inherited predictable source; it does not establish its repeated integration with all older E/R/B interactions. The complex domain in (4.220) concerns the source with real exterior, not an arbitrary complex continuation of the exterior fields.

The exact next problem is stated in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md), §6.2: admit this interaction and every inherited old readout into the same domains and norms used for the next complete integral, then extract its local vacuum and field coefficients without dropping any survivor mass. That is the still-open R1/R2 transition.

## 4.34 Fixed contact regularity and quantitative extension to general tests

The analysis in [Tensor channels, scalar derivatives and contact regularity](regular_tensor_channels.md), §§5–7, proves the remaining functional implications with explicit order dependence. They apply to admitted local coefficients or an actual hierarchy satisfying their displayed input bounds; those physical inputs remain open R1–R4 inputs.

For an m-linear source coefficient of supremum norm A_m supported in a collar of radius hR about z, subtract the joint source Taylor polynomial through total degree four. With the factorially weighted C⁵ algebra norm, its remainder obeys

\[
 |(B_m-\mathcal P_4B_m)(f_1,\ldots,f_m)|
 \le A_m(hR/\ell_0)^5\prod_i\|f_i\|_{5,\ell_0}^{\rm alg}.
 \tag{4.221; P for the stated local coefficient}
\]

The exact fifth-derivative multinomial sum is bounded by the product of the algebra norms, so no additional m⁵ or factorial loss is needed. Exponential carrier decay pays R⁵; a scale anchor density h⁻⁴ leaves a summable factor h. This is the local operator estimate, not a construction of the complete partial-diagonal collision forest.

There is also an explicit quantitative extension theorem. Suppose the actual m-linear forms satisfy |S_m(f_1,…,f_m)|≤A^m(m!)^p∏_ip_s(f_i), with one fixed integer s and one fixed p. Then on general Schwartz functions F on R^{4m},

\[
 |S_m(F)|\le(A')^m(m!)^p q_{(2s+16)m}(F),
 \quad q_n(F)=\max_{|\alpha|\le n}\sup_x
         (1+|x|^2)^{n/2}\|\partial^\alpha F(x)\|.
 \tag{4.222; P under the displayed product-test hypothesis}
\]

Expand in tensor products of four-dimensional Hermite functions. Their weighted C^s norms are at most C_sλ^{s+3}; the summable square weight λ⁻⁶ and Cauchy–Schwarz bound the coefficient sum by C^m‖(H^{s+6})^{⊗m}F‖₂. Expanding this fixed-order oscillator power in each variable bounds the latter by C^m q_{(2s+16)m}(F). Finite tensor dimension contributes only an exponential constant. The full proof gives density and uniqueness. In particular s=5 yields order 26m, with a fixed factorial exponent.

A uniform complex bound for the actual renormalized generating functional would imply fixed-order product-test bounds by polarized Cauchy, with moments and cumulants treated separately. [Tensor channels, scalar derivatives and contact regularity](regular_tensor_channels.md), §7, states the exact support and normalization hypotheses. The regular scalar disk in §4.30 is not that all-history functional bound. Nor does (4.222) produce compatible coincident-point bounds from estimates proved only on separated cells. These distinctions keep the analytic implications from being mistaken for a completed R3.
