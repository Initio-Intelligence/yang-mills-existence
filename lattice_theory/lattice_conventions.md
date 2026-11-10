# Lattice conventions and hypotheses

## 1. Target, lattice, and source conventions

**Target.** Construct the existence-only YM-E hierarchy described in Section 5 below. At the continuum level the curvature-pair source space is the full pair-antisymmetric, pair-symmetric space; the observable notes in this directory give its 21-dimensional decomposition. The identity is an additional field. At finite lattice spacing the Wilson scalar and the clover scalar are distinct representatives; their difference must be controlled as an artifact.

**Status convention.** P means proved with the displayed hypotheses, L means a checked literature assertion in its stated scope, C means its Yang–Mills application still depends on an explicit unproved premise, and O means open. None of the conditional applications below is an extra assumed interface.

Let \(G=SU(N)\), \(N\ge2\), in the fundamental representation. Haar measure on every link is normalized. The lattice is \(\Lambda_{a,T}=(a\mathbb Z/T\mathbb Z)^4\). A positive link is \(b=(x,\mu)\), with variable \(U_b\in G\). The oriented forward plaquette has holonomy
\(U_p=U_{x,\mu}U_{x+a\mu,\nu}U_{x+a\nu,\mu}^{-1}U_{x,\nu}^{-1}\), \(\mu<\nu\).

\[
s_p=N-\operatorname{ReTr}U_p,\quad
S=\sum_p s_p,\quad
d\mu_{a,T}=Z_{a,T}^{-1}e^{-\beta_a S}\,d\mathrm{Haar},
\quad
\beta_a=\frac{2N}{g_0^2}=2Nx_0.
\tag{C1; P: definitions}
\]

Fix an admitted odd block factor \(L\), a physical terminal length \(\ell_0\), and \(a=L^{-K}\ell_0\). Write \(h_k=L^ka\), \(N_k=(T/h_k)^4\), and \(N_T=N_K\). The construction may select one cofinal geometry satisfying the primary construction; it does not claim every nominal \(L\ge3\) or every compatible torus.

Balaban uses normalized trace \(\operatorname{tr}=N^{-1}\operatorname{Tr}\), so its plaquette is \(a_p=s_p/N\). The exact bare conversion is

\[
X_{B,0}=N\beta_a=2N^2x_0,\qquad
g_{B,0}=g_0/(\sqrt2\,N).
\tag{C2; P}
\]

The running-coordinate identification must be checked with the same extraction prescription. A bare conversion alone is not that check. This is recorded as ICR-N1-1 in Section 4.

Sources have a real scalar component \(j^{(0)}\) and a tensor \(j^{\mu\nu\rho\sigma}\), antisymmetric within each index pair and symmetric between pairs. Their lattice values come from \(C^5\) functions with the fixed physical derivative norm
\(\sum_{|\alpha|\le5}\ell_0^{|\alpha|}\sup|\partial^\alpha j|\le r_0\).
For the consistently based four-plaquette clover, put
\(\widehat F_{\mu\nu}=\mathsf P_{\rm tr}\frac18\sum(P-P^{-1})\) and
\(Q_{\mu\nu\rho\sigma}=\operatorname{ReTr}(\widehat F_{\mu\nu}\widehat F_{\rho\sigma})\).

\[
S_a[j]=\sum_p(\beta_a-j^{(0)}(x_p))s_p
-\sum_xj^{\mu\nu\rho\sigma}(x)Q_{\mu\nu\rho\sigma}(x),
\qquad
Z_{a,T}[j]=\int e^{-S_a[j]}\,d\mathrm{Haar}.
\tag{C3; P: definitions}
\]

With independent pairs \(A=(\mu<\nu)\), \(B=(\rho<\sigma)\), the coefficient of \(\sum_{A,B}Q_{AB}\) is \(J_{AB}=4j^{\mu\nu\rho\sigma}\) when the original tensor sum is over all ordered indices. Keep this factor and the sign \(Q_{AA}\le0\).

Cells have side \(\ell_0\), and supported sources have margin \(\ell_0/8\). P2's lower-vertex plaquette label is not exactly covariant under every cell reflection; ICR-N1-2 states a symmetric discretization alternative. The revised construction may instead prove that the original-placement defect vanishes after renormalization.

