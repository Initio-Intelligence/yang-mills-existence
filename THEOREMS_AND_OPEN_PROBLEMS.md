# Theorem catalogue and open problems

The statements below refer to one fixed group $SU(N)$ and to the same sequence of four-dimensional Wilson lattices. Each entry states the required theorem, its present scope, and the hypotheses used to formulate or apply it. A dependency can supply a definition or a conditional implication; it need not be an established estimate.

[Paper](paper/Yang_Mills_Existence.pdf) · [Mathematical scope](SCOPE.md) · [Contents](README.md)

## Common hypotheses

### GC · Uniform Gaussian calibration

Identify the signed sum of projected Gaussian decrements with the composite constrained Gaussian in the same coordinates and prove a bounded remainder from its linear drift, uniformly in depth on the admitted family. The logarithmic coefficient and the finite Schur algebra alone do not bound the transverse remainder. **Status: open for the full application.** [Derivation](native_estimates/gaussian_calibration.md).

### CL · Compatibility of the conditional law

Identify the conditioning variables, selectors, marginal and conditional normalizers, moving support, and derivative coordinates for each estimate used together. Equality of the final Wilson integral under two factorizations is not equality of their conditional laws or their derivatives. **Status: open for the full application.** [Derivation](native_estimates/local_test.md).

## Wilson action and its coupling

[Supporting derivations](coupling/README.md).

### B-01 · Expose the exact positive source-free representation

For the chosen SU(N), identify the actual localized RG/R integral, its reference kernels, selectors, coordinate Jacobians and positive history lift at each scale. Give the equality with the Wilson measure, using $\beta=2N x_0$ and $X_B=N\beta$ throughout.

**Scope.** Source identity, under the published domain and admissibility assumptions. A signed polymer activity is not a history probability.

**Required conclusion.** The published hypotheses and exact integral identity, with every unavailable premise identified; signed polymer activities are never used as history probabilities.

**Dependencies:** definitions and stated hypotheses.

### B-02 · Choose one admissible cofinal geometry

Choose one admitted odd L and integers K_n,M_n giving $a_n=L^{-K_n}\ell_0$ and $T_n=2L^{M_n}\ell_0$. Verify every minimum size, coarse-grid, reflection-plane and coupling ceiling in the actual source-free statements.

**Scope.** Geometric construction. Permitting an expanding sequence of cubic tori does not determine the running coupling or the physical endpoint.

**Required conclusion.** An explicit sequence satisfying all displayed inequalities and permitting every compact support to embed; no unproved rectangular extension.

**Dependencies:** B-01.

### B-03 · Extract the actual one-step coupling remainder

In the source-free Wilson recursion, identify a marginal coupling coordinate u and prove its ultraviolet recurrence $u_{j+1}=u_j-bu_j^2+r_j$ with $b>0$ and $|r_j|\leq A u_j^3$, or a comparably quantified trajectory theorem retaining dependence on earlier couplings.

**Scope.** Conditional on the homogeneous charts and GC. The universal coefficient and the recurrence for a calibrated coordinate have different hypotheses.

**Required conclusion.** The coefficient dictionary, sign, history dependence and uniform remainder are proved for the actual map; a numerical iteration or a native frozen derivative is insufficient.

**Dependencies:** B-01. Additional condition: GC.

### B-04 · Prove stability and asymptotics of the perturbed AF recurrence

Given b>0 and the recurrence in B-03, prove an invariant positive small-coupling interval, reciprocal linear bounds, $u_j=[b(j+\kappa)]^{-1}+O(\log(1+j/\kappa)/(j+\kappa)^2)$, and square-summable tails, uniformly over all admissible remainders.

**Scope.** Arithmetic theorem for a recurrence satisfying the stated uniform error. Its application to the Wilson map depends on B-03.

**Required conclusion.** A complete elementary proof with explicit smallness conditions and constants; actual Wilson identification remains B-03.

**Dependencies:** definitions and stated hypotheses.

### B-05 · Match the trajectory to the finite-cutoff construction

Construct one coherent set of bare Wilson coefficients whose finite-depth RG trajectories stay inside the admitted source-free domains and satisfy the chosen finite physical normalization at ell0.

