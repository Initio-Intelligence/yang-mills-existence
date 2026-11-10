# Tensor channels, scalar derivatives and contact regularity

## 1. Target and status

The target is the actual R3 theorem of the revised Yang–Mills program: every component of the local dimension-four curvature-pair field, its running normalization and collision terms, with one factorial growth exponent independent of ultraviolet depth and insertion order. The only assumed numerical interface is N2-F. This note does not promote R1 or R2 conclusions to hypotheses that have already been verified.

**Current verdict: full R3 remains O.** The complete spatial/tensor source admission through the actual E/R/B history system and the normalized all-history bound are not established here. The conclusions proved below are substantive parts of that theorem, with their scope separated from its remaining inputs:

1. The previous regular current/old-family analyticity theorem implies one ultraviolet-depth-independent **bare constant-scalar source disk**, and every regular scalar derivative, once its exact baseline running-coordinate dictionary is identified. This strengthens the previous two-jet implication; it uses the same R0-reg identification and no common-family strengthening of N2-F.
2. The full algebraic dimension-four tensor space has 21 components. Its scalar, pseudoscalar and stress parts have dimensions 1, 1 and 9; ten further traceless self-dual/anti-self-dual components remain. The literal pair symmetries of the source convention in [Lattice conventions and hypotheses](../lattice_conventions.md) retain all 21.
3. There is an exact positive remainder identity comparing the scalar clover trace with the symmetrized Wilson plaquette energy. It proves the bare tensor energy domination and identifies the genuine scalar-representative artifact rather than discarding it.
4. A fixed complex source bound for the actual renormalized hierarchy would give order-uniform factorial estimates, fixed C⁵ contact regularity, and a quantitative extension to general Schwartz tests with derivative order at most a constant times the number of insertions. These implications are proved below; their complete-theory analytic input remains O.

The statuses are **P** (proved), **L** (checked primary source in its scope), **C** (application conditional on a displayed hypothesis), and **O** (unproved actual-theory assertion). Every displayed formula is labelled. This note is an intermediate proof module, not a claim that original N1-S or YM-E is now established.

The relevant existing results are §§4.25–4.26 of [Regular jet transport, pressure and coupling windows](regular_jets.md): the corrected logarithmic-cutoff regular E family on fixed background domains, its joint current-coupling/old-family holomorphy, and its exact scalar two-jet recursion conditional on R0-reg. Their fresh activities are **unprojected**; the vacuum and Wilson subtractions are fixed linear assembly maps. Pure finite-dimensional log-g vacuum constants are kept in their separate vacuum ledger.

## 2. One fixed bare scalar disk controls every regular scalar order

### 2.1 A nonlinear analytic iteration theorem

Let E_j be complex Banach spaces for unprojected fresh regular activities. For the step k→k+1, set H_{≤k}=(H₁,…,H_k), with the maximum-over-generations norm. The empty family at k=0 has norm zero. Fix real baseline data X_k⁰≥X_*>0 and H_j⁰, and let P_k:E_{k+1}→C be linear, with norm at most P. The exact recursion is

\[
 H_{k+1}=G_{k+1}+\Phi_k(X_k,H_{\le k}),
 \qquad X_{k+1}=X_k-P_kH_{k+1},
 \qquad X_0=X_0^0+\lambda ,
 \tag{R3.1; P: definition of the analytic iteration}
\]

where G_j is independent of λ in the fixed background convention and the baseline satisfies the same recursion at λ=0. Assume the initial old datum, if present, is also independent of λ.

For fixed σ,b>0, suppose Φ_k is jointly holomorphic on

\[
 {\cal D}_k=
 \{\,|X-X_k^0|<\sigma X_k^0,\ 
       \|H_{\le k}-H_{\le k}^0\|<b\,\},
 \qquad
 \|\partial_X\Phi_k\|\le A h_k,\quad
 \|D_H\Phi_k\|\le q_k\le q<1 .
 \tag{R3.2; C: exact local analytic input}
\]

Suppose 0≤h_k≤h_* is nondecreasing and ∑_{k<K}h_k≤B, with B,h_* independent of K. Define C_H=A/(1−q), L=P C_H, and M=e^{LB}. Choose a positive r satisfying

\[
 r<
 \min\!\left\{\frac{\sigma X_*}{4M},
       \frac{b}{4C_H h_*M}\right\},
 \tag{R3.3; P}
\]

Omit the second radius term when h_*=0, with the zero-forcing case interpreted directly.

**Theorem R3-A (P as an analytic iteration theorem).** For every finite K, recursion (R3.1) is defined and holomorphic on |λ|<r, and

\[
 \max_{i\le k}|X_i(\lambda)-X_i^0|\le M|\lambda|,
 \qquad
 \|H_{k+1}(\lambda)-H_{k+1}^0\|
 \le C_H h_k M|\lambda| .
 \tag{R3.4; P under R3.2}
\]

Consequently, for every m≥1,

\[
 |\partial_\lambda^m X_k(0)|
 \le m!M r^{1-m},
 \qquad
 \|\partial_\lambda^m H_{k+1}(0)\|
 \le m!C_H h_kM r^{1-m}.
 \tag{R3.5; P under R3.2}
\]

The radius and constants are independent of ultraviolet depth. The theorem does not require a bound on the first or second coupling tangent as an extra assumption.

**Proof.** Fix |λ|<r. Write D_k=max_{i≤k}|X_i(λ)−X_i⁰|. At each already constructed step, the line segment from the baseline pair (X_k⁰,H_{≤k}⁰) to the perturbed pair remains in the convex product domain D_k whenever the displayed perturbation bounds hold. Integrating the two partial derivatives along this line therefore gives

\[
 \|\delta H_{k+1}\|
 \le A h_k|\delta X_k|
       +q_k\max_{j\le k}\|\delta H_j\|.
 \tag{R3.6; P}
\]

Suppose inductively that each old difference obeys
\(\|\delta H_j\|\le C_H h_{j-1}D_{j-1}\).
Both h and D are nondecreasing, so the old-family maximum is at most C_H h_kD_k. Equation (R3.6) then gives
\(\|\delta H_{k+1}\|\le(A+qC_H)h_kD_k=C_Hh_kD_k\).
The coefficient recursion now implies

