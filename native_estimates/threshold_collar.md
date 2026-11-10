# Threshold collars, reflection and growth of the dependency cone

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

## 2. The cone obstruction

### 2.1 The cone is forced — additional assumption

Let \(r\) be the record "\((n,\square)\) is flagged". TM's local algorithm \(\mathcal C^{\rm loc}\) runs every rule with \(A_{\rm loc}\) in place of \(A\). For \(O_r\subset O^{\rm loc}_r\cup\bigcup_{c\in{\rm cone}(r)}\mathrm{Amb}_c\) to hold, the cone must contain every R-test whose literal outcome can change \(O_r\) or \(O^{\rm loc}_r\).

Take \(m<n\) and a step-\(m\) test cube \(\square_m\subset\square\), and suppose the two algorithms differ only at the R-test of \((m,\square_m)\): the literal test passes and the local one fails. In \(\mathcal C^{\rm loc}\) a region \(X\ni\square_m\) is then born at step \(m\).

* If \(X\)'s lineage is not replaced before step \(n\) (for instance because later births occur in it), the growth rule (1.76) adds at least ten layers of \(MR\)-cubes per step.
* So \(Z_n\) contains a step-\(n\) neighbourhood of \(\square_m\) of side \(\ge10MR_n\supset\square\), since \(M\gg LM_2\) (Port note l.7).
* Then \(\square\) is not a testable cube at step \(n\) in \(\mathcal C^{\rm loc}\), while it can be flagged in the literal algorithm.

Such configurations form a set of positive probability. The conditions are open conditions on the field together with a collar condition at one bond additional assumption. Hence

\[
{\rm cone}(r)\ \supset\ \{(m,\square_m):m<n,\ \square_m\subset\square\ \text{a step-}m\text{ test cube}\},\qquad \#\{\square_m\}=L^{d(n-m)}\Bigl(\frac{R_n}{R_m}\Bigr)^d.
\]

### 2.2 Proposition 2.1

**Assumptions.**

* **(AF)** The source trajectory satisfies \(g_m^{-2}\le g_n^{-2}+b_1(n-m)\) for \(m\le n\). This is Annex W (2.11), \(w_{j-1}=w_j+\beta_j(g_{j-1})\phi_j\), with \(0\le\beta_j\le b_1\) assumed input.
* \(R_m=(\log g_m^{-2})^r\).
* **Collar costs of polylogarithmic size:** \(c_{\rm amb}(m)\le C_a(\log g_m^{-2})^a\) for fixed \(a,C_a\).

The last assumption covers TM's requirement \(c_{\rm amb}\ge\frac12c_\square(m,R)\asymp p_0(g_m)^2\). It also covers any improvement by the collar's thinness, since \(\log(1/\eta_m)\asymp R_m\) by (3.19).

**Statement.** For a record at step \(n\), the factor that TM's reduction attaches to it is at least

\[
\Sigma_n:=\sum_{j=0}^{n}L^{dj}\Bigl(\frac{\log g_n^{-2}}{\log(g_n^{-2}+b_1j)}\Bigr)^{dr}\exp\bigl(-C_a(\log(g_n^{-2}+b_1j))^a\bigr).
\]

For every fixed \(g_n\), \(\Sigma_n\to\infty\) as the depth \(n\to\infty\). Hence on a sequence with fixed terminal coupling and depth \(K\to\infty\), the bound the reduction gives for \(\mathbb P(O_r)\) itself is larger than \(1\) at large depth.

**Proof.** T2 bounds intersections of records. \(A_t=\bigcap_{r\in R_t}(O^{\rm loc}_r\cup\bigcup_{\rm cone}\mathrm{Amb})\) must therefore be expanded into a union over choices of one event per \(r\), and T2 applied to each term. Summing over choices gives

\[
\mathbb P\Bigl(\bigcap_tA_t\Bigr)\le\prod_te^{\mathsf E/N}\prod_{r\in R_t}\Bigl(w(r)+\sum_{c\in{\rm cone}(r)}e^{-c_{\rm amb}(c)}\Bigr).
\]