**Scope.** Open for a prescribed physical endpoint. A positive emergent weak endpoint, conditional on calibration, and positivity of seven finite measurements do not impose that prescription.

**Required conclusion.** Compatibility across cutoff depths and all coupling ceilings, including any shooting or matching argument; no independently chosen incompatible finite trajectories.

**Dependencies:** B-02, B-03, B-04.

## Physical field normalization and products

[Supporting derivations](physical_scale/README.md).

### F-01 · Fix a separating finite field-normalization prescription

Specify the 21 curvature-bilinear representatives, Wick/reflection conventions, seven hypercubic projectors, identity direction, and explicit finite normalization functionals at mu. State a checkable nondegeneracy condition for the finite normalization system.

**Scope.** Finite prescription under its nondegeneracy condition; the uniform inverse problem is F-05.

**Required conclusion.** One concrete prescription whose coefficients and tensor laws can be checked, rather than an unspecified choice of Z; actual invertibility is checked in F-05.

**Dependencies:** B-02.

### F-02 · Absorb logarithmic running into a fixed factorial budget

For a family bounded by $a^\delta C^{m+1}(m!)^p[1+\log(\ell_0/a)]^{\gamma m+\eta}\nu_{qm}$, prove that every $0<\theta<\delta$ gives $a^\theta C_\theta^{m+1}(m!)^{p+\gamma}\nu_{qm}$. Include finite label mixing and logarithmically many errors.

**Scope.** Factorial-budget inequality; no identification with the Wilson fields is required for this implication.

**Required conclusion.** The factorial exponent is fixed, constants are independent of a,m, and convergence is quantitative; no logarithmic factor is hidden in a cutoff-dependent constant.

**Dependencies:** definitions and stated hypotheses.

### F-03 · Compute the seven actual first mixing coefficients

Project the exact regular transported one-field outputs onto the seven fixed hypercubic channels and identify Gamma in $M_j=I+u_j\Gamma+R_j$, with the prescribed field and coupling normalization.

**Scope.** Native Gaussian and regular-channel calculations are available. Open for the exactly transported physical fields.

**Required conclusion.** Seven explicit coefficient formulas or finite invariant integrals with their evaluated normalization; Gaussian/native coefficients must be connected to the exact transport.

**Dependencies:** F-01, M-04, M-05.

### F-04 · Bound the one-step mixing matrix error

Prove $\|M_j-I-u_j\Gamma\|\le C u_j^2$ (or a stated summable substitute) for the actual channel matrices, uniformly in cutoff, carriers, retained backgrounds and histories admitted to this regular calculation.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** A uniform matrix norm with the exact source of every derivative and remainder; symmetry alone does not supply its size.

**Dependencies:** F-03, C-08.

### F-05 · Construct the actual running Z and identity coefficients

Apply the proved commuting-product theorem to the actual matrices, solve the finite normalization system at mu, and construct identity coefficients matching that same prescription. Establish the precise logarithmic coefficient budgets.

**Scope.** Open along a common sequence. Positivity of the seven finite reflected measurements does not bound their reciprocals uniformly.

**Required conclusion.** The inverse matrices, finite normalization determinant and scalar identity coefficients are controlled on the chosen cofinal sequence.

**Dependencies:** B-05, F-01, F-04.

### F-06 · Construct compatible local product subtractions

Specify all source-jet contact coefficients generated by the exact induction using shrinking stencils or point jets; prove compatibility under truncation in m and a linear-in-m spatial distribution order.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** One compatible hierarchy of contacts with explicit bounds and reality/reflection/tensor laws; fixed physical-cell locality is excluded.

**Dependencies:** F-01, M-06.

### F-07 · Close the weighted additive-remainder budget

For the exact matching expansion, bound the sum of inverse-running-product-weighted additive vertices, including identity and collision responses, in the joint observable norm required by S-06.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** The actual series $\sum_j \|T_{j+1}^{-1} R_j\|$ is summable with fixed source-order growth; unweighted summability does not count.

**Dependencies:** F-02, F-05, F-06, M-07.

## Transport of microscopic fields

[Supporting derivations](observable_transport/README.md).

### M-01 · Realize arbitrary frozen kernels as reverse-tail innovations

For a source-free positive Markov RG/R chain on standard Borel history spaces, realize Q_{0:k}F on one path space as a reverse-tail conditional expectation, prove orthogonal innovations and the infinite-depth covariance/tail identity for L2 marks.