\[
 D_{k+1}\le(1+Lh_k)D_k
 \le |\lambda|\exp\!\left(L\sum_{i\le k}h_i\right).
 \tag{R3.7; P}
\]

Starting with D₀=|λ| proves (R3.4). The radius choice gives
D_k<σX_*/4≤σX_k⁰/4 and
\(\max_{j\le k}\|\delta H_j\|<b/4\).
Thus every subsequent input lies strictly within its admitted domain. This is a finite induction defining the maps on the whole fixed disk, not an assertion that a merely local germ can be continued without a bound. Holomorphic composition proves holomorphy at every stage. Cauchy's formula on circles of radius r'<r and then r'↑r gives (R3.5). The estimates apply in the Banach activity norm, so no carrier or volume factor is created by taking source derivatives. ∎

### 2.2 Application to the proved regular current/old-family map

In the existing regular construction, Φ_k(X,H)=Ψ_k(X^{-1/2},H). The relative current-g disk and the fixed enlarged old-family ball in main §4.25 contain a domain of the form (R3.2). The square-root branch is centered at positive X_k⁰; choose σ once so that |X−X_k⁰|<σX_k⁰ maps inside the stated relative-g disk. Along the entire straight segment used above, |g(X)| and g_k⁰ are comparable.

The current-g Cauchy bound, together with dg/dX=−g³/2, and the old-family bound give

\[
 \|\partial_X\Phi_k\|
 \le C\theta(g_k^0)(g_k^0)^2,\qquad
 \|D_H\Phi_k\|\le C\theta(g_k^0),\qquad
 h_k=A_{\rm cut}(g_k^0)^3(\log (g_k^0)^{-2})^p .
 \tag{R3.8; P from the regular CT bounds}
\]

Here θ(g)=A_cut g(log g⁻²)^p; A_cut is the fixed cutoff constant, distinct from the derivative constant A in (R3.2). One fixed reduction of the admitted coupling ceiling makes q<1/4. Positive drift of X makes g increase; a sufficiently weak ceiling makes h increase as well. If X_k⁰−X_{k+1}⁰≥d>0, comparison with the integral of x⁻³ᐟ²(log x)^p gives

\[
 \sum_{k<K} h_k
 \le C_{d,p,A_{\rm cut}}\,g_K^0(1+\log (g_K^0)^{-2})^p .
 \tag{R3.9; P}
\]

All constants are independent of K. Hence Theorem R3-A applies.

**Corollary R3-A′ (C on the same R0-reg physical identification as main §4.26).** The actual universal regular E-family recursion has one fixed bare constant-scalar disk and all scalar coupling/activity derivatives with the bounds (R3.5), after its exact running-coordinate dictionary and admitted baseline have been matched.

This closes the *regular constant-scalar all-order feedback implication*. It uses neither r_k'' nor an analytic interpolation of N2-F's numerical r_k. No separate common-family strengthening of N2-F is assumed. The physical running dictionary remains conditional, exactly as it was for the previous two-jet theorem.

The finite-dimensional powers of g produce explicit log-g vacuum normalizations outside H. They are retained in the physical partition function and are analytic on the same disk, but their unsubtracted sum has a fine-volume factor. Theorem R3-A does not call that divergent vacuum sum bounded. Its subtraction and source-locality must use the same vacuum recipe. The theorem also makes no zero-free assertion about the complete partition function and no spatial/tensor/R/B source claim.

## 3. The exact 21-component tensor space and its seven hypercubic sectors

### 3.1 There is no additional algebraic Bianchi quotient

Let V=Λ²R⁴ with orthonormal basis e₁₂,e₁₃,e₁₄,e₂₃,e₂₄,e₃₄. For independent oriented pairs A,B, the curvature-pair observable is Q_AB=Re Tr(F_A F_B). The pair antisymmetries have already been imposed by this basis, and pair exchange says Q_AB=Q_BA. Thus the coefficient space is

\[
 {\cal T}=\operatorname{Sym}^2(V),\qquad
 \dim{\cal T}=\frac{6\cdot7}{2}=21 .
 \tag{R3.10; P}
\]

No further linear relation follows from gauge invariance or the differential Bianchi identity. Indeed choose any nonzero T∈su(N) normalized by −Tr(T²)=1, and any v∈R⁶. The local Abelian connection A_μ(x)=−(1/2)∑_νF_{μν}x_ν with F_A=v_AT has exactly this constant curvature near the chosen point; multiply by a smooth cutoff away from that point if a global chart is needed. Its matrix Q is −vvᵀ. If a symmetric coefficient matrix J annihilates every such Q, then vᵀJv=0 for every v. Taking v=e_A and v=e_A+e_B gives every entry of J equal to zero.

In particular, the three familiar classes “scalar, pseudoscalar and stress tensor” are not by themselves a basis of the literal tensor space of the source convention. That convention retains all 21 through its stated pair symmetries; its parenthetical examples must not be used to reduce the space to eleven components.

### 3.2 Orthogonal continuum decomposition

Let * be the Euclidean Hodge involution on V. The ± eigenspaces V_± have dimension three. An explicit orthonormal basis is

\[
 e_1^\pm=\frac{e_{12}\pm e_{34}}{\sqrt2},\quad
 e_2^\pm=\frac{e_{13}\mp e_{24}}{\sqrt2},\quad
 e_3^\pm=\frac{e_{14}\pm e_{23}}{\sqrt2}.
 \tag{R3.11; P}
\]

In V_+⊕V_− coordinates, a symmetric matrix has blocks
\(Q=\left(\begin{smallmatrix}A&B\\ B^\mathsf T&C\end{smallmatrix}\right)\),
where A,C are symmetric 3×3 matrices and B is arbitrary. Decompose A and C into their traces and traceless parts. This gives

\[
 {\cal T}
 ={\bf1}_{\rm scalar}\oplus{\bf1}_{\rm pseudo}
   \oplus{\cal T}_{\rm stress}
   \oplus{\cal W}_+\oplus{\cal W}_-,
 \qquad
 21=1+1+9+5+5.
 \tag{R3.12; P}
\]

