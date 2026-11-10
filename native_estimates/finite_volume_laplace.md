# A finite-volume Laplace estimate for the Wilson integral

The positive-trace comparison holds on intermediate rectangular Wilson tori. A thermal-to-vacuum comparison for polynomial insertions also requires the [marked-insertion condition](transfer_normalization.md). The Laplace estimate concerns $\beta\ge\beta_*m^{C_0}$ and gives no bound on a physically matched sequence with fixed terminal coupling.

**Scope.** The calculations below give a proposed proof in the very weak-coupling range. The physical matched-coupling estimate is not asserted.

## 1. Setting and statements

**Lattice.** \(\Lambda_m=(\mathbb Z/m\mathbb Z)^4\), \(m\ge2\), coordinates \(x_\mu\in\{0,\dots,m-1\}\). Links \((x,\mu)\), set \(E\), \(\lvert E\rvert=4m^4\). Plaquettes \((x;\mu,\nu)\), \(\mu<\nu\), \(6m^4\) of them, with
\[
U_p=U_{x,\mu}\,U_{x+\mu,\nu}\,U_{x+\nu,\mu}^{-1}\,U_{x,\nu}^{-1}.
\]

**Group.** \(G=SU(N)\), \(\mathfrak g=\mathfrak{su}(N)\) with \(\langle X,Y\rangle=-\operatorname{tr}XY\) and norm \(\lvert X\rvert\) (Hilbert–Schmidt). \(\lVert\cdot\rVert\) is the Hilbert–Schmidt norm on matrices. Haar measure \(dU\) has mass one. \(c_N:=1/\operatorname{vol}(G)\), the volume taken in the bi-invariant metric defined by \(\langle\cdot,\cdot\rangle\).

**Action and partition function.**
\[
s(g)=N-\operatorname{Re}\operatorname{tr}g=\tfrac12\lVert g-1\rVert^2,\qquad S(U)=\sum_ps(U_p),\qquad Z_m(\beta)=\int\prod_{\ell\in E}dU_\ell\;e^{-\beta S(U)}.
\]
This is \(Z^W_{\rm cube}(m)\) of `Periodic transfer states and a finite-volume criterion` §2.1 and the Wilson weight of Annex M (1.1).

