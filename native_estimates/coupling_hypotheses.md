# Hypotheses for a projected Wilson recurrence

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 1. Projected recurrence

**Corollary D′ (A §9.4, N §7).** For the source-free Wilson recursion of CMP119 with \(Y_k=g_k^{-2}\), on \(Y\ge Y_*\): with \(v=1/(Y+D^G_i-d_Bi)\),
\[
v_{m+1}=v_m-d_Bv_m^2+r_m,\qquad d_B=\frac{11N^2\log L}{12\pi^2}>0,\qquad\lvert r_m\rvert\le A\,v_m^3 ,
\]
\(r_m\) history-dependent, \(A\) uniform in depth, volume and history. Logical chain: Theorem A′ (one step; inputs L2, (L1\(^*\)), (R\(^*\)), (F1), (F2)) → Theorems B′, C′ (inputs (P), (C2\(^*\)), (G), (N\(^*\))) → Corollary D′ (algebra, deduction).

## 2. Hypotheses, with status

### 2.1 construction conventions

| | Statement | Status |
|---|---|---|
| **(the level-adapted restriction)** | Native spaces = CMP109 (1.11)–(1.16) with clause (iv) level-adapted: level \(n\) controlled on \(Z^{(n)}=\{\mathrm{dist}_\infty(x,Z^c)\ge2M\ell_{n-1}\}\). | **Adopted** (the level-adapted restriction). Ref §3: Theorem 3.1′ gives the bounds on \(\Omega_n(Z)\supseteq Z^{(n)}\), compatible. |
| **(Conv-CR)**  | For \(\mathbf U=e^{i\xi A'}U\) with real representative \(U\), the reconstructed pair \((U_n(M'(\mathbf U)),J_n(M'(\mathbf U)))\) is CMP102 Proposition 9's extension about the data \(M'(U)\) of the real representative, in the axial gauge relative to \(U_n(M'(U))\). | **Convention.** Ref §2.1: the source's "\(U_n(V)\) in the axial gauges" for complex \(V\) is defined only up to a complex gauge transformation in CMP99 (1.14), because the axial gauge CMP99 (1.19) depends on the reference configuration; clause (iv) for complex data is therefore a statement about a chosen representative. Every use in B-03 and in Annexes AD/AE is of the above form; the bound of (CR) is the same for any reference whose half-tube contains \(M'(U)\). |

### 2.2 Statements about the actual recursion

| | Statement | Status |
|---|---|---|
| **(F1)** | At every admitted step assume $\|\mathbf E^{(j)}\|_j\le E_0$ and $|\mathbf R^{(j)}(X)|\le g_j^{\kappa_0}e^{-\kappa d_j(X)}$ on the native spaces. | The regular and remainder terms require level-adapted restrictions. Restriction of boundary terms on the multiscale spaces of CMP119 (3.43) is a separate hypothesis. |
| **(F2)** | \(c_{k+1}=\mathcal P\) of the whole-lattice birth sum (CMP119 pp.278–279). | source input. |
| **Admission** | The trajectory stays in the admitted region. | conditional by the bootstrap of Theorem C′. |

### 2.3 Single-scale source estimates (L1\(^*\) §4.1)

