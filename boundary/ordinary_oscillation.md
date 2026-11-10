# Ordinary stopped-density oscillation on mixed scales

**Composed-response hypothesis (CR).** Each complete boundary conclusion below assumes the displayed native-chart and spatial response estimates for the actual iterated reconstruction, with the prescribed earlier innovations and raw variables fixed, uniformly over the admitted histories. A sufficient estimate for the latent contribution is (A.8) in [Conditional-law estimates and the continuum application](../continuum/conditional_to_continuum.md), refined for the anchored exterior derivative in PG.18–PG.20. The two endpoint bounds concern the identical Wilson-subtracted primitive, its actual cutoff and its independently extended current. A direct minimizing-field derivative alone does not establish this hypothesis. The application to every required original Wilson history remains open. Complete boundary estimates and their C06/C08 applications in this chapter are conditional on CR and the other displayed source, AF, domain and support assumptions. Exact density identities and abstract inequalities retain their individually stated hypotheses.

In the projective density formulation, a sufficient comparison is
\[
 \sup_{\zeta,x,a}\left|
 \log\frac{W_\zeta(x,a)W_0(x,a_*)}
               {W_0(x,a)W_\zeta(x,a_*)}
 \right|\le\delta_r<\pi/2,
\]
on the stipulated chart with the required uniform rates and actual fixed support. The composed ordinary response is the unresolved input in its derivation. The exact partial-gauge transport and the surviving fixed-exterior derivative are given in the chapter [Gauge covariance of partial integrals and exterior scores](../continuum/partial_gauge_transport.md), equations PG.2–PG.6 and the subsequent anchored-score criterion.

## 1. Evaluation age and forcing age

The boundary-induction argument's OR.14–OR.16 did not justify OR.19. An ordinary term has a birth index \(b\), an actual evaluation layer \(n\), and an integration stage \(j\). On an interrupted history, \(b\le n<j\) is possible. CMP119 (3.56)–(3.67) gives an irrelevant remainder measured by \(n-b\). It does not replace that exponent by \(j-b\).

Write

\[
 a=n-b,\qquad c=j-n,\qquad \lambda=5-\vartheta>4.
 \tag{SR.1}
\]

The missing calculation cannot be supplied by performing the convergent sum OR.15 again. Nor does the physical-input/native-radius conversion RL.25 alone supply spatial decay. The decay comes from the actual determining-data response and the retained carrier joining its attachment to the term's root.

This repair uses a weaker sufficient estimate. It obtains **two bounds on the identical finite difference** and interpolates their minimum. The first uses the Ward cancellation at the two endpoints. The second uses a direct, deliberately crude response bound, for which the E term and its own Wilson term may be estimated separately. There is no differentiation of a Ward identity asserted only on the physical-current graph.

The boundary-induction argument's final-mass restoration, moving-normalizer calculation, and local quadratic cumulant estimate are not changed by this argument. Their application still requires the ordinary bound proved here.

## 2. Keep the source object and its cutoff exactly

At fixed birth \(b\), the inherited source expression is

\[
 \mathcal E_b(U)=E^{(b)}(\Lambda_b,U)-E^{(b)}(\Lambda_b,1)
                         -\beta_b A(\phi_b,U).
 \tag{SR.2}
\]

The coefficient \(\beta_b\), cutoff \(\phi_b\), domain \(\Lambda_b\), and primitive bank are fixed during a preparatory prefix. The prefix creates the additional C bank; it does not replace the ordinary E bank by a newly projected one. This is the content of LFR I (1.60)–(1.63).

CMP119 (2.26)–(2.29) and (3.65) give the exact partition

\[
 \begin{split}
 \mathcal E_b(U)
 &=\sum_{z\in\Lambda_b^0}\mathcal R_{b,z}(U)
       +\mathcal B_b^{\rm cut}(U),\\
 \mathcal R_{b,z}(U)
 &=\sum_{X\ni z,\ X\subset\Lambda_b} E^{(b)}(X,U,z)
       -E^{(b)}(\Lambda_b,1,z)-\beta_b A(h_z,U),\\
 \mathcal B_b^{\rm cut}(U)
 &=-\beta_b\sum_{z\notin\Lambda_b^0} A(h_z\phi_b,U).
 \end{split}
 \tag{SR.3}
\]

