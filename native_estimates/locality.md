# Restriction to a level-adapted interior

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 3. Geometry

### 3.1 Domains, sequences, data

Fix a scale \(s\). The fine lattice is the original lattice, with spacing \(\xi=L^{-s}\) in step-\(s\) units. Levels are absolute: write \(\ell_n:=L^n\xi\) for the side of a level-\(n\) block. A *domain* is a finite union of level-0 big blocks (side \(M_1\ell_0\)), of any class.

The *maximal sequence* of \(Z\) (CMP109 clause (iv): "the sequence \(\{\Omega_n\}\) … of maximal possible domains satisfying the conditions (1.3)–(1.6) [14]", with \(R=R_1\)) is:
\[
\Omega_0(Z)=Z,\qquad \Omega_{p+1}(Z)=\bigcup\{c:\ c\text{ a level-}(p+1)\text{ big block},\ c\subset\Omega_p(Z),\ \mathrm{dist}(source input; \Omega_p(Z)^c)\ge R_1M_1\ell_p\}.
\]
This is [V] (1), p.277 source: "\(\Omega_j\) is a union of big block of the size \(M_1L^j\eta\), \((L^j\eta)^{-1}\mathrm{dist}(\Omega_j^c,\Omega_{j+1})>RM_1\)".

> **(G1)** (reading additional assumption). "Maximal possible" means the union of all admissible blocks. This is well defined, because the admissible family is closed under unions.

Write \(\nu_Z(x):=\max\{p\le n:\ x\in\Omega_p(Z)\}\) for the *\(Z\)-level*. As in CMP109 (1.15), the data of \(\mathbf U\) for the \(Z\)-problem at top level \(n\) are \(M'_Z(\mathbf U)=(\bar{\mathbf U}^p\text{ on }\Lambda_p(Z))_{p\le n}\), where \(\Lambda_0(Z)\) is the outer collar and the field itself is prescribed there. The **reconstruction** is \(R_n[Z](\mathbf U):=U_n(Z;M'_Z(\mathbf U))\): the minimiser of [V] Theorem 1 on the sequence \(\{\Omega_p(Z)\}_{p\le n}\), in the axial gauge, continued analytically by [V] Proposition 9.

**Lemma 3.1.** Let \(Z\subset Z'\).

1. \(\Omega_p(Z)\subset\Omega_p(Z')\) for every \(p\). Hence \(\nu_Z\le\nu_{Z'}\) on \(Z\).
2. If \(\mathrm{dist}_1(x,Z^c)\ge2(1+dL)R_1M_1\ell_{n-1}\), then \(x\in\Omega_n(Z)\). More precisely, \(\mathrm{dist}_1(x,\Omega_n(Z)^c)\ge\mathrm{dist}_1(x,Z^c)-2(1+dL)R_1M_1\ell_{n-1}\) for \(L\ge2\).
3. Let \(\mathbf U\) be any configuration on \(Z'\), and \(W'\) any configuration on \(Z'\) with the same \(Z'\)-data. Then \(M'_Z(\mathbf U)\) and \(M'_Z(W')\) can differ only on \(\Gamma:=\{\nu_Z<\nu_{Z'}\}\cap\mathfrak B(Z)\subset Z\setminus\Omega_n(Z)\).

