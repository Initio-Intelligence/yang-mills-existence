# Source operators for the deformed reconstruction

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

## 2. The calculus nodes of (179)–(180) (list asked for in [DN] §10.4, step 1)

The **package** is \(\mathfrak P=(G',C',G_0,C_0)\) together with their transposes. It satisfies [P]'s inequalities (3.42)–(3.49) and (3.132), each with \(B_0\to B\ge1\) and \(\delta_0\to\delta\), where \(\delta RM\) is large enough for Lemma 2.1 of [P2].

The **derived nodes** are defined *by formula* from the package and local maps. The fourth column gives the crude norm in powers of \(B\). Here \(\alpha_J:=O(1)M\alpha_0\,(+\alpha_1)\) measures the smallness of \(J\) and of \(U'\).

| Node | Formula | Source | Norm |
|---|---|---|---|
| \(P,\ R\) | \(P=G'Q'^*C'Q'G'\), \(R=I-P\) | [P] (3.25), p.415 | \(B^3\) |
| \(\Delta'_\pi\) | quadratic form (3.120): \(J\)-weighted commutators of \(A\), \(G'RD^*A\), \(DG'RD^*A\); derivatives moved onto neighbours as in (3.131) | [P] (3.120), (3.131) (text, garbled) | \(\alpha_JB^{8}\), as a form additional assumption |
| \(G_\pi\) | \(\sum_nG_0(\Delta'_\pi G_0)^n\) | [P] (3.130) | \(2B\) if \(\alpha_JB^9\le c\) |
| \(C_\pi\) | \(C_0\sum_n(-QG_0\Delta'_\pi G_\pi Q^*C_0)^n\) | from \(QG_\pi Q^*=QG_0Q^*+QG_0\Delta'_\pi G_\pi Q^*\) | \(2B\) |
| \(H,\ H_0\) | \(G_\pi Q^*C_\pi(L\eta)^{-1}\), \(G_0Q^*C_0(L\eta)^{-1}\) | [P] (3.126), [V] (129) | \(B^2\) |
| \(\Delta^{(2)}\) | local in \(A\), coefficient field \(H^*J\) | [P] (3.136)–(3.137) | \(\alpha_JB^2\) |
| \(G\) (new), \(C\) | \(\sum_nG_0(\Delta^{(2)}G_0)^n\), Neumann as for \(C_\pi\) | [V] p.306 | \(2B\) |
| \(\tilde G\) | \(G-GQ^*CQG\) | [V] p.300 | \(B^3\) |
| \(D(A')\) | fixed point of \(X\mapsto C_j(L^j\eta A'-L^j\eta HX)\) | [V] (50) | \(4C_2m^2\) |
| \(\mathfrak D\) | \((I+\mathfrak R)^{-1}L\eta\,\frac{\delta C}{\delta A}(A'-HD)\), \(\mathfrak R=L\eta\langle\frac{\delta C}{\delta A},H\rangle\) | [V] (68)–(70) | \(\le cm\) |
| \(\mathscr R\) ("\(\Delta H\)") | \(Q^*C_\pi(L\eta)^{-1}-Q^*a(L\eta)^{-1}+\Delta'_\pi H\) | (137) and \(\Delta=\Delta_\pi+\Delta'_\pi\) | \(B^{10}\alpha_J+B\) |
| \(\delta V_\Delta/\delta A'\) | (85), (88)–(90), (93)–(96) with \(\Delta_\pi H\to\mathscr R-\Delta'_\pi H\), plus \(\delta W/\delta A'\) of Lemma 3.1 | [V] pp.291–292 | \(C_4\le cB\) on \(m\le cB^{-2}\) |

The local holomorphic maps are \(C_j\), \(\delta C_j/\delta A\) and its transpose, \(V'_0\) and \(\partial V'_0/\partial A\) (bound (40)), \(J\), \(\mathfrak c\) (the zero-order curvature term of (135)), \(\Delta'\) ((3.10), local), \(Q,Q^*,a\), and the commutator identities (94)–(96). Those identities are pointwise algebraic facts about lattice covariant derivatives, so they hold for any complex fields.

Here \(m(A')=\max\{\lvert A'\rvert_{(-1)},\lvert\nabla A'\rvert_{(-2)}\}\).

The exponents in the last column are a crude product count, not optimized. Only their polynomiality is used. The structure of \(\Delta'_\pi\) is read from a damaged source, hence additional assumption for its exponent.

## 3. Theorem S: [V] §§C–G re-run for an arbitrary package

### 3.1 The correction term

**Lemma 3.1 (deduction; given (138)).** \(V_\Delta=V+W\) with \(W(A')=-\langle A',\Delta'_\pi HD(A')\rangle\).

By (138),
\[
W(A')=-\tfrac12\bigl\langle i[(G'RD^*A')(b_-)+R_b(G'RD^*A')(b_+),(HD(A'))conditional],J\bigr\rangle ,
\]
and \(\lvert\delta W/\delta A'\rvert_{(-3)}\le c\,\alpha_JB^{6}m^2\) for \(m\le cB^{-2}\).

*Proof.* (74) with \(\Delta\) in place of \(\Delta_\pi\) differs from (80) by \(-\langle A',\Delta'_\pi HD\rangle+\frac12\langle HD,\Delta'_\pi HD\rangle\). By (138) with \(A=HD\), the second term contains \(G'RD^*HD=0\), so it vanishes. The derivative has two pieces. The first is \((G'RD^*)^T\) applied to \(i[HD,J]\); it has weight \((L\eta)^{-4}\varepsilon\), and \((G'RD^*)^T\) maps it to weight \((L\eta)^{-3}\), giving \(\le cB^4\cdot\alpha_JB^2\cdot4C_2m^2\). The second is \(\mathfrak D^*H^*\) applied to \(i[G'RD^*A',J]\), which is \(\le cm\cdot B^2\cdot B^4\alpha_Jm\). \(\square\)

### 3.2 The theorem

**Theorem S.** Fix \(d,L\) and the source constants \(C_2,C_3\) and \(M_1,R_1\). There are \(c_S,C_S>0\) depending only on these such that the following holds. Let \(\mathfrak P\) satisfy §2's bounds with \(B\ge1\), let \(\alpha_JB^{10}\le c_S\), and let the background (real or complex) lie in the domain on which the local maps are defined. Define every node by §2's formulas. Then:

1. **(Prop. 3′)** For \(m(A')<\varepsilon_3:=c_SB^{-2}\), \(D(A')\) exists, is unique in \(\{\lvert X\rvert_\infty<\varepsilon_3/B\}\), is holomorphic, and \(\lvert D\rvert\le4C_2m^2\). The kernel of \(\mathfrak D\) satisfies (73) with \(C_3\varepsilon_3\to cB\,\varepsilon_3\) and rate \(\frac12\delta\).
2. **(Prop. 4′)** \(\delta V_\Delta/\delta A'\) is holomorphic on \(m(A')<a_3:=c_SB^{-2}\) and satisfies \(\lvert\delta V_\Delta/\delta A'\rvert_{(-3)}\le C_4'm^2\) with \(C_4'\le C_SB\).
3. **(Prop. 6′, eq. (180))** Let \(\varepsilon_4=c_SB^{-4}\) and \(r(B)=c_SB^{-6}\). For every \(\mathfrak g^c\)-valued block field \(B\) with \(\lvert B\rvert_\infty<r(B)\), the map \(T(A_0)=\tilde G\Delta^{(2)}H_0B-\tilde G\,\frac{\delta V_\Delta}{\delta A'}(A_0+H_0B)\) is a contraction (factor \(\frac12\)) of \(\{m(A_0)<\varepsilon_4\}\). Its fixed point \(\mathscr A_0(B)\) is holomorphic in \(B\), and in the package when the package depends holomorphically on parameters. It is the uniform limit of \(T^n(0)\).
4. **(Outputs)** Put \(\mathscr H=\mathscr A_0+H_0B-HD(\mathscr A_0+H_0B)\). For \(\lvert B\rvert_\infty<r(B)\):
   - \(\lvert\mathscr H\rvert_{(-1)}\), \(\lvert\nabla\mathscr H\rvert_{(-2)}\) and the Hölder norm are each \(\le C_SB^2\lvert B\rvert_\infty\);
   - the second-order outputs \(\Phi_\Delta\) and \(\Phi_{D^*D}\) **defined in §3.3** are \(\le C_SB^4\lvert B\rvert_\infty=:K(B)\lvert B\rvert_\infty\) in \(\lvert\cdot\rvert_{(-3)}\).
5. **(Agreement)** If \(\mathfrak P\) is the true package of a real or complex background in [P]'s domain, then \(\Phi_\Delta=\Delta_U\mathscr H\) and \(\Phi_{D^*D}=D^*D\mathscr H\).

*Proof.*

(1) This is [V] (51)–(55) and (65)–(73) line by line. The only operator inputs are \(\lvert HX\rvert_{(-1)}\le cB^2\lvert X\rvert\) in (52) and (54), and the kernel bound of \(H\) in (69). The Cauchy steps (53) and (69) need only holomorphy of \(C_j\). The Neumann series (71) needs \(9C_2cB^2\varepsilon_3c_1<\frac12\). The range statement (59)–(62) concerns existence of the variational minimiser and is not needed.

(2) This is [V]'s term list in the source pp.291–292, checked term by term.
- (85) is \(J\cdot H^T\cdot\mathfrak D_2^T\).
- (88)–(89) are taken *in their final form*, which contains \(C_\pi\), \(Q\), \(a\), \(D\), \(\mathfrak D^T\) and not \(\Delta_\pi H\).
- (90) is \((1-\mathfrak D^TH^T)\,\partial V'_0\).
- (93)–(96) are \((1-\mathfrak D^TH^T)\frac12D^*\sum i[A'',A'']\) with \(A''=A'-HD\). The terms in which the derivative acts on \(HD\) use \(\nabla H\). The \(D^*\) of the leading commutator is reduced by the *local* identity (96) to \(O(\lvert\nabla A''\rvert\lvert A''\rvert)\).
- Add Lemma 3.1.

Every nonlocal factor enters through one weighted-sup bound, at most \(B^3\) per term. Every term is \(O(m^2)\) once \(Bm\le c\). So \(C_4'\le C_SB\).

(3) This is [V] (116)–(121) with \(\tilde G\) in place of the operator of (116). We have \(\lvert\tilde G\rvert_{(-3)\to m}\le cB^3\) and \(\lvert H_0B\rvert\le cB^2\lvert B\rvert\le\frac12\varepsilon_4\). The term \(\tilde G\Delta^{(2)}H_0B\) is \(\le c\alpha_JB^7\lvert B\rvert\). The Lipschitz constant, obtained by Cauchy as in (119)–(120), is \(4cB^3C_4'(\frac32\varepsilon_4)\le\frac12\). Holomorphy follows from uniform convergence of holomorphic iterates (as in [V] p.296).

(4) For the first-order bounds: the sup over the ball is \(\le c\varepsilon_4\), and \(\mathscr H(0)=0\) because \(D\), \(\delta V/\delta A'\) and \(\Delta^{(2)}H_0B\) all vanish at \(B=0\). The Schwarz lemma on the ball of radius \(r(B)\) gives the linear bound. The second-order outputs are treated in §3.3.

(5) See §3.3. \(\square\)

### 3.3 Second-order outputs: what fails and the repair

At \(s=1\) the source proves (pp.298–299; (135) holds for any bond field):
\[
\text{(I1)}\quad D^*DHX=\Delta HX-\Delta'HX=[Q^*C_\pi-Q^*a](L\eta)^{-1}X+\Delta'_\pi HX-\Delta'HX ,
\]
\[
\text{(I2)}\quad \Delta_UHX=D^*DHX+DPD^*HX+\mathfrak cHX\quad(\text{since }RD^*H=0\Rightarrow DD^*H=DPD^*H),
\]
\[
\text{(I3)}\quad D^*D\mathscr H=\Delta_U\mathscr H-DPD^*\mathscr H-\mathfrak c\mathscr H\quad(\text{since }RD^*\mathscr H=0).
\]

**These identities fail for a perturbed package.** A deformed \(H(s)\) has no reason to satisfy \(RD^*H(s)=0\), and the \(\Delta_U\)-bound per walk term of \(H\) is not available (F3). So "\(\lvert\Delta_U\mathscr H(B;s)\rvert\)" is *not* controlled by the walk bounds. [DN] Theorem M(1) and Theorem T′ silently assume that it is.

**Repair: define the outputs by the right-hand sides.**
\[
\Phi_\Delta:=\Delta_U(\mathscr A_0+H_0B)-\bigl([Q^*C_\pi-Q^*a](L\eta)^{-1}X+(\Delta'_\pi-\Delta')HX+DPD^*HX+\mathfrak cHX\bigr),\qquad X=D(\mathscr A_0+H_0B),
\]
\[
\Phi_{D^*D}:=\Phi_\Delta-DPD^*\mathscr H-\mathfrak c\mathscr H.
\]

- \(\Delta_U\mathscr A_0=\Delta_U\tilde G[\dots]\) and \(\Delta_UH_0\) need only the Laplacian bound of \(G_0\), which [P] Theorem 3.3 states for \(G_0\) ([V] (130) for \(H_0\)), propagated through the Neumann series for the new \(G\) and through \(\tilde G\).
- The rest uses first-order bounds and (138)/(3.49).
- This gives item (4).

At the true package, (I1)–(I3) hold. The relation \(RD^*\mathscr H=0\) holds at real \(B\) (Landau gauge); at complex \(B\) it follows by the identity theorem. Hence item (5).

**Table of every use of an operator other than through its bound** in [V] §§C–G, (179)–(180):

| Use | Where | Needed for (179)–(180)? | Treatment |
|---|---|---|---|
| \(\Delta_\pi H=(G_\pi^{-1}-Q^*aQ)H\) | (87), (137) | to derive (88)–(89) | deformed system *defined* by the final forms ([DN] already noted this) |
| \(RD^*H=0\), \(RD^*\mathscr H=0\) | (79), (137)–(140), (134)–(136) | second-order outputs | representation outputs (above) |
| \(QHB=B\), \(Q(\eta\mathscr H)=B\) | (45), (48) | no (only to *interpret* \(D\)) | not used. False for \(s\ne1\) and irrelevant there |
| variational equivalence, positivity, uniqueness of the minimiser | §§D–F, (142) | only to identify the \(s=1\) solution with the minimiser at real data | used only at \(s=1\), real \(B\) |
| \(P_0^*J=0\) (criticality) | (178) | absence of the \(J\)-term in (180) | real critical background: source source input. Elsewhere (180) is the *definition* ([I] p.273) |
| gauge covariance, axial↔Landau map | §§A, G | no | — |
| commutator identities (94)–(96), (135) | local | yes | hold for all complex fields |

**Conclusion on (S-struct)(ii).** [II] p.3's assertion ("only these bounds were important") is *true for the fixed-point equations* and *false, as literally stated, for the second-order regularity*. That regularity is identity-based in [V]. Theorem S, with the representation outputs, is the correct form.

## 4. Theorem P9♮: the statement B-03 (CR) needs

**Theorem P9♮.** Let \(\{\Omega_j\}\) be as in [V] (1). Let \(U_0=U_k(V_0)\) be the real minimiser, with \(V_0\) satisfying (7) for \(\varepsilon_1\le\varepsilon_9\). More generally, \(U_0\) may be any real configuration satisfying [V] (14) and (2) and the criticality \(P_0^*(U_0)J=0\). There are constants \(r_9,K_9,\varepsilon_9>0\) depending only on \(d,L,M_1,R_1\) (absolute) such that, for every \(\mathfrak g^c\)-valued \(B\) on \(\mathfrak B_k\) with \(\lvert B\rvert_\infty<r_9\):

1. (179)–(180) have a unique solution with \(m(\mathscr A_0)<\varepsilon_4\). The function \(\mathscr H(B)\) is holomorphic, and equals [V] Proposition 9's function on the common domain. In particular, for real \(B\) it is the Landau-gauge minimiser response.
2. The (19)-type bounds hold:
\[
\lvert\mathscr H(B)\rvert_{(-1)},\ \lvert\nabla\mathscr H(B)\rvert_{(-2)},\ \lVert\zeta\nabla\mathscr H\rVert_{\beta},\ \lvert D^*D\mathscr H(B)\rvert_{(-3)},\ \lvert\Delta_{U_0}\mathscr H(B)\rvert_{(-3)}\ \le\ K_9\lvert B\rvert_\infty.
\]
3. \(Q(\eta\mathscr H(B))=B\) and \(RD^*\mathscr H(B)=0\), i.e. (20)–(21).

We may take \(r_9=c_SB_0^{-6}\) and \(K_9=C_SB_0^4\), where \(B_0\) is [P]'s common constant (Theorem 3.12 and the text after it).

*Proof.* Apply Theorem S to the **true** package of the real background \(U_0\), with \(B=B_0\) and no deformation. Items (1)–(4) follow.

To identify the solution with the minimiser at real \(B\):
- At real \(B\), \(\mathscr A_0=A'_1-H_0B\) for the critical \(A'_1\) satisfies (143), hence (180). This is pp.298–300 and 306: (133) is derived from the variational equation (127), and \(\tilde GJ=GP_0^*J=0\) by criticality.
- It lies in the contraction ball, by [V] (62), (104) and Prop. 6, with \(\varepsilon_1\le\varepsilon_9\).
- So it is *the* fixed point.
- Both functions are holomorphic on the connected ball. They agree on its real points, which form a totally real subspace of maximal dimension (\(\mathfrak g\subset\mathfrak g^c\)). The identity theorem gives (1).

Item (3): \(RD^*\mathscr H=0\) and \(Q(\eta\mathscr H)=B\) hold at real \(B\) and continue analytically. Item (2): Theorem S(4)–(5); at the true package the representation outputs equal \(\Delta_{U_0}\mathscr H\) and \(D^*D\mathscr H\). \(\square\)

**Status conditional, on printed source statements only.** No walk expansion, no deformation and no (W-ms) is used. The inputs are:
- [P] Theorem 3.3 for \(G_0\), including the Laplacian inequality (text p.399). Its proof rests on the sketched Theorem 3.10.
- [P] Theorem 3.12, (3.133) for \(H\) (text p.423).
- [P] (3.49) for \(P\), \(DPD^*\); (3.132) for \(C_0\) and \(C_\pi\). (3.132) is stated "let us write only bounds", i.e. asserted without proof.
- [P] (3.137) for \(\Delta^{(2)}\).
- [V] (130), (137)–(140), (143) and (179)–(180) (source); [V] Props 3 and 4 (proofs, §3); [V] (62), (104) and Prop. 6.
- Lemma 3.1 (deduction; given (138)).

**For the CR note.** This replaces "[V] Proposition 9 used at its own word … Its proof in §G is 'We repeat the whole procedure of Sects. A–E'" (CR §9 item 1) by an explicit re-run, at an absolute radius, with second-order bounds, for complex \(B\) on a real background.

One caveat for the citation. The variable is the block field \(B\) of (20) and (180). Prop. 9 is stated in \(B'=\frac1i\log V'\) (172). The two differ by the factor \(\le2dL\) that CR §9 already records; take \(r_9\) correspondingly smaller.

## 5. (W-ms): complex walk expansions of the four primitives

### 5.1 Localized operators on the complex domain

**Lemma L (deduction; modulo an elementary BCH estimate, sketched).** Let \(U\) be real and satisfy (3.35) with \(O(1)M\alpha_0\le a\). Let \(A'\) satisfy (3.37) and (3.38) for the global sequence with \(\alpha_1\). For \(\square\in\mathscr D\) with its local sequence \(\{\Omega_n(\square)\}\subset\tilde\square^5\) ([P] p.408), take the real gauge transformation \(u\) of (3.35) on the cube containing \(\square^5\). Then \((U'U)^u=e^{i\eta R(u)A'}e^{i\eta A}=e^{i\eta A''}\), where \(A''\in\mathfrak g^c\) satisfies (3.37) with respect to \(U=1\) and \(\{\Omega_n(\square)\}\) with \(\alpha''=c(M\alpha_0+L^2\alpha_1)\).

*Proof.* Let \(A''\) be the BCH combination of \(R(u)A'\) and \(A\). Differences of \(A''\) are controlled through the identities \(D^{U^u}R(u)=R(u)D^U\) and \(D^{U^u}-D^1=i\,\mathrm{ad}A+O(\eta)\). Where the local layer index exceeds the global one by one, the local condition is stricter by \(L\) (resp. \(L^2\) for the gradient); this is [DN] Remark 3.4's factor. \(\square\)

Hence, if \(c(M\alpha_0+L^2\alpha_1)\le a_1\), [P] Corollary 3.5 applies to \(G'_\square,C_\square,G_\square\) on the complex domain. Corollary 3.5 is §B (displayed Neumann series (3.64), (3.67), (3.86), with the bounds (3.63), (3.66), (3.85)) together with [CMP96] for \(U=1\). Gauge covariance (3.33)–(3.34) for real \(u\) and complex \(U'U\) follows by analytic continuation.

Differences of localized operators on two domains (p.412) follow the same way. Subtract the two Neumann series (3.64), each around \(U=1\), term by term. Each difference contains one factor \(G'_{\Omega}(1)-G'_{\Omega'}(1)\), which [CMP95/96] bounds with the exponential factor.

### 5.2 The expansions

**Proposition W♭.** Under the hypotheses of Lemma L, with \(M\) large, the expansions of [P] Theorems 3.7 (\(G'\)), 3.9 (\(C'\)) and 3.10 (\(G_0\)), and the expansion of \(C_0\) asserted with (3.132), hold for \(U'U\). Each term is holomorphic in \(A'\) restricted to \(\bigcup_iX_i^5\). Each satisfies (3.94), (3.99), (3.108) and the corresponding inequalities in all norms of (3.42)–(3.47), with constants changed by a factor \(1+O(\alpha'')\).

**Hypotheses: deduction given those theorems for real \(U\), at the proof level at which [P] states them.** Theorem 3.7: "exactly the same as in … [3], [4], so we will not repeat them". Theorems 3.9 and 3.10: sketches on pp.411–415. (3.132): asserted.

*Proof.* Go through the source construction step by step.
- (3.87) defines \(G'_0,C_0,G_0\) from localized operators. These are defined and bounded on the complex domain by Lemma L.
- (3.88), (3.95), (3.100)–(3.105) and the cancellation on p.415 are algebraic identities in the operators. They use Leibniz rules for covariant derivatives with \(R(U)\) for complex \(U\), and \(P=G'Q'^*C'Q'G'\). They hold wherever the operators are defined.
- The smallness bounds (3.89), the analysis of (3.95), (3.97) and the bounds on \(R\) in (3.105) use only the bounds of the localized operators and of their domain differences (Lemma L), plus [P2] Lemma 2.1.
- The Neumann series (3.96) and (3.106) converge in operator norm. Their sums are the inverses, because \(\Delta_a(U'U)\), \(\Delta'_a(U'U)\) and \(Q'G'^2Q'^*(U'U)\) are invertible by §B. On a finite lattice a right inverse is the inverse.
- Positivity (Thm 3.11) is not used (F5).

An alternative route: both sides of each expansion identity are holomorphic in \(A'\) (uniform convergence) and agree at real \(A'\). There \(U'U\) satisfies (3.35) with \(\alpha_0+O(\alpha_1/M)\) (BCH). The identity theorem then applies. \(\square\)

### 5.3 Counting constants (Lemma W0(d))

These follow from the source's description on p.413 (text): "We consider only very small families … A biggest … a sum of \(5^d\) cubes". Each \(X\) is a connected union of at most \(N_X\le5^d\) cubes of \(\mathscr D\). The number \(N_\alpha\) of factor types is finite and depends only on \(d\); the source does not enumerate them additional assumption.

Let \(c_{\mathscr D}\le(2L+3)^d+5^d+3^d\) bound the number of \(\mathscr D\)-cubes (scales \(j-1,j,j+1\)) meeting a given one. Then:
\[
n_0\le c_{\mathscr D},\qquad K_w\le N_\alpha\cdot2N_Xc_{\mathscr D}(e\,c_{\mathscr D})^{N_X-1},
\]
and the convergence condition is \(O(1)K_wM^{-1/2}\le\frac12\). This is the source's "factor \(O(M^{-1/2})\) to control the sum over random walks", made explicit.

These constants are astronomically large but depend on \(d\) and \(L\) only.

**Tree-like walks are not needed.** The operators with tree-like expansions in [P] are \(G_1\), \(H_1\) and the new \(G\) of (180) (through \(\Delta^{(2)}\ni H^*J\)). In the calculus they are Neumann series and compositions of deformed primitives. [DN] Lemma 4.1 (R3)–(R4) handles them. Each primitive factor absorbs its own \(e^{\kappa\lvert\mathcal T(\omega)\rvert}\) through (W3), so a tile visited by several factors costs nothing extra. The counting constants of [DN]'s (W-ms) for \(G_1,H_1\) therefore drop out.
