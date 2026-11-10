# Local deformation of propagators and the minimizer

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

## 2. Geometry

**Setting (G).** \(d\ge1\), integers \(L\ge2\), \(M\ge1\). Nested grids \(\mathcal G_n\), \(n\ge n_{\min}-1\), of closed cubes of side \(s_n=Mh_n\), \(h_n=L^nh_0\); every cube of \(\mathcal G_{n+1}\) is a union of \(L^d\) cubes of \(\mathcal G_n\). A **graded tiling** \(\mathcal T\) is a locally finite set of closed cubes ("tiles") with pairwise disjoint interiors covering \(\mathbb R^d\) (or a torus), each tile \(c\in\mathcal G_{\sigma(c)}\), \(\sigma(c)\ge n_{\min}\), such that

- **(T1a)** two tiles that touch (have a common point) differ in scale by at most one.

Tiles touching \(c\) are its neighbours; \(\Delta_*\) is a bound on their number; a set of tiles is \(*\)-connected if connected under "touch". The **tile metric** \(d_{\mathcal T}\) is the path metric with line element \(\lvert dx\rvert_\infty/h_{\bar\sigma(x)}\), \(\bar\sigma(x)=\max\{\sigma(c):x\in c\}\). (A tile has \(d_{\mathcal T}\)-diameter \(\le M\).)

*Examples.* (1) The proper tiling \(\mathcal T^{(k)}\) of [Boundary estimate e] §5.1 for a sequence satisfying (Nest), (Seq), (Thick): (T1a) is [Boundary estimate e] Lemma T1(a), \(\Delta_*=(L+2)^d-L^d\) is T1(c). (2) The same construction for any coarsened sequence, e.g. the \(j\)-floored tiling (all levels \(<j\) merged into scale \(j\)), or the uniform grid \(\mathcal G_k\). The lemmas below hold for all of them. *Over-sized tiles are allowed*: all that is used is that the tile metric is dominated by the metric of the operators (hypothesis (e) of Lemma W0).

