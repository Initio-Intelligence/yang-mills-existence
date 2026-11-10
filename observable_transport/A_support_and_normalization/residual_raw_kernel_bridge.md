# Residual raw-kernel bridge: a Schur estimate and the remaining variational input

## 1. Conclusion and exact scope

The proposed inference from LFR II (1.59)–(1.60), a local step lift, and the PR/GM Gaussian constructions to BC.2 is **not established**. There is a specific source-coordinate obstruction to that inference: the positive native comparison in LFR II (1.73)–(1.75) freezes part of the old operation, whereas a change of raw retained variables can change the background-dependent Schur precisions in that specified part. A native substitution `(U,J)=(1,0)` is consequently not, by itself, a construction of a reference law depending only on the bounded current core.

The matrix difficulty can be separated cleanly from this nonlinear pullback. Theorem RK.1 below proves a uniform comparison of Schur precisions and their complete Gaussian densities when the primitive precisions agree, or are quantitatively close, on a buffer. Its loss is the actual old rank plus old quadratic size, and its small factor is exponential in the buffer measured in that old scale. Such a factor can dominate the arbitrarily large pre-birth rank **if the actual composed raw backgrounds supply it**. One precise sufficient pointwise route is (RK.12)–(RK.14). That old-scale buffer estimate has not been proved for the actual composed backgrounds.

BC.2 is a sufficient theorem, not a necessary condition for M-04. Arbitrary old rank times a small per-mode precision variation can prevent an old-state L∞ logarithmic-density estimate even when normalized Gaussian expectations remain controlled. Section 7 gives a separate exact normalized route through relative Hilbert–Schmidt perturbations and centered Gaussian scores. Neither route replaces the nonlinear raw pullback by a formal native substitution.

This is a source-free kernel issue. It is distinct from the incoming marked moment, the microscopic-to-current scaling dictionary, and discrete core-label transport. Solving the estimate in this note would not, on its own, prove those marked statements.

## 2. What the source does and does not localize

### 2.1 The surviving old Gaussian is explicit

CMP119, printed p.258, (2.21), contains the ordinary old fluctuation factor with precision

\[
 S_j
 =K_j-K_jP_{\Lambda_{j+1}}
       (P_{\Lambda_{j+1}}K_jP_{\Lambda_{j+1}})^{-1}
       P_{\Lambda_{j+1}}K_j,
 \qquad K_j=C_j^*\Delta^{(j)}C_j,
 \tag{RK.1}
\]

restricted to the surviving fluctuation coordinates. This is the Schur form written in the source as
`C*Δ^(j)C − C*Δ^(j)C C^(j)(Λ_{j+1}) C*Δ^(j)C`.
Only entries coupling variables in the same old large-field component are retained in that operation; the other entries are assigned to boundary terms. This is a decomposition of one complete quadratic form, not permission to omit the boundary entries.

At the first step, the same issue is visible without inductive notation: (1.26), printed p.253, explicitly states that the conditional expressions depend on `U₁`, and (1.29), p.254, retains their Schur precision. The preceding changes (1.22)–(1.25) localize the **hard characteristic functions** in the raw new field. They do not state that the Schur precision has become a function only of those raw links.

The support assertion in CMP119 (2.19) is used legitimately to locate the integrated old coordinates. It cannot be silently strengthened into a raw-locality theorem for every coefficient of their density. LFR I p.194 explicitly leaves the inner `T_h` integral unchanged during the prepared coordinate transformation.

### 2.2 Native analyticity remains a genuine result

LFR II pp.379–380 says that, in its chosen independent native continuation, only the new `B` quadratic form and the resummed self interaction `V(X̃)` vary with `(U,J)`. The small relative exponent then proves the normalized total-variation estimate (1.75), independently of the tiny positive mass of the old operation. RT.19–RT.29 use precisely that statement.

It follows that evaluation at `(1,0)`, when taken in that native definition, is a positive reference on the same fixed native support. It does **not** follow that all coefficient values specified in `T_h` are independent of exterior raw retained data. No later literal identity moving every such dependence into `V(X̃)` is available in the source. The source-map analysis reaches the same qualification.

Thus, if a local positive reference is introduced on the padded old support, its Radon–Nikodym exponent must include the ratio of all the old factors (RK.1), their actual normalization terms, and the full cross action. Omitting them would change the posterior.

### 2.3 The useful pre-grouped estimates

