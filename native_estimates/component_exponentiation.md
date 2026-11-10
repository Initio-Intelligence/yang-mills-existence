# Exponentiation around retained components

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

## 2. SC: where it is and is not needed

Notation: cubes are scale-\(k\) \(M\)-cubes; \(\delta(F)=\delta_M(F)\) is the visiting size of [Hidden components] (1.1); \(K_d=4\cdot9^d\), \(\kappa'_{\rm cnt}(d)=2^{d+1}\log K_d+\log2\) as in [Boundary estimate b] Prop. B2′; \(N_{\rm att}(Q)\) is the number of cubes not in \(Q\) that touch \(Q\).

### 2.1 Proposition (the main exponentiation converges under (W)) (deduction; given (1.90), (1.97))

Let the polymer representation (1.90) hold. Write \({\rm act}(X')\) for the activity of a polymer \(X'\) and \(E(X')=X'\setminus\bigcup Y_i\ne\emptyset\) for its exterior (a set of cubes). Assume a polymer is determined by its exterior and the set of retained components it contains, and two polymers are compatible when no cube of one exterior equals or touches a cube of the other. Assume the retained components are at index distance \(\ge3\) from each other, every \(Y_i\subset X'\) touches a cube of \(E(X')\), and
\[
|{\rm act}(X')|\le c_1e^{-a\,\delta(E(X'))},\qquad a\ge\kappa'_{\rm cnt}(d)+2^{d+1}a_0,\qquad 3^d\cdot4c_1e^{a_0 2^d}K_d^{3\cdot2^d}\le a_0.
\]
Then the Kotecký–Preiss condition holds with the weight \(a(X')=a_0\,\#E(X')\), so \(\log\{\cdots\}\) has a convergent cluster expansion, uniformly in the sizes of the \(Y_i\).