Here \(h_z\phi_b=h_z\) for \(z\in\Lambda_b^0\). The last line must be retained. In particular, an interior root estimate must not silently delete the remaining cutoff terms.

The marginal cancellation is a statement about the complete root aggregate \(\mathcal R_{b,z}\). The Euclidean tensor reduction uses the summed primitive catalog. It is not a cancellation available for each absolute \(X\)-summand. CMP119 (3.61)–(3.66) identifies its coefficient with the same \(\beta_b\) in (SR.2).

Both estimates below are applied to

\[
 \Delta_j\mathcal R_{b,z}
   =\mathcal R_{b,z}(U^1)-\mathcal R_{b,z}(U^0),
 \tag{SR.4}
\]

with the actual two stopped configurations and the earlier raw variables fixed. No subtraction, reference field, or cutoff is changed between the bounds.

## 3. An elementary response interpolation theorem

Let \(S_j\) be the actual forcing cells in a stage-\(j\) strip. Fix \(0<\eta<1\) and put \(u=1-\eta\). Suppose the same difference (SR.4) satisfies

\[
 \begin{split}
 |\Delta_j\mathcal R_{b,z}|&\le
 C_A E_0\ell_r^{D_A}(1+a)^{s_A}L^{-\lambda a}=:A_{b,n},\\
 |\Delta_j\mathcal R_{b,z}|&\le
 C_B E_0\ell_r^{D_B}(1+a+c)^{s_B}e^{-\Gamma c}
       \sum_{s\in S_j} w_j(z,s)^{1/u}=:B_{b,n,j,z}.
 \end{split}
 \tag{SR.5}
\]

Normalize the spatial weights by a fixed constant so that \(0\le w_j\le1\), and choose their decay with sufficient reserve that

\[
 \sum_{z\text{ at birth mesh }b\text{ and layer }n}w_j(z,s)
       \le C(1+a+c)^{s_0}L^{4(a+c)}.
 \tag{SR.6}
\]

The four-dimensional density is explicit. It is not hidden inside a source row that has already included it.

Since \(\min(A,B)\le A^\eta B^u\) and \((\sum_s v_s)^u\le\sum_s v_s^u\), (SR.5) implies

\[
 |\Delta_j\mathcal R_{b,z}|
 \le C E_0\ell_r^D(1+a+c)^s
       L^{-\eta\lambda a}e^{-u\Gamma c}
       \sum_{s\in S_j}w_j(z,s).
 \tag{SR.7}
\]

Take \(D\ge\max(D_A,D_B)\), increasing a fixed polynomial exponent if necessary. Sum first over the literal roots using (SR.6), and then over the two ages:

\[
 \begin{split}
 \sum_{b\le n\le j}\sum_z|\Delta_j\mathcal R_{b,z}|
 &\le CE_0\ell_r^D|S_j|\,\mathcal S,\\
 \mathcal S&=\sum_{a,c\ge0}(1+a+c)^s
   L^{-(\eta\lambda-4)a}
   e^{-[u\Gamma-4\log L]c}.
 \end{split}
 \tag{SR.8}
\]

This sum is finite if

\[
 \eta\lambda>4,\qquad (1-\eta)\Gamma>4\log L.
 \tag{SR.9}
\]

Such an \(\eta\) exists precisely when

\[
 \Gamma>\frac{4\lambda}{\lambda-4}\log L.
 \tag{SR.10}
\]

For example, choose

\[
 \vartheta=\tfrac12,\quad \lambda=\tfrac92,\quad
 \eta=\tfrac{11}{12},\quad \Gamma\ge60\log L.
 \tag{SR.11}
\]

The summand in (SR.8) is then bounded by
\((1+a+c)^sL^{-a/8}L^{-c}\). Factor
\(1+a+c\le(1+a)(1+c)\) to see convergence directly. All constants are independent of the total history depth and volume.

This proof does **not** assign a Ward bound to each marked forcing derivative. The Ward bound applies once to the complete two-endpoint difference. Only afterwards does subadditivity distribute its majorant over the forcing cells. It also does not retain the original spatial rate for free: the response bound must reserve \(w^{1/u}\), since interpolation leaves \(w\).

