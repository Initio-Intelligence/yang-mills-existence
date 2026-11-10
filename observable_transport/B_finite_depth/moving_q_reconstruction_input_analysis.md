# Input analysis for local frames in the actual first moving-Q cutoff

This note verifies a reconstruction input needed to treat the moving first-step Q cutoffs. Its domain is the original homogeneous first Wilson step with no inherited activities, on admitted weak-curvature coarse data and their specified native analytic buffer. It proves a local compact reference frame, its restriction consistency, an exponentially small outside-decoupler shift, and summed normalized raw currents. It does not claim that the frame is a new minimum, nor does it discard the Jacobian of the subsequent change of variables.

The coefficient construction is taken from the already proved source fixed-point family, not from an assumption that a marked output has localized support. The distinction between FC.1's original weak-link chart and the subsequent weak-curvature construction is made explicit below.

## 1. The genuine first-step primitive

Let \(g=g_0\), let \(P\) be the literal first free-coordinate radius, and let \(P_0\ge P\) denote a fixed source multiple of the first background regularity factor. In this first step

\[
 \varepsilon(V)\le CgP_0,
 \qquad P_0/P\le C_{\rm source},\qquad
 gP_0\longrightarrow0.
 \tag{MQ.1}
\]

All constants may depend on the fixed blocking and gauge conventions. The first two running couplings are comparable; write \(s_1=(1+\beta_1)^{-1/2}\asymp g\) for the physical size of a normalized raw coarse-link direction.

Use the actual source representative of the first minimum \(U_1(V)\), and the compact local face lift \(U_f(V)=Q^fV\), CMP119 (1.3). On the admitted first-step domain their relative field is uniformly near the identity, so define, on positively oriented fine links,

\[
 U_{1,e}(V)=e^{i\Theta_e(V)}U_{f,e}(V),
 \qquad
 \Theta_e=\frac1i\Log\bigl(U_{1,e}U_{f,e}^{-1}\bigr).
 \tag{MQ.2}
\]

The branch is the fixed small logarithm. Reverse links are defined by inversion, not by independently truncating a second logarithm. On real data \(\Theta_e\) is Hermitian and lies in the source Lie algebra.

The compact representative in (MQ.2) includes the actual block gauge map. In particular, if an intermediate variational construction uses a different block gauge, the averaged gauge can be imposed by its exact local contour variables: the group mean \(U(y,x)\) in CMP109 (0.11) transforms covariantly at its two endpoints, so a center-fixed gauge sets these variables to the identity. This map is analytic on the native small-field domain, is compact on real data, and uses only one fixed L-block. Its footprint and derivatives are included in \(\Theta\). Gauge invariance of a scalar is not used to change the underlying reconstruction.

## 2. Which previously proved carrier theorem applies

FC.1 alone is insufficient: [flat chart variational carriers](../A_support_and_normalization/flat_chart_variational_carriers.md) initially assumes a common global weak-link logarithm. That assumption must not be inferred from small plaquettes.

There are two verified first-step routes that avoid it.

1. [local extension kernel](../A_support_and_normalization/local_extension_kernel.md), Sections 1–3 and 4.4, starts from the literal local lift \(Q^fV\). Its coarse averages are exact, its Wilson force is bounded by the local coarse plaquette defects, and its internal averaged-gauge force is zero. At the first step all scale ratios are fixed powers of L. The source force-containing fixed point therefore gives a relative correction of order \(\varepsilon(V)\), uniformly on the enlarged decoupler domain. The local-reference gap is proved in [first step precision gap](../A_support_and_normalization/first_step_precision_gap.md), and its raw-supported resolvents in PR.1. Local coarse gauges are used only to bound these local coefficients, never to define a long-path raw coordinate map.
2. The homogeneous alternative in [local bundle reference](../A_support_and_normalization/local_bundle_reference.md), BR.1 and Section 9, gives a genuinely raw-local regular reference on arbitrary sufficiently weak-curvature data, with a local native complex identification. Its force and average mismatch are local and of order \(\varepsilon\). The source equations CMP102 (111)–(121) and the common CMP116 decouplers then give the same actual homogeneous minimum. This extends FC.1.

For the present first-step statement, route 1 suffices. Route 2 confirms that the use of a weak-curvature raw domain is substantive and not a silent global-gauge assumption. Neither route proves a completed old-component reconstruction budget.

The relevant source localization is the fundamental-theorem expansion in CMP116 (1.9)–(1.18). One coefficient is kept for each connected fundamental-theorem carrier; internal propagator walk and fixed-point indices remain within that analytic coefficient. An unsupported absolute sum over those finer internal indices is not used.

## 3. Quantitative Hermitian carrier and current budgets

Let \(S_e\) contain the fixed raw footprint of the local lift, the output link, and its block gauge map. The common source construction gives

