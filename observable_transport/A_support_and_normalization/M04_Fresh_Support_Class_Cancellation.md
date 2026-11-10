# Fresh support classes and exact cancellation of the common reset kernel

This note refines RS.4 for the literal fresh reference factor. It proves support-class identification and common-kernel cancellation when the source's localized action cutoff and other fresh construction rules are fixed. It keeps a residual within-support mixture whenever two actual fresh kernels differ despite having the same support. Nothing here estimates the old raw Schur precisions or the microscopic marked moments.

## 1. Literal fresh data

Fix one final residual component Y, the current scale and coupling parameters, and a buffered admitted real chart. At a complete fresh descriptor r, let Lambda_r be the prepared core and G_r its anchored axial tree/forest with the allowed fixed-exterior anchors. Fill the current shell Y\Lambda_r by Haar measure and use the actual conditional fresh gauge-slice kernel on Lambda_r, as in HS20.4. This defines the positive full-Y reference measure rho_r. It includes the actual fresh cutoff and has a locally absolutely continuous positive density on every strict open patch of its slice used below.

LFR I (1.74) uses the homogeneous localized determining map U_{k,Y} of the current field. Equations (1.77)-(1.79) define the unique minimizing **orbit** with the shell fixed, and its representative V_{Lambda_r}; the orbit does not depend on the old mixed determining set B''_k or the old T_h variables. The fresh h_r/H_r of (1.100) is determined by:

- Lambda_r, Y and the retained shell;
- the fresh graph G_r, anchors and representative/orientation conventions;
- the actual localized action cutoff zeta_Y and fresh cutoff rule;
- the fixed scale/coupling parameters.

The old mixed tree T0 and the older history stay in the old measure. If the orientation average correlates T0 and G_r, its conditional finite weights stay in that old measure after G_r is fixed. They do not create a new fresh kernel.

The fresh shell cutoff chi_{k,Lambda_r} and final residual selector restrict the active output. At a fixed support class with common fresh data, they are retained-only common factors and may be canceled from the old quotient on its positive fibers. Their values and the old version outside support must still be recorded when defining a kernel extension.

## 2. Distinct prepared cores give mutually singular fresh measures

### Lemma FS.1

Suppose Lambda_r and Lambda_s are distinct source rectangles, so one has an interior gauge site in its difference from the other. Then rho_r and rho_s are mutually singular.

**Proof.** Interchange r and s if necessary so that there is an interior site x in Lambda_s\Lambda_r, together with the needed fixed local neighborhood. The source cores are unions of fixed M-cubes, so a proper difference contains such a site after accounting for their fixed boundary convention.

Apply gauge transformations at x, with identity outside that neighborhood. Under rho_r this is a shell gauge direction: the full shell Haar reference is absolutely continuous along it. The reference minimizing orbit for core r is gauge covariant, and the transformation is identity on that core and its graph endpoints. Thus the graph constraints defining r are preserved. Remaining positive densities may change but cannot turn this Haar direction into an atom.

For core s the exterior shell is unchanged by the same transformation. Its chosen reference representative is therefore fixed. The anchored graph G_s contains a constraint fixing the gauge at x relative to its anchored component. Satisfying all those graph equations fixes this local gauge variable to a Haar-null set. Disintegration along that direction gives rho_r(S_s)=0, where S_s is the support slice of rho_s. Hence rho_r is concentrated on the complement of an rho_s-full set. This proves mutual singularity. The argument does not require the two slices to have the same dimension or to have a positive-mass intersection. \(\square\)

This is the source-specific free-direction argument. It is not a declaration that every pair of differently named descriptors is singular.

## 3. Graph changes on a fixed core

### Lemma FS.2

Fix Lambda and its retained shell. If two anchored graphs impose genuinely different tree-edge constraints, their fresh measures are mutually singular, except for graph descriptions whose constraint sets are identical and should be merged.