## 4. Source domains: a fixed reserve before any estimate

The interpolation theorem is unconditional mathematics. Its Wilson application requires actual endpoint and ordinary-response admission. The following reserve records the intended source application explicitly.

Use a fixed external/map profile and a larger ordinary primitive profile,

\[
 \gamma_n=g_n\ell_n^{q+Q},\qquad
 \alpha_n=g_n\ell_n^{q+Q+D_{\rm prep}+2}.
 \tag{SR.12}
\]

Here \(D_{\rm prep}\) is fixed before \(Q\); it bounds the finite preparation and top-band losses, including \(L_0^{2N_0}\). It does not depend on the number of derivatives or the history depth. The source exponents, map/localizer parameters, and common coupling ceiling are then selected once. This reserve concerns the ordinary source family, not an enlargement of arbitrary completed relative inputs.

PF.1–PF.3 in Annex AV of the retained theorem group prove that a fixed strong native core is contained in every modified prefix domain, including the independent-current and reconstructed-current clauses. They use the actual mixed determining sets in LFR I (1.14)–(1.17). The source's forward insertion statement on p.191 supplies the additional step from a later prefix chart to the earlier one. Mere inclusion of the input core would not by itself prove a bound on every possible modified output.

For the actual outputs, the displayed modified norms give a bound
\(C\ell_r^{D_{\rm prep}}\gamma_n\). The stipulated AF comparison yields
\(\ell_n\ge\ell_r-C\) for \(n\le r\). Consequently