\[
 \Theta_e(V)=\sum_{X\supset S_e}\Theta_{e,X}(V_X),
 \tag{MQ.3}
\]

where every declared physical carrier X is connected. On real data every coefficient is Hermitian. This follows by using the real fundamental-theorem formula: at real decouplers the source equations and the exact compact gauge reconstruction preserve the real Lie algebra; differentiating and integrating that real logarithm preserves Hermiticity. Complex Cauchy is used only for its majorant.

There are fixed positive \(\nu_0\) and C such that, with \(n(X)=|X|+t(X)\),

\[
 \sup_e\sum_Xe^{\nu_0n(X)}\|\Theta_{e,X}(V_X)\|
 \le CgP_0
 \tag{MQ.4}
\]

on the actual first-step weak-curvature domain. This is the needed small *value* budget, not merely an O(1) carrier norm.

To see the scale in (MQ.4), the source fixed point has its actual force-linear input and vanishes when that force vanishes; its uniform bound on the original enlarged decoupler polydisc is \(C_R\varepsilon(V)\). A coefficient with n differentiated source cubes is therefore bounded by

\[
 C_R\varepsilon(V)(R-1)^{-n}.
 \tag{MQ.5}
\]

Connected-set entropy and the fixed raw footprint per source cube are paid exactly as in FC.7–FC.8. Applying the logarithm and block gauge map on their fixed small analytic domain does not change the linear order of this bound. This proves (MQ.4), using (MQ.1). The force-resolved argument is important: applying an O(1) bound on a fixed geometric tube would not produce the factor \(gP_0\).

For normalized raw directions \(D_d\), a possibly smaller fixed rate \(\nu_1>0\) gives

\[
 \sup_e\sum_X e^{\nu_1n(X)}
       \sum_{d\in\operatorname{foot}X}
       \|D_d\Theta_{e,X}(V_X)\|
 \le Cg.
 \tag{MQ.6}
\]

Here is the derivative argument, rather than an inference from (MQ.4). Around a real admitted field there is a fixed physical one-coordinate analytic radius \(r_*>0\) inside the native geometric tube. On that larger tube (MQ.5) has a fixed geometric bound \(C\gamma(R-1)^{-n}\). Cauchy in that coordinate gives a physical derivative bounded by \(C\gamma/r_*\) times the same carrier majorant. Multiplication by the normalized step \(s_1\asymp g\) gives \(Cg\). The number of raw directions in a carrier is at most a fixed multiple of \(|X|\); spending a strict part of the positive carrier rate sums it. This is (MQ.6).

For weak-curvature fields the one-coordinate analytic radius is justified either by the first-step local-gauge coefficient proof or by BR's local Kato comparison. It is not obtained by selecting a field-dependent global axial gauge. Fixed real gauges used on a local proof patch stay fixed while taking the Cauchy circle.

The same argument proves a version of (MQ.6) for any fixed number of required raw derivatives, with its corresponding factorial and spare rate. Only the first summed current is needed here.

## 4. A compact, local and restriction-consistent frame

Fix the coefficient family (MQ.3) once. For a union D of physical blocks, and an output link with \(S_e\subset D\), set

\[
 \Theta_e^D=\sum_{X\subset D}\Theta_{e,X},
 \qquad U_{1,e}^D=e^{i\Theta_e^D}U_{f,e}.
 \tag{MQ.7}
\]

The sums converge absolutely. On real data \(U_1^D\) is compact. It depends only on raw variables in D. If \(D\) has separated components, every surviving connected carrier belongs to one component; the value at e is exactly the value obtained by applying the same restriction rule to its component. If two restrictions agree on a carrier, that coefficient is unchanged. Thus the family is restriction-consistent at the level actually required for component localization.

The family is **not** asserted to equal a variational minimum solved separately on D. It need not satisfy the prescribed block averages. It is a compact coordinate frame. This distinction does not affect either its locality or its use in the Q test.

If \(\operatorname{dist}(S_e,D^c)\ge\ell\), every omitted connected carrier has \(n(X)\ge c\ell\). Equations (MQ.4)–(MQ.6), with rate slack, give

\[
 \|\Theta_e-\Theta_e^D\|\le CgP_0e^{-\nu\ell},
 \qquad
 \sum_d\|D_d(\Theta_e-\Theta_e^D)\|
 \le Cg e^{-\nu\ell}.
 \tag{MQ.8}
\]

The local reference factor in (MQ.2) has normalized derivative O(g), and both logarithms are uniformly small. The analytic BCH map consequently gives the same bounds for the relative link logarithm:

\[
 \left\|g^{-1}\Log(U_{1,e}(U_{1,e}^D)^{-1})\right\|
 \le CP_0e^{-\nu\ell},
 \qquad
 \sum_d\left\|D_d\left[g^{-1}\Log(U_{1,e}(U_{1,e}^D)^{-1})\right]\right\|
 \le Ce^{-\nu\ell}.
 \tag{MQ.9}
\]

