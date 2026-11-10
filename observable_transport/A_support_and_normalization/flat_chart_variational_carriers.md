# An all-depth raw-carrier construction on a common weak-link chart

This note proves one restricted primitive variational theorem without using an unsmoothed step lift. The restriction is explicit: the homogeneous current retained links lie in one fixed product chart around the identity. The theorem is uniform in the fine depth and volume. It does not cover all weak-curvature gauge fields by silently choosing a nonlocal gauge. A concrete failure of naive gluing of local minimum orbits is given at the end.

## 1. The regular reference can be exactly flat at every depth

Use current lattice units, with fine mesh `η=L⁻ᵏ`, and impose homogeneous `k`-fold averages on the whole current lattice. Write the raw retained links as

\[
 v_c=\exp(iB_c),\qquad \|B\|_\infty<\varepsilon_*.
 \tag{FC.1}
\]

The same fixed logarithm is used on the complex product ball. The Lie-algebra multiplicity per current bond is fixed. There are no inherited large-field holes in this theorem.

Take the reference fine field to be `U₀=1` and the reference coarse field `V₀=1`. This is an exact regular minimal configuration at every depth. CMP102 p.280, hypothesis (14), permits a regular reference whose determining averages differ from the specified data by a sufficiently small amount; the reference need not already have those specified averages. More directly, Section G, (172)–(180), takes `U₀=U_k(V₀)` and constructs `U_k(exp(iB)V₀)` analytically. Thus `U₀=1` is legitimate for every `k` in (FC.1). No fine curvature concentrated on coarse faces is introduced.

Two primary-source facts make the constants uniform in `k`:

- CMP98 pp.38–42, Propositions 4–5, gives the nonlinear `k`-fold averaging remainder on the two adjacent current `k`-blocks, with analytic and derivative constants independent of `k`.
- CMP99's flat propagators have their stated uniform source norms and generalized random-walk representations. CMP102 Proposition 4, especially (98), gives the corresponding uniform quadratic nonlinear bound, and Section G gives the analytic fixed point.

The nonlinear averaging map is local in **current physical blocks** even though the number of fine coordinates inside each block grows with `k`. Its bounds are the source's normalized field/operator bounds, not an unweighted sum of all fine coordinate derivatives.

## 2. The actual equations and their decoupling

Let `H₀,H,G` denote the flat operators in the source representation of the Landau increment. Schematically, but with the actual source maps identified,