**Scope.** Positive-chain identity. The terminal tail is retained.

**Required conclusion.** Replacement noise is included in the dilation; the terminal tail covariance is retained unless a separate triviality/orthogonality hypothesis proves it vanishes. The old finite telescope is a separate identity.

**Dependencies:** definitions and stated hypotheses.

### M-02 · Extend exact microscopic matching to shrinking mesoscopic blocks

Integrate compact Wilson variables by their true conditional laws on independent factor scopes, retaining inherited marginal factors. Prove a scope-radius recurrence and an all-order full-product contact estimate when the final physical radius tends to zero; include blocks of side O(sqrt(a)).

**Scope.** Finite-scale identity and shrinking-block contact estimate. No all-depth transport assertion.

**Required conclusion.** A direct full-Wilson proof for every SU(N), fixed q,p and a vanishing error, with no restart of the original one-link action and no claim that a^-4 becomes the coarse-scale field budget.

**Dependencies:** definitions and stated hypotheses.

### M-03 · Define a current-scale norm for exact transported marks

Choose one explicit localized value/gradient/current norm on the augmented history variables. Show its initial finite-cutoff field values, its carrier geometry and its compatibility with conditional expectation and the source-jet algebra.

**Scope.** Norm and initial bounds specified. For moving support, uniform derivatives require support and normalizer responses; see M-04.

**Required conclusion.** A fully specified norm and initial bounds, including retained-variable dependence; renaming a bare Lp norm a current-scale norm does not meet the test.

**Dependencies:** B-01, F-01.

### M-04 · Match the exact scalar mark through one regular step

At one RG step, expand the actual transported scalar insertion in the fixed incoming reference basis of F-01, under an explicit one-step induction budget, into the current scalar basis, identity term and a localized remainder. Include constrained background, E/B/R responses and coarea terms present in that sector. This does not assume the final running Z from F-05.

**Scope.** Open in the required norm: the original ambient derivative can jump with the integration support. The local-mask construction reaches three regular integrations with separate current origins. Uniform transport of the completed quadratic and moving cores remains open.

**Required conclusion.** Equality with Q_k F_k and a remainder estimate in M-03, uniform in scale; the left side is not a freshly inserted coarse plaquette.

**Dependencies:** M-03, C-08.

### M-05 · Match the remaining tensor channels through one regular step

Perform the same exact one-step matching for all tensor channels, with their hypercubic transformations and every generated retained-field response, in the same norm and normalization.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** All 21 components, including Weyl-type directions, are represented with uniform coefficients; scalar trace matching alone is insufficient.

**Dependencies:** M-04, F-01.

### M-06 · Close the full finite-jet response algebra at one step

For arbitrary source order m, give an exact local expansion for the full jet transported through one step, retaining every collision, reset and remainder vertex; establish a fixed factorial budget for the expansion coefficients.

**Scope.** Open for the uniform iterated application. Bounds on individual coefficients can lose a fixed factor at each step. The analytic-family formulation needs the stated contact and regulator estimates.

**Required conclusion.** Compatibility as m varies and a carrier-bound sum with fixed q,p; a finite truncation of the number of one-field labels is not a truncation of the generated vertices.

**Dependencies:** M-05, C-08.

### M-07 · Prove the all-scale exact matching induction

Iterate the exact one-step expansion over the actual source-free histories with a current-scale field budget and summable irrelevant gains; give the resulting local fields, response kernels and terminal remainder.

**Scope.** Open at arbitrary depth. The clean first-order transfer is conditional; higher-order composite subtractions and marked large-field estimates do not follow from it.

**Required conclusion.** Constants are uniform in total RG depth and volume, with the outer retained-data responses explicitly present; finite-depth mesoscopic elimination does not itself prove this induction.

**Dependencies:** M-06, H-04, F-04.

## The regular conditional measure

[Supporting derivations](boundary/README.md).

### C-01 · Identify every term of the actual conditional density

Write the constrained quadratic form, complete classical action, inherited E/R/B activities, coarea, selectors and boundary terms once each in common current coordinates.

**Scope.** Density identity on a specified representation. CL is required to transfer any derivative or support estimate from a different representation.

