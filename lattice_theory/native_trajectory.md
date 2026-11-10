# Native base and trajectory admission

This paper preserves N0 and N2. Its main trajectory target is **not proved**. It supplies an exact base interface, a native incremental value modulus and fixed-depth endpoint transfer, quantitative consequences of an admitted trajectory, and a full-state forward shooting theorem. The completed direct argument is §§9 and 12: a Gaussian reserve estimate for the native complete fluctuation action, avoiding the unused cross-volume copying approach retained in §4. Neither an endpoint nor a bounded individual coefficient supplies positive cumulative drift.

Status labels: **P** means a deduction proved here; **L** means a checked native statement within its hypotheses; **C** means an application conditional on an explicitly unproved estimate; **O** means open. Section 12 proves the native incremental value modulus and the fixed-depth EP transfer for the specified fixed-cutoff/readout family, using the projector identification (12.13). This supplies the native inputs left open in §§3–5, 8–9 and 11; it does not establish the unused decorated-support construction in §4. The all-depth F-admit and F-AF interfaces remain O. Section 10's mathematical full-state implication is proved, with its unverified signed-drift premise stated.

## 1. Fixed construction and actual objects

Fix SU(N), an admitted sufficiently large odd L, the (0.12)/(0.10) block average of CMP109, its fixed physical cutoff (2.9), and all of the native constants in N0. Alternative g-dependent cutoffs are not substituted. Write

\[
 S=\sum_{p,\,\mu<\nu}(N-\mathop{\rm ReTr}U_p),\quad A_B=S/N,
 \quad X_B=2N^2x=N\beta,\quad g_B=X_B^{-1/2}.
\]

All link measures are normalized product Haar; one unoriented plaquette is counted once. The bare density is exp(-X_B A_B)=exp(-2NxS). The conventional inverse squared coupling Y is Nx. Thus a standard decrement 11N/(24π²) per logarithmic length corresponds to 11/(24π²) in x and 11N²/(12π²) in X_B. This conversion does not evaluate a native finite step.

The native scalar at step j is the infinite-lattice polarization moment of the **combined** generated term, including its Gaussian normalizer. In native units,

\[
 X_{B,j+1}=X_{B,j}-\beta_{j+1}(g_{B,j};g_{B,0},\ldots,g_{B,j-1}).                 \tag{1.1}
\]

The semicolon is essential. CMP109 printed p.298 expressly says that the displayed beta function also depends on all preceding couplings. The current scalar alone is not a proved state variable. The full state includes the complete incoming localized action and its fixed construction data. The source uses the small-field beta coefficients in the full large-field representation; there is no extra R beta correction in (1.1).

For a real external coarse link field B, let U_{j+1}(exp(iB)) be the regular constrained classical minimizer, and let E^{[j+1]} be the generated term in the second representation (1.6). With the color delta suppressed,

