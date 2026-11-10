# Domains and localization of boundary responses

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

## 1. The statement the summation theorems need

### 1.1 The printed forms

Notation is that of [Hidden components] §4.1: grades \(g\); graded metric \(d_g=d^{(1)}\); capped metric \(d^{(b)}\) with local unit \(M\max(h_{g(x)},h_b)\); \(d_g\ge d^{(b)}\ge|\cdot|_2/M\) (C.2). Sites \(x_i\) have grade \(K\) and density \(n_I\).

| Source | Hypothesis | Domain | Distance to |
|---|---|---|---|
| [Hidden components] (C.5) | \(\lvert\partial_iF_\rho\rvert\le\frac{w_\rho}Pe^{-\nu d_g(x_i,\cup E_\rho)}\) | \(D_P\) | exterior \(E_\rho\) (\(=X_\rho\) for ordinary records) |
| [Boundary estimate b] (Loc′) | same, with \(d_g(x_i,\cup X_\rho)\) | \(D_P\) | full carrier |
| [Boundary estimate c] (Loc′\(_b\)) | \(\sup_{D_P\times\Omega_v}\lvert\partial_iV_e\rvert\le\frac{w_e}Pe^{-\nu d^{(b)}(x_i,\cup X_e)}\) | \(D_P\times\Omega_v\) | full carrier, capped at \(b\) |
| [Boundary estimate d] R6 (Loc′) | \(\sup_{D_P\times\Omega_v}\lvert\partial_iV_e\rvert\le\frac{w_e}Pe^{-\nu d_g(x_i,X_e)}\), records of birth \(j_e\ge b_v\) | \(D_P\times\Omega_v\) | full carrier |

Since \(d(x,\cup E)\ge d(x,\cup X)\) and \(d_g\ge d^{(b)}\), we have (C.5) ⇒ (Loc′) ⇒ (Loc′\(_b\)). The weakest form is therefore the capped one.

### 1.2 Definition (Loc★)

Let \(J_i\subset\mathbb R\) (or the real Lie-algebra ball, coordinatewise) be the real support of the current coordinate \(z_i\), i.e. \(\lvert z_i\rvert\le P_k\). For \(r>0\) put
\[
\mathcal S_r=\{z\in\mathbb C^I:\ \operatorname{dist}(z_i,J_i)<r\ \ \forall i\}\supseteq z_0+D_r\quad\text{for every real }z_0\in\prod_iJ_i.
\]
A record \(\rho\) has a birth \(b\), a paid exterior \(F_\rho\neq\emptyset\) of \(\mathcal G_b\)-cubes, declared holes \(H_\rho\), carrier \(X_\rho=F_\rho\cup\bigcup H_\rho\), and an anchor as in [Boundary estimate b] §2.1. It also has a family of admissible old data \(\eta\in\mathfrak E_\rho\): frozen variables (old fluctuations, raw large-field links, selectors, internal variables of non-eligible components) and integrated kernel variables \(\omega_v\).

> **(Loc★)** One \(r>0\), \(\nu>0\), \(\kappa_*\) serve for all records. Each \(F_\rho(\cdot;\eta)\) is holomorphic on \(\mathcal S_r\) for each \(\eta\), bounded and measurable in \(\eta\), and for all \(i\in I\), \(z\in\mathcal S_r\):
> \[
> \sup_{\eta\in\mathfrak E_\rho}\lvert\partial_iF_\rho(z;\eta)\rvert\le\frac{w_\rho}{r}\,e^{-\nu\,d^{(b)}(x_i,\cup X_\rho)},\qquad w_\rho\le W_b\,e^{-\kappa_*\delta_b(F_\rho)}.
> \]
> For kernels: \(\sup_\omega\lvert\partial_i\sigma_v\rvert\le\frac{s_*}re^{-\nu d^{(b_v)}(x_i,\cup Q_v)}\).
> **Zero-range form.** Each \(F_\rho\) depends on \(z\) only through the coordinates \(z_i\) with \(x_i\in\cup X_\rho\), and \(\sup\lvert\partial_iF_\rho\rvert\le w_\rho/r\). This implies (Loc★) for every \(\nu\).