| | Content | Status |
|---|---|---|
| (S1), (S2) | Generalised axial gauge on cubes, CMP109 (3.26); Landau-gauge minimiser on \(\square_0\), (3.27), (3.37) | source input; (3.26)–(3.27), (3.37) as stated in the source in Ref §1 and §5(a) below. |
| **(S3)** | \(\mathbf H_j=H_{1,j}B+O(B^2)\); decay of \(\delta\mathbf H_j/\delta B\) at non-zero data, CMP109 (3.9), (3.45), (3.50) | source input for the citation; the decay (190) is replaced by C-05 **Theorem T′♯** (Source operators for the deformed reconstruction §6; the five-norm Theorem T′ of the Decoupling note is "not justified as stated", Source operators for the deformed reconstruction §0 (E2), and repaired with representation-defined second-order outputs). conditional on (W-ms), (S-struct)(ii) as re-proved in Source operators for the deformed reconstruction, with the rate, radius and constant changes of CR §7. |
| (S4) | Averaging identities; minimiser of a minimiser (3.38)–(3.39), (3.48)–(3.49) | source input; complex case of (3.38) by analytic continuation. |
| **(S5)** | A-ball at one scale with homogeneous radius \(c_2^{\rm ball}\alpha_0\) | **conditional**: clause-(iv) part by CR Corollary 4.3 with Ref Lemma 4.2′: \(c_2^{\rm ball}=(1280K_c)^{-1}\), \(K_c=8(1+\sqrt2)^3B_3\), under the ceiling \(\alpha_1^2\le\alpha_0/300\); (i)–(iii) parts CMP109 (3.10)–(3.14) source input. |
| (S6)–(S10) | Derivatives and tree decay (CMP109 (4.2)–(4.5), (4.22)); decoupled propagators (CMP116 (1.2)–(1.21)); Ward identities (CMP109 §4); polarization tensor (CMP109 (4.35)–(4.45), §5); unsubtracted families (CMP119 (3.49)). | Source estimates. |

### 2.4 Locality of reconstructions (Theorem 4.1′ of the analysis)

