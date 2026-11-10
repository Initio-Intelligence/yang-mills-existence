# Summation over roots with hidden holes

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

**Propagation hypothesis.** Any use of a T-step bound on a holed ancestor requires the conditional single-ancestor estimate and, for connected products, a separate collective crossing estimate. An argument from the diameter of the union of paid components alone is invalid.

## 2. A root-sum theorem with hidden holes and no shell

### 2.1 Setting

Keep [Hidden components] §4.1 verbatim:
- \(d,L,M,K\), meshes \(h_n=L^{n-K}\);
- the grade function \(g\) and the metrics \(d_g\), \(d^{(b)}\) of (C.1), with (C.2);
- the layer hypothesis (Geo) (C.3)–(C.4);
- sites \(x_i\) (\(i\in I\)) with \(g(x_i)=K\) and density \(n_I\);
- the polydisc \(D_P\);
- the visiting size \(\delta_b=\delta_{s_b}\) of (1.1), \(s_b=Mh_b\).

Add the following.

- **Holes.** For each birth \(b\), a family \(\mathcal Q_b\) of pairwise disjoint finite sets of \(\mathcal G_b\)-cubes. Any shape is allowed. Distinct holes have \(\ell^\infty\) index distance \(\ge3\): **(H-sep)**. Put \(D_Q=s_b^{-1}\operatorname{diam}_\infty(\cup Q)\), the hole diameter in own cubes.
- **(Col), proportional collar.** For some \(\theta\in(0,1]\): \(d_g(x_i,\cup Q)\ge\theta D_Q\) for all \(i\in I\), all \(b\) and all \(Q\in\mathcal Q_b\).
- **Records.** Each \(\rho\) has:
  - a birth \(b\);
  - a finite set \(H_\rho\subset\mathcal Q_b\) of holes;
  - a nonempty finite set \(F_\rho\) of \(\mathcal G_b\)-cubes, the *exterior*, containing no cube of any \(Q\in H_\rho\);
  - the carrier \(X_\rho=F_\rho\cup\bigcup_{Q\in H_\rho}Q\);
  - **(Att)**: every \(Q\in H_\rho\) contains a cube touching (sharing a point with) a cube of \(F_\rho\). This holds automatically if \(X_\rho\) is face-connected, \(F_\rho\neq\emptyset\) and (H-sep) holds;
  - an anchor cube \(q_\rho\in F_\rho\) meeting \(\overline{\{g\le b\}}\);
  - a weight \(w_\rho\) and \(F_\rho(z)\) holomorphic on \(D_P\) with

