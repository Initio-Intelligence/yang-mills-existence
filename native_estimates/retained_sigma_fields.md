# Retained sigma-fields and conditional expectations

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

**Conditional coordinates.** Clause (2″) in [Retained coordinates](retained_coordinates.md) specifies all variables integrated, including the completed preparation stages and auxiliary gauge variables. On a relocated bond the log Jacobian is combined with the Haar density ratio.

## 3. The σ-fields, stated precisely

**Setting.** Fix a finite cutoff and an admitted geometry. Let \((\Omega,\mathfrak F,\mathbb P)\) be the positive path space of Annex W §4.1, built on the **main-line** representation (F1–F6). It is standard Borel, and every variable ever introduced (fine field, labels, gauge variables, fresh reference variables) is a coordinate. Order the elementary operations chronologically as sub-steps \(s=1,2,\dots\): each T step, each R step, each label exposure and each fresh sampling. Let \(\mathfrak F_s\) be the σ-field of all variables created up to and including sub-step \(s\). After sub-step \(s\), let:

- \(C_s\): the current field and the exposed labels, i.e. the data \((h,V)\) of Annex W (4.2);
- \(P_s\): every variable introduced by sub-step \(s\) that the main-line representation has **not yet integrated**. This includes S-a, S-c and S-d variables, the parts of stopped preparations that are not yet integrated, and fresh variables still present;
- \(T_s\subset P_s\): the hidden variables of second-class components (S-c and S-d).

Define
\[
\mathcal G^\star_s=\sigma(C_s,P_s),\qquad
\mathcal G^{B}_s=\sigma(C_s,P_s\setminus T_s),\qquad
\mathcal G^\alpha_s=\sigma(C_s),
\]
so that \(\mathcal G^\alpha_s\subset\mathcal G^B_s\subset\mathcal G^\star_s\). [Boundary estimate e]'s Fork A is \(\mathcal G^{A}_s=\sigma(C_s,P_s\setminus T^{\rm new}_s)\), where \(T^{\rm new}_s\) are the hidden variables of tags born at the R step immediately before the T step \(s\). So \(\mathcal G^B_s\subset\mathcal G^A_s\subset\mathcal G^\star_s\) at that T step, and \(\mathcal G^A_s=\mathcal G^\star_s\) at all other steps.

**The one-step law** at a T step \(s\) is the regular conditional law of the current free coordinates \(z_s\) given the chosen σ-field. Under ★ it is the law of \(z_s\) given \(\mathcal G^\star\), where \(\mathcal G^\star\) contains everything except \(z_s\). The **transport** of a mark is \(F_s=\mathbb E[F_{s-1}\mid\mathcal G_s]\), \(F_0=\Phi\).

**Premise (Mem\(^{\mathcal G}\)).** For every \(s\): (i) \(\mathcal G_{s+1}\subset\mathcal G_s\vee\sigma(\xi_{s+1})\), where \(\xi_{s+1}\) is the tuple of new auxiliary variables (labels, fresh fields, gauge variables) introduced at \(s+1\); and (ii) the conditional law of \(\xi_{s+1}\) given \(\mathfrak F_s\) is a function of the \(\mathcal G_s\)-data. In words: every partition of unity, reference kernel and gauge average used at the next sub-step is evaluated on retained data only.

- For \(\mathcal G^\star\), (i) holds by construction. Blocking is a function of the current field. New postponed variables are restrictions of the current field or fresh variables. Consumed variables leave the state. (ii) is the statement that the source applies every operation to an integrand that is a function of not-yet-integrated variables only ([III] (2.18), F1, F6). That is [RB]'s open item (M), restricted to what the source integrates. **source input; additional assumption**, to be checked on LFR II pp.365–379.
- For \(\mathcal G^B\), (ii) additionally requires that no later kernel uses tag hidden variables. This is plausible. The reference kernel uses the constrained filling \(V_\Lambda\), which LFR I Prop. 1 makes a function of raw data ([BI] l.294, assumed input). Preparations act on levels \(>h\) and leave the deep factor untouched ([C05U] l.3189, assumed input). **additional assumption**
- For \(\mathcal G^\alpha\), (ii) **fails** in the actual construction. The coarse-field selector \(P_{j+1}\) tests "the local minimizing background determined by the coarse field" ([MS] l.13880). That background is \(U_{\mathbf B}(V)\), which depends on postponed belts (F1). The preparatory R tests are tests on postponed old variables ([MS] l.13884; LFR I p.178 "we try to do a part of the integrations in the operations \(\mathbf T^{(j)}(Z_j)\)"). **source** for the inputs, **additional assumption** that the dependence is genuine.

## 4. Measure-theoretic relations (proved)

