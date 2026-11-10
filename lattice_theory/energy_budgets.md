# Wilson normalization of local energy budgets

## 1. Target, new result and scope

This note addresses the normalization part of R1/R2 using the actual Wilson law. It does not condition on a favorable reference measure and does not delete a compulsory old mass. The full R1 and R2 theorems remain open. The new theorem is a cutoff- and volume-uniform exponential estimate for a local Wilson-energy budget, and for arbitrary nonnegative weighted collections of such budgets, along the given N2-F trajectory. It also proves an averaged exponential estimate for the ordinary frustration observable whose same-exterior bound failed in the preceding manuscript.

Throughout, G=SU(N), N≥2; d=N²−1; Haar measure is normalized; the fine periodic lattice has n sites in each of four directions, V=n⁴, and n≥2. There are 4V positive links and 6V plaquettes. The action and its normalized expectation are

\[
 s_p=N-\operatorname{ReTr}U_p,\qquad S=\sum_ps_p,\qquad
 Z_n(\beta)=\int e^{-\beta S}\,dU,\qquad
 \mu_{n,\beta}(F)=Z_n(\beta)^{-1}\int F e^{-\beta S}\,dU.
 \tag{CA.1; P: definitions}
\]

Let S_b be the sum of the six plaquettes incident on a positive link b. Every S_b is nonnegative and bounded by 12N. The main normalized estimate will have fixed constants κ,C>0 such that

\[
 \log\mu_{n,\beta_K}
       \exp\!\left(\kappa\beta_K\sum_bw_bS_b\right)
 \le C\sum_bw_b,
 \qquad 0\le w_b\le1,
 \tag{CA.2; P: theorem proved in §§2–5}
\]

for every compatible torus and every depth K on N2-F, with constants depending on N,L,γ,g_* and the fixed construction constants, not on K,T or the weights. Here β_K denotes the bare P2 coefficient at depth K; it is not the effective coupling at step K. The notation avoids confusing a terminal effective coefficient with the original Wilson law.

The estimate has the literal number or total weight of fine-link roots on its right-hand side. Physical-volume normalization follows for a budget whose weights already supply the required fourth power of the fine physical length. The theorem does not confer that weight on the original unrenormalized scalar source. The previous preintegration obstruction remains valid.

The proof uses an elementary partition-ratio estimate, exact reflection positivity through site planes, and a fully stated chessboard argument for the chosen interior blocks. No reflection theorem, sourced extension of Balaban, or further interface is assumed. All uses of N2-F are explicit numerical consequences of its bare recurrence.

Labels are P (proved), L (a checked literature assertion), C (a physical application with an explicit unverified premise), and O (an unproved actual-theory estimate). This note contains no new L import; the finite-lattice arguments are proved directly.

## 2. Exact plaquette forests and a uniform partition-ratio bound

### 2.1 The one-plaquette integral

Put z(β)=∫_{SU(N)}exp[−β(N−ReTr U)]dU. There are constants c_N,C_N>0 such that

\[
 c_N(1+\beta)^{-d/2}\le z(\beta)
       \le C_N(1+\beta)^{-d/2}\qquad(\beta\ge0).
 \tag{CA.3; P}
\]

To prove this, use an exponential chart U=exp X near the identity in su(N), with the Euclidean metric −Tr X². The Haar density in that fixed chart is bounded above and below by positive constants. The exact identity s(U)=‖U−I‖²_HS/2 and the derivative of exp at zero show that c‖X‖²≤s(exp X)≤C‖X‖² on a sufficiently small chart. Outside that chart, the continuous function s has a positive minimum because its unique zero on SU(N) is I. The chart integral is bounded by ordinary d-dimensional Gaussian integrals; the remaining integral is exponentially small for β≥1. Compactness handles 0≤β≤1. This establishes both bounds without an asymptotic expansion.

### 2.2 Upper bound by an exactly integrable plaquette forest

Retain only plaquettes in planes (1,μ), μ=2,3,4, with first coordinate t=0,…,n−2. There are 3(n−1)n³ such plaquettes. All omitted action terms are nonnegative, so discarding them gives an upper bound on Z_n(β). Hold every direction-1 link fixed.

For each μ and each transverse coordinate, the remaining direction-μ links form an open chain U_μ(t), t=0,…,n−1. A retained plaquette has the form
U_1(t)U_μ(t+1)U_1(t+e_μ)⁻¹U_μ(t)⁻¹. Its integral in the terminal chain variable U_μ(n−1), with the others fixed, is exactly z(β), by left and right Haar invariance. After that integration the next terminal variable also occurs in only one retained plaquette. Continue down the chain. The chains for different μ and transverse coordinates have disjoint free variables; their shared direction-1 links were fixed throughout. No independence of those fixed links is needed.

The remaining free Haar integrals are one, so

\[
 Z_n(\beta)\le z(\beta)^{3(n-1)n^3}.
 \tag{CA.4; P}
\]