**Required conclusion.** A term-by-term identity on the stated domain, not a schematic density; any additional premises are stated.

**Dependencies:** B-01. Additional condition when changing the conditioning law: CL.

### C-02 · Prove a simultaneous current-coordinate E contour

For every localized E carrier, prove a quantitative complex margin for the joint current/background variables used by the marked derivatives, including the independently extended current and preparation factors.

**Scope.** Regular analytic contour on the stated common chart; application requires the same representation as C-01.

**Required conclusion.** An explicit radius and prefactor whose Cauchy derivative bound can be summed over old scales; membership in an open analytic set alone is insufficient.

**Dependencies:** C-01. Additional condition when changing the conditioning law: CL.

### C-03 · Prove the corresponding R contour and marginal transfer

Prove a simultaneous contour for each actual localized R pullback and its marginal/coordinate transfer, retaining the current-dependent extension and denominators appearing in the true construction.

**Scope.** Regular localized contour and marginal transfer on the specified charts. A change to the local R test requires CL.

**Required conclusion.** A uniform holomorphic norm and carrier decay with the verified preparation losses; the source-free R value bound is not differentiated without this domain.

**Dependencies:** C-01. Additional condition when changing the conditioning law: CL.

### C-04 · Sum the actual E/R derivative carriers

Sum the current-coordinate value, gradient and Hessian majorants over old scales and carriers with the actual running radii, coupling sequence and preparation losses.

**Scope.** Carrier-summation theorem under the given radii, scale and preparation bounds. It does not include the whole boundary response.

**Required conclusion.** A displayed small weighted-Hessian budget plus local source-derivative budgets, not just convergence of an unmarked value sum.

**Dependencies:** C-02, C-03. Additional condition when changing the conditioning law: CL.

### C-05 · Control the complete boundary activities

Establish the same local derivative bounds for the actual B and boundary-induced activities, including collars, constraints and current-coordinate dependence.

**Scope.** Open for all required Wilson histories. Two-age summation is valid when both estimates apply to the same subtracted quantity. The anchored response of the stopped reconstruction at fixed earlier innovations, after retaining the common mass, is still needed.

**Required conclusion.** Boundary constants do not grow with total volume or hidden carrier distance; source formulas not verified here remain premises until checked.

**Dependencies:** C-01.

### C-06 · Control heterogeneous blocks and nonconstant backgrounds

Extend the admitted regular derivative/coercivity estimates to the heterogeneous retained backgrounds and layer geometry actually encountered, with explicit weighted norms and domain margins.

**Scope.** Conditional heterogeneous coercivity. Application requires the complete C-05 Hessian estimate on the same domain.

**Required conclusion.** One uniform theorem on the specified admissible class; homogeneous identity-background bounds are not extrapolated.

**Dependencies:** C-04, C-05.

### C-07 · Treat selectors and the integration support

Justify the covariance/IBP argument on the true selected domain, by an admitted convex-core representation with controlled boundary corrections or another complete support theorem.

**Scope.** Support/IBP identity on the stated regular product support; this does not independently establish coercivity on all heterogeneous histories.

**Required conclusion.** Every selector derivative and boundary flux is accounted for; a Hessian inequality on an unrelated open set is insufficient.

**Dependencies:** C-06.

### C-08 · Obtain the complete regular conditional moment and decay estimate

Combine the actual quadratic lower bound and complete perturbation budget to prove current-scale mean, all-p field/gradient moments, and spatial cumulant decay for the selected regular conditional law.

**Scope.** Conditional regular moment and cumulant theorem. Applications require the complete score, Hessian and true selected support; it does not estimate outer history cumulants.

**Required conclusion.** The law is the one in C-01, with fixed factorial growth and volume-uniform constants; its remaining application to all histories is H-04.

**Dependencies:** C-04, C-05, C-06, C-07.

## Retained histories and their response

[Supporting derivations](history/README.md).

### H-01 · Expose normalized history probabilities

Express the law of every retained history and reset under the normalized Wilson measure, with all conditional normalizers and the resampling kernels used in the exact transport.

**Scope.** Normalized path and reset identity; the law includes each conditional mass.

**Required conclusion.** An exact normalized identity suitable for marked expectation; an absolute signed activity is not called a probability.

**Dependencies:** B-01, C-01.