\[
 D=\mathcal C_k(A'-HD),\qquad
 A_0+G\mathcal N_H(H_0B+A_0)=0,
\]

\[
 \mathcal A_k(B)=H_0B+A_0
              -H D(H_0B+A_0).
 \tag{FC.2}
\]

Here `C_k` is the exact nonlinear averaging remainder of CMP98; `N_H` is the derivative of the exact transformed Wilson remainder. These are CMP116 (1.2)–(1.5), specialized to the flat reference, or CMP102 (174)–(180). At this reference the original force is zero. The terms displayed in the remainder begin at second order in the normalized small fields. The source inverse block gauge map converts `exp(iη A_k)` to the actual axial representative. It is retained, not replaced by a new saddle.

Partition current physical space into the fixed source cubes of side `M`. Attach a complex parameter `s_Δ` to every such cube outside a fixed root buffer. In each generalized random-walk term of `H₀,H,G`, multiply by the product of the parameters of all cubes met by its **full** localization domain. This is exactly the construction preceding CMP116 (1.9). It uses flat coefficient operators, so none of these primitive coefficients has a hidden raw-field argument.

Fix a radius `R=exp(κ₁)>1`. The source estimate (1.11) gives the same operator bounds on `|s_Δ|≤R`, with the explicit possible enlargement `B₀ exp(16κ₁)`, after the source block size is chosen so `δ₁M≥κ₁`. The source then proves the nonlinear contraction and analytic continuation, (1.13)–(1.18). For example the sufficient restrictions include

\[
 4C_2B_0e^{16\kappa_1}\varepsilon_2<1,
 \qquad
 4C_4B_0^2e^{32\kappa_1}\varepsilon_3<1,
 \qquad
 2B_0e^{16\kappa_1}\varepsilon_3\le\varepsilon_2.
 \tag{FC.3}
\]

Choose a strict margin in these inequalities and then choose `ε_*` so the raw `B` ball of radius `2ε_*` maps inside `ε₃`. This leaves a fixed analytic margin around the closed ball used below. The choices depend on `L`, the group and fixed source parameters, but not on `k` or total volume. The resulting solution obeys the current-scale version of the source regularity bounds,

\[
 \|\mathcal A_k(B;s)\|_{\mathrm{reg}}
       \le C_R\|B\|_\infty,
 \tag{FC.4}
\]

on the full enlarged polydisc. Here `‖·‖reg` denotes the field and derivative norms occurring in CMP102 (19)–(21) and CMP116 (1.18), restricted at an output current block; in the homogeneous current region their scale factors are the current ones. In particular the Landau field has a bounded current potential and derivative, and its fine plaquette curvature is `O(ε_*η²)`.

The fixed point is the actual minimum only at `s=1`. At other decoupler values it is the analytic extension of the source equations. No claim of exact stationarity or exact original averaging at every complex `s` is needed or made. If these functions are used inside a fluctuation action, the already critical-cancelled normal form must still be continued, as in the earlier first-clean construction.

### Exact component identity

When the parameters outside a union `Y` are set to zero, the modified propagators have kernels only within its components, with the source boundary buffers. The nonlinear averaging operation uses two adjacent current blocks. The buffers therefore separate its equations as well. CMP116's proof following (1.9) applies verbatim to (FC.2): the solution at the root depends only on the current raw variables `B` in its root component and the fixed collar.

This is an exact identity of the maps, not a decay estimate. It is consistent under enlargement of `Y`, because every coefficient family is obtained from the same flat walk series and the same fixed-point equations with different parameter masks. The inverse axial gauge reconstruction uses only the corresponding current averaging block: CMP98 pp.29–33, (77), (87), and (104)–(106), express the gauge by the nested contours and averages inside that block. At a given level its small logarithms are bounded by `C L^j η ε_*`; their sum over `j<k` is bounded by `C ε_*`, since `L^kη=1`. The analytic neighborhood and bound are therefore uniform in depth. Including that fixed current collar preserves the support identity for the actual source readout. For a fine link crossing a block boundary both endpoint blocks are included.

## 3. The connected raw-carrier theorem

Let `S_x` be the fixed root buffer for a fine output link, plaquette, or local source-normalized field component at current position `x`. All carriers below are sets of **current physical blocks**. The fixed source cubes and averaging collars are included in their footprints.

### Theorem FC.1

There exist `ε_*>0`, `κ>0` and `C<∞`, independent of `k` and volume, such that on the product chart (FC.1) the homogeneous constrained minimum, in its source Landau field and its local axial readout, has an actually supported tagged expansion. For the Landau field at the root it has the form

\[
 \mathcal A_{k,x}(B)
      =\sum_{Y\ni S_x}\mathcal A_{k,x,Y}(B_{\operatorname{foot}Y}),
 \tag{FC.5}
\]

with connected footprints and

\[
 \sum_{Y\ni S_x}
 e^{\kappa(|\operatorname{foot}Y|+t(\operatorname{foot}Y))}
 \sup_{\|B\|_\infty\le\varepsilon_*}
       \|\mathcal A_{k,x,Y}(B)\|_{\mathrm{reg},x}
       \le C\varepsilon_*.
 \tag{FC.6}
\]

The same conclusion applies to local analytic readouts after charging their explicit root bound and a fixed part of the decay. Gauge-invariant plaquette readouts have their genuine fine-curvature normalization; a gauge-dependent axial link is not assigned the bounded Landau-potential norm without its actual gauge map.

**Proof.** Apply the product fundamental theorem of calculus in the decouplers, as in CMP116 (1.9)–(1.10), before any coefficient aggregation. The component identity above makes every term with a differentiated component disjoint from the root vanish. The remaining term has exactly the raw dependence declared in (FC.5).

For `n` differentiated cubes, Cauchy on a circle of radius at least `R−1` about the real integration point gives the deterministic bound

\[
 C_R\varepsilon_*(R-1)^{-n}.
 \tag{FC.7}
\]

There is no `n!` in this estimate: each distinct decoupling parameter is differentiated once. Use one coefficient tag for each fundamental-theorem carrier, together with any necessary output-record labels. The propagator walks and fixed-point iterations remain internal to the analytic construction of that coefficient. Bound (FC.7) is a bound on the entire differentiated map; it is not asserted as an absolute sum over separately exposed internal walk indices. The number of connected source-cube sets of size `n` containing the fixed root is at most `A_d^n` times a fixed root constant. The full physical footprint satisfies

\[
 |\operatorname{foot}Y|+t(\operatorname{foot}Y)
       \le C_M(n+1),
 \tag{FC.8}
\]

where `C_M` includes the volume of each fixed source cube and the actual local averaging/gauge collars.

Choose `R>A_d+1` with a strict margin, then choose the source buffer `M` large enough for its walk bound, and finally choose a positive `κ` so
`A_d exp(κ C_M)/(R−1)<1`. Shrink `ε_*` according to (FC.3) after these choices. The geometric sum of (FC.7), including the physical weight, proves (FC.6). All of these choices are uniform in `k` because the averaging and flat propagator constants used in (FC.2)–(FC.4) are uniform in `k`.

The source axial readout is an analytic function of this Landau solution on one current block. Including that block's collar and applying the same fixed-point/component and Cauchy argument proves its supported expansion. At `s=1` it is the actual variational minimum with the original prescribed averages by CMP102 Proposition 9. ∎

The proof never turns off arbitrary weak-curvature raw links and then assumes that curvature remains admissible. Its raw domain is the explicitly admitted product ball (FC.1); setting any of those `B` variables to zero stays inside that ball. More importantly, the actual locality identities were established by the common propagator family before performing the expansion.

## 4. Mixed raw derivatives and the local Euler system

The theorem also gives uniform mixed raw-coordinate jets. Restrict to the inner ball `‖B‖∞≤ε_*/2`. For any list of raw current coordinates `c₁,…,c_m`, Cauchy applied to the individual tagged coefficients gives

\[
 \sum_Y w_\kappa(\operatorname{foot}Y)
 \sup_{\|B\|\le\varepsilon_*/2}
 \|\partial_{c_1}\cdots\partial_{c_m}
          \mathcal A_{k,x,Y}\|
 \le C\varepsilon_* m!\,(C/\varepsilon_*)^m.
 \tag{FC.9}
\]

Each derivative is zero unless its coordinate belongs to the declared footprint. Thus a spanning-tree distance joining `x,c₁,…,c_m` can be extracted from the weight, giving a tree-decaying mixed derivative estimate with the same depth-independent constants and a possibly smaller rate.

One can see the same jets directly by differentiating the local fixed-point system. If its nonlinear unknown is `y=T(B,y)`, the strict contraction gives

\[
 D_By=(I-D_yT)^{-1}D_BT.
 \tag{FC.10}
\]

At higher orders, the chain rule attaches derivatives of `T` to the leaves of the earlier derivatives; inversion by the same resolvent produces rooted trees. The local nonlinear vertices and flat random-walk propagators account for every connection. This agrees with the analytic coefficient construction above. The support conclusion is not inferred from (FC.10) alone: it follows from the already constructed common component family (FC.2).

The small parameter of this construction is the physical weak-link radius `ε_*`, after the source parametrix buffer is fixed. The underlying flat walk/parametrix error is made small by the source block buffer. This is a successful primitive construction on a common chart; it is not a nonlinear Schwarz theorem for arbitrary weak-curvature gauge data.

## 5. Why this does not yet glue arbitrary local minimum orbits

The local source minima in [residual raw kernel bridge](residual_raw_kernel_bridge.md), (RK.15a), provide regular patches on arbitrary weak-curvature data. They are initially specified as gauge orbits, with local analytic representatives. A naive partition-of-unity interpolation of independently chosen representatives does not preserve their scale-normalized regularity.

There is a concrete Abelian example inside any fixed torus subgroup of the gauge group. Let the two local representatives be

\[
 U^{(1)}=1,\qquad U^{(2)}_{xy}
       =\exp\{iT[\phi(x)-\phi(y)]\}.
 \tag{FC.11}
\]

Choose `φ=0` at current block centers, with amplitude `δ` and a fine oscillation in the second direction. Both fields have identically zero plaquette curvature, lie in the same minimal orbit, and have identical coarse averages, by gauge covariance of the averaging. Their relative fine gauge may nevertheless vary on the fine lattice scale.

If one interpolates their link logarithms with a smooth current-scale partition `χ(x)` varying in the first direction, the interpolated Abelian connection contains `χ dφ`. Its curvature contains

\[
 d\chi\wedge d\phi.
 \tag{FC.12}
\]

With `|dφ|` of order `δ/η`, this produces a fine plaquette angle of order `δη`, rather than the required `O(δη²)`. The violation grows by `η⁻¹`. All input plaquette curvatures were exactly zero. This is a failure of the naive representative interpolation, not a no-go theorem for gauge-compatible gluing.

Even after compatible regular representatives are found, simple interpolation does not preserve the exact averaging constraint. In the linearized notation, the residual contains the commutator `[Q_k,χ](A_1−A_2)`. A smooth current partition may make this `O(1/M)` in the correct norm, but its correction must use one common constrained right inverse and its gauge maps. The source local-patch existence theorem does not construct those common data automatically.

Equation (181) of CMP102 extends the variational minimum covariantly to gauge orbits. For a **prescribed gauge transformation independent of the raw field**, applying it to the entire construction above preserves locality, with the corresponding fixed representatives. Selecting a gauge from the raw retained field is different: its dependency footprint must be charged. A spanning-tree gauge chosen on a large region can have paths outside the intended carrier. The pointwise orbit extension is therefore not yet a compatible ambient carrier extension for M-03.

The restricted theorem FC.1 resolves the smooth primitive map on a global weak-link product chart at arbitrary depth. The naive representative interpolation above does not provide an extension beyond that chart.

### The homogeneous weak-curvature extension

The [local bundle reference](local_bundle_reference.md), Theorem BR.1 and Section 9, closes the homogeneous regular-reference problem by a different construction. A local near-projection is corrected to a rank-N bundle, with explicit dual frames, an exact SU reduction, the correct coarse edge holonomies, uniform fine curvature/derivative bounds, and a local Kato comparison for the native complex domain. Its literal nonlinear averages are `O(ε)` from the prescribed data uniformly in depth, which suffices for CMP102 (14). The actual force-containing variational equations then give the same common component construction on homogeneous weak-curvature data. The mixed determining geometry, specified old factors, and complete old Schur/coarea/cross pullback remain separate. The bundle construction does not supply the missing microscopic scalar transport budget, and neither FC.1 nor BR.1 completes M-04.

## Mathematical sources

- CMP98 (1985), pp.29–33, (77), (87), (104)–(106): the block-local inverse axial gauge; pp.38–42, Propositions 4–5 and (133)–(157): current-block locality and depth-independent analytic/derivative bounds for the nonlinear averaging remainder.
- CMP99 (1985), generalized random-walk propagators and normalized bounds used explicitly in CMP116 (1.6)–(1.11).
- CMP102 (1985), p.280 (14); pp.292–294, Proposition 4 and (98); pp.305–309, (172)–(190) and Proposition 9: the regular reference, nonlinear equations, analytic expansion and exact physical readout.
- CMP116 (1988), pp.2–7, (1.2)–(1.21): common decoupled propagators, exact component identity, enlarged-disc contraction and bounds.
- [residual raw kernel bridge](residual_raw_kernel_bridge.md): distinction between local regular patches, a raw-local core law and the unresolved old Schur comparison.
