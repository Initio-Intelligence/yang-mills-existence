# Iteration of the projected coupling

The coupling recurrence is conditional. For the projected sum $C_n$ of the actual constrained Gaussian increments, Gaussian calibration requires identification with the composite constrained Gaussian and $\sup_n|C_n-nd_B|<\infty$. The finite-dimensional projection and the logarithmic shell coefficient do not prove this uniform bound. In the transverse decomposition it requires $\sup_n|\mathcal B_n|<\infty$. Level-adapted restriction, real-centered complex reconstruction, the multiscale boundary restriction, flat-vertex constants and a common coupling ceiling are required in the same representation. See [Gaussian calibration](gaussian_calibration.md) and [complex reconstruction](complex_reconstruction.md).

## 1. Objects and notation

### 1.1 Conventions

- **Couplings.** \(Y_k=g_k^{-2}\) is Bałaban's normalized-trace Wilson coefficient, \(\ell_k=\log Y_k\). The index \(k\) increases toward the infrared, so the actual decrement is \(c_{k+1}=Y_k-Y_{k+1}=\beta_{k+1}(g_k)\) (CMP119 (2.24), p.259; CMP109 (0.20), p.256).
- **Cutoff and radii.** The normalized cutoff is \(P_k=A_1\ell_k^{p_0}\) with \(p_0>1\); the physical cutoff is \(\delta_k=g_kP_k\) (AD (E14.20); CMP119 (2.4), with \(\varepsilon_j=g_jA_0(\log g_j^{-2})^{p_0}\)). The running analytic radii are \(\alpha_{u,k}=C_ug_k\ell_k^q\) for one fixed integer \(q>p_0\) (CMP119 (2.28); AD Theorem E14.3). Write \(r_k=c_r\alpha_{0,k}\).
- **Spaces and bounds.** \(\mathcal U_j(X)=U^c_j(X,\alpha_{0,j},\alpha_{1,j})\) is the native regular space of CMP109 (1.11)–(1.16), with the running radii of CMP119 (2.26)–(2.28). The localization size is \(d_j(X)\) (CMP109 p.257). The source decay constant is \(\kappa\), and \(\kappa_*<\kappa\) is the decay left after the fixed CMP116 Lemma 1 losses. The R exponent is \(\kappa_0\) (CMP119 (2.31)).
- **Gaussian benchmark.** \(d_k^G\) is the uncut stationary Gaussian decrement in \(Y\) units, \(D_n^G=\sum_{k<n}d_k^G\), and \(d_B=11N^2\log L/(12\pi^2)\) (the finite-cutoff construction §1; the coupling comparison, coefficient paragraph).

### 1.2 Birth families, norms and the projection

A **birth family at scale \(j\)** is \(F=(F(X))_{X\in\mathbf D_j}\). Each \(F(X)\) is holomorphic on \(\mathcal U_j(X)\), depends on the fields in \(X\), and is gauge invariant (CMP109 (1.19)). The unrestricted whole-lattice sum is Euclidean covariant (CMP119 (2.29)). Its native norm is
\[
\|F\|_j=\sup_{X\in\mathbf D_j}\ \sup_{\mathcal U_j(X)}|F(X)|\,e^{\kappa d_j(X)}.
\tag{P22.1}
\]
The CMP119 inductive hypothesis is \(\|E^{(j)}\|_j\le E_0\) for the raw (pre-subtraction) births (CMP119 (2.26)–(2.27) with property (iv) = CMP109 (1.18)).

For such \(F\) at scale \(k+1\), \(\mathcal PF\) denotes its Wilson coefficient in \(Y\) units. It is computed by the second spatial moment of the infinite-volume polarization tensor at the flat field (CMP109 (1.20)–(1.22), p.264). It is **linear** in \(F\). The actual decrement is \(c_{k+1}=\mathcal PE^{(k+1)}\) (CMP119 p.279).

### 1.3 The step-\(k\) input, activities and the single-step map

An **input at step \(k\)** is a pair \(\mathcal I=(F,\mathcal R)\).

