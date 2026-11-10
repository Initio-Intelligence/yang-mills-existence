# Decoupling of localized fluctuation terms

The pointwise supremum over retained marked states cannot, in general, be small. The joint event and flat-test estimates below concern integrated insertions. The local R-test requires the [structured cluster estimate and parameter conditions](local_test_estimates.md); transfer of derivative, normalized mark, reset and shell estimates to that same representation is a separate hypothesis. The literal test and the local test cannot be interchanged in a norm estimate solely because the Wilson marginals agree.

**Local-chart hypotheses.** In every application use (A8′) in the structured form 3′ and 4′, F(4′) on (Avg), (Sm3′), (Par-g_Z′), and (Lay-W), with $M_W\mid M_1$ and $M_1\ge6M_W$. In particular the per-potential rate must satisfy $\kappa_1/2\ge\sqrt d(1+3\beta)\kappa/(1-3\delta)$. The bound on the joint terminal law requires the action estimate and item 4′.

## 2. The [Dec] reading: closure

### 2.1 The problems, the tiles, the backgrounds

Two families of determining-set problems occur.

* **(T)** the box problems \(\mathbb G=\mathbb B_b=\mathbf B_{k+1}(\square_b^{\sim4})\), \(b\in\mathfrak B_{k+1}\) ([RD] §§2.1, 2.5). Top level \(t=k+1\). Sequence: [III] p.256 with \(\Omega=\square_b^{\sim4}\), levels \(0,\dots,k+1\). Space \(\mathcal S_{\mathbb G}\): \(\tilde U^c_{k+1}(X,(1+\beta)\tilde\alpha_0,(1+\beta)\tilde\alpha_1)\) for \(X\subset\square_b^{\sim4}\). By [RD] (B5), \(\square_b^{\sim4}\subset\Omega_{k+1}\) with margin \(\ge2LM_2R_{k+1}\), so only the top-level clauses (\(n=j=k+1\)) of (2.34)–(2.39) apply there.
* **(R)** the component problems \(\mathbb G=\mathbb B^{(n+1)}_k(Z)\) of [IV] (1.19), \(Z\) an eligible component, preparatory step \(n+1\), \(j=h+n\). Top level \(t=k\). Sequence: the admissible sequence \(\{\Omega''_m\}\) of (1.12)–(1.13) inside \(Z\), with the \(\mathbf B_k(Z)\)-collar of width \(\le2M_1\) at \(\partial Z\) inside \(\Omega_k\). Space: \(\tilde U^{(n+1)c}_k(X,\tilde\alpha_0,\tilde\alpha_1)\), \(X\subset Z\), (1.64)–(1.69).

**Tiling.** \(\mathcal T_{\mathbb G}\) := the cubes of the \(M\)-partition \(\pi_k\) (side \(M\) in \(T^{(k)}\) units) meeting the domain of \(\mathbb G\), intersected with it. This is one uniform scale, the one Bałaban uses (S6), and the one in which the R- and B-classes measure linear size (\(\mathbf D_k\)). The layers of \(\mathbb G\) near its boundary are thinner than a tile ([AU] E4), so no proper (graded) tiling with (Thick) exists; none is needed.

**Walk block.** \(M_W\) denotes the big-block size of [P] (the "\(M\)" of [P] Theorem 3.1 and §C, \(M_W=KR_0M_0\), \(M_W\ge M_W^{\min}(d,L)\)). It is fixed after \(d,L\). The estimates in Local deformation of propagators and the minimizer/Domains of the representation-defined derivatives identify it with [III]'s \(M_1\); §2.2 shows that this identification must be dropped for the collars.

### 2.2 Geometry

**(G-adm) Admissibility — deduction, given S1, S4, S5.** Every layer \(\Lambda^{\mathbb G}_m=\Omega^{\mathbb G}_m\setminus\Omega^{\mathbb G}_{m+1}\) of \(\mathbb G\) has width \(\ge LM_1\) in level-\(m\) units, and every \(\Omega^{\mathbb G}_m\) is a union of level-\(m\) \(M_1\)-cubes.
*Proof.* (T): S4 gives \({\rm dist}(\Omega_{m+1},\Omega^c_m)\ge L^{m+1}\xi M_1=LM_1\cdot L^m\xi\). (R): the \(\mathbf B_k(Z)\)-collar has the same structure (S4 applied to \(Z\)); the \(Z''\)-layers are one \(M\)-cube thick at their level (S5, p.179), and \(M\ge LM_1\); the old layers \(\Omega_m\setminus\Omega_{m+1}\) are \(\ge2MR_m\) thick (S4, p.256). \(\square\) (The junction of the \(Z''\)-structure with the \(\mathbf B_k(Z)\)-collar is taken from (1.19) as printed; that the combined set is an admissible sequence in the sense of [P2] is additional assumption, the same reading the source makes on p.180.)

Hence \(\mathbb G\) satisfies [P2] (2.1)–(2.2) with big blocks \(M_W\) (if \(M_W\mid M_1\)) and \(R=LM_1/M_W\), so \(RM=LM_1\).

**(Lay-W) the two-layer geometry of [P] §C — deduction for the arithmetic, an additional assumption that this is the containment [P] §C uses.** [P] builds the local sequence of a walk cube inside \(\tilde\square^5\) from at most two consecutive global layers (S3). For the \(M_1\)-thin collars this holds iff the walk block is small enough compared with \(M_1\):

> **(Lay-W)** \(M_W\mid M_1\) and \(M_1\ge6M_W\).

*Proof (sufficiency).* The layers of \(\mathbf B_j(\Omega)\), for rectangular \(\Omega\), are rectangular shells; a cube meets exactly the layers met by the range of the \(\ell^\infty\)-depth over the cube, so a 1D cross-section suffices. A level-\(m\) walk cube has side \(2M_W\), its \(\tilde\square^5\) side \(12M_W\) (level-\(m\) units). Its own layer has width \(\ge LM_1\) (level \(m\)); the finer neighbour has width \(\ge M_1\) in level-\(m\) units, the coarser one \(\ge L^2M_1\). With \(M_1\ge6M_W\) the 5-neighbourhood reaches at most \(6M_W\le M_1\) beyond the walk cube's own layer, so it never crosses a neighbouring layer.  item (2) checks the exact integer geometry of [III] p.256 (maximal domains, cube-aligned) for \(L=3,5,13\), five levels: at \(M_1/M_W=1,2\) a 5-neighbourhood meets up to 7 layers; at 4 up to 3; at \(\ge6\) never more than 2. \(\square\)

