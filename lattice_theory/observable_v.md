# All-depth physical Q/R births on strict regular carriers

**Status:** A new all-depth conditional sector, with the inherited cutoffs and their exact denominator retained. This result is restricted to an actual full regular input carrier and a strictly admitted next coarse background. It includes physical large-fluctuation births, beyond the canonical-small gauge-innovation sector H9.37. It does not estimate P-bad coarse outputs or arbitrary unprocessed exteriors.

The probability law used below is the positive conditional law **before** the Q and R decompositions are performed. In particular, it is not normalized again after prescribing a Q-good pattern. All running couplings, action coefficients, averaging maps, and cutoffs are frozen.

### 1. The actual carrier and the next-background restriction

Fix a scale \(k\), a compatible finite torus, and an actual carrier whose current determining data consist of the current field \(V_k\) alone. There are no unprocessed older-field variables. Assume its current physical density has the regular form

\[
\rho_{k,H}(V_k)
=c_H\,\chi_k(V_k)
\exp\{-g_k^{-2}\mathcal W_k(V_k)+\mathcal F_{k,H}(V_k)\},
\qquad \mathcal F_{k,H}=E_k+R_k=B_k+\delta_{k,H}.
\tag{RB9.1}
\]

Here \(\mathcal W_k=A\circ U_k\) is the retained leading Wilson action. The equality and admitted intrinsic norms of the actual regular action are those of A8.27–A8.41. The regular reference \(B_k\) has a fixed bounded analytic norm; \(\delta_{k,H}\) has arbitrarily high inverse-coupling-power smallness on the actual narrow chart. Any carrier scalar \(c_H>0\) is retained in the outer history weight. It cancels only in this fixed carrier's conditional fiber law. A boundary potential outside the A8 regular norm is not included in (RB9.1).

The label \(H\) records this current positive carrier after the source's regular resummations. It does not additionally reveal individual past labels that have already been summed into \(E_k+R_k\). Conditioning on such extra labels can change the physical density and would require a separate verification of (RB9.1). Earlier successful resets are allowed when their contributions are already in the identified regular action.

Condition on the next field \(W=MV_k\). Let
\(\bar V_k=M^kU_{k+1}(W)\) be its admitted full regular minimizing field, in the source averaged-contour axial gauge. The background restriction used here, denoted \(\mathcal G_k\), is the following concrete strict version of the source P-good carrier:

* the local copied-data backgrounds entering the P tests and the full minimizing field are admitted by the source regular atlas;
* the local backgrounds entering the inherited characteristic factors \(\chi_k\), evaluated at \(\bar V_k\), are below their original curvature thresholds by a fixed fraction;
* the source local-to-global minimizing-field comparison on each Q test interior, and on every eligible R test interior, has error at most \(C\varepsilon_k e^{-cR_k}\).

The fraction is fixed before the weak endpoint. This is a condition on the actual background, not a removal of a cutoff. At the flat background it holds with a strict margin. The source contraction estimates preserve it on an admitted neighborhood. More generally, the source P test with a suitably stricter bound, the scale factor \(L^{-2}\), and the local-to-global comparison give this carrier whenever the corresponding global regular minimum is admitted. We do not replace a merely P-good or a mixed-boundary output by an element of \(\mathcal G_k\) without this check.

Write

\[
p_k=p_0(g_k),\qquad
\varepsilon_k=g_kp_k,\qquad
\delta_k=c_\delta g_kp_k,\qquad
R_k\asymp(1+\log g_k^{-2})^r,
\quad p_k\asymp(1+\log g_k^{-2})^P,
\quad P\ge5r.
\tag{RB9.2}
\]

The source constants, including \(c_\delta=A_1/A_0\), are fixed. Norm equivalence constants for the fixed Lie algebra are absorbed below.

### 2. Put the complete pre-classification fiber in one regular chart

Insert the actual normalized soft axial-gauge identity and make the source change of variables. Because the block-center gauge values are fixed, the averaging constraint \(MV_k=W\) is unchanged. The resulting measure describes the actual joint field and auxiliary-gauge law used to define the Q/R labels. This is the same positive gauge-fixing identity used in H9-B.

The inherited \(\chi_k\) bounds the current plaquettes. The axial factor bounds the block contour variables. The block axial comparison with \(\bar V_k\) then gives, throughout the complete pre-Q fiber,

