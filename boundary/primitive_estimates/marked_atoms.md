# Majorants for marked atoms and composition of prefixes

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

**Status.** On the retained C01/J0 source construction and the stipulated AF class, the conditional-law estimates C-01 through C-08 hold in the sense stated in [Conditional law on admissible heterogeneous backgrounds](../conditional_law_theorem.md). C-01–C-04 and C-07 are inputs; C-05 is the assembly below together with the two-age replacement of OR.19 in [Ordinary stopped-density oscillation on mixed scales](../ordinary_oscillation.md) (especially Sections 3–8, with the source analysis in Addenda A–D of [Ward estimates, cutoff residuals and polarization tensors](../ward_source_derivation.md)); the C-06 and C-08 applications are in [Heterogeneous constrained precision and coercivity](../heterogeneous_coercivity.md) and [Regular conditional covariance, moments and cumulants](../conditional_probability.md). The explicit radius dictionary and conservative external-map loss are in Section 3 of [Conditional law on admissible heterogeneous backgrounds](../conditional_law_theorem.md). The C-05 assembly itself is the fixed-fiber normalization and positive boundary induction of [Complete boundary activities and normalized component induction](../boundary_induction.md) (FP.1–FP.26). The transition from OR.14–OR.16 to OR.19 alone does not supply the integration-response decay when \(b\le n<j\); the two-age interpolation supplies it on the stipulated AF/C01/C02 source scope. The AF trajectory is a stipulated input. The independent AF/source construction, general M03/M07 regulator conversion, moving-selector flux SS, projected microscopic marks, outer-history transport and continuum Yang–Mills identification are not established here. The all-history application of the C-08 regular law is assigned to H-04.

**Norm convention.** The activity labels in the final norm are complete coarsened atoms [PC.12](positive_catalog_coarsening.md). A linear prefix block is summed before new native Taylor expansion and Gaussian conditioning. [PC.1](positive_catalog_coarsening.md)–[PC.6](positive_catalog_coarsening.md) and [ND.4](native_domain_count.md) prove this order of operations, with the literal self kernel of one source-permitted representation fixed before iteration. [CT.1](operative_source_scope.md)/[ND.1](native_domain_count.md) supplies the actual per-component, proper-mesh coordinate count. The canceled internal labels are not separately normed pieces. Section 30 below records the norm passage.

## 1. Result and exact application boundary

Independent activity marks give a useful positive lift of the final scalar estimate. The decisive place to introduce them is the **linear localization and resummation before exponentiation**, not the already nonlinear connected logarithm.

For a fixed actual history, suppose the last linear resummation produces

\[
 V_Y(z;\xi,\omega)=v_{Y,0}(\xi,\omega)
       +\sum_{a\in A}z_a v_{Y,a}(\xi,\omega).
\tag{M1}
\]

The label `a` may be one incoming boundary activity with its birth and carrier, or one consistently marked old/new-history add-back block. It need not distinguish the internal localization histories already summed into `v_{Y,a}`. If the final spatial bound holds uniformly for every independent `|z_a|<=1`, then

\[
 |v_{Y,0}(\xi,\omega)|+\sum_a|v_{Y,a}(\xi,\omega)|
 \le A_Y
\tag{M2}
\]

at every admitted common native point and every actual hidden-variable value. No factor depending on the number of marks occurs.

The pre-completion age estimate still bounds these **same resummed blocks**: take the triangle inequality over the localization histories inside each `v_{Y,a}`. Thus a final spatial estimate and the earlier age estimate can be put on the same positive coefficients without identifying a signed scalar norm with an absolute history sum. Positive-reference integration, the Mayer expansion and the connected cluster majorant then accept (M2) pointwise. The final current/native differentiation can be performed by the common-contour vector-valued Cauchy argument.

This positive lift is justified for the literal full-tree input class of LFR II (1.59)–(1.68), and for any relative input class on which the same scalar construction is already verified. It does **not** itself prove the missing mixed-old-hole spatial estimate. CMP119 p.262's explicit alternative frees the corresponding whole `Z_j`; the C05 geometry frees only genuine bounded completed components, possibly strict subcomponents of a later `Z_j`. That distinction remains substantive.

The improvement is therefore precise: once the scalar final-carrier estimate is established in the correct weaker/decorated metric, its positivity requirement need not be proved by tracking every signed localization term. Independent linear marks supply it. A remaining scalar metric transfer must not be disguised as a consequence of marking.

## 2. Dimension-free positive lifting at the linear stage

### Proposition M1 — phase lifting

Let `A` be finite. For complex numbers `c_0,c_a`,

\[
 \sup_{|z_a|\le1}\left|c_0+\sum_a z_a c_a\right|
   = |c_0|+\sum_a|c_a|.
\tag{M3}
\]

**Proof.** The triangle inequality gives the upper bound. If `c_0` is nonzero, choose each phase `z_a` so that `z_a c_a` has the phase of `c_0`. If `c_0=0`, choose an arbitrary common phase. Terms with `c_a=0` cause no difficulty. This attains the upper bound. QED.

Apply (M3) separately at each fixed `(xi,omega)` to (M1). A uniform bound on the full phase polydisc proves (M2). The maximizing phases may vary with that fixed point; no analytically varying phase field is introduced. The input theorem holds for every constant phase vector, which is exactly what this pointwise argument needs.

For countably many labels, apply the finite statement to every finite set, placing the remaining physical terms in the unmarked base, and pass to increasing sets. The nonnegative partial sums are bounded uniformly. Alternatively, work at finite cutoff throughout and take the already controlled cutoff limit. The constants do not depend on the number of marks.

If the bound contains a deterministic output weight `W_Y`, it is preserved:

\[
 \sup_{\xi,\omega}\sum_a W_Y|v_{Y,a}(\xi,\omega)|
 \le W_Y A_Y.
\tag{M4}
\]

This is a bound with the supremum **outside** the coefficient sum. It is not the generally stronger expression `sum_a sup_(xi,omega) |v_{Y,a}|`. The distinction is useful rather than a defect: the actual current and native targets are uniform pointwise sums on common admitted domains. Subsequent estimates should preserve that norm.

### Why activity blocks are the right labels

Write an actual linear contribution as

\[
 v_{Y,a}=\sum_{\ell\in L(Y,a)}v_{Y,a,\ell},
\]

where `ell` denotes the internal localization domains, Cauchy integrals or equivalent source records. If the established age estimate gives

\[
 |v_{Y,a,\ell}|\le q_{Y,a,\ell},\qquad
 q_{Y,a}:=\sum_\ell q_{Y,a,\ell},
\]

then `|v_{Y,a}|<=q_{Y,a}`. Hence the same blocks `p_{Y,a}=|v_{Y,a}|` have both the marked spatial bound and the old age bound. There is no need to mark every internal localization record separately. Doing that would require a larger input hypothesis that the native scalar bound does not state.

Nor should one mark an arbitrarily chosen decomposition of an incoming `B^(b)(X)` into summands. The input bound controls that admitted activity as a whole. Independent marks inside an unverified decomposition need not preserve the input class. One mark per admitted activity, or one mark per entire birth if sufficient, is safe.

## 3. Matching the marks to the linear source construction

All page references in this note are to printed page numbers of the primary sources.

### 3.1 What is held fixed

Fix one admitted actual history, its determining geometry, all raw/adjoint slots, its regularity domains, its classical background maps and the physical source measures. Mark the boundary scalar activities appearing at the stage under discussion. Do not modify the coupling trajectory, the classical part of the action, the determining-set selection or the hidden integration support.

Boundary activities have the native locality, gauge covariance, analyticity and bounds specified by CMP119 (2.40)–(2.42), pp.261–262. Multiplication by a constant complex scalar of modulus at most one preserves those properties. Individual boundary activities are the appropriate inputs here; marking regular E terms could interfere with their separately organized renormalization or covariance conditions and is unnecessary for the repeated-boundary bottleneck.

### 3.2 Every relevant pre-exponentiation step is linear

The following facts are directly visible in the source formulas.

| Source step | Dependence on an incoming boundary scalar |
|---|---|
| LFR II (1.59), (1.60), pp.372–373 | Evaluation and subtraction are linear. |
| Substitutions (1.61)–(1.64), pp.373–374 | The reconstructed maps are fixed; composition acts linearly on the incoming function. |
| Localization-parameter expansions, pp.373–376 | Differentiation, Cauchy/FTC integration and collection of domains are linear. |
| Summation over old carriers, births and types, p.376 | These are linear sums. |
| Last resummation and separation of self/nonself domains, p.377 | Classification uses fixed domains, followed by linear sums. |
| Restoring `A'_k` and subtracting its missing terms, p.377 | Addition/subtraction is linear in the prescribed old and reconstructed-history coefficient lists. |

Thus (M1) is an exact identity at this stage. Use the same mark for corresponding original-history and reconstructed-history terms whenever their cancellation is used. In particular, the deep-incidence refinement below marks complete **balanced reference blocks**, not the old and new addbacks independently. Native size bounds for two independent lists would not preserve an additional endpoint obtained from their cancellation. The physical identity is required at marks equal to one. There is no need to assert that every intermediate marked list is itself generated by a globally phase-marked Wilson history.

The source estimates at this stage use the absolute native bounds, Cauchy estimates and nonnegative domain sums. These operations are unaffected by multiplying a boundary input by a unit complex number. In particular the ordinary full-tree proof leading from (1.66) to (1.68) applies uniformly to all such marks. The source's final (1.68) therefore has the positive lift (M2) for this literal input class. The old and newly reconstructed boundary pieces can be assigned their stated separate input budgets; no cancellation between them is needed to justify this uniformity.

CMP119 p.262 explicitly says that the constructions and proofs also proceed with its alternative relative invariant. The next remark formulates the operation on the full space of densities satisfying the inductive assumptions. These statements support use of the appropriate **stated** input class, rather than only one previously generated numerical density. They do not alter which exceptional set is allowed in the bound.

### 3.3 Canonical self kernels are kept physical

Do not try to infer a uniformly small complex deformation of the canonical self kernel by independently marking every large incoming self-action. The real self-action can be extensive, and arbitrary complex marks could destroy positivity or the source's small-deformation comparison.

That inference is unnecessary. Stop the auxiliary marked construction at the linear nonself coefficients `v_{Y,a}`. For the nonlinear expansion use the **original physical** canonical `T'_v`, its mass `tau_v=T'_v 1`, and its normalized kernel `Pi_v`. Define an auxiliary family only by

\[
 \mathcal Z(z;\xi)
 =\left(\prod_v\Pi_v^\xi\right)
       \exp\!\left[v_0(\xi,\omega)
               +\sum_{Y,a}z_{Y,a}v_{Y,a}(\xi,\omega)\right].
\tag{M5}
\]

The marks in (M5) may now be independent even across output domains. The bound (M2) has already been obtained for each domain; introducing these new output marks uses that proven pointwise bound rather than a new source theorem. At every mark equal to one, (M5) is the physical nonself exponential under the unchanged canonical kernels. The self masses, selectors and real supports retain their exact source roles.

LFR II (1.71)–(1.75), pp.378–380, supplies the canonical kernel comparison. Its native normalized density relative to a fixed positive probability reference satisfies a bound of the form

\[
 |r_v(\xi,\omega_v)|\le M_v,
\tag{M6}
\]

with a uniform `M_v`; the exact `M_s=e^s/(2-e^s)` follows from the source small deformation as proved in the first analysis. This is the physical kernel, not a large phase-deformed replacement.

## 4. Pointwise positive integration and nonlinear completion

### Proposition M2 — hidden integration preserves the lifted majorant

Suppose `mu_0` is the actual product positive reference on the integrated slots, and the density factors satisfy (M6). Let `f_{a,j}(xi,omega)` be the factors in a fixed finite interaction family, and suppose

\[
 \sum_j|f_{a,j}(\xi,\omega)|\le a_a
\]

uniformly at the same external point and all actual hidden values. Then

\[
 \sum_{j_1,\ldots,j_q}
 \left|\int \prod_{a=1}^q f_{a,j_a}(\xi,\omega)
                    \prod_{v\in I} r_v(\xi,\omega_v)
                    \,d\mu_0(\omega)\right|
 \le \left(\prod_{v\in I}M_v\right)\prod_{a=1}^q a_a.
\tag{M7}
\]

**Proof.** Apply the triangle inequality inside the positive integral, interchange finite nonnegative sums and integration, and factor the independent label sums. Bound the actual density factors and the pointwise sums. For countable sums use Tonelli. No supremum is interchanged with an individual coefficient sum. QED.

The same proof works with the actual hidden internal histories included in `mu_0`. They are not enumerated again as independent polymer multiplicities. Moment products in a connected-cumulant expansion may use different copies of the hidden variables; apply (M7) on the corresponding product of the actual positive reference measures. The pointwise bounds hold for each copy.

### Mayer coefficients need no multivariate Cauchy extraction

At one fixed domain and one fixed `(xi,omega)`,

\[
 \exp\!\left(\sum_a z_a v_{Y,a}\right)-1
 =\sum_{\nu\ne0}\frac{z^\nu v_Y^\nu}{\nu!}.
\]

Consequently the exact sum of the absolute Taylor coefficients on the unit activity polydisc is

\[
 \sum_{\nu\ne0}\frac{|v_Y|^\nu}{\nu!}
 =\exp\!\left(\sum_a|v_{Y,a}|\right)-1
 \le e^{A_Y}-1.
\tag{M8}
\]

This is the positive activity majorant needed in the Mayer step. Repeated occurrences, including repeated birth labels, already have their exact factorial denominators. There is no independent multiplicity factor for the number of marks.

An unmarked base `v_{Y,0}` is included by the same inequality with `|v_{Y,0}|+sum_a|v_{Y,a}|`: the constant coefficient obeys `|exp(v_{Y,0})-1|<=exp(|v_{Y,0}|)-1`, and all nonconstant coefficients have the additional factor `exp(v_{Y,0})`. Equivalently, give the base its own auxiliary output mark after (M2) has been established.

If a fixed larger activity radius `R>1` is desired, replace `A_Y` by `R A_Y` in (M8). Choose the physical primitive smallness with a fixed margin so that the component-incidence criterion still holds at that radius. No age-dependent radius is required.

The source two-stage positive estimates can then be applied to these nonnegative majorants. LFR II (1.91)–(1.97), pp.388–390, explicitly retains the products of primitive amplitudes and the sums over their supports. The second normalized expansion on pp.391–392 retains one `e^3` factor for every newly used normalized component and omits a sum over its fixed component domain. Those factors remain in (M7) and in the rooted incidence weights; activity marking removes none of them.

The losses such as `alpha^(1/3)` are inequalities allocating a primitive small factor among several estimates. They are not nonanalytic operations on the actual activity. The finite-cutoff Mayer and connected-log expressions are analytic on their normal-convergence domains. Replacing `alpha` by `R alpha` for fixed `R` changes these bounds to `(R alpha)^(1/3)`, leaving the same fixed positive power of the collar suppression. This fits the previously stated closed-ball induction.