### H-02 · Bound inherited low-margin and unreplaced events

Prove current-scale joint probability or directly marked bounds for inherited low-margin and unreplaced sectors, including overlap and retained-data dependence.

**Scope.** Open. Arbitrary retained large fields obstruct a uniform pointwise bound. An integrated substitute uses native-scale joint events, their shapes, and marked flat-test estimates; it must pay the actual losses in H-04 and S-05.

**Required conclusion.** The exponent and geometric cost compensate the actual insertion/carrier losses in the stated norm; isolated microscopic rarity is not substituted for a coarse event.

**Dependencies:** H-01, M-03.

### H-03 · Localize the exact history-reset responses

Estimate the conditional covariance and higher cumulants generated when a live history label is averaged and resampled, with a carrier radius or decay function uniform in the remaining history.

**Scope.** Spatial cumulants for the mixed reset posterior under its specified law. Its marked use in arbitrary bad histories remains part of H-04.

**Required conclusion.** A spatial response estimate for the exact reset jet, beyond the stated integral identity.

**Dependencies:** H-01, M-01, M-03. Additional condition when changing the conditioning law: CL.

### H-04 · Sum marked bad-history contributions

At one arbitrary scale, sum regular, repaired, residual and inherited bad sectors in the full normalized law for input jets satisfying the M-03/M-06 induction budget, keeping all exact output responses and a fixed factorial growth budget, uniformly over admissible scales and histories.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** One full-law one-step estimate that can feed M-07, with no discarded positive-probability sector and no hidden denominator/volume loss. The all-scale input bounds to be proved in M-07 are not assumed.

**Dependencies:** H-02, H-03, C-08, M-06.

### H-05 · Control the outer retained-mean covariance and cumulants

Bound the variations of the retained conditional means and their higher joint cumulants at each scale and at the terminal physical scale.

**Scope.** Open. A one-sided inner Schur comparison controls a specific normalizer contribution. It does not control the retained marginal’s outside curvature or moving support.

**Required conclusion.** The law-of-total-covariance outer term and its higher-order analogues satisfy the required spatial/terminal budget; a within-sector covariance estimate alone does not pass.

**Dependencies:** H-04, M-07.

## Connected kernels and joint distributions

[Supporting derivations](continuum/README.md).

### S-01 · Pass between connected and full joint distributions

From connected functionals on coincidence-flat joint Schwartz spaces with a common bound $A^{m+1}(m!)^p\nu_{qm}$, p>=1, construct partition full moments on joint tests, independently of contact extensions, with the same q,p; include inverse Mobius and stability budgets.

**Scope.** Joint-test distribution theorem for connected versus full moments under the stated seminorm bounds.

**Required conclusion.** An explicit tensor-product/distribution argument; bounds only on simple tensor tests do not count. Preserve extension independence on flat tests.

**Dependencies:** definitions and stated hypotheses.

### S-02 · Assemble exact connected shells and terminal distributions

Given an exact connected-shell identity, a uniform physical tree-kernel bound and summable shell weights, combine the flat-shell estimate, terminal and one-point budgets into a full joint-test OS hierarchy, with a uniform ultraviolet tail and cofinal convergence.

**Scope.** Assembly theorem conditional on the kernel identity, weights and convergence. It does not supply the Wilson-law bounds.

**Required conclusion.** A quantified theorem with fixed q,p and a correct convergence hypothesis; actual shell identity and kernel bounds remain S-04/S-05.

**Dependencies:** S-01.

### S-03 · Prove terminal and one-point distribution budgets

At fixed ell0, prove the normalized identity/one-point prescription and all-order joint-test terminal distribution bounds uniformly as the torus expands.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** Fixed q,p,C and the same fields as F-05, with no infrared mass-gap assumption used unless independently established.

**Dependencies:** F-05, M-07, H-05.

### S-04 · Identify the actual connected physical shell kernels

Represent exact connected Wilson correlations by the physical shell kernels and terminal term required by S-02, including outer means, collision vertices, history resets and normalization.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** An exact equality on joint tests with precisely located kernel/remainder terms; an algebraic label for the whole unknown correlation is not a localized representation.

**Dependencies:** M-07, H-05, F-06.

### S-05 · Prove the all-order full-law tree-kernel majorant

