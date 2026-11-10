# The third homogeneous integration: analytic base and two inherited defect generations

This note performs one more actual homogeneous integration after AD's complete two-step density. Each R partition is summed with its mass; the three P/Q-regular regions are the full lattice. The operation is the density-state physical averaging operation of RA/BA/TD, not an assertion that the original history kernels can be used after their labels have been erased.

The result concerns the actual analytic base, the primitive Gaussian and interaction certificates for both inherited Q-defect generations, and their common normalized gas. It supplies the source-free kernel and normalization inputs to the third marked calculation. A microscopic marked energy--velocity bound is a separate calculation; it is not inferred from a bound on the unmarked mass. Constants and carrier-rate losses in this note may depend on three fixed levels.

## 1. Exact input and bookkeeping for the leading action

Use integrating couplings \(g_0,g_1,g_2\), final retained coupling \(g_3\), and fields \(V_j\) at \(h_j=L^jh_0\). Set
\[
 p_0=\delta_0/g_0,\qquad
 p_1=c_1\delta_1/g_1,\qquad
 p_2=c_2\delta_2/g_2,\qquad
 P_{Q,i}=\delta_i/g_i\quad(i=1,2).
 \tag{TC.1}
\]
The positive fixed fractions \(c_i\) are sufficiently small for the strict Q-domain containment. The comparison radii \(p_1,p_2\) are introduced after the corresponding exact R sums. They are not the printed later R-good radii. The entire Q fiber, and every contour used for it, is covered using \(P_{Q,i}\), not the smaller \(p_i\).

AD gives the exact positive two-step density
\[
 \rho_{QQ,2}(V_2)=\rho_{\mathrm{aux},2}(V_2)e^{E_2(V_2)},
 \qquad
 E_2=H^{[0]}_2+H^{[1]}_2,
 \tag{TC.2}
\]
where \(H^{[0]}_2=\Delta_2\) contains at least one first-integration Q defect and \(H^{[1]}_2=\delta E_{\mathrm{new},2}\) contains at least one second-integration Q defect. Their complete parametric integral representations are retained.

It is unnecessary, and would require an additional scheme comparison, to identify the auxiliary cutoff's polarization subtraction with a separately prescribed running-coupling subtraction. We use the following exact bookkeeping convention:
\[
 \rho_{\mathrm{aux},2}(V_2)
 =\chi_2(V_2)\,c_{\mathrm{vac},2}
       \exp\{-g_1^{-2}A(U_2(V_2))
                    +{\cal A}_2(U_2(V_2),J_2(V_2))\}.
 \tag{TC.3}
\]
The leading \(g_1^{-2}\) is the one in BA.5a's factor \(C_1\). The complete logarithm of AD's auxiliary integral, its Gaussian normalization, the inherited analytic action, the Haar/coarea and constraint Jacobians, and any previously chosen quadratic subtraction are included in \({\cal A}_2\) or the genuine retained-independent constant \(c_{\mathrm{vac},2}\). Thus a difference between auxiliary and source polarization conventions is retained in \({\cal A}_2\). No equality of beta functions is used.

### Lemma TC.1 — the actual third analytic input

On a fixed buffered native domain, \({\cal A}_2\) has the local analytic coefficient class of CMP109 (1.7)--(1.19), with constants allowed to depend on two fixed levels. Its local coefficients have a strict exponential carrier margin, complex gauge covariance and a simultaneous field/force continuation. They include the determinant.

**Proof.** BA constructs the first action in this class using CMP109 Theorem 3 as completed by CMP116. Its second fluctuation difference is CMP116 Lemma 1, (1.33)--(1.36); the complete classical, gauge and measure remainder is Lemma 2, (1.41)--(1.43). Replace only the fixed free-coordinate product radius in the second analytic comparison by \(p_1\). This radius tends to infinity, while \(g_1p_1\) tends to zero. Every analytic vertex remains in the same fixed physical-angle tube. The fixed-ball failed-cutoff vertices have Gaussian tails at \(p_1\); the normalized marginal bounds and the component identities in CMP116 (2.5)--(2.26) are unchanged. The same cluster proof therefore constructs its logarithm in the native class, with strict margins. This is precisely the analytic comparison retained in AD, not the sharp Q correction.

The localized Gaussian normalization is restored as on CMP116 printed pp.21--22. Adding the inherited value at \(U_2\) and the retained-only local factors produces (TC.3). At two fixed levels the conversion of the earlier carriers to this lattice has fixed incidence and preserves a smaller positive rate. Keeping a bounded projected quadratic term in \({\cal A}_2\) is permitted by the same local analytic class; it is not silently moved into \(g_2\). This proves the claim. \(\square\)

