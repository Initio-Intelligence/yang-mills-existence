# Exact marked reset maps and selector currents

**Annex BB.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 0. Scope

**This note does not close H-03.** It identifies exactly which fresh-coordinate currents vanish in the literal positive R operation, derives the complete selector-crossing current, checks why summing the internal histories of a fixed eligible component does not remove its selection, and gives an explicit positive joint-history reset that preserves the entire source-free output law while changing the marked coupling. It also separates the actual fixed-size continuous integration core from the larger retained-data and history-label footprint.

The last construction is a possible alternative. Its current, regulator and spatial estimates have not been proved. It is not substituted for the fixed-component kernel in the H-03 argument of the earlier annexes.

The source-free construction and admissibility assumptions retain the scope of C-01. Page references below are to the printed pages of Balaban, CMP119 (1988), 243–285, and Large Field Renormalization I and II, CMP122 (1989), 175–202 and 355–392. The marked algebra below is proved directly.

### 1. What the actual source keeps fixed

LFR I printed p.177 defines an eligible component as a whole component of the existing large-field region. It must fit in a cube of side 100 M R, and no new large-field region has been created inside it during the prescribed preceding N steps. These conditions select histories; they do not declare their union to be the unconstrained history space.

Printed pp.200–201 and (1.99)–(1.100) separate the external component domains from the remaining history sums. The localized replacement reference contains its actual integration region, axial tree, cutoff and background. In particular, the component name X alone is not a proof that two history branches use the same reference kernel. The reference data in (1.100) occur within the remaining history sum. Printed p.177 also explicitly distinguishes this localized reference from the schematic full density in the introduction.

LFR II printed pp.378–379 and (1.71)–(1.72) integrate and sum internal histories while holding the eligible component geometry fixed. The cross action is acted on by the same history sum. It is therefore incorrect to replace the fixed-component sum by an unrestricted partition of unity, or to take the old posterior to be the fresh reference law.

The exact positive quotient operation nevertheless provides a useful stronger statement for a correctly fixed reference descriptor. It is the next theorem.

### 2. The exact reset when its reference descriptor is fixed

Let gamma collect every discrete datum that selects the replacement kernel: the integration region, the relevant determining geometry, axial/tree convention and any other branch label on which that reference depends. Continuous retained arguments are denoted v. The definition of gamma is deliberately complete; a coarser label is permitted only after proving that it determines the same reference.

Write u for the old integrated variables, including any remaining old labels whose summation does not change this reference, and u' for the fresh variables. On an active fiber let