Prove a uniform bound $A^{m+1}(m!)^{p_0} h_j^{-4m}w_j\exp[-c\tau/((m+d_0)h_j)]$ for the actual kernels, with one common nonnegative weight majorant satisfying $\sum_j h_jw_j<\infty$, or a quantitatively sufficient substitute with a proved fixed-factorial summation theorem.

**Scope.** Open for the complete law. An all-order ultraviolet estimate on flat native tests does not control the transported and retained terms of the physically normalized fields.

**Required conclusion.** Constants, factorial exponent, range parameters and the summable weight majorant are uniform in cutoff, volume, m and history. The normalized complete law is used.

**Dependencies:** S-04, C-08, H-04.

### S-06 · Realize the complete contact and approximation budget

Bound all finite-cutoff stencil, normalization and contact approximation errors in a single vanishing or summable joint-test norm, compatible with the exact hierarchy and positive-time algebra. Specify whether the error is connected or full; use S-01 inverse stability before inserting a full-moment error into a connected-shell identity.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** A fixed q_E,p_E and a cofinal rate, including partial diagonals. Absorb a connected error into the terminal bound or use S-01 stability. The final OS exponents include q_E,p_E; the illustrative (6,7) is not automatic.

**Dependencies:** F-07, M-02, S-04.

## Positivity and translations

[Supporting derivations](foundations/Annex_E.md).

### P-01 · Verify the actual normalization lies in the positive architecture

Check that the constructed field/source substitutions are real, local, reflection-compatible, and split across separated time half-spaces, including all required tensor Wick phases.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** Apply the existing Gram-congruence theorem to the actual coefficients; arbitrary symmetry of a counterterm does not replace the splitting identity.

**Dependencies:** F-05, F-06, S-06.

### P-02 · Verify translation and permutation compatibility of the realization

For the chosen lattice representatives and any auxiliary block skeleton, prove exact fine-lattice translation symmetry or a vanishing translation defect, plus permutation symmetry of the full hierarchy.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** The common seminorm controls approximation by fine translations; a fixed physical cell-grid symmetry is insufficient.

**Dependencies:** P-01, S-05, S-06.

## Rotations of the action and fields

[Supporting derivations](energy_and_symmetry/angular_implication.md).

### R-01 · Identify all finite hypercubic rotational splits

Write the three compatibility relations that join the seven hypercubic channels into the four rotational tensor types for the actual field normalization.

**Scope.** Finite-dimensional compatibility relations. Their validity for the interacting normalization is a separate estimate.

**Required conclusion.** Explicit channel coefficients and finite normalization conditions; the representation classification is an algebraic input.

**Dependencies:** F-03.

### R-02 · Bound the action's angular defect

Express the angular variation of the normalized effective action as local defect carriers plus controlled remainders and show their contribution vanishes on fixed physical tests.

**Scope.** Conditional on coefficient contraction and full-law localization on the chosen Wilson sequence.

**Required conclusion.** A bound for each rotation generator on the actual full law, including nonlocal tails and inherited terms; hypercubic invariance alone is insufficient.

**Dependencies:** C-08, H-04.

### R-03 · Bound the observable and contact angular defects

Prove the matching fields, running matrices and product contacts transform with a vanishing defect under each continuum angular generator.

**Scope.** Conditional on exact marked transport, contact control and coefficient matching.

**Required conclusion.** All 21 labels and all source orders with the same normalization as S0; scalar action isotropy does not determine tensor normalization.

**Dependencies:** R-01, M-07, F-06.

### R-04 · Obtain a common rotation-defect budget

Combine action and observable defects into a uniform joint-test estimate stable under the finite parameter paths used to integrate each fixed rotation.

**Scope.** Conditional joint-test theorem integrating generator bounds uniformly along a rotation path.

**Required conclusion.** A rate tending to zero with the cutoff for each fixed rotation and joint test, with no unproved uniformity over intermediate rotations.

**Dependencies:** R-02, R-03, S-05.

### R-05 · Apply the angular reconstruction and reflection checks

Integrate the stated generator reduction and use the exact discrete reflection to establish full O(4) covariance of the limit, including tensor labels.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** Full covariance for the same limiting hierarchy, without averaging rotated theories or replacing the original hierarchy.

