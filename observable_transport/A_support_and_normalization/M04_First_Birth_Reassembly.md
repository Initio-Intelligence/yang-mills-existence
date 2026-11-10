# Exact first-birth reassembly and the remaining relative quiet-mask estimate

The exact retained-readout question has a positive answer on the literal ordinary stack used in LFR I (1.2). Reintroducing the actual previously integrated variables gives one original positive path space; the old current field outside a fixed prepared core is the same iterated block average, up to the common reference gauge of that fresh class. At `h=1`, the subclass with `Omega_1` full has an additional useful separation: all later selector functions are independent of the first fluctuation once the first coarse field and its birth geometry are fixed.

This does not yet prove a comparison of the complete old posterior across birth locations. In particular, the other initial P/Q sectors retain microscopic determining data, and the later preparation cutoffs have a smaller logarithmic exponent than the initial R threshold. The exact identities below identify where a relative comparison can work and where absolute error subtraction fails.

## 1. The common retained readout is the literal composition

Let `M_j` denote the actual source block averaging map in the ordinary step from lattice `j` to lattice `j+1`. Define

\[
 \mathcal A_{0:k}
   :=\mathcal M_{k-1}\circ\cdots\circ\mathcal M_0.
 \tag{FR.1}
\]

This is a definition by chronological composition. It does not identify this map with a separately defined direct average without a source identity.

The primitive ordinary transition is

\[
 dH(V_j)\,
 \delta_G\!\left(\mathcal M_j(V_j)V_{j+1}^{-1}\right),
 \tag{FR.2}
\]

as in CMP119 (0.1), its later-step use in (3.1), and Annex W (2.1). Its group delta is normalized against Haar. Consequently a path of ordinary transitions satisfies

\[
 V_k=\mathcal A_{0:k}(U)
 \tag{FR.3}
\]

before the final core replacement, where `U` is the original field at the start of this ordinary stack.

### Proposition FR.1 — exact exterior readout after reassembly

Consider the literal preparation whose last ordinary operations are displayed in LFR I (1.2), and fix a complete fresh class with prepared core `Lambda`. Undo its previous conditional integrations and its exact coordinate changes, retaining all factors. Then its old retained current field on `Lambda^c` is the restriction of (FR.3), in a common reference gauge determined by the fixed class and retained shell. The readout does not depend on the internal old geometric history.

**Proof.** Reinstate the positive integrals which define the completed effective action, together with their ordinary group deltas (FR.2). Fubini/Tonelli does not change those constraints. The nonlinear constraint parametrization also does not change them: CMP119 (1.14)-(1.15) and (3.15) solve the exact group constraint, retaining the exceptional-bond correction and its determinant. The equation `Q C A=0` is the linearized description inside that exact parametrization, not a replacement of the nonlinear delta.

The inserted block gauge transformations fix the next block centers. The gauge covariance of the actual averaging map, CMP98 (11), therefore gives

\[
 \mathcal M_j(V_j^{u_j})
  =\mathcal M_j(V_j)^{u_j|_{j+1}}
  =\mathcal M_j(V_j)
 \quad\text{when }u_j|_{j+1}=1.
 \tag{FR.4}
\]

For the preliminary annular integrations this condition is stated explicitly on LFR I p.182, immediately after (1.25): the allowed gauge is identity on the next lattice. Thus those gauge disintegrations leave the next output, and hence the final retained output, unchanged. Their normalized soft weights or hard tree deltas remain in the reinstated positive path measure.

The final mixed tree `T0` fixes gauge freedom in the integrated core and respects its prescribed exterior anchors. Its history-dependent interior gauge does not alter the retained exterior current field. The subsequent AL reference convention is constructed from the same `U0`, `Lambda` and shell, through (1.85)-(1.87). If a chosen implementation also changes the representative of retained data, that is one common reference-gauge change for this class; undo it once. It is not an old-history-dependent readout. The fresh-class analysis FS.4 keeps the representative rule among the fixed fresh inputs.

Finally the old current variables on `Lambda` are integrated in (1.76). Deleting their fixed-output constraints leaves precisely the exterior restriction of (FR.3). No mixed minimizing configuration is substituted for the original physical field in this argument. \(\square\)

