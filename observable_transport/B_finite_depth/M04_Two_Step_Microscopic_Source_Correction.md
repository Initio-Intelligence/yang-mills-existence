# Two-step microscopic source correction on the native averaged route

## 1. Scope and exact microscopic sources

This note extends the two-step density theorem TD to a specified microscopic source family. It proves a rare correction estimate for the composite physical conditional law. It does not identify that estimate with the canonical second-step M04 transport of previously filed direct/kernel records, and it does not prove the absolute energy-graded second-step marked theorem.

Use exactly the two homogeneous P/Q-regular levels and the new physical averaging operation of BA, CA and TD, with both R partitions summed. Put

\[
h_1=Lh_0,\qquad h_2=L^2h_0,\qquad P_0=\delta_0/g_0,
\qquad P_Q=\delta_1/g_1.
\tag{MS.1}
\]

The adjacent coupling ratios and P_Q/P_0 are bounded in this fixed two-level operation. All couplings, maps and cutoffs are specified at zero physical source. Constants below may depend on the fixed group, L and the two fixed levels, but not on volume, source order or sufficiently small coupling.

Let the actual microscopic marks be

\[
F_j(U)=\alpha_j\beta_0\sigma_{h_0}(x_j;U)-c_j,
\qquad b_j=|\alpha_j|+h_0^4|c_j|,
\qquad \beta_0g_0^2=1/N.
\tag{MS.2}
\]

These are the original gauge-invariant Wilson scalars with their original microscopic stencil and centering, not new native plaquette sources at scale h1 or h2. Gauge-preimage variables can be retained as in RA.4a; their normalized Haar factors have no effect on these marks or their products.

For the exact first integrals define

\[
G_{P,1}(\mathbf t;V_1)=Z_{P,0}(\mathbf t;V_1)/Z_{P,0}(0;V_1),
\qquad
S_1(\mathbf t;V_1)=\log G_{P,1}(\mathbf t;V_1),
\]
\[
H_1(\mathbf t;V_1)=\log Z_{Q,0}(\mathbf t;V_1)
                         -\log Z_{P,0}(\mathbf t;V_1).
\tag{MS.3}
\]

The same complete first density and reconstruction are used in both integrals. Write \(\nu_W=\nu^P_{Q,1}(\cdot\mid W)\) for TD's normalized second Q operation on the analytic first-P base. Its reconstructed old current field is V1 = Psi_W(a). Then the exact second conditional source functions are

\[
G_{PQ,2}(\mathbf t;W)
   =\nu_W\exp S_1(\mathbf t;V_1),
\]
\[
G_{QQ,2}(\mathbf t;W)
   =\frac{\nu_W\exp\{S_1(\mathbf t;V_1)+H_1(\mathbf t;V_1)\}}
                {\nu_W\exp H_1(0;V_1)}.
\tag{MS.4}
\]

The first formula is the same next actual Q integration with the first P comparison law; the second uses the first actual R-averaged Q law. These are composite physical conditional expectations of exp(sum t_j F_j(U)). The first density is included exactly once. Every second coarea, gauge, inherited action and normalizer is the one in TD.1–3.

In particular the first background value is retained:

\[
S_1(\mathbf t;V_1)
=\sum_j t_jF_j(\Phi_{V_1}(0))
 +\log q_{P,0,V_1}\exp\!\sum_j t_j
       [F_j(\Phi_{V_1}(z_0))-F_j(\Phi_{V_1}(0))].
\tag{MS.5}
\]

The first term depends on V1 and remains inside the second integral. It cancels from H1 at fixed V1, but cannot be removed from (MS.4).

Define

\[
\mathcal C_2(\mathbf t;W)
=\log G_{QQ,2}(\mathbf t;W)-\log G_{PQ,2}(\mathbf t;W).
\tag{MS.6}
\]

Equivalently it is the source-containing part of

\[
\Delta_2(\mathbf t;W)
=\log\nu_W e^{S_1(\mathbf t)+H_1(\mathbf t)}
 -\log\nu_W e^{S_1(\mathbf t)},
\quad
\mathcal C_2=\Delta_2(\mathbf t)-\Delta_2(0).
\tag{MS.7}
\]

At zero source this is TD's density correction. The subtraction in (MS.7) removes its possibly extensive vacuum part. All logarithms below use their common convergent cluster branches at zero.

## 2. A joint primitive bound for the full first scalar

Set

\[
M_j=b_jh_0^{-4}P_0^2.
\tag{MS.8}
\]