**Proof.** If the actual constrained edge sets differ, choose an edge constrained by s but not by r. On the r slice this edge is a free compact group variable, after solving the r tree equations. The strict fresh cutoff leaves a relatively open set of that variable; its law is absolutely continuous with respect to Haar. The s condition fixes it to a prescribed reference value. That condition is Haar-null. The reference value depends only on the shell, which has been fixed here, and not on this free interior field. Fubini over the shell proves singularity of the full-Y measures. Duplicate edge/anchor descriptions of the same constraints are merged. \(\square\)

When the same graph is used with different representative conventions, an additional distinction is essential. Tree-edge values do **not** determine an arbitrary physical connection. The following comparison uses the already established uniqueness of the **same minimizing orbit** for the same Lambda, Y and shell.

### Lemma FS.3

Suppose two reference representatives belong to that same minimizing orbit, agree at the fixed exterior, and have the same values on one complete anchored graph. Then the representatives coincide on the whole core.

**Proof.** They differ by an allowed gauge transformation u which is identity at the exterior anchors. Equality of the two reference connections on a graph edge transports the value of u from one endpoint to the other. Starting at each fixed anchor and following the graph fixes u at every interior site. Thus u is identity throughout the core, and the two representatives coincide on every edge. The physical connection was fixed beforehand by uniqueness of the orbit; the tree only fixes its gauge representative. \(\square\)

If the graph/reference constraints are not identical as functions of the shell, the corresponding slices are generically distinct. On an analytic buffered chart a proper equality condition is Haar-null unless it holds identically on the relevant chart component. One may split by those chart components and merge only genuinely coincident supports. This avoids treating accidental equality at a flat shell point as equality of the full reference measures.

## 4. Fixed fresh rules give a common kernel on a support class

Assume the localized action cutoff zeta_Y, the fresh cutoff, and all remaining fresh construction rules are fixed functions of the source geometric data and fixed scale parameters. By CG.2, Y is itself determined by Lambda on the literal quiet branch.

Lemmas FS.1-3 identify the generic support class a by its actual core, graph constraints and reference representative. Descriptors in one such class then have the same fresh kernel

