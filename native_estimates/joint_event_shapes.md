# Joint events indexed by retained shapes

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

## 1. Setting, target and sources

### 1.1 Notation and the target

* Dimension \(d=4\), \(G=SU(N)\), block factor \(L\).
* Steps \(n=0,1,\dots\) of Bałaban's procedure (CMP 119, LFR I–II), with couplings \(g_n\le\gamma\) (the hypothesis of LFR II Theorem 1).
* Thresholds \(p_0(g)=A_0(\log g^{-2})^{p_0}\) and cube sizes \(R_n\asymp(\log g_n^{-2})^{r}\).
* \(Z_n\): the large-field region after the operations of step \(n\), a union of \(MR_n\)-cubes of the scale-\(n\) lattice. "Component" means connected component.
* \(d_n'(X)\): Bałaban's linear size of a localization domain \(X\) at scale \(n\). It is the length of a shortest tree graph meeting all \(MR_n\)-cubes of \(X\), in units of the cube side (CMP 109 p.257, before (0.24), clean text: "a length of a shortest graph in this class, divided by M, is the linear size of X"; the primed version for \(MR_n\)-cubes is used in LFR II with the same meaning, which is a reading).
* \(|Y|\): the number of scale-\(j\) unit cells of \(Y\).

A *retained record at step \(j\)* is a pair \((Y,b)\): \(Y\) is a component of \(Z_j\), and \(b=b(Y)\) is the earliest step of a birth among the ancestor records of \(Y\) (defined in §3.1). Write \(E_{Y,b}\) for the corresponding event in the H-01 lift. These are the "events \(D\) born at \(b\) still alive at \(j\)" of the analysis (§3.3). For a chain of births the relevant \(b\) is the **oldest** birth: the native-scale coordinates of that step are still retained in \(Y\), and \(L^{4(j-b')}\le L^{4(j-b)}\) for every later \(b'\). This settles a point the analysis leaves implicit.

The per-event inequality is proved below in four forms, with \(\delta\) small:

* **(E1) Single event.** \(\mathbb P(E_{Y,b})\le\delta\,L^{-4(j-b)}e^{-\sigma|Y|}\).
* **(E2) Joint.** \(\mathbb P(\bigcap_iE_{Y_i,b_i})\le\prod_i\delta\,L^{-4(j-b_i)}e^{-\sigma|Y_i|}\) for pairwise disjoint \(Y_i\).
* **(E3) Shape-summed.** \(\sum_{b\le j}\sum_{Y\ni x}L^{4(j-b)}e^{\sigma|Y|}\,\mathbb P(E_{Y,b})\le\delta\) for every scale-\(j\) cell \(x\).
* **(E4) Covering.** \(\mathbb P(S\subset Z_j)\le e^{-(\sigma-\delta)|S|}\) for every deterministic set \(S\) of scale-\(j\) cells.

(E3) is the analysis (E) with "log(count)" read as the shape sum. (E4) is the form of the native-domain comparison's Theorem 4.2.

### 1.2 Primary-source facts used — source input, as stated in the source

| Ref. | Content used |
|---|---|
| LFR I p.177 | Eligibility: "(i) it is contained in a cube of the size \(100MR_k\), (ii) in the preceding \(N\) renormalization steps no new large field regions were created inside this component, and the previous regions contained in it satisfy the condition (i) on the corresponding scales". "Each renormalization step adds at least ten layers of \(MR_k\)-cubes, hence the size must be greater than \(20MR_k\)". |
| LFR II p.383, (1.79) | \(\mathbf T_k'(X)1\le\sup\exp\{\sum_jO(1)M^dR_j^{d+1}d_j'(Z_j)\}\prod_j\prod_i\exp(-\tfrac12\gamma_0A_0^2p_0^2(g_j)(d_j'(Z_j^{(i)})+1)-2p_0(g_j))\prod'\exp(-p_0(g_j))\). The last product runs over components satisfying (i),(ii) "for which some large fields are created during the preparatory steps". Preparatory factors are \(\le\exp(-p_0(g_j))\) under \(2p_1-(d+5)r_0>p_0\). |
| LFR II p.384 | \(S(Z)=Z'^{\sim10}\): the smallest union of \(LMR_{j+1}\)-cubes covering \(Z\), plus ten layers. "The factor \(\exp(-\kappa_j(Z))\) controls \(K\) renormalization steps …", with (1.80) \(\kappa_j(Z)\ge\sum_{n=j+1}^{j+K}O(1)M^dR_n^{d+1}d'_n(S^{n-j}(Z))\), where \(N=R_j\). Also \(S^{n-j}(Z)\subset\bigcup_{\square_0\subset Z^{(n-j)}}\square_0^{\sim31}\) and \(d_n'(S^{n-j}(Z))\le(63)^d3\cdot2^{d-1}d_n'(Z^{(n-j)})\), or \(\le(64)^d\) if the latter vanishes. |
| LFR II p.385 | \(d'_n(Z^{(n-j)})\le L^{-\frac12(n-j)}d'_j(Z)\le2^{-(n-j)}d'_j(Z)\). Then \(K\le n_0-j+R_j\), and (1.81)–(1.83), including survival \(\kappa_{j+1}(Z)=\kappa_j(Z_0)-O(1)M^dR^{d+1}_{j+1}d'_{j+1}(Z)\). |
| LFR II p.386 | Failure rule: "a new large field was introduced in the preparatory operations … We define \(\kappa_{j+1}(Z)=p_0(g_j)-O(1)M^dR^{d+1}_{j+1}d'_{j+1}(Z)\) … \(K=R_{j+1}\)". (1.84) \(Z\subset\bigcup_n(Z_j^{(n)})'^{\sim10}\cup\bigcup_i(Z^{(i)}_{j+1})^{\sim2}\). (1.85) merge rule. The tree-graph induction. |
| LFR II p.387 | (1.86)–(1.88), closed "for \(p_0\) large and \(\gamma\) small"; (1.89) \(\mathbf T_k'(X)1\le\exp(-2(1+\beta_0)^{-1}p_0(g_k))\) for eligible \(X\) (\(K=0\)). |

### 1.3 construction inputs

* **H-01 lift** (Annex W §4): one probability space carrying the Wilson field with its exact marginal and all primitive labels.
* **K-02** (Annex A Theorem 3.1): \(\mathbb E e^{\eta E_X}\le K^{b(X)}\).
* **RB9.20–21, H9.37**: as stated in [All-depth physical Q/R births on strict regular carriers](../lattice_theory/observable_v.md) (RB9.20–21) and [Normalized early births, causal stencils, and restart histories](../lattice_theory/observable_iv.md) (H9.37), and used in `Strict births and reverse reveal` (the "Strict-QR note"). **The argument assumes them.** They enter only Corollary 3.8.

## 3. Theorem R: reduction of (E) for every retained sector to a joint record bound

### 3.1 Records and ancestry — source readings

* **(G1)** \(Z_n\) is a union of \(MR_n\)-cubes. New large-field regions at step \(n\) are components ("\(Z_n^{(i)}\)" in (1.79), (1.84)) made of test cubes. There are at most \(\nu_0=\nu_0(L,M,M_2,d)\) test cubes per \(MR_n\)-cube.
* **(G2)** A component \(C\) of \(Z_n\) that is not replaced at step \(n+1\) satisfies \(S(C)\subset Z_{n+1}\). Every component of \(Z_{n+1}\) satisfies the inclusion (1.84). The R operation at step \(n+1\) is applied exactly to the components satisfying (i),(ii) (with \(N=R\)) for which no preparatory large field is created; all others are retained (LFR I p.177; LFR II pp.383, 386).
* **(G3)** The ancestry of a component — its ancestor components and its shape at every step — is a deterministic function of its ancestor records. Evolution between records is \(S\) plus the merge construction. Replacement depends only on the component's own geometry, its own history and its own failure label.
* **(G4)** Every component of \(Z_n\) has linear extent \(>20MR_n\) (LFR I p.177). Hence it contains two cubes 19 cube-units apart, so \(d_n'(C)\ge18\ge1\).
* **(G5)** \(R_{n+1}/R_n\in[L^{-1},L]\) (LFR I p.177, LFR II p.385), and the \(MR_n\)-partitions are nested under rescaling.

Some definitions follow.
* A **birth record** is \((n,X)\) with \(X\) a new region at step \(n\). A **failure record** is \((n,C)\) with \(C\) an eligible component at step \(n\) whose preparatory tests create a large field.
* For a component \(Y\) of \(Z_j\), the **ancestor components** are defined backwards: \(\mathrm{Anc}_j(Y)=\{Y\}\), and \(\mathrm{Anc}_n(Y)\) is the set of components \(C\) of \(Z_n\), not replaced at step \(n+1\), with \(S(C)\) contained in a member of \(\mathrm{Anc}_{n+1}(Y)\).
* The **ancestor records** \(\mathcal R(Y)\) are the records located in ancestor components.
* The **space-time ancestry** is \(\mathfrak S(Y)=\{(n,Q):\ Q\text{ an }MR_n\text{-cube in a member of }\mathrm{Anc}_n(Y),\ b(Y)\le n\le j\}\).

Bałaban's costs are
\[
c^{\rm Bal}(n,X)=\gamma_0A_1^2p_0^2(g_n)\,(d_n'(X)+1)+2p_0(g_n)\ \ \text{(birth, (1.85))},\qquad c^{\rm Bal}(n,C)=p_0(g_n)\ \ \text{(failure, p.386)},
\]
and his per-step loss is \(w_n(C)=c_0M^dR_n^{d+1}d_n'(C)\), with \(c_0>0\) the \(O(1)\) of (1.79).

**(G-R) Bałaban's reserve lemma source input, with scaled costs.** Fix \(\theta\in(0,1]\). Define \(\kappa_n(C)\) for every component of every admissible history by these rules:
* survival (1.83);
* the failure rule of p.386;
* the merge rule (1.85), with births costing \(\theta c^{\rm Bal}\) and failures \(\theta p_0\);
* the first step by (1.85) with no old components. That (1.82) comes from this definition is the interpretation of "From the definition of \(\kappa_1(Z)\)".

Then \(\kappa_n(C)\ge\sum_{m=n+1}^{n+K}w_m(S^{m-n}C)\ge0\) for \(p_0\ge\bar p_0(\theta)\) and \(\gamma\le\bar\gamma(\theta)\). For \(\theta=1\) this is LFR II (1.80)–(1.88). For \(\theta<1\) it follows by inspecting that proof: the costs enter only through the three closing inequalities, namely the condition after (1.82), the failure case on p.386, and (1.87)–(1.88). Each has the form "(cost coefficient)\(\times p_0^2\) or \(p_0\)" \(\ge C\,M^dR^{d+2}\), so scaling costs by \(\theta\) only raises \(\bar p_0\).

### 3.2 Four lemmas

**Lemma 3.1 (covering).** A finite connected union \(T\) of segments of total length \(\ell\), in units of the cube side, meets at most \(3^d(2\ell+2)\) closed cubes of a unit lattice partition. Hence, by (G4), a component \(C\) of \(Z_n\) has \(\#\mathrm{cubes}(C)\le4\cdot3^d\,d'_n(C)\).

*Proof.* Traverse \(T\) by a closed walk that uses each edge twice, of length \(2\ell\). Points at arc-length spacing 1 along it number at most \(\lceil2\ell\rceil+1\), and every point of \(T\) lies within distance \(\frac12\) of one of them. A closed ball of radius \(\frac12\) meets at most \(3^d\) closed unit cubes. A cube of \(C\) is met by a shortest tree. For the second claim use \(d'\ge1\). \(\square\)

**Lemma 3.2 (spent reserve) — deduction, given (G-R).** For every component \(Y\) of \(Z_j\),
\[
\sum_{n\le j}\ \sum_{C\in\mathrm{Anc}_n(Y)}w_n(C)\ \le\ \theta\sum_{r\in\mathcal R(Y)}c^{\rm Bal}(r).
\]

*Proof.* Put \(\tau_n(C)=\kappa_n(C)+2\theta p_0(g_{j(C)})\), where \(j(C)\) is the index of the first large-field region in \(C\) as in (1.85). Define \(\tilde\tau_n(C)\) as \(\theta\) times the costs of the records of \(C\), minus the \(w\)'s already spent on the ancestors of \(C\). By the three rules:
* survival: \(\tau_{n+1}=\tau_n-w\);
* failure: \(\tau_{n+1}=\theta p_0(g_n)-w+2\theta p_0\le\tau_n(C_0)+\theta p_0(g_n)-w\), because \(\kappa_n(C_0)\ge0\) by (G-R) with \(K=0\);
* merge: by (1.85), \(\tau\) is additive over the merged parts, plus the new costs, minus \(w\).

By induction \(\tau_n\le\tilde\tau_n\). Since \(\tau_j(Y)\ge0\), the claim follows. \(\square\)

**Lemma 3.3 (space-time connectivity) — deduction, given (G2), (G5).** Let \(\mathfrak G\) be the graph on pairs \((n,Q)\) with edges between touching cubes at the same \(n\), and between \((n,Q)\) and \((n+1,Q')\) when \(Q'\) meets the rescaled image of \(Q\). Its degree is at most \(\Delta:=3^d+2^d+(L^2+2)^d\), and \(\mathfrak S(Y)\) is connected in \(\mathfrak G\).

*Proof.*
* *Degree.* A cube touches \(\le3^d\) cubes at its own time. By (G5) its rescaled image meets \(\le2^d\) cubes at time \(n+1\). Its preimage at time \(n-1\) has side \(\le L^2\) cube units, so it meets \(\le(L^2+2)^d\) cubes.
* *Connectivity.* Each \(C\in\mathrm{Anc}_n(Y)\) is connected. Since \(S(C)=(\rho C)'^{\sim10}\supset\rho C\) lies in a member of \(\mathrm{Anc}_{n+1}(Y)\), every cube of \(C\) has a forward neighbour in \(\mathfrak S(Y)\). Following forward edges reaches \(Y\), which is connected. \(\square\)

**Lemma 3.4 (animals).** In a graph of maximal degree \(\Delta\), at most \((\Delta+1)^{2s}\) connected vertex sets of size \(s\) contain a given vertex.

*Proof.* Encode such a set by a depth-first walk on a spanning tree. The walk has \(2(s-1)\) steps, each a choice among at most \(\Delta\) neighbours or a return. \(\square\)

### 3.3 The hypothesis and the theorem

**(J) Joint record bound.** For every finite set \(\mathcal R\) of deterministic records at steps \(\le j\),
\[
\mathbb P(\text{every record in }\mathcal R\text{ occurs})\ \le\ \exp\Big(-\sum_{r\in\mathcal R}c^J(r)\Big),\qquad c^J(r)\ge2\theta\,c^{\rm Bal}(r).
\]
(J) may also be assumed conditionally on a \(\sigma\)-field \(\mathcal G_t\), for records at steps \(>t\); every conclusion below then holds conditionally on \(\mathcal G_t\) for \(b>t\).

**Theorem R — conditional: inputs (J), (G1)–(G5), (G-R).** Set
\[
\varepsilon_n:=(\Delta+1)^2\,2^{2\nu_0}\,L^4\exp\Big(\sigma(MR_n)^d-\frac{c_0M^dR_n^{d+1}}{4\cdot3^d}\Big),\qquad \varepsilon_*:=\sup_n\varepsilon_n ,
\]
and assume \(\varepsilon_*\le\frac12\). This holds once \(R_n\ge\bar R(\sigma,L,M,d,c_0)\), i.e. for \(\gamma\) small. Put
\[
\delta:=2\varepsilon_*\exp(-\theta\gamma_0A_1^2p_*^2),\qquad p_*=\min_{n\le j}p_0(g_n).
\]
Then (E3) holds. Consequently (E1), (E2) and (E4) hold with this \(\delta\), with \(\sigma\) as chosen, and uniformly in the volume, in \(j\), and in the history.

**Proof.**

*Union bound.* \(E_{Y,b}\) is contained in the union, over the possible ancestor record sets \(\mathcal R\) with \(Y(\mathcal R)=Y\) and \(b(\mathcal R)=b\), of the events "all records of \(\mathcal R\) occur". By (G3), \(\mathcal R\) determines the ancestry, hence \(\mathfrak S=\mathfrak S(\mathcal R)\). Conversely, given \(\mathfrak S\), the records are determined by choosing, at each time, a set of test cubes inside \(\mathfrak S_n\) (the births, as its components) and a failure flag per ancestor component. That is at most \(2^{2\nu_0|\mathfrak S|}\) choices.

*Cost of one record set.* By (J), Lemma 3.2, Lemma 3.1 and (G4),
\[
\mathbb P(\mathcal R)\le e^{-\theta\sum c^{\rm Bal}}\,e^{-\theta\sum c^{\rm Bal}}\le e^{-\theta\gamma_0A_1^2p_0(g_b)^2}\prod_{n}\prod_{C\in\mathrm{Anc}_n}e^{-w_n(C)}\le e^{-\theta\gamma_0A_1^2p_*^2}\prod_{(n,Q)\in\mathfrak S}e^{-c_0M^dR_n^{d+1}/(4\cdot3^d)}.
\]
The first factor uses that the oldest record is a birth at \(b\).

*The weights in (E3).* Every slice \(n\in[b,j]\) of \(\mathfrak S\) is nonempty, so \(L^{4(j-b)}\le\prod_{(n,Q)\in\mathfrak S}L^4\). Also \(|Y|\le(MR_j)^d\,\#\mathfrak S_j\), so \(e^{\sigma|Y|}\le\prod_{(n,Q)\in\mathfrak S}e^{\sigma(MR_n)^d}\).

*Summation.* Sum over the connected sets \(\mathfrak S\ni(j,Q_x)\), where \(Q_x\) is the \(MR_j\)-cube containing \(x\), using Lemmas 3.3–3.4:
\[
\sum_{b,\,Y\ni x}L^{4(j-b)}e^{\sigma|Y|}\mathbb P(E_{Y,b})\le e^{-\theta\gamma_0A_1^2p_*^2}\sum_{s\ge1}\varepsilon_*^s\le\delta.
\]
This is (E3).

*(E1).* Each term of (E3) is at most \(\delta\).

*(E2).* Distinct components at \(j\) have disjoint ancestor record sets: a shared record would put both in one component by (G2). Apply (J) to the union of the record sets. The sum then factorizes into \(\prod_ia(Y_i,b_i)\) with \(a(Y,b):=\sum_{\mathcal R\mapsto(Y,b)}e^{-C^J(\mathcal R)}\). The proof of (E3) bounds \(L^{4(j-b)}e^{\sigma|Y|}a(Y,b)\) by \(\delta\).

*(E4).* On \(\{S\subset Z_j\}\), the components meeting \(S\) form a disjoint family \(\{Y_i\}\) with \(\sum|Y_i|\ge|S|\). Hence
\[
\mathbb P(S\subset Z_j)\le e^{-\sigma|S|}\sum_{\text{families}}\prod_ie^{\sigma|Y_i|}a(Y_i,b_i)\le e^{-\sigma|S|}\prod_{x\in S}\Big(1+\sum_{Y\ni x,b}e^{\sigma|Y|}a(Y,b)\Big)\le\big(e^{-\sigma}(1+\delta)\big)^{|S|}.
\]
The middle step assigns each \(Y_i\) to its first point of \(S\) in a fixed order; this map is injective. \(\square\)

### 3.4 Corollaries and the sectors covered

**Lemma 3.5 (forward composition).** Let \(\mathcal H_n\) be the \(\sigma\)-field of all labels through step \(n\), and \(\mathcal H_{n-\frac12}\) that of the labels through the new regions of step \(n\). Suppose:
* (B): \(\mathbb P(X_1,\dots,X_k\text{ all new at step }n\mid\mathcal H_{n-1})\le\prod e^{-c^J(n,X_i)}\);
* (B′): the analogous bound for failures given \(\mathcal H_{n-\frac12}\).

Then (J) holds. *Proof.* Condition on the latest stage and iterate, as in the native-domain comparison's Lemma 5.6. Earlier records are measurable for the earlier stage. \(\square\)

**Remark 3.6.** (B) asks for more than the RB9, which forbids conditioning on microscopic past labels inside the carrier (Strict-QR note §1). (J) is the minimal input. It can be supplied by (B), by the chronological H9.37 tower (Strict-QR note §6), or by direct joint arguments.

**Corollary 3.7 (first-step lineage) — conditional: K-02, (G-R), and (G1) for step 0.** Let \(\mathcal R\) consist of step-0 births only. A step-0 region \(X\) is a bounded fattening of flagged \(LM_2R_0\)-cubes, so it contains at least \(\#\mathrm{cubes}(X)/C_{\rm fat}\) flagged cubes (reading). Distinct regions use distinct flagged cubes. By the native-domain comparison's Lemma 4.1, (J) holds with \(c^J(r)=(\eta P_0/\mu_0-\log(n_\Pi K))\#\mathrm{cubes}(X)/C_{\rm fat}\ge c\,p_0(g_0)^2(d'(X)+1)\). This is \(\ge2\theta c^{\rm Bal}\) for a fixed small \(\theta\). Hence (E1)–(E4) hold for every component whose ancestry consists of step-0 births only: no later births and no failures, any merges, any lifetime.

**Corollary 3.8 (strict Q/R lineages) — conditional: RB9.20–21, H9.37 (unverified), (G-R).** Consider the classes for which the Strict-QR note §6 eq. (6) gives a joint bound \(\exp(-cp_b^2n-c'\sum p_{k_i}^2|S_i|)\): a strict b-step birth family together with later canonical-small P-admitted Q/R births, in chronological order. For those classes (J) holds with \(c^J\ge2\theta c^{\rm Bal}\), \(\theta\) small. Then (E1)–(E4) hold for components whose ancestry consists of such records. Failures and P-births are excluded.

### 3.5 What Theorem R does and does not do

* It handles chains, mergers, oversized components, repeated failures and arbitrarily long lifetimes in one argument. There is no separate case analysis and no clean-window or branching hypothesis, unlike H8-A and the Strict-QR note §§1, 7–10.
* Arbitrarily many scales cost nothing beyond the per-cube factor \(\varepsilon_*\). This answers the problem "comparable physical costs on arbitrarily many scales remain untreated" (Strict-QR note §4), *given (J)*.
* It proves no probability bound by itself. The entire analytic content of H-02 is now (J).

## 4. The input (J)

### 4.1 Known

* Step 0, by K-02 (Corollary 3.7).
* Strict Q/R classes, conditional on RB9/H9 (Corollary 3.8).
* Nothing for P-births at depth, for preparatory failures, or for births on mixed carriers.

### 4.2 How far microscopic certificates reach

**Lemma 4.2 (typical energy).** Let \(\beta\ge200N\), and let \(C_1=\frac{25\pi^2}2n_sN\) be the constant of the native-domain comparison's Lemma 2.1. Let \(A\subset(3\mathbb Z)^4\) be finite and \(X_A=\{(x,12):x\in A\}\). Then
\[
\mathbb P\Big(\sum_{p\in X_A}e_p<\frac{|A|}{4eC_1}\Big)\le\exp\Big(-\frac{0.13}{2e}|A|\Big).
\]
Hence every region \(\Gamma\) that is a union of \(|\Gamma|/81\) blocks of \(3^4\) unit cells has Wilson energy at least \(c_N|\Gamma|\), with \(c_N=(4\cdot81\,eC_1)^{-1}\), with probability at least \(1-e^{-c|\Gamma|}\).

*Proof.* The link \((x,1)\) is "private" to \(p_x=(x,12)\) within \(X_A\): the other plaquettes containing it are \((x-e_2,12)\) and the \((1,3)\)-, \((1,4)\)-plaquettes, and \(x-e_2\notin(3\mathbb Z)^4\). Apply Lemma 2.1 with \(t=1/C_1\); the hypothesis \(t\le\beta/(200N)\) holds because \(C_1>1\):
\[
\mathbb P(e_{p_x}\ge1/C_1\mid\text{all links but }(x,1))\ge\tfrac12e^{-1}=:q.
\]
The events for the other \(p_{x'}\) are measurable for that conditioning. So for the indicator count \(S\) and \(\lambda=1\), induction gives \(\mathbb E e^{-S}\le(1-q(1-e^{-1}))^{|A|}\). Chernoff yields \(\mathbb P(S\le q|A|/2)\le\exp(q|A|(\frac12-(1-e^{-1})))=e^{-0.132q|A|}\). On the complementary event, \(\sum e_p\ge(q|A|/2)/C_1\). \(\square\)

**Meaning.** A certificate "event \(\Rightarrow E_\Gamma\ge T\)" carries no rarity unless \(T\ge c_N|\Gamma|\).
* A step-\(b\) birth lives on \(\Gamma\) of at least \(L^{4b}\) fine cells.
* The Wilson energy it forces cannot exceed that of a smooth configuration realising it. That is \(\approx C(g_b/g_0)^2p_0(g_b)^2\) (additional assumption; classical scaling).

So microscopic certificates fail once \(c_NL^{4b}\gtrsim Cp_0^2\). This is the quantitative form of "isolated microscopic rarity is not substituted for a coarse event".

**Corollary 4.3 (shallow births) — conditional: forcing input (F).**
* *Input (F).* A birth record \((n,X)\) forces \(E_{\Gamma(X)}\ge c_fp_0(g_n)^2\#\mathrm{cubes}(X)\) on a fine region \(\Gamma(X)\) of at most \(v_fL^{4n}(MR_n)^d\#\mathrm{cubes}(X)\) plaquettes, with overlap multiplicity \(\le\mu\) across records.
* *Conclusion.* By the argument of Lemma 4.1 applied to the sets \(\Gamma(X)\),
\[
\mathbb P(\mathcal R)\le\exp\Big(-\sum_r\big[\eta c_fp_0^2/\mu-v_fL^{4n_r}(MR)^d\log K\big]\#\mathrm{cubes}(X_r)\Big).
\]
This gives (J) for records at steps \(n\le b_{\rm mic}\) with \(L^{4b_{\rm mic}}\le\eta c_fp_0^2/(2\mu v_f(MR)^d\log K)\), i.e. \(b_{\rm mic}\approx\frac14\log_L(p_0^2/R^4)\to\infty\) slowly.
* *Mechanism for (F) at a P-flag, additional assumption.* The actual field is a competitor for the constrained local minimizer, so \(A_{\square^\sim}(U)\ge A_{\square^\sim}(U_{\min})\). Regularity of the minimizer (CMP 102) turns one large minimizer plaquette into action \(\gtrsim\varepsilon_b^2\) on a unit scale-\(b\) volume. The indicated CMP 102 estimate is a separate hypothesis.

### 4.3 Forms of (J) that are impossible

* Conditional on fields (Proposition F).
* Proved by one-scale local surgery from a thin collar (Proposition N and Remark N.3).

### 4.4 Proposed route — additional assumption

The analytic object that exists is the exact fiber law Annex W (3.14) of the current fluctuation given the coarser retained data \(v\). The plan is coarse-to-fine:
1. **Q/R records at step \(n\) given \(v\).** On fibers whose coarse data are regular near \(X\), prove \(\mathbb P(\text{flags in }X\mid v)\le e^{-cp_0^2\#X}\). This is a tail estimate for the normalized fiber law, of C-08 type, and needs the C-05/C-08 regular-law inputs.
2. **P records at step \(n\).** A P-flag on \(V_n\) is either produced by the fluctuation of step \(n\), which is a fiber tail as in step 1, or inherited from a large background \(V^{(n)}(V_{n+1})\). In the second case it sits under a coarser near-threshold configuration, i.e. under a coarser record, and is charged to that record.
3. **Feeding Theorem R.** Theorem R's counting is time-symmetric: it sums over space-time animals. A record charged to a coarser record in the same space-time animal is already paid there. So the needed input becomes a joint bound for "irreducible" records, those not under a coarser record, with the others absorbed into the animal entropy, which is already controlled by \(\varepsilon_*\).