A zero b_j gives a zero source. Pure constant marks factor from both conditional source functions, so every positive-order correction involving such a label vanishes.

### Lemma MS.1 — full-root joint coefficient budget

Use CA's real capped next field and its common outside-parameter continuation, with the cap identity on the actual next Q support and on every declared moved-coordinate contour. Continue the old reconstruction in the same native canceled coefficient registry used by CA; no ambient smooth retained-field guard is complexified. The **full** microscopic root, including its zero-old-fluctuation value, has a connected joint expansion

\[
F_j(\Phi_{V_1^{cap}(B,s_1)}(z_0;s_0))
                 =\sum_X f^{(2)}_{j,X}(z_0,B,W;s_0,s_1)
\tag{MS.9}
\]

whose carriers contain the microscopic stencil projected to the current lattice and every actual raw-W and coordinate dependency. After one fixed carrier-rate reduction,

\[
\sum_{X\supset x_j}e^{\nu n(X)}
 \left(\sup|f^{(2)}_{j,X}|
       +\sup\sum_d|D_d^{(2)}f^{(2)}_{j,X}|\right)
\le C_L M_j.
\tag{MS.10}
\]

The suprema include the joint fixed outside polydisc, the fixed enlarged old coordinate chart, real capped next variables, and the bounded complex coordinate displacements used by CA/QC. The derivative is the normalized raw W direction, of physical size O(g2), with couplings fixed. Buffered finite paths satisfy the same estimate. Only fixed collars are attached to an ordinary root carrier; Q-reference halos are still charged to the corresponding Q defects.

**Proof.** The relevant small parameter is not a generic geometric Cauchy bound on beta0 times the Wilson trace. CA.15–16 and CA.21 give on the joint family

\[
q_{new}=C_L(\epsilon_2+g_1P_Q),\qquad
q_{new}/g_0\le C_LP_0,\qquad
g_0|z_{0,i}|\le C g_0P_0.
\tag{MS.11}
\]

Use the native force-resolved background and zero-subtracted reconstruction registry MQ.34–36, before integration. Each old background relative-log tree has a force leaf J(Qf V1); each old fluctuation tree has a leaf g0 z0. The face-lift plaquette defect is a local conjugate of a V1 plaquette defect. For the capped joint field its size is O(q_new), by CA.15, including the admitted complex continuation. The local Wilson force is O(q_new) on the same chart. The fixed-point contraction and its distinguished-leaf majorant are uniform on this tube. Consequently every fine plaquette defect is represented by supported sums with at least one of these curvature/force/fluctuation leaves, of respective sizes q_new or g0 |z0|. The coefficients have the same strictly summable carrier majorant as the underlying reconstruction.

This is also a direct way to retain the zero-fluctuation contribution: setting z0 = 0 removes fluctuation leaves but does not remove the force and face-lift curvature leaves. Flat local data, including a flat nontrivial holonomy represented in local gauges, give zero local plaquette defect; an absolute connection potential is not substituted for a curvature leaf.

On complex links use the holomorphic Wilson polynomial, not ReTr as a holomorphic function. For any plaquette matrix P in the admitted chart,

\[
\mathsf s(P)=N-\tfrac12\operatorname{Tr}(P+P^{-1})
 =-\tfrac12\operatorname{Tr}[(P-I)^2P^{-1}].
\tag{MS.12}
\]

Its inverse is uniformly bounded there. Thus each root has two curvature leaves. Their supported convolution remains connected through the plaquette stencil and gives the absolute majorant

\[
C|\alpha_j|h_0^{-4}a_{j,X}
 [\beta_0q_{new}^{2}(1+|X|)+\beta_0g_0^2|z_{0,X}|^2]
 +|c_j|\,\mathbf1_{X=X_j},
\tag{MS.13}
\]

with a strictly summable coefficient sequence after a fixed rate loss. Coefficient multiplicities and fixed source-block-to-raw covers cost only the already admitted fixed conversion and a polynomial in |X|. The joint support is obtained from the same local force/reconstruction maps composed with CA's raw registry; it is not assigned to an already integrated function. Local transport factors and the small analytic substitutions cost exp(C q_new |X|), as in CA.6, and use a strict part of that rate. No growing collar is needed for these ordinary vertices.

Equations (MS.11) and beta0 g0^2 = 1/N bound (MS.13) by C M_j (1+|X|)^C a_{j,X} on the fixed enlarged old chart. In particular its z0 = 0 part is still of order M_j. This proves the value bound.