So with the identification \(M_W=M_1\) (Local deformation of propagators and the minimizer (W-ms): constants "depending on \(d,L,M_1\)"; Domains of the representation-defined derivatives §4: "\(M\ge160L^3M_1\)") the [P] §C construction does not apply to the collars: a level-\(m\) walk neighbourhood crosses every finer layer. (Lay-W) is a condition on the free constant \(M_1\) fixed after \(d,L,M_W\). It agrees with S4's reading of \(M_1\) as "the size of large cubes for which all the theorems of the previous papers … are valid".

**(Geo-α) [P2] (2.59) for the collars.** Theorem S of Source operators for the deformed reconstruction bounds operators by row sums of the deformed kernels, which decay at \(\delta=\frac14\delta_0\) (Local deformation of propagators and the minimizer Theorem W). Lemma 2.1 at \(\alpha=\frac14\) with \(RM=LM_1\):

> **(Geo-α)** \(\frac1{16}\delta_0LM_1>2d\log\coth(\delta_0/16)+1\); for \(d=4\): \(\delta_0LM_1>371.1\) at \(\delta_0=1\), \(>548.3\) at \(\delta_0=\frac14\) (finite comparison.

The conditions recorded in the collar estimate for CT♯ (\(\alpha=\frac12\)) and its \(s\)-variant (\(\alpha=\frac18\)) are also needed for \(RM=LM_1\) wherever CT♯ is used on these sets. They must be **doubled** (finding 5, §5): 141.4 and 919.3 at \(\delta_0=1\).

**(Tile) Lemma W0(e) on \(\mathcal T_{\mathbb G}\).** W0(e) asks (i) \(d\ge d_{\mathcal T}\) along paths and (ii) \({\rm diam}_\infty\tilde X_i\le s_\sigma/(8L^2)\) for walk dependence domains \(\tilde X_i\).
* (i) Bałaban's \(d\) measures a path in a layer of level \(m\) in units \(L^m\eta\) ([P2] (2.46), source). The tile metric of \(\mathcal T_{\mathbb G}\) uses the unit \(L^k\eta\). For (R), every level is \(\le k\), so \(d\ge d_{\mathcal T}\). For (T), the top region has level \(k+1\), so \(d\ge d_{\mathcal T}/L\). In Local deformation of propagators and the minimizer Lemma G3 replace \(\ell_0\) by \(\ell_0/L\) for (T) (this is Source operators for the deformed reconstruction (E5), [AU] E4).
* (ii) \(\tilde X_i\) of a level-\(m\) walk has diameter \(\le20M_WL^m\eta\) (Domains of the representation-defined derivatives §4 with \(M_W\) for \(M_1\)), and \(m\le t\).

> **(Tile)** \(M\ge160L^{2+(t-k)}M_W\) (\(160L^3M_W\) for (T), \(160L^2M_W\) for (R)), and \(\pi_k\) nested in the block partitions (Par-c).

Then W0 holds with \(\delta=\frac14\delta_0\) and
\[
\kappa_{\max}^{\mathbb G}=\frac{\delta_0M}{2^{d+6}L^{2+(t-k)}}.
\]
For a uniform tiling \(\Delta_*=3^d-1\) and \(b_0=\log(2^{d+1}\Delta_*^2)\) (\(=12.23\) for \(d=4\)). Local deformation of propagators and the minimizer Lemmas G1–G3 hold trivially for one scale.

### 2.3 Lemma N (normalisation comparison) — deduction, given source input for S2, S4, S5

Put, for (T),
\[
a_0^{\mathbb G}:=BC(1+\beta)M\alpha_{0,k+1},\qquad a_1^{\mathbb G}:=(1+\beta)\alpha_{1,k+1},\qquad a_J^{\mathbb G}:=(1+\beta)\alpha_{0,k+1},
\]
and for (R), with \(\Theta_0:=3L_0^{2N_0}\) and maxima over \(h\le m\le k\),
\[
a_0^{\mathbb G}:=\Theta_0BCM\max_m\alpha_{0,m},\qquad a_1^{\mathbb G}:=\Theta_0\max_m\alpha_{1,m},\qquad a_J^{\mathbb G}:=\Theta_0\max_m\alpha_{0,m}.
\]

**Lemma N.** Let \((\mathbf U,\mathbf J)\in\mathcal S_{\mathbb G}\) on the domain \(X\) of a term, with \(\mathbf U=U'U\). Then on \(X\), for the sequence of \(\mathbb G\):
1. \(U\) satisfies [P] (3.35) with "\(O(1)M\alpha_0\)" \(=a^{\mathbb G}_0\), i.e. with \(\alpha_0^{[P]}=a_0^{\mathbb G}/(12M_W)\);
2. \(A'\) satisfies [P] (3.37) with \(\alpha_1^{[P]}=a_1^{\mathbb G}\);
3. \((L^m\eta)^3|\mathbf J(b)|\le a_J^{\mathbb G}\) for \(b\) in a level-\(m\) layer of \(\mathbb G\).

[P] (3.36) and (3.38) are not implied, and they are not needed. Theorem 3.4 and Corollaries 3.5–3.6 use only (3.35) and (3.37) (S2). (3.36) serves only to bound \(J(U)\) and \(H^*J\), and with an independent \(\mathbf J\) item 3 replaces it ((S-calc♯), the representation convention).

*Proof.* (T). A [P]-class cube \(\square_P\) of the box sequence has index \(m\le k+1\) and size \(12M_WL^m\eta\le12M_W\le CM\) (top units; (Tile)). It lies in a cube \(\square\subset\Omega_{k+1}\) of size \(CM\), by the margin of \(\square_b^{\sim4}\) in \(\Omega_{k+1}\). (2.38) gives a gauge on \(\square\cap X\) with \(L^{k+1}\xi|A|,(L^{k+1}\xi)^2|\nabla A|<BC(1+\beta)M\alpha_{0,k+1}\). Since \(L^m\xi\le L^{k+1}\xi\), the same gauge gives \(L^m\xi|A|<a_0^{\mathbb G}\) and \((L^m\xi)^2|\nabla A|<a_0^{\mathbb G}\) on \(\square_P\cap X\). This is (3.35) for index \(m\) with \(O(1)M_W\alpha_0^{[P]}=a_0^{\mathbb G}\) and \(O(1)=12\) (S3). Items 2 and 3 follow the same way from (2.39) and (2.36): the bounds at level \(k+1\) imply those at every finer level. That is the monotonicity of all these conditions in the level, since the weights \((L^m\eta)^{-p}\) increase as \(m\) decreases.
(R). (1.64)–(1.69) impose the level-\(m\) clause on \((\Omega''_m\setminus\Omega''_{m+1})\cap X\) and on \((\Omega_m\setminus\Omega_{m+1})\cap X\). These are the layers of \(\mathbb G\) at level \(m\) (S5, (1.13), (1.19); matching (d) at the junction, as in (G-adm)). On \(\Omega_k\cap X\), which contains the \(\mathbf B_k(Z)\)-collar, the clause is the level-\(k\) one with \(c=3\), and it implies the finer collar levels by monotonicity. The extra factors are \(L_0^{2\max(0,m-k_0)}\le L_0^{2N_0}\) and \(c\le3\). \(\square\)

**Consequence.** [P] Theorem 3.1 needs \(M_W\alpha_0^{[P]}\le a_0\), i.e. \(a^{\mathbb G}_0\le12a_0\). Lemma L of Source operators for the deformed reconstruction needs \(c(a_0^{\mathbb G}/12+L^2a_1^{\mathbb G})\le a_1\). Both are **coupling ceilings**, because \(a^{\mathbb G}_\cdot=g\cdot\)polylog with \(M\) fixed before \(g\). For (R), \(\Theta_0<3L(L+1)N_0^{-1}R_k\) (S5, p.192) adds a polylogarithm. For bounds that only involve the datum support (Lemma D), the constants of Lemma N **on that support** may be used: \(a^{\rm dat}_0,a^{\rm dat}_1\), equal to \(a^{\mathbb G}_0,a^{\mathbb G}_1\) for (T) and to \(\Theta_0BCM\alpha_{0,k}\), \(\Theta_0\alpha_{1,k}\) for (R) (the collar lies in \(\Omega_k\), level-\(k\) clause).

### 2.4 Lemma F (the axial frame, and covariance)

**Lemma F.**
1. *The axial representative leaves [P]'s complex domain.* Let \(\mathbf U=U'U\) with \(U\) real and \(A'\) satisfying (3.37) at the top level \(t\), and let \(u_{\mathbf U}\) be its hierarchical axial frame ([RD] Definition 2.5 item 1). Then \(\mathbf U^{\rm ax}=\mathbf U^{u_{\mathbf U}}\) has, in general, no decomposition \(\tilde U'\tilde U\) with \(\tilde U'\) satisfying (3.37) with a constant comparable to \(\alpha_1\). Abelian example: on a transverse bond at a block boundary of level \(m\), \({\rm Im}A^{\rm ax}=\eta^{-1}\times\)(imaginary flux through the loop closed by the two axial contours). That is \(\asymp\alpha_1L^m/(L^t\eta)\) against the bound \(\alpha_1/(L^t\eta)\). A complex gauge transformation with a non-smooth imaginary part cannot be absorbed into the real factor. finite comparison: the ratio grows linearly in the block side (2.4, 5.3, 10.9, 22.0 for sides 4, 8, 16, 32).
2. *Covariance.* For every \(G^c\)-valued gauge transformation \(u\) these are identities between explicit formulas, where the right-hand sides are defined:
   * \(\Delta'_a(\mathbf U^u)=R(u)\Delta'_a(\mathbf U)R(u)^{-1}\), and likewise for \(Q(\mathbf U)\), \(Q'(\mathbf U)\), \(\Delta_a\), each local walk operator \(G'_\square,C_\square,G_\square\) of [P] (3.87), each walk term, hence each deformed operator \(P(s)\);
   * the right-form \(\Delta'_\pi\) of (S-calc♯) (D1) with \(\mathbf J\to R(u)\mathbf J\), (D2), (D3);
   * the local maps of [V] (179)–(180).

   Consequently \(\mathscr H(B;s;\mathbf U^u,R(u)\mathbf J)=R(u)\,\mathscr H(B^{u};s;\mathbf U,\mathbf J)\), with \(B^u\) the block datum transported by \(u\) at block points.
3. *Repair of Definition 2.5.* Read item 3 of [RD] Definition 2.5 as: compute the response at \((\mathbf U,\mathbf J)\) itself, with datum \(\tilde B_b:={\rm Ad}(u_{\mathbf U}^{-1})B_b(\mathbf U)\), and conjugate the output by \(u_{\mathbf U}\). By item 2 this is the same function wherever both are defined. It is the one controlled by Theorem Dec♯, since \((\mathbf U,\mathbf J)\in\mathfrak U_{\mathbb G}\) by Lemma N. The same reading applies to the component analogue (§3) and to [IV]'s own (1.56).
4. *Frame bound.* \(u_{\mathbf U}=u_U\,v\) with \(u_U\) the (unitary) axial frame of the real factor and \(|\log v(x)|\le\sum|\eta A'|\) along the axial contour of \(x\). The contour has length \(\le\frac{dL^2}{L-1}L^t\eta\) ([I] (0.11), source). So \(|\log v|\le2dL(1+\beta)a_1^{\mathbb G}\) and \(\|{\rm Ad}(u_{\mathbf U}^{\pm1})\|\le e^{2|\log v|}\le2\) under the ceiling \(4dLa^{\mathbb G}_1\le\log2\). For (T) the contour runs up to level \(t\) and the top-level bound \(|A'|<a_1^{\mathbb G}(L^t\eta)^{-1}\) holds on the whole box, so the level-\(n\) segments contribute \(\le dLa^{\mathbb G}_1L^{n-t}\) and the sum is geometric. For (R) the axial conditions hold at every level present in the determining set ([RD] §3), so a point of a level-\(m\) layer has its contour inside its own level-\(m\) block, where the level-\(m\) bound holds. The sum is again geometric and the same bound results.

*Proof.* 1: computation (abelian, which is enough for a counterexample); finite comparison. 2: each operator is either an explicit finite-difference or averaging expression covariant under all \(u\), or the inverse of one. For an inverse, \((R(u)XR(u)^{-1})^{-1}=R(u)X^{-1}R(u)^{-1}\). Walk terms are products of such operators with scalar cutoff functions \(h_\square\). The deformed system is a fixed-point equation in these, so its unique small solution transforms covariantly. 3, 4: immediate. \(\square\)

This upgrades [RD] Lemma 3.2(2)'s "\(|{\rm Ad}(u_{\mathbf U}^{-1})|\le2\)" from (d) to (a) (given [I] (0.11)). It also removes the background domain question for the frame.

### 2.5 Lemma D (the datum) — conditional on (Avg)

> **(Avg)** For every level \(m\le t\), the averaging maps \(\mathbf U\mapsto M^m(\mathbf U)(c)\) of [I]/[A] are block-local and analytic in the scaled field \(a=L^t\eta A\) (in any gauge in which \(\mathbf U=e^{i\eta A}\) on the block) on a ball \(|a|_\infty<r_*\). Here \(r_*>0\) depends on \(d,L\) only, uniformly in \(m,t\), and \(M^m(1)=1\).

Status of (Avg): additional assumption. It is what [A] proves for real configurations (assumed). The complex case is the same holomorphic statement. Its uniformity in the number of levels is the content of the scaled normalisation (\(L^m\eta Q_mA\) is bounded by the top-scale \(L^t\eta|A|\)).

**Lemma D.** Under (Avg) and the frame ceiling of Lemma F(4), for \((\mathbf U,\mathbf J)\in\mathcal S_{\mathbb G}\):
\[
|B_{\mathbb G}(\mathbf U)|_\infty\le C_B(additional assumption; L)\,(a_0^{\rm dat}+a_1^{\rm dat}).
\]
Here \(B_{\mathbb G}\) is \(B_b\) of [RD] Definition 2.5 item 2 for (T), and the argument of \(\mathbb H\) in (1.56) for (R). At the construction's real configurations the source's own bound \(44d^2B_3\varepsilon\) holds ([III] p.268; [IV] p.188; source).
*Proof.* \(B_{\mathbb G}(c)\) is \(\frac1i\log\) of a product of two averages of \(\mathbf U^{\rm ax}\) and of \(Q^{s*}_tM^t(\mathbf U^{\rm ax})\) at a collar bond \(c\). \(Q^{s*}\) is block-local (S4, (1.3)). So \(B_{\mathbb G}(c)\) is a block-local analytic function of \(\mathbf U\), invariant in modulus under gauge changes (Lemma F). Compute it in the gauge of (2.38)/(1.65) on a cube containing the \(t\)-blocks of \(c\). There \(|a|\le a^{\rm dat}_0+a^{\rm dat}_1\) (Lemma N on the datum support) and the function vanishes at \(a=0\). The Schwarz lemma on \(|a|<r_*\) gives the bound, with \(C_B=\pi/r_*\) times a factor for the logarithm. \(\square\)

### 2.6 Theorem Dec♯

**Theorem Dec♯.** Let \(\mathbb G\) be a problem of type (T) or (R) (§2.1), with the tiling \(\mathcal T_{\mathbb G}\). Assume:
* the source premises (U1)–(U6) of Domains of the representation-defined derivatives §7.1 and (S-calc♯) (the representation convention);
* (G-adm), (Lay-W), (Geo-α), (Tile) of §2.2;
* \(1\le\kappa_1\le\kappa^{\mathbb G}_{\max}\);
* the ceilings
  * (Sm1) \(a^{\mathbb G}_0\le12a_0\) and \(c(a^{\mathbb G}_0+L^2a^{\mathbb G}_1)\le a_1\) ([P] Thms 3.1, 3.4; Lemma L);
  * (Sm2) \(\alpha_J\hat B^{11}\le c_S\) with \(\alpha_J:=c(a^{\mathbb G}_0+a^{\mathbb G}_1+a^{\mathbb G}_J)\) and \(\hat B:=2n_0B_se^{2^d\kappa_1}\) (the representation convention's ceiling for the deformed package);
  * (Sm3) \(4dLa^{\mathbb G}_1\le\log2\);
  * (Sm4) \(2C_B(a_0^{\rm dat}+a_1^{\rm dat})\le\frac12c_S\hat B^{-6}\).

Then, for every \((\mathbf U,\mathbf J)\in\mathcal S_{\mathbb G}\):
1. **Domain.** \((\mathbf U,\mathbf J)\) lies in [P]'s domain \(\mathfrak U_{\mathbb G}\) ((3.35)+(3.37)) for the sequence of \(\mathbb G\), with \(\alpha^{[P]}_0=a_0^{\mathbb G}/(12M_W)\) and \(\alpha^{[P]}_1=a^{\mathbb G}_1\); and \(|\mathbf J|\le a^{\mathbb G}_J(L^m\eta)^{-3}\). (Lemma N.)
2. **M♯ for \(\mathbb G\).** The deformed system of [V] (179)–(180), without the \(J\)-term and with the operators defined by (S-calc♯), built on the deformed package over \(\mathcal T_{\mathbb G}\), has a unique small solution \(\mathscr H_{\mathbb G}(B;s;\mathbf U,\mathbf J)\). It is holomorphic on
\[
\{|B|_\infty<\varepsilon_{\mathcal H}:=c_S\hat B^{-6}\}\times\{|s_t|<e^{\kappa_1}\}\times\mathcal S_{\mathbb G}.
\]
It satisfies \(|\mathscr H_{\mathbb G}|_\nu\le C_S\hat B^2|B|_\infty\) for \(\nu\in\{0,1\}\), \(\mathscr H_{\mathbb G}(B;1)=\mathscr H_{\mathbb G}(B)\) and \(\mathscr H_{\mathbb G}(0;s)=0\). It is \(Y\)-subordinate of depth \(\ge0\) for every zero pattern \(Y\supset R\) (Local deformation of propagators and the minimizer §4.1).
3. **Covariance.** Lemma F(2) holds, and so does covariance under the lattice isometries preserving all partitions, provided the [P] §C families \(\mathscr D\) and the partition of unity \(\{h_\square\}\) are chosen covariantly. This can always be done: \(h_\square=\varphi_\square/(\sum\varphi^2)^{1/2}\) with a symmetric bump \(\varphi\).
4. **Tube expansion with vanishing.** Take a root \(R\) of \(\le2^d\) tiles and a composite \(\Phi(s)=F(\mathscr H_{\mathbb G}(\tilde B_{\mathbb G}(\mathbf U);s)\restriction_{{\rm core}(R)})\). Here \(F\) is holomorphic, local in \({\rm core}(R)\), with \(F(0)=0\) and \(|F(h)|\le C_F|h|\) for \(|h|\le C_S\hat B^2\varepsilon_{\mathcal H}\). Then
\[
\Phi(1)=\sum_T\Phi_T,\qquad|\Phi_T|\le A_{\mathbb G}\,(e^{\kappa_1}-1)^{-|T|},\qquad A_{\mathbb G}:=2C_FC_S\hat B^2\sup_{\mathcal S_{\mathbb G}}|B_{\mathbb G}|_\infty\le2C_FC_S\hat B^2C_B(a_0^{\rm dat}+a^{\rm dat}_1).
\]
The sum runs over sets \(T\) of tiles outside \(R\) such that \(R\cup T\) is \(*\)-connected and **meets the support of the datum**. Every other term vanishes identically. \(\Phi_T\) depends on \((\mathbf U,\mathbf J)\) only through their restriction to \(R\cup T\). It is holomorphic on \(\mathcal S_{\mathbb G}\) restricted there, and covariant as in item 3.
5. All constants depend on \(d,L,M_W,M,\kappa_1\) and the source constants only, not on \(k\), \(n\), \(b\), \(Z\), the number of levels, the volume or the background.

**Hypotheses: conditional** on (U1)–(U6), (S-calc♯), and (Avg) (the last through (Sm4) only).

*Proof.*
* (G-adm), (Lay-W) and (Geo-α) put \(\mathbb G\) under [P2] (2.1)–(2.2) with \((M,R)=(M_W,LM_1/M_W)\), under the two-layer geometry of [P] §C, and under Lemma 2.1 at \(\alpha=\frac14\). So the printed theorems behind (U1)–(U3) apply to the sequence of \(\mathbb G\), with constants independent of the sequence (S2, p.399).
* Item 1 is Lemma N. With (Sm1), Prop. W♭ of Source operators for the deformed reconstruction, conditional on (U1)–(U4), gives the complex walk expansions of the four primitives.
* (Tile) and §2.2 give W0(a)–(e) on \(\mathcal T_{\mathbb G}\), hence Local deformation of propagators and the minimizer Theorem W with \((\hat B,\frac14\delta_0)\) for \(\kappa_1\le\kappa^{\mathbb G}_{\max}\).
* Source operators for the deformed reconstruction Theorem S with \(B=\hat B\), under (Sm2), with Lemma GP (The one-sided collar estimate/The one-sided collar estimate) replacing the \(G_\pi\) node and (D1)–(D3) as definitions for an independent \(\mathbf J\), gives the contraction and the first-order bound (U6). This is item 2's existence, holomorphy and bound. Holomorphy in \((\mathbf U,\mathbf J)\) follows from uniform convergence of iterates, each holomorphic in the background (Source operators for the deformed reconstruction, F4).
* Subordination is Local deformation of propagators and the minimizer Lemma 4.1 (R1)–(R4) applied to the admissible calculus (Local deformation of propagators and the minimizer §4.2 with the node list of Source operators for the deformed reconstruction §2 and the right forms of The one-sided collar estimate (D1)–(D3)). Domains of the representation-defined derivatives checked it deduction, and nothing there depends on the tiling being graded.
* Item 3: Lemma F.
* Item 4 is the argument of [AU] §1.4 (Local deformation of propagators and the minimizer Theorem D applied to the composite). Lemma D and (Sm3)–(Sm4) put \(\tilde B_{\mathbb G}\) in the ball, so \(A_{\mathbb G}\) bounds \(|\Phi|\) on the polydisc. Vanishing ([AU] §1.2): on the slice \(s=0\) off \(R\cup T\), if \(R\cup T\) misses the datum support, subordination makes \(\mathscr H\) on \({\rm core}(R)\) equal to its value at datum \(0\), which is \(0\). Hence \(\Phi=F(0)=0\) there, and \(\Phi_T=\int\partial^T(\cdot)=0\).
* Item 5 collects the constants. \(\square\)

**What Dec♯ does not do.** It gives no decay in the background, only exact localisation. It gives no decay below one tile. It does not cover the second-order rows (\(\Delta\), \(D^*D\)); they are not used in Lemma 3.4, Lemma W or (A8′). It does not prove (U1)–(U6) or (Avg).

### 2.7 Consequences for the T step

**Lemma 3.4♯ (replaces [RD] Lemma 3.4 with [AU] E3/E4) — conditional on Dec♯.** Let \(R_b\) be the tiles meeting the \((K+1)\)-neighbourhood of the \(k\)-block of \(b\) and of the \((k+1)\)-block carrying its axial contour (\(|R_b|\le2^d\)). Let \(\mathcal L_b\) be the collar of \(\mathbb B_b\). Then
\[
\hat{\mathbf H}_b(\mathbf U,\mathbf J)=\sum_T\hat{\mathbf H}_b(T;\mathbf U,\mathbf J),
\]
over sets \(T\) of \(\pi_k\)-cubes of \(\square_b^{\sim4}\setminus R_b\) with \(R_b\cup T\) \(*\)-connected and meeting \(\mathcal L_b\). Each term has (H2), (H3), (H5), (H6), (H8) on \(R_b\cup T\), and \(|\hat{\mathbf H}_b(T)|\le A_b(e^{\kappa_1}-1)^{-|T|}\) with \(A_b=A_{\mathbb G}\). Every such \(T\) has
\[
|T|\ \ge\ n_{\rm coll}:=\Bigl\lceil\frac{L(2M_2R_{k+1}-2M_1-1)}{M}\Bigr\rceil-2\ \ \ge\ \frac{2LM_2R_{k+1}}{M}-3,
\]
and, if \(\kappa_1\ge4(1+b_0)\) (\(b_0=\log(2^{d+1}(3^d-1)^2)\); \(\kappa_1\ge52.9\) for \(d=4\)),
\[
\sum_T|\hat{\mathbf H}_b(T)|\,e^{\frac12\kappa_1|T|}\ \le\ e\,A_b\,e^{-\frac14\kappa_1n_{\rm coll}}.
\tag{3.1♯}
\]
*Proof.* Dec♯(4) with \(\Phi\) the composite of [RD] Definition 2.5 read by Lemma F(3). Its local part \(F\) (datum transport, average \(M^k\) at \(b\), frames at \(b_-\)) lives in \({\rm core}(R_b)\). The distance from \(b\) to \(\mathcal L_b\) is \(\ge2M_2R_{k+1}-2M_1-1\) in \(T^{(k+1)}\) units ([RD] (B2), [III] p.256). For (3.1♯), apply Local deformation of propagators and the minimizer Lemma 5.1 with \(b=\frac12\kappa_1-1=b_0+\theta\), \(\theta\ge\frac14\kappa_1\), and \(D=n_{\rm coll}\). \(\square\)

**(CD-T) is now available without CT♯.** (3.1♯) gives [RD] Lemma 3.2(2) with \(\hat\eta_k\le eC\,\ell^q\hat B^2e^{-\frac14\kappa_1n_{\rm coll}}\). With the real datum \(44d^2B_3\varepsilon_{k+1}\) it gives Lemma 3.2(1) and Lemma 4.1, with \(\theta_k\le C\hat B^2(A_0/A_1)e^{-\frac14\kappa_1n_{\rm coll}}\). Since \(n_{\rm coll}\propto R_{k+1}\ge\ell^r_{k+1}\) and \(M\) is fixed before \(g\), the prefactor \(\hat B^2\) (\(\sim e^{1700}\)) is absorbed by a coupling ceiling. So uses U1–U4 of [RD] §10 rest on Dec♯ alone. CT♯ remains an alternative, not a requirement. conditional

**Lemma W** ([RD] §4.5 with [AU] §4.2) holds as written with (3.1♯) in place of (3.1) and \(c'=\sqrt d\) per tile (a tree through centres of \(*\)-adjacent \(\pi_k\)-cubes). Condition: \(\frac12\kappa_1\ge\sqrt d(1-4\delta)\kappa\). conditional

## 3. (A8′): the (A8) terms in passing components, written out

### 3.1 Setting

R operation at step \(k\) ([IV] §1), eligible component \(Z\), preparatory integration \(n+1\), \(j=h+n\in[h,k-1]\). Integrated bonds: \(\mathfrak B_Z:=(\Omega^c_{j+1}\setminus Z''_{j+1})^{(j)*}\cap Z\). Backgrounds: \(U^{(n+1)}_k\) (global, (1.18)) and \(U^{(n+1)}_{k,Z}\) (component, (1.20)). \(V^{(j)}=M^j(U^{(n+1)}_k)=\exp(i\mathbb H^{(j)}_Z)V^{(j)}_Z\) (1.58). (A8) is in force: the test is \(\chi(\{|B^Z_j(b)|<\delta'_j/g_j,\ b\in\mathfrak B_Z\})\) with \(V_j=e^{ig_jB^Z_j}V^{(j)}_Z\) (the representation convention convention, [AU] E6). \(Z\) is **passing**.

The integration variable of (1.60) is \(B^Z\). The chart is \(B_j(b)=\varphi_{\mathbb H_Z(b)}(B^Z(b)):=\frac1{ig_j}\log(e^{ig_jB^Z(b)}e^{-i\mathbb H_Z(b)})\) on \(\mathfrak B_Z\), written \(B_j=\Phi_Z(B^Z)\). It is a right translation in the group, so it preserves Haar measure ([RD] Lemma 2.2; [AU] §6 for the (A8) chart, deduction). Let \(\mathscr A(A_j,B_j)\) be the exponent of the integrand of (1.60), and
\[
\mathscr V_Z:=\mathscr A(A_j,\Phi_Z(B^Z))-\mathscr A(A_j,B^Z)+\log|\det D\Phi_Z(B^Z)|.
\]
Then the integrand of (1.60) in the variable \(B^Z\) is \(\chi'(B^Z)\exp[\mathscr A(A_j,B^Z)+\mathscr V_Z]\) ([RD] (2.3)). These \(\mathscr V_Z\) are "the new terms" of [AU] E1.

**The extension of \(\mathbb H_Z\).** Define \(\hat{\mathbb H}_Z(b;\mathbb U,\mathbb J)\) by [RD] Definition 2.5 with \(\mathbb B_b\) replaced by \(\mathbb G_Z:=\mathbb B^{(n+1)}_k(Z)\), \(M^k\) at \(b\) replaced by \(M^j\), and the datum
\[
B_Z(\mathbb U):=\tfrac1i\log\bigl[M_{\mathbb G_Z}(\text{component data built from }M^\cdot(\mathbb U))\,M_{\mathbb G_Z}(\mathbb U^{\rm ax})^{-1}\bigr],
\]
with the component data as in (1.20) (\(M^\cdot(Q^{s*}_kM^k(\cdot))\) on \(Z\cap\Omega_k\), the old data on \(Z\cap\Omega^c_k\)). Read it through Lemma F(3) (response at \((\mathbb U,\mathbb J)\), transported datum). The datum is supported in the \(2M_1\) boundary layer \(\mathcal L_Z\subset Z\cap\Omega_k\): (1.56) states the support, and (1.19)–(1.20) place it in \(\Omega_k\) because the data differ only where \(Q^{s*}\)-data are used. source input; additional assumption

### 3.2 Statement

> **Preliminary single-potential estimate (only the structured items 3′/4′ of [the local-test estimates](local_test_estimates.md) imply the inductive decay).**

**Theorem A8′.** Assume Dec♯ for \(\mathbb G_Z\) (all its hypotheses), and:
> * **(S9-R)** the exponent \(\mathscr A\) of (1.60) has a localised analytic expansion \(\mathscr A=\sum_Y\mathbf V(Y;\mathbb U,\mathbb J,A_j,B)\) of the type of [III] §3 ([IV] p.189, S5). Each \(\mathbf V(Y)\) is analytic on \(\tilde U^{(n+1)c}_k(Y,\tilde\alpha_0,\tilde\alpha_1)\times\{|B|<r_B\}\times\{A_j\text{-domain}\}\), gauge invariant, and bounded by \(C_Vp(g_j)^2|Y|^2e^{-(1-2\delta)\kappa d(Y)}\) in its native linear size.
> * **(Geo-Z)** the \(\ell^\infty\)-distance from \(\mathfrak B_Z\) to \(\mathcal L_Z\) is \(\ge c_ZMR_k\) in \(T^{(k)}\) units, with an absolute \(c_Z>0\).
> * **(Clu-R)** the source's expansion of (1.60) ("the same type as … Sect. 3 [III]", p.189; the bounds "easily obtained", p.191) accepts additional localised analytic potentials bounded by \(\varepsilon\) times the bounds of the source potentials (with \(\kappa\to(1-3\delta)\kappa\)), and yields \(\mathbb C\)-terms in the format (1.63), (1.70) multiplied by \(O(\varepsilon)\).
> * **(Par-g\(_Z\))** \(\varepsilon_Z:=C\,p(g_j)^2\,\ell_k^{\,q'}\,e^{-\frac14\kappa_1(c_ZR_k-2)}\le g_j^{\kappa_0+2}\), and \(\frac12\kappa_1\ge\sqrt d(1+3\beta)\kappa\), \(\kappa_1\ge4(1+b_0)\).
> Then, in every passing component:
> 1. **Extension.** \(\hat{\mathbb H}_Z(b)\), \(b\in\mathfrak B_Z\), is a function of \((\mathbb U,\mathbb J)\restriction Z\), holomorphic on \(\tilde U^{(n+1)c}_k(Z,\tilde\alpha_0,\tilde\alpha_1)\), with (H5), (H6), (H8). It equals \(\mathbb H^{(j)}_Z(b)\) of (1.58) at the construction's configurations.
> 2. **Tubes.** \(\hat{\mathbb H}_Z(b)=\sum_T\hat{\mathbb H}_Z(b;T)\), over sets \(T\) of \(\pi_k\)-cubes of \(Z\) with \(R_b\cup T\) \(*\)-connected and meeting \(\mathcal L_Z\). Each term depends on \((\mathbb U,\mathbb J)\restriction(R_b\cup T)\), is holomorphic on the space restricted there, has (H5), (H6), (H8), and \(|\hat{\mathbb H}_Z(b;T)|\le A_Z(e^{\kappa_1}-1)^{-|T|}\) with \(A_Z=A_{\mathbb G_Z}\le C\ell_k^{q}g_k\). Every such \(T\) has \(|T|\ge n_Z:=\lceil c_ZR_k\rceil-2\), and \(\sum_T|\hat{\mathbb H}_Z(b;T)|e^{\frac12\kappa_1|T|}\le eA_Ze^{-\frac14\kappa_1n_Z}\).
> 3. **Localised new potentials.** \(\mathscr V_Z=\sum_XW_Z(X)\). The index \(X\) runs over domains of \(\mathbf D_k\) of the form "smallest \(\mathbf D_k\)-domain containing \(Y\cup\bigcup_iR_{b_i}\cup T_i\)", with \(Y\) a domain of (S9-R) meeting \(\mathfrak B_Z\), \(b_i\in Y\cap\mathfrak B_Z\), and \(T_i\) tubes of \(b_i\). By the coarsening rule (1.63), \(X\) has index \(m=k\), because it meets \(\mathcal L_Z\subset\Omega_k\). Each \(W_Z(X)\):
>    * depends on \((\mathbb U,\mathbb J,A_j,B^Z)\restriction X\);
>    * is holomorphic on \(\tilde U^{(n+1)c}_k(X,\tilde\alpha_0,\tilde\alpha_1)\times\{|B^Z|<r_B-1\}\times\{A_j\text{-domain}\}\);
>    * is gauge invariant (simultaneous transformation) and covariant under the isometries preserving all partitions;
>    * vanishes if \(B_Z(\mathbb U)=0\) on \(X\), in particular at \(\mathbb U=1\);
>    * satisfies
> \[
> |W_Z(X)|\ \le\ \varepsilon_Z\,e^{-(1-5\delta)\kappa\,d_k(X)}.
> \]
> 4. **Booking.** Inserted into (1.60) as potentials, the \(W_Z(X)\) produce, by (Clu-R), additional terms of \(\mathbb C^{(n+1)}_k(X)\) in the format (1.63). They are analytic on \(\tilde U^{(n+1)c}_k(X,\tilde\alpha_0,\tilde\alpha_1)\) and satisfy **(1.70) with \(C_0\) replaced by \(C\varepsilon_Z\le g_j^{\kappa_0}C_0\)**. They are boundary terms of the R operation and are booked exactly as the source's own \(\mathbb C^{(n+1)}_k\).
> 5. **Labels.** No label changes. (FP) is unaffected.
> **Hypotheses: conditional** on Dec♯ (hence (U1)–(U6), (S-calc♯), (Avg)), (S9-R), (Geo-Z), (Clu-R), and [V] Theorem 1 and Proposition 9 as used in (1.56) (item 1's identification).

### 3.3 Proof

**Item 1.** The construction is that of [RD] Definition 2.5, so (H2), (H3), (H5), (H6), (H8) follow as in [RD] Lemma 3.3 ((H5) re-derived in [AU] §3.4, deduction), with Lemma F for the frame. Identification: (1.56) (c) states that \(U^{(n+1)}_k\restriction Z\) is the \(\mathbb G_Z\)-response at the component background to the datum (1.56). Equivalently, by uniqueness of the minimal orbit ([V] Theorem 1) and [V] Proposition 9 with reference datum \(M^\cdot(U^{(n+1)}_k)\), \(U^{(n+1)}_{k,Z}\) is the response at \(U^{(n+1)}_k\) to the reversed datum. This is [RD] Lemma 3.1 with \((U_{k+1},U_{k+1,b})\to(U^{(n+1)}_k,U^{(n+1)}_{k,Z})\). The datum is small: \(44d^2B_3\varepsilon_k\) source input. Then \(M^j\) at \(b\) gives (1.58).

**Item 2.** This is Dec♯(4) for \(\mathbb G_Z\), with root \(R_b\) and the composite of item 1. The size \(A_Z\): Lemma D with Lemma N's (R)-parameters on \(\mathcal L_Z\subset\Omega_k\), where the space imposes the level-\(k\) clause, gives \(|B_Z|\le C_B\cdot3L_0^{2N_0}(BCM\alpha_{0,k}+\alpha_{1,k})\le C\ell_k^qg_k\). Count: by (Geo-Z), a \(*\)-connected chain of \(\pi_k\)-cubes from the cube of \(b\) to \(\mathcal L_Z\) has \(\ge c_ZR_k-2\) cubes. The sum is Local deformation of propagators and the minimizer Lemma 5.1, as in (3.1♯).

**Item 3.** This is [RD] Lemma W step 3, as written out in [AU] §4.2, with:
* \(\rho_H=\frac12g_j\) (the chart is analytic for \(|g_jB^Z|,|\mathbb H|\le\rho_0\) and shifts \(B\) by \(\le2g_j^{-1}|\mathbb H|\le1\));
* \(\hat\eta_Z:=\sup_b\sum_T|\hat{\mathbb H}_Z(b;T)|e^{\frac12\kappa_1|T|}\le eA_Ze^{-\frac14\kappa_1n_Z}\);
* \(x_Y=2n_c|Y^*|\hat\eta_Z/\rho_H\le C|Y^*|\ell_k^q(g_k/g_j)e^{-\frac14\kappa_1n_Z}\), where \(g_k\le g_j\).

For a source term \(Y\), \(w(Y)=\mathbf V(Y;\Phi_Z(B^Z))-\mathbf V(Y;B^Z)\) is analytic on the polydisc \(|\mathbb H_b|<\rho_H\), \(b\in Y\cap\mathfrak B_Z\), and vanishes at \(\mathbb H=0\). The Jacobian contributes one-bond terms of the same kind. Expand in \(\mathbb H\), substitute item 2, and collect by the union \(X\). Then:
* \(d_k(X)\le d(Y)+1+\sqrt d\sum_i(|T_i|+1)\), since coarsening to \(\mathbf D_k\) does not increase the linear size, and the root and tubes consist of \(\pi_k\)-cubes joined to \(Y\) inside the cube of \(b_i\);
* the weights \(e^{-\frac12\kappa_1|T_i|}\) pay \(e^{-\sqrt d(1+3\beta)\kappa|T_i|}\);
* \(S_Yx_Ye^{x_Y}\le C_Vp^2|Y|^2e^{-(1-2\delta)\kappa d(Y)}\cdot C|Y^*|\ell^qe^{-\frac14\kappa_1n_Z}\cdot e^{\delta\kappa d(Y)}\), using (Par-g\(_Z\)) to absorb \(e^{x_Y}\) and the polynomial factors;
* the sum over \(Y\subset X\) is \(\le C(d_k(X)+1)\) ([AU] §4.2).

This gives \(|W_Z(X)|\le\varepsilon_Ze^{-(1-5\delta)\kappa d_k(X)}\). Locality, analyticity and covariance hold term by term: Dec♯(3)–(4), and joint invariance of the source terms with \(\Phi_Z\) commuting with \(R(u)\). Vanishing: (H8) and \(w=0\) at \(\mathbb H=0\). The coarsening index: \(X\supset T_i\), \(T_i\) meets \(\mathcal L_Z\subset\Omega_k\), and \(\Omega_{k+1}=\emptyset\) in (1.63), so \(m=k\).

**Item 4.** The potentials \(W_Z(X)\) satisfy (Clu-R)'s input hypothesis with \(\varepsilon=\varepsilon_Z\) (item 3; analyticity domain as in [IV] (1.64)–(1.69) restricted to \(X\), radius in \(B^Z\) reduced by 1). The \(\delta\)-loss \(3\delta\kappa\) is absorbed as for every newly created term (the source chooses \(\delta\) small, [II] (1.36)), exactly as in [RD] Theorem 4.5. (Clu-R) then gives the format (1.63) and the bound (1.70) times \(C\varepsilon_Z\). (Par-g\(_Z\)) makes this \(\le g_j^{\kappa_0}C_0\), which is "with room" in the sense the source needs for cumulating \(\le N_0\) contributions (p.191–192: the terms "are multiplied by \(g_j\)").

**Item 5.** The chart and the extension change the representation, not the test. \(\square\)

**On (Geo-Z).**
* For \(j\le k-2\): \(\mathfrak B_Z\subset\Omega^c_{j+1}\) and \(\mathcal L_Z\subset\Omega_k\subset\Omega_{k-1}\). [III] p.256 (c) gives \({\rm dist}(\Omega^c_{k-1},\Omega_k)\ge2MR_{k-1}\) in level-\((k-1)\) units. Reading this as a Euclidean separation additional assumption, it is \(\ge2MR_{k-1}/L\ge2MR_k/L^2\) in \(T^{(k)}\) units ((G5): \(R_{k}/R_{k-1}\le L\)), so \(c_Z\ge2/L^2\).
* For \(j=k-1\): the separation is the level-\(k\) summand \(MR_k\) of (1.57)'s exponent source input, read as a Euclidean distance additional assumption. It is also the one-layer separation of \(S_k\) from \(\Lambda_k\) ((3.20) [III], quoted in [RD] (B5), c\*).

[AU] §5.2 item 3 says the tube length is "proportional to the scaled distance \(10M(R_{j+1}+\dots+R_{k-1})+MR_k\)". On one uniform tile scale this is not right: the fine-level summands count with weight \(L^{i-k}\). Only the bound \(\gtrsim R_k\) is true, and only it is needed.

### 3.4 Failing components

In components with the large-field function \(1-\chi'^{(j)}\), the (A8) test is the source's (1.59) with cutoff 1 ([RD] §2.6). The terms created by the change of variables stay in the new large-field region and are treated by the source's large-field bounds, as in the literal construction ([AU] §5.2, last sentence). They need no (1.70), because the component leaves \(Z\). Nothing to add. source input; additional assumption
