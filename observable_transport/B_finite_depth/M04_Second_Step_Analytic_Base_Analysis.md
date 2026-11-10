# The analytic base for a second regular step

## 1. Conclusion and exact scope

Bałaban's papers do provide an analytic native input for a second regular integration of the first all-R-good density. They also provide the correct weak-curvature ordinary Gaussian precision and a coefficient construction with exact component identities. These are substantive inputs to a second-step proof, rather than merely a flat Gaussian analogy.

Three qualifications delimit that result.

1. The leading coarse action is the Wilson action of the first minimizing field, \(A(U_1(V_1))\). It is not the bare coarse Wilson action \(A(V_1)\). The first determinant and all measure/coarea terms remain in the effective action.
2. The source locality and analyticity are in the native pair \((U,J)\) and the next fluctuation variables. A common family in the raw retained field \(V_2\), with the required compact extension and physical current footprints, still requires the actual minimizing-field pullback. Native locality alone is not that pullback theorem.
3. The first R-averaged correction \(\delta E_1=\log(Z_{Q,0}/Z_{P,0})\) has not been proved analytic in \(V_1\), and is not included in the analytic base. Sharp moving-Q factors remain separate integral payloads. No closure for the complete second R-averaged density is claimed here.

Use \(g_0,g_1\) for the first two couplings, \(V_1,V_2\) for their retained fields, and

\[
 P_0=\delta_0/g_0
 \tag{BA.1}
\]

for the unambiguous first normalized free-coordinate cutoff in CMP119 (1.18). Subscripts on \(Z_{P,0}\) and \(Z_{Q,0}\) indicate the first integration. Fixed trace, lattice and Gaussian normalization factors are kept in the same place on both sides of each displayed identity.

## 2. What the first base density actually contains

Take the first branch with \(\Omega_1=\Lambda_1\) equal to the full lattice, no P/Q bad components and \(R_1=\varnothing\). Then \(S_1=\varnothing\). There is no remaining old-variable operation \(T_1\), no boundary \(B^{(1)}\), and no reset correction.

CMP119, printed pp.252–254, (1.25)–(1.30), identifies its density. In the notation used for the current R-average, write

\[
 \rho_{P,1}(V_1)=C_0(V_1)Z_{P,0}(V_1).
 \tag{BA.2}
\]

Restoring the retained selector explicitly, the source formula is

\[
 \rho_{P,1}(V_1)
 =\chi_1(V_1)e^{-E_1^{\rm vac}}
   \exp\!\left[
      -g_1^{-2}A(U_1(V_1))
      +\mathcal E_1(U_1(V_1))
   \right],
 \tag{BA.3}
\]

where

\[
 \mathcal E_1(U)
 =E^{(1)}(g_0,U)-E^{(1)}(g_0,1)
             -\beta_1(g_0)A(U).
 \tag{BA.4}
\]

On this full branch the source spatial coupling and counterterm cutoff are constant. Equation (BA.3) includes the running-coupling convention (1.27); it is the specialization of (1.30), not a new renormalization.

The paragraph following (1.30) explicitly says that the Gaussian normalization \(\log Z^{(0)}(\Lambda_1)\) in (1.26) has been combined into the new \(E^{(1)}\). The original Haar density, nonlinear averaging Jacobian and exceptional-bond coarea factor occur in (1.14)–(1.16) before that integration. They are part of the same output; none may be set to one. The vacuum constant collects only terms independent of the retained field. CMP109 (1.3)–(1.6) gives the corresponding convention with the Gaussian normalization displayed separately.

The equality in (BA.3) concerns the first all-R-good subdensity. The full first R average is instead

\[
 \rho_{Q,1}
    =\rho_{P,1}e^{\delta E_1}.
 \tag{BA.5}
\]

This is the exact density identity RA.20. Equation (BA.5) does not imply that the last factor belongs to the analytic class used for \(\mathcal E_1\).

There is a concrete starting formula for the second-step construction considered here. Apply the next full-lattice physical group-averaging operation to this **new first R-averaged density**, insert its ordinary next P/Q partition, and take the \(\Omega_2=\) full term. Sum the next R partition exactly, so that it is absent again. With the chart \(\Psi_{V_2}\), precision \(K_1\) and smooth perturbation \(W_1\) defined below, that term is