For a normalized W variation, differentiate one leaf or one analytic map in the same convergent registry. CA.5 and the fixed-depth local solve give a physical input derivative O(g2); differentiating the force/reconstruction equation uses its bounded contraction inverse. A differentiated plaquette defect is therefore O(g2), with its full supported derivative envelope and polynomial incidence count. Differentiating (MS.12) costs at most

\[
C\beta_0 g_2(q_{new}+g_0|z_{0,X}|)
 +C\beta_0 g_2(q_{new}+g_0|z_{0,X}|)^2,
\tag{MS.14}
\]

up to that same support polynomial. The bounded ratio g2/g0, (MS.11), and P0 >= 1 put this within C M_j. Derivatives of transport coefficients retain a curvature leaf and are included in the second term. The real B and old-coordinate caps do not depend on W; they contribute no hidden raw derivative. A cap is the identity on any coordinate which is continued along a contour. Integrating the derivative majorants along buffered native paths proves the finite form. This proves (MS.10).

The gain in (MS.13) is essential. Applying a generic fixed-geometric-tube Cauchy estimate to a pre-existing root bound O(g0^-2) and then invoking the real native inequality E <= C P0^2 would not establish this joint result. Here the two curvature leaves are kept before composition and localization. ∎

## 3. Sources in the same two-layer primitive family

For each fixed vector of nonnegative polyradii r satisfying

\[
\sum_j r_jM_j\le\eta,
\tag{MS.15}
\]

choose eta below a fixed fraction of the strict two-layer component and decorated KP margins. The value and current Mayer envelopes of the actual root species exp(t_j f_j,X^(2)) - 1 have total rooted norm at most C sum r_j M_j. As in FJ, a coordinatewise old cutoff is one through 7P0/2 and zero from 4P0. It changes neither physical first integral and is the identity on every old moved defect coordinate. Unmoved variables stay real. This makes the source envelope bounded also in the untruncated comparison integration, without changing any Gaussian quadratic or actual normalizer.

The fixed-polydisc quantifier is material. One monotone envelope r_j is used for every species with label j. Taking a separate supremum over the entire weighted source ball for every tag would introduce an uncontrolled number-of-labels factor.

The complete first P source logarithm S1 has source-containing connected payloads of total rooted envelope O(sum r_j M_j), in the same latent Gaussian representation as CA. Its domains are fixed old P balls (or their exact failed-cutoff expansion). It has no moving old Q core and needs no growing core halo. Its background term from (MS.5) is among these source vertices. The Gaussian comparison CA.19–20, ordinary exact integration and the strictly reserved first cluster bounds give their uniform-in-B primitive certificate. For a source-only payload its small old-rank loss is paid by strict ordinary carrier decay and any actual failed-P tails, not by a nonexistent old-Q reserve. The first global P normalizer is canceled through the source-containing connected logarithm before this bound is taken. Sources are bounded small Mayer factors; no residual B-quadratic tilt per source payload is introduced.

More explicitly, for each constituent primitive Gaussian marginal with initial ordinary support I_i, a fixed old marginal buffer gives r_i <= C_m |I_i|, with C_m polynomial in that fixed buffer size. Choose the buffer first so that its exponentially small omitted-covariance tail times C_m fits a strict part of the ordinary carrier rate. Then choose the remaining Gaussian tilts and the coupling ceiling so that their rank-loss coefficient times C_m, including q_new C_m, fits another strict part of that rate. Charge exp(eta r_i) to this primitive activity before the first logarithmic cluster sum, and use the resulting strictly enlarged ordinary activity margin in that sum. Repeated overlapping primitive components retain their separate latent copies and their separate charges. No bound of sum r_i by the volume of the union of their supports is asserted. This payment needs no old-Q tail and is independent of the number of payloads or their source multiplicity.

The source-dependent H1 has the same old-Q integral payloads as TD, now with these bounded source vertices. Its unmarked part has anchored envelope O(exp(-cP0^2)). Its source-containing part has total rooted envelope

\[
C e^{-cP_0^2}\sum_j r_jM_j.
\tag{MS.16}
\]

Both bounds retain each old domain, Gaussian certificate and first-current decoration. They follow by the same first connected expansion with the source species added before integration, and the joint root bound MS.1; they are not an application of an already integrated FJ output estimate to a complex V1 field.

Arbitrary products of these old payloads use separate latent old integration copies, conditional on the same real B. CA.22's comparison is uniform in B. The next Gaussian is integrated once, and the common constrained frame costs exp(C|S|) for the union of old Q stencils, independently of multiplicity. Only occurrences with a Q defect contribute to S and its growing halo. Smooth source connectors retain their fixed collars.