| | Content | Status |
|---|---|---|
| (V1) | [V] Theorem 1 | source input, proved in the source. |
| (V2) | [V] Proposition 9 without (190) | **Upgraded**: for the case B-03 needs (real critical background, complex block field, absolute radius \(r_9\), first- and second-order bounds) it is Source operators for the deformed reconstruction **Theorem P9♮**, conditional on printed source statements: [P] Thm 3.3 (\(G_0\), incl. Laplacian inequality; proof rests on sketched Thm 3.10), Thm 3.12/(3.133), (3.49), (3.132) (asserted), (3.137); [V] (130), (137)–(140), (143), (179)–(180), Props 3, 4 , (62), (104), Prop 6; Source operators for the deformed reconstruction Lemma 3.1. Caveat: variable \(B\) vs \(B'\), factor \(\le2dL\) in the radius. |
| (V3′) | Linear propagator bounds, incl. second order in a background | For (CR): subsumed in P9♮. For the locality theorem's current clause: CR §5 reduces it to [V] (130), [P] Thm 3.3 (\(G_0\)), (3.132), (3.137) by a Neumann series conditional; Ref §6 item 4 agrees in structure. |
| (V5)–(V7), (G1)–(G3) | Axial gauge and plaquettes, change from Landau to axial gauge and local expansion of the current (regular configurations, (1.43)–(1.54), (1.65), (1.70)–(1.72)); maximal domain sequence, constraints determined by finer data and nested axial conditions. | Source estimates and domain geometry. |
| **(CR)** | For \(\mathbf U=e^{i\xi A'}U\) on \(Z\) with \(\lvert A'\rvert\le a_1\), complex curvature \(\le a_c\xi^2\), below absolute ceilings (Ce1)–(Ce3): \(\lvert\partial U_n(Z;M'(\mathbf U))-1\rvert\le K_c(a_c+344a_1^2)\xi^2\), \(\lvert J_n\rvert\le K_c(a_c+344a_1^2)\ell_n^2\) on \(\Omega_n(Z)\supseteq Z^{(n)}\), \(K_c=8(1+\sqrt2)^3B_3\), uniform in level, number of levels, scale, \(Z\), \(M\), torus; reconstruction defined per (Conv-CR). | **conditional** (CR Theorem 3.1 as amended in Ref Theorem 3.1′) on: [V] Theorem 1; P9♮ and its list; [A] Props 2, 4, 6, 7; [R] (1.47)–(1.54); the Landau→axial map [A] (106) with [R] (1.70)–(1.72) for complex fields ((c) real, (d) complex). **No unproved-source premise, no (W-ms), no walk expansion, no (190).** The analysis form (with \(a_1^\nabla\)) follows by Lemma 4.2′ with \(K_c'=344K_c\). Ceilings (Ce1)–(Ce2) with \(T_0\asymp B_0^{12}\) are coupling ceilings on the running chart. |

Theorem 4.1′ (locality): real half conditional under the same hypotheses; complex half conditional on (CR) above, hence on source inputs only.

### 2.6 Cluster expansion, readout, comparator, calibration

| | Statement | Status |
|---|---|---|
| **Lemma L2** | CMP116 §2 expansion as a bounded holomorphic map on the potentials | conditional. Delivery on native polymer spaces is (S-Res-1): holds under the level-adapted restriction by §2.4. |
| **(L1\(^*\))** | E potentials, linear, gain \(\rho_k\), age sum uniform (L1\(^*\) Theorem 3.1) | conditional on (S1)–(S9), §2.4, CMP119 (2.6)–(2.7), (K1)–(K8′). **Lemma 5.1 (CMP109 Lemma 4 with running radii) line-as stated in the source of CMP109 pp.276–280** (§5(a) below): every inequality matches; (K1)–(K5) are the source's conditions with the running factors. §§6–7 read for structure, construction (6.2) assumed (as assumed here). |
| **(R\(^*\))** | Mature R potentials, \(C_R\rho_kg_k^{\kappa_0-7}\) (L1\(^*\) Theorem 3.3) | conditional, same inputs plus (S10) and the lower slope. The per-domain identity CMP119 (3.49) is used in place of CMP109 (4.34) (L1\(^*\) §10 item 5); not assumed where used. |
| **(P)** | \(\lvert\mathcal PF\rvert\le C_P\alpha_2^{-2}\lVert F\rVert\) | conditional on (S5) (now conditional), (S6). |
| **Driven comparator** | The pure regular comparator with an exogenous coupling sequence reproduces the Gaussian projection to order $1/Y_k$. | Requires flat-background derivative constants, hard-cut moments and the same canonical cutoff convention for both integrals. See [the comparator](driven_comparator.md). |
| **(G)** | The sum of the actual scalar Gaussian projections has the bounded linear remainder in [Gaussian calibration](gaussian_calibration.md). | Open; requires composite identification and the uniform transverse remainder. |
| **(N\(^*\))** | \(\beta'\ge\frac54d_B+2B_G\), lower-slope sums, suffix device | conditional; source input under the same hypotheses. |

### 2.7 Constants and their order

1. \(L\) (odd, admitted; \(L\ge3\) for the first half of (K7)).
2. \(M\ge M_0\): the source's \(M(\kappa)\), \(M\ge(1+L)R_1M_1\), first term of (K8′), and the enlargement by \(\asymp2^{d+6}L^2\sqrt d\) from the T′♯ rate (CR §7). Not quantified.
3. Ratios: (K1)–(K3) with \(c_2\le c_2^{\rm ball}=(1280K_c)^{-1}\); \(c_3\le1/(32B_3)\); \(q>p_0\); **\(\kappa_0\ge16\)** (see §5(d)).
4. Ceilings on the coupling: (K4)–(K6), second half of (K7) with \(K_\flat=1+\beta/2\), second term of (K8′); \(Y_*\ge Y_\sharp\); **new from (CR)**: (Ce1) \(\alpha_1\le\rho_9/(64T_0)\), (Ce2) \(4(1+T_0)\alpha_0+688(1+T_0)^2\alpha_1^2\le\varepsilon^\sharp\) (with \(\ell_n\le1\)), (Ce3); \(\alpha_1^2\le\alpha_0/(688K_c)\) for the corrected (1.17) at full radius; \(\alpha_1^2\le\alpha_0/300\) for (S5); \(344K_cc_{\rm loc}^2\alpha_0\le\frac14\); the radius of T′♯, \(\alpha_{3,j}\lesssim\varepsilon_{\mathcal H}\) (depends on \(M\)). All absolute or \(M\)-dependent numbers; none depends on age, depth, torus or history.
