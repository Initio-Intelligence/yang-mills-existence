# Conditional assembly of the boundary derivative estimate

**Annex AW.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).

**Scope of the inference.** The endpoint, stopped-prefix and repeated positive carrier estimates on actual all-history data are assumptions in this application. The native estimates cited below apply on their own admitted domains. In particular a derivative of an isolated minimizing map does not establish the derivative of a composed field at fixed older variables.


The following assembly assumes uniform estimates for the same conditional representation, every composed reconstruction and the complete positive repeated-component and stopped-prefix expansions. These assumptions are required at the points where the corresponding endpoint and carrier estimates are used below.

### 1. Statement, conventions and exact scope

Use the source-free representation and current conditional split of C-01, with its actual admitted histories, reference measure and consistently normalized coupling trajectory. For completed replacement components choose the exact alternative representation LFR II (1.103)–(1.104), as specified in Section 2. This is an exact marginalization of their hidden variables with the entire incoming boundary exponential. Work on the current \(k\)-lattice in its unit physical coordinates. Let \(I\) be the independent free bonds integrated in the current regular region, and write \(z=(z_i)_{i\in I}\) for their real Lie-algebra coordinates. Surviving earlier fluctuation variables, retained raw component fields, current-scale exterior variables, selectors and history labels are retained.

Put
\[
 \ell_k=\log g_k^{-2},\quad
 P_k=A_1\ell_k^{p_0},\quad
 \delta_k=g_kP_k,\quad
 \varepsilon_k=A_0g_k\ell_k^{p_0},\quad
 \alpha_k=C_\alpha g_k\ell_k^q,\qquad
 q_0=q_1=q>p_0+r+2.
 \tag{AB17.1}
\]
Here \(r>1\) is the fixed running-collar exponent, \(R_k\asymp\ell_k^r\), with the source rounding convention. Equal native exponents are an allowed fixed choice in CMP119 (2.28); their fixed constants may differ. The stronger inequality includes the real-center enhancement in every preparatory prefix (PF.2–PF.3). The actual real current support is the full unprimed support \(P_k\). Fixed conversions between scalar coordinate norms and the source Lie-algebra norm are included in constants. A current contour denoted \(2P_k\) below means twice a fixed coordinate radius containing that full support; it is not a replacement of the support by the smaller LFR primed cutoff.

The native external field chart is the strong source chart
\[
 \|E\|_{\mathfrak N_{\rm curl}}
 =\sup_n\alpha_n^{-1}\max\{
 h_n|E|,\ h_n^2|\nabla_{U_*}E|,
 h_n^3|D_{U_*}^{*}D_{U_*}E|\}.
 \tag{AB17.2}
\]
Here \(h_n\) is the physical mesh of the actual layer and \(U_*\) the fixed real reference. Independent-current arguments use the common weighted radius of BC16.4, including the embedding of actual inner layers into all earlier primitive conventions. A native direction is measured in these norms. It is not assigned a cutoff-independent radius merely because its raw coordinate value is one.

Let \(B_k^{\rm cur}(z,\xi)\) denote the complete current-dependent boundary perturbation in CMP119 (3.25), including every sector listed in Section 5 below. The symbol \(\xi\) denotes the admitted native external coordinates; old real variables and selectors remain fixed parameters. The current Gaussian precision, its retained cross force and its Schur-complement scalar remain in their exact C-01 roles. Define
\[
 \widetilde B_k(z,\xi)
 =B_k^{\rm cur}(z,\xi)-B_k^{\rm cur}(0,\xi).
 \tag{AB17.3}
\]
The subtracted value remains in the outer marginal. The subtraction changes no current derivative.

#### Theorem AB17.1 — boundary budget under the composed-response and representation hypotheses

Under the stated C-01/source hypotheses, choose the fixed source parameters and common coupling ceiling in the order specified in Section 7. There are a fixed \(\gamma>0\), constants independent of cutoff depth, total volume and admissible history, and a quantity \(\mathcal K_{B,k}\) specified in (AB17.24), such that
\[
 \sup_i\sum_l e^{\gamma\rho(i,l)}
 \|D_iD_l\widetilde B_k\|_{\rm op}
 \le C\mathcal K_{B,k}P_k^{-2}.
 \tag{AB17.4}
\]
Moreover \(\mathcal K_{B,k}P_k^{-2}\to0\) uniformly as the common coupling ceiling tends to zero. Thus the boundary budget can be made smaller than any prescribed fixed share of the source principal coercivity gap.

For \(m\ge1\), a fixed \(\sigma>0\), and the minimum connecting-tree length \(\tau\) of the current positions,
\[
 \sup_{i_1}\sum_{i_2,\ldots,i_m}
 e^{\sigma\tau(i_1,\ldots,i_m)/m}
 |D_{i_1}\cdots D_{i_m}\widetilde B_k|
 \le C^{m+1}(m!)^5\mathcal K_{B,k}P_k^{-m}.
 \tag{AB17.5}
\]
Every finite mixed native jet exists on the common smaller external chart. For native directions \(h_1,\ldots,h_r\), the right side can be multiplied by
\[
 C^r r!\prod_{s=1}^r
      \frac{\|h_s\|_{\rm native}}{r_{\rm ext}},
 \tag{AB17.6}
\]
where \(r_{\rm ext}>0\) is the fixed radius actually retained by the joint construction. Further nonlinear pullbacks to arbitrary retained data retain their full higher chain-rule terms; (AB17.6) is not a claim about differentiating selectors or old cutoffs.

The physical current jets are derivatives of the exact reduced real density. The mixed native jets are derivatives of the explicitly specified compatible analytic extensions: each agrees with its physical expression for the entire real current family at fixed admitted retained physical data. An off-minimum formal background is not asserted to be a constrained minimum or to satisfy every identity of a different off-physical extension. A later pullback to moving physical retained data must keep all of its higher chain-rule terms.

The proof uses the direct primitive one-endpoint method of BC16. It does not import the unidentified \(p_1(g_k)\) in CMP119 (3.43), nor require a new identity for arbitrary prepared joined minimizers.

### 2. The outer operator and the current conditional density

CMP119 (2.19)–(2.23) states that \(T_k\) is supported in the old large-field region \(Z_k\), factorizes over its components, and contains the retained older integrations, their cutoffs, gauge constraints and within-component old Gaussian pieces. The present free current is supported in \(\Lambda_{k+1}\). The source constructs \(\Omega_{k+1}\), and then \(\Lambda_{k+1}\), beyond several current-size cube layers surrounding \(Z_k\); see (3.2)–(3.5) and (3.20).

The current substitution is the literal source map
\[
 I_k(A)=\exp i[g_kCA-hD(g_kCA)]\,V^{(k)}.
 \tag{AB17.7}
\]
The one-step constraint map \(C,hD\) has its stated block locality. Its fixed enlargement of the inner support stays inside the buffer and does not change the directly retained coarse data on \(Z_k\). This fact does **not** prove that every coefficient of \(T_k\), when written through the full background, is independent of the current. A prose factorization cannot supply a missing coefficient identity.