## 5. Combining the spatial and age bounds on the same coefficients

The cleanest common positive coefficients are

\[
 p_{Y,a}(\xi,\omega)=|v_{Y,a}(\xi,\omega)|
\]

**after** the entire linear resummation. The source age estimate before final completion supplies an upper bound on these by the triangle inequality. The marked scalar spatial theorem supplies (M2) on the same coefficients. No equality with the sum of absolute unresummed localization histories is asserted.

For any nonnegative deterministic incidence weight `u_{Y,a}`, final cost `t_Y`, and `0<theta<1`, Hölder gives, pointwise,

\[
 \sum_{Y,a\in\mathcal R}p_{Y,a}u_{Y,a}e^{\theta Kt_Y}
 \le
 \left(\sum_{Y,a\in\mathcal R}
   p_{Y,a}u_{Y,a}^{1/\theta}e^{Kt_Y}\right)^\theta
 \left(\sum_{Y,a\in\mathcal R}p_{Y,a}\right)^{1-\theta}.
\tag{M9}
\]

Here `mathcal R` is an actual rooted class. Taking suprema **after** the sums preserves this inequality with the corresponding uniform bounds. The same argument can be integrated over a positive reference. If the incidence weight depends only on the completed domain, (M2) bounds the first factor directly after the ordinary rooted domain count.

The old-root count `L^{4(k-b)}` must still be included in the age-side sum whenever it is an actual count of distinct birth sites. It cannot be dropped because a marking argument has been performed. Conversely, no new factor counting the number of marks is inserted. The established scalar suppression, including its fixed `g_k^{-a}` prefactor and age exponent, pays the genuine old-root count after the stated rate reserve.

For a fixed finite input ball, the resulting connected majorant is controlled by a finite function of that ball and a fixed positive power of the fresh nonself small factor. Its exact parameters depend on the scalar spatial theorem used on the first side of (M9). This note does not replace that theorem by the numerical recurrence it is meant to justify.

## 6. Why a direct nonlinear Cauchy argument would be insufficient

It is tempting to apply the final scalar bound to an activity polydisc and then sum absolute multivariate Cauchy coefficients. Without additional structure that incurs uncontrolled dimension entropy.

### A degree-two counterexample

Let `N=2^m` and let `H` be a real Hadamard matrix, so its entries have modulus one and `H H^T=N I`. Define

\[
 P_N(x,y)=N^{-3/2}\sum_{i,j=1}^N H_{ij}x_i y_j.
\]

For `|x_i|,|y_j|<=1`, Cauchy–Schwarz gives

\[
 |x^T H y|\le\|x\|_2\|H y\|_2
 \le\sqrt N\,\sqrt N\,\sqrt N=N^{3/2}.
\]

Thus `sup |P_N|<=1`, whereas the sum of the absolute degree-two coefficients is `sqrt(N)`. A fixed larger polydisc radius merely changes this by a fixed squared-radius factor. There is no dimension-free absolute-coefficient estimate even for these homogeneous quadratic polynomials.

Ordinary multivariate Cauchy on `N` variables with a common radius `R>1` gives a bound proportional to `(1-R^{-1})^{-N}` for the total coefficient sum. That is not an acceptable substitute for actual attachment counting. Infinite or depth-growing activity labels make the defect worse.

The safe order is therefore essential: lift the **linear** pre-exponentiation estimate by independent phases; then use the explicit positive exponential/product/tree majorants. Do not try to reconstruct their positivity from the supremum of an already nonlinear logarithm.

## 7. Exact remaining source-metric question

For the original full-tree incoming boundary class, the source matching in Section 3 proves the marked scalar final estimate, and therefore its positive lift. This is an actual application, not merely a statement about an arbitrary linear operator.

For repeated completed scalars, the necessary scalar norm is different. A completed activity can retain older bounded holes `H_m` outside the currently attempted union. Those holes can be strict subcomponents of a much larger later `Z_b`. The desired physical estimate must keep the ordinary, potentially unbounded large-field component paid while allowing only those genuine completed holes to be free.

CMP119 p.262 permits resummation over components of its actual `Z_j` and states the corresponding relative estimate. It does not literally assert the selectively decorated metric for arbitrary older strict subcomponents. LFR II (1.67), p.376, also charges the whole length through the exceptional region while omitting interior cell coverage. The second exponentiation, p.391, uses an exterior size after removing fixed eligible domains. These expressions cannot be identified without specifying the actual tree convention and the support-completion rule.

The marked theorem can be invoked as soon as one proves a scalar statement of the form

\[
 \sup_{|z_a|\le1}|V_Y(z;\xi,\omega)|
 \le C\alpha_k\exp[-K\ell_{\mathrm{decorated}}(Y)]
\tag{M10}
\]

for the true mixed fixed-hole input class, with the required rooted/volume reserves. If the proof of (M10) uses only the absolute input bounds, phase uniformity comes for free from the linearity already established. It is enough to prove the corresponding scalar bound on that input ball. No separate reconstruction of positive localization-history coefficients is then needed.

An adequate weaker quotient/decorated pushforward may establish (M10) without the full halo-visiting FH invariant. That option is treated in [Positive attachment bounds and the quotient forest](quotient_forests.md). This section does not claim it, nor does it replace true bounded holes by arbitrary full `Z_j` components.

## 8. Conclusion for the C-05 proof

The marking route gives a rigorous and useful reduction of the current-side bottleneck. It establishes a dimension-free pointwise positive coefficient majorant for the actual linear source stage, shows how the same resummed coefficients inherit the age bound, and carries that majorant through the canonical positive integration and both connected expansions without moving any self mass.

## 9. Source correction: the ordinary boundary owner is a birth halo

On CMP119 p.261, the support clause immediately below (2.41) is

\[
 X\cap\Omega_b\ne\varnothing,
 \qquad X\cap Z_b^{\sim}\ne\varnothing,
\tag{M11}
\]

not necessarily `X intersection Z_b != empty`. The actual large-field core behind a reconstructed old boundary term is still external to the attempted component after history deletion, but its displayed support may meet only that core's birth-scale halo. An ordinary boundary owner's grade must therefore be checked with the buffer geometry, rather than assigned from nesting alone. CMP119 p.265 begins the next ordinary step by taking a compatible cover of `Z_b` and adding four new-scale layers before any further exclusions. This is the relevant protection for the birth halo. Genuine completed-core ports, chosen inside `H_m subset Z_m`, retain their previous direct grade statement.

This correction does not change the phase-lifting proof. It does affect any application that had inferred a literal core intersection from (2.41).

## 10. Every genuinely integrated field coordinate has a deep source support

Fix one attempted pre-R component `H`, and put `h=k-N`. The fields integrated by its literal completed operation can be read from the source rather than inferred from the final decorated carrier:

* LFR I (1.81), p.195, defines `B_0=B''_k intersection Lambda_0`, with `Lambda_0 subset Lambda`.
* LFR I (1.72), p.192, leaves preliminary variables on the nested `Z''_(j+1) subset Z''_k subset Lambda`.
* The unchanged deep `T_h` and `V_h` pieces on p.194 are supported in the deep `Z_h` region, contained in `Lambda`, with the fixed endpoint collars.
* The new coarse integration introduced on pp.193–194 and written in (1.100), p.201, is on `Lambda`.

The retained final raw `V_k` data on `H` are parameters, not additional hidden coordinates to be placed in this list. LFR II p.392 expressly distinguishes the remaining raw multiplier from integrations at later ordinary steps.

All earlier geometric sets `Z_j`, `j<k`, lie in the pre-R `Omega_k^c`. The ordinary construction gives a gap of at least `2MR_k` between this inner set and the boundary of `H=Lambda_k^c`; see CMP119 p.256 and (3.20), p.269. LFR I (1.73), p.192, constructs `Lambda` by a fixed number of current `M`-layers around an earlier inner set. Hence, after including fixed averaging, bond and local-operator collars, there is an inner set `K_H` with

\[
 \operatorname{dist}(K_H,H^c)\ge cMR_k
\tag{M12}
\]

that contains the genuine remaining field coordinates and all varying older determining/history geometry. The lower cutoff on `R_k` absorbs those fixed collars. The support of the recent fixed cutoff `Lambda_k=H^c` is a separate issue: changing it to the reconstructed cutoff changes a deterministic region across all `H`, not merely `K_H`.

The general `K_H` needed for geometry can have diameter `O(MR_k)`. Only the smaller `Lambda_H` is guaranteed to lie in the source's `100M` cube. Therefore a component-root count over general `K_H` must allow a polynomial `O(R_k^4)` factor; it must not be replaced by a fixed `100^4` factor.

### 10.1 What the early Wilson collar does not establish

LFR II p.360, after (1.17), has an explicit `exp[-delta MR_k/2]` guard from the support of `zeta_0` to the outer boundary. That is a genuine source estimate. It does not by itself identify the precise thickness of the `H^~` used at the final self resummation on p.377. The tilde is locally redefined for localization boxes on p.372, and sufficiently thick enlargements of different components could overlap. The deep support (M12) is the safer endpoint for the incidence argument; no thick final self halo is assumed here.

## 11. Geometry dependence: a local-record proof, not an inference from (2.41)

The explicit `{S_i intersection X}` in (2.41) is not enough by itself to prove that a scalar coefficient is local in every `Omega_i,Lambda_i`. CMP119 pp.257–259 says that some of this dependence is suppressed in the notation. The additional information is in the actual source construction.

### 11.1 Exact localized operator records

CMP99 pp.408–409 constructs each local propagator from a sequence `Omega_n(square)` determined by the original geometry in the local enlarged block; the constructed support lies in `square^5`. Its generalized random-walk factors are products of these local operators and local cutoffs. Pages 412–413 describe the records `R_a(X)` explicitly. Corollary 3.8, p.410, and the subsequent generalized versions identify their field localization.

CMP99 Theorem 3.14, pp.426–427, proves the corresponding domain-change estimate by cancellation: common localized walks cancel, while every surviving difference walk reaches a region where the determining geometries differ. Its printed coincidence region is `Omega_k intersection Omega'_k`. One must not silently replace that region in the theorem statement. For the actual mixed-grade histories, use the same proof at the local-block level: wherever the full determining geometries agree on every dependency collar, the local blocks, cutoff functions and walk labels are identical. Pair those records there. Any unpaired or changed record has a local block meeting the enlarged disagreement region. The exponential walk bounds, including (3.108), retain the connection to that block.

CMP119 pp.276–278 constructs its scalar coefficients from precisely these localized walks, local integrals and connected unions. CMP116 (2.8)–(2.13), pp.13–15, likewise retains the localized input supports before taking the connected sum. Thus the common-record cancellation extends through a scalar product or connected cluster: if every input record and every local integration block has the same data, the resulting record is identical. If a product differs, mark its first changed factor in the elementary telescoping product identity. A record uses a completed historical kernel only together with its actual component footprint; the kernel cannot be assigned a hidden geometric dependence at a remote unsupported location.

This proves the structural rule for the actual constructed record catalog: after including its genuine local-operator and component footprints, a record whose dependency support misses the disagreement region is the same on both histories. This is stronger than field locality, but it is justified by the construction above. It is not an assumption about every arbitrary history-indexed function satisfying the scalar inequality (2.42).

For old births `b<k`, the changed source sets through birth `b` are in the deep region from (M12). Inherited completed-core footprints inside the current attempt also lie there by eligibility and nesting. Thus their structural differences carry a real deep endpoint. For current-born and preparatory coefficients, the change of `Lambda_k` across all `H` prevents assigning this conclusion blindly. Any outside-`K_H` reference term independent of all hidden coordinates and internal histories is an external scalar term, not an interaction with the current normalized slot. Its ordinary/full-tree or prefix budget must be kept separately.

### 11.2 Exact elimination of a purely declared incidence

Write the physical operation before normalization as a sum over actual internal histories,

\[
 T_H F=\sum_{\theta_H}\int F\,dM_{H,\theta_H}.
\]

If `F` is independent both of the field coordinates and of `theta_H`, then, for **each** fixed internal history,

\[
 \int F\,dM_{H,\theta_H}
       =F\int1\,dM_{H,\theta_H}.
\]

Summing the exact identity and dividing by the original `tau_H=T_H1` gives `Pi_H F=F`. Neither the canonical reference nor its mass has changed. This is the precise algebra behind the normalization observation on LFR II p.391. It remains valid on the native complex chart.

Independence of only the continuous field coordinates is insufficient: a function of the internal history is still averaged by `Pi_H`. Nor does a mere declared support enlargement prove independence. The local-record argument above is what allows an incidence inserted solely by deterministic saturation to be removed. A coefficient's external dependence on retained raw fields is also distinct from a dependence on an integrated slot.

## 12. The actual reference split and its permitted field leg

For a matched old/new record use the exact algebra

\[
 E_{\rm old}(\Phi_\omega)-E_{\rm new}(U_{\rm new})
 =\bigl[E_{\rm old}(\Phi_\omega)-E_{\rm old}(U_{\rm new})\bigr]
  +\bigl[E_{\rm old}(U_{\rm new})-E_{\rm new}(U_{\rm new})\bigr].
\tag{M13}
\]

The second bracket is treated by the local-history record comparison, with the current-cutoff qualification just stated. The first bracket must use an actual admitted source family. A straight or geodesic interpolation through arbitrary large-field raw variables is not justified.

There is a useful exact two-case implementation.

1. If the incoming primitive dependency collar `X^+` meets `K_H`, that is already a genuine deep endpoint. Use the native value bounds; no new hidden-coordinate derivative is required to create the endpoint.
2. If `X^+` misses `K_H`, it misses `Lambda` and the deep splice region as well. The identities (1.51), (1.54), (1.57), (1.58) are then valid on `X^+` as the exterior reconstruction around the new background. In (1.54), `U_(1,2)=U_1` outside its deep splice piece. Formula (1.55) localizes the otherwise nonlocal current argument. The resulting response terms have source arguments in `Lambda_H` or its fixed deep boundary collar. Their nonempty localization domains have the actual deep endpoint. The admitted scalar family (1.65) and its established gauge/native conversion supply the estimates.

This restriction is important: the source first introduces that four-map reconstruction on `Z^c`, and its splice does not coincide globally with the new background inside the untouched deep region. The two-case argument uses the extension only where the source identities actually agree. It does not interpolate away unbounded hidden data.

Mark the complete balanced record in (M13), so that common reference pieces cancel before absolute values. The phase lift then applies to the resulting blocks. For an old exterior component, retain its genuine core/dependency footprint in the record; its mere overlap with a newly added decorative halo is not a new deep endpoint or a new normalized slot.

### 12.1 What still must be assembled quantitatively