The same bound arises if the chessboard is applied to \(A_t\) directly, since bounding \(\mathbb P(\bigcap_s\vartheta_sA_t)\) from (J_U) and (TC) goes through the same expansion. By §2.1, the inner sum is \(\ge\Sigma_n\). For \(j\to\infty\), the \(j\)-th term is \(\exp(dj\log L-C_a(\log(g_n^{-2}+b_1j))^a-O(\log\log j))\), and this tends to \(\infty\) because \((\log x)^a=o(x)\). \(\square\)

**Remark 2.2 (magnitudes).** Take \(d=4\), \(L=13\), \(2p_0\in\{20,24\}\) and \(c=\frac14\). The first depth at which a single cone term exceeds \(1\) is about \(10^{37}\) or \(10^{47}\) (`collar_checks`, item 1). The obstruction is real only because the integrated test demands uniformity in depth. On the "future candidate with \(\max_{j\le K_n}Y_j\le C(1+n)\)" of the Port note (l.47), \(p_0(g_m)^2\le C(\log n)^{2p_0}\) while the depth is of order \(n\). The obstruction applies there too.

**Remark 2.3 (what this does and does not show).** It refutes TM's reduction, not (J). The physical reason additional assumption: deep-ultraviolet large fields are *typical* in a coarse cube. The expected number of step-\(m\) R-flags in a step-\(n\) cube is about \(L^{d(n-m)}e^{-cp_0(g_m)^2}\), which is unbounded in depth. Bałaban replaces and sums them, and Theorem C′ never sees them. A pointwise comparison of two different algorithms sees all of them. The comparison breaks down exactly as soon as the two algorithms resample differently.

