# M-04: residual old-energy trial normalizers

This records a source-specific limitation of a proposed constrained-partition proof. It does not supply the normalized residual old-energy upper bound still needed by M-04.

## 1. What the residual native energy can pay

On an active residual component, the final failed fresh selector forces a current native curvature witness on its complete determining footprint; see Proposition AH.1 in [active history test](../E_limits_and_targets/active_history_test.md). Its dimensionless Wilson energy is at least cP(g_k)^2. An eligible component has current volume at most C R_k^4, and the cutoff exponents satisfy p_0≥5r when P(g) is proportional to [log(g^{-2})]^{p_0} and R(g) is comparable to [log(g^{-2})]^r.

Therefore a cost C R_k^4 log(g_k^{-2}) is smaller than any fixed positive fraction of P(g_k)^2 for sufficiently small g_k:

\[
 \frac{R_k^4\log(g_k^{-2})}{P(g_k)^2}
 \le C[\log(g_k^{-2})]^{4r+1-2p_0}\longrightarrow0.       \tag{RN.1}
\]

This would pay an entropy loss proportional to the **current** number of degrees of freedom in Y. It does not prove that all old conditional entropy has that size.

## 2. The retained chronological age is R, not log R

LFR I printed p.177 requires an eligible component to have no new bad field in its last N steps. The preparatory coarsening length N_0 on p.179 is determined by

\[
 L^{-N_0+1}R_{k-N_0+1}=1.
\]

Thus N_0 is of order log R. This should not be confused with N. LFR II printed p.384, immediately before (1.80), sets the chronological quiet period to **N=R_j** in the inductive construction. LFR I p.198 independently requires N to be a positive power of log(g_k^{-2}) to pay the inherited boundary estimates. The text explicitly assumes N much larger than N_0.

The old operation in LFR I (1.76) still includes the core T_h, h=k−N; p.194 says that this first old-core integral is left unchanged. Two distinct counts must be kept separate.

For each of the **last N** scales, eligibility condition (i) bounds the region in its own lattice units by a cube of side 100MR_j. Thus the remaining independent coordinates from those scales satisfy the conservative bound

\[
 D_{\rm quiet}\le C_M\sum_{j=h}^{k}R_j^4
       \le C_M N R_k^4\le C_M R_k^5,                   \tag{RN.2}
\]

on the short small-coupling interval of a first eligible quiet history. Here the source trajectory gives comparable R_j across N=O(R_k) steps. Already integrated variables are not counted again. In particular, **N=R does not imply L^{4N} surviving rank for a fresh local seed**. An inference from the size of the current prepared core to such a rank is too broad.

Consequently its elementary compact trial entropy is affordable:

\[
 \frac{R_k^5\log(g_k^{-2})}{P(g_k)^2}
    \le C[\log(g_k^{-2})]^{5r+1-2p_0}\longrightarrow0,  \tag{RN.3}
\]

for the source's positive integer r and p_0≥5r. The source's coarser chronological domain-cost bound can include a further factor R, giving O(R^6); this is also paid by P^2 under that exponent inequality.

In contrast, the **unchanged T_h** may contain arbitrary earlier history. Eligibility does not bound the native coordinate count of all that earlier history by current volume. For example, a large earlier component can shrink to a small h-scale component before the final quiet window. Any rank loss from those genuinely surviving coordinates must be treated through its actual old Gaussian and normalization factors. NR20.7–NR20.9a explicitly retain and pay that old-scale sum in unnormalized estimates; they do not replace it by |Y|.

An elementary trial-ball lower bound of the form

\[
 Z_{\rm old}\ge e^{-C E_{\rm trial}}(c\beta^{-1/2})^{D_{\rm old}}
\]

therefore produces a loss D_old log β. The contribution of D_quiet is controlled by (RN.2)–(RN.3). No bound of this kind for the whole earlier T_h follows merely from the current size of Y or the small prepared core.

This is a limitation of a direct trial in an arbitrary fixed older branch, not a lower bound on the actual normalized old energy. In the **full** residual history sum the denominator may instead be bounded below by restricting to one younger admissible history with the same actual retained output descriptor. This is a useful route, provided the replacement history really has that descriptor and the prior renormalized density is included.

## 3. Two additional restrictions on a trial prolongation

First, a uniformly small minimum-energy prolongation need not be an admissible point of a specified old history. The old base includes the actual birth selectors and all preparatory labels. Replacing them by all-good constraints changes the partition function. A source-specific trial configuration has to realize the retained geometric event and all still-conditioned old selectors, or else integrate their true posterior rather than conditioning on an invented event.

Second, the source upper mass bound for a component is not a lower bound for its old normalizer. The fresh denominator has a separate lower bound in LFR II pp.357–358, (1.7)–(1.11); it concerns the current prepared core, with an O(M^4) Gaussian dimension. It is not the normalization of the old T_h operation in (1.76), and it cannot be substituted into that old quotient.

## 4. A concrete remaining approach

One possible route is to condition on the retained current shell, construct an admissible old coarse-to-fine extension, and compare the **complete old normalized Gaussian/coarea measure** to a uniformly controlled reference centered at that extension. Such a comparison must show that all vacuum and determinant terms cancel at the level of the same restricted old normalizer. It must then pay the selectors with the actual rank count.

A second route is to use the old history sum itself. For a given eligible Y and prepared core, attempt to create its h-scale rectangle by finitely many fresh pure-gauge Q seeds at h, then follow the same quiet S^N geometry. This would replace complicated pre-h internal history in the **trial subset of the denominator**, not change the full law. The same prepared core and fresh graph must be preserved; a trial on another singular output stratum contributes zero to the required lower bound. The local seed cost of NR20.26 is O(P(g_h)^2), and (RN.2) makes the subsequent quiet-window entropy polynomial and affordable. The unresolved source-specific part is a lower bound for the complete pre-h renormalized local density and its exact normalization, conditional on the same retained exterior, together with realizability of the required h-scale rectangle and prepared core.