The periodic plaquettes with first coordinate n−1 were deliberately omitted. Thus there is no leftover cycle in the chain integration. The argument also applies at n=2, where each retained chain has one plaquette.

### 2.3 Lower bound with the correct tree-gauge dimension

Choose a spanning tree of the lattice graph and fix its V−1 links to the identity by a tree gauge transformation with root gauge fixed. This is an exact Haar-coordinate change: recursively determine the vertex gauge from the tree links; for every non-tree link use its transformed link as a coordinate. Conditional left/right invariance of Haar gives product Haar measure in the new variables. The gauge-invariant action no longer depends on the integrated tree coordinates, whose integrals equal one. There remain

\[
 M_{\mathrm{free}}=4V-(V-1)=3V+1
 \tag{CA.5; P}
\]

independent link variables. Periodic and multiple edges cause no problem for a spanning tree of the finite connected graph.

Restrict all these free links to a fixed identity chart ball of radius δ=c(1+β)⁻¹ᐟ², with c small enough that its Haar measure is at least c_1δ^d. Every plaquette is a product of at most four such links or their inverses, the other links being tree identities. The telescoping product bound gives ‖U_p−I‖op≤4δ, and hence s_p≤8Nδ². Therefore βS≤48NβVδ²≤C_NV on this event. Its product Haar measure and action give

\[
 Z_n(\beta)\ge
 e^{-C_NV}(1+\beta)^{-\frac d2(3V+1)}.
 \tag{CA.6; P}
\]

All fixed powers of the chart constants have been absorbed into exp(−C_NV), since 3V+1≤4V. This lower bound uses the tree-gauge number of free links. Restricting all 4V original links instead would leave an extensive log β loss in the ratio below.

### 2.4 The ratio and its asymptotically free bound

Combining (CA.3), (CA.4) and (CA.6), for 0<s<1 one obtains

\[
 0\le\log\frac{Z_n((1-s)\beta)}{Z_n(\beta)}
 \le C_{N,s}V+
       \frac d2(3n^3+1)\log(1+\beta).
 \tag{CA.7; P}
\]

Indeed 1+(1−s)β≥(1−s)(1+β); the exponent difference is exactly
(3V+1)−3(n−1)n³=3n³+1. The nonnegative lower bound follows from S≥0.

For the N2-F trajectory, let x_j be its numerical coordinates and B=b₀log L+C_rγ². The recurrence and x_j≥γ⁻² give x_j−x_{j+1}≤B. Consequently, without using an unspecified asymptotic remainder,

\[
 \beta_K=2Nx_0\le2N(g_*^{-2}+KB),\qquad
 n=(T/\ell_0)L^K\ge2L^K.
 \tag{CA.8; P from N2-F (i)–(iii) and compatibility}
\]

The quantity (3/n+1/n⁴)log(1+β_K) is uniformly bounded in K and compatible T. Divide (CA.7) by V to conclude that, for each fixed 0<s<1,

\[
 \sup_{K,T}\frac1V
     \log\frac{Z_n((1-s)\beta_K)}{Z_n(\beta_K)}
 \le A_{N,L,\gamma,g_*,s}<\infty.
 \tag{CA.9; P}
\]

Only the bare coefficient in the literal Wilson integral is used here. The coefficient (1−s)β_K need not itself be identified with an N2-F trajectory: (CA.7) holds for every positive coefficient. No running-coordinate identification R0-reg is needed for (CA.9).

### 2.5 A stronger recursive plaquette forest

The boundary-sized loss in (CA.7) can be reduced to a fixed global-degree loss. The following sharper bound is also exact:

\[
 Z_n(\beta)\le z(\beta)^{3n^4-3}.
 \tag{CA.9a; P}
\]

Here is a construction that verifies the extra factors without treating dependent plaquettes as independent. More generally, consider a j-dimensional periodic n-lattice, j≥2. Separate its direction-1 links that wrap from first coordinate n−1 to zero. There are n^{j−1} such variables W(x_perp). For each transverse nearest-neighbor edge from x_perp to x_perp+e_mu, the wrapping (1,mu) plaquette is
W(x_perp)U_mu(0,x_perp)W(x_perp+e_mu)⁻¹U_mu(n−1,x_perp)⁻¹.
Choose a spanning tree in this transverse graph and retain only its n^{j−1}−1 wrapping plaquettes.

Also retain all (1,mu) open-chain plaquettes with first coordinate 0,…,n−2, and retain recursively a plaquette forest in the (j−1)-dimensional slice x₁=0. No selected open-chain or slice plaquette contains a wrapping direction-1 variable W. With every other variable fixed, integrate the W variables by deleting leaves of their transverse tree. Each leaf occurs in exactly one remaining selected plaquette and gives one factor z(β), independent of its neighbor and of both tangential-link coefficients. After all n^{j−1}−1 edges are removed, the last W variable is free Haar.