*Proof.* (1) By induction on \(p\). If \(\Omega_p(Z)\subset\Omega_p(Z')\), a block admissible for \(Z\) lies in \(\Omega_p(Z')\). Its distance to \(\Omega_p(Z')^c\) is at least its distance to \(\Omega_p(Z)^c\). So it is admissible for \(Z'\), and (G1) gives the inclusion.

(2) A level-\((p+1)\) big block has \(\ell^1\)-diameter at most \(dM_1\ell_{p+1}\). If \(\mathrm{dist}_1(x',\Omega_p^c)\ge R_1M_1\ell_p+dM_1\ell_{p+1}\), the block containing \(x'\) is admissible. Hence \(\mathrm{dist}_1(x,\Omega_{p+1}^c)\ge\mathrm{dist}_1(x,\Omega_p^c)-R_1M_1\ell_p-dM_1\ell_{p+1}\). Summing over \(p<n\) and using \(M_1\le R_1M_1\) and \(\sum_{p<n}(L^p+dL^{p+1})\le2(1+dL)L^{n-1}\) (check (3)) gives the claim.

(3) On \(\{\nu_Z=\nu_{Z'}=q\}\) both data are the level-\(q\) averages at the same points, and these coincide because the \(Z'\)-data agree. The inclusion \(\Gamma\subset Z\setminus\Omega_n(Z)\) holds because \(\nu_Z<\nu_{Z'}\le n\). \(\square\) deduction, given (G1). Check (5a) tests (1) on random 2D domains.

### 3.2 The region of clause (iv)

For a domain \(Z\) and a level \(n\) put
\[
Z^{(n)}:=\{x\in Z:\ \mathrm{dist}_1(x,Z^c)\ge 2M\ell_{n-1}\}.
\tag{3.1}
\]
This region depends only on \(Z\) and on the absolute level \(n\). In particular \(Z\subset Z'\Rightarrow Z^{(n)}\subset Z'^{(n)}\), because \(\mathrm{dist}(x,Z^c)\le\mathrm{dist}(x,Z'^c)\). For \(M\ge(1+dL)R_1M_1\), Lemma 3.1(2) gives \(Z^{(n)}\subset\Omega_n(Z)\), and every \(x\in Z^{(n)}\) lies at \(\ell^1\)-distance at least \((2M-2(1+dL)R_1M_1)\ell_{n-1}\) from \(\Omega_n(Z)^c\supset\Gamma\).

### 3.3 The literal regions are not nested

CMP109 p.262 source: "The domain \(\tilde X^{-2}\) is obtained from \(X\) by taking away two layers of cubes from \(\pi_j\) which are closest to the boundary of \(X\)." The same region serves every level \(n\le j\). For the scale-\((k+1)\) spaces on domains of class \(\mathbf D_k\) (\(\square_0\), \(Y\)), the source uses layers of \(\pi_k\): Step 0 of Lemma 5.1 reads clause (iv) of \(U^c_{k+1}(\square_0,\cdot)\) on \(\tilde\square^3=\square_0^{-2}\) with \(\square_0=\tilde\square^5\) (CMP109 p.273: "\(\tilde\square^4\subset\square_{k+1}\)"). In step-\(k\) units the thicknesses are:

| space | domain class | thickness of "\(-2\)" |
|---|---|---|
| scale \(k+1\), native | \(\mathbf D_{k+1}\) (polymers \(X\)) | \(2LM\) |
| scale \(k+1\), potential domain | \(\mathbf D_k\) (\(Y\), \(\square_0\)) | \(2M\) |
| scale \(j=k-m\), native | \(\mathbf D_j\) (far carriers \(X\)) | \(2ML^{-m}\) |

If \(A\subset B\) with thicknesses \(t_A,t_B\), then \(A^{-t_A}\subset B^{-t_B}\) for all such pairs if and only if \(t_A\ge t_B\). So:

- (S-Res-2), \(\square_0\subset Y\): \(2M\ge2M\). Nested.
- (X-far) at \(m=0\), \(X\in\mathbf D_k\subset Y\): \(2M\ge2M\). Nested.
- (S-Res-1), \(Y\subset X\in\mathbf D_{k+1}\): \(2M\ge2LM\) fails. In CMP116 p.15 the potential domain satisfies \(Y\subset Z_0\) and \(\tilde Z_0\subset X\), where the tilde adds one layer of \(M\)-cubes (CMP116 p.12: "the tilde over \(Z_0\) concerns \(M\)-cubes"). Then \(Y^{-2}\) lies at distance \(\ge3M\) from \(X^c\), while \(X^{-2}\) needs \(2LM>3M\) for \(L\ge2\).
- (X-far) at \(m\ge1\), \(X\in\mathbf D_j\subset Y\): \(2ML^{-m}\ge2M\) fails for \(X\) within \(2M\) of \(\partial Y\). This happens generically: \(Y\supset X_0\), the smallest \(\mathbf D_k\)-domain containing \(X\), may share boundary with \(X_0\) (CMP116 p.8).

Where the target region is not inside the source region, the source's clause (iv) contains no information about the reconstructions there. Check (5c) gives an explicit 2D instance.

### 3.4 The level-adapted convention (iv\(_t\))

> **(iv\(_t\))** In the definition of \(U^c_s(Z,\alpha_0,\alpha_1,\gamma_0)\) (CMP109 (1.11)–(1.16)), replace clause (iv) by: *for \(n=1,\dots,s\), the pair \((U_n(Z;M'(\mathbf U)),J_n(Z;M'(\mathbf U)))\) satisfies \(|\partial U_n-1|<\alpha_0\xi^2\) and \(|J_n|<\alpha_0\ell_n^2\) on \(Z^{(n)}\) of (3.1); and the same holds for \(U\) in place of \(\mathbf U\).*

This changes the source's region in two ways. At the top level of a native space (\(n=s\)) the margin becomes \(2M\ell_{s-1}=2M/L\) step-\(s\) units instead of \(2M\). At lower levels the margin is smaller still. A smaller margin is a **stronger** condition, so the (iv\(_t\))-spaces are *subsets* of the source's spaces. The conditions concern the absolute objects \(U_n(Z;\cdot)\) on absolute regions, so they nest across scales and classes. For the scale-\((k+1)\) spaces on \(\mathbf D_k\)-domains, the level-\((k+1)\) region is \(2M\ell_k=2M\) step-\(k\) units: exactly the source's \(\tilde\square^3\) inside \(\square_0=\tilde\square^5\).

## 4. Statement

**Setting.** A configuration \(\mathbf U\) on \(Z'\) at scale \(s\) is in \(\mathcal K_s(Z';a_0,a_1)\) if it satisfies the plaquette parts of CMP109 (1.11), (1.13), (1.14). That is: \(\mathbf U=U'U\) with \(U\) \(G\)-valued and \(|\partial U-1|<a_0\xi^2\); \(U'=\exp i\xi A'\) with \(A'\) \(\mathfrak g^c\)-valued and \(|A'|,|\nabla^\xi_UA'|<a_1\); and \(|\partial\mathbf U-1|<a_0\xi^2\). The variable \(\mathbf J\) plays no role, because reconstructions depend on \(\mathbf U\) only.

**Constants.**

- \(B_0\), \(B_3\): from [V] (161), (162).
- \(K_9\): the \(O(1)\) of [V] (190).
- \(C_p,C_J\): absolute constants of the basic estimate [R] (1.43)–(1.54), for the plaquette and the current of \(e^{i\eta A}U_0\).
- \(C_u\): the constant in [R] (1.70)–(1.71).
- \(C_A\): the absolute constant in \(|\partial(e^{i\xi A_1}U)-\partial(e^{i\xi A_2}U)|\le C_A\xi^2(|\nabla_U(A_1-A_2)|+(|A_1|+|A_2|)|A_1-A_2|)\), from the same estimate.
- \(\delta_0\): the decay rate.
- Derived constants:
\[
S_{1/2}:=\sup\sup_{z}\sum_{y'}e^{-\frac12\delta_0d(z,y')}(L^{j'}\eta)^{-1}\ \le\ \frac{B_3}{72d^3L^3B_0},\qquad
K_R:=\frac{11}{9}\,\frac{\max\{C_p,C_J\}\,K_9\,B_3^2}{L^3B_0},
\]
\[
T(D):=\sum_{t\ge D}(2t+1)^de^{-\delta_0t/2}\le C_Te^{-\delta_0D/4},\qquad D_0:=\frac{2M-2(1+dL)R_1M_1}{L}-d,\qquad \omega_0:=\tfrac4\pi\arctan\tfrac12.
\]

The bound on \(S_{1/2}\) is (162) with \(d+1\ge1\). The bound on \(T(D)\) is elementary, with \(C_T=\sum_t(2t+1)^de^{-\delta_0t/4}\) (check (4)). The value of \(\omega_0\) is checked in check (1).

**Inputs.**

| | Statement used | Source | Status |
|---|---|---|---|
| (V1) | For an admissible sequence and real data \(V\) with (7), \(\varepsilon_1\le a_1\): a minimal orbit exists in \(\mathfrak U_k(\{\Omega_j\},B_3\varepsilon_1)\cap\mathfrak B_k(\mathfrak B_k,V)\), and it is "a unique critical orbit in the space (6) if \(B_3\varepsilon_1\le\varepsilon_0\) and \(\varepsilon_0\le a_0\)" | [V] Theorem 1, p.279 | source input |
| (V2) | "The minimal configuration \(U_k(V)=U_k(V'V_0)\) in the axial gauge has an extension to an analytic function of \(G^c\)-valued small configurations \(V'\)" (\(V'=e^{iB'}\), \(|B'|<2C_1\varepsilon_1\), (172)). Transformed to the Landau gauge, \(U_k(V'V_0)U_k(V_0)^{-1}=\exp i\eta\mathcal H(B)\). Extension to orbits by (181) | [V] Proposition 9, p.309; (172), (181), p.306–307 | source input |
| (V3) | Derivative bound (190) for \(\delta\mathcal H/\delta B\), with \(\nabla\), \(D^*D\), \(\Delta\), for \(x\in\Delta(y)\), \(y\in\Lambda_j\), \(y'\in\Lambda_{j'}\) | [V] (190), p.308 | source input |
| (R190) | Reading of (V3): integrated against a perturbation \(b\), at a top-level point (\(L^j\eta=1\)), the four quantities are bounded by \(K_9\sum_{y',\nu}e^{-\frac12\delta_0d(y,y')}(L^{j'}\eta)^{-1}|b_\nu(y')|\). This is the bound (161) for the linear part \(H\), with \(\delta_0\to\frac12\delta_0\). Basis: "We will prove that this derivative has regularity and decay properties identical to the propagator \(H\), or \(H_0\)" (p.307), and the printed factor \((L^{j'}\eta)^{-d}\) is compensated by the volume element of the level-\(j'\) sum | [V] p.307–308 | additional assumption |
| (V4) | (162) and "\(B_3\) depends on \(d\) and \(L\) only" | [V] p.303 | source input |
| (V5) | "the conditions (1.33)–(1.35) imply \(\lvert(\overline{U'U_0})^j-\bar U_0^j\rvert=\lvert\bar U'^j-1\rvert<11d^2\alpha_0+\alpha_1\) on \(\Omega_j^{(j)}\)" (1.65). Its derivation uses only the plaquette conditions (1.7), Lemma 1 and Proposition 2 of [A] (reading (d) of p.87) | [R] p.87 | source input; additional assumption |
| (V6) | The Landau-gauge transformation \(u\) is "determined uniquely in terms of \(U_1\) and is given by (106)", with \(\lvert u_1(x)-1\rvert\le2\sum_n\max\lvert\frac1i\log(\bar R^n\bar U_1^n)(\Gamma_{x_{n+1},x})\rvert\) (1.70), each term \(\le\lvert Q_n(U_0,\eta A)(\Gamma)\rvert+O(\lvert Q_n\rvert^2)\) (1.71). This is local along the chain of blocks of \(x\) | [R] p.88 | source input |
| (V7) | Basic estimate: the plaquette and \(D^*\partial\) of \(e^{i\eta A}U_0\) expanded in \(A\), with absolute constants | [R] (1.43)–(1.54), pp.83–86 | source input, in the source; constants assumed |
| (V8) | CMP109 (1.17): \((\mathbf U,\mathbf J)\) satisfying (i)–(iii) with \(\alpha'_0\) has \(\lvert\partial U_n(M'\mathbf U)-1\rvert<2B_3\alpha'_0\xi^2\) and \(\lvert J_n\rvert<2B_3\alpha'_0\ell_n^2\). Printed "on \(\tilde X^{-2}\)"; read as valid on \(\Omega_n(X)\) (it is [V] Theorem 1, Proposition 9 on the top-level region) | CMP109 p.263 | source input; additional assumption |
| (G2) | Finer data determine coarser constraints. If \(\nu_Z\le\nu_{Z'}\), every \(Z'\)-constraint whose support meets \(\Omega_1(Z)\) is a function of the \(Z\)-data and of the field on \(Z'\setminus\Omega_1(Z)\). Source precedent: [V] (11)–(13), p.279–280, and (147)–(150), p.301 | [V], [A] | source input; additional assumption |
| (G3) | The axial conditions [R] (1.19) at \(x_0\) involve only the chain \(x_0,\dots,x_{\nu(x_0)}\) of the global block hierarchy. Hence \(\mathrm{Ax}(\mathfrak B(Z'),1)\vert_Z\subset\mathrm{Ax}(\mathfrak B(Z),1)\) when \(\nu_Z\le\nu_{Z'}\), and the reconstruction functions are axial relative to 1 | [R] p.79 | additional assumption |

> **Theorem 4.1 (locality of reconstructions).** There is a ceiling \(c_*>0\), depending only on \(d\), \(L\) and the source constants above, such that the following holds. Take any scale \(s\), any \(1\le n\le s\), any domains \(Z\subset Z'\) of any classes, any \(M\ge(1+dL)R_1M_1+L(d+1)\), and any \(\mathbf U\in\mathcal K_s(Z';a_0,a_1)\) with \(B_3^2(a_0+a_1)\le c_*\). (The ceiling on \(a_1\) carries the factor \(B_3^2\) because Step E applies part (a) at curvature \(a_*\).) Put \(W:=R_n[Z](\mathbf U)\) and \(W':=R_n[Z'](\mathbf U)\). Then for every plaquette \(p\) and bond \(b\) of \(Z^{(n)}\):
> **(a) Real case** (\(\mathbf U=U\) is \(G\)-valued):
> \[
> |\partial W(p)-\partial W'(p)|\le K_RT(D_0)\,a_0\,\xi^2,\qquad |J_n(W)(b)-J_n(W')conditional|\le K_RT(D_0)\,a_0\,\ell_n^2.
> \]
> Also \(W'|_Z=U_n(Z;M'_Z(W'))\) on all of \(Z\) (Step A).
> **(b) Complex case:** with \(a_*:=a_0+4C_Aa_1\),
> \[
> |\partial W(p)-\partial W'(p)|\le\Theta_{\mathbb C}\,\xi^2,\quad |J_n(W)(b)-J_n(W')conditional|\le\Theta_{\mathbb C}\,\ell_n^2,\qquad \Theta_{\mathbb C}:=4B_3\,a_*\Big(\frac{K_RT(D_0)}{4B_3}\Big)^{\omega_0}.
> \]
> All constants are independent of \(s,n,Z,Z'\), the age, and \(\mathbf U\).

> **Corollary 4.2 (transfer of clause (iv)).** Under the hypotheses of Theorem 4.1, let \(S\subset Z^{(n)}\) be any set on which \(W'\) satisfies \(|\partial W'-1|<a\xi^2\) and \(|J_n(W')|<a\ell_n^2\). Then \(W\) satisfies the same bounds on \(S\), with \(a\) replaced by \(a+\Theta\) (\(\Theta=K_RTa_0\) in the real case, \(\Theta_{\mathbb C}\) in the complex case). The same holds for the real factor \(U\), with the real \(\Theta\). Under (iv\(_t\)) take \(S=Z^{(n)}\subset Z'^{(n)}\). Under the literal convention, take \(S\) to be the target's literal region, whenever it lies inside the source's literal region.

*Proof of the corollary.* Triangle inequality. \(\square\)

## 5. Proof of Theorem 4.1

Units: for the level-\(n\) subproblem Use the units of [V], in which the level-\(n\) blocks have side 1 and the fine spacing is \(\eta_n:=\xi/\ell_n\). Dimensionless quantities (plaquette deviations, bond angles of data) do not change between units.

### 5.1 Step A: identity on \(Z\) (real \(U\))

Let \(\mathbf U=U\) be real, with curvature radius \(a_0\).

1. *Data.* By Proposition 2 of [A] (quoted in [R] p.87: "the bounds \(|\partial U-1|<\alpha_0\eta^2\) imply \(|\partial U^j-1|<\ldots<2\alpha_0L^{2j}\eta^2\)"), the \(Z'\)-data satisfy [V] (7) with \(\varepsilon_1:=2a_0\ell_n^2\).
2. *Regularity of \(W'\).* By (V1), \(W'\in\mathfrak U_n(\{\Omega_p(Z')\},B_3\varepsilon_1)\). The regularity conditions [V] (2) at level \(p\) on \(\Omega_p\), namely \(|\partial U-1|<\varepsilon_0L^{-2p}\) and \(|D^*\partial U|<\varepsilon_0L^{-2p}(L^p\eta)^{-1}\), weaken as \(p\) decreases. Since \(\nu_Z\le\nu_{Z'}\) (Lemma 3.1), \(W'|_Z\in\mathfrak U_n(\{\Omega_p(Z)\},B_3\varepsilon_1)\).
3. *Restriction is critical.* Write \(\mathcal M_Z\) for the set of configurations on \(Z\) whose \(Z\)-data equal \(M'_Z(W')\), and \(\iota\) for extension by \(W'\) on \(Z'\setminus Z\). On \(\Lambda_0(Z)=Z\setminus\Omega_1(Z)\) the field is prescribed, equal to \(W'\). So \(\iota Y=W'\) off \(\Omega_1(Z)\), and by (G2), \(\iota\mathcal M_Z\subset\mathcal M_{Z'}\). The plaquette sets satisfy "plaquettes with a corner in \(Z\)" \(\subset\) "plaquettes with a corner in \(Z'\)", and every plaquette of \(Z'\) without a corner in \(Z\) sees only bonds where \(\iota Y=W'\). Hence \(A_{Z'}(\iota Y)=A_Z(Y)+\mathrm{const}\). \(W'\) is critical for \(A_{Z'}\) on \(\mathcal M_{Z'}\), so \(W'|_Z\) is critical for \(A_Z\) on the submanifold \(\mathcal M_Z\). deduction, given (G2).
4. *Uniqueness.* The \(Z\)-data of \(W'\) satisfy (7) with \(\varepsilon_1^\circ\le2B_3\varepsilon_1\) (Proposition 2 of [A] again). Take \(\varepsilon_0:=2B_3^2\varepsilon_1\). Then \(B_3\varepsilon_1^\circ\le\varepsilon_0\le a_0^{[V]}\) by the ceiling, and \(W'|_Z\) lies in the space (6) of the \(Z\)-problem (monotonicity in \(\varepsilon_0\)). By (V1) it lies on the minimal orbit, which is the orbit of \(\hat W:=U_n(Z;M'_Z(W'))\) under the subgroup (4) for \(\mathfrak B(Z)\).
5. *Same element.* By (G3), \(W'|_Z\) and \(\hat W\) both satisfy \(\mathrm{Ax}(\mathfrak B(Z),1)\). [R] p.79 source: "The conditions (1.19) determine uniquely an element in each orbit given by the subgroup (1.14)". Hence \(W'|_Z=\hat W\). conditional

*Remark.* This is the argument of [V] p.301, used there for nested cubes source: "The configuration \(U'_k\) is a minimum of the functional (5) in the space (6) with \(V'\) instead of \(V\), hence it is a minimum of this functional in the space (150), because this space is defined by more restrictive functional conditions and a sufficiently small neighborhood of \(U'_k\) in (150) is contained in (6)." It is also the content of CMP109 (3.38) ("a minimiser of a minimiser"), used in Step 5 of Lemma 5.1 of L1\(^*\).

Without (G3) the conclusion is "\(W'|_Z=\hat W\) up to a \(G\)-valued gauge transformation". That suffices for every real statement below, because \(|\partial\cdot-1|\) and \(|J|\) are invariant under unitary gauge transformations. (G3) is used only to define \(F\) in Step E as an analytic function with no gauge ambiguity.

### 5.2 Step B: the data difference lives on \(\Gamma\) and is \(O(B_3a_0)\)

Gauge-transform \(U\) by an element of the subgroup (1.14) for \(\mathfrak B(Z')\), so that \(U\in\mathrm{Ax}_n(\mathfrak B(Z'),W')\). This changes neither the data nor \(W'\). Then \(U=U'W'\) in the notation of [R]. With \(U_0:=W'\), the hypotheses of (V5) hold:

- both configurations satisfy (1.7) for the \(Z'\)-sequence with \(\alpha_0^{[R]}:=\max\{a_0\ell_n^2,\,B_3\varepsilon_1\}=2B_3a_0\ell_n^2\). For \(U\) this is because \(a_0\xi^2=a_0\ell_n^2\eta_n^2\le a_0\ell_n^2L^{-2p}\); for \(W'\) it is item 2;
- (1.35) holds with \(\alpha_1^{[R]}=0\), because the \(Z'\)-data coincide.

So \(|\bar U'^p-1|<11d^2\cdot2B_3a_0\ell_n^2\) on \(\Omega_p(Z')^{(p)}\) for all \(p\). The data perturbation for the \(Z\)-problem is \(V'=M'_Z(U)\,M'_Z(W')^{-1}\) bond by bond. This is \(\bar U'^p\) of [R] (1.20) at the \(Z\)-level \(p\). By Lemma 3.1(3), \(V'=1\) off \(\Gamma\). With \(B:=\frac1i\log V'\) and \(|\log(1+x)|\le2|x|\) for \(|x|\le\frac12\) (ceiling),
\[
B=0\ \text{off }\Gamma,\qquad |B|\le b_{\max}:=44\,d^2B_3\,a_0\,\ell_n^2\quad\text{on }\Gamma.
\tag{5.1}
\]
Status conditional, from (V1), (V5), Proposition 2 of [A].

This is the "collar bound" the L1\(^*\) outline asks for. Its constant contains \(B_3\), because near \(\Gamma\) the only regularity known for \(W'\) is that of Theorem 1.

### 5.3 Step C: decay into \(Z^{(n)}\)

Apply (V2) around the real datum \(V_0:=M'_Z(W')\). The minimiser there is \(\hat W=W'|_Z\), so \(\mathcal H(0)=0\). Choose \(\varepsilon^{(9)}:=\max\{\varepsilon_1^\circ,\,b_{\max}/2C_1\}\). The ceiling gives \(\varepsilon^{(9)}\le a_1^{[V]}\), so \(B\) lies in the domain (172). Then
\[
W=\big(e^{i\eta_n\mathcal H(B)}\,\hat W\big)^{u}\quad\text{with }u\text{ unitary},\qquad \mathcal H(B)=\int_0^1\frac{\delta\mathcal H}{\delta B}(tB)\,B\,dt.
\]
Fix a top-level point \(y\in\Lambda_n(Z)\) whose block lies within \(\ell^1\)-distance \(d\ell_n\) of \(Z^{(n)}\).

**Splitting the distance.** Let \(y'\in\Gamma\). An optimal contour from \(y\) to \(y'\) leaves \(\Omega_n(Z)\) at a first point \(z\in\Lambda_n\cap\Sigma_n\). Up to \(z\) it consists of level-\(n\) bonds (CMP96 (2.46)). Hence
\[
d(y,y')\ge|y-z|_1/\ell_n+d(z,y'),\qquad |y-z|_1/\ell_n\ge D_0
\]
by §3.2.

**Bounding the four quantities.** By (R190), with \(B\) supported on \(\Gamma\) and bounded by (5.1), the quantity
\[
h:=\max\{|\mathcal H|,|\nabla\mathcal H|,|D^*D\mathcal H|,|\Delta\mathcal H|\}(x)
\]
satisfies, at \(x\in\Delta(y)\),
\[
h\le K_9\,d\,b_{\max}\sum_{z:\ |y-z|_1\ge D_0\ell_n}e^{-\frac12\delta_0|y-z|_1/\ell_n}\ \sup_z\sum_{y'}e^{-\frac12\delta_0d(z,y')}(L^{j'}\eta)^{-1}
\le K_9\,d\,b_{\max}\,T(D_0)\,S_{1/2}.
\]
Here the number of level-\(n\) points at \(\ell^1\)-distance \(t\ell_n\) is at most \((2t+1)^d\). With \(S_{1/2}\le B_3/(72d^3L^3B_0)\),
\[
h\ \le\ \frac{11}{18}\,\frac{K_9B_3^2}{L^3B_0}\,T(D_0)\,a_0\ell_n^2.
\tag{5.2}
\]
Status conditional, from (V2), (R190), (V4). Note that the contribution of every layer of every collar is absorbed by the single sum \(S_{1/2}\), which is the sum defining \(B_3\). No per-layer "\(e^{-\delta_0R_1M_1}\) against \(L^2\)" bookkeeping (L1\(^*\) outline, step 4) is needed.

### 5.4 Step D: plaquettes and currents (real case)

Let \(P_2:=\partial(e^{i\eta_n\mathcal H}\hat W)(p)\) and \(P_1:=\partial\hat W(p)=\partial W'(p)\).

**Plaquettes.** By (V7) (BCH, as in [R] (1.21), (1.47)–(1.49)), \(|P_2-P_1|\le C_p\eta_n^2(h+h^2)\).

**Gauge factor.** In these units the top-level block has side 1, and \(|Q_{n'}(U_0,\eta_n\mathcal H)(\Gamma)|\le c\,L^{n'+1-n}\sup|\mathcal H|\) for the chain contours. So (V6) gives \(|u(x)-1|\le C_u\sup_{B^n(x)}|\mathcal H|\le C_uh\). The chain of \(x\) stays in its level-\(n\) block, which is covered by (5.2) because of the "\(-d\)" in \(D_0\). Hence
\[
|\partial W(p)-\partial W'(p)|=|uP_2u^{-1}-P_1|\le|P_2-P_1|+3|u-1|\,|P_2-1|\le\eta_n^2h\big(C_p(1+h)+12C_uB_3a_0\ell_n^2\big)\le2C_p\,\eta_n^2h
\]
under the ceiling. Here \(|P_2-1|\le|P_1-1|+|P_2-P_1|\le4B_3a_0\xi^2\), by (V1) on \(\Omega_n(Z')\). Converting with \(\eta_n^2\ell_n^2=\xi^2\) and (5.2):
\[
|\partial W(p)-\partial W'(p)|\le\frac{11}{9}\,\frac{C_pK_9B_3^2}{L^3B_0}\,T(D_0)\,a_0\,\xi^2\le K_RT(D_0)a_0\xi^2.
\]

**Currents.** \(J_n\) is (1.8) with spacing \(\eta_n\). By the basic estimate (1.54) of [R], \(J(e^{i\eta_nA}\hat W)-J(\hat W)=D^*D A\) plus terms bounded by \(C(|A|+|\nabla A|)(|A|+|\nabla A|+B_3a_0\ell_n^2)\). With \(A=\mathcal H\), this is at most \(C_Jh\le K_RT(D_0)a_0\ell_n^2\) in the clause-(iv) normalisation. The gauge factor is treated as above, since \(J\) transforms by \(R(u)\). This proves deduction. conditional

### 5.5 Step E: complex \(\mathbf U\), by two constants

Write \(A'=A'_r+iA'_i\) with \(A'_r,A'_i\) \(\mathfrak g\)-valued, and put \(\mathbf U_z:=\exp(i\xi(A'_r+zA'_i))\,U\) for \(z\in\mathbb C\). Then:

- \(\mathbf U_i=\mathbf U\);
- \(\mathbf U_x\) is \(G\)-valued for real \(x\);
- for \(|z|\le3\), by (V7) and (ii), \(\mathbf U_z\in\mathcal K_s(Z';a_*,4a_1)\) with \(a_*=a_0+4C_Aa_1\). The reason: \(|z-i|\le4\), the real and imaginary parts of \(A'\) and of \(\nabla_UA'\) are bounded by the whole (\(R(U)\) preserves hermiticity), and \(C_A\) absorbs the factor \(1+5a_1\).

Under the ceiling, the data of \(\mathbf U_z\) lie in the domain of (V2) around the real data of \(\mathbf U_{\mathrm{Re}\,z}\), for every \(|z|\le3\). Their imaginary part is \(O(a_1)\) in the dimensionless normalisation.

Define \(F(z):=\partial W(\mathbf U_z)(p)-\partial W'(\mathbf U_z)(p)\), using the axial representatives of (V2), (G3). \(F\) is analytic on a neighbourhood of the closed upper half-disc \(\bar H=\{|z|\le3,\ \mathrm{Im}\,z\ge0\}\) (composition of analytic maps; (181) makes \(U_n(\cdot)\) a single analytic function on the union of the orbits).

- On the diameter \([-3,3]\), part (a) gives \(|F|\le\varepsilon_I:=K_RT(D_0)a_*\xi^2\).
- On the arc, (V8) applied to \(Z\) and to \(Z'\) gives \(|F|\le F_{\max}:=4B_3a_*\xi^2\). The point \(p\) lies in \(Z^{(n)}\subset\Omega_n(Z)\subset\Omega_n(Z')\).

\(\log\|F\|\) is subharmonic. Let \(\omega\) be the harmonic measure of the diameter in the upper half-disc. Then \(\log\|F\|-\omega\log\varepsilon_I-(1-\omega)\log F_{\max}\) is subharmonic and \(\le0\) on the boundary, hence \(\le0\) inside (maximum principle; deduction).

**The constant \(\omega(i)\).** The map \(\zeta=(1+z/3)/(1-z/3)\) followed by \(\log\) sends the half-disc onto the half-strip \(\{\mathrm{Re}\,\sigma>0,\ |\mathrm{Im}\,\sigma|<\frac\pi2\}\). It sends the diameter to the end \(\mathrm{Re}\,\sigma=0\) and \(z=i\) to the real point \(\sigma=\log\frac{3+1}{3-1}\) (the problem is rotation-symmetric). The harmonic measure of the end is \(\frac4\pi\sum_{k\text{ odd}}\frac{(-1)^{(k-1)/2}}ke^{-k\sigma}\cos(k\,\mathrm{Im}\,\sigma)\). At \(\mathrm{Im}\,\sigma=0\) this equals \(\frac4\pi\arctan e^{-\sigma}\). So \(\omega(i)=\frac4\pi\arctan\frac12=\omega_0=0.5903\). Check (1) confirms this by Monte Carlo: \(0.5910\).

**Conclusion.** \(|F(i)|\le\varepsilon_I^{\omega_0}F_{\max}^{1-\omega_0}=\Theta_{\mathbb C}\xi^2\). The current is treated identically, using the second line of (V8). This proves conditional. conditional

*Why two constants rather than a complex Step B.* For complex \(\mathbf U\), a direct Step B needs a \(G^c\)-version of Lemma 1 of [R] with non-unitary parallel transports. Splitting through the real factor \(U\) gives data differences of size \(a_1\ell_p\). That would leave a factor \((a_1/a_0)\ell_n^{-1}\), unbounded for low levels \(n\), which is an artefact of the splitting. The two-constants argument uses only real configurations plus the crude bound (V8). It pays a power \(\omega_0\) in the exponent and a factor \(a_*/a_0\). The latter is \(\propto M\), by (K1) of L1\(^*\) (\(C_1/C_0\propto B_3^2c_\sharp M\)), and the exponential \(e^{-\omega_0\delta_0D_0/4}\) absorbs it (§6.2). \(\square\)

## 6. Consequences for (S-Res) and (X-far)

Write \(\varrho_1:=a_1/a_0\) for the radius ratio of the source space (\(C_1/C_0\) on the running chart) and
\[
\Theta_{\rm rel}(M):=4B_3\,(1+4C_A\varrho_1)\Big(\frac{K_RC_T}{4B_3}\Big)^{\omega_0}e^{-\omega_0\delta_0D_0/4},\qquad\text{so that }\ \Theta_{\mathbb C}\le\Theta_{\rm rel}(M)\,a_0.
\]

> **(K8)** \(\Theta_{\rm rel}(M)\le\beta/2\).

\(D_0\) grows like \(2M/L\), while \(\varrho_1\) grows at most linearly in \(M\) under (K1). So (K8) holds for \(M\ge M_0(d,L,\beta,\text{source constants})\). It does not depend on the scale, the age, the domains or the couplings. The quantifier order is that of L1\(^*\) §4.1 (remark on quantifiers): first \(L\), then \(M\), then the ratios \(c_2,c_3,C_1/C_0\), then the ceilings.

### 6.1 With the source's literal definitions

The relevant geometry is in §3.3. In each case where the literal regions are nested, the literal region of the target is contained in the target's \(Z^{(n)}\) for every relevant \(n\) (it is \(\{\mathrm{dist}\ge2M\}\) in step-\(k\) units, versus \(2M\ell_{n-1}\le2M\)), so Corollary 4.2 applies there.

- **(S-Res-2)** \(U^c_{k+1}(Y,(1+\beta)\alpha_0,\ldots)|_{\square_0}\subset U^c_{k+1}(\square_0,(1+2\beta)\alpha_0,\ldots)\). Clauses (i)–(iii) restrict trivially. Clause (iv) follows from Corollary 4.2 with \(a=(1+\beta)\alpha_0\) and the source curvature \((1+\beta)\alpha_0\). The new constant is \((1+\beta)(1+\beta/2)\alpha_0\le(1+2\beta)\alpha_0\) for \(\beta\le1\). The real factor is treated likewise. **Holds**, conditional.
- **(X-far), age 0.** \(K_\flat=1+\beta/2\). **Holds**, conditional.
- **(X-far), ages \(m\ge m_\flat\)** (true \(m_\flat\), finite but unknown, \(\ge5,4,3,3\) for \(L=3,5,7,13\)): by (1.17), as in L1\(^*\). **Holds**, conditional.
- **(X-far), \(1\le m<m_\flat\), and (S-Res-1).** On the part of the target region outside the source region, the hypothesis contains no clause-(iv) information. Theorem 4.1 still says the target reconstruction is within \(\Theta\) of the source reconstruction there, but the latter is bounded only by (1.17), i.e. \(2B_3\times\)curvature. The best literal statement is therefore the (1.17) one.
  - For (X-far) the question reduces to whether the true sup-norm amplification constant \(K_{\rm amp}\) of the reconstruction map satisfies \(K_{\rm amp}\le L^{2(m+1)}/(2(1+\beta)\Gamma_m)\) for \(m\ge1\). That would be true for any \(L\)-uniform \(K_{\rm amp}\) of moderate size. Only \(2B_3\gtrsim L^3\) is proved.
  - For (S-Res-1) one would need \(K_{\rm amp}\le1+\beta\). That is **plausibly false**: the reconstruction is an \(L^2\)-projection-type smoothing, whose \(L^\infty\) norm generically exceeds 1 (Gibbs-type overshoot). additional assumption

**Effect on CMP116 Lemma 1 under the literal definitions.** The statement analytic on \(U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\) holds for the near terms and for the far terms at ages 0 and \(\ge m_\flat\). For far terms at ages \(1\le m<m_\flat\) whose carrier \(X\) lies within \(2M\) (step-\(k\) units) of \(\partial Y\), it is **not established**. The subsequent use on p.15 (potentials analytic on \(U^c_{k+1}(X,\alpha_0,\alpha_1)\) for polymers \(X\)) is **not established** for \(Y\) within \(2LM\) of \(\partial X\).

### 6.2 Under convention (iv\(_t\))

All regions are \(Z^{(n)}\), so \(Z\subset Z'\Rightarrow Z^{(n)}\subset Z'^{(n)}\) (check (5b)). Corollary 4.2 together with (K8) gives:

- **(S-Res-1)** \(U^c_{k+1}(X,\alpha_0,\alpha_1)|_Y\subset U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\), for every \(Y\subset X\) of any classes.
- **(S-Res-2)** as in §6.1.
- **(X-far)** for every age \(m\ge0\) and every \(X\in\mathbf D_j\), \(X\subset Y\), with \(K_\flat=1+\beta/2\). The reconstructions \(U_n(\cdot)\), \(n\le j\), are the same absolute objects for the scale-\((k+1)\) space on \(Y\) and the scale-\(j\) space on \(X\). Source curvature and source clause-(iv) constant are both \((1+\beta)a_0L^{-2(m+1)}\) in scale-\(j\) normalisation, so the relative loss \(\Theta_{\rm rel}\) is scale-free.

The second half of L1\(^*\) (K7), \(K_\flat(1+\beta)\theta L^{-2}\le\frac12\), then holds for every \(L\ge2\): \((1+\frac18)(1.25)(1.05)/4=0.37\). The first half still needs \(L\ge3\).

### 6.3 Every use of clause (iv) survives (iv\(_t\))

| Use (L1\(^*\) numbering) | Needs | Under (iv\(_t\)) |
|---|---|---|
| CMP109 (1.17): (i)–(iii) imply (iv) with \(2B_3\) | bound on \(Z^{(n)}\subset\Omega_n(Z)\) | (V8) reading; unchanged |
| Lemma 5.1, Step 0: level \(k+1\) on \(\tilde\square^3\) | \(\tilde\square^3\subset\square_0^{(k+1)}\) | equality of regions (\(2M\ell_k=2M\) step-\(k\) units) |
| Lemma 5.1, Step 5: reconstructions of the near configuration on \(X\subset\tilde\square^2\) | the reconstruction of a minimiser is itself | Step A of Theorem 4.1, on **all** of \(X\) (\(\nu_X\le\nu_{\square_0}\)); every region is covered |
| Lemma 5.2 / (S5): A-ball perturbation keeps (iv) | the response of reconstructions to a data change of size \(\alpha_2\) is \(\le B_3\alpha_2\) on the top-level region | region-independent; (S5) reading unchanged |
| Lemma L2 / CMP116 p.15: potentials on polymer spaces | (S-Res-1) | §6.2 |
| Births \(E^{(k+1)}(X)\) analytic on native spaces | — | (iv\(_t\))-spaces are subsets of the source's, so analyticity there is weaker and follows |
| Actual configurations lie in the spaces | global minimisers reconstruct to themselves | Step A with \(Z'=\) torus |

Status conditional. There is no identified use of clause (iv) that needs the *larger* literal space.