### 1.3 Proposition 1

Replace (Loc)/(Loc′)/(Loc′\(_b\))/(Resp) by (Loc★), and replace (Col) by its capped form (Col\(_b\)): \(d^{(b)}(x_i,\cup Q)\ge\theta D_Q\) for holes of birth \(b\). Lemma NE.3 of [Boundary estimate d] supplies this, and in every later grid \(j\) as well. Then the conclusions of [Hidden components] Theorems C and E, [Boundary estimate b] Theorems C′ and E′, [Boundary estimate c] Prop. R3 and Cor. R5, and [Boundary estimate d] Theorems NE and R6 hold at every real point \(z_0\) of the support, on \(z_0+D_{r/2}\), with \(P\) replaced by \(r\).

*Proof.* Each theorem is a statement about one polydisc. Apply it to \(z_0+D_r\subset\mathcal S_r\). The recentring of [Boundary estimate c] R1 is then at \(z_0\), and (Real) is required at \(z_0\). It remains to check that no proof uses \(d_g\) except through properties that \(d^{(b)}\) shares. Consider each proof line by line.

- **Theorem C.** Step 1 uses only the number \(e^{-\nu\max_sd_s}\). Steps 2–3 use \(\operatorname{dist}_\infty(x,\cup E)\le M\,d(x,\cup E)\), which is (C.2) and holds for \(d^{(b)}\). Step 4 uses Lemma C2, whose proof shows \(d^{(b)}(x,a)\le d^{(b)}(x,p)+\delta_b(E)+2\sqrt d\) for every \(p\in\cup E\). It invokes \(d^{(b)}\le d_g\) only in its last sentence, so it holds with \(d^{(b)}(x,\cup E)\). Step 5 uses only \(d^{(b)}(x,a_q)\).
- **Theorem C′.** In Lemma C3 put \(\Delta:=d^{(b)}(x,\cup X)\). Case \(p\in\cup F\) is as above. Case \(p\in\cup Q\) uses (Col\(_b\)) and the fact that a Euclidean segment of length \(\ell\) has capped length \(\le\ell/s_b\), because the capped unit is \(\ge s_b\). Steps 1–5 are unchanged.
- **NE** reduces to Theorem C. **R3** is already capped.
- **R6.** Put \(d_e(i):=d^{(j_e)}(x_i,\cup X_e)\). Then Step 1 is literally "\(d^{(j)}(x_i,\cup Q)\le d^{(j)}(x_i,X_e)+\delta_e+2\sqrt d\)". (2.1) follows with (Col\(_j\)). Step 2 uses only \(d^{(j)}\). The \(\sigma_v\) term is treated with \(d^{(b_v)}\). Step 3 is C′ in capped form, as in the previous item. Step 4b uses (2.1).

The constants are unchanged, with \(P\to r\). \(\square\)

### 1.4 Remarks

(i) **[Hidden components] (C.5) is the wrong form under (W).** A record depends on the fields of its holes, so its derivative at a site near a hole decays only to \(\cup X\), not to \(\cup E\). (C.5) agrees with (Loc′) only under the halo reading ([Hidden components] B1(3)), which [Boundary estimate c] §1.2 refuted.

(ii) **The cap at the record's own birth is sharp.** Let all records of birth \(b\) be one-cube carriers at every \(\mathcal G_b\)-cube of a grade-\(\le b\) island, at a fixed number of layers from a site. Suppose they saturate a bound capped at a coarser scale \(c>b\). Then the root sum at that site contains \(L^{d(c-b)}\) anchors per \(\mathcal G_c\)-cube at equal capped distance. The layers \(b+1,\dots,c\), whose crossing pays this multiplicity in Lemma C1, are not counted, so the sum grows like \(L^{d(c-b)}\). This is [Hidden components] §5.4's obstruction one level up.

(iii) **The common contour.** The theorems need one Cauchy radius \(r\) on the whole stadium. They do not need a polydisc centred at \(0\) of radius \(\ge2P_k\). The Hessian budget is \(\mathfrak S/r^2\). HC.18 then needs \(\mathfrak S/r^2\to0\). With \(W_b=O(1)\) it is enough that \(r\to\infty\) along the trajectory, for instance \(r\ge cP_k\). [Boundary estimate d] §4.2 states C-05★ on \(D_{P/2}\) with \(P=c_PP_k\). For the real support to lie inside, \(c_P\ge2\) is implicit. The stadium form removes that bookkeeping.