\[
\left\|V_k\bar V_k^{-1}-1\right\|_\infty
\le C\varepsilon_k.
\tag{RB9.3}
\]

This is the regular input version of the estimate stated before CMP119 (1.8), and used in its (3.13)–(3.14). It uses the prior cutoff and the good coarse background, not the new Q-small selector. At weak coupling the relative field is therefore in the source logarithmic chart even on a Q-bad branch.

Linearize the block-average constraint and eliminate the distinguished bonds, exactly as in the source one-step construction. With \(A\) the rescaled independent starred-bond variables,

\[
V_k(A)=\exp i\{g_kCA-\mathfrak hD(g_kCA)\}\,\bar V_k.
\tag{RB9.4}
\]

The independent-to-physical map is block local. On an independent starred bond, the constraint elimination has left the logarithm equal to \(g_kA_b\). The local map and its inverse are analytic in a fixed small physical field ball. Equation (RB9.3) therefore puts the exact fiber support inside

\[
D_H=\prod_b\{|A_b|\le H_k\},\qquad H_k=C_Hp_k.
\tag{RB9.5}
\]

The constant \(C_H\) is chosen to contain the entire support, not to impose a new physical restriction. The chart radius needed to evaluate the regular potentials contains \(g_kH_k\). Indeed A8.20–A8.22 give a narrow radius \(r_k=c_rg_k(\log g_k^{-2})^{q_1}\) with \(g_kH_k/r_k\to0\). The constant multiple in (RB9.5) does not change this.

After subtracting field-independent terms, the exact conditional law is

\[
d\mu_{k,H,W}(A)
=Z_{k,H,W}^{-1}\,
{\bf1}_{D_H}(A)
\prod_{a\in\mathcal I_k}\eta_a(A;H,W)
\exp\{-\tfrac12\langle A,M_k(W)A\rangle+\mathcal V_k(A;H,W)\}\,dA.
\tag{RB9.6}
\]

The factors \(\eta_a\in\{0,1\}\) are all inherited curvature and axial cutoff factors. Jacobians and the nonquadratic gauge-fixing action are in \(\mathcal V_k\). No inherited factor has been dropped. The precision is the actual constrained Gaussian precision, including the prescribed soft gauge term. The source propagator bounds give a volume- and depth-uniform positive gap and exponential kernel bounds.

The inherited factors have the following source-specific properties:

\[
\begin{split}
&\eta_a\text{ depends on }A|_{S_a},\qquad
\operatorname{diam}S_a\le CR_k,
\quad |S_a|\le CR_k^4,\\
&\sup_b\#\{a:b\in S_a\}\le C_{\rm ov},\\
&\eta_a(A)=1\quad\text{if }\sup_{b\in S_a}|A_b|\le r_{\rm in,k},
\qquad r_{\rm in,k}=c_hp_k.
\end{split}
\tag{RB9.7}
\]

For the curvature factors, finite dependence is literal: CMP119 (2.16)–(2.17) defines the local minimum from current links in one enlarged \(LM_2R_k\) cube. Composing with (RB9.4) adds only a fixed block collar. The supports of the relevant cube families have bounded overlap. Axial factors have one-block support. The last line is the strict-margin version of the argument (3.6)–(3.9): a fluctuation of size \(c_hg_kp_k\), with \(c_h\) chosen sufficiently small, cannot exhaust the fixed inherited margin. Its constants do not grow with the microscopic depth. Local factors can be extended by zero outside their local portion of \(D_H\); this gives bounded, finite-support functions everywhere without changing (RB9.6).

In particular the actual denominator is positive, because a product neighborhood of \(A=0\) of radius \(r_{\rm in,k}\) is present. We will not use the extensive measure of that neighborhood to estimate the denominator.

### 3. The regular interaction remains admitted on the larger box

The regular localized fluctuation expansion can be performed on \(D_H\). The leading Wilson remainder has cubic physical-field order. The regular old action is evaluated through the base-preserving intrinsic pair map. Hence its local-potential norm obeys a bound of the form

\[
\|\mathcal V_k\|_{\rm loc,D_H}
\le Cg_kH_k^3+Cg_kH_k\|B_k\|_{
\rm pot}+C\|\delta_{k,H}\|_{
\rm pot,narrow}
=:v_k\longrightarrow0.
\tag{RB9.8}
\]

