# Noneligible components and the sum over births

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

**Propagation hypothesis.** Any use of a T-step bound on a holed ancestor requires the conditional single-ancestor estimate and, for connected products, a separate collective crossing estimate. An argument from the diameter of the union of paid components alone is invalid.

## 1. Non-eligible components

Terminology. Following LFR I p.177, a component of the large-field region \(\Lambda_k^c\) is **eligible** if it satisfies (i) "it is contained in a cube of the size \(100MR_k\)" and (ii) "in the preceding \(N\) renormalization steps no new large field regions were created inside this component, and the previous regions contained in it satisfy the condition (i) on the corresponding scales". It is **non-eligible** otherwise. "Tag" means a retained (second-class) eligible component of an earlier R step whose raw multiplier or kernel has not yet been consumed ([U17] AU "active tags").

### 1.1 What the source does with them

**N1 (LFR I p.177, source).** After defining the class of eligible components: "Let us denote the union of the above class of components by \(Z\). […] Thus we write the factorization property (2.19) [III], \(\mathbf T_k(Z_k)=\mathbf T_k(Z_k\cap Z^c)\mathbf T_k(Z)=\mathbf T_k(Z_k\cap Z^c)\prod_i\mathbf T_k(X_i)\) (1.1) […] **In this section we do not make any changes in the operation \(\mathbf T_k(Z_k\cap Z^c)\), therefore we will usually omit it in the formulas.**"