LFR II pp.372–373, (1.59)–(1.60), subtract the same vertex at zero `B` and localize the resulting difference. Every nonzero domain meets the prepared core, and the text states the full native `d_k` bound before the later grouping. The construction retains its compensating gauges.

The subsequent construction, (1.61)–(1.65), starts with `Y₁` containing the **whole** relevant old component. Its key regularity statement (1.65) is proved on that geometry. Finally (1.67)–(1.69) use a distance with the old components contracted. These are substantial analytic bounds, but they do not identify an absolute raw-retained carrier expansion with bounded core. In particular, (1.65) must not simply be reused after replacing `Y₁` by an arbitrary small connected carrier that cuts through the old component.

## 3. A complete matrix estimate for the old Gaussian factors

Here all matrices act on actual independent coordinates. A constrained covariance is first represented on its nondegenerate coordinate space; no determinant on a redundant gauge space is used.

Let `I` be a set of surviving old coordinates, let `J` denote the coordinates integrated out, and let `P_I` and `P_J` be the corresponding projections. On the whole free-coordinate space suppose

\[
 mI\le K,\widehat K\le MI,
 \qquad m>0,
 \tag{RK.2}
\]

with uniform exponential entry-row and entry-column bounds at an old-scale distance `d`. For example, a fixed-range precision with a uniform row bound satisfies this condition. The resolvents then obey the usual weighted operator bound: for a sufficiently small fixed `\gamma>0` and every 1-Lipschitz real function `f`,

\[
 \|e^{\gamma f}K^{-1}e^{-\gamma f}\|
 +\|e^{\gamma f}\widehat K^{-1}e^{-\gamma f}\|
 \le C(m,M).
 \tag{RK.3}
\]

One obtains (RK.3) directly by conjugating the precision. The difference from the unconjugated matrix has norm bounded by
`sup_i Σ_j |K_ij|(exp(γ d(i,j))−1)` and the analogous column sum. Choose γ so that this is at most `m/2`, then invert by a Neumann series. The same proof applies to principal restrictions. There is no dimension factor in this step.

Take the buffer `D=I^{+r}`. Assume that the two precisions have the same coordinate geometry there and that

\[
 E:=K-\widehat K=E_{\rm near}+E_{\rm far},\qquad
 \|E_{\rm near}\|\le\delta,
 \qquad P_D E_{\rm far}P_D=0,
 \qquad \|E_{\rm far}\|\le C_E.
 \tag{RK.4}
\]

This formulation includes an arbitrary change outside the buffer, and a small change of primitive background coefficients inside it. If coordinates differ outside `D`, embed the two systems in a common space with independent positive mass on the extra coordinates; retain the same coordinates on `D`.

### Theorem RK.1 — buffered Schur and Gaussian comparison

Let

\[
 C_I=P_IK^{-1}P_I,\quad \widehat C_I=P_I\widehat K^{-1}P_I,
 \qquad S_I=C_I^{-1},\quad\widehat S_I=\widehat C_I^{-1}.
 \tag{RK.5}
\]

These are the exact marginal covariances and Schur precisions. Then

\[
 \|S_I-\widehat S_I\|
 \le C\,[\delta+e^{-\gamma r}],
 \qquad mI\le S_I,\widehat S_I\le MI.
 \tag{RK.6}
\]

For the corresponding normalized real Gaussian densities on `I`,

\[
 \left|\log\frac{d\mu_{S_I}}{d\mu_{\widehat S_I}}(a)\right|
 \le C\,[\dim I+\|a\|^2]
                  [\delta+e^{-\gamma r}].
 \tag{RK.7}
\]

**Proof.** The resolvent identity gives

\[
 C_I-\widehat C_I
 =-P_IK^{-1}E\widehat K^{-1}P_I.
\]

The near term is bounded by `m⁻²δ`. Write the far term as
`P_{D^c}E_far + P_D E_far P_{D^c}`. Each summand has a resolvent joining `I` to `D^c`. Use (RK.3) with `f(x)=dist(x,I)` to bound that factor by `C exp(−γr)`; the other resolvent has norm at most `m⁻¹`. This yields the same bound for the covariance difference. Compression of `(RK.2)⁻¹` gives
`M⁻¹ I≤C_I,Ĉ_I≤m⁻¹ I`, so multiplication by their inverses proves (RK.6).

For (RK.7), the exact log density ratio is