One can retain the quadratic remainder estimates of CMP116 Lemma 2 instead of the first term in this supremum bound; either supplies the required admissible local neighborhood. The source normalization has already removed the leading linear term by constrained stationarity. The remaining old-action and Jacobian linear terms are included in the small potential in (RB9.8). The microscopic fine-link count is not used as the potential norm.

There is enough fixed spatial reserve for the source Mayer and Gaussian-localization constructions. In particular the global regular interaction is not replaced by a bounded extensive Radon–Nikodym factor.

### 4. Inherited nonlinear cutoffs are local rare defects

Set \(d_a=1-\eta_a\). For every finite family \(\mathcal A\subset\mathcal I_k\), (RB9.7) gives a union over choices of witness bonds in the supports. A bond belongs to at most \(C_{\rm ov}\) supports. Thus at least \(|\mathcal A|/C_{\rm ov}\) different witness bonds are needed. For a sufficiently small fixed \(u>0\),

\[
\prod_{a\in\mathcal A}d_a(A)
\le
\sum_{\text{witness assignments}}
\exp\{-cu r_{\rm in,k}^2|\mathcal A|\}
\exp\{u\sum_{b\in P}|A_b|^2\},
\tag{RB9.9}
\]

where \(P\) is the set of distinct witnesses and the number of assignments is at most \((CR_k^4)^{|\mathcal A|}\). Constants absorb the fixed overlap loss. The positive quadratic exponential is absorbed into the Gaussian precision. Its Gaussian determinant cost is at most \(e^{C|P|}\), uniformly in the ambient volume and the admitted interpolated precision. The remaining Gaussian coordinates are integrated; this is not a uniform estimate after conditioning them to an arbitrary exterior value.

Here is the precise modification of the source cutoff expansion. First Mayer-expand the regular interaction. On the union \(Y_0\) of active potential supports, keep the product cutoff from \(D_H\), exactly as in CMP116 (2.1)–(2.3). Expand its remaining one-bond factors in the usual way. In addition, use the finite identity

\[
\prod_a\eta_a
=\sum_{\mathcal A}(-1)^{|\mathcal A|}
\prod_{a\in\mathcal A}d_a.
\tag{RB9.10}
\]

Include the entire \(S_a\) in the initial localization domain whenever \(a\in\mathcal A\). Only a present cutoff defect enlarges that domain by \(O(R_k^4)\). One does not enlarge every ordinary potential support by an \(R_k\)-collar; doing that would incorrectly charge the large support cost to the regular activity.

Now perform the conditional Gaussian integration and covariance localization of CMP116 (2.5)–(2.26). The bounded real functions \(d_a(A;H,W)\) stay inside the finite-coordinate integrand. The complex decoupling parameters differentiate covariance and precision operators, while these fixed cutoff functions are left unchanged. Consequently no differentiability of a hard cutoff, and no holomorphic dependence of its moving background boundary, is required. This argument proves a real conditional probability estimate for fixed \(H,W\); it does not prove analyticity of this pre-classification law in \(W\).

Here is the uniform complex-integral estimate used in that step. Let \(Z\) be the active localized domain, including every selected \(S_a\), and let \(\mathcal I_{\mathcal D}\) denote the ordinary active-potential integrand, with its retained outer cutoffs. After the source conditional Gaussian completion, all remaining integration coordinates have a complex quadratic precision \(M_{s,t}\) with \(\operatorname{Re}M_{s,t}\ge mI\) and bounded operator norm, uniformly on the source switch polydisc and for the small diagonal tilt \(0\le t\le u_*\) used below. Coordinates outside the localized carrier have already integrated to one. These bounds include the source's small quadratic interaction absorption. Choose a further fixed \(u<m/4\) for (RB9.9). Then \(\operatorname{Re}(M_{s,t}-2uP)\ge mI/2\). Absolute Gaussian integration and the witness sum give

\[
\int |d\gamma_{s,t}(A)|\,
|\mathcal I_{\mathcal D}(A)|
\prod_{a\in\mathcal A}d_a(A)
\le
\mathcal P_{\mathcal D}
\exp\!\left\{
C|Z|-c r_{\rm in,k}^{\,2}|\mathcal A|
+C|\mathcal A|\log(2+R_k)
\right\}.
\tag{RB9.10a}
\]