**Important distinctions.** The auxiliary background variable \(J\) in Balaban's complex domains is not the physical source \(j\). In the regular coupling proofs, \(H_j\) means the unprojected fresh E activity; vacuum and Wilson subtraction occur when assembling the old effective action. Pure Gaussian \(\log g\) vacuum normalizations are tracked separately. The logarithmic raw cutoff is \(\theta(g)=Ag(\log g^{-2})^p\); the rescaled free-coordinate cutoff is \(R(g)=\theta(g)/g\).

## 2. The sole assumed numerical interface, verbatim

> **(N2-F) Coupling flow.** There are constants γ ∈ ]0, 1], b_0 > 0, C_r < ∞, depending only on N, L and Balaban's fixed construction constants, such that for every K ∈ N and every g\_\* ∈ ]0, γ/2] there is a bare coupling g_0 = g_0(K; g\_\*) with the following properties. Let x_k = g_k^{-2}, k = 0, …, K, be Balaban's effective couplings for the theory on Λ\_{a,T}, a = L^{-K} ℓ_0 (x_k is the coefficient of the Wilson term in the inductive representation of ρ_k, in the normalization in which x_0 = g_0^{-2} = β_a/(2N); by N0's dictionary D2 it does not depend on the torus T). Then: (i) x\_{k+1} = x_k − b_0 log L + r_k(x_k) with |r_k(x)| ≤ C_r/x for all 0 ≤ k < K and all x ≥ γ^{-2}; (ii) g_k ≤ γ for all 0 ≤ k ≤ K; (iii) g_K = g\_\*; (iv) x_0 = b_0 K log L + O(log(K+1)) with the O depending only on (N, L, g\_\*); (v) g\_\* ↦ g_0(K; g\_\*) is continuous on ]0, γ/2]; (vi) each r_k extends to a function of x that is C^1 on [γ^{-2}, ∞) with |r_k′(x)| ≤ C_r/x². Here b_0 is the one-loop coefficient in the normalization x = g^{-2} (expected value 11N/(24π²) for SU(N); the value in the preamble's conventions, with its derivation, is to be supplied with N2).

Only N2-F is an assumed interface. Its literal coefficient sentence conflicts with the unnormalized Wilson convention (C1); the working arguments use its numerical recurrence in its own variable until the running-coordinate dictionary is verified. They do not infer a theorem from inconsistent normalization sentences. The common-family derivative interpretation is not added. See ICR-N1-1 and ICR-N1-3 in Section 4.

## 3. Original N1-S target, verbatim

**Status: not proved.** The literal initial Wilson coefficient has the proved normalization obstruction recorded in Stability with spatially varying Wilson couplings. The normalization-consistent scalar and tensor completion remains open. The R1–R3 construction is an observable-hierarchy argument and is not identified with this stronger all-source, all-torus interface.

