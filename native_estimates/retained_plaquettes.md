# A lower tail for plaquettes and retained birth-scale marks

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

## 1. Conventions, primary-source facts and analytic inputs

### 1.1 Notation

\(G=SU(N)\), \(D=N^2-1\), dimension \(d=4\). Plaquette action \(s(U)=N-\operatorname{Re}\operatorname{Tr}U=\tfrac12\|U-1\|_{\rm HS}^2\), Wilson weight \(\exp(-\beta\sum_ps(U_p))\) on a periodic lattice with at least three sites per direction, \(e_p=\beta s(U_p)\), \(E_X=\sum_{p\in X}e_p\) (Annex A (1.1)). Every link lies in \(n_s=2(d-1)=6\) plaquettes. The fine spacing is \(a\), the block factor \(L\), and \(h_j=L^ja\).

The scalar member of the F-01 family is the vertex action density \(w_a(x)\) of Annex E (1.5), (1.9); thus
\[
a^4\beta w_a(x)=\tfrac14\sum_{p\ni x}e_p ,\qquad
O_x:=\beta w_a(x)-\mathbb E[\beta w_a(x)] ,\qquad
C_E:=\sup_x\mathbb E[a^4\beta w_a(x)]\le 6\sup_p\mathbb E e_p.
\tag{1.1}
\]
\(O_x\) is the centered, energy-normalized scalar mark in physical units. Under K-02 below, \(C_E\le 6\eta^{-1}\log K\) by Jensen.

Balaban's integer \(N\) of LFR I p.177 is written \(N_B\) to avoid the clash with \(SU(N)\). His matrix norm \(|\cdot|\) is not specified in the pages used here; only
\[
|A|\le\|A\|_{\rm HS}\le\sqrt N\,|A|
\tag{1.2}
\]
is used (true for the operator norm; another equivalent norm changes fixed constants only).

### 1.2 Primary-source facts used — label