Here and below constants absorb the harmless factor i in a Hermitian logarithm. Couplings and all grid/halo choices are specified under the raw directions.

## 5. A fixed outside grid and its enlarged polydisc

Choose an outside-decoupler radius \(R_o>1\) once, above the fixed combinatorial entropy needed later. Choose a fixed coarse cube side m sufficiently large compared with \(\log R_o/\nu\). This grid does not grow with g or P.

Let I be the initial support of the particular cutoff-defect group, including every raw Q-reference box used by those tests and their defining local footprints. Let D be the union of m-grid cubes meeting its \(\ell\)-neighborhood, with any further fixed lift/gauge collar included. This enlargement is additive under unions. The initial halo \(\ell\), rather than the outside grid m, will grow with \(P_0\).

In a mixed Mayer application the enlargement is instead explicitly species-dependent:
\[
 D=D_m(I_{\rm regular})\;\cup\!
       \bigcup_{e\in S_Q}D_\ell(Q\!\operatorname{foot}_e).
 \tag{MQ.10a}
\]
Only genuine Q-defect boxes receive the growing halo; ordinary interaction and marked-root supports retain the fixed m enlargement. This rule is still additive and restriction-consistent. Assigning the \(\ell\)-halo to every ordinary carrier would charge \(e^{\kappa\ell^4|I_{\rm regular}|}\) without a tail reserve and would not follow from the fixed primitive decay. All bounds below at a Q slot use its own buffered Q box contained in (MQ.10a).

For each omitted coefficient let \(O_D(X)\) be the m-cubes outside D met by X, and set

\[
 \Delta\Theta_e^D(s)=
 \sum_{X\not\subset D}
  \left(\prod_{\Delta\in O_D(X)}s_\Delta\right)
  \Theta_{e,X},
 \qquad
 U_{1,e}(s)=e^{i[\Theta_e^D+\Delta\Theta_e^D(s)]}U_{f,e}.
 \tag{MQ.10}
\]

The connected-set cube bound proved in GM.2 is

\[
 |O_D(X)|\le a_4(1+|X|/m).
 \tag{MQ.11}
\]

Thus on \(|s_\Delta|\le R_o\), the monomial costs at most
\(R_o^{a_4}\exp[(a_4\log R_o/m)|X|]\). Fix m so this consumes only a prescribed fraction of the remaining carrier rate. Normal convergence, (MQ.8), and the same coefficient-current sum then imply

