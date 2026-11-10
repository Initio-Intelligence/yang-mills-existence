# Weighted operator estimates on collars

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

## 2. Setting and hypotheses

### 2.1 Geometry

\(\{\Omega_j\}_{j\le k}\) as in [V] (1) / [P2] (2.2): \(\operatorname{dist}(\Omega_j^c,\Omega_{j+1})>RML^j\eta\) (\(M\) = [P]'s walk-cube size = \(M_1\) of [III]; \(R=R_1\)). \(\mathfrak B=\bigcup_j\Lambda_j\) (localization points), \(\Delta(y)=B^j(y)\) for \(y\in\Lambda_j\) ([P] p.397: "if \(y\in\Lambda_j\), then \(\Delta(y)=B^j(y)\)"); the blocks \(\Delta(y)\) partition the lattice; each bond and each datum is assigned to one block \(y(\cdot)\). The distance \(d\) is [P2] (2.46): infimum over admissible contours of \(\sum_j(L^j\eta)^{-1}\lvert\Gamma\cap B^j(\Lambda_j)\rvert\) (text p.231). It is symmetric and satisfies the triangle inequality ([P2] (2.54), text: "This is of course the triangle inequality for our distance").

- **Row sums.** \(S(\delta'):=\sup_y\sum_{y'\in\mathfrak B}e^{-\delta'd(y,y')}\). [P2] Lemma 2.1 (text p.233–234): \(S(\alpha\delta_0)\le c_1(\alpha)\) if \(\frac12\alpha\delta_0RM>2d\log c_0(\frac12\alpha)+1\) (2.59). The source uses \(\alpha=\frac12\). Assume (2.59) at \(\alpha=\frac12\) only.
- **Layer separation.** [MS] Lemma BM.1: \(y\in\Lambda_n\), \(y'\in\Lambda_k\) \(\Rightarrow d(y,y')\ge RM(\lvert k-n\rvert-1)_+\). Its proof decomposes a contour at the interfaces as in [P2] (2.47)–(2.48), (2.57). ; deduction given [P2] (2.2), (2.46). Consequence (scale exchange): for every real \(\gamma\),
\[
(L^{j'}/L^{j})^{\gamma}\le L^{\lvert\gamma\rvert}\exp\Bigl(\frac{\lvert\gamma\rvert\log L}{RM}\,d(y,y')\Bigr).\tag{2.1}
\]
- **(Geo)** Assume (2.59) at \(\alpha=\frac12\), and \(\delta_0RM\ge16\log L\). Then for \(\lvert\gamma\rvert\le4\) the exchange (2.1) costs at most the rate \(\frac14\delta_0\).

### 2.2 Weights and weighted norms (definitions)

Fix \(\lambda\ge0\). \(\mathcal W_\lambda\) is the set of functions \(w=\lambda\rho\), \(\rho:\mathfrak B\to\mathbb R\), with \(\lvert\rho(y)-\rho(y')\rvert\le d(y,y')\). They are extended to bonds and data by \(w(b):=w(y(b))\), so they are **block-constant**. \(0\in\mathcal W_\lambda\). For \(y_0\in\mathfrak B\) and \(S\subset\mathfrak B\), \(\rho=d(\cdot,y_0)\) and \(\rho=d(\cdot,S)\) are admissible (triangle inequality).

For a field \(f\) and real \(\alpha\): \(\lvert f\rvert_{(\alpha),w}:=\sup_be^{w(b)}(L^{j(b)}\eta)^{-\alpha}\lvert f(b)\rvert\). This is [P] (3.41) with a weight. For jets: \(m_w(A):=\max\{\lvert A\rvert_{(-1),w},\lvert\nabla A\rvert_{(-2),w}\}\), so \(m_0=m\) of [SI]. A field and its covariant gradient are always carried **together as a jet**, and the weight multiplies both components at the same point. **The weight is never differentiated.** This is possible because in every formula used below a derivative falls either on the kernel of an operator (\(\nabla P\), \(P\nabla^*\), \(\Delta_UP\), with their own kernel bounds) or inside a pointwise local map of jets ([V] (94)–(96)). This is [REF] §2.4 (P1); see (S-calc).