- \(F=(F_j)_{j\le k}\) is a tuple of raw birth families. The step-\(k\) exponent contains \(F_j-F_j(1)-(\mathcal PF_j)A\), so each birth enters with its *own* Wilson subtraction.
- \(\mathcal R\) is the family of mature (absorbed) R terms. CMP119 p.271 includes \(\mathbf R'_k=\sum_{j\le k_1}\mathbf R^{(j)}\) into \(\mathbf E_k\).

**Activities.** Let \(\mathcal K_{k,Y}\) be the product contour (E14.49) for a carrier \(Y\in\mathbf D_k\):
\[
\|z\|_\infty<2P_k,\quad \|b\|_{{\rm native},k}<c_{\rm ext}\alpha_{0,k},\quad
\|J-J_{0,k}\|_\infty<c_{\rm ext}\alpha_{0,k},\quad |s(\Delta)|<e^{\kappa_1}.
\]
Let \(\mathcal K^{T}_{k,Y}\) be the same contour with \(\|z\|_\infty<2T_kP_k\), where \(T_k:=\ell_k^{(q-p_0)/2}\). The activity space \(\mathfrak A_k\) consists of families \(V=(V_Y)_{Y\in\mathbf D_k}\) holomorphic on \(\mathcal K_{k,Y}\), with norm
\[
\|V\|_{\mathfrak A_k}=\sup_Y\sup_{\mathcal K_{k,Y}}|V_Y|\,e^{\kappa_*d_k(Y)}.
\tag{P22.2}
\]

**Linear activity maps.** \(\mathcal V^E_k(F)\) is the localized fluctuation difference of the subtracted sum of the \(F_j\). Precisely, it is the right side of CMP116 (1.33), equivalently AD (E14.16), with \(\mathbf E_k\) replaced by \(\sum_j[F_j-(\mathcal PF_j)A]\). \(\mathcal V^R_k(\mathcal R)\) is the localized R pullback contribution of AE §10, (RM.13). Both maps are **linear**. Each is a fixed sequence of evaluations at the actual insertion maps, Cauchy integrals in the decoupling parameters and partitions of unity. The maps and geometry do not depend on the activities (CMP116 (1.10), (1.23); AD §§3–5).

**Single-step representation.** For the homogeneous whole-lattice regular step with Wilson coefficient \(Y_k\) and cutoff \(P_k\),
\[
H_{k+1}[\mathcal I]=\mathcal G_k+\mathcal C_k\big(\mathcal V^E_k(F)+\mathcal V^R_k(\mathcal R)\big).
\tag{P22.3}
\]

- \(\mathcal G_k\) is the input-independent part: the background-dependent Gaussian log-determinant and its normalizer, CMP119 (3.33)–(3.37) first two lines, and the cutoff term.
- \(\mathcal C_k(V)\) is the localized logarithm of the normalized cutoff-Gaussian expectation of \(\exp(V_P+V)\). Here \(V_P\) are the Wilson-remainder activities of \(P^{(k)}(g_k,\cdot)\) (CMP116 Lemma 2; CMP119 (3.30), (3.37)).

\(V_P\), the covariance, the cutoff and all maps depend only on \(Y_k\), \(P_k\) and the background. The input enters only through the activity \(\mathcal V^E_k(F)+\mathcal V^R_k(\mathcal R)\). The fluctuation measure does not depend on the input. In CMP116 pp.10–11 the quadratic form \(Q\) of Lemma 2 (1.42)–(1.43) comes from cancelling \(1/g_k^2\) in \(P^{(k)}\). If any part of \(Q\) depended on the input, it would be included in the activity data, and the argument below would be unchanged.

### 1.4 The two recursions

**Actual homogeneous recursion.** \(\mathcal I^{\rm act}_k=((E^{(j)})_{j\le k},\mathcal R_k)\), where \(E^{(j)}\) are the actual whole-lattice raw births and \(\mathcal R_k\) the actual mature R family at step \(k\). Then
\[
E^{(k+1)}=H_{k+1}[\mathcal I^{\rm act}_k],\qquad c_{k+1}=\mathcal PE^{(k+1)},\qquad Y_{k+1}=Y_k-c_{k+1}.
\tag{P22.4}
\]

**Driven comparator \(\mathfrak B'\).** \(\mathcal I'_k=((H'_j)_{j\le k},0)\), and
\[
H'_{k+1}=H_{k+1}[\mathcal I'_k]\ \text{ computed with the actual }Y_k,\qquad p'_{k+1}=\mathcal PH'_{k+1}.
\tag{P22.5}
\]
Its Wilson coefficient at step \(k+1\) is prescribed to be the actual \(Y_{k+1}\); it is **not** \(Y_k-p'_{k+1}\). Equivalently, \(\mathfrak B'\) is the pure small-field recursion plus a Wilson counterterm \((c_{k+1}-p'_{k+1})A\) inserted after each step. This is the z = 0 endpoint of the family in [Reset remainders](../coupling/reset_remainders.md) §4 ("the ordinary E-only map at the same externally specified couplings"). Both recursions start from the bare Wilson density \(\exp(-Y_0A)\) (CMP119 Theorem 1).

**Differences.** Put
\[
\delta H_j=E^{(j)}-H'_j,\qquad D_k=\sup_{j\le k}\|\delta H_j\|_j\quad(D_0=0).
\tag{P22.6}
\]
Since \(\mathcal P\) is linear, \(c_j-p'_j=\mathcal P\delta H_j\). The step-\(k\) exponents of the two recursions differ by
\[
\sum_{j\le k}\big[\delta H_j-\delta H_j(1)-(\mathcal P\delta H_j)A\big]+\mathcal R_k.
\]
Every summand in the bracket is marginal-free, and the Wilson coefficient \(Y_k\) is identical. This is the structural point of the reformulation.

**Remark (no hidden marginal term).** Summed over \(j\), the subtractions above contain the current-scale Wilson term \(-t'_kA(U_k)\), with \(t'_k=\sum_{j\le k}(c_j-p'_j)\). This is the accumulated difference between the actual decrements and the comparator's own projections. Unlike the self-consistent comparator (§8(ii)), it does **not** enter as a free marginal perturbation. Each piece \((\mathcal P\delta H_j)A(U_k)\) is paired with the birth \(\delta H_j\) whose quadratic curvature part it cancels.

The cancellation is scale-invariant: the old curvature scales by \(L^{-2}\) per argument and the density by \(L^4\) (the constant-flux calculation (24)). The pair is therefore marginal-free at every later scale. This is exactly the "matching Wilson subtraction" row of the AD §5.4 construction, which must be applied birth by birth ("bounding those two terms separately would leave an unsummable marginal expression"). In the self-consistent comparator, by contrast, the term \(t_kA\) has no partner birth.

## 2. Hypotheses

Each hypothesis concerns a single step \(k\), at an input admitted through \(k\).

**(F) Footing and identification.**

- **(F1)** Through every admitted step, the actual births satisfy \(\|E^{(j)}\|_j\le E_0\) (CMP119 Theorem 1, inductive assumptions (2.26)–(2.28), pp.259–262).
- **(F2)** The actual decrement \(c_{k+1}\) equals \(\mathcal P\) of the whole-lattice birth \(H_{k+1}[\mathcal I^{\rm act}_k]\), computed with \(g_k\) and data through step \(k\) only.
  - CMP119 p.278 says the interior terms of (3.47) "do not depend on \(\Lambda_{k+1}\), and coincide with the corresponding terms arising from the expressions defined on the whole lattice, i.e. in the framework of [I]". Page 279 subtracts \(\beta_{k+1}(g_k)A(\phi_{k+1},U_{k+1})\) from \(\mathbf E^{(k+1)}-\mathbf E^{(k+1)}(1)\).
  - The provisional-chart ordering and replay are the finite-cutoff construction §1 step 3 and the constant-flux calculation (23)–(24).
  - Hypotheses: source input for the source sentences; construction-level for the replay.

**(L1) Linear E-activity bound with current reserve.** For each \(k\) and each tuple \(F=(F_j)_{j\le k}\) of birth families (gauge invariant, whole-lattice covariant) with \(\sup_j\|F_j\|_j<\infty\):

- each \(\mathcal V^E_k(F)_Y\) extends holomorphically to \(\mathcal K^T_{k,Y}\);
- it vanishes at \(z=0\) for every fixed \((b,J,s)\);
- it satisfies
\[
\sup_{\mathcal K^T_{k,Y}}|\mathcal V^E_k(F)_Y|\le C_V\ell_k^{b_V}\Big(\sup_{j\le k}\|F_j\|_j\Big)e^{-\kappa_*d_k(Y)}.
\tag{P22.7}
\]

The support is Proposition 4.1 below. AD Theorem E14.3 (C-02, complete) gives (P22.7) on \(\mathcal K_{k,Y}\) for the actual activities with \(C_V\ell^{b_V}E_0=\mathfrak K_E\) (E14.50)–(E14.51), and \(b_V=0\).

**(L2) Cluster-expansion map.** There are \(b_*>0\), \(M_*<\infty\) and \(b_{\mathcal C}\ge0\), independent of \(k\), such that:

- \(\mathcal C_k\) is defined on \(\{\|V\|_{\mathfrak A_k}\le b_*\}\);
- its values are raw birth families at scale \(k+1\) on the native output domain, with decay \(\kappa\);
- for each \(X\) and each \((U,J)\), \(w\mapsto\mathcal C_k(V_0+wV_1)(X;U,J)\) is holomorphic wherever the line stays in the ball;
- \(\|\mathcal C_k(V)\|_{k+1}\le M_*\ell_k^{b_{\mathcal C}}\) on the ball.

Here "native output domain" means the union of the scale-\(k+1\) native domains for every \(g\) with \(|g/g_k-1|\le C/Y_k\). This covers both the provisional chart (\(g=g_k\)) and the actual chart (\(g=g_{k+1}\)). CMP119 p.262 says the new expressions are constructed "on slightly larger spaces, with the coefficients in their definition bigger by \(\beta\) multiplied by a corresponding number". A relative change \(O(1/Y_k)\) of the radii is far inside that enlargement.

Support: CMP116 §2. Bałaban's output bound is linear in the activity bound: Lemma 3, (2.38), \(|H(Z)|\le C_3\varepsilon_1e^{-(1-8\delta)\frac L2\kappa d_{k+1}(Z)}\), and (2.39)–(2.41). The constant \(C_3\) is proportional to the activity constant \(E_0\varepsilon_1C_1M^qe^{C_2\kappa_1}\). This holds under budget conditions that bound that constant by fixed numbers: (2.28) and \(\varepsilon_2\le1\) in (2.33). The expansion uses \(|\exp\sum\tau V|\le\exp\sum|\tau||V|\) (2.15) and fixed Cauchy circles (2.18), so complex activity data cause no new difficulty. The cutoff-defect contribution, \(\max\{\varepsilon_2,\exp(-\gamma_2\varepsilon_1^2/20g^2)\}\) in (2.33), is input-independent and bounded by \(e^{-cP_k^2}\). It is superpolynomially small and is absorbed into \(M_*\). CMP119 pp.276–278, (3.43)–(3.47), repeats this on the running chart with "\(B_0\) replaced by \(O(p_0^3(g_k))\)", so \(b_{\mathcal C}=3p_0\) is the conservative reading. Hypotheses: source input for the displayed bounds. The formulation for general admissible activity data within the budget is an additional assumption until written out (§9).

**(R) Mature R forcing.**
\[
\|\mathcal V^R_k(\mathcal R_k)\|_{\mathfrak A_k}\le 2C_R\ell_k^{b_R}g_k^{\kappa_0-11}.
\]
AE Theorem R14.3 (C-03, complete) gives \(\sup|\mathcal R_{k,Y}|\le C_Rg_k^{\kappa_0-11}e^{-\kappa_*d_k(Y)}\) on (RM.12) = \(\mathcal K_{k,Y}\). The factor 2 covers the fluctuation difference. The mature sub-sum inherits the bound because the proof sums nonnegative per-scale majorants (RM.9)–(RM.10). R14.3 needs \(\kappa_0\ge12\) with an arbitrary fixed choice (CMP119 p.260 after (2.31)). Hypotheses: source input for R14.3; the sub-sum remark is.

**(P) Readout.** For a birth family \(F\) at scale \(k+1\),
\[
|\mathcal PF|\le C_P\ell_k^{b_P}r_{k+1}^{-2}\|F\|_{k+1}.
\]
Support: AD §5.4, table, row "Matching Wilson subtraction": \(|\beta_j|\le CE_0r_j^{-2}\). That bound is linear in \(E_0\), since \(\beta\) is a second-order coefficient with a second spatial moment (CMP109 (1.20)–(1.22)). The flux version is the constant-flux calculation (9) and (25). Hypotheses: source input for AD at the stated scope.

**(C) Driven comparator.** Along any admitted actual prefix:

- **(C1)** the driven births are bounded, \(\|H'_j\|_j\le E_0'\), by restricting their fixed-chart bound to \(\mathcal U_j\);
- **(C2)** \(|p'_{k+1}-d_k^G|\le C_p/Y_k\), with \(C_p\) uniform.

Support: the constant-flux calculation §3 and (12)–(13), the pure-E fixed-chart induction with the CMP119 cutoff "requires no bound on its length". the finite-cutoff construction §2 proves the comparator decrement bound. Both are written for the self-consistent comparator with Wilson coefficient \(\widetilde Y_i=Y_i-t_i\) and gauge mismatch \(t_iG\). \(\mathfrak B'\) is the case \(t\equiv0\), with actual \(Y_i\). Hypotheses: construction-level (accepted at window scope in the finite-cutoff construction; depth uniformity argued in the native estimate §§14.8, 15.10).

**(G) Gaussian calibration.** \(|d^G_k|\le D_G\), \(|D_n^G-d_Bn|\le B_G\), and \(d_B=11N^2\log L/(12\pi^2)\) (the finite-cutoff construction §1; the constant-flux calculation §1; the coupling comparison). 

**(N) Numerical source inequalities.** The source constants \(\beta',\beta_0\) of CMP119 (2.6) satisfy \(\beta'\ge\frac54d_B+2B_G\). (2.7)–(2.9) follow from (2.6) as on CMP119 p.256. Lemma 3.4 shows (2.6) holds along any trajectory with the decrement bound of Theorem C.

**Parameter order.**

1. Fix the source constants (\(L,M,\kappa,\kappa_1,\beta,A_0,A_1,p_0,E_0,\ldots\)) and the constants in (L2), (P), (C), (G).
2. Fix an integer \(q>p_0\) with \((q-p_0)/2>b_V+b_{\mathcal C}\).
3. Fix \(\kappa_0\ge16\), so that \(C_R=C_R(\kappa_0)\).
4. Fix the ceiling \(Y_*\).

None of \(C_V,b_V,M_*,b_*,b_{\mathcal C},C_P,C_p\) depends on \(\kappa_0\). The parameter estimates found the same for its constants (the native estimate §12.4, §12.6).

## 3. Elementary lemmas (proved)

**Lemma 3.1 (Schwarz lemma on a polydisc).** Let \(f\) be holomorphic on \(\{z\in\mathbb C^n:\|z\|_\infty<R\}\), with \(|f|\le M\) and \(f(0)=0\). Then \(|f(z)|\le M\|z\|_\infty/R\).

*Proof.* Fix \(z\ne0\), put \(\rho=\|z\|_\infty<R\) and \(\varphi(\lambda)=f(\lambda z/\rho)\) for \(|\lambda|<R\). Then \(\varphi\) is holomorphic, \(|\varphi|\le M\) and \(\varphi(0)=0\). The one-variable Schwarz lemma on the disc of radius \(R\) gives \(|\varphi(\lambda)|\le M|\lambda|/R\). Take \(\lambda=\rho\). \(\square\)

**Lemma 3.2 (Lipschitz bound from a bounded holomorphic map).** Let \(\mathcal C\) satisfy (L2) at step \(k\), with \(M:=M_*\ell_k^{b_{\mathcal C}}\). Then for \(\|V\|,\|V'\|\le b_*/2\),
\[
\|\mathcal C(V)-\mathcal C(V')\|_{k+1}\le \frac{4M}{b_*}\|V-V'\|_{\mathfrak A_k}.
\]

*Proof.* Put \(\Delta=\|V-V'\|\). If \(\Delta\ge b_*/2\), the left side is at most \(2M\le 4M\Delta/b_*\). Otherwise fix \(X\) and \((U,J)\), and set
\[
f(w)=e^{\kappa d_{k+1}(X)}\big[\mathcal C(V'+w(V-V'))-\mathcal C(V')\big](X;U,J).
\]
For \(|w|<R:=b_*/(2\Delta)>1\), the line stays in the \(b_*\)-ball. So \(f\) is holomorphic there, \(|f|\le2M\) and \(f(0)=0\). Lemma 3.1 with \(n=1\) gives \(|f(1)|\le 2M/R=4M\Delta/b_*\). Take the supremum over \(X\) and \((U,J)\). \(\square\)

**Lemma 3.3 (max-recursion).** Let \(a_{k+1}\le\theta_kD_k+\Phi_k\), \(D_{k+1}=\max(D_k,a_{k+1})\), \(D_0=0\), with \(0\le\theta_k\le1/2\) and \(\Phi_k\ge0\). Then \(D_n\le 2\max_{k<n}\Phi_k\) for all \(n\).

*Proof.* Induction on \(n\). If \(D_k\le2\Phi_k\), then \(a_{k+1}\le\Phi_k+\Phi_k=2\Phi_k\). Otherwise \(a_{k+1}\le D_k/2+D_k/2=D_k\). So \(D_{k+1}\le\max(D_k,2\Phi_k)\). \(\square\)

**Lemma 3.4 (signed-prefix numerics).** Assume (G). Let \(Y_0,\dots,Y_n\) satisfy \(Y_i-Y_{i+1}=d_i^G+e_i\) with \(|e_i|\le d_B/4\) and \(Y_i\ge Y_*\ge 8B_G+4\). Then for \(m\le k\le n\):

- (a) \(Y_m-Y_k\le\big(\tfrac54d_B+2B_G\big)(k-m)\);
- (b) \(Y_m-Y_k\ge\tfrac34d_B(k-m)-2B_G\);
- (c) \(Y_m\ge Y_k-2B_G\ge Y_k/2\). Hence \(g_m\le(1+\beta_0)g_k\) as soon as \((1+\beta_0)^2\ge 1+4B_G/Y_*\);
- additional assumption for \(s>1\), \(\sum_{m\le k}Y_m^{-s}\le C_sY_k^{1-s}\) with \(C_s=2^s\big(1+\frac{2}{3d_B(s-1)}\big)\);
- (e) for \(h(x)=(\log x)^bx^{-\sigma}\) with \(\sigma>0\) and \(Y_*\ge 2e^{b/\sigma}\): \(\max_{m\le k}h(Y_m)\le 2^{\sigma}h(Y_k)\).

*Proof.* \(Y_m-Y_k=\sum_{i=m}^{k-1}(d_i^G+e_i)=d_B(k-m)+(b_k-b_m)+\sum e_i\), where \(b_i=D_i^G-d_Bi\) and \(|b_i|\le B_G\). This gives deduction and conditional, and (b) gives source input. The ratio statement is \(Y_k\le(1+\beta_0)^2Y_m\).

The ratio follows from \(Y_k/Y_m\le Y_k/(Y_k-2B_G)\le1+4B_G/Y_k\).

For additional assumption, conditional and \(Y_k\ge4B_G\) give \(Y_m\ge Y_k/2+\frac34d_B(k-m)\). Compare the sum with \(Y_k^{-s}2^s+\int_0^\infty(Y_k/2+\frac34d_Bx)^{-s}dx\) and use \(Y_k\ge1\).

For (e), \(h\) is decreasing on \([e^{b/\sigma},\infty)\). By source input, every \(Y_m\ge Y_k/2\ge e^{b/\sigma}\), so \(h(Y_m)\le h(Y_k/2)\le2^\sigma h(Y_k)\), using \(\log(Y_k/2)\le\log Y_k\). \(\square\)

Lemma 3.4(a) is the first inequality of CMP119 (2.6), \(Y_m\le Y_k+\beta'(k-m)\), under (N). Lemma 3.4(c) is the second. A numerical check of (a)–(d) is in §10.

## 4. One step: actual versus driven comparator

### 4.1 Proposition 4.1 (the current reserve in (L1))

*Claim.* Choose the ceiling so that, in addition to the AD conditions, \(\ell_k^{(q-p_0)/2}\) exceeds the fixed constants listed below and \(Cg_k\ell_k^{(q+p_0)/2}\le c_0\). Then the conclusion of AD Theorem E14.3, namely joint holomorphy and (E14.51) with the same \(\mathfrak K_E\), holds on the enlarged contour \(\mathcal K^T_{k,Y}\). This is the contour obtained from the choice \(e_{1,k}=2T_k\delta_k\) in place of (E14.21).

*Verification (conditional).* In AD the current radius enters only through \(e_{1,k}\), equivalently the ball \(\|z\|<2P_k\). Each displayed occurrence was located and checked:

| AD location | Condition at \(e_{1,k}=2\delta_k\) | Condition at \(e_{1,k}=2T_k\delta_k\) |
|---|---|---|
| (E14.8): \(e_1\le\min\{\varepsilon_{\rm abs},e_3/(2C_B),\alpha_2/(32C_\zeta KC_B)\}\); hence (E14.9)–(E14.11) with \(T_*\ge2\) | (E14.22)–(E14.24): \(\ell_k^{q-p_0}\ge 64C_\zeta KC_BA_1/c\), and \(Cg\ell^{p_0}\le c_0\) | \(\ell_k^{(q-p_0)/2}\ge64C_\zeta KC_BA_1/c\), and \(Cg\ell^{(q+p_0)/2}\le c_0\) |
| (E14.24e)–(E14.24f), nearby coarse input | \(\ell_k^{q-p_0}\ge8DA_1C_{\rm AF}/(c_3C_0)\) | \(\ell_k^{(q-p_0)/2}\ge8DA_1C_{\rm AF}/(c_3C_0)\) |
| (E14.33)–(E14.34), far carriers | factor \(\ell_k^{p_0-q}\sqrt{1+a}L^{-a}e^{-cML^a}\) | factor \(\ell_k^{(p_0-q)/2}\sqrt{1+a}L^{-a}e^{-cML^a}\le\sqrt{1+a}L^{-a}e^{-cML^a}\); (E14.35) unchanged |
| (E14.42)–(E14.44), far insertion path | \(2D_{\rm av}\delta_k\le\rho_{\rm map}/2\), and \(\ell^{q-p_0}\ge24D_{\rm far}A_1C_{\rm AF}/(c_2C_0)\) | \(2D_{\rm av}T_k\delta_k\le\rho_{\rm map}/2\), and \(\ell^{(q-p_0)/2}\ge24D_{\rm far}A_1C_{\rm AF}/(c_2C_0)\) |
| §5.4 construction, (E14.36)–(E14.38): \(Q_k\le c_Q\alpha_{0,k}\) bounds background plus prepared insertion | the insertion is at most \(\alpha_2/8\) by (E14.10) | unchanged; (E14.10) follows from the first row |
| §5.2 real centres (E14.26)–(E14.32); §5.6 background/current (E14.45)–(E14.48) | independent of \(z\) | unchanged |

Every condition involving the current radius has one of the two forms recorded in AD before (E14.49): a lower bound on a power of \(\ell_k^{q-p_0}\), or \(Cg_k\ell_k^b\le c_0\). Both survive the substitution after lowering the ceiling. The constant \(\mathfrak K_E\) of (E14.50) contains no current radius. The far-term factor only improves on the original contour.

**Vanishing at \(z=0\).** Each localized term in CMP116 (1.10) and (1.23) is a Cauchy coefficient, in \(t_\square\) and the decoupling parameters \(s\), of \(\mathbf E(\square_0,(t\zeta_\square+t_\square\zeta_\square)\mathbf H_k(s,B'))\). At \(B'=0\) the insertion vanishes identically in \(s\):

- \(|D(H,A')|\le4C_2|A'|^2\) by (1.14);
- \(|\mathbf A_0(s,H_0B')|\le4C_4(\cdots)|B'|^2\) by (1.16);
- hence \(\mathbf H_k(s,0)=0\) by (1.17)–(1.18);
- \(B'=g_kCB-h\tilde D(g_kCB)\) vanishes at \(B=0\) by (1.19)–(1.20).

These equations are on CMP116 pp.4–6. The argument of \(\mathbf E\) is therefore constant in \(t_\square\) and \(s\) at \(z=0\), and every such coefficient vanishes. The \(\mathcal PF_j\cdot A\) terms of the input enter as fluctuation differences of the same kind.

**Linear families.** AD uses the activity only through its native bound (linear: "applies with \(E_0\) → current bound"), the linear Ward identities, the matching subtraction by its own projection, and covariance. All other inputs concern maps and geometry. The statement-level analysis in Appendix A below tabulates this. AD's proof paragraph after Theorem E14.3 and §5.4 contain no other activity-dependent input. Gauge invariance and covariance pass to the differences \(\delta H_j\). The own-projection subtraction is linear.

*What is not done.* The proofs underlying AD (CMP109 §§3–4 and CMP116 §1 via AD §§3–5) were assumed symbol by symbol. If AD contains a use of \(e_1=2\delta_k\) that is not displayed, (L1) must be rechecked there.

**Consequence.** By Lemma 3.1 on the \(z\)-polydisc of radius \(2T_kP_k\), with \((b,J,s)\) fixed, and by (P22.7),
\[
\|\mathcal V^E_k(F)\|_{\mathfrak A_k}\le C_V\ell_k^{b_V}\rho_k\sup_{j\le k}\|F_j\|_j,\qquad \rho_k:=T_k^{-1}=\ell_k^{-(q-p_0)/2}.
\tag{P22.8}
\]

### 4.2 Theorem A (one-step Lipschitz bound)

*Statement.* Assume (F1), (L1), (L2), (R) and (C1) at step \(k\). Assume also the smallness condition
\[
C_V\ell_k^{b_V}\rho_k\max(E_0,E'_0)+2C_R\ell_k^{b_R}g_k^{\kappa_0-11}\le b_*/2.
\tag{P22.9}
\]
Then
\[
\|\delta H_{k+1}\|_{k+1}\le\theta_kD_k+\Phi_k,\qquad
\theta_k=\frac{4M_*C_V}{b_*}\ell_k^{\,b_{\mathcal C}+b_V-(q-p_0)/2},\qquad
\Phi_k=\frac{8M_*C_R}{b_*}\ell_k^{\,b_{\mathcal C}+b_R}g_k^{\kappa_0-11}.
\]

*Proof.*

1. By (P22.3)–(P22.5), \(\delta H_{k+1}=\mathcal C_k(V^{\rm act})-\mathcal C_k(V')\). Here \(V^{\rm act}=\mathcal V^E_k((E^{(j)})_j)+\mathcal V^R_k(\mathcal R_k)\) and \(V'=\mathcal V^E_k((H'_j)_j)\). The \(\mathcal G_k\) terms are identical because \(Y_k\), \(P_k\), the background and the maps are identical.
2. By (F1), (C1), (P22.8), (R) and (P22.9), both activities lie in the \(b_*/2\)-ball.
3. By linearity, \(V^{\rm act}-V'=\mathcal V^E_k((\delta H_j)_j)+\mathcal V^R_k(\mathcal R_k)\). The \(\delta H_j\) are birth families, as differences of birth families on the common domain \(\mathcal U_j\). So (P22.8) and (R) give \(\|V^{\rm act}-V'\|\le C_V\ell^{b_V}\rho_kD_k+2C_R\ell^{b_R}g_k^{\kappa_0-11}\).
4. Lemma 3.2 completes the proof. \(\square\)

The estimate compares the two genuine single-step integrals. The only interpolation is along a complex line *in the activity variable inside one step*. No synthetic multi-step trajectory, no synthetic coupling array and no compensating Wilson term at intermediate parameters is involved. Contrast this with (6) of [Reset remainders](../coupling/reset_remainders.md).

## 5. Theorem B (all-depth control of the reset-induced birth changes)

*Statement.* Assume the hypotheses of Theorem A at every step \(k\le n\). Assume \(\theta_k\le1/2\) for \(k\le n\); this holds once \(\ell_k^{(q-p_0)/2-b_{\mathcal C}-b_V}\ge8M_*C_V/b_*\). Assume the prefix satisfies Lemma 3.4. Then, with \(\sigma=(\kappa_0-11)/2\) and \(b=b_{\mathcal C}+b_R\),
\[
\sup_{j\le n+1}\|E^{(j)}-H'_j\|_j\le 2\max_{k\le n}\Phi_k\le\frac{16M_*C_R}{b_*}\,2^{\sigma}\,\ell_n^{\,b}\,g_n^{\kappa_0-11}.
\tag{P22.10}
\]
The constant depends only on the fixed constants and \(\kappa_0\). It is independent of the depth \(n\), the torus, the number, ages and grids of the absorbed resets, and the history.

*Proof.* Theorem A gives \(a_{k+1}:=\|\delta H_{k+1}\|\le\theta_kD_k+\Phi_k\). Lemma 3.3 gives the first inequality. \(\Phi_k\) is a constant times \(h(Y_k)\) with \(h(x)=(\log x)^bx^{-\sigma}\). Lemma 3.4(e) gives the second inequality, after enlarging \(Y_*\). \(\square\)

**Interpretation.** \(\delta H_j\) is exactly the change that all resets before \(j\) have made to the \(j\)-th regular birth, through every transport path, including the induced births of induced births. It is measured in the native norm on the native domain \(\mathcal U_j\), which is the domain in which the next step uses it. Old births are fixed functions once born (CMP109 (0.22)–(0.24); CMP119 (2.25)). Their later influence passes only through new births, and each new birth sees all old ones through the age-summed linear map \(\mathcal V^E_k\). Hence a scalar max-recursion suffices. No age kernel, resolvent tail or renewal mass condition is needed. This is the part of the finite-cutoff construction open problem that Theorems A–B address.

## 6. Theorem C (the coupling decrement at every admitted step)

*Statement.* Assume (F), (L1), (L2), (R), (P), (C), (G), (N), with the parameter order of §2 and \(\kappa_0\ge16\). There is \(Y_*\) such that, for every bare \(Y_0\ge2Y_*\) and every admitted step \(n<K\), where \(K\) is the first index with \(Y_K<Y_*\),
\[
|c_{n+1}-d_n^G|\le\frac{C_*}{Y_n},\qquad C_*:=C_p+1.
\tag{P22.11}
\]
Moreover every step before \(K\) satisfies the numerical source conditions (2.6)–(2.9), so the induction admits it.

*Proof.* Induction on \(n\) for the statement \(\mathsf S(n)\): steps \(0,\dots,n\) are admitted and (P22.11) holds for all \(k<n\). \(\mathsf S(0)\) is the bare density.

1. **Prefix.** By \(\mathsf S(n)\) and \(Y_*\ge4C_*/d_B\), \(|c_{k+1}-d_k^G|\le d_B/4\) for \(k<n\). Lemma 3.4 applies to \(Y_0,\dots,Y_n\), and with (N) gives (2.6)–(2.9) through \(n\).
2. **Births.** By (F1) the actual births through \(n\) are in the \(E_0\)-ball. By (C1) the driven births through \(n\) are in the \(E_0'\)-ball. Both are computed from \(Y_0,\dots,Y_n\) only.
3. **Next decrement.** By (F2), \(c_{n+1}=\mathcal PH_{n+1}[\mathcal I^{\rm act}_n]\), computed with \(g_n\) on the provisional output chart (the finite-cutoff construction §1). Then \(c_{n+1}-d_n^G=(p'_{n+1}-d_n^G)+\mathcal P\delta H_{n+1}\). By (C2) the first term is at most \(C_p/Y_n\).
4. **Readout of the difference.** By (P), Theorems A–B and Lemma 3.3,
\[
|\mathcal P\delta H_{n+1}|\le C_P\ell_n^{b_P}r_{n+1}^{-2}\big(\theta_nD_n+\Phi_n\big)
\le C_P\ell_n^{b_P}r_{n+1}^{-2}\cdot 2^{\sigma+1}\Phi_n.
\]
The readout is taken on the provisional chart (\(g=g_n\)), where \(c_{n+1}\) is computed and (L2) controls \(\delta H_{n+1}\). There \(r_{n+1}^{-2}=(c_rC_0)^{-2}Y_n\ell_n^{-2q}\). Hence
\[
|\mathcal P\delta H_{n+1}|\le K_\sharp\,\ell_n^{\,b_P+b_{\mathcal C}+b_R-2q}\,Y_n^{\,1-(\kappa_0-11)/2}\le K_\sharp\ell_n^{\,b'}Y_n^{-3/2},
\]
for \(\kappa_0\ge16\) and \(K_\sharp=K_\sharp(\kappa_0)\). Enlarging \(Y_*\) makes this at most \(1/Y_n\), which proves (P22.11) at \(n\).
5. **Admission.** (P22.11) and \(|d_n^G|\le D_G\) give \(|c_{n+1}|\le D_G+1\). The extended prefix satisfies Lemma 3.4 and hence (2.6)–(2.9) through \(n+1\), using (N). By the replay in (F2), the source admits step \(n+1\) as long as \(Y_{n+1}\ge Y_*\). This is \(\mathsf S(n+1)\).

The smallness (P22.9) and \(\theta_k\le1/2\) hold for \(Y_k\ge Y_*\), since \(\rho_k\to0\), \(g_k\to0\), and the logarithmic powers are dominated by the parameter order. \(\square\)

## 7. Corollary D (the UV recurrence; the completion-test items)

Put \(b_i=D_i^G-d_Bi\), \(y_i=Y_i+b_i\) and \(e_i=c_{i+1}-d_i^G\). Then exactly
\[
y_i-y_{i+1}=d_B+e_i.
\tag{P22.12}
\]
Let \(u_i=1/y_i\), and in ultraviolet order \(v_m:=u_{K-1-m}\), \(m=0,1,\dots,K-1\). Both endpoints of every step used below are then admitted, with \(Y\ge Y_*\).

*Statement.* Under Theorem C, with \(Y_*\ge\max(8B_G+4,\,4C_*/d_B,\,4C_*)\),
\[
v_{m+1}=v_m-d_B\,v_m^2+r_m,\qquad |r_m|\le A\,v_m^3,\qquad A=2C_*+(d_B+1)^2,\qquad 0\le m<K-1.
\tag{P22.13}
\]
The coefficient \(d_B=11N^2\log L/(12\pi^2)>0\) is in Bałaban's \(Y=g^{-2}\) units (normalized-trace, once-counted plaquette; the comparison argument coefficient paragraph). Equivalently it is \(11N/(24\pi^2)\) per step in \(g_{\rm std}^{-2}\), with \(Y=2N/g_{\rm std}^2\). The sequence \(v_m\) decreases toward the UV. The remainder \(r_m\) depends on the entire actual history through \(c_{K-1-m}\), including every reset and its transport. \(A\) is uniform in depth, volume and history.

*Proof.*

1. From (P22.12), \(u_i=u_{i+1}/(1+u_{i+1}(d_B+e_i))\), so \(v_{m+1}=v_m/(1+x_m)\) with \(x_m=v_m(d_B+\varepsilon_m)\) and \(\varepsilon_m=e_{K-2-m}\).
2. Since \(y\ge Y-B_G\ge Y/2\) for \(Y\ge 2B_G\), Theorem C gives \(|\varepsilon_m|\le C_*/Y\le 2C_*v_{m+1}\). Because \(|\varepsilon_m|\le d_B/4\), \(x_m>0\), so \(v_{m+1}<v_m\) and \(|\varepsilon_m|\le2C_*v_m\).
3. Expanding, \(v/(1+x)=v-vx+vx^2/(1+x)\). So \(r_m=-\varepsilon_mv_m^2+v_m^3(d_B+\varepsilon_m)^2/(1+x_m)\).
4. Hence \(|r_m|\le2C_*v_m^3+v_m^3(d_B+2C_*v_m)^2\le A v_m^3\), using \(2C_*v_m\le1\). \(\square\)

B-04 (Annex S) applies pathwise to (P22.13).

**Completion-test checklist, conditional on §2:**

- **Dictionary.** \(b=d_B\); \(u=1/y\), \(y=Y+D^G_i-d_Bi\), a bounded deterministic correction of the Wilson coordinate.
- **Sign.** \(d_B>0\).
- **History dependence.** Retained in \(r_m\).
- **Uniform remainder.** \(A=2C_*+(d_B+1)^2\).
- **Actual map.** The estimate controls the actual recursion, including all transported reset effects (Theorem B). It is not a frozen derivative.

## Appendix A. Statement-level inputs of AD §§5.1–5.6

This appendix records the statement-level check behind the paragraph **Linear families** of §4.1. The λ-family is the deformation of the activities on a finite admitted history in which the actual couplings \(Y_i\) and counterterms \(c_iA\), the selectors and the maps are frozen. Every displayed inequality in AD §§5.1–5.6 that involves an activity, and every proof step marked "actual", is listed below.

| Location | Input | Type | Status in the λ-family |
|---|---|---|---|
| (E14.24c), §5.1 | α_{0,k}/α_{0,j} ≤ C_AF√(1+a) | coupling sequence | identical: couplings are frozen |
| (E14.26)–(E14.27) | real-center regularity ≤ C′_reg ε_j | configuration support / selectors | identical: selectors are frozen |
| (E14.24d)–(E14.24e), (E14.40)–(E14.44) | insertion maps, minimizer derivative (CMP102 (190)) | maps and background only | identical |
| (E14.33)–(E14.34) | far-term bound C E_0 … | linear in E_0 | applies with E_0 → current bound |
| §5.4 table, (E14.36)–(E14.38) | near terms C E_0 r_j^{−r} …; Ward identities "linear identities in these coefficients" | linear in E_0 | applies |
| §5.4 table, last row | marginal F² cancelled against the same β_j | exact normal-form identity | holds in normal form; the difference is the mismatch m_k, handled by (C-M) |
| (E14.45)–(E14.48) | background/current transfer | maps only | identical |
| (E14.50)–(E14.51) | 𝔎_E = C_src E_0(1+S_near+S_far) | linear in E_0 | applies |

Here (C-M) is the admissibility of a small coupling mismatch \(m_kA\), modeled on §2 of [The Wilson trajectory on intervals admitting mature resets](../coupling/finite_window.md); it remains a stated condition. No other exact identity of the actual trajectory occurs. The input (C-E), that is, E14.3 for the λ-family, is therefore checked at statement level. The displayed derivations are not re-derived symbol by symbol.