\[
\begin{split}
 \rho^{\,{\rm new}}_{QQ,2}(V_2)
  ={}&\chi_2(V_2)C_1(V_2)
       \int da\,\chi_{Q,1}(a,V_2)\\
    &\times
       \exp\!\left[-\tfrac12 a^TK_1(U_2)a
                          +W_1(a,U_2,J_2)\right]\,
       \exp\!\left[\delta E_1(\Psi_{V_2}(a))\right].
\end{split}
 \tag{BA.5a}
\]

Here \(C_1\) retains the leading factor
\(\exp[-g_1^{-2}A(U_2)]\), the zero-fluctuation inherited value
\(\exp[\mathcal E_1(U_2)]\), the previous vacuum constant, all retained-only Haar/coarea or normalization factors, and any Gaussian normalization assigned to it by the chosen measure convention. The smooth \(W_1\) contains the inherited difference (BA.7), every nonconstant classical/gauge remainder, and all remaining Haar/coarea terms of CMP109 (2.12). Section 5 justifies removal of the old \(\chi_1\) on this fiber. The sharp old correction is left as the exact displayed insertion.

Equation (BA.5a) is a change of variables in the stated physical averaging operation. It does not assert that the original future history-dependent geometry kernels may be applied after the first R labels have been erased. The operation change and the density-state convention in RA remain explicit. At this scope there is no old-component analytic boundary functional: there is the ordinary no-old-component base plus the separately retained \(\delta E_1\) payload.

## 3. The supplied analytic class is a constructed local family

CMP109 (1.7)–(1.19), printed pp.261–264, defines

\[
 E^{(1)}(U)=\sum_X E^{(1)}(X,U,J(U)),
 \qquad
 |E^{(1)}(X,U,J)|\le E_0e^{-\nu d_1(X)}.
 \tag{BA.6}
\]

Each coefficient depends only on \((U,J)|_X\), is analytic on its specified local complex domain, and has the stated complex gauge covariance. The domain includes a local real gauge representative, a small complex relative field, a bound on the current \(J\), and admission of the nested determining maps; these are (1.11)–(1.16). The discussion on printed p.263 proves that sufficiently regular actual minimizing fields lie in an interior subdomain of this class. It does not assume a global small-link gauge.

CMP109 alone does not complete the locality proof: printed p.298 expressly defers that step. The supplied successor, CMP116, completes it. Its first page states that it finishes CMP109 Theorem 3, and its final paragraph on printed p.22 closes that proof. The following concrete constructions matter here.

### 3.1 A fixed coefficient construction and component equations

CMP116 (1.2)–(1.5) writes the nonlinear minimizing-field response in terms of the actual propagators and contraction equations for \(D\) and \(A_0\). Equations (1.6)–(1.7) expand the propagators into generalized walks. Each walk term depends on the gauge field restricted to its full localization domain; its kernel vanishes near that domain's boundary.

The source then attaches decouplers to those same terms. On setting outside decouplers to zero, (1.3) and (1.4) become separate contraction equations in the connected components. Uniqueness of their solutions gives the component identity, not just an estimate of weak communication. The discussion preceding (1.10), printed pp.4–5, proves that a derivative belonging to a component disjoint from the marked initial component vanishes. The resulting terms depend only on the native data in their displayed carrier.

The complex decoupler disc is controlled in (1.11)–(1.21). This is a simultaneous family obtained from one coefficient registry for the given initial localization. Independently re-solving unrelated domain problems and identifying their coefficients is unnecessary.

### 3.2 All inherited action and measure terms are included

CMP116 Lemma 1, (1.33)–(1.36), localizes the inherited difference