These source checks supply the relevant deep field supports, the local-history cancellation mechanism and the exact removal of spurious operator incidences. To complete the weaker graph proof, the refined pregraph must retain these actual reconstruction/history legs at every join which previously occurred only through an artificially saturated current component. The positive exponent must dominate the charged current physical length of that graph. The scalar (1.66) by itself does not pay an arbitrary extra physical join across such a component.

Once a genuine nonself graph visits `K_H` and has an actual terminal outside `H` for each used current component, disjoint guard annuli give a cost of order `R_k` per incidence, because no older zero-cost core lies in those annuli. Terms whose entire pre-completion dependency graph is confined to one self region are assigned to the original self action; decorative support alone cannot supply an exterior endpoint. The companion quotient note formalizes this geometry and the polynomial completion root count.

The remaining check is therefore concrete: verify that the source-preserving record refinement supplies those deep and exterior endpoints together with a positive length budget for every genuine nonself class, and keep the ordinary/current-born external sector under its accepted separate bounds. This note does not replace that check by the abstract graph lemma or by the phase identity.

## 13. The complete normalized historical kernel is local

The history-locality argument must include the entire completed operation, rather than just the primitive propagators occurring inside it. LFR II p.378 factorizes the defining integrations by components of the attempted region. Immediately after (1.71), p.379, the source states that all expressions defining the component operation are localized in that component; the self term has the displayed carrier `H^~`. The history sum is the actual component-restricted sum. Store the full defining kernel and self-action footprint, with its fixed native stencils, in the dependency record.

If two determining histories and their reference fields agree on this full footprint, their component integration catalogs, restrictions, domains and integrands agree. Consequently both `T_H` and `tau_H=T_H 1` agree. Since the canonical mass is nonzero on the source native chart by (1.74)–(1.75), the normalized operations `Pi_H=tau_H^(-1)T_H` agree as well. Products, local integrations and normally convergent connected sums preserve this exact equality. Normalization therefore introduces no remote geometry dependence.

This is an exact locality statement. By itself, a decorative footprint meeting a disagreement set would not be a paid graph connection. The following source geometry removes precisely that potential ambiguity for an exterior older kernel.

### 13.1 Exterior older kernel footprints remain exterior

Write `h_m` for the physical lattice spacing at birth `m`. LFR I p.177 explicitly describes the only possible downward jump of `R_m`: a factor `L` in a step. Hence

`h_m R_m <= h_(m+1) R_(m+1)`.

In particular, making `L` larger does **not** always shrink the physical old `MR` scale: a downward jump of `R` can cancel that scaling. The correct argument uses collar thickness, not the diameter of the whole old component.

The actual kernel footprint is the self carrier `H_m^~`, together with fixed local stencils. Under either possible tilde convention discussed above, its added layer has thickness at most `M R_m h_m`. A fixed number of `M h_m` stencils is smaller than another such layer once the common lower cutoff on `R` is chosen. Thus the whole footprint lies within two birth `MR` layers of its genuine core.

CMP119 pp.264–265 begins the next ordinary transformation with the compatible cover of `Z_m` and **four** layers of the next-scale `MR` cubes. Therefore the entire old kernel footprint lies in the next large-field component containing `H_m`. Nesting keeps this connected footprint in the current component containing that core. If the old core is exterior to the presently attempted component `H`, its whole defining footprint is disjoint from `H`, and therefore from `K_H`. If the old core lies in `H`, eligibility and nesting put the genuine core in the deep region.

This proves that a changed inherited completed kernel cannot obtain a fake deep endpoint solely from an exterior decorative halo. It also avoids expanding a normalized-kernel difference and introducing a new absolute sum over old internal histories. The self action and mass remain the literal source ones.

## 14. Native canonical normalization is a source input, not the desired current estimate

The uniform bound (1.75) is proved in the native chart by the source's first-order complex correction `sigma` to the positive real component density. LFR II p.379 explicitly includes boundary terms from all previous renormalization steps in this correction. The proof controls their first-order response by its connection to the indicated fluctuation/current data set.

CMP119 p.262 permits the whole-current-large-field relative scalar invariant and states that the renormalization transformation maps the full admitted input class to the next one. LFR II p.392 then expressly states that the final alternative representation (1.104) may be used inductively, and that the preceding considerations give the proof of Theorem 1. At the declared source-dependent scope, this is an imported uniform native estimate for the literal repeated alternative algorithm. It is not a consequence of the new selectively free-core graph norm, and it must not be inferred from the current Hessian estimate being proved.

Thus the canonical bound may be used before the new graph estimate, provided the proof keeps the literal source self action, completed operation and mass. A redefinition that moves arbitrary scalar terms into the self measure would require a new `sigma` proof and would not be licensed by this import. The auxiliary activity marking in this note is used on nonself coefficients only; it does not phase-deform the physical self measure.

## 15. Fixed-rate quotient induction

It is not valid to split the entire old decay exponent into fixed fractions at every completed operation. That would drive the maintained rate to zero with the number of repetitions. The maintained graph cost must instead satisfy the coefficient-one inequality

\[
 \ell_k(G_{\rm out})
 \le \sum_{a}L^{-(k-b_a)}\ell_{b_a}(G_a)
       +\ell_k(G_{\rm new}),
\tag{M14}
\]

where the `G_a` are old actual quotient connectors, the new pieces are actual paid localizer or reconstruction/history legs, and only genuine completed cores are zero-cost sets. Old costs are converted to current physical units. Declaring the new current cores free can only lower the output cost. Connections through a shared genuine core cost zero. Neither step costs a constant greater than one on the old lengths. Unions in the two connected expansions preserve this subadditivity.

For old inputs with `b_a<k`, the coarsening factor supplies the source reserve: `L^(k-b_a)>=L`. With the source's fixed choice of `beta` and sufficiently large admitted `L`, the input factor `(1-beta)kappa` can supply the full output invariant rate and a fixed age reserve, as in LFR II (1.66)–(1.67). Fresh same-scale ordinary terms have the improved `(1+4 beta)kappa` rate explicitly stated on CMP119 p.262. New localizer rates are chosen once to pay their entropy, actual incidence guards and the new output edges.

Any later conversion from quotient diameter to physical current diameter uses a weaker fixed **analysis** rate, taken once from the stronger maintained norm. It is not performed anew inside the inductive map. A numerical closed-ball recurrence cannot repair a geometric estimate with a multiplying constant on every old rate.

### 15.1 The intervening ordinary transformation has two old-input classes

CMP119 p.262 says that carried expressions with `j<k` retain their prior properties and labels. These must not be assigned the improved same-scale rate merely by relabeling them.

The ordinary transformation also creates boundary descendants containing old boundary inputs. CMP119 pp.270–271, (3.26)–(3.27), introduces the boundary parameter `t` into the complete normalized fluctuation integral. Pages 276–277 apply the localization formulas to those old boundary inputs and gain an additional factor `O(epsilon_k)`. Such a descendant is not automatically a full-tree forcing term when its input is a completed relative scalar. Its actual old input mark and quotient connector must remain in the positive ordinary cluster calculation. The scale change supplies the reserve in (M14), while the new ordinary localizer pieces remain fully paid. Source terms with no completed input are the separate ordinary full-tree forcing.

This distinction remains necessary even if the resulting descendant is finally grouped into a new current-born scalar family. Its construction estimate must retain the inherited connector before that grouping.

## 16. A stronger deterministic norm is available if the actual graph ledger is established

The phase argument is a useful way of converting a uniform signed scalar estimate into a pointwise positive sum. It is not an obstruction to proving a stronger norm directly.

Suppose the exact refined nonself records have deterministic, whole-native-domain bounds `q_a`, with their actual support/incidence/quotient geometry, and satisfy a rooted sum bound for `sum_a w_a q_a`. Then one may maintain

\[
 \sum_a w_a\,\|F_a\|_{\mathcal D}
\tag{M15}
\]

directly. Source localization Cauchy estimates use the full admitted domain of the incoming scalar. Perform the exact old/new reference cancellation before taking absolute values; a nonzero structural difference either has a genuine deep dependency point or resident core, while an exterior kernel's full footprint is excluded by Section 13.1. A bound by twice the old scalar norm then retains its existing connector without reopening its old internal history expansion.

The physical canonical integration has the uniform native operator bound from Section 14. Exponentials, products and the ordinary rooted forest inequalities act on the nonnegative majorants in (M15), so their uniform-domain versions pass through both completed expansions. Independent phase variables and a later interchange of pointwise suprema are unnecessary on this stronger route.

The remaining substantive input is still the actual source graph ledger: every newly used slot must have a paid deep-to-exterior connection, all joins must obey (M14), and ordinary old-input descendants must be included as in Section 15.1. Stating a Banach norm does not establish those source facts. Once they are verified, however, there is no separate positive-coefficient or `sum of suprema` barrier.

## 17. Paid joins for the nonempty source localizers

The source's retained distance factor in (1.66) refers to the first nonempty localizer, so it must not be silently used as a separate distance for every connected localization component. There is nevertheless a direct payment for the missing joins.

For every connected component `W` of a nonempty `Y'_i`, retain its actual contact with the preceding determining boundary and its actual `Lambda` endpoint, as specified on LFR II pp.373–374. If the contact belongs to an already paid old or new graph piece, join there with a bounded current-cell adjustment. If it belongs only to a whole attempted component artificially inserted in `Y_1`, then `W` connects a deep `Lambda` component to that determining boundary. It therefore has at least `cR_k` current cells along a path. This remains true when its deep component and the artificially inserted contact component differ: it must first exit the former's guard.

The inserted contact component has diameter at most `100 M R_k`. Connect the contact through that component to the actual old carrier/core contact which caused it to be included in `Y_1`. This new physical path has length at most `C M R_k`, and hence at most `C' M |W|/M^4`. A fixed share of the **new** `kappa_1` volume exponent pays it. Retain separate shares for the deep guard, the ordinary localization entropy and the final output rate. No old connector is multiplied by a constant. Later localizers attach to previous actual pieces or to the same initial inserted components, so this construction applies successively.

This is the concrete amendment needed to infer a paid connected pregraph from (1.66). The current components are not declared free until the output quotient is formed. The argument does not manufacture a first-distance factor for every derivative or every map port.

### 17.1 One real guard can control all current contacts

There is a useful weakening of the earlier one-deep-endpoint-per-slot condition. Assume the actual quotient graph has one genuine deep-to-exterior connection, so its paid length is at least `cR_k`. Traverse a spanning tree twice and cut the paid traversal into pieces of length at most `R_k`. The CR.1 relative-component diameter lemma puts each such piece, including its traversed genuine old cores, inside a physical ball of radius `C M R_k`; the largest old core has diameter at most this scale. Decorations are in the same ball after a fixed enlargement.

Each such ball meets only a bounded number of the disjoint eligible current components. These are rectangles with every side at least `20MR_k` and with diameter at most a fixed multiple of `MR_k`; the lower side bound follows from the ten-layer growth in LFR I p.177. Comparing volumes after enlarging the ball gives a bound independent of history and depth. Hence the number `q` of current contacts satisfies

`q <= C(1+ell_k/R_k)`.

The one real guard removes the additive constant and yields `ell_k>=c' R_k q`. Thus a shallow `Y_1` contact does not require an independently constructed deep derivative leg. The proof still requires an actual graph contact, up to the fixed decoration neighborhood, and a genuine nonself endpoint. A self graph is never promoted to a nonself graph solely by a decorative enlargement.

## 18. Ordinary attachments: separate connector-paid sites from protected footprints

A concrete false shortcut is to charge the old-owner collar once for every ordinary-T attachment. An old carrier can already extend into the current integration region. Many new local ordinary terms may attach at those sites with only the source `O(g_k P_k)` factor. A single old-owner path cannot be counted repeatedly to assign `exp[-cR_k]` to each attachment.

The correct dichotomy is as follows.

**Connector-paid sites.** Every old free core lies in the inner old large-field set. The new ordinary construction surrounds that set by the fixed several-layer `MR_k` buffer. At sites separated by at least a fixed current-cell distance from these free cores, a graph visiting `N` separated current cells pays at least `c(N-1)` in length. To see this, take disjoint small balls around a separated subfamily of the visited cells. There is no free core in these balls; except for one possible root, each visit requires a fixed positive paid graph length. Consequently the number of such attachment cells is bounded by `C(ell_k+1)`.

The source ordinary forest/localizer sum at these sites may give `exp[C g_k P_k N]`. Its length-dependent part is paid by the fixed coarsening reserve `(L-1)lambda ell_k`, with the coupling ceiling chosen after all constants. CMP116 pp.20–21, (2.38)–(2.41), uses exactly the analogous length reserve to pay the local exponential factor generated by cluster attachments. CMP119 pp.277–278, (3.44)–(3.47), makes the normalized expectation expansion explicit: the denominator response is the connected cluster sum touching the distinguished numerator carrier. It must be included; no global, volume-independent Gaussian operator norm is assumed.

**Protected footprints.** A new ordinary localizer rooted at an old free-core footprint must connect to the actual ordinary integration region. The four-layer inclusion in Section 13.1 gives a real collar for this connection. Its native reconstruction row or its full new localization-domain volume supplies `exp[-cR_k]`, with the fixed allowed inverse-coupling and logarithmic prefactors. The number of possible current attachment cells contributes a fixed polynomial in `R_k`, not a count of microscopic historical tags.

The zero-attachment branch is kept exactly as the old scalar composed with the admitted source map, so its norm factor is one. For a nonempty family whose new pieces attach at already exposed regular sites, retain **one** old-owner-to-regular-region guard after paying the length-dependent family factor. This guard is genuine: a resident old owner is deep in the attempted component; an exterior old owner lies inside the ordinary-growth buffer of its own current large-field component, which the graph must leave to reach the changed cutoff or current integration region. All old zero-cost cores remain inside the inner set, so this annulus cannot be traversed for free.

Any remaining exponential loss proportional to noncoarsening counts is then of the form treated in `Summable reserves in the native norm`: its intensity has a superlogarithmic collar and is summable on the retained AF trajectory. A bare `O(g_k P_k)` loss on an unchanged old-tag count would not be covered. The summable reserve is not used to hide that loss; the connector-paid part is removed first.

These facts identify the source allocation required for the ordinary step's rooted forest estimate. The exact forest factors are those of (3.44)–(3.47), or their completed-component counterpart. An independent factorial must not be inserted simply to make a desired exponential sum converge.

## 19. The supported current in (1.55) on the independent native-current family

The repair of `G'' J_(1,2)` in (1.55) uses a genuine criticality identity. It would be invalid to replace the current of its auxiliary minimizer by an arbitrary independent current and then use that identity.

The actual source construction does not make that replacement. A visual check of LFR II p.370, (1.52)–(1.53), shows that

`U_1 = U_(B_1)(mixed determining data)`

