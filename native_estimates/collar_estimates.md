# The one-sided collar estimate

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

## 2. (S-calc)

### 2.1 The form \(\Delta'_\pi\)

[P] p.419, (3.117): "\(\langle D\lambda,J\rangle=0\), or \(D^*J=0\)", and
"\(\langle A-D\lambda,\Delta(A-D\lambda)\rangle=\langle A,\Delta A\rangle-\langle i[\lambda(b_-),A(b)]-i[A(b),R_b\lambda(b_+)]-i[\lambda(b_-),(D\lambda)(b)],J\rangle\)".
(3.119): "\(\langle A,\Delta_\pi A\rangle=\langle A-DG'RD^*A,\Delta(A-DG'RD^*A)\rangle\)". (3.120): the same with \(\lambda=G'RD^*A\), "\(=\langle A,\Delta A\rangle-\langle A,\Delta'_\pi A\rangle\)".
p.421, (3.130): "\(G=G_0(I-\Delta'_\pi G_0)^{-1}=\sum_{n=0}^\infty G_0(\Delta'_\pi G_0)^n\)", and: "we have to be careful only with the third term in the definition (3.120) of \(\Delta'_\pi\). One of the three derivatives there has to be applied either to an expression on the right, or on the left, of \(\Delta'_\pi\). For example one of the terms in \(\langle A_1,\Delta'_\pi A_2\rangle\) is \(\frac12\langle i[(DG'RD^*A_1)(b),(G'RD^*A_2)(b_-)],J\rangle\), and we apply the derivative \(D^*\) to \(A_1\)." p.422, (3.131): the bound with \(\lVert D^*A_1\rVert_{L^1}+(L^j\eta)^{-1}\lVert A_1\rVert_{L^1}\) on the left and \(\lvert D^*A_2\rvert+(L^{j'}\eta)^{-1}\lvert A_2\rvert\) on the right.

Write \(\Lambda:=G'RD^*\), \(\lambda_i:=\Lambda A_i\), \((S\lambda)conditional:=\lambda(b_-)+R_b\lambda(b_+)\). The first two terms of (3.120) polarize to \(\frac12\langle i[S\lambda_1,A_2],J\rangle+\frac12\langle i[S\lambda_2,A_1],J\rangle\). The third polarizes to \(-\frac12\langle i[\lambda_1(b_-),D\lambda_2]+i[\lambda_2(b_-),D\lambda_1],J\rangle\) (signs as printed; they play no role below).

### 2.2 The placement problem and its repair

**The problem.** With the symmetric polarization, one term needs \(D\lambda_1=DG'R(D^*A_1)\) and the other \(D\lambda_2=DG'R(D^*A_2)\). As an operator, \(\Delta'_\pi A_2=f_0+Df_1\) with \(f_0\) depending on \((A_2,D^*A_2)\), and \(f_1=RG'D^*(J\star\lambda_2)\) only Hölder continuous. In \(G_0\Delta'_\pi G_0\Delta'_\pi G_0\) the middle factor then appears as \(D^*G_0D\,f_1\). The only printed bound for it is [P] (3.44), p.398 source:
"\(\lvert(\nabla_UG'(U)\nabla_U^*\lambda)(x)\rvert\le B_0'(\varepsilon)e^{-\delta_0d(y,y')}(\lVert\lambda\rVert^{\xi'}_\varepsilon+\lvert\lambda\rvert)\) for \(0<\varepsilon\le1\), \(x\in\Delta(y)\), \(\operatorname{supp}\lambda\subset\tilde\Delta(y')\)", with \(B_0'(\varepsilon)\to\infty\) as \(\varepsilon\to0\).

**Lemma PL (one-sided placement).** For site fields \(\lambda_1,\lambda_2\) and any bond field \(J\),
\[
\bigl\langle[\lambda_1(b_-),D\lambda_2]+[\lambda_2(b_-),D\lambda_1],J\bigr\rangle=\bigl\langle[\lambda_1,\lambda_2],D^*J\bigr\rangle-\bigl\langle[D\lambda_1,S\lambda_2],J\bigr\rangle.
\]
*Proof.* \(R_b\) is an automorphism of the Lie algebra and \(R_b\lambda(b_+)=\lambda(b_-)+\eta D\lambda\). So \(D[\lambda_1,\lambda_2]=[D\lambda_1,\lambda_2(b_-)]+[\lambda_1(b_-),D\lambda_2]+\eta[D\lambda_1,D\lambda_2]\). The left bracket of the claim is \([\lambda_1(b_-),D\lambda_2]-[D\lambda_1,\lambda_2(b_-)]=D[\lambda_1,\lambda_2]-[D\lambda_1,2\lambda_2(b_-)+\eta D\lambda_2]=D[\lambda_1,\lambda_2]-[D\lambda_1,S\lambda_2]\). Pair with \(J\). \(\square\)

**Right form as an operator.** For a pair \(u=(A,a)\), with \(a\) standing for \(D^*A\), put \(\lambda[u]:=G'Ra\) and
\[
\Delta^R[u]:=\tfrac12\,i[J,S\lambda[u]]^\flat+\tfrac12\,DRG'S^T\bigl(i[A,J]\bigr)+\tfrac12\,DRG'S^T\bigl(i[DG'Ra,J]\bigr)
\]
(\(\flat\): the bond field representing the pairing; signs as in §2.1). Then \(\Delta'_\pi A=\Delta^R[(A,D^*A)]\) when \(D^*J=0\). Every kernel is of a printed sup-input type: \(G'\), \(\nabla G'\) ([P] (3.42) entries 1–2), \(R=I-G'Q'^*C'Q'G'\) ((3.48)), and \(J\) is a pointwise multiplier. **No derivative falls on \(J\).**

**Lemma GP (the chain for \(G_\pi\)) (b on K1–K3 of §3).** Let \(\mathcal G f:=(G_0f,D^*G_0f)\) and \(N:=\Delta^R\circ\mathcal G\) on \(\lvert\cdot\rvert_{(-3)}\). Then \(\lVert N\rVert_\lambda\le c\,\alpha_J\hat B_\lambda^{9}\). If this is \(\le\frac12\):
1. \(G_\pi:=G_0(I-N)^{-1}\) satisfies \(\lVert G_\pi\rVert_\lambda,\lVert\nabla G_\pi\rVert_\lambda\le2\hat B_\lambda\), the Hölder form of (3.43), **and** \(\lVert\Delta_UG_\pi\rVert_\lambda\le2\hat B_\lambda\), because \(\Delta_UG_\pi=(\Delta_UG_0)(I-N)^{-1}\). When \(D^*J=0\) it is \((\Delta_a-\Delta'_\pi)^{-1}\).
2. The transpose is the left-form chain: \(\Delta^LA=F_0(A)+DF_1(A)\) with \(F_0=\frac12i[J,S\Lambda A]^\flat\), \(F_1=\frac12RG'S^T(i[A,J])+\frac12RG'D^*(J\star S\Lambda A)\), \(\Lambda A=(G'RD^*)A\) through the kernel \(G'\nabla^*\) ((3.42) entry 3). Both depend on \(\lvert A\rvert_{(-1)}\) only, and \(G_0(F_0+DF_1)=G_0F_0+(G_0\nabla^*)F_1\). So \(G_\pi^T\) is bounded in \(\lVert\cdot\rVert_\lambda\) from \(\lvert\cdot\rvert_{(-3)}\) and from sources \(D^Tg\), \(\lvert g\rvert_{(-2)}\), to \(\lvert\cdot\rvert_{(-1)}\).
3. Hence \(C_\pi=(QG_\pi Q^*)^{-1}\), \(H=G_\pi Q^*C_\pi(L\eta)^{-1}\), \(\nabla H\), \(H^T\), \(H^T\nabla^T\) are \(\lambda\)-bounded with constants polynomial in \(\hat B_\lambda\).

*Proof.* Count the factors in \(\Delta^R\): \(\lVert R\rVert_\lambda\le1+\hat B_\lambda^3\), so each of the three terms is \(\le c\alpha_J\hat B_\lambda^8\) from \(\lvert A\rvert_{(-1),w}+\lvert a\rvert_{(-2),w}\) to \(\lvert\cdot\rvert_{(-3),w}\); \(\lVert\mathcal G\rVert_\lambda\le2\hat B_\lambda\) by (3.42) entries 1–2 for \(G_0\) (Theorem 3.3). Neumann series in the weighted norm. Item 2 is the same count with entry 3. Item 3: \(Q(G_\pi-G_0)Q^*C_0\) is small, Neumann again. \(\square\)

**Remark 2.4.** (i) Item 1 gives a Laplacian bound for \(G_\pi\) directly. [P] p.423 says the Laplacian inequality "does not hold for \(G,G_1\)". For \(G_1\) the obstruction is genuine (\(\Delta^{(2)}_\pi\) contains \(DRG'D^*\Delta^{(2)}\), (3.135), with nothing to integrate by parts against). For \(G=G_\pi\) The interpretation of the remark is "not obtained from (3.131)". Consistency check: [V] (138)–(139) obtains \(\lvert\Delta'_\pi HB\rvert_{(-3)}\le O(1)\lvert B\rvert\), which is the right form at \(\lambda_{HB}=0\). **This point contradicts a printed sentence and should be read by a second person before it is used; nothing in Theorem CT♯ depends on it** (the second-order rows use the representation output of [SI] §3.3). (ii) For an independent variable \(\mathbf J\) ([I] (3.13)), for the \(s\)-deformed package and for an abstract package, \(D^*J=0\) or the symmetry of the primitives may fail. There \(\Delta'_\pi\) entering \(G_\pi\) is *defined* by the right form (with deformed primitives), and transposes by the left form. This agrees with the source when \(\mathbf J=J(\mathbf U)\), \(s=1\). It is the same device as [DN] §4.2's "defined by the final operator forms". additional assumption as a convention; it must be written into (S-calc).

### 2.3 The node formula of \(\delta W/\delta A'\)

[V] p.299, (138) source: "\(2\langle A,\Delta'_\pi HB\rangle=\langle i[(G'RD^*A)(b_-)+R_b(G'RD^*A)(b_+),(HB)(b)],J\rangle\)", after "This equality [\(RD^*H=0\)] implies also that \(\Delta'_\pi H\) simplifies essentially". This is §2.1 with \(\lambda_{HB}=0\). [V] p.297 source: "we get the functional (74), with the operator \(\Delta\) instead of \(\Delta_\pi\)"; (127) holds "for all \(\delta A'\) satisfying \(Q\delta A'=0\)". With (80) (p.290, c) this gives [SI] Lemma 3.1: \(V_\Delta=V+W\), \(W(A')=-\langle A',\Delta'_\pi HD(A')\rangle=-\frac12\langle i[S\Lambda A',HD(A')],J\rangle\). ; the term \(\frac12\langle HD,\Delta'_\pi HD\rangle\) vanishes because every term of (3.120) contains \(\Lambda HD=0\).

Node formula:
\[
\frac{\delta W}{\delta A'}=-\tfrac12\,D\,RG'\,S^T\bigl(i[HD(A'),J]\bigr)^\flat-\tfrac12\,\mathfrak D(A')^TH^T\bigl(i[J,S\,G'RD^*A']\bigr)^\flat.
\]
Derivatives: in the first term, the outer \(D\) sits on the kernel of \(RG'=G'-G'Q'^*C'Q'G'G'\), type \(\nabla G'\); in the second, \(D^*\) sits on the kernel \(G'\nabla^*\) (or on the jet component \(D^*A'\)). \(J\) is multiplied pointwise in both. Weights: \([HD,J]\in(-4)\), \(G'\to(-2)\), \(\nabla G'\to(-3)\); \(\Lambda A'\in(0)\), \([J,\cdot]\in(-3)\), \(H^T\) to block fields, \(\mathfrak D^T\) back. Both terms are \(O(m^2)\). **No derivative on \(J\); every derivative on a decaying kernel.**

### 2.4 \(\Delta'_\pi H\) and the second-order outputs

By (138), \(\Delta'_\pi HX=\frac12DRG'S^T(i[HX,J])^\flat\): one kernel \(\nabla G'\), one pointwise \(J\). [V] p.298, (137) source: "\(\Delta_\pi H=(\Delta_\pi+DRD^*+Q^*aQ)H-Q^*a(L^{j(\cdot)}\eta)^{-1}=Q^*(QGQ^*)^{-1}(L^{j(\cdot)}\eta)^{-1}-Q^*a(L^{j(\cdot)}\eta)^{-1}\)". p.299 source: "\(\Delta=D^*D+\Delta'\), \(\Delta'\) is a local, bounded operator"; (140): "\(D^*DHB=(D^*D+DRD^*)HB=(D^*D+DD^*)HB-DPD^*HB\), and we use again the formula (135), and the fact that \(DPD^*\) is a bounded operator". [P] (3.49), p.399 source: pointwise kernel bounds for \(P,DP,PD^*,DPD^*\) with \((L^{j'}\eta)^{-d}e^{-\frac12\delta_0d}\); so \(DPD^*\) is a sup→sup composite \((\nabla G')Q'^*C'Q'(G'\nabla^*)\). Hence [SI]'s
\[
\Phi_\Delta=\Delta_U(\mathscr A_0+H_0B)-\bigl([Q^*C_\pi-Q^*a](L\eta)^{-1}+\tfrac12DRG'S^T\operatorname{ad}_J^\flat H-\Delta'H+DPD^*H+\mathfrak cH\bigr)D(\mathscr A_0+H_0B)
\]
is a formula of the calculus, with \(\Delta_U\) falling only on \(G_0\) ((3.42) entry 4 through Theorem 3.3; [V] (130) for \(H_0\), c) and \(\Delta^{(2)}\) of zeroth order ([P] (3.136)–(3.137), p.422–423, c: "\(\lvert(\Delta^{(2)}A)(b)\rvert\le O(1)M\alpha_0(L^j\eta)^{-2}\lvert A\rvert\) … the supremum \(\lvert A\rvert\) is taken over several \(j\)-blocks surrounding \(\Delta(y)\)").

### 2.5 \(F=\delta V_\Delta/\delta A'\) term by term

Read on [V] pp.291–292.
- **(85)**: "\(-\sum_{b'}\eta^d\sum_{c_1\in\mathfrak B_k}(L^{j_1}\eta)^d\operatorname{tr}J(b')H(b',c_1)\mathfrak D_2(A';c_1,b)\)" \(=-\mathfrak D_2(A')^T(H^TJ)\). \(H^TJ\) is a fixed block field ([P] p.422: "\(\lvert(H^*J)(b)\rvert\le O(1)M\alpha_0(L^j\eta)^{-3}\)", c). \(\mathfrak D^T\varphi=[L\eta\,\delta C/\delta A(A'')]^Tv\) with \(v=\varphi-H^T[L\eta\,\delta C/\delta A(A'')]^Tv\), the transpose of (68)–(70): a (C3) node, and the linear part \((\delta C^{(2)}/\delta A)^T\varphi=\Delta^{(2)}A'\) is local. No derivative.
- **(88)**: "\(Q^*(QGQ^*)^{-1}(L^{j(\cdot)}\eta)^{-1}D(A')-Q^*a(L^{j(\cdot)}\eta)^{-1}D(A')+\mathfrak D^*(A')(L^{j(\cdot)}\eta)^{-1}(QGQ^*)^{-1}QA'-\mathfrak D^*(A')(L^{j(\cdot)}\eta)^{-1}aQA'\)". Nodes \(C_\pi\), \(Q\), \(Q^*\), \(a\), \(D\), \(\mathfrak D^T\). No derivative.
- **(89)**: \(\mathfrak D^*(L\eta)^{-1}C_\pi(L\eta)^{-1}D-\mathfrak D^*(L\eta)^{-4}D\). No derivative.
- **(90)**: \((1-\mathfrak D^TH^T)\sum_{p\in st(b)}\partial V_0'/\partial A(b)\) at \(A''=A'-HD\). By (39)–(40) (p.284, c: "Here we have used only the first bound (32) on the field \(A\) alone") \(V_0'\) is a holomorphic function of the four bond values. No derivative.
- **(91)–(96)**: the term \(\frac12\langle DA'',\sum i[A'',A'']\rangle\). Variation through the commutator: pointwise in \((DA'',A'')\), then \((1-\mathfrak D^TH^T)\). Variation through \(DA''\): "\(\frac12D^*\sum i[A'',A'']\)" (93), reduced by (94) ("we can use the factor \(\eta\) to replace this derivative by a simple difference operation") and by the Leibniz rule (96) to a local polynomial in the jet \((A'',\nabla A'')\) on neighbouring bonds. The jet of \(A''\) is \((A'-HD,\ \nabla A'-(\nabla H)D)\): the derivative sits on the kernel of \(H\) ((3.133), c) or is a jet component of the variable. The part of \(DA''\) through \(HD\): \(\mathfrak D^T(\nabla H)^T(\dots)\), kernel \(H^T\nabla^T\) (Lemma GP(2), or the pointwise bound (3.133)).
- **\(\delta W/\delta A'\)**: §2.3.

### 2.6 Conclusion on (S-calc)

**(S-calc) holds in the following corrected form, source input; deduction:**

> **(S-calc♯)** \(F=\delta V_\Delta/\delta A'\) and the outputs are finite formulas of the calculus \(\mathcal C\) whose nodes are: the primitives \(G',C',G_0,C_0\) in the sup-input types K1–K3 of §3; \(G_\pi\), \(C_\pi\), \(H\) either with their printed bounds (K4) or built by Lemma GP with \(\Delta'_\pi\) in right form (transposes in left form); \(\Delta'_\pi H\) and \(W\) in the (138)-reduced form; the local holomorphic maps of [CT] §2.4–2.5; the fixed fields \(J\), \(H^TJ\) as pointwise multipliers; the fixed points \(D\) and \((I+\mathfrak R)^{-T}\). The type \(\nabla P\nabla^*\) does not occur. No derivative falls on \(J\) or on any other fixed field. The identity used is \(D^*J=0\); where it is unavailable the right form is the definition.

## 3. Hypothesis (K): what the source prints

| Operator | Printed, checked source input | Form | Used in CT♯ |
|---|---|---|---|
| \(G'\) | (3.42) p.397: \(\lvert G'\lambda\rvert,\lvert\nabla_UG'\lambda\rvert,\lvert G'\nabla_U^*\lambda\rvert,\lvert\Delta_UG'\lambda\rvert\le B_0[(L^j\eta)^2,L^j\eta,L^j\eta,1]e^{-\delta_0d(y,y')}\lvert\lambda\rvert\), \(\operatorname{supp}\lambda\subset\Delta(y')\) | sup→sup, sharp block input: (2.2) after the exchange (2.1) | entries 1–3 (**K1**) |
| \(G'\) Hölder | (3.43): \(\lVert\zeta\nabla G'\lambda\rVert_\beta,\lVert\zeta G'\nabla^*\lambda\rVert_\beta\) from \(\lvert\lambda\rvert\) | sup→Hölder | not needed |
| \(\nabla G'\nabla^*\) | (3.44)–(3.45): from \(\lVert\lambda\rVert_\varepsilon^{\xi'}+\lvert\lambda\rvert\), \(\operatorname{supp}\lambda\subset\tilde\Delta(y')\) | **Hölder→sup; not (2.2)** | **not used** (Lemma PL) |
| \(C'\) | (3.48) p.398 | block kernel | **K1** |
| \(G_0\) | Theorem 3.3, p.399: "satisfies the inequalities (3.42)–(3.47), with \(G'(U)\) replaced by \(G(U)\)" | as for \(G'\) | entries 1–4 and (3.43) (**K2**) |
| \(P,DP,PD^*,DPD^*\) | (3.49) p.399, pointwise | derived from K1 | \(P_1\) row |
| \(C_\pi\) | (3.132) p.422, "let us write only bounds" | block kernel, asserted | **K4** (or Lemma GP) |
| \(C_0=(QG_0Q^*)^{-1}\) | not printed separately; [V] (129)–(130) p.297–298 assert (3.133) and the Laplacian bound for \(H_0\) | asserted | **K3** |
| \(H\) | (3.133) p.422, rate \(\frac12\delta_1\), then "a common, best possible, decay rate … \(\delta_0\)" p.423 | pointwise kernel, block input | **K4** (or Lemma GP) |
| \(\Delta^{(2)}\) | (3.136)–(3.137) | local, zeroth order | local map |
| complex \(U'U\) | p.407: "This way we get all these inequalities for the operator \(G(U'U)\) … Thus Theorem 3.4 is proved, assuming that Theorems 3.1–3.3 hold"; Cor. 3.5–3.6 p.407–408 | K1–K2 on (3.37) | §5.2 |

So: **(K) as stated in [CT] §2.3 is what the source prints for every type used, except \(\nabla P\nabla^*\)**, which is printed only with a Hölder input and which the repaired proof does not use. The exchange of scale factors is printed ([P] p.398, c: "Using Lemma 2.1 in [4] we may replace the factor \((L^j\eta)^\alpha\) by \((L^j\eta)^\beta(L^{j'}\eta)^\gamma\) with \(\beta+\gamma=\alpha\)"); [CT]'s (2.1) is a correct quantitative form, deduction given (BM.3), which The formula gives against [P2] (2.47), (2.57). \(B_0,\delta_0\) depend on \(d,L\) only for \(M\ge M_1\) (Theorem 3.1, p.397, c) and not on \(\{\Omega_j\}\) (p.399, c). Proof level in the source is unchanged from P9♮: Theorems 3.1–3.3 through the sketched walk expansions; (3.132) and K3 asserted.

## 4. The weighted calculus and the proofs, line by line

**[CT] §2.2.** The definition by conjugation must go (E2). With operator norms between weighted norms everything below is literal. The sentence "the weight is never differentiated" is then true by construction.

**Lemma 3.1.** Correct deduction for sup-input kernels. The row sum is \(S(\delta-\lambda)\); under (Geo) the rate after exchange is \(\ge\frac34\delta_0\) and \(S(\frac12\delta_0)\le c_1(\frac12)\) by [P2] (2.58)–(2.59) source input. It does not apply to (3.44) (E1). Transposes: the primitives are symmetric for the bilinear pairing, and (3.42) lists both \(\nabla G\) and \(G\nabla^*\); \(H\) has a pointwise kernel bound. Fine.

**Lemma 3.2.** Correct deduction. One precision: at an interface between layers the neighbours of a bond have scale factors differing by \(L^{\pm1}\), so \(\ell_f\) acquires a factor \(\le L^4\). It is a constant.

**Lemma 3.3.** Correct deduction once stated for norms.

**Lemma 3.4.** Correct deduction. The set form needs no row sum, as claimed.

**Lemma 3.5.** Correct deduction. (C2): Cauchy with margins. (C3): \((I-\partial_X\Psi)DX=\partial_Z\Psi\) and the weighted Neumann series.

**Lemma 4.1.** Item 1 is where E1 bites: "\(\Delta'_\pi G_0\) is a composite" is true only in the right form, \(N=\Delta^R\circ\mathcal G\) (Lemma GP). With that, items 1–3 are correct conditional. The count \(\alpha_J\hat B_\lambda^9\le\frac12\) is reproduced by Lemma GP.

**Lemma 4.2.**  All terms of §2.5 are \(O(m^2)\), including (85) (through \(\mathfrak D_2\)) and \(\delta W/\delta A'\).

**Proposition 4.3 (weighted (189)).** Correct conditional. \(g(t)=e^{w(b)}(L^{j(b)}\eta)^3\,DF(tA')[h](b)\) with \(m_w(h)\le1\) is holomorphic on \(\lvert t\rvert<a_\lambda/m(A')\), bounded by \(\mathsf K_F\), and vanishes at \(0\). (The printed "\(e^wDF(tA')e^{-w}h\)" with \(m_w(h)\le1\) has one weight too many; cosmetic.)

**Theorem CT, Steps 1–6.**
- Step 1: (182)–(184) are as printed on p.307 source input. The equation (180) with the new \(G=(\Delta_a-\Delta^{(2)})^{-1}\) is correct: The formula gives it from (128) (\(\tilde G\Delta_aH_0B=0\) because \(\Delta_aH_0B\in\operatorname{Ran}Q^*\) and \(P_b^*Q^*=0\)).
- Step 2: Schwarz in \(B\). 
- Step 3: \(\lVert\tilde G\,DF(A'_B)\rVert_\lambda\le\frac12\) for \(\lvert B\rvert<r_{CT}\).  The solution of the weighted Neumann series is the true \(\mathfrak a\) because the lattice is finite and \(I+\tilde GDF\) is invertible.
- Step 4: correct; the Hölder row uses (3.43) for \(G_0\) and (3.133) for \(H\), both with sup inputs.
- Step 5: correct for \(\Phi_\Delta\) as a formula (§2.4). The identification with \(\Delta_U\mathscr H\) and \(D^*D\mathscr H\): see §5.3.
- Step 6: correct.

**Where smallness is used.** (i) \(\alpha_J\hat B_\lambda^{10}\le c_S\): the background's regularity constant times \(M\). (ii) \(m(A')<a_\lambda=c_S\hat B_\lambda^{-2}\). (iii) \(\lvert B\rvert_\infty<r_{CT}=c\hat B_\lambda^{-q}\). All three are absolute (functions of \(d,L,B_0,\delta_0,c_1(\frac12),r_{\rm loc}\) and the local-map constants). None depends on \(k\), the number of levels, the volume, \(\eta\), or \(\{\Omega_j\}\). The argument does not require explicit exponents \(p,q,p_F\); only polynomiality is used.

## 5. Backgrounds

### 5.1 Real critical background, complex data conditional

This is the case we use under (Conv-CR) (the representation convention), and it is the cleanest: (K) is needed at the real background only (K1–K4 as printed); \(\mathscr H\) is Prop. 9's function by the identity theorem in \(B\) ([SI] P9♮, correct); \(RD^*\mathscr H=0\) and (I1)–(I3) hold for all \(\lvert B\rvert<r_{CT}\), so \(\Phi_\Delta=\Delta_U\mathscr H\) and \(\Phi_{D^*D}=D^*D\mathscr H\). All of [CT] stands, in the six rows \(0,1,\beta,P_1,D^*D,\Delta\).

### 5.2 Complex backgrounds conditional

K1–K2 on (3.37) are Theorem 3.4 and Cor. 3.5–3.6 (c for the statement). K3 for \(C_0(U'U)\) follows by a Neumann series around the real \(U\) from K2 (not written out; additional assumption). K4 is **not** printed for complex backgrounds or for an independent \(\mathbf J\): \(H\) and \(C_\pi\) come from Lemma GP. \(\mathscr H\) is defined by (179)–(180) without the \(J\)-term ([I] p.273, c: "we replace the configurations \(U_{k+1},J_{k+1}\) occurring in operators there by the configurations \(\mathbf U,\mathbf J\)").

### 5.3 The analytic-continuation step ([CT] §9 doubt 4) — settled

**(a) \(RD^*H=0\) needs no continuation when \(J=J(U)\).** It follows algebraically from: \(\Delta_\pi=(I-D\Lambda)^T\Delta(I-D\Lambda)\) ((3.119)); \((I-D\Lambda)D\mu=0\) for \(Q'\mu=0\) (definition of \(R\)); \(QD\mu=0\) for \(Q'\mu=0\) ([P] p.420, c: "we have used (3.115) and the condition \(Q'\lambda=0\). They imply that \(QA\) is gauge invariant with respect to gauge transformations satisfying this condition"). Then \(G_\pi^{-1}D\mu=D(D^*D\mu)\), so \(G_\pi DR=DG'R\), and \(RD^*G_\pi Q^*=(QDG'R)^T=0\) since \(Q'G'R=0\). These are identities between the formula-defined operators and hold at complex \(U'U\) with bilinear transposes. Hence (I1), (I2) hold and **\(\Phi_\Delta=\Delta_U\mathscr H\) at every background with \(J=J(U)\)**. Level deduction given the three (c) items; the equivalence (3.119) ⇔ (3.120) at complex \(U\) is the continuation of a polynomial identity.

**(b) \(RD^*\mathscr H=0\) is not available off the real critical set.** [SI] Theorem S(5) and [CT] §6.2 are wrong on this point. So \(\Phi_{D^*D}\) is a representation only there. Conjecturally, \(RD^*\mathscr H=O(J\cdot\mathscr H)\ne0\) (the functional without its linear term is not gauge invariant), but did not compute it.

**(c) Independent \(\mathbf J\).** Then \(RD^*H(\mathbf U,\mathbf J)=0\) is not available either, and \(\Phi_\Delta\) is the definition of the second-order row. This is what [I] needs: any analytic extension of (3.7) that agrees on the real slice serves ([I] p.272–273). If Remark 2.4(i) is accepted, the literal \(\Delta_U\mathscr H\) is bounded directly and (c) becomes moot.

## 6. The statement the construction may cite

**Setting.** \(\{\Omega_j\}_{j\le k}\) as in [V] (1)/[P2] (2.2), layer separation \(>RML^j\eta\); \(d\) the distance [P2] (2.46); \(\mathcal W_\lambda\) the functions \(w=\lambda\rho\) on \(\mathfrak B\), \(\rho\) 1-Lipschitz for \(d\), extended block-constantly. Weighted norms \(\lvert f\rvert_{(\alpha),w}=\sup_be^{w(b)}(L^{j(b)}\eta)^{-\alpha}\lvert f(b)\rvert\), \(m_w=\max\{\lvert\cdot\rvert_{(-1),w},\lvert\nabla\cdot\rvert_{(-2),w}\}\), \(\lvert b\rvert_{{\rm dat},w}=\sup_ce^{w(c)}\lvert b(c)\rvert\). For a linear map, \(\lVert T\rVert_\lambda\) is the supremum over \(w\in\mathcal W_\lambda\) of its operator norm between the weighted norms.

- **(Geo)** [P2] (2.59) at \(\alpha=\frac12\): \(\frac14\delta_0RM>2d\log c_0(\frac14)+1\), \(c_0(a)=\coth(a\delta_0/2)\); and \(\delta_0RM\ge16\log L\).
- **(K♯)** For the background considered, with constants \((B_0,\delta_0)\):
 K1. \(G'\): [P] (3.42) entries 1–3; \(C'\): (3.48).
 K2. \(G_0\): (3.42) entries 1–4 and (3.43) (Theorem 3.3).
 K3. \(C_0=(QG_0Q^*)^{-1}\): the bound (3.132).
 K4 (real backgrounds with \(J=J(U)\); otherwise replaced by Lemma GP): \(H\): (3.133); \(C_\pi\): (3.132).
- **(S-calc♯)** of §2.6; **(Loc)** of [CT] §2.5.
- **(Small)** \(\alpha_J\hat B_\lambda^{10}\le c_S\), where \(\hat B_\lambda=e^{\lambda r_{\rm loc}}L^4c_1(\tfrac12)B_0\), \(c_1(\frac12)=12c_0(\frac14)^d\).

> **Theorem CT♯.** Assume (Geo), (K♯), (S-calc♯), (Loc), (Small), and let \(0<\lambda\le\frac14\delta_0\). There are \(K_{CT}=C\hat B_\lambda^{p}\), \(r_{CT}=c\hat B_\lambda^{-q}\) (\(p,q\) fixed integers; \(c,C\) depending on \(d,L\), the local-map constants and the formula only) such that for every complex block datum \(B\) with \(\lvert B\rvert_\infty<r_{CT}\), every \(w\in\mathcal W_\lambda\), every datum \(b\), every \(y\) and \(x\in\Delta(y)\), \(y\in\Lambda_j\):
> \[
> e^{w(y)}\bigl\lvert D\mathscr H(B)[b](x)\bigr\rvert_\nu\le K_{CT}\,\mathfrak w_\nu(j)\,\lvert b\rvert_{{\rm dat},w},
> \]
> for \(\nu\in\{0,1,\beta,P_1,\Delta\}\) with \(\mathfrak w_\nu=[(L^j\eta)^{-1},(L^j\eta)^{-2},(\lVert\zeta\rVert_\beta^\xi+\lvert\zeta\rvert)(L^j\eta)^{-2-\beta},(L^j\eta)^{-3},(L^j\eta)^{-3}]\), where the row \(\Delta\) is the derivative of the representation output \(\Phi_\Delta\) (§2.4) and \(P_1=DPD^*\). Here \(\mathscr H\) is the function defined by [V] (179)–(180) (without the \(J\)-term).
> 1. **Kernel form, all distances:** \(\lvert\partial\mathscr H(B)(x)/\partial B(c)\rvert_\nu\le K_{CT}\mathfrak w_\nu e^{-\lambda d(y,y(c))}\).
> 2. **Set form, no row sum:** if \(b\) is supported in the blocks of \(S\), \(\lvert D\mathscr H(B)[b](x)\rvert_\nu\le K_{CT}\mathfrak w_\nu e^{-\lambda d(y,S)}\lvert b\rvert_\infty\).
> 3. **Finite differences:** if also \(\lvert B+b\rvert_\infty<r_{CT}\), \(\lvert\mathscr H(B+b)(x)-\mathscr H(B)(x)\rvert_\nu\le K_{CT}\mathfrak w_\nu e^{-\lambda d(y,S)}\lvert b\rvert_\infty\).
> 4. **Identification.** (i) If \(J=J(U)\) (real or complex background): the row \(\Delta\) is \(\Delta_UD\mathscr H(B)[b]\). (ii) If the background is real and critical (\(P_0^*J=0\); in particular \(U_0=U_k(V_0)\), \(V_0\) satisfying [V] (7)): \(\mathscr H\) is the function of [V] Prop. 9, for real \(B\) the Landau-gauge minimiser response, and the same bound holds for the sixth row \(\nu=D^*D\), weight \((L^j\eta)^{-3}\).
> 5. **Weighted (189):** \(\lVert DF(A')\rVert_{\lambda;\,m\to(-3)}\le(\mathsf K_F/a_\lambda)\,m(A')\) for \(m(A')<a_\lambda=c_S\hat B_\lambda^{-2}\).
> 6. **Source term (CT-J).** If the equation is \(\mathscr A_0=\mathfrak j+\tilde G\Delta^{(2)}H_0B-\tilde GF(\mathscr A_0+H_0B)\) with a jet field \(\mathfrak j\), \(m(\mathfrak j)\le\frac14\varepsilon_4\), the solution is holomorphic in \((\mathfrak j,B)\) and \(\lvert D_{\mathfrak j}\mathscr H[\delta\mathfrak j]\rvert_{m,w}\le K_{CT}m_w(\delta\mathfrak j)\).
> All constants are uniform in \(\{\Omega_j\}\), \(k\), the number of levels, the volume, \(\eta\), \(B\) and the background in the class where (K♯), (Small) hold.
> **Variant for the \(s\)-deformed package** ([CT] §6.3). With the deformed primitives of [DN] Theorem W, (W-ms) read for the sup-input types K1–K2 (including \(P\nabla^*\) as separate operators) and their adjoints, \(\Delta'_\pi(s)\) defined by the right form, and \((B_0,\delta_0)\to(\hat B,\frac14\delta_0)\), \(\hat B=2n_0B_se^{2^d\kappa}\): the same statement with \(\lambda\le\frac1{16}\delta_0\), uniformly on the polydisc \(\lvert s_t\rvert\le e^\kappa\), under [P2] (2.59) at \(\alpha=\frac18\) and \(\delta_0RM\ge64\log L\); rows \(0,1,\beta,P_1,\Delta\) (representation outputs).

**Hypotheses: conditional** on (K♯) (printed statements; proofs in the source sketched for Theorems 3.1–3.3, asserted for (3.132) and K3), (Geo), and on [SI] Theorem S(1)–(4) (justified in [REF]; Use them as [CT] does). (S-calc♯) is now source input; deduction. The proof is [CT] §§3–5 with Lemma GP replacing the first item of Lemma 4.1 and norms replacing conjugations. Item 6 is Step 3 with one more inhomogeneity: \((I+\tilde GDF)\,\delta\mathscr A_0=\delta\mathfrak j\). The \(P_1\) row: \(DPD^*\) is \(\lambda\)-bounded from \((-1)\) to \((-3)\) by (3.49).

## 7. Consumers

| Consumer | What it uses (checked) | CT♯ delivers | Status |
|---|---|---|---|
| [V] (190) | kernel, five rows, any \(B\), complex regular \(U\) | item 1; at complex \(U\) without the \(D^*D\) row | **covered** conditional, with E3 |
| [I] (3.9), p.271 source: "\(\lvert\delta\mathbf H_j\rvert\le B_3\exp(-\frac12\delta_0{\rm dist}^{(\xi)}(X,\square)-\frac12\delta_0M(L^j\eta)^{-1})\times2L^j\eta\lvert\zeta_\square\mathbf H_k(B')\rvert\) on \(X\), and the same for derivatives and the second order operators", for \({\rm dist}^{(\xi)}(X,\square)\ge M(L^j\eta)^{-1}\); norms (3.14) p.272: "\(\lvert\mathbf A\rvert,\lvert P_1\mathbf A\rvert,\lvert\nabla^\xi_{\mathbf U}\mathbf A\rvert,\lvert\Delta^\xi_{\mathbf U}\mathbf A\rvert<\alpha_2\)"; background \((\mathbf U,\mathbf J)\) complex with \(\mathbf J\) independent (p.272–273) | item 2 with \(S\) = blocks meeting \(\operatorname{supp}\zeta_\square\), base point \(B(t)\); rows \(0,P_1,1,\Delta\); rate \(\frac12\lambda=\frac18\delta_0\) in each of the two exponents | **covered** conditional. Needs: the \(P_1\) row (E4); at complex \((\mathbf U,\mathbf J)\) Lemma GP and the convention of Remark 2.4(ii); the row \(\Delta\) is \(\Phi_\Delta\) unless Remark 2.4(i) is accepted. Homogeneous geometry. |
| [III] (3.6)–(3.8), p.266 source input | \(\lvert\mathbf H_{k,\square}\rvert,\lvert\nabla\mathbf H_{k,\square}\rvert\le B_3(4\delta_k+\exp(-\delta2M_2R_k)30d^2L^2B_3(1+\beta_0)\varepsilon_k)<\frac1{10}\varepsilon_k\) on \(\square^\sim\); real data, real local minimiser as background | item 3 with \(b_{\rm coll}\) on the boundary layer, plus \(\lvert\mathscr H(b_{\rm bulk})\rvert\le K_{CT}\lvert b_{\rm bulk}\rvert\) | **covered** conditional if \(\lambda\cdot2M_2\ge1\) (\(\delta_0M_2\ge2\)), \(80K_{CT}A_1\le A_0\), \(20K_{CT}\cdot30d^2L^2B_3(1+\beta_0)e^{-R_k}\le1\), \(O(\varepsilon_k)<r_{CT}\). additional assumption: that the local determining set \(\mathbf B_k(\square^{\sim4})\) is of [V]-type and that \(d(\square^\sim,\text{layer})\ge2M_2R_k\) (the local sequence occupies a strip \(\le2R_1M_1\)). |
| [III] (3.17)–(3.19), p.268 source input | \(\mathbf H_{k+1,\square'}\le B_3\exp(-\delta LM_2R_{k+1})44d^2B_3\varepsilon_{k+1}\) on \(\square'^{\sim2}\) | item 3 with \(B=0\) | **covered** conditional, \(\delta_0LM_2\ge4\) |
| R^loc ((M3) of `Local test construction`), "complex (3.19)" | (3.17)–(3.19) with complex data relative to the real centre | item 3 at a real critical background with complex \(b\) (§5.1) | **covered** conditional, given (Conv-CR). The re-derivation of [III] §3 for R^loc is a separate task. |
| [MS] AF.1 (BM.7) | per-layer \(\gamma\); five rows and the (3.14) combinations; base point \(B_0\ne0\) | item 2 with \(S\) = layer \(k\) and (BM.3): \(\gamma=\lambda RM\), no row sum | **covered** conditional, \(\delta_0RM\ge4\gamma\) and (Geo) |
| [MS] AF.1 (BM.8)–(BM.10) | weighted contraction for the prepared map | the \(s\)-variant | **covered** conditional on (W-ms) for the sup-input types, with the right-form definition. The sketch (BM.8)–(BM.9) omitted the nested fixed points and the derivative placement. |
| [UPD] AO (JI.33)–(JI.37) | (JI.34): kernel form with some \(\delta>0\); (JI.36): part of the rate pays \(\sqrt{1+k-n}\) | items 1–2 composed with the local map \(z\mapsto B'(z)\) | **covered** conditional |
| B-03 (S3), far carriers | as [I] (3.9) | as above | **covered** conditional |
| B-03 locality theorem | does not use (190) ([LA] Lemma 2.1; `Projected coupling hypotheses` l.83) | optional improvement | [CT]'s correction of the representation convention is right (source input; by reading) |
| [Deep retained tags and boundary rotations] (H-dec) | §8 | Corollary HD, not the literal premise | **not covered as stated** |
| other (190) citations in [MS] | l.18138 confirms the four norms of (3.14); the rest not checked here | — | not checked |

## 8. (H-dec)

### 8.1 What [Deep retained tags and boundary rotations] assumes, and why CT does not give it

[Deep retained tags and boundary rotations] §5.1: \(\mathcal W^{Lan}(\Phi):=e^{i\eta H''_k(\Phi)}U_{1,2}(\Phi)\), and for \(\Phi,\Phi'\) with exposed data \(\varepsilon\)-close, on a hidden block \(B\) of old layer \(j\): \(h_j\lvert\mathcal H\rvert_B+h_j^2\lvert\nabla\mathcal H\rvert_B\le K_o\varepsilon e^{-\delta_od_{old}(B,\text{exposed})}\), \(e^{i\eta\mathcal H}\mathcal W^{Lan}(\Phi):=\mathcal W^{Lan}(\Phi')\) on \(B\). Its justification: "on a hidden block \(U_{1,2}=U_2\) is fixed, so \(\mathcal H\) is the difference of two Landau responses relative to the same reference".

[LFR II] p.370 source: (1.53) "\(U_{1,2}=U_1\) on \(\Omega''^\sim_{h+1}\), \(U_2\) on \((\Omega''^\sim_{h+1})^c\)"; "In the configuration \(U_{1,2}\) the arguments are separated completely across the boundary \(\partial\Omega''^\sim_{h+1}\)"; (1.54) "\(U^0_k=(\exp i\eta\mathbf H''_k(\mathbf G''_kJ_{1,2},H''_{1,k}\tilde Q(\eta\mathbf A_0)\restriction_{Z''_k\cap\Omega''^{\sim2}_{h+1}})U_{1,2})^{(u^0_k)^{-1}}\)"; "The field \(J_{1,2}\) is not localized". p.371 source: (1.55), (1.57): \(U_1\) is built on \(U_{k,\Lambda}\), hence on the current data.

So \(H''_k(\Phi)\) is the Landau-gauge field of the old configuration **relative to the whole glued background \(U_{1,2}(\Phi)\)**, which is not critical (source \(\mathbf G''_kJ_{1,2}\)) and which changes with \(\Phi\) on \(\Omega''^\sim_{h+1}\). The two backgrounds \(U_{1,2}(\Phi)\), \(U_{1,2}(\Phi')\) agree on hidden blocks only. The Landau condition \(R(U_{1,2})D^*_{U_{1,2}}H''=0\), the operators \(\mathbf G''_k,H''_{1,k}\), and \(J_{1,2}\) all depend non-locally on the background. Therefore \(\mathcal H\) of (H-dec) contains: (i) the response to the data change, at a non-critical background; (ii) the response to the change of the source \(J_{1,2}\); (iii) the response to the change of the background on the exposed side. CT♯ items 3 and 6 give (i) and (ii). **Nothing in [CT] or here gives (iii).** deduction for the diagnosis.

### 8.2 The version that CT does cover

By [LFR II] (1.61) (quoted in [Deep retained tags and boundary rotations] §2.5 in the source; not assumed here), \(U^0_k=U(\mathbf B''_k(Y_1),M'(U^0_k))\): the old configuration is the minimiser on the old determining set \(\mathfrak B^0=\mathbf B''_k(Y_1)\) with its own data \(\mathfrak D\). On hidden blocks the data are the frozen \(V''\).

> **Corollary HD conditional.** Let \(\mathfrak B^0\) be a determining set of [V]-type (1) with distance \(d_{old}\) = [P2] (2.46) for its own sequence, and let \(W_0\) be a real minimiser on \(\mathfrak B^0\) satisfying the hypotheses of CT♯(4)(ii). Let \(b\) be a complex datum on \(\mathfrak B^0\), \(\lvert b\rvert_\infty<r_{CT}\), vanishing on a set \(\mathcal H\!id\) of blocks, and \(S\) the set of blocks carrying \(b\). Then the reconstruction of the data \(e^{ib}\mathfrak D(W_0)\) relative to \(W_0\) (Conv-CR) is \((e^{i\eta\mathscr H(b)}W_0)^{u}\) with \(\mathscr H(b)\) holomorphic in \(b\), and on every block \(\Delta(y)\), \(y\) in old layer \(j\):
> \[
> h_j\lvert\mathscr H(b)\rvert+h_j^2\lvert\nabla\mathscr H(b)\rvert+h_j^3\lvert\Delta\mathscr H(b)\rvert+h_j^3\lvert D^*D\mathscr H(b)\rvert\le K_{CT}\,e^{-\lambda d_{old}(y,S)}\lvert b\rvert_\infty,\qquad\lambda\le\tfrac14\delta_0,
> \]
> and for a holomorphic family \(b(z)\) and every \(w\in\mathcal W_\lambda\) (for \(d_{old}\)): \(e^{w(y)}\lvert\partial_i\mathscr H(b(z))(x)\rvert_\nu\le K_{CT}\mathfrak w_\nu\lvert\partial_ib(z)\rvert_{{\rm dat},w}\) (the main inequality of CT♯ applied to the datum \(\partial_ib\)). In particular, for \(y\in\mathcal H\!id\) at layer distance \(n\) from \(S\): the factor is \(\le e^{-\lambda RM(n-1)_+}\).

*Proof.* CT♯ item 3 at base point \(0\) and \(\mathscr H(0)=0\); item 4(ii) for the identification and the six rows. \(\square\)

This is the statement [Deep retained tags and boundary rotations] §10 item 1 asks for ("the response to data changes supported on a sub-region, with the decay in the old scaled distance"). Its premises: (K♯) and (Geo) for the old geometry, and that \(\mathfrak B^0\) (a joined determining set, [III] (2.14)) is of [V]-type — the premise (P9-ms) that [Deep retained tags and boundary rotations] already carries at additional assumption.

### 8.3 Using HD in [Deep retained tags and boundary rotations] Theorem H additional assumption

Replace the Landau-framed chain by the base-relative family \(\mathcal W^\natural(\Phi):=e^{i\eta\mathscr H_{W_0}(b(\Phi))}W_0^\natural\), \(W_0^\natural=\mathcal W^{Lan}(z_0)\), \(b(\Phi)\) = the exposed data of the old configuration relative to their value at \(z_0\) (rotated to the frame of \(W_0^\natural\); zero on hidden blocks). Then:
1. \(\mathcal W^\natural\) is holomorphic in \(\Phi\) wherever \(b(\Phi)\) is, and lies in the old space by the six-row bound of HD with \(\lambda=0\) (this replaces (CH-L) by holomorphy and sup-smallness of the *data map* only);
2. for real \(z\) the actual configuration is \(\mathcal W(z)=(\mathcal W^\natural(z))^{\mathfrak r^\natural(z)}\), because both are minimisers with the same data up to the rotation \(\mathfrak r(z_0)\) at the determining sites (\(Q(\eta\mathscr H)=b\) is exact, [V] (44)–(48));
3. on a hidden block, \(\mathfrak r^\natural(z)\mathfrak r(z_0)^{-1}\) is the block-local axial frame map ([Deep retained tags and boundary rotations] Lemma F(ii), (Fr-Lip)) of \(e^{i\eta\operatorname{Ad}\mathscr H}\mathcal W(z_0)\vert_B\) relative to \(U_2\vert_B\), and \(\mathcal W(z_0)\vert_B\) is already in that frame; so \(\lvert\lambda^\natural(z)(x)\rvert\le C_aK_{CT}e^{-\lambda d_{old}(B,S)}\lvert b(z)\rvert_\infty\).

This gives [Deep retained tags and boundary rotations] Theorem H(2)–(3) with \(K_o=K_{CT}\), \(\delta_o=\lambda\). Steps 1–3 require compatibility with [Deep retained tags and boundary rotations]'s full proof or against [LFR II] (1.59)–(1.65); that belongs to the analysis of [Deep retained tags and boundary rotations]. Two things are needed there: the data map \(\Phi\mapsto b(\Phi)\) is holomorphic on the new space with \(\lvert b\rvert_\infty<r_{CT}\) (a weakening of (CH-L)); and Lemma F/(Fr-Lip) with the reference \(W_0\vert_B\).

A **background-variation theorem (CT-U)**: for a perturbation \(U\to e^{i\eta a}U\) with \(a\) supported in \(S\), \(\lvert\partial_a\mathscr H(B;U)(x)\rvert_\nu\le K\,e^{-\lambda d(y,S)}\lvert a\rvert\) in the norms (3.37)–(3.38). Route: every node depends on \(a\) through a vertex supported near \(S\) — for the primitives by [P] (3.82)–(3.86) (p.407, c: "\(\Delta_a(U'U)=\Delta_a(U)-V_3(A)-P_1(A)-P_2(A)\)", \(V_3\) "a local differential operator of the first order", \(P_1(A)\) "non-local bounded", \(P_2\) "semi-local"), for local maps trivially — so \(\partial_a\mathscr H\) is a sum of terms (weighted-bounded chain)∘(field supported near \(S\)), and Lemma 3.4(2) applies; the fixed points are handled as in (C3). The non-local \(P_1(A)\) (through \(R(U'U)\)) must be expanded once more. This remains an assumption. With CT-U, CT-J and item 3, the literal (H-dec) follows with decay in the distance to \(\Omega''^\sim_{h+1}\cup\) exposed blocks.

**Definite answer.** CT (also CT♯) does **not** deliver (H-dec) as stated in [Deep retained tags and boundary rotations] §5.1. It delivers Corollary HD, which is the form requested in [Deep retained tags and boundary rotations] §10 item 1 and is sufficient for Theorem H under the substitution of §8.3, at status conditional for HD and additional assumption for the substitution.

## 9. Parameter conditions and the representation convention

Let \(\gamma_\star:=4\log L+\log2+2\) (\(=5.466\) for \(L=2\)) and \(c_0(a)=\coth(a\delta_0/2)\) ([P2] p.233, c: "\(c_0(\alpha)=\sum_{z\in\mathbb Z}e^{-\alpha\delta_0\lvert z\rvert}\)", (2.59) "\(\frac12\alpha\delta_0RM>2d\log c_0(\frac12\alpha)+1\)", \(c_1(\alpha)=12c_0^d(\frac12\alpha)\)).

| Use | Conditions on \(\delta_0RM\) | \(d=4,L=2\), \(\delta_0=1\) | \(\delta_0=0.25\) |
|---|---|---|---|
| CT♯, true package | \(>4(2d\log c_0(\frac14)+1)\); \(\ge16\log L\) | \(>70.7\); \(\ge11.1\) | \(>114.9\) |
| (BM.7), \(\gamma>\gamma_\star\) | \(>4\gamma_\star\) | \(>21.9\) | \(>21.9\) |
| \(s\)-variant | \(>16(2d\log c_0(\frac1{16})+1)\); \(\ge64\log L\) | \(>459.7\); \(\ge44.4\) | \(>637.1\) |
| (BM.10), \(\gamma>\gamma_\star\) | \(>16\gamma_\star\) | \(>87.5\) | \(>87.5\) |

Further conditions:
- \(\delta_0M_2\ge2\) ([III] (3.7); 8 with margin), \(\delta_0LM_2\ge4\) ([III] (3.18)).
- \(80K_{CT}A_1\le A_0\) and \(600d^2L^2B_3(1+\beta_0)K_{CT}e^{-R_k}\le1\) in [III] (3.7); the analogous condition in (3.19). These replace the source's "\(A_1/A_0\) and \(\gamma\) sufficiently small" with \(B_3\to K_{CT}\).
- Ceilings: \(\alpha_J(e^{\lambda r_{\rm loc}}L^4c_1(\frac12)B_0)^{10}\le c_S\) and data \(<r_{CT}\); for prepared maps \(\alpha_J(e^{\lambda r_{\rm loc}}L^4c_1(\frac18)\cdot2n_0B_se^{2^d\kappa})^{10}\le c_S\). The second is tighter than the representation convention's ceiling by the factor \((e^{\lambda r_{\rm loc}}L^4c_1(\frac18))^{10}\); note \(c_1(\frac18)=12\coth(\delta_0/32)^4\approx1.3\cdot10^7\) at \(\delta_0=1\).

**Consistency with the representation convention's order** \(d,L\to\kappa\to M\to C_0,C_1\to g\)-ceilings: yes. \(B_0,\delta_0\) depend on \(d,L\) only (Theorem 3.1, c) and not on \(R\), \(M\ge M_1\) or the sequence; [P] p.408 (c) takes "\(R_0,M_0\) of smallest possible numbers" for the local propagators and \(M=KR_0M_0\) larger. So all conditions on \(\delta_0RM\) and \(\delta_0M_2\) are conditions on the geometric constants \(R_1,M_1,M_2\), fixed right after \(d,L\) and before \(\kappa\) and the tile size \(M\) (\(M\ge c_dL^2M_1\), \(M_1<M_2<M\)); they raise \(M_1\) or \(R_1\), which raises the lower bound on \(M\) only. \(K_{CT}\) is absolute, so \(A_0/A_1\ge80K_{CT}\) sits with \(C_0,C_1\). The ceilings come last. No circularity. deduction for the logic; The argument assumes whether some other proposition imposes an *upper* bound on \(R_1M_1\) or \(M_2\).
