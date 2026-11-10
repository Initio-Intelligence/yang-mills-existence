# Multiscale incidence and logarithmic jets

These estimates concern current-rooted derivatives on a specified conditional law. Use the [retained coordinates and Haar factors](retained_coordinates.md), including clause (2″), throughout. The purely native derivatives, retained-data derivatives, and current-independent outer density are separate. For collared box estimates the [two-layer constraint](local_test_estimates.md) is required. A statement about a single holed record does not control overlapping records at a T step; the collective crossing estimate is open. See [external branches](holed_ancestors.md).

**Propagation hypothesis.** Any use of a T-step bound on a holed ancestor requires the conditional single-ancestor estimate and, for connected products, a separate collective crossing estimate. An argument from the diameter of the union of paid components alone is invalid.

## 2. What (M2) asks, and the fork

### 2.1 The statement in [Boundary estimate d]

[Boundary estimate d] §2.2 defines, for the family \(\mathcal E_1=\bigsqcup_v\mathcal E_1(v)\) of single-kernel records,
\[
\textbf{(M2)}\qquad\mathcal A'_j(\vartheta):=\sup_{q\in\mathcal G_j}\ \sum_{e\in\mathcal E_1:\ j_e=j,\ q\in F_e}w_e\,e^{\vartheta\delta_j(F_e)}\ \le\ \mathfrak a\,W_j\qquad(\vartheta=\nu+1),
\]
and §2.3 Remark 3 fears that for \(j\gg b\) a fixed exterior \(F\) of \(\mathcal G_j\)-cubes carries one record for each of the \(\sim L^{d(j-b)}\) old tags it touches.

### 2.2 Which kernels are live: the fork

Fix the step \(k\to k+1\). Before the R step at \(k\), every earlier tag \(Y\) (a retained component of an R step at \(b<k\)) that has not been consumed in between lies in the large-field region \(Z_k\), because \(Z_{j+1}=\Lambda_{j+1}^c\supseteq\Lambda_j^c=Z_j\) by (2.1) (G1) and "The new large field region is equal to \(Z_k\cup\bigcup Y_i\)" (LFR II p.390, as quoted in [Boundary estimate c] Q9). Let \(C\) be the component of \(Z_k\) containing \(Y\). By G6 there are exactly three cases.

