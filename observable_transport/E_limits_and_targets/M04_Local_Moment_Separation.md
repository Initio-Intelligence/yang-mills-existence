# The full-component reserve does not yet give a core-local scalar moment

This note records the precise remaining moment issue after the bounded-core geometry and successful-mask costs have been separated. It establishes an actual separation between the location of the fresh residual witness and the prepared core. It does **not** establish a diverging conditional microscopic Wilson scalar or a counterexample to the repaired M-04 augmentation.

## 1. An actual active output can be flat at the prepared core

Let Lambda be the prepared rectangle, of current side at most 100M, and let D0 be any fixed current enlargement used for its direct old-state and graph footprint. For arbitrarily weak admitted couplings, the final component Y has radius of order MR_k. The final source residual selector is tested on the corresponding eroded interior of Y, with the six-region-layer convention of LFR II p.379. This eroded interior still has radius of order MR_k. It is not confined to D0.

The active construction in [M04 Residual Strata Analysis](../A_support_and_normalization/M04_Residual_Strata_Analysis.md), analysed further in [residual strata analysis](../A_support_and_normalization/residual_strata_analysis.md), gives the following more concrete data. Choose a coarse bond pulse at a distance D>=cMR_k from D0 and well inside the old masked hole. Scale its amplitude so that the actual local variational test curvature is strictly between epsilon_k and 2epsilon_k, with margin. Choose the raw current field to be identity in a fixed neighborhood of D0. The source averaging identity and variational locality give the required pulse, the retained-shell extension test chi_{k,Lambda}=1, and the final residual chi_k^c=1. The last ordinary new-field tests do not see the pulse in the inherited masked region.

The reference minimum V_Lambda induced by that remote pulse has a core potential of size at most

\[
 C_M\epsilon_k e^{-cD}.
 \tag{LM.1}
\]

The source fresh tree gauge can be imposed by a gauge transformation supported in the core. It preserves exact current plaquette flatness there. If the native output includes the relative fresh free coordinate, its dimensionless square is at most C_M P(g_k)^2 exp(-cD). Consequently, for the augmentation retaining only the current fields and bounded fresh core labels,

\[
 R_{D_0}(v)\le 1+C_M P(g_k)^2e^{-cD},
 \qquad R_Y(v)\asymp 1+P(g_k)^2,
 \tag{LM.2}
\]

up to the fixed native conventions. The first quantity stays uniformly bounded and tends to one; the second detects the remote pulse. At finite cutoff the construction lies on strict positive active strata, with positive relative neighborhoods. It is not based on values assigned to a zero-normalizer fiber.

The localized Wilson cutoff zeta_Y does not force this witness into the core. Its outer transition is near the boundary of Y, and the source's estimates exploit its separation from Lambda. The retained residual test is a separate current-field test. There is no source implication that it must fail near Lambda.

Thus a bound of the form

\[
 \|1+\mathcal F\|_{L^p(q_v)}\le CpR_Y(v)
\]

does not yield the same bound with R_{D0}. Adding Y to the mark's carrier is a real physical enlargement and incurs its exponential weight. This is the precise limitation of substituting the young-trial logarithmic-mass estimate directly into BC.3.

## 2. A bad birth does not deterministically force physical Wilson energy

The old history sum at a fixed fresh-reference class includes its actual allowed birth mechanisms. A convenient R-only history used to lower-bound its denominator is not a retained event of conditional probability one.

For suitable classes, choose an h-rectangle large enough to be realized by the actual pure-gauge Q birth as well as by R births. It is enough to take h=1 and k=N+1 on an admitted short weak-coupling plateau, so the explicit first-step seed NR20.4 applies directly to the microscopic field. A gauge transformation equal to identity at every first-block center, supported on a noncentral local site, preserves the exact first and all later coarse averages and all microscopic plaquette traces. Its amplitude can cross the literal approximate Q threshold while remaining inside the larger soft-gauge contour. The full source density is positive there. The padded region cover can be chosen to give the same old h-rectangle, hence the same later quiet geometry and the same fresh Lambda, Y and graph class.

Apply this gauge seed to the actual remote-pulse reference chain used in Section 1. In the old core the physical Wilson curvature remains the exponentially small reference curvature. The seed creates a large **gauge** coordinate, not a large physical plaquette. At fixed cutoff, sufficiently small coarea neighborhoods keep the physical Wilson energy below any prescribed positive excess above this reference value while preserving the strict Q and preparation selectors. These neighborhoods have positive old mass, though no uniform lower probability is asserted.

Therefore the inference

\[
 \text{old bad history in this class}
   \Longrightarrow \text{old physical Wilson energy}\ge cP(g_k)^2
 \tag{LM.3}
\]