\[
 \frac12\log\det S_I-\frac12\log\det\widehat S_I
       -\frac12\langle a,(S_I-\widehat S_I)a\rangle.
 \tag{RK.8}
\]

Interpolate linearly between the two positive precisions. Its lower bound remains `m`, so integrating `Tr[S_t⁻¹(S_I−Ŝ_I)]` bounds the determinant difference by `m⁻¹(dim I)‖S_I−Ŝ_I‖`. The quadratic term has the claimed bound. This proves the result. ∎

If the source factor is an **unnormalized** Gaussian exponential, use only the quadratic term of (RK.8). Its determinant, Haar-coordinate constant, or vacuum term must be included where the exact source algebra places it. Adding a second determinant or a second `g^{dim I}` factor is incorrect. The estimate permits the actual determinant ratio when it is present, but does not manufacture it.

### Why old rank is not an intrinsic obstacle to a buffered comparison

Suppose an actual primitive localization gives (RK.4) for the `j`th old precision with

\[
 r_j\ge c\rho L^{k-j},\qquad
 \delta_j\le C e^{-c\rho L^{k-j}},
 \tag{RK.9}
\]

where `\rho>0` is one fixed current-scale collar outside the prepared core. Let `n=k−j≥N`. The number of `j`-scale coordinates in a bounded current region is at most `C L^{4n}`. If their actual support obeys `|A_j|≤P_j`, (RK.7) bounds the sum of their log-density changes by

\[
 C\sum_{n\ge N} L^{4n}(1+P_{k-n}^2)
                         e^{-c\rho L^n}.
 \tag{RK.10}
\]

This formula is the safe statement without an additional coupling comparison. Whenever the actual old-chart envelope has at most a fixed exponential in age times a polynomial coupling loss, the sum is bounded by