There is therefore a common colored component gas for each integral in (MS.7): ordinary next analytic/Q vertices, smooth first-source vertices, and old-Q vertices with or without sources. The numerator contains all old-Q vertices; the denominator in that difference omits them but keeps exactly the same smooth source vertices. Every separated component uses the same covariance, determinant, coefficient and cutoff registry. The full old exponential is included before any normalization or logarithm.

Choose the total source budget eta within the base strict margin. Then apply TD's positive old-fugacity enlargement to the remaining old-Q budget, choosing its constant small enough for both the component and final decorated KP inequalities uniformly on this fixed source polydisc. The source-containing logarithmic difference has one source color and one old-Q color. The double-rooted cluster majorant gives

\[
\sum_a e^{\kappa n(Y_a)}
 \left[\sup_{|t_j|\le r_j}\sup|\mathcal C_{2,a}|
 +\sup_{|t_j|\le r_j}\sup_W\sum_d\sup_{0<|u|\le1}
       |\delta^{norm}_{d,u}\mathcal C_{2,a}|\right]
\le C e^{-cP_0^2}\sum_j r_jM_j.
\tag{MS.17}
\]

Every tag contains a source and an old Q defect, with a genuinely connected full raw-W carrier. The constant is independent of the number and positions of sources and total volume. Normal convergence holds on a spare neighborhood after eta is reduced once. Source-free clusters cancel before the total rooted bound is taken; their extensive vacuum sum is never bounded by (MS.17).

The first-current proof retains all terms from CA.25. Old-domain shells keep an old tail. Whole next-Q shells on S retain that tail through the uniform old certificate. A source current is bounded by (MS.10); changing any other factor leaves a source vertex and an old defect in its cluster. Centered density scores, determinant and inverse responses, complete coarea terms, and exact coordinate Jacobians are included. Positive decorated majorants handle vanishing species without dividing by their values. Fixed rank/coordinate polynomials use the reserved rate and one allocated remaining tail fraction.

## 4. All finite microscopic cumulant corrections

For a multiindex n of total order q >= 1 put

\[
\Gamma^{(2)}_{\mathbf n}(W)
=\partial_{\mathbf t}^{\mathbf n}\mathcal C_2(0;W).
\tag{MS.18}
\]

By (MS.4), this is exactly the difference of the composite conditional microscopic cumulants for the QQ and PQ routes. The full first background source participates in both.

### Theorem MS.2 — finite source jets with one composite physical current

There are fixed positive kappa, c and C_L such that

\[
\begin{split}
h_2^{4q}\sum_a e^{\kappa n(Y_a)}
\left[\sup|\Gamma^{(2)}_{\mathbf n,a}|
 +\sup_W\sum_d\sup_{0<|u|\le1}
             |J^{(2)}_{\mathbf n,a,d,u}|\right]
\le C_L^{q+1}(q!)^2L^{8q}
       \prod_j b_j^{n_j}\,e^{-cP_0^2}.
\end{split}
\tag{MS.19}
\]

Here J is the finite current of the composite physical conditional cumulant in the filing described below. Every nonzero differentiated tag contains all differentiated microscopic source footprints and an old Q defect. The coupling threshold and kappa do not depend on q.

**Proof.** For n_j > 0 use the fixed polyradius

\[
r_j=\frac{\eta n_j}{2qM_j}.
\tag{MS.20}
\]

Apply Cauchy to each individual value and finite-current tag of (MS.17), before absolute aggregation. This bounds the result by

\[
C e^{-cP_0^2}(Cq)^q
             h_0^{-4q}P_0^{2q}\prod_j b_j^{n_j},
\tag{MS.21}
\]

since product(n_j!/n_j^{n_j}) <= 1. The same Cauchy estimate applies to the analytic numerator of each real finite difference uniformly in its displacement. Use q^q <= e^q q! and

\[
P_0^{2q}e^{-(c/2)P_0^2}\le q!(2/c)^q.
\tag{MS.22}
\]

This spends one fixed tail fraction for all q, rather than requiring q to be small relative to P0^2. Finally h2^(4q)/h0^(4q) = L^(8q), proving (MS.19). A source label absent from a tag gives zero derivative, proving the support assertion. ∎

## 5. Exact current filing and what is not proved

The microscopic marks in (MS.2) are unchanged functions on the original physical field U. Let K_PQ,W and K_QQ,W denote the two composite physical pushforward kernels defined by (MS.4), including all old and new densities, reconstructions and gauge preimages. For these bare microscopic marks, use the physical-pushforward convention already permitted in the first Gaussian/QC construction:

