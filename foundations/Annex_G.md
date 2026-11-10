# Complete-action analytic domains and the remaining R-bulk theorem

**Annex G.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Hypotheses for the R Hessian

A real value bound gives no uniform R Hessian estimate. The R activities have a complex norm on specified multiscale spaces. Their pullback to the current free coordinates requires a quantitative domain and localization argument, as in Annexes AE and AH for the regular native law under CL.

In Annex B, Theorem 3.1, a fixed physical radius and prefactor apply to the fixed-domain small-field construction. The complete CMP119 construction has running constants. The transferred small-field lemma must retain both the actual radius and the activity majorant until their uniformity has been established.

The complete homogeneous classical-action estimate, native-chart bounds, and fixed-parameter no-R comparison have their separate hypotheses.

The results below are:

1. A source-specific identification of the actual complex R norm, the distinction between its original and current localization scales, and the source's six-power loss in the old-scale sum.
2. A proved Cauchy theorem that keeps actual analytic margins and activity majorants explicit. It gives the precise statement for E and the correct form of a future R theorem.
3. A proved old-scale summation calculation, conditional on an explicitly stated complex marginal-transfer estimate. It keeps the two analytic derivative powers separate from the six old-scale powers and from the current-coordinate normalization.
4. An exact statement of the remaining domain and localization premise. Neither selecting convenient logarithmic exponents nor recentering the native chart alone supplies that premise.

Here **P** means a mathematical implication proved in this note, **L** a precisely scoped source result, **C** a conditional application, and **O** an unproved application to the complete construction.

### 2. The actual R activity is complex analytic

#### 2.1 Original activity space and norm — L

CMP119, printed pp.259–260, separates the inherited effective action into E, R, and B. R has only its vacuum value subtracted:

\[
 R_k(U_k)=\sum_{j=1}^k
 \left[R^{(j)}(\Lambda_j,U_k)-R^{(j)}(\Lambda_j,1)\right].
 \tag{2.1}
\]

Each \(R^{(j)}\) has a localized representation over its specified \(X\in\mathcal D_j\). Its terms have the same three properties as the preceding E activities: localized dependence; extension to a complex analytic function of \((U,J)\); and gauge invariance. The analytic space is the specified \(\mathcal U_j(X,\alpha_{0,j},\alpha_{1,j})\), not a ball of arbitrary link values. Formula (2.28) is

\[
 \alpha_{0,j}=g_j C_0(\log g_j^{-2})^{q_0},\qquad
 \alpha_{1,j}=g_j C_1(\log g_j^{-2})^{q_1}.
 \tag{2.2}
\]

The integers \(q_0,q_1>1\) and the constants are subject to the construction's restrictions. Formula (2.31), is

\[
 \left|R^{(j)}(X,(U,J))\right|
 \le g_j^{\kappa_0}e^{-\kappa d_j(X)}.
 \tag{2.3}
\]

The construction can arrange an arbitrarily large \(\kappa_0\) by fixing its parameters appropriately. This is a complex norm on the stated domain. It is neither a norm on every complex gauge field nor already a norm on the current free fluctuation coordinates.

The distinction matters because admission to these activity spaces involves several conditions simultaneously: plaquette regularity, currents, reconstructed configurations, gauges on the indicated local cubes, and relative complex fields with their required spatial regularity. The multiscale definition on CMP119 p.261, (2.34)–(2.39), makes this explicit for the complete construction. A bound for one relative link coordinate is not the whole admission test.

LFR II, printed p.390, (1.98)–(1.100), verifies the generation of new R activities. The particularly strong new-activity estimate is

\[
 |R'^{(k)}(X,(U,J))|
 \le e^{-p_0(g_k)}e^{-\kappa d_k(X)}
 \tag{2.4}
\]

on its stated complex space. This explains the freely large power in (2.3). It also confirms that R can remain after a previous replacement has removed a large-field region. An empty current large-field set does not imply \(R_k=0\).

#### 2.2 What the real marginal theorem proves — L

CMP119 Theorem 2, (2.44), controls the vacuum-subtracted R sum for regular real backgrounds. Its proof on printed p.283 applies the same gauge identities as for E, but stops at (3.49), without subtracting a coupling term. The resulting small-carrier factor is

\[
 O(1)(L^{j-n})^4g_j^{\kappa_0}e^{-\kappa d_j(X)}.
 \tag{2.5}
\]