The first two coordinates are Tr A+Tr C and Tr A−Tr C. The two five-dimensional summands are the traceless parts of A and C. An orientation-reversing orthogonal transformation exchanges them and changes the sign of the pseudoscalar.

The nine-dimensional cross block is exactly the symmetric traceless stress representation. One direct check avoids an appeal to representation classification. Let J_i^± be the skew 4×4 matrices associated with √2e_i^±. Their products K_ij=J_i^+J_j^- are symmetric and traceless; explicit multiplication gives [J_i^+,J_j^-]=0 and Tr(K_ijK_kl)=4δ_ikδ_jl. Consequently the nine K_ij form a basis of the traceless symmetric 4×4 matrices. The contraction

\[
 {\cal S}(Q)_{\mu\nu}
 =\sum_\rho Q_{\mu\rho,\nu\rho}
 -\frac14\delta_{\mu\nu}
       \sum_{\lambda,\rho}Q_{\lambda\rho,\lambda\rho}
 \tag{R3.13; P}
\]

annihilates both same-duality blocks and sends the cross matrix B to
\(-\sum_{i,j}B_{ij}K_{ij}\).
Thus it is an isomorphism on the cross block and has inverse
\(B_{ij}=-(1/4)\operatorname{Tr}({\cal S}(Q)K_{ij})\).
Signs reflect the chosen two-form convention and do not change the decomposition.

### 3.3 Hypercubic covariance reduces the linear transport to seven scalars

The exact finite-lattice symmetry group H₄ is the signed-permutation group of the four coordinate axes. Its real orthogonal action on T is multiplicity-free with seven invariant summands:

\[
 21=1_{\rm scalar}+1_{\rm pseudo}
       +3_{\rm stress,diag}+6_{\rm stress,off}
       +2_{\rm W,diag}+2_{\rm W,disjoint}+6_{\rm W,shared}.
 \tag{R3.14; P}
\]

Here is a concrete description and proof. Under independent coordinate sign changes, diagonal entries Q_{ij,ij} have trivial character. Their six-dimensional space is the permutation representation on the edges of the complete graph on four vertices. It contains the scalar sum, the three independent differences
\(\sum_{j\ne i}Q_{ij,ij}-(1/2)\sum_{k<l}Q_{kl,kl}\),
and the two independent differences among the three matching sums
Q₁₂,₁₂+Q₃₄,₃₄, Q₁₃,₁₃+Q₂₄,₂₄, Q₁₄,₁₄+Q₂₃,₂₃.
These are mutually orthogonal invariant spaces of dimensions 1,3,2. The commutant of the edge permutation representation has dimension three: an invariant matrix entry depends only on whether the two edges coincide, share one vertex, or are disjoint. Thus these three invariant spaces are irreducible and inequivalent.

The disjoint-pair coordinates
(Q₁₂,₃₄,−Q₁₃,₂₄,Q₁₄,₂₃)
have the sign-change character ε₁ε₂ε₃ε₄. Permutations act by the three matching permutation representation with a common orientation-sign twist. Its scalar sum is the pseudoscalar; its sum-zero part has dimension two. Its commutant has dimension two, so these are irreducible and inequivalent.

For each pair i≠j, the two shared-index coordinates Q_{ik,jk}, Q_{il,jl}, with {k,l} the complementary pair, have sign-change character ε_iε_j. The six such characters form one orbit. The stabilizer of one character acts on its two-dimensional weight space by preserving both coordinates under i↔j and exchanging them under k↔l. Its two eigenspaces are their sum and difference. Inducing over the six characters gives the stress off-diagonal six-space and a distinct Weyl six-space. An intertwiner is determined by its restriction to one weight space and must commute with that exchange, so the commutant here has dimension two. Distinct sign-character orbits cannot mix. This proves (R3.14) and the multiplicity-free assertion.

Let Π_s denote the seven orthogonal projectors. Every H₄-covariant linear source transport M on the full tensor space therefore has the form

\[
 M=\sum_{s=1}^7 m_s\Pi_s,\qquad
 \|M\|=\max_s|m_s|,\qquad
 \|M^{-1}\|=\max_s|m_s|^{-1}
 \quad\text{if all }m_s\ne0.
 \tag{R3.15; P}
\]

This reduces the actual tensor marginal calculation to seven scalar coefficients; it does not compute or bound those coefficients. No equality between distinct hypercubic sectors follows merely from hypercubic covariance. Restoration of the larger continuum symmetry remains an R4 task.

The continuum nonidentity dimension-four family has 21 components; including the identity gives 22. The bare preamble has 22 nonidentity source coordinates because it uses both the Wilson scalar representative and the 21 clover coordinates. Their trace-channel redundancy is only modulo a lattice artifact, identified exactly in the next section. On that literal 22-coordinate bare system, the trivial hypercubic representation occurs twice: the full commutant contains an arbitrary two-by-two scalar block, together with the six remaining scalar sector coefficients. Thus the seven-coefficient reduction applies to the 21-dimensional curvature-pair marginal after a justified scalar-representative choice. Reducing the actual 22-coordinate induction to it requires control of the artifact direction; covariance alone does not perform that reduction.

## 4. Exact scalar/clover artifact and the full tensor energy budget

Fix one clover plane at a site x. Write its four consistently oriented plaquette matrices, all based at x, as P₁,…,P₄. For unitary plaquettes define

\[
 H_i=\frac{P_i+P_i^\dagger}{2},\quad
 B_i=\frac{P_i-P_i^\dagger}{2},\quad
 A_i=B_i-\frac{\operatorname{Tr}B_i}{N}I,\quad
 \widehat F=\frac14\sum_{i=1}^4A_i,\quad
 S_{\rm sym}=\frac14\sum_{i=1}^4
          (N-\operatorname{ReTr}P_i).
 \tag{R3.16; P: definitions in the literal clover convention}
\]

The factor 1/4 in Fhat is exactly the preamble's factor 1/8 multiplying P−P⁻¹.

**Theorem R3-B (P): exact positive artifact.** On every real compact-group configuration,