**Lemma G1 (collar).** Let \(c\in\mathcal T\) have scale \(n\) and let \(N(c)=\{p:\operatorname{dist}_\infty(p,c)<s_{n-1}\}\). Every tile meeting \(N(c)\) touches \(c\). Hence two tiles that do not touch are at \(\infty\)-distance \(\ge\max(s_{\sigma(c)},s_{\sigma(c')})/L\), and \(\bar\sigma\le n+1\) on \(N(c)\).

*Proof.* Let \(t\ne c\) meet \(N(c)\). Since \(t\) is the closure of its interior and \(N(c)\) is open, there is \(p'\in\operatorname{int}t\cap N(c)\) off the hyperplanes of \(\mathcal G_{n-1}\); \(p'\notin c\) because interiors are disjoint. The faces of \(c\) lie on \(\mathcal G_{n-1}\)-hyperplanes, so \(p'\) lies in the interior of a \(\mathcal G_{n-1}\)-cube \(Q\) that touches \(c\) and has \(\operatorname{int}Q\cap c=\emptyset\). Let \(q\in Q\cap c\). By local finiteness some tile \(t_q\) contains \(q\) and points of \(\operatorname{int}Q\). Then \(t_q\ne c\) touches \(c\), so \(\sigma(t_q)\ge n-1\) by (T1a); \(t_q\) is a union of \(\mathcal G_{n-1}\)-cubes and meets \(\operatorname{int}Q\), so \(Q\subset t_q\). Thus \(p'\in\operatorname{int}t\cap\operatorname{int}t_q\), \(t=t_q\), and \(t\) touches \(c\). \(\square\)

**Lemma G2 (\(2^d\)).** Let \(S\) have \(\operatorname{diam}_\infty S<s_n\) and suppose every tile meeting \(S\) has scale \(\ge n\). Then \(S\) meets at most \(2^d\) tiles.

*Proof.* For each tile \(t\) meeting \(S\) pick a \(\mathcal G_n\)-cube \(Q_t\subset t\) meeting \(S\). Distinct tiles give distinct cubes. In each coordinate the projection of \(S\) has length \(<s_n\) and meets at most two closed grid intervals. \(\square\)

**Lemma G3 (tiles along a tree).** Let \(\Gamma\) be a connected union of finitely many rectifiable arcs of total \(d_{\mathcal T}\)-length \(D\). Let \(S_1,\dots,S_N\) be sets, each containing a point \(y_i\in\Gamma\), with \(\operatorname{diam}_\infty S_i\le s_\sigma/(8L^2)\) for some tile of scale \(\sigma\) containing \(y_i\). Then
\[
\#\{t\in\mathcal T:\ t\cap\textstyle\bigcup_iS_i\ne\emptyset\}\ \le\ 2^d\Bigl(1+\frac{16L^2}{M}\,D\Bigr).
\]
*Proof.* Put \(\ell_0=M/(8L^2)\). A closed depth-first tour of \(\Gamma\) has length \(2D\); cutting it into arcs of length \(\le\ell_0\) covers \(\Gamma\) by at most \(\max(1,\lceil2D/\ell_0\rceil)\le1+2D/\ell_0\) connected pieces of intrinsic diameter \(\le\ell_0\). Fix a piece \(A\), a point \(p\in A\) and a tile \(c\ni p\) of scale \(n\). A path in \(A\) from \(p\) of \(d_{\mathcal T}\)-length \(\le\ell_0\) has, as long as it stays in \(N(c)\), \(\infty\)-length \(\le h_{n+1}\ell_0=s_{n-1}/8\) (G1: \(\bar\sigma\le n+1\) there); so it never leaves \(N(c)\), and \(A\subset\{\lvert q-p\rvert_\infty\le s_{n-1}/8\}\). If \(y_i\in A\), any tile containing \(y_i\) touches \(c\), has scale \(\le n+1\), so \(\operatorname{diam}_\infty S_i\le s_{n+1}/(8L^2)=s_{n-1}/8\). Hence \(A\cup\bigcup_{y_i\in A}S_i\) lies in the ball \(\lvert q-p\rvert_\infty\le s_{n-1}/4\subset N(c)\), of \(\infty\)-diameter \(<s_{n-1}\). All tiles meeting it touch \(c\) and have scale \(\ge n-1\); by G2 there are at most \(2^d\). \(\square\)

This is the statement behind [II] (1.11): with \(m\) tiles met, \(D\ge(m-2^d)M/(2^{d+4}L^2)\). The threshold \(2^d\) (\(=2^4\) in the source) is the right one.

## 3. Deformed propagators

**Setting (S).** A finite set \(\mathfrak L\) of sites (bonds and points of all lattices and levels) with a tile map \(t:\mathfrak L\to\mathcal T\) and a reflexive symmetric relation \(\approx\) ("local neighbours"); \(S^+=\{b:b\approx b'\in S\}\). For \(T\subset\mathcal T\): \(\mathfrak L(T)=t^{-1}(T)\). Fix an integer \(K\ge1\) and put \(\operatorname{core}(T)=\{b:b^{+(K+1)}\subset\mathfrak L(T)\}\). Localization points \(y\in\mathfrak B\) with a pseudometric \(d\) and site sets \(\Delta(y)\) covering \(\mathfrak L\). Operators act on fields over \(\mathfrak L\); \(\lVert1_{\Delta(y)}P1_{\Delta(y')}\rVert\) denotes the operator norm from the sup norm on \(\Delta(y')\) to a fixed local seminorm on \(\Delta(y)\), and \(\mathfrak w_P(y,y')>0\) is the scale weight of the operator class (e.g. \((L^j\eta)^2\) in (3.108)). \(\mathfrak U\) is a domain of backgrounds.

**Hypothesis (W)** for an operator \(P\). \(P=\sum_{\omega}P_\omega\) (a countable family, each \(\omega\) carrying a finite \(*\)-connected \(\mathcal T(\omega)\subset\mathcal T\)), with
- (W1) \(P_\omega(b,b')=0\) unless \(b,b'\in\operatorname{core}(\mathcal T(\omega))\);
- (W2) \(P_\omega\) is a holomorphic function on \(\mathfrak U\) of the background restricted to \(\mathfrak L(\mathcal T(\omega))\);
- (W3) there are \(B,\delta,\kappa_{\max}>0\) with, for all \(y,y'\), all \(0\le\kappa\le\kappa_{\max}\), uniformly on \(\mathfrak U\):
\[
\sum_\omega e^{\kappa\lvert\mathcal T(\omega)\rvert}\,\lVert1_{\Delta(y)}P_\omega1_{\Delta(y')}\rVert\ \le\ B\,e^{2^d\kappa}\,\mathfrak w_P(y,y')\,e^{-\delta d(y,y')}.
\]

**Lemma W0 (the source form implies (W)).** Suppose \(P=\sum_\omega P_\omega\) over walks or trees \(\omega\) of localization domains \(X_0,\dots,X_n\) (\(n=\lvert\omega\rvert\)), with dependence domains \(\tilde X_i\supset X_i\), \(\bigcup_i\tilde X_i\) connected, such that
- (a) \(P_\omega(b,b')=0\) unless \(b^{+(K+1)},b'^{+(K+1)}\subset\bigcup_i\tilde X_i\);
- (b) \(P_\omega\) is holomorphic on \(\mathfrak U\) in the background restricted to \(\bigcup_i\tilde X_i\);
- (c) \(\lVert1_{\Delta(y)}P_\omega1_{\Delta(y')}\rVert\le B_s\,\mathfrak w_P(y,y')\,\epsilon^{\lvert\omega\rvert}e^{-\delta_sd(\omega,y,y')}\), where \(d(\omega,y,y')\) is the infimum of the \(d\)-lengths of trees through \(y,y'\) and one point \(y_i\) of each \(X_i\);
- (d) the number of \(\omega\) with \(\lvert\omega\rvert=n\) and \(X_0\cap\Delta(y)\ne\emptyset\) is \(\le n_0K_w^n\), and \(K_w\epsilon\le\frac12\);
- (e) \(d\ge d_{\mathcal T}\) on paths, and \(\operatorname{diam}_\infty\tilde X_i\le s_\sigma/(8L^2)\) for every tile (of scale \(\sigma\)) containing a point of \(X_i\).

Let \(\mathcal T(\omega)\) be the set of tiles meeting \(\bigcup_i\tilde X_i\). Then (W) holds with \(B=2n_0B_s\), \(\delta=\frac12\delta_s\), \(\kappa_{\max}=\delta_sM/(2^{d+5}L^2)\).

*Proof.* \(\mathcal T(\omega)\) is \(*\)-connected because \(\bigcup\tilde X_i\) is connected. (W1), (W2) are deduction, conditional. Take a tree \(\Gamma\) through \(y,y_1,\dots,y'\) of \(d\)-length \(\le d(\omega,y,y')+\epsilon'\); its \(d_{\mathcal T}\)-length is no larger. Lemma G3 with \(S_i=\tilde X_i\) gives \(\lvert\mathcal T(\omega)\rvert\le2^d(1+16L^2d(\omega,y,y')/M)\), so \(e^{\kappa\lvert\mathcal T(\omega)\rvert}\le e^{2^d\kappa}e^{\frac12\delta_sd(\omega,y,y')}\) for \(\kappa\le\kappa_{\max}\). With \(d(\omega,y,y')\ge d(y,y')\) (triangle inequality) and additional assumption,
\[
\sum_\omega e^{\kappa\lvert\mathcal T(\omega)\rvert}\lVert\cdot\rVert\le B_s\mathfrak w_Pe^{2^d\kappa}e^{-\frac12\delta_sd(y,y')}\,n_0\sum_n(K_w\epsilon)^n\le2n_0B_s\,\mathfrak w_Pe^{2^d\kappa}e^{-\frac12\delta_sd(y,y')}.\qquad\square
\]
With [P] (3.108): \(\delta_s=\frac12\delta_0\), \(\epsilon=O(1)M_1^{-1/2}\), so \(\delta=\frac14\delta_0\) and \(\kappa_{\max}=\delta_0M/(2^{d+6}L^2)\).

**Theorem W.** Assume (W). For \(s\in\mathbb C^{\mathcal T}\) put \(P(s)=\sum_\omega s^{\mathcal T(\omega)}P_\omega\), \(s^T=\prod_{t\in T}s_t\). Then for \(\lvert s_t\rvert\le e^\kappa\), \(\kappa\le\kappa_{\max}\):
1. the series converges absolutely, \(P(s)\) is holomorphic in \((s,U)\), \(P(1)=P\), and \(\lVert1_{\Delta(y)}P(s)1_{\Delta(y')}\rVert\le Be^{2^d\kappa}\mathfrak w_P(y,y')e^{-\delta d(y,y')}\);
2. if \(s_t=0\) for \(t\notin Y\), and \(Y_a\) are the \(*\)-components of \(Y\), then \(P(s)=\sum_aP_a(s)\), where \(P_a(s)=\sum_{\mathcal T(\omega)\subset Y_a}s^{\mathcal T(\omega)}P_\omega\) has kernel supported in \(\operatorname{core}(Y_a)\times\operatorname{core}(Y_a)\) and depends only on \(s\restriction Y_a\) and the background on \(\mathfrak L(Y_a)\).

*Proof.* (1) is (W3). (2): a \(*\)-connected \(\mathcal T(\omega)\subset Y\) lies in one component; \(\operatorname{core}\) is monotone. \(\square\)

So \(P(s)\) satisfies every kernel bound of \(P\) with \((B_0,\delta_0)\to(\hat B_0,\hat\delta_0):=(2n_0B_se^{2^d\kappa},\frac14\delta_0)\). This is [II] (1.11) with its two gaps closed.

**Remark 3.4 (walk terms on the complex domain; status conditional; additional assumption).** The proofs of [P] Theorems 3.7–3.10 use (i) the inequalities of Theorems 3.1–3.3 for the *localized* operators \(G'_\square,C_\square,G_\square\), and (ii) the algebraic identities (3.88), (3.95), (3.104), (3.105). For a complex \(U'U\) on (3.37), (i) holds by Corollary 3.6 and Theorem 3.4 applied to the local sequences \(\{\Omega_n(\square)\}\) (the local sequence needs \(\lvert A'\rvert<\alpha_1(L^n\eta)^{-1}\) on \(\Omega_n(\square)\); where the global layer index is one less than the local one this costs a factor \(L\), resp. \(L^2\), in \(\alpha_1\)). (ii) are identities between functions holomorphic in \(A'\) on the connected domain (3.37), valid at real points, hence everywhere. So the expansions hold on the complex domain with each term holomorphic in the background restricted to \(\bigcup\tilde X_i^5\), and with the constants of Theorem 3.4. The proof assumes the estimates of [P] §C; this is why (W-ms) below stays a named input.

## 4. The decoupling calculus and the localized minimiser

### 4.1 Subordination

Fix \(Y\subset\mathcal T\) with \(*\)-components \(Y_a\), and restrict to \(s\) with \(s_t=0\) for \(t\notin Y\). Put \(Z^\kappa_a=\operatorname{core}(Y_a)^{+\kappa}\) for \(0\le\kappa\le K\); then \((Z^\kappa_a)^+\subset\mathfrak L(Y_a)\), and the sets \(\mathfrak L(Y_a)\) are disjoint. Data are fields \(z\) (the variables) and the background \(U\).

**Definition.** A field-valued function \(\Psi\) of \((z,U,s)\) is **\(Y\)-subordinate of depth \(\kappa\)** if, for each \(a\), \(\Psi\restriction Z^\kappa_a\) depends on \((z,U,s)\) only through \((z,U)\restriction\mathfrak L(Y_a)\) and \(s\restriction Y_a\).

**Lemma 4.1 (rules).**
- (R1) \(z\), and every \(\approx\)-local function of \((z,U)\), has depth \(K\).
- (R2) If \(F\) is \(\approx\)-local (\(F(\Psi_1,\dots;U)(b)\) depends only on \(\Psi_i\restriction b^+\), \(U\restriction b^+\)) and the \(\Psi_i\) have depth \(\ge\kappa+1\), then \(F(\Psi_1,\dots)\) has depth \(\kappa\).
- (R3) If \(P\) satisfies (W) and \(\Psi\) has depth \(\ge0\), then \(P(s)\Psi\) has depth \(K\). The same holds for \(P^*(s)=\sum s^{\mathcal T(\omega)}P_\omega^*\).
- (R4) Sums, and pointwise limits, of functions of depth \(\ge\kappa\) have depth \(\ge\kappa\).

*Proof.* (R1), (R2): for \(b\in Z^\kappa_a\), \(b^+\subset Z^{\kappa+1}_a\subset\mathfrak L(Y_a)\). (R3): by Theorem W(2), \(P(s)\Psi=\sum_{a'}P_{a'}(s)(\Psi\restriction\operatorname{core}(Y_{a'}))\), and the \(a'\)-th term is supported in \(\operatorname{core}(Y_{a'})\subset\mathfrak L(Y_{a'})\), which does not meet \(Z^K_a\subset\mathfrak L(Y_a)\) for \(a'\ne a\). On \(Z^K_a\) only the \(a\)-th term survives, and it depends on \(s\restriction Y_a\), \(U\restriction\mathfrak L(Y_a)\) and \(\Psi\restriction Z^0_a\). (R4) is clear. \(\square\)

**Calculus systems.** A formula built from data, unknown fields \(X_i\) (assigned depths \(\kappa_i\)), deformed operators \(P(s),P^*(s)\) with \(P\) from a finite list \(\mathcal O\) satisfying (W), and \(\approx\)-local holomorphic maps, is **admissible** if, computing depths by R1–R3, every node has depth \(\ge0\) and the node defining \(X_i\) has depth \(\ge\kappa_i\). If \(\mathfrak F\) is admissible and \(X\) is \(Y\)-subordinate with the depths \((\kappa_i)\), so is \(\mathfrak F(X)\). Hence a fixed point obtained as the limit of the iterates \(\mathfrak F^n(0)\) is \(Y\)-subordinate (R4). A depth budget \(K\) means: at most \(K\) local maps between two consecutive operators of \(\mathcal O\).

### 4.2 The two inputs

> **(W-ms).** For the sequence \(\{\Omega_n\}\) and backgrounds in the complex domain \(\mathfrak U\) of [P] ((3.35)–(3.38) with small absolute \(\alpha_0,\alpha_1\)), every operator of \(\mathcal O=\{H,H_0,\tilde G,(QGQ^*)^{-1},P_1\}\) and its adjoint has an expansion satisfying (a)–(e) of Lemma W0 in all the norms of [P] Theorems 3.1–3.3, (3.132), (3.133) and [V] (130), with \(B_s,\epsilon,n_0,K_w,\delta_s=\frac12\delta_0\) depending on \(d,L,M_1\) only, and with tiles of size \(M\ge c_dL^2M_1\).

Hypotheses: source input for real backgrounds at the level of proof described in S2–S3; the complex extension is S4/Remark 3.4; the counting constants \(n_0,K_w\) for tree-like walks are not printed additional assumption. \(M\ge c_dL^2M_1\) (hypothesis (e) and the margin deduction) is the multiscale form of "\(R_1M_1M^{-1}\le1\)" ([II] p.3) and of \(M_1<M_2<M\) ([III] p.245).

> **(S-struct).** (i) *Form.* \(\mathcal H(B)=\mathscr A_0+H_0B-HD(\mathscr A_0+H_0B)\), where \(D\) is the fixed point of [V] (50), \(\mathscr A_0\) the fixed point of (180), \(\delta V/\delta A'\) is given by the right-hand sides of (85), (88), (89), (90), (93)–(96), and \(\mathfrak D^*w=L\eta(\delta C/\delta A)^*(\cdot)\,u\) with \(u=w-H^*[L\eta(\delta C/\delta A)^*(\cdot)u]\) (the adjoint of (70)). Every map in these formulas is an operator of \(\mathcal O\) (or \(Q,Q^*,a,D^*\), which are local at the block scale) or a \(\approx\)-local holomorphic map (\(C_j\), \(\delta C_j/\delta A\) and its adjoint, \(V_0'\), \(\partial V_0'/\partial A\), \(J\), the commutator expressions (94)–(96)); the depth budget is \(K=3\). (ii) *Estimates.* The proofs of [V] Propositions 3, 4, 6 and of Proposition 9's bounds (19)–(21), and of [II] (1.13)–(1.21), use the operators of \(\mathcal O\) only through their kernel bounds with constants \((B_0,\delta_0)\), and remain valid, with thresholds \(\propto B_0^{-2}\), when these bounds hold with other constants.

Hypotheses: (i) is (c) — printed source for (80), (85)–(96), (179), (180); source text for (44)–(73). The depth count is mine: \(A'=\mathscr A_0+H_0B\) has depth 3; \(D(A')\) depth 2; \(A'-HD\) depth 3; \(V_0'\) and the \(D^*\)-commutators depth 2; \(\mathfrak D^*w\) depth \(\ge1\); then \(\tilde G\) resets to 3. (ii) is the source's own assertion ([II] p.3, source, quoted in S6); The formula gives it against [V] §C (source), the displayed proof of Proposition 4 (source) and (116)–(121) (source), where every use of an operator is through a norm or kernel bound or a Cauchy estimate. The proof assumes [V] §§E–F in full.

**A point the source leaves implicit.** The identities used to *derive* (87)–(89) (e.g. \(\Delta_aH=(G^{-1}-Q^*aQ)GQ^*(QGQ^*)^{-1}\)) hold for the true operators only. The deformed system must therefore be *defined* by the final operator forms (88)–(90), (93), (179), (180) with each operator of \(\mathcal O\) replaced by its \(s\)-version — not by (80) with \(H(s)\) inserted. At \(s=1\) the two agree; for other \(s\) the deformed solution is an auxiliary interpolation, which is all that is needed. Likewise the \(J\)-term is absent from (180) because the base point is critical; in the deformed system and for off-critical complex \((\mathbf U,\mathbf J)\) it is absent by definition ([I] p.273: "we replace the configurations \(U_{k+1},J_{k+1}\) occurring in operators there by the configurations \(\mathbf U,\mathbf J\)").

### 4.3 Theorem M (the localized response) conditional

Let \(\mathcal T\) be a graded tiling for which (W-ms) holds (the proper tiling \(\mathcal T^{(k)}\), or any coarsening). Let \(1\le\kappa\le\kappa_{\max}\) and \(\hat B_0=2n_0B_se^{2^d\kappa}\). For an output label \(x\) (a site together with one of the admissible seminorms \(\nu\), normalized by its scale weight \(\mathfrak w_\nu(x)\)) let \(R_x\) be the set of tiles meeting \(x^{+(K+1)}\); \(\lvert R_x\rvert\le2^d\) (G2), every tile of \(R_x\) touches or equals \(t(x)\) (G1), and \(x\in\operatorname{core}(R_x)\). Let \(\mathcal Y(x)\) be the set of finite \(Y\supset R_x\) such that every \(*\)-component of \(Y\setminus R_x\) touches \(R_x\).

**Theorem M.** Assume (W-ms) and (S-struct). There is \(\varepsilon_{\mathcal H}=c_{\mathcal H}\hat B_0^{-2}\) (\(c_{\mathcal H}\) depending on \(d,L,C_2,C_4\)) such that:
1. the deformed system has a unique small solution \(\mathcal H(B;s,U)\), holomorphic on \(\{\lVert B\rVert_\infty<\varepsilon_{\mathcal H}\}\times\{\lvert s_t\rvert<e^\kappa\}\times\mathfrak U\), with \(\lvert\mathcal H(B;s,U)\rvert_\nu\le4\hat B_0\lVert B\rVert_\infty\) in every admissible norm, \(\mathcal H(B;1,U)=\mathcal H(B;U)\), \(\mathcal H(0;s,U)=0\);
2. for every zero pattern \(Y\), \(\mathcal H(\cdot;s,\cdot)\) is \(Y\)-subordinate of depth \(\ge0\);
3. **(M-loc):** \(\mathcal H(B)(x)=\sum_{Y\in\mathcal Y(x)}\psi_{x,Y}(B)\), where \(\psi_{x,Y}\) is holomorphic on \(\{\lVert B\rVert_\infty<\varepsilon_{\mathcal H}\}\times\mathfrak U\), depends only on \(B\) and \(U\) restricted to \(\mathfrak L(Y)\), vanishes at \(B=0\), and
\[
\lvert\psi_{x,Y}(B)\rvert_\nu\le4\hat B_0\,\lVert B\restriction\mathfrak L(Y)\rVert_\infty\,e^{-(\kappa-1)\lvert Y\setminus R_x\rvert}.
\]
4. The same holds for the composite response \(\Psi^{(j,k)}(z)=\mathcal H_j\bigl(Q_j(\eta\mathcal H_k(B'(z)))\bigr)\), \(j\le k\) (for \(j=k\): \(\mathcal H_k(B'(z))\)), \(z=A_k\), \(B'=g_kCz-h\tilde D(g_kCz)\), \(\lvert B'\rvert\le C_{B'}g_k\lvert z\rvert\), on the proper tiling \(\mathcal T^{(k)}\), with the walks of both sequences deformed by the same \(s\): on \(\lVert z\rVert_\infty<R_z:=\varepsilon_\Psi/g_k\),
\[
\lvert\psi_{x,Y}(z)\rvert_\nu\le C_1^\Psi\,g_k\lVert z\restriction Y\rVert_\infty\,e^{-(\kappa-1)\lvert Y\setminus R_x\rvert},\qquad C_1^\Psi=16\,c_QC_{B'}\hat B_0^{(j)}\hat B_0^{(k)},\quad\varepsilon_\Psi=\varepsilon_{\mathcal H}/(4c_QC_{B'}\hat B_0^{(k)}).
\]

*Proof.* (1) By Theorem W the deformed operators satisfy the kernel bounds with \((\hat B_0,\frac14\delta_0)\); (S-struct)(ii) gives the contractions, and the solution is a uniform limit of holomorphic iterates. \(\mathcal H(0;s)=0\) because \(D\) and \(\delta V/\delta A'\) vanish to second order. (2) The iterates of the three nested fixed points (\(D\); \(u\); \(\mathscr A_0\)) are admissible calculus systems by (S-struct)(i); apply §4.1. (3) Fix \(x\) and apply Theorem D (§5) to \(\Phi(B,s)=\mathcal H(B;s)(x)\) with root \(R_x\) (\(s\equiv1\) on \(R_x\)) and \(\rho=e^\kappa\). (Dec) holds: for a pattern \(Y\supset R_x\), \(x\in\operatorname{core}(R_x)\subset Z^0_a\) for the component \(Y_a\supset R_x\), and (2). The bound \(A=4\hat B_0\varepsilon_{\mathcal H}\), \((e^\kappa-1)^{-1}\le e^{-(\kappa-1)}\), and the Schwarz lemma on the polydisc in the variables \(B\restriction\mathfrak L(Y)\) (the terms vanish at \(0\) because \(\Phi(0,s)=0\) for all \(s\)) give the estimate. (4) \(B'\) and \(Q_j\) are local (blocks are contained in tiles), so the composite is again a calculus system. For the \(j\)-sequence the proper tiles of \(\mathcal T^{(k)}\) in \(\Omega_{j+1}\) are over-sized, which Lemma W0(e) allows. The bound is the product of the two bounds of (1). \(\square\)

**Remark 4.4 (constants).** With \(d=4\): \(\hat B_0=2n_0B_se^{16\kappa}\), exactly the \(B_0e^{16\kappa_1}\) of [II] (1.11); \(\varepsilon_{\mathcal H}\propto e^{-32\kappa}\), the "\(e^{32\kappa_1}\varepsilon_1\) smaller than an absolute constant" of [II] (1.21). \(\kappa\) is free in \([1,\delta_0M/(2^{d+6}L^2)]\).

## 5. Abstract decoupling

In this section \(\mathcal T\) is a finite set with a symmetric relation "touch" of degree \(\le\Delta_*\); variables \(z=(z_i)_{i\in I}\), each with a tile \(t(i)\); \(\mathcal T_{\rm cur}=t(I)\); \(\mathcal Z_r=\{\lvert z_i\rvert<r\}\). For \(Y\supset R\), \(Y_R\) is the union of the \(*\)-components of \(Y\) that meet \(R\).

**Theorem D.** Let \(\emptyset\ne R\subset\mathcal T\), \(\rho>1\), and let \(\Phi\) be holomorphic on \(\mathcal Z\times\{s\in\mathbb C^{\mathcal T\setminus R}:\lvert s_t\rvert<\rho\}\) with \(\lvert\Phi\rvert\le A\). Assume
> **(Dec)** for every \(Y\) with \(R\subset Y\subset\mathcal T\), on the slice \(\{s_t=0\ \forall t\notin Y\}\) the function \(\Phi\) depends only on the \(z_i\) with \(t(i)\in Y_R\) and the \(s_t\) with \(t\in Y_R\setminus R\).

Then \(\Phi(z,1)=\sum_T\Phi_T(z)\), the sum over \(T\subset\mathcal T\setminus R\) each of whose \(*\)-components touches \(R\), with
\[
\Phi_T(z)=\int_{[0,1]^T}\partial_s^T\Phi(z;s_T,0)\,ds_T ,\qquad\lvert\Phi_T\rvert\le A(\rho-1)^{-\lvert T\rvert},
\]
and \(\Phi_T\) depends only on the \(z_i\) with \(t(i)\in R\cup T\).

*Proof.* For smooth \(f\) on \([0,1]^S\): \(f(1_S)=\sum_{T\subset S}\int_{[0,1]^T}\partial^Tf(s_T,0_{S\setminus T})ds_T\) (induction on \(\lvert S\rvert\)). Take \(S=\mathcal T\setminus R\). If a component of \(T\) does not touch \(R\), then by (Dec) with \(Y=R\cup T\) the integrand does not depend on some \(s_t\), \(t\in T\), and the term vanishes. For \(s_T\in[0,1]^T\) the polydisc of radius \(\rho-1\) about \(s_T\) lies in the domain; Cauchy gives the bound. The \(z\)-dependence is (Dec). \(\square\)

**Theorem D′ (dangling clusters resummed).** Under the hypotheses of Theorem D, \(\Phi(z,1)=\sum_{Y'}\Phi^{\rm res}_{Y'}(z)\), the sum over \(Y'\subset\mathcal T\setminus R\) (including \(\emptyset\)) each of whose \(*\)-components touches \(R\) **and contains a tile of \(\mathcal T_{\rm cur}\)**, where
\[
\Phi^{\rm res}_{Y'}(z)=\int_{[0,1]^{Y'}}\partial_s^{Y'}\Phi(z;s_{Y'},\sigma^{Y'})\,ds_{Y'},\qquad\sigma^{Y'}_t=\begin{cases}0,&t\in\bigl(N(Y')\cup\mathcal T_{\rm cur}\bigr)\setminus(R\cup Y'),\\1,&\text{otherwise},\end{cases}
\]
\(N(Y')\) being the set of tiles touching \(Y'\). \(\Phi^{\rm res}_{Y'}\) depends only on the \(z_i\) with \(t(i)\in R\cup Y'\), and \(\lvert\Phi^{\rm res}_{Y'}\rvert\le A(\rho-1)^{-\lvert Y'\rvert}\).

*Proof.* Each \(T\) of Theorem D splits uniquely as \(T=Y'\sqcup T_d\): \(Y'\) the union of the components containing a current tile, \(T_d\) the rest. Then \(T_d\subset W(Y'):=\mathcal T\setminus(R\cup Y'\cup N(Y')\cup\mathcal T_{\rm cur})\) and every component of \(T_d\) touches \(R\). Conversely, for \(T_d\subset W(Y')\) the components of \(Y'\sqcup T_d\) are those of \(Y'\) and of \(T_d\); if all components of \(T_d\) touch \(R\) this is a \(T\) of Theorem D with this splitting, and otherwise the term \(\int\partial^{Y'\sqcup T_d}\Phi(\cdot,0)\) vanishes by (Dec). Therefore
\[
\sum_{T_d}\Phi_{Y'\sqcup T_d}=\sum_{T_d\subset W(Y')}\int_{[0,1]^{T_d}}\partial^{T_d}g(s_{T_d},0)=g(1_{W(Y')}),\qquad g(s_W)=\int_{[0,1]^{Y'}}\partial^{Y'}\Phi(z;s_{Y'},s_W,0),
\]
by the interpolation identity in the \(W(Y')\)-variables. This is \(\Phi^{\rm res}_{Y'}\). The bound is Cauchy in \(s_{Y'}\) at a point whose other coordinates are \(0\) or \(1\). At this pattern the "on" set is \(Y^0=R\cup Y'\cup W(Y')\), and \(\mathcal T_{\rm cur}\cap Y^0\subset R\cup Y'\); (Dec) gives the \(z\)-dependence. \(\square\)

Theorem D′ is not in the source. In the small-field case the root is one cube with \(O(1)\) neighbours and [II] (1.27) bounds the sum over all \(Y_0\) by \(e\). In the multiscale case an old carrier \(X\) of birth \(j\) that reaches a layer \(n<j\) has \(\sim L^{(d-1)(j-n)}\) proper tiles on its boundary there, and the corresponding bound \(\exp(\epsilon\lvert\partial R(X)\rvert)\) is not uniform. Clusters that do not reach the current region carry no current dependence; D′ sums them exactly.

**Lemma 5.1 (counting).** Let \(R_x\subset\mathcal T\) with \(\lvert R_x\rvert\le2^d\) and \(\mathcal Y(x)\) as in §4.3. Put \(b_0=\log(2^{d+1}\Delta_*^2)\). For \(b\ge b_0+\theta\), \(\theta\ge0\), \(D\ge0\):
\[
\sum_{Y\in\mathcal Y(x),\ \lvert Y\setminus R_x\rvert\ge D}e^{-b\lvert Y\setminus R_x\rvert}\le e\cdot e^{-\theta D}.
\]
*Proof.* \(Y\setminus R_x\) is a union of \(*\)-connected clusters, each containing one of the \(\le2^d\Delta_*\) tiles touching \(R_x\). The number of \(*\)-connected sets of \(m\) tiles containing a given tile is \(\le\Delta_*^{2(m-1)}\) ([Hidden components] Lemma A4). So the sum of \(e^{-(b-\theta)\lvert Y\setminus R_x\rvert}\) is \(\le\prod_u\bigl(1+\sum_{m\ge1}\Delta_*^{2(m-1)}e^{-(b-\theta)m}\bigr)\le\exp(2^d\Delta_*\cdot2e^{-(b-\theta)})\le e\). \(\square\)

(For \(d=4\), \(L=2\): \(\Delta_*=240\), \(b_0\approx14.4\).)

**Definition (M-loc)\((a,R_z,\{A_x\})\).** Output labels \(x\) with roots \(R_x\) as in Lemma 5.1; functions \(\psi_{x,Y}\), \(Y\in\mathcal Y(x)\), holomorphic on \(\mathcal Z_{R_z}\), depending only on the \(z_i\) with \(t(i)\in Y\), with \(\psi_{x,Y}(0)=0\) and \(\lvert\psi_{x,Y}(z)\rvert\le A_x(\lVert z\restriction Y\rVert_\infty/R_z)e^{-a\lvert Y\setminus R_x\rvert}\); \(\Psi_x=\sum_Y\psi_{x,Y}\). Consequently \(\psi_{x,Y}\equiv0\) unless \(Y\cap\mathcal T_{\rm cur}\ne\emptyset\). Let \(D(R_x,t)\) be the least \(\lvert Y\setminus R_x\rvert\) over \(Y\in\mathcal Y(x)\) containing \(t\) (the tile distance), and \(D_x=\min_{t\in\mathcal T_{\rm cur}}D(R_x,t)\).

**Theorem T (tangent decay).** Under (M-loc) with \(a>b_0\): for \(\lVert z\rVert_\infty\le R_z/2\) and every \(i\),
\[
\lvert\partial_i\Psi_x(z)\rvert\le\frac{2e\,A_x}{R_z}\,e^{-(a-b_0)D(R_x,t(i))}.
\]
*Proof.* Only \(Y\ni t(i)\) contribute, and they have \(\lvert Y\setminus R_x\rvert\ge D(R_x,t(i))\). Cauchy on the polydisc of radius \(R_z/2\) about \(z\) gives \(\lvert\partial_i\psi_{x,Y}\rvert\le2A_xe^{-a\lvert Y\setminus R_x\rvert}/R_z\). Lemma 5.1 with \(b=a\), \(\theta=a-b_0\). \(\square\)

This is [Boundary estimate f] Lemma 3 with the root handled by Lemma 5.1 (no factor \(\Delta_*^{2\lvert R_x\rvert}\)).

**Lemma RE (second deformation).** Assume (M-loc) with \(a\ge\kappa_2+b_0+\theta\), \(\kappa_2,\theta\ge0\). Fix \(R\subset\mathcal T\). For \(\tau\in\mathbb C^{\mathcal T\setminus R}\) put \(\Psi_x(z;\tau)=\sum_{Y\in\mathcal Y(x)}\tau^{Y\setminus R}\psi_{x,Y}(z)\). Then on \(\mathcal Z_{R_z}\times\{\lvert\tau_t\rvert\le e^{\kappa_2}\}\):
1. \(\Psi_x(z;\tau)\) is holomorphic, \(\Psi_x(z;1)=\Psi_x(z)\), \(\Psi_x(0;\tau)=0\), and
\[
\lvert\Psi_x(z;\tau)\rvert\le e\,A_x\,\frac{\lVert z\rVert_\infty}{R_z}\,e^{\kappa_2\lvert R_x\setminus R\rvert}\,e^{-\theta D_x};
\]
2. if \(\tau_t=0\) for \(t\notin Y^0\) (\(Y^0\supset R\)) and \(R_x\subset R\), then \(\Psi_x(z;\tau)\) depends only on the \(z_i,\tau_t\) with \(t(i),t\in(Y^0)_R\).

*Proof.* (1) \(\lvert\tau^{Y\setminus R}\rvert\le e^{\kappa_2\lvert R_x\setminus R\rvert}e^{\kappa_2\lvert Y\setminus R_x\rvert}\); nonzero terms have \(\lvert Y\setminus R_x\rvert\ge D_x\); Lemma 5.1 with \(b=a-\kappa_2\). (2) Only \(Y\subset Y^0\) contribute; such \(Y\) is \(*\)-connected to \(R_x\subset R\), so \(Y\subset(Y^0)_R\). \(\square\)

**This is the estimate the multiscale case needs and the source does not display:** the deformed response is small in old layers — by \(e^{-\theta D_x}\), with \(D_x\) the number of proper tiles between \(x\) and the current region — *uniformly on the complex polydisc*. The first deformation (on walks) does not give this without a weighted fixed-point argument; the second (on the terms of the first expansion) gives it for free.

**Theorem C (composition).** Assume (M-loc) with \(a\ge\kappa_2+b_0+\theta\), \(\kappa_2\ge1\), \(\theta\ge0\). Let \(\mathfrak X\) be a finite set of output labels, \(R\supset\bigcup_{x\in\mathfrak X}R_x\) \(*\)-connected, and \(G\) holomorphic with \(\lvert G\rvert\le K_G\) on \(\{u\in\mathbb C^{\mathfrak X}:\lvert u_x\rvert<\varrho_x\}\). Put
\[
r_T=\min\Bigl(R_z,\ \inf_{x\in\mathfrak X}\frac{\varrho_x\,R_z\,e^{\theta D_x}}{e\,A_x}\Bigr).
\]
Then on \(\mathcal Z_{r_T}\): \(G\bigl((\Psi_x(z))_{x\in\mathfrak X}\bigr)=\sum_{Y'}F_{Y'}(z)\), over \(Y'\subset\mathcal T\setminus R\) each of whose components touches \(R\) and contains a current tile, with \(F_{Y'}\) holomorphic on \(\mathcal Z_{r_T}\), depending only on the \(z_i\) with \(t(i)\in R\cup Y'\), and
\[
\lvert F_{Y'}(z)\rvert\le K_G\,e^{-(\kappa_2-1)\lvert Y'\rvert},\qquad F_{Y'}(0)=0\ (Y'\ne\emptyset),\qquad F_\emptyset(0)=G(0).
\]
Hence for \(i\) with \(t(i)\in R\cup Y'\): \(\lvert\partial_iF_{Y'}(z)\rvert\le K_Ge^{-(\kappa_2-1)\lvert Y'\rvert}/(r_T-\lvert z_i\rvert)\), and \(\partial_iF_{Y'}\equiv0\) otherwise.

*Proof.* By Lemma RE(1) (with \(R_x\subset R\)), \(\Phi(z,\tau)=G(\Psi(z;\tau))\) is defined, holomorphic and bounded by \(K_G\) on \(\mathcal Z_{r_T}\times\{\lvert\tau_t\rvert<e^{\kappa_2}\}\). By RE(2) it satisfies (Dec) with root \(R\). Apply Theorem D′ with \(\rho=e^{\kappa_2}\). \(\Phi(0,\tau)=G(0)\) for all \(\tau\), so the terms with \(Y'\ne\emptyset\) vanish at \(z=0\). \(\square\)

## 6. The T step for one B-term

### 6.1 Set-up

T step \(k\to k+1\). Variables \(z=A_k\) on \(\Lambda^{(k)*}_{k+1}\); real support \(\lVert z\rVert_\infty\le P_k=A_1\ell_k^{p_0}\) (S9). Tiling: the proper tiling \(\mathcal T=\mathcal T^{(k)}\) of [Boundary estimate e] §5.1 for \(\{\Omega_n\}_{n\le k}\) (premises (Nest), (Seq), (Thick)); \(\mathcal T_{\rm cur}\) = the scale-\(k\) tiles containing current sites. By [Boundary estimate e] Lemma T3, a \(*\)-connected set containing a tile of scale \(n\) and a current tile has \(\ge k-n+1\) tiles; so \(D_x\ge(k-n-1)_+\) for \(x\) in layer \(n\).

A boundary term of birth \(j\le k\): \(\mathbf B^{(j)}(X,(\mathbf U,\mathbf J),A,\{S_i\cap X\})\), \(X\in\mathbf D_j\), analytic on \(\tilde U^c_j(X,\tilde\alpha_0,\tilde\alpha_1)\) with \(\lvert\mathbf B^{(j)}\rvert<B_0e^{-\kappa_Bd_j(X)}\) uniformly in the old variables ((2.42), source). By [III] p.276 ("we apply the formulas (3.6), (3.7) [I]") and S8, on the real ball the current dependence is
\[
\mathbf B^{(j)}\bigl(X,U_k(\exp i[\dots]V^{(k)})\bigr)=G_X\bigl(\Psi^{(j,k)}(z)\restriction X\bigr),\qquad G_X(\mathbf A):=\mathbf B^{(j)}\bigl(X;\exp(i\xi\mathbf A)\mathbf U,\ \mathbf J'(\mathbf U,\mathbf J,\mathbf A)\bigr),
\]
with \(\mathbf J'=(L^{j-1}\eta)^3\mathbf J+\Delta\mathbf A-P_1\mathbf A+\mathbf F_1(\mathbf U,\mathbf A)\) ((I.3.13)) and \((\mathbf U,\mathbf J)\) the new background. The right-hand side is the analytic continuation used from here on. \(G_X\) is a function of the labels \(\mathfrak X_X=\{(x,\nu):x\in X,\ \nu\in\{\lvert\cdot\rvert,\nabla,P_1,\Delta\}\}\) (the four norms of (I.3.14); \(P_1\Psi\) is included in the calculus as one more operator of \(\mathcal O\)). Root: \(R(X)\) = the proper tiles meeting the \((K+1)\)-neighbourhood of \(X\); it is \(*\)-connected and contains every \(R_x\).

> **(Res).** For every new background \((\mathbf U,\mathbf J)\) in the domain claimed for the new terms, \(G_X\) is holomorphic and bounded by \(B_0e^{-\kappa_Bd_j(X)}\) on \(\{\lvert u_x\rvert<\varrho_x\}\), where \(u_x\) are the scale-normalized components (\(L^n\xi\lvert\mathbf A\rvert\), \((L^n\xi)^2\lvert\nabla\mathbf A\rvert\), \((L^n\xi)^3\lvert\Delta\mathbf A\rvert\), \((L^n\xi)^3\lvert P_1\mathbf A\rvert\) for \(x\) in layer \(n\)).

**The pattern additional assumption.** Reading (2.34)–(2.39): a birth-\(j\) term allows the coefficient \(1-\beta(1-2^{-(j-n)})\) at layer \(n<j\); a term created at step \(k\) is claimed on the domain with coefficient \(1-\beta(1-2^{-(k+1-n)})\). The difference is \(\ge\frac\beta22^{-(j-n)}\). The field slot is governed by \(\alpha_{1,n}\), the current slot by \(\alpha_{0,n}\). So
\[
\textbf{(Res-pat)}\qquad\varrho_x\ge\tfrac\beta2\,2^{-(j-n)}\alpha_{\wedge,n}\ \ (n<j),\qquad\varrho_x\ge\tfrac\beta2\,L^{n-j}\alpha_{\wedge,j}\ \ (n\ge j),\qquad\alpha_\wedge:=\min(\alpha_0,\alpha_1).
\]
(For \(n\ge j\) the term's domain is normalized at scale \(j\) on \(X\cap\Omega_j\), which gains \(L^{n-j}\) for a quantity normalized at scale \(n\).) That this is the intended mechanism is the p.277 quotation in S9 source input. The exact bookkeeping of \(\beta\) (including the factor \((1+\beta)\) in (3.43)) is not displayed in the source; (Res) is stated so that any other bookkeeping can be inserted.

### 6.2 Theorem ST conditional

**Theorem ST.** Assume Theorem M(4) (i.e. (W-ms), (S-struct)), the geometry of §6.1, and (Res). Let \(1\le\kappa\le\kappa_{\max}\), \(\theta\ge0\), \(\kappa_2:=\kappa-1-b_0-\theta\ge1\). Put
\[
r_T=\min\Bigl(\frac{\varepsilon_\Psi}{g_k},\ \inf_{x\in\mathfrak X_X}\frac{\varrho_x\,e^{\theta D_x}}{e\,C_1^\Psi\,g_k}\Bigr).
\]
Then for \(\lVert A_k\rVert_\infty<r_T\):
\[
\mathbf B^{(j)}\bigl(X,U_k(\cdot)\bigr)=\sum_{Y'}F_{X,Y'}(A_k),
\]
over sets \(Y'\) of proper tiles outside \(R(X)\), each \(*\)-component touching \(R(X)\) and containing a current tile; each \(F_{X,Y'}\) is holomorphic in \(A_k\) on \(\lVert A_k\rVert_\infty<r_T\) and in the new background, depends on \(A_k\) only at the current sites in the tiles of \(R(X)\cup Y'\), and
\[
\lvert F_{X,Y'}\rvert\le B_0\,e^{-\kappa_Bd_j(X)}\,e^{-(\kappa_2-1)\lvert Y'\rvert}\quad\text{uniformly in the old data;}\qquad F_{X,Y'}(0)=0\ \text{for }Y'\ne\emptyset.
\]
If \(R(X)\) contains no current tile, \(F_{X,\emptyset}=\mathbf B^{(j)}(X,U_{k+1})\) is independent of \(A_k\).

*Proof.* Theorem C with (M-loc)\((a=\kappa-1,\ R_z=\varepsilon_\Psi/g_k,\ A_x=C_1^\Psi\varepsilon_\Psi)\) from Theorem M(4), \(G=G_X\), \(R=R(X)\). \(\square\)

**Corollary (S-T) and (Loc★) for B-terms.** The current-dependent part of \(\mathbf B_k\) is \(\sum_{j,X,Y'}F_{X,Y'}\) over the records with a current tile in \(R(X)\cup Y'\); the rest is independent of \(A_k\). If \(r_T\ge(1+\theta_R)P_k\), every record satisfies (Loc★) of [Boundary estimate f] §1.2 in zero-range form on the stadium \(\mathcal S_r\), \(r=r_T-P_k\ge\theta_RP_k\): \(S_\rho\) = current sites of \(R(X)\cup Y'\), \(\sup\lvert\partial_iF_\rho\rvert\le w_\rho/r\), \(w_\rho=B_0e^{-\kappa_Bd_j(X)}e^{-(\kappa_2-1)\lvert Y'\rvert}\), uniformly in all frozen and integrated old data and in the complex new background. The bound involves neither the volume, nor the age \(k-j\), nor any hidden distance. By the Schwarz lemma also \(\lvert F_{X,Y'}(z)\rvert\le w_\rho\lVert z\rVert_\infty/r_T\) for \(Y'\ne\emptyset\).

This is statement (S-T) of [Boundary estimate f] §3.2 for the boundary terms, in a multiscale record format (hull \(R(X)\cup Y'\) in proper tiles) rather than with \(Y\in\mathbf D_k\). Resumming to \(\mathbf D_k\) is possible but loses nothing that (Loc★) needs.

**Scope.** Only the terms \(\mathbf B^{(j)}\). For \(\mathbf E^{(j)}\), \(\mathbf R^{(j)}\) the same theorem applies to the pieces with \(X\cap(\tilde\square^2)^c\ne\emptyset\) ((I.3.5), first case); the "fundamental case" needs the renormalization cancellations of [I] §§3–5 before localization and is not treated. The fluctuation action \(\mathbf P^{(k)}\) and the quadratic form are not treated.

### 6.3 The radius and (R) conditional

**Proposition R.** Assume (Res-pat), \(\theta\ge2\), \(L\ge2\), and \(\alpha_{\wedge,k}/\alpha_{\wedge,n}\le C_{AF}\sqrt{1+k-n}\) for \(n\le k\) (asymptotic freedom; [Boundary estimate f] §4.2). Then
\[
r_T\ \ge\ \min\Bigl(\frac{\varepsilon_\Psi}{g_k},\ \frac{\beta\,\alpha_{\wedge,k}}{c_\star\,g_k}\Bigr),\qquad c_\star=4\sqrt2\,e\,C_{AF}\,C_1^\Psi.
\]
*Proof.* For \(x\) in layer \(n<j\): \(\varrho_xe^{\theta D_x}\ge\frac\beta2\alpha_{\wedge,k}\cdot2^{-(j-n)}e^{\theta(k-n-1)_+}/(C_{AF}\sqrt{1+k-n})\). With \(m=k-n\ge j-n\) the last factor is \(\ge2^{-m}e^{\theta(m-1)_+}/(C_{AF}\sqrt{1+m})\), which for \(\theta\ge2\) is minimal at \(m=1\): \(1/(2\sqrt2C_{AF})\). For \(n\ge j\): \(L^{n-j}e^{\theta(k-n-1)_+}/(C_{AF}\sqrt{1+k-j})\ge1/(2\sqrt2C_{AF})\) as well (at \(n=k\): \(L^{k-j}/\sqrt{1+k-j}\ge1\); for \(n<k\): \(\min(L,e^\theta)^{k-j-1}/\sqrt{1+k-j}\ge1/2\)). \(\square\)

Since \(\varepsilon_\Psi\) is an absolute constant and \(\alpha_\wedge=O(g\,\mathrm{polylog})\), the second term is the minimum. With (2.28):
\[
r_T\ \ge\ \frac{\beta}{c_\star}\,\min\bigl(C_0\ell_k^{q_0},\,C_1\ell_k^{q_1}\bigr).
\]
**Consequences.**
1. **(3.43) is true with the radius \(r_T\)**, i.e. with "\(C_1p_1(g_k)\)" read as \((\beta/c_\star)\min(C_0\ell_k^{q_0},C_1\ell_k^{q_1})\). This agrees in form with the source's own small-field formula: [II] (1.22) gives the radius \(\alpha_2/(8B_0C_1e^{16\kappa_1}g_k)\), and here \(\alpha_2\leftrightarrow\frac\beta2\alpha_{\wedge,k}\). The constant symbol \(C_1\) of (3.43) is plausibly that of (2.28), as [Boundary estimate f] observed, but the true radius carries the small factor \(\beta/c_\star\) (\(c_\star\propto e^{2\cdot2^d\kappa}\)).
2. **(R)**, i.e. \(r_T\ge(1+\theta_R)A_1\ell_k^{p_0}\), follows from this lower bound for all small \(g_k\) **iff** \(\min(q_0,q_1)>p_0\), or \(\min(q_0,q_1)=p_0\) and the constant(s) \(C_i\) with \(q_i=p_0\) satisfy \(C_i\ge(1+\theta_R)c_\star A_1/\beta\). Sufficiency is conditional; necessity holds on *this* route (the composition must stay in the domain at the edge of the real support for the deformed functions, exactly as in [II] (1.22)).
3. **The constraint \(q_0\ge p_0\) is forced by the source independently:** the real background has \(\lvert U_{k+1}(\partial p)-1\rvert\) of size \(2B_3L^2(1+\beta_0)\varepsilon_k\) in its own units ((3.12)), and must lie in the real slot (2.34) of every term evaluated on it, so \(2B_3L^2(1+\beta_0)A_0\ell^{p_0}\lesssim(1-\beta)C_0\ell^{q_0}\). (source input; deduction.) The constraint on \(q_1\) is not forced by definedness at real points; it is forced by the T-step localization.
4. **Compatibility additional assumption.** A consistent choice is \(q_0=q_1=p_0\) (or larger), \(C_1=(1+\theta_R)c_\star A_1/\beta\), \(C_0\ge\max(B_3C_1,\ cB_3L^2A_0)\) (the first for "\(B_3\alpha_1<\alpha_0\)", [V] Theorem 1). Every smallness condition the source states in [III]/LFR is of the form \(g\cdot\mathrm{polylog}\ll1\) and tolerates this. LFR I's "\(p_1<p_0\)" concerns the primed threshold \(\delta'_j\), not \(\alpha_1\). The cited estimate is taken as a hypothesis. 

So (R) is no longer a reading of \(p_1\). It is a derived inequality whose only free inputs are the constants \((q_0,q_1,C_0,C_1)\) of (2.28), which must be **recorded as a parameter constraint of the construction** (as \(q>p_0\) already is in [U17] AD17.15), together with the bookkeeping assumption (Res-pat).

**Remark (the "additional factor \(O(\varepsilon_k)\)").** [III] p.277 claims this factor for the localized B-terms. On the (2.28) domain Cauchy/Schwarz gives the factor \(\lVert A_k\rVert/r_T\le c_\star\delta_k/(\beta\alpha_{\wedge,k})=O(\ell_k^{p_0-\min q})\): bounded by \((1+\theta_R)^{-1}\), or a negative power of the logarithm, but not \(O(\varepsilon_k)=O(g_k\ell_k^{p_0})\). The claim would follow if the analyticity radius in \(\mathbf A\) were \(O(1)\), as in [I] (where \(\alpha_0,\alpha_1\) are absolute constants), not with (2.28). This does not affect (Loc★) as [Boundary estimate f] uses it (budget \(\mathfrak S/r^2\)), but T-step B-records are \(O(1)\cdot B_0e^{-\kappa d}\), not small. additional assumption

## 8. Resummation at a fixed carrier, and the count 𝔑

### 8.1 Record format handed to (M2)

At step \(k\) the current-dependent B-records are \(\rho=(j,X,Y')\):
- birth \(j\le k\) of the *source* term; \(X\in\mathbf D_j\) a union of \(\pi_j\)-cubes, \(\lvert X\rvert_j\) their number;
- root \(R(X)\): the proper tiles of \(\mathcal T^{(k)}\) meeting the neighbourhood of \(X\) (in layers \(n<j\) it contains \(\sim L^{d(j-n)}\) tiles per cube; it is never counted);
- \(Y'\): a set of proper tiles outside \(R(X)\), every \(*\)-component touching \(R(X)\) and containing a current tile;
- hull \(N_\rho=R(X)\cup Y'\); current support \(S_\rho\) = current sites in \(N_\rho\); zero range;
- weight \(w_\rho\le W_je^{-\kappa_B\lvert X\rvert_j}e^{-b\lvert Y'\rvert}\), \(b=\kappa_2-1\) (using \(d_j(X)\ge c(\lvert X\rvert_j-1)\)).

\[
\mathfrak N(\vartheta):=\sup_{q\in\mathcal T_{\rm cur}}\ \sum_{\rho:\ q\in N_\rho}w_\rho\,e^{\vartheta\lvert Y'\rvert}.
\]
Differences from the format (MS) of [Boundary estimate e] §5.3: the weight is per proper tile only on \(Y'\); on the root it is per \(\pi_j\)-cube of \(X\) ((MS-b) fails on the root and is not needed); all records have current birth; hull tiles have all scales \(\le k\).

### 8.2 Proposition N (deduction; given the premises)

Premises: the tiling lemmas T1–T3 of [Boundary estimate e] for \(\mathcal T^{(k)}\);
- **(Lay)** \(\operatorname{dist}_\infty(U_{m+1},\overline{\mathbb R^d\setminus U_m})\ge R\,s_m\) with \(R\ge1\) ([III] p.256 via [Boundary estimate e] G2: \(2MR_j\); (c) there);
- **(Anc)** every birth-\(j\) carrier \(X\) contains a \(\pi_j\)-cube not contained in \(U_{j+2}\) ((2.41): \(X\cap Z_j^\sim\ne\emptyset\), p.261; \(\Omega_{j+1}\) is built at distance \(\ge2LMR\) from \(Z_j\), (3.5) and p.248; source input; additional assumption);
- at most \(m_0\) records share \((j,X,Y')\); the number of connected \(X\ni Q\) with \(\lvert X\rvert_j=\ell\) is \(\le c_\pi^\ell\).

**Proposition N.** Let \(b''=b-\vartheta-2\log\Delta_*\ge(d-1)\log L+\log2\) and \(\kappa_B\ge\kappa_N\) (it suffices that \(\kappa_B-\log c_\pi-6c_d\Delta_*^{-2}e^{-b''}\ge1\)). Then \(\mathfrak N(\vartheta)\le C_{\mathfrak N}\,m_0\sup_{j\le k}W_j\), with \(C_{\mathfrak N}\) depending on \(d,L,R,c_\pi,\Delta_*\) only — not on \(k\), the volume, the sequence or the history.

*Proof.* (1) *Sum over \(Y'\) at fixed \(X\).* \(Y'\) is a disjoint, mutually non-touching union of clusters from \(\mathcal C(X)\) = \(*\)-connected sets outside \(R(X)\), touching \(R(X)\), containing a current tile. Put \(\Xi(X)=\sum_{C\in\mathcal C(X)}e^{-(b-\vartheta)\lvert C\rvert}\). A cluster containing a boundary tile \(u\) of scale \(n\) and a current tile has \(\ge k-n+1\) tiles (T3), so its total weight is \(\le\sum_{m\ge k-n+1}\Delta_*^{2(m-1)}e^{-(b-\vartheta)m}\le2\Delta_*^{-2}e^{-b''(k-n+1)}\). The number of boundary tiles of scale \(n\) is \(\le c_d\lvert X\rvert_jL^{(d-1)(j-n)_+}\). Hence
\[
\Xi(X)\le2c_d\Delta_*^{-2}\lvert X\rvert_j\Bigl[\sum_{n<j}(L^{d-1}e^{-b''})^{j-n}e^{-b''(k-j+1)}+\sum_{j\le n\le k}e^{-b''(k-n+1)}\Bigr]\le\epsilon_\Xi\lvert X\rvert_j,\qquad\epsilon_\Xi=6c_d\Delta_*^{-2}e^{-b''}.
\]
**This is where the fine multiplicity of the root boundary is paid: by the layers between it and the current region.** Then \(\sum_{Y'}e^{-(b-\vartheta)\lvert Y'\rvert}\le e^{\Xi(X)}\), and with the constraint \(q\in Y'\): \(\le e^{\Xi(X)}\sum_{C\in\mathcal C(X),\,C\ni q}e^{-(b-\vartheta)\lvert C\rvert}\).

(2) *Sum over \(X\).* It remains to bound, for \(\kappa'=\kappa_B-\epsilon_\Xi\),
\[
\sum_{j\le k}W_j\Bigl[\sum_{X:\ q\in R(X)}e^{-\kappa'\lvert X\rvert_j}+\sum_{C\ni q}e^{-(b-\vartheta)\lvert C\rvert}\sum_{X:\ R(X)\text{ touches }C}e^{-\kappa'\lvert X\rvert_j}\Bigr].
\]
If \(R(X)\) touches a tile \(u\in C\) of scale \(n\), then \(X\) has a \(\pi_j\)-cube \(Q\) within two tiles of \(u\) (a tile \(r\in R(X)\) touches \(u\), has scale \(\ge n-1\), and meets the neighbourhood of \(Q\)); in particular \(Q\) meets \(U_{n-2}\) (Lemma G1). The number of such \(Q\) is \(\le c_d'\) if \(n\le j\) and \(\le c_d'L^{d(n-j)}\) if \(n>j\). For \(n=j+p\), \(p\ge5\): by (Anc) the connected set \(X\) joins a point of \(U_{n-2}\) to a point outside \(U_{j+2}\), and by (Lay) these are at \(\infty\)-distance \(\ge\sum_{m=j+2}^{n-3}Rs_m\ge Rs_{n-3}\), so \(\lvert X\rvert_j\ge RL^{p-3}\). With \(\kappa''=\kappa'-\log c_\pi\ge1\),
\[
\mu_j(n):=\#\{Q\}\cdot\sup_Q\sum_{X\ni Q}e^{-\kappa'\lvert X\rvert_j}\ \le\ \begin{cases}c_3,&n\le j+4,\\2c_d'\,L^{dp}e^{-\kappa''RL^{p-3}}=:c_p,&n=j+p,\ p\ge5,\end{cases}
\]
and \(\sum_pc_p<\infty\): the factor \(L^{d(n-j)}\) is beaten super-exponentially. **This is where the fine multiplicity of carriers inside a coarse tile is paid: by the length of the carrier itself.**

(3) *Sum over \(j\).* The second term is \(\le\sum_jW_j\sum_{C\ni q}e^{-(b-\vartheta)\lvert C\rvert}\sum_{u\in C}\mu_j(\sigma(u))\). A cluster containing \(q\) (scale \(k\)) and a tile of scale \(n\) has \(\ge k-n+1\) tiles, so \(\sum_{C\ni q,\ C\ni\text{scale }n}\lvert C\rvert e^{-(b-\vartheta)\lvert C\rvert}\le c_2e^{-\frac12b''(k-n)}\). Hence the second term is \(\le c_2\sup_jW_j\sum_{j\le k}\sum_{n\le k}\mu_j(n)e^{-\frac12b''(k-n)}\). For \(n\le j+4\) there are at most \(k-n+5\) values of \(j\) for each \(n\), and \(\sum_n(k-n+5)e^{-\frac12b''(k-n)}<\infty\). For \(n=j+p\), \(p\ge5\): \(\sum_pc_p\sum_{j\le k-p}e^{-\frac12b''(k-j-p)}<\infty\). The first term (\(q\in R(X)\)) is the case \(n=k\) of the same count: \(\sum_j\mu_j(k)\le5c_3+\sum_pc_p\). \(\square\)

**Remarks for (M2).** (i) The statement is single-birth in the sense of [Boundary estimate f] §3.4 (all records are created at step \(k\)), but the source births \(j\) are summed; the sum converges by tile crossing and carrier length, without (Geo). (ii) Two variants fail: with Theorem D instead of D′ the count is not uniform (factor \(\exp(\epsilon L^{(d-1)(j-n)})\) from clusters at the fine boundary of \(X\)); and with the \(j\)-floored or the uniform tiling in place of the proper one (then Lemma RE gives decay only in the number of *coarse* tiles, \(e^{-\theta(k-j-1)}\) at every layer \(n<j\), which does not beat the reserve \(2^{-(j-n)}\) of (Res-pat) — the *domain* condition can no longer be verified; the count is not the issue). (iii) After the cluster expansion and the R step the format changes; that propagation is the open construction (MS) of [Boundary estimate e] and is not addressed here. (iv) Prop. Z of [Boundary estimate f] applies with \(\operatorname{diam}_Y\le M(\lvert Y'\rvert+c\lvert X\rvert_j)\) in current units only for the part of the hull in \(U_k\); the current support \(S_\rho\) lies there.
