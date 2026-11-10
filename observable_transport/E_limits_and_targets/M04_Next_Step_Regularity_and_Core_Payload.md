# The next-step regularity gate and a retained Q-core payload

## 1. Result and precise boundary

The first R-averaged theorem gives an actual small correction
\[
 \delta E(V)=\log Z_Q(V)-\log Z_P(V)
\]
with connected physical carriers and finite first raw currents. It does **not** follow that this correction belongs to the holomorphic effective-action class required by an unchanged later analytic RG step.

This note proves three concrete statements.

1. At the flat retained field, the actual first-Q partition function has an explicit one-sided shape derivative. If two local comparison minima at one overlapping slot have different first responses in one raw direction, the logarithmic density correction has a nonzero cusp in that direction. The exact source response condition is reduced below to the actual finite constrained matrices. A nonzero matrix entry for the literal source boxes has **not** been proved here; it is not inferred merely from their distinct boundaries.
2. The first correction has a stronger representation than an unspecified Lipschitz function on each long carrier. Its real nonsmooth domain can be kept on the union of the original Q boxes for each defect, independently of all analytic connector supports. This is an exact first-step integral representation, with the same Gaussian reserve and carrier estimate as QC/RA.
3. The resulting physical density has an exact positive pushforward through one further group-averaging step while retaining that integral. There is also a local integral lemma: after the next R sum, keeping its Q tests whole on the old core freezes the old real domain and these new tests simultaneously. The analytic density can then be localized without applying Stokes to a nonsmooth old factor. Its explicit next-step density, admission and reserve hypotheses are stated below; a complete source application is not asserted.

The first-step source, coupling, cutoff and basis conventions are unchanged. The discussion is on the actual native P/Q-regular branch unless an ambient guard branch is explicitly mentioned.

## 2. Literal overlapping source tests

CMP119 p.246, (1.2), defines a local comparison minimum
\[
 U_{1,\square}(V)
 =U\bigl(B_1(\square^{\sim4}),\mathcal M^\cdot(Q^fV)\bigr).
 \tag{NP.1}
\]
The partition cubes are disjoint, but the tests in p.247, (1.8), run over starred bonds of \((\square^{\sim2})^*\). Those enlarged test stencils overlap. A nonexceptional bond in the overlap can therefore have at least two factors using different four-layer determining boxes. The number of factors per bond is fixed by the source geometry; it is not necessarily one. The source's incidence convention and the exclusion of the exceptional bonds are the same ones verified in AB and MQ.

At \(V=I\), every global and local comparison minimum is I. All Q factors at a slot therefore have the same real domain
\[
 \mathcal B_g=\{z:\|e^{igz}-I\|<2gP\}
 \tag{NP.2}
\]
on the principal small logarithm chart. For the operator norm this is the Lie-algebra norm ball of radius \(2g^{-1}\arcsin(gP)\). It contains \(B_P\), and has radius asymptotic to \(2P\). Its finite perimeter and the first shell estimates were proved in QS; they do not imply higher differentiability of an intersection.

Let \(V(t)\) be a real analytic raw-link path through I, inside the native buffer. Put
\[
 M_{e,\square}(t)
  =U_{1,e}(V(t))U_{1,\square,e}(V(t))^{-1}.
\]
The one-test domain in the global free coordinate is the image of \(\mathcal B_g\) under
\[
 T_{e,\square,t}(z)
  ={1\over ig}\Log\bigl(e^{igz}M_{e,\square}(t)^{-1}\bigr).
 \tag{NP.3}
\]
Write \(v_{e,\square}(z)=\partial_tT_{e,\square,t}(z)|_{t=0}\). On the reduced boundary of \(\mathcal B_g\), let n be its outward unit normal and define
\[
 w_e(z)=\max_{\square\ni e}n(z)\cdot v_{e,\square}(z)
               -\min_{\square\ni e}n(z)\cdot v_{e,\square}(z)\ge0.
 \tag{NP.4}
\]
This is the width of the normal velocities, not their absolute size. A common change of global frame adds the same velocity to every test and cancels from the width.

## 3. An actual flat-point regularity theorem

Work first at a fixed finite volume. The complete first normal-form density \(D_{V(t)}(z)\) is real analytic near t=0 on the compact enlarged free-coordinate domain. It is strictly positive on real data. No Haar, coarea, gauge or action factor is discarded in the following statement.

Let \(Z_Q(0)>0\), and define the unnormalized boundary marginal
\[
 f_e(z_e)
  =\int_{\prod_{i\ne e}\mathcal B_g}
                   D_I(z)\,\prod_{i\ne e}dz_i.
 \tag{NP.5}
\]
It is continuous and strictly positive on the one-slot boundary. The integral includes all other free variables with their actual flat Q cutoffs.