If this yields the actual logarithmic mass bound \(-\log m_Y(v)\le C[1+E_{\rm native}(v)]\) after the fixed source normalization is accounted for, then NR20.18 immediately gives

\[
 \|\mathcal F_Y^\natural\|_{L^p(\nu_{Y,v})}
       \le C[1+E_{\rm native}(v)+p].                   \tag{RN.4}
\]

There is no exponential inverse-mass cost in (RN.4); the reserve is converted into a tail bound and the lower mass enters through its logarithm. The full native-energy dictionary and strong currents/carriers remain separate even if this moment estimate is obtained.

There is no elementary counting contradiction to that last payment. A normalized Gaussian estimate can make a bad-cutoff union bound of size

\[
 D_{\rm old}e^{-cP(g)^2}
\]

small for the last quiet window, and even for some much larger old ranks. But a tail union bound alone does not compare the complete interacting old partition function with its marked energy numerator; its Gaussian center, covariances, history restrictions, and vacuum normalization must be the actual ones. Establishing that source-specific comparison remains open.

## 5. Earlier replacements do not bound all possible pre-R genealogy

The completed R operation does erase the old interior on residual eligible components as well as successful ones. LFR II (1.33)–(1.35), printed p.365, replaces the determining data throughout the eligible Z by the current k-grid field, retaining the older data only outside Z. The old internal residual variables are integrated in T'_k(Y), and HS20.4 completes that old-state average. The later residual test does not undo this integration. Thus a component which actually underwent a previous R operation does not carry its pre-R raw interior into the next primitive state merely because the fresh component was residual.

This fact does **not** give a polynomial rank bound for every component at its first R operation.

### Proposition RN.2 (arbitrarily large pre-R native genealogy is allowed)

Within the displayed soft-gauge source convention there are positive primitive histories which first become eligible at a current scale k, whose last quiet-window rank is bounded as in (RN.2), but whose unchanged earlier T_h contains arbitrarily many surviving old raw compact coordinates and ordinary old Gaussian boundary coordinates compared with any fixed polynomial of current R_k.

**Construction and proof.** On the initial lattice, choose one large rectangular array of the strict pure-gauge Q1 seeds from NR20.4. Put a seed at an interior noncentral fine vertex of each selected test cube, with enough such cubes to make the padded bad region one connected rectangle. The gauge transformations remain equal to the identity at every first-block center. Their product is again a pure gauge, so every fine plaquette and the first coarse field equal the identity. All Q1 inequalities defining the selected array have strict margins; the physical P0/P1 tests are good. The soft-gauge density is positive. The strict inequalities persist on a positive-volume/coarea neighborhood.

Set all subsequent current fields to the identity and all true regular fluctuations to zero. Every new P,Q,R selector is good. The single rectangle evolves by the exact S map of LFR II p.384. Its initial size can be chosen so large that it fails eligibility condition (i) for an arbitrarily long interval. Because R acts on eligible **whole connected components**, there is no earlier replacement of this one component or of a hypothetical subcomponent of it. The source's ordinary operations do not integrate its original bad interior; that interior remains inside the growing physical bad region.

One can keep this example on a short-coupling plateau without relying on a long running-trajectory estimate. Choose g in the interior of a rounded R interval, take an earlier age H=R^2, and use an initial rectangle of fine-grid side comparable to L^H MR. Since g^2(H+R) tends to zero, the source one-step coupling bound keeps R_j=R throughout H+R steps when the plateau is chosen with margin. The rectangle cannot satisfy the size test until scale H+O(1). Its initial boundary free-coordinate count grows at least like a fixed positive multiple of L^{3H} times a polynomial in R. This is already larger than every fixed polynomial in current R. The torus and cutoff can be chosen large enough; in final current physical units the initial rectangle has size O(MR L^{-R}), so a fixed macroscopic torus is also compatible.

Let k be its first eligible scale and put h=k−N for its actual qualifying quiet window. Existence of such a scale under repeated S is the chronological statement proved at LFR II (1.80). This choice also handles a possible intervening rounded change of R_j; no monotonicity of the size ratio is presumed at the first instant when (i) alone holds. Every one of the last N regions now has the required size. The old physical rectangle has become very small in current units, but its original fine fields have not disappeared. LFR I (1.10) leaves all regions with j≤h unchanged in the preparatory construction, and p.194 leaves T_h unchanged in (1.76). The raw compact coordinates of the initial rectangle therefore remain in that old integral. Its ordinary first-step boundary annulus also contains arbitrarily many disjoint complete free blocks; each contributes a fixed positive number of physical Gaussian degrees of freedom after axial and averaging constraints. Hence the surviving Gaussian rank as well as the compact coordinate count can be made arbitrarily large by increasing the initial rectangle and the cutoff depth.

The final fresh component can be residual: keep its shell flat, so the exterior-extension selector is strictly good, and choose a small physical non-tree fresh fluctuation inside its prepared core. The source's M_0ε_k link cutoff is much larger than the final ε_k curvature test. A continuous increase of this fluctuation gives a strictly failed final local curvature test while staying strictly inside the fresh cutoff and the regular reference chart. The fresh gauge-slice density is positive there. Thus the construction also reaches an active residual Y, not only a successful first replacement. QED.

The assertion is about what coordinates occur in the **pre-R conditional integral**. It does not say that an old history with huge rank has substantial posterior probability, and it gives no divergence of a normalized marked moment. Its actual small mass is precisely what the chronological source extraction retains. It shows why a uniform rank bound cannot replace that integration in the normalization problem.