For a linear map \(T\) between such normed spaces: \(\lVert T\rVert_\lambda:=\sup_{w\in\mathcal W_\lambda}\lVert e^{w}Te^{-w}\rVert\), the norm being between the weighted norms (equivalently, between unweighted norms of the conjugated operator). Since \(0\in\mathcal W_\lambda\), \(\lVert T\rVert_\lambda\ge\lVert T\rVert_0\). All lattices are finite, so \(e^{w}\) is an invertible diagonal matrix and conjugation is an algebra automorphism.

### 2.3 Hypothesis (K): block-kernel bounds of the package

A linear map \(P\) has a **block-kernel bound of type \((\alpha\to\beta)\) with constants \((B_P,\delta)\)** if for all \(y,y'\), all \(f\) supported in \(\Delta(y')\) and all \(x\in\Delta(y)\):
\[
(L^{j(y)}\eta)^{-\beta}\lvert(Pf)(x)\rvert\le B_P\,e^{-\delta d(y,y')}\,(L^{j(y')}\eta)^{-\alpha}\lvert f\rvert_\infty.\tag{2.2}
\]
For Hölder outputs, replace the left side by the localized Hölder norm \(\lVert\zeta\nabla Pf\rVert_\beta\) with \(\zeta\in C_0^\infty(\tilde\Delta(y))\) and its scale factor, as in [P] (3.43), (3.45), (3.133).

> **(K)** The four primitives \(G'\), \(C'=(Q'G'^2Q'^*)^{-1}\), \(G_0=(\Delta+DRD^*+Q^*aQ)^{-1}\), \(C_0=(QG_0Q^*)^{-1}\), with the derivative placements \(\nabla P\), \(P\nabla^*\), \(\nabla P\nabla^*\), \(\Delta_UP\) (the latter for \(G_0\), \(G'\)) and the Hölder forms, satisfy (2.2) in the types of [P] (3.42)–(3.45), (3.48), (3.132), with constants \((B_0,\delta_0)\). Here \(\delta_0\), \(B_0\) are [P]'s "common, best possible, decay rate … and common constants" (p.423, after Theorem 3.12).

*Hypotheses.* source input for the statements. [P] (3.42) (p.397): "\(\lvert(G'(U)\lambda)(x)\rvert,\ \lvert(\nabla_UG'(U)\lambda)(x)\rvert,\ \lvert(G'(U)\nabla_U^*\lambda)(x)\rvert,\ \lvert(\Delta_UG'(U)\lambda)(x)\rvert\le B_0[(L^j\eta)^2,L^j\eta,L^j\eta,1]e^{-\delta_0d(y,y')}\lvert\lambda\rvert\) for \(x\in\Delta(y)\), \(y\in\Lambda_j\), \(\operatorname{supp}\lambda\subset\Delta(y')\)". Theorem 3.3 (p.399): "the operator \(G(U)\) (\(a=1\)) satisfies the inequalities (3.42)–(3.47)". (3.48) for \(C'\) (p.398). (3.132) for \((QGQ^*)^{-1}\) (p.422). [P] writes (3.42) with the scale factor at the output level only. The form (2.2) follows by (2.1): type \((\gamma\to\gamma+2)\) for \(G'\) holds with \(B_P=L^{\lvert\gamma\rvert}B_0\) and rate \(\delta_0-\lvert\gamma\rvert\log L/(RM)\ge\frac34\delta_0\) under (Geo). (deduction given BM.3; this is [P] p.398's "Using Lemma 2.1 in [4] we may replace the factor \((L^j\eta)^\alpha\) by \((L^j\eta)^\beta(L^{j'}\eta)^\gamma\)".) **Proof level in the source:** Theorems 3.1–3.3 rest on the sketched random-walk Theorem 3.10 ((U1) of [REF]); (3.132) is asserted ("let us write only bounds", (U2)). For complex \(U'U\) on (3.37): [P] Theorem 3.4 and Corollaries 3.5–3.6 (text; [SI] F4). These are exactly the inputs of [SI] Theorem P9♮. **No walk expansion is used below.**

Every other operator in [V] (179)–(180) is a composite of these four, their transposes and local maps ([SI] §2; [REF] §5.2 for \(P_1\)). The primitives are symmetric for the bilinear pairing, which continues analytically from the real case ([SI] F4), so transposes of composites are again composites.

### 2.4 Hypothesis (S-calc): the formula structure

