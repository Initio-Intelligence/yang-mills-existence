# Yang–Mills existence through observable derivatives

*Proved reductions and remaining construction theorems*

**Abstract.** The source-free RG/R construction, with its maps and selectors frozen at zero source, is developed into a concrete conditional construction program. Exact jet transport and a scale-by-scale covariance identity are proved. A joint off-diagonal kernel estimate is shown to imply the corrected Osterwalder–Schrader growth condition, with one fixed factorial exponent. The Gaussian diagnostic is extended to all orders, and an explicit example shows why its scalar stationarity cancellation does not extend to constant tensor marks. Further reductions identify six angular defects sufficient for rotations, an arbitrary-vector heat-semigroup estimate sufficient for polynomial energy bounds, and a central-projection estimate sufficient for transferring ultraviolet coefficients to pure phases. None of the central interacting marked estimates is established here. This note is an incomplete existence argument with precisely stated remaining obligations, not a construction of four-dimensional Yang–Mills theory.

## Contents

1. Conclusion and fixed target
2. Source-free base and normalization
3. Exact frozen transport and the first two-point target
4. What the Gaussian calculation establishes
5. A joint kernel estimate that closes OS regularity
6. The interacting marked theorem still to prove
7. Positivity, compactness, and rotations
8. Energy bounds and phasewise ultraviolet identification
9. Conditional assembly and completion criteria
10. Interface statement

## 1. Conclusion and fixed target

The route developed here removes unnecessary finite-source demands while preserving the substantial work that reconstruction actually requires. The decisive missing result is a cutoff- and volume-uniform theorem for renormalized local insertions on the *complete compact Wilson measure*, including its large-field histories. The exact positive transport identities do not establish that estimate.

The target here is the reduced form P1 of the existence problem: a continuum limit along one cofinal Wilson sequence, the finite gauge-invariant field family of engineering dimension at most four, corrected OS regularity, full Euclidean covariance, reflection positivity, symmetry, the specified energy bounds and phase selection, and quantitative asymptotically free short-distance identification. No mass gap, confinement, uniqueness of the continuum limit, or all-dimensional composite family is added. If P1 quantifies all compact simple groups, its group dependence must also be proved; the displayed Wilson convention below is for fixed \(SU(N)\).

**Status labels.** **(P)** means proved here under the hypotheses stated in the proposition. **(L)** identifies a precisely scoped literature input. **(C)** marks an assembly implication whose substantive hypotheses remain unproved for Yang–Mills. **(O)** marks a required interacting estimate. In particular, a proved implication with an open hypothesis is not an unconditional Yang–Mills result.

### 1.1 The full finite field family

For the stated polynomial class and a compact simple Lie algebra, the positive-dimensional fields of dimension at most four are the curvature bilinears
\[
 Q_{\mu\nu,\rho\sigma}=\operatorname{Tr}(F_{\mu\nu}F_{\rho\sigma}).
 \tag{1}
\]
Fix the sign and normalization of the invariant quadratic form. Antisymmetry in each index pair and symmetry under exchange of pairs put this family in
\[
 \operatorname{Sym}^2(\Lambda^2\mathbb R^4),\qquad
 \dim\operatorname{Sym}^2(\Lambda^2\mathbb R^4)=6\cdot7/2=21.
 \tag{2}
\]
The identity is an additional mixing direction. The scalar, pseudoscalar, and symmetric traceless stress-type channels account for \(1+1+9=11\) components; ten further curvature-bilinear components remain. Indeed, \(\Lambda^2=\Lambda^2_+\oplus\Lambda^2_-\) gives the \(SO(4)\) decomposition \((1+5)+(1+5)+9\). No linear algebraic Bianchi identity should be imposed on these bilinears without justification. A scalar construction therefore does not finish the finite tensor family.

## 2. Source-free base and normalization

With the same plaquette-counting convention, set
\[
 s_p=N-\operatorname{Re}\operatorname{Tr}U_p,\qquad
 S=\sum_p s_p,\qquad
 A_B=\sum_p\Bigl(1-\frac1N\operatorname{Re}\operatorname{Tr}U_p\Bigr)=S/N.
 \tag{3}
\]
The bare action is specified as \(2Nx_0S\). Consequently
\[
 \boxed{\,2Nx_0S=X_{B,0}A_B,\qquad X_{B,0}=2N^2x_0.\,}
 \tag{4}
\]
If \(X_{B,k+1}=X_{B,k}-b_B\log L+r_{B,k}\), then
\[
 x_{k+1}=x_k-\frac{b_B}{2N^2}\log L+\frac{r_{B,k}}{2N^2}.
 \tag{5}
\]
Also \(\partial_x=2N^2\partial_{X_B}\). An \(m\)-fold coupling derivative changes by \((2N^2)^m\). Older numerical beta coefficients or short-distance coefficients must be converted before reuse.

**(L)** Balaban's LFR II, Theorem 1 and (0.1), pp.355–356, provide the complete source-free effective-density representation and stability bounds under the assumption that all effective couplings remain sufficiently small [2]. That source explicitly treats physical observable estimates as further work. Its statement that the trajectory theorem's proof had not been published is a statement made in 1989; this note does not turn it into an unverified claim about the entire subsequent literature.

CMP109 uses normalized trace and an odd block parameter \(L>11\) in its initial geometry; further choices in the complete construction must also be respected [5]. Fix one sufficiently large admitted odd \(L\), rather than claiming all odd \(L\ge3\). Use
\[
 a_n=L^{-K_n}\ell_0,\qquad T_n=2L^{M_n}\ell_0,\qquad K_n,M_n\longrightarrow\infty,
 \tag{6}
\]
with all required coarse-size conditions. The \(\eta\)-scale volume conventions in CMP109 and CMP119 are consistent with counting coarse volume in the stability estimate [5, 3].

