# M-04: residual gauge strata and active conditional versions

Theorem RS.5 below proves a finite-cutoff continuity obstruction for the actual residual descriptor mixture in HS20.4. It is for the **descriptor-erased output** consisting of the new current field, retained residual Y geometry, and unreplaced exterior. It tests a local scalar of the old current field immediately before R. It does **not** identify that native scalar with the already transported microscopic M-04 scalar. The source preparation and the stated scope are analysed further in [residual strata analysis](residual_strata_analysis.md).

HS20 also permits a newly resampled internal descriptor to be retained. Such an enriched output can separate the strata by a discrete coordinate; an ambient extension may then depend on that coordinate off support. The erased-output continuity obstruction must not be asserted for every such augmentation. Section 9 gives the exact finite algebra of this constructive lift, with the remaining quantitative and regularity obligations stated separately.

## 1. The specific source mechanism

LFR I (1989), printed pp.192–194, defines the prepared replacement domain

\[
 \Lambda_\gamma=(\Omega_{k_0+1}^{-4})^c\cap Y,
 \qquad k_0=k-N_0.
\]

It is a rectangular union of current M-cubes, contained in a cube of side 100M. Its location and shape depend on the old domain sequence. Printed p.194 explicitly says that the regions of integration usually differ for terms in the sum. LFR I (1.100) then introduces a fresh axial graph \(G_\gamma\subset\Lambda_\gamma\) and the fresh factor

