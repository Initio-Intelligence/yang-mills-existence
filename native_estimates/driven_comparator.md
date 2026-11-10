# Variation of the even Gaussian comparator

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 1. Objects

### 1.1 Conventions

- \(Y_k=g_k^{-2}\), \(\ell_k=\log Y_k\). The CMP119 cutoff has canonical radius \(P_k=A_1\ell_k^{p_0}\) (\(p_0>1\)) and physical radius \(\delta_k=g_kP_k\) (the native-domain comparison §1.1; CMP119 (2.4)).
- **Reading of CMP119 (3.16)** (p.268). The display is \(\chi(\sup_{b}|A_k(b)|<\delta_k)\), while \(A_k\) is the canonical fluctuation (the same page writes \(\exp i[g_kCA_k-h\tilde D(g_kCA_k)]\)). As in the supplementary constant-flux calculation §1 item 3 and the L2 note §5 (S-cut), The interpretation of the canonical radius is \(\delta_k/g_k=P_k\). This reading is **needed** for (C2): under the literal reading the canonical radius tends to zero, and the \(s=0\) term below would not be the Gaussian. See (S6).
- **Fixed chart.** \(\mathbf U^c_j(X,\alpha_0,\alpha_1)\) with CMP109's *absolute* constants \(\alpha_0,\alpha_1\) (CMP109 p.263, (1.11)–(1.18)). The norm is \(\|F\|_{\rm fix}=\sup_X\sup_{\mathbf U^c_j(X,\alpha_0,\alpha_1)}|F(X)|e^{\kappa d_j(X)}\).
- **Readout.** \(\mathcal P\) is the Wilson coefficient of CMP109 (1.20)–(1.22) (page-checked p.264), in \(Y\) units:
\[
\mathcal PF=-\Big(\tfrac{\partial^2}{\partial p_\mu\partial p_\nu}\tilde\Pi_{\mu\nu}\Big)(0)=\sum_x\Pi_{\mu\nu}(x)x_\mu x_\nu ,\qquad\mu\ne\nu,
\]
where \(\Pi\) is the infinite-volume second derivative at the flat coarse field of the whole-lattice sum. It is linear, and \(\mathcal PA=1\). The normalisation \(\mathcal PA=1\) is forced by the cancellation of CMP109 (4.38)–(4.42) against (5.42) (pp.291 and 297; displays not independently verified).

### 1.2 The single step (CMP109 §2)

The following is page-checked on CMP109 pp.265–268. Given an action of the inductive form
\[
A_k=-\frac1{g^2}A(U_k)+\mathbf E_k,\qquad
\mathbf E_k=\sum_{j\le k}\big[H_j(U_k)-H_j(1)-(\mathcal PH_j)\,A(U_k)\big]
\tag{1.1}
\]
(CMP109 (0.22)–(0.23) and (1.6), with each birth \(H_j\) carrying its own projection; Gaussian normalisers included in the births as on p.261), the transformation (2.1) is
\[
\log\mathbf N_k^{-1}\!\int dV\,\delta(\bar VW^{-1})\,\chi_k\exp\Big[-\frac1{g^2}\mathbf G(V)-\frac1{g^2}A(U_k(V))+\mathbf E_k(U_k(V))\Big].
\]
**The gauge-fixing coefficient is the same \(1/g^2\) as the Wilson coefficient** (p.265, source).

After the change of variables (2.3)–(2.11), the result (2.12) is
\[
-\frac1{g^2}A(U_{k+1})+\mathbf E_k(U_{k+1})+\big[\log Z^{(k)}(U_{k+1})-\log Z^{(k)}(1)\big]+\log\mathbf N_k''^{-1}\!\int d\mu_{C^{(k)}}(B)\chi_k\exp\big[\mathbf P^{(k)}(g,U_{k+1},B)+\{\cdots\}\big].
\tag{1.2}
\]
Here \(\{\cdots\}=\mathbf E_k(U_k(\exp i[gCB-h\tilde D(gCB)]V^{(k)}))-\mathbf E_k(U_k(V^{(k)}))\). The function \(\mathbf P^{(k)}\) collects the Jacobian \(\mathrm{Tr}\log(I-h\frac{\delta}{\delta B}\tilde D)(gCB)\), \(\log\sigma(gCB-h\tilde D(gCB))\), \(g^{-2}\langle H_1h\tilde D_3(gCB),J\rangle\), \(-g^{-2}\mathbf G_3(gB)\), the two \(g^{-2}\langle H_1\cdot,\Delta_1H_1\cdot\rangle\) terms with \(h\tilde D(gCB)\), and \(-g^{-2}V(H_1(gCB-h\tilde D(gCB)))\).

