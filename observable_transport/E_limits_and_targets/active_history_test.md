# M-04: active-history energy test after repairing the ambient extension

This note tests an actual-model obstruction on positive-mass fibers. It does not use the artificial inactive-fiber discontinuity. It also does not prove the missing M-04 marked-kernel bound.

## 1. Proposed mechanism and its necessary conditions

The proposed mechanism is concrete. A birth-scale bad plaquette selector can require

\[
 \beta_0\sum_{p\subset D}s(U_p)\ge c\beta_0\varepsilon_0^2
       =c_N P(g_0)^2,                                     \tag{AH.1}
\]

where \(\varepsilon_0=g_0P(g_0)\), \(P(g)=A_0[\log(g^{-2})]^{p_0}\), and the Wilson convention is \(\beta_0=(Ng_0^2)^{-1}\). The bad cube has volume \(O(R(g_0)^4)\), with \(R(g)\asymp[\log(g^{-2})]^r\). If the microscopic energy were integrated out while its bad flag remained fixed, and if the output native regulator were bounded, then a scalar averaging argument would suggest

\[
 \max_{x\in D}h^4|QF_x|\gtrsim
           \frac{P(g_0)^2}{R(g_0)^4}.                    \tag{AH.2}
\]

Since \(p_0\ge5r\), the right side grows at least as a positive multiple of \([\log(g_0^{-2})]^{6r}\). The ordinary centering contribution costs only O(R^4), so it would not remove a P^2 total-energy lower bound.

For (AH.2) to refute a pointwise M-03 estimate, all of the following must hold simultaneously:

1. the specific event enforcing (AH.1) is measurable in the actual output state, rather than a retained label subsequently averaged by the true posterior;
2. its old energy coordinates have actually been erased from the native output list;
3. the actual output carrier, including the event's full defining footprint, has a bounded native regulator;
4. the output is the true conditional scalar under that state, not an additionally conditioned version.

The literal source construction does not supply this combination in the proposed first-birth/fresh-reset cases. The exact reasons differ for the three classes of history.

## 2. Before replacement: the bad microscopic coordinates are retained

CMP119, printed p.256, states that in the first step the integration in
\(U|_{\Omega_1^c}=V_0\) is left unchanged. It then describes the corresponding retained fields \(V_{j-1}\) at later ordinary steps and puts them into the mixed-scale determining configuration, (2.10). The actual C7.2 regular kernel integrates the independent free coordinates in the regular interior. Its outer data include those retained exterior variables.

The initial curvature test is CMP119 (1.1). If a cube D belongs to P0, at least one plaquette in its tested footprint has

\[
 \|U_p-I\|\ge\varepsilon_0.
\]

The source's padding places this footprint in the old exterior whose raw compact field V0 is retained. It is not an erased regular-interior coordinate. On the compact group,

\[
 s(U_p)=\tfrac12\|U_p-I\|_{\rm HS}^2,
\]

so, after the harmless fixed norm conversion if the source uses operator norm,

\[
 R_{h,X}\ge1+c_N\beta_0\varepsilon_0^2               \tag{AH.3}
\]

for every actual carrier X containing that test's full native footprint. M.5 uses the actual retained/native plaquette list, not just the newest coarse field. Deleting the V0 contribution from this regulator would violate its definition.

There is also an elementary alternative: if an insertion remains simply the microscopic local Wilson scalar in the retained old field, its original local stencil already controls its own value. One must not force it onto the entire large component merely because a separate geometry flag was recorded elsewhere.

The ordinary free-field bad selector (CMP119 (1.18), or (3.16)) gives a related statement. Its bad witness is a free coordinate outside the new regular integration domain. That retained dimensionless free coordinate contributes its square to M.5. Thus a large retained free fluctuation is not hidden from the prescribed native regulator. The exact printed cutoff and rescaling convention must be kept: the source analysis records an ambiguity in the general-step notation, so this note claims the literal lower bound \(R_{h,X}\ge1+r_{\rm cut}^2\), not an unverified conversion of every such cutoff to P(g)^2.

These statements concern the actual regular inner kernel of C7.2. If one instead integrates all exterior variables and conditions on a finer primitive history, one has chosen another conditional operator. Its norm application must be stated and proved separately; it is not a counterexample to that regular kernel by relabeling its output.