**Working premise.** The construction may proceed assuming its trajectory input N2-F and the exact source-free base. N2-F is not proved in this note; a final proof must supply and check that input, including its identification with \(X_B=2N^2x\). Even granting this premise, the observable and operator estimates below remain open.

The primary effective-action and cluster-expansion papers CMP109 and CMP116 [5, 6] provide the relevant source-free localization machinery, not the new marked induction by themselves.

## 3. Exact frozen transport and the first two-point target

### 3.1 Transport as conditional expectation

Let a positive source-free operation act on densities by \(P\), preserve integrals, and send \(\rho\) to \(\rho'=P\rho\). On nonzero output support define
\[
 QF=\frac{P(\rho F)}{\rho'}.
 \tag{7}
\]
For the localized positive R replacement, \(P\) has the normalized-kernel form (4) of [Conditional reconstruction from Wilson source derivatives](local_sources/assembly_and_counterexamples.md). More generally use the positive history lift before introducing signed polymer activities. The old and new normalized measures then admit a joint probability law with
\[
 QF=\mathbb E[F\mid\text{output}],\qquad Q1=1,\qquad
 \mathbb E_{\mu'}QF=\mathbb E_\mu F,\qquad
 \|QF\|_{L^p(\mu')}\le\|F\|_{L^p(\mu)}.
 \tag{8}
\]
Signed activity terms are not individual probability measures. No step below treats them as such. The actual localized R formula and its integral identity are LFR I (1.100), (1.102), p.201 [1].

**Proposition 3.1** (All finite source jets, **(P)**). *Work with distinct formal labels \(t_1,\ldots,t_M\) and truncate above total source degree \(M\). If \(G_k(0)=1\), \(\Psi_k=\log G_k\), and \(G_{k+1}=Q_kG_k\), then for each nonempty label set \(I\),*
\[
 \Psi^I_{k+1}=\sum_{\pi\in\Pi(I)}\kappa_{Q_k}\bigl(\Psi^B_k:B\in\pi\bigr).
 \tag{9}
\]
*Every integrated coefficient of \(G_k\) is unchanged along the transport.*

*Proof.* The conditional cumulant expansion is the formal identity \(\log Qe^\Psi=\sum_{r\ge1}\kappa_Q(\Psi,\ldots,\Psi)/r!\). At source degree at most \(M\), the sum is finite. Extracting the mixed coefficient indexed by \(I\) groups its labels into the blocks of a partition, giving (9). Integral preservation holds coefficient by coefficient. No convergent cutoff-independent exponential-source series or zero-free region is assumed. \(\square\)

The degree-two formula includes a conditional covariance. More generally, at degree \(m\) the term \(Q_k\Psi^I_k\) is linear in the old degree-\(m\) coefficient; every other term uses smaller blocks. This triangular structure is useful, but each term still needs a spatial and scale estimate.

**Proposition 3.2** (Covariance telescoping, **(P)**). *Let \(F_0,G_0\in L^2(\mu_0)\), \(F_{k+1}=Q_kF_k\), \(G_{k+1}=Q_kG_k\), and*
\[
 D_k=Q_k(F_kG_k)-F_{k+1}G_{k+1}.
 \tag{10}
\]
*Then for \(K\) exact positive transport steps,*
\[
 \boxed{\,\operatorname{Cov}_{\mu_0}(F_0,G_0)=\sum_{k=0}^{K-1}\mathbb E_{\mu_{k+1}}D_k+\operatorname{Cov}_{\mu_K}(F_K,G_K).\,}
 \tag{11}
\]

*Proof.* Integral preservation gives \(\mathbb E_{\mu_k}F_kG_k=\mathbb E_{\mu_{k+1}}Q_k(F_kG_k)\) and preserves both means. Add and subtract \(\mathbb E_{\mu_{k+1}}F_{k+1}G_{k+1}\) to obtain the one-step identity, and sum. Nested sigma-algebras are unnecessary; each step has its own valid joint-law conditional expectation. \(\square\)

### 3.2 A first interacting milestone with a checkable exit criterion

Use the renormalized scalar field at separated points, with running normalization and identity subtraction fixed at \(\mu\). Formula (11) is exact for its finite-cutoff lattice representatives. Constants subtracted from individual fields do not affect this covariance. Contact stencils are handled by their separate locality estimates.

**(O)** A concrete sufficient first target is an all-history estimate for each shell of physical size \(h\),
\[
 \mathbb E\,|D_h(x,y)|\le Bh^{-8}\bigl(1+\log(\ell_0/h)\bigr)^be^{-c|x-y|/h},\qquad a\le h\le\ell_0,
 \tag{12}
\]
and a terminal bound \(|\operatorname{Cov}_{\mu_K}(F_K(x),F_K(y))|\le B\ell_0^{-8}\) on the region considered. The constants must be independent of cutoff, number of RG steps, and torus along the chosen sequence. The expectation is over the actual normalized source-free histories; it is not a bound only in a regular background or in a selected small-field sector.

**Lemma 3.3** (Summing the two-point shells, **(P)**). *For geometric scales \(h_j=\ell_0L^{-j}\), \(b\ge0\), \(c>0\), and \(0<r\le\ell_0\),*
\[
 \sum_{j\ge0}h_j^{-8}\bigl(1+\log(\ell_0/h_j)\bigr)^be^{-cr/h_j}\le Cr^{-8}\bigl(1+\log(\ell_0/r)\bigr)^b.
 \tag{13}
\]

*Proof.* Choose the scale \(h_*\) with \(r\le h_*<Lr\). For larger scales \(h=L^\ell h_*\), the factor \(h^{-8}\) supplies \(L^{-8\ell}\) and the logarithm is no larger than the right-hand logarithm up to a fixed constant. For smaller scales \(h=L^{-\ell}h_*\), put \(u=r/h\). The term is bounded by \(Cr^{-8}L^{8\ell}e^{-c'L^\ell}(1+\log(\ell_0/r)+\ell\log L)^b\). The double-exponentially decaying factor makes the sum converge, even after the polynomial in \(\ell\) is included. The two pieces give (13). \(\square\)

Thus (12), together with the terminal estimate, proves a separated scalar two-point bound. If the actual localization radius has logarithmic corrections, one must prove summability of its actual decay profile instead of replacing it silently by \(e^{-cr/h}\). This milestone is significant but does not give all orders, tensor mixing, or nontriviality.

## 4. What the Gaussian calculation establishes

Let \(D\) be the linearized curvature map, \(T\) the constrained fluctuation inclusion, and \(m\) the source-free minimizer, with \(T^*D^*Dm=0\). Set \(H=xT^*D^*DT>0\), \(C=H^{-1}\). For
\[
 O_i=c_i+b_i^Tz+\tfrac12z^TV_iz,\qquad z\sim N(0,C),
 \tag{14}
\]
put \(A_i=C^{1/2}V_iC^{1/2}\) and \(u_i=C^{1/2}b_i\). The exact formal identity is
\[
 \log\mathbb Ee^{\sum_it_iO_i}=c(t)+\frac12\sum_{r\ge1}\frac{\operatorname{Tr}A(t)^r}{r}+\frac12\sum_{r\ge0}u(t)^TA(t)^ru(t).
 \tag{15}
\]
It follows by completing the square; analytically it holds on the Gaussian convergence domain, and formally it holds to any finite degree.

For distinct labels \(1,\ldots,m\), the determinant contribution to the cumulant is
\[
 \frac1{2m}\sum_{\sigma\in S_m}\operatorname{Tr}\bigl(A_{\sigma(1)}\cdots A_{\sigma(m)}\bigr).
 \tag{16}
\]
For \(m\ge2\) the background contribution is
\[
 \frac12\sum_{\sigma\in S_m}u^T_{\sigma(1)}A_{\sigma(2)}\cdots A_{\sigma(m-1)}u_{\sigma(m)}.
 \tag{17}
\]
For \(m=2\) these are \(\tfrac12\operatorname{Tr}(CV_1CV_2)+b_1^TCb_2\). The formulas expose both loops and retained-background chains; determinant estimates alone omit the latter.

For scalar multiplication marks, specialize to \(V_f=T^*D^*M_fDT\), \(b_f=T^*D^*M_fDm\), and \(c_f=\tfrac12\langle Dm,M_fDm\rangle\). Then \(\sqrt x\,DTC^{1/2}\) is an isometry. Hence \(\|A_i\|\le x^{-1}\|f_i\|_\infty\). Put \(\omega_i=\|f_i-f_{i,*}\|_\infty\) and let \(M\) be the fluctuation dimension. Stationarity and the dual quadratic-form norm give \(\|u_i\|\le x^{-1/2}\omega_i\|Dm\|\). Therefore, for \(m\ge2\),
\[
 |\kappa^{\rm vac}_m|\le\frac{(m-1)!\,M}{2x^m}\prod_i\|f_i\|_\infty,
 \tag{18}
\]
\[
 |\kappa^{\rm bg}_m|\le\frac{(m-2)!\,\|Dm\|^2}{2x^{m-1}}\sum_{i\ne j}\omega_i\omega_j\prod_{l\ne i,j}\|f_l\|_\infty.
 \tag{19}
\]
The second formula follows by fixing the ordered endpoint labels and counting the \((m-2)!\) interior permutations. This proves the two-endpoint scalar oscillation gain at every order. It still leaves the fluctuation dimension, background energy, spatial localization, and complete history average to be controlled.

### 4.1 The scalar cancellation is not a tensor cancellation

For scalar multiplication \(M_f\), stationarity gives \(b_f=T^*D^*(M_f-f_*I)Dm\), hence the endpoint gradient factors in the scalar Gaussian calculation. A constant tensor matrix need not be proportional to \(I\).

**Proposition 4.1** (Constant tensor counterexample, **(P)**). *Take \(D=I_2\), \(Tz=(z,0)\), \(m=(0,1)\), and*
\[
 M=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
 \tag{20}
\]
*Then \(T^*D^*Dm=0\) and \(C=1/x\), but*
\[
 \tfrac12(m+Tz)^TM(m+Tz)=z,\qquad b=1,\qquad \operatorname{Cov}(O,O)=1/x.
 \tag{21}
\]
*The tensor source is constant, while its background response is nonzero.*

This is a finite-dimensional diagnostic, not a Yang–Mills counterexample. It shows that the tensor induction must retain its constant-source marginal responses. Freezing the minimizer remains exact; discarding those responses does not.

### 4.2 A complete Gaussian hierarchy diagnostic

Suppose a centered finite-component Gaussian curvature field has covariance \(\Gamma_n\) satisfying, for distinct points,
\[
 \bigl|\Gamma^{ab}_n(x,y)\bigr|\le K\max\{1,|x-y|^{-4}\}
 \tag{22}
\]
uniformly in the cutoff. Let each observable be a fixed Wick quadratic form with bounded coefficients in those components. At \(m\) pairwise distinct points, Wick's rule contracts \(2m\) legs into \(m\) edges. Each edge contributes at most \(K\delta_m^{-4}\), where \(\delta_m=\min(1,\min_{i<j}|x_i-x_j|)\). The number of pairings is
\[
 (2m-1)!!=\frac{(2m)!}{2^mm!}\le2^mm!.
 \tag{23}
\]
Summing the finite component indices and coefficients therefore gives the full Gaussian bound
\[
 \bigl|S^{\rm G}_{m,n}(x_1,\ldots,x_m)\bigr|\le C^mm!\,\delta_m^{-4m}.
 \tag{24}
\]
Together with the next section this proves the corrected OS growth bound in this Gaussian diagnostic. Hypothesis (22) for the relevant physical kernels, and its use through all nonlinear histories, are distinct issues. This calculation does not replace the compact Wilson measure.

## 5. A joint kernel estimate that closes OS regularity

This section supplies a concrete sufficient output for the marked theorem. It avoids identifying separate tensor-product estimates with a uniform joint-distribution estimate.

**Definition 5.1.** Let \(\Delta_m=\bigcup_{i<j}\{x_i=x_j\}\) and
\[
 \mathcal S_0(\mathbb R^{4m})=\{F\in\mathcal S(\mathbb R^{4m}):\partial^\alpha F|_{\Delta_m}=0\text{ for all }\alpha\}.
 \tag{25}
\]
Write \(|X|^2=\sum_i|x_i|^2\) and
\[
 \nu_s(F)=\max_{|\alpha|\le s}\sup_X(1+|X|^2)^{s/2}|\partial^\alpha F(X)|.
 \tag{26}
\]
Set \(\delta_1=1\) and \(\delta_m(X)=\min(1,\min_{i<j}|x_i-x_j|)\) for \(m\ge2\).

**Theorem 5.2** (Kernel bound implies the full OS growth condition, **(P)**). *Suppose connected kernels exist away from \(\Delta_m\) and, uniformly in \(n\) and all field labels, obey*
\[
 |C_{m,n}(X)|\le A^{m+1}(m!)^p\delta_m(X)^{-\sigma m}(1+|X|^2)^{bm/2},
 \tag{27}
\]
*where \(A\ge1\), \(\sigma,b\ge0\), and \(p\ge1\) are fixed. Form full kernels by the partition identity. For any fixed integer \(q>\max\{\sigma,b+4\}\), there is \(B\) independent of \(m,n\) such that*
\[
 |S_{m,n}(F)|\le B^{m+1}(m!)^p\nu_{qm}(F),\qquad F\in\mathcal S_0.
 \tag{28}
\]
*The same conclusion holds if (27) is assumed directly for full kernels. Controlled contact remainders may be added as specified below.*

*Proof.* First consider the partition sum. For \(p\ge1\), \(\prod_{B\in\pi}|B|!\le m!\) gives
\[
 \sum_{\pi\in\Pi_m}\prod_{B\in\pi}(|B|!)^p\le(m!)^{p-1}\sum_{\pi\in\Pi_m}\prod_{B\in\pi}|B|!
 \tag{29}
\]
\[
 =(m!)^p\sum_{k=1}^m\frac1{k!}\binom{m-1}{k-1}\le2^{m-1}(m!)^p.
 \tag{30}
\]
For fixed \(k\), the equality follows by ordering the blocks, choosing their positive sizes, assigning all labels, and dividing by \(k!\). The factors \(A^{m+|\pi|}\) are at most \(A^{2m}\). Since \(\delta_{|B|}(X_B)\ge\delta_m(X)\) and the polynomial weights multiply to at most \((1+|X|^2)^{bm/2}\), the full kernel has the same bound with a larger exponential base and the same \(p\).

Suppose next that \(\delta=\delta_m(X)<1\). Let \(Y\) be the orthogonal projection obtained by replacing a nearest pair by its midpoint. Then \(Y\in\Delta_m\), \(V=X-Y\) has only eight potentially nonzero coordinates, \(\|V\|_1\le2\delta\), and \(|V|^2=\delta^2/2\). Also \(Y\perp V\), so along \(Y+tV\),
\[
 \frac{1+|X|^2}{1+|Y+tV|^2}\le\frac32.
 \tag{31}
\]
Take \(r=\lceil\sigma m\rceil\) when \(\sigma>0\). Flatness kills every Taylor coefficient below order \(r\). The integral remainder yields
\[
 |F(X)|\le\frac{(2\delta)^r}{r!}(3/2)^{qm/2}\nu_{qm}(F)(1+|X|^2)^{-qm/2}.
 \tag{32}
\]
Here \(r\le qm\). The factor \(\delta^{r-\sigma m}\) is at most one after multiplication by the kernel. When \(\delta=1\), or \(\sigma=0\), the direct Schwartz bound suffices. Constants depending only on \(q,\sigma\) are exponential in \(m\).

It remains to integrate \((1+|X|^2)^{-(q-b)m/2}\). Put \(c=(q-b)/2>2\). Since
\[
 \Bigl(1+\sum_i|x_i|^2\Bigr)^{-cm}\le\prod_{i=1}^m(1+|x_i|^2)^{-c},
 \tag{33}
\]
the integral is bounded by \([\int_{\mathbb R^4}(1+|x|^2)^{-c}\,dx]^m\). This gives (28). \(\square\)

For the Gaussian bound (24), \(\sigma=4\), \(b=0\), and \(q=8\) are safe choices. Logarithmic singular factors can often be absorbed by a fixed small increase in \(\sigma\), provided their order dependence is explicitly controlled.

### 5.1 Lattice sampling and contacts

The proof also applies to \(a^{4m}\sum_X\) in place of integration: for \(a\le1\), \(a^4\sum_{x\in a\mathbb Z^4}(1+|x|^2)^{-c}\) is uniformly bounded. Exact collisions contribute zero for flat sampled tests. On expanding tori, embed compact tests in the central region; for global Schwartz tests use product cutoffs \(0\le\chi_n\le1\), invariant under reflection, equal to one on expanding central regions, and supported where torus and Euclidean pair distances agree. Apply the kernel proof directly to \(F\), keeping the cutoff factors bounded by one, so no cutoff derivatives enter that bound. For differentiated contact errors, choose one fixed Gevrey cutoff with \(\|\partial^r\chi\|_\infty\le C^{r+1}(r!)^s\) for a fixed \(s\); the derivative cost at order \(qm\) then increases the factorial exponent by at most a fixed amount. At every fixed order the cutoff embeddings converge in the Schwartz topology.

An exact finite-order distribution supported on \(\Delta_m\) annihilates \(\mathcal S_0\). A lattice stencil supported within width \(w_n\to0\) need not have this property without a coefficient bound. Require its contribution \(E_{m,n}\) to obey, for fixed \(q_c,p_c,B_c\),
\[
 |E_{m,n}(F)|\le B_c^{m+1}(m!)^{p_c}\epsilon_n\nu_{q_cm}(F),\qquad\epsilon_n\to0,
 \tag{34}
\]
or a comparably explicit bounded approximation scheme. If derivative orders grow faster than linearly in \(m\), or coefficients grow faster than every factorial power, coincidence support at each fixed order does not recover the required common estimate.

**Useful simplification.** OS reconstruction on \(\mathcal S_0\) does not require choosing a convergent extension of every Schwinger function onto all coincidence diagonals. Full moments of individually renormalized local lattice fields are a particularly direct starting point. Product counterterms remain useful internally and for additional prescribed normalization data; they need not be promoted to a globally convergent finite-source functional.

## 6. The interacting marked theorem still to prove

### 6.1 A concrete sufficient output

**(O)** Prove (27), or its direct full-kernel version, for the actual renormalized Wilson hierarchy along the chosen cofinal sequence. Its important quantifiers are
\[
 \exists A,p,\sigma,b\quad\forall m,n,\ \forall\alpha_1,\ldots,\alpha_m\in\mathcal A,
 \tag{35}
\]
with no factor growing with the number of RG steps or the total torus volume. For a density-only statement, use physical coordinates and dimensionless units set by \(\ell_0\).

A sufficient constructive certificate is a decomposition of the renormalized, off-diagonal connected kernel into marked terms \(\mathcal K_{m,n,\omega,\tau}\) for which
\[
 \sum_{\omega,\tau}\int|\mathcal K_{m,n,\omega,\tau}(X;v)|\,d\mu_{n,\omega}(v)\le A^{m+1}(m!)^p\delta_m(X)^{-\sigma m}(1+|X|^2)^{bm/2}.
 \tag{36}
\]
Here \(\sum_\omega\mu_{n,\omega}\) has total mass one on the positive history lift, and \(\tau\) indexes the subsequent signed expansion after local renormalization. This is a sufficient, potentially stronger-than-necessary absolute estimate. It demands an average with the actual history weights, not a uniform bound on every exceptional history separately. The decomposition, norms, and denominator cancellations must be derived from the localized formulas, not assumed from a schematic quotient.

### 6.2 Local types and remainders

Power counting organizes the local subtraction list but does not prove the analytic estimates. If a cluster \(B\) of inserted fields of dimensions \(d_i\le4\) produces a local operator of dimension \(d_\beta\), its superficial subtraction degree is
\[
 \omega_{B,\beta}=\sum_{i\in B}d_i-4(|B|-1)-d_\beta\le4-d_\beta.
 \tag{37}
\]
For dimension-four external marks, identity terms therefore allow at most four source-position derivatives, while dimension-four output fields allow zero. Gauge covariance and the Ward identities are needed to justify the actual finite relevant/marginal type list. The irrelevant remainder contains all higher-dimensional vertices generated by the dynamics; it is retained and estimated, even though those vertices are not added to the external field family.

The induction must bound the homogeneous degree-\(m\) transport in (9), the lower-degree conditional-cumulant source terms, local mixing coefficients, and the remainder in a norm whose order weights close with fixed \(p\). Overlapping collision subclusters need compatible forest subtractions. The powers in (37) do not establish this compatibility or convergence by themselves.

### 6.3 A specific all-order obstruction to a crude large-field estimate

Suppose an estimate produces \(g^{-cm}\) and one tries to absorb it into a large-field factor \(\exp[-A(\log g^{-2})^s]\). With \(t=\log g^{-2}\) and \(s>1\),
\[
 \sup_{t\ge0}\exp\{(c/2)mt-At^s\}=\exp\{C_{A,c,s}m^{s/(s-1)}\}.
 \tag{38}
\]
Differentiating the exponent proves the formula. Its growth exceeds \(B^m(m!)^p\) for every fixed \(B,p\). For \(s=1\), the supremum is infinite at sufficiently large \(m\). Thus absorbing each fixed mark order into a rare-field penalty does not establish J2.

One possible repair keeps physical scale and moment order together. If AF control gives \(g(h)^{-2}\le C(1+\log(\ell_0/h))\), then, for every \(\varepsilon>0\),
\[
 g(h)^{-cm}\le D_\varepsilon^m(\ell_0/h)^{\varepsilon m}.
 \tag{39}
\]
This follows by taking the supremum of \((1+t)^{c/2}e^{-\varepsilon t}\) once, before raising it to \(m\). It increases the singular order only linearly in \(m\), which the OS bound permits. It is not a full solution: the residual scale sum and the actual large-field geometry still have to close. Alternatively, direct integrated moment regulators may supply the required factorial growth.

## 7. Positivity, compactness, and rotations

### 7.1 A positivity route requiring no exponential-source convergence

Choose running local linear field mixing and real identity subtractions equivariant under reflection, with stencil radius tending to zero. At each cutoff, full moments of these actual random variables inherit Wilson reflection positivity on positive-time tests with sufficient support margin. Use the standard ordered positive-time OS test kernels, so that the combined reflected kernels belong to the coincidence-flat test space. Arbitrary overlapping products of one-point test functions should not be identified with this space without a separate extension argument.

If additional scalar source counterterms are used, the splitting rule
\[
 C(\Theta\bar f+g)=\overline{C(f)}+C(g)
 \tag{40}
\]
preserves the exponential reflection kernel by diagonal congruence, and finite jets by a triangular transformation of the positive-time algebra. Nonlinear source redefinitions require the corresponding locality and reflection splitting. These are sufficient mechanisms; the actual scheme must meet them.

### 7.2 Compactness

Given (28), choose a countable dense set in each \(\mathcal S_0(\mathbb R^{4m})\), for each of the finitely many label tuples at each \(m\). Diagonal subsequence extraction gives simultaneous convergence. The common seminorm bound extends the limit and convergence to every test. Positivity of each fixed finite OS quadratic form, permutation symmetry, and correctly controlled translation defects pass to the limit. No mass gap or clustering is used. This is the compactness part of the conditional assembly theorem of [Conditional reconstruction from Wilson source derivatives](local_sources/assembly_and_counterexamples.md).

### 7.3 Six angular identities suffice

Let \(\mathcal L_{\mu\nu}\) be the infinitesimal test action for a coordinate-plane rotation, including all tensor indices:
\[
 \mathcal L_{\mu\nu}=\sum_{i=1}^m\bigl(x_i^\mu\partial_{x_i^\nu}-x_i^\nu\partial_{x_i^\mu}\bigr)+\sum_{i=1}^mJ^{(i)}_{\mu\nu}.
 \tag{41}
\]
The sign of \(J\) is fixed by the chosen contragredient test representation.

**Proposition 7.1** (Angular-defect reduction, **(P)**). *It suffices to prove, for all fixed \(m,F\) and the six pairs \(\mu<\nu\),*
\[
 S_{m,n}(\mathcal L_{\mu\nu}F)\longrightarrow0.
 \tag{42}
\]
*Every limit is then \(SO(4)\) covariant. An inherited orientation-reversing symmetry with the correct tensor action gives \(O(4)\) covariance.*

*Proof.* The limit obeys \(S_m(\mathcal L_{\mu\nu}F)=0\). The rotation action is differentiable on the Schwartz test space and preserves flatness. Hence \(\frac{d}{dt}S_m(e^{t\mathcal L_{\mu\nu}}F)=0\). Coordinate-plane rotations generate \(SO(4)\). \(\square\)

**(O)** The vanishing in (42) remains unproved. Bare factors such as \(a^2\) in a dimension-six lattice artifact cannot be used without controlling its mixing into dimension-four fields and the identity. For a dimension-six *density*, those power divergences have dimensions \(a^{-2}Q_4\) and \(a^{-6}\mathbf 1\); after multiplication by \(a^2\), the identity coefficient is \(a^{-4}\). Averaging a hypercubic limit over rotations does not establish its needed reflection positivity or its status as the stated Wilson limit.

**(L)** Once the corrected growth, covariance, positivity, and symmetry hypotheses hold, OS II supplies reconstruction without imposing clustering, with a possibly nonunique vacuum. The relevant statements are §IV.1, pp.287–288, and Remarks 5–6, p.283 [7]. They do not supply the marked estimates or the angular defects.

## 8. Energy bounds and phasewise ultraviolet identification

### 8.1 An explicit sufficient energy estimate

**Proposition 8.1** (Heat regularization implies a polynomial energy bound, **(P)**). *Let \(H\ge0\) be self-adjoint and \(\phi_\alpha(f)\) closed. Suppose \(e^{-tH}\mathcal H\subset D(\phi_\alpha(f))\) and*
\[
 \bigl\|\phi_\alpha(f)e^{-tH}\bigr\|\le C\nu_s(f)t^{-r},\qquad0<t\le1,
 \tag{43}
\]
*for fixed \(r\ge0\), \(s\), \(C\) across the finite field family. Then for every \(R>r\),*
\[
 \bigl\|\phi_\alpha(f)(1+H)^{-R}\bigr\|\le C_R\nu_s(f).
 \tag{44}
\]

*Proof.* Use the spectral formula
\[
 (1+H)^{-R}=\frac1{\Gamma(R)}\int_0^\infty t^{R-1}e^{-t}e^{-tH}\,dt.
 \tag{45}
\]
For \(t\ge1\), the operator norm after multiplication by \(\phi_\alpha(f)\) is bounded by its value at \(t=1\). For \(0<t\le1\), the integrand norm is bounded by \(C\nu_s(f)t^{R-r-1}\). Both integrals converge. Truncate away from zero, take the integrals in the graph of the closed field operator, and use closedness to pass to the limit. This also proves the required domain inclusion for \((1+H)^{-R}\). \(\square\)

**(O)** Estimate (43) is an arbitrary-vector operator estimate. Vacuum values do not suffice. It should be sought for spacetime-smeared fields, with a rigorously identified transfer or reconstruction expression; unsmeared time-zero dimension-four fields are not an incidental requirement. The usual Gaussian constant-field counterexample has excellent vacuum moments, \(H=0\), and unbounded field multiplication, demonstrating the distinction.

**(L)** Driessler–Summers, Definition 2.1 and Theorem 2.3, provide a pure-phase decomposition under generalized energy bounds or their alternative intrinsic-locality hypothesis. Clause (vi) transfers an established energy estimate to almost every component; the result extends to finitely many field components [8]. A countable dense test family and seminorm control give a common full-measure set. Thus the bound need not be reproved independently in each phase, but it must first be established.

### 8.2 A sufficient phase-transfer criterion

First fix the actual quantitative ultraviolet target. For pairwise separated reference tests, write \(f_{i,\rho}(x)=\rho^{-4}f_i((x-x_*)/\rho)\). For \(m=2,3\), an explicit completion statement must specify normalization factors \(\mathcal N_m(\rho,\mu)\) and predicted coefficients \(c_m\) in the current coupling convention, then prove a bound of the form
\[
 \Bigl|\mathcal N_m(\rho,\mu)S^c_{m,n}(f_{1,\rho},\ldots,f_{m,\rho})-c_m(f_1,\ldots,f_m)\Bigr|\le\epsilon_{\rm UV}(\rho)+\epsilon_{\rm cut}(a_n/\rho,\rho/T_n).
 \tag{46}
\]
The functions on the right must tend to zero in the stated limits with the required uniformity, and the specified third coefficient must be nonzero. Any coupling-dependent leading correction can instead be included explicitly on the left. The exact logarithmic normalization is determined by the chosen renormalized scalar, not guessed from its name. The continuum limit is taken first at fixed \(\rho\), with \(a_n/\rho\to0\) and \(T_n\to\infty\); only then is \(\rho\to0\). Such a statement, including its phase transfer, is still **(O)**.

Let \(A_\rho\) be a suitably renormalized, normalized ultraviolet product, with its domains and phase decomposition defined. Let \(c_\rho\) be its specified AF leading expression. If its conditional phase expectation is \(a_\rho(\xi)\), an estimate only of \(\int a_\rho\,d\nu\) cannot determine the individual phase coefficients.

**Proposition 8.2** (Central estimate transfers the coefficient, **(P)**). *Suppose for every central projection \(E\),*
\[
 |\omega(EA_\rho)-c_\rho\omega(E)|\le\epsilon(\rho)\omega(E).
 \tag{47}
\]
*Then \(|a_\rho(\xi)-c_\rho|\le\epsilon(\rho)\) for almost every \(\xi\).*

*Proof.* Central projections are indicator functions of measurable phase sets \(B\). Thus the integral of \(a_\rho-c_\rho\) over every \(B\) has magnitude at most \(\epsilon(\rho)\nu(B)\). For real values, a superlevel set contradicts this if the claimed bound fails. For complex values, apply the real argument to \(\operatorname{Re}(e^{-i\theta}(a_\rho-c_\rho))\) for a countable dense set of angles, then intersect the full-measure sets. \(\square\)

An operator estimate \(\|P_0(A_\rho-c_\rho I)P_0\|\le\epsilon(\rho)\), on the entire vacuum space, is one sufficient way to obtain (47), with decomposability and domains checked. Countable test configurations and scale parameters, together with quantitative continuity, produce a common phase for the required statements. For connected coefficients, the corresponding lower moments and cumulant subtractions must be controlled too; connected functions do not generally commute with mixing.

For translation-invariant scalar phases and zero-integral one-point tests, the phase means vanish, so a third connected function is the average of the component third connected functions. Its nonzero value forces at least one non-Gaussian observable component, but does not transfer a prescribed AF coefficient. A quadratic composite of a free field can itself have a nonzero third cumulant, so that cumulant alone is not the requested Yang–Mills identification.

**Additional phase check.** A symmetry of a mixture may permute its phases. If P1 requires full \(O(4)\) covariance in the selected phase, prove that its disconnected symmetries, including the appropriate parity action on pseudoscalars, are retained in a phase that also has the AF and energy conclusions. Generic pure-phase decomposition does not alone settle this discrete-symmetry question.

**Regularity in the selected phase.** If corrected OS growth is required of that phase, its transfer is another quantitative obligation. The cited decomposition theorem supplies Wightman properties and existing energy bounds, not by itself the same fixed-order factorial Euclidean estimate. A sufficient stronger hypothesis is
\[
 |\omega(EA_m(F))|\le B^{m+1}(m!)^p\nu_{qm}(F)\,\omega(E)
 \tag{48}
\]
for every central projection \(E\) and appropriately defined decomposable Euclidean product \(A_m(F)\). The central-projection argument, a countable dense test family, and continuity then transfer the bound phasewise. Alternatively, prove a separate quantitative deduction from the arbitrary-vector operator estimates. P1 only needs fixed constants within the selected phase, not necessarily uniform constants for every phase. This transfer is not assumed from the mixed hierarchy's vacuum bound.

## 9. Conditional assembly and completion criteria

**Theorem 9.1** (Refined conditional assembly, **(C)**). *Assume an admissible cofinal Wilson sequence and a correctly normalized source-free base. Suppose \(S_{m,n}\) are the full moments of the specified locally renormalized Wilson observables, modified only by a proved positivity-compatible prescription or by contact errors satisfying (34). Require compatibility in source degree and reflection, permutation symmetry, and one orientation-reversing covariance. Suppose the connected or full kernels satisfy the hypotheses of Theorem 5.2, or the full hierarchy directly satisfies (28), and the translation and six angular defects vanish. Then a subsequence yields a continuum full hierarchy satisfying corrected OS regularity, Euclidean covariance, reflection positivity, and symmetry, hence its OS reconstruction without a clustering premise.*

*If the prescribed AF two-point and nonzero connected three-point laws hold with their quantitative remainders, the energy input (43) holds on the common reconstructed domain, the decomposition hypotheses are met, and a selected phase retains those ultraviolet laws, the required covariance, and corrected OS regularity with fixed linear order and factorial exponent across its complete hierarchy, then that phase meets the reduced P1 target.*

*Proof.* Theorem 5.2 gives the common OS bound. The countable compactness and finite positivity-form argument give the continuum hierarchy. Proposition 7.1 supplies rotations from the six defects, and the checked reconstruction theorem supplies the relativistic fields. Proposition 8.1 gives the specified polynomial energy control, and the checked decomposition theorem transfers it to phases. The ultraviolet, phase-covariance, and phase-regularity hypotheses supply the remaining identification and selection conclusions. No omitted hypothesis is established by the assembly step. \(\square\)

| Item | Required theorem | Criterion |
|---|---|---|
| B | Base and trajectory identification | Exact action/trace/plaquette dictionary, admitted geometry and group, positive source-free histories, and the verified trajectory for the actual effective coefficient. N2-F may be a working premise; it must be inspectable for a final independent claim. |
| S2 | Full-law scalar two-point estimate | Prove the actual-history shell and terminal bounds in Section 3, or an explicit summable replacement. Include background chains, nonlinear interactions, and the large-field R operation. A Gaussian or fixed-scale proof does not close this item. |
| M | All-order marked induction for the 21 components | Establish the joint kernel bound with fixed \(A,p,\sigma,b\), uniform in cutoff and chosen expanding volume, while retaining every generated response and remainder vertex. No \(K\)-dependent constants or order-by-order unspecified growth remain. |
| L | Locality and positive-time compatibility | Fix running mixing at \(\mu\), collision-subcluster subtractions and their order bounds, and prove the reflection-compatible lattice moment or splitting construction. Control shrinking-stencil errors quantitatively. |
| R | Rotation restoration | Establish the six tensor angular defects uniformly before extraction. Identify and bound renormalized lattice artifacts and their lower-dimensional mixings. |
| U | Yang–Mills short-distance identification | Specify and prove the two-point AF law and one nonzero connected three-point coefficient with a remainder uniform in cutoff and volume, and a valid common-phase transfer argument. |
| E | Operator estimates and phase selection | Prove an arbitrary-vector estimate such as (43), check the common domain and decomposition hypotheses, and transfer corrected OS growth and every required discrete symmetry to the chosen phase. |
| A | Final assembly | Apply the proved bridges and primary reconstruction/decomposition theorems only after all hypotheses above are discharged. Check one common field normalization and one cofinal subsequence throughout. |

The next main calculation is S2. Its success would be a genuine interacting observable advance. The jump from S2 to M is substantial: two marks do not control every finite jet, its factorial growth, or tensor mixing. R and E can be investigated in parallel because neither follows from vacuum moment estimates. U must be formulated early enough that the normalization and phase estimates required for it are built into M and E.

## 10. Interface statement

**Assumed** for the proposed construction: the J0 source-free base and trajectory, the indicated physical covariance hypotheses when discussing the Gaussian diagnostic, and each explicitly displayed interacting estimate when deriving its consequence.

**Proved reductions:** the finite jet partition rule; covariance telescoping; geometric shell summation; the constant-tensor diagnostic; the Gaussian Wick hierarchy estimate under its covariance hypothesis; connected-to-full factorial control; joint-kernel-to-OS continuity; angular-generator reduction; heat-semigroup-to-energy control; and central-projection-to-phase coefficient transfer.

**Not proved here:** a cutoff-uniform renormalized scalar two-point estimate for the full Wilson measure, the all-order finite-tensor marked theorem, rotation restoration for the interacting limit, the specified AF remainder estimates, or an interacting arbitrary-state energy estimate. Accordingly, four-dimensional Yang–Mills existence is not proved in this note.

The normalized-trace and geometry checks use the published primary papers listed below. The proofs in this note are mathematical deductions from their displayed hypotheses.

## References

1. T. Balaban, Large field renormalization. I. The basic step of the R operation, *Commun. Math. Phys.* 122 (1989), 175–202. Relevant formulas: (0.3)–(0.4), p.176; localized (1.100), (1.102), p.201.
2. T. Balaban, Large field renormalization. II. Localization, exponentiation, and bounds for the R operation, *Commun. Math. Phys.* 122 (1989), 355–392. Theorem 1 and (0.1), pp.355–356.
3. T. Balaban, Convergent renormalization expansions for lattice gauge theories, *Commun. Math. Phys.* 119 (1988), 243–285. Section 2, especially pp.262–264.
4. T. Balaban, Propagators for lattice gauge theories in a background field, *Commun. Math. Phys.* 99 (1985), 389–434. Regular-background kernel results are not identified with all-history physical marked bounds in this note.
5. T. Balaban, Renormalization group approach to lattice gauge field theories. I. Generation of effective actions in a small field approximation and a coupling constant renormalization in four dimensions, *Commun. Math. Phys.* 109 (1987), 249–301. DOI: 10.1007/BF01215223. Geometry p.251; normalized trace (0.2), p.252; scale volumes and theorem statements pp.258–260.
6. T. Balaban, Renormalization group approach to lattice gauge field theories. II. Cluster expansions, *Commun. Math. Phys.* 116 (1988), 1–22. DOI: 10.1007/BF01239022.
7. K. Osterwalder and R. Schrader, Axioms for Euclidean Green's functions II, *Commun. Math. Phys.* 42 (1975), 281–305. Remarks 5–6, p.283; flat Schwartz space p.284; E0′ and main reconstruction theorem pp.287–288.
8. W. Driessler and S. J. Summers, On the decomposition of relativistic quantum field theories into pure phases, *Helv. Phys. Acta* 59 (1986), 331–348. Definition 2.1, p.334; Theorem 2.3, pp.335–336, especially clause (vi) and Remark 2.
