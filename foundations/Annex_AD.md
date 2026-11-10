# Actual E contours and uniformly summable derivatives

**Annex AD.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Result and a correction to the preceding domain conditions

Under the stated source-free construction hypotheses, Theorem E14.3 supplies a common native complex contour for the regular E contribution and summable old-age majorants before Cauchy differentiation. The contour includes the native background, the independently extended current and the preparation parameters. Boundary activities B, complete conditional coercivity and matching after a change of retained coordinates require separate estimates. Identification with the Wilson conditional law requires CL.

There is a useful correction to the source estimates. CMP119 p.259 places a primitive E activity on the regular space \(U_j^c(X,\alpha_{0,j},\alpha_{1,j})\) of CMP109 (1.11)-(1.16). The multiscale space defined in CMP119 (2.34)-(2.39), pp.260-261, is introduced for the boundary activities B. A primitive E activity should not itself be assigned all the B-domain conditions. The latter re-enter when an E expression is localized across a multiscale boundary. This distinguishes the interior and boundary admission problems; it does not discard the boundary contribution.

The primary source already resums the old E scales before stating its current-scale analytic activity bound. Differentiating that resummed identity on a verified common complex domain is a viable alternative to charging every primitive old-scale Cauchy cost separately. Sections 5.1–5.6 control its running-domain margin and retain the coefficient-order dependence of the old-scale constants.

No Gaussian substitution, source-dependent background, or deletion of an inherited counterterm is made below.

### 2. The precise primary inputs

See CMP119, pp. 247, 250, 255, 259–263, 265, 267–268 and 275–284, CMP102, p. 285, (44), Proposition 9 and (172), (179)–(190), and CMP99, pp. 391–392 and 404–406.

The source chain used here is:

1. **Primitive regular domain.** CMP109 (1.11)-(1.16) distinguishes a real representative, its relative complex field, the independent current, and reconstructed fields. The paragraph on p.263 after (1.16) gives a sufficient smaller basic domain: the basic conditions (i)-(iii), with appropriately reduced constants, imply the reconstructed conditions. Its displayed estimates use the constant \(2B_3\) from the minimizing-field theorem. One therefore need not independently rebuild every reconstructed constraint after proving admission to that smaller basic domain.
2. **Independent-current insertion.** CMP109 (3.11)-(3.14) replaces the second-order operator in the localized current by the covariant Laplacian, the projection term and the displayed local corrections. The controlled insertion norms include \(A,P_UA,\nabla_UA,\Delta_UA\). The physical-current identity for an unlocalized Landau-gauge minimizer is not imposed separately on each localized summand.
3. **A native additive margin.** CMP109 Lemma 4, (3.53), admits an extra coarse determining-field input \(B'\), uniformly along the real parameter interval of the expansion. The proof displays restrictions of the form
   \[
   B_3\alpha_3<\alpha_1/2,\qquad
   C_{51}\alpha_3\le\beta L^{-2}\alpha_0.
   \tag{E14.1}
   \]
   Here \(C_{51}\) denotes the fixed coefficient in the derivative estimate (3.51); no ambiguous printed superscript is used as a numerical value. Thus there is a source-native additive margin with a linear dependence on the displayed radii, after the other hypotheses of that lemma have been met. This is more information than membership in an open analytic set. It is not yet a margin on the full current-coordinate support.
4. **Preparation and old-scale summation.** CMP116 (1.11)-(1.22) control the actual localized minimizing map with complex decoupling parameters. Lemma 1, (1.33)-(1.36), then states the jointly analytic, localized E fluctuation identity after the old scales have been summed. CMP119 p.276 transfers the interior construction to the complete geometry and gives a different multiscale domain for the remaining boundary terms.

These are source-scoped inputs, with their published parameter and regularity hypotheses retained.

### 3. Quantifying the actual native preparation

#### 3.1 The maps and the source losses

Write \(z\) for the free current fluctuation field called \(B\) in CMP116. This temporary notation avoids confusing it with the coarse determining-field input in CMP109 Lemma 4. The exact input map in CMP116 (1.19) is

\[
 b'(z)=g_k C z-hD(g_k C z).
 \tag{E14.2}
\]

Here \(C,h,D\) are the actual constraint-elimination and nonlinear linearization maps of that construction. They are not replaced by their linear parts.

For a localized decoupling family \(s\), the minimizing response is

\[
 \mathcal H_s(b')
 =H_0(s)b'+A_0(s,H_0(s)b')
 -H(s)D\!\left(H(s),H_0(s)b'+A_0(s,H_0(s)b')\right).
 \tag{E14.3}
\]

This is CMP116 (1.17). Its operators depend on the same external field and independent current as the original construction.

Put

\[
 K=B_0e^{16\kappa_1}.
 \tag{E14.4}
\]

The source controls the localized propagators by \(K\), in all their admitted regularity norms, simultaneously for
\[
 |s(\Delta)|\le e^{\kappa_1}.
 \tag{E14.5}
\]

With \(C_B\) denoting the source constant in (1.20), the ensuing bounds are