The factor \((L^{j-n})^4\) compensates the number of old-scale cells per current physical volume. Large carriers are handled by the stronger exponential in (3.48). The result is a marginal contribution, whose summability comes from \(g_j^{\kappa_0}\), rather than from an extra irrelevant scale factor.

The old-scale estimate printed in (2.46) is

\[
 |R_k(U_k)|
 \le R_1\sum_n |\Gamma_n|\sum_{j\le n}g_j^{\kappa_0}
 \le R_1\sum_n |\Gamma_n|g_n^{\kappa_0-6}.
 \tag{2.6}
\]

The source loses **six** powers here. A two-power loss is not what this source states. Formula (2.6) concerns regular real fields. Differentiating it is not a valid way to obtain a Hessian estimate.

#### 2.3 The current localization transfer — L, with scope

CMP119 printed p.276, first performs the generalized random-walk localization and resums onto current carriers \(Y\in\mathcal D_k\). For carriers inside \(\Lambda_{k+1}\), it transfers the small-field lemmas. The subsequent paragraph explicitly treats R by the corresponding analysis with the coupling-subtraction step omitted. This is genuine evidence for a complex R fluctuation theorem; R is not being replaced by E.

There are two points that the transfer sentence does not make numerically explicit for the present application:

* the full dependence of the fluctuation majorant on the running analytic radii (2.2);
* a complex tube, with quantitative margin, about every point of the actual real cutoff, admitted by every localized old activity and all its auxiliary current variables.

For the other carriers, CMP119 gives in (3.43) the radius \(C_1p_1(g_k)\). It does not print a fixed radius divided by \(g_k\). No identification of that symbol with the later LFR I sharper selector is used here.

### 3. Fixed radii in the original theorem and running radii in the complete construction

#### 3.1 The source dependence is real

CMP109, printed p.263, (1.18), assumes fixed \(\alpha_0,\alpha_1\), independent of the old index. CMP116 (1.19)–(1.22) admits the free fluctuation field on \(g_k\|B\|<\epsilon_1\), subject to

\[
 4B_0C_1e^{16\kappa_1}\epsilon_1\le \tfrac12\alpha_2.
 \tag{3.1}
\]

The proof's interpolation derivative costs \(O(1)\epsilon_1/\alpha_2\). CMP109 p.280, immediately following (3.54), states this dependence explicitly. Its Lemma 4 also imposes restrictions including

\[
 B_3\alpha_3<\tfrac12\alpha_1,
 \qquad 2B_3\alpha_3\le \beta L^{-2}\alpha_0.
 \tag{3.2}
\]

CMP116 p.8 describes the final prefactor as obtained from these parameter restrictions. With fixed parameters this is a fixed constant. Replacing their role by the sequence (2.2) requires another quantitative argument.

Thus the proof step

\[
 \delta_k/\epsilon_1\longrightarrow0
 \quad\hbox{with one fixed admissible }\epsilon_1
 \tag{3.3}
\]

has not been established for the complete-history inherited E action. Furthermore, merely changing \(\epsilon_1\) to \(\epsilon_{1,k}\) while continuing to declare the prefactor fixed is not enough. Some radius ratios in the proof can cancel, but that cancellation has to be shown.

This is a correction to our previous application. It is not a counterexample to the transferred lemma or to Balaban's construction.

#### 3.2 A precise Cauchy replacement — P

Let \(I_k\) be the current free coordinates, \(K_k\) a real set, and \(V_Y\) a localized analytic activity. Suppose for every \(z\in K_k\) the complex polydisc

\[
 \mathbb D_I(z,r_k)=
 \{z+w: \|w\|_\infty<r_k\}
 \tag{3.4}
\]

is in its actual pullback domain, and on this disc

\[
 |V_Y(z+w)|\le A_{k,Y}.
 \tag{3.5}
\]

The activity depends only on the permitted coordinates of \(Y\). Define

\[
 \mathcal A_{k,\gamma}:=
 \sup_i\sum_{Y\ni i}\sum_{l\in Y}
 e^{\gamma d(i,l)}A_{k,Y}.
 \tag{3.6}
\]

Then

\[
 \sup_{z\in K_k}\sup_i\sum_l e^{\gamma d(i,l)}
 \left|\partial_i\partial_l\sum_Y V_Y(z)\right|
 \le {8\mathcal A_{k,\gamma}\over r_k^2}.
 \tag{3.7}
\]

