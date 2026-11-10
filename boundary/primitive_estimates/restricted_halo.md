# Halo bounds on interior and boundary sectors

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

Supporting note. This note does not complete C-05.

## 1. Source checks that passed

1. **Fresh exterior halo.** LFR II printed p.377 distinguishes `Z^~` in the condition on the support Y from `Z` in the exponent `d_{k,Z}(Y)`. A nonself Y contains a whole component of the enlarged region `Z^~`; the tree must visit the exterior M-cubes outside Z. These exterior halo cubes are therefore paid terminals.
2. **Whole physical connecting length.** LFR II (1.67), p.376, defines a connected tree contained in Y and charges its complete length. It omits interior cube coverage, not physical connecting length through Z.
3. **Eligible geometry.** LFR I p.177 selects whole current components, imposes containment in a 100MR_k cube, and says the recent regions are rectangular parallelepipeds. The ten-layer construction increases each coordinate side, so eligible current rectangles have lower side lengths of order MR_k. CMP119 p.245 describes `~` as addition of a layer of the defining cube family; at minimum the relevant halo contains a positive exterior neighborhood. The fresh localization is on M-cube domains.
4. **Ordinary T first terms are unchanged native functions.** CMP119 p.268, (3.15), contains exactly
   `(E_k+R_k+B_k)(U_k(exp i[...] V^(k))) - (E_k+R_k+B_k)(U_{k+1})`.
   The unchanged coefficient is evaluated at the new background. Its original carrier is not projected to its exterior. Pages 276–277 describe localization of each boundary difference. A declared halo can therefore remain in the unchanged coefficient's support.
5. **The R add-back must be kept.** LFR II p.377 explicitly restores old-age terms on the new determining history in A'_k and subtracts them in V(Y). It is incorrect to say that every old-age term meeting the attempted region simply disappears into a new birth label.

## 2. Geometric shell payment

Let H be a rectangular component in d=4, with all side lengths between c a R and C a R, where a is the physical M-cell length at its original birth. Assume its scalar support contains a complete positive exterior halo, hence all exterior a-cells along its faces. For a connected rectifiable tree T visiting those exterior cells,

\[
\operatorname{length}(T)\ge c_1 a R^3.
\tag{A1}
\]

To prove this, choose a face and retain every third tangential a-cell, away from its edges. This gives cR^3 uniformly separated cells. A connected tree meeting these cells must spend at least ca length in mutually disjoint small neighborhoods of all but at most one of them. Equivalently, its doubled Euler traversal has length 2 length(T), and a chain of O(1+length(T)/a) unit balls covers it; each such ball meets only O(1) a-cells. Either argument proves (A1).

For pairwise separated holes, choose these shell neighborhoods disjoint across holes. Then the bound adds:

\[
\operatorname{length}(T)\ge c_1\sum_v a_v R_v^3.
\tag{A2}
\]

An arbitrary specified point in H can be connected to a tree meeting H's halo at cost at most C_1 aR. Thus one interior port per hole costs

\[
C_1\sum_v a_vR_v
\le \frac{C_1}{c_1R_{\min}^2}\operatorname{length}(T).
\tag{A3}
\]

This ratio is unchanged on every later lattice: dividing both tree and port lengths by a new common current-cell length does not change it. It is not necessary to turn each old halo into a new halo merely to retain this inequality.

The port statement is uniform for a fixed number of ports per scalar occurrence. It is **not** a claim that arbitrarily many native derivative evaluation points can all be connected for the same cost. For the source value-localization argument, the defensible interpretation is to use the one original-carrier attachment in the first-nonempty distance factor of (1.66). The number of interpolation maps alone does not bound their derivative orders.

For the final all-order current derivative theorem, the divided-tree weight and the already established Cauchy machinery must be retained. One must not replace it by a stronger undivided m-port tree weight and then charge mR without a budget.

## 3. Exact mixed-mesh coarse-cover lemma

### Lemma A (proved here)

Let the fine grid have cell length a and the coarse grid cell length A=ma, m a positive integer, with compatible partitions. Let X be a union of fine cells. Let H be a finite family of closed, pairwise disjoint holes with positive pairwise gaps. Assume that whenever a hole is declared for X, X contains the whole hole and a positive exterior neighborhood of it.

A fine or coarse cell is called required if it is **not wholly contained in the union of declared holes**. Let X_0 be the minimal compatible coarse-cell cover of X, using cells with positive-interior overlap; do not add all neighboring cells that merely touch X at their boundaries.

Then every required coarse cell of X_0 contains a required fine cell of X. Consequently, if t_a(X;H) is physical length divided by a of a shortest connected tree in X visiting every required fine cell, and t_A is defined similarly, then

\[
 t_A(X_0;H)\le \frac{a}{A}t_a(X;H).
\tag{A4}
\]