1. \(C\) is eligible and processed at \(k\). Its operation \(\mathbf T_k(C)\) contains the old operation of \(Y\) (G6, (1.2)); the R step integrates it and produces one new operation \(\mathbf T'_k(C)\). The old tag is **consumed**. Every term whose domain meets \(C\) is re-expressed with a domain in \(\mathbf D_k\) containing \(C\) (LFR II p.373, [Boundary estimate c] Q1), i.e. has birth \(k\).
2. \(C\) is not eligible. \(\mathbf T_k(Z_k\cap Z^c)\) is untouched (G6).
3. \(C\) is eligible but its preparation is stopped (the PF sector, [U17] AV; not examined here). The deep operation is retained ([U17] OT.5).

[Boundary estimate d] premise #2 reads: "**(Frz)** Internal variables of non-eligible components are retained data in the current law." The integration variables of the old operation of \(Y\subset C\) are internal variables of \(C\). So:

> **Fork A (literal (Frz)).** In cases 2 and 3 the kernel variables \(\omega_Y\) of every earlier tag \(Y\subset C\) are retained data, like all other internal variables of \(C\). Then at step \(k\) the only kernels that are integrated in the current law are the operations \(\mathbf T'_k(Y_i)\) of the second-class components of the R step at \(k\) itself.

> **Fork B (hybrid).** The internal variables of \(C\) are retained **except** the kernel variables of earlier completed tags inside it, which are integrated in the current law. This is the law one gets if the finite-cutoff construction conditional law (in which completed components were integrated at birth through LFR II (1.103)–(1.104), so that their variables are not part of the retained data) is kept, and only the exponentiation at birth is replaced by Route A.

[Boundary estimate d] works in Fork B (§1.7: "Under Route A its kernel is still unintegrated, and records born at later scales may depend on its variables") while stating (Frz) in a form that gives Fork A. The two laws are different conditional laws (different retained \(\sigma\)-algebras). Both are legitimate; the choice is a statement about what C-06, C-08 and H-03 consume.

- Under Fork A the retained data are finer. Uniform bounds for the finer conditional law pass to uniform bounds on conditional moments of the coarser one by averaging, but statements about *cumulants* or *coercivity* of the coarser law do not follow by averaging (law of total covariance). The outer law then has to control the dependence on \(\omega_Y\), exactly as it has to for the other frozen variables of non-eligible components ([Boundary estimate d] §1.8 assigns this to H-02).
- Under Fork B the C-01 law is unchanged but the incidence problem of §4 has to be solved.

The needed incidence hypothesis depends on whether one inserts a single birth or all births at once; the two cases are distinguished below.

## 3. Fork A: (M2) is the single-birth statement

### 3.1 Proposition (the coarse format has no multiplicity in \(\mathcal E_1\))

Let the records of birth \(j\) be indexed by their carriers, at most \(m_0\) per \((j,X)\) with \(X\) a finite set of \(\mathcal G_j\)-cubes, with \(w\le W_je^{-\kappa_*\delta_j(X)}\) and \(\kappa_*-\vartheta\ge\kappa'_{\rm cnt}(d)\). Call a record single-kernel if it depends on the variables of exactly one live kernel. Then, for the family of single-kernel records with \(F_e:=X_e\),
\[
\sup_{q\in\mathcal G_j}\sum_{e:\ j_e=j,\ q\in X_e}w_e\,e^{\vartheta\delta_j(X_e)}\le4m_0K_d^{3\cdot2^d}W_j.
\]
*Proof.* Each \((j,X)\) contributes at most \(m_0\) records in total, whatever kernels they depend on. Apply [Boundary estimate b] Prop. B2′ with \(H=\emptyset\). \(\square\)

So with the printed indexing (G3), (M2) is not an open problem. What is open is the complement: records that depend on two or more kernels (§4).

### 3.2 Theorem A conditional

**Premises.** (Frz) in the literal form of Fork A. **(Cons)**: case 1 of §2.2 (source: G6 in the source; LFR II p.373 and p.390 via [Boundary estimate c]). **(H-sep\(_k\))**: the components of the eligible union at step \(k\) are pairwise at \(\ell^\infty\) index distance \(\ge\rho_k\ge3\) in \(\mathcal G_k\) (source: [Hidden components] S2, additional assumption). (M1) with \(m_0\); \(w_e\le W_ke^{-\kappa_*\delta_k(F_e)}\).

**Theorem A.** Under these premises, at the step \(k\to k+1\):

1. every live kernel \(v\) has birth \(b_v=k\), and every record \(e\) with \(I_e\ne\emptyset\) has birth \(k\); all other records are kernel-free (sector S1), with the frozen \(\omega\) among their parameters;
2. (M2) holds: \(\mathcal A'_k(\vartheta)\le4m_0K_d^{3\cdot2^d}W_k\) for \(\kappa_*-\vartheta\ge\kappa'_{\rm cnt}(d)\), and \(\mathcal A'_j=0\) for \(j\ne k\);
3. Theorem R6 of [Boundary estimate d] applies in its single-birth case (\(j_e=b_v=k\), (Col\(_j\)) = (Col\(_k\))), with \(\mathfrak S=\Gamma_k(\mathfrak aW_k+m_1s_*)\), \(\Gamma_k=L^de^{C_0}\) (here \(K=k+1\)).

*Proof.* (1) By §2.2 an earlier tag is consumed, or lies in a component whose internal variables are retained. A record depending on \(\omega_v\) for a birth-\(k\) kernel has a domain meeting the component, hence was re-expressed at the R step (Cons). (2) [Boundary estimate b] Prop. B2′ in the grid \(\mathcal G_k\); (H-sep\(_k\)) is its hypothesis. (3) Substitution. \(\square\)

Under Fork A the birth-summed generality of R6, Lemma NE.3 for later births, and the whole of (M2) "for later births near dense old tags" are not needed. What remains of the retained-tag sector is [Boundary estimate c] Theorem R1, Prop. R3, Cor. R5 and the multi-kernel remainder \(Z_2\).

### 3.3 Proposition W (weighted component load, one birth)

This is the weighted form of [Boundary estimate c] Prop. R4 that [Boundary estimate c] §3.4 and [Boundary estimate d] #13 list as open.

**Setting.** That of [Boundary estimate c] Prop. R4: holes of one birth in the grid \(\mathcal G_b\), pairwise index distance \(\ge\rho\ge3\); hole diameters \(D_Q\le D_{\max}\) (in cubes). Each \(e\in\mathcal E_2\) has a hole set \(H_e\), \(|H_e|\ge2\), an exterior \(F_e\) containing for each \(Q\in H_e\) a cube touching \(Q\), \(\sup|V_e|\le We^{-\kappa_*\delta_b(F_e)}\), at most \(m_0\) per \((F,H)\). Define the extent \(\ell_e:=s_b^{-1}\operatorname{diam}_\infty(\cup X_e)\), \(X_e=F_e\cup\bigcup H_e\).

**Proposition W.** (i) \(\ell_e\le\delta_b(F_e)+2+2D_{\max}\), and for interactions \(e_1,\dots,e_n\) such that consecutive ones share a hole, \(\operatorname{diam}_\infty\bigl(\bigcup_a\cup X_{e_a}\bigr)\le s_b\sum_a\ell_{e_a}\). (ii) Let \(\varrho\ge1\), \(\lambda\ge0\), \(\kappa_2>0\) with \(\kappa_*-\lambda-2^{d+1}\log\varrho-\kappa_2\ge\kappa'_{\rm cnt}(d)\). Then for every hole \(Q\)
\[
\sum_{e\in\mathcal E_2:\ Q\in H_e}\varrho^{|H_e|}\,\sup|V_e|\,e^{\lambda\ell_e}\ \le\ 4m_0\varrho^{2^d}K_d^{3\cdot2^d}\,W\,N_{\rm att}(Q)\,e^{2\lambda(1+D_{\max})}\,e^{-\kappa_2(\rho-3)}.
\]
*Proof.* (i) A point of \(\cup X_e\) lies in \(\cup F_e\) or in a hole touching a cube of \(F_e\), hence within sup-distance \(s_bD_{\max}\) of \(\cup F_e\); and \(\operatorname{diam}_\infty(\cup F_e)\le s_b(\delta_b(F_e)+2)\) ([Hidden components] Lemma A3). Sets that pairwise intersect along a chain have diameter at most the sum of the diameters. (ii) By (i), \(e^{\lambda\ell_e}\le e^{2\lambda(1+D_{\max})}e^{\lambda\delta_b(F_e)}\). Now repeat the proof of [Boundary estimate c] Prop. R4 with \(\kappa_*\) replaced by \(\kappa_*-\lambda\). \(\square\)

**Use conditional.** With the source numbers \(D_{\max}=100R_b+1\), \(\rho\ge R_b\), \(N_{\rm att}\le(100R_b+3)^d\), the right side is \(\le CW\sup_R(100R+3)^de^{4\lambda+3\kappa_2}e^{-(\kappa_2-200\lambda)R}\), which is finite and proportional to \(W\) as soon as \(\kappa_2>200\lambda\). With \(\varrho=eM_{\rm op}\), \(M_{\rm op}=e^{3\Lambda_*}\), this is (R11) of [Rep21] for the system \(Z_2\), with (R10) from (i). The hidden diameter of a tag is paid by the separation of the tags, with rate ratio \(200\). **Not covered:** (R11)–(R12) are stated in [Rep21] for finite current supports \(S_e\subset X_e\). The actual supports have tails; the localization of [Rep21] §5 has to be applied to the dressed kernels \(\Pi'_{v,z}\), and the current-root load \(K_\lambda\) in tail form is then the \(m=1\) case of [Boundary estimate b] Theorem C′. That step is assumed.

## 4. Fork B in the printed format: the incidence is unbounded, and that matters

### 4.1 Example N1 (geometry)

Take any \(b<j\) and \(\omega\ge1\). Let \(c_0\) be a \(\mathcal G_j\)-cube, and put in it \(n\) tags of birth \(b\): boxes of \(\mathcal G_b\)-cubes of side \(20R\) with gaps \(R\) (index distance \(\ge3\) in \(\mathcal G_b\), so (H-sep) holds in the tags' own grid), i.e. \(n=\lfloor L^{j-b}/(21R)\rfloor^d\). Let \(U_m\), \(b<m\le j\), be nested unions of \(\mathcal G_m\)-cubes with layers \(U_m\setminus U_{m+1}\) of width \(\omega s_m\), arranged so that \(U_j\) begins at distance \(\sum_{m=b+1}^{j-1}\omega s_m<\omega s_j/(L-1)\) from \(c_0\). Let \(X\) be \(c_0\) together with a straight row of \(\lceil\omega/(L-1)\rceil+1\) cubes of \(\mathcal G_j\) ending in \(U_j\). Then \(X\in\mathbf D_j\), \(X\cap U_j\ne\emptyset\), \(X\) has a cube in \(\overline{\{g\le j\}}\), and \(d_j(X)\le\omega/(L-1)+2\). All the geometric hypotheses of [Hidden components] §4.1 and of [Boundary estimate d] §2.2 hold, with layer widths \(\omega\) as large as one likes. A record with this carrier is allowed by G3 to depend on the variables of all \(n\) tags. Its weight \(B_0e^{-\kappa(\omega/(L-1)+2)}\) does not depend on \(j-b\); \(n\) grows like \(L^{d(j-b)}\).

With the source's numbers (\(\omega\approx8R_m\), [Boundary estimate c] §5) such a record has weight \(\approx B_0e^{-8\kappa R_j/(L-1)}\): small, but independent of \(n\). The age \(j-b\) of tags inside one non-eligible component is bounded only by \(O(\log D)+R_j\) with \(D\) its diameter ([Boundary estimate d] N3), so \(n\) is unbounded over admissible histories. Whether such configurations have positive weight in the outer law is not a C-05 question (additional assumption: this is not an example of an admitted Wilson history; the statement is that no hypothesis on record excludes them).

### 4.2 Example N2 (a small interaction touching many kernels can produce a zero)

Let \(\mathcal V=\{1,\dots,n\}\), \(\Omega_v=\{\pm1\}\), \(\mu_v\) uniform, one current coordinate \(z\) with \(|z|<P\), \(0<\varepsilon\le\frac1{20}\), and
\[
e^{\sigma_v(z,s)}=1+2\varepsilon s\,z/P,\qquad V(s_1,\dots,s_n)=w\cos(\theta S),\quad S=\sum_vs_v,\ \theta=\arctan\varepsilon,\ w\in\mathbb R.
\]
Then \(N_v\equiv1\), \(\sigma_v(0,\cdot)=0\), the kernels are positive for real \(z\), \(\sup|\sigma_v|\le4\varepsilon\le\frac14\), \(|\partial_z\sigma_v|\le4\varepsilon/P\) (so (Pos), (Resp) and the hypotheses of [Boundary estimate c] Theorem R1 hold with \(s_*=4\varepsilon\)); \(V\) is real, independent of \(z\), \(|V|\le|w|\), and \(|I_V|=n\).

**Claim.** Put \(T=(1+\varepsilon^2)^{n/2}\). If \(T>18\), then \(Z_2(z)=\bigl(\bigotimes_v\Pi_{v,z}\bigr)e^V\) vanishes at \(z=iP/2\) for some \(w\in(-3/T,0)\).

*Proof.* At \(z=iP/2\) the kernel is integration against \(\prod_v\frac12(1+i\varepsilon s_v)\), a complex measure of total variation \(T\). For real \(a\), \(\langle e^{iaS}\rangle=(\cos a-\varepsilon\sin a)^n\). With \(a=\mp\theta\): \(\langle e^{-i\theta S}\rangle=(1+\varepsilon^2)^{n/2}=T\) and \(\langle e^{i\theta S}\rangle=((1-\varepsilon^2)/\sqrt{1+\varepsilon^2})^n\in(0,1)\). So \(\langle\cos\theta S\rangle\ge T/2\). The map \(s\mapsto-s\) conjugates the measure and fixes \(\cos(\theta S)\), so every \(\langle\cos^k(\theta S)\rangle\) is real and \(Z_2\) is real for real \(w\). Also \(|\langle\cos^k\theta S\rangle|\le T\). Hence for \(|w|\le1\), \(Z_2=1+w\langle\cos\theta S\rangle+R\) with \(|R|\le T(e^{|w|}-1-|w|)\le T w^2\). At \(w=-3/T\): \(Z_2\le1-\frac32+\frac9T<0\). \(Z_2=1\) at \(w=0\). \(\square\)

**Meaning.** In the class "normalized kernels with variation \(\le t\) on the polydisc, interactions with sup norm \(\le w\)", zero-freeness of \(Z_2\) forces \(w\lesssim e^{-ct^2n}\) for an interaction touching \(n\) kernels. So the factor \((eM_{\rm op})^{|I_e|}\) in (R11) is of the right nature, and a uniform theorem needs one of: (a) bounded incidence relative to the weight, \(|I_e|\le C\cdot(\text{size charged by }w_e)\); (b) a bound on \(\sum_{v\in I_e}t_v\); (c) a bound on the dependence of \(V_e\) on each \(\omega_v\). The printed format with N1 gives none of them. The multiscale format of §5 gives deduction and conditional.

**What is not claimed.** N2 is a statement about hypothesis classes. In the actual model the response of an old kernel deep in the structure to the current is expected to be exponentially small in the graded depth (this is what Prop. MS-5 proves in the multiscale format). N2 shows that this has to be *proved and used*; a uniform bound \(t_v\le\Lambda_*\), as in [Boundary estimate d] Theorem R6, is not enough for the multi-kernel sector.

## 5. Fork B: the multiscale statement (M2★)

### 5.1 Setting

- **(G1)** \(d\ge1\), integer \(L\ge2\), \(M\ge1\), \(K\ge1\), \(h_n=L^{n-K}\), \(s_n=Mh_n\).
- **(Nest)** \(\mathcal G_n\) (\(1\le n\le K\)) is a tiling of \(\mathbb R^d\) (or of a torus) by closed cubes of side \(s_n\), and every cube of \(\mathcal G_{n+1}\) is the union of \(L^d\) cubes of \(\mathcal G_n\). (Source: G1; the cubes of \(\pi_j\) are the \(M\)-blocks centred at points of the coarser lattice; nestedness for odd \(L\) is additional assumption.)
- **(Seq)** closed sets \(\mathbb R^d=U_1\supseteq U_2\supseteq\dots\supseteq U_K\ne\emptyset\), \(U_{K+1}:=\emptyset\), with \(U_n\) a union of \(\mathcal G_n\)-cubes. \(g(x):=\max\{n:x\in U_n\}\). (\(U_n=\Omega_n\); G1.)
- **(Thick)** for \(1\le n\le K-1\): every \(\mathcal G_n\)-cube that touches \(U_{n+1}\) is contained in \(U_n\). ("Touch" = have a common point. Source: G2 gives width \(2R_n\) cubes for ordinary domains; prepared sequences inside eligible components have one-cube layers, [Hidden components] S10; (d) that these are one cube of the right scale.)
- \(d_g\) and \(d^{(n)}\) are the graded and capped metrics of [Hidden components] (C.1) for this \(g\) (unit \(Mh_{g(x)}\), resp. \(M\max(h_{g(x)},h_n)\)). \(d^{(n)}\le d_g\) and \(|x-y|_\infty\le M\,d^{(n)}(x,y)\).
- \(\omega_m\ge0\) with \(\operatorname{dist}_2(\overline{\mathbb R^d\setminus U_m},U_{m+1})\ge\omega_mMh_m\) (\(2\le m\le K-1\)), and **(Geo)** = [Hidden components] (C.4) with constants \(c,\gamma,C_0\). \(\Gamma_n\) as in [Hidden components] (C.9), and \(\Gamma_\Sigma:=\sum_{n=1}^K\Gamma_n\le1+L^de^{C_0}/(1-e^{-\gamma})\).
- Sites \(x_i\in U_K\), density \(n_I\); polydisc \(D_P\).

**Tiles.** For \(1\le j\le K\),
\[
\mathcal T^{(j)}:=\{c\in\mathcal G_n:\ 1\le n<j,\ c\subset U_n,\ \operatorname{int}c\cap U_{n+1}=\emptyset\}\ \cup\ \{c\in\mathcal G_j:\ c\subset U_j\},
\]
with scale \(\sigma(c)=n\) resp. \(j\). \(\mathcal T:=\mathcal T^{(K)}\), and \(\mathcal T_n\) is the set of tiles of \(\mathcal T\) of scale \(n\). \(\mathcal T^{(j)}\) is the tiling by cubes of the local scale for the truncated sequence \(U_1\supseteq\dots\supseteq U_j\); it is what [III] p.276 calls "cubes in proper scales" at step \(j\). A set of tiles is \(*\)-connected if it is connected under "touch".

### 5.2 Lemmas on the tiling

**Lemma T0.** \(\mathcal T^{(j)}\) covers \(\mathbb R^d\) and its tiles have pairwise disjoint interiors. If \(\sigma(c)=n<j\) then \(g=n\) on \(\operatorname{int}c\), \(g\ge n\) on \(c\), and \(c\in\mathcal T\); if \(\sigma(c)=j\) then \(g\ge j\) on \(c\), and \(c\in\mathcal T\) iff \(\operatorname{int}c\cap U_{j+1}=\emptyset\). Every \(q\in\mathcal T_n\) satisfies \(q\subset\overline{\mathbb R^d\setminus U_{n+1}}\), and \(q\in\mathcal T^{(j)}\) iff \(j\ge n\).

*Proof.* By (Nest), \(U_{n+1}\) is a union of \(\mathcal G_n\)-cubes, so a \(\mathcal G_n\)-cube is contained in \(U_{n+1}\) or has interior disjoint from it. If \(g(x)\ge j\), \(x\) lies in a \(\mathcal G_j\)-cube contained in \(U_j\). If \(g(x)=n<j\), \(x\) lies in a \(\mathcal G_n\)-cube \(c\subset U_n\), and \(c\not\subset U_{n+1}\) since \(x\notin U_{n+1}\). For two tiles of scales \(n\le n'\), the coarser is a union of \(\mathcal G_n\)-cubes, so interiors are disjoint or \(c\subset c'\); the latter with \(n<n'\) gives \(c\subset U_{n'}\subset U_{n+1}\), a contradiction. The rest is read off the definition. \(\square\)

**Lemma T1 (adjacent scales, degree).** (a) If two tiles of \(\mathcal T^{(j)}\) touch, their scales differ by at most one. (b) \(\operatorname{dist}_\infty(U_{n+1},\overline{\mathbb R^d\setminus U_n})\ge s_n\) for \(1\le n\le K-1\); so one may always take \(\omega_m\ge1\). (c) Every tile of \(\mathcal T^{(j)}\) touches at most \(\Delta_*:=(L+2)^d-L^d\) other tiles.

*Proof.* (a) Let \(\sigma(c)=m\), \(\sigma(c')\ge m+2\). Then \(c'\subset U_{m+2}\). The \(\mathcal G_{m+1}\)-cube \(\hat c\supset c\) touches \(U_{m+2}\), so \(\hat c\subset U_{m+1}\) by (Thick), hence \(c\subset U_{m+1}\); but \(m<j\) and \(\operatorname{int}c\cap U_{m+1}=\emptyset\). (b) A point \(y\in\overline{\mathbb R^d\setminus U_n}\) lies in a \(\mathcal G_n\)-cube \(c_y\not\subset U_n\) (local finiteness). If \(|y-u|_\infty<s_n\) with \(u\) in a \(\mathcal G_n\)-cube \(c_u\subset U_{n+1}\), then in each coordinate the two grid intervals are equal or adjacent, so \(c_y\) touches \(c_u\subset U_{n+1}\), and (Thick) gives \(c_y\subset U_n\). (c) Let \(\sigma(c)=n\ge2\) and let \(P\) be the set of \(\mathcal G_{n-1}\)-cubes that touch \(c\) and are not contained in \(c\); \(|P|=(L+2)^d-L^d\). A tile \(c'\ne c\) touching \(c\) has scale \(\ge n-1\) by deduction, so it is a union of \(\mathcal G_{n-1}\)-cubes; the one containing a point of \(c\cap c'\) lies in \(P\) (it is not inside \(c\), interiors being disjoint). Distinct tiles give distinct elements of \(P\). For \(n=1\) the neighbours have scale \(1\) or \(2\) and there are at most \(3^d-1\le\Delta_*\). \(\square\)

**Lemma T2 (counting).** For \(q\in\mathcal T^{(j)}\) and \(m\ge1\), the number of \(*\)-connected \(N\subset\mathcal T^{(j)}\) with \(q\in N\), \(|N|=m\), is at most \(\Delta_*^{2(m-1)}\).

*Proof.* Depth-first traversal of a spanning tree, as in [Hidden components] Lemma A4, with \(\Delta_*\) neighbours. \(\square\)

**Lemma T3 (crossing).** If \(N\subset\mathcal T^{(j)}\) is \(*\)-connected and contains tiles of scales \(n<n'\), it contains a tile of every scale \(n\le m\le n'\); so \(|N|\ge n'-n+1\).

*Proof.* T1(a) along a \(*\)-path. \(\square\)

**Lemma T4 (tiles are short).** For \(c\in\mathcal T^{(j)}\), \(x,y\in c\) and any \(n\): \(d^{(n)}(x,y)\le d_g(x,y)\le\sqrt d\), and \(\operatorname{diam}_\infty c\le s_j\le M\). Hence for \(*\)-connected \(N\subset\mathcal T^{(j)}\): \(d_g(x,y)\le\sqrt d\,|N|\) for \(x,y\in\cup N\), and \(\operatorname{diam}_\infty(\cup N)\le M|N|\).

*Proof.* The segment \([x,y]\subset c\) has Euclidean length \(\le\sqrt d\,s_{\sigma(c)}\), and \(g\ge\sigma(c)\) on \(c\) (T0), so the unit is \(\ge s_{\sigma(c)}\). Chain through common points. \(\square\)

**Lemma C1′.** For \(a\in\overline{\mathbb R^d\setminus U_{n+1}}\) and \(x\in U_K\): \(d^{(n)}(a,x)\ge\sum_{m=n+1}^{K-1}\omega_m\).

*Proof.* [Hidden components] Lemma C1 with the closure convention of [Boundary estimate b] §1.1: for \(n<m<K\) let \(\sigma_m=\sup\{t:\gamma(t)\in\overline{\mathbb R^d\setminus U_m}\}\), \(\tau_m=\inf\{t>\sigma_m:\gamma(t)\in U_{m+1}\}\). On \((\sigma_m,\tau_m)\) the path is in \(\operatorname{int}U_m\setminus U_{m+1}\), so \(g=m\) and the capped unit is \(Mh_m\); the piece has Euclidean length \(\ge\omega_mMh_m\); the pieces are disjoint because points of \((\sigma_m,\tau_m)\) lie outside \(U_{m'}\) for \(m'>m\). \(\square\)

### 5.3 Records, tags, and the premise (MS)

**Tags.** A family \(\mathcal V\); \(v\in\mathcal V\) has a birth \(b_v\), a closed set \(\cup Q_v\), \(\Delta_v=\operatorname{diam}_\infty(\cup Q_v)\), \(D_v=\Delta_v/s_{b_v}\). Let \(\mathcal T(v)\) be the set of tiles of \(\mathcal T\) touching \(\cup Q_v\), and \(n_{\rm att}(v)=|\mathcal T(v)|\).

- **(Tag-1)** every tile of \(\mathcal T(v)\) has scale \(b_v\). (Then \(\cup Q_v\cap U_{b_v+1}=\emptyset\), \(n_{\rm att}(v)\le(D_v+2)^d\), and for every \(j\ge b_v\) the tiles of \(\mathcal T^{(j)}\) touching \(\cup Q_v\) are exactly those of \(\mathcal T(v)\). Source: the tag and its margin of eight \(LMR_{b+1}\)-layers have grade \(b\), [Boundary estimate c] §5; additional assumption for the inside of the tag after the R step.)
- **(Tag-2)** \(\operatorname{dist}_\infty(\cup Q_v,\cup Q_{v'})>s_{\min(b_v,b_{v'})}\) for \(v\ne v'\). (Source gives \(\ge R\,s_{\max}\): [U17] (OT.30), [Hidden components] S2; additional assumption.)
- **(Col)** \(d_g(x_i,\cup Q_v)\ge\theta D_v\) for all sites, \(\theta\in(0,1]\). ([Boundary estimate c] §5, [Boundary estimate d] Lemma NE.3.) \(\Theta=1+1/\theta\), \(\Theta'=1+\sqrt d/\theta\).

**Records (multiscale format).** A record \(\rho\) has a birth \(j\); a finite \(*\)-connected **hull** \(N_\rho\subset\mathcal T^{(j)}\); a finite set \(H_\rho\subset\mathcal V\) of declared holes, each touching a tile of \(N_\rho\), all of birth \(j\); the carrier \(X_\rho=\cup N_\rho\cup\bigcup_{v\in H_\rho}\cup Q_v\); an anchor tile \(q_\rho\in N_\rho\cap\mathcal T\), of scale \(n_\rho\), with \(n_\rho=j\) if \(H_\rho\ne\emptyset\); a set \(I_\rho\subset\mathcal V\) of kernels on whose variables it depends; a weight \(w_\rho\); and \(F_\rho\) holomorphic on \(D_P\) (and measurable in the kernel variables) with
\[
\textbf{(Loc-ms)}\qquad\sup_\omega|\partial_iF_\rho(z,\omega)|\le\frac{w_\rho}{P}\,e^{-\nu d_g(x_i,X_\rho)}.
\]

> **Premise (MS).** At the current step every record of sectors S1–S3 is given in this format, with
> (MS-a) \(I_\rho\subset\{v:\cup Q_v\text{ touches }\cup N_\rho\}\) (dependence only through tiles of the hull);
> (MS-b) \(w_\rho\le W_je^{-\kappa_\bullet|N_\rho|}\), uniformly in the frozen and integrated variables;
> (MS-c) the hull of a birth-\(j\) record contains a tile of scale \(j\) (it meets \(U_j\); G3) and a tile of \(\mathcal T\) (the anchor; G3: \(X\cap Z_j^\sim\ne\emptyset\));
> (MS-d) at most \(m_0\) records share \((j,N,H)\);
> (MS-e) (Loc-ms).

**Status of (MS).** (c) at the localization stage: by G4–G5 the T-step localization is built on proper-scale cubes, each carrying \(e^{-(\kappa_1-1)}\), with dependence restricted to the cubes used. (d) beyond that: the source resums to \(\mathbf D_k\) before the Mayer and cluster expansions ([III] p.277) and before the R-step relocalization, so the multiscale form of the *final* records \(\mathbf B^{(j)}\) is not printed. Producing it means running those expansions with multiscale polymers. Lemmas T1–T2 are the combinatorial input such a construction needs (bounded degree, exponential animal count); the analytic steps are unchanged in kind. This is a construction to be written, comparable in size to [Boundary estimate c] §3.6. Lemma 5.9 below shows that (MS) refines (2.42) and cannot contradict it.

### 5.4 Lemma C3-ms (a record seen from a site)

Let \(\rho\) be a record, \(x=x_i\), \(\Delta=d_g(x,X_\rho)\), \(a\in q_\rho\), \(n=n_\rho\). Assume (Col) if \(H_\rho\ne\emptyset\). Then

1. \(\operatorname{dist}_\infty(x,\cup N_\rho)\le M\Theta\Delta\);
2. \(d^{(n)}(x,a)\le\Theta'\Delta+\sqrt d\,|N_\rho|\);
3. \(\operatorname{diam}_\infty(\cup N_\rho)\le M|N_\rho|\).

(If \(H_\rho=\emptyset\) one may take \(\Theta=\Theta'=1\).)

*Proof.* (3) is T4. Let \(p\in X_\rho\) with \(d_g(x,p)\le\Delta+\epsilon\). If \(p\in\cup N_\rho\): (1) follows from \(|x-p|_\infty\le M(\Delta+\epsilon)\), and (2) from T4 and \(d^{(n)}\le d_g\). If \(p\in\cup Q_v\), \(v\in H_\rho\): then \(n=j=b_v\), and by (Col) \(\Delta+\epsilon\ge\theta\Delta_v/s_n\). Let \(r\in\cup Q_v\cap\cup N_\rho\). Then \(|p-r|_\infty\le\Delta_v\le M(\Delta+\epsilon)/\theta\), which gives (1); the segment \([p,r]\) has Euclidean length \(\le\sqrt d\Delta_v\) and capped unit \(\ge s_n\), so capped length \(\le\sqrt d(\Delta+\epsilon)/\theta\); continue from \(r\) to \(a\) inside \(\cup N_\rho\) by T4. Let \(\epsilon\downarrow0\). \(\square\)

### 5.5 Theorem MS-1 (multiscale root sum)

Put \(\vartheta_0:=1+\nu(1+\sqrt d)/4\) and
\[
\mathcal A^{\rm ms}(\vartheta):=\sup_{q\in\mathcal T}\ \sum_{\rho:\ q_\rho=q}w_\rho\,e^{\vartheta|N_\rho|}\qquad(\text{all births}).
\]
**Theorem MS-1.** Assume §5.1, a family of records as in §5.3 with (Loc-ms), (Col) if some \(H_\rho\ne\emptyset\), \(0\le\chi\le\nu/(4M\Theta)\), and (Geo) with \(c=\nu/(4\Theta')\). Then for every \(m\ge1\), \(i_1\), \(z\in D_{P/2}\) and all values of the kernel variables,
\[
\sum_\rho\sum_{i_2,\dots,i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}\,|\partial_{i_1}\cdots\partial_{i_m}F_\rho(z)|\le\frac{C_a^{\rm ms}(C'_b)^{m-1}((m-1)!)^{d+1}}{P^m}\ \Gamma_\Sigma\ \mathcal A^{\rm ms}(\vartheta_0),
\]
\[
C_a^{\rm ms}=3^dS_d\!\Bigl(\frac{\nu}{8\Theta'}\Bigr)e^{1+\nu/(16\Theta')},\qquad C'_b=2n_I(2M\Theta+1)^d\Bigl[(2d)^d+\Bigl(\frac{8de}\nu\Bigr)^d\Bigr].
\]
The constants depend on \(d,M,\nu,n_I,\theta\) only.

*Proof.* Fix \(\rho\); write \(d_s=d_g(x_{i_s},X_\rho)\), \(u=|N_\rho|\).

*Step 1.* Cauchy on the polydisc of radius \(P/2\), as in [Hidden components] Theorem C Step 1: \(|\partial_{i_1}\cdots\partial_{i_m}F_\rho|\le(m-1)!2^{m-1}w_\rho P^{-m}e^{-\nu\max_sd_s}\).

*Step 2.* By C3-ms(1),(3): \(|x_{i_1}-x_{i_s}|_\infty\le Mu+2M\Theta\max_sd_s\). Since \(2\chi M\Theta\le\nu/2\): \(e^{\chi\max|x_{i_1}-x_{i_s}|}e^{-\nu\max d_s}\le e^{\chi Mu}e^{-\frac\nu4d_1}\prod_{s\ge2}e^{-ad_s}\), \(a=\nu/(4(m-1))\).

*Step 3.* Sites with \(d_g(x_i,X_\rho)\le t\) lie within sup-distance \(M\Theta t\) of \(\cup N_\rho\), hence in a cube of side \(Mu+2M\Theta t\); so \(N(t)\le n_I(2M\Theta+1)^d(u+1+t)^d\). The computation of [Hidden components] Step 3 (with \(2M+1\) replaced by \(2M\Theta+1\), as in [Boundary estimate b]) gives
\[
\sum_{i_2,\dots,i_m}(\cdots)\le\frac{w_\rho}{P^m}(C'_b)^{m-1}((m-1)!)^{d+1}e^{(\chi M+1)u+1}e^{-\frac\nu4d_1}.
\]
*Step 4.* By C3-ms(2), \(e^{-\frac\nu4d_1}\le e^{\frac{\nu\sqrt d}{4\Theta'}u}e^{-\frac{\nu}{4\Theta'}d^{(n_\rho)}(x_{i_1},a)}\) for \(a\in q_\rho\). The coefficient of \(u\) is \(\chi M+1+\nu\sqrt d/(4\Theta')\le\vartheta_0\). For each \(q\in\mathcal T_n\) fix \(a_q\in q\); by T0, \(a_q\in\overline{\mathbb R^d\setminus U_{n+1}}\).

*Step 5.* Sum first over the records with anchor \(q\), then over \(q\in\mathcal T_n\), then over \(n\). The tiles of \(\mathcal T_n\) are distinct cubes of \(\mathcal G_n\), so [Hidden components] Step 5 applies verbatim with \(b=n\) and Lemma C1′: with \(c=\nu/(4\Theta')\),
\[
\sum_{q\in\mathcal T_n}e^{-c\,d^{(n)}(x_{i_1},a_q)}\le e^{c/4}3^dS_d(c/2)\,L^{d(K-n)}e^{-\frac c2\sum_{m=n+1}^{K-1}\omega_m}\le e^{c/4}3^dS_d(c/2)\,\Gamma_n.\qquad\square
\]

The anchors are tiles of the **local** scale. Their multiplicity \(L^{d(K-n)}\) at scale \(n\) is paid by the crossing of the layers \(n+1,\dots,K-1\), as in [Hidden components] Theorem C; the difference is that the index \(n\) is the scale of the anchor, not the birth of the record.

### 5.6 Theorem MS-2 (rooted multiscale norm; this is (M2★))

Let \(\kappa_{\rm ms}:=2\log\Delta_*+2\log2\) (\(\approx15.7\) for \(d=4\), \(L=2\), where \(\Delta_*=1280\)).

**Theorem MS-2.** Assume §5.1, (Tag-2), and (MS-b,c,d) for a family of records. Let \(\vartheta\ge0\) with \(\kappa_\bullet-\vartheta\ge\kappa_{\rm ms}\). Then for every tile \(q\in\mathcal T\) of scale \(n\),
\[
\sum_{\rho:\ q\in N_\rho}w_\rho\,e^{\vartheta|N_\rho|}\ \le\ \frac{m_0}{\Delta_*^2}\sum_{j=n}^{K}2^{-(j-n)}\,W_j\ \le\ \frac{2m_0}{\Delta_*^2}\,\sup_{j\ge n}W_j.
\]
In particular \(\mathcal A^{\rm ms}(\vartheta)\le2m_0\Delta_*^{-2}\bar W\), \(\bar W=\sup_jW_j\).

*Proof.* A record of birth \(j\) has its hull in \(\mathcal T^{(j)}\), and \(q\in\mathcal T^{(j)}\) only if \(j\ge n\) (T0). Fix \(j\ge n\). By (MS-c) and T3, \(|N_\rho|\ge j-n+1\). The number of hulls with \(|N|=m\) containing \(q\) is \(\le\Delta_*^{2(m-1)}\) (T2). By (Tag-2) each tile touches at most one tag of a given birth: two tags of birth \(j\) touching a tile \(c\) are within \(s_{\sigma(c)}\le s_j\) of each other. So \(H\) has at most \(2^m\) choices. By (MS-d) and (MS-b) the sum over birth \(j\) is at most
\[
m_0W_j\sum_{m\ge j-n+1}\Delta_*^{2(m-1)}2^me^{-(\kappa_\bullet-\vartheta)m}\le\frac{m_0W_j}{\Delta_*^2}\sum_{m\ge j-n+1}2^{-m}\le\frac{m_0W_j}{\Delta_*^2}\,2^{-(j-n)}.\qquad\square
\]

**Corollary (S1 in the multiscale format).** Under the hypotheses of MS-1 and MS-2 with \(\kappa_\bullet-\vartheta_0\ge\kappa_{\rm ms}\), the weighted jets of \(\sum_\rho F_\rho\) are bounded by \(2m_0\Delta_*^{-2}C_a^{\rm ms}(C_b')^{m-1}((m-1)!)^{d+1}P^{-m}\,\Gamma_\Sigma\,\bar W\). No relation between the birth of a record and the scale of its anchor is assumed; the sum over births converges at each anchor by tile crossing, without (Geo).

### 5.7 Prop. MS-3 and MS-4 (incidence and kernel-rooted loads)

**Proposition MS-3 (incidence).** Assume (Tag-1), (Tag-2). Every tile of every \(\mathcal T^{(j)}\) touches at most one tag. Hence under (MS-a), \(|I_\rho|\le|N_\rho|\) for every record.

*Proof.* If a tile \(c\) of scale \(n\) touches \(\cup Q_v\), then \(n\le b_v\): otherwise \(c\subset U_n\subset U_{b_v+1}\), which is disjoint from \(\cup Q_v\) by (Tag-1). If \(c\) touches two tags, they are within sup-distance \(s_n\le s_{\min(b_v,b_{v'})}\), contradicting (Tag-2). \(\square\)

**Proposition MS-4 (kernel-rooted loads).** Assume §5.1, (Tag-1), (Tag-2), (MS-a–d), and that records with \(v\in I_\rho\) have birth \(\ge b_v\). Let \(\varrho\ge1\), \(\lambda\ge0\), \(\kappa_2\ge0\) with \(\kappa_\bullet-\lambda-\log\varrho-\kappa_2\ge\kappa_{\rm ms}\). Then for every \(v\):
\[
\sum_{\rho:\ v\in I_\rho}\varrho^{|I_\rho|}\,w_\rho\,e^{\lambda|N_\rho|}\ \le\ \frac{2m_0}{\Delta_*^2}\,n_{\rm att}(v)\,\sup_{j\ge b_v}W_j,
\]
\[
\sum_{\rho:\ v\in I_\rho,\ |I_\rho|\ge2}\varrho^{|I_\rho|}\,w_\rho\,e^{\lambda|N_\rho|}\ \le\ \frac{2m_0}{\Delta_*^2}\,n_{\rm att}(v)\,e^{-\kappa_2\rho_v}\,\sup_{j\ge b_v}W_j,
\]
where \(\rho_v\) is the least number of tiles of a \(*\)-connected set touching both \(\cup Q_v\) and another tag.

*Proof.* By (MS-a) the hull contains a tile \(t\in\mathcal T(v)\), of scale \(b_v\) (Tag-1). By MS-3, \(\varrho^{|I_\rho|}\le\varrho^{|N_\rho|}\). Apply the computation of MS-2 rooted at \(t\), with \(\vartheta=\lambda+\log\varrho\) (resp. extracting \(e^{-\kappa_2|N|}\le e^{-\kappa_2\rho_v}\) first), and sum over the \(n_{\rm att}(v)\) tiles. \(\square\)

**Use conditional.** With \(\varrho=eM_{\rm op}\) this is the component load (R11) of [Rep21] with extents measured in tiles. With the source numbers (\(n_{\rm att}\le(100R_b+3)^d\); \(\rho_v\ge cR_{b_v}\), from the margin of [Boundary estimate c] §5 and the separation; additional assumption) the multi-kernel load is \(\le C\bar W\sup_R(100R+3)^de^{-c\kappa_2R}\): uniformly small, **for tags of all ages together**. The same holds for the Kotecký–Preiss weight \(a(\rho)=a_0|N_\rho|\): a record is incompatible with at most the records sharing one of its \(\le|N_\rho|\) kernels. The physical extent of a record including the diameter of a touched tag is converted by the collar: for \(v\in I_\rho\) and a site \(x_i\), with \(r_i=\operatorname{dist}_\infty(x_i,\cup Q_v)\),
\[
r_i+\Delta_v\le M\Theta\bigl(d_g(x_i,X_\rho)+\sqrt d\,|N_\rho|\bigr)\qquad(H_\rho\subset\{v\}),
\]
by \(d_g(x_i,\cup Q_v)\le d_g(x_i,X_\rho)+\sqrt d|N_\rho|\) (T4), \(r_i\le Md_g(x_i,\cup Q_v)\) and (Col). As in §3.3, the application of [Rep21] §5 (tails) is not redone.

### 5.8 Prop. MS-5 (the load of a kernel decays with its graded depth)

**Setting.** As in [Boundary estimate d] §2.2 for the kernels ((Real), (Pos), (Resp) with \(d_g\), \(m_1\) kernels per anchor), and (MS) for the single-kernel records \(\mathcal E_1(v)\) (hull containing a tile of \(\mathcal T(v)\), \(H_e\subset\{v\}\), birth \(\ge b_v\)). \(a_v(i):=P\sup|\partial_i\tau_v|\), \(r_i=\operatorname{dist}_\infty(x_i,\cup Q_v)\), \(\Lambda_v:=\sum_la_v(l)e^{\chi r_l}\), and \(\Omega_v:=\sum_{m=b_v+1}^{K-1}\omega_m\) (the graded depth).

**Proposition MS-5.** Assume \(\chi M\le\nu/4\), \(\kappa_\bullet-\nu\sqrt d\ge\kappa_{\rm ms}\), (Tag-1), (Tag-2), (Col). Then for every \(v\),
\[
\Lambda_v\ \le\ C^{\rm ms}_\Lambda\,(s_*+m_0\bar W)\,e^{-\frac\nu4\Omega_v},\qquad C^{\rm ms}_\Lambda=n_I(2M+1)^d\sup_{D\ge0}\bigl(1+2(D+2)^d\bigr)\bigl(D+1+\tfrac{4d}\nu\bigr)^de^{-\frac\nu4\theta D},
\]
and \(t_v\le\Lambda_v\). No (Geo) hypothesis is used.

*Proof.* For \(e\in\mathcal E_1(v)\): \(d_g(x_l,\cup Q_v)\le d_g(x_l,X_e)+\sqrt d|N_e|\) (T4, since the hull touches \(\cup Q_v\)), and \(\chi r_l\le\chi Md_g(x_l,\cup Q_v)\le\frac\nu4d_g(x_l,\cup Q_v)\). So
\(w_ee^{-\nu d_g(x_l,X_e)}e^{\chi r_l}\le w_ee^{\nu\sqrt d|N_e|}e^{-\frac{3\nu}4d_g(x_l,\cup Q_v)}\). By the computation of MS-2 at the tiles of \(\mathcal T(v)\) (two choices of \(H_e\)), \(\sum_{e\in\mathcal E_1(v)}w_ee^{\nu\sqrt d|N_e|}\le2m_0\Delta_*^{-2}n_{\rm att}(v)\bar W\le2m_0(D_v+2)^d\bar W\). By (Col) and Lemma C1′ (with \(n=b_v\); \(\cup Q_v\subset\overline{\mathbb R^d\setminus U_{b_v+1}}\)), \(d_g(x_l,\cup Q_v)\ge\max\{\theta D_v,\Omega_v\}\), so \(e^{-\frac{3\nu}4d_g}\le e^{-\frac\nu4\theta D_v}e^{-\frac\nu4\Omega_v}e^{-\frac\nu4d_g}\). The sites with \(d_g(x_l,\cup Q_v)\le t\) lie in a cube of side \(\Delta_v+2Mt\le M(D_v+2t)\), so \(\sum_le^{-\frac\nu4d_g(x_l,\cup Q_v)}\le n_I(2M+1)^d(D_v+1+4d/\nu)^d\). The \(\sigma_v\) term is the same with weight \(s_*\) and no record sum. Finally \(|\tau_v(z)|\le\sum_l|z_l|\sup|\partial_l\tau_v|\le\sum_la_v(l)\). \(\square\)

**Consequences.**
1. With \(\Lambda_*:=C_\Lambda^{\rm ms}(s_*+m_0\bar W)\le\frac14\), [Boundary estimate c] Theorem R1 applies to every kernel, and Steps 3–4 of [Boundary estimate d] Theorem R6 go through with Theorem MS-1 in place of [Boundary estimate b] Theorem C′ and Theorem MS-2 in place of (M2) (anchor of a single-kernel record: a tile of \(\mathcal T(v)\) in its hull, of scale \(b_v\), so C3-ms applies with the ordinary collar). The result is R6's two inequalities with \(\mathfrak S\) replaced by \(\mathfrak S^{\rm ms}:=\Gamma_\Sigma(2m_0\Delta_*^{-2}\bar W+m_1s_*)\), under \(\chi\le3\nu/(16M\Theta)\) and (Geo) at \(c=3\nu/(16\Theta')\). conditional: The formula gives each step against the replacements listed; This remains an assumption.
2. **Summable variation.** \(t_v\le\Lambda_*e^{-\frac\nu4\Omega_v}\): the kernels deep in old structure have exponentially small variation over the current polydisc. For a hull \(N\), \(\sum_{v\text{ touching }N}t_v\le\Lambda_*\sum_{t\in N}e^{-\frac\nu4\Omega(t)}\). This is item (b) of §4.2. In the coarse format of [Boundary estimate d] the corresponding bound (R6 Step 2) is \(\Lambda_v\le\Lambda_*\) with no decay, because a coarse record of recent birth is attached to an old tag at no cost in the capped metric \(d^{(j)}\).

### 5.9 Lemma (the multiscale form refines the printed bound)

For a hull \(N\subset\mathcal T^{(j)}\) let \(X(N)\) be the set of \(\mathcal G_j\)-cubes containing a tile of \(N\). Then \(X(N)\) is \(*\)-connected, \(|X(N)|\le|N|\), \(\delta_j(X(N))\le\sqrt d\,|N|\). If records satisfy (MS-b,c,d) with \(\kappa_\bullet\ge\kappa_{\rm ms}+1+\sqrt d\,\kappa'\), then for every finite set \(X\) of \(\mathcal G_j\)-cubes,
\[
\sum_{\rho:\ \text{birth }j,\ X(N_\rho)=X}w_\rho\ \le\ \frac{2m_0}{\Delta_*^2}\,W_j\,e^{-\kappa'\delta_j(X)}.
\]
*Proof.* Every tile of \(\mathcal T^{(j)}\) lies in exactly one \(\mathcal G_j\)-cube (Nest), touching tiles lie in touching cubes, and a tree through the centres along a spanning tree of the \(*\)-adjacency of \(X\) has length \(\le\sqrt ds_j(|X|-1)\). By (MS-c) the hull contains a cube of \(X\) as a tile; root at one of the \(|X|\le e^{|X|}\) cubes, use \(|N|\ge|X|\) and the count of MS-2 with \(\vartheta=0\): the sum is \(\le m_0W_j|X|\Delta_*^{-2}\sum_{m\ge|X|}2^{-m}e^{-(1+\sqrt d\kappa')m}\). \(\square\)

So resumming a multiscale family over hulls with the same coarse cover gives a record of the printed form (2.42). The converse (recovering the multiscale family from the coarse record) is not possible from the bound alone (§4).

## 6. Jets of all orders of \(\sum_v\log G_v\) (a abstract; b application)

[Boundary estimate d] Theorem R6 gives orders 1 and 2 and leaves \(m\ge3\) open (§2.3 Remark 2). Setting and notation of [Boundary estimate c] Theorem R1 and [Boundary estimate d] §2.2 (either format).

For \(m\ge1\) put \(A_v^{(m)}(i_1,\dots,i_m):=P^m\sup_{D_{P/2}\times\Omega_v}|\partial_{i_1}\cdots\partial_{i_m}\tau_v|\), \(r_i(v)=\operatorname{dist}_\infty(x_i,\cup Q_v)\), and
\[
\mathsf L_m:=\sup_v\sum_{i_1,\dots,i_m}e^{\chi\max_sr_{i_s}(v)}A_v^{(m)}(i_1,\dots,i_m),\qquad
\mathsf R_m:=\sup_{i_1}\sum_v\sum_{i_2,\dots,i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}e^{\chi(r_{i_1}(v)+\Delta_v)}A_v^{(m)}(i_1,\dots,i_m).
\]

**Lemma J.** Assume (Real) and \(t_v\le\frac14\) for all \(v\). Then for \(m\ge1\), every \(i_1\) and \(z\in D_{P/2}\),
\[
\sum_{i_2,\dots,i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}\Bigl|\partial_{i_1}\cdots\partial_{i_m}\sum_v\log G_v(z)\Bigr|\ \le\ \frac3{P^m}\sum_{\pi}(2e^{3/4})^{|\pi|}\,|\pi|!\ \mathsf R_{|B_1(\pi)|}\prod_{B\in\pi,\ B\ne B_1(\pi)}\mathsf L_{|B|},
\]
the sum over the set partitions \(\pi\) of \(\{1,\dots,m\}\), with \(B_1(\pi)\) the block containing \(1\).

*Proof.* (1) *Formula.* For fixed \(v\) and \(z\), let \(\mathbb E=\Pi'_{v,z}\) (a normalized complex measure of total variation \(\le e^{3t_v}\le e^{3/4}\), [Boundary estimate c] R1(2)) and \(\partial_B\tau_v:=(\prod_{s\in B}\partial_{i_s})\tau_v\) for \(B\subset\{1,\dots,m\}\). Then
\[
\partial_{i_1}\cdots\partial_{i_m}\log G_v=\sum_\pi\kappa_{|\pi|}\bigl(\partial_B\tau_v:\ B\in\pi\bigr),
\]
with \(\kappa_k\) the joint cumulants under \(\mathbb E\). Indeed \(\log G_v(z+\sum_st_se_{i_s})-\log G_v(z)=\log\mathbb E\exp[\tau_v(z+\sum t_se_{i_s})-\tau_v(z)]\); the multilinear part of the exponent is \(\sum_{B\ne\emptyset}t^B\partial_B\tau_v\); and, writing \(f_B=\partial_B\tau_v\), the coefficient of \(t_1\cdots t_m\) in \(\log\mathbb E\exp\sum_Bt^Bf_B=\sum_k\frac1{k!}\sum_{B_1,\dots,B_k}\kappa_k(f_{B_1},\dots,f_{B_k})t^{B_1}\cdots t^{B_k}\) collects exactly the set partitions (terms with a repeated \(t_s\) do not contribute to it). This is an identity of power series in \(t\), valid for normalized complex measures because \(\mathbb E\exp(\cdot)\ne0\) near \(t=0\). For \(m=2\) it is [Boundary estimate d] Lemma H.

(2) *Cumulant bound.* \(\kappa_k(f_1,\dots,f_k)=\sum_{\sigma}(-1)^{|\sigma|-1}(|\sigma|-1)!\prod_{C\in\sigma}\mathbb E\prod_{a\in C}f_a\), the sum over set partitions \(\sigma\) of \(\{1..k\}\). So \(|\kappa_k|\le e^{3k/4}\prod_a\sup|f_a|\sum_\sigma|\sigma|!\). The number \(\sum_\sigma|\sigma|!\) of ordered set partitions has exponential generating function \(1/(2-e^x)\); evaluating at \(x=\frac12\) gives \(\sum_\sigma|\sigma|!\le k!\,2^k/(2-e^{1/2})\le3\cdot2^kk!\).

(3) *Weight.* For \(s\in B_1\): \(|x_{i_1}-x_{i_s}|\le\max_{s\in B_1}|x_{i_1}-x_{i_s}|\). For \(s\in B\ne B_1\): \(|x_{i_1}-x_{i_s}|_\infty\le r_{i_1}(v)+\Delta_v+r_{i_s}(v)\). All terms being \(\ge0\),
\(e^{\chi\max_s|x_{i_1}-x_{i_s}|}\le e^{\chi\max_{s\in B_1}|x_{i_1}-x_{i_s}|}e^{\chi(r_{i_1}+\Delta_v)}\prod_{B\ne B_1}e^{\chi\max_{s\in B}r_{i_s}}\).
Insert (1)–(2), bound \(\sup|\partial_B\tau_v|\le P^{-|B|}A_v^{(|B|)}\), sum over the sites of each block \(B\ne B_1\) (factor \(\le\mathsf L_{|B|}\) uniformly in \(v\)), then over \(v\) and the remaining sites of \(B_1\) (\(\le\mathsf R_{|B_1|}\)). \(\square\)

**Proposition J′ (the two quantities in the setting of [Boundary estimate d] §2.2).** Assume the hypotheses of [Boundary estimate d] Theorem R6 with \(\chi\le3\nu/(16M\Theta)\), (Geo) at \(c=\nu/(8\Theta')\) and \(\kappa_*\ge\nu+1+\kappa'_{\rm cnt}(d)\). Put \(\tilde\Lambda:=s_*+e^{C_0}\bar W\). There are \(C_L,C_R\) depending on \(d,M,\nu,\theta,n_I,m_0,m_1,\gamma\) only such that for all \(m\ge1\)
\[
\mathsf L_m\le C_L^m(m!)^{d+1}\tilde\Lambda,\qquad\mathsf R_m\le C_R^m(m!)^{d+1}\,\mathfrak S,\qquad\mathfrak S=\sum_{j\le K}\Gamma_j(\mathfrak aW_j+m_1s_*).
\]
*Proof.* By Cauchy on the polydisc of radius \(P/2\) and (Loc′), for \(e\in\mathcal E_1(v)\): \(P^m\sup_{D_{P/2}}|\partial_{i_1}\cdots\partial_{i_m}V_e|\le(m-1)!2^{m-1}w_ee^{-\nu\max_sd_e(i_s)}\), \(d_e(i)=d_g(x_i,X_e)\); likewise for \(\sigma_v\) with weight \(s_*\) and carrier \(\cup Q_v\).

\(\mathsf R_m\): by [Boundary estimate d] (2.1) and \(\chi M\Theta\le\nu/4\), \(e^{\chi(r_{i_1}+\Delta_v)}\le e^{\nu\sqrt d/2}e^{\frac\nu4\delta_e}e^{\frac\nu4d_e(i_1)}\), so the summand is \(\le e^{\nu\sqrt d/2}(m-1)!2^{m-1}\,[w_ee^{\frac\nu4\delta_e}]\,e^{\chi\max|x_{i_1}-x_{i_s}|}e^{-\frac{3\nu}4\max_sd_e(i_s)}\). This is the quantity that Steps 2–5 of the proof of [Boundary estimate b] Theorem C′ bound (Step 1 is the only place where \(F_\rho\) itself enters), with rate \(3\nu/4\) and weights \(w_ee^{\nu\delta_e/4}\); the needed rooted norm is at \(\vartheta=\frac\nu4+\frac{3\nu}8+1\le\nu+1\), which is (M2). The \(\sigma_v\) family is treated the same way ([Boundary estimate d] R6 Step 3).

\(\mathsf L_m\): by [Boundary estimate d] (2.1), \(e^{\chi\max_sr_{i_s}}\le e^{\frac\nu4(\delta_e+2\sqrt d)}e^{\frac\nu4\max_sd_e(i_s)}\). For \(e\) of birth \(j\), [Boundary estimate d] R6 Step 1–2 give \(d_e(i)\ge D_*:=\max\{\theta D^{(j)},\sum_{n=j+1}^{K-1}\omega_n\}-\delta_e-2\sqrt d\) for every site. Hence
\(e^{-\frac{3\nu}4\max_sd_e(i_s)}\le e^{\frac\nu4(\delta_e+2\sqrt d)}e^{-\frac\nu8\theta D^{(j)}}e^{-\frac\nu8\sum_{n>j}\omega_n}\prod_{s=1}^me^{-\frac\nu{2m}d_e(i_s)}\).
By [Boundary estimate b] Lemma C3(1),(3) the site sum is \(\sum_ie^{-ad_e(i)}\le n_I(2M\Theta+1)^d(\delta_e+3+d/a)^d\) with \(a=\nu/(2m)\), and as in [Hidden components] Step 3, \(\prod_{s\le m}(\cdots)\le C^m(m!)^de^{\delta_e+3}\). The record sum at fixed \(j\) is \(\sum_ew_ee^{(\nu/2+1)\delta_e}\le4m_0K_d^{3\cdot2^d}W_j(D^{(j)}+3)^d\) ([Boundary estimate b] Prop. B2′ at the \(\le(D^{(j)}+3)^d\) cubes touching the tag), \((D+3)^de^{-\frac\nu8\theta D}\) is bounded, and (Geo) gives \(e^{-\frac\nu8\sum_{n>j}\omega_n}\le e^{C_0}e^{-\gamma(K-1-j)}\) for \(j\le K-1\). Sum over \(j\). \(\square\)

**Theorem J.** Under the hypotheses of Prop. J′ and \(\Lambda_*\le\frac14\), for all \(m\ge1\), \(i_1\), \(z\in D_{P/2}\):
\[
\sum_{i_2,\dots,i_m}e^{\chi\max_s|x_{i_1}-x_{i_s}|_\infty}\Bigl|\partial_{i_1}\cdots\partial_{i_m}\sum_v\log G_v(z)\Bigr|\le\frac{C_1C_2^{\,m}(m!)^{d+1}}{P^m}\,(1+\tilde\Lambda)^{m-1}\,\mathfrak S.
\]
*Proof.* Lemma J and Prop. J′: each term is \(\le3(2e^{3/4})^{|\pi|}|\pi|!\,C^m\prod_B(|B|!)^{d+1}\tilde\Lambda^{|\pi|-1}\mathfrak S\), and \(\sum_\pi|\pi|!\prod_B(|B|!)^{d+1}\le(m!)^d\sum_\pi|\pi|!\prod_B|B|!=(m!)^d\,m!\,2^{m-1}\) (ordered set partitions with ordered blocks are the compositions of a permutation). \(\square\)

The growth \((m!)^{d+1}\) is the same as for ordinary records ([Hidden components] (C.10)), i.e. the power five of (AB17.5) in \(d=4\). In the multiscale format the same statement holds with MS-1, MS-2, MS-5 in place of C′, (M2), R6 Step 2; then \(\tilde\Lambda=s_*+m_0\bar W\) and no (Geo) is needed for \(\mathsf L_m\) (b; replacements as in §5.8, not rewritten).

## 7. (FT)/(Mon) at T steps: the weights

[Boundary estimate d] N7 has (source input; source) for the carriers and additional assumption for the weights. of [I§6]:

- p.7, (1.24), quoted in G5: the term with domain \(Y_0\) built from a record \(\mathbf E^{(j)}(X)\) is bounded by \(\dots(L^j\eta)^5\exp(-(\kappa_1-1)M^{-4}|Y_0\setminus\tilde\square^4|)\exp(-\kappa d_j(X))\). **The old factor is carried unchanged and each new cube is charged.**
- p.8: for the terms of type (I.3.7), "It is defined now as the family of all cubes \(\Delta\) disjoint with the interior of \(X_0\), where \(X_0\) is the smallest localization domain from \(\mathbf D_k\) containing \(X\)."
- p.9: the bound ends with "\(\exp(-(\kappa_1-1)M^{-4}|Y\setminus X_0|)\exp(-\kappa d_j(X))\) (1.30). By the definition of the linear size functions they satisfy the following fundamental scaling inequality \(d_j(X)\ge(L^j\eta)^{-1}d_k(X_0)\) (1.31). It implies that the last two exponentials in (1.30) can be bounded by \(\exp(-(1-\delta)\kappa d_k(Y)-\delta\kappa d_j(X))\) (1.32), if \(\frac14(\kappa_1-1)\ge(1-\delta)\kappa\), \(0<\delta<1\)."

So at a T step the new carrier \(Y\) contains \(X_0\supseteq X\), the new bound charges every cube of \(Y\) in the new grid, and a fraction \(\delta\) of the old tree factor survives. With G4 ("The remaining considerations and bounds are the same as in [I]") this is (Mon) and the weight half of (FT) for T steps: **source** for the single-sequence case, **(c) + the one sentence of G4** for the multiscale sequence. For a record with a declared hole the same computation applies to the visiting size of its paid exterior \(F\) (a tree visiting the cubes of \(F\) visits the coarse cubes containing them, so \(\delta_j(F)\ge L^{k-j}\delta_k(F_0)\)); deduction for this remark, (d) that the source's (1.30) is used in that form.

The record itself, evaluated at zero fluctuation, keeps its index \(j\), its carrier and its bound ([III] p.262: "the expressions with indices \(j<k\) are exactly as described above").
