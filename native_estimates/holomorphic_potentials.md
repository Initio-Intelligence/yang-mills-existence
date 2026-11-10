# Holomorphic dependence of the fluctuation potential

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 1. Setting (CMP116 §2)

All page references in this section are to CMP116 (printed pages). Fix a step \(k\). The following objects are those of CMP116 §2 and do not involve the potentials.

- **Fields.** External variables \((\mathbf U,\mathbf J)\); fluctuation field \(B\) on the bonds of the unit lattice. The Gaussian measure \(d\mu_{C^{(k)}}(B)\), the operators \(\Delta_k\), \(C\), \(C^{(k)}(Z_0)\), \((C^{(k)})^{1/2}\) and their generalised random-walk expansions with decoupling parameters \(s(\Delta)\). They are analytic in \((\mathbf U,\mathbf J)\) on the space of conditions I.(i)–(iii) with constants \(\alpha_0',\alpha_1'\) "much bigger than \(\alpha_0,\alpha_1\)" (p.10, p.15).
- **Cutoff.** \(\chi_k=\prod_b\chi(\{|B(b)|<\varepsilon_1/g_k\})\), with the decomposition (2.3) \(\chi_k=\sum_{P\subset Y_0^{c*}}(-1)^{|P|}\chi_{k,Y_0}\chi^c_{k,P}\).
- **Geometry.** Partitions \(\pi_k,\pi_{k+1}\), localisation domains \(\mathbf D_k,\mathbf D_{k+1}\), sizes \(d_k,d_{k+1}\) (CMP109 p.257).
- **Constants.** \(L,M,\kappa,\kappa_1,\delta\), with \(\tfrac18(\kappa_1-1)\ge(1-3\delta)\kappa\), \((1-10\delta)\tfrac L2=1\) (p.21); the auxiliary \(\alpha_4,\alpha_6,\gamma_2\) and \(\alpha_5=O(1)e^{-\frac13\delta_0M}+O(\alpha_0+\alpha_1)+O(1)\alpha_4+\gamma_2\) (p.17, p.20), with \((LM)^4\alpha_0,(LM)^4\alpha_1,(LM)^4\alpha_4,(LM)^4\gamma_2\le1\) (p.20).
- **Wilson quadratic form.** \(Q(Y,B,b,b')\) of Lemma 2, (1.42)–(1.43): it comes from \(P^{(k)}(g_k,\cdot)\) after cancelling \(1/g_k^2\) (pp.10–11) and satisfies
\[
|Q(Y,B,b,b')|\le C_3\varepsilon_1M^4e^{C_2\kappa_1}\exp\!\big(-\tfrac18(\kappa_1-1)d_k(Y)-\tfrac12(\kappa_1-1)M^{-4}|Y|\big).
\tag{1.43}
\]
Put \(a_Q:=C_3\varepsilon_1M^8e^{C_2\kappa_1}\).

**The potential space.** Write \(\kappa_*:=(1-2\delta)\kappa\). Let \(\mathcal V=\mathcal V_k\) be the complex Banach space of families \(v=(v_Y)_{Y\in\mathbf D_k}\) such that each \(v_Y\) is a function on the space CMP116 (1.34),
\[
\mathbf U^c_{k+1}\big(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0\big)\times\{B:\ |B|<\varepsilon_1g_k^{-1}\ \text{on }Y\},
\tag{L2.1}
\]
analytic in \((\mathbf U,\mathbf J)\), measurable in \(B\), depending only on the restrictions of \((\mathbf U,\mathbf J,B)\) to \(Y\), with
\[
\|v\|:=\sup_{Y}\ \sup_{(L2.1)}|v_Y|\,e^{\kappa_*d_k(Y)}<\infty.
\tag{L2.2}
\]
The full potential of the step is \(V_Y(B)=\tfrac12\langle Q(Y,B)B,B\rangle+v_Y(B)\), as in (1.42). In the source, \(v=\mathbf V''_k\) and \(\|v\|\le a_{\rm src}:=E_0\varepsilon_1C_1M^qe^{C_2\kappa_1}\) by (1.36).

Two remarks on (L2.1). First, analyticity in \(B\) is *not* required in §2: \(B\) is integrated over the real support of \(\chi_{k,Y_0}\) only. Second, the domain in \((\mathbf U,\mathbf J)\) is the \(\beta\)-enlarged **native** scale-\((k+1)\) space, not a ball around a real centre. The lemma below is pointwise in \((\mathbf U,\mathbf J)\): the output at a point of \(\mathbf U^c_{k+1}(X,\alpha_0,\alpha_1)\) uses the potentials \(v_Y\), \(Y\subset X\), at the same point.

**The expansion.** For \(v\in\mathcal V\), CMP116 (2.1)–(2.13) defines, with \(V=V[v]\):

- the Mayer-type expansion (2.1) in subfamilies \(\mathbf D\subset\mathbf D_k\), with \(Y_0=\bigcup_{Y\in\mathbf D}Y\);
- the cutoff decomposition (2.3), the smallest \(Z_0\in\mathbf D_k\) containing \(Y_0\) and \(P\), the conditioning (2.5)–(2.6), the decoupling (2.8) in the cubes of \(\pi_{k+1}\) outside \(Z_0'\);
- the polymer activities \(H(Z)=\sum_{Z_0:\tilde Z_0\subset Z}H(Z,Z_0)\), (2.9), their factorisation (2.10) and the polymer representation (2.11);
- the output
\[
\mathfrak E(X)[v]:=\sum_{n\ge1}\frac1{n!}\sum_{(Z_1,\dots,Z_n):\,\bigcup Z_i=X}\rho^T(Z_1,\dots,Z_n)\,H(Z_1)\cdots H(Z_n),\qquad X\in\mathbf D_{k+1}.
\tag{2.13}
\]

## 2. Statement

Let \(c_1\) denote the absolute constant "\(O(1)\)" in the sum over components before (2.37), and \(c_3\) the absolute constant "\(O(1)\)" in (2.41). For \(a>0\) put
\[
\varepsilon_2(a):=\frac{2a}{\alpha_4\alpha_6},\qquad C_3(a):=2(L+2)^4c_1\,\varepsilon_2.
\]
In the source \(a=a_{\rm src}\), \(\varepsilon_2(a_{\rm src})\) is the \(\varepsilon_2\) of p.19, and \(C_3(a_{\rm src})=C_3\varepsilon_1\) is the constant of (2.38).

**Budget conditions on \(a\).**

- (A0) \(a\ge a_Q\).
- (A1) \(\varepsilon_2(a)e^{5\kappa}\le1\) (the assumption before (2.28); it implies \(\varepsilon_2\le1\), used in (2.33), and \(a\le\alpha_4/\sqrt2\)).
- (A2) \(2(L+2)^4c_1\varepsilon_2(a)e^{5\kappa}\le1\) (the assumptions before (2.37)).
- (A3) \(\exp\!\big(-\tfrac1{20}\gamma_2\varepsilon_1^2/g_k^2\big)\le\varepsilon_2(a)\) (p.19, after (2.33)).
- (A4) \(C_3(a)\) is below the threshold required by the convergence argument for (2.39)–(2.40) ("for \(\kappa\) sufficiently large, and \(\varepsilon_1\) sufficiently small", p.21).

Let \(a_*\) be the largest \(a\) satisfying (A1), (A2), (A4). It has the form \(a_*=c_*\alpha_4\alpha_6e^{-5\kappa}(L+2)^{-4}\) with an absolute \(c_*>0\): a fixed number, independent of \(k\), \(g_k\) and the potentials.

> **Lemma L2.** Assume the standing restrictions of CMP116 §2 on \(L,M,\kappa,\kappa_1,\alpha_0,\alpha_1,\alpha_4,\alpha_6,\gamma_2,\gamma,\varepsilon_1\) (those listed in §1 and in §5 below), and let \(a\) satisfy (A0)–(A4). Then for every \(v\in\mathcal V\) with \(\|v\|\le a\):
> 1. **Activities.** For each \(Z\in\mathbf D_{k+1}\), \(H(Z)[v]\) is well defined, is an analytic function of \((\mathbf U,\mathbf J)\in\mathbf U^c_{k+1}(Z,\alpha_0,\alpha_1)\), depends only on \((v_Y)_{Y\subset Z}\), and
> \[
> |H(Z)[v]|\le C_3(a)\exp\!\big(-(1-8\delta)\tfrac12L\kappa\,d_{k+1}(Z)\big).
> \tag{L2.3}
> \]
> For fixed \(Z\) and \((\mathbf U,\mathbf J)\), \(v\mapsto H(Z)[v]\) extends to an **entire** function on \(\mathcal V\).
> 2. **Output.** The series (2.13) converges absolutely, uniformly in \(\|v\|\le a\) and in \((\mathbf U,\mathbf J)\in\mathbf U^c_{k+1}(X,\alpha_0,\alpha_1)\), and
> \[
> |\mathfrak E(X)[v](\mathbf U,\mathbf J)|\le c_3\,C_3(a)\,e^{-\kappa d_{k+1}(X)}.
> \tag{L2.4}
> \]
> \(\mathfrak E(X)[v]\) is analytic in \((\mathbf U,\mathbf J)\), depends only on \((v_Y)_{Y\subset X}\) and on \((\mathbf U,\mathbf J)\) in \(X\), and is gauge invariant if \(Q\) and all \(v_Y\) are.
> 3. **Holomorphy.** For each \(X\) and \((\mathbf U,\mathbf J)\), \(v\mapsto\mathfrak E(X)[v](\mathbf U,\mathbf J)\) is holomorphic on the open ball \(\{\|v\|<a\}\) of \(\mathcal V\).
> 4. **Sum rule.** On a finite torus, \(\sum_X\mathfrak E(X)[v]\) is a branch of \(\log\int d\mu_{C^{(k)}}(B)\chi_k\exp\sum_YV_Y[v](B)\); in particular this integral does not vanish for \(\|v\|\le a\). For real potentials at real fields it is the real logarithm.
> 5. **Derivative bound.** Let \(a=a_*\) and assume (A0), (A3) at \(a_*\). For \(\|v\|\le a_*/2\) and \(u\in\mathcal V\),
> \[
> \big|D\mathfrak E(X)[v]\cdot u\big|\le\Lambda\,\|u\|\,e^{-\kappa d_{k+1}(X)},\qquad
> \Lambda:=\frac{2c_3C_3(a_*)}{a_*}=\frac{8c_1c_3(L+2)^4}{\alpha_4\alpha_6}.
> \tag{L2.5}
> \]
> Consequently \(|\mathfrak E(X)[v]-\mathfrak E(X)[v']|\le\Lambda\|v-v'\|e^{-\kappa d_{k+1}(X)}\) for \(\|v\|,\|v'\|\le a_*/2\).

The constant \(\Lambda\) depends on \(L,M,\kappa\) (through \(\alpha_4,\alpha_6\)) and on nothing else. It is the same constant by which the source closes its own induction: on p.21 the condition is \(O(1)C_3\varepsilon_1\le\tfrac12E_0\), and \(C_3\varepsilon_1=C_3(a_{\rm src})\) is \(\Lambda/(2c_3)\) times the activity bound \(a_{\rm src}\), which is itself proportional to \(E_0\varepsilon_1\). Theorem A of the native-domain comparison is the Lipschitz version of that closing inequality.

## 3. Proof

### 3.1 Where the potentials enter (dependency analysis)

Consider CMP116 (2.1)–(2.41) line by line. The potentials occur in the following places and in no other.

| Place | What is used about the potentials | Holds for every \(v\) with \(\|v\|\le a\)? |
|---|---|---|
| (2.1): \(e^{\sum V_Y}=\sum_{\mathbf D}\prod_{Y\in\mathbf D}\int_0^1dt(Y)\,e^{\sum_{\mathbf D}t(Y)V_Y}\prod_{\mathbf D}V_Y\) | an algebraic identity (iterate \(e^x=1+\int_0^1x e^{tx}dt\)); needs a finite family of bounded functions | yes, in finite volume |
| (2.2)–(2.4): \(Y_0\), \(P\), \(Z_0\), \(F(Z_0,B)\) | locality: \(V_Y\) depends on \(B\) in \(Y\); \(V_Y\) is evaluated only on the support of \(\chi_{k,Y_0}\), i.e. \(|B|<\varepsilon_1/g_k\) on \(Y_0\supset Y\) | yes, by (L2.1) |
| (2.5)–(2.9): conditioning, change of variables, decoupling in \(s\), definition of \(H(Z,Z_0)\), \(H(Z)\) | none (the \(s\)-dependence is in the operators only; the potentials are functions of \((\mathbf U,\mathbf J,B)\)) | yes |
| p.15, analyticity paragraph | \(V_Y\) analytic on \(\mathbf U^c_{k+1}(Y,(1+\beta)\alpha_0,(1+\beta)\alpha_1,\alpha_0)\), hence on \(\mathbf U^c_{k+1}(X,\alpha_0,\alpha_1)\) for \(Y\subset Z_0\subset Z\subset X\) | yes, by (L2.1) |
| (2.14): \(\prod_{Y\in\mathbf D}V_Ye^{t(Y)V_Y}\) written as \(\prod\frac1{2\pi i}\oint\frac{d\tau(Y)}{(\tau(Y)-t(Y))^2}e^{\tau(Y)V_Y}\) | Cauchy's formula for the entire function \(\tau\mapsto e^{\tau V_Y}\); any radius \(|\tau(Y)|>1\) | yes; the radius is a free parameter and the value does not depend on it |
| (2.15): \(|e^{\sum\tau V}|\le e^{\sum|\tau||V|}\), factor \(\prod 2/|\tau(Y)|\) | absolute values only; \(\frac1{2\pi}\oint\frac{|d\tau|}{|\tau-t|^2}=\frac{R}{R^2-t^2}\le\frac2R\) for \(R=|\tau|\ge\sqrt2\), \(0\le t\le1\) | yes, if \(|\tau(Y)|\ge\sqrt2\) |
| (2.18): choice \(1/|\tau(Y)|=a\,\alpha_4^{-1}e^{-(1-3\delta)\kappa d_k(Y)}\) | the *bound constant* \(a\), not the potential | yes; \(|\tau(Y)|\ge\alpha_4/a\ge\sqrt2\) by (A1) |
| (2.19): \(|\tau(Y)|\cdot\tfrac12|\langle Q(Y,B)B,B\rangle|\) bounded by the quadratic form with matrix elements \(\alpha_4M^{-4}e^{-\frac14(\kappa_1-1)M^{-4}|Y|-\frac1{16}(\kappa_1-1)M^{-1}|b_--b_-'|}\) | (1.43), \(\tfrac18(\kappa_1-1)\ge(1-3\delta)\kappa\), and \(C_3\varepsilon_1M^4e^{C_2\kappa_1}/a\le M^{-4}\) | yes, by (A0). (The source obtains the same inequality from "\(C_3\le E_0C_1\) and \(q\ge8\)".) |
| (2.20): \(\sum_{Y\in\mathbf D}|\tau(Y)||v_Y|\le\sum_{Y\in\mathbf D}\alpha_4e^{-\delta\kappa d_k(Y)}\le O(1)\alpha_4M^{-4}|Y_0|\) | \(|v_Y|\le ae^{-(1-2\delta)\kappa d_k(Y)}\) on the support of \(\chi_{k,Y_0}\) | yes, by (L2.2) |
| (2.26): the factor \(\prod_{Y\in\mathbf D}2a\alpha_4^{-1}e^{-(1-3\delta)\kappa d_k(Y)}\) | the constant \(a\) | yes |
| (2.28), (2.33), (2.35), (2.37): \(\varepsilon_2\), \(\varepsilon_2e^{5\kappa}\le1\), \(\max\{\varepsilon_2,e^{-\gamma_2\varepsilon_1^2/20g^2}\}\), \(2(L+2)^4O(1)\varepsilon_2\le\tfrac12\) | the constant \(a\) through \(\varepsilon_2(a)\) | yes, by (A1)–(A3) |
| (2.38)–(2.41) | only the bound (2.38) on \(|H(Z)|\) | yes, by (A4) |
| last remark, p.21–22 | gauge invariance of the potentials | only for gauge-invariant \(v\) |

Everything else in (2.15)–(2.37) concerns the operators, the cutoff and the geometry: the perturbative comparison (2.16)–(2.17) of the complex operators with the real ones at \(\sigma=0\), \(\mathbf U=U\), \(\mathbf J=0\); the Gaussian integrals (2.21)–(2.25); the cutoff bound (2.22); the geometric inequalities (2.27), (2.30), (2.32), (2.36); the combinatorial sums (2.29), (2.31), (2.34). These are used below exactly as displayed (status source).

Three points deserve an explicit remark.

- **No adaptive choice.** The sets \(Y_0\), \(Z_0\), \(Z_0'\), \(Z\) are determined by the combinatorial data \((\mathbf D,P)\) and by the decoupling expansion, never by the values of the potentials. The Cauchy radii \(|\tau(Y)|\) are chosen from the *bound* \(a\); the value of each term is independent of the radius. The constants \(\alpha_4,\alpha_6,\gamma_2\) are fixed before the potentials.
- **Complex potentials.** The estimates take absolute values of \(e^{\sum\tau V}\) with complex \(\tau\) already in the source. Complex values of \(v\) need nothing new. Positivity of \(e^{\sum V}\) is never used.
- **The terms with \(\mathbf D=\emptyset\).** These contain no potential and at least one large-fluctuation factor \(\chi^c\). They are bounded by \(\exp(-\frac1{20}\gamma_2\varepsilon_1^2/g_k^2)\) (p.19). They are the reason why \(H(Z)\) is not bounded by a multiple of \(\|v\|\) but by a multiple of \(\max\{a,\ \alpha_4\alpha_6e^{-\gamma_2\varepsilon_1^2/20g_k^2}\}\); condition (A3) puts them inside the budget. They cancel in differences and derivatives.

### 3.2 The bound (L2.3) with a general budget

Fix \(Z\), \(Z_0\), \(\mathbf D\), \(P\) and a point of \(\mathbf U^c_{k+1}(Z,\alpha_0,\alpha_1)\). With the radii of (2.18) (with \(a\) in place of \(E_0\varepsilon_1C_1M^qe^{C_2\kappa_1}\)), the first estimate (2.15) holds as displayed, by the rows (2.14)–(2.15) of the table. By the rows (2.19)–(2.20),
\[
\sum_{Y\in\mathbf D}|\tau(Y)||V_Y(B)|\le\tfrac12O(1)\alpha_4\sum_{b\subset Y_0}|B(b)|^2+O(1)\alpha_4M^{-4}|Y_0|,
\]
which is (2.20). From here to (2.26) the source's computation involves only the operators, the cutoff bound (2.22) and Gaussian integrals, and gives
\[
|(2.14)|\le e^{-(\kappa_1-1)(LM)^{-4}|Z\setminus Z_0'|}\Big[\prod_{Y\in\mathbf D}2a\alpha_4^{-1}e^{-(1-3\delta)\kappa d_k(Y)}\Big]e^{-\frac12\gamma_2\frac{\varepsilon_1^2}{g_k^2}|P|}\,e^{O(1)\alpha_5|Z|}.
\tag{2.26\('\)}
\]
The resummations over \(\mathbf D\), \(P\), \(Y_0\), \(Z_0\), \(Z_0'\) on pp.17–20 use (2.26\('\)) and the constant \(\varepsilon_2=\varepsilon_2(a)\) only:

- (2.27)–(2.29), with (A1): the sum over \(\mathbf D\) with fixed \(Y_0\) is at most \(\varepsilon_2(a)e^{-(1-4\delta)\kappa d_k(Y_0)}\) per component of \(Y_0\). (Check: each factor is \(\alpha_6e^{-\delta\kappa d_k(Y)}\cdot\varepsilon_2e^{-(1-4\delta)\kappa d_k(Y)}\); by (2.27) and \(\varepsilon_2e^{5\kappa}\le1\) the product of the second factors over a component is at most \(\varepsilon_2e^{-(1-4\delta)\kappa d_k(Y_0)}\); (2.29) sums the first factors.)
- (2.31)–(2.34), with (A3): the sums over \(P\) and \(Y_0\subset Z_0\) give (2.35) with \(\varepsilon_2(a)\).
- (2.36)–(2.37), with (A2): the sum over \(Z_0\) with fixed \(Z_0'\) gives (2.37) with \(2(L+2)^4c_1\varepsilon_2(a)=C_3(a)\).
- The sum over \(Z_0'\subset Z\) (p.20, last paragraph before Lemma 3) uses the restrictions on \(\alpha_0,\alpha_1,\alpha_4,\gamma_2,\kappa_1\) only and gives (L2.3).

This proves (L2.3). Locality and analyticity in \((\mathbf U,\mathbf J)\) are the statements of p.14 (after (2.9)) and p.15, which use (L2.1) only.

### 3.3 Each activity is an entire function of the potentials

Fix \(Z\) and \((\mathbf U,\mathbf J)\). The sum defining \(H(Z)\) over \((Z_0,\mathbf D,P)\) is finite: \(\mathbf D\) is a subfamily of the finitely many \(Y\in\mathbf D_k\) with \(Y\subset Z\), and \(P\) is a set of bonds in \(Z\). Consider one term, in the form (2.14) with all radii \(|\tau(Y)|=\sqrt2\) (allowed, since the value does not depend on the radii). Let \(v=v_0+\lambda v_1\) with \(v_0,v_1\in\mathcal V\), \(\lambda\in\mathbb C\). The integrand of (2.14) depends on \(\lambda\) through
\[
\exp\Big[\sum_{Y\in\mathbf D}\tau(Y)\big(\tfrac12\langle Q(Y,B)B,B\rangle+v_{0,Y}(B)+\lambda v_{1,Y}(B)\big)\Big],
\]
which is entire in \(\lambda\) for every value of the integration variables. On the support of \(\chi_{k,Y_0}\) its modulus is at most
\[
\exp\Big[\sqrt2\,|\mathbf D|\big(\|v_0\|+|\lambda|\|v_1\|\big)\Big]\cdot\exp\Big[\sqrt2\sum_{Y\in\mathbf D}\tfrac12|\langle Q(Y,B)B,B\rangle|\Big].
\]
The first factor is a constant, locally bounded in \(\lambda\). The second factor is the one treated in (2.19) (with \(|\tau|=\sqrt2\), which is smaller than the radius (2.18), so the quadratic form is smaller). Hence the integrand is dominated, locally uniformly in \(\lambda\), by the integrable majorant of (2.15)–(2.25). The remaining integrations are over compact contours and intervals. By Fubini and Morera, the term is entire in \(\lambda\). A function on a complex Banach space which is entire on every complex line and locally bounded is entire; local boundedness is the displayed majorant. \(\square\)

### 3.4 Convergence, the bound (L2.4) and holomorphy

The passage from (2.38) to (2.41) (pp.20–21) replaces each \(|H(Z_i)|\) by the right side of (2.38) and uses the tree-graph bound for \(\rho^T\) and geometric sums, "for \(\kappa\) sufficiently large, and \(\varepsilon_1\) sufficiently small". The smallness is a condition on the constant in (2.38), here \(C_3(a)\); this is (A4). The result is (2.41) with \(C_3\varepsilon_1\) replaced by \(C_3(a)\), and with \((1-10\delta)\frac L2=1\) it is (L2.4). The majorant series depends on \(v\) only through \(a\), so the convergence is uniform on \(\{\|v\|\le a\}\times\mathbf U^c_{k+1}(X,\alpha_0,\alpha_1)\). This step is cited (status source): the source refers to its reference [26] for the combinatorics, and The proof assumes the tree-graph estimate. It is a statement about absolute values of activities satisfying (2.38), with no reference to their origin.

Each term of (2.13) is a finite product of activities, hence entire in \(v\) by §3.3. A uniformly convergent series of holomorphic functions on the open ball is holomorphic there (apply Weierstrass on each complex line; the sum is bounded by (L2.4)). This proves item 3. Uniform convergence in \((\mathbf U,\mathbf J)\) gives analyticity in \((\mathbf U,\mathbf J)\). Locality follows from that of the activities, since \(\bigcup Z_i=X\). Gauge invariance is the source's last remark (pp.21–22) and uses gauge invariance of the potentials.

### 3.5 The sum rule

On a finite torus the family of polymers is finite. Then (2.9)–(2.11) is the identity \(\int d\mu\chi_ke^{\sum V}=\sum_{\{Z_i\}}\prod H(Z_i)\) (a finite sum over compatible families), valid for all \(v\in\mathcal V\): its derivation uses only the algebraic identity (2.1), (2.3), Fubini and the fundamental theorem of calculus in \(s\). The right side is a polynomial \(\Xi\) in the finitely many numbers \(H(Z)\). The series \(\sum_X(2.13)\) is the formal logarithm of \(\Xi\) as a power series in these numbers, and it converges absolutely when they satisfy (2.38) with (A4). Hence \(\Xi=\exp\sum_X\mathfrak E(X)\) there. In particular \(\Xi\ne0\). For real potentials at real fields every \(H(Z)\) is real (it is a sum of integrals and \(s\)-derivatives of real quantities), so \(\sum_X\mathfrak E(X)\) is real, and \(\Xi>0\) as the integral of a positive function; hence the sum is the real logarithm. \(\square\)

### 3.6 The derivative bound

Let \(\|v\|\le a_*/2\), \(\|u\|=1\). For \(|\lambda|<a_*/2\) the point \(v+\lambda u\) lies in the open ball of radius \(a_*\). By items 2 and 3, \(\lambda\mapsto\mathfrak E(X)[v+\lambda u]\) is holomorphic and bounded by \(c_3C_3(a_*)e^{-\kappa d_{k+1}(X)}\) on that disc. Cauchy's estimate at \(\lambda=0\) gives (L2.5) with \(\Lambda=2c_3C_3(a_*)/a_*\). Since \(C_3(a)\) is linear in \(a\), \(\Lambda=8c_1c_3(L+2)^4/(\alpha_4\alpha_6)\). The Lipschitz bound follows by integrating the derivative along the segment from \(v'\) to \(v\), which stays in the ball of radius \(a_*/2\). \(\square\)

This completes the proof of Lemma L2, conditional on the cited potential-independent estimates of CMP116 §2.

## 4. The rooted form needed by Theorem A

### 4.1 Why a Lipschitz bound for (2.13) is not yet enough

The inductive hypotheses of CMP119 are for **rooted** births: \(\mathbf E^{(j)}(U,z)=\sum_{X\ni z}\mathbf E^{(j)}(X,U,z)\), (2.26)–(2.27), with the exact Euclidean covariance (2.29) of the rooted density. The covariance is used in CMP119 (3.57)–(3.61): the second-order coefficient \(\Pi^{(j)}_{\mu\nu,\kappa\lambda}\) is independent of \(z\) and isotropic, so the \(\beta_j\) Wilson subtraction cancels the marginal term *pointwise in \(z\)*. A family whose rooted density is covariant only under a sublattice would leave a zero-mean periodic marginal remainder (the problem treated for R terms in [Reset remainders](../coupling/reset_remainders.md) §2). So in Theorem A the difference \(\delta H_{k+1}\) must be delivered as a rooted family with a covariant rooted density, a native bound, and the correct sum.

CMP119 obtains its rooted births from the \(g_k\)-derivative representation (3.30)–(3.37) and the numerator/denominator expansion (3.44)–(3.47). The latter is described but not displayed in full (the factor \(H'(Z_0)\) is "given by an integral with the integrand including, as one of the factors, a localized term from the expansion of the integrated function", p.277). Therefore do not prove holomorphy of that specific representation. Instead the following construction produces a rooted difference family directly from Lemma L2. It is legitimate because only three things are needed of the difference family: its sum, the covariance of its rooted density, and its bound. The localisation of a difference is not prescribed by the source.

### 4.2 Rooted potentials

Let \(\mathcal Z\) be the set of roots at scale \(k+1\) (sites of \(T^{(k+1)}\)). A **rooted potential** is a family \(w=(w_{Y,z})_{Y\in\mathbf D_k,z\in\mathcal Z}\) with \(w_{\cdot,z}\in\mathcal V\) for each \(z\), \(w_{Y,z}=0\) unless \(z\in Y\), and norm
\[
|||w|||:=\sup_{z}\|w_{\cdot,z}\|.
\]
Its sum is \(w_Y:=\sum_zw_{Y,z}\in\mathcal V\) (finite sum for each \(Y\)). It is **covariant** if, on the whole lattice, \(\sum_Yw_{Y,z}\) transforms as \(\sum_Yw_{Y,rz}(r\mathbf U,r\mathbf J,rB)=\sum_Yw_{Y,z}(\mathbf U,\mathbf J,B)\) under the Euclidean transformations \(r\) of the lattice \(T^{(k+1)}\).

(The support convention \(z\in Y\) can be arranged at the cost of a fixed constant: a rooted term whose domain \(Y\) is within one \(M\)-cube of \(z\) is reassigned to the union of \(Y\) and that cube, which changes \(d_k\) by a bounded amount.)

### 4.3 Proposition L2.2 (rooted difference family)

> **Proposition L2.2.** Let the hypotheses of Lemma L2 hold at \(a=a_*\), including (A0) and (A3). Let \(v^{(1)},v^{(0)}\in\mathcal V\) with \(\|v^{(1)}\|\le a_*/4\). Let \(w\) be a rooted potential with sum \(v^{(1)}-v^{(0)}\), and suppose \(\|v^{(1)}-v^{(0)}\|\le\omega\) and \(|||w|||\le\omega\) with \(\omega\le a_*/4\). Put \(v_s:=v^{(0)}+s(v^{(1)}-v^{(0)})\) and
> \[
> \Delta(X,z):=\int_0^1ds\ \frac{\partial}{\partial\lambda}\,\mathfrak E(X)\big[v_s+\lambda w_{\cdot,z}\big]\Big|_{\lambda=0},\qquad X\in\mathbf D_{k+1},\ z\in\mathcal Z.
> \tag{L2.6}
> \]
> Then:
> 1. \(\Delta(X,z)=0\) unless \(z\in X\); \(\Delta(X,z)\) is analytic on \(\mathbf U^c_{k+1}(X,\alpha_0,\alpha_1)\), depends on \((\mathbf U,\mathbf J)\) in \(X\), and is gauge invariant if \(Q\), \(v^{(0)}\), \(v^{(1)}\), \(w\) are.
> 2. \(\displaystyle|\Delta(X,z)|\le2\Lambda\,\omega\,e^{-\kappa d_{k+1}(X)}\), with \(\Lambda\) of (L2.5).
> 3. On a finite torus,
> \[
> \sum_{z}\sum_{X\ni z}\Delta(X,z)=\log\!\int\!d\mu\,\chi_k\,e^{\sum_YV_Y[v^{(1)}]}-\log\!\int\!d\mu\,\chi_k\,e^{\sum_YV_Y[v^{(0)}]} ,
> \]
> and the rooted density is \(\sum_{X\ni z}\Delta(X,z)=\int_0^1ds\,\langle\sum_Yw_{Y,z}\rangle_{v_s}\), where \(\langle\cdot\rangle_{v}\) is the normalised (complex) expectation with weight \(d\mu\,\chi_k\,e^{\sum V[v]}\).
> 4. If the Gaussian data, the cutoff and \(Q\) are covariant under the Euclidean transformations of \(T^{(k+1)}\), the sums \(\sum_Yv^{(i)}_Y\) are covariant, and \(w\) is covariant, then the rooted density \(\sum_{X\ni z}\Delta(X,z)\) satisfies the covariance (2.29).

*Proof.* For \(0\le s\le1\), \(\|v_s\|\le\|v^{(1)}\|+(1-s)\|v^{(1)}-v^{(0)}\|\le a_*/2\). For \(|\lambda|\le a_*/(2\omega)\), \(\|v_s+\lambda w_{\cdot,z}\|\le a_*\). By Lemma L2, items 2–3, \(\lambda\mapsto\mathfrak E(X)[v_s+\lambda w_{\cdot,z}]\) is holomorphic on that disc and bounded by \(c_3C_3(a_*)e^{-\kappa d_{k+1}(X)}\). Cauchy's estimate gives \(|\partial_\lambda\mathfrak E(X)|_{\lambda=0}\le c_3C_3(a_*)e^{-\kappa d_{k+1}(X)}\cdot2\omega/a_*=\Lambda\omega e^{-\kappa d_{k+1}(X)}\), uniformly in \(s\) (the stated bound has a spare factor 2). The dependence on \(s\) is continuous, so the integral exists. This is item 2.

Item 1: \(\mathfrak E(X)[v]\) depends only on \((v_Y)_{Y\subset X}\). If \(z\notin X\), every \(Y\subset X\) has \(w_{Y,z}=0\), so \(\mathfrak E(X)[v_s+\lambda w_{\cdot,z}]\) does not depend on \(\lambda\). Analyticity, locality and gauge invariance are inherited from Lemma L2, since the \(\lambda\)-derivative is a Cauchy integral of such functions.

Item 3: by the sum rule and item 1,
\[
\sum_{X\ni z}\partial_\lambda\mathfrak E(X)[v_s+\lambda w_{\cdot,z}]\big|_0=\partial_\lambda\log\!\int\!d\mu\chi_ke^{\sum V[v_s]+\lambda\sum_Yw_{Y,z}}\Big|_0=\Big\langle\sum_Yw_{Y,z}\Big\rangle_{v_s}.
\]
(The derivative may be taken termwise: the series over \(X\) is a finite sum on a torus, and differentiation under the integral is justified by boundedness of \(\sum_Yw_{Y,z}\) on the support.) Summing over \(z\) gives \(\langle\sum_Y(v^{(1)}_Y-v^{(0)}_Y)\rangle_{v_s}=\frac{d}{ds}\log\int d\mu\chi_ke^{\sum V[v_s]}\). Integrate over \(s\).

Item 4: the expectation \(\langle\cdot\rangle_{v_s}\) is covariant when the measure, cutoff and the total potential \(\sum_YV_Y[v_s]\) are; the observable \(\sum_Yw_{Y,z}\) is covariant by assumption. \(\square\)

### 4.4 Use in Theorem A

In the analysis §9 this proposition is applied at step \(k\) with \(v^{(1)}\) the actual potentials (Wilson remainder, E fluctuation difference of the actual births, mature R), \(v^{(0)}\) the comparator potentials, and \(w\) the rooted, covariant potentials of the differences \(\delta H_j\), \(j\le k\), and of the mature R terms. Then \(\Delta=\delta H_{k+1}\) is a rooted birth family at scale \(k+1\) with
\[
\|\delta H_{k+1}\|_{k+1}\le2\Lambda\,\omega_k,\qquad\omega_k\le C_V\rho_k\sup_{j\le k}\|\delta H_j\|_j+C_R\,g_k^{\kappa_0-11}.
\]
The comparator birth is *defined* as \(H'_{k+1}:=\mathbf E^{(k+1)}-\delta H_{k+1}\). No holomorphy of the CMP119-specific localisation of the actual birth is used; the actual birth enters only through its source bound (F1) and through the identity "sum of rooted densities = logarithm of the fluctuation integral" (CMP119 (3.28), (3.38), (3.42)).

## 5. The running chart: every restriction on constants

On the running chart of CMP119 the correspondence is
\[
\alpha_0,\alpha_1\ \to\ \alpha_{0,k+1},\alpha_{1,k+1}\ (\text{provisional: computed with }g_k),\qquad
\varepsilon_1/g_k\ \to\ P_k=A_1\ell_k^{p_0},\qquad\varepsilon_1\ \to\ \delta_k=g_kP_k.
\]
The auxiliary constants \(\alpha_4,\alpha_6,\gamma_2,\kappa,\kappa_1,M,L,\delta\) stay fixed. The potentials are given on the source domain CMP119 (3.43); only its real section \(|A|\le P_k\) in the fluctuation variable is used.

| Restriction in CMP116 §2 | Kind | On the running chart |
|---|---|---|
| \(e^{-\frac13\delta_0M}e^{16\kappa_1}<1\); \(\tfrac18(\kappa_1-1)\ge(1-3\delta)\kappa\); \(\tfrac12(\kappa_1-1)\ge2L\kappa\); \((1-10\delta)\tfrac L2=1\) (pp.16, 18, 20, 21) | fixed constants | unchanged |
| \((LM)^4\alpha_0\le1\), \((LM)^4\alpha_1\le1\); \(O(\alpha_0+\alpha_1)\) in (2.16), (2.17), (2.21), \(\alpha_5\) | upper bounds on the external radii | improve: \(\alpha_{u,k+1}=C_ug_k\ell_k^q\to0\) |
| \(\alpha_5\|C^{(k)}(Z_0,0)\|<\tfrac12\) (p.17) | fixed | unchanged |
| \((LM)^4\alpha_4\le1\), \((LM)^4\gamma_2\le1\); \(\alpha_6\) small for (2.29) | fixed constants | unchanged |
| \(\tfrac1{20}\gamma_2\varepsilon_1^2/g_k^2\ge4\kappa\) (p.18–19) and (2.31) "for \(g_k^2\) sufficiently small depending on \(M,\kappa\)" | lower bound on the normalised cutoff | \(\gamma_2P_k^2\ge80\kappa\) and \(\tfrac1{20}\gamma_2P_k^2\ge4M^4e^{-\gamma_2P_k^2/10}\): hold for \(\ell_k\) large, since \(P_k\to\infty\) |
| (A3): \(e^{-\gamma_2\varepsilon_1^2/20g_k^2}\le\varepsilon_2(a_*)\) | cutoff defect inside the budget | \(e^{-\gamma_2A_1^2\ell_k^{2p_0}/20}\le\varepsilon_2(a_*)\): holds for \(\ell_k\) large; the left side is smaller than any power of \(g_k\) because \(p_0>1\) |
| (A0): \(a_*\ge a_Q=C_3\varepsilon_1M^8e^{C_2\kappa_1}\) | Wilson quadratic form inside the budget | \(a_Q=C_3\delta_kM^8e^{C_2\kappa_1}\to0\); holds below a ceiling |
| \(e^{32\kappa_1}\varepsilon_1\) below an absolute constant; \(4B_0C_Be^{16\kappa_1}\varepsilon_1\le\tfrac14\alpha_2\), with \(C_B\) the constant printed as \(C_1\) in CMP116 (1.20) (CMP116 p.7; these belong to §1, i.e. to (L1)) | upper bounds on \(\delta_k\) | the first holds below a ceiling; the second is \(\ell_k^{q-p_0}\ge16B_0C_Be^{16\kappa_1}A_1/(c_2C_0)\) with \(\alpha_{2,k}=c_2\alpha_{0,k}=c_2C_0g_k\ell_k^q\) |
| \(\|v\|\le a_*/4\) for the actual potentials | input smallness | the Wilson part is \(O(\delta_k)\); the E part is \(C_V\rho_kE_0\) with \(\rho_k\asymp\ell_k^{p_0-q}\) (hypothesis (L1*) of the analysis); the R part is \(C_Rg_k^{\kappa_0-11}\). All below \(a_*/4\) for \(\ell_k\) large. This is (P22.9) of the native-domain comparison. |

**Output domain.** Lemma L2 gives the output at every point at which all \(v_Y\), \(Y\subset X\), are given. With potentials on CMP119 (3.43), i.e. on \(\tilde U^c_{k+1}(Y,(1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1)\) with provisional radii, the output is analytic on the corresponding \((1+\beta)\)-enlarged space on \(X\). This contains the native space with radii computed from any \(g\) with \(g\ell(g)^q\le(1+\beta)g_k\ell_k^q\). The crude bound \(|c_{k+1}|\le C_PE_0r_{k+1}^{-2}=O(Y_k\ell_k^{-2q})\) already gives \(g_{k+1}/g_k=1+O(\ell_k^{-2q})\), so the actual chart at \(k+1\) is covered. No circularity arises with the admission argument.

**Decay regeneration.** Input decay \(\kappa_*=(1-2\delta)\kappa\) at scale \(k\); output decay \((1-10\delta)\frac L2\kappa=\kappa\) at scale \(k+1\). The mechanism is the geometric inequality (2.36), \(2d_k(Z_i)\ge Ld_{k+1}(Z_i')\), which does not involve the potentials or the radii. It is the same on the running chart.

**Two differences of CMP119 from CMP116 that The argument assumes.**

- *(S-cut)* CMP119 uses the cutoff \(\chi^{(k)}\) of (3.16), a product over cubes of indicator functions of \(\sup_b|A_k(b)|\) (after the scaling \(A_k'=g_kA_k\) the bound must be read as \(|A_k(b)|<\delta_k/g_k\); as printed the display has \(\delta_k\)). CMP116 uses a product over bonds. The decomposition (2.3) and the estimates (2.22), (2.31)–(2.34) have obvious analogues, and the source says the expansion is made "in exactly the same way as in Sect. 7 [I]" and that the differences "do not matter" (p.277). Take this as a cited assumption.
- *(S-op)* On the whole lattice the operators are those of [I]. For the whole-lattice (homogeneous) births used in B-03 no boundary layers occur.