#### Proof

A coarse cell C in X_0 contains a fine cell B of X. If B is required, the first assertion is immediate. Otherwise its interior lies in a declared hole H_v. Since C is required, C is not wholly contained in the union of holes. A path in C from an interior point of B to a point outside the holes leaves H_v. Because the holes are a finite disjoint family with positive gaps, the path has points outside every hole arbitrarily close to that first exit. Because X contains a positive exterior neighborhood of H_v, choose such a point in X, and off the fine-grid cell boundaries. Its fine cell B' is contained in C and in X and contains a point outside all holes. Thus B' is required.

Now a fine required-cell visiting tree T in X also lies in X_0. By the first assertion, for each required coarse C it meets a fine required B' contained in C. Hence the same physical tree visits every required coarse cell. Divide its length by A and take infima. QED.

This lemma supplies the exact geometric scale gain; no hole-interior volume is filled. In the YM indexing it gives

\[
 t_k(X_0;H)\le L^{-(k-b)}t_b(X;H).
\tag{A5}
\]

### Scope of Lemma A

- The tree is a genuinely connected physical tree; a quotient metric with free interior traversal would not supply the same physical estimate.
- The exterior-cell convention matters for nonaligned old holes. A partially covered current cell remains required.
- The positive halo must remain attached to the coefficient's support. This condition is established for fresh source nonself interactions and is preserved by support unions. Its preservation under every reconstructed-history definition must be included in the induction.
- The lemma does not identify the analytic coefficient or prove an interaction norm. It is a geometric ingredient for that proof.

## 4. Common-halo cluster joins

For two interaction occurrences sharing an integrated component, their declared supports contain its full halo. Their physical trees each meet a common chosen exterior M-cell. Joining the two meeting points costs at most the diameter of one cell. A spanning tree on q interaction occurrences therefore joins them with at most C(q-1) additional source-cell lengths.

This cost is per occurrence edge, not the component diameter. It can be included in the component-interaction smallness condition. The argument remains valid for repeated occurrences of the same interaction label.

For the two explicit exponentiations, the localization supports are unions, so a common halo is not destroyed merely by taking the connected logarithm. Source (1.90) has unusual connectedness before the first exponentiation, while p.391 switches to ordinary connectedness for the second. The declared input halos and actual union supports should be retained through both choices rather than inferred from the final weaker printed scalar bound.

## 5. Remaining points that must be proved before declaring C-05 closed

### 5.1 Surviving holes outside the newly attempted region

An old scalar can bridge the current attempted component and another old completed component outside it. A newly generated scalar can retain the second component. Dropping that old hole from the exceptional set would require visiting all its interior cells, with a possible R_old^4 cost. Its original shell supplies only an R_old^3 cost. The old hole must be kept, or an actual alternative payment must be displayed.

Original physical halo terminals can be retained without changing their port-cost ratio, by (A3). The fresh new-component halo is not removed by such an outside old hole: current-component separation puts the old hole outside that halo.

### 5.2 Tiny older holes and counting

A current cell cannot be wholly contained in a hole smaller than that cell in every direction. Such holes remove no required current cells. They can be omitted from the current free-hole geometry for the current-cell tree estimate. Multiple tiny historical holes within one current cell do not produce one new normalized kernel factor apiece; the only new normalized slots are the actual components integrated at this operation.

For holes of bounded but nonzero current-cell size, filling a bounded current-cell region may be paid from an original shell reserve, but this payment and its packing have to be stated. Do not enumerate all original fine tags as independent current incidence sites.

### 5.3 Port assignment in the source localization

The repaired proof should explicitly identify the original-tree endpoint in the first-nonempty factor

\[
 d_\Omega\bigl(X,\Sigma_{i_0}\bigr)
\]

of (1.66). If the chosen point of X lies inside a declared old hole, (A3) attaches it to the old exterior tree. Subsequent localization volumes have their own connected-domain requirements. The proof must check that no additional uncharged attachment to an old hole is needed when those domains are joined. Merely saying there are four maps is not enough.

### 5.4 Restoring the source rate

An unchanged old coefficient can retain its original native bound at rate kappa, because it is the same native function on the same declared support. A newly generated coefficient must recover the full rate required for the next operation. Source (1.66) has the scale gain for old births and the improved `(1+4 beta) kappa` input for same-scale ordinary-T births; Lemma A explains the geometric old-to-new gain for the refined norm. The final proof must allocate positive fractions of this reserve to the port, current output, and sums once. It must not pass only `(1-beta) kappa` as the next inductive input at every completion.

### 5.5 Complete source/current matching