(iv) **Uniformity in \(\eta\)** is part of (Loc★). Theorem NE needs it pointwise in the frozen data. R1 and R6 need the supremum over \(\Omega_v\).

### 1.5 Proposition Z (zero-range root sum)

Let \(\{F_Y\}\) be records in zero-range form with current supports \(S_Y\subset I\), holomorphic on \(\mathcal S_r\), with \(\sup_{\mathcal S_r\times\mathfrak E}\lvert F_Y\rvert\le w_Y\). Put \(\operatorname{diam}_Y=\operatorname{diam}_\infty\{x_i:i\in S_Y\}\). Then for real \(z_0\), \(z\in z_0+D_{r/2}\) and \(m\ge1\):
\[
\sum_Y\sum_{i_2,\dots,i_m}e^{\chi\max_s\lvert x_{i_1}-x_{i_s}\rvert_\infty}\lvert\partial_{i_1}\cdots\partial_{i_m}F_Y(z)\rvert\le\frac{m!\,2^m}{r^m}\sum_{Y:\,i_1\in S_Y}w_Y\,e^{\chi\operatorname{diam}_Y}\lvert S_Y\rvert^{m-1}.
\]
*Proof.* The derivative vanishes unless every \(i_s\in S_Y\). The polydisc of radius \(r/2\) about \(z\) lies in \(z_0+D_r\subset\mathcal S_r\). Cauchy gives \(\lvert\partial^\alpha F_Y\rvert\le\alpha!(2/r)^{\lvert\alpha\rvert}w_Y\le m!(2/r)^mw_Y\). There are at most \(\lvert S_Y\rvert^{m-1}\) tuples. \(\square\)

**Consequence for holes.** Current sites never lie in a hole. Holes lie in large-field regions, and sites lie in \(\Lambda_{k+1}\). So \(S_Y\) is contained in the paid exterior \(F_Y\), and \(\operatorname{diam}_Y\le M(\delta(F_Y)+2)\) by [Hidden components] Lemma A3. **No collar is needed.** The hidden diameter of a hole never enters, because a zero-range record cannot couple two sites across a hole without its paid exterior spanning them. The only remaining input is the rooted norm \(\mathfrak N=\sup_{i}\sum_{Y\ni x_i}w_Ye^{(\chi M+1)(\delta(F_Y)+2)}\), with \(\lvert S_Y\rvert\le n_I(\operatorname{diam}_Y+1)^d\) absorbed. This is a counting statement over multiscale carriers rooted at a **current** site: a single-birth case of (M2) (§3.4).

## 2. Two lemmas

**Lemma 2 (native directional disc).** Let \((E,\lVert\cdot\rVert)\) be a complex normed space, \(\Omega\subset E\) open, and \(b:\Omega\to\mathbb C\) holomorphic with \(\lvert b\rvert\le K\). Let \(\Phi:\mathcal S\to E\) be holomorphic with \(\Phi(z)+B_\rho\subset\Omega\) for all \(z\in\mathcal S\). Then
\[
\lvert\partial_i(b\circ\Phi)(z)\rvert\le K\,\lVert\partial_i\Phi(z)\rVert/\rho.
\]
If \(b\) depends only on the restriction to \(X\) and the hypothesis holds for the cylinder of the seminorm \(\lVert\cdot\rVert_X\), the same bound holds with \(\lVert\partial_i\Phi\rVert_X\).

*Proof.* \(\partial_i(b\circ\Phi)=Db(\Phi)[\partial_i\Phi]\). Let \(u=\Phi(z)\) and \(v\ne0\). The function \(t\mapsto b(u+t\rho v/\lVert v\rVert)\) is holomorphic and bounded by \(K\) on \(\lvert t\rvert<1\), so \(\lvert Db(u)[v]\rvert\le K\lVert v\rVert/\rho\). \(\square\)