\[
 \sup_{|s|\le R_o}
  \|g^{-1}\Log(U_{1,e}(s)(U_{1,e}^D)^{-1})\|
 \le CP_0e^{-\nu'\ell},
 \tag{MQ.12}
\]

\[
 \sup_{|s|\le R_o}\sum_d
  \left\|D_d\left[g^{-1}\Log(U_{1,e}(s)(U_{1,e}^D)^{-1})\right]\right\|
 \le Ce^{-\nu'\ell}.
 \tag{MQ.13}
\]

The physical endpoint is exact: \(U_1(1)=U_1\), and \(U_1(0)=U_1^D\). For real s the field is compact; for complex s it is the stated analytic continuation. When parameters outside a union are zero, every surviving coefficient lies in that union and its root component. Because the restriction coefficients were fixed before choosing I and D, disconnected components agree with independently calculated component families.

No stationary-point assertion at complex s is made. In a fluctuation density, the already critical-cancelled complete normal form must be continued in compatible coordinates. Inserting \(U_1(s)\) into the original Wilson action and deleting a new linear force would be invalid.

Choose, for a fixed small \(a>0\),

\[
 \ell\ge\frac1{\nu'}\log\frac{CP_0}{a},
 \tag{MQ.14}
\]

rounding only the initial halo to the fixed grid. Then the normalized relative shift in (MQ.12) is at most a. Every outside-grid and carrier-rate constant remains independent of g. The cost of enlarging the defect footprint is explicit, at most \(C(\ell+m)^4|I|\) in this crude bound; the sharper source Q-box size gives \(C(R_1+\ell+m)^4\) per defect. It is charged to that defect's failed-cutoff reserve. Ordinary supports in (MQ.10a) pay only their fixed enlargement.

## 6. Comparison with the actual local Q references

For a Q test cube \(\square\) and a starred bond e in its tested interior, let \(U_{1,\square}(V)\) be the literal local source reference in CMP119 (1.2), (1.8), (1.19). Its complete raw defining box is included in I. CMP119 p.250, immediately after (1.19), gives in the common source gauge

\[
 \|U_{1,e}U_{1,\square,e}^{-1}-I\|
 \le C\varepsilon_1 e^{-cLM_2R_1}.
 \tag{MQ.15}
\]

This is an actual global/local minimum comparison, not an inference from covariance decay. The analytic localized map and its exponential property are identified again on p.251, (1.21), by reference to CMP102 (190).

For completeness, its summed normalized raw derivative has a compatible exponentially small bound. For raw coordinates in the local reference box and a fixed halo, use the source complex buffer and Cauchy on (MQ.15), replacing \(\varepsilon_1\) by the fixed geometric ceiling on that circle. There are only \(O(R_1^4)\) such coordinates. For coordinates outside that box, the local reference has zero derivative and the common global carrier family (MQ.6) gives the required distance tail. The polynomial count is absorbed in a smaller exponential. Hence

\[
 \sum_d\left\|D_d\left[g^{-1}
   \Log(U_{1,e}U_{1,\square,e}^{-1})\right]\right\|
 \le C e^{-c'R_1}.
 \tag{MQ.16}
\]

Combining (MQ.9), (MQ.15) and the first-step coupling comparison gives

\[
 H_{e,\square}:=U_{1,e}^D U_{1,\square,e}^{-1}
 \quad\hbox{compact and raw-local in D},
\]

\[
 \|g^{-1}\Log H_{e,\square}\|
 \le CP_0(e^{-\nu'\ell}+e^{-cR_1})\le 2a,
 \tag{MQ.17}
\]

for small g after (MQ.14), and

\[
 \sum_d\|D_d[g^{-1}\Log H_{e,\square}]\|
 \le C(e^{-\nu'\ell}+e^{-c'R_1}).
 \tag{MQ.18}
\]

If a bond belongs to several original Q tests, keep every corresponding \(H_{e,\square}\). The number of such tests at a bond is fixed by the source covering convention.

## 7. The Q domain in this frame

On an independent starred bond the original reconstruction is exactly
\(U_e=e^{igA_e}U_{1,e}\), since C preserves that coordinate and the nonlinear correction acts only at exceptional bonds. Write instead

\[
 U_e=e^{igB_e}U_{1,e}^D.
 \tag{MQ.19}
\]

At the real physical endpoint this is an exact local Lie-coordinate change. The literal Q restriction becomes the intersection of the original tests

\[
 \|e^{igB_e}H_{e,\square}-I\|<2gP.
 \tag{MQ.20}
\]

It depends on raw variables in D only, and does not depend on the outside decouplers in (MQ.10). No test is replaced by a different threshold.

By (MQ.17), for all sufficiently small g,

\[
 \{|B_e|\le 3P/2\}
 \subset \bigcap_{\square\ni e}\{\text{(MQ.20)}\}
 \subset\{|B_e|<3P\}.
 \tag{MQ.21}
\]

For the first inclusion use \(\|e^{igB}-I\|\le g|B|\) and \(\|H-I\|\le 2ag\). For the second use the triangle inequality, then the small principal logarithm; in the operator norm its exact radius is controlled by the corresponding arcsine. The errors \(O(g^2P^3)+O(a)\) are smaller than the available fixed P margin. The same conclusion holds for all original test intersections.

For complex outside parameters, the inverse coordinate change is

\[
 A_e(s;B)=\frac1{ig}\Log\bigl(e^{igB_e}
           U_{1,e}^D U_{1,e}(s)^{-1}\bigr).
 \tag{MQ.22}
\]

On the real B domain (MQ.21), the shift (MQ.12) keeps A(s;B) in a fixed enlarged analytic free-coordinate tube, for example 4P, uniformly on the fixed outside polydisc. The BCH derivative with respect to B is the identity plus \(O(ga)\), so the local coordinate Jacobian is nonsingular on that tube and has its analytic logarithm. It must be retained, together with the original exceptional-bond and Haar factors. Equations (MQ.13) and (MQ.18) give the summed normalized raw current budget for this change of frame and for the centers of its fixed local domain.

## 8. Conclusion and remaining obligations

The requested frame input is established for the actual first homogeneous Wilson step:

* it is real compact and genuinely raw-local;
* its restriction family has exact component consistency;
* its normalized difference from the actual minimum is \(CP_0e^{-\nu\ell}\), including a fixed enlarged outside-decoupler polydisc;
* its summed normalized raw derivative tail is controlled by a fixed positive carrier rate;
* its Q-domain is the original domain in new coordinates and satisfies (MQ.21).

The weak-curvature claim relies on the actual local-lift/force construction and, independently, BR's admitted homogeneous bundle reference. It is not a reuse of FC.1 outside its original weak-link hypothesis.

This input analysis does not complete the moving-cutoff cluster theorem. That theorem must keep the exact Jacobian of (MQ.22), the complete critical-cancelled normal form and its normalizer, the fixed real domain (MQ.20), and the explicit raw domain-current contribution. The growing initial halo must be charged to the failed-cutoff reserve. No inherited completed B term or changed source geometry is covered simply by the first-step construction.