\[
 \begin{aligned}
 R_{\rm lat}
 &:=S_{\rm sym}+\frac12\operatorname{Tr}\widehat F^2\\
 &=\frac18\sum_i\|I-H_i\|_{\rm HS}^2
   +\frac1{8N}\sum_i|\operatorname{Tr}B_i|^2
   +\frac18\sum_i\|A_i-\widehat F\|_{\rm HS}^2
 \ge0.
 \end{aligned}
 \tag{R3.17; P}
\]

**Proof.** Unitarity gives H_i²−B_i²=I, with H_i Hermitian and B_i anti-Hermitian. Therefore
\(s(P_i)-(1/2)\|B_i\|_{\rm HS}^2=(1/2)\|I-H_i\|_{\rm HS}^2\).
The trace projection is orthogonal for the Hilbert–Schmidt norm:
\(\|B_i\|_{\rm HS}^2=\|A_i\|_{\rm HS}^2+|\operatorname{Tr}B_i|^2/N\).
Finally,
\((1/4)\sum_i\|A_i\|_{\rm HS}^2-\|\widehat F\|_{\rm HS}^2
=(1/4)\sum_i\|A_i-\widehat F\|_{\rm HS}^2\).
Combine these three identities and use
Tr Fhat²=−‖Fhat‖². ∎

This is stronger than merely saying that the Wilson and clover scalars have the same leading classical limit. It identifies their nonzero lattice difference.

Let Q_AB=Tr(Fhat_A Fhat_B) in independent-pair coordinates. Then −Q is a real positive semidefinite Gram matrix. For any complex symmetric 6×6 matrix J,

\[
 |J:Q(x)|
 \le \|J\|_{\rm op}\sum_A\|\widehat F_A(x)\|_{\rm HS}^2
 \le2\|J\|_{\rm op}\sum_A S_{{\rm sym},A}(x).
 \tag{R3.18; P}
\]

The first inequality follows by expanding the six Lie-algebra coordinates in an orthonormal real color basis and applying |vᵀJv|≤‖J‖op‖v‖² to each real vector v. The second is (R3.17). Under the preamble's sum over all ordered four indices, the independent-pair coefficient matrix is **J_AB=4j^{μνρσ}**, for A=(μ<ν), B=(ρ<σ). Equation (R3.18) uses this J; its factor four must not be dropped.

Every plaquette belongs to the clovers at its four vertices. Consequently
\(\sum_{x,A}S_{{\rm sym},A}(x)=\sum_ps_p\), exactly. The real compact-field domination in (R3.18) therefore controls the full bare tensor source in the same Wilson energy budget. This domination was already available in weaker form; the positive artifact decomposition is the additional conclusion here.

### 4.1 The analytic artifact bound and its actual regularity hypothesis

Replace P_i† by P_i⁻¹ in (R3.16), and replace s by its holomorphic trace extension. The identity becomes

\[
 R_{\rm lat}^{\rm hol}
 =\frac18\sum_i\operatorname{Tr}(I-H_i)^2
  -\frac1{8N}\sum_i(\operatorname{Tr}B_i)^2
  -\frac18\sum_i\operatorname{Tr}(A_i-\widehat F)^2.
 \tag{R3.19; P}
\]

This is a polynomial identity in P_i,P_i⁻¹; no complex conjugation is used. Positivity is claimed only on the unitary slice.

Suppose P_i∈SL(N,C) lie in one fixed sufficiently small identity chart, with
max_i‖P_i−I‖≤δ and max_{i,j}‖A_i−A_j‖≤η. Then

\[
 |R_{\rm lat}^{\rm hol}|\le C_N(\delta^4+\eta^2).
 \tag{R3.20; P}
\]

Indeed \(I-H_i=-(1/2)(P_i-I)^2P_i^{-1}\), so its norm is O(δ²). The principal logarithm K_i is traceless; B_i=sinh K_i gives Tr B_i=O_N(δ³). Also ‖A_i−Fhat‖≤η. Substitution in (R3.19) proves (R3.20).

For a smooth continuum connection sampled at spacing a, the required local bounds are δ≤C a² and η≤C a³, after the plaquettes are brought to the same base point. These follow from bounded curvature and one bounded covariant curvature derivative; they are the hypotheses needed here. Under them R_lat=O(a⁶). More generally, a determining scale ℓ and covariant Hölder control with exponent α>0 give
δ≤C(a/ℓ)², η≤C(a/ℓ)^{2+α}, hence a bound
C[(a/ℓ)^8+(a/ℓ)^{4+2α}].
Counting O((ℓ/a)^4) plaquettes leaves a genuine positive scale power on that regular record.

This is not a uniform quantum estimate on an arbitrary large-field history. There δ and η need not be small, and the artifact remains a bounded but nonzero compact-field observable.

### 4.2 Literal lower-vertex sources retain a placement defect

For a scalar profile f let
\(\bar f_p=(1/4)\sum_{x\in{\rm vertices}(p)}f(x)\).
Clover counting gives the exact identity

\[
 \sum_p f(x_p)s_p+\frac12\sum_{x,A}f(x)Q_{AA}(x)
 =\sum_{x,A}f(x)R_{{\rm lat},A}(x)
   +\sum_p[f(x_p)-\bar f_p]s_p.
 \tag{R3.21; P}
\]

With the preamble's lower-vertex x_p,
\(|f(x_p)-\bar f_p|\le Ca\|\nabla f\|_\infty\).
Its leading term is
\(-\frac a2(\partial_\mu+\partial_\nu)f(x_p)\)
for a μν plaquette. Thus an O(a²) claim for the literal source placement would be incorrect without symmetrizing it or treating this first-order defect.

At leading classical dimension four, the bare source pair (j⁽⁰⁾,J) maps to the tensor coefficient J−(j⁽⁰⁾/2)I. The one-dimensional bare redundancy direction is therefore (1,I/2). At finite cutoff it is the artifact and source-placement expression in (R3.21), not an exact zero observable. Its renormalized suppression is part of the R1/R4 estimates and cannot be inferred from its smooth-field expansion alone.

## 5. Polynomial running transport and one fixed Gevrey exponent

This section separates an actual tensor marginal estimate still to prove from the all-order bookkeeping that follows from it.