\[
\textbf{(Loc}'\textbf{)}\qquad |\partial_iF_\rho(z)|\le\frac{w_\rho}{P}e^{-\nu d_g(x_i,\cup X_\rho)}\qquad(i\in I,\ z\in D_P).
\]

- **Rooted norm.** \(\mathcal A'_b(\vartheta)=\sup_{q\in\mathcal G_b}\sum_{\rho:\,b(\rho)=b,\,q_\rho=q}w_\rho e^{\vartheta\delta_b(F_\rho)}\).

Put \(\Theta=1+1/\theta\) and \(\Theta'=1+\sqrt d/\theta\).

Note that (Loc′) is stated with the **full** carrier, holes included. That is the physically correct form: a record depends on the fields of its holes.

### 2.2 Lemma C3 (geometry of a record seen from a site)

Let \(\rho\) be a record of birth \(b\), \(x=x_i\) a site, \(\Delta=d_g(x,\cup X_\rho)\), \(\delta=\delta_b(F_\rho)\). Then

1. \(\operatorname{dist}_\infty(x,\cup F_\rho)\le M\Theta\,\Delta\);
2. for every point \(a\) of the anchor cube \(q_\rho\): \(d^{(b)}(x,a)\le\Theta'\Delta+\delta+2\sqrt d\);
3. \(\operatorname{diam}_\infty(\cup F_\rho)\le s_b(\delta+2)\).

*Proof.* (3) is Lemma A3 of [Hidden components], which needs no connectivity.

For (1)–(2), let \(\varepsilon>0\) and pick \(p\in\cup X_\rho\) with \(d_g(x,p)\le\Delta+\varepsilon\). By (C.2), \(|x-p|_\infty\le M(\Delta+\varepsilon)\).

*Case \(p\in c\in F_\rho\).* (1) is immediate. For (2), go from \(x\) to \(p\) (capped length \(\le d_g(x,p)\), because capping only enlarges the unit). Then go straight to a point of \(T\cap c\), where \(T\) is a tree meeting every cube of \(F_\rho\) with \(|T|\le s_b(\delta+\varepsilon)\). Then go along \(T\) to \(T\cap q_\rho\), and straight to \(a\). The capped unit is \(\ge s_b\) everywhere, so the capped length is \(\le\Delta+\varepsilon+\sqrt d+\delta+\varepsilon+\sqrt d\).

*Case \(p\in\cup Q\), \(Q\in H_\rho\).* By (Col), \(\Delta+\varepsilon\ge d_g(x,\cup Q)\ge\theta D_Q\). By (Att) there are cubes \(c''\in Q\) and \(c\in F_\rho\) and a point \(r\in c''\cap c\). Then \(|p-r|_\infty\le\operatorname{diam}_\infty(\cup Q)=s_bD_Q\le M(\Delta+\varepsilon)/\theta\). So
\[
\operatorname{dist}_\infty(x,\cup F_\rho)\le|x-p|_\infty+|p-r|_\infty\le M(\Delta+\varepsilon)(1+1/\theta),
\]
which is (1). For (2), the straight segment \(p\to r\) has Euclidean length \(\le\sqrt d\,s_bD_Q\), hence capped length \(\le\sqrt dD_Q\le\sqrt d(\Delta+\varepsilon)/\theta\). Continue from \(r\in c\) as in the first case. Total \(\le(\Delta+\varepsilon)(1+\sqrt d/\theta)+\delta+2\sqrt d+O(\varepsilon)\).

Let \(\varepsilon\downarrow0\). \(\square\)

### 2.3 Theorem C′

**Theorem C′.** Assume §2.1 with \(\nu>0\), \(0\le\chi\le\nu/(4M\Theta)\), and (Geo) with \(c=\nu/(4\Theta')\), with constants \(\gamma,C_0\); let \(\Gamma_b\) be as in (C.9). Then for every \(m\ge1\), \(i_1\in I\) and \(z\in D_{P/2}\),
\[
\sum_{\rho}\sum_{i_2,\dots,i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}\,|\partial_{i_1}\cdots\partial_{i_m}F_\rho(z)|
\le\frac{C'_a\,C_b'^{\,m-1}((m-1)!)^{d+1}}{P^m}\sum_{b=1}^K\Gamma_b\,\mathcal A'_b\!\left(\tfrac\nu2+1\right),
\tag{C′.1}
\]
\[
C'_a=3^dS_d\!\left(\tfrac{\nu}{8\Theta'}\right)\exp\Bigl\{3+\tfrac\nu2+\tfrac{\nu\sqrt d}{2\Theta'}+\tfrac{\nu}{16\Theta'}\Bigr\},\qquad
C'_b=2n_I(2M\Theta+1)^d\Bigl[(2d)^d+\Bigl(\tfrac{8de}{\nu}\Bigr)^d\Bigr].
\]
The constants depend only on \(d,M,\nu,n_I,\theta\). In particular they do not depend on the sizes \(D_Q\), on the number or positions of the holes, or on the volume.

*Proof.* Fix \(\rho\) of birth \(b\). Write \(d_s=d_g(x_{i_s},\cup X_\rho)\), \(\delta=\delta_b(F_\rho)\) and \(u=\delta+2\).

*Step 1.* As in [Hidden components]: \(|\partial_{i_1}\cdots\partial_{i_m}F_\rho(z)|\le(m-1)!\,2^{m-1}w_\rho P^{-m}e^{-\nu\max_sd_s}\).

*Step 2.* By Lemma C3(1),(3):
\[
|x_{i_1}-x_{i_s}|_\infty\le\operatorname{dist}_\infty(x_{i_1},\cup F)+\operatorname{diam}_\infty(\cup F)+\operatorname{dist}_\infty(x_{i_s},\cup F)\le Mu+2M\Theta\max_sd_s.
\]
Since \(2\chi M\Theta\le\nu/2\),
\[
e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}e^{-\nu\max_sd_s}\le e^{\chi Mu}e^{-\frac\nu4d_1}\prod_{s\ge2}e^{-a d_s},\qquad a=\frac{\nu}{4(m-1)}.
\]

*Step 3.* By Lemma C3(1), a site with \(d_g(x_i,\cup X_\rho)\le t\) lies within sup-distance \(M\Theta t\) of \(\cup F\), hence in a cube of side \(Mu+2M\Theta t\). So
\[
N(t)\le n_I(Mu+2M\Theta t+1)^d\le n_I(2M\Theta+1)^d(u+1+t)^d,
\]
using \(\Theta\ge1\). The rest of [Hidden components] Step 3 is unchanged with \(2M+1\) replaced by \(2M\Theta+1\):
\[
\sum_{i_2,\dots,i_m}(\cdots)\le\frac{w_\rho}{P^m}C_b'^{\,m-1}((m-1)!)^{d+1}e^{(\chi M+1)u+1}e^{-\frac\nu4d_1}.
\]

*Step 4.* For \(a\in q_\rho\), Lemma C3(2) gives \(d_1\ge(d^{(b)}(x_{i_1},a)-\delta-2\sqrt d)/\Theta'\). So
\[
e^{-\frac\nu4d_1}\le e^{\frac{\nu}{4\Theta'}(\delta+2\sqrt d)}e^{-\frac{\nu}{4\Theta'}d^{(b)}(x_{i_1},a)}.
\]
The total coefficient of \(\delta\) is \(\chi M+1+\nu/(4\Theta')\le\nu/2+1\). The constant is \(\le e^{2(\chi M+1)+1+\nu\sqrt d/(2\Theta')}\le e^{3+\nu/2+\nu\sqrt d/(2\Theta')}\). Fix the points \(a_q\in q\cap\overline{\{g\le b\}}\) once and for all, and sum first over the records with a given anchor.

*Step 5.* This is [Hidden components] Step 5 with \(c=\nu/(4\Theta')\). By Lemma C1 and (C.2), \(d^{(b)}(x,a_q)\ge\frac12\sum_{n=b+1}^{K-1}\omega_n+\frac12|x-a_q|_\infty/M\). The anchor count is \(\le(3(j+1))^dL^{d(K-b)}\) per shell \([jM,(j+1)M)\). (C.4) with this \(c\) turns \(L^{d(K-b)}e^{-\frac c2\sum\omega_n}\) into \(\Gamma_b\). \(\square\)

**Remarks.**

1. With \(H_\rho=\emptyset\) for all records, Theorem C′ is Theorem C with \(\theta\) irrelevant.
2. Under the literal reading (holes \(=Q\), \(F=X\setminus\bigcup Q\), shell in \(F\)), [Hidden components]'s Theorem C applies without (Col). Theorem C′ covers both readings at the price of (Col).
3. (Col) cannot be dropped under (W). Take a record \(Q\cup\{c\}\), \(c\) touching \(Q\), with weight \(w\), and two sites at graded distance \(O(1)\) from \(Q\) on opposite sides. The mixed derivative is \(\asymp w\) under (Loc′) saturated, while \(|x_i-x_l|\ge s_bD_Q\). So the \(\chi\)-weighted row is \(\gtrsim we^{\chi s_bD_Q}\), which is unbounded in \(D_Q\) at fixed \(b\). This is the "hidden carrier distance" of the completion test. Under (W) it is controlled only by a collar.

### 2.4 Prop. B2′ (rooted counting at an exterior cube)

Let \(K_d=4\cdot9^d\) and \(\kappa'_{\rm cnt}(d)=2^{d+1}\log K_d+\log2\) (\(\approx326.3\) for \(d=4\)). Assume (H-sep). Let \(\mathcal P\) be the set of pairs \((F,H)\): \(F\neq\emptyset\) a finite set of \(\mathcal G_b\)-cubes, \(H\subset\mathcal Q_b\) with (Att), no cube of \(F\) in \(\cup H\). Let \(w:\mathcal P\to[0,\infty)\) with \(w(F,H)\le We^{-a\delta_b(F)}\), and \(a-\vartheta\ge\kappa'_{\rm cnt}(d)\). Then for every cube \(q\),
\[
\sum_{(F,H)\in\mathcal P:\ q\in F}w(F,H)\,e^{\vartheta\delta_b(F)}\le4\,W\,K_d^{\,3\cdot2^d}.
\tag{B2′}
\]

*Proof.* Fix \(j\ge0\) and consider the pairs with \(\delta_b(F)\in[j,j+1)\). Choose a tree \(T\) meeting all cubes of \(F\) with \(|T|<s_b(j+1)\). Let \(N(T)\) be the set of grid cubes meeting \(T\).

1. **Size of \(N(T)\).** The proof of Lemma A3 bounds the number of all cubes meeting \(T\), so \(|N(T)|<2^d(2j+3)=:n_j\).
2. **\(N(T)\) is \(*\)-connected** (cubes adjacent if they share a point). If \(N(T)=N_1\sqcup N_2\) with no cube of \(N_1\) touching a cube of \(N_2\), then \(T\cap\cup N_1\) and \(T\cap\cup N_2\) are disjoint, closed and nonempty, and they cover \(T\). That contradicts the connectedness of \(T\).
3. **Counting \(N\).** By the DFS argument of Lemma A4 with \(3^d-1\) neighbours, the number of \(*\)-connected sets of \(n\) cubes containing \(q\) is \(\le(3^d-1)^{2(n-1)}\le9^{dn}\).
4. **Choices of \(F\subset N\):** \(\le2^n\).
5. **Choices of \(H\).** If two holes both had a cube touching the same cube \(c\in F\), they would be at index distance \(\le2\), contradicting (H-sep). So at most \(|F|\le n\) holes satisfy (Att) for \(F\), and \(H\) has \(\le2^n\) choices.

Hence the number of pairs with \(q\in F\) and \(\delta_b(F)\in[j,j+1)\) is \(\le\sum_{n\le n_j}K_d^{\,n}\le2K_d^{\,n_j}\). Therefore
\[
\sum\cdots\le\sum_{j\ge0}2We^{-(a-\vartheta)j}K_d^{\,2^d(2j+3)}=2WK_d^{\,3\cdot2^d}\sum_j\bigl(K_d^{\,2^{d+1}}e^{-(a-\vartheta)}\bigr)^j\le4WK_d^{\,3\cdot2^d}.\qquad\square
\]

**Remarks.**

1. There is no shell gain \(e^{-\tau S}\), and also no attachment factor, because the sum is **rooted at an exterior cube**.
2. The attachment entropy appears only when one roots at the hole. By (Att), every pair with \(Q\in H\) has a cube of \(F\) touching \(Q\). Summing (B2′) over those cubes gives
\[
\sum_{(F,H):\,Q\in H}w\le4WK_d^{3\cdot2^d}\,N_{\rm att}(Q),\qquad N_{\rm att}(Q)=\#\{c\notin Q:\ c\ \text{touches}\ Q\}.
\]
For a box of side \(n\), \(N_{\rm att}=(n+2)^d-n^d\). This is the component-incidence load under (W). It grows like \(R^{d-1}\) (§4).

### 2.5 Theorem E′ conditional

The setting is the step \(k\to k+1\) as in [Hidden components] §6.1 (\(K=k+1\), grades from \(\{\Omega_n\}\), sites on the free bonds of \(\Lambda_{k+1}\)).

- **P1′ (representation; weaker than P1).** The current-dependent part of the inherited-B and retained-component boundary action is \(\sum_\rho F_\rho(z)\) over records as in §2.1, at most one per \((b,F,H)\). The holes of birth \(b\) are the retained (second-class) components of the R step at scale \(b\), with (H-sep). The bound is \(w_\rho\le W_be^{-\kappa_*\delta_b(F_\rho)}\). *No halo, shell or connectivity requirement.* The bound must charge every cube of the carrier outside whole holes (§1.4). P1′ includes SC (§4) wherever the representation itself relies on an exponentiation around retained components.
- **P2′.** (Loc′) with the full carrier, the current graded distance, and \(P\) a fixed multiple of \(P_k\).
- **P3′.** (Geo) with \(c=\nu/(4\Theta')\). Every record has an anchor cube in \(F_\rho\) meeting \(\overline{\{g\le b\}}\). For a record with holes, the exterior cubes that touch a hole meet \(\overline{\{g\le b\}}\), and one of them is chosen. Sites have density \(n_I\).
- **P4 = (Col).** With a constant \(\theta>0\) independent of \(k\), \(b\) and the history.

**Theorem E′.** Assume P1′–P3′, P4, \(0\le\chi\le\nu/(4M\Theta)\), and \(a:=\kappa_*-\nu/2-1\ge\kappa'_{\rm cnt}(d)\). Then for all \(m\ge1\) and \(z\in D_{P/2}\),
\[
\sup_{i_1}\sum_\rho\sum_{i_2..i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}|\partial_{i_1}\cdots\partial_{i_m}F_\rho(z)|\le\frac{4K_d^{3\cdot2^d}C'_aC_b'^{\,m-1}((m-1)!)^{d+1}}{P^m}\sum_{b\le k}\Gamma_bW_b.
\tag{E′.1}
\]

*Proof.* Records with a given anchor \(q\) are among the pairs \((F,H)\) with \(q\in F\). So Prop. B2′ with \(\vartheta=\nu/2+1\) gives \(\mathcal A'_b(\nu/2+1)\le4W_bK_d^{3\cdot2^d}\). Now apply Theorem C′. \(\square\)

**Uniformity.** The constants depend on \(d,L,M,\nu,n_I,\gamma,C_0,\kappa_*,\theta\) only. Hidden holes enter only through \(\theta\). The sum over births converges if \(W_b\) is subexponential in the age. (E′.1) holds under **either** reading of (1.68): under the literal one, \(w\le We^{-\kappa_*\delta(E)}\le We^{-\kappa_*\delta(F)}\) because \(E\supseteq F\).

### 2.6 Source support for P4 additional assumption

1. Holes are retained components, which "are still large field domains" (p.391). While they persist they lie in the large-field region, hence in \(\Omega_{b+1}^c\), and at later steps in \(\Omega_K^c\).
2. When a later R step completes a component containing a hole, the records carrying that hole are integrated there. They become "old records" of Theorem D/Prop. D3′, not current records.
3. The diameter of an eligible component is at most \(100MR_b\), so \(D_Q\le100R_b+1\) (S1, quoted in [Hidden components]).
4. The current sites lie in \(\Omega_K\subset\Omega_{b+1}\). By S11 (CMP119 pp.264–269), \(\Omega_{b+1}^c\) contains \(Z_b\) enlarged by at least four layers of \(MR_{b+1}\)-cubes of scale \(b+1\). That is physical width \(\ge4LMR_{b+1}h_b\), lying in grade \(\le b\), so graded width \(\ge4LR_{b+1}\).
5. With \(R_b\le(L+1)R_{b+1}\) (CMP119 (2.9), as quoted in [Hidden components]),
\[
\theta\ \ge\ \frac{4LR_{b+1}}{100R_b+1}\ \ge\ \frac{4L}{(L+1)(100+1/R_b)}\ \gtrsim\ \frac1{30}.
\]

This is a reading in the source and has not been as stated in the source of pp.264–269. The "four layers" count is the item to check.

## 3. GP reduced to one identification

### 3.1 Lemma G1 (lattice scaled distance vs graded distance)

Let \(\{B^j\}\) be the regions of a determining sequence with mesh \(h_j\) on \(B^j\) (current units). Let \(d_*\) be the CMP96 (2.46) distance, i.e. the infimum over admissible lattice contours of \(\sum_jh_j^{-1}|\Gamma\cap B^j|\). Let \(g^+(x)=\max\{j:x\in\overline{B^j}\}\) (coarse convention on interfaces), and let \(d_{g^+}\) be (C.1) with local unit \(Mh_{g^+(x)}\). Then
\[
d_*(y,y')\ \ge\ M\,d_{g^+}(y,y').
\]

*Proof.* An admissible contour is a continuum path whose bonds have Euclidean length equal to their lattice length. A bond counted in \(B^j\) consists of points \(x\in\overline{B^j}\), so \(g^+(x)\ge j\) and \(h_{g^+(x)}\ge h_j\). Hence \(h_j^{-1}|{\rm bond}|\ge\int_{\rm bond}|dx|_2/h_{g^+(x)}=M\ell_{g^+}({\rm bond})\). Sum over the bonds and take the infimum. \(\square\)

By §1.1, Theorems C and D of [Hidden components] (with \(\tau\) defined through closures) and Theorem C′ hold verbatim for \(g^+\).

### 3.2 Lemma G2 (GP from the identification) conditional

Inputs:

- **(GP-i)** The scaled distance in (1.66) is the CMP96 (2.46) distance \(d_*\) of the determining set \(\mathbf B''_k(Y_1)\). Status additional assumption. Supporting facts:
  - F2 above.
  - The four functions listed on p.376 decay in the scaled distance of their own determining sets (CMP96 Prop. 2.2, CMP99, source).
  - Of these functions, only \(\mathbf H(\mathbf B''_k(Y_1),\cdot)\) is defined on all of \(Y_1\), so it is the only one that connects \(X\) to the boundary layer of \(Y_1\); see [Hidden components] §5.4.
- **(GP-ii)** On \(\overline{Y_1^0}\) the regions of \(\mathbf B''_k(Y_1)\) are those of the prepared sequence \(\{Z''_j\}\). Hence the coarse-convention grades agree there: \(g^+_*=g''\) on \(\overline{Y_1^0}\). Source: p.373 "\(Y_1^0\) is the domain on which the determining sets \(\mathbf B''_k(Y_1)\) and \(\mathbf B''_k\) coincide" (source; [Hidden components]: source), together with LFR I (1.10)–(1.12) (source, [Hidden components]).
- **(GP-iii)** Every point of \(\overline{Y_1\setminus Y_1^0}\cup\partial Y_1^0\) can be joined to \(\mathbb R^d\setminus Y_1\) by a path of \(g''\)-graded length \(\le c_{\rm BL}\). Reading "a boundary layer … of the width \(2M_1\) at most, for the corresponding scale" (p.373) as \(2M_1\) lattice spacings of the local mesh gives \(c_{\rm BL}=2\sqrt d\,M_1/M\).

**Lemma G2.** Under (GP-i)–(GP-iii), let \(Z_1\subset Y_1\) be the eligible component, \(X\subset Y_1\), \(A\subset Y_1\setminus Y_1^0\), and \(1\le b\le k\). Then
\[
d_*(A,\cup X)\ \ge\ M\bigl[d^{(b)}_{g''}(\cup X,\mathbb R^d\setminus Z_1)-c_{\rm BL}\bigr].
\]
So GP holds with \(c_{\rm GP}=M\) and \(C_{\rm GP}=Mc_{\rm BL}=2\sqrt dM_1\).

*Proof.* Take an admissible contour \(\gamma\) from \(x\in\cup X\) to a point of \(A\). Let \(t^*\) be the first time \(\gamma\) meets \(\overline{\mathbb R^d\setminus Y_1^0}\); \(t^*\) exists because \(A\cap Y_1^0=\emptyset\). The prefix \(\gamma|_{[0,t^*]}\) lies in \(\overline{Y_1^0}\). By Lemma G1 and (GP-ii), \(\ell_*(\gamma)\ge\ell_*(\gamma|_{[0,t^*]})\ge M\ell_{g''}(\gamma|_{[0,t^*]})\). The point \(\gamma(t^*)\) lies in \(\partial Y_1^0\), or in \(\overline{Y_1\setminus Y_1^0}\) if \(t^*=0\). By (GP-iii), \(d_{g''}(\gamma(t^*),\mathbb R^d\setminus Y_1)\le c_{\rm BL}\). So
\[
d_{g''}(x,\mathbb R^d\setminus Y_1)\le\ell_{g''}(\gamma|_{[0,t^*]})+c_{\rm BL}.
\]
Finally, \(\mathbb R^d\setminus Y_1\subset\mathbb R^d\setminus Z_1\), and \(d^{(b)}\le d_{g''}\) because capping enlarges the unit. Take the infimum over \(\gamma\) and \(x\). \(\square\)

**What GP now rests on.** The triangle-inequality part is proved. What remains is (GP-i): *which* scaled distance (1.66) uses. GP-ii is a source fact, stated by [Hidden components], and GP-iii is a reading of a width. the finite-cutoff construction per-map question is therefore reduced to a one-line identification, and the only plausible alternative to (GP-i) is that the distance is the flat one of \(\mathbf B_k\) or \(\mathbf B''_k\) restricted to coarse scales. [Hidden components] §5.4 shows that the flat alternative would make the source's own sum over \(j\) at fixed \(Y\) diverge. That argument is in the source's favour but is not a proof.

### 3.3 Corollary G3 (the lattice factor removes the layer count) conditional

In (1.66) the remaining factor after extraction is \(e^{-\frac12\delta d_*(\cdots)}\) (p.376 bottom, source). With Lemma G2, Prop. D3 of [Hidden components] applies with \(c_1=\beta\kappa\) and \(c_2=\delta M/2\), up to the constant factor \(e^{\delta Mc_{\rm BL}/2}=e^{\delta\sqrt dM_1}\). Its hypothesis \(L^de^{-c\omega}\le\frac12\), with \(c=\min(c_1,c_2)/2\), holds for **every** layer of width \(\omega\ge1\) own \(M\)-cube as soon as
\[
\min\bigl(\beta\kappa,\ \delta M/2\bigr)\ \ge\ 2(d\log L+\log2).
\tag{G3}
\]

- Old layers have \(\omega\ge3LR\) or \(10LR\) ([Hidden components] §5.3).
- Prepared layers have width one \(M\)-cube of scale \(j+1\), i.e. \(\omega=L\) in grade-\(j\) units, or \(\omega=1\) if that layer carries grade \(j+1\) (S10). Either way \(\omega\ge1\).

So the "three layers" count that [Hidden components] read in the source is no longer needed. Moreover, (D1) holds for the prepared grades too. Theorem D can therefore be applied with \(N_0=0\) **for those births whose anchors are grade-faithful** (D3). For recent births [Hidden components]'s depth argument (D4) is still used.

Condition (G3) requires the decay rate \(\delta\) in (1.66) not to degrade with \(M\). In CMP96 the rate \(\delta_0\) comes from the local operators \(G'(\square)\) ((2.43), source) and Prop. 2.2 requires only "\(M\) sufficiently large". That is (source input; source) for CMP96. For the LFR II constant \(\delta\) it is additional assumption.

The same lattice factor applies to P2: if the kernels decay like \(e^{-\delta_0d_*}\), then (Loc) holds with \(\nu=\delta_0M\), and (Geo) is easy even with thin layers.

### 3.4 Prop. D3′ (old records with holes) conditional

Old records inside an eligible component may carry holes from earlier R steps. In the setting of Prop. D3 of [Hidden components], let each record have exterior \(E_\rho\), holes \(H_\rho\) with (Att), and anchor in \(E_\rho\). Assume the **interior collar** \(d^{(b)}(\cup Q,\mathbb R^d\setminus Z)\ge\theta_{\rm in}D_Q\) for every hole. Assume also
\[
\Phi_\rho\ge c_1\delta_b(E_\rho)+c_2d^{(b)}(\cup X_\rho,\mathbb R^d\setminus Z).
\]
Then (D.3) holds with \(c_2\) replaced by \(c_2/(1+\sqrt d/\theta_{\rm in})\) and with the rooted norm taken in \(\delta_b(E_\rho)\).

*Proof.* Let \(p\) be a point of \(\cup X_\rho\) nearest to \(Z^c\) in \(d^{(b)}\). If \(p\) lies in a hole \(Q\), the collar gives \(\theta_{\rm in}D_Q\le d^{(b)}(\cup X,Z^c)\). The path \(p\to\)(touching exterior cube)\(\to\)anchor has capped length \(\le\sqrt dD_Q+\delta+2\sqrt d\), exactly as in Lemma C3(2). Hence \(d^{(b)}(a_\rho,Z^c)\le(1+\sqrt d/\theta_{\rm in})d^{(b)}(\cup X,Z^c)+\delta+2\sqrt d\). Continue as in [Hidden components]. \(\square\)

**Source support additional assumption.** A hole retained at step \(b\) inside the component \(Z\) of step \(k>b\) is surrounded by at least ten layers of \(MR_{b+1}\)-cubes added at step \(b+1\) (S1(i), LFR I p.177, quoted in [Hidden components]). That gives \(\theta_{\rm in}\ge10LR_{b+1}/(100R_b+1)\gtrsim1/12\).

## 4. SC: the convergence of the exponentiation around retained components

**Lemma 4.1.** Under (W) and (H-sep), for one retained component \(Q\),
\[
\sum_{Y\supset Q^\sim,\ Y\setminus Z^\sim\ne\emptyset}\alpha e^{-(1+2\beta)\kappa\,\delta_M(Y\setminus Z^\sim)}\ \le\ 4\alpha K_d^{3\cdot2^d}N_{\rm att}(Q^\sim)
\]
if \((1+2\beta)\kappa\ge\kappa'_{\rm cnt}(d)\), where \(N_{\rm att}(Q^\sim)=(n+2)^d-n^d\) for a box \(Q^\sim\) of side \(n\).

*Proof.* Apply Prop. B2′ with holes \(Q^\sim\) and \(F=Y\setminus Z^\sim\). (H-sep) holds for the \(Q^\sim\) when the components are \(\ge5\) cubes apart, e.g. \(R_k\ge5\) by S2. Sum over the cubes \(q\) touching \(Q^\sim\): every admissible \(Y\) has such a cube in \(F\), by (Att). \(\square\)

**Diagnosis additional assumption.** Under (W), Lemma 4.1 is the best the printed bounds give: they do not exclude that a fixed fraction of the \(N_{\rm att}\) attachment positions carries terms of size \(\asymp\alpha e^{-c\kappa}\). All polymers containing a fixed retained component \(Y_i\) are pairwise incompatible, because they overlap in \(Y_i\). The standard cluster-expansion criterion (Kotecký–Preiss with \(Y_i\) as a shared vertex) then needs
\[
\sum_{X'\supset Y_i}|F(X')|e^{a(X')}\le a(Y_i),\qquad a(X')\ge a(Y_i),
\]
hence \(\sum_{X'\supset Y_i}|F(X')|\le\sup_{a>0}ae^{-a}=1/e\). Under (W) the printed bounds give only \(C\alpha R_k^{d-1}\). The source's sentence on p.391 ("this bound is enough for the convergence … such factors are not needed, because there are no summations over these domains") is correct **under the literal reading**, where the sum is \(\le e^{-\tau S_{\min}}\). Under (W) it requires
\[
\textbf{(SC)}\qquad \text{either (1.68) holds literally (shell charged), or } \alpha_k\,R_k^{\,d-1}\le c_{\rm SC}\ \text{for a small absolute } c_{\rm SC}.
\]

For the first-class components the analogous sum is harmless, because of the factor \(e^{-2p_0(g_k)/(1+\beta_0)}\) in (1.92) and \(R_k=\mathrm{polylog}(g_k^{-1})\). In the bracket of (1.103) the source states that this factor is replaced by \(e^3\) per \(Y_i\subset X'\), so SC is genuinely needed there.

The printed \(\alpha\) "can be chosen arbitrarily small for \(\gamma\) small enough" (p.377). It is uniform in \(k\) and does not visibly carry a power of \(g_k\). In CMP119 (2.42) the constant is \(B_0\) and the smallness comes from \(e^{-\kappa d}\) (p.263). So the second alternative of SC is not supplied as printed. To settle SC one would have to:

- (a) find a mechanism in LFR II pp.376–377 that charges the shell. There is no identifiedne.
- (b) Or show that the boundary terms have amplitude \(\le Cg_k^{c}\), or carry the large-field factor of their component.
- (c) Or restructure the alternative representation so that polymers attached to a retained component at different surface points are compatible. One way is to expand \((\mathbf T'_k(Y_i)1)^{-1}\mathbf T'_k(Y_i)\) locally along \(\partial Y_i\), with a decoupling expansion inside \(Y_i\). That is a real construction, not a citation.

SC affects the **values** (P1′), not Theorems C′ and E′, which take the records as given.