### Theorem NP.1 — one-sided derivative and cusp criterion

The actual density correction obeys
\[
 \lim_{t\downarrow0}
 {\delta E(V(t))+\delta E(V(-t))-2\delta E(I)\over t}
 =-{1\over Z_Q(0)}
       \sum_e\int_{\partial^*\mathcal B_g} f_e(z)w_e(z)\,dS(z).
 \tag{NP.6}
\]
Every term on the right is nonnegative before the displayed minus sign. In particular, a positive-width surface patch at one slot implies that \(\delta E\) is not differentiable along this raw path. Its small coefficient does not make the cusp analytic.

**Proof.** On a regular patch of the common boundary at t=0, use inward/outward normal coordinates. The boundary of one moving test has signed displacement
\(t\,n\cdot v_{e,\square}+O(t^2)\). For t positive the intersection takes the minimum of those displacements. For t negative it takes their maximum. Thus the sum of the two first-order displacements is
\(-|t|w_e\). The thin-shell estimate provides an integrable dominating bound. Approximation by regular patches, or the finite-perimeter transport formula, proves the same expression on the reduced boundary; the norm and intersection corners cause no extra first-order term.

At distinct slots, the event of lying in both moving shells has volume O(t squared). The density is smooth on the compact domain, so the first-order product-domain change is the sum of its one-slot boundary terms with marginals (NP.5). The change of the density itself has an ordinary two-sided derivative. Its odd first-order term cancels in the symmetric difference; density-change times shell-change is second order. This proves the corresponding formula for \(Z_Q\).

The fixed-P integral \(Z_P(V(t))\) is analytic near t=0 and positive there. Expanding the logarithm of the positive \(Z_Q\) gives the factor \(Z_Q(0)^{-1}\); the symmetric linear term of \(\log Z_P\) is zero. This proves (NP.6). Strict positivity of (NP.5) rules out cancellation between different slots. ∎

For the small group ball, a difference between two infinitesimal center translations gives positive width on a surface patch whenever that Lie-algebra difference is nonzero. One way to check this is to take a radial boundary point aligned with that difference: the small group norm increases strictly in that radial direction. A small regular patch has the same strict sign. Equivalently, a nonzero right-translation vector field cannot be tangent to every boundary point of a sufficiently small proper identity ball. This argument uses translations, not conjugations, which would preserve the group norm.

Consequently a sufficient actual-source condition is
\[
 \partial_tU_{1,\square_1,e}(V(t))|_0
 \ne\partial_tU_{1,\square_2,e}(V(t))|_0
 \tag{NP.7}
\]
for two literal overlapping tests. The common global-minimum derivative drops out. The comparison estimate (1.19) makes such a difference small, if present; it does not make it zero.

The theorem is an actual-source regularity statement even before (NP.7) is settled: it gives the exact directional obstruction and its sign. This note does **not** claim that a particular pair of source boxes has already been shown to satisfy (NP.7).

## 4. The precise source matrix test, and what is not inferred

At flat data use the actual independent-coordinate matrix from AB:
\[
 K=C^*(d^*d+\tau_{\rm av}^*\tau_{\rm av})C.
 \tag{NP.8}
\]
Here C eliminates the literal distinguished bonds and retains the other coordinates; \(\tau_{\rm av}\) is the source averaged soft gauge, not a replacement gauge. The first-layer local incidence permits zero extension of local independent variations, as checked in the ambient MQ proof.

For a local determining box H, use the **actual** local constrained chart, held collar, action sum and averaged gauge of the source problem (NP.1). Write its classical function as \(\mathcal S_H(a;V)\), and set
\[
 K_H=\partial_a^2\mathcal S_H(0;I),\qquad
 J_Hv=\partial_V\partial_a\mathcal S_H(0;I)[v].
 \tag{NP.8a}
\]
These matrices are not defined by taking an arbitrary principal submatrix of (NP.8). If \(C_H\) denotes the derivative of this actual local chart and \(\mathscr H_H\) its full fine-link classical Hessian, including the literal boundary and gauge restrictions, then \(K_H=C_H^*\mathscr H_H C_H\). The actual reference lift gives the corresponding mixed force. In the ordinary first-layer zero-extension realization checked in MQ, this is \(J_H=C_H^*d^*d Q^f_H\), with all action terms incident to the variable set retained; the averaged-gauge term vanishes because \(\tau Q^f_Hv=0\). If a different local boundary chart is used, (NP.8a), rather than an inferred principal compression, is the definition to use.

