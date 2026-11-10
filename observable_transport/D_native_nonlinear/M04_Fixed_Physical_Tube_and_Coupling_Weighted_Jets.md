# A fixed physical raw-field tube and coupling-weighted jets of the actual smooth mark

This note strengthens EJ.3 for the actual smooth three-layer microscopic mark. The native coefficient construction admits a fixed, sufficiently small physical raw-link tube about the identity. This is wider than the normalized one-coordinate discs used in EJ. On that tube the marked norm is of order the microscopic beta, so q normalized field derivatives have the explicit factor `g_3^q/g_0^2`. In particular the cubic-and-higher raw Taylor remainder is small on the actual weak-coupling small-link slice.

The wider object is an analytic coefficient continuation with the explicit retained selectors factored out. Its restriction to the admitted native domain equals the actual smooth conditional observable. It is not an analytic continuation of a sharp Q characteristic function. The result is fixed at three levels and does not give an all-depth source bound or a curvature-energy estimate on every native weak-curvature field.

## 1. The actual mark and the physical tube

Use the exact source F01/SE and SW conventions. On the final lattice define

\[
 \Phi_n(W)
   =h_0^4\sum_{x\in B_3(n)}
      (\mathcal T^{aaa}F_x)(W),
 \qquad F_x=\alpha\beta_0\sigma_{h_0}(x)-c,
 \quad \beta_0=(Ng_0^2)^{-1}.
 \tag{PJ.1}
\]

The three conditionals are precisely TR's first P / second auxiliary P / third auxiliary P conditionals. Their maps, couplings, gauge terms and domains remain fixed at zero microscopic source. The input is the complete microscopic source. In particular no retained-background piece is discarded before a conditional expectation.

The identity insertion transports exactly. Define

\[
 \Phi_n^{\alpha}(W)
    =\Phi_n(W)+c h_0^4|B_3(n)|.
 \tag{PJ.2}
\]

All field derivatives of \(\Phi_n\) and \(\Phi_n^\alpha\) agree. For \(\alpha=0\) they vanish. We work with the latter and restore the displayed identity term whenever values are needed.

Write the final raw links as

\[
 W_e=\exp B_e,\qquad
 B_e\in\mathfrak{su}(N)^{\mathbb C},\qquad
 \|B\|_\infty<r.
 \tag{PJ.3}
\]

The negative orientations are determined by inverse links. Fix the block size L, the three localization meshes and strict buffers. All constants below can depend on those fixed choices, N and fixed compact bounds for the three adjacent coupling ratios. They do not depend on the torus volume or the microscopic cutoff. The actual auxiliary radii are the source polylogarithmic radii, with fixed comparison fractions. In particular they obey

\[
 P_i\longrightarrow\infty,\qquad
 g_i P_i^3\longrightarrow0,
 \qquad i=0,1,2.
 \tag{PJ.4}
\]

Here \(P_0=p_0\), \(P_1=p_1\), \(P_2=p_2\) are TC's fixed product-ball comparison radii. They are not the later printed R-good radius. The displayed cubic smallness also implies \(g_iP_i\to0\) and \(g_i^2P_i^4\to0\). Merely assuming \(g_iP_i\to0\) would not justify the bounded-vertex estimates used below. Constants multiplying a fixed power of these radii cause no difficulty for the actual source polylogarithmic choice.

For an anchored supported family \(A_{n,Z}(B_Z)\), use

\[
 \|A\|_{\kappa,r}
   =\sup_n\sum_{Z\ni n}e^{\kappa n(Z)}
        \sup_{\|B_Z\|_\infty<r}|A_{n,Z}(B_Z)|.
 \tag{PJ.5}
\]

The carriers contain the original block root, every raw determining input and every normalization connector. This norm is only used on the stated small physical chart; it is not substituted for the specified global M03 norm.

## 2. Why the fixed physical tube is available

### Lemma PJ.1 — actual fixed-depth analytic continuation

There are \(r_0>0\), a positive carrier rate \(\kappa_0\), and a coupling ceiling, with the dependencies above, for which the actual smooth normalized family has a representation