\[
 \mathcal E_k\!\left(U_k(e^{iB'}V^{(k)})\right)
        -\mathcal E_k\!\left(U_k(V^{(k)})\right).
 \tag{BA.7}
\]

Lemma 2, (1.41)–(1.43), adds the remaining classical, gauge and measure terms in the fluctuation integral. It writes the complete perturbation as localized analytic vertices, with a small quadratic-form part and a bounded inherited part. Thus one does not need to assume that the determinant has no response when the second field varies.

### 3.3 The Gaussian marginal and final polymer identities

CMP116 (2.5)–(2.6) is an exact normalized Gaussian conditional integration. It retains its determinant ratio, Schur completion and the outside Gaussian variables. The inverse square root is localized using its resolvent representation and the same source propagator expansions, printed p.13.

Equations (2.8)–(2.10) then give a local family \(H(Z)\) and the exact identity

\[
 H(Z_1\cup\cdots\cup Z_n)=\prod_{i=1}^n H(Z_i)
 \tag{BA.8}
\]

for the actual separated components in that construction. Equations (2.11)–(2.13) perform the connected logarithm. At printed p.21 the localized Gaussian log normalization is added back, with its own exponential coefficient bound. This proves the full native action class, including the determinant.

The source may choose its walk localization domains to suit an initial carrier \(Z_0\). That choice is an explicit tag of the construction. Equation (BA.8) is a consistency statement for the resulting source family. It does not assert that an arbitrarily selected, independently reconstructed raw-field covariance family has the same coefficients.

The source distance \(d_1(X)\) is a tree length on a fixed M-block grid, as defined in CMP109 (0.24)–(0.25). At this fixed scale the full M-block count of a connected carrier is bounded by a constant times \(1+d_1(X)\). A strict loss of rate therefore pays finite incidence factors. This observation does not pay a growing MR halo around every carrier.

## 4. The correct second saddle, force cancellation and Gaussian gap

The next classical saddle is the minimum, at fixed next average \(V_2\), of

\[
 V_1\longmapsto A(U_1(V_1))+G(V_1).
 \tag{BA.9}
\]

CMP109 (2.2)–(2.3) and CMP119 (3.10) identify it as
\(V^{(1)}=M^1 U_2(V_2)\). The first action in (BA.9) is already a minimized microscopic action. Replacing its Hessian by the bare one-step Wilson precision is incorrect.

Use the actual next constraint chart

\[
 V_1=\Psi_{V_2}(a)
     =\exp i\{g_1 C_1a-h_1D_1(g_1C_1a)\}\,V^{(1)},
 \qquad Q_1C_1a=0.
 \tag{BA.10}
\]

The map \(C_1\) solves precisely the source exceptional bonds and leaves the independent entries unchanged. The nonlinear solve is local to the actual averaging footprints; CMP109 printed p.267 gives \(LQ_1h_1=I\) and the equation for \(D_1\).

### 4.1 The constraint-force term is essential

CMP109 (2.6)–(2.11) performs the expansion. The nominal \(g_1^{-1}\) linear term vanishes because the derivative of the classical action annihilates the exact next-average tangent space. The quadratic precision includes the second derivative of the constraint parametrization paired with the nonzero microscopic force \(J_2\).

This term is displayed explicitly in CMP109 (1.5) and CMP99 (3.156):

\[
 q_1(b)
 =\tfrac12\langle b,\text{classical response Hessian}\,b\rangle
       -\langle H_1D^{(2)}_1(b),J_2\rangle
       +\tfrac12G^{(2)}(b).
 \tag{BA.11}
\]

The notation here collects the source trace factors. It is the complete constrained quadratic form. The force is not discarded merely because it is small.

CMP109 (2.12)–(2.13) retains the full nonlinear action, Haar and constraint-Jacobian terms, and the inherited action (BA.7). The Gaussian normalization \(Z^{(1)}(U_2)\) is part of the next effective action, just as \(Z^{(0)}\) was at the first step.

### 4.2 The nonflat source gap

CMP99, printed p.428 immediately after (3.158), states that the independent-coordinate operator

\[
 C^*\Delta_k C\ge \gamma_0 I
 \tag{BA.12}
\]

has a positive lower bound independent of \(k\) and of the admitted weak-curvature background \(U\). Its hypotheses are (3.35)–(3.36), with \(M\alpha_0\) sufficiently small. The preceding (3.156) includes the force/constraint correction. The text explains that the flat result is extended by localization and the weak-background estimates. The generalized-walk construction and complex extensions are developed in that paper; CMP116 (2.15)–(2.24) explicitly controls their complex perturbations, including determinant ratios.

The formulation in CMP99 at this point uses the axial slice. CMP109 (2.11) uses the corresponding quadratic with exponential gauge fixing. Here is the precise transfer.

On the exact next-average fiber, the classical functional is gauge invariant and critical at \(V^{(1)}\). Its constrained Hessian therefore annihilates every center-fixed infinitesimal gauge vector \(D_{V^{(1)}}\phi\), including mixed pairings. This follows by differentiating invariance at a critical point. Omitting the force term in (BA.11) would invalidate that argument.

Let \(\tau_{\rm av}b\) be the derivative of the actual averaged contour variable. At the source representative the contour variable is identity and covariance gives

\[
 \tau_{\rm av}D_{V^{(1)}}\phi=\phi.
 \tag{BA.13}
\]

All maps in (BA.13) are within fixed L-blocks. Their norms, and those of a tree-slice gauge projection, are bounded by constants depending only on fixed L and the admitted native bounds.

Put \(b_{\rm av}=b-D_{V^{(1)}}\tau_{\rm av}b\). Project it to the hard tree slice. The classical quadratic is unchanged, and the two slice representatives have uniformly comparable norms. The axial bound (BA.12) implies
\(q_{\rm cl}(b_{\rm av})\ge c_L\|b_{\rm av}\|^2\).
The actual soft-gauge quadratic is a fixed positive multiple of
\(\|\tau_{\rm av}b\|^2\). Since
\(\|b\|\le C_L(\|b_{\rm av}\|+\|\tau_{\rm av}b\|)\), adding these bounds yields

\[
 K_1(U_2)=C_1^*\Delta^{\rm soft}_1(U_2)C_1
       \ge c_L I,
 \qquad \|C_1a\|\ge\|a\|.
 \tag{BA.14}
\]

This is the native second-step Gaussian gap, with no flat substitution and no missing gauge variables.

### 4.3 What may be inferred about the complete smooth potential

The source native perturbation is analytic in a fixed physical-angle tube, equivalently \(\|a\|_\infty<\epsilon_*/g_1\). Its localized decomposition is Lemma 2 of CMP116. Choose a strict interior tube. Cauchy estimates on each inherited bounded vertex, followed by the exponentially convergent sum of its carrier incidences, give an operator-norm Hessian bound \(C E_0g_1^2/\epsilon_*\). The classical/gauge nonlinear and Haar/coarea vertices give a bound \(C\epsilon_*\); this also follows directly by differentiating their Taylor expansions, whose classical remainder begins at order three before division by \(g_1^2\).

More explicitly, the source coefficient bound (1.43) supplies the quadratic matrix row summability. Differentiating its analytic coefficients adds finite powers of carrier size; the strict carrier-rate margin sums those powers. Differentiating the bounded inherited vertices twice costs \(O((g_1/\epsilon_*)^2)\) and the factor \(E_0\epsilon_*\) in (1.36). These estimates are volume independent. They do not follow from a bound on an extensive unlocalized logarithm.

Consequently, for the smooth second-step potential written as
\(\tfrac12a^TK_1a-W_1(a)\),

\[
 \|\nabla_a^2 W_1\|_{2\to2}
       \le C\epsilon_*+C E_0g_1^2/\epsilon_*.
 \tag{BA.15}
\]

Choose \(\epsilon_*\) first, inside the source tube and small relative to (BA.14), and then \(g_1\) small. The complete smooth potential retains a gap at least \(c_L/2\) on the smaller tube. Any broad comparison radius \(P_1\) with \(g_1P_1\to0\) eventually lies there. The statement concerns this smooth density before moving hard cutoffs. It does not assert that a log of a completed sharp-cutoff marginal has the same Hessian.

## 5. Old admission on the full next Q-domain

The old coarse selector is not left as an unexplained indicator in the second fully regular operation.

CMP119 inserts the new P and Q decompositions in (3.2)–(3.3). On \(\Omega_{k+1}^{\sim-1}\), the proof in (3.6)–(3.9), printed p.266, then shows

\[
 \chi_k=1,\qquad \chi_{\rm Ax}=1.
 \tag{BA.16}
\]

This calculation occurs before the saddle construction, the rescaling in (3.15), and the R decomposition (3.16). It therefore uses the actual next P/Q restrictions and their source buffer, rather than a later all-R-good restriction.

At \(k=1\), \(\Omega_2=\) full, there is no remaining boundary strip. Equation (BA.16) removes the old \(\chi_1(V_1)\) throughout the original source-admitted Q2 fiber. The local-field comparison (3.7) gives strict smallness after taking \(A_1/A_0\) and the coupling sufficiently small; (3.8) then proves the old local minimizing-field curvature bound. The new minimum is regular by (3.12), and the actual relative field satisfies

\[
 \|\log(V_1(V^{(1)})^{-1})\|_\infty
          \le C\epsilon_1(g_1)\longrightarrow0
 \tag{BA.17}
\]

by (3.13)–(3.14). No all-R-good assumption is used in (BA.17).

For the analytic base, this resolves the native admission question. CMP109 printed p.263 admits the actual regular minima in a strictly buffered complex \((U,J)\) domain. CMP116 (1.13)–(1.21) gives the simultaneous minimizing-field response on a fixed physical-angle tube and fixed complex decoupler disc. Since the real bound in (BA.17) tends to zero, the entire actual second Q-domain lies in an interior part of that native tube at weak coupling. The allowed complex neighborhood may be chosen with a fixed positive physical-angle radius before dividing by \(g_1\).

Two limitations remain essential. First, this is the source's admitted fiber and its stated native complex continuation; it is not an off-support identity for every compact retained field. Second, a newly constructed outside-decoupled raw frame must be shown to remain in that tube. The quantitative criterion is explicit: its local complex change in the physical fluctuation angle and native current must be less than a fixed fraction of the above buffer. Real selector redundancy alone does not verify that criterion for an arbitrary new family.

The modified shrinking radii in CMP119 (2.28) are also a legitimate source filing, with their own parameter choices and nested bounds. They should not be mixed silently with the fixed-radius small-field filing. For the two clean steps here the fixed native tubes of CMP109/CMP116 and the actual minimum admission just described suffice; the broader mixed-history filing is not being claimed.

## 6. The literal next cutoff and a permissible auxiliary comparison

There are three distinct radii.

| Source operation | Variable and literal radius | Consequence |
|---|---|---|
| CMP109 (2.9) | Physical relative angle \(B'\): \(|B'|<\epsilon_*\); after scaling, \(|a|<\epsilon_*/g_1\). The optional coupling-dependent cutoff in the sentence following (2.9) is a separate convention. | This is the original small-field analytic construction. |
| CMP119 first split (1.18) | Normalized first free variable: \(|a_0|<\delta_0/g_0=P_0\). | This is the first all-R-good base used in (BA.2). |
| CMP119 next split (3.16) | After the explicit scaling preceding (3.15), the printed inequality is \(|A_1|<\delta_1\), while (3.3) defines physical \(\delta_1=g_1(A_1/A_0)p_0(g_1)\). | Read literally, this normalized radius tends to zero. It must not be called the broad radius \(\delta_1/g_1\). |

The prior normalization analysis remains applicable. No notation correction is made here.

After the exact next R sum, however, its partition is absent from the physical Q integral. One may introduce a new auxiliary broad comparison cutoff, for example \(P_1=c\,\delta_1/g_1\) with a fixed small positive \(c\), provided its inclusion in the actual Q-domain is proved. This is a comparison density, not a relabeling of the printed next R-good sector.

The needed inclusion uses the sharper comparison in CMP119 (3.17)–(3.19), printed pp.268–269, not the coarser \(O(\epsilon_1)\) bound in (3.13). The argument of the local minimizing response in (3.17) is supported near the boundary of the four-layer determining box. Equation (3.18) applies its exponential decay, and the actual averaging estimates in (3.19) give

\[
 \|V^{(1)}_e(V^{(1)}_{\square,e})^{-1}-I\|
       \le C\epsilon_1(g_1)e^{-cR_{\rm next}}
       =o(\delta_1)
 \tag{BA.18a}
\]

on every overlapping starred Q footprint. Here \(R_{\rm next}\) denotes the source next-scale buffer; replacing it by the comparable preceding radius in the printed final bound makes no difference. Although these equations are displayed after the R decomposition, this estimate concerns only the fixed new background and its local comparisons. It does not use the amplitude of the integrated fluctuation.

On a starred free bond the nonlinear exceptional correction vanishes. The actual source reconstruction and (BA.18a) therefore give the concrete bound

\[
 \|V_{1,e}(V^{(1)}_{\square,e})^{-1}-I\|
 \le Cg_1|a_{1,e}|+
                C\epsilon_1(g_1)e^{-cR_{\rm next}}.
 \tag{BA.18b}
\]

Choose the fixed fraction in \(P_1=c\,\delta_1/g_1\) small enough that the first term is at most \(\delta_1/2\), and then the coupling small enough that the second is at most \(\delta_1/2\). Thus, with the same fixed hierarchy and a strict margin,

\[
  \|a_1\|_\infty<P_1
 \quad\Longrightarrow\quad
 \|V_1(V^{(1)}_{\square})^{-1}-I\|<2\delta_1
 \tag{BA.18}
\]

on every literal Q test footprint. The new coarse P2 restrictions are retained separately. The comparison must include every overlapping reference box, not just one box assigned to the bond.

This use of a smaller fixed fraction is safe even before sharp optimization of the margin. Obtaining a particular larger radius or the precise defect shell constants required by a later theorem requires that theorem's local-frame estimate.

For a broad \(P_1\to\infty\), \(g_1P_1\to0\), the source cluster construction is compatible with this comparison: the analytic fluctuation vertices remain inside their fixed physical-angle tube, and the fixed-coordinate excluded tails are Gaussian-small. The proof of locality and component factorization is unchanged. One must retain the resulting comparison normalization and its difference from the exact Q density. The tiny literal radius in the last row of the table does not support a near-unit Gaussian-tail argument.

## 7. Relation to companion results

The note flat_ordinary_innovation_gap proves the flat lower bound at arbitrary depth, using the four-dimensional curvature-averaging contraction and the fixed-L block gauge inequality. It supplies an independent flat check of (BA.14). By itself it does not control the nonflat constraint-force term. CMP99 (3.156)–(3.158) and the soft-gauge argument in §4 supply that additional input here.

The restored_source_energy_identity_kernel note identifies actual constrained Hessians, Schur restoration and the cancellation of first force terms on admitted restored charts. Its exact Schur identities are consistent with (BA.11), and they prevent dropping a hard-cutoff completion. Its residual-core energy comparison is not required to manufacture the present second ordinary gap, and does not replace the local coefficient construction in CMP116.

The first_step_precision_gap note proves a finite-range bare first precision at the local lift. The inherited second precision need not be finite range: the first constrained minimizing action has already been integrated classically. Its source generalized-walk family, rather than a false reuse of the first finite-range matrix, supplies the needed decay and native coefficient localization.

## 8. Discharged inputs and the remaining second-step application

On the two clean, fully P/Q-regular native steps the following inputs are now sourced or derived:

* the exact first analytic base, with its first determinant, Haar/coarea terms, vacuum term and coupling counterterm;
* the true second classical minimum and the constrained force cancellation;
* the native nonflat ordinary Gaussian gap, including the actual soft gauge;
* a local analytic fluctuation-action family with exact component identities;
* the strict native admission of the first analytic base throughout the actual second Q-domain, before any second R split;
* a buffered smooth-potential gap, and the precise distinction between a broad auxiliary comparison cutoff and the printed next R-good radius.

The following are not consequences of those facts alone:

* a raw-\(V_2\) compact coefficient family with all physical carrier/current footprints and compatible exceptional-bond reconstruction;
* a joint second integration of the nonsmooth old Q-core payload retaining its original Gaussian tail reserve;
* a proof that an arbitrary new outside-decoupled family preserves the old admission buffer and all local Q reference domains;
* the next source-density/finite-jet theorem, complementary P/Q histories, uniform depth, or the final Yang–Mills hierarchy.

Those are concrete application requirements. In particular the analytic base should no longer be treated as an unidentified old boundary functional; it is the explicitly constructed source action (BA.3). Its nonsmooth correction must continue to be carried separately.

## Mathematical sources

The mathematical references are:

* T. Bałaban, CMP 99 (1985), 389–434: printed pp.396–397, (3.35)–(3.38); pp.425–428, (3.147)–(3.158), especially the explicit positive-gap paragraph after (3.158); Theorems 3.12–3.15.
* T. Bałaban, CMP 109 (1987), 249–301: printed pp.260–264, (1.1)–(1.19), Theorem 3; pp.265–269, (2.1)–(2.15); p.298, the explicit localization deferral.
* T. Bałaban, CMP 116 (1988), 1–22: printed pp.2–7, (1.2)–(1.21); pp.9–11, Lemmas 1–2; pp.12–17, (2.1)–(2.24); pp.21–22, restoration of log Gaussian normalization and completion of the inductive proof.
* T. Bałaban, CMP 119 (1988), 243–285: printed pp.247–254, (1.8)–(1.30); pp.258–260, (2.23)–(2.28); pp.264–268, (3.1)–(3.16).