**Scalar Laplacian.** \(\Delta_m=d_0^*d_0\) on functions on \(\Lambda_m\), eigenvalues \(\lambda(k)=\sum_\mu4\sin^2(k_\mu/2)\), \(k\in\frac{2\pi}m\mathbb Z_m^4\). \(\det{}'\) omits the zero eigenvalue. \(e_4=\int_{[-\pi,\pi]^4}\log\lambda(p)\,\frac{d^4p}{(2\pi)^4}\).

**Bulk value.**
\[
\mathfrak B_m(\beta):=c_N^{\,3m^4}\Big(\frac{2\pi}\beta\Big)^{3m^4d_G/2}\big(\det{}'\Delta_m\big)^{-d_G}.
\]

**Theorem W (a; uses source input for \(N\ge3\)).** Fix \(N\ge2\). There are \(C_0,\beta_*,C_U,C_L\), depending only on \(N\), such that for all \(m\ge2\) and \(\beta\ge\beta_*m^{C_0}\):
\[
-\frac{d_G}2\log\beta+10d_G\log m-C_L\ \le\ \log Z_m(\beta)-\log\mathfrak B_m(\beta)\ \le\ \frac{3d_G}2\log\beta+17d_G\log m+C_U.
\]

**Corollary W′ (Lemma (W) as posed).** With \(p(\beta):=3\log c_N+\frac{3d_G}2\log\frac{2\pi}\beta-d_Ge_4\) and the same range of \(m,\beta\),
\[
-\frac{d_G}2\log\beta-C\ \le\ \log Z_m(\beta)-m^4p(\beta)\ \le\ \frac{3d_G}2\log\beta+15d_G\log m+C.
\]

**Theorem Φ.** For integers \(L\ge2\), \(m\ge2\) and \(\beta\ge\beta_*(Lm)^{C_0}\),
\[
0\le\Phi:=L^4\log Z_m(\beta)-\log Z_{Lm}(\beta)\le\frac{(3L^4+1)d_G}2\log\beta+17d_GL^4\log m+CL^4.
\]

Remarks.
- The true exponents are known heuristically: \(Z_m\asymp\mathfrak B_m\,\beta^{\max\{d_G/2,\,3(N-1)/2\}}\) up to powers of \(m\), with an extra \(\log\beta\) for \(N=2\) where the two strata tie (§12). The theorem brackets this between \(\beta^{-d_G/2}\) and \(\beta^{3d_G/2}\). Nothing sharper is needed for E-05.
- The exponents of \(m\) and the threshold \(C_0\) are not optimized.

## 2. Three elementary tools

### 2.1 Haar measure in an exponential chart (source input; standard)

For \(U_0\in G\) the map \(A\mapsto e^AU_0\) is injective on \(\{A\in\mathfrak g:\lVert A\rVert_{\rm op}<\pi\}\), and there
\[
dU=c_N\,j(A)\,dA,\qquad j(A)=\prod_{1\le a<b\le N}\Big(\frac{\sin\frac{\theta_a-\theta_b}2}{\frac{\theta_a-\theta_b}2}\Big)^2,
\]
where \(i\theta_a\) are the eigenvalues of \(A\) and \(dA\) is Lebesgue measure in \(\langle\cdot,\cdot\rangle\)-orthonormal coordinates. (This is the Jacobian \(\lvert\det\frac{1-e^{-\operatorname{ad}A}}{\operatorname{ad}A}\rvert\); the same formula is derived in TS20.6.) Hence
\[
0<j(A)\le1,\qquad j(A)\ge1-\tfrac N{12}\lvert A\rvert^2.
\tag{2.1}
\]
The lower bound uses \((\sin x/x)^2\ge1-x^2/3\) and \(\sum_{a<b}(\theta_a-\theta_b)^2=N\sum_a\theta_a^2=N\lvert A\rvert^2\) for traceless \(A\).

Also, for \(\lVert A\rVert_{\rm op}\le\pi\),
\[
\tfrac2\pi\lvert A\rvert\le\lVert e^A-1\rVert\le\lvert A\rvert ,
\tag{2.2}
\]
because \(\lvert e^{i\theta}-1\rvert=2\lvert\sin(\theta/2)\rvert\in[\frac2\pi\lvert\theta\rvert,\lvert\theta\rvert]\) for \(\lvert\theta\rvert\le\pi\). Finally \(\lVert ab-1\rVert\le\lVert a-1\rVert+\lVert b-1\rVert\) for unitary \(a,b\).

### 2.2 Taylor expansion of one plaquette

Let \(U_1,\dots,U_4\in G\), \(c:=U_1U_2U_3^{-1}U_4^{-1}\), and for \(A=(A_1,\dots,A_4)\in\mathfrak g^4\)
\[
F(A):=s\big(e^{A_1}U_1\,e^{A_2}U_2\,(e^{A_3}U_3)^{-1}(e^{A_4}U_4)^{-1}\big).
\]
Put \(B_1=A_1\), \(B_2=\operatorname{Ad}(U_1)A_2\), \(B_3=\operatorname{Ad}(U_1U_2U_3^{-1})A_3\), \(B_4=\operatorname{Ad}(c)A_4\) and
\[
X:=B_1+B_2-B_3-B_4,\qquad a:=\sum_i\lvert A_i\rvert.
\]
Then the argument of \(s\) is \(e^{B_1}e^{B_2}e^{-B_3}e^{-B_4}c\), and:

**Lemma 2.1.**
1. \(F(A)=s(c)-\operatorname{Re}\operatorname{tr}\big(X(c-1)\big)+\tfrac12\lvert X\rvert^2-\operatorname{Re}\operatorname{tr}\big((\tfrac12X^2+Y)(c-1)\big)+R(A)\), where \(Y=\tfrac12\sum_{i<j}\pm[B_i,B_j]\) is the second-order Baker–Campbell–Hausdorff term, \(\lvert Y\rvert\le a^2/2\).
2. \(\lvert R(A)\rvert\le\frac N6a^3\le\frac{8N}3\sum_i\lvert A_i\rvert^3\) for **all** \(A\in\mathfrak g^4\).
3. In particular, if \(c=1\): \(F(A)=\tfrac12\lvert X\rvert^2+R(A)\).

*Proof.* Expand \(e^{tB_1}e^{tB_2}e^{-tB_3}e^{-tB_4}=1+tX+t^2(\tfrac12X^2+Y)+O(t^3)\). Since \(\operatorname{tr}X=\operatorname{tr}Y=0\) and \(-\operatorname{tr}X^2=\lvert X\rvert^2\), item 1 is the second-order Taylor polynomial of \(t\mapsto F(tA)\) at \(t=1\). For item 2: for anti-Hermitian \(P,Q\), Duhamel's formula gives \(\frac{d^k}{dt^k}e^{P+tQ}=k!\int_{\Delta_k}e^{s_0(P+tQ)}Q\cdots Qe^{s_k(P+tQ)}ds\), so its operator norm is at most \(\lVert Q\rVert_{\rm op}^k\). By Leibniz the third \(t\)-derivative of the product of the four exponentials has operator norm at most \((\sum_i\lVert A_i\rVert_{\rm op})^3\le a^3\), and \(\lvert\operatorname{tr}M\rvert\le N\lVert M\rVert_{\rm op}\). Finally \((\sum_{i=1}^4a_i)^3\le16\sum a_i^3\). \(\square\)

### 2.3 Tree gauge (source input; standard)

**Lemma 2.2.** Let \(\mathcal T\subset E\) be a spanning tree of the graph \((\Lambda_m,E)\) and \(f\) a continuous gauge-invariant function on \(G^E\). Then \(\int f\prod_EdU=\int f\vert_{U_{\mathcal T}=1}\prod_{E\setminus\mathcal T}dU\).

*Proof.* For fixed \(U_{\mathcal T}\) there is a gauge transformation \(g=g(U_{\mathcal T})\) with \((U^g)_{\mathcal T}=1\). On each non-tree link \(U\mapsto U^g\) is a left and right translation, so it preserves the product Haar measure on \(G^{E\setminus\mathcal T}\). Hence \(\int f(U)\prod_{E\setminus\mathcal T}dU=\int f(1_{\mathcal T},U')\prod_{E\setminus\mathcal T}dU'\) for every \(U_{\mathcal T}\); integrate over \(U_{\mathcal T}\). \(\square\)

## 3. The comb gauge and the fibres over the holonomy links

**Definitions.**
- A link \((x,\mu)\) is a **box link** if \(x_\mu\le m-2\) and **\(\mu\)-wrapping** if \(x_\mu=m-1\).
- A plaquette \((x;\mu,\nu)\) is a **box plaquette** if \(x_\mu,x_\nu\le m-2\), **doubly wrapping** if \(x_\mu=x_\nu=m-1\) (\(6m^2\) of these), and **singly wrapping** otherwise.
- **Comb tree** \(\mathcal T:=\{(x,\mu):x_\mu\le m-2,\ x_\nu=0\ \text{for all }\nu<\mu\}\). It is a spanning tree with \(m^4-1\) box links.
- **Holonomy links** \(\ell_\mu:=((m-1)e_\mu,\mu)\), \(\mu=0,\dots,3\). They are wrapping and not in \(\mathcal T\).
- \(E':=E\setminus(\mathcal T\cup\{\ell_0,\dots,\ell_3\})\), \(n:=\lvert E'\rvert=3m^4-3\).

By Lemma 2.2,
\[
Z_m(\beta)=\int_{G^4}dh\;I(h),\qquad I(h):=\int\prod_{\ell\in E'}dU_\ell\;e^{-\beta S(U)}\Big\vert_{U_{\mathcal T}=1,\ U_{\ell_\mu}=h_\mu}.
\tag{3.1}
\]

**Reference configuration.** For \(h\in G^4\) let \(U^h_\ell:=1\) on box links and \(U^h_\ell:=h_\mu\) on every \(\mu\)-wrapping link. It lies in the fibre of (3.1). Its plaquettes are
\[
U^h_p=1\ \ (\text{box and singly wrapping}),\qquad U^h_p=c_{\mu\nu}(h):=h_\mu h_\nu h_\mu^{-1}h_\nu^{-1}\ \ (\text{doubly wrapping}).
\tag{3.2}
\]
(For a singly wrapping plaquette the two parallel wrapping links contribute \(h_\mu\cdots h_\mu^{-1}\) and the other two links are box links.) So \(U^h\) is flat exactly when the \(h_\mu\) commute, and otherwise all its curvature sits on the \(6m^2\) doubly wrapping plaquettes.

**Lemma 3.1 (small action forces the configuration to its reference point).** Let \(U\) satisfy \(U_{\mathcal T}=1\), \(U_{\ell_\mu}=h_\mu\) and \(S(U)\le\delta\). Then
1. \(\lVert U_\ell-1\rVert\le3m\sqrt{2\delta}\) for every box link;
2. \(\lVert U_\ell-h_\mu\rVert\le21m^2\sqrt{2\delta}\) for every \(\mu\)-wrapping link;
3. \(\lVert c_{\mu\nu}(h)-1\rVert\le\varepsilon_c:=85m^2\sqrt{2\delta}\) for all \(\mu<\nu\).

*Proof.* Each plaquette has \(\lVert U_p-1\rVert\le\sqrt{2\delta}\).

*Item 1.* Direction-0 box links are in \(\mathcal T\). For a box link \((x,\mu)\), \(\mu\ge1\), lower the coordinates \(x_0,x_1,\dots,x_{\mu-1}\) to zero one unit at a time, in this order. A step from \(y+e_\nu\) to \(y\) (\(\nu<\mu\), \(y_{\nu'}=0\) for \(\nu'<\nu\), \(y_\nu\le m-2\)) uses the plaquette \(p=(y;\nu,\mu)\): its links \((y,\nu)\) and \((y+e_\mu,\nu)\) are in \(\mathcal T\), so \(U_p=U_{y+e_\nu,\mu}U_{y,\mu}^{-1}\), i.e. \(U_{y+e_\nu,\mu}=U_pU_{y,\mu}\). After at most \(3(m-1)\) steps one reaches a link of \(\mathcal T\). Hence \(U_{x,\mu}\) is an ordered product of at most \(3m\) plaquette variables.

*Item 2.* Let \(y_\mu=m-1\) and \(\nu\ne\mu\) with \(y_\nu\le m-2\). The plaquette spanned by \(y,\mu,\nu\) is singly wrapping; its two \(\nu\)-links \((y,\nu)\) and \((y+e_\mu,\nu)\) are box links. Solving the plaquette relation for \(U_{y+e_\nu,\mu}\) gives
\(\lVert U_{y+e_\nu,\mu}-U_{y,\mu}\rVert\le\lVert U_p-1\rVert+\lVert U_{y,\nu}-1\rVert+\lVert U_{y+e_\mu,\nu}-1\rVert\le(1+6m)\sqrt{2\delta}\).
Any \(x\) with \(x_\mu=m-1\) is reached from \((m-1)e_\mu\) by at most \(3(m-1)\) such steps, and \(3m(1+6m)\le21m^2\).

*Item 3.* The doubly wrapping plaquette at \(y=(m-1)(e_\mu+e_\nu)\) has all four links wrapping, each within \(21m^2\sqrt{2\delta}\) of \(h_\mu\) or \(h_\nu\). Hence \(\lVert U_p-c_{\mu\nu}(h)\rVert\le84m^2\sqrt{2\delta}\). \(\square\)

**Chart on a fibre.** Write \(U_\ell=e^{A_\ell}U^h_\ell\), \(A=(A_\ell)_{\ell\in E'}\in\mathfrak g^{E'}\). By Lemma 3.1 and (2.2), every point of the fibre with \(S\le\delta\) has
\[
\lvert A_\ell\rvert\le\rho:=33m^2\sqrt{2\delta}\qquad(\ell\in E').
\tag{3.3}
\]
Norms on \(\mathfrak g^{E'}\): \(\lvert A\rvert^2=\sum_\ell\lvert A_\ell\rvert^2\), \(\lvert A\rvert_\infty=\max_\ell\lvert A_\ell\rvert\).

## 4. The fibre Hessian and its uniform coercivity

For \(h\in G^4\) and \(A\in\mathfrak g^{E'}\) (extended by zero to \(\mathcal T\) and the holonomy links), define on each plaquette, with \(U_i=U^h_{\ell_i}\) and Lemma 2.1's notation,
\[
(D_hA)_p:=X_p=A_1+\operatorname{Ad}(U_1)A_2-\operatorname{Ad}(U_1U_2U_3^{-1})A_3-\operatorname{Ad}(U^h_p)A_4,\qquad H_0(h):=D_h^*D_h.
\]
Summing Lemma 2.1 over plaquettes and using (3.2):
\[
S(e^AU^h)=S(U^h)+\langle g_h,A\rangle+\tfrac12\langle A,H(h)A\rangle+R_3(A),\qquad H(h)=H_0(h)+E(h),
\tag{4.1}
\]
where \(g_h\) and \(E(h)\) come only from the doubly wrapping plaquettes. Each link lies in six plaquettes, so:

**Lemma 4.2.** With \(\varepsilon:=\max_{\mu<\nu}\lVert c_{\mu\nu}(h)-1\rVert\):
1. \(\lvert R_3(A)\rvert\le16N\sum_\ell\lvert A_\ell\rvert^3\) for all \(A\);
2. \(\lvert g_h\rvert\le12m\,\varepsilon\);
3. \(\lVert E(h)\rVert_{\rm op}\le48\,\varepsilon\);
4. \(\lVert D_h\rVert_{\rm op}\le5\), and \(\lVert H_0(h)-H_0(h')\rVert_{\rm op}\le400\max_\mu\lVert h_\mu-h'_\mu\rVert\).

*Proof.* (1) is Lemma 2.1(2) summed. (2): \(\lvert\langle g_h,A\rangle\rvert\le\varepsilon\sum_{p\,{\rm d.w.}}\sum_{i\in p}\lvert A_i\rvert\le\varepsilon(24m^2)^{1/2}(6\lvert A\rvert^2)^{1/2}\). (3): the quadratic term from a doubly wrapping plaquette is \(-2\operatorname{Re}\operatorname{tr}((\frac12X^2+Y)(c-1))\), bounded by \(2a^2\varepsilon\le8\varepsilon\sum_{i\in p}\lvert A_i\rvert^2\). (4): \(\lvert X_p\rvert^2\le4\sum_{i\in p}\lvert A_i\rvert^2\) gives \(\lVert D_h\rVert^2\le24\). The \(\operatorname{Ad}\) factors in \(X_p\) are words of length at most four in the \(h_\mu^{\pm1}\), and \(\lVert\operatorname{Ad}(u)-\operatorname{Ad}(u')\rVert\le2\lVert u-u'\rVert\). So \(\lvert(D_hA-D_{h'}A)_p\rvert\le8\eta\sum_{i\in p}\lvert A_i\rvert\) with \(\eta=\max\lVert h_\mu-h'_\mu\rVert\), hence \(\lVert D_h-D_{h'}\rVert\le40\eta\) and \(\lVert D_h^*D_h-D_{h'}^*D_{h'}\rVert\le2\cdot5\cdot40\,\eta\). \(\square\)

**Lemma 4.1 (uniform coercivity on the fibre).** For every \(h\in G^4\) — commuting or not — and every \(A\in\mathfrak g^{E'}\),
\[
\lvert D_hA\rvert^2\ \ge\ \frac1{600\,m^7}\,\lvert A\rvert^2.
\]
The same holds, with the same proof, for the scalar twisted operator \(d_1^\varphi\) of §5 on \(F_0\).

*Proof.* This is the linearization of Lemma 3.1. Let \(\tau:=\lvert D_hA\rvert\).

*Box links.* On box plaquettes \(U^h\equiv1\), so \(X_p=(dA)_p\) is the ordinary lattice curl. Following the path in the proof of Lemma 3.1(1), with \(A_{\mathcal T}=0\): \(A_{y+e_\nu,\mu}=A_{y,\mu}\pm X_p\) at each step. Hence \(A_\ell\) is a signed sum of at most \(3m\) curls, and \(\lvert A_\ell\rvert\le(3m)^{1/2}\tau\).

*Wrapping links.* For a singly wrapping plaquette spanned by \(y,\mu,\nu\) (\(y_\mu=m-1\), \(y_\nu\le m-2\)), (3.2) and the definition give \(X_p=\pm\big(A_{y,\mu}-A_{y+e_\nu,\mu}+\operatorname{Ad}(h_\mu)A_{y+e_\mu,\nu}\big)\mp A_{y,\nu}\), so
\(\lvert A_{y+e_\nu,\mu}-A_{y,\mu}\rvert\le\lvert X_p\rvert+2(3m)^{1/2}\tau\).
Start at the holonomy link, where \(A=0\), and take at most \(3m\) steps: \(\lvert A_{x,\mu}\rvert\le(3m)^{1/2}\tau+6m(3m)^{1/2}\tau\le7m(3m)^{1/2}\tau\).

Summing squares over at most \(4m^4\) links: \(\lvert A\rvert^2\le4m^4\cdot147m^3\tau^2\le600m^7\tau^2\). \(\square\)

*Why this is the key point.* Near a reducible flat connection the gauge-fixed Hessian of the Wilson action has small eigenvalues of order \(\lvert\alpha(\theta)\rvert^2/m^2\) in the charged constant modes, and at the centre it has \(4d_G\) exact zero modes. All of these modes are nonzero on the holonomy links. Freezing those four links removes them, uniformly in \(h\).

## 5. Twisted cochain complexes: a determinant bound on the fibre

### 5.1 The complex

Fix \(\varphi\in(-\pi,\pi]^4\). Let \(u(x,\mu)=e^{i\varphi_\mu}\) on \(\mu\)-wrapping links and \(u=1\) on box links. On complex cochains put
\[
(d_0\lambda)(x,\mu)=u(x,\mu)\lambda(x+\mu)-\lambda(x),
\]
\[
(d_1a)(x;\mu,\nu)=a(x,\mu)+u(x,\mu)a(x+\mu,\nu)-u(x,\nu)a(x+\nu,\mu)-a(x,\nu).
\]
Then \(d_1d_0=0\). Let \(\Delta^\varphi:=d_0^*d_0\), \(Q:=d_1^*d_1\), and \(F_0:=\{a\in C^1:a=0\text{ on }\mathcal T\cup\{\ell_\mu\}\}\), \(\dim_{\mathbb C}F_0=n=3m^4-3\). Set
\[
q_\varphi:=\det\big(Q\vert_{F_0}\big)\quad\text{(the determinant of the compression of }Q\text{ to the coordinate subspace }F_0).
\]

**Lemma 5.1 (source input; Fourier).** The gauge transformation \(\lambda\mapsto e^{-i\varphi\cdot x/m}\lambda\) makes the phases uniform, \(u\equiv e^{i\varphi_\mu/m}\). Hence \(\Delta^\varphi\) has eigenvalues \(\lambda(k+\varphi/m)\), \(k\in\frac{2\pi}m\mathbb Z_m^4\), and \(d_0d_0^*+d_1^*d_1\) acts on \(C^1\) as \(\Delta^\varphi\otimes1_4\). On \(K:=\ker d_0^*=(\operatorname{im}d_0)^\perp\) the operator \(Q\) therefore has eigenvalues \(\lambda(k+\varphi/m)\) with multiplicity three for each \(k\) with \(\lambda\ne0\), together with a four-dimensional kernel (the constants) when \(\varphi=0\).

Write \(\lambda_\flat:=\min_k\lambda(k+\varphi/m)\) and \(\det{}^\flat\Delta^\varphi:=\prod\lambda(k+\varphi/m)\) with **one** factor \(\lambda_\flat\) omitted. For \(\varphi=0\) this is \(\det{}'\Delta_m\).

Two facts about the spectrum:
- \(\lambda_\flat\le\lambda(\varphi/m)=\sum_\mu4\sin^2\frac{\varphi_\mu}{2m}\le\sum_\mu4\sin^2\frac{\varphi_\mu}2=:\lvert\varphi\rvert_\sharp^2\).
- All eigenvalues other than the omitted one are at least \(4/m^2\). (If \(\lambda(p)<4/m^2\) then every \(\lvert p_\mu\rvert<\pi/m\) mod \(2\pi\); two distinct \(k\) cannot both satisfy this.)

**Lemma 5.2 (diamagnetic bound).** For every \(\varphi\),
\[
\log\det{}^\flat\Delta^\varphi\ \ge\ \log\det{}'\Delta_m-6\log m-\log17-\tfrac14.
\]

*Proof.* \(e^{-t\Delta^\varphi}=e^{-8t}e^{t\mathsf A^\varphi}\), where the twisted adjacency matrix \(\mathsf A^\varphi\) is entrywise dominated in modulus by \(\mathsf A^0\). The power series gives \(\lvert(e^{t\mathsf A^\varphi})_{xx}\rvert\le(e^{t\mathsf A^0})_{xx}\), so \(\operatorname{Tr}e^{-t\Delta^\varphi}\le\operatorname{Tr}e^{-t\Delta^0}\). By Frullani's integral \(\log a=\int_0^\infty(e^{-t}-e^{-ta})\frac{dt}t\), for every \(\mu^2>0\)
\[
\log\det(\Delta^\varphi+\mu^2)\ \ge\ \log\det(\Delta^0+\mu^2)\ \ge\ \log\mu^2+\log\det{}'\Delta_m.
\tag{5.1}
\]
On the other hand \(\log\det{}^\flat\Delta^\varphi\ge\log\det(\Delta^\varphi+\mu^2)-\log(16+\mu^2)-\mu^2\sum^\flat\lambda^{-1}\), and \(\sum^\flat\lambda^{-1}\le m^4\cdot m^2/4\). Take \(\mu^2=m^{-6}\). \(\square\)

### 5.2 The Jacobian of the tree-and-holonomy slice

Let \(P\) be the orthogonal projection of \(C^1\) onto \(K\), \(P_F:=P\vert_{F_0}\), \(\mathcal G:=P(F_0)\subset K\).

**Lemma 5.3.** \(P_F\) is injective, \(Q(a)=\langle Pa,QPa\rangle\), and
\[
q_\varphi=\det(P_F^*P_F)\cdot\det(Q_{\mathcal G}),
\tag{5.2}
\]
where \(Q_{\mathcal G}\) is the compression of \(Q\vert_K\) to \(\mathcal G\). Moreover
\[
\det(P_F^*P_F)\ \ge\ \frac{\lvert\varphi\rvert_\sharp^2}{\det\Delta^\varphi}\ \ge\ \frac1{\det{}^\flat\Delta^\varphi}\quad(\varphi\ne0),\qquad
\det(P_F^*P_F)\ \ge\ \frac{m^4}{\det{}'\Delta_m}\quad(\varphi=0).
\tag{5.3}
\]

*Proof.* *Injectivity.* If \(d_0\lambda\in F_0\) then \(\lambda\) is constant along \(\mathcal T\) (where \(u=1\)), hence constant, and on \(\ell_\mu\) one gets \((e^{i\varphi_\mu}-1)\lambda=0\) for all \(\mu\). So \(d_0\lambda=0\). Thus \(F_0\cap\operatorname{im}d_0=0\). \(Q\) vanishes on \(\operatorname{im}d_0\), which gives \(Q(a)=Q(Pa)\) and (5.2).

*Case \(\varphi\ne0\).* Then \(d_0\) is injective. Consider \(\Psi:F_0\oplus C^0\to C^1\), \(\Psi(a,\lambda)=a+d_0\lambda\). In the orthogonal splitting \(\mathcal G\oplus\operatorname{im}d_0\) of its range it is block triangular with diagonal blocks \(P_F\) and \(d_0\), so \(\det(\Psi^*\Psi)=\det(P_F^*P_F)\det\Delta^\varphi\). In standard coordinates the columns of \(\Psi\) are the unit vectors \(e_\ell\), \(\ell\in E'\), and the vectors \(d_0\delta_x\). The Gram determinant is unchanged by projecting the latter orthogonally to the former, so \(\det(\Psi^*\Psi)=\det(M^*M)\) with \(M\) the restriction of \(d_0\) to the rows \(\mathcal T\cup\{\ell_\mu\}\). By Cauchy–Binet, \(\det(M^*M)\ge\sum_\mu\lvert\det M_{\mathcal T\cup\{\ell_\mu\}}\rvert^2\). The graph \(\mathcal T\cup\{\ell_\mu\}\) has a single cycle, with holonomy \(e^{i\varphi_\mu}\); in the coordinates (\(\lambda(0)\), differences along \(\mathcal T\)) the matrix is triangular with determinant \(\pm(e^{i\varphi_\mu}-1)\). Hence \(\det(M^*M)\ge\lvert\varphi\rvert_\sharp^2\). The second inequality in (5.3) is \(\lambda_\flat\le\lvert\varphi\rvert_\sharp^2\).

*Case \(\varphi=0\).* Replace \(C^0\) by the functions vanishing at the origin. Then \(\det(d_0^*d_0)\) on that space is the number of spanning trees, \(\det{}'\Delta_m/m^4\) (matrix-tree theorem), and \(\det(M^*M)\ge\lvert\det M_{\mathcal T}\rvert^2=1\). \(\square\)

### 5.3 The determinant bound

**Proposition 5.4.** For every \(\varphi\in(-\pi,\pi]^4\) and \(m\ge2\),
\[
q_\varphi\ \ge\ c_q\,m^{-33}\,\big(\det{}'\Delta_m\big)^2,\qquad c_q:=9600^{-4}\,(17e^{1/4})^{-2}.
\]

*Proof.* Let \(r=\operatorname{codim}_K\mathcal G\); \(r=3\) for \(\varphi\ne0\) and \(r=4\) for \(\varphi=0\). By Cauchy interlacing for compressions, \(\lambda_j(Q_{\mathcal G})\ge\lambda_j(Q\vert_K)\) (eigenvalues in increasing order). Bound the \(r\) smallest eigenvalues of \(Q_{\mathcal G}\) from below by \(\lambda_{\min}(Q_{\mathcal G})\) and the others by interlacing, and use \(\lambda\le16\):
\[
\det Q_{\mathcal G}\ \ge\ \lambda_{\min}(Q_{\mathcal G})^{\,r}\,16^{-r}\prod_{j>r}\lambda_j(Q\vert_K)=\lambda_{\min}(Q_{\mathcal G})^{\,r}\,16^{-r}\big(\det{}^\flat\Delta^\varphi\big)^3.
\]
(By Lemma 5.1 the \(r\) smallest eigenvalues of \(Q\vert_K\) are \(\lambda_\flat\) three times, resp. zero four times.) Next,
\(\lambda_{\min}(Q_{\mathcal G})=\min_{a\in F_0}Q(a)/\lvert Pa\rvert^2\ge\min_{a\in F_0}Q(a)/\lvert a\rvert^2\ge(600m^7)^{-1}\) by Lemma 4.1. With (5.2)–(5.3):
\[
q_\varphi\ge(9600m^7)^{-3}\big(\det{}^\flat\Delta^\varphi\big)^2\ \ (\varphi\ne0),\qquad q_0\ge m^4(9600m^7)^{-4}\big(\det{}'\Delta_m\big)^2.
\]
Lemma 5.2 converts \(\det{}^\flat\Delta^\varphi\) into \(\det{}'\Delta_m\) at the cost \((17e^{1/4}m^6)^{-2}\). \(\square\)

*Remark (additional assumption; numerical).* The truth is much better than the proposition: \(q_0=(\det{}'\Delta_m)^2/m^4\) exactly in the cases computed, and \(q_\varphi/(\det{}^\flat\Delta^\varphi)^2\) stays of order one, continuously in \(\varphi\) down to \(\varphi=0\).

### 5.4 The fibre Hessian at commuting holonomies

**Corollary 5.5.** Let \(h'\in G^4\) have commuting entries. Then, in \(\langle\cdot,\cdot\rangle\)-orthonormal real coordinates on \(\mathfrak g^{E'}\),
\[
\det H_0(h')\ \ge\ \Big[c_q\,m^{-33}\big(\det{}'\Delta_m\big)^2\Big]^{d_G}.
\]

*Proof.* Commuting unitaries are simultaneously diagonalizable, and a global conjugation is an orthogonal map of \(\mathfrak g^{E'}\) intertwining \(H_0(h')\) and \(H_0(gh'g^{-1})\). So let \(h'_\mu=\operatorname{diag}(e^{i\theta^1_\mu},\dots,e^{i\theta^N_\mu})\). Write \(A_\ell=\sum_ait^a_\ell e_{aa}+\sum_{a<b}(z^{ab}_\ell e_{ab}-\bar z^{ab}_\ell e_{ba})\). Since \(U^{h'}\) is flat, \(X_p=A_1+\operatorname{Ad}(U_1)A_2-\operatorname{Ad}(U_4)A_3-A_4\), and \(\operatorname{Ad}(U^{h'}_\ell)\) multiplies \(e_{ab}\) by \(e^{i(\theta^a_\mu-\theta^b_\mu)}\) on \(\mu\)-wrapping links. Therefore the \(e_{ab}\)-component of \(D_{h'}A\) is \(d_1^{\varphi^{ab}}z^{ab}\) with \(\varphi^{ab}_\mu=\theta^a_\mu-\theta^b_\mu\), the diagonal components are untwisted, and
\[
\lvert D_{h'}A\rvert^2=\sum_a\lvert d_1^0t^a\rvert^2+2\sum_{a<b}\lvert d_1^{\varphi^{ab}}z^{ab}\rvert^2.
\]
In orthonormal coordinates this is \(N-1\) real copies of \(Q^0\vert_{F_0}\) and, for each \(a<b\), the realification of the Hermitian form \(Q^{\varphi^{ab}}\vert_{F_0}\) in the variable \(\sqrt2z^{ab}\). Hence \(\det H_0(h')=q_0^{\,N-1}\prod_{a<b}q_{\varphi^{ab}}^{\,2}\), with \(N-1+N(N-1)=d_G\) factors. Apply Proposition 5.4. \(\square\)

## 6. Almost commuting tuples

Let \(\mathcal C\subset G^4\) be the set of commuting 4-tuples and \(f(h)=\sum_{\mu<\nu}\lVert c_{\mu\nu}(h)-1\rVert^2\), a real-analytic function on the compact real-analytic manifold \(G^4\) with zero set \(\mathcal C\).

**Lemma 6.1 (c; Łojasiewicz).** There are \(C_{\rm Ł}=C_{\rm Ł}(N)\ge1\) and \(\kappa=\kappa_N\in(0,1]\) such that every \(h\in G^4\) with \(\max_{\mu<\nu}\lVert c_{\mu\nu}(h)-1\rVert\le\varepsilon\le1\) has some \(h'\in\mathcal C\) with \(\max_\mu\lVert h_\mu-h'_\mu\rVert\le C_{\rm Ł}\varepsilon^\kappa\).

*Source.* S. Łojasiewicz, *Sur le problème de la division*, Studia Math. 18 (1959) 87–136 (the inequality \(\lvert f(x)\rvert\ge c\operatorname{dist}(x,f^{-1}(0))^\alpha\) on compact sets for real-analytic \(f\)); see also Bierstone–Milman, Publ. Math. IHÉS 67 (1988), Theorem 6.4. Apply it to \(f\) in finitely many analytic charts.

**Lemma 6.2 (\(SU(2)\), explicit).** For \(N=2\) one may take \(C_{\rm Ł}=\sqrt2\), \(\kappa=\tfrac12\).

*Proof.* Write \(h_\mu=c_\mu+i\,v_\mu\!\cdot\!\sigma\) with \(c_\mu^2+\lvert v_\mu\rvert^2=1\). Then \(\lVert c_{\mu\nu}(h)-1\rVert=\lVert h_\mu h_\nu-h_\nu h_\mu\rVert=2\sqrt2\,\lvert v_\mu\times v_\nu\rvert\). Let \(v_*\) be the longest of the \(v_\mu\) (if all vanish, \(h\in\mathcal C\)), \(e=v_*/\lvert v_*\rvert\), and \(h'_\mu:=c_\mu+i\,w_\mu e\!\cdot\!\sigma\) with \(w_\mu=\operatorname{sgn}(v_\mu\!\cdot\!e)\lvert v_\mu\rvert\). The \(h'_\mu\) lie in one maximal torus. With \(v_\mu^\perp\) the component of \(v_\mu\) orthogonal to \(e\):
\(\lvert v_\mu-w_\mu e\rvert^2=2\lvert v_\mu\rvert(\lvert v_\mu\rvert-\lvert v_\mu\!\cdot\!e\rvert)\le2\lvert v_\mu^\perp\rvert^2\), and \(\lvert v_\mu^\perp\rvert=\lvert v_\mu\times v_*\rvert/\lvert v_*\rvert\le\varepsilon/(2\sqrt2\lvert v_*\rvert)\). Also \(\lvert v_\mu-w_\mu e\rvert\le2\lvert v_*\rvert\). Hence \(\lvert v_\mu-w_\mu e\rvert\le\min\{\varepsilon/(2\lvert v_*\rvert),2\lvert v_*\rvert\}\le\sqrt\varepsilon\) and \(\lVert h_\mu-h'_\mu\rVert=\sqrt2\lvert v_\mu-w_\mu e\rvert\le\sqrt{2\varepsilon}\). \(\square\)

The exponent \(\tfrac12\) is sharp: near the centre, \(h_\mu=e^{X_\mu}\) with \(\lvert X_\mu\rvert\sim r\) in general position has commutators of size \(r^2\) and distance \(r\) from \(\mathcal C\).

## 7. The upper bound

**Parameters.** Fix
\[
K:=3\lvert\log c_N\rvert+\tfrac92d_G,\qquad\delta:=\frac{Km^4\log\beta}\beta,\qquad\varepsilon_c=85m^2\sqrt{2\delta},\qquad\rho=33m^2\sqrt{2\delta}.
\]
The hypothesis \(\beta\ge\beta_*m^{C_0}\), with \(C_0=\max\{73,9+22/\kappa\}\) and \(\beta_*=\beta_*(N)\) large, is used only through:

| | Condition | Needs \(\beta\) (up to logs and constants) |
|---|---|---|
| (c1) | \(48\varepsilon_c\le(1200m^7)^{-1}\) | \(\ge m^{22}\) |
| (c2) | \(48\varepsilon_c+400C_{\rm Ł}\varepsilon_c^\kappa\le(3600d_Gm^{11})^{-1}\) | \(\ge m^{8+22/\kappa}\) |
| (c3) | \(\beta\cdot16N\cdot3m^4\rho^3\le1\) | \(\ge m^{32}\) |
| (c4) | \(\beta\cdot16N(14400m^8\varepsilon_c)^3\le1\) | \(\ge m^{72}\) |

(Insert \(\varepsilon_c^2=14450Km^8\log\beta/\beta\) and \(\rho^2=2178Km^8\log\beta/\beta\). The logarithms are absorbed by the spare power of \(m\) and by \(\beta_*\).)

**Step 1 (large action).** By (3.1), \(Z_m\le\sup_hI(h)\), and \(I(h)\le e^{-\beta\delta}+I_\delta(h)\), where \(I_\delta(h)\) is the integral over \(\{S\le\delta\}\). Here \(e^{-\beta\delta}=\beta^{-Km^4}\).

**Step 2 (chart).** Fix \(h\) with \(\{S\le\delta\}\) nonempty on its fibre; otherwise \(I_\delta(h)=0\). By Lemma 3.1(3), \(\varepsilon(h)\le\varepsilon_c\). By (3.3) and §2.1, with \(j\le1\),
\[
I_\delta(h)\le c_N^{\,n}\int_{\lvert A\rvert_\infty\le\rho}e^{-\beta S(e^AU^h)}\,dA.
\]

**Step 3 (quadratic lower bound for the action).** Let \(q(A):=S(U^h)+\langle g_h,A\rangle+\frac12\langle A,H(h)A\rangle\). By (4.1) and Lemma 4.2(1), \(S\ge q-16N\cdot n\rho^3\) on the chart ball, and \(\beta\cdot16Nn\rho^3\le1\) by (c3). By Lemmas 4.1, 4.2(3) and (c1),
\[
H(h)\ \ge\ \frac1{600m^7}-48\varepsilon_c\ \ge\ \frac1{1200m^7}>0.
\]
Therefore
\[
I_\delta(h)\le e\,c_N^{\,n}\int_{\mathfrak g^{E'}}e^{-\beta q(A)}dA=e\,c_N^{\,n}\Big(\frac{2\pi}\beta\Big)^{nd_G/2}\big(\det H(h)\big)^{-1/2}e^{-\beta q_{\min}},\qquad q_{\min}=\min q=q(A_*).
\]

**Step 4 (the minimum of \(q\) is almost nonnegative).** \(A_*=-H(h)^{-1}g_h\), so by Lemma 4.2(2), \(\lvert A_*\rvert\le1200m^7\cdot12m\,\varepsilon_c=14400m^8\varepsilon_c\). Since \(S\ge0\) and Lemma 4.2(1) holds for all \(A\),
\[
q_{\min}=S(e^{A_*}U^h)-R_3(A_*)\ \ge\ -16N\lvert A_*\rvert^3,\qquad\text{so}\quad e^{-\beta q_{\min}}\le e\ \text{ by (c4).}
\]
This is the step that replaces any knowledge of the true constrained minimizer for non-commuting \(h\).

**Step 5 (the determinant).** By Lemma 6.1 (Lemma 6.2 if \(N=2\)) choose \(h'\in\mathcal C\) with \(\eta:=\max\lVert h_\mu-h'_\mu\rVert\le C_{\rm Ł}\varepsilon_c^\kappa\). By Lemma 4.2(3,4),
\(\lVert H(h)-H_0(h')\rVert\le48\varepsilon_c+400\eta=:\eta'\). Since \(H_0(h')\ge(600m^7)^{-1}\), Weyl's inequality gives \(\lambda_j(H(h))\ge\lambda_j(H_0(h'))(1-600m^7\eta')\). By (c2), \(600m^7\eta'\cdot nd_G\le\frac12\), so
\[
\det H(h)\ \ge\ e^{-1}\det H_0(h')\ \ge\ e^{-1}\Big[c_q\,m^{-33}\big(\det{}'\Delta_m\big)^2\Big]^{d_G}
\]
by Corollary 5.5.

**Step 6 (assembly).** For every \(h\),
\[
I_\delta(h)\le e^{5/2}\,c_N^{\,3m^4-3}\Big(\frac{2\pi}\beta\Big)^{(3m^4-3)d_G/2}c_q^{-d_G/2}\,m^{33d_G/2}\big(\det{}'\Delta_m\big)^{-d_G}=:\mathcal R.
\]
Since \(\det{}'\Delta_m\le16^{m^4}\) and \(\log\beta\ge1\), \(\log\mathcal R\ge-Km^4\log\beta\), i.e. \(e^{-\beta\delta}\le\mathcal R\). Hence \(Z_m\le2\mathcal R\), which is
\[
\log Z_m(\beta)\le\log\mathfrak B_m(\beta)+\frac{3d_G}2\log\beta+\frac{33d_G}2\log m+C_U,\qquad C_U=\log2+\tfrac52+3\lvert\log c_N\rvert+\tfrac{d_G}2\log\tfrac1{c_q}.
\]
This proves W-U. \(\square\)

## 8. The lower bound

Write \(M\) for the side (to match its use for the large cube) and assume \(\beta\ge\beta_*M^{41}\). Let \(W:=\{A\in\mathbb R^E:A_{\mathcal T}=0\}\), \(n_1:=\dim W=3M^4+1\). Restrict (after Lemma 2.2) to \(U_\ell=e^{A_\ell}\), \(A\in W\otimes\mathfrak g\), with every colour component in the cube \(\lvert A^a_\ell\rvert\le\rho_2\); then \(\lvert A_\ell\rvert\le\rho_1:=\sqrt{d_G}\rho_2\). Choose
\[
\rho_2:=9\sqrt2\,M^{11/2}\beta^{-1/2}.
\]

**Step 1 (nonlinear factors).** At the trivial connection Lemma 2.1(3) gives \(S(e^A)\le\frac12\lvert dA\rvert^2+16N\sum_\ell\lvert A_\ell\rvert^3\), with \(d\) the untwisted curl. By (2.1), \(\prod_\ell j(A_\ell)\ge\exp(-\frac N6n_1\rho_1^2)\). For \(\beta\ge\beta_*M^{41}\) both \(\beta\cdot16Nn_1\rho_1^3\le1\) and \(\frac N6n_1\rho_1^2\le1\). Hence
\[
Z_M(\beta)\ \ge\ c_N^{\,n_1}e^{-2}\,J^{\,d_G},\qquad J:=\int_{A\in W,\ \lvert A\rvert_\infty\le\rho_2}e^{-\frac\beta2\lvert dA\rvert^2}dA\quad(\text{real scalar }A).
\]

**Step 2 (the Gaussian integral \(J\)).** Let \(P\) be the orthogonal projection onto \(K=(\operatorname{im}d_0)^\perp=\mathcal H\oplus K_c\) (constants \(\mathcal H\), \(\dim4\); coexact forms \(K_c\), \(\dim3M^4-3\)). As in Lemma 5.3 (case \(\varphi=0\), without removing the holonomy rows), \(P:W\to K\) is a bijection with
\[
\lvert\det P\rvert=\big(M^4/\det{}'\Delta_M\big)^{1/2},\qquad\lVert P^{-1}\rVert\le9M^{5/2}.
\]
(For the norm: if \(A=B+d_0\lambda\in W\) with \(B=PA\), then \(d_0\lambda=-B\) on \(\mathcal T\), so \(\lvert\lambda(x)-\lambda(0)\rvert\le(4M)^{1/2}\lvert B\rvert\), \(\lvert d_0\lambda\rvert\le8M^{5/2}\lvert B\rvert\).) Therefore \(P(\{\lvert A\rvert_\infty\le\rho_2\})\) contains \(\{b_h+b_c:\lvert b_h\rvert\le r,\lvert b_c\rvert\le r\}\) with \(r:=\rho_2/(9\sqrt2M^{5/2})=M^3\beta^{-1/2}\), and \(\lvert dA\rvert^2=\langle b_c,Qb_c\rangle\). On \(K_c\), \(\det Q=(\det{}'\Delta_M)^3\) and \(\operatorname{Tr}Q^{-1}\le3M^4\cdot M^2/16\). By Chebyshev, the Gaussian measure with covariance \((\beta Q)^{-1}\) gives \(\{\lvert b_c\rvert\le r\}\) probability at least \(1-\frac{3M^6}{16\beta r^2}\ge\frac12\). Hence
\[
J\ \ge\ \Big(\frac{\det{}'\Delta_M}{M^4}\Big)^{1/2}\cdot\frac{\pi^2r^4}2\cdot\frac12\Big(\frac{2\pi}\beta\Big)^{(3M^4-3)/2}\big(\det{}'\Delta_M\big)^{-3/2}
=\frac{\pi^2}4\,M^{10}\beta^{-2}\Big(\frac{2\pi}\beta\Big)^{(3M^4-3)/2}\big(\det{}'\Delta_M\big)^{-1}.
\]

**Step 3 (assembly).**
\[
\log Z_M(\beta)\ \ge\ \log\mathfrak B_M(\beta)-\frac{d_G}2\log\beta+10d_G\log M-C_L,\qquad C_L=2+\lvert\log c_N\rvert+d_G\big(\tfrac32\log2\pi-\log\tfrac{\pi^2}4\big).
\]
This proves W-L. \(\square\)

## 9. The scalar determinant; proofs of Corollary W′ and Theorem Φ

**Lemma 9.1 (finite-size law, weak form).** For \(d=4\) and all \(m\ge2\),
\[
m^4e_4+2\log m-C_4\ \le\ \log\det{}'\Delta_m\ \le\ m^4e_4+4\log m+G_4(0),\qquad G_4(0)=\int\frac{d^4p}{(2\pi)^4}\frac1{\lambda(p)}<\infty.
\]

*Proof of the upper bound (Bloch waves and diamagnetism).* For \(\mu^2>0\) put \(e_4(\mu^2)=\int\log(\lambda(p)+\mu^2)\frac{d^4p}{(2\pi)^4}\). Changing variables \(p=k+\varphi/m\),
\(\int_{(-\pi,\pi]^4}\log\det(\Delta^\varphi_m+\mu^2)\frac{d^4\varphi}{(2\pi)^4}=m^4e_4(\mu^2)\) exactly. By (5.1) the integrand is at least \(\log\mu^2+\log\det{}'\Delta_m\) for every \(\varphi\). Hence \(\log\det{}'\Delta_m\le m^4e_4(\mu^2)-\log\mu^2\le m^4e_4+m^4\mu^2G_4(0)-\log\mu^2\). Take \(\mu^2=m^{-4}\).

*Proof of the lower bound (heat kernel).* Let \(p_t(x)=\prod_ie^{-2t}I_{x_i}(2t)\) be the heat kernel of \(\mathbb Z^4\) and \(\psi_m(t)=\operatorname{Tr}e^{-t\Delta_m}-m^4p_t(0)=m^4\sum_{w\ne0}p_t(mw)\ge0\). Frullani's integral gives
\[
\log\det(\Delta_m+\mu^2)=m^4e_4(\mu^2)-\int_0^\infty e^{-\mu^2t}\psi_m(t)\frac{dt}t.
\]
- \(t\le1\): \(e^{-2t}I_k(2t)\le t^{\lvert k\rvert}/\lvert k\rvert!\), so \(\psi_m(t)\le16m^4t^m/m!\) and \(\int_0^1\psi_m\frac{dt}t\le C\).
- \(1\le t\le m^2\): shifting the contour in \(e^{-2t}I_k(2t)=\frac1{2\pi}\int e^{-ik\theta-2t(1-\cos\theta)}d\theta\) to \(\theta-is\), \(s=\min(1,k/2.2t)\), and using \(e^{-x}I_0(x)\le0.63x^{-1/2}\), \(\cosh s-1\le0.55s^2\): \(e^{-2t}I_k(2t)\le t^{-1/2}\exp[-\min(k^2/4.4t,k/2)]\). Then \(\psi_m(t)\le C(m^2/t)^2\exp[-\min(m^2/4.4t,m/2)]\), whose integral against \(dt/t\) over \([1,m^2]\) is bounded.
- \(t\ge m^2\): \(\psi_m\le1+\sum_{k\ne0}e^{-t\lambda(k)}\); \(\int_{m^2}^\infty e^{-\mu^2t}\frac{dt}t\le\log(1+\frac1{\mu^2m^2})\) and \(\int_{m^2}^\infty\sum_{k\ne0}e^{-t\lambda(k)}\frac{dt}t\le\sum_{j\ne0}\frac{e^{-16\lvert j\rvert^2}}{16\lvert j\rvert^2}\), using \(\lambda(2\pi j/m)\ge16\lvert j\rvert^2/m^2\).

Hence \(\log\det(\Delta_m+\mu^2)\ge m^4e_4-C-\log(1+\frac1{\mu^2m^2})\). Finally \(\log\det{}'\Delta_m\ge\log\det(\Delta_m+\mu^2)-\log\mu^2-\mu^2\sum_{k\ne0}\lambda(k)^{-1}\) and \(\sum_{k\ne0}\lambda^{-1}\le m^6/16\). Take \(\mu^2=m^{-6}\). \(\square\)

*Remarks.* The sharp law \(\log\det{}'\Delta_m=m^4e_4+2\log m+c+o(1)\) is the main theorem of Chinta–Jorgenson–Karlsson, Nagoya Math. J. 198 (2010) 121–172 (not needed here), and is Lemma 4.3 of `Periodic transfer states and a finite-volume criterion`, whose Bessel bound is the one rederived above. Numerically \(\log\det{}'\Delta_m-m^4e_4-2\log m\in[-2.65,-1.70]\) for \(2\le m\le24\).

**Proof of Corollary W′.** Insert Lemma 9.1 into Theorem W: \(\log\mathfrak B_m=m^4p(\beta)-d_G(\log\det{}'\Delta_m-m^4e_4)\). \(\square\)

**Proof of Theorem Φ.** \(\Phi\ge0\) is Theorem 2 of `Periodic transfer states and a finite-volume criterion`. Apply W-U at side \(m\) and W-L at side \(M=Lm\); both are allowed when \(\beta\ge\beta_*(Lm)^{C_0}\). The powers of \(c_N\) and of \(2\pi/\beta\) in \(\mathfrak B\) cancel exactly because \(L^4\cdot3m^4=3(Lm)^4\), leaving
\[
\Phi\le L^4\Big[\tfrac{3d_G}2\log\beta+\tfrac{33d_G}2\log m+C_U\Big]+\tfrac{d_G}2\log\beta-10d_G\log(Lm)+C_L+d_G\big[\log\det{}'\Delta_{Lm}-L^4\log\det{}'\Delta_m\big].
\]
By Lemma 9.1 the last bracket is at most \(4\log(Lm)+G_4(0)-L^4(2\log m-C_4)\). Collecting terms gives the stated bound (indeed with \(\frac{29}2\) in place of 17). \(\square\)

## 10. Application to the B-02 family

Data from `Finite Wilson family` §§1–3 (source input; proposition B-02): odd \(L_{\rm B}\ge13\); \(a_n=L_{\rm B}^{-K_n}\ell_0\), \(T_n=2L_{\rm B}^{H_n}\ell_0\), \(H_n=3n+O(1)\), \(0\le n-K_n\le O(1)\); \(\beta_{W,n}=Y_0/N\) with \((\log Y_0)^r=L_{\rm B}^{2n+s+1/2}\), \(r\ge2\) fixed; the measure is the Wilson measure \(e^{-\beta_{W,n}\sum_ps_p}\) on the cube with \(N_n=T_n/a_n=2L_{\rm B}^{H_n+K_n}\) sites per side.

**Theorem 10.1 (Theorem 5 of `Periodic transfer states and a finite-volume criterion` without hypothesis (W)).** On this family, for all large \(n\),
\[
0\le\Gamma_n\le\tfrac12\Phi_n\Big\vert_{L=2}\le13\,d_G\log\beta_{W,n}+140\,d_G\log N_n+C_N,\qquad\frac{\Gamma_n}{T_n/\ell_0}\longrightarrow0.
\]

*Proof.* \(N_n\) is even, so Theorem 2 of `Periodic transfer states and a finite-volume criterion` applies with \(L=2\), \(m=N_n/2\). Theorem Φ needs \(\beta_{W,n}\ge\beta_*N_n^{C_0}\): \(\log\beta_{W,n}=L_{\rm B}^{(2n+s+1/2)/r}-\log N\) grows exponentially in \(n\), while \(C_0\log N_n\le C_0(4n+O(1))\log L_{\rm B}\). Then \(\Phi_n\le\frac{49}2d_G\log\beta+272d_G\log m+16C\). Finally \(\log\beta_{W,n}\le L_{\rm B}^{\,n+(s+1/2)/2}\) because \(r\ge2\), \(\log N_n=O(n)\), and \(T_n/\ell_0=2L_{\rm B}^{3n+O(1)}\). \(\square\)

**Corollary 10.2.** On the B-02 family, Annex M (4.5) holds for every fixed positive-time polynomial \(F\) of every degree, for any field prescription whose marks satisfy the growth condition (G) of `Periodic transfer states and a finite-volume criterion` §1.3 (and the structural hypothesis recorded in `Transfer normalization and the marked-insertion condition` §1.4). In particular it holds for prescriptions whose coefficients are bounded by a fixed power of \(\beta_{W,n}/a_n\), such as the comparison multipliers \(z_h\sim\beta_W/2\) of `Coupling comparison` §4.
