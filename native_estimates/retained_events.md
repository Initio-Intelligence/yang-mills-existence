# Integrated tests for retained large-field events

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

**Local-chart hypotheses.** In every application use (A8′) in the structured form 3′ and 4′, F(4′) on (Avg), (Sm3′), (Par-g_Z′), and (Lay-W), with $M_W\mid M_1$ and $M_1\ge6M_W$. In particular the per-potential rate must satisfy $\kappa_1/2\ge\sqrt d(1+3\beta)\kappa/(1-3\delta)$. The bound on the joint terminal law requires the action estimate and item 4′.

## 1. Theorems

### Theorem I (bounded terminal volume) — conditional

* A cofinal sequence of the construction, at every member of which
\[
(E_++E'_-)(g_{K})\,|T_{K}|\ \le\ \tfrac18\gamma_0A_1^2p_*^2,\qquad p_*=\min_{n\le K}p_0(g_n).
\]
* Premises P1–P4, P10–P12 of §2.
* P5–P6 if replacements (R operations) occur on the sequence.
* P9 if second-class records occur.

**Conclusion.** For every step \(j\le K\) there are weights \(a(Y,b)\ge0\) such that:

1. **(Joint bound.)** \(\mathbb P(\bigcap_iE_{Y_i,b_i})\le\prod_ia(Y_i,b_i)\) for pairwise disjoint step-\(j\) components \(Y_i\).
2. **(Shape-summed bound.)** \(\sum_{b\le j}\sum_{Y\ni x}L^{4(j-b)}e^{\sigma|Y|_\natural}a(Y,b)\le\delta<1\) for every step-\(j\) cell \(x\). Here \(\delta=4\varepsilon_*\exp(-\frac{\theta}{4}\gamma_0A_1^2p_*^2)\), with \(\theta=\frac34\) and \(\varepsilon_*\le\frac12\).

\(E_{Y,b}\) is the label-defined retained event of clause (1) of the test: a whole component of the unreplaced region at step \(j\), with oldest birth \(b\). The constants are uniform in the scale \(j\), the depth and the history. Uniformity in the volume holds within the stated volume window.

**Proof chain.**

1. (T_U) gives (T_J) by TM Theorem T1 (deduction).
2. (T_J), with (M), (RD), (S) and (G-R), gives the joint bound for all marks: IM Theorem C′ deduction and RB Theorem C.
3. Lineage weights, the covering sum and the native sizes then give the conclusion: IM Theorem R″ / RB Theorem R′ conditional, with (G6) from IM Lemma 4.1.

### Corollary I′ (the B-02 witness) — conditional

On the sequence of `Finite Wilson family`, the volume condition of Theorem I holds with margin \(L^{7n-O(1)}\) (TM §3.3). No R operation is performed there (P8). So Theorem I holds with premises **P1–P4, P8, P10–P12 only**. Neither H-03 nor (M) nor (S-Y) is used.

### Theorem II (local test on an admissible sequence; conditional)

Let \(\mathcal C^{\rm loc}\) be the construction with (3.16)/(1.18) replaced by \((R^{\rm loc})\) of TC §5.2.

* Premises P1–P6, P9–P12, read for \(\mathcal C^{\rm loc}\).
* Q1–Q4 of §2.
* **Q5 (open):** the amendment is valid.

**Conclusion.** On every cofinal sequence, the physical one included, the conclusion of Theorem I holds for \(\mathcal C^{\rm loc}\). The constants are uniform in volume, scale, depth and history. Moreover PE's joint record bound (J) holds for all finite record sets, terminal lineages included.

**Proof chain.**

1. TC Prop. 5.3 gives exact finite propagation for every rule.
2. TC Prop. 4.1 / Lemma 1.1 give (Cov).
3. TC Theorem 5.1 = TM Prop. 4.3, which rests on:
   * TM Theorem T2 and Corollary 4.2 deduction;
   * TM Lemma 4.1 deduction;
   * FILS external theorem;
   * (J_U) from P1, P5, P6 via IM Theorem C′, TM §4.4 and TC Lemma 1.2.
4. PE Theorem R (b) then gives the integrated test, with (G6).

### Status II-literal (literal construction, physical sequence) — **open**

What is established:

* IM Theorem R″ reduces the test to (T_J), the joint terminal record bound.
* (T_J) does not follow from unnormalized bounds (TM §3.4, deduction).
* The chessboard route needs exact tile-locality of the record events (TC Theorem 5.1). This fails for the literal construction (TC §1.7, source).
* Collar patches cannot give depth-uniform bounds (TC Prop. 2.1, deduction).
* Tile symmetrization fails for record-dense tiles (TC §5.5, additional assumption).

What would close it: exact locality, through the amendment, or a different normalizing principle. TC §9 discusses both.

Partial results on this sequence, conditional:

* Every event whose lineage closes before the terminal step is covered (RB Theorem R′ without (T)).
* So is the first-step lineage, without any closure input (PE Corollary 3.7).

## 2. Premise list

| # | Premise | Content | Used in | Status | Pointer |
|---|---|---|---|---|---|
| P1 | (T_U) | Per-term reading of the UV-stability upper bound. \(\sum_{h:M\subset C_*}Z_{K,h}\le e^{E_+|T_K|}\prod\zeta^0\). Also \(\mathscr Z\ge e^{-E'_-|T_K|}\), with \(E_\pm\) counting current-lattice sites and \(E_\pm\le C\log g_K^{-2}\). | I, II | source input for the printed bound (2.49)–(2.50) and the lattice of \(E_\pm\); additional assumption for "per term", the lower bound and the size of \(E_\pm\) | TM §2.2 |
| P2 | (S) | LFR II (1.79), read per internal history. | I, II | source input for the derivation pp.380–383; additional assumption for "per history" | IM §2, RB §3.4 |
| P3 | (G-R)\(_{c_0}\) | Bałaban's reserve induction (1.80)–(1.88), with free loss constant \(c_0\); requires \(p_0\)-exponent \(\ge6r\). | I, II | source input for the induction; deduction for the \(c_0\)-scaling, given that it is printed as read | RB §1.2 |
| P4 | (G1)–(G5), (G6) | (G1)–(G5): cubes, growth (1.76)/(1.84), ancestry determined by records, size \(>20MR\), \(R_{n+1}/R_n\in[L^{-1},L]\). (G6): native cells lie in ancestor cubes. | I, II | source input; additional assumption for (G1)–(G5) (PE §3.1); deduction from source input for (G6) | PE §3.1, IM §4 |
| P5 | (M) = (Mem★) | No memory across steps on the ★ state. | I, II (only if replacements occur) | source input for all structural premises (LFR II (1.33)–(1.35), (1.72), (1.98)–(1.104)); additional assumption for the conclusion | IM §1, DN-1 §3 |
| P6 | (RD) | Closure domination: HS20.1, HS20.4, HS20.7 of Annex BI (H-03); \(\lambda_R\le\frac14p_0\) suffices. | I, II (only if replacements occur) | assumed input: accepted H-03 result; IM §6 checked uniformity next to old components (source input; deduction) | RB §3.2, IM §6 |
| P7 | Trajectory hypothesis | \(g_k\le\gamma\) along the actual trajectory (LFR II Theorem 1). | everything | Standing construction hypothesis (B-proposition); not H-02's obligation | Annex W §0 |
| P8 | B-02 geometry | Periods, centring, and "no (1.76) processing" (no R operation) on the witness. | I′, and the §4.3 geometry of II | assumed input | `Finite Wilson family`, TM §3.3 |
| P9 | (S-Y) | Second-class factor \(\chi_k^c(Y^{\sim-6})\), paid by the Wilson term of the new action. | I, II (only with second-class records) | source input for location, function and Wilson term; additional assumption for "the p.380 factor applies" | TM §1 |
| P10 | Parameters | \(p_0\)-exponent \(\ge6r\), \(r\ge2\); \(\gamma\) small depending on \(\sigma,L,M,d,c_0\). | I, II | choice | RB §1.2, parameter assumptions |
| P11 | \(\sigma\) fixed | The carrier threshold of (M.2) plus \(q_0A^{1/q_0}\) is a constant independent of \(\gamma\). | I, II | assumed input: M-03 constants | RB §6.2 |
| P12 | Lift | H-01 path space (Annex W §§2, 4). \(\mathbb P(H=h)=Z_{K,h}/\mathscr Z\). Law \(\mu_W\otimes\mathrm{Leb}^I\) with labels as functions. | I, II | assumed input: accepted H-01; deduction for the product form given Annex W (2.13) | TM Lemma 4.1, TC §1.2 |
| Q1 | (FP) for every rule except the R-test | P/Q/second-class tests, growth, eligibility, preparatory and exterior tests, resampling: all local. | II | source input for P, Q, growth and second class (CMP 119 pp.257, 265; LFR II p.381); assumed input for preparatory/exterior (LFR I p.183, via IM); assumed input for the kernel | TM §5.2 |
| Q2 | (FP) for \(R^{\rm loc}\) | Strictly local, gauge invariant, covariant. | II | deduction, given the minimizer's covariance | TC Lemma 5.2 |
| Q3 | (C1) global covariance | Every rule is covariant under the site-plane reflections of TM §4.3. | II | source input for the axial gauge (p.247); assumed input for the R kernel; deduction for the geometric rules; **additional assumption for the block averaging (CMP 98), the eliminated bonds \(b_0(c)\) and the linearizing map** | TC §4 |
| Q4 | RP / chessboard machinery | Lemma 4.1 (RP of \(\mu_W\otimes\) seeds), T2, Corollary 4.2, per-tiling realization, cube/region costs. | II | deduction; FILS chessboard external theorem | TM §4, TC Lemmas 1.1–1.2 |
| Q5 | **Validity of the amendment** | Bałaban's small-field analysis and bounds hold for \(\mathcal C^{\rm loc}\): bulk \(\mathbf H\)-terms of size \(O(1)\varepsilon_ke^{-R_k}\) from the global change of variables (1.22)/(3.22) with \(g\equiv1\); background gauge invariance with \(\mathbf H\) as a covariant external field. All of P1–P6, P9, read for \(\mathcal C^{\rm loc}\). | II | conditional on the structured local-chart bounds, exact cost attribution and common choice of parameters | TC §5.4 |
| (opt) | (FT), (Mem★) | Fiber tail of the ★ T-step law. Only for the conditional collar bound (TC Theorem 3.1), which no theorem above needs. | — | conditional; (FT) ⇐ (HC) + mean bound (C-06/C-08 type, acyclic) | TC §3 |
