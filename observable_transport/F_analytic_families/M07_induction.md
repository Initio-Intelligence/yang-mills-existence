# Exact matching identities for conditional source transport

## 1. Setting, objects, notation

### 1.1 Scales and couplings

Fix \(L\) odd, \(\ell_0\), \(a=L^{-K}\ell_0\), \(h_k=L^ka\) for \(0\le k\le K\), on the torus \(T\). Scale \(k=0\) is the bare Wilson lattice; \(k=K\) is the physical scale \(\ell_0\). Bałaban's RG runs \(k\to k+1\) (toward the infrared); the coupling \(g_k\) increases with \(k\) (asymptotic freedom). B-03/B-04 index the coupling toward the ultraviolet: with \(u_j\) the B-04 variable, the coupling at RG scale \(k\) is \(u^{\rm RG}_k:=u_{K-k}\), \(u^{\rm RG}_k\asymp g_k^2\) in the coordinate of §2 of [The Wilson trajectory on intervals admitting mature resets](../../coupling/finite_window.md). In particular (Annex S (B.5)) \(u^{\rm RG}_k=[b(K-k+\kappa)]^{-1}(1+o(1))\), \(\kappa=(bu_0)^{-1}\), \(u_0=u^{\rm RG}_K=g_*^2\) fixed.

### 1.2 The law and the norm (recalled, not redefined)

The state at scale \(k\) is the augmented source-free state of Annex Y §1: retained coordinates, history labels, padded inactive sectors, reference point \(x_*\). Its law \(\mu_{h_k}\) is the **actual normalized law** of Annex W (4.1)–(4.2); sectors are events, with probabilities \(\mathbb P(H_k=h)=Z_{k,h}/\mathscr Z\). The one-step operation \(Q_k\) is the actual conditional expectation / replacement / reset in common coordinates, (M.28), including coarea, selectors and all normalizers in the kernel \(q_y\).

A decorated coefficient is \(\mathbf A_{I,X}=(A,B,J)\) with \(\delta_\tau A=B_\tau+J_\tau\) (M.10). Its current-scale carrier norm is (M.12),
\[
\|\mathbf A_I\|_{h,\kappa}=\sum_{X\supset\mathrm{anchors}(I)}w_h(X)\,[v_{h,m,X}(A)+g_{h,m,X}(B)+j_{h,m,X}(J)],
\]
with \(w_h(X)=e^{\kappa(|X|+\mathsf t_h(X))}\) (M.2), \(v,g,j\) from (M.11) with the \(h^{4m}\) grading, the native regulator (M.5) and the averaged moment norm (M.8). Exact transport is Theorem M.3, (M.30)–(M.32); exact cumulant transport of a finite jet is (M.42):
\[
A'_I=\sum_{\pi\in\Pi(I)}\kappa_{Q}\big(A_B:B\in\pi\big).
\]
All statements below are about finite jets of every order \(m\); no infinite source series is summed.

### 1.3 Transported fields on the path space

By Annex T, Theorem 1.1 (M-01, complete), the transported one-field marks are path-space conditional expectations \(F_{k,\alpha}=\mathbb E[\Phi_{a,\alpha}\mid\mathcal G_k]\), where \(\Phi_{a,\alpha}\), \(\alpha=1,\dots,21\), are the bare F-01 fields (M.20), \(\Phi_a=Z_{a,T,\mu}\widetilde q_a-c_{a,T,\mu}e_S\). The initial decorated record has \(B=\delta\Phi\), \(J=0\), and \(\|\mathbf\Phi_{\alpha,a}\|_{a,\kappa}\le Cb_a\) (M.22). **No bound on \(b_a\) is used anywhere below**; this is how the M-04 clarification ("does not assume the final running \(Z\) from F-05") is respected.

### 1.4 Channels, local fields and the local extraction

Let \(E=\mathrm{Sym}^2(\Lambda^2\mathbb R^4)\), \(\dim E=21\), with the seven absolutely irreducible \(H_4\)-summands of Annex D/Annex P §1, projectors \(P_\rho\), dimensions \(1,3,2,6,6,1,2\). The identity \(\mathbf 1\) is a separate field in the trivial channel (Annex P §4). Write \(e_{k,\alpha}\) for the scale-\(k\) native F-01 representative of component \(\alpha\) at a given anchor (the scalar-repaired clover basis of Annex X §1 on the scale-\(k\) lattice), and \(\rho(\alpha)\) for its channel.

