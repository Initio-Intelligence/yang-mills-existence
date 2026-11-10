# Ambient local frames for the first moving-Q cutoff

This note uses the native definitions and budgets in [moving q reconstruction input analysis](moving_q_reconstruction_input_analysis.md) (MQ.1–MQ.22). It proves the additional local finite-box comparison and ambient guard construction. It is kept separate from the native input. The numbering MQ.23–MQ.37 continues that input note.

## 1. A common finite-box comparison, without extending its raw data globally

The native argument above is not by itself an ambient argument. In particular, the coefficients of a previously chosen fixed-geometric extension are bounded by \(C\gamma\), not by \(CgP_0\), on arbitrary real retained data. Moreover, activating a local Q reference must not introduce a global admission test. The following first-step local comparison supplies the additional fact needed for a local guard.

### Lemma MQ.1 — common primitive first-step coefficients

The global first minimum and the literal local minimum \(U_{1,\square}\) can be given Hermitian-log carrier families in the same reference \(Q^fV\) and the same averaged block gauge such that:

1. each family has a uniform weighted majorant \(C\gamma\) on its own local weak-curvature domain, and summed normalized raw derivative majorant \(Cg\);
2. whenever an entire carrier lies in the region where the global and local determining problems have identical primitive stencils and constraints, the two coefficients are identical;
3. every coefficient which can distinguish the problems at a tested bond e reaches the local problem's boundary collar. That collar is at distance at least \(cR_1\) from the tested set in CMP119 (1.19).

The local assertion needs only raw data on the local source determining box and a fixed primitive halo. It does not assume that those data extend to a globally admitted coarse field.

**Proof from the first-step local equations.** At \(k=1\), parameterize the exact constrained fiber near \(U_f=Q^fV\) by its physical, unscaled independent Lie variables a. The nonlinear constraint map has the form
\[
 \Xi(a)=\exp i\{C(V)a-h(V)D_V(C(V)a)\}\,U_f.
 \tag{MQ.23}
\]
Each exceptional equation is on its own coarse face and its two adjacent blocks; its paths cannot meet another coarse-face exceptional bond. Consequently the implicit exceptional solve and all its derivatives are finite-range local functions, not an inverse spanning the whole lattice. This is the concrete content of CMP119 p.249 and CMP109 p.267 used in AB.3–AB.6.

Substitute (MQ.23) into the *classical* Wilson action plus the actual averaged soft-gauge action. The resulting function \(\mathcal S(a;V)\) is a sum of finite-range analytic vertices. On a fixed small physical a-ball its derivative is
\[
 \nabla_a\mathcal S=J_f(V)+K_0(V)a+N_V(a),
 \quad N_V(0)=0,\quad DN_V(0)=0.
 \tag{MQ.24}
\]
The actual constraint-curvature contribution is in \(K_0\). The force has a local carrier norm \(\|J_f\|\le C\gamma\); the soft-gauge force at \(Q^fV\) is zero. The nonlinear coefficient rows have a convergent local analytic majorant
\[
 \|N(a)\|_\nu\le\frac{C\|a\|_\nu^2}{1-C\|a\|_\nu}.
 \tag{MQ.25}
\]
Here \(\|a\|_\nu=\sup_e\sum_Xe^{\nu n(X)}\|a_{e,X}\|\). A nonlinear vertex joins only a fixed number of neighboring roots; including its full fixed stencil makes the union of its input carriers connected and gives (MQ.25). Its constants are fixed at this one step.

For the finite local problem, keep precisely the fine determining values and coarse constraints of \(B_1(\square^{\sim4})\) in CMP119 (1.2). The former are the corresponding values of \(Q^fV\), and the latter are its exact coarse averages. The first-layer incidence is important. CMP119 p.255, (2.2), defines \(\Gamma_0=\Omega_1^c\) and \(\Gamma_1=\Omega_1^{(1)}\) for the point, bond and plaquette sets. On bonds this is the complementary index set, as independently confirmed by the integration over \(\Omega_1^*\) and the solve of every \(b_0(c)\), \(c\in\Omega_1^{(1)}\), on p.249. It is not a second application of incidence to the geometric complement. Thus crossing exceptional variables for incident coarse constraints remain available in this first-layer chart. The held-master interface in CF is a different situation.

Relative fine boundary variations are zero. The independent-coordinate solve and the classical vertices in the common interior are therefore exactly those of (MQ.23)–(MQ.24); boundary modifications stay in their actual fixed stencil collar. The gauge map is the same averaged block map on every common block. There is no comparison of two arbitrarily chosen gauge representatives.