There is a necessary scope qualification. Across an **earlier actual R replacement**, the current field need not be the block average of the original microscopic Wilson field. For such a path (FR.3) starts from the actual field after that earlier replacement, and the earlier Markov kernel remains in the common path law. The present first-birth application uses the literal ordinary stack and does not erase prior reset kernels by an averaging identity.

## 2. What must be reintroduced

Reintroducing only the last-N annular Gaussian variables is insufficient to recover the first full fluctuation law. The retained first-step operation still contains the Schur factor in CMP119 (1.29). Its complement was integrated in (1.26), and its effects occur in the complete `E^(1)` and `B^(1)` terms and in the associated vacuum and Wilson renormalization terms.

To obtain the common first-step law, undo the **whole equality** (1.26)-(1.30), and subsequently the corresponding complete equalities (3.25)-(3.29). This restores the original first-scale variables also on the regular complement of the first bad region. The full precision is then the original first-step `K_0(V_1)`, instead of the Schur precision associated with one retained set. The later full cross action is included in the same undoing. A self-operation alone does not have this identity.

The first boundary relocalization (1.22) must also be undone, with its Jacobian (1.24) and with the mark composed with the actual inverse map. The source explicitly states that this change leaves the free R indicators unchanged; it only changes the representation of the remaining approximate-fluctuation restriction and moves the resulting terms into the action. Thus it causes no ambiguity in the old R pattern when it is undone correctly.

This procedure is exact because the source's effective action is defined by these complete positive integrals. Its named E/R/B pieces, counterterms and normalization constants are not individually discarded. A formal native substitution of the background by the identity is a different operation and does not establish this reassembly.

## 3. The h=1 R-only separation

Assume `h=1` and `Omega_1` is full on the region being reassembled. Then

\[
 \Gamma_0=\Omega_1^c=\varnothing
 \tag{FR.5}
\]

there, by CMP119 (2.2). The initial surviving variable is the first free fluctuation `A_0`; it is not a raw microscopic determining datum in any later minimizing map.

Use the original pre-relocalization first chart. Its reconstruction is the exact source map

\[
 U=\exp\{i[g_0 C(V_1)A_0-hD(g_0C(V_1)A_0)]\}\,U_1(V_1),
 \tag{FR.6}
\]

with the actual coarea/Haar factors. All these fields have first average `V_1`. The first R pattern is determined by the prescribed sup tests on the free entries of `A_0` in (1.18). Write `s` for that complete pattern, or for a disjoint grouping of patterns with the same first geometric data. It is important that grouping sums positive primitive patterns, rather than replacing them by one representative seed.

### Proposition FR.2 — later test functions do not read A0

At fixed first coarse field, fixed first R pattern, and fixed later primitive auxiliary variables, every subsequent ordinary P/Q/R selector and every preparatory selector in the literal final operation is independent of `A_0`.

**Proof.** The later minimizing fields are functions of the determining set of CMP119 (2.2), (2.10)-(2.12). By (FR.5) this set contains only fields on scales at least one, together with the fixed unreplaced exterior; it has no microscopic raw datum generated by `A_0`. The later ordinary test functions in CMP119 (3.2), (3.3), (3.16) and in LFR I (1.3)-(1.9) use precisely those fields, the later free fluctuations, and the prescribed geometric masks.

The preliminary functions (1.22)-(1.28) and the completed function (1.24) use the same later determining fields and later fluctuation variables. The last fluctuation test (1.82) uses the actual mixed variable on `B0`; it does not use the old `A_0` in `T_1`. The last half-threshold test (1.88) uses `(1,V_1)`. LFR I p.194 explicitly leaves the inner `T_h` integral unchanged while performing the preparation on the other variables. These definitions prove the assertion. \(\square\)

This is **functional independence conditional on the displayed data**. The original Wilson density couples `A_0` to `V_1`. The retained first precision, old E/B/R terms, and their reconstructed forms are not thereby independent probabilities.

## 4. An exact common-space formula

Let `y` contain the first coarse field and whatever fixed exterior conditioning is needed. Before the first R decomposition, disintegrate the actual first regular-chart measure as