\[
 \Phi_n^\alpha(e^B)=\sum_{Z\ni n}\Phi_{n,Z}^\alpha(B_Z),
 \qquad
 \|\Phi^\alpha\|_{\kappa_0,2r_0}
     \le C_L L^{12}|\alpha|g_0^{-2}.
 \tag{PJ.6}
\]

It is the analytic continuation of the admitted smooth mark. The coefficients and their component restrictions are the same fixed-depth family. They retain the complete determinant, Haar/coarea and normalized-kernel contributions.

**Proof.** The argument checks the size of the input to the existing native coefficient construction before using Cauchy estimates.

**(a) Source physical radii.** BA Section 4.3 and its admission discussion explicitly use the fixed physical-angle tube of CMP109 (2.9), equivalently a normalized fluctuation radius \(\epsilon_*/g_i\). CMP116 (1.13)--(1.21) gives the simultaneous minimizing-field and decoupler continuation on that physical tube. The local native class also contains the current/force input, as in CMP109 (1.11)--(1.19). None of these physical radii is the shrinking selector radius \(\epsilon_i(g_i)\).

**(b) Raw input admission about the identity.** On (PJ.3), each finite reference path, group mean, fractional edge lift and exceptional-coordinate solve is analytic on a smaller fixed chart. It equals its flat value at \(B=0\). The supported homogeneous BR/FC minimum construction used in TC.9 has a contraction with a strict margin and a gapped constrained propagator. Its input force and its prescribed-average mismatch vanish at identity and have absolute coefficient row sums bounded by \(C_L r\). The fixed-point equations therefore give a background correction of the same size. The full native input, including force and the averaged-gauge conversion, is bounded by \(C_Lr\) relative to the flat input. The three readouts add finite fixed-L stencils; they do not add a volume-dependent norm.

On a later real integration variable, the additional physical input is bounded by \(C_L\sum_i g_iP_i\). Choose r first, smaller than a fixed fraction of every native analytic buffer, and then use (PJ.4). Every complete input in the three nested integrations remains in that buffer. This verifies raw pullback admission on this small-link chart; it is not inferred from numerical closeness of one already integrated coefficient.

The supported substitution argument is TC.9 / CA.6: a physical correction of coefficient size q costs at most \(\exp(C_L q n(X))\) on a prior analytic carrier X. At these three fixed levels, choose \(r\) so that the sum of those costs fits the retained native carrier-rate margin. The same bounds apply when the complete outside-tag inputs are turned off in the common registry, because their absolute coefficient majorant only decreases. Thus the component equations and their local analytic branches remain the same ones.

**(c) Gaussian and interaction admission.** Each complete constrained precision retains its constraint-force terms and full averaged soft sampler. The physical raw perturbation of each coefficient is \(O_L(r)\), uniformly in the real capped later variables. The relative inverse and determinant use the same precision. The normalized complex marginal bound is TC.19 with an additional \(C_Lr\) in its small comparison parameter. A marginal of rank s has the resulting cost \(e^{C_Lrs}\). There are no growing hard-Q cores in the all-auxiliary family. Its ordinary rank is bounded by its fixed-buffer carrier volume, so choosing r below another fixed part of the spatial margin pays this cost at the primitive level. Old copies keep their own ranks and conditional normalization; they do not receive a new later quadratic store for each occurrence.

The source classical cancellations hold identically on this analytic family. Each minimizing map is the same critical branch, and the complete force correction is retained. The classical/gauge fluctuation remainder therefore has normalized size bounded by \(C_L(g_iP_i^3+g_i^2P_i^4+\cdots)\); the inherited bounded action difference has size \(C_LE_i g_iP_i\). The Haar/coarea factors are part of that same local perturbation. All are small at sufficiently weak coupling. Background-only classical terms are retained outside the normalized conditional; no uncanceled \(g_i^{-2}\) background action is treated as a small Mayer vertex.

The failed fixed-P tails remain Gaussian-small, with the covariance and determinant in the same family. CN's same-gas component cancellation and TC/TR's strict rooted estimates thus hold on a fixed smaller physical tube. Explicit retained selectors have already been factored out on the admitted domain; they are not continued as functions of B. Values of the resulting analytic extension outside that domain are used only for coefficient estimates.