Even a successful scalar connector induction must be placed on the actual joint current/native contour, with all ordinary Gaussian/Schur responses and failed-preparation Jacobians retained. The one-load theorem in `primary analysis` controls the current-root sum once the stronger physical component load and operator layers are verified. Pure native-rooted terms and moving retained-data maps are not eliminated by a fixed-current Hessian proof.

## 6. Analysis conclusion

The full-halo mechanism supplies real information absent from the common-spin diagnostic. The shell lower bound, fixed-port restoration, common-halo joins, and exact same-tree mesh conversion are valid under their written geometric hypotheses. The ordinary T identity also supports retention of unchanged coefficient supports.

The remaining task is a complete invariant statement for the actual reconstructed scalar coefficients, including outside surviving holes, source-localization attachments, and the numerical restoration of the analytic/decay budget. These are narrower checks than the original unsupported age inequality, but they must appear in the proof. This analysis does not treat them as proved merely by the validity of the geometric lemmas.

## 7. Scope even if the age estimate is repaired

The submitted Theorem AB17.1 is a **current-anchored** theorem. Its definition is `B_tilde(z,xi)=B_cur(z,xi)-B_cur(0,xi)`, and (AB17.5) quantifies m>=1 current derivatives. Equation (AB17.6) adds native derivatives only to those current-anchored expressions.

The accepted C-04 directional theorem (DS.13)–(DS.16), by contrast, permits the current component of every source direction to vanish. It anchors a local native direction and bounds that derivative of the full corresponding scalar activity. The C-05 statement asks for the same local derivative bounds. Thus an additive scalar `H(xi)=B_cur(0,xi)` is a real logical difference: it disappears from every AW estimate and remains in the outer density.

A repaired CR.22d can complete the current boundary part of (HC.18), together with the stated AW sector/domain inputs. It does not by itself prove the pure-native clause. A sufficient additional argument is to establish the **unsubtracted**, locally native-rooted scalar expansion on the common joint contour and apply directional Cauchy there. The one-load theorem is compatible with this extension if the actual native-coordinate supports and normalized-kernel dependence are identified on the same physical footprint system. Uniform local value control must precede that Cauchy step.

Canonical scalar masses `tau_Y` depend on retained raw fields and may properly remain outside the inner conditional B when those raw fields are fixed. The full C-05 statement does not thereby require arbitrary derivatives of hard selectors or arbitrary later moving raw-data coordinates: those are explicitly separate M-04/M-06/H-04 items in the C-04 scope. What cannot be omitted is the native dependence of the actual scalar B activities that the C-05 statement does include.

## 8. The retained outer reconstruction kernel: verified stronger source mechanism

### 8.1 Exact placement of the gauge factor

LFR II (1.61), p.373, has the form

\[
 U_k^0=U\bigl(B_k''(Y_1),\;v_1(H_k'',u_k^0,U_1)\big|_{C_1},
                  \;v_{\mathrm{interior}}\bigr),
\qquad C_1=(Y_1^0)^c\cap Y_1.
\tag{A6}
\]

The gauge factor `u_k^0` occurs inside the determining input v_1 on C_1. There is no separately multiplying output gauge in this printed identity. The interior entries, explicitly including retained V'' and the indicated averages of U_0^(AL), are fixed during the selective H-localization increments under discussion.

Consequently, writing

\[
 K_1=D_{\mathrm{data}}U(B_k''(Y_1),\cdot),
\]

the derivative of the first reconstruction with respect to H_k'' includes K_1 both for the exponential-field response and for the block-local derivative of u_k^0. The latter is not a direct interior bypass. The source explicitly describes u_k^0(x) as a function of H_k'' on the determining block of x; since x here is in C_1, this enlarges its boundary footprint only by the corresponding block convention.

### 8.2 Later first-nonempty increments

The substitutions (1.62)–(1.64) act through U_1 and then U_{k,Lambda}. If their earlier localization increments are empty, the earlier reconstruction maps remain in the exact expression. Applying the ordinary chain rule therefore retains the schematic leading factors

\[
 K_1D H_k'',\qquad K_1K_2D H_{B_1},\qquad K_1K_2K_3D H_k
\tag{A7}
\]

for the three possible first-nonempty stages, together with the explicitly required local averaging/gauge derivatives inside their boundary input maps. The notation is schematic: the products include those finite derivative factors, and the evaluation points vary along exact interpolations. Earlier empty localization increments do not set K_1 to the identity or erase it.

This is a stronger available fact than the single first-nonempty distance factor displayed in the weakened value majorant (1.66). It is therefore reasonable to retain K_1 before taking that coarse majorant.

### 8.3 Native derivative and current slots