\[
 P_{j+1,\mu\nu}(g;x,x')=
 \left.\frac{\delta^2 E^{[j+1]}(g,U_{j+1}(e^{iB}))}
 {\delta B_\mu(x)\delta B_\nu(x')}\right|_{B=0},
 \qquad \beta_{j+1}=\sum_z P_{j+1,\mu\nu}(g;z)z_\mu z_\nu\quad(\mu\ne\nu).       \tag{1.2}
\]

The infinite-volume limit precedes the spatial moment. The displayed sign and moment are those of CMP109 printed p.264, (1.20)–(1.22). All comparisons in this paper use this common projection.

## 2. B: the exact positive base and its limits

**L/P, imported from N0 §§2–4 and Appendix C.** On a compatible finite torus and along a sequence satisfying the native weak-coupling and interscale hypotheses, the exact transformations preserve the Wilson partition integral. The positive history lift consists of the original positive integrals, partitions of unity, normalized gauge identities and normalized positive reference ratios before signed cluster reorganization. Its pushforward is the complete R-renormalized density. The outer coarse measure remains product Haar. One has

\[
 \chi_j(V)\exp\{-X_{B,j}A_B(U_j(V))-E_-N_j\}
 \le \rho_j(V)\le \exp(E_+N_j),\qquad N_j=(T/\ell_j)^4.                 \tag{2.1}
\]

The selector uses the localized minimizers, whereas the action in (2.1) uses the all-small global minimizer. The lower bound is not an unconditional positive constant, and (2.1) is not a normalized conditional patch law. Constants E± may depend on N, L and fixed construction constants, not on T, j or V in the theorem's admitted domain. Signed E/R/B polymer summands are not probabilities. For positive transport one retains the actual lifted integrals and every inherited term.

Choose physical terminal scale ℓ0, cutoff a_K=ℓ0 L^{-K}, and ℓ_j=a_KL^j. Let M=L^u, M2=L^v, R_j=L^{r_j}, where

\[
 R_j=\min\{L^n:L^n\ge(\log X_{B,j})^r\},\quad
 \epsilon_j=X_{B,j}^{-1/2}A_0(\log X_{B,j})^{p_0},\quad p_0\ge5r.
\]

The exact N0 cofinal choice is

\[
 d_K=\max_{0\le j\le K}\{j-K+u+r_j,\ j-K+1+v+r_j,\ 0\},\quad
 h_K=\max\{K,d_K+q,h_{K-1}+1\},\quad T_K=2\ell_0 L^{h_K},              \tag{2.2}
\]

with fixed L^q>1000 and a common centered grid shift. It tiles every native MR_jℓ_j and LM2R_jℓ_j block. This is a cofinal construction once finite trajectories are supplied; it does not construct those trajectories.

No current-scale observable matching, retained-field moment bound, or spatial source response follows from B. O1 and O2 can use (2.1) and the exact lift with the trajectory dependence displayed.

## 3. Source readings and the finite-volume endpoint

**Note.** Section 12 supplies the volume- and depth-uniform remainder bound missing from the fixed-volume proof below. The exact source readings in §3.1 remain in force.

### 3.1 Precise readings of the source formulas

* CMP109 p.263 states fixed positive field-chart constants α0, α1 independent of X and j, with the analytic localized bound (1.18). These are the charts used below. The g-dependent CMP119 charts (2.28) cannot replace them in the endpoint argument.
* CMP109 p.268, (2.12), retains exactly the incoming difference E_j(U_j(e^{i[gCB-hD(gCB)]}V))-E_j(U_j(V)). Its prose states that the exponent in (2.13) vanishes at g=0. **Equation (2.14) itself is log N''_j=E^{(j+1)}(g_j,1), at the actual coupling.** It is a normalization identity, not an asserted zero-coupling limit.
* CMP116 p.21, (2.41), is
  \[
  |E^{(j+1)}(X)|\le O(1)C_3\epsilon_1
     \exp\{-(1-10\delta)\tfrac12 L\kappa d_{j+1}(X)\}.
  \]
  The choice (1-10δ)L/2=1 gives the required decay. The following paragraph adds log Z^{(j)}(U)-log Z^{(j)}(1) to obtain the combined representation (1.6). This addition must be made before projecting beta.
* CMP109 p.298 explicitly retains all previous coupling arguments. The current-g smoothness sentence on p.264 cannot by itself be differentiated along an unspecified coherent full-state trajectory.

### 3.2 Fixed-volume Laplace statement with an evolving inherited action

**Proposition 3.1 (P from the regular native chart/coercivity imports).** Fix a depth j and one finite compatible torus. Let all earlier generated actions lie in the native bounded analytic class on fixed smaller field charts. Their coupling parameters may vary arbitrarily within that class. In the regular fixed-cutoff integral (2.12) of CMP109, let the current g tend to zero. After division by the explicit Gaussian normalizer and normalization at external identity, the remaining logarithm tends to zero, uniformly over those earlier actions, on real external fields in a fixed smaller regular neighborhood. The corresponding statement holds for its external-field Hessian when the native holomorphic bound on that fixed neighborhood is retained.

**Proof.** Work in the independent real coordinates remaining after the actual nonlinear constraint and gauge elimination. The regular stationary point is at fluctuation zero. Its quadratic form is C*Δ^{(j)}C, including the constraint current and gauge contributions. On this fixed finite torus its eigenvalues have a positive lower bound throughout a compact smaller real background chart. The normalized Gaussian in (2.13) uses this very form.

After dilation, a fluctuation b in a fixed compact set gives physical displacement O(g|b|). The terms divided by g² have the quadratic terms already removed; their remainder is O(g|b|³). The coordinate/Haar densities tend to their value at zero. On the fixed physical cutoff, Taylor's estimate bounds the higher classical terms by c ε1 |b|²; choose ε1 small enough to leave a positive Gaussian quadratic bound. The inherited difference tends to zero uniformly on compact b sets: Cauchy estimates for the incoming fixed analytic charts give

\[
 |E_j(U_j(e^{i[gCb-hD(gCb)]}V))-E_j(U_j(V))|
 \le C_{j,T}\min\{g|b|,1\},                                               \tag{3.1}
\]

after increasing C_{j,T}; boundedness on the whole cutoff supplies the second alternative. Constants here may depend on j and T but not on the actual earlier coupling parameters. Smooth coordinate densities on the regular cutoff are bounded by another fixed constant. Thus the dilated integrand is dominated by C_{j,T} exp(-c_{j,T}|b|²). The cutoff tends pointwise to one. Dominated convergence gives the Gaussian ratio one. The same result at external identity subtracts the logarithmic normalizer.

For complex field derivatives one does not use a real positivity inequality at complex fields. Instead use the native uniform holomorphic bound on a fixed complex field neighborhood, convergence on the real neighborhood, and normal-family uniqueness; Cauchy then gives convergence of the Hessian on a smaller neighborhood. This proves the stated finite-volume result. ∎

This proof alone does not interchange the small-g and infinite-volume limits. Its constants may grow with T. Section 4 addresses that distinct point.

## 4. Fixed-depth endpoint transfer: the cross-volume construction

**Status of this section.** The decorated-support majorant (4.1) is not proved here, and localization alone does not prove cross-volume consistency. This section is a candidate route only; none of the EP/value-modulus conclusions of §12 uses it.

This section gives a candidate completed EP proof for the **regular, fixed physical cutoff scheme**, with its nontrivial copying step stated explicitly. It concerns no full large-field R history and makes no estimate uniform as j tends to infinity.

### 4.1 Native primitives used for copying

The argument needs equality of the same localized coefficient on embedded patches, not just a bound on its magnitude. The following are the construction clauses used to obtain that equality.

1. **Local propagator factors.** CMP99 p.394 defines the inverses by Dirichlet restriction Ω0ΔΩ0 and explains that they depend only on the field on that domain. Its pp.414–416 construct (3.107) from those finite-domain inverses, fixed partition functions and local differential/averaging operators. In particular the local matrix on an embedded domain, including its specified collar, is literally the same matrix in two ambient tori. Its inverse is therefore identical. CMP99 p.427 proves the corresponding domain-difference statement by cancelling all walks contained in the common region, (3.154).
2. **Nonlinear constraint/minimizer localization.** CMP116 pp.3–5, (1.6)–(1.10), multiplies each walk by its weakening variables s(Δ). At s(Y0^c)=0 all equations split into components. The solution on Y0 is determined by the restricted local operators and local B′; the unique small solution is the same in any ambient torus containing that patch. The text on printed p.4 proves this component restriction before (1.10), rather than merely asserting decay afterwards.
3. **Inherited terms.** The term localized in (1.23) is constructed from an old localized action and the just-described restricted nonlinear solution. Its complete support is the union with the old support, called Y in (1.24)–(1.29). Thus copying requires the old coefficient on that support to have been copied. This is an induction in generation; it is not an assumption that unrelated old actions have equal coefficients.
4. **The normalized fluctuation integral.** CMP116 pp.12–14 first conditions on Z0 and then localizes the remaining covariance/square root in (2.6)–(2.8) by exactly the same weakening procedure. At s(Z^c)=0 the coordinates outside Z factor as normalized product standard Gaussians and integrate to one. The integrand on Z is determined by the same finite-domain matrices and localized interactions. There is consequently no ambient-volume Gaussian constant left in this coefficient.
5. **Connected resummation.** CMP116 p.14, (2.9)–(2.13), constructs H(Z) and E(X) by unions of these supports and a numerical connected-graph coefficient. The overlap relation and graph coefficient agree for an embedded union. Absolute convergence permits regrouping. The Gaussian log normalizer is added separately by its closed random-walk expansion, as stated on p.21; its nonwrapping loops likewise copy.

These clauses yield the following induction. Start from the bare finite-range Wilson action. Fix the same periodic grids, local partitions, field chart and cutoff convention on all tori. At each generation construct every local coefficient by the formulas above, retaining its full determining support, including all collars and all ancestor supports. If that full support embeds in two tori, every matrix, small nonlinear equation, normalized finite-dimensional integral and connected-graph coefficient in its construction is identical. Hence the coefficients are identical. Coupling parameters are the same numerical history on both tori; the prescribed beta coefficients are infinite-lattice numbers and are not redefined by finite-box fitting. This proves copying for this coherent family, by induction in j.

The enlargement between a nominal support and the complete determining support costs a fixed factor c_j at fixed j. One may either retain decorated supports throughout or sum them into enlarged domains. Every local walk has its finite collar recorded, nonlinear localization takes unions, and there are only j generations. The native exponential bounds, with a fixed fraction reserved for the enlargement and polynomial counting, give

\[
 \sup_{\mathfrak h}\sum_{X\ni0,\,\operatorname{diam}\widehat X\ge R}
  \|E_{j,\mathfrak h}(X)\|_{\mathcal U'}\le C_j e^{-c_jR}.                  \tag{4.1}
\]

Here the supremum is over the admitted incoming histories, \(\widehat X\) is the full determining support, and \(\mathcal U'\) is a fixed smaller CMP109 chart. The constants may depend on j, N, L and the fixed construction constants, but not on the torus or on the numerical admitted history. One does not conclude this merely by enlarging a final support without recording its ancestor decorations: the sum of those decorations is bounded at the corresponding construction stage by the absolutely convergent native walk/cluster majorants.

### 4.2 Uniform fixed-depth thermodynamic approximation

For a periodic regular background U, take compatible tori of side T, all multiples of the background period. Normalize the generated logarithm by its value at identity and by the number of current sites. Denote this quantity p_{j,T,\mathfrak h}(U). Copy all full supports of diameter less than T/4. Their contributions per site agree with those of the infinite-lattice sum. Every unmatched or winding support has full diameter at least T/4. Equation (4.1) gives

\[
 \sup_{\mathfrak h,U\in\mathcal U'}
 |p_{j,T,\mathfrak h}(U)-p_{j,\mathfrak h}(U)|
 \le C_j e^{-c_jT}.                                                       \tag{4.2}
\]

Changing T/4 to T/c_j absorbs the support collars. A weaker modulus tending to zero would suffice. The same conclusion holds for the explicit Gaussian term, by the same closed-walk construction.

For an external coarse plane wave B of compatible finite period, the constrained minimizer on one period torus extends periodically to every multiple. The extension solves the same local constrained stationary equations; uniqueness of the regular constrained minimizer modulo the fixed gauge, imported in N0 from CMP102, identifies it with the minimizer on the larger torus. Thus the background arguments in the copied coefficients agree. One first fixes the wave period sufficiently large to accommodate the local native grids. No continuous constant-flux family on a fixed torus is invoked.

### 4.3 Endpoint and projection

Fix j. Apply Proposition 3.1 on a fixed torus T. Apply (4.2), uniformly in the admitted history, to compare its pressure to infinite volume. First choose T to make the two thermodynamic errors smaller than ε; then choose g so the finite-dimensional Laplace error is smaller than ε. Therefore the normalized residual pressure tends to zero at infinite volume for every sufficiently small real periodic background, uniformly over admitted incoming histories at this fixed j.

The native fixed complex chart gives uniform holomorphic bounds on the amplitudes of any finitely many plane waves. Normal-family uniqueness gives convergence of their amplitude Hessians. Compatible wavevectors with periods of the form 2L^m form a dense subset of the momentum torus. To pass from their Fourier coefficients to (1.2), use the uniform exponential tail of the polarization at this fixed j. Here is the relevant justification. Local analytic E(X) has uniform first and second field derivatives on a smaller chart. Its first derivative at identity vanishes by global color invariance. The external-field Hessian after substitution U_{j+1}(e^{iB}) therefore uses only first derivatives of the minimizer. These are the classical minimizing interpolation operators whose exponential localization is supplied by the CMP99 propagator construction. Convolving the two interpolation kernels with the support majorant (4.1) gives, with possibly smaller c_j,

\[
 \sup_{g,\mathfrak h}|P_{j+1,\mathfrak h}(g;z)|
 \le C_j e^{-c_j|z|}.                                                       \tag{4.3}
\]

The same bound holds for the Gaussian endpoint. Normal-family convergence in momentum on a smaller strip, or truncation of the weighted spatial sum and Fourier uniqueness, now yields

\[
 \lim_{g\downarrow0}\sum_z(1+|z|^2)
 |P_{j+1,\mathfrak h}(g;z)-P^G_{j+1}(z)|=0,                               \tag{4.4}
\]

uniformly over incoming histories within the fixed-j bounded native class. Thus the projected step coefficient tends to its Gaussian value. Along a physical bare curve, every earlier coupling tends to zero at fixed j: boundedness of the finitely many generated scalar coefficients in (1.1) implies X_{B,i}=X_{B,0}+O_j(1). Repeating the above argument at earlier steps matches the inherited endpoints. This is exactly the fixed-depth EP identification required in N2 Appendix I, provided the copying construction in §4.1, including (4.1), is established.

The conclusion is a value limit at fixed j. It asserts no uniform rate in j, no total history derivative, and no bounded cumulative adjoint correction. It does not establish F-admit. The Gaussian color obstruction may be transferred only after this endpoint argument and the common projection calibration are established.

## 5. First unresolved admission estimate

**Note.** The finite-coupling remainder input is supplied by (12.11)–(12.13). The signed Gaussian window in this section remains open.

F-admit remains open even if §4 is established. One needs information that survives j increasing with K. In program units the Gaussian cumulative decrement from N2 Appendix H is

\[
 D_k^G=2u_k-\frac{1-L^{-4k}}{8N^2}.                                      \tag{5.1}
\]

The explicit compactness correction has total variation at most 1/(8N²). No such bound has been proved for the adjoint sequence u_k. Even the weaker positive-window estimate

\[
 d_-(n-m)-B\le D_n^G-D_m^G\le d_+(n-m)+B,
 \qquad d_->0,                                                         \tag{5.2}
\]

is open. Its unresolved operator expression is the curvature coefficient of the actual constrained determinant/coarea combination. N2 I.3 writes it as the combination of log det(H+J*SJ), log det[J(H+J*SJ)^{-1}J*], and the actual coordinate/gauge density. A uniform curved readout row bound does not bound these trace derivatives.

In addition, (4.4) is not a depth-uniform finite-coupling estimate. A full-state proof could use (5.2) plus a uniform small error in the **physical cumulative drift**; no derivative or exact identical step increment is logically necessary for admission by a topological construction. But neither that cumulative estimate nor a closed full-state invariant region is proved here. The abstract scalar inverse theorems in N2 cannot be applied by suppressing the older state variables in (1.1).

The stronger F-AF target requires the numerical slope d=11 log L/(24π²), for example |D_k^G-dk|≤B plus finite-coupling errors whose cumulative size is o(K), and the same actual scalar/field convention. Identical finite one-loop increments are unnecessary. The present paper proves neither this aggregate slope nor the actual UV matching law.

## 6. Quantitative interface conditional on a supplied trajectory

The following elementary estimates are recorded so O1/O2 do not need an unnecessarily strong F-AF premise. Suppose an actual trajectory obeys

\[
 A+c_-(K-j)\le x_j\le A_++c_+(K-j),\qquad A>1,\quad c_->0.              \tag{6.1}
\]

The fixed endpoint and additive constants can be absorbed into A,A+. Write n=K-j and λ=2N².

**P conditional consequences.** For q>1,

\[
 \sum_{j=0}^{K}x_j^{-q}
 \le A^{-q}+\frac{A^{1-q}}{c_-(q-1)}.                                  \tag{6.2}
\]

For q=1 the same comparison gives
\[
 \sum_{j=0}^{K}x_j^{-1}\le A^{-1}+c_-^{-1}\log(1+c_-K/A).                \tag{6.3}
\]

If b≥0, q>1, then Σ_j x_j^{-q}(log(λx_j))^b is bounded uniformly in K by a constant depending on A,A+,c±,λ,q,b. This follows by the upper bound in (6.1) for the logarithm and the lower bound for the power; a logarithmic power times n^{-q} is summable. In particular native powers g_{B,j}^{2q} have this property. A mere g_B or g_B² error is not summable without additional scale factors.

The rounded radius obeys
\[
 (\log[\lambda(A+c_-n)])^r\le R_{K-n}
 <L(\log[\lambda(A_++c_+n)])^r.                                        \tag{6.4}
\]

Therefore every fixed physical collar of the form C ℓ_j R_j is bounded by
\[
 CL\ell_0 L^{-n}(\log[\lambda(A_++c_+n)])^r.                            \tag{6.5}
\]

Its sum over n is finite independently of K. The collar tends to zero as n tends to infinity; it need not shrink at a fixed terminal generation n. Replacing the radius by a fixed physical cell would lose this distinction. Any finitely many powers of log x_j or R_j can be included in a scale-weighted sum Σ L^{-σ(K-j)}(log x_j)^bR_j^c, σ>0.

These estimates give the radius and summability interface only. Native one-step and interscale comparisons such as CMP119 (2.6)–(2.9) must also follow from the eventual actual drift bound; (6.1) alone does not imply every printed comparison with its prescribed constants. No source-radius or field normalization follows from (6.1).

## 7. Constant and source ledger

| Result | Allowed dependence | Uniformity actually asserted |
|---|---|---|
| Base (2.1) | N,L,fixed construction constants and weak threshold | j,T and admitted external data in the native theorem |
| Finite-volume Laplace Proposition 3.1 | also j,T | admitted inherited actions on fixed smaller charts |
| Fixed-depth copying/endpoint §§4.1–4.3 | also fixed j | Candidate only; decorated-support majorant (4.1) not proved and not used |
| Native incremental modulus §12 | fixed N,L,construction constants and strict chart margins | j,T and actual admitted histories |
| Coarse Schur second moment §13 | same fixed constants and fixed penalty s | k,T |
| Radius/sums §6 | also c±,A,A+,ℓ0,q,b,r | K,j,T |
| Native positive-window drift (5.2) | desired N,L,fixed construction constants only | **not proved** |

| Primary clause | Use | Scope check |
|---|---|---|
| CMP109 pp.263–264, (1.18),(1.20)–(1.22), Theorem 3 | Fixed analytic charts, generated scalar and its moment | Small-field admitted sequence; not source derivatives |
| CMP109 p.268, (2.12)–(2.15) | Actual inherited difference, Gaussian extraction and identity normalization | Fixed physical cutoff, independent constraint coordinates |
| CMP109 p.298, final paragraph | Explicit older-coupling dependence | Rules out silently applying one-state inverse shooting |
| CMP99 p.394; pp.414–416, (3.107); p.427, (3.154) | Dirichlet local matrices and matching-walk cancellation | Regular fields and compatible local partitions |
| CMP116 pp.3–5, (1.6)–(1.10); pp.7–8, (1.23)–(1.29) | Exact component restriction including inherited supports | Small solution on fixed analytic charts |
| CMP116 pp.12–14, (2.5)–(2.13) | Localized normalized Gaussian integrals and connected coefficients | Keep covariance square root and denominator |
| CMP116 p.21, (2.41) and following paragraph | Absolute majorant and Gaussian addition | Does not itself compare different tori |
| N0 §§2–4, C.2; LFR II (0.1) | B and compatible cofinal geometry | Conditional on admitted actual trajectory |
| N2 H.4, I.3–I.4 | Explicit compactness transient and unresolved adjoint determinant | Abstract shooting hypotheses not imported as true |

## 9. Direct remainder estimate from the native fluctuation action

**Relation to §4.** This is a more direct endpoint route than §4: it uses a bound uniform in finite volume before taking either limit, and therefore does not need the decorated-support copying claim. The argument and its exact imports are stated explicitly. Sections 3–4 are retained, but §9, with the inputs supplied in §12, is the endpoint proof used here. It does not evaluate the Gaussian drift.

**Completion.** Section 12 supplies the three native inputs left open in this section, with the scope stated there. The square-root hypothesis in the lower-bound proof of §9.2 is replaced by §12.3, not retained as an extra assumption.

### 9.1 A pointwise bound for the complete inherited fluctuation action

Use the actual independent real Gaussian coordinates b after the constraints in CMP109 (2.12) have been solved. At a fixed real regular external field, write the residual integral as

\[
 I_{j,g}(U)=\mathbb E_{C_j(U)}\bigl[\chi_g(b)e^{V_{j,g}(U,b)}\bigr],
 \qquad V_{j,g}=P^{(j)}+\{E_j(U_j(\cdots))-E_j(U_j(V))\}.                 \tag{9.1}
\]

The cutoff is the fixed physical cutoff of CMP109 (2.9), expressed on the independent coordinates: each Lie-algebra coordinate has magnitude less than ε1/g. Fixed group-dimension constants can be absorbed when passing between component and Lie-algebra norms. The explicit Gaussian/coarea factor has already been removed. The residual logarithm used in the combined generated action is log I_{j,g}(U)-log I_{j,g}(1).

**Exact cutoff-coordinate check (P/L).** CMP109 printed p.267 defines h to be zero except on the solved bonds b0(c). Its nonlinear change is B_old=B_new-hD(B_new). Equation (2.9), printed p.266, tests only bonds outside {b0(c)}; these coordinates are unchanged by the nonlinear map. The subsequent dilation is B_new=g B_scaled. Linear elimination gives B_scaled=Cb, with C equal to the identity on the remaining independent bonds by their definition, printed p.268. Consequently the original selector is exactly the product of the independent tests |g b(bond)|<ε1. It equals one on ||b||∞≤g^{-1/6} for small g, after the fixed Lie-norm conversion. Bounds on eliminated bonds are consequences of the solved constraint, not additional indicators. This settles the cutoff part of the native-coordinate check for the fixed-cutoff small-field scheme. It says nothing about the full large-field selectors.

**Native imports, CMP116 printed pp.9–11.** Lemma 1, (1.33)–(1.36), is for the **complete inherited difference**, after its old marginal cancellations. It is analytic in the b-polydisc ||b||∞<ε1/g and has localized bound

\[
 |V'_j(Y,U,J,b)|\le C\epsilon_1 e^{-\kappa' d_j(Y)}.                     \tag{9.2}
\]

The constant is E0 C1 M^q exp(C2 κ1), fixed independently of j, the volume and the admitted numerical coupling history. The sum over all older generations has already been performed in this bound: p.9 explicitly uses the factor L^iη to sum those generations. No old-coupling derivative is being imported.

The other terms are localized in Lemma 2. In its construction, the terms divided by g² have their constant, linear and quadratic physical-fluctuation terms removed into the stationary value and explicit Gaussian. The remainder begins at degree three. The coefficient in the second-order Taylor-integral representation (1.40) is proportional to |B′|; in particular it vanishes at B′=0. All other localized terms have a bounded analytic expansion in gb and vanish at b=0. Thus one can use the displayed decomposition (1.42) with

\[
 V_j(Y,b)=\tfrac12\sum_{i,l\in Y}Q_j(Y,b;i,l)b_i b_l+V''_j(Y,b),
 \qquad Q_j(Y,0;i,l)=0,\quad V''_j(Y,0)=0.                              \tag{9.3}
\]

This vanishing refers to the decomposition constructed by (1.38)–(1.40), not to an arbitrary rewriting of V. It also follows term by term directly from CMP109 (2.12): the g^{-2} terms use D3, G3, the product (gCb)D2(gCb), D2(gCb)^2, or the third-order Wilson remainder. The log Jacobian and Haar terms instead belong to V'' and vanish at zero. The inherited localized differences vanish at zero because the weakened mean-field displacement is zero when b=0; each interpolation term starts with that displacement.

In (1.43) the bound on Q has both tree and volume decay. Reserving part of the decay absorbs |Y|², the two indices i,l, and support counting. All constants remain fixed. Radial Schwarz's lemma now gives, throughout the **entire** open cutoff polydisc,

\[
 |V''_j(Y,b)|\le Cg\|b\|_{\infty,Y}e^{-\kappa''d_j(Y)},\qquad
 |Q_j(Y,b;i,l)|\le Cg\|b\|_{\infty,Y}w(Y;i,l),                          \tag{9.4}
\]

where w has the summable tree/volume majorant just described. Indeed, for a bounded analytic f on the ball ||b||∞<ε1/g with f(0)=0, apply the one-variable Schwarz lemma to z↦f(zb/||b||∞). This gives |f(b)|≤(g||b||∞/ε1)sup|f|. A half-radius loss is unnecessary here.

Sum (9.4). Use ||b||∞,Y^r≤Σ_{i∈Y}|b_i|^r for r=1,3, and the native anchored support sum after reserving the indicated decay. One obtains the pointwise bound

\[
 |V_{j,g}(U,b)|\le Cg\sum_{i=1}^{n}(1+|b_i|^3)\quad\text{on }\chi_g=1.   \tag{9.5}
\]

The constant is independent of j,n,volume and numerical admitted history. Crucially, (9.5) treats the renormalized inherited difference as the single object in Lemma 1; it does not sum the absolute primitive beta counterterms over the history.

### 9.2 Uniform per-coordinate logarithm estimate

The real Gaussian covariances in (9.1) have uniform operator bound K0 and the square roots have uniform absolute row sum K1. These are the regular unit-lattice covariance estimates of CMP99, including the constrained/gauge convention; CMP116 p.13 constructs the square-root expansion by the integral (2.7) and the same generalized random-walk bounds. They apply on a fixed smaller regular real chart. No covariance of a full large-field law is asserted.

More precisely, CMP99 Theorem 3.15, printed p.432, (3.187), gives |C^{(j)}(y,y′)|≤B0 exp(-δ0|y-y′|), with B0 and δ0 depending on d and L only. Summing rows gives the operator bound. The square-root expansion on CMP116 p.13 uses the same localized resolvents and their row-summable majorants. Matching these operators to the independent coordinates in (9.1), including the eliminated bonds and all cutoff factors, is part of the native-coordinate check below; an exponential bound for a differently constrained Gaussian is not sufficient.

In particular CMP109 p.267 explicitly replaces the delta gauge of CMP99 (3.156) by exponential gauge. These covariances must not be equated. A sufficient weaker hypothesis for the lower bound is an exact factorization b=Lz with independent standard Gaussians z, at most Cn of them, and sup_iΣ_α|L_{iα}|≤K1; no symmetric square root is required. The exact gauge algebra supplied by O1 is: let V embed centered gauge parameters, K be the actual gauge rows, R=V(KV)^{-1}, P=I-RK. For a valid axial-complement covariance of the same constrained Wilson Hessian,

\[
 C_{\exp}=P C_{\rm ax}P^*+RR^*.                                       \tag{9.2a}
\]

The decomposition z=h+Rw, h∈ker K, gives the horizontal Wilson form plus |w|². If C_ax=L_axL_ax*, then L=(P L_ax,R) is a Gaussian factor. Native rank, uniform row bounds on the inclusions and P,L_ax,R, and boundedness of the local inverse KV remain required; finite-dimensional invertibility alone is insufficient.

Choose the native ε1 small enough that Cε1<1/(8K0). This is an additional explicit smallness inequality among the fixed construction constants, compatible with their existing hierarchy. Put R=g^{-1/6}. From (9.5) and the cutoff bound |b_i|≤ε1/g,

\[
 V_{j,g}(b)\le\delta_g(n+\|b\|_2^2)
       +C\epsilon_1\sum_i b_i^2\mathbf1_{|b_i|>R},\qquad
 \delta_g=C(g+gR)=O(g^{5/6}).                                           \tag{9.6}
\]

On ||b||∞≤R the cutoff is one for small g and

\[
 V_{j,g}(b)\ge-Cg(1+R^3)n\ge-Cg^{1/2}n.                               \tag{9.7}
\]

For completeness, the Gaussian reserve proof is as follows. Absorb δ_g||b||² into the Gaussian, paying O(K0δ_g)n in its log normalization; its tilted covariance is at most 2K0. Expand exp(cΣb_i²1_{|b_i|>R}) as a product of 1+(exp(cb_i²)-1)1_{|b_i|>R}. Choose t>0 with c+t<1/(4K0). For any selected set S,

\[
 \mathbb E\prod_{i\in S}(e^{cb_i^2}-1)\mathbf1_{|b_i|>R}
 \le e^{-tR^2|S|}\mathbb E e^{(c+t)\sum_{i\in S}b_i^2}
 \le\left[e^{-tR^2}(1-4K_0(c+t))^{-1/2}\right]^{|S|}.                   \tag{9.8}
\]

Summing subsets bounds the upper logarithm by n[O(δ_g)+O(exp(-tR²))]. For the lower bound write b=Lz using the row-summable Gaussian factor above (a symmetric square root is one option) and restrict each |z_α|≤R/K1. This implies ||b||∞≤R; its product probability has logarithm at least -Cn exp(-cR²), and (9.7) controls the integrand. Consequently

\[
 \frac1n\left|\log I_{j,g}(U)\right|\le Cg^{1/2}                       \tag{9.9}
\]

for sufficiently small g, uniformly in the cutoff dimension, volume, step j, real external fields in the fixed smaller chart, and actual admitted incoming histories. The exponentially small terms have been absorbed into the power bound. The number n of independent coordinates per coarse site is bounded above and below by fixed positive constants depending on N,L; hence the same statement holds per current coarse site. Subtracting the value at identity only doubles the constant.

This verifies the unmarked per-volume tail hypothesis of N2 I.5 using the complete native inherited-action bound. It is not a marked-source estimate.

### 9.3 From a pressure value estimate to the beta value estimate

This passage does not differentiate (9.9) as an inequality. The native analytic activity bound gives a separate uniform bound on a fixed complex **external field** chart. After substituting the analytic regular minimizing field, the per-site residual action on finitely many plane-wave amplitudes is analytic in a polydisc of radius ρ>0 and bounded by C. The constants can be chosen independently of j and volume using the regular minimizing-field bounds at their current scale. This assertion uses the fixed CMP109 charts, not the shrinking CMP119 chart parameters.

For a real-analytic function f(s,t) with |f|≤δ on the real square and a fixed complex bound giving |D^4 f|≤C, the four-point mixed difference with step h has error O(h²), while the difference itself is O(δ/h²). Choosing h=δ^{1/4} gives |∂s∂t f(0)|≤Cδ^{1/2}. The same symmetric difference handles a pure second derivative. Apply this with δ=Cg^{1/2}, and use real sine/cosine amplitudes in two polarization directions. Translation invariance identifies the per-site mixed Hessian with the Fourier polarization, up to fixed numerical factors. Thus, for compatible real momenta,

\[
 |\widehat P_{j+1}(g;p)-\widehat P^G_{j+1}(p)|\le Cg^{1/4}.              \tag{9.10}
\]

The Fourier bound passes to the native infinite-volume polarization at fixed g. No order of g and volume limits has been exchanged. The native fixed-chart local-activity bound, together with exponential locality of the linearized classical minimizing interpolation, supplies a uniform exponential polarization tail. As in §4.3, the first derivative of each gauge-invariant local action at identity is zero, so no second derivative of the minimizing field occurs in this Hessian. With that uniform tail,

\[
 |P_{j+1}(g;z)|+|P^G_{j+1}(z)|\le Ce^{-c|z|},                          \tag{9.11}
\]

Fourier inversion bounds each difference coefficient by Cg^{1/4}. Split the weighted sum at radius R0=c_0 log(1/g). The inner sum costs O(R0^6) in four dimensions, while the outer exponential tail can be made O(g^{1/4}). It follows that

\[
 |\beta_{j+1}(g;\mathfrak h)-\beta^G_{j+1}|
 \le Cg^{1/4}(1+|\log g|)^6.                                           \tag{9.12}
\]

This is a deliberately weak **value** modulus. It neither implies nor is used to infer any derivative in g or in the older couplings. Its significance is that the right-hand side tends to zero with a constant uniform in the step, provided the fixed-chart interpolation/tail import in (9.11) is certified with that uniformity. The finite-volume bound (9.9) itself does not need (9.11).

**Separation of inputs.** The native bound (9.2), quadratic coefficient bound (1.43), and exact independent-coordinate cutoff are taken from the printed sources. The Schwarz, Gaussian reserve and finite-difference arguments are deductions for their displayed hypotheses. Three details remain for (9.12) at this point: (a) the stated termwise zero-fluctuation vanishing through the particular localizations defining Q and V''; (b) matching the actual exponential-gauge covariance to uniform operator and Gaussian-factor row bounds, including the independent-coordinate inclusion; (c) the depth-uniform fixed external chart and exponential tail after the classical minimizer substitution. The small-cube cutoff issue is resolved above. A fixed-j version of the remaining checks suffices for EP; uniformity in j is needed below. Neither (9.9) nor (9.12) is established by §9 alone; the three details are supplied in §12.

## 10. Full-state admission without scalar inverses

This theorem removes a false scalar-state requirement. Its Yang–Mills application remains conditional on the signed Gaussian window estimate (5.2) and the uniform finite-coupling value bound of §12. It supplies no marked sensitivity.

**Theorem 10.1 (P, continuous full-state shooting).** Consider a native causal evolution depending continuously on its initial bare inverse coupling x0. At step j its state may include every preceding action and coupling. Suppose it is defined whenever all previous x_i>A_native, and its coupling component has the form

\[
 x_{j+1}=x_j-d_j+r_j(\mathfrak s_j),\qquad
 |r_j(\mathfrak s_j)|\le\omega(x_j),\qquad\omega(A)\downarrow0.          \tag{10.1}
\]

The scalar d_j may depend on j but not on the history; no inverse map or state derivative is assumed. Suppose all windows obey

\[
 d_-(n-m)-B\le\sum_{m\le j<n}d_j\le d_+(n-m)+B,
 \quad d_->0.                                                         \tag{10.2}
\]

Choose A>A_native with ω(A)≤d_-/2 and take x*>A+B. For every K there exists an actual bare value whose full forward history stays above A and ends at x_K=x*. Its trajectory satisfies

\[
 x_*-B+\tfrac12d_-(K-j)\le x_j
 \le x_*+B+(d_++\omega(A))(K-j).                                      \tag{10.3}
\]

**Proof.** By the length-one windows, |d_j|≤D for a fixed D depending on d±,B. While admitted, each step changes x by at most D+ω(A). Thus all initial values exceeding A+K[D+ω(A)]+1 generate K admitted steps, and their terminal values tend to infinity as x0 tends to infinity.

Let I be the connected component containing those sufficiently large initial values of the open set of bare values whose first K iterates stay strictly above A. It is an interval (b,∞). It has a finite lower endpoint b≥A, since admission includes x0>A. As x0 decreases to b within I, every coordinate stays in a bounded interval by the step bound. The causal maps are continuous on a neighborhood of x_i≥A, since A>A_native. Recursively they extend to the limiting full history at b, and every x_i(b)≥A. If all were strictly greater than A, continuity through finitely many steps would extend I below b. Hence x_m(b)=A for some m≤K.

Sum (10.1) from m to K and use the lower window and ω(A)≤d_-/2:

\[
 x_K(b)\le A-d_-(K-m)+B+\omega(A)(K-m)\le A+B<x_*.
\]

The continuous terminal function on [b,∞) takes a value below x* at b and tends to infinity. The intermediate value theorem supplies a bare value in I with endpoint x*. This is a forward trajectory of the same full-state evolution, not a backward assembly of inconsistent states. Summing (10.1) backwards from K gives (10.3). ∎

Continuity in the chosen endpoint, uniqueness of the chosen bare value, and marked derivative bounds do **not** follow from this theorem. They are unnecessary for existence of one admitted sequence. No such additional claims are made.

**Native-domain qualification.** Theorem 10.1 assumes the causal maps exist on the whole threshold domain used in its continuation argument. For the complete native construction, its interscale comparisons, including CMP119 (2.6)–(2.9), must be checked in addition. Bounds (10.3) give the scale/radius estimates in §6 but do not, on their own, imply every prescribed native interscale inequality with its original constants. The theorem therefore applies directly to a full-state evolution defined on this threshold domain, or to the native evolution only after a proof that its additional admissibility conditions follow from (10.1)–(10.2) with suitably chosen constants. A boundary caused by failure of another native condition, rather than by x_m=A, would invalidate the shooting argument as written. This remains an explicit native application condition.

If (9.12) is certified, its program-unit remainder is bounded by a function ω(x)=C x^{-1/8}(1+log x)^6, after X_B=2N²x is used. This tends to zero and suffices in Theorem 10.1. Along (10.3) its total size is O(K^{7/8}(1+log K)^6), hence o(K), although it is not summable. If the Gaussian cumulative coefficient additionally obeys |Σ_{j<K}d_j-dK|≤B, this gives the leading law x0/K→d. It does not give the sharper O(log K) finite-coupling error from N2-F, nor the complete F-AF observable identification. The numerically signed Gaussian window (10.2), or a substitute actual full-state window estimate, is still unproved.

### 10.2 The printed interscale comparisons from full window bounds

The following deduction closes the specific CMP119 (2.6)–(2.9) check, conditionally on (10.1)–(10.2), after increasing A. The formulas are those of printed pp.255–256. It uses the full windows, not merely (10.3).

Put H_i=λx_i, λ=2N², ℓ=n-m≥1. On an admitted history, with ω(A)≤min(d_-/2,1),

\[
 H_n-B_B\le H_m\le H_n+D\ell,\qquad
 B_B=\lambda B,\quad D=\lambda(d_++B+1),\quad H_i\ge A_B=\lambda A.      \tag{10.4}
\]

Thus in native couplings g_i=H_i^{-1/2},

\[
 g_n\le(1+Dg_n^2\ell)^{1/2}g_m
 \le(1+D/A_B)^{1/2}\ell^{1/2}g_m,\quad
 g_m\le(1+B_B/A_B)^{1/2}g_n.                                          \tag{10.5}
\]

Choose A_B so the two fixed prefactors are at most 1+β0. This is (2.6) with β′=D. For each fixed positive integer p used in the construction,

\[
 (\log H_n/\log H_m)^p
 \le(1+B_B/(A_B\log A_B))^p\le1+\beta_0,                               \tag{10.6}
\]

and

\[
 (\log H_m/\log H_n)^p
 \le(1+D\ell/H_n)^{p/\log A_B}
 \le(1+Dg_n^2\ell)^{\beta_0}
 \le(1+\beta_0)\ell^{\beta_0}.                                       \tag{10.7}
\]

The first estimate uses H_n≤H_m+B_B when its ratio exceeds one. The second uses H_m≤H_n(1+Dℓ/H_n) and (1+t)^p≤exp(pt), with log A_B≥p/β0 and (1+D/A_B)^β0≤1+β0. One threshold handles the finite list of construction exponents p0,r,q0,q1. A threshold uniform over unbounded p is not claimed.

For ε_i=g_i A0(logH_i)^p0, note that H^{-1/2}(logH)^p0 decreases for logH≥2p0. If H_n≥H_m, ε_n≤ε_m; otherwise its logarithm ratio is at most one and (10.5) gives ε_n≤(1+β0)ℓ^{1/2}ε_m. In the reverse ratio, if H_m≥H_n the coupling ratio is at most one and (10.7) applies; otherwise the logarithm ratio is at most one and g_m/g_n≤1+β0. Therefore

\[
 \epsilon_m\le(1+\beta_0)(1+Dg_n^2\ell)^{\beta_0}\epsilon_n
 \le(1+\beta_0)^2\ell^{\beta_0}\epsilon_n,                              \tag{10.8}
\]

which is (2.8).

Let R_i be the least L-power above (logH_i)^r. Make the slack in (10.6) smaller than L-1. The ratio of the two unrounded quantities in the n/m direction is then less than L. Since R_n/R_m is an L-power, rounding yields R_n≤L R_m. In the opposite direction, (10.7) gives

\[
 R_m\le L(1+Dg_n^2\ell)^{\beta_0}R_n
 \le(L+1)\ell^{\beta_0}R_n,                                           \tag{10.9}
\]

after requiring L(1+D/A_B)^β0≤L+1. This is (2.9). Every choice is independent of K and volume.

The logical use is to shoot with the small-field causal construction, whose CMP109 Theorem 3 assumes the weak sequence and fixed regularity constants. The full windows then prove (10.4)–(10.9) for the resulting trajectory before applying the complete-field construction. This discharges the displayed interscale comparisons conditionally on the window hypotheses. Any additional condition on the small-field causal domain beyond that theorem must still be checked separately.

## 11. Scope of §§1–10 and the next signed estimate

The results of §§1–10 are the convention/base source (§§1–2), the precise primary formula readings (§3.1), the explicit Gaussian reserve deduction (§9.2) under its stated coordinate and integrand hypotheses, and the full-state shooting theorem (§10). The shooting implication and the Gaussian reserve lemma are proved as mathematical implications; their native input identifications are not established in §§1–10. No EP, F-admit or F-AF interface is established in §§1–10.

The next analytic problem has two parts, with no need to repeat scalar shooting. First, the three coordinate/localization/chart checks at the end of §9.3 (supplied in §12). Second, one can attack the Gaussian signed window through the bordered determinant in N2 I.3. Retain the exact gauge/coarea density and compare its hard constraint H|ker J to a reference massive background-gauge quadratic form. The required quantity is the quadratic-curvature coefficient per terminal site of the **combined difference**, not the norm of a flat covariance. A sufficient bound is

\[
 \left|\Pi_{F^2}\Bigl[
 \log h_k-\tfrac12\log\det(H_k+J_k^*S J_k)
 -\tfrac12\log\det(J_k(H_k+J_k^*S J_k)^{-1}J_k^*)
 -\mathcal G^{\rm ref}_k\Bigr]\right|\le C,                            \tag{11.1}
\]

uniform in k, after the same vacuum subtraction and per-volume normalization on every term. The reference must include its gauge determinant and have its curvature coefficient evaluated in the program convention. A bound (11.1) with reference slope 11 log L/(24π²) would provide bounded cumulative Gaussian transients, hence positive windows. A weaker comparison supplying only a positive lower window and finite upper window would already suffice for F-admit. No estimate (11.1) is proved here; the local readout estimates and flat covariance convergence in N2 do not supply its two external derivatives.

The source material used here clarifies what the finite-coupling estimate would have to use and removes the scalar-state obstruction from the abstract admission implication. It does not remove the remaining signed determinant problem, the native admissibility-domain check, or the marked work in O1/O2.

## 12. Completing the native remainder input

This section keeps the earlier candidate arguments, but replaces their outstanding square-root hypothesis by a Gaussian rectangle theorem and gives explicit native checks for the other inputs. With the generated increment identified in (12.13), it proves the scoped native incremental value modulus and fixed-depth EP. F-admit and F-AF are not inferred from them.

### 12.1 Zero-fluctuation local representatives

Separate the integrand in CMP109 (2.12) into the terms with a factor g^{-2} and the remaining bounded analytic terms. Before any localization the former are compositions of D3, G3, V3, the product of a linear fluctuation and D2, and D2 squared. Their Taylor series in the physical fluctuation q starts at order three. Here D2 and D3 denote the quadratic and degree-at-least-three portions of the solved constraint; V3 is the Taylor remainder of the Wilson action after its actual constrained Hessian has been extracted. This statement includes the current term: the quadratic part of D has already entered Δ^{(j)}, leaving D3 in (2.12).

Every localization operation used for these terms preserves order-three vanishing. The weakening procedure replaces a linear propagator by another linear propagator and replaces the nonlinear small solution by the solution of the same equation with the weakened propagators. That solution is zero at q=0 and has the same lowest Taylor order, by its defining contraction equation. Differentiation or Cauchy integration in weakening variables commutes with the first three Taylor coefficient evaluations at q=0, since the field and weakening variables are jointly analytic. Multiplication by the fixed partition functions and summation preserve the same vanishing. Thus the localized functions in (1.38) have zero constant, linear and quadratic Taylor coefficients before division by g². This also appears directly in the cubic bound (1.39).

Use the actual second-order Taylor integral of these localized functions, as in (1.40), to define Q_Y. It has Q_Y(0)=0, because the second derivative of an order-three function vanishes at zero. Substitution q=gCb-hD(gCb) does not change this conclusion: that substitution is zero at b=0 and starts linearly in b. Thus the choice of Q in §9.1 with Q_Y(0)=0 is a valid native localized representative, not an inference that every decomposition (1.42) must have that property.

The remaining analytic terms are the coordinate and Haar logarithms plus the complete inherited difference. Their total is zero at b=0. For the inherited construction this can also be seen locally: the mean-field displacement is zero at b=0 for every choice of weakening parameters, and each differentiated interpolation of the difference retains at least one displacement factor. There is a simple convention that removes any issue about a later regrouping of constant pieces. Replace every bounded localized V''_Y(b) by

\[
 \widetilde V''_Y(b)=V''_Y(b)-V''_Y(0).                                  \tag{12.1}
\]

Absolute convergence permits the subtraction to be summed, and Σ_Y V''_Y(0)=0 because the complete nonquadratic integrand is zero at b=0. Hence (12.1) preserves the actual fluctuation action exactly on its physical background family. It preserves support, analyticity and gauge invariance, and at most doubles (1.36). All new representatives vanish individually. This is a recentering of an already extracted integrand, not a new vacuum subtraction from the physical density.

Consequently radial Schwarz applies to these representatives with the constants of §9.1. The pointwise estimate (9.5) follows for the **actual complete regular inherited action** on its independent-coordinate cutoff. Its constant C_V depends on N,L,M,κ,κ1,E0 and fixed chart radii, not on j, torus volume or the particular admitted numerical coupling history. The native sum over older generations was already performed in Lemma 1 of CMP116, rather than estimated again term by term here.

### 12.2 The actual exponential-gauge covariance has a uniform bound

All spaces in this paragraph are on the current input lattice, whose bond spacing is one; the next coarse blocks have side L. Let J_* be restriction to the independent bonds, and C_* the linear solved-bond inclusion. Each solved bond is in one fixed L-block corridor. Its coefficient in the linear block constraint has an inverse bounded by a constant depending on N,L on the fixed regular chart. There are finitely many such coefficients per block. Thus C_* and J_* have uniformly bounded row and column sums and range O(L), independently of j and volume. This is the linear elimination described on CMP109 pp.267–268; no original-fine-lattice norm is substituted for this current-lattice norm.

Let D_U be the infinitesimal gauge action on current bonds, with gauge parameter zero at each next-coarse center, and put V=J_*D_U. Each row of D_U has at most two adjoint transports of norm one; each column meets at most eight bonds in four dimensions. These give uniform row and column bounds. The coarse readout is gauge covariant, so its derivative kills D_U on these centered parameters and C_*V=D_U.

The exponential gauge has one Lie-algebra row for each noncenter site, the linearization of its center-to-site path variable. At the reference gauge this path variable is identity. Gauge covariance gives KV=-I in the unweighted Lie convention, or a fixed bounded scalar/isometric conjugate after the normalized-trace precision is included. This verifies rank and excludes redundant gauge rows. Every path or contour-average defining a row has at most cL links and a fixed number depending only on L of allowed contours. Its derivatives on a fixed regular chart are bounded; composing with C_* retains finite range and uniformly bounded row and column sums. Thus K, (KV)^{-1},

\[
 R=V(KV)^{-1},\qquad P=I-RK                                             \tag{12.2}
\]

have row and column sums bounded by C_{N,L}, and range at most a fixed multiple of L. The inverse of KV is sitewise (with fixed parallel transports), so this step is stronger than finite-dimensional invertibility. The number of gauge rows is (L^4-1) dim G per next-coarse cell; the number of independent current bond coordinates is 4(L^4-1) dim G. These counts are fixed-volume ratios, not bounds that grow with RG depth.

Let C_ax be the covariance for a native axial complement of the same constrained Wilson Hessian, embedded and then restricted to the independent bond coordinates. CMP99 Theorem 3.15, (3.187), gives its exponentially decaying current-lattice kernel with constants depending only on d,L (and the fixed group normalization). Its operator norm is therefore at most K_ax. The constrained Wilson Hessian annihilates V by stationarity on the nonlinear fiber and exact gauge invariance. The decomposition into h∈ker K and Rw then gives the exact identity, already established in O1 §10,

\[
 C_{\exp}=P C_{\rm ax}P^*+RR^*.                                         \tag{12.3}
\]

If the axial complement is different from ker K, the factors P are essential. Using the row/column estimates and Schur's test,

\[
 \|C_{\exp}\|\le\|P\|^2K_{\rm ax}+\|R\|^2=:K_0<\infty.               \tag{12.4}
\]

The same finite-range convolutions preserve exponential kernel decay. All bounds apply to real regular external fields in a fixed smaller chart and are uniform in j,volume and incoming history. The latter does not enter the explicit Gaussian precision: the inherited action is retained in V_{j,g}. The normalization and the exponential gauge are kept, so (12.3) is not an identification of different gauge prescriptions.

### 12.3 No square-root row bound is needed

Use the following primary import: Šidák, *Rectangular Confidence Regions for the Means of Multivariate Normal Distributions*, JASA 62 (1967), Corollary 1, printed p.628, equation (4). For any centered Gaussian vector, with arbitrary correlations including singular ones,

\[
 \Pr\{|b_i|\le R_i\ \forall i\}\ge\prod_i\Pr\{|b_i|\le R_i\}.           \tag{12.5}
\]

The singular case is obtained by Gaussian approximation in the original proof. Primary text: [Šidák, Corollary 1](https://www.math.toronto.edu/mccann/assignments/477/Sidak67.pdf).

With (12.4), every coordinate variance is at most K0. For R large, (12.5) and the one-dimensional Gaussian tail bound imply

\[
 \Pr\{\|b\|_\infty\le R\}\ge(1-2e^{-R^2/(2K_0)})^n,
 \quad n^{-1}\log\Pr\{\|b\|_\infty\le R\}\ge-4e^{-R^2/(2K_0)}.         \tag{12.6}
\]

The fixed component/Lie-norm conversion changes K0 by a fixed factor only. This replaces the Gaussian-factor argument in §9.2. The upper bound (9.8) already needed only the operator norm (12.4). Therefore no covariance square-root estimate, factorization with latent variables, or latent-dimension bound remains in the reserve proof.

Choose ε1 so C_V ε1<1/(8K0), then choose g≤g0 with the exact product cutoff containing ||b||∞≤g^{-1/6}. Equations (9.5)–(9.8), now with (12.6) for the lower probability, give

\[
 n^{-1}|\log I_{j,g}(U)|\le C g^{1/2}.                                  \tag{12.7}
\]

This is an actual real regular fluctuation integral and its actual inherited action. Constants are uniform in all the indices stated after (12.4). The estimate is volume-uniform before any limit; no cross-volume copying argument from §4 is needed.

### 12.4 Fixed external chart and the polarization tail

The required minimizer import is precise: CMP102, *The variational problem and background fields*, printed pp.305–309, (172)–(175), (190), Proposition 9. It gives an analytic extension in V′ with |V′-1|<C1 ε_v, where ε_v is sufficiently small independently of depth and volume. The constant B5 in (173) is absolute. Proposition 9 bounds the normalized fine potential and its derivatives in the regular norms (19)–(21), and gives the functional derivative bounds (190). Here ε_v is distinguished from the fluctuation cutoff ε1.

For the all-small determining set, take η=L^{-j} and current terminal scale one. In (190) the only determining layer is the terminal layer: both factors L^iη and L^{i′}η are one. Thus its first-derivative estimate, in the normalized regular field norm on a local current-scale region X, reads

\[
 \|D_{B_y}\mathcal U_j(0)\|_{\mathrm{reg},X}
 \le C_H e^{-c_H\operatorname{dist}(X,y)}.                               \tag{12.8}
\]

The map \(\mathcal U_j\) here includes the fine group field and its current, in the local gauges used to define the CMP109 analytic chart. The regular norm is the maximum of the scale-normalized potential, its first derivative, the required Hölder seminorm and current; a fine link is exp(iηA), so it is not an unweighted supremum of all original fine coordinates. The constants in (190), and hence C_H,c_H, are independent of j. Gauge changes back to the prescribed representative are analytic local changes on fixed block neighborhoods; the local action is gauge invariant, so these gauges may be used separately on its supports.

Choose a fixed complex coarse-field radius ρ>0 small enough that the regular bounds of Proposition 9 place its image strictly inside the fixed CMP109 α0,α1 charts, including their smaller local-synthetic-background conditions. This is possible with a depth-independent choice because the constants just listed are uniform. A finite sum of real sine/cosine waves with amplitudes of total magnitude below ρ has coarse sup norm below ρ independent of wavevector and volume. Hence every per-site residual action on these amplitudes is holomorphic in a fixed smaller polydisc and uniformly bounded by the native activity norm.

For the tail, let F_X be either the combined generated local activity or its Gaussian part. At identity its first derivative in the (U,J) variables is zero: global color invariance would otherwise give an invariant linear functional on the semisimple Lie algebra at some coordinate. A scalar such functional is zero. Thus the second derivative after minimizer substitution is D²F_X[D\mathcal U_j,D\mathcal U_j]; the term with D²\mathcal U_j is absent. Cauchy on the fixed chart and (12.8) imply

\[
 |D_{B_0}D_{B_z}F_X(\mathcal U_j(0))|
 \le C e^{-\kappa' d(X)}
 e^{-c_H\operatorname{dist}(X,0)}e^{-c_H\operatorname{dist}(X,z)}.        \tag{12.9}
\]

Any fixed support-polynomial from the local norm is absorbed by decreasing κ′. To sum X, reserve half the exponent. If diam X≥|z|/3, its size decay supplies exponential decay in |z|. Otherwise one of the two distances is at least |z|/3. The remaining exponent is summable over supports and their locations by the anchored native polymer majorant. Consequently

\[
 |P_{j+1}(g;z)|+|P^G_{j+1}(z)|\le C_P e^{-c_P|z|},                     \tag{12.10}
\]

with C_P,c_P independent of j,g,volume and the admitted history. This proves the missing depth-uniform tail using the fixed field charts and the native minimizer derivative estimate, not analyticity in a coupling or in an observable source.

### 12.5 Native value modulus and EP scope

Here P is exactly the scalar color-diagonal kernel Π of CMP109 (1.20)–(1.22), with the derivative taken in the fixed coarse coordinates V=exp(iB). Its generating function is the **new generated increment**, in the convention (1.6) combining the Gaussian normalizer with the non-Gaussian term (2.13):

\[
 \mathcal E_{j+1}(g;B)=\log Z^{(j)}(\mathcal U_{j+1}(B))
       +\log I_{j,g}(\mathcal U_{j+1}(B)).                              \tag{12.13}
\]

Field-independent normalizations can be subtracted on either side. The full carried action evaluated at the new minimizer has already been subtracted in the definition preceding (1.7), printed p.261. Its change under the fluctuation remains inside I through the curly bracket of (2.12); it was estimated by the complete inherited-difference lemma in §12.1. Thus (12.7) does not estimate or discard the sum of the carried actions themselves. Define P^G by the Hessian of the first term of (12.13), on precisely the same minimizer family. Then P−P^G is the Hessian of log I, and the native scalar increment is β_{j+1}(g)=Σ_z P_{j+1,μν}(g;z)z_μz_ν for μ≠ν. The reference decrement used in §10 is d_j=β^G_{j+1}/(2N²), with this same projector and Gaussian normalization. This identification follows the printed (1.6), (1.20) and (1.22), not the name “polarization.”

Combine (12.7) with the fixed fourth field-derivative bound just established. The symmetric real finite-difference argument in §9.3 gives Fourier Hessian error Cg^{1/4}; the uniform tail (12.10), Fourier inversion, and the spatial cutoff R0=O(log(1/g)) give

\[
 \sum_z(1+|z|^2)|P_{j+1}(g;z)-P^G_{j+1}(z)|
 \le C g^{1/4}(1+|\log g|)^6.                                          \tag{12.11}
\]

All constants depend only on the fixed group, L, fixed construction constants and the chosen strict field-chart margins. They do not depend on j, volume, or the particular actual admitted incoming history. The exponent six comes from the four-dimensional count of sites in a radius-R0 ball and the quadratic spatial weight; it is not an anomalous-dimension claim. The residual action is normalized at external identity, so field-independent constants do not enter the Hessian.

The infinite-volume polarization is taken at fixed g as in CMP109 (1.22); (12.11) is inherited from volume-uniform finite-volume estimates and their uniform tails. Then g tends to zero. At any fixed physical depth, bounded scalar increments imply that every earlier coupling also tends to zero as the bare coupling tends to zero. Applying (12.11) successively identifies all incoming weak endpoints. Thus this proof removes EP for the fixed physical cutoff and readout family used here. It neither concerns a g-dependent alternative cutoff nor transfers the endpoint to a different scalar projection.

In program units the resulting value error is

\[
 |r_j(\mathfrak s_j)|\le C x_j^{-1/8}(1+\log x_j)^6,                    \tag{12.12}
\]

with λ=2N² absorbed into C. No derivative with respect to the bare coupling, earlier couplings, or a scalar source has been taken or bounded. The native signed Gaussian window required by Theorem 10.1 remains a separate unproved statement. In particular (12.12) alone does not construct a fixed-terminal trajectory.

## 13. Coarse Schur determinant: a bounded contribution, with the fine comparison left intact

This section isolates a genuine part of (11.1). It uses the same terminal coarse coordinates and regular classical minimizer as §12. It does not replace the hard density by a new gauge prescription, and it leaves its coordinate/gauge factor with the fine determinant.

This section proves the exact Schur identity, the native fixed-chart local derivative argument, and the connected trace-kernel estimate below. The result is only the uniformly bounded second spatial moment of the coarse Schur contribution.

### 13.1 Exact Schur identity in the actual constraint coordinates

At fixed depth k and finite volume choose a fixed smooth fine gauge slice for gauge transformations that are identity at terminal centers. Let a denote its coordinates, and let q(a) be the logarithm of the **composite** readout in the prescribed coarse chart. Thus the constraint is q(a)=B, not an affine approximation to the group-valued constraint. Write a_k(B) for the constrained minimizer and

\[
 S_k(B)=A(a_k(B)),\quad J=Dq(a_k(B)),\quad
 DA(a_k(B))=J^*\mu(B),\quad
 H=D^2A(a_k(B))-\sum_\gamma\mu_\gamma(B)D^2q_\gamma(a_k(B)).             \tag{13.1}
\]

The starred maps here are transposes in these fixed real coordinates, extended bilinearly when B is complex. H is the stationary Lagrangian Hessian. In particular it includes the constraint-current term. Set M=Da_k(B) and G_k=D²S_k(B). Differentiating the constraint and stationarity gives

\[
 JM=I,\qquad DS_k=\mu,\qquad HM=J^*G_k.                               \tag{13.2}
\]

Consequently, for D_s=H+sJ*J,

\[
 D_s M=J^*(sI+G_k),\qquad
 J D_s^{-1}J^*=(sI+G_k)^{-1}.                                         \tag{13.3}
\]

Invertibility is not assumed merely from the existence of J. Decompose an arbitrary fine tangent as t+Mb, with Jt=0. Equation (13.2) makes the H cross term vanish, and its quadratic form is

\[
 (t+Mb)^*D_s(t+Mb)=t^*Ht+b^*(G_k+sI)b.                                \tag{13.4}
\]

The regular native constrained Hessian is positive on ker J. Once sI+G_k is positive, (13.4) proves invertibility. No depth-uniform lower eigenvalue for the fine slice is needed for this finite-dimensional identity. The right side acts on the actual coarse constraint coordinates, including their longitudinal directions if those coordinates have not been quotiented. One must not replace it by a transverse Hessian without the corresponding change of measure.

### 13.2 Uniform local derivative bounds for the classical coarse action

Here the CMP102 Proposition 9 and (190) import is the one used in §12.4. Let η=L^{-k}. Partition the fine plaquettes into terminal unit cells Δ, and write

\[
 S_k(B)=\sum_\Delta s_{k,\Delta}(B),\qquad
 s_{k,\Delta}(B)=\sum_{p\text{ assigned to }\Delta}
       [1-\operatorname{tr}_{\rm sym}U_k(B)(\partial p)],               \tag{13.5}
\]

where tr_sym U=(tr U+tr U^{-1})/2 is the analytic continuation of Re tr U. On the fixed smaller complex B chart, the normalized regular bounds give U_k(∂p)−1=O(η²). The linear term of tr_sym at identity is zero, so each summand in (13.5) is O(η⁴). There are at most Cη^{-4} plaquettes assigned to a unit cell. Therefore |s_{k,Δ}|≤C uniformly in k, Δ and volume.

The regular norm in (190) controls the variation of the plaquette curvature as well as the potential. At a coarse bond/component y it gives

\[
 |D_{B_y}U_k(B)(\partial p)|\le C\eta^2
            e^{-c\operatorname{dist}(p,y)}.
\]

Gauge-dependent variations of the representative cancel in the plaquette trace. Multiplication by the O(η²) first derivative of tr_sym and summation over the Cη^{-4} fine plaquettes yields

\[
 |D_{B_y}s_{k,\Delta}(B)|\le C e^{-c\operatorname{dist}(\Delta,y)}.    \tag{13.6}
\]

This bound holds on a strictly larger complex chart than the one subsequently used. Cauchy differentiation in any further at most three coarse components therefore preserves the right side up to fixed constants. Derivatives commute; applying the bound with each of the differentiated components in the distinguished first position gives, for 1≤m≤4,

\[
 |D_{B_{y_1}}\cdots D_{B_{y_m}}s_{k,\Delta}(B)|
 \le C_m\exp[-c_m\max_i\operatorname{dist}(\Delta,y_i)].              \tag{13.7}
\]

This argument requires neither a global affine-flux family on the torus nor differentiation of a k-dependent analyticity radius. All Cauchy radii are the fixed strict chart margins of §12.4. Summing Δ and reserving part of the exponential gives

\[
 |D_{y_1}\cdots D_{y_m}S_k(B)|
 \le C_m' e^{-a_m\operatorname{diam}\{y_1,\ldots,y_m\}},\quad
 2\le m\le4.                                                        \tag{13.8}
\]

For example choose one y_i as anchor, split the maximum distance into a fixed fraction of the diameter and the remaining distance from Δ to the anchor, and sum the latter in four dimensions. The harmless polynomial from this summation is absorbed by decreasing a_m. These statements use periodic distances on finite tori and remain uniform in their size.

In particular, for some a>0,

\[
 \sup_u\sum_v e^{a|u-v|}|(G_k(B))_{uv}|\le C_G,                       \tag{13.9}
\]

with the corresponding column bound. The same tensor bounds give exponentially localized first and second external-field derivatives of G_k. Choose a single s>2C_G, increasing it if necessary for the finite color/direction multiplicities. This choice is independent of depth and volume. It gives both the positivity required by (13.4) on real fields and a convergent weighted Neumann series on the complex chart.

### 13.3 The Schur polarization has a uniform second spatial moment

Define the actual coarse Schur contribution to the hard logarithmic prefactor by

\[
 C_k(B)=-\tfrac12\log\det[J D_s^{-1}J^*]
       =\tfrac12\log\det(sI+G_k(B)).                                 \tag{13.10}
\]

Vacuum constants are immaterial. Let R_k=(sI+G_k)^{-1}. Its weighted kernel norm is bounded by (s−C_G)^{-1}, by the Neumann series in the norm (13.9). For two coarse components b,c, differentiation of the finite-dimensional determinant gives exactly

\[
 D_bD_c C_k=\tfrac12\operatorname{Tr}
 [R_k D_bD_cG_k-R_k(D_bG_k)R_k(D_cG_k)].                              \tag{13.11}
\]

Every factor on the right has the locality bound just proved: the inverse has two-index exponential decay; D_bG and D_bD_cG have the three- and four-index diameter bounds (13.8). In the first trace, the diameter contains b,c and both contracted indices. In the second, the two inverse kernels connect the two three-index groups. Their combined connected graph spans b and c. Reserve a fixed fraction of each decay exponent to obtain e^{-a'|b-c|}; the remaining exponents sum the internal indices. This proves

\[
 |D_bD_c C_k(0)|\le C_C e^{-a'|b-c|},\qquad
 \sum_z(1+|z|^2)|D_{B_0}D_{B_z}C_k(0)|\le C_C'.                     \tag{13.12}
\]

The constants are independent of k and volume. Hence the native off-diagonal second-moment projection of the coarse Schur term is bounded uniformly in k. This is a local-kernel proof of its curvature coefficient; no finite-volume quantized-flux differentiation is used. The term alone need not be gauge invariant under nonlinear coarse coordinate changes. Its bounded projection is taken in the fixed actual chart, and the other terms retain their matching coordinate density.

### 13.4 Exact remaining signed estimate

With the fixed scalar penalty s above, the full hard Gaussian log prefactor remains

\[
 \mathcal L_k(B)=\log h_k(B)-\tfrac12\log\det D_s(B)+C_k(B).           \tag{13.13}
\]

Equation (13.12) removes the coarse Schur term from the list of quantities that can grow linearly in k. It does not bound the other two terms separately or their combination. A sufficient remaining form of (11.1) is

\[
 \left|\Pi_{F^2}\{\log h_k-\tfrac12\log\det D_s
                         -\mathcal G_k^{\rm ref}\}\right|\le C,       \tag{13.14}
\]

where the reference includes its actual gauge determinant and has a proved positive cumulative slope in program units. No such comparison or positive slope is established here. Uniform locality of G_k does not bound a trace over the increasing number of fine degrees of freedom in D_s.

### 13.5 A gauge simplification that does not close (13.14)

One can exactly change the fine Gaussian gauge while keeping the correct density. At fixed background let V embed infinitesimal gauge parameters that vanish at terminal centers, so HV=0 and JV=0. Let Q be any complementary inclusion. For a linear gauge L with LV invertible, write a=Qu+Vt. The integral over t in

\[
 |\det LV|\int da\,\delta(Ja)\exp[-\tfrac12a^*Ha-\tfrac12|La|^2]
\]

is independent of L: the change w=LQu+LVt cancels |det LV|. The remaining density is the common coordinate Jacobian |det[Q,V]| times the quotient Gaussian integral. This proves gauge independence of the **combined** normalized prefactor, not of either determinant alone. If Q or V varies with background, its coordinate Jacobian must remain in h_k.

A tempting further step is invalid: the ghost operator for a background divergence gauge with parameters pinned only at terminal centers is not uniformly massive as η→0. At the flat background it is the η-lattice Laplacian on scalar parameters vanishing at those centers. Take the trial function equal to one at all other sites and zero at every terminal center. In the η⁴-weighted norm its squared norm is of order the terminal volume. Only a fixed number of bonds adjacent to each center contributes to its Dirichlet energy, each with weight η². Therefore its Rayleigh quotient is at most Cη². Its smallest eigenvalue tends to zero. The same test applies componentwise to the adjoint Lie algebra.

Thus the one-step bounded gauge bridge of §12.2, whose blocks have fixed side L in current units, cannot be reused as a cumulative depth-uniform massive ghost bound for blocks of side L^k. Any background-gauge reference proof of (13.14) must keep this low-mode determinant and its coarea compensation, or establish a separate comparison that handles them together. The positive-window problem remains at that combined signed fine-scale estimate.

## 14. Summary of scope

The new analytic results are (12.7), (12.11)–(12.13), and (13.12). They use the native fixed physical cutoff, the prescribed composite readout, the actual combined new increment and its printed polarization projector. The real finite-coupling estimate retains the complete inherited fluctuation difference. It is uniform over actual admitted histories, and it does not differentiate those histories.

| Interface | Final scope |
|---|---|
| B | Checked native import (2.1), conditional on an admitted actual trajectory and native geometry |
| Native value modulus | Proved: per-site residual logarithm O(g^{1/2}); weighted polarization difference O(g^{1/4}(1+|log g|)^6) |
| Fixed-depth EP | Proved for the same fixed-cutoff/readout/projector family; no cutoff or scheme change |
| Coarse Schur determinant | Proved: projected second spatial moment bounded uniformly in depth, (13.12) |
| F-admit | Open: positive signed Gaussian windows (5.2), reduced to the combined fine determinant and gauge/coordinate comparison (13.14), are not proved |
| F-AF | Open: no native aggregate universal Gaussian slope has been established |
| Marked history/source derivatives | Not supplied by these value estimates; a separate problem (O1) |
| Full-law patch reserve | Not supplied by the small-field pressure estimate; a separate problem (O2) |

The remaining finite-coupling error is already sublinear along any trajectory admitted by §10. Indeed (12.12) and its linear windows give, with constants independent of K,

\[
 \sum_{j<K}|r_j(\mathfrak s_j)|
 \le C(1+K)^{7/8}(1+\log(1+K))^6=o(K).                              \tag{14.1}
\]

This follows by comparing the sum with the integral of (A+ct)^{-1/8}(1+log(A_++c_+t))^6. Thus a bound D_k^G=dk+O(1), with the correct native d, would both provide the signed windows and, through the conditional shooting theorem, yield x_0=dK+o(K) at fixed terminal x_K. The value-modulus part of this implication is no longer an additional unknown. Neither its Gaussian slope premise nor the existence conclusion is asserted here. Section 10.2 verifies the displayed CMP119 interscale comparisons once those windows are available; application still uses the native small-field causal domain and all fixed construction hypotheses.

Primary locations supporting the new proof are CMP109 pp.261,263–264,266–268, (1.6)–(1.22),(2.9)–(2.15); CMP116 pp.9–11, Lemmas 1–2 and (1.33)–(1.43); CMP99 p.432, Theorem 3.15/(3.187); CMP102 pp.305–309, (172)–(175),(190), Proposition 9; and Šidák Corollary 1, p.628, (4). The exact remaining signed expression is (13.14), with the counterexample to a uniform cumulative ghost mass immediately below it. No unconditional Yang–Mills existence statement follows from this source.