**(d) The actual local source.** On this complete tube, the reconstructed microscopic links and their plaquettes have bounded holomorphic matrix norms. Their supported analytic row expansions are the same BR/FC and fluctuation reconstructions just admitted. The holomorphic Wilson trace, and hence \(h_0^4F_x\) with its constant removed, has absolute coefficient norm at most \(C_L|\alpha|\beta_0\). Summing over the \(L^{12}\) microscopic sites in the final block gives at most \(C_L L^{12}|\alpha|g_0^{-2}\), with N absorbed into the constant.

Insert this source before the normalized component expansion. A circle of radius \(c g_0^2/(L^{12}|\alpha|)\), with c sufficiently small, makes its source species fit the same strict margin. The three exact denominators are the ones of TR; CN cancels their vacuum components against the same full gas. Source Cauchy therefore returns the source norm once and gives (PJ.6). This is the bounded-source version of TR's construction. It needs no probability bound for a whole-volume P event and no source-dependent coupling retuning.

Normal convergence proves holomorphy and the asserted identical component restrictions. On admitted real inputs all changes used in the construction are the exact original fixed-P coordinate changes and normalizations. Thus its value there is (PJ.1)--(PJ.2). \(\square\)

The fixed tube is a local chart about the identity orbit. The lemma does not assert that every globally weak-curvature field has one global small-link representative, or that a large winding carrier can be gauged into this tube with uniform constants.

### Corollary PJ.1a — the same bound on every compact real gauge chart

For a fixed real site gauge \(u\), use the physical chart
\[
 W_e=u_{x(e)}\exp B_e\,u_{y(e)}^{-1},\qquad \|B\|_\infty<2r_0.
 \tag{PJ.6a}
\]
Transport the entire reference, force, target, constraint and Gaussian family by this gauge before forming its component restrictions. The bound (PJ.6), with exactly the same radius and envelope constants, holds in every such chart, uniformly in u and in the number of sites. It holds for each complete scalar coefficient in the native equivariant registry. A later compact Haar projection of these scalar coefficients therefore has a uniformly bounded integrand on every orbit chart.

**Proof.** CMP116 Lemma 2, printed p.11, states that each localized fluctuation vertex and both pieces of its decomposition are invariant under simultaneous complex gauge transformations in a neighborhood of all real gauge transformations. Printed pp.21--22 proves the same statement for the component activities (2.14), then explicitly extends the coefficient functions constantly along whole gauge orbits meeting the native domain. The local marked insertion is a gauge-invariant Wilson trace. Inserting it before the same component construction preserves these transformation statements. Source differentiation and the exact normalizations preserve them as well.

For the raw pullback, BR.27--29 and TC.9 transform the complete reference configuration, source-normalized force and prescribed-average mismatch simultaneously. Uniqueness of the critical branch transports the minimum and its constrained reconstruction. The finer site gauge is the natural block lift of u, followed by the already specified averaged-gauge conversion. It is never replaced by a new identity reference on an outside-decoupled component. In the relative link charts the linear tangent maps are unitary adjoint maps. They preserve the physical sup radii, normalized Lie-algebra balls, quadratic positive bounds and fluctuation measures. Precision and covariance conjugate by the same real orthogonal maps; their inverse and determinant branches therefore transform together. Haar/coarea densities and source scalar insertions are invariant.

Every operation in the proof of Lemma PJ.1 consequently has the same absolute coefficient majorant after this transport. The analytic B tube has the same radius because conjugation by a real compact-group element is isometric. Integrating over real u therefore cannot increase its coefficient supremum or its carrier sum. This proves the claimed uniformity. It does not assert that an arbitrary independent complex gauge transformation is isometric. \(\square\)

One may use the support-preserving compact gauge projection developed in EC for a scalar coefficient family whose literal representation is not already termwise invariant. Each complete scalar coefficient is projected only after its full contractions and determining support have been recorded. Projection of individual overlapping uncontracted factors would not in general preserve their product and is not used here. For derivatives, fixed-order group constants and carrier incidence polynomials are paid in the same way as in PJ.2; the claim is not a blind interchange of a path supremum and an integral.