The flat gap proof PG.1 applies to the local zero-extended variation: the held fine variations vanish, the incident coarse constraints are solved, and any remaining coarse constraint has zero variation because its full two-block stencil is outside the variable domain. The averaged gauge term is the same on variable blocks and zero on held internal blocks. Local coarse gauges and the fixed IMS argument then give a uniform gap for \(K_0\) in either problem on a sufficiently small fixed local curvature domain. This argument uses only a fixed halo of the actual local domain.

Apply the PR.1 buffered local-inverse construction using the same fixed partition and the same primitive local inverses wherever their full halos coincide. If desired, pad coordinates outside a finite problem with a fixed independent positive mass. Boundary flags are part of a coefficient's declared footprint. Local inverses and commutator coefficients are identical whenever that footprint cannot see the boundary difference. The ensuing common word construction gives
\[
 \|K_0^{-1}\|_\nu\le B
 \tag{MQ.26}
\]
and the stated interior coefficient identity, uniformly for both problems. This is the same local inverse consistency argument used in GM.1, now applied before any minimum is solved.

In the carrier Banach space, solve the actual local Euler equation by
\[
 a=-K_0^{-1}\{J_f+N(a)\}.
 \tag{MQ.27}
\]
Choose the fixed geometric ceiling so that the ball \(\|a\|_\nu\le2BC\gamma\) is inside the analytic chart and the map in (MQ.27) has Lipschitz constant less than one half. Equations (MQ.25)–(MQ.26) give this directly. Carrier multiplication unions supports at a common index. Thus the iteration preserves exact interior equality of all coefficients whose complete primitive footprints cannot distinguish the two domains. Its absolutely convergent limit has norm \(C\gamma\) and the same equality. Applying the local map in (MQ.23), or its small Hermitian logarithm, preserves these assertions. The real iteration stays in the real Lie algebra.

This is a coefficientwise majorant for this particular finite-range first-step Euler system. It does not assume an absolute sum over arbitrary internal indices of the earlier FC.7 bound. The PR inverse majorant and the local analytic multiplication estimate are the explicit inputs to this additional Banach-space proof.

At the physical endpoint, the solution is the actual constrained critical field. Source uniqueness of the first regular critical orbit, with the fixed averaged gauge, identifies it with \(U_1\) or with the literal \(U_{1,\square}\), respectively. The source local problem therefore has the same interior coefficients, not merely the same formal equation at a different gauge. One-coordinate native Cauchy and the explicit fixed source stencils give the current majorant as in (MQ.6). Finally a differing carrier must reach the boundary collar, and the source \(\square^{\sim2}\) versus \(\square^{\sim4}\) separation gives its \(cR_1\) distance. ∎

This lemma is specific to the first bare step, where (MQ.23) and the classical potential are genuinely finite range. It must not be asserted for a completed old action on the strength of a covariance decay estimate alone.

### An interior-stability proof of the comparison, independent of the local boundary chart

The consequence needed below can also be proved without assigning any carrier identity to the actual local problem at its boundary. This provides a separate check on the incidence issue.

Choose an auxiliary window H of ordinary independent coordinates, with its fixed primitive halo inside the guarded Q box and with the tested bond a distance \(cR_1\) from its boundary. Set the independent coordinates outside H equal to zero in the *global primitive formula* (MQ.23) and solve (MQ.27) for the remaining ones. Every affected exceptional equation is still solved by (MQ.23), including those in the fixed halo. This auxiliary problem is not declared to be the source local problem. Its Hessian is the principal restriction of the global primitive K0, its nonlinear vertices are the corresponding restrictions, and the PG gap and the Banach contraction just proved apply using only the guarded raw data. Its compact field \(U^H\) satisfies the exact coarse constraints on the entire common inner region.

The PR coefficients and the Picard coefficient construction are manifestly identical to the global ones on every full carrier inside H. Thus the globally clipped logarithm and the logarithm of \(U^H\) differ at the tested bond by \(C\gamma e^{-cR_1}\), whenever the guard makes those interior coefficient cutoffs equal one. This step compares common primitive-coordinate constructions, not two different boundary gauges.