The tangential link variables now have no remaining coupling to the removed wrapping factors. Integrate the (j−1)n^{j−1} open chains from first coordinate n−1 down to one, exactly as in §2.2, obtaining (j−1)(n−1)n^{j−1} further factors. The unintegrated tangential variables at x₁=0 carry precisely the recursively selected slice action. Unused direction-1 variables integrate to one. This proves by induction that the selected integral is z(β)^{r_j}, where

\[
 r_1=0,\qquad
 r_j=(n^{j-1}-1)+(j-1)(n-1)n^{j-1}+r_{j-1}
      =(j-1)n^j-j+1.
 \tag{CA.9b; P}
\]

Every omitted Wilson plaquette has nonnegative action, so its removal is an upper bound on the original partition function. At j=4 the exponent is 3n⁴−3, proving (CA.9a). The integration order is essential: wrapping-tree variables are integrated before the tangential open chains, and the lower-dimensional slice last. At no stage is an unintegrated coefficient approximated by the identity.

Combining this bound with (CA.3) and the same tree-gauge lower bound (CA.6) improves (CA.7) to

\[
 0\le\log\frac{Z_n((1-s)\beta)}{Z_n(\beta)}
 \le C_{N,s}V+2d\log(1+\beta),\qquad0<s<1.
 \tag{CA.9c; P}
\]

Only four group-valued degrees separate the exponents 3V+1 and 3V−3. Formula (CA.9), and every normalized consequence below, follow from this stronger estimate as well. The simpler open-chain bound was kept above as an independent check of the integration mechanism. Neither upper bound integrates the discarded torus constraints or claims that the full action is a product of independent plaquettes.

## 3. Exact site-plane reflection positivity and the required chessboard estimate

### 3.1 Reflection positivity through sites, including the shared links

Take a coordinate reflection θ through the two site hyperplanes x₁=0 and x₁=n/2, with n even. The reflection sends an oriented link to its reflected oriented link; if the reflected orientation is negative, use the inverse of the corresponding positive-link variable. Haar measure is invariant under these permutations and inversions, and ReTr of a plaquette is invariant under the resulting reversal/conjugation.

Let B₀ contain all links tangential to the two fixed site hyperplanes. The other links split into B₊ and B₋, exchanged by θ: normal links on one of the two half-torus paths belong to that half; tangential links at an interior site belong to its half. Every unit plaquette is either contained in one closed half or is tangential and entirely in one fixed hyperplane. In particular, no plaquette contains a free link of both B₊ and B₋. Thus

\[
 S(U)=S_\partial(U_0)+S_+(U_+,U_0)
                         +S_+(\theta U_-,U_0).
 \tag{CA.10; P: exact site-plane action decomposition}
\]

The shared boundary links U₀ have not been independently duplicated. They are integrated once. For any function F of U₊ and U₀, define ΘF(U)=overline{F(θU)}. Product Haar measure and (CA.10) give

\[
 \mu_{n,\beta}(\Theta F\,F)
 =\frac1{Z_n(\beta)}\int e^{-\beta S_\partial(U_0)}
     \left|\int F(U_+,U_0)e^{-\beta S_+(U_+,U_0)}\,dU_+\right|^2dU_0
 \ge0.
 \tag{CA.11; P}
\]

This proves precisely the site-plane positivity used below. No bond-plane positivity or character expansion is needed. Translations and permutations of coordinates give the same statement for every translated coordinate site plane and its opposite plane.

### 3.2 Canonical reflected blocks

Let b be an integer dividing n and let m=n/b be even. The block interiors are translates of the cube (0,b)⁴. Observables used below depend only on links strictly inside these cubes. Label blocks by c∈(Z/mZ)⁴. For ξ in the base cube, define the geometric identification coordinatewise by

\[
 (\tau_c\xi)_i=
 \begin{cases}
 c_i b+\xi_i,&c_i\text{ even},\\
 c_i b+b-\xi_i,&c_i\text{ odd},
 \end{cases}
 \quad\pmod n.
 \tag{CA.12; P: canonical chessboard reflection map}
\]