- **Cutoff.** By (2.9) (p.266, source), \(\chi_k=\prod_{b\in T^{(k)}\setminus\{b_0(c)\}}\chi(|B'(b)|<\varepsilon_1)\). It is a product over the **independent** bonds only; on these \(B'=gB\) after the change of variables.
- **The new birth.** It is (2.13), \(\mathbf E^{(k+1)}(g,\cdot)=\log\int d\mu\chi_k e^{\mathbf P+\{\cdots\}}\), together with the Gaussian bracket in (1.2).
- **The coupling.** It is renormalised only afterwards, by (2.15), \(1/g_k^2=1/g_{k+1}^2+\beta_{k+1}(g_k)\). The text after (2.15) says that (2.12)–(2.15) "imply that the action \(A_{k+1}\) is given by (1.3) with \(k+1\) instead of \(k\)".

### 1.3 The driven fixed-chart comparator \(\mathfrak B^{\rm fix}[Y_0,\dots,Y_n]\)

**Definition.** Let \((Y_0,\dots,Y_n)\) be any real array with \(Y_k>0\), and \(g_k=Y_k^{-1/2}\).

- Start from the bare Wilson density \(\exp(-Y_0A)\), as in CMP119 Theorem 1.
- At step \(k\), given births \(H^{\rm fix}_1,\dots,H^{\rm fix}_k\) (localised families on the absolute domains) and their projections \(p_j=\mathcal PH^{\rm fix}_j\), form the action (1.1) with \(g=g_k\) and \(H_j=H^{\rm fix}_j\).
- Apply the single step of §1.2 with \(g=g_k\), with \(\chi_k\) replaced by the CMP119 product cutoff of canonical radius \(P_k\) on the independent bonds, and with the CMP116 localisation. The output birth \(H^{\rm fix}_{k+1}\) is the Gaussian bracket of (1.2) plus (2.13).
- Set \(p^{\rm fix}_{k+1}:=\mathcal PH^{\rm fix}_{k+1}\). The action at step \(k+1\) is (1.1) with \(g=g_{k+1}\) **prescribed**.

Equivalently, on the whole lattice,
\[
\mathbf T_{g_k}A^{\rm fix}_k=A^{\rm fix}_{k+1}+\big(Y_{k+1}-Y_k+p^{\rm fix}_{k+1}\big)A(U_{k+1}).
\]
This is the pure small-field recursion of CMP109 with (2.15) replaced by the prescribed array, i.e. with a Wilson counterterm inserted after each step. That is the description in the native-domain comparison (P22.5) and in [Reset remainders](../coupling/reset_remainders.md) §4 ("\(z=0\)").

**Remark (no hidden mismatch).** The comparator's step-\(k\) integrand contains \(g_k\) in exactly three places: the Wilson coefficient, the gauge-fixing coefficient (both \(1/g_k^2\), by (2.1)), and the cutoff \(P_k\). The *actual* recursion at step \(k\) has the same three. The self-consistent comparator of the supplementary constant-flux calculation (12)–(13) needed a gauge mismatch \(t_iG\) and a shifted cutoff \(\delta_i/\tilde g_i\). Neither exists here.

### 1.4 The amplitude family

Fix \(k\), the torus \(\Lambda\), the inherited births, and the canonical cutoff domain
\[
D=D_k:=\prod_{b\ \text{independent}}\{B_b\in\mathfrak g:\ |B_b|<P_k\}
\tag{1.3}
\]
(a product of convex balls, by (2.9) and (S6)). The coarse background is \(W_u=\exp(iu)\) at scale \(k+1\), with \(u\) real near \(0\). For real \(s\) with \(|s|\le g_k\) put
\[
Z_\Lambda(s,u):=\int_D e^{-H_{s,u}(B)}\,dB,\qquad H_{s,u}(B):=\tfrac12\langle B,M(u)B\rangle-V_s(u,B),
\tag{1.4}
\]
where:

- \(\frac12\langle B,M(u)B\rangle\) is the Gaussian form of (2.11), \(M(u)=C^*\Delta^{(k)}C\) at the background \(U_{k+1}(W_u)\). It is independent of \(g\).
- \(V_s(u,B)\) is \(\mathbf P^{(k)}+\{\cdots\}\) of (1.2) with **every occurrence of \(g\) replaced by \(s\)**: \(gCB\to sCB\) and \(g^{-2}\to s^{-2}\). The cutoff \(D\) and the inherited \(\mathbf E_k\) are frozen.

By (2.14), \(V_0\equiv0\) (the exponent "vanishes at \(g_k=0\)", p.268), interpreted by continuity. With \(Z^{(k)}(U)\) the normaliser of \(d\mu_{C^{(k)}}\) (CMP109 (1.4)), the whole-lattice sum of the comparator birth at step \(k\) is
\[
\sum_XH^{\rm fix}_{k+1}(X)(U_{k+1}(W_u))=\log Z_\Lambda(g_k,u)-\log Z_\Lambda(g_k,u_{\rm vac})+(\text{constants}),
\tag{1.5}
\]
by (1.2) and (2.13)–(2.14). Define the finite-volume readouts
\[
p_\Lambda(s):=\mathcal P_\Lambda\log Z_\Lambda(s,\cdot),\qquad d^G_{k,\Lambda}:=\mathcal P_\Lambda\log Z^{(k)}(U_{k+1}(W_\cdot)),
\]
where \(\mathcal P_\Lambda F=\sum_{x\in\Lambda,\,|x|_\infty<\frac12{\rm side}}x_\mu x_\nu\,\partial_{u_{x,\mu}}\partial_{u_{0,\nu}}F|_{u=0}\). Finally
\[
d^G_k:=\lim_\Lambda d^G_{k,\Lambda}=\mathcal P\log Z^{(k)}.
\]
This is the uncut, stationary Gaussian decrement of step \(k\). It is **independent of the array**, since \(M(u)\) and \(Z^{(k)}\) contain no coupling ((2.11), p.267).

## 2. Statement

### 2.1 Theorem

> **Theorem 2.1 (C2 for an exogenous array).** Assume (S1)–(S7) below. There are \(Y_\sharp\) and \(C_\sharp\), depending only on the source constants (\(L,M,\kappa,\kappa_1,\beta,\varepsilon_0,\alpha_0,\alpha_1,E_0,\gamma\) of CMP109/116, the cutoff constants \(A_1,p_0\), and the constants of (S2)–(S7)), such that for every \(n\) and every real array \((Y_0,\dots,Y_n)\) with \(Y_k\ge Y_\sharp\) for all \(k\le n\):
> 1. \(\mathfrak B^{\rm fix}[Y_0,\dots,Y_n]\) is defined through step \(n\). Each \(H^{\rm fix}_j\) satisfies CMP109 (1.18) with the constant \(E_0\) on \(\mathbf U^c_j(X,\alpha_0,\alpha_1)\), together with gauge invariance (1.19) and Euclidean covariance.
> 2. For every \(k\le n\),
> \[
> |p^{\rm fix}_{k+1}-d^G_k|\ \le\ \tfrac12C_K'\,g_k^2+C_{\rm def}\,e^{-\gamma_2A_1^2\ell_k^{2p_0}/20}\ \le\ \frac{C_\sharp}{Y_k},
> \tag{2.1}
> \]
> with \(C_K'\) from Proposition 4.6 and \(C_{\rm def}\) from Lemma 4.7.
> 3. \(C_\sharp\), \(C_K'\), \(C_{\rm def}\) and \(Y_\sharp\) do not depend on \(n\), \(k\), the torus or the array. \(Y_\sharp\) is the maximum of the finitely many thresholds (T1)–(T5) of §4.8, each a condition on \(g_k\) alone.

### 2.2 Inputs (each single-step and array-free)

| Label | Content | Source | Status |
|---|---|---|---|
| (S1) | **Single-step regeneration on the fixed chart.** If (1.1) holds with births satisfying (1.18)–(1.19) and Euclidean covariance, and \(0<g\le\gamma\), then the output birth of §1.2 satisfies the same, with the same \(E_0\). This holds also with \(\chi_k\) replaced by the product cutoff of canonical radius \(P\), whenever \(\gamma_2P^2\ge\Pi_*\) and \(gP\le\varepsilon_{\rm fix}/4\). | CMP109 p.265 ("we assume that after \(k\) steps we have obtained the action \(A_k\) described in the previous section"), p.268 ("the proof of Theorem 3 is reduced to proving the remaining properties of (2.13)"); §§3–5; CMP116 §§1–2 and p.21 (closing inequality); CMP119 p.262, second remark (single step as a map between inductive spaces). Cutoff replacement: CMP116 (2.31)–(2.34) repeated for \(P\) in [the homogeneous projection](../coupling/homogeneous_projection.md) §20.2 | source input for the source single step (pp.264–268); conditional for the cutoff replacement (the comparison argument, printed pages) |
| (S2) | **Localised inherited difference.** CMP116 Lemma 1, (1.33)–(1.36): for any trial radius \(\varepsilon\le\varepsilon_{\rm fix}\), \(\{\cdots\}=\sum_{Y\in\mathbf D_k}\mathbf V'_k(Y,U_{k+1},B)\), with \(\mathbf V'_k(Y,\mathbf U,\mathbf J,B)\) analytic on \(\mathbf U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\times\{|B|<\varepsilon g^{-1}\text{ on }Y\}\) and \(|\mathbf V'_k|\le E_0\varepsilon C_1M^qe^{C_2\kappa_1}e^{-(1-2\delta)\kappa d_k(Y)}\), with **absolute** \(C_1,C_2,q\) | CMP116 p.9 | source input, page-checked |
| (S3) | **Localised explicit terms.** CMP116 (1.37)–(1.43) (Lemma 2): \(\mathbf P^{(k)}=\sum_Y[\frac12\langle Q(Y,B)B,B\rangle+\mathbf V''(Y,B)]\). Every piece is a function of the physical insertion \(B'=gCB-h\tilde D(gCB)\), analytic on a fixed ball \(e^{16\kappa_1}|B'|\le a_1\) and in \((\mathbf U,\mathbf J)\) on the absolute domain, with the stated vanishing orders (\(V\), \(\mathbf G_3\), \(\tilde D_3\) cubic) and exponential localisation | CMP116 pp.10–11 | (c) (p.10 page-checked) |
| (S4) | **Flat Gaussian and tangents.** (i) \(M(0)\ge\gamma_0\), with \(\gamma_0\) independent of \(k\) (CMP95 Prop. 1.1, (1.90), and \(\|CB\|\ge\|B\|\)). (ii) \(\lvert M(0)_{bb'}\rvert\le C_Me^{-\nu d(b,b')}\), and the \(u\)-derivatives of \(M\) at \(0\) up to order two have kernels decaying exponentially away from the derivative sites (CMP95 Prop. 1.2; CMP99 Th. 3.3). (iii) The minimiser tangents \(\partial_{u_x}U_{k+1}\) and \(\partial_{u_x}\partial_{u_y}U_{k+1}\) at flat decay exponentially from \(x\) (and \(y\)) in scale-\((k+1)\) units (CMP102 Prop. 9, (190)). All constants depend only on \(d,L\) | the native estimate §18.2, §21.3; the supplementary constant-flux calculation §2 last paragraph | source input for (i) (CMP95 p.33); text-level for (ii), (iii) |
| (S5) | **HC-W and raw moments.** For \(\mu\propto\mathbf 1_De^{-H}\), \(D\) a finite product of bounded convex bodies containing \(0\), \(H\in C^3\) near \(\bar D\), and block-scalar \(W\) with \(\mathrm{Sym}(WH''W^{-1})\ge\lambda\): (HC5) \(\lvert\mathrm{Cov}_\mu(f,g)\rvert\le\lambda^{-1}\|W\nabla f\|_{L^2(\mu)}\|W^{-1}\nabla g\|_{L^2(\mu)}\); and, for \(0<w_b\le1\), \(\big\||WB|\big\|_{L^p(\mu)}\le\|W\nabla H(0)\|/\lambda+\sqrt{(\mathrm{tr}W^2+p-2)/\lambda}\) | [the homogeneous projection](../coupling/homogeneous_projection.md) §20.1 (elliptic proof), §22.1 (integration by parts) | conditional, proved there; see also §4.4, remark |
| (S6) | **Cutoff structure.** The CMP119 step integral in the whole-lattice regular sector uses the product cutoff (1.3) on independent bonds with canonical radius \(P_k=\delta_k/g_k=A_1\ell_k^{p_0}\) | CMP109 (2.9) (page-checked: product over \(T^{(k)}\setminus\{b_0(c)\}\)); CMP119 (3.16) (page-checked, read with \(\delta_k/g_k\)) | (c) plus the convention of §1.1 |
| (S7) | **Defect expansion.** Lemma L2 of the companion note at \(v=0\), \(Q=0\): \(\log\mu_{C^{(k)}(U)}(D)=\sum_X\mathfrak E(X)[0]\), with \(\mathfrak E(X)[0]\) analytic on \(\mathbf U^c_{k+1}(X,\alpha_0,\alpha_1)\) and \(\lvert\mathfrak E(X)[0]\rvert\le c_3\cdot2(L+2)^4c_1e^{-\gamma_2P_k^2/20}e^{-\kappa d_{k+1}(X)}\) | Holomorphic dependence of the fluctuation potential Lemma L2 (choose \(a\) with \(\varepsilon_2(a)=e^{-\gamma_2P^2/20}\); (A0) is void at \(Q=0\)) | conditional |

None of (S1)–(S7) refers to any coupling other than the current \(g_k\) (§3).

### 2.3 Corollary (transfer to the analysis comparator)

> **Corollary 2.2.** Assume in addition the analysis Theorem A′ inputs at steps \(\le k\): (F1), (F2), (L1\(^*\)), (R\(^*\)), Lemma L2, and the **real** part of (D\(^*\)). The real part of (D\(^*\)) says: for real backgrounds in the real native domain at scale \(i+1\) and real fluctuations in \(D_i\), all composite configurations at older scales \(j\le i\) lie in the real native domains \(\mathbf U_j\). Let \(\mathsf H'_j:=\sum_X(\mathbf E^{(j)}-\delta H_j)(X)\) be the whole-lattice sums of the analysis comparator (analysis §6 and §9.3). Then for every admitted \(k\),
> \[
> \mathcal P\mathsf H'_{k+1}=p^{\rm fix}_{k+1}[Y_0,\dots,Y_k],
> \]
> and hence (C2\(^*\)) holds with \(C_p=C_\sharp\) whenever \(Y_*\ge Y_\sharp\).

**What the actual \(Y_k\) must satisfy.** For (C2): only \(Y_k\ge Y_\sharp\) at steps \(k<K\). This is automatic from the definition of \(K\) once \(Y_*\ge Y_\sharp\). For the transfer: the actual trajectory's own admission, which Theorem C′ already establishes inductively from the prefix numerics (the native-domain comparison Lemma 3.4, analysis §8.1). No further condition is created by (C2).

## 4. Proofs

Throughout, "constant" means a number depending only on the data listed in Theorem 2.1. The threshold conditions (T1)–(T5) are collected in §4.8.

### 4.1 Lemma 4.1 (the driven comparator is well defined; array enters only via \(g_k\))

*Statement.* Under (S1), (S6) and (T1)–(T3), for every array with \(Y_k\ge Y_\sharp\):

- \(\mathfrak B^{\rm fix}\) is defined through step \(n\);
- each \(H^{\rm fix}_j\) satisfies (1.18)–(1.19) and Euclidean covariance with the constant \(E_0\);
- the step-\(k\) output is a function of \((H^{\rm fix}_j)_{j\le k}\) and \(g_k\) alone.

*Proof.* Induction on \(k\).

1. **Step \(0\).** At \(k=0\) there are no inherited births.
2. **Inductive hypothesis.** Suppose \(H^{\rm fix}_1,\dots,H^{\rm fix}_k\) satisfy (1.18)–(1.19) and covariance. Then (1.1) with \(g=g_k\) is an action of the inductive form of CMP109 §1:
   - the inherited part is \(\sum_j[H_j-H_j(1)-(\mathcal PH_j)A]\), with each birth's own \(\beta\) by (1.20)–(1.22);
   - the Wilson coefficient is \(1/g_k^2\);
   - the Gaussian normalisers are inside the births (p.261).

   No relation \(1/g_k^2=1/g_0^2-\sum_j\beta_j\) is part of the inductive assumptions (1.1)–(1.22). The formula gives the list on pp.260–264: it consists of the form (1.3)/(1.6), the representation (1.7), the domains (1.11)–(1.16), the bound (1.18), gauge invariance (1.19), Euclidean invariance, and the definition (1.20)–(1.22).
3. **One step.** With \(g_k\le\gamma\) (T1), (S1) applies (with the cutoff of radius \(P_k\) under (T2)–(T3)). The output \(H^{\rm fix}_{k+1}\) has the stated properties.
4. **Where couplings appear in the step.** By §1.2, the step uses \(g_k\) in exactly the Wilson coefficient, the gauge-fixing coefficient, the scaling and the cutoff. The inherited births enter only through \(\{\cdots\}\), as fixed functions on absolute domains.
5. **Next action.** Replacing \(1/g_k^2\) by \(1/g_{k+1}^2\) in (1.1) at the next step produces again an action of the inductive form, with \(g_{k+1}\le\gamma\). \(\square\)

### 4.2 Lemma 4.2 (exact evenness)

*Statement.* On every torus, \(Z_\Lambda(-s,u)=Z_\Lambda(s,u)\) for \(|s|\le g_k\) and real \(u\). Hence \(\partial_s\log Z_\Lambda(0,u)=0\) and \(p'_\Lambda(0)=0\).

*Proof.* Every term of \(V_s(u,B)\) in (1.2) is of the form \(F(sCB)\) or \(s^{-2}F(sCB)\), with \(F\) depending also on \(u\) through the background.

- The Jacobian, \(\log\sigma\) and \(\{\cdots\}\) are of the first form.
- \(V(H_1\cdot)\), \(\mathbf G_3\), the \(\tilde D_3\)-term with \(J\) and the two \(\Delta_1\)-terms are of the second form.

Hence \(V_{-s}(u,-B)=V_s(u,B)\). The Gaussian form is even in \(B\). The domain \(D\) of (1.3) is symmetric under \(B\mapsto-B\), and it does not depend on \(s\) because the canonical radius is frozen. Substitute \(B\mapsto-B\). \(\square\)

(the finite-cutoff construction statement "\(Z(-\tau,u)=Z(\tau,u)\)" is thus exact. It needs the frozen canonical cutoff, which is the reason for freezing it.)

### 4.3 Lemma 4.3 (cumulant splitting identity)

*Statement.* Let \(X_1,\dots,X_n\) be random variables with finite moments, \(m(A)=\mathbb E\prod_{i\in A}X_i\), \(m(\emptyset)=1\). Let \(\{1,\dots,n\}=I\sqcup J\) with \(I,J\ne\emptyset\), and put \(\tilde m(A)=m(A\cap I)\,m(A\cap J)\). Then
\[
\kappa_n(X_1,\dots,X_n)=\sum_\pi c_\pi\Big[\prod_{A\in\pi}m(A)-\prod_{A\in\pi}\tilde m(A)\Big],\qquad c_\pi=(-1)^{|\pi|-1}(|\pi|-1)!,
\]
and \(m(A)-\tilde m(A)=\mathrm{Cov}\big(\prod_{A\cap I}X_i,\prod_{A\cap J}X_j\big)\). This vanishes unless \(A\) meets both \(I\) and \(J\). Consequently
\[
|\kappa_n|\le C_n\max_{A:\,A\cap I\ne\emptyset\ne A\cap J}\Big|\mathrm{Cov}\Big(\prod_{A\cap I}X_i,\prod_{A\cap J}X_j\Big)\Big|\cdot\max_{\pi,\ \text{sub-products}}\prod\big(|m(\cdot)|+|\tilde m(\cdot)|\big).
\]

*Proof.* \(\tilde m\) are the joint moments of \((X_i)_{i\in I}\) and an independent copy \((X'_j)_{j\in J}\) of \((X_j)_{j\in J}\). A joint cumulant of two mutually independent groups vanishes, so \(\kappa_n[\tilde m]=0\). Subtract this from the moment–cumulant formula for \(\kappa_n[m]\). Expand the difference of products by telescoping, \(\prod a_l-\prod b_l=\sum_l(\prod_{l'<l}b_{l'})(a_l-b_l)(\prod_{l'>l}a_{l'})\). \(\square\) (Checked numerically, §9 (1).)

### 4.4 Lemma 4.4 (tree decay of cumulants under a weighted-convex law)

*Setting.* Let \(\Lambda\) be a finite torus, \(\mathcal B\) its independent bonds with lattice distance \(d\), and \(D=\prod_{b}D_b\) with \(D_b\) a ball centred at \(0\). Let \(\mu\propto\mathbf 1_De^{-H}\) with \(H\) real-analytic on \(N=\prod_b\{|B_b|<2P\}\), and assume:

- (i) \(H''\ge m>0\) on \(N\);
- (ii) \(|H''_{bb'}|\le C_He^{-\nu d(b,b')}\) on \(N\);
- (iii) \(\nabla H(0)=0\).

Let \(\alpha\le\alpha_*:=\min\{\nu/2,\ m/(4C_H\Sigma_\nu)\}\), where \(\Sigma_\nu:=\sup_b\sum_{b'}d(b,b')e^{-(\nu/2)d(b,b')}\), and put \(\lambda=m/2\).

*Statement.* Let \(F_1,\dots,F_r\) (\(r\le4\)) be \(C^1\) functions on \(N\), with \(F_i\) depending only on \(B|_{Y_i}\) (\(Y_i\subset\mathcal B\) finite) and
\[
|F_i(B)|+|\nabla F_i(B)|\le K_i(1+|B|_{Y_i})^{m_0},\qquad |B|_Y:=\max_{b\in Y}|B_b|.
\]
Let \(\ell=\ell(Y_1,\dots,Y_r)\) be the length of a minimal spanning tree of the complete graph on \(\{1,\dots,r\}\) with edge lengths \(d(Y_i,Y_j)\). Then
\[
|\kappa_r(F_1,\dots,F_r)|\le C\prod_{i}K_i(1+|Y_i|)^{m_0+1}\,e^{-\alpha\ell/(r-1)}\quad(r\ge2),\qquad|\mathbb E F_1|\le CK_1(1+|Y_1|)^{m_0},
\]
with \(C\) depending only on \(r,m_0,m,\alpha\).

*Proof.*

1. **Weighted gap.** For any \(S\subset\mathcal B\), let \(W^S=\mathrm{diag}(e^{\alpha d(b,S)})\), a block-scalar weight. Since \(|d(b,S)-d(b',S)|\le d(b,b')\),
\[
\|W^SH''(W^S)^{-1}-H''\|\le\sup_b\sum_{b'}C_He^{-\nu d}(e^{\alpha d}-1)\le C_H\alpha\Sigma_\nu\le m/4
\]
by Schur's test. So \(\mathrm{Sym}(W^SH''(W^S)^{-1})\ge m/2=\lambda\) on \(N\). Thus (S5) (HC5) applies with every such weight.
2. **Moments.** Apply the raw-moment bound of (S5) with \(W_{b'}=e^{-\alpha d(b',b)}\) (\(\le1\); \(\mathrm{tr}W^2\le C_\alpha\); \(\nabla H(0)=0\)). It gives \(\|B_b\|_{L^p(\mu)}\le C_{p}\), uniformly in \(b\) and \(\Lambda\). Hence \(\|(1+|B|_Y)^{q}\|_{L^p}\le(1+|Y|C_{pq})^{q}\), and every \(|m(\cdot)|\), \(|\tilde m(\cdot)|\) in Lemma 4.3 is bounded by \(C\prod K_i(1+|Y_i|)^{m_0}\).
3. **Splitting.** Choose the split \(I\sqcup J\) obtained by deleting the longest edge \(e\) of a minimal spanning tree. By the cut property of minimal spanning trees, \(d(\bigcup_IY_i,\bigcup_JY_j)=|e|\ge\ell/(r-1)\). For \(A\) meeting both sides put \(\Phi=\prod_{A\cap I}F_i\), \(\Psi=\prod_{A\cap J}F_j\), and \(S=\bigcup_{A\cap I}Y_i\). Then \(\nabla\Phi\) is supported in \(S\), so \(W^S\nabla\Phi=\nabla\Phi\). Also \(\nabla\Psi\) is supported in \(\bigcup_{A\cap J}Y_j\), at distance \(\ge|e|\) from \(S\), so \(|(W^S)^{-1}\nabla\Psi|\le e^{-\alpha|e|}|\nabla\Psi|\).
4. **Covariance bound.** By (HC5) and Hölder with step 2,
\[
|\mathrm{Cov}(\Phi,\Psi)|\le\lambda^{-1}e^{-\alpha|e|}\,C\prod_iK_i(1+|Y_i|)^{m_0+1}.
\]
Lemma 4.3 finishes the proof. \(\square\)

*Moment conditions (S5).*

- The raw-moment proof is complete as written. The boundary term has the right sign because \(D_b\) is convex and contains \(0\).
- The HC-W proof (Neumann problem, Bochner identity with block-pure normals, even reflection at corners) is standard elliptic theory and There is no identified gap.
- An independent route, not written in full here: replace \(\mathbf 1_D\) by \(e^{-n\varphi}\), \(\varphi=\sum_b(|B_b|-P)_+^4\), which is block-separable and convex. Then \(\mathrm{Sym}(W(H+n\varphi)''W^{-1})\ge\lambda\) for block-scalar \(W\) (after extending \(H\) outside \(N\) with Hessian bounded below by \(\lambda\)). The Helffer–Sjöstrand representation on \(\mathbb R^n\) gives (HC5) for the regularised law, and \(n\to\infty\) gives it for \(\mu\).

conditional either way.

### 4.5 Lemma 4.5 (local polynomial bounds on the insertions)

Labels: \(\mathsf s\) denotes an \(s\)-derivative, and \(\mathsf x,\mathsf 0\) denote \(\partial_{u_{x,\mu}},\partial_{u_{0,\nu}}\). For a sub-multiset \(\beta\subset\{\mathsf s,\mathsf s,\mathsf x,\mathsf 0\}\), let \(\mathcal F^\beta:=-\partial^\beta H_{s,u}|_{u=0}\).

*Statement.* Assume (S2)–(S4) and (T2)–(T4). For \(|s|\le g_k\), each \(\mathcal F^\beta\) is a finite sum \(\sum_Y F^\beta_Y\) over finite bond sets \(Y\). Each \(F^\beta_Y\) depends only on \(B|_Y\) and satisfies on \(N\)
\[
|F^\beta_Y(B)|+|\nabla F^\beta_Y(B)|\le K_*\,(1+|B|_Y)^{4}\,e^{-c_*d(Y)}\,e^{-c_*d(Y,a(\beta))},
\tag{4.1}
\]
where:

- \(d(Y)\) is the tree size of \(Y\);
- \(a(\beta)\) is the set of anchors among \(\{x,0\}\) present in \(\beta\), with \(d(Y,\emptyset)=0\) and \(d(Y,\{x,0\})=d(Y,x)+d(Y,0)\);
- \(K_*,c_*\) are constants.

The Hessian \((V_s)''\) satisfies \(|(V_s)''_{bb'}|\le C_V(\delta_k+g_k^2)e^{-c_*d(b,b')}\) on \(N\), and \(\nabla_BV_s(0,0)=0\).

*Proof.*

1. **Gaussian part** (only for \(\beta\subset\{\mathsf x,\mathsf 0\}\), since it is \(s\)-independent). It contributes \(-\frac12\langle B,\partial^\beta M(0)B\rangle\). Use pieces \(Y=\{b,b'\}\) and (S4)(ii).
2. **The inherited part.** By (S2) with trial radius \(\varepsilon_{\rm fix}\), \(\{\cdots\}_s=\sum_Y f_Y(\mathbf U,\mathbf J;sB)\). Here \(f_Y(\cdot;b):=\mathbf V'_k(Y,\cdot,b/g_k)\) is analytic in the physical variable \(b\) for \(|b|_Y<\varepsilon_{\rm fix}\), with \(|f_Y|\le K_Ee^{-\kappa_*d(Y)}\), \(K_E=E_0\varepsilon_{\rm fix}C_1M^qe^{C_2\kappa_1}\), \(\kappa_*=(1-2\delta)\kappa\).
   - On \(N\), \(|sB|_Y\le2\delta_k\le\varepsilon_{\rm fix}/2\) by (T2).
   - Apply Cauchy to \(\lambda\mapsto f_Y(sB+\lambda\hat B)\) with \(\hat B=B/|B|_Y\) on the disc of radius \(\varepsilon_{\rm fix}/2\). This gives \(|\partial_s^jf_Y(sB)|\le j!K_E(2|B|_Y/\varepsilon_{\rm fix})^je^{-\kappa_*d(Y)}\), and similar bounds for one \(B\)-gradient.
   - The \(u\)-derivatives act through \((\mathbf U,\mathbf J)=(U_{k+1},J_{k+1})(W_u)\). The chain rule uses (S4)(iii) tangents. Cauchy in \((\mathbf U,\mathbf J)\) on the \((1+\beta)\)-enlarged absolute domain gives a fixed factor. The tangent decay gives \(e^{-c\,d(Y,x)}\), as in the supplementary constant-flux calculation §2, last paragraph.
3. **The explicit part.** By (S3), each piece of \(\mathbf P^{(k)}\) with \(g\to s\) is \(\phi_Y(sB)\) or \(s^{-2}\phi_Y(sB)\), with \(\phi_Y\) analytic on a fixed physical ball, of the stated vanishing order, and localised.
   - For \(s^{-2}\phi(sB)\) with \(\phi=\sum_{n\ge3}\phi_n\): \(s^{-2}\phi(sB)=\sum_{n\ge3}s^{n-2}\phi_n(B)\), so \(|\partial_s(\cdot)|\le C|B|^3\) and \(|\partial_s^2(\cdot)|\le C|B|^4\). This is the native estimate §20.3, row (J16), checked there symbol by symbol.
   - The remaining pieces are handled the same way.
   - Degree \(\le4\) results; the \(B\)-gradient is of degree \(\le3\).
4. **Hessian.** The \(s^{-2}\phi(sB)\) pieces have \(\partial_B^2\) of size \(O(|sB|)=O(\delta_k)\). The \(\phi(sB)\) pieces have size \(O(s^2)\). The inherited part has \(s^2K_E(2/\varepsilon_{\rm fix})^2\).
5. **Vanishing gradient.** \(\nabla_BV_s(0,0)=0\): the explicit pieces vanish to second order at \(B=0\) (the linear term is absent from (2.12), by (2.10)–(2.11)). The inherited part's gradient at \(B=0\) is \(s\) times the first variation of a gauge-invariant function at the flat field, which vanishes by invariance under constant colour rotations (CMP109 (1.19); the adjoint representation has no invariant vector). \(\square\)

### 4.6 Proposition 4.6 (uniform second amplitude derivative of the readout kernel)

*Statement.* Under (S2)–(S5) and (T1)–(T4), there are constants \(C_K,c_K\) such that for every torus, every \(|s|\le g_k\) and every \(x\),
\[
\Big|\partial_s^2\partial_{u_{x,\mu}}\partial_{u_{0,\nu}}\log Z_\Lambda(s,u)\big|_{u=0}\Big|\le C_Ke^{-c_K|x|}.
\]
Consequently \(|p''_\Lambda(s)|\le C_K':=C_K\sum_{x\in\mathbb Z^4}|x|^2e^{-c_K|x|}\).

*Proof.*

1. **Cumulant expansion.** \(D\) is independent of \((s,u)\). Repeated differentiation of \(\log\int_De^{-H_{s,u}}\) gives the standard identity
\[
\partial_{a_1}\cdots\partial_{a_r}\log Z=\sum_{\pi}\kappa_{|\pi|}\big((\mathcal F^{\beta})_{\beta\in\pi}\big),
\]
summed over the set partitions \(\pi\) of the label multiset \(\{\mathsf s,\mathsf s,\mathsf x,\mathsf 0\}\), under \(\mu_s:=\mu\) at \(u=0\). This is N7.42 iterated, or Faà di Bruno for the cumulant generating function. There are 15 partitions, with cumulants of order \(\le4\).
2. **The law \(\mu_s\).** It satisfies Lemma 4.4 (i)–(iii). Indeed \(H''=M(0)-(V_s)''\ge\gamma_0-C_V(\delta_k+g_k^2)\ge\gamma_0/2\) by (S4)(i), Lemma 4.5 and (T4). The decay (ii) comes from (S4)(ii) and Lemma 4.5. Condition (iii) is Lemma 4.5.
3. **Bounding each partition.** Expand each \(\mathcal F^\beta\) into pieces (Lemma 4.5) and use multilinearity. For a tuple of pieces \((Y_1,\dots,Y_r)\), Lemma 4.4 and (4.1) bound the term by
\[
CK_*^r\prod_i(1+|Y_i|)^{5}e^{-c_*d(Y_i)}e^{-c_*d(Y_i,a(\beta_i))}\cdot e^{-\alpha\ell/(r-1)}.
\]
4. **Anchoring.** Every partition has the anchors \(x\) and \(0\) in some blocks. Following anchor \(x\) to its piece, through the tree, to the piece of anchor \(0\):
\[
|x|\le\sum_i\big[d(Y_i,a(\beta_i))+\mathrm{diam}\,Y_i\big]+\ell,\qquad\mathrm{diam}\,Y\le C(1+d(Y)).
\]
5. **Summation.** Spend half of each exponential rate to obtain \(e^{-c_K|x|}\). Sum the remaining half over the positions of the pieces:
   - the piece carrying anchor \(0\) is summed with its own anchor decay;
   - the others are summed through the tree decay;
   - the polynomial factors \((1+|Y|)^5\le C(1+d(Y))^{20}M^{20}\) are absorbed by \(e^{-c_*d(Y)/2}\).

   The sums are uniform in \(\Lambda\), because all weights are summable on \(\mathbb Z^4\) and periodic images only add exponentially small terms.

None of the constants involves \(k\), \(\Lambda\), \(P_k\) or the array. \(\square\)

*Remark (why the real-variable step is needed).* A purely analytic proof is possible: holomorphy of the CMP116 expansion in complex \(s\) on \(|s|<c/P_k\), followed by Cauchy. It loses \(P_k^2\). On that disc the cubic term is of size \(|s|P_k|B|^2\), so the activities are \(O(1)\) rather than \(O(s^2)\), and Cauchy gives only \(|p(g)-p(0)|\le Cg^2P_k^2=C\ell_k^{2p_0}/Y_k\). That form is **not** sufficient for Corollary D, which needs \(|r_m|\le Av_m^3\) without logarithms. The moment bounds of Lemma 4.4 see Gaussian moments of order \(1\), not the cutoff. The toy model in §9 (3) shows \((p(g)-p(0))/g^2\) converging to its Wick value while \(P\) grows.

### 4.7 Lemma 4.7 (the \(s=0\) term)

*Statement.* Under (S6), (S7) and (T3), \(|p_\Lambda(0)-d^G_{k,\Lambda}|\le C_{\rm def}e^{-\gamma_2P_k^2/20}\), uniformly in \(\Lambda\) and in the infinite-volume limit.

*Proof.*

1. **Reduction to the defect.** \(V_0=0\), so \(\log Z_\Lambda(0,u)=\log Z^{(k)}(U_{k+1}(W_u))+\log\mu_{C^{(k)}(U)}(D)+\text{const}\), and \(p_\Lambda(0)-d^G_{k,\Lambda}=\mathcal P_\Lambda\log\mu_{C^{(k)}(U)}(D)\).
2. **Localised defect.** By (S7), \(\log\mu_{C^{(k)}(U)}(D)=\sum_XF(X)\) with \(F(X)\) analytic on \(\mathbf U^c_{k+1}(X,\alpha_0,\alpha_1)\) and \(|F(X)|\le C'e^{-\gamma_2P_k^2/20}e^{-\kappa d_{k+1}(X)}\).
3. **Fixed-chart readout.** For such a family, \(|\mathcal P_\Lambda\sum_XF(X)|\le C_P\sup_X|F(X)|e^{\kappa d(X)}\). Proof:
   - \(\partial_{u_x}\partial_{u_0}F(X)\) at flat equals \(D^2F(X)[\partial_xU,\partial_0U]+DF(X)[\partial_x\partial_0U]\), with \(U=(U_{k+1},J_{k+1})(W_u)\).
   - Cauchy on the absolute domain bounds \(DF\) and \(D^2F\) by fixed multiples of \(\sup|F(X)|\).
   - (S4)(iii) bounds the tangents restricted to \(X\) by \(Ce^{-c(d(x,X)+d(0,X))}\).
   - The second moment \(\sum_X\sum_x|x|^2e^{-\kappa d(X)-c\,d(x,X)-c\,d(0,X)}\) is finite.

   This is the fixed-chart (absolute radii) case of the readout in the supplementary constant-flux calculation §2, last paragraph, and of (P). \(\square\)

### 4.8 Proof of Theorem 2.1

**Thresholds.** \(Y_\sharp\) is the least value for which every \(Y\ge Y_\sharp\) (with \(g=Y^{-1/2}\), \(\ell=\log Y\), \(\delta=A_1g\ell^{p_0}\)) satisfies:

- (T1) \(g\le\gamma\), CMP109/116's ceiling, including the closing inequality \(O(1)C_3\delta\le\frac12E_0\) of CMP116 p.21 with \(\varepsilon_1\to\delta\);
- (T2) \(4\delta\le\varepsilon_{\rm fix}\), with \(\varepsilon_{\rm fix}\) admissible as trial radius in CMP116 Lemma 1 and as analyticity radius in (S3);
- (T3) \(\gamma_2A_1^2\ell^{2p_0}\ge\Pi_*\), the H-cut lower bounds of the native estimate §20.2;
- (T4) \(C_V(\delta+g^2)\le\gamma_0/2\);
- (T5) \(e^{-\gamma_2A_1^2\ell^{2p_0}/20}\le1/Y\). This holds for large \(Y\) because \(2p_0>1\).

Each is a condition on the single number \(Y\), so (0.1) gives all of them at every step.

**Part 1** is Lemma 4.1.

**Part 2.** Fix \(k\le n\) and a torus \(\Lambda\) large enough for the localised representations.

1. **Smoothness.** \(p_\Lambda\) is a smooth function of \(s\in[-g_k,g_k]\): it is a finite-dimensional integral over a fixed compact domain of an integrand analytic in \((s,u,B)\).
2. **Taylor.** By Lemma 4.2, \(p'_\Lambda(0)=0\). Taylor's formula with integral remainder and Proposition 4.6 give
\[
|p_\Lambda(g_k)-p_\Lambda(0)|=\Big|\int_0^{g_k}(g_k-s)p''_\Lambda(s)\,ds\Big|\le\tfrac12C_K'g_k^2.
\]
3. **The \(s=0\) end.** Lemma 4.7 gives \(|p_\Lambda(0)-d^G_{k,\Lambda}|\le C_{\rm def}e^{-\gamma_2P_k^2/20}\).
4. **Volume limit.**
   - By (1.5), \(p_\Lambda(g_k)\) is the finite-volume readout of the whole-lattice birth sum.
   - By the localised representation of (S1) (CMP116 output, volume-independent for non-wrapping domains, wrapping terms \(O(e^{-\kappa\,{\rm side}})\)), \(p_\Lambda(g_k)\to p^{\rm fix}_{k+1}\) as \(\Lambda\to\infty\). This is the limit of CMP109 (1.21)–(1.22).
   - Likewise \(d^G_{k,\Lambda}\to d^G_k\) and the defect readouts converge.

   The bounds in steps 2–3 are uniform in \(\Lambda\), so they pass to the limit.

This proves the first inequality of (2.1). The second follows from \(g_k^2=1/Y_k\) and (T5), with \(C_\sharp=\frac12C_K'+C_{\rm def}\).

**Part 3.** All constants are those of Lemmas 4.4–4.7. The thresholds depend on \(g_k\) only. \(\square\)

Only steps 2–3 need more than the source. No limit of derivatives in \(s\) is taken, so analyticity in \(s\) of the infinite-volume objects is not needed.

### 4.9 Proof of Corollary 2.2 (identification with the analysis comparator)

*Claim, by induction on \(j\le k+1\).* On the real native domain \(\mathbf U^{\mathbb R}_j\) at scale \(j\) (provisional radii for the newest scale), the real functions \(\mathsf H'_j\) and \(\mathsf H^{\rm fix}_j:=\sum_XH^{\rm fix}_j(X)\) coincide, and \(\mathcal P\mathsf H'_j=\mathcal P\mathsf H^{\rm fix}_j\).

- **Domains.** Below the ceiling, the running radii \(\alpha_{u,j}=C_ug_j\ell_j^q\) are smaller than the absolute \(\alpha_u\). Conditions (i)–(iv) of CMP109 (1.11)–(1.16) are monotone in the radii, so \(\mathbf U^{\mathbb R}_j\subset\mathbf U^c_j(\cdot,\alpha_0,\alpha_1)\). Hence \(\mathsf H^{\rm fix}_j\) is defined wherever \(\mathsf H'_j\) is.
- **Base.** \(j=0\): no births.
- **Step.** Assume the claim for all \(i\le j\).
  - By the analysis Theorem A′ (last sentence), with (F2) and Proposition L2.2 item 3, \(\mathsf H'_{j+1}\) is the pure-E step at Wilson coefficient \(Y_j\), with the cutoff \(D_j\), applied to the sums \(\mathsf H'_i\) with their subtractions \(\mathcal P\mathsf H'_i\).
  - \(\mathsf H^{\rm fix}_{j+1}\) is the same step applied to \(\mathsf H^{\rm fix}_i\) with subtractions \(\mathcal P\mathsf H^{\rm fix}_i\).
  - The step-\(j\) integral evaluates the inherited sums only at composite configurations built from a real background in \(\mathbf U^{\mathbb R}_{j+1}\) and a real fluctuation in \(D_j\). By the real part of (D\(^*\)) these lie in \(\mathbf U^{\mathbb R}_i\), where the inherited sums and their subtractions coincide by the induction hypothesis.
  - The Gaussian, the cutoff, the gauge fixing and \(\mathbf P^{(j)}\) are identical (same \(Y_j\)).
  - So the two integrals are the same real integral, and the outputs coincide on \(\mathbf U^{\mathbb R}_{j+1}\).
  - The projection is a germ quantity at the flat field, an interior point. On each torus the two second derivatives agree, so the infinite-volume limits agree.

Taking \(j=k+1\) and Theorem 2.1 gives the corollary. \(\square\)

This is the point of the analysis Finding 2. The fixed-chart content is a statement about whole-lattice sums. No identification of two different localisations is made.

## 5. Coefficient dictionary and sign, as far as (C2) carries them

1. **(C2) is normalisation-free.** Both \(p^{\rm fix}_{k+1}\) and \(d^G_k\) are read by the same \(\mathcal P\) of CMP109 (1.22), with \(\mathcal PA=1\) (§1.1). So (2.1) holds in whatever units \(\mathcal P\) uses. The numerical value of \(d_B\) is entirely in (G).
2. **What \(d^G_k\) is.** \(d^G_k=\mathcal P\log Z^{(k)}\): the uncut, stationary, \(g\)-independent Gaussian normaliser of CMP109 (1.4)/(2.11), including the background-dependent constraint and coarea factors in \(Z^{(k)}\). It depends only on \(k\), through the depth of the fine minimiser. **Interface check for (G):** the cumulative \(D^G_n=\sum_{k<n}d^G_k\) of the constant-flux calculation §§1–3 is computed as a cumulative hard density at constant flux, identified with the product of per-step Gaussian densities "including the native coareas" through N2 H.1. That identification was not checked here. It is the one place where the object of (C2) and the object of (G) must be matched.
3. **Arithmetic (rerun).** In Bałaban's units (\(\exp(-Y A)\), \(A=\sum_p[1-\mathrm{Re}\,\mathrm{tr}\,U_p]\), \(\mathrm{tr}\,1=1\), plaquettes once), \(Y=\beta_{\rm std}=2N/g_{\rm std}^2\). The textbook one-loop value \(d(g_{\rm std}^{-2})/d\ln\mu=11N/(24\pi^2)\) gives
\[
d_B=2N\cdot\frac{11N}{24\pi^2}\log L=\frac{11N^2\log L}{12\pi^2}>0.
\]
4. **Sign.** If (G) holds, (C2) makes the comparator decrement positive on average: \(p^{\rm fix}_{k+1}=d^G_k+O(1/Y_k)\) and \(\sum d^G_k=d_Bn+O(1)\), so \(Y\) decreases toward the infrared.
5. **Per-step sign.** (C2) does **not** give a positive sign per step: \(d^G_k\) may carry a bounded transient of either sign. This is why Corollary D uses the corrected coordinate \(y=Y+D^G_i-d_Bi\).