\[
B^{new}_{\mathbf n,a,d,u}=0,\qquad
J^{(2)}_{\mathbf n,a,d,u}
=\frac{\Gamma^{(2)}_{\mathbf n,a}(W_u)
                 -\Gamma^{(2)}_{\mathbf n,a}(W)}{u}.
\tag{MS.23}
\]

At order one this is the actual composite kernel response of the fixed microscopic scalar. At higher orders it is the compatible response of that kernel's conditional cumulant. In deriving its absolute bound, changes of the old reconstruction, old density/domain, new reconstruction, and new density/domain are retained as separate tagged subrecords; they are not canceled to improve the estimate. All are contributions to this newly specified composite physical kernel. The direct microscopic field difference with respect to W is zero in this presentation.

This is not a reassignment of already filed incoming M04 records. For canonical stepwise transport the next insertion is itself the old conditional field F1(V1). Its direct next record contains the variation of F1 along the reconstruction, including the old direct and old kernel records separately. To specify its two-copy comparison unambiguously, define

\[
q_{P,1}(da\mid W)=\nu_W(da),\qquad
q_{Q,1}(da\mid W)
=\frac{e^{H_1(0;\Psi_W(a))}}{\nu_We^{H_1(0;V_1)}}\nu_W(da),
\]
\[
G_{\eta,0}(\mathbf t;V_1)
=Z_{\eta,0}(\mathbf t;V_1)/Z_{\eta,0}(0;V_1),
\qquad\eta\in\{P,Q\}.
\tag{MS.23a}
\]

Thus G_{P,0} is the same function called G_{P,1} in (MS.3); the index 0 here labels its microscopic integrating layer. A canonical two-copy formula would keep

\[
\mathcal H_\eta(\mathbf t;W_{ins},W_{ker})
=\log\int q_{\eta,1}(da\mid W_{ker})
      G_{\eta,0}(\mathbf t;\Psi_{W_{ins}}(a)),
\tag{MS.24}
\]

and use its exact endpoint differences in the two copies. On the diagonal it gives the corresponding conditional source logarithm. Off the diagonal, the old and new domain families must be admitted and localized simultaneously. CA's diagonal core frame does not by itself verify that stronger rectangular two-copy family. No separate canonical second-step B/J bound is claimed here.

Likewise (MS.19) bounds the **rare difference** between two microscopic conditional laws. It is not a bound for the full PQ baseline in the final native energy grading. The latter requires a common two-layer primitive estimate of the form

\[
\beta_0\,|\mathsf s(U_{0,p}(z_0,z_1;W))|
\le C_L a_Y\left[\widehat R_Y(W)
       +\sum_{i\in Y}|z_{0,i}|^2
       +(g_1/g_0)^2\sum_{i\in Y}|z_{1,i}|^2\right]
\tag{MS.25}
\]

with actual full raw carriers, compatible reconstruction/background value, and the complete first-current coefficient records. Variational nesting identifies the zero-innovation field U1(M U2) with U2 on the minimal orbit. It does not alone prove the required local comparison of its microscopic curvature with the final raw-W Wilson-energy regulator. A forward averaged-curvature contraction is also not that comparison. That final-background force/prolongation estimate and the canonical two-copy marked family are the precise additional tasks for the absolute second marked theorem.

The cruder native bound MS.10 deliberately retains P0^2. Its use in the rare correction is legitimate because (MS.22) pays it with the old defect tail. The same cancellation is unavailable for an arbitrary nonrare smooth marked baseline.

The result therefore supplies actual two-step finite microscopic **correction** jets and their composite physical currents. It proves neither an ambient theorem, canonical M04 record propagation, an absolute scale-uniform marked theorem, all-depth closure, complementary P/Q sectors, nor a full outer connected physical hierarchy.

## Dependencies

* FJ/QC/LC: exact first sources, strict primitive marked Mayer reserve, original scalar reconstruction and first-cutoff domain certificates.
* MQ.34–37: compatible force-leaf and zero-subtracted fluctuation reconstruction; native coefficients are used here, without complexifying ambient guards.
* CA.4–25: raw joint field, exact constrained frame, capped native tube, common centered old Gaussian certificate and both real shell-current types.
* TD: joint multiplicity bound, same-gas colored component construction, strict fugacity enlargement and connected logarithm.
* CN: exact normalized same-gas current and complete support bookkeeping.