> **(N1-S) Base with sources.** There is r_0^\* > 0 depending only on (N, L, γ) such that for every r_0 ∈ ]0, r_0^*], every j ∈ 𝒥(r_0), every K ∈ N with a = L^{-K} ℓ_0 and g_0 = g_0(K; g\_\*) as in N2-F, and every compatible torus T, there are a functional E\_{a,T}[j] ∈ R and constants b\_+, b\_−, b_0, C_L, C_e, C_Z < ∞ depending only on (N, L, ℓ_0, γ, g\_\*, r_0) — never on a, T, j — such that: (i) Z\_{a,T}[j] = exp(−E\_{a,T}[j]) ∫ ρ_K[j] dν_T, where ν_T is the reference measure on step-K configurations identified in N0 (Haar or Balaban's gauge-fixed measure) and ρ_K[j] ≥ 0; ρ_K[j] ≤ e^{b\_+ N_T} ν_T-a.e.; and ρ_K[j] ≥ e^{−b\_− N_T} on a ν_T-measurable set of measure ≥ e^{−b_0 N_T}. Hence |log Z\_{a,T}[j] + E\_{a,T}[j]| ≤ (b\_+ + b\_− + b_0) N_T. (ii) (Locality of the counterterm in the source.) E\_{a,T}[j] − E\_{a,T}[0] = −Σ\_{cells c ⊂ Λ\_{a,T}} L_a(j|*c) − R*{a,T}[j] with |R\_{a,T}[j]| ≤ C_L N_T, where L_a maps restrictions of sources to a single cell (with margin) to R, does not depend on T or on the cell (covariance under the translations of the cell grid), satisfies L_a(0) = 0 and L_a(Θj) = L_a(j) for every reflection Θ in a face of the cell (with the tensor transformation of j^{μνρσ}), and for every finite linear family j = Σ_i λ_i f_i of cell-supported sources the map λ ↦ L_a(Σ_i λ_i f_i) is real-analytic on {Σ_i |λ_i| ‖f_i‖*{C^5} ≤ r_0}. (iii) Consequently W^{ren}*{a,T}[j] := log(Z\_{a,T}[j]/Z\_{a,T}[0]) − Σ_c L_a(j|*c) satisfies |W^{ren}*{a,T}[j]| ≤ C_W N_T for all j ∈ 𝒥(r_0), with C_W := 2(b\_+ + b\_− + b_0) + C_L, uniformly in a and T. (iv) For the chessboard replication Wj of a cell-supported source j with margin (Wj ∈ 𝒥(r_0)), L_a((Wj)|\_{c′}) = L_a(j) for every cell c′. (v) (Inductive form with sources.) For every k ≤ K, ρ_k[j] has Balaban's inductive form (N0 dictionary D2) with Wilson term Σ_p x_k(y_p) s_p(U_k), where x_k(y) = x_k − j^{(0)}*k(y)/(2N) + e_k(y), |e_k(y)| ≤ C_e r_0, and with the clover term Σ_y (Z^{(k)} j_k)^{μνρσ}(y) Q*{μνρσ}(U_k; y), Z^{(k)} an H_4-covariant linear map of the dimension-4 tensor space with ‖Z^{(k)}‖ + ‖(Z^{(k)})^{-1}‖ ≤ C_Z; all other terms (E-, R-, B-terms) obey Balaban's bounds with constants independent of a, T, j, k. The sourced couplings satisfy x_k(y) ≥ γ^{-2}/2 for all y.

The original scalar specialization is obtained by setting the tensor source to zero. It is also not proved as a complete theorem. A counterterm chosen arbitrarily from the exact partition function would not constitute the prescribed local counterterm recipe.

## 4. Interface clarifications ICR-N1-1 to ICR-N1-3

No new premise is imposed on N2-F. Two convention clarifications are stated, followed by an explicit common-family compatibility statement. The quantitative complex tube in (4.101) is a residual theorem to prove for the actual construction, not an additional assumed interface.

Section and equation numbers cited below refer to the underlying proof development, not to this file. These statements are not assumed additional interfaces.

**ICR-N1-1 — against P2/N2-F's coefficient dictionary.** Preserve the specified bare theory and state:

> The running variable \(x_k=g_k^{-2}\) is the Wilson coefficient after a prefactor \(2N\) has been extracted. In the P2 fundamental-trace convention, the sourced Wilson contribution is \(2N\sum_p x_k(y_p)s_p(U_k)\). At the bare scale its coefficient after extraction is \(x_0-j^{(0)}(x_p)/(2N)\). The coefficient in Balaban's normalized-trace action is \(X_{B,k}=2N^2x_k\), with the same plaquette indexing. All beta-function coefficients, coupling thresholds, and remainder constants imported in the variable \(X_B\) are converted accordingly.

The exact bare conversion is (2.1). The request also fixes the provisional expected one-loop value consistently with the literal P2 theory:

> With \(\operatorname{Tr}(T^aT^b)=\delta^{ab}/2\) and conventional Yang–Mills coupling \(u\), the literal P2 action has \(g_0^2=Nu^2\). Its formal one-loop coefficient in \(x=g_0^{-2}\) is \(b_0=11/(24\pi^2)\); \(11N/(24\pi^2)\) is the coefficient in \(u^{-2}\).

Section 4.20 proves this convention conversion from the checked formal coefficient. The running identification and the nonperturbative flow remainder still require their matching proof. Neither quoted interface is modified.

**ICR-N1-2 — against P2's scalar source placement.** Under a reflection in a coordinate contained in a plaquette, its initial-vertex label acquires a one-link displacement. Thus a lower-vertex scalar weight does not transform by ordinary site pullback alone. One exact reflection-covariant alternative is
\(\bar j_p=\frac14\sum_{v\in\mathrm{vertices}(p)}j(v)\), with
\(O^{(0),\mathrm{sym}}_a(x)=a^{-4}\sum_{p:x\in p}s_p/4\).
Another is a consistently specified plaquette-center convention. If the original discretization is kept, its placement defect must instead be controlled through the renormalized construction. A pointwise \(O(a)\) difference is not by itself a uniformly negligible ultraviolet error.

**ICR-N1-3 — against the common-family quantification in N2-F.** The exact requested additional statement is:

> For each fixed \(K\), the functions \(r_{K,k}\) in clauses (i) and (vi) may be chosen jointly for all terminal \(g_*\) in any fixed compact subinterval of \(]0,\gamma/2[\), and the resulting recurrences give the Wilson coefficients of the same source-free extraction recipe at the corresponding bare couplings. Their bounds use the same \(C_r\).

**Status: O, requested clarification or strengthening; not assumed.** Proving this compatibility from the source-free recipe would discharge it. It is needed to identify the derivative of selected numerical recurrence functions with the derivative of the actual neighboring coefficient family. The quantifier order of N2-F as stated does not explicitly exclude trajectory-dependent choices of the extensions. Section 4.15 therefore keeps the numerical tangent P and the physical identification C. The request adds neither a second derivative nor a response theorem for arbitrary irrelevant perturbations. Even with this compatibility, Proposition 4.15.1 shows that a uniform second response still requires another estimate.

The substantive remaining estimates are residual propositions within this work. Except for this explicit compatibility request, they are not relabelled as extra N-interfaces, and none is added to the assumptions.

## 5. Full existence-only target and proof strategy

The target is a subsequential continuum and infinite-volume theory for SU(N), N≥2, generated by the identity and all components of Tr(F_{μν}F_{ρσ}). Its renormalized Schwinger hierarchy must satisfy corrected Osterwalder–Schrader regularity E0′, including temperedness and the required linear growth on the test space with the prescribed contact subtractions; full translation and O(4) covariance with the tensor transformation laws; reflection positivity; and permutation symmetry. Full Schwinger moments and connected derivatives of W are distinguished and converted by their exact partition formulas.

For each reconstructed field, the target also requires polynomial energy bounds of the form ‖φ_α(f)(1+H)⁻ⁿ‖≤C_f on the domains needed for the stated pure-phase decomposition. Nontriviality means the scalar field in a selected pure component has the asymptotically free short-distance two-point law and the specified nonzero connected three-point coefficient at its first nonzero interaction order. The error must be small relative to that order. A mixed-state coefficient alone does not supply the phasewise conclusion.

The target does not require a mass gap, confinement, uniqueness of the vacuum before decomposition, uniqueness of the continuum or infinite-volume limit, or the clustering axiom before phase selection. It does not require an operator product expansion as a general theorem, or observables of dimension at least five, apart from the finite artifact family needed internally for covariance control.

The construction retains the literal Wilson/clover observables and one consistent local renormalization prescription. It may freeze all transformations at zero source and construct their derivatives directly. It may select one cofinal sequence of geometries actually admitted by the source-free construction. It may use a specified running normalization for the finite field family and finite jets with a single fixed factorial exponent, instead of the stronger finite-source tensor-inverse bound in original N1-S. These are choices of proof strategy, not changes to the quoted interface.

No conclusion called R1, R2 or R3 is assumed. The results in this repository prove local components and analytic implications. The exact actual-theory inputs still needed are listed in [THEOREMS_AND_OPEN_PROBLEMS.md](../THEOREMS_AND_OPEN_PROBLEMS.md). The original N1-S formulation, including its Theorem 3.1 and scalar specialization, retains its negative/open status; the notes in this repository provide the proof development.
