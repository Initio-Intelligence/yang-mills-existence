# Chart factors, covariance and exactness for the local test

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

**Local-chart hypotheses.** In every application use (A8′) in the structured form 3′ and 4′, F(4′) on (Avg), (Sm3′), (Par-g_Z′), and (Lay-W), with $M_W\mid M_1$ and $M_1\ge6M_W$. In particular the per-potential rate must satisfy $\kappa_1/2\ge\sqrt d(1+3\beta)\kappa/(1-3\delta)$. The bound on the joint terminal law requires the action estimate and item 4′.

## 1. the tube expansion (Lemma 3.4) and its decoupling input

### 1.1 What the source itself does

* **[II] pp.4–6 (source), (1.9)–(1.18).** \(\mathbf E(\square_0,\dots\mathbf H_k(B'))\) is expanded with \(s(\Delta)\) on \(M\)-cubes, by the fundamental theorem of calculus over \(\sigma\subset\sigma_0\). "Kernels of the operators \(H(s),\tilde G(s),H_0(s)\) vanish, unless both arguments are in the interior of one component of \(Y(\sigma)\)". The solution of the response equations "restricted to the interior of a component depends on \(A',H(s)\), hence \(s\) restricted to this component". The output is the sum (1.10) over connected \(Y_0\supset\tilde\square^4\). The walk bound (1.11) has "\(\delta_0d(\omega)\ge\delta_1mM\)" for \(m>2^4\). (1.18) gives \(\lvert\mathbf H_k(s(Y_0),B')\rvert\le4B_0e^{16\kappa_1}\lvert B'\rvert\). p.6: "all the considered functions and operators are analytic functions of the configurations \(\mathbf U,\mathbf J\) in a domain given by the conditions I.(i)–(iii) … and all the bounds above are uniform on the domain." The last sentence is an assertion, not a proof.
* **[LFR II] pp.372–374 (source).** For \(\mathbf E^{(j)}(X,\mathbf U''_k,z)\) depending on \(\mathbf H''_k(g_kB)\) restricted to \(\square_0\): "we apply the expansion (6.9) [I] … with \(\sigma_0\) defined as the set of cubes \(\Delta\) disjoint with \(\square_0\) and \(\Lambda^\sim\). … the summation is over domains \(Y_0\in\mathbf D_k\) containing \(\square_0\), and at least one of the components of \(\Lambda^\sim\). **The other terms in the expansion vanish, because of the localization of the field \(B\).**" The same is then done for \(\mathbf H_{\mathbf B_1}\), \(\mathbf H_k\) with \(\tilde\sigma_0\) (pp.373–374).

So the structure of Lemma 3.4 is Bałaban's own device:

1. decouple the response of a multi-level determining-set problem;
2. keep only components containing the output point;
3. discard every term whose component does not reach the support of the datum.

The source applies it to response functions of component-type determining sets (\(\mathbf B''_k(Y_1)\), \(\mathbf B_1(Y_2)\), \(\mathbf B_k(Y_3)\)) at analytically extended backgrounds. Lemma 3.4 adds no new kind of input. It applies an input the source already uses to one more family of determining sets (the boxes \(\mathbb B_b\)).

### 1.2 The vanishing mechanism — deduction given [Dec]

On a slice \(s=0\) off \(R\cup T\), the deformed response at sites of the root component depends only on the datum there (Local deformation of propagators and the minimizer Theorem M(2); [II] p.4). If \(R\cup T\) does not meet the collar \(\mathcal L_b\), that datum is \(0\). The deformed system then has the solution \(\mathscr H_b(s;0)=0\): \(D\) and \(\delta V/\delta A'\) vanish to second order, and the small fixed point is unique by contraction ([II] (1.16); Local deformation of propagators and the minimizer Theorem M(1)). So the composite \(\Phi\) equals its value at zero datum, which is \(0\) by (H8). Every \(\Phi_T\) with \(R\cup T\) not reaching \(\mathcal L_b\) is then \(\int\partial^T\) of a function independent of \(s_T\), hence \(0\).

* the terms sum to \(\Phi(1)\) exactly;
* all \(1013\) terms that are disconnected or miss the collar vanish (\(<10^{-13}\));
* the \(11\) surviving terms are unchanged (to \(3\cdot10^{-24}\)) when the background and the datum outside \(R\cup T\) are re-randomised;
* they decay geometrically in \(\lvert T\rvert\).

Local deformation of propagators and the minimizer Theorems W, D and M are proved in the abstract. Domains of the representation-defined derivatives checked them deduction. Source operators for the deformed reconstruction M♯ is conditional on Prop. W♭ ([P] Thms 3.7, 3.9, 3.10, (3.132) as printed and sketched), with the collar estimate right-form repair (S-calc♯) pending the second reading of Lemmas PL/GP.

M♯ is stated for "the sequence \(\{\Omega_n\}\)" and "backgrounds in the complex domain \(\mathfrak U\) of [P]". Three points must hold for \(\mathbb B_b=\mathbf B_{k+1}(\square_b^{\sim4})\):

1. **[P]-type sequence.** By [III] p.256 (source), \(\mathbf B_j(\Omega)\) has layers \(\Omega_n\), each a union of \(L^n\xi M_1\)-cubes, with \(\operatorname{dist}(\Omega_n,\Omega_{n-1}^c)\ge L^n\xi M_1\). This is exactly the generality of [P], whose constants "do not depend on the sequence" (Local deformation of propagators and the minimizer S1, p.399). source input; additional assumption.
2. **Tiling.** The layers are thinner than \(M\)-tiles, so Multiscale incidence and logarithmic jets's proper tiling (premise (Thick)) does not exist. W0 allows over-sized tiles, so one uniform tile scale works (E4).
3. **Background domain.** On \(\square_b^{\sim4}\subset\Omega_{k+1}\) (B5) the space \(\tilde U^c_{k+1}\) imposes the top-level (strongest) regularity. The box sequence asks for weaker regularity in its finer collar layers, so the space lies inside the box problem's \(\mathfrak U\). additional assumption: The argument assumes the normalisations of [P] (3.35)–(3.38) with [III] (2.34)–(2.39) line by line.

The same three points apply to the component problems \(\mathbb B^{(n+1)}_k(Z)\) needed in §5. There the source itself asserts the device (§1.1).

**Constants.** The datum must lie in M♯'s ball: \(\lVert B_b(\mathbf U)\rVert_\infty\le C_Bg_k\ell_k^q<\varepsilon_{\mathcal H}=c_S\hat B^{-6}\), with \(\hat B=2n_0B_se^{2^d\kappa_1}\). This is a coupling ceiling of the same type as the representation convention's. It belongs in (A9), and B-02 must verify it (§8).

**Conclusion on Attack 1.** Lemma 3.4 holds at conditional on [Dec]. [Dec] is: M♯ (b on (W-ms) and printed source theorems, pending PL/GP) together with reading (d) that it applies to \([P]\)-type sequences with \(M_1\)-thick layers on a uniform tiling, at complex backgrounds with independent \(\mathbf J\). The source asserts the same for its own component problems ([II] p.6; [LFR II] p.372).

### 1.4 Repair E3 — deduction given [Dec]

Let \(F\) be the composite of Definition 2.5 items 2–4: the datum on the collar, \(\mathscr H_b\) at the sites of the \(k\)-block of \(b\), \(M^k\) at \(b\), and the frames at \(b_-\). Set \(\Phi(s):=F\bigl(\mathscr H_b(s;B_b(\mathbf U))\bigr)\).

* \(\Phi\) is holomorphic on \(\lvert s_t\rvert<e^{\kappa_1}\) and bounded by \(A=C\,g_k\ell_k^q\). This needs only the sup-norm row \(\nu=0\) of M♯(1) and the Lipschitz bound of \(F\) near \(0\).
* (Dec) holds with root \(R_b\) (the tiles meeting a neighbourhood of the \(k\)-block of \(b\)). Its depth is \(\ge0\) by Local deformation of propagators and the minimizer Lemma 4.1 (R1)–(R4), because \(F\) is local at block scale and blocks lie inside tiles.
* Local deformation of propagators and the minimizer Theorem D gives \(\Phi(1)=\sum_T\Phi_T\) with \(\lvert\Phi_T\rvert\le A(e^{\kappa_1}-1)^{-\lvert T\rvert}\), each \(\Phi_T\) depending only on \(R_b\cup T\).
* §1.2 gives \(\Phi_T=0\) unless \(R_b\cup T\) is connected and meets \(\mathcal L_b\).

This is Lemma 3.4 verbatim, including (H5), (H6) and (H8) term by term. (H5)/(H6) per term need gauge and lattice covariance of the individual walk terms. The source asserts this for its localized terms ("gauge invariant", [II] Lemma 2, source). additional assumption

### 1.5 Repair E4 and the counts

\(D_{\rm coll}\ge2M_2R_{k+1}-2M_1-1\) in \(T^{(k+1)}\) units ((B2) and [III] p.256: the collar has width \(\le2M_1\)).

* **Tiles of scale \(k+1\)** (side \(M\) in \(T^{(k+1)}\) units): \(n_{\rm coll}\ge D_{\rm coll}/M\ge M_2R_{k+1}/M\). Each tile contains \(L^d\) \(M\)-cubes of \(\pi_k\), so \(d_k(T)\le c_LL^d\lvert T\rvert\), and \(\tfrac12\kappa_1\ge c_LL^d\kappa\) is needed.
* **Tiles of scale \(k\)**: \(n_{\rm coll}\ge LD_{\rm coll}/M\) (as in [RD]). Then \(\kappa_{\max}\to\kappa_{\max}/L\) (Source operators for the deformed reconstruction (E5)), and \(\tfrac12\kappa_1\ge c\,\kappa\) suffices.

Either way \(\kappa_1\) is fixed after \(\kappa\) and before \(M\) (\(\kappa_1\le\kappa_{\max}\propto\delta_0M\)). The order \(d,L\to\kappa\to\kappa_1\to M\to C_0,C_1\to g\) agrees with the representation convention/the collar estimate. In both cases \(c_\star=\tfrac14\kappa_1M_2/M\) times a fixed factor, and (Par-g) holds for small \(g\) because \(R_j\ge\ell_j^r\), \(r\ge2\) ([III] (2.5), c-text: "\(R_j\) is the smallest number of the form \(L^n\) such that \(R_j\ge(\log g_j^{-2})^r\)").

## 2. the R⁴-against-R count and the R/B classes

### 2.1 The count — deduction, definitions

* **Index sets.** R-terms are indexed by \(X\in\mathbf D_j\) with bound \(g_j^{\kappa_0}e^{-\kappa d_j(X)}\), "\(\kappa_0\) can be chosen arbitrarily large" ([III] p.260, source, (2.30)–(2.31)).
* **Linear size.** \(\mathbf D_j\) consists of connected unions of cubes of \(\pi_j\) (the \(M\)-partition). \(d_j(X)\) is the length of a shortest tree meeting all cubes, divided by \(M\) ([I] §0, source).
* [LFR II] p.380 (source) distinguishes "\(d'_j\) … the linear size defined in terms of \(MR_j\)-cubes **instead of \(M\)-cubes**".
* [LFR II] (1.100), p.390 (source): \(\lvert\mathbf R'^{(k)}(X,(\mathbf U,\mathbf J))\rvert\le\exp(-p_0(g_k))\exp(-\kappa d_k(X))\), with \(X\in\mathbf D_k\).

The R-class is therefore measured in \(M\)-cubes, and a box of side \(\sim2L^2M_2R\) has \(d_k\sim(2L^2M_2R/M)^4\). With B-02's constants (\(L=13\), \(M_2=L^2M_1\), \(M=L^6\), \(R=L^n\)) finite comparison gives:

| \(n\) | \(d(\text{box})\) | collar tiles \(n_{\rm coll}\) |
|---|---|---|
| 4 | \(3.7\cdot10^{14}\) | \(1.7\cdot10^{2}\) |
| 10 | \(2.0\cdot10^{41}\) | \(8.2\cdot10^{8}\) |

Box-locality fails (2.31) by many orders of magnitude. Tube localization is necessary. F3 is confirmed.

### 2.2 The new terms are R-class and B-class — conditional

[RD] Theorem 4.5 items 1–7, on Lemma W, [Dec] and the source's cluster expansion (3.44)–(3.47) (pp.277–278: \(H'(Z_0)\) "satisfies the same bound as the other factors").

**Analyticity domain.** Lemma W (W1) holds on \(\tilde U^c_{k+1}(X,(1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1)\times\{\lvert\tilde A\rvert<r-1\}\), where \(r\) is the radius of the source terms. The chart shift is \(\le2g^{-1}\lvert\mathbf H\rvert\le1\) for \(\lvert\mathbf H\rvert<\rho_H=\frac12g_k\). The construction reads the radius as \(r_T\ge(1+\theta)P_k\) (Local deformation of propagators and the minimizer Prop. R; Domains of the representation-defined derivatives: \(\min(q_0,q_1)\ge p_0\)). The new terms lose 1 in the radius, which is harmless.

**Bound.** \(g_k^{\kappa_0+2}e^{-(1-5\delta)\kappa d_k(X)}\) (§4.2). After integration and rescaling, \((1+4\beta)\kappa d_{k+1}\) follows because the gain per step is at least \(L^{1/2}\) ([LFR II] p.384 cites the scaling (6.31) [I]) and \((1-5\delta)L^{1/2}\ge1+4\beta\) for \(L\ge13\). conditional

**Locality, covariance, \(\Lambda\)-independence, vacuum.** As in [RD]. Two additions:

* **Euclidean covariance (2.32)** needs every partition the term sees (\(\pi'\), the \(M\)-partition, the blocks) to be mapped to itself by each transformation preserving the \(MR_{k+1}\)-partition. B-02's constants (odd \(L\); \(M_1,M_2,M,R\) all powers of \(L\)) give nested cube partitions with common face *and centre* planes. Odd \(L\) is what makes the central sub-cube concentric.
* **Merging into \(\mathbf E_k\)** ([III] pp.270–271: the partition cubes are "contained in \(L\)-cubes corresponding to the \(L\)-blocks"). It applies to \(\mathbf R_W^{(j)}\) for the same reason.

**Which R-terms go where.** [III] (2.30) (p.260) localizes \(\mathbf R^{(j)}\) in \(\Lambda_j^{\sim-1}\). p.279 (source) assigns the terms with \(X\subset\Lambda_{k+1}\) to \(\mathbf R''^{(k+1)}\) and "the remaining terms … again into the boundary term". This index discrepancy is the source's. \(\mathbf R_W\) follows p.279, so whatever reading settles the source applies to \(\mathbf R_W\) verbatim. additional assumption

**B-class.** The terms with \(X\not\subset\Lambda_{k+1}\) and all \(\mathscr V_{\rm bd}\)-terms are B-terms with the **full** decay of (2.42). p.262 (source) makes the full-decay form the main-line assumption ("we have chosen the ones above, because they agree with the assumptions for E-terms and R-terms"). The resummed \(d_j(X\setminus Z_j)\) form is an alternative. Tube localization gives the full form. conditional

## 3. the second non-local test, every label rule, and the locality proposition

### 3.1 F5

* [IV] p.180 (source), (1.18): \(U^{(n)}_k=U(\mathbb B^{(n)}_k,V)\), with \(\mathbb B^{(n)}_k\) containing \(\mathbb B_k\cap(\Omega_k\cup Z^c)\) ((1.14)–(1.17)): the whole-lattice determining set.
* p.187, (1.53): \(V^{(j)}=M^j(U^{(n+1)}_k)\).
* p.188, (1.55): \(\chi'^{(j)}=\chi(\{\lvert B_j(b)\rvert<\delta'_j\})\); "We exclude from \(Z\) the components with the large field function \(1-\chi'^{(j)}\)".
* (1.58): \(\mathbb H^{(j)}_Z\) "is an analytic function of the configuration \(U^{(n+1)}_k\) restricted to \(Z\)", and that configuration depends on \(V\) outside \(Z\).

The label is non-local. It sits after the p.183 sentence that TM §5.2 item 6 quotes. **F5 is confirmed.**

### 3.2 Every label rule, read on the pages

| Rule | Where (source) | Background used | Local? |
|---|---|---|---|
| \(P_0\), \(P_1\) (first step) | [III] pp.245–246 source input, (1.2)–(1.4) | bare plaquettes; \(U_{1,\square'}\) | yes |
| Soft axial gauge (1.5) | [III] p.247 | product over sites of normalized single-site integrals | yes (seeds) |
| \(Q_1\) (1.8), \(Q\) (3.3)–(3.4) | [III] pp.247, 265 | \(U_{1,\square'}\), \(U_{k+1,\square'}\) | yes |
| \(P\) (3.2) | [III] p.265 | \(U_{k+1,\square'}\) | yes |
| \(R\) (1.18), (3.16) | [III] pp.250, 268 | **global** \(U_1\), \(U_{k+1}\) | **no** → (A1) |
| \(\Omega\), \(\Lambda\), \(S\), hulls (1.10), (1.20), (3.5), (3.20) | [III] pp.248, 251, 265, 269 | geometry; hull inside \(100LMR\) | yes |
| \(\chi^{(n)}_k\) (1.22)–(1.24) | [IV] pp.181–182 | \(U^{(n)}_{k,Z}\) (1.20), component | yes |
| \(\chi'_j\) (1.27) | [IV] p.182 | \(V^{(j)}_Z=M^j(U^{(j+1-h)}_{k,Z})\) | yes |
| Completion (1.28) | [IV] p.183 | chart variable of (3.22): \(V^{(j)}_{\Lambda^c\cap\Lambda_j}\) (component) or, amended, \(V^{(j)}_b\) | yes |
| \(\chi'^{(j)}\) (1.55) | [IV] p.188 | **global** \(U^{(n+1)}_k\) | **no** → (A8) |
| \(\chi_{k,\Lambda}\) (1.75) | [IV] p.193 | \(U_{k,Z}\) | yes |
| \(\chi'\) (1.82) | [IV] p.196 | \(V_0=M_{\mathbb B''_k}(U_0)\), \(U_0=U_{k,Z}(V_\Lambda)\) | yes |
| \(\chi_{k,1/2}\) (1.88) | [IV] p.197 | \(U_{h,\square}\) | yes |
| \(\chi(\Lambda_i)\) and resampling kernel (1.100)–(1.101) | [IV] p.201 | \(V_{\Lambda_i}\), \(U_{k,X_i}\) | yes |
| Eligibility (i), (ii) | [IV] p.177 | labels in a \(100MR_k\) cube | yes |
| Second class \(\chi_k((\Omega_k^{\sim-4})^c)\), \(\chi^c_k(Y^{\sim-6})\) | [LFR II] p.378 | \(U_{k,\square}\) ((2.17), p.257) | yes |
| Growth (1.76) | [LFR II] p.381 | deterministic | yes |
| Averaging over \(2^d\) reflections × \(d!\) permutations of the gauge graph | [LFR II] p.379; [IV] p.201 | mixture (seed) | yes |

[LFR II] pp.355–377, which [RD] did not read, contain no decomposition of unity that produces a label. They contain:

* the smooth localization partition "connected with the partition \(\pi_k\)" (p.360);
* the \(\zeta\)-cutoffs;
* the new determining set and background (1.33)–(1.35), (1.50)–(1.58);
* the localization expansions (pp.372–376).

None of these is a label. [III] pp.253–264 and 272–285 contain no further decomposition of unity (c-text search; the "special decomposition of unity" of p.263 is a device in the proof of (2.43)).

**There is no third non-local rule.** Two rules use a global background, (3.16)/(1.18) and (1.55), and (A1) and (A8) replace both.

### 3.3 Finite propagation — conditional

With (A1) and (A8), each label is a function of the following:

* **T-step:** fields within \((L+8)LM_2R_{k+1}\) of its cube ((B4)).
* **R-operation:** fields within its eligible component, which lies in a cube of side \(100MR_k\).
* **Gauge fixing:** seeds at sites.
* **Resampling:** seeds at the component.

(FP) follows with \(\rho\) independent of \(n\), by TC Prop. 5.3's geometric sum. The inputs are this page reading and TM items 2 and 7 on seed realization (c\*; The formula gives the product structure of (1.5) on p.247). **[RD] Proposition 8.1 holds.** TC Prop. 5.3 as stated (only (3.16) replaced) is false, as [RD] says. Repair E1 changes no label.

### 3.4 Gauge and reflection covariance of the amended tests — deduction, with one stated condition

* **(H5).** : \(u_{\mathbf U^u}=u_0u_{\mathbf U}u^{-1}\), and \((\mathbf U^u)^{\rm ax}=(\mathbf U^{\rm ax})^{u_0}\) by uniqueness of the frame normalized on \(T^{(k+1)}\). The datum transforms by \({\rm Ad}(u_0(c_-))\) bondwise, and the frame of \(W^{u_0}\) is \(u_0u_Wu_0^{-1}\). The final identity checks.
* **Label invariance.** The label is invariant under \(V_{k+1}\to V^v_{k+1}\) together with \(V_k\to V_k^{u_0}\) (\(u_0\) block-constant). Like the source's Q-test, it is **not** invariant under non-block-constant gauge transformations of \(V_k\). It depends on the soft axial gauge of \(V_k\), which seeds realize (TM item 2).
* **Reflections.** Reflection covariance (Prop. 5.1 item 3) needs, besides (B3), that the axial frames are reflection-covariant. [I] (0.11) (source) defines the contour variables as averages over the set \(G(y,x)\) of contours, "invariant with respect to permutations of the contours", so the axial gauge is Euclidean covariant. It also needs the reflection planes to be common symmetry planes of all partitions: odd \(L\) and \(L\)-power constants (§2.2).
* **Reflection positivity** is a property of the Wilson measure, unaffected (as [RD] says).

## 4. Proposition 4.4 and Lemma W

### 4.1 Proposition 4.4

* The source's third term on p.271 (source) is \(\log[z^{(k)}\int dA\,\chi^{(k)}\exp(-\frac12\langle A,C^*\Delta^{(k)}CA\rangle-\dots)]_{s=t=0}\).
* Its integrand ((3.25), p.270, source) also contains \(-\langle A,C^*\Delta^{(k)}CA_k\rangle\) and \(\mathbf P^{(k)}(g_k,(A_k,A))\), so it depends on the external field \(A_k\).
* The source then expands in \(tA_k\) (p.271), and \(\mathbf E^{(k+1)}\) comes from the \(A_k\)-independent part (pp.277–279).

In the amended construction the same function is evaluated at the amended chart values. As a function of \(U_{k+1}\), of the external values and of \(\Lambda_{k+1}\), \(F(0,0)\) is identical, and \(\mathbf E^{(k+1)}_0(\Lambda_{k+1},X,z)\) (p.278) is literally the source's.

The proposition is correct. As [RD] F7 says, \(\mathbf E_k\) itself differs from the literal construction's by the merged \(\mathbf R_W^{(j)}\) (size \(g_j^{\kappa_0}\)). "The regular part is the source's" therefore means "the same functional of \(\mathbf E_k\)". B-03's \(d_B\) and (G) come from the Gaussian part at \(\mathbf U=1\), where every \(\mathbf R_W\) vanishes. Unaffected.

### 4.2 Lemma W, step 3, written out — deduction, given S9 and Lemma 3.4

For a source term \(Y\), \(w(Y;\tilde A,\mathbf H)=\sum_{m\ne0}w_m\mathbf H^m\) with \(\lvert w_m\rvert\le S_Y\rho_H^{-\lvert m\rvert}\) on the polydisc in \(n_c\lvert Y^*\rvert\) variables. Substitute \(\mathbf H_b=\sum_T\hat{\mathbf H}_b(T)\) and put \(\hat\eta=\sup_b\sum_T\lvert\hat{\mathbf H}_b(T)\rvert e^{\frac12\kappa_1\lvert T\rvert}\). The absolutely convergent total is
\[
\le S_Y\bigl[(1-\hat\eta/\rho_H)^{-n_c\lvert Y^*\rvert}-1\bigr]\le S_Y\,x_Ye^{x_Y},\qquad x_Y=2n_c\lvert Y^*\rvert\hat\eta/\rho_H.
\]
The elementary inequality is \((1-y)^{-N}-1\le2Ny\,e^{2Ny}\) for \(y\le\frac12\).

**Geometry of a single contribution.** A contribution with tube family \(\{T_i\}\) is localized in \(X=Y\cup\bigcup_iT_i\). This set is connected because \(b_i\in Y\cap\Delta_{b_i}\), and it lies in \(\mathbf D_k\) because tiles are unions of \(M\)-cubes. Join a tree for \(Y\) to trees for the \(T_i\) inside the \(M\)-cube of \(b_i\). This gives \(d_k(X)\le d_k(Y)+\sum_i(d_k(T_i)+\sqrt d)\le d_k(Y)+c'\sum_i\lvert T_i\rvert\). Repeated tubes only overcount. With \(\frac12\kappa_1\ge c'(1-4\delta)\kappa\), a contribution is bounded by its weighted size times \(e^{-(1-4\delta)\kappa(d_k(X)-d_k(Y))}\).

**Sum over \(Y\).** Use \(S_Y\le C_Vp_1^2\lvert Y\rvert^2e^{-(1-2\delta)\kappa d_k(Y)}\) and absorb \(\lvert Y\rvert^3e^{x_Y}\le Ce^{\delta\kappa d_k(Y)}\) (this uses (Par-g)). Then
\[
\lvert W(X)\rvert\le C\,p_1^2\ell_k^qe^{-c_\star R_{k+1}}\,e^{-(1-4\delta)\kappa d_k(X)}\sum_{Y\subset X,\ \text{conn.}}e^{-\delta\kappa d_k(Y)}.
\]
The last sum is at most \(C(d_k(X)+1)\), since there are at most \(\#\{M\text{-cubes of }X\}\) starting cubes and a convergent connected-set sum for \(\delta\kappa\) large. This is absorbed by \(e^{\delta\kappa d_k(X)}\). Result: \(\lvert W(X)\rvert\le g_k^{\kappa_0+2}e^{-(1-5\delta)\kappa d_k(X)}\) under (Par-g). Uniform convergence on the analyticity domain gives (W1). The covariances hold term by term (§1.4).

## 5. Error E1 and its repair (A8′)

### 5.1 The error — deduction, on source input for (1.57), (1.58), (1.63), (1.70)

The shift region and the size of the shift:

* In a passing component, (A8) writes \(V_j=e^{ig_jB^Z_j}V^{(j)}_Z\), with \(e^{ig_jB^Z_j}=e^{ig_jB_j}e^{i\mathbb H^{(j)}_Z}\) ((1.58), p.188).
* The integrand of (1.60) acquires \(\mathscr A(\varphi_{\mathbb H_Z}(B^Z))-\mathscr A(B^Z)+\log\det\) on bonds of \((\Omega^c_{j+1}\setminus Z''_{j+1})^{(j)*}\).
* There \(\lvert\mathbb H^{(j)}_Z\rvert\le O(1)e^{-R_j}\varepsilon_j\) ((1.58); the region lies inside \(\Omega^c_{j+1}\setminus Z''_j\) because \(Z''_j\subset Z''_{j+1}\) by (1.11)).

Why this gives terms of whole-component size:

* \(\mathbb H^{(j)}_Z(b)\) is built from the response of the component problem to a datum in the boundary layer of \(\partial Z\) ((1.56)–(1.57)). As a function it depends on \(U^{(n+1)}_k\) on all of \(Z\).
* Hence each new term, one per source term \(Y\), is a function of the background on \(Y\cup Z\).

Why this fails the source's bookkeeping:

* [IV] books these terms as \(\mathbb C^{(n+1)}_k=\sum_X\mathbb C^{(n+1)}_k(X,U^{(n+1)}_k)\) (1.63), with \(\lvert\mathbb C^{(n)}_k(X,(\mathbf U,\mathbf J))\rvert\le C_0\exp(-(1+3\beta)\kappa d_m(X))\) (1.70), p.192. That is the **full** linear size.
* With \(X\supset Z\cap\) (support), \(d_m(X)\) is of order \(d_k(Z)\le(100R_k)^4\) (\(3.6\cdot10^{52}\) at \(n=10\) in finite comparison). The only smallness is \(e^{-R_j}\).
* LFR II's later relative form \(d_{k,Z}(Y)\) ((1.67)–(1.69), pp.376–377) applies only *after* the end-of-R resummation. The intermediate preparatory steps of [IV] are run on (1.70).

[RD] §7.2's "satisfy (1.70) with room … no tube localization … is needed here" is therefore false.

### 5.2 Repair (A8′) — conditional, on [Dec] for \(\mathbb B^{(n+1)}_k(Z)\) (§1.3)

The steps:

1. Define \(\hat{\mathbb H}_Z(b)\) on the spaces \(\tilde U^{(n+1)c}_k\) of [IV] pp.190–191, from (1.56)–(1.58), exactly as in Definition 2.5.
2. Apply the decoupling expansion of the component response, with \(\sigma_0\) the tiles of the proper tiling of \(\{\Omega_i\}\cap Z\). This is the source's own construction for \(\mathbf H''_k\), [LFR II] pp.372–374.
3. By §1.2, only tubes from the tile of \(b\) to the boundary layer of \(\partial Z\) survive. Their number of tiles is at least proportional to the scaled distance \(10M(R_{j+1}+\dots+R_{k-1})+MR_k\) of (1.57).
4. Feed the tubes into the power-series step of §4.2 (Lemma W with \(\rho_H=\frac12g_j\)).

Result: every new term is localized on a tube domain \(X\in\mathbf D_m\). It satisfies (1.70) provided \(\kappa_1\ge2c'(1+3\beta)\kappa\) and \(e^{-c\,R_j}\ll C_0\), which is a ceiling of the (Par-g) type. Its analyticity domain is that of (1.64)–(1.69) restricted to \(X\). In failing components the source's own treatment stands: the terms stay in the large-field region, as in (1.59).

**Alternative repair** (not recommended). Book the terms in the resummed B-form of [III] p.262, with \(d_j(X\setminus Z_j)\). This rests on Bałaban's unproved "all constructions and proofs … can be carried on with these inductive assumptions" source input, and the cluster expansions of the remaining preparatory integrations would then have to accept polymers covering \(Z\).

**Effect.** The labels are unchanged, so (FP) is unaffected. The construction's representation changes: (A5) now also covers (A8).

## 6. Lemma 3.1, the charts and the Jacobian

* **Lemma 3.1 — conditional** on [V] Theorem 1 (uniqueness of the critical orbit) and Proposition 9 (representation). The first equality of (3.17) (p.268, source) is "minimizer restricted = minimizer of the restricted problem with its own averages". For a rectangular union of \(M_1\)-cubes it follows from the same uniqueness, since [V] is written for general sequences. [RD]'s open item 8 is thereby reduced to the same input.
* **Frames.** The frame \(u^{-1}_{k+1,\square'}\) of (3.17)–(3.18) is the frame that returns \(\exp(iL^{-1}\eta\mathbf H)U_{k+1,\square'}\) to the axial gauge. Definition 2.5's \(u_b\) plays exactly that role.
* **Collar gauge.** The gauge chosen in the collar does not affect \(V^{(k)}_b(b)\). A residual transformation supported at collar points is block-constant there and leaves the interior unchanged.
* **Lemma 2.2.** On starred bonds the source variable is exactly \((ig_k)^{-1}\log(V_k(b)V^{(k)}(b)^{-1})\) (p.249: the linearizing map is the identity off \(b_0(c)\)). Starred bonds are Haar-distributed given \(V_{k+1}\), because the constraint is solved on \(b_0(c)\) (p.247 (1.6)). The chart is the right translation by \(e^{i\mathbf H_b}\), which is \(V_{k+1}\)-measurable. The Jacobian cancels the change of the Haar density exactly; [RD]'s check (1) reproduces this.
* **(A8) chart.** It is the right translation by \(e^{i\mathbb H^{(j)}_Z}\). \(U^{(n+1)}_k\) is the background *after* the \((n+1)\)st integration, since its determining set already carries level-\((j+1)\) data on the integrated region ((1.16)). So it does not depend on the integrated \(V_j\), and the chart is Haar-preserving by the same argument.
* **Cutoff.** The source's cutoff \(g\) (p.252) is identity below \(\frac43g_0^{-1}\delta_0\) and 1 above \(\frac53\delta_0\). Its role was to keep the R-test unchanged while localizing the Q-test. With the R-test already local, it is unnecessary, as [RD] says.

## 7. Exactness, positivity, normalization (B-01's content)

* (3.16\(^{\rm loc}\)) and (A8) are partitions of unity by indicator functions: every configuration has exactly one label pattern.
* The charts are bijective, Haar-preserving reparametrizations by elements measurable with respect to the non-integrated variables (§6).
* The extension \(\hat{\mathbf H}_b\) does not change any value on real configurations (Lemma 3.1). (A8′) only re-books terms.
* The R-operation's kernels (1.100)–(1.101) and its normalization (1.102) ([IV] p.201, source) are unchanged.

So each operation is still an exact identity, or an equivalence with equal integrals, for the same Wilson measure. Every term of the expansion is a nonnegative product of characteristic functions and densities. Positivity and normalization are preserved.

## 8. partitions and parameter conditions

**(Par-c).** Nested cube partitions with common symmetry planes are the source's own assumption ("compatible with all the other partitions", [III] pp.257, 265, source). B-02's choice realizes them:

* odd \(L\ge13\);
* \(M_1\) an \(L\)-power, \(M_2=L^2M_1\), \(M=L^u\);
* \(R_j\) a power of \(L\) by (2.5).

Nesting \(\pi'\subset MR\)-partition needs \(LM_2\mid M\), i.e. \(u\) large. Common centre planes need odd \(L\).

**(Par-M)** \(M\ge(L+8)M_2\) holds for \(u\) large. Lemma 2.1's \(L\ge5\) holds.

**Ceilings and their order.** The conditions to add are:

| Condition | Where it comes from | Type |
|---|---|---|
| \(\frac12\kappa_1\ge c'\kappa\), \(\kappa_1\le\kappa_{\max}\) (\(/L\) if scale-\(k\) tiles) | E4, §1.5 | \(M\) large |
| \(\lVert B_b\rVert,\lVert B_Z\rVert<c_S\hat B^{-6}\) | M♯ datum ball, §1.3 | \(g\) ceiling |
| \(\alpha_J\hat B^{10}\le c_S\) | Source operators for the deformed reconstruction | \(g\) ceiling |
| (Par-g) | [RD] (A9) | \(g\) ceiling |
| (Par-g′) | if (CD-T) is used | \(g\) ceiling |
| (A8′)'s \(e^{-cR_j}\ll C_0\) | §5.2 | \(g\) ceiling |
| [P2] (2.59), the collar estimate item 4, for the layers of \(\mathbb B_b\) and \(\mathbb B(Z)\) | layers one \(M_1\)-block thick per scale | \(\delta_0M_1\) large, with \(M_1\) free in the source (p.245) additional assumption |

All of them fit the order \(d,L\to\kappa\to\kappa_1\to M_1<M_2<M\to C_0,C_1\to g\) of the representation convention/the collar estimate. deduction for the arithmetic.

**B-02 (E2).** These are ceilings "in the actual statements", so B-02 must re-verify them. B-02's witness has \(g_{K_n}\to0\), so finitely many initial terms can be discarded. (d) until that check is done.

## 9. The amended construction, final form

[RD]'s (A1)–(A10) stand, with these changes:

* **(A5′)** Tube localization (Lemma 3.4 with the proof of §1.4) applies to the terms born from \(\mathscr V\) in the T-step **and** to the terms born from the (A8) chart in passing components of the R-operation preparatory steps (§5.2). It uses one uniform tile scale per determining-set problem (E4).
* **(A8)** is unchanged as a label rule. The threshold is written \(\delta'_j/g_j\) under the representation convention's convention (E6).
* **(A9)** adds:
  * the \(\kappa_1\) window;
  * the M♯ datum ceiling for \(\mathbb B_b\) and \(\mathbb B^{(n+1)}_k(Z)\);
  * (A8′)'s ceiling;
  * odd \(L\) with \(L\)-power constants for (Par-c) with common centre planes;
  * [P2] (2.59) for \(M_1\)-thick layers.
* **(A10)** adds B-02 (§11).