is a literal constrained minimizer for the joined set `B_1`. The field `J_1` in the following criticality argument is the action current computed from that constructed field. The native extension paragraph on p.375 begins by introducing the independent pair `(U,J)` into the **last** `H_k`, then substitutes the resulting configurations and their corresponding data into the earlier literal minima `U(B_k(Y_3),data)`, `U(B_1(Y_2),data)`, and the outer reconstructed minimum. The independent external current affects `U_1` indirectly through these data; it is not identified with `J_1`.

For every admitted complex value of those data, the analytic constrained minimizer satisfies its constrained Euler–Lagrange equations. Its computed current therefore annihilates the constrained tangent space. Together with the algebraic propagator identity `G'' Q^*=0`, this gives the supported expression (1.55) on the entire admitted independent-current family. This is an application of the variational equations for complex data, not analytic continuation from the lower-dimensional graph `J=J(U)`.

Apply the localization expansion to the **already rewritten supported right-hand side** of (1.55). There is no need to assert that an arbitrarily decoupled propagator `G''(s)` still gives the original unrepaired identity on every deformation.

The preceding argument proves the criticality step for the literal-minimum native family. It does **not** by itself identify that family's zero-forcing reference with an arbitrary off-minimum native field `U`. In particular the interior reconstruction (1.63) can contain a projection `U(B,M(U))`. The next paragraph states the separate source-compatible extension used for the reference cancellation.

### 19.1 Perform the exterior reference cancellation before choosing its extension

On the physical family use the exterior four-response telescope (1.51), (1.54), (1.57), (1.58), ending at the actual new background `U_k`. Pair its exact old/new reference terms there. Then extend the supported response differences by the exterior construction on pp.372–373, retaining `F_new(U,J)` as the reference. CMP116 (1.16)–(1.18) gives `H(s;0)=0` uniformly on its independent `(U,J)` domain. In the response extension use the already rewritten supported right-hand side of (1.55) as its formal argument; its equality to the unrepaired expression is needed on the physical family, while its support, analyticity and absolute bounds hold on the whole chosen chart.

This gives a zero-forcing reference equal to `F_new(U,J)`, without adding a hidden residual `F_new(U(B,M(U)))-F_new(U)`. It is not an assertion that the exterior response extension is identical off the physical family to the interior projection extension in (1.63)–(1.65). The distinction is allowed by the explicit compatible-extension convention following AB17.6: the physical current jets come from the exact real density, and native jets refer to the specified admitted analytic extension, with the physical identity valid for the entire real current family.

When the full dependency support misses `K_H`, these exterior identities apply on that support because all mixed determining data and the splice discrepancy are deep; the support need not miss all of `Z`. The localizer proof excludes the actual old support and deep forcing set, and the uniform propagator estimate CMP116 (1.11) remains valid after increasing this excluded set. The same fixed strong core and full printed localization disks admit this exterior family. Historical coefficients and complete normalized kernels coincide on the common reference by Section 13. A record meeting the deep set uses its old norm and genuine connector instead.

The canonical self operation retains its literal source native extension. Only the nonself response catalog is organized by this exterior telescope. No mass or self coefficient has been redefined.

## 20. Prefix operations must retain inherited completed inputs

The coefficients `C_r^(i)` in LFR I (1.61)–(1.70) are not all pure full-tree forcing after earlier alternative completions. The source formula (1.60) has the old action as an input, so some of these coefficients are descendants of completed relative scalars. Keep those input records and their physical connectors through the entire preparation. Only the terms with no completed input belong to the independent full-tree forcing bank.

The source also provides an important quantitative restriction on accumulation. Pages 189–192 retain the old action composed with the new background, and add the separate `C_r^(i)` terms. The modified analytic spaces are descending, with the mapping inclusion stated on p.191. Thus unchanged composition has norm factor one. The lower preparation strips are disjoint. The cumulative overlap discussed explicitly on pp.191–192 occurs only in the top `N_0` layers, and is paid there by the fluctuation factor `g_j`, more precisely by `N_0 delta'_j`; `N_0=O(log R_r)`. There is no source factor `C^{N_r}` and no iterated fractional power of the old input norm.

For the strengthened norm, the inherited-input part must use the attachment dichotomy of Section 18: protected-core responses retain their genuine collar or grade-distance row; attachments to exposed paid graph portions use the physical connector reserve, with the actual strip overlap included. The original resident completed cores have births at most `h=r-N_r` and remain in the unchanged deep piece. Exterior younger scalar families retain their exterior owners and connectors. A remaining loss proportional to a noncoarsening old-tag count must still have a summable superlogarithmic factor. The source's bare `N_0 g_j P_j` bound is not itself such a factor.

This is the exact prefix allocation required in the all-history positive theorem. It prevents both misclassifying inherited prefix descendants as new full-tree forcing and paying a constant once per preliminary integration.

## 21. The interacting conditional prefix: a phase estimate with its actual source scope

This section replaces a fixed-real-reference argument for a whole prefix, which is not valid in that generality. Two restrictions are essential: normalize only through the last directly integrated old slot, conditional on the later variables; and include the ordinary interaction in the positive conditional law. The norm of a pure Gaussian conditional law would not control an arbitrary bounded old-slot observable after multiplication by an ordinary interaction of size `B_0 poly(R_r,N_r)`.

### 21.1 Exact ordinary and completed-input separation

At a fixed admitted history write the old action as its independently controlled full-tree ordinary part plus the completed/relative scalar input records. Put separate auxiliary marks on the latter records, including completed outputs with no completed ancestor. The mark-zero prefix partition is the **ordinary reference partition**. Thus a term conventionally called `C_r^(i)` belongs to the ordinary reference only if it has no completed-input mark; the whole actual `C_r^(i)` is not assigned the printed full-tree `C_0` estimate.

This separation is compatible with the literal action. CMP119 pp.270–271, (3.26)–(3.27), places the response to an old boundary term in the boundary sector. LFR I pp.188–189, (1.60)–(1.63), places every preparation contribution in the boundary sector because its integration is in the old large-field region. Setting completed-input marks to zero therefore does not change the bulk `E/R` subtraction scheme or the retained coupling trajectory. The general admitted-input formulation stated on CMP119 p.262 applies to the mark-zero full-tree input. Its constants may depend on the once-chosen analytic profiles but are constants, not additional powers of the running logarithm.

The identity used in an estimate is exactly

`Z_actual = Z_ord Pi_ord exp(V_relative)`,

with the already extracted reference scalars restored in their original action positions. The ordinary mass `Z_ord` remains in the ordinary forcing logarithm. The Taylor/Mayer expansion of the last factor restores every completed-input contribution, including the normalization response. This is an auxiliary prefix factorization only. It changes neither a canonical completed operation `T'_H`, nor its self term, nor its physical mass `tau_H`.

For several attempted components the factorization is made before normalization. A record is absorbed in the ordinary law for `P` only if all its **actual integrated** raw-variable slots lie in `P`. A common independent native pair `(U,J)` is external and is harmless. An integrated `A/B/V` variable of another component is not external. Cross-component Gaussian blocks, ordinary boundary terms, and reconstruction-map response records remain interactions. Their dependency carrier reaches the deep integrated support and leaves `P`, hence has the ordinary full-tree or actual kernel guard. Terms independent of all integrated variables can be factored out exactly. They stay in the scalar action; their phase is irrelevant to the normalized functional.

This classification can be performed on the source localized records, or by real-reference centering of their finitely many actual component slots. The latter has only the fixed per-incidence centering factors already accounted for in Section 11. A geometric halo without a genuine variable dependence is not an extra slot.

### 21.2 The actual truncation and fixed support

Let `r` be the attempted outer scale, `h=r-N_r`, and let `F` have latest explicit old-slot creation label `b`. Suppose it has a direct dependence on a slot integrated during the preparation. Let `j_*` be the largest such old slot index. For an input present before the ordinary step at `r`,

`h <= j_* <= b-1 <= r-2`.

Keep every later variable, every deep `T_h` variable and every retained raw field fixed. Normalize jointly over the genuine free-coordinate pairs `(A_j,B_j)` through `j_*`, with their actual ordered dependence. Do not replace this conditional law by a product of `N_r` separately bounded normalized laws. A fixed endpoint convention can enlarge the recent band by a fixed number of grades; a newly created outer `A_(r-1)` is kept in its actual ordinary-T creation records rather than included in this deep arbitrary-test branch.

The support is fixed in these real free coordinates. CMP119 p.249 explains that the nonlinear constraint change and the exceptional-bond map `C` change only the excluded bonds; the cutoff on the remaining free bonds is unchanged. LFR I p.183, (1.27)–(1.29), completes the real fluctuation restrictions, and pp.187–189, (1.53)–(1.60), explicitly integrates the free `A_j` and `B_j` with these restrictions. The failed selector is first relocated as in (1.59), including its full action and Jacobian response; it is not differentiated as a moving characteristic function. Work on a fixed admitted history/selector branch. No assertion of holomorphy across a changing discrete selector is made.

At each `j`, the coordinates are counted in their own `j`-grid. The eligibility definition on LFR I p.177 requires the preceding regions inside the attempted component to satisfy the `100 M R_j` condition at their corresponding scales; the source immediately states the resulting rectangular-chain property. Its notation thereafter uses `Z_j` for the intersection with the chosen attempted component. The explicit use of this condition on p.192, (1.73), bounds the terminal rectangle `Lambda` by a `100 M` cube. Consequently the actual strip at level `j` has at most

`D_j <= C (L M R_(j+1))^4`

free coordinates, including fixed bond and Lie-algebra multiplicities. This is the source eligible chain, not a weakened condition permitting arbitrarily many untracked ancestors inside the component. No whole coarse component is subdivided into `L^{4(r-j)}` independent old atoms. The proper-scale row measures are retained before this coordinate count is used.

For clarity, the geometry input is the retained C01 **bounded nested rectangular history per attempted component**. LFR I p.195 explicitly says that the gauge construction makes essential use of the single nested sequence `Lambda superset Z''_r superset ... superset Z''_(h+1) superset (Omega'_(h+1))^c` consisting of rectangles. Page 179's statement about rectangular components alone would not bound the total number of unrelated ancestors. Reading condition (ii) merely as a bound on each of arbitrarily many separated ancestors would be insufficient for the estimate above and would not supply the stated p.195 construction. No such weakened replacement for the source history class is used here.

The source permits `N_r` to be a fixed power of `ell_r` after (1.94), p.198. Throughout this finite window the retained AF comparison makes the running profiles comparable up to fixed logarithmic powers. Thus `sum_(j=h)^(j_*) D_j P_j^d` is a fixed logarithmic polynomial for every fixed cutoff power `d`. The exponent is chosen before any extra analytic-radius exponent.

### 21.3 All density terms, and no fixed-real-center comparison

After the exact coordinate changes, write the conditional ordinary density on this fixed positive real measure as

`w_xi(a)=c(xi) 1_S(a) exp[-q_xi(a)+v_explicit,xi(a)+v_ord,xi(a)]`.

Here `a` is the full vector of the actual partial-prefix free coordinates. The quadratic `q` includes every actual old Gaussian precision, its principal/Schur block, linear force and quadratic cross term retained by the source. An order-one real cross term is not moved into a supposedly small remainder. The background-current correction in `C_j^* Delta^(j) C_j` is included. If a quadratic block connects different attempted components it is one of the marked cross interactions of Section 21.1.

The explicit term includes the nonlinear constraint/Haar/coarea factors and the true higher-order Wilson remainder. Every factor depending on `a` is retained. An `a`-independent determinant or coarea factor may be put in `c(xi)` because it cancels from the normalized functional; its logarithm remains in the exact action. If it depends on an earlier integrated coordinate, it is estimated by its actual local log/trace expansion. The branch of each such logarithm is the one real on its positive real small-field density.

The native coefficient row estimates in CMP99, including its principal covariance theorem, and their explicit free-coordinate identification in OR17.8–OR17.10 apply to these exact precisions. Cauchy on that fixed absolute coefficient domain gives, in the actual normalized row convention,

`sup_x sum_y |Im K_j(x,y)| <= C alpha_r^+ poly(ell_r)`.

Accordingly the quadratic phase is bounded by `C sum_j D_j P_j^2 alpha_r^+ poly(ell_r)`. The same local coefficient/trace count treats the genuine coarea factors. One must not use a bound for the entries of an unweighted fine kernel and then count fine bonds a second time. The row here is already the source row with its native measure.

The unrenormalized `g_j^(-2)` Wilson action is not estimated by a crude running-chart supremum. Its actual linear/quadratic decomposition is made first, exactly as in CMP119 pp.249–250 and CMP116 pp.10–11, (1.37)–(1.43). The remaining constrained Taylor term has its explicit `g_j` times a cutoff polynomial bound. The coupling-difference terms use their source expansion and localized coefficient, as on CMP119 p.277; their large coefficient is accompanied by the reconstruction decay or by the explicit powers of the fluctuation. This prevents an artificial loss growing with the chosen extra analytic exponent. The real parts of all these terms can be left unestimated for the normalization argument.

For the ordinary scalar part, use three profiles as in the companion `Complex radius reserve for the phase cone`: the target jet profile `alpha^-`, the completed-activity value profile `alpha^+`, and an independently chosen larger ordinary-source profile `alpha^{++}=ell^{Q_phase} alpha^+`. Only the original full-tree ordinary family is needed at `++`. There is no requirement to prove the unknown completed family on a fourth chart.

The source bounds used here are explicit:

* The actual regular `E` bank has the **running** chart in CMP119 (2.27)–(2.28); (2.27) imports the value bound (1.1.18), not the fixed absolute chart of the earlier small-field paper. Use its already renormalized fluctuation family, localized by CMP116 Lemma 1, (1.33)–(1.36), and transferred to the actual mixed history on CMP119 pp.275–277, on the independently chosen ordinary `++` profile. The own Wilson subtraction and the sum over earlier `E` grades are performed inside that family. Section 29 below records the source scope and radius count. An extensive unrenormalized `E` action is never used as its substitute.
* `R` has the arbitrarily high coupling power in CMP119 p.260, (2.31), with its actual renormalized fluctuation difference treated as stated on p.276.
* The ordinary `B` coefficients have `B_0 exp[-kappa d_b(X)]` on their declared running chart, CMP119 (2.42). The mark-zero pure-prefix coefficients have `C_0 exp[-(1+3 beta) kappa d_m(X)]`, LFR I p.192, (1.70).

Raising the two ordinary profile exponents by a fixed `Q_phase` changes the once-chosen constants and coupling ceiling. It does not replace `B_0` or `C_0` by `ell^{a Q_phase}`: the displayed source estimates are uniform constants for the selected exponents. CMP119 (2.28) permits fixed integer exponents greater than one. The real choice of `N_r` in LFR I (1.94) depends on the real cutoff exponents and is made first.

