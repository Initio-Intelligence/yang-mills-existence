# Global Gaussian source families and conditional contraction of the first-order remainder

The Gaussian result applies at all orders to the global energy budget. The interacting order-one conclusion below requires separate local, geometric, regulator and covariance hypotheses. The fixed source radius is taken sufficiently small for convergence of the local polymer expansion.

### 1.1 Setting

Let \(\varphi\in\mathbb R^N\) be a centred Gaussian vector with covariance \(C_0>0\) (the free lattice link field at cutoff \(a\) on the torus; \(N\) is the number of link components). Let the "block fields" be \(\psi_k=B_k\varphi\), \(B_k:\mathbb R^N\to\mathbb R^{N_k}\) surjective and nested (\(B_{k+1}=b_kB_k\)), \(k=0,\dots,K\), \(B_0=I\). Conditionally on \(\psi_k\), \(\varphi\) is Gaussian with mean \(T_k\psi_k\), \(T_k=C_0B_k^T(B_kC_0B_k^T)^{-1}\), and covariance
\[
C_k:=C_0-T_kB_kC_0,\qquad 0=C_0^{\rm cond}\le C_k\le C_{k+1}\le C_K\le C_0 .
\tag{1.1}
\]
Marks: \(n\) centred quadratic forms \(\Phi_l=\varphi^TA_l\varphi-\operatorname{Tr}(C_0A_l)\), \(A_l\) real symmetric (for \(\operatorname{Tr}F^2\) smeared with \(f_l\), \(A_l=\sum_xf_l(x)\,\mathsf s_x\) with \(\mathsf s_x\) the curl–curl stencil at \(x\)). Write \(A(z)=\sum_lz_lA_l\), \(A_l=A_l^+-A_l^-\) with \(A_l^\pm=\sum_x f_l^\pm(x)\mathsf s_x\ge0\) for the curvature stencil; any positive decomposition with the stated bound suffices, and the **insertion size**
\[
\mathfrak a_l:=\|(A_l^+)^{1/2}C_0(A_l^+)^{1/2}\|+\|(A_l^-)^{1/2}C_0(A_l^-)^{1/2}\|,\qquad
\mathfrak a(z):=\sum_l|z_l|\mathfrak a_l,\qquad
\lambda:=\Big(4\sum_l\mathfrak a_l\Big)^{-1}.
\tag{1.2}
\]
For the curvature field \(\mathfrak a_l\le Cg_0^2\|f_l\|_\infty\) uniformly in \(a\), because \(\partial(-\Delta)^{-1}\partial\) is bounded on \(\ell^2\); this is the only place the dimension-four nature of the insertion enters. Let \(E_k(\psi):=\psi^T(B_kC_0B_k^T)^{-1}\psi=(T_k\psi)^TC_0^{-1}(T_k\psi)\) be the coarse Gaussian energy (Annex Y's regulator (M.5) in the free case).

### Theorem 1.1 (exact analytic-family form of the free transported jet)

For \(z\in\mathcal D_\lambda:=\{|z_l|\le\lambda\}\) and every \(k\le K\),
\[
G_k(z;\psi):=\mathbb E\Big[e^{\sum_lz_l\Phi_l}\,\Big|\,\psi_k=\psi\Big]
=\exp\big(\mathfrak L_k(z)+\psi^T\mathfrak B_k(z)\psi\big),
\tag{1.3}
\]
\[
\mathfrak L_k(z)=-\sum_lz_l\operatorname{Tr}(C_0A_l)-\tfrac12\operatorname{Tr}\log\big(I-2C_k^{1/2}A(z)C_k^{1/2}\big),\qquad
\mathfrak B_k(z)=T_k^TA(z)\big(I-2C_kA(z)\big)^{-1}T_k ,
\tag{1.4}
\]
both analytic on \(\mathcal D_\lambda\), with the **uniform field-exponent budget**
\[
\boxed{\ \sup_{z\in\mathcal D_\lambda}\big|\psi^T\mathfrak B_k(z)\psi\big|\le\frac{\mathfrak a(z)}{1-2\mathfrak a(z)}E_k(\psi)\le\tfrac12E_k(\psi)\quad\text{for all }k,K,N.\ }
\tag{1.5}
\]
The one-step map is the exact Möbius recursion
\[
\mathfrak B_{k+1}=t_k^T\mathfrak B_k\big(I-2c_k\mathfrak B_k\big)^{-1}t_k,\qquad
\mathfrak L_{k+1}=\mathfrak L_k-\tfrac12\operatorname{Tr}\log\big(I-2c_k^{1/2}\mathfrak B_kc_k^{1/2}\big),
\tag{1.6}
\]
where \(t_k\psi_{k+1}\) and \(c_k\) are the conditional mean map and covariance of \(\psi_k\) given \(\psi_{k+1}\). Consequently the connected coefficients of order \(m\) in \(z\) of the field-dependent exponent obey, by Cauchy,
\[
\Big|\partial_z^{I}\big(\psi^T\mathfrak B_k(z)\psi\big)\big|_{z=0}\Big|\le m!\,\lambda^{-m}\,\tfrac12E_k(\psi),\qquad|I|=m,
\tag{1.7}
\]
a fixed-factorial budget with exponent \(1\), uniform in \(k,K,N\), relative to the regulator \(E_k\): exactly the shape of the M-03 sup-part (M.11) at grade \(m\), and exactly what [I, Prop 3.8(c)] showed the per-step coefficient iteration **cannot** reproduce.

*Proof.* For a Gaussian vector with mean \(\mu\) and covariance \(C\) and complex symmetric \(A\) with \(\|C^{1/2}AC^{1/2}\|<\tfrac12\), completing the square gives \(\mathbb E e^{\varphi^TA\varphi}=\det(I-2C^{1/2}AC^{1/2})^{-1/2}\exp(\mu^TA(I-2CA)^{-1}\mu)\), the branch of the square root being the one analytic in \(A\) and equal to \(1\) at \(A=0\). Apply this to the conditional law (1.1) with \(\mu=T_k\psi\), \(C=C_k\), \(A=A(z)\); the centring produces the linear term of \(\mathfrak L_k\). For the domain: \(C_k\le C_0\) and \(A_l^\pm\ge0\) give \(\|C_k^{1/2}A_l^\pm C_k^{1/2}\|=\|(A_l^\pm)^{1/2}C_k(A_l^\pm)^{1/2}\|\le\|(A_l^\pm)^{1/2}C_0(A_l^\pm)^{1/2}\|\), hence \(\|C_k^{1/2}A(z)C_k^{1/2}\|\le\mathfrak a(z)\le\tfrac14\) on \(\mathcal D_\lambda\), uniformly in \(k\). For (1.5) put \(w=T_k\psi\), \(u=C_0^{-1/2}w\) (so \(|u|^2=E_k(\psi)\)), \(\tilde A=C_0^{1/2}A(z)C_0^{1/2}\), \(\tilde C_k=C_0^{-1/2}C_kC_0^{-1/2}\in[0,I]\); then \(\psi^T\mathfrak B_k\psi=\sum_{j\ge0}u^T\tilde A(2\tilde C_k\tilde A)^ju\) and \(\|\tilde A\|\le\mathfrak a(z)\) by the same splitting, so the series is bounded by \(\mathfrak a\sum_j(2\mathfrak a)^j|u|^2\). (1.6) is the same Gaussian formula applied to one step (tower property), and composing two Möbius maps of the form (1.6) reproduces the closed form with \(c_k\) added to the covariance, which is (1.1). (1.7) is Cauchy on \(\mathcal D_\lambda\). \(\square\)


The covariance bands can satisfy an operator-order bound on their sum while the sum of their individual operator norms increases proportionally to depth. The Gaussian result uses the exact composition (1.6).

## 2. The analytic-family induction hypothesis and its closure

### 2.1 Objects

Fix finitely many smeared sources \(f_1,\dots,f_n\) (cell-supported \(C^5\) profiles as in [Transport of insertions on a reference torus](../../lattice_theory/insertion_transport.md) §1.4 and the preamble, or any fixed finite test family) and the complex source vector \(z\in\mathbb C^n\). The bare insertion is \(\sum_lz_l\Phi_a(f_l)\), \(\Phi_a(f)=\sum_xa^4f(x)\Phi_{a}(x)\) in the F-01 basis (M.20). The transported jet at scale \(k\) is \(G_k(z;x)=Q_{0\to k}\exp(\sum_lz_l\Phi_a(f_l))(x)\), \(x\) the augmented state of Annex Y §1.

**Definition 2.1 (analytic-family state).** The state at scale \(k\) consists of:
1. the running local coefficients \(t_{\rho,k}>0\), \(v_k\) of [I, Def. 1.1];
2. the **renormalized source** \(\zeta_l:=t_{\rho(l),k}\,z_l\) (channel of the component carried by \(f_l\)) and the fixed polydisc \(\mathcal D_\lambda=\{|\zeta_l|\le\lambda\}\);
3. the c-number counterterm \(\mathfrak L_k(z)\), a polynomial in \(z\) of degree \(\le m_{\max}\) with explicit coefficients (the identity kernels \(C^{(k)}_{I,\mathbf 1}\) of [I, (1.5)–(1.6)]);
4. the local field kernels \(\mathfrak K_k(z;x)=\sum_lz_lt_{\rho,k}e_k(f_l^{(k)})(x)+\sum_{2\le|I|\le m_{\max}}z^I\sum_{P\ne\mathbf 1}C^{(k)}_{I,P}P(x)\), with \(f^{(k)}_l\) the block-averaged profile;
5. the **irrelevant polymer remainder** \(\Psi_k(z;x)=\sum_{X}\Psi_k(X;z;x|_X)\), a sum over connected carriers \(X\) of the scale-\(k\) block graph of activities depending on the state only inside \(X\), each analytic in \(\zeta\in\mathcal D_\lambda\) and in the field variables on the common contour (RM.12)/(E14.49) of Theorems E14.3/R14.3, with \(\Pi^{(m)}_k\Psi_k=0\) coefficientwise (no local polynomial part);

such that, exactly,
\[
G_k(z;x)=\exp\big(\mathfrak L_k(z)+\mathfrak K_k(z;x)+\Psi_k(z;x)\big)
\quad\text{as finite jets of order }\le m_{\max}.
\tag{2.1}
\]
The norm on the remainder is the Kotecký–Preiss type weighted supremum
\[
\|\Psi_k\|_{\kappa,\lambda}:=\sup_{b}\sum_{X\ni b}e^{\kappa|X|}\ \sup_{\zeta\in\mathcal D_\lambda}\ \sup_{x\in\mathcal C_k}\ \frac{|\Psi_k(X;z;x)|}{\widehat R_{h_k,X}(x)},
\tag{2.2}
\]
with \(\widehat R\) the Annex Y regulator (M.6) and \(\mathcal C_k\) the contour. The **analytic-family budget** is
\[
(\mathsf{AF}_k)\qquad\|\Psi_k\|_{\kappa,\lambda}\le\psi_*\quad(\psi_*\ \text{below the KP threshold } \psi_0(\kappa)).
\tag{2.3}
\]
At \(k=0\): \(\Psi_0=0\), \(\mathfrak L_0=0\), \(\mathfrak K_0=\sum_lz_l\Phi_a(f_l)\) with \(t_{\rho,0}=z_{\rho,a,T,\mu}\). The bare \(a^{-4}\) size of \(\Phi_a\) sits entirely in the **local** term \(\mathfrak K_0\), whose one-step image is computed by exact extraction, never by a sup bound of its exponential. This is why no "radius conversion" is needed for the remainder: its radius is \(\lambda\) from the start.

### 2.2 The one-step hypothesis (to be supplied by M-04/M-05/M-06 and H-04; §3)

**(\(\mathsf{OS}_k\)).** There are \(\theta\in(0,1)\), \(\beta_*,C_\Pi<\infty\) and a KP threshold \(\psi_0\), independent of \(k,K,T\), history and \(m_{\max}\), such that for every admitted \(k<K\) and every state satisfying \((\mathsf{AF}_k)\), the full-law one-step operation \(Q_k\) (all sectors, Annex W (4.2)–(4.9)) produces a state of the form (2.1) at scale \(k+1\) with
\[
t_{\rho,k+1}=M_{\rho,k}t_{\rho,k},\quad\|M_k-I-u_k\Gamma\|\le C_4u_k^2;\qquad
\mathfrak L_{k+1},\mathfrak K_{k+1}\ \text{given by the exact extraction } \Pi^{(\le m_{\max})}_{k+1}\log Q_ke^{\mathfrak K_k+\Psi_k};
\tag{2.4}
\]
\[
\boxed{\ \|\Psi_{k+1}\|_{\kappa,\lambda}\le\theta\,\|\Psi_k\|_{\kappa,\lambda}+\beta_* .\ }
\tag{2.5}
\]
Here the logarithm exists because \((\mathsf{AF}_k)\) with \(\psi_*<\psi_0\) puts \(e^{\Psi_k}\) in the KP convergence region on the polydisc (the local part \(e^{\mathfrak K_k}\) is handled by the extraction, not by a smallness condition), and the births in \(\beta_*\) are the irrelevant parts of the collisions of local terms and of the residual history/selector currents.

### Theorem 2.3 (closure at all orders; conditional on \((\mathsf{OS}_k)\) for all \(k<K\))

Let \(\psi_*:=\beta_*/(1-\theta)\) and suppose \(\psi_*<\psi_0\). Then \((\mathsf{AF}_k)\) holds for every \(k\le K\) with the same \(\psi_*\), uniformly in \(K\), the torus and the history. Consequently, for every \(|I|=m\le m_{\max}\), the irrelevant connected coefficient satisfies
\[
\sup_b\sum_{X\ni b}e^{\kappa|X|}\sup_{x\in\mathcal C_k}\frac{|\partial_z^I\Psi_k(X;0;x)|}{\widehat R_{h_k,X}(x)}
\le m!\,\lambda^{-m}\prod_{i\in I}t_{\rho(i),k}\ \psi_* ,
\tag{2.6}
\]
i.e. the M-03 budget [I, (B_k)] relative to the explicit normalization [I, (1.6)] with **factorial exponent \(p=1\)** and no logarithmic accumulation; the local kernels \(\mathfrak L_k,\mathfrak K_k\) are explicit; and the terminal remainder is [I, Prop 3.7].

*Proof.* Induction on \(k\): \(\Psi_0=0\le\psi_*\); if \(\|\Psi_k\|\le\psi_*\) then (2.5) gives \(\|\Psi_{k+1}\|\le\theta\psi_*+\beta_*=\psi_*\). No partition sum, no product of lower-order budgets and no per-order constant occur: the births are already summed inside \(\beta_*\) as a sup over the polydisc. (2.6) is Cauchy in \(\zeta\) on \(\mathcal D_\lambda\) followed by \(\partial_{z_l}=t_{\rho(l),k}\partial_{\zeta_l}\). Uniformity in \(K\), volume and history is inherited from the constants of \((\mathsf{OS}_k)\). \(\square\)


**Remark 2.5 (comparison with [I, Thm 3.6]).** The coefficient-norm closure needed (G3-strong) with \(\sum_k\varepsilon_k<\infty\), false in the M-03 norm (Cor. 1.2). The analytic-family closure needs only (2.5). The price is that \((\mathsf{OS}_k)\) must be proved for the exponent on a complex polydisc **and** on the field contour, i.e. in Bałaban's inductive space (CMP 119 p. 262, second remark: "RT transforms the space with the index \(k\) into the space with the index \(k+1\)"), which is precisely the form in which E14.3/R14.3 are already proved for the source-free E/R activities.

---

### Lemma 9.1 (the extraction F-06a at orders \(m=1,2\); exact recursions)

Define \(\Pi^{(\le)}_{k+1}\) on an activity \(\Phi(X')(V';z)\) analytic in the coarse variables \(F_P\), \(P\in X'\), as the removal of the Taylor monomials at \(x_*\) of (a) field degree \(r=0\) (pure source polynomials: the **identity kernels**, any \(j\)), and (b) field degree \(r=2\) with \(j=0\) (block-averaged sources times a quadratic form in the \(F_P\), \(P\in X'\)); the quadratic form is further split into its diagonal/clover part, which is the span of the 21 fields \(e_{k+1,\beta}\) at the anchor, and its separated part \(\sum_{P\ne P'}Q_{PP'}F_PF_{P'}\), which is kept as a (nonlocal, dimension-four) remainder. Then \(\mathcal L^{(m)}_{k+1}\) of Definition 2.1 is \(\mathrm{span}\{\mathbf 1\cdot(\text{source monomials}),\ \bar f^{\,m}e_{k+1,\beta}\}\), and the local kernels obey, exactly,
\[
\mathfrak L_{k+1}(z)=\mathfrak L_k(z)+\Delta\mathfrak L_k(z),\qquad
\Delta\mathfrak L_k(z)=\big[\Pi^{(\le)}_{k+1}\log Q_ke^{\mathfrak K_k+\Psi_k}\big]_{r=0},
\tag{9.1}
\]
\[
m=1:\quad t_{\rho,k+1}=M_{\rho,k}t_{\rho,k},\qquad
m=2:\quad c^{(k+1)}_{2,\beta}=M_{\rho(\beta),k}\,c^{(k)}_{2,\beta}+b^{(k)}_{2,\beta},
\tag{9.2}
\]
where \(c^{(k)}_{2,\beta}\) is the coefficient of \(\bar f^{\,2}e_{k,\beta}\) in \(\mathfrak K_k\), \(M_{\rho,k}\) is the one-field ratio of [I, (1.3)] (the same number for every monomial carrying \(e_\beta\), by linearity of \(Q_k\) and equivariance), and \(b^{(k)}_{2,\beta}:=\big[\Pi^{(\le)}_{k+1}\kappa_{Q_k}(\text{two linear insertions})\big]_{\bar f^2e_\beta}\) is the extracted degree-two, order-two collision. Equivariance makes (9.2) channel-diagonal.

*Proof.* The Taylor expansion of an analytic function of finitely many \(F_P\) at \(x_*\) is unique, so \(\Pi^{(\le)}\) is a well-defined linear projection commuting with the \(H_4\) action and with the block-average structure of the sources. Degree-\(0\) monomials are \(V'\)-independent, hence \(Q_k\)-invariant up to the extracted collisions, giving (9.1). For \(m=1\), the coefficient of \(z_l\) in \(\mathfrak K_k\) is \(t_{\rho,k}\bar f_le_{k,\cdot}\); its image under \(Q_k\) has \(r=2,j=0\) part \(M_{\rho,k}t_{\rho,k}\bar f_le_{k+1,\cdot}\) by [I, Lemma 1.1] (the \(r\ge3\) and \(j\ge1\) parts are not extracted). For \(m=2\), the coefficient of \(z_lz_{l'}\) in \(\log Q_ke^{\mathfrak K_k+\Psi_k}\) is \(Q_k[c^{(k)}_{2,\beta}\bar f\bar f'e_{k,\beta}]+\kappa_{Q_k}(t\bar fe,t\bar f'e)+(\text{terms with }\Psi_k)\); the first has \(r=2,j=0\) part \(M_{\rho,k}c^{(k)}_{2,\beta}\bar f\bar f'e_{k+1,\beta}\) by the same lemma; the second's extracted part is \(b^{(k)}_{2,\beta}\); terms with \(\Psi_k\) have no \(r\le2,j=0\) content at scale \(k\) by the induction hypothesis, but their transported images can acquire an \(r=2,j=0\) part at scale \(k+1\) only through the separated-to-local merging of Theorem 9.2(c) below, which is included in \(b^{(k)}_{2,\beta}\). \(\square\)

**Remark 9.1a (free-field check of (9.2)).** In the free case \(b^{(k)}_{2,\beta}\) is the zeroth Taylor moment of \(F_x\,C^F_k(x-y)\,F_y\) in \(y\) around \(x\), with \(C^F\) the curvature covariance. In the continuum \(C^F_{\mu\nu,\rho\sigma}(y)=(\partial_\mu\partial_\rho\delta_{\nu\sigma}-\dots)G(y)\), \(G\) harmonic away from \(0\), so every angular average \(\oint\partial_\mu\partial_\rho G=\tfrac14\delta_{\mu\rho}\oint\Delta G=0\): the free composite kernel \(\bar f^2e_\beta\) receives **no** logarithm, only an \(O(1)\) lattice-artifact contribution from \(|x-y|\lesssim a\) and nothing from scales \(j\ge1\). This is consistent with Theorem 1.1 (the free exponent is bounded on a fixed polydisc) and shows that the running of the \(m\ge2\) composite kernels is an interaction effect, \(b^{(k)}_{2,\beta}=O(u_k)\) in the interacting theory; (9.2) then runs like Annex P (R.18)–(R.20) with an additive \(O(u_k)\) source, i.e. a further explicit logarithmic power. These kernels are explicit outputs; they are **not** bounded uniformly and are not claimed to be.

## Order-one contraction at fixed block parameters

Fix admissible block parameters L and M. Assume the age-n real-centre and relative second-order curvature transfer with exponential tails, (I2), (I3), a common hull-regular contour on the small carriers, transverse complex regulator control, the sector hypotheses and the Kotecký–Preiss smallness region. The separated-carrier improvement additionally requires translation covariance of the extracted coefficient and the stated physical first-difference estimate. All constants in the following estimate may depend on L and M.

For the n-step composition with extraction at its terminal scale, one has

\[
\|\Psi^{(1)}_{k+n}\|_{\varkappa,\lambda}\le \theta_n \|\Psi^{(1)}_k\|_{\varkappa,\lambda}+nC^\prime(L,M)\beta_*.
\]

The separated-within-block bilinear row has \(L^{4n}\) (block count) \(\times\) \((L^{-2n})^2\) (two curvature factors) \(\times\) \(L^{-n}\) (one fine difference, (12.2)) \(=L^{-n}\), which gives the following estimate:
\[
\theta_n=C_R(L,M)\,n\,L^{4n}\Big[\frac{(2C_\Psi'L^{-2n})^3}{1-2C_\Psi'L^{-2n}}+C_{\rm sep}L^{-5n}\Big]
+L^{4n}C_RC_\Psi'^{2}\,B_dA_d^{\,C_{L^n}}e^{-(\varkappa-\log A_d)(1-C'/L^n)C_{L^n}/2}
\ \lesssim\ C(L,M)\big(nL^{-2n}+nL^{-n}\big)+e^{-c\varkappa L^n},
\tag{13.1}
\]
so \(\theta_n\to0\) and \(n_0(L,M)\) exists; for the displayed entropy bound one chooses \(\varkappa\) with a strict margin above \(3\log A_d\) and then \(n\) large enough that \((\varkappa-\log A_d)(1-C^\prime/L^n)>2\log A_d\). This absorbs the explicitly displayed \(A_d^{C_{L^n}}\). The source decoupling radius must leave room for this choice and the intermediate-step window below.

### 13.2 Carrier weights over the \(n\) intermediate steps: symbols and the window

Symbols: \(\varkappa\) is **M-07's carrier weight** in the norm (2.2) (also denoted \(\kappa\)); \(\kappa_1\) is Bałaban's decoupling radius (E14.5); \(\kappa_*\) the activity decay rate of E14.3/R14.3; \(\kappa_{\rm KP}\) the Kotecký–Preiss loss per cluster step (a universal constant, \(\kappa_{\rm KP}\le1\) for the weight \(e^{\varkappa|X|}\) with \(a(X)=|X|\)).

*Per intermediate step \(i<n\).* The activities after step \(i\) live on scale-\((k+i+1)\) carriers. Two facts: (i) **reblocking never loses weight**: every fine block lies in exactly one coarse block, so \(|X^{(i+1)}|\le|X^{(i)}|\) and \(e^{\varkappa|X^{(i+1)}|}\le e^{\varkappa|X^{(i)}|}\) for every carrier, small or large (the Bałaban bound \(|X'|\le C_d+C'|X|/L\) of (11.3) is used only to obtain a *gain* for \(|X|\ge C_L\); the factor \(e^{\varkappa C_d}\) in (11.3) is therefore not a loss and is replaced by the trivial bound for small carriers); (ii) the decoupling tails of step \(i\) (rate \(\kappa_1\)) are summable against the weight \(e^{\varkappa|\cdot|}\) iff \(\varkappa<\kappa_1-\log A_d\), with no loss of rate; the cluster/KP step loses \(\kappa_{\rm KP}\). Hence the weight sequence is
\[
\varkappa_0=\varkappa,\qquad \varkappa_{i+1}=\varkappa_i-\kappa_{\rm KP}\quad(i<n),\qquad \varkappa_n=\varkappa-n\kappa_{\rm KP},
\tag{13.2}
\]
and the extraction at scale \(k+n\), together with the reblocking gain (11.3) for \(|X|\ge C_{L^n}\), restores \(\varkappa\) provided the entropy sums converge at the end, i.e. \(\varkappa_n>\log A_d\). The **window** is therefore
\[
\log A_d+n_0\kappa_{\rm KP}\ <\ \varkappa\ <\ \kappa_1-\log A_d .
\tag{13.3}
\]
*Non-circularity.* \(n_0=n_0(L,M)\) is determined by (13.1), whose constants \(C_R,C_\Psi',C_{\rm sep}\) come from (I-L/n) and (I3) **at \(s\equiv1\)** (the physical minimizer and the one-scale fluctuation covariance), hence do **not** depend on \(\kappa_1\); the decoupling bound \(K=B_0e^{16\kappa_1}\) enters only the births \(\beta_1\) of Theorem 8.1 and the KP constant, not \(\theta_n\). So the order is: fix \((L,M)\); fix \(n=n_0(L,M)\); fix \(\varkappa\) with \(\varkappa>\log A_d+n_0\kappa_{\rm KP}\); fix \(\kappa_1>\varkappa+\log A_d\) (compatible with Bałaban's "\(\kappa_1\) large" and the parameter order of B-03 in §19.3 of [homogeneous_projection.md](../../coupling/homogeneous_projection.md), which also needs \(\kappa_1\ge16\kappa+1\)); then \(K\) is fixed; then \(\lambda\) small enough that \(C(L,M)^{n}\,n\,C'\beta_*(\lambda,K)/(1-\theta_n)<\psi_0(\varkappa)\); then the coupling ceiling. (13.3) is non-empty and there is no cycle. If, contrary to the reading in §12.2(b), the constants in (13.1) did depend on \(\kappa_1\) (through the localized \(C_H\)), the window would require \(n_0(\kappa_1)\kappa_{\rm KP}<\kappa_1-2\log A_d\), i.e. \(n_0\) sublinear in \(\kappa_1\): with \(C_\Psi'\propto e^{c\kappa_1}\) one gets \(n_0\asymp c\kappa_1/\log L\) and the window is non-empty iff \(L>e^{c\kappa_{\rm KP}}\), a condition on the fixed \(L\) — still not circular, but it would make \(L_1\) depend on the (unknown) \(c\). This is why (I-L/n) is stated at \(s\equiv1\).

### 13.3 Translation covariance behind the extra \(L^{-1}\) in Lemma 9.3(b) / Theorem 11.4(b)

The extraction of \(\sum_{p\subset P}F_p^2\) as the local clover \(e_{k+n,\beta}(P)\) plus terms of dimension \(\ge6\) uses the cancellation of the linear term \((x_p-c_P)\cdot\nabla F\) when summed over the positions \(p\subset P\) (symmetric block, \(L^n\) odd), and the identification of the resulting coefficient with the **same** number for every block. The first is geometric; the second requires

**(TC) translation covariance.** On the clean sector, \(\Psi_{k\leftarrow k+n}\) commutes with translations by scale-\((k+n)\) lattice vectors and with the block reflections; equivalently the extraction coefficient \([\Pi^{(1)}_{k+n}Q^{(n)}_ke_{k}]_{e_{k+n,\beta}}\) is independent of the anchor block. *Source:* the Euclidean covariance of the inductive assumption, CMP 119 (2.29), restated for the layer functions on p. 275 ("when defined on the whole lattice, it is Euclidean covariant"); it holds on the homogeneous clean sector and fails on sectors with large-field geometry, where the extraction coefficient becomes sector-dependent — exactly the sector-dependent \(t_{\rho,k,h}\) of §10.1. (TC) is added to the hypotheses of Theorem 11.4.


Choose a fixed n with contraction factor below one, followed by the carrier weight and decoupling radius in the stated window. Taking the source radius sufficiently small puts the uniform block-end bound nC′β*/(1−θₙ) and the finitely many intermediate bounds inside the convergence region. This gives the uniform first-order result conditional on the required physical inputs. At order two and above the extraction recursion for composite sources must be shown compatible with their renormalization. The full-law applications also require selector flux and the marked reset quotient.