Differentiating the actual constrained Euler equation at I gives exactly
\[
 a'_H(v)=-K_H^{-1}J_Hv.
 \tag{NP.9}
\]
The constrained curvature-force correction itself is zero at the flat point. On a nonexceptional tested bond in the common interior,
\[
 \partial_tU_{H,e}(V(t))|_0
 =i\left[(Q^f_Hv)_e+(C_Ha'_H(v))_e\right].
 \tag{NP.10}
\]
The unscaled physical angle convention is used in (NP.9)–(NP.10); a normalized raw direction simply multiplies v by its prescribed coupling scale.

Equations (NP.8)–(NP.10) reduce (NP.7) to an explicit finite matrix comparison with no unspecified continuum limit. A variation outside one defining box is exactly invisible to that local reference. To prove the cusp by that route, one must still exhibit a nonzero row of the other map
\[
 e_e^*K_H^{-1}J_H
 \tag{NP.11}
\]
on a variation supported in the difference of the boxes. In the verified ordinary first-layer realization this is the explicit row \(e_e^*K_H^{-1}C_H^*d^*dQ^f_H\). A gap and an exponential upper bound do not prove that entry is nonzero. Different boundary Green matrices likewise do not by themselves prove it after composition with the constrained force map. No diagonal-dominance or scalar maximum-principle property of the Yang–Mills precision is assumed here.

Thus the established first-current bounds justify Lipschitz regularity and (NP.6). They do not provide the raw holomorphy needed to put \(\delta E\) into the next analytic effective-action class. Proving equality of the relevant rows would remove this particular first-order cusp in that direction, but would not by itself prove higher analyticity of all intersections.

## 5. Exact local Gaussian illustration of the regularity issue

The following model is solely a finite-dimensional regularity example. It is not substituted for the actual Yang–Mills matrix or declared to realize (NP.7).

Let \(f_\lambda(x)=\sqrt{\lambda/(2\pi)}e^{-\lambda x^2/2}\), \(\lambda>0\), and take two moving scalar cutoffs
\[
 D_t=\{|x-t|<R\}\cap\{|x+t|<R\}
     =(-R+|t|,R-|t|),\quad |t|<R.
\]
Then, exactly,
\[
 I(t)=\int_{D_t}f_\lambda(x)dx
       =2\Phi\bigl(\sqrt\lambda(R-|t|)\bigr)-1,
\]
and
\[
 \log {I(t)\over I(0)}
       =-{2f_\lambda(R)\over I(0)}|t|+O(t^2).
 \tag{NP.12}
\]
The coefficient is exponentially small in R squared but nonzero. For the local scalar mark \(x^2\), let \(m_R\) be its Gaussian expectation conditioned on \(|x|<R\). Direct differentiation of numerator and denominator gives
\[
 \mathbb E[x^2\mid x\in D_t]-m_R
 =-{2f_\lambda(R)\over I(0)}(R^2-m_R)|t|+O(t^2).
 \tag{NP.13}
\]
Since \(R^2>m_R\), this normalized scalar also has a genuine cusp. The example shows why an arbitrarily small carrier norm and a finite first-current norm do not justify a holomorphic effective-action input.

## 6. A canonical local frame confines the nonanalytic core

The first correction need not be discarded or treated as an arbitrary nonanalytic function on every long carrier. Keep the following more informative representation.

For each Q-defect slot e choose one of its literal original test boxes \(\square(e)\) by a fixed geometric rule, independent of the total Mayer support. Define
\[
 C_e=\bigcup_{\square\ni e}\operatorname{foot}(U_{1,\square,e}),
 \qquad U^{\rm loc}_e=U_{1,\square(e),e}.
 \tag{NP.14}
\]
All fixed lift, gauge and incidence collars are included. The real domain
\[
 D_e^{\rm loc}(V_{C_e})=
 \left\{B:\|e^{igB}U_e^{\rm loc}
             U_{1,\square,e}^{-1}-I\|<2gP
                     \text{ for every original }\square\ni e\right\}
 \tag{NP.15}
\]
depends only on this Q core. It is independent of every analytic connector support. On native data the actual global/local comparison implies
\(B_{3P/2}\subset D_e^{\rm loc}\subset B_{3P}\).

Use the same outside-decoupled global background as QC and set
\[
 F_{e,s}^{\rm loc}(B)
    ={1\over ig}\Log\bigl(e^{igB}U_e^{\rm loc}U_{1,e}(s)^{-1}\bigr).
 \tag{NP.16}
\]
Its displacement is bounded by the sum of the actual local/global comparison and the omitted-carrier tail. For the species-additive D of QC,
\[
 \sup_{|s|\le R_o}|F_{e,s}^{\rm loc}(B)-B|
 \le C P_0e^{-cR_1}+C P_0e^{-\nu\ell},
 \tag{NP.17}
\]
on the required fixed free-coordinate tube, with the corresponding derivative bound. Choose the same fixed outside grid and logarithmic additional halo as before. The right side is a fixed small constant. Unlike the frame \(U_1^D\), the real reference in (NP.14) does not change when an unrelated analytic connector is added to D.

### Theorem NP.2 — exact integrated-core representation

Every first-step Q-defect functional may be represented exactly by
\[
 \mathcal P_{e,s}[f]=
  \int_{D_e^{\rm loc}(V_{C_e})}
       f(F_{e,s}^{\rm loc}(B))\det DF_{e,s}^{\rm loc}(B)\,dB
              -\int_{B_P}f(z)\,dz.
 \tag{NP.18}
\]
At s=1 it is precisely integration against the original \(\rho_e-\mathbf1_{B_P}\). Its real-domain dependence is confined to \(C_e\). Its remaining dependence on native raw data outside \(C_e\) occurs in analytic density and coordinate coefficients. The QC annulus/side-chain representation, component identity, Gaussian reserve, carrier estimate and finite first-current estimate remain valid with this choice.

**Proof.** Equation (NP.16) is the exact per-slot coordinate change at the physical endpoint; the starred-coordinate reconstruction does not alter its nonexceptional entry. The Jacobian in (NP.18) is retained. The source (1.19) comparison and the MQ outside-tail bound give (NP.17). Thus the hypotheses of the integrated homotopy lemma are unchanged. Each slot still has an annulus at radius at least P or a boundary chain with real norm at least \(3P/2-C\), and bounded imaginary displacement.

The chosen local reference and all tests in (NP.15) have their full defining boxes inside the same initial component. Their definitions are independent of the total D. Restricting to a component therefore gives exactly the same local reference and domain as constructing that component alone. The Gaussian and analytic coefficient families already have the common restriction identity. This proves factorization of the complete integral families.

The domain and its finite-perimeter boundary are fixed when varying any raw variable outside \(C_e\). Dominated integration of the analytic integrand on these fixed real parameter domains proves the asserted native analyticity in those variables. Inside \(C_e\), only the proven real shell/finite-current estimate is asserted. The same Gaussian tail calculation and species-additive size bound prove the old carrier estimates. ∎

For an ambient nonempty guard branch J, choose a fixed original box in J instead. The real domain depends on the original Q boxes, and the weight depends on **all** the slot's original boxes, including unselected guards. MQ.29 gives the comparison on that branch with \(\gamma e^{-cR_1}/g\), paid by the actual R buffer. The empty branch is the fixed 3P ball. The assertion of analyticity away from the core is intended on native coefficient tubes: arbitrary ambient smooth coefficient guards elsewhere are not thereby made holomorphic.

### What is carried by a payload

A connected logarithmic tag can now retain the following data: its Q-defect slots (with multiplicity), their Q cores, their real domains or boundary-chain parameters, the complete local Gaussian marginal and determinant, and the supported analytic connector coefficients. If its real core is \(C=\bigcup_{e\in S}C_e\) and its connector support is X, its true support remains \(Y=C\cup X\). The original integral formula, not just the value of the integrated coefficient, is retained.

**The bare annulus or side-chain functional is not small in total variation.** Its geometric mass is polynomial in P. The factor \(e^{-cP^2}\) belongs to its pairing with the complete Gaussian/interaction reserve on that chain. A payload therefore includes the certificate that each selected defect coordinate remains at radius of order P, with bounded imaginary displacement, and that the remaining density admits the positive quadratic reserve used in QC.18. It does not detach an intrinsically tiny signed measure from that density. If its already integrated small coefficient is used instead, the same Gaussian tail cannot be charged a second time.

This distinction is material for another integration. The first-step carrier estimate survives in this decorated representation, but the later operation must either preserve its retained reserve or prove a new compatible one. Smallness of the previously integrated value alone does not establish that fact.

## 7. Exact real fiber-frame identity at a following ordinary step

There is one useful concrete coordinate identity independent of analyticity of the payload. Consider the actual one-block group-average constraint at the next lattice spacing. Let U and \(U_D\) be two admissible real backgrounds with the **same** prescribed coarse averages. Use the ordinary source exceptional-bond chart about each background.

On all nonexceptional free edges in the full constraint stencil of a physical set X put
\[
 A_e(B)={1\over ig_1}\Log
             \bigl(e^{ig_1B_e}(U_D)_eU_e^{-1}\bigr).
 \tag{NP.19}
\]
Then the two reconstructed nonexceptional old links agree exactly. Each exceptional old link is the unique solution of its actual local group-average equation with its coarse target and the neighboring free links fixed. Those data are now the same. Hence
\[
 \chi_U(A(B),W)|_X=\chi_{U_D}(B,W)|_X.
 \tag{NP.20}
\]
All exceptional footprints must be included; this is not an identity obtained by matching only the visibly stored edges. The common first-layer source incidence makes the exceptional equations available. The exact finite coordinate Jacobian remains part of any changed integral.

Thus a real physical cutoff payload on X can be specified in a local fiber frame. This algebraic identity requires exact equal coarse averages. A background obtained merely by clipping link logarithms is insufficient. One can construct exact constrained auxiliary frames by restricting independent coordinates and using the local exceptional solve, as in MQ, but a simultaneous complex density family for a later interacting step still has to be supplied.

Equation (NP.20) also does not make a nonsmooth payload holomorphic in B. In particular, one cannot apply QC's closed-holomorphic-form Stokes argument to the product of an analytic density and an already aggregated arbitrary Lipschitz function of B. The retained joint real-domain representation in Section 6 is the appropriate object on which a further chain argument would have to act.

## 8. One exact further physical integration

Let \(\mathcal M_1\) be the literal next group-averaging map. Without invoking an analytic effective action, the physical first-branch density has the exact pushforward measure
\[
 \lambda_2(dw)=
  \int dV\,C_0(V)\int dz\,D_V(z)\prod_e\rho_e(z_e,V)
                        \,\delta_{\mathcal M_1(V)}(dw).
 \tag{NP.21}
\]
This is a positive finite-volume measure and is exactly the next coarse readout of the first R-averaged branch. No replacement of \(\delta E\) by an analytic function occurs. For a gauge-invariant microscopic mark insert \(F(\Phi_V(z))\) in the same integral. For an arbitrary pre-insertion mark also integrate the exact normalized center-fixed Haar preimage in RA.4a. Products use the same joint law.

More generally, if a specified exact next operation has kernel \(\mathcal L_2(dw,dV)\), including its actual coarea, gauge and selector factors, replace the last pushforward in (NP.21) by that kernel. Its source-independent geometric choices remain specified. The identity is an ordinary positive iterated integral before any conditional normalization.

When the corresponding base conditional law \(\nu_w^P(dV)\), formed with \(C_0Z_P\), exists, the corrected conditional law is exactly
\[
 \nu_w^Q(dV)
  ={e^{\delta E(V)}\nu_w^P(dV)
        \over\nu_w^P(e^{\delta E})}.
 \tag{NP.22}
\]
For a microscopic source, the more informative identity is
\[
 Z_2(t;w)=\int\mathcal L_2(w,dV)\,C_0(V)Z_Q(t;V).
 \tag{NP.23}
\]
Finite source derivatives commute with this finite-volume integral on its bounded source domain. Thus the density jets, with the original cutoff-core integrals retained, pass exactly to the next physical readout. The conditional or outer connected logarithm is taken **after** this integral; an average of \(\log Z_Q(t;V)\) would be a different quantity.

These formulas perform a genuine next physical integration and preserve normalization. They do not bound its localized connected coefficients. In particular, they do not authorize inserting the Lipschitz function \(\delta E\) into the next step's holomorphic action input and quoting the ordinary theorem unchanged.

## 9. The one-step size payment, and the unproved closure condition

Keep each nonanalytic core separate from its analytic connectors. For n old Q defects, the old core volume is at most \(CnR_1^4\). In the next lattice units, enlarging only those cores by a next-scale Q buffer has volume
\[
 |C^{\rm next}|\le Cn(R_1/L+R_2+m)^4.
 \tag{NP.24}
\]
The source running couplings are comparable over one ordinary step, so the rounded logarithmic radii \(R_2,R_1\) are comparable up to a fixed L-dependent factor. Hence (NP.24) is at most \(C_LnR_1^4\). The first Gaussian reserve, if preserved in the later joint integral, has enough remaining tail to pay this **single additional** footprint cost, since \(P_0^2/R_1^4\to\infty\). Reserve fractions must be allocated once; the same tail is not spent independently in two estimates.

An arbitrary long analytic connector X receives only its fixed primitive collar. A growing R-neighborhood of every such X would cost \(\exp(C\kappa R^4|X|)\), which a fixed \(\exp(-\nu|X|)\) carrier bound does not pay. The core/connector distinction avoids that invalid step.

The remaining concrete transport condition is a common **joint** next-step localization of the analytic density, exact physical fiber frames and retained first-cutoff domains, with a uniform quadratic reserve on every resulting chain and exact component identities. In such a representation a new boundary piece may come from an old cutoff surface; its old large-fluctuation coordinate and reserve must remain visible. Neither (NP.20), a first-distance-decay estimate, nor the small norm of the integrated \(\delta E_X\) proves this condition. No complete second-step carrier theorem is claimed here.

## 10. A further local integral lemma after the next R sum

The real fiber identity gives more than the pushforward formula if the next R sum is also completed. There is then no need to keep the next fixed-P comparison cutoff on a coordinate carrying the old nonsmooth domain. Keep its actual next Q factors whole instead.

Let C be a union of n old Q cores, and let S contain every independent next-step coordinate in the full ordinary exceptional-constraint stencil needed to reconstruct C. Include the adjacent fixed-L gauge and incidence collars. Enlarge the current raw footprint to contain every **next** local Q reference box for slots in S. Its size is as in (NP.24). This construction is attached to the old cores, not to an arbitrary long analytic connector.

Merge core components whose full constraint halos overlap, and use one common frame on each merged component. This prevents conflicting frame assignments on a shared independent coordinate. The union of the next Q footprints is contained in the Minkowski enlargement of the old core union, so its bound is \(Cn(R_1/L+R_2+m)^4\); it is not \(|S|R_2^4\). The choice of these merged core frames is independent of analytic connector supports.

Choose an exact constrained real local frame \(U_D(W)\) with the same next coarse target W as the global frame. On S perform (NP.19). A next source Q test on e in S then becomes exactly
\[
 \|e^{ig_1B_e}(U_D)_eU_{2,\square,e}(W)^{-1}-I\|<2g_1P_1.
 \tag{NP.25}
\]
Its reference boxes are in the chosen enlarged core. It is independent of the outside localization parameters. The original old physical readout on C is simultaneously \(\chi_{U_D}(B,W)|_C\), by (NP.20). Thus all of the old real cutoff domains, as functions of B and old latent variables, are also fixed under those parameters.

Here \(g_1P_1\) denotes the literal next Q threshold in its own free-coordinate convention. It is not an identification of that threshold with the printed later R radius. The local bound below keeps the next Q factors whole and does not use \(P_1\to\infty\) or a new next-cutoff tail estimate.

An important coordinate qualification applies to a complex outside family. Either its backgrounds must satisfy the same coarse constraints, or its exceptional entries must be defined by the local exceptional solve with the **fixed target W directly**. A family made only by clipping link logarithms need not have this property. With the fixed-target solve, equality of the free physical entries forces equality of the exceptional entries on the old stencil for every admitted complex parameter. No stationarity of that decoupled family is required for this algebraic identity.

### Lemma NP.3 — analytic localization of one retained real-core integral

Consider a finite next-step Mayer term with one or more retained old core payloads. Suppose the following primitive data have been supplied.

Here the next leading action and precision are the actual inherited ones, including the constrained classical action \(A(U_1(V_1))\), its Schur Hessian and the next gauge term. They are not replaced by a new bare Wilson precision merely because the first-step PG gap was proved.

* The next normal-form density and analytic connector coefficients have a common outside-parameter family. Its normalized marginal Gaussian is generated by the same continued covariance in its precision and determinant. Relative to a positive real **centered** marginal \(p_{1,0}(B)\), its usual GM discrepancy is tunably small. Its complete interaction and coarea coefficients are holomorphic on the stated free-coordinate tube and have the corresponding small quadratic majorant.
* On S, the simultaneous physical-frame change \(A_s(B)\) is holomorphic, equals the exact real change at s=1, and obeys
\[
 \sup_{e\in S}|A_{s,e}(B)-B_e|\le a,\quad
 \|D_{B_S}A_{s,S}-I\|_{\rm row}\le Cg_1a,
 \qquad a\le a_*<\infty,
 \tag{NP.26}
\]
with fixed constants. Outside S it is the identity until any separately declared next-defect transformation. The complete old physical stencil is fixed as just described. The local next-Q domains in (NP.25) lie inside a fixed multiple of \(B_{P_1}\).
* For every real B in the retained parameter domain, the reconstructed first retained field and all analytic continuations used by the coefficient family lie inside the **first-step native coefficient tubes**, or inside a separately specified extension having the same analytic reserve. This is an admission hypothesis. An ambient smooth guard composed with a complex changing raw field is not holomorphic merely because the outside parameter is complex. Old admission selectors that are not redundant must be retained on their actual footprints.
* The old payload retains its conditional Gaussian certificate before integration. At fixed real B, its analytic old marginal/interaction factors are bounded relative to a positive normalized **centered** old Gaussian \(p_{0,B}\), with uniform covariance bounds, by a small quadratic tilt, a tunably small loss per old integrated rank, and the stated analytic connector majorant. Every old selected defect coordinate remains on an annulus or side chain with real norm at least \(cP_0\), bounded imaginary displacement and polynomial surface mass. The same bound holds uniformly on the outside polydisc. This is the QC/QS integrand certificate with B as a real parameter, not an assumption that an already integrated \(\delta E_X\) is small or a bound for an arbitrary pinned old mean.

Then the integral of the retained old real domains and the whole next Q factors on S is holomorphic in the outside parameters. It satisfies an absolute bound of the form
\[
 C A_I\exp\{\eta(r_0+r_1)+C_a|S|\}
                         e^{-c_0 nP_0^2},
 \tag{NP.27}
\]
after a fixed allocation of the old Gaussian reserve. Here \(A_I\) is the supported analytic connector majorant, \(r_0,r_1\) are the local old and next marginal ranks, \(\eta>0\) can be made small within the stated reserve, and \(C_a\) depends only on the fixed displacement bound and the marginal gaps. There is no factor \(e^{CP_1^2|S|}\).

**Proof.** In the B coordinates the joint real parameter domain consists of the next local Q restrictions (NP.25), the retained old domains as functions of B, and any explicitly retained local real weights. It is independent of outside parameters. These real factors may be nonsmooth in B. All remaining factors—both Gaussian precision/determinant families, complete analytic interactions and connector coefficients, and the exact coordinate Jacobian—are holomorphic in those parameters. Dominated integration therefore proves holomorphy without applying Stokes to a nonsmooth old factor.

For the bound, write \(A_s(B)=B+\Delta_s(B)\), with \(\Delta_s\) supported on S. The covariance reserve and Young's inequality give, for arbitrarily small fixed positive \(\delta\),
\[
 |p_{1,s}(A_s(B))\det DA_s(B)|
 \le \exp\{C u_m r_1+C_{a,\delta}|S|}
          p_{1,0}(B)\exp\{(C u_m+\delta)|B|^2\}.
 \tag{NP.28}
\]
Indeed \(\|\Delta_s\|_2^2\le a_*^2|S|\). The mixed real displacement term is bounded by \(\delta|B|^2+C_{a,\delta}|S|\), and the Jacobian costs at most \(e^{Cg_1a_*|S|}\). The relative determinant loss remains \(e^{Cu_mr_1}\). This step uses the O(1) **normalized** displacement in (NP.26); a generic pinned mean of order P would not give (NP.28).

Apply the old conditional Gaussian certificate at fixed B. Integrate the old ordinary variables exactly and use the old defect coordinates' tails as in QS.17. Surface powers and constants per old defect are paid once from that reserve. The result is bounded by
\(C A_I e^{\eta r_0+b|B|^2}e^{-c_0nP_0^2}\), with b in the remaining next Gaussian reserve. The fixed real next-Q factors are bounded by one, so they can be dropped for this absolute upper bound. Integrate all remaining B coordinates against the positive real Gaussian with its small total quadratic tilt. Its exact normalization costs \(e^{\eta r_1}\). Equation (NP.27) follows. ∎

Since \(|S|\le Cn(R_1/L+R_2+m)^4\), one fixed fraction of the old tail pays \(e^{C_a|S|}\) for sufficiently small coupling. This is the core-only size payment. It does not inflate the norm of a long analytic connector by an R-dependent factor per connector block.

For next-defect transformations on coordinates outside S, the old real domain is independent of those coordinates because S contains its full constraint stencil. The QC contour **identity** is therefore algebraically available in those outer coordinates without differentiating the old nonsmooth factor. Its quantitative use additionally requires the actual next Q radius, a verified coordinate tube and frame displacement, and the old Gaussian/analytic certificate uniformly on those added transformations. Those next-cutoff budgets are not proved by domain independence and are not imported unchanged from the first R radius. If such a coordinate is actually read by an old domain, it must first be added to S; omitting that closure would invalidate the claim.

### What the local lemma does and does not close

The lemma removes a genuine obstruction in the *form* of the next integral: raw nonsmoothness of the old core does not by itself prevent analytic outside localization. It is enough to freeze the old physical readout and keep the next Q tests whole on that core. A comparison to the unchanged fixed-P operation on those same coordinates is unnecessary and would reintroduce moving boundaries there.

For the exact finite expansion, if a retained core is present, absorb all Q factors on S into its composite integral and expand the cutoff alternatives only outside S. This is the identity
\[
 H_C\prod_e\rho_{2,e}
    =\left(H_C\prod_{e\in S}\rho_{2,e}\right)
                         \prod_{e\notin S}\rho_{2,e}.
 \tag{NP.29}
\]
Overlapping core stencils must be merged before making this choice. An individual next-cutoff alternative on S must not also be inserted. The unmarked denominator is still the actual next Q operation, not a fresh Gaussian or the probability of all P tests.

To turn this lemma into a complete next-step theorem one must construct the stated common density/frame family for the actual next action, check the first-native admission uniformly on its real parameter domains, and verify component consistency for the merged-core prescription and the unmarked denominator. Disconnected factors must cancel using that actual denominator before a normalized carrier norm is concluded. Standard anchored unmarked cluster smallness would pay the additional vacuum incidences of a finite core, but that algebra cannot repair a missing density or component-family identity. The first theorem's ambient smooth extension alone supplies none of these new holomorphic-composition claims. These are the explicit remaining source-application gates; (NP.27) is a local integral theorem under primitive matrix and domain bounds, not an assumed marked output estimate.

## 11. Complementary Q histories cancel their artificial boundary exactly

The cusp criterion above concerns the selected P/Q-regular branch. It is not automatically a cusp of the complete coarse Wilson law. There is a separate exact recombination route.

Before derived geometries, coordinate relocations or conditional normalizations are introduced, use the common physical first-step integration/readout variables. If \(\chi_\ell(V,z)\) is the good indicator for primitive Q test \(\ell\), the complete set of complementary patterns satisfies pointwise
\[
 \sum_{\omega\in\{0,1\}^{\mathcal T}}
       \prod_{\ell\in\mathcal T}
       \chi_\ell^{\omega_\ell}(1-\chi_\ell)^{1-\omega_\ell}=1.
 \tag{NP.30}
\]
The product notation means selecting one of the two factors, including at a boundary according to the literal complementary convention. With the same complete physical density and the same readout kernel in every summand,
\[
 \sum_\omega\int D_V(z)F(z)\,\chi_\omega(V,z)dz
                    =\int D_V(z)F(z)dz.
 \tag{NP.31}
\]
The identity holds for the unmarked mass, every original mark and all finite source jets. It includes the normalized gauge preimage when that is part of the chosen old state.

Along a real raw path, the sum of the signed finite differences of the indicators is identically zero. Hence their one-sided boundary currents cancel **before** division by any conditional mass. In particular the negative first-order loss in the all-good branch in (NP.6) is balanced by complementary branches in this common representation. If the remaining density and readout are analytic on a fixed common domain, this particular cutoff partition creates no raw nonanalyticity in their sum.

For branch masses \(M_\omega\) and normalized branch expectations \(Q_\omega F\), the correct recombination is
\[
 QF={\sum_\omega M_\omega Q_\omega F\over\sum_\omega M_\omega},
 \tag{NP.32}
\]
not an unweighted sum of conditional outputs or conditional logarithms. Once the source has assigned different integration regions, backgrounds and relocation coordinates to different patterns, all of those changes must be undone, or proved to be exact pushforwards to the same physical integration/readout, before (NP.31) can be invoked. A retained-output state that differs by geometry is not already that common representation.

At the first split, CMP119 (1.8) is literally the complementary identity (NP.30), so the recombination statement is source-exact. It does not estimate the complementary branches, prove a common global holomorphic readout, or supply their physical carrier/current bounds. Nor does it claim that summing only some favorable patterns cancels every boundary. It does establish that a branch cusp is not a no-go theorem for the full Yang–Mills measure.

## 12. Status

The actual first correction has an explicit flat-point cusp criterion and an exact decorated integral representation with nonanalytic Q cores, analytic connectors and a retained Gaussian tail certificate. The physical measure can be pushed to the next coarse lattice without making a false analyticity assertion. The further local integral lemma shows how simultaneous physical-frame freezing and whole next-Q factors avoid Stokes on an old nonsmooth factor, under explicit next primitive admission and Gaussian bounds. Exact mass-weighted Q-complement recombination gives a distinct way to cancel the artificial cutoff boundary.

A genuine nonzero source response in (NP.11), the actual next common density/frame and component construction, and the full complementary-branch estimates remain unresolved here. These are precise downstream gates, not a claim that the first R-averaged construction fails or that Yang–Mills existence is impossible.

Primary sources: CMP119 pp.246–251 and 255; CMP109 pp.252–254 and 267; the actual flat constraint/gauge identities and finite-range matrix are recorded in AB. Companion proofs: MQ native/ambient input, QS, QC, RA and the density-weighted interface DW.