> **(S-calc)** On the complex ball \(\mathfrak D_a=\{A':m(A')<a\}\), \(F:=\delta V_\Delta/\delta A'\) is a **formula of the calculus \(\mathcal C\)** of §3.2. Its terms are [V] (85), (88), (89), (90), (93)–(96) and the term \(\delta W/\delta A'\) of [SI] Lemma 3.1, the latter in the (138)-reduced form. Its nodes are: the derived operators of [SI] §2 (\(P\), \(R\), \(\Delta'_\pi\), \(G_\pi\), \(C_\pi\), \(H\), \(H_0\), \(\Delta^{(2)}\), the new \(G\), \(C\), \(\tilde G\)), with derivatives placed as in [REF] (P1); the local holomorphic maps \(C_j\), \(\delta C_j/\delta A\) and its transpose, \(V_0'\), \(\partial V_0'/\partial A\), the commutator expressions (94)–(96), multiplication by the fixed fields \(J\), \(H^*J\), and \(Q,Q^*,a,D,D^*\); and the nested fixed points \(D(A')\) ([V] (50)) and \(v\mapsto(I+\mathfrak R)^{-T}v\) (the transpose of (70)). The same holds for the representation outputs \(\Phi_\Delta,\Phi_{D^*D}\) of [SI] §3.3, with [REF] §3.2's reading.

*Hypotheses.* The term list: source input. See [V] pp.290–292 in the source: (80), (85)–(90), (91)–(96), Prop. 4 (p.292–293). The node decomposition: additional assumption. It is [SI] Theorem S(2), justified in [REF] §3.2. The (138)-reading: [REF] §3.2.