Now perform the third physical averaging, with normalized source gauge insertion, exact average constraint and the literal Q partition. Source CMP119 (3.6)--(3.9) removes \(\chi_2\) on the complete third Q fiber before any R split. Summing that R partition leaves the exact integral
\[
 Z^{QQQ}_3(W)=
 \int dc\,\chi_{Q,2}(c,W)D_2(c;W)
        \exp\{H^{[0]}_2(\Psi_W(c))+H^{[1]}_2(\Psi_W(c))\},
 \qquad W=V_3,
 \tag{TC.4}
\]
\[
 \rho_{QQQ,3}(W)=\chi_3(W)C_2(W)Z^{QQQ}_3(W).
 \tag{TC.5}
\]
Here \(C_2\) is the exact retained-only factor in the same third coordinate change. It includes \(c_{\mathrm{vac},2}\), the value \(\exp[-g_1^{-2}A(U_3)+{\cal A}_2(U_3,J_3)]\), and every retained-only coarea or normalization factor assigned to it. The rest is the complete smooth normal form
\[
 D_2(c;W)=\exp\{-\tfrac12c^{\mathsf T}K_2(W)c+W_2(c;W)\}.
 \tag{TC.6}
\]
Neither inherited \(H^{[i]}_2\) is already present in \(D_2\). Each occurs exactly once in (TC.4). Equations (TC.3)--(TC.6) are identities of the specified physical operation, not a replacement of the logarithm of an expectation by an expected logarithm.

## 2. Actual third precision, gauge and raw coefficient family

Let \(V_*^{(2)}=M^2U_3(W)\) in the source averaged-gauge representative. Criticality and uniqueness identify \(U_2(V_*^{(2)})=U_3(W)\) as regular critical orbits; use VN's tangent-kernel proof, not an inclusion of the entire regular admissible sets. The full constrained Hessian of \(A(U_2(V_2))\) at this field is the source force-corrected form \(\Delta_{2,\mathrm{cl}}\). It includes the constraint multiplier paired with the second derivative of the nonlinear average, and the earlier force corrections in the inherited propagators.

The physical displacement is \(g_2\mathsf C_2c\). Consequently the convention (TC.3) gives
\[
 K_2=\mathsf C_2^*
   \{\lambda_2\Delta_{2,\mathrm{cl}}
                    +c_{\mathrm{gf}}\tau_2^*\tau_2\}\mathsf C_2,
 \qquad \lambda_2=(g_2/g_1)^2 .
 \tag{TC.7}
\]
The map \(\mathsf C_2\) is the linear exceptional-bond solve; \(C_2(W)\) in (TC.5) is the distinct scalar retained prefactor. The sampler \(\tau_2\) is the derivative of the full nonlinear averaged contour variable, not an average of derivatives with dexp factors discarded. At the canonical representative that variable is identity, so its positive outer soft potential has the exact quadratic \(c_{\mathrm{gf}}\|\tau_2\mathsf C_2c\|^2\). AP and BA give the gauge decomposition and source identification.

The first force term cancels on the exact third constraint tangent. Multiplying the classical action by \(\lambda_2\) preserves this cancellation. Since the supplied adjacent coupling ratios are bounded, \(\lambda_2\) lies in a fixed positive compact interval. On the critical constraint tangent the classical form is nonnegative and gauge-null. Hence comparison with the actual source axial gap and the full soft sampler gives
\[
 m_2I\le K_2\le M_2I
 \tag{TC.8}
\]
with fixed-three-level constants. CMP99 printed p.428, (3.156)--(3.158), is the classical/constraint input; CMP109 (2.2)--(2.13) supplies the averaged-gauge, coarea and complete fluctuation expansion. Any analytic projected quadratic left in \({\cal A}_2\) remains in \(W_2\); its twice-normalized fluctuation derivatives are \(O(g_2^2)\) times its native coefficient bound.

CMP116 Lemmas 1--2 apply to \({\cal A}_2\). The classical nonlinear terms have their literal factor \(g_2^3/g_1^2=\lambda_2g_2\); the gauge remainder has its own original \(g_2\). On a fixed small physical tube the complete \(W_2\) therefore has the strict small quadratic and bounded inherited vertex majorants used in BA.15. No bare \(g_2^{-1}\) force is created.