The AF comparison in this finite window must also be used sharply enough to avoid an artificial circular exponent. Put `t_j=g_j^(-2)`. The retained two-sided AF envelope gives `c<=t_j/t_r<=C+O(N_r/t_r)` for `r-N_r<=j<=r`, with fixed `c,C>0`. Since `N_r` is a fixed power of `ell_r=log t_r`, it follows that `ell_j/ell_r=1+O(1/ell_r)`. For each fixed chosen exponent, including `q+Q+Q_phase`, this ratio raised to that exponent is bounded by two after decreasing the common ceiling. A crude global estimate by `(1+|j-r|)^(q+Q+Q_phase)` is unnecessary here and would introduce a spurious `ell^{p_N Q_phase}` loss. The polynomial exponent paid by `Q_phase` is therefore fixed before `Q_phase` is selected.

At a real native pair and real integrated variables these ordinary coefficients are real. This is also true for the specified independent-current extension: the propagator/constraint formulas, real Taylor operations, real integrals, inclusion–exclusion and the logarithm branch at a positive real density commute with the real conjugation. An arbitrary holomorphic extension agreeing only on the physical submanifold would not justify this assertion; the assertion is for these literal source-formula extensions. Only real compact gauge transformations are used when comparing with the real chart; they preserve the reality and bounds of the fixed adjoint coordinates.

The modified prefix spaces and their successive insertion inclusion are given on LFR I pp.190–192, (1.64)–(1.69). The multipliers `L_0^{O(N_0)}` are polynomial in `R_r`, as proved immediately after (1.70). The cleanest phase argument applies Cauchy to the **full composed local coefficient** `G_gamma(xi;a)` at real localization parameters, with all real integration coordinates `a` fixed. The source insertion theorem and PF.1 admit this composed function on the external strong `++` ball and give the corresponding `B_0/C_0` local bound there. It is real at a real external input `xi_0`. The external `+` input is within `poly(ell_r) alpha_j^+` of that real input, with a fixed `++` affine margin, so one-variable Cauchy in this external variable gives the phase gain `C poly(ell_r) ell_r^(-Q_phase)`.

This formulation does not infer a strong affine norm for an arbitrary modified-output `A'` from only the weaker clauses of its source chart. It uses the genuine external strong core, the exact composed source family and its independent/reconstructed-current admission. The later estimate of the remote localization change extends the result to the full complex localization disks. No interpolation through a new raw large-field complex domain is introduced.

There is a polynomial bound for the required local sum. An ordinary `B` term with an explicit `A_j` slot has birth at least `j+1`. For the direct prefix branch its relevant births are in the finite window through `r`. Assign it to one genuine integrated endpoint; at each birth the rooted full-tree sum is bounded by a constant times `B_0`, and there are at most `N_r` birth labels. A pure-prefix term has the actual pair of integration/localization labels from (1.63), costing at most `N_r^2`, and the same rooted full-tree sum. Summing the native counts `D_j` gives the announced polynomial bound. Terms older than the window have no direct slot being integrated; their background response is the separately guarded map/attachment response, with its true old grading. They are not counted by a fabricated polynomial coarse volume or absorbed into this ordinary base. Regular `E/R` use their already localized fluctuation differences just cited.

Combining these bounds gives constants `D_1,D_2,D_3,u,c>0`, fixed independently of the cutoff and of the old observable, such that the oscillating phase of the included ordinary law is bounded by

`eta_r <= C g_r ell_r^(D_1) + C ell_r^(D_2-Q_phase)`

`          + C g_r^(-u) ell_r^(D_3) exp[-c R_r]`.       (M16)

Choose `Q_phase>D_2+2`, and then the one common small coupling ceiling so that `eta_r<pi/3`. An `a`-independent phase is harmless. No comparison with one fixed real-center density is asserted: the pointwise comparison is the positive measure `|w_xi(a)| da`.

### 21.4 Which localization disks are covered

The last term of (M16) is a separate localization estimate. The truncated directly integrated region lies in `Z_b subset Z_(r-1)`, hence is deep in the attempted component `P`. Take the source localization family outside the **whole** `P`. Every changed coefficient row rooted in this region then has a genuine source path to `P^c`. The localized covariance, constraint, reconstruction and coarea expansions retain a fixed positive part of this path on the full printed complex disks. Ordinary interaction records reaching outside `P` have their own full source tree from the integrated endpoint; they are either marked cross interactions or have the same bound. Terms with no integrated endpoint cancel from normalization.

This proves the superlogarithmic term in (M16), with the finite native strip/stage count and any fixed inverse-coupling normalization cost displayed in its prefactor. It is not a claim about arbitrary complex decouplings inside `P`. Such a decoupling can have order-one phase even at zero complex background. It is also not a claim about a blanket full prefix containing the top `B_(r-1)` near the boundary of `P`. The conditional last-slot truncation is essential.

### 21.5 The resulting operator bound and higher-slot creation

For every point of this admitted contour, let `tau_xi=int w_xi`. The phase-cone inequality gives

`|tau_xi| >= cos(eta_r) int |w_xi|`,

`Pi_xi 1=1`,

`||Pi_xi||_(L-infinity -> C) <= sec(eta_r) <= 2`.         (M17)

The estimate holds for arbitrary bounded measurable dependence on the real old `A_j` variables. It uses no analytic old-`A_j` extension. Fixed support, the source holomorphy and local domination give holomorphy of the unnormalized integral, and (M17) gives holomorphy after normalization. The bound is for one joint conditional law per attempted component, not a factor `2^{N_r}`. Later stages, after the last direct old slot is eliminated, are handled by their native map records and fixed-old-slot Taylor argument.

Tilting by ordinary interactions can introduce a higher external old slot which was absent from `F`. Do not claim the pure-Gaussian no-new-slot property for this tilted law. Split the ordinary interaction into its value with those higher slots frozen at a real admitted reference plus the difference `V_hi`. Only terms genuinely depending on the integrated variables need be retained in `V_hi`. For an ordinary `B^beta` term containing an integrated `A_j` and a higher `A_l`, one has `beta>=l+1` and `j<=l-1`, up to the fixed endpoint convention. The integrated endpoint is in `Z_(beta-1)`, whereas the carrier also meets `Omega_beta`; the ordinary buffer at its own grade gives `exp[-c R_beta]`. For a pure prefix `C_m` term, (1.63) places its carrier in `Omega_(m+1)^c` and meeting `Omega_m`. A genuine `A_l` slot forces `m>=l+1`, apart from the same fixed endpoint convention. The same own-grade buffer applies. The recent-window profile comparison and true rooted counts therefore give

`||V_hi||_(positive rooted) <= C poly(ell_r) exp[-c'R_r]`.

The phase argument also applies to the real tilt `V_lo+t V_hi`, `0<=t<=1`. The exact identity

`Pi_1 F-Pi_0 F = int_0^1 [Pi_t(F V_hi)-Pi_t(F) Pi_t(V_hi)] dt`

includes the moving-mass derivative and bounds this response by `6 ||F|| ||V_hi||` under (M17). Thus a higher-slot creation is a new guarded response. A new already-small response can take the outer creation label `r`; all its remaining explicit slots have grade below `r`. The unchanged `Pi 1` branch creates no slots. After a failed component at `r`, a later containing attempt has lower endpoint at least `r`, so that lineage does not suffer another unguarded direct-slot normalization. Disjoint-component couplings remain marked with their genuine crossing guard, rather than being hidden in an allegedly independent reference law.

The conclusion of this section is the **ordinary-tilted conditional operator estimate** on its stated contour. It is a source-matched replacement for a Gaussian-only estimate. The small rooted majorant for the completed interactions left outside it still comes from the actual graph/attachment argument; (M17) cannot substitute for that argument.

### 21.6 A larger excluded collar also permits a single whole-prefix operator

There is a useful stronger variant of the last-slot construction. Let `D(P)` be the attempted component together with one or two whole current `M R_r` layers. Exclude all cubes meeting `D(P)` from the **new** walk-localization variables. Every actual partial-prefix integration coordinate, including the top newly introduced `B_(r-1)`, lies in `P`, and consequently is at distance at least `c M R_r` from `D(P)^c`. The row perturbation caused by those localization variables therefore has the guarded bound used in (M16) for the whole successful prefix, conditional only on the variables not integrated by that prefix.

This enlargement is compatible with the source estimate, not a claim of uniformity for an arbitrary inside-component decoupling. In CMP116 p.5, (1.11), each walk is multiplied by the localization parameters of the chosen cubes which meet it. Removing parameters by increasing the excluded set can only reduce their number for that walk; the same absolute bound and full printed disks remain valid. The component-locality proof preceding (1.10) is unchanged with the connected initial domain `D(P)` in place of the small initial cube. New localization animals attach to this fixed domain with their usual source volume and distance weights.

The phase count remains `sum_j D_j P_j^d`: the actual eligible strips are integrated. The whole geometrical collar is not filled with newly invented fine integration variables. Its size at the current mesh is only polynomial in `R_r`; any finer walk-root count is summed with its actual distance to that collar before changing scale. The full composed native family is the source family on LFR I pp.190–192; its modified-chart tube has the same fixed `L_0^{O(N_0)}` polynomial already used in Section 21.3. Thus (M16)–(M17) apply to one whole-prefix ordinary-tilted operator on this enlarged-exclusion contour as well.

`D(P)` is only native dependency metadata. The actual bounded protected core is `P`. Overlap of two such collars does not create an integrated raw-variable edge, does not merge their kernels, and does not contract either collar for free. The factorization rule of Section 21.1 still precedes the estimate: actual cross-component raw slots and cross-component map records remain marked interactions. The original pure Gaussian operation already has this convention: CMP119 p.258 after (2.21) keeps only the within-component quadratic block in the operation and assigns the other quadratic terms to `B`.

The next ordinary four-layer enclosure contains this one- or two-layer collar, so the exterior-footprint exclusion proof continues to apply. A **new small response** may carry `P` and `D(P)` after its actual small coefficient has been established. An unchanged old scalar keeps its original birth and cores and factors out of `Pi 1`; it is not promoted to a large protected component. The ordinary normalization mass is still estimated in its independent full-tree source expansion and retains its exact action role. These conditions are why the enlarged-exclusion variant does not manufacture a spatial gain from a decorative collar.

The persistent free core `P` is declared only on a branch in which the whole original component is retained, such as a failed preparation or the final failed alternative. If the preparation succeeds and the main R operation subsequently removes `P`, this is only a temporary support/integration grouping. The source successful-component mass pays the full-tree restoration, including the interior-volume factor on LFR II p.389. A coefficient of size `exp(-cR_r)` alone is not used to pay `exp(CR_r^4)`.

Either variant is sufficient for the normalized arbitrary-old-slot estimate. The original exclusion of `P` alone requires the last-slot truncation of Section 21.2. The enlarged exclusion of `D(P)` permits the single whole-prefix norm and avoids multiplying stagewise constants. The higher-slot creation response and real-reference centering in Section 21.5 remain part of the algebra in both variants.

## 22. The correlated Gaussian step must precede the independent-slot forest estimate

Disjoint declared supports do not make the original Gaussian variables independent. The source first constructs connected Gaussian records, and only then has the factorization needed for the Mayer/forest algebra.

The precise source mechanism is CMP116 pp.12–16: (2.5) conditions on the actual fluctuation support `Z_0`; (2.6) uses the square root of the complementary covariance to introduce a product Gaussian; (2.8) localizes the precision, covariance and covariance-square-root operators. The connected-component factorization appears only in (2.10), followed by the hard-core polymer formula (2.11). Its complex estimate (2.16)–(2.17) includes the determinant and quadratic loss

`exp{ C [exp(-delta_0 M/3+16 kappa_1)+alpha_0+alpha_1] |Z_0| }`.

This cost cannot be omitted. CMP119 pp.277–278, (3.44)–(3.47), gives the corresponding **distinguished insertion** construction and exact denominator cancellation: the surviving ordinary clusters touch the numerator insertion.

For an inherited scalar under an ordinary T, apply the native Taylor expansion at its admitted zero-new-forcing reference before this Gaussian step. The coefficient `D^nu F(reference; old slots)` is independent of the new current Gaussian variable. Every nonconstant term applies that coefficient to explicit new map records `H_gamma(A)`. Thus the Gaussian insertion support is the union of the actual `A`-supports of these **new records**, together with any other new ordinary interactions being integrated. The old carrier and its free-core decorations remain external native coefficient support; they do not become Gaussian integration volume merely by being stored in the record.

The source Gaussian construction applies also to these bounded multilinear coefficients: retain them as Banach operators, integrate the tensors of new map records, and contract afterwards. If one old coefficient joins several disconnected new supports, keep that old occurrence as one hyperedge. It is not factorized incorrectly into separate scalar functions. The Gaussian connected records and their actual measure factorization are obtained first; the old hyperedge is retained in the subsequent incidence graph.

The Gaussian insertion volume has a necessary split. Some current integration cells can already lie on the exposed paid part of the old carrier, even for an empty external localizer. The ordinary integration region misses the old free cores and their protected inner footprints, so these cells are counted by `C(ell_current+1)` as in Section 18. All other insertion cells belong to the genuinely new localization pieces. Thus the required bound is

`|Z_0| <= C [ell_current+1+V_new]`.

The old-cell part of the determinant/quadratic loss is paid by the exact `L` coarsening reserve; the new part and its animal entropy are paid by a fixed share of the **new** localization-volume exponent. The coefficient `exp(-delta_0 M/3+16 kappa_1)` in the Gaussian comparison is small after the fixed source choices, but is not asserted to be summable over scales. It must not be charged at every step to an unchanged old tag count. No interior volume of an old free core is charged. The zero-new-map branch factors out of the normalized expectation exactly, with factor one.

This also explains why a current-born ordinary-T descendant must retain its actual map and Gaussian creation records through the subsequent R operation. Declaring it an arbitrary old scalar with an unexplained direct current slot would throw away precisely the insertion support and volume which pay this estimate. Direct old-slot averaging in a preparatory prefix is the different case handled by Section 21.

After this Gaussian connected-record construction, and after the literal completed or conditional component integrations, the independent-slot forest recursion in the companion quotient note is applicable. It is not applicable directly to the correlated Gaussian measure merely because metadata incidence sets have been declared disjoint.

### 22.1 The mixed-prefix root count

At a fixed actual stage `j`, root a new record on its genuine integration strip. There are only `D_j` such native roots. For an incoming birth `b<=j`, combine its paid quotient connector with the actual prefix reconstruction row, retaining a true old owner/core port of grade at most `b`. The source annular decay, LFR I (1.47) with the actual native measure, can be chosen as `exp[-Gamma(j-b)]` with `Gamma>4 log L`. It pays the true finer-patch count `L^{4(j-b)}` before that count is summed. It is not an estimate assigned to an arbitrary map endpoint elsewhere on the old carrier. Resident old grades at most `h` remain unchanged by preparation; recent exterior records retain their exterior owner and history. A fixed halo grade allowance, if used instead of an interior port, costs only a fixed polynomial in `R`.