CMP102, printed pp.307–309, Proposition 9 and (190), gives the derivative of the Landau displacement of the reconstructed minimal configuration on its native mixed geometry. The printed bound contains the scaled exponential `exp[-delta_0 d(y,y')/8]`, the output field/gradient/current mesh powers, and the determining-data density factor `(L^{j'} eta)^(-d)`. The latter must be paired with the source's determining-data measure, rather than treated as a counting-matrix entry. Transfer to the axial representative involves the block-local analytic gauge reconstruction in CMP98 (104)–(106), pp.32–33; it is not a literal identification of the two derivative kernels. Its nested paths remain inside the determining block and their normalized path lengths have a bounded geometric sum. This establishes the relevant block locality and absolute gauge response, but does not by itself give the source's strong physical norm for a raw fine axial potential. The composed scalar application must use the admitted inverse-gauge/old-adjoint-field compensator in the declared predecessor interface.

The discussion immediately before Proposition 9 extends these estimates to regular complex external backgrounds. The derivation of (190) explicitly invokes gauge covariance (181), so its scope is not limited to a frozen identity gauge.

The old current slot also follows this reconstruction. CMP109 pp.261–262, (1.15), substitutes the pair `(U_n(M' U), J_n(M' U))` into older activities. Its p.275 explanation after (3.24) explicitly says the shorter notation E^(j)(X,U_j) suppresses E^(j)(X,U_j,J_j). Thus the derivative of an older activity's current slot uses the second-order/current row of K_1. The independently extended new J enters the relevant H-functions and hence the boundary determining data. This does not authorize arbitrary independent changes of every old current slot.

### 8.4 Resident halo grades

A still-resident completed component born at b carries raw V_b data that subsequent ordinary transformations avoid. A one-M_b halo around it has native grade at most b at birth. The next ordinary T step puts multiple current MR layers between this whole old component and the new current region; consequently that thin halo remains outside the newly integrated region and retains its old native grades.

For a later eligible attempt k, resident tag births satisfy b<=h=k-N. The deep part of B_k'' in LFR I (1.17), p.180, leaves the determining layers i<h unchanged. For the borderline b=h, the relevant part of Gamma_h retained on Z''_{h+1} must be used. The thin old halo fits that part because the preparatory construction removes at most the prescribed five layers from the original at-least-ten-layer buffer. The source's allowed R rounding still leaves the next physical MR layer at least as thick as one old M layer. Therefore the sufficient grade inequality is i<=b+O(1), not an unsupported exact equality i=b.

This claim applies to a genuinely surviving component/slot. It must not be used after a component has been consumed and its determining data replaced by coarser new variables. Such contributions require the explicit rebasing/cancellation described next.

### 8.5 Add-back cancellation for consumed slots

Suppose an old-age add-back C_new in A'_k depends only on the new determining data and surviving raw fields, so it is independent of the old variables integrated by Pi. Then

\[
 e^{C_{\rm new}}\Pi\bigl(e^{V_{\rm old}-C_{\rm new}}\bigr)
 =\Pi\bigl(e^{V_{\rm old}}\bigr).
\tag{A8}
\]

This elementary identity permits assigning the consumed contribution to the fresh normalized scalar output, rather than leaving a fictitious old-birth coefficient attached to a new coarse anchor. The source-specific condition is independence from the actually eliminated slots; it must be verified from the new determining-data formulas before using (A8). An add-back still involving surviving integration data cannot be removed this way.

### 8.6 What this stronger mechanism could prove

When a resident halo port has native grade i<=b+O(1), K_1 connects it to the boundary of Y_1, which contains the whole attempted component. The prepared-layer geometry in LFR I (1.47), p.186, then supplies an age cost proportional to `(M/M_1)(k-b-O(1))` in the genuine scaled metric. This is the right type of gain to pay the old root entropy. It is not supplied by a current-grid distance alone.

A complete proof must retain this K_1 factor through the exact old scalar sum, use its native measure convention, and treat consumed/add-back contributions by their actual new labels. The verification above establishes the algebraic chain and the source basis for its rows; it is not a substitute for writing that complete quantitative sum and its induction.

## 9. Exact old-boundary add-back classification

The following source check removes a real ambiguity in the record bookkeeping. CMP119 p.254, (2.1), has

\[
 \Omega_1\supset\Lambda_1\supset\Omega_2\supset\Lambda_2
 \supset\cdots\supset\Omega_k\supset\Lambda_k.
\]

Equation (2.3), p.255, defines \(Z_j=\Lambda_j^c\). Thus, on each admitted determining history,

\[
 Z_b\subset Z_k,\qquad Z_b\subset\Omega_{b+1}^c.
\tag{A9}
\]