**Dependencies:** R-04, P-01, P-02, A-01.

## Short-distance coefficients

[Supporting derivations](energy_and_symmetry/README.md).

### U-01 · Identify the normalized two-point leading coefficient

Compute the prescribed scalar/tensor two-point coefficient in the exact matched normalization and coupling dictionary, including logarithmic running.

**Scope.** Comparison coefficients available; open for the physically normalized interacting hierarchy.

**Required conclusion.** A specified distribution and coefficient; the computed native/Wick coefficient is used only after its matching is proved.

**Dependencies:** F-05, M-07.

### U-02 · Identify a specified nonzero connected three-point coefficient

Compute the target connected three-point coefficient on an explicit admissible profile and prove it is nonzero in the same physical normalization.

**Scope.** Separated nonzero comparison terms available; connected identification and uniform interacting errors remain open.

**Required conclusion.** A definite coefficient with a checkable nonvanishing witness and correct distinction between connected and full moments.

**Dependencies:** F-05, M-07.

### U-03 · Bound the interacting two- and three-point UV remainders

Prove the coefficient formulas with remainders uniform in cutoff and expanding volume before the short-distance limit, retaining all exact matching and history contributions.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** The order of limits is justified and the nonzero coefficient survives; a finite-order formal expansion is insufficient.

**Dependencies:** U-01, U-02, S-05.

### U-04 · Prove the reflected four- and six-field block estimates

For the two positive-time UV block observables used in Annex L, prove the interacting vacuum norm remainder after subtracting the prescribed scalar coefficient.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** A summable logarithmic-scale error on a common test-space norm, with the correct reflected two-block geometry.

**Dependencies:** S-05, U-03.

### U-05 · Control scale derivatives and all compact UV profiles

Establish the same interacting block norm budget for the logarithmic scale derivative and the quantitative profile continuity required for the continuous-scale phase-transfer theorem.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** The error is integrable/summable in the specified scale norm and uniform on the required bounded test sets, not only a countable sequence of numerical profiles.

**Dependencies:** U-04.

## Energy bounds and periodic states

[Supporting derivations](energy_and_symmetry/README.md).

### E-01 · Prove a local-cylinder alternative for periodic state passage

Derive the exact local periodic/vacuum path-law density and a sufficient local total-variation or entropy comparison, with explicit cutoff observable budgets, that transfers vacuum slab estimates to periodic OS forms without the global thermal trace condition.

**Scope.** Local-cylinder transfer criterion; the required cofinal comparison remains E-05.

**Required conclusion.** A quantitative bridge covering the physical a^-4m losses and fixed polynomial vectors; actual convergence/rate is E-05.

**Dependencies:** definitions and stated hypotheses.

### E-02 · Prove the renormalized scalar arbitrary-vector bound

Bound the actual scalar logarithmic transfer response or periodic OS insertion after physical renormalization, including its prescribed identity coefficient, uniformly in the cutoff.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** An arbitrary-vector heat or graph estimate with the required common domain; pressure derivatives and vacuum moments are insufficient.

**Dependencies:** F-05, M-07.

### E-03 · Prove the renormalized pseudoscalar seed bound

Establish the corresponding operator estimate for the correctly normalized pseudoscalar field, including any electric/magnetic mixed realization and domain.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** Uniform physical energy weight and Schwartz seminorm for the actual field; a scalar or bare plaquette estimate is not substituted.

**Dependencies:** F-05, M-07.

### E-04 · Prove the renormalized off-diagonal magnetic seed bound

Upgrade the compact magnetic comparison to the actual continuum-normalized B1B2 seed, controlling physical powers, running mixing and temporal admixtures.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** A cutoff-uniform physical estimate; the existing dimensionless compact bound with a^-4 loss remains an input, not the conclusion.

**Dependencies:** F-05, M-07.

### E-05 · Verify the chosen periodic-state transfer criterion

On one admissible cubic cofinal sequence prove either the local state-comparison rate in E-01, the retained thermal trace-increment criterion, or a direct periodic OS insertion bound.

**Scope.** Open on cofinal cubic tori. Fixed-volume trace bounds and a finite-torus comparison criterion do not give the required uniform local state comparison or a gap.

**Required conclusion.** The criterion applies to the actual renormalized hierarchy and all fixed polynomial degrees; fixed-volume large-time convergence alone does not count.