\[
 m_\gamma(v)=\int\rho_\gamma(u,v)\,du>0,
 \qquad k_\gamma(u'\mid v)\ge0,
 \qquad\int k_\gamma(u'\mid v)\,du'=1.
 \tag{MG19.1}
\]

Here rho is the entire old positive baseline density at this operation. Any incoming source-free boundary exponential must be included in rho before the posterior is formed. The kernel k is the localized source reference h/H, with the source's numerator and denominator retained together.

#### Theorem MG19.1 — all pure fresh-coordinate reset currents vanish

The literal replacement and its marked quotient are

\[
 (P_\gamma f)(u',v)
 =k_\gamma(u'\mid v)\int f(u,v)\,du,
 \quad \rho'_\gamma=k_\gamma m_\gamma,
 \tag{MG19.2}
\]

\[
 Q_\gamma F(u',v)
 =\frac{P_\gamma(\rho_\gamma F)}{\rho'_\gamma}
 =\frac{\int\rho_\gamma(u,v)F(u,v)\,du}{m_\gamma(v)}.
 \tag{MG19.3}
\]

Consequently the exact reset output is independent of the fresh u' coordinates. Every finite difference or derivative in a pure fresh direction is zero, wherever the same descriptor and retained datum are used. This holds for every coefficient of the full transported finite source jet and of its formal logarithm.

**Proof.** Both numerator and denominator contain the same factor k. It cancels on their common nonzero support. The remaining expression has no u' argument. On null output fibers one may use that same right-hand side as an extension; a newly chosen unrelated reference value is unnecessary. Integrating (MG19.2) first in u' proves exact integral preservation. Applying it coefficientwise to a finite source polynomial proves the full-jet statement. Its constant term is one, so the finite logarithm exists and is again independent of u'. All its covariance and higher response vertices are retained by that algebraic operation. No source-series convergence is assumed. \(\square\)

This is an application to the actual positive quotient in LFR I (1.100)–(1.102), not a claim that the displayed factor T'(X) in a later refactorization is separately independent of every new background argument. If the source divides out a new effective action and moves factors into a boundary exponential, all those factors must be recombined in the actual baseline conditional law before applying (MG19.3).

The conclusion does not make retained v currents vanish. It also does not apply after summing descriptors whose references differ. Coordinate changes that mix fresh variables with v have their own direct pullback records. The theorem identifies the exact zero-current subspace of the reset and prevents a redundant estimate of fresh-reference derivatives that cancel from its true marked quotient.

For an incoming logarithmic jet with coefficients A_B, the output coefficient is the usual full conditional-cumulant partition sum under the old law in (MG19.3). The vanishing above includes every term in that full sum; it is not obtained by retaining only the first input mark.

### 3. Descriptor changes and the full normalized selector current

#### 3.1 A changing reference cannot be canceled across branches

When gamma is itself erased, the actual old posterior at a fixed fresh output is

\[
 \mathbb P(\gamma,du\mid u',v)
 =\frac{k_\gamma(u'\mid v)\rho_\gamma(u,v)\,du}
 {\sum_\delta k_\delta(u'\mid v)m_\delta(v)}.
 \tag{MG19.4}
\]

Thus its descriptor probabilities are proportional to m_gamma times k_gamma. A common fixed-component symbol does not remove the second factor. This formula is Bayes' rule for the actual joint positive density and is valid for discrete, continuous or padded sector inputs.

If the references happen to coincide on the erased family, their common factor cancels and the posterior weights reduce to m_gamma divided by their sum. That is a special case to be proved, not a convention for a normalized component.

#### 3.2 Exact finite differences, including moving support

Let M_0 and M_t be two positive finite unnormalized kernel measures on a common padded space, with masses Z_0,Z_t>0, and put Q_s=M_s/Z_s. For marks F_0,F_t the exact identity is

\[
 \frac{Q_tF_t-Q_0F_0}{t}
 =Q_t\frac{F_t-F_0}{t}
 +\frac1{tZ_t}\int(F_0-Q_0F_0)\,d(M_t-M_0).
 \tag{MG19.5}
\]

The first term is the direct marked response. If F already contains a previous kernel-current record, it is carried inside that direct difference according to its existing compatible decomposition; it is not folded into the newly generated current. The second term is the complete new normalized-kernel current. Equation (MG19.5) remains exact across hard selector interfaces and rank changes represented by the padded sectors.

**Proof.** Add and subtract Q_t F_0. Then write the difference of the two normalized expectations over the common denominator Z_t, using the equality M_0(F_0-Q_0F_0)=0. \(\square\)

Suppose on a given comparison chart one can write

\[
 M_0(d\eta)=\chi_0(\eta)r(d\eta),\qquad
 M_t(d\eta)=e^{\sigma_t(\eta)}\chi_t(\eta)r(d\eta).
 \tag{MG19.6}
\]

The selector weights may be indicators or positive sums of history weights. The exact new current in (MG19.5) splits into

\[
 \begin{split}
 J_t(F_0)={}&\frac{Z_0}{tZ_t}
 Q_0\big[(e^{\sigma_t}-1)(F_0-Q_0F_0)\big]\\
 &+\frac1{tZ_t}\int e^{\sigma_t}
       (\chi_t-\chi_0)(F_0-Q_0F_0)\,dr.
 \end{split}
 \tag{MG19.7}
\]

The first line is the smooth density response. The second is the selector/support response. For real positive data, the latter obeys the exact usable upper bound

\[
 |J_t^{\rm sel}(F_0)|
 \le\frac1{|t|Z_t}\int e^{\sigma_t}|\chi_t-\chi_0|
      \bigl(|F_0|+|Q_0F_0|\bigr)\,dr.
 \tag{MG19.8}
\]

This exposes a required crossing-measure or trace estimate. A bounded analytic tilt with fixed support controls only the first line unless chi_t equals chi_0. In particular, a representation M_t=exp(sigma_t) M_0 with uniformly bounded sigma_t requires equivalent supports. It cannot hold where a positive-measure selector branch is newly admitted or removed.

The pointwise native statement LFR II (1.73)–(1.75) is exactly of the fixed-support type. The paper says on p.379 that only its quadratic B form and self V term depend on the native pair (U,J). It supplies no estimate of (MG19.8) for a different physical change that moves an archived selector.

#### 3.3 Why a fixed-component history sum is not the missing gluing

For a full positive history partition, write chi_h for its weights and let Gamma(h) be the component/reference event being retained. For a prescribed event E, the sum over the histories compatible with E is

\[
 w_E=\sum_{h:\,\Gamma(h)\in E}\chi_h.
 \tag{MG19.9}
\]

Only the sum over the whole partition is one. In general w_E is the probability weight or indicator of the retained selection. A fixed eligible component X is such an event. The source's internal sum does not include the histories with no such component: eligibility was imposed before the sum, and the component domains were explicitly separated from the remaining sums on LFR I pp.200–201.

Thus summing those internal histories can simplify selectors, but it does not justify setting the total selected weight to one. A proof that a particular current cancels must exhibit the relevant complete family of branches and its common marked numerator. Moreover, if the branch has a different fresh kernel, (MG19.4) supplies its additional weight.

This is an exact index-set check of the actual source operation. It is not a lower bound on the size of its current and is not a counterexample to Yang–Mills.

### 4. What gauge covariance is actually available

#### 4.1 The archived approximate-fluctuation selector has a restricted symmetry

CMP119 printed p.250, (1.17)–(1.19), explicitly distinguishes arbitrary simultaneous fine gauge covariance of the effective functions from covariance of the approximate-fluctuation characteristic function. The latter is preserved when a gauge of the new coarse field is extended constantly over its fine blocks. The displayed selector contains the product

\[
 \exp(i g A(b))\,U_1(b)\,U_{1,\Box}(b)^{-1}.
 \tag{MG19.10}
\]

The local approximant is selected from the coarse field in its prescribed axial convention. Under a coarse gauge and its block-constant extension, the two backgrounds and the relative field transform together, and the invariant matrix norm in the selector is unchanged. Haar measure and the Lie-algebra norm are unchanged as well. This verifies the protected real transformation for that actual selector, not merely for a generic gauge-invariant cutoff.

An arbitrary residual fine gauge need not have this property. For example, a fine gauge may be the identity on coarse sites but nontrivial at an interior fine site. The raw averaged coarse field is then unchanged by endpoint covariance, while the prescribed axial approximant remains the one selected from that coarse field. The separately transformed U_1 factor in (MG19.10) need not transform with that fixed approximant. This explains the source's exception directly. The observation concerns the literal selector; it is not an assertion that every such configuration belongs to every later fixed-history fiber.

The source removes these selectors on the regular cells using (1.18)–(1.19). On the remaining cells, (1.21)–(1.25), printed pp.251–252, makes an exact small relocation so the selectors depend only on the raw variables in the large-field region. It does **not** prove invariance under every fine gauge. At a later current insertion those raw variables can be held fixed; changing them or using a different residual gauge still requires the corresponding marked pullback or selector current.

#### 4.2 Preliminary R integration has a genuinely gauge-invariant subintegral

LFR I p.179 explains why the preliminary integrations are needed: several older cutoff factors are not gauge invariant in the variables one would like to transform. Printed pp.194–196 then identify a specific result of those integrations. The second integral in (1.76), on the stated Bo domain outside the untouched old core, is gauge invariant. The first integral, containing the earlier operation T_h on the old core, is left unchanged. The source subsequently fixes the Bo gauge by the actual tree T_0.

For that gauge-invariant subintegral one may transport a mark through gauge fixing by the exact Haar orbit average. If a marked function is gauge invariant on that subintegral, its value is unchanged. For a general mark it must be replaced by its average over the removed gauge variables. This follows by the finite compact-group change of variables underlying the Faddeev–Popov identity; the Haar average is positive, sends one to one and preserves the marked integral. Its logarithmic source jets retain the generated gauge-orbit covariances.

This supplies a marked version of that specific source gauge-fixing operation. It does not make the untouched core selectors gauge invariant. In particular, the source's statement about the second integral cannot be applied to the first integral or to an arbitrary unintegrated marked kernel.

#### 4.3 The proposed hole-patching shortcut needs an additional domain estimate

The source input and output spaces must be kept separate. LFR II p.375, (1.65), has an ordinary new-field input space and a prepared old-field output space. The latter is the multiscale space defined in LFR I (1.64)–(1.69), pp.190–191. Its weaker old-region restrictions do not exempt the corresponding part of the ordinary input from the relative-field condition of CMP119 (2.39).

A proposed converter may agree with the old residual gauge at every hidden raw endpoint and interpolate across a component collar. To keep all old raw variables fixed by a double covariance argument, those endpoint values are prescribed. The sparse-node argument used after scalar integration in C-05 applies because surviving raw nodes have the required terminal mesh grading. Hidden nodes inside T_h do not have that proved grading relative to the newly regular input mesh.

There is an elementary necessary estimate. Let eta be a fine hidden mesh and h the relevant native input mesh. If a gauge interpolant v matches prescribed values at adjacent fine nodes x and x+eta e, then

\[
 h\,|D_\eta v(x)|
 =\frac h\eta\,|v(x+\eta e)-v(x)|.
 \tag{MG19.11}
\]

A value bound on the nodal logarithms alone cannot bound this expression uniformly in h/eta. The analogous second-difference issue enters the native gradient row. A collar-small value exp(−cR) is not by itself a bound for all arbitrarily fine hidden nodes at fixed current R. The current-endpoint estimates in the completed scalar theorem are not spatial finite-difference estimates on those nodes.

This is a limitation of that deduction, not a proof that the actual converter has bad spatial differences. To complete the patching argument, one must prove either the appropriate spatial regularity of the actual nodal values, a controlled-depth reduction of all nodes that really have to be fixed, or a new marked common-domain construction. Fixing only the raw V_h endpoints is less costly, but treating the whole earlier marked T_h operation as unchanged then requires its own exact marked argument. LFR I (1.76) expressly retains that older operation.

#### 4.4 A fixed continuous core is a real improvement, but is not the full kernel carrier

LFR I printed p.192, (1.73), states that the prepared domain Lambda is contained in a cube of side **100 M in current units**. The eligible original component X only had the larger bound 100 M R. The remaining coordinates of (1.76), printed p.194, comprise the old operation on Z_h and the B_0 variables on the complementary prepared shell. The nested prepared rectangles place these continuous integrations in Lambda. The final versions (1.100) and LFR II (1.71) redistribute an old V_h collar; that collar must be followed explicitly, or included in a fixed current-block enlargement of Lambda. It does not turn the integration volume back into the original 100 M R component. Annex BC, Proposition RN19.1, records that support bookkeeping.

This distinction is useful: for marks which depend on continuous hidden variables only, every input participating in a newly generated nonzero cumulant must meet this bounded physical core. A fixed connected cover can join those input carriers with a constant weight. It is unnecessary to pay the original component volume merely to connect continuous variables which are all located inside that core. The number of fine hidden coordinates inside the bounded region can still grow with the remaining depth, so the spatial nodal regularity issue in Section 4.3 is not resolved by the volume bound.

The source does not identify the full normalized kernel carrier with Lambda. LFR II (1.71) still sums the histories restricted to X, and its self action includes the older boundary terms localized in X. Most decisively, the actual native-variation connection set printed on p.379 is

\[
 \mathcal B_0\;\cup\;(\Gamma''_k\cap X^{\sim}),
 \tag{MG19.17}
\]

with subscript **k**, as checked in the published formula. It is not the old h-scale core. The second set contains the current determining variables inside the component; the printed connection statement therefore does not localize every retained-variable response to Lambda. The associated decay is valuable, but its endpoint set and all full carrier weights must remain in the estimate.

A historical domain label may also describe X or a whole earlier layer even when its remaining continuous coordinates lie in Lambda. By M-03's definition, such a label keeps its full dependency footprint until an exact local reindexing or cancellation is proved. One may retain exterior history labels and reset only core labels, but the resulting theorem must then bound the dependence on those retained exterior labels. A scalar factor independent of all erased coordinates cancels from a normalized posterior. A scalar which varies among the histories being erased supplies their relative weights and cannot be canceled term by term.

The source's fixed-core fact removes a specific overly large connector cost. It does not, by itself, prove the missing preintegration common chart, history-current bound, or output-regulator comparison.

### 5. An exact joint-history reset preserving the full source-free output law

The previous obstruction concerns a termwise fixed-descriptor coupling. There is an explicit alternative coupling that shows how one could retain component masses before normalization without changing the unmarked output distribution. This construction is finite and exact. Its estimates are a separate question.

Let the complete family of old descriptors have positive joint density rho_gamma(u,v), and put

\[
 m(v)=\sum_\gamma m_\gamma(v),\qquad
 \rho'_\gamma(u',v)=m_\gamma(v)k_\gamma(u'\mid v).
 \tag{MG19.12}
\]

The sums can be finite or countable with finite positive m on active fibers. The finite cutoff construction has a finite descriptor family after its actual discrete data are fixed. Define a source-independent positive map on the joint old state by

\[
 (P_{\rm mix}f)(\gamma',u',v)
 =\frac{\rho'_{\gamma'}(u',v)}{m(v)}
      \sum_\gamma\int f(\gamma,u,v)\,du.
 \tag{MG19.13}
\]

The zero-mass fibers are null for the baseline and may be assigned the fixed reference convention.

#### Theorem MG19.2 — exact mixture reset and its full marked jet

The map (MG19.13) is positive and integral preserving. On the baseline it has exactly the same full output density, including the retained output descriptor, as the original termwise replacements:

\[
 P_{\rm mix}\rho=\rho'.
 \tag{MG19.14}
\]

Its normalized marked transfer is

\[
 Q_{\rm mix}F(\gamma',u',v)
 =\frac{\sum_\gamma\int\rho_\gamma(u,v)F(\gamma,u,v)\,du}{m(v)}.
 \tag{MG19.15}
\]

It is independent of the fresh output coordinates and output descriptor. It preserves every integrated full source-jet coefficient, hence every original full moment. It is an Lp contraction from the actual old baseline law to the output law, for every 1≤p≤infinity.

**Proof.** Summing rho'_gamma over gamma and integrating u' gives m. Therefore the prefactor in (MG19.13) is a conditional probability density at fixed v. Integration proves preservation, substitution of f=rho proves (MG19.14), and division gives (MG19.15). One can sample the original old variables conditional on v and independently sample the output pair (gamma',u') with density rho'/m. Formula (MG19.15) is the conditional expectation of the old mark given that output. Jensen proves the Lp contraction. Source jets are finite polynomial expressions, so positivity and linearity apply coefficientwise. Their logarithm retains the full conditional cumulant partition rule. \(\square\)

The map uses only the source-free masses and kernels. It does not use a nonzero observable source. Thus, if adopted with its actual footprints and estimates checked, it would remain a frozen source-free mark transport. The unmarked output law and every subsequent source-free operation can be left unchanged. The marked coupling to the past, however, is different from the original termwise coupling. Its use must be recorded explicitly in the transport and history ledgers.

#### What this construction does and does not resolve

The old descriptor weights in (MG19.15) are m_gamma/m. Small component masses remain in those weights. The output mark has zero direct dependence on gamma', so the artificial amplification caused by changing that output label is absent. These are exact identities; they need no analyticity or component estimate.

There are nevertheless additional generated correlations. For two marks,

\[
 \operatorname{Cov}_{Q_{\rm mix}}(F,G)
 =\sum_\gamma\pi_\gamma
       \operatorname{Cov}_{Q_\gamma}(F,G)
  +\operatorname{Cov}_{\pi}
       (Q_\gamma F,Q_\gamma G),
 \quad \pi_\gamma=m_\gamma/m.
 \tag{MG19.16}
\]

Higher orders obey the full law of total cumulance. The second term in (MG19.16), and its higher counterparts, cannot be discarded. They measure changes of the component means across the erased histories.

Nor does a common conditional density make the map local. If the family of descriptors ranges over arbitrarily large or distant geometry alternatives, the dependence footprint of (MG19.15) can grow accordingly. A useful implementation must specify a local family closed under the required history changes, retain the true normalization, and prove its carrier, shifted-current and pointwise regulator estimates. Full-law moment contraction alone is insufficient, as regulator examples already show.

A no-reset branch can be included in the finite algebra only after representing it with the same retained variables and a common padded integration window: its output kernel is its own normalized old conditional law, not a Dirac identity on variables that the other branches erase. Empty and successful branches may then be mixed by exactly the same construction. Whether that common window and denominator retain the required local bounds is an additional source application. Unrepaired residual components cannot be included merely by renaming them as an empty branch.

The positive-gas insertion/deletion approach examined in Annex BC, Section 6, is relevant to this joint alternative: it can keep unnormalized component masses in an estimate before the final normalized mixture is formed. It does not automatically bound the stronger norm of a fixed selected posterior.

### 6. Application conditions and remaining tests

The actual fixed-reference reset has the exact zero fresh-current theorem (MG19.1). The full current formula (MG19.5) and selector decomposition (MG19.7) identify the response that a native fixed-support argument omits. The history-index analysis of the source rules out erasing component selection merely by summing its compatible internal histories. The joint-history map (MG19.13) is an explicit alternative positive coupling preserving the original unmarked output, with all marked responses retained.

None of these statements proves the missing physical H-03 estimate. In particular the following tests remain:

1. For the chosen actual marked representation, identify a preintegration common current chart and its full set of fixed and moving hidden variables. The residual-gauge patch must satisfy the ordinary input domain, not just the prepared output bounds.
2. Bound (MG19.8), or prove exact cancellation in a fully specified joint branch sum, for all retained, selector and geometry changes required by M-03.
3. Prove the actual regulator pullback and shifted-envelope estimates, including all direct and previous/new kernel-current records.
4. Establish the full physical carrier sum. If the joint-history alternative is adopted, also bound the descriptor-mean cumulants and its actual enlarged dependency footprint.

The same source assumptions remain visible. No generic counterexample in this annex is presented as a counterexample to the actual Yang–Mills law.