**Proof.** Use coordinate circles of radius \(r_k/2\). For different coordinates, the two-variable Cauchy formula bounds the mixed derivative by \(4A_{k,Y}/r_k^2\). For the same coordinate, the one-variable second-derivative estimate gives \(8A_{k,Y}/r_k^2\). A derivative vanishes when a coordinate is absent from the activity. Sum these bounds using (3.6). Finite-volume sums are immediate; uniformly absolutely convergent activity sums follow by the same majorant. This proves (3.7). No continuation or nonvanishing statement for a logarithm is used. \(\square\)

The actual radius can depend on a real point or on a carrier. Replacing the right side of (3.6) by the corresponding sum of \(A_{k,Y}/r_{k,Y}(z)^2\), and then taking the supremum, gives the identical proof. A common radius is merely a convenient sufficient version.

#### 3.3 Correct E statement — C

Suppose the transferred current E activities have the **proved** majorant

\[
 |V^E_{k,Y}(B)|\le E_0\epsilon_{1,k}K_k^E
 e^{-\kappa_*d_k(Y)},
 \qquad \|B\|<\epsilon_{1,k}/g_k,
 \tag{3.8}
\]

where \(K_k^E\) includes all radius dependence. On a real window \(\|B\|\le P_k\), set \(\delta_k=g_kP_k\). If \(\delta_k<\epsilon_{1,k}\), the actual Cauchy margin gives

\[
 \eta_\gamma(W_k^{E,\mathrm{bulk}})
 \le C E_0K_k^E
 {\epsilon_{1,k}g_k^2\over(\epsilon_{1,k}-\delta_k)^2}.
 \tag{3.9}
\]

The carrier entropy constant is the usual current-scale constant, provided \(\kappa_*\) retains its entropy reserve. There is no new old-scale sum: (3.8) is already the resummed E estimate. Formula (3.9) is the valid replacement for the fixed-radius inference.

For example, if a separate proof establishes \(\delta_k\le\theta\epsilon_{1,k}\), \(\theta<1\), and \(K_k^E\) bounded, then the right side is \(O(g_k^2/\epsilon_{1,k})\). If the established majorant is instead uniformly \(O(E_0)\), and the free-coordinate margin is of order \((\log g_k^{-2})^q\), (3.7) gives \(O(E_0(\log g_k^{-2})^{-2q})\). Both are sufficient smallness mechanisms. Neither set of premises has been proved here for the complete history construction.

The literal cutoff printed in CMP119 (3.16) deserves separate bookkeeping: if it indeed bounds the already normalized free variable by \(\delta_k\), it is smaller than the conservative window \(P_k=\delta_k/g_k\) used. It could improve the margin. This note does not silently resolve the source's variable convention in order to assert a larger theorem.

### 4. R derivative costs and the old-scale sum

#### 4.1 What follows directly from the primitive complex norm — P with L input

Fix an old activity \(R^{(j)}_X\) and an analytic coordinate chart whose polydisc of radius \(a\) lies inside its actual \((U,J)\) domain. Cauchy's formula applied to (2.3) gives, at its center,

\[
 |\partial_u\partial_v R^{(j)}_X|
 \le 2a^{-2}g_j^{\kappa_0}e^{-\kappa d_j(X)}
 \tag{4.1}
\]

for unit coordinate directions, using the full radius by a limiting argument. This is an actual complex second-derivative estimate for the original R activity. It does not concern the current coordinate Hessian until the pullback, localization, and admissible radius have been established. In particular, the current derivative of a composite function includes

\[
 D^2(R\circ\Phi)
 =(D\Phi)^T(D^2R)(D\Phi)+(DR)D^2\Phi.
 \tag{4.2}
\]

Ignoring the second term away from the zero configuration is invalid. Applying (3.7) to the full pulled-back activity would automatically include it.

#### 4.2 A radius-explicit marginal-transfer premise — O

The following is one sufficient quantitative form of what still has to be proved. It is stated as a premise, not as an extraction already completed from the transfer sentence.

Let \(V^R_{j,k,Y}\) be the current localized vacuum-subtracted activity originating at old scale \(j\). For every real cutoff point suppose its admitted complex current tube has common radius \(r_k\), and suppose