### Lemma PJ.1b — a bounded-source envelope at every admitted native center

Let \(\mathfrak N_3\) be the actual real three-level homogeneous smooth native class used in TC/TR, with the fixed strict buffers. Its fields need not have a global small-link representative. On a smaller uniform relative physical tube about every center of \(\mathfrak N_3\), the same complete scalar carrier family can be given nonnegative deterministic envelopes \(m_{n,Z}\) such that
\[
 |\Phi_{n,Z}^\alpha(W)|\le \frac{m_{n,Z}}{g_3^2},\qquad
 \sup_n\sum_{Z\ni n}e^{\kappa_1 n(Z)}m_{n,Z}
       \le C_L B_3,
 \quad B_3=L^{12}|\alpha|(g_3/g_0)^2.
 \tag{PJ.6b}
\]
For the normalized raw left derivatives and a fixed smaller rate,
\[
 \sum_d\sup_{W\in\mathfrak N_3}
       |D_d\Phi_{n,Z}^\alpha(W)|
    \le \frac{C_L n(Z)m_{n,Z}}{g_3}.
 \tag{PJ.6c}
\]
The supremum can include each admitted normalized coordinate path in its buffered domain. The constants and envelopes are uniform over the real native centers and their compact gauge orbits. The conclusion is termwise and precedes summation of the physical conditional; a bound on its total expectation is not used in its place.

**Proof.** We apply a bounded source to the existing TC/TR common coefficient construction at each native center. Three facts verify uniformity.

First, the real background bounds, their full constraint-force corrections and their strict native \((U,J)\) buffers are uniform at those centers. The actual background-uniform constrained gap is BA Section 4.2, from CMP99 (3.156)--(3.158), transferred there to the full soft gauge. BR/FC expresses the relative background in the complete compact reference, force and prescribed-average mismatch, with the same convergent contraction and row-sum bounds. At three fixed levels each raw physical perturbation of size r changes these complete inputs by at most \(C_Lr\). The reference is constructed from locally close contour transports and near-identity plaquette defects; its real base links may be arbitrary unitary matrices. The fixed-point contraction and the local exceptional solves therefore give a unique continued branch on a fixed smaller r, uniformly in the center. Choosing r inside all native buffers admits all its component restrictions by the same absolute substitution bound as in Lemma PJ.1. The capped real innovations add only \(C_L\sum_i g_iP_i\), which is smaller than that buffer. No global gauge of a nontrivial holonomy is taken.

Second, the covariance and determinant comparison, ordinary ranks, interaction envelopes and exact component normalizations are precisely those of TC/TR at that center. Their constants depend on the uniform native gap and the same strict margins, so they are uniform in the center. The continuation uses the complete precision and the complete native force; it does not reconstruct a different Gaussian at a different center. Every old conditional node is estimated before its parent is integrated, as in TC, and leaves no new parent quadratic store per old occurrence.

Third, the microscopic Wilson trace has the elementary bounded-source estimate on these tubes. A reconstructed link is a bounded holomorphic perturbation of a unitary link. A plaquette contains four such links, so its holomorphic trace is bounded by a fixed group constant times \(e^{C_Lr}\), independently of its real base and of its holonomy. Thus the complete local source \(h_0^4\sum_{x\in B_3(n)}\alpha\beta_0\sigma_{h_0}(x)\) has supported source envelope at most \(C_LL^{12}|\alpha|g_0^{-2}\). Insert this source with the inverse-beta circle used in Lemma PJ.1(d) before taking the rooted expansion. The strict marked and unmarked component bounds and CN's exact same-gas cancellation give a summable nonnegative envelope for each root tag. Their absolute estimates were uniform in the native center, so the resulting envelopes can be chosen before that center varies. This proves (PJ.6b), since \(B_3/g_3^2=L^{12}|\alpha|/g_0^2\).

Finally, one normalized raw variation has physical size \(g_3\). Cauchy on the fixed smaller relative tube gives \(C_Lm_{n,Z}/g_3\) per raw direction. There are at most \(C_Ln(Z)\) directions in the complete determining footprint. These deterministic envelopes hold along the whole buffered path, giving (PJ.6c); their incidence polynomial is summable at a smaller rate. Corollary PJ.1a and EC permit compact gauge projection without changing support or the value envelopes. \(\square\)

