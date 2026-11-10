# Native-domain restriction and the age sum

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 2. Setting

### 2.1 Scales, radii, ages

Step \(k\) integrates the fluctuation field on the unit lattice \(T^{(k)}_1\); \(\eta=L^{-k}\). An old scale is \(j\le k\), \(\xi=L^{-j}\), and its **age** is \(m=k-j\ge0\). The scale ratio is \(\lambda_m:=L^j\eta=L^{-m}\); the ratio from scale \(k+1\) is \(L^{j-1}\eta=L^{-(m+1)}\).

Native radii (CMP119 (2.28), with one exponent \(q>p_0\) as in Annex AD):
\[
\alpha_{u,j}=C_ug_j\ell_j^{\,q}\ (u=0,1),\qquad \alpha_{2,j}=c_2\alpha_{0,j},\qquad\alpha_{3,j}=c_3\alpha_{0,j},\qquad \ell_j=\log g_j^{-2}.
\]
Cutoff: \(P_k=A_1\ell_k^{p_0}\), \(\delta_k=g_kP_k\) (CMP119 (3.3), (3.16) after the scaling \(A_k'=g_kA_k\)).

**Output radii.** The birth at \(k+1\) is constructed before \(g_{k+1}\) is known. Fix \(\theta:=1+\beta_0\) and put
\[
a_u:=\theta\,\alpha_{u,k}\qquad(u=0,1).
\tag{2.1}
\]
The potentials of step \(k\) live on the scale-\((k+1)\) spaces with radii \((1+\beta)a_u\); the births come out on the spaces with radii \(a_u\) (§2.4). Since \(g\mapsto g(\log g^{-2})^q\) is increasing for small \(g\), \(\alpha_{u,k+1}\le a_u\) as soon as \(g_{k+1}\le(1+\beta_0)g_k\). The crude readout bound (Proposition 3.4) gives \(g_{k+1}/g_k=1+O(\ell_k^{-2q})\), so this holds below a ceiling and the output space contains the native space at \(k+1\) (the spaces are monotone in the radii, §2.2). No estimate on \(c_{k+1}\) is presupposed. (The analysis used the actual \(\alpha_{u,k+1}\) and the factor \(\sqrt{a+2}\); (2.1) is slightly sharper and makes age zero transparent.)

**Lemma 2.1 (radius comparison).** *Assume CMP119 (2.6)–(2.7) on the prefix through \(k\). For \(j=k-m\le k\) put*
\[
\Gamma'_m:=\begin{cases}1,&m=0\\(1+\beta_0)^2\sqrt m,&m\ge1\end{cases}\qquad\Gamma_m:=\theta\,\Gamma'_m.
\]
*Then (a) \(\alpha_{u,k}/\alpha_{u,j}\le\Gamma'_m\) and \(a_u/\alpha_{u,j}\le\Gamma_m\); (b) \(\delta_k/\alpha_{2,j}\le\Gamma'_m\,\delta_k/\alpha_{2,k}\); source input for \(L\ge2\) and \(m\ge1\): \(\sqrt m\,L^{-m}\le\tfrac12\), hence \(\Gamma'_mL^{-sm}\le1\) for every \(s\ge1\), \(m\ge0\), provided \((1+\beta_0)^2\le2\).*

*Proof.* For \(m\ge1\), (2.6) gives \(g_k\le(1+\beta_0)m^{1/2}g_j\) and (2.7) with \(p=q\) gives \(\ell_k^q\le(1+\beta_0)\ell_j^q\); multiply. (b) is deduction for \(u=0\). source: \(\sqrt m\le2^{m-1}\) for \(m\ge1\). \(\square\) (Status deduction; check (1) of finite comparison.)

Only *upper* bounds on new radii in terms of old ones are ever used below. No lower bound on any radius relative to a fixed constant occurs (this answers the analysis second doubt as far as the displayed and cited steps go; see §4.1, last column).

### 2.2 The spaces

\(U^c_j(X,\alpha_0,\alpha_1,\gamma_0)\), \(X\in\mathbf D_j\), is the space of CMP109 (1.10)–(1.16), p.262 source: gauge orbits of pairs \((\mathbf U,\mathbf J)\) on the fine lattice in \(X\) with

- (i) \(\mathbf U=U'U\), \(U\) real with \(|\partial U-1|<\alpha_0\xi^2\) and, on every cube of size \(O(1)LM\) in \(X\), a gauge with \(U^u=\exp i\xi A\), \(|A|,|\nabla^\xi A|<O(1)LMB\alpha_0\);
- (ii) \(U'=\exp i\xi A'\), \(|A'|,|\nabla^\xi_UA'|<\alpha_1\);
- (iii) \(|\partial\mathbf U-1|<\alpha_0\xi^2\), \(|\mathbf J|<\gamma_0\);
- (iv) for the sequence \(\{\Omega_n\}_{n\le j}\) built from \(X\), the reconstructed pairs \((U_n(M^\cdot(\mathbf U)),J_n(M^\cdot(\mathbf U)))\), \(n\le j\), satisfy \(|\partial U_n-1|<\alpha_0\xi^2\), \(|J_n|<\alpha_0(L^n\xi)^2\) on \(\tilde X^{-2}\).

\(\gamma_0=\alpha_0\) is omitted from the notation. Write \(\mathcal U_j(X;\alpha_0,\alpha_1)\) for the set of \(\mathbf U\) satisfying (i), (ii), the first half of (iii), and (iv). All clauses are upper bounds, so the spaces are **monotone** in \((\alpha_0,\alpha_1,\gamma_0)\) deduction. For \(Y\in\mathbf D_k\) the source also uses the scale-\((k+1)\) spaces \(U^c_{k+1}(Y,\cdot)\) (CMP116 p.7, (1.34)); Use them as the source does and do not re-define them.

Two facts from CMP109 p.263 (c) are used repeatedly:

- **(1.17).** If \((\mathbf U,\mathbf J)\) satisfies (i)–(iii) with \(\alpha_0'\), then by Proposition 9 of [15] the reconstructions satisfy the bounds of (iv) with \(2B_3\alpha_0'\). So (i)–(iii) with \(\alpha_0'\le\alpha_0/(2B_3)\) imply membership.
- A configuration which is itself a minimiser reconstructs to itself up to a gauge constant on blocks (CMP109 (3.38)); for it, (iv) follows from (iii) "with a bit better constant".

### 2.3 Families

A **family at scale \(j\)** is \(F=(F(X))_{X\in\mathbf D_j}\) with:

- **(H1)** \(F(X)\) is analytic on \(U^c_j(X,\alpha_{0,j},\alpha_{1,j})\) and depends on \((\mathbf U,\mathbf J)\) in \(X\) only;
- **(H2)** \(\lVert F\rVert_j:=\sup_X\sup|F(X)|e^{\kappa d_j(X)}<\infty\);
- **(H3)** \(F(X)\) is invariant under the \(G^c\)-valued gauge transformations (CMP109 (1.10), (1.19));
- **(H4)** \(F(X)\) does not depend on the torus for \(X\) not wrapping it, and for real regular \(U\) the whole-lattice sum \(\sum_XF(X,U,J(U))\) is invariant under the Euclidean transformations of \(T^{(j)}\) (CMP109 p.263, (5.2)).

These are CMP109 (1.7), (1.18), (1.19) and the symmetry paragraph on p.263, for a general family. **No roots are used** (see §8). For such \(F\) the polarisation tensor \(\Pi^F(x-y)=\sum_{X\in\mathbf D_j^0}\partial^2F(X,U_j(\exp iB))/\partial B(x)\partial B(y)|_{B=0}\) and the Wilson coefficient
\[
\mathcal PF:=\sum_x\Pi^F_{\mu\nu}(x)x_\mu x_\nu\quad(\mu\ne\nu)
\]
are defined by CMP109 (4.37), (5.1), (5.42). \(\mathcal P\) is linear. Put \(\mathbb F:=F-F(1)-(\mathcal PF)A\), the vacuum- and Wilson-subtracted family (CMP109 (1.6); the Wilson term localised by the partition of unity of \(\pi_j\), (4.38)–(4.39)).

A family satisfying (H1)–(H3) but not necessarily (H4), with no Wilson subtraction, is called **unsubtracted** (mature R terms: CMP119 (2.30)–(2.32)).

### 2.4 The potential domain

For \(Y\in\mathbf D_k\) put
\[
\mathfrak D_k(Y):=U^c_{k+1}\big(Y,(1+\beta)a_0,(1+\beta)a_1,a_0\big)\times\{B:\ |B(b)|<2P_k,\ b\subset Y\},
\tag{2.2}
\]
with complex \(B\). This is CMP116 (1.34) and CMP119 (3.43) with the radii (2.1) and \(\varepsilon_1g_k^{-1}\to2P_k\). The space \(\mathcal V_k\) of the companion note is the space of families \(v=(v_Y)\) analytic on \(\mathfrak D_k(Y)\) with \(\lVert v\rVert:=\sup_Y\sup_{\mathfrak D_k(Y)}|v_Y|e^{\kappa_*d_k(Y)}<\infty\), \(\kappa_*=(1-2\delta)\kappa\). On \(\mathfrak D_k(Y)\) put
\[
\varrho:=\frac{g_k\sup_{b\subset Y}|B(b)|}{\alpha_{2,k}}\ \le\ \rho_k:=\frac{2A_1}{c_2C_0}\,\ell_k^{-(q-p_0)}.
\]

The fluctuation difference of a function \(\mathsf F\) of the background is \(\Delta_k\mathsf F:=\mathsf F(U_k(\exp iB'\,V^{(k)}))-\mathsf F(U_{k+1})\), \(B'=g_kCB-h\tilde D(g_kCB)\) (CMP109 (2.12), (3.2)).

## 3. Statements

**Conditions on constants.** \(K_H:=4B_0C_Be^{16\kappa_1}\) is the constant of CMP116 (1.21) (\(C_B\) is the constant printed as \(C_1\) in (1.20)). \(c_\sharp\), \(c_Q\), \(c_{\rm av}\) denote the absolute constants printed as \(O(1)\) in CMP109 (3.26)–(3.27)/(3.37), in (3.49), and in the bound \(|B|<O(1)L^j\eta\) after (3.34). \(\vartheta\in(0,1)\) is the Hölder index of (3.31) (printed \(\beta\) there; not the \(\beta\) of the enlargement).

- **(K1)** \(C_1/C_0>\max\{2B_3^2c_\sharp M(1+2\beta)\theta/L,\ 8B_3c_3\}\).
- **(K2)** \(c_3\le1/(32B_3)\).
- **(K3)** \(c_2\le\min\{c_3/c_Q,\ c_2^{\rm ball}\}\), \(c_2^{\rm ball}\) from (S5).
- **(K4)** \(L\ge2\), \((1+\beta_0)^2\le2\), \((1+7\beta)\theta L^{-2}\le\tfrac34\). (With \(\beta=\tfrac14\), \(\beta_0\le0.05\), every \(L\ge2\) qualifies.)
- **(K5)** coupling ceilings: \(c_\sharp M(1+2\beta)a_1+2B_3^2c_\sharp M(1+2\beta)a_0\le\log\frac{1+3\beta}{1+2\beta}\); \((4B_3^2c_\sharp M(1+2\beta))^2a_0\le\beta\); \(B_3(B_3c_\sharp M(1+2\beta))^2a_0\le\beta\); \(16\,(B_3^2c_\sharp M(1+2\beta)\theta+4B_3c_3)^2\alpha_{0,j}\le\beta L^{-2}\) for \(j\le k\) (by the second line of (2.6) these follow from a ceiling on \(g_k\)); and the absolute smallness conditions of CMP116 (1.13)–(1.20) on \(\delta_k\).
- **(K6)** \(\ell_k^{\,q-p_0}\ge8K_HA_1/(c_2C_0)\), i.e. \(K_Hg_k|B|\le\tfrac14\alpha_{2,k}\) on \(|B|\le2P_k\) (CMP116 p.7).
- **(K7)** far carriers: \((1+\beta)\theta L^{-1}\le\tfrac12\) (clauses (i)–(iii); \(L\ge3\) for \(\beta=\tfrac14\)) and \(K_\flat(1+\beta)\theta L^{-2}\le\tfrac12\) (clause (iv), with the constant \(K_\flat\) of hypothesis (X-far)).

All are ratio conditions, mild lower bounds on \(L\), or ceilings. None depends on the age.

> **Theorem 3.1 (L1\(^*\): E potentials on the source domain).** Assume the cited inputs (S1)–(S9) of §4.1, hypotheses (S-Res) and (X-far) of §4.2, CMP119 (2.6)–(2.7) on the prefix through \(k\), and (K1)–(K7). Let \(F_j\) be a family at scale \(j=k-m\le k\) satisfying (H1)–(H4). Then there are functions \(V_{k,j}[F_j](Y)\), \(Y\in\mathbf D_k\), such that:
> 1. **Representation.** \(\sum_YV_{k,j}[F_j](Y;U_{k+1},J_{k+1},B)=\Delta_k\mathbb F_j\) for real \(B\) in the support of the cutoff and actual backgrounds.
> 2. **Domain.** \(V_{k,j}[F_j](Y)\) is analytic on \(\mathfrak D_k(Y)\), depends on \((\mathbf U,\mathbf J,B)\) in \(Y\) only, and is invariant under the simultaneous gauge transformations CMP109 (3.29).
> 3. **Linearity.** \(F_j\mapsto V_{k,j}[F_j]\) is linear.
> 4. **Bound.** On \(\mathfrak D_k(Y)\),
> \[
> |V_{k,j}[F_j](Y)|\le\varrho\,\Big[C_E\,\Gamma_m^{5}L^{-\vartheta m}+C_F\,\Gamma_m\,L^{3m}e^{-c_FL^{m}}\Big]\lVert F_j\rVert_j\,e^{-\kappa_*d_k(Y)}.
> \tag{3.1}
> \]
> In particular \(V_{k,j}[F_j](Y)\) vanishes at \(B=0\).
> The constants \(C_E,C_F,c_F\) depend on \(L,M,\kappa,\kappa_1,\delta,\beta,\beta_0,\vartheta\), the source constants \(B_0,B_3,C_B,c_\sharp,c_Q,c_{\rm av}\), the ratios \(c_2,c_3,C_1/C_0\), and nothing else: not on \(k\), \(j\), the couplings, the torus, or the family.

> **Corollary 3.2 (age sum).** For a tuple \((F_j)_{j\le k}\) put \(\mathcal V^E_k(F):=\sum_{j\le k}V_{k,j}[F_j]\). Then \(\mathcal V^E_k\) is linear, \(\sum_Y\mathcal V^E_k(F)(Y)=\Delta_k\sum_j\mathbb F_j\), and
> \[
> \lVert\mathcal V^E_k(F)\rVert\le C_V\,\rho_k\,\sup_{j\le k}\lVert F_j\rVert_j,\qquad C_V:=C_E\sum_{m\ge0}\Gamma_m^5L^{-\vartheta m}+C_F\sum_{m\ge0}\Gamma_mL^{3m}e^{-c_FL^m}<\infty.
> \tag{3.2}
> \]
> \(C_V\) is independent of the depth \(k\).

> **Theorem 3.3 (R\(^*\): unsubtracted families).** Under the same assumptions with (S10) in place of (S8)–(S9), let \(G_j\) be an unsubtracted family at scale \(j\) ((H1)–(H3)). Then \(\Delta_k[G_j-G_j(1)]=\sum_YV_{k,j}^{\rm u}[G_j](Y)\) with items 2–3 of Theorem 3.1 and
> \[
> |V^{\rm u}_{k,j}[G_j](Y)|\le\varrho\,\Big[C_M\,\Gamma_m^{5}+C_F\,\Gamma_m\,L^{3m}e^{-c_FL^{m}}\Big]\lVert G_j\rVert_j\,e^{-\kappa_*d_k(Y)}.
> \tag{3.3}
> \]
> If moreover \(\lVert G_j\rVert_j\le g_j^{\kappa_0}\) with \(\kappa_0\ge9\) and the prefix has the lower slope \(Y_j\ge\tfrac12Y_k+\tfrac34d_B(k-j)\) (Lemma 3.4(b),(c) of the native-domain comparison), then for every set \(\mathcal J\subset\{1,\dots,k\}\) (e.g. the mature indices \(j\le k_1\))
> \[
> \Big\lVert\sum_{j\in\mathcal J}V^{\rm u}_{k,j}[G_j]\Big\rVert\le C_R\,\rho_k\,g_k^{\kappa_0-7}\le C_R\,g_k^{\kappa_0-7}.
> \tag{3.4}
> \]

> **Proposition 3.4 (P: readout).** For a family \(F\) at scale \(k+1\) on the output chart (radii \(a_u\)) with (H1)–(H4): \(|\mathcal PF|\le C_P\,(c_2a_0)^{-2}\lVert F\rVert_{k+1}\), \(C_P=C(B_3,M,\kappa)\). On the output chart \((c_2a_0)^{-2}=(c_2\theta C_0)^{-2}Y_k\ell_k^{-2q}\).

Theorem 3.1 with Corollary 3.2 is hypothesis (L1\(^*\)) of the analysis §9.2 in unrooted form. Theorem 3.3 is (R\(^*\)) with a better exponent than was asked (\(\kappa_0-7\) instead of \(\kappa_0-11\)). Lemma 5.1 and Lemma 5.2 are (D\(^*\)).

## 4. Inputs

### 4.1 Cited single-scale estimates

Each row is a statement of the source about objects that do not involve the births, used at **one** scale with the radii of that scale, or a scale-covariant statement whose scale factors are displayed. "Checked" means the display was read in the source and its use below matches it; none was re-derived.

| | Statement (as used) | Source | Dependence on radii |
|---|---|---|---|
| (S1) | Generalised axial gauge on a cube of size \(O(M)\): \(M^\cdot(\mathbf U)=V^v\), \(|V(b)-1|<c_\sharp M\alpha_0\), \(|v-1|<c_\sharp M\alpha_1\) for \(\mathbf U\) with radii \((\alpha_0,\alpha_1)\) | CMP109 (3.26); [12] (77), [15] §F | linear; needs \(M\alpha_0,M\alpha_1\) small |
| (S2) | Landau-gauge minimiser on \(\square_0\): \(U_{k+1}(\square_0,V)=(\exp iL^{-1}\eta\mathbf H_{k+1})^{u}\), \(|\mathbf H_{k+1}|,|\nabla\mathbf H_{k+1}|,\lVert\mathbf H_{k+1}\rVert_{1,\vartheta}<B_3c_\sharp M\alpha_0\), \(|u-1|<B_3c_\sharp M\alpha_0\); the same at scale \(j\) with the factor \(L^{j-1}\eta\): (3.37) | CMP109 (3.27), (3.37); [15] §G | linear |
| (S3) | \(\mathbf H_j(\square_0,B)=H_{1,j}B+\) terms of order \(\ge2\), with \(|\partial^\xi\mathbf H_j-\partial^\xi H_{1,j}B|<B_3|B|_{(1)}^2\); \(|\delta\mathbf H_j/\delta B|\) bounded by \(B_3\) with decay \(\delta_0\) in all the norms of (3.14), including second-order operators | CMP109 (3.9), (3.45), (3.50); [15] (174), Prop. 9, (190) | none (operator bounds) |
| (S4) | Averaging identities: (97) of [12]; (3.38)–(3.39) (a minimiser of a minimiser); \(|Q'|\le c_QL^j\eta|\mathbf A|\) for \(Q'\) of (3.48); \(|Q_j(\eta A)|\le c_{\rm av}L^j\eta|A|\) and the derivative bounds (4.17)–(4.18) | CMP109 (3.38), (3.39), (3.48)–(3.49), (4.16)–(4.18); [7] Prop. 5 | none |
| (S5) | **A-ball at one scale.** There is \(c_2^{\rm ball}>0\) such that for \(\mathbf U\in\mathcal U_j(X;\tfrac12\alpha_0,\tfrac12\alpha_1)\), \(|\mathbf J^\circ|\le\tfrac12\alpha_0\) and \(\max\{|\mathbf A|,|P_1\mathbf A|,|\nabla^\xi\mathbf A|,|\Delta^\xi\mathbf A|\}<c_2^{\rm ball}\alpha_0\) on \(X\): \((\exp i\xi\mathbf A\,\mathbf U,\ \mathbf J^\circ+\Delta_{\mathbf U}\mathbf A-P_1\mathbf A+\mathbf F_1(\mathbf U,\mathbf A))\in U^c_j(X,\alpha_0,\alpha_1)\). Also with \(\mathbf U=1,\mathbf J^\circ=0\): (4.4) | CMP109 (3.10)–(3.14), (4.4): "there exists a constant \(\alpha_2\), depending on \(\alpha_0\) and on some absolute constants" | homogeneous (see remark) |
| (S6) | Derivatives of \(F(X,U_j(\square_0,\exp iB))\) at \(B=0\): the chain rule (4.3); each of \(r\) derivatives of \(F(X,\exp i\xi\mathbf A)\) costs \(rB_3/\alpha_{2}\) by Cauchy on (4.4); tree decay \(\exp(-O(1)\kappa d_j(X\cup\{x_i\}))\) | CMP109 (4.2)–(4.5), (4.22) | \(\alpha_{2,j}^{-r}\) only |
| (S7) | The propagators \(H,H_0,\tilde G\) at scale \(k\), their random-walk expansions with decoupling parameters \(|s(\Delta)|\le e^{\kappa_1}\), and \(|\mathbf H_k(s,B')|\le K_Hg_k|B|\) in all admissible norms, analytic in \((\mathbf U,\mathbf J)\) on (i)–(iii) with fixed \(\alpha_0',\alpha_1'\) "much bigger than \(\alpha_0,\alpha_1\)" | CMP116 (1.2)–(1.21) | ceilings only |
| (S8) | Ward identities (4.9)–(4.15) and their use (4.21)–(4.34): linear identities among the coefficients \(F^{(n)}(X)\), \(n\le4\), valid for each gauge-invariant \(F(X)\) separately; the discarded ("irrelevant") terms have spatial gain \((L^j\eta)^{4+\vartheta}\) or \((L^j\eta)^5\) | CMP109 §4 | via (S6) |
| (S9) | Polarisation tensor: for a family with (H4), \(\Pi^F(p)=\beta(\delta_{\mu\nu}\Delta(p)-\overline{\partial_\mu}\partial_\nu)+\Pi'^F(p)\), \(\beta=\mathcal PF\), \(|\Pi'^F_{\ldots}(x-y)|\le O(1)\sup|\Pi^F|e^{-\frac12\delta_1|x-y|}\); the same structure for \(A\) itself, (4.40)–(4.45); extension of the \(X\)-sum to \(\mathbf D_j^0\), (4.36) | CMP109 (4.35)–(4.45), §5, (5.37)–(5.44) | via (S6) |
| (S10) | For each gauge-invariant \(G(X)\) separately and any anchor \(z\in X\): \(\sum_{n\le4}\frac1{n!}\langle G^{(n)}(X),\otimes^nB\rangle=\big[\sum_{x,y}G^{(2)}_{\mu\nu}(X,x,y)(x-z)_\kappa(y-z)_\lambda\big]\tfrac12{\rm tr}(\partial_\kappa B_\mu+\tfrac12i[B_\kappa,B_\mu])(z)(\partial_\lambda B_\nu+\tfrac12i[B_\lambda,B_\nu])(z)+\) irrelevant terms; all terms are \(O((L^j\eta)^4)\) | CMP119 (3.49), p.283 ("\(\mathbf E^{(2)}(X,x,y,z)\) is replaced by \(\mathbf R^{(2)}(X,x,y)\), and \(z\) is an arbitrary point from \(X\)") | via (S6) |

*Remark on (S5).* The source does not display \(\alpha_2\) as a multiple of \(\alpha_0\). The map \(\mathbf A\mapsto(\exp i\xi\mathbf A\,\mathbf U,\ldots)\) changes the plaquette by \(O(|\nabla\mathbf A|+|\mathbf A|^2)\), the relative field by \(O(|\mathbf A|+|\nabla\mathbf A|)\), the current by \(O(|\Delta\mathbf A|+|P_1\mathbf A|+\ldots)\), and the reconstructions by \(B_3\) times these ((1.17)). So a radius \(c_2^{\rm ball}\alpha_0\) with \(c_2^{\rm ball}\asymp1/B_3\) is the natural form, and it is what Annex AD (E14.32) derives. Treat it as the reading (d) of a (c) statement. Also, the source states (3.13) with current argument \((L^{j-1}\eta)^3\mathbf J\), \(|\mathbf J|<\alpha_0\); Equivalently, write it with a free current \(|\mathbf J^\circ|\le\tfrac12\alpha_0\), which contains the source's case because \(L^{-3}\le\tfrac12\).

*Remark on quantifiers.* Bałaban fixes \(\alpha_0,\alpha_1\) once, as \(M\)-dependent numbers at the top of their admissible range (this is why CMP116 (1.29) writes \(\alpha_2^{-1}(\alpha_1/\alpha_3)^5\) as \(O(M^q)\)). The running chart uses (S1)–(S6) for **every** small pair with fixed ratios. In the displayed proofs the radii enter only through upper bounds (\(M\alpha_1\le\beta/O(1)\), \((4B_3^2O(1)M)^2\alpha_0\le\beta\), …) and ratios (\(B_3^2O(1)M\alpha_0<\tfrac12\alpha_1\), \(2B_3\alpha_3\le\beta L^{-2}\alpha_0\), \(4B_0C_Be^{16\kappa_1}\varepsilon_1\le\tfrac14\alpha_2\)). There is no identified lower bound on a radius against a fixed number in CMP109 §§1–5 or CMP116 §§1–2. The cited papers [12]–[15] were not searched for one.

### 4.2 Two hypotheses about the spaces

> **(S-Res) Same-scale restriction.** For \(Y\subset X\) (domains at scale \(k+1\) in the sense used by the source) and radii below the ceiling:
> \[
> U^c_{k+1}(X,\alpha_0,\alpha_1)\big|_Y\subset U^c_{k+1}\big(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0\big),\qquad
> U^c_{k+1}\big(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0\big)\big|_{\square_0}\subset U^c_{k+1}\big(\square_0,(1+2\beta)\alpha_0,(1+2\beta)\alpha_1,\alpha_0\big).
> \]

Source: CMP116 p.15 ("The potentials are also analytic functions on the subspace \(\mathbf U^c_{k+1}(X,\alpha_0,\alpha_1)\)") and p.7 ("we take its subspace \(\mathbf U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\)"). Both are asserted, not proved source input. The first is the inclusion used by Lemma L2 to deliver births on the native space; the second feeds Lemma 5.1. It is a single-scale statement and transfers to the running chart verbatim.

> **(X-far) Far-carrier inclusion, clause (iv), scaling form.** There is \(K_\flat\ge1\), independent of scales, domains and radii, such that for \(j\le k\), \(X\in\mathbf D_j\), \(X\subset Y\in\mathbf D_k\), and radii below the ceiling: if \(\mathbf U\in\mathcal U_{k+1}(Y;a_0',a_1')\), then \(\mathbf U|_X\) satisfies clause (iv) of the scale-\(j\) space on \(X\) with the constant \(K_\flat L^{-2(k+1-j)}a_0'\).

Source: CMP109 (3.16) and CMP116 p.9 ("All these spaces contain the subspace \(\mathbf U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\)"), which is the case of equal radii with conclusion \(\mathcal U_j(X;\tfrac12\alpha_0,\tfrac12\alpha_1)\). Asserted, not proved.

Assumptions for (X-far):

- *Clauses (i), (ii), (iii).* By change of units: a plaquette bound \(a_0'L^{-2(k+1)}\) is \(a_0'L^{-2(k+1-j)}\xi^2\); a regular-gauge field scales with \(L^{-(k+1-j)}\) and its first difference with \(L^{-2(k+1-j)}\). So \(\mathbf U|_X\) satisfies clauses (i), (ii) and the first half of (iii) at scale \(j\) with the radii \(L^{-2(k+1-j)}a_0'\), \(L^{-(k+1-j)}a_1'\) and no constant deduction, up to the source's convention for the cubes of size \(O(1)LM\) in a domain of a different class, which Take from the source.
- *Clause (iv).* This is **not** a change of units: the reconstructions \(U_n(X;M^\cdot(\mathbf U))\), \(n\le j\), are built from the domain sequence of \(X\), those of clause (iv) at scale \(k+1\) from the sequence of \(Y\). Two routes:
  - **By (1.17): excluded for young ages.** Clause (iv) at scale \(j\) follows from clauses (i)–(iii) with \(K_\flat=2B_3\); then the second half of (K7) reads \(L^2\ge4(1+\beta)\theta B_3\). But \(B_3\) is displayed in CMP102 (162), p.303 (source input):
  \[
  B_3=72d^3L^3B_0\ \sup_{\mathfrak B_k}\sup_{y_1}\sum_{y_2\in\mathfrak B_k}e^{-\frac12\delta_0d(y_1,y_2)}\,(d(y_1,y_2)+1)\,(L^{j_2}\eta)^{-1}.
  \]
  The sum dominates the sum in the propagator bound (161) with the same \(B_0\), and that bound must reproduce constant fields, so \(B_0\cdot(\text{sum})\ge1\) (reading additional assumption). Hence \(B_3\ge72d^3L^3=4608L^3\) for \(d=4\), and \(L^2\ge4(1+\beta)\theta B_3\) fails for **every** \(L\). So the far-carrier inclusion of CMP116 p.9 cannot be obtained from (1.17) at age zero, at fixed or running radii. For ages \(m\ge m_\flat:=\min\{m:\ L^{2(m+1)}\ge4B_3(1+\beta)\Gamma_m\}\) the route works with no further input; with \(B_3=4608L^3\), \(m_\flat=6,4,3\) for \(L=3,5,13\) (check (3c) of finite comparison).
  - **By locality of minimisers.** (S-Res), with loss \(1+\beta<2\le2B_3\), cannot come from (1.17) either, so the source must intend a locality argument. It uses exactly such an argument, with displayed estimates, in CMP119 (3.6)–(3.8) and (3.17)–(3.19) (pp.266, 268; source): a minimiser on a sub-cube is written as \(\exp i\eta\mathbf H(\cdot)\) of another minimiser, the argument of \(\mathbf H\) is supported in a boundary layer, and the decay (190) of [15] gives a factor \(\exp(-\delta_0\cdot\text{distance})\) in the interior.

> **Proposition 4.1 (outline of (X-far) and (S-Res) by locality; an additional hypothesis).** Let \(X\subset Y\) be as in (X-far) or (S-Res), \(\mathbf U\in\mathcal U_{k+1}(Y;a_0',a_1')\), \(n\le j\), and \(W_n:=U_n(Y;M^\cdot(\mathbf U))\). Then on \(\tilde X^{-2}\) the reconstruction \(U_n(X;M^\cdot(\mathbf U))\) obeys the bounds of \(W_n\) up to a factor \(1+CB_3^2e^{-\frac12\delta_0M}\). In particular \(K_\flat=1+\beta\) for \(M\ge M_0(L,\beta)\).

*Outline.* (1) \(W_n\) is critical for the action under the constraints of \(Y\)'s sequence at level \(n\). The constraints of \(X\)'s sequence are finer (lower-level averages in the collar \(X\setminus\Omega_n(X)\), the same level-\(n\) averages on \(\Omega_n(X)\subset\Omega_n(Y)\)), and \(W_n\), being regular at scale \(j\) by clause (iv) on \(Y\), lies in the regular space of \(X\)'s sequence. A configuration critical under coarser constraints is critical under finer ones; by uniqueness of the critical orbit (CMP102 Theorem 1), \(W_n|_X=U_n(X;M^\cdot_X(W_n))\) up to gauge. (2) By CMP102 Proposition 9 for the determining set of \(X\), \(U_n(X;M^\cdot_X(\mathbf U))\) is \(\exp i\xi\mathcal H(D)\) times \(W_n\) in the Landau gauge, with \(D=\frac1i\log[M^\cdot_X(\mathbf U)M^\cdot_X(W_n)^{-1}]\). (3) \(D=0\) on \(\Omega_n(X)\), because the level-\(n\) averages of \(\mathbf U\) and \(W_n\) agree on \(\Omega_n(Y)\). On the collar \(|D|\le Ca_0'(L^n\xi)^2\) (two regular configurations with equal level-\(n\) averages; the analogue of (1.65) of [14] used in CMP119 (3.7)). (4) The collar has width \(O(R_1M_1)\ll M\) in the units of its own layers. By (190), \(\mathcal H(D)\) and its derivatives on \(\tilde X^{-2}\) carry \(e^{-\delta_0R_1M_1}\) per intermediate layer, which beats the unit factors \(L^2\) per layer by CMP102 (163), and \(e^{-\frac12\delta_0M}\) across the two \(M\)-layers. \(\square\)

With (X-far), the running version needs \((1+\beta)\Gamma_mL^{-(m+1)}\le\tfrac12\) and \(K_\flat(1+\beta)\Gamma_mL^{-2(m+1)}\le\tfrac12\) for all \(m\). By Lemma 2.1(c) this is (K7), i.e. the age-zero conditions with the single extra factor \(\theta=1+\beta_0\). So the unproved content of (X-far) concerns the finitely many young ages \(m<m_\flat\), and it is the same content as in the source's fixed-radius Lemma 1.

*Clause (iv) cannot be dropped.* One might try to run the induction on the simpler spaces defined by (i)–(iii) alone. Then Step 0 of Lemma 5.1 is available only through (1.17), with the factor \(2B_3\), and the plaquette clause at age zero would need \(2B_3(1+7\beta)\theta L^{-2}\le1\), which is false; the admissible radius would shrink by \(2B_3L^{-2}\) per step. Clause (iv) is the device that makes the spaces self-similar (the leading term in Lemma 5.1 has coefficient \(1+O(\beta)\) and no \(B_3\)); the price is that restriction to a sub-domain is no longer trivial. This is the precise form of the tension the analysis describes in its §5.2 and §5.5.

## 5. The domain lemmas (D\(^*\))

### 5.1 Lemma N: CMP109 Lemma 4 with running radii

> **Lemma 5.1.** Assume (S1)–(S4), Lemma 2.1 and (K1)–(K5). Let \(j=k-m\le k\), \(\square_0=\tilde\square^5\), and
> \[
> (\mathbf U,\mathbf J)\in U^c_{k+1}\big(\square_0,(1+2\beta)a_0,(1+2\beta)a_1,a_0\big);\quad |\mathbf A|,|\nabla^\eta\mathbf A|,\lVert\mathbf A\rVert_{1,\vartheta}<\alpha_{2,k}\ \text{on }\square_0;\quad |B'|<\alpha_{3,j};\quad\tau\in[0,1].
> \]
> Let \(B=Q(\eta A)\) with \(A\) as in CMP109 (3.30). Then for every \(X\in\mathbf D_j\), \(X\subset\tilde\square^2\),
> \[
> \big(U_j(\square_0,\exp i(\tau B+B')),\ J_j(\square_0,\exp i(\tau B+B'))\big)\big|_X\in U^c_j(X,\alpha_{0,j},\alpha_{1,j}),
> \]
> and the pair is analytic in \((\mathbf U,\mathbf J,\mathbf A,B')\). Moreover \(|B|\le c_{\rm av}\lambda_m\mathfrak b_k\), \(\mathfrak b_k:=2(\alpha_{2,k}+B_3c_\sharp M(1+2\beta)a_0)=K_{\mathfrak b}\alpha_{2,k}\), \(K_{\mathfrak b}=2(1+B_3c_\sharp M(1+2\beta)\theta/c_2)\).

*Proof.* I follow CMP109 pp.277–280 and write each inequality with the two sets of radii. \(\lambda:=L^{j-1}\eta=L^{-(m+1)}\).

*Step 0 (what the hypothesis gives).* Clause (iv) at level \(n=k+1\) of the input space gives (3.40):
\[
|\partial U_{k+1}(\square_0,M^\cdot(\mathbf U))-1|<(1+2\beta)a_0(L^{-1}\eta)^2,\qquad|J_{k+1}(\square_0,M^\cdot(\mathbf U))|<(1+2\beta)a_0\quad\text{on }\tilde\square^3.
\]
This is the step that makes the lemma free of any factor \(B_3\) in the leading term. By (S1), (S2): the gauges \(v,u_{k+1}\) and the field \(\mathbf H_{k+1}\) of (3.26)–(3.27) have sizes \(c_\sharp M(1+2\beta)a_1\), \(B_3c_\sharp M(1+2\beta)a_0\).

*Step 1 (\(\mathbf A=0\), \(B'=0\); clauses (i), (ii)).* By (S2) at scale \(j\), (3.37): \(U_j(\square_0,\exp i\tau Q(L^{-1}\eta\mathbf H_{k+1}))=(\exp i\xi\mathbf H_j)^{u_j}\) with
\[
|\mathbf H_j|,|\nabla^\xi\mathbf H_j|<B_3^2c_\sharp M(1+2\beta)a_0\lambda\le B_3^2c_\sharp M(1+2\beta)\,\Gamma_mL^{-(m+1)}\alpha_{0,j}<\tfrac12\alpha_{1,j}
\]
by Lemma 2.1 and (K1) (\(\Gamma_mL^{-(m+1)}\le\theta/L\)). The orbit contains \(\exp i\xi\mathbf H_j\); take \(U=1\), \(U'=\exp i\xi\mathbf H_j\). Clauses (i), (ii) hold on \(\tilde\square^3\supset X\).

*Step 2 (plaquette clause).* By the identity (3.39) (S4) and Step 0, (3.41):
\[
|\partial\exp i\xi\mathbf H_j-1|<e^{B_3^2c_\sharp Ma_0}e^{B_3c_\sharp Ma_0}e^{c_\sharp M(1+2\beta)a_1}(1+2\beta)a_0\lambda^2\xi^2<(1+3\beta)a_0\lambda^2\xi^2
\]
by the first ceiling of (K5). The source then passes to all \(\tau\in[0,1]\) through the linear part \(H_{1,j}Q\): the quadratic remainder (3.43) and the nonlinear part (3.45) of \(\mathbf H_j\) (S3) are each used once in each direction, and each is \(\le\beta a_0\lambda^2\) by the second and third ceilings of (K5). Result, (3.47):
\[
|\partial\exp i\xi\mathbf H_j(\square_0,\tau Q(L^{-1}\eta\mathbf H_{k+1}))-1|<(1+7\beta)a_0\lambda^2\xi^2\le(1+7\beta)\Gamma_mL^{-2(m+1)}\alpha_{0,j}\xi^2\le\tfrac34\alpha_{0,j}\xi^2,
\]
by Lemma 2.1(c) and (K4). At fixed radii and \(j=k\) this is the source's "\((1+7\beta)L^{-2}\le1\)".

*Step 3 (current clause).* By (3.39) and Step 0, (3.42): \(|D^*\xi^{-2}\pi{\rm Im}\,\partial\exp i\xi\mathbf H_j|<(1+3\beta)a_0\lambda^3\). The source obtains the bound on the linearised second-order operator "in the same way", from (1.43)–(1.54) of [14] and (S3). The age factor is \(\Gamma_mL^{-3(m+1)}\), better than in Step 2. So \(|J_j|<\tfrac34\alpha_{0,j}\).

*Step 4 (general \(\mathbf A\), \(B'\)).* By (3.48)–(3.49) (S4), \(B=Q(L^{-1}\eta\mathbf H_{k+1})+Q'\) with
\[
|Q'|\le c_QL^j\eta|\mathbf A|<c_Q\lambda_m\alpha_{2,k}\le c_Qc_2\Gamma'_mL^{-m}\alpha_{0,j}\le\alpha_{3,j}
\]
by (K3) and Lemma 2.1(c). So \(\tau B+B'=\tau Q(L^{-1}\eta\mathbf H_{k+1})+B''\) with \(|B''|<2\alpha_{3,j}\). By (3.50) and (S3), \(\mathbf H_j(\ldots+B'')=\mathbf H_j(\ldots)+\mathbf A_2\) with \(|\mathbf A_2|,|\nabla\mathbf A_2|\le B_3|B''|<2B_3\alpha_{3,j}<\tfrac14\alpha_{1,j}\) by (K1); clauses (i), (ii) persist (\(\tfrac12+\tfrac14<1\)). By (3.51) and (K2),
\[
|\partial^\xi\mathbf H_j(\ldots+B'')|<(1+6\beta)a_0\lambda^2+4B_3\alpha_{3,j}\le\big[(1+6\beta)\Gamma_mL^{-2(m+1)}+\tfrac18\big]\alpha_{0,j},
\]
and with the quadratic remainder (now of the field \(\mathbf H_j+\mathbf A_2\); fourth ceiling of (K5)), (3.52): \(|\partial\exp i\xi\mathbf H_j(\ldots+B'')-1|<[(1+7\beta)\theta L^{-2}+\tfrac18]\alpha_{0,j}\xi^2<\alpha_{0,j}\xi^2\) by (K4). The current clause is the same with the second-order bounds of (S3): \(|J_j|<[\tfrac34+\tfrac18]\alpha_{0,j}\).

*Step 5 (clause (iv)).* The configuration is a minimiser on \(\square_0\). By (3.38) (S4) its reconstructions on \(X\) are gauge transforms of itself, by gauges with the bound of \(u_j\). So \(|\partial U_n-1|\) obeys the bound of Step 4, and \(|J_n|=(L^n\xi)^3|J_j|\le(L^n\xi)^2\alpha_{0,j}\) for \(n\le j\).

*Analyticity* is that of the compositions, as in the source. The bound on \(B\) is (3.32) with (S4). \(\square\)

**Hypotheses.** conditional. The chain is complete for the radii and the ages: each inequality of CMP109 pp.277–280 appears above with its running form, including the two that the analysis table does not display in full (Step 3, Step 5). What is cited are the estimates (S1)–(S4) themselves. Check (2) of finite comparison evaluates the closing inequality of Step 4 over \(L\le39\), \(m\le199\).

### 5.2 The far insertion

> **Lemma 5.2.** Assume (S5), (X-far), Lemma 2.1, (K3), (K7). Let \(X\in\mathbf D_j\), \(X\subset Y\in\mathbf D_k\), \((\mathbf U,\mathbf J)\in U^c_{k+1}(Y,(1+\beta)a_0,(1+\beta)a_1,a_0)\), and let \(\mathbf A\) satisfy CMP109 (3.14) on \(X\) with \(\alpha_{2,j}\). Then
> \[
> \big(\exp i\xi\mathbf A\,\mathbf U,\ (L^{j-1}\eta)^3\mathbf J+\Delta^\xi_{\mathbf U}\mathbf A-P_1\mathbf A+\mathbf F_1(\mathbf U,\mathbf A)\big)\big|_X\in U^c_j(X,\alpha_{0,j},\alpha_{1,j}).
> \]

*Proof.* Put \(a_u'=(1+\beta)a_u\). By the change of units (§4.2) and Lemma 2.1, \(\mathbf U|_X\) satisfies clauses (i), (ii), (iii)\(_1\) at scale \(j\) with radii \((1+\beta)\Gamma_mL^{-2(m+1)}\alpha_{0,j}\), \((1+\beta)\Gamma_mL^{-(m+1)}\alpha_{1,j}\), and by (X-far) clause (iv) with \(K_\flat(1+\beta)\Gamma_mL^{-2(m+1)}\alpha_{0,j}\). By (K7), Lemma 2.1(c) and monotonicity, \(\mathbf U|_X\in\mathcal U_j(X;\tfrac12\alpha_{0,j},\tfrac12\alpha_{1,j})\). The current \(\mathbf J^\circ=(L^{j-1}\eta)^3\mathbf J\) satisfies \(|\mathbf J^\circ|<\Gamma_mL^{-3(m+1)}\alpha_{0,j}\le\tfrac12\alpha_{0,j}\). Apply (S5) at scale \(j\). \(\square\)

## 6. Proof of Theorem 3.1

The construction is that of CMP109 §§3–5 and CMP116 §1, applied to \(\mathbb F_j\) in place of \(\mathbf E^{(j)}-\beta_jA\). The list gives the steps, say for each whether it is an identity or an estimate, and give the running form of each estimate.

### 6.1 Identities (linear in the family)

1. First localisation, CMP109 (3.3)–(3.4): with the partition of unity \(\{\zeta_\square\}\) on \(\pi_k\),
\[
\Delta_k F_j=\sum_\square\int_0^1dt\ \frac{d}{dt_\square}F_j\big(U_j(\exp iQ_j(\eta(t+t_\square\zeta_\square)\mathbf H_k(B'))\bar U^j_{k+1})\big)\Big|_{t_\square=0}.
\]
Uses gauge invariance (H3), the fundamental theorem of calculus and (S4). No property of the specific births.
2. Split of \(F_j=\sum_XF_j(X)\) into **near** (\(X\subset\tilde\square^2\)) and **far** (\(X\cap(\tilde\square^2)^c\ne\emptyset\)), (3.5).
3. Near: reconstruction on \(\square_0\), (3.18)–(3.25), and the removal (3.21)–(3.22) of the part of the coarse field outside \(\tilde\square^3\); the removed parts are far-type terms. Then Taylor's formula (3.34) to fourth order with integral remainder.
4. Orders \(n\le4\): the localisation (4.1), the chain rule (4.3), the Ward identities (S8), the resummations (4.35)–(4.37). The same for the family \((\mathcal PF_j)A\) localised by \(\pi_j\), (4.38)–(4.45). The marginal terms of \(F_j\) and of \((\mathcal PF_j)A\) are, by (S9), the same expression with coefficients \(\mathcal PF_j\) and \(-\mathcal PF_j\cdot1\): they cancel identically. This is the only place where (H4) and the definition of \(\mathcal P\) are used. \(F_j(1)\) drops out of \(\Delta_k\).
5. Decoupling: the interpolation (1.9)–(1.10) of CMP116 in the parameters \(s(\Delta)\) and the Cauchy representation (1.23). Uses (S7) only.

Every operation is linear in \(F_j\) (evaluation, differentiation, Cauchy integrals, sums). This gives items 1 and 3 of the theorem. Gauge invariance of the terms is the paragraph of CMP109 containing (3.29) and the last remark of CMP116 §1; it uses (H3).

### 6.2 The fifth-order tail

For the remainder of (3.34), CMP116 (1.23)–(1.24) combine the Cauchy integral in \(t_\square\) over the circle (1.22) with (3.54). In running form:

- *the \(t_\square\) circle.* The field \((t\tilde\zeta_\square+t_\square\zeta_\square)\mathbf H_k(\sigma,B')\) must satisfy (3.31) with \(\alpha_{2,k}\). By (S7) and (K6), \(t\tilde\zeta_\square\mathbf H_k\) satisfies (3.31) with \(\tfrac12\alpha_{2,k}\), and \(t_\square\zeta_\square\mathbf H_k\) does so on the circle fixed by
\[
\frac1{|t_\square|}=2K_H\,\frac{g_k|B|}{\alpha_{2,k}}=2K_H\varrho
\tag{CMP116 (1.22)}
\]
(a scale-\(k\) statement; \(\alpha_2\) there is the radius of (3.31), i.e. \(\alpha_{2,k}\));
- *the fifth derivative.* By Lemma 5.1, for \(|\sigma B|<\alpha_{3,j}\) the pair \((U_j(\square_0,\exp i(\tau B+\sigma B)),J_j(\ldots))|_X\) lies in the domain of \(F_j(X)\). Cauchy in \(\sigma\) and (H2) give, as in (3.54),
\[
\Big|\int_0^1d\tau\frac{(1-\tau)^4}{4!}\Big\langle\frac{\delta^5}{\delta B^5}F_j(X,U_j(\square_0,\exp i\tau B)),\otimes^5B\Big\rangle\Big|\le\lVert F_j\rVert_j\Big(\frac{|B|}{\alpha_{3,j}}\Big)^5e^{-\kappa d_j(X)}\le\lVert F_j\rVert_j\Big(\frac{c_{\rm av}K_{\mathfrak b}c_2}{c_3}\Gamma'_m\lambda_m\Big)^5e^{-\kappa d_j(X)},
\]
using \(|B|\le c_{\rm av}\lambda_mK_{\mathfrak b}\alpha_{2,k}\) and Lemma 2.1.

So the term of CMP116 (1.23) for \((\square_0,Y_0,j,X)\) is bounded by
\[
2K_H\varrho\cdot\lVert F_j\rVert_j\,(K_5\Gamma'_m\lambda_m)^5\,e^{-(\kappa_1-1)M^{-4}|Y_0\setminus\tilde\square^4|}\,e^{-\kappa d_j(X)},\qquad K_5:=c_{\rm av}K_{\mathfrak b}c_2/c_3.
\tag{6.1}
\]
This is (1.24) with \(E_0\to\lVert F_j\rVert_j\), \(\alpha_2^{-1}g_k|B|\to\varrho\), \((\alpha_1/\alpha_3)^5(L^j\eta)^5\to(K_5\Gamma'_m\lambda_m)^5\). The inner localisation in \(\tilde\square^4\) (the remark after (3.54)) is a far-type correction.

### 6.3 The Ward and coupling terms

Here the \(t_\square\)-derivative is taken explicitly, (4.6): one factor \(\delta B\), linear in \(\zeta_\square\mathbf H_k(B')\). (The analysis §5.4 says every term of the E potential is a \(t_\square\)-Cauchy integral; for these terms the factor \(g_k|B|\) comes instead from the linearity in \(\delta B\). The gain is the same.) By (S4), (S7):
\[
|\delta B|\le C_\zeta c_{\rm av}\lambda_m\,\mathfrak d,\quad|\partial\delta B|\le C_\zeta c_{\rm av}\lambda_m^2\,\mathfrak d,\quad[\partial\delta B]_\vartheta\le C_\zeta c_{\rm av}\lambda_m^{2+\vartheta}\,\mathfrak d,\qquad\mathfrak d:=K_Hg_k|B|=K_H\varrho\,\alpha_{2,k},
\]
and the same three bounds for \(B\) with \(\mathfrak b_k=K_{\mathfrak b}\alpha_{2,k}\) in place of \(\mathfrak d\) ((4.17)–(4.18); these are the bounds the source writes as \(\alpha_1(L^j\eta)^2\), \(\alpha_1(L^j\eta)^{2+\beta}\); Retain \(\mathfrak b_k\) instead of bounding it by \(\alpha_1\)).

**construction.** Every term of CMP109 §§4–5 that is kept after the cancellation of §6.1(4) has: a field degree \(n\in\{2,3,4\}\) (one \(\delta B\) and \(n-1\) factors \(B\); a field may be replaced by a difference or a Taylor remainder of the same field, which does not change the degree); a coefficient order \(r\le n\) (the number of derivatives of \(F_j(X,\exp i\xi\mathbf A)\); by (S6) each costs \(O(B_3)/\alpha_{2,j}\)); and a spatial gain \(\lambda_m^{4+\vartheta}\) or better. Its bound is therefore

\[
C\,\lVert F_j\rVert_j\,\alpha_{2,j}^{-r}\,\mathfrak d\,\mathfrak b_k^{\,n-1}\,\lambda_m^{4+\vartheta}\,W
\ \le\ C\,K_H\varrho\,K_{\mathfrak b}^{\,n-1}\,(\Gamma'_m)^{r}\,\lVert F_j\rVert_j\,\lambda_m^{4+\vartheta}\,W ,
\tag{6.2}
\]
where \(W\) is the decay weight of the term, and Use \(\mathfrak d\,\mathfrak b_k^{n-1}=K_H\varrho K_{\mathfrak b}^{n-1}\alpha_{2,k}^{\,n}\), \(\alpha_{2,k}/\alpha_{2,j}\le\Gamma'_m\) and \(\alpha_{2,k}^{\,n-r}\le1\).

| Terms | Source | \(n\) | \(r\) | Gain | Weight \(W\) |
|---|---|---|---|---|---|
| \(m<n\) in (4.1) (a factor localised outside \(\tilde\square^4\)) | (4.5) | 2–4 | \(\le n\) | \(e^{-\delta_0ML^{m}}\) | \(e^{-\kappa d_j(X)}\) |
| field differences \((\partial B)(\Gamma_{x,x_3})\) in the 4th-order term | (4.21)–(4.22) | 4 | \(\le4\) | \(\lambda_m^5\) | \(e^{-\frac13\kappa d_j(X)}\) |
| commutator and second-moment terms from the Ward identities | (4.24)–(4.31) | 3, 4 | 2, 3 | \(\lambda_m^5\) | as (4.22) |
| Taylor remainder (4.30) with the Hölder bound | (4.30), (4.18) | 3 | \(\le3\) | \(\lambda_m^{4+\vartheta}\) | as (4.22) |
| \(\mathbf H_j(\square_0)\to\mathbf H_j\); sums over \(y\) and over \(X\) extended | (4.35)–(4.36) | 2–4 | 2 | \(e^{-cL^m}\) | \(e^{-\delta_1|x-y|}\) |
| third-order part \(\Pi'\) of the polarisation tensor | (5.38), (5.43)–(5.44) | 2 | 2 | \(\lambda_m^{4+\vartheta}\) | \(e^{-\frac12\delta_1|x-y|}\) |
| the same list for \((\mathcal PF_j)A\) | (4.38)–(4.45) | \(\ge2\) | — | same | same |

For the last row the family is \((\mathcal PF_j)A_{\square'}\), \(\square'\in\pi_j\). On \(U^c_j(X,\alpha_{0,j},\alpha_{1,j})\) the localised Wilson action is \(O(M^4\alpha_{0,j}^2)\), and \(|\mathcal PF_j|\le C_P\alpha_{2,j}^{-2}\lVert F_j\rVert_j\) (Proposition 3.4 at scale \(j\)). So this family has native norm \(\le C_PM^4c_2^{-2}\lVert F_j\rVert_j\): it is a family of the same kind, and (6.2) applies to it with a fixed constant. This is the "matching Wilson subtraction" row of AD §5.4; it must be paired with \(F_j\) **before** bounding, as §6.1(4) does.

*What is checked and what is not.* The interpretation of CMP109 pp.281–298 against this table: the degrees, the positions of the Cauchy denominators ((4.3), (4.5), (4.22)) and the spatial gains are is stated, and no step multiplies two coefficients or uses a radius other than through (S6) and the field bounds. The argument assumes the algebra (4.24)–(4.34) or §5; they are identities and bounds of the source, linear in the family. Status of (6.2): conditional from (S6), (S8), (S9). The same construction, on the reduced contour, is AD (E14.36)–(E14.38).

### 6.4 The far terms

For far \(X\) the source uses the analytic extension (3.13)–(3.15): \(F_j(X,\exp i\xi\mathbf A\,\mathbf U,\ldots)\) with \(\mathbf A=\mathbf H_j(B(t))+t_\square\delta\mathbf H_j\), and the Cauchy integral in \(t_\square\) with radius \(r\), \(r\max\{|\delta\mathbf H_j|_X,\ldots\}=\tfrac13\alpha_{2,j}\). Running form:

- *domain.* Lemma 5.2. The field \(\mathbf H_j(B(t))\) must satisfy (3.14) with \(\tfrac13\alpha_{2,j}\): by (S3), (S4), (S7) its norms are \(\le B_3c_{\rm av}\lambda_mK_Hg_k|B|\le B_3c_{\rm av}\Gamma'_m\lambda_m\cdot\tfrac14\alpha_{2,j}\) by (K6) and Lemma 2.1; so the condition holds if \(B_3c_{\rm av}\le\tfrac43\), or else after lowering the ceiling in (K6) by the fixed factor \(B_3c_{\rm av}\);
- *bound.* By (3.9) (S3), \(|\delta\mathbf H_j|\le2B_3\lambda_m|\zeta_\square\mathbf H_k|\exp(-\tfrac12\delta_0{\rm dist}^{(\xi)}(X,\square)-\tfrac12\delta_0ML^m)\) when \({\rm dist}^{(\xi)}(X,\square)\ge ML^m\); otherwise \(X\) is large, \(d_j(X)\ge L^m\). Hence, as in (3.17) and CMP116 (1.30),
\[
|\text{far term}|\le\frac{6B_3\lambda_mK_Hg_k|B|}{\alpha_{2,j}}\lVert F_j\rVert_j\,e^{-(\ldots)}e^{-\kappa d_j(X)}\le6B_3K_H\,\varrho\,\Gamma'_m\lambda_m\,\lVert F_j\rVert_j\,e^{-(\ldots)}\,e^{-(\kappa_1-1)M^{-4}|Y\setminus X_0|}\,e^{-\kappa d_j(X)}.
\tag{6.3}
\]
No cancellation is needed for far terms, so \(\mathbb F_j\) may be replaced by each of its three parts (the Wilson part by the family of §6.3, last row).

### 6.5 Carrier resummation

This is CMP116 pp.7–9 and involves only geometry: (1.25)–(1.28) for near terms, (1.31)–(1.32) for far terms.

- *Near.* For fixed \(\square\) and \(j\): \(\sum_{X\subset\tilde\square^2}e^{-\kappa'd_j(X)}\le O(1)\cdot\#\{\square'\in\pi_j:\square'\subset\tilde\square^2\}=O(1)5^4\lambda_m^{-4}\) by (1.26). With (6.1): \(\lambda_m^{-4}(\Gamma'_m\lambda_m)^5\le(\Gamma'_m)^5L^{-m}\). With (6.2): \(\lambda_m^{-4}(\Gamma'_m)^r\lambda_m^{4+\vartheta}\le(\Gamma'_m)^4L^{-\vartheta m}\). The sums over \(Y_0\) and \(\square_0\) are (1.27)–(1.28) and give \(e\cdot\exp\tfrac1{16}(\kappa_1-2)d_k(Y)\), absorbed by \(\exp(-\tfrac18(\kappa_1-1)d_k(Y))\) from (1.25).
- *Far.* By the scaling inequality (1.31), \(d_j(X)\ge\lambda_m^{-1}d_k(X_0)\), and (1.32), the weights give \(e^{-(1-\delta)\kappa d_k(Y)-\delta\kappa d_j(X)}\). The sum over \(X\supset\square'\) is (1.26) with \(\delta\kappa\). The sum over \(\square'\in\pi_j\) is at most \(C\lambda_m^{-4}e^{-c_FL^m}\), \(c_F:=\tfrac12\min\{\delta\kappa,\tfrac12\delta_0M\}\) (cubes inside \(\tilde\square\) need a large \(X\); the others have the separation factor). With (6.3): \(\Gamma'_m\lambda_m\cdot\lambda_m^{-4}e^{-c_FL^m}=\Gamma'_mL^{3m}e^{-c_FL^m}\).

The decay left is \(e^{-(1-2\delta)\kappa d_k(Y)}=e^{-\kappa_*d_k(Y)}\) under the source's conditions \(\tfrac1{16}\kappa_1\ge(1-2\delta)\kappa\) (CMP116 p.9). Collecting, with \(\Gamma'_m\le\Gamma_m\), gives (3.1); the constants are \(C_E=O(M^{q'})e^{O(1)\kappa_1}K_H\max\{K_5^5,CK_{\mathfrak b}^3\}\), \(C_F=O(M^{q'})e^{O(1)\kappa_1}B_3K_H\).

Analyticity on \(\mathfrak D_k(Y)\): each term is analytic on \(U^c_{k+1}(\square_0,(1+2\beta)a_0,(1+2\beta)a_1,a_0)\) (near; Lemma 5.1) or on the space of Lemma 5.2 (far), and in \(B\) on \(|B|<2P_k\) by (S7), (K5), (K6). By (S-Res) all contain \(\mathfrak D_k(Y)\). The sum over terms with carrier \(Y\) converges uniformly by the majorant. This is item 2. \(\square\)

### 6.6 The age sum

\(\sum_m\Gamma_m^5L^{-\vartheta m}\le\theta^5(1+(1+\beta_0)^{10}\sum_{m\ge1}m^{5/2}L^{-\vartheta m})\) and \(\sum_m\Gamma_mL^{3m}e^{-c_FL^m}\) are finite numbers depending on \(L,\vartheta,\beta_0,c_F\) only (check (4) of finite comparison). This proves Corollary 3.2. They are AD (E14.24h), (E14.35), (E14.38), now on the source domain. The convergence is uniform in \(k\) because the comparison of Lemma 2.1 is in the age, not in the depth.

## 7. Proof of Theorem 3.3 and Proposition 3.4

**Theorem 3.3.** The identities of §6.1, items 1–3 and 5, do not use (H4). For near \(X\) This argument does not use CMP109 §4 (whose form (4.34), anchored at the insertion point, contains a first-moment term that vanishes only by Euclidean symmetry of the sum, p.290). Instead: by (S10) and Lemma 5.1, for every \(X\subset\tilde\square^2\) the function
\[
t_\square\ \longmapsto\ G_j\big(X,U_j(\square_0,\exp iB(t,t_\square))\big)-G_j(X,1)
\]
is analytic on the disc (1.22) and bounded there by \(C\lVert G_j\rVert_j(K_{\mathfrak b}\Gamma'_m)^5\lambda_m^4e^{-\kappa'd_j(X)}\): orders \(n\le4\) by (S10) with the construction (6.2) (degree \(n\), order \(r\le n\), gain \(\lambda_m^4\)), order five by §6.2. Cauchy's estimate at \(t_\square=0\) multiplies by \(2K_H\varrho\). The count \(\lambda_m^{-4}\) leaves \(C_M\varrho\Gamma_m^5\), with no decay in \(m\): the terms are marginal, as the source says (CMP119 p.260). Far terms are as in §6.4. This gives (3.3).

For (3.4): \(g_j^{\kappa_0}=Y_j^{-\kappa_0/2}\le(\tfrac12Y_k+\tfrac34d_Bm)^{-\kappa_0/2}\), and \(\sum_{m\ge0}\Gamma_m^5(\tfrac12Y+cm)^{-s}\le C_sY^{7/2-s}\) for \(s=\kappa_0/2\ge\tfrac92\) (compare with \(\int x^{5/2}(\tfrac12Y+cx)^{-s}dx\); check (5) of finite comparison). \(\square\)

The lower slope enters here and only here. The mature terms are a marginal perturbation, paid once per step as forcing (analysis §4(d)).

**Proposition 3.4.** By (S5) with \(\mathbf U=1\), \(F(X,\exp i\eta'\mathbf A)\) is analytic on the ball (4.4) of radius \(\alpha_2=c_2a_0\). By (S6), \(|F^{(2)}(X,x,y)|\le(8B_3/\alpha_2)^2\lVert F\rVert e^{-O(1)\kappa d(X\cup\{x,y\})}\), so \(|\Pi^F(x)|\le O(1)(B_3/\alpha_2)^2\lVert F\rVert e^{-\delta_1|x|}\) (this is (5.10)), and \(|\mathcal PF|\le\sum_x|x|^2|\Pi^F(x)|\le C(B_3,\delta_1)\alpha_2^{-2}\lVert F\rVert\), \(\delta_1=\tfrac12\min\{\delta_0,\kappa M^{-1}\}\). \(\square\)

## 9. The residue of Lemma L2

### 9.1 The cube-sup cutoff is the bond-product cutoff

CMP119 (3.16) defines \(\chi^{(k)}(R^c_{k+1})=\prod_{\square'\subset R^c_{k+1}}\chi(\{\sup_{b\in(\tilde\square'^{2})^{(k)*}}|A_k(b)|<\delta_k\})\). An indicator of a supremum bound over a set \(S\) of bonds is \(\prod_{b\in S}\chi(\{|A_k(b)|<\delta_k\})\), and indicators are idempotent. Hence
\[
\chi^{(k)}(R^c_{k+1})=\prod_{b\in\bigcup_{\square'\subset R^c_{k+1}}(\tilde\square'^2)^{(k)*}}\chi(\{|A_k(b)|<\delta_k\}).
\]
On the whole lattice (\(R_{k+1}=\emptyset\)) this is \(\prod_{b\in T^{(k)*}}\chi(\{|A_k(b)|<\delta_k\})\): exactly the cutoff \(\chi_k\) of CMP109 (2.9) and CMP116 (2.3) with \(\varepsilon_1g_k^{-1}\) replaced by the normalised cutoff \(P_k\) (the starred set excludes the bonds \(b_0(c)\) in both). The other characteristic functions of CMP119 §3 are either restrictions on the new background ((3.2)) or equal to 1 on the support of (3.16) ((3.3), by (3.19) of the source). So for the whole-lattice births the decomposition (2.3) and the estimates (2.22), (2.31)–(2.34) of CMP116 apply literally. Item (S-cut) of the companion note is not an assumption. (The printed \(\delta_k\) in (3.16) is in the variable before the scaling \(A_k'=g_kA_k\); in the scaled variable the bound is \(\delta_k/g_k=P_k\), as the companion note says.)

### 9.2 The tree-graph step conditional

*Setting.* Polymers: \(Z\in\mathbf D_{k+1}\) (on a finite torus); \(Z\not\sim Z'\) iff \(Z\cap Z'\) contains a cube or a wall of a cube (CMP116 (2.11)); activities \(H(Z)\) with \(|H(Z)|\le C_3(a)e^{-(1-8\delta)\frac L2\kappa d_{k+1}(Z)}\) (L2.3). \(\rho^T/n!\) on ordered tuples is the Ursell function of this hard-core relation.

*Kotecký–Preiss (1986).* If \(\mathsf a,\mathsf d\ge0\) satisfy \(\sum_{Z'\not\sim Z}|w(Z')|e^{\mathsf a(Z')+\mathsf d(Z')}\le\mathsf a(Z)\) for all \(Z\), then the cluster series converges absolutely and \(\sum_{\mathcal C\not\sim Z}|\phi^T(\mathcal C)\prod w|e^{\mathsf d(\mathcal C)}\le\mathsf a(Z)\), \(\mathsf d(\mathcal C)=\sum_i\mathsf d(Z_i)\). (To use the conclusion with \(Z\) a single cube, add the single cubes to the polymer set with activity zero; the criterion for them is the same computation.)

*Application.* Put \(c_{\mathsf d}:=(1-9\delta)\tfrac L2\kappa\), \(\mathsf d(Z):=c_{\mathsf d}(d_{k+1}(Z)+5)\), \(\mathsf a(Z):=\) number of \(LM\)-cubes of \(Z\). A polymer incompatible with \(Z\) contains one of at most \(9\mathsf a(Z)\) cubes. With \(\mathsf a(Z')\le24d_{k+1}(Z')\) (CMP116 (2.30)) the criterion holds if
\[
9\,C_3\,e^{5c_{\mathsf d}}\ \sup_{\square}\sum_{Z'\ni\square}e^{-(\frac12\delta L\kappa-24)d_{k+1}(Z')}\le1.
\]
The supremum is \(O(1)\) for \(\kappa\) large (the inequality (1.26)/(2.29) of the source, cited). Let \(C_3^{\rm KP}\) be the largest \(C_3\) for which this holds. For \(X\in\mathbf D_{k+1}\), every cluster with \(\bigcup Z_i=X\) is incompatible with a fixed cube of \(X\) and has \(\mathsf d(\mathcal C)\ge c_{\mathsf d}(d_{k+1}(X)+5)\) by (2.27). Hence for activities bounded by \(C_3^{\rm KP}e^{-(\ldots)}\): \(|\mathfrak E(X)|\le e^{-5c_{\mathsf d}}e^{-c_{\mathsf d}d_{k+1}(X)}\le e^{-5c_{\mathsf d}}e^{-\kappa d_{k+1}(X)}\), using \((1-10\delta)\tfrac L2=1\).

*Linearity in \(C_3\).* For activities \(zH(Z)\), \(|z|\le z_0:=C_3^{\rm KP}/C_3(a)\), the sum \(S_X(z)\) of the clusters with union \(X\) is a convergent power series in \(z\) without constant term, bounded by \(e^{-5c_{\mathsf d}}e^{-\kappa d_{k+1}(X)}\) on \(|z|\le z_0\). By the Schwarz lemma, \(|\mathfrak E(X)|=|S_X(1)|\le(C_3(a)/C_3^{\rm KP})e^{-5c_{\mathsf d}}e^{-\kappa d_{k+1}(X)}\). This is (L2.4) with \(c_3=e^{-5c_{\mathsf d}}/C_3^{\rm KP}=9\,O(1)\), and condition (A4) of the companion note is \(C_3(a)\le C_3^{\rm KP}\). It replaces the reference to [26] in CMP116 p.21. What stays cited: (2.27), (2.30) and the counting inequality.