CMP119 (2.41), p.261, requires an old boundary carrier to meet \(Z_b\). LFR I p.201, immediately after (1.99), redefines the external region as the old \(Z_k\setminus Z\), and places the histories restricted to every attempted component \(X_i\subset Z\) inside the corresponding component operation (1.100). LFR II p.365, (1.33), independently makes the determining-set replacement explicit: \(\Gamma_j^{\rm new}=\Gamma_j''\cap Z^c\) for \(j<k\), while \(\Gamma_k^{\rm new}=\Gamma_k''\cup Z^{(k)}\). The external large-field-set statement comes from the componentwise history factorization, in addition to this determining-set identity. The action reconstructed as \(A'_k\) in LFR II p.377 is the action on this new external determining history. Consequently an old reconstructed boundary add-back \(B^{(b)}_{\rm new}(X)\), \(b<k\), with \(X\cap Z\ne\varnothing\), also has

\[
 X\cap Z_b^{\rm new}\ne\varnothing,
 \qquad Z_b^{\rm new}\subset Z_k^{\rm new}\subset Z^c.
\tag{A10}
\]

It therefore connects the attempted component to surviving exterior large-field geometry. A consumed-only old boundary add-back supported entirely inside \(Z\) is absent under these source support rules. It is unnecessary, and potentially misleading, to manufacture such a term and then move it into a redefined scalar mass.

The identity \(e^C T(e^{V-C})=T(e^V)\) is algebraically valid for an external \(C\), but it alone gives no norm estimate: redefining the reference kernel multiplies its scalar mass by \(e^C\), whose response remains in the complete density. The quantitative argument should keep the source's canonical \(T'\), its positive reference and its \(\tau=T'1\) unchanged. Old reconstructed B terms are handled by (A10). Ordinary E/R add-backs and same-scale boundary terms retain their separate source budgets. Actual incoming component-self terms remain inside canonical \(T'\) and its source small deformation \(\sigma\).

### 9.1 A precise one-port convention

For a repeated completed-hole occurrence it suffices to attach one physical point \(q\) inside an actually retained component \(H\) of birth \(m\le b\). On its actual history, \(H\subset Z_m\subset\Omega_{m+1}^c\), so this point has native grade at most \(m\), subject only to the source's fixed endpoint convention. For a later eligible attempt \(k\), \(m\le h=k-N\); the deep data are retained by LFR I (1.15)–(1.17). In the endpoint case \(m=h\), nesting gives \(Z_h\subset Z''_{h+1}\), so a point inside the actual old component avoids the previously delicate question about the exact grade of an exterior halo point. Lemma (A3) pays the connector from this interior point to the charged halo tree.

If a record has no completed free hole, its full carrier tree supplies a point meeting its ordinary source boundary set, with a bounded endpoint cost. For a reconstructed old B add-back, (A10) gives the exterior bridge. For newly completed outputs, a retained failed component supplies a new same-scale whole halo; an exterior surviving old component supplies its actual physical port; and an output disjoint from all retained components has its full carrier tree restored by the successful-component estimate before LFR II (1.95), followed by (1.99)–(1.100). These are the source's actual alternatives.

The quantitative invariant should be uniform for the choice of **one** required port per scalar occurrence, or use the union of actual already-paid input trees. It should not demand a tree through arbitrarily many tiny historical tags introduced merely by a coarse cover and charge only a fixed constant. The one-port convention is sufficient for the K_1 concatenation and does not create such multiplicity.

## 10. Analysis of the composite tree/K_1 age bound

With an actual resident point of grade at most \(b+O(1)\), the proposed inequality in `Conditioning, deletion and mass factors for the retained history`, (H10), is a valid geometric route:

\[
 C_T(M/M_1)t_b+d_{\mathcal B''(Y_1)}(x,C_1)
 \ge c_T(M/M_1)(k-b-c_1)_+-C'_T.
\tag{A11}
\]

The old full physical connector joins the resident point to an attachment \(x\); the retained outer reconstruction joins \(x\) to \(C_1\). Their concatenation crosses the prepared annuli. On the portions of the old connector in grades at least \(b\), the scaled metric density is bounded by a fixed multiple of \(h_b^{-1}\); lower-grade portions need not be bounded by this coarse density. Complete higher-grade annulus crossings are nevertheless unavoidable. This is precisely why concatenating the two paths is stronger than replacing the original map by a current Euclidean distance.

The derivative is used to bound a **value difference** along the actual admitted source interpolation, before Cauchy in localization parameters. Its two fixed data sets must remain fixed as in (1.61). For all-empty localization branches, an exterior nonself carrier itself connects the resident region to the exterior; wholly interior self terms belong to the canonical component kernel and its published native deformation estimate. The method must not apply a nonempty K_1 factor to a branch in which there is no such difference.

Splitting positive source reserves yields an age exponential strong enough to pay the explicit \(L^{4(k-b)}\) old root density if the decay parameters are fixed in the source order. CMP102 (190) contributes rate \(\delta_0/8\), not \(\delta_0/2\). The input density normalization and the remaining multiscale row bound are both required; canceling mesh powers alone is not a proof of a uniform row sum.