\[
 \|b'(z)\|_\infty\le C_B g_k\|z\|_\infty,\qquad
 \|\mathcal H_s(b'(z))\|_{\mathrm{adm}}
 \le4KC_Bg_k\|z\|_\infty.
 \tag{E14.6}
\]

The norm \(\|\cdot\|_{\mathrm{adm}}\) means the collection of regularity norms actually used in this source step, including the relevant second-order output. Uniformity in the allowed external variables is part of the stated native domain. It is not asserted on an arbitrary enlarged domain.

The proof in CMP116 uses two auxiliary radii. The displayed sufficient inequalities include

\[
 4C_2K\varepsilon_2\le1,\qquad
 4C_4K^2\varepsilon_3\le1,\qquad
 2K\varepsilon_3\le\varepsilon_2.
 \tag{E14.7}
\]

These inequalities expose the preparation cost. In particular, it is not legitimate to call the localized map a contraction with its original unlocalized constant and omit \(e^{16\kappa_1}\).

#### Proposition E14.1 — an explicit native reserve

Retain all the source's external-field and propagator hypotheses. Let \(\varepsilon_{\mathrm{abs}}>0\) be a fixed admitted ceiling for its local analytic maps and the remaining fixed smallness conditions. Let \(C_\zeta\ge1\) bound multiplication by the cutoffs used in the insertion norm. Define

\[
\begin{split}
 e_2&=\min\{\varepsilon_{\mathrm{abs}},(16C_2K)^{-1}\},\\
 e_3&=\min\{\varepsilon_{\mathrm{abs}},e_2/(4K),
                         (16C_4K^2)^{-1}\},\\
 e_1&=\min\{\varepsilon_{\mathrm{abs}},e_3/(2C_B),
                         \alpha_2/(32C_\zeta KC_B)\}.
\end{split}
\tag{E14.8}
\]

The actual map (E14.3) is analytic for the source's external variables, the simultaneous preparation parameters (E14.5), and

\[
 g_k\|z\|_\infty<e_1.
 \tag{E14.9}
\]

All the inequalities (E14.7) hold with a strict numerical reserve. Moreover, its insertion output has

\[
 C_\zeta\|\mathcal H_s(b'(z))\|_{\mathrm{adm}}
 \le\alpha_2/8.
 \tag{E14.10}
\]

The extra insertion parameter \(t_\square\) can be admitted simultaneously on

\[
 |t_\square|\le T_*,
 \qquad T_*=\frac{\alpha_2}{16C_\zeta KC_Be_1}\ge2,
 \tag{E14.11}
\]

along with the real parameter \(0\le t\le1\). In particular the sum
\((t\zeta+t_\square\zeta_\square)\mathcal H_s(b'(z))\)
has insertion norm at most \(3\alpha_2/8\).

**Proof.** The first two minima give
\(4C_2Ke_2\le1/4\),
\(4C_4K^2e_3\le1/4\), and
\(2Ke_3\le e_2/2\). The next minimum gives
\(\|b'(z)\|<C_Be_1\le e_3/2\).
The analytic fixed-point construction in CMP116 (1.12)-(1.18) therefore applies on these smaller domains, with its displayed margins, proving (E14.9) and (E14.6).
The last term in the minimum gives (E14.10). The second summand with \(t_\square\) costs at most
\[
 C_\zeta4KC_Be_1T_*=\alpha_2/4.
\]
Adding the bound \(\alpha_2/8\) for the first summand gives the claimed strict insertion reserve. \(\square\)

This is a quantitative statement about the actual native nonlinear maps and simultaneous preparation variables. It does not assume a bound for a substituted Gaussian map. The source constant \(\alpha_2\) and the external-field domain have not been declared fixed under the subsequent running-domain transfer.

#### 3.2 The independently extended current has a genuine native direction

Within the regular domain, the independent variable \(J\) occurs in the basic current norm constraint. The reconstructed currents in condition (iv) are constructed from the field \(U\); they do not turn the independent \(J\) into a function of \(U\).

Consequently, with \(U\) fixed in an admitted smaller basic domain, an independent-current center \(J_0\) with
\(\|J_0\|_\infty<\gamma_*\) has the explicit native affine current margin

\[
 \rho_J=\gamma_*-\|J_0\|_\infty.
 \tag{E14.12}
\]

For \(\|\delta J\|_\infty<\rho_J\), all the current constraints on this independent variable remain satisfied. This is an immediate check of the source definition, and it remains simultaneous with (E14.9) and (E14.5). The actual real-center margin and the running prepared-current substitutions are quantified separately in Sections 5.2, 5.5 and 5.6.

#### Corollary E14.2 — all native current and preparation derivatives

Let \(z_0\) be a real center with \(\|z_0\|_\infty\le P\) and
\[
 P<e_1/g_k,\qquad \rho_z=e_1/g_k-P>0.
 \tag{E14.13}
\]

Take the external background in the smaller native domain just specified, \(J_0\) as in (E14.12), and a real preparation center \(s_0(\Delta)\in[0,1]\). After including a fixed Lie-algebra coordinate norm factor \(c_G>0\), the radii

\[
 r_z=c_G\rho_z,\qquad
 r_J=c_G\rho_J,\qquad
 r_s=(e^{\kappa_1}-1)/2
 \tag{E14.14}
\]

define a simultaneous product contour in all these variables. For multi-indices \(a,b,c\), the complete minimizing output obeys

\[
 \|\partial_z^a\partial_J^b\partial_s^c
       \mathcal H_s(b'(z))\|_{\mathrm{adm}}
 \le a!\,b!\,c!\,
       4KC_Be_1\,
       r_z^{-|a|}r_J^{-|b|}r_s^{-|c|}.
 \tag{E14.15}
\]

**Proof.** The current polydisc stays in (E14.9), the independent-current polydisc stays in its basic constraint, and \(|s_0+\delta s|<e^{\kappa_1}\). The same native bound (E14.6) holds uniformly on their product, since the native source construction is jointly analytic there. Multivariable Cauchy, applied to each of the admitted output norms, proves (E14.15). The finite Lie-algebra dimension determines \(c_G\); it does not introduce a factor equal to the number of lattice sites. \(\square\)

In particular, this calculation retains the nonlinear constraint map, independent current and complex preparation parameters simultaneously. It is stronger than estimating only the physical current of an unlocalized minimizing field. Its scope is the verified native domain, and its radius is displayed rather than presumed uniform.

#### 3.3 A linear reserve in the nearby-carrier preparation

The nearby-carrier proof supplies a further quantitative fact. In CMP109 (3.49), the extra coarse field \(Q'(A)\) generated by the insertion satisfies

\[
 \|Q'(A)\|_\infty
 \le C_Q L^j\eta\,\|A\|_{\rm reg},\qquad L^j\eta\le1,
 \tag{E14.15a}
\]

where \(C_Q\) is the fixed source constant and the regular norm is the one in (3.31). The argument (3.50)-(3.53) admits an independent additive coarse input of radius \(\alpha_3\), subject to (E14.1). Fix an admitted absolute ceiling \(\epsilon_*\), retaining the source's other background hypotheses, and choose

\[
 r_3=\min\left\{\epsilon_*,
         \frac{\alpha_1}{4B_3},
         \frac{\beta L^{-2}\alpha_0}{4C_{51}}\right\},
 \qquad
 a_{\rm near}=\min\left\{\epsilon_*,\frac{r_3}{4C_Q}\right\}.
 \tag{E14.15b}
\]

For \(\|A\|_{\rm reg}<a_{\rm near}\), \(0\le\tau\le1\), and an independent additive perturbation \(\|B''\|_\infty<r_3/4\), one has

\[
 \|\tau Q'(A)+B''\|_\infty<r_3/2.
 \tag{E14.15c}
\]

The source's simultaneous native inclusion therefore applies with a strict reserve. The proof is direct: (E14.15a) bounds the first summand by \(r_3/4\), the second has the same bound, and (E14.15b) makes both inequalities (E14.1) strict. This retains the actual nonlinear \(Q'\), rather than replacing it by its first derivative.

With \(L,M,\beta\) fixed and \(\alpha_1/\alpha_0\) fixed in the range required by the source, this yields

\[
 a_{\rm near}\ge c_{\rm near}\alpha_0
 \tag{E14.15d}
\]

once \(\alpha_0\) is below the fixed absolute ceilings. Thus the additional coarse input in the nearby-carrier argument does not itself force a superlinear loss of the running analytic radius. Its background-ratio hypothesis is real: the proof preceding (3.37) requires \(\alpha_1\) large compared with a fixed multiple of \(M\alpha_0\). Equal logarithmic exponents with an appropriate fixed ratio of their coefficients meet this displayed restriction. This calculation does not by itself prove the corresponding far-carrier current bound or admission of all running multiscale centers.

### 4. The resummed E identity and what its bound already accomplishes

CMP116 Lemma 1 identifies

\[
\begin{split}
 &E_k\!\left(U_k(e^{ib'(z)}V^{(k)})\right)
       -E_k\!\left(U_k(V^{(k)})\right)\\
 &\hspace{35mm}=\sum_Y V'_{k,Y}(U_{k+1},J_{k+1},z).
\end{split}
\tag{E14.16}
\]

Here \(E_k\) is the renormalized inherited action; its old coupling subtractions have already been included. The source proves a product analytic domain and a bound of the form

\[
 |V'_{k,Y}|
 \le \mathcal K_E e_1
        e^{-(1-2\vartheta)\kappa d_k(Y)},\qquad
 \mathcal K_E=E_0C_1M^q e^{C_2\kappa_1}.
 \tag{E14.17}
\]

The notation \(\vartheta\) distinguishes the fixed exponent loss from the cutoff radius. The constants in \(\mathcal K_E\) are those fixed by the native parameter choice. Their dependence must be retained if that choice changes.

The source summation preceding this lemma is substantive. In the nearby-carrier case its fifth-order factor pays the four-dimensional old-cell count, leaving a summable old-scale factor. In the distant-carrier case the source uses the spatial exponential and its scale-transfer inequality. Thus (E14.17) is a bound after old-scale summation, on one common native domain. It is not a primitive activity bound with an uncounted old-cell multiplicity.

Combining this source result with (E14.13)-(E14.14), for example, gives

\[
 |\partial_z^a V'_{k,Y}(z_0)|
 \le a!\,\mathcal K_Ee_1\,r_z^{-|a|}
        e^{-(1-2\vartheta)\kappa d_k(Y)}.
 \tag{E14.18}
\]

At \(P\le e_1/(2g_k)\), the current derivative cost is explicitly
\[
 a!\,\mathcal K_Ee_1
       \left(\frac{2g_k}{c_Ge_1}\right)^{|a|}.
 \tag{E14.19}
\]

Preparation differentiations commute with this estimate on a smaller common contour: the source's convergent expansion has a uniform majorant there. This step does not require a zero-free generating functional.

Equations (E14.15) and (E14.18) are source-domain consequences for actual maps and actual E activities. The running-background substitutions are verified in Sections 5.2–5.6; the native formulas alone would not justify an unverified substitution.

### 5. Testing an explicit running parameter choice

The conservative normalized real cutoff in the complete construction is

\[
 P_k=A_1\ell_k^{p_0},\qquad
 \delta_k=g_kP_k,\qquad \ell_k=\log g_k^{-2}.
 \tag{E14.20}
\]

This uses the normalized bound, regardless of the ambiguity in the printed later cutoff formula. Choose
\[
 e_{1,k}=2\delta_k
 \tag{E14.21}
\]
gives \(\mathscr R_{z,k}=e_{1,k}/g_k=2P_k\) and a margin \(\mathscr R_{z,k}-P_k=P_k\). This analytic radius is distinct from the source's geometric collar range \(R_k\). Substitution into the *actual* preparation budget (E14.8) reduces its principal insertion condition to

\[
 64C_\zeta K C_B\,\delta_k\le\alpha_{2,k}.
 \tag{E14.22}
\]

The other fixed native smallness conditions are then eventually satisfied because \(g_k\ell_k^{p_0}\) tends to zero. The right side of (E14.22) is supplied by the native local admission calculation and the whole-map argument in Sections 5.2 and 5.5.

Those calculations give
\[
 \alpha_{2,k}\ge c\,g_k\ell_k^q,\qquad q>p_0,
 \tag{E14.23}
\]
with the displayed preparation constants fixed; (E14.22) therefore holds whenever
\[
 \ell_k^{q-p_0}
 \ge64C_\zeta K C_B A_1/c.
 \tag{E14.24}
\]

Any finitely many additional inequalities \(C g_k\ell_k^b\le c_0\) have an explicit sufficiently small coupling ceiling. Indeed, for
\(\ell\ge16b^2\), the bound \(\log\ell\le\sqrt\ell\) gives
\(e^{-\ell/2}\ell^b\le e^{-\ell/4}\); it remains to require
\(\ell\ge4\log(C/c_0)\).

Section 3.3 proves the needed linear behavior for the extra coarse input in the nearby-carrier preparation. Sections 5.2–5.6 supply the far insertion, actual real-center and common native background/current margins. CMP119 (2.28) states \(q_0,q_1>1\) and sufficiently large constants. Equal exponents \(q_0=q_1=q>p_0\), with a suitable fixed ratio of coefficients, satisfy the displayed nearby-carrier requirements. The remaining fixed native map restrictions are imposed through the displayed minima and the common coupling ceiling. The real-center and old-scale comparison proofs use the complete construction on its actual admitted regular geometry; the numerical choice of exponents alone would not imply those inclusions.

Nor should one use the minimum of all unrescaled old \(\alpha_{2,j}\) as a common current radius: on an expanding ultraviolet trajectory it can tend to zero. The scale improvement of the actual old-coordinate map must enter before taking that minimum, or one must use the already-resummed common-domain theorem with its running constants.

#### 5.1 The actual coupling comparison pays the nearby scale change

The coupling comparison in CMP119 (2.6)-(2.7), pp.255-256, gives a quantitative improvement. Set \(a=k-j\), and take one fixed exponent \(q\) in
\(\alpha_{0,j}=C_0g_j\ell_j^q\). For the admitted source trajectory,

\[
 \frac{\alpha_{0,k}}{\alpha_{0,j}}
 \le C_{\rm AF}\sqrt{1+a},\qquad
 C_{\rm AF}=(1+\beta_0)^2.
 \tag{E14.24c}
\]

For \(a\ge1\), multiply the source's ratio bound for \(g_k/g_j\) by its bound for \(\ell_k^q/\ell_j^q\); for \(a=0\), the ratio equals one. This uses the actual age comparison, not a bound by the absolute ultraviolet cutoff logarithm.

At a native background for which the source's nearby preparation is admitted, (E14.6) and (E14.15a) give its complete current-dependent extra coarse field the bound

\[
 \|Q'_j(\mathcal H_s(b'(z)))\|_\infty
 \le Dg_k\|z\|_\infty L^{-a},
 \quad D=4C_QC_\zeta KC_B,
 \tag{E14.24d}
\]

Here \(\eta=L^{-k}\), so the factor \(L^j\eta\) in the displayed source estimate is exactly \(L^{-a}\). Suppose the absolute ceilings are imposed so that the actual nearby coarse radius from (E14.15b) satisfies \(r_{3,j}\ge c_3\alpha_{0,j}\). On the full product ball \(\|z\|_\infty<2P_k\), equations (E14.20), (E14.24c)-(E14.24d) imply

\[
 \frac{\|Q'_j(\mathcal H_s(b'(z)))\|_\infty}{r_{3,j}}
 \le
 \frac{2DA_1C_{\rm AF}}{c_3C_0}
 \ell_k^{p_0-q}L^{-a}\sqrt{1+a}.
 \tag{E14.24e}
\]

For \(L\ge\sqrt2\), one has \(L^{-a}\sqrt{1+a}\le1\) for every integer \(a\ge0\): use \(1+a\le2^a\) for \(a\ge1\). Therefore the explicit condition

\[
 \ell_k^{q-p_0}
 \ge \frac{8DA_1C_{\rm AF}}{c_3C_0}
 \tag{E14.24f}
\]

places this current-dependent input inside one quarter of its native coarse margin **simultaneously at every old nearby scale**. This calculation removes the putative obstruction from taking the minimum of unrescaled old radii. The real-center reserve is supplied in Section 5.2; the joint external-variable reserve is supplied in Section 5.6.

The fifth-order nearby remainder has a related summation. The source's coarse determining field has size at most a fixed multiple of \(\alpha_{0,k}L^{-a}\) on the admitted contour. Here the remainder is the integral Taylor remainder along the segment \(\tau B\), \(0\le\tau\le1\). Lemma 4 supplies the same additive \(r_{3,j}\)-tube at every point of that segment. Apply fifth-order Cauchy there and integrate the Taylor weight. No assertion that the Taylor series at zero converges all the way to \(B\) is needed. The resulting age factor is

\[
 C\left(\frac{\alpha_{0,k}}{\alpha_{0,j}}\right)^5L^{-5a}
 \le C C_{\rm AF}^5(1+a)^{5/2}L^{-5a}.
 \tag{E14.24g}
\]

Multiplying by the four-dimensional old-cell count \(O(L^{4a})\) leaves

\[
 \sum_{a\ge0}(1+a)^{5/2}L^{-a}<\infty.
 \tag{E14.24h}
\]

The convergence is uniform in total depth. Once all the activity arguments are admitted on the same current ball, further current differentiation can be performed after this majorized sum and costs \(m!P_k^{-m}\), with the fixed Lie-coordinate norm factor retained. This closes the running-age bookkeeping for this nearby **fifth-order remainder**. It does not replace the source's treatment of the lower-order subtraction terms, the distant carriers, or the complete running-background admission test.

#### 5.2 Actual real centers and the local relative-field comparison

The actual real centers are not arbitrary elements of the largest regular domain. The complete construction supplies stronger bounds. CMP119 p.275 identifies the minimizing field on each regular layer with a minimizing field at that layer's scale and transfers its regularity bounds; p.276 transfers the interior arguments of CMP109 Sections 3–4 with that scale. In CMP102 Theorem 1, membership in the regular space, defined in (2), includes both the plaquette and the physical-current bound. Its local gauges satisfy (9)–(10), including the derivative and second-order bounds. Thus the transfer is not a curvature-only assertion.

In a layer of scale \(n\ge j\), the resulting bounds in old \(j\)-scale units are

\[
 b_j(U_0)\le C_{\rm reg}\epsilon_n L^{-2(n-j)},
 \qquad
 \|J^{\rm phys}_j(U_0)\|_\infty
 \le C_{\rm reg}\epsilon_n L^{-3(n-j)}.
 \tag{E14.26}
\]

The regular-gauge field and its first derivative have the corresponding factors \(L^{-(n-j)}\) and \(L^{-2(n-j)}\). Here \(C_{\rm reg}\) is a fixed maximum of the constants in those source bounds, at fixed \(L,M\). This statement uses the actual local gauges specified in the source; it does not assert the existence of one globally small gauge potential across all history interfaces.

The actual coupling comparison gives
\(\epsilon_n/\epsilon_j\le C_{\rm AF}\sqrt{1+n-j}\). Consequently each of these native regularity bounds is at most a fixed multiple \(C'_{\rm reg}\epsilon_j\). Since

\[
 \frac{C'_{\rm reg}\epsilon_j}{\alpha_{0,j}}
 =\frac{C'_{\rm reg}A_0}{C_0}\ell_j^{p_0-q},
 \tag{E14.27}
\]

any fixed requested fractional reserve is obtained at every old scale by the explicit lower bound on \(\ell_j^{q-p_0}\) displayed in (E14.27). For example, the bound by \(\alpha_{0,j}/(64B_3)\) follows if
\(\ell_j^{q-p_0}\ge64B_3C'_{\rm reg}A_0/C_0\).
At a real center the relative complex field can be taken equal to zero. These deductions establish the smaller *real-center* reserve for the actual regular layers, under the source-scoped complete inductive representation. They do not by themselves establish a simultaneous complex tube through every subsequent substitution.

There is also a direct local comparison needed by that tube. On one of the admitted local gauges write \(U_0=e^{i\xi a_0}\), and take \(\|a_0\|_\infty\) below a fixed ceiling. Since

\[
 \xi^{-1}\|\operatorname{Ad}_{e^{i\xi a_0}}-I\|
 \le 2e^{2\xi\|a_0\|}\|a_0\|,
 \tag{E14.28}
\]

the ordinary and covariant first differences of any field \(B\) obey

\[
 \|\nabla B-\nabla_{U_0}B\|_\infty
 \le C_G\|a_0\|_\infty\|B\|_\infty.
 \tag{E14.29}
\]

This is a scale-independent estimate; the link displacement supplies the power \(\xi\) needed to cancel the difference quotient. The same observation controls composition of relative fields. The analytic map

\[
 \mathcal B_\xi(A,B)
 =\frac1{i\xi}\log(e^{i\xi A}e^{i\xi B})
 \tag{E14.30}
\]

has bounded first derivatives on a fixed small matrix chart, uniformly for \(0<\xi\le1\). The convergent BCH series starts with \(A+B\); every nonlinear term has at least one positive power of \(\xi\). Applying the discrete product rule, and (E14.29) to change the reference connection, gives

\[
 \|\mathcal B_\xi(A,B)\|_{H^1_\infty}
 \le C_{\rm cmp}
       (\|A\|_{H^1_\infty}+\|B\|_{H^1_\infty}),
 \tag{E14.31}
\]

with a fixed constant on that chart. The \(H^1_\infty\) notation denotes the supremum and first-difference norms used here, not an \(L^2\) Sobolev norm. A fixed Hölder first-difference norm can be included by the same product-rule estimate when it is required by the local regularity chart.

Together with the actual-current calculation in the supplement, (E14.31) removes the local coefficient obstruction to a linear insertion radius. More precisely, choose the real center as in (E14.27), an independent-current center satisfying the same smaller current bound, and relative-field and insertion perturbations whose required norms are all less than

\[
 u_j=c_{\rm loc}\min\{\alpha_{0,j},\alpha_{1,j}\},
 \tag{E14.32}
\]

where \(c_{\rm loc}>0\) is smaller than the reciprocals of the fixed constants in (E14.31), (LC.7), (LC.24), and the factor \(16B_3\) in the smaller-domain reconstruction test. The plaquette, relative-field and independent-current clauses then lie strictly inside the smaller basic domain. CMP109 p.263 supplies its reconstructed-field clauses, with its displayed factor \(2B_3\). This is a quantitative **native local admission** calculation, including reconstruction. Its restrictions are on the actual native norms; a bound on an input in different coordinates must still be transported to these norms by the actual source maps.

For a local coordinate description, the native norm ball is quantitative even on the fine lattice. The first-difference constraint is satisfied by a simultaneous scalar-coordinate polydisc of radii \(c_G\xi u_j\); the unscaled independent-current coordinates have radii \(c_Gu_j\). This follows from the bounded degree of the lattice stencil and (E14.29), with no factor equal to the total number of sites. The much larger current-coordinate radius in (E14.24f) is obtained only after using the smoothing preparation map; it is not inferred from these raw-link coordinate radii.

#### 5.3 Far-carrier summation with the actual derivative bound

For a distant old E carrier the native source gives more than a generic analytic function bound. CMP109 (3.8)–(3.9) applies the derivative of the actual old minimizing map to the prepared current input. It bounds the resulting field and each of the first- and second-order operators required in (3.14), with the factor \(L^j\eta\) and the separation exponential. Equation (3.17) performs the Cauchy insertion using that same collection of norms. The paragraph following it explicitly retains these bounds under the subsequent localization. For a large carrier the primitive carrier decay supplies the corresponding small exponential instead.

Write \(a=k-j\), so \(L^j\eta=L^{-a}\). On an admitted joint native contour, (E14.6) and that actual source bound give

\[
 |\mathcal E^{\rm far}_{j,X,\square}|
 \le C E_0 e^{-\kappa' d_j(X)}
       \frac{g_k\|z\|_\infty}{\alpha_{2,j}}
       L^{-a}e^{-cML^a}.
 \tag{E14.33}
\]

All fixed constants in (E14.33) include the preparation factor \(K\), the native norm-comparison constants and the fixed loss of carrier decay. For a large carrier, a fraction of its decay supplies \(e^{-cML^a}\) and the remaining fraction is the displayed carrier weight. This is the source's actual far-carrier derivative estimate; it is not an estimate obtained by replacing the nonlinear minimizing map with a Gaussian map or by dilating a projection from a different determining geometry.

In this common notation choose \(c\le\delta\kappa/M\) for the large-carrier branch, whose direct source factor is \(e^{-\delta\kappa L^a}\), as well as the separation constant for the other branch. The fixed \(M\)-dependence is retained; an \(M\)-independent value of \(c\) is not claimed.

If its insertion arguments satisfy the native norm reserve (E14.32), then \(\alpha_{2,j}\) may be chosen equal to \(c_2\alpha_{0,j}\), with fixed \(c_2>0\). On \(\|z\|_\infty<2P_k\), (E14.24c) yields the explicit age majorant

\[
 |\mathcal E^{\rm far}_{j,X,\square}|
 \le C E_0 e^{-\kappa'd_j(X)}
       \ell_k^{p_0-q}\sqrt{1+a}\,
       L^{-a}e^{-cML^a}.
 \tag{E14.34}
\]

After the four-dimensional old-cell count, the remaining sum is bounded by

\[
 \sum_{a\ge0}\sqrt{1+a}\,L^{3a}e^{-cML^a}<\infty.
 \tag{E14.35}
\]

This convergence is uniform in the total depth. For example, \(\sqrt{1+a}\le C_LL^a\), and \(x^4e^{-cMx}\le C_{cM}e^{-cMx/2}\); the remaining lacunary exponential series is finite. On one verified common current ball, the sum is holomorphic by this majorant and subsequent current Cauchy derivatives cost \(m!(c_GP_k)^{-m}\), independent of the old age. Thus the far *summation* is no longer an independent obstacle once its arguments meet the displayed native norm reserve.

The precise domain proviso matters. The source needs both the background part of the old insertion and the localized variation to satisfy (3.14), with the displayed spare fractions. The derivative estimate (3.9) supplies the latter. For the former, integrate the actual derivative along its defining coarse-input segment and use its value at zero, retaining the nonlinear reconstructed background. A change of determining geometry is handled by CMP102 (190), as in the source proof; it is not handled by declaring the old projection to be a dilation of the new one. Section 5.5 verifies this entire background segment on a fixed internal-map domain before testing the smaller E-activity radius. Equations (E14.33)–(E14.35) by themselves would not suppress that prerequisite.

#### 5.4 The Ward and coupling terms: a degree-preserving radius bounds

The fifth-order tail is not the complete inherited E action. The remaining terms can nevertheless be given a running-radius majorant without demanding that the final constant equal the strongest small native constant in (E14.17). This subsection concerns the actual nearby E decomposition of CMP109 Sections 4–5, with the matching source Wilson subtraction retained, on the common native contour used by that decomposition.

The source operations have the following finite decomposition. Let \(Q_k\le c_Q\alpha_{0,k}\) bound the regular coarse-background and prepared-insertion norms on this contour. Put \(r_j=c_r\alpha_{0,j}\), where \(c_r>0\) is a fixed smaller native analytic radius. Fix \(0<\theta<1\) in the source's irrelevant-term estimates.

| Actual source operation | Coefficient order and radius cost | Field factors retained | Geometric factor after subtraction |
|---|---|---|---|
| Integral tail in CMP109 (3.34), Lemma 4 | fifth derivative, \(CE_0r_j^{-5}\) | five factors, each of size at most \(CQ_k\) before its scale weight | \(L^{-5a}\) |
| Fourth-order terms, (4.21)–(4.29) | derivatives of orders \(r=2,3,4\), each costing \(CE_0r_j^{-r}\) | total field degree four; replacing a field by a difference does not lower that degree | \(L^{-(5-\theta)a}\) for the discarded terms |
| Third-order terms, (4.30)–(4.34) | orders \(r=2,3\) | total field degree three | \(L^{-(5-\theta)a}\) for the discarded terms |
| Vacuum-polarization remainder, Section 5 | order two, \(CE_0r_j^{-2}\) | degree two, or higher commutator terms with the same coefficient | \(L^{-(5-\theta)a}\) |
| Matching Wilson subtraction, (4.38)–(4.45) | \(|\beta_j|\le CE_0r_j^{-2}\) | degree at least two; the marginal degree-two expression cancels before summing old scales | \(L^{-(5-\theta)a}\) for its remaining terms |

The constants absorb fixed spatial moments of the source's exponentially decaying kernels and a fixed loss of carrier decay. They are independent of the old age. If polynomial factors in the length of an auxiliary localization box are retained instead of absorbed, write a fixed factor \((1+a)^{b_*}\) throughout; no derivative-order-dependent value of \(b_*\) is introduced.

Here is why the radius bookkeeping in this table is valid. The coefficients in (4.3) are obtained by a finite chain rule. A term involving \(r\) derivatives of the primitive E activity has \(r\) Cauchy denominators, while the derivatives of the minimizing map have the fixed regularity and tree-decay bounds given there. Its total degree \(n\) in the displayed fields is at least \(r\). The Ward identities (4.24)–(4.31) are linear identities in these coefficients. They replace a higher coefficient by lower coefficients multiplied by commutators or coordinate differences. They do not multiply two activity coefficients or introduce an extra Cauchy denominator. For example, (4.22) displays the fourth-order cost as the fourth power of the field-radius/analytic-radius ratio. The passage from (4.34) to the polarization tensor uses only linear kernel summation, its fixed spatial moments, and the stated symmetries. The coefficient defining \(\beta_j\) is a second-order coefficient with a second spatial moment, so it has the bound in the table.

The spatial gains in the last column are precisely the gains of the source's irrelevant remainders. CMP119 (3.49)–(3.67) gives the same accounting after the layer transfer, with gain \(5-\theta\). In particular the marginal \(F^2\) term must be cancelled against the *same* \(\beta_j\) Wilson term before applying the table. Bounding those two terms separately would leave an unsummable marginal expression.

Since \(Q_k\) is below a fixed ceiling less than one, a degree-\(n\) term with coefficient order \(r\le n\), \(2\le r\le5\), is bounded by

\[
 CE_0r_j^{-r}Q_k^n
 \le CE_0\left(\frac{\alpha_{0,k}}{\alpha_{0,j}}\right)^r,
 \qquad 2\le r\le5.
 \tag{E14.36}
\]

One must retain the value of \(r\) in this inequality. Replacing every denominator by \(\alpha_{0,j}^{-5}\) while leaving a quadratic numerator would not prove it. The Wilson remainder is handled with its coefficient order two and its actual field degree; its higher-degree factors only improve (E14.36).

For the Wilson analytic tail, degrees above five are bounded by their convergent fixed-chart majorant, retaining the degree-five factor and its coefficient order two. The argument does not truncate that analytic tail or declare all its terms to have degree at most five.

The AF comparison therefore bounds the complete nearby irrelevant majorant by

\[
 CE_0(1+a)^{b_*}
 \left[\sum_{r=2}^5C_{\rm AF}^{r}(1+a)^{r/2}\right]
 L^{-(5-\theta)a}e^{-\kappa'd_j(X)}.
 \tag{E14.37}
\]

After the four-dimensional old-cell count, the explicit remaining sum is

\[
 \sum_{a\ge0}(1+a)^{b_*+5/2}
             L^{-(1-\theta)a}<\infty.
 \tag{E14.38}
\]

For fixed \(\theta,L,b_*\), this is a numerical constant uniform in the total RG depth. This proves the running-radius *majorant* for all terms in the nearby E decomposition, provided the common native domain, the regularity size \(Q_k\), and the source's exact matching subtraction are retained. It supplies no weighted Hessian smallness by itself.

The role of the independent current in this argument is specific. CMP109 (3.36) defines the nearby pair by the minimizing pullback of the coarse determining field \(B\). The Taylor formula (3.34) has the arbitrary regular field \(A\) and the external background \(U\); the external independent current enters when \(A\) is subsequently replaced by the actual \(\mathcal H_s(U,J,z)\). Section 4 then evaluates its Taylor coefficients at the primitive pair \(U=1,J=0\). CMP116 begins its localization from the already-subtracted local analytic functions of \((U,J,A)\) and performs this actual preparation substitution. Thus the cancellation is an identity in the coarse determining field followed by analytic substitution. It is not an assertion that a holomorphic identity on the physical-current graph determines an arbitrary independently extended function.

#### 5.5 Admitting the whole far insertion before testing the E radius

The coarse average in the far formula need not be identified with the modified nearby \(Q'_j\). An actual unmodified-average estimate is available in the published papers. CMP102 p.285, (44), writes

\[
 Q_j(\eta A)=L^j\eta\,Q_jA+C_j(L^j\eta A),
 \qquad
 |C_j(L^j\eta A)|\le C_2(L^j\eta)^2\|A\|_\infty^2.
 \tag{E14.39}
\]

The left-hand \(Q_j\) is the nonlinear relative average and the \(Q_j\) in its first term is its linearization. These are not the different nearby map \(Q'_j\).

CMP99 p.406, immediately after (3.78), gives a direct uniform estimate for the nonlinear relative averages. On \(\|A\|<\alpha_1/(L^j\eta)\), their logarithms at the intermediate steps satisfy
\(\|B_n\|\le C\alpha_1L^n\xi\), with \(\xi=L^{-j}\) and \(0\le n\le j-1\). The remaining one-block operation has a fixed number of inputs once \(L,d\) are fixed. It is analytic on a fixed small chart and vanishes at zero relative input. Equation (3.79) controls its linearized averaging operator; converting this derivative to the fixed logarithmic coordinates introduces only a fixed chart factor. Thus its derivative is uniformly bounded on that smaller chart. It therefore sends \(\|B_{j-1}\|\le C\alpha_1/L\) to a logarithm of norm at most \(C_L\alpha_1\). Choosing \(\alpha_1=2L^j\eta\|A\|\), below that fixed chart ceiling, proves

\[
 \|Q_j(\eta A)\|_\infty
 \le C_{\rm av}L^j\eta\|A\|_\infty.
 \tag{E14.40}
\]

The case \(j=0\) is the direct relative link input and has the same bound. The constants are uniform in the old index and the number of fine bonds; the last step is a fixed \(L\)-block operation, not a chain of uncontrolled Lipschitz constants. The same argument holds on the source's admitted complex-background domain. The independent current is not an argument of this relative averaging operation.

We now separate two different domains. Choose a fixed absolute small regular domain for the internal averaging and minimizing maps of CMP102 Proposition 9 and CMP116 (1.11)–(1.18). Call its admitted coarse-input radius \(\rho_{\rm map}>0\). This is chosen before, and independently of, the shrinking primitive E-activity radii \(\alpha_{0,j}\). The real regular centers from (E14.26) and sufficiently small native background/current perturbations lie in this fixed domain. The geometric and localized-propagator hypotheses of those primary results are retained.

In CMP109 (3.6) the relative coarse input is formed from \(tA\), with \(A\) the prepared field, and it vanishes at \(A=0\). Equations (179)–(180) of CMP102 define the corresponding relative minimizing map with value zero at zero input. The localized formula (1.17) of CMP116 preserves that zero: all its terms contain the input, and its nonlinear correction is the unique small solution with zero value there. These facts remain true when the source current is independently extended.

Let \(C_H\) be the fixed operator bound, in the four output norms required by CMP109 (3.14), for the first derivative of that relative minimizing map on the smaller absolute map domain. This bound is the integrated kernel estimate of CMP102 (190). Its scale measure cancels the kernel's input-cell volume factor; the remaining exponential has a uniformly bounded row sum under the source geometry. The localized versions obey the same estimate with their fixed preparation loss, as stated after CMP109 (3.17) and quantified by CMP116's propagator bound. Thus, for coarse inputs \(B\) in \(\|B\|<\rho_{\rm map}/2\), integrating the actual derivative on the segment \(vB\), \(0\le v\le1\), gives

\[
 \|\mathcal H_{j,s}(B)\|_{{\rm adm},j}
 \le C_H\|B\|_\infty.
 \tag{E14.41}
\]

When using the current-scale partition to sum localized derivatives, apply the bound at a fixed output point first. For \(\lambda=L^{-a}\le1\), the sum over partition cubes is bounded by
\(C_d\sum_{r\ge0}(1+r)^{d-1}e^{-cMr}\), independently of \(a\). Taking the output supremum afterwards avoids a factor equal to the carrier's volume. The same pointwise argument applies to the source's first-difference, Hölder and second-order output bounds. This is the row-sum interpretation used in \(C_H\).

This segment lies in the fixed map domain before any E-activity condition is imposed. There is consequently no circular use of the desired smaller E-domain admission. Equation (E14.41) also retains the projection term: it uses all the source's required second-order output norms, not a pure-dilation claim for projections defined on different determining geometries.

Combining (E14.6), (E14.40) and (E14.41) for the actual current input yields

\[
 \begin{split}
 \|B_{j,s}(t,z)\|_\infty
 &\le D_{\rm av}L^{-a}g_k\|z\|_\infty,\\
 \|\mathcal H_{j,s}(B_{j,s}(t,z))\|_{{\rm adm},j}
 &\le D_{\rm far}L^{-a}g_k\|z\|_\infty,
 \end{split}
 \qquad 0\le t\le1,
 \tag{E14.42}
\]

where one may take
\(D_{\rm av}=4C_{\rm av}C_\zeta KC_B\) and
\(D_{\rm far}=C_HD_{\rm av}\), enlarged by the fixed localization constants if the source puts them outside \(C_H\). Both inequalities hold jointly with the native external variables and the complex preparation parameters. First impose \(2D_{\rm av}\delta_k\le\rho_{\rm map}/2\); this admits all coarse inputs to the fixed map domain. Then, with \(\alpha_{2,j}=c_2\alpha_{0,j}\), impose

\[
 \ell_k^{q-p_0}
 \ge \frac{24D_{\rm far}A_1C_{\rm AF}}{c_2C_0}.
 \tag{E14.43}
\]

For \(\|z\|<2P_k\), the AF comparison and
\(L^{-a}\sqrt{1+a}\le1\) give

\[
 \|\mathcal H_{j,s}(B_{j,s}(t,z))\|_{{\rm adm},j}
 <\alpha_{2,j}/12
 \quad\hbox{at every old scale and every }0\le t\le1.
 \tag{E14.44}
\]

The spare factor admits the localized insertion-parameter variation as in (E14.11). It is the whole background insertion in the far formula, not merely its infinitesimal localized response, that is now controlled. The independently varied background and current still have to be kept in the common native external domain; their actual real-center and native local reserves were proved in Section 5.2. This calculation resolves the far coarse-input mismatch without replacing \(Q_j\) by \(Q'_j\).

#### 5.6 A common native background/current contour and its summed prefactor

The scale transfer of the independent current is fixed before introducing it as an independent variable. If \(h\) and \(\xi\) are two choices of lattice length unit, the physical current definition \(J_h=D_h^*h^{-2}\pi\operatorname{Im}dU\) gives

\[
 J_\xi=(h/\xi)^3J_h.
 \tag{E14.45}
\]

For the current-scale and old-scale units in CMP109 (3.12), this gives the conservative coefficient bound \(|\tau_j|\le C_JL^{j-k}\), with a fixed one-step unit-convention factor \(C_J\). Either \(h=\eta\) or \(h=L^{-1}\eta\), with \(\xi=L^{-j}\), gives the bound with \(C_J=1\); retaining \(C_J=L^3\) also covers a fixed adjacent-step convention. This uses the physical definition in the substitution being extended and the known relative scale, not a reading of an unclear printed superscript or an assumed exact convention. The subsequent independent replacement in (3.13) changes the variable, not that coefficient. No identity between the independently varied \(J\) and the physical current of the independently varied \(U\) is imposed afterwards.

For clarity, use the native external background coordinate \(b\), the relative regular field in the source local charts, and its source norm. This is the coordinate of the analytic source theorem; it is not an arbitrary reparameterization of the entire retained configuration. The old reconstructed relative field caused by a change \(b\) is bounded by

\[
 \|b_j\|_{{\rm native},j}
 \le C_{\rm ext}L^{-a}\|b\|_{{\rm native},k}.
 \tag{E14.46}
\]

Indeed, the relative average has the actual bound (E14.40), the relative minimizing map has (E14.41), and the relative-gauge compositions have (E14.31). Their fixed constants may be multiplied into \(C_{\rm ext}\). Where the field is merely written in old length units, the bound is its direct scaling; where its determining geometry changes, the proof uses (E14.41) on that actual geometry. This argument does not identify different projections under dilation. The same local gauges and reconstruction domains are used as in the native source extension. The analytic gauge conjugations of the independent current in CMP109 (3.26)–(3.28) have uniformly bounded norm on the smaller fixed chart. Their changes are bounded by a fixed constant times the relative-background change; multiplying the small current center and retaining the scale coefficient gives the same bound, with that fixed constant included in \(C_{\rm ext}\).

Choose \(c_{\rm ext}>0\) so that

\[
 c_{\rm ext}C_{\rm AF}\max\{C_{\rm ext},C_J,1\}
 \le\frac1{128}\min\{c_{\rm loc},c_2,c_3,c_{\rm near}\}.
 \tag{E14.47}
\]

On the common background and independent-current balls

\[
 \|b\|_{{\rm native},k}<c_{\rm ext}\alpha_{0,k},
 \qquad
 \|J-J_{0,k}\|_\infty<c_{\rm ext}\alpha_{0,k},
 \tag{E14.48}
\]

(E14.45)–(E14.47) and the AF comparison put every old native background/current perturbation inside its reserved fractional radius. The actual real centers already lie in the smaller domain by (E14.26)–(E14.27). The local-current and relative-field proof supplies the basic-domain inclusion; the primary smaller-domain theorem supplies reconstruction. The same inequalities apply along the coarse-field Taylor segments used by the nearby analysis. In particular \(Q_k\) in Section 5.4 may be taken to be a fixed small multiple of \(\alpha_{0,k}\), after imposing the already displayed normalized-current cutoff inequalities.

Take one fixed \(q>p_0\), and take the uniform coupling ceiling small enough to meet (E14.24), (E14.24f), (E14.27), (E14.43), the fixed map-domain ceiling in Section 5.5, and the absolute smallness conditions of Section 3. Each inequality has the form already quantified there: either a lower bound on \(\ell_k^{q-p_0}\), or \(Cg_k\ell_k^b\le c_0\). No new choice of \(q\) is made for a higher observable derivative.

The result is the simultaneous product contour

\[
 \begin{split}
 &\|z\|_\infty<2P_k,\qquad
   \|b\|_{{\rm native},k}<c_{\rm ext}\alpha_{0,k},\\
 &\|J-J_{0,k}\|_\infty<c_{\rm ext}\alpha_{0,k},\qquad
   |s(\Delta)|<e^{\kappa_1}.
 \end{split}
 \tag{E14.49}
\]

All internal activity arguments are admitted jointly on this contour, with the insertion-parameter reserves above. Boundary-crossing contributions assigned to B by the actual source localization remain in C-05; this statement applies to the E carriers of the C-01 decomposition. It does not discard those boundary contributions from the complete law.

To display the prefactor, fix \(0<\theta<1\), and put

\[
 \begin{split}
 S_{\rm near}&=\sum_{a\ge0}(1+a)^{b_*+5/2}L^{-(1-\theta)a},\\
 S_{\rm far}&=\sum_{a\ge0}\sqrt{1+a}\,L^{3a}e^{-cML^a},\\
 \mathfrak K_E&=C_{\rm src}E_0(1+S_{\rm near}+S_{\rm far}).
 \end{split}
 \tag{E14.50}
\]

Here \(C_{\rm src}\) is a fixed maximum/product of the displayed preparation, local-comparison and source carrier-resummation constants. The finite factors \(C_{\rm AF}^r c_r^{-r}\), \(2\le r\le5\), are included; the constants are independent of the cutoff depth, torus volume, history, and the order of subsequent differentiation. Let \(\kappa_*>0\) be the decay rate left after the fixed carrier losses in CMP116 Lemma 1. Its geometric localization argument is unchanged: only the old-age scalar majorant has been replaced by (E14.37) and (E14.34). The source localization and the convergent sums give

\[
 |\mathcal E_{k,Y}(z,b,J,s)|
 \le \mathfrak K_E e^{-\kappa_*d_k(Y)}
 \quad\hbox{on (E14.49).}
 \tag{E14.51}
\]

For a real current center \(\|z_0\|\le P_k\), the coordinate radii may therefore be taken as

\[
 r_z=c_GP_k,\quad
 r_b=c_Gc_{\rm ext}\alpha_{0,k}/2,\quad
 r_J=c_Gc_{\rm ext}\alpha_{0,k}/2,\quad
 r_s=(e^{\kappa_1}-1)/2.
 \tag{E14.52}
\]

For \(b\), this is the radius in the stated native norm. For the supremum and first-difference norm, the simultaneous fine-link scalar-coordinate polydisc has radius \(\xi r_b\), as in Section 5.2. If a fixed first-difference Hölder seminorm of exponent \(\beta\) is included, use instead \(\xi^{1+\beta}r_b\): the distance between distinct lattice points is at least \(\xi\), so the first-difference Hölder norm of a scalar-coordinate perturbation is bounded by a fixed constant times its amplitude divided by \(\xi^{1+\beta}\). No second-order or nonlocal projection bound for an arbitrary raw coordinate direction is inferred from its first-difference norm.

For current, native-background, independent-current and preparation multi-indices \(u,v,w,t\), multivariable Cauchy gives

\[
 |\partial_z^u D_b^v\partial_J^w\partial_s^t
       \mathcal E_{k,Y}|
 \le u!w!t!\,e^{|v|}|v|!\,\mathfrak K_E e^{-\kappa_*d_k(Y)}
       r_z^{-|u|}r_b^{-|v|}r_J^{-|w|}r_s^{-|t|}.
 \tag{E14.53}
\]

Native-background derivatives in (E14.53) mean directions of norm at most one in the stated native norm. For \(m=|v|\) such directions, use scalar radii \(r_b/m\); their derivative cost is \(m^mr_b^{-m}\le e^m m!r_b^{-m}\). For raw coordinate derivatives the simultaneous polydisc instead gives \(v!(\xi r_b)^{-|v|}\), or \(v!(\xi^{1+\beta}r_b)^{-|v|}\) when the stated Hölder norm is used. This distinction avoids interpreting a norm ball as an unrestricted product of arbitrary unit directions. The primitive old-age sums are absolutely convergent before differentiation on this common contour, so their Cauchy bounds have no uncounted inverse old-scale radius. This is the quantitative contour and summed-prefactor statement requested by C-02. It supplies neither the C-04 weighted-Hessian smallness nor the C-05 boundary estimates, and it does not perform the further arbitrary-mark coordinate transport assigned to M-04/M-06.

#### The direct native-domain shortcut and its polynomial ambiguity

The product domain printed in CMP119 (3.43) would directly give a current margin

\[
 \rho_k=C_1p_1(g_k)-P_k
 \tag{E14.24a}
\]

if this number were known to be positive on the actual support. This approach legitimately uses the source's completed localization and preparation maps. It need not reconstruct every internal substitution again. The enlarged background domain in the same formula is also a genuine native domain that can be used directly after quantifying its margin at the actual background and independent-current center.

A notation check prevents using this shortcut without another step. The paragraph after CMP119 (3.4), p.265, defines the **unprimed** \(\delta_k\) using \(p_0(g_k)\). The normalized cutoff \(g_0^{-1}\delta_0\) appears explicitly already in (1.18), p.250. The smaller polynomial \(p_1\) introduced later in LFR I belongs instead to the **primed** preparation threshold \(\delta'_j\), with \(p_1<p_0\); it is not the threshold in LFR I (1.9). The \(p_1(g_k)\) printed in CMP119 (3.43) has not been identified with either polynomial by a checked definition in that paper.

In particular, identifying it with the sharper LFR polynomial would give

\[
 \frac{C_1p_1(g_k)}{P_k}
 =\frac{C_1}{A_1}\ell_k^{p_1-p_0}\longrightarrow0,
 \tag{E14.24b}
\]

so no choice of a fixed larger coefficient would repair the reserve. This disproves that proposed identification as a way to justify (E14.24a); it does not disprove the construction. The underlying-map proof in Sections 5.2–5.6 resolves C-02 without using that unidentified polynomial: it directly admits the conservative full support with a strict margin. The printed polynomial ambiguity remains an observation, not a premise of Theorem E14.3.

### 6. The completed contour theorem and its scope

#### Theorem E14.3 — the actual regular E contour

Retain the source-free complete RG representation, its admitted geometry, regular and large-field history decomposition, and consistently normalized trajectory as in J0/C-01. Use the actual E/B assignment of that representation. Fix the source group, one admissible block size, the localization parameters, and one integer \(q>p_0\). Choose \(\alpha_{0,k}=C_0g_k\ell_k^q\), \(\alpha_{1,k}=C_1g_k\ell_k^q\), with the fixed ratio required by the nearby-source inclusion. Impose the common small-coupling ceiling specified in Section 5.6.

Then every actual localized regular E activity has the simultaneous native contour (E14.49), containing the entire real normalized-current support \(\|z\|\le P_k=\delta_k/g_k\), and the uniform carrier bound (E14.51) with the explicit summable prefactor (E14.50). Its current, native-background, independently extended current and preparation derivatives satisfy (E14.53), with radii (E14.52). The constants are uniform in the cutoff depth, torus volume and remaining admissible history. In particular the old-scale sums are controlled before differentiation on a common contour; differentiating does not introduce an uncounted inverse old-scale radius.

**Proof.** The actual real centers have the strict smaller-domain reserve (E14.26)–(E14.27). The local relative-field comparison (E14.28)–(E14.31), the Wilson-current calculation in the supplement, and the primary smaller-basic-domain inclusion give the native local reserve (E14.32), including reconstruction. The complete nonlinear preparation is admitted by the explicit minima (E14.8). The independent additive nearby input has radius (E14.15b), and its running current input is admitted at every old scale by (E14.24f).

For far insertions, the unmodified nonlinear averaging estimate (E14.40) first admits the whole input path to a fixed absolute internal-map domain. The old relative minimizing map vanishes at zero and satisfies the actual four-norm derivative estimate there; integrating it proves (E14.41). Equations (E14.42)–(E14.44) then put the whole old insertion path strictly inside the running E radius. This order of the argument avoids using the desired E-domain conclusion to justify the derivative estimate used to prove it.

The native background/current transfer (E14.45)–(E14.48) admits the external variables on the same contour at every old scale. The near fifth-order tail, all lower-order Ward and matching-coupling remainders, and far terms have respectively the bounds (E14.24g), (E14.37) and (E14.34). The marginal quadratic coefficient is cancelled by its prescribed Wilson subtraction before summation. The explicit age sums (E14.38) and (E14.35), with the source's geometric carrier resummation, give (E14.50)–(E14.51). Normal convergence gives joint holomorphy. Cauchy on the product contour gives (E14.53), with the stated directional-versus-coordinate convention for the background norm. \(\square\)

The complex margin and the old-scale summable derivative prefactor include the independently extended current and preparation factors. The uniform Wilson trajectory and the compatible conditional representation remain hypotheses.

The following obligations remain distinct:

- C-03 concerns the actual R marginal and its additional transfers and denominators.
- C-04 asks for the small weighted derivative/Hessian budget; the finite contour prefactor here is deliberately not called that bound.
- C-05 includes the E-origin expressions which the source actually assigns to B at a multiscale boundary.
- C-06 and M-04/M-06 include further conditional and marked-coordinate estimates beyond the native contour proved here.

No term is omitted from the complete law by these distinctions. There is no inference of the full Schwinger hierarchy or Yang–Mills existence from this one completed statement.

### 7. Primary references

- T. Balaban, *Propagators for Lattice Gauge Theories in a Background Field*, CMP 99 (1985), 389-434, (3.3)-(3.12), (3.69)-(3.81), especially pp.391-392 and 404-406.
- T. Balaban, *The Variational Problem and Background Fields in Renormalization Group Method for Lattice Gauge Theories*, CMP 102 (1985), 277-309, especially Proposition 9 and (172), (179)-(190).
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. I*, CMP 109 (1987), 249-301, especially (1.11)-(1.18), (3.11)-(3.17), and Lemma 4/(3.53). [DOI](https://doi.org/10.1007/BF01215223).
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. II. Cluster Expansions*, CMP 116 (1988), 1-22, especially (1.11)-(1.22) and Lemma 1/(1.33)-(1.36). [DOI](https://doi.org/10.1007/BF01239022).
- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP 119 (1988), 243-285, (2.25)-(2.28), (2.34)-(2.39), (3.43), and the transfer discussion on pp.276-277.

The quantitative contour theorem is proved above at the stated source scope. No primary theorem is used as an unqualified proof of the full four-dimensional observable hierarchy.


### 8. Supplement: quantitative local-current proof

The following calculation uses CMP99, pp. 391–392 and 404–405.

##### 1. Result and scope

This part resolves a local coefficient question in the contour analysis. The nonlinear current remainder in CMP109 (3.11) can be bounded with a constant independent of the fine lattice spacing. Its control does not require an unspecified compactness argument, or the first variational paper.

The proof uses the explicit current, Hessian and covariant-difference formulas in CMP99, pp.391–392 and 404–405. It gives a source-specific bound for the local current extension:

\[
 \|F(U,A)\|_\infty
 \le C_G\left(
 b\|A\|_\infty+
 \|A\|_\infty\|\nabla_U A\|_\infty+
 \|A\|_\infty^3
 \right),
 \qquad
 b=\sup_p\xi^{-2}\|U_p-I\|.
 \tag{LC.1}
\]

All norms are taken on the fixed enlargement of the output bond star needed by the displayed local formulas. The constant depends on the fixed dimension, group and regular-chart bounds, not on \(\xi\), carrier size, torus volume or old-scale index.

Together with the exact discrete Weitzenböck identity, this yields a current-clause insertion radius \(c_G\alpha_0\) on a quantitatively smaller input current domain. It identifies and proves the needed local coefficient bound. It does not by itself prove all reconstructed-field and preparation-domain conditions of C-02/C-03.

##### 2. Coordinates and actual primary formulas

Work in a regular representative on a lattice of spacing \(0<\xi\le1\). Assume that one-link parallel transports and their inverses have norm at most a fixed \(K_0\), and that the plaquette bound \(b\le b_*\) holds. In the source regular complex chart, the real compact-group factor has norm one and the relative complex factor is small; \(K_0\) can therefore be fixed uniformly.

For Lie-algebra fields define the covariant translation and difference

\[
 (T_\mu f)(x)=\operatorname{Ad}_{U_\mu(x)}
 f(x+\xi e_\mu),\qquad
 D_\mu=\xi^{-1}(T_\mu-I),\qquad
 D_\mu^*=\xi^{-1}(T_\mu^{-1}-I).
 \tag{LC.2}
\]

The exterior covariant curl is

\[
 (D_UA)_{\mu\nu}=D_\mu A_\nu-D_\nu A_\mu.
 \tag{LC.3}
\]

These are CMP99 (3.3)–(3.9). The adjoint here is the algebraic transpose for the invariant bilinear form when the fields are complex; it is not an antilinear operation on the holomorphic variables.

Let \(\mathcal A(U)\) be the source Wilson action with its lattice scaling and normalized trace. CMP99 (3.11)–(3.12) identify its left-coordinate gradient and Hessian:

\[
 \mathcal A(e^{i\xi B}U)
 =\mathcal A(U)+\langle B,J(U)\rangle
   +\tfrac12\langle B,\Delta(U)B\rangle+\cdots,
 \qquad
 J(U)=D_U^*\xi^{-2}\pi\operatorname{Im}dU,
 \tag{LC.4}
\]

where \(\pi\) is the fixed Lie-algebra projection. Formula (3.10) gives

\[
 \Delta(U)=D_U^*D_U+\Delta'(U).
 \tag{LC.5}
\]

Its two error terms have coefficients \(\xi^{-2}(\operatorname{Re}U_p-I)\) multiplying unscaled covariant curls, and \(\xi^{-2}\operatorname{Im}U_p\) multiplying products of transported bond fields. This is the actual source Hessian, including the curvature term.

For \(U_t=e^{it\xi A}U\), CMP99 (3.71)–(3.73) give the explicit local operator comparison

\[
 \begin{split}
 \|(D_{U_t}^*D_{U_t}-D_U^*D_U)B\|_\infty
 \le C_G\big(
  |t|a\|\nabla_U B\|_\infty
  +|t|a_1\|B\|_\infty
  +t^2a^2\|B\|_\infty\big),
 \\
 a=\|A\|_\infty,\qquad a_1=\|\nabla_U A\|_\infty.
 \end{split}
 \tag{LC.6}
\]

The formula is obtained by expanding the transport factors \(e^{it\xi\operatorname{ad}A}\). Each first difference supplies its compensating \(\xi^{-1}\); the remainder is bounded by \(C\xi^2a^2\), so the two differences leave \(Ca^2\), not \(Ca^2/\xi\). Equation (LC.6) is also read directly from the source's displayed formula. For a complex initial regular representative the same finite-product proof applies, with a changed fixed \(K_0\)-dependent constant.

##### 3. The three scale-independent estimates

###### 3.1 Curvature along the insertion path

For \(a,a_1,b\) in a fixed bounded small range and \(0\le t\le1\),

\[
 b_t:=\sup_p\xi^{-2}\|(U_t)_p-I\|
 \le C_G(b+a_1+a^2).
 \tag{LC.7}
\]

Here is the cancellation in the matrix product. For a positively oriented \(\mu\nu\) plaquette at \(x\), put \(P=U_{\mu\nu}(x)\). Moving the inserted exponentials to the initial vertex writes the new plaquette as

\[
 \begin{split}
 (U_t)_p={}&
 e^{it\xi A_\mu(x)}
 e^{it\xi T_\mu A_\nu(x)}
 e^{-it\xi\operatorname{Ad}_{P}T_\nu A_\mu(x)}
 e^{-it\xi\operatorname{Ad}_{P}A_\nu(x)}P.
 \end{split}
 \tag{LC.8}
\]

The sum of the four linear exponents is

\[
 \xi(D_\mu A_\nu-D_\nu A_\mu)
 -(\operatorname{Ad}_P-I)
      (T_\nu A_\mu+A_\nu).
 \tag{LC.9}
\]

The first term, after multiplication by \(t\xi\), is bounded by \(C\xi^2a_1\). The second is bounded by \(C\xi^3ba\). The terms at least quadratic in the exponents are bounded by \(C\xi^2a^2\), using the convergent exponential series and the fixed transport bound. Adding \(P-I\) proves (LC.7). There is no division by an uncontrolled first-order plaquette variation.

###### 3.2 Current and Hessian-error estimates

The local formula for \(D_U^*\) gives the crude but sufficient bound

\[
 \xi\,\|J(U_t)\|_\infty\le C_G b_t.
 \tag{LC.10}
\]

Only this bound is needed below; a uniform bound for the physical current itself is not inferred from curvature.

The identity

\[
 \operatorname{Re}P-I
 =\tfrac12(P-I)^2P^{-1}
 \tag{LC.11}
\]

and the complex definition \(\operatorname{Im}P=(P-P^{-1})/(2i)\) imply

\[
 \|\operatorname{Re}P-I\|\le C\xi^4 b_t^2,
 \qquad
 \|\operatorname{Im}P\|\le C\xi^2b_t.
 \tag{LC.12}
\]

Applying the finite-stencil Hessian formula (3.10), or the estimate preceding (3.69), now gives

\[
 \|\Delta'(U_t)B\|_\infty
 \le C_G(b_t+\xi^2b_t^2)\|B\|_\infty
 \le C'_G b_t\|B\|_\infty.
 \tag{LC.13}
\]

The first term in the source quadratic form is written with unscaled curls; their operator norm on a fixed bond star is bounded. Equivalently, if scaled curls are used, the two factors \(\xi^{-1}\) consume two of the four powers in the first estimate in (LC.12). Either convention gives the explicit \(\xi^2b_t^2\) remainder in (LC.13).

###### 3.3 Exact moving-gradient identity

The current gradient cannot be differentiated as though the left-coordinate chart were fixed. Its exact identity is

\[
 \frac{d}{dt}J(U_t)
 =\Delta(U_t)A+\frac{i\xi}{2}[A,J(U_t)].
 \tag{LC.14}
\]

To prove it, fix a test direction \(B\). The mixed coefficient in
\(\mathcal A(e^{is\xi B}e^{it\xi A}U)\) can be computed from

\[
 \frac{1}{i\xi}\log
    (e^{is\xi B}e^{it\xi A})
 =sB+tA+\frac{i\xi}{2}st[B,A]
       +O(s^2t+st^2).
 \tag{LC.15}
\]

Using (LC.4) and trace invariance gives
\(\langle B,J'_0\rangle
=\langle B,\Delta(U)A+\frac{i\xi}{2}[A,J(U)]\rangle\).
The same argument at \(U_t\) proves (LC.14). This is a finite-dimensional exact identity. It does not require a convergent source generating functional.

##### 4. Proof of the local nonlinear-current bound

Integrate (LC.14), insert (LC.5), and subtract the linear term \(D_U^*D_UA\). This gives the exact remainder

\[
 \begin{split}
 F(U,A)=\int_0^1\big[
 &(D_{U_t}^*D_{U_t}-D_U^*D_U)A
 +\Delta'(U_t)A
 +\tfrac{i\xi}{2}[A,J(U_t)]
 \big]\,dt.
 \end{split}
 \tag{LC.16}
\]

The first term is bounded by \(C(aa_1+a^3)\) by (LC.6). The second is bounded by \(Cb_ta\) by (LC.13). The last is bounded by \(Cab_t\) by (LC.10): its explicit factor \(\xi\) cancels the only crude \(\xi^{-1}\) current estimate. Using (LC.7) and integrating proves

\[
 \|F(U,A)\|_\infty
 \le C_G(ba+aa_1+a^3).
 \tag{LC.17}
\]

This proves (LC.1) for the actual Wilson current. Every expression is holomorphic in the regular complex links and \(A\). The proof also displays why a bound obtained by estimating each unpaired fine-lattice difference separately would introduce a spurious inverse-spacing loss.

##### 5. The local part of the independent-current extension

Define the componentwise covariant Laplacian
\(\Delta_{\mathrm{cov}}=\sum_\nu D_\nu^*D_\nu\).
The exact identity on one-forms is

\[
 D_U^*D_U+D_UD_U^*
 =\Delta_{\mathrm{cov}}+\mathcal L_U,
 \qquad
 (\mathcal L_UA)_\mu
 =\sum_\nu[D_\mu,D_\nu^*]A_\nu.
 \tag{LC.18}
\]

Each commutator is a difference of two two-link transports divided by \(\xi^2\). Their quotient is a plaquette transport. Thus

\[
 \|\mathcal L_UA\|_\infty\le C_Gb\,a.
 \tag{LC.19}
\]

This derivation uses only the source covariant differences; no second derivative of the background enters.

Write the source projection as \(R=I-P_0\), and put
\(\mathcal P_U=D_UP_0D_U^*\). Then

\[
 D_U^*D_U+D_URD_U^*
 =\Delta_{\mathrm{cov}}-\mathcal P_U+\mathcal L_U.
 \tag{LC.20}
\]

For the Landau-gauge minimizing field the added term vanishes. After localization, (LC.20) supplies the source's independent extension rather than reimposing that gauge identity on each localized summand.

Let \(\tau J\) denote the retained-current term after its exact source rescaling. Suppose \(|\tau|\le1\) and use a smaller input domain
\[
 \|J\|_\infty\le\alpha_0/4,\quad b\le b_*,
 \quad
 \|A\|_\infty,\|\nabla_UA\|_\infty,
 \|\Delta_{\mathrm{cov}}A\|_\infty,
 \|\mathcal P_UA\|_\infty\le u.
 \tag{LC.21}
\]

The extended current

\[
 J_{\mathrm{ext}}
 =\tau J+
   (\Delta_{\mathrm{cov}}-\mathcal P_U+\mathcal L_U)A
   +F(U,A)
 \tag{LC.22}
\]

therefore satisfies, for \(u\le1\),

\[
 \|J_{\mathrm{ext}}-\tau J\|_\infty
 \le 2u+C_G(bu+u^2+u^3)
 \le K_*u,
 \tag{LC.23}
\]

where \(K_*=2+C_G(b_*+2)\) is fixed. Choosing
\[
 u\le\frac{\alpha_0}{4K_*}
 \tag{LC.24}
\]
gives \(\|J_{\mathrm{ext}}\|_\infty\le\alpha_0/2\), with a fixed further reserve.

This proves a linear current-clause radius. It avoids relying on an ambiguous off-by-one reading of the rescaling factor in CMP109 (3.12). If the larger input current ball is used instead, its exact scale factor must leave a quantitative reserve before (LC.24) is substituted.

##### 6. What remains to obtain the full \(\alpha_2\) admission statement

The proved bound removes the possible hidden inverse-lattice-spacing cost from the **local current formula**. In a smaller regular basic input domain, a choice
\[
 \alpha_2=c_*\min(\alpha_0,\alpha_1)
 \tag{LC.25}
\]
is sufficient for the current clause by (LC.24), and for the direct plaquette clause by (LC.7), after reducing \(c_*\) and reserving enough of the initial \(\alpha_0\) bound.

Two identifications must still be supplied when applying (LC.25):

1. the relative complex-field and first-difference part of the actual source domain must use the same covariant/local regular norm, or be compared to it with uniform constants;
2. the input must lie in a sufficiently smaller basic domain so that the reconstructed-field clause follows from the precise CMP109 p.263 subdomain statement, or the reconstructed-field change must be estimated directly.

These are separate domain conditions. The local remainder (LC.17) does not imply them. In particular, a curvature bound alone does not bound the physical current without the factor \(\xi\) in (LC.10).

If the actual background and current are proved to occupy the smaller basic domain, and the actual prepared insertion satisfies the four norms in (LC.21), the local-current step causes only a fixed multiplicative loss. It then permits the proposed running choice \(\alpha_{0,k},\alpha_{1,k}\asymp g_k\ell_k^q\) with an exponent large enough to contain the actual cutoff and verified fixed preparation losses. This does not complete the statement.

##### 7. Sources

CMP99 gives the formulas on pp.392, 404 and 405 used in this argument. It supplies the exact action gradient and Hessian, the curvature error formula, and the explicit covariant-operator perturbation estimate. The difference convention is the one on p.391.

CMP109 (3.11)–(3.14) specifies the independent-current construction.


---