**Local extraction.** For \(m\ge1\) let \(\mathcal L^{(m)}_k\) be the finite-dimensional space of local polynomial kernels of engineering dimension \(\le4m\) at the (merged) anchor(s) of an \(m\)-tuple of labels, built from the fields \(e_{k,\beta}\), \(\mathbf 1\) and their lattice differences, with the reblocking convention that an order-\(m\) coefficient of block labels is the \(L^{-4m}\)-weighted sum over the fine labels it contains (as in [Transport of insertions on a reference torus](../../lattice_theory/insertion_transport.md) (3.3), \(c_{k+1}(x)=L^{-4}\sum_{y\in\mathrm{block}(x)}c_k(y)\)). Let \(\Pi^{(m)}_k\) denote the Taylor-moment extraction onto \(\mathcal L^{(m)}_k\) at the reference point \(x_*\) (Bałaban's extraction of the vacuum and Wilson coefficients from small polymers; [Transport of insertions on a reference torus](../../lattice_theory/insertion_transport.md), Theorem 3.1(iii), \"extraction of \(R^{(0)}\) and \(R^{(2)}_{m_0}\) of every small marked polymer\"). For \(m=1\), \(\mathcal L^{(1)}_k=\mathrm{span}\{e_{k,\beta}\}\oplus\mathbb R\mathbf 1\) and \(\Pi^{(1)}_k\) extracts the coefficient of each \(e_{k,\beta}\) and of \(\mathbf 1\). **Convention:** "dimension \(\le4m\)" counts the \(4(m-1)\) carried by the coincidence \(\delta\)-functions of an order-\(m\) contact kernel; the local operator \(P\) itself is marginal when \(\dim P=4\) and relevant when \(\dim P<4\). The extracted set is therefore exactly the identity kernels (any number of source derivatives) and \(\bar f^{\,m}e_\beta\); see [M07 analytic family](M07_analytic_family.md), Lemma 9.1 and §11.7.

The properties of \(\Pi^{(m)}_k\) that are used — it is a linear, \(H_4\)-equivariant, history-independent projection, bounded on the range of \(Q_k\) in the norm (M.12), with \(\Pi^{(m)}_{k}\) applied to a scale-\(k\) local kernel equal to that kernel — are **hypotheses** listed under (G1)(iii). The exact construction of \(\Pi^{(m)}\) for \(m\ge2\) with all compatible contact terms is the object of F-06 ("actual compatible local extractions"); M-07 uses it as an interface.

### 1.5 The decomposition and the running coefficients

**Definition 1.1.** For \(0\le k\le K\) and each \(\alpha\) write
\[
F_{k,\alpha}=t_{\rho(\alpha),k}\,e_{k,\alpha}+v_k\,\delta_{\rho(\alpha),\mathrm{triv}}\mathbf 1+W_{k,\alpha},
\qquad \Pi^{(1)}_kW_{k,\alpha}=0.
\tag{1.1}
\]
Here \(t_{\rho,k}\in\mathbb R\) is the **local field coefficient** of channel \(\rho\), \(v_k\) the **identity coefficient**, and \(W_{k,\alpha}\) the **one-field remainder** (irrelevant and nonlocal records, including all history-dependent parts). By equivariance of \(Q_{0\to k}\) and of \(\Pi^{(1)}\), \(t\) depends on \(\alpha\) only through \(\rho(\alpha)\) and \(W_{k,g\alpha}=g\cdot W_{k,\alpha}\). Initially \(t_{\rho,0}=z_{\rho,a,T,\mu}\) (F.33), \(v_0=-c_{a,T,\mu}\), \(W_{0,\alpha}=0\).

Define the **normalized remainder** and the **renormalized transported field**
\[
\omega_{k,\alpha}:=t_{\rho(\alpha),k}^{-1}W_{k,\alpha},
\qquad
Y_{k,\alpha}:=t_{\rho(\alpha),k}^{-1}\big(F_{k,\alpha}-v_k\delta_{\rho,\mathrm{triv}}\mathbf 1\big)=e_{k,\alpha}+\omega_{k,\alpha},
\tag{1.2}
\]
whenever \(t_{\rho,k}\ne0\) (Lemma 3.4 gives \(t_{\rho,k}>0\) under (I-F4)).

**Lemma 1.1 (exact channel-matrix identity).** Assume \(\Pi^{(1)}_{k+1}\) exists with the properties in (G1)(iii). Define the numbers
\[
M_{\rho,k}:=\Pi^{(1)}_{k+1}\big[Q_k e_{k,\alpha}\big]_{e_{k+1,\alpha}}+\Pi^{(1)}_{k+1}\big[Q_k\omega_{k,\alpha}\big]_{e_{k+1,\alpha}},
\qquad
c_k:=\Pi^{(1)}_{k+1}\big[Q_k e_{k,S}\big]_{\mathbf 1}+\Pi^{(1)}_{k+1}\big[Q_k\omega_{k,S}\big]_{\mathbf 1},
\tag{1.3}
\]
where \([\cdot]_{e}\) denotes the extracted coefficient of \(e\). Then, exactly,
\[
t_{\rho,k+1}=M_{\rho,k}\,t_{\rho,k},
\qquad
v_{k+1}=v_k+c_k\,t_{\mathrm{triv},k},
\qquad
W_{k+1,\alpha}=(I-\Pi^{(1)}_{k+1})Q_kF_{k,\alpha}.
\tag{1.4}
\]
*Proof.* \(F_{k+1,\alpha}=Q_kF_{k,\alpha}=t_{\rho,k}Q_ke_{k,\alpha}+v_k\delta Q_k\mathbf 1+Q_kW_{k,\alpha}\) by linearity and the tower property (Annex T (1.5)); \(Q_k\mathbf 1=\mathbf 1\) by \(q_y(1)=1\) (M.28). Apply \(\Pi^{(1)}_{k+1}\), use \(\Pi^{(1)}\mathbf 1=\mathbf 1\), \(\Pi^{(1)}e=e\), and equivariance (the extracted coefficient of \(e_{k+1,\beta}\) in \(Q_ke_{k,\alpha}\) vanishes unless \(\beta=\alpha\) by Schur's lemma on absolutely irreducible real summands, Annex P §1). The remaining coefficient is \(t_{\rho,k}M_{\rho,k}\) with \(M\) as in (1.3), since \(W_{k,\alpha}=t_{\rho,k}\omega_{k,\alpha}\). The \(\mathbf 1\)-coefficient gives the \(v\)-recursion (only the trivial channel has a \(\mathbf 1\) component). \(\square\)

**Remark 1.2 (what Lemma 1.1 says about F-04).** The "actual channel matrix" \(M_k=\sum_\rho M_{\rho,k}P_\rho\) of F-03/F-04 is *by definition* the local-projection ratio (1.3). It therefore **already contains the feedback** \(\Pi^{(1)}Q_k\omega_k\) of the accumulated irrelevant remainder into the local field. Consequently the exact one-field recursion has **no additive field-valued remainder in the coefficient**: in the notation of Annex P (R.20), \(\mathcal R_j\equiv0\) for the coefficients, and (R.21)–(R.22) are not needed for the one-field level. The whole irrelevant content sits in \(W\), which is normalized by its *own* channel's \(t_{\rho,k}\). This is what removes the relative anomalous-dimension logarithms \((t_\rho/t_\sigma)_k\) between channels that would otherwise appear in a norm-level (non-expectation) induction; see Lemma 3.2 and Remark 3.9.

### 1.6 Order \(m\ge2\): local kernels and response remainder

For \(|I|=m\ge2\) write the exact transported connected coefficient (M.42) as
\[
A^{(k)}_I=\sum_{P\in\mathcal L^{(m)}_k}C^{(k)}_{I,P}\,P+R^{(k)}_I,\qquad \Pi^{(m)}_kR^{(k)}_I=0.
\tag{1.5}
\]
The numbers \(C^{(k)}_{I,P}\) are the **local response kernels** (contact and lower-dimension mixing kernels: relevant when \(\dim P<4m\), marginal when \(\dim P=4m\)); \(R^{(k)}_I\) is the **irrelevant response remainder**. The **explicit normalization** of label tuple \(I\) at scale \(k\) is
\[
\mathfrak N^{(k)}_I:=\prod_{i\in I}t_{\rho(i),k}+\sum_{P\in\mathcal L^{(m)}_k}|C^{(k)}_{I,P}|\,\|P\|_{h_k,\kappa}
\quad(m\ge2),\qquad
\mathfrak N^{(k)}_{\{i\}}:=t_{\rho(i),k}.
\tag{1.6}
\]
This is the "specified incoming current-scale carrier budget with its actual running mixing coefficients" of (HL.42). All budgets below are stated **relative to \(\mathfrak N^{(k)}\)**; the uniform constants are the ratios.

---

## 2. Interface hypotheses

Each hypothesis is stated at **one fixed scale \(k\)** for an input satisfying the **induction budget at scale \(k\)**:
\[
(\mathsf B_k)\qquad
\|\mathbf A^{(k)}_B\|_{h_k,\kappa}\le b_*^{|B|+1}\,(|B|!)^{p_*}\,\mathfrak N^{(k)}_B
\quad\text{for every label set }B,\ 1\le|B|\le m,
\tag{2.1}
\]
with fixed \(b_*,p_*\) and the explicit normalization (1.6). The constants in every hypothesis are independent of \(k\), \(K\), \(T\), the admitted history and the source order \(m\), unless a dependence is displayed. "Admitted" means: the trajectory satisfies the source ceilings of J0/C-01 (CMP 119 (2.4)–(2.9), p. 255–256) and \(u^{\rm RG}_k\le u_*\).

### (I-M6) — the one-step regular finite-jet response algebra (what M-06 promises)

*M-06 statement:* exact local expansion of the full jet through one step, retaining every collision, reset and remainder vertex; fixed factorial budget. *Test:* compatibility as \(m\) varies; a carrier-bound sum with fixed \(q,p\).

**(I-M6).** There are \(C_6\ge1\), \(p_6\ge0\) and a spatial order \(\kappa>0\) (the \(q\) of the test is the exponential carrier weight (M.2) with this \(\kappa\)) such that for every admitted \(k<K\), every regular-sector one-step kernel \(Q^{\rm reg}_k\), every finite decorated input jet satisfying \((\mathsf B_k)\), every \(I\) with \(|I|=m\) and every partition \(\pi\in\Pi(I)\), the exact conditional cumulant admits compatible carrier records (M.36)–(M.39) with
\[
\big\|\kappa_{Q^{\rm reg}_k}(\mathbf A^{(k)}_B:B\in\pi)\big\|_{h_{k+1},\kappa}
\le C_6^{\,m+1}\,(|\pi|!)^{p_6}\prod_{B\in\pi}\|\mathbf A^{(k)}_B\|_{h_k,\kappa},
\tag{2.2}
\]
and in particular (\(|\pi|=1\)) \(\|Q^{\rm reg}_k\mathbf A^{(k)}_I\|_{h_{k+1},\kappa}\le C_6\|\mathbf A^{(k)}_I\|_{h_k,\kappa}\). Compatibility: the records for the order-\(m\) jet restrict to those of every lower-order truncation (Annex Y §5, last paragraph).

*Exactness check.* (2.2) is the fixed-factorial carrier-bound sum of the test, with \(p=p_6\) the factorial parameter and \(q=\kappa\) the spatial parameter; "compatibility as \(m\) varies" is the restriction property. Nothing about contraction, locality gains, or the size of the local projection is included — M-06's test does not promise them. **M-07 needs more** (see (G1)).

### (I-H4) — the one-step full-law estimate (what H-04 promises)

*H-04 statement (clarified):* at one arbitrary scale, sum regular, repaired, residual and inherited bad sectors in the full normalized law for input jets satisfying the M-03/M-06 induction budget, keeping all exact output responses and a fixed factorial growth budget, uniformly over admissible scales and histories. *Test:* one full-law one-step estimate that can feed M-07, no discarded positive-probability sector, no hidden denominator/volume loss; **the all-scale input bounds to be proved in M-07 are not assumed.**

**(I-H4).** Let \(Q_k\) be the full one-step operation of the normalized law (Annex W (4.2)–(4.9): regular kernel on the regular sector, replacement kernels (4.3)–(4.5) and resets (4.7)–(4.9) on the other sectors, with their actual normalizers). There are \(C_H\ge1\), \(p_H\ge0\) such that for every admitted \(k<K\), every input jet satisfying \((\mathsf B_k)\), every \(I\) with \(|I|=m\) and every \(\pi\in\Pi(I)\),
\[
\big\|\kappa_{Q_k}(\mathbf A^{(k)}_B:B\in\pi)\big\|_{h_{k+1},\kappa}
\le C_H^{\,m+1}\,(|\pi|!)^{p_H}\prod_{B\in\pi}\|\mathbf A^{(k)}_B\|_{h_k,\kappa},
\tag{2.3}
\]
where the left side is the **sum over all sectors** of the normalized law weighted by their exact probabilities (4.2), with every output response (direct records \(B\), kernel currents \(J\) from selector/support/normalizer changes (M.29), reset responses (4.9)) retained. The hypothesis is on \(Q_k\) at scale \(k\) only; the input bound is \((\mathsf B_k)\), which M-07 supplies inductively.

*Exactness check.* (2.3) is "one full-law one-step estimate that can feed M-07", with the fixed factorial budget and no sector discarded. It does **not** state the *size* of the bad-sector contribution relative to the regular one; H-04's test does not promise that. Where M-07 would need it, see (G2).

### (I-F4) — the one-step mixing-matrix error (what F-04 promises)

*F-04 statement:* \(\|M_j-I-u_j\Gamma\|\le Cu_j^2\) for the actual channel matrices, uniformly in cutoff, carriers, retained backgrounds and histories admitted to this regular calculation. *Test:* a uniform matrix norm with the exact source of every derivative and remainder.

**(I-F4).** With \(M_k=\sum_\rho M_{\rho,k}P_\rho\) the channel matrix of Lemma 1.1 (the projection of the exact regular transported one-field outputs onto the seven channels, as in F-03's statement), there are a fixed equivariant \(\Gamma=\sum_\rho\gamma_\rho P_\rho\), \(\|\Gamma\|\le G\), and \(C_4<\infty\), such that for every admitted \(k<K\),
\[
\|M_k-I-u^{\rm RG}_k\Gamma\|\le C_4\,(u^{\rm RG}_k)^2 .
\tag{2.4}
\]
*Exactness check.* This is F-04's displayed inequality. The identification of \(\Gamma\) is F-03 and is not used; only \(\|\Gamma\|\le G\) enters. Note that \(M_k\) in (1.3) includes the irrelevant feedback; F-04's "uniformly in ... histories" is what makes that inclusion legitimate.

### (I-B3) — the one-step coupling recurrence (what B-03 promises)

**(I-B3).** There are \(b>0\), \(A\ge0\), \(u_*>0\) satisfying Annex S (B.1), such that the B-03 coupling coordinate obeys \(u_{j+1}=u_j-bu_j^2+r_j\), \(|r_j|\le Au_j^3\), \(0<u_0\le u_*\), with \(r_j\) allowed to depend on the whole earlier sequence (Annex S (B.2)).

The coupling recurrence is assumed at each admitted scale before the weak stop.

### (G1) — the gap: irrelevant contraction, bounded births, bounded extraction (needed by M-07, promised by no dependency)

**(G1).** There are \(\theta\in(0,1)\), \(\beta_*<\infty\), \(C_\Pi<\infty\) such that for every admitted \(k<K\) and every \(m\ge1\):

(i) *Irrelevant contraction.* For every decorated record \(\mathbf R\) of order \(m\) at scale \(k\) with \(\Pi^{(m)}_k\mathbf R=0\) and finite norm,
\[
\big\|(I-\Pi^{(m)}_{k+1})\,Q_k\mathbf R\big\|_{h_{k+1},\kappa}\le\theta\,\|\mathbf R\|_{h_k,\kappa}.
\tag{2.5}
\]
(ii) *Bounded births from local kernels.* For every \(P\in\mathcal L^{(m)}_k\),
\[
\big\|(I-\Pi^{(m)}_{k+1})\,Q_kP\big\|_{h_{k+1},\kappa}\le\beta_*\,\|P\|_{h_k,\kappa}.
\tag{2.6}
\]
(iii) *Extraction.* \(\Pi^{(m)}_{k+1}\) is a linear, \(H_4\)-equivariant, history-independent projection onto \(\mathcal L^{(m)}_{k+1}\) with \(\|\Pi^{(m)}_{k+1}Q_k\mathbf A\|_{h_{k+1},\kappa}\le C_\Pi\|\mathbf A\|_{h_k,\kappa}\) on the full-law output, and \(\Pi^{(m)}_kP=P\) for \(P\in\mathcal L^{(m)}_k\).

*Why this is a gap.* M-07's statement itself says "with ... summable irrelevant gains"; (2.5) is that gain. M-06's test gives only (2.2) with \(C_6\ge1\); H-04's test gives (2.3). Neither mentions a contraction of the non-local part, nor the extraction (iii), which is F-06's object ("actual compatible local extractions"), and F-06 is **not** a dependency of M-07 in the catalogue. Proposition 3.8 shows (2.5) cannot be dispensed with. The natural source of (2.5) is the dimensional gain \(L^{-(d-4m)}\) of a dimension-\(d>4m\) record under one blocking in the \(h^{4m}\)-graded norm ([Transport of insertions on a reference torus](../../lattice_theory/insertion_transport.md) (3.6): \(L^{-2(k-j)}\) for degree \(\ge3\) births; Annex P §5: \(L^{-\epsilon j}\)), **but** \(Q_k\) is a conditional expectation under the actual law, not a rescaling; §6.1 records exactly which one-step law property is needed.

### (G2) — soft gap: size of the bad-sector correction to the channel matrices

**(G2).** \(\sum_{k<K}\big\|M^{\rm full}_k-M^{\rm reg}_k\big\|\le C_{\rm bad}\) uniformly in \(K\), where \(M^{\rm full}_k\) is (1.3) computed with the full-law \(Q_k\) and \(M^{\rm reg}_k\) with \(Q^{\rm reg}_k\).

F-04 is stated for the regular calculation; (I-H4) bounds the full-law output but not the difference. The expected size is the large-field weight \(e^{-p_0(g_k)}=e^{-A_0\ell_k^{p_0}}\) (LFR II (1.99)–(1.101), p. 390), which is summable in \(k\) for \(p_0>1\) (Annex Z, Prop. EC.7's upper bound with \(m\) fixed). **(G2) is not needed for the closure of the induction** (Lemma 3.3 needs only \(|M^{-1}_{\rho,k}|\le1+\delta\)); it is needed to transfer the log-power asymptotics (R.15) from the regular to the full-law running coefficients, which is F-05's input.

### Hypothesis-use table

| Hypothesis | Used in | What is used |
|---|---|---|
| (I-M6) | Thm 3.6 | fixed-factorial cumulant births (2.2) on the regular sector |
| (I-H4) | Lemma 3.3, Thm 3.6 | full-law one-step bound (2.3): same form with \(C_H,p_H\); sectors summed |
| (I-F4) | Lemma 3.3 (only \(\|M_k^{-1}\|\le1+\delta\)); Lemma 3.4 (full strength) | invertibility and smallness; Annex P (R.4) |
| (I-B3) | Lemma 3.4 only | Annex P (R.3), (R.13) via Annex S Thm 1.1 |
| (G1) | Lemmas 3.2–3.3, Thm 3.6 | contraction \(\theta\), births \(\beta_*\), extraction |
| (G2) | Remark 3.10 only | asymptotics of full-law \(t_{\rho,k}\) for F-05 |

### 2bis. (G3) — the nonlinear gap: per-step connection cost at orders \(m\ge2\)

The hypotheses above suffice for the **one-field** induction (Theorem 3.1). For orders \(m\ge2\) the literal forms (2.2)–(2.3) are **not iterable** (Proposition 3.8(b)). What would make them iterable is:

**(G3-strong).** For \(|\pi|\ge2\), (2.2)–(2.3) hold in the sharpened form
\[
\big\|\kappa_{Q_k}(\mathbf A^{(k)}_B:B\in\pi)\big\|_{h_{k+1},\kappa}
\le \varepsilon_k^{\,|\pi|-1}\,|\pi|!\,\prod_{B\in\pi}\|\mathbf A^{(k)}_B\|_{h_k,\kappa},
\qquad \sum_{k<K}\varepsilon_k\le E_*<\infty .
\tag{2.7}
\]
Proposition 3.8(c) shows that (2.7) is **false for the free Gaussian step** in the M-03 coefficient norm (there \(\varepsilon_k=O(1)\) at every step, yet the true all-order hierarchy is depth-uniform). So (G3-strong) is a sufficient but unnatural hypothesis; the natural repair is an analytic-family induction hypothesis (Lemma 3.10 and §5, gap G3).

---

## 3. The induction theorem

Throughout, \(u_k:=u^{\rm RG}_k\le u_*\) with \(u_*\) small enough that \(Gu_*+C_4u_*^2\le\tfrac12\) (Annex P (R.5)) and \(\theta(1+2Gu_*+2C_4u_*^2)\le\theta'<1\).

### Theorem 3.1 (one-field exact matching induction; conditional)

Assume (I-F4), (I-H4) and (G1). Then for every \(0\le k\le K\), every \(\alpha\), on every admitted torus and history:

(a) **Local fields.** \(F_{k,\alpha}=t_{\rho,k}e_{k,\alpha}+v_k\delta_{\rho,\rm triv}\mathbf 1+W_{k,\alpha}\) with \(t_{\rho,k}=z_{\rho,a,T,\mu}\prod_{j<k}M_{\rho,j}>0\), \(v_k=-c_{a,T,\mu}+\sum_{j<k}c_jt_{\rm triv,j}\), the \(M_{\rho,j},c_j\) being the exact extraction ratios (1.3). No property of \(z_{\rho,a,T,\mu}\) or \(c_{a,T,\mu}\) is used.

(b) **Response kernels.** \(W_{k,\alpha}\) carries compatible records \((A,B,J)\); its kernel-current component \(J\) is the sum over steps \(j<k\) of the transported currents (M.30)–(M.32) and reset responses (4.9), and its direct component \(B\) the transported direct differences, all retained separately.

(c) **Uniform budget, no logarithmic accumulation.**
\[
\boxed{\ \|\omega_{k,\alpha}\|_{h_k,\kappa}=\|t_{\rho,k}^{-1}W_{k,\alpha}\|_{h_k,\kappa}\le\omega_*:=\frac{(1+\delta)\beta_*\,\|e\|_*}{1-\theta'}\ }
\tag{3.1}
\]
with \(\delta:=2Gu_*+2C_4u_*^2\), \(\|e\|_*:=\sup_{k,\alpha}\|e_{k,\alpha}\|_{h_k,\kappa}<\infty\) (Prop. M.1 at every scale, the native fields being scale-covariant), uniformly in \(k\), \(K\), \(T\) and history. Hence \(\|Y_{k,\alpha}\|_{h_k,\kappa}\le\|e\|_*+\omega_*\).

(d) **Running normalization.** If in addition (I-B3) holds, then with \(T_k:=\sum_\rho(t_{\rho,k}/t_{\rho,0})P_\rho\), Annex P Theorem 2.1 and Corollary 3.1 apply: \(\|T_k\|+\|T_k^{-1}\|\le2\exp(G\sum_{j<k}u_j+C_1V)\) and \(((K-k+\kappa)/(K+\kappa))^{\Gamma/b}\,T_k\to\) a positive definite limit as \(K\to\infty\) at fixed \(K-k\), up to the full-law correction (G2).

(e) **Terminal remainder.** Proposition 3.7.

### Lemma 3.2 (normalized remainder recursion; exact)

Under (G1)(iii), for every \(k<K\),
\[
\omega_{k+1,\alpha}=M_{\rho,k}^{-1}\,(I-\Pi^{(1)}_{k+1})\big[Q_ke_{k,\alpha}+Q_k\omega_{k,\alpha}\big].
\tag{3.2}
\]
*Proof.* From (1.4), \(W_{k+1,\alpha}=(I-\Pi^{(1)}_{k+1})Q_kF_{k,\alpha}=(I-\Pi^{(1)}_{k+1})[t_{\rho,k}Q_ke_{k,\alpha}+v_k\mathbf 1+t_{\rho,k}Q_k\omega_{k,\alpha}]\); \((I-\Pi)\mathbf 1=0\); divide by \(t_{\rho,k+1}=M_{\rho,k}t_{\rho,k}\). \(\square\)

The decisive feature of (3.2): **no running coefficient other than the single step ratio \(M_{\rho,k}\) appears.** The quantities \(t_{\rho,j}\), \(j\le k\), their products, and their ratios across channels, have cancelled identically. This is where the logarithmic accumulation of the marginal channels is absorbed: entirely into the explicit \(t_{\rho,k}\), and never into the budget.

### Lemma 3.3 (closure of the one-field budget; conditional on (I-F4), (I-H4), (G1))

For all \(k\le K\), \(\|\omega_{k,\alpha}\|_{h_k,\kappa}\le\omega_*\) with \(\omega_*\) as in (3.1).

*Proof.* Induction on \(k\); \(\omega_{0,\alpha}=0\). Assume \(\|\omega_{k,\alpha}\|\le\omega_*\). By (I-F4) and \(u_k\le u_*\), the eigenvalues of \(M_k\) lie in \([1-\delta/2,1+\delta/2]\subset[\tfrac12,\tfrac32]\) (Annex P proof of Thm 2.1), so \(|M_{\rho,k}^{-1}|\le1+\delta\). The input \(\omega_{k,\alpha}\) satisfies \(\Pi^{(1)}_k\omega_{k,\alpha}=0\) and the budget \((\mathsf B_k)\) at order one; (I-H4) makes \(Q_k\omega_{k,\alpha}\) a finite-norm full-law output, so (G1)(i) applies: \(\|(I-\Pi^{(1)}_{k+1})Q_k\omega_{k,\alpha}\|\le\theta\omega_*\). By (G1)(ii), \(\|(I-\Pi^{(1)}_{k+1})Q_ke_{k,\alpha}\|\le\beta_*\|e\|_*\). Then (3.2) gives \(\|\omega_{k+1,\alpha}\|\le(1+\delta)(\beta_*\|e\|_*+\theta\omega_*)\le\omega_*\) by the choice (3.1) and \(\theta(1+\delta)\le\theta'\). All constants are those of the one-step hypotheses; none depends on \(k,K,T\) or the history. \(\square\)

### Lemma 3.4 (the running normalization is explicit; conditional on (I-F4), (I-B3))

Set \(R_k:=M_k-I-u_k\Gamma\). By (I-F4), \(\|R_k\|\le C_4u_k^2\); by (I-B3) and Annex S (B.6), \(V:=\sum_ku_k^2\le8/(b^2\kappa)\); by (B.1), \(0\le u_k\le1\) and \(Gu_k+C_4u_k^2\le\tfrac12\). These are (R.3)–(R.5). The matrices commute (Annex P §1), so the order of the product is immaterial and Theorem 2.1 of Annex P gives positivity of every \(M_k\), (R.7)–(R.10). Annex S (B.5) gives (R.13); \(\Gamma_j\equiv\Gamma\) gives (R.14) with \(\Xi_j=0\); Corollary 3.1 gives (R.15)–(R.16) in the variable \(n=K-k\). \(\square\)

**Remark 3.5a (what is and is not used).** Lemma 3.3 uses (I-F4) only through \(|M_{\rho,k}^{-1}|\le1+\delta\), hence only one-step smallness. The full \(u_k^2\) error and (I-B3) enter only in Lemma 3.4, i.e. only in the *explicit form* of the local fields, never in the closure.

### Lemma 3.5 (partition sums at fixed factorial exponent; proved)

For \(m\ge1\), \(x\ge0\) and integers \(p\ge1\), \(0\le s\le1\),
\[
\sum_{\pi\in\Pi(m)}x^{|\pi|-1}\,|\pi|!\prod_{B\in\pi}|B|!=m!\,(1+x)^{m-1},
\tag{3.3}
\]
\[
\sum_{\pi\in\Pi(m)}x^{|\pi|-1}(|\pi|!)^{s}\prod_{B\in\pi}(|B|!)^{p}\le(m!)^{p}(1+x)^{m-1}.
\tag{3.4}
\]
*Proof.* Group set partitions by the multiset of block sizes, an integer partition \(\lambda\vdash m\) with multiplicities \(c_j\) and \(\ell\) parts. There are \(m!/\prod_j(j!)^{c_j}c_j!\) set partitions of type \(\lambda\), each with \(\prod_B|B|!=\prod_j(j!)^{c_j}\) and \(|\pi|=\ell\). Hence the left side of (3.3) equals \(m!\sum_\lambda x^{\ell-1}\ell!/\prod_jc_j!\). Now \(\ell!/\prod_jc_j!\) is the number of distinct orderings of the parts of \(\lambda\), i.e. the number of compositions of \(m\) with part multiset \(\lambda\); summing over \(\lambda\) with \(\ell\) fixed gives the number of compositions of \(m\) into \(\ell\) parts, \(\binom{m-1}{\ell-1}\). Thus the sum is \(m!\sum_{\ell=1}^m\binom{m-1}{\ell-1}x^{\ell-1}=m!(1+x)^{m-1}\). For (3.4) use \((|\pi|!)^s\le|\pi|!\) and \(\prod_B(|B|!)^p=(\prod_B|B|!)^{p-1}\prod_B|B|!\le(m!)^{p-1}\prod_B|B|!\), the multinomial coefficient being \(\ge1\). \(\square\)

### Theorem 3.6 (all orders; conditional on (I-M6), (I-H4), (I-F4), (G1), (G3-strong))

Define \(\Lambda_k:=\Lambda_0\prod_{j<k}(1+\varepsilon_j)\le\Lambda_0e^{E_*}\) and the budget \(\beta^{(k)}_m:=(m!)^{p_*}\Lambda_k^{\,m}\), \(p_*:=\max(1,p_6,p_H)\). Then for every \(k\le K\), \(|I|=m\ge1\):
\[
A^{(k)}_I=\sum_{P\in\mathcal L^{(m)}_k}C^{(k)}_{I,P}P+R^{(k)}_I,\qquad
\|R^{(k)}_I\|_{h_k,\kappa}\le r_*\,\beta^{(k)}_m\,\mathfrak N^{(k)}_I,\qquad
\|A^{(k)}_I\|_{h_k,\kappa}\le(1+r_*)\beta^{(k)}_m\mathfrak N^{(k)}_I,
\tag{3.5}
\]
with \(r_*:=(1+\delta)(\beta_*+C_\Pi\Lambda_0^{-1})/(1-\theta')\) uniform in \(k,K,T\), history and \(m\), provided \(\Lambda_0\ge\max(1,\|e\|_*)(1+r_*)\). The local kernels obey the exact linear recursion
\[
C^{(k+1)}_{I,P'}=\sum_{P}\big[\Pi^{(m)}_{k+1}Q_kP\big]_{P'}C^{(k)}_{I,P}+\sum_{\pi\in\Pi(I),|\pi|\ge2}\big[\Pi^{(m)}_{k+1}\kappa_{Q_k}(A^{(k)}_B:B\in\pi)\big]_{P'}+\big[\Pi^{(m)}_{k+1}Q_kR^{(k)}_I\big]_{P'},
\tag{3.6}
\]
whose coefficients are bounded by (I-M6)/(I-H4)/(G1)(iii); they are the relevant (\(\dim P'<4m\)) and marginal (\(\dim P'=4m\)) **response kernels**, explicit but not uniformly bounded (they are the contact and composite-mixing counterterms whose control is F-06/F-07/S-06).

*Proof.* Induction on \(k\), simultaneously for all \(m\). At \(k=0\), \(A^{(0)}_I=0\) for \(m\ge2\) (Annex Y §5: \(\log G_0\) is linear). Assume (3.5) at scale \(k\). Write \(A^{(k+1)}_I=Q_kA^{(k)}_I+\sum_{|\pi|\ge2}\kappa_{Q_k}(A^{(k)}_B:B\in\pi)\) by (M.42) and set \(R^{(k+1)}_I:=(I-\Pi^{(m)}_{k+1})A^{(k+1)}_I\), which gives (3.6) by applying \(\Pi^{(m)}_{k+1}\). For the remainder: (G1)(i) on \(Q_kR^{(k)}_I\) gives \(\theta r_*\beta^{(k)}_m\mathfrak N^{(k)}_I\); (G1)(ii) on the local part gives \(\beta_*\mathfrak N^{(k)}_I\le\beta_*\beta^{(k)}_m\mathfrak N^{(k)}_I\) (\(\Lambda\ge1\)); for the births, (2.7) and the induction hypothesis give
\[
\sum_{|\pi|\ge2}\varepsilon_k^{|\pi|-1}|\pi|!\prod_{B\in\pi}(1+r_*)\beta^{(k)}_{|B|}\mathfrak N^{(k)}_B
\le(1+r_*)^{m}\Lambda_k^{m}\mathfrak N^{(k)}_I\sum_{|\pi|\ge2}\varepsilon_k^{|\pi|-1}|\pi|!\prod_B(|B|!)^{p_*},
\]
using \(\prod_{B\in\pi}\mathfrak N^{(k)}_B\le\mathfrak N^{(k)}_I\) (every tuple of partitions of the blocks composes injectively to a refinement of \(\pi\), cf. (1.6)). By (3.4) the last sum is \(\le(m!)^{p_*}[(1+\varepsilon_k)^{m-1}-1]\). Finally \(\mathfrak N^{(k)}_I\le C_{\mathfrak N}\mathfrak N^{(k+1)}_I\) with \(C_{\mathfrak N}\le1+\delta\) by (1.3)–(1.4) and (G1)(iii) (each local kernel is transported by a bounded ratio; the identity and relevant kernels only grow). Collecting, and absorbing \((1+r_*)^m\le(\Lambda_0/\|e\|_*)^m\) into \(\Lambda_0^m\),
\[
\|R^{(k+1)}_I\|\le(1+\delta)\Big[\theta r_*+\beta_*+(1+\varepsilon_k)^{m-1}-1\Big]\beta^{(k)}_m\mathfrak N^{(k+1)}_I
\le r_*\,(m!)^{p_*}\Lambda_k^{m}(1+\varepsilon_k)^{m}\,\mathfrak N^{(k+1)}_I=r_*\beta^{(k+1)}_m\mathfrak N^{(k+1)}_I ,
\]
where the middle inequality uses \((1+\varepsilon_k)^{m-1}-1\le(1+\varepsilon_k)^m-1\), \(\theta'(1+\varepsilon_k)^m\le\theta'\cdot(1+\varepsilon_k)^m\) and the definition of \(r_*\). The budget constant \(\Lambda_K\le\Lambda_0e^{E_*}\) is uniform in \(K\) exactly because \(\sum\varepsilon_k\le E_*\). \(\square\)

### Proposition 3.7 (terminal remainder with the outer retained-data responses explicitly present; proved)

For \(F,G\in L^2(\mu_0)\) and the finite chain stopped at \(K\), Annex T Corollary 1.2 gives, exactly,
\[
\operatorname{Cov}_{\mu_0}(F,G)=\sum_{k<K}\mathbb E\big[\overline{\eta^F_k}\eta^G_k\big]+\operatorname{Cov}\big(M^F_K,M^G_K\big),
\qquad \eta^F_k=M^F_k-M^F_{k+1},
\tag{3.7}
\]
with \(M^F_k=F_{k}\) the transported field. The first sum is the sum over steps of the within-step conditional covariances, i.e. the order-two connected responses \(\kappa_{Q_k}(\cdot,\cdot)\) of Theorem 3.6 integrated over the outer law; the last term is the **covariance of the retained conditional means at the terminal scale**, the "outer retained-data response" of M-07's required conclusion and the object of H-05. In the normalized variables, \(\operatorname{Cov}(M^F_K,M^G_K)=t_{\rho,K}t_{\sigma,K}\operatorname{Cov}(Y_{K,\alpha},Y_{K,\beta})\) with \(\|Y_{K,\cdot}\|\le\|e\|_*+\omega_*\); the law of \(Y_K\) under the outer retained law is **not** estimated here (Annex T Cor 1.3: the terminal term vanishes only under (1.15); Annex O §7 item 3). The higher-order analogue is the finite formal logarithm of (4.9) applied to the full jet (Annex W, after (4.9)). \(\square\)

### Proposition 3.8 (necessity of the gaps; proved)

(a) *(G1) cannot be dropped.* Let the one-step map satisfy (I-M6), (I-H4), (I-F4) literally with \(C_6=C_H=:C>1\), and suppose \((I-\Pi^{(1)}_{k+1})Q_k\) acts on a one-dimensional irrelevant direction as multiplication by \(C\) (allowed: (2.2) bounds \(Q_k\) only by \(C\)). Then \(\omega_K=\sum_{j<K}C^{K-j}\beta=\beta(C^{K+1}-C)/(C-1)\), i.e. \(\omega_K\asymp(\ell_0/a)^{\log_LC}\): not uniform in depth. With \(C=1\) (no gain, no loss), \(\omega_K=K\beta\asymp\log(\ell_0/a)\): still not uniform. Hence a strict contraction \(\theta<1\) is necessary. The marginal-feedback analogue is Annex P Proposition 5.1.

(b) *The literal (2.2)–(2.3) do not iterate at \(m\ge2\).* Suppose births are bounded exactly by \(C^{m+1}|\pi|!\prod_B\|A_B\|\) with \(C\ge1\) and no small factor. Repeating the proof of Theorem 3.6 with \(\varepsilon_k\equiv C\) gives \(\Lambda_{k+1}\ge\Lambda_k(1+C)\), so \(\Lambda_K\ge(1+C)^K=(\ell_0/a)^{\log_L(1+C)}\): the order-\(m\) budget degrades like \((\ell_0/a)^{m\log_L(1+C)}\). By (3.3) this is sharp within the interface class: a one-step map whose births realize \(\varepsilon^{|\pi|-1}|\pi|!\prod\|A_B\|\) with equality has, after one step, order-\(m\) norm exactly \((1+\varepsilon)^{m-1}\) times the budget.

(c) *(G3-strong) is false for the free Gaussian step, although the truth there is depth-uniform.* Let the marks be \(m\) quadratic forms of a Gaussian field and \(Q_k\) the Gaussian conditional expectation given block averages. The conditional joint cumulant of \(r\ge2\) quadratic forms is \(2^{r-1}\) times a sum over the \((r-1)!\) oriented cycles of traces of products of covariances (Port_11_7_1_Observables, eq. (2)); for neighbouring anchors the one-step covariance is \(O(1)\) in M-03 units. Hence \(\varepsilon_k=O(1)\) at every step, \(\sum_k\varepsilon_k\asymp K\), and (2.7) fails. Nevertheless the exact connected \(m\)-point function of the transported quadratic marks at every scale is \(\le C^m(m-1)!\) uniformly in \(K\), because each quadratic mark can be contracted at most twice **in total over all scales**. The coefficient-norm iteration cannot see this degree constraint; the compounding in (b) is therefore an artifact of the interface, not of the model. \(\square\)

### Lemma 3.10 (positive kernels preserve analytic-family budgets exactly; proved)

Let \(G_k(t;x)\) be, for each configuration \(x\), analytic in \(t\in\mathbb C^n\) on the polydisc \(\mathcal D_\lambda=\{|t_i|\le\lambda\}\) with \(\sup_{\mathcal D_\lambda}|G_k(t;x)|\le\mathcal M_k(x)\), and let \(Q_k\) be a normalized positive kernel (M.28) with \(Q_k\mathcal M_k<\infty\). Then \(Q_kG_k(t;\cdot)\) is analytic on \(\mathcal D_\lambda\) and \(\sup_{\mathcal D_\lambda}|Q_kG_k|\le Q_k\mathcal M_k\). In particular the exponential jet \(G_K=Q_{K-1}\cdots Q_0\exp(\sum t_i\Phi_i)\) satisfies \(\sup_{\mathcal D_\lambda}|G_K|\le Q_{0\to K}\sup_{\mathcal D_\lambda}|e^{\sum t_i\Phi_i}|\) **with no loss per step**, and Cauchy then gives \(|A^{(K)}_I|\le m!\,\lambda^{-m}\sup|G_K|\) for the full (not connected) coefficients. *Proof.* Dominated convergence for the \(t\)-derivatives under the positive measure \(q_y\), and \(|Q_kG|\le Q_k|G|\). \(\square\)

This is the mechanism by which Bałaban's inductive assumption (CMP 119 p. 262, "RT transforms the space with index \(k\) into the space with index \(k+1\)") iterates sup-norm analytic budgets with fixed radii. The obstruction to using it for M-07 is the bare radius: \(|\Phi_{\alpha,a}|\le Ca^{-4}(1+E_X)\) (M.15) forces \(\lambda\asymp a^4\), the "bare \(a^{-4}\) budget" that M-02 and Annex T §5 warn does not become \(h^{-4}\) by conditioning alone. Converting the radius requires the exact extraction of the local kernels at every step (the \(C^{(k)}_{I,P}\) of (3.6)) *inside the analytic family*, i.e. an interacting version of Theorem 3.3 of [Transport of insertions on a reference torus](../../lattice_theory/insertion_transport.md), which §1.5(5) there records as not proved. That is the precise content of gap G3. **Remark (see [M07 analytic family](M07_analytic_family.md), Remark 2.4 and §4.3):** once the bare insertion is placed in the *local* term and transported by exact extraction, the remainder's polydisc is fixed in renormalized sources from the start, so the radius conversion is not the obstruction; the open core is the complex-contour, tail-weighted regulator transfer for the pulled-back mark, (4.2)–(4.3) there.

### Remarks

**3.9 (channel-resolved normalization versus Annex P (R.21)).** Annex P treats the field vector \(X_j\in E\) with a remainder \(\mathcal R_j\) and needs \(\sum_j\|T_{j+1}^{-1}\mathcal R_j\|<\infty\). In a norm-level induction the factor \(\|T_{j+1}^{-1}\|\,\|T_j\|\) is the condition number \(\max_\rho t_\rho/\min_\rho t_\rho\asymp((K+\kappa)/(K-j+\kappa))^{(\gamma_{\max}-\gamma_{\min})/b}\), a power of \(\log(\ell_0/a)\) at the infrared end; with a remainder of size \(u_j^{3/2}\) the sum is **not** uniform in \(K\). Definition 1.1 avoids this by normalizing each channel's remainder with its own \(t_\rho\) (equivariance of \(Q\) and \(\Pi\) puts \(W_{k,\alpha}\) in channel \(\rho(\alpha)\)) and by Lemma 1.1, which puts the feedback into \(M_k\) so that \(\mathcal R_j\equiv0\) for the coefficients. No relative anomalous-dimension power survives in (3.2).

**3.10 (full-law channel matrices and F-05).** Lemma 3.4 is stated for the matrices (1.3) of the operation actually iterated. If \(M_k\) is the full-law matrix and (I-F4) is only known for \(M^{\rm reg}_k\), one needs (G2) to recover (R.4) with a summable \(R_j\); without it the product still exists and is explicit, with \(\|T_k^{\pm1}\|\le2\exp((G+C)\sum u+\dots)\), but the asymptotics (R.15) are not asserted.

**3.11 (volume).** All norms are anchored (M.12, sup over the first anchor) with exponential carrier weights; the one-step constants are volume-uniform by hypothesis (as in Annex AH (DS.3)–(DS.7)); the recursion (3.2) and the fixed point (3.1) contain no volume factor.

**3.12 (why mesoscopic elimination does not prove this).** Annex T §5: M-02 gives conditional means with the bare \(a^{-4}\) budget and no running normalization; its retained marginal is not a Wilson measure at a new coupling. The induction above requires the current-scale budget relative to \(\mathfrak N^{(k)}\), the extraction \(\Pi^{(m)}\) and the contraction (2.5), none of which M-02 supplies.

---