**Dependencies:** E-01, B-02.

### E-06 · Apply the field-domain and three-seed theorems

Pass the established seed bounds to the reconstructed fields on the common graph core and then use the finite Lorentz-orbit theorem to obtain all 21 field estimates.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** The field identified by reconstruction is the bounded extension under discussion, and all domain/covariance hypotheses are checked.

**Dependencies:** E-02, E-03, E-04, E-05, R-05, A-02.

## Decomposition into vacuum phases

[Supporting derivations](foundations/Annex_V.md).

### V-01 · Characterize disconnected symmetry in selected phases

For a valid translation-ergodic decomposition on a specified separable bounded algebra, prove a criterion for almost-everywhere finite/disconnected symmetry invariance using central defects P0(alpha_g(A)-A)Omega and macroscopic translation averages.

**Scope.** Central-defect criterion conditional on a valid phase decomposition; a symmetric mixed state need not have symmetric individual phases.

**Required conclusion.** A simultaneous common-null-set theorem and exact defect norm formula; invariance of the mixed state or a common UV coefficient alone is not used to infer phase invariance.

**Dependencies:** definitions and stated hypotheses.

### V-02 · Verify the actual decomposition theorem hypotheses

Apply a precisely scoped phase decomposition theorem to the actual finite field family, with its generalized energy or proved intrinsic-locality hypotheses, measurable fields and symmetry representation.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** A valid field decomposition with measurable closed fields, proper-orthochronous covariance, unique translation-invariant vacuum and clustering in the phases, and the required phasewise field energy domains. Disconnected symmetry is separately V-04. Vacuum OS moments alone do not verify the decomposition hypotheses.

**Dependencies:** A-02, E-06.

### V-03 · Transfer the specified UV coefficients to one common phase set

Apply the existing block-variance/continuous-scale theorem simultaneously to both required coefficients, all specified profiles and normalizations.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** One common full-measure set retaining the prescribed coefficients, not merely some phase with a nonzero cumulant.

**Dependencies:** V-02, U-04, U-05.

### V-04 · Verify the required disconnected phase symmetries

Prove the actual central symmetry defects vanish for the finite disconnected symmetries required by P1, or give another valid selection theorem supplying them.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** A phasewise symmetry statement for the selected theory; symmetric mixtures of symmetry-breaking phases are not accepted.

**Dependencies:** V-01, V-02.

### V-05 · Select a phase with all required properties

Intersect the verified full-measure sets and select a phase with the required finite field family, common energy domains, proper-orthochronous covariance, the required disconnected symmetries, unique vacuum, clustering and the fixed UV coefficients.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** The selected phase is nonempty and each requested property is established for the same field normalization and phase.

**Dependencies:** V-03, V-04, E-06.

## Continuum existence and identification

[Supporting derivations](paper/Yang_Mills_Existence.pdf).

### A-01 · Extract the compatible continuum hierarchy

Apply the proved cofinal compactness theorem to every order and field tuple on a countable dense flat-test family, then extend by the common seminorm bound.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** One subsequence for the entire hierarchy, preserving normalization, positivity and symmetry; no uniqueness assertion.

**Dependencies:** S-02, S-03, S-05, S-06, P-01, P-02.

### A-02 · Apply corrected OS reconstruction to this hierarchy

Verify the corrected OS II regularity and covariance hypotheses for the constructed full moments and reconstruct the relativistic fields without imposing clustering at the initial mixed stage.

**Scope.** Open for the stated Wilson hierarchy.

**Required conclusion.** A source-scoped reconstruction application with the actual fields and common domains; an abstract reconstruction theorem is not counted as construction of its inputs.

**Dependencies:** A-01, R-05.

### A-03 · Identify the limiting fields with the stated existence target

Identify each conclusion of the existence theorem with its corresponding estimate, field normalization and phase, and obtain an identification with no unsupported cross-reference or scope extension.

**Scope.** Open identification theorem for the stated fixed-group existence target. No positive spectral gap is derived.

**Required conclusion.** The unconditional conclusion requires every Wilson-law hypothesis to be proved. A remaining Wilson-law estimate prevents a claim of Yang–Mills existence.

**Dependencies:** A-02, V-05, U-03.