**N2 (LFR II p.391, source).** The final representation reads
\[
\mathbf R\rho_k=\sum_{Z_k}\sum_{\{Y_1,\dots,Y_m\}}\chi_k\Bigl(\sum_{\{\Omega'_j,Z_j\}}\mathbf T''_k(Z_k)\Bigr)\prod_{i=1}^m\chi^c_k(Y_i^{\sim-6})\chi_{k,\Lambda_i}\delta_{G_i}(V_kV_{\Lambda_i}^{-1})(\mathbf T'_k(Y_i)1)\cdot\exp\Bigl[A'_k+\sum\mathbf R'^{(k)}(X)+\sum\mathbf B'^{(k)}(X)\Bigr]\quad(1.104).
\]
The operations \(\mathbf T''_k(Z_k)\) on the remaining large-field region, which contains the non-eligible components, remain **integration operations** acting on the whole expression.

**N3 (LFR II p.384, source).** The source controls the persistence of a large-field component \(Z\) created at scale \(j\) by its own large-field factor: "The factor \(\exp(-\kappa_j(Z))\) controls \(K\) renormalization steps, under the assumption that no large fields are created in these steps, where the number \(K\) is the smallest positive integer having the property that the domain \(S^K(Z)\), considered as a domain in the lattice of the scale \(L^{-(j+K)}\), satisfies the conditions (i), (ii), with \(N=R_j\). More precisely this means that \(\kappa_j(Z)\ge\sum_{n=j+1}^{j+K}O(1)M^dR_n^{d+1}d'_n(S^{n-j}(Z))\) (1.80)." On pp.384–385: \(d'_n(Z^{(n-j)})\le L^{-\frac12(n-j)}d'_j(Z)\), and once \(S^{n_0+1-j}(Z)\) lies in a cube of size \(64MR_{n_0+1}\) it "satisfies the condition (i), and doing at most \(R_j\) further steps we obtain a domain satisfying both conditions (i), (ii)". So a non-eligible component of initial linear size \(D\) stays non-eligible for at most \(O(\log D)+R_j\) steps (the inference is additional assumption), and the age of the structures inside it is bounded in the same way.

**Reading (c+d).** The source never integrates the variables of a non-eligible component. It never exponentiates around one, and it never needs a logarithm of its integral. It bounds the whole density by positivity, using (1.79), and lets the large-field factor pay for the number of steps until the component becomes eligible. Only then do the R operation and its preparations act. [Boundary estimate c] §4.3 item 2 asked which case holds: **retained, not integrated**.

### 1.2 What the conditional law does with them (source input; construction text)

- [U17] Annex AW §1, statement of AB17.1: "Surviving earlier fluctuation variables, retained raw component fields, current-scale exterior variables, selectors and history labels are retained." And: "The symbol \(\xi\) denotes the admitted native external coordinates; **old real variables and selectors remain fixed parameters**."
- [U17] Annex AS §4: "This section applies the response argument to the **unreplaced** operations of CMP119 (2.21)." Their coefficient dependence on the current enters only through the exact log-ratio \(\Theta(z,a;v)=\log w(z,a;v)/w(0,a;v)\) (OR17.1) at **fixed** \(a\).
- [U17] Annex AT §8: "contracting **all** of an arbitrarily large unreplaced component would lose too much spatial information. A stronger bookkeeping choice keeps the particular bounded components that have actually been integrated, or are being used as bounded over-carriers. Call these the active tags." Annex AU: "It does not collapse an arbitrary, possibly enormous, unreplaced large-field component into a free atom."
- Manuscript Annex W §2.3 (2.6)–(2.7): \(\mathcal T_k\) factorizes over components and contains the old integrations, which stay in the outer law (§3.2, paragraph after (3.11)).

So for C-05, the internal variables of non-eligible components are **conditioning data** (premise **(Frz)**, source-consistent). That includes the raw large-field links, the retained fluctuations \(a_j\) in \(Z_{j+1}\cap\Omega_{j+1}\), and the raw multipliers \(\mathbf T'_b(Y)1\) of older tags inside them.

### 1.3 The bounds of the activities that touch them

**N4 ([III] p.261, source).** \(\mathbf B^{(j)}(U_k,A,\{S_i\})=\sum_X\mathbf B^{(j)}(X,U_k,A,\{S_i\cap X\})\) (2.41), "where the sum is over domains \(X\in\mathbf D_j\) such, that \(X\cap\Omega_j\ne\emptyset\), and \(X\cap Z_j^\sim\ne\emptyset\). The localized term […] (i) it depends on \(U_k,A\) restricted to \(X\); […] (iv) it satisfies the bound \(|\mathbf B^{(j)}(X,(\mathbf U,\mathbf J),A,\{S_i\cap X\})|<B_0\exp(-\kappa d_j(X))\) (2.42)."

**N5 ([III] p.262, source).** "There are other possible forms of the inductive assumptions for the boundary terms. For example, we may resum all the terms with localization domains intersecting a given component of the large field region. […] we obtain the bound (2.42) with \(d_j(X)\) replaced by \(d_j(X\setminus Z_j)\). All constructions and proofs of the procedure can be carried on with these inductive assumptions. **We have chosen the ones above, because they agree with the assumptions for E-terms and R-terms.**"

**N6 (LFR II p.372, source).** At the R step, for the incoming terms re-expressed around the new backgrounds: "This resummation is almost exactly the same as the one discussed in Sect. 6 [I], it is controlled by […] the bounds (2.42) [III] for **B**-terms. In effect, for a given \(Y_0\) we obtain a term which is small, and satisfies the exponential bound (2.42) [III] in \(d_k(Y_0)\)." Here \(Z\) is the eligible union (N1). The contracted size (1.67), \(d_{k,Z}(Y)\), visits "all \(M\)-cubes of the components of \(Y\setminus Z\)" (p.376, source, quoted in [Boundary estimate c] Q3), so non-eligible parts of \(Y\) are charged. The R-output bound (1.99) contracts only the second-class \(Y_i\subset Z\) (p.390, source, per [Boundary estimate c]).

**N7 ([III] p.276, source).** At a T step: "The expression determined by the boundary terms \(\mathbf B_k\) is much simpler to deal with. To its terms we apply the formulas (3.6), (3.7) [I], and next we localize the obtained expressions. The localized expansion is over domains \(Y_0\in\mathbf D_k\) having nonempty intersections with \(\Lambda_{k+1}\)." The localization expansion of [I§6] (6.9)–(6.10) (source, CMP116 pp.4–5) is a sum "over connected domains \(Y_0\) containing \(\square^4\)", where \(\square^4\supseteq X\). Its terms are obtained by Cauchy estimates in the decoupling parameters \(s(\Delta)\), \(|s(\Delta)|\le e^{\kappa_1}\), for the new cubes \(\Delta\subset Y_0\setminus\square^4\). So new domains **contain** the old ones and the new cubes are **charged**. This is the carrier half of (Mon) for T steps; [Boundary estimate c] listed it as unchecked. That the old factor \(e^{-\kappa d_j(X)}\) is carried unchanged into the new term is additional assumption from the structure of the expansion. This remains an assumption.

**Conclusion (c+d).** In the source's main line, every activity that touches a non-eligible component is bounded in a size that charges every cube of its carrier except those inside **eligible** components (tags, or the current eligible union at an R step). Denote this premise:

> **(FT) Full-tree charging of non-eligible regions.** Every record in the current representation has a carrier \(X\) and a set \(H\) of declared holes. Each declared hole is a tag (an eligible component of its birth step, diameter \(\le100MR_b\) in birth units). The record's weight charges every cube of \(X\setminus\cup H\), in the record's own birth units, and in particular every cube of \(X\) lying in a non-eligible component.

(FT) is source input for R steps (N6). For T steps it is (source input; source) for the carriers (N7) and additional assumption for the weights. It is also the declared bookkeeping (§1.2, AT §8).

### 1.4 No two-attachment mechanism for frozen components

**Lemma NE.1.** Let \(\{V_e(z;\eta)\}_{e\in\mathcal E}\) be a finite family of functions holomorphic in \(z\in D_P\), depending on a parameter \(\eta\) (the frozen data), and let \(B(z;\eta)=\sum_eV_e(z;\eta)\). Then for every \(i,l\)
\[
\partial_i\partial_lB=\sum_e\partial_i\partial_lV_e.
\]
In particular, if each \(V_e\) obeys (Loc) of [Hidden components] (C.5) with the full carrier \(X_e\) (graded distance to \(\cup X_e\)), then
\[
|\partial_i\partial_lV_e(z)|\le\frac{2w_e}{P^2}e^{-\nu\max\{d_g(x_i,\cup X_e),d_g(x_l,\cup X_e)\}}\qquad(z\in D_{P/2}),
\]
and the weighted row \(\sum_le^{\chi|x_i-x_l|_\infty}|\partial_i\partial_lV_e|\) is bounded by \([Hidden components]\) Theorem C, Steps 1–3, with the record's own carrier. No quantity attached to a non-eligible component other than the cubes of \(X_e\) enters.

*Proof.* Linearity, then [Hidden components] Theorem C Step 1 (Cauchy on the polydisc of radius \(P/2\)). \(\square\)

**Why this is the whole point.** The two-attachment example of [Rep21] (R29) is \(F=\log\Pi e^{V_x+V_y}\) with a **kernel** \(\Pi\) integrating a common variable \(\sigma\). Its mixed derivative \(F_{xy}=g^2\) is a covariance under \(\Pi\), a product of two attachments. Without the integration, \(\log e^{V_x+V_y}=V_x+V_y\) and \(\partial_x\partial_y(V_x+V_y)=0\). By §1.1–1.2, the variables of non-eligible components are never integrated in the current law, so their contribution to C-05 is linear in the records.

### 1.5 Theorem NE conditional

**Setting.** That of [Hidden components] §4.1: grades \(g\), metrics \(d_g\), \(d^{(b)}\), (Geo) with constants \(\gamma,C_0\) for \(c=\nu/4\), and current sites \(x_i\) of grade \(K\) with density \(n_I\). Let \(\mathcal R^{\rm NE}\) be the family of records that touch a non-eligible component and contain no declared hole, i.e. the records with \(H=\emptyset\), together with the records of the ordinary inherited sector. Each \(\rho\) has birth \(b\), a carrier \(E_\rho\) of \(\mathcal G_b\)-cubes, an anchor cube meeting \(\overline{\{g\le b\}}\), and the bound \(w_\rho\le W_be^{-\kappa_*\delta_b(E_\rho)}\), at most \(m_0\) per \((b,E)\). Its derivatives obey (Loc) (C.5) **uniformly in the frozen data \(\eta\)**.

**Theorem NE.** Assume (Frz), (FT), (Loc) uniformly in \(\eta\), (Geo), and \(\kappa_*-\nu/2-1\ge\kappa_{\rm cnt}(d)\) ([Hidden components] Lemma A4 constant). Then for \(m\ge1\), \(z\in D_{P/2}\) and every \(i_1\),
\[
\sum_{\rho\in\mathcal R^{\rm NE}}\sum_{i_2,\dots,i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}|\partial_{i_1}\cdots\partial_{i_m}F_\rho(z)|\le\frac{C_aC_b^{m-1}((m-1)!)^{d+1}}{P^m}\,C_{\rm cnt}m_0\sum_{b\le K}\Gamma_bW_b ,
\]
with the constants of [Hidden components] (C.11). The constants and the right side do not depend on the number, diameters, shapes, ages or positions of the non-eligible components, on the volume, or on the depth \(K\).

*Proof.* (FT) puts each such record in the format of [Hidden components] §4.1 with \(E_\rho=X_\rho\) (no holes), and (Frz) makes \(F_\rho\) a function of \(z\) alone at fixed \(\eta\). Lemma NE.1 shows the current dependence is the sum of the \(F_\rho\). [Hidden components] Theorem C applies. Its rooted norm is \(\mathcal A_b(\nu/2+1)\le C_{\rm cnt}m_0W_b\) by Lemma A4/Prop. B2 with \(H=\emptyset\). \(\square\)

**Remarks.**
1. Theorem C uses (Geo) to pay the multiplicity \(L^{d(K-b)}\) of fine anchors. Structures inside a non-eligible component can be old (N3: up to \(O(\log D)+R\) steps), and Theorem C handles every age, since \(\sum_b\Gamma_bW_b\) is summable when \(W_b\) is subexponential in \(K-b\). No age-dependent premise beyond that enters.
2. Nothing here uses a collar. Current sites in fact lie at least eight \(LMR_{k+1}\)-layers from \(Z_k\) ([Boundary estimate c] §5), so a record touching a non-eligible component has an extra factor \(e^{-c\nu LR_{k+1}}\). That is a gain is not needed.
3. **Uniformity in the frozen data.** (Loc) must hold uniformly over the admissible values of the frozen large-field variables. The source's bounds (2.42) are sup bounds over the analyticity space \(\widetilde U^c_j(X,\dots)\) in \((\mathbf U,\mathbf J)\) at fixed real large-field variables \(A\) in their admissible set (N4). So the sup bound is uniform. The **first-derivative** form is the P2′ (Annexes AO–AR) and is not re-derived here. It is the same premise as for every other record.

### 1.6 Why (FT) is necessary, and why it is free

**Necessity.** Suppose a record \(e\) attached to a non-eligible component \(N\) of diameter \(D_N\) (in current \(M\)-units) were carried in the resummed form of N5, with exterior \(F_e\) a single cube touching \(N\) and (Loc′) with carrier \(F_e\cup N\). Let \(x_i,x_l\) be current sites at the minimal distance \(8LR_{k+1}\) from \(N\), at opposite ends of it. If (Loc′) is saturated, \(|\partial_i\partial_lV_e|\asymp w_e e^{-16\nu LR_{k+1}}/P^2\) while \(|x_i-x_l|\ge D_N\), so the weighted row is \(\gtrsim w_ee^{\chi D_N-16\nu LR_{k+1}}\). Since \(D_N\) is unbounded and the margin is fixed (no proportional collar exists for \(N\): [Boundary estimate c] §4.3 item 2), the completion test would fail. This is [Boundary estimate b] Remark 3 to Theorem C′ with \(\theta\to0\).

**Lemma NE.2 (un-resummation).** Let \(V=\sum_{X\in\mathcal S}V_X\) be a resummed record in the sense of N5: \(\mathcal S\) is the set of carriers \(X\) meeting a component \(N\), and each \(V_X\) is a full-tree record with (Loc) on \(X\) and weight \(w_X\le W e^{-\kappa\delta(X)}\). Then the family \(\{V_X\}_{X\in\mathcal S}\) has the same sum, and Theorem NE applies to it. The resummed bound is never needed for derivative estimates.

*Proof.* Linearity (Lemma NE.1). \(\square\)

The resummed form is a choice of bookkeeping. The only way a record can be **intrinsically** non-local across \(N\), i.e. not a sum of full-tree records, is that it is produced by integrating variables of \(N\) together with two attachments. By §1.1–1.2 that never happens while \(N\) is non-eligible. So (FT) costs nothing, provided the representation keeps the unresummed family for non-eligible components, as AT §8 already does.

### 1.7 Tags inside non-eligible components: the collar persists (deduction; given the margin)

A tag \(Q\) born at \(b\) may later lie inside a non-eligible component \(N_j\) of \(Z_j\), \(j>b\). Under Route A ([Boundary estimate c] §3) its kernel is still unintegrated, and records born at later scales may depend on its variables. [Boundary estimate c] §4.3 item 1 proposed to attach such records to the "shadow" of \(Q\), the component of \(Z_j\) containing it. **That would make \(N_j\) a hole**, the case §1.6 shows to be fatal. It is also unnecessary. By (FT) such a record is full-tree outside \(Q\) itself, so its hole is \(Q\), with the record's own birth grid.

What has to be checked is the collar of \(Q\) as seen in the coarser units of a later birth.

**Lemma NE.3 (collar of a tag in every later birth metric).** Let \(Q\) be a tag born at \(b\), with \(\Delta_Q=\operatorname{diam}_\infty(\cup Q)\). Let \(U_Q=\{y:\operatorname{dist}_\infty(y,\cup Q)<\theta\Delta_Q\}\). Assume (i) \(U_Q\cap\{x_i\}=\emptyset\), and (ii) \(g\le b\) on \(U_Q\setminus\cup Q\). Then for every \(j\in\{b,\dots,K\}\) and every current site,
\[
d^{(j)}(x_i,\cup Q)\ \ge\ \theta\,\frac{\Delta_Q}{s_j}=:\theta D_Q^{(j)},\qquad s_j=Mh_j.
\tag{Col\(_j\)}
\]
*Proof.* A path from \(x_i\notin U_Q\) to \(\cup Q\) has a sub-arc inside \(\overline{U_Q}\setminus\cup Q\) of Euclidean length \(\ge\theta\Delta_Q\) (it must cross from sup-distance \(\theta\Delta_Q\) to sup-distance \(0\), and the Euclidean length dominates the sup-norm displacement). On that arc \(g\le b\le j\), so the capped unit \(M\max(h_g,h_j)\) equals \(Mh_j=s_j\). Hence the capped length is \(\ge\theta\Delta_Q/s_j\). \(\square\)

**Source support for (i)–(ii)** (c for the margin, additional assumption for the identification). [Boundary estimate c] §5 ([III] p.265): \(\Omega_{b+1}^c\supseteq Z'^{\sim8}_b\), a margin of eight \(LMR_{b+1}\)-layers around \(Z_b\). With \(\Delta_Q\le100MR_bh_b\) (condition (i)) and \(R_b\le(L+1)R_{b+1}\), the margin has width \(\ge\theta\Delta_Q\) with \(\theta=8L/(101(L+1))\). It lies in \(\Omega_{b+1}^c\), where the grade is \(\le b\), giving (ii). Current sites lie in \(\Lambda_K\subset\Omega_K\subset\Omega_{b+1}\), giving (i). The grade on the margin does not change later, for three reasons:
- T steps do not change the old \(\Omega_n\).
- R steps change grades only inside an eligible component.
- An eligible component meeting the margin contains \(Q\), since the margin lies in \(\Omega_{b+1}^c\subset Z_j\) and is connected to \(Q\), and an R component is a whole component of \(Z_j\). In that case \(Q\) is promoted ([U17] AT §8.1) and replaced by a new tag with its own margin.

A non-eligible component containing \(Q\) changes nothing on the margin. **So tags swallowed by non-eligible components keep (Col\(_j\)) at every later birth \(j\), with the same \(\theta\).**

### 1.8 Interface with H-02 additional assumption

- C-05 gives current-coordinate derivative bounds **conditional on** the geometry, including all non-eligible components, and uniform in it (Theorem NE, Theorem R6). It gives **no** decay in the size of a non-eligible component and needs none.
- The suppression of geometries containing non-eligible or unreplaced components is a value or probability statement. The source's mechanism is (1.79)–(1.80) (N3): the factor \(e^{-\kappa_j(Z)}\) pays \(\sum_nO(1)M^dR_n^{d+1}d'_n(S^{n-j}(Z))\) over the \(K\) steps until the component becomes eligible. This belongs to H-02 (per-event inequality) and to the outer-law normalization, not to C-05.
- The one point where the two meet is the conditional normalizer of the current law. Its **logarithmic derivatives** in the current are C-05's. Its **value** grows with the volume of the geometry and is not bounded by C-05. H-02 must not use C-05 as a value bound for ratios of normalizers.
- N3 also gives the age bound \(O(\log D)+R_j\) for structures inside a non-eligible component. H-02 may want it. C-05 does not need it (Remark 1 to Theorem NE).

## 2. Route A summed over births: Theorem R6

[Boundary estimate c] Theorem R1 recentres each normalized kernel and Prop. R3 bounds the increment load of a kernel whose attached records all have the kernel's own birth. At later steps, records of later births \(j>b\) attach to an older tag (§1.7). Their decay is measured in the coarser capped metric \(d^{(j)}\le d^{(b)}\), so they cannot be treated as birth-\(b\) records. [Boundary estimate c] §4.3 item 1 left this open ("This estimate remains a hypothesis"). The theorem below closes it for the single-kernel sector, i.e. the interactions \(\mathcal E_1(v)\). The idea is to sum the covariance terms through the **records** rather than through the kernels, so that the multiplicity of old tags is paid by each record's own anchor.

### 2.1 Lemma H (Hessian of a recentred kernel logarithm)

In the setting of [Boundary estimate c] Theorem R1, let \(t_v\le\frac14\), \(G_v(z)=\mu'_v(e^{\tau_v(z,\cdot)})\) and \(\Pi'_{v,z}\) as there. For \(z\in D_{P/2}\):
\[
\partial_i\partial_l\log G_v=\Pi'_{v,z}(\partial_i\partial_l\tau_v)+\Pi'_{v,z}(\partial_i\tau_v\,\partial_l\tau_v)-\Pi'_{v,z}(\partial_i\tau_v)\,\Pi'_{v,z}(\partial_l\tau_v),
\]
\[
|\partial_i\partial_l\log G_v(z)|\le e^{3t_v}\sup_\omega|\partial_i\partial_l\tau_v(z,\omega)|+2e^{6t_v}\sup_\omega|\partial_i\tau_v(z,\omega)|\,\sup_\omega|\partial_l\tau_v(z,\omega)|.
\]
*Proof.* Differentiate \(\partial_l\log G_v=\Pi'(\partial_l\tau_v)=G_v^{-1}\mu'(e^{\tau_v}\partial_l\tau_v)\) once more (differentiation under the integral is justified by Cauchy bounds on compact subsets of \(D_P\), as in R1(4)). The bound uses \(|\Pi'(f)|\le e^{3t}\sup|f|\) (R1(2)) twice. \(\square\)

**Remark (mass cancellation, a).** Write the kernel at the current step as \(\mathbf T'_v(z)=\lambda_ve^{\sigma_v(z,\cdot)}\mu_v\), with \(\lambda_v=\mathbf T'_v(0)1>0\) and \(\mu_v\) a probability. Then
\[
\mathbf T'_v(z)\,e^{S_v(z,\cdot)}=\lambda_ve^{c_v}G_v(z).
\]
So the **total** current dependence of the single-kernel factor, mass included, is \(\log G_v\). [Boundary estimate c] Cor. R5 uses \(\rho_v=\log G_v-\log N_v\), the normalized part. The mass \(\mathbf T'_v(z)1=\lambda_vN_v(z)\) contributes \(+\log N_v\). **construction hazard:** if the construction counts the mass response through an AX/OR17-type log-ratio \(\Theta\) and also uses \(\rho_v\), the two \(N_v\) terms must both be present. Using \(\log G_v\) directly avoids the issue. additional assumption: by LFR II p.392 (source), "These functions depend only on the new field variables \(V_k\) restricted to \(Y_i\)". This suggests that after the birth step the kernel does not depend on the later current at all, i.e. \(\sigma_v\equiv0\) and (Resp) holds with \(s_*=0\) at later steps. The argument assumes it for the native pair \((U,J)\) of (1.71).

### 2.2 Setting

That of [Hidden components] §4.1 and [Boundary estimate b] §2.1, with the following.
- **Kernels** \(v\in\mathcal V\). Each has a birth \(b_v\), a tag \(Q_v\) (finite set of \(\mathcal G_{b_v}\)-cubes in \(\overline{\{g\le b_v\}}\)) with \(\Delta_v=\operatorname{diam}_\infty(\cup Q_v)\), and an anchor cube \(c_v\in\mathcal G_{b_v}\) touching \(Q_v\) and meeting \(\overline{\{g\le b_v\}}\). At most \(m_1\) kernels share an anchor cube.
- **(Col\(_j\))** For all \(v\), all \(j\in\{b_v,\dots,K\}\) and all sites: \(d^{(j)}(x_i,\cup Q_v)\ge\theta\Delta_v/s_j\). (Lemma NE.3.)
- **Records.** \(\mathcal E_1=\bigsqcup_v\mathcal E_1(v)\). A record \(e\in\mathcal E_1(v)\) has a birth \(j_e\in\{b_v,\dots,K\}\) and an exterior \(F_e\ne\emptyset\) of \(\mathcal G_{j_e}\)-cubes not meeting \(\cup Q_v\)'s interior. One cube of \(F_e\) touches \(\cup Q_v\) and meets \(\overline{\{g\le j_e\}}\); this is the anchor. The carrier is \(X_e=\cup F_e\cup\cup Q_v\). The record has a function \(V_e(z,\omega_v)\) holomorphic in \(z\in D_P\), bounded measurable in \(\omega_v\), with
\[
\sup_{D_P\times\Omega_v}|\partial_iV_e|\le\frac{w_e}{P}e^{-\nu d_g(x_i,X_e)},\qquad w_e\le W_{j_e}e^{-\kappa_*\delta_{j_e}(F_e)}.
\tag{Loc′}
\]
- **(Resp)** \(\sup|\partial_i\sigma_v|\le\frac{s_*}{P}e^{-\nu d_g(x_i,\cup Q_v)}\).
- **Multiplicities.** (M1) At most \(m_0\) records of \(\mathcal E_1(v)\) per \((j,F)\). (M2) The global rooted norms are finite:
\[
\mathcal A'_j(\vartheta):=\sup_{q\in\mathcal G_j}\sum_{e:\,j_e=j,\ q\in F_e}w_ee^{\vartheta\delta_j(F_e)}\le\mathfrak a\,W_j\quad\text{for }\vartheta=\nu+1.
\]
- Put \(\Theta=1+1/\theta\), \(\Theta'=1+\sqrt d/\theta\), and \(\bar W=\sup_jW_j\).

(M2) is exactly the hypothesis that [Boundary estimate b] Theorem C′ needs for this family of records. By Prop. B2′ it holds with \(\mathfrak a=4m_0K_d^{3\cdot2^d}\) if \(\kappa_*-\nu-1\ge\kappa'_{\rm cnt}(d)\), **provided** the tags touching a common \(\mathcal G_j\)-cube satisfy (H-sep) in the grid \(\mathcal G_j\). See Remark 3 below for when that can fail.

### 2.3 Theorem R6

Assume §2.2, (Real) and (Pos) of [Boundary estimate c] R1 for every kernel, (Geo) with \(c=\nu/(8\Theta')\) and constants \(\gamma,C_0\), \(0\le\chi\le\nu/(4M\Theta)\), and \(\kappa_*\ge\nu+\kappa'_{\rm cnt}(d)\). Put
\[
\Lambda_*:=C_\Lambda\bigl(s_*+e^{C_0}\bar W\bigr),\qquad C_\Lambda=C(additional assumption; M,\nu,\theta,n_I,m_0,\gamma)\ \text{(explicit in the proof)},
\]
and assume \(\Lambda_*\le\frac14\). Then \(t_v\le\Lambda_*\le\frac14\) for every \(v\), every \(G_v\) is zero-free on \(D_P\), and for \(z\in D_{P/2}\):
\[
\sup_i\Bigl|\partial_i\sum_v\log G_v(z)\Bigr|\le\frac{C_1}{P}\,\mathfrak S,\qquad
\sup_i\sum_le^{\chi|x_i-x_l|_\infty}\Bigl|\partial_i\partial_l\sum_v\log G_v(z)\Bigr|\le\frac{C_2(1+\Lambda_*)}{P^2}\,\mathfrak S,
\]
\[
\mathfrak S:=\sum_{j\le K}\Gamma_j\bigl(\mathfrak a\,W_j+m_1s_*\bigr),
\]
with \(\Gamma_j\) as in [Hidden components] (C.9). The constants depend on \(d,L,M,\nu,n_I,\theta,m_0,m_1,\gamma,C_0\) only. In particular they do not depend on the volume, the depth \(K\), the number, ages, sizes or positions of the tags, or on non-eligible components.

*Proof.* Write \(a_v(i):=P\sup_{D_P\times\Omega_v}|\partial_i\tau_v|\le P\sup|\partial_i\sigma_v|+\sum_{e\in\mathcal E_1(v)}P\sup|\partial_iV_e|\). Fix \(v\), put \(Q=Q_v\), \(r_i=\operatorname{dist}_\infty(x_i,\cup Q)\), and for \(e\in\mathcal E_1(v)\) of birth \(j\) put \(d_e(i)=d_g(x_i,X_e)\) and \(\delta_e=\delta_j(F_e)\).

*Step 1 (geometry, as [Boundary estimate c] R3 Step 1 in the capped metric \(d^{(j)}\)).* \(d^{(j)}(x_i,\cup Q)\le d^{(j)}(x_i,X_e)+\delta_e+2\sqrt d\le d_e(i)+\delta_e+2\sqrt d\), since \(d^{(j)}\le d_g\). Also \(r_i\le Md^{(j)}(x_i,\cup Q)\) by (C.2), and \(\Delta_v\le(s_j/\theta)d^{(j)}(x_i,\cup Q)\le(M/\theta)d^{(j)}(x_i,\cup Q)\) by (Col\(_j\)). Hence
\[
r_i+\Delta_v\le M\Theta\,(d_e(i)+\delta_e+2\sqrt d).
\tag{2.1}
\]

*Step 2 (per-kernel load).* Define \(\Lambda_v:=\sum_la_v(l)e^{\chi r_l}\). For \(e\) of birth \(j\), by (2.1) with \(\chi M\le\nu/4\) and Step 1,
\[
w_ee^{-\nu d_e(l)}e^{\chi r_l}\le w_ee^{\frac\nu4(\delta_e+2\sqrt d)}e^{-\frac{3\nu}4d_e(l)}\le w_ee^{\nu(\delta_e+2\sqrt d)}e^{-\frac{3\nu}4d^{(j)}(x_l,\cup Q)}.
\]
The number of \(\mathcal G_j\)-cubes touching \(\cup Q\) is \(\le(D^{(j)}+3)^d\), with \(D^{(j)}=\Delta_v/s_j\). By Prop. B2′ at each such cube, with the hole fixed (so no hole entropy) and (M1), \(\sum_{e\in\mathcal E_1(v),\,j_e=j}w_ee^{\nu\delta_e}\le4m_0K_d^{3\cdot2^d}W_j(D^{(j)}+3)^d\), using \(\kappa_*-\nu\ge\kappa'_{\rm cnt}\). For the site sum, \(d^{(j)}(x_l,\cup Q)\ge\max\{\theta D^{(j)},\sum_{n=j+1}^{K-1}\omega_n\}\) by (Col\(_j\)) and [Hidden components] Lemma C1 (applicable because \(\cup Q\subset\overline{\{g\le j\}}\)). So
\[
e^{-\frac{3\nu}4d^{(j)}}\le e^{-\frac\nu4d^{(j)}}\,e^{-\frac\nu4\theta D^{(j)}}\,e^{-\frac\nu4\sum_{n=j+1}^{K-1}\omega_n}.
\]
As in [Hidden components] Theorem C Step 3, the sites with \(d^{(j)}(x_l,\cup Q)\le t\) lie in a cube of side \(\Delta_v+2Mt\le M(D^{(j)}+2t)\). Hence \(\sum_le^{-\frac\nu4d^{(j)}(x_l,\cup Q)}\le n_I(2M+1)^d(D^{(j)}+1+4d/\nu)^d\). (Geo) with \(c=\nu/(8\Theta')\le\nu/2\) gives \(\frac\nu4\sum_{n>j}\omega_n\ge\gamma(K-1-j)-C_0\). Collecting,
\[
\sum_{e\in\mathcal E_1(v)}\sum_lw_ee^{-\nu d_e(l)}e^{\chi r_l}\le\sum_{j=b_v}^{K}C_3W_je^{C_0}e^{-\gamma(K-1-j)}\le\frac{C_3e^{C_0}\bar W}{1-e^{-\gamma}},
\]
\[
C_3=4m_0K_d^{3\cdot2^d}e^{2\nu\sqrt d}n_I(2M+1)^d\sup_{D\ge0}(D+3)^d(D+1+4d/\nu)^de^{-\frac\nu4\theta D}<\infty.
\]
The \(\sigma_v\) term is treated in the same way, with \(j=b_v\) and no record sum: \(\sum_ls_*e^{-\nu d_g(x_l,\cup Q)}e^{\chi r_l}\le C_3's_*\). Hence \(\Lambda_v\le C_\Lambda(s_*+e^{C_0}\bar W)=\Lambda_*\), with \(C_\Lambda=\max\{C'_3,C_3/(1-e^{-\gamma})\}\). Integrating along the segment, \(|\tau_v(z)|\le\sum_l|z_l|\sup|\partial_l\tau_v|\le\sum_la_v(l)\le\Lambda_v\). So \(t_v\le\Lambda_*\le\frac14\), and [Boundary estimate c] Theorem R1 applies to every kernel.

*Step 3 (gradient).* By R1(4), \(|\partial_i\log G_v|\le e^{3/4}a_v(i)/P\). So \(\sum_v|\partial_i\log G_v|\le e^{3/4}P^{-1}\bigl[\sum_vP\sup|\partial_i\sigma_v|+\sum_{e\in\mathcal E_1}P\sup|\partial_iV_e|\bigr]\). The second sum is over **all** single-kernel records, each counted once. It is the \(m=1\) case of [Boundary estimate b] Theorem C′ for the family \(\{V_e\}\) with holes \(H_e=\{Q_v\}\). The hypotheses of C′ hold: (Col) in \(d_g\) follows from (Col\(_j\)) since \(d_g\ge d^{(j)}\) and \(D_Q\) in own units is \(D^{(j)}\); (Att) by construction; the anchor meets \(\overline{\{g\le j\}}\); and (M2) gives the rooted norm. The first sum is C′ for the "records" \(\sigma_v\), with exterior \(\{c_v\}\), weight \(s_*\) and multiplicity \(m_1\) per anchor. This gives the first inequality.

*Step 4 (Hessian row).* By Lemma H with \(t_v\le\frac14\),
\[
|\partial_i\partial_l\log G_v|\le e^{3/4}\Bigl(\sup|\partial_i\partial_l\sigma_v|+\sum_{e\in\mathcal E_1(v)}\sup_{D_{P/2}}|\partial_i\partial_lV_e|\Bigr)+\frac{2e^{3/2}}{P^2}a_v(i)a_v(l).
\]
(4a) The first group, summed over \(v\) and weighted by \(e^{\chi|x_i-x_l|}\), is the \(m=2\) case of Theorem C′ for the same two families (Step 3).

(4b) For the covariance term use \(|x_i-x_l|_\infty\le r_i+\Delta_v+r_l\):
\[
\sum_v\sum_le^{\chi|x_i-x_l|}a_v(i)a_v(l)\le\Bigl[\sup_v\Lambda_v\Bigr]\cdot\sum_va_v(i)e^{\chi(r_i+\Delta_v)}.
\]
For a record \(e\in\mathcal E_1(v)\), (2.1) and \(\chi M\Theta\le\nu/4\) give \(w_ee^{-\nu d_e(i)}e^{\chi(r_i+\Delta_v)}\le e^{\nu\sqrt d/2}\,(w_ee^{\frac\nu4\delta_e})\,e^{-\frac{3\nu}4d_e(i)}\). So \(\sum_va_v(i)e^{\chi(r_i+\Delta_v)}\) is bounded by the \(m=1\) case of Theorem C′ applied with rate \(3\nu/4\) to records with weights \(w_ee^{\nu\delta_e/4}\), plus the analogous \(\sigma_v\) sum. That is \(\le C\sum_j\Gamma_j(\mathcal A'_j(\nu+1)+m_1s_*)\le C\,\mathfrak S\), because the weight exponent needed by C′ is \(\frac\nu4+\frac{3\nu}8+1\le\nu+1\). (Geo) is used at \(c=3\nu/(16\Theta')\ge\nu/(8\Theta')\), and (C.4) at a larger \(c\) is implied by (C.4) at a smaller one. Hence the covariance contribution is \(\le2e^{3/2}C\Lambda_*\mathfrak S/P^2\). Adding (4a) gives the second inequality. \(\square\)

**Remarks.**
1. **What has been gained.** Under Route A, the kernels add to the root sums of the ordinary record sector only two things: the per-kernel load \(\Lambda_*\), which is bounded uniformly in tag size and age via the collar, and the covariance factor \((1+\Lambda_*)\). There is no component-load condition, no SC, no shadow holes, and no birth-by-birth summation of kernels.
2. **What has not.** Interactions touching two or more kernels (\(\mathcal E_2\)) still need [Boundary estimate c] Prop. R4 and the finite-cutoff construction theorem, with its weighted loads ([Boundary estimate c] §3.4 end). R6 does not touch them. Jets of order \(m\ge3\) of \(\sum_v\log G_v\) involve higher cumulants under \(\Pi'_v\). The same factorization (one record sum times powers of \(\Lambda_*\)) should work through the tree-graph formula for cumulants. It is an additional prerequisite.
3. **(M2) for later births near dense old tags.** A coarse \(\mathcal G_j\)-cube may touch many old tags of birth \(b\ll j\): tags are separated only by \(c\,s_{b}\) ([U17] (CR.5)). A single-kernel record attached to one of them has exterior cubes of grid \(j\). The global rooted norm (M2) then counts, at a fixed exterior \(F\), every tag that \(F\) touches. That number can be of order \(L^{d(j-b)}\) unless the records are represented in the **multiscale** localization domains \(\mathbf D_j\), whose cubes near old structures are of the old scale (N7, [III] p.276: "if \(\Delta\subset\Omega_j\setminus\Omega_{j+1}\), then the size of \(\Delta\) is equal to \(ML^j\eta\)"). In that representation the tags are separated in the local grid. The rooted count is then the multigrid version of Prop. B2′ (the "birth-scale gap"). **This is the same open item as for the ordinary sector.** R6 shows that Route A adds nothing to it. Treat it as premise **(M2)**.