For true raw-\(W\) carriers use the BR/FC homogeneous minimum registry at this fixed depth, followed by the actual two-level readout \(M^2\) and its fixed-\(L\) averaged-gauge conversion. Relative to the face lift \(Q^fW\), the independent background angles obey
\[
 a^{(3)}_e=\sum_{X\ni e}a^{(3)}_{eX}(W_X),\qquad
 \sup_e\sum_Xe^{\nu n(X)}\|a^{(3)}_{eX}\|\le C_L\epsilon_3,
\]
\[
 \sup_e\sum_Xe^{\nu' n(X)}
                   \sum_{d\in X}\|D_da^{(3)}_{eX}\|\le C_Lg_3.
 \tag{TC.9}
\]
This is CA.3--6 with the fixed readout depth increased from two to three. The proof uses the same force-containing contraction, local logarithm and fundamental-theorem coefficients; finite \(L^2\) readout stencils are included before extraction. Every old local analytic coefficient reads at most a fixed-three-level multiple of its carrier volume. Its Taylor substitution by a physical correction of size \(q\) costs \(\exp(C_Lq|X|)\), by the explicit geometric-series proof CA.6. The old analytic carrier gets only its fixed coarse covering and a fixed collar. Choose the output rate below the native rate divided by that fixed covering incidence, leaving strict slack.

These operations include the full \(K_2\), the inherited \({\cal A}_2\) difference, the canceled classical/gauge remainder and the Haar/coarea terms. PR.2 gives supported Gram factors for the actual positive \(K_2\); GM gives their common positive restrictions and normalized marginal family. The same covariance supplies the inverse quadratic and determinant branch.

Let \(Q_3\) denote the literal third Q domain. The source saddle/reference comparison (3.17)--(3.19) gives, on every starred slot,
\[
 B_{2p_2}\subset Q_3^{\mathrm{loc}}
      \subset B_{(2+o(1))P_{Q,2}+O(1)}.
 \tag{TC.10}
\]
All overlapping reference tests are retained. A coefficient cap is chosen equal to the identity through \(3.5P_{Q,2}\), bounded by \(4P_{Q,2}\), and used only in analytic coefficient inputs. The Gaussian quadratic remains uncapped. The identity plateau contains the entire physical Q domain and its bounded-displacement chains. Real unbounded ordinary Gaussian coordinates are capped coefficientwise; no ambient smooth guard is evaluated at complex raw data.

## 3. The inherited state is a two-colour integral registry

The input to the third step is stronger than the integrated norm AD.10. Retain the original QC/TD/AD primitive and logarithmic labels. Each tag \(\tau\) of \(E_2\) has a finite conditional Gaussian tree of depth at most two:

* middle-level Gaussian copies in the second free variables;
* for a transported first defect, first-level copies conditional on that copy's real middle variables;
* actual real Q cores, their annulus/chain currents, analytic connector coefficients and all Gaussian inverse/determinant factors.

Copies created by products or connected logarithms remain distinct even when their physical supports coincide. Let \(r_\tau\) be the sum of their local ranks with multiplicity; let \(n_0(\tau)\) and \(n_1(\tau)\) be their numbers of first and second defect occurrences. A nonzero tag has \(n_0+n_1\ge1\). A transported-first tag can also contain second Q alternatives from its middle gas, and these remain in its registry.

The original positive proofs have strict primitive margins. Retaining those margins yields envelopes \(A_\tau\) for which
\[
 \sup_x\sum_{\tau:\,x\in X_\tau}
 e^{\nu_2n(X_\tau)}A_\tau e^{\eta_*r_\tau}
     e^{-c_*[n_0(\tau)p_0^2+n_1(\tau)p_1^2]}
 \le C_L(e^{-c p_0^2}+e^{-c p_1^2}).
 \tag{TC.11}
\]
One first signed density response has the same bound after decreasing the margins. The following explicit majorant construction recovers this reserve from the exact QC/TD/AD primitive family; it is not inferred from convergence of AD.10.

For every constituent Gaussian node \(v\), with real reference \(\Sigma_v\), real coordinate \(x_v\) and rank \(r_v\), insert in its positive majorant, but not in its physical integrand, the factor
\[
 \exp\{\zeta r_v+\zeta|\Sigma_v^{-1/2}x_v|^2\}.
 \tag{TC.11a}
\]
Also multiply every individual analytic vertex weight by \(e^{\zeta n(X_v)}\). Choose \(\zeta>0\) below a fixed portion of the Gaussian fractions retained in QC.18/CA.20. Integrating a lower node's additional quadratic store against its normalized positive conditional reference costs at most \(e^{C\zeta r_v}\), uniformly in its real ancestor coordinates. It leaves no quadratic store in those ancestors. A node with a defect retains a smaller positive multiple of its original \(p_i^2\) tail; the real annulus and the bounded imaginary/real frame displacements satisfy exactly the same reserved Gaussian estimate. This calculation is made per node, before any product or cluster sum.

For each primitive marginal, \(r_v\le C_{m_v}|I_v|\), with \(m_v\) its fixed ordinary buffer. The extra factor \(e^{C\zeta r_v}\) is therefore a small exponential change of that primitive's activity weight when \(\zeta C_{m_v}\) is below the reserved ordinary spatial rate. Where \(I_v\) also includes a growing inherited core, split its rank into the ordinary contribution and the core contribution: the latter is bounded by its fixed geometric core volume and is paid by a separately allocated fraction of that occurrence's birth tail, exactly as in TD.9--10 and AD.8--9. It is not bounded by the volume of a union after repeated copies have been identified. The output carrier size is at most the sum of its individual vertex/carrier sizes with the already fixed covering constant, so a further \(e^{\zeta n(X_\tau)}\) can be paid by another small portion of the same vertex-wise rate and the allocated core tails.

Replay the actual positive overlap-tree/component and connected-log expansions of TD Section 4 and AD Section 2 with these enlarged primitive weights. Their unmarked ordinary activities have a strict KP margin, and their old coloured input activities have a strict component and final KP margin at TD's fixed inflated fugacity. Hence choosing the one \(\zeta\) smaller if necessary keeps each of those same positive sums finite. Every old occurrence retains its own factorial and its own node rank. This proves a positive reserve neighborhood of the exact retained family and gives (TC.11).

For one current, place a single signed score or shell insertion in the original primitive before this replay. Its inverse/determinant polynomial is bounded by one additional small Gaussian fraction; carrier/rank incidences use a further vertex-wise rate loss; the actual Q perimeter and cutoff powers use a further fraction of a present birth tail. Uniformity on the real lifted-path tube comes from the coefficient and shell certificates, not from differentiating an already integrated Lipschitz tag. The differentiated-position sum is the first derivative of the same convergent positive generating series. Thus the primitive first-jet family also has (TC.11) with smaller positive margins. This construction is the reserve argument of TD.8 applied before the two-level integrals and logarithms are aggregated.

The third construction below can use an equivalent finer labeling of these exact coefficients. No value identity or physical integral is modified.

## 4. Third core frame and nested real admission

Keep the full nonanalytic \(V_2\) input core of each old tag. For a first-born defect this includes its whole second-step core frame, all whole-Q tests on that frame, and their defining boxes. For a second-born defect it includes its actual second Q-reference boxes. Analytic connector supports are kept separate.

Close these cores under the exact independent-coordinate/exceptional/gauge stencil of the third reconstruction. Call the union \(S_2\). Include every third Q-reference box touching \(S_2\) and add an \(R_3\) collar. Merge only components whose full stencils overlap; use unions of cubes, never bounding rectangles. For a collection of tags with total counts \(n_0,n_1\), the third core \(D_2\) obeys
\[
 |D_2|+|S_2|
 \le C_L\{n_0(R_1/L^2+R_2/L+R_3+m)^4
              +n_1(R_2/L+R_3+m)^4\}.
 \tag{TC.12}
\]
The ordinary marginal buffers \(m\) are fixed constants. The physical readout and domain admission are the nested zero-completion construction verified separately by the support analysis.

Restrict the single registry (TC.9) to \(D_2\), and reconstruct its exceptionals with the fixed target \(W\). This produces a compact constrained local frame \(V_D\); it is not claimed to be a new minimum. For any analytic connector \(I\) use the additive initial region \(D_2\cup D_m(I)\), while the core frame remains the one from \(D_2\). On \(S_2\) make
\[
 c_{s,e}(B_e)=\frac1{ig_2}
       \Log(e^{ig_2B_e}V_{D,e}V_{s,e}^{-1}).
 \tag{TC.13}
\]
The common carrier tail and fixed exceptional solve give
\[
 |c_s-B|_{S_2}\le
       C_L(\epsilon_3/g_2)e^{-cR_3}=o(1),
 \quad
 \|D_{B_{S_2}}c_{s,S_2}-I\|\le C_L\epsilon_3e^{-cR_3}.
 \tag{TC.14}
\]
All required physical \(V_2\) links are consequently fixed, real and independent of the third outside parameters. Their exact coarse constraints hold also for the complex family because the target is imposed by the solve.

Keep third Q whole on \(S_2\). For a real point in these domains, retain its independent entries and put all other third free entries equal to zero. Zero entries are strictly Q-good by the sharp saddle/reference comparison. The resulting global Q3 field is old-\(\chi_2\)-admitted by source (3.6)--(3.9), and has exactly the same \(V_2\) core. This proves real admission of every middle local Q problem.

For each first-born core, keep only that copy's middle whole-Q entries on its full original stencil, and zero-complete the other middle independent entries. Those outside zeros are Q2-good. Its \(V_1\) core is unchanged, so the same source redundancy proves the first local admission. Any auxiliary middle defect chain outside that stencil is omitted from this real completion; a complex chain coordinate is not declared a real physical field. The full-stencil independence is why omitting it changes no old core. Second-born local references already have the admitted real \(V_2\) data and need no such middle completion.

Thus all old real domains can be kept real under every outside parameter. The remaining analytic inputs use the fixed caps. Their physical perturbation size at the third substitution is
\[
 q_3=C_L(\epsilon_3+g_2P_{Q,2})\longrightarrow0.
 \tag{TC.15}
\]
At fixed three levels, the reconstructed old native first/second regularity and force norms change by at most \(C_Lq_3\), using their buffered analytic maps and the actual fixed-depth readouts. The source conditions CMP109 (1.11)--(1.18), including its nested-minimum condition, therefore remain in their interior tube. This is analytic coefficient admission; it does not assign a value to a hard selector at a complex field.

## 5. Joint Gaussian certificate, with no third tilt per old copy

Choose fixed ordinary buffers in the order: first-level marginal buffer, middle buffer containing its fixed coarse cover, then third buffer containing both covers. Each can be increased to make its omitted-covariance connector tail \(u_{m_i}\) as small as required. After fixing these buffers and all rate margins, choose the coupling small. All are fixed-three-level choices.

At a fixed real capped third array \(B\), each middle node has a centered positive Gram-reference marginal \(\Sigma_{1,B}\). Conditional on its own real capped middle array \(b\), each first node has a centered positive Gram-reference marginal \(\Sigma_{0,b,B}\). References and continuations are restrictions of the same pulled-back coefficient registries. Every covariance generates its own inverse and determinant together.

The first and middle Gram coefficients have a physical-angle derivative row bound on their fixed native tube; this is CA.17 for level zero and the identical PR/GM inverse/Gram differentiation applied to the inherited middle precision. The complete inherited matrix, including its force and full sampler, is used. The Taylor/carrier substitution CA.6 consequently costs
\[
 e^{C_Lq_3|X|}
 \tag{TC.16}
\]
for an old analytic coefficient on \(X\). It does not cost a fixed \(C^{|X|}\) and does not attach an \(R_3\) halo to \(X\).

The resolvent identity in this common row/column norm gives the following concrete relative covariance comparisons:
\[
 \|\Sigma_{1,B}^{-1/2}
       (\Sigma_{1;s;B}-\Sigma_{1,B})\Sigma_{1,B}^{-1/2}\|
       \le C_L(u_{m_1}+q_3),
 \tag{TC.17}
\]
\[
 \|\Sigma_{0,b,B}^{-1/2}
       (\Sigma_{0;s;b,B}-\Sigma_{0,b,B})
                    \Sigma_{0,b,B}^{-1/2}\|
       \le C_L(u_{m_0}+q_2+q_3).
 \tag{TC.18}
\]
Here \(q_2\) is the previous small capped middle physical variation, enlarged by a fixed constant to include its bounded defect contours; it is \(O_L(\epsilon_3+g_2P_{Q,2}+g_1P_{Q,1})\) on this family and tends to zero. An order-one old covariance connector changed by a higher outside parameter must leave that node's fixed marginal buffer and belongs to \(u_{m_i}\). It is not mislabeled as a small local background perturbation.

The proof of (TC.17)--(TC.18) is at the coefficient level: a physical input change \(q_3\) changes each Gram row by its summed Cauchy derivative times \(q_3\); Gram multiplication and the resolvent preserve this bound; compression preserves the relative operator estimate by the uniform gaps. GM controls the omitted full-carrier tails. This works simultaneously on the fixed polydiscs and uniformly in the real capped ancestor variables. It does not assume that an independently decoupled minimum is stationary for the undeformed action. All action terms remain in their original critical-canceled native continuation.

The smooth three-innovation baseline may use four independently continued copies of one normalized terminal path: one in the microscopic reconstruction and one in each normalized kernel. Their physical raw displacements on fixed one-coordinate discs are \(O(g_3)\). The same local analytic substitution, fixed-depth readout bounds and resolvent argument add at most \(C_Lg_3\) to (TC.17)--(TC.18), and the corresponding third comparison. Compare all copies to the same positive real center, use one covariance/inverse/determinant triple for each conditional occurrence, and keep each occurrence's own already-canceled normal form. The fixed product \(p_0,p_1,p_2\) domains are unchanged. Thus these independent smooth source/current copies have the same strict Gaussian stores on a smaller fixed tube. This statement concerns that fixed-domain baseline; it does not claim holomorphy of the actual sharp Q laws in independent retained copies.

For each node the same elementary Gaussian calculation as CA.20 now yields
\[
 |p_{\Sigma_s}(x+iy)|
 \le e^{C\delta r+C_a n}\,
          p_{\Sigma_{\rm ref}}(x)e^{C\delta|x|^2},
 \tag{TC.19}
\]
where \(y\) is supported only on that node's defect contours. A further arbitrarily small Young tilt accounts for its bounded real frame shift. Complete non-Gaussian vertices retain the strict native quadratic reserve. Ordinary coordinates are integrated exactly against the normalized positive reference, and only actual defect marginals contribute fixed constants per defect.

The relevant old global/local comparisons also persist. Their defining core data have been fixed by (TC.13). In the common interior constrained and averaged-gauge chart, the complex mean-value operator is a small perturbation of the positive real one. Its weighted inverse gives \(C\gamma e^{-cR_i}\) influence of boundary discrepancies, plus the actual omitted-carrier tail. After division by the appropriate \(g_i\), these displacements are bounded and tend to zero for the full \(R_i\) buffer; the fixed-depth coupling and cutoff ratios preserve the smaller old defect-only halo bounds as well. Hence the old annuli and side chains retain radius \(c p_i\). No stationarity claim is made for an outside-decoupled field.

Integrate first every first-level copy conditionally on its real middle and third ancestors. Its bound retains its first tail and is uniform in those ancestors. Then integrate each middle copy, retaining its own middle tail when present. One obtains, for any product of old tags \(\tau_1,\ldots,\tau_m\), at fixed real third \(B\),
\[
 \left|\prod_{\ell=1}^m{\cal H}_{\tau_\ell}(B;s)\right|
 \le C^m\prod_{\ell=1}^m A_{\tau_\ell}\,
       e^{\eta\sum_\ell r_{\tau_\ell}}\,
       e^{-c\sum_\ell[
           n_0(\tau_\ell)p_0^2+n_1(\tau_\ell)p_1^2]}.
 \tag{TC.20}
\]
The notation means the exact product-integral representation with distinct latent copies. In particular (TC.20) has **no factor \(e^{cm|B|^2}\)**. Every lower conditional reference is normalized at its actual real ancestors; its rank cost belongs to that copy. The ordinary coefficient cap does not truncate the third Gaussian.

Only after (TC.20) is established is the one third Gaussian integrated. Its single frame displacement is supported on the union \(S_2\), with per-coordinate bound (TC.14) independent of the number of payload copies. Its density and Jacobian cost at most
\[
 e^{\eta r_2+C_a|S_2|}
     p_{2,\mathrm{ref}}(B)e^{\zeta |B|^2}
 \tag{TC.21}
\]
with the complete third interaction reserve and small fixed \(\zeta\). Drop the whole Q factors on \(S_2\) for this upper bound. This integrates once, giving the joint primitive estimate
\[
 C^m A_I\prod_\ell A_{\tau_\ell}\,
 e^{\eta(r_2+\sum_\ell r_{\tau_\ell})+C_a|S_2|}
 e^{-c\sum_\ell[n_0(\tau_\ell)p_0^2+n_1(\tau_\ell)p_1^2]} .
 \tag{TC.22}
\]
Rank multiplicities are retained. Source hierarchy gives \(p_i^2/R_{i+1}^4\to\infty\), with comparable adjacent radii over these three fixed levels. Thus (TC.12), the reanchoring polynomial and core current factors use one allocated portion of the appropriate birth tails. Ordinary analytic connector losses use only their strict spatial rate.

Additional third Q contours occur only outside \(S_2\). They do not change old real domain inputs. Their bounded normalized displacement changes old analytic arguments by \(O(g_2)\), already covered in (TC.17)--(TC.18). Their new tails are charged to the new third defect species, not to a second use of the old birth tails.

## 6. Components, the same denominator, and both old masses

All restrictions use one raw background/Gram/vertex registry. The core rule is additive before merging; every constraint stencil lies inside its assigned halo; analytic connectors do not change the chosen core frame. At each lower node use the same canonical local frame and normalized covariance registry as in the original primitive representation, now evaluated on the identical restricted higher input.

Consequently a separated component has exactly the construction obtained by keeping that component alone. A component disjoint from all old full core-plus-connector carriers has the unmarked third Q family: the same scalar prefactor convention, Gaussian inverse/determinant, \(W_2\), raw Q references and domains. Every frame is the identity there. This proves the root-deletion identity for the third construction, not merely small interaction between separated components. It permits CN's excluded-vacuum identity with the actual third denominator.

Introduce two old source colours:
\[
 {\cal Z}_3(\lambda_0,\lambda_1)=
 \int dc\,\chi_{Q,2}D_2\,
   e^{\lambda_0H^{[0]}_2(\Psi_W(c))
                   +\lambda_1H^{[1]}_2(\Psi_W(c))}.
 \tag{TC.23}
\]
Expand both exponentials with their exact factorials and distinct latent copies. Products share the one physical third variable \(c\). The common component gas has base activities \(z_\gamma\) and additional connected activities \(u_\gamma(\lambda_0,\lambda_1)\), each of the latter containing at least one old colour:
\[
 {\cal Z}_3(\lambda_0,\lambda_1)/{\cal C}(W)
   = Z\bigl(z+u(\lambda_0,\lambda_1)\bigr).
 \tag{TC.24}
\]
The common factor \({\cal C}\) is removed identically in every ratio. At \((1,1)\) this is (TC.4), and at \((0,0)\) it is the third Q integral of the analytic base. A conditional expectation under the full law uses \(Z(z+u(1,1))\), not \(Z(z)\).

After the paid core enlargements and fixed carrier conversions, (TC.11)--(TC.22) give a total old input budget
\[
 \varepsilon_{\mathrm{old}}
    \le C_L(e^{-c p_0^2}+e^{-c p_1^2}).
 \tag{TC.25}
\]
For completeness, this bound is summable through the whole exponential, not just its first term. Multiply both old colours by a positive counting variable \(s\). The positive component majorant converges when the old budget is \(s\varepsilon_{\mathrm{old}}\) in a fixed neighborhood of zero, by the same rooted overlap-tree proof as TD Section 4, with the per-copy estimate (TC.20) and a single third store (TC.21). Choose \(a_*>0\) inside both that component radius and the final decorated KP margin, and use \(s_*=a_*/\varepsilon_{\mathrm{old}}\). At \(s=s_*\) the full positive majorant and connected logarithm are bounded. Every old-containing coefficient has positive degree in \(s\), so its sum at \(s=1\) gains \(s_*^{-1}\). This proves
\[
 \left\|\log\frac{{\cal Z}_3(1,1)}
                         {{\cal Z}_3(0,0)}\right\|_{\kappa,\mathrm{anc},1}
       \le C_L(e^{-c p_0^2}+e^{-c p_1^2}).
 \tag{TC.26}
\]
For the value part this is the connected logarithm of one full gas. It is not an average of \(E_2\). The first-current statement uses the signed primitive stores described next. Its finite path version uses common envelopes over the same buffered native paths.

The pure third Q/auxiliary correction has the same generalized QC construction as AD with the actual \(K_2,W_2\), and satisfies
\[
 \left\|\log\frac{{\cal Z}_3(0,0)}
      {\displaystyle\int dc\,\chi_{p_2}(c)D_2(c;W)}
                           \right\|_{\kappa,\mathrm{anc},1}
       \le C_L e^{-c p_2^2}.
 \tag{TC.27}
\]
Its cap is based on the whole \(P_{Q,2}\) fiber as in (TC.10). Therefore, with
\[
 \rho_{\mathrm{aux},3}
 =\chi_3C_2\int\chi_{p_2}D_2,\qquad
 \rho_{QQQ,3}=\rho_{\mathrm{aux},3}e^{E_3},
\]
\[
 \boxed{\quad
 \|E_3\|_{\kappa,\mathrm{anc},1}
   \le C_L(e^{-c p_0^2}+e^{-c p_1^2}+e^{-c p_2^2}).
 \quad}
 \tag{TC.28}
\]
This is a fixed-third-level native unmarked density conclusion. Its three defect births remain distinguished in the integral registry.

## 7. First jets, physical origins and the marked boundary of this result

The exact third conditional is
\[
 q_2(dc\mid W)=
 \frac{\chi_{Q,2}D_2(c;W)e^{E_2(\Psi_W(c))}\,dc}
                         {{\cal Z}_3(1,1;W)}.
 \tag{TC.29}
\]
All inherited masses in this density and its normalizer are occurrences of the new kernel. Equal-valued masses occurring in an old normalized conditional retain their old labels. Form the value and first jets of the complete nested physical integral before any cancellation, using the exact product and inverse rules as in DP.22a--c.

Here is the uncanceled source identity that fixes those occurrences. Write \(n_{0,Q}\) for the complete first Q density in its free chart, \(m_0=Z_{0,Q}/Z_{0,P}\), \(n_{1,PQ}=\chi_{Q,1}D_1\), and
\[
 Z_{1,QQ}(V_2)=\int n_{1,PQ}(a,V_2)m_0(V_1)\,da,\qquad
 Z_{1,A}(V_2)=\int\chi_{p_1}(a)D_1(a;V_2)\,da .
\]
AD gives \(m_2=Z_{1,QQ}/Z_{1,A}=e^{E_2}\). The common retained factor in these two masses cancels literally. With \(n_{2,AQ}=\chi_{Q,2}D_2\), the exact third conditional source mean is
\[
 \frac{1}{Z_3}\int dc\,n_{2,AQ}(c,W)m_2(V_2)
  \frac{1}{Z_{1,QQ}(V_2)}
    \int da\,n_{1,PQ}(a,V_2)m_0(V_1)
       \frac{1}{Z_{0,Q}(V_1)}
            \int dz\,n_{0,Q}(z,V_1)e^{tF(\Phi_{V_1}(z))},
 \tag{TC.29a}
\]
where \(V_2=\Psi_W(c)\), \(V_1=\Psi_{V_2}(a)\), and \(Z_3={\cal Z}_3(1,1)\). All source normalized gauge-preimage variables may be retained in these measures; they cancel on a constant insertion and do not alter a gauge-invariant microscopic scalar.

Assign the source factor to M, \(n_{0,Q}\) and its displayed inverse normalizer to 0, the entire middle density including \(m_0\) and its inverse normalizer to 1, and the entire outer density including \(m_2\) and \(Z_3^{-1}\) to 2. In particular \(Z_{1,QQ}\) inside \(m_2\) and the displayed \(Z_{1,QQ}^{-1}\) have equal values but different first-jet ownership. Apply the common maps, coefficient substitutions and covariance/determinant continuation to these occurrences before any cancellation. Each occurrence's inverse uses its own exact inverse-jet rule. The component expansion is an expansion of this integral family, not a pairing of independently continued current coefficients with a previously chosen value family. Thus at every admitted outside parameter,
\[
 q_{j,s}(1)=1,\qquad \dot q_{j,s}^{\,j}(1)=0
       \quad(j=0,1,2).
 \tag{TC.29b}
\]
These identities retain the actual normalizers; no separate core normalization has been introduced.

The full three-level change of variables is triangular:
\[
 (z_0,z_1,z_2)
   =(T_0(u_0,u_1,u_2),T_1(u_1,u_2),T_2(u_2)).
 \tag{TC.30}
\]
For a physical path set \(v=(DT)^{-1}\partial_\theta T\). Its upper components are independent of lower variables. For the conditional density at level \(j\), with its own diagonal Jacobian \(J_j\), the exact transported derivative is
\[
 J_j(\partial_\theta q_j|_{\rm original\ coordinates})\circ T
   =\left(\partial_\theta-\sum_{\ell\ge j}v_\ell\partial_{u_\ell}
                         -\operatorname{div}_{u_j}v_j\right)
                                     \widetilde q_j .
 \tag{TC.31}
\]
Only its own fiber divergence occurs. Together with the insertion derivative these identities sum to the full density derivative minus the full divergence. Each normalized conditional's own first jet annihilates 1 at every admitted outside parameter, since its numerator and denominator use the identical occurrence-level registry. This proves P2's normalized algebra for the actual third family.

For the unmarked stores used in (TC.26)--(TC.28), differentiating one primitive adds a fixed polynomial in its full rank, carrier incidence, core volume and cutoffs, together with the actual normalized factors \(g_3/g_2\), \(g_3/g_1\) or \(g_3/g_0\). Those ratios are bounded at this fixed depth. The response includes every inverse/determinant term, every inherited action/coarea term, and the shell currents from all three real Q-domain generations. The full lifted-path shape rule follows by applying DP's finite-perimeter and joint-tie argument to the actual triangular independent variables; independent levels have transverse old-coordinate normals. No generic Lipschitz partial derivative is evaluated on a diagonal. Persistent coincident sheets use their one common physical velocity.

Integrate the lower signed primitive stores in the same order as (TC.20). Uniformity in the real ancestors preserves each birth tail when a higher Q shell is inserted. The small covariance/interaction stores and one fixed fraction of the birth tail pay all resulting polynomials. All currents remain rooted before absolute connected summation. This proves the once-differentiated majorant needed in the unmarked density norm. The support analysis supplies the explicit lifted-domain admission and tie scope; no complex indicator is evaluated.

For a microscopic mark, (TC.31) supplies the correct normalized ownership and the common first-jet family, but it does not itself prove PC.10's energy--velocity estimates. Those require a three-innovation physical root with fixed Gaussian stores chosen before integration. In particular the lower unmarked copied trees have the uniform bound (TC.20), whereas a single distinguished marked tree may require an additional third quadratic reserve. The latter is allocated once, not once per copied old vacuum. The three-innovation marked calculation is separate from this note.

## 8. Exact scope and why this is not an all-depth induction

The construction uses the actual third analytic input, force-corrected inherited precision, full averaged soft gauge, literal Q radii, fixed-target exceptional solves, real old-domain admission, common normalized covariance and exact same-gas denominator. Both inherited masses are present once. It closes the unmarked third density transfer and the common normalized first-jet kernel construction on the specified homogeneous native domain.

It does not settle complementary P/Q histories, residual components, an ambient third-step extension, the canonical rectangular-current interface, an outer law or Yang--Mills existence. The marked energy--velocity transfer still requires its actual root calculation.

Three sources of depth dependence are explicit: repeated fixed carrier-cover/rate losses; the accumulated nested marginal/reference and core-frame reserve allocations; and repeated scalar/identity or relevant/vacuum extraction. At fixed depth three the buffers and positive spare margins can be chosen once. No assertion here makes their products, normalization costs or engineering factors summable through arbitrary depth. AP/SG's real primitive Gaussian estimates do not by themselves supply that common complex interacting induction.

Primary source inputs: CMP99 printed pp.421--428, especially (3.127)--(3.138), (3.156)--(3.158); CMP102 (111)--(121) and Proposition 9; CMP109 printed pp.261--269, (1.7)--(1.19), (2.2)--(2.13); CMP116 Lemmas 1--2, (1.33)--(1.43), normalized marginal bounds (2.5)--(2.26) and the final restoration of log Gaussian normalization; CMP119 printed pp.264--268, (3.6)--(3.19). Companion inputs are the specified BR/FC, PR/GM, BA/CA, QC/QS, CN/TD/AD, DP and VN proofs, with the stated fixed-third-level applications proved above.