## 3. Successful replacements: the old bad event is not retained conditioning

The actual post-reset variables are specified in HS20.4: the new field, the unreplaced exterior data and the residual Y geometry. The successful component family C and every internal old state \(\eta_X\) are integrated in the posterior. Successful components retain their unnormalized positive masses \(M_X\); they are not normalized one at a time and then inserted as certain events.

For a nonnegative old energy E and a retained birth event B implying E≥a, the exact true conditional inequality is

\[
 Q_vE\ge a\,\pi_v(B),                                   \tag{AH.4}
\]

not Q_vE≥a. Replacing \(\pi_v(B)\) by one conditions on an extra event that the H-03 output has averaged.

The source's deletion comparison makes the distinction quantitative for a successful species:

\[
 \pi_v(X\in C)\le e^{\lambda_X}M_X(v,1).                \tag{AH.5}
\]

Here the positive component mass stays on the right. The source and source text prove exponential suppression in P(g) for that mass. Since p0≥5r>4r, this suppression is stronger than the exponential physical-volume cost of a component of side O(R):

\[
 e^{-cP(g)}e^{C\kappa R(g)^4}\longrightarrow0.          \tag{AH.6}
\]

LFR II printed p.389 makes precisely this type of payment in (1.92)–(1.97). This does not by itself bound an arbitrary marked numerator; the full energy dictionary remains necessary. It does show why the proposed deterministic lower bound cannot simply be passed through the successful-geometry erasure.

In particular, a pointwise conditional calculation at a flat new field may still involve successful old bad histories, but their actual probabilities remain present. Conditioning on the presence of one such X would change the state and the operator.

## 4. Residual replacements: the fresh bad test forces output energy

The residual components Y_i are different. LFR II printed p.378 classifies components using the final fresh test. The successful class carries the good factor \(\chi_k(X_i^6)\); the residual class carries \(\chi_k^c(Y_i^6)\). The residual Y geometry is retained. Its old internal states and descriptors are still averaged in HS20.4.

It would be incorrect to infer a raw curvature lower bound merely by contraposing the one-way statement on p.378 that \(\chi_k=1\) implies \(|dV_k-I|<2\varepsilon_k\). Instead use the actual variational regularity theorem.

### Proposition AH.1 (an active residual component has a native witness)

Let Y be an active residual component, and let W_Y contain the full current-field determining footprint of its literal final test \(\chi_k^c(Y^6)\). On the source's admitted small-coupling class there is a fixed constant C_var such that at least one actual retained current plaquette p in W_Y obeys

\[
 \|V_k(\partial p)-I\|\ge\varepsilon_k/C_{\rm var}.      \tag{AH.7}
\]

Consequently, for a carrier X containing that footprint,

\[
 R_{h,X}\ge1+c_N\beta_k\varepsilon_k^2
           =1+c'_N P(g_k)^2.                            \tag{AH.8}
\]

### Proof

CMP119 (2.16)–(2.17), printed p.257, defines \(\chi_k\) by the local minimizing fields \(U_{k,\Box}(V_k)\). The defining data are the actual current field restricted to the enlarged local cube, through the explicit prolongation and determining-set construction. The same local construction is used by the fresh component test in LFR II p.378.

Theorem 1 of CMP102, printed p.279, puts a minimizing field with sufficiently small determining-data plaquette bounds a in the regular class with bound B3 a. In a current k-scale interior test cube, the resulting fine plaquette bound is B3 a times the exact scale factor \(\eta^2\) used in (2.17). The fixed conversion from the raw current plaquette bounds to the compatible determining-set bounds is included in C_var; it uses the literal local prolongation (CMP119 (1.3)/(2.16)), whose nontrivial plaquettes are copies of compatible current plaquettes. No old component state is inserted into these new-field test data.

If every actual current plaquette on W_Y were smaller than \(\varepsilon_k/C_{\rm var}\), with C_var chosen larger than twice the variational comparison constant, all the local minimizing-field tests entering \(\chi_k(Y^6)\) would have strict margin below \(\varepsilon_k\eta^2\). Hence \(\chi_k(Y^6)=1\), contradicting the active residual factor \(\chi_k^c(Y^6)\). This proves (AH.7).

The compact Wilson identity and fixed trace normalization give