The structure I actually use is weak. Every term is a finite composition of linear package composites and pointwise local holomorphic maps of jets, with finitely many fixed points that are contractions. [V] p.292 shows how derivatives enter. (93) is "\(\frac12D^*\sum i[A'',A'']\)". By (96) (source) the \(D^*\) of the leading commutator becomes a local expression in \((A',\nabla A')\). The other terms are "obtained by replacing some \(A'\) in the commutator by \(-HD(A')\)", whose gradients are \((\nabla H)D(A')\).

### 2.5 Hypothesis (Loc): local maps

Each local holomorphic map \(f\) has an output at \(b\) that depends only on its arguments on blocks \(\Delta(y')\) with \(d(y(b),y')\le r_{\rm loc}\). It is holomorphic and bounded by \(K_f\) on a product of balls of radii \(\rho_f\) in the scale-weighted sup norms. The bounds are [V] (40), (44) (\(\lvert C_j(A)\rvert\le C_2(L^j\eta)^2\lvert A\rvert^2\)), (72), and [P] (3.137) for \(\Delta^{(2)}\) ("the supremum \(\lvert A\rvert\) is taken over several \(j\)-blocks surrounding \(\Delta(y)\)", p.423). \(r_{\rm loc}\) is a fixed number. Adjacent blocks of equal or adjacent levels are at distance \(O(d)\); Take \(r_{\rm loc}\le3d\) additional assumption. Put \(\varkappa:=e^{\lambda r_{\rm loc}}\le e^{3d\delta_0/4}\).

## 3. The weighted calculus

### 3.1 Basic lemmas

**Lemma 3.1 (package operators).** If \(P\) satisfies (2.2) with \((B_P,\delta)\) and \(0\le\lambda<\delta\), then \(\lVert P\rVert_\lambda\le B_PS(\delta-\lambda)\) from \(\lvert\cdot\rvert_{(\alpha)}\) to \(\lvert\cdot\rvert_{(\beta)}\). Under (Geo), every primitive in every type of (K) with \(\lvert\gamma\rvert\le4\) satisfies \(\lVert P\rVert_\lambda\le B_\lambda:=L^4c_1(\tfrac12)B_0\) for \(0\le\lambda\le\frac14\delta_0\).

*Proof.* Write \(f=\sum_{y'}1_{\Delta(y')}f\). For \(x\in\Delta(y)\):
\[
e^{w(y)}(L^j\eta)^{-\beta}\lvert P(e^{-w}f)(x)\rvert\le\sum_{y'}B_Pe^{-\delta d(y,y')}e^{w(y)-w(y')}(L^{j'}\eta)^{-\alpha}\lvert f\rvert_{\Delta(y')}\le B_P\sum_{y'}e^{-(\delta-\lambda)d(y,y')}\lvert f\rvert_{(\alpha)}.
\]
For the second claim, (K) and (2.1) give rate \(\ge\frac34\delta_0\) and constant \(\le L^4B_0\); then \(\frac34\delta_0-\lambda\ge\frac12\delta_0\) and \(S(\frac12\delta_0)\le c_1(\frac12)\). Hölder outputs are the same computation. \(\square\)

**Lemma 3.2 (local linear maps).** If \(T\) is linear, \((Tf)(b)\) depends only on \(f\) on blocks within \(d\)-distance \(r\) of \(y(b)\), and \((L^{j(b)}\eta)^{-\beta}\lvert(Tf)(b)\rvert\le\ell\,\sup(L^{j'}\eta)^{-\alpha}\lvert f\rvert\) over those blocks, then \(\lVert T\rVert_\lambda\le e^{\lambda r}\ell\). If \(f\) is a local holomorphic map as in (Loc), and the arguments \(Z\) stay in balls of radius \(\rho_f-\sigma\), then \(Df(Z)\) is such a \(T\) with \(r=r_{\rm loc}\) and \(\ell\le K_f/\sigma\) in each slot.

*Proof.* \(\lvert w(b)-w(b')\rvert\le\lambda r\). For the second part, for fixed \(b\) and \(\lvert h\rvert_{(\alpha)}\le1\), the scalar function \(t\mapsto f(Z+th)(b)\) is holomorphic for \(\lvert t\rvert<\sigma\) and bounded by \(K_f\) in its scale weight. Cauchy then gives the bound, and the derivative at \(b\) depends only on \(h\) near \(b\). \(\square\)

**Lemma 3.3 (products, Neumann series).** \(\lVert ST\rVert_\lambda\le\lVert S\rVert_\lambda\lVert T\rVert_\lambda\). If \(\lVert K\rVert_\lambda\le q<1\), then \(I-K\) is invertible and \(\lVert(I-K)^{-1}\rVert_\lambda\le(1-q)^{-1}\). The inverse is the ordinary one: \(e^{w}(I-K)^{-1}e^{-w}=(I-e^{w}Ke^{-w})^{-1}\).

*Proof.* Conjugation by the invertible diagonal \(e^{w}\) is an algebra automorphism; Neumann series. \(\square\)

**Lemma 3.4 (readouts).** Suppose \(\lVert T\rVert_\lambda\le K\), with \(T\) mapping data or fields into \(\lvert\cdot\rvert_{(\beta)}\).
1. *Kernel form.* For \(f\) supported in \(\Delta(y')\) and \(x\in\Delta(y)\): \((L^{j}\eta)^{-\beta}\lvert Tf(x)\rvert\le Ke^{-\lambda d(y,y')}(L^{j'}\eta)^{-\alpha}\lvert f\rvert_\infty\).
2. *Set form.* For \(f\) supported in blocks of \(S\subset\mathfrak B\) and \(x\in\Delta(y)\): \((L^j\eta)^{-\beta}\lvert Tf(x)\rvert\le Ke^{-\lambda d(y,S)}\lvert f\rvert_{(\alpha)}\). **No row sum is needed.**

*Proof.* Take \(w=\lambda d(\cdot,y')\), resp. \(w=\lambda d(\cdot,S)\). Both lie in \(\mathcal W_\lambda\) and vanish on the support of \(f\). Then \(e^{w(y)}\lvert Tf(x)\rvert\le K\lvert f\rvert\). \(\square\)

### 3.2 The calculus \(\mathcal C\) and the weighted chain rule

Fix a complex ball \(\mathfrak D_a\) in a jet norm. **Formulas** are holomorphic maps \(\Phi:\mathfrak D_a\to\) fields, built by:
- (C0) the variable \(Z\), or a fixed field \(\varphi\) (independent of \(Z\));
- (C1) \(P\Psi\), with \(P\) a package composite or a local linear map;
- (C2) \(f(\Psi_1,\dots,\Psi_m)\), with \(f\) local holomorphic (sums and pointwise products included);
- (C3) \(X(Z)\), the unique solution in a ball of \(X=\Psi(X,Z)\), where \(\Psi\) is a formula in the two variables \((X,Z)\).

For every node define
\[
\mathsf K_\Phi(\lambda):=\sup_{Z\in\mathfrak D_a}\lVert D\Phi(Z)\rVert_\lambda ,
\]
and, for (C3), \(\mathsf q_\Psi(\lambda):=\sup\lVert\partial_X\Psi(X(Z),Z)\rVert_\lambda\).

**Lemma 3.5 (weighted chain rule).** The following hold, with every node's base value ranging over its values on \(\mathfrak D_a\).
- (C0) \(\mathsf K_Z=1\), \(\mathsf K_\varphi=0\).
- (C1) \(\mathsf K_{P\Psi}\le\lVert P\rVert_\lambda\mathsf K_\Psi\).
- (C2) \(\mathsf K_{f(\Psi)}\le\varkappa\sum_i\ell_{f,i}\mathsf K_{\Psi_i}\), with \(\ell_{f,i}\le K_f/\sigma_i\) as in Lemma 3.2, where \(\sigma_i\) is the margin of the values of \(\Psi_i\) inside \(f\)'s domain.
- (C3) If \(\mathsf q_\Psi(\lambda)<1\), then \(\mathsf K_X\le\mathsf K^{(Z)}_\Psi/(1-\mathsf q_\Psi)\), where \(\mathsf K^{(Z)}_\Psi\) is the bound for \(\partial_Z\Psi\) at frozen \(X\).

Hence, for any finite formula all of whose fixed-point nodes satisfy \(\mathsf q<1\), \(\mathsf K_\Phi(\lambda)\) is finite. It is obtained from the unweighted recursion (\(\lambda=0\)) by replacing each package-composite norm by its \(\lambda\)-norm and multiplying each local derivative by \(\varkappa\).

*Proof.* Holomorphy gives Fréchet derivatives. (C1), (C2): chain rule and Lemmas 3.2–3.3. (C3): differentiate \(X(Z)=\Psi(X(Z),Z)\) to get \((I-\partial_X\Psi)DX=\partial_Z\Psi\), then Lemma 3.3. \(\square\)

*Remark.* In (C2) the coefficients of \(Df\) are base-point values: non-decaying, merely bounded fields such as \(J\), \(H^*J\), \(D(A')\), \((I+\mathfrak R)^{-T}v\). They enter as **pointwise** multipliers, so they cost no rate. This is exactly [MS] (BM.8)–(BM.9)'s "place the weight on the one differing factor and bound the other factors in the ordinary small norm". Lemma 3.5 is the precise form of that sketch, including the nested fixed points.

## 4. The weighted form of (189) conditional

Fix \(0<\lambda\le\frac14\delta_0\) and assume (Geo), (K), (S-calc), (Loc). \(B\ge1\) denotes the package constant of [SI] §2 (for the true package, \(B\simeq B_0\) up to the [SI] crude composite counts). Write \(\hat B_\lambda:=\varkappa B_\lambda\). \(c,C\) denote constants depending only on \(d,L,C_2,C_3,C_4\), the (Loc) constants, \(M_1,R_1\), and the formula. They do **not** depend on \(\{\Omega_j\}\), \(k\), the volume or the background.

**Lemma 4.1 (nested contractions are weighted contractions).** Assume the background ceiling \(\alpha_J\hat B_\lambda^{10}\le c_S\) ([SI] Theorem S with \(B\to\hat B_\lambda\)) and \(a=a_\lambda:=c_S\hat B_\lambda^{-2}\). Then on \(\mathfrak D_{a_\lambda}\):
1. the Neumann series defining \(G_\pi,C_\pi,G,C\) converge in \(\lVert\cdot\rVert_\lambda\) with per-step factor \(\le\frac12\);
2. the fixed point \(D(A')\) satisfies \(\mathsf q\le\frac12\);
3. so does the linear fixed point \((I+\mathfrak R(A'))^{-T}\).

Consequently \(\mathsf K_F(\lambda)\le C\hat B_\lambda^{p_F}\) for a fixed integer \(p_F\).

*Proof.*
1. The per-step operators (\(\Delta'_\pi G_0\), \(\Delta^{(2)}G_0\), \(QG_0\Delta'_\pi G_\pi Q^*C_0\), …) are composites. Their \(\lambda\)-norms are [SI]'s crude unweighted counts with \(B\to\hat B_\lambda\) (Lemmas 3.1–3.3). [SI]'s table gives at most \(\alpha_J\hat B_\lambda^{9}\le\frac12\).
2. \(\partial_X\Psi_D=-L^j\eta\,C_j'(L^j\eta(A'-HX))\,L^j\eta H\). By Lemma 3.2 with [V] (44)/(72), \(\lVert\cdot\rVert_\lambda\le\varkappa\cdot cC_2\,\hat B_\lambda^{2}\,a\le\frac12\). This is [V] (69), (71), "\(1-9C_2B_0\varepsilon_3dc_1(\frac12)\)", with the weight.
3. \(\mathfrak R=L\eta\langle\delta C/\delta A,H\rangle\) is bounded the same way.

The bound on \(\mathsf K_F\) is Lemma 3.5 applied to the finite formula (S-calc). Base values lie in the domains of the local maps with margins by [SI] Theorem S(1)–(2), which bound every intermediate node on \(\mathfrak D_{a_3}\), \(a_3=c_SB^{-2}\ge a_\lambda\). \(\square\)

*Exponent.* \(p_F\) is the maximal number of primitive factors along a root-to-leaf chain of \(F\)'s formula, each Neumann series counted once. From [SI] §2's crude table (\(H\sim B^2\), \(\tilde G\sim B^3\), \(G'RD^*\sim B^4\), \(\mathfrak D\sim B\)) and the terms (85)–(96), Lemma 3.1, the chain is longest for the \(W\)-term, \(p_F\le8\) additional assumption. Only finiteness matters.

**Lemma 4.2 (Schwarz).** \(F(0)=0\) and \(DF(0)=0\).

*Proof.* [SI] Theorem S(2): \(\lvert F(A')\rvert_{(-3)}\le C_4'm(A')^2\) on \(\mathfrak D_{a_3}\). (This is [V] (98) for \(V_\Delta\).) Hence \(F(tA')=O(t^2)\) for complex \(t\). \(\square\)

**Proposition 4.3 (weighted (189)).** For complex \(A'\) with \(m(A')<a_\lambda\) and every \(w\in\mathcal W_\lambda\),
\[
\lVert e^{w}\,DF(A')\,e^{-w}\rVert_{m\to(-3)}\le\frac{\mathsf K_F(\lambda)}{a_\lambda}\,m(A').\tag{4.1}
\]
In kernel form (Lemma 3.4(1)), for \(\mathfrak A\) supported in \(\tilde\Delta(y')\) and with \(y\in\Lambda_j\):
\[
\Bigl\lvert\Delta(y)\frac{\delta^2V_\Delta}{\delta A'^2}(A')\mathfrak A\Bigr\rvert\le\varkappa\frac{\mathsf K_F}{a_\lambda}m(A')(L^j\eta)^{-3}e^{-\lambda d(y,y')}\max\{\lvert\mathfrak A\rvert_{(-1)},\lvert\nabla\mathfrak A\rvert_{(-2)}\}.
\]
This is (189), with its printed rate \(\frac14\delta_0\) available (\(\lambda=\frac14\delta_0\)) and \(O(1)\varepsilon_3\) replaced by \(\varkappa(\mathsf K_F/a_\lambda)m(A')\le C\hat B_\lambda^{p_F+2}m(A')\).

*Proof.* Fix \(w\), \(A'\), a jet \(h\) with \(m_w(h)\le1\), an output bond \(b\) and a component. The scalar \(g(t):=[e^{w}DF(tA')e^{-w}h](b)\cdot(L^{j(b)}\eta)^3\) is holomorphic on \(\lvert t\rvert<a_\lambda/m(A')\), because \(tA'\in\mathfrak D_{a_\lambda}\) and \(m\) is a norm. It is bounded by \(\mathsf K_F\) (Lemma 4.1), and \(g(0)=0\) (Lemma 4.2). The Schwarz lemma gives \(\lvert g(1)\rvert\le\mathsf K_Fm(A')/a_\lambda\). Taking the sup over \(b,h\) gives (4.1). The support \(\tilde\Delta(y')\) costs the factor \(\varkappa\). \(\square\)

So the "awkward and complicated" kernel computation of [V] p.308 is not needed in sharp form. Crude weighted bounds on a fixed ball, plus the vanishing of \(DF\) at the origin, give (189) with the small factor \(m(A')\). This is the factor the source writes as \(\varepsilon_3\).