This is [Hidden components] Rem. 4.4(4) and [U17] AQ (NP.23)–(NP.24).

**Lemma 3 (localization ⇒ tangent decay).** Let \(\mathcal C\) be a set of cells with a symmetric adjacency in which each cell has at most \(N\) neighbours. Let \(D\) be the graph distance, and let \(c(x)\) be the cell of a point \(x\). Suppose
\[
\Phi_x(z)=\sum_{Y\ni c(x)}\varphi_{x,Y}(z)
\]
over finite connected cell sets, normally convergent on \(\mathcal S_R\). Suppose each \(\varphi_{x,Y}\) is holomorphic, depends only on the \(z_i\) with \(c(x_i)\in Y\), and satisfies \(\lVert\varphi_{x,Y}\rVert\le Ae^{-a\lvert Y\rvert}\), where \(a_1:=a-2\log N>0\). Then on \(\mathcal S_{R/2}\):
\[
\lVert\partial_i\Phi_x(z)\rVert\le\frac{2A}{RN^2(1-e^{-a_1})}\,e^{-a_1(D(c(x),c(x_i))+1)}.
\]
If in addition \(d^{(b)}(x,y)\le d_g(x,y)\le c_{\mathcal C}(D(c(x),c(y))+1)\), the decay is \(e^{-(a_1/c_{\mathcal C})d^{(b)}(x,x_i)}\).

*Proof.* Only sets \(Y\) containing both \(c(x)\) and \(c(x_i)\) contribute, and such sets have \(\lvert Y\rvert\ge D+1\). Cauchy on the polydisc of radius \(R/2\) gives \(\lvert\partial_i\varphi_{x,Y}\rvert\le2Ae^{-a\lvert Y\rvert}/R\). The DFS count of [Hidden components] Lemma A4 gives at most \(N^{2(n-1)}\) connected sets of \(n\) cells containing a given cell. Sum the geometric series. \(\square\)

For multiscale cubes of local scale, with adjacent layers differing by one scale (the [III] geometry), one may take \(N\le3^d(L+2)^d\) for \(*\)-adjacency and \(c_{\mathcal C}=2\sqrt d\). This is deduction given that geometric property, which is additional assumption from [III] §3.

## 3. Route I: the source's T-step localization (zero-range)

### 3.1 What the source prints