*Proof.* A polymer incompatible with \(X'_0\) has an exterior cube within index distance 1 of one of the \(\#E(X'_0)\) exterior cubes of \(X'_0\). So it suffices that for every cube \(q\), \(\sum_{X':q\in E(X')}|{\rm act}(X')|e^{a_0\#E(X')}\le a_0/3^d\). By [Hidden components] Lemma A3, \(\#E\le2^d(2\delta(E)+1)\), so \(e^{a_0\#E}\le e^{a_02^d}e^{2^{d+1}a_0\delta(E)}\). The pairs (exterior, set of contained components) with \(q\) in the exterior are among the pairs \((F,H)\) of [Boundary estimate b] Prop. B2′, and that proposition gives \(\sum\le4c_1e^{a_02^d}K_d^{3\cdot2^d}\). \(\square\)

With (1.97), \(a=(1+\beta)\kappa\) and \(c_1\in\{\alpha^{1/3},e^{-p_0(g_k)}\}\), the hypotheses hold for \(\kappa\) large and \(\alpha\) small. (1.97) is stated with \(d_{k,\cup Y_i}(X')\ge\delta(E(X'))\); under (W) one reads \(E(X')\) as the paid exterior and the same derivation (1.92)–(1.96) applies, because (1.93)–(1.96) use (1.68) only through the tree and volume of the cubes that \(d_{k,Z'}\) visits. The first-class components inside \(X'\) are charged in \(d_{k,\cup Y_i}\) and compensated by \(e^{-p_0}\), as on p.389. The proof assumes (1.92)–(1.96) in full; the statement about them is source input; additional assumption.

**Consequence.** LFR II Theorem 1, in the representation (1.72)+(1.98)+(1.101)+(1.102), does not depend on the shell reading. SC is not a gap in it.

### 2.2 What the final remark needs

In (1.103) with ordinary connectedness, all polymers containing \(Y_i\) are pairwise incompatible. Consider the sub-gas of polymers that contain \(Y_i\) and no other retained component. Its partition function is \(1+\sum_{X'\supset Y_i}{\rm act}(X')\), and the cluster series for its logarithm is \(\sum_{n\ge1}\frac{(-1)^{n-1}}n(\sum{\rm act})^n\). As a series in the activities it converges absolutely if and only if
\[
\Sigma_i:=\sum_{X'\supset Y_i}|{\rm act}(X')|<1.
\tag{2.1}
\]
(The Kotecký–Preiss condition would need \(\Sigma_i\le1/e\), [Boundary estimate b] §4.) So (2.1) is necessary for the argument on p.391, not only sufficient.

### 2.3 What the printed bounds give for \(\Sigma_i\)

Under (W) the printed bound for the activities is \(|{\rm act}(X')|\le e^{3n(X')}c_0e^{-(1+\beta/4)\kappa\delta(F(X'))}\), \(c_0=(O(1)c_1)^{1/3}\), \(c_1=\alpha^{1/3}\), where \(F(X')\) is the paid exterior and \(n(X')\) is the number of retained components in \(X'\). The exterior may be a single cube touching \(Y_i\), at any of the \(N_{\rm att}(Y_i)\) positions. By [Boundary estimate b] Lemma 4.1 (= the source's (1.94)) the bound for \(\Sigma_i\) is \(C\alpha^{1/9}N_{\rm att}(Y_i)\), and nothing in the printed bounds prevents the terms at different positions from each having size comparable to \(\alpha^{1/9}e^{-c\kappa}\). \(N_{\rm att}(Y_i)\ge2d(20R_k)^{d-1}\) (Q12). By Q13 this is unbounded while \(\alpha\) is fixed.

**Conclusion (conditional).** With the bounds that the construction supplies, the sentence "This bound is enough for the convergence of the exponentiated cluster expansion" on p.391 is not justified. It is justified under the literal reading of p.377 (every polymer containing \(Y_i\) contains and pays for the shell, so \(\Sigma_i\le Ce^{-c\kappa R_k^{d-1}}\)), which Conjecturally, is what the displayed estimate requires, and which the construction does not deliver. **SC is a real gap in the final remark (1.103)–(1.104), and only there.**

### 2.4 Is the gap real, or only unproved?

The total interaction between a retained component and its surroundings is a genuine surface term of size \(\asymp N_{\rm att}\). What decides whether \(\log\langle e^{\sum_e B_e}\rangle\) under the normalized \(\mathbf T'_k(Y_i)\) splits into local terms with uniformly small norms is how much of each \(B_e\) *depends on the integrated variables*. If a fixed fraction did, the \(n\)-th cumulant of \(n\) terms at \(n\) arbitrary surface positions would not be small after summing the positions, and (1.104) with uniformly bounded local terms would be false. By Q11–Q12 the integrated variables sit at distance \(\ge10R_k-5\) cubes from the surface, so Conjecturally, the dependence to be \(O(e^{-cR_k})\) (§3.5). So the resulting statement is: **the final remark is very probably true, by a mechanism the source does not state, and its printed justification is incomplete.**

## 3. Repairs

Three results, in decreasing order of what they assume about the source.

- §3.1–3.4 (Route A): no exponentiation at birth; the kernels are kept and recentred at the current step. Needs positivity at real fields and the collar. All proofs complete.
- §3.5 (Route B): the final remark itself, under the new premise (Osc).
- §3.6: a modification of the source's last resummation (thicker collar) which makes the printed argument of the final remark valid. Combinatorial part proved; analytic consequences not examined.

### 3.1 Theorem R1 (recentring of normalized positive kernels)

**Setting.** \(I\) is a finite set (current coordinates), \(D\subset\mathbb C^I\) a polydisc centred at \(0\). \(\mathcal V\) is a finite set (components). For \(v\in\mathcal V\): a measurable space \(\Omega_v\) with a **probability measure** \(\mu_v\); a bounded jointly measurable \(\sigma_v:D\times\Omega_v\to\mathbb C\), holomorphic in \(z\), with \(\sigma_v(0,\cdot)=0\). The kernel is
\[
\Pi_{v,z}A=\frac{\mu_v(e^{\sigma_v(z,\cdot)}A)}{N_v(z)},\qquad N_v(z)=\mu_v(e^{\sigma_v(z,\cdot)}).
\]
\(\mathcal E\) is a finite set of interactions; \(e\in\mathcal E\) has a nonempty \(I_e\subset\mathcal V\) and a bounded measurable \(V_e:D\times\prod_{v\in I_e}\Omega_v\to\mathbb C\), holomorphic in \(z\). \(\mathcal E_1(v)=\{e:I_e=\{v\}\}\), \(\mathcal E_2=\{e:|I_e|\ge2\}\). Put
\[
Z(z)=\Bigl(\bigotimes_v\Pi_{v,z}\Bigr)\exp\sum_{e\in\mathcal E}V_e(z,\cdot),\qquad S_v(z,\omega_v)=\sum_{e\in\mathcal E_1(v)}V_e(z,\omega_v).
\]

**(Real)** \(S_v(0,\omega_v)\in\mathbb R\) for all \(v,\omega_v\).

Define \(c_v=\log\mu_v(e^{S_v(0,\cdot)})\in\mathbb R\), the probability measure \(\mu'_v=e^{S_v(0,\cdot)-c_v}\mu_v\), and
\[
\tau_v(z,\omega_v)=\sigma_v(z,\omega_v)+S_v(z,\omega_v)-S_v(0,\omega_v),\quad t_v=\sup_{D\times\Omega_v}|\tau_v|,\quad s_v=\sup_{D\times\Omega_v}|\sigma_v|,
\]
\[
G_v(z)=\mu'_v(e^{\tau_v(z,\cdot)}),\qquad \Pi'_{v,z}A=\frac{\mu'_v(e^{\tau_v(z,\cdot)}A)}{G_v(z)}.
\]

**Theorem R1.** Assume (Real) and \(t_v\le\frac14\), \(s_v\le\frac14\) for all \(v\). Then on \(D\):

1. \(|G_v-1|\le e^{t_v}-1\), \(|N_v-1|\le e^{s_v}-1\); \(G_v,N_v\) are zero-free, and \(|\log G_v|\le2t_v\), \(|\log N_v|\le2s_v\).
2. \(\Pi'_{v,z}\) is a normalized kernel (\(\Pi'_{v,z}1=1\)), holomorphic in \(z\), and for every \(J\subset\mathcal V\) and bounded \(A\): \(\bigl|\bigl(\bigotimes_{v\in J}\Pi'_{v,z}\bigr)A\bigr|\le e^{3\sum_{v\in J}t_v}\sup|A|\).
3. **Identity.**
\[
Z(z)=\prod_v\frac{e^{c_v}G_v(z)}{N_v(z)}\cdot Z_2(z),\qquad Z_2(z)=\Bigl(\bigotimes_v\Pi'_{v,z}\Bigr)\exp\sum_{e\in\mathcal E_2}V_e(z,\cdot).
\]
4. \(\partial_i\log G_v(z)=\Pi'_{v,z}(\partial_i\tau_v(z,\cdot))\), hence \(|\partial_i\log G_v(z)|\le e^{3t_v}\sup_{\omega}|\partial_i\tau_v(z,\omega)|\); likewise \(|\partial_i\log N_v(z)|\le e^{3s_v}\sup_\omega|\partial_i\sigma_v(z,\omega)|\).
5. \(G_v(0)=N_v(0)=1\). If \(\mathcal E_2=\emptyset\), then \(Z\) is zero-free on \(D\), \(Z(0)=e^{\sum_vc_v}\), and \(\log Z(z)-\log Z(0)=\sum_v(\log G_v-\log N_v)(z)\).

*Proof.* (1) \(\mu'_v\) is a probability measure, so \(|G_v-1|=|\mu'_v(e^{\tau_v}-1)|\le e^{t_v}-1\le e^{1/4}-1<0.285\). The function \(f(t)=-\log(2-e^t)\) is convex with \(f(0)=0\) and \(f(\frac14)<0.335\), so \(f(t)\le1.34\,t\) on \([0,\frac14]\). Same for \(N_v\).

(2) \(\Pi'_{v,z}\) is integration against the complex measure \(e^{\tau_v}\mu'_v/G_v\), of total variation \(\le e^{t_v}/(2-e^{t_v})\). The function \(h(t)=e^{2t}(2-e^t)\) has \(h(0)=1\) and \(h'(t)=e^{2t}(4-3e^t)>0\) for \(t<\log\frac43\), so \(e^{t}/(2-e^{t})\le e^{3t}\) on \([0,\frac14]\). Total variation is multiplicative for product measures. Holomorphy: the integrands are holomorphic in \(z\) and uniformly bounded.

(3) \(Z(z)=\int\prod_v\frac{\mu_v(d\omega_v)e^{\sigma_v}}{N_v}\,e^{\sum_vS_v(z,\omega_v)}e^{\sum_{\mathcal E_2}V_e}\), and \(\mu_v(d\omega_v)e^{\sigma_v+S_v(z)}=e^{c_v}\mu'_v(d\omega_v)e^{\tau_v}=e^{c_v}G_v\cdot\frac{\mu'_v(d\omega_v)e^{\tau_v}}{G_v}\).

(4) Differentiate under the integral (Cauchy bounds for \(\tau_v\) on compact subsets of \(D\)) and use (2). (5) follows from (3) and (1). \(\square\)

**Remarks.**

1. The component-incidence load \(\sum_{e\in\mathcal E_1(v)}\sup|V_e|\) does not appear. It is hidden in the real constant \(c_v\) and in the tilt \(\mu_v\to\mu'_v\), neither of which costs anything because \(\mu_v\ge0\). What must be small is \(t_v\), the total *increment* \(\sup|S_v(z)-S_v(0)|\) plus the kernel response.
2. \(c_v\) is independent of \(z\) but depends on the retained data. It belongs to \(H(\xi)\) in (R8) of the corresponding construction repair. Its size is \(\le\sum_{e\in\mathcal E_1(v)}\sup|V_e(0)|\), i.e. of order \(WN_{\rm att}\).
3. If (Real) fails by a bounded amount, replace \(S_v(0)\) by \(\operatorname{Re}S_v(0)\) in the tilt and add \(\sup|\operatorname{Im}S_v(0)|\) to \(t_v\).
4. \(Z_2\) is a system of the kind treated by the corresponding construction theorem (Repair §4, (R9)–(R14)): normalized holomorphic kernels with product bound \(M=e^{3t}\), and only the interactions of \(\mathcal E_2\).

**Source support for the hypotheses.** Positivity: LFR II p.379–380 (source): "All the expressions in the definition (1.71), for the configuration \(U\), are real, and the exponential density in the integral is positive. […] The expression \(\mathbf T'_k(X,(U,0))1\) is obviously positive". The kernel response is uniformly small on the whole analyticity domain: p.379, "We expand them up to the first order in \(A',\mathbf J\), the first order terms are already small", with the bound \(O(1)B_3^2A_1^2C_0M^dR_k^{d+2}p_1^2(g_k)q_0(g_k)g_k\), and (1.73)–(1.75), p.380, with \(|\sigma|\le1\) used on p.388. (Real) for the boundary terms at real fields is not printed; it is expected because the densities are positive and all expansions are real at real fields. It is a premise.

### 3.2 Proposition R3 (the increment load of a component, with a collar)

**Setting.** As in [Boundary estimate b] §2.1: \(d,L,M,K\); the grid \(\mathcal G_b\) of cubes of side \(s_b=Mh_b\le M\); the capped metric \(d^{(b)}\) of [Hidden components] (C.1), for which \(|x-y|_\infty\le M\,d^{(b)}(x,y)\) and a Euclidean segment of length \(\ell\) has capped length \(\le\ell/s_b\); sites \(x_i\), \(i\in I\), with at most \(n_I(r+1)^d\) sites in any cube of side \(r\); the polydisc \(D_P\). Fix a component \(v\) with hole \(Q\), a finite set of \(\mathcal G_b\)-cubes with \(D_Q=s_b^{-1}\operatorname{diam}_\infty(\cup Q)\). Assume:

- **(Col\(_b\))** \(d^{(b)}(x_i,\cup Q)\ge\theta D_Q\) for all \(i\in I\), with \(\theta\in(0,1]\).
- Each \(e\in\mathcal E_1(v)\) has an exterior \(F_e\ne\emptyset\), a finite set of \(\mathcal G_b\)-cubes not in \(Q\), one of which touches \(Q\); carrier \(X_e=F_e\cup Q\); at most \(m_0\) interactions have the same exterior; and
\[
\sup_{D_P\times\Omega_v}|\partial_iV_e|\le\frac{w_e}{P}e^{-\nu d^{(b)}(x_i,\cup X_e)},\qquad w_e\le We^{-\kappa_*\delta_b(F_e)}.
\tag{Loc′\(_b\)}
\]
- **(Resp)** \(\sup_{D_P\times\Omega_v}|\partial_i\sigma_v|\le\frac{s_*}{P}e^{-\nu d^{(b)}(x_i,\cup Q)}\).
- \(0<\nu_1\le\nu\) and \(\kappa_*-\nu_1\ge\kappa'_{\rm cnt}(d)\).

(Loc′\(_b\)) follows from [Boundary estimate b]'s (Loc′), because \(d^{(b)}\le d_g\). (Col\(_b\)) is stronger than [Boundary estimate b]'s (Col); the source support is the same, see §5.

**Proposition R3.** Put \(C_A=4m_0K_d^{3\cdot2^d}e^{2\nu_1\sqrt d}\), \(\Theta_3=M(2+1/\theta)+1\), \(J_d(\nu_1)=2e^{\nu_1/2}d!\,(2/\nu_1)^d\). Then:

1. For every site \(i\) and all \((z,\omega)\):
\[
|\partial_i\tau_v(z,\omega)|\le\frac{s_*+C_AW\,N_{\rm att}(Q)}{P}\,e^{-\nu_1d^{(b)}(x_i,\cup Q)}.
\]
2. \(\displaystyle t_v\le\bigl(s_*+C_AW\,N_{\rm att}(Q)\bigr)\,n_I\Theta_3^d\,J_d(\nu_1)\,e^{-\nu_1\theta D_Q/2}\ \le\ C_B\,(s_*+W),\)
with \(C_B=n_I\Theta_3^dJ_d(\nu_1)\max\{1,\,C_A3^d(2d/(e\nu_1\theta))^d\}\). \(C_B\) depends on \(d,M,\nu_1,n_I,m_0,\theta\) only; in particular not on \(D_Q\).
3. If \(t_v\le\frac14\): \(\displaystyle|\partial_i\log G_v(z)|\le\frac{\widehat W}{P}e^{-\frac{\nu_1}2d^{(b)}(x_i,\cup Q)}\) on \(D_P\), with \(\widehat W=e^{3/4}\bigl(s_*+C_A3^d(2d/(e\nu_1\theta))^dW\bigr)\); and \(|\partial_i\log N_v(z)|\le e^{3/4}\frac{s_*}{P}e^{-\nu d^{(b)}(x_i,\cup Q)}\).

*Proof.* **Step 1 (geometry).** For \(e\in\mathcal E_1(v)\) and a site \(x\): \(d^{(b)}(x,\cup X_e)\ge d^{(b)}(x,\cup Q)-\delta_b(F_e)-2\sqrt d\). Indeed let \(p\in\cup X_e\) with \(d^{(b)}(x,p)\le d^{(b)}(x,\cup X_e)+\varepsilon\). If \(p\in\cup Q\) there is nothing to prove. If \(p\in c\in F_e\), take a tree \(T\) meeting all cubes of \(F_e\) with \(|T|\le s_b(\delta_b(F_e)+\varepsilon)\), and the cube \(c'\in F_e\) touching \(Q\). The path \(p\to T\cap c\to\) (along \(T\)) \(\to T\cap c'\to\) a point of \(c'\cap\cup Q\) has capped length \(\le\sqrt d+\delta_b(F_e)+\varepsilon+\sqrt d\). So \(d^{(b)}(x,\cup Q)\le d^{(b)}(x,p)+\delta_b(F_e)+2\sqrt d+\varepsilon\).

**Step 2 (item 1).** For real \(a\ge\max(a',0)\) and \(\nu_1\le\nu\), \(e^{-\nu a}\le e^{-\nu_1a'}\). With Step 1,
\[
\sum_{e\in\mathcal E_1(v)}w_ee^{-\nu d^{(b)}(x_i,\cup X_e)}\le e^{2\nu_1\sqrt d}e^{-\nu_1d^{(b)}(x_i,\cup Q)}\sum_eWe^{-(\kappa_*-\nu_1)\delta_b(F_e)}.
\]
Every exterior has a cube among the \(N_{\rm att}(Q)\) cubes touching \(Q\). For a fixed such cube \(q\), [Boundary estimate b] Prop. B2′ (with \(H=\{Q\}\), \(\vartheta=0\), \(a=\kappa_*-\nu_1\)) gives \(\sum_{F\ni q}We^{-a\delta_b(F)}\le4WK_d^{3\cdot2^d}\). Multiply by \(m_0N_{\rm att}(Q)\) and add (Resp).

**Step 3 (item 2).** For \(z\in D_P\), \(|V_e(z)-V_e(0)|\le\sum_i|z_i|\sup|\partial_iV_e|\) (integrate along the segment), likewise for \(\sigma_v\). So \(t_v\le(s_*+C_AWN_{\rm att}(Q))\sum_ie^{-\nu_1d^{(b)}(x_i,\cup Q)}\). Let \(N(t)=\#\{i:d^{(b)}(x_i,\cup Q)\le t\}\). These sites are within sup-distance \(Mt\) of \(\cup Q\), which lies in a cube of side \(s_bD_Q\le MD_Q\), so \(N(t)\le n_I(MD_Q+2Mt+1)^d\). By (Col\(_b\)), \(N(t)=0\) for \(t<\theta D_Q\), and for \(t\ge\theta D_Q\), \(MD_Q\le Mt/\theta\), so \(N(t)\le n_I\Theta_3^d(1+t)^d\). Hence
\[
\sum_ie^{-\nu_1d^{(b)}(x_i,\cup Q)}=\nu_1\!\int_{\theta D_Q}^\infty\!e^{-\nu_1t}N(t)\,dt\le n_I\Theta_3^de^{-\nu_1\theta D_Q/2}\,\nu_1\!\int_0^\infty\!e^{-\nu_1t/2}(1+t)^ddt\le n_I\Theta_3^dJ_d(\nu_1)e^{-\nu_1\theta D_Q/2}.
\]
Finally \(N_{\rm att}(Q)\le(D_Q+2)^d\le3^dD_Q^d\) and \(\sup_{D\ge1}D^de^{-\nu_1\theta D/2}\le(2d/(e\nu_1\theta))^d\).

**Step 4 (item 3).** Theorem R1(4), item 1, and \(e^{-\nu_1d^{(b)}(x_i,\cup Q)}\le e^{-\nu_1\theta D_Q/2}e^{-\frac{\nu_1}2d^{(b)}(x_i,\cup Q)}\) by (Col\(_b\)). \(\square\)

**Reading.** The attachment entropy \(N_{\rm att}(Q)\le3^dD_Q^d\) is polynomial in the diameter. Every current site is at capped distance \(\ge\theta D_Q\) from the hole, and each increment needs a first derivative, which costs \(e^{-\nu_1\theta D_Q}\) either through (Loc′\(_b\)) or through the exterior tree. The collar therefore pays the surface entropy as well as the hidden carrier distance. Under (W) the collar is needed anyway ([Boundary estimate b] Remark 3 to Theorem C′; the corresponding construction two-attachment diagnostic (R29)–(R31)), so this costs no new premise.

### 3.3 Corollary R5 (the single-component part of the boundary functional as hole-anchored records) conditional

Assume the setting of [Boundary estimate b] Theorem E′ with (Loc′\(_b\)), (Col\(_b\)), (Resp), (Real), positivity of the base kernels at the centre of \(D_P\), and \(C_B(s_*+W_b)\le\frac14\) for every birth \(b\). For each component \(v\) of birth \(b\) with hole \(Q_v\) choose a cube \(c_v\notin Q_v\) touching \(Q_v\) and meeting \(\overline{\{g\le b\}}\). Then \(\rho_v:=\log G_v-\log N_v\) (which vanishes at \(z=0\)) is holomorphic on \(D_P\) and satisfies
\[
|\partial_i\rho_v(z)|\le\frac{2\widehat W_b}{P}\,e^{-\frac{\nu_1}2d^{(b)}(x_i,\,c_v\cup\cup Q_v)} ,
\]
i.e. it is a record in the format of [Boundary estimate b] §2.1 with \(H=\{Q_v\}\), \(F=\{c_v\}\), \(\delta_b(F)=0\), weight \(2\widehat W_b\), decay rate \(\nu_1/2\), measured in the capped metric; distinct components have distinct anchor cubes by (H-sep). Consequently the family \(\{\rho_v\}\) obeys the root-sum bound (C′.1) of [Boundary estimate b] with \(\mathcal A'_b\le2\widehat W_b\), \(\nu\) replaced by \(\nu_1/2\) and \(d_g\) replaced by \(d^{(b)}\) in (Loc′) and (Col).

*Hypotheses.* The displayed derivative bound is deduction from Prop. R3(3) (enlarging the set to which distance is measured only weakens the bound). The application of Theorem C′ in its capped form is conditional: The formula gives each step of [Boundary estimate b]'s proof uses \(d_g\) only through \(|x-p|_\infty\le M\,d(x,p)\), the triangle inequality, (Col), and — in Step 4 — the inequality \(d^{(b)}\le d_g\), all of which hold with \(d^{(b)}\) throughout; This remains an assumption.

So, when \(\mathcal E_2=\emptyset\), the full current dependence of the retained-component sector is \(\sum_v\rho_v\) (Theorem R1(5)), and its Hessian rows and jets are bounded uniformly in the volume, the depth and the number, sizes and positions of the holes, **with no condition on the component loads**.

### 3.4 Proposition R4 (interactions touching several components)

Assume the holes of one birth \(b\) are pairwise at \(\ell^\infty\) index distance \(\ge\rho_b\ge3\). Let \(e\) have hole set \(H_e\), \(|H_e|\ge2\), exterior \(F_e\) containing for each \(Q\in H_e\) a cube touching \(Q\), and \(\sup|V_e|\le We^{-\kappa_*\delta_b(F_e)}\), at most \(m_0\) per \((F,H)\). Let \(\varrho\ge1\), \(\kappa_2>0\) with \(\kappa_*-2^{d+1}\log\varrho-\kappa_2\ge\kappa'_{\rm cnt}(d)\). Then for every hole \(Q\),
\[
\sum_{e\in\mathcal E_2:\,Q\in H_e}\varrho^{|H_e|}\sup|V_e|\ \le\ 4m_0\,\varrho^{2^d}K_d^{3\cdot2^d}\,W\,N_{\rm att}(Q)\,e^{-\kappa_2(\rho_b-3)}.
\]

*Proof.* Cubes touching two different holes of \(H_e\) are at index distance \(\ge\rho_b-2\), so any tree visiting both has length \(\ge(\rho_b-3)s_b\): \(\delta_b(F_e)\ge\rho_b-3\). By (H-sep) distinct holes need distinct touching cubes, so \(|H_e|\le|F_e|\le2^d(2\delta_b(F_e)+1)\) and \(\varrho^{|H_e|}\le\varrho^{2^d}e^{2^{d+1}\log\varrho\,\delta_b(F_e)}\). Extract \(e^{-\kappa_2(\rho_b-3)}\) and apply [Boundary estimate b] Prop. B2′ at each of the \(N_{\rm att}(Q)\) cubes touching \(Q\). \(\square\)

With \(\rho_b\ge R_b\) and \(D_Q\le100R_b+1\) (source: components of \(Z\) are unions of \(MR_k\)-cubes of one partition and are joined when they "intersect, or touch", LFR II p.386, source; so distinct components are separated by a full \(MR_k\)-cube; additional assumption for the inference, as in [Hidden components] S2), the right side is \(\le CW\sup_R(100R+3)^de^{-\kappa_2(R-3)}\), uniformly small for small \(W\). With \(\varrho=e\cdot e^{3t}\) this is the unweighted form of the component-load condition (R11) for the system \(Z_2\) of Theorem R1. The version with the extent weights \(e^{\lambda\ell_e}\) of (R10)–(R11), and the current-root load \(K_*\) of (R23) for \(Z_2\), are not derived here; they need the same collar and the corresponding construction localization of kernels (R21)–(R24) applied to \(\Pi'_{v,z}\). That part is conditional on the corresponding construction theorem.

### 3.5 Route B: the final remark under (Osc)

**Premise (Osc).** For a retained component \(Q\) of the R step at scale \(k\), with integration variables \(\omega\) of \(\mathbf T'_k(Q)\), every term \(B_e\) attached to \(Q\) alone satisfies
\[
\operatorname{osc}_\omega B_e:=\sup_{\omega,\omega'}|B_e(\cdot,\omega)-B_e(\cdot,\omega')|\ \le\ w_e\,e^{-\delta_*\ell_Q},\qquad\ell_Q=\operatorname{dist}(\partial Q,\Lambda_Q)/M\ \ge10R_k-5,
\]
on the analyticity domain, where \(w_e\) is the bound for \(|B_e|\).

**Proposition 3.6 (deduction; given (Osc) and a standard cluster theorem).** Put \(B_e^{\rm ext}=\mu_Q(B_e)\) (average over \(\omega\) with the base kernel at a real field) and \(\widetilde B_e=B_e-B_e^{\rm ext}\). Then
\[
(\mathbf T'1)^{-1}\mathbf T'\exp\sum_eB_e=\exp\Bigl(\sum_eB_e^{\rm ext}\Bigr)\cdot(\mathbf T'1)^{-1}\mathbf T'\exp\sum_e\widetilde B_e,
\]
\(|B_e^{\rm ext}|\le w_e\), \(B_e^{\rm ext}\) is analytic and independent of \(\omega\), and \(\sum_e\sup|\widetilde B_e|\le4K_d^{3\cdot2^d}WN_{\rm att}(Q)e^{-\delta_*\ell_Q}\) when \(w_e\le We^{-\kappa_*\delta(F_e)}\), \(\kappa_*\ge\kappa'_{\rm cnt}\). Since \(N_{\rm att}(Q)\le(100R_k+3)^d\), this load tends to \(0\) as \(R_k\to\infty\), and the second factor exponentiates by the standard criterion ((2.1), or (R11) of the corresponding construction repair). The representation (1.104) then holds with boundary terms \(B_e^{\rm ext}\) (same carriers and bounds as \(B_e\), under (W)) plus cluster terms of total weight \(O(WN_{\rm att}e^{-\delta_*\ell_Q})\) per component.

*Proof.* \(B_e^{\rm ext}\) does not depend on \(\omega\), so it commutes with \(\mathbf T'\). \(|\widetilde B_e|\le\operatorname{osc}_\omega B_e\). The count is [Boundary estimate b] Lemma 4.1. \(\square\)

**Why (Osc) is plausible additional assumption.** A term \(V(Y)\), \(Y\supset Q\), with exterior at the surface of \(Q\) can depend on the variables in \(\Lambda_Q\) in three ways.

1. Through a nonempty localization domain \(Y'_i\). Each component of \(Y'_i\) "contains a component of \(\Lambda\), and intersects" the boundary layer of \(Y_{i-1}\) (pp.373–374), so it crosses \(\ge\ell_Q\) cubes inside \(Q\) and carries \(\exp(-(\kappa_1-1)M^{-d}|Y'_i|)\le e^{-(\kappa_1-1)\ell_Q}\) in (1.66). After extraction of \(d_{k,Z}(Y_4)\), half of this factor is still present ("the following exponential remains", p.376) and is used for resummations; a quarter can be kept.
2. Because the original domain \(X\) itself reaches \(\Lambda_Q\). Then \(d_k(Y_0)\ge\max\{d_{k,Z}(Y),\ell_Q\}\ge(1-\lambda)d_{k,Z}(Y)+\lambda\ell_Q\), and with \(\lambda=\beta/(1+3\beta)\) the factor \(e^{-(1+3\beta)\kappa d_k(Y_0)}\) of (1.66) yields \(e^{-(1+2\beta)\kappa d_{k,Z}(Y)}e^{-\beta\kappa\ell_Q}\). deduction for this arithmetic.
3. For an exceptional term with \(X\) far from \(\Lambda_Q\): only through the dependence of the configuration \(U(\mathbf B''_k(Y_1),\cdot)\) at \(X\) on its data in \(\Lambda_Q\), (1.61). Minimizers depend on distant data with exponentially small derivative in the scaled distance (the decay used for (1.66); CMP99, CMP102 277–309). No estimate of this form for the terms \(V(Y)\) is displayed. **This is the part of (Osc) that needs a proof.**

Route B needs neither positivity nor the collar and is valid at the birth step, so it would restore [Hidden components]/[Boundary estimate b]'s premise P1/P1′ in its original form (alternative representation at each R step, with (W) bounds).

### 3.6 A modified last resummation (thick collar)

**Lemma T.** Let \(n\ge1\) and let \(\mathcal E_1^{>n}(Q)\) be the single-hole terms of \(Q\) whose exterior is not contained in \(Q^{\sim n}\) (index distance \(\le n\) from \(Q\)). If \(w_e\le We^{-\kappa_*\delta(F_e)}\) and \(\kappa_*-\kappa_3\ge\kappa'_{\rm cnt}(d)\), then
\[
\sum_{e\in\mathcal E_1^{>n}(Q)}w_e\le4K_d^{3\cdot2^d}W\,N_{\rm att}(Q)\,e^{-\kappa_3(n-1)}.
\]
*Proof.* \(F_e\) has a cube touching \(Q\) and a cube at index distance \(>n\) from \(Q\), so \(\delta(F_e)\ge n-1\). Then as in Prop. R4. \(\square\)

So if the "last resummation" of p.377 is made with \(Z^{\sim n_k}\) in place of \(Z^\sim\), \(n_k=1+\lceil(d\log(100R_k+3)+C)/\kappa_3\rceil=O(\log R_k)\), the terms absorbed into \(\mathbf T'_k\) obey the volume bound (1.69) on \(Q^{\sim n_k}\) (volume still \(\le(103R_k)^d\), which every estimate on pp.379–389 tolerates), and the remaining terms attached to one component have total weight \(\le\eta\), any prescribed constant. Then the argument of the final remark works as printed. The collars of different components do not meet since \(n_k\ll R_k\). *Not examined:* the multiplier \(\mathbf T'_k(Y_i)1\) then depends on \(U_k\) on \(Y_i^{\sim n_k}\), and the statement "These functions depend only on the new field variables \(V_k\) restricted to \(Y_i\)" (p.392) has to be replaced by dependence on a neighbourhood that still lies in \(\Omega_{k+1}^c\) (it does, by §5: the margin is \(8LR_{k+1}\) cubes). This is (d) beyond the lemma.

### 3.7 Comparison of the routes

| | Representation used | Needs | Gives |
|---|---|---|---|
| A (§3.1–3.4) | Main representation of the source, (2.18) [III]: kernels kept; logarithm taken at the current step | (Pos), (Real), (Loc′\(_b\)) uniform in \(\omega\), (Resp), (Col\(_b\)), separation \(\rho_b\gtrsim\log D_Q\) | Current jets of the retained-component sector with no component-load condition for single-component terms |
| B (§3.5) | Final remark (1.104) | (Osc) | P1/P1′ as stated in [Hidden components], [Boundary estimate b], under (W) |
| Thick collar (§3.6) | Final remark with modified \(\mathbf T'\) | re-examination of pp.378–392 with \(Z^{\sim n_k}\) | as B, without (Osc) |

Route A is consistent with the two-attachment diagnostic (R29)–(R31): there the centre values vanish, the increments are small, and \(F_{xy}=g^2\) is unbounded only against a weight \(e^{\chi\rho(x,y)}\) with no collar. In Cor. R5 the collar supplies \(e^{-\nu_1\theta D_Q}\) per derivative.

## 4. The "whole-hole" condition of P1′

### 4.1 Lemma N (normalization by enlargement and resummation)

Let \(\mathcal Q\) be a family of holes with (H-sep) (index distance \(\ge3\)). Let \(\mathcal R\) be a family of records, each with a \(*\)-connected finite carrier \(X\) of \(\mathcal G_b\)-cubes not contained in a single hole, a sub-family \(H^0\subset\{Q\in\mathcal Q:Q\subset X\}\) of holes it contains *entirely*, and a weight
\[
w\le We^{-\kappa\,\delta_b(X\setminus\cup H^0)},
\tag{N.1}
\]
at most one record per pair \((X,H^0)\). (So the bound charges every cube of the carrier outside the holes that are wholly contained and declared.) For such a record put \(H=\{Q\in\mathcal Q:Q\cap X\ne\emptyset\}\), \(F=X\setminus\cup H\), \(X^+=X\cup\bigcup H\). Then:

1. \(F\ne\emptyset\), every \(Q\in H\) touches a cube of \(F\), and \(X^+=F\cup\bigcup H\).
2. If the record satisfies (Loc′) with carrier \(X\), it satisfies (Loc′) with carrier \(X^+\).
3. For every pair \((F,H)\), with \(\kappa''=2^{d+1}\log(2K_d)\) and \(\kappa>\kappa''+\log 2\),
\[
\sum_{\rho\in\mathcal R:\ (F_\rho,H_\rho)=(F,H)}w_\rho\ \le\ 4(2K_d)^{3\cdot2^d}e^{\kappa-\kappa''}\,W\,e^{-(\kappa-\kappa'')\delta_b(F)}.
\]

So after summing the records with the same \((F,H)\), the family is in the format of [Boundary estimate b] P1′ with \(\kappa_*=\kappa-\kappa''\).

*Proof.* (1) \(X\) is \(*\)-connected and not inside one hole, and holes are at index distance \(\ge3\), so \(X\) has a cube outside all holes, and for each \(Q\) met by \(X\) a \(*\)-path in \(X\) from \(Q\) to that cube leaves \(Q\) through a cube touching \(Q\), which lies in no other hole. (2) \(d(x,\cup X^+)\le d(x,\cup X)\). (3) Fix \((F,H)\) and a cube \(q\in F\). A record with this pair has \(X=F\cup A\) with \(A\subset\cup H\), and \(X\setminus\cup H^0\supseteq F\cup(A\setminus\cup H^0)\). Put \(G=X\setminus\cup H^0\); then \(q\in G\), \(\delta_b(G)\ge\delta_b(F)\), and \(w\le We^{-\kappa\delta_b(G)}\). The record is determined by \(G\) and \(H^0\), and \(H^0\) is a set of holes each touching a distinct cube of \(G\) (as in (1)), so at most \(2^{|G|}\) choices. By the counting in the proof of [Boundary estimate b] Prop. B2′, the number of sets \(G\ni q\) with \(\delta_b(G)\in[j,j+1)\) is \(\le2K_d^{\,n_j}\) with \(n_j=2^d(2j+3)\) (there \(K_d^n\) counts a \(*\)-connected hull, a subset, and a set of attached holes; Use it for the pair \((G,H^0)\)), and \(|G|\le n_j\). Hence
\[
\sum w\le\sum_{j\ge\lfloor\delta_b(F)\rfloor}2K_d^{\,n_j}We^{-\kappa j}\le2K_d^{3\cdot2^d}W\sum_{j\ge\lfloor\delta_b(F)\rfloor}e^{-(\kappa-2^{d+1}\log K_d)j},
\]
which is bounded by the stated expression (the constants are not optimized; I enlarged \(K_d\) to \(2K_d\) to leave room). \(\square\)

### 4.2 What Lemma N reduces the condition to

(N.1) covers both forms that occur in the source:

- terms created by a T step in the form chosen in [III]: \(X\in\mathbf D_j\), \(X\cap\Omega_j\ne\emptyset\), \(X\cap Z_j^\sim\ne\emptyset\), \(|\mathbf B^{(j)}(X)|<B_0e^{-\kappa d_j(X)}\) ((2.41)–(2.42), p.261, source). Here \(H^0=\emptyset\) and the full carrier is charged;
- terms created by an R step: carrier containing whole components of \(Z\), bound in \(d_{k,\cup Y_i}\) ((1.99), p.390, source). Here \(H^0\) is the set of those components.

Bałaban's own statement of the normalized form is [III] p.262 (source): "we may resum all the terms with localization domains intersecting a given component of the large field region. This gives sum (2.41), with the summation over domains \(X\in\mathbf D_j\) such that \(X\) either contains a component of the large field region \(Z_j\), or is disjoint with it. Resumming we lose a part of the exponential factor in (2.42), connected with the region \(Z_j\); hence for the new terms we obtain the bound (2.42) with \(d_j(X)\) replaced by \(d_j(X\setminus Z_j)\). All constructions and proofs of the procedure can be carried on with these inductive assumptions." Lemma N(3) is a proof of the "lose a part of the exponential factor" step with explicit constants.

What remains to be checked in the source for later steps is therefore only:

> **(Mon)** When a later operation produces a term from a record with carrier \(X\) and declared holes \(H^0\), the new carrier contains \(X\), and the new bound charges every cube of the new carrier outside \(\cup H^0\).

Then the new record again satisfies (N.1) with respect to the holes of its own step, including the case where the component has grown (\(S(Z)=Z'^{\sim10}\)): the grown part is not in \(H^0\), so it is charged, and Lemma N(3) handles the resummation over the shapes inside it. Source support for (Mon), source: LFR II p.373 (Q1), p.376 (Q2): the new domains \(Y_0,Y_1,\dots,Y_4\) all contain \(X\), and (1.66) keeps \(e^{-\beta\kappa d_j(X)}\) and adds factors for the new parts. For the T steps of [III] §3 The argument assumes it (p.275: "we resum them in localization domains \(Y_0\in\mathbf D_k\)").

### 4.3 Two points about the hole families that both notes should fix

1. **Holes per birth.** [Boundary estimate b] P1′ says "the holes of birth \(b\) are the retained components of the R step at scale \(b\)". A record born at a later scale \(j>b\) near a component retained at \(b\) attaches to that component *as it is at scale \(j\)*, i.e. to the corresponding component of \(Z_j\) (grown by the intermediate steps, a union of \(MR_j\)-cubes). The hole family \(\mathcal Q_j\) should be the set of components of the large-field region \(Z_j=\Lambda_j^c\) at step \(j\) ([III] (2.3)), and one kernel \(v\) then has a "shadow" \(Q_v^{(j)}\in\mathcal Q_j\) for every \(j\) from its birth on. In Theorem R1, \(\mathcal E_1(v)\) contains the records of all births attached to these shadows, and Prop. R3(2) is applied birth by birth and summed. The sum over \(j\) converges if the layer widths between consecutive grades are bounded below (each later birth has a larger capped distance to the current sites) and \(W_j\) is subexponential in the age. This estimate remains a hypothesis; it is the same summation as \(\sum_b\Gamma_bW_b\).
2. **Components that are not eligible.** A large-field component that fails condition (i) can have any diameter, while its collar to \(\Omega_{k+1}\) is \(8LR_{k+1}\) cubes (§5). For such a component (Col), (Col\(_b\)) fail, \(N_{\rm att}\) is unbounded, and neither Prop. R3 nor [Boundary estimate b] Theorem C′ applies. The source never needs a logarithm of the integral over such a component (it is bounded by positivity, (1.73), with the large-field factors). If the conditional law integrates the internal variables of non-eligible components, the two-attachment mechanism is unbounded for them; if it conditions on those variables, there is no kernel and the terms are ordinary records with frozen parameters. The hypotheses do not specify from [Hidden components], [Boundary estimate b] or the corresponding construction repair which is the case. **This must be settled before any premise list for C-05 is complete.**

## 5. P4: the layer margin, as stated in the source

[III] pp.264–265 (source):

- p.264: "The term has a large field region \(Z_k=\Lambda_k^c\), and we denote by \(Z'_k\) the union of all \(LMR_{k+1}\)-cubes intersecting the region \(Z_k\), and belonging to the partition of the lattice \(T_\eta\). […] We surround \(Z'_k\) by"
- p.265: "four layers of the \(LMR_{k+1}\)-cubes, i.e., we take the domain \(Z'^{\sim4}_k\), and we introduce the following decomposition of unity for the domain \((Z'^{\sim4}_k)^c\) […] where the summation is over domains \(P_{k+1}\subset(Z'^{\sim4}_k)^c\) […] We take the set \(P'_{k+1}\) – the union of all \(LMR_{k+1}\)-cubes intersecting \(P_{k+1}\) – and we surround the union \(P'_{k+1}\cup Z'^{\sim4}_k\) by a layer of \(LMR_{k+1}\)-cubes. In the complement \((P'^\sim_{k+1}\cup Z'^{\sim5}_k)^c\) we introduce the axial gauge fixing […] Denote by \(P^1_{k+1}\) the subset of \(T^{(k+1)}\) such that \(B^{k+1}(P^1_{k+1})=(P'^\sim_{k+1})^c\cap(Z'^{\sim5}_k)^c\). […] Denote \(\Omega_{k+1}=(Q'^{\sim2}_{k+1}\cup(B^{k+1}(P^1_{k+1})^c)^{\sim3})^c\) (3.5)".

Hence \(\Omega_{k+1}^c\supseteq(B^{k+1}(P^1_{k+1})^c)^{\sim3}\supseteq(Z'^{\sim5}_k)^{\sim3}=Z'^{\sim8}_k\). **The margin between \(Z_k\) and \(\Omega_{k+1}\) is at least eight layers of \(LMR_{k+1}\)-cubes**, i.e. \(8LR_{k+1}\) scale-\(k\) \(M\)-cubes. [Boundary estimate b] §2.6 used four, which is where new large fields \(P_{k+1}\) may start, and is a valid lower bound. After an R step at scale \(k\), "The new large field region is equal to \(Z_k\cup\bigcup Y_i\)" (LFR II p.390, source), so the retained \(Y_i\) are part of the \(Z_k\) of [III] §3 for the next T step.

With \(D_Q\le100R_k+1\) (condition (i)) and \(R_k\le(L+1)R_{k+1}\) ([III] (2.9), p.256, source):
\[
\theta\ \ge\ \frac{8LR_{k+1}}{100R_k+1}\ \ge\ \frac{8L}{101(L+1)}\quad(\ge1/19\ \text{for }L\ge2).
\]
The margin lies in \(\Lambda_k\setminus\Omega_{k+1}\subset\Omega_k\setminus\Omega_{k+1}\), where the grade is \(k\) and the capped and graded units coincide, so the same \(\theta\) serves (Col\(_b\)). The regions are nested, \(\Omega_K\subset\Omega_{k+1}\) for \(K>k\) ([III] §2, source), so the margin persists for later current sites, except inside a later eligible component that swallows the hole (then the hole's records are old records of that component, as in [Boundary estimate b] §2.6 item 2).

Status of P4: source input for the eight layers and for (2.9); additional assumption for the identification of the current sites with points of \(\Omega_K\); **valid only for components satisfying condition (i)** (§4.3 item 2).
