# M-07. A positive curvature majorant and a local transfer on a clean chart

**Result.** All 21 analytic one-field stencils admit a positive majorant which agrees exactly with the specified Wilson energy on real links. For a homogeneous clean background in a global weak-link chart, a local gauge construction gives a coarse-curvature estimate with an additive unit in energy units. The unit pays for the distant transition of the gauge. On the real clean full-torus step, the actual interacting conditional fluctuations add bounded energy per fine plaquette. The estimates are uniform in the volume on the chart specified below. M-07 remains open. In particular a deterministic estimate for a direct minimizing background is only one part of the iterated, normalized, interacting map. [M-07 theorem](../../THEOREMS_AND_OPEN_PROBLEMS.md) · [Analytic family, §§8–13](M07_analytic_family.md)

## 1. Positive complex curvature and the 21 stencils

For a based plaquette matrix \(P\in SL_N(\mathbb C)\) set
\[
 e_+(P)=\tfrac14(\|P-I\|_{HS}^2+\|P^{-1}-I\|_{HS}^2).
 \tag{1}
\]
Use \(R^+_{h,X}=1+\sum_{p\subset X}\beta_p e_+(P_p)+\sum_{i\subset X}|z_i|^2\), with precisely the specified footprints. Take the shifted envelope by (M.6) on real configurations. Both orientations give the same energy. Unitary changes of frame preserve it, and conjugation by \(v\) multiplies it by at most \(\|v\|_{op}^2\|v^{-1}\|_{op}^2\). This frame qualification matters on a complex gauge orbit. On the compact slice \(e_+(P)=N-\operatorname{Re}\operatorname{Tr}P\) exactly, including large plaquettes.

The analytic continuation of the Wilson scalar obeys
\[
 |N-\tfrac12\operatorname{Tr}(P+P^{-1})|
 =\tfrac12|\operatorname{Tr}[(P-I)(I-P^{-1})]|\le e_+(P).
\]
Also \(\|P-P^{-1}\|_{HS}^2\le8e_+(P)\). Continue each based clover with inverse in place of adjoint. Trace projection has HS norm one. Cauchy–Schwarz in the finite clover sum and in the trace of two clovers bounds every repaired diagonal and off-diagonal component, including the scalar subtraction/addition, by \(C h^{-4}\sum_{p\in\mathrm{stencil}}\beta_p e_+(P_p)\) in the homogeneous energy normalization. Rotating the starting corner of an elementary plaquette uses at most three links, with a fixed norm cost on a weak complex-link chart. Fixed channel coefficients multiply the bound by their displayed operator norm. Field normalizations from F-05 are separate. The regulator is used only in estimates, so holomorphy is required of the stencils and maps, not of (1). [F-01 stencils and M.13–19](../../foundations/Annex_Y.md)

As a test, for \(P=I+tE_{12}\) the analytic Wilson scalar vanishes, while (1) gives exactly \(|t|^2/2\). With \(t=0.031i\) these values are 0 and 0.0004805. A second check over 1,000 near-identity complex \(2\times2\) matrices normalized to determinant one gave a largest observed ratio of absolute Wilson scalar to (1) of 0.999201. The two matrix inequalities above supply the proof for every \(N\).

## 2. Local background transfer