For a recent coarser input `b>j`, each actual `j`-cell is contained in only a fixed number of `b`-cells. Sum the whole old atoms at those `b`-roots, costing at most `C D_j A_b`; do not subdivide them into `L^{4(b-j)}` new atoms. The genuine strip avoids all persistent resident old kernel footprints by the retained three-layer collar, and every recent old core is exterior by eligibility and whole-component exclusion. Consequently a directly integrated slot lies on the old atom's active paid dependency part, not in an uncounted free old core. The block root used in this estimate is real.

The actual integration/localization label pairs in (1.63) cost at most `N_r^2`. Keep the native grade of every new piece even after the component-`P` rooted sum has been proved. The deterministic decoration of a new protected `P` is performed only after this sum. This gives the required polynomial component-root load without ever enumerating every fine cell of the whole coarse attempted component.

## 23. Nonlinear recent-input terms do not require a repeated fractional-power loss

Let `K_r` be the strong rooted positive load of the recent completed inputs in a single whole-prefix construction, after the actual mixed-grade sum. Introduce one common scalar mark `t` on exactly these inputs. Keep the independently controlled ordinary conditional law fixed. All other guarded interaction marks remain explicit. Suppose the positive forest bound is uniform with total primitive load at most a fixed small `sigma_r`, and put

`R_t = sigma_r/(C K_r) > 2`.

For `|t|<=R_t`, each marked Mayer factor satisfies

`||exp(t v)-1|| <= 2 |t| ||v||`,

because its individual load is at most the total rooted load and `|t| ||v||` is below the fixed threshold. The same positive graph/forest proof therefore gives a bound `C sigma_r` for the resulting Banach-valued logarithm `L(t)` on the entire disk. The Banach space here is the weighted activity space; it retains each new graph record and its common analytic-domain norm. It is not only the norm of a signed scalar sum.

Cauchy in the **one common mark** gives

`||L(1)-L(0)-L'(0)||`

` <= C sigma_r sum_(n>=2) R_t^(-n)`

` = C sigma_r/[R_t(R_t-1)] <= C' K_r^2/sigma_r`.          (M18)

This argument uses no independent fine-coordinate phases and no unproved coefficient `l1` consequence of a nonlinear scalar supremum. There is only one homogeneous degree variable, and its geometric Cauchy sum is explicit.

For the conservative choices `K_r<=poly(ell_r) epsilon_r^(1/18)` and `sigma_r=poly(ell_r) epsilon_r^(1/72)`, the right side has exponent

`2/18-1/72=7/72 > 1/18`.

The strict spare exponent pays the fixed recent-window and root-count polynomials and leaves the same target `epsilon_r^(1/18)` envelope. It is unnecessary, and would be wrong, to apply another source `1/9` power to this coefficient at every inner preparation stage. This is one whole-prefix analytic calculation.

The degree-one term needs its exact interpretation. If the reference is just the ordinary conditional law, it is the linear transport `Pi_ord F`, with its consumed-slot annotations. If guarded interactions `W` remain in the reference exponential, it is instead `Pi_W F`. The difference from `Pi_ord F` is given by the exact normalized covariance identity with a `W` mark and is a new guarded response. One may not silently drop that denominator response or call it unchanged transport. The pure linear transport retains its old norm annotation; the marked response and the degree-at-least-two part receive their new small bounds. The whole-component failure rule and the higher-slot marks of Section 21.5 then prevent an unguarded operator constant from being multiplied indefinitely along the same lineage.

## 24. Raw ownership, remote low slots, and a valid one-time reserve

### 24.1 The large-field components are geometric components

The source geometry must be distinguished from its later polymer connectivity. CMP109 p.251 defines its sets first in continuous space, then uses the same symbol for the induced lattice points, bonds and plaquettes. Page 257 explicitly uses closed partition cubes and introduces the **special wall-connected convention for localization domains** `D_j`. CMP119 p.251, after (1.20), and p.255, (2.3), instead refer to connected components of the large-field complement before replacing a small component by its smallest convex rectangular union.

At the retained C01 geometric-component convention, touching closed cubes belong to the same large-field component. Distinct components of the compatible `M R_r` grid therefore have a gap at least a fixed multiple of that mesh. The wall-only or hard-core conventions later used for polymer localization are not substituted here. This is the convention needed for the CR.5 separation of newly retained bounded components. The source does not contain a separate sentence literally saying “connectedness includes touching”; the distinction follows from the geometric-set convention and the separately declared special definition for localization domains.

### 24.2 A local prefix layer must not secretly acquire remote lower raw slots

The ordinary tilt can create a previously absent lower-grade external raw argument, as well as a higher `A_l`. The high-slot split alone does not exclude this. Localize the actual conditional law outside `D(P)` and retain its zeroth layer. This layer has its complete actual raw dependency in `D(P)`. A remaining record depending on raw data outside `D(P)` has a real source path from the integrated support in `P` through the enlarged collar.

There is an **absolute density** estimate here, not only a phase estimate. The Gaussian/Schur/coarea walk difference has an absolute normalized-row or trace bound `poly(ell_r) exp(-cR_r)`. If an ordinary full-tree `B/C` coefficient contains an integrated raw endpoint and a raw argument outside `D(P)`, its carrier itself crosses the collar. A real-reference finite difference is bounded by twice its source value bound, with no derivative in an old raw variable. Directly coupled births are in the finite preparation window, so the genuine strip-root count remains polynomial. For a dependence conveyed through the native background, retain the actual reconstruction response and apply Cauchy to the composed coefficient on the external `++` chart; the explicit cost is at worst a fixed inverse coupling and a fixed logarithmic polynomial. Earlier native-only terms use their separately guarded source-map records.

After factoring terms independent of all integrated variables, the actual density can consequently be written

`w_s(a)=w_0(a) exp(Delta_s(a))`,

`sum_new_records weight ||Delta_record|| <= epsilon_r`,

`epsilon_r=C g_r^(-u) poly(ell_r) exp[-cR_r]`,             (M19)

on the required full outside-`D(P)` localization disks. The changed raw endpoint and its connector remain in each record. The quadratic difference includes all true cross blocks assigned to this comparison; cross-component terms already separated in Section 21.1 remain marked rather than being counted twice.

Let `Pi_0` be the normalized local ordinary law and `||Pi_0||<=M`. Put `E=exp(Delta)-1`. The exact quotient identity is

`Pi_s F-Pi_0 F = [Pi_0(EF)-Pi_0(F) Pi_0(E)]/[1+Pi_0(E)]`.

If `M(exp(epsilon_r)-1)<1/2`, then

`||Pi_s-Pi_0|| <= 2(M+M^2)[exp(epsilon_r)-1] <= C_M epsilon_r`.

Expanding `E` and the denominator in their actual convergent positive exponential/geometric majorants preserves the weighted new-record bound in (M19). This is the moving-mass response. It proves that a remote lower raw dependence is a **new guarded record**, rather than a free new argument of a purportedly unchanged transport.

For a retained failed component, the next ordinary enclosure contains all of `D(P)`. Any later attempt meeting that complete footprint then contains the retained component and obeys its failure clock. Thus the local layer's older raw arguments are protected. The preceding argument is needed for the genuinely remote layers and cannot be replaced by a mere assertion that all normalized-kernel arguments are local.

### 24.3 One reserve per original source block, not per fine coordinate

An arbitrary resummed ordinary `B^(b)(X)` can contain many much finer old `A_j` coordinates. Its bound `B_0 exp[-kappa d_b(X)]` does not justify multiplying its norm by `M^{number of all those fine coordinates}`. The following ownership fact provides the correct finite reserve.

Fix an original source `b`-block of the incoming paid carrier. The record is present before the current ordinary step, so `b<=r-1` and every directly occurring old fluctuation slot has index `j<=b-1<=r-2`. If a successful preliminary integration in an attempted component `P` directly uses a slot in that block, the slot belongs to

`Z_(j+1) subset Z_(r-1)`.

The current ordinary growth puts this set inside `P` with distance at least `c M R_r h_r` to `P^c`. The original block has diameter at most `C M h_b<=C M h_r/L`. Hence, for the one common large lower cutoff on `R`, the **whole original block is contained in P**. This conclusion uses the deep endpoint, not just the fact that the block intersects `P`.

There are two possible endings.

* If the preparation fails, the entire original `P` survives with its failure index `r`. Any later containing attempt starts above that event. All old slots of the original block have grade below `r`, so no such slot is directly integrated again along that retained lineage. The local extra raw support in `D(P)` has the same protection; remote new dependencies have (M19).
* If the component reaches a complete R integration, every old `A_j` variable in the contained block is integrated. This follows from the exact operation list, not from the size of the block. CMP119 (2.20)–(2.22) lists the old factors. LFR I (1.71)–(1.72) retains precisely the complementary prepared factors after the shell integrations. LFR II p.378 defines `T'_r(P)` by composing the remaining integrations and the `T_h` operation in LFR I (1.100). Finally LFR II (1.103)–(1.104), p.392, states that a completed retained component has no integral operations left and only a multiplier depending on the new `V_r` restricted to it. No old `A_j` inside `P` survives that completed integral. The assertion holds in particular on a successful component which is then removed.

Thus one bounded-operator reserve per **original source block** suffices for all its fine old coordinates. There is no `L^{4(b-j)}` mark count. Distinct simultaneous components cannot each own the same small block; each ownership event contains the whole block. On an early failed branch all later possible uses are ruled out by its clock; after complete integration the slots have disappeared.

The reserve can be chosen as a fixed factor covering `M_pref` and the fixed new-tag convention. It is paid once from a small part of the original full-tree carrier/active-block reserve when an ordinary source atom first enters the completed-input bank. A full-tree source carrier visits every one of its original blocks, so its spare source exponent pays this factor per block. A relative input retains its already allocated original block marks. Free-core interior fine points and purely decorative halo points receive no new marks. For genuinely new `A_(r-1)` supports in an ordinary-T response, use its explicit creation records instead: their new Gaussian-support volume, or their exposed paid-connector cells, pays the finite number of new marks. The phase estimate gives `M_pref=sec eta_*` with `eta_*` arbitrarily small at a smaller ceiling, so this fixed per-block or per-created-coordinate cost fits the already chosen reserves even when their native block multiplicity is large.

This is an actual-family annotation. It does not assert a weighted raw-coordinate norm for every abstract bounded input function. The original blocks, true raw support and the disappearance/protection just proved are indispensable.

### 24.4 Successful components are a new paid creation

The claim that successive direct-component events are geometrically disjoint uses a retained **failed** component. If an earlier component succeeds and is removed, a later grown component can overlap its former position without containing an earlier retained failure. The failure-clock argument must not be applied to that pair.

The source has a different exact payment in this case. A connected record genuinely using a successful component carries its actual `T'_r(P)1` mass in the first polymer expansion, LFR II (1.89), (1.91)–(1.99). The p.389 bound pays the restored interior with its full volume factor. Such a record is assigned a new successful-component creation budget, including its new argument list and any corresponding original-block reserves. It is not an unguarded linear transport of the same older budget. If the inserted function is independent of the component, `Pi_P 1=1` removes that incidence before any estimate.

This distinction covers possible new raw dependencies of a successful-kernel output outside the original owned block. It also avoids spending a released interior segment twice: on retained failures that segment is released once into a new core; on successes its restoration and any later use have the separate successful-component payment. The maintained connector rate is unchanged in both cases.

### 24.5 The transport polynomial is charged once to an original creation

Keep the creation grade `b` of an unchanged direct old-slot list distinct from its later geometric transport grades and from the original block grades carrying its finite operator marks. An unguarded direct preliminary use at attempt `r` requires

`h_r <= j <= b-1`, and consequently `r-b < N_r`.

The source choice `N_r <= C(1+ell_r)^p_N` and the retained AF envelope imply that there are at most `C(1+ell_b)^p_N` possible outer attempt labels for this unchanged list. The actual eligible rectangular chain bounds the native strip/root counts in that window by a further fixed logarithmic polynomial. Sum those possible regroupings for the original creation before taking the final grade/root supremum. This spends one fixed polynomial in `ell_b`; it is not a polynomial multiplier at every subsequent transport. Original-block marks pay the corresponding normalized-operation constants separately. Local newly acquired raw slots are protected by the failed-component footprint, remote new slots are the guarded records of Section 24.2, and a genuinely used successful component is a new creation as in Section 24.4. None of these cases recreates an uncharged copy of the original creation list.

## 25. Literal-catalog repair: no recursive change of native extension

This section replaces Section 19.1 **as an instruction for the recursive construction**. That section correctly describes one compatible exterior extension of a final physical response, but equality on the unlocalized physical current family alone does not identify every localized self coefficient at the next stage. CMP116 (1.5), (1.11), and (1.17) allow propagators with localization parameters to be arbitrary operators with the required bounds. A real localized parameter need not put the intermediate field on the original minimizing graph. It would therefore be invalid to replace an inherited analytic extension, localize it anew, and silently identify its self part with the original canonical self part.

The repair is to keep the literal source catalog throughout. Use the exterior four-map construction of LFR II pp.369–373 only in its original branch, where the actual localization domain `X` is disjoint from the attempted union `Z`. For `X` meeting `Z`, retain the interior reconstruction (1.61)–(1.65), including the all-empty projection reference. No identity `U(B,M(U))=U` is used on an independent native pair. Retain the literal resummation into `V(Y)`, the self coefficient `V(P^~)`, and the old-action add-back on p.377. The following geometry supplies the guard which the proposed extension replacement was intended to obtain.

### 25.1 The old owner supplies the missing guard

The displayed support has an exact ledger. CMP109 p.257 defines localization domains as connected unions of the actual `M`-cubes, not convex hulls of activity carriers. In LFR II the new carrier is the union `Y_1 union Y'_2 union Y'_3 union Y'_4`; the initial cover adds the touched whole components. Apart from paid source/localizer cubes, the only uncharged support is an actual owned component footprint, of thickness at most two birth `MR` layers, and fixed `M`-scale cover/stencil padding. The `C R` neighborhood in the root estimate (Q6) is only an upper bound on distance to this specified decoration; it is not permission to attach a free ball or hull of that radius. A padding-only contact therefore cannot jump the four-layer owner buffer: an owned footprint stays in its owner's component, and fixed `M`-padding leaves a positive `MR_r` crossing once the common lower cutoff is fixed.

Fix an attempted current component `P`.