These checks resolve the specific abstract port/cancellation objections to the proposed scalar recurrence. They do not on their own assert the full C-05 native derivative theorem described next.

The numerical current application still needs the complete scalar row `DE times K_1` in the actual admitted gauge/current chart, including the old current argument and the old adjoint-field convention. It is insufficient to replace this by a bound on the Landau H field alone. The claimed fixed polynomial and fixed exponential profile loss must be derived from or explicitly matched to the already proved converter bounds; writing an unnamed `Gamma_dom` does not establish that match. Once that scalar estimate is supplied, the displayed geometric reserve split and chronological contraction are available without an additional abstract cluster theorem.

## 11. Pure-native derivative scope remains a separate explicit check

The source directions in C04 (DS.13)–(DS.16) may have zero current component. AW (AB17.2) defines the native external field norm by a supremum over **all actual native layers**, including old strata, with the field, first derivative and current weights. Thus this is not merely a perturbation of the current determining variables at the outer boundary \(C_1\).

A native perturbation supported inside a retained core can change the `D_fixed` arguments of (1.61). The K_1 proof above holds those arguments fixed and varies the outer determining data. Its age gain therefore cannot be assigned automatically to every pure native direction. This is not an obstacle when a full unsubtracted **value** estimate has already been proved uniformly on that native contour: in that case Cauchy is applied afterwards, and no separate K_1 factor in the native derivative is needed. The published (2.42) native bound controls each scalar at its native scale, and (2.48) controls an extensive total. Neither statement alone is an all-depth local anchor sum for the unsubtracted scalar on the joined native contour.

A concrete sufficient remaining bound is the following. For a localized expansion of the full unsubtracted boundary scalar

\[
 B(z,\xi)=\sum_\Gamma F_\Gamma(z,\xi)
\]

on the common joint contour, with actual native dependency supports \(S_\Gamma^\xi\), prove

\[
 \sum_{\Gamma:S_\Gamma^\xi\cap S\ne\varnothing}
 e^{\gamma\operatorname{diam} S_\Gamma}\|F_\Gamma\|_D
 \le J_{\rm nat}\,N(S)
\tag{A12}
\]

uniformly in depth, volume and admitted histories, with the same local support-count convention required by DS.16. Then the exact directional Cauchy argument gives

\[
 \sum_\Gamma e^{\gamma\operatorname{diam} S_\Gamma}
 |D_{h_1}\cdots D_{h_m}F_\Gamma|
 \le e^m m! J_{\rm nat}N(S_1)\prod_{a=1}^m q_a.
\tag{A13}
\]

The one-load transfer in `primary analysis` can also prove (A12) if the native supports and native kernel layers satisfy its physical extent and bounded-overlap hypotheses. That extension is promising, but the actual native map must include interior-data responses. Terms with empty integrated support, especially \(H(\xi)=B(0,\xi)\), require their own scalar root norm in this calculation. A current-root theorem, even with arbitrary mixed native derivatives afterwards, does not constrain such a term.

For the fresh source-localized V(Y) terms, the exact native dependence on U,J restricted to Y is useful: with the full scalar component load already established uniformly on the joint contour, the spatial root argument may be repeated at native support points in the ambient mesh. The unresolved conclusion must not be inflated to claim that all those fresh terms require a new native age theorem. The precise remaining issue is the full native-rooted expansion, including external persistent terms and the actual map from native source directions to those support sets.

Canonical raw masses remain in their exact outer roles. This check does not request arbitrary derivatives of old selectors or arbitrary nonlinear retained-coordinate maps; those remain the separate matching/interface items explicitly excluded from C04's admitted analytic-slot scope.

## 12. Scalar-row analysis: the restricted boundary/interior repair holds

**This section refines the scalar-interface status at the end of Section 10.** The argument is Section 13.10 of [Conditioning, deletion and mass factors for the retained history](history_masses.md) and Sections 7–8 of [Age dependence of the outer reconstruction](reconstruction_age.md). The arbitrary refined-data claim of Section 13.8 of the former note does not hold in that generality. The following restricted scalar statement holds at the stipulated AO–AR, NP.5, AD17.26–AD17.28 and PF common-chart scope.

The difficulty was real. The localized determining history in the outer boundary layer can refine an original grade. A derivative estimated in that finer output normalization cannot automatically be regarded as a tangent in the old primitive's strong ball. Neither the cancellation of the determining-data measure nor analyticity alone proves that conversion.

The repair splits the **whole** primitive dependency carrier, including its actual old-node and stencil collars. If this enlarged carrier reaches the outer disagreement collar, its old connector from a true resident port already crosses the intervening prepared grades. The scalar value estimate `|E(Phi_1)-E(Phi_0)| <= 2 ||E||` then suffices. No refined-output tangent estimate is used on that branch. Reconstructed old boundary add-backs have the exterior owner proved in (A10), so the same bridge alternative applies.