\[
 \beta_k s(V_k(\partial p))
 \ge c_N\beta_k\varepsilon_k^2.
\]

This plaquette is an actual retained native variable on W_Y, so it appears in M.5 for every X containing that footprint. Since \(\varepsilon_k=g_kP(g_k)\) and \(\beta_k=(Ng_k^2)^{-1}\), (AH.8) follows. QED.

In particular, a completely flat new field is not an active residual datum. More strongly, active residual data cannot have bounded native energy on the complete fresh-test footprint as g tends to zero. An argument which assigns a residual Y flag but sets its full new-field stencil to a flat or uniformly bounded-energy datum is again testing an inactive or incompatible state, even if it avoids the specific default reference convention of the previous note.

### Carrier qualification

The footprint in this proposition must actually be present in the proposed carrier. The residual-component indicator is a history variable whose definition tests the indicated entire region. M.1 requires that full defining footprint. If a conditional scalar is independent of a fresh variable after an exact quotient cancellation, that independence can reduce its field dependence, but it does not permit deleting a residual history indicator on which the represented activity still depends. Conversely, an activity truly independent of the component and its indicator need not be assigned that component's full support. No universal lower bound for every small scalar stencil is asserted by (AH.8).

## 5. A retained bad geometry does not specify a bad Wilson seed

Even before the preceding output-energy issue, the initial lower bound (AH.1) must identify the right bad event. The source has several different selectors. A generic bad component can be born from the approximate-fluctuation test Q1, not only from the physical plaquette test P0.

NR20.4 of [Annex BJ](../../history/Annex_BJ.md) gives an actual source configuration with

\[
 U(e)=u(e_-)u(e_+)^{-1},\qquad
 U_p=I,\qquad V_1=I,
\]

and a center-fixed local gauge transformation satisfying
\(3\delta_0<\|u(x)-I\|<4\delta_0<\varepsilon_0\).
The soft gauge factor remains positive, P0=P1=empty, but Q1 is bad. These strict inequalities persist in a positive-volume neighborhood whose Wilson curvature can be made arbitrarily small. This proves that the implication

\[
 \text{an initial source component is bad}
 \Longrightarrow\beta S\ge cP(g)^2
\]

is false for the displayed soft-gauge source convention. The soft-gauge action, rather than the physical Wilson action, pays that particular seed.

After H-03, the precise P0/Q1/R1 and preparatory descriptors are part of the averaged old internal state \(\eta_Y\), not retained output labels. A lower bound conditioned on P0-bad cannot be silently applied to a residual component conditioned only on Y. A theorem showing that a particular final Y forces P0-bad would require an additional source-specific history implication. The supplied pure-gauge example is a birth-level statement, so this note does not claim it realizes every possible final eligible Y.

This does **not** prove that normalized old Wilson energy is small on every residual component. Rare selection can raise a conditional mean even when it does not impose a pointwise lower bound. The point is that the proposed deterministic lower-bound proof has not identified a retained event that enforces its premise.

## 6. What is settled and what remains

The candidate low-output-regulator obstruction does not yield an actual M-04 counterexample in the identified cases:

| Actual source state | Why the candidate inference fails |
|---|---|
| Ordinary regular kernel before replacement, with P0 bad exterior | The bad microscopic plaquette is a retained native coordinate; its energy remains in the regulator. |
| Ordinary exterior free-field bad witness | Its retained dimensionless free coordinate remains in the regulator. A Wilson-energy lower bound is a separate issue. |
| Successful component after true H-03 averaging | The old component and bad seed are averaged with their actual mass; replacing their conditional probability by one changes the kernel. |
| Residual component after H-03 | The active fresh bad test forces a large actual new-field native energy on its full footprint; flat/bounded-energy configurations with that flag are inactive. |
| Generic initial bad geometry or a residual geometry without its old seed descriptor | It does not identify a P0 Wilson-curvature event; pure-gauge Q1 seeds invalidate the generic birth-level implication. |

These are actual source/state distinctions, not a replacement toy model. They do not prove an upper bound for normalized old energy, its derivative, or its full physical carrier decomposition. In particular the independent exponential-volume obstruction could still occur even when the pointwise output regulator is large: an activity may depend on a whole component without amplitude suppression proportional to that volume. Proving or disproving that possibility requires actual supported output coefficients or a representation-independent active-fiber lower bound. Neither is supplied here.