* **An exterior owner.** Let its current large-field component be `Q`, with `Q` disjoint from `P`. The compatible cover of `Z_(r-1)` and its four current-scale layers lie in `Q`. The old owner/footprint lies on the inner side. Any actual paid dependence reaching `P`, or its fixed one-layer self collar, must cross a positive part of this ordinary-growth buffer. No old free core occupies the buffer. In birth-`b` units the charged length is at least `c R_r L^(r-b)`, up to the fixed endpoint allowance. This remains true for an all-empty interior projection term. Its two analytic values may be bounded separately by the old norm; there is no need to identify their offphysical references.
* **A resident owner.** If the nonself record already has an actual old terminal outside `P`, its old paid graph crosses the annulus from the protected owner to `P^c`. If the original domain is wholly inside `P`, a nonself output must contain a genuinely nonempty new localization component escaping the self region. The literal source `Y'_i` contains a deep component of `Lambda` and meets the preceding determining boundary. Its new paid volume and actual first-nonempty reconstruction leg provide the guard, as in Sections 17–17.1. A wholly contained all-empty record is the literal canonical self term, not a nonself small activity.
* **A reconstructed old-action add-back.** The source history deletion and nesting `Z_b^new subset Z_r^new` give it an actual surviving exterior owner. Apply the first case. A deleted owner cannot be replaced by a formal exterior label.

An incidence created solely by enlarging `Y_1` is removed by the exact normalized identity when the scalar is independent of that hidden variable. An external direct scalar with no genuine hidden incidence remains in the scalar catalog; the previously paid connector is retained. No such scalar is discarded.

This case division uses the original source domain in deciding interior versus exterior. It does not enlarge the exterior branch from `Z^c` to every domain missing only the smaller deep set. For the new-localizer branch, the first-nonempty source map still carries the actual outer reconstruction row needed for the native age/root estimate. For the old-connector branch, the physical buffer crossing itself gives the stronger birth-scale length `c R_r L^(r-b)`. Thus the repaired guard does not require an offphysical cancellation or a new self law.

### 25.2 A consumed core remains one bounded test

The released factor per consumed old tag can pay a fixed factor per tag. It cannot pay a factor exponential in the number of fine native sites inside an old core. No such fine-site expansion is made. The entire resident old scalar, including all its real old/raw slots in the consumed core, remains a single bounded Banach-valued test under the literal completed operation. The source deep `Lambda` contains the resident protected footprints; localization parameters are outside that deep set. Only genuinely new exterior response pieces, old exposed active blocks, and the actual new localization volumes are expanded. Source Cauchy estimates act on the admitted whole old scalar and on the new localization variables. They do not introduce one independent Taylor patch for every fine interior point of a consumed core.

The existing Taylor product of Section 18 therefore applies to persistent near/exterior perturbations and exposed paid supports. It is not used to manufacture a volume weight on an old free interior. When several consumed tags merge, their released tag weights pay only the corresponding finite tag constants, with the remaining constant per new component paid by the current incidence guard.

### 25.3 The canonical operation is imported on an intersection of actual invariants

The abstract selectively free-core norm does not imply the source physical outside-tree norm at the same rate. For example, many widely separated exterior ports can be joined cheaply through one free box, while a physical tree visiting those ports is much longer. A single collar factor cannot restore every such physical tree. No embedding of all abstract `A_*`-bounded inputs into the original source invariant is asserted.

Instead, the induction ranges over the literal source-generated histories which retain the source scalar invariant **and** the additional positive selective estimate proved here. Theorem 1 and LFR II pp.391–392 explicitly retain the alternative (1.103)–(1.104) in that source induction. On these same literal histories, p.379 expands the actual self coefficient and actual quadratic form, roots the old-boundary response at `B_0 union (Gamma''_k intersection Gamma)`, and includes all earlier boundary terms. Equations (1.73)–(1.75) give the unchanged canonical normalized-operation bound. The primitive native and independent-current chart is its stipulated source chart, restricted to the admitted fixed strong core; the larger value profile is chosen within that source domain by the retained chart results.

Because Sections 25.1–25.2 leave every source self coefficient and its analytic extension unchanged, this is now an independent source input. It is not obtained from C05, and it is not an operator theorem for arbitrary selectively bounded inputs. Auxiliary large activity marks remain outside the canonical completed self law. The ordinary mark-zero partial reference has its own independently proved phase bound. This separation avoids both the extension-switch compensation and an implicit circular use of the desired current estimate.

## 26. Ordinary forcing can enter as whole resummed source atoms

The inherited-owner proof in Section 25 does not apply to an arbitrary local ordinary `E` or `R` term near the boundary of an attempted component: such a primitive need not have an old boundary owner. Also, the statement on LFR II p.377 that `alpha` can be made arbitrarily small is not, by itself, an AF-summable estimate. The following restricted use of the actual source bound closes this ordinary sector without making either inference.

### 26.1 The restricted source class and the atom retained

After the explicit Wilson/quadratic rearrangements on LFR II pp.356–369, the construction of `V(Y)` on pp.369–377 is linear in the incoming scalar `E/R/B/C` activities, with its field maps and history fixed. Keep the purely ordinary part, namely the independently bounded full-tree `E/R/B_0/C_0` inputs and their stated source subtractions. All completed/relative-input descendants are excluded from this part. They continue to use the direct positive proof of Sections 15–25. The ordinary part may equivalently be obtained by putting the relative-input marks equal to zero at this linear stage; this is an auxiliary decomposition, not a change of the physical canonical self action or coupling trajectory.

The remaining inputs satisfy the ordinary full-tree inductive assumptions used in the proof of (1.66)–(1.68). The source estimates and resummation therefore apply to this part by itself, with fixed ordinary constants. Keep the **entire resummed coefficient**

`V_ord(Y,(U,J))`

as one new atom. On the admitted value chart it has the literal source bound

`||V_ord(Y)|| <= C_ord exp[-a_s d_(k,Z)(Y)]`,

`a_s=(1+2 beta) kappa`,                                (M20)

for the nonself domains in (1.68). One may arrange `C_ord<=1`, but only its uniform boundedness is needed below. The norm here is the supremum of this one coefficient on the full stated native chart. No norm of its individual signed internal histories is inferred from (M20).

The independently ordinary family is available on the fixed larger source profile used for the prefix phase estimate. Its restriction to the completed value profile and the common strong core gives (M20), with the original source map admission and its fixed margin. The fixed logarithmic profile powers are chosen once before lowering the ceiling. This does not assert a new larger chart for the unknown completed-input induction. Its constants may depend on those fixed powers, but not on cutoff depth or on the running logarithm.

Ordinary direct terms reconstructed in `A'_k` which have no completed incidence stay in the ordinary scalar ledger. They are not assigned a new free component merely because of displayed support overlap. The exact Wilson, Gaussian/Schur, coarea and subtraction terms remain in the source roles which precede the `V` construction; the standalone Gaussian and classical responses are still counted in the accepted ordinary-current sectors.

### 26.2 A source physical tree, not a proposed halo pushforward

The output domains in the literal p.377 statement satisfy the full source self-footprint predicate: their intersection with `Z^~` is a union of whole components of `Z^~`, containing at least one. Here `Z` is the union of the attempted bounded components. An unbounded unrelated ordinary large-field component is not excused from the metric.

The tree in (1.67) is an actual physical tree visiting all `M`-cubes of `Y\Z`; paths through `Z` still have their physical length. For each used original component `P`, the output contains its full positive self footprint. Its exterior shell contains `M`-cubes on opposite faces of a rectangle of side at least `20 M R_k`. Thus that tree has length at least `c M R_k`. This implication needs only a positive complete `M`-shell; it does not depend on deciding whether the printed tilde has the larger `MR_k` thickness.

The stronger surface count is also available when useful: a positive `M`-shell has at least `c R_k^3` distinct exterior `M`-cubes in four dimensions, and a connected physical tree meeting `N` grid cubes has length at least `cM(N-1)`. The fixed disjoint eligible rectangles have bounded shell overlap. In particular the source tree pays at least `cR_k` per genuine current component incidence, either by this count or by the physical tour/packing argument. Retain a spare part of `a_s d_(k,Z)(Y)` for that payment.

The selective output cost is no larger than this physical tree cost: declaring only the actual bounded completed cores free can shorten a path but cannot increase it. The actual outside cubes, new marks and any support covers can therefore be kept in the positive catalog using a fixed smaller tree/count rate. This is a direct property of the source's **already resummed ordinary atom**. It is not an unproved claim that an arbitrary old selectively free-core pregraph pushes forward to a full-halo visiting majorant.

### 26.3 Absolute rooted summation over the final domains

For completeness, an individual estimate (M20) is not yet a rooted activity norm. The following counting argument gives the required sum with constants independent of the sizes and number of fixed current components.

Write `E=Y\Z`, in its `M`-cube cover, and let `d=d_(k,Z)(Y)`. Discretizing a physical tree of length at most `M(d+1)` produces a connected `M`-cube animal `S` of at most `C(d+1)` cubes meeting every cube of `E`. A fixed enlargement changes only `C`. This elementary bound follows by dividing each tree edge into intervals of length at most `M`; one such interval meets a bounded number of grid cubes. The connected graph can be traversed with total length at most twice its tree length, so the number of intervals is linear in `d+1`.

For an outside root, anchor `S` at that root. There are at most `A_d^n` rooted grid animals of size `n`. Within `S` there are at most `2^n` choices of the outside-cube set. Each included whole component has an exterior shell cube in this set. The fixed compatible eligible components have bounded local overlap, so at most `C n` component choices can be incident to `S`. Their subsets contribute at most `2^(C n)`. Once the outside cubes and these fixed components are specified, the source domain `Y` is specified; there is no sum over a new shape of a component. Consequently

`#{Y rooted outside: n<=d_(k,Z)(Y)<n+1} <= C exp(C_ent n)`. (M21)

If the root is inside a used component, choose an exterior shell cube at distance at most `C M R_k`; this costs at most `C(1+R_k)^4` root choices. A component root can instead use one fixed shell cube of that component. These factors are polynomial, and the preceding `cR_k` source reserve pays them. Merged self-footprint components cause no additional shape sum: their original eligible constituents are still fixed, and the same bounded local packing count applies.

Choose the positive output count and connector rates below fixed available shares of `a_s`, and retain enough of the large source exponent to dominate `C_ent`. The actual source parameter choices permit this. Fixed canonical-incidence factors, the finite original-block mark weight and tag weights are paid by the unused component/length reserve. Combining (M20)–(M21) gives

`sup_x sum_(ordinary nonself Y containing x)`

`    weight(Y) ||V_ord(Y)|| <= C (1+R_k)^p exp[-cR_k]`.  (M22)

The same bound holds at a genuine component root. It is a sum of the individual analytic suprema of the whole `V_ord(Y)` atoms. It is AF summable by the retained envelope. No use of `alpha(g)` as a superlogarithmic factor, and no phase-lifting interchange of suprema, is involved.

### 26.4 Scope of the ordinary seed

Equation (M22) supplies the genuinely new ordinary nonself primitive load required by the rooted forest argument. The literal ordinary self terms stay in the canonical operation. The independently current Gaussian/classical/E/R and direct-scalar terms stay in their accepted sectors. The harder inherited selectively free-core input continues to use Sections 25.1–25.2, coarsening, actual new localizer volume and the same positive forest algebra. Thus the ordinary seed and inherited propagation cover distinct, exhaustive inputs without assuming the disputed full-halo bound for the latter.

## 27. A complex phase cone gives a common positive reference on a smaller chart

The operator estimate `sup_xi ||Pi_xi||<=2`, by itself, does not justify interchanging a sum of activity suprema with integration when the activity catalog depends on an integrated history. A common dominating measure is needed. The already established phase cone on a fixed larger **complex** domain supplies it without a new high-dimensional density Lipschitz estimate.

### 27.1 Analytic strip lemma

Let `p_z(a)` be normalized densities on one fixed measure space, holomorphic for `|z|<R`, nonzero on their fixed support, and suppose

`p_0(a)>0`, `integral p_z(a) da=1`,

`|arg p_z(a)|<=2 eta<pi/2`.

For `|z|<=qR`, `0<q<1`, the following pointwise bound holds:

`|p_z(a)| <= exp[C_q eta] p_0(a)`,

`C_q=(4/pi) log[(1+q)/(1-q)]`.                         (M23)

To prove it, fix `a` in the common support and set `f(z)=log[p_z(a)/p_0(a)]`, using the branch in the right half-plane. Then `f(0)=0` and `|Im f|<=2 eta`. The function `H=exp[pi f/(4 eta)]` maps the disk to the right half-plane and has `H(0)=1`. Schwarz's lemma applied to `(H-1)/(H+1)` gives its modulus at most `q`. Hence `(1-q)/(1+q)<=|H|<=(1+q)/(1-q)`, which is exactly (M23) after taking logarithms. The case `eta=0` follows by continuity, or because a real-valued holomorphic normalized ratio is constant.

The same result holds on a complex Banach ball or a polydisc: restrict to the complex line from its fixed real center to a point in a fixed homothetic smaller domain. This argument is dimension independent.

### 27.2 Application to the whole ordinary prefix

In Section 21 take the full joint variable `a` to include **every** integrated real coordinate and every internal discrete history label. Remove only factors independent of all those variables. Any history-dependent coarea/normalization factor stays in the phase estimate. The cutoffs and admissible supports are fixed after the actual source relocations.

At every admitted complex native/localizer point, `w(a)` lies in a common cone of half-angle `eta_r`. Its integral lies in the same cone. Thus the normalized density `p=w/integral w` satisfies `|arg p(a)|<=2 eta_r`. At the single fixed center consisting of the real native background and localization parameters `s=1`, the normalized density `p_0` is positive.

Reserve a fixed extra factor in the native analytic ball and in the new localization disks before choosing the source constants: for example, use the phase estimate on a ball twice the working radius and on `|s|<=4 exp(kappa_1)`, and use `|s|<=exp(kappa_1)` for the actual coefficient contours. Along the line from `s=1` to a working point, a fixed line-radius margin then remains. CMP116 (1.11) allows this fixed enlargement by replacing the already fixed `kappa_1` by `kappa_1+log 4`; choose `M` and the coupling ceiling afterward. The excluded `D(P)` collar and all previous absolute remote-row estimates are unchanged except for fixed constants. This is one fixed domain reserve, not a new radius at every prefix.

Applying (M23) gives one positive probability reference `mu_0` for the whole attempted component such that

`|dPi_(xi,s)(a)| <= M_pref dmu_0(a)`,

`M_pref=exp[C eta_*] -> 1` as the common ceiling tends to zero. (M24)

Use this slightly larger, still arbitrarily near-one constant for the original-block marks. It replaces `sec eta_*` when a common majorant measure is needed. The simpler sector inequality remains valid as an operator bound, but it is not the justification for changing the order of a sum and a supremum.

### 27.3 Strong catalogs and internal histories

The precise order of the stored conditional norm is

`sup_(external history, real exterior raw data)`

`       sum_G w_G sup_(native xi) |F_G(xi, real raw data)|`.