* **(S1) First-step selector.** CMP 119 p.246, (1.1): the first decomposition of unity is over unions \(P_0\) of \(LM_2R_0\)-cubes \(\square\), with small-field factor \(\chi(\{\sup_{p\subset\square^\sim}|U(\partial p)-1|<\varepsilon_0\})\) and large-field factor \(\chi(\{\sup_{p\subset\square^\sim}|U(\partial p)-1|\ge\varepsilon_0\})\); \(\varepsilon_0=g_0p_0(g_0)\), \(p_0(g_0)=A_0(\log g_0^{-2})^{p_0}\), \(p_0\ge5r\). Checked in the source (in the source text of this display is corrupted).
* **(S2) Bounded inherited window and the P-test.** CMP 119 p.264, text after (3.1): "the restrictions introduced by the characteristic function \(\chi_k\) imply that the new fields \(V_{k+1}\) satisfy the bounds \(|V_{k+1}(\partial p')-1|<2L^2\varepsilon_k\)". P.265, (3.2): the new decomposition of unity on \((Z_k'^{\sim4})^c\) is over unions \(P_{k+1}\) of \(L^2M_2R_{k+1}\)-cubes \(\square'\), with large-field factor \(\chi(\{\sup_{p\subset\square'^\sim}|U_{k+1,\square'}(\partial p)-1|\ge\varepsilon_{k+1}(L^{-1}\eta)^2\})\). (3.3) and (3.16) are the Q and R tests on the approximate and exact fluctuation fields, thresholds \(2\delta_k\), \(\delta_k=g_k(A_1/A_0)p_0(g_k)\). as stated in the source.
* **(S3) Eligibility for the R operation.** LFR I p.177: a component is eligible only if "(i) it is contained in a cube of the size \(100MR_k\), (ii) in the preceding \(N\) renormalization steps no new large field regions were created inside this component, and the previous regions contained in it satisfy the condition (i) on the corresponding scales." P.179: "\(N>N_0\), in fact … \(N\) is much greater than \(N_0\)", where \(L^{-N_0+1}MR_{k-N_0+1}=M\).
* **(S4) Unnormalized large-field factors and their horizon.** LFR II p.380: the P, Q, R characteristic functions of step \(j\) yield the factors \(\exp(-\gamma_0\frac1{2g_j^2}(B_3^{-1}\varepsilon_j)^2(LM_2R_j)^{-d}|P_j|)\), \(\exp(-\tfrac12\gamma_0g_j^{-2}(2\delta_j)^2(LM_2R_j)^{-2}|Q_j|)\), \(\exp(-\gamma_0g_j^{-2}\delta_j^2(LM_2R_j)^{-d}|R_j|)\). P.381: per component \(Z_j^{(i)}\) these are bounded by \(\exp(-\tfrac12\gamma_0A_1^2p_0^2(g_j)(d_j'(Z_j^{(i)})+1)-2p_0(g_j))\); preparatory factors are bounded by \(\exp(-p_0(g_j))\) (p.383). P.383, (1.79) and p.384, (1.80): the reserve \(\kappa_j(Z)\) "controls \(K\) renormalization steps … where \(K\) is the smallest positive integer having the property that the domain \(S^K(Z)\) … satisfies the conditions (i), (ii), with \(N=R_j\)"; \(S(Z)=Z'^{\sim10}\); \(S^{n-j}(Z)\subset\bigcup_{\square_0\subset Z^{(n-j)}}\square_0^{\sim31}\) with \(Z^{(n-j)}\) the cover of \(Z\) by \(MR_n\)-cubes. P.387, (1.89): \(\mathbf T_k'(X)1\le\exp(-2(1+\beta_0)^{-1}p_0(g_k))\). **All of (S4) is unnormalized** (Annex AK §6 already records this); it is used here only for the dictionary in §4.3 and §5.6, never as a probability.

### 1.3 construction inputs used — conditional wherever they enter

* **(K-02) Compact Wilson reserve**, Annex A Theorem 3.1, (3.4): on the cofinal class (3.3), for \(0<\eta\le1/8\) and every plaquette set \(X\),
  \(\mathbb E e^{\eta E_X}\le K^{b(X)}\), \(b(X)\) the least number of closed unit cubes covering \(X\) (so \(b(X)\le|X|\)), \(K\ge1\) independent of cutoff, volume and \(X\). The proof uses (chessboard (3.1) plus the matched powers (2.1)) and the result is an accepted construction result and is used in §4 only.
* **(H-01) Positive history lift**, Annex W §4: one probability space carrying the original Wilson field with exactly its Wilson marginal, all selector labels, and all later variables; the transported mark at step \(j\) is the conditional expectation \(Q_jF=\mathbb E[F\mid\mathcal F_j]\) with respect to the σ-field \(\mathcal F_j\) of the data retained at step \(j\) (W (4.5), (4.8) composed). W §4.2 requires that the retained data "include the history, graph and exterior data deciding which kernel was applied".
* **(M-03) Norm**, Annex Y (M.8), (M.11), (M.12): \(\mathfrak m_d(F;\mu)=\sup_{p\ge1}(dp)^{-d}\|F\|_{L^p(\mu)}\); the value part of the norm of a one-label coefficient is \(h^4[\mathfrak m_1(A_X^\sharp;\mu_h)+\sup_xA^\sharp_X/\widehat R_{h,X}]\), summed over the carriers of a specified representation with weights \(w_h(X)\ge1\).
* **(Ret) Retention hypothesis.** For the steps \(j\) considered, the first-step label event \(E_\Pi\) of §2.2 is \(\mathcal F_j\)-measurable. This is *forced* for \(1\le j<N_B\) in any lift satisfying the W §4.2 requirement: by (S3)(ii) the kernel applied at a step \(k\le N_B\) (eligible or not) depends on whether a large-field region was created in the component during the preceding \(N_B\) steps, i.e. on the first-step label. It is also how the accepted H-03 theorem is formulated: "Unreplaced Zbar labels … are retained, not silently reset" (H03/M04 update, §"physical supports"). H-01 keeps the *primitive* labels ("the exposed history through scale \(k\), including primitive selector and graph labels before any resummation"), which is exactly \(E_\Pi\in\mathcal F_j\). The variant in which only the resummed region \(\Omega_1\) is retained is treated in Remark 3.6.

## 2. A volume-uniform lower tail for one Wilson plaquette

The reserve K-02 bounds \(\mathbb P(e_p\ge t)\) from above by \(Ke^{-\eta t}\). The obstruction in §3 needs the matching bound from below. It is elementary and holds conditionally on all other links.

### Lemma 2.1 — one-link lower tail

Let \(\mu\) be the Wilson measure with coefficient \(\beta>0\) on any finite lattice in which every link lies in at most \(n_s\) plaquettes and no plaquette contains a link twice. Let \(p\) be a plaquette and \(\ell\in\partial p\). Put
\[
C_1:=\tfrac{25\pi^2}{2}\,n_sN.
\]
Then for every \(t\) with \(0<t\le\beta/(200N)\), almost surely,
\[
\boxed{\ \mu\bigl(e_p\ge t\ \big|\ U_{\ell'},\ \ell'\ne\ell\bigr)\ \ge\ \tfrac12e^{-C_1t}.\ }
\tag{2.1}
\]
The same bound therefore holds unconditionally, on every such lattice, for every boundary condition, and on every probability space carrying a field with this conditional law.

**Proof.** Fix all links except \(U:=U_\ell\). For each plaquette \(p'\ni\ell\), reading \(\partial p'\) from \(\ell\) in its positive direction gives \(U_{p'}=UB_{p'}\) up to cyclic rotation and inversion, neither of which changes \(s\); with \(W_{p'}:=B_{p'}^*\in SU(N)\),
\(s(U_{p'})=N-\operatorname{Re}\operatorname{Tr}(UW_{p'}^*)\). Hence the conditional law of \(U\) has Haar density proportional to \(e^{\beta\Phi(U)}\),
\[
\Phi(U)=\operatorname{Re}\operatorname{Tr}(US^*),\qquad S=\sum_{p'\ni\ell}W_{p'},\qquad \|S\|_{\rm tr}\le n_sN.
\]
Write \(W=W_p\). Since \(U,W\) are unitary, \(s(U_p)=\tfrac12\|U-W\|_{\rm HS}^2\). With \(\tau:=(2t/\beta)^{1/2}\) the complementary event is the open ball \(B(W,\tau)=\{\|U-W\|_{\rm HS}<\tau\}\). The hypothesis on \(t\) is \(\tau\le1/(10\sqrt N)\). By bi-invariance, \(\operatorname{Haar}(B(Y,r))=:h(r)\) does not depend on \(Y\).

*Step 1: second-order bound at a maximizer.* Let \(U_*\) maximize \(\Phi\), \(M=\Phi(U_*)\). Let \(\|U-U_*\|_{\rm HS}\le r\le1/(2\sqrt N)\) and \(V=U_*^{-1}U\). Write \(V=\sum_ke^{i\theta_k}P_k\) with \(\theta_k\in(-\pi,\pi]\). From \(|e^{i\theta}-1|=2|\sin(\theta/2)|\ge2|\theta|/\pi\), \(\sum_k\theta_k^2\le(\pi r/2)^2\). Since \(\det V=1\), \(\sum_k\theta_k\in2\pi\mathbb Z\), while \(|\sum_k\theta_k|\le\sqrt N\,\pi r/2<2\pi\); hence \(\sum_k\theta_k=0\), \(X:=i\sum_k\theta_kP_k\in\mathfrak{su}(N)\), \(V=e^X\) and \(\rho:=\|X\|_{\rm HS}\le\pi r/2\le1\). Now
\[
\Phi(U_*e^X)-M=\operatorname{Re}\operatorname{Tr}(U_*XS^*)+\operatorname{Re}\operatorname{Tr}\bigl(U_*(e^X-1-X)S^*\bigr).
\]
The first term is the derivative at \(s=0\) of \(s\mapsto\Phi(U_*e^{sX})\), which has a maximum there; it vanishes. For the second, \(|\operatorname{Tr}(AB)|\le\|A\|_{\rm op}\|B\|_{\rm tr}\), \(\|X\|_{\rm op}\le\rho\) and \(e^\rho-1-\rho\le\rho^2\) for \(\rho\le1\) give a lower bound \(-\rho^2n_sN\). Therefore
\[
\Phi(U)\ \ge\ M-\tfrac{\pi^2}{4}n_sN\,r^2\qquad\text{whenever }\|U-U_*\|_{\rm HS}\le r\le\tfrac1{2\sqrt N}.
\tag{2.2}
\]

*Step 2: a disjoint ball of the same radius.* There is \(Y\in SU(N)\) with \(\|Y-W\|_{\rm HS}\ge2\tau\) and \(\|Y-U_*\|_{\rm HS}<4\tau\). If \(\|U_*-W\|_{\rm HS}\ge2\tau\) take \(Y=U_*\). Otherwise the continuous function \(U\mapsto\|U-W\|_{\rm HS}\) on the connected group vanishes at \(W\) and equals \(2\sqrt2>2\tau\) at \(W\operatorname{diag}(-1,-1,1,\dots,1)\); choose \(Y\) where it equals \(2\tau\). Then \(B(Y,\tau)\cap B(W,\tau)=\varnothing\) and \(B(Y,\tau)\subset B(U_*,5\tau)\), with \(5\tau\le1/(2\sqrt N)\).

*Step 3.* By (2.2) with \(r=5\tau\) and \(\beta\tau^2=2t\),
\[
\int_{G\setminus B(W,\tau)}e^{\beta(\Phi-M)}\,dU\ \ge\int_{B(Y,\tau)}e^{\beta(\Phi-M)}\,dU\ \ge\ e^{-C_1t}h(\tau),
\qquad
\int_{B(W,\tau)}e^{\beta(\Phi-M)}\,dU\ \le\ h(\tau).
\]
Thus the conditional odds of \(\{e_p\ge t\}\) against its complement are at least \(e^{-C_1t}\), and the conditional probability is at least \(e^{-C_1t}/(1+e^{-C_1t})\ge\tfrac12e^{-C_1t}\). \(\square\)

### 2.2 The first-step label: a two-sided probability

For a finite nonempty plaquette set \(\Pi\) and \(\varepsilon_0>0\) put
\[
E_\Pi:=\Bigl\{\max_{p\in\Pi}|U(\partial p)-1|\ge\varepsilon_0\Bigr\},\qquad P_0:=\tfrac12\beta\varepsilon_0^2.
\tag{2.3}
\]
By (S1) the first-step large-field label of a cube \(\square\) is \(E_\Pi\) with \(\Pi=\{p\subset\square^\sim\}\), \(|\Pi|\le6(LM_2R_0+2)^4\); and \(P_0\) is a fixed multiple of \(p_0(g_0)^2\).

### Corollary 2.2 — deduction for the lower bound, (b: K-02) for the upper bound

On \(E_\Pi\), \(\max_{p\in\Pi}e_p\ge P_0\). If \(\varepsilon_0\le1/(10N)\) then, for every \(p\in\Pi\),
\[
\tfrac12e^{-C_1NP_0}\ \le\ \mathbb P(e_p\ge NP_0)\ \le\ \mathbb P(E_\Pi)\ \le\ |\Pi|\,K\,e^{-\eta P_0}.
\tag{2.4}
\]

**Proof.** By (1.2), \(|U_p-1|\ge\varepsilon_0\) implies \(s(U_p)\ge\varepsilon_0^2/2\), i.e. \(e_p\ge P_0\); and \(e_p\ge NP_0\) means \(\|U_p-1\|_{\rm HS}\ge\sqrt N\varepsilon_0\), which implies \(|U_p-1|\ge\varepsilon_0\). The lower bound is Lemma 2.1 with \(t=NP_0\le\beta/(200N)\). The upper bound is the union bound and \(\mathbb P(e_p\ge P_0)\le e^{-\eta P_0}\mathbb Ee^{\eta e_p}\le Ke^{-\eta P_0}\). \(\square\)

## 3. An obstruction: retained labels keep transported marks at their birth scale

### Theorem 3.1 — conditional expectations on a retained event

Let \((\Omega,\mathcal A,\mathbb P)\) be a probability space, \(O\in L^1\), \(\mathcal F\subset\mathcal A\) a σ-field and \(E'\in\mathcal F\) with \(\mathbb P(E')>0\). Then for every \(1\le r\le\infty\),
\[
\bigl\|\mathbb E[O\mid\mathcal F]\bigr\|_{L^r}\ \ge\ \mathbb P(E')^{1/r}\,\bigl|\mathbb E[O\mid E']\bigr|.
\tag{3.1}
\]

**Proof.** Put \(Y=\mathbb E[O\mid\mathcal F]\). Since \(E'\in\mathcal F\), \(\mathbb E[Y\mathbf 1_{E'}]=\mathbb E[O\mathbf 1_{E'}]\). Hölder gives \(|\mathbb E[Y\mathbf 1_{E'}]|\le\|Y\|_r\,\mathbb P(E')^{1-1/r}\). Divide. \(\square\)

### Theorem 3.2 — the scalar mark on a sector that forces microscopic energy

Let \(\mathbb P\) be any probability law on a space carrying a lattice gauge field with Wilson(\(\beta\)) marginal, \(\mathcal F\) any σ-field, \(X\) a finite plaquette set, \(P_{\min}>0\), and \(E'\in\mathcal F\), \(\mathbb P(E')>0\), an event on which \(E_X\ge P_{\min}\) pointwise. Then there is a vertex \(x_*\) of a plaquette of \(X\) such that for every \(1\le r\le\infty\)
\[
\boxed{\ \bigl\|\mathbb E[O_{x_*}\mid\mathcal F]\bigr\|_{L^r}\ \ge\ \mathbb P(E')^{1/r}\,a^{-4}\Bigl(\frac{P_{\min}}{4|X|}-C_E\Bigr).\ }
\tag{3.2}
\]

**Proof.** \(\sum_{p\in X}\mathbb E[e_p;E']=\mathbb E[E_X;E']\ge P_{\min}\mathbb P(E')\), so some \(p_*\in X\) has \(\mathbb E[e_{p_*}\mid E']\ge P_{\min}/|X|\). Let \(x_*\) be a vertex of \(p_*\). By (1.1) and \(e_p\ge0\), \(a^4\beta w_a(x_*)\ge\tfrac14e_{p_*}\), hence \(\mathbb E[a^4O_{x_*}\mid E']\ge P_{\min}/(4|X|)-C_E\). Apply Theorem 3.1. \(\square\)

No property of the event beyond \(\mathcal F\)-measurability and the pointwise energy bound is used: no independence, no structure of the lift, no information on how the other variables are distributed.

### Corollary 3.3 — the M-03 averaged norm at a later scale — deduction, given (Ret)

Assume \(\varepsilon_0\le1/(10N)\) and \(P_0\ge\max\{1,\,8|\Pi|C_E\}\). Let \(j\ge1\) be a step with \(E_\Pi\in\mathcal F_j\). Then there is a vertex \(x_*\) of a plaquette of \(\Pi\) with
\[
\bigl\|Q_jO_{x_*}\bigr\|_{L^r}\ \ge\ \bigl(\tfrac12e^{-C_1NP_0}\bigr)^{1/r}a^{-4}\frac{P_0}{8|\Pi|}\qquad(1\le r\le\infty),
\tag{3.3}
\]
\[
\boxed{\ h_j^4\,\mathfrak m_1\bigl(Q_jO_{x_*};\mu_{h_j}\bigr)\ \ge\ \frac{e^{-C_1N}}{16\,|\Pi|}\,L^{4j},\ }
\tag{3.4}
\]
and for every integer \(m\ge1\)
\[
\mathbb E\bigl|h_j^4Q_jO_{x_*}\bigr|^m\ \ge\ \tfrac12e^{-C_1NP_0}\,L^{4jm}\Bigl(\frac{P_0}{8|\Pi|}\Bigr)^m.
\tag{3.5}
\]
The lower bound (3.4) holds for the M-03 value norm of **every** carrier representation of \(Q_jO_{x_*}\).

**Proof.** (3.3) is (3.2) with \(E'=E_\Pi\), \(X=\Pi\), \(P_{\min}=P_0\) (Corollary 2.2), using (2.4) and \(P_0/(4|\Pi|)-C_E\ge P_0/(8|\Pi|)\). For (3.4) take \(r=P_0\ge1\) in (M.8): \(\mathfrak m_1\ge P_0^{-1}\|Q_jO_{x_*}\|_{L^{P_0}}\ge P_0^{-1}\cdot\tfrac12e^{-C_1N}a^{-4}P_0/(8|\Pi|)\). (3.5) is (3.3) with \(r=m\). If \(Q_jO_{x_*}=\sum_\tau A_\tau\) is a carrier representation, then \(\sum_\tau w_h(X_\tau)\mathfrak m_1(A_\tau^\sharp)\ge\mathfrak m_1(\sum_\tau A_\tau)\) because \(w_h\ge1\), \(A^\sharp\ge|A|\) and \(\mathfrak m_1\) is a monotone seminorm. \(\square\)

### Corollary 3.4 — no cutoff-uniform all-order budget — deduction, given (Ret) and (S3), (S4)

Suppose that along a cutoff family with \(g_0\to0\) one had constants \(C,d\) with
\(\sup_{j,x}\mathbb E|h_j^4Q_jO_x|^m\le C^m(m!)^d\) for all \(m\ge1\) and all cutoffs. Take \(m=\lceil P_0\rceil\) and \(j=N_B-1\) in (3.5). Since \(P_0/m\le1\) and \((m!)^{d/m}\le m^d\),
\[
C\ \ge\ \tfrac12\,e^{-C_1N}\,\frac{P_0}{8|\Pi|}\,(P_0+1)^{-d}\,L^{4(N_B-1)}.
\]
With \(N_B\ge R_0\ge(\log g_0^{-2})^r\), \(|\Pi|\le6(LM_2R_0+2)^4\) and \(P_0\asymp(\log g_0^{-2})^{2p_0}\), the right side tends to infinity as \(g_0\to0\). Hence no such pair \((C,d)\) exists. The offending orders are \(m\approx P_0\to\infty\); for each *fixed* \(m\) there is no obstruction once \(g_0\) is small (Theorems 4.4–4.5).

### Remarks

**3.5 What exactly is obstructed.** (i) The averaged part of the M-03 norm of the exact one-field transported jet at steps \(1\le j<N_B\) is at least \(c\,L^{4j}/|\Pi|\); since \(|\Pi|\asymp R_0^4\) and \(L^{N_0-1}=R\) (S3), this exceeds any fixed constant once \(j\ge N_0+C\), i.e. during almost the whole unreplaced lifetime \(N_B\gg N_0\). The M-03/M-06 induction budget "uniformly bounded norm of the transported jet" therefore fails for the literal norm, independently of any H-02 probability estimate. (ii) The all-\(r\) budget \(\|F_{i,k}\|_{L^r(\mu_k)}\le Ar^sh_k^{-4}[1+\log(\ell_0/h_k)]^b\) of manuscript §5, and the premise \(\|A_{\alpha,k}\|_r\le Cb_{\alpha,k}r^s\) with a current-scale \(b\) in Annex A (6.2), fail at \(r\approx P_0\) by the factor \(L^{4j}r^{1-s}/|\Pi|\). (iii) the finite-cutoff construction condition (1), \(cB\ge C_1(\dots+dG^{1/d})\), was recorded as "a constraint on this majorization". For \(d=1\) it is in fact *necessary* for the averaged norm: (3.4) says the norm is \(\ge c\,G/\log(1/q)\) with \(G=L^{4j}\), \(q=\mathbb P(E')\). (iv) Nothing here contradicts fixed-order estimates, and nothing is asserted about the physical correlations; the statement concerns a norm that takes all moment orders with a polynomial weight.

**3.5a Later births.** For a label born at a step \(b\ge1\) the same mechanism is expected with \(a,P_0\) replaced by \(h_b,P_b\) (an additional hypothesis). Theorem 3.2 itself gives nothing there: the label forces energy only in a set \(X\) of order \(L^{4b}\) fine plaquettes, and the right side of (3.2) is then negative. A proof would need a lower bound for the label probability and for the scale-\(b\) transported mark on the label.

**3.6 Coarser retained labels.** If only the resummed region is retained (CMP 119 p.248 resums \(P_0,P_1,Q_1\) at fixed \(\Omega_1\)), apply Theorem 3.2 to \(E'=\{\square\subset\Omega_1^c\}\supset E_\Pi\). The probability factor only improves. The energy hypothesis "\(E_X\ge P_{\min}\) on \(E'\)" then requires the source implication *every first-step flag forces Wilson energy at least \(c\min(A_0,A_1)^2p_0^2(g_0)\) in a bounded neighbourhood*, which is how the factors in (S4) are obtained; The proof assumes that implication from the action expansion for the Q and R flags, so for coarser labels the conclusion is conditional with that named input. Under the primitive-label convention of H-01 the corollaries above are unconditional given (Ret).

**3.7 Why (Ret) cannot be designed away.** A lift that forgets the label before step \(N_B\) cannot apply the R operation with a kernel that is a function of retained data, because eligibility (S3)(ii) depends on the label. Forgetting the label *after* a completed reset is exactly what the accepted H-03 reset does, and the obstruction then disappears for that component. The obstruction is thus attached precisely to the sector H-02 is about: retained, not yet reset.

**3.8 Relation to the finite-cutoff construction remark.** the finite-cutoff construction finding that a genuine selector jump has infinite strong divided-current norm concerns the current part \(j_{h,m,X}\). (3.4) is a statement about the value part alone and uses no differentiation.

## 4. The first-step lineage: joint probability at the current scale and a sharp window

This section closes one unreplaced sector completely: large-field regions all of whose births are first-step \(P_0\) flags (S1), observed at a later scale \(j\) while still unreplaced. Its birth events are microscopic, so the probability input is the compact reserve; what is new is the *current-scale* joint statement with all geometric costs, and the two-sided window.

### Lemma 4.1 — joint probability of first-step labels — (b: K-02)

Let \(\mathcal Q\) be a family of plaquette sets with \(|\Pi|\le n_\Pi\) for \(\Pi\in\mathcal Q\), such that every plaquette belongs to at most \(\mu_0\) members. For distinct \(\Pi_1,\dots,\Pi_n\in\mathcal Q\),
\[
\mathbb P\Bigl(\bigcap_{i=1}^nE_{\Pi_i}\Bigr)\ \le\ \bigl(n_\Pi K e^{-\eta P_0/\mu_0}\bigr)^n.
\tag{4.1}
\]

**Proof.** On the intersection choose \(p_i\in\Pi_i\) with \(e_{p_i}\ge P_0\) (Corollary 2.2). Let \(X=\{p_1,\dots,p_n\}\) as a set. A plaquette equals \(p_i\) for at most \(\mu_0\) indices, so \(nP_0\le\sum_ie_{p_i}\le\mu_0E_X\). Hence
\(\mathbf 1_{\cap E_{\Pi_i}}\le\sum_{(p_i)\in\prod\Pi_i}\exp\{\eta(E_{X}-nP_0/\mu_0)\}\).
Take expectations and use \(\mathbb Ee^{\eta E_X}\le K^{b(X)}\le K^n\); there are at most \(n_\Pi^n\) tuples. \(\square\)

For the family (S1), \(n_\Pi\le6(LM_2R_0+2)^4\) and \(\mu_0\le3^4\) (a plaquette lies in \(\square^\sim\) for at most \(3^4\) cubes of a partition). No independence of the labels is used, and the sets may overlap.

### Theorem 4.2 — current-scale joint probability — (b: K-02)

Fix \(j\ge1\) and an integer \(\rho\ge1\). A *scale-\(j\) cell* is a cube of side \(L^j\) fine spacings in a fixed partition. For a cell \(c\) let \(\mathcal Q(c,\rho)\) be the set of \(\Pi\in\mathcal Q\) within sup-distance \(\rho L^j\) (fine units) of \(c\), and
\[
A_c:=\bigcup_{\Pi\in\mathcal Q(source input; \rho)}E_\Pi ,\qquad
N_{j,\rho}:=\sup_c|\mathcal Q(source input; \rho)| ,\qquad
\delta_j:=1+\Bigl\lceil L^{-j}\max_{\Pi\in\mathcal Q}\operatorname{diam}\Pi\Bigr\rceil.
\]
Then for every deterministic finite set \(S\) of scale-\(j\) cells,
\[
\boxed{\ \mathbb P\Bigl(\bigcap_{c\in S}A_c\Bigr)\ \le\ e^{-\sigma_j|S|},\qquad
\sigma_j:=\frac{\bigl[\eta P_0/\mu_0-\log(N_{j,\rho}\,n_\Pi K)\bigr]_+}{(4\rho+2\delta_j+1)^4}.\ }
\tag{4.2}
\]
For the family (S1), \(N_{j,\rho}\le((2\rho+1)L^j+2)^4\).

**Proof.** Measure the distance between two cells by the sup-distance of their integer indices. Choose \(S^\circ\subset S\) maximal with pairwise index distance greater than \(2\rho+\delta_j\); by maximality every cell of \(S\) is within index distance \(2\rho+\delta_j\) of \(S^\circ\), so \(|S^\circ|\ge|S|/(4\rho+2\delta_j+1)^4\). The families \(\mathcal Q(c,\rho)\), \(c\in S^\circ\), are pairwise disjoint: two cells at index distance \(k\) are at fine distance at least \((k-1)L^j\), and a common member \(\Pi\) would force \((k-1)L^j\le2\rho L^j+\operatorname{diam}\Pi\), i.e. \(k\le2\rho+\delta_j\). On \(\bigcap_{c\in S^\circ}A_c\) choose \(\Pi_c\in\mathcal Q(c,\rho)\) with \(E_{\Pi_c}\); the \(\Pi_c\) are distinct. Sum (4.1) over the at most \(N_{j,\rho}^{|S^\circ|}\) choices. If the bracket in (4.2) is nonpositive the bound is trivial. \(\square\)

### Remark 4.3 — the lineage dictionary — source input, not used in any proof

By (S4), if no large field is created near a region \(Z\) of step 1, its step-\(j\) descendant is \(S^{j-1}(Z)\subset\bigcup_{\square_0}\square_0^{\sim31}\), \(\square_0\) the \(MR_j\)-cubes covering \(Z\). Consequently a scale-\(j\) unit cell lying in a clean descendant of regions generated by \(P_0\) flags satisfies \(A_c\) with \(\rho=\rho_j\le33MR_j\) (the fixed first-step layers of CMP 119 (1.10) are absorbed in the last unit). With this \(\rho\),
\[
\sigma_j\ \ge\ \frac{\eta P_0/81-4\log(67MR_jL^j+2)-\log\bigl(6K(LM_2R_0+2)^4\bigr)}{(132MR_j+2M_2R_0+9)^4}
\]
(using \(\delta_j\le M_2R_0+4\) for \(j\ge1\)). Since \(P_0\asymp(\log g_0^{-2})^{2p_0}\), \(R\asymp(\log g^{-2})^{r}\), \(p_0\ge5r\), and \(j<N_B\) with \(N_B\) of order \(R\) (S3, S4), the numerator is of order \((\log g_0^{-2})^{2p_0}\) while the subtracted terms and the denominator are of order at most \((\log g_0^{-2})^{r}\) and \((\log g_0^{-2})^{4r}\); hence \(\sigma_j\to\infty\) as \(g_0\to0\), uniformly in \(1\le j<N_B\) and in the volume. In particular \(\sigma_j\) exceeds the carrier threshold \(\kappa+\log A\) of Annex AC, Corollary H.3a, for the weight (M.2) and connected carriers.

### Theorem 4.4 — windowed sector bounds for the complete transported jet

Let \((\Omega,\mathbb P)\) be a probability space, \(\mathcal F\) a σ-field, \(Q=\mathbb E[\,\cdot\mid\mathcal F]\), and \(E\in\mathcal F\) with \(\mathbb P(E)\le e^{-\lambda}\). Let \(F_1,\dots,F_m\) satisfy \(\|F_i\|_{L^p}\le b_{\rm in}p^s\) for all \(p\ge1\), let \(0<b_{\rm cur}\le b_{\rm in}\) and \(G=b_{\rm in}/b_{\rm cur}\). Then for every real \(r\ge1\) with
\[
r\,m\,\log G\ \le\ \lambda/4
\tag{4.3}
\]
one has
\[
\Bigl\|\mathbf 1_E\,Q\Bigl(\prod_iF_i\Bigr)\Bigr\|_{L^r}\le(2rm)^{sm}\,b_{\rm cur}^m\,e^{-\lambda/(4r)},
\qquad
\bigl\|\mathbf 1_E\,\kappa_Q(F_1,\dots,F_m)\bigr\|_{L^r}\le m!\,2^{m-1}(2rm)^{sm}\,b_{\rm cur}^m\,e^{-\lambda/(4r)}.
\tag{4.4}
\]

**Proof.** Since \(E\in\mathcal F\), \(\mathbf 1_EQ(Z)=Q(\mathbf 1_EZ)\). Conditional Jensen and Hölder give, for any \(q\ge1\) and any \(Z\),
\(\|\mathbf 1_EQ(Z)\|_q\le\|\mathbf 1_EZ\|_q\le\mathbb P(E)^{1/(2q)}\|Z\|_{2q}\).
With \(Z=\prod_iF_i\), \(q=r\) and \(\|Z\|_{2r}\le\prod_i\|F_i\|_{2rm}\) this is at most \(e^{-\lambda/(2r)}b_{\rm in}^m(2rm)^{sm}=b_{\rm cur}^m(2rm)^{sm}\exp\{-\lambda/(2r)+m\log G\}\), and (4.3) gives the first bound. For the cumulant use (H.7). In a partition \(\mathcal P\), \(\mathbf 1_E\prod_BQ(\prod_{i\in B}F_i)=\prod_B\mathbf 1_EQ(\prod_{i\in B}F_i)\). Hölder across the blocks with exponents \(rm/|B|\ge1\), then the displayed inequality with \(q=rm/|B|\), and \(\|\prod_{i\in B}F_i\|_{2rm/|B|}\le\prod_{i\in B}\|F_i\|_{2rm}\), bound the \(L^r\) norm of each term by \(\mathbb P(E)^{1/(2r)}\prod_i\|F_i\|_{2rm}\). The sum of the absolute coefficients \((|\mathcal P|-1)!\) is at most \(m!2^{m-1}\) (Annex A, proof of (4.9)). \(\square\)

The statement is about the sector part of the *exact* transported coefficients; no clipping of the marks and no conditional normalizer occurs. For the microscopic F-01 fields, K-02 gives \(b_{\rm in}=C_Oa^{-4}\), \(s=1\) (Annex A (3.8)); at step \(j\), \(b_{\rm cur}=C_Oh_j^{-4}\) and \(G=L^{4j}\).

### Theorem 4.5 — the window is sharp for the first-step sector — (a)+(b: K-02), given (Ret)

Let \(E=\bigcap_{i\le n}E_{\Pi_i}\) for distinct first-step sets, \(E\in\mathcal F_j\), and \(\lambda_n:=n(\eta P_0/\mu_0-\log(n_\Pi K))\). Then:

1. *(inside)* for all \(r\ge1\), \(m\ge1\) with \(r\,m\le\lambda_n/(16\,j\log L)\), the sector part of every transported product or conditional-cumulant coefficient of \(m\) microscopic F-01 fields obeys (4.4) with \(b_{\rm cur}=C_Oh_j^{-4}\);
2. *(outside, \(n=1\))* under the hypotheses of Corollary 3.3, for all \(r\ge r_+(j):=C_1NP_0/(2j\log L)\),
\[
h_j^4\bigl\|\mathbf 1_{E_\Pi}Q_jO_{x_*}\bigr\|_{L^r}\ \ge\ \tfrac12L^{2j}\,\frac{P_0}{8|\Pi|}.
\]

So the critical moment order of this sector satisfies \(c\,P_0/(j\log L)\le r_{\rm crit}(j)\le C\,P_0/(j\log L)\) with constants depending only on \(N,\eta,K,\mu_0\) and \(\log n_\Pi/P_0\). For \(1\le j<N_B\) the window bound \(\lambda_1/(16j\log L)\) is at least \(\lambda_1/(16N_B\log L)\), which tends to infinity as \(g_0\to0\) because \(P_0\asymp(\log g_0^{-2})^{2p_0}\), \(N_B\) is of order \(R_0\asymp(\log g_0^{-2})^r\) and \(p_0\ge5r\) (S1, S4).

**Proof.** 1 is Lemma 4.1 and Theorem 4.4 with \(G=L^{4j}\). For 2, the proof of Theorem 3.1 applied to \(Y\mathbf 1_{E_\Pi}\) gives \(\|\mathbf 1_{E_\Pi}Q_jO_{x_*}\|_r\ge\mathbb P(E_\Pi)^{1/r}|\mathbb E[O_{x_*}\mid E_\Pi]|\); insert (2.4) and note \(e^{-C_1NP_0/r}\ge L^{-2j}\) for \(r\ge r_+(j)\). \(\square\)

### 4.5 The reformulated completion test H-02′

Theorems 3.2 and 4.5 require a window in any pointwise compensation bound. The following formulation gives the corresponding integrated estimate.

> **H-02′.** For every admissible scale \(j\) and every class of retained bad sectors (unreplaced components, low-margin clusters, preparatory failures), with label events \(E_D\in\mathcal F_j\) indexed by their current-scale footprints \(D\) and birth scales \(b(D)\le j\):
> 1. **Joint probability.** \(\mathbb P(\bigcap_iE_{D_i})\le\exp(-\sum_i\lambda(D_i))\) for distinct footprints, conditionally on the retained data outside a declared neighbourhood, with \(\lambda(D)\ge\sigma\,|D|\) and \(\sigma>2(\kappa+\log A)\) for the actual carrier weight and count;
> 2. **Windowed compensation.** For all moment and source orders with \(r\,m\le\lambda(D)/(16\,(j-b(D))\log L)\), the sector part of the exact transported jet obeys the current-scale budget (this is then automatic from 1 by Theorem 4.4, given the birth-scale budget of the marks);
> 3. **Window growth.** The window bound in 2 tends to infinity as the coupling at the birth scale tends to zero, uniformly in volume, depth and history; at scales whose coupling is bounded below the loss \(L^{4(j-b)m}\) is a cutoff-independent constant to the power \(m\).
> No compensation is claimed outside the window; by Theorem 3.2 none is possible in a norm taking all moment orders.

Downstream, the supremum over \(p\ge1\) in (M.8) has to be replaced by a supremum over the window (or the sector parts must be carried as separate records with the factor \(e^{-\lambda/(4r)}\) of (4.4)); this affects the criterion of M-06, H-04 and M-07 and is outside this proposition's authority. For a fixed-order Schwinger function only finitely many \((r,m)\) occur, and clause 3 places them inside the window for all sufficiently fine cutoffs; clause 3 for the first-step sector is Remark 4.3.

**What §4 does not cover.** Births at steps \(b\ge1\) (coarse events), P-flags, preparatory failures, components kept alive beyond \(N_B\) by later births, and components that are too large for condition (i). For those, clause 1 is the open problem; §5 is a contribution to it.

## 5. Inherited low-margin sectors: a surgery theorem

### 5.1 The problem and the structural fact that solves its combinatorial half

A P-flag at step \(k+1\) is an event of the retained field (S2). Conditionally on the field outside a block its probability need not be small: the exterior can force curvature into the block, and a filling that satisfies the selected support may not exist near the cheapest one. This is the "low-margin" phenomenon of Annex A §§6–7, where (6.1) splits failures into low-margin centres and a predictable remainder and leaves the low-margin probability open. The usual Peierls argument fails for the same reason: with one threshold, the cells just below threshold in the collar make the extension as expensive as the interior.

The source supplies one fact that removes this difficulty: **the inherited window has bounded ratio**. By (S2) the old selector already confines the new field to \(|V_{k+1}(\partial p')-1|<2L^2\varepsilon_k\), while the new test is at the scale \(\varepsilon_{k+1}\); and the regularity imposed by \(\chi_k\) (CMP 119 p.266, (3.8): \(|U_{k,\square}(\partial p)-1|<\varepsilon_k\eta^2\) on the fine plaquettes; LFR I (1.3)) bounds the background action of every unit cell of the old small-field region by about \(3N\varepsilon_k^2/g_k^2\). So every "bad" cell costs at least \(P_*\) and *no* cell costs more than \(C_{\rm cap}P_*\), with \(C_{\rm cap}\) a pure constant. Under such a cap a pigeonhole over nested neighbourhoods always finds a surgery domain with a factor-two energy margin (Lemma 5.1), and clusters of bad cells have good collars by construction (Lemma 5.2). What remains is an analytic *local domination* property (LD) of the conditional density, which is the honest content of the missing "local ratio/surgery theorem" named in Annex AK §6.

### 5.2 Setting

* \(\Lambda\) is a finite set of cells with a metric \(\operatorname{dist}\) taking integer values; \(A^{+r}=\{c:\operatorname{dist}(c,A)\le r\}\); \(|\{c\}^{+r}|\le v(r)\) with \(v\) nondecreasing, \(v\ge1\). A set is *\(r\)-connected* if it is connected in the graph joining cells at distance \(\le r\).
* \((\mathbb X_c,\lambda_c)\), \(c\in\Lambda\), are standard Borel probability spaces, \(\mathbb X=\prod_c\mathbb X_c\), \(\lambda=\bigotimes\lambda_c\); for \(D\subset\Lambda\), \(x=(x_D,x_{D^c})\). \((\Xi,\tau)\) is a σ-finite parameter space.
* \(f:\Xi\times\mathbb X\to[0,\infty)\) is measurable and integrable for \(\tau\otimes\lambda\). It vanishes outside a measurable set \(\mathcal S\).
* \(W\subset\Lambda\) is the *window*. For \(c\in W\), \(e_c:\mathcal S\to[0,\infty)\) is measurable; \(e(A)=\sum_{c\in A}e_c\).
* Constants: \(P_*>0\), \(C_{\rm cap}\ge1\), \(C_{\rm ext}\ge1\), an integer \(r_0\ge1\), \(c_F\ge0\), \(\nu\in(0,1]\), \(v_{\max}\in\mathbb N\cup\{\infty\}\).

For \(z=(\xi,x)\in\mathcal S\) the **bad set** is \(\mathfrak B(z)=\{c\in W:e_c(z)\ge P_*\}\). A pair \((D^-,D)\) is *admissible* if \(D^-\subset W\), \(D=(D^-)^{+r_0}\subset W\) and \(|D|\le v_{\max}\); its *collar* is \(D\setminus D^-\), and the collar is *good* at \(z\) if it contains no bad cell.

**(H1) Cap.** \(e_c(z)\le C_{\rm cap}P_*\) for all \(z\in\mathcal S\), \(c\in W\).

**(LD) Local domination.** For every admissible \((D^-,D)\) there is a measurable set \(\mathcal N_D\subset\Xi\times\mathbb X_D\times\mathbb X_{D^c}\) such that, for every \(z=(\xi,x)\in\mathcal S\) whose collar is good, the section \(N=\{y\in\mathbb X_D:(\xi,y,x_{D^c})\in\mathcal N_D\}\) satisfies \(\lambda_D(N)\ge\nu^{|D|}\) and
\[
f(\xi,x)\ \le\ \exp\Bigl\{-\bigl[e(D^-)-(C_{\rm ext}-1)\,e(D\setminus D^-)\bigr](z)+c_F|D|\Bigr\}\ f(\xi,y,x_{D^c})\qquad\text{for all }y\in N.
\tag{5.1}
\]
The set \(N\) depends on the configuration only through \((\xi,x_{D^c})\).

Put
\[
\gamma=\frac1{2C_{\rm ext}},\qquad
K=\min\{k\ge1:(1+\gamma)^k\ge C_{\rm cap}\,v(kr_0)\},\qquad
\rho_1=Kr_0,\qquad v_1=v(\rho_1).
\tag{5.2}
\]
\(K\) is finite because \(v\) is polynomially bounded in the applications (on a four-dimensional lattice \(v(r)=(2r+1)^4\)); it depends only on \(C_{\rm cap},C_{\rm ext},r_0\) and \(v\).

### Lemma 5.1 — energy-margin pigeonhole

Assume (H1). Let \(z\in\mathcal S\) and let \(S'\subset\mathfrak B(z)\) be finite and nonempty with \(S'^{+\rho_1}\subset W\). Put \(D_i=S'^{+ir_0}\), \(0\le i\le K\). Then there is \(i\in\{0,\dots,K-1\}\) with
\[
e(D_{i+1}\setminus D_i)\le\gamma\,e(D_i),\qquad\text{hence}\qquad
e(D_i)-(C_{\rm ext}-1)\,e(D_{i+1}\setminus D_i)\ \ge\ \tfrac12e(D_i)\ \ge\ \tfrac12|S'|P_*.
\tag{5.3}
\]

**Proof.** \(E_i:=e(D_i)(z)\) is nondecreasing, \(E_0\ge|S'|P_*\) since the cells of \(S'\) are bad, and \(E_K\le C_{\rm cap}P_*|D_K|\le C_{\rm cap}P_*|S'|v(Kr_0)\) by (H1). If \(E_{i+1}>(1+\gamma)E_i\) for all \(i<K\) then \(E_K>(1+\gamma)^K|S'|P_*\ge C_{\rm cap}v(Kr_0)|S'|P_*\), a contradiction. For the chosen \(i\), \((C_{\rm ext}-1)\gamma\le\tfrac12\). \(\square\)

### Lemma 5.2 — clusters have good collars

For \(S\subset W\) and \(z\in\mathcal S\) let \(\mathcal C_S(z)\) be the union of the \(\rho_1\)-connected components of \(\mathfrak B(z)\) that meet \(S\). Then \(\mathcal C_S(z)^{+\rho_1}\setminus\mathcal C_S(z)\) contains no bad cell.

**Proof.** A bad cell within distance \(\rho_1\) of a component belongs to that component. \(\square\)

### Theorem 5.3 — joint probability of bad cells from local domination

Assume (H1) and (LD). For a finite nonempty \(S\subset W\) let
\[
G_S=\bigl\{z\in\mathcal S:\ S\subset\mathfrak B(z),\ \ \mathcal C_S(z)^{+\rho_1}\subset W,\ \ v_1|\mathcal C_S(z)|\le v_{\max}\bigr\}.
\]
Then for every measurable \(\Phi\ge0\) depending only on \((\xi,x_{\Lambda\setminus W})\),
\[
\int\!\!\int f\,\mathbf 1_{G_S}\,\Phi\,d\tau\,d\lambda\ \le\
K\sum_{n\ge|S|}\bigl(4v_1^2\bigr)^n\exp\Bigl\{-n\Bigl[\tfrac12P_*-v_1\bigl(c_F+\log\tfrac1\nu\bigr)\Bigr]\Bigr\}\int\!\!\int f\,\Phi\,d\tau\,d\lambda.
\tag{5.4}
\]
In particular, if
\[
\sigma_*:=\tfrac12P_*-v_1\bigl(c_F+\log\tfrac1\nu\bigr)-\log(4v_1^2)\ \ge\ \log2,
\tag{5.5}
\]
then
\[
\boxed{\ \int\!\!\int f\,\mathbf 1_{G_S}\,\Phi\ \le\ 2K\,e^{-\sigma_*|S|}\int\!\!\int f\,\Phi.\ }
\tag{5.6}
\]
Equivalently: under the probability law proportional to \(f\,d\tau\,d\lambda\), the conditional probability of \(G_S\) given the parameter and everything outside the window is at most \(2Ke^{-\sigma_*|S|}\) almost surely. \(S\) is arbitrary: no separation, connectedness or disjointness is assumed.

**Proof.** *Step 1 (reduction to finitely many shapes).* Let \(z\in G_S\), \(S'=\mathcal C_S(z)\), \(n=|S'|\ge|S|\). By Lemma 5.2 every collar \(D_{i+1}\setminus D_i\subset S'^{+\rho_1}\setminus S'\), \(i<K\), is good. By Lemma 5.1 there is \(i<K\) with (5.3). The pair \((D_i,D_{i+1})\) is admissible: \(D_{i+1}\subset S'^{+\rho_1}\subset W\) and \(|D_{i+1}|\le nv_1\le v_{\max}\). Hence
\[
G_S\subset\bigcup_{S'}\bigcup_{i<K}G_{S',i},\qquad
G_{S',i}:=\Bigl\{z\in\mathcal S:\ (D_{i+1}\setminus D_i)\cap\mathfrak B(z)=\varnothing,\ \ \bigl[e(D_i)-(C_{\rm ext}-1)e(D_{i+1}\setminus D_i)\bigr](z)\ge\tfrac12|S'|P_*\Bigr\},
\]
the union over sets \(S'\supset S\), \(S'^{+\rho_1}\subset W\), \(v_1|S'|\le v_{\max}\), each of whose \(\rho_1\)-components meets \(S\).

*Step 2 (one shape).* Fix \((S',i)\), \(n=|S'|\), \(D^-=D_i\), \(D=D_{i+1}\). For \(z=(\xi,x)\in G_{S',i}\), (5.1) holds for all \(y\) in the section \(N\); averaging over \(y\in N\) with respect to \(\lambda_D\) and using \(\lambda_D(N)\ge\nu^{|D|}\),
\[
f(\xi,x)\ \le\ e^{-nP_*/2+c_F|D|}\,\nu^{-|D|}\int_{\mathbb X_D}f(\xi,y,x_{D^c})\,\lambda_D(dy).
\]
The right side depends only on \((\xi,x_{D^c})\), as does \(\Phi\) (because \(D\subset W\)). Integrating over \(x_D\) with the probability measure \(\lambda_D\), then over \(x_{D^c}\) and \(\xi\) (Tonelli; joint measurability of \(\mathcal N_D\) is part of (LD)),
\[
\int\!\!\int f\,\mathbf 1_{G_{S',i}}\Phi\ \le\ \exp\bigl\{-\tfrac12nP_*+nv_1(c_F+\log\tfrac1\nu)\bigr\}\int\!\!\int f\,\Phi ,
\]
using \(|D|\le nv_1\).

*Step 3 (counting).* A \(\rho_1\)-connected set of \(m\) cells containing a given cell is determined by a depth-first walk of a spanning tree, at most \(v_1^{2m}\) possibilities. Order \(S=\{s_1,\dots,s_k\}\). A shape \(S'\) is determined by the tuple \((A_1,\dots,A_k)\), \(A_i\) the component of \(s_i\) if \(s_i\) is the first element of \(S\) in it and \(A_i=\varnothing\) otherwise. There are at most \(\binom{n+k-1}{k-1}\le4^n\) size vectors and at most \(v_1^{2n}\) tuples for each. Summing Step 2 over \(S'\) and the \(K\) values of \(i\) gives (5.4); (5.6) follows by the geometric series, whose ratio is at most \(\tfrac12\) under (5.5). \(\square\)

**Flags.** If a flag at a test cube forces a bad cell within distance \(r_f\) (input In-4 below), then for a set \(T\) of flagged cubes one takes a union bound over the choices of one bad cell per cube; \(|S|\ge|T|/v(2r_f)\) after removing coincidences, at the cost of \(v(r_f)^{|T|}\) choices.

### Proposition 5.4 — a sufficient form of (LD)

Suppose that on \(\mathcal S\)
\[
f=\exp(-\mathcal A+F)
\]
with measurable real \(\mathcal A,F\), and that there are a measurable \(\mathcal S^\flat\subset\mathcal S\) ("support with margin") and constants \(c_F',c_N\ge0\), \(\nu\in(0,1]\) such that for every admissible \((D^-,D)\):

* **(P2) bounded local oscillation.** \(|F(\xi,x)-F(\xi,\tilde x)|\le c_F'|D|\) whenever both points lie in \(\mathcal S\) and \(x_{D^c}=\tilde x_{D^c}\);
* **(P3) surgery.** for every \(z=(\xi,x)\in\mathcal S\) with good collar there is \(z'=(\xi,y',x_{D^c})\in\mathcal S^\flat\) with
  \(\mathcal A(z')\le\mathcal A(z)-e(D^-)(z)+(C_{\rm ext}-1)\,e(D\setminus D^-)(z)\);
* **(P4) neighbourhood.** for every \(z'=(\xi,x')\in\mathcal S^\flat\) there is a measurable \(B\subset\mathbb X_D\), \(\lambda_D(B)\ge\nu^{|D|}\), with \((\xi,y,x'_{D^c})\in\mathcal S\) and \(\mathcal A(\xi,y,x'_{D^c})\le\mathcal A(z')+c_N|D|\) for all \(y\in B\);
* **(P0) measurability.** \(m_D(\xi,\omega):=\inf\{\mathcal A(\xi,y,\omega):(\xi,y,\omega)\in\mathcal S^\flat\}\) is measurable (for instance \(\mathcal A\) continuous and \(\mathcal S^\flat\) closed in compact metric spaces).

Then (LD) holds with the same \(\nu\) and \(c_F=c_F'+c_N+1\).

**Proof.** Put \(\mathcal N_D=\{(\xi,y,\omega)\in\mathcal S:\mathcal A(\xi,y,\omega)\le m_D(\xi,\omega)+c_N|D|+1\}\). Let \(z=(\xi,x)\in\mathcal S\) have a good collar and \(\omega=x_{D^c}\). By (P3), \(m_D(\xi,\omega)\le\mathcal A(z)-\text{gain}(z)<\infty\), where gain is the bracket in (5.1). Choose \(z''\in\mathcal S^\flat\) over \((\xi,\omega)\) with \(\mathcal A(z'')\le m_D+1\); the set \(B\) of (P4) for \(z''\) lies in the section \(N\), so \(\lambda_D(N)\ge\nu^{|D|}\). For \(y\in N\): \(-\mathcal A(z)\le-m_D-\text{gain}(z)\le-\mathcal A(\xi,y,\omega)+c_N|D|+1-\text{gain}(z)\), and \(F(z)\le F(\xi,y,\omega)+c_F'|D|\) by (P2). Multiply. \(\square\)

The reference set is a sub-level set of the *conditional minimum* over the margin support. Annex A §7 observed that an estimate of fluctuations around a conditional minimum does not pay a retained flux; here the retained flux is paid by (P3), which compares the conditional minimum with the configuration itself, and the pigeonhole guarantees that the comparison has a margin.

### 5.5 Histories, parameters and several steps

**Corollary 5.5 — mixtures.** Let the law be \(\mathcal Z^{-1}\sum_h\tau_h(d\xi)f_h(\xi,x)\lambda(dx)\) over a countable set of history labels \(h\), and let \(\mathcal H\) be a set of labels for which (H1), (LD) hold with common constants and windows \(W_h\supset W\). Then for \(S\subset W\) and \(\Phi\ge0\) depending on \((h,\xi,x_{\Lambda\setminus W})\),
\(\mathbb E[\Phi;\,h\in\mathcal H,\,G_S]\le2Ke^{-\sigma_*|S|}\,\mathbb E[\Phi;\,h\in\mathcal H]\).
*Proof:* apply (5.6) for each \(h\) and sum. \(\square\)

Thus the bound is conditional on the history label, on all internal variables collected in \(\xi\) (in the application: integration variables of large-field operations and old fields whose footprint lies outside the window), and on the current field outside the window. This is the "retained-data dependence" clause of the criterion for this sector.

**Lemma 5.6 — predictable composition.** Let \(\mathcal G_1\subset\mathcal G_2\subset\cdots\) be σ-fields and \(B_i\in\mathcal G_{i+1}\) events with \(\mathbb P(A\cap B_i)\le q_i\mathbb P(A)\) for all \(A\in\mathcal G_i\). Then \(\mathbb P(\bigcap_{i\in I}B_i)\le\prod_{i\in I}q_i\) for every finite \(I\). *Proof:* induction on the largest index. \(\square\)

In the application \(\mathcal G_i\) must contain the earlier events. With Corollary 5.5 this is the case when the earlier events are functions of the history label, of \(\xi\) and of the field outside the current window — in particular for flags at *other places*. A second flag at a later step *inside the cone* of an earlier one is a different situation: the window of the later step is then not clean, and the joint bound requires (LD) across a large-field component (§5.7(c)).

### 5.6 Dictionary for the P-flags of CMP 119 (3.2), and the inputs it needs — conditional, inputs not verified here

Fix a step \(k\), a history label \(h\) through step \(k\) with large-field region \(Z_k(h)\), and work on the unit lattice of scale \(k\).

| Abstract object | Proposed instance |
|---|---|
| cells \(\Lambda\) | unit cubes of the scale-\(k\) lattice |
| \(\mathbb X_c,\lambda_c\) | the bond variables \(V_k\) attached to the cell, Haar |
| \(\xi\) | all internal integration variables of \(\mathbf T_k(Z_k)\) and old fields with footprint outside the window |
| \(f_h\) | the positive integrand of \(r_{k,h}\) (Annex W (4.1)) |
| window \(W_h\) | cells at distance \(\ge3LMR_{k+1}\) from \(Z_k'\) (inside the domain \((Z_k'^{\sim4})^c\) where (3.2) is applied) |
| \(\mathcal S\) | the support of \(\chi_k\) and of the other small-field functions on the window |
| \(\mathcal A\) | \(g_k^{-2}A(U_k(V))\), \(U_k\) the background minimizer |
| \(e_c\) | \(g_k^{-2}\) times the fine-lattice action of \(U_k\) in the block of \(c\) |
| \(P_*\) | \(c_*\,\varepsilon_k^2/g_k^2=c_*\,p_0(g_k)^2\) with a small fixed \(c_*\) |

The inputs, with their status:

* **In-1 (form and positivity).** On the window, \(f_h=\mathbf 1_{\mathcal S}\exp(-\mathcal A+F)\) with \(F\) collecting every other term (vacuum and normalization constants, \(\mathbf E,\mathbf R,\mathbf B\), Jacobians, the logarithm of the positive large-field operations). Source: CMP 119 (2.18)–(2.27), (2.49); positivity is asserted in LFR I p.176 and LFR II p.380. *Hypotheses: the form is the inductive representation; An additional assumption is that every term can be written on the real support with the sign conventions of Annex W §6.2.*
* **In-2 (bounded local oscillation of \(F\)), i.e. (P2).** A change of \(V_k\) inside \(D\subset W_h\) changes \(F\) by at most \(c_F'|D|\), uniformly in \(\xi\) and in the history. Sources to be used: CMP 119 (2.42)–(2.48) for terms localized near \(D\), and the exponential decay of the minimizer's response for the rest. *Hypotheses: not verified; it is a real-support Lipschitz statement of the same nature as the first half of C-05, but only its zeroth-order (oscillation) form is needed, not a Hessian.*
* **In-3 (cap), i.e. (H1).** On \(\mathcal S\) the selector \(\chi_k\) gives \(|U_{k,\square}(\partial p)-1|<\varepsilon_k\eta^2\) for the fine plaquettes of the *local* minimizers (CMP 119 (3.8); LFR I (1.3)); with (1.2) and \(6\eta^{-4}\) fine plaquettes per unit cell this is \(3N\varepsilon_k^2/g_k^2\) of action per cell, so \(C_{\rm cap}\approx3N/c_*\). *Hypotheses: the selector is source input; the transfer from the local minimizers \(U_{k,\square}\) to the global background \(U_k\) (exponentially small difference, CMP 119 (3.6)–(3.7)) and the normalization of Balaban's action relative to \(s\) are not checked here.*
* **In-4 (a flag forces a bad cell).** If the test (3.2) fails at \(\square'\), some unit cell within a fixed distance of \(\square'^{\sim}\) has \(e_c\ge P_*\). Mechanism: \(U_{k+1,\square'}\) is controlled by the plaquettes of \(V_{k+1}\) (CMP 102 Theorem 1), a plaquette of \(V_{k+1}\) is an average of at most \(L^2\) unit plaquettes of \(V_k\) (the bounded window (S2)), and a unit plaquette defect of \(V_k\) is bounded by the square root of the local background action. *Hypotheses: not verified; it is the normalized counterpart of the factor "using Theorem 1 [15] and (71) [16]" in (S4).*
* **In-5 (surgery with support margin), i.e. (P3).** For admissible \((D^-,D)\) with \(|D|\le v_{\max}\): if all collar cells have \(e_c<P_*\), there is a field on \(D\), equal to the given one outside, lying in the support with a fixed margin, whose total action in \(D\) is at most \(C_{\rm ext}\) times the collar action. The smallness of \(c_*\) is what converts "collar energy below \(P_*\)" into "collar regular enough for the extension to stay in the support". Sources to be used: LFR I Proposition 1 and (1.75)–(1.78) (existence, uniqueness and regularity of the minimizing extension on parallelepipeds inside a \(100M\)-cube), CMP 102 Theorem 1. *Hypotheses: not verified; see §5.7(b) for why \(v_{\max}\) must be finite.*
* **In-6 (neighbourhood), i.e. (P4).** Around a point of the margin support, the ball of radius \(g_k/p_0(g_k)\) in each coordinate of \(D\) stays in \(\mathcal S\) and changes \(\mathcal A\) by \(O(|D|)\); then \(\log(1/\nu)\le C\log(p_0(g_k)/g_k)\). *Hypotheses: not verified; a first-order bound on \(g_k^{-2}A(U_k(\cdot))\) on the support.*

**Conditional conclusion — (b: In-1…In-6).** With these inputs, \(K,\rho_1,v_1\) are pure constants, \(\sigma_*=\tfrac12c_*p_0(g_k)^2-O(\log(p_0(g_k)/g_k))\to\infty\) as \(g_k\to0\), and for every deterministic set \(T\) of test cubes
\[
\mathbb P\bigl(T\subset P_{k+1},\ \text{clusters inside the window and below }v_{\max}/v_1\ \bigm|\ h,\ \xi,\ V_k\text{ outside the window}\bigr)\ \le\ 2K\,C_f^{|T|}\,e^{-\sigma_*|T|/C_f'}
\]
with constants \(C_f,C_f'\) depending only on the flag geometry. This would be clause 1 of H-02′ for the inherited low-margin sector at one step, with overlap and retained-data dependence, and with an exponent \(c\,p_0(g_k)^2\) that pays the carrier count and, in the window of Theorem 4.4, the insertion cost. **It is not claimed**: the inputs are open.

### 5.7 Limits of the method

**(a) A conserved flux defeats (P3): a one-dimensional example.** On a chain of sites \(i=0,\dots,n\) with real variables \(x_i\) (reference measure: normalized Lebesgue measure on a large interval), let \(f=\prod_{i<n}\mathbf 1[|x_{i+1}-x_i|<\varepsilon]\exp(-\beta(x_{i+1}-x_i)^2)\); cells are the sites, \(e_i=\beta(x_{i+1}-x_i)^2\) is the energy of the bond to the right of \(i\), and \(P_*=\beta\theta^2\) with \(0<\theta<\varepsilon\). Take the configuration with increment \(\theta\) on the bonds starting at the sites of an interval \(I\) and increment \(0\) elsewhere. Its bad set is \(I\), and every collar is good with zero energy. Let \(D\supset I\) be an interval of sites strictly inside the chain and let \(x'\) agree with \(x\) outside \(D\). The \(|D|+1\) bonds meeting \(D\) have increments summing to the same total \(\theta|I|\), fixed by the two sites adjacent to \(D\); by Cauchy–Schwarz their energy is at least \(\beta\theta^2|I|^2/(|D|+1)\). The gain is therefore at most \(\beta\theta^2|I|\,(1-|I|/(|D|+1))\), which is less than \(\tfrac12e(I)\) whenever \(|D|+1<2|I|\). In Theorem 5.3 the domains satisfy \(|D|\le|I|+2Kr_0\), so (P3) fails, for every \(C_{\rm ext}\), as soon as \(|I|>2Kr_0+1\). The total increment across \(D\) is a conserved quantity fixed by the exterior. The hypothesis (P3) therefore has content: it asserts that no locally conserved flux survives across a good collar. (In this example the true probability of the configuration class is still of order \(e^{-\beta\theta^2|I|}\); what fails is the local method.)

**(b) Four dimensions: the instanton scale — additional assumption.** For lattice gauge fields with all plaquettes \(\varepsilon\)-small, a ball of radius \(r\ll\varepsilon^{-1/2}\) is globally small in a radial gauge and a cut-off extension from a good collar is available; shells \(S^3\times[0,w]\) are simply connected, so there is no holonomy obstruction. For \(r\gtrsim\varepsilon^{-1/2}\) the field can carry topological charge, the charge inside a ball is fixed by the collar for every admissible filling, and every filling then costs at least a multiple of \(8\pi^2/g_k^2\). Conditionally on such an exterior, flags produced by the core of a small instanton are not rare. Hence In-5 can hold only for \(|D|\le v_{\max}\asymp\varepsilon_k^{-2}\), and the event "bad cluster larger than \(v_{\max}/v_1\)" is excluded from \(G_S\). Its probability (expected to be of order \(e^{-c/g_k^2}\)) needs a different, non-local argument. This paragraph is heuristic; it is the reason for the parameter \(v_{\max}\) in the theorem.

**(c) Clusters that reach the window boundary, and unreplaced components.** \(G_S\) excludes clusters within \(\rho_1\) of \(\Lambda\setminus W\), i.e. chains of bad cells joining a flag to an older large-field region. These are exactly the *mixed* sectors of the criterion. Theorem 5.3 itself covers them if cells of large-field components are declared bad, with \(e_c\) an apportionment of the reserve \(\kappa_j(Z)+2p_0\) of (S4), the label variables are included in \(\mathbb X_c\), and (LD) is proved for domains \(D\) containing whole components: the reference configurations \(y\) are then small-field fillings with the component deleted. That (LD) is a normalized comparison between the weight \(\mathbf T_k(Z)1\), bounded above in (1.79)–(1.89), and the mass of the small-field alternative with the same exterior, which needs a *local lower* stability bound. For eligible components this comparison is the content of the R operation (LFR II p.358, before (1.10): the denominator integral is bounded below by \(\exp(-O(1)|\Lambda|)\), with \(\Lambda\) inside a \(100M\)-cube) and of the accepted conditional presence bound of HS20; for non-eligible components it is open. **This is the main remaining estimate of H-02.**