The averaged-gauge matching in this comparison is exact. Write the actual group-valued averaged contour variable at an interior vertex x of a block centered at y as \(w_x=U(y,x)\), in the notation of CMP119 (1.5)–(1.7). A center-fixed gauge transformation changes the w variables independently, preserves the Wilson action and all coarse averages, and leaves its nonexceptional variation inside H whenever the vertex star and its fixed constraint halo lie there. The soft-gauge action is a sum of the corresponding one-variable class functions \(1-\operatorname{Re}\operatorname{tr}w_x\). Its only critical point in the fixed small identity neighborhood is \(w_x=I\). Consequently auxiliary stationarity forces the same averaged gauge as the chosen source representative at every vertex of the common inner blocks. This does not assert that the whole auxiliary boundary gauge is identity. No boundary gauge value is used beyond its \(C\gamma\) bound.

Now compare the exact auxiliary field \(U^H\) with the actual \(U_{1,\square}\). On a smaller inner window, both have the same prescribed coarse averages, the same local averaged gauge, and the same classical first-step Euler equations. Both are within \(C\gamma\) of \(Q^fV\) in these coordinates. No condition on their boundary charts is needed there. Write their ordinary interior independent coordinates as a and b. The source uniqueness and stationarity imply
\[
 [K_0+\mathcal E](a-b)=0
 \quad\hbox{on that inner window},\qquad
 \mathcal E=\int_0^1 DN(b+t(a-b))\,dt,
 \quad\|\mathcal E\|_{\rm row}\le C\gamma.
 \tag{MQ.27a}
\]
The operator has fixed range. Its inner principal block has gap at least \(\lambda/2\) for small fixed \(\gamma\). The discrepancy at the boundary is only required to be bounded by \(C\gamma\). Moving the fixed-stencil boundary contribution to the right side and applying the Dirichlet massive Green bound gives
\[
 |a_e-b_e|\le C\gamma e^{-c'R_1}.
 \tag{MQ.27b}
\]
The polynomial size of the boundary is absorbed by reducing the exponent. The local map (MQ.23) transfers this bound to the compact link logarithm.

The same estimate holds on a smaller fixed complex raw tube: the source analytic solutions remain \(C\gamma\), and the complex mean-value operator is a small perturbation of its positive real reference. Cauchy for the finitely many raw coordinates in the box costs at most a polynomial \(R_1^4\); the exterior global coefficients are handled by their summed current tail. This gives the normalized derivative form used below.

This alternative never compares the Euler equation of a coefficientwise clipped link field with the original equation. Such a clipped field need not satisfy the exact nonlinear coarse constraint. The intermediate \(U^H\) does satisfy it, by construction, and both fields in (MQ.27a) are actual critical fields on their common interior. Consequently no unproved correction of a clipped constraint defect is needed.

## 2. Local guards and an ambient comparison

Choose a fixed small geometric ceiling \(\gamma\) as in Lemma MQ.1. For every coefficient carrier choose the same smooth real gauge-invariant cutoff \(\eta_X\), depending only on the plaquettes in its full raw footprint, such that

* \(\eta_X=1\) when all these plaquettes obey a smaller ceiling \(\gamma/2\);
* \(\eta_X=0\) before any required native local input leaves the \(\gamma\) domain;
* its normalized summed derivative is bounded by \(Cg|X|/\gamma\).

Products of smooth functions of the squared plaquette defects supply these cutoffs. The PG local gap and all first primitive analytic conditions follow at the chosen small ceiling; no separate global spectral or regularity switch is introduced. Define
\[
 \Theta_{e,\mathrm{ext}}=\sum_X\eta_X\Theta_{e,X},
 \qquad U_{1,e}^{\mathrm{ext}}=e^{i\Theta_{e,\mathrm{ext}}}U_{f,e}.
 \tag{MQ.28}
\]
This is the local Hermitian extension of Section 4.4 of [local extension kernel](../A_support_and_normalization/local_extension_kernel.md), with the coefficient family of Lemma MQ.1 fixed consistently. It has global value budget \(C\gamma\), normalized current budget \(Cg\), and the same restriction family obtained by retaining only \(X\subset D\). Each cutoff derivative is retained explicitly. On actual admitted first-step data at small g all cutoffs equal one, so the reconstruction is unchanged.

For each original Q reference box choose a guard \(\eta_\square(V)\) on its full raw determining footprint and a fixed primitive halo. Set it equal to one below a ceiling \(\gamma/8\), and support it strictly below \(\gamma/4\). On its support the actual local minimum \(U_{1,\square}\) is defined in its larger native tube. Every coefficient whose complete footprint is in the common interior of this guarded box has \(\eta_X=1\), and Lemma MQ.1 identifies it exactly with the corresponding coefficient of that local minimum. The remaining coefficients of both families reach a distance \(cR_1\) from the tested bond. Consequently
\[
 \eta_\square>0\quad\Longrightarrow\quad
 \|\Log(U_{1,e}^{\mathrm{ext}}U_{1,\square,e}^{-1})\|
 \le C\gamma e^{-\nu R_1},
 \tag{MQ.29}
\]
with the summed normalized derivative bound \(Cg e^{-\nu'R_1}\). This holds with completely arbitrary real raw data outside the guard footprint. The unknown outside field does not enter the local native minimum, and every surviving extended coefficient there is bounded by its own local cutoff.

The same argument applies to \(U_1^{D,\mathrm{ext}}\). At a Q slot, its original defining reference box is already a distance \(cR_1\) buffer around the tested bond. Omitted carriers must traverse that buffer and any added halo. Equations (MQ.11)–(MQ.13) therefore give on the fixed outside polydisc
\[
 g^{-1}\|\Log(U_{1,e}^{\mathrm{ext}}(s)
                     (U_{1,e}^{D,\mathrm{ext}})^{-1})\|
 \le C\frac{\gamma}{g}e^{-\nu'(cR_1+\ell)}.
 \tag{MQ.30}
\]
There is no claim that \(\gamma/g\) is a polylogarithm. Instead use the actual source hierarchy \(R_1\asymp(\log g^{-2})^r\), \(r\ge2\). For sufficiently small g,
\[
 (\gamma/g)e^{-\nu'cR_1}
 \le P_0 e^{-\nu''R_1}
 \tag{MQ.31}
\]
for a smaller fixed positive \(\nu''\). Thus the original Q box itself pays the apparent \(g^{-1}\) loss. A logarithmic initial halo as in (MQ.14) is sufficient; alternatively one may use an ambient halo \(C\log(1/g)\), which is still \(O(R_1)\). Only Q defects receive either growing halo, as in (MQ.10a). Their full volume cost is \(O(R_1^4)\) per defect and is paid by \(e^{-cP^2}\).

It follows from (MQ.29)–(MQ.31) that whenever a guard is positive, the Q domain in either the global extended frame or its compact local D frame contains \(B_{3P/2}\) and is contained in \(B_{5P/2}\), for small g. The margins are strict. The fixed local guard, not D or the full retained field, decides whether that Q test is active.

## 3. A positive ambient one-slot cutoff with the correct native endpoint

On the actual global extended reconstruction, define
\[
 \rho_e^{\mathrm{ext}}(z,V)=\mathbf1_{|z|<3P}
  \prod_{\square\ni e}
  \left[1-\eta_\square(V)+\eta_\square(V)
   \mathbf1_{\{\|e^{igz}U_{1,e}^{\mathrm{ext}}
                       U_{1,\square,e}^{-1}-I\|<2gP\}}\right].
 \tag{MQ.32}
\]
The local minimum inside a term needs to be evaluated only where its guard is supported. This cutoff lies between zero and one, equals one on \(B_{3P/2}\), and vanishes outside \(B_{3P}\), on every real retained datum. On actual native data all guards are one and the outer \(3P\) cutoff is redundant, so (MQ.32) is the literal Q cutoff.

Expand a slot into the finite convex sum over subsets J of its original tests, with weights
\[
 w_J=\prod_{\square\in J}\eta_\square
       \prod_{\square\notin J}(1-\eta_\square).
 \tag{MQ.33}
\]
For J empty the domain is the fixed \(3P\) ball and no frame change is needed. For J nonempty the selected guarded intersection is contained in \(B_{5P/2}\). In the local frame \(U_1^{D,\mathrm{ext}}\), the shift (MQ.30) is at most a fixed small number, so the additional global \(3P\) cutoff is still redundant. The selected intersection is a real domain depending only on the corresponding Q boxes and D; it is fixed with respect to outside decouplers. It contains \(B_{3P/2}\) up to an arbitrarily small fixed margin adjustment, and its difference from the P ball is a true failed-cutoff species.

The guards themselves depend only on their fixed Q boxes and are not chosen from the total Mayer support or a global admission event. The common coefficient restriction and the additive mixed enlargement (MQ.10a) therefore preserve the component identity. Physical raw variation still changes the guards and the real domains. Their product-rule and surface currents must be kept; the guard-current term is itself supported outside the P ball because every branch agrees there.

This supplies the missing **ambient frame and cutoff input** for the first-step contour construction. Positivity follows before any expansion, since the complete extended Gaussian/interaction density is positive and (MQ.32) contains the P ball. The normalizer and the reconstruction are the same ones used by that positive kernel. The surrounding cluster proof, its marked root, and its exact separate current records remain the work of the moving-Q theorem; no such output estimate was assumed in Lemma MQ.1 or in the local guard comparison.

## 4. One compatible background and reconstruction registry

The coefficient family fixed in Lemma MQ.1 can be chosen together with the complete first-step reconstruction, rather than identified after two unrelated extensions have been made. Let its zero-fluctuation relative logarithm be \(\Theta_{0,e}=\Theta_e(0,V)\), and let
\[
 \Delta\Theta_e(z,V)=\Theta_{\mathrm{rec},e}(z,V)
                         -\Theta_{\mathrm{rec},e}(0,V).
 \tag{MQ.34}
\]
At the native endpoint, \(\Theta_{\mathrm{rec}}(0,V)=\Theta_0\). Construct the supported family of \(\Delta\Theta\) from this difference itself, using the same local maps and background registry. It vanishes coefficientwise at z=0. In particular, no cancellation between two separately extended zero-fluctuation values is required. The exact compact gauge maps and the original coarea coordinate map remain in this reconstruction.

There is an explicit force majorant for the new Euler family. Every Picard tree for (MQ.27) has at least one leaf \(J_f(Q^fV)\). Distinguish one such leaf and bound the remaining force leaves by \(C\gamma\). The convergent contraction majorant, with the leaf count included, is still bounded by a fixed constant. Local products and the PR inverse retain the entire footprint of the distinguished leaf. Cauchy–Schwarz in that footprint, followed by a fixed reduction of the carrier rate, therefore gives nonnegative deterministic coefficients with
\[
 |\Theta_{0,e,X}|
 \le c^{(0)}_{e,X}
       \left(\sum_{f\in\operatorname{foot}X}|J_f(Q^fV)|^2\right)^{1/2},
 \qquad
 \sup_e\sum_X e^{\nu n(X)}c^{(0)}_{e,X}\le C.
 \tag{MQ.35}
\]
Equivalently, the distinguished-leaf majorant is the first source derivative of the convergent scalar analytic majorant for the fixed point; its inverse factor is bounded by the contraction reserve. It introduces no inverse power of g or of the force. The local composition (MQ.23) has no constant relative-log term, so it preserves this estimate.

The difference in (MQ.34) has at least one fluctuation leaf \(g z_i\). Apply the same argument, or integrate its analytic derivative along tz, \(0\le t\le1\), on the fixed small physical tube \(g|z_i|\le CgP\). The remaining background and fluctuation factors are uniformly small there. After the same fixed support collars and rate reduction,
\[
 |\Delta\Theta_{e,X}(z,V)|
 \le c^{(z)}_{e,X}\,g
       \left(\sum_{i\in\operatorname{foot}X}|z_i|^2\right)^{1/2},
 \qquad
 \sup_e\sum_X e^{\nu n(X)}c^{(z)}_{e,X}\le C.
 \tag{MQ.36}
\]
The coefficients include all raw determining and fluctuation footprints. These are the two terms of the local-energy majorant (4.11) of [local extension kernel](../A_support_and_normalization/local_extension_kernel.md); they are preserved by the present force-resolved coefficient construction. They are not an assumed bound on a conditional scalar output.

Extend the background coefficients by the \(\eta_X\) in (MQ.28), and extend the difference coefficients by the same class of local admissibility cutoffs, equal to one on every active first-step datum. Define the one common ambient reconstruction by
\[
 \chi_{e,\mathrm{ext}}(z,V)
  =\exp i\{\Theta_{0,e,\mathrm{ext}}(V)
                     +\Delta\Theta_{e,\mathrm{ext}}(z,V)\}
                       (Q^fV)_e.
 \tag{MQ.37}
\]
Its zero-fluctuation value is exactly the \(U_{1,e}^{\mathrm{ext}}\) used in (MQ.29)–(MQ.32). Each summand is Hermitian on real data, so the field is compact, and (MQ.35)–(MQ.36) remain valid on every surviving local term. The corresponding positive extended density is chosen once with this registry as permitted by the GM construction; all native Gaussian, interaction, Haar and coarea factors agree with the original kernel on its admitted domain. This is a concrete compatible off-domain choice, not a claim that every previously arbitrary off-domain coefficient choice would coincide. Every microscopic mark is evaluated on (MQ.37), and all product-rule derivatives of its retained cutoffs remain in the current certificate.