In the other branch, all relevant output points lie where the localized history agrees with the prepared history. Preparation only coarsens the original grading there. If `i` is an original output grade and `n` its prepared grade, then `i <= n`; the old primitive's innermost convention also gives `i <= b`, where `b` is its scalar birth. There is no universal ordering `b <= n`: both `n <= b` and `n > b` occur and are treated separately in the concatenation.

Use the fixed **absolute** determining-data ball of CMP102 (172), rather than imposing an unproved refined input bound proportional to `alpha_s`. Proposition 9 and the printed (190), pp.307–309, give decay `exp[-delta_0 d/8]`. The density `h_s^{-4}` is paired with its actual source measure. CMP96 Lemma 2.1, (2.59)–(2.61), supplies the remaining absolute native-center row sum; cancellation of mesh powers alone would not supply that sum. Thus, for the output rows of physical orders `p=1,2,3`,

\[
 h_n^p|D\,\mathrm{output}_p(x)|
 \le C e^{-\delta d(x,C_1)}.
\tag{A14}
\]

The exact source datum includes the gauge and averaging factors in (1.61). Those factors remain inside the outer determining input; they are not a separate output rotation. The finitely many later reconstruction maps alter fixed constants and fixed inverse-coupling powers, while retaining the outer `K_1` in every nonempty branch.

For old native normalization the admitted AF comparison gives

\[
 \alpha_i^{-1}(h_i/h_n)^p
 \le Cg_k^{-1}(1+k-i)^aL^{-p(n-i)}
 \le C_p g_k^{-1}(1+k-n)^a.
\tag{A15}
\]

The last inequality follows from the finite supremum of `(1+n-i)^a L^{-p(n-i)}`. The polynomial in `k-n` is paid by a fixed reserve of the prepared distance in LFR I (1.47). If `n>b`, the old connector supplies the grades from `b` to `n`; if `n<=b`, the `K_1` path already supplies the required `k-b` gain. This is a genuine fixed inverse-coupling loss, not a uniform constant and not an age-dependent analytic radius.

The scalar gauge transfer also has the required source match. CMP102 Proposition 2, p.281, treats the nonzero corrected fiber `Q(U_0,eta A)=B` with terminal normalization `R_0 u_j=1`. The algebraic inverse-gauge formulas RM.26–RM.36 do not assume `B=0`. They therefore apply to the actual first reconstruction with its fixed real reference. Recent old adjoint fields in the preparation strips have been integrated out. The borderline surviving `A_{h-1}` is supported in `Omega_h intersection Z_h`, and `Z_h subset Z''_{h+1}` keeps its terminal grade at most `h`, up to the fixed endpoint convention; deeper old slots retain their grades. The old-node converter AD17.26–AD17.28 and retained-raw extension CR.2 then turn (A14)–(A15) into the fixed-old-variable scalar tangent. This argument does not assert a strong physical bound for a raw axial potential.

The domain qualification must remain explicit. PF.1 places the declared strong core inside the modified source domain; it does not identify every point of that entire modified domain with an NP.5 ball. CMP116 (1.11), (1.18) introduces only the fixed enlargement `exp(16 kappa_1)`. Choose the fixed native/core reserve after that constant, and then the common coupling ceiling; `q>p_0+r+2` pays the prefix real-center enhancement. Keep the **full** authorized localization-parameter disks and physical current contour. The permitted reduction is a fixed native/core reserve, not a silent shrinkage with age or a deletion of part of the current support.

At this scope, apply the genuine directional Cauchy disc to the composed scalar, integrate the actual selective interpolation, and only then apply the source localization-parameter Cauchy estimates. The resulting bound has the form

\[
 \|\Delta E_X\|
 \le C g_k^{-a}(1+k-b)^s e^{-\Gamma(k-b)}
       \mathfrak a_b(X),
\tag{A16}
\]

where `a,s` are fixed and `mathfrak a_b` retains the unused old-carrier reserve. The age exponent can pay the actual `L^{4(k-b)}` birth-root density after a strict reserve is chosen in the source parameter order. This resolves the particular scalar `DE K_1` interface from Section 10. It does **not** establish a bound for arbitrary independent fine-data tangents, arbitrary moving retained data, or all pure-native directions.

Two further scope points prevent a false conclusion. First, the deliberately crude factor `g_k^{-a}` in (A16) cannot be used to prove that the canonical self deformation is small: `g_k^{-a} A_*` need not tend to zero. Keep the separate exact source self estimate (1.71)–(1.75). Second, an exact scalar-first construction can integrate the native kernels before taking current derivatives. Native operator holomorphy, the complete scalar expansion and its actual gauge covariance suffice for that route; scalar differentiation then includes all normalized-kernel response. A separate arbitrary-test-function covariance theorem for a pulled-back current kernel is useful for a marked or operator-layer approach, but is not an additional unavoidable C-05 requirement.