\[
 d\nu_0(y)\,q_{0,y}(dA_0).
 \tag{FR.7}
\]

Here `q_{0,y}` is the actual normalized first-step law, including the first regular P/Q support and all original density factors. It is not declared Gaussian. If exterior old fields are conditioned, their boundary forces remain in this conditional law.

All later normalized gauge and graph choices can be generated from a common finite auxiliary probability space `Xi`, padded by unused auxiliary variables when an operation is inactive. Once `s` is fixed, Proposition FR.2 makes the later fields and tests functions of `(y,xi;s)`, with no further `A_0` argument. The source gauges may be different functions for different `s`; their exact samplers or Jacobian factors are retained. This does not assert that all histories have identical Gaussian innovation coordinates.

Let `E_s` be the actual first R-pattern event, `I_{r,s}(y,xi)` the indicator of the complete later event leading to fresh class `r`, and `T(y,xi)` the retained readout. Proposition FR.1 identifies the current-field part of `T` with the common exterior block average. Any fixed exterior history data are included in the same conditioning. Then the **entire Omega1-full contribution**, with every first R pattern kept, has the exact positive representation

\[
 \sum_s\int d\nu_0(y)\,d\lambda(\xi)
       \int q_{0,y}(dA_0)\,
         \mathbf1_{E_s}(A_0)\,
         I_{r,s}(y,\xi)\,
         F\bigl(U(A_0,y)\bigr),
 \tag{FR.8}
\]

disintegrated at the prescribed retained value of `T`. The gauge-invariant microscopic mark is evaluated on its physical preimage. The displayed equality applies to each coefficient of the full finite source jet.

Formula (FR.8) is not a chosen young trial submeasure: it sums all first R patterns and all later histories in this subclass. It is also not yet the entire old measure of `r`. Initial P/Q sectors with `Omega_1^c` nonempty have an additional microscopic determining coordinate and must be included separately unless their actual relative mass is bounded.

The common-space formula is strongest as an exact primitive identity. If one instead uses one later Gaussian chart for all `s`, the source has not automatically supplied an identity map between those charts. Its coordinate maps, gauge transformations, determinants and density pullbacks must be retained. The common retained readout alone does not prove those changes harmless.

## 5. The exceptional-bond convention gives a real first-threshold separation

The approximate Q test in CMP119 (1.8)-(1.9) is starred: it excludes the exceptional bonds `b0(c)`. The exact nonlinear constraint correction acts only at those exceptional bonds, as stated immediately after (1.14). Consequently, on the bonds actually tested by Q, (FR.6) has the literal relative form

\[
 \exp(i g_0 A_0(b))\,
     U_1(V_1;b)U_{1,\Box}(V_1;b)^{-1}.
 \tag{FR.9}
\]

The second factor differs from identity by

\[
 O(\varepsilon_1 e^{-c M_2 R_1})
 \tag{FR.10}
\]

on the actual inner stencil, by (1.19). Let `P=delta_0/g_0`. On the admitted logarithmic chart, the complete Q support is therefore sandwiched between free-coordinate norm cutoffs with radii `(2-eta)P` and `(2+eta)P`, where

\[
 \eta=O((g_0P)^2)
       +O\!\left((\varepsilon_1/\delta_0)
                         e^{-cM_2R_1}\right)=o(1).
 \tag{FR.11}
\]

The coarse P test is a condition on `V_1`. The source removes the microscopic plaquette and soft-gauge cutoffs on `Omega_1` when the approximate Q conditions hold and the fixed constant hierarchy `A_0>>A_1` is imposed; see CMP119 p.248 after (1.10). Thus the gap between the R radius `P` and the Q radius approximately `2P` is an actual feature of the source chart. It is not an estimate obtained by ignoring exceptional coordinates.

In a common Gaussian first law, homogeneity makes the Q large-deviation rate approximately four times the minimal R rate. Transferring this statement to the full normalized first law requires a relative density comparison on the actual support. The local comparison and radial support transport of [first birth relative weights](first_birth_relative_weights.md) address that step; no numerical rate conclusion for the entire posterior is inferred merely from (FR.11).

## 6. Why a relative later-quiet estimate is necessary