### 5.1 A precise tensor-flow input

Let M_k be the linear marginal map obtained by differentiating the **actual universal regular bulk** construction in a constant tensor source and extracting its dimension-four field part after vacuum subtraction, with one justified scalar representative. Matching this map to the coefficient in the complete sourced induction, while controlling any additional history-dependent dimension-four contributions, remains part of R1/R3. Hypercubic covariance gives (R3.15) for such a universal map. It does not give the following quantitative estimate:

\[
 |m_{k,s}-1|\le C/X_k
 \quad(s=1,\ldots,7),\qquad
 X_k-X_{k+1}\in[d,D],\quad
 X_k\ge X_*\ge2C.
 \tag{R3.22; O for the actual tensor marginal; drift is supplied after R0 matching}
\]

No statement about these seven coefficients is silently added to N2-F.

**Matrix transport lemma (P).** Under the displayed estimates, put
Z_{j,k}=M_{k-1}\cdots M_j. Then, with ν=2C/d,

\[
 \|Z_{j,k}\|+\|Z_{j,k}^{-1}\|
 \le2(X_j/X_k)^\nu
 \le2\{1+(D/X_*)(k-j)\}^\nu .
 \tag{R3.23; P under R3.22}
\]

To prove it, |m−1|≤1/2 gives
\(|\log|m||\le2|m-1|\).
Also
\(\int_{X_{i+1}}^{X_i}dx/x\ge d/X_i\).
Summing and exponentiating bounds each product and its inverse by
\((X_j/X_k)^{2C/d}\).
The upper drift gives the last inequality. The same norm estimate holds for a noncommuting matrix sequence with ‖M_k−I‖≤C/X_k; multiplicity-free covariance merely identifies the seven physical scalar coefficients that must be checked.

This bound allows running normalization. It does not imply a bounded inverse uniformly between the bare and terminal scales, which the literal N1-S interface requests.

### 5.2 A one-shot memory estimate at every order

**Lemma (P).** For fixed a>0, c≥0 and ν≥0, let d_ν=⌈ν⌉ when ν>0 and d_ν=0 when ν=0. There are finite constants C₀,C₁, depending only on a,c,ν, such that

\[
 \sum_{n\ge0}e^{-an}(1+cn)^{\nu m}
 \le C_0 C_1^m(m!)^{d_\nu}
 \qquad(m=0,1,2,\ldots).
 \tag{R3.24; P}
\]

**Proof.** The case ν=0 is geometric. Otherwise replace 1+cn by C_c(1+n), and νm by the larger integer d_νm. For r=d_νm,
\(\sum_{n\ge0}e^{-an}(1+n)^r
 \le e^{2a}r!a^{-r-1}\),
by comparing each term with the integral over [n,n+1] and shifting the integral variable. Finally
\((d_\nu m)!\le d_\nu^{d_\nu m}(m!)^{d_\nu}\):
the ratio on the left is a multinomial coefficient, bounded by the sum of all coefficients in the expansion of a d_ν-term sum raised to degree d_νm. Absorb the fixed exponential factors into C₀C₁^m. ∎

For an already unrolled carrier coefficient with source-order bound C^m(m!)^p and a single geometric age gain, polynomial tensor transport of its m slots therefore changes p by at most the one fixed integer d_ν. It does not introduce a cutoff-dependent factorial exponent.

The word **unrolled** matters. Applying (R3.24) afresh after each RG step would spend this exponent repeatedly and would not prove R3. Linear transport must first be composed using its exact cocycle; the actual source/contact forest must exhibit where its geometric gain is spent. That ownership statement is part of the missing analytic construction.

A bound merely of the form
‖M_k−I‖≤Cg_k²(log g_k⁻²)^q, q>0,
does not give (R3.23): its crude product can grow like
exp(C(log X_j)^{q+1}).
The resulting all-order optimization can exceed every fixed factorial power. A logarithmic loss that is harmless at a fixed insertion order is not automatically harmless for R3.

### 5.3 A common formal-source Banach algebra

For a Banach source space B and a Banach algebra A, let F_m be symmetric m-linear maps B^m→A. Define the factorial-weighted formal jet norm

\[
 \|F\|_{\tau,p}
 =\sum_{m\ge0}\frac{\tau^m}{(m!)^p}\|F_m\|_{\rm op},
 \qquad p\ge1 .
 \tag{R3.25; P: definition}
\]

The usual labelled Leibniz product obeys

\[
 \|FG\|_{\tau,p}\le
 \|F\|_{\tau,p}\|G\|_{\tau,p},
 \qquad
 \|\exp F\|_{\tau,p}\le e^{\|F\|_{\tau,p}} .
 \tag{R3.26; P}
\]

Indeed the r,s contribution, r+s=m, carries
\(\binom mr(r!)^p(s!)^p/(m!)^p
 =[r!s!/m!]^{p-1}\le1\).
Summation proves the product inequality, and the exponential follows by its power series. The same proof works in every finite jet truncation, with constants independent of the truncation order.

Thus connected polymer algebra, positive raw integration, bounded linear tensor projections and contact operators can be carried out in one fixed Gevrey norm when their actual operator and primitive bounds hold in that norm. The finite 21-dimensional tensor index space adds only fixed constants. This algebraic fact does not prove the required primitive norms, normalized denominators or collision-forest bounds.

A uniform finite complex source disk is a sufficient p=1 mechanism. It is not logically necessary for a fixed-p Gevrey construction. The polynomial running factors and one-shot memory estimate above give a second route, provided the complete historical source accounting is established before the bound is applied.

## 6. Fixed C⁵ contact regularity and a quantitative Schwartz extension

### 6.1 The contact Taylor remainder has no hidden insertion-order loss

Let B_m be an m-linear functional of source restrictions to a collar contained in
\(\{|x-z|_\infty\le hR\}\), with operator norm A_m on the product of componentwise supremum norms. The source value space may be any fixed finite-dimensional tensor space. Put

\[
 \|f\|_{5,\ell_0}^{\rm alg}
 =\sum_{|\alpha|\le5}\frac{\ell_0^{|\alpha|}}{\alpha!}
       \sup\|\partial^\alpha f\|.
 \tag{R3.27; P: definition}
\]

