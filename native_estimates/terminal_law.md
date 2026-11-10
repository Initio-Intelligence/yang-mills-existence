# Terminal volume and reflection bounds

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

## 1. (S-Y): the second-class factor

### 1.1 Where the violating cube sits

LFR II p.378: "Now we try to remove the characteristic functions \(\chi_{k,\Lambda}\chi\). We introduce the decompositions of unity \(1=\chi_k((\Omega_k^{\sim4})^c)+\chi_k^c((\Omega_k^{\sim4})^c)\) in components of \(Z\). The components with the second, large field function are included again into the large field domain of the new action … The restrictions introduced by \(\chi_k\) imply that \(|\partial V_k-1|<2\varepsilon_k\) on the corresponding components of \(Z\)". The display (1.72) on p.379 writes the same function as \(\prod_{i=1}^m\chi_k^c(Y_i^{\sim-6})\chi_{k,\Lambda_i}\chi_i\delta_{G_i}(V_k')\mathbf T_k'(Y_i)\), and (1.102), (1.104) on pp.390–391 as \(\chi_k^c(Y^{\sim-6})\). The exponent is **\(-6\)** (checked at 220 dpi); \(X^{\sim-n}\) is the shrinking by \(n\) layers (CMP 119 (2.14) uses \(\Omega^{\sim-2}\subset\Omega\) in the same sense), consistent with \((\Omega_k^{\sim4})^c\subset\Omega_k^c\subset Z\). So the second-class test region is \(Y^{\sim-6}=(\Omega_k^{\sim4})^c\cap Y\), six layers inside \(Y\). IM's doubt "whether the plaquette may sit in \(Y^{\sim6}\setminus Y\)" is void.

### 1.2 Which function it is

CMP 119 p.257, source, (2.16)–(2.17): "We consider the partition of the lattice \(T_\eta\) into \(LM_2R_k\)-cubes, compatible with the other partitions, and for each cube \(\square\) of this partition we define the function \(U_{k,\square}(V_k)\) by \(U_{k,\square}(V_k)=U(\mathbf B_k(\square^{\sim4}),M^\cdot(Q_k^{s*}V_k))\) (2.16) … \(\chi_k(\Omega_k)=\prod_{\square\subset\Omega_k}\chi(\{\sup_{p\subset\square^\sim}|U_{k,\square}(V_k,\partial p)-1|<\varepsilon_k\eta^2\})\) (2.17)". So \(\chi_k(S)\) is a product over cubes of functions \(\chi_{k,\square}\), each a function of \(V_k\restriction\square^{\sim4}\) through the **local** minimizer with the homogeneous determining set \(\mathbf B_k(\square^{\sim4})\): history-free and strictly local. Hence
\[
\chi_k^c(Y^{\sim-6})=\sum_{\emptyset\ne P\subset Y^{\sim-6}}\chi_k^c(P)\,\chi_k(Y^{\sim-6}\setminus P),
\]
a sum over nonempty index-\(k\) large-field sets \(P\) of exactly the type "\(\chi_j^c(P_j)\)" of p.380, located in \(Y^{\sim-6}\), with dependence set \((Y^{\sim-6})^{\sim4}\subset Y\). The field tested is the new field \(V_k\), the argument of \(\mathbf R\rho_k\) (the fresh reference variable on \(\Lambda\subset Y\) times \(V_\Lambda\)).

### 1.3 The Wilson term that pays

LFR II p.365 (1.33)–(1.35) (quoted in IM §1): on \(Z\), including the second-class components, the new determining set is \(\{Z^{(k)}\}\) and \(U_k=U_{\mathbf B_k}(V)\). The new action (1.101) is \(A_k=A_k'+\sum\mathbf R'^{(k)}+\sum\mathbf B'^{(k)}\) with \(A_k'((g_k(\cdot))^{-2},U_k)\) containing \(-A((g_k(\cdot))^{-2},U_k)\) on the whole lattice (CMP 119 (2.23), p.258). In (1.104) the second-class components carry "no integral operations … only the characteristic functions" (p.391, source) and the scalar \(\mathbf T_k'(Y_i)1\). So in every later bound of the lineage, the \(k\)-th step contributes the factor \(\chi_k^c(Y^{\sim-6})\) **and** the Wilson term of \(U_k\) on \(Y\) at coupling \(g_k\): exactly the data from which p.380 derives, "in the usual way, using Theorem 1 [15] and (71) [16]", the factor
\[
\exp\Bigl(-\gamma_0\frac1{2g_k^2}(B_3^{-1}\varepsilon_k)^2(LM_2R_k)^{-d}|P|\Bigr)\ \le\ \exp\bigl(-\tfrac12\gamma_0B_3^{-2}A_0^2\,p_0^2(g_k)\bigr)\quad(P\ne\emptyset).
\]
The mechanism is checked on CMP 102 p.273, source, (67)–(71): "the part of the action \(\frac1{g_k^2}A''(U_k)\) localized to the sum of four \(j\)-blocks \(\Delta'\) connected with the plaquette \(p'\) can be bounded from below by \(\frac14p^2(g_j)\), and the corresponding part of the exponential gives the small factor \(\exp(-\frac14p^2(g_j))\). We get these small factors for all plaquettes in all large fields set \(P\)." Also LFR II p.378: "We denote the component by \(X\), it may be any component of the first, or of the second class, and we define \(\mathbf T_k'(X)=\dots\)", so (1.79) bounds the history scalar \(\mathbf T_k'(Y)1\) of a second-class component as well.

### 1.4 Consequences — deduction given 1.1–1.3; additional assumption for the one sentence

1. **Cost.** A second-class record at step \(k\) has \(c^{\rm Bal}\ge\frac12\gamma_0A_1^2p_0^2(g_k)(d_k'(\mathrm{cover}P)+1)+2p_0(g_k)\ge p_0(g_k)\) (p.381's reduction of the cube factor to the fundamental factor). This is far more than the \(e^{-p_0(g_j)}\) of a preparatory failure.
2. **Reserve lemma.** Bałaban's failure rule (p.386: "a new large field was introduced in the preparatory operations. Then \(\kappa_j(Z_0)\ge0\), and we do not have a better bound for it, but we have the new factor \(\exp(-p_0(g_j))\). We define \(\kappa_{j+1}(Z)=p_0(g_j)-O(1)M^dR_{j+1}^{d+1}d_{j+1}'(Z)\). It satisfies (1.80), because \(Z\) is a small domain, it is contained in a cube of the size \(100MR_{j+1}\)") applies verbatim to a second-class \(Y\): \(Y\) is an eligible, hence small, component and the new factor is at least \(e^{-p_0(g_k)}\). The induction (1.80)–(1.88) therefore covers second-class lineages, and (G-R)\(_{c_0}\) holds for them (RB §1.2).
3. **(S) for lineages through a second-class record** holds with the product of the old \((1.79)\) factor for \(\mathbf T_k'(Y)1\) and the new \(P\)-type factor; the only non-printed sentence is that p.380's factor is applied to the index-\(k\) function \(\chi_k^c(Y^{\sim-6})\) additional assumption. Regard it as the same mechanism, not a new estimate.
4. **Locality.** The second-class test is strictly local in the new field (§1.2). This is used in §5.

## 2. The unnormalised terminal bound (T_U)

### 2.1 Statement

Let \(Z_{K,h}\ge0\) be the weight of the complete primitive history \(h\) at the terminal step \(K\) in the positive lift of Annex W (B-01; Annex W (2.15): \(\sum_hZ_{K,h}=\mathscr Z\)), and \(\mathbb P(h)=Z_{K,h}/\mathscr Z\). For a terminal mark \(m=(X,\mathfrak L)\) put
\[
\zeta^0(X,\mathfrak L)=\exp\Bigl(-\sum_{r\in\mathfrak L}c^{\rm Bal}(r)+c_1\sum_{(n,C)\in\mathfrak L}M^dR_n^{d+1}d_n'(C)\Bigr)
\]
(the right side of (1.79) read per history, RB (S)). **(T_U)**: there are constants \(E_+(g_K),E_-'(g_K)<\infty\) such that for every finite set \(M\) of pairwise disjoint terminal marks
\[
\sum_{h:\,M\subset C_*(h)}Z_{K,h}\ \le\ e^{E_+|T_K|}\prod_{m\in M}\zeta^0(m),\qquad\mathscr Z\ \ge\ e^{-E_-'|T_K|},
\]
where \(|T_K|\) is the number of sites of the terminal (step-\(K\), unit) lattice.

### 2.2 Source status

* **Volume constants and their lattice.** LFR II p.355, source, (0.1): "\(\chi_k\exp[-\frac1{g_k^2}A(U_k)-E_-|T_\eta|]\le\rho_k\le\exp E_+|T_\eta|\)". CMP 119 p.264, source, Corollary 3: "there exist constants \(E_-,E_+\) independent of \(\eta\) and \(T\), but depending on \(g_k\), such that \(\chi_k(T_\eta)\exp[-\frac1{g_k^2}A(U_k(V_k))-E_-|T_\eta|]\le\rho_k(V_k)\le e^{E_+|T_\eta|}\) (2.50)", preceded by (2.49) "\(A_k=-A(\frac1{g_k^2},U_k)+\)(the logarithmic terms)\(+O(1)\sum_{j=1}^k|\Gamma_j|\)" and p.263 "The volumes are taken in the corresponding scales, i.e. \(|\Gamma_n\cap\Omega|\) means the number of points in the set \(\Gamma_n\cap\Omega\subset T_\eta^{(n)}\)" and "the combinatorics now is the same, relative to the \(\eta\)-scale of the lattice \(T_\eta\), as in [6]". CMP 102 p.273, source, (65)–(66): "\(|E_k|\le\dots\le O(1)|T_1^{(k)}|\)", "\(-\frac1{g_k^2}A''(U_k)+\sum_{j=0}^{k-1}O(\log g_j^{-1})|Z_j|+O(1)|T_1^{(k)}|\)". So \(E_\pm\) count **sites of the current unit lattice**; the logarithmic terms are attached to the large-field regions (native volumes) and are paid by the large-field factors (LFR II p.380: "every large field domain \(Z_j\) contributes the constant \(O(1)\log g_j^{-2}|Z_j|\le\dots\le O(1)M^dR_j^{d+1}d_j'(Z_j)\)"). This answers IM §7.6's open sub-point.
* **Per-term form of the upper bound — additional assumption, supported by.** CMP 102 pp.273–274: "We get these small factors for all plaquettes in all large fields set \(P\). … The analysis of Sect. 3.C [9], which is model independent, show that these small factors are enough to control all sums in (41) … This gives the upper bound in (5)." CMP 119 p.264: "The first term on the right-hand side yields the small factors for large field characteristic functions. It also controls the logarithmic terms. Thus we estimate the integral \(\int dV_k\rho_k\) by a sum of terms". LFR II pp.383–384: (1.79) and "the above inequality holds for all large field regions, not only for the regions satisfying the conditions (i), (ii)"; (2.19) of CMP 119 (p.258): \(\mathbf T_k(Z_k)=\prod_i\mathbf T_k(X_i)\). The upper bound is thus obtained by bounding each term by the product of its large-field factors and summing. Restricting the sum to the terms whose large-field region contains the components of \(M\) with the prescribed histories, and using the factorisation, gives the first line of (T_U) with the same \(E_+\). The extraction is used without the full sum before the factors are extracted; this is the same reading as RB's (S).
* **Lower bound — additional assumption.** The second line is the lower bound of (0.1) integrated, \(\mathscr Z\ge e^{-E_-|T_K|}\int dV\,\chi_K(V)e^{-g_K^{-2}A(U_K(V))}\), together with an elementary small-ball estimate \(\int\chi_Ke^{-g_K^{-2}A(U_K)}\ge(cg_K)^{C|T_K|}\) (the minimizer's action is at most that of any admissible extension of a near-identity \(V\)); \(E_-'=E_-+O(\log g_K^{-2})\). Not printed as such.
* **Size of \(E_\pm\) — additional assumption.** From (2.49) and CMP 102 (66): \(E_\pm\le C\log g_K^{-2}\). Theorem T1 below needs only \(E_\pm\le(\log g_K^{-2})^{c_E}\) with \(c_E<2p_0-6r\) on the B-02 witness.

(T_U) is a statement about positive integrals; it uses no analyticity and no comparison. It is of the same nature as (S): a per-history reading of a printed sup-bound. Use it as the single source input of §3.

## 3. Theorem T1: ultraviolet stability as a probability estimate in bounded terminal volume

### 3.1 Statement and proof — conditional: input (T_U), (G-R)\(_{c_0}\) with \(c_0\ge2c_1\)

Put \(\mathsf E:=(E_++E_-')|T_K|\) and \(c_{\min}:=\frac12\gamma_0A_1^2p_*^2\), \(p_*=\min_{n\le K}p_0(g_n)\).

**Theorem T1.** For every finite set \(M\) of pairwise disjoint terminal marks,
\[
\mathbb P(M\subset C_*)\ \le\ e^{\mathsf E}\prod_{m\in M}\zeta^0(m).
\]
If \(\mathsf E\le\frac14c_{\min}\), then (T_J) of IM §7.4 holds with \(\theta=\frac34\), \(c_T=c_1\): \(\mathbb P(M\subset C_*)\le\prod_{m\in M}\zeta_T(m)\), \(\zeta_T(m)=\exp(-\frac34\sum_{\mathfrak L}c^{\rm Bal}+c_1\sum M^dR^{d+1}d')\).

*Proof.* The first display is the quotient of the two lines of (T_U). For the second: every lineage contains a birth, so \(\sum_{r\in\mathfrak L}c^{\rm Bal}(r)\ge c_{\min}\) for each \(m\in M\); if \(M\ne\emptyset\), \(e^{\mathsf E}\le e^{c_{\min}/4}\le\exp(\frac14\sum_{r\in\mathfrak L_{m_1}}c^{\rm Bal})\) for any \(m_1\in M\), and \(e^{\mathsf E}\prod_m\zeta^0(m)\le\prod_m\zeta_T(m)\). (For \(M=\emptyset\) both sides are 1.) \(\square\)

By IM Theorem R″, (T_J) with these constants gives the integrated test with \(\theta=\frac34\) in Step 1 and \(c_0\ge2(c_1+c_1+c_2)/\theta\). (The requirement that the weights be \(\le1\) uses (G-R)\(_{c_0}\) with \(c_0\ge2c_1\), as in RB Step 1.)

### 3.2 Scope

T1 is uniform in history and depth, but **not in volume**: it requires
\[
(E_++E_-')(g_K)\cdot|T_K|\ \le\ \tfrac18\gamma_0A_1^2p_*^2 ,
\]
i.e. a terminal torus with at most \(c\,p_0(g_K)^2/\log g_K^{-2}\) sites, poly-logarithmically many in \(g_K^{-2}\). On a sequence with fixed terminal coupling \(g_*\) and \(T_n\to\infty\) it says nothing (§3.4).

### 3.3 The B-02 witness — conditional: T1, and assumed input for the geometry and the absence of R operations

`Finite Wilson family` §§1, 3: \((\log Y_0)^r=L^{2n+s+1/2}\), \(R_j=L^{2n+s+1}\) for all \(j\le K_n\le n\), \(M=L^u\), \(T_n=2L^{H_n}\ell_0\) with \(H_n=3n+s+2+\max(u,1+v)+q\), \(a_n=L^{-K_n}\ell_0\), \(\max_{j\le K_n}g_j\to0\). Hence \(|T_{K_n}|=16L^{4H_n}\) and, with \(p_0(g)=(\log g^{-2})^{p_0}\) and \(E_\pm\le(\log g^{-2})^{c_E}\),
\[
\log_L\bigl(\mathsf E\bigr)\le4H_n+c_E\frac{2n+s+\frac12}r+\log_L32,\qquad
\log_L p_*^2\ \ge\ \frac{2p_0}{r}\Bigl(2n+s+\tfrac12\Bigr)-O(1).
\]
For \(r\ge2\), \(p_0\ge5r\), \(c_E=1\): \(13n+O(1)\) against \(20n+O(1)\); the condition of T1 holds for all large \(n\) (margin \(7n-O(1)\); still positive for \(c_E=7\)). So **(T_J) holds on the B-02 witness, conditional on (T_U)**.

Moreover, on that witness no \(\mathbf R\) operation is performed: `Finite Wilson family` §1, "the literal Wilson start has no (1.76) processing in this interval, since LFR I pp.177–179 require \(j\ge N>N_0\)" with \(N=R_j=L^{2n+s+1}>n\ge K_n\) (c\*; consistent with LFR I p.177 (ii), quoted in IM §3). Then every lineage is terminal, there are no failure and no second-class records, and RB Theorem R′/IM Theorem R″ needs neither (M) nor (RD) nor Annex BI. Hence:

> **Corollary 3.1 — conditional.** On the B-02 witness sequence, the adopted H-02 test (clauses (1), (3), (4) of the amendment) holds for all retained events, conditional on (T_U), (S), (G-R)\(_{c_0}\), (G1)–(G6) and the Port note's geometry, uniformly along the sequence.

This closes H-02 on that sequence at the same evidential level as RB/IM's inputs, but the witness has \(g_{K_n}\to0\) and is not the physical sequence of B-05; see the Port note's own table of excluded uses.

### 3.4 Why unnormalised bounds cannot do more

The two lines of (T_U) are compatible with \(\mathbb P(M\subset C_*)=1\) as soon as \(2\mathsf E\ge\log(1/\zeta^0(m))\): put all weight on one history containing \(M\). So in unbounded terminal volume at fixed \(g_K\), (T_J) needs a principle that normalises per unit volume. Conditioning on exterior fields is false (PE Prop. F, RB Prop. N′). The remaining principle is reflection positivity.

## 4. Theorem T2: chessboard reduction for tile-local record events

### 4.1 Setting

* **Torus and tilings.** \(\mathbb T=(\mathbb Z/T\mathbb Z)^d\) is the bare lattice, \(T=2L^{H+K}\). A *tiling* \(\mathcal T\) is given by an integer \(\ell\mid L^{H+K}\) with \(T/\ell=2m\) even and an offset \(a\in\mathbb Z^d\); the tiles are the closed cubes \(t_z=\prod_\mu[a_\mu+z_\mu\ell,a_\mu+(z_\mu+1)\ell]\), \(z\in(\mathbb Z/2m)^d\); the reflections \(\vartheta_{\mu,c}\) are \(x_\mu\mapsto2(a_\mu+c\ell)-x_\mu\) (site planes; on the torus each fixes the two planes \(c\) and \(c+m\)).
* **Reflection-positive structure.** A probability space \((\Omega,\mathfrak F,\mathbb P)\) with (R1) sub-\(\sigma\)-fields \(\mathfrak F_S\) for closed boxes \(S\), monotone in \(S\); (R2) for each plane \(P\) a measurable involution \(\vartheta_P\) of \(\Omega\) preserving \(\mathbb P\), with \(\vartheta_P^{-1}\mathfrak F_S=\mathfrak F_{\vartheta_PS}\); (R3) for each \(P\) and each bounded real \(F\) measurable w.r.t. \(\mathfrak F_{H_P^+}\), \(H_P^+\) the closed half torus on one side of \(P\): \(\mathbb E[F\cdot F\circ\vartheta_P]\ge0\).
* **Chessboard estimate.** Under (R1)–(R3), for events \(A_t\in\mathfrak F_t\), \(\mathbb P(\bigcap_tA_t)\le\prod_t\|A_t\|\), \(\|A_t\|:=\mathbb P(\bigcap_s\vartheta_{s\leftarrow t}A_t)^{1/N}\), \(N=(2m)^d\), where \(\vartheta_{s\leftarrow t}\) is the composition of coordinate reflections taking \(t\) to \(s\). This is Fröhlich–Israel–Lieb–Simon, CMP 62 (1978), Theorem 4.3, whose proof uses only (R2)–(R3) and the Cauchy–Schwarz step direction by direction; it applies to closed tiles sharing faces (the 1D case is Hölder's inequality for \(\operatorname{Tr}\prod A_i\) with \(A_i^T=\) reflected \(A_i\)). **External standard theorem.**

**Lemma 4.1 (realisation).** Let \(\Omega=\{U\}\times[0,1]^I\), \(\mathbb P=\mu_W\otimes\mathrm{Leb}^{\otimes I}\), where \(I\) is a countable index set of *seeds* with a location map \(\mathrm{loc}:I\to\{\text{closed boxes}\}\) and an action of the reflections on \(I\) compatible with \(\mathrm{loc}\); \(\mathfrak F_S=\sigma(U_b:\ b\subset S;\ \xi_i:\ \mathrm{loc}(i)\subset S)\); \(\vartheta_P(U,\xi)=(\vartheta_PU,\xi\circ\vartheta_P)\) with \((\vartheta_PU)_b=U_{\vartheta_Pb}\) (orientation reversed for links normal to \(P\)). Then (R1)–(R3) hold.

*Proof.* (R1), (R2) are immediate (\(\mu_W\) is invariant under lattice reflections, the plaquette action being a sum of \(\operatorname{Re\,tr}\) of oriented plaquettes). (R3): write \(S_W=S_++S_-+S_0\) with \(S_0\) the plaquettes contained in the plane, \(S_\pm\) the rest on each side, \(S_-=S_+\circ\vartheta_P\). Conditionally on the plane links \(U_0\), the links on the two sides are independent under \(\mu_W\) with mirror-image laws; the seeds located strictly on one side are independent of everything else. For \(F\) measurable w.r.t. \(\mathfrak F_{H^+}\) put \(f(U_0)=\mathbb E[F\mid U_0]\) (integrating the \(+\) links and the \(+\) seeds). Then \(\mathbb E[F\cdot F\circ\vartheta_P]=\mathbb E[f(U_0)^2]\ge0\), because \(\vartheta_P\) fixes \(U_0\) and maps the \(+\) data to independent \(-\) data with the mirror law. \(\square\)

* **Records.** A countable set \(\mathfrak R\) of *records* with events \(O_r\in\mathfrak F\) and weights \(w(r)\in(0,1]\). A record is *\(t\)-local* if \(O_r\) coincides a.s. with an event of \(\mathfrak F_t\).
* **(Cov)** For \(r\) \(t\)-local and every tile \(s\), \(\vartheta_{s\leftarrow t}O_r=O_{r_s}\) for a record \(r_s\in\mathfrak R\) with \(w(r_s)=w(r)\), the map \((s,r)\mapsto r_s\) being injective.
* **(J_U)** For every finite \(S\subset\mathfrak R\): \(\mathbb P(\bigcap_{r\in S}O_r)\le e^{\mathsf E}\prod_{r\in S}w(r)\).

### 4.2 Statement and proof

**Theorem T2.** Under (R1)–(R3), (Cov), (J_U): for every finite \(R=\bigsqcup_tR_t\) with each \(r\in R_t\) \(t\)-local,
\[
\mathbb P\Bigl(\bigcap_{r\in R}O_r\Bigr)\ \le\ \prod_{t:\,R_t\ne\emptyset}\Bigl(e^{\mathsf E/N}\prod_{r\in R_t}w(r)\Bigr).
\]

*Proof.* \(A_t:=\bigcap_{r\in R_t}O_r\in\mathfrak F_t\). By the chessboard estimate \(\mathbb P(\bigcap_tA_t)\le\prod_t\|A_t\|\), and by (Cov) and (J_U), \(\|A_t\|^N=\mathbb P(\bigcap_s\bigcap_{r\in R_t}O_{r_s})\le e^{\mathsf E}\prod_{r\in R_t}w(r)^N\) (the \(r_s\) are distinct). \(\square\)

**Corollary 4.2 (several tilings).** Let \(\mathcal T_1,\dots,\mathcal T_q\) be tilings satisfying the hypotheses, \(R\) finite with every \(r\) local for some tile of some \(\mathcal T_i\), and \(w(r)\le e^{-2\mathsf E/N}\) for all \(r\). Then \(\mathbb P(\bigcap_{r\in R}O_r)\le\prod_{r\in R}w(r)^{1/(2q)}\).

*Proof.* Split \(R=\bigsqcup_iR^i\) by a choice of tiling. \(\mathbb P(\bigcap_R)\le\min_i\mathbb P(\bigcap_{R^i})\le\prod_i\mathbb P(\bigcap_{R^i})^{1/q}\), and by T2 each factor is \(\le\prod_{t}(e^{\mathsf E/N}\prod_{R^i_t}w)^{1/q}\le\prod_{r\in R^i}w(r)^{1/(2q)}\), since every occupied tile contains a record with \(e^{\mathsf E/N}\le w(r)^{-1/2}\). \(\square\)

### 4.3 The geometry on the B-02 torus — deduction given the Port note's periods assumed input

Let \(S_{\max}\) be the side (in bare units) of the coarsest partition cube used up to step \(K\) (\(MR_K\) or \(LM_2R_K\) cubes of the terminal lattice). The Port note arranges all partitions centred at a common origin with \(S\mid L^{H+K}\) for every partition side \(S\). Take \(\ell=L^{q'}S_{\max}\), \(q'\ge1\), \(\ell\mid L^{H+K}\); then \(T/\ell=2L^{H+K}/\ell\) is even and the tile planes are centre planes of **every** partition cube and of every block up to level \(K\): the reflections preserve the whole block hierarchy up to level \(K\), the gauge-fixing blocks, and all cube partitions. Shifted tilings with offsets \(a=cS_{\max}\), \(0\le c<L^{q'}\), have the same property; \(q=2^d\) tilings with offsets \(0\) and \(\lfloor L^{q'}/2\rfloor S_{\max}\) in each coordinate make every set of diameter \(<\ell/4\) interior to a tile of one of them. The per-tile constant is
\[
\frac{\mathsf E}N=(E_++E_-')\,(L^{q'}S_{\max}/L^K)^d\le C\log g_K^{-2}\,L^{d(q'+1)}\max(M,M_2)^dR_K^d,
\]
which is \(\le\frac12c_{\min}\) for \(\gamma\) small, since \(p_0(g)^2=(\log g^{-2})^{2p_0}\) and \(2p_0>dr+1\) (true for \(p_0\ge5r\), \(d=4\), \(r\ge2\)). So the volume constant is harmless **per tile**, uniformly in \(T\), \(K\) and history.

### 4.4 What T2 gives for H-02 — conditional

Take as records the *flagged test cubes* \((n,\square,\tau)\): "\(\square\) is a testable cube at step \(n\) and the test of type \(\tau\) (\(P\), \(Q\), \(R\), preparatory, exterior, second-class) fails there", with weight \(w=e^{-c_\square(n,\tau)}\) the per-cube factor of LFR II pp.380–383 (for \(P\): \(\exp(-\gamma_0\frac1{2g_n^2}(B_3^{-1}\varepsilon_n)^2)\)). Their unnormalised joint bound (J_U) follows from (T_U) and RB's Theorem C/covering sum exactly as RB §4.3 derives (J) from (T): peel the replaced lineages by (RD) (Annex BI), bound the terminal ones by (T_U), with the per-cube factors of (1.79) in place of the region factors; this is IM's Theorem C′ with (T_J) replaced by (T_U) and the factor \(e^{\mathsf E}\) carried along. A region record \((n,X)\) implies its flagged cubes, and \(c^{\rm Bal}(n,X)\le C_{\rm fat}\sum_{\square\text{ flagged in }X}c_\square\) (PE Cor. 3.7's fattening reading plus PE Lemma 3.1). Therefore:

> **Proposition 4.3 — conditional.** Assume (R1)–(R3) [Lemma 4.1], (J_U) [(T_U) + RB's inputs], and that every flagged-cube record is tile-local for one of the \(2^d\) tilings of §4.3 and satisfies (Cov). Then PE's (J) holds with \(c^J(r)\ge2\theta c^{\rm Bal}(r)\), \(\theta=2^{-d-2}/C_{\rm fat}\), for **all** finite record sets, terminal lineages included; by PE Theorem R the adopted H-02 test follows, uniformly in volume, depth and history. In particular (T_J) holds.

So in unbounded volume, **(T_J) is reduced to the two structural properties "every flagged-cube event is tile-local" and (Cov)**. Both are statements about the label algorithm, not estimates. Their status is §5.

## 5. Locality and covariance of the label algorithm: what holds, what fails

### 5.1 Finite propagation (FP) — the property needed

**(FP)** There is \(\rho<\infty\) such that for every space-time cube \((n,\square)\) and test type \(\tau\) the event "\(\square\) is testable at step \(n\) and the \(\tau\)-test fails" is measurable w.r.t. the bare links and seeds within distance \(\rho\,S_n\) of \(\square\), \(S_n\) the side of the coarsest step-\(n\) partition cube in bare units.

(FP) implies tile-locality for every cube at distance \(\ge\rho S_n\) from the tile boundary, hence (with \(\ell\ge4\rho S_K\)) for one of the \(2^d\) tilings. (Cov) then follows from the Euclidean covariance of the rules under the reflections of §4.3.

### 5.2 Rules that are strictly local

1. **\(P\)-test.** CMP 119 (2.16)–(2.17) (p.257, quoted in §1.2) and (3.2) (p.265): per cube, a function of the field restricted to \(\square^{\sim4}\) through the local minimizer with homogeneous determining set. History-free.
2. **\(Q\)-test.** CMP 119 (3.3)–(3.4), p.265: \(\chi(\{\sup_{b\in(\square'^{\sim2})^{(k)*}}|V_k(b)(V_{\square'}^{(k)}conditional)^{-1}-1|<2\delta_k\})\), \(V_{\square'}^{(k)}=M^k(U_{k+1,\square'})\): a function of \(V_k\) (in the block axial gauge) and \(V_{k+1}\) on \(\square'^{\sim2}\). The gauge fixing (1.5) (p.247) is a product over blocks and sites of normalised factors in the contour variables \(U(y,x)\): given \(U\), the gauge variables are independent across sites, hence realisable by seeds located at sites; Bałaban: "The main point in introducing it in the form (1.5) is to preserve the Euclidean invariance".
3. **Second-class test** \(\chi_k^c(Y^{\sim-6})\): §1.2.
4. **Growth.** LFR II (1.76), p.381: \(Z_j\subset Z_{j-1}'^{\sim10}\cup\bigcup_i(Z_j^{(i)})^{\sim2}\): deterministic layers, at most ten \(MR\)-cubes per step.
5. **Eligibility.** LFR I p.177 (i) "contained in a cube of the size \(100MR_k\)", (ii) no new large field in the preceding \(N\) steps inside the component (quoted in IM §3): decided from the labels within a \(100MR_k\)-cube and the component's own ancestry, which lies inside it.
6. **Preparatory and exterior tests.** LFR I p.183 (IM §3): "all the characteristic functions introduced above depend on the field variables localized in the corresponding components of the large field region \(Z_k\)"; the component is eligible, hence small. (c) via IM's quotation.
7. **Resampling.** The reference kernel \(K_{k,X,G}(dV'\mid v)\) of Annex W (2.12)–(2.13) depends on \(v\) near \(X\) and is Euclidean covariant by the averaging over the \(2^d\) reflections and \(d!\) permutations of the axial graph (LFR II p.379: "we take only the \(2^d\) reflections for subsets of coordinates, and the \(d!\) permutations of the coordinates"; p.390: "they are Euclidean covariant, i.e., they have the property (2.32) [III]"). It is realisable by a seed located at \(X\); for components inside a tile a covariant realisation is obtained by transporting one from a base tile (the tile action is simply transitive).

### 5.3 The rule that is not strictly local

**\(R\)-type test.** CMP 119 (1.18), p.250: \(\chi(\{\sup_{b\in(\square'^{\sim2})^*}|A(b)|<g_0^{-1}\delta_0\})\), where \(A\) is the fluctuation variable relative to the **global** background, \(U(b)=\exp(ig_0A(b))U_1(b)\) ((1.19)), and p.250: "both configurations \(U_1,U_{1,\square'}\) are determined by the same configuration \(V\) on \(\square'^{\sim3}\), hence on \(\square'^{\sim2}\) the difference between these configurations is very small. More precisely \(|U_1U_{1,\square'}^{-1}-1|<O(1)B_3\exp(-\delta LM_2R_1)\varepsilon_1\)". The general step (3.16) is of the same form. So the \(R\)-test outcome depends on the whole small-field domain and on its shape (history) through an exponentially small term. **(FP) is false for the literal construction**, and since the \(R\)-flags feed the regions, the eligibility and the resampling, every later label inherits the defect.

The defect is confined to a *threshold collar*: the local quantity \(A_{\rm loc}(b)=(ig_0)^{-1}\log(U(b)U_{1,\square'}(b)^{-1})\) determines the outcome unless \(|A_{\rm loc}(b)|\in[g^{-1}\delta-\eta,g^{-1}\delta+\eta]\), \(\eta=O(1)B_3e^{-\delta LM_2R}\varepsilon/g\). Hence what is needed is:

> **(TC) Threshold-collar bound.** Let \(\mathrm{Amb}_{n,\square}\) be the local event that some \(b\in(\square^{\sim2})^*\) has \(|A_{\rm loc}(b)|\) in the collar. Then \(\mathbb P(\bigcap_{(n,\square)\in S}\mathrm{Amb}_{n,\square}\cap\bigcap_{r\in S'}O_r)\le e^{\mathsf E}\prod_{S}e^{-c_{\rm amb}(n)}\prod_{S'}w(r)\) with \(c_{\rm amb}(n)\ge\frac12c_\square(n,R)\).

With (TC), define \(O_r^{\rm loc}\) by running the label rules with \(A_{\rm loc}\) in place of \(A\); then \(O_r\subset O_r^{\rm loc}\cup\bigcup_{(n,\square)\in\mathrm{cone}(r)}\mathrm{Amb}_{n,\square}\), all events on the right are tile-local, and T2 applies to the family \(\{O^{\rm loc}\}\cup\{\mathrm{Amb}\}\) provided (J_U) holds for it. (TC) is **not** a label event of the construction: on the collar the actual test may pass, and the small-field integral restricted to the collar is not bounded by any printed estimate. It is the exact residual analytic statement for the chessboard route. Conjecturally, it to be true (the collar carries the same Gaussian weight \(e^{-\frac12\langle A,\Delta A\rangle}\) at \(|A|\approx g^{-1}\delta\) that produces the \(R\)-factor on p.380), but it is not proved here and not in the source.

### 5.4 Components crossing tiles

(FP) suffices even for lineages larger than a tile: Proposition 4.3 uses flagged *cubes*, each local to one of the tilings; a lineage's cost is the sum of its cubes' costs up to \(C_{\rm fat}\). No cluster or moat construction is needed. This removes the objection "multi-scale dissemination" of IM §7.6: a single tiling at the terminal scale with tile side \(L^{q'}S_{\max}\) serves all scales, since the per-tile constant \(\mathsf E/N\) is paid by any single record.

### 5.5 The R-free regime

If no \(\mathbf R\) operation occurs before step \(K\) (as on the B-02 witness, §3.3), the actual fields are \(V_n=\mathcal M^n(U)\) everywhere, no seeds beyond the gauge ones are needed, and (FP) holds for all labels except the \(R\)-type flags; (TC) remains the only gap for the chessboard route there too. (In that regime T1 already settles (T_J) when the volume is small, so the chessboard route matters only for hypothetical R-free sequences with large terminal volume.)