\[
 k_\gamma(du'\mid v_\gamma)
  =H_\gamma(v_\gamma)^{-1}
    \delta_{G_\gamma}(V'_k)\,
    \chi_\gamma(V'_k)\,
    e^{-g_k^{-2}A(\zeta,U_{k,Y}(V'_kV_{\Lambda_\gamma}))}
    \,du',
\]

where \(V_{\Lambda_\gamma}\) is the reference minimizer determined by the shell outside \(\Lambda_\gamma\). Proposition 1, (1.77)–(1.78), makes this orbit depend on that shell rather than on an unintegrated old continuous variable. The axial representative is fixed at p.197, (1.83).

On successful components the fresh gauge factor is removed by the positive Haar restoration described in HS20 §1. On residual components it remains, together with the descriptor-dependent exterior-extension selector \(\chi_{k,\Lambda_\gamma}\), the fresh cutoff, and the final residual test \(\chi_k^c(Y^6)\). Thus different residual descriptors can supply different singular measures on the same full current-field space over Y. HS20 handles this correctly by first including the shell Haar measure and then taking a finite positive mixture of the resulting full-Y descriptor measures.

At fixed \(\gamma\), the literal old conditional is independent of the fresh field:

\[
 Q_\gamma F(u',v_\gamma)
   =\frac{\int F(u,v_\gamma)\rho_\gamma(du,v_\gamma)}
          {\int\rho_\gamma(du,v_\gamma)}.                 \tag{RS.1}
\]

After erasing \(\gamma\), the fresh density enters the posterior. It cannot be canceled between different descriptors. In particular, replacing the actual residual mixture by a product of separately normalized old laws would remove the mechanism being investigated.

## 2. A measure-theoretic active-version criterion

### Proposition RS.1

Let \(\mu=\sum_{\gamma=1}^J \mu_\gamma\) be a finite positive output mixture on a finite-dimensional smooth ambient field chart. Assume each \(\mu_\gamma\) has a locally bounded density with respect to smooth surface measure on its smooth support stratum \(S_\gamma\), positive almost everywhere on the patches used below. Let \(f\ge0\) be an incoming mark and let \(m_\gamma\) be its conditional mean on descriptor \(\gamma\).

Suppose there are two strata, a common point \(v_*\) in the closures of their positive-density patches, and constants \(c,r>0\), such that:

1. on a full-surface-measure subset of \(S_1\cap B_r(v_*)\), the posterior mean of f is at least c;
2. on a full-surface-measure subset of \(S_2\cap B_r(v_*)\), that mean is a continuous function \(\phi(v)\) with \(\phi(v_*)=0\);
3. the full-surface-measure subsets in (1) and (2) have points arbitrarily close to \(v_*\).

Then the conditional mean of f has no ambient continuous version agreeing \(\mu\)-almost everywhere. In particular it cannot have a finite combined direct/current M-03 norm on that chart.

**Proof.** If an ambient continuous version \(g\) existed, its equality almost everywhere with the conditional mean and positivity of the chart densities would imply \(g\ge c\) on a dense subset of the first patch and \(g=\phi\) on a dense subset of the second. Taking sequences from the two sets to \(v_*\) yields both \(g(v_*)\ge c\) and \(g(v_*)=0\). This is impossible. The finite-cutoff local-Lipschitz implication of the M-03 direct/current norm is proved in [support analysis](support_analysis.md), Proposition 2.1. QED.

The common intersection need not itself have positive output mass. Changing values on that intersection, or on any other null set, does not change the conclusion. This is the distinction from the default inactive-fiber jump already established in [support analysis](support_analysis.md).

### Useful finite-mixture verification

If \(S_1\) has a descriptor with strictly positive old normalizer, strictly positive old expectation of f, and positive fresh density near \(v_*\), then its contribution supplies the constant c in condition 1, provided the total density of the descriptors sharing its stratum is bounded above there. Descriptors with distinct smooth strata contribute zero Radon–Nikodym density on the generic part of \(S_1\), except when the strata coincide on an open patch. A descriptor supported on a larger-dimensional stratum also gives zero mass to \(S_1\). All these statements concern the full shell-plus-slice measures, not gauge deltas treated as pointwise functions.

For condition 2, it is enough that every descriptor with nonzero Radon–Nikodym weight at generic points of \(S_2\) leaves the support of f unreplaced. Then (RS.1) gives its exact retained value \(\phi(v)\), and summing the posterior leaves that value unchanged.

## 3. Why separated replacement cores would identify the reset mask

Take a current Wilson scalar \(\phi_x\ge0\) on a fixed local plaquette stencil P_x. Suppose P_x lies deep in \(\Lambda_1\), while \(\operatorname{dist}(P_x,\Lambda_2)>200M\). Every eligible prepared core has diameter at most 100M in the coordinate-wise maximum metric, so any core that touches P_x is disjoint from \(\Lambda_2\).

Let \(S_2\) be the fresh gauge stratum of descriptor 2. A fresh gauge transformation supported inside a core \(\Lambda_\gamma\) touching P_x, and fixed on its exterior, changes the tree constraint of descriptor \(\gamma\). It leaves the support equations defining \(S_2\) unchanged: the two cores are disjoint, and covariance of the reference minimizing orbit implies that a shell gauge transformation equal to the identity near \(\Lambda_2\) does not change its fixed axial reference there. Consequently the constraint equations for \(S_\gamma\) are not identically satisfied on an open patch of \(S_2\). On the small regular analytic chart, their intersection has zero \(S_2\)-surface measure. A finite union of these intersections is still null.

Thus, at generic points of \(S_2\), no positive posterior descriptor resets a bond of P_x. Successful components cannot cause an exception, since they are disjoint from the retained residual Y. Other residual components are also disjoint. On this generic set the exact conditional mark is simply \(\phi_x(v)\).

This argument requires an actual pair of positive descriptor patches with the stated geometry. It does not manufacture such patches merely from the fact that arbitrary rectangular reset domains could be written down.

## 4. A source geometry lemma for equal outer regions

The exact no-new-bad-field region map S is stated in LFR II, printed p.384: cover the old MR_j-cube region by the smallest union of next-scale LMR_{j+1} cubes, then add ten layers. On a rectangular component and in fixed physical coordinates, let a_j denote the physical mesh of those region cubes. The meshes are nested; each ratio a_{j+1}/a_j is an integer under the source's discrete choice of R_j. In one coordinate the left and right endpoints obey

\[
 \ell_{j+1}=a_{j+1}\bigl\lfloor\ell_j/a_{j+1}\bigr\rfloor-10a_{j+1},
 \quad
 r_{j+1}=a_{j+1}\bigl\lceil r_j/a_{j+1}\bigr\rceil+10a_{j+1}.    \tag{RS.2}
\]

### Lemma RS.2

For a translated birth rectangle with fixed side length, after finitely many maps (RS.2), translating its initial left endpoint through one final-mesh period produces at most two endpoint transition locations. Consequently there is a subinterval of length at least one third of the final mesh on which both final endpoints are constant. Intersecting with the birth lattice loses at most two birth meshes in its length.

**Proof.** Nested integer meshes imply by induction that each final left endpoint is the final mesh times the floor of an affine function of the initial translation, with slope the reciprocal of the final mesh. The padding changes only the additive constant. The same statement holds with ceiling for the final right endpoint. Each of those functions has at most one jump in a final-mesh period. Their two transition locations cut that period into at most three intervals. At least one has the claimed length. QED.

Apply the lemma in one coordinate and hold the other coordinates fixed. A final current region mesh is MR_k. For large enough R_k, a constant-output interval contains birth seeds separated by more than 400M in current coordinates. The prepared cores contain the old seed region and have coordinate-wise diameter at most 100M, by LFR I (1.10)–(1.12), (1.73). Thus the corresponding prepared cores are separated by more than 200M, while their final Y rectangles agree.

This is a statement about the source's allowed geometric operation. The positive field realization of both descriptor sequences and their common residual output patch is supplied in §§6–8; it is not inferred from geometry alone.

For the existence construction it suffices to use an especially simple admitted segment: choose the weak coupling away from a rounded R threshold, so R_j=R throughout the N=R quiet steps. The one-step source coupling bound gives a change O(g^2R) in the relative inverse-coupling scale; this tends to zero as g tends to zero. Such interior plateaus therefore exist for arbitrarily large rounded R. With constant R, the rescaled width recursion is bounded by the decaying birth width plus

\[
 20MR\sum_{n\ge0}L^{-n}+2MR
       =\left(20\frac{L}{L-1}+2\right)MR<100MR
\]

for the admitted fixed L. All quiet-window regions fit the eligibility size bound. Here N_0=1+log_LR and the prepared core has current width O(M), directly consistent with (1.73). This particular choice avoids any issue from a rounded R change in the active-stratum existence proof; Lemma RS.2 itself remains valid for the more general nested grids.

### Exact common old hole in the no-new-field case

The geometry can be made more precise. Let C denote the next-grid cover of Z_{k−1}. Set the new P_k,Q_k,R_k selectors to their empty values. CMP119 printed p.265, (3.2)–(3.5), then gives

\[
 P_k\text{ is tested only outside }C^{+4},\qquad
 B^k(P_k^1)^c=C^{+5},\qquad
 \Omega_k^c=C^{+8}.
\]

Printed p.269, (3.20), gives

\[
 Y=\Lambda_k^c=(\Omega_k^c)^{+2}=C^{+10}.              \tag{RS.3}
\]

Here +q denotes addition of q current MR_k-cube layers. These are the printed formulas. On a rectangle these layer additions are invertible by removing the stated number of layers. Thus two no-new-field histories with the same final Y have the **same** C and the **same** old \(\Omega_k^c\). Their prepared replacement cores can still differ, because those come from the older k−N_0+1 domains.

There is consequently no common-selector prohibition on placing a final bad-curvature witness in the interior of C, far from the two prepared cores. The new P_k test does not examine that region. C has side lengths at least MR_k, while each prepared core has side lengths at most 100M. For large R_k there is room for a fixed-size pulse, its full local test stencil, and a buffer of order R_k from the cores and the relevant tested boundary. The source hierarchy M≫M_2 (CMP119 p.245) supplies the fixed margin for the LM_2R_k test stencils.

## 5. Source realization requirements and observable scope

The actual realization starts with the strict pure-gauge Q1 birth seed of NR20.4. Its coarse average is the identity, its physical Wilson curvature is zero, and the soft-gauge weight is positive. Subsequent flat fields produce no new bad regions, so their regions evolve by S. This supplies the geometric histories used in §4 with positive old support near the flat state, before the final residual requirement.

To obtain a **residual** rather than successful final component, the fresh new field must have \(\chi_k^c(Y^6)=1\). A completely flat full output is therefore unavailable. The desired common output would instead have a strictly bad local curvature witness in the common old large-field interior, outside both small prepared cores. Its scale should lie between the final test threshold \(\varepsilon_k\) and the exterior-extension threshold \(2\varepsilon_k\) of LFR I (1.75). All plaquettes of P_x should remain flat.

The concrete requirements, proved in §§6–8, are:

1. identify a common subregion of the two old \(\Omega_k^c\) domains which is a distance of order MR_k from their outer boundary and from both cores;
2. choose a localized coarse pulse there for which the global determining-set minimizing field has maximal curvature, for example, \(3\varepsilon_k/2\), while each local test minimizer agrees on the witness stencil closely enough to violate the \(\varepsilon_k\) test;
3. check every preparatory and prior-step selector, not just the two final thresholds; the same smooth background has curvature \(L^{-2(k-j)}\varepsilon_k\) at an earlier j-scale, but the actual determining collars and old zero-mode data must be included;
4. impose the two fresh axial conditions by gauge transformations supported inside the disjoint cores. The two raw fields can remain physically flat near P_x; tree constraints alone do not force nonzero plaquette curvature;
5. verify one fixed open old-field/coarea box for descriptor 1 with a genuinely fluctuating current plaquette in P_x. Strict selector margins then give a positive lower bound for its old scalar mean and posterior share on its stratum near the common output.

The fifth step needs no uniform ultraviolet lower bound: at one fixed admitted cutoff, a strictly positive bound already contradicts an infinite-sensitivity norm. Its positive numerator comes from an actual old coarea box. The finite denominator is bounded in the complete old source integral, not replaced by a fresh reference normalizer.

The proposed incoming mark is the local Wilson scalar of the **old current** field V_k immediately before R. It is an actual coordinate, not a dummy Haar variable: CMP119 (2.21) still has the block-average constraints there; the integration in LFR I pp.193–194 changes the density and removes those constraints on \(\Lambda\). At fixed cutoff this local scalar has finite value, variation, and full-law moments in an elementary local M-03 input representation.

It is nevertheless not automatically the particular \(F_k\) obtained by transporting the microscopic F-01 scalar through all previous steps. A completed construction for this native current test would obstruct a universal M-06/H-04 operator assertion on all admitted local inputs. It would not by itself prove that the specific microscopic M-04 scalar has the same active jump. That additional identification or a separate old-microscopic-energy comparison must be proved.

## 6. Same-lattice variational nesting: the exact identity available for the realization

An independent source check removes one apparent obstacle in §5. CMP98 §B, (42)–(43), defines the higher block averages by successive composition. CMP119 printed p.255, (2.2), defines the actual determining set by

\[
 \Gamma_0=\Omega_1^c,\qquad
 \Gamma_j=\Omega_j^{(j)}\setminus\Omega_{j+1}^{(j)}\ (1\le j<k),
 \qquad \Gamma_k=\Omega_k^{(k)}.
\]

### Lemma RS.3 (same-lattice fiber inclusion)

Let U_* be a regular minimum of the fine Wilson action with its **complete final** k-average fixed. Choose an actual aligned nested determining sequence, and set its data on \(\Gamma_j\) equal to \(M^jU_*\). Then every fine field W with those mixed determining data has the same complete k-average as U_*. Therefore U_* is also a minimum on the mixed fiber, and its restriction to the source regular region is the unique source minimal orbit for those data.

**Proof.** At level zero, W=U_* on \(\Omega_1^c\). Suppose the complete j-average is already equal outside \(\Omega_{j+1}^{(j)}\). On the next shell the equality is specified directly by the \(\Gamma_{j+1}\) data. Outside \(\Omega_{j+1}\), the next averaging paths are built entirely out of already specified lower-level values; the domains are unions of the source block partitions. Cross-interface bonds are included in the shell by the source point/bond convention. Thus recursive averaging gives equality outside \(\Omega_{j+2}^{(j+1)}\). Iterating and then using the \(\Gamma_k\) data yields equality everywhere at level k. The mixed fiber is therefore a subset of the full k-average fiber and contains U_*. Global minimality gives minimality on that subset. The source's uniqueness of the regular minimal orbit identifies the actual map. QED.

This is a same-fine-lattice constraint inclusion. It does not assert equality between minimizing problems posed on different reconstructed lattices, and does not solve the unrelated C-05 reconstruction transfer issue recorded in BM.24.

The source uses this principle in the displayed intermediate minimum CMP119 p.266, (3.10): the minimizing old current field is \(M^j(U_{j+1})\). To obtain zero **true** regular fluctuations one must also choose the actual gauge representatives. Minimal-orbit uniqueness alone is not equality of two arbitrary axial representatives. Choose a backward stationary chain \(V_{j-1}=M^{j-1}U_j(V_j)\), or use the source's compensating center-fixed gauge transformations at each step. Those transformations preserve every already fixed higher average. The resulting chain is represented by averages of one final fine representative, in the source gauges. Insert the birth seed only afterward, by its center-fixed first-step transformation supported in the old bad interior. The approximate local fluctuation tests are then controlled by the exponentially small localization difference in CMP119 (3.17)–(3.19).

## 7. Positive native-current realization

The following construction verifies the active-support hypotheses of Proposition RS.1. The literal source-coordinate pullbacks and preparations are made explicit in §8 and analysed further in [residual strata analysis](residual_strata_analysis.md).

Choose the two histories of §4 at the first time their old component is eligible, so that there is no earlier replacement. Pick a coarse bond pulse supported well inside their common cover C, a distance of order R_k from both prepared cores and from the relevant test boundaries. On a sufficiently large torus let V_k(s) be identity away from that pulse. Let U_*(s) be the regular fine Wilson minimum with complete final average V_k(s).

CMP102 Proposition 9 and (190) give the analytic map and its exponentially decaying derivative. Thus the normalized curvature of U_*(s) is exponentially localized near the pulse. It is nonzero to first order: otherwise the k-average would have zero first-order coarse curvature, contrary to the chosen coarse plaquette pulse (the averaging estimate used in [support analysis](support_analysis.md) gives this implication quantitatively). After scaling s, arrange

\[
 \max_p\eta^{-2}\|U_*(s;\partial p)-I\|=\tfrac32\varepsilon_k.
                                                               \tag{RS.4}
\]

The maximum lies in a fixed current-size neighborhood of the pulse. Comparing the full minimum with the component and local determining-set minima changes the curvature there by O(\(e^{-cR_k}\varepsilon_k\)); outside that neighborhood the fields have the same small localization bound. This uses the same-source-lattice boundary comparison, with boundary data equal to identity up to the localized tail. Applied on the actual determining collars, (RS.4) therefore implies simultaneously

\[
 \chi_{k,\Lambda_1}=\chi_{k,\Lambda_2}=1,
 \qquad \chi_k^c(Y^6)=1,
\]

with strictly positive margins, because their thresholds are 2\(\varepsilon_k\) and \(\varepsilon_k\), respectively.

Use Lemma RS.3 to set the old fields equal to the corresponding successive averages of U_*. At an earlier j-scale the fine curvature remains the same, while the threshold is \(\varepsilon_jL^{2(k-j)}\eta^2\). Thus the earlier curvature tests have a strict margin. All true fluctuations vanish. The approximate ones are exponentially small by (3.17)–(3.19), below their source cutoffs.

At the birth location insert the strict center-fixed pure-gauge Q1 seed of NR20.4. Its center-fixed gauge transformation preserves the complete first average and hence every later average. It does not change any Wilson plaquette eigenvalues. Since the fine field of U_* there is exponentially small in the chronological age and in the pulse-to-seed distance, the strict Q1 bad margin and the strict P0/P1 good margins persist. It creates the translated birth rectangle and no other birth rectangle. Later new P,Q,R selectors remain empty; the final moderate pulse is masked by C^{+4}, as checked in (RS.3).

The preparation around \(\Lambda_i\) sees only the exponentially small pulse tail. Its new reference minimum differs from V_k(s) inside that core by the same small tail; therefore the relative fresh cutoff and the preparatory \(\chi'\) have strict margin. The old-core physical curvature cutoff is also good, since the birth seed is pure gauge. Section 8 proves these statements on the complete preparation coordinate maps, including the artificial seam.

Finally, impose the two fresh graph conditions by gauge transformations supported in the disjoint cores and fixed on their exterior. A tree graph permits this unique gauge fixing once its exterior anchor is fixed. The source covariance (CMP102 (181)) and the local axial representative imply that fixing one core leaves the other core's reference conditions unchanged. The resulting common field v_* is in both fresh strata, and its plaquettes near either core are still flat. The fresh factors and the residual selector are strictly positive on relative neighborhoods of v_* in each stratum.

For descriptor 1, a small physical perturbation of an old V_k plaquette in P_x is permitted while keeping its exterior fixed: reconstruct it using the same regular constraint maps and retain the strict selector margins. Such perturbations form a positive coarea-volume old set on which \(\phi_x>0\). They supply a positive old marked numerator. At fixed cutoff the source upper bound on the unnormalized old operation and the separate fresh-reference lower bound control the remaining finite denominator; no lower bound on an old rare mass is inferred from its upper bound.

For descriptor 2, every descriptor whose core touches P_x has core disjoint from \(\Lambda_2\). Use compact gauge transformations supported inside \(\Lambda_2\) and fixed on its exterior. Under such a transformation the reference orbit of the other descriptor is unchanged on its own, disjoint core by gauge covariance; hence its fresh graph support is preserved. Its full-Y shell Haar factor supplies absolute continuity along this gauge orbit. Its remaining old and fresh positive densities may change, but they do not turn that orbit measure into an atom. The graph equations of descriptor 2 fix a nontrivial, anchored gauge transformation on \(\Lambda_2\), a Haar-null subset of this orbit. Disintegrating along the gauge orbit therefore proves that the other descriptor assigns zero mass to \(S_2\). This is stronger and safer than conditioning on the whole raw shell while treating a shell-dependent reference as fixed. It follows that all descriptors resetting P_x have zero posterior weight at almost every point of \(S_2\), and the exact conditional mean there is \(\phi_x(v)\), tending to zero as v tends to v_*.

These facts meet Proposition RS.1 and prove an extension-independent infinite strong-current cost for this actual **native current scalar input** on the descriptor-erased residual H-03 output. The construction does not identify that input with the particular microscopic transported scalar. It also does not establish a continuum obstruction: the phenomenon belongs to the specified singular residual gauge-reference representation and the ambient M-03 continuity requirement. Section 9 explains why retaining a new support-class label changes this topological conclusion.

## 8. Reference-tail estimate for the fresh and preparatory cutoffs

The required reference estimate can be reduced to the actual source Hessian rather than inferred from an arbitrary reference Gaussian. Work in the fixed axial coordinates a for the current field in one prepared core \(\Lambda\), with the shell pulse parameter s fixed. Define the **classical source functional**

\[
 \mathscr A_\Lambda(a,s)
   =A\bigl(U_{k,Y}(V_\Lambda(a),V_{\rm shell}(s))\bigr).
                                                               \tag{RS.5}
\]

Its minimizer \(a_*(s)\) is precisely the reference orbit of LFR I (1.77)–(1.78). It is not the mean of the old conditional law. At s=0 its axial representative is zero.

The source proof in LFR II pp.357–359, (1.7)–(1.9), bounds the Hessian on the fixed axial core below by \(c_M I\), with \(c_M>0\) depending only on the fixed M. The same bound with half that constant holds on a sufficiently small real regular neighborhood; the reference bound (1.78)/(1.83) puts both zero and \(a_*(s)\), and their line segment, there when the coupling is sufficiently small. The current coordinate dimension is O(M^4), independent of the old chronological age.

Let D be the current-scale separation of the pulse and \(\Lambda\). The actual analytic minimizing-field response in CMP102 Proposition 9, (190), implies

\[
 \|\nabla_a\mathscr A_\Lambda(0,s)\|
       \le C_M|s|e^{-cD}.                                \tag{RS.6}
\]

To see the source of this factor, write the first variation of the Wilson plaquette sum. The curvature of the unperturbed-core field is localized at the pulse, while its derivative in an a-direction is localized at \(\Lambda\). Their product has a connecting exponential. Summing the output plaquettes convolves these exponentials; reserve half their rate to absorb the polynomial in D. Each curvature and each curvature variation has its source factor \(\eta^2\), so the two factors cancel the \(\eta^{-4}\) fine plaquette count in four dimensions. The normalized current derivative bounds in (190) justify this summation without a chronological-rank factor.

Since \(\nabla_a\mathscr A_\Lambda(a_*(s),s)=0\), strong convexity along the segment gives

\[
 c_M\|a_*(s)\|^2
 \le \bigl\langle a_*(s),
   \nabla_a\mathscr A_\Lambda(a_*(s),s)
      -\nabla_a\mathscr A_\Lambda(0,s)\bigr\rangle
 \le \|a_*(s)\|\,\|\nabla_a\mathscr A_\Lambda(0,s)\|.
\]

Consequently

\[
 \|a_*(s)\|\le C_M|s|e^{-cD}.                           \tag{RS.7}
\]

The tree gauge transformation sending the flat current field to the relative graph condition uses only O(M^4) edges. Its products and inverses are uniformly smooth on this small chart. It therefore changes the links by at most another fixed C_M times (RS.7). The relative fresh field satisfies

\[
 \sup_{b\subset\Lambda}|\log V'_k(b)|
       \le C_M\varepsilon_k e^{-cD}
       <M_0\varepsilon_k.                                \tag{RS.8}
\]

This argument allows either actual graph orientation and does not require silently matching the reference's axial tree with the fresh tree. It uses the reference minimizer, the source positive Hessian, and the literal fresh cutoff in LFR I (1.101).

The same two fields enter the literal old preparatory relative coordinate of LFR I p.195, (1.81):

\[
 V''=V'V_0,\qquad V_0=M_{\mathbb B''_k}(U_0),\qquad
 \mathbb B_0=\mathbb B''_k\cap\Lambda_0,\quad
 \Lambda_0=\Lambda\cap\Omega_{h+1}^{\prime\prime\,\sim2}.
\]

The displayed source identity identifies the inner excluded region as a padded old core; in particular the strict seed support is disjoint from \(\mathbb B_0\). Boundary-crossing bonds at \(\partial\Lambda\) belong to \(\mathbb B_0\), while those at its inner boundary do not. This exact domain is preferable to the schematic shorthand \(\Lambda\setminus Z_h\).

Before the removal of the current averages, all preparations can be set at zero true fluctuation by Lemma RS.3 on their new, still aligned determining sequences, using the compatible gauge representatives just described. Removing the averages on \(\Lambda\) changes the reference only by (RS.7). Its reconstruction into the old mixed scales is controlled by the source normalized minimizing response. The averaging estimate to cite here is **CMP98 Proposition 6, (164)**, not the algebraic identities (106)–(108) alone: if \(U_0\) obeys its regular curvature condition (52) and \(U'=\exp(i\eta A')\), then the complete average obeys

\[
 \bigl|M^j(U'U_0)(M^jU_0)^{-1}-I\bigr|
       \le C L^j\eta\,\|A'\|,
\]

after rescaling that proposition to averaging order j. Its constants are independent of j; this follows from Proposition 4 and the geometric sum in (162)–(163). Relative-gauge compensation must still be retained in the actual B' convention. The same displayed gauge identities control that compensation by a fixed multiple of the small relative field; no unproved derivative formula is obtained merely by naming (106)–(108).

The remaining gauge factor is controlled more precisely by the **one literal mixed-scale tree** T_0, not by N separate large tree changes. Printed p.196 constructs one axial tree in each rectangular annulus and connects it to its predecessor by one external bond. The quotient graph of shells is a chain. A simple root path visits each annulus at most once, and the displayed detoured coordinate contour has length at most C M R_j in the j-scale lattice. The relative gauge transformation on such a path is the ratio of the old and reference path transports. Since the fields are unitary, telescoping the products yields a sum of the bond differences, with no product of path lengths. Hence, writing a for the fine relative-potential bound \(C_M\varepsilon_ke^{-cD}\),

\[
 \sup|u-I|
   \le C M a\sum_{j=h}^{k}R_jL^{j-k}
   \le C_M R_k a.                                      \tag{RS.9}
\]

The last inequality is immediate on the chosen R plateau, and also follows from the source polynomial comparison of R_j at neighboring old ages and the geometric factor L^{j-k}. Even the cruder bound C_M N R_max a is only polynomial in R on this history. Imposing the literal T_0 gauge on \(V''(M_{B''}U_0)^{-1}\) therefore gives \(\|B'\|\le C_MR_k\varepsilon_ke^{-cD}\). It is smaller than \(\delta'_k\) for sufficiently small coupling and D≥c_0MR_k. No factor R_k^N or product of N tree sizes has been hidden in this estimate.

The pure-gauge birth seed is strictly inside Z_h and equals the identity near its boundary. Its higher block averages are exactly unchanged by center-fixed gauge covariance. It therefore creates no additional term in this relative-field comparison. The other literal cutoff is \(\chi_{h,1/2}\) of **(1,V_h)**, not merely of V_h. The identity extension creates an artificial seam at the old-domain boundary. The seed gauge is one near that seam, so its contribution remains pure gauge after extension. The physical annular links and their compensated axial/Landau gauge change obey the same localized tail estimate. Their seam plaquettes are therefore smaller than the h-scale cutoff with strict margin. Applying the local variational regularity estimate proves the required \(\chi_{h,1/2}\) test. LFR I (1.89) then proves that the original \(\chi_k''\) factor is one; it is not discarded without checking its replacement cutoffs.

This proves the reference and preparation cutoff claims used in §7. The independent primary-source analysis verifies the exact annular domain, compatible representatives, single mixed-tree transport, and filled-field seam. The analytic response is the original same-lattice minimizing map. No cross-lattice reconstruction identity from the open C-05 problem is used.

## 9. An exact descriptor lift that separates the topological strata

### 9.1 Reference classes and support classes are different objects

A **complete fresh-reference class** r must include every descriptor feature entering the normalized fresh factor: its actual integration domain, fresh graph and anchoring convention, reference orbit/representative rule, cutoff choice, localized action cutoff \(\zeta\), any scale or coupling labels actually used there, and any additional choice in the primitive h/H formula. Only after these agree is cancellation of the common fresh kernel literal.

In the displayed source formula, at fixed Y, the local determining map \(U_{k,Y}\) is the one in LFR I (1.74), the reference orbit is selected by (1.77)–(1.78), and the localization cutoff is the fixed source \(\zeta_Y\). Thus the significant varying features are the prepared core and fresh graph. This notation is not permission to omit an additional feature if a different ledger has retained it.

Let \(M_r(v_r,d\eta)\) be the sum of the actual old positive measures with that common fresh reference, including all their old internal history weights. Set

\[
 m_r(v_r)=M_r(v_r,1),\qquad
 n_r(v_r)=M_r(v_r,F),\qquad
 q_r(v_r)=n_r(v_r)/m_r(v_r)
\]

on m_r>0. The normalized fresh kernel is \(k_r(du'\mid v_r)\). For the fixed residual output geometry, let \(c_Y(v)=\chi_k^c(Y^6)\) denote the common final residual selector, including any other genuinely common output support factor. Its output component measure is

\[
 \mu_r(du',dv_r)=c_Y(v)k_r(du'\mid v_r)m_r(v_r)\,dv_r. \tag{RS.10}
\]

The notation dv_r denotes the actual retained reference, including coarea conventions when present. Descriptor-dependent exterior selectors remain in M_r and are not canceled as common Y-only factors. The old marked component measure is \(q_r\mu_r\). The common c_Y is one on the active patches used above and cancels from the posterior there; it has not been removed from the output law. These identities preserve every old normalizer and use no assumed equality between old and fresh laws. M_r is the complete old positive baseline, including cross terms and any completed other-component factors; a separately refactored T'_k(Y) is not substituted for that baseline without recombination.

Two different complete reference classes can have the same support stratum. For example, two different smooth positive reference weights on the same graph slice need not be mutually singular. Group such classes into support classes a whenever necessary. Claim singularity between two groups only when it has been proved by a genuinely free direction: distinct prepared domains have a free local gauge direction outside one domain; distinct tree edge sets on a common domain have a non-tree link coordinate free on one slice. The relative reference must be held covariantly, as in the gauge-orbit argument of §7. If the direction is unavailable, retain the posterior over both classes instead of declaring it zero.

### Theorem RS.4 (finite exact lift by mutually singular support classes)

Suppose the complete reference classes have been grouped so that

\[
 \mu_a=\sum_{r\in a}\mu_r
\]

are mutually singular for distinct a. Let \(\mu=\sum_a\mu_a\), and let \(p_a=d\mu_a/d\mu\). After choosing disjoint full-measure carriers of the \(\mu_a\), p_a equals the indicator of the corresponding carrier almost everywhere. Define the lifted output law

\[
 \widehat\mu(dv,da')=\sum_a\mu(dv)p_a(v)\delta_a(da'), \tag{RS.11}
\]

with a' sampled independently of the old internal state conditional on v, exactly as in the history reset of HS20.

Then the erased current-field marginal is unchanged, and the exact marked conditional in the lifted state is

\[
 \widehat QF(v,a')=QF(v)
    =\sum_{r\in a'}\frac{d\mu_r}{d\mu_{a'}}(v)q_r(v_r)
                                                               \tag{RS.12}
\]

for \(\widehat\mu\)-almost every output. If a' contains a single complete fresh-reference class, or several descriptions with the same literal fresh kernel and integration domain, this reduces to the summed old quotient q_{a'}(v_{a'}). In that case the exact mark is independent of the newly sampled fresh variables on its active stratum. In general the posterior within a' remains in (RS.12).

**Proof.** Marginalizing (RS.11) gives μ because \(\sum_a p_a=1\). Conditional independence of the fresh copy a' gives \(\widehat QF=QF\). The mutually singular support decomposition makes every class outside a' have zero posterior weight on its carrier. Within that class the Radon–Nikodym form of Bayes' rule applied to (RS.10) gives (RS.12). When the fresh kernel is common, factor it out of both the summed numerator and denominator; this yields the summed old quotient. QED.

### 9.2 Local continuous extension and what it requires

Suppose on a buffered real chart the numerator and denominator representing the right side of (RS.12) are C^1 functions N_a,D_a, with D_a≥d_a>0. Then N_a/D_a is C^1 there. For an actual graph slice, a smooth local retraction can set the graph links to their reference values while leaving its free coordinates and shell fixed. Composing the quotient with that retraction gives an ambient C^1 extension on the chart at the fixed discrete label a. When the common fresh factor cancels, one simply uses the old quotient as a function of its shell and makes it independent of the fresh coordinates.

This extension agrees almost everywhere with the **lifted** actual marked law. It may assign different off-support values at the same raw current field for two different discrete labels. That is precisely why the two erased strata approaching a common point do not force an infinite continuous difference in the enriched state.

The C^1 and positive-buffer hypotheses are substantive. Integrated sharp old selectors can create nonsmooth boundaries, and neither positivity of the old integral nor the formal quotient alone proves them. The theorem removes the requirement of continuity **between different singular support classes**; it does not prove all old quotient derivatives, a global extension through all other interfaces, or their uniform normalized costs.

The repair can be specified at kernel level, rather than choosing unrelated extensions for individual marks. When one complete fresh-reference class is identified on a stratum, use the normalized old measure \(M_r(v_r,d\eta)/m_r(v_r)\) on the corresponding buffered ambient chart at the fixed new label r. For a support class containing several fresh references, use their full positive mixture with the same h/H weights and common graph-chart retraction. These kernels agree with the actual conditional law on its support and preserve the constant coefficient one. Apply them coefficientwise to the **whole finite incoming source jet** and take its finite logarithm afterward. All inherited higher vertices and generated cumulants remain present. The direct/current records are derived from that chosen kernel extension; they are not assigned independently. This is an explicit use of M.1's permitted better-extension convention.

### 9.3 The remaining full physical carrier cost

A discrete change of a is an M-03 difference with denominator one. Its carrier includes the actual dependency footprint of the core/graph/reference label. For the residual construction this includes the relevant Y history and its source collars; it cannot be reduced to the storage block of the label. The weight remains

\[
 e^{\kappa(|Y^+|+\mathsf t(Y^+))},\qquad |Y^+|=O(R_k^4).
\]

The lifted quotient need not have a compensating factor of this size. Source smallness of an unnormalized component mass cannot simply be assigned to a normalized residual mean. Thus the lift is a valid finite law and extension repair, with a clear regularity premise. It does not pay the specified full physical carrier norm, prove the all-history current estimates, or finish M-04.

## 10. The completed finite-cutoff result

### Theorem RS.5 (native scalar on the descriptor-erased residual output)

For the displayed soft-gauge Wilson construction with a nontrivial physical gauge sector, choose admissible fixed source parameters and a sufficiently small coupling on one of the plateaus described in §4. There exist a finite cutoff and volume, an active retained residual component Y, and a local old-current Wilson scalar \(\phi_x\) such that:

1. \(\phi_x\), as a function of the actual current field immediately before the R preparation/replacement, has finite M-03 value and direct-difference cost at that cutoff;
2. its exact conditional mean under the complete positive H-03 operation, with the internal core/graph descriptors erased and Y retained, has no ambient continuous version agreeing with the actual output law almost everywhere;
3. consequently every compatible direct/current carrier representation of that erased output has infinite combined M-03 cost, already at this finite cutoff. Subtracting any continuous scalar/identity term does not remove the failure.

**Proof.** Lemma RS.2 and the constant-R construction give two actual geometric histories with the same final Y and separated prepared cores. The exact old-hole computation (RS.3) leaves a common region where the moderate pulse does not create a new bad selector. Lemma RS.3, with its representative prescription, the pure-gauge birth seed, and §§7–8 give two strictly positive old and fresh coarea patches with the common residual flag. The native scalar stencil is chosen inside the first core and far from the second; the common intersection field has flat plaquettes on that stencil and has its strict residual witness elsewhere.

On the first patch a physical perturbation of the old current stencil remains admitted and has positive scalar value. It supplies a strictly positive old marked numerator, uniformly on a sufficiently small retained-data neighborhood. The finite source integral bounds and the finite number of descriptors at this cutoff bound the total density on its generic stratum, so its conditional scalar mean has a positive lower bound. Every other contribution is nonnegative.

On the second generic patch, a descriptor resetting the chosen stencil has a core disjoint from the second core. The gauge-orbit disintegration in §7 gives it zero posterior mass there. All descriptors which remain retain the old scalar stencil, so their conditional mean is exactly \(\phi_x(v)\). This tends to zero at the common intersection. Proposition RS.1 excludes every continuous version, regardless of values assigned on null or inactive fibers.

At fixed cutoff the incoming native Wilson function is smooth and bounded on its compact link coordinates; its elementary differences are bounded and its full-law moments are finite. A finite carrier representation, with its genuine finite footprints, therefore has finite incoming cost. Conversely finite combined output direct/current cost implies local ambient Lipschitz continuity, as proved in [support analysis](support_analysis.md); hence no such representation of the erased output is finite. A continuous subtraction has the same limiting value on the two approaches and cannot remove their nonzero difference. QED.

This theorem and the residual strata analysis do not prove M-04, M-06, H-04, or M-07. The microscopic transported-input identification is unproved, and the exact descriptor lift is an allowed way to separate these particular strata. After that lift the remaining sharp-interface, normalized-moment, current, and full-volume carrier estimates are the substantive next problems.