**Corollary 2.4 (shallow sequences) — conditional.** Suppose
\[
\sup_n\sum_{m\le n}L^{d(n-m)}(R_n/R_m)^de^{-c_{\rm amb}(m)}\le\exp(-\theta'c_\square(n)),
\]
which roughly means \(p_0(g_K)^2\gtrsim K\log L\). Then TM's route closes for flagged-cube records, with (TC) from Theorem 3.1 and (TC_post) of §3.3. Such sequences have a terminal coupling that tends to \(0\), so they are not the physical sequence. They are recorded only for completeness.

## 3. The collar bound itself

### 3.1 Setting

The setting is the ★ path space of DN-1 §3. At the T sub-step \(s\) of RG step \(n\):

* The current free coordinates \(z_n\) are the scaled fluctuation variables \(A_n\) on the final small-field domain \(\Lambda_n\) (CMP 119 (1.20)/(3.20)).
* They are integrated in that step and are not part of the state afterwards (DN-1 §5.1 item 4).
* The step-\(n\) R-labels are exposed before \(z_n\) is integrated. They belong to the domain \(\mathcal D_{n,v}\) of the step law (Annex W (3.14), c\*).
* \(\nu_{n,v}\) is the regular conditional law of \(z_n\) given \(\mathcal G^\star_s\), which contains all labels up to and including step \(n\).

Write \(t_n=g_n^{-1}\delta_n\asymp A_1p_0(g_n)\) for the R-threshold in scaled units (CMP 119 p.247: \(\delta_0=g_0A_1p_0(g_0)\); p.265: \(\delta_k=g_kA_1A_0^{-1}p_0(g_k)\); the two pages use different \(A_0\) conventions). For a test cube \(\square\) at step \(n\) and a width \(w\ge0\):

\[
\mathrm{Coll}^w_{n,\square}:=\{\square^{\sim2}\subset\Lambda_n\}\cap\{\text{the R-test at }\square\text{ passes}\}\cap\{\exists b\in(\square^{\sim2})^*:\ |A_n(b)|\ge t_n-w\}.
\]

The first two events are labels. The third concerns \(z_n\).

**(FT) Fiber tail.** There are \(c_F>0\) and \(m_F<\infty\) such that for every step \(n\), every active ★ datum \(v\), every finite set \(B\) of distinct free bonds in \(\Lambda_n\) and every \(s\ge0\),
\[
\nu_{n,v}\Bigl(\bigcap_{b\in B}\{|z(b)|\ge s\}\Bigr)\le\exp\bigl(-c_F|B|(s-m_F)_+^2\bigr).
\]

### 3.2 Theorem 3.1 (label-conditional collar bound) — conditional: inputs (Mem★), (FT)

Let \(\mathcal S\) be a finite set of pairs \((n,\square)\). Assume that for each \(n\) the neighbourhoods \(\square^{\sim2}\) of the cubes in \(\mathcal S_n\) are pairwise disjoint. Then for **every** event \(L\) in the σ-field generated by all labels,

\[
\mathbb P\Bigl(L\cap\bigcap_{(n,\square)\in\mathcal S}\mathrm{Coll}^{w_n}_{n,\square}\Bigr)\ \le\ \mathbb P(L)\prod_{(n,\square)\in\mathcal S}N_b\exp\bigl(-c_F(t_n-w_n-m_F)_+^2\bigr),
\]

where \(N_b\) bounds \(\#(\square^{\sim2})^*\).

**Proof.**

*Setup.* Let \(n_1<\dots<n_p\) be the steps that occur in \(\mathcal S\), and put \(C_i:=\bigcap_{\mathcal S_{n_i}}\mathrm{Coll}\). Induct on \(p\); the case \(p=0\) is trivial. Let \(s\) be the T sub-step of \(n_1\).

*The future factor.* \(\mathbf 1_L\mathbf 1_{C_2\cap\dots\cap C_p}\) is a function of three things:

* the labels up to step \(n_1\), which are \(\mathcal G^\star_s\)-measurable;
* the state after \(s\), which is \(\mathcal G^\star_s\)-measurable and does not contain \(z_{n_1}\);
* auxiliary variables created later.

By (Mem★)(ii), the conditional law of each later auxiliary variable given the past depends only on the current ★ data. By induction over the later sub-steps (as in DN-1 Prop. 4.2), \(\mathbb E[\mathbf 1_L\mathbf 1_{C_{\ge2}}\mid\mathfrak F_s]=\varphi\), with \(\varphi\) \(\mathcal G^\star_s\)-measurable. In particular \(\varphi\) does not depend on \(z_{n_1}\).

*The step-\(n_1\) factor.* \(C_1\) is the intersection of a \(\mathcal G^\star_s\)-measurable label event with \(\{z_{n_1}\in B(v)\}\), where
\[
B(v)\subset\bigcup_{(b_\square)}\bigcap_{\square\in\mathcal S_{n_1}}\{|z(b_\square)|\ge t_{n_1}-w_{n_1}\},
\]
the union running over choices of one bond \(b_\square\in(\square^{\sim2})^*\) per cube. The chosen bonds are distinct by the disjointness assumption. So (FT) gives
\[
\nu_{n_1,v}(B(v))\le N_b^{|\mathcal S_{n_1}|}e^{-c_F|\mathcal S_{n_1}|(t-w-m_F)_+^2}=:q_1.
\]

*Conclusion.* \(\mathbb P(L\cap C_1\cap C_{\ge2})=\mathbb E[\mathbf 1_{C_1}\varphi]=\mathbb E[\nu_{n_1,v}(B(v))\,\mathbf 1_{\rm lab}\varphi]\le q_1\mathbb P(L\cap C_{\ge2})\). The induction hypothesis finishes the proof. \(\square\)

**Remarks.**

* `collar_checks` item 2 runs exact enumeration on a toy chain. The worst ratio is \(1.0000\), attained. Dropping the Markov premise (a future label that reads \(z\)) gives \(1.0\) against \(q=0.43\).
* This is not a field-conditional bound of the kind excluded by PE Prop. F. It conditions on labels and on *coarse* retained data, and the collar variable is a fresh fluctuation integrated at its own step.
* The same argument does **not** work for R-*flags*. A flagged cube's fluctuation is a postponed variable that later maps read, so the future is not conditionally independent of it. This is why R-records need a different normalizer at all.

### 3.3 Lemma 3.2 ((FT) from coercivity) — deduction; external theorem

Let \(\nu=Z^{-1}e^{-W}\mathbf 1_K\,dz\) on \(\mathbb R^N\), with \(K\) closed and convex, and \(D^2W\ge c_H\) on \(K\). Assume \(|\mathbb E_\nu z(b)|\le m_0\) for every bond, with \(z(b)\in\mathbb R^k\) and \(k=\dim\mathfrak g\). Then (FT) holds with \(c_F=c_H/2\) and \(m_F=m_0+\sqrt{k/c_H}\).

*Proof.*

1. By Caffarelli's contraction theorem (ext; it covers log-concave perturbations of a Gaussian, convex restrictions included), \(\nu=T_\#\gamma_{c_H^{-1}}\) with \(T\) \(1\)-Lipschitz.
2. \(F=\sum_{b\in B}|z(b)|\) is \(\sqrt{|B|}\)-Lipschitz. Gaussian concentration gives \(\nu(F\ge\mathbb E_\nu F+u)\le e^{-c_Hu^2/(2|B|)}\).
3. By Brascamp–Lieb external theorem, \(\mathbb E|z(b)-\mathbb Ez(b)|^2\le k/c_H\), so \(\mathbb E_\nu F\le|B|m_F\).
4. On \(\bigcap\{|z(b)|\ge s\}\), \(F\ge|B|s\). Take \(u=|B|(s-m_F)\). \(\square\)

**What this asks of the construction.**

* **(HC)** \(-D^2\log\) of the ★ fiber density (Annex W (3.11)+(3.13)) is \(\ge c_H\) on the selected domain, uniformly in history and in the retained data.
* **A mean bound.**

These are the "quadratic lower bound" and "current-scale mean" of **C-08**, on the heterogeneous backgrounds of **C-06**, with the convex-core representation of **C-07**. On \(\Lambda_n\) the selected domain is a product of balls \(\{|A_n(b)|<t_n\}\) in the free coordinates (p.269: "On the domain \(\Lambda_{k+1}\) … there are only the small field characteristic functions from (3.16)", c), hence convex. Dependency check: no ancestor of C-08 is H-02 (§7). (d) that (HC) is what C-06/C-08 will deliver. DN-1 Prop. 4.5.4 warns that coercivity is lost when projecting to coarser σ-fields; the ★ law is the finest, so this is the right law.

### 3.4 TM's (TC) — Corollary 3.3, conditional, and its limits

On cubes with \(\square^{\sim2}\subset\Lambda_n\), (3.19) gives \(|A-A_{\rm loc}|\le\eta_n\). Hence \(\mathrm{Amb}_{n,\square}\subset\{\text{R-flag at }\square\}\cup\mathrm{Coll}^{2\eta_n}_{n,\square}\). Theorem 3.1 together with (J_U) then gives TM's (TC) for such cubes, with \(c_{\rm amb}=c_F(t_n-2\eta_n-m_F)^2-\log N_b\). This is \(\ge\frac12c_\square(n,R)\) when \(c_F\ge\gamma_0\). Otherwise \(c_{\rm amb}\) is a fixed fraction of \(c_\square\), which is enough for every use.

Every other testable cube in \(\Omega_n^{\sim-1}\setminus\Lambda_n\) lies within two cube layers of \(\Omega_n^c\) or of an R-flag (definition (3.20)). Two cases arise:

* If the neighbouring record is new at step \(n\), Amb can be charged to it with bounded multiplicity.
* If the neighbour is an *old* unreplaced component, its lineage pays only the per-step loss \(w_n=O(1)M^dR^{d+1}d'\) per step (RB §1.2). That cannot pay \(e^{-c_{\rm amb}}\) at every step. The collar there concerns a postponed variable of the T-operation (2.7). Its factor would have to come from a reading **(TC_post)**: inserting a thin-shell indicator on a postponed fluctuation into Bałaban's positivity bound of (2.7) (LFR II p.383: "estimated using the positivity properties of the quadratic forms") gives the Gaussian measure of the shell as an extra factor. additional assumption

TM's (TC) "for every \(S\)" is therefore not derivable from Theorem 3.1 alone. Given §2 this is moot for the physical sequence.

## 4. (Cov), rule by rule

**Proposition 4.1.** Fix a tiling and realize the lift as in Lemma 1.1. Suppose:

* **(C1)** every rule of the construction is covariant under \(G_{\mathcal T}\): applying \(g\) to all inputs applies \(g\) to all outputs, including selectors, domains, backgrounds and kernels;
* **(FP)** holds with range \(\rho\);
* \(\ell\ge8\rho_{\rm cum}S_K\).

Then every flagged-cube record at distance \(\ge\ell/8\) from the tile boundary satisfies TM's (Cov) with equal weights and an injective map \(r\mapsto r_s\).

*Proof.* Induct over sub-steps. The record event is computed by covariant rules from the data in its cone, which lies inside the tile. The transported samplers make the randomness covariant. Weights depend only on the step and the test type. Injectivity holds because \(G_{\mathcal T}\) acts freely on tiles. \(\square\)

**Status of (C1), rule by rule.** Covariance is for coordinate reflections through planes that contain the centres of every partition cube and block up to level \(K\). There are no coordinate permutations.

| Rule | Source | Covariance | Label |
|---|---|---|---|
| Wilson action, Haar measure | — | yes | deduction |
| Smoothed axial gauge (1.5)–(1.7) | CMP 119 p.247 | "The main point in introducing it in the form (1.5) is to preserve the Euclidean invariance". Axial contours inside a block are mapped to axial contours by coordinate reflections through the block centre. | source input |
| Block averaging \(M\) | CMP 98, not read | built from block contours; assumed covariant | additional assumption |
| Eliminated bonds \(b_0(c)\), the set \(X^*\) (1.9); linearizing map \(h,D\) | CMP 119 pp.247, 249 | the definition of \(b_0(c)\) is not displayed on the pages read; covariance needed | additional assumption |
| P-test (2.16)–(2.17), (3.2); fresh-field and second-class tests | CMP 119 pp.257, 265 | local minimizer with homogeneous determining set; covariant if the variational problem is | source input for the form; additional assumption for the minimizer's covariance |
| Q-test (3.3)–(3.4) | p.265 | same | source input; additional assumption |
| R-test (3.16), literal | p.268 | covariant globally (the global minimizer is), but **not local** | source input |
| \(R^{\rm loc}\) (§5.2) | — | covariant (per-bond box centred on the blocks of \(b\)) | deduction given the minimizer's covariance |
| Domains (3.5), (3.20), rectangle hulls, growth (1.76), \(S(Z)\) | pp.251, 267–269; LFR II p.381 | purely geometric; commute with isometries that preserve the partitions | deduction |
| Eligibility | LFR I p.177 | geometric and label-defined | deduction |
| Preparatory and exterior tests | LFR I pp.181–198 (via IM, RB) | localized backgrounds of the component | assumed input; additional assumption |
| R kernel, graph choice | LFR II pp.379, 390 (via TM) | averaged over \(2^d\) reflections and \(d!\) permutations | assumed input |

**scope.** (Cov) holds given (C1). (C1) is a reading. Its weakest points are the block averaging, the choice of \(b_0(c)\) and the linearization, which must be checked on CMP 98 and on CMP 119 p.248 (not read here).

## 5. What closes the terminal bound

### 5.1 Theorem 5.1 (exact locality suffices) — conditional

**Inputs.**

* **(FP)** Every rule has finite propagation. There is \(\rho\) such that each label at \((n,\square)\) is a function of the bare links and seeds within distance \(\rho S_n\) together with labels at earlier sub-steps within that distance. **No exception for the R-test.**
* (C1).
* Lemma 1.1 and Lemma 4.1.
* The FILS chessboard estimate external theorem.
* (J_U), i.e. (T_U) together with RB's inputs (M)/(RD)/(S)/(G-R).
* (G1)–(G6).

**Conclusion.** PE's (J) holds for all finite record sets, with \(c^J\ge2\theta c^{\rm Bal}\) and \(\theta=2^{-d-2}/(C_{\rm fat}\cdot4C_1)\). Hence the adopted H-02 test (clauses (1), (3), (4)) holds uniformly in volume, depth and history (PE Theorem R with (G6), RB §1.3 item 7).

*Proof.* TM Prop 4.3, with the per-tiling realization (Lemma 1.1) and the cube-level (J_U) (Lemma 1.2). With (FP), every record at distance \(\ge\ell/8\) from the boundary of a tile of one of the \(2^d\) tilings is exactly tile-local. No Amb events occur, so §2 does not apply. \(\square\)

### 5.2 The local R-test — definition and Lemma 5.2

At the step \(V_k\to V_{k+1}\), for a bond \(b\) of the step-\(k\) lattice, let \(\square_b\) be the union of the coarse cubes of side \(LM_2R_{k+1}\) centred at the blocks that contain the endpoints of \(b\) (one or two cubes). Following CMP 119 (2.16), (3.4), set

\[
U_{k+1,\square_b}:=U\bigl(\mathbf B_{k+1}(\square_b^{\sim4}),\,M^\cdot(Q^{s*}_{k+1}V_{k+1})\bigr),\qquad V^{(k)}_b:=M^k(U_{k+1,\square_b}),\qquad A^{\rm loc}_k(b):=\frac1{ig_k}\log\bigl(V_k(b)V^{(k)}_b(b)^{-1}\bigr),
\]

and replace (3.16) (and (1.18) at the first step) by

\[
1=\sum_{R_{k+1}}\prod_{\square'\subset R^c_{k+1}}\chi\Bigl(\Bigl\{\sup_{b\in(\square'^{\sim2})^{(k)*}}|A^{\rm loc}_k(b)|<t_k\Bigr\}\Bigr)\prod_{\square'\subset R_{k+1}}\chi\Bigl(\Bigl\{\sup|A^{\rm loc}_k(b)|\ge t_k\Bigr\}\Bigr).
\tag{\(R^{\rm loc}\)}
\]

**Lemma 5.2 — deduction, given the minimizer's covariance.**

1. The label at \(\square'\) is a function of \(V_k\) on \((\square'^{\sim2})^*\) and of \(V_{k+1}\) on \(\bigcup_b\square_b^{\sim4}\). It is therefore strictly local, with range \(O(LM_2R_{k+1})\) coarse units, and history-free.
2. It is invariant under gauge transformations of \(V_{k+1}\), since the local minimizer transforms covariantly (p.250 argument).
3. It is covariant under the §4.3 reflections, because \(\square_b\) is defined symmetrically.
4. On cubes where (3.19) applies, \(|A^{\rm loc}_k(b)-A_k(b)|\le\eta_k:=O(1)44d^2B_3^2(1+\beta_0)A_0A_1^{-1}e^{-R_k}t_k\). This requires the analogue of (3.17)–(3.19) for \(\square_b\) in place of \(\square'\), which is the same computation additional assumption. So \(R^{\rm loc}\) and (3.16) agree outside the \(\eta_k\)-collar.

### 5.3 Proposition 5.3 — conditional

Let \(\mathcal C^{\rm loc}\) be the literal construction with (3.16) replaced by \((R^{\rm loc})\), and every other rule unchanged. Then (FP) holds for every rule of \(\mathcal C^{\rm loc}\), given TM §5.2 items 1–7 at TM's labels. Consequently, if \(\mathcal C^{\rm loc}\) satisfies (T_U), (S), (G-R), (G1)–(G6), (M)/(RD) and (C1) as the literal construction is read to, Theorem 5.1 gives the adopted H-02 test for \(\mathcal C^{\rm loc}\) **on every cofinal sequence**, the physical one included.

*Proof.* TM §5.3 identifies (3.16) as the only non-local rule. Every other rule computes from local fields, labels and seeds: the minimizers with homogeneous or component-local determining sets, the geometric rules, and the resampling. Their composition over steps has range \(\rho_{\rm cum}S_n\le\rho\sum_{m\le n}S_m\le C\rho S_n\). The sum is geometric because \(S_m/S_n\le L^{-(n-m)}(R_m/R_n)\), and \(R_m/R_n\) grows only polylogarithmically. \(\square\)

### 5.4 Is the amendment legitimate? — additional assumption, open

Bałaban's objection to a local test is analytic, not combinatorial. A characteristic function that depends on \(V_{k+1}\) through a background spoils the analyticity of the integrated density in \(V_{k+1}\) and the background gauge invariance (1.17) (pp.250, 268). \(R^{\rm loc}\) can be brought into his form.

* **(V1) Change of variables.** On all of \(\Lambda_{k+1}\), change variables \(A_k\mapsto A^{\rm loc}_k\) bond by bond. This is (1.22)/(3.22) with \(g\equiv1\) and \(\mathbf H(b):=\frac1i\log(V^{(k)}(b)V^{(k)}_b(b)^{-1})\). In the new variables the small-field restriction is \(\prod_b\chi(|A^{\rm loc}(b)|<t_k)\), a product of fixed balls, "depending on the fluctuation field only". The induced terms are a Jacobian of type (1.24) and a first-order term of type \(V^{(k)}(S,A,\mathbf H)\), now in the bulk of \(\Lambda\) instead of on \(S\). By (3.19), \(|\mathbf H|\le O(1)\varepsilon_ke^{-R_k}\). Bałaban (p.269): "\(\mathbf H^{(k)}\) is an analytic function of the background field … bounded … by \(O(1)\varepsilon_k\exp(-R_k)\), hence by any positive power of \(g_k\)." The critical point moves by \(O(g_k^{-1}|\mathbf H|)\). The resulting linear term is \(O(p_0e^{-R_k})\) per bond and analytic. It is not the "dangerous" \(g^{-2}\langle A,J_1\rangle\) of p.250.
* **(V2) Large-field factor.** On \(R^{\rm loc}\)-flagged cubes, \(|A|\ge t-\eta_k\). The factor of p.380 becomes \(\exp(-\gamma_0(t-\eta)^2\cdots)\), a relative change of \(O(e^{-R})\). deduction given p.380's mechanism.
* **(V3) The Q-test is implied on passed cubes** with margin, by Lemma 5.2(4) and (3.19). So \(\chi'_k\) can be omitted there as in (3.16).
* **(V4) Background gauge invariance (1.17).** Treat \(\mathbf H\) as a covariant external field. The joint expression is then invariant. additional assumption
* **(V5) construction proposition to re-analysis.**
  * B-01: the selector table entry for "Current free-field split (1.18)/(3.16)".
  * C-01: the term construction (3.11) gains the bulk \(\mathbf H\)-terms.
  * C-02 to C-04 and C-07: new small analytic activities; the domain is still a product of balls.
  * C-05: already carries \(\mathbf H\)-terms on \(S\).
  * B-04/B-05: the coupling recursion shifts by \(O(e^{-R})\) per step.
  * H-01 and H-03: no structural change.

The estimates for the local test require the same amended representation throughout.

### 5.5 The literal construction: tile symmetrization, and why it does not close — additional assumption

The cone obstruction comes from comparing two *algorithms* on one configuration. For each tile \(t\), compare instead one algorithm on two *configurations*: \(\omega\), and \(\Psi_t\omega\), which equals \(\omega\) on \(t\) and its reflected images elsewhere. Crossing seeds are set to a constant.

* \(A_t:=\{\Psi_t\omega\in O_{R_t}\}\) is tile-local. It is exactly covariant by global covariance, since \(g\Psi_tg^{-1}=\Psi_{gt}\).
* Discrepancies between the labels of \(\omega\) and \(\Psi_t\omega\) start at the tile boundary. They move inward:
  * by exact propagation, about \(\rho S_m\) per step;
  * by R-collars, with width \(\varepsilon e^{-\delta x/S_m}\) at distance \(x\). This needs an exponential-decay reading (Dec) of the global minimizer and width-proportional collar bounds.
* A deterministic front profile with free zone \(Z_m\asymp S_m(K-m+q')\) beats the boundary entropy \((\ell/S_m)^{d-1}\) at every scale. The total front depth is \(O(q'S_K)\ll\ell\).
* So \(O_{R_t}(\omega)\subset A_t\cup B_t\), where \(B_t\) ("a collar beyond the front in \(\Psi_t\omega\)") is tile-local with weight \(\beta_*\le C\kappa_*\varepsilon^ae^{-q'}\).
* The chessboard estimate then gives \(\prod_te^{\mathsf E/N}\bigl(w(R_t)+3\beta_*\bigr)\).

**The failure.** \(\beta_*\) does not depend on \(R_t\). PE Theorem R needs (J) for record sets of unbounded cost per tile, for example a large birth region with many flagged cubes. For such sets \(w(R_t)\ll\beta_*\).

Enlarging tiles does not help. Making \(\beta_*\le w(R_t)\) needs \(L^{q'}\gtrsim-\log w(R_t)\). Keeping \(e^{\mathsf E/N}\le w(R_t)^{-1/2}\) needs \(L^{dq'}\lesssim-\log w(R_t)\). The two conditions are incompatible for \(d\ge1\).

One bad event can spoil every record within distance \(\asymp S_{m+R}\) of it, and nothing tile-local recovers their costs. The route gives (J) only for record sets of bounded content per tile, which is insufficient.