Here \(\mathcal P_{\mathcal D}\) is the ordinary product of active-potential bounds from the source Mayer estimate; its existing spatial reserve pays the ordinary part of \(|Z|\). The complex Gaussian determinant ratio costs at most \(e^{C|Z|}\). The extra initial support is at most \(CR_k^4|\mathcal A|\); the subsequent localization extensions have the source switch-decay factors. This proves the asserted defect bound with no dependence on the ambient volume. Cauchy derivatives in the switch parameters retain the same tail majorant because the defect functions are fixed real-coordinate functions inside the active carrier. With a root \(|A_b|^2\), the completed positive Gaussian after this absorption has a uniformly bounded diagonal second moment, so (RB9.10a) gains only a fixed constant, after reserving the same coercivity slack. It does not gain the outer-box radius squared. This is also the root estimate required in §5.

The extra determinant, coordinate-volume, and localization-weight cost from each enlarged defect support is at most \(\exp(C_\kappa R_k^4)\). The witness entropy is \(\exp(C\log(2+R_k))\). Retaining portions of the tail factor to pay both, the added cutoff activity has weighted size bounded by

\[
\epsilon_{\rm inh,k}
\le C\exp\{-c p_k^2+C_\kappa R_k^4+C\log(2+R_k)\}
\le C e^{-c' p_k^2}.
\tag{RB9.11}
\]

The final inequality holds at one sufficiently weak endpoint, by \(P\ge5r\). The usual outer-box defects have the stronger one-bond threshold \(H_k\) and satisfy the same conclusion. The source sums (2.27)–(2.34) are therefore unchanged except for the addition of this small activity. Factorization over disjoint localization components is valid because every \(d_a\) is assigned together with its whole support.

Together with (RB9.8), these bounds leave a strict, volume-independent convergence margin for the polymer logarithm. They are also valid with an arbitrary diagonal precision decrease of sufficiently small fixed norm. This last uniformity will normalize the desired tail estimate.

### 5. A normalized quadratic exponential bound

For any finite set \(P\) of independent bonds, define \(P_P\) as the orthogonal projection onto their Lie-algebra coordinates. Choose \(u_*>0\) so small that

\[
M_{k,t}=M_k-2tP_P\ge\tfrac12m_0I,
\qquad 0\le t\le u_*.
\tag{RB9.12}
\]

This choice is independent of \(P\), the volume, and \(k\). The exponentially weighted covariance norm stays bounded: use
\((M_k-2tP_P)^{-1}=(I-2tM_k^{-1}P_P)^{-1}M_k^{-1}\)
and choose \(t\) below the reciprocal of the fixed weighted covariance norm. The same resolvent expansion supplies the Gaussian localizations used in §4. The nonlinear potential and every inherited cutoff are kept fixed as \(t\) varies.

Let \(Z(t)\) be the exact integral in (RB9.6) with this precision. The preceding construction gives its connected expansion uniformly for \(0\le t\le u_*\). It also gives the normalized one-root bound

\[
\sup_b\mathbb E_{\mu_t}|A_b|^2\le C.
\tag{RB9.13}
\]

For completeness, insert \(|A_b|^2\) before the source Gaussian localization. The root is one fixed finite-dimensional coordinate. In the localized Gaussian estimate it costs a second Gaussian moment bounded by a constant, since the real part of the localized precision retains a fixed gap. If the root meets a cutoff-defect support, the same estimate is made after spending a further fixed fraction of that defect's quadratic tail; its remaining \(e^{-cp_k^2}\) still pays \(R_k^4\). The rooted activity consequently has a uniform summable norm. Exponentiating the unmarked gas and dividing the rooted gas by the same partition function cancels every cluster disconnected from the root. The remaining rooted connected sum is bounded by the strict unmarked convergence margin. This is the normalized rooted identity used in CMP119 (3.43)–(3.47), now with the extra defects (RB9.10). It proves (RB9.13) without estimating \(Z(t)^{-1}\) separately.

Equivalently, the uncut Gaussian part contributes its bounded diagonal covariance, while differentiating the connected interaction/cutoff logarithm creates a localized quadratic root. Both descriptions retain the identical denominator.

The finite-dimensional derivative identity is exact:

\[
\frac{d}{dt}\log Z(t)
=\mathbb E_{\mu_t}\sum_{b\in P}|A_b|^2
\le C|P|.
\tag{RB9.14}
\]

Integration gives the promised positive estimate

\[
\boxed{\quad
\mathbb E_{\mu_{k,H,W}}
\exp\{u_*\sum_{b\in P}|A_b|^2\}
=\frac{Z(u_*)}{Z(0)}
\le e^{C|P|}.
\quad}
\tag{RB9.15}
\]

This is an actual normalized exponential moment. A small-ball lower bound establishes positivity only; the quantitative estimate is the connected rooted estimate (RB9.13) integrated along the same conditional law.

In particular, for specified distinct independent bonds,

\[
\mu_{k,H,W}\bigl(|A_b|\ge ap_k\text{ for every }b\in P\bigr)
\le\exp\{-(u_*a^2p_k^2-C)|P|\}.
\tag{RB9.16}
\]

### 6. Identify the actual Q/R event inside this global fiber

For a Q cube \(C\), the source event is a starred-bond comparison of \(V_k\) with its prescribed local background \(V_C^{(k)}\), with threshold \(2\delta_k\). Both the local background and \(\bar V_k\) use the actual matching averaged-contour axial convention; no post hoc gauge change is made to just one comparison field. On \(\mathcal G_k\),

\[
\sup_{b\in C^{+*}}
|\bar V_k(b)(V_C^{(k)}(b))^{-1}-1|
\le C\varepsilon_ke^{-cR_k}\le\tfrac14\delta_k.
\tag{RB9.17}
\]

Unitary multiplication and the independent-coordinate property of (RB9.4) therefore imply

\[
\{\text{actual Q-birth in }C\}
\subset
\bigcup_{b\in C^{+*}}\{|A_b|\ge c p_k\}.
\tag{RB9.18}
\]

There is a related point for R births. Their chart is constructed after the Q geometry has been selected; it uses the mixed minimum with the current variables retained outside \(\Omega^{k+1}\). For an eligible R cube the starred test bonds are in the protected interior of that region. Compare this mixed minimum to the full regular minimum \(\bar V_k\). The two have the same next average. Their differing determining data are on the outer boundary, bounded by (RB9.3). The source exponential minimizing-field comparison, used in (3.17)–(3.19), gives an \(O(\varepsilon_ke^{-cR_k})\) difference on the R test bonds. Its proof uses the prior P/Q regularity and the protected interior, not the R-small restriction. Thus the actual R-bad independent coordinate, whose rescaled cutoff is \(\delta_k/g_k\) by LFR I (1.9), also forces a global independent coordinate to be at least \(cp_k\).

Consequently, with an event set to false when its source geometric eligibility fails,

\[
\{\text{actual Q or R-bad birth in }C\}
\subset
\bigcup_{b\in C^{++*}}\{|A_b|\ge c p_k\}.
\tag{RB9.19}
\]

The enlarged test set has \(O(R_k^4)\) coordinates. Its enlargement and overlap constants are fixed. R birth is labeled at its actual defining decomposition and carried through subsequent changes of variables; these later reparametrizations do not change the event in the positive lift.

For a specified family \(\mathcal C\) of distinct actual test cubes, select a fixed color subfamily with disjoint enlarged test sets. This retains a fixed fraction of the cubes. Assign one witness to each retained cube and apply (RB9.16). The witness entropy \((CR_k^4)^{|\mathcal C|}\) is absorbed into \(p_k^2\). We obtain the all-depth conditional theorem

\[
\boxed{\quad
\Pi\left(
\bigcap_{C\in\mathcal C}\{
\text{Q or R-bad birth at }C\}
\,\middle|\,H,W\right)
\le e^{-c p_k^2|\mathcal C|},
\qquad W\in\mathcal G_k.
\quad}
\tag{RB9.20}
\]

Q and R test grids can first be separated into their finitely many types. The color loss remains a constant. The bound is uniform in the ultraviolet depth and volume within the stated carrier. In particular it covers canonical-large physical Q/R fluctuations, rather than assuming that only gauge innovations can cause a birth.

No conditional reflection positivity is used. No factor from the posterior probability of \(H\) or \(\mathcal G_k\) is discarded. Averaging the uniform estimate gives, for any nonnegative function \(F(H,W)\),

\[
\mathbb E_\Pi\!\left[
F(H,W){\bf1}_{\mathcal G_k}
\prod_{C\in\mathcal C}{\bf1}_{\{Q/R\text{ birth at }C\}}
\right]
\le e^{-c p_k^2|\mathcal C|}
\mathbb E_\Pi[F(H,W){\bf1}_{\mathcal G_k}].
\tag{RB9.21}
\]

This statement applies to a measurable choice of the specified family from \((H,W)\), by applying the fixed-family inequality fiberwise. It does not assert a causal tower product over different scales: the later coarse backgrounds used in the conditioning need not be predictable from the earlier history.

### 7. Selected current marks and the old-field limitation

Suppose an actual incoming marked function has the deterministic bound
\(|F_k|\le A h_k^{-4}T(h_k)^s\)
on the complete conditional support (RB9.6), where \(h_k\) is the physical lattice spacing. For a selected birth event \(B\), (RB9.20) gives

\[
\mathbb E_\Pi\bigl[
{\bf1}_{\mathcal G_k}{\bf1}_{B}|F_k|^2\mid H,W\bigr]
\le C A^2h_k^{-8}T(h_k)^{2s}
{\bf1}_{\mathcal G_k}e^{-cp_k^2}.
\tag{RB9.22}
\]

Conditional Jensen passes this bound to the corresponding selected conditional mean, with its posterior selector retained. This closes a current-norm entry contribution on the same strict regular carrier. For an old microscopic mark known only to satisfy \(|F_0|\le Aa^{-4}\), the right-hand side still contains \(a^{-8}\). Neither (RB9.15) nor (RB9.20) silently replaces that scale by \(h_k\). The earlier H8/H9/R9 age arguments or an actual regular marked transport bound are still needed.

### 8. What a finite boundary collar does and does not supply

The proof is local enough to apply to a finite regular conditional domain when its **actual** constrained covariance has the same gap/localization bounds, its complete conditional potential is admitted with the same local reserve, and its inherited cutoff factors satisfy the strict local margin (RB9.7) uniformly up to the resampled boundary. Fixed regular boundary values can be carried as parameters in that version. The exact proof then gives (RB9.15) and (RB9.20) for its interior eligible cubes.

This is not automatic for an old unprocessed exterior. A collar of finite physical width does not by itself remove its boundary action or make a surviving characteristic function equal one. The source regular interactions are exponentially local, rather than exactly finite range, and an uncontrolled boundary coefficient can overwhelm the small connecting tail. An inherited boundary cutoff can also force the conditional minimum onto its boundary, destroying the lower neighborhood (RB9.7). These are specific missing estimates: one needs the admitted conditional boundary potential and the strict inherited margin for the same fixed exterior. The fresh reset denominator supplies neither on a failed-preparation exterior.

Accordingly the new unconditional-in-depth conclusion is (RB9.20) on the actual full regular carrier, and its selected-mark consequence (RB9.22). Physical P-bad outputs, persistent preparation failures, arbitrary old boundary coefficients, mixed-history terminal old means, and joint multiscale ancestry certificates remain outside this sector.

### 9. Sources

The source is used at the following exact interfaces; the added inherited-defect and quadratic-tilt argument is proved in §§4–5.

* **CMP119 (1988), printed pp.246–249, (1.5)–(1.9):** normalized gauge insertion, pre-Q block axial comparison, starred coordinates, and constraint elimination.
* **CMP119, pp.256–257, (2.16)–(2.17):** finite current-field determining patches for the inherited curvature cutoffs.
* **CMP119, pp.265–269, (3.3)–(3.19):** actual Q/R comparison fields, strict inherited-cutoff implication, and the protected local/global minimum comparison.
* **LFR I, printed p.178, (1.8)–(1.9):** the final rescaled ordinary R threshold \(\delta_k/g_k\). This avoids treating the CMP119 (3.16) notation as an established erratum.
* **CMP116 (1988), printed pp.11–19, §2:** fixed cutoff factors remain under the localized Gaussian integral; quadratic tail absorption, determinant bounds, and connected exponentiation. [DOI](https://doi.org/10.1007/BF01239022).
* **CMP119, pp.278–279, (3.43)–(3.47):** the normalized rooted expansion with cancellation of components disconnected from the insertion.
* **A8.20–A8.22 and A8.27–A8.41:** admission of the actual regular E/R potential on a chart containing the larger pre-classification fiber. This module does not identify a mixed-boundary action with that regular action.

The normalization is retained at each stage. The presence of a product lower neighborhood proves that the actual conditional fiber is nonempty; the connected expansion, rather than an extensive small-ball comparison, proves its local normalized probability bound.

---