This lemma is restricted to the actual all-smooth fixed-depth native class. It neither supplies a globally holomorphic hard-Q density nor asserts admission for arbitrary compact fields. It also does not eliminate winding dependence: a flat field with nontrivial torus holonomy can lie in \(\mathfrak N_3\), and its long or winding scalar coefficient is controlled by (PJ.6b), not by the small-link Taylor estimate below.

## 3. All fixed field orders with the actual coupling powers

Use normalized final coordinates \(B_e=g_3a_e\). For a fixed nonnegative spatial moment order s and integer q define

\[
 \mathcal J_{q,s}(\Phi)
 =\sup_n\sum_{Z\ni n}e^{\kappa n(Z)}
   (1+\operatorname{diam}(Z)^s)
   \sum_{d_1,\ldots,d_q}
    \left|\partial_{a_{d_1}}\cdots\partial_{a_{d_q}}
                \Phi_{n,Z}^\alpha(e^{g_3a})\big|_{a=0}\right|.
 \tag{PJ.7}
\]

The indices d are actual final raw bond/colour directions; directions not read by the complete carrier have zero derivative. Distances are in final lattice units.

### Theorem PJ.2 — coupling-weighted actual smooth jets

For every fixed q and s, and \(0<\kappa<\kappa_0\),

\[
 \mathcal J_{q,s}(\Phi)
 \le C_{L,q,s,\kappa_0-\kappa}
          L^{12}|\alpha|\frac{g_3^q}{g_0^2}.
 \tag{PJ.8}
\]

In particular, for \(q\ge2\),

\[
 \mathcal J_{q,s}(\Phi)
 \le C_{L,q,s}\,B_3\,g_3^{q-2},
 \qquad
 B_3=L^{12}|\alpha|(g_3/g_0)^2.
 \tag{PJ.9}
\]

Thus the normalized cubic through sixth-order jets have factors \(g_3,g_3^2,g_3^3,g_3^4\), respectively. This strengthens the fixed-order boundedness in EJ.25. The constants here are not asserted independent of q.

**Proof.** Apply the multivariable Cauchy formula to each coefficient in (PJ.6) on a smaller physical polydisc. Each normalized derivative contributes \(g_3/r_0\). For a list of q coordinate derivatives, the bound is \(C_q r_0^{-q}g_3^q\) times the coefficient supremum. The number of coordinate lists is at most \(C_L^q n(Z)^q\), since the full determining data are part of the carrier. Its fixed spatial moment is bounded by a polynomial of degree s in the same size. The spare exponential rate sums these polynomial factors. This proves (PJ.8), and (PJ.9) is its exact coupling rearrangement. No radius proportional to g is used for this step. \(\square\)

The actual mark is invariant under global colour conjugation on the physical real tube, by SW.1, and this identity continues analytically. If needed average each coefficient over the compact global colour group; the tube and its bounds are unchanged, support is preserved, and the sum remains the same physical function. Its linear coefficient is then an invariant linear functional on the adjoint representation and is zero. We can therefore use a supported coefficient family with

\[
 D\Phi_{n,Z}^\alpha(0)=0.
 \tag{PJ.10}
\]

The actual retained gauge and hypercubic symmetries of the summed physical mark are unchanged. The compact colour averaging is only a choice of coefficient representation, not a change of the conditional law.

## 4. A quantitative nonlinear remainder on the actual small-link slice

Write

\[
 Q_n(a)=\frac12D_a^2\Phi_n^\alpha(0)[a,a],
 \qquad
 \mathcal N_n(a)
    =\Phi_n^\alpha(e^{g_3a})-\Phi_n^\alpha(I)-Q_n(a).
 \tag{PJ.11}
\]

The same subtraction is made coefficientwise in the representation of (PJ.10). Let \(P\ge1\), and suppose

\[
 g_3(P+2)\le r_0/4.
 \tag{PJ.12}
\]