The remaining concrete estimate is still the full normalized old-moment/current comparison and actual marked-root localization, with the complete native coordinate list. A source upper bound for an unnormalized component mass is not a lower bound for its normalizer. Conversely, an invented deterministic bad-seed condition cannot replace the actual posterior. This test rules out that proposed shortcut while preserving the precise unresolved estimate.

## 7. A proposed successful-species active jump is removed by the common selector

Another proposed obstruction is that a successful species X has a retained-field cutoff in its mass, so its contribution might turn off discontinuously while the absent-X branch remains positive. For the literal successful-sector factor, the source rules this out.

LFR II printed p.378 says that the successful-component small-field factors \(\chi_k(X_i^6)\) are combined with the old regular factor \(\chi_k(\Omega_k^4)\). The common-background construction of pp.365 and 378–379 puts these into the new regular small-field factor. HS20 §1 states this precisely: at fixed new field, unreplaced exterior and residual Y geometry, the successful family C is summed while the new determining data and new regular small-field factor are common.

If X is absent, its region is filled by the regular background of that branch. Its small-field test is therefore already part of the same common output support. If X is present and successful, the test is imposed by the successful factor and then incorporated into that same support. On the common active set it is identically one in either representation. A field change that makes this particular χ_X fail consequently violates the fixed output's common regular selector; it does not leave an active absent-X branch with the same retained Y state.

Thus the simple successful-species threshold argument would only reproduce an off-support change, not an extension-independent active jump.

The residual bases are different. Their descriptor-dependent exterior-extension selector \(\chi_{k,\Lambda_\gamma}\), fresh cutoff \(\chi_\gamma\), and gauge-slice factors remain inside \(\mathcal B_Y(v,d\eta_Y)\); HS20 explicitly warns not to cancel them as common v-only factors. A genuine active jump would require exhibiting two actual residual descriptors with positive conditional mass, a raw path where one supported measure changes discontinuously while the other survives, and a nonzero scalar conditional mismatch. The abstract fact that such mixtures can jump is not that actual-source construction. No such counterexample is claimed here.

## 8. Residual strata and old normalizers

The source-specific residual-stratum analysis is given in [M04 Residual Strata Analysis](../A_support_and_normalization/M04_Residual_Strata_Analysis.md). It proves a no-continuous-version criterion for two actual positive strata and derives a same-Y/different-prepared-core geometry from the literal no-new-field rounding operation. Direct inspection of CMP119 (3.5), (3.20) gives a stronger fact: two no-new-field histories with the same final rectangular Y have the same current old hole \(\Omega_k^c\), although their prepared O(M)-size replacement cores can be separated by O(MR_k).

The same-lattice variational nesting lemma there uses the exact determining shells (2.2) and recursive averages. It allows a quiet old history to be constructed from a single final-constrained Wilson minimum, with zero true regular fluctuations. A strict pure-gauge birth seed can then be added without changing any later average. The remaining proposed active output has a moderate physical curvature witness in the common old hole, outside both cores, and flat current plaquettes near one core. Different fresh graph strata then distinguish whether that local current scalar was reset or retained.

The note supplies a source Hessian/locality estimate for the fresh reference cutoff and identifies the precise final preparation-coordinate analysis. It has **not** been used here to claim a counterexample for the particular already transported microscopic M-04 scalar. Even if the native-current version is completed, that observable identification remains separate.

The proposed old-energy partition lower bound is examined in [M04 Residual Normalizer Test](../A_support_and_normalization/M04_Residual_Normalizer_Test.md). The quiet chronological period in LFR II (1.80) is N=R_j, while the shorter preparatory N_0 is O(log R). Eligibility bounds each of those last N domains in its own lattice units; their total remaining rank is at most O(R^5), whose O(R^5 log β) trial entropy **is** paid by one P^2 native witness. Exponential rank does not follow from the quiet age alone. The genuinely arbitrary earlier history remains in the unchanged T_{k−N}, and its Gaussian/determinant/vacuum factors cannot be discarded. A promising denominator trial would replace that older internal history by a fresh h-scale birth with the same prepared core and fresh graph, inside the exact history sum; its prior renormalized density still needs a source-specific lower bound.