\[
 \sup_i\sum_{Y\ni i}\sum_{l\in Y}e^{\gamma d(i,l)}
 \sup_{\mathbb D(z,r_k)}|V^R_{j,k,Y}|
 \le C\ell_j^A g_j^{\kappa_0}{Q_k^2\over a_j^2},
 \quad \ell_j=\log g_j^{-2}.
 \tag{4.3}
\]

Here \(a_j\) is an actual admitted old-field radius, \(Q_k\) bounds the physical field/curvature amplitude needed by the marginal estimate on the tube, and \(A\) is fixed. The four powers of the scale ratio have already compensated the old-cell count in (4.3). This is exactly where the marginal, gauge-invariant localization enters. It must also include the large-carrier tail, the localized decoupling parameters, and both terms of (4.2).

The original analytic norm (2.3), by itself, does not prove (4.3). Without the marginal factor one can retain an old-cell multiplicity growing as \(L^{4(k-j)}\), which no logarithmic asymptotic-freedom bound can absorb.

#### 4.3 Summation theorem with all coupling costs visible — P as an implication

Assume (4.3), \(a_j\ge c g_j\), and

\[
 Q_k\le \Theta_k g_k r_k.
 \tag{4.4}
\]

Assume the numerical trajectory satisfies the old-scale bound used in CMP119 (2.46), in the form

\[
 \sum_{j\le k}g_j^s\le C_s g_k^{s-6},\qquad s>6.
 \tag{4.5}
\]

Then for every fixed \(\varepsilon>0\) and \(\kappa_0>8+\varepsilon\),

\[
 \eta_\gamma(W_k^{R,\mathrm{bulk}})
 \le C_{\varepsilon}\Theta_k^2
 g_k^{\kappa_0-6-\varepsilon}.
 \tag{4.6}
\]

If the logarithmic factor in (4.3) is absent, one can take \(\varepsilon=0\).

**Proof.** Apply (3.7) to each old scale, use (4.3), and sum. Equations (4.4) and \(a_j\ge cg_j\) give

\[
 \eta_\gamma(W_k^{R,\mathrm{bulk}})
 \le C\Theta_k^2 g_k^2
 \sum_{j\le k}\ell_j^A g_j^{\kappa_0-2}.
 \tag{4.7}
\]

For fixed \(A\) and \(\varepsilon>0\), elementary calculus gives \(\ell^A\le C_{A,\varepsilon}g^{-\varepsilon}\) on a fixed sufficiently small coupling interval. Apply (4.5) with \(s=\kappa_0-2-\varepsilon\):

\[
 g_k^2\sum_{j\le k}g_j^{\kappa_0-2-\varepsilon}
 \le Cg_k^2 g_k^{\kappa_0-8-\varepsilon}
 =Cg_k^{\kappa_0-6-\varepsilon}.
 \tag{4.8}
\]

This proves (4.6). \(\square\)

The bookkeeping is deliberate: two powers can be lost to an old radius proportional to \(g_j\); six more are lost in the available old-scale bound; and two powers return because current free-coordinate derivatives carry \(g_k^2\). A claim of \(g_k^{\kappa_0-6}\) without identifying these three mechanisms would not be a proof. If a different admission or localization argument loses additional fixed powers, those powers must be displayed. The ability to choose \(\kappa_0\) large can absorb any proved fixed loss; it cannot replace a proof that the loss is fixed.

The statement also shows why a common tube and its amplitude must be recorded together. A vanishing tube radius is not necessarily fatal when \(Q_k/r_k\) has the physical normalization in (4.4). Conversely, small values on a domain disjoint from parts of the real cutoff give no Hessian control there.

### 5. Can logarithmic exponents or recentering finish the admission step?

#### 5.1 Choosing exponents before the construction

For a prospective origin-centered tube, suppose a checked choice gave

\[
 \epsilon_{1,k}=c g_k\ell_k^q,
 \qquad P_k=A_1\ell_k^{p_0}.
 \tag{5.1}
\]

Then the ratio of the real window to the analytic radius is exactly

\[
 {g_kP_k\over\epsilon_{1,k}}
 ={A_1\over c}\ell_k^{p_0-q}.
 \tag{5.2}
\]

Thus \(q>p_0\) would provide an eventual strict margin; \(q=p_0\) would require an explicit constant margin; \(q<p_0\) would not work for this particular origin-ball argument.