The field can additionally be restricted to the actual admitted native small-link slice. For example \(P\le c_Lp_0(g_3)\), with the fixed c sufficiently small for the source selector buffers, is sufficient: the minimum/reference row estimates in Lemma PJ.1 bound its actual defining fields by \(C_Lg_3P\). No assertion about arbitrary weak-curvature holonomy fields is made.

### Proposition PJ.3 — supported small nonlinear remainder

On \(\|a\|_\infty\le P\), at a smaller positive carrier rate,

\[
 \sup_n\sum_{Z\ni n}e^{\kappa n(Z)}
          \sup_{\|a\|_\infty\le P}|\mathcal N_{n,Z}(a)|
       \le C_L B_3 g_3P^3,
 \tag{PJ.13}
\]

\[
 \sup_n\sum_{Z\ni n}e^{\kappa n(Z)}
       \sup_{\|a\|_\infty\le P}
          \sum_d|\partial_{a_d}\mathcal N_{n,Z}(a)|
       \le C_L B_3 g_3P^2.
 \tag{PJ.14}
\]

Fixed spatial moments can be inserted in both estimates by a further strict rate loss. The analogous bounds for p=2 and p=3 normalized derivatives have factors \(B_3g_3P\) and \(B_3g_3\). For a finite normalized coordinate path, its integrated derivative has the bound (PJ.14) with P replaced by P+1.

**Proof.** For a single coefficient set \(f(t)=\Phi_{n,Z}^\alpha(tg_3a)\). It is holomorphic for \(|t|<2r_0/(g_3\|a\|_\infty)\), with the bound in (PJ.6). Its linear coefficient vanishes by (PJ.10). The geometric bound on its Taylor tail beginning at degree three gives \(C(g_3P/r_0)^3\) times that coefficient bound. Summing with the remaining rate gives (PJ.13).

For one physical coordinate derivative, the Taylor series of the differentiated remainder begins at degree two. A Cauchy estimate in that coordinate on a fixed fraction of the physical tube gives the bound \(C g_3(g_3P)^2r_0^{-3}\) times the same supremum. Summing the differentiated positions costs one carrier incidence polynomial, paid by the strict rate margin. This proves (PJ.14). The p=2 and p=3 cases follow from the same differentiated Taylor series. A finite current is the integral of this actual derivative along its prescribed path; no fresh value representation is chosen after differentiation. \(\square\)

These estimates are actual nonlinear bounds, with a small factor \(g_3P^3\) when P has the source logarithmic growth. They are bounds on the small-link slice and in its supported analytic carrier norm. They do not yet compare the nonlinear conditional law to the FH Gaussian transfer, and they do not turn \(\mathcal N_n\) into a gauge-invariant object by itself. Subtracting a raw quadratic Taylor polynomial preserves only its linearized gauge symmetry. A fully nonlinear Wilson completion, followed by the local-source Ward argument, is a separate necessary step for a gauge-invariant irrelevant field.

## 5. What is available to the next calculation

PJ.8 supplies finite jets through order six and any fixed carrier moment for the **actual local** marked field \(\Phi_n\), with the explicit normalized coupling powers. It is therefore an input to local two-momentum Ward matching and to a finite smooth-background engineering expansion. It does not assume a common physical source radius independent of beta; the local source circle in the proof has the actual inverse-beta size.

PJ.13--PJ.14 supply a concrete nonlinear Taylor error with physical supports and a normalized composite first current. The input coupling ratio \((g_3/g_0)^2\), the fixed-depth engineering factor \(L^{12}\), and every original conditional normalizer remain present. The proof neither differentiates a running map nor changes the supplied zero-source couplings.

The unresolved comparison is between this actual nonlinear marked conditional transport and its inherited Gaussian quadratic part on the full native class, with moving hard Q cores and separately retained physical origins. A global small-link chart is not a substitute for that class. No M04 completion or Yang--Mills existence claim follows from this note.

Primary inputs: CMP109 (1.7)--(1.19), (2.6)--(2.18); CMP116 (1.13)--(1.21), Lemmas 1--2, and (2.5)--(2.26); the actual native tube analysis BA; the complete raw/coefficient/conditional families in TC, CN and TR; and SW's literal physical symmetries.