- **[III] p.268, (3.15).** The current fluctuation enters only through \((\mathbf E_k+\mathbf R_k+\mathbf B_k)(U_k(\exp i[g_kCA_k-h\widetilde D(g_kCA_k)]V^{(k)}))\). The small-field restriction is (3.16): \(\sup_b\lvert A_k(b)\rvert<\delta_k\) (normalization discussed in §5).
- **[III] p.276.** "After the completion of the operations of Sects. 3–5 [I] we localize the obtained expressions. We repeat again the analysis of Sect. 6 [I], with the only change that the random walk expansions we use now are constructed for the sequence \(\{\Omega_j\}\), so we apply Theorems 3.7–3.10 [13] in their full generality. The expansions (6.9) [I] are constructed for families \(\sigma_0=\{\Delta\}\) of cubes in proper scales, i.e. if \(\Delta\subset\Omega_j\setminus\Omega_{j+1}\), then the size of \(\Delta\) is equal to \(ML^j\eta\). Then we resum them in localization domains \(Y_0\in\mathbf D_k\) […]. The remaining terms satisfy such conditions also, but with analyticity space (I.6.34) replaced by the space
\[
\widetilde U^c_{k+1}(Y,(1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1)\times\{A:\operatorname{supp}A\subset Y\cap\Lambda^{(k)*}_{k+1},\ \lvert A\rvert<C_1p_1(g_k)\}.\ \ (3.43)
\]
Notice also that the localization domains occurring in this expansion have nonempty intersections with \(\Lambda_{k+1}\). […] The expression determined by the boundary terms \(\mathbf B_k\) is much simpler to deal with. To its terms we apply the formulas (3.6), (3.7) [I], and next we localize the obtained expressions. The localized expansion is over domains \(Y_0\in\mathbf D_k\) having nonempty intersections with \(\Lambda_{k+1}\). Terms of this expansion can be extended [as in (I.3.13)] to analytic functions defined on the corresponding spaces (3.43)."
- The \((U,J)\) argument in (3.43) is the **new** background \(U_{k+1}\), which is fixed by the outer variables \(V_{k+1}\) and independent of \(A\). So the whole current dependence of a localized term is through \(A\restriction Y\cap\Lambda^{(k)*}_{k+1}\).
- **Small-field model of the proof ([II] §1, source).** The minimizing field \(H_k(B')=H_0B'+A_0-HD(H_0B'+A_0)\) (1.2) is localized by decoupling the propagators' random-walk expansions with parameters \(s(\Delta)\) ((1.6)–(1.10)). Each term for a connected \(Y_0\) "depends on propagators and function \(B,s\) restricted to the component \(Y_0\)". It is analytic for \(\lvert s(Y_0)\rvert\le e^{\kappa_1}\) and \(g_k\lvert B\rvert<\varepsilon_1\) (1.21), "and all the bounds above are uniform on the domain" of \(U,J\). The Cauchy estimate in \(s\) gives \(e^{-(\kappa_1-1)\lvert Y_0\setminus\square^4\rvert}\) ((1.23)–(1.25)). The resummation over old \((j,X)\) at fixed \(Y\) uses (1.26) and the factor \((L^j\eta)^5\) of E-terms ((1.24)–(1.29), (1.30)–(1.32)).

### 3.2 Theorem I conditional

**Inputs.**
- **(S-T).** At the T step \(k\to k+1\), the current-dependent part of the integrand equals \(\sum_YF_Y\) over \(Y\in\mathbf D_k\) with \(Y\cap\Lambda_{k+1}\ne\emptyset\), plus terms independent of \(A\). Each \(F_Y\) is analytic on (3.43) and bounded there by \(w_Y\le We^{-\kappa_*\delta(F_Y)}\), uniformly in the old data. Here \(F_Y\) is the paid part of \(Y\) in multiscale cubes, outside declared holes, with (FT) for non-eligible components ([Boundary estimate d] §1).
- **(R).** \(C_1p_1(g_k)\ge(1+\theta)P_k\) for a fixed \(\theta>0\) (§5).

**Conclusion.** With \(r:=\theta P_k\), every \(F_Y\) satisfies (Loc★) in zero-range form on \(\mathcal S_r\), with \(S_Y=\{i:x_i\in Y\}\) and \(\sup\lvert\partial_iF_Y\rvert\le w_Y/r\). The derivative is uniform in all frozen and integrated old data, including tag variables under Route A. The bound does not depend on the volume, the age of any old structure, or the distance to hidden carriers. Prop. Z then gives all current jets of (S1)+(S2) in terms of one rooted norm \(\mathfrak N\).

*Proof.* \(\mathcal S_r\subset\{\lvert A\rvert<C_1p_1\}\) by (R). Apply Cauchy in the single coordinate \(z_i\). For \(x_i\notin Y\), \(F_Y\) does not depend on \(z_i\). \(\square\)

### 3.3 What (S-T) contains, and its status

- The **statement** is (c) of [III] p.276.
- Its **proof** is "the same as in [I]", with multiscale random-walk expansions ([CMP99] Theorems 3.7–3.10). The small-field version has displayed proofs in [I] §6 and [II] §1 (source). The multiscale generalization is asserted, not displayed. By the completion test, (S-T) is a primary formula that remains a premise until it is checked.
- **The resummation at fixed \(Y\) is where the fine multiplicity is paid.**
  - B-terms are anchored at \(Z_j^\sim\subset\Omega_{j+1}^c\), i.e. in grade \(\le j\). There the cubes of \(Y\in\mathbf D_k\) have the local scale, which is \(\le j\). So at most one \(\mathcal G_j\)-anchor of an old \(X\) lies in each cube of \(Y\), and the multiplicity is \(\le\lvert Y\rvert\), paid by \(e^{-\kappa_1d_k(Y)}\).
  - E-terms anchored in coarse regions are paid by their volume factor \((L^j\eta)^5\) ([II] (1.24), source).
  - This is the "multigrid" mechanism of [Boundary estimate d] Rem. 3, as the source uses it. Status additional assumption for the B-term counting, which is an additional hypothesis.

### 3.4 Consequence for C-05 and the interface with (M2)

On Route I, **all** current-dependent records at the current step have the current birth and multiscale carriers.

- [Hidden components] Theorem C's birth sum and (Geo) are not needed for the derivative estimate of (S1). They are replaced by Prop. Z, with \(\mathfrak N=\sup_i\sum_{Y\ni x_i}w_Ye^{(\chi M+1)(\delta(F_Y)+2)}\).
- \(\mathfrak N<\infty\) uniformly is a count of multiscale localization domains containing one current-scale point, weighted by \(e^{-(\kappa_*-\chi M-1)\delta}\). It is the single-birth case of the incidence hypothesis (M2). The argument requires it here, to avoid duplicating that work.
- (S2) still needs the collar, because the per-kernel load \(\Lambda_v\) sums over all attachment positions. With zero range the collar enters through the weight. Take a record \(e\) attached to \(Q_v\) with \(x_l\in F_e\). By (Col\(_j\)), the Euclidean distance from \(x_l\) to \(Q\) is \(\ge s_jd^{(j)}(x_l,\cup Q)\ge\theta\Delta_Q\), because the capped unit is \(\ge s_j\). So \(\delta_j(F_e)\ge\theta\Delta_Q/s_j-2\sqrt d\), and \(w_e\le We^{-\kappa_*(\theta\Delta_Q/s_j-2\sqrt d)}\) pays \(N_{\rm att}(Q)\le3^d(\Delta_Q/s_j)^d\), both being measured in grid-\(j\) units. This is [Boundary estimate d] R6, Step 2, with \(\nu=\infty\).

## 4. Route II: global background map and native disc (the AO–AR route)

### 4.1 Theorem II conditional

A primitive record is \(F_\rho(z)=b_\rho(\Phi(z)\restriction X)\), where \(\Phi(z)=(U_k(I_k(z)),J(U_k(I_k(z))))\) is the step-\(k\) background map. In the form of AR AD17.3, \(\Phi\) is the fixed-old-field replacement \((U_L^{v^{-1}},\operatorname{Ad}_{v^{-1}}J_L)\).

**Inputs.**
- **(V)** \(\lvert b_\rho\rvert\le K_\rho=B_0e^{-\kappa d_j(X)}\) on \(\widetilde U^c_j(X,\tilde\alpha_0,\tilde\alpha_1)\) ([III] (2.42), (c) p.261).
- **(A)** Admission. For \(z\in\mathcal S_r\), the strong-norm ball of radius \(\rho_0\) about \(\Phi(z)\restriction X\) lies in that domain. This is [U17] NP.5 together with AD17.28 and (R).
- **(T)** Tangent decay. \(\lVert\partial_i\Phi(z)\rVert_{\mathfrak N,X}\le\frac{\tau}{r}\sup_{x\in X}e^{-\mu d_\Omega(x_i,x)}\), where \(d_\Omega\) is the step-\(k\) scaled distance ([CMP96] (2.46), [BM] (BM.2)).

**Conclusion.** (Loc★) holds with \(w_\rho=K_\rho\tau/\rho_0\) and \(\nu=\mu M\).

*Proof.* Lemma 2. Then \(d_\Omega\ge M\,d_g\) ([Boundary estimate b] Lemma G1, using that grade \(k+1\) on \(\Omega_{k+1}\) has a unit \(L\) times coarser than the \(h_k^{-1}\)-weight of \(d_\Omega\)), and \(d_g\ge d^{(b)}\). Since \(d_j(X)\ge\delta_j(X)\) (multiscale cubes are no coarser than \(\mathcal G_j\)), \(w_\rho\le W_je^{-\kappa\delta_j}\). \(\square\)

### 4.2 The scale-change accounting (deduction; given the raw kernel bound)

Suppose (T) is supplied in raw form: \(h_n\lvert\partial_iA_L(x)\rvert\le Cg_ke^{-\delta d_\Omega(x_i,x)}\) for \(x\) in layer \(n\) ([U17] (JI.34)). The record's domain (2.39) normalizes layer \(n\le j\) by \(L^n\xi\lvert A'\rvert<(1-\beta)\alpha_{1,n}\), and layers \(n>j\) by the birth scale \(j\).

- **Layers \(n\le j\).** The normalized tangent is \(\le\frac{Cg_k}{\alpha_{1,n}}e^{-\delta d_\Omega}\le\frac{Cg_k}{\alpha_{1,k}}C_{\rm AF}\sqrt{1+k-n}\,e^{-\delta d_\Omega}\). By (BM.3), \(d_\Omega\ge RM(k-n-1)_+\), so \(\sqrt{1+k-n}\,e^{-\frac\delta2RM(k-n-1)_+}\le C'\).
- **Layers \(n>j\).** Here \(h_j\lvert\partial_iA\rvert\le L^{-(n-j)}h_n\lvert\partial_iA\rvert\). The factor \(L^{-(n-j)}\sqrt{1+n-j}\le C\) pays the extra ratio \(\alpha_{1,n}/\alpha_{1,j}\).

Hence \(\tau=Cr\,g_k/\alpha_{1,k}=Cr/r_*\) with \(r_*:=\alpha_{1,k}/g_k\), and
\[
w_\rho=\frac{C}{\rho_0}\frac{r}{r_*}B_0e^{-\kappa d_j(X)},\qquad\nu=\tfrac\delta2M.
\]
**The age \(k-j\) does not appear.** The mesh powers cancel exactly: the output factor \((L^n\eta)^{-1}\) of [V] (190) matches the domain normalization. The input factor \((L^{j'}\eta)^{-d}\) cancels against the measure ([BM] (BM.7)). The fine-anchor multiplicity is not part of (Loc★); it is paid by (Geo) in Theorem C.

**Routes I and II give the same Hessian scale.** Route II on \(\mathcal S_r\) with \(r\le c\,r_*\) gives \(w/r\propto B_0/r_*\). Route I gives \(w/r=W/(C_1p_1-P_k)\). Both are \(\asymp B_0g_k/\alpha_{1,k}\) per derivative. The construction's choice \(P=2P_k\) together with \(\vartheta_k=g_kP_k/\alpha_k\) is the same budget written differently.

### 4.3 The tangent input (T): two sources

- **[V] (190)** source input. The bound covers \(\delta/\delta B_\nu(y')\,\mathscr H_\mu(B,x)\), its gradient, the \(\beta\)-Hölder norm, \(D^*D\) and \(\Delta\), by \(O(1)[(L^j\eta)^{-1},(L^j\eta)^{-2},\dots,(L^j\eta)^{-3}](L^{j'}\eta)^{-d}\exp(-\frac18\delta_0d(y,y'))\). It is derived from (188), Lemma 2.1, Prop. 2, (181) **and (189)**. Of (189) the source states: "To prove an exponential decay we have to investigate more closely the kernel \(((\delta^2/\delta A'^2)V)(A')\). This is, unfortunately, a very awkward and complicated problem, although quite straightforward. […] **We do not perform these calculations here**, we have obtained all necessary results to do the calculations and estimates, let us formulate a final result only." (p.308). Prop. 9 (p.309) asserts (190) for the extension to complex \(B\) and to regular external backgrounds. **So (190) at nonzero data is a primary assertion without a primary proof.**
- **[II] §1 decoupling** (source). Lemma 3 applied to the expansion (1.10) of \(H_k(B')(x)\) gives (T) in the multiscale decoupling-cube metric. Its inputs are the bound (1.7) on the walk terms ([CMP99] (3.108)) and analyticity in \(s\) and \(B\) on \(g_k\lvert B\rvert<\varepsilon_1\) (1.21). Here \(R=\varepsilon_1/g_k\gg P_k\), and the decay rate is \(\kappa_1-c\). This is a source route with displayed proofs (small-field, single sequence). The multiscale version is [III] p.276's "full generality". **One may use it over (190).** conditional on (1.7), (1.21) and the multiscale generalization.

The linear part of the kernel (\(H_1=G_1Q^*(QG_1Q^*)^{-1}\), [U17] RM.6) needs neither. Its decay is a propagator bound in [CMP99] (3.127)–(3.133), which [U17] AP cites; The argument assumes it.

## 5. The radius premise (R)

### 5.1 Source data

- [III] (2.28), p.259: "\(\alpha_{0,j}=g_jC_0(\log g_j^{-2})^{q_0},\ \alpha_{1,j}=g_jC_1(\log g_j^{-2})^{q_1}\), where \(q_0,q_1\) are integers greater than 1, \(C_0,C_1\) are sufficiently large positive numbers."
- [III] (3.43), p.276: \(\lvert A\rvert<C_1p_1(g_k)\). The constant symbol \(C_1\) is the one in (2.28).
- [III] p.265 and (3.16), p.268: \(\delta_k=g_k(A_1/A_0)p_0(g_k)\) and \(\sup\lvert A_k\rvert<\delta_k\). The intended normalized support is \(P_k=\delta_k/g_k\); the literal reading would make the Gaussian fluctuation support \(\ll1\) ([U17] AR §2.1).
- LFR I p.183 (source): "\(\delta'_j=g_jA_1p_1(g_j),\ p_1(g)=(\log g_j^{-2})^{p_1}\), and \(p_1<p_0\)". This is the primed preparation threshold.
- LFR II p.379 (source): the first-order term is bounded by "\(O(1)B_3^2A_1^2p_1^2(g_k)\lvert\mathbf B_0\rvert(\alpha_{0,k}+\alpha_{1,k})<O(1)B_3^2A_1^2C_0M^dR_k^{d+2}p_1^2(g_k)q_0(g_k)g_k\)". So Bałaban writes \(q_0(g)\) for \((\log g^{-2})^{q_0}\).
- [I] p.263 (source): in the small-field paper "\(\alpha_0,\alpha_1\)" are "absolute constants (i.e., constants independent of \(X\) and \(j\))", and the current radius is \(\varepsilon_1/g_k\) ([II] (1.21), (1.34)).

### 5.2 Readings

| Reading of \(p_1\) in (3.43) | \(C_1p_1(g_k)\) vs \(P_k=A_1\ell_k^{p_0}\) | (R)? |
|---|---|---|
| \(p_1\equiv q_1\)-polynomial, so \(C_1p_1(g_k)=\alpha_{1,k}/g_k\) | \(C_1\ell^{q_1}\) | yes iff \(q_1>p_0\), or \(q_1=p_0\) and \(C_1>(1+\theta)A_1\) |
| \(p_1\equiv p_0(g)=A_0\ell^{p_0}\) | \(C_1A_0\ell^{p_0}\) | yes: \(A_1/A_0\) is small in the source and \(C_1\) large |
| LFR I's \(p_1\), exponent \(<p_0\) | \(o(P_k)\) | no |

**The consistency argument additional assumption.** The T step integrates the localized integrand over the real support \(\lvert A_k\rvert<P_k\) (intended (3.16)). A term defined only on (3.43) must therefore be defined on that support, so \(C_1p_1(g_k)\ge P_k\). The third reading violates this. Under it the source would integrate outside its own analyticity domain, so that definition is inconsistent, in agreement with [U17] AR §2.2. The two consistent readings give (R) with a fixed margin. additional assumption, with every fact.

**Route II needs the same premise.** [U17] AD17.15 sets \(\alpha_{i,n}=C_ig_n\ell_n^q\) with \(q>p_0\), "the already proposed normalization radii", and NP.20 needs \(\vartheta_k=g_kP_k/\alpha_k\to0\). In the source this is a choice of \(q_0,q_1\) in (2.28) ("integers greater than 1"). It is the first reading's (R). Its compatibility with the rest of [III]/LFR is not checked in AO–AR. Every displayed smallness condition the source states has the form \(g\cdot\mathrm{polylog}(g^{-1})\ll1\) and tolerates any fixed \(q\). That is additional assumption. **So AR §§2.3, 6 ("the native-ball route … establish[es] the required radius independently, without deciding the typographical intention of \(p_1\)") is overstated:** the native-ball route assumes (R) in its (2.28) form.