## 13. What remains of the final-carrier issue in a weaker quotient norm

The full physical-connector transfer called **FH** in [Conditioning, deletion and mass factors for the retained history](history_masses.md), Section 13.9, is a sufficient strengthened invariant. It is not itself part of the C-05 statement. The original polynomial rooted quotient norm (CR.10) may suffice instead. The distinction matters for the last proposed alternative.

### 13.1 The quotient age observation is valid

Let the only zero-cost footprints attached to a birth-`b` occurrence be genuine completed components `H_m` of birth `m<=b`, with their actual source grading. By (A9), each lies entirely in native grades at most `m`, with the fixed endpoint allowance. Assigning zero traversal cost inside these footprints therefore cannot remove any complete crossing of a grade greater than `b` (or greater than `b+c_0` with the endpoint convention). Concatenate a quotient connector from a true resident footprint to the scalar evaluation point with the actual outer `K_1` path. The same high-grade crossings used in (A11) remain paid.

This observation removes the shell `R^3` payment from the **age** argument when this exact weaker norm is used. Quotient connectors are also subadditive when two interactions share the same fixed component. Physical diameter can then be recovered by the separated-component estimate CR.6, with one remaining component diameter paid by the separately extracted current collar. An already promoted larger footprint cannot be inserted into this argument under the old birth label unless its grade property is re-established; the grade conclusion is about the genuine declared footprints.

### 13.2 An elementary positive saturation pushforward

Here is the precise abstract fact a weaker route can use. Let `a_eta>=0` be actual pre-completion majorants. Suppose a deterministic support saturation `S` gives completed coefficients

\[
 b_Y=\sum_{\eta:S(X_\eta)=Y}a_\eta.
\]

If the target quotient cost obeys

\[
 \ell_{\rm out}(S(X_\eta))\le\ell_{\rm in}(X_\eta),
\]

then for every rooted class `R`,

\[
 \sum_{Y\in R}b_Ye^{\lambda\ell_{\rm out}(Y)}
 \le \sum_{\eta:S(X_\eta)\in R}
       a_\eta e^{\lambda\ell_{\rm in}(X_\eta)}.
\tag{A17}
\]

This is immediate from positivity and contains no cancellation. If the preimage of a root is covered by `P(R)` genuine input roots, an input rooted norm yields at most the factor `P(R)`. At a current completed component the intended factor is polynomial in its current size; the old-grid factor `L^{4(k-b)}` must still be paid by (A16). Actual occurrence coefficients and normalized-kernel factors must remain in `a_eta`.

If saturation adds only subsets of atoms that are already entirely free in the target metric, the geometric cost inequality in (A17) holds: extend the input tree through those atoms at zero cost. This proves an abstract alternative to a full halo-visiting majorant.

### 13.3 The actual source matching is still unfinished

If only the genuine component `H` is free, the source completion by its positive enlargement `H^~` adds exterior terminals. Their quotient visiting cost is not bounded just because the interior `H` has been made free. Thus (A17) does not apply automatically in that convention.

If the whole enlargement `H^~` is made free, the elementary saturation inequality does apply, but the source-specific induction must prove that these enlarged atoms retain all of the required properties: a native grade bound up to a fixed shift; mixed-age separation and bounded aspect ratio; whole-footprint absorption under later attempted components; and a polynomial root-preimage count on the actual source mesh. It must also retain the nonself small factor, exterior entropy reserve and canonical normalized-operation factors. Declaring arbitrary enlarged halos free without these checks can merge components, remove paid crossings or conceal root multiplicities. Using uniformly thin birth-mesh halos is a plausible way to satisfy the geometry, but that exact all-history positive pushforward has not been established here.

The two-majorant/Hölder lemma (H29)–(H30) in `Conditioning, deletion and mass factors for the retained history` is correct. It can combine an age estimate and a final spatial estimate when they bound the **same positive birth-resolved occurrence coefficients**. A bound on the norm of their signed, resummed scalar sum does not supply either of those positive coefficient sums. The same distinction applies to the weaker pushforward (A17).

The final status is therefore precise: the structural add-back/port theorem and the restricted scalar age channel are established at their stated source/predecessor scope. The current-root route still requires either FH **or an adequate weaker positive quotient/saturation transfer for the actual completed coefficients**. The unsubtracted native-root estimate (A12), including the persistent `H(xi)` sector, is independently open. Neither the abstract shell lemmas nor the quotient age observation alone closes those two remaining requirements.