\[
 \frac{C\ell_r^{D_{\rm prep}}\gamma_n}{\alpha_n}
 \le \frac{C'}{\ell_n^2},
 \tag{SR.13}
\]

after reducing the common coupling ceiling. Thus the actual endpoint jets lie strictly within the larger ordinary native profile. The C02/E14 admission calculations, including E14.26–E14.32 and E14.40–E14.48, then use this reserve for the genuine minimizing map, local gauges, and independent-current substitution.

For an ordinary interpolation between the two allowed input tuples, retain the exact constraint correction \(g_jCB_j-hD(g_jCB_j)\). The normalized input is \(g_jP_j\), not \(P_j\). With \(c=j-n\), the full smooth determining-data row gives a bound of the form

\[
 C\ell_r^{D_{\rm prep}}
 \frac{g_jP_j}{\alpha_n}(1+c)^v e^{-\gamma c}
 \le \frac{\beta}{8}\,2^{-c},
 \tag{SR.14}
\]

by the fixed profile reserve, a sufficiently large fixed geometric rate, and the common weak-coupling ceiling. Summing these contributions preserves a fixed fraction of the dyadic margins in LFR I (1.64)–(1.69). This is ordinary primitive analyticity; it does not assert Ward cancellation at every point of that interpolation.

The independent current is carried by the actual source extension and its complete current-output row. It is not replaced by a physical current off the physical slice. Likewise, no bare fine-link tangent is substituted for the admitted collection of field, gradient, projection, Laplacian, and reconstructed-current norms.

For the problematic stratum \(n<j\), the determining sets below \(j\) are unchanged by the stage-\(j\) integration: LFR I (1.15)–(1.17) retain their already-prepared lower shells. Thus the two endpoints have a common lower evaluation layer. The changing layer \(n=j\) has no missing age. Coarser outputs \(n>j\) keep their true mesh and spatial cover and are treated separately in Section 8.1; they are not relabeled as grade \(j\). A stopped component is removed as a whole from subsequent integrations; it is not silently assigned the grading of a still-active component.

## 5. The endpoint bound keeps the cancellation and cutoff error

At either actual endpoint, apply the source's nearby/far split at its true layer \(n\). The far-carrier estimate is CMP119 (3.48). For the nearby part, CMP109 (3.28)–(3.36), Lemma 4, and CMP119 (3.49)–(3.67) give the Ward expansion with the same Wilson subtraction.

The chosen analytic extension matters. CMP109 carries the independent current through its analytic gauges, then permits the regular complex insertion \(A\) of (3.31). The C02/E14 calculations track this prescribed pullback and its running radii. They do not appeal to uniqueness of an extension from a physical-current graph.

The coefficient-order decomposition retains an order \(p\) denominator \(\alpha_b^{-p}\) together with field degree at least \(p\), for \(2\le p\le5\). The full-lattice marginal quadratic coefficient cancels with its own \(\beta_b\). The ordinary irrelevant remainder has geometric factor \(L^{-\lambda(n-b)}\), but a restricted-bank coefficient error must also be retained if a prepared local patch crosses the old cutoff. The AF profile comparison gives

\[
 \left(\frac{\alpha_n}{\alpha_b}\right)^p
       \le C_Q(1+n-b)^{p/2}.
 \tag{SR.15}
\]

Fixed preparation powers can be included in \(\ell_r^{D_A}\), with \(D_A\) independent of \(Q\). No claim of \(j-b\) Ward decay is made.

### 5.1 Ancient births: the true layer gain

For \(b<h\), the preserved inclusion \(\Omega'_{b+1}=\Omega_{b+1}\subset\Lambda_b\) implies that a root at prepared layer \(n\) is separated from \(\Lambda_b^c\) by a fixed multiple of \(h_n\), except for harmless adjacent-layer cases. The same graded admissibility used in (SR.17) proves this separation. A primitive carrier omitted in extending the coefficient sum to the full lattice therefore has \(d_b(X)\ge cL^{n-b}\). Its reserved full-tree decay is bounded by any fixed irrelevant power. Thus both endpoints satisfy the first line of (SR.5), with their exact restricted bank and own Wilson subtraction.

### 5.2 Recent births: retain the truncated-tensor error

For \(h\le b\le n\le j\), the preparation can expand a determining domain through the old \(\Lambda_b\) cutoff. It would be incorrect to assert that the preceding separation always holds. Instead, stop the source coefficient calculation at (3.56), and keep the error in extending the restricted \(X\)-sum to the full-lattice tensor in (3.57).

Since \(z\in\Lambda_b^0\), any omitted carrier has to cross the original \(MR_b\) interior buffer. Reserving a share of its literal full-tree decay gives \(e^{-\kappa_{\rm tail}R_b}\). The tensor is calculated at the flat reference \((1,0)\), where these primitive coefficients are defined. No evaluation of a missing primitive at a field outside its admitted domain is needed. The retained coefficient-order/field-degree decomposition bounds its field factors by fixed age polynomials through (SR.15). Consequently the actual two-endpoint bound is

\[
 |\Delta_j\mathcal R_{b,z}|
 \le C_QE_0\ell_r^{D_A}(1+a)^{s_A}
     \left[L^{-\lambda a}+e^{-\kappa_{\rm tail}R_b}\right].
 \tag{SR.15a}
\]

The counterterm remains the original \(\beta_b\). The second term measures the part of the finite-domain tensor not canceled by that coefficient; it is not a newly selected Wilson subtraction.

The response bound in Section 6 is for the entire original difference. Thus it also handles (SR.15a) without a separate response theorem for a manufactured error term. For positive numbers,

\[
 \min(A_1+A_2,B)
 \le (A_1+A_2)^\eta B^{1-\eta}
 \le (A_1^\eta+A_2^\eta)B^{1-\eta}.
 \tag{SR.15b}
\]

The first summand gives (SR.8). For the second, \(a\le N_r\), and the recent-window AF comparison gives \(R_b\ge c_RR_r\), with one fixed \(c_R>0\). LFR II p.361, immediately after (1.20), requires \(N_r\le R_r\); retaining a fixed endpoint/rounding factor, write \(N_r\le C_NR_r\). The retained waiting-depth choice on p.384 is compatible with this relation. There is no substitution of a shorter preparation window.

After the full root count, the extra contribution is bounded by

\[
 \begin{split}
 &CE_0\ell_r^D |S_j|(1+N_r)^{s+1}
   \exp\!\left[4N_r\log L-\eta\kappa_{\rm tail}c_RR_r\right]\\
 &\hspace{25mm}\times
   \sum_{c\ge0}(1+c)^s e^{-[(1-\eta)\Gamma-4\log L]c}.
 \end{split}
 \tag{SR.15c}
\]

Choose the remaining carrier-tail rate, after allocating the spatial and entropy shares, so that

\[
 \eta\kappa_{\rm tail}c_R>4C_N\log L+\epsilon,
 \qquad \epsilon>0.
 \tag{SR.15d}
\]

The source permits the ordinary carrier exponent to be fixed sufficiently large, with the larger block/localization parameters and the weak-coupling ceiling chosen afterwards. This is an explicit strengthened fixed rate inequality. It changes neither the real cutoffs nor the preparation depth nor the class of histories at those parameters. The expression (SR.15c) is bounded by a fixed polynomial times \(e^{-\epsilon R_r}\).

Thus the recent restricted-bank error is summable. A finite number of births alone would not have paid \(L^{4(n-b)}\); the retained cutoff buffer and (SR.15d) are essential.

## 6. The crude bound keeps the response

For this second bound, work with the original \(E^{(b)}(X,U,z)\), before any nearby minimizing-map replacement. Ordinary native Cauchy gives its differential at cost \(CE_0e^{-\kappa d_b(X)}/\alpha_b\). Compose with the actual response row and keep the physical forcing \(g_jP_j\).

For an attachment at native grade \(m\ge b\), the source conversion for an output of physical order \(p\ge1\) contains \((h_b/h_m)^p\). In particular there is no positive power of \(L^{m-b}\). The ratio

\[
 \frac{g_jP_j}{\alpha_b}\le C_Q\ell_r^{D_1}(1+j-b)^{v_1}
 \tag{SR.16}
\]

has no uncanceled inverse coupling. The fixed logarithmic degree here is independent of the chosen enlargement exponent \(Q\).

### 6.1 The response must be rooted at the same \(z\)

The source row initially reaches an attachment \(y\) of grade \(m\), which may differ from the root's grade \(n\). If \(m\le n+1\), the row pays \(j-n\), up to a fixed endpoint factor. If \(m\ge n+2\), the literal full carrier contains a path from the root \(z\) to \(y\). Graded admissibility gives

\[
 \operatorname{dist}(z,y)\ge cM_1h_{m-1},\qquad
 d_b(X)\ge c' L^{m-n},
 \tag{SR.17}
\]

where fixed block ratios and endpoint conventions are absorbed in \(c'\). Indeed \(z\notin\Omega_{n+1}\) and \(y\in\Omega_m\), so the interlayer separation may be applied at layer \(m-1\). The same argument uses the actual prepared determining domains.

For every fixed required \(G>0\),

\[
 e^{-\kappa' d_b(X)}\le C_Ge^{-G(m-n)}
 \tag{SR.18}
\]

using one reserved share of the full carrier. The remaining row pays \((j-m)_+\). Together they pay \(j-n\); remaining positive shares are kept for spatial summation and carrier entropy. This argument uses the ordinary full E carrier, not a contracted quotient tree with an artificial root.

Choose the source geometric constants so that the remaining age rate is at least \(\Gamma\) in (SR.11), and keep enough spatial decay for the power \(w^{1/u}\) in (SR.5). CMP119 fixes \(M_1\) and \(M_2=L^2M_1\) before choosing \(M\) large; LFR I (1.47) supplies the rate proportional to \(M/M_1\). The parameter choice is fixed before the weak-coupling ceiling and never depends on a history's depth.

The original source measure factors in the normalized reconstruction row must be paired before counting roots. Summing the primitive catalog with the remaining full-tree reserve yields the E part of the second line of (SR.5).

### 6.2 The Wilson term has two curvature factors

The birth coefficient satisfies

\[
 |\beta_b|\le CE_0\alpha_b^{-2}.
 \tag{SR.19}
\]

The Wilson plaquette action has a quadratic zero at the identity. Its difference contains one background-curvature factor and one response-curvature factor. On a birth cell whose actual evaluation layer is \(n\), the fine-plaquette count cancels their physical mesh factors, giving

\[
 |\beta_b\Delta_j A(h_z\phi_b,U)|
 \le CE_0\frac{\alpha_n}{\alpha_b}
             \frac{g_jP_j}{\alpha_b}
       L^{-4(n-b)} e^{-\Gamma(j-n)}
       \sum_{s\in S_j}w_j(z,s)^{1/u},
 \tag{SR.20}
\]

up to the already retained fixed profile and age polynomials. The two radii in the denominator are canceled by the two physical field factors. Replacing \(\beta_b\) by a purported uniform constant would hide the calculation.

For an interior root, discard the favorable \(L^{-4(n-b)}\) in this crude estimate and combine it with the E response. This proves the second line of (SR.5) for the same complete difference (SR.4). The Ward estimate is not used in this calculation.

## 7. The remaining cutoff terms

Formula (SR.3) still contains the literal cutoff remainder. It is handled by (SR.20), retaining its four curvature powers. For a cutoff label outside \(\Lambda_b^0\), choose an actual support anchor in \(\operatorname{supp}(h_z\phi_b)\subset\Lambda_b\); the label itself may lie just outside \(\Lambda_b\). This changes the root count by a bounded multiplicity and ensures \(n\ge b\). The local Wilson stencil has comparable native grades by the same interlayer separation.

Put \(h=r-N_r\), the lower end of the current preparation window.

### 7.1 Ancient births \(b<h\)

LFR I (1.11) and (1.15)–(1.17) leave the determining layers through \(h\) unchanged. A cutoff support anchor lies within \(CMR_bh_b\) of a point outside the literal \(\Lambda_b\). By \(\Omega_{b+1}\subset\Lambda_b\), that point belongs to an unchanged lower-grade region. CMP102 p.277, condition (1), applied to the prepared admissible sequence therefore gives

\[
 L^{n-b}\le C R_b.
 \tag{SR.21}
\]

This is a logarithmic allowance, not an assertion that \(n=b\). If an anchor has \(n\ge b+2\), compare it to that outside point using the separation between \((\Omega'_{n-1})^c\) and \(\Omega'_n\); the cases \(n=b,b+1\) are absorbed in the constant.

The factor \(L^{-4a}\) in (SR.20) cancels the birth-to-layer portion \(L^{4a}\) of the root density. Use

\[
 \mathbf 1_{\{L^a\le CR_b\}}\le CR_b L^{-a},\qquad
 R_b\le C\ell_r^\rho(1+a+c)^\rho.
 \tag{SR.22}
\]

The second inequality follows from the stipulated AF comparison and the fixed logarithmic cutoff profile. The resulting old-birth sum is bounded by

\[
 C E_0\ell_r^D |S_j|
 \sum_{a,c\ge0}(1+a+c)^s
       L^{-a}e^{-[\Gamma-4\log L]c}<\infty.
 \tag{SR.23}
\]

No Ward estimate for an artificial boundary root is used.

### 7.2 Recent births \(b\ge h\)

There are at most \(N_r+1\) such births in the current bank. For \(b\le n\le j\), retain the \(L^{-4a}\) in (SR.20); it cancels the \(a\)-density exactly. The remaining \(c\)-sum converges for \(\Gamma>4\log L\), and the number of possible \(a\) values costs at most a fixed polynomial in \(N_r\).

If \(b>j\), keep the entire coarse birth atom. An actual stage-\(j\) cell intersects only a bounded number of coarser birth cells; a fictitious factor \(L^{4(b-j)}\) is not inserted. The same-profile Wilson bound is \(CE_0\), and the ordinary primitive bound is \(CE_0\), with the actual response and its spatial row retained. Again only the finite window is counted.

At the start of a new attempt these are the current canonical cutoffs, not every historical cutoff ever consumed. LFR II p.377 reconstructs the new ordinary action and subtracts the same added terms into the remainder; p.390–391 returns the full source induction hypothesis. The ancient-layer argument is then applied within the new attempt's literal geometry.

## 8. Replacement for OR.19

### 8.1 Coarser outputs \(b\le j<n\)

This case is different from a recent birth \(b>j\). Retain the actual output cover at grade \(n\). A forcing cell at grade \(j\) belongs to only a bounded number of compatible coarser \(n\)-cells. The remaining native spatial row, at the post-interpolation rate, has a bounded sum over those output cells. The birth-root count in one such cell is \(L^{4(n-b)}\), not \(L^{4(j-b)}\).

Put \(a=n-b\). The endpoint estimate still uses \(L^{-\lambda a}\), while the crude response has no required missing-age factor. The identical min calculation, now with the spatial kernel normalized on the actual \(n\)-cover, leaves

\[
 L^{4a}L^{-\eta\lambda a}
       =L^{-(\eta\lambda-4)a}.
 \tag{SR.23a}
\]

This is summable in the old birth. There are at most \(N_r\) output grades \(j<n\le r\), so that enumeration costs a fixed polynomial in the preparation window. For the recent truncated-tensor error, \(h\le b\le j<n\le r\), and the worst root density is \(L^{4(r-b)}\le L^{4N_r}\). The same fixed inequality (SR.15d) pays it. For ancient births the cutoff distance again supplies the actual irrelevant-age gain.

For the literal Wilson cutoff residual, its \(L^{-4(n-b)}\) cancels the actual \(n\)-cell birth density. Recent births and output grades are finite in the window. Ancient cutoff anchors retain (SR.21) at their true layer \(n\); the indicator estimate (SR.22) supplies a summable \(L^{-(n-b)}\). The remaining spatial row is used with its original native measures. Since \(0\le w\le1\), a stronger raw factor \(w^{1/u}\) may be weakened to \(w\) for this Wilson estimate.

No fine subdivision of a coarse forcing/output atom, or implicit factor \(L^{4(n-j)}\) beyond the displayed actual birth-root count, is introduced. The separate \(b>j\) case remains the whole-coarse-atom calculation in Section 7.2.

### 8.2 The scalar bound

Combining the ancient/interior estimate (SR.8), the recent truncated-tensor estimate (SR.15c), the literal cutoff estimate (SR.23), the recent-birth count, and the existing actual strip count gives

\[
 \sup_{\mathcal D^{++}}\!|D_{\rm ord}^{E}|
 \le C_Q E_0\,\ell_r^{D_*}
       N_r^{s_*}L_0^{c_*N_0}
       \sum_{j=h}^{r-1}D_j(P)
 \le C_Q\ell_r^{D_E}.
 \tag{SR.24}
\]

The degree \(D_E\) is fixed before \(Q\). The constants and common weak-coupling ceiling may depend on the selected source profiles. The comparison keeps all earlier real variables fixed and retains both stopped endpoint configurations.

This is the form of OR.19 that the ordinary phase argument needs. It is obtained without claiming the stronger per-term factor \(L^{-\lambda(j-b)}\). The rates actually paid after summation can be the explicit \(L^{-a/8}L^{-c}\) of (SR.11).

## 9. Conditions for the two-age implication

The following conditions enter the application:

1. The two endpoint fields use the prescribed analytic C02/E14 extension, including the independent current, and meet the native norms after the fixed reserve (SR.12).
2. The response bound is for the original primitive bank on the actual fixed-raw family, including all required smooth/current rows; the physical \(g_j\) factor survives constraint elimination and relocation.
3. The root-to-attachment carrier and the source row refer to the same primitive record, and retain the spatial reserve lost in interpolation.
4. The literal Wilson cutoff remainder is retained and uses the ancient/recent split above.
5. The recent truncated E-bank error is kept as in (SR.15a), and its full density cost is paid with the actual \(N_r\le C_NR_r\) relation and the explicit remaining-rate inequality (SR.15d).
6. The range \(b\le j<n\) keeps its actual output mesh and birth-root density, as in Section 8.1. It is separate from \(b>j\). The spatial weights are normalized to lie between zero and one.

Equation (SR.24) therefore supplies the missing ordinary E input to the boundary-induction argument's already repaired normalization and positive-root arguments. Together with the retained fixed-fiber normalization, local cumulant estimate, once-paid linear transport and running-tail induction, under CR this gives the C05 estimates on every history admitted by that fixed source construction and the stipulated AF trajectory. The original stronger per-term \(j-b\) Ward assertion is not restored or required.

These implications assume CR. The AF trajectory is not constructed here. C06/C08 retain their own direct derivative/readout requirements, and the remaining Yang–Mills existence obligations keep their separate status.