For \(f_{i,t}(x)=f_i(z+t(x-z))\), write b(t)=B_m(f_{1,t},…,f_{m,t}). Define the local contact projection by the Taylor polynomial of b at zero through degree four:

\[
 ({\cal P}_4B_m)(f_1,\ldots,f_m)
 =\sum_{\sum_i|\alpha_i|\le4}
   \frac{
    B_m\big((\,\cdot-z)^{\alpha_1}\partial^{\alpha_1}f_1(z),
       \ldots,
       (\,\cdot-z)^{\alpha_m}\partial^{\alpha_m}f_m(z)\big)}
    {\prod_i\alpha_i!}.
 \tag{R3.28; P: definition}
\]

It is supported on the full source diagonal at z. Applying it to appropriate proper collision clusters would produce partial-diagonal counterterms; the actual forest assigning those clusters is a separate construction.

**Proposition (P).** For all m≥1,

\[
 |(B_m-{\cal P}_4B_m)(f_1,\ldots,f_m)|
 \le A_m(hR/\ell_0)^5
       \prod_{i=1}^m\|f_i\|_{5,\ell_0}^{\rm alg}.
 \tag{R3.29; P}
\]

**Proof.** The fifth derivative of b is a sum over multiindices α_i with total order five. The exact coefficient is 5!/∏α_i!, and the product of all displacement factors is bounded by (hR)^5. The sum of the corresponding derivative-norm products is at most the product of the algebra norms (R3.27), divided by ℓ₀⁵. Thus
\(|b^{(5)}(t)|\le5!A_m(hR/\ell_0)^5\prod_i\|f_i\|_{5,\ell_0}^{\rm alg}\).
Taylor's integral remainder has total weight 1/5!, proving (R3.29).

There is no m⁵ factor: the exact multinomial sum is already bounded by the product of the factorially weighted finite-derivative norms. In particular, if A_m≤C^m(m!)^p, this contact subtraction preserves p. A rooted carrier decay pays R⁵ with a fixed exponent margin. The scale-j anchor count h_j⁻⁴ combines with h_j⁵ to leave h_j; its ultraviolet sum converges. Polynomial running factors of the m slots can then be handled once by (R3.24).

This proves an operator bound for admitted local source coefficients. It does not prove that every complete E/R/B coefficient has that source norm or that the required collision forest has been constructed.

### 6.2 Product-test bounds imply a Schwartz order growing only linearly in m

For simplicity rescale the fixed physical length to one. For a V-valued Schwartz function on R⁴, set
\(p_s(f)=\max_{|\alpha|\le s}\sup_x(1+|x|^2)^{s/2}\|\partial^\alpha f(x)\|\).
Suppose m-linear forms S_m obey, for one fixed integer s≥0 and p≥1,

\[
 |S_m(f_1,\ldots,f_m)|
 \le A^m(m!)^p\prod_{i=1}^m p_s(f_i).
 \tag{R3.30; C: the actual renormalized product-test bound to establish}
\]

**Theorem R3-C (P as a quantitative extension theorem).** They extend uniquely to Schwartz distributions on R^{4m} with values in the tensor index space, and there is a constant A', independent of m, such that