The real-raw supremum is **outside** the activity sum. Uniformity over literal old/raw support means a uniform conditional catalog bound at each fixed real tuple. It does not mean a sum of independent raw suprema for different activities. The positive reference may depend on that fixed exterior tuple, which is harmless in this order. Allow the internal catalog to vary with the integrated `a`; take the union of all possible output labels and put absent entries equal to zero. Retain the relevant history/geometry label in an output record when it determines its weight. With the already proved uniform per-history, pointwise-real-input positive bound,

`sum_G w_G sup_xi |integral Pi_xi(da) F_G(xi,a)|`

` <= M_pref integral mu_0(da)`

`       sum_G w_G sup_xi |F_G(xi,a)|`.

The last sum is bounded at each real `a` by the actual conditional strong catalog norm. Integrating its bound against the one probability measure proves the inequality, after which the exterior raw/history supremum may be taken. This is the needed uniform-domain, sum-of-native-suprema inequality. It remains true for different admitted current/native pullback curves in the different records, since the same measure dominates the kernel everywhere on the common working chart. No interchange of a raw supremum with the activity sum is used.

For the canonical completed operation, the fixed-real-center comparison in LFR II pp.379–380 already supplies a common positive reference and the uniform `sigma` ratio bound. It is applied on the unchanged literal source family, as in Section 25.3. The elementary argument above is needed for the auxiliary ordinary prefix, whose initial proof was formulated only as a phase cone. Both integrations now preserve the strong positive catalog without an illicit interchange of a history supremum, a native supremum and an integral.

## 28. Linear prefix grouping commutes with future self extraction

Equality of complete scalar functions alone would not justify changing the localized self coefficient used by a future canonical operation. The one-time linear transport has an additional source support property which is needed here.

For a boundary insertion `F(X)`, the source localization retains the whole original carrier `X`: the new operators are localized outside that carrier and the resulting domains are unions containing it. This is the boundary-term construction in CMP119 pp.276–277 and the localized insertion construction (3.44)–(3.47), as used in LFR I (1.60)–(1.63). Retain that original label even if a particular reference evaluation is independent of one of its old slots. The direct prefix branch has an actual old raw endpoint in `X intersection P`, with the depth and original-block ownership of Section 24.3.

Group the outside reference and the degree-one correction only in the zero operator layer whose additional dependence is contained in `D(P)`. Here zero layer means deleting or zero-marking the actual remote coefficient/walk records, while keeping their original source localization labels. It does not mean replacing an existing native coefficient by another offphysical continuation. Their literal source domains remain recorded; all lie between the original `X` and `X union D(P)`, up to the fixed support conventions already included in that footprint. Source changes with a genuine extra outside localization domain remain separately marked records. Their current/new-volume or remote-kernel guard has already been paid. The exact ordinary numerator/denominator cancellation then identifies this zero-remote linear sum with the zero-layer normalized insertion on the common analytic family.

After a retained failure, consider any later component `H` and its literal self region `H^~`. If `X` is contained in `H^~`, its original deep raw endpoint is there. The ordinary owner buffer prevents the self halo of an exterior component from reaching that endpoint. Hence `H` contains the whole retained `P`; the failure clock and preserved inner layers put its complete `D(P)` inside `H`. Every member of the grouped zero-layer family is then self. If `X` is not contained in `H^~`, every member still contains `X` and is nonself. For several genuinely used components, apply the argument to each original endpoint.

Thus the exact zero-layer identity which combines the outside reference with the degree-one logarithmic correction holds **after every later source self restriction as well**. It does not replace a self coefficient by an analytically different one. New ordinary-T/map/localizer pieces outside the protected union are separate guarded responses; a successful component has its own mass-paid new creation. These are precisely the cases in which the old linear family is not carried unchanged. This ownership argument is the justification for the whole-prefix regrouping under the literal-catalog convention of Section 25.

## 29. The regular E phase uses its running source chart

This section corrects the fixed-absolute-chart wording in Section 21.3. The actual reset-affected regular action is the one in CMP119 (2.25)–(2.29). Its coefficient value bound has a grade-independent constant `E_0`, but its two analytic radii are `g_b C_i ell_b^(q_i)`, as printed in (2.28). The fixed absolute radii in CMP109 (1.18) are not a larger chart for that actual bank.

### 29.1 The quantity entering the ordinary conditional density

At an ordinary integration grade, keep the literal renormalized fluctuation difference in CMP116 (1.33). Equations (1.34)–(1.36) give joint native/current analyticity and its local activity bound; the proof (1.24)–(1.32) has already summed the earlier `E` grades and their fine roots. CMP119 p.276 transfers this proof to the actual scale layers: the interior terms satisfy exactly the stated earlier lemmas, and the remaining terms use its mixed-native space (3.43).

At a partial prefix step with integration grade `j`, the inherited bank is the whole outer `E_r`, not a truncation to births `b<=j`. Keep the difference of that same whole bank between the actual stage configuration and its `A_j=B_j=0` reference. LFR I p.182 after (1.24) states that the old action changes only by the new boundary contributions; (1.60) displays this extraction explicitly. Its localization is of the mixed type before (1.63), and (1.63) keeps a separate proper support grade `m>=j+1`, with `m<=r`. Denote the regular-action pieces by `V^E_(j,m)(Y)`. The proper-layer Ward calculation groups primitive births `b<=m`; the genuine `E^(b)` anchor and the support of its matched `phi_b A` lie in `Lambda_b subset Omega_b`, so a carrier containing that dependence cannot be assigned a smaller maximal regularity grade. This retains also every birth `j<b<=r`. One must not replace the whole prefix difference by `E_j`.

The whole inherited action includes each of its own vacuum and Wilson subtractions from CMP119 (2.25). The Ward operations are made at each proper regularity grade before the birth sum: CMP119 (3.49)–(3.67), or CMP109 Sections 3–5. No estimate of a separate extensive sum of raw `E^(b)` values, and no separate sum of `|beta_b A|`, is inserted into the phase proof.

In the full conditional prefix density, telescope the ordinary operations in their literal order. Every `E` factor which depends on one of the integrated coordinates occurs in these fluctuation differences. A term independent of **all** integrated coordinates and internal discrete labels factors out of both numerator and denominator and belongs to the common external scalar. A term depending on an earlier integrated coordinate is retained at that earlier grade. This is an exact identity of the conditional density, not an estimate which drops an old action or a mass. The same rule applies if a higher external raw slot has been centered in the `V_lo/V_hi` decomposition.

### 29.2 The source family at the independently chosen larger profile

Choose the ordinary profile exponents `q_i+Q_1+Q_2` once, before lowering the common coupling ceiling, and apply the retained original source invariant with these exponents. CMP119 (2.28) permits fixed sufficiently large integer exponents; the source constants and the weak-coupling ceiling are chosen afterward. The new ordinary output also has the analytic and decay reserves stated on p.262. The relevant source assertion is the actual-family invariant on this selected chart, including the simultaneous localizer and independently extended current variables. It is not an assertion that arbitrary complex synthetic `E` inputs with an inconsistent numerical coupling array satisfy that invariant.

Reserve the fixed input-to-output factor `c_ext` of E14.47–E14.49 in the ordinary source constants. Thus the actual source coefficient chart at this exponent is chosen large enough to admit the desired external `++` strong ball. This is a single fixed factor for the already known ordinary family, not an iterative assertion that a reduced output ball regenerates its own input radius. The quantitative running-radius transfer is precisely E14.33–E14.38 and E14.45–E14.51; it is stronger for this purpose than a blind substitution in a fixed-radius source constant.

In particular the localized `V_j^E(Y)` on that admitted external chart has the source full-tree rooted bound

`sup_x sum_(Y containing x) exp(kappa_E d_m(Y)) sup_(++) |V^E_(j,m)(Y)| <= C_E`,  (M25)

with one fixed `kappa_E>0` below the available source rate. Here `C_E` may depend on the once-selected exponents and fixed block parameters but has no running factor `ell_j^(a Q_2)`. Its derivation is the positive summation in CMP116 (1.24)–(1.32) followed by (1.36), with the actual scale replacement at CMP119 p.276. The actual cutoff is used; there is no enlargement of its real support. The fields and the old real variables are fixed pointwise while taking the native supremum.

There is a useful direct check that the use of (M25) is consistent with the radius bookkeeping. If `b<=j`, the retained two-sided terminal AF envelope, with constants `a_AF,A>0`, gives

`Y_b >= (a_AF/A) Y_j`,  `Y_b <= (A/a_AF) Y_j + A(j-b)`.

These follow by comparing the two envelope bounds at `b` and `j` to the same terminal value. No one-step drift or additional signed-prefix upper-slope hypothesis is needed here.

For every fixed selected exponent `q`, after choosing the ceiling depending on it,

`(g_j ell_j^q)/(g_b ell_b^q) <= C (1+j-b)^(1/2)`,

and, for the two selected profiles,

`(g_j ell_j^(q+Q_1))/(g_b ell_b^(q+Q_1+Q_2))`

`    <= C (1+j-b)^(1/2) ell_j^(-Q_2)`.             (M26)

To see this, use `ell_b >= ell_j+log c` and `Y_b/Y_j <= C(1+j-b)`. The factor `(ell_j/ell_b)^(q+Q_1+Q_2)` is at most two at one sufficiently large ceiling, while `g_j/g_b=(Y_b/Y_j)^(1/2)`. This choice changes a fixed constant and the ceiling, not a running logarithmic exponent. At fixed prefix age window the stronger finite-window comparison in Section 21.3 applies.

The grade sum in the source proof must preserve its Ward cancellation. The marginal curvature tensor is canceled by the **own** `beta_b=P_b E^(b)`; its coefficient is not assumed uniformly bounded independently of the radius. A native Cauchy estimate may give `|beta_b|<=C E_0 (r_b^(++))^(-2)`. This causes no separate term in (M25). E14.36 retains a coefficient order `p` with its actual field degree `d>=p`, rather than replacing every denominator by the fifth power. Its near-branch sum after the four-dimensional root count is exactly the finite constant `sum_a (1+a)^(b_*+5/2) L^(-(1-theta)a)` of E14.38. The far branch uses E14.33–E14.35 and its explicit `exp[-c M L^a]` reserve. Formula (M26) leaves only that fixed polynomial in the age. In particular one may not substitute shrinking radii into the crude fixed-radius constant `C_3 epsilon_1` at the end of CMP116 while discarding the field powers retained in its earlier Ward argument. The independently extended current is covered by the actual primitive-pair Taylor identity followed by the source preparation substitution, as stated after E14.38; no identity on a physical-current graph is promoted to an arbitrary extension.

### 29.3 Phase and common-reference estimate

Apply Cauchy to each complete composed source coefficient `V^E_(j,m)(Y;xi,a)` on its admitted external strong `++` chart, with the actual real integrated tuple `a` fixed. Reality at the real center follows from the literal source formulas. At proper grade `m`, the `+` displacement is at most `poly(ell_r) alpha_m^+`; the polynomial comes from the actual finite prefix and its top-band insertion, and is fixed before `Q_2`. Equation (M26), with `m` in place of its current index, and the fixed chart margin give

`|V^E_(j,m)(Y;xi,a)-V^E_(j,m)(Y;xi_0,a)|`

`    <= C poly(ell_r) ell_r^(-Q_2) sup_(++) |V^E_(j,m)(Y)|`. (M27)

The estimate is for the full complex difference and therefore also bounds the phase. Every genuine grade-`j` integration endpoint belongs to a bounded number of proper-grade-`m` cells, with `m>=j+1`; the coarse cover of the actual strip therefore contains at most `C D_j` possible roots. Use (M25) there and sum the actual pairs `(j,m)` from (1.63), at most a fixed power of `N_r`. There is no factor `L^(4(m-j))` and no enumeration of all fine cells in the outer component. Thus the total `E` contribution is bounded by

`C ell_r^(D_E-Q_2)`,                                (M28)

where `D_E` is fixed before `Q_2`. The source old-grade sum inside (M25) is not repeated. Remote complex localizer changes are handled by the already retained absolute path estimate outside `D(P)`, not by reality at a complex localizer point. Equations (M28), (M16) and (M24) therefore retain the previously stated phase cone and common positive domination, without any fixed-absolute-`E` claim.

This correction is within the original admitted source-prefix scope of C05. It proves neither the physical asymptotically-free trajectory nor the synthetic same-radius reset-feedback invariant required separately in [Reset remainders](../../coupling/reset_remainders.md), target (6).

## 30. Complete atoms and the corrected order of operations

**Status.** The C-05 proof uses the complete-atom convention below together with the two-age replacement of OR.19 (see the status paragraph at the top of this note).

The positive-norm interpretation of Sections 24–29 must be read as follows. A degree-one local prefix telescope is one complete internally resummed atom. Its canceled internal pieces are not individually normed. Their labels remain available for the literal self projection in the single source-permitted component-saturated representation, fixed before the iteration.

The exact construction is [PC.1](positive_catalog_coarsening.md)–[PC.6](positive_catalog_coarsening.md). Internal localization choices are summed by the finite fundamental-theorem-of-calculus identity before the native supremum. At a new ordinary step, first Taylor-expand that whole atom through the common actual native map. For a fixed tuple of new map factors, the old derivative coefficient is independent of the new Gaussian variables. Choose a common conditioning support and parametrix at that point, then perform Gaussian localization and the distinguished-insertion cluster expansion. This ordering preserves the linear cancellation without asserting that independently localized covariance/precision families are inverses or have matching coefficients.

Only genuine Gaussian variables enter the trace and determinant support. A protected native footprint behind the ordinary boundary adds none. Its external native anchors and physical diameter remain in the graph, with the root conversion and divided-tree cost paid once by [PC.6a](positive_catalog_coarsening.md). A wholly contained unguarded atom has its genuine fresh relative tail; a non-small ordinary B/C0 term wholly in a component stays in the ordinary reference law.

The ordinary-prefix normalization in Sections 21,27,29 is unchanged, but its coordinate count is now explicitly sourced by [CT.1](operative_source_scope.md)/[ND.1](native_domain_count.md): both A_j and B_j lie in the complete admitted strip within Z_{j+1}[P], and the mesh conversion costs L^4 rather than the volume of an outer current box on a fine lattice. [ND.2](native_domain_count.md)–[ND.3](native_domain_count.md) proves the common positive domination with the real exterior supremum outside the positive sum.

Physical graphs are joined by union; mark and creation records retain their multiplicities. Global capacity indices are scale/operation-sector families, with all spatial positions inside the corresponding rooted catalog. The fixed proper-root incidence estimate precedes the global capacity sum. Thus no factor proportional to the total number of spatial components enters the recurrence.

Under these conventions, the four cases of [PC.6](positive_catalog_coarsening.md) preserve the direct-prefix capacity and give the same fresh primitive load, two forest estimates and closed-ball recurrence as A15–A16. The native/current readout and complete boundary budget are Theorem [FC.1](complete_boundary_estimate.md). A norm of a canceled sum does not bound the sum of its pieces' norms.