The same map acts on link observables with the orientation/inverse convention of §3.1. Reflection in any block face carries τ_cF to τ_{c'}F, with c'_i=2t−c_i−1 in the reflected coordinate and the other indices unchanged. The evenness of m makes this parity rule consistent modulo m. Thus the reflected copy is literal, including orientation; no scalar source-placement approximation is used.

For a nonnegative base-block observable F, define its disseminated norm by

\[
 \|F\|_{\rm cb}
 =\left[\mu_{n,\beta}\!\left(\prod_c\tau_cF\right)\right]^{1/M},
 \qquad M=m^4.
 \tag{CA.13; P: definition}
\]

**Theorem 3.1 (P): the required generalized chessboard inequality.** For nonnegative bounded base-block observables F_c,

\[
 \mu_{n,\beta}\!\left(\prod_c\tau_cF_c\right)
       \le\prod_c\|F_c\|_{\rm cb}.
 \tag{CA.14; P}
\]

The theorem holds for every even m; no power-of-two restriction on the number of blocks is imposed.

**Proof.** First take a finite list F₁,…,F_r of strictly positive bounded observables; the list may include all M observables appearing in the desired array. Normalize each F_i by its positive disseminated norm, obtaining G_i whose fully homogeneous disseminated expectation is one. Among the finitely many colorings a of the M blocks by labels 1,…,r, let A be the maximal expectation of ∏_cτ_cG_{a(c)}. Every homogeneous coloring has expectation one, so A≥1.

If a coloring attains A, cut the torus at any pair of opposite block faces. The two half-products belong to opposite closed halves. Applying the Cauchy–Schwarz inequality associated with (CA.11) gives the square of its expectation bounded by the product of the expectations for the two colorings obtained by reflecting either half into the other. Both new expectations are at most A by maximality. Their product is at least A², so both equal A. Every such half-copy of a maximizing coloring is therefore still maximizing.

We now obtain a homogeneous maximizing coloring. Along the first coordinate, regard each block slice as a single letter containing its entire transverse array of colors. Start with any cyclic run of identical slice letters. If its length r₀ is less than m/2, copy a half whose last r₀ slices are that run; reflection across its ending face produces a run of length at least 2r₀. The new coloring still maximizes. If a run has length at least m/2, choose a half entirely inside it and reflect it; the coloring becomes constant along that coordinate. Repeating this finite doubling process therefore makes the first coordinate homogeneous.

Perform the same procedure along the next coordinate, treating its slices as arrays. Reflections in that coordinate preserve the homogeneity already obtained in the preceding coordinates. After all four coordinates, the maximizing coloring is globally homogeneous. Its expectation is one by the normalization of G_i. Hence A=1 and every normalized coloring has expectation at most one. Undoing the scalar normalizations proves (CA.14).

For general nonnegative bounded observables, apply the proved result to F_i+ε and let ε decrease to zero. All integrals are finite and converge by bounded convergence. This also handles a zero disseminated norm. ∎

### 3.3 The exact blocks used for N2-F

For K≥2 choose b=L². Then n/b=(T/ℓ₀)L^{K−2} is even on every compatible torus. Since b≥9, a full six-plaquette link star, including all its staples, fits strictly inside the base cube. For example take its positive root link in direction μ with starting coordinates (b−1)/2 in every direction. All incident sites lie at least three fine lattice units from the nearest face when b=9, and the margin increases with b.

Different reflected block stars have disjoint plaquette sets, and every copy is the literal reflected star. Consequently, if A_b is either S_b or the exterior minimum of S_b,

\[
 \sum_c\tau_c A_b\le\sum_c\tau_cS_b\le S
 \quad\text{pointwise on every real configuration.}
 \tag{CA.15; P}
\]

For K=0,1, the coefficients β_K are bounded by (CA.8), and direct compact-field bounds handle the finitely many depths. No incompatible block divisibility is needed for those cases.

## 4. Actual normalized local energy moments

**Theorem 4.1 (P).** For every fixed 0<s<1 there is C_s<∞, depending only on N,L,γ,g_* and the fixed N2-F constants, such that for every compatible torus, every depth K and every fine link b,

\[
 \mu_{n,\beta_K}\big(e^{s\beta_K S_b}\big)\le e^{C_s}.
 \tag{CA.16; P}
\]

The same bound holds with S_b replaced by any nonnegative, literally reflected block observable A_b satisfying 0≤A_b≤S_b.

**Proof.** For K≥2, take the b=L² block of §3.3 and F=exp(sβ_K A_b). The complete replicated product is at most exp(sβ_KS) by (CA.15). Its expectation is therefore at most Z_n((1−s)β_K)/Z_n(β_K). Equations (CA.9), (CA.13) and (CA.14) yield

\[
 \log\mu_{n,\beta_K}(e^{s\beta_K A_b})
 \le \frac1M\log\frac{Z_n((1-s)\beta_K)}{Z_n(\beta_K)}
 \le A_s b^4.
 \tag{CA.17; P}
\]

Translation invariance permits the translated block grid centered at any prescribed link; the four orientations have the same bound by coordinate permutation. At K=0,1, use S_b≤12N and the explicit bound on β_K in (CA.8). Enlarge C_s once. ∎

In particular, for every integer m≥0 and u≥0,

\[
 \mu_{n,\beta_K}\big((\beta_KS_b)^m\big)
       \le m!s^{-m}e^{C_s},\qquad
 \mu_{n,\beta_K}\{\beta_KA_b\ge u\}
       \le\min\{1,e^{C_s-su}\}.
 \tag{CA.18; P}
\]

This is an averaged statement under the true normalized Wilson law. It does not claim a bound uniform in every fixed exterior. In fact, a fully frustrated exterior may force S_b to be large for all values of the active link; the theorem bounds the probability of such an exterior under its actual law.

Define the exterior ground-star energy by

\[
 W_b(U_{b^c})=\min_{V\in SU(N)}S_b(V,U_{b^c}).
 \tag{CA.19; P: definition}
\]

The compact minimum exists; it is a continuous function of the finitely many exterior staple variables. It is gauge invariant and transforms as the corresponding link-star scalar under lattice reflections. Because 0≤W_b≤S_b, (CA.16)–(CA.18) hold for W_b. Thus, under the true exterior marginal,

\[
 \mu_{n,\beta_K}\{W_b\ge w\}
        \le e^{C_s-s\beta_Kw},\qquad w\ge0.
 \tag{CA.20; P}
\]

An exterior on which the conditional Wilson source has poor uniform bounds is therefore paid for here by its actual Gibbs probability. This conclusion uses the complete normalized law, including every exterior interaction. It has not been proved after conditioning on an additional arbitrary selector or future event.

## 5. Arbitrary weighted root budgets and physical-cell counting

### 5.1 A bounded covering by literal chessboard stars

For K≥2 retain b=L² and partition the positive fine links into
q=4(2b)⁴ classes, indexed by their orientation μ and their starting site modulo 2b in each coordinate. Every class is contained in one canonical disseminated-star array for a suitable translated block grid: if the base root starts at c₀=((b−1)/2,…,(b−1)/2), translate the grid origin to r−c₀ for the chosen residue r. The even-indexed blocks of this grid have roots r+2b z, with no orientation reversal. Those are exactly the links in the chosen residue class. The other blocks can be assigned observable one. This construction uses only translations by fine lattice sites, so all reflection planes remain site planes.

For one such class C and weights 0≤w_b≤1, apply (CA.14) with the cell observable exp(s w_bβ_K S_b). Since t↦t^w is concave for 0≤w≤1,

\[
 \|e^{s w\beta_K S_b}\|_{\rm cb}
 \le\|e^{s\beta_KS_b}\|_{\rm cb}^{w}
 \le e^{C_s w}.
 \tag{CA.21; P}
\]

The constant is the same type as in (CA.17). Thus

\[
 \log\mu_{n,\beta_K}
     \exp\!\left(s\beta_K\sum_{b\in C}w_bS_b\right)
 \le C_s\sum_{b\in C}w_b.
 \tag{CA.22; P}
\]

No independence among these stars or among different classes is asserted.

Apply Hölder with exponent q to the product over the q classes. With κ=s/q, this gives

\[
 \log\mu_{n,\beta_K}
       \exp\!\left(\kappa\beta_K\sum_bw_bS_b\right)
 \le\frac{C_s}{q}\sum_bw_b.
 \tag{CA.23; P}
\]

For K=0,1, the pointwise bound β_KΣ_bw_bS_b≤12Nβ_KΣ_bw_b proves the same form after increasing the constant. Taking, for example, s=1/2 proves (CA.2) with fixed κ,C for all depths. A smaller κ is also allowed.

### 5.2 A normalized dimension-four-weighted fine budget

Let D be a collection of physical cells of side ℓ₀, and let the root-link set consist of the four positive links starting at each fine site in those cells. Define

\[
 \mathcal B_D(U)
 =\beta_K(a/\ell_0)^4
       \sum_{b:\,\operatorname{start}(b)\in D}S_b(U).
 \tag{CA.24; P: definition}
\]

Each physical cell has exactly L^{4K} starting sites, and (a/ℓ₀)⁴=L^{-4K}. The total weight in (CA.2) is therefore exactly 4|D|. It follows that

\[
 \mu_{n,\beta_K}(e^{\kappa\mathcal B_D})\le e^{4C|D|},\qquad
 \mu_{n,\beta_K}(\mathcal B_D^m)
       \le m!\kappa^{-m}e^{4C|D|}.
 \tag{CA.25; P}
\]

The estimate is uniform in the cutoff, compatible torus and location or size of D. Unlike a raw component estimate under an unnormalized reference, this is already an estimate under the actual normalized Wilson probability measure.

If literal observables F_i obey |F_i|≤a_i B_{D_i}, where each D_i contains at most q₀ physical cells, then their joint absolute moments have one fixed factorial exponent:

\[
 \left|\mu_{n,\beta_K}\!\left(\prod_{i=1}^mF_i\right)\right|
 \le m!\left(\kappa^{-1}e^{4Cq_0}\right)^m\prod_i a_i.
 \tag{CA.26; P}
\]

Indeed B_{D_i}≤B_D for D=∪_iD_i, and |D|≤q₀m, so (CA.25) applies. The exact moment–cumulant partition formula then gives the same factorial exponent for the connected coefficients, with an enlarged exponential constant. One direct bound is
Σ_π(|π|−1)!∏_{B∈π}|B|!≤2^m m!, obtained by summing over the number of blocks.

This is a theorem for observables with the displayed actual weighted-energy majorant. It does not identify the renormalized scalar or tensor source with such an observable. In particular, the physical bare scalar insertion is Σ_pj(x_p)s_p, without the factor (a/ℓ₀)⁴. Its vacuum and collision divergences have not disappeared.

## 6. The frustration source is paid by the actual exterior energy

### 6.1 A pointwise bound for every SU(N)

Use the Lie metric −Tr(T_AT_B)=δ_AB. Split the six plaquettes incident on b into their three two-plaquette plane pairs, with action pieces S_{b,i}, i=1,2,3. Write
S_{b,i}(U)=2N−ReTr(UA_i), where A_i is the sum of two unitary staples; write A=A₁+A₂+A₃. Put F_i=∇_bS_{b,i}, F=Σ_iF_i, P=|F|², D=Σ_i|F_i|² and ℓ=Δ_bS_b. The ordinary and frustration quantities are

\[
 h_b=\beta\left(D-\frac13P\right)
       =\frac\beta3\sum_{i<j}|F_i-F_j|^2,
 \qquad r_b=\beta D-\frac13\ell.
 \tag{CA.27; P: definitions and elementary identity}
\]

These are the same observables used in main §4.23. Let M(A)=max_{U∈SU(N)}ReTr(UA). Since the Haar average of ReTr(UA) is zero, M(A)≥0. Cauchy–Schwarz gives M(A)≤√N‖A‖HS, and the triangle inequality gives M(A)≤6N. By definition W_b=6N−M(A).

The gradient components of ReTr(UB) are the coefficients of its real Hilbert–Schmidt projection onto the Lie algebra. Bessel's inequality therefore yields |F_i−F_j|²≤‖A_i−A_j‖²_HS. Also ‖A_i‖²_HS≤4N. Expanding the three pair differences gives

\[
 \begin{aligned}
 \sum_{i<j}|F_i-F_j|^2
 &\le3\sum_i\|A_i\|_{\rm HS}^2-\|A\|_{\rm HS}^2\\
 &\le36N-\frac{M(A)^2}{N}
 =12W_b-\frac{W_b^2}{N}.
 \end{aligned}
 \tag{CA.28; P}
\]

Consequently, on every real compact-group configuration,

\[
 0\le h_b\le4\beta W_b\le4\beta S_b.
 \tag{CA.29; P}
\]

This relates the frustration source to an actual exterior-dependent minimal Wilson energy. It is stronger than bounding it by a fixed multiple of β on all configurations.

For a single plaquette, Bessel's inequality applied to U_p−I gives |∇_bs_p|²≤2s_p. Cauchy–Schwarz for each two-plaquette pair then gives D≤4S_b. The Casimir identity Σ_AT_A²=−(d/N)I gives ℓ=(d/N)(6N−S_b), so |ℓ|≤6d. Hence

\[
 |r_b|\le4\beta S_b+2d.
 \tag{CA.30; P}
\]

### 6.2 Actual normalized moments, despite the failure at a fixed exterior

Theorem 4.1 and (CA.29)–(CA.30) imply the existence of κ₁,C₁>0, independent of depth, torus and link, such that

\[
 \mu_{n,\beta_K}(e^{\kappa_1h_b})
 +\mu_{n,\beta_K}(e^{\kappa_1|r_b|})\le C_1.
 \tag{CA.31; P}
\]

Every local absolute moment therefore has a uniform factorial bound. The weighted joint version follows from (CA.2) with the same fixed loss in the exponent parameter and the deterministic term 2dΣ_bw_b for r_b.

This resolves the local averaged normalization issue exhibited by the previous conditional counterexample. In that SU(2) configuration the total staple sum A vanishes, so the physical ground-star energy is W_b=12. Any sufficiently small exterior neighborhood of it has W_b bounded below by a fixed positive number. Equation (CA.20) gives an exponentially small probability in β_K for that neighborhood under the actual Wilson exterior marginal. A large conditional variance on that set therefore does not imply a large unconditional local variance.

More quantitatively, for 0<s<1 and every integer m≥0,

\[
 \mu_{n,\beta_K}\!\left(h_b^m\,1_{\{\beta_KW_b\ge u\}}\right)
 \le m!(8/s)^m e^{C_s-su/2}.
 \tag{CA.32; P}
\]

Indeed h_b^m≤4^m(β_KW_b)^m, and x^m≤m!(2/s)^mexp(sx/2); on x≥u use exp(sx/2)≤exp(sx−su/2), then apply (CA.16) to W_b.

The uniform same-exterior theorem remains false, exactly as before. The new result averages with the true exterior law and pays the rare frustrated configurations instead of replacing that law. It does not prove the full marked susceptibility bound Var(Σ_bf_bh_b)≤CΣ_b|f_b|². Its joint estimates control positive extensive budgets, not the cancellation or decay of long-range connected covariances. That distinction is necessary when using this result in R2.

### 6.3 Bare clover directions are covered by the same actual majorant

The result also applies to every bare tensor direction, without a regular-field assumption. For a plaquette P, the traceless anti-Hermitian part B⁰ of (P−P⁻¹)/2 obeys ‖B⁰‖²_HS≤2s(P). Averaging the four consistently based plaquettes of a clover and using Cauchy–Schwarz gives ‖Fhat_A(x)‖²_HS≤2S_sym,A(x). The matrix −Q_AB(x)=−Tr(Fhat_A Fhat_B) is a positive Gram matrix. Thus for any complex symmetric six-by-six matrix J,

\[
 |J:Q(x)|
 \le\|J\|_{\mathrm{op}}\sum_A\|\widehat F_A(x)\|_{\mathrm{HS}}^2
 \le\frac{\|J\|_{\mathrm{op}}}{4}
          \sum_{b\text{ incident on }x}S_b.
 \tag{CA.32a; P}
\]

For the last equality of counts, every plaquette touching x appears in exactly one of its four-plaquette clovers and in exactly two of the eight incident link stars. The ordered-index source convention is J_AB=4j^{μνρσ}, A=(μ<ν), B=(ρ<σ).

For 0≤w_x≤1 and ‖J_x‖op≤1, summing the right side of (CA.32a) gives bond weights (w_x+w_y)/4≤1/2 on b=(x,y), with total weight 2Σ_xw_x. Hence the actual normalized estimate is

\[
 \log\mu_{n,\beta_K}\exp\!\left(
        \kappa\beta_K\sum_xw_x|J_x:Q(x)|\right)
 \le2C\sum_xw_x.
 \tag{CA.32b; P}
\]

In particular every normalized fine clover direction β_KJ:Q(x) has uniform local exponential moments. Taking w_x=(a/ℓ₀)⁴ on physical cells gives an active-cell bound of the same kind as (CA.25). This is a compact-field, actual-measure estimate for bare clovers. It does not establish the marginal tensor transport, coincident-field counterterms or the physical renormalized insertion, whose continuum source normalization must be matched separately.

## 7. What a complete positive kernel can transport without inverse masses

### 7.1 An integrated majorant norm

Let Q(dv|U) be any complete normalized positive history kernel whose initial field is the original Wilson configuration. Its output v may include current fields, old fields, every selector label and auxiliary reference variables. Normalize with the actual source-free Wilson law μ=μ_{n,β_K}, and write μ̄=μQ. For an original-field payload F define the signed output measure

\[
 \nu_F(A)=\int Q(A\mid U)F(U)\,\mu(dU),\qquad
 \frac{d\nu_F}{d\bar\mu}(v)=\mathbb E[F(U)\mid v].
 \tag{CA.33; P}
\]

The equality is disintegration of the positive joint law μ(dU)Q(dv|U). For p≥1, Jensen and the tower property give

\[
 \left\|\frac{d\nu_F}{d\bar\mu}\right\|_{L^p(\bar\mu)}
 \le\|F\|_{L^p(\mu)},\qquad
 |\nu_F|\le Q(|F|\mu)
 \quad\text{as measures.}
 \tag{CA.34; P}
\]

These statements remain true after any further complete positive kernel. They retain the masses of rare history labels automatically: those masses are part of μ̄. No division by an isolated survivor mass is inserted into the estimate.

For the actual positive energy budget B_D in (CA.24), a further useful majorant is its conditional expectation B̄_D(v)=E[B_D(U)|v]. The actual normalized exponential estimate survives every such complete kernel:

\[
 \int e^{\kappa\bar{\mathcal B}_D(v)}\,\bar\mu(dv)
 \le\mu(e^{\kappa\mathcal B_D})\le e^{4C|D|}.
 \tag{CA.35; P}
\]

More generally, if an original source packet F_m obeys |F_m|≤c_mB_D^m, then |ν_{F_m}|≤c_mQ(B_D^mμ), and its integrated absolute bound is at most c_mm!κ⁻ᵐexp(4C|D|). These are concrete averaged raw norms that can replace an overstrong pointwise bound when the literal packet is covered by this majorant.

The difference from the R1 sufficient raw norm is substantial. That norm asks for a bound on every allowed exterior in terms of a deterministic assigned capacity. Equations (CA.34)–(CA.35) instead retain the true normalized distribution of the exterior and labels. The uniform local exponential estimates for h_b and r_b coexist with essential suprema growing like β_K in the SU(2) frustrated example. Uniform averaged admission therefore cannot be identified with uniform pointwise admission.

### 7.2 The limitations that prevent a full R1/R2 claim

First, the kernel must be complete and normalized after all its alternatives are retained. Restricting to a prescribed future event H changes the normalized law to Hμ̄/μ̄H. The inequalities above do not remove the denominator μ̄H. A selector-conditioned theorem still needs its actual comparison or a proof that the selected contribution is being summed without that separate normalization.

Second, the new majorant theorem applies to packets that actually satisfy the displayed bound in the original Wilson law, or to their genuine conditional pushforwards. It does not prove that a complete renormalized source packet has such a bound. The negative-source flat-field obstruction of [Wilson action lower bounds and the first SU(2) integration](local_sources/wilson_action_and_first_integration.md) rules out obtaining the full vacuum-subtracted source merely by assigning it a positive weighted-original-energy envelope before regular and erased-R integration.

Third, an averaged raw norm alone does not give the complex-background analytic norm needed for a local E/R/B projection. Point evaluation and field differentiation on a prescribed complex domain are not bounded operators on an arbitrary real L^p space. The mixed operation that turns a raw old kernel into an analytic current-field activity must be proved separately, with its actual measure and its analytic domain. The exact erased-R conditional mean and covariance of R1 remain the first such operation to admit.

The practical alternative is therefore a two-part proof space: admitted complex analytic atoms retain their existing local norms, while genuinely raw compulsory packets may use an actual integrated majorant such as (CA.34). A successful mixed transition must map those specific inputs to the next analytic/raw decomposition and prove the local identity and dimension-four projections. This is a proposed norm choice with proved raw transport and actual Wilson examples; its complete E/R/B invariance is O.

## 8. Outcome, exact remaining work and summary of inputs

The main new conclusion is the actual normalized estimate (CA.2), valid on every compatible torus along N2-F. It is proved from exact lattice integrals. The upper partition bound uses 3(n−1)n³ plaquettes whose Haar integrations form open chains. The lower bound uses precisely 3n⁴+1 non-tree gauge variables. That first logarithmic mismatch is of order n³ log(1+β). The sharper recursive wrapping-tree construction improves the upper count to 3n⁴−3 and reduces the mismatch to only 2(N²−1)log(1+β). Both are harmless per fine volume on the stated trajectory. A site-plane positivity proof with shared boundary links, followed by the explicit even-block chessboard argument, converts that global comparison into local normalized estimates. The fixed block size L² fits the star and all staples and divides every compatible fine torus for K≥2. The two earlier depths are covered by compact-field bounds.

The exact frustration inequality h_b≤4βW_b then pays the problematic exterior by its actual minimal star energy. It proves uniform local averaged exponential moments for the ordinary and frustration observables, even though a uniform same-exterior variance estimate is false. The same actual-measure bound covers all bare clover directions through their compact-field Gram-energy inequality. These theorems do not establish the marked ℓ² susceptibility, decay of connected correlations or renormalized tensor mixing.

The normalized weighted-energy estimate also supplies a concrete integrated raw majorant for complete positive history kernels. Its mass accounting is automatic under disintegration and Jensen, and it survives full positive pushforward. It is weaker than a deterministic pointwise-exterior capacity bound and can therefore admit literal payloads that the latter norm would reject.

**Full R1 remains O.** Prove the actual mixed analytic/raw operation, including the erased-R mean and covariance, on one admitted set of source and complex-background norms. Its local identity and full dimension-four projection must be the prescribed source construction. The new averaged norm is a valid option only for packets whose literal majorant and transition into analytic atoms have been proved.

**Full R2 remains O.** The new theorem normalizes literal local and weighted Wilson-energy budgets under the original measure. It does not identify the complete vacuum-subtracted physical source with those budgets, nor establish its compulsory-selector-conditioned law. The full source-local complex pressure route or a complete packet comparison remains necessary for that source. The regular and erased-R vacuum extractions must still be performed before the proposed complete domination stage.

| Assertion | Input and verification |
|---|---|
| One-plaquette integral (CA.3) | Compact SU(N), its exponential chart, exact s(U)=‖U−I‖²/2 and Haar density bounds; proved directly |
| Upper/lower partition bounds (CA.4), (CA.6), (CA.9a) | Explicit open chains, recursive wrapping trees and exact tree-gauge coordinates; every remaining variable counted |
| Uniform ratio (CA.9) | Only the numerical bound derived in (CA.8) from N2-F (i)–(iii), and the literal bare P2 coefficient |
| Reflection positivity and chessboard (CA.11), (CA.14) | Exact site-plane factorization with shared boundary links; normalized finite-color maximum and slice-reflection argument |
| Weighted normalized energy (CA.2) | Literal reflected interior stars, disjoint replicated plaquette sets, finite residue-class cover and Hölder |
| Frustration bound and actual moments (CA.29), (CA.31) | Hilbert–Schmidt projection, three-vector identity, exact ground-star energy and the proved actual energy estimate |
| Complete-kernel transport (CA.34), (CA.35) | Disintegration/Jensen for a normalized positive full kernel; no isolated survivor denominator removed |
| Complete interacting source admission and normalization | O; source identification, mixed analytic/raw closure, local vacuum/contact extraction and actual compulsory continuations remain |

The new estimates may be inserted into a continued R1/R2 proof with exactly these scopes. They do not require a new N-interface, a numerical second derivative, a source-free Gaussian approximation to an old kernel, or a claim that the first SU(2) decimation remains a Wilson law.