\[
 k_a(du'\mid v_{\rm ext})=h_a/H_a.
 \tag{FS.1}
\]

The old history, the mixed preparation coordinates and the old T0 choices may still differ, and are summed with their exact positive weights.

### Theorem FS.4 — exact class cancellation

Let M_a(v_ext,d eta) be the **complete** old positive measure in class a, including the successful-component sum and all cross interactions. The notation uses the original pre-refactorization old variables; no self-operation is substituted for the complete measure. For any old mark F, or coefficient of a whole finite incoming source jet, the actual conditional mean on the generic positive stratum a is

\[
 QF(v,a)=
 \frac{M_a(v_{\rm ext},F)}{M_a(v_{\rm ext},1)}.
 \tag{FS.2}
\]

It is independent of the fresh interior variable u' on Lambda_a. This statement is almost everywhere on the actual active support. It does not prescribe an off-support ambient version or prove a uniform derivative bound.

**Proof.** Before the action is refactorized, the literal fixed-reference joint measure is the positive product

\[
 k_a(du'\mid v_{\rm ext})\,
        M_a(v_{\rm ext},d\eta)\,dv_{\rm ext},
 \tag{FS.3}
\]

times genuinely common retained output support factors. This is the exact marked identity MG19.1/HS20.0a. The old mark is evaluated on its old physical preimage and is independent of the independently sampled u'. All histories in class a share k_a, so the positive old sum can be performed before dividing numerator by denominator. The common fresh kernel and the genuinely common final output selectors cancel, giving (FS.2).

The successful-component geometry and internal states have not been conditioned to a chosen value; they remain inside M_a. Their fresh fields lie outside Lambda_a by component compatibility. Similarly, for several fixed residual cores one uses the product of their common fresh kernels and sums the complete old joint measure. The equality survives every exact refactorization of the action. Apparent fresh-core dependence in individual reconstructed self or cross terms must cancel in their complete combination; it may not be discarded term by term.

Finally, the mutual singularity statements identify the class a from the full current output almost surely. Positive disintegration therefore gives the same conditional mean as the descriptor-erased law on that generic stratum. The identity is linear and applies to every coefficient of the entire finite incoming jet; its finite logarithm is taken only after transport. \(\square\)

## 5. Resampling the identified local class

Let p_a(v) be the actual posterior probability of a support class. On disjoint full-measure carriers of the mutually singular class measures, p_a is the indicator of its class. The allowed HS20 resampling draws a new a' with probability p_a(v), conditionally independently of the old internal state. Its transported mark remains QF(v), and almost surely on the lifted support,

\[
 \widehat QF(v,a')=QF(v)
     =\frac{M_{a'}(v_{\rm ext},F)}{M_{a'}(v_{\rm ext},1)}.
 \tag{FS.4}
\]

Thus the support-class lift can use the bounded anchored core/graph code of CG.4. It separates the singular reset strata without retaining the old internal history as a conditioning event. Any subsequent ambient extension is chosen at kernel level and transported through the complete finite jet. The raw locality and the uniform currents of that extension still need their own proof.

## 6. Different fresh kernels on the same support must remain mixed

If the ledger leaves zeta, a cutoff parameter, or another fresh rule as a genuine unfixed choice, different values may give the **same** graph slice while changing h/H. Such choices are not identified by support singularity. They must remain distinguished as internal labels in the exact within-support posterior:

\[
 QF(v,a)=\sum_{r\in a}
      \frac{d\mu_r}{d\mu_a}(v)\,
      \frac{M_r(v_r,F)}{M_r(v_r,1)}.
 \tag{FS.5}
\]

A newly resampled r drawn from this posterior does not make its old conditional quotient equal to QF: the resampling is conditionally independent of the old state, so the mark remains the full mixture. Merely writing a new label does not cancel unequal fresh factors. In particular, it is incorrect to treat all graph-coincident descriptors as one common kernel without checking their actual fresh cutoffs and localized actions.

This is why FS.4 is stated for fixed fresh rules, or for an actual class on which every such rule is common. The source's usual deterministic cutoff/representative convention is of that kind; any noncanonical choice in the selected ledger must be examined explicitly.

## 7. Scope

The theorem provides the exact old-quotient identity needed by a constructive support lift and by a common-fresh-patch comparison. It preserves the actual old posterior and all higher source coefficients. It does not imply that the quotient has a bounded raw retained carrier: old Schur precision dependence, old coordinate pullbacks, reference-minimum tails, the full cross action, and the actual microscopic scalar moment remain separate analytic obligations.

Nor does it prove a microscopic counterpart of the native scalar continuity obstruction RS.5. Independence from one fresh core direction is an algebraic ingredient; a nonconstant actual microscopic conditional scalar on another stratum must still be established from the original Wilson law.

## Sources

- LFR I, pp.194-201, (1.74), (1.77)-(1.79), (1.83), (1.100)-(1.101): homogeneous fresh map, unique reference orbit, anchored graph and fresh quotient.
- LFR II, pp.356 and 378-379, (1.1), (1.71)-(1.72): complete old operation and final residual factors.
- Annexes [BI](../../history/Annex_BI.md)–[BM](../../history/Annex_BM.md), MG19.1/HS20.0a, HS20.4 and §8 of [Annex BI](../../history/Annex_BI.md): actual marked positive coupling, full posterior and conditionally independent descriptor resampling.
- [M04 Bounded Core Source Map](M04_Bounded_Core_Source_Map.md), CG.2-4: exact component redundancy, local code, native support and reference-law qualifications.
- [M04 Residual Strata Analysis](M04_Residual_Strata_Analysis.md), RS.1 and RS.4: positive-stratum arguments and the general support-class lift with an explicit within-class mixture when necessary.