The issue is visible already in CMP119 pp.253–254: the old Gaussian precision and its Schur covariance depend on \(U_1\). The later R-modified operator is written explicitly as \(T'_k(X,(U,J))\) in LFR II, pp.379–380. Its old integration support alone does not eliminate this dependence. The nodal identity (AB17.11) changes no integration variables, so it does not itself remove such responses.

The following three source cases exhaust that older response.

#### 2.1 Ordinary unreplaced Gaussian operations

On fixed free coordinates put \(G=K_{II}^{-1}\),
\(S=K_{OO}-K_{OI}GK_{IO}\), and
\(\mathcal E a=(-GK_{IO}a,a)\). The exact old retained exponent and its variation are
\[
 q(U,J,a)=-\tfrac12a^{\mathsf T}Sa,\qquad
 dq=-\tfrac12(\mathcal E a)^{\mathsf T}(dK)(\mathcal E a).
 \tag{AB17.7a}
\]
The latter identity includes the covariance derivative; its cancellation with the variation of the harmonic extension is proved algebraically in OR17.4. The actual \(K=C^*\Delta^{(j)}C\) includes the source constraint-current correction. CMP99's localized inverse/walk expansions provide local coefficient dependence as well as off-diagonal decay. Thus the common-disc argument applies to each actual quadratic carrier with value prefactor \(CP_j^2\), not an abstract background-independent precision.

Theorem OR17.1 proves the resulting complete ordinary response bound
\[
 \mathcal K^{\rm G}_{T,k}
 \le C\theta_kP_k^2e^{-c_{\rm G}MR_k},
 \qquad \theta_k=\ell_k^{p_0-q}.
 \tag{AB17.7b}
\]
Old raw Haar, raw averaging delta and selector factors depend on their actual retained local data and are constant under the new inner current. Earlier Gaussian determinant normalizations are already assigned to E/vacuum terms by the source; they are not omitted or counted a second time. The fixed old-field nodal argument applies to the two endpoints of each quadratic scalar carrier.

#### 2.2 Preparatory prefixes and failed branches

Use every actual prefix determining history in LFR I (1.15)–(1.16), not only the final completed prefix. PF.1 proves a simultaneous ordinary native core inside the modified domains (1.64)–(1.69). The real-center enhancement
\(L_0^{2N_0}\le C N_0^{\beta_0}R_b\) is paid by the fixed choice in (AB17.1).

Apply the ordinary response proof to each actual prefix principal constraint/Schur block on that admitted history. Its coefficient is still \(C^*\Delta C\), with the same current correction, and its principal inverse is the actual one used at that prefix. The CMP99 localized coefficient, principal-inverse and complex-domain results are uniform on the admitted determining class; they do not require that the history be homogeneous or unprepared. PF.1 supplies precisely that class and the common strong core, including its real-center check. Retained ordinary fluctuation variables obey \(CP_t\); the newly failed variable is bounded by \(6\delta'_t/g_t\ll P_t\). Thus OR17.4 and the \(CP_t^2\) primitive majorant apply without freezing a prefix covariance. For the recent one-\(M\)-layer prepared collars, retain the fixed \(\delta M\) age reserve as in CR.22b, not an unprepared \(RM\) factor. The source block order places the fixed propagator collars inside these admissible blocks before the common ceiling is chosen. PF supplies the remaining selector, domain and relocation changes, while this prefix version of the ordinary response supplies its remaining quadratic coefficients.

The failed-selector displacement uses the exact boundary-supported data in (1.56). Its selected formal extension has zero displacement for zero data. PF.2 admits its actual mixed-data localized background on the primary absolute chart and retains the source collar
\[
 D_{b,t}=10M\sum_{s=t+1}^{b-1}R_s+MR_b.
 \tag{AB17.7c}
\]
The displacement and all its current/native responses carry \(e^{-cD_{b,t}}\). The supported extension agrees with the actual relocation for every real current at fixed retained physical data. It is not asserted to equal an arbitrary two-average difference on every off-minimum native background.

The hard selectors become functions of retained real component data after (1.59); they are not differentiated. The failed branch retains the **whole** action difference and its logarithmic coordinate Jacobian. This old failed Jacobian depends on a future current and does not cancel. PF.14–PF.21 bounds it explicitly. The potentially large number of shifted fine coordinates is
\(C(MR_b)^4L^{4(b-t)}\); (AB17.7c) pays that factor and the prefix sum. In the action difference use the angular coordinate \(\beta=g_ta\): its derivative has cost at most \(Cg_b^{-3}\ell_b^A\), while \(\Delta\beta=O(\alpha_b e^{-cD_{b,t}})\). This yields the stated \(g_b^{-2}\) coefficient, including all coupling factors.

The action difference is quasi-local. Its inherited carrier connector and the future endpoint path are kept together, as in PF.20a; it is not replaced by a compactly supported scalar. The resulting absolute fresh coefficient and current endpoint obey
\[
 \varepsilon_b^{\rm PF}
 \le Cg_b^{-2}(1+\ell_b)^{A_F}e^{-c_FR_b},
 \qquad
 |\partial_iF_{b,Z}^{\rm PF}|
 \le \frac{C\theta_k}{P_k}
 (1+k-b)^Be^{-\Gamma(k-b)}
 \varepsilon_b^{\rm PF}e^{-c d_k(i,Z)}.
 \tag{AB17.7d}
\]
This includes failures at intermediate stages, their retained older ordinary operations, and the selectors localized by their actual relocation. A whole-component geometric promotion alone would not have established it.

#### 2.3 Completed replacements: exact integration before the next current split

For each completed component operation use the literal alternative on LFR II pp.391–392:
\[
 \prod_Y T'_b(Y)\,e^{B_{\rm in}}
 =\prod_Y\tau_Y\,
       \left[\prod_Y\Pi_Y\,e^{B_{\rm in}}\right],
 \quad
 \tau_Y=T'_b(Y)1,\quad
 \Pi_Y=\tau_Y^{-1}T'_b(Y).
 \tag{AB17.7e}
\]
The bracket integrates the **entire** incoming boundary exponential. Its convergent scalar logarithm is part of the new boundary action. The source proves that each remaining \(\tau_Y\) depends only on the raw \(V_b|_Y\) and explicitly excludes it from the next renormalization step. This assertion is used only for that completed scalar mass; it is false for the earlier pointwise kernel \(T'_b(Y,(U,J))\).

The equality is an equality of reduced measures after those hidden variables have been integrated, not pointwise equality at every old hidden coordinate. The unintegrated real variables of ordinary or failed branches remain present. All canonical masses and their normalizations are kept. No old self term is moved into a mass to simplify the argument.

The source output loses full-tree coverage inside retained eligible components. The proof in Annex AU retains the actual outside-tree and outside-volume reserves, the normalized-operation factors, and the polynomial attachment cost of each fixed component. Its two rooted connected sums establish a full-\(\kappa\) absolute carrier norm. The small fresh coefficient follows from the **final printed** (1.68) on its completed carrier, with a fixed source/analysis-rate split:
\[
 \varepsilon_b^{\rm R}
 \le C(1+\ell_b)^A e^{-c_{\rm R}R_b}.
 \tag{AB17.7f}
\]
It is not inferred by assigning the newly added completed halo to an earlier pre-carrier estimate.

For later steps keep each untouched activity's original birth anchor, original holes and fixed absolute majorant. Promotion affects future cluster incidence, not old record norms. Source terms whose variables or sole boundary tag are consumed enter the exact fresh output or the primary new-history full-tree reference classification; no nonexistent old anchor is retained. The actual source support classification is distinct from the new quantitative bound.

The uniform repeated bound is chronological. Earlier resident completed masses have births at most \(h=b-N(b)\); scalar tails born outside at intermediate scales retain their carrier connectors. They feed PF before the same-birth completed output is constructed. With \(F_0\ge1\) the fixed ordinary source norm, and with original birth-majorant norms \(A_{j,b}\), CR.22–CR.25 proves
\[
\begin{split}
 \mathcal A_b&=\sum_{j\le b}e^{-\lambda(b-j)}A_{j,b},\\
 \zeta_b&=\varepsilon_b^{\rm R}(1+R_b)^s
                     +\varepsilon_b^{\rm PF},\\
 \mathcal A_b
 &\le (e^{-\lambda}+C\zeta_b)\mathcal A_{b-1}
                         +CF_0\zeta_b,\\
 \mathcal A_b&\le
 \mathcal A_*:=
 \frac{CF_0\sup_j\zeta_j}{1-\rho},
 \qquad \rho=\tfrac12(1+e^{-\lambda})<1,
\end{split}
 \tag{AB17.7g}
\]
after \(C\sup\zeta\le(1-e^{-\lambda})/2\). There are no initial completed families. In particular \(\mathcal A_*\to0\) with the common ceiling. The value-age estimate needed in this recurrence uses the old-tree and first-nonempty localization factors of source (1.66), not a future observable derivative. Recent prepared layers have one \(M\)-cell collars, so its fixed rate is supplied by \(\min(\beta\kappa,\delta M,\kappa_1-1)\), not by a fictitious \(MR_b\) guard. The growing \(R_b\) is used separately in (AB17.7f).

Raw fields surviving this integration are held real and fixed in the native extension. CR.2 extends the nodal construction to both raw bond endpoints, using actual raw endpoint covariance. Fine hidden raw fields inside the completed operation have already been integrated and require no pointwise complex-gauge claim.

#### 2.4 The full older-density budget

Combining OR17.1, PF.21–PF.22 and CR.3/CR.25 gives the finite sufficient bound
\[
 \mathcal K_{T,k}\le
 C\theta_k\left[
    P_k^2e^{-c_{\rm G}MR_k}
       +\mathcal A_*+\varepsilon_*^{\rm PF}\right],
 \qquad
 \varepsilon_*^{\rm PF}:=\sup_b\varepsilon_b^{\rm PF}.
 \tag{AB17.7h}
\]
Every scalar contribution is assigned once in the actual density; this nonnegative upper bound can conservatively cover a prefix term both directly and in the forcing of a later scalar norm. It does not duplicate a term in the action. The carrier/age sums and the current guard pay each polynomial component attachment cost. There is no total-volume factor. Both \(\mathcal A_*\) and \(\varepsilon_*^{\rm PF}\) tend to zero because \(r>1\). Hence
\[
 \mathcal K_{T,k}P_k^{-2}
 \le C\theta_k\left[
 e^{-c_{\rm G}MR_k}
   +P_k^{-2}(\mathcal A_*+\varepsilon_*^{\rm PF})\right]
 \longrightarrow0 .
 \tag{AB17.7i}
\]

Older cross-component Gaussian terms which the source already assigned to B remain in the primitive B sector. The present cross term \(z^{\mathsf T}K_{IO}a\) is different: it stays in the conditional Gaussian mean. Its force need not be small. Current exterior relocation changes that retained force and scalar, but not the current-current precision block.

If marks are present, (AB17.7e) transports their numerators through the same positive conditional operation. The exact quotient identity preserves their integrals. It does not establish local bounds for those transported marks; H-03 and the later observable hierarchy remain separate obligations.

### 3. A common contour obtained from the actual maps

#### 3.1 Original map and actual gauge family

Fix the symmetric raw averaging operation CMP109 (0.11)–(0.12), and use its own associated corrected relative average and inverse-axial gauge. The selected original nonlinear source family is the one used in E14.3, CMP102 (179)–(180) and CMP116 (1.17). Its formal extension at an arbitrary native background is not called a physical minimum. CMP102, pp.307–309, supplies the associated gauge conversion and the stated extension of this analytic family.

BM.10–BM.11 retain the original-geometry value, gradient and current kernel rows, with their actual physical measures and weighted source distance. JI.32–JI.40 and RM.26–RM.36 apply the inverse-axial gauge to this same family. In particular the nodal response uses the actual fine gauge restricted to coarse grid sites, not its iterated gauge mean.

Write
\[
 \theta_k=\ell_k^{p_0-q}.
 \tag{AB17.8}
\]
The source kernel rows and AF comparison give, for the current insertion on the full fixed multiple of \(P_k\), a normalized layer response bounded by
\[
 C\theta_k(1+k-n)^b e^{-\Gamma_0(k-n-c_0)_+},
 \tag{AB17.9}
\]
with fixed \(b,c_0\). Its marked one-coordinate version is the same expression divided by \(P_k\), with a retained spatial endpoint exponential. All exponents below are reduced fixed shares of the original endpoint decay. The source row sums, rather than an unnormalized sum over fine bonds, are used in (AB17.9).

For a native background increment of radius \(r_{\rm ext}\), the same original-family bounds add \(Cr_{\rm ext}\) to the local normalized strong size. This parameter is selected small once. Thus the entire smooth source family, including the fixed real exterior current and its shift discussed below, has normalized size
\[
 C(\theta_k+r_{\rm ext})
 \tag{AB17.10}
\]
inside one strong chart. The absolute internal analytic domains are admitted first: \(g_kP_k\), \(\alpha_k\), and all their fixed parameter multiples tend to zero. Only afterward is the smaller running primitive radius tested.

#### 3.2 Primitive B domain and all older slots

NP.5 proves a genuine strong ball inside all U-dependent restrictions (2.34)–(2.39), including the actual joined reconstructed field/current predicates. Its proof uses the zero-relative-data variational projection on the actual admitted geometry, followed by the bounded actual gauge converter. The second-order input row is (AB17.2); a first derivative of a domain predicate is not used as a certificate.

For each primitive \(B^{(j)}(X)\), use the nodal gauge interpolation AD17.3 only on its actual earlier fluctuation slots. For scalar families after completed integration, CR.2 additionally includes both endpoints of every retained raw bond used by that primitive. Ordinary old fluctuation nodes lie within a fixed range of their one-step mesh; surviving raw endpoints satisfy the one-sided grid-to-local-grade relation CR.8. The admitted graded geometry, including the R-rebuilt history, supplies disjoint interpolation balls with radii fixed multiples of those local meshes. Repeated nodes are merged, and each uses the same actual fine-gauge value. Fixed real local regular gauges are used on each ball.

If \(U_{\rm L}=U_{\rm AX}^u\), the interpolating gauge \(v_X\) matches \(u\) at the old bond basepoints on which that primitive depends. On real parameters, the two exact source covariance identities give
\[
 B^{(j)}(X,U_{\rm AX},J_{\rm AX},\mathbf A)
 =
 B^{(j)}(X,U_{\rm L}^{v_X^{-1}},
             \operatorname{Ad}_{v_X^{-1}}J_{\rm L},\mathbf A).
 \tag{AB17.11}
\]
The last expression has fixed older fields. The analogous identity for a raw bond uses both endpoint factors, which are canceled by the same nodal matching. Its native field/current arguments lie in the NP.5 ball by (AB17.10) and the fixed reserve (AD17.28). It defines the holomorphic extension of the actual real pullback and therefore all its physical jets. No analytic extension in arbitrary complex older \(A_j\) or arbitrary complex retained raw links is required.

AD17.24–AD17.27 show that its one-current tangent has the same normalized endpoint estimate as (AB17.9). The curl row follows from exact current covariance and the local action-chart identity; a third derivative of an interpolated gauge potential is not assumed. The interpolation changes carrier and endpoint constants only by fixed factors. It introduces neither a fine-spacing factor nor a sum over all earlier fields.

#### 3.3 Independent currents and native directions

Use the common independent-current profile of BC16.21–BC16.23. Its fixed embedding constant includes every older primitive's innermost-region convention. Under the gauge conversion the auxiliary current is co-transformed with the physical current. The triangular extension
\[
 J_{\rm aux}=J_{\rm phys}(\Phi)+\zeta
 \tag{AB17.12}
\]
has a fixed uniform slack after the common norm comparison. On \(\zeta=0\) it is the original physical expression, so its physical jets agree exactly. Derivatives in \(\zeta\) are additional admitted native derivatives, not omitted chain-rule responses of \(J_{\rm phys}\).

The field/current argument lists are finite at each cutoff, with uniform sup-type norms. Taking a simultaneous ball in those norms, not one shrinking radius for each old scale, avoids a factor proportional to the number of layers.

For clarity, a raw unit field coordinate \(\delta E\) on a fine bond in layer \(n\) has at worst the explicit native cost
\[
 C\alpha_n^{-1}
 \max\{h_n,\ h_n^2/\eta,\ h_n^3/\eta^2\}.
 \tag{AB17.13}
\]
The \(\eta^{-1},\eta^{-2}\) come from its finite-difference stencil. A raw unit link-angle direction has the additional conversion \(E=\eta^{-1}\delta(\text{link angle})\). Neither is called a uniformly bounded native direction. The actual current-coordinate tangent is smooth at the physical layer scale by the source kernel, which is why (AB17.9) has no such fine-mesh loss.

### 4. The complete exterior relocation on this contour

#### 4.1 Exact composition and Jacobian cancellation

AD17.2 proves that the source relocation acts only on the retained current-scale exterior coordinates \(a\), with
\[
 a'=\mathcal R(a;H^{(k)}),\qquad
 g_k\mathcal R_b(a;H)
 =\frac1i\log\{\exp(ig_ka_b)\exp[-i\chi_b(a_b)H_b]\}.
 \tag{AB17.14}
\]
The smooth real cutoff \(\chi_b(a_b)\), and the derivatives entering its real Jacobian, are fixed coefficients in the native complex continuation. The displacement and Jacobian are independent of \(z\). The Jacobian cancels exactly from the normalized inner law and remains in the outer marginal.

We estimate each sector of the **entire relocated action**
\[
 F_X(z,\xi)
 =b_X\bigl(\Phi(I_k(z,\mathcal R(a;H^{(k)}(\xi))),\xi),
                      \mathbf A\bigr)
 \tag{AB17.15}
\]
directly. There is no Taylor truncation in the exterior displacement. In particular every term in the source's \(V^{(k)}\) is retained, either in this exact shifted action or in the outer Jacobian. The nonlinear \(C,hD\) dependence in (AB17.7) is retained to all orders.

#### 4.2 Only a coarse native bound on the relocation field is needed

For actual real backgrounds the source gives
\(|H^{(k)}|\le C\varepsilon_ke^{-R_k}\). We do not assume that exponential estimate on an arbitrary off-minimum native ball. The sufficient uniform bound for the present continuation is instead
\[
 |H^{(k)}(\xi)|\le C\varepsilon_k+C r_{\rm ext}\alpha_k,
 \qquad
 g_k|a'|\le D_k:=C(\varepsilon_k+r_{\rm ext}\alpha_k).
 \tag{AB17.16}
\]

To verify it, use the actual two specified current-scale averages and gauges in CMP119 (3.22), with their own real reference values. The input native field has strong size \(r_{\rm ext}\alpha\). NP.13 bounds the **smooth relative Landau** correction of each actual localized reconstruction. Cauchy on its genuine NP.5 ball bounds its change from the real reference by \(C r_{\rm ext}\alpha\) in the corresponding local weighted rows. We do not claim a small fine axial potential from a bounded gauge.

Instead apply exact raw averaging covariance. If the source reconstructed representative is \(W=L^t\), then
\[
 M^k(W)(x,x')=t(x)\,M^k(L)(x,x')\,t(x')^{-1}.
 \tag{AB17.16a}
\]
The smooth factor \(L\) has the forward averaging estimate of NP.4. The **relative** change of \(t\) from its real value has the RM/JI bound
\(Ch_s(\|\delta A_{\rm L}\|+\|\delta E\|)\), not merely a bound on \(\|t\|\). The fixed reference gauge factors are unitary. The old physical layers reached by the actual \(k\)-averaging footprint are current or fixed adjacent layers, so the combined coarse increment is \(C r_{\rm ext}\alpha_k\). Joined localization collars may have \(h_s\ll h_k\); NP.13 gives \(h_s^2w_{\rm old}\) there and the factor \(h_s\) in the gauge response only improves this estimate. No fine collar is removed from the argument.

At the real reference the ratio of the two source averages has its stated \(O(\varepsilon_ke^{-R_k})\) size. Their separate relative changes just estimated keep that ratio in one fixed logarithm chart. This proves the first inequality in (AB17.16), conservatively retaining \(C\varepsilon_k\). The local logarithm product in (AB17.14) is bounded by the sum of its small arguments; the original retained real exterior field obeys \(g_k|a|\le C\varepsilon_k\) from (3.14). This proves the second inequality.

Since \(D_k\le Cg_k\ell_k^q\), the shifted exterior field remains in every fixed absolute internal-map domain after the common ceiling is reduced. It need not stay inside the real current cutoff \(P_k\), because it is a retained parameter on this complex native contour. The integrated current still has the entire \(2P_k\) contour.

For the regular E/R arguments, the original absolute-map admission and running-radius comparison are repeated with
\[
 \frac{g_kP_k+D_k}{\alpha_n}
 \le C(\theta_k+r_{\rm ext})
       (1+k-n)^b
 \tag{AB17.17}
\]
before the same age kernel is applied. This is a fixed-fraction admission when \(r_{\rm ext}\) is chosen first and \(\theta_k\) made small. Thus the shift is accommodated by their existing native domains, not by pretending that the E14 \(2P_k\) current cube already bounded every complex exterior coordinate. The regular primitive value bounds and Ward subtractions remain exactly those used in C-04.

The first current response of (AB17.15) has no derivative of \(H^{(k)}\) or \(a'\) with respect to \(z\). The differentiated original map at the shifted datum has the same uniform endpoint row on its admitted absolute contour. All higher current responses are obtained by Cauchy from that full composition, so its second and higher nonlinear coordinate derivatives are included.

### 5. The complete sector majorants

The ledger is the exact exponent C-01 (3.11), followed by the exterior change (3.12), and the source B assignments in CMP119 pp.276–277. No sector is inferred from a determinant calculation alone.

| Sector | Function estimated and quantitative input |
|---|---|
| Inherited B, including old Gaussian terms assigned to B | The primitive full-tree bound CMP119 (2.42), pulled back through (AB17.11), on NP.5's genuine ball. |
| E/R expressions assigned to the current boundary | The actual layerwise E/R majorants and subtractions of C-04/C-03, restricted to the source's boundary-assigned subfamilies. The shift is admitted by (AB17.17). |
| Homogeneous nonlinear classical and nonlinear-constraint remainder | The complete source remainder after its actual constrained quadratic part; CMP116 (1.37)–(1.43), transferred to the actual multiscale operators by CMP119 p.276. |
| Haar and current constraint/coarea factors | The analytic current coordinate density in C-01 (3.6), with its constant factor (3.6a) kept outside the normalized current law. |
| Ordinary older Gaussian/Schur response | The exact covariance/precision response (AB17.7a), with local normalized walk expansions and prefactor (AB17.7b). Raw/delta/selector factors use their actual retained local data. |
| Intermediate preparatory and failed branches | Every prefix native chart, the boundary-supported failed relocation, its full action difference and its noncanceling future-current Jacobian; (AB17.7c)–(AB17.7d). |
| Completed R operations and surviving raw multipliers | The exact whole-boundary integration (AB17.7e); full-rate relative-carrier majorants, the chronological bound (AB17.7g), and the raw endpoint extension. The canonical raw masses stay fixed. |
| Heterogeneous Wilson coefficient | The exact difference \(A(w_k-g_k^{-2},\Phi(z))-A(w_k-g_k^{-2},\Phi(0))\), with the local recursion (2.24), its transition cutoff collars and the fine-cell estimate BC15.1. |
| Entire exterior relocation | Every preceding row evaluated at \(a'\); the exterior Jacobian cancels only in the inner conditional quotient by AD17.2. |

#### 5.1 Inherited B

For a primitive at age \(a=k-j\), (2.42) gives
\[
 K_X=B_0e^{-\kappa d_j(X)}.
 \tag{AB17.18}
\]
NP.5 and AD17.3 provide a fixed native directional disc at every point of the common current contour. The actual one-endpoint tangent, (AB17.9) and (AD17.27), gives a first-current derivative bounded by the primitive value divided by that fixed native radius, times the tangent norm.

When an attachment is in a layer \(n\le j\), the original kernel pays the full age \(k-n\). The ratio \(g_kP_k/\alpha_n\) has at most a fixed polynomial age cost times \(\theta_k\). Summing these earlier layer restrictions costs another fixed polynomial.

When \(n>j\), the kernel pays \(k-n\). The full primitive tree, which meets \(Z_j\), must connect the attachment to that old boundary. Grading of the actual \(\Omega\)-history makes its old-\(j\) length at least \(cL^{n-j-c_0}\), apart from fixed adjacent-level conventions. A fixed part of its exponential can therefore pay any prescribed finite rate times \(n-j\), leaving a positive full-tree reserve. This is the explicit path/carrier split of BC16.5. It is not a claim that the original kernel alone pays age \(k-j\) at such an attachment.

The resulting first-current bound has the BC16 form
\[
 |\partial_iF_X|
 \le
 \frac{C B_0\theta_k}{P_k}
 (1+a)^{b_B}e^{-\Gamma a}
 e^{-\kappa' d_j(X)}e^{-c d_X(i)}.
 \tag{AB17.19}
\]
Here \(d_X(i)\) is current-unit distance to the physical carrier, with a fixed collar enlargement from the termwise nodal interpolation. The normalized original kernel rows and the actual carrier tree are both retained. The coupling/volume constants do not hide a carrier-to-current distance.

#### 5.2 Boundary-assigned E and R

The C-04 regular contour proof and the C-03 R proof supply the complete layerwise primitive sums
\[
 \mathfrak K_E,\qquad C_Rg_k^{\kappa_0-11},
 \qquad \kappa_0\ge12.
 \tag{AB17.20}
\]
Their analytic input is the admitted running native field/current class. Equation (AB17.17) verifies that class after the exact exterior shift, with the same fixed fraction of reserve. Thus their Ward subtractions and old-index summations are not changed.

CMP119 p.276 first performs those estimates on each actual physical layer, then assigns the boundary-crossing localizations to B. Taking the absolute majorant of that subfamily does not increase the already summed regular majorant. In particular carriers meeting the newest boundary use (AB17.20) directly. No old-\(Z_k\) collar factor is asserted for them. Remote older-layer pieces retain the original endpoint kernel and are summed with its age reserve as in Section 6.

Scalar gauge invariance of these E/R primitives permits their smooth-family analytic extension without an old-field rotation. Their original exact subtractions, including the E coupling counterterm, remain present. They are not replaced by an unrenormalized vacuum bound.

#### 5.3 Classical, constraint and measure remainder

The source constrained Hessian is the Gaussian precision of C-01 (3.8). In particular the quadratic background-current contribution from nonlinear constraint elimination is already in that Hessian. The classical remainder starts at third order in the unscaled current argument; the selected formal extension preserves this source decomposition.

CMP116 (1.39) gives its localized cubic bound, and (1.40)–(1.43) supplies the local coefficient representation. The neighboring argument says the other classical terms have the same bounds. With the actual full unscaled input bounded by \(D_k+2\delta_k\), enlarge \(D_k\) by a fixed factor and obtain
\[
 K_{\rm cl,k}\le Cg_k^{-2}D_k^3.
 \tag{AB17.21}
\]
The localization polynomial in carrier size is paid by a fixed share of the source exponential. The absolute current domain \(\epsilon_{\rm abs}/g_k\) is admitted because \(D_k\to0\). No identification of the \(p_1\) in (3.43) is used.

The Haar and coarea logarithms are analytic in the same small unscaled arguments; after their fixed normalization at zero their conservative localized bound is \(CD_k\). Their higher constraint-map and density derivatives are covered by the same common analytic contour. These functions use the original current-coordinate map, not an ad hoc affine fluctuation.

The exact shifted classical function has induced linear and quadratic terms in \(z\), even though the unshifted remainder starts cubically in the full field. They are included in (AB17.21) by evaluating the full cubic analytic remainder at \((z,a')\). They are not set to zero by the word “remainder.” The current-current Gaussian block is left unchanged, and its separate shifted cross force is retained.

#### 5.4 Heterogeneous coefficient, including transition collars

Let \(w_l=g_l^{-2}\). The exact recursion gives
\[
 w_k(x)-w_k
   =\sum_{l=1}^k(w_{l-1}-w_l)(1-\phi_l(x)).
 \tag{AB17.22}
\]
No sign of \(w_{l-1}-w_l\) is assumed. If a point is on actual layer \(n\), the safely sufficient bound is
\[
 |w_k(x)-w_k|
 \le Cg_k^{-2}\bigl(1+k-n+\log\ell_k\bigr)^{b_\phi},
 \tag{AB17.23}
\]
with one fixed \(b_\phi\). The slightly weaker logarithmic factor here avoids silently identifying the earliest active cutoff index with \(n\).

Here is the cutoff-geometry verification. A nonzero \(1-\phi_l\) lies outside the prescribed plateau of \(\Lambda_l\), hence within at most one fixed localization collar of \(Z_l\). Its physical width is bounded conservatively by \(CMR_lh_l\); using the smaller source \(M\)-cell convention only improves the bound. For \(l<n-1\), interlacing gives \(Z_l\subset\Omega_{l+1}^{c}\). The admitted separation of \(\Omega_n\) from \(\Omega_{n-1}^{c}\) then forces
\[
 L^{n-l}\le C R_l
\]
whenever that collar reaches layer \(n\). The AF comparison gives
\(\ell_l\le\ell_k+C+\log(1+k-l)\), and the definition of \(R_l\) gives
\(R_l\le C\ell_l^r\), including its fixed rounding factor. It follows that the number of possible extra older indices, and their ages \(k-l\), are bounded by a fixed polynomial in \(1+k-n+\log\ell_k\). For instance absorb \(c\log(1+k-l)\) into half of \(k-l\) to obtain
\(k-l\le C(1+k-n+\log\ell_k)\).
The remaining indices \(l\ge n-1\) already have age at most \(1+k-n\). Bound
\(|w_{l-1}-w_l|\le w_{l-1}+w_l\le C(1+k-l)w_k\) and sum. This proves (AB17.23), without any unrecorded equality of cutoff and geometric layers.

The source \(k+1\) collar is formed around \(Z_k\) before the current support is chosen. Here the geometric constant can be checked, rather than left as an arbitrary \(C\). The cutoff plateau costs at most one \(MR_l\)-cube layer at its own mesh. Choose the small AF comparison parameter \(\beta_0>0\) so that
\[
 B_{\rm AF}:=(1+\beta_0)2^{\beta_0}\le5/4.
 \tag{AB17.23a}
\]
Using (2.7) with the fixed power \(r\), then the rounding \(R_l<L\ell_l^r\), gives for \(a=k-l\ge1\)
\[
 \frac{R_lh_l}{R_kh_k}
 \le L^{1-a}(1+\beta_0)(1+a)^{\beta_0}
 \le B_{\rm AF}.
 \tag{AB17.23b}
\]
The last expression decreases for \(a\ge1\) after, for example, \(\beta_0\le1/4\); for \(a=0\) the ratio is exactly one. The adjacent version also gives
\(LR_{k+1}\ge R_k/B_{\rm AF}\).

Since \(Z_l\subset Z_k\), the union of all the older cutoff collars is contained in the \(B_{\rm AF}MR_kh_k\)-neighborhood of \(Z_k\). CMP119 p.265 surrounds the compatible cube cover of \(Z_k\) by **four** \(LMR_{k+1}\)-cube layers before the first new decomposition; subsequent steps remove further layers before choosing the current free support. Already those four layers give distance at least \(4MR_kh_k/B_{\rm AF}\). Subtracting the entire old cutoff collar leaves
\[
 \left(4/B_{\rm AF}-B_{\rm AF}\right)MR_kh_k
 \ge (39/20)MR_kh_k.
 \tag{AB17.23c}
\]
Fixed block footprints and plaquette/star conventions subtract only a fixed \(C_{\rm foot}LMh_k\). Taking the common coupling ceiling small enough that \(R_k\ge 2C_{\rm foot}L\) leaves a positive \(MR_kh_k\) collar. This also covers the source p.277 shorthand which places the coefficient in \(Z_k\): the proof here has allowed the actual one-layer cutoff transitions rather than dropping them. No unverified equality between a transition index and the geometric layer is used.

The one-current variation of the smooth plaquette field therefore retains
\(e^{-c_{\rm col}R_k}\), together with the age and spatial endpoint shares. In dimension four, BC15.1 bounds the plaquette-action difference by the product of two curvature-scale factors. Its fourth power of the fine spacing cancels the number of fine plaquettes in a proper-scale cell. The coefficient (AB17.23) consequently yields the summed prefactor
\[
 K_{\rm het,k}
 \le Cg_k^{-2}\delta_k
       (1+\log\ell_k)^{b_\phi}e^{-c_{\rm col}R_k}.
\]
The omitted fixed age polynomial is included in the convergent age sum below. A bound on an individual link without the curvature-square cancellation would not justify this estimate. The running \(g_k^{-2}\) is paid by the actual growing collar \(R_k\ge\ell_k^r\), not by a fixed number.

#### 5.5 Total prefactor

The entire relocation has already been included by shifted evaluation in every row. Its exterior Jacobian has zero current contribution. Thus a sufficient total prefactor is
\[
 \boxed{\displaystyle
 \mathcal K_{B,k}
 \le C_{\rm src}(1+S_{b,\Gamma})\!
 \left[
  \mathfrak K_E+C_Rg_k^{\kappa_0-11}
  +B_0\theta_k
  +g_k^{-2}D_k^3+D_k
  +g_k^{-2}\delta_k(1+\log\ell_k)^{b_\phi}
                      e^{-c_{\rm col}R_k}
  +\mathcal K_{T,k}
 \right].}
 \tag{AB17.24}
\]
Here \(S_{b,\Gamma}\) is the finite age sum in Section 6. The last summand is the proved explicit older-density budget (AB17.7h); it is not an outstanding premise. Every summand retains the full exactly shifted action. The conservative bound does not demand an exponential current-exterior relocation estimate on an arbitrary native background.

### 6. Spatial/age summation and all derivative orders

The exponential allocations are made once, before differentiation. For inherited B, combine the current-to-attachment kernel path with a path inside the full primitive carrier to \(Z_j\). The connector inequality is BV.6:
\[
 d_\Omega(i,\partial_{\rm in}\Lambda_j)
 \le d_\Omega(i,y)+C_Md_j(X)+C_{\rm edge}.
\]
Use separate positive shares for the current collar where required, the age, the normalized kernel/carrier sum, and the final current-distance decay. The passage \(n>j\) is paid as in Section 5.1. The actual distance is the weighted source distance, with layer weight \(h_n^{-1}\); it is not replaced by distance divided by the oldest mesh.

CMP96 (2.46)–(2.59), as given in BM.1 and Supplement AF.3, charges one fixed \(RM\) separation per complete layer transition. After retaining the source entropy reserve, choose the fixed separation so that the remaining age rate obeys
\[
 \Gamma>4\log L+\log2+2.
 \tag{AB17.25}
\]
The extra \(\log2\) is harmless here because the strong-center proof uses a fixed native reserve rather than the older dyadic reserve; retaining it also covers the conservative prior bookkeeping. At fixed age the number of earlier-layer restrictions and coefficient costs is a fixed polynomial. A conservative old-root density factor is \(L^{4a}\), so
\[
 S_{b,\Gamma}
 =\sum_{a\ge0}(1+a)^b
       e^{-(\Gamma-4\log L-\log2)a}<\infty.
 \tag{AB17.26}
\]
This is a sum with an anchored spatial kernel. It is not a count of every old root in the torus.

For the separate **prepared value recurrence**, recent prefix layers need only have one \(M\)-cell separation. The rate used in CR.22b–CR.22d is instead a fixed share of \(\min(\beta\kappa,\delta M,\kappa_1-1)\), chosen above the same root-entropy threshold. The two estimates refer to their actual respective geometries. A growing \(R_k\) is not assigned to every prepared layer.

For the all-history inference assume that each primitive current pullback satisfies BC16.4 on the full \(2P_k\) contour with the same uniform sector constants. For composed reconstructions this is a CR hypothesis. For the already localized current-scale classical/E/R pieces it follows directly from their admitted product disc and support; for inherited B and the heterogeneous sector it is the native directional-disc estimate with the retained endpoint path.

At order \(m\), choose each differentiated coordinate in turn as the first derivative, apply Cauchy to the other \(m-1\) coordinates on a radius \(P_k/2\) polydisc, and take the best estimate. Commutation of analytic derivatives gives
\[
 |D_{i_1}\cdots D_{i_m}F_X|
 \le K_X\vartheta_X (m-1)!(2/P_k)^m
           e^{-c\max_s d_X(i_s)}.
 \tag{AB17.27}
\]
This includes every derivative of the nonlinear current coordinate map and of the nodal representative. It is not obtained by discarding \(D^2\Phi\).

BC16.2 sums the \(m=2\) row, with a factor \(|S_X|e^{\gamma\operatorname{diam}S_X}\) explicitly paid by the remaining carrier exponential. BC16.3 sums all orders. Its layer-cake argument counts at most \(C(n+R+1)^4\) current coordinates within radius \(R\) of a length-\(n\) carrier. The resulting \(4(m-1)\)-moment contributes at most \(C^m((m-1)!)^4\), and Cauchy contributes the remaining factorial. This gives precisely (AB17.4)–(AB17.5).

For completed-R relative carriers, use CR.1–CR.3 in this last step. Their current diameter is at most \(C[Mh_j(\ell(X)+1)+MR_k]\); the one free component diameter is paid by a separate small spatial rate and a share of the already extracted current guard. Keep carrier length, that diameter and the endpoint radius inside the **one** polynomial moment of degree \(4(m-1)\), as in CR.14. This retains factorial power five, instead of multiplying separate factorial losses. Exterior-volume/attachment sums use the rooted absolute norm, not a pointwise contracted decay with its entropy omitted. The exact prefix sum has already been paid in PF.16–PF.21 before this all-order counting.

These estimates are normally convergent in their anchored differentiated sums. They are uniform on a fixed smaller external native chart. Cauchy in any finite family of native directions then gives (AB17.6), with the exact norms (AB17.2) and the independent-current norm. Normal convergence justifies taking those derivatives after the age/carrier sum. No exact thin-polymer decomposition with an exponential volume weight is asserted by this direct endpoint method.

### 7. Fixed parameter order and quantitative smallness

All choices below are independent of derivative order, cutoff depth, torus volume and the individual admitted history.

1. Fix one admitted odd \(L\), the fixed finite gauge group dimension and the source geometric conventions. Choose one fixed admitted \(r>1\), \(p_0\), and integer native exponents \(q_0=q_1=q>p_0+r+2\). This explicitly pays every prefix real-center enhancement; the choice does not depend on the number of prefix integrations.
2. Fix the source \(\beta>0\), the full invariant carrier rate \(\kappa\), the localization reserve \(\kappa_1\), and the block/separation parameters in the primary order. CMP119 after (2.31) permits the large decay choice; CMP116 (1.7), (1.11) allows \(M\) large enough to retain all required fractions of \(\delta_1M\). Retain positive shares for full-\(\kappa\) output, primitive entropy, collars, age, normalized anchored summation and final spatial weights. In original histories choose the admitted separation for (AB17.25). In prepared histories require the fixed one-\(M\)-layer rate from CR.22b to exceed (CR.22c). Do not spend a rate repeatedly at later births: the source full rate is preserved and a fixed weaker analysis rate is tested against it. This fixes all constants in NP, RM, JI, the nodal interpolation, CR and BC16.
3. Choose the AF comparison parameter
\[
 0<\beta_0\le
 \min\left\{\frac18,
 \frac{\log(5/4)}{2(1+\log2)}\right\}.
 \tag{AB17.28}
\]
The AF theorem permits this fixed choice by reducing the common coupling ceiling. It supplies (AB17.23a) with slack.
4. Let \(r_{\rm NP}>0\) be the genuine whole-ball radius of NP.5, and let \(\sigma_{\rm src}>0\) be the smallest normalized primitive reserve after the auxiliary-current embeddings and old-current comparison. Take one fixed
\[
 r_{\rm ext}\le
 \min\left\{\frac{r_{\rm NP}}{64C_{\rm map}},
             \frac{\sigma_{\rm src}}{64C_{\rm map}C_{\rm node}},
             \frac1{64C_{\rm ER}}\right\}.
 \tag{AB17.29}
\]
The constants here are the already fixed map, nodal and E/R admission constants. The factors \(64\) pay the larger contour and a smaller domain for Cauchy; increasing them has no effect on the argument. Set the independent-current radius by the same fixed reserve and the actual BC16 inner-layer embedding constant.
5. Only now reduce the common coupling ceiling so that \(C\theta_k\), including the prefix enhancement divided by \(\alpha_k\), occupies at most the same fixed reserve; \(D_k+2\delta_k<\epsilon_{\rm abs}/8\); all logarithm charts remain in their chosen balls; \(R_k\ge2C_{\rm foot}L\); and all source small-field hypotheses hold. Also impose the primitive rooted-sum threshold in CR.20 and \(C\sup_b\zeta_b\le(1-e^{-\lambda})/2\), with the resulting \(\mathcal A_*\) inside that threshold. Since all exponential coefficients tend to zero, these are compatible finitely many choices. The resulting interval applies to every scale of the admitted trajectory.

For all local sectors, the smallness can be read directly from (AB17.24). The fixed external radius does not have to tend to zero with the coupling. Since \(D_k\le Cg_k\ell_k^q\),
\[
\begin{array}{ll}
 \mathfrak K_E P_k^{-2}
     &\le C\ell_k^{-2p_0}\longrightarrow0,\\[2mm]
 C_Rg_k^{\kappa_0-11}P_k^{-2}
     &\le Cg_k^{\kappa_0-11}\ell_k^{-2p_0}\longrightarrow0,\\[2mm]
 B_0\theta_kP_k^{-2}
     &\le C\ell_k^{-q-p_0}\longrightarrow0,\\[2mm]
 g_k^{-2}D_k^3P_k^{-2}
     &\le Cg_k\ell_k^{3q-2p_0}\longrightarrow0,\\[2mm]
 D_kP_k^{-2}
     &\le Cg_k\ell_k^{q-2p_0}\longrightarrow0,\\[2mm]
 g_k^{-2}\delta_k(1+\log\ell_k)^{b_\phi}
               e^{-c_{\rm col}R_k}P_k^{-2}
     &\le Cg_k^{-1}\ell_k^{-p_0}
        (1+\log\ell_k)^{b_\phi}e^{-c_{\rm col}\ell_k^r}
        \longrightarrow0 .
\end{array}
 \tag{AB17.30}
\]
Here the R exponent is the admitted \(\kappa_0\ge12\). The last limit follows from \(g_k^{-1}=\exp(\ell_k/2)\) and \(r>1\). All limits are uniform for \(0<g_k\le\bar g\) as \(\bar g\downarrow0\), because the right sides have a finite decreasing tail in \(\ell_k\).

The full older-density term is uniformly vanishing by (AB17.7i). Its two small coefficient norms obey
\[
 \mathcal A_*+\varepsilon_*^{\rm PF}
 \le C\sup_b\left[
  (1+\ell_b)^A e^{-cR_b}
       +g_b^{-2}(1+\ell_b)^{A_F}e^{-c_FR_b}\right]
 \longrightarrow0 ,
 \tag{AB17.31}
\]
after enlarging fixed exponents and reducing fixed rates. Here \(g_b^{-2}=e^{\ell_b}\) and \(R_b\ge\ell_b^r\), \(r>1\). For any prescribed \(\varepsilon_B>0\), choose the ceiling once more so that the finite sum in (AB17.30) and (AB17.7i) is at most \(\varepsilon_B/C_{\rm row}\). Equation (AB17.4) then supplies the specified share of the source principal coercivity gap. No own-sector smallness assumption is left in this final choice.

### 8. Sector hypotheses and consequences

For the all-history boundary application, the same local derivative bounds are required for the **actual complete B and boundary-induced activities**, including collars, constraints and current-coordinate dependence. A response of an older reference density is within that statement whenever it actually remains in the current conditional law.

| Application component | Result under these hypotheses | Status |
|---|---|---|
| Full unprimed current support | The contour contains a fixed multiple of the actual \(P_k\); no \(p_1\) identification is used. | Included in the theorem. |
| Primitive nonlinear reconstructed field and physical-current domain | NP.5 gives a strong native ball on the specified source chart. | Transfer to a composed Wilson history requires CR and CL. |
| Symmetric average and source gauge | RM/JI use the specified raw average and corrected chart, with the fine gauge restriction acting on old slots. | The comparison must hold on the same retained data. |
| Surviving old fluctuation and raw arguments | The proposed native gauge conversion in AD17.3 and CR.2 must control both endpoints of raw links. | Uniform control for the composed reconstruction is a hypothesis. |
| Independent currents and arbitrary admitted native directions | A common radius includes all older embeddings; derivatives use the explicit strong norm (AB17.2). | Supplied at the stated norm, with raw-coordinate costs exposed. |
| Complete current exterior relocation | The whole shifted action is estimated on an absolute small-field contour; this relocation's Jacobian is independent of the inner current. | Included, with its outer factor retained. |
| Heterogeneous coefficient and collar | The exact recursion, transition-index bound and four-layer collar calculation retain the running \(g_k^{-2}\). | Included in Section 5.4. |
| Inherited B, E/R boundary pieces, classical/measure/constraint remainders | All are retained on the shifted common contour with their actual sector majorants. | Included in Sections 3–5. |
| Ordinary older Gaussian/Schur coefficients | The exact derivative (AB17.7a), local walk dependence and the \(P_j^2\) old-field cost are summed. | OR17.1 supplies the uniform budget. |
| Every interrupted preparatory branch | Actual modified charts, selector localization, supported failed shift, complete action difference and its noncanceling future-current Jacobian are retained. | PF.1–PF.22 supplies the budget; \(q>p_0+r+2\). |
| Completed R components and old reference masses | Exact (1.104) integrates all hidden dependence with the incoming boundary; canonical raw masses remain. | Reduced scalar law is exact; no pointwise hidden-density identity is claimed. |
| Repeated relative-carrier norm | Actual bounded tags, attachment entropy, full-\(\kappa\) output, original birth anchors and the chronological recurrence are retained. | CR.1–CR.25 supplies the value norm and factorial-five derivative application. |
| Uniform summed derivatives and weighted Hessian | Assume every actual sector has the common contour and anchored endpoint majorant; the total bound is (AB17.24). | Equations (AB17.4)–(AB17.6), (AB17.7i), (AB17.30)–(AB17.31). |

The sector sum supplies the complete derivative estimate provided the stated sector, domain and transport hypotheses hold simultaneously.

Under CL the representation gives the Wilson marginal and the conditional law on the stated retained data. Differentiating that representation requires the current and gauge conventions and the contour used above.

### 9. Compatibility with the already proved C-06 implication

The exact reduction (AB17.7e) changes which older hidden variables have already been integrated; it does not change the current free-bond coordinates or the source current precision
\[
 K_{II}=(C^*\Delta^{(k)}C)_{II}.
 \tag{AB17.32}
\]
The background, determining geometry and free-coordinate map in this formula are the actual ones of the reduced source representation. Its surviving retained histories still satisfy C-06's primary admissibility hypotheses. That theorem's principal lower bound is uniform on this entire heterogeneous class. It is not an identity-background bound or an inverse covariance estimate for the interaction.

All current-dependent effects of the older ordinary or failed operations, and the completed scalar logarithms, now belong to the explicit scalar boundary perturbation just bounded. Canonical \(\tau_Y\) factors are current-independent raw multipliers; the current interior and its one-step stencil miss their old large-field support. The current exterior relocation is supported in the retained regular exterior region and does not change those raw \(V_b|_Y\). Earlier prefix relocations leave already completed resident masses in the unchanged deep factor (1.76). Their scalar action responses have nevertheless been included where they occur.

The source conditional potential therefore has exactly the form used in HC.15: its unchanged principal quadratic form, its retained exterior linear force, and the complete local/boundary scalar perturbations. If a bulk classical or measure term has already been counted in this note, omit its duplicate from HC's separate local remainder; this only improves the majorant. The exterior force has zero current Hessian and stays in the mean.

Intersect the genuine current/native contours proved here with C-04's and C-06's absolute principal-map reserves, taking a fixed fraction of each radius in its own norm. The strong native rows include the required second-order curl/current row, and the actual current map includes its \(g_k\) scaling. The current contour still contains the full real \(P_k\) support. At a real exterior datum the source bound is the one used by HC; on the auxiliary complex ball the larger \(D_k\) still tends to zero, so it fits the same fixed absolute radius.

With (AB17.4) below the share allotted in (HC.28), the perturbation criterion in Annex AI yields coercivity of this reduced law. The Wilson application requires the complete boundary budget under CR and CL.

### Primary references and proof dependencies

- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP **119** (1988), 243–285: pp.253–254 for the first old Gaussian factor; pp.255–259 for admitted histories, AF comparisons, old operators and the localized coupling recursion; pp.261–262 for primitive B domains and covariance; pp.264–270 for the exact current substitution and relocation; pp.276–277 for the complete sector assignments.
- T. Balaban, *Propagators for Lattice Gauge Theories in a Background Field*, CMP **99** (1985), 389–434: corrected relative average, physical-current and constrained-covariance formulas, used with the actual symmetric family specified in RM/JI.
- T. Balaban, *The Variational Problem and Background Fields in Renormalization Group Method for Lattice Gauge Theories*, CMP **102** (1985), 277–309: the original analytic family, reproduced local averaging derivatives, formal extension and inverse gauge on pp.307–309.
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories I*, CMP **109** (1987), 249–301: (0.11)–(0.12), the actual symmetric raw averaging family.
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories II*, CMP **116** (1988), 1–22: (1.17), (1.37)–(1.43), the complete localized classical and measure remainder.
- T. Balaban, *Large Field Renormalization I*, CMP **122** (1989), 175–202: pp.179,191–192,201, the changed admissible history and localized replacement.
- T. Balaban, *Large Field Renormalization II*, CMP **122** (1989), 355–392: (1.65)–(1.75), native prepared domains and the background-dependent operation; (1.95)–(1.104), source carrier majorants, classification and the exact integrated alternative.