Use coarse units and a homogeneous, whole-torus determining set with terminal mesh one. Let \(\eta=L^{-a}\) denote the fine observation mesh for the direct, depth-\(a\) variational problem; it is not the running inverse coupling. Take the branch of the **actual** homogeneous minimizing map about the identity data with its smooth relative Landau representative, as in CMP102 Proposition 9. At the identity the real minimum is flat. On a fixed absolute determining-data disc, (190) gives a kernel for its derivative in the log determining links \(B\). For a local observation at coarse cube \(x\), its value, physical gradient and interior localized Hölder-gradient rows are bounded by \(C\exp[-\delta d(x,e)]\). The terminal factors \((L^j\eta)^{-1},(L^j\eta)^{-2},(L^j\eta)^{-2-\nu}\) and the determining measure in (190) all have unit scale here. Choose one admitted Hölder exponent \(0<\nu<1\), and a fixed smooth cutoff equal to one on the subcube where the Hölder row is used. The constants are uniform in \(a\) in these physical units. This use takes the published derivative estimate as input. [CMP102, pp.305–309, (172), (181), (190)](https://doi.org/10.1007/BF01229381)

**A test chart with no gluing.** Suppose the only nonidentity coarse links are in a separated family and that for each such link there is an incident plaquette with its other three links equal to identity. Then \(\|B_e\|\le C\sqrt{e_+(P_e)}\) on the small log disc. The fine field in the smooth chart is \(\exp(i\eta A)\), and \(A(B)=\int_0^1 D A(tB)[B]dt\). Applying (190) on this very segment gives
\[
 |A|+|\nabla_\eta A|\le C\sum_q e^{-\delta' d(x,q)}\sqrt{e_+(P_q)}.
 \tag{2}
\]
The same bound holds for the localized Hölder seminorm of the gradient. Plaquette expansion now yields \(\|P_{\rm fine}-I\|\le C\eta^2\) times the right side. The linear term is the physical curl times \(\eta^2\). The remaining products are bounded by \(C\eta^2\sup|A|^2\) in the fixed small chart. There is no real-centre error on this example. It includes complex nonnormal links such as the nilpotent test above.

**A larger chart with a logarithmic box.** Suppose the coarse determining links have a representative in which
\[
 \sup_e\|\log V_e\|\le\epsilon,\qquad
 \epsilon\le C g_c(1+\log g_c^{-2})^q,\qquad \beta_c\asymp g_c^{-2},
 \tag{3}
\]
with fixed \(q\). A real gauge change is allowed in obtaining (3). Fix a coarse observation cube \(x\), use the supremum metric for boxes, and choose
\[
 R=R_0+\lceil A\log(2+\sqrt{\beta_c}\epsilon)\rceil .
\]
Here \(A,R_0\) are fixed in terms of the decay rate. Require that the periodic lattice have side greater than \(4R+10\) in coarse units. The analytic map requires a *fixed absolute* data disc, and \(R\epsilon\) tends uniformly to zero as the coupling ceiling decreases. In particular, the logarithmic box does not impose a fixed bound on \(\sqrt{\beta_c}\epsilon\).

Inside the radius-\(R\) box use the coarse gauge \(v(y)\) given by the transport from the box centre to \(y\) on the coordinate-ordered path. Set \(v=I\) outside. This is an exact vertex gauge, including on crossing bonds. On the box \(\|v^{\pm1}\|\le e^{C R\epsilon}\) and \(\|v-I\|\le C R\epsilon\). Every transition link of \(V^v\) consequently lies in the log disc with log norm at most \(C(R+1)\epsilon\). Exterior links away from this transition are unchanged. For an interior link at distance \(r\), its transformed value is the product on the coordinate-path loop through the link. Sorting its path by elementary adjacent interchanges and cancelling retraced edges takes at most \(C(1+r)^2\) plaquettes inside radius \(r+C\). Each intermediate word has length at most \(C(1+r)\). Telescoping the *words* therefore costs at most \(C e^{C R\epsilon}\) times the sum of their plaquette defects. This proves
\[
 |\log (V^v)_e|\le C(1+r)^2\max_{d(x,q)\le r+C}\sqrt{e_+(P_q)} .
 \tag{3a}
\]
The principal logarithm here is valid independently of this last upper bound, since the entire word is within \(C R\epsilon\) of the identity. This construction does not integrate the original real centre from identity in an unspecified local gauge.

Take the actual analytic determining-data path \(V_e(t)=\exp[t\log(V^v)_e]\). Every one of its links is in the absolute disc of Proposition 9. At zero it is exactly the identity; at one it gives the gauge transform of the original data. Sum (3a) against the endpoint kernel (190). There are at most \(C(1+r)^4\) coarse links in the radius-\(r\) ball. Bound the maximum in (3a) by a sum over its ball and interchange the sums. All the polynomial factors are then absorbed in a reduced exponential. The exterior and transition terms together cost at most \(C(R+1)\epsilon e^{-cR}\le C\beta_c^{-1/2}\). Thus in the smooth representative belonging to the transformed data, on the observation stencil,
\[
 |A|+|\nabla_\eta A|\le C D_x,\qquad
 D_x=\beta_c^{-1/2}+\sum_q e^{-c' d(x,q)}\sqrt{e_+(P_q)} .
 \tag{4}
\]
One may always additionally use \(C R\epsilon\) as a small absolute bound. The cutoff version of \([\nabla_\eta A]_\nu\) obeys (4) wherever its cutoff is one. Equation (181) identifies the axial raw-data solution under the block-constant lift of \(v\). On real data all representative changes are unitary. On complex data (4) estimates the energy in the chosen smooth representative. Gauge-invariant traces of its stencils agree with the analytic continuation of the physical ones by covariance and continuation from real data. A matrix norm in an independently prescribed complex gauge would require bounds on that additional converter. This proof does not assume that every globally clean real orbit has a global representative satisfying (3). [CMP102, pp.307–309](https://doi.org/10.1007/BF01229381)

For a fine plaquette in this chart the result is
\[
 \beta_f e_+(P_{\rm bg})\le
 C\,\frac{\beta_f}{\beta_c}\eta^4
 \left[1+\sum_q e^{-c'd(x,q)}\beta_c e_+(P_q)\right].
 \tag{5}
\]
It follows from the elementary plaquette expansion used in (2), followed by the weighted Cauchy–Schwarz inequality and the uniform coarse-lattice exponential row sum. The prefactor \(\eta^4\) cancels the four-dimensional count in summing over the descendants of a coarse cell. The \(1\) can be omitted in the separated-link example. A single sharp local bound gives a tail over *all* coarse plaquettes. An exact carrier decomposition for a normalized insertion still requires localization.

At a later physical scale the pre-fluctuation links are the actual raw averages \(V^{(k)}=M^k(U_{k+1})\). The one-step native background also satisfies (5), with \(\eta=L^{-1}\), on (3) and a complete local averaging footprint. To see the extra point required here, apply the value and gradient rows at the underlying fine mesh in coarse physical units throughout the footprints of the four output links. Those footprints have bounded coarse diameter, so each right side in (4) is bounded by a fixed multiple of \(D_x\). Apply the already proved local two-power averaging estimate BM.17–19 there with identity reference, \(h_n=1\), \(h_p=L^{-1}\), and \(u=C\min(D_x,R\epsilon)\), reducing the coupling ceiling as needed. One ordered axial frame on the union of the four footprints gives a bound \(Cu L^{-2}\) for each gauged average's log, hence for their plaquette. Equivariance gives the same real energy and the same invariant trace statements as above. This argument also applies when the observed averaging length in coarse units is \(L^{-a}\) on the direct homogeneous background. It asserts no equality of that background with a composition of \(a\) interacting conditional expectations. [BM.17–21](../../foundations/Annex_AF.md) and [C-01 (3.4)](../../foundations/Annex_W.md) · [CMP109, p.263](https://doi.org/10.1007/BF01215223)

**A weaker adjacent-curvature gain suffices for the bilinear power count.** For adjacent parallel elementary plaquettes inside a region with the Hölder cutoff equal to one, compare them after transport along their connecting fine link. In the smooth chart, expand the product of four exponentials to degree two in \(\eta A\). Its linear difference is \(\eta^2\) times a difference of first difference quotients bounded by \(C\eta^\nu D_x\). The quadratic terms are fixed bilinear polynomials in nearby \(A\)'s. Their translated difference is at most \(C\eta^3 D_x^2\) by the gradient bound. The cubic remainders are \(O(\eta^3 D_x^3)\); in these products use the small absolute bound just after (4) for all but one factor. Conjugating the second plaquette by its connecting link adds \(O(\eta^3 D_x^2)\). Passing to the principal logarithms uses a bounded differential. Hence the transported difference of log curvatures is \(O(\eta^{2+\nu}D_x)\). The separated bilinear term with one such difference costs \(L^{4a}\eta^{4+\nu}=L^{-\nu a}\) in this degree count. This result uses the Hölder row actually printed in (190). It gives neither the full Lipschitz estimate in (12.2) nor an adjacent-difference estimate for arbitrarily iterated *raw averages* of the smooth links. Stencils crossing the cutoff boundary need an overlapping Hölder patch for the same conclusion.

## 3. Fluctuation energy for an actual real clean step

Specify the slice precisely. All preceding and present blocks are regular, the current free-bond region is the whole periodic native lattice, there are no inherited large-field components or exterior force, and the coarse data are real and admitted in the source's homogeneous regular chart. The real support for the normalized independent variables \(z_i\) is the fixed product of symmetric norm balls of radius \(P_k=A_1(\log g_k^{-2})^{p_0}\). Here the complete real density in C-01 is
\[
 d\nu_t=Z_t^{-1}{\bf1}_{D}\exp[-z^{\mathsf T}Kz/2+tW(z)]\,dz,
 \qquad 0\le t\le1.
\]
\(K\) is the constrained precision at the fixed real background. \(W\) includes the regular effective-action difference, complete nonlinear classical remainder and Haar/coarea logarithms. At \(t=1\) this is the interacting conditional law on this specified slice. A general regular component with an exterior force or previously retained boundary does not satisfy this description. [Complete homogeneous density and estimates, Annex F §§1–3](../../foundations/Annex_F.md); [C-01](../../foundations/Annex_W.md) and [C-07](../../foundations/Annex_AA.md) · [Primary conditional integral, CMP119 (3.15), (3.25)](https://doi.org/10.1007/BF01217741)

Here is a direct check on the running logarithmic window. The regular gradient and Hessian budgets are DS.9–10. The localized classical remainder is cubic on a larger current disc \(2P_k\), with amplitude bounded by \(C g_k^{-2}(g_kP_k)^3\) times a summable carrier norm; the normalized measure logarithms have bound \(C g_kP_k\) times such a norm. One Cauchy derivative and the anchored sum give
\[
 \sup_{z,i}|D_iW|\le D_k=C(P_k^{-1}+g_kP_k^2+g_k).
 \tag{6}
\]
The real Hessian budgets also follow from HC.20–24 and DS.10 after choosing their fixed radii and then reducing the coupling ceiling. They apply throughout the interpolation since \(0\le t\le1\). These estimates, the principal gap, and the actual convex product support give the weighted covariance inequality (Annex F (1.19), C7.2) and a gap \(\lambda>0\) for every real linear tilt. The symmetric restricted quadratic law has zero mean. Thus
\[
 |\nu_1 z_i|\le\int_0^1|\operatorname{Cov}_{\nu_t}(z_i,W)|\,dt
 \le C D_k\sum_j e^{-\gamma d(i,j)}\le C D_k .
\]
The log-mgf of a centred unit component of \(z_i\) has second derivative bounded by \(1/\lambda\) under every linear tilt, by the convex Poincaré inequality. Hence \(\|z_i\|_{L^p(\nu_1)}\le C\sqrt p\) for \(p\ge1\), uniformly in depth and volume. Annex F Theorem 2.1 already proves a sharper \(O(g_k)\) mean on its own fixed-domain homogeneous law. The new use here is the estimate of the native energy relative to (5). [Annex F](../../foundations/Annex_F.md), [AH](../../foundations/Annex_AH.md) and [AI](../../foundations/Annex_AI.md)

Use the actual local chart \(V_k(z)=e^{i\theta(z)} V^{(k)}\) with \(\theta(z)=g_kCz-hD(g_kCz)\). Its local row estimate (5.3) in the recentered constraint-chart proof, integrated from zero along the real support, yields \(\|\theta_e(z)\|\le Cg_k\sum_i e^{-\gamma d(e,i)}|z_i|\). Telescoping four unitary link factors bounds each plaquette difference by the sum of this bound on its edges. Since \(\beta_k g_k^2\le C\), Minkowski and the coordinate moments give
\[
 \|\beta_k e_+(V_k(z)_p)\|_{L^s(\nu_1)}
 \le C\{\beta_k e_+(V^{(k)}_p)+s\},\qquad s\ge1 .
 \tag{7}
\]
A retained free-coordinate energy \(|z_i|^2\) likewise has \(L^s\) norm at most \(Cs\). In (7) real gauges may change with the centre since they preserve the HS norm. Combining (5) and (7), for a union of full descendants of a set of coarse cells \(X'\), gives a one-step bound for the plaquette part
\[
 C\frac{\beta_k}{\beta_{k+1}}\sum_{x\in X'}
       \left(1+\sum_q e^{-c'd(x,q)}\beta_{k+1}s(V'_q)\right)
 + C s L^4 |X'|.
 \tag{8}
\]
A fixed halo covers crossing plaquettes. Equations (1) and (8) bound the real conditional expectation and all \(L^s\) norms of each **incoming native** energy-normalized stencil after multiplication by \(h_k^4\). They do not compute its extracted coarse field, the transport of an arbitrary previously renormalized mark, or the identity counterterm.

For comparison, on a *fixed reference Gaussian* with covariance \(C\) of bounded operator norm, a centred whitened linear row \(\ell W\) satisfies \(\|\ell W\|_{2s}\le C\sqrt{s}\|\ell\|_2\). Conditioning on a symmetric convex cutoff preserves this estimate via the same tilt argument applied in whitened coordinates, since every tilt has Hessian \(I\). Complex coefficients can be split into real and imaginary parts. This gives finite local moments for an explicit Gaussian majorant whenever the actual rows used in the coordinate map have the stated bound. The extension of (7) to a normalized **complex interacting** expectation requires control of its numerator and denominator, uniformly on the prepared domain. Positivity of the real law and the centred Gaussian estimate do not establish that control. Nor does a sum of one-step uncentred moment estimates imply that the fluctuation cost of an iterated interacting map is precisely linear in its age.

## 4. What converts to the specified M-03 norm

For a local analytic activity on a fixed homogeneous regular chart suppose that its actual constituent obeys \(|A_Y|\le h^{-4}a_Y R^+_{h,Y}\) on the required complex tubes. Here \(Y\) includes every plaquette and native-coordinate dependency of that constituent. The real value envelope then gives \(h^4 A_Y^\sharp\le a_Y\widehat R_{h,Y}\) directly on shifts remaining in the chart. A radial upper bound with tails over the entire torus such as (8) still needs an exact local representation before this statement applies.

There is also a direct finite-difference conversion. At a real group perturbation in (M.3), extend the parameter to a complex disc of radius \(r>0\) about every \(t\in[-1,1]\). Assume these discs are admitted and \(r\le1\). Each affected based plaquette differs from its real value at \(t\) by at most \(C r/(1+\beta_e)^{1/2}\), with the same bound for its inverse. This follows by telescoping the at most four bounded link factors. On a homogeneous chart \(\beta_p/(1+\beta_e)\le C\) on the stencil. Hence
\[
 R^+_{h,Y}(\tau_{t+w}x)\le C\widehat R_{h,Y}(x),\qquad |w|\le r.
 \tag{9}
\]
For a normalized Euclidean-coordinate shift the corresponding square changes by at most \(2|z_i+t|^2+2r^2\). Cauchy at every point on the real segment and integration over that segment give \(h^4|\delta_\tau A_Y|\le C r^{-1}a_Y\widehat R_{h,Y}\). Summing over the \(n_Y\) elementary real *continuous* directions costs at most \(C r^{-1}n_Y\). If the value estimate is for the explicit integrand pullback at fixed kernel, this proves the corresponding smooth direct-difference contribution whenever the same envelope holds after integration. For a bound just on the final analytic scalar, the conclusion controls the total smooth finite difference; it cannot split the direct and kernel records in (M.29). Actual shifts crossing an ambient sector edge, discrete replacements and varying normalizers retain their own differences.

To see the moment cost explicitly, suppose \(\|\widehat R_{h,Y}\|_{L^p(\mu_h)}\le D_Y p\) for the actual law on which the converted record is claimed. Then (M.8) gives the value moment with coefficient \(a_YD_Y\) and the smooth difference moment with coefficient \(C a_YD_Y n_Y/r\), even with target grade \(3/2\). The pointwise denominators in (M.11) only improve the latter since \(\widehat R\ge1\). This identifies the extra input that is lost if the regulator denominator in a complex supremum is mistaken for an averaged estimate. On a connected carrier, \(\mathsf t_h(Y)=|Y|-1\), so the specified weight is \(e^{\kappa(2|Y|-1)}\). The representation must retain sufficient decay for that weight and the indicated costs after footprint closure. An unqualified AF weight \(e^{\kappa|Y|}\) at the *same* numerical exponent cannot pay it. [M.2–12 and M.28–32](../../foundations/Annex_Y.md)

There is an actual moment check at the first coarse scale. On the first, globally regular branch the coarse links are the raw one-block averages of the microscopic links, up to real gauges. For a coarse plaquette take its four averaging footprints in a fixed enlarged box of side \(C L\) in bare units. Fix an axial tree there. In this finite box, sorting paths as in (3a), now on unitary fields, bounds the deviations of all tree-gauged fine links from identity by \(C_L\sum_{p\in Y^+}\|U_p-I\|_{HS}\). If a fine plaquette exceeds a fixed threshold chosen at this fixed \(L\), the compact coarse energy is bounded by \(C_L\sum_{p\in Y^+}s(U_p)\) trivially. Otherwise every tree-gauged fine link is in a fixed small neighborhood where the actual one-step raw averaging operation is analytic, sends identity to identity, and has a bounded derivative on this finite input box. Apply it to the four coarse links and square the bound. Thus
\[
 s((MU)_q)\le C_L\sum_{p\in Y^+(q)}s(U_p).
 \tag{10}
\]
There is no power of the inverse coupling in \(C_L\). The augmented positive source-free law preserves the bare Wilson marginal. On the cofinal geometry of the established microscopic moment reserve (M.14), with \(\beta_1/\beta_0\le C\), (10) yields
\[
 \|{\bf1}_{\rm clean}\sum_{q\subset Y}\beta_1s(V_{1,q})\|_{L^p(\mu_1)}
 \le C_L |Y|p.
\]
This is the unnormalized sector contribution to an actual full-law moment. Dividing by the probability of the globally clean history is unnecessary and could lose volume uniformity. On this branch there are no retained large-field coordinates. For continuous native perturbations of the homogeneous plaquette list the shifted moments follow from (9) on the compact slice, or directly from (M.19). The supremum over discrete sector changes in the *full* (M.6) and the full ambient supremum of recursively extended activities require their own records. Iterating (10) alone produces a power of \(C_L\), which is unsuitable for the specified depth-uniform conclusion. Bare reserve and positive lift, [Annex W](../../foundations/Annex_W.md) and [Annex Y](../../foundations/Annex_Y.md) · [Actual one-step raw mean, CMP109 (0.11)–(0.12)](https://doi.org/10.1007/BF01215223)

## 5. Localization of a marked analytic function

On a finite set of decoupling variables suppose \(F(s,V)\) is analytic for \(|s_i|<R\), \(R>1\), bounded on smaller closed polydiscs by a common majorant. Define
\[
 F_S(V)=\sum_{T\subseteq S}(-1)^{|S|-|T|} F(\mathbf 1_T,V).
 \tag{11}
\]
The inactive coordinates of \(\mathbf1_T\) are zero. By inclusion–exclusion this selects exactly the Taylor monomials **at zero** with support \(S\), evaluated at one. Consequently \(\sum_S F_S=F(\mathbf1,V)\). If every switched-off configuration restricts the normalized insertion to the connected component of its anchor, a disconnected part of \(S\) has no influence on \(F(\mathbf1_T,V)\) once the other coordinates outside \(S\) are zero. Its alternating sum vanishes. If the restricted polydisc for \(S\) has bound \(B_S(V)\), absolute coefficient Cauchy estimates give, with \(r\uparrow R\),
\[
 |F_S(V)|\le B_S(V)\prod_{i\in S}\sum_{m\ge1}R^{-m}
            =B_S(V)(R-1)^{-|S|}.
 \tag{12}
\]
Thus with at most \(B A^j\) rooted supports of size \(j\), any weight \(e^{\varkappa j}\) is summable if \(Ae^{\varkappa}<R-1\), including fixed polynomial losses in \(j\). For M-03 use the actual doubled weight discussed above. CMP116 (1.10) uses decoupling with exterior parameters set to zero. At the physical point \(s=1\) a Taylor series in \(s-1\) has only its constant term left, which can itself be nonlocal. Equations (11)–(12) explain what must be verified for the actual *normalized marked* integral: the restricted-polydisc majorant against its local regulator, zero-free normalized kernels, and component factorization on the switched-off sets. A bound only at \(s=1\) gives none of these by Cauchy. [CMP116, (1.7)–(1.11)](https://doi.org/10.1007/BF01239022)

## Remaining steps

The weak-link proof controls the physical homogeneous map on its stated chart; the general clean centre is only locally regular in the admitted gauges. Extending (5) to that class requires a localization or comparison with uniform transition and topology costs. The full family also needs complex normalized fluctuation estimates, exact normalized carrier localization and the raw-average adjacent comparison wherever the bilinear subtraction uses it. The fixed-window test in (13.1) requires \((\varkappa-\log A_d)(1-C'/L^n)>2\log A_d\) with slack for the large-carrier term; the M-03 weight and intermediate analytic/KP losses must fit in the same parameter choices. The extraction onto the actual 21-field basis and identity, irreversible growth of constants under naive repeated transfer, the higher contact kernels, and the separate normalized kernel/interface and outer retained-data responses remain open. The all-scale assertion of M-07 is not proved by this clean, one-field calculation.
