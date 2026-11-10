# Native domains and the one-step comparison

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 2. The structure of the step in the source

These facts are used throughout. All are.

- **Effective action.** \(A_k=-g_k^{-2}A(U_k)+\mathbf E_k+\mathbf R_k+\mathbf B_k\), with \(\mathbf E_k=\sum_{j\le k}[\mathbf E^{(j)}(U_k)-\mathbf E^{(j)}(1)-\beta_j(g_{j-1})A(U_k)]\) (CMP119 (2.23)–(2.25)). Births are rooted, (2.26)–(2.27), analytic on \(U^c_j(X,\alpha_{0,j},\alpha_{1,j})\) with running radii (2.28), bounded by \(E_0e^{-\kappa d_j(X)}\), and their rooted densities are exactly Euclidean covariant on the whole lattice, (2.29).
- **R terms.** \(\mathbf R_k=\sum_j[\mathbf R^{(j)}(U_k)-\mathbf R^{(j)}(1)]\), with \(|\mathbf R^{(j)}(X)|\le g_j^{\kappa_0}e^{-\kappa d_j(X)}\) and **no** Wilson subtraction ((2.30)–(2.31); "we obtain a sum of marginal terms", p.260). Covariance only under transformations preserving the \(MR_j\)-grid, (2.32).
- **Mature and recent R.** At step \(k\), the terms with \(j\le k_1\) (grid cubes contained in \(L\)-cubes) form \(\mathbf R'_k\), which "has the same covariance property as the expression determined by \(\mathbf E_k\), and we include it into \(\mathbf E_k\)" (p.271). The recent \(\mathbf R''_k\) is interpolated separately and contributes to \(\mathbf R^{(k+1)}\) and \(\mathbf B^{(k+1)}\) only.
- **The E birth.** The last logarithm in (3.28) contains only the Gaussian, the cutoff \(\chi^{(k)}\), \(\mathbf P^{(k)}(g_k,A)\) and the fluctuation difference \(\mathbf E_k(U_k(\exp i[g_kCA-h\tilde D(g_kCA)]V^{(k)}))-\mathbf E_k(U_{k+1})\), with \(\mathbf E_k\) including \(\mathbf R'_k\). By (3.30)–(3.38), (3.42) it is the sum of the rooted densities \(\mathbf E_0^{(k+1)}(\cdot,z)\). On the whole lattice these are Euclidean covariant, (3.39). The interior terms "coincide with the corresponding terms arising from the expressions defined on the whole lattice" (p.278), and \(\beta_{k+1}(g_k)\) is subtracted from \(\mathbf E^{(k+1)}-\mathbf E^{(k+1)}(1)\) (p.279).
- **The minimiser.** \(U_k(V)\) minimises the Wilson action alone under the averaging constraints (CMP109 (0.21), (1.1); CMP119 (2.12)). It does not depend on \(g_k\) or on \(\mathbf E_k\).
- **Admission.** CMP119 Theorem 1 is conditional on the coupling sequence: "satisfies the inequalities (I.0.33)". CMP109 has no (0.33); its last introductory displays are (0.31) (the two-sided asymptotic-freedom inequality of the unpublished Theorem 2) and (0.32). The interpretation of the citation is (I.0.31). The proofs use the pairwise comparisons (2.6)–(2.9) and sums \(\sum_{j\le n}g_j^{\kappa_0}<g_n^{\kappa_0-6}\) ((2.46)), which need a *lower* bound on the decrement as well as an upper one. The second remark after Theorem 1 (p.262) says the theorem is a statement that RT maps the space with index \(k\) into the space with index \(k+1\).

Consequence: the corresponding representation (P22.3), "input-independent part plus a function of the potentials", is correct at the level of whole-lattice sums. Actual and comparator share \(Y_k\), the Gaussian, the cutoff, the gauge-fixing coefficient and all maps. This part of the note is correct.

## 3. Theorems A–C and Corollary D as implications

- **Lemmas 3.1–3.3.**  (In Lemma 3.2 the line stays in the \(b_*\)-ball because \(\|V'\|\le b_*/2\) and \(|w|\Delta<b_*/2\).)
- **Lemma 3.4.**  (a) is stated with \((\frac54d_B+2B_G)(k-m)\); this is true for \(k>m\) and trivial for \(k=m\). (a) is exactly the first inequality of CMP119 (2.6) with \(\beta'=\frac54d_B+2B_G\): \(g_n\le(1+g_n^2\beta'(n-m))^{1/2}g_m\) is \(Y_m-Y_n\le\beta'(n-m)\). (c) gives the second.
- **Theorem A.** A correct implication from (F1), (L1), (L2), (R), (C1) as stated. The problem is that the stated (L1) and (L2) cannot both hold with the support claimed (Finding 1), and that the conclusion is needed in rooted covariant form (Finding 3).
- **Theorem B.** Correct given Theorem A and Lemma 3.4(e).
- **Theorem C.** The induction is correctly ordered: \(c_{n+1}\) is computed on the provisional chart from data through \(n\), and only then is \(g_{n+1}\) admitted. There is no identified circularity. Two additions are needed: the lower slope must be listed among the source conditions (§8), and (C1) should not be a hypothesis (§6).
- **Corollary D.** The algebra is correct: \(y_i-y_{i+1}=d_B+e_i\); \(v_{m+1}=v_m/(1+x_m)\); \(r_m=-\varepsilon_mv_m^2+v_m^3(d_B+\varepsilon_m)^2/(1+x_m)\); \(|r_m|\le(2C_*+(d_B+1)^2)v_m^3\). In step 2 the inequality needed is \(1/Y\le2/y\), i.e. \(y\le Y+B_G\le2Y\); the note writes the opposite direction "\(y\ge Y-B_G\ge Y/2\)". Both are true for \(Y\ge2B_G\); the conclusion stands.

## 4. Does a marginal perturbation re-enter?

I examined each route by which a marginal mismatch could come back.

**(a) The Wilson coefficient.** In the comparator the coefficient at step \(k+1\) is set to the actual \(Y_{k+1}\). The term \((c_{k+1}-p'_{k+1})A=(\mathcal P\delta H_{k+1})A\) is the Wilson subtraction of the difference family and is carried with it. At step \(k\) the two exponents differ by
\[
\sum_{j\le k}\big[\delta H_j-\delta H_j(1)-(\mathcal P\delta H_j)A\big](U_k)+\big[\mathbf R'_k(U_k)-\mathbf R'_k(1)\big].
\]
This is exact, by linearity of \(\mathcal P\) and (2.25). Each bracket in the sum is irrelevant in the sense of CMP119 (3.67) **if** \(\delta H_j\) is a rooted family with gauge invariance and exactly covariant rooted density, since then (3.49)–(3.66) apply to it verbatim: they are linear identities in the family. That is the content of Finding 3.

**(b) Minimisers and Gaussians.** The minimiser does not depend on the coupling or on the births (§2). The quadratic form of the fluctuation integral comes from \(-Y_kA\) and the gauge-fixing term with the same \(Y_k\) (CMP109 (2.1)). The E terms are never put into the Gaussian. So \(\mathcal G_k\) is identical in the two recursions, and there is no \(Y\)-dependent mismatch of the kind that defeats the self-consistent comparator.

**(c) Other marginal components.** By gauge invariance and exact covariance of the rooted density, the only non-irrelevant parts of a birth are the constant and the isotropic \(F^2\) term ((3.55)–(3.61)). Anisotropic or grid-periodic marginal terms are excluded by (2.29). For mature R terms the weaker covariance (2.32) is sufficient only after maturity, which is why the source waits for it (p.271).

**(d) The mature R terms.** These *are* a marginal perturbation of the actual exponent: they are never Wilson-subtracted, and they stay in \(\mathbf E_k\) at all later steps. Their total second-order coefficient at scale \(k\) is of size \(\sum_{j\le k_1}g_j^{\kappa_0}(\alpha_{0,k}/\alpha_{0,j})^2\) per unit volume; the four scale powers pay the old-cell count and nothing is left over for a geometric sum in the age. The sum over \(j\) converges only through the coupling, using the lower slope of the prefix: \(\sum_jY_j^{-s}\le C_sY_k^{1-s}\) (Lemma 3.4(d)). This is how CMP119 (2.46) and Annex AE (RM.10) proceed. In the recursion this term is forcing \(\Phi_k\) at every step, not a multiplier, and Lemma 3.3 needs only \(\sup\Phi\). The formula gives the corresponding treatment. It should say explicitly that this term is marginal and that (R) depends on the lower slope.

**(e) Domain shrinkage per step.** This is where the note fails as written. See §5.

**(f) The provisional chart.** The birth at \(k+1\) is produced on spaces with radii from \(g_k\), \(\beta\)-enlarged (CMP119 p.262). The crude bound \(|c_{k+1}|\le CE_0r_{k+1}^{-2}=O(Y_k\ell_k^{-2q})\) gives \(g_{k+1}/g_k=1+O(\ell_k^{-2q})\), far inside the enlargement. No estimate on \(c_{k+1}\) is presupposed.

**(g) The bootstrap.** At step \(n\) the induction uses: the prefix numerics through \(n\) (from \(\mathsf S(n)\)); (F1) for births through \(n+1\) on the provisional chart (a single-step consequence of the density at \(n\)); Theorem B through \(n\); the readout once. The comparator's two-loop bound (C2) at step \(n\) uses the couplings through \(n\) only. No future information is used.

## 5. Finding 1: the activity domain

### 5.1 The mismatch

The note defines the activity space \(\mathfrak A_k\) on the contour \(\mathcal K_{k,Y}\) = (E14.49):
\[
\|z\|_\infty<2P_k,\qquad\|b\|_{{\rm native},k}<c_{\rm ext}\alpha_{0,k},\qquad\|J-J_{0,k}\|_\infty<c_{\rm ext}\alpha_{0,k},\qquad|s(\Delta)|<e^{\kappa_1}.
\]
In Annex AD, \(b\) is the relative complex field around an **actual real centre**, i.e. a real background of regularity \(O(\varepsilon_k)\), \(\varepsilon_k=g_kA_0\ell_k^{p_0}\) ((E14.26)–(E14.27)), and \(c_{\rm ext}\) is fixed by (E14.47):
\[
c_{\rm ext}C_{\rm AF}\max\{C_{\rm ext},C_J,1\}\le\tfrac1{128}\min\{c_{\rm loc},c_2,c_3,c_{\rm near}\}.
\]
AD states its scope accordingly: a contour "at every real point of the regular current support" (AD §1). Annex AE (RM.12) is the same contour.

The native space at scale \(k+1\), \(U^c_{k+1}(X,\alpha_{0,k+1},\alpha_{1,k+1})\) (CMP109 (1.11)–(1.16)), contains every real configuration with plaquette bound \(\alpha_{0,k+1}\) in scale-\((k+1)\) units, together with relative complex fields of size \(\alpha_{1,k+1}\). Take such a real configuration with plaquette size close to \(\alpha_{0,k+1}\). Every real centre has curvature \(O(\varepsilon_k)\ll\alpha_{0,k+1}\), so the relative field \(b\) carries essentially all of the curvature, which is \(L^{-2}\alpha_{0,k+1}\) in scale-\(k\) units. A plaquette of \(b\) is a sum of two first differences up to quadratic terms, so \(\sup|\nabla b|\gtrsim\tfrac12L^{-2}\alpha_{0,k+1}\). If the native norm also contains the supremum of \(b\) in a chart on an \(M\)-cube (as in CMP109 (1.12)–(1.13), (3.26)–(3.27)), Stokes' formula on a loop of side \(M\) gives \(\sup|b|\gtrsim\tfrac14ML^{-2}\alpha_{0,k+1}\). Containment of the native space in the contour would therefore require at least
\[
c_{\rm ext}\ \gtrsim\ \tfrac12L^{-2}\qquad\text{and, with the chart supremum,}\qquad c_{\rm ext}\ \gtrsim\ \tfrac14ML^{-2}.
\]
By (E14.47) and the definition of \(c_{\rm loc}\) after (E14.32), \(c_{\rm ext}\le\frac1{128}c_{\rm loc}<1/(128\cdot16B_3)\). The second requirement is then impossible as soon as \(M\ge L^2/32\) (the source takes \(M=L^m\) "much bigger than the previously fixed scales", CMP109 p.257). The first would need \(L^2>1024B_3\), a relation between \(L\) and a constant depending on \(L\) which is neither proved nor claimed in AD. (These lower bounds are heuristic in the non-abelian complex setting, status additional assumption; the point that no containment is established is not.) So the inclusion "native output space \(\subset\) AD contour" is unavailable, and with \(M\)-cube charts it is false.

The cluster expansion is pointwise in the external variables: the output at \((\mathbf U,\mathbf J)\) uses the potentials at the same \((\mathbf U,\mathbf J)\) (CMP116 (2.14), p.15). Hence:

- with \(\mathfrak A_k\) on the AD contour, the output of \(\mathcal C_k\) is defined only on the corresponding reduced set, and (L2) ("values are raw birth families … on the native output domain") cannot hold;
- on the reduced set, the output norm is weaker than the native norm \(\|\cdot\|_{k+1}\) which (L1) requires of the inputs at the next step (AD takes its primitive births on the native space and uses Cauchy radii \(r_j=c_r\alpha_{0,j}\) there). The recursion \(D_{k+1}\le\max(D_k,\theta_kD_k+\Phi_k)\) is then not established in any single norm.

[Reset remainders](../coupling/reset_remainders.md) records exactly this: "Annex AD (E14.46)–(E14.49) maps a reduced output background ball into a larger input ball, which does not supply the same-radius iterative hypothesis." The note does not address it, and its §9 list of scope omits it.

Proposition 4.1 of the note is, on its stated domain, correct *on its contour*: The formula gives the substitutions in (E14.8)/(E14.22)–(E14.24), (E14.24e–f), (E14.33)–(E14.34) and (E14.42)–(E14.44). Its limitation is the contour, not the arithmetic.

### 5.2 What the source states

The source poses the potentials on the full native space, \(\beta\)-enlarged. source:

- CMP109 p.275: the nearby term (3.25) "is analytic on the space \(U^c_{k+1}(\square_0,(1+2\beta)\alpha_0,(1+2\beta)\alpha_1,\alpha_0)\)".
- CMP109 Lemma 4, (3.53), p.280: for \(\mathbf U\) in that space, \(\mathbf A\) satisfying (3.31) and \(|B'|<\alpha_3\), the old pair \((U_j(\square_0,\exp i(\tau B+B')),J_j(\cdot))|_X\) lies in \(U^c_j(X,\alpha_0,\alpha_1)\).
- CMP116 p.7 and Lemma 1, (1.34): each potential is analytic on \(\mathbf U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\times\{|B|<\varepsilon_1g_k^{-1}\}\).
- CMP119 p.276, (3.43): on the running chart the terms "satisfy exactly all the conditions of those lemmas" on \(\tilde U^c_{k+1}(Y,(1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1)\times\{|A|<C_1p_1(g_k)\}\).

The mechanism by which the source avoids any loss of domain is visible on CMP109 pp.277–280. The scale-\((k+1)\) radius \((1+2\beta)\alpha_0\) is carried to scale \(j\le k\) with a factor \((L^{j-1}\eta)^2=L^{-2(k+1-j)}\); the nonlinear corrections are absorbed as multiples of \(\beta\) because \(\alpha_0,\alpha_1\) are small; the result \((1+8\beta)L^{-2}\alpha_0\) is below \(\alpha_0\). The definition of the spaces by condition (iv) (reconstructed fields at every level) makes them self-similar. No constant of the type \(C_{\rm ext}\) has to be beaten by \(L\).

### 5.3 Proposition D\(^*\): the displayed conditions of CMP109 Lemma 4 with running radii

Let \(a=k-j\ge0\), \(a_u:=(1+2\beta)\alpha_{u,k+1}\) (provisional radii, from \(g_k\)), and let \(C_{\rm AF}=(1+\beta_0)^2\) be the comparison constant of CMP119 (2.6)–(2.8), so that \(\alpha_{u,k+1}/\alpha_{u,j}\le C_{\rm AF}\sqrt{a+2}\) on an admitted prefix (AD (E14.24c)). Take \(\alpha_{2,k}=c_2\alpha_{0,k}\), \(\alpha_{3,j}=c_3\alpha_{0,j}\).

*Claim (conditional: every displayed restriction on CMP109 pp.277–280 was located and rewritten; the cited results behind them, [12] (97), [14] (1.43)–(1.54), [15] Proposition 9 and (190), were assumed).* Under the conditions in the right column, the conclusion (3.53) of Lemma 4 holds with target space \(U^c_j(X,\alpha_{0,j},\alpha_{1,j})\), for every \(j\le k\).

| CMP109 location | Restriction at fixed radii | Running form |
|---|---|---|
| (3.37) and the sentence after it | \(B_3^2O(1)M\alpha_0<\tfrac12\alpha_1\) | \(B_3^2O(1)Ma_0L^{-(a+1)}<\tfrac12\alpha_{1,j}\) for all \(a\); sufficient: \(C_1/C_0\ge2\sqrt2(1+2\beta)B_3^2O(1)MC_{\rm AF}/L\) |
| (3.41) | \(O(1)M\alpha_1\le\beta\) | \(O(1)Ma_1\le\beta\): coupling ceiling |
| (3.43) | \((4B_3^2O(1)M)^2\alpha_0\le\beta\) | same with \(a_0\): ceiling |
| (3.45) | \(B_3(B_3O(1)M)^2\alpha_0<\beta\) | same with \(a_0\): ceiling |
| (3.47), (3.52) | \((1+7\beta)L^{-2}\le1\), \((1+8\beta)L^{-2}\le1\) | \((1+7\beta)C_{\rm AF}\sqrt{a+2}\,L^{-2(a+1)}\le\tfrac12\) for all \(a\); sufficient: \(L^2\ge2\sqrt2(1+7\beta)C_{\rm AF}\) |
| (3.49) | \(|Q'|<O(1)\alpha_2L^j\eta\), to be \(<\alpha_3\) | \(O(1)\alpha_{2,k}L^{-a}\le\alpha_{3,j}\); sufficient: \(c_2\le c_3/(O(1)C_{\rm AF})\) (use \(\sqrt{1+a}L^{-a}\le1\)) |
| (3.50) | \(B_3\alpha_3<\tfrac12\alpha_1\) | \(c_3<C_1/(2B_3C_0)\) |
| (3.51) | \(2B_3\alpha_3\le\beta L^{-2}\alpha_0\) | \(2B_3\alpha_{3,j}\le\tfrac14\alpha_{0,j}\), i.e. \(c_3\le1/(8B_3)\) (the role of the inequality is only to keep the sum below the target radius) |
| (3.42) and "the second inequality … is obtained in the same way" | as for (3.47), with \((L^{j-1}\eta)^3\) | better: \(L^{-3(a+1)}\) |
| condition (iv), via (3.38) | "a consequence of condition (iii), with a bit better constant" | unchanged (identity) |
| far carriers, (3.16): \(U^c_{k+1}(Y,(1+\beta)\cdot)\subset U^c_j(X,\tfrac12\alpha_0,\tfrac12\alpha_1,\alpha_0)\) (CMP116 p.9) | \((1+\beta)L^{-1}\le\tfrac12\) | \((1+\beta)C_{\rm AF}\sqrt{a+2}L^{-(a+1)}\le\tfrac12\); sufficient: \(L\ge2\sqrt2(1+\beta)C_{\rm AF}\) |
| insertion, CMP116 (1.21)–(1.22) | \(4B_0C_Be^{16\kappa_1}\varepsilon_1\le\tfrac14\alpha_2\) (\(C_B\): the constant printed as \(C_1\) in CMP116 (1.20); not the radius constant of (2.28)) | \(\ell_k^{q-p_0}\ge32B_0C_Be^{16\kappa_1}A_1/(c_2C_0)\) on \(\|B\|\le2P_k\) |

Every condition is of one of four kinds: a fixed ratio \(C_1/C_0\), \(c_2\), \(c_3\); a mild lower bound on \(L\) (with \(\beta=\frac14\) and \(\beta_0\) small, \(L\ge4\) suffices); a coupling ceiling; a lower bound on \(\ell_k^{q-p_0}\). The age enters only through \(C_{\rm AF}\sqrt{a+2}\,L^{-(a+1)}\) or better. So the running substitution is absorbed with a large margin: the exponential scale gain dominates the polynomial ratio of radii. This is evidence that (D\(^*\)) is true. It is not a proof: the proofs of CMP109 §§4–5 (Ward identities, vacuum polarisation) and the complex-\(s\) localisation of CMP116 §1 also take place on these spaces and were not rerun. For those, the degree-preserving construction of AD §5.4, (E14.36)–(E14.38), is radius-homogeneous and can be reused once the inclusion is available.

### 5.4 The gain is in the source

With the potentials on the source domain, the contraction gain needs no Schwarz lemma and no new contour. Every term of the E potential is a first derivative in \(t_\square\) at \(t_\square=0\), written as a Cauchy integral over a circle whose radius is fixed by
\[
\frac1{|t_\square|}=8B_0C_Be^{16\kappa_1}\alpha_2^{-1}g_k|B|
\tag{CMP116 (1.22)}
\]
and the resulting bound (1.24) is linear in \(\alpha_2^{-1}g_k|B|\) and in \(E_0\). The source remarks: "Another possibility is to use the expression \(g_k|B|\) instead of \(\varepsilon_1\). It gives a better bound" (p.8). The far terms (1.30) carry the same factor \(\alpha_2^{-1}\varepsilon_1\). On the running chart \(\alpha_{2,k}=c_2C_0g_k\ell_k^q\) and \(|B|\le2P_k\), so
\[
\rho_k:=\sup_{\|B\|\le2P_k}\frac{g_k\|B\|}{\alpha_{2,k}}=\frac{2A_1}{c_2C_0}\,\ell_k^{-(q-p_0)}.
\]
This is the square of the corresponding gain. CMP109 p.280 states the purpose of this factor: the constant in (3.54) "is much bigger than \(E_0\) … Eventually we have to recover the constant \(E_0\) … the mechanism for it is provided by the differentiation with respect to \(t_\square\) … This differentiation yields a factor \(O(1)\alpha_2^{-1}\varepsilon_1\)". So \(\theta_k\le\frac12\) is the Lipschitz form of the source's own closing inequality \(O(1)C_3\varepsilon_1\le\frac12E_0\) (CMP116 p.21), with \(\varepsilon_1\alpha_2^{-1}\) replaced by \(\rho_k\). On the running chart the source needs \(q>p_0\) for this; CMP119 (2.28) states only \(q_0,q_1>1\). (The remark of CMP119 p.278 that "multiplication by \(g_k\) yields small bounds" is accurate for the Wilson part; for the E part the smallness is \(\rho_k\), not a power of \(g_k\).)

A possible reading of the printed domain (3.43) supports this. If \(p_1(g)=(\log g^{-2})^{q_1}\), by analogy with (2.4) and (2.28), then \(\{|A|<C_1p_1(g_k)\}\) is \(\{g_k|A|<\alpha_{1,k}\}\): the fluctuation ball reaches the analytic radius, which is the largest admissible trial radius in CMP116 (1.21). The ratio to the real support is \(C_1\ell_k^{q_1-p_0}/A_1\). This reading is additional assumption; Annex AD (after (E14.24a)) considered a different identification and rejected it.

### 5.5 Alternative domain condition

One could try to close the recursion on reduced domains (real centres plus complex balls), redoing AD with inputs given only there. Writing the one-step change of units exactly (\(\|b\|_{{\rm native},j}=L\|b\|_{{\rm native},j-1}\) for the field, \(L^2\) for first differences), the output ball at scale \(j\) has radius \(Lc_{\rm ext}\alpha_{0,j-1}\) in scale-\(j\) units, and step \(k\) needs births of age \(a\ge1\) on balls of radius \((c_r+C_{\rm ext}C_{\rm AF}\sqrt{1+a}L^{-a}c_{\rm ext})\alpha_{0,j}\). Closure needs roughly \(C_{\rm ext}C_{\rm AF}\sqrt2\le L^2\), a numerical relation between \(L\) and constants that depend on \(L\). If it fails the admissible radius shrinks geometrically with depth. The source's spaces avoid this. Therefore regard §5.2–5.3 as the right repair.

## 6. Finding 2: the comparator and (C1)

The comparator is a recursion for **whole-lattice sums**: the step-\(k\) integral depends on the earlier births only through \(\sum_X F_j(X,\cdot)\). Localised representatives are tools for estimates and are not unique. The note needs the comparator birth in two roles:

- in Theorem A, localised by the same map as the actual birth, on native running spaces, so that the difference is small in the native norm;
- in (C2), with fixed-chart bounds (constant radii), so that the readout costs \(O(1)\) and the evenness argument of the finite-cutoff construction §2 gives \(O(1/Y_k)\).

(C1) obtains the first from the second "by restricting their fixed-chart bound to \(\mathcal U_j\)". That identifies the localised pieces of two different constructions (CMP116 (2.13) on fixed charts; the running-chart map of the note). Only their sums agree.

**Repair.** Drop (C1). Define the difference families \(\delta H_j\) inductively (by Proposition L2.2) and *define* \(H'_j:=\mathbf E^{(j)}-\delta H_j\). Then:

- \(H'_j\) is a rooted covariant family with \(\|H'_j\|_j\le E_0+D_j\). Under the induction hypothesis \(D_k\le1\) this is \(E_0+1\), the comparator potentials are in the ball, the next comparator birth is defined, and Theorem A gives \(D_{k+1}\le\max(D_k,2\Phi_k)\le1\). So both the native bound and the well-definedness of the comparator follow from (F1) and the bootstrap; they are conclusions, not hypotheses.
- The whole-lattice sum of \(H'_{k+1}\) is \(\mathcal G_k\) plus the logarithm of the fluctuation integral with the comparator potentials (Proposition L2.2, item 3, and CMP119 (3.28), (3.38)). By induction it is the pure-E step, with Wilson coefficient \(Y_k\) and the cutoff of CMP119, applied to the comparator sums of the earlier steps. This is the object to which the fixed-chart induction (the constant-flux calculation §3) and the finite-cutoff construction §2 apply. Equality of the two descriptions is equality of one real integral on the common real domain near the flat field.

So the fixed-chart content is entirely in (C2\(^*\)) (§9).

**Driven comparator.** Single-step estimates use the prescribed input coefficient $Y_k$ and its cutoff, the uniform fixed-chart bounds and the flat-law moments. The comparator need not satisfy its own recursion for the next coefficient. Uniformity of those inputs, including their field derivatives, is required.

## 7. Finding 3: rooted covariance

See the companion note §4.1 for why the difference family must be rooted and covariant. In the corresponding setup this would be automatic *if* (L2) were proved for the CMP119 rooted construction (3.37)–(3.47), because actual and comparator births would then be images of the same covariant map. But that construction is only described in the source (p.277–278), so its holomorphy cannot be verified line by line.

Proposition L2.2 removes the need. The difference is built as
\[
\delta H_{k+1}(X,z)=\int_0^1ds\ \partial_\lambda\mathfrak E(X)\big[v'+s(v^{\rm act}-v')+\lambda w_{\cdot,z}\big]\Big|_{\lambda=0},
\]
where \(\mathfrak E\) is the CMP116 output map of Lemma L2 and \(w_{\cdot,z}\) are the rooted potentials of the differences. Its rooted density is \(\int_0^1ds\langle\sum_Yw_{Y,z}\rangle_{v_s}\), which is covariant when the rooted potentials are. This requires (L1\(^*\)) and (R\(^*\)) in rooted form. That is natural: the whole analysis of CMP119 (3.48)–(3.67) is at a fixed root \(z\) (Theorem 2 "is an immediate consequence of the inequality with the set \(\Lambda^0_j\cap\Omega\) replaced by one point", p.263).

## 9. The repaired statement

### 9.1 Objects

- **Rooted birth family at scale \(j\).** \(F=(F(X,z))\), \(X\in\mathbf D_j\), \(z\in X\) a site of \(T^{(j)}\): analytic on \(U^c_j(X,\alpha_{0,j},\alpha_{1,j})\), local in \(X\), gauge invariant, with \(F(U,z)=\sum_{X\ni z}F(X,U,z)\) exactly covariant on the whole lattice ((2.26)–(2.29)). Norm \(\|F\|_j=\sup_{X,z}\sup|F(X,\cdot,z)|e^{\kappa d_j(X)}\). \(\mathcal PF\) is the Wilson coefficient of \(\sum_zF(\cdot,z)\) (CMP109 (1.20)–(1.22); CMP119 (3.61)–(3.64)).
- **Potential space \(\mathcal V_k\)**, rooted potentials, \(\|\cdot\|\), \(|||\cdot|||\): companion note §1, §4.2, on the source domain with provisional running radii and current radius \(2P_k\).
- **Output map \(\mathfrak E_k\)**, constants \(a_*\), \(\Lambda\): Lemma L2.

### 9.2 Hypotheses

- **(F1)** \(\|\mathbf E^{(j)}\|_j\le E_0\) and \(|\mathbf R^{(j)}(X)|\le g_j^{\kappa_0}e^{-\kappa d_j(X)}\) on the native spaces, through every admitted step (CMP119 Theorem 1; source input, single-step by the remark on p.262).
- **(F2)** \(c_{k+1}=\mathcal P\mathbf E^{(k+1)}\), and \(\sum_z\mathbf E^{(k+1)}(\cdot,z)\) equals the input-independent part plus the logarithm of the fluctuation integral (CMP119 (3.28), (3.38), (3.42), pp.278–279; source input; provisional-chart replay at construction level).
- **(D\(^*\))** Map-domain inclusion on the full native space with running radii: the conclusion of CMP109 Lemma 4 and of (I.3.16) in the form of §5.3, for all \(j\le k\), on an admitted prefix. (Displayed conditions verified, §5.3; assumed.)
- **(L1\(^*\))** For every tuple \((F_j)_{j\le k}\) of rooted birth families there are rooted covariant gauge-invariant potentials \(\mathcal V^E_k(F)\in\mathcal V_k\), linear in \(F\), whose sum over \(Y\) and \(z\) is the fluctuation difference of \(\sum_j[F_j-F_j(1)-(\mathcal PF_j)A]\), with
\[
\|\mathcal V^E_k(F)\|\le C_V\rho_k\sup_{j\le k}\|F_j\|_j,\qquad|||\mathcal V^E_k(F)|||\le C_V\rho_k\sup_{j\le k}\|F_j\|_j,\qquad\rho_k=\frac{2A_1}{c_2C_0}\ell_k^{-(q-p_0)}.
\]
Support: CMP109 §§3–5 and CMP116 §1 are linear in the family (bounds linear in \(E_0\); Ward identities linear; own-projection subtraction linear), with the factor (1.22); the age sums are AD (E14.24g–h), (E14.34)–(E14.38). Hypotheses: source input for the fixed-chart statement for the actual births (CMP116 Lemma 1); source assertion for the running chart (CMP119 p.276); the linear, rooted, running-radius form is not written out anywhere.
- **(R\(^*\))** The mature R terms have rooted covariant potentials \(\mathcal V^R_k\in\mathcal V_k\) with \(\|\mathcal V^R_k\|,|||\mathcal V^R_k|||\le C_Rg_k^{\kappa_0-11}\). Support: CMP119 p.276 ("treated in exactly the same way as \(\mathbf E_k\)", without the coupling counterterm), p.283, and the estimates of Annex AE (RM.5)–(RM.10), which are proved on the reduced contour only; the lower slope is used.
- **Lemma L2** (companion note; conditional).
- **(P)** \(|\mathcal PF|\le C_Pr_{k+1}^{-2}\|F\|_{k+1}\) on the provisional chart (AD §5.4 construction; source).
- **(C2\(^*\))** Let \(\mathsf H'_j\), \(j\le k\), be the whole-lattice sums of the comparator, i.e. of the pure-E recursion with the cutoff of CMP119 driven by \(Y_0,\dots,Y_k\). Then \(|\mathcal P\mathsf H'_{k+1}-d_k^G|\le C_p/Y_k\). (Fixed-chart induction plus the finite-cutoff construction §2; construction level.)
- **(G)** as in the note. **(N\(^*\))** \(\beta'\ge\frac54d_B+2B_G\), together with the lower-slope sums and the suffix device of §8.

### 9.3 Theorem A′ (one step)

Let step \(k\) be admitted, let \(\delta H_j\), \(j\le k\), be rooted birth families with \(D_k=\sup_{j\le k}\|\delta H_j\|_j\le1\), and put
\[
v^{\rm act}=v_P+\mathcal V^E_k((\mathbf E^{(j)})_j)+\mathcal V^R_k,\qquad w=\mathcal V^E_k((\delta H_j)_j)+\mathcal V^R_k,\qquad v'=v^{\rm act}-w,
\]
where \(v_P\) is the non-quadratic Wilson potential. Assume \(\|v^{\rm act}\|\le a_*/4\) and \(\omega_k:=C_V\rho_kD_k+C_Rg_k^{\kappa_0-11}\le a_*/4\) (both hold below a ceiling, by (F1), (L1\(^*\)), (R\(^*\))). Then the family \(\delta H_{k+1}\) of Proposition L2.2 is a rooted birth family at scale \(k+1\) on the provisional (hence the actual) chart, with
\[
\|\delta H_{k+1}\|_{k+1}\le\theta_kD_k+\Phi_k,\qquad\theta_k=2\Lambda C_V\rho_k,\qquad\Phi_k=2\Lambda C_Rg_k^{\kappa_0-11},
\]
and \(\sum_z[\mathbf E^{(k+1)}-\delta H_{k+1}](\cdot,z)\) is the pure-E step applied to the sums of \(\mathbf E^{(j)}-\delta H_j\), \(j\le k\), at Wilson coefficient \(Y_k\).

*Proof.* Proposition L2.2 with \(v^{(1)}=v^{\rm act}\), \(v^{(0)}=v'\): \(\|v^{(1)}-v^{(0)}\|=\|w\|\le\omega_k\), \(|||w|||\le\omega_k\) by (L1\(^*\)) applied to \((\delta H_j)_j\) and by (R\(^*\)). Items 1–2 give the family and the bound; item 4 gives covariance. For the last statement: by linearity in (L1\(^*\)), \(v'=v_P+\mathcal V^E_k((\mathbf E^{(j)}-\delta H_j)_j)\), so \(\sum_Yv'_Y\) is the Wilson remainder plus the fluctuation difference of the subtracted comparator sums, with no R term; item 3 and (F2) give the claim. \(\square\)

### 9.4 Theorems B′, C′ and Corollary D′

Define \(\delta H_0=0\) and \(\delta H_{k+1}\) by Theorem A′. With \(\theta_k\le\frac12\) (i.e. \(\ell_k^{q-p_0}\ge8\Lambda C_VA_1/(c_2C_0)\)), Lemma 3.3 and Lemma 3.4(e) give, by induction (the hypothesis \(D_k\le1\) is reproduced because \(2\max\Phi\le1\) below a ceiling):
\[
\sup_{j\le n+1}\|\delta H_j\|_j\le2\max_{k\le n}\Phi_k\le C\,g_n^{\kappa_0-11}.
\]
Then \(c_{n+1}=\mathcal P\mathsf H'_{n+1}+\mathcal P\delta H_{n+1}\), and with (C2\(^*\)), (P) and \(\kappa_0\ge16\): \(|c_{n+1}-d_n^G|\le(C_p+1)/Y_n\). The admission induction and Corollary D are as in the note, with (N\(^*\)). These are conditional, conditional on §9.2.

Uniformity: all constants depend on the fixed source parameters, \(q\), \(\kappa_0\) and the constants of §9.2. They do not depend on the depth, the torus, the number, ages or grids of resets, or the history, *provided* the constants in (D\(^*\)), (L1\(^*\)), (R\(^*\)) are uniform in age. For (L1\(^*\)) and (R\(^*\)) that is the content of the age sums (E14.24h), (E14.35), (E14.38), (RM.10), which are radius-homogeneous.