Throughout, \(\mathcal G\subset\mathcal G'\) are sub-σ-fields of a standard Borel probability space, and \(Z\) is a random variable in \(\mathbb R^I\).

**Lemma 4.1 (coarse law = mixture of fine laws).** Let \(\nu'(\cdot,dz)\) and \(\nu(\cdot,dz)\) be regular conditional laws of \(Z\) given \(\mathcal G'\) and \(\mathcal G\). Then \(\nu(\cdot,A)=\mathbb E[\nu'(\cdot,A)\mid\mathcal G]\) a.s. for every Borel \(A\). If \(\mathcal G'=\mathcal G\vee\sigma(\eta)\) and \(\nu'(dz)=p'(z;\eta)\,dz\), then \(\nu(dz)=p(z)\,dz\) with \(p(z)=\int p'(z;\eta)\,\kappa(d\eta)\), where \(\kappa=\mathbb P(\eta\in\cdot\mid\mathcal G)\).

*Proof.* For \(B\in\mathcal G\), \(\mathbb E[1_B1_{Z\in A}]=\mathbb E[1_B\,\mathbb E(1_{Z\in A}\mid\mathcal G')]=\mathbb E[1_B\nu'(A)]\). Conditioning \(\nu'\) on \(\mathcal G\) disintegrates over \(\kappa\). \(\square\)

**Proposition 4.2 (exact transport needs (Mem)).** Let \(\mathcal G_s\) satisfy (Mem). Then \(F_s:=\mathbb E[F_{s-1}\mid\mathcal G_s]\), \(F_0=\Phi\in L^1(\mathfrak F_0)\), satisfies \(F_s=\mathbb E[\Phi\mid\mathcal G_s]\) for all \(s\). Without (Mem) one still has \(\mathbb E F_s=\mathbb E\Phi\), but in general \(F_s\neq\mathbb E[\Phi\mid\mathcal G_s]\).

*Proof.* Induction. Since \(\xi_{s+1}\) is conditionally independent of \(\mathfrak F_s\) given \(\mathcal G_s\) by (Mem)(ii), and \(\Phi\in\mathfrak F_s\), we have \(\mathbb E[\Phi\mid\mathcal G_s\vee\sigma(\xi_{s+1})]=\mathbb E[\Phi\mid\mathcal G_s]\). Then (Mem)(i) and the tower property give \(\mathbb E[\Phi\mid\mathcal G_{s+1}]=\mathbb E\bigl[\mathbb E[\Phi\mid\mathcal G_s]\mid\mathcal G_{s+1}\bigr]\). The expectation identity is the law of total expectation. \(\square\)

**Example 4.3 (lift α is not a transport filtration).** Let \(X\in\{0,1\}\) be fair, postponed, and the only variable. Let \(\mathcal G^\alpha_s\) be trivial. Let the label at \(s+1\) be \(\xi=X\), exposed by the partition of unity \(1=\mathbf 1_{X=1}+\mathbf 1_{X=0}\), and \(\mathcal G^\alpha_{s+1}=\sigma(\xi)\). Take \(\Phi=X\). Then \(\mathbb E[\Phi\mid\mathcal G^\alpha_s]=\tfrac12\) and \(\mathbb E[\tfrac12\mid\mathcal G^\alpha_{s+1}]=\tfrac12\), but \(\mathbb E[\Phi\mid\mathcal G^\alpha_{s+1}]=X\). With \(\mathcal G^\star_s=\sigma(X)\), (Mem) holds and the chain is exact.

*Consequence (deduction; given §3).* α-marks \(\mathbb E[\Phi\mid C_s]\) are well-defined, as projections \(\mathbb E[F^\star_s\mid\mathcal G^\alpha_s]\). They cannot be propagated by α-steps alone. Annex I makes an α-type chain exact by resampling every postponed variable at every step (Theorem 2.1, Cor. 2.2). The price is a reset cumulant response at every step, which Annex I says "can be nonlocal" and which no proposition estimates.

**Proposition 4.4 (retain vs average-and-resample).** Let the future after sub-step \(s\) be generated from \((W,\eta)\) and new auxiliary variables by fixed kernels, where \(W\) is the \(\mathcal G^B\)-type data at \(s\) and \(\eta\) are tag variables. Draw \(\eta'\sim\mathbb P(\eta\in\cdot\mid W)\) independently, and generate the future from \((W,\eta')\) by the same kernels. Then the joint law of \((W,\eta',\text{future})\) equals that of \((W,\eta,\text{future})\). In particular, every subsequent conditional law given \(\sigma(W,\eta',\dots)\) has the same form as the one given \(\sigma(W,\eta,\dots)\).

*Proof.* \((W,\eta')\overset d=(W,\eta)\) by construction, and the future is the same measurable function of them and of independent noise. \(\square\)

*Application (conditional; given (Mem\(^\star\)) and [BI] §8).* At an R step, H-03's \(\pi_v\) conditions on \(v\supseteq(U_k,V_k,\text{Zbar data, Y geometry})\). Everything later depends on \((v,\eta_Y)\). So "average \(\eta_Y\) at birth and resample" (A1) and "retain \(\eta_Y\) from birth" (A2) give the same joint law and identical T-step laws. They differ only in the transported mark: A1 averages over \(\eta_Y\) at birth; A2 keeps the dependence until consumption.

**Proposition 4.5 (what transfers from fine \(\mathcal G'\) to coarse \(\mathcal G\)).** In the notation of Lemma 4.1:

1. **Event and label probabilities.** \(\mathbb P(E)\) does not depend on the conditioning, and \(\mathbb P(E\mid\mathcal G)=\mathbb E[\mathbb P(E\mid\mathcal G')\mid\mathcal G]\). Joint bounds of the H-02 form \(\mathbb P(\bigcap_iE_i)\le\prod a_i\) are statements about \(\mathbb P\) and are identical in every lift. Annex W (4.2) gives \(\mathbb P(H_k=h)=Z_{k,h}/\mathscr Z\) in every lift.
2. **Values and moments.** \(\mathbb E_\nu f=\mathbb E[\mathbb E_{\nu'}f\mid\mathcal G]\). Any bound of the form "\(\mathbb E_{\nu'}f\in K\) a.s." with \(K\) closed and convex (sup bounds, \(L^p\) moment bounds, regulator-relative bounds with a \(\mathcal G\)-measurable regulator) passes to \(\nu\).
3. **First derivatives at real points.** If \(p'(\cdot;\eta)>0\) is \(C^1\), then \(\partial_i\log p(z)=\int\partial_i\log p'(z;\eta)\,\kappa_z(d\eta)\) with \(\kappa_z\propto p'(z;\cdot)\kappa\). Hence \(|\partial_i\log p(z)|\le\sup_\eta|\partial_i\log p'(z;\eta)|\). This is the only sense in which "derivative bounds transfer by sup".
4. **Second derivatives.** \(\partial_i\partial_l\log p=\mathbb E_{\kappa_z}[\partial_i\partial_l\log p']+\operatorname{Cov}_{\kappa_z}(\partial_i\log p',\partial_l\log p')\). The covariance matrix is positive semidefinite, so (i) \(-D^2\log p\preceq\mathbb E_{\kappa_z}[-D^2\log p']\): **coercivity can only be lost**; and (ii) a weighted Hessian-row bound for \(p\) needs a row bound on the covariance. That is the two-attachment term of [Rep21] (R29) and [Boundary estimate d] §1.4, and it is not implied by row bounds for \(p'\). Counterexample to transfer of coercivity: \(p'(z;\eta)=\phi(z-\eta)\), \(\eta=\pm a\) with probability \(1/2\) each, gives \(-(\log p)''(0)=1-a^2<0\) for \(a>1\).
5. **Complex domains.** Zero-freeness of \(p'(\cdot;\eta)\) on a polydisc does not give zero-freeness of \(p\). [Boundary estimate e] Example N2 (checked there) exhibits a zero for kernels of uniformly small variation. Cauchy-type derivative bounds for \(\log p\) on complex polydiscs therefore do not transfer.
6. **Cumulants.** By the law of total cumulance, \(\kappa_\nu(f_1,\dots,f_r)=\sum_\pi\kappa_{\mathcal G}\bigl(\kappa_{\nu'}(f_B)_{B\in\pi}\bigr)\). Spatial decay of the \(\nu'\)-cumulants gives nothing for the \(\pi\neq\{\text{one block}\}\) terms, i.e. for the outer cumulants of conditional means.
7. **Retained-coordinate differences** (Annex Y (M.4)). For a \(\mathcal G\)-coordinate \(y\), \(\delta_y\mathbb E[F\mid\mathcal G]=\mathbb E[\delta_yF\mid\mathcal G]+(\text{score term from the change of }\kappa\text{ in }y)\), cf. [BI] BL (J\(^{\rm new}\)). Difference bounds do not transfer by sup unless \(\kappa\) does not depend on \(y\).
8. **Coarse → fine.** Nothing transfers in general: \(\nu'\) can be singular with respect to \(\nu\).

*Proof.* 1–2: Lemma 4.1 and Jensen. 3–4: differentiate \(\log\int p'\kappa\) under the integral. 5: the cited example. 6: the standard partition formula for conditional cumulants. 7: product rule for the quotient \(\int F\,p'\,d\kappa/\int p'\,d\kappa\). 8: take \(\eta=Z\). \(\square\)

**Proposition 4.6 (pinning preserves a Dobrushin condition) (a abstract; b for H-03).** Let a finite specification on coordinates \(I\) have total-variation influence coefficients \(c_{ij}\) on admissible pairs, with \(\sup_ia_i^{-1}\sum_jc_{ij}a_je^{\theta d(i,j)}\le\varepsilon<1\). For \(J\subset I\) and an admissible pinned value on \(J\), the conditional law on \(I\setminus J\) has the same single-site conditionals. Its influence matrix is \(c|_{(I\setminus J)^2}\), whose weighted row sums are at most \(\varepsilon\).

*Proof.* Single-site conditionals given all other coordinates do not change when some of those coordinates are additionally fixed. Restricting a nonnegative matrix reduces row sums. \(\square\)

*Application conditional.* The proofs of HS20.3–HS20.4 use (HS20.13), (HS20.16) and (HS20.20). (HS20.13) holds for every admissible outside configuration, including fixed Y states. The proof of HS20.3 already "Condition[s] on the J coordinates" ([BI] l.546). So HS20.3–HS20.4 hold for \(\pi_v(\cdot\mid\eta_Y)\), the law needed in variant A2, with the same constants. The posterior disintegration and the corresponding closure-bound properties are required as inputs.