is false at the actual selector scope. This is the same source-specific distinction as NR20.4, now compatible with the remote residual pulse and fixed fresh class. The positive envelope F^natural contains genuine precision/gauge energy as well as the remaining Wilson energy; it is not the physical scalar itself.

This observation does not prove that the conditional physical scalar is small. A positive low-energy set can have very small posterior probability. Conversely, the young R trial does not prove a large scalar mean. Establishing either conclusion requires a relative comparison of the physical and gauge birth contributions in the full old sum, including the later preparation and its exact normalization.

## 3. The exact obstruction criterion for a growing scalar contrast

Here is what would suffice to turn the local-moment issue into a genuine strong-norm obstruction.

Suppose two actual positive lifted fibers, or their positive-measure limits, have the same current data near an insertion and have an old scalar conditional contrast a(g) after the fixed current-scale normalization. Suppose their core labels can be connected by a fixed number of elementary **anchored** label replacements, while the retained fields are held fixed. Assume the selected augmentation has no extra resampled continuous old energies near the core, so the native regulator remains bounded there as in (LM.2), and its total energy is O(P^2) in the remote witness region.

Every compatible M-03 representation must reproduce this contrast through its direct and kernel records. A carrier avoiding the remote witness has a bounded regulator. A carrier reaching that witness has tree length at least cR and hence weight at least exp(c kappa R), while its grade-3/2 regulator factor is at most C P^3. Consequently, with C_norm denoting the strong one-field current budget,

\[
 a(g)\le C_M C_{\rm norm}
       \left(1+P(g)^3e^{-c\kappa R(g)}\right).
 \tag{LM.4}
\]

The fixed number of discrete path steps is absorbed in C_M. This is just the exact compatibility identity summed over tags and bounded with their actual M-03 weights; no cancellation between records is used. Since the parenthesis stays bounded, any proved a(g) tending to infinity would contradict a uniform strong-current bound for this augmentation.

A label-independent identity subtraction and a fixed native scalar subtraction evaluated at the same retained field cancel from this label contrast. A genuinely label-dependent subtraction would have to be recorded with its own direct/current cost; merely moving the contrast into such a counterterm would not estimate it.

There are two essential qualifications. First, the actual transported microscopic scalar contrast a(g) has not been proved. The native old-current scalar obstruction in RS.5 gives a nonzero fixed-cutoff contrast, not the required growth. Second, an inactive or otherwise inadmissible endpoint cannot be assigned a fixed value and then used as evidence of an intrinsic contrast: its kernel version is free to be extended as permitted by M.1. The endpoints of the criterion must be fixed by the actual positive law; only intermediate discrete path values may use the chosen extension.

## 4. What remains to be proved

The repaired bounded-core route needs a quantitative estimate for the **actual transported microscopic scalar and its readout**, on the core-local positive reference law or on its supported perturbation. The old energy reserve and young trial give an upper bound of order P^2 for a larger positive envelope, but that bound is neither a physical-scalar lower bound nor a core-local uniform upper bound.

A proof of a growing physical conditional excess would require, for example, a source-specific posterior lower bound for sufficiently energetic physical births after averaging the competing gauge births and all hidden histories. An upper bound for the local scalar would instead need the appropriate physical fluctuation/thermal cancellation and the fixed scalar/identity extraction. Neither follows from the presently available absolute mass estimates.

The geometry and positivity results in [M04 Bounded Core Source Map](../A_support_and_normalization/M04_Bounded_Core_Source_Map.md), [residual trial mass](../A_support_and_normalization/residual_trial_mass.md), and [M04 Core Label Exclusion Currents](../A_support_and_normalization/M04_Core_Label_Exclusion_Currents.md) remain useful regardless of which conclusion holds. They isolate this problem without weakening the specified physical carrier norm or changing the actual conditional law.

## Mathematical sources

- LFR I (1.73)-(1.101), pp.192-201: bounded prepared core, retained extension test, reference minimum, literal seam and fresh graph/cutoff.
- LFR II (1.5), (1.29)-(1.37), (1.71)-(1.75), pp.357-380: cutoff separation, classical cancellation, residual selector and fixed positive old operation.
- H-03/M-04 marked-source estimates NR20.4-5: actual center-fixed pure-gauge Q seed and its positive weight; NR20.15-18: the distinction between the positive energy envelope and the missing logarithmic normalization control.
- RS.5 and the residual strata analysis: admitted far-pulse geometry and the native descriptor-erased continuity theorem at its stated scope.
- Annex Y M.1-M.12 and M.28-M.39: permissible kernel versions, actual native regulators, elementary discrete changes and compatible tagged currents.