\[
 |S_m(F)|\le(A')^m(m!)^p\,q_{(2s+16)m}(F),
 \quad
 q_n(F)=\max_{|\alpha|\le n}\sup_{x\in\mathbb R^{4m}}
       (1+|x|^2)^{n/2}\|\partial^\alpha F(x)\|.
 \tag{R3.31; P under R3.30}
\]

The tensor norm may be any fixed Euclidean norm per factor; changing it only changes A'. For s=5 the explicit bound uses q_{26m}. The constant 26 is not optimal, but it is independent of the insertion order.

**Proof.** Let e_n be the normalized four-dimensional Hermite functions and let
\({\cal H}=1-\Delta+|x|^2\), with eigenvalues
λ_n=5+2|n|. Multiplication and differentiation are finite linear combinations of creation and annihilation operators. Fourier Cauchy–Schwarz gives the Sobolev bound
\(\|u\|_\infty\le C\sum_{|\alpha|\le3}\|\partial^\alpha u\|_2\)
in four dimensions. Applying it to polynomially weighted derivatives of e_n yields
\(p_s(e_n)\le C_s\lambda_n^{s+3}\);
the deliberately loose integer exponent suffices.

Expand F in products of these functions and in an orthonormal tensor-component basis. Equation (R3.30) bounds the value on a product basis element by
\((AC_s)^m(m!)^p\prod_i\lambda_{n_i}^{s+3}\).
Cauchy–Schwarz over all mode and component indices therefore gives

\[
 \sum_{n_1,\ldots,n_m}|c_{n_1,\ldots,n_m}|
       \prod_i\lambda_{n_i}^{s+3}
 \le C^m
 \|({\cal H}^{s+6})^{\otimes m}F\|_2 ,
 \tag{R3.32; P}
\]

because ∑_{n∈N⁴}λ_n⁻⁶<∞. The fixed finite tensor dimension contributes only another exponential constant.

For q=s+6, the differential operator H^q is a finite sum of polynomial coefficients of degree at most 2q multiplying derivatives of order at most 2q. Its m-fold product consequently has at most C_q^m such terms. The seminorm with n=2(q+2)m bounds each term pointwise by
\(C_q^m q_n(F)\prod_{i=1}^m(1+|x_i|^2)^{-2}\).
The product has L² norm C^m in dimension 4m. This proves (R3.31).

The Hermite series converges in every Schwartz seminorm after inserting sufficiently high oscillator powers. The displayed absolute sum therefore defines a continuous extension agreeing with the original multilinear form on tensor products; density gives uniqueness. No qualitative kernel theorem is needed in place of the quantitative order estimate. ∎

The theorem supplies the linear growth of distribution order needed in the corrected OS regularity route once the actual renormalized product-test bound has been proved. Bounds only for separated cell supports do not supply (R3.30) for arbitrary coincident tests. Their compatible contact extension must still be constructed. Likewise the theorem establishes neither reflection positivity nor an operator-relative energy estimate.

## 7. What one actual complex source bound would prove at every order

### 7.1 Cauchy extraction without a uniform zero-free hypothesis

Let the *same* vacuum prescription define the finite-cutoff normalized source functional

\[
 G_{a,T}(j)
 =\exp\!\left(-\sum_c L_a(j|_c)\right)
       \frac{Z_{a,T}[j]}{Z_{a,T}[0]},
 \qquad G_{a,T}(0)=1 .
 \tag{R3.33; C: actual normalized source functional}
\]

The sign is the preamble's sign: \(\log G=W^{\rm ren}\). Suppose the actual complete construction makes G holomorphic in every finite source family on one radius r>0, independent of a,T, for all 21 tensor components and the chosen scalar representative. Suppose further that for profiles f₁,…,f_m, each supported in at most B₀ admitted cells, the full physical estimate is

\[
 \left|G_{a,T}\!\left(\sum_{i=1}^m z_i f_i\right)\right|
 \le e^{C B_0m}
 \quad\hbox{whenever}\quad
 \sum_{i=1}^m|z_i|\|f_i\|_{C^5}\le r .
 \tag{R3.34; O: the actual complete-theory input}
\]

The estimate must hold for these profiles together, including overlaps. It is not an estimate of a product of separately normalized single-source partition functions. A verified active-cell version with \(e^{C n_{\rm active}}\) implies (R3.34).

**Theorem R3-D (P as an implication from R3.34).** The renormalized moment coefficients M_m and connected coefficients K_m of this one functional obey

\[
 \begin{split}
 |M_m(f_1,\ldots,f_m)|
 &\le A^m m!\prod_i\|f_i\|_{C^5},\\
 |K_m(f_1,\ldots,f_m)|
 &\le (2A)^m m!\prod_i\|f_i\|_{C^5},
 \qquad A=e^{C B_0+1}/r .
 \end{split}
 \tag{R3.35; P under R3.34}
\]

**Proof.** If one profile has zero norm the claim follows by multilinearity. Otherwise use the polydisc radii
\(\rho_i=(1-\varepsilon)r/(m\|f_i\|_{C^5})\).
Multivariate Cauchy gives
\(\left|M_m\right|\le e^{CB_0m}[m/((1-\varepsilon)r)]^m\prod_i\|f_i\|_{C^5}\).
Let ε↓0 and use \(m^m\le e^m m!\). This proves the first estimate.

Since G(0)=1, its logarithm has a germ at the origin for each finite cutoff and finite source family. The exact cumulant identity is

\[
 K_m(f_1,\ldots,f_m)
 =\sum_{\pi\in{\cal P}([m])}
   (-1)^{|\pi|-1}(|\pi|-1)!
       \prod_{B\in\pi}M_{|B|}((f_i)_{i\in B}) .
 \tag{R3.36; P}
\]

For fixed block count l, summing the product of block factorials over partitions gives
\(\sum_{|\pi|=l}\prod_{B\in\pi}|B|!
=(m!/l!)\binom{m-1}{l-1}\).
Therefore the absolute combinatorial multiplier is

\[
 \sum_{\pi}(|\pi|-1)!\prod_{B\in\pi}|B|!
 =m!\sum_{l=1}^m\frac1l\binom{m-1}{l-1}
 =\frac{2^m-1}{m}\,m!
 \le 2^m m! .
 \tag{R3.37; P}
\]

This proves the second estimate. No ultraviolet-uniform zero-free radius of G, and no bound on \(\log G\) on a complex ball, was assumed. The only complex estimate used was the actual normalized estimate (R3.34). ∎

The subtraction in (R3.33) has mixed derivatives when two or more profiles meet. These are precisely part of its contact prescription. The theorem does not identify a coefficient for coincident profiles with a product of independently renormalized one-field operators. That identification, where required for an OS field algebra, needs the compatible field-valued and vacuum contact construction.

### 7.2 The additional covering input needed for arbitrary Schwartz profiles

Functions supported with margin in the cells of one fixed tiling do not cover the neighborhoods of that tiling's faces. Thus the fixed-grid chessboard conclusion alone cannot be applied to an arbitrary Schwartz test by an unsupported partition of unity.

A sufficient additional *geometric and prescription-compatibility* input is a finite family of translated cell grids and a smooth, uniformly locally finite partition of unity \((\psi_c)\) subordinate to interiors with margin of those cells. The same normalized hierarchy must satisfy (R3.35) for finite tuples drawn from this cover; its definition must be independent of which cover decomposes a profile. The cover itself is elementary. The extension of the physical estimate and counterterm prescription to it is an actual input, not a consequence of elementary geometry.

Assuming that compatibility, each \(\psi_cf\) is admitted with uniform derivative bounds, and in four dimensions

\[
 \sum_c\|\psi_cf\|_{C^5}
 \le C\,p_5(f),\qquad
 p_5(f)=\max_{|\alpha|\le5}
      \sup_x(1+|x|^2)^{5/2}\|\partial^\alpha f(x)\| .
 \tag{R3.38; P for a fixed uniformly locally finite cover}
\]

Indeed the Leibniz formula costs a fixed constant, every support has bounded diameter, and the sum of \((1+|c|^2)^{-5/2}\) over a four-dimensional cell grid converges. Apply the multilinear estimate to finite decompositions and then use absolute convergence. The result is

\[
 |M_m(f_1,\ldots,f_m)|+
 |K_m(f_1,\ldots,f_m)|
 \le A_1^m m!\prod_i p_5(f_i).
 \tag{R3.39; C on the complete source bound and cover compatibility}
\]

Theorem R3-C now gives a general Schwartz-distribution extension with seminorm order 26m and fixed factorial exponent one. This explicitly completes the analytic-source-to-OS-growth implication. It does not prove the actual analytic-source estimate. The running-transport approach in §5 is a different sufficient route: a fixed Gevrey exponent can be obtained without a fixed analytic radius if its complete renormalized coefficient norm and one-time memory budget are proved directly.

## 8. Exact remaining R3 propositions and construction

### 8.1 Why two-jet closure alone cannot be upgraded to R3

There is a simple positive-probability obstruction to an inference from uniformly controlled first and second jets and finite-cutoff analyticity to an all-order estimate. For M≥1 let a random variable X_M take the values M and −M, each with probability 1/(2M²), and zero otherwise. Then

\[
 \mathbb E X_M=0,\qquad
 \mathbb E X_M^2=1,\qquad
 \mathbb E e^{zX_M}
 =1-M^{-2}+M^{-2}\cosh(Mz),\qquad
 \kappa_4(X_M)=M^2-3 .
 \tag{R3.40; P}
\]

Every finite-M generating function is entire, with uniformly bounded first two derivatives, while even its fourth connected derivative is unbounded. This is not a counterexample to Yang–Mills R3. It demonstrates the logical insufficiency of that proposed bootstrap. The regular scalar disk theorem succeeds because it proves the additional nonlinear holomorphic derivative bounds and one summable feedback budget, rather than appealing only to the previously controlled jets.

The logarithmic refinement of the tensor-flow requirement in §5 also matters quantitatively. If the only available transport estimate were
\(\rho_n=\exp(b[\log(1+n)]^{q+1})\) with b,q>0, then

\[
 \sum_{n\ge0}e^{-an}\rho_n^m
 \ge \exp\!\left(-am+
       bm[\log(1+m)]^{q+1}\right) .
 \tag{R3.41; P}
\]

For every fixed constants A and p, this exceeds \(A^m(m!)^p\) for all sufficiently large m: the logarithm of the latter is at most \(m\log A+pm\log m\). Thus a logarithmically enhanced drift estimate that produces this transport growth is not enough for the particular one-time geometric-memory argument. Either the actual marginal drift must be sharpened, or the complete scale/insertion organization must exploit additional cancellations or decay. A claim that arbitrary logarithmic losses automatically fit a fixed factorial exponent is false.

### 8.2 The physical inputs still missing

The following are distinct actual-theory propositions. They must use the same Wilson/clover action, the same finite-cutoff normalization and one compatible contact prescription.

| Label | Actual proposition still required | What this note already supplies |
|---|---|---|
| R3-a (O) | Admit position-dependent sources in every retained tensor channel through the actual regular E, renormalized large-field R and boundary B activities, including all incoming histories and their masses. Prove the admitted norms from the actual preceding step. | One common disk for constant-scalar regular feedback, conditional on the existing physical R0-reg dictionary; the exact bare tensor domination and scalar artifact identity. |
| R3-b (O) | Identify the actual universal bulk marginal derivative, its seven sector coefficients after a valid scalar-representative choice, and quantitative invertible transport. Match this derivative with the coefficient in the complete sourced induction; account for any remaining history-dependent dimension-four terms. | The exact seven-sector decomposition and the polynomial-cocycle theorem under the explicit near-identity estimate (R3.22). |
| R3-c (O) | Construct the full source/contact recursion at every order. At collisions, retain both vacuum-valued and field-valued counterterms; show that derivative orders, graph combinatorics and locality norms admit one factorial exponent independent of scale depth. | A fixed-C⁵ Taylor remainder with no order-dependent derivative loss; a source-series Banach algebra; a one-time polynomial-memory bound. |
| R3-d (O) | Prove the actual normalized all-history majorant, or the actual complex normalized source estimate (R3.34), with the identical deterministic vacuum subtraction on all branches and all admitted tori along the selected cofinal family. | Exact implications from such an estimate to moment and connected bounds; no spurious uniform zero-free assumption. This is the R2 interface needed here, not a result established by R3's algebra. |
| R3-e (O) | Extend the local source/contact bounds compatibly to all coincident product tests and to a source cover sufficient for arbitrary Schwartz profiles. The same prescription must define the continuum distributions and, later, the reflected field algebra. | Explicit covering criterion (R3.38) and the quantitative Schwartz extension with derivative order at most 26m when s=5. |

The field-valued contact requirement in R3-c is substantive. Several dimension-four insertions can have a collision whose local output is another dimension-four field. The corresponding coefficient is nonlinear in the source and multiplies that field; it is not removed merely by a vacuum functional L_a. A complete scheme may absorb it into a nonlinear source-coordinate map or keep it as a local contact activity, but must define and estimate it. The positive bare action budget does not control the signed cancellations creating this renormalized contact coefficient.

The literal bare Wilson scalar together with all 21 clover channels is a 22-coordinate source system. The trace-clover/Wilson difference is the artifact in §4, not an exact finite-cutoff null source. An implementation that keeps both scalar representatives must retain their two-by-two invariant scalar block, or prove a triangular separation between one physical scalar marginal and its artifact remainder. Discarding the second scalar without that estimate changes the actual induction.

### 8.3 Scope of the completed modules

The new uniform-disk theorem does remove a specific regular scalar all-order gap: once the existing physical coordinate dictionary is supplied, no further scalar coupling-flow differentiability hypothesis beyond the actual regular holomorphic map is needed. The exact tensor decomposition removes ambiguity about the number of marginal channels. The positive remainder formula identifies the precise finite-cutoff scalar redundancy and its regular-field improvement. The Gevrey, contact and Schwartz theorems remove several abstract order-growth steps from the list of unresolved analysis.

They do not establish the incoming full-history tensor norms, the seven actual marginal coefficients, or the normalized collision hierarchy. In particular neither the one-link SU(2) calculation in [Wilson action lower bounds and the first SU(2) integration](wilson_action_and_first_integration.md) nor the one-scale constrained tensor Hessian calculation in [Tensor quadratic admission and the marked transition](tensor_quadratic_admission.md) constitutes these missing repeated-integration estimates.

**Full R3: O.** No stronger numerical form of N2-F has been assumed here. The original N1-S assertion of a uniformly bounded tensor transport and its inverse has not been proved by allowing polynomially running normalization. Such an alternative normalization must continue to state its distinct normalization explicitly. Establishing R3-a through R3-e, together with the remaining R1/R2 physical inputs, would turn the quantitative implications in this note into the target all-order hierarchy theorem. Continuum Euclidean symmetry restoration, reflection-positive compatibility, energy bounds and non-triviality remain separate requirements for YM-E.
