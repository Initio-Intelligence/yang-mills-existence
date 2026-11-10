# Normalized joint record bounds

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

## 2. Propositions N and F

**Proposition F.** Re-derived: the plaquettes of the centre-valued bonds, the exterior loop \(\partial Q\) (the top row at \(x_2=m+1\) carries one bond equal to \(z\), since \(c_2\le m+1\le c_2'\)), the triviality of the ring, the perturbation budget \(20(m+2)\delta\), and the SU(2) one-link version.  Its exterior is itself large-field next to \(B\) (the sheet continues outside the slices), as PE notes. It refutes field-conditioned bounds for arbitrary exteriors, which is what is claimed.

**Proposition N.** Re-derived Steps 0–4 against (LD) and (5.2) of R1 §5.2 as printed. Correct: literal (LD) fails for an all-good uniform-flux configuration on a cube of side \(s>16C_{\rm ext}r_0+4\).

**A loophole in Remark N.1.** The proof of Theorem 5.3 applies (5.1) to \(z\in G_{S',i}\) for *one* index \(i\) per \(z\). N.1 shows failure "for every \(i<K\) with \(s_i\) beyond that threshold", i.e. on large domains. With the provable constant 0.64, (5.1) is not refuted for sides between \(\approx8(C_{\rm ext}-1)r_0\) and \(16C_{\rm ext}r_0\), and a strongly bad cell admits small \(i\) where (5.1) plausibly holds. So N and N.1 do not exclude a repaired Theorem 5.3 that uses (LD) only on favourable pairs. The following does.

### 2.2 Proposition N′ — no pair works at a marginal bad cell

Setting and notation of PE §2.1 (Wilson instance of R1 §5.2: unit cells, \(f=e^{-\mathcal A}\), \(e_c\) the Wilson energy of the plaquettes owned by \(c\), \(W=\Lambda\)).

**Lemma 2.1 (sharp filling bound).** Let \(d\) be the bi-invariant geodesic distance on \(SU(N)\) for the Hilbert–Schmidt metric, \(c_N=\min(8/N,2/\pi^2)\), \(\bar d_N=c_N/(4\pi\sqrt N)\). Let \(z\) be the uniform-flux configuration of PE Step 1 with angle \(\varphi\), let \(D\) be a cube of side \(s\), and assume \(\sqrt2\varphi\le\bar d_N\) and \(\varphi(s+2)^2\le\pi/2\). Then for every \(y\) equal to \(z\) on the bonds not owned by \(D\),
\[
\sum_{p\in P(D),\ p\ \text{a }(1,2)\text{-plaquette}}\beta s(y_p)\ \ge\ \Bigl(1-\frac{\varphi^2}6\Bigr)\,b\,n_{12}(D),\qquad b=4\beta\sin^2(\varphi/2),
\]
where \(n_{12}(D)\) is the number of \((1,2)\)-plaquettes in \(P(D)\). The same holds if \(z\) is modified on bonds of directions 3, 4.

*Proof.* (i) \(d(AB,1)\le d(A,1)+d(B,1)\) and \(d(gAg^{-1},1)=d(A,1)\). (ii) For \(\Phi\le\pi/2\), \(d(e^{i\Phi H},1)=\sqrt2\Phi\): a logarithm has eigenvalues \((\Phi+2\pi m_1,-\Phi+2\pi m_2,2\pi m_3,\dots)\) with \(\sum m_k=0\); if some \(m_k\ne0\), two of them are nonzero and each such eigenvalue has modulus \(\ge3\pi/2\). (iii) If \(d(U,1)\le1\), the minimal logarithm has eigenvalues \(|\theta_k|\le1\) and \(s(U)=\sum(1-\cos\theta_k)\ge g_0(d(U,1))\), \(g_0(t)=t^2/2-t^4/24\), since \(\sum\theta_k^4\le(\sum\theta_k^2)^2\). (iv) If \(d(U,1)\ge1\) then \(s(U)\ge c_N\): if \(s(U)<c_N\), the principal angles satisfy \(\sum\theta_k^2\le\tfrac{\pi^2}2s(U)<1\) and \(|\sum\theta_k|\le\sqrt N\pi\sqrt{s/2}<2\pi\), so they sum to zero and \(d(U,1)<1\). (v) Let \(\bar d=\sqrt2\varphi\) and \(\ell\) the tangent to \(g_0\) at \(\bar d\). \(g_0\) is convex and increasing on \([0,1]\), so \(s(U)\ge\ell(d(U,1))\) when \(d\le1\); when \(d\ge1\), \(\ell(d)\le\bar d\,d\le\bar d\cdot2\pi\sqrt N\le c_N\le s(U)\). Hence \(s(U)\ge\ell(d(U,1))\) for all \(U\). (vi) Fix a slice and the square \(Q\) of PE Step 3. Non-abelian Stokes with (i), (ii): \(\sum_{p\in Q}d(y_p,1)\ge\sqrt2\varphi|Q|\). Ring plaquettes take their \(z\)-values, with \(d=\sqrt2\varphi\) exactly, so \(\sum_{p\in Q\cap P(D)}d(y_p,1)\ge\bar d\,|Q\cap P(D)|\). By (v) and \(\ell'>0\), \(\sum_{Q\cap P(D)}s(y_p)\ge|Q\cap P(D)|\,g_0(\bar d)=|Q\cap P(D)|\varphi^2(1-\varphi^2/6)\). Multiply by \(\beta\), use \(b\le\beta\varphi^2\), and sum over slices; every \((1,2)\)-plaquette of \(P(D)\) lies in one \(Q\). Bonds of directions 3, 4 do not enter \((1,2)\)-plaquettes. \(\square\)

**Proposition N′.** Let the constants of R1 §5.2 satisfy (5.5) and \(v_{\max}\ge v_1\). Put \(\delta=1/P_*\) and let \(\beta\ge\beta_1:=\max\{P_*^2v_1,\ P_*(2Kr_0+3)^4,\ \pi^2P_*/(2\bar d_N^2)\}\). For all large \(\ell\) there is \(z\in G_S\), \(S=\{c_{x_0}\}\), such that **for every \(i<K\) with \(z\in G_{S',i}\) the inequality (5.1) for \((D_i,D_{i+1})\) fails for every \(y\)**. By Lemma 5.1 of R1 at least one such \(i\) exists. Hence no version of (LD) restricted to the pairs used in the proof of Theorem 5.3 holds for the Wilson density.

*Proof.* Choose \(\varphi\) with \(\varphi\ell^2\in2\pi\mathbb Z\) and \(b\in[(1-\delta)P_*,(1-\delta/2)P_*]\). Since \(b\ge4\beta\varphi^2/\pi^2\), \(\varphi^2\le\pi^2P_*/(4\beta)\), so the hypotheses of Lemma 2.1 hold for every \(s\le2Kr_0+1\). Modify the bond \((x_0,3)\) by \(e^{i\psi H}\). The six plaquettes containing it become \(e^{\pm i\psi H}\) up to conjugation (the background is abelian and independent of \(x_3\)), each with energy \(t=2\beta(1-\cos\psi)\). Cell \(c_{x_0}\) owns three of them, each of \(c_{x_0-e_\mu}\), \(\mu=1,2,4\), owns one. Take \(t=(P_*-b)/2\). Then \(e_{c_{x_0}}=b+3t\ge P_*\), \(e_{c_{x_0-e_\mu}}=b+t<P_*\), and all other cells have \(e_c=b<P_*\). So \(\mathfrak B(z)=S'=\{c_{x_0}\}\), \(z\in G_S\), and the total excess is \(6t\le3\delta P_*=3\).

Let \(i<K\) with \(z\in G_{S',i}\), i.e. \(\text{gain}_i:=[e(D_i)-(C_{\rm ext}-1)e(D_{i+1}\setminus D_i)](z)\ge\tfrac12P_*\). Put \(D=D_{i+1}\), a cube of side \(s=2(i+1)r_0+1\), \(|D|\le v_1\). All excess plaquettes lie in \(P(D)\), so \(\sum_{P(D)}\beta s(z_p)=b\,n_{12}(D)+6t\). If (5.1) held for some \(y\), then with Lemma 2.1
\[
\Bigl(1-\frac{\varphi^2}6\Bigr)b\,n_{12}\ \le\ \sum_{P(D)}\beta s(y_p)\ \le\ b\,n_{12}+6t-\text{gain}_i+c_F|D| ,
\]
so \(\tfrac12P_*\le3+\tfrac{\varphi^2}6b\,n_{12}+c_Fv_1\). Here \(n_{12}\le s^2(s+1)^2\le2v_1\) and \(\tfrac{\varphi^2}6b\,n_{12}\le\tfrac{\pi^2}{12}P_*^2v_1/\beta\le1\). By (5.5), \(c_Fv_1\le\tfrac12P_*-\log(8v_1^2)\). Hence \(\log(8v_1^2)\le4\), false because \(v_1\ge3^4\). \(\square\)

**Meaning.** At a marginal flag the whole gain the pigeonhole finds is background energy of *good* cells, and that energy cannot be removed by any filling. This is the rigorous form of PE Remark N.3 at one scale. The transfer to the step-\(k\) density remains additional assumption, as in PE N.2.

## 3. Where a normalized record bound can come from

### 3.1 What the source normalizes — source input, assumed input

The source bounds on large-field histories are bounds on \(\mathbf T_k'(X)1\), the operation of LFR II (1.71). It is normalized by the localized reference integral of LFR I (1.100) (p.201: the quotient with denominator \(\int dV'\!\restriction_{\Lambda_i}\delta_{G_i}(V')\chi(\Lambda_i)\exp[-g_k^{-2}A(\zeta_i,U_{k,X_i}(V'V_{\Lambda_i}))]\)), and it exists as a normalized object only for components to which the R operation is applied. LFR I p.202: "we have to extract from the expression in the curly bracket \(\{\cdots\}\) the density \(\exp A_k\), where \(A_k\) is the effective action determined by the assumption that \(Z_k\) is the only large field region. The remaining expression should be localized around the components \(X_1,\dots,X_n\), represented as a polymer expansion". The \(n=0\) term of (1.100) is the density in which none of the candidate components was ever large.

So the source compares, **at the same post-replacement field**, the branch "component \(X\) carried the history \(\mathfrak L\) and was replaced" with the branch "\(X\) was never large". There is no such comparison for a component that is still open. This is why a direct attack on PE's (J) for open records has no starting point, and why Proposition F does not obstruct the closure comparison: its exterior fails the test (1.75), so no replacement is attempted.

### 3.2 The construction's accepted form: (HS20.4) — assumed input

Annex BI of `Reset posterior and scalar Fourier comparison` (H-03, complete at law level) states, for the common post-replacement data \(v\) ("the actual new background \(U_k\), the new current field \(V_k\) where it occurs explicitly, the unreplaced Zbar history data, and the Y geometry"):
\[
\pi_v(dC,d\eta_Y,d\eta_C)=\mathcal Z_v^{-1}\mathbf 1_{\{C\ \text{admissible}\}}e^{H_C(v,\eta_Y,\eta_C)}\prod_i\nu_i(d\eta_{Y_i})\prod_{X\in C}M_X(v,d\eta_X),\qquad M_X(v,\cdot)=\mathbf T_k'(X;v)(\cdot),
\tag{HS20.4}
\]
with Lemma HS20.1 (the family is closed under deleting whole components, with unchanged measures) and (HS20.7): "the cross-action change upon inserting one compatible \(X\)" is at most \(\lambda_R=C(1+R)^b\alpha_k\), \(\alpha_k\le Ce^{-cR}\). Consequently, for \(X\notin C\), \(C\cup\{X\}\) admissible, and any measurable set \(A\) of internal states of \(X\),
\[
\pi_v\bigl(C\cup\{X\},\ \eta_X\in A,\ d\eta_C,d\eta_Y\bigr)\ \le\ e^{\lambda_R}M_X(v,A)\ \pi_v\bigl(C,\ d\eta_C,d\eta_Y\bigr).
\tag{3.1}
\]
Use (HS20.4), HS20.1 and (HS20.7) as accepted construction results. The argument assumes them.

### 3.3 Theorem C — closure domination gives joint bounds

**Setting.** A probability space carries, for steps \(k=1,\dots,K_*\):
* a *live state* \(s_k\) in a standard Borel space \(\Sigma_k\);
* a finite random set \(C_k\) of *marks*, a subset of a countable set \(\mathbb M_k\).

**(M) Markov.** For every \(k\), the conditional law of \((s_l,C_l)_{l>k}\) given \((s_l,C_l)_{l\le k}\) is a function of \(s_k\) alone.

**(RD) Domination.** For every \(k\), \(m\in\mathbb M_k\) and finite \(C\subset\mathbb M_k\setminus\{m\}\), as measures on \(\Sigma_k\),
\[
\mathbb P\bigl(s_k\in\cdot\,,\ C_k=C\cup\{m\}\bigr)\ \le\ \zeta(m)\ \mathbb P\bigl(s_k\in\cdot\,,\ C_k=C\bigr).
\]

**Theorem C.** Under (M) and (RD), for distinct pairs \((k_1,m_1),\dots,(k_n,m_n)\), \(m_i\in\mathbb M_{k_i}\),
\[
\mathbb P\bigl(m_i\in C_{k_i}\ \text{for all }i\bigr)\ \le\ \prod_{i=1}^n\zeta(m_i).
\]

*Proof.* Induction on \(n\); \(n=0\) is trivial. Order so that \(k_1=\min_ik_i\). Let \(M'=\{m_i:i\ge2,\ k_i=k_1\}\), let \(E_{\rm fut}\) be the event that \(m_i\in C_{k_i}\) for all \(i\) with \(k_i>k_1\), and \(E'=\{m_i\in C_{k_i},\ i\ge2\}\). By (M) there is a measurable \(\phi:\Sigma_{k_1}\to[0,1]\) with \(\mathbb P(E_{\rm fut}\mid(s_l,C_l)_{l\le k_1})=\phi(s_{k_1})\). Summing over finite \(C\supset M'\) with \(m_1\notin C\),
\[
\mathbb P(m_1\in C_{k_1},E')=\sum_C\mathbb E\bigl[\mathbf 1_{\{C_{k_1}=C\cup\{m_1\}\}}\phi(s_{k_1})\bigr]\le\zeta(m_1)\sum_C\mathbb E\bigl[\mathbf 1_{\{C_{k_1}=C\}}\phi(s_{k_1})\bigr]\le\zeta(m_1)\,\mathbb P(E'),
\]
and \(\mathbb P(E')\le\prod_{i\ge2}\zeta(m_i)\) by induction. \(\square\)

**Remarks.**
1. The proof conditions only forward. No bound on an earlier event given a later label is used, so the reverse-reveal problem of the Strict-QR note §3 does not arise.
2. (M) cannot be dropped: if one Bernoulli(\(q\)) variable is recorded as a mark at two steps, each step satisfies (RD) with \(\zeta=q/(1-q)\) but both marks occur with probability \(q\). In the retained law (M) says that once a component is successfully replaced, nothing used later remembers its internal history.
3. (RD) is a bound conditional on the *post-closure* live state, which contains fields. It is the one field-conditional statement not excluded by Proposition F.

### 3.4 The retained law instance — conditional, readings stated

* **Step and state.** One step is one RG step including its R operation. \(s_k\) consists of the common data \(v\) of §3.2 together with the internal states \(\eta_Y\) of the components that remain large (non-eligible components, failed preparations, second class). \(C_k\) is the set of pairs \((X,\mathfrak L)\): \(X\) a successfully replaced component, \(\mathfrak L\) its complete internal label history (its exact ancestor record set and ancestry).
* **(RD) at successful replacements** is (3.1) integrated over \(v\), with
\[
\zeta(X,\mathfrak L)=e^{\lambda_R}\sup_vM_X(v,\{\mathfrak L\})=e^{\lambda_R}\sup_v\mathbf T_k'(X;\mathfrak L)1.
\]
* **(S) Size.** \(\sup_v\mathbf T_k'(X;\mathfrak L)1\le\exp\bigl(-\sum_{r\in\mathfrak L}c^{\rm Bal}(r)+c_1\sum_{(n,C)\in\mathfrak L}M^dR_n^{d+1}d_n'(C)\bigr)\). This is LFR II (1.79) (p.383, source) read per internal history: the display is a supremum over admissible domains, and the sum over histories was removed just before it — "the summations over the admissible sequences can be replaced by the factors \(\exp O(1)(MR_j)^{-d}|Z_j|\)". The bound is for real fields at \(J=0\): p.380, source, "\(\mathbf T_k'(X,(U,0))1\) is obviously positive", and (1.73)–(1.75). For a history containing a second-class record it also needs that the earlier scalar \(\mathbf T'_k(Y)1\) reappears as a factor of the later operation (LFR II (1.103)–(1.104), not read here).
* **(M)** is a reading of LFR I p.202 (quoted in §3.1) and of LFR II p.379 assumed input: "\(\Omega_k\) is the new \(k\)th domain defined by the determining set of the configuration \(U_k\)". HS20 states the one-step half: "Varying \(C\) in (1.72) therefore does not vary \(v\)". That later maps use only \((v,\eta_Y)\) is **not verified**.
* **(T) Terminal domination.** Add a last step \(K_*=K+1\) at which every component still large is given a mark. (RD) at that step says: for the terminal law, the set \(C\) of terminal lineages satisfies \(\mathbb P(C\cup\{m\})\le\zeta(m)\mathbb P(C)\) with \(\zeta\) obeying (S). The source says of (1.79) "the above inequality holds for all large field regions, not only for the regions satisfying the conditions (i), (ii)" (pp.383–384, source), which gives the size. It gives no normalized comparison for a non-eligible region. **(T) is an open hypothesis.**

## 4. Theorem R′: the integrated test from closure domination

### 4.1 Statement

A **lineage** is the complete ancestry of a component that receives a mark: the component \(X\), the step \(k\) of the mark, the exact set \(\mathcal R(\mathfrak L)\) of its ancestor records (births and failures, PE §3.1), and the resulting space-time set \(\mathfrak S(\mathfrak L)\) of ancestor cubes, determined by the records through (G3). By PE Lemma 3.3 \(\mathfrak S(\mathfrak L)\) is connected in the graph \(\mathfrak G\) of degree \(\le\Delta\).

**Theorem R′ — conditional.** Assume:
* (M), and (RD) with weights satisfying (S), at every step including the terminal one (T);
* (G1)–(G6);
* (G-R)\(_{c_0}\) with \(c_0\ge2(c_1+c_2)\), where \(c_2>0\) is chosen below.

Put \(c_3(n)=c_2M^dR_n^{d+1}/(4\cdot3^d)\) and assume
\[
\varepsilon_*:=\sup_n4(\Delta+1)^2L^4\exp\bigl(\sigma L^d(MR_n)^d-\tfrac12c_3(n)\bigr)\le\tfrac12,\qquad\eta_*:=\sup_n8(\Delta+1)^2e^{-c_3(n)/2}\le\tfrac12.
\]
Both hold for every fixed \(\sigma\) once \(c_2\ge1\) and \(R_n\ge\bar R(\sigma,L,M,d)\), i.e. \(\gamma\) small. For a component \(Y\) at step \(j\) with exact ancestor record set \(R\) define
\[
u(R)=\exp\Bigl(-\tfrac12\sum_{r\in R}c^{\rm Bal}(r)\Bigr)\prod_{(n,Q)\in\mathfrak S(R)}e^{-c_3(n)/2},\qquad a(Y,b)=2\sum_{R\mapsto(Y,b)}u(R).
\]
Then, with \(E_{Y,b}\) the retained event of the amendment (a whole component of the unreplaced region at step \(j\), \(b\) its oldest birth):
\[
\mathbb P\Bigl(\bigcap_iE_{Y_i,b_i}\Bigr)\le\prod_ia(Y_i,b_i)\quad\text{for pairwise disjoint }Y_i,
\tag{4.1}
\]
\[
\sum_{b\le j}\ \sum_{Y\ni x}L^{4(j-b)}e^{\sigma|Y|_\natural}a(Y,b)\ \le\ \delta:=4\varepsilon_*\exp\bigl(-\tfrac14\gamma_0A_1^2p_*^2\bigr),\qquad p_*=\min_{n\le j}p_0(g_n),
\tag{4.2}
\]
for every step-\(j\) cell \(x\). Constants are uniform in volume, \(j\), depth and history. This is clause (3) of the adopted H-02 test. Without (T), (4.1)–(4.2) hold for the events \(E_{Y,b}\cap\{\)the lineage of \(Y\) is successfully replaced before the terminal step\(\}\).

### 4.2 Proof

*Step 1: weight of one lineage.* By (S), \(e^{\lambda_R}\le2\), (G-R)\(_{c_0}\) and PE Lemma 3.1 (\(\#\text{cubes}(C)\le4\cdot3^dd_n'(C)\)),
\[
\zeta(\mathfrak L)\le2\exp\Bigl(-\tfrac12\sum_{\mathcal R(\mathfrak L)}c^{\rm Bal}-\bigl(\tfrac12c_0-c_1\bigr)\sum_{(n,C)}M^dR_n^{d+1}d_n'(C)\Bigr)\le2\exp\Bigl(-\tfrac12\sum_{\mathcal R(\mathfrak L)}c^{\rm Bal}\Bigr)\prod_{(n,Q)\in\mathfrak S(\mathfrak L)}e^{-c_3(n)}.
\]
(G-R) applies to the whole lineage because the marked component is a component of an admissible history.

*Step 2: fixed record sets.* Let \(Y_1,\dots,Y_n\) be disjoint components at step \(j\) with exact ancestor record sets \(R_1,\dots,R_n\), and \(E_{R_i}\) the event that \(Y_i\) is a component with exactly this ancestry. The \(R_i\) are pairwise disjoint, and so are the \(\mathfrak S(R_i)\) (PE, proof of (E2)). On \(\bigcap E_{R_i}\) every \(Y_i\) lies in exactly one lineage that receives a mark, at a step \(>j\) or at the terminal step. So \(\bigcap E_{R_i}\) is contained in the union, over *families* \(\{\mathfrak L_1,\dots,\mathfrak L_m\}\) of distinct lineages such that the sets \(I(\mathfrak L_l)=\{i:\mathfrak S(R_i)\subset\mathfrak S(\mathfrak L_l)\}\) partition \(\{1,\dots,n\}\), of the events "all marks \(\mathfrak L_l\) occur". By Theorem C,
\[
\mathbb P\Bigl(\bigcap E_{R_i}\Bigr)\le\sum_{\text{families}}\ \prod_l\zeta(\mathfrak L_l).
\]
Since \(\mathcal R(\mathfrak L)\supset\bigsqcup_{i\in I(\mathfrak L)}R_i\) and \(\mathfrak S(\mathfrak L)\supset\bigsqcup_{i\in I(\mathfrak L)}\mathfrak S(R_i)\), Step 1 gives
\[
\zeta(\mathfrak L)\le\prod_{i\in I(\mathfrak L)}u(R_i)\cdot\rho(\mathfrak L),\qquad\rho(\mathfrak L):=2\prod_{(n,Q)\in\mathfrak S(\mathfrak L)}e^{-c_3(n)/2}.
\]
*Covering sum.* Each family is determined by choosing, for every \(i\), either nothing or one lineage \(\mathfrak L\) with \(\min I(\mathfrak L)=i\). Hence
\[
\sum_{\text{families}}\prod_l\rho(\mathfrak L_l)\le\prod_{i=1}^n\Bigl(1+\sum_{\mathfrak L\ni(j,Q_i)}\rho(\mathfrak L)\Bigr),
\]
with \(Q_i\) a fixed cube of \(Y_i\). A lineage is determined by \(\mathfrak S\) and, per cube, a birth bit and a failure bit. With PE Lemma 3.4, \(\sum_{\mathfrak L\ni(j,Q)}\rho(\mathfrak L)\le\sum_{s\ge1}\eta_*^s\le1\). Therefore \(\mathbb P(\bigcap E_{R_i})\le\prod_i2u(R_i)\).

*Step 3: (4.1).* \(E_{Y,b}=\bigsqcup_{R\mapsto(Y,b)}E_R\). Sum Step 2 over \(R_1,\dots,R_n\).

*Step 4: (4.2).* By (G6), \(e^{\sigma|Y|_\natural}\le\prod_{\mathfrak S(R)}e^{\sigma L^d(MR_n)^d}\). Every slice \(b\le n\le j\) of \(\mathfrak S(R)\) is nonempty, so \(L^{4(j-b)}\le\prod_{\mathfrak S(R)}L^4\). The oldest record is a birth, so \(\sum_Rc^{\rm Bal}\ge\tfrac12\gamma_0A_1^2p_*^2\). A record set is determined by \(\mathfrak S\ni(j,Q_x)\) and two bits per cube. By PE Lemmas 3.3–3.4 the left side of (4.2) is at most \(2e^{-\gamma_0A_1^2p_*^2/4}\sum_{s\ge1}\varepsilon_*^s\le\delta\). \(\square\)

### 4.3 Corollaries

* **PE's (J) — conditional, same inputs.** Let \(\mathcal R\) be a finite set of deterministic records. Each record that occurs lies in exactly one lineage that receives a mark, and a record fixes a space-time cube of that lineage (a cube of the new region \(X\), or of the failed component \(C\)). By Step 1, \(\zeta(\mathfrak L)\le\prod_{r\in\mathcal R\cap\mathcal R(\mathfrak L)}e^{-c^{\rm Bal}(r)/2}\cdot\rho(\mathfrak L)\), and the covering sum of Step 2, anchored at the records instead of the components, gives
\[
\mathbb P(\text{all records of }\mathcal R\text{ occur})\ \le\ \prod_{r\in\mathcal R}2e^{-c^{\rm Bal}(r)/2}\ \le\ \prod_{r\in\mathcal R}e^{-c^{\rm Bal}(r)/4},
\]
the last step because \(c^{\rm Bal}\ge p_0(g)\ge4\log2\). So (J) holds with \(\theta=\tfrac18\) as a consequence, not an input, and PE's Theorem R with its forms (E1)–(E4) follows.
* **First-step lineage — conditional: K-02 and (G1)–(G6), (G-R).** PE Corollary 3.7 with §1.3 item 7 gives weights of the form (4.1)–(4.2) for components whose ancestry consists of step-0 births only. This uses no closure input and no H-03. It covers one sector, not the test.

## 5. Inherited low-margin events

PE §4.4 proposed to charge a P-flag under a coarser near-threshold background to the coarser record. In the closure formulation no charging rule is needed.

* **Inside a lineage** a low-margin flag, a failed preparation and a P-birth at depth are records. Theorem R′ needs only the size (S) of the whole lineage at its mark. Bałaban's factors are additive over records ((1.79) is a product; the failure factors \(\prod'\) multiply the birth factors), so (S) contains the joint cost.
* **Why the conditional non-rarity does not enter** — additional assumption. N′ and Remark N.3 hold a *fine-scale* exterior fixed. A successful replacement happens at least \(N=R\) steps after the last birth in the component (LFR I p.177 (ii); LFR II p.384 "with \(N=R_j\)"), on a component inside a \(100MR_k\)-cube whose exterior passed (1.75). The comparison (3.1) is made at the scale-\(k\) state \(v\). A fine near-threshold background of extent below \(L^N\) fine cells has been integrated in both branches and costs its own action in the numerator only. A background large enough to survive to scale \(k\) is above threshold at an intermediate scale, creates births there, and keeps the component ineligible: it is part of the lineage. This is the multi-scale mechanism PE §4.4 asked for; it is built into conditions (i), (ii).
* **What remains analytic** is (S) and (3.1) themselves, i.e. the uniformity of the source bounds over the admitted exterior history, which H-03 records as its scope.