The preparation cutoff is not at the original R scale. LFR I (1.27), printed pp.182-183, gives

\[
 \delta'_j/g_j=A_1(\log g_j^{-2})^{p_1},
 \qquad p_1<p_0,
 \tag{FR.12}
\]

and (1.82) uses `delta'_k` for the final mixed fluctuation. Even a Gaussian model assigns such a failure an exponent of order `log^{2p1}`, which is smaller than the initial R-birth exponent of order `log^{2p0}`. Subtracting an unconditional preparation-failure probability and then dividing by a rare R mass does not yield a small relative error.

The useful exact algebra is different. Suppose, on the actual retained fiber, that the complete initial events under comparison satisfy

\[
 e^{-\epsilon}p_s\le q_{0,y}(E_s)\le e^\epsilon p_s
 \tag{FR.13}
\]

uniformly in the later admitted data. Suppose also that a common later event `G` implies every compared later admission, and that its probability under the correctly normalized common later measure is at least `1-eta`. If translated first events have the same `p_s=p`, then their complete masses obey

\[
 e^{-\epsilon}p(1-\eta)
       \le Z_s\le e^\epsilon p,
 \qquad
 e^{-2\epsilon}(1-\eta)
       \le \frac{Z_s}{Z_t}
       \le\frac{e^{2\epsilon}}{1-\eta}.
 \tag{FR.14}
\]

The rare factor cancels before estimating the quiet error. In this argument a union bound of the form `exp(CN-c log^{2p1})` is adequate whenever its exponent tends to minus infinity; it need not beat the initial birth cost. The proof of (FR.14) is direct integration of (FR.13) over `G` for the lower bound and over the whole later probability space for the upper bound.

There are two actual applications still to verify. The first-event estimate must cover the **complete event** being compared, rather than just a local witness with uncounted outside R restrictions. The later common event must be constructed from the literal masked variational and preparation tests, and its probability estimated under the correctly normalized common later law. A family of independent Gaussian tests or a native background comparison at a fixed history is not, by itself, that theorem.

## 7. Other initial sectors and older memory

If an initial P or Q sector has `Omega_1^c` nonempty, then `Gamma_0` is nonempty. The later minimal configurations use the retained microscopic variables on that set. The corresponding later tests can therefore depend on the initial microscopic field even after `V_1` is fixed. The common exterior readout FR.1 remains valid on the ordinary primitive stack, but the separated formula (FR.8) does not apply to that sector with the same first variable split.

This is the concrete reason the R-only subclass cannot simply be declared the full conditional. A complete argument must either keep those sectors in an exhaustive exchange construction or bound their true mass relative to the R-only contribution. The actual factor-two Q threshold and the larger P threshold offer a possible rate advantage, but the later admission and normalization must remain in that comparison.

For `h>1` there is another distinction. Reassembling a newly born fluctuation restores its actual incoming density, which includes the inherited action and the surviving `T_h` memory. Unless all preceding actual kernels are undone as well, this density is not the original Wilson first-step law. If earlier R kernels have occurred, undoing the full path still gives a positive primitive law, but the microscopic mark has been transported through those kernels. A new ordinary fluctuation must not be substituted for that mark. The old Schur precisions and inherited E/B/R dependence are precisely the density terms that remain to be controlled in such an extension.

## Mathematical sources

- CMP119, (0.1), (1.14)-(1.30), (2.2), (2.10)-(2.23), (3.1), (3.15), (3.25)-(3.29).
- CMP98, (11): exact gauge covariance of the averaging map. Its later relative-average composition formulas are not replaced by an assumed direct averaging identity here.
- LFR I, (1.2)-(1.9), pp.179-183, (1.25)-(1.29), pp.194-198, (1.76)-(1.89).
- Annex W, (2.1)-(2.4), (4.1)-(4.9): actual primitive positive construction, normalized gauge disintegration and marked path law.
- Companion notes: [M04 Fresh Support Class Cancellation](M04_Fresh_Support_Class_Cancellation.md), [M04 Fresh Class Birth Position](../E_limits_and_targets/M04_Fresh_Class_Birth_Position.md), [birth position dilution](birth_position_dilution.md), [first birth relative weights](first_birth_relative_weights.md).