\[
 C\,g_k^{-b}(1+|\log g_k|)^b e^{-c'\rho L^N}.
 \tag{RK.11}
\]

The standard compact logarithmic chart gives a crude `P_j≤C/g_j`; the inherited running-coupling comparison makes that an admissible envelope here. Much smaller literal cutoff envelopes can be retained instead. The point is that the buffer factor is exponential in `L^n`, so an arbitrary pre-birth rank does not force an arbitrary normalization loss.

Since `|Y|≤C R_k^4` and the quiet horizon is a positive power of `log(g_k⁻²)`, the factor in (RK.11) can also pay `exp[κ C R_k^4]` for every fixed κ once the source hierarchy is fixed and coupling is sufficiently small. This is a conditional quantitative benefit, not a proof of (RK.9). In the actual composed reconstruction a remote current perturbation may first propagate through a current-scale minimum before it enters an old precision. One cannot then insert `L^{k−j}` into its decay merely by measuring geometric distance on an old lattice. The retained raw collars at consecutive old scales might instead provide a product of attenuation factors, but that coefficient-level nesting also needs proof. The source-map analysis specifically identified this distinction.

## 4. The sharp remaining target

Let `γ` be any actual old internal descriptor admitted in the fixed prepared class, and let `u` be any old state in its literal hard support. No moment averaging over `u` is allowed in the following target. For every surviving `j≤h−1`, let `K_{j,γ}(v,u)` be the actual primitive precision whose Schur form appears in (RK.1). Its arguments include the actual variational background, the free-coordinate embedding, and the constraint-curvature term. Let `D₀` be the fixed current enlargement of the prepared core supplied by CG.1.

One sufficient construction within the pointwise BC route is a **positive local precision family**

\[
 K^{\rm core}_{j,\gamma}(v_{D_0},u)
 \quad\hbox{with}\quad
 mI\le K^{\rm core}_{j,\gamma}\le MI,
 \tag{RK.12}
\]

on a common padded coordinate space, with the same actual old chart and hard support. It must be defined from local raw data, not from the values of a global minimizer restricted to `D₀`. On the old-scale buffer of width `cL^{k−j}` it should satisfy the near comparison in (RK.9).

For a full physical-carrier conclusion, the corresponding complete precision/Schur comparison must have deterministic tagged majorants. One suitable exact target is

\[
 S_{j,\gamma}(v,u)-S^{\rm core}_{j,\gamma}(v_{D_0},u)
     =\sum_X \Delta S_{j,\gamma,X}(v_X,u),
 \tag{RK.13}
\]

with real symmetric tags, connected actual raw footprints `X` joining the core, and

\[
 \sup_{\gamma}\sum_{j\le h-1}\sum_X
 e^{\kappa(|X|+t(X))}
 \sup_{v,u}
 \Big\{\dim I_{j,\gamma}
       +\|A_{j,\gamma}(u)\|^2\Big\}
 \|\Delta S_{j,\gamma,X}(v_X,u)\|
 \le C g_k^{-b}(1+|\log g_k|)^b e^{-cL^N}.
 \tag{RK.14}
\]

For determinant factors, use the **same** localized precision family and its logarithmic determinant expansion; (RK.8) identifies the required rank cost. The sum in (RK.14) is outside the suprema over raw retained fields and old states. A bound on a summed Schur difference after cancellation does not imply it. The actual coarea and constraint-map changes must either be unchanged in these coordinates or have their own terms generated by the same map; they cannot disappear from the density ratio.

This target is primitive and unmarked. It mentions no incoming scalar, marked numerator, or normalized output. It is also sharper than demanding a uniform microscopic rank bound, which is false. The quantitative rank payment is explicit. It is deliberately a sufficient target: if the actual old-state supremum fails, one should use normalized transport or a weaker relative-kernel norm, rather than infer failure of M-04.

The immediate old Gaussian obstruction would be removed by (RK.12)–(RK.14). The still-new prepared `B` precision and the unmarked `E/B/R` and cross terms must then be pulled through the same source-coordinate map, before whole-component grouping, using the native budgets already specified by CMP119 (2.27), (2.31), (2.42) and LFR II (1.59)–(1.60). The map must preserve the critical cancellation and the analyticity domain of (1.65) on its complex decoupling discs. Those requirements are on the actual variational and constraint map, not on the unknown marked output.

## 5. Why the step lift does not supply that map

The symbol in LFR I p.192, (1.74), is `Q_k^{s*}`. CMP119 p.257, immediately after (2.16), defines it by (1.3) with `k`-blocks replacing `1`-blocks. It is the **step lift**: internal fine links are identity and links crossing a coarse face carry the corresponding coarse link. The superscript does not turn it into a smoothing right inverse.

This has a direct Abelian test. Embed a fixed one-dimensional torus in the gauge group and choose coarse links whose one coarse plaquette has holonomy `exp(iθT)`. A fine plaquette at the intersection of its two block faces has exactly this same holonomy under the step lift. If the fine mesh is `η=L⁻ᵏ` in current units, then

\[
 \eta^{-2}\|Q_k^{s*}V(\partial p)-1\|
        \asymp L^{2k}|\theta|.
 \tag{RK.15}
\]

The native current-regularity class requires a bound of order `|θ|`, uniformly in `k`, after that normalization. Thus the literal step lift fails it by `L^{2k}`. A gauge transformation cannot fix (RK.15), since the plaquette norm is gauge invariant.

CMP98 Proposition 1 and its later analytic propositions prove control of **forward averages** of an already regular fine field. They do not assert a uniformly regular local inverse. CMP102 p.280 makes the same distinction in its construction: at the first step it can start from the elementary lift because `L` is fixed; at general `k` it starts from an already constructed `(k−1)`-step minimal configuration. That starting field is not shown there to have an absolute raw-retained carrier expansion.

The smoothing in LFR I (1.74) is supplied by the outer minimum

\[
 U\bigl(\mathbb B_k(Y),M'(Q_k^{s*}V)\bigr),
\]

not by `Q_k^{s*}` alone. The source proves useful local minima and exponential response estimates for this operation. A telescope over larger and larger balls, however, produces supports of volume `r⁴` with only a distance error `exp(−cr)`. That does not give a sum weighted by `exp(κr⁴)`. This elementary mismatch is why numerical locality or first-derivative decay cannot be substituted for an absolute connected-carrier construction.

## 6. The precise next variational lemma

### Local regular patches already supplied by the source

There is a useful sharper distinction here. A regular prolongation on one buffered current cube is available from the existing local minimum; a **common decoupling family assembled from those patches** has not been proved.

Fix a cube `D` of a fixed current size `CM₁` and use the minimal determining set `B_k(D)` of CMP119 (2.13). For a weakly curved current field `v` on its fixed enlargement, define the orbit-valued map

\[
 \mathcal P_{k,D}(v_D)
 =U\bigl(\mathbb B_k(D),M'(Q_k^{s*}v_D)\bigr).
 \tag{RK.15a}
\]

Its dependence on raw current links is exactly local by its displayed determining data. The intermediate averages of a step lift have the same step form on the nested grids: the internal block links are identity and crossing links carry the prescribed coarse matrix. Thus the mixed determining plaquette condition of CMP102 (7) is controlled by `Cε` when the current plaquette bound is `ε`. At interfaces one retains the source mixed plaquette convention rather than inventing missing boundary links. Theorem 1 supplies the local minimum. On the homogeneous current-scale interior of `D`, separated from its artificial boundary collar, it gives

\[
 |\mathcal P_{k,D}(\partial p)-1|\le C\epsilon\eta^2,
 \qquad M^k(\mathcal P_{k,D})=v_D
       \quad\hbox{on the interior current determining bonds}.
 \tag{RK.15b}
\]

The constants are uniform in `k`; the domain and its current size are fixed. The finer artificial boundary collar has the weaker multiscale regularity allowed by `B_k(D)`, so (RK.15b) is not asserted there. Local analytic dependence and local gauge representatives follow from the same variational construction and its analytic-response propositions. Gauge covariance of the orbit follows from uniqueness and covariance of the constraints; any chosen local axial/AL representative and its orientation must retain the actual patch footprint.

Consequently a new interpolation citation is not needed merely to obtain a smoothed local patch. What remains is to join or decouple these patches in one gauge-compatible family with the identities below. Choosing a different patch at each bond can create uncontrolled fine-scale jumps, and choosing the global minimum to align all patches would reintroduce the raw dependence being localized. Nor does a local gauge transformation fix the unsmoothed lift itself: (RK.15) is gauge invariant.

### The common family still needed

A sufficient constructive route to (RK.12)–(RK.14) is a **current-normalized local regular prolongation with an admissible decoupling family**. On each connected current-block carrier meeting `D₀`, it must provide the actual constrained variational/constraint maps from raw retained links, with all of the following identities built into the same map:

1. At the physical decoupling endpoint it is the actual source map, including `V_Λ`, the AL compensator, the nonlinear constraint correction, and the old precision arguments.
2. At zero exterior decouplers its restriction to a component uses only the raw data on that component and the fixed old core state. Components separate exactly. It is not obtained by masking coefficients of an inverse after inversion.
3. On one fixed enlarged decoupling polydisc, uniformly in `k`, all admitted old descriptors and their hard-supported states, its reconstructed fields lie in the precise LFR II (1.65) native regularity/analyticity spaces with fixed slack. The gauge maps use actual local footprints, and the change of old coordinates preserves the literal support or records the complete Jacobian.

With such a family, CMP116's Cauchy/connected-set expansion supplies the missing actual supports; the source's native estimates can then be used on the verified domain. PR supplies inverse and square-root locality once the primitive coefficient carriers exist. GM supplies a consistent normalized Gaussian marginal once its covariance carriers exist. Neither theorem creates the primitive nonlinear raw prolongation or proves item 3.

The stated source proof of (1.65) has the whole-component choice of `Y₁` and does not prove these identities on arbitrary bounded-core carriers. The published real local-minimum theorem is not the missing enlarged-polydisc theorem. This is the concrete remaining input, rather than an assumed bound for the marked numerator.

The present analysis therefore resolves the matrix comparison and rejects the proposed step-lift shortcut, but leaves BC.2 for the complete actual residual kernel open. The already proved RT/MW energy and native-current results remain valid at their stated scope. Even a future proof of BC.2 would still require the actual incoming marked budget: RT's total old energy is of order `P(g_k)²`, whereas a local core regulator can be small, and Annex Y does not turn a bare microscopic `a⁻⁴` coefficient into `h⁻⁴` by conditional contraction.

## 7. A normalized Gaussian alternative to the pointwise BC hypothesis

The normalization must be kept before estimating a Gaussian change of background. This gives exact cancellation of the trace term, which a pointwise bound on the unnormalized quadratic form loses.

Let `μ₀=N(0,K₀⁻¹)` and `μ₁=N(0,K₁⁻¹)` on the same actual independent-coordinate space, and put

\[
 H=K_0^{-1/2}(K_1-K_0)K_0^{-1/2},
 \qquad \|H\|\le r<1.
 \tag{RK.16}
\]

All expressions are finite dimensional here; a bound uniform in their dimension is a separate conclusion of the formulas. In the whitened coordinate `x=K₀^{1/2}a`, the exact density ratio is

\[
 L_H(x)=\det(I+H)^{1/2}\exp[-\tfrac12 x^THx].
 \tag{RK.17}
\]

### Theorem RK.2 — dimension-free relative Gaussian bounds

For `p≥1` with `pr<1`,

\[
 \mathbb E_0 L_H^p
   =\det(I+H)^{p/2}\det(I+pH)^{-1/2},
 \qquad
 \log\mathbb E_0 L_H^p
   \le C_{p,r}\|H\|_{\mathrm{HS}}^2.
 \tag{RK.18}
\]

One explicit sufficient constant is
`C_{p,r}=p(p−1)/[4(1−r)²(1−pr)²]`. In particular, for `2r<1`,

\[
 \|L_H-1\|_{L^2(\mu_0)}^2
       \le \exp[C_{2,r}\|H\|_{\mathrm{HS}}^2]-1.
 \tag{RK.19}
\]

The Hellinger affinity has the exact value

\[
 \mathcal A(\mu_0,\mu_1)
 =\mathbb E_0 L_H^{1/2}
 =\det(I+H)^{1/4}\det(I+H/2)^{-1/2},
 \quad
 -\log\mathcal A\le C_r\|H\|_{\mathrm{HS}}^2.
 \tag{RK.20}
\]

Consequently their total-variation distance, in the convention `sup_A|μ₁(A)−μ₀(A)|`, is at most `C_r min(1,‖H‖HS)`. For a square-integrable insertion,

\[
 |\mu_1F-\mu_0F|
 \le\|F\|_{L^2(\mu_0)}
       \big[\exp(C_{2,r}\|H\|_{\mathrm{HS}}^2)-1\big]^{1/2}
 \tag{RK.21}
\]

whenever `2r<1`.

**Proof.** Diagonalize the symmetric matrix `H` and integrate the independent scalar Gaussians. This gives the determinant identity in (RK.18). For an eigenvalue λ, put
`f_p(λ)=p log(1+λ)−log(1+pλ)`. Both its value and its first derivative vanish at zero, and

\[
 f_p''(\lambda)
 =\frac{p(p-1)(1-p\lambda^2)}
 {(1+\lambda)^2(1+p\lambda)^2}.
\]

Taylor's integral formula and `|λ|≤r` give the displayed constant after the factor one half in the logarithm of (RK.18). Since `E₀L_H=1`, (RK.19) follows by expanding `(L_H−1)²`. The same determinant calculation at `p=1/2` proves (RK.20); its logarithm again has no first-order term and is bounded by a constant times `Σλ²`. Cauchy–Schwarz applied to the square roots of the two densities gives the total-variation bound. Applying it to `F(L_H−1)` proves (RK.21). ∎

Thus a logarithmic-density supremum may grow with rank while the normalized change remains bounded by a Hilbert–Schmidt quantity. Conversely, operator-norm smallness alone does not imply a dimension-uniform result: for `H=εI_D`, the squared Hilbert–Schmidt norm is `Dε²`. The trace cancellation removes the linear rank loss, but it does not remove this quadratic rank loss.

### The separate normalized kernel score

Let `K_t` be a differentiable positive family and set `C_t=K_t⁻¹`. Its exact centered score is

\[
 S_t(a)=\partial_t\log d\mu_{K_t}(a)
 =\frac12\operatorname{Tr}(C_t\dot K_t)
      -\frac12 a^T\dot K_ta.
 \tag{RK.22}
\]

It has mean zero and

\[
 \|S_t\|_{L^2(\mu_{K_t})}^2
   =\frac12\|C_t^{1/2}\dot K_tC_t^{1/2}\|_{\mathrm{HS}}^2,
 \qquad
 \|S_t\|_{L^p}\le C p
       \|C_t^{1/2}\dot K_tC_t^{1/2}\|_{\mathrm{HS}},\quad p\ge2.
 \tag{RK.23}
\]

The variance is Wick's identity. The higher-moment estimate follows by applying the product Gaussian moment-generating formula to the centered quadratic form (or the elementary second-chaos bound); a sharper version separates `sqrt(p)‖·‖HS` and `p‖·‖op`. Consequently, on its actual differentiability domain,

\[
 \partial_t\mu_{K_t}F_t
   =\underbrace{\mu_{K_t}\dot F_t}_{B_t}
    +\underbrace{\mu_{K_t}(F_tS_t)}_{J_t}.
 \tag{RK.24}
\]

This is a separate kernel record with the determinant term included, not a cancellation between the direct and kernel records. One may use Hölder with (RK.23) and the supplied incoming marked moment. At finite endpoints the two-copy rectangular split of M.30 applies to the same expectations and preserves the separate records exactly.

There is an additional useful exact identity for a local quadratic mark. If
`F(a)=aᵀPa+ℓᵀa+c`, with symmetric `P`, Wick's identity gives

\[
 J_t=-\operatorname{Tr}(P C_t\dot K_tC_t),
 \qquad
 |J_t|\le\|C_t^{1/2}PC_t^{1/2}\|_{\mathfrak S_1}
          \|C_t^{1/2}\dot K_tC_t^{1/2}\|.
 \tag{RK.25}
\]

The linear part has zero pairing with this centered even score. A local finite-rank `P` therefore pays its local trace rank, not the whole old Gaussian rank. This is a genuine closed Gaussian subcase. Extending it to the actual old mixture, hard cutoffs, nonquadratic microscopic mark and interacting density requires the corresponding source estimates; they are not consequences of Wick's identity.

For the raw residual problem, (RK.18)–(RK.25) suggest a weaker viable target: localize the **relative precision perturbations and scores** in Hilbert–Schmidt/trace ideals, with actual raw carriers and with the exact normalizer, or prove their pairing with the supplied rooted marked class directly. No source theorem checked in this analysis supplies that composed raw Schatten estimate for all surviving old histories. This route remains available even if the pointwise BC target (RK.14) is too strong.

## 8. A complete energy-weighted reduction for Gaussian precision carriers

There is an even more direct way to avoid a uniform old-state logarithmic-density bound when the reference has exponential moments of a common old energy envelope. It requires an operator-norm carrier budget, rather than a uniform rank bound or a Schatten estimate.

Fix the padded old sectors. For each old Gaussian factor let its reference Schur precision be `S⁰_{j,γ}`, with
`mI≤S⁰_{j,γ}≤MI`. Its raw retained dependence is required to be confined to `D₀`; dependence on the integrated core state is allowed. Suppose the **actual** precision difference has real symmetric carrier tags

\[
 S_{j,\gamma}-S^0_{j,\gamma}
       =\sum_{X\supset D_0}\Delta S_{j,\gamma,X}(v_X,u),
 \qquad
 \|\Delta S_{j,\gamma,X}\|\le a_X,
 \qquad
 a:=\sum_X e^{\kappa(|X|+t(X))}a_X<m.
 \tag{RK.26}
\]

The deterministic `a_X` bound is simultaneous in `j,γ,v,u`; this is the order of supremum and sum needed below. Let the common reference energy envelope satisfy

\[
 E(u)\ge\sum_j[\dim I_{j,\gamma}+\|A_{j,\gamma}(u)\|^2].
 \tag{RK.27}
\]

### Theorem RK.3 — the Gaussian log ratio has an energy-weighted carrier budget

Retain precisely those determinant factors present in the actual density. For normalized Gaussian factors the complete logarithmic ratio

\[
 \sigma_G
 =\frac12\sum_j\operatorname{Tr}\log\!left[
      I+(S^0_{j,\gamma})^{-1}(S_{j,\gamma}-S^0_{j,\gamma})\right]
  -\frac12\sum_j
      \langle A_{j,\gamma},(S_{j,\gamma}-S^0_{j,\gamma})
                              A_{j,\gamma}\rangle
 \tag{RK.28}
\]

has actual carrier tags `σ_{G,X}` with

\[
 |\sigma_{G,X}(v_X,u)|\le b_X E(u),\qquad
 \sum_X e^{\kappa(|X|+t(X))}b_X
   \le\frac a2+\frac12[-\log(1-a/m)].
 \tag{RK.29}
\]

In particular the right side is at most `C_m a` if `a≤m/2`. The constant is independent of the total old rank and the number of old scales. If a factor is unnormalized, omit its determinant contribution in (RK.28), retaining its genuine source normalization wherever it occurs instead.

**Proof.** The quadratic term has the exact supported expansion indexed by `X`. Its absolute value at a fixed `X` is at most
`(a_X/2)Σ_j||A_j||²≤(a_X/2)E`.

For the determinant use the convergent trace-log series. A word of length `n` with carrier indices `X₁,…,X_n` has trace bounded by

\[
 (\dim I_{j,\gamma})m^{-n}\prod_{\ell=1}^n a_{X_\ell}.
\]

Its actual raw support is `X₁∪⋯∪X_n`, since every inverse reference matrix depends only on `D₀`. This union is connected and its weight is at most the product of the weights. Sum over `j` and use (RK.27), then sum the individual deterministic word bounds before aggregating by carrier. The resulting budget is
`(1/2)Σ_{n≥1}(a/m)^n/n=(1/2)[−log(1−a/m)]`.
The same series defines the physical logarithm because the perturbation norm is less than one and the real precisions are positive. Together with the quadratic part this proves (RK.29). ∎

The theorem is an exact reduction of a **kernel coefficient** estimate. It does not assume a marked numerator estimate. If the local positive reference satisfies
`ν₀Eⁿ≤n!(C K)ⁿ`, an exponent with a bound of the form (RK.29) is small in its normalized exponential series whenever `aK` is sufficiently small. For an incoming mark bounded by `bE`, the numerator is paid by the same moments with one additional energy factor. The energy-weighted quotient argument makes this implication precise.

This shows what must actually be proved for the old precision sector: construct the local positive references and the operator carrier tags in (RK.26), including every actual old Schur pullback. One need not prove the much stronger pointwise old-state bound (RK.14), or postulate a uniform old rank. Coarea/Jacobian factors that change with the same raw-coordinate map and cross-component interactions still require their own energy-weighted tags; unchanged factors remain in the positive reference. Retained-only factors common to all old states cancel exactly. A factor that varies with the old descriptor does not cancel merely because it is independent of its continuous variables.

The common energy in (RK.27) and its reference moment bound must be checked for the actual chosen reference; RT's native tail does not certify an arbitrary locally truncated law. This is the remaining reference-map issue in a concrete form.

## 9. The homogeneous reference obstruction is resolved

The construction in [local bundle reference](local_bundle_reference.md) proves a local regular reference on homogeneous weak-curvature SU(N) current data, without a global weak-link gauge or an iterated step lift. Its projection, dual-frame and SU-connection formulas have a fixed raw-current footprint. Exact current edge holonomies, fine `εη²` curvature and `εη³` divergence, and the uniform literal-average discrepancy are proved explicitly. A local center-fixed Kato identification verifies the stronger native complex-field domain. Section 9 of that note applies the actual force-containing CMP102 fixed point and the common CMP116 decouplers to obtain homogeneous variational raw carriers.

Accordingly the inability of the naive step lift to furnish a homogeneous regular reference is no longer a remaining lemma. The Abelian test of Section 5 still rules out that particular lift. What remains for RK.26 is the actual mixed determining map and its complete old-factor comparison, including specified fine data, every old Schur and coarea term, and the cross action. The homogeneous construction is not an identification of those mixed factors with a raw-local positive reference law. The incoming microscopic mark and local moment budget are also unchanged by this advance.

## Mathematical sources

- CMP119 (1988), pp.246, 251–254, 257–258, 261–262: (1.3), (1.22)–(1.30), (2.13)–(2.22), (2.27), (2.31), (2.42), including the two Schur formulas and the step-lift definition.
- CMP99 (1985), pp.409–428: local parametrix/random-walk constructions and uniform weighted propagator bounds; these are native-background bounds and do not themselves identify raw retained carriers.
- CMP98 (1985), pp.17–51: forward averaging and analytic dependence; no regular local inverse is inferred.
- CMP102 (1985), pp.278–281, 305–309: variational domain, inductive reference construction, and local analytic response.
- LFR I (1989), pp.192–201: (1.73)–(1.100), actual prepared coordinates, AL gauge, and unchanged inner old operation.
- LFR II (1989), pp.370–380: (1.50)–(1.75), pre-grouped localization, whole-component analytic reconstruction, and relative native comparison.
- Companion proofs: [physical carrier resolvent](physical_carrier_resolvent.md), [ambient gaussian marginal](ambient_gaussian_marginal.md), [bounded core quotient](bounded_core_quotient.md), [residual trial mass](residual_trial_mass.md), [residual merger witness](residual_merger_witness.md), [M04 Bounded Core Source Map](M04_Bounded_Core_Source_Map.md).
