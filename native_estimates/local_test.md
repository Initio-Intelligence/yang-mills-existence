# A local test for the exterior retained field

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

**Local-chart hypotheses.** In every application use (A8′) in the structured form 3′ and 4′, F(4′) on (Avg), (Sm3′), (Par-g_Z′), and (Lay-W), with $M_W\mid M_1$ and $M_1\ge6M_W$. In particular the per-potential rate must satisfy $\kappa_1/2\ge\sqrt d(1+3\beta)\kappa/(1-3\delta)$. The bound on the joint terminal law requires the action estimate and item 4′.

## 1. Source facts used

All (c) unless marked.

**S1. The three tests.** [III] p.265: (3.2) P-test with \(U_{k+1,\square'}\); (3.3) Q-test \(\chi(\{\sup_{b\in(\square'^{\sim2})^{(k)*}}|V_k(b)(V^{(k)}_{\square'}conditional)^{-1}-1|<2\delta_k\})\) on \(L^2M_2R_{k+1}\)-cubes \(\square'\subset(B^{k+1}(P^1_{k+1}))^{\sim-1}\); (3.4) \(V^{(k)}_{\square'}=M^k(U_{k+1,\square'})\); \(\delta_k=g_kA_1A_0^{-1}p_0(g_k)\). p.268, (3.16): the R-test on cubes \(\square'\subset\Omega_{k+1}^{\sim-1}\), printed \(|A_k(b)|<\delta_k\); the first step prints \(|A(b)|<g_0^{-1}\delta_0\), (1.18) p.250, and [IV] (1.9) p.178 prints \(|A_j(b)|<g_j^{-1}\delta_j\). Use \(t_k:=\delta_k/g_k\) (the representation convention).

**S2. Starred sets.** p.247, (1.9): \(X^*=X\setminus\{b_0(c):c\in X^{(1)}\}\). p.249: "the linearizing transformation is different from the identity only on bonds \(\{b_0(c)\}\)". Hence on starred bonds of \(\Omega_{k+1}\) the full fluctuation \(g_kCA_k-h\tilde D(g_kCA_k)\) of (3.15) equals \(g_kA_k(b)\), and \(V_k(b)=e^{ig_kA_k(b)}V^{(k)}(b)\).

**S3. Why Bałaban wants (3.16).** p.268: "the characteristic functions \(\chi'_k\) depend now on the field \(V^{(k)}\), hence on the new field variables \(V_{k+1}\) on the whole set \(\Gamma_{k+1}\). We want to have characteristic functions depending on the fluctuation field only". p.250: the two invariances, under \(V\to V^v\) with \(A\to R(u_0)A\), and under (1.17).

**S4. The comparison (3.17)–(3.19)**, p.268:
\[
U_{k+1}=U\bigl(\mathbf B_{k+1}(\square'^{\sim4}),[M^\cdot(U_{k+1})(M^\cdot(Q^{s*}_{k+1}V_{k+1}))^{-1}]M^\cdot(Q^{s*}_{k+1}V_{k+1})\bigr)=\Bigl(\exp iL^{-1}\eta\mathbf H_{k+1,\square'}\bigl(\tfrac1i\log[\cdots]\bigr)U_{k+1,\square'}\Bigr)^{u^{-1}_{k+1,\square'}},
\]
"the argument of the function \(\mathbf H_{k+1,\square'}\) is bounded by \(44d^2B_3\varepsilon_{k+1}\), and has a support in a boundary layer of the width \(2LM_1\) at the boundary of \(\square'^{\sim4}\). Thus, the function \(\mathbf H_{k+1,\square'}\) is bounded by \(B_3\exp(-\delta LM_2R_{k+1})44d^2B_3\varepsilon_{k+1}\le44d^2B_3^2(1+\beta_0)\exp(-R_k)\varepsilon_k\) on \(\square'^{\sim2}\)"; (3.18) \(V^{(k)}(b)=u^{-1}_{k+1,\square'}(b_-)\exp i\tilde Q_k(L^{-1}\eta\mathbf H_{k+1,\square'})\tilde R^ku_{k+1,\square'}(b_+)V^{(k)}_{\square'}(b)\); "These facts, and the bounds (106)–(108), (159)–(163) in [12], imply" (3.19) \(|V^{(k)}(b)(V^{(k)}_{\square'}conditional)^{-1}-1|<O(1)44d^2B_3^2(1+\beta_0)\frac{A_0}{A_1}e^{-R_k}\delta_k<\delta_k\). The same representation with the two configurations in the other order is (3.6), p.266. The decay is "the exponential decay property (190) [15]" (p.266).

**S5. Determining sets.** p.256: "Consider a domain \(\Omega\) such that it is a union of \(M_1\)-cubes in the lattice \(T_\xi\), \(\xi=L^{-j}\). For this domain we build a minimal determining set with a support in \(\Omega\), or a sequence of maximal domains \(\Omega=\Omega_0\supset\Omega_1\supset\dots\supset\Omega_j\) such that \(\Omega_n\) is a union of \(L^n\xi M_1\)-cubes, and \({\rm dist}(\Omega_n,\Omega^c_{n-1})\ge L^n\xi M_1\) … \({\rm dist}(\Omega_j,\Omega^c)\le2M_1\)". So \(\mathbf B_j(\Omega)\) exists for every union of \(M_1\)-cubes, not only for unions of partition cubes. p.257, (2.16): \(U_{k,\square}(V_k)=U(\mathbf B_k(\square^{\sim4}),M^\cdot(Q^{s*}_kV_k))\).

**S6. The classes.** p.259: properties (i)–(iv) of \(\mathbf E^{(j)}(X,U_k,z)\): "(i) it depends on \(U_k\) restricted to \(X\); (ii) there exists an analytic function \(\mathbf E^{(j)}(X,(\mathbf U,\mathbf J),z)\) of the variables \((\mathbf U,\mathbf J)\in U^c_j(X,\alpha_{0,j},\alpha_{1,j})\), which is an extension of this term …; (iii) the extended function is invariant with respect to the gauge transformations (I.1.10)"; (2.28) \(\alpha_{0,j}=g_jC_0(\log g_j^{-2})^{q_0}\), \(\alpha_{1,j}=g_jC_1(\log g_j^{-2})^{q_1}\). p.260: R-terms have "the properties (i)–(iii) formulated above", the bound (2.31) \(|\mathbf R^{(j)}(X,(\mathbf U,\mathbf J))|\le g_j^{\kappa_0}\exp(-\kappa d_j(X))\) with "\(\kappa_0\) can be chosen arbitrarily large", the vacuum subtraction (2.30), and the covariance (2.32) "for these Euclidean transformations \(r\), which leave the partition of the lattice \(T_\xi\) in \(MR_j\)-cubes invariant". p.261: the spaces \(\tilde U^c_j(X,\tilde\alpha_0,\tilde\alpha_1)\), (2.34)–(2.39); their definition contains the configurations \(U_{p,X}(M^\cdot(\mathbf U))=U(\mathbf B_p(X)\cup\{\Gamma_i\}_{i<p},M^\cdot(\mathbf U))\). p.261, (2.41)–(2.42): B-terms are indexed by \(X\in\mathbf D_j\) with \(X\cap\Omega_j\ne\emptyset\), \(X\cap Z_j^\sim\ne\emptyset\), bound \(B_0e^{-\kappa d_j(X)}\). [I] p.263, (1.19): invariance "for all \(G^c\)-valued gauge transformations \(u\)". The linear size \(d_j(X)\) is the length of a shortest tree meeting all \(M\)-cubes of \(X\), divided by \(M\) ([I] §0, source); [II] (2.30) (source): \((3^{23})^{-1}M^{-4}|Y|\le d_k(Y)\le M^{-4}|Y|-1\). So \(d\) is comparable to the number of \(M\)-cubes.

**S7. The source's bookkeeping in the fluctuation integral.** p.271: "Introduce now auxiliary parameters \(s,t\), the parameter \(t\) multiplying the expressions \(\mathbf B_k\), \(A((1/g_k^2(\cdot))-(1/g_k^2),\dots)\), \(V^{(k)}\), \(s\) multiplying \(\mathbf R''_k\)"; (3.26); "The first is the integral over \(t\) of the expectation value of the boundary terms, and it contributes to \(\mathbf B^{(k+1)}\) only. The second is the integral over \(s\) of the expectation value of the R-terms, and it contributes to \(\mathbf R^{(k+1)}\) and \(\mathbf B^{(k+1)}\). The third expression is the logarithm of the fluctuation field integral involving the regular terms of the effective action only". pp.270–271: \(\mathbf R'_k=\sum_{j\le k_1}\mathbf R^{(j)}\), \(k_1\) the largest integer with \(L^{-(k-k_1)}MR_j\le L\), "has the same covariance property as the expression determined by \(\mathbf E_k\), and we include it into \(\mathbf E_k\)". p.279 (source): "The expansion (3.47) for the second expectation value in (3.26) is divided into two parts. The terms with localization domains contained in \(\Lambda_{k+1}\) have the same important property as the corresponding \(\mathbf E^{(k+1)}\)-terms, namely they do not depend on \(\Lambda_{k+1}\). We denote them by \(\mathbf R''^{(k+1)}\) … The remaining terms are included again into the boundary term."

**S8. Extension of \(\mathbf H\)-functions to the spaces.** [I] p.273: "we substitute \(\mathbf A=\mathbf H_j(B(t))+t_\square\langle\dots\rangle\), with functions \(\mathbf H_j,\mathbf H_k\) depending on \(\mathbf U,\mathbf J\). These functions are given by (179), (180) [15], and we replace the configurations \(U_{k+1},J_{k+1}\) occurring in operators there by the configurations \(\mathbf U,\mathbf J\)."

**S9. Localized form of the fluctuation action.** [II] Lemma 2 (source): \(\mathbf P^{(k)}(g_k,U_{k+1},B)+\{\dots\}=\sum_{Y\in\mathbf D_k}\mathbf V_k(Y,U_{k+1},B)\), each term analytic on \(U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\times\{B:|B|<\varepsilon_1g_k^{-1}\text{ on }Y\}\), \(\mathbf V_k=\frac12\langle B,\mathbf V^{(2)}_k(Y)B\rangle+\mathbf V''_k(Y,B)\) with (1.43), (1.36), gauge invariant. [III] p.276: the same with the covers of the sequence \(\{\Omega_j\}\) and the space (3.43) \(\tilde U^c_{k+1}(Y,(1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1)\times\{A:{\rm supp}A\subset Y\cap\Lambda^{(k)*}_{k+1},|A|<C_1p_1(g_k)\}\); "The expression determined by \(\mathbf R_k\) is treated in exactly the same way as \(\mathbf E_k\), except the second renormalization". The decoupling device is [II] (1.9)–(1.18): \(s\)-dependent propagators, analytic for \(|s(\Delta)|\le e^{\kappa_1}\), kernels vanishing unless both arguments lie in one component, and the bound (1.18) \(|\mathbf H_k(s(Y_0),B')|\le4B_0e^{16\kappa_1}|B'|\) on the polydisc.

**S10. Large-field factors.** [LFR II] p.380: "The function \(\chi'^c_j(Q_j)\) yields the factor \(\exp(-\frac12\gamma_0\frac1{g_j^2}(2\delta_j)^2(LM_2R_j)^{-2}|Q_j|)\), by expanding the Wilson action locally in the approximate fluctuation field, and using the positivity bound for the resulting quadratic form. The characteristic function \(\chi^{(j-1)c}(R_j)\) yields the factor \(\exp(-\gamma_0\frac1{g_j^2}\delta_j^2(LM_2R_j)^{-d}|R_j|)\), by the same positivity bound for the quadratic form."

## 2. Definition of the amended one-step map

Notation of [III] §3 throughout. The step is \(V_k\to V_{k+1}\). Lengths are in units of the lattice \(T^{(k)}\) unless said otherwise. \(\pi'\) is the partition into cubes \(\square'\) of side \(L^2M_2R_{k+1}\) (side \(LM_2R_{k+1}\) in \(T^{(k+1)}\)-units). The operation \(\sim\) on these cubes adds one layer of sub-cubes of side \(LM_2R_{k+1}\) ("sublayers").

### 2.0 Standing parameter conditions (Par)

* **(Par-c)** The partitions \(\pi'\), the sub-cube partition, the \(MR_{k+1}\)- and \(M\)-partitions and the block partitions are nested regular subdivisions with common symmetry planes (the source's "compatible", [III] pp.245, 265, read as in FS §3.4).
* **(Par-M)** \(M\ge(L+8)M_2\). (The source: "\(M\) will be chosen much larger than \(M_2\)", p.245.)
* **(Par-g)** The coupling ceiling \(\gamma\) is so small that, for all \(j\), \(C_\star\,p_1(g_j)^2\,\ell_j^{q}\,e^{-c_\star R_j}\le g_j^{\kappa_0+2}\), where \(\ell_j=\log g_j^{-2}\), \(q=\max(q_0,q_1)\), and \(C_\star,c_\star\) are the constants of Lemma 3.4. This is possible because \(R_j\ge\ell_j^{\,r}\), \(r\ge2\) ([III] p.245), so \(e^{-c_\star R_j}\le\exp(-c_\star\ell_j^2)\).

### 2.1 The box of a bond

Let \(\mathfrak B_{k+1}\) be the set of bonds \(b\) of \(T^{(k)}\) with \(b\in(\square'^{\sim2})^{(k)*}\) for some \(\square'\in\pi'\), \(\square'\subset\Omega_{k+1}^{\sim-1}\). These are the bonds on which the source's (3.16) tests \(A_k\).

**Definition 2.1.** For a bond \(b\) of \(T^{(k)}\),
\[
\square_b:=\bigcup\{\square''\in\pi':\ b\text{ has an endpoint in }\square''^{\sim2}\}.
\]

**Lemma 2.1 (properties of the boxes).** Assume \(L\ge5\).
* (B1) \(\square_b\) is a rectangular union of at most \(2^d\) cubes of \(\pi'\).
* (B2) If \(b\in(\square''^{\sim2})^*\) then \(\square''\subset\square_b\), and \({\rm dist}(b,(\square_b^{\sim4})^c)\ge2LM_2R_{k+1}-1\).
* (B3) \(\square_{rb}=r\square_b\) for every lattice isometry \(r\) mapping \(\pi'\) to itself.
* (B4) \(\square_b^{\sim4}\) lies within \(\ell^\infty\)-distance \((L+6)LM_2R_{k+1}\) of \(b\).
* (B5) Under (Par-M): for \(b\in\mathfrak B_{k+1}\), \(\square_b^{\sim4}\subset\Omega_{k+1}\); for \(b\in\mathfrak B_{k+1}\) with an endpoint in \(S_{k+1}^{\sim2}\), \(\square_b^{\sim4}\subset\Lambda_{k+1}^c\).

*Proof.* Coordinate-wise, a site lies in \(\square''^{\sim2}\) for one or two adjacent cubes, two exactly when it is within two sublayers of a face (\(4\le L\)). The two endpoints of \(b\) differ in one coordinate by one unit, so the union is a product of intervals of one or two cubes: (B1). (B2): \(\square''^{\sim4}\subset\square_b^{\sim4}\) and an endpoint of \(b\) is in \(\square''^{\sim2}\). (B3): the definition uses only \(\pi'\) and \(\sim\). (B4): per coordinate the box reaches at most \(L+2\) sublayers from \(b\). (B5): \(\Omega^{\sim-1}_{k+1}\) is one layer of \(LMR_{k+1}\)-cubes inside \(\Omega_{k+1}\), width \(LMR_{k+1}\ge(L+8)LM_2R_{k+1}\); \(S_{k+1}\) and \(\Lambda_{k+1}\) are separated by one such layer ((3.20)). \(\square\) 

*Remark (other boxes).* Any assignment \(b\mapsto\square_b\) of unions of \(M_1\)-cubes with (B2)–(B5) works in everything below; by S5 the box need not be a union of partition cubes (FS (M4) and its criticism of TC's box are not forced). Retain Definition 2.1 because it makes (3.17)–(3.19) apply with \(\square'\) replaced by \(\square_b\) and nothing else changed.

### 2.2 The local background, the local fluctuation, the test

**Definition 2.2.** For \(b\in\mathfrak B_{k+1}\), following (2.16) and (3.4),
\[
U_{k+1,b}:=U\bigl(\mathbf B_{k+1}(\square_b^{\sim4}),M^\cdot(Q^{s*}_{k+1}V_{k+1})\bigr)\ \text{(axial gauge)},\qquad V^{(k)}_b:=M^k(U_{k+1,b}),\qquad A^{\rm loc}_k(b):=\frac1{ig_k}\log\bigl(V_k(b)\,V^{(k)}_b(b)^{-1}\bigr).
\]
The amended decomposition of unity, replacing (3.16) (and (1.18) for \(k=0\)):
\[
1=\sum_{R_{k+1}}\ \prod_{\square'\subset R^c_{k+1}}\chi\Bigl(\Bigl\{\sup_{b\in(\square'^{\sim2})^{(k)*}}|A^{\rm loc}_k(b)|<t_k\Bigr\}\Bigr)\prod_{\square'\subset R_{k+1}}\chi\Bigl(\Bigl\{\sup_{b\in(\square'^{\sim2})^{(k)*}}|A^{\rm loc}_k(b)|\ge t_k\Bigr\}\Bigr)=\sum_{R_{k+1}}\chi^{{\rm loc}(k)}(R^c_{k+1})\chi^{{\rm loc}(k)c}(R_{k+1}),
\tag{3.16\(^{\rm loc}\)}
\]
\(t_k=\delta_k/g_k\), the sum over unions \(R_{k+1}\subset\Omega^{\sim-1}_{k+1}\) of cubes of \(\pi'\), exactly as in (3.16). \(|\cdot|\) is an Ad-invariant norm on \(\mathfrak g\).

The label of \(\square'\) is a function of \(V_k\) on \((\square'^{\sim2})^*\) and of \(V_{k+1}\) on \(\bigcup_b\square_b^{\sim4}\), by Definition 2.2 and (2.16). It is the Q-test (3.3) at the threshold \(\delta_k\) with the bond's box in place of the cube.

### 2.3 The local chart

On \(\Omega_{k+1}\) the source writes \(V_k(b)=e^{ig_kA_k(b)}V^{(k)}(b)\) on starred bonds (S2), \(V^{(k)}=M^k(U_{k+1})\), (3.10)–(3.11). Put
\[
e^{i\mathbf H_b}:=V^{(k)}(b)\,V^{(k)}_b(b)^{-1}\qquad(b\in\mathfrak B_{k+1}),
\tag{2.1}
\]
the convention of (3.22). Then \(e^{ig_kA^{\rm loc}_k(b)}=e^{ig_kA_k(b)}e^{i\mathbf H_b}\), that is
\[
A_k(b)=\varphi_{\mathbf H_b}(A'conditional):=\frac1{ig_k}\log\bigl(e^{ig_kA'(b)}e^{-i\mathbf H_b}\bigr)=A'(b)-a_b(A'conditional,\mathbf H_b),\qquad A'conditional:=A^{\rm loc}_k(b),
\tag{2.2}
\]
\(a_b(A',\mathbf H)=g_k^{-1}\mathbf H+g_k^{-1}\mathbf F(g_kA',-\mathbf H)\). This is (1.22) with \(g\equiv1\) and \(\mathbf H_{1,Ax}\) replaced by \(\mathbf H_b\).

**Definition 2.3 (chart).** The integration variables on the starred bonds of \(\Omega_{k+1}\) are \(\tilde A\):
* for \(b\in\mathfrak B_{k+1}\): \(\tilde A(b)=A^{\rm loc}_k(b)\), i.e. \(V_k(b)=e^{ig_k\tilde A(b)}V^{(k)}_b(b)\);
* for the remaining starred bonds of \(S_{k+1}\) (they lie in \(\Omega_{k+1}\setminus\Omega^{\sim-1}_{k+1}\)): the source's variable of (3.22), second form, i.e. \(V_k(b)=e^{ig_k\tilde A(b)}V^{(k)}_{\Lambda^c_{k+1}\cap\Lambda_k}(b)\), \(\mathbf H^{(k)}\) as in (3.22), cutoff replaced by 1 as the source itself does there.

Write \(A_k=\Phi(\tilde A)\) for the resulting bondwise map. The cutoff function \(g(A')\) of (1.22) is not used anywhere.

*Why the outermost bonds keep the source's chart.* For a starred bond of \(\Omega_{k+1}\setminus\Omega^{\sim-1}_{k+1}\) not in \(\mathfrak B_{k+1}\) the box may leave \(\Omega_{k+1}\). There \(U_{k+1}\) is not critical for the box problem and \(\mathbf H_b\) would be \(O(\varepsilon_k)\), not \(e^{-R}\)-small. On these bonds there is no R-test, so nothing forces the local chart. This is FS (M5), with its reason.

**Lemma 2.2 (the chart is a Haar-preserving reparametrization).** For real \(\mathbf H\) and \(|g_kA'|,|\mathbf H|\) below the injectivity radius of \(\exp\), let \(\sigma\) be the density of Haar measure in exponential coordinates, \(d(e^{iX})=\sigma(X)dX\). Then
\[
\sigma\bigl(g_k\varphi_{\mathbf H}(A')\bigr)\,\Bigl|\det\frac{\partial\varphi_{\mathbf H}(A')}{\partial A'}\Bigr|=\sigma(g_kA').
\]
*Proof.* In the group variable \(W=e^{ig_kA}\), (2.2) is the right translation \(W=W'e^{-i\mathbf H}\), which preserves Haar measure. \(\square\) (Numerical check for SU(2):  item 1, relative error \(10^{-9}\).)

Consequences. (1) The amended construction does not change the integral: on each bond it uses the base point \(V^{(k)}_b(b)\) instead of \(V^{(k)}(b)\) to coordinatize the same Haar-distributed \(V_k(b)\). Positivity of every term of the expansion is untouched (B-01). (2) With \(g\equiv1\) the Jacobian (1.24) is exactly the change of the Haar-density term \(\sum_b\log\sigma(\cdot)\) of (1.14); the two cancel. The argument does not use this cancellation (the general step hides the \(\sigma\)-term inside \(\mathbf P^{(k)}\)); Use the always-valid identity
\[
\int dA\,F(A)\,e^{\mathscr A(A)}=\int d\tilde A\,F(\Phi(\tilde A))\,e^{\mathscr A(\tilde A)+\mathscr V(\tilde A)},\qquad\mathscr V(\tilde A):=\mathscr A(\Phi(\tilde A))-\mathscr A(\tilde A)+\log\bigl|\det D\Phi(\tilde A)\bigr|,
\tag{2.3}
\]
which is the manuscript's Annex W (3.12)–(3.13) with \(\vartheta_b\equiv1\) assumed input. Here \(\mathscr A(A)\) is the exponent of the \(A_k\)-integral in (3.15).

### 2.4 The amended step, in the source's order

| Source | Amended |
|---|---|
| (3.1) – (3.15): P-test, gauge fixing, Q-test, \(\Omega_{k+1}\), \(\chi_k=\chi_{Ax}=1\) on \(\Omega^\sim_{k+1}\), the background \(U_{k+1}\), the fluctuation, linearization, scaling | **unchanged** |
| (3.16) | **replaced** by (3.16\(^{\rm loc}\)) |
| "The first is equal to 1 …" (Q implied on \(R^c\)) | holds, by Lemma 4.2 (purely local proof) |
| (3.20): \(R'_{k+1}\), \(\Lambda_{k+1}\), \(S_{k+1}\), rectangular hulls | **unchanged** as rules; the input \(R_{k+1}\) is the new one |
| (3.21): \(\chi(\Omega_{k+1}\cap\Lambda^c_{k+1},S_{k+1})=\chi^{(k)}(R^c\cap\Lambda^c)\chi^{(k)c}(R)\chi'_k(S)\) | same product with \(\chi^{\rm loc}\); every factor is now a local function of \((V_k,V_{k+1})\) |
| (3.22) and the two changes of variables on \(S^{(k)*}_{k+1}\), with cutoff \(g\) | **replaced** by the chart \(\Phi\) of Definition 2.3 on all starred bonds of \(\Omega_{k+1}\); no cutoff |
| new term \(V^{(k)}(S_{k+1},A_k,\mathbf H^{(k)})\) | **replaced** by \(\mathscr V\) of (2.3), which lives on all of \(\Omega_{k+1}\) |
| (3.23) \(\mathbf T^{(k+1)}\), (3.24) | **unchanged in form**, in the variables \(\tilde A\) |
| (3.25) | same, with \(\mathscr V((A_k,A))\) in place of \(V^{(k)}(S_{k+1},(A_k,A))\) |
| (3.26)–(3.27): parameters | \(t\) multiplies \(\mathbf B_k\), \(A(g_k^{-2}(\cdot)-g_k^{-2})\) and \(\mathscr V_{\rm bd}\); \(s\) multiplies \(\mathbf R''_k\) and \(\mathscr V_{\rm reg}\) (Definition 4.3) |
| (3.28)–(3.47), construction of \(\mathbf E^{(k+1)}\), renormalization, proof of Theorem 2, (3.48)–(3.66) | **unchanged** |
| \(\mathbf R''^{(k+1)}\), \(\mathbf B^{(k+1)}\) | defined by the source's rule (S7); they now contain the terms born from \(\mathscr V\) |
| R operation ([IV], [LFR II]) | unchanged except [IV] (1.55), see (A8) |

After the chart, on a cube \(\square'\subset R_{k+1}\) the two functions are
\[
\chi\Bigl(\Bigl\{\sup_{b\in(\square'^{\sim2})^*}|\tilde A(b)|\ge t_k\Bigr\}\Bigr)\cdot\chi\Bigl(\Bigl\{\sup_{b\in(\square'^{\sim2})^*}\bigl|e^{ig_k\tilde A(b)}V^{(k)}_b(b)V^{(k)}_{\square'}(b)^{-1}-1\bigr|<2\delta_k\Bigr\}\Bigr),
\tag{2.4}
\]
the analogue of (1.23). The first depends on \(\tilde A\) only. The second depends on \(V_{k+1}\) through two local minimizers, in \(\square_b^{\sim4}\cup\square'^{\sim4}\subset\Lambda^c_{k+1}\) by (B5). This is the "desired localization property" of p.252, obtained without any cutoff.

### 2.5 The functional \(\hat{\mathbf H}_b\)

The terms born from \(\mathscr V\) must be functions of the background on the analyticity spaces. \(\mathbf H_b\) of (2.1) is defined on the construction's configurations only. Its extension is fixed as follows.

Let \(\mathbb B_b:=\mathbf B_{k+1}(\square_b^{\sim4})\) (S5). Its top level \(k+1\) occupies \(\square_b^{\sim4}\) minus a collar \(\mathcal L_b\) of width \(\le2LM_1\) at the boundary.

**Definition 2.5.** Let \((\mathbf U,\mathbf J)\) be defined on a set containing \(\square_b^{\sim4}\) and belong to the space \(\tilde U^c_{k+1}\) there.

1. *Axial frame.* \(u_{\mathbf U}\) is the gauge transformation that brings \(\mathbf U\) to the hierarchical block axial gauge of the construction on the \((k+1)\)-blocks meeting \(\square_b^{\sim4}\), normalized by \(u_{\mathbf U}=1\) on \(T^{(k+1)}\): for \(x\in B(y)\cap T^{(j)}\), \(y\in T^{(j+1)}\), \(u_{\mathbf U}(x)=u_{\mathbf U}(y)\,(M^j\mathbf U)(y,x)\), with the contour variables of [I] (0.11). Put \(\mathbf U^{\rm ax}:=\mathbf U^{u_{\mathbf U}}\), \(\mathbf J^{\rm ax}=R(u_{\mathbf U})\mathbf J\).
2. *Datum.* \(B_b(\mathbf U):=\frac1i\log\bigl[M_{\mathbb B_b}\bigl(Q^{s*}_{k+1}M^{k+1}(\mathbf U^{\rm ax})\bigr)\,M_{\mathbb B_b}(\mathbf U^{\rm ax})^{-1}\bigr]\), a field on \(\mathbb B_b\). It vanishes on the top level, so \({\rm supp}\,B_b\subset\mathcal L_b\).
3. *Response.* \(\mathscr H_b(\mathbf U,\mathbf J;B)\) is the function of [V] (179)–(180) for the determining set \(\mathbb B_b\), with the operators taken in the background \((\mathbf U^{\rm ax},\mathbf J^{\rm ax})\) (the convention of S8), at the datum \(B\); \(u_b\) is the accompanying map to the axial gauge, as in (3.6), (3.17). Put \(\mathbf U^\flat_b:=\bigl(\exp[iL^{-1}\eta\,\mathscr H_b(\mathbf U,\mathbf J;B_b(\mathbf U))]\,\mathbf U^{\rm ax}\bigr)^{u_b}\).
4. \(\exp\bigl(i\mathbf H^{\rm ax}_b(\mathbf U,\mathbf J)\bigr):=M^k(\mathbf U^{\rm ax})(b)\cdot M^k(\mathbf U^\flat_b)(b)^{-1}\), and
\[
\hat{\mathbf H}_b(\mathbf U,\mathbf J):={\rm Ad}\bigl(u_{\mathbf U}(b_-)^{-1}\bigr)\,\mathbf H^{\rm ax}_b(\mathbf U,\mathbf J).
\]

This is the formula (3.17)–(3.18) of the source with the two configurations in the order of (3.6), the reference being the background itself. Item 1 is the device of [I] (3.26) ("we introduce the same generalized axial gauge for the configuration \(M^\cdot(\mathbf U)\). This is achieved by a gauge transformation \(v\)", quoted in (CR) §1, c\*).

The amended action is *defined* with \(\mathbf H_b\) replaced by \(\hat{\mathbf H}_b(\mathbf U,\mathbf J)\) wherever a term is regarded as a function on the spaces. Lemma 3.1 shows that this changes nothing on the construction's configurations.

### 2.6 The R operation: one change

**(A8)** In [IV], preparatory integration \(n+1\) (\(j=h+n\)), replace the fluctuation \(B_j\) of (1.53) by the fluctuation against the component-local background:
\[
V_j(b)=e^{ig_jB^Z_j(b)}V^{(j)}_Z(b),\qquad V^{(j)}_Z:=M^j(U^{(n+1)}_{k,Z}),\qquad\chi'^{(j)}:=\chi(\{|B^Z_j(b)|<\delta'_j\ \text{for }b\in(\Omega^c_{j+1}\setminus Z''_{j+1})^{(j)*}\}),
\]
with \(U^{(n)}_{k,Z}\) of [IV] (1.20), in all components (small-field and large-field). Equivalently: apply the source's own change of variables [IV] (1.58)–(1.59) with cutoff 1 in every component before testing. Details and consequences in §7.2.

### 2.7 The modification list

| | Modification | Replaces in FS §2.10 | Status |
|---|---|---|---|
| (A1) | (3.16) → (3.16\(^{\rm loc}\)) with the boxes of Definition 2.1; \(k=0\): (1.18) likewise with \(U_{1,b}\) | (M4) | definition |
| (A2) | Chart \(\Phi\) of Definition 2.3 on all starred bonds of \(\Omega_{k+1}\); no cutoff \(g\); (3.22) kept only on the outermost starred bonds of \(S_{k+1}\) | (M5) | definition; Lemma 2.2 deduction |
| (A3) | \(\mathbf H_b\) extended as \(\hat{\mathbf H}_b(\mathbf U,\mathbf J)\) of Definition 2.5 | (M2), corrected (F2) | definition; Lemma 3.1–3.3 |
| (A4) | \(\mathscr V=\mathscr V_{\rm reg}+\mathscr V_{\rm bd}\); \(\mathscr V_{\rm reg}\) under the parameter \(s\), \(\mathscr V_{\rm bd}\) under \(t\); output with localization in \(\Lambda_{k+1}\) is R-class, the rest B-class | (M1), (M6) corrected (F4) | Theorem 4.5 conditional |
| (A5) | The terms born from \(\mathscr V\) are localized on tubes by the decoupling expansion of \(\hat{\mathbf H}_b\) | new (F3) | Lemma 3.4, Lemma W conditional |
| (A6) | Collar decay as a named input, in one of two forms (CD-CT) or (CD-T) of §3.2 | (M3), refined (F6) | input |
| (A7) | (3.17)–(3.19) for \(\square_b\); comparison of two local minimizers; \(R^{\rm loc}\Rightarrow Q\) | (M7) | Lemma 4.1, 4.2 conditional |
| (A8) | [IV] (1.55) against the component-local background | new (F5) | definition; §7.2 |
| (A9) | (Par-c), (Par-M), (Par-g) | — | conditions |
| (A10) | Re-reads of proposition | (M8) | §9 |

## 3. The field \(\hat{\mathbf H}_b\): identification, size, covariance, localization

"Axial gauge" means the reference-free block conditions of [III] p.248 and (3.10) ("\(U(y,x)=1\) for \(x\in B(y)\)", in the contour variables (0.11) [I]) at every level present in the determining set. In Definition 2.5 item 3, \(u_b\) is the axial frame (item 1, with the levels of \(\mathbb B_b\)) of the configuration \(\exp[iL^{-1}\eta\mathscr H_b]\mathbf U^{\rm ax}\).

### 3.1 Identification

**Lemma 3.1 — conditional** on [V] Theorem 1 (uniqueness of the minimal orbit) and [V] Proposition 9 in the form the source uses in (3.6), (3.17). On the configurations of the construction (\(\mathbf U=U_{k+1}\), \(\mathbf J=J_{k+1}\), \(b\in\mathfrak B_{k+1}\)): \(\hat{\mathbf H}_b(U_{k+1},J_{k+1})=\mathbf H_b\) of (2.1).

*Proof.* \(U_{k+1}\) is in the axial gauge, so \(u_{\mathbf U}=1\). By (B5) the box lies in \(\Omega_{k+1}\), where the constraints give \(M^{k+1}(U_{k+1})=V_{k+1}\). The first equality of (3.17) (S4) says that \(U_{k+1}\) restricted to the box is the minimizer of the box problem for its own data: \(U_{k+1}=U(\mathbb B_b,M_{\mathbb B_b}(U_{k+1}))\). By Definition 2.2 and item 2, \(U_{k+1,b}=U(\mathbb B_b,e^{iB_b}M_{\mathbb B_b}(U_{k+1}))\) with \(B_b=B_b(U_{k+1})\). Proposition 9 of [V] with reference datum \(V_0=M_{\mathbb B_b}(U_{k+1})\) and \(V'=e^{iB_b}\) gives \(U_{k+1,b}=(\exp[iL^{-1}\eta\mathscr H_b(B_b)]U_{k+1})^{u_b}=\mathbf U^\flat_b\). This is (3.6) with the pair \((U_{k+1,\square'},U_{k,\square})\) replaced by \((U_{k+1},U_{k+1,b})\). Item 4 is then (2.1). \(\square\)

### 3.2 The collar-decay input, in two forms

Let \(D_{\rm coll}:=2M_2R_{k+1}-2M_1-1\) (in \(T^{(k+1)}\)-units): by (B2) and S5 this is a lower bound for the distance from \(b\) to \(\mathcal L_b\).

> **(CD-CT)** Theorem CT♯ (analysis §6), items 2–3, rows \(\nu=0,1\) only, for the determining sets \(\mathbb B_b\): at a fixed background in the class where (K♯), (Small) hold, for complex data \(|B|_\infty,|B+b|_\infty<r_{CT}\) with \(b\) supported in the blocks of \(S\): \(|\mathscr H(B+b)(x)-\mathscr H(B)(x)|_\nu\le K_{CT}\mathfrak w_\nu e^{-\lambda d(y,S)}|b|_\infty\), \(\lambda\le\frac14\delta_0\). Status assumed input: conditional on (Geo), (K♯), (S-calc♯), (Loc), (Small), subject to the second reading of Lemmas PL/GP (the collar estimate). Two cases are used here.
> * *Real critical background, real or complex data* ([CT analysis](collar_estimates.md) §5.1): fully covered. The consumer table of the CT analysis lists [III] (3.6)–(3.8) (conditions \(\delta_0M_2\ge2\), \(A_0\ge80K_{CT}A_1\), \(600d^2L^2B_3(1+\beta_0)K_{CT}e^{-R_k}\le1\), data \(<r_{CT}\)), (3.17)–(3.19) (\(\delta_0LM_2\ge4\)) and the "complex (3.19)" of \(R^{\rm loc}\) under (Conv-CR). It is a reading additional assumption, in the CT analysis and here, that the local determining sets \(\mathbf B_{k+1}(\square^{\sim4})\) are of [V]-type with the stated distances.
> * *Complex background with independent \(\mathbf J\)* (CT analysis §5.2): K1–K2 are printed ([P] Thm 3.4, Cor. 3.5–3.6); K3 by a Neumann series not written out additional assumption; K4 replaced by Lemma GP; \(\mathscr H\) defined by (179)–(180) without the \(J\)-term. The rows \(0,1\) used here do not involve the \(D^*D\) row, which is unavailable off the real critical set.
> The binding geometric condition is [P2] (2.59): \(\delta_0RM>4(8\log\coth(\delta_0/8)+1)\) (the collar estimate item 4), to be read for the layers of \(\mathbb B_b\).
> **(CD-T)** The decoupling input [Dec] of §3.4 together with the ceiling **(Par-g′)** \(R_j\ge N_T\sqrt d\,M/M_2\) for all \(j\). Then Lemma 3.4 itself gives the bound of Lemma 3.2 with \(c_H=c_\star\). No use of CT♯. conditional

Either form is called (CD) below. With (CD-CT), \(c_H:=2\lambda M_2\).

### 3.3 Size, analyticity, covariance

**Lemma 3.2 (size) — conditional** on (CD), on the bound of the datum, and on the averaging bounds "(106)–(108), (159)–(163) in [12]" that the source invokes for (3.18)→(3.19).
1. On the construction's configurations: \(|\mathbf H_b|\le C_H\varepsilon_{k+1}e^{-c_HR_{k+1}}\). Hence \(\eta_k:=\sup_bg_k^{-1}|\mathbf H_b|\le C_HA_0(1+\beta_0)p_0(g_k)e^{-c_HR_{k+1}}\).
2. On the space \(\tilde U^c_{k+1}\) (constants \((1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1\)): \(|\hat{\mathbf H}_b(\mathbf U,\mathbf J)|\le C_Hg_k\ell_k^{\,q}e^{-c_HR_{k+1}}=:g_k\hat\eta_k\).

*Proof.* 1. S4 with \(\square'\to\square_b\): the datum is bounded by \(44d^2B_3\varepsilon_{k+1}\) and supported in \(\mathcal L_b\) (the argument uses (3.12) on the box and the axial gauge, both available by (B5)); (CD); then (3.18) and the cited averaging bounds give \(|\mathbf H_b|\le O(1)L\sup|\mathscr H_b|\) near \(b\) (the form [IV] (1.37)). 2. On the space the datum is bounded by \(C_B(\alpha_{0,k+1}+\alpha_{1,k+1})\le C_Bg_k\ell_k^q\) by (2.34), (2.39), (2.28) and the same reasoning; this is below \(r_{CT}\) for small \(g\). Then (CD) at the fixed background \((\mathbf U^{\rm ax},\mathbf J^{\rm ax})\), base point \(0\), datum \(B_b(\mathbf U)\): with (CD-CT) this is the complex-background case of CT♯; with (CD-T) it is Lemma 3.4. \(|{\rm Ad}(u_{\mathbf U}^{-1})|\le2\): the non-unitary part of \(u_{\mathbf U}\) is a product over a hierarchical path of holonomies of \(\mathbf U'=e^{i\xi A'}\), of total size \(O(d\,\alpha_1)\) by (2.39). \(\square\)

The bound on the complex datum and on \({\rm Ad}(u_{\mathbf U}^{-1})\) are additional assumption: They are additional inputs beyond [A]. Note the difference from FS §2.2: the smallness in item 2 comes from the decay of the response kernel, not from \(\mathbf U\) being a minimizer, so it holds on the whole space.

**Lemma 3.3 — conditional** on the analyticity of \(\mathscr H\) in \((\mathbf U,\mathbf J,B)\) ([V] Prop. 9; construction: P9♮, CT §6.2) and the covariance of the averaging and of the minimal determining sets (FS §3, source input; deduction).
* (H2) \(\hat{\mathbf H}_b(\mathbf U,\mathbf J)\) depends on \((\mathbf U,\mathbf J)\) restricted to \(\square_b^{\sim4}\).
* (H3) It is analytic on the space restricted to \(\square_b^{\sim4}\).
* (H5) \(\hat{\mathbf H}_b(\mathbf U^u,R(u)\mathbf J)={\rm Ad}(u(b_-))\,\hat{\mathbf H}_b(\mathbf U,\mathbf J)\) for all gauge transformations \(u\) for which both sides are defined (\(G\)-valued, and \(G^c\)-valued near them).
* (H6) \(\hat{\mathbf H}_{rb}(r\mathbf U,r\mathbf J)=r\hat{\mathbf H}_b(\mathbf U,\mathbf J)\) for lattice isometries \(r\) preserving \(\pi'\) and the block partitions.
* (H8) \(\hat{\mathbf H}_b(\mathbf U,\mathbf J)=0\) whenever \(B_b(\mathbf U)=0\); in particular at \(\mathbf U=1\).

*Proof.* (H2), (H3): every map in Definition 2.5 is local in the box and analytic. (H8): \(\mathscr H_b(\cdot;0)=0\). (H6): (B3) and covariance of each ingredient. (H5): let \(u_0(x):=u(y)\) for \(x\) in the \((k+1)\)-block of \(y\). Then \(u_{\mathbf U^u}=u_0u_{\mathbf U}u^{-1}\): the right side takes \(\mathbf U^u\) to \((\mathbf U^{\rm ax})^{u_0}\), which is axial because block-constant transformations preserve the block conditions, and it equals 1 on \(T^{(k+1)}\). So \((\mathbf U^u)^{\rm ax}=(\mathbf U^{\rm ax})^{u_0}\). \(M_{\mathbb B_b}\) and \(Q^{s*}M^{k+1}\) commute with block-constant transformations, so \(B_b\mapsto{\rm Ad}(u_0)B_b\). The response equations are covariant under a gauge transformation of the background acting by Ad on fields and data (the invariance (1.17), p.250), so \(\mathbf U^\flat_b\mapsto(\mathbf U^\flat_b)^{u_0}\) and \(\mathbf H^{\rm ax}_b\mapsto{\rm Ad}(u_0(b_-))\mathbf H^{\rm ax}_b\). Finally \({\rm Ad}(u_{\mathbf U^u}(b_-)^{-1}){\rm Ad}(u_0(b_-))={\rm Ad}(u(b_-)u_{\mathbf U}(b_-)^{-1})\). \(\square\)

### 3.4 Tube localization

**Why it is needed (F3).** Suppose a term of the new action is regarded as a function of \(\mathbf U\) on a localization domain \(X\in\mathbf D\) containing \(\square_b^{\sim4}\). By S6, \(d(X)\ge c\,(\text{side}/M)^4\ge c(2L^2M_2R_{k+1}/M)^4\). The R-class bound then demands a factor \(\exp(-c\kappa(L^2M_2/M)^4R_{k+1}^4)\). Lemma 3.2 supplies \(e^{-c_HR_{k+1}}\). For small \(g\) (large \(R\)) the requirement fails by three powers of \(R\) in the exponent. No choice of box avoids this: a box must reach a distance \(\gtrsim\kappa_0\delta_0^{-1}\log g^{-1}\) from \(b\) for \(\mathbf H_b\le g^{\kappa_0}\), and its volume in tiles is the fourth power of its side. (In the source the same volume factors \(e^{\kappa R^4}\) occur for replaced large-field regions and are paid by \(e^{-p_0(g)^2}\) with \(p_0\)-exponent \(\ge5r\); in the bulk there is no such factor.) So \(\hat{\mathbf H}_b\) must be decomposed into pieces localized on sets whose size is of order \(R\), not \(R^4\).

> **[Dec]** The decoupling expansion of [II] (1.9)–(1.18) (S9) for the response function \(\mathscr H_b\) of the box problem: with a partition \(\sigma\) of \(\square_b^{\sim4}\) into cubes \(\Delta\) of the \(M\)-partition \(\pi_k\) (side \(M\) in \(T^{(k)}\)-units; in the proper scales in \(\mathcal L_b\)) and parameters \(s(\Delta)\), there is \(\mathscr H_b(s;B)\), analytic for \(|s(\Delta)|\le e^{\kappa_1}\), equal to \(\mathscr H_b(B)\) at \(s=1\), bounded by \(C_D|B|_\infty\) on the polydisc in the norms used, and such that if \(s=0\) outside a union \(Y\) of cubes then \(\mathscr H_b(s;B)(x)\) depends on \((\mathbf U,\mathbf J,B,s)\) restricted to the component of \(Y\) containing \(x\), and vanishes if \(B=0\) there. Source: [II] p.4–6 source input on the unit lattice; [III] p.276 for the sequence \(\{\Omega_j\}\) ("we apply Theorems 3.7–3.10 [13] in their full generality"). construction: Theorem M♯ of Local deformation of propagators and the minimizer/Source operators for the deformed reconstruction as justified in Domains of the representation-defined derivatives, conditional on (W-ms), with the repair recorded in the collar estimate item 1 (one-sided derivative placement, \(\Delta'_\pi(s)\) in the right form) assumed input. That M♯ covers the minimal determining sets \(\mathbb B_b\), and complex backgrounds with independent \(\mathbf J\) (the source asserts uniformity on the domain I.(i)–(iii), [II] p.6, source), is additional assumption.

**Lemma 3.4 (tube expansion) — conditional** on [Dec]. Let \(\Delta_b\) be the cube of \(\sigma\) containing \(b\), and \(n_{\rm coll}:=\lceil LD_{\rm coll}/M\rceil\ge M_2R_{k+1}/M\) (the number of tiles a connected set needs to join \(b\) to \(\mathcal L_b\)). Then
\[
\hat{\mathbf H}_b(\mathbf U,\mathbf J)=\sum_T\hat{\mathbf H}_b(T;\mathbf U,\mathbf J),
\]
the sum over connected unions \(T\subset\square_b^{\sim4}\) of cubes of \(\sigma\) with \(\Delta_b\subset T\) and \(T\cap\mathcal L_b\ne\emptyset\). Each term depends on \((\mathbf U,\mathbf J)\) restricted to \(T\), is analytic on the space restricted to \(T\), has the covariances (H5), (H6) and the property (H8), and
\[
|\hat{\mathbf H}_b(T;\mathbf U,\mathbf J)|\le C_D'\,g_k\ell_k^{\,q}\,e^{-(\kappa_1-1)(|T|-1)},\qquad|T|\ge n_{\rm coll},
\]
\(|T|\) the number of cubes. Consequently, if \(\kappa_1\ge4(1+\log c_d)\) (\(c_d^n\) bounds the number of connected sets of \(n\) cubes containing a given one),
\[
\sum_T|\hat{\mathbf H}_b(T)|\,e^{\frac12\kappa_1|T|}\le C_\star\,g_k\ell_k^{\,q}\,e^{-c_\star R_{k+1}},\qquad c_\star:=\tfrac14\kappa_1M_2/M.
\tag{3.1}
\]

*Proof.* As in [II] (1.9)–(1.10): \(\mathscr H_b(1;B)(x)=\sum_{Y_0}\int\prod_{\Delta\subset Y_0\setminus\Delta_b}ds(\Delta)\,\partial_{s(\Delta)}\mathscr H_b(s(Y_0);B)(x)\), over connected \(Y_0\supset\Delta_b\), with \(s=0\) off \(Y_0\). The term of \(Y_0\) depends on \(B\) restricted to \(Y_0\). Here \(B=B_b(\mathbf U)\) is supported in \(\mathcal L_b\). If \(Y_0\cap\mathcal L_b=\emptyset\) the term is \(\mathscr H_b(s;0)=0\). So only \(Y_0\) reaching the collar contribute, and such \(Y_0\) contain at least \(n_{\rm coll}\) cubes. The Cauchy formula on the circles \(|s(\Delta)|=e^{\kappa_1}\) and the polydisc bound give \(C_D|B|_\infty e^{-(\kappa_1-1)(|Y_0|-1)}\) ([II] (1.23)–(1.24)). The remaining maps of Definition 2.5 (the datum on \(Y_0\cap\mathcal L_b\), the average at \(b\), the frame at \(b_-\)) are local in \(Y_0\); put \(T=Y_0\). For (3.1): \(\sum_{n\ge n_{\rm coll}}c_d^ne^{-(\frac12\kappa_1-1)(n-1)}\le2e^{\kappa_1}e^{-\frac14\kappa_1n_{\rm coll}}\) and \(n_{\rm coll}\ge M_2R_{k+1}/M\). \(\square\)

Which tiles the walk expansions use in the multi-level collar, and at which scale in the top-level region, is taken from the source's general statement ([III] p.276) and not worked out here additional assumption; only the lower bound on \(n_{\rm coll}\) matters.

*Remarks.* (1) Lemma 3.4 gives decay per tile from the vanishing of decoupled kernels alone. This is F6: when \(n_{\rm coll}\) is large, which is a coupling ceiling, no lattice-scale decay theorem is needed. (2) With the \(s\)-variant of CT♯ (deformed package, on (W-ms), \(\lambda\le\frac1{16}\delta_0\)) the polydisc bound carries an extra factor \(e^{-\lambda D_{\rm coll}}\), and \(c_\star\) improves to \(\frac1{16}\delta_0\cdot2M_2\). (3) The localization sets \(T\) are tubes: the minimal ones have \(\approx2M_2R_{k+1}/M\) cubes.

[The CT analysis](collar_estimates.md) stresses (§§8.1, 8.3 there; the collar estimate item 3) that CT♯ differentiates in the **data at a fixed background** and gives no decay for variations of the background. This note uses the following, and nothing else.

| Place | Kind of variation | Tool |
|---|---|---|
| Lemma 3.2(1), 4.1, 4.2 (real configurations of the construction) | datum \(0\to B_b\), supported in the collar, at the fixed real critical background \(U_{k+1}\) restricted to the box | CT♯ item 3 at \(B=0\) (or (CD-T)) |
| Remark after Lemma 4.1; §7.2 | datum supported in a collar, at a fixed real critical local minimizer | same |
| Lemma 3.2(2) (size on the space) | datum \(0\to B_b(\mathbf U)\) at the fixed background \((\mathbf U^{\rm ax},\mathbf J^{\rm ax})\) | CT♯ at a complex background with independent \(\mathbf J\) (CT analysis §5.2, weaker status), or (CD-T) |
| Lemma 3.4, Lemma W (dependence of \(\hat{\mathbf H}_b\) on \((\mathbf U,\mathbf J)\) away from \(b\)) | **this is a background variation** | **not** a decay estimate: exact localization by the decoupling expansion [Dec] (walk expansions of the operators in the background, \(s\)-parameters, Cauchy in \(s\)) |
| §8 (finite propagation of labels) | none | exact locality by definition |

So the derivation **does** need control of how \(\hat{\mathbf H}_b\) responds to changes of the configuration far from \(b\) in the form of a background variation, and it takes that control from [Dec], which is an input **in addition to** CT♯. It does not need the unproved background-variation theorem (CT-U) of the [CT analysis](collar_estimates.md) §8.3. A decay bound of that kind would not suffice anyway: property (i) of the R-class is exact dependence on \(\mathbf U\) restricted to \(X\), which only a decoupling gives.

*Why the definition of \(\hat{\mathbf H}_b\) is the source-style one and not the (Conv-CR) one.* Under (Conv-CR) one would write \(\mathbf U=e^{i\xi A'}U\) with a real representative \(U\), take as fixed real critical background the box minimizer \(U^\sharp=U(\mathbb B_b,M_{\mathbb B_b}(U))\), and put the complex part into the data. The size bound is then exactly the justified real-critical case of CT♯ ("complex (3.19)", level conditional). But \(U^\sharp\) depends on the real data in the whole box, so the tube terms would depend on \(U\) outside the tube through the background. Localizing that dependence is a background variation of the kind CT♯ does not cover; it would need (CT-U) or a decoupling of the composite reconstruction. Definition 2.5 avoids this at the price stated in the table: on the space the size bound uses CT♯ at complex backgrounds with independent \(\mathbf J\), or no CT at all through (CD-T). On the construction's own (real, critical) backgrounds the two definitions coincide and the question does not arise. If the construction prefers to stay strictly inside the justified real-critical case, the route is (CD-T), i.e. [Dec] plus the ceiling (Par-g′).

## 4. CMP 119 §3 for the amended map, line by line

### 4.1 (3.1)–(3.15): verbatim

Nothing in pp.264–268 up to (3.15) refers to the R-test. (3.2) P-decomposition; axial gauge fixing; (3.3)–(3.4) Q-decomposition; (3.5) \(\Omega_{k+1}\); (3.6)–(3.9) \(\chi_k=\chi_{Ax}=1\) on \(\Omega^\sim_{k+1}\); (3.10)–(3.11) \(V^{(k)}=M^k(U_{k+1})\) and \(V'_k\); (3.12)–(3.14) \(|V'_k-1|<O(1)\varepsilon_k\); the resummation \(\zeta(\Omega^c_{k+1})\); expansion, linearization, \(A'_k=g_kA_k\); (3.15). All hold as printed. The decay input of (3.6)–(3.8) is the source's own and is not new (either form of (CD) covers it; CT's consumer table lists it).

### 4.2 (3.16)–(3.19)

(3.16) is replaced by (3.16\(^{\rm loc}\)). The sentence after it becomes Lemma 4.2. (3.17)–(3.19) remain true statements about \(U_{k+1}\) and \(U_{k+1,\square'}\) and are used in Lemma 4.1.

**Lemma 4.1 — conditional** on (CD) and the inputs of S4. Let \(\theta_k:=O(1)44d^2B_3K(1+\beta_0)\frac{A_0}{A_1}e^{-c_HR_{k+1}}\) (\(K=B_3\) in the source's notation). For \(b\in\mathfrak B_{k+1}\) and every \(\square'\in\pi'\) with \(b\in(\square'^{\sim2})^*\):
\[
|V^{(k)}(b)V^{(k)}_b(b)^{-1}-1|\le\theta_k\delta_k,\qquad|V^{(k)}(b)V^{(k)}_{\square'}(b)^{-1}-1|\le\theta_k\delta_k,\qquad|V^{(k)}_b(b)V^{(k)}_{\square'}(b)^{-1}-1|\le2\theta_k\delta_k.
\]
*Proof.* The second is (3.19); it needs \(\square'^{\sim4}\subset\Omega_{k+1}\), which holds by (B2), (B5). The first is (3.17)–(3.19) with \(\square'\) replaced by \(\square_b\): the argument (S4) uses the regularity (3.12) of \(U_{k+1}\) on the box, \(M^{k+1}(U_{k+1})=V_{k+1}\) there, that the box is a union of \(M_1\)-cubes (S5), and the distance \(D_{\rm coll}\) from \(b\) to the collar (B2). The third follows from \(|WW'-1|\le|W-1|+|W'-1|\) for unitary \(W,W'\) and a unitarily invariant norm. \(\square\)

*Remark (purely local form).* The third inequality also follows without the global background, when \(U_{k+1,b}\) is regular on \(\square'^{\sim4}\): restricted to \(\square'^{\sim4}\subset\square_b^{\sim4}\), \(U_{k+1,b}\) is the minimizer for its own data on \(\mathbf B_{k+1}(\square'^{\sim4})\); these data differ from \(M^\cdot(Q^{s*}V_{k+1})\) only in the collar of \(\square'^{\sim4}\); apply (CD). Use this form in §7.2 and §8. Status conditional, same inputs; the coincidence of the two determining sets near shared faces is additional assumption.

**Lemma 4.2 (\(R^{\rm loc}\Rightarrow Q\); comparison with the literal test) —** given Lemma 4.1 and \(2\theta_k<1\).
1. If \(\sup_{b\in(\square'^{\sim2})^*}|A^{\rm loc}_k(b)|<t_k\) then \(\sup_{b\in(\square'^{\sim2})^*}|V_k(b)V^{(k)}_{\square'}(b)^{-1}-1|<(1+2\theta_k)\delta_k<2\delta_k\). So on \(R^c_{k+1}\) the Q-functions \(\chi'_k(\square')\) equal 1 and are dropped, as on p.268.
2. On \(\mathfrak B_{k+1}\): \(|A^{\rm loc}_k(b)-A_k(b)|\le2\eta_k\) whenever \(|g_kA_k(b)|\) is below an absolute constant. So (3.16\(^{\rm loc}\)) and (3.16) give the same label unless \(\sup|A_k|\) lies within \(2\eta_k\) of \(t_k\) (TC Lemma 5.2(4)).

*Proof.* 1. \(V_kV_{\square'}^{-1}=(V_kV_b^{-1})(V_bV_{\square'}^{-1})\), \(|e^{iX}-1|\le|X|\), Lemma 4.1. 2. \(e^{ig_kA^{\rm loc}}=e^{ig_kA}e^{i\mathbf H_b}\) and the Baker–Campbell–Hausdorff series. \(\square\) 

### 4.3 (3.20)–(3.25)

(3.20) is unchanged. (3.21) holds with \(\chi^{\rm loc}\). The sentence "The last function above depends nonlocally on \(V_{k+1}\), through the function \(V^{(k)}\)" describes the source's parametrization. In the chart of Definition 2.3 the functions on \(S_{k+1}\) are (2.4) on cubes of \(R_{k+1}\) and, on cubes of \(S_{k+1}\setminus R_{k+1}\), the Q-function in the form \(\chi(\{\sup_b|e^{ig_k\tilde A(b)}W_b(b)V^{(k)}_{\square'}(b)^{-1}-1|<2\delta_k\})\) with \(W_b=V^{(k)}_b\) or \(V^{(k)}_{\Lambda^c_{k+1}\cap\Lambda_k}\) according to the bond. All depend on \(V_{k+1}\) restricted to \(\Lambda^c_{k+1}\) ((B5); p.269 for the second). The R-functions, small-field and large-field, are functions of \(\tilde A\) alone. This is what (3.21)–(3.22) are for.

The map \(\Phi\) is a diffeomorphism of the relevant domain: on \(\Omega_{k+1}\), \(|g_kA_k|\le O(1)\varepsilon_k\) by (3.14), \(|\mathbf H|\le g_k\eta_k\), and (2.2) is a right translation in the group. Identity (2.3) holds. (3.23)–(3.24) keep their form in the variables \(\tilde A\) ("we denote the new variables \(A'\) by \(A\)", p.252). In (3.25) the term \(V^{(k)}(S_{k+1},(A_k,A))\) is replaced by \(\mathscr V((A_k,A))\).

**Definition 4.3 (splitting of the exponent).** Let \(\Phi=\Phi_{\rm loc}\circ\Phi_S\) (they act on disjoint sets of bonds). Write the exponent of (3.15), after the source's chart \(\Phi_S\) on the outermost bonds, as \(\mathscr A_0+\mathscr A_{R''}+\mathscr A_{\rm bd}\):
* \(\mathscr A_0=-\frac12\langle A,C^*\Delta^{(k)}CA\rangle+\mathbf P^{(k)}+\{\mathbf E_k(U_k(\cdots))-\mathbf E_k(U_{k+1})\}\), with \(\mathbf R'_k\) included in \(\mathbf E_k\) (S7);
* \(\mathscr A_{R''}=\mathbf R''_k(U_k(\cdots))-\mathbf R''_k(U_{k+1})\);
* \(\mathscr A_{\rm bd}=\) the \(\mathbf B_k\)-difference, the \(A(g_k^{-2}(\cdot)-g_k^{-2})\)-difference, and the source's \(V^{(k)}\) on the outermost bonds.

Put
\[
\mathscr V_{\rm reg}:=(\mathscr A_0+\mathscr A_{R''})\circ\Phi_{\rm loc}-(\mathscr A_0+\mathscr A_{R''})+\log|\det D\Phi_{\rm loc}|,\qquad\mathscr V_{\rm bd}:=\mathscr A_{\rm bd}\circ\Phi_{\rm loc}-\mathscr A_{\rm bd}.
\]
By (2.3) the integrand of the amended (3.25) is \(\chi^{{\rm loc}(k)}(\Lambda_{k+1})\exp[\mathscr A_0+\mathscr A_{R''}+\mathscr A_{\rm bd}+\mathscr V_{\rm reg}+\mathscr V_{\rm bd}]\).

### 4.4 (3.26)–(3.27): the parameters

Let \(F(s,t):=\log[z^{(k)}\int dA\,\chi^{{\rm loc}(k)}(\Lambda_{k+1})\exp(\mathscr A_0+s(\mathscr A_{R''}+\mathscr V_{\rm reg})+t(\mathscr A_{\rm bd}+\mathscr V_{\rm bd}))]\). Then
\[
F(1,1)=\int_0^1dt\,\bigl\langle\mathscr A_{\rm bd}+\mathscr V_{\rm bd}\bigr\rangle_{s=1,t}+\int_0^1ds\,\bigl\langle\mathscr A_{R''}+\mathscr V_{\rm reg}\bigr\rangle_{s,t=0}+F(0,0).
\tag{3.26\(^{\rm loc}\)}
\]
This is (3.26) with \(V^{(k)}(S_{k+1})\) replaced by \(\mathscr V_{\rm bd}\) plus the source's outermost part, and \(\mathbf R''_k\)-difference replaced by \(\mathbf R''_k\)-difference \(+\mathscr V_{\rm reg}\). The measure (3.27) changes accordingly. — deduction. No further parameter is needed (F4).

**Proposition 4.4 (the regular part is the source's).** \(F(0,0)\) is, as a function of \(U_{k+1}\), of the values of the external chart variable and of \(\Lambda_{k+1}\), identical with the third term of the source's (3.26): the integrand is \(\exp\mathscr A_0\), and \(\chi^{{\rm loc}(k)}(\Lambda_{k+1})\) is the same function of the integration variable as \(\chi^{(k)}(\Lambda_{k+1})\), namely \(\prod\chi(\{|A(b)|<t_k\})\). Hence (3.28)–(3.42), the definitions (3.37), (3.41), the terms \(\mathbf E^{(k+1)}_0(\Lambda_{k+1},X,z)\), their independence of \(\Lambda_{k+1}\) for \(X\subset\Lambda_{k+1}\), and the definition of \(\mathbf E^{(k+1)}\) on p.279 hold verbatim.

### 4.5 The expansion of \(\mathscr V\): Lemma W

**Lemma W — conditional** on S9 (the localized form of \(\mathscr A_0\), \(\mathscr A_{R''}\), \(\mathscr A_{\rm bd}\) and of the kernel \(C^*\Delta^{(k)}C\), with the source's analyticity and bounds), Lemma 3.2–3.4, (Par-g). There is a representation
\[
\mathscr V_{\rm reg}=\sum_{X\in\mathbf D_k}W(X;U_{k+1},J_{k+1},\tilde A)
\]
such that:
* (W1) \(W(X;\mathbf U,\mathbf J,\tilde A)\) is defined and analytic on \(\tilde U^c_{k+1}(X,(1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1)\times\{\tilde A:|\tilde A|<C_1p_1(g_k)-1\text{ on }X\}\) and depends on its arguments restricted to \(X\);
* (W2) it is invariant under the simultaneous gauge transformations \(\mathbf U\to\mathbf U^u\), \(\mathbf J\to R(u)\mathbf J\), \(\tilde A\to R(u)\tilde A\);
* (W3) \(|W(X;\mathbf U,\mathbf J,\tilde A)|\le g_k^{\kappa_0+2}\exp(-(1-4\delta)\kappa\,d_k(X))\), \(\kappa\) and \(\delta\) as in [II] (1.36), provided \(\frac12\kappa_1\ge\kappa\);
* (W4) \(W(X;\mathbf U,\mathbf J,\tilde A)=0\) if \(B_b(\mathbf U)=0\) for all \(b\in X\cap\mathfrak B_{k+1}\); in particular \(W(X;1,0,\tilde A)=0\);
* (W5) \(W\) is covariant under the lattice isometries that preserve \(\pi'\), the \(M\)-partition and the covariance group of the corresponding terms of S9;
* (W6) for \(X\subset\Lambda_{k+1}\), \(W(X;\cdot)\) does not depend on \(\Lambda_{k+1}\), given the same property of the terms of S9.

The same holds for \(\mathscr V_{\rm bd}\), with terms whose localization domains meet \(Z_k^\sim\) or \(\Lambda^c_{k+1}\).

*Proof.* *Step 1 (the chart map).* \(a_b(A',\mathbf H)=A'-\varphi_{\mathbf H}(A')\) is analytic for complex \(|g_kA'|,|\mathbf H|\le\rho_0\) (an absolute radius of convergence of the Baker–Campbell–Hausdorff series), vanishes at \(\mathbf H=0\), and \(|a_b|\le2g_k^{-1}|\mathbf H|\), \(|\partial a_b/\partial A'|\le C|\mathbf H|\). Let \(\rho_H:=\frac12g_k\). For \(|\mathbf H_b|<\rho_H\) and \(|\tilde A|<C_1p_1-1\) the point \(\Phi_{\rm loc}(\tilde A)\) lies in \(\{|A|<C_1p_1\}\).

*Step 2 (one localized term, \(\mathbf H\) free).* Take a term \(\mathbf V(Y;\mathbf U,\mathbf J,A)\) of S9, or a term \(\langle A,K(Y)A\rangle\) of the walk expansion of \(K=C^*\Delta^{(k)}C\), and put \(w(Y;\tilde A,\mathbf H):=\mathbf V(Y;\Phi_{\rm loc}(\tilde A))-\mathbf V(Y;\tilde A)\), a function of \((\tilde A(b),\mathbf H_b)_{b\subset Y}\), analytic on the polydisc \(|\mathbf H_b|<\rho_H\), zero at \(\mathbf H=0\), bounded there by \(S_Y:=2\sup|\mathbf V(Y)|\le C_V\,p_1(g_k)^2|Y|^2e^{-(1-2\delta)\kappa d_k(Y)}\) (the quadratic parts are polynomially bounded on \(|A|<C_1p_1\)). The Jacobian contributes the one-bond terms \(\log\det(1-\partial a_b/\partial A')\), with the same properties.

*Step 3 (insert the tubes).* Expand \(w(Y;\tilde A,\cdot)\) in its power series in \(\mathbf H\) about 0: \(w=\sum_{m\ne0}w_m(Y;\tilde A)\mathbf H^m\), \(|w_m|\le S_Y\rho_H^{-|m|}\). Substitute \(\mathbf H_b=\sum_T\hat{\mathbf H}_b(T)\) (Lemma 3.4) in each monomial. A product \(\prod_i\hat{\mathbf H}_{b_i}(T_i)\) with \(b_i\subset Y\) is localized in \(Y\cup\bigcup_iT_i\), which is connected because \(\Delta_{b_i}\subset T_i\) and \(b_i\subset Y\). Let \(X\) be this set (a domain of \(\mathbf D_k\); in the collar regions take the smallest one containing it). Since a tree for \(X\) is obtained from a tree for \(Y\) and trees for the \(T_i\), \(d_k(X)\le d_k(Y)+c\sum_i|T_i|\). With \(\hat\eta:=\) the right side of (3.1) and \(n_c=\dim\mathfrak g\),
\[
\sum_{m\ne0}|w_m|\prod_b\Bigl(\sum_T|\hat{\mathbf H}_b(T)|e^{\frac12\kappa_1|T|}\Bigr)^{m_b}\le S_Y\Bigl[\prod_{b\subset Y}\bigl(1-\hat\eta/\rho_H\bigr)^{-n_c}-1\Bigr]\le S_Y\,x_Ye^{x_Y},\qquad x_Y:=2n_c|Y^*|\hat\eta/\rho_H.
\]
By (Par-g), \(\hat\eta/\rho_H\le2C_\star\ell_k^qe^{-c_\star R_{k+1}}\) is so small that \(e^{x_Y}\le e^{\delta\kappa d_k(Y)}\) (\(|Y^*|\le dM^d(d_k(Y)+1)\cdot3^{23}\)) and \(S_Yx_Y\le g_k^{\kappa_0+2}e^{-(1-3\delta)\kappa d_k(Y)}\cdot\)(a factor absorbed in \(e^{\delta\kappa d_k}\)). Define \(W(X)\) as the sum of all contributions with the given \(X\). The weights \(e^{-\frac12\kappa_1|T_i|}\) and \(e^{-(1-3\delta)\kappa d_k(Y)}\) give \(e^{-(1-4\delta)\kappa d_k(X)}\) and leave a convergent sum over \((Y,\{T_i\})\) with union \(X\) ([II] (1.26), (2.29)). This is (W3). (W1): composition of analytic maps; the series converges uniformly on the stated domain. (W2): the terms of S9 are jointly invariant; \(\Phi_{\rm loc}\) commutes with \(R(u)\) when \(\mathbf H_b\to{\rm Ad}(u(b_-))\mathbf H_b\); (H5) holds for each \(\hat{\mathbf H}_b(T)\). (W4): (H8) for each tube term and \(w=0\) at \(\mathbf H=0\). (W5): (H6), (B3) and the covariance of the terms of S9. (W6): \(\hat{\mathbf H}_b\) and \(\Phi_{\rm loc}\) are defined without reference to \(\Lambda_{k+1}\). \(\square\)

*What is taken from the source in Lemma W.* That \(\mathscr A_0\), \(\mathscr A_{R''}\), \(\mathscr A_{\rm bd}\) and the kernel \(K\) have localized analytic expansions with the stated bounds ([II] Lemma 2 and [III] pp.275–277). The proof assumes these.

### 4.6 Where the new terms land: Theorem 4.5

**Theorem 4.5 — conditional** on Lemma W and on the source's cluster expansion of expectation values, [III] (3.44)–(3.47) with the sentence "The other expectation values in (3.26), (3.28) are treated in exactly the same way" (S7; source). Apply the source's procedure to the second term of (3.26\(^{\rm loc}\)). Then
\[
\int_0^1ds\,\langle\mathscr A_{R''}+\mathscr V_{\rm reg}\rangle_{s,t=0}=\sum_{X\in\mathbf D_{k+1},X\subset\Lambda_{k+1}}\bigl[\mathbf R''^{(k+1)}_{\rm src}(X)+\mathbf R^{(k+1)}_W(X)\bigr]+(\text{terms with }X\not\subset\Lambda_{k+1}),
\]
where \(\mathbf R''_{\rm src}\) are the terms in which the integrated function is a term of \(\mathscr A_{R''}\) and \(\mathbf R_W\) those in which it is a \(W(X_0)\). The terms \(\mathbf R^{(k+1)}_W(X,U_{k+1})\):
1. depend on \(U_{k+1}\) restricted to \(X\) (property (i));
2. extend analytically to \(\tilde U^c_{k+1}(X,\cdot,\cdot)\) with the improved constants of p.262 (property (ii));
3. are gauge invariant (property (iii));
4. satisfy \(|\mathbf R^{(k+1)}_W(X,(\mathbf U,\mathbf J))|\le g_{k+1}^{\kappa_0}\exp(-(1+4\beta)\kappa d_{k+1}(X))\) ((2.31));
5. do not depend on \(\Lambda_{k+1}\);
6. are covariant under the Euclidean transformations leaving the \(MR_{k+1}\)-partition invariant ((2.32));
7. vanish at \(\mathbf U=1\): \(\mathbf R^{(k+1)}_W(X,1)=0\).

They are therefore R-class terms in the sense of (2.30)–(2.32), and are included in \(\mathbf R^{(k+1)}\). The terms with \(X\not\subset\Lambda_{k+1}\), and all terms of the first expectation in (3.26\(^{\rm loc}\)) that come from \(\mathscr V_{\rm bd}\), meet the large-field region and are included in \(\mathbf B^{(k+1)}\); they satisfy (2.41)–(2.42) with \(B_0\) replaced by \(g_k^{\kappa_0}\).

*Proof.* In the source's expansion the potentials of the measure and the integrated function are sums of localized analytic terms. The \(W(X_0)\) enter in two places. (a) In the measure \(\langle\cdot\rangle_{s,t=0}\) as additional potentials \(sW(X_0)\); by (W3) they are bounded on the real integration domain and on the analyticity space by \(g_k^{\kappa_0+2}e^{-(1-4\delta)\kappa d_k(X_0)}\), far below the smallness \(\alpha_4\) required of potentials in [II] (2.18)–(2.20); all estimates of [II] §2 hold with unchanged constants. (b) As the integrated function: the factor \(H'(Z_0)\) of (3.44) contains one \(W(X_0)\) and "satisfies the same bound as the other factors" times \(g_k^{\kappa_0+2}\). The resummations (3.45)–(3.47) are the source's. This gives items 1–4 with \(g_k^{\kappa_0+2}\cdot O(1)\le g_{k+1}^{\kappa_0}\) ((2.6)) and the improved decay by the choice of \(\kappa_1\), as for every newly created term. Item 5 is the source's argument for the terms with \(X\subset\Lambda_{k+1}\), with (W6). Item 6: a transformation preserving the \(MR_{k+1}\)-partition preserves \(\pi'\), the \(M\)-partition and the blocks by (Par-c); use (W5) and the covariance of the measure. Item 7: at \(\mathbf U=1\) all \(W(X_0)\) vanish identically in \(\tilde A\) by (W4), so every term containing one as integrated function is zero. \(\square\)

*Consequences.* (i) The vacuum-energy subtraction (2.30) is void for the new terms. (ii) Theorem 2, (2.44), holds for them by the source's argument ("It follows from the considerations of Sects. 3, 4 [I]", p.263), which uses (i)–(iii) and (2.31) only. (iii) Nothing restricts the density of R-terms in (2.30)–(2.32); the sum over \(X\) is controlled by \(e^{-\kappa d}\), the sum over \(j\) by \(g_j^{\kappa_0}\) (p.260).

### 4.7 pp.275–285

The localized expansions, the space (3.43), the cluster expansions (3.44)–(3.47), the definition of \(\mathbf E^{(k+1)}\), \(\mathbf R''^{(k+1)}\), \(\mathbf B^{(k+1)}\), the vacuum and coupling renormalization on p.279, and the proof of Theorem 2 with (3.48)–(3.66) hold as printed, with the additions of §§4.5–4.6. The analyticity radius in the fluctuation field for the new terms is \(C_1p_1(g_k)-1\) instead of \(C_1p_1(g_k)\); only boundedness on the real domain \(|A|<t_k=A_1p_0(g_k)\) is used for them.

### 4.8 The first step, §1

(1.1)–(1.17) unchanged. (1.18) → the local test with \(U_{1,b}=U(\mathbf B_1(\square_b^{\sim4}),M^\cdot(Q^{s*}_1V))\), \(A^{\rm loc}(b)=(ig_0)^{-1}\log(U(b)U_{1,b}(b)^{-1})\). (1.19): the second function equals 1 by Lemma 4.2. (1.20) unchanged. (1.21) is kept for the outermost bonds of \(S_1\) only. (1.22) is replaced by (2.2) (no cutoff). (1.23) → (2.4). (1.24) → the Jacobian of \(\Phi\), which cancels the change of \(\log\sigma\) in (1.14) by Lemma 2.2. \(V^{(0)}(S_1,A,\mathbf H_{1,Ax})\) → \(\mathscr V\). (1.25) with \(\chi^{\rm loc}\). The conditional integral is treated as in §§4.4–4.6 with \(\mathbf R''_0=0\).

## 5. Gauge invariance and reflection covariance of the amended test

**Proposition 5.1 —** given the covariance of the averaging, the gauge fixing and the minimizers (FS §3: source input; deduction).
1. *First invariance* (p.250). Under \(V_{k+1}\to V_{k+1}^v\) every local minimizer transforms by the block-constant \(u_0\), \(u_0(x)=v(y)\) for \(x\in B(y)\): \(V^{(k)}_b\to(V^{(k)}_b)^{u_0}\). With \(V_k\to V_k^{u_0}\), \(V_k(b)V^{(k)}_b(b)^{-1}\) is conjugated by \(u_0(b_-)\), so \(|A^{\rm loc}_k(b)|\) is invariant. The label (3.16\(^{\rm loc}\)) is invariant.
2. *Second invariance* (1.17). The integrand of the amended (3.25) is \(F(U_{k+1},\tilde A,\mathbf H)\) with \(F(U^u,R(u)\tilde A,R(u)\mathbf H)=F(U,\tilde A,\mathbf H)\): the source's exponent is invariant under (1.17), \(\Phi_{\rm loc}\) commutes with \(R(u)\), and \(\chi^{{\rm loc}(k)}(\Lambda_{k+1})\) depends on \(|\tilde A(b)|\) only. With \(\mathbf H=\hat{\mathbf H}(\mathbf U,\mathbf J)\) and (H5), every term is invariant under all gauge transformations, as (iii) and [I] (1.19) require. The source asserts the same of \(V^{(k)}(S,A,\mathbf H^{(k)})\) without saying how \(\mathbf H^{(k)}\) is extended; Definition 2.5 item 1 supplies it there too.
3. *Lattice isometries.* For every isometry \(r\) of the lattice that preserves \(\pi'\) and the block partitions, \(A^{\rm loc}_k(rb)[rV_k,rV_{k+1}]=rA^{\rm loc}_k(b)[V_k,V_{k+1}]\) by (B3), and the label map commutes with \(r\). This includes the reflections through hyperplanes containing centres of partition cubes used in the chessboard argument (TC §4; FS §3.4).

Reflection positivity itself is a property of the Wilson measure and is not affected by the choice of labels. What the chessboard argument needs from the labels is items 1, 3 and §8.

## 6. The coupling recursion

**Proposition 6.1 — conditional** on Theorem 4.5 and Proposition 4.4.
1. \(\mathbf E^{(k+1)}\) is given by the source's formulas from \(\mathbf E_k\) (including \(\mathbf R'_k\)). The recursion (2.24) and the definition of \(\beta_{k+1}\) by (3.61)–(3.64) are unchanged.
2. The new terms never receive a coupling counterterm. Their second-order (marginal) part is carried in \(\mathbf R\) with the bound (2.44): \(R_1g_j^{\kappa_0}\) per unit volume of each later scale.
3. They influence \(\beta_m\), \(m>j\), only after they have been merged into \(\mathbf E_{m-1}\) as part of \(\mathbf R'_{m-1}\) (S7), exactly as the source's R-terms do. The change of \(\beta_m\) relative to the literal construction is bounded by \(C\sum_{j\le k_1(m)}g_j^{\kappa_0}\le Cg_m^{\kappa_0-2}\) along an asymptotically free trajectory ((2.6)).
4. In the idealized whole-lattice flow (\(\Omega_j=\Lambda_j=T\)) the literal construction has no R-terms and its \(\beta_j\) is that of [I]. The amended construction has the bulk terms \(\mathbf R_W\), so its \(\beta_j\) differs from [I]'s by at most \(Cg_j^{\kappa_0-2}\), \(\kappa_0\) arbitrary. The difference is beyond all orders, not zero. FS's "no coupling-recursion shift" should be read in this sense.

For B-03 (Corollary D′ of `Hypotheses for a projected Wilson recurrence`, c\*): its hypothesis (F1) asks \(|\mathbf R^{(j)}(X)|\le g_j^{\kappa_0}e^{-\kappa d_j(X)}\) on the native spaces and (R\(^*\)) bounds mature R potentials by \(C_R\rho_kg_k^{\kappa_0-7}\). The terms \(\mathbf R_W\) satisfy (F1) by Theorem 4.5 and enter (R\(^*\)) with the same bound. The one-loop coefficient \(d_B\) and the Gaussian calibration (G) come from \(F(0,0)\), which is unchanged (Proposition 4.4). The remainder \(|r_m|\le Av_m^3\) is affected at order \(g^{\kappa_0-7}\), below \(v^3\) for \(\kappa_0\ge14\). B-03's (F1) for the R-part currently rests on the source's "exactly the same way"; the new family adds no hypothesis of a new kind but must be named there.

## 7. The large-field side

### 7.1 What [IV] and [LFR II] read from the R-test

| Use | Source (label) | Amended construction |
|---|---|---|
| Large-field factor of flagged cubes | [LFR II] p.380 source input, S10: \(\chi^{(j-1)c}(R_j)\) "yields the factor \(\exp(-\gamma_0g_j^{-2}\delta_j^2(LM_2R_j)^{-d}|R_j|)\), by the same positivity bound for the quadratic form" | **Survives.** In a flagged cube some \(|\tilde A(b)|\ge t_j\), hence \(|A_j(b)|\ge t_j-2\eta_j\) (Lemma 4.2(2)); the factor holds with \(\delta_j^2\to(1-2\eta_j/t_j)^2\delta_j^2\). Alternatively use the Q-mechanism of the preceding sentence of p.380 with threshold \(\delta_j\) (FS §2.4). deduction given p.380 |
| The seven groups of functions of an eligible component | [IV] p.178 source: (1.7) Q in \(V_j\); (1.8) \(\chi(\{\sup|\exp ig_jA_j(b)V^{(j)}_{Z_{j+1}\setminus Z_j}(b)(V^{(j)}_{\square'}conditional)^{-1}-1|<2\delta_j\})\) on \(\square'\subset(\Omega_{j+1}\setminus\Lambda^\sim_{j+1})\cap Z\); (1.9) \(\chi(\{\sup|A_j(b)|<g_j^{-1}\delta_j\})\) on \(\square'\subset(\Lambda^\sim_{j+1}\setminus\Lambda_{j+1})\cap Z\) | (1.9): the same function of the chart variable \(\tilde A_j\). (1.8): the same Q-function, written with \(V^{(j)}_b\) on bonds of \(\mathfrak B_{j+1}\); as a function of \(V_j\) it is of type (1.7) |
| Completion (1.28) of the R-functions to \(Z_{j+1}\cap\Omega_{j+1}\) | [IV] p.183 source input | Same decomposition in \(\tilde A_j\). On bonds of \(\mathfrak B_{j+1}\) the test is against \(V^{(j)}_b\); on the outermost bonds against \(V^{(j)}_{\Lambda^c_{j+1}\cap\Lambda_j}\), as in the source. Both are functions of the fields in the component |
| (1.29): the new restrictions make (1.3)–(1.5), (1.7), (1.8), \(\chi^{(n)}_k\) equal to 1 | [IV] pp.183–187 source input; (1.32) uses \(\chi^{(0)}_j\), (1.39)–(1.42) the smallness of \(V^{(j)}_{Z_{j+1}\setminus Z_j}-V^{(j)}_{\square'}\) | **Survives, with a shorter proof for (1.8).** \(|\tilde A_j(b)|<t_j\) gives \(|V_jV_b^{(j)-1}-1|\le\delta_j\); the Remark after Lemma 4.1 gives \(|V^{(j)}_bV^{(j)-1}_{\square'}-1|\le2\theta_j\delta_j\). conditional |
| First integral of (1.60): \(\int dA_j\,\chi^{(j)}(Z_{j+1}\cap\Omega_{j+1})\exp[-\frac12\langle A_j,C^*\Delta^{(j)}CA_j\rangle]\) | [IV] p.188 source input | Same form in \(\tilde A_j\): a product of balls. The dependence of the B-terms on \(\tilde A_j\) is analytic; the cutoff \(g(A')\), which made it only \(C^\infty\), is gone |
| Positivity of the postponed Gaussians, (1.79) | [LFR II] p.383 (assumed input; FS §2.4) | Unchanged quadratic form in \(A_j=\Phi(\tilde A_j)\); the shift is \(\le2\eta_j\) |
| R′ kernel (1.100), \(\chi(\Lambda_i)\) (1.101), normalization (1.102) | [IV] p.201 source input | Uses \(U_{k,X_i}(V'_kV_{\Lambda_i})\), component-local. Unchanged |
| Second-class test \(\chi_k(X^{\sim-6})\), growth (1.76), reserve induction | [LFR II] pp.378, 381 source input | Do not read the R-test. Unchanged. The per-cube R-factor is the same up to \(1-O(\eta/t)\) |
| \(\mathbf T'_k(X)\): expansion of \(V(X^\sim)\) to first order | [LFR II] p.379 source input | The terms of \(\mathscr V\) with localization in \(X^\sim\) are B-terms and join \(V(X^\sim)\); bounded by \(g^{\kappa_0}\) |

Not read: [LFR II] pp.355–377. Any use of the R-test there is unexamined.

### 7.2 The preparatory test [IV] (1.55): a second global-background test (F5)

**Source.** [IV] p.180: "\(U^{(n)}_k=U^{(n)}_k(V)=U(\mathbb B^{(n)}_k,V)\). (1.18) These configurations are background fields in the successive integrations", with \(\mathbb B^{(n)}_k\supset\mathbb B_k\cap(\Omega_k\cup Z^c)\), the determining set of the whole lattice; and (1.20) the localized \(U^{(n)}_{k,Z}=U(\mathbb B^{(n)}_k(Z),(M^\cdot(Q^{s*}_kV_k)\restriction_{Z\cap\Omega_k},V\restriction_{Z\cap\Omega^c_k}))\). p.187: "(1.53) \(V'_j=V_j(V^{(j)})^{-1}\), \(V^{(j)}=M^j(U^{(n+1)}_k)\), \(B'_j=\frac1i\log V'_j\)". p.188: "(1.55) \(\chi'^{(j)}=\chi(\{|B_j(b)|<\delta'_j\) for \(b\in(\Omega^c_{j+1}\setminus Z''_{j+1})^{(j)*}\})\). We exclude from \(Z\) the components with the large field function \(1-\chi'^{(j)}\)"; (1.56)–(1.58): \(V^{(j)}=\exp i\mathbb H^{(j)}_ZV^{(j)}_Z\), \(\mathbb H^{(j)}_Z\) "is an analytic function of the configuration \(U^{(n+1)}_k\) restricted to \(Z\), and on \((\Omega^c_{j+1}\setminus Z''_j)^{(j)}\) it is bounded by \(O(1)\exp(-R_j)\varepsilon_j\)"; then the change of variables (1.22) [III] "for the bonds belonging to … the components of this set with the large field function \(1-\chi'^{(j)}\)", giving (1.59).

**Consequence.** The cutoff of (1.22) is the identity near the threshold, so the failure event of (1.55) is \(\{\exists b:|\log(V_j(b)M^j(U^{(n+1)}_k)(b)^{-1})|\ge g_j\delta'_j\}\). It depends on the fields outside the component through \(\mathbb H^{(j)}_Z\). This label is a record of the construction (a preparatory failure; IM §3 and RB §1.3 list it among the failure records). So the literal R operation has a non-local label rule of exactly the kind of (3.16), and the cone obstruction of TC Prop. 2.1 applies to it as well. TM §5.2 item 6 and IM §3 quote the p.183 sentence ("all the characteristic functions introduced above depend on the field variables localized in the corresponding components"), which precedes (1.55) and does not cover it.

**Amendment (A8).** Test \(B^Z_j(b):=(ig_j)^{-1}\log(V_j(b)V^{(j)}_Z(b)^{-1})\) against \(\delta'_j\), in every component. Then:
* the label is a function of the fields in the component (the backgrounds \(U^{(n+1)}_{k,Z}\) are component-local by (1.20));
* \(|B^Z_j|<\delta'_j\) implies the function (1.27) (which tests the same quantity at \(2\delta'_j\)), so on passing components (1.27) is dropped, and on failing components the product is (1.59), the form the source reaches;
* in passing components the integration variable of (1.60) is \(B^Z_j\), and the exponent acquires \(\mathscr A(\varphi_{\mathbb H_Z}(B^Z))-\mathscr A(B^Z)+\log\det\). "The integration in (1.60) is localized in the large field region \(Z\), therefore the integral contributes to the boundary terms only" (p.189, source). The new terms are boundary terms \(\mathbb C^{(n+1)}_k\) and satisfy (1.70) with room, by the bound on \(\mathbb H^{(j)}_Z\). No bulk term, no tube localization, no R-class booking is needed here;
* the smallness of \(\mathbb H^{(j)}_Z\) is the source's (1.57), a decay across at least \(MR_k\) (many tiles). It is a far-carrier use: T′♯ or CT♯ (data in the boundary layer of \(Z\), fixed real background) covers it. assumed input

The formula gives the remaining tests of [IV] in the source: (1.22)–(1.24) (\(U^{(n)}_{k,Z}\)), (1.27) (\(V^{(j)}_Z\)), (1.75) (\(U_{k,Z}\)), (1.82) (\(V_0=M_{\mathbb B''}(U_0)\), \(U_0=U_{k,Z}(V_\Lambda)\)), (1.88) (\(U^{(0)}_{h,\square}\)), (1.101). All use component-local backgrounds.

## 8. The locality statement H-02 needs

**(FP)** (TC §5.1): every label at \((n,\square)\) is a function of the bare links and seeds within distance \(\rho S_n\) and of labels at earlier sub-steps within that distance.

**Proposition 8.1 — conditional**; replaces TC Lemma 5.2 and Prop. 5.3. For the construction defined in §2, with (A1) **and** (A8):
1. The \(R^{\rm loc}\)-label of \(\square'\) at step \(k+1\) is a function of \(V_k\) on \((\square'^{\sim2})^{(k)*}\) and of \(V_{k+1}\) on \(\{x:{\rm dist}_\infty(x,\square')\le(L+8)LM_2R_{k+1}\}\) (Definition 2.2, (B4)). It is history-free: it does not depend on the domains \(\Omega_j,\Lambda_j\) except through the fact that the test is made.
2. It is invariant under gauge transformations of \(V_{k+1}\) and covariant under the lattice isometries preserving the partitions (Proposition 5.1).
3. It agrees with the literal label outside the collar \(|\sup|A_k|-t_k|\le2\eta_k\) (Lemma 4.2). conditional
4. The preparatory label (1.55) in the form (A8), and the labels (1.22)–(1.24), (1.27), (1.28), (1.75), (1.82), (1.88) of [IV], are functions of the fields in the eligible component, which lies in a cube of side \(100MR_k\) ([IV] p.177 (i)). (c-text for the definitions; deduction for the conclusion)
5. Given TM §5.2 items 1–5 and 7 at TM's labels (P- and Q-tests, second-class test, growth, eligibility, resampling kernel; c/c\*), (FP) holds for every label rule, with range \(\rho S_n\), \(\rho\) independent of \(n\), and cumulative range \(\le C\rho S_n\) (TC Prop. 5.3's geometric sum).

Hence TC Theorem 5.1 applies to this construction on its stated inputs. TC Prop. 5.3 as stated (only (3.16) replaced) is **false**: with the literal (1.55) the preparatory-failure records are not tile-local.

*Proof.* 1–3 are proved above. 4: §7.2. 5: composition, as in TC. \(\square\)

Covariance of the assignments and locality of the eliminated-bond choices are required as assumptions for the local-test estimates.