CMP119 Theorem 1 quantifies the construction parameters existentially and requires all the inherited restrictions. Its (2.28) gives only \(q_0,q_1>1\). A further hypothesis is needed to prescribe \(q_0,q_1>p_0\) while maintaining every restriction in CMP109, CMP116, CMP119, and LFR I–II. Several checked LFR estimates contain a factor \(g_k\) times a fixed polynomial in logarithms, which would tolerate arbitrarily large fixed logarithmic powers. This is consistent with the requirement but is not a check of all restrictions. No exponent choice is asserted here as an already verified construction.

In particular, LFR I's later auxiliary exponent \(p_1<p_0\) and the symbol in CMP119 (3.43) must not be identified simply because they have the same name.

#### 5.2 Recentered tubes

The native-chart lemma and CMP102 Proposition 9 support recentering at an admitted real point. Recentered tubes can avoid requiring an origin radius larger than the entire real support. They must still preserve the actual analytic constraints.

A sufficient complete admission theorem would show, uniformly in all relevant histories and real cutoff points, that for a specified \(r_k>0\), every localized pullback on \(\mathbb D(z,r_k)\):

1. satisfies the original and reconstructed \((U,J)\) conditions at every old layer with a fixed fractional margin;
2. satisfies the local gauge and spatial-derivative bounds, including the required current bounds;
3. remains admissible when all localization/decoupling parameters run over the complex contours used by the source;
4. obeys the current activity bound (4.3), including the old-scale sum and large-carrier tail.

Old-layer gains such as \(L^{j-k}\) in relative fields and \(L^{2(j-k)}\) in curvature are relevant. They do not prove the simultaneous assertions above without tracking the radii and the current norms. In particular, (2.3) is a bound only after this admission has been verified.

### 6. Scope for assembly

| Item | Status |
|---|---|
| Primitive inherited R complex activity norm | L: exact (2.31) verified |
| Generation of superpolynomially small new R activities | L: LFR II (1.100) verified |
| R real marginal factor and old-scale sum | L: CMP119 (2.44), (2.46), proof on p.283; six-power loss |
| Primitive R second derivatives inside an admitted chart | P with L input: (4.1) |
| Current localized R Hessian on every real cutoff point | O: (4.3) and full tube admission remain |
| Current R summation once that premise holds | P implication: (4.6)–(4.8) |
| Complete-history E-bulk bound with fixed \(\epsilon_1\) and fixed prefactor | The fixed-radius, fixed-prefactor import is not justified; use (3.9) until its premises are checked |
| Homogeneous classical-action estimate and exact coarea bound | Unaffected by this radius analysis |
| Fixed-parameter pure CMP109 no-R conditional model | Unaffected within its explicitly stated scope |
| Complete homogeneous RG/R coercivity | Not closed: inherited R remains, and the complete-history E domain import is not justified |
| General-history coercivity and observable hierarchy | Not closed; boundary terms and marked transport remain in addition |

For the regular domains, Annexes AD, AE and AH track the running radii in the current contour and its derivative majorants. Application to the complete conditional representation requires CL, including the heterogeneous boundary terms.

### 7. References

* T. Balaban, **Convergent renormalization expansions for lattice gauge theories**, CMP119 (1988), 243–285, (2.31) and p. 276. The R portion of the proof of Theorem 2 appears on p. 283.
* T. Balaban, **Large field renormalization. I, II**, CMP122 (1989), 175–202 and 355–392. R generation and complex norm at II (1.98)–(1.100). Auxiliary exponent restrictions at I p.183 and II p.383.
* T. Balaban, **Renormalization group approach to lattice gauge field theories. I**, CMP109 (1987), 249–301. [DOI](https://doi.org/10.1007/BF01215223). Fixed-domain quantifiers at p.263; Lemma 4 and radius dependence at p.280.
* T. Balaban, **Renormalization group approach to lattice gauge field theories. II. Cluster expansions**, CMP116 (1988), 1–22. [DOI](https://doi.org/10.1007/BF01239022). The \(\epsilon_1/\alpha_2\) dependence is in (1.21)–(1.24); parameter dependence in the prefactor is discussed after (1.29). Formula (1.43) is not used.
* T. Balaban, **The variational problem and background fields in renormalization group method for lattice gauge theories**, CMP102 (1985), 277–309, Proposition 9. Its recentered analytic minimizer theorem remains an input to the proposed tube argument, not a substitute for admission of every localized activity.

This note makes no claim that four-dimensional Yang–Mills existence or the complete conditional-coercivity obligation has been proved.


---
