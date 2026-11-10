# Composite operators, contacts and reflected susceptibility

On the reference Wilson tori ordinary susceptibility reduces to a single uniformly weighted temporal source. Section 4.136 proves the required centered real pressure estimate on the specified early native convergence, selector and support margins. With the finite smooth additive action-pressure clauses identified in §§4.113 and 4.117, it yields extensive ordinary susceptibility for every weighting. Those complex clauses and the research imports are distinguished from the real estimate. The paper also gives the contact algebra, constrained integrations, an explicit magnetic inverse spectral formula, and a positive local reflection test at mesoscopic separation. Full interacting operator mixing, all-history cumulants and fixed-physical-scale nondegeneracy remain open.

## 1. Target and interfaces assumed

**Conventions.** $G=SU(N)$, $N\ge2$; $S=\sum_p(N-\operatorname{Re}\operatorname{Tr}U_p)$, $\beta_a=2N/g_0(a)^2$, and $d\mu_a=Z_a^{-1}e^{-\beta_aS}d\lambda$. The fixed torus has side $t^*$; $a=L^{-K}\ell_0$, $L\ge3$ odd, $n=t^*/a$, and $g_k\le\bar g$. Constants may depend on $N,L,M,D,t^*,\ell_0,\bar g$, a fixed norm convention, and displayed additional hypotheses, but never on $a,K$, history depth, or test functions unless stated. No mass gap is assumed. No compact Wilson law is replaced by a Gaussian reference law.

**Imports.** Only the program interfaces I-0c and I-1, exactly as stated, are imported. I-0c supplies the complete intermediate-scale small/large-field representation and the stated flow remainder. I-1 supplies the marked $P_6\mathcal L^{(2)}$ contraction through all histories, uniform first and second source-derivative bounds in its stated source norms, and analyticity of the source pressure on a fixed polydisc. It does not specify a locally bounded family of analytic pressures after all required contact subtractions, a lattice-mark norm uniform over every lattice momentum, or a reflected lower bound. None of those is silently imported. T1 denotes [Transport of insertions on a reference torus](insertion_transport.md) and T2 denotes [Large-field admission with insertions](large_field_admission.md).

**Labels.** P = proved here, including elementary finite-dimensional identities; C(H) = deduction proved under the displayed additional hypothesis H, whose validity for Wilson theory remains open; L = a checked primary-source theorem; O = not proved. A P lemma with arbitrary input matrices does not establish that the matrices produced by the Wilson RG meet a displayed estimate.

**Normalization.** With the density of T1 ([Transport of insertions on a reference torus](insertion_transport.md)) $\mathcal O_a=a^{-4}\sum_{\mu<\nu}(1-\operatorname{Re}\operatorname{Tr}U_{\mu\nu}/N)$, the conventions above give $\beta_aS=2N^2g_0^{-2}\sum_xa^4\mathcal O_a(x)$. Thus a constant source $J\sum a^4\mathcal O_a$ shifts $g_0^{-2}$ by $-J/(2N^2)$. This agrees with T1 (2.2'). All formulas here retain the convention above.

## 2. Definitions and conventions

### 2.1 A compatible finite classical type space (P)

Introduce formal adjoint-valued letters $Y_{r,\boldsymbol\mu;\nu\rho}$, $0\le r\le D-2$, with $\nu<\rho$, $\boldsymbol\mu\in\{1,2,3,4\}^r$, weight $r+2$, representing ordered covariant derivatives of curvature. Their color components transform by the adjoint representation. There are at most
\[
J_D=6(N^2-1)\sum_{r=0}^{D-2}4^r
\]
scalar generators. Let $V_D$ be all polynomials of weighted degree at most D. It has dimension at most $\binom{J_D+D}{D}$, a deliberately loose explicit bound. Projection by Haar averaging,
\[
(\mathscr RP)(Y)=\int_G P(\operatorname{Ad}_gY)\,dg,
\]
is an idempotent onto the gauge-invariant subspace. Choose bases degree by degree, once for all D, using linear independence of projected monomials. Identity and all derivative descendants are retained. Linear algebra then gives nested finite bases. Complex tensors can be replaced by real and imaginary parts to obtain Hermitian types.

Universal Bianchi and derivative-commutator identities may subsequently be imposed as homogeneous algebraic relations in the classical jet space. They do not authorize an interacting equations-of-motion quotient. To avoid unproved quantum identities, this paper retains the redundant ordered-derivative presentation until a contact identity has been established. Thus this construction proves a finite spanning space and compatible independent formal types; independence of their quantum realizations is O.

For an explicit compact lattice representative set
\[
C_N(U)=\tfrac12(U-U^{-1})-\tfrac1{2N}\operatorname{Tr}(U-U^{-1})I,
\quad \delta_\mu^UX(x)=\operatorname{Ad}_{U_\mu(x)}X(x+a\hat\mu)-X(x).
\]
Replace a letter by $a^{-r-2}(\delta^U_{\mu_1}\cdots\delta^U_{\mu_r}C_N(U_{\nu\rho}))(x)$, with all factors based at x. Adjoint covariance makes every invariant polynomial exactly gauge invariant. At fixed a it is a bounded smooth function on the compact link space, with a stencil depending only on D. Taylor expansion on a fixed smooth classical connection gives the intended classical polynomial. This classical statement gives no quantum uniform estimate. Smearing is $O^{\rm bare}_{\alpha,a}(f)=a^4\sum_x f(x)P_{\alpha,a}(x)$.

### 2.2 Contacts are multilinear data

The scalar formulas below define the identity-contact sector. The complete operator-valued collision prescription uses the nonlinear local source map of §4.17; the scalar formula must not be mistaken for a complete all-composite construction.

For a vector source J let
\[
W_a[J]=\log\mathbb E_{\mu_a}\exp\!\left(\sum_\alpha O^{\rm bare}_{\alpha,a}(J_\alpha)\right),\qquad
W_a^{\rm ren}[J]=W_a[Z_a^TJ]-L_a[J].
\]
The branch of the logarithm at J=0 is used where it exists. Require $L_a[0]=0$. Its source derivatives $L_a^{(m)}$ are joint contact counterterms. A strictly local contact has distribution kernel supported on the total diagonal, with a finite number of derivatives; a finite-range kernel is not, by that fact alone, a strictly local contact.

Define renormalized connected distributions as $\kappa^{\rm ren}_{a,m}=D^mW_a^{\rm ren}[0]$. Unless positivity is separately established, these need not be ordinary cumulants of random variables. Only the first derivative is an individual operator plus an identity shift. In particular subtracting $L_a^{(2)}$ from a covariance does not alter the ordinary variance of the bare observable appearing in I-3(iv).

### 2.3 Ordinary and reflected forms

Put $F_{b,i}=(X_b^AS_i)_A$, $F_b=\sum_iF_{b,i}$, $D_b=\sum_i|F_{b,i}|^2$, $\ell_b=\sum_A(X_b^A)^2S$. Then
\[
r_b=\beta D_b-\ell_b/3,\quad
h_b=\beta(D_b-|F_b|^2/3)=\tfrac\beta3\sum_{i<j}|F_{b,i}-F_{b,j}|^2,\quad
t_b=h_b-r_b.
\]
For marks f write $r_f=\sum_bf_br_b$, $M_f=\sum_b|f_b|^2$. The physical source is exactly $r_H(f)=c_\beta^{-1}a^{-2}r_f$; a variance bound acquires $c_\beta^{-2}a^{-4}$. The additional $a^4$ rescaling needed for the program's non-tight bare H must remain separate from this conversion.

For positive-time observables $A_i$, define the centered reflected Gram matrix
\[
G^\theta_{ij}=\mathbb E[\overline{A_i(\theta U)}A_j(U)]-\overline{\mathbb EA_i}\,\mathbb EA_j.
\]
It is not the ordinary covariance matrix. Positive-time supports are separated from both reflection planes on a periodic torus.

## 3. Main theorems

### Theorem 3.1. Exact scalar-contact and compatibility algebra (P)

For any cutoff-dependent triangular $Z_a$ and local functional $L_a$, renormalized connected distributions are exactly
\[
\kappa^{\rm ren}_{a,m}(J_1,\ldots,J_m)
=\kappa_{a,m}(Z_a^TJ_1,\ldots,Z_a^TJ_m)-L_a^{(m)}[0](J_1,\ldots,J_m).
\]
For $m\ge2$, adding an identity row to an individual observable does not change its ordinary cumulant. A strictly local $L_a^{(m)}$ vanishes when the m supports have empty common intersection. If $W_{a,D+1}^{\rm ren}[J,0]=W_{a,D}^{\rm ren}[J]$, compatibility of every cumulant follows by differentiation. Conversely, analytic germs with all derivatives agreeing and value zero at the origin agree on their common connected analytic domain.

For reflection positivity, suppose bare $\mathcal Z[J]=e^{W[J]}$ is reflection positive and
\[
L[\theta\overline{J_i}+J_j]=\overline{L[J_i]}+L[J_j]
\tag{SPLIT}
\]
for all positive-half sources under consideration, and the mixing matrix $Z_a$ commutes with reflection on the component/tensor indices. Then $e^{-L[J]}\mathcal Z[J]$ is reflection positive on those sources, including its polynomial derivatives. For disjoint reflected supports, the centered two-point form is unchanged by a strictly local quadratic contact, after the linear change of operator basis. Finite range bounded by a positive physical length does not imply SPLIT.

### Theorem 3.2. Quantitative triangular normalization and age summation (P algebra; C for its RG application)

Let $A_{k,D}$ be finite block lower-triangular mixing matrices in a fixed degree-ordered basis, with invertible diagonal blocks. Their product $B_{K,D}=A_{K-1,D}\cdots A_{0,D}$ is invertible and lower triangular. $Z_{a,D}=B_{K,D}^{-1}$ normalizes the retained coefficients exactly. If every $A_{k,D}$ is the leading principal truncation of $A_{k,D+1}$, the inverse normalizations are compatible as D increases. No estimate for $Z_{a,D}$ follows from invertibility alone.

For a diagonal block $A_k=I+E_k$ with $\|E_k\|\le c_Dg_k^2\le1/2$,
\[
\|A_{K-1}\cdots A_0\|\le e^{c_D\sum g_k^2},\qquad
\|(A_{K-1}\cdots A_0)^{-1}\|\le e^{2c_D\sum g_k^2}.
\]
When $b=b_0\log L>0$ and $C\bar g^2\le b/2$, I-0c gives $g_j^{-2}\ge g_K^{-2}+(b/2)(K-j)$, hence
\[
\sum_{j=0}^{K-1}g_j^2\le\frac2b\log\!\left(1+\frac{bK}{2g_K^{-2}}\right).
\]
These products can grow as a power of $1+K$, and are not uniformly bounded just because the exponent is logarithmic.

For every fixed q, s>0, no smallness condition proportional to q is needed to sum the I-1 age factor. Put $h=\bar g^{-2}$, $b_+=b+C\bar g^2$, $c=b_+/h$, $r=q/2$, $d=\lceil r\rceil$, and $\rho=L^{-s}$. Then
\[
\sum_{j=0}^{k}L^{-s(k-j)}(g_k/g_j)^q
\le A_{q,s}:=\sum_{u=0}^{d}\binom du c^u\frac{u!}{(1-\rho)^{u+1}}<\infty.
\tag{AGE}
\]
Thus a uniform sum over birth histories of graded input norms, if established, closes the age summation for each finite dimension. AGE does not control the number or total norm of histories and does not recover components removed by $P_6$.

### Theorem 3.3. Uniform analytic functional gives all cumulants (C(AN-D))

Let $\mathcal X_D=\bigoplus_{\dim\alpha\le D}C^{s_D}(T^*)$, normed by the sum of component norms. Suppose the renormalized $W_{a,D}^{\rm ren}$ is holomorphic on $\|J\|_{\mathcal X_D}<R_D$, vanishes at zero, and satisfies $|W_{a,D}^{\rm ren}[J]|\le A_D$ there, uniformly in a. Then for every m and every $J_i\in\mathcal X_D$,
\[
|D^mW_{a,D}^{\rm ren}[0](J_1,\ldots,J_m)|
\le A_D(m/R_D)^m\prod_i\|J_i\|
\le A_D(e/R_D)^m m!\prod_i\|J_i\|.
\tag{CUM}
\]
Thus the desired cumulant growth has p=1 with $C_D=(e/R_D)\max(1,A_D)$. These constants are independent of K and source order m. Mere analyticity for each a, and bounds for its first two derivatives, do not supply AN-D.

### Theorem 3.4. Fixed-volume susceptibility from plane-wave zero-freeness alone (C(ZF))

Fix $\sigma>0$ and restrict to $n=t^*/a\ge3$, $\beta\ge1$, $\log\beta\le\sigma n$. There are constants $A_\sigma,C_{W,\sigma}$ depending only on $N,\tau,\sigma$ and the fixed source stencil conventions such that the following holds. Put $R_0=1/(32\tau)$ and fix $0<R\le R_0$. Assume only the additional source assertion that, for every lattice momentum p and unit $v\in\mathbb C^4$, the partition function of each real mark
\[
f_{p,v}^{\rm re}(x,\nu)=\operatorname{Re}(v_\nu e^{ip\cdot x}),\qquad
f_{p,v}^{\rm im}(x,\nu)=\operatorname{Im}(v_\nu e^{ip\cdot x})
\]
has no zero on $|z|<R$:
\[
\mathbb E_{\mu_a}e^{zh_f}\ne0.
\tag{ZF}
\]
Then, for every real mark f,
\[
\operatorname{Var}_{\mu_a}(r_f)
\le(8A_\sigma/R^2+C_{W,\sigma})M_f.
\tag{SUS}
\]
The physical bound is $c_\beta^{-2}a^{-4}(8A_\sigma/R^2+C_{W,\sigma})M_f$.

No separate moment hypothesis or complex logarithm bound is imported. Section 4.11 proves directly from the full Wilson law that
\[
\log\mathbb E_{\mu_a}\exp\left(R_0\sum_bh_b\right)\le A_\sigma n^4
\tag{M}
\]
and that the ordinary r/h covariance matrices differ by an operator of norm at most $C_{W,\sigma}$. The latter uses the exact complete H contact and only a first plaquette-action moment, also proved there. Harmonic Fourier coefficients of $\log\mathbb E e^{zh_f}$ then give SUS. ZF is required only on the reference-torus trajectory, not uniformly over arbitrarily large physical volumes.

### Theorem 3.5. Exact reflected boundary representation (P; lower bound C(BND))

For an even periodic lattice with site reflection through time 0 and time $n/2$, let B consist of spatial links on both reflection planes. Let $A_i$ depend only on links strictly in the positive half, possibly with the boundary links as parameters. With
\[
a_i(B)=\mathbb E[A_i\mid B],\qquad \nu_a=\operatorname{Law}_{\mu_a}(B),
\]
the exact Wilson law satisfies
\[
G^\theta_{ij}=\int\overline{(a_i-\nu_aa_i)}(a_j-\nu_aa_j)\,d\nu_a.
\tag{BOUNDARY}
\]
Thus physical reflected nondegeneracy is precisely noncollapse of the boundary conditional means, not the ordinary variances of $A_i$.

Here is a quantitative sufficient criterion for a fixed r-dimensional family. Suppose there is a boundary readout $y_a(B)$ with law density at least c>0 relative to a fixed probability measure $\nu_*$, and fixed functions $\phi_1,\ldots,\phi_r$ with covariance $\operatorname{Cov}_{\nu_*}\phi\ge\lambda_*I$. If
\[
\sup_{|v|=1}\left\|\sum_i v_i\big(a_i-\phi_i(y_a)\big)\right\|_{L^2(\nu_a)}\le\varepsilon,
\tag{BND}
\]
then $G^\theta\ge(\sqrt{c\lambda_*}-\varepsilon)_+^2 I$. In particular $\varepsilon<\sqrt{c\lambda_*}$ supplies the required positive lower bound. Neither the boundary minorization nor BND is supplied by the allowed interfaces. The formula makes the missing physical information explicit and uses the actual Wilson conditional law.

### Theorem 3.6. Local Taylor extraction with a uniformly summable remainder (P; C for the RG kernel estimate)

This theorem gives an actual subtraction procedure, rather than removing entire finite-range kernels. Let $\ell_k=L^ka$, $0\le k\le K$, and let a bilinear contribution have the form
\[
B_k(f,g)=\int_{T^*}dx\int K_k(x,du) f(x)g(x+u),
\]
where $K_k(x,\cdot)$ is a complex finite measure, supported on a chosen local lift with $|u|\le R\ell_k$, and
\[
\sup_x\|K_k(x,\cdot)\|_{\rm TV}\le C_0\ell_k^{-4}.
\tag{KT}
\]
The same conclusion holds with $dx$ replaced by normalized lattice counting measure $a^4\sum_x$. Set
\[
T_kg(x,u)=\sum_{|\alpha|\le4}\frac{u^\alpha}{\alpha!}\partial^\alpha g(x),\quad
L_k(f,g)=\sum_{|\alpha|\le4}\int dx\,m_{k,\alpha}(x)f(x)\partial^\alpha g(x),
\quad m_{k,\alpha}=\int\frac{u^\alpha}{\alpha!}K_k(x,du).
\]
Then $L_k$ is strictly diagonal and
\[
|B_k-L_k|(f,g)\le\frac{C_0R^5}{5!}\ell_k\operatorname{Vol}(T^*)\|f\|_\infty\|D^5g\|_{\rm op,\infty}.
\tag{TR}
\]
Here the derivative norm is the supremum norm of the fifth multilinear differential, so the displayed constant is literal. Hence $\sum_{k=0}^K(B_k-L_k)$ has a uniform $C^0\times C^5$ bound with coefficient at most
\[
\frac{C_0R^5}{5!}\frac{L\ell_0}{L-1}\operatorname{Vol}(T^*).
\]
The contact coefficient of derivative order q satisfies $|m_{k,\alpha}|\le C_0R^q\ell_k^{q-4}/\alpha!$. Its scale sum has leading sizes $a^{q-4}$ for q<4 and K for q=4. When the kernel is even in u, odd moments vanish, leaving the advertised $a^{-4},a^{-2},\log(\ell_0/a)$ divergences. Symmetrization in f,g and averaging under the finite lattice reflection group preserve the bounds up to the same fixed convention constants and give a reflection-covariant diagonal subtraction.

For scales with $R\ell_k$ too large to choose a local torus lift, retain the entire kernel instead. There are only $O(1+\log_L(R\ell_0/t^*))$ such terminal scales, independent of a, and their total bilinear norm is finite independent of a. This avoids imposing a fictitious unique displacement across a periodic cut.

**Extension to a fixed source order m (P).** Suppose a connected m-source scale kernel, anchored at x, has total variation at most $C_{D,m}\ell_k^{-w}$, all m−1 relative coordinates have norm at most $R\ell_k$, and $w=\sum_i d_i-4(m-1)\ge0$. Taylor-expand the function $\prod_{i=2}^m f_i(x+u_i)$ in all relative variables through degree $q=\lfloor w\rfloor$. The remainder has scale factor $\ell_k^{q+1-w}$, and is summable since q+1−w>0. If w<0 no subtraction is needed. This is a fixed-m construction with explicit dependence on the kernel constant and the Taylor derivative norm. It does not supply an all-m bound on $C_{D,m}$, nor a source norm whose derivative order is independent of m.

In particular for all $d_i=4$, w=4 at every source order. A dimension-four source has engineering dimension zero: power counting does not truncate a local counterterm functional at source degree four. Every $\int J(x)^m dx$ can have a coefficient of engineering dimension four. This distinguishes field Taylor degree from source degree.

### Theorem 3.7. Positive transfer reduces susceptibility to one periodic mark (P reduction)

On the commensurate tori and fixed strides of §§4.29–4.32, let $f^{\rm comb}$ mark one bond orientation once per rectangular cell of $m_\Pi$ lattice sites. Then
\[
\sup_{f\ne0}\frac{\operatorname{Var}(r_f)}{M_f}
\le 4m_\Pi\frac{\operatorname{Var}(r_{f^{\rm comb}})}
{n^4/m_\Pi}.
\]
Consequently the full variance estimate is equivalent to its restriction to this one nonnegative mark. A fixed complex zero-free disc for the corresponding frustration source suffices by the proved real pressure and Ward estimates. On an even torus the oriented $1\times2\times2\times2$ rectangle gives $m_\Pi=8$ and prefactor 32. The same proof, under the marked-moment tiling hypothesis of §4.22, gives an unconditional bound for Fourier marks separated from all coordinate momentum planes. Every positive innovation and retained-mean contribution through two actual constraints inherits the latter bound. Proofs are in §§4.26–4.32.

### Theorem 3.8. Two real constrained innovations on the regular nonflat clean body (P/L)

For the original two independent clean selectors on the admitted small physical terminal chart, the averaged conditional covariance and the variance of the first retained mean together obey NONFLAT-TWO-INNOVATIONS for every real mark. The constants depend on the fixed two-step geometry and the strict native margins, uniformly in volume and ultraviolet cutoff. The proof establishes positivity of the exact joint constrained Hessian and uses the original fine plaquette first moment in the undivided average. The nonlinear critical source obeys NONLINEAR-CRITICAL-DISC. On the native first-fiber domain of T1 Proposition 7.67, the integrated first nonidentity row obeys FIRST-NONIDENTITY-COMB with its winding remainder. Proofs and the precise remaining sectors are in §§4.39–4.43.

### Theorem 3.9. The bare physical source has nearby complex zeros (P)

For the program's unrescaled physical \(H\) source at a constant smooth mark, the nearest complex zero has modulus at most \(Ca^2\) on the weak reference trajectory. This holds also for \(r_H\) and under arbitrary real linear mixing with the six standard plaquette orientation energies and scalar entire contact factors. A fixed source disc would require the multiplicative coefficient of the physical \(H\) term to be \(O(a^2)\). This obstruction concerns bare-source pressure analyticity. The unamplified eight-site mark has a different normalization. See PHYSICAL-H-ZERO and PLAQUETTE-MIXED-ZERO in §4.56.

### Theorem 3.10. Sharp full-Wilson innovation and conditional-jet obstruction (P)

For the eight-site temporal mark, exact single-link disintegration gives SINGLE-LINK-TOWER. Under FIRST and the marked-moment hypothesis of §4.22, the per-link ordinary innovation tends to \(8\tau^2\dim SU(N)\), and the corresponding frustration innovation tends to zero. Their retained exterior field is identical and is given by SINGLE-LINK-MEAN. At compact exteriors the conditional zero-free radius can be \(O(1/\beta)\) and the conditional variance of an unamplified link can be of order \(\beta^2\). For \(SU(2)\), the integrated absolute conditional source jets have exact factorial exponent two. For every group in the question, the integral's mean is the difference of a fixed linear combination of six-link Wilson energies and the conditional mean of an explicit nonnegative quartic plaquette polynomial. Proofs are in §§4.57–4.60.

### Theorem 3.11. Full-law box innovations, retained boundary response and Fourier concentration (P)

On the marked-moment reference tori, for comb-supported real marks and \(4\)-dimensional tree-fixed Wilson boxes of side at most \(s\le\beta^{1/30}\), the averaged ordinary conditional variance after retaining the tangential grid-face links is at most \(C_N M_f\). For comparable nested boxes of sides \(s\mid S\le\beta^{1/200}\) and a unit comb, the next retained-mean innovation is at most \(C_N n^4/s\). On these smaller growing scales the field-dependent conditional mean has surface-order absolute norm on each box. Its response at distance \(d\) from the boundary has \(L^2\) bound \(C_N/(1+d)^2\) plus the explicit small local error in FACE-DEPTH-ROW. The retained positive operator consequently has trace \(O(n^4/s)\), and a common susceptibility threshold holds outside a vanishing fraction of Fourier bins. The possibly exceptional zero mode, equivalently the final retained face covariance, is still open. Proofs and growth limits are in §§4.68–4.72.

### Theorem 3.12. Signed zero-mode sum and real pressure (P in the stated ranges)

For the actual unit comb, the signed covariance sum through lattice distance \(S_\beta\asymp\beta^{1/35}(\log\beta)^{-6/35}\) converges to the finite Gaussian constant (GAUSSIAN-COMB-CONSTANT). Each covariance there obeys \(C(1+d)^{-14/3}\). The signed sum at larger separations has nonnegative liminf and has no proved uniform upper bound on the specified trajectory. When \(n\le c S_\beta\) the estimate covers all separations and proves the full ordinary susceptibility bound on that finite-size regime.

The actual real pressures of both unamplified combs converge on a fixed interval to their Gaussian determinant pressures. Their slopes have error at most \(C S_\beta^{-3}\). A large finite-volume variance at exactly zero would require zeros of the full comb partition function at radii \(o(S_\beta^{-3})\). More precisely (SIGNED-COMB-ZEROS) computes the variance per site up to bounded error by the signed inverse-square sum of the true zeros inside a disc of that order. The unconditional bound currently obtained is \(C(1+V/S_\beta^6)\) per site. Severe staple cancellations and sufficiently large energetic components make a vanishing variance-scale contribution under the thresholds of §4.76.

With \(\mathcal E\) all links except the selected temporal links, the ordinary and frustration combs have the same retained mean. For literal frustration \(Y^h\), the centered heatbath noise has \(\log\mathbb E\exp[t(Y^h-\mathbb E[Y^h\mid\mathcal E])]\le C Vt^2/\beta^2\) on a fixed real interval. Removing it changes the full variance by \((\gamma_N+o(1))|\mathcal C|/\beta^2\) with explicit \(\gamma_N>0\). Singular one-link conditional partition zeros have exponentially small annealed inverse-square mass. The exact exterior action, including degenerate staples, is (EXACT-DECIMATED-ACTION); its determinant prefactor costs \(O(V/\beta)\) in the log normalization after its vacuum value is extracted. Extracting its one-loop star coupling leaves \(O(V/\beta^2)\). On typical rough fields a universal face-projection contraction fails, whereas the two-shift estimate (SHIFTED-ROUGH-CONTRACTION) suppresses the actual comb variance above a common outer face grid. Sections 4.73–4.96 prove these statements.

### Theorem 3.13. Physical-scale exterior sectors and the remaining singlet (P; additive action row under I-1)

On the required large fine torus, the entire fine one-skeleton of a macroscopic grid retains \(o(V)\) zero-mode variance by (COMPLETE-ONE-SKELETON). The estimate uses uniform one-link mixing in every nontrivial group representation, and extends to dense arrays of long path products with the spectator restrictions of §§4.98–4.102. Conditioning all temporal Polyakov products to identity changes the real full comb variance by \(o(V)\). The resulting axial transfer is precisely (AXIAL-PRODUCT-TRANSFER). Its kinetic perturbation obeys the uniform complex form bound (GLOBAL-KINETIC-FORM), with the separate exponentially small magnetic vacuum scale (MAGNETIC-VACUUM-SCALE).

For the actual remaining axial magnetic histories, a full temporal star integration has extensive variance and the normalized exterior mean \(M_{\rm sp}\) has canonical Dirichlet energy at most \(CV\), with uniformly summable time-response rows in (SPATIAL-EXTERIOR-SCORE). A true slowly varying magnetic singlet excludes a uniform Poincaré bound for arbitrary scalars on that same exterior. This spectral route leaves the unconditioned variance open by itself. The separate positive early-pressure theorem in §4.136 bounds it under the listed hypotheses, since it is one term in the true variance decomposition.

Separately, full Wilson random-walk bridges give all finite regulated colored resolvent trace moments in (COLORED-RESOLVENT-MOMENTS), a negligible terminal colored force component in (TERMINAL-COLORED-LOWPASS), and an extensive real Wilson-divergence component in (HODGE-WARD-SCORE). These bounds concern the adjoint connection and a specific source component. They do not control the remaining correlated singlet traces in (SINGLET-HODGE-RESIDUAL). Under I-1 for the smooth six-component additive action family, all microscopic linear plaquette-energy marks, including the Casimir remainder, satisfy (ADDITIVE-PLAQUETTE-SUS). Equations (SIGNED-HODGE-COVARIANCE) and (TOTAL-FORCE-QUADRATIC-SUS) give a full signed contact and complete deterministic total-force quadratic estimates. Section 4.117 controls the actual quartic normal diagonal for all fine marks and the full quartic correction at its uniform component under the specified finite smooth family. Section 4.119 even allows arbitrary exterior-adapted off-diagonal total-force kernels on the original comb. Sections 4.98–4.120 prove these statements and identify the remaining signed sector.

### Theorem 3.14. Fine-uniform susceptibility and the complete magnetic spectral reduction (P under the stated smooth-source clauses)

On the reference tori, (FINE-UNIFORM-WARD-REDUCTION) bounds the structure factors at every fine momentum by the single ordinary fine-uniform temporal frustration structure factor, using only the six oriented additive plaquette sources for the Ward Casimir. Under the precise additional smooth finite collection of additive loop realizations of §4.117, (SUBLINEAR-COMB-SUS) gives \(\operatorname{Var}_\mu(r_f)\le C[1+\beta^{4/7}(\log\beta)^{24}]\sum|f_b|^2\) on the tori of (COLUMN-BOX-SCALE). The sharper balanced-box Ward estimate (CUBIC-CORRECTED-SUS) is used here. A disc of radius \(c s_{**}^{-3}\) for the fine-uniform unamplified source would give the requested constant bound. The remaining variance also has the exact positive inverse formula (MAGNETIC-EXTERIOR-SPECTRAL), the genuine spatial Ward split (SPATIAL-GAUGE-WARD-SPLIT), and the reduced positive density (MAGNETIC-QUOTIENT-LAW). These formulas include the constant component and all compact histories. See §§4.121–4.137.

### Theorem 3.15. Early positive pressure and the ordinary susceptibility implication (P/L on the specified native margins; C under the smooth pressure clauses)

On the early-prefix family of §4.136 the true fine-uniform centered additive real log satisfies (EARLY-FINE-UNIFORM-REAL). The independent canonical cutoff is the physical convention enforced by the original squared large-field reserve; the homogeneous comparison includes its field-dependent normalization. The normalized source is tested on protected real coordinates and its complement is integrated with the original occupied-volume bank. If I-1's fixed pressure polydisc includes precisely the short-loop/tensor-product smooth additive realizations of §4.117, then \(\operatorname{Var}_\mu Y_0\le CV\). With the six oriented smooth plaquette clauses of §4.113 this gives \(\operatorname{Var}_\mu(r_f)\le C\sum |f_b|^2\), including the constant mode on the full compact reference torus. The ordinary physical source acquires \(c_\beta^{-2}a^{-4}\). For the spatial exterior this also bounds the complete dyadic positive sum in (MAGNETIC-EXTERIOR-SPECTRAL), since its variance is a contribution to the true comb variance. This theorem establishes an implication on the stated weak reference family and these native proof margins. It does not verify the unrestricted composite-source polydisc or the remaining parts of I-3.

### Theorem 3.16. The exact Ward contact in the ordinary and reflected forms (P)

On the full fine Wilson law under (FIRST), the additionally rescaled total-force Ward component converges jointly to Gaussian white noise with the explicit covariance (WARD-WHITE-NOISE), and its separated reflected form vanishes identically at each cutoff. Its contact cross-form with frustration is explicit, and (ORDINARY-H-WARD-FLOOR) is a strictly positive ordinary lower bound for every smooth nonzero orientation profile. Section 4.139 proves these statements without a source analyticity hypothesis. The norm of the independent residual in separated reflection remains open.

### Theorem 3.17. Physical stopped windows and true-plane probes (P/L for the stated bounds; O for the interacting overlap)

A fixed physical intermediate stop has two full retained Haar neighborhoods of uniformly positive actual mass and separated regular minimizing-field action values, by (FIXED-CYLINDER-MASS). On the genuine microscopic reflection plane the complete fixed straight-graph projection of any polynomially sized separated action test vanishes by (STRAIGHT-BOUNDARY-PROJECTION). Raw spatial adjoint heat smoothing at fixed positive physical time also vanishes by (RAW-PLANE-HEAT). Section 4.143 supplies a bounded nonlinear spatial test in that same plane algebra and computes a strictly positive free overlap with the fixed positive-time action smearing. Sections 4.144–4.145 compute its true normalized source derivative, bound the entire bounded early-mode covariance under the stated oriented plaquette clauses, and exhibit a strictly signed failure of the Gaussian comparison for separated constituents of the early mode. The fixed terminal overlap is exactly the remaining signed late sum (FIXED-PLANE-LATE-SCORE), up to a vanishing error.

## 4. Proofs and further deductions

### 4.1 Contact algebra and reflection positivity

The derivative formula in Theorem 3.1 follows by the chain rule because $Z_a$ is source-independent. Cumulants of order m≥2 are invariant under deterministic shifts: adding a constant changes the logarithm of the moment generating function only linearly. A diagonal contact is a sum of derivatives of delta distributions; if the common intersection of compact supports is empty, its evaluation is zero. These facts also prove compatibility by restriction of the source functional.

For the reflection statement take finitely many positive-half sources $J_i$. The bare matrix $M_{ij}=\mathcal Z[\theta\overline{J_i}+J_j]$ is positive semidefinite. SPLIT gives
\[
M^{\rm ren}_{ij}=\overline{d_i}M_{ij}d_j,\qquad d_i=e^{-L[J_i]},
\]
which is a diagonal congruence and therefore positive semidefinite. Difference quotients of exponentials give the polynomial-source matrices by limits of positive semidefinite matrices. Equivalently multiplication by $e^{-L[J]}$ acts triangularly on finite source jets with diagonal one. This proves positivity for the contact-renormalized source algebra without asserting an ordinary random-variable realization. At connected order two the local term $L^{(2)}(\theta\bar f,g)$ vanishes for supports separated from the reflection planes.

The necessity of distinguishing ordinary positivity is concrete: if the bare random variable is identically zero and $L(z)=z^2/2$, then $W^{\rm ren}(z)=-z^2/2$ has second derivative −1. It cannot be the log moment generating function of a real random variable. For a finite-range counterterm, choose a kernel supported at a pair $x\ne y$ on opposite sides of a reflection plane, with $|x-y|$ within its allowed range. Tests near x and y produce a nonzero mixed derivative. Thus finite range alone does not imply SPLIT. This also explains why the off-diagonal remainder in Theorem 3.6 must remain in the physical correlation function.

### 4.2 Triangular normalization and the age sum

Block triangular matrices are invertible exactly when their diagonal blocks are invertible; solving by back-substitution gives a triangular inverse. The leading principal inverse block equals the inverse of the leading principal block. This proves the exact compatibility assertion. It supplies no lower bound on a physical Gram matrix: the latter requires bounds on the actual transported functions, not just the coordinate matrix.

Use $\|I+E_k\|\le1+c_Dg_k^2\le e^{c_Dg_k^2}$ and the Neumann-series estimate $\|(I+E_k)^{-1}\|\le(1-c_Dg_k^2)^{-1}\le e^{2c_Dg_k^2}$. The flow gives
\[
x_j=x_k+b(k-j)-\sum_{u=j}^{k-1}r_u,\qquad x_j=g_j^{-2}.
\]
Its lower bound under $C\bar g^2\le b/2$ gives the logarithmic sum in Theorem 3.2 by comparison of $\sum_{n=1}^K(x_K+bn/2)^{-1}$ with the integral from 0 to K.

For AGE only the upper bound $x_j\le x_k+b_+(k-j)$ and $x_k\ge h$ are needed. Therefore $(g_k/g_j)^q=(x_j/x_k)^{q/2}\le(1+c(k-j))^r\le(1+c(k-j))^d$. Expand the last polynomial. For u≥0,
\[
\sum_{n=0}^{\infty}n^u\rho^n\le\frac{u!}{(1-\rho)^{u+1}}.
\]
For u=0 this is the geometric series. For u>0 use $n^u\le u!\binom{n+u}{u}$ and the binomial generating series. This proves AGE for every finite q. In particular the requirement that q times the small coupling fit into an exponential estimate is an optional simplification, not a necessary restriction on finite-D summation.

**What P6 loses.** If $Q$ lies in the kernel of $P_6$, adding $c_aQ$ to a transported insertion leaves every $P_6$ estimate unchanged for arbitrary divergent $c_a$. Thus no estimate of the retained identity, dimension-four, or other removed jets can be deduced solely from the displayed I-1 contraction. For a dimension-six insertion these rows must be explicitly tracked and subtracted. Powers of L alone do not define their normalization: an integrated dimension-d source with a dimension-e target scales canonically by $L^{4-e}$ after its input units have been fixed, whereas a density coefficient has different units. The procedure here requires the actual coefficient matrix, not a name for its power.

### 4.3 All-order Cauchy estimate and its limitation

Normalize nonzero $J_i$ to unit norm and apply Cauchy's formula in the m variables $z_i$ to $W[\sum_i z_iJ_i]$ on $|z_i|<(R_D/m)$. The source remains in the norm ball. The coefficient of $z_1\cdots z_m$ is the mixed derivative; letting the radii approach $R_D/m$ gives the first CUM estimate. The inequality $m^m\le e^m m!$ gives the second. Zero inputs are handled by multilinearity.

The analytic functions $F_A(z)=A^{-2}(e^{Az}-1-Az)$ have $F_A'(0)=0$, $F_A''(0)=1$, are entire, and have $F_A^{(m)}(0)=A^{m-2}$. They are log moment generating functions of centered compound-Poisson variables with jump A and rate $A^{-2}$. Thus a fixed domain of analyticity plus first/second derivative bounds has no abstract all-order quantitative implication. This is a diagnostic about analytic estimates, not a substitute model of the Wilson law.

AN-D is sufficient, and can be stronger than necessary. For high-degree composites one may instead seek factorial bounds with p>1 directly on source derivatives. For example a power $X^{2r}$, r>1, of a real Gaussian has finite moments of every order but no finite positive exponential moment. Therefore an all-order local source construction must specify whether it is analytic or only has a controlled derivative expansion. This paper does not impose an unproved analytic completion on every irrelevant composite.

### 4.4 Fourier reduction, Wilson Ward locality, and the zero-free improvement

For every link b, Haar integration by parts gives
\[
3t_be^{-\beta S}=\sum_A X_b^A(e^{-\beta S}F_b^A),\qquad
\mathbb Et_b=0,\qquad
\operatorname{Cov}(t_b,G)=-\tfrac13\mathbb E\sum_AF_b^AX_b^AG.
\tag{WARD}
\]
These identities hold exactly for the compact Wilson law. Let $b\sim c$ mean that b,c share a plaquette, including b=c. Each local r,h,t row depends only on the at most 19 links in the plaquettes through its root. Thus $\operatorname{Cov}(t_b,r_c)=\operatorname{Cov}(t_b,h_c)=\operatorname{Cov}(t_b,t_c)=0$ if $b\not\sim c$. Expanding r=h−t gives
\[
E_{bc}:=\operatorname{Cov}(r_b,r_c)-\operatorname{Cov}(h_b,h_c)=0\quad(b\not\sim c).
\]
The complete H contact identity of §4.7 gives $E_{bc}=-\mathbb EB_{bc}$. Section 4.11 proves directly under REG that its row and column absolute sums are at most $C_{W,\sigma}$. The Schur bound therefore gives $\|E\|_{\ell^2\to\ell^2}\le C_{W,\sigma}$. One could alternatively use a separately known local variance bound C2 to get $38C_2$, but no such input is needed here.

Translation invariance makes the covariance of h a convolution in x with a 4×4 orientation matrix $c^h_{\nu\nu'}(z)$. Define $\hat c^h(p)=\sum_z e^{-ipz}c^h(z)$. With unitary transform $\hat f(p,\nu)=n^{-2}\sum_xe^{-ipx}f(x,\nu)$, direct expansion gives
\[
\operatorname{Var}(h_f)=\sum_p\hat f(p)^*\hat c^h(p)\hat f(p),\qquad
M_f=\sum_p|\hat f(p)|^2.
\]
Each symbol is positive semidefinite since it is the covariance matrix of Fourier modes divided by $n^4$. Thus the best susceptibility constant is $\max_p\lambda_{\max}\hat c^h(p)$, and complex plane-wave marks suffice. Real and imaginary parts contribute additively to the ordinary complex variance.

We now prove the improved analytic implication with no Borel–Carathéodory theorem imported. For one of the real plane-wave marks f, let $Z_f(z)=\mathbb Ee^{zh_f}$. Since h_b≥0 and $|f_b|\le1$, M gives $|Z_f(z)|\le e^{An^4}$, where $A=A_\sigma$ for $|z|<R$. Under ZF a holomorphic branch $g_f=\log Z_f$, $g_f(0)=0$, exists on the disc; $\operatorname{Re}g_f\le An^4$.

Write $g_f(z)=\sum_{m\ge1}a_mz^m$. For each $0<r<R$, the nonnegative function $u(\theta)=An^4-\operatorname{Re}g_f(re^{i\theta})$ has mean $An^4$ and nonzero Fourier coefficients $-a_mr^m/2$. Its coefficient magnitude is bounded by its mean, hence $|a_m|\le2An^4r^{-m}$. Letting r increase to R yields
\[
|g_f^{(m)}(0)|\le2An^4m!R^{-m},\qquad
\operatorname{Var}(h_f)=g_f''(0)\le4An^4/R^2.
\]
For a complex plane wave the two real parts give $n^{-4}\operatorname{Var}(h_f)\le8A/R^2$. The Fourier formula and the Ward-local matrix error prove SUS. This proves Theorem 3.4, including every multiplier.

**No extra moment import.** The reduction does not import a marked-set exponential estimate. Section 4.11 proves directly everything actually used here: global M, a uniform first plaquette-action moment, and the complete Ward contact row. Higher local moments are not asserted by that elementary argument and are not needed for SUS.

**Why smooth-source control does not fill ZF.** For a lattice momentum of order one the physical oscillation frequency is of order a−1. Its $C^s$ norm grows as a−s. A fixed physical $C^s$-source ball therefore only admits a scalar source radius of order a^s in that direction. Cauchy's estimate then loses a−2s. Renormalized two-point bounds also permit an arbitrary quadratic contact subtraction, while SUS concerns the unchanged bare ordinary covariance. These are two distinct reasons the susceptibility is not an automatic corollary of CUM.

### 4.5 Reflected boundary factorization and quantitative noncollapse

For the site reflection in Theorem 3.5, decompose the Wilson action exactly as
\[
S(U)=S_\partial(B)+S_+(U_+,B)+S_+(\theta U_-,B).
\]
No plaquette meets both open halves: a plaquette touching a reflection plane lies in one closed half, and plaquettes entirely in a plane contribute to $S_\partial$. Product Haar measure has the analogous decomposition. Conditional on B, the two half-fields are independent and their conditional laws are reflected copies. The boundary law is proportional to $e^{-\beta S_\partial(B)}Z_+(B)^2d\lambda_\partial(B)$. Integrating the two observables separately proves BOUNDARY, including the mean subtraction.

For the lower bound let $P_a$ denote the orthogonal projection onto constants in $L^2(\nu_a)$. If $a_v=\sum v_ia_i$ and $\phi_v=\sum v_i\phi_i$, the centered-error norm is at most the uncentered-error norm, so
\[
\|(I-P_a)a_v\|_2
\ge \|(I-P_a)\phi_v(y_a)\|_2-\varepsilon |v|.
\]
The first squared norm is $\inf_z\int|\phi_v(y)-z|^2d(y_{a*}\nu_a)(y)$, at least $c\inf_z\int|\phi_v-z|^2d\nu_*=c\,v^*\operatorname{Cov}_{\nu_*}(\phi)v$. This proves the bound. It also identifies the null space exactly: a linear combination is null if and only if its boundary conditional mean is constant almost everywhere. An equations-of-motion designation alone does not prove this condition.

If $G_a^\theta\ge\lambda I$ and the finitely many entries converge along a subsequence, then $v^*G^\theta v=\lim_a v^*G_a^\theta v\ge\lambda|v|^2$ for every v. This supplies the required limiting argument once the uniform lower bound is proved. It does not prove the lower bound.

### 4.6 Proof of local Taylor extraction

Apply the one-variable Taylor formula with integral remainder to $t\mapsto g(x+tu)$ between 0 and 1. The order-five remainder has absolute value at most $|u|^5\|D^5g\|_{\mathrm{op},\infty}/5!$. Integrating against the total variation of $K_k$ proves TR. The geometric sum $\sum_{k=0}^K\ell_k\le L\ell_0/(L-1)$ proves uniform summability. The moment bound follows by $|u^\alpha|\le|u|^{|\alpha|}$. The sums of $\ell_k^{q-4}$ are geometric for q<4 and equal K+1 for q=4. Evenness kills odd moments. Since the finite symmetry group preserves distance and the relevant derivative norms, averaging the extraction under that group preserves the estimates. Symmetrization preserves diagonal support.

For m sources use the same Taylor argument along $t\mapsto\prod_{i=2}^m f_i(x+tu_i)$, with the stated joint derivative norm. The power of scale in the remainder is $\ell_k^{q+1-w}$; its sum is at most $\ell_0^{q+1-w}/(1-L^{-(q+1-w)})$. This proves the fixed-order extension and states exactly the norm loss. For terminal torus scales with $\ell_k\ge t^*/(4R)$, sum their full norms directly; their number and the resulting bound depend on $R,t^*,\ell_0,L$, not on a.

### 4.7 Applying the contact calculation to the actual bare H source

The following calculation uses the actual Wilson score and the complete two-source coefficient, including its mixed ordinary responses. It is not a pure-current model.

Write $W_f=\sum_{b,A} f_bF_b^AX_b^A$ and $V_f=-W_f/3$ in the **unscaled** convention of §2.3. Then $D_{V_f}\rho=\rho t_f$ for $D_V\rho=-\operatorname{div}(\rho V)$ and $h_f=t_f+r_f$. For distinct squarefree source labels 1,2, exact conjugation by $e^{-D_{\eta_1V_1+\eta_2V_2}}$ gives
\[
B_{12}
=\tfrac12(V_1t_2+V_2t_1)+V_1r_2+V_2r_1
=V_1h_2+V_2h_1-\tfrac12(V_1t_2+V_2t_1).
\tag{H2}
\]
To verify rather than import this, set $A=\eta_1h_1+\eta_2h_2$, $V=\eta_1V_1+\eta_2V_2$, $t=\eta_1t_1+\eta_2t_2$. If $e^{-sD_V}(\rho e^A)=\rho e^{B(s)}$, then $\partial_sB=VB-t$ and $B(0)=A$. Thus $B(1)=e^VA-\int_0^1 e^{uV}t\,du$, whose mixed coefficient is H2. Integrating the density gives the exact identity
\[
\operatorname{Cov}(h_f,h_g)
=\operatorname{Cov}(r_f,r_g)+\mathbb EB_{12}(f,g).
\tag{H-COV}
\]
Equivalently this follows directly from WARD and integration by parts. This is the full physical coefficient of §155 of the [source estimates](source_estimates/README.md), equations PD12.13–PD12.18.

Expand $B_{12}=\sum_{b,c}f_bg_cB_{bc}(U)$. Every nonzero $B_{bc}$ has $b\sim c$ (or the fixed finite enlargement when the original pointing average is included). In every term at least two first derivatives of a plaquette action survive. For the $\beta D$ and $\beta P$ seeds this follows because multiplying by the force in W adds one first derivative and differentiation consumes at most one. For the scalar seed use the exact Casimir identity $\ell_c=C_F\sum_{p\ni c}(N-s_p)$, whose derivative is a first plaquette derivative. All remaining fixed-order derivatives are bounded by compactness of $SU(N)$. Therefore, pointwise,
\[
|B_{bc}(U)|\le C(\beta+1)\sum_{p\in Y_{bc}}s_p(U),
\tag{H-LOCAL}
\]
with $|Y_{bc}|\le C$ and fixed lattice range. This estimate is P and does not require a moment assumption.

Section 4.11 proves $\mathbb E(\beta s_p)\le C_\sigma$ directly under REG, so
\[
\sum_c|\mathbb EB_{bc}|\le C,\qquad
|\mathbb EB_{12}(f,g)|\le C\|f\|_{\ell^2}\|g\|_{\ell^2}.
\tag{H-ROW}
\]
The same estimates hold for the matrix of $\mathbb E|B_{bc}|$. With original finite pointings, sum their literal product weights and enlarge C by their fixed absolute sum. No shifted roots are identified.

Restoring the physical sources $O_H=c_\beta^{-1}a^{-2}h_f$ and $r_H=c_\beta^{-1}a^{-2}r_f$ multiplies H2 by $c_\beta^{-2}a^{-4}$. Thus the physical contact coefficient per root has size $Ca^{-4}$, and after expressing the root sum as $a^{-4}\int dx$ its anchored physical kernel has total variation $Ca^{-8}$ and range $Ca$. The dimension-six two-source version of Theorem 3.6 consequently has **w=8**, requires Taylor extraction through degree 8, and leaves a remainder bounded by $Ca\|f\|_\infty\|g\|_{C^9}$ at birth. The dimension-four w=4/C5 theorem must not be applied to this unrescaled physical H kernel.

For the separately prescribed tightness rescaling $\widetilde O_H=a^4O_H$, both sources supply $a^8$: the resulting expected contact has per-root size $Ca^4$ and physical row total variation $C$. It is uniformly bounded without further subtraction. Its off-diagonal contribution vanishes for separated fixed physical supports once a is small enough. A nonzero limiting ordinary variance can therefore be entirely a diagonal contact and need not create a reflected excitation.

**Exactly what transport preserves.** For a positive, mass-preserving, source-independent kernel T on the complete physical configuration space, $\|T_*(B_{bc}\mu)\|_{\rm TV}\le\mathbb E|B_{bc}|$. This is immediate from the dual definition of total variation and $\|T\phi\|_\infty\le\|\phi\|_\infty$. Since the source marks remain literal original coordinates, the expected bare H contact retains H-ROW under such a transport when treated as its own signed measure.

But a new logarithmic two-source coefficient is a sum of the transported contact **and a conditional covariance of the degree-one insertions**. More precisely, if an already exact sourced input density has linear coefficients $r_1,r_2$ and mixed coefficient $B_{12}$, and is then pushed forward by a source-independent conditional kernel onto Y, its output satisfies
\[
W_{12}(Y)=\mathbb E[B_{12}\mid Y]
+\operatorname{Cov}(r_1,r_2\mid Y)
\]
with every carrying response included in the exact input prescription. Applying the bare current conjugation to an arbitrary retained carrying function also transforms that function by $e^V$; those responses must be included before using this formula for the physical RG map. The unconditional second derivative of the stated source-independent-kernel representation is
\[
\mathbb EW_{12}(Y)+\operatorname{Cov}(\mathbb E[r_1\mid Y],\mathbb E[r_2\mid Y]).
\]
The covariance term can have long source-anchor range and is not bounded by H-ROW. The first/second derivative clause of I-1 controls it only in the unspecified allowed source norm, not in the row total-variation norm KT. Nor does $P_6$ control its scalar/contact projection. Consequently the actual **bare** contact is now controlled directly under REG, but KT for all newly generated physical-scale contact kernels remains an exact, separate residual. Substituting $\ell_k$ for a in H-LOCAL is not justified: later densities have new scores, moving constraints, and field-dependent coefficients.

### 4.8 A uniform quadratic source domain at every flat background (P)

This section approaches the arbitrary-lattice-mark source problem through its actual quadratic form. It establishes the Gaussian domain exactly, including the soft modes, and separates the nonlinear obstruction.

Fix the generator metric by $-\operatorname{Tr}(T_AT_B)=\tau\delta_{AB}$, $\tau>0$. At any flat lattice background, identify fluctuations by parallel transport. Let $d_i$ be the covariant linearized plaquette curl for the two planes of matching i. Flatness implies
\[
S_{i,2}(A)=\frac{\tau}{2}\|d_iA\|^2,\qquad
M_i=\tau d_i^*d_i\ge0,\qquad M=\sum_iM_i.
\]
Each row of $d_i$ contains four orthogonal parallel transports, and each bond belongs to two matching-i plaquettes. Cauchy–Schwarz followed by incidence counting gives $\|d_iA\|^2\le8\|A\|^2$, hence $\|M_i\|\le8\tau$, uniformly in n and in the flat holonomies.

The first-order matching force is $M_iA$. Therefore the quadratic coefficient of the exact frustration source is
\[
h_{f,2}(A)
=\beta\sum_b f_b\left(\sum_i|(M_iA)_b|^2-\frac13|(MA)_b|^2\right).
\]
For real marks $|f_b|\le1$ the summand in parentheses is nonnegative. Consequently
\[
|h_{f,2}(A)|\le\beta\sum_i\|M_iA\|^2
\le8\tau\beta\sum_i\langle A,M_iA\rangle
=16\tau\beta S_2(A).
\tag{QREL}
\]
This is a relative **quadratic-form** estimate, rather than a bound using the inverse of the smallest nonzero momentum. In particular every vector in $\ker M$ is also annihilated by the source quadratic form. The estimate covers flat torons and does not discard or charge an uncontrolled inverse to their zero modes.

On the real quotient $\mathcal H=(\ker M)^\perp$, write $h_{f,2}(A)=(\beta/2)\langle A,K_fA\rangle$. QREL says $-16\tau M\le K_f\le16\tau M$. Set $Q_f=M^{-1/2}K_fM^{-1/2}$ on this quotient; $\|Q_f\|\le16\tau$. The normalized Gaussian integral is exactly
\[
\mathcal Z_f^{(0)}(z)=\det_{\mathcal H}(I-zQ_f)^{-1/2}.
\]
For $|z|<1/(16\tau)$ it has an analytic branch with value 1 at zero and no zeros or poles. For $|z|\le1/(32\tau)$,
\[
|\log\mathcal Z_f^{(0)}(z)|
\le\frac{\dim\mathcal H}{2}\log2
\le2(N^2-1)n^4\log2.
\tag{GZF}
\]
This proves precisely the required extensive Gaussian log bound and fixed source radius for every bounded real lattice mark, not just smooth marks. The finite-dimensional determinant formula follows by diagonalizing the real symmetric $Q_f$ and integrating one-dimensional Gaussian factors; no comparison to the compact law is used or claimed.

**Nonlinear continuation remains O.** In a uniformly small bond chart around a flat field, differentiating the exact local force expressions and using finite incidence gives perturbations of Hessians bounded by $C\delta\|A\|^2$, where $\delta$ is the chart radius. This absolute bound does not give the relative estimate QREL uniformly: the smallest nonzero eigenvalue of M can have size $n^{-2}$, so absorbing it by a global inverse would require $\delta n^2\ll1$. The logarithmic small-field radii do not meet that requirement. A successful continuation must use the constrained fluctuation covariance at each RG scale, retain source-dependent interactions and large fields, and control the scalar logarithm on the complex disc. I-0c does not state stability of its full representation under this complex source; I-1 does not give a uniform norm for the oscillatory mark class. GZF is the exact quadratic starting lemma for that missing stability theorem.

### 4.9 An explicit nonzero Gaussian reflected test (P for the reference; Wilson comparison O)

For a concrete reflected witness take a real free Maxwell field on $\mathbb R^4$ with $N^2-1$ independent color components and covariance in Feynman gauge
\[
\mathbb E A_\mu^A(x)A_\nu^B(y)=\delta_{AB}\delta_{\mu\nu}D(x-y),
\qquad D(x)=\frac1{4\pi^2|x|^2}.
\]
Only its gauge-invariant curvature covariance is used. Let time be coordinate 4, and set
\[
\mathcal O^{(0)}(x)=\frac12\sum_{A,\mu<\nu}:F_{\mu\nu}^A(x)^2: .
\]
For separated points, Wick contraction gives
\[
\operatorname{Cov}\big(\mathcal O^{(0)}(x),\mathcal O^{(0)}(y)\big)
=\frac{N^2-1}{2}\sum_{\mu<\nu,\rho<\sigma}
C_{\mu\nu,\rho\sigma}(x-y)^2.
\tag{GW}
\]
This is a separated distributional calculation; no ordinary coincident Euclidean random variable is asserted. For the spatial component,
\[
C_{12,12}(z)=-(\partial_1^2+\partial_2^2)D(z)
=\frac{z_4^2+z_3^2-z_1^2-z_2^2}{\pi^2|z|^6}.
\]
Choose $t>0$ and a nonnegative smooth f of integral 1, supported where $|x_4-t|\le t/10$ and $|(x_1,x_2,x_3)|\le t/10$. For two points in this support, the separation from reflection satisfies $z_4\ge1.8t$, $z_4\le2.2t$, and $|z_{\rm space}|\le0.2t$. Hence
\[
C_{12,12}(\theta x-y)
\ge\frac{3.2}{4.88^3\pi^2t^4}
>\frac1{40\pi^2t^4}.
\]
The scalar is reflection even. Every summand in GW is a real square, so retaining just this component proves the explicit reflected lower bound
\[
G_0^\theta(f,f)
\ge\lambda_0:=\frac{N^2-1}{3200\pi^4t^8}>0.
\tag{GLOW}
\]
Thus even a one-element finite test family supplies a concrete nonzero reference excitation.

To use this for the Wilson theory, one must first specify the interacting operator normalization so its leading canonical coefficient is $\mathcal O^{(0)}$; if it is c times that field, replace $\lambda_0$ by $c^2\lambda_0$. Then it is sufficient to prove the actual separated estimate
\[
\left|
G^\theta_a\big(O_a^{\rm ren}(f),O_a^{\rm ren}(f)\big)-G_0^\theta(f,f)
\right|\le\lambda_0/2
\tag{REF}
\]
uniformly in a. It would give $G^\theta_a\ge\lambda_0/2$, with the limit justified by §4.5. At fixed torus, REF must include the finite-volume correction from this $\mathbb R^4$ reference as well as the interacting and lattice errors; choosing t of order $\ell_0$ requires the test to fit the reference torus with a reflection margin. There is no assumption that the torus reference equals the infinite-volume one.

QREL and GLOW do not prove REF: the first is a quadratic action statement at a flat field and the second is a Gaussian correlation calculation. No allowed interface supplies a relative comparison for the physical reflected Schwinger function, or a lower bound on the boundary conditional means in BOUNDARY. The derivative upper bounds and $P_6$ contraction cannot replace this. The next attack is to transport this particular two-source reflected product jointly, keep the complete scalar and mixing rows, compute its leading coefficient at the stopping scale, and bound the remaining joint-history contribution by a fixed fraction of GLOW. The exact norm required is the absolute error in this one smeared reflected matrix entry, not a mass-gap or infinite-volume clustering statement.

### 4.10 An actual compact Wilson reflected witness on a fixed Dirichlet cell (P)

We now pass beyond a Gaussian-only assertion, at fixed lattice geometry. The resulting constant is explicit at leading order; its cutoff scaling also shows why this local result does not yet prove I-3(v).

**Fixed-cell setting.** Let B be a fixed rectangular spatial lattice box with enough interior plaquettes that its transverse edge space is nonzero. Form the spacetime rectangle $B\times\{0,\ldots,M\}$, M even, and fix every link tangential to its outer boundary to the identity. Integrate the remaining links with the actual compact Wilson weight $e^{-\beta S}$. Interior gauge transformations are allowed and equal the identity on the boundary. Constants below depend on this fixed cell and on N; the number of links does not grow in the theorem.

Let $d$ be the spatial gradient with Dirichlet vertex values and C the spatial plaquette curl on the active spatial edges. On $\mathcal E_T=(\operatorname{im}d)^\perp$, choose a unit real eigenvector
\[
C^*Ce=\mu e,\qquad \mu>0,
\]
and put $q=Ce/\mu$, so $C^*q=e$. For a spatial plaquette p at time j, transport $C_N(U_p)$ along a fixed spatial path to one common base vertex. Define the exactly gauge-invariant, real, bounded slice observable
\[
P_j(U)=\left\|\sum_p q_p\,\operatorname{Ad}_{U_{\gamma_p(j)}}C_N(U_p)\right\|_{\mathfrak g}^2.
\tag{CELL-P}
\]
The metric is the one for which the color generators are orthonormal. Paths at times j and M−j are chosen as reflected copies. Thus $\theta P_j=P_{M-j}$, and for $j>M/2$ both the observable and its reflection are separated from the middle reflection plane.

**Theorem (fixed-cell physical reflection bound).** Write $\cosh\omega=1+\mu/2$. For every fixed $M/2<j<M$ there are finite constants $C_B,\beta_B$ such that
\[
\left|
\beta^2\operatorname{Cov}_{B,\beta}(P_j,P_{M-j})
-\frac{2(N^2-1)}{\tau^2}
\left[
\frac{\sinh^2(\omega(M-j))}
{\sinh\omega\,\sinh(\omega M)}
\right]^2
\right|
\le C_B\beta^{-1/2}\qquad(\beta\ge\beta_B).
\tag{CELL-G}
\]
In particular the centered reflected Gram of $\beta P_j$ is at least half the strictly positive displayed leading constant for all sufficiently large beta. This is an estimate for the actual compact-law fixed-cell observable. It needs no assumption about I-0c or I-1.

**Proof of the compact-law comparison.** Fix an interior spanning tree rooted at the connected identity boundary. Exact compact gauge integration sets its links to the identity; the remaining configuration space is a finite product of compact groups with product Haar measure. A zero of S has every plaquette equal to the identity. The rectangular cell is simply connected, so path transport constructs a gauge transformation making every link the identity. It is the identity on the boundary; tree gauge then leaves only the identity configuration. Thus S has a unique zero in the tree-gauge coordinates.

The Hessian H at this zero is positive. Indeed its quadratic form is $\tau\|d_{\rm spacetime}A\|^2$. If it vanishes, zero discrete curl gives a vertex potential by path integration; boundary conditions make that potential constant on the boundary, and tree gauge forces its increments to vanish on the spanning tree, so A=0. Finite dimensionality gives a smallest eigenvalue $\lambda_B>0$. Compactness gives a positive action gap outside a fixed coordinate neighborhood of the identity.

In this neighborhood, with $U=\exp(A)$ on the free links,
\[
S(A)=\tfrac12 A^THA+O_B(|A|^3),\qquad
d\lambda=J_B(A)dA,\quad J_B(A)=J_B(0)+O_B(|A|),
\]
where $J_B(0)>0$. Also
\[
P_j(A)=\sum_{A_{\rm color}=1}^{N^2-1}
\langle e,A_j^{A_{\rm color}}\rangle^2+O_B(|A|^3).
\]
Set $A=\beta^{-1/2}X$. Choose the coordinate neighborhood small enough that $S(A)\ge\lambda_B|A|^2/4$ and the cubic remainder is bounded by $\lambda_B|A|^2/8$. The mean-value formula for exponentials bounds the difference between the scaled weight and its Gaussian weight by
\[
C_B\beta^{-1/2}(1+|X|^3)e^{-c_B|X|^2}.
\]
The same argument, multiplied by the fixed-degree polynomials from $\beta P_j$ and $\beta^2P_jP_{M-j}$, gives integrable Gaussian polynomial bounds of order $\beta^{-1/2}$. Outside the coordinate neighborhood the action gap contributes at most a polynomial in beta times $e^{-\eta_B\beta}$; after division by the partition function, whose leading size is a positive constant times $\beta^{-\dim(H)/2}$, it is smaller than the same error. This proves convergence with the stated error for the means and mixed second moment, hence for the connected covariance. Every comparison here is to the original normalized compact integral, with its full complement included.

**Evaluation of the leading covariance.** In the linearized theory, decompose each spatial edge field orthogonally into a gradient part and its transverse part. Spatial curl kills the gradient part. The temporal electric quadratic form is $\|\nabla_0A-dA_0\|^2$; its transverse component is exactly $\|\nabla_0A^T\|^2$, independent of the longitudinal and temporal variables. Therefore the transverse mode $X_j=\langle e,A_j^T\rangle$ has, for each color, quadratic action
\[
\frac{\tau}{2}\left\{\sum_{j=0}^{M-1}(X_{j+1}-X_j)^2+
\mu\sum_{j=1}^{M-1}X_j^2\right\},\qquad X_0=X_M=0.
\]
This gauge-invariant covariance can be evaluated in any gauge, so the tree-gauge calculation gives the same answer. The inverse of the tridiagonal matrix with diagonal $2+\mu$ and off-diagonal −1 is
\[
G_\mu(i,j)=
\frac{\sinh(\omega\min(i,j))\,
\sinh(\omega(M-\max(i,j)))}
{\sinh\omega\,\sinh(\omega M)}.
\]
One verifies this formula by applying the difference operator away from i=j, checking its zero boundary values, and its unit jump at i=j. The covariance of a color mode is $\tau^{-1}G_\mu$. Wick's finite-dimensional Gaussian identity gives
$\operatorname{Cov}(\sum_AX_j^{A\,2},\sum_AX_{M-j}^{A\,2}) =2(N^2-1)\tau^{-2}G_\mu(j,M-j)^2$.
This proves CELL-G.

**The cutoff scaling is decisive.** CELL-G is uniform in beta only with the cell fixed in lattice units. It yields a real reflected excitation localized on a shrinking physical cell as $a\to0$. It does not yield a fixed positive-time test at scale $\ell_0$.

For an explicit diagnostic, keep the spatial cell fixed, so $\mu>0$ and $\omega>0$ remain fixed, but move the test to physical distance t from the mirror by $j-M/2=t/a$. The Dirichlet Green function is bounded by its infinite-line counterpart,
\[
0<G_\mu(j,M-j)\le\frac{e^{-2\omega t/a}}{2\sinh\omega}.
\]
This follows directly from the displayed formula, or from the positive Dirichlet resolvent. Thus the Gaussian reflected norm is at most
\[
\frac{N^2-1}{2\tau^2\sinh^2\omega}e^{-4\omega t/a}.
\]
No fixed polynomial renormalization in a can turn this high-lattice-momentum witness into a nonzero physical reflected limit. To keep a physical mode, one needs $\mu=O(a^2)$ and a spatial cell whose side grows like a−1. The constants $\lambda_B,\eta_B,C_B$ in the compact-law Laplace proof are then no longer fixed. Replacing a by the stopping scale $\ell_0$ would produce a fixed-size witness only after proving that the **physical jointly transported insertion** has a controlled nonzero component along that coarse witness. This is the precise remaining passage, rather than a failure of positivity at fixed cutoff.

### 4.11 Real frustration pressure and Ward contact row from the full Wilson law (P)

This closes the previously displayed real-moment input for the susceptibility reduction. It uses the full compact Wilson law, with no small-field restriction or RG import.

Fix $\sigma>0$ and consider $n\ge3$, $\beta\ge1$ with
\[
\log\beta\le\sigma n.
\tag{REG}
\]
This includes every trajectory $\beta(a)=O(\log(t^*/a))$ for sufficiently small a, but REG, not an unimported trajectory theorem, is the hypothesis used here. Put $d_G=N^2-1$ and
\[
q_\beta=\int_G e^{-\beta(N-\operatorname{Re}\operatorname{Tr}U)}\,dU.
\]
There are constants $c,C>0$ depending only on G and its metric such that
$q_\beta\le C\beta^{-d_G/2}$ for every $\beta\ge1$. Indeed the action has its unique minimum at I, has a positive quadratic Hessian there, and is bounded away from zero off any identity neighborhood. Haar measure in an exponential chart has bounded smooth density. Integrating the local Gaussian bound and the compact complement proves the claim; enlarging C gives the same bound for $0<\beta<1$.

**Full-tree lower bound.** The periodic graph has $n^4$ vertices and $4n^4$ positively oriented links. Exact spanning-tree gauge fixing leaves
\[
R_n=3n^4+1
\]
free group variables. Restrict each of these variables to a Haar ball of radius $\delta\beta^{-1/2}$ around I, for one fixed small $\delta>0$. The volume of each ball is at least $c_\delta\beta^{-d_G/2}$. Every plaquette is a product of four links, each either fixed to I by the tree or in such a ball, so its action is at most $C_\delta/\beta$. There are $6n^4$ plaquettes. Therefore
\[
Z_\beta\ge e^{-C_Ln^4}\beta^{-d_GR_n/2}.
\tag{ZT-L}
\]
All gauge changes preserve the normalized product Haar measure exactly. This is a lower bound by a small set, not an assertion that its complement can be discarded in a renormalized representation.

**Temporal-forest upper bound.** Gauge-fix all links in direction 4 with time coordinate $0,\ldots,n-2$ to I, leaving the wrap links unfixed. Discard every action term except the temporal plaquettes in planes $(\mu,4)$, $\mu=1,2,3$, at those times. Since every plaquette action is nonnegative, this gives an upper bound for the partition function. For each of the $3n^3$ spatial bonds, its n spatial link matrices form one independent Haar chain with n−1 factors
$e^{-\beta s(U_tU_{t+1}^{-1})}$. Sequential Haar integration gives exactly $q_\beta^{n-1}$. The unfixed temporal wrap variables integrate to one. Thus
\[
Z_\beta\le q_\beta^{T_n},\qquad T_n=3(n-1)n^3.
\tag{ZT-U}
\]
Spatial wrap bonds obey the same chain calculation.

For any fixed $0<\gamma<1$, combine ZT-L at beta with ZT-U at $\gamma\beta$. Since $R_n-T_n=3n^3+1$,
\[
\log\frac{Z_{\gamma\beta}}{Z_\beta}
\le C_\gamma n^4+\frac{d_G}{2}(3n^3+1)\log\beta.
\tag{RATIO}
\]
Here $C_\gamma$ depends on $N,\tau,\gamma$, not on n or beta. Under REG, the right side is at most $A_{\gamma,\sigma}n^4$. This is an extensive bound in the **number of lattice sites**. It does not compare renormalized physical pressure densities across tori and therefore does not supply or contradict S94.

**Global frustration domination.** Orthogonality of $T_A/\sqrt\tau$ in the real Hilbert–Schmidt metric gives the sharp pointwise bound
\[
\sum_A|X_b^As_p|^2\le\tau\|U_p-I\|_{\rm HS}^2=2\tau s_p.
\]
A matching has at most two plaquettes through b, so
$|F_{b,i}|^2\le4\tau\sum_{p\ni b,\;p\in i}s_p$.
Each plaquette has four edges. Consequently, on the whole compact configuration space,
\[
0\le\sum_b h_b\le16\tau\beta S.
\tag{GLOBAL-H}
\]
Taking $R_0=1/(32\tau)$ and $\gamma=1/2$ in RATIO yields
\[
\log\mathbb E_\beta\exp\left(R_0\sum_bh_b\right)
\le\log(Z_{\beta/2}/Z_\beta)
\le A_\sigma n^4.
\tag{REAL-M}
\]
Thus the one-sided real hypothesis M of the original reduction is now proved directly under REG.

**First action moment.** Convexity of $F(\beta)=\log Z_\beta$ gives
\[
\beta\mathbb E_\beta S\le2\left[\log Z_{\beta/2}-\log Z_\beta\right]\le2A_\sigma n^4.
\]
All $6n^4$ plaquettes have the same mean by translations and lattice rotations, so
\[
\beta\mathbb E_\beta s_p\le A_\sigma/3.
\tag{FIRST}
\]
For $\beta\in[1,2]$ the same assertion, with an enlarged constant, also follows immediately from $s_p\le2N$.

**Ward contact row without local second moments.** Apply FIRST to the pointwise complete H contact bound H-LOCAL:
\[
\mathbb E_\beta|B_{bc}|
\le C(\beta+1)\sum_{p\in Y_{bc}}\mathbb E_\beta s_p
\le C_\sigma.
\]
The matrix has a fixed bounded number of nonzero entries in each row and column. H-COV says
\[
\operatorname{Cov}(r_b,r_c)-\operatorname{Cov}(h_b,h_c)
=-\mathbb EB_{bc}.
\]
Therefore its $\ell^2$ operator norm is at most a constant $C_{W,\sigma}$ independent of n and beta under REG. No local second-moment estimate and no chessboard dissemination are needed for this step. The same argument proves H-ROW for the physical contact after restoring its stated multiplier.

Combining REAL-M, this direct Ward-row bound, the plane-wave Fourier formula, and the harmonic-coefficient proof in §4.4 gives the strengthened conclusion: **the only remaining input for the fixed-reference-torus susceptibility is ZF**. No separate real-moment input (ICR-3-MOM) is needed for this application, by the elementary full-law estimates above.

### 4.12 The retained action row and the exact physical Gram error needed

This section tests the stopping-scale route against the precise allowed interfaces.

**Constant-source differentiation (P identity, with its representation assumptions explicit).** Put $x=g^{-2}$ and $c_N=2N^2$, so the bare Wilson exponent is $-c_Nx_0Y_0$ for the normalized integrated plaquette density $Y_0=\sum_xa^4\mathcal O_a(x)$. A constant source $uY_0$ is exactly $x_0\mapsto x_0-u/c_N$. Suppose a differentiable family of complete representations is written with a fixed extraction convention as
\[
\rho_K(x_0,U)=
\exp\{-V_*e_K(x_0)-c_Nx_K(x_0)Y_K(U)-V_K(x_0,U)\},
\tag{ROW-REP}
\]
where $Y_K$ is independent of $x_0$ and the retained action coefficient has been normalized to $c_Nx_K$. Differentiating the representation obtained by running the shifted-coupling algorithm gives the constant-source insertion
\[
\mathcal A_K=
x_K'(x_0)Y_K+\frac{V_*}{c_N}e_K'(x_0)
+\frac1{c_N}\partial_{x_0}V_K.
\tag{ROW}
\]
This formula retains the identity and interaction derivatives. If the representation includes several sectors, it is first an identity for their undivided density derivative; replacing it by a derivative of one selected sector is not valid. A source-independent transport algorithm may distribute the same derivative differently among its carrying responses; the integrated identity is unchanged.

The coefficient $z_K=x_K'(x_0)$ is therefore the natural candidate for the marginal action row, once ROW-REP and a common local extraction are established. The exact I-0c statement does not specify differentiability in complex coupling, a coupling-independent $Y_K$, or that this normalization identifies the whole local source row. A constant source fixes only zero momentum; a divergence term can have zero integral and still affect positive-time local tests.

**The real flow estimate does not bound this derivative (P diagnostic).** For any large $x_*>0$ and C>0 define, on x>0,
\[
r(x)=-\frac Cx\sin\!\left(\frac{x_*}{C}(x-x_*)\right).
\]
Then $|r(x)|\le C/x$, $r(x_*)=0$, and $r'(x_*)=-1$. Thus the flow map $F(x)=x-b+r(x)$ satisfies exactly the size of the I-0c remainder, yet $F'(x_*)=0$. Its output remains in an admitted positive range if $x_*$ is large. This is not a Wilson counterexample; it proves that the numerical flow bound alone cannot establish a nonzero retained action coefficient.

**What proportional complex control would give.** If a closed scalar step map $F_j(x)=x-b+r_j(x)$ is holomorphic on $|z-x_j|\le\eta x_j$ and satisfies $|r_j(z)|\le C/|z|$, then Cauchy's estimate gives
\[
|r_j'(x_j)|\le A/x_j^2,\qquad A=C/[\eta(1-\eta)].
\]
If $x_j\ge x_K+c(K-j)$ and $A/x_K^2\le1/2$, the chain rule and the geometric/integral bound give
\[
e^{-2A/(cx_K)}\le
\left|\prod_{j<K}(1+r_j'(x_j))\right|
\le e^{A/(cx_K)},\qquad
\left|\prod_{j<K}(1+r_j'(x_j))-1\right|
\le e^{A/(cx_K)}-1.
\tag{ROW-CF}
\]
This is a cutoff-independent nonzero coefficient with error $O(g_K^2)$. If the effective map depends on other running coordinates, the derivative must be the derivative of the complete slaved family or of the full coupled map; holding those coordinates artificially fixed changes ROW. T1's proportional-disc analysis addresses this precise additional requirement. It is not part of I-0c's real remainder estimate.

**Exact reflection-error budget.** Work in the original positive-half algebra, with its actual reflected seminorm. Suppose a canonically normalized physical insertion has an exact decomposition
$A_a^{\rm can}=z_aF_a^{\rm can}+R_a+c_a$,
where the identity is removed by centering and all terms are positive-half observables. Reflection positivity and ordinary Cauchy–Schwarz imply
\[
\|R_a\|_\theta\le\sqrt{\operatorname{Var}(R_a)},\qquad
G_a^\theta(A_a^{\rm can},A_a^{\rm can})
\ge\left(|z_a|\sqrt{G_a^\theta(F_a^{\rm can},F_a^{\rm can})}
-\sqrt{\operatorname{Var}(R_a)}\right)_+^2.
\tag{GRAM-BUDGET}
\]
Indeed the reflected form is positive semidefinite, hence obeys its triangle inequality, while
$|\operatorname{Cov}(\theta R_a,R_a)|\le \sqrt{\operatorname{Var}(\theta R_a)\operatorname{Var}(R_a)} =\operatorname{Var}(R_a)$.
Thus a witness lower bound $\lambda_0$ and $|z_a|\ge z_0>0$ require only the concrete error
$\operatorname{Var}(R_a)\le z_0^2\lambda_0/4$ to produce
$G^\theta(A_a^{\rm can})\ge z_0^2\lambda_0/4$.

For raw action density, the leading canonical amplitude is of order $g_*^2$ at the stopping scale. Before dividing by that factor, the required error is
$\operatorname{Var}(R_a^{\rm raw})\le z_0^2g_*^4\lambda_0/4$,
up to the fixed convention coefficient. An ungraded $O(g_*)$ bound on an amplitude does not meet this $O(g_*^2)$ amplitude requirement. The canonical-degree conversion and the actual remainder covariance must be supplied. The I-1 displayed P6 contraction does not control the removed rows or the absolute sum of birth/history norms; its first/second derivative statement gives uniform bounds in its specified norm, not this small relative error by itself.

Finally $F_a^{\rm can}$ must be an actual positive-half physical observable, or its coarse representation must preserve the joint reflected product. Inserting a convenient fixed-cell coarse reference field into GRAM-BUDGET without such a map would not be a valid use of reflection positivity.

**An exact boundary-response version (P).** For any real positive-half observable A supported away from the reflection planes, tilt the actual Wilson law by the reflection-symmetric source
$d\mu_\lambda\propto e^{-\lambda(A+\theta A)}d\mu$.
Let $\nu_\lambda$ be its boundary marginal in BOUNDARY. Conditional independence of the two halves gives
\[
\left.\partial_\lambda\log\frac{d\nu_\lambda}{d\nu_0}(B)\right|_0
=-2\big(\mathbb E[A\mid B]-\mathbb EA\big).
\]
Consequently
\[
G^\theta(A,A)=\frac14
\int\left|\left.\partial_\lambda\log\frac{d\nu_\lambda}{d\nu_0}\right|_0\right|^2d\nu_0,
\quad
G^\theta(A,A)\ge
\frac{|\left.\partial_\lambda\mathbb E_{\nu_\lambda}\phi\right|_0|^2}
{4\operatorname{Var}_{\nu_0}\phi}
\tag{BOUNDARY-RESPONSE}
\]
for every nonconstant square-integrable boundary test $\phi$. The inequality is ordinary Cauchy–Schwarz against the boundary score. This identifies a concrete alternative lower-bound target: one nonvanishing physical response of a boundary Fourier or curvature mode. A nonzero bulk coupling coefficient does not automatically prove such a response; the source could affect an interior factor whose normalized boundary marginal is unchanged.

### 4.13 Explicit first constrained Gaussian rows for the action, H, and the Ward companion

This computes retained coefficients rather than assigning them names. All covariance formulas refer to the actual constrained quadratic form supplied to the step. The nonlinear comparison is stated separately with the precise differentiable remainder it needs.

**Constrained geometry.** Work in finite gauge-fixed coordinates on which the fine quadratic action is
$S_2(A)=\frac12 A^THA$, $H>0$. Let Q be a surjective linearized block constraint and retain $QA=B$. Define
\[
\Sigma=QH^{-1}Q^*,\qquad \Gamma=\Sigma^{-1},\qquad
E=H^{-1}Q^*\Gamma,\qquad
C=H^{-1}-H^{-1}Q^*\Gamma QH^{-1}.
\tag{CONSTRAINT}
\]
Then $QE=I$, $QC=0$, $C\ge0$, and the constrained Gaussian field is
$A=m+\zeta$, $m=EB$, with covariance $\mathbb E\zeta\zeta^*=C/\beta$.
These assertions follow either by completing the square with Lagrange multipliers or by changing to a basis of $\ker Q$ and its H-orthogonal complement. In particular
\[
S_2(m+\zeta)=S_2(m)+S_2(\zeta),\quad
CHm=0,\quad S_2(m)=\tfrac12B^T\Gamma B.
\]
The number of fluctuating real coordinates is $d_f=\dim\ker Q$ and
$\operatorname{Tr}(HC)=d_f$.

**Action insertion: exact row and every scalar contact.** The conventionally normalized integrated bare action density is $Y=S_2/N$. Its constant source u changes $\beta$ to $\beta-u/N$. At frozen B the Gaussian sourced ratio is exactly
\[
\frac{Z_{\beta-u/N}^{(0)}(B)}{Z_\beta^{(0)}(B)}
=\exp\!\left(\frac uN S_2(EB)\right)
\left(1-\frac{u}{N\beta}\right)^{-d_f/2}.
\tag{ACTION-GEN}
\]
Hence
\[
\mathbb E[Y\mid B]=\frac{S_2(EB)}N+\frac{d_f}{2N\beta},\qquad
\operatorname{Var}(Y\mid B)=\frac{d_f}{2N^2\beta^2}.
\tag{ACTION-ROW}
\]
For m≥2 the conditional source cumulant is
$d_f(m-1)!/(2N^m\beta^m)$.
The retained action coefficient is exactly one; its canonical $\beta Y$ identity row is $d_f/(2N)$. Here $d_f$ counts physical constrained fluctuations. When using the native augmented gauge integral, §4.25 computes that physical dimension and distinguishes it from the auxiliary gauge coordinates. The second contact is a scalar and has no retained-field quadratic part. This vanishing is the orthogonality identity $CHm=0$, not an assumption that all contacts are scalars.

**H insertion: exact identity, retained quadratic row, and new contact.** Let
$h_i=(\beta/2)A^TK_iA$, where $K_i$ is the actual symmetric quadratic form of the frustration mark. Direct Gaussian integration gives
\[
\mathbb E[h_i\mid B]
=\frac\beta2 B^TE^*K_iEB+\frac12\operatorname{Tr}(K_iC),
\tag{H-GROW}
\]
\[
\operatorname{Cov}(h_i,h_j\mid B)
=\beta B^TE^*K_iCK_jEB
+\frac12\operatorname{Tr}(K_iCK_jC).
\tag{H-GCONTACT}
\]
For real symmetric matrices the scalar background expression is symmetric in i,j, since its transpose interchanges i,j. To verify the formula, expand
$h_i-\mathbb E[h_i\mid B] =\beta m^TK_i\zeta+(\beta/2)(\zeta^TK_i\zeta-\operatorname{Tr}(K_iC)/\beta)$.
The mixed cubic terms vanish, and the linear and quadratic Gaussian contractions give the two displayed terms.

QREL gives $-cH\le K_i\le cH$ with $c=16\tau$ for $|f_i|\le1$. Since C is the H-orthogonal fluctuation inverse, it follows that
\[
\left|\tfrac12\operatorname{Tr}(K_iCK_jC)\right|
\le \tfrac12c^2d_f,\qquad
\left|\beta m^TK_iCK_jm\right|
\le c^2\beta\,m^THm=2c^2\beta S_2(m).
\tag{H-GBOUND}
\]
For the first inequality restrict to $\ker Q$ and use the operator bounds on
$C^{1/2}K_iC^{1/2}$; for the second use $C\le H^{-1}$ and
$\|H^{-1/2}K_iH^{-1/2}\|\le c$.
Thus the first new H contact has both a bounded scalar row and an explicitly controlled background quadratic row. Dropping the latter would alter the joint source.

**Ordinary r and Ward t do not merge.** Let $H_i$ be the three matching Hessians, $H=\sum_iH_i$, and F the diagonal matrix of the real bond marks, repeated on color coordinates. Set
\[
D_f=\sum_iH_iFH_i,\qquad P_f=HFH.
\]
Then the exact quadratic/constant rows of the unscaled sources are
\[
r_f=\beta A^TD_fA-\tfrac13\operatorname{Tr}(FH),\quad
h_f=\beta A^T(D_f-P_f/3)A,\quad
t_f=\tfrac13\operatorname{Tr}(FH)-\tfrac\beta3A^TP_fA.
\]
Since $H-HCH=Q^*\Gamma Q$, the conditional Ward row is
\[
\mathbb E[t_f\mid B]
=\frac13\operatorname{Tr}(QFQ^*\Gamma)
-\frac\beta3 B^T\Gamma QFQ^*\Gamma B.
\tag{WARD-COARSE}
\]
This is exactly the Gaussian Ward divergence of the retained density
$e^{-\beta B^T\Gamma B/2}$ with vector field
$V_B=-(QFQ^*\Gamma B)/3$.
Its conditional mean need not vanish. Subtracting WARD-COARSE from H-GROW gives the transported ordinary row, including the original Casimir companion. This prevents an erroneous identification of the physical frustration insertion with the ordinary source at retained field B.

**Dictionary for the native first step.** Following T1 ([Transport of insertions on a reference torus](insertion_transport.md)), Balaban CMP 109 (1987), printed pp. 267–268, identifies the nonlinear constrained readout as
$B'=g_B\mathcal C B-hD(g_B\mathcal C B)$,
with $Q\mathcal C=0$, and the actual independent Gaussian precision as
$\mathcal C^*A^{(k)}\mathcal C$.
At the flat first-step background the quadratic H readout is the pullback
$\mathcal C^*K_h\mathcal C$; the nonlinear $D$ begins at quadratic field order and does not change that quadratic insertion. In the conventions of §1
\[
g_B^{-2}(S/N)=\beta S,\qquad
\beta=g_B^{-2}/N,\qquad g_B=g_0/(\sqrt2\,N).
\]
Thus, writing $A_{\rm fl}=\mathcal C^*A^{(0)}\mathcal C$, the literal first Gaussian H identity row is
\[
\frac1{2N}\operatorname{Tr}
\left(\mathcal C^*K_h\mathcal C\,A_{\rm fl}^{-1}\right).
\tag{NATIVE-TRACE}
\]
The covariance is the actual constrained one; no unrestricted Maxwell inverse is inserted. If $A_{\rm fl}$ is written in the unnormalized original Wilson Hessian convention, it must be divided by N correspondingly. Agreement with H-GROW checks this conversion. At nonzero retained background, derivatives of the constrained minimizer, this precision, the readout, and the Jacobian all contribute; the flat identity trace alone does not identify the action-mixing coefficient. The source dictionary and its printed-page provenance are recorded here as the exact first-step object to be checked, not as an independently verified all-history propagator theorem.

**Actual nonlinear action row from a controlled constrained Laplace remainder.** Suppose the actual constrained compact integral at fixed retained B has been proved in the form
\[
Z_w(B)=e^{-wS_*(B)}w^{-d_f/2}a(B)e^{\mathcal E(w,B)},
\quad
|\mathcal E(w,B)|\le A_Q/|w|
\tag{LAP-ROW}
\]
on $|w-\beta|\le\eta\beta$ and a retained complex B-ball of radius $\delta_Q$, with $a(B)$ nonzero and independent of w. The physical constraint measure, integration domain and retained B are held fixed when w varies. A cutoff frozen only in coupling-rescaled Gaussian coordinates does not meet this requirement; its exact flux correction is proved in §4.21. T1's actual fixed-block theorems establish this structure for their displayed block integrals; applying it to the native constrained first step requires the corresponding measure/readout dictionary, rather than silently substituting a Dirichlet boundary integral.

For the actual action source $uS/N$, differentiation is exact:
\[
O_{Y,\beta}(B)=\frac{S_*(B)}N+\frac{d_f}{2N\beta}
-\frac1N\partial_\beta\mathcal E(\beta,B),
\tag{ACTUAL-ACTION-ROW}
\]
\[
W_{YY,\beta}(B)=\frac{d_f}{2N^2\beta^2}
+\frac1{N^2}\partial_\beta^2\mathcal E(\beta,B).
\tag{ACTUAL-ACTION-CONTACT}
\]
The background-dependent one-loop determinant $\log a(B)$ drops out of these coupling derivatives because it is w-independent. This is the explicit reason the marginal Jacobian correction starts at order $\beta^{-2}$ rather than $\beta^{-1}$.

Cauchy on smaller discs gives
\[
|\partial_\beta\mathcal E|\le
\frac{A_Q}{\eta(1-\eta)\beta^2},\qquad
|\partial_\beta^2\mathcal E|\le
\frac{2A_Q}{\eta^2(1-\eta)\beta^3}.
\]
For unit retained directions v,w, Cauchy on
$B=z_1v+z_2w$, $|z_i|\le\delta_Q/2$, gives
\[
|D_B^2\partial_\beta\mathcal E(0)[v,w]|
\le\frac{4A_Q}{\eta(1-\eta)\delta_Q^2\beta^2}.
\tag{ACTION-ERROR}
\]
If the classical retained Hessian has smallest positive eigenvalue $\lambda_Q$, the relative quadratic action-row error is therefore at most
$4A_Q/[\eta(1-\eta)\lambda_Q\delta_Q^2\beta^2]$.
All factors that must be controlled for a growing native block are now visible.

If the actual native estimates yield
$A_Q/(\lambda_Q\delta_Q^2)\le C(\log\beta)^p$
for fixed integer p, then this row error is summable along
$\beta_j\ge\beta_K+c(K-j)$, once $\beta_K\ge e^{p/2}$:
\[
\sum_{j<K}\frac{(\log\beta_j)^p}{\beta_j^2}
\le\frac1{c\beta_K}
\sum_{r=0}^{p}\frac{p!}{(p-r)!}(\log\beta_K)^{p-r}.
\]
The integral formula follows by p integrations by parts. Thus a nonzero total marginal coefficient can follow from a sufficiently small terminal coupling with these *actual* row estimates. The open step is the native, background-uniform constrained estimate LAP-ROW (and its nonconstant-source extension), not the Gaussian row calculation or the summation algebra.

### 4.14 All-order connected Gaussian source kernels with native locality (P with checked L input)

This supplies the anchored absolute kernel estimate for the **first constrained Gaussian step**, at every source order. It does not estimate its nonlinear compact correction.

**Checked covariance input (L, at the flat background).** Balaban, *Propagators for lattice gauge theories in a background field*, CMP 99 (1985), printed p. 428, equations (3.157)–(3.158), identifies the physical constrained covariance as
\[
C^{(k)}=\mathcal C(\mathcal C^*\Delta_k\mathcal C)^{-1}\mathcal C^*.
\]
Printed p. 432, Theorem 3.15, equation (3.187), proves exponential decay
$|C^{(k)}(y,y')|\le B_0e^{-\delta_0|y-y'|}$, with its stated regular-domain hypotheses and $M\alpha_0$ sufficiently small. The regularity conditions (3.35)–(3.36), printed p. 396, require local gauges with bounds on A, its first derivative, and $d^*dA$. At the identity background A=0 all these conditions hold for every positive sufficiently small $\alpha_0$. The fluctuation region must still be a union of the theorem's big blocks with its prescribed boundary margin. The result is not asserted on an arbitrary large-field history.

For the canonically scaled physical fluctuation $X=\sqrt\beta\,A=B_{\rm native}/\sqrt N$, the covariance is
$C_X=C^{(0)}/N$. Absorb fixed norm-equivalence constants into $C_0$ and reduce $\delta_0$ if needed so that
\[
\|C_X(x,y)\|_{\rm color}\le C_0e^{-\delta d(x,y)}
\tag{CEXP}
\]
in unit-lattice bond distance. One may equivalently work in independent coordinates, but the trace identities below use the **physical** covariance. Thus the locality of the original source is not lost inside an unspecified pullback matrix. The singularity of $C_X$ on eliminated gauge/constraint directions causes no problem: determinants are taken on its range, and all trace formulas remain valid.

**The actual quadratic source is local (P).** At the flat background, let $H_i$ be the Hessian of matching-i Wilson action. Each row $H_i(b,\cdot)$ is supported on the plaquettes through b in that matching and has block-operator absolute row sum at most $8\tau$: there are two plaquettes, each with four signed parallel transports. The total H row sum is at most $24\tau$. Let $P_b$ be the projection onto the color coordinates of bond b. The original frustration quadratic source is exactly
\[
h_b^{(2)}(X)=\tfrac12X^TK_bX,\qquad
K_b=2\sum_iH_i^*P_bH_i-\tfrac23H^*P_bH.
\tag{LOCAL-K}
\]
Both indices of $K_b$ lie in $D(b)$, the at most 19 bonds sharing a plaquette with b. Moreover
\[
\sum_{x,y}\|K_b(x,y)\|_{\rm color}
\le 2\cdot3(8\tau)^2+\tfrac23(24\tau)^2
=:\kappa=768\tau^2.
\tag{KTV}
\]
For the original finite pointing average, retain each shifted stencil and multiply $\kappa$ by the fixed absolute sum of its weights. These statements concern the literal physical quadratic readout. At the first step the nonlinear constraint correction begins at quadratic field order, so its substitution into the quadratic H source contributes only field degree three and higher; it does not change LOCAL-K.

Let $r_s$ bound the distance from b to its determining stencil, and set
\[
J=\kappa C_0e^{2\delta r_s},\qquad
S_\alpha=\sup_b\sum_c e^{-\alpha d(b,c)}.
\]
For $\alpha>0$, $S_\alpha$ is finite uniformly in the finite torus or subdomain. For the $\ell^1$ site-distance convention one can take
$S_\alpha\le4[(1+e^{-\alpha})/(1-e^{-\alpha})]^4$,
up to a fixed bond-center convention factor. Color is accounted for separately by $d_G=N^2-1$.

**Scalar cycle theorem.** For the centered Gaussian fluctuation, define
\[
W_0(t)=\log\mathbb E\exp\!\left(\sum_b t_bh_b^{(2)}\right)
=-\tfrac12\log\det(I-C_XK(t)),\quad K(t)=\sum_bt_bK_b.
\]
For labels $b_1,\ldots,b_m$, including repeated anchors, its mixed derivative at zero is
\[
\kappa^{G}_{m}(b_1,\ldots,b_m)
=\frac1{2m}\sum_{\pi\in S_m}
\operatorname{Tr}(C_XK_{b_{\pi(1)}}\cdots C_XK_{b_{\pi(m)}})
=\frac12\sum_{\pi\in S_{m-1}}
\operatorname{Tr}(C_XK_{b_1}C_XK_{b_{\pi(2)}}\cdots C_XK_{b_{\pi(m)}}).
\tag{CYCLE}
\]
For $m=1$ the last sum has one term. For every $0\le\delta'<\delta$, let $\mathcal T(b_1,\ldots,b_m)$ be the minimum length of a tree joining the anchors. Then
\[
\sup_{b_1}\sum_{b_2,\ldots,b_m}
e^{\delta'\mathcal T(b_1,\ldots,b_m)}
|\kappa^{G}_{m}(b_1,\ldots,b_m)|
\le\frac{d_G}{2}(m-1)!\,J^m S_{\delta-\delta'}^{m-1}.
\tag{G-KT}
\]
This is a true anchored absolute bound, uniform in the number of blocks and the lattice cutoff in unit-scale coordinates.

**Proof.** Expand the determinant logarithm as
$\frac12\sum_{m\ge1}\operatorname{Tr}(C_XK(t))^m/m$ near zero. Taking labeled derivatives gives the first expression in CYCLE; cyclicity of trace gives the second, with b1 fixed first. Each product is a sum over the two local indices at every source vertex. CEXP, KTV, and
$d(x_i,y_{i+1})\ge d(b_i,b_{i+1})-2r_s$
give the termwise estimate
\[
|\operatorname{Tr}(C_XK_{b_1}\cdots C_XK_{b_m})|
\le d_GJ^m\exp\!\left[-\delta\sum_{i=1}^{m}d(b_i,b_{i+1})\right],
\quad b_{m+1}=b_1.
\]
A cycle connects the anchors, so its length is at least $\mathcal T$. After paying the tree weight, keep exponent $\delta-\delta'$ on the cycle. Drop its closing edge and sum along the remaining path; each new anchor costs at most $S_{\delta-\delta'}$. There are $(m-1)!$ cyclic orders. This proves G-KT without losing an additional factorial or a volume factor.

**Retained-background open chains.** For a fixed canonical mean field $\xi$ the same Gaussian integral gives
\[
W_\xi(t)=W_0(t)+\tfrac12\xi^TK(t)(I-C_XK(t))^{-1}\xi.
\]
Its m-source background contribution is
\[
b_m^\xi(b_1,\ldots,b_m)
=\tfrac12\sum_{\pi\in S_m}
\xi^TK_{b_{\pi(1)}}C_XK_{b_{\pi(2)}}\cdots C_XK_{b_{\pi(m)}}\xi.
\tag{CHAIN}
\]
With $\|\xi\|_\infty$ the maximum Euclidean color norm at one physical bond,
\[
\sup_{b_1}\sum_{b_2,\ldots,b_m}
e^{\delta'\mathcal T}
|b_m^\xi(b_1,\ldots,b_m)|
\le\frac{m!}{2}\|\xi\|_\infty^2
\kappa J^{m-1}S_{\delta-\delta'}^{m-1}.
\tag{CHAIN-KT}
\]
Indeed each path has m source vertices and m−1 covariance edges. KTV bounds its endpoints against $\|\xi\|_\infty^2$ and the other factors as before. The fixed anchor b1 may lie inside the path; sum independently in its two directions to obtain the same $S^{m-1}$. There are m! ordered paths. The quadratic **coefficient** norm is uniform after dividing out $\|\xi\|_\infty^2$; evaluating at a growing canonical small-field radius introduces that actual radius squared and must not be suppressed.

**Native scale and physical factors.** These estimates concern original root labels at one unit fluctuation scale. If its mesh is $\ell$, distances in CEXP are $|x-y|/\ell$; converting the anchored source sum to physical volume contributes $\ell^{-4}$. No source label is silently moved to another mesh.

For a physical H source with its original common mesh a, each label carries $c_\beta^{-1}a^{-2}$. Therefore the anchored scalar absolute kernel in physical coordinates is bounded by
\[
a^{-4}(c_\beta^{-1}a^{-2})^m
\frac{d_G}{2}(m-1)!J^mS^{m-1}.
\tag{H-GKT-PHYS}
\]
Its engineering singularity is $a^{-(2m+4)}$, exactly
$\sum_i6-4(m-1)$ for m dimension-six insertions. At m=2 this is the w=8 kernel required in §4.7. If an inherited label carries the original mesh a while the current integration scale is $\ell_k$, its original multiplier remains $a^{-2}$; the coordinate volume and covariance range belong to $\ell_k$. Their conversion must be made explicitly.

For the action source $Y=S/N$, each microscopic quadratic vertex has the additional factor $(N\beta)^{-1}$ relative to the canonical action quadratic form. The corresponding anchored physical kernel has the form
$a^{-4}C^m(m-1)!\beta^{-m}$, with no further negative power of a per source. This is w=4 at every source order. To extend Theorem 3.6 from finite range to these kernels, use the tree weight: every anchor displacement from the root is at most $\mathcal T$, and $\mathcal T^5\le5!(\delta')^{-5}e^{\delta'\mathcal T}$. This supplies the fifth displacement moment. Taylor extraction through total degree four therefore uses at most fifth derivatives of each test. The product derivative and relative-coordinate factors cost only a fixed-degree polynomial in m, which can be absorbed into a fixed exponential $C^m$. Thus the **Gaussian action-sector contact subtraction** has a uniform all-order $C^5$ bound with factorial growth, provided the same source kernels and their retained background chains are used.

For the separate tightness rescaling $a^4O_H$, the scalar m-source contact bound becomes
$C^m(m-1)!a^{2m-4}$: at m=2 it can survive as a diagonal contact; at each fixed m≥3 it tends to zero. This concerns the first-step Gaussian contact sector, not the full interacting H limit.

**What is closed and what remains.** G-KT and CHAIN-KT verify the required first-Gaussian-step absolute connected locality and all-order source factorial control, using an actual constrained covariance with checked hypotheses and the literal H source stencil. The nonlinear source terms, source dependence of the covariance/readout, large-field R-operation, and higher-history transitions require T1's controlled nonlinear analytic remainder or connected polymer expansion. Bounds on those corrections must use the same anchored absolute norm; a small bound on a summed scalar logarithm alone is weaker. The cycle theorem does not assert that an arbitrary renormalized contact matrix has native locality.

### 4.15 Uniform complex source stability of the actual first-step Gaussian covariance

The previous cycle estimate extends to a full local source polydisc, with exponential locality retained. This is the Gaussian input needed for a nonlinear connected expansion.

For block matrices on physical bonds define the weighted Schur norm
\[
\|A\|_\alpha=
\max\left\{
\sup_x\sum_y e^{\alpha d(x,y)}\|A(x,y)\|_{\rm color},
\sup_y\sum_x e^{\alpha d(x,y)}\|A(x,y)\|_{\rm color}
\right\}.
\]
Triangle inequality for distance makes this norm submultiplicative, by direct summation. Let $0<\alpha<\delta$ and put
\[
B_\alpha=C_0S_{\delta-\alpha},\qquad
K_\alpha=z_s\kappa e^{2\alpha r_s},\qquad
z_s=\sup_x\#\{b:x\in D(b)\}\le19
\]
for the unaveraged original source. Fixed pointing enlargements change only the fixed stencil constant. CEXP and KTV give
$\|C_X\|_\alpha\le B_\alpha$ and
$\|K(t)\|_\alpha\le K_\alpha\|t\|_\infty$.

Choose a fixed r with $rB_\alpha K_\alpha\le\theta<1$. For **independent complex source values** $|t_b|\le r$, the actual constrained Gaussian covariance is
\[
C_t=(I-C_XK(t))^{-1}C_X
=C_X+C_XK(t)C_X+C_XK(t)C_XK(t)C_X+\cdots,
\tag{CSOURCE}
\]
and
\[
\|C_t\|_\alpha\le \frac{B_\alpha}{1-\theta}.
\tag{CSOURCE-BOUND}
\]
The inverse and series exist uniformly in the torus size because the weighted Schur norm is a Banach algebra. On the physical fluctuation range this is the inverse of the original constrained precision minus the quadratic source. The eliminated gauge/constraint directions remain eliminated.

Also $\|C_X^{1/2}K(t)C_X^{1/2}\|_{\rm op}\le B_\alpha K_\alpha r\le\theta$, by the ordinary Schur operator bound. Thus the real part of the canonical Gaussian precision is at least $(1-\theta)I$ on the physical fluctuation range, and the Gaussian integral is absolutely convergent throughout the polydisc. Consequently its partition function is nonzero and has a holomorphic logarithm on this fixed product polydisc. One can obtain its extensive bound either by integrating
$\partial_{t_b}W_0=\frac12\operatorname{Tr}(C_tK_b)$ along the radial segment or by G-KT. No determinant factor growing exponentially in the total number of variables is charged as an error.

The source responses are exact:
\[
\partial_{t_b}C_t=C_tK_bC_t,\qquad
\partial_{t_{b_1}}\cdots\partial_{t_{b_m}}C_t
=\sum_{\pi\in S_m}
C_tK_{b_{\pi(1)}}C_t\cdots K_{b_{\pi(m)}}C_t.
\tag{CRESPONSE}
\]
For the mean, $\xi_t=(I-C_XK(t))^{-1}\xi$ and
$\partial_{t_b}\xi_t=C_tK_b\xi_t$.
Thus the same open-chain and cycle arguments as §4.14 bound the first and higher source responses in an anchored, exponentially weighted norm. To obtain a strictly positive locality exponent in those bounds, use a smaller exponent $\alpha'<\alpha$ and replace the constants by the corresponding $S_{\alpha-\alpha'}$ and $B_\alpha/(1-\theta)$. This is a fixed loss of decay, paid once, not once per derivative.

This result applies to the original quadratic H source because its LOCAL-K/KTV properties were proved and its physical covariance was checked against the native constrained propagator. It is not a theorem about arbitrary bounded perturbation matrices. It also applies to the Gaussian action-density source with its actual factor $(N\beta)^{-1}$, giving a still larger allowed source radius.

**Boundary of the result.** The complex Gaussian domain does not by itself control the nonlinear Wilson vertices, the Jacobian, the moving readout, or the sharp cutoff correction. A comparison that divides an absolute global error by the full determinant would reintroduce an exponential volume loss. The remaining first-step nonlinear proof must estimate connected local corrections with C_t and its exact responses above. This section supplies the uniform complex covariance and locality needed to formulate that proof on the actual native variables.

### 4.16 A single-factorial anchored derivative theorem for analytic source polymers (P)

This removes an unnecessary factorial loss when passing from a genuine local analytic polymer expansion to all source orders.

Let X range over connected polymers on a fixed native block lattice. Suppose the source carriers have been included in X, so that:

1. A source label belongs to $S_X$ only if its anchor lies in X; at most $s_0$ labels lie in each block, hence $s_X=|S_X|\le s_0|X|$.
2. $F_X(J)$ depends only on $\{J_b:b\in S_X\}$, is holomorphic on the independent polydisc $|J_b|<r$, and obeys
   $\sup |F_X(J)|\le\varepsilon e^{-\kappa|X|}$.
   The bound may hold uniformly over a retained-field domain; the following conclusion then holds uniformly on that domain.
3. The anchored polymer count obeys
   $\sup_a\sum_{X:\,a\in S_X}e^{-\kappa_0|X|}\le K_0$.
4. The spatial tree length of any collection of source anchors in X is at most $t_0|X|$.

Fixed finite carrier enlargements only change $s_0,t_0,K_0$. They are not allowed to grow silently with the age of an inherited source.

Define the connected source coefficient
\[
K_m(b_1,\ldots,b_m)=
\sum_{X:\,\{b_1,\ldots,b_m\}\subset S_X}
\partial_{J_{b_1}}\cdots\partial_{J_{b_m}}F_X(0),
\]
where repetitions among the b's are permitted. Fix $\eta\ge0$ with
$\kappa>\kappa_0+\eta t_0$, and choose any $0<u<1$ such that
\[
s_0\log\frac1{1-u}\le\kappa-\kappa_0-\eta t_0.
\tag{POLY-SPARE}
\]
For example one can choose
$u=1-\exp[-(\kappa-\kappa_0-\eta t_0)/(2s_0)]$.
Then for every m≥1,
\[
\sup_{b_1}\sum_{b_2,\ldots,b_m}
e^{\eta\mathcal T(b_1,\ldots,b_m)}
|K_m(b_1,\ldots,b_m)|
\le
\varepsilon K_0\frac{u}{1-u}
(m-1)!(ru)^{-m}.
\tag{POLY-KT}
\]
Thus one fixed loss of polymer decay and one fixed reduction of the source radius give all-order anchored control with a **single factorial**. No source-order-dependent shrinking of the field domain is required by this combinatorial step.

**Proof with repeated labels retained.** Write
$F_X(J)=\sum_\alpha c_{X,\alpha}J^\alpha$.
Cauchy gives
$|c_{X,\alpha}|\le\varepsilon e^{-\kappa|X|}r^{-|\alpha|}$,
by taking radii increasing to r. Fix $a=b_1\in S_X$. An ordered tuple
$(b_2,\ldots,b_m)$ with total multiplicity vector $\alpha$ occurs
$(m-1)!/[(\alpha_a-1)!\prod_{b\ne a}\alpha_b!]$ times.
Its derivative is $\alpha!c_{X,\alpha}$. Therefore
\[
\sum_{b_2,\ldots,b_m\in S_X}
|\partial_a\partial_{b_2}\cdots\partial_{b_m}F_X(0)|
\le
(m-1)!\,\varepsilon e^{-\kappa|X|}r^{-m}
\sum_{\substack{|\alpha|=m\\\alpha_a\ge1}}\alpha_a.
\]
The last sum is exactly
$\binom{s_X+m-1}{m-1}$.
Indeed its generating function in m−1 is
$(1-z)^{-s_X-1}$: differentiate the a-factor in
$\prod_{b\in S_X}(1-z_b)^{-1}$ and then set all variables to z.
Because its coefficients are nonnegative,
\[
\binom{s_X+m-1}{m-1}
\le u^{-(m-1)}(1-u)^{-s_X-1}.
\]
Multiply by the tree weight, at most $e^{\eta t_0|X|}$, and use
$s_X\le s_0|X|$ and POLY-SPARE. The remaining anchored sum is bounded by K0. The factors outside that sum are
$\varepsilon(m-1)!r^{-m}u^{-(m-1)}(1-u)^{-1}$,
which give POLY-KT. This proves the claim.

The naive estimate "$s_X^{m-1}$ choices, each derivative at most $m!r^{-m}$" loses the cancellation between multiplicities and derivative factorials. Keeping the exact multiplicity count is what prevents a second factorial.

**Application to the actual first-step source carriers.** In T1's first-step construction with source-independent covariance and cutoff, each original source label enters only its finite determining carrier $Y_b$. A connected output activity X therefore depends only on labels whose determining carriers meet its assembled input cluster; after a fixed native-grid enlargement, their number is at most $s_0|X|$. This is the support property required above. One must use the expansion with these labels retained; a scalar bound after summing unrelated source labels would not suffice.

Accordingly, whenever the actual nonlinear first-step activities are proved holomorphic with the displayed independent polydisc and connected-polymer bound, POLY-KT supplies their all-order absolute source kernels, including the m=2 H contact needed by Theorem 3.6. This deduction has no additional all-order probabilistic hypothesis. It is conditional only on that precise source-local analytic polymer estimate, which T1 is proving for the specified first-step admitted domain. It does not assert that the same estimate has already been established through arbitrary old-source histories, whose source-anchor density per current block can grow.

A source-diagonal Taylor coefficient can still be a field-dependent, quasilocal retained operator. The source-kernel estimate alone does not identify it with a finite curvature-jet basis or prove that its retained-field support lies on one side of a reflection plane. Those are separate field-localization/extraction requirements in FULL-CONTACT and FULL-SPLIT. If a coefficient is decomposed into localized field polymers, terms reaching across a fixed physical reflection margin must be retained or bounded as a remainder, rather than silently included in a supposedly point-local subtraction.

For the action-density sector, combine POLY-KT with the fifth-displacement-moment argument of §4.14 to obtain all-order strictly local contact extraction with factorial growth and $C^5$ tests at this step. For physical H, restore each original $c_\beta^{-1}a^{-2}$ multiplier before using the w=8 two-source Taylor extraction. This preserves the source normalization and the distinction between connected ordinary covariance and removable diagonal contacts.

### 4.17 Operator-valued collision contacts and the nonlinear source algebra (P)

The scalar contact algebra of Theorem 3.1 is a necessary special case, not the whole composite-operator algebra. The computed background term in H-GCONTACT is an explicit example: a two-source contact is itself a retained quadratic field and cannot be represented solely by subtracting a field-independent quadratic functional.

Let J range over the chosen renormalized source labels. Introduce a formal local map into bare operator sources,
\[
\Psi_a(J)=Z_a^TJ+
\sum_{m\ge2}\frac1{m!}\Psi_{a,m}(J,\ldots,J),
\qquad \Psi_a(0)=0,
\tag{NONLINEAR-SOURCE}
\]
and set
\[
W_a^{\rm ren}[J]=W_a^{\rm bare}[\Psi_a(J)]-L_a[J].
\tag{FULL-CONTACT}
\]
Each multilinear coefficient $\Psi_{a,m}$ is an operator-valued local contact: its output source at x depends on a finite jet of all m input sources at x. At any fixed D and source order m, only the explicitly included finite list of output types is used. A convergent analytic map is not presumed when only a formal or finite-order construction has been proved.

**Partition formula.** If $\mathcal P_m$ denotes the partitions of $\{1,\ldots,m\}$, then
\[
D^mW_a^{\rm ren}[0](J_1,\ldots,J_m)=
\sum_{\pi\in\mathcal P_m}
D^{|\pi|}W_a^{\rm bare}[0]
\left(
\big(\Psi_{a,|B|}(J_i:i\in B)\big)_{B\in\pi}
\right)
-L_a^{(m)}[0](J_1,\ldots,J_m),
\tag{PARTITIONS}
\]
with $\Psi_{a,1}=Z_a^T$. To prove it, substitute the source Taylor series into the Taylor series for W. A term is selected by assigning the m labeled derivatives to the arguments of the outer derivative. Dividing by the Taylor factorials identifies exactly one contribution for each unordered partition, with no extra multiplicity. This proves the formula as a finite source-jet identity independently of convergence.

For example, the third derivative includes
\[
\kappa_2^{\rm bare}(\Psi_{a,2}(J_1,J_2),Z_a^TJ_3)
+\text{the other two pairings}.
\]
Such a term can be nonzero when the first two supports meet but the third is disjoint. It is a **partial-diagonal** contact. A scalar local $L_a^{(3)}$, supported on the total diagonal, cannot cancel or encode it. Thus the earlier empty-common-intersection vanishing statement applies to scalar total-diagonal contacts, not to the complete operator-valued contact algebra.

**Reflection positivity with full local contacts.** Suppose both maps respect reflection and conjugation and, for sources supported in opposite open halves with a margin,
\[
\Psi_a(\theta\overline{J_i}+J_j)
=\theta\overline{\Psi_a(J_i)}+\Psi_a(J_j),\qquad
L_a(\theta\overline{J_i}+J_j)
=\overline{L_a(J_i)}+L_a(J_j).
\tag{FULL-SPLIT}
\]
A genuinely local nonlinear map has the first property: mixed products of source jets on disjoint halves vanish at every point. The bare source matrix evaluated at $\Psi_a(J_i)$ is reflection positive. Multiplying by $e^{-\overline{L_a(J_i)}-L_a(J_j)}$ is again diagonal congruence. Differentiating by finite difference quotients proves reflection positivity of all finite source jets, with operator-valued contacts included. No ordinary random-variable interpretation of the contact-subtracted functional is required.

At the two-point reflected level with separated supports,
$\Psi_{a,2}(\theta\bar f,g)=0$ and $L_a^{(2)}(\theta\bar f,g)=0$.
Thus the reflected connected matrix still sees the actual linear renormalized operators, and cannot be made nondegenerate by a contact choice. For products within one half, the nonlinear maps alter the product algebra through the full partition formula; those terms cannot be omitted from an equations-of-motion quotient.

**Compatibility.** The correct all-D requirement is that the source maps and scalar functionals restrict exactly:
$\Psi_{a,D+1}(J,0)=\Psi_{a,D}(J)$ and
$L_{a,D+1}(J,0)=L_{a,D}(J)$,
as coefficientwise identities in a common graded space of output operators. PARTITIONS then proves compatibility of every joint connected distribution. When $\Psi_{a,1}$ is invertible on the retained finite type space, the map on finite source jets is triangular with invertible diagonal, so it gives an algebraic change of product prescriptions. This still does not imply a physical Gram lower bound.

**Why D alone does not close collision types.** A local source-action term
\[
\int dx\,\left(\prod_{i=1}^m\partial^{q_i}J_{\alpha_i}(x)\right)O_\gamma(x)
\]
has a coefficient of engineering dimension
\[
\sum_i d_{\alpha_i}-4(m-1)-\sum_iq_i-d_\gamma.
\]
Hence the dimensionally allowed divergent or logarithmic contacts can have
\[
d_\gamma\le\sum_i d_{\alpha_i}-4(m-1)-\sum_iq_i.
\tag{CONTACT-DEGREE}
\]
If all inserted dimensions are at most D>4, the upper envelope is
$m(D-4)+4$, which exceeds D at sufficiently high source order. This does not assert that every allowed coefficient is nonzero. It does show that a finite D source family is not automatically a closed finite **output** family for every collision order. One must either establish the necessary cancellations or construct the compatible graded family with these higher contact targets and quantified growth.

For D=4 the upper envelope remains four; this is why the action-sector scalar plus dimension-four operator contact algebra can be closed at all source orders once its actual coefficient bounds are proved. For H with D=6, order two already permits dimension-eight targets. The Gaussian H-GCONTACT occupies only its scalar and quadratic portions; it is not a proof that all nonlinear higher-dimensional contact rows vanish.

This section strengthens the target algebra and the interface statement: all joint counterterms in I-3 must be supplied through $\Psi_a$ and $L_a$, or an equivalent explicitly stated operator-product prescription. A formula containing only a linear mixing matrix and scalar L is adequate only for the subcase where all operator-valued contacts have already been shown absent or separately retained.

### 4.18 A nonflat compact-block innovation bound paid by actual background energy (P)

A fixed pointwise canonical-background radius is unnecessary for this finite-order estimate. The large background contribution is retained as an energy term and then averaged under the actual Wilson law.

**Fixed block.** Let C be a fixed contractible Wilson block with identity boundary as in §4.10 at its reference point. Allow boundary links $e^{b}$ with real $\|b\|<\delta_C$, in a fixed gauge chart; $\delta_C$ is a small physical radius independent of beta. Use the full compact conditional integral over its interior links. Mark only roots whose complete original plaquette-force stencil is in C, and put
$H_f=h_f/\beta$ with the original force definition. Let $U_*(b)$ be the constrained minimizer of $S_C$ and $S_*(b)=S_C(U_*(b))$.

There exist $C_C,\beta_C,\delta_C>0$, depending on this fixed geometry and group, such that for every real mark f and $\beta\ge\beta_C$,
\[
\operatorname{Var}_{\beta,C,b}(h_f)
\le C_C M_f\,[1+\beta S_*(b)]
\qquad(\|b\|<\delta_C).
\tag{ENERGY-INNOVATION}
\]
This is an actual compact-law conditional variance. It includes the compact complement of the local saddle.

**Fixed-cell analytic comparison used in the proof.** For $\|f\|_\infty\le1$, consider
$\Phi(A;b,\eta)=S_C(A;b)-\eta H_f(A;b)$.
At b=η=0, the tree-gauge Hessian is positive by the path argument of §4.10. Finite-dimensional analytic implicit inversion therefore gives a holomorphic critical point $A_*(b,\eta)$ for sufficiently small b and η, with uniformly invertible Hessian. The local critical scalar is $\Phi_*(b,\eta)$.

For completeness, the compact comparison can be justified as follows. Outside a fixed coordinate cube around the identity, $S_C$ has a positive gap at b=0; continuity preserves half this gap for small real b. The pointwise force inequality gives $|H_f|\le16\tau S_C$, so sufficiently small complex η preserves a positive real-action gap there. The critical scalar is $O(|b|^2)$, hence shrinking $\delta_C$ makes that compact tail exponentially small relative to $e^{-\beta\Phi_*}$.

Inside the chart, translate the real contour cube to the complex critical point. The phase is holomorphic and the connecting side faces stay at a positive real-action distance from the saddle: this follows from the positive reference Hessian, the fixed cube radius, and $|A_*(b,\eta)|$ sufficiently smaller than that radius. Their integrals are exponentially small relative to the saddle term. On the translated cube, scale $A-A_*=\beta^{-1/2}X$. The Gaussian Hessian is uniformly accretive; its cubic Taylor term integrates to zero on the symmetric cube. The quartic remainder and the square of the cubic are bounded by integrable Gaussian polynomials times $\beta^{-1}$. The analytic Haar/Jacobian amplitude is treated in the same way. All dimensions are fixed here. This proves
\[
Z_{\beta,C,b}(\eta)
=e^{-\beta\Phi_*(b,\eta)}\beta^{-d_C/2}
a_C(b,\eta)\exp R_{\beta,C}(b,\eta),
\quad
|R_{\beta,C}|\le C_C/\beta,
\tag{CELL-LAP}
\]
uniformly on a fixed complex η-disc, with $a_C$ nonzero and holomorphic. The argument is the fixed-block saddle mechanism also detailed in T1 Theorem 7.15. The domain and constants may depend on C; no growing-block conclusion is hidden here.

**Compute the critical source response.** At η=0 write $H_*=\nabla_A^2S_C(A_*(b,0);b)$. It satisfies $H_*\ge\lambda_C I$ for small real b. Differentiating the critical-point equation gives
\[
\partial_\eta A_*|_0=H_*^{-1}\nabla_AH_f(A_*(b,0);b),
\]
\[
\partial_\eta^2\Phi_*|_0
=-\nabla_AH_f^T H_*^{-1}\nabla_AH_f.
\tag{CRITICAL-RESPONSE}
\]
The finite plaquette-force stencil and its bounded derivatives imply
\[
\|\nabla_AH_f(U_*(b))\|^2
\le C_C M_f S_*(b).
\tag{FORCE-ENERGY}
\]
To see this, each derivative of a force square retains one first-force factor; the other differentiated factors are bounded. The first-force square is bounded by a fixed sum of plaquette actions. Sum over the finite block, use Cauchy–Schwarz in the marks, and use the bounded chart/gauge derivative matrices. This proves FORCE-ENERGY in the actual group-coordinate convention.

Differentiating the logarithm of CELL-LAP twice gives the exact conditional variance
\[
\operatorname{Var}(h_f)
=\beta\,\nabla_AH_f^TH_*^{-1}\nabla_AH_f
+\partial_\eta^2\log a_C|_0
+\partial_\eta^2R_{\beta,C}|_0.
\]
Uniform holomorphy on the fixed source disc bounds the last two terms by
$C_C\|f\|_\infty^2$ (the remainder is in fact $O(\beta^{-1})$). FORCE-ENERGY and $\|f\|_\infty^2\le M_f$ prove ENERGY-INNOVATION. The exact critical scalar has not been reset or bounded by a worst-case canonical cutoff.

**The ordinary source has the same innovation bound.** At η=0 the positive real Laplace comparison also gives
$\beta\,\mathbb E_{\beta,C,b}(S_C-S_*)\le C_C$:
inside the saddle chart, uniform quadratic coercivity and the change of variables
$A-A_*=\beta^{-1/2}X$ bound the energy numerator by a fixed Gaussian second moment times the partition scale; the compact complement is exponentially smaller. Hence
$\beta\mathbb E S_C\le\beta S_*+C_C$.
For the marked interior roots, Haar integration by parts is legitimate with the boundary fixed, and the action derivatives are exactly those of the full original stencil. Apply H-COV and H-LOCAL to this conditional law. Its Ward contact row has Schur norm at most $C_C[1+\beta S_*(b)]$. Therefore
\[
\operatorname{Var}_{\beta,C,b}(r_f)
\le C_C M_f[1+\beta S_*(b)]
\tag{ORDINARY-INNOVATION}
\]
after enlarging the constant. This controls the actual ordinary conditional covariance; it does not replace it by a one-site spectral gap or discard its conditional mean.

**Annealing under the original Wilson measure.** Partition a periodic lattice into congruent fixed-size cells with retained collars thick enough that no plaquette touches two distinct interior regions. Conditional on the collar links, those interiors are independent. Let $G_C$ be the collar-measurable event that the boundary of cell C lies in the admitted gauge chart. Let $h_{f,C}$ use only roots with full stencils in that cell; the remaining roots and bad cells are kept as separate source terms.

The minimizer obeys the deterministic fiber inequality
$S_*(B_C)\le S_C(U_C,B_C)$.
The cell actions have bounded overlap, so
\[
\sum_C S_*(B_C)\le C_{\rm ov}S(U).
\]
Translation invariance of the congruent cell grid and FIRST consequently give
\[
\beta\,\mathbb E S_*(B_C)\le C_C
\]
for each fixed cell type, uniformly under REG. This uses only the actual Wilson law and a minimization inequality; it is not a Gaussian comparison. Independence of the conditional interiors and ENERGY-INNOVATION now yield
\[
\mathbb E\operatorname{Var}\!\left(
\sum_C G_C h_{f,C}\,\middle|\,\text{collars}\right)
\le C_C\sum_C M_{f,C}.
\tag{ANNEALED-CELL}
\]
ORDINARY-INNOVATION gives the same ANNEALED-CELL bound with every h replaced by the ordinary source r. Thus the admitted nonflat compact-block innovation has an extensive bound without replacing the background radius by its worst-case logarithmic value.

The admitted boundary event can be made gauge invariant and is not confined to boundary links accidentally close to I. Choose a fixed spanning tree on the boundary of the four-dimensional rectangular cell, gauge its links to I, and use the remaining boundary loop variables as coordinates. Every such loop has a filling by finitely many boundary plaquettes; the boundary cell complex is simply connected. The product inequality for unitary matrices then gives
$\max_e\|U_e^{\rm gauge}-I\|\le C_C(\sum_{p\subset\partial C}s_p)^{1/2}$.
Hence the condition $\sum_{p\subset\partial C}s_p\le c_C\delta_C^2$ implies the admitted chart condition. FIRST and Markov's inequality give the actual bound
\[
\mathbb P(G_C^c)\le C_C/(\beta\delta_C^2).
\]
Thus fixed-cell admitted boundaries have probability tending to one as beta grows. This probability estimate is not a bound on their connected source contribution and is not used to discard bad cells.

The remaining terms are explicit: source roots whose stencils cross the retained collars, bad-boundary cells, and the ordinary variance of the conditional mean. ANNEALED-CELL does not bound or delete any of them. Refining the grid or taking shifted coverings does not by itself remove the last term. At this stage these are unresolved. Sections 4.22–4.23 subsequently remove the bad-boundary and single-grid collar restrictions for fixed-cell innovations, leaving the actual retained conditional-mean covariance to be controlled by complete row/history transport.

### 4.19 Higher-degree first-step Gaussian composites without an analytic-source assumption (P with CEXP)

The quadratic determinant is not needed to control a finite family of higher-degree composite insertions. Their source exponentials need not exist on a fixed positive real disc, but all fixed-order cumulants can still be bounded.

Let $X$ be the actual first-step constrained Gaussian fluctuation with covariance CEXP. For each root b and type $\alpha$ through a fixed cutoff D, let $P_{\alpha,b}(X)$ be a polynomial of canonical degree at most $q_D$, depending only on field coordinates within distance $R_D$ of b. Suppose the sum of absolute monomial coefficients, including color and stencil labels, is at most $B_D$. Fixed-order lattice differences and linearized curvature representatives fit this form with explicitly finite $q_D,R_D,B_D$; physical factors in a and g are kept outside this canonical estimate.

For every $0\le\eta<\delta$ there is a constant $C_D$, depending only on
$q_D,R_D,B_D,C_0,\delta-\eta$ and the fixed lattice/group conventions, such that
\[
\sup_{b_1}\sum_{b_2,\ldots,b_m}
e^{\eta\mathcal T(b_1,\ldots,b_m)}
\left|
\kappa_m(P_{\alpha_1,b_1},\ldots,P_{\alpha_m,b_m})
\right|
\le C_D^m(m!)^{p_D},
\qquad p_D=\max(1,q_D/2).
\tag{HIGH-GKT}
\]
The bound is uniform in the cutoff and number of blocks at this one Gaussian step. No exponential moment of a polynomial of degree greater than two is assumed.

**Proof.** Expand the polynomial insertions into monomials. For a fixed choice of monomials, Gaussian Wick expansion expresses the joint moment as a sum over pairings of all field legs. Associate a vertex to each insertion and an edge to each pair; a pair within one insertion is a loop. The moment–cumulant partition identity cancels exactly the pairings whose insertion graph is disconnected. This can be verified by grouping any pairing according to its connected components: the usual set-partition expansion of moments is then precisely the decomposition into connected pairings. This is a finite-order combinatorial identity, not an analytic logarithm argument.

Each surviving pairing has at most $Q=q_Dm$ legs and at most Q/2 covariance factors. Its connected graph contains a spanning tree on the m insertion vertices. Choose one such tree by a fixed deterministic ordering of the already labeled pairing; no additional sum over trees is introduced. CEXP and the stencil bound give a factor at most
$C_1^{Q/2}$, $C_1=\max(1,C_0e^{2\delta R_D})$,
times $e^{-\delta d(b_i,b_j)}$ for each selected tree edge. Discarding the other decay factors only enlarges the bound. The desired tree weight is paid from those same edges, since the minimum anchor-tree length is no greater than their total length. Summing the remaining anchors along that fixed tree gives at most $S_{\delta-\eta}^{m-1}$.

The total number of pairings is at most $Q^{Q/2}$, with zero contribution when the actual number of legs is odd. The coefficient sum is at most $B_D^m$. Since
\[
(q_Dm)^{q_Dm/2}
\le (e q_D)^{q_Dm/2}(m!)^{q_D/2},
\]
these factors prove HIGH-GKT after enlarging $C_D$. Constant monomials give no cumulant for m≥2, and the m=1 constant contribution is absorbed into $C_D$. If $q_D=0$ the claim is immediate. This proves the higher-degree bound without adding a tree-counting factorial.

**A compatible Gaussian mixing prescription.** On the finite polynomial algebra define Wick ordering by
\[
\mathcal W_{C_X}P
=\exp\!\left(-\frac12\sum_{u,v}C_X(u,v)
\frac{\partial^2}{\partial X_u\partial X_v}\right)P.
\tag{WICK-MIX}
\]
The series terminates at fixed polynomial degree. This is a triangular, invertible linear map, with inverse obtained by reversing the sign. It subtracts exactly the self-contractions, including identity and lower-degree rows. Using the same covariance and type ordering for every D makes the prescription compatible as D increases. The fixed local stencil and CEXP bound every coefficient of this finite map in terms of D and the stated canonical constants. Restoring engineering dimensions supplies the corresponding original powers of a and g; it does not turn this Gaussian map into the interacting mixing matrix.

Wick ordering commutes with every linear symmetry preserving the covariance and the chosen stencil prescription. It does not by itself prove restoration of continuum rotations or identify nonlinear Yang–Mills equations of motion. The connected-pairing proof works equally for Wick-ordered polynomials, with loops removed.

**Why the factorial exponent should be allowed to depend on the family.** Let Z be a standard real Gaussian and $Y=Z^{2r}$, r>1. Every moment exists, but $\mathbb E e^{tY}=\infty$ for every t>0: the positive degree-2r exponent dominates the Gaussian tail. Moreover an all-order cumulant bound
$|\kappa_m(Y)|\le C^m(m!)^p$ with p≥1 and C enlarged to at least one would imply
\[
\mathbb E Y^m
\le(2C)^m(m!)^p.
\]
Indeed, in the moment–cumulant partition formula,
$\prod_{B\in\pi}(|B|!)^p \le(m!)^{p-1}\prod_{B\in\pi}|B|!$,
and
$\sum_\pi\prod_{B\in\pi}|B|! =m!\sum_{k=1}^m\binom{m-1}{k-1}/k! \le m!2^{m-1}$.
But $\mathbb E Y^m=(2rm-1)!!$ has factorial order $(m!)^r$, as follows directly from the factorial formula and Stirling bounds. Hence p<r is impossible. This is a quantitative diagnostic for higher-degree source methods: the single-factorial quadratic/action result should not be imposed on arbitrary high-degree composites.

HIGH-GKT therefore supplies the appropriate finite-family factorial estimate at the first Gaussian step, while AN-D remains an optional stronger sufficient hypothesis only where an actual analytic source functional exists. The outstanding interacting problem is to transport the higher polynomial source jets, their operator-valued collision rows, and their original a/g grades through the nonlinear and large-field histories with controlled growth in D and source order.

### 4.20 Actual compact-cell higher-composite cumulants and Gaussian convergence (P)

The factorial hierarchy in §4.19 also has an actual compact-law counterpart. This result uses no exponential source for an irrelevant polynomial.

Fix the contractible Dirichlet cell of §4.10 with identity boundary, gauge-fix a rooted interior forest, and let $d_C$ be the number of remaining real coordinates. Write $S_C$ for its Wilson action and $\mu_{\beta,C}$ for its full compact Wilson probability law. Constants below depend on this fixed cell. The action has the unique zero I and a positive Hessian in these gauge-fixed coordinates, as proved in CELL-G. Consequently there are constants $0<c_C<C_C$ such that
\[
c_C\beta^{-d_C/2}\le Z_{\beta,C}
\le C_C\beta^{-d_C/2}\qquad(\beta\ge1).
\tag{CELL-PARTITION}
\]
The lower bound follows by integrating a ball of radius $\beta^{-1/2}$ in a coordinate chart at I. For the upper bound, the chart has $S_C(A)\ge c|A|^2$ and bounded Haar density; its integral is at most a constant times $\beta^{-d_C/2}$. The compact complement has a fixed action gap and exponentially small integral. Enlarging the constants covers the bounded beta interval. Thus
\[
\mathbb E_{\beta,C}\exp(\beta S_C/2)
=\frac{Z_{\beta/2,C}}{Z_{\beta,C}}\le K_C
\qquad(\beta\ge1),
\tag{CELL-EXP}
\]
where the compact interval $1\le\beta\le2$ is included separately.

Let $\Phi_1,\ldots,\Phi_s$ be finitely many smooth, bounded compact lattice components that vanish at I and are analytic near I. Examples are the color components of transported $C_N(U_p)$, their fixed lattice covariant differences, and Wilson force components in the same fixed tree gauge. On the coordinate chart $|\Phi_j|\le C|A|$; on the complement the action gap gives the same global estimate with another constant:
\[
|\Phi_j(U)|\le C_C S_C(U)^{1/2}.
\tag{COMP-ENERGY}
\]
For each label $\alpha,b$, let $P_{\alpha,b,\beta}$ be a polynomial of total degree at most $q_D$ in the canonical components $\sqrt\beta\,\Phi_j(U)$, with coefficient sum bounded by $B_D$. Explicit original powers of a and g are kept outside this statement. Compact representatives constructed from finitely many curvature components and fixed-order differences fall in this class. COMP-ENERGY implies
\[
|P_{\alpha,b,\beta}(U)|
\le B'_D(1+\beta S_C(U))^{q_D/2}.
\tag{POLY-ENERGY}
\]
The constants do not depend on beta or on the number of insertions.

Set $p_D=\max(1,q_D/2)$. For every m≥1, arbitrary permitted labels, and all beta≥1,
\[
\left|\kappa_m^{\mu_{\beta,C}}
(P_{\alpha_1,b_1,\beta},\ldots,
 P_{\alpha_m,b_m,\beta})\right|
\le A_{C,D}^{\,m}(m!)^{p_D}.
\tag{COMPACT-HIGH}
\]
This is a bound for cumulants of actual compact Wilson random variables.

**Proof.** CELL-EXP and
$\sup_{x\ge0}(1+x)^u e^{-x/2}\le e^{1/2}\max(1,(2u/e)^u)$
show that every product of k insertions satisfies
\[
\mathbb E_{\beta,C}\prod_{i=1}^k|P_{\alpha_i,b_i,\beta}|
\le A_0^k(k!)^{p_D},
\]
after enlarging $A_0$ to absorb the fixed $K_C$ and using $k!\ge(k/e)^k$. For $q_D=0$ the bound follows directly from bounded constants.

In the moment–cumulant formula, a partition $\pi$ with k blocks has coefficient $(k-1)!$. For p≥1,
\[
\prod_{B\in\pi}(|B|!)^p
\le(m!)^{p-1}\prod_{B\in\pi}|B|!,
\]
and counting partitions by ordered positive block sizes gives
\[
\begin{split}
\sum_{\pi}(|\pi|-1)!\prod_{B\in\pi}|B|!
&=m!\sum_{k=1}^m\frac1k\binom{m-1}{k-1}\\
&\le m!2^{m-1}.
\end{split}
\]
Multiplying the moment bounds over the blocks, and applying these two identities, proves COMPACT-HIGH with $A_{C,D}=2A_0$. No analyticity of $\mathbb E\exp(tP)$ was used. At finite beta the canonical variables are bounded and their exponentials exist, but their positive-source bounds need not remain uniform as beta tends to infinity.

**Fixed-order identification of the limiting cumulants.** In the chart set $A=\beta^{-1/2}X$. Then
$\beta S_C(A)=\frac12\langle X,H_CX\rangle+O_C(\beta^{-1/2}|X|^3)$
and
$\sqrt\beta\,\Phi_j(A)=D\Phi_j(0)X+O_C(\beta^{-1/2}|X|^2)$.
The Haar density has a bounded smooth expansion as well. Let $P^0_{\alpha,b}(X)$ denote the polynomial obtained by replacing each canonical component by $D\Phi_j(0)X$, and let $\gamma_C$ be the Gaussian with covariance $H_C^{-1}$. For every fixed m and choice of labels,
\[
\kappa_m^{\mu_{\beta,C}}(P_{1,\beta},\ldots,P_{m,\beta})
=
\kappa_m^{\gamma_C}(P^0_1,\ldots,P^0_m)
+O_{C,D,m}(\beta^{-1/2}).
\tag{COMPACT-HIGH-LIMIT}
\]
To check the error, shrink the physical chart so that both its exact action and its quadratic part are bounded below by $c|X|^2$. The inequality
$|e^{-u}-e^{-v}|\le|u-v|e^{-\min(u,v)}$
bounds the density difference by
$C\beta^{-1/2}(1+|X|^3)e^{-c|X|^2}$.
Taylor expansion of each polynomial factor costs only a further fixed polynomial in X. The omitted Gaussian chart tail and the actual compact complement are exponentially small times fixed powers of beta. These bounds prove the claimed error for each fixed joint moment, including the partition normalization. The finite moment–cumulant formula proves COMPACT-HIGH-LIMIT. This is a full compact integral comparison, not a substitution of its Gaussian tangent law.

For a fixed cell the finitely many roots can also be summed with any fixed anchor-tree weight; its number and diameter are absorbed into $A_{C,D}^m$. That observation supplies no uniform large-cell estimate: CELL-PARTITION, the chart coercivity, the action gap and the support counts depend on the cell. The full physical operator problem still requires the actual RG to transport these finite-family grades, mixing and cumulants across growing scales and all retained histories.

### 4.21 Coupling differentiation with a frozen canonical cutoff (P)

The exact identity ACTUAL-ACTION-ROW requires the physical integration measure and fiber to remain fixed as the coupling varies. Freezing a selector in rescaled fluctuation coordinates is a different operation. Its extra term can be computed exactly.

Fix the retained physical background b and a coupling-independent local constraint chart $v\mapsto\Psi_b(v)$, with positive smooth density $J_b(v)\,dv$ for the original constrained measure. Let $S_b(v)=S(\Psi_b(v))$, let $g(\beta)=(N\beta)^{-1/2}$, and fix the canonical box $\Omega_p=[-p,p]^d$. Set
\[
I_\beta(b)=\int_{\Omega_p}
J_b(gB)e^{-\beta S_b(gB)}\,dB,\qquad
Z_\beta^{\rm mov}(b)=g^d I_\beta(b).
\]
This is the original physical integral over the moving chart domain $g(\beta)\Omega_p$. Its probability law is normalized by $I_\beta$. Define the boundary flux
\[
F_\beta(b)=\int_{\partial\Omega_p}
(B\cdot n)J_b(gB)e^{-\beta S_b(gB)}\,d\sigma(B),
\qquad T_\beta(b)=F_\beta(b)/I_\beta(b).
\]
Then
\[
-\partial_\beta\log Z_\beta^{\rm mov}(b)
=\mathbb E_{\beta,b}^{\rm mov}S
+\frac{T_\beta(b)}{2\beta}.
\tag{CUTOFF-FLUX}
\]
In particular the flux is nonnegative at real data. It is generally nonzero even for an exactly Gaussian action.

**Proof.** Put $f_\beta(v)=J_b(v)e^{-\beta S_b(v)}$. Differentiating the scaled integral gives
\[
\partial_\beta Z_\beta^{\rm mov}
=-g^d\int_{\Omega_p}S_b(gB)f_\beta(gB)\,dB
+\frac{g'}g\,g^d\int_{\Omega_p}
\operatorname{div}_B[B f_\beta(gB)]\,dB.
\]
Use $g'/g=-1/(2\beta)$ and the divergence theorem. Dividing by $Z_\beta^{\rm mov}$ proves CUTOFF-FLUX. The argument includes every chart Jacobian through $J_b$ and does not presume a flat background.

For a smooth compactly supported selector $\chi(B)$ the same calculation replaces the boundary integral by
\[
F_{\beta,\chi}
=-\int_{\mathbb R^d}
(B\cdot\nabla\chi(B))J_b(gB)e^{-\beta S_b(gB)}\,dB.
\]
A radial nonincreasing selector again gives a nonnegative real flux. Neither expression vanishes merely because the selector has been declared coupling independent in B.

If the normalized moving-domain integral has LAP-ROW, the actual insertion is consequently
\[
O_{Y,\beta}^{\rm mov}(b)
=\frac{S_*(b)}N+\frac d{2N\beta}
-\frac{\partial_\beta\mathcal E(\beta,b)}N
-\frac{T_\beta(b)}{2N\beta}.
\tag{MOVING-ACTION-ROW}
\]
The physical fixed-domain source covariance likewise cannot be identified with a second derivative of the moving-domain logarithm without differentiating its selector response. One may instead use the exact fixed-domain source partition function; this automatically includes the correct response and avoids interpreting the moving family as the source family.

**The defect is small in a genuinely fixed cell, but that fact needs proof.** Suppose $S_b$ has its minimum at v=0, and in a fixed physical chart
\[
c|v|^2\le S_b(v)-S_*(b)\le C|v|^2,\qquad
0<c_J\le J_b(v)\le C_J .
\]
These constants can be uniform on a fixed admitted real boundary neighborhood by the compact-cell saddle construction, after translating to its physical minimizer. If $gp$ stays in that chart and p≥1, the denominator after extracting $e^{-\beta S_*}$ is bounded below by integrating a fixed canonical ball. On each face at least one canonical coordinate has absolute value p. Gaussian integration of the other coordinates therefore gives, for fixed d,
\[
0\le T_\beta(b)\le C_{C}\,p\,e^{-c_Cp^2}.
\tag{FIXED-CELL-FLUX}
\]
To verify this bound, $\beta g^2=1/N$ converts coercivity into $c'|B|^2$; $B\cdot n=p$ on every face, and the sum of the $2d$ remaining Gaussian integrals is a fixed constant. No ratio of growing-dimensional determinant factors is suppressed.

Thus the first fixed-cell action row differs from the coupling derivative by at most
$C_C\beta^{-1}p e^{-c_Cp^2}$.
A logarithmically growing canonical cutoff makes this smaller than every fixed inverse power of beta. This proves the real fixed-cell statement only. To bound retained-background derivatives or to obtain a uniform rooted estimate over many native blocks, one must establish the analogous tagged complex face/selector estimate on a common background domain. Real smallness alone does not supply those derivatives.

The native first-step scalar bound in T1 §7.27 is therefore useful, but its conversion to an actual action-source row must specify either a fixed physical fiber/domain or the controlled flux in MOVING-ACTION-ROW. This is an explicit measure-identification requirement in LAP-ROW, not an extra term that can be removed by renaming the cutoff frozen.

### 4.22 Full-torus marked energy moments and local composite cumulants (P with the checked chessboard inequality)

The fixed-cell constants in §4.20 can be avoided for local composite moments by using the original Wilson reflection positivity. This does not give decay or absolute summability of connected correlations.

In addition to REG, fix an integer block side $\ell\ge2$ with $\ell\mid n$ and $n/\ell$ even. For example $\ell=2$ works when $4\mid n$, a condition preserved under multiplication by the program's odd blocking factor. Cover the torus by closed cubes of side $\ell$ whose corner coordinates are multiples of $\ell$. Shared boundary links are allowed. Let $M=(n/\ell)^4$ be the number of cubes.

**Reflection positivity and the exact imported inequality.** For every coordinate reflection through a pair of lattice-site hyperplanes, condition on all links lying in those hyperplanes. No plaquette contains interior links from both complementary halves. The conditional interiors are independent reflected copies; the remaining boundary action is a positive common weight. Hence
$\mathbb E(\overline{\theta F}F)\ge0$
for every bounded function of one closed half. This proves the needed site-reflection positivity directly for the compact Wilson law, as in Theorem 3.5.

The general chessboard inequality is used in the following checked form: for functions $F_j\ge0$ supported on distinct closed cubes,
\[
\mathbb E\prod_jF_j
\le\prod_j\left[
\mathbb E\prod_{C}\theta_C(F_j^{\,0})
\right]^{1/M}.
\tag{CHESS}
\]
Here $F_j^{\,0}$ is the inverse-reflected copy in a reference cube and $\theta_C$ disseminates it to cube C. This is Theorem 4.8, (4.31), in [Biskup, *Reflection Positivity and Phase Transitions in Lattice Spin Models*, §4.3, pp.42–44](https://www.math.ucla.edu/~biskup/PDFs/papers/Prague-School.pdf). Its proof uses only reflection-positive Cauchy–Schwarz and an even factor torus; it permits shared block faces. Thus it applies to these link-supported block algebras after the reflection-positivity check above. No independent-spin law is imported.

**Marked-set theorem.** There are constants $t_*>0$ and $K_{\sigma,\ell}<\infty$, independent of n, beta and the marked set, such that for every set $\mathcal P$ of distinct plaquettes,
\[
\mathbb E_{\beta,n}
\exp\!\left(t_*\beta\sum_{p\in\mathcal P}s_p\right)
\le \exp(K_{\sigma,\ell}|\mathcal P|).
\tag{MARKED-EXP}
\]
One can take $t_*=1/32$ using the conservative overlap constant 16.

**Proof.** Assign each marked plaquette to one closed cube containing it. Every unit plaquette has such a containing cube, including those on block boundaries. For each occupied cube C define
$F_C=\exp(t_*\beta\sum_{p\text{ assigned to }C}s_p)$.
Reflection preserves the plaquette action, including when it reverses orientation. Disseminating any one F_C gives at most one copy of a given local plaquette pattern per closed cube. A global plaquette belongs to at most 16 closed cubes in dimension four. Therefore, pointwise,
\[
\prod_{C'}\theta_{C'}(F_C^{\,0})
\le \exp(16t_*\beta S)
\le\exp(\beta S/2).
\]
The full-law partition comparison of §4.11 gives
$\log\mathbb E e^{\beta S/2}\le A_\sigma n^4$,
with a harmless enlargement for $1\le\beta\le2$. Thus every factor on the right of CHESS is at most
$\exp(A_\sigma n^4/M)=\exp(A_\sigma\ell^4)$.
There are at most $|\mathcal P|$ occupied cubes. This proves MARKED-EXP with $K_{\sigma,\ell}=A_\sigma\ell^4$. All compact field sectors, and every plaquette not in the marked set, remain in the normalized measure.

The same argument gives the explicit simultaneous tail bound
\[
\mathbb P(\beta s_p\ge u\text{ for every }p\in\mathcal P)
\le \exp[-(t_*u-K_{\sigma,\ell})|\mathcal P|].
\tag{MARKED-TAIL}
\]
This estimate concerns specified original plaquettes. It is not a bound for arbitrary connected source activities or for the cost of all possible large-field histories.

**Higher local composite moments on the actual torus.** Consider a fixed family of compact lattice components built from transported $C_N(U_p)$, fixed-order covariant differences, or Wilson force components. For each root b all requested stencils are contained in a set $Y_b$ of at most $s_D$ plaquettes, uniformly in n. Unitary transport preserves matrix norms. The compact-group inequality
$\|C_N(U_p)\|\le C_N\sqrt{s_p}$
and the finite sums in each difference or force imply
\[
|\Phi_{j,b}(U)|\le C_D
\left(\sum_{p\in Y_b}s_p\right)^{1/2}.
\]
For the force bound use the sum of the plaquette forces and the pointwise force-square estimate proved in §4.11. These are global compact-field inequalities; no logarithm chart or gauge-near-identity event is needed.

Let $P_{\alpha,b,\beta}$ be a polynomial of degree at most $q_D$ in these components multiplied by $\sqrt\beta$, with a uniformly bounded coefficient sum. Then
\[
|P_{\alpha,b,\beta}|
\le B_D(1+\beta S_{Y_b})^{q_D/2},
\qquad S_Y=\sum_{p\in Y}s_p .
\]
MARKED-EXP bounds $\mathbb E e^{t_*\beta S_{Y_b}}$ by
$\exp(K_{\sigma,\ell}s_D)$ uniformly. The elementary exponential-to-moment bound used in §4.20 now gives
\[
\mathbb E|P_{\alpha,b,\beta}|^k
\le C_D^k(k!)^{p_D},
\qquad p_D=\max(1,q_D/2),
\tag{TORUS-LOCAL-MOM}
\]
with constants depending on $\sigma,\ell,D$ and the fixed group/stencil conventions. For arbitrary locations, including repeated ones, Hölder's inequality gives
\[
\mathbb E\prod_{i=1}^k|P_{\alpha_i,b_i,\beta}|
\le\prod_{i=1}^k
\bigl(\mathbb E|P_{\alpha_i,b_i,\beta}|^k\bigr)^{1/k}
\le C_D^k(k!)^{p_D}.
\]
The exact partition counting in §4.20 therefore proves
\[
\sup_{b_1,\ldots,b_m}
\left|\kappa_m(P_{\alpha_1,b_1,\beta},\ldots,
P_{\alpha_m,b_m,\beta})\right|
\le (2C_D)^m(m!)^{p_D}
\tag{TORUS-LOCAL-CUM}
\]
for the full compact Wilson torus, uniformly under REG and the displayed tiling condition.

TORUS-LOCAL-CUM has a supremum over source locations, not an anchored sum over the other locations. Summing this bound alone would introduce powers of the lattice volume. Restoring the original a/g grades also leaves the ultraviolet contact divergences in place. Thus this supplies a genuine uniform local moment/cumulant hierarchy for the bare canonically scaled compact composites, while all-history connected locality, operator mixing, diagonal subtraction and the continuum smeared bounds remain separate problems. It does not prove the renormalized all-order clause of I-3 or full-torus complex zero-freeness.

### 4.23 Full-sector fixed-cell innovations and the remaining conditional means (P under §4.22's tiling condition)

MARKED-EXP removes the good-boundary restriction from the fixed-cell innovation bound. It does not require evaluating the constrained saddle at an inadmissible boundary.

The ordinary source has the global pointwise bound
\[
|r_b|\le C\left(1+\beta\sum_{p\in Y_b}s_p\right).
\tag{ORDINARY-POINT}
\]
Indeed $D_b$ is bounded by a fixed sum of plaquette force squares, hence by $C\sum_{Y_b}s_p$. The trace of the Wilson plaquette Hessian contributing to $\ell_b$ is bounded on the compact group, and only finitely many plaquettes enter. The same bound holds for $h_b$, which has no independent bounded Hessian term. TORUS-LOCAL-MOM yields
\[
\sup_{b,n,\beta}\mathbb E(|r_b|^2+|h_b|^2)\le C
\]
under the stated hypotheses.

Take disjoint fixed-size cell interiors separated by retained collars as in §4.18, and let $\mathcal B$ denote their collar-link sigma algebra. For real marks f, let
$A_C=\sum_{b\in C_{\rm int}}f_b r_b$,
where each requested complete stencil lies in the interior and its adjacent retained collar. These stencils must involve no other cell's interior. Conditional on $\mathcal B$, different interiors are independent. If each cell contains at most $v_C$ source roots, then
\[
\begin{split}
\mathbb E\operatorname{Var}\left(\sum_C A_C\mid\mathcal B\right)
&=\sum_C\mathbb E\operatorname{Var}(A_C\mid\mathcal B)\\
&\le\sum_C\mathbb E A_C^2\\
&\le v_C\sum_C\sum_{b\in C_{\rm int}}f_b^2\mathbb E r_b^2
\le C_C\sum_b f_b^2 .
\end{split}
\tag{ALL-CELL-INNOVATION}
\]
The identical proof applies to h. All boundary configurations and all interior field sectors are included. There is no discarded bad-cell term in this statement.

For completeness, MARKED-EXP also improves the good-chart tail in §4.18. If failure of the sufficient chart condition requires
$\sum_{p\in Y_C^{\rm bdry}}s_p>c_C\delta_C^2$
on a fixed boundary stencil, then
\[
\mathbb P\!\left(\sum_{p\in Y_C^{\rm bdry}}s_p
>c_C\delta_C^2\right)
\le C_C e^{-c'_C\beta\delta_C^2}.
\]
Combining this with the uniform fourth moments of r by Cauchy–Schwarz bounds the corresponding bad-cell second-moment contribution by another exponentially small quantity. ALL-CELL-INNOVATION does not need this refinement.

There is also a finite geometric way to cover every requested original stencil. Choose the fixed tiling side in §4.22 large enough compared with the stencil radius, retain sufficiently thick collars, and consider all lattice translations of that grid modulo its side. Thus the divisibility and even-factor requirements are the already displayed ones, now for this chosen larger side. Each root has its complete stencil strictly inside a cell of at least one translated grid. Assign each root to one such grid. The number J of grids is fixed. For grid j write the assigned sum as $A_j$, its collar algebra as $\mathcal B_j$, and
$M_j=\mathbb E(A_j\mid\mathcal B_j)$.
Then the full original sum A has the exact decomposition
\[
A=\sum_{j=1}^J M_j+\sum_{j=1}^J(A_j-M_j).
\]
Cauchy–Schwarz and ALL-CELL-INNOVATION give
\[
\left\|\sum_j(A_j-M_j)\right\|_{L^2}^2
\le J\sum_j\mathbb E\operatorname{Var}(A_j\mid\mathcal B_j)
\le C_C\sum_b f_b^2.
\tag{COVERED-INNOVATION}
\]
This covers the roots that crossed the collars of any single chosen grid. It does not assume independence between different grids.

Set $M=\sum_jM_j$ and $Q_f=\sum_bf_b^2$. The exact decomposition and COVERED-INNOVATION give the quantitative comparison
\[
\bigl(\sqrt{\operatorname{Var}M}-\sqrt{C_CQ_f}\bigr)_+^2
\le\operatorname{Var}A
\le\bigl(\sqrt{\operatorname{Var}M}+\sqrt{C_CQ_f}\bigr)^2.
\tag{RETAINED-MEAN-REDUCTION}
\]
Hence a uniform ordinary susceptibility bound for these marks is equivalent, up to a fixed additive square-root constant, to the corresponding bound for this explicitly retained sum M.

The only remaining piece in this decomposition is $\sum_jM_j$, with its actual cross-grid covariance. Its variance can be macroscopic even when every conditional innovation is bounded. No subtraction, positivity argument or rare-cell estimate in this section bounds it. This sharpens the next full-law susceptibility target to the retained conditional means; propagating their actual source rows and generated covariances is still necessary. Repeating the fixed-cell proof on a coarse marginal would require moment estimates for that marginal and its transported source, which MARKED-EXP for the original plaquettes does not automatically provide.

### 4.24 Native physical-chart construction and localized scalar differences (P/L geometry; C on scalar and physical-source matching)

There are two distinct requirements in applying LAP-ROW: a genuine physical coarse-field chart, and the coupling-family/selector identification. A local construction with constants uniform in volume is given below using the actual augmented native Hessian. An explicit based-gauge variation identifies its critical point with the physical minimum. This does not remove the flux or coupling-normalization issue of §4.21.

Use the original first-step selected corridor coordinates described in T1 Lemma 7.19, and write b for the physical coarse-link logarithms. These coordinates eliminate the average constraint; the gauge orbit coordinates are retained and controlled by the native exponential axial-gauge term. The same local constraint equation that eliminates a selected bond at target zero can be solved at a small target b: its derivative in that selected coordinate is invertible at the identity, and changing the target only adds an analytic inhomogeneous term. The resulting fine-link logarithms have a local analytic parametrization
\[
A=\Psi(b,y)=Rb+\mathcal C y+O((|b|+|y|)^2).
\tag{PHYSICAL-CHART}
\]
Here y are the independent fine fluctuation coordinates, $QR=I$, $Q\mathcal C=0$, and R and $\mathcal C$ have bounded finite-range row and column norms. The actual average and axial-gauge readout are used; no square root of a covariance is substituted. T1's check of the selected corridor equations also applies with this target. Since L and the stencil geometry are fixed, the analytic radius and every fixed-order local derivative bound are independent of the number of blocks.

**The gauge/Hessian dictionary.** Let $\mathscr G(U)$ be the original exponential axial-gauge action: a positive fixed multiple of the sum of $1-\operatorname{Re}\operatorname{tr}U(y,x)$ over the averaged contour variables from block center y to $x\ne y$. Define the augmented action
$\mathscr S(U)=S(U)+\mathscr G(U)$,
with the fixed relative coefficient chosen exactly as in the native first step. Its identity Hessian $H_{\rm aug}$ is the one used in the native covariance, including the gauge term. In particular
$A_{\rm fl}=\mathcal C^*H_{\rm aug}\mathcal C$,
not $\mathcal C^*H_{\rm Wilson}\mathcal C$. The checked covariance and the identity rows of the selected-coordinate injection give
\[
\|(A_{\rm fl}^{-1})_{xy}\|\le C e^{-\delta d(x,y)}.
\tag{AUGMENTED-INVERSE}
\]
Fixed action-normalization factors are included in C.

The augmented critical point is physical for a reason that can be checked directly. A based gauge transformation has $u(y)=I$ at every coarse center. It preserves the prescribed coarse average and sends each averaged contour variable to $U(y,x)u(x)^{-1}$. The independent values u(x) thus vary these gauge coordinates independently. The Wilson action is constant along this orbit. At an augmented constrained critical point, every orbit derivative of $\mathscr G$ must vanish. The function $1-\operatorname{Re}\operatorname{tr}V$ has a nondegenerate critical point at I and no other critical point in a fixed small chart; the same follows for its holomorphic extension by the local inverse theorem for its gradient. Consequently $U(y,x)=I$ for every such pair, $\mathscr G=0$, and the derivative of $\mathscr G$ in every direction vanishes. The remaining critical equation is precisely the constrained Wilson equation.

This uses the endpoint gauge covariance of the averaged contour, not a gauge-kernel deletion. The native definitions and critical-point identification are those of [CMP109, (0.11), (0.14)–(0.16), (2.2)–(2.5), printed pp.253–255,265–266](https://doi.org/10.1007/BF01215223). In the native normalized-trace convention the fixed multiple in $\mathscr G$ changes together with the normalization of S; it has no effect on the above orbit argument.

The constrained critical equation is
\[
0=D_y[\mathscr S(\exp\Psi(b,y))]
=A_{\rm fl}y+Tb+\mathcal N(b,y),
\qquad T=\mathcal C^*H_{\rm aug}R,
\tag{CONSTRAINED-NEWTON}
\]
where T is finite range, $\mathcal N(0,0)=D\mathcal N(0,0)=0$, and
\[
\|\mathcal N(b,y)-\mathcal N(b,\widetilde y)\|_\infty
\le C\rho\|y-\widetilde y\|_\infty
\]
on $\|b\|_\infty+\|y\|_\infty\le\rho$. These estimates follow by differentiating the finite-range analytic chart, local plaquette action and block-local gauge action; each derivative component meets only a bounded number of action terms.

Choose rho so that the exponential Schur norm of $A_{\rm fl}^{-1}$ times $C\rho$ is below 1/2, and then choose a fixed $\delta_b>0$ so that $\|b\|_\infty<\delta_b$ makes
\[
y\longmapsto-A_{\rm fl}^{-1}[Tb+\mathcal N(b,y)]
\]
a self-map of a smaller rho-ball. The contraction theorem gives a unique small solution $y_*(b)$, holomorphic in b, with
$\|y_*(b)\|_\infty\le C\|b\|_\infty$.
For real b it is the regular augmented minimum: the real restricted augmented Hessian remains positive by the same operator-norm perturbation estimate. The based-gauge argument above puts it on the axial slice and identifies the physical constrained minimizing orbit. This identifies the local regular branch, rather than claiming global convexity of the compact action.

For a fixed finite set E of coarse bonds, introduce
$\|y\|_{\alpha,E}=\sup_x e^{\alpha d(x,E)}|y_x|$, $0<\alpha<\delta$.
Finite-range products obey
$\|uv\|_{\alpha,E}\le C\|u\|_\infty\|v\|_{\alpha,E}$,
and the exponential inverse is bounded in this weighted norm. Reducing the fixed radius once more, the same contraction for b supported in E gives
\[
|A_*(b)_x|+|J_*(b)_x|
\le C\|b\|_\infty e^{-\alpha d(x,E)}.
\tag{PHYSICAL-RESPONSE}
\]
The current $J_*$ is the original local physical action-current readout; it is analytic and vanishes at the identity, so its bound follows from the fine-field bound. First differences and the finitely scaled current satisfy the same estimate. At the first step all mesh factors are fixed powers of L. Shrinking $\delta_b$ places the real part at the identity and the complex perturbation in the smaller simple native external domain. CMP109 pp.262–263, after (1.16), shows that these smaller first-order/current bounds imply its additional nested-domain condition. Thus this construction supplies a common physical chart inside that first-step native domain. It does not assert this chart uniformly through an unbounded number of inherited steps.

**A nonzero classical quadratic direction.** Let H in this paragraph denote the Wilson Hessian alone, and let $E_{\rm min}b=Rb+\mathcal C y_*'(0)b$. Then
$QE_{\rm min}b=b$ and $S_{*,2}(b)=\frac12\langle E_{\rm min}b,H E_{\rm min}b\rangle$.
There is a finite-range bounded operator $\mathcal R_2$ satisfying
\[
d_{\rm coarse}Q=\mathcal R_2d_{\rm fine}.
\]
To see this directly, expand the coarse plaquette boundary after applying the linearized contour average Q. Each resulting fine chain is closed: endpoint contributions cancel around the coarse plaquette. It lies in a fixed finite union of the four endpoint blocks and corridors, and it can be filled by finitely many fine plaquettes. Choose these fillings once for every translated contour type and sum their averaging coefficients. This constructs $\mathcal R_2$ with bounded overlap and hence bounded $\ell^2$ norm. Therefore
\[
S_{*,2}(b)\ge
\frac{\tau}{2\|\mathcal R_2\|_{2\to2}^2}
\|d_{\rm coarse}b\|_2^2 .
\tag{DIRECTIONAL-HESSIAN}
\]
For a unit color field on one coarse bond of a nondegenerate torus,
$\|d_{\rm coarse}b\|_2^2=6$ in four dimensions. This gives a fixed positive classical coefficient in a concrete physical direction, without using a whole-torus lower bound on the massless Hessian.

**How the rooted scalar bound is actually used.** Suppose the native scalar remainder has a local expansion
$\mathcal E(w;U,J)=\sum_X\mathcal E_X(w;U,J)$
with
\[
\sup_{(U,J)\in\mathcal D}|\mathcal E_X(w;U,J)|
\le \frac{A}{|w|}w_X,\qquad
\sup_x\sum_{X\ni x}w_X\le K,
\tag{ROOTED-SCALAR}
\]
on a common external domain with fixed spare radius. T1 §7.27 proposes this at the first step with $A=Cp^2$, subject to its stated native expansion and cutoff-transfer proof. It is kept as an explicit input here.

Fix the preceding compactly supported physical direction $b=sb_0$. Locality of $\mathcal E_X$, Cauchy's formula on the spare external radius, and PHYSICAL-RESPONSE imply
\[
|\mathcal E_X(w;U_*(sb_0),J_*(sb_0))
-\mathcal E_X(w;I,0)|
\le \frac{CA}{|w|}w_X\,|s|
\sum_{x\in X}e^{-\alpha d(x,E)}.
\]
Sum first over X containing x and then over x. This proves the volume-independent difference estimate
\[
|\mathcal E(w;sb_0)-\mathcal E(w;0)|
\le C_E A/|w|
\qquad(|s|<\delta_b).
\tag{LOCALIZED-SCALAR-DIFFERENCE}
\]
The extensive background-independent scalar was subtracted before applying Cauchy; its size is not mistaken for a local coefficient.

On $|w-\beta|<\eta\beta$, Cauchy in w and s now bounds the coefficient
\[
\left|[s^2]\partial_\beta
[\mathcal E(\beta;sb_0)-\mathcal E(\beta;0)]\right|
\le\frac{C_E A}{\eta(1-\eta)\delta_b^2\beta^2}.
\tag{LOCALIZED-ACTION-ERROR}
\]
Combined with DIRECTIONAL-HESSIAN, this gives the desired small relative correction to the chosen physical classical-action quadratic direction if ROOTED-SCALAR and the fixed-physical-domain coupling identification hold. For a frozen canonical selector the additional flux coefficient must be included as in MOVING-ACTION-ROW. The derivative of the native exponential gauge factor and its Faddeev–Popov normalization must also be retained: the based-gauge argument identifies the saddle, but a truncated selector need not factor along entire gauge orbits. It does not automatically cancel the gauge-energy expectation against the normalization derivative.

This is a directional, first-step conclusion. It is not yet the full tensor mixing matrix or the zero-momentum marginal action coefficient: a localized physical direction also evaluates higher-derivative quadratic rows. Identifying that particular marginal coefficient requires the specified local extraction and its displacement-moment bounds. Neither the chart construction nor the scalar difference estimate suppresses this distinction.

### 4.25 Physical action source versus the auxiliary gauge coupling (P at the first Gaussian step)

The augmented Hessian in §4.24 must also be respected when counting the identity row. A physical Wilson-action source changes the Wilson action only, while the native exponential gauge factor can be held fixed. The two derivatives need not have the same identity coefficient.

At a regular axial critical point, the based gauge group provides local orbit coordinates a and physical slice coordinates z. Its contour coordinates satisfy $U(y,x)=a_x$, while the Wilson action is independent of a. The gauge action is a function of a alone. At the identity, and at fixed coarse field b to quadratic order, the original quadratic forms consequently have the simultaneous decomposition
\[
S_2=S_{*,2}(b)+\frac12 z^{\mathsf T}H_{\rm ph}z,\qquad
\mathscr G_2=\frac12 a^{\mathsf T}H_{\rm g}a,
\]
with positive $H_{\rm ph}$ and $H_{\rm g}$. The physical/gauge coordinate transformation has a constant linear Jacobian; cross terms vanish in these orbit coordinates. Let their dimensions be $d_{\rm ph}$ and $d_{\rm g}$.

Fix the reference gauge coupling $\beta_0$ and vary the Wilson coefficient w. The full Gaussian integral is exactly
\[
Z_2(w,b;\beta_0)
=a_2\,e^{-wS_{*,2}(b)}
w^{-d_{\rm ph}/2}\beta_0^{-d_{\rm g}/2},
\tag{TWO-COUPLING-GAUSSIAN}
\]
where $a_2$ is independent of w and $\beta_0$. The Gaussian gauge normalization, if included, is also independent of w. Thus the physical source $uS_2/N$, at $w=\beta_0=\beta$, has normalized source ratio
\[
\exp[uS_{*,2}(b)/N]\,
\left(1-\frac{u}{N\beta}\right)^{-d_{\rm ph}/2}.
\tag{PHYSICAL-GAUSSIAN-ROW}
\]
Its retained action coefficient is one, its identity row is $d_{\rm ph}/(2N\beta)$, and its scalar second contact is $d_{\rm ph}/(2N^2\beta^2)$. More generally its mth scalar cumulant is
$d_{\rm ph}(m-1)!/[2N^m\beta^m]$ for m≥2.
These are the formulas of §4.13 with the *physical* fluctuation dimension, when the original native augmented integral is used.

**The first periodic dimension count.** On a nondegenerate periodic lattice with fine side n and coarse side n/L, the derivative of each coarse-link constraint has an independent selected bond. Therefore
\[
d_{\rm tot}=d_G(E_f-E_c),\qquad
d_{\rm g}=d_G(V_f-V_c).
\]
Based gauge transformations are fixed at every coarse center and have one independent Lie-algebra parameter at each other fine vertex. The action is free locally; hence these orbit coordinates have the stated dimension. Since $E_f=4V_f$, $E_c=4V_c$,
\[
d_{\rm ph}=3d_G\bigl[n^4-(n/L)^4\bigr].
\tag{PHYSICAL-DIMENSION}
\]
Per coarse block this is $3d_G(L^4-1)$, giving the identity coefficient
$3d_G(L^4-1)/(2N\beta)$ for the integrated normalized action source. Original lattice or physical source-density conversion factors must still be restored. This is an off-shell constrained count; no massless on-shell polarization argument is used.

If w instead multiplies both S and $\mathscr G$, the unnormalized determinant has exponent $(d_{\rm ph}+d_{\rm g})/2$. Its derivative inserts the augmented action. Subtracting a background-independent gauge normalization can remove the gauge piece only when the actual integration domain permits the corresponding factorization. An arbitrary original small-field selector can couple a and z, so the exact cancellation is not asserted for that cutoff integral.

**A concrete fixed-domain physical-source family.** At reference coupling $\beta_0$, keep the physical readout $\Psi_b(g_0B)$, original selector, all Jacobians, exponential gauge factor and its normalization fixed. Introduce the independent parameter w only in $\exp[-wS]$. This family has exactly the desired physical action derivatives, without the moving-domain flux caused by replacing $g_0$ with $g(w)$.

At the flat quadratic level its precision is
$wH_{\rm W}+\beta_0H_{\rm G}$.
For $|w/\beta_0-1|<\theta<1$, positivity of the two real quadratic forms gives
\[
\operatorname{Re}\langle v,
(wH_{\rm W}+\beta_0H_{\rm G})v\rangle
\ge(1-\theta)\beta_0
\langle v,(H_{\rm W}+H_{\rm G})v\rangle.
\]
Thus the physical-source Gaussian comparison has a proportional complex w-domain. Its nonlinear constrained Wilson action still has no linear tangent fluctuation term, because its saddle is a physical constrained minimum. This is the exact next two-parameter expansion to verify in the native nonlinear theorem. The Gaussian domain and dimension count do not by themselves prove its cluster remainder, its cutoff comparison or its inherited-step analogues.

### 4.26 Two constrained steps with the ordinary source

Fix the reference torus and the original Wilson measure under the hypotheses of MARKED-EXP. Let $X_1$ and $X_2$ be two successive real retained variables of the original positive blocking map, including any retained history coordinates. The argument applies to an exact disintegration of the positive joint law. A signed or complex term of a polymer expansion requires separate absolute estimates before one can use it as a probability weight.

For each original bond b set $m_{0,b}=r_b-\mathbb E r_b$ and $m_{j,b}=\mathbb E(m_{0,b}\mid X_j)$. Write $m_j$ for the complete vector indexed by the original bonds and set
\[
D_1=m_0-m_1,\qquad D_2=m_1-m_2.
\]
The Markov property gives $\mathbb E(D_1\mid X_1,X_2)=0$ and $\mathbb E(D_2\mid X_2)=0$. Consequently the actual connected two-source matrix has the positive decomposition
\[
K_0=J_1+J_2+K_2,\qquad
J_j=\mathbb E D_jD_j^*,\quad K_2=\mathbb E m_2m_2^*.
\tag{TWO-STEP-WILSON}
\]
Here $J_1$ is the first conditional innovation. The second innovation is the covariance created when the *whole* first retained ordinary source is integrated in step two. Original Casimir terms, action rows, irrelevant terms and history-dependent scalar rows all occur inside $m_1$.

There is a uniform matrix estimate for these actual terms. TORUS-LOCAL-MOM gives
\[
\operatorname{Tr}J_1+\operatorname{Tr}J_2+\operatorname{Tr}K_2
=\sum_b\operatorname{Var}(r_b)\le C\,4n^4.
\tag{SHARED-TRACE}
\]
Both innovations and the twice-retained mean share this one budget. In a unitary fine-lattice Fourier basis it gives
\[
\frac1{n^4}\sum_{p,\nu}
\left[\langle e_{p,\nu},J_1 e_{p,\nu}\rangle+
\langle e_{p,\nu},J_2 e_{p,\nu}\rangle+
\langle e_{p,\nu},K_2 e_{p,\nu}\rangle\right]\le4C.
\tag{AVERAGED-SUS}
\]
The vectors $e_{p,\nu}$ have fine-lattice norm one. No fine-translation invariance of a particular coarse grid is needed. This estimates the momentum average uniformly in the cutoff. The maximum over momenta required by SUS remains a stronger norm.

For example, if $X_j=(W_j,H_j)$ has physical field $W_j$ and positive history record $H_j$, then
\[
\mathbb E\operatorname{Cov}(m_{j-1}\mid W_j)
=J_j+\mathbb E\operatorname{Cov}(m_j\mid W_j),
\]
provided $m_j=\mathbb E(m_{j-1}\mid W_j,H_j)$, as follows from the Markov chain. Thus forgetting history adds its conditional-mean covariance to the innovation. Its matrix is positive and included within the original trace budget. A history-dependent scalar row can contribute to it even when that row has no physical field dependence within one history. A deterministic identity row contributes zero.

**Both linearized native constraints, including the retained quadratic row.** The quadratic comparison gives a stronger bound with the full source norm. Work on the physical Gaussian quotient at the flat background and omit harmonic null directions, which are killed by every matching Hessian. Let $H=\sum_{i=1}^3H_i\ge0$, $0\le H_i\le H$, and $\|H_i\|_{\rm op}\le8\tau$ as in §4.8. Let $Z$ be standard real Gaussian on the range of H, so $\sqrt\beta A=H^{+1/2}Z$, where $H^{+1/2}$ denotes the square root of the Moore–Penrose inverse. For a real mark f let F be its diagonal matrix repeated on color coordinates. Set
\[
T_i=H_i H^{+1/2},\qquad A_f=\sum_i T_i^*FT_i .
\]
The ordinary source, including its Casimir companion, is
\[
r_f^{(2)}=Z^*A_fZ-\tfrac13\operatorname{Tr}(FH).
\]
Since $H_iH^+H_i\le H_i$, the operator and Hilbert–Schmidt bounds are
\[
\|A_f\|_{\rm op}\le24\tau\|f\|_\infty,\qquad
\|A_f\|_{\rm HS}\le24\tau\sqrt{d_G}\,\|f\|_2 .
\tag{ORDINARY-HS}
\]
Indeed $H^{+1/2}H_iH^{+1/2}\le I$, giving the first displayed inequality for $H_iH^+H_i$ by factoring with $H_i^{1/2}$. Then apply the ideal property of the Hilbert–Schmidt norm to each $T_i^*FT_i$. No inverse soft-mode constant enters ORDINARY-HS.

Let $Q_1$ and $Q_2$ be the actual linearized first and second physical coarse averages on the gauge quotients. In whitened fine coordinates their observations are
$L_1Z=Q_1 H^{+1/2}Z$ and
$L_2 Z=Q_2Q_1 H^{+1/2}Z$.
Scalars from mesh rescaling do not change their row spaces. Put
\[
P_0=I,\qquad P_j=L_j^*(L_jL_j^*)^+ L_j,\qquad R_j=P_{j-1}-P_j .
\]
Because $\operatorname{ran} P_2\subset\operatorname{ran} P_1$, both $R_1$ and $R_2$ are orthogonal projections. Conditioning on $L_j Z$ retains $P_jZ$ and integrates the independent complement. Hence
\[
\mathbb E(r_f^{(2)}\mid L_j Z)
=Z^*P_j A_fP_j Z+
\operatorname{Tr}[(I-P_j)A_f]
-\tfrac13\operatorname{Tr}(FH).
\tag{TWO-STEP-QUADRATIC-MEAN}
\]
In particular the second retained quadratic kernel is $P_2 A_f P_2$. The additional identity term created at step j is exactly $\operatorname{Tr}(R_j A_f)$.

At step j, conditional on $P_j Z$, the innovation variance is
\[
2\|R_jA_fR_j\|_{\rm HS}^2+
4(P_j Z)^* A_fR_j A_f(P_j Z).
\tag{TWO-STEP-QUADRATIC-CONTACT}
\]
The second term is a background-dependent quadratic contact. The formula follows by writing $P_{j-1} Z=P_j Z+R_j Z$ and integrating the independent standard vector $R_j Z$. The covariance between the linear and centered quadratic fluctuation vanishes by odd Gaussian parity. After averaging the background,
\[
\mathbb E\operatorname{Var}
\big(\mathbb E[r_f^{(2)}\mid L_{j-1}Z]\mid L_jZ\big)
=2\left(\|P_{j-1}A_fP_{j-1}\|_{\rm HS}^2
-\|P_jA_fP_j\|_{\rm HS}^2\right).
\]
The two innovations plus the variance of the retained quadratic mean telescope to
$2\|A_f\|_{\rm HS}^2\le C M_f$.

There is also explicit volume scaling for plane waves:
\[
\operatorname{Var}\mathbb E(r_f^{(2)}\mid L_jZ)
=2\|P_jA_fP_j\|_{\rm HS}^2
\le C\,d_G(n/L^j)^4\|f\|_\infty^2 .
\tag{RETAINED-GAUSSIAN-VOLUME}
\]
Use $\operatorname{rank}P_j\le 4d_G(n/L^j)^4$ and ORDINARY-HS. Relative to a unit-amplitude plane wave on $n^4$ fine sites, the retained variance bound carries $L^{-4}$ after one constraint and $L^{-8}$ after two. Complex plane waves follow by applying the real calculation to both components. These formulas are exact for the actual physical *linearized* constraints. Restoring the nonlinear Wilson measure requires controlling the change in the connected kernels. Its gauge/selector terms and its histories remain present in TWO-STEP-WILSON.

**Two exact local disintegrations on the full Wilson torus.** For comparison with the native averages, there is a full-law two-step construction where both innovations admit an extensive bound without a small-field selection. Use nested block partitions with fixed fine sides L and $L^2$ (or any two fixed compatible sides large enough for the required stencils), and retain separating collars. Choose the second collar set as a subset of the first. Every plaquette then touches at most one open interior in each partition. Write $\mathcal C_2\subset\mathcal C_1$ for their collar sigma algebras.

Assign complete source stencils to finest cells, with finitely many translated grids as in §4.23 if needed. For one such grid, $m_{1,b}=\mathbb E(r_b\mid\mathcal C_1)$ is a function only of the first collar around its assigned cell, by Wilson finite-range conditional independence. Choose the cell collars and assignments so that this function involves only its containing second cell and its second collar. Alternatively include a finest cell only when its collar is contained there, using the finite shifted coverings below for boundary cells.

Conditional on $\mathcal C_2$, different second-cell interiors are independent. For a largest cell B set $M_{1,B}=\sum_{b\text{ assigned in }B}f_b m_{1,b}$. Then
\[
\begin{split}
\mathbb E\operatorname{Var}(\sum_B M_{1,B}\mid\mathcal C_2)
&\le\sum_B\mathbb E |M_{1,B}|^2\\
&\le v_2\sum_b |f_b|^2\mathbb E|m_{1,b}|^2
\le C v_2 M_f,\qquad v_2\le C L^8.
\end{split}
\tag{SECOND-COLLAR-INNOVATION}
\]
The last inequality is conditional Jensen followed by TORUS-LOCAL-MOM. The first innovation costs $C v_1 M_f$ with $v_1\le CL^4$. The same finite family of translates modulo the large-cell side covers every original stencil by choosing, for each root, a translate placing it and its entire small collar inside a large cell. Cauchy–Schwarz over these finitely many grids preserves the bound with a constant depending on L. This argument includes every Wilson field sector.

The twice-retained collar observable has the exact expression
$\sum_b f_b\mathbb E(r_b\mid\mathcal C_2)$ on each grid. Its variance and its cross-grid covariances remain. The cost $v_j$ in this direct local estimate grows as $L^{4j}$ on longer towers, in contrast with the decreasing retained rank bound in the Gaussian calculation. The native coarse-average state retains different information from a separating collar. Independent interiors in SECOND-COLLAR-INNOVATION cannot be transferred to the native conditional measure merely by deleting the collars.

### 4.27 Uniform transport of the Ward row and connected energetic clusters

There is an extensive estimate in TWO-STEP-WILSON for the complete Ward companion, including its retained mean. It uses the full compact Wilson law and therefore applies to every genuine positive blocking kernel in the tower.

Recall $t_b=h_b-r_b$ and $t_b\rho=-\operatorname{div}(\rho V_b)$ with $V_b=-\frac13\sum_A F_b^A X_b^A$. Haar integration gives
\[
\mathbb E t_b=0,\qquad \mathbb E(t_bF)=\mathbb E(V_b F).
\]
For $F=t_c,r_c,h_c$, this derivative vanishes unless the two microscopic stencils meet. On a meeting stencil the force-factor argument for H-LOCAL applies to each term separately:
\[
|V_bt_c|+|V_br_c|+|V_bh_c|
\le C(\beta+1)\sum_{p\in Y_{bc}}s_p .
\tag{SEPARATE-WARD-ROWS}
\]
Each quadratic force derivative contains one remaining first force and the vector field supplies another. The derivative of the Casimir term is a plaquette first derivative. The first moment bound FIRST therefore gives a uniform absolute row and column sum for all three expected matrices. In particular
\[
0\le\operatorname{Cov}(t)\le C I
\]
as an operator on the original bond-mark space. This alone uses REG and FIRST. The stronger chessboard tiling assumption is unnecessary here.

Apply TWO-STEP-WILSON to t. Every positive component of its covariance satisfies
\[
0\le J_1^t+J_2^t+K_2^t\le CI.
\tag{FULL-WARD-TOWER}
\]
More generally the same inequality holds for any number of positive steps. If a history is forgotten, the covariance of its conditional mean forms another positive component of the same budget. Thus each Ward innovation, every twice-retained Ward mean, and their sum of variances have the required extensive bound for all marks, uniformly in n.

For any one of the orthogonal projections onto the jth innovation or the final retained information, write $\Pi$ for the corresponding map on centered square-integrable original observables. The exact identity $r_f=h_f-t_f$ and FULL-WARD-TOWER give
\[
\left|\|\Pi r_f\|_2-\|\Pi h_f\|_2\right|
\le C^{1/2}\|f\|_2.
\tag{EACH-ROW-REDUCTION}
\]
An actual two-step estimate for the frustrated force square consequently suffices for the ordinary row at that same step. This covers the Ward part across mixed states without identifying its conditional expectation with zero.

**Connected energetic defects.** There is an actual summable part of the two-source history matrix. Fix a finite-range graph on original plaquettes of bounded degree. Mark a plaquette as energetic when $\beta s_p\ge u$. Let $E_{bc}$ be the event that one connected component of energetic plaquettes meets the fixed stencils of b and c. MARKED-TAIL gives
\[
\mathbb P(E_{bc})\le C e^{-m(u)d(b,c)}
\]
for a sufficiently large dimensionless u, uniformly on the tori covered by §4.22. Indeed a component connecting the stencils contains a simple path of length at least $c d(b,c)-C_0$. There are at most $C\Delta^k$ possible paths of k vertices from the first stencil. The probability that all k vertices are energetic is at most $\exp[-(t_*u-K_{\sigma,\ell})k]$. Summation gives the displayed decay.

Let $U_b,V_c$ be any two of the centered original ordinary sources, their first or second retained means, or their first or second innovations. TORUS-LOCAL-MOM and conditional Jensen give uniformly bounded fourth moments for each of these variables. Cauchy–Schwarz gives
\[
|\mathbb E[U_bV_c\,1_{E_{bc}}]|
\le C e^{-m(u)d(b,c)/2}.
\tag{ONE-DEFECT-CLUSTER}
\]
This has uniformly summable anchor rows. It applies equally when the two conditional means include positive history labels. The complementary covariance includes different clusters and clean fluctuations. This estimate quantifies the contribution selected by the specified energetic event, whose relation to each native live or merger label must still be checked in its own definition.

**Energy through two physical averages.** Consider a real coarse average formed from the stated finite contour averages wherever its fine field lies in the common small chart. For each coarse plaquette P after one or two such steps, choose a contractible fine neighborhood $Y(P)$ containing all of its determining contours and their fillings. For fixed j=1,2 and L the sizes and overlaps are bounded independently of n. On a sufficiently large torus these patches do not wrap. Then
\[
s_P(W_j)\le C_{j,L}\sum_{p\in Y(P)}s_p(U).
\tag{TWO-AVERAGE-ENERGY}
\]
On the event of small right-hand side, gauge-fix a tree inside the patch. Every other link is a loop with a fixed finite filling, so all fine links lie within $C\sqrt{\sum_{Y(P)}s_p}$ of I. The contour averages are locally Lipschitz and take I to I. Use this once or twice and square the resulting distance bound for the coarse plaquette. On the complement, compactness gives $s_P\le2N$ and the fine energy exceeds a fixed threshold. The conclusion also holds for a measurable compact extension of the average on that complement. A replacement which can alter the output even on the specified good patch requires its own check.

For a set of k distinct coarse plaquettes, sum TWO-AVERAGE-ENERGY over the set. A fine plaquette has bounded multiplicity in these patches. MARKED-EXP therefore gives constants $t_{j,L}>0,K_{j,L}<\infty$ with
\[
\mathbb E\exp\bigl(t_{j,L}\beta\sum_{P\in\mathcal A}s_P(W_j)\bigr)
\le e^{K_{j,L}k}.
\tag{COARSE-MARKED-EXP}
\]
Explicitly choose $t_{j,L}=t_*/(C_{j,L}m_{\rm ov})$, where $m_{\rm ov}$ is the maximum fine overlap, and $K_{j,L}=K_{\sigma,\ell}\sup_P|Y(P)|$. This controls canonical local plaquette and force rows at the two physical retained scales, and reproduces ONE-DEFECT-CLUSTER for their specified energetic events. Exact conditional means of original sources can also depend on the rest of the coarse state. COARSE-MARKED-EXP alone does not identify them with these local rows.

### 4.28 The ordinary and frustration quadratic reserve across two clean constrained steps

Consider the first two clean small-field integrations of the native map with terminal coarse field equal to I. Keep both independent fluctuation fields $B_0,B_1$ as integration variables. The first coarse background $W_1$ is then a function of $g_1B_1$. The fine field is obtained from the original first constraint at $W_1$ and $g_0B_0$. This composition gives a two-step bound for the physical source at the level of its actual integrand. The ratios $g_1/g_0$ are bounded under the stated one-step weak-coupling flow.

**Locality of the required Taylor coefficients.** Work on a periodic grid and write a field map at output bond x as an ordered Taylor kernel. For a positive physical radius r define
\[
\|A\|_{r,\alpha}=\sup_x\sum_{m\ge0} r^m
\sum_{u_1,\ldots,u_m}|A_m(x;u_1,\ldots,u_m)|
e^{\alpha\mathcal T(x,u_1,\ldots,u_m)} .
\tag{TREE-ANALYTIC-NORM}
\]
All color, species and orientation labels are summed in the finite coefficient norm. Distances are measured on the original unit grid, with L fixed. A connected tree joining x and the argument anchors gives the weight. Constants depend on L.

The norm is submultiplicative for products rooted at x because the union of their two connecting trees is connected. An exponentially decaying linear kernel acts boundedly at every smaller exponent by attaching the edge from x to its input root. A finite-range analytic map of a bounded number of arguments has a convergent norm on a sufficiently small physical radius. These statements follow by summing the absolute Taylor coefficients in the indicated order. They also show that composition with a field map of sufficiently small norm converges: each Taylor factor's argument tree is attached at its argument root, and the union joins the output to every new input.

Apply this construction to CONSTRAINED-NEWTON. Its linear forcing has size $O(r)$ in TREE-ANALYTIC-NORM. The remainder $\mathcal N$ has no constant or linear term and is a uniformly local analytic map. On a ball of norm $Cr$ its composition has norm $O(r^2)$ and Lipschitz constant $O(r)$. AUGMENTED-INVERSE has a finite exponentially weighted Schur norm below its decay rate. For sufficiently small r the same contraction as in §4.24 now converges in TREE-ANALYTIC-NORM. Its limit agrees with the physical minimizer by local uniqueness. This strengthens PHYSICAL-RESPONSE to an absolutely summed bound on all Taylor coefficients of that first minimizer.

The second constraint at the flat terminal field has the selected-coordinate readout of T1 Lemma 7.19 with physical argument $u_1=g_1B_1$. In the first constrained readout the selected equation also depends locally and analytically on its finitely many first-minimizer background links and contour variables. Its selected-coordinate derivative at I is invertible. The local implicit-function theorem gives a common radius in those variables and in $u_0=g_0B_0$. Combine these finite-range maps, the minimizing background map just proved and the local group products. The resulting original fine field, written in logarithm coordinates as $A(u_0,u_1)$, has finite TREE-ANALYTIC-NORM on a common physical polydisc, satisfies $A(0,0)=0$, and has a finite exponentially weighted linear response. All complete original plaquette stencils are evaluated after this composition.

**The joint source coefficient.** Let $\mathcal H_b(U)=h_b(U)/\beta$ be the exact frustration polynomial and let $\mathcal D_b(U)=D_b(U)$. Both vanish to at least order two at I. Their pullbacks through the preceding actual two-step map therefore have Taylor expansions starting at degree two, with the weighted norm just proved. Selecting the first two factors in each ordered Taylor monomial gives
\[
h_b=\sum_{i,k} B_i v^b_{ik}(u_0,u_1)B_k ,
\tag{JOINT-FRUSTRATION}
\]
where the combined index ranges over both fluctuation species, including their original lattice labels. Each selected pair supplies a factor $\beta g_{\mathrm{sp}(i)}g_{\mathrm{sp}(k)}$, uniformly bounded because $\beta g_0^2$ is fixed and $g_1/g_0$ is bounded. On a smaller polydisc the remaining Taylor coefficients converge absolutely with the connecting-tree weight. The same assertion holds for $\beta D_b$.

The root norm bounds $\sup_b\sum_{i,k}|v_{ik}^b|$. For the needed column bound one can anchor at i instead. One justification sums the translation-covariant absolute coefficients over every root in a periodic fundamental cell of the two-step coarse grid, and exchanges the root and selected index sums. There are only finitely many species and positions in that cell, depending on L. Translation covariance then gives a bound on every such column. This argument is applied to the majorant Taylor coefficients before evaluating a nonconstant background or an arbitrary mark. It yields
\[
\sup_i\sum_{b,k}
e^{\alpha'\mathcal T(i,b,k)}
|v_{ik}^b(u_0,u_1)|\le C_L
\quad (0<\alpha'<\alpha)
\tag{JOINT-COLUMN}
\]
after shrinking the radius. Symmetrizing in i,k gives both Schur bounds. The constants are independent of the volume and of the canonical cutoff height, as long as the physical fields remain in the common chart.

For $|\eta_b|\le r_s$, the real quadratic-growth allowance is consequently
\[
\left|\sum_b\eta_b h_b\right|
\le C_L r_s\left(\|B_0\|_2^2+\|B_1\|_2^2\right).
\tag{JOINT-RESERVE}
\]
This is the original two-step frustration source at the clean integrand. If one first fixes $B_1$ and expands in $B_0$, the $B_1B_1$ part is a field-dependent scalar and the $B_0B_1$ part is the first-step linear row. JOINT-RESERVE pays that cross term by both integrated Gaussian energies. It keeps the complete scalar and linear rows and avoids a supremum proportional to the square of the allowed canonical background radius. For the ordinary source one also keeps the Casimir term $-\ell_b/3$. Its constant row is explicit and its difference from its identity value is quadratic in the same two physical fields by the plaquette Casimir identity.

A localized coefficient can be assigned to a connected lattice carrier by filling a chosen shortest connecting tree for its labels. Absolute convergence in TREE-ANALYTIC-NORM pays the tree length at any smaller exponent. This supplies a two-step verification of the source part of the required quadratic-growth class for the joint pair of fluctuation fields. To conclude nonvanishing or an extensive two-step connected covariance one also needs the corresponding joint unmarked Gaussian comparison, constraint and gauge Jacobians, and the actual two selectors in their connected expansion. Detaching the two conditional denominators would lose precisely the retained mean term in TWO-STEP-WILSON. This calculation does not perform that detachment.

### 4.29 Full Wilson susceptibility away from the coordinate momentum planes (P)

The full Wilson transfer operator and the local moment bound control a class of Fourier directions, including their innovations through the two actual constrained steps. Write $p_j=2\pi k_j/n$ for dimensionless lattice momenta. Fix $\delta>0$. Uniformly for all momenta satisfying
\[
\min_{1\le j\le4}|\sin(p_j/2)|\ge\delta,
\]
and for arbitrary bond polarizations v, one has
\[
\operatorname{Var}\!\left(\sum_{x,\nu}
v_\nu e^{ip\cdot x}r_{x,\nu}\right)
\le C_{\delta,\sigma} n^4 |v|^2 .
\tag{OFF-PLANE-SUS}
\]
For complex marks, variance denotes the squared centered complex $L^2$ norm. The same statement holds for h. The hypotheses are REG and the torus tiling condition in §4.22 yielding uniform local second moments. The bounded number of tori smaller than a fixed insertion stencil can be absorbed into the constant by Cauchy–Schwarz.

**Positive transfer along any coordinate.** Pick one coordinate as time. A spatial slice consists of the three-dimensional set of spatial links $\sigma$. Its spatial Wilson weight supplies one half-factor at each end of a step. Before averaging the temporal links, the kinetic convolution has product kernel
\[
K(\sigma,\sigma')=\prod_e
\exp\bigl(\beta\operatorname{Re}\operatorname{Tr}
(\sigma_e{\sigma'_e}^{-1})\bigr)
\]
up to a positive scalar. Each central factor defines a positive convolution operator. Indeed expand the exponential into products of the fundamental trace character and its conjugate. Every product is a character of a tensor product with a nonnegative coefficient, and its convolution operator is positive by matrix-element orthogonality. Absolute convergence on the compact group permits summing the expansion. Integrating the temporal links averages over slice gauge transformations. This is an orthogonal projection P commuting with K, since simultaneous slice gauge transformation preserves each factor. The resulting transfer operator is $T=V^{1/2}KPV^{1/2}$, where V multiplies by the positive spatial Wilson weight. It is positive and selfadjoint. Inserting the slice kernels and performing the temporal Haar integrations gives the periodic Wilson partition function $\operatorname{Tr}T^n$, with its scalar factors included. This is the pure-gauge part of the construction in [Lüscher, *Construction of a selfadjoint, strictly positive transfer matrix for Euclidean lattice gauge theories*](https://doi.org/10.1007/BF01614090).

**A transverse Fourier mode.** Fix one bond orientation $\nu$ and a transverse momentum q in the three remaining coordinates. Let
\[
A_q(t)=n^{-3/2}\sum_{x_\perp} e^{iq\cdot x_\perp}
\big(r_{(t,x_\perp),\nu}-\mathbb E r_{(t,x_\perp),\nu}\big),\qquad
C_q(s)=\mathbb E[\overline{A_q(0)}A_q(s)] .
\]
There is a slab of fixed integer width w containing the whole stencil at t. Its midpoint is at the time coordinate of the bond center, an integer for a transverse bond and a half-integer for a time bond. Choose the endpoints as lattice site planes symmetric about that midpoint. Reflection in this midpoint preserves the local insertion. Coordinate-axis reflection preserves each Wilson matching action. Reversal of an oriented link converts its left derivative to a right derivative with an orthogonal adjoint change of color coordinates, preserving the squared force. The bi-invariant Casimir Laplacian is preserved as well. These facts give the same midpoint property for h.

Integrating this slab with the insertion and half of each endpoint spatial action yields an operator $O_q$ on slice configurations. Reflection of the slab interchanges its endpoints. Complex conjugation reverses the transverse Fourier phase, so $O_{-q}=O_q^*$. For two disjoint open slabs, at integer separation $w\le s\le n-w$,
\[
C_q(s)=\frac{1}{\operatorname{Tr}T^n}
\sum_{\alpha,\gamma}
|(O_q)_{\alpha\gamma}|^2
\lambda_\alpha^{\,s-w}\lambda_\gamma^{\,n-s-w},
\tag{SLAB-SPECTRUM}
\]
up to interchanging the two eigenvalue indices. Here $\lambda_\alpha\ge0$ are the eigenvalues of T. Each spatial-slice operator has a bounded integral kernel at fixed n and beta. Products of positive powers of the transfer operator and these Hilbert–Schmidt kernels justify the trace expansion. The centered insertion is used on both slabs.

Every term in SLAB-SPECTRUM is nonnegative and discretely convex as a function of s. For positive eigenvalues this follows from the convexity of an exponential in s. Zero eigenvalues follow by limits, with zero raised to power zero interpreted as the identity in the corresponding transfer factor. Stationarity gives $C_q(n-s)=\overline{C_q(s)}$ and the spectral formula is real on the separated interval. Thus $C_q(s)$ decreases from w to $\lfloor n/2\rfloor$. Regardless of separation, Cauchy–Schwarz gives $|C_q(s)|\le C_q(0)$.

**Sum in one direction.** The nonnegative spectral density of the chosen orientation is
$S_\nu(p_j,q)=\sum_s e^{ip_js}C_q(s)$.
Separate the at most $2w-1$ short separations from the two monotone intervals. For a monotone nonnegative sequence bounded by $C_q(0)$, summation by parts bounds its Fourier sum on any interval by $2C_q(0)/|1-e^{ip_j}|$. Hence for $p_j\ne0$,
\[
S_\nu(p_j,q)\le
\left(2w+2|\sin(p_j/2)|^{-1}\right)
\frac1n\sum_{k=0}^{n-1} S_\nu(2\pi k/n,q).
\tag{ONE-AXIS-SUS}
\]
The inverse Fourier identity gives the displayed average $C_q(0)$. The argument permits a different fixed w for each orientation and choice of time axis. Use the largest of these finite widths.

Iterate ONE-AXIS-SUS in each coordinate. The average over all four momenta is the single-site variance, bounded by TORUS-LOCAL-MOM. This proves
\[
S_\nu(p)\le C_\sigma\prod_{j=1}^4
\left(2w+2|\sin(p_j/2)|^{-1}\right)
\tag{PRODUCT-SUS}
\]
whenever all four factors are finite. The spectral covariance matrix across orientations is positive and its largest eigenvalue is at most its trace. This proves OFF-PLANE-SUS.

Each positive summand $J_1,J_2,K_2$ in TWO-STEP-WILSON is dominated in quadratic-form order by the original covariance. Thus OFF-PLANE-SUS separately bounds every actual innovation and the twice-retained ordinary source on these plane waves, even when a selected grid does not commute with fine translations. Fourier diagonalization of the original covariance extends the result to all marks supported in this momentum region.

A further uniform consequence applies to any mark of the form
$f=\nabla_1\nabla_2\nabla_3\nabla_4 g$ with unit-lattice differences. Its Fourier multiplier vanishes on each coordinate momentum plane. Multiplying PRODUCT-SUS by its squared modulus gives a bounded function on the complement, so $\operatorname{Var}(r_f)\le C_\sigma\|g\|_2^2$. This is a difference-norm estimate. The constant for the unfiltered marks in OFF-PLANE-SUS deteriorates as $\delta$ tends to zero. Fixed physical momenta approach the coordinate planes as a tends to zero. Those directions and the constant source still require additional control.

### 4.30 Reduction of full susceptibility to finitely many periodic source patterns (P)

The slab argument gives a stronger consequence if one first samples a fixed sublattice. Choose a fixed integer stride m at least the largest slab width w in §4.29. Assume $m\mid n$ and take $n/m\ge2$. On a native sequence one may choose $m=L^s$ with fixed s large enough for the stencil, whenever the stated divisibility holds. Define the finite reciprocal grid
\[
\mathcal A_m=\left\{2\pi(k_1,k_2,k_3,k_4)/m:
0\le k_i<m\right\}.
\]
For each individual bond orientation $\nu$, the exact full Wilson spectral covariance satisfies
\[
\sup_p S_\nu(p)\le \sum_{h\in\mathcal A_m}S_\nu(h).
\tag{FINITE-GRID-SUS}
\]
The finite grid depends on the fixed stencil, not the ultraviolet cutoff.

**Proof.** Sample $r_{my,\nu}$ on the sublattice of spacing m and write its scalar spectral density as $S_\nu^{[m]}(q)$. The sampled transverse Fourier sum in any chosen time direction still lies in a slab of original width w. At every nonzero sampled separation s, the two original slabs have disjoint interiors because
$m\le ms\le n-m$.
SLAB-SPECTRUM consequently gives $C^{[m]}_{q_\perp}(s)\ge0$ for every such s. The diagonal term is an ordinary variance. Hence
\[
S_\nu^{[m]}(q_j,q_\perp)\le S_\nu^{[m]}(0,q_\perp)
\]
for every q. Apply the argument successively in all four directions to obtain $S_\nu^{[m]}(q)\le S_\nu^{[m]}(0)$.

The Fourier identity for sublattice sampling is
\[
S_\nu^{[m]}(mp)=m^{-4}\sum_{h\in\mathcal A_m} S_\nu(p+h).
\]
Indeed the reciprocal-grid sum of characters is m⁴ on original displacements belonging to the sampled sublattice and zero on the remaining displacements. Every term is a scalar variance and nonnegative. Thus
\[
S_\nu(p)\le m^4S_\nu^{[m]}(mp)
\le m^4S_\nu^{[m]}(0)
=\sum_{h\in\mathcal A_m} S_\nu(h),
\]
as claimed. This proof uses no spatial decay estimate. It also applies to the frustration observable h with its same reflection property.

The covariance matrix across bond orientations has largest eigenvalue at most $\sum_\nu S_\nu(p)$. It follows that uniform bounds for the finitely many numbers $S_\nu(h)$, $h\in\mathcal A_m$, imply the full extensive ordinary susceptibility for every real mark. Necessity follows immediately by testing those plane waves. Every positive covariance term generated by any number of actual retained-state constraints then satisfies the same uniform quadratic-form bound.

**Sharpened complex-source input.** Under REG, impose the zero-free hypothesis of Theorem 3.4 only on the real and imaginary parts of the single-orientation frustration marks at momenta in $\mathcal A_m$. Let the minimum of their cutoff-uniform radii be $R_m>0$. The proved real pressure estimate and H-ROW bound give
\[
S_\nu(h)\le 8A_\sigma/R_m^2+C_{\mathrm{W},\sigma}.
\]
Consequently FINITE-GRID-SUS and Fourier diagonalization prove
\[
\operatorname{Var}(r_f)\le
4m^4(8A_\sigma/R_m^2+C_{\mathrm{W},\sigma})M_f.
\tag{FINITE-ZF-IMPLIES-SUS}
\]
For the physical source the right side is multiplied by $c_\beta^{-2}a^{-4}$. On the even block tilings of §4.22, OFF-PLANE-SUS already supplies the required bounds for all $h\in\mathcal A_m$ with every component nonzero, with a constant depending on m. Thus only the finite set with at least one zero component, including h=0, needs additional control. A direct real variance estimate on these modes can be used in place of complex zero-freeness.

For $m=L^s$, each remaining mark is periodic on a fixed number s of native scales. After those s blockings, a simultaneous translation by one coarse block preserves the entire source pattern. This reduces the number and spatial dependence of the retained rows that must be propagated. The initial patterns still oscillate on the original lattice spacing, and their effective action, field-dependent lower rows and scalar responses still require quantitative bounds. The source norm of I-1 does not automatically bound them.

### 4.31 Consuming the two-step clean expansion and matching separated reflections

T1 §7.21, Theorem 7.37, constructs a localized source logarithm for the two original clean integrations with terminal field I, using JOINT-RESERVE and a direct-sum Gaussian comparison. Here its use is conditional on that two-species transfer of the native expansion with both original selectors. The consequences below specify the actual conditional variance rows furnished by this input.

Let $\mu_{2,I}^{\rm clean}$ be the normalized, real, two-step constrained joint law with both clean selectors and terminal field I. It includes the intermediate field $W_1$ as an integrated variable. By the single-factorial polymer derivative estimate, the ordinary unscaled second-source matrix of this law obeys
\[
\sup_b\sum_c e^{\alpha d(b,c)}|K^{\rm clean}_{2,I}(b,c)|\le C_L
\tag{JOINT-CLEAN-KERNEL}
\]
for a positive rate in original lattice units. To apply the frustration theorem to the ordinary source, replace its local quadratic seed by $\beta D_b$ in JOINT-FRUSTRATION. The Casimir companion has a deterministic identity part, and its difference from that part is a fixed sum of compact plaquette excesses by the Casimir identity. It also fits the joint quadratic reserve, with its explicit smaller coupling factor. The remaining source-free Gaussian, Jacobian and selector comparison is unchanged by this replacement. Equivalently one can rerun the stated two-species theorem with these displayed source coefficients. Extract the deterministic identity exponential before estimating the connected logarithm.

For every original mark f the two actual clean variances satisfy
\[
\begin{split}
&\mathbb E_{\mu_{2,I}^{\rm clean}}\!
\operatorname{Var}(r_f\mid W_1)
+\operatorname{Var}_{\mu_{2,I}^{\rm clean}}\!
\left(\mathbb E[r_f\mid W_1]\right)\\
&\hspace{30mm}=\operatorname{Var}_{\mu_{2,I}^{\rm clean}}(r_f)
\le C_L M_f .
\end{split}
\tag{CLEAN-TWO-INNOVATIONS}
\]
Both terms are nonnegative and each has the same individual bound. This computes what happens to the first retained source in the second integration. One only needs the absolute kernel of the *complete* two-step covariance to deduce these quadratic-form estimates. An absolute entrywise tree bound for the two individual conditional matrices would be a further assertion, since they can cancel entrywise outside the diagonal. The conditioning and all denominators in this identity belong to the same real constrained law.

For physical H sources at fixed positive and reflected supports separated by length d, JOINT-CLEAN-KERNEL gives an exponentially small two-step connected kernel at that flat terminal field. In the normalization of §2.3 one concrete bound for uniformly bounded marks is
\[
\left|\operatorname{Cov}_{\mu_{2,I}^{\rm clean}}
(r_H(f),r_H(\theta g))\right|
\le C_L c_\beta^{-2} a^{-4}n^4
\|f\|_\infty\|g\|_\infty e^{-\alpha d/a}.
\tag{CLEAN-SEPARATED}
\]
The polynomial factors are explicit and the right side tends to zero at fixed physical d when $c_\beta^{-1}$ is bounded or grows at most polynomially along the trajectory. This is the conditional fluctuation contribution with a fixed terminal field, not a positive lower bound for the physical reflected Gram. A nonflat terminal law contributes the covariance of its retained means.

For the original full Wilson law a different exact two-step matching is available with the nested reflection-symmetric collars of §4.26. Assume that the large cell side is fixed in lattice units, that the grid is invariant under the chosen site reflection, and that the positive and negative supports are physically separated by more than the largest cell diameter including its collar. Conditional on the retained collars, a source and its reflected partner then depend on disjoint open interiors, with all common collar links fixed. Thus their conditional covariance is zero. If $A$ is the original positive-time observable and $A_2=\mathbb E(A\mid\mathcal C_2)$, reflection symmetry gives
\[
G^\theta(A,A)
=\operatorname{Cov}(\overline{\theta A_2},A_2).
\tag{COLLAR-REFLECTION-MATCH}
\]
This holds jointly for any finite family with the stated separation, including their actual operator normalization factors. Conditional means of local summands use only the collar around their contributing cells, so $A_2$ still has positive-time support with a microscopic collar enlargement. Equation COLLAR-REFLECTION-MATCH transports the separated Gram exactly in this full positive disintegration. Its strictly positive lower eigenvalue remains to be proved for the retained means at fixed physical scale. The native averaged constraints require a corresponding all-history separated-kernel estimate before the same matching can be inferred from CLEAN-SEPARATED.

### 4.32 A single real replicated mark suffices (P)

The finite reciprocal-grid sum in FINITE-GRID-SUS is itself the variance of one real periodic mark. Its positivity and the orientation symmetry reduce the remaining source input further.

Fix one bond orientation $\nu_0$. With common stride $m\mid n$ as in §4.30 define
\[
f^{\rm comb}_{x,\nu}
=1_{\{\nu=\nu_0\}}1_{\{x\in m\mathbb Z^4\}},\qquad
N_{\rm cell}=(n/m)^4.
\]
Then
\[
S_{\nu_0}^{[m]}(0)
=N_{\rm cell}^{-1}\operatorname{Var}(r_{f^{\rm comb}}).
\]
Combining this with the maximum-at-zero property of the sampled spectrum gives
\[
\sup_p S_{\nu_0}(p)
\le m^4N_{\rm cell}^{-1}
\operatorname{Var}(r_{f^{\rm comb}}).
\tag{ONE-MARK-DOMINATION}
\]
All four orientations have the same bound, because coordinate permutations preserve the Wilson measure and permute the three matching actions. Taking the trace of the positive Fourier polarization matrix now proves that
\[
\operatorname{Var}(r_{f^{\rm comb}})\le B N_{\rm cell}
\quad\Longrightarrow\quad
\operatorname{Var}(r_f)\le 4m^4 B M_f
\quad\hbox{for every real mark }f .
\tag{ONE-MARK-SUS}
\]
Conversely the full susceptibility bound immediately gives the left-hand condition. Thus the missing real estimate has been reduced to one fixed, nonnegative microscopic pattern. Its source order and pattern size are independent of a.

The same argument works on a rectangular sublattice with fixed strides $m_j\ge w$, $m_j\mid n$. Replace $m^4$ by $m_\Pi=\prod_jm_j$ and $N_{\rm cell}$ by $n^4/m_\Pi$. For another bond orientation permute the whole rectangle together with its oriented mark. Only the one original scalar bound is required.

There is a literal chessboard realization. Choose $m_{\nu_0}$ odd so the center of an oriented bond lies at the midpoint between the two site-plane faces in that direction. Choose the other three strides even so the transverse site coordinates lie at the midpoints of those faces. Place the original stencil at this common rectangular center. Neighboring block reflections preserve the marked observable, including the link reversal along its own orientation. Its full dissemination is exactly the positive periodic mark above, up to a translation. Take an even number of rectangles per direction when invoking the usual chessboard convention. For example, on compatible reference tori a sufficiently large fixed odd $L^s$ and transverse strides $2L^s$ realize this pattern. A common uncentered stride is already sufficient for ONE-MARK-SUS and needs no chessboard interpretation.

**One complex disc.** The sole extra zero-free hypothesis sufficient for SUS on these tori is now
\[
\mathbb E_{\mu_a}\exp(z h_{f^{\rm comb}})\ne0
\quad (|z|<R)
\tag{COMB-ZF}
\]
for one $R>0$ independent of a. The real pressure of this mark is controlled. Under REG one may use §4.11 and $n^4=m_\Pi N_{\rm cell}$. On the tilings of §4.22 there is also a direct marked-set proof. Each $h_b$ is bounded by $C\beta$ times the sum of finitely many neighboring plaquette excesses. A plaquette has bounded overlap in these stencils. MARKED-EXP gives
$\log\mathbb E\exp(R_* h_{f^{\rm comb}})\le C N_{\rm cell}$
for fixed $R_*>0$. Since the mark and h are nonnegative, the same bound controls the real part of the source logarithm on the complex disc whenever the logarithm exists there.

The harmonic coefficient estimate of §4.4 therefore gives
$\operatorname{Var}(h_{f^{\rm comb}})\le C_R N_{\rm cell}$.
H-ROW gives the corresponding ordinary variance by adding at most $C_{\rm W}N_{\rm cell}$. Applying ONE-MARK-SUS proves the full physical conclusion after multiplication by $c_\beta^{-2}a^{-4}$.

The replicated cell here has a fixed number of *lattice* spacings and physical side tending to zero. The original I-1 statement specifies a fixed polydisc for its admitted smeared sources and includes chessboard replicas, but supplies no quantitative source-norm identification for this particular microscopic rectangular seed. COMB-ZF becomes an I-1 consequence if that identification is proved with a radius independent of a. This is the exact remaining admissibility check. For the displayed physical $C^5$ source class of T1, there is a quantitative obstruction to identifying it by ordinary interpolation. Choose strides greater than five. A physical H test for $\lambda h_{f^{\rm comb}}$ has values $J_a=c_\beta a^2\lambda f^{\rm comb}$ at the lattice sites in its oriented component. Its fifth forward difference starting on a marked site has modulus $c_\beta a^2|\lambda|$, since the next five sites along the chosen coordinate are unmarked. The integral representation of a finite difference implies
\[
\|D^5J_a\|_\infty\ge c_\beta |\lambda|a^{-3}.
\tag{COMB-SMOOTH-COST}
\]
Therefore the stated physical smooth-source ball gives at best a shrinking radius of order $a^3$ through this interpolation. A separate microscopic seed estimate, or a proved matching after finitely many original blockings, is required. A bound for one seed in a fixed *physical* cell, with the number of fine sites diverging, would have a different normalization in ONE-MARK-DOMINATION.

### 4.33 The dimension gain in the retained Gaussian force row (P)

There is an additional decay factor beyond RETAINED-GAUSSIAN-VOLUME. It follows from the actual contour averages and the physical, divergence-free current. Use link-angle coordinates, the uniform full torus at the flat identity, and the physical quotient of the linearized Wilson action. Let $s=L^j$ be the blocking stride, with $j=1,2$ in the two-step calculation.

For each fine Fourier momentum, the Wilson Hessian H is proportional to $|\widehat q|^2$ on the transverse space and zero on gradients. Each matching Hessian $H_i$ is positive, annihilates gradients, and is bounded above by H. It therefore commutes with H in that Fourier fiber and
\[
\sum_i H_i^2\le H\sum_iH_i=H^2 .
\tag{MATCHING-FORCE-SUM}
\]
This is a flat physical identity, with the same fixed metric factor in all Hessians.

Write $Q_s$ for the composed native linearized average, $E_s$ for its minimizing extension and $\Gamma_s$ for the retained Wilson action Hessian on the coarse physical quotient. Then
\[
HE_sB=Q_s^*\Gamma_s B .
\]
The coarse current $\Gamma_s B$ is divergence-free by gauge invariance. The native linear contour average is a straight-path average plus a coarse gradient coming from its two endpoint contour frames. The latter vanishes against a divergence-free coarse current. The adjoint maps such a current to a divergence-free fine current, because it annihilates every fine gradient by endpoint gauge covariance. Thus the cancellation holds at each factor of the two-step composition.

In unweighted link-angle $\ell^2$ norms the straight one-step averaging matrix has absolute row sum L and column sum $L^{-3}$. A row averages $L^4$ parallel translated length-L paths. For any fine bond in a fixed orientation there are exactly L possible starts of such paths across all coarse blocks, each with coefficient $L^{-4}$. Schur's inequality gives operator norm at most $L^{-1}$. Composition and the endpoint cancellation give
\[
\|Q_s^*J\|_2\le s^{-1}\|J\|_2
\qquad (d_{\rm coarse}^*J=0).
\tag{CURRENT-DILUTION}
\]
The powers here use *link angles* and unweighted sums; the physical-measure adjoint convention in T2 §4.10 includes the compensating cell-volume ratio.

**Uniform physical curl lower bound.** The flat endpoint frames also cancel in the coarse curl. Its remaining straight square is the average of translates of a fine $s\times s$ square. Fill each such square by its $s^2$ fine plaquettes. This gives $d_{\rm coarse}Q_s=\mathcal R_{2,s}d_{\rm fine}$, where each nonnegative orientation-preserving averaging row has sum $s^2$. Every fine plaquette belongs to exactly $s^2$ translated squares when counted over the whole coarse grid and their starting offsets, each with weight $s^{-4}$. Thus the column sum is $s^{-2}$ and $\|\mathcal R_{2,s}\|_{2\to2}\le1$. In the unweighted link-angle convention this strengthens DIRECTIONAL-HESSIAN to
\[
S_{*,2}(B)\ge\tfrac{\tau}{2}\|d_{\rm coarse}B\|_2^2
\]
at every flat homogeneous blocking depth. The endpoint and volume factors cancel before applying Schur.

**Uniform upper bound for $\Gamma_s$.** For a coarse plane wave at $p\in[-\pi,\pi]^4$ lift to the fine branch $q=p/s$. Put
$D_s(u)=s^{-1}\sum_{k=0}^{s-1}e^{iku}$.
In orientation $\nu$, the straight averaged amplitude equals the fine amplitude multiplied, up to a phase, by
\[
s D_s(q_\nu)\prod_{\rho=1}^4D_s(q_\rho).
\]
For a composition this follows also from $D_{ab}(q)=D_a(q)D_b(aq)$. Endpoint terms are coarse gradients and therefore irrelevant in this physical quotient. Since
$|D_s(p_\rho/s)|\ge2/\pi$,
the corresponding fine amplitude is at most $C|B(p)|/s$. Its fine curl is at most $C|p||B(p)|/s^2$, and the fine-to-coarse site count ratio is $s^4$. The fine energy of this competitor is therefore bounded by $C|p|^2|B(p)|^2$ per coarse mode in the normalized Fourier convention. Superpose modes; taking real parts supplies a real competitor when needed. Minimization gives $\|\Gamma_s\|_{\rm op}\le C$, uniformly in s. Harmonic zero modes contribute no force.

Combining MATCHING-FORCE-SUM and CURRENT-DILUTION gives
\[
\sum_i\|H_iE_sB\|_2^2
\le\|Q_s^*\Gamma_s B\|_2^2
\le C s^{-2}\langle B,\Gamma_s B\rangle .
\]
With the whitened notation of §4.26 this proves
\[
\|P_j A_f P_j\|_{\rm op}\le C L^{-2j}\|f\|_\infty,\qquad
\operatorname{Var}\mathbb E(r_f^{(2)}\mid L_jZ)
\le C d_G n^4 L^{-8j}\|f\|_\infty^2 .
\tag{GAUSSIAN-FORCE-GAIN}
\]
The second inequality uses the retained rank $O(d_G n^4L^{-4j})$ and the exact quadratic variance. The deterministic identity and Casimir rows do not enter this variance. At the first two constraints the factors relative to the fine volume are respectively $L^{-8}$ and $L^{-16}$. This isolates the expected lower-row gain of this particular force-square observable. Nonlinear mixing into the action row and history-dependent means require their own estimates before this rate can be applied to the compact Wilson measure.

### 4.34 Nonflat two-step classical contact paid by actual Wilson energy (P)

There is a concrete comparison field for the native constraints. It controls the nonflat stationary-value part of the two-source innovation without a supremum over the canonical background radius.

Let $W$ be any real coarse configuration at stride $s=L^j$, $j=1,2$. Make a fine configuration $U^{\rm pr}(W)$ by setting every link inside each s-block to I. Give every crossing link in the face between two neighboring blocks the value of their prescribed coarse bond, with the corresponding orientation. All parallel crossings of that face have the same value. Every contour used in the native coarse average has its in-block pieces equal to I and its crossing equal to the prescribed bond. All words compared inside each logarithm are consequently I. The exact average equals W, including for a coarse bond far from I. For two steps this assertion holds successively at the L-block levels. The intermediate field is precisely the same face prolongation at its own scale. The two in-block averaged contour variables appearing in the axial penalties are I.

A fine plaquette crossing neither face, or crossing only one coordinate face, has trivial holonomy. A plaquette crossing both coordinate faces carries the original coarse plaquette word. In the remaining two coordinates there are $s^2$ copies. Hence in dimension four
\[
S(U^{\rm pr}(W))=s^2 S_{\rm coarse}(W),\qquad
\mathscr G_0(U^{\rm pr})=\mathscr G_1(M_1U^{\rm pr})=0 .
\tag{FACE-PROLONGATION}
\]
In particular the infimum of the physical constrained action, including these nonnegative gauge penalties with their actual positive coefficients, is at most $s^2 S_{\rm coarse}(W)$. This is an actual compact competitor for the original averages.

On a sufficiently small physical neighborhood of the identity the regular constrained minimizer has the same upper bound. To verify the comparison there, retain both independent coordinate species as in §4.28 with a small real terminal b. The zero-background augmented Hessian is positive with a volume-uniform inverse on those constraints. The fine conditional stationarity makes its two physical fluctuation blocks diagonal at the origin, with the bounded positive first-step coupling-ratio correction. The local coordinate maps and their tree-weighted derivatives imply a uniformly small Schur perturbation of this Hessian on a smaller physical neighborhood. Applying the contraction argument of §4.24 to both species gives a unique regular critical point there and a positive Hessian on a convex independent-coordinate ball containing it and the face prolongation for sufficiently small b. The augmented action at this minimum is bounded by that at the competitor. Based gauge variations put both in-block gauge coordinates of the critical point at I, first at the fine scale and then at the coarse scale with the fine representative restored. Thus, writing $U_*(W)$ for the regular fine representative,
\[
S(U_*(W))\le s^2 S_{\rm coarse}(W)
\tag{REGULAR-ENERGY}
\]
on this neighborhood. No claim on the probability of a globally small coarse chart is used.

Let $\mathcal H_f=\sum_b f_b h_b/\beta$ and tilt the constrained physical augmented action by $-z\mathcal H_f$. Write $\phi_*(W,z)$ for the critical value on this regular branch, and $H_{\rm fl}(W)$ for its unperturbed constrained augmented Hessian in the two physical fluctuation coordinate species. Differentiation at the true constrained critical point gives
\[
-\partial_z^2\phi_*(W,0)
=\langle D\mathcal H_f(U_*),
H_{\rm fl}(W)^{-1}D\mathcal H_f(U_*)\rangle .
\tag{REGULAR-CRITICAL-CONTACT}
\]
Here D differentiates in independent physical coordinates at fixed W. The identity follows by solving the differentiated critical equation once. It includes all derivatives of the coordinate map.

The first matching force in $\mathcal H_b$ is $O((\sum_{Y_b}s_p)^{1/2})$ and the derivative of a matching force is bounded. At the actual minimizer, the tree-weighted derivative of the original fine readout with respect to either independent coordinate gives
\[
|D_y\mathcal H_b(U_*)|
\le C_L e^{-\alpha d(y,b)}
\left(\sum_{p\in Y_b}s_p(U_*)\right)^{1/2}.
\]
Schur summation and the uniform inverse bound on the stated regular branch imply
\[
0\le-\beta\partial_z^2\phi_*(W,0)
\le C_L\beta\sum_b |f_b|^2
\sum_{p\in Y_b}s_p(U_*).
\tag{WEIGHTED-CRITICAL-CONTACT}
\]

Now take $W=W_j$ from the full real Wilson law and its local physical averages, with the hypotheses of TWO-AVERAGE-ENERGY. Let G denote the admitted regular neighborhood used above. COARSE-MARKED-EXP implies
$\beta\mathbb E S_{\rm coarse}(W_j)\le C_{j,L}(n/s)^4$.
Bound the source weights by their supremum, sum the finite overlaps and use REGULAR-ENERGY to obtain
\[
\mathbb E\big[1_G(-\beta\partial_z^2\phi_*(W_j,0))\big]
\le C_{j,L}\|f\|_\infty^2 n^4/s^2 .
\tag{ANNEALED-CRITICAL-CONTACT}
\]
For the periodic comb this is at most a fixed multiple of its $M_f=n^4/m_\Pi$. The estimate is for the actual stationary-value response on the specified part of the two-step constrained fiber. The determinant and integrated fluctuation responses, the complement of G, and the variance of $\mathbb E(r_f\mid W_j,H_j)$ are separate terms. Replacing the latter by the stationary value would discard a conditional mean required by TWO-STEP-WILSON.

### 4.35 A periodic reflected witness after all linearized blockings (P)

The fixed physical separation can be tested on the actual linearized block averages rather than on a fixed microscopic eigenmode. Let the coarse stopping torus have $N_*=t^*/\ell_0$ sites in each direction, $N_*\ge4$, and let $s=L^K$ be the fine-to-coarse stride. Use the canonical flat Wilson Gaussian on the physical quotient. Choose the nonzero coarse spatial momentum $k=2\pi/N_*$ along axis 1 and a positive time slice j with $j-\frac12>0$, $j+\frac12<N_*/2$. The spatial magnetic curl $F_{12}$ at slice j, after the original linearized contour averages, has fine support strictly in the positive half.

Let $Y_j^A$ be its real cosine Fourier mode in color A with spatial $\ell^2$ normalization. Translates of the cosine or a sine give the same covariance. The endpoint contour frames in the averaged links are a coarse gradient and disappear from the curl. In coarse Fourier space the second term of $d_{12}A$ vanishes because the second spatial momentum is zero. The remaining multiplier is $e^{ik}-1$ times the averaged second link component.

To compute the exact covariance, put
\[
q_r=(k+2\pi r)/s\pmod {2\pi},\quad 0\le r<s,\qquad
\cosh\omega_r=1+\tfrac12|\widehat q_r|^2,\qquad
\widehat q=2\sin(q/2).
\]
The transverse spatial aliases in directions two and three other than zero are killed by their block factors $D_s(2\pi r/s)$. Thus the surviving fine potential component is transverse to its spatial momentum. Its periodic time Green function is
\[
G_{n,\omega}(t)=
\frac{e^{-\omega t}+e^{-\omega(n-t)}}
{2\sinh\omega(1-e^{-\omega n})},\quad
0\le t\le n,\qquad n=sN_* .
\]
This follows by summing the integer translates of the infinite-line Green function $e^{-\omega|t|}/(2\sinh\omega)$, or by direct substitution in its difference equation.

Spatial Fourier normalization gives a factor $s^{-3/2}$ between fine and coarse normalized modes. The averaged longitudinal path contributes s, since its momentum in direction two is zero. The amplitude for each spatial alias is therefore $s^{-1/2}D_s(q_r)$ up to a unit phase. The temporal block average is uniform over s original time layers. Consequently, for a unit color component,
\[
c_s(j)=\mathbb E_G(Y_j^A Y_{-j}^A)
=\frac{|\widehat k|^2}{\tau s}
\sum_{r=0}^{s-1}|D_s(q_r)|^2
\frac1{s^2}\sum_{u,v=0}^{s-1}
G_{sN_*,\omega_r}(2sj+u-v).
\tag{PERIODIC-BLOCK-CROSS}
\]
The time arguments are interpreted cyclically. The magnetic component is even under time reflection. All terms in the sum are nonnegative. No harmonic fine mode enters at this nonzero coarse momentum.

The term $r=0$ suffices for a uniform lower bound. One has $|D_s(k/s)|\ge2/\pi$, $\omega_0\le k/s$ and $s\sinh\omega_0\le Ck$. All unreduced positive time separations are at most $s(2j+1)$ and smaller than the period by the choice of j. It follows that
\[
c_s(j)\ge c_*=
\frac{c|\widehat k|^2}{\tau k}e^{-k(2j+1)}>0
\tag{PERIODIC-BLOCK-LOWER}
\]
independently of s. The same-slice variance $\sigma_s^2$ has a uniform upper bound. Indeed each nonzero alias has principal absolute momentum at least $k/s$, so $s\sinh\omega_r\ge c k$ and $sN_*\omega_r\ge c N_* k$. Moreover $\sum_r|D_s(q_r)|^2=1$ by finite Fourier orthogonality. The formula with zero coarse time separation therefore gives $\sigma_s^2\le C_{N_*,\tau}$. It also satisfies $\sigma_s^2\ge c_s(j)\ge c_*$.

For the color vector $Y_j$, the centered squared mode has exact Gaussian reflected covariance
\[
\operatorname{Cov}_G(|Y_j|^2,|Y_{-j}|^2)
=2d_G c_s(j)^2\ge2d_Gc_*^2 .
\tag{PERIODIC-BLOCK-GRAM}
\]
The spatially averaged positive magnetic energy also contains this mode. Complete its normalized real Fourier vector to an orthonormal basis. The covariance of two squared Gaussian modes is twice a squared cross covariance. Hence all terms in the reflected covariance of the sum of squares are nonnegative and the chosen mode gives a lower bound, with the fixed spatial averaging factor restored.

The Gaussian mean of the complete stopped magnetic energy is bounded uniformly in s. For a coarse link Fourier component use its straight representative. Each fine alias carries the four block-average factors and an additional path factor of modulus at most s. With unitary four-dimensional Fourier normalization the squared coarse amplitude relative to the fine one is bounded by $s^{-2}\prod_\mu|D_s(q_\mu)|^2$. Every nonzero fine mode has $|\widehat q|\ge c/(sN_*)$. The products of squared block factors sum to one over each alias fiber. Thus its covariance is bounded by $C N_*^2$ per coarse mode; bounded coarse curl multipliers and the fixed number of stopped sites finish the estimate. Endpoint frame terms are removed before this estimate by the curl.

PERIODIC-BLOCK-GRAM is a stopped-scale Gaussian statement for the periodic native averaging geometry. It corrects the scaling limitation of a fixed microscopic Dirichlet mode. Identifying these fields with a jointly transported physical composite in the actual Wilson law is still necessary.

### 4.36 A bounded-density event criterion for physical reflected nondegeneracy (P implication)

An actual reflected lower bound can be tested against a bounded event in the opposite half. This only requires a contrast of conditional means on the chosen event. It avoids the coincident ordinary variance of a renormalized local composite.

Let A be a real positive-time observable in the original Wilson algebra. Let C be an indicator in the same positive half, $E=\{\theta C=1\}$ and $p=\mathbb P(E)>0$. Reflection positivity and Cauchy–Schwarz on the centered reflected form give
\[
G^\theta(A,A)\ge
\frac{p}{1-p}
\left|\mathbb E(A\mid E)-\mathbb E A\right|^2
\qquad(0<p<1).
\tag{REFLECTED-EVENT}
\]
Indeed the mixed reflected entry is $p(\mathbb E[A\mid E]-\mathbb E A)$ and $G^\theta(C,C)\le\operatorname{Var}(C)=p(1-p)$. If the indicator has zero reflected norm its mixed entry is zero by the same inequality. Any harmless identity subtraction from A cancels in the contrast.

For a finite family $A_i$ use disjoint reflected events $E_j$ with probabilities $p_j>0$. Put $D_{ij}=\mathbb E(A_i\mid E_j)-\mathbb E A_i$. Positivity of the joint reflected Gram and the upper bound on the indicator Gram by its ordinary covariance yield
\[
G^\theta(A_i,A_k)\succeq D\,\operatorname{diag}(p_j)\,D^* .
\tag{REFLECTED-EVENT-MATRIX}
\]
To verify this even in singular cases, the ordinary indicator covariance is $\operatorname{diag}(p)-pp^*$ and is dominated by $\operatorname{diag}(p)$. Replacing the indicator diagonal block of the positive joint Gram by the larger strictly positive diagonal matrix preserves positivity. Its Schur complement yields the displayed inequality.

**A finite comparison window.** Use the periodic canonical Gaussian pair $X=Y_j$, $Y=Y_{-j}$ of §4.35, including all color components. Its conditional Gaussian mean is $\alpha_sY$, where $\alpha_s=c_s(j)/\sigma_s^2\ge\alpha_*>0$. Its conditional covariance is bounded by $\sigma_{\max}^2 I$. Choose a fixed M large enough that
$\mathbb P_G(|X-\alpha_sY|\le M\mid Y)\ge3/4$
for every s, for example by the second-moment Markov inequality. For a fixed $R\ge2M/\alpha_*$ let
\[
E_R=\{R\le |Y|\le R+1\},\qquad
B_R=E_R\cap\{|X-\alpha_sY|\le M\}.
\]
The Gaussian probability of $E_R$ is bounded below by $p_*(R)>0$ independently of s. This follows from the explicit Gaussian density on the fixed annulus and $c_*\le\sigma_s^2\le\sigma_{\max}^2$.

Here is one sufficient *actual-law* comparison. Suppose the physical readouts X in the positive half and Y in the reflected half have
\[
\mathbb P_{\rm W}(B_R)\ge l\,\mathbb P_G(B_R),\qquad
\mathbb P_{\rm W}(E_R)\le u\,\mathbb P_G(E_R)
\tag{WINDOW-COMPARISON}
\]
with fixed $l,u>0$. Suppose a retained energy readout F is nonnegative on $E_R$, obeys $F\ge b|X|^2$ on $B_R$, and satisfies $\mathbb E_{\rm W}F\le M_0$. Then
\[
\mathbb P_{\rm W}(E_R)\ge\tfrac34 l p_*(R),\qquad
\mathbb E_{\rm W}(F\mid E_R)-\mathbb E_{\rm W}F
\ge\frac{3lb\alpha_*^2R^2}{16u}-M_0 .
\tag{WINDOW-CONTRAST}
\]
Indeed $|X|\ge\alpha_*R/2$ on $B_R$, and the ratio of the two displayed event probabilities is at least $3l/(4u)$. If the last right-hand side is a positive number $\delta$, choose the positive-half indicator whose reflection is $1_{E_R}$ and apply REFLECTED-EVENT.

This criterion permits order-one bounded changes in a finite comparison density. For example, a density ratio between two fixed positive constants on both required event probabilities gives fixed l,u; a sufficiently large fixed R then gives a positive contrast whenever $M_0$ is bounded. Only a finite annulus and its correlated partner window are used. No Gaussian lower density on the whole unbounded field space is required.

For the physical insertion write the proposed matched row as $A=zF+\mathcal R$ with $|z|\ge z_0>0$. It suffices to bound the actual separated error by
\[
|\mathbb E_{\rm W}(\mathcal R\mid E_R)-\mathbb E_{\rm W}\mathcal R|
\le z_0\delta/2 .
\tag{WINDOW-ERROR}
\]
REFLECTED-EVENT then gives $G^\theta(A,A)\ge (3lp_*(R)/4)(z_0\delta/2)^2$. Local diagonal contact terms cancel on the separated indicator product. If normalization leaves the leading amplitude of order $g_*^2$, the error contrast must retain that same amplitude, as in §4.12.

PERIODIC-BLOCK-CROSS verifies the reference response in this window for the original linearized periodic averages. I-0c gives a representation of the unmarked effective density, but does not itself state WINDOW-COMPARISON for these jointly transported physical readouts or WINDOW-ERROR for their operator row. An actual observable on the stopping variables must also be pulled back into the correct original positive or negative half. These are the remaining verification steps for this reflected criterion.

### 4.37 All complex source orders in the retained Gaussian precision (P)

The dimension gain in §4.33 persists for a finite complex source, including the nonnegative comb of §4.32. This concerns the flat Gaussian constrained law of the original linearized averages.

Use white coordinates Z and let P be the retained projection at stride $s=L^j$, $R=I-P$. Write A for the symmetric normalized quadratic source matrix, absorbing the fixed factor two so that its contribution to the exponent is $z Z^*A Z/2$. For the ordinary force row this is $2A_f$ of §4.26. For frustration one also subtracts the corresponding total-force matrix with coefficient one third. The Casimir row at this order is a scalar. The following estimates hold for both matrices:
\[
\|A\|_{\rm op}\le C\|f\|_\infty,\qquad
\|PAP\|_{\rm op}\le C s^{-2}\|f\|_\infty,\qquad
\|RAP\|_{\rm op}+\|PAR\|_{\rm op}\le C s^{-1}\|f\|_\infty .
\tag{FORCE-BLOCKS}
\]
For the last assertion, write each summand as $T_i^*FT_i$. Section 4.33 gives $\|T_i P\|\le Cs^{-1}$, while $\|T_i\|\le C$. The total force uses $T=H H^{+1/2}$ and has the same restricted bound by CURRENT-DILUTION. This proof also covers signed real marks, without a positivity assumption on their quadratic matrix.

For $|z|C\|f\|_\infty<1$, integrate the original R-fluctuation Gaussian exactly. Its determinant contributes the scalar factor $\det_R(I_R-z RAR)^{-1/2}$. Completing the square gives the retained white precision
\[
H_{\rm ret}(z)
=P-zPAP-z^2PAR(I_R-zRAR)^{-1}RAP
\quad\text{on }\operatorname{ran}P.
\tag{FORCE-SCHUR}
\]
The inverse and determinant branch are holomorphic on that disc. The Schur formula includes the entire cross response from the fluctuation mean shifted by the source. In particular,
\[
\|H_{\rm ret}(z)-P\|_{\rm op}
\le\frac{C'|z|\|f\|_\infty s^{-2}}
{1-C|z|\|f\|_\infty}.
\tag{COMPLEX-FORCE-GAIN}
\]
Every retained nonidentity coefficient of the Gaussian source logarithm inherits this dimension gain by Cauchy estimates. The scalar determinant has the actual trace multiplicity of the eliminated directions. It cannot be omitted from a two-source contact bound.

This computation holds for every depth of the homogeneous flat linearized averaging. The screened momentum row and its scalar determinant are now explicitly available as starting data for the nonlinear comb deformation. The interacting action and history-dependent scalar responses remain to be controlled in the original positive measure.

### 4.38 The smallest centered rectangle and its exact temporal transfer insertion (P)

For a bond in orientation $\nu_0$ the slab width along that orientation is one. Its incident plaquettes lie between the two endpoint site planes. In each transverse direction the slab width is two, since the plaquette star extends one site to either side. The proof of §4.32 only requires that the stride in each direction dominate its *own* slab width. Thus on every even torus we may use
\[
m_{\nu_0}=1,\qquad m_j=2\ (j\ne\nu_0),\qquad m_\Pi=8.
\]
The comb consists of all $\nu_0$ bonds whose three transverse site coordinates occupy one fixed parity class. It is present at every time step when $\nu_0$ is chosen as time. Its source is centered in a $1\times2\times2\times2$ rectangle, and on tori with $4\mid n$ it is an exact site-plane chessboard dissemination on an even factor torus. Translation of the transverse parity class changes no variance. The implication is now
\[
\operatorname{Var}(r_{f^{\rm comb}})\le B n^4/8
\quad\Longrightarrow\quad
\operatorname{Var}(r_f)\le32B M_f .
\tag{EIGHT-SITE-COMB}
\]
Along a transverse line its samples alternate 1 and 0. The absolute fifth forward difference at a marked site is 16, so COMB-SMOOTH-COST holds with the additional factor 16 for this choice.

There is an explicit one-step operator for this mark, independent of time. Write $\sigma,\sigma'$ for the spatial link configurations on neighboring slices and $u_x$ for their temporal links. Put
\[
K_\beta(\sigma,{\sigma'}^u)
=\exp[-\beta\sum_e s_e(\sigma,{\sigma'}^u)]
\]
for the full temporal-plaquette kinetic kernel, including its constant terms, and let $P$ integrate the slice gauge transformation u. Write $T=V^{1/2}K_\beta P V^{1/2}$ as in §4.29. At spatial site x let $D_{x,i}^A$ generate the site gauge variation on the two spatial links in direction i incident at x, acting on the second slice argument. Then $D_x^A=\sum_{i=1}^3D_{x,i}^A$ is the full site generator. These are skew-adjoint Haar derivatives. The partial-direction generator differentiates precisely the matching force on the two temporal plaquettes in its plane. Different orientations occur on disjoint spatial link sets at x.

For the temporal bond b at x, differentiate the exact kinetic exponential before performing the u integral. This gives
\[
r_b K_\beta
=\beta^{-1}\sum_{i,A}(D_{x,i}^A)^2 K_\beta
+\tfrac23\ell_b K_\beta,\qquad
t_b K_\beta
=-\frac1{3\beta}\sum_A(D_x^A)^2 K_\beta.
\tag{KINETIC-SEED}
\]
Indeed differentiating the exponential twice gives its force square times $\beta^2$, minus its action Hessian times $\beta$. The Casimir term in the ordinary definition subtracts one third of that Hessian. Integrating the second identity over $u_x$ gives zero, even at fixed endpoint slices and fixed other temporal links. Thus the ordinary and frustration first insertions give exactly the same one-slab kernel after this gauge projection.

Let $\mathscr E_x=-\sum_{i,A}(D_{x,i}^A)^2$ be the positive directional electric Casimir. Let $\dot K_x$ denote the derivative obtained by changing only the six temporal-plaquette coefficients incident at x from $\beta$ to $\beta+\lambda$ and differentiating at zero. Since
$\ell_b=C_F\sum_{e\ni x}(N-s_e)$,
the exact transfer insertion is
\[
O_x=-\beta^{-1}V^{1/2}K_\beta P\mathscr E_x V^{1/2}
+\frac{2C_F}{3}V^{1/2}(6N K_\beta+\dot K_x)P V^{1/2}.
\tag{TEMPORAL-ORDINARY-OPERATOR}
\]
To check the placement of the derivatives, integrate twice by parts on the second spatial slice. The kinetic convolution commutes with independent simultaneous left and right rotations of corresponding slice links. The sum of squared partial site generators is invariant under full slice gauge transformations, so it commutes with P. Spatial Wilson factors remain on their original sides of the operator. These identities hold first on smooth functions and hence for their finite-volume integrated kernels.

Sum $O_x$ over the selected spatial parity class to get the one-time comb operator O. If $A_t=\sum_{x\ {\rm marked}}r_{(t,x),\nu_0}$ and
$\widetilde O=O-(\mathbb E A_t)T$,
then for $1\le d\le n-1$ its exact connected covariance is
\[
\operatorname{Cov}(A_0,A_d)=
\frac1{\operatorname{Tr}T^n}
\sum_{\alpha,\gamma}
|\widetilde O_{\alpha\gamma}|^2
\lambda_\alpha^{\,d-1}\lambda_\gamma^{\,n-d-1}.
\tag{COMB-TRANSFER-SPECTRUM}
\]
The equal-time term uses the actual two-insertion kernel on one slab. At distinct times the terms in this formula are nonnegative. The desired variance is n times the sum of the equal-time term and these separated terms. This identifies the microscopic periodic source with a definite electric-current and local kinetic-coupling response in the physical transfer space. A uniform bound on that sum per selected spatial site, including near-degenerate transfer eigenvalues and the equal-time term, remains open.

### 4.39 Nonlinear Wilson matching forces and the two-step critical source gain (P)

There is a nonlinear estimate for the original matching forces. It uses the covariant difference algebra on the actual compact lattice and a cube identity. For every real Wilson field,
\[
\sum_{b,i}|F_{b,i}|^2
\le \sum_b |F_b|^2+C_N\sum_p s_p^{3/2}.
\tag{WILSON-FORCE-HODGE}
\]
In particular the error on a region of uniformly small plaquette excess is controlled by the small plaquette distance times the original action.

**Original Wilson differences.** Write
$P_{\mu\nu}(x)=U_\mu(x)U_\nu(x+\mu)U_\mu(x+\nu)^{-1}U_\nu(x)^{-1}$
and $\Omega_{\mu\nu}(x)=C_N(P_{\mu\nu}(x))$, with $C_N$ as in §2.1. These are alternating Lie-algebra-valued two-form components. Define the unitary parallel shifts on Lie-algebra fields by
$T_\mu v(x)=\operatorname{Ad}_{U_\mu(x)}v(x+\mu)$
and $D_\mu=T_\mu-I$. Differentiating the two plaquettes in a matching at the link $(x,\mu)$ gives, in generator coefficient norm, its force as
$-\tau D_\nu^*\Omega_{\mu\nu}(x)$,
where $\nu$ is the matched partner of $\mu$. The forward plaquette supplies its based force and the backward one supplies the oppositely signed parallel transport from $x-\nu$. Thus the total force is $\tau d_U^*\Omega$, where $d_U=\sum_\mu \varepsilon_\mu D_\mu$ and $\varepsilon_\mu$ is exterior multiplication. Since $D_\nu^*=-T_\nu^{-1}D_\nu$,
\[
\sum_{b,i}|F_{b,i}|^2
\le\tau^2\sum_\rho\|D_\rho\Omega\|_2^2.
\]

**Cube remainder.** Compare the path in three distinct directions $\lambda\mu\nu$ with the path $\nu\mu\lambda$ by the two possible sequences of three adjacent exchanges. One sequence produces the product of faces
\[
P_{\lambda\mu}(x),\quad
\operatorname{Ad}_{U_\mu(x)}P_{\lambda\nu}(x+\mu),\quad
P_{\mu\nu}(x);
\]
the other produces
\[
\operatorname{Ad}_{U_\lambda(x)}P_{\mu\nu}(x+\lambda),\quad
P_{\lambda\nu}(x),\quad
\operatorname{Ad}_{U_\nu(x)}P_{\lambda\mu}(x+\nu).
\]
The two ordered products are equal because each is the original path times the inverse final path. For $P\in SU(N)$ one has $P=I+C_N(P)+O_N(s(P))$ globally. The Hermitian remainder is quadratic in $P-I$, and the removed trace component of the anti-Hermitian part has vanishing first derivative on the special-unitary tangent. Compactness covers the complement of a chart. Expanding each three-factor product to first order now gives
\[
|(d_U\Omega)_{\lambda\mu\nu}(x)|
\le C_N\sum_{p\text{ on this cube}} s_p .
\tag{CUBE-REMAINDER}
\]
This is an estimate on the actual non-Abelian group words, including the transporting links. Finite overlap yields $\|d_U\Omega\|_2^2\le C_N\sum_p s_p^2$.

**Hodge identity.** Using $\iota_\nu=\varepsilon_\nu^*$ and the exterior anticommutator gives
\[
d_Ud_U^*+d_U^*d_U
=\sum_\rho D_\rho^*D_\rho+
\sum_{\mu,\nu}\varepsilon_\mu\iota_\nu[D_\mu,D_\nu^*].
\]
Each commutator of shifts compares two length-two paths with the same endpoints. Their ratio is a conjugate of one plaquette word, so its contribution to the quadratic form is bounded by fixed local sums of
$C\sqrt{s_p}\,|\Omega(x)|\,|\Omega(x')|$.
Since $|\Omega_{\mu\nu}|^2\le C s_{\mu\nu}$, Young's inequality and finite overlap bound the sum by $C_N\sum_p s_p^{3/2}$. Applying the identity to $\Omega$ and using CUBE-REMAINDER yields WILSON-FORCE-HODGE. The extra $\sum s_p^2$ is absorbed because $s_p\le2N$. No smoothness or small action was assumed in this global inequality.

**Constraint current at the regular minimum.** Now take the actual first or second physical average at stride $s=L^j$, $j=1,2$, and the regular Wilson representative $U_*(W)$ of §4.34. Use the exact left-trivialized derivative $\mathcal Q(U_*)$ of this average. Constrained stationarity and surjectivity in the physical chart give
\[
F_{\rm tot}(U_*)=\mathcal Q(U_*)^*J,\qquad
J=\nabla_W S_*(W)
\]
with the same fixed metric normalization on both gradients. The based-gauge term vanishes at this representative. Coarse gauge invariance gives the exact covariant divergence equation for J. On $\|\log W\|_\infty\le\delta_s$ its ordinary divergence therefore obeys
$\|d^*J\|_2\le C\delta_s\|J\|_2$.

The local finite-range average and its adjoint differ from their flat linearizations by at most $C_s\delta_s$ in operator norm, because the minimizing link logarithms and their finite determining stencils are $O_s(\delta_s)$. The flat endpoint contour part pairs with $d^*J$ and has finite norm $C_s$. CURRENT-DILUTION for the remaining straight part consequently gives
\[
\|F_{\rm tot}(U_*)\|_2
\le(s^{-1}+C_s\delta_s)\|J\|_2 .
\tag{REGULAR-CURRENT-DILUTION}
\]
No endpoint coefficient is discarded. For the two-step composition the output of the first adjoint is covariantly divergence-free at its own intermediate field, or equivalently one can compare the complete finite-range composite derivative to $Q_s$ at once.

The physical coarse action has Hessian at zero $\Gamma_s$ with the uniform upper bound of §4.33. Its local analytic chart and tree summability in §4.28 give
$\|\nabla_b^2 S_*(b)-\Gamma_s\|_{2\to2}\le C_s\|b\|_\infty$:
differentiate the local scalar action after the minimizing substitution and anchor the two differentiated indices before summing the absolutely convergent coefficients. Thus on a smaller neighborhood the Hessian norm is at most a fixed $M>0$ independent of s, with the size of the neighborhood allowed to depend on s. Since $S_*\ge0$, Taylor's inequality applied at $b-M^{-1}\nabla_b S_*(b)$ gives $\|\nabla_b S_*(b)\|_2^2\le2M S_*(b)$. To ensure that point stays in the chart, first fix its Hessian neighborhood and then shrink the admitted b-radius. The local derivative bound gives $\|\nabla_b S_*(b)\|_\infty\le C_s\|b\|_\infty$. The left-trivialized current has the same estimate up to a fixed coordinate factor.

Every minimizing plaquette has $\sqrt{s_p}\le C_s\delta_s$ in this chart. Shrink the fixed positive radius so the current error is at most $s^{-1}$ and the plaquette error at most a fixed multiple of $s^{-2}$. WILSON-FORCE-HODGE yields
\[
D(U_*)=\sum_{b,i}|F_{b,i}(U_*)|^2
\le C s^{-2}S_*(W).
\tag{NONLINEAR-CRITICAL-FORCE-GAIN}
\]
The contraction factor has an s-independent prefactor for these two fixed strides. Its admissible physical radius can depend on s. This distinction matters for any proposed iteration through unbounded depth.

**Finite complex source at the classical saddle.** For $|f_b|\le1$, $|\mathcal H_f(U_*)|\le D(U_*)$. The derivative of the frustration polynomial retains a first matching force. With the true constrained readout of §4.28, Schur summation gives
\[
\|D_y\mathcal H_f(U_*)\|_2\le C_s D(U_*)^{1/2}.
\]
The fixed-radius analytic Hessian bounds and positive regular inverse give a unique nearby holomorphic critical point $y_z$ for the phase $\mathscr S-z\mathcal H_f$. In physical coordinates its shift satisfies
\[
\|y_z-y_0\|_2
\le C_s|z|\|D_y\mathcal H_f(U_*)\|_2.
\]
One obtains this by integrating the Hessian along the short complex segment from $y_0$ to $y_z$ and inverting a small perturbation of the original constrained Hessian. Existence and control in the common $\ell^\infty$ chart follow by the same local analytic contraction, with z small independently of volume. Taylor's formula for the critical phase thus gives
\[
|\phi_*(W,z)-S_*(W)|
\le |z|D(U_*)+C_s|z|^2D(U_*).
\]
On a fixed sufficiently small $|z|<r_s$, NONLINEAR-CRITICAL-FORCE-GAIN proves
\[
|\phi_*(W,z)-S_*(W)|\le C |z|s^{-2} S_*(W).
\tag{NONLINEAR-CRITICAL-DISC}
\]
Here $r_s$ is chosen to absorb the displayed $C_s|z|$ factor. This is a nonlinear irrelevance estimate for the actual critical scalar. It uses the true plaquette forces and the constrained Wilson minimizer.

Combining the sharper derivative bound with FACE-PROLONGATION gives
\[
\mathbb E[1_G|\beta\partial_z\phi_*(W_j,0)|]
+\mathbb E[1_G|\beta\partial_z^2\phi_*(W_j,0)|]
\le C_{j,L}(n/s)^4
\tag{COARSE-VOLUME-CRITICAL}
\]
for the comb or any real $|f_b|\le1$ in the two-step setting of §4.34. The first derivative costs $\beta D(U_*)$. The second costs $C_s\beta D(U_*)$ by REGULAR-CRITICAL-CONTACT. The remaining expectation of $\beta S_{\rm coarse}(W_j)$ is bounded by COARSE-MARKED-EXP. The integrated fluctuation determinant, cutoff terms, nonregular sectors and covariance of the retained conditional mean are additional contributions to the actual susceptibility.

### 4.40 Gauge-invariant vacuum subtraction bounds the first clean fluctuation row by the physical action (P implication)

Let $F_X(U,J)$ be localized scalar activities on a periodic unit grid with $n_0$ sites per direction. Assume a uniform bound $|F_X|\le a_X$ on the admitted external domain, including a fixed small complex ball at $(I,0)$, and
\[
\sup_x\sum_{X\ni x}e^{\kappa d(X)} a_X\le A .
\]
The carrier is connected, includes all determining links and endpoints, and its geometric diameter is bounded by $C(1+d(X))$. Let the physical current satisfy
$|J_x(U)|^2\le C_J\sum_{p\in Y_x}s_p(U)$
on a fixed stencil in these units. The native physical current at one fixed scale has this property because it is a finite covariant difference of plaquette forces. Fixed mesh conversion factors are retained in $C_J$.

Suppose the total activity is gauge-invariant. Average each term over compact site gauges in its determining set and endpoint collar. Gauge covariance of the total and the gauge-invariant external domain preserve the sum and its rooted majorant, so one may take the terms individually invariant. Then for every admitted real configuration,
\[
\left|\sum_X
[F_X(U,J(U))-F_X(I,0)]\right|
\le C A\, S(U)+ C A\, n_0^4 e^{-c n_0}.
\tag{POLYMER-ENERGY-SUBTRACTION}
\]
The constants depend on the fixed physical Cauchy radius, stencil, grid conversion and spare carrier exponent. The last term explicitly retains carriers that can wind around the torus.

**Proof.** Take a nonwinding carrier of diameter $D_X=C(1+d(X))<n_0/4$ and a contractible bounding rectangle $Y_X$ with fixed stencil collar. Gauge-fix a coordinate spanning tree in this rectangle. Each remaining link is a tree loop that can be filled by at most $C D_X^2$ plaquettes with bounded multiplicity by successively moving its coordinate path. The product inequality for unitary matrices and Cauchy–Schwarz yield
\[
\max_{e\in X}\|U_e^g-I\|^2\le C D_X^2\sum_{p\in Y_X}s_p .
\]
This gauge transformation is used only to evaluate a gauge-invariant activity. The current transforms in the adjoint representation and satisfies the same local energy bound.

At the identity the linear Taylor coefficient of a gauge-invariant scalar in the link logs and current coordinates vanishes. A constant site gauge acts by the adjoint representation on every such slot, which has no invariant linear functional on $\mathfrak{su}(N)$. If the displayed energy is small enough to put the local variables inside half the fixed Cauchy radius, Taylor's formula in their common direction gives
\[
|F_X(U,J(U))-F_X(I,0)|
\le C a_X D_X^2\sum_{p\in Y_X}s_p .
\]
The physical current may be varied as an independent extended variable on this Cauchy line. If that energy threshold fails, the same bound follows by enlarging C and using the two absolute bounds $a_X$.

For each fixed plaquette p in $Y_X$ there is a carrier site x at distance at most $C D_X$. Spend part of the exponential carrier weight on this distance and on $D_X^2$. Then the rooted sum at x is bounded by A and the remaining sum over x by a uniform exponential shell sum. This bounds the total coefficient of $s_p$ by $CA$. Carriers without a contractible bounding rectangle of the indicated size have $d(X)\ge c n_0-C$, including carriers with nontrivial winding. Their two absolute values sum to at most $CA n_0^4e^{-c n_0}$. Such a term really can distinguish a flat winding holonomy and so should not be absorbed into S. This proves POLYMER-ENERGY-SUBTRACTION.

**First clean source application (P/L on the admitted orbit domain).** T1 Proposition 7.67 checks invariance of the actual localized tagged terms from T1 Theorems 7.44 and 7.57. The contracted matching forces, covariant Gaussian walks, unique sourced saddle and signed spheres all respect the simultaneous site rotations. The carrier support and its bound survive orbit extension on the native domain. The same property for the original unmarked scalar expressions is established in the closing paragraph of [Balaban, CMP116, pp. 21–22](https://doi.org/10.1007/BF01239022). Use only the first regular fiber with the fixed physical analytic slack, orbit intersection and carrier margins of those theorems. Its fluctuation logarithm $L(W,z)$ after the critical scalar has rooted majorant $A=C_L|z|$ on the actual minimizing data $U_*(W),J(U_*(W))$. The unsourced value of this particular source difference vanishes. Apply POLYMER-ENERGY-SUBTRACTION on the original determining grid and use $S(U_*)=S_*(W)$. This gives
\[
|L(W,z)-L(I,z)|
\le C_L |z| S_*(W)+ C_L |z|n^4e^{-c_L n}.
\]
For the comb mark on the smaller common real regular chart, combine this with NONLINEAR-CRITICAL-DISC at $s=L$. The first clean conditional source ratio, denoted $Z_{1,W}(z)/Z_{1,W}(0)$, then satisfies
\[
\left|\log\frac{Z_{1,W}(z)}{Z_{1,W}(0)}
-\log\frac{Z_{1,I}(z)}{Z_{1,I}(0)}\right|
\le C |z|\bigl(L^{-2}+C_L/\beta\bigr)\beta S_*(W)
+C_L|z| n^4e^{-c_L n}.
\tag{FIRST-NONIDENTITY-COMB}
\]
This compares the actual integrated clean row at nonflat W with its identity value. Its field-dependent classical part gains $L^{-2}$, and its fluctuation part relative to the canonical action gains $\beta^{-1}$. Cauchy on the spare z-disc gives the corresponding fixed first and second row bounds. The identity derivatives are separately retained in the pressure and contact tower.

The fixed physical Cauchy radius is essential. On a mixed record with only a shrinking external-field radius $\alpha_k$ the two-jet estimate has an additional factor $\alpha_k^{-2}$. The present proof therefore does not assert the same $O(g_k^2)$ coefficient on those records without a matching domain or reserve estimate.

### 4.41 Uniform classical action on a finite periodic stopping window (P/L)

A primary variational estimate identifies the classical action in the reflected comparison window more precisely. Use the homogeneous, full native hierarchy, fixed stopped side $N_*=t^*/\ell_0$ and fine mesh $\eta=s^{-1}=L^{-K}$ in stopped units. The action and the averages here are the original regular classical ones used in CMP109 (1.1) and (2.2).

The parameter and domain checks use [Balaban, *The Variational Problem and Background Fields in Renormalization Group Method for Lattice Gauge Theories*](https://doi.org/10.1007/BF01229381), Theorem 1, equations (2), (5), (7)–(10), and Proposition 9 with (19)–(21), (172)–(173). The relevant statements are on printed pages 279 and 309. Take all localization domains to be the full torus, with the author's fixed blocking parameters and required native big-block compatibility. At the coarse real base $V_0=I$ the regular-orbit and small-plaquette conditions hold. Fix an admissible $\epsilon_1$ below the constants of Theorem 1. Proposition 9 supplies a complex perturbation $V'=e^b$ on a fixed sufficiently small $\|b\|_\infty<\delta$ independent of K. The relative field in its prescribed gauge is $e^{i\eta\mathcal A}$ and (19), (173) give $|\mathcal A|\le C\epsilon_1$ and $|\nabla^\eta\mathcal A|\le C\epsilon_1$ on the homogeneous unit-scale region. Here $\delta$ implements (172); it is not a canonical radius growing with $s$.

**Periodic restriction of the regular orbit.** If additional room is required for the native big cubes, take a finite compatible periodic cover of the stopped torus and repeat the deterministic target on it. The homogeneous variational equations and constraints are translation covariant. A translation by an original period therefore preserves the unique regular critical orbit on the cover. To obtain an exactly periodic representative, choose inside each coarse block one fine spanning tree rooted at its coarse center, translated with the blocks. In any orbit of the based gauge group there is exactly one representative with these tree bonds equal to I. The translation preserves this gauge, so uniqueness of the orbit gives equality of the translated representatives. Restriction to the original period is a regular critical point there.

Conversely a periodic critical point on the smaller torus lifts to a critical point on the cover. Indeed average any tangent variation on the cover over translations by the smaller periods. At the periodic field it remains tangent to the linearized constraints. The action derivative on the original variation equals its value on the averaged variation, which is zero by the smaller-torus critical equation. Uniqueness on the cover and the based tree gauge therefore also identify the restricted critical orbit uniquely. The scalar action on repeated fields is exactly the number of periods times its value on one period. For complex perturbations the corresponding scalar identity follows by analytic continuation from the real chart. This construction concerns the deterministic variational problem alone. It involves no product or comparison of quantum partition functions on different tori.

**Classical Taylor estimate.** Expand the four analytic link factors of a plaquette in the relative gauge at $V_0=I$. The first discrete curl is $O(\epsilon_1\eta^2)$ by (19) and the terms quadratic in link logarithms are $O(\epsilon_1^2\eta^2)$. Thus $\|P-I\|\le C\epsilon_1\eta^2$ throughout a smaller fixed complex chart. The holomorphic Wilson action uses
$N-\frac12\operatorname{Tr}(P+P^{-1})$,
whose absolute value is at most $C\|P-I\|^2$. In dimension four there are $6\eta^{-4}N_*^4$ fine plaquettes per original period, giving
\[
\sup_{\|b\|_\infty<\delta}|S_*(e^b)|
\le C\epsilon_1^2 N_*^4
\tag{PERIODIC-CLASSICAL-CHART}
\]
uniformly in K. Alternatively apply the estimate on the cover and divide by its number of periods.

The first derivative at zero vanishes and the Hessian is the constrained Wilson Hessian $\Gamma_s$ computed from the actual linearized average. The classical first variation at I is zero, so the second derivative only requires the linear minimizing extension. Apply one-variable Cauchy estimates on the ray of a fixed coarse field B. For every fixed R and sufficiently small $g=\beta_*^{-1/2}$ with $gR<\delta/2$,
\[
\left|\beta_*S_*(e^{g B})-
\tfrac12\langle B,\Gamma_s B\rangle\right|
\le C_{N_*,\delta,R}\,g,\qquad \|B\|_\infty\le R .
\tag{STOPPED-CLASSICAL-MATCH}
\]
The constant is independent of K. If the native normalized-trace action is used, absorb its fixed N into $\beta_*$ and $\Gamma_s$ together. Haar Jacobians in these finitely many link coordinates are smooth, uniformly bounded above and below on this fixed window.

This proves the classical exponential-weight approximation on a finite canonical stopping window around the identity. The bounded fluctuation potential, all history contributions, normalization outside the window including flat holonomies, and the actual pullback of the physical insertions are separate issues in WINDOW-COMPARISON and WINDOW-ERROR. In particular the classical window estimate by itself gives no lower bound for the normalized probability of the reflected event.

### 4.42 Why higher source orders should use finite jets (P diagnostic)

The Gaussian example in §4.19 has a counterpart in the full compact Wilson measure. T1 Theorem 7.41 identifies the following obstruction, whose argument is included here because it fixes the scope of ICR-3-ALL.

On the fixed physical torus let $\lambda_a=a^{-4}$ and consider one fixed plaquette orientation with bare dimension-eight integral
$Y_a=\lambda_a\sum_x s_{12}(x)^2$.
Along the weak trajectory assume $\beta_a/\lambda_a\to0$. The zeros of
$\mathbb E_{\mu_a}e^{zY_a}$ approach the origin.

Suppose a sequence instead had a common zero-free disc. On that disc choose
\[
F_a(z)=(\lambda_a n^4)^{-1}
\log\mathbb E_{\mu_a}e^{zY_a},\qquad F_a(0)=0 .
\]
Since $Y_a\le C\lambda_a n^4$, the real parts of $F_a$ are bounded above on each smaller disc. The harmonic coefficient estimate or the Borel–Carathéodory inequality makes this a locally bounded normal family.

For a fixed real $t<0$, $F_a(t)\le0$. Keep all links in Haar balls of radius a about I. Their probability under product Haar measure is at least $\exp[-C n^4\log(1/a)]$, their Wilson action is at most $C n^4a^2$, and the squared plaquette energies are at most $Ca^4$ each. The Wilson normalization is at most one. These inequalities give $\liminf F_a(t)\ge0$. For $t>0$, the product Haar mean of $\sum_xs_{12}(x)^2$ is $c_N n^4$ with $c_N>0$. Boundedness of each summand implies that this sum exceeds $c_Nn^4/2$ on a set of Haar probability bounded below independently of a. The Wilson cost on that set is at most $C\beta_an^4$. Hence $\liminf F_a(t)\ge tc_N/2$. Any analytic subsequential limit would vanish on a negative real interval and be strictly positive on the positive one, contradicting the identity theorem.

This is a statement about the specified bare dimension-eight exponential. Scalar entire contact factors preserve its zeros. The argument concerns a different source amplitude from the normalized action and the frustration comb. Together with TORUS-LOCAL-CUM it explains why fixed-order, degree-dependent factorial estimates are the appropriate alternative for high composite insertions. Matching an interacting renormalized operator still requires its own lower-row prescription.

### 4.43 Actual two-step real innovations at nonflat regular terminal fields (P/L)

The two real innovations on the original clean chart can be bounded without a complex source logarithm. The proof uses a positive Hessian in the *joint constrained coordinates*. It does not require a Poincaré inequality for the full Wilson measure.

Use the two original CMP109 independent-coordinate selectors, with their physical cutoff $\epsilon_1$ small inside the chart of §§4.24,4.28. Each selector constrains the original independent bond logs in a product of balls; the selected corridor bonds are determined by the constraint. This follows from CMP109 (2.9)–(2.12), printed pp.266–268. Let the terminal real $W_2$ lie in a sufficiently small physical neighborhood of I, or in an admitted gauge representative of that neighborhood. Write $\mathcal B=(B_0,B_1)$ for the real canonical coordinates in the two fibers.

**Conditional Hessian.** Up to a scalar independent of $\mathcal B$, the exact joint potential is the augmented fine Wilson phase with its two original gauge terms, evaluated at the composed readout, minus the logarithms of the two Haar and selected-coordinate Jacobians. In normalized native units its classical part has the exact form
\[
g_0^{-2}[A(U)-A(U_1)+G_0(U)]
+g_0^{-2}A(U_1)+g_1^{-2}G_1(V_1),
\]
with the second fiber now centered at its actual regular minimizer for $W_2$. This is the same original change of variables as T1 Lemma 7.36. For the first bracket, stationarity at its fine minimizer holds for each real $V_1$. At the joint identity its canonical Hessian is the positive direct sum of the two original augmented constrained precisions, with the bounded $g_1^2/g_0^2=1+O(g_0^2)$ correction in the second physical block. Its smallest eigenvalue is bounded below by a constant depending on L and the native margins, independently of volume, by the exponential Schur bounds for the two inverse covariances.

Varying $W_2$ and the physical coordinate arguments $v_i=g_iB_i$ changes this Hessian by at most
$C_L(\|\log W_2\|_\infty+\epsilon_1+g_0^2)$
in Schur norm. To verify this quantitatively, expand the original local phase after the tree-analytic substitutions of §4.28, with the small terminal target added as an argument of the same implicit maps. Differentiate two canonical slots in each monomial of degree at least three. Their two factors $g_i g_j$ cancel the original inverse-square coupling up to a bounded ratio, leaving at least one small physical argument. The absolute anchored coefficients sum uniformly, including all mixed slots. The Haar logs and finite corridor-determinant logs have a common local analytic domain and their two canonical derivatives cost $C_L\max_i g_i^2$ after the same summation. Constants independent of the two fields drop out. This proves that for sufficiently small stated parameters the exact real conditional potential $V_{W_2}$ satisfies
\[
\nabla_{\mathcal B}^2 V_{W_2}\ge m_L I,\qquad m_L>0,
\tag{JOINT-CONVEXITY}
\]
throughout the product selector. It is important here that the physical selector is small even though its canonical height may grow. This calculation does not cover a nonconvex live or mixed selector.

On this convex product domain the real conditional law consequently satisfies
\[
\operatorname{Var}_{2,W_2}^{\rm clean}(F)
\le m_L^{-1}\mathbb E_{2,W_2}^{\rm clean}|\nabla_{\mathcal B} F|^2 .
\]
For a direct check, the integrated Bochner identity for the weighted Neumann generator bounds its squared-generator norm below by $m_L$ times the gradient form. The interior Hessian term gives this bound and the second fundamental form of a smooth convex boundary is nonnegative. The spectral decomposition then puts the first nonconstant eigenvalue at least at $m_L$. Approximate the product of balls from within by smooth convex domains and pass to the normalized integrals. This is the strong-convexity consequence of the [Brascamp–Lieb variance inequality](https://doi.org/10.1016/0022-1236(76)90004-5), with the required positivity established for this actual joint fiber.

**Ordinary source derivative.** Differentiating the original fine $r_b$ with respect to a canonical coordinate retains a factor $g_i$. The derivative of its force square retains an original first force and its remaining derivative has a bounded tree-summable kernel. The Casimir derivative is a fixed sum of original first plaquette forces. Weighted Schur summation therefore gives
\[
|\nabla_{\mathcal B} r_f|^2
\le C_L\beta_0\sum_b |f_b|^2\sum_{p\in Y_b}s_p(U)
\tag{JOINT-REAL-GRADIENT}
\]
on the admitted real chart. The same bound holds for h. This estimate uses $\beta_0 g_i^2=O_L(1)$ for both species, and actual fine plaquette excesses. In particular it does not replace a nonflat background by the square of its canonical cutoff height.

**Undivided averaging.** Multiply the conditional variance by the actual positive weight of this selected two-clean body and integrate over its admitted terminal $W_2$. The selected measure may equivalently be obtained by adjoining the two normalized based-gauge integrations to the original Wilson law and retaining their original real selectors. The Faddeev–Popov factor is a conditional probability on each based orbit by (0.15)–(0.16) of CMP109. Coarse based gauges can be lifted constantly inside their fine blocks, preserving the earlier gauge-invariant action and conjugating its in-block contour variables. The original plaquette excesses are gauge-invariant. Thus a nonnegative function of those excesses integrated over this selected body is bounded by its full Wilson expectation. No signed polymer term is declared a conditional probability.

Let $w_{\rm cc}(W_2)$ denote that conditional clean probability in the positive lift and G the admitted terminal chart. FIRST and JOINT-REAL-GRADIENT give
\[
\mathbb E\left[1_G w_{\rm cc}(W_2)
\operatorname{Var}_{2,W_2}^{\rm clean}(r_f)\right]
\le C_L\sum_b |f_b|^2\sum_{p\in Y_b}
\mathbb E_{\rm W}(\beta_0s_p)
\le C'_L M_f.
\tag{NONFLAT-TWO-INNOVATIONS}
\]
By positive total variance within the very same selected body, the left side is the sum of the averaged conditional innovation given the first retained field and the variance of its first retained mean in the second integration. Each therefore satisfies this extensive bound individually. This is an actual two-step result at admitted nonflat terminal fields and uses their real probability weights. It controls the whole specified positive contribution even if that contribution has small mass. The other sectors, the covariance between sector means and the remaining second-terminal mean still occur in TWO-STEP-WILSON.

### 4.44 Uniform coarse curl energy at a regular classical minimum (P/L)

There is a nonlinear lower bound on the classical stopping action which is uniform in the depth of the homogeneous hierarchy. It retains the four-dimensional volume normalization.

Use a real regular fine configuration and write $K_p=\log P_p$ in the common small plaquette chart. Put $\delta=\sup_p|K_p|$. Fix one coarse plaquette P for a single L-step and take a bounded contractible fine rectangle $Y(P)$ containing its contour frames, straight paths and fillings. All constants in this local calculation depend on fixed L. Periodically lift the deterministic data as in §4.41 if the determining rectangle requires more room.

Gauge-fix a coordinate tree in $Y(P)$. The remaining fine link logs A obey
\[
\|A\|_{\infty,Y}\le C_L\delta,\qquad
\|A\|_{2,Y}\le C_L\left(\sum_{p\in Y(P)}s_p\right)^{1/2}
\]
by the finite loop fillings. On this fixed finite chart the plaquette and contour maps are analytic. Their second derivatives are uniformly bounded. Taylor expansion about I therefore bounds each nonlinear remainder by $C_L\delta(\sum_Ys_p)^{1/2}$. The linear coarse curl is $dQ A=\mathcal R_2 dA$, because the endpoint contour frames form a coarse gradient. Replacing $dA$ by the actual fine plaquette logs costs the same quadratic remainder. This proves the pointwise bound
\[
|\log P^{\rm coarse}|
\le\sum_p(\mathcal R_2)_{Pp}|K_p|
+C_L\delta\left(\sum_{p\in Y(P)}s_p\right)^{1/2}.
\tag{NONLINEAR-CURL-STEP}
\]
All coarse holonomies are conjugated by the chosen gauge; their norms and the fine plaquette norms are unchanged. The actual linear square filling has nonnegative coefficients, row sum $L^2$ and column sum $L^{-2}$ as in §4.33.

The neighborhoods $Y(P)$ have bounded overlap. Schur summation and the comparison $s_p=\frac{\tau}{2}|K_p|^2[1+O_N(\delta^2)]$ give
\[
S(M_1U)\le(1+C_L\delta)S(U),\qquad
\delta_{\rm coarse}\le L^2\delta+C_L\delta^2 .
\tag{CURL-STEP-BUDGET}
\]
For the first estimate first sum squared log norms and then convert both fine and coarse logs back to Wilson action. The coarse log radius is $O_L(\delta)$, so no factor larger than one survives in the leading term. The coefficient one is the product of the exact filling row and column norms in dimension four.

Let $U=U_K(W)$ be the regular minimal representative of a target with coarse plaquettes bounded by $\epsilon$. CMP102 Theorem 1 puts the fine representative in (8), and its defining regularity condition (2) gives $\delta_0\le C\epsilon L^{-2K}$ on the homogeneous hierarchy. Apply CURL-STEP-BUDGET to its successive actual averages. For sufficiently small fixed $\epsilon$,
\[
\delta_j\le 2C\epsilon L^{-2(K-j)},\qquad
\sum_{j=0}^{K-1}\delta_j\le C'_L\epsilon .
\]
Indeed after multiplying the one-step radius inequality by $L^{2(K-j-1)}$, the multiplicative excess is bounded by $C_L\delta_j$. Bootstrap the factor two using the summable geometric series and shrink $\epsilon$ if necessary. Multiplying the action inequalities now yields
\[
S_{\rm coarse}(W)\le e^{C_L\epsilon}S_*(W).
\tag{UNIFORM-CLASSICAL-ENERGY}
\]
No power of K is incurred by accumulating the gauge and nonlinear contour errors.

This lower bound for the regular classical action and STOPPED-CLASSICAL-MATCH improve two distinct parts of a possible finite-window probability estimate. The former controls a real regular target by its coarse Wilson curvature. The latter gives the correct quadratic weight on the selected bounded canonical window. Neither bounds the complete normalized history sum or the gauge and holonomy integrations outside that window.

### 4.45 The periodic Gaussian witness in flat holonomy sectors (P)

The reference witness of §4.35 does not disappear merely because a periodic flat background has nontrivial commuting holonomies.

A flat real connection on the untwisted periodic lattice determines a commuting tuple of cycle holonomies. After a gauge choice it has constant commuting parallel transports, and there is a common Cartan subalgebra of dimension at least $\operatorname{rank}SU(N)$. On its parallel Cartan component the covariant differences are ordinary differences. The linearized contour frames, straight averages, physical quadratic action and curvature readout restricted to this component are the same as at the identity. Orthogonal charged components are preserved by the flat covariant operators. Remove harmonic null directions as before. The selected nonzero spatial Cartan momentum has no such null direction.

Use a magnetic mode with the same spatial pointing in both halves and transport its color to a common spatial root within each slice. On the parallel Cartan part these transports act trivially. Thus the real cross covariance $C_{XY}$ of the full color vectors has a Cartan block $c_s(j)I$. For centered real Gaussian vectors, Wick's formula gives
\[
\operatorname{Cov}_G(|X|^2,|Y|^2)
=2\|C_{XY}\|_{\rm HS}^2
\ge2\,\operatorname{rank}(SU(N))\,c_*^2 .
\tag{FLAT-HOLONOMY-GRAM}
\]
This uses only the Cartan contribution; no lower estimate on singular values in every charged direction is asserted.

The bound also survives a probability mixture over these flat Gaussian backgrounds when evaluating the reflected magnetic squared mode. At a fixed flat background, translation of the mode in time preserves its same-slice squared expectation, with any common color rotation removed by the norm. The covariance decomposition for a mixture therefore adds the nonnegative variance of this conditional squared expectation to the average of FLAT-HOLONOMY-GRAM.

This statement concerns the Gaussian tangent laws in the indicated flat sectors. The compact Wilson stopping law also contains the interacting normal directions, the actual conditional weights near singular holonomies and the transported physical operator. Those are part of the remaining reflected comparison.

### 4.46 A real two-jet summation threshold for the remaining comb (P implication)

Uniform holomorphy of the complete pressure is sufficient for variance, but a real second-order proof can allow scale-dependent constants. The volume factors specify how much growth is affordable.

Let $N_j=(n/L^j)^4$ and use the single temporal comb of §4.38, so $N_{\rm cell}=n^4/8$. Suppose the complete positive transition tower, including history means, has real innovation bounds
\[
\mathbb E\operatorname{Var}(m_{j-1,f^{\rm comb}}\mid X_j)
\le C N_{j-1}(1+j)^q A_j^2
\]
for fixed q and an amplitude satisfying
$A_{j+1}\le(1+C g_j^2)A_j+C(1+j)^q$ with bounded $A_0$. Suppose also that the terminal retained variance is at most $C N_K^2(1+K)^q A_K^2$, with the fixed stopped grid. Then full SUS follows, even if these amplitudes grow polynomially and no common complex source disc has been proved.

Indeed in the admitted small-coupling regime I-0c gives $x_i=g_i^{-2}\ge x_j+c(j-i)$ for $i\le j$ after lowering the weak threshold. Consequently
\[
\sum_{i<j}g_i^2\le C'\log(2+j)
\]
uniformly in a and in the endpoint coupling. Iterating the amplitude inequality gives $A_j\le C''(1+j)^{q'}$ for a fixed $q'$. Sum the positive innovations using $N_{j-1}=n^4 L^{-4(j-1)}$. The exponential geometric factor sums their polynomial costs. The terminal bound divided by $n^4=N_K L^{4K}$ is bounded as well. The result is an extensive variance for the comb, and EIGHT-SITE-COMB extends it to all marks.

In fact a fixed exponential amplitude is also affordable. If $A_j\le C(1+j)^q B^j$ with $B<L^2$, the innovation sum is bounded by $C n^4\sum_j (1+j)^{q'}(B^2/L^4)^j$. The terminal term obeys the same comparison. Thus an individually nonsummable relative feedback per step can still be compatible with real susceptibility.

For example, the fixed-domain two-jet argument in POLYMER-ENERGY-SUBTRACTION costs $C\alpha_j^{-2}$ on an actually verified smaller physical holomorphic radius $\alpha_j$. Relative to $\beta_j S$ the loss is $C g_j^2/\alpha_j^2$. If the true spare radius is at least $c g_j(\log g_j^{-2})^q$, $q>0$, this becomes $C'(\log g_j^{-2})^{-2q}$. Taking the weak endpoint small makes $1+C'(\log \bar g^{-2})^{-2q}<L^2$, which is enough for the preceding geometric sum even though it is weaker than a summable flow derivative. This observation requires the claimed spare radius for the actual inherited readout at each step. A radius for an unrelated set of external variables does not supply it.

The same threshold applies when the second jet is constructed by a connected polymer expansion only to source order two. Work in the finite algebra generated by two commuting square-zero variables $\epsilon_i$. Its coefficient norm $|a_0|+\rho(|a_1|+|a_2|)+\rho^2|a_{12}|$ is submultiplicative. The ordinary absolutely convergent polymer proof applies in this algebra whenever its rooted activity majorant including these weighted coefficients meets the same strict summability margin. If the first and second rooted majorants are $A_j$ and $B_j$, choose the algebra weight proportional to $(1+A_j+\sqrt{B_j})^{-1}$. The resulting second logarithmic coefficient costs at most $C N_j(1+A_j^2+B_j)$. This argument includes the product of the two distinct first jets and the within-activity second jet. It never exponentiates an unbounded physical mark at a fixed complex amplitude.

This is an alternative real interface target. Theorems 3.7–3.8 and §§4.39–4.40 supply the single mark, the first two admitted clean innovations, the nonlinear critical gain and the first integrated nonidentity bound. A uniform polynomial-cost induction through the remaining mixed, healed and terminal rows is still required to apply the summation threshold.

### 4.47 A normalized regular-holonomy window criterion (C on the terminal density and physical readout)

The classical estimates permit a finite-dimensional verification of the probability comparison in §4.36 under a concrete terminal density hypothesis. It is useful to distinguish this hypothesis from the classical variational theorem.

Fix $N_*\ge4$ as in §4.35 and a sufficiently small **positive fixed** $g=\beta_*^{-1/2}$. Uniformity below is in the fine depth K. Assume the following fieldwise statement for the complete stopped density, with its common scalar removed:
\[
\widetilde\rho_K(W)=1_{\mathcal S_g}(W)
b_K(W)e^{-S_*(W)/g^2}+\mathcal R_K(W),\qquad
\|\mathcal R_K\|_\infty\le C e^{-c/g^2}.
\tag{TERMINAL-DENSITY}
\]
Require $0\le b_K\le C_b$ on the real regular branch and $b_K\ge c_b>0$ in the bounded canonical windows around the regular flat backgrounds selected below. The regular branch must contain the windows up to canonical radius $C_R\sqrt{\log(1/g)}$ used in the argument, and satisfy UNIFORM-CLASSICAL-ENERGY. Constants are uniform in K and at weak g. The full density is positive. This is a pointwise statement about the summed remainder and the named physical stopped variables. An estimate only on integrated sector masses needs a separate implication before using TERMINAL-DENSITY.

Choose a compact conjugation-invariant set of spatial holonomies with simple spectrum and an eigenvalue gap bounded below. Require a smaller such set with nonempty relative interior for the lower bound. At the negative slice choose the coarse spatial cycle holonomy H in direction one, based at the same root as the transported magnetic Fourier mode. Project the mode onto the Lie-algebra centralizer of H, which is a Cartan algebra on this set. The projection is a smooth, gauge-covariant function of H there. Let $Y_-$ be that projected mode in $g^{-1}$ curvature units and define the negative-half event
\[
E_R=\{H\text{ belongs to the chosen set},\quad
R\le |Y_-|\le R+1\}.
\]
The defining paths are spatial and the chosen coarse slice has the positive/negative margin specified in §4.35. Norms and the holonomy condition are gauge invariant. Let F be $g^{-2}$ times the spatially averaged coarse $12$-plaquette energy on the reflected positive slice, with a fixed positive normalization.

**Normal coordinates.** Gauge-fix a based spanning tree on the fixed coarse lattice. The remaining space is finite dimensional and has smooth Haar densities in local charts. The flat configurations with H in this regular set form a smooth manifold. Indeed the four cycle holonomies commute, one is regular, and the others belong to its unique maximal torus. Locally the commuting tuples are parametrized by the common conjugation frame and four torus coordinates, up to a finite Weyl identification. The tangent space is precisely the kernel of the covariant curl in this based gauge. On the Cartan part, closed linear cochains split into gradients and four harmonic coordinates. On every root part the first cycle has nontrivial adjoint monodromy, so a closed cochain is a covariant gradient: one can solve for its potential along that cycle using the invertible difference of the monodromy from I, and the other commuting difference equations follow by closure. Fixing the based tree removes the based gradients. The remaining infinitesimal global conjugations are tangent to the flat manifold. In particular its normal codimension d is constant on the selected compact set.

On a slightly larger regular set the ordinary coarse Wilson energy is bounded below by c times the squared distance to this flat manifold in a fixed tube. This follows from its positive normal Hessian, compactness and Taylor's formula. Away from the tube the coarse energy has a positive lower bound when H remains in the selected set. UNIFORM-CLASSICAL-ENERGY transfers these lower bounds to the regular stopping action. The fixed-depth-independent upper bound on the normal Hessian follows from PERIODIC-CLASSICAL-CHART applied at a flat real base in Proposition 9. The proof of §4.41 at such a base is the same covariant relative plaquette expansion, because the base plaquette is I. Its normal Hessian $\Gamma_{s,H}$ also has a uniform positive lower bound: in local parallel frames the flat covariant coarse-curl filling in §4.33 has the same unitary row and column bounds, and the coarse covariant curl has a positive lower singular value on this compact normal bundle. Thus both the Gaussian normal covariance and its inverse are bounded uniformly in K.

Write the normal coordinate as $g\xi$. The volume element is $g^d$ times a smooth bounded positive density times flat-manifold measure and $d\xi$. On $|\xi|\le R_0$, STOPPED-CLASSICAL-MATCH gives
\[
g^{-2} S_*(W)=\tfrac12\langle\xi,\Gamma_{s,H}\xi\rangle
+O(g R_0^3)
\]
uniformly on this finite cover of regular flat charts. The projected negative readout differs from its Cartan Gaussian linearization by $O(gR_0^2)$ there. The same estimate holds for a positive Cartan mode used only to lower bound F. The derivative of the holonomy projection does not enter the leading term, because the base plaquette curvature is zero. All Cartan transports are trivial, hence the two linear Cartan modes have exactly the covariance of §4.35 in $\operatorname{rank}SU(N)$ components, independently of the other holonomies. A choice of tree or Cartan frame does not change their norms.

**Window masses.** Let $p_s(R)$ denote the Gaussian Cartan probability of the annulus $[R,R+1]$. The variances are bounded above and below uniformly in K. For $R\ge1$, widening or narrowing each edge by a sufficiently small multiple of $(1+R)^{-1}$ changes this probability by at most fixed multiplicative constants. This follows directly by integrating the radial Gaussian density. Take $R_0=C_0(1+R)$ large enough that the uniform normal tail $e^{-cR_0^2}$ is at most a fixed multiple of $p_s(R)$. Require $gR_0^3$ and $(1+R)gR_0^2$ small.

On this window the upper unnormalized mass of $E_R$ is at most $C g^d p_s(R)$ by the upper bound on $b_K$, the Gaussian density comparison and the widened annulus. Contributions with $|\xi|>R_0$ still inside the regular tube are at most $C g^d e^{-cR_0^2}$ by its quadratic lower bound. Outside the tube the regular mass is exponentially small in $g^{-2}$, and the absolute complete remainder has the same form by TERMINAL-DENSITY. These errors fit the displayed upper bound for the choices below.

For the joint lower mass, restrict H to the interior subset, put the negative Cartan mode in the narrowed annulus, and keep the positive Cartan linear mode within a fixed M of its conditional Gaussian mean. The conditional mean has magnitude at least $\alpha_*R$. The other normal coordinates can be kept in $|\xi|\le R_0$ at a fixed fraction of the annulus mass: their conditional Gaussian covariances are bounded and their means given the Cartan mode are $O(R)$ uniformly. Increasing $C_0$ once suffices. Gaussian normalization factors on the normal spaces and the flat-chart Jacobians have fixed positive upper and lower bounds. This gives unnormalized joint mass at least $c g^d p_s(R)$. The true positive F on this event is at least $c'R^2$ for large R, by the small readout error and the positive spatial sum-of-squares bound. The negative remainder in TERMINAL-DENSITY cannot remove this lower mass when $g$ is sufficiently small, since its total absolute mass is $O(e^{-c/g^2})$.

Consequently $\mathbb E(F\mid E_R)\ge c'' R^2$ and $\mathbb P(E_R)\ge c g^d p_s(R)$, the latter using the uniform total mass upper bound. The unconditional mean obeys
\[
\mathbb E F\le C[1+\log(1/g)] .
\]
To see this, the normalization has a lower bound $c g^d$ from a bounded regular flat normal window. On the regular branch $F\le Cg^{-2}S_{\rm coarse}$ and UNIFORM-CLASSICAL-ENERGY gives an exponential upper tail for this last variable, divided by at most the harmless $g^d$ normalization lower bound. Integrate the tail starting at a sufficiently large multiple of $\log(1/g)$. On the complete remainder use $F\le Cg^{-2}$ and the exponential absolute bound. This argument does not require that the regular flat stratum dominate the global normalization.

Choose $R^2=A[1+\log(1/g)]$ with A sufficiently large, followed by sufficiently small g. Then $gR_0^3\to0$ and $p_s(R)$ is bounded below by a fixed power of g uniformly in K. The conditional contrast is positive. If these stopped variables pull back to the stated original halves, REFLECTED-EVENT therefore gives a strictly positive K-uniform reflected Gram for this coarse magnetic energy at the **fixed** g. The lower bound can depend on g and is not asserted uniform as $g\downarrow0$.

This is a conditional coarse-observable conclusion. It uses TERMINAL-DENSITY, a fixed physical endpoint and the positive-half pullback. To obtain the requested renormalized local operator one must still prove WINDOW-ERROR with its actual normalization. The exact I-0c phrase concerning large-region weights should be matched to the fieldwise remainder in TERMINAL-DENSITY; a thermodynamic pressure upper bound or a Gaussian toron calculation alone does not perform that match.

### 4.48 Old Wilson carriers on regular minima and logarithmic anchor counting (P/L)

Let the old lattice spacing be \(\xi=L^{-(k-l)}\) in units of one current block. Let \(U=M^lU_k(W)\) be the actual old contour readout on a completed regular interior cube of a homogeneous hierarchy. The underlying fine minimum and its complex coarse variations are in the domains of CMP102 Proposition 9. Use local representatives with a collar containing all determining contours. In current units the old links are \(\exp(\xi A)\) with \(A\) bounded in \(C^1\) by \(C\epsilon\). A unit coarse variation at \(y\) has the same norm locally with bound \(C\exp[-c\,d(y,X)]\) on an old carrier \(X\), with distance in current units. These statements follow from CMP102 (9),(19),(190) and T1 Lemma 7.54: its coarse representative averages derivatives with leading norm one, and the nonlinear excess at mesh \(\xi_i\) is \(C\epsilon\xi_i\), whose sum is bounded. Its product estimates hold for complex matrices as well. The cubes where these bounds are used must include the collars. On a smaller coarse-target polydisc of radius \(\rho\) all these bounds hold throughout the disc. The final anchor bounds below include \(\rho^m\) for \(m\) external derivatives. Here \(\rho\) is a physical coarse-target radius, distinct from a composite source radius.

Consider first a literal old Wilson carrier, the normalized character trace in a fixed finite-dimensional representation around a contractible old loop of length \(D\). Suppose it admits a conjugated elementary-plaquette filling with at most \(C D^2\) faces and paths of length at most \(C D\) to a base point. Coordinate rectangles and loops in a contractible coordinate box have such fillings by successively sorting their coordinate steps. Denote the trace with its identity value removed by \(F_X\). All constants below may depend on the representation. Old plaquettes in the complex chart obey \(\|P-I\|\le C\epsilon\xi^2\), by expanding the four old link exponentials using the first-difference bound. Path conjugation costs at most \(\exp(C\epsilon \xi D)\). If \(D\xi\le c_0\), the filling therefore bounds the logarithm of the loop by \(C D^2\epsilon\xi^2\), after decreasing \(c_0,\epsilon\). The first derivative of a character at identity vanishes since every Lie algebra element is a sum of commutators. Consequently
\[
 |F_X|\le C D^4\epsilon^2\xi^4 .
\]
If \(D\xi>c_0\), the raw product has norm at most \(\exp(C\epsilon\xi D)\), and \(1\le c_0^{-4}D^4\xi^4\). For either size the absolute value is at most \(C D^4 e^{C\epsilon D}\xi^4\). This last form uses a fixed regularity cutoff and does not assert a small \(\epsilon^2\) factor for the large carrier.

Cauchy's estimate for a fixed tuple of \(m\) coarse target coordinates on a smaller interior disc gives the same bound for \(\rho^m|\partial_{\mathbf y}F_X|\), with a constant depending on \(m\). There is a second bound for the same tuple. Choose its most distant anchor relative to a fixed old root \(x\in X\), write \(R=\max_i d(x,y_i)\), and differentiate the ordered product of old links once at that anchor. The preceding variation estimate, the \(D\) possible differentiated links and the product norm give \(C D\exp(C\epsilon D+cD\xi)e^{-cR}\), since \(d(y_i,X)\ge R-D\xi\). Cauchy on the other \(m-1\) coordinates preserves this exponential. We can reduce \(c\) and \(\epsilon\) so all positive exponent costs in \(D\) use an arbitrarily specified spare carrier weight. For \(m=0\) the value estimate alone suffices.

For \(m\ge1\) and any fixed spatial moment \(p\ge0\), the number of anchor tuples with \(r\le R<r+1\) is at most \(C_m(1+r)^{4m-1}\). This follows by choosing an outermost anchor and summing the others in the radius-\(r+1\) ball; the same shell bound holds with periodic coordinate distances. Split the sum of the two bounds at \(r=4\log(1/\xi)/c\), taking the smaller bound on each side. For any specified \(\delta>0\), after the indicated domain and decay choices,
\[
 \rho^m\sum_{\mathbf y}(1+R)^p|\partial_{\mathbf y}F_X|
 \le C_{m,p,\delta}(1+D)^4 e^{\delta D}
       \xi^4(1+k-l)^{4m+p}.
 \tag{OLD-WILSON-ANCHORS}
\]
Indeed the tail sum of \(e^{-cr}(1+r)^{4m+p-1}\) is bounded by \(C\xi^4(1+\log(1/\xi))^{4m+p-1}\). Torus wrapping paths which have no contractible filling are excluded and keep their own carrier weights. The estimate applies to genuine contractible old Wilson loops at all regular clean ages, including the individual Wilson plaquette. It controls all fixed absolute physical moments and retains the whole fourth power. Interpolating the two displayed bounds by a fixed fractional power would lose part of that power.

For these literal loops the stronger bound with no polynomial in age also holds. Write the filling as \(\mathcal U=\prod_j T_jP_jT_j^{-1}\). Let a dot denote the derivative at the most distant anchor. Direct differentiation of an elementary plaquette gives
\[
 \|\dot P_j\|\le C\xi^2\exp[-c(R-C D\xi)].
\]
In fact the oriented sum of the four first variations of \(\xi A\) has a forward difference in each opposing edge pair and is \(O(\xi^2)\) times the weighted \(C^1\) response. All other terms contain a background \(O(\epsilon\xi)\) as well as one variation \(O(\xi)\). In the conjugated factor the terms involving \(\dot T_j\) reduce to a commutator with \(P_j-I\). The path product rule gives \(\|\dot T_j\|\le C D\xi e^{C\epsilon D\xi}\exp[-c(R-CD\xi)]\), and similarly for the inverse. For \(D\xi\le c_0\), the product norms over all the filling factors are at most \(\exp(C D^2\epsilon\xi^2)\). Consequently
\[
 \|\mathcal U-I\|\le C D^2\epsilon\xi^2,\qquad
 \|\mathcal U^{-1}\dot{\mathcal U}\|\le C D^2\xi^2 e^{-cR}.
\]
For the representation \(\pi\), the derivative of its trace is \(\operatorname{tr}[(\pi(\mathcal U)-I)d\pi(\mathcal U^{-1}\dot{\mathcal U})]\) by tracelessness of \(d\pi\). The product of the two displayed bounds supplies the whole \(\xi^4 e^{-cR}\). For \(D\xi>c_0\) use the original word's differentiated product bound and \(1\le c_0^{-4}D^4\xi^4\). After Cauchy in the other slots and the shell sum, for any fixed \(m,p\) one obtains
\[
 \rho^m\sum_{\mathbf y}(1+R)^p|\partial_{\mathbf y}F_X|
 \le C_{m,p,\delta}(1+D)^5 e^{\delta D}\xi^4 .
 \tag{OLD-WILSON-ANCHORS-SHARP}
\]
This bound sums over every coarse external anchor at the same scale gain as the undifferentiated marginal operator.

The same differentiated filling controls each tree-gauge log of a contractible \(U\)-only activity in a genuine holomorphic orbit tube. If \(C D^2\epsilon\xi^2\le\alpha_l/2\), its gradient in these coordinates is bounded in dual sup norm by \(C a_X \alpha_l^{-2}D^2\epsilon\xi^2\) because the scalar's first jet vanishes. Multiplying by the tree-log variation bound above controls its remote derivative and then the other fixed anchor slots. Outside that coordinate ball an independently verified Cauchy margin on the evaluated orbit gives the ordinary first-response bound. The split argument above remains available there. This extension requires the precise evaluated domain of the activity. The Wilson-loop assertion follows directly from the entire character and has no such extra domain condition.

More generally the counting argument applies to a vacuum-subtracted scalar activity on the same graph whenever its value on the larger complex chart is bounded by \(a_X(1+D)^q e^{\delta D}\alpha_l^{-2}\xi^4\) and its first derivative by \(C a_X(1+D)^q e^{\delta D}\alpha_l^{-b} e^{-cR}\). Here \(\alpha_l\le1\) is its own activity chart. When \(b>2\) the split radius acquires the extra term \((b-2)\log(1/\alpha_l)/c\). An absolute value bound for a holomorphic gauge-invariant activity of norm \(a_X\) on a genuine orbit tube follows on small carriers by fixing an old coordinate tree. Every remaining link in that gauge is a based loop with logarithm \(O(D^2\epsilon\xi^2)\). There is no invariant linear scalar jet at the identity under simultaneous constant \(SU(N)\) conjugation. Taylor's formula on the old activity radius gives the value bound when these logs fit in radius \(\alpha_l/2\). When the bound \(C D^2\epsilon\xi^2\) exceeds \(\alpha_l/2\), the size majorant itself suffices, provided the activity really is bounded on the evaluated orbit. Extra independent current components require the same control of their actual values and derivatives on that activity's physical graph. The fine Wilson current, the current of the old averaged links, and the derivative of an inherited effective action are distinct. No identification of them is assumed here. T1 Proposition 7.67 establishes gauge saturation for the complete scalar carriers of its first-fiber expansion. Evaluation of an inherited carrier with independent current at a different age still requires its actual minimizing graph on the retained orbit domain.

A current cell contains \(\xi^{-4}\) old roots. Summing OLD-WILSON-ANCHORS cancels this multiplicity exactly. The polynomial clean-age cost is affordable for the real two-jet target of §4.46, even if carriers are born repeatedly. Precisely, if the nonnegative first-jet amplitudes satisfy
\[
 A_j\le C(1+j)^q+\delta_0\sum_{l<j}(1+j-l)^d A_l ,
\]
choose any \(1<\gamma<L^2\), put \(M=\sum_{h\ge1}(1+h)^d\gamma^{-h}<\infty\), and take \(\delta_0 M<1\). Multiplying by \(\gamma^{-j}\) and taking a finite running supremum gives \(A_j\le C_\gamma\gamma^j/(1-\delta_0 M)\). Thus positive tower innovations of size \(C N_{j-1}(1+j)^q A_j^2\) would sum extensively. This scalar recurrence does not prove its small prefactor for inherited clean or mixed vertices. The concrete old Wilson carrier estimate supplies the marginal transport and anchor counting for that class without requiring such a prefactor.

### 4.49 The inherited current on the original minimizing graph (P/L on homogeneous admitted cores)

There is a useful native distinction between the old averaged links and the pair on which an old activity is evaluated. In [Balaban, CMP109, pp. 261–263, (1.8)–(1.16)](https://doi.org/10.1007/BF01215223), the pair in (1.15) consists of the reconstructed minimizing configuration \(U_l(M'U)\) and its current \(J_l(M'U)\), computed using mesh \(L^{-l}\) in old units. For the current configuration with mesh \(\eta=L^{-k}\) in terminal units, (1.16) gives on the twice-reduced native core
\[
 |J_l(M'U)|\le \alpha_0(L^l\eta)^2.
 \tag{NATIVE-OLD-CURRENT}
\]
This supplies exactly the required two powers of \(\xi=L^{l-k}\) for that current's **value** on the admitted domains. It includes the original localized multiscale target \(M'U\); no differentiation of an effective action is involved.

We can compute the derivatives and the other coordinates explicitly on a homogeneous regular hierarchy near the identity target. Assume the physical current-target polydisc is inside the CMP102 regular margin, the old carrier has its required interior collar, and the old activity has native analytic slack \(\alpha>0\) on the inherited physical graph. More precisely use (1.12)–(1.14) with their smaller constants sufficient for condition (iv), as verified on CMP109 p. 263. An old logarithmic potential, its first differences and its independent current of norm below \(c\alpha\) then give an admissible line of analytic variables. The constants below may depend on those fixed margins. Choose the terminal physical regularity radius \(\epsilon\le c\alpha\). Use the common small chart about the flat target, or a contractible carrier and the same chart on all its determining stencils. The homogeneous statement uses the full nested constraints at each old scale.

Write \(U=U_k(W)\) for the fine minimum and \(W_l=M^lU\) for the old *averaged* links. The old *reconstructed* minimum \(U_l(W_l)\) is in the based gauge orbit of \(U\). Indeed any variation preserving \(M^lU\) preserves \(M^kU=M^{k-l}(M^lU)\). Stationarity of the Wilson action therefore holds on the old constraint as well. The same fine field satisfies the old regularity conditions on the homogeneous chart: its fine curvature in old units is \(O(\epsilon\xi^2)\), and its covariant current in old units is \(O(\epsilon\xi^3)\), by rescaling the terminal bounds. The old averaged target has plaquettes \(O(\epsilon\xi^2)\) by CURL-STEP-BUDGET or T1 Lemma 7.54. The uniqueness of the regular critical orbit in CMP102 Theorem 1 now identifies the two reconstructions. Gauge-invariant evaluated functions consequently agree on the real neighborhood; the holomorphic identities used below extend from that neighborhood. Equality with the homogeneous reconstruction is not used to replace a different mixed-domain variational problem.

The exact mesh factors can be read directly from (1.8). If the same fine links are expressed with old mesh \(\eta_l=\eta/\xi\), the curvature normalization changes by \(\xi^2\), and the adjoint covariant difference changes by \(\xi\). Therefore \(J_l=\xi^3 J_k\) on the common reconstructed field, up to its based adjoint gauge transformation. There is a uniform one-anchor estimate for \(J_k\) in the terminal chart about identity. To see it, write \(U=e^{i\eta A}\), with \(A\) and its first differences bounded in terminal units. The expansion of the ordered four-link word gives
\[
 \eta^{-2}\pi\operatorname{Im}P
    = d^\eta A + Q(A,A)+\eta R.
\]
Here the fixed quadratic polynomial \(Q\) consists of commutators of coincident field values with the usual orientation factors. Replacing adjacent fields in these quadratic terms by coincident ones costs \(O(\eta)\). The cubic and higher exponential terms after division by \(\eta^2\) also cost \(O(\eta)\). The resulting \(R\) and its one-anchor variation are bounded by the \(C^1\) norms of the fields and responses on the fixed stencil. Thus one adjoint difference of \(\eta R\) costs a fixed constant, including for the anchored derivative. The ordinary divergence of \(Q\) uses only first differences. Replacing the ordinary divergence by its covariant version costs a factor \((\operatorname{Ad}U-I)/\eta=O(\|A\|)\) times the local curvature. The linear term is \(d^{\eta *}d^\eta A\), whose response is the fourth row of CMP102 (190) at the flat reference. This proves \(|\partial_yJ_k|\le C e^{-c d(y,X)}\) locally on a smaller complex target chart. Baseline fields, ordinary first differences and their response use the first two rows of (190). These estimates keep the \(\eta\) factor on the nonlinear remainder before applying its difference.

Let \(X\) have old-unit diameter at most \(D\ge1\) and base site \(x_0\). For \(D\xi\le c_0\), change the fine gauge over its bounding rectangle by the exponential of the linear function \(\sum_\mu(x-x_0)_\mu A_\mu(x_0)\), with the sign chosen to cancel the constant potential at the base point. In continuum notation this subtracts \(A(x_0)\) from \(A(x)\); for the actual links the identity is the expansion of \(u(x)e^{i\eta A_\mu(x)}u(x+\eta e_\mu)^{-1}\). The first-order remainder after division by \(\eta\) is bounded by \(C\epsilon(|x-x_0|+\eta)\). Indeed \(A(x)-A(x_0)\) has this Lipschitz bound, and differentiating the exponential of the linear gauge function changes its constant derivative by \(O(\epsilon^2(|x-x_0|+\eta))\). Discrete first differences of the resulting potential are bounded by \(C\epsilon\). The same product estimates after one target variation give the analogous bounds with \(\epsilon\) replaced by \(C e^{-c(R-CD\xi)}\), \(R=d(y,x_0)\). These computations use no number of fine bonds proportional to the old depth.

In old units let \(A_o\) denote this representative's potential and use the norm \(\|(A_o,J_l)\|_*=\|A_o\|_\infty+\|\nabla^{\eta_l}A_o\|_\infty+\|J_l\|_\infty\). The preceding bounds, the old current rescaling, and its adjoint gauge rule give
\[
 \|(A_o,J_l)\|_*\le C(1+D)\epsilon\xi^2,\qquad
 \|\partial_y(A_o,J_l)\|_*\le C(1+D)\xi^2 e^{-cR}
 \quad(D\xi\le c_0).
 \tag{OLD-GRAPH-COORDINATES}
\]
The gauge transformation is unitary for real target data in Hermitian conventions. Equality in the complex chart follows by holomorphic continuation of the real gauge identity, so invariance under arbitrarily large complex gauge changes is unnecessary.

Take a complete gauge-invariant old scalar \(F_X\) of norm \(a_X\), holomorphic in the actual old variables with the stated slack. In the ball of radius \(c\alpha\), the linear coefficient at the vacuum vanishes by constant color conjugation. One-variable Cauchy along bounded directions and its polarized two-direction version thus give
\[
 |F_X(A_o,J_l)-F_X(0,0)|\le C a_X\alpha^{-2}\|(A_o,J_l)\|_*^2,\qquad
 |\partial_y F_X|\le C a_X\alpha^{-2}\|(A_o,J_l)\|_*
                                   \|\partial_y(A_o,J_l)\|_* .
\]
The bound uses the analytic line with the current varied independently as in (1.9). On \(D\xi\le c_0\) the actual field norm fits the inner ball by the choice of \(\epsilon\). On larger carriers in the common flat chart use \(A_o=\xi A\) without the linear gauge correction. The old norm and its one-anchor variation are then bounded by \(C\epsilon\xi\) and \(C\xi e^{-c(R-CD\xi)}\), with the exact current included. The two powers of \(\xi\) lost in the resulting quadratic bound are restored with \(1\le c_0^{-2}D^2\xi^2\). Periodic carriers without a contractible chart keep their winding remainder as in §4.40 unless the common flat chart actually holds. For small \(\delta>0\) take \(c\) small enough that the positive exponential in \(D\) uses at most \(e^{\delta D}\).

For a tuple of \(m\ge1\) external slots, differentiate once at a most distant slot and apply Cauchy to the remaining targets exactly as in §4.48. For \(m=0\) subtract the vacuum. On smaller polydiscs, the result is
\[
 \rho^m \sum_{\mathbf y}(1+R)^p
  \left|\partial_{\mathbf y}
      [F_X(U_l(W_l),J_l(W_l))-F_X(I,0)]\right|
 \le C_{m,p}a_X\alpha^{-2}(1+D)^2e^{\delta D}\xi^4 .
 \tag{OLD-GRAPH-SCALAR}
\]
The bound absorbs the fixed small \(\epsilon\). All constants are independent of the mesh separation and torus volume under the displayed margins. In particular this applies to the gauge-invariant first clean scalar source carriers of T1 Theorems 7.44, 7.57 and Proposition 7.67, propagated by any number of subsequent **classical** homogeneous minimizing maps on these charts. The source label of the old scalar is kept in its carrier. There are \(\xi^{-4}\) old roots per current cell, and the rooted exponential sum pays \((1+D)^2e^{\delta D}\). Its vacuum-subtracted quantum first row therefore has an extensive bound in the *current* cell count, with every fixed absolute external moment. This result propagates a genuine fluctuation scalar already born on the first Wilson fiber. It does not perform the subsequent fluctuation integrations or sum their positive history innovations. NATIVE-OLD-CURRENT supplies a localized graph value beyond the homogeneous case; its use for holes, return-scale quantum births and moving boundaries still needs corresponding response and chart estimates.

### 4.50 A real clean innovation of the transported quantum scalar (P/L)

The preceding field estimate can be integrated in a fresh original fluctuation step. Work at terminal identity in the homogeneous real kernel of T1 Lemmas 7.51–7.52 and Corollary 7.66. Their positive precision, common enlarged physical chart and original independent cutoff balls are retained. Write \(V(B)=\exp(i\Psi(g_kB))\) for the actual unit constraint readout, so \(V(0)=I\) and each derivative of \(\Psi\) has its fixed corridor anchor. Assume that the determining old carriers and their old-current graph have the margins of §4.49.

For an old scalar carrier set
\[
 F_X(B)=F_X\bigl(U_l(M^l U_k(V(B))),J_l(M^l U_k(V(B)))\bigr)-F_X(I,0).
\]
In this formula the unmarked fluctuation field is \(B\) and the arguments inside the function on the right are the old normalized minimizing pair. Put \(Q_x(B)=1+\sum_i e^{-c d(x,i)}|B_i|\), with \(x\) the current root cell of \(X\). By T1 Lemma 7.51 every fixed moment of this quantity is uniform under the normalized real selector law. Along the segment from the zero target logarithms to those of \(V(B)\), integrate the single-slot response in OLD-GRAPH-COORDINATES. The resulting value bound on a small carrier gains \(g_k Q_x(B)\) in place of \(\epsilon\). For one derivative in \(B_i\), the remote bound gains \(C g_k e^{-c d(i,x)}\). For large carriers use the uncorrected common gauge with the two factors \(\xi\) as in §4.49. The radius and product-norm estimates used for the Taylor gradient itself remain the original uniform chart estimates. It follows that
\[
 \|F_X(B)\|_{L^p}\le C_p b_X\alpha^{-2}g_k^2\xi^4,\qquad
 \|\partial_{B_i}F_X(B)\|_{L^2}
      \le C b_X\alpha^{-2}g_k^2\xi^4 e^{-c d(i,x)} ,
 \qquad b_X=a_X(1+D)^2e^{\delta D}.
 \tag{OLD-SCALAR-REAL-JET}
\]
All norms here use the same positive clean measure. In particular the \(g_k^2\) arises from the field's vacuum-subtracted first jet and the derivative of the actual readout, without a maximum over the whole cutoff field.

One true fresh vertex is \(V'_k(Y)\), the localized difference of the previously integrated unmarked action in CMP116 Lemma 1, (1.33)–(1.36). T1 Corollary 7.66 obtains on its fixed slack
\(\|\partial_{B_i} V'_k(Y)\|_{L^2}\le C g_k e^{-\kappa d_k(Y)}1_{\{i\in Y\}}\).
Inserting these two gradients in T1 Lemma 7.52's real weighted covariance identity gives
\[
 |\operatorname{Cov}(F_X,V'_k(Y))|
 \le C b_X\alpha^{-2}g_k^3\xi^4
      e^{-c' d(x,Y)-\kappa' d_k(Y)} .
 \tag{OLD-SCALAR-FRESH}
\]
The sum over Gaussian response cells is bounded by convolution of two exponential kernels. The native carrier count in \(Y\) uses the spare part of \(\kappa\). The old-to-current loss is zero after the original old-root count. This is a connected attachment on the actual real fluctuation law and includes the entire unmarked inherited difference in this vertex.

There is also a direct bound for the *whole conditional variance* of this old scalar contribution. Assign each old carrier to an old root \(r\) in it, put \(x(r)\) for its current cell, and let \(f_r\) be a real mark on these roots. Suppose \(\sup_r\sum_{X:\operatorname{root}X=r}b_X\le C_0\), as for a rooted expansion with the stated spare decay. Define
\[
 P_f(B)=\sum_r f_r\sum_{X:\operatorname{root}X=r}F_X(B),\qquad
 v_x=\xi^4\sum_{r:x(r)=x}|f_r|.
\]
For independently tagged first-source carriers the assignment may keep the actual source anchor as root. A bounded enlargement to include that stencil changes only the constants; at the first birth the fine-to-old block has fixed side \(L\). OLD-SCALAR-REAL-JET bounds \(\|\partial_{B_i}P_f\|_{L^2}\) by \(C C_0\alpha^{-2}g_k^2\sum_x e^{-c d(i,x)}v_x\). The real Poincaré inequality for this same convex selector, followed by the convolution Schur bound, therefore yields
\[
 \operatorname{Var}(P_f\mid I,\mathrm{clean})
 \le C C_0^2\alpha^{-4}g_k^4\sum_x v_x^2
 \le C C_0^2\alpha^{-4}g_k^4\,\xi^4\sum_r f_r^2 .
 \tag{OLD-SCALAR-INNOVATION}
\]
The final inequality is Cauchy–Schwarz within the \(\xi^{-4}\) old sites of each current cell. For a bounded periodic mark the right side has current-volume order. At a nonflat terminal field the deterministic background generally adds an \(O(\epsilon g_k)\) gradient before this argument, so the stated \(g_k^4\) variance estimate is for terminal identity. It bounds one actual future quantum integration of the scalar born on the first regular Wilson fiber, after arbitrary intervening homogeneous classical propagation. Joint repeated fluctuating ancestors, the record labels and the terminal mean covariance remain in the full Wilson variance tower.

**Nonflat local moments and innovation.** The moment estimate needed above extends to any actual homogeneous nonflat fiber satisfying the same spare-chart condition (7.113), centered independent ball selectors and a uniform augmented quadratic precision \(H\ge mI\) with exponential Schur bound. Keep the original normalized conditional density. If its nonlinear part is \(V=\sum_X V_X\), interpolate through \(d\mu_t\propto e^{-B^THB/2+tV(B)}1_{\mathcal D}\,dB\). The physical regular neighborhood is chosen so the nonlinear Hessians have total Schur norm at most \(m/2\), by the Cauchy estimate in T1 Lemma 7.52. Along this interpolation the Poincaré and weighted covariance constants are uniform. The gradient at zero obeys \(|D_i V_X(0)|\le C v_X\) by Cauchy on a fixed unit component circle (choose a fixed smaller radius when \(P=1\)). The Hessian bound on the convex product then implies
\[
 |D_i V_X(B)|\le C v_X[1+|X|\sum_{h\in X}|B_h|],\qquad i\in X.
\]
For \(m_t=\max_i|\mathbb E_t B_i|\) the Poincaré inequality gives \(\max_i\|B_i\|_2\le C+m_t\). Consequently the weighted covariance of \(B_i\) with \(V\) has modulus at most \(C\epsilon_s(1+m_t)\), where \(\epsilon_s\) is the rooted smallness in (7.113). Indeed the single gradient slot of \(B_i\) fixes the left endpoint, and the carrier moments on the right are absorbed by spare exponential decay. This covariance is \(d\mathbb E_t B_i/dt\). At \(t=0\) the centered joint Gaussian restricted to the product of symmetric balls has zero coordinate means. Integration and Gronwall's inequality now give \(m_t\le C\) independently of the number of cells and the radius \(P\). Finite volume justifies the interpolation before passage to uniform estimates.

For a real unit coordinate functional \(b_i\), an additional tilt by \(s b_i\) preserves the convexity lower bound and the selector. Its normalized variance is at most \(2/m\) for every real \(s\) by the same Poincaré inequality. Integrating the second derivative of its cumulant generating function gives \(\log\mathbb E e^{s(b_i-\mathbb E b_i)}\le s^2/m\). The preceding uniform means therefore imply all fixed moments of \(Q_x(B)\), uniformly on these nonflat conditional laws as well.

Suppose the actual background target \(V(0)\) and its original readout \(V(B)\) belong to the same homogeneous near-identity regular chart used in §4.49, with \(\|\log V(0)\|_\infty\le C\epsilon\) and the physical canonical derivative of each fixed corridor at most \(C g_k\). The latter is the original unit constraint map in its smaller chart. Decompose the old variables into their value at \(V(0)\) plus the integral of their response to \(\log V(B)-\log V(0)\). The gauge-corrected old coordinate value bound gains \(\epsilon+g_k Q_x(B)\), and the derivative in \(B_i\) still has \(g_k e^{-c d(i,x)}\). The same argument for the uncorrected large-carrier chart and the same root sums yield
\[
 \operatorname{Var}(P_f\mid W,\mathrm{clean})
 \le C C_0^2\alpha^{-4}(\epsilon g_k+g_k^2)^2
       \xi^4\sum_r f_r^2.
 \tag{OLD-SCALAR-NONFLAT-INNOVATION}
\]
This bound is uniform over the stated physical backgrounds. Its contribution can therefore be integrated against the positive undivided law of those records. Arbitrary histories whose conditional kernels fail these precise chart and convexity conditions are outside the result.

### 4.51 The retained conditional mean of the old quantum birth (P/L)

One can estimate the mean itself after removing its inherited classical evaluation. Work on the original real clean kernels of §4.50 with fixed physical cutoff and Cauchy slack, so the canonical radius and its spare analytic margin are both bounded below by \(c/g_k\). Write \(P\asymp g_k^{-1}\) for that radius. At fixed external physical pair the localized original fluctuation action in CMP116 (1.41)–(1.43) has a quadratic-form term with bounded analytic coefficient and a separate bounded analytic scalar term. The former has zero linear jet in \(B\). For the latter the original bound (1.36) and Cauchy on a canonical circle of radius \(c/g_k\) give a linear jet bounded by \(C g_k v_X\), allowing the fixed native carrier constants in \(v_X\). These statements follow on the displayed fixed-slack domains; shrinking physical margins change this factor.

On the full real product of selected balls a three-direction Cauchy estimate for \(V_X\) gives \(|D_iD_jD_h V_X|\le C v_X |X|/P\) for slots in \(X\), with zero otherwise. Indeed the larger chart bounds the function by \(C v_X(1+|X|P^2)\) and supplies a circle of radius \(cP\) in each of three directions. With \(V_o(B)=[V(B)-V(-B)]/2\) and \(V_e=V-V_o\), the linear jet just identified and Taylor's formula about zero imply
\[
 |D_i(V_o)_X(B)|\le Cg_k v_X
      [1+|X|(\sum_{h\in X}|B_h|)^2].
\]
The Hessian at zero of the odd part vanishes by parity. Interpolate from \(V_e\) to \(V_e+tV_o\), \(0\le t\le1\). These potentials are convex combinations of \(V(B)\) and \(V(-B)\) and obey the same small Hessian, covariance and local moment estimates of §4.50. Thus \(\|D_i(V_o)_X\|_{L^2}\le Cg_k v_X(1+|X|)^3\). The covariance of \(B_i\) with \(V_o\), summed over its carriers using the exponential covariance row of T1 Lemma 7.52, is bounded by \(C g_k\). The even law has zero mean at \(t=0\). Integrating the exact normalized derivative gives
\[
  |\mathbb E B_i|\le C g_k .
  \tag{NATIVE-ODD-MEAN}
\]
This argument includes the field-dependent fluctuation Hessian in the even reference. It requires neither a field-independent determinant nor a change in the sharp physical selector.

Set \(F(B)=F_X(U_l(M^lU_k(V(B))),J_l(M^lU_k(V(B))))\) as in §4.50, and retain the actual nonflat \(V(0)\). Taylor's formula in \(B\) about zero separates \(\sum_i D_{B_i} F(0)\mathbb E B_i\) from the second-order integral remainder. In OLD-GRAPH-SCALAR the one-slot derivative multiplied by \(D_B\log V=O(g_k)\) gives \(|D_{B_i} F(0)|\le C b_X\alpha^{-2}g_k \xi^4 e^{-c d(i,x)}\). Applying its two-slot estimate and differentiating the fixed finite-corridor map a second time yields uniformly on \(0\le t\le1\)
\[
 |D_{B_i}D_{B_j}F(tB)|
 \le C b_X\alpha^{-2}g_k^2\xi^4
       e^{-c'\max(d(i,x),d(j,x))}.
\]
Indeed fitting the most distant slot in the direct one-response bound and using Cauchy in the other slot retains this exponential, as in the proof of (OLD-GRAPH-SCALAR). The second readout derivative has a bounded finite corridor and its two canonical slots each supply \(g_k\). All physical target radii are included in \(C\). In the Taylor remainder the expected \(|B_iB_j|\) are uniformly bounded on the true normalized nonflat measure. The double spatial sum is finite by exponential shells. Together with NATIVE-ODD-MEAN this proves
\[
 \left|\mathbb E[F(B)\mid W,\mathrm{clean}]-F(0)\right|
    \le C b_X\alpha^{-2}g_k^2 \xi^4 .
 \tag{OLD-SCALAR-RETAINED}
\]
Thus on this actual clean step the retained mean consists of the old scalar evaluated on the next minimizing field and a newly produced real scalar of relative size \(g_k^2\), after the old root count. Its identity value may be subtracted separately and retained as the correct history-dependent scalar. When the older physical tube shrinks, the relative cost in this bound is \(g_k^2/\alpha_l^2\); the radius ratio and every history scalar must then be accounted for in the full tower. OLD-SCALAR-RETAINED is a real value bound on the normalized conditional mean. To iterate it as a new birth requires its target-response and carrier estimates on its actual new domain.

### 4.52 Cancellation of the alternating comb components on a transported scalar (P/L)

The temporal mark of §4.38 is one eighth of the sum of eight spatial parity characters. Seven have a nonzero momentum in at least one old coordinate. Their cancellation can be retained in the homogeneous old-scalar estimates. Work on the actual common regular chart of §4.49 with the interior first-difference Hölder exponent \(0<\lambda<1\) supplied by CMP102 (9),(190). Use translated copies of the same scalar carrier at old roots \(r\). For a tagged source this translation convention is available whenever the complete labeled integral is equivariant under old-lattice translations. Indeed one can average a rooted decomposition and its translates under the finite old translation group, translating the label and field together. The sum is the same labeled function by equivariance, and convexity preserves each rooted absolute norm. Supports are allowed to be translates of the original carriers with their fixed grid enlargement. On a homogeneous full torus the original constraint map, Wilson action, and clean selectors have this translation covariance at the natural output lattice scale. For an old birth at bounded fine offsets \(b=c+L^l r\), an alternating sign in a chosen physical fine coordinate is a fixed sign times \((-1)^{r_j}\) since \(L\) is odd.

Let \(F_r\) denote the scalar on a fixed carrier shape with root \(r\), with the vacuum removed. For neighboring old roots \(r,r+e_j\), identify their fine stencils by translation (physical distance \(\xi\) in current units). If \(D\xi\le c_0\), use the separate gauges in §4.49 which subtract the constant potential at the respective root. On corresponding stencils the two corrected old potentials differ in old \(C^1\) norm by at most \(C(1+D)^2\epsilon\xi^{2+\lambda}\). Here are the mesh factors. For the uncorrected potential with its base value removed, translate the two arguments by \(\xi e_j\) and telescope the \(\xi/\eta\) fine increments. The first derivatives evaluated at two locations separated by at most \(CD\xi\) differ by \(C\epsilon (D\xi)^\lambda\). Multiplying the resulting difference by \(\xi\) to pass to an old potential yields \(C D^\lambda\epsilon\xi^{2+\lambda}\). For the old first difference, the two corresponding first derivatives differ by \(C\epsilon\xi^\lambda\), and the old-unit normalization is \(\xi^2\).

The extra terms from the linear-exponential gauge have the same or smaller bound. To verify this locally write the relative coordinate as \(h=x-x_r\), the base potential as \(a=A(x_r)\), and \(u_a(h)=\exp(i h\cdot a)\) with the sign of §4.49. The logarithm divided by \(\eta\) of \(u_a(h)e^{i\eta A_\mu(x_r+h)}u_a(h+\eta e_\mu)^{-1}\) equals \(A_\mu(x_r+h)-a_\mu\) plus an analytic remainder. On the small chart the remainder and its derivatives with respect to \(a,A\) are bounded by \(C\epsilon^2(|h|+\eta)\) and \(C\epsilon(|h|+\eta)\), respectively. This follows by expanding the three exponentials: at \(h=\eta=0\) the linear \(A_\mu-a_\mu\) is exact after division by \(\eta\); all remaining terms have at least two fields and a factor of \(h\) or \(\eta\). Translating changes both \(a\) and the field at corresponding points by \(O(\epsilon\xi)\). Differencing in \(h\) differentiates this analytic coefficient or the field and uses its translated first-difference Hölder bound. After the old normalizations these remainders are \(O(C(1+D)^2\epsilon\xi^{2+\lambda})\). The old currents need no extra Hölder theorem: each satisfies \(C\epsilon\xi^3\) on this homogeneous graph, hence their difference has the required bound as well. After one target variation, the same argument uses the weighted Hölder row in (190) for the variation and the differentiated product rule. It gives the corresponding coordinate difference with \(\epsilon\) replaced by \(C e^{-c(R-CD\xi)}\).

Each single old profile is \(O((1+D)\epsilon\xi^2)\). The scalar gradient vanishes at the vacuum and its old Hessian is at most \(C a_X\alpha^{-2}\). The mean-value theorem between the two profiles therefore gives the extra \(\xi^\lambda\) in their difference. For one derivative use
\[
 DF(z_1)\dot z_1-DF(z_0)\dot z_0
 =[DF(z_1)-DF(z_0)]\dot z_1+DF(z_0)(\dot z_1-\dot z_0).
\]
Both terms retain the extra \(\xi^\lambda\) and the one-anchor exponential. Cauchy for the remaining slots and shell summation proceed as before. On large carriers in the common chart use their ordinary bound with \(\xi^2\), and absorb the missing \(\xi^{2+\lambda}\) by \(C(1+D)^{2+\lambda}\) when \(D\xi>c_0\). Thus, for fixed \(m,p\), including \(m=0\),
\[
 \rho^m\sum_{\mathbf y}(1+R)^p
       |\partial_{\mathbf y}(F_{r+e_j}-F_r)|
 \le C_{m,p}a_X\alpha^{-2}(1+D)^5e^{\delta D}\xi^{4+\lambda}.
 \tag{OLD-TRANSLATE-DIFFERENCE}
\]
It is a difference of the evaluated fields on corresponding old determining stencils. Differentiating a rapidly alternating continuum test would give the wrong scaling.

Pair consecutive old roots with opposite signs along coordinate \(j\) within each current cell. Its odd side \(s=\xi^{-1}\) leaves at most \(s^3\) unpaired roots; the other three parity signs are constant on each pair. The leftover terms use OLD-GRAPH-SCALAR. The aggregate absolute external moments per current cell are therefore bounded by
\[
 C\alpha^{-2}C_0\,[s^4\xi^{4+\lambda}+s^3\xi^4]
 \le C'\alpha^{-2} C_0\,\xi^\lambda .
 \tag{COMB-OSCILLATING-SCALAR}
\]
The paired calculation applies also to the real fluctuation derivative in §4.50. On the original nonflat regular fiber the canonical derivative of a pair has \(L^2\) norm at most \(C b'_X\alpha^{-2}(\epsilon g_k+g_k^2)\xi^{4+\lambda}e^{-c d(i,x)}\), with \(b'_X\) absorbing the polynomial and spare carrier decay. For this assertion integrate the translated-coordinate response along target logarithms as in §4.50; the deterministic part has \(\epsilon\) and the fluctuation part has \(g_k Q_x(B)\). The unpaired derivative uses the previously proved \(\xi^4\) bound. The clean Poincaré estimate for the sum over all current cells consequently gives
\[
 \operatorname{Var}(P_{\rm alternating}\mid W,\mathrm{clean})
 \le C C_0^2\alpha^{-4}(\epsilon g_k+g_k^2)^2
                  N_k\,\xi^{2\lambda}.
 \tag{COMB-OSCILLATING-INNOVATION}
\]
The constant component of the comb still has the marginal current-volume contribution, and the full ordinary observable also contains its critical and history rows. This result isolates the extra decay of the seven alternating components of the genuine old scalar on the homogeneous regular graph.

### 4.53 Fixed target jets of the new retained quantum scalar (P/L at the homogeneous identity)

On the homogeneous fixed-slack identity chart one can retain the small \(g_k^2\) of OLD-SCALAR-RETAINED after any fixed number of physical target differentiations. Use the actual combined target, proper axial precision and normalized score estimates in T1 Theorems 7.74–7.75. Their canonical upper target is \(W=\exp(g_k\theta)\); write \(q=g_k\theta\) for the physical logarithm and take derivatives in \(q\). Their \(g_k\) per canonical slot exactly accounts for this conversion. These precision and score statements are used at the identity and on the specified pure regular graph. Only the finite-order estimates below are claimed.

Let \(\mathcal R_X(q)=\mathbb E_q[F(B,q)]-F(0,q)\), for the same old scalar and exact fresh fluctuation fiber as §4.51. The physical external \(q\) enters through the original nonflat current readout and conditional measure. For a fixed set \(I\) of physical target slots \(y_i\), and \(R_I=\max_{i\in I}d(x,y_i)\), the conclusion is
\[
 |\partial_{q_I}\mathcal R_X(0)|
 \le C_{|I|} b'_X\alpha^{-2}g_k^2 \xi^4
                    e^{-c_{|I|}R_I}.
 \tag{RETAINED-QUANTUM-JETS}
\]
Here a fixed polynomial in \(D\) and an arbitrarily small carrier decay loss are included in \(b'_X\). The fixed physical analytic margins enter the constants. All fixed polynomial moments of the external anchors consequently remain summable. We detail how the first and second order remainders of the *observable* Taylor formula retain their powers on the normalized measure.

First differentiate the identity
\[
 a_i(q)=\mathbb E_q B_i=\int_0^1
       \kappa_{t,q}(B_i,V_o)\,dt
\]
from NATIVE-ODD-MEAN. For real \(q\), \(\mu_{t,q}\) uses \(V_e+tV_o\); its symmetric quadratic precision is the same as for \(t=1\). Under a derivative of a normalized cumulant, differentiate each argument once and add one more connected argument \(G_y=\partial_{q_y}\log w_{t,q}\), where \(w_{t,q}\) is the unnormalized positive weight. Repetition gives a finite sum involving higher score derivatives with the labels partitioned among them. Deterministic pieces inside connected scores of order at least two drop out. This identity follows by differentiating the finite-dimensional normalized generating integral at zero auxiliary test sources; finite Taylor jets suffice. The original selectors are frozen in these physical target derivatives.

For every fixed number of external slots the odd vertex and its \(B\)-gradient have \(L^p\) envelopes with an overall \(g_k\). To verify the factor after target differentiation, apply the covariance and external locality of the original two pieces of (1.42) used in T1 Theorem 7.75. The quadratic-form piece still has zero linear jet for every target. The bounded piece still gives a canonical first jet of order \(g_k\) on the fixed physical \(B\)-margin. Third-derivative Cauchy on that margin gives the same \(O(g_k)\) for the Taylor remainder of the differentiated odd gradient, with a fixed polynomial in the \(B\)'s in the carrier. Integrating that gradient from zero controls the odd value as well. T1's one-most-distant-target response estimates and smaller-disc Cauchy retain the spatial exponential to the carrier. The ordinary score vertices have the corresponding fixed \(L^p\) and gradient bounds of order one in physical slots, with their own external anchors. These statements are unchanged by the convex combination with the \(B\mapsto-B\) reflected potential. The moments in §4.50 apply uniformly in \(t\).

T1 Lemma 7.70 bounds the connected cumulant of any fixed number of such anchored functions by their envelope product times a reduced exponential of the anchor diameter. Briefly, split a spanning tree at its longest minimum-tree edge. The two groups are separated by at least the diameter divided by one less than their number. In the partition polynomial for the cumulant, replace each mixed moment by the product of its two group moments. The resulting polynomial vanishes by independence of two copies of the law. Each replacement error is bounded by the real covariance estimate for the two products, using Hölder for their gradients, giving the stated decay. This argument retains the norms of each source vertex and also applies after summing its carrier anchor using spare decay. It follows that the differentiated \(a_i(0)\) is bounded by \(C_{|I|}g_k e^{-c_{|I|}\max_j d(i,y_j)}\), since every term has exactly one odd vertex or its derivative. This step preserves the actual normalized conditional mean.

Now retain Taylor's integral formula in the form
\[
 \mathcal R_X(q)=\sum_i D_i F(0,q)\,a_i(q)
 +\int_0^1(1-t)\sum_{i,j}
    \mathbb E_q[B_iB_j D_iD_jF(tB,q)]\,dt .
\]
Here \(D_i\) means canonical \(B_i\) differentiation. For the first term every finite mixed external derivative of \(D_iF(0,q)\) has a \(g_k\xi^4\) factor and exponential decay to the most distant of \(i\) and its target slots, by §4.49 and the actual combined finite-corridor derivatives of T1 Theorem 7.75. The bound just proved for \(a_i\) supplies the second \(g_k\). The product of these exponentials connects all the slots to the carrier root; spend part of it on summing \(i\). For the second term the observable inside the expectation and each of its fixed target derivatives already have two canonical derivatives and thus \(g_k^2\xi^4\). They have exponentially weighted \(L^p\) and \(B\)-gradient bounds with roots \(x,i,j\): differentiating the two explicit \(B\) factors or differentiating \(F\) once more has this property by the same graph bounds and §4.50. More explicitly keep a part of \(e^{-c\max(d(x,i),d(x,j))}\) for summing \(i,j\) and treat the observable as anchored at \(x\), after a further fixed decay loss. Derivatives of the normalized expectation add only the already controlled scores. Apply the cumulant estimate and sum \(i,j\) to obtain (RETAINED-QUANTUM-JETS). This proves a genuine small newly produced scalar and its finite physical response kernels on the original clean identity graph. A uniform invariant-carrier expansion on the entire external complex domain, and its continuation through mixed records, are additional requirements for iterating it in full.

### 4.54 The true positive-time action smearing on the minimizing field (P/L; reflected transfer C)

The coarse spatial energy in §4.47 can be replaced in the conditional-contrast argument by the classical row of an actual smooth fine Wilson action test. Let \(\mathcal P_+\) be the stopped spatial \(12\)-plaquettes based on the positive slice \(j\) of §4.35. Under one original averaging step choose for each coarse plaquette the coordinate box spanned by its endpoint blocks, their connecting straight segments and their contour frames. The coordinate tree, loop fillings and all plaquette stencils in the proof of NONLINEAR-CURL-STEP can be kept inside that box. Define its immediate fine ancestors as the plaquettes in this rectangle, and take unions when there are several coarse plaquettes. Neighboring coarse rectangles have uniformly bounded overlap for fixed \(L\).

For any subset \(\mathcal P\) of the coarse plaquettes, restrict the nonnegative square-filling operator \(\mathcal R_2\) to its rows and their immediate fine ancestors. Its \(\ell^2\) norm is at most one by the same row and column sums as §4.44. The squared sum over those rows of the nonlinear errors is at most \(C_L\delta^2\sum_{\rm ancestors}s_p\) by the overlap bound. Converting logarithmic norms to the Wilson energy as in CURL-STEP-BUDGET yields
\[
 \sum_{P\in\mathcal P}s_P(MU)
 \le(1+C_L\delta)\sum_{p\in\operatorname{anc}(\mathcal P)}s_p(U).
\]
On \(U_K(W)\) the regularity radii along the successive original averages have bounded sum by §4.44. Consequently
\[
 \sum_{P\in\mathcal P_+}s_P(W)
 \le e^{C_L\epsilon}\sum_{p\in\operatorname{anc}^K(\mathcal P_+)}
                             s_p(U_K(W)).
 \tag{LOCAL-CLASSICAL-ENERGY}
\]
The bound is uniform in the depth. In particular it has no factor \(C_L^K\).

The fine time support can be specified using the actual contour geometry of [CMP109, (0.4),(0.11),(0.12)](https://doi.org/10.1007/BF01215223). Each frame path from a block center to a site consists of coordinate segments within that block. The middle straight segment between the two translated endpoints stays between their blocks. The time projection of a chosen fine ancestor rectangle is therefore contained in the union of time blocks of the parent's endpoint times, with intermediate points if it is a temporal plaquette. The stopped spatial plaquettes have all endpoints at time \(j\). Repeated centered odd-\(L\) subdivisions nest; if a temporal edge subsequently occurs, both child endpoint blocks still belong to the original parent time block. Induction puts all the ancestral vertices in the stopped time slab centered at \(j\), of half-width at most \(\ell_0/2\) in physical units. Torus spatial wrap does not change this time support. Choose \(0\le f\le1\), spatially constant, smooth, supported strictly in the positive half and identically one on that slab. The separation conditions of §4.35 give room for this choice. With the same plaquette-center sampling at fine mesh the entire ancestor set receives weight one. This gives the actual classical inequality
\[
 g^{-2}S_f(U_K(W))\ \ge\
 e^{-C_L\epsilon}g^{-2}\sum_{P\in\mathcal P_+}s_P(W) .
 \tag{PHYSICAL-CLASSICAL-POSITIVE-ROW}
\]
Here \(g^{-2}=\beta_*\) is the chosen stopped normalization. This row is the fine Wilson action integrated against \(f\) at the true regular minimum. A factor representing the actual operator's renormalization still has to multiply it.

To apply §4.47 let \(A_{\rm cl}(W)=g^{-2}S_f(U_K(W))\) on the named regular branch, extended by zero off that branch for purposes of comparison. On every regular field \(0\le A_{\rm cl}\le S_*/g^2\). The classical regularity bound on the fine plaquettes also gives \(S_*\le C_{N_*}\) uniformly in \(K\). Under TERMINAL-DENSITY the unconditional tail of \(S_*/g^2\) on that branch is bounded by \(C g^{-d}e^{-u/2}\) above \(u\), using the regular compact Haar volume and the normalization lower bound of §4.47. The absolute remainder times \(A_{\rm cl}\) is at most \(C g^{-2-d}e^{-c/g^2}\). Therefore \(\mathbb E A_{\rm cl}\le C(1+\log(1/g))\). On the regular joint window selected in §4.47 the coarse energy on the right side of PHYSICAL-CLASSICAL-POSITIVE-ROW is bounded below by \(c R^2\), and its conditional mass in \(E_R\) is bounded below uniformly in \(K\). Nonnegativity elsewhere then gives, for the \(R^2=A(1+\log(1/g))\) of that section with sufficiently large \(A\),
\[
 d_{\rm cl}=\mathbb E(A_{\rm cl}\mid E_R)-\mathbb E A_{\rm cl}
 \ge cR^2-C(1+\log(1/g))>0 .
 \tag{CLASSICAL-ACTION-CONTRAST}
\]
Although the original fine smearing \(f\) is supported in the positive half, its minimizing-field conditional row can depend on the whole terminal configuration. Only the fine observable and the opposite testing event require half support in the reflected Cauchy–Schwarz inequality.

There is an explicit negative-half observable even outside the regular charts. Recursively form the native coarse fields needed for the negative spatial paths only, on their own ancestral negative slab. When a required group average or logarithm leaves its admitted real chart, set a failure flag and choose the straight endpoint path as a Borel fallback. The flag and the admitted orbit-invariant readouts depend only on original negative-half links. Impose success in the definition of the negative Cartan annulus event \(E_R^-\). On regular fibers where the exact constraint readouts equal these repeated admitted averages, \(E_R^-\) agrees with the stopped event. If agreement is only proved on an underlying positive set, the probability and weighted expectations of its complement must be estimated before using (CLASSICAL-ACTION-CONTRAST). For example an absolute positive probability at most \(C g^{-d}e^{-c/g^2}\) there bounds the event error and the comparison error of the bounded \(A_{\rm cl}\), uniformly against the fixed-power annulus mass. An abstract signed terminal-density remainder alone does not identify a positive underlying defect set.

Finally, for the actual normalized, positive-time action insertion \(A_a(f)\), testing against \(E_R^-\) yields a precise remaining target. On the matched terminal readout write its conditional row \(m_a(W)=\mathbb E[A_a(f)\mid W]=c_a+z_a A_{\rm cl}(W)+Q_a(W)\). This identity simply defines the remainder once a normalization and \(z_a\) have been chosen. If the event is a function of \(W\) on the full matched law, then its contrast is \(z_a d_{\rm cl}+\mathbb E(Q_a\mid E_R)-\mathbb E Q_a\). More generally include the discrepancy of the events in this signed contrast for the actual joint law. If \(|z_a|\ge z_0>0\) and the modulus of that combined error is at most \(z_0d_{\rm cl}/2\), REFLECTED-EVENT proves a fixed positive lower bound. The explicit minimizing-field part now has the correct smooth action-density smearing and a proved lower contrast. Its actual coefficient, the signed fluctuation and history correction, and the fieldwise stopping comparison used here remain open.

There is an exact free-field check for this **same smooth fine test** and the same original blockings. Use the periodic canonical Gaussian law of §4.35 and put \(A_f=(\tau/2)\sum_{p,a}f_p|\mathcal F^a_p|^2\), \(\mathcal F=dA\). Write \(Y_+\) for one unit spatial magnetic Fourier mode on the positive stopped slice, with colors kept separately. The original square-filling maps express it as \(Y_+^a=\sum_p w_p\mathcal F_p^a\) on the fine positive ancestors with \(\sum_p|w_p|^2\le1\), since every intermediate linear \(\mathcal R_2\) has norm at most one and the final Fourier vector is normalized. Use a real Fourier vector as in §4.35. Then Wick's formula, the test's value one on the ancestors, and Cauchy–Schwarz give
\[
 \operatorname{Cov}_G(A_f,|Y_-|^2)
 =\tau d_G\sum_p f_p
       |\mathbb E_G(\mathcal F^1_pY_-^1)|^2
 \ge \tau d_G\,|\mathbb E_G(Y_+^1Y_-^1)|^2
 \ge \tau d_G c_*^2 .
\]
Here \(d_G=\dim SU(N)\) counts independent color components. The centered reflection norm of \(|Y_+|^2\) is at most \(2d_G\sigma_{\max}^4\) by the fixed same-slice variance bound. Reflected Cauchy–Schwarz in the positive free gauge-invariant algebra thus yields
\[
 G^\theta_G(A_f,A_f)\ \ge\
       \frac{\tau^2d_G\,c_*^4}{2\sigma_{\max}^4}>0
 \tag{PERIODIC-FINE-ACTION-GRAM}
\]
through every original linearized blocking on the fixed physical torus. A sharper direct calculation avoids the divided reflected norm. Wick's formula writes the left side as \((\tau^2d_G/2)\sum_{p,q}f_pf_q|\mathbb E_G(\mathcal F_p^1\theta\mathcal F_q^1)|^2\). On the ancestors the two weights equal one. Pair this covariance matrix with \(w\otimes w\), whose Euclidean norm is at most one. Its pairing is \(\mathbb E_G(Y_+^1Y_-^1)\), including the reflected orientation of the plaquette. It follows that \(G_G^\theta(A_f,A_f)\ge(\tau^2d_G/2)c_*^2\). Equivalently the exact Gaussian conditional expectation of \(A_f\) given the coarse field consists of its value on the orthogonal minimizing extension and the field-independent trace of the conditional covariance. That trace drops out of the opposite-event contrast even if its coincident-cutoff size grows. Nonflat regular quantum records need the signed remainder estimate in CLASSICAL-ACTION-CONTRAST.

### 4.55 All contact orders on a single compact-support test class (P implication and first-fiber application)

A fixed test norm can control the growth of the diagonal Taylor order with the number of irrelevant insertions. For \(\sigma>1\) and fixed \(H>0\) use the Gevrey norm
\[
 \|f\|_{\sigma,H}
 =\sup_{n\ge0}\frac{\|D^n f\|_{\rm op,\infty}}{H^n(n!)^\sigma}.
\]
Compactly supported tests exist in this class for sufficiently large \(H\) relative to the requested support. For instance convolve normalized interval indicators of half-width \(r_j=cj^{-\sigma}\). The supports sum to a finite interval. Differentiating the first \(n\) factors once each gives signed measures of total variation \(r_j^{-1}\); keeping the next factor as a bounded density and convolving the rest gives \(\|D^n f\|_\infty\le(2r_{n+1})^{-1}\prod_{j=1}^n r_j^{-1}\le C^{n+1}(n!)^\sigma\). Keeping another bounded-density factor also makes each derivative continuous. Product kernels, periodization, and convolution with the indicator of a slightly larger box give positive-half tests equal to one on a smaller slab, including the smearing in §4.54. A fixed \(\sigma,H\) can be used for all engineering dimensions.

Suppose that every dimensionally normalized \(m\)-source scale kernel, with one site anchored, satisfies the absolute bound
\[
 \sup_x\int |K_{k,m}(x,d\boldsymbol u)|
                  e^{\gamma\mathcal T(\boldsymbol u)/\ell_k}
 \le A_D^m(m!)^{\nu_D}\ell_k^{-w},\qquad
 w=\sum_{i=1}^m d_i-4(m-1).
 \tag{CONTACT-ALL-KERNEL}
\]
Here \(\mathcal T\) is the minimum tree length of all \(m\) locations including the anchor. A lattice anchor integral has its physical volume element. Assume integer dimensions \(d_i\le D\). If \(w\ge0\), subtract the anchored relative Taylor polynomial of degree \(w\) as a diagonal local functional, exactly as in Theorem 3.6. If \(w<0\), retain the entire kernel. This produces, after summing scales,
\[
 |B^{\rm sub}_{a,m}(f_1,\ldots,f_m)|
 \le C_D^m(m!)^{\,\nu_D+\sigma\max(D-4,0)}
         \prod_i \|f_i\|_{\sigma,H}.
 \tag{ALL-CONTACT-GEVREY}
\]
Constants depend also on \(\gamma,H,\sigma,L,\ell_0\) and the fixed reference volume. This is a bound on the contact-renormalized joint functional, in the sense of §§4.1 and 4.17.

Indeed put \(q=w+1\) for \(w\ge0\). For each tuple take shortest periodic displacement vectors from the anchor; at a tie one can average over minimal lifts. Their lengths are bounded by \(\mathcal T\). The derivative along \(t\mapsto\prod_{i=2}^m f_i(x+t u_i)\), divided by \(q!\), is bounded by
\[
 2^{q+m}(H\mathcal T)^q(q!)^{\sigma-1}
                         \prod_{i=2}^m\|f_i\|_{\sigma,H}.
\]
The product rule divides each directional derivative by its own factorial, the factors \(\prod_i(n_i!)^{\sigma-1}\) are bounded by \((q!)^{\sigma-1}\), and the number of weak compositions of \(q\) is at most \(2^{q+m}\). Taylor's integral remainder has the same bound. The elementary exponential moment inequality \(s^q\le q!\,e^s\) with \(s=\gamma\mathcal T/\ell_k\) now gives \(C^{q+m}(q!)^\sigma\ell_k^{q-w}\) times the input majorant and test norms. The gain is \(\ell_k\); if \(w<0\), \(\ell_k^{-w}\) supplies at least this gain at small scales because \(w\) is integral. The finitely many scales larger than one in fixed units cost at most a further \(C_D^m\). Since \(q\le m\max(D-4,0)+5\), the multinomial inequality \((dm)!\le d^{dm}(m!)^d\) and a fixed polynomial for the additional five derivatives give the asserted exponent. For \(m=1\) there are no relative variables and the scalar one-point term is fixed by its chosen vacuum normalization. Averaging over anchor choices and lattice symmetries changes no norm. The subtracted polynomial is local even when the original kernel has exponential tails or periodic winding.

The type-specific subtraction order depends on the actual \(d_i\), so enlarging the type cutoff leaves all previously fixed diagonal prescriptions compatible. Strictly separated supports still annihilate these local terms. For arbitrary smooth tests at any *fixed* \(m\) the same argument gives a continuous distributional bound using \(C^{q}\) norms, without a Gevrey restriction. The uniform all-order estimate uses the indicated stronger common norm; it is not an estimate in an a priori specified fixed \(C^5\) norm for all irrelevant types.

For the actual first constrained Gaussian step, restore the canonical dimension factor of each local polynomial in HIGH-GKT. Its engineering-density factor \(\ell_k^{-d_i}\) multiplied by the relative integration measures \(\ell_k^{4(m-1)}\) gives exactly \(\ell_k^{-w}\). Explicit additional coupling or normalization grades are retained as products of their actual per-insertion factors. HIGH-GKT then gives CONTACT-ALL-KERNEL at that step with \(\nu_D=\max(1,q_D/2)\) for the chosen finite degrees \(q_D\). The first clean quadratic \(H\) source also has this exponential kernel majorant at all source orders on the fixed admitted original chart by §4.16 and T1's first-step polymer construction, with its explicit normalization. ALL-CONTACT-GEVREY applies to these sectors with one source-order-independent test norm. It does not manufacture CONTACT-ALL-KERNEL for the missing interacting histories or identify the full triangular physical mixing matrix.

### 4.56 Quantitative zeros for the program's bare physical \(H\) source (P)

The obstruction to a fixed bare source disc reaches the precise physical insertion in §2, with a quantitative mesh rate. It is useful to separate this from the remaining unamplified comb variance.

Here is a general elementary estimate. Write \(V=n^4\) and let \(D_V\) be a real compact-lattice function with \(|D_V|\le M V\). Suppose its product-Haar distribution gives \(\mathbb P_{\rm Haar}(D_V\ge bV)\ge p>0\), and under the Wilson law \(\mathbb E_\beta D_V/V\le b/4\). The total Wilson action is between zero and \(C_S V\), and the Haar-normalized partition function is at most one. For every \(\lambda>0\), the complex exponential moment \(Z(z)=\mathbb E_\beta e^{z\lambda D_V}\) has a zero in
\[
 |z|\le C_{M,b,C_S,p}\frac{\beta+1}{\lambda}.
 \tag{COMPACT-SOURCE-ZERO}
\]
Indeed on any zero-free disc of radius \(R\) define \(F(z)=\log Z(z)/(\lambda V)\) with \(F(0)=0\). Then \(\operatorname{Re}F\le MR\). The map \(F/(2MR-F)\) has modulus at most one and vanishes at zero, so Schwarz's lemma gives \(|F|\le2MR\) on the radius-\(R/2\) disc. Taylor's Cauchy bound now gives \(F(t)\le F'(0)t+16M t^2/R\) on \(0<t\le R/4\). On the other hand the Haar event and the Wilson weight give
\[
 F(t)\ge bt-\frac{C_S\beta}{\lambda}
              -\frac{\log(1/p)}{\lambda V}.
\]
Take \(t=K(\beta+1)/\lambda\) with \(K\) large enough that \(F(t)\ge3bt/4\). If \(R\ge4t\), comparison yields \(R\le32Mt/b\). Otherwise \(R<4t\) already. The moment is entire on this finite compact system, so this upper bound on every zero-free radius implies the claimed zero. The proof uses only first moment and compact real tilts, without a thermodynamic-limit analytic continuation.

Apply the estimate to \(d_b=h_b/\beta=(1/3)\sum_{i<j}|F_{b,i}-F_{b,j}|^2\). The local force is bounded by a group constant and \(\mathbb E_{\rm Haar}d_b\ge b_0>0\) uniformly on sufficiently large periodic tori. For an explicit nonzero value fix one link \(b\), keep its local stencil at identity except for the opposite parallel link of one forward plaquette, and put that link at \(\exp(\varepsilon T)\) with a fixed nonzero traceless anti-Hermitian generator and small real \(\varepsilon\). The two other matching forces at \(b\) vanish, while the chosen plaquette force has a nonzero first-order color component. The opposite backward plaquette is still the identity. Continuity and positivity of Haar measure on open cylinder sets give the lower expectation independently of the number of lattice sites. For \(D_V=\sum_b f_b d_b\), take \(0\le f_b\le1\) with \(\sum_b f_b\ge c_f V\). The bounded variable \(D_V/V\) has a fixed positive Haar mean, hence a fixed positive Haar probability above half that mean. This includes a constant smooth source, smooth marks of positive spacetime mean, and the temporal eight-site pattern. H-LOCAL and FIRST give \(\mathbb E_\beta D_V/V\le C/\beta\) on the stated trajectory. We may take \(\beta\) sufficiently large for the preceding lemma.

In the program convention \(c_\beta=2N\) is the fixed coupling-normalization constant and \(O_H(f)=c_\beta^{-1}a^{-2}\sum_b f_b h_b\). The amplification is \(\lambda=c_\beta^{-1}\beta a^{-2}\). COMPACT-SOURCE-ZERO gives
\[
 \inf\{|z|:\mathbb E_\beta e^{z O_H(f)}=0\}\le C_f a^2
 \qquad(\beta\to\infty).
 \tag{PHYSICAL-H-ZERO}
\]
The same conclusion holds for the bare ordinary \(r_H(f)\): \(r_b/\beta=D_b-\ell_b/(3\beta)\), where the first term is the bounded matching force-square sum and the second is uniformly \(O(\beta^{-1})\). Its Haar high-value event and small Wilson expectation follow by the same local example, H-LOCAL's force estimate and FIRST. For the dimension-eight example of §4.42 take \(D_V=\sum_p s_p^2\), \(\lambda=a^{-4}\). The Haar event is again immediate from its strictly positive local mean, and \(s_p^2\le C s_p\) gives the required Wilson smallness. Its nearest zero is at most \(C(\beta+1)a^4\).

An entire scalar contact multiplier cannot remove any of these zeros. This rules out a cutoff-independent log-pressure disc if I-1 is interpreted as applying at the bare physical \(H\) normalization even to a constant smooth source. It supplies only a fixed-order upper bound for the radius of the **unamplified** \(h_{f^{\rm comb}}\), consistent with a possible positive smaller uniform radius there. It does not disprove ordinary extensive variance, a finite-jet subtraction, or estimates after the additional \(a^4\) rescaling required by the program.

**Robustness under linear plaquette mixing.** For the standard compact Wilson representatives even arbitrary orientation-dependent linear plaquette rows cannot rescue the bare physical disc. On an even torus write \(S_{\mu\nu}=\sum_x s_{\mu\nu}(x)\), \(D=\sum_b h_b/\beta\), and consider
\[
 Y=A_D D+\sum_{\mu<\nu} A_{\mu\nu} S_{\mu\nu}+A_{\bf1}
\]
with real coefficients which may depend on the mesh. Let \(A=\max(|A_D|,\max_{\mu<\nu}|A_{\mu\nu}|)>0\). Drop the deterministic scalar for the zero locations. There is a group-dependent \(C\), independent of these coefficients, such that for weak \(\beta\)
\[
 \inf\{|z|:\mathbb E_\beta e^{zY}=0\}\le C(\beta+1)/A .
 \tag{PLAQUETTE-MIXED-ZERO}
\]

For each plane \(\mu\nu\) choose a nontrivial central \(z_0\in SU(N)\) and set \(U_\nu(x)=z_0^{x_\mu\bmod2}\), all other directions at identity. Only the \(\mu\nu\) plaquettes differ from identity, taking the two center values \(z_0^{\pm1}\). Every matching force vanishes since the derivative of the real trace of a center element in a traceless direction is zero. Thus \(D/V=0\), \(S_{\mu\nu}/V=N-\operatorname{Re}\operatorname{Tr}z_0>0\), and all other orientation averages vanish. A seventh configuration has \(U_\nu(x)=\exp(i\varepsilon T(-1)^{x_\mu})\), with fixed traceless Hermitian \(T\ne0\), all other directions at identity. On a \(\nu\)-link the two incident \(\mu\nu\) plaquette angles are \(2\varepsilon\) and \(-2\varepsilon\), up to an overall sign. Differentiating that one link in direction \(T\) gives opposite orientation signs on those plaquettes. Their two action derivatives add, with modulus \(4\varepsilon\operatorname{Tr}T^2+O(\varepsilon^3)\). Every other matching force there vanishes. Hence \(D/V\ge c_N>0\) for a fixed small \(\varepsilon\), independently of the side. The \(7\) vectors of intensive values of \((D,S_{\mu\nu})\) form an invertible real matrix. Consequently at one of these configurations the normalized combination \((Y-A_{\bf1})/(AV)\) has absolute value at least \(2b>0\) uniformly over the normalized coefficient vector. Change overall sign if necessary.

Require each link to stay in a fixed small Haar ball about its value in this configuration. Every local summand in the normalized combination has a uniformly bounded derivative and uniformly bounded stencil. The signed value is at least \(b\) throughout that event, and its Haar probability is at least \(e^{-C_0 V}\). In the proof of COMPACT-SOURCE-ZERO this event cost contributes \(C_0/A\) to the real lower bound; the same choice \(t=K(\beta+1)/A\) absorbs it. The normalized Wilson mean has absolute value at most \(C/\beta\) by FIRST and the matching force estimate. The signed proof applies, and a zero for the sign-reversed variable is reflected to a zero for \(Y\). This proves PLAQUETTE-MIXED-ZERO. For the normalized ordinary \(\sum r_b/\beta\) the six center-stripe first components are \(O(\beta^{-1})\) and the noncentral one is bounded away from zero. The same uniform invertibility and estimate hold for sufficiently large \(\beta\).

In particular if \(Y\) contains \(z_H(a) O_H(1)\), then \(A\ge |z_H(a)|\,c_\beta^{-1}\beta a^{-2}\). A uniform physical zero-free disc would require \(|z_H(a)|\le C a^2\) even after adding arbitrary standard Wilson plaquette orientations, an identity row and zero-free scalar contact factors. This statement concerns these explicit compact representatives at constant test. Alternative operator-valued nonlinear source changes must be analyzed through their own generating functions.

### 4.57 Exact single-link disintegration for the temporal comb (P)

The eight-site geometry gives an exact positive disintegration of the full Wilson law, including arbitrary nonregular backgrounds. Let \(\mathcal C\) be the selected temporal links, all times and one spatial parity class. No Wilson plaquette contains two members of \(\mathcal C\): a temporal plaquette's two temporal edges are nearest spatial neighbors. Let \(\mathcal E\) record all links outside \(\mathcal C\). The selected links are then conditionally independent. Moreover \(r_b,h_b\) for a selected \(b\) depend on no other selected link. This is an exact original Wilson conditional expectation, without selector or gauge cutoff.

For fixed exterior write \(W_{i,\pm}\in SU(N)\) for its six oriented staples with \(u=U_b\) in the convention that the \(b\)-dependent part of the action is \(-\operatorname{Re}\operatorname{Tr}(u^\dagger K)\), \(K_i=W_{i,+}+W_{i,-}\), \(K=\sum_i K_i\). Conditioned on \(\mathcal E\), \(u\) has density \(e^{\beta\operatorname{Re}\operatorname{Tr}(u^\dagger K)}/\mathcal Z(K)\) relative to Haar. Single-link integration by parts makes its ordinary and frustration means exactly equal, since \(h_b-r_b\) is the total-force Ward row. Define their common value
\[
 m_b(\mathcal E)=\frac{1}{3\beta}\sum_{i<j,A}
  \frac{D^2\mathcal Z(K)[T_A(K_i-K_j),T_A(K_i-K_j)]}{\mathcal Z(K)},
 \quad
 \mathcal Z(K)=\int_G e^{\beta\operatorname{Re}\operatorname{Tr}(u^\dagger K)}\,du .
 \tag{SINGLE-LINK-MEAN}
\]
Here \(T_A\) are the anti-Hermitian generators of the left variations and \(D\) is the real matrix derivative of the single-link integral. Indeed \(X_A S_i=\operatorname{Re}\operatorname{Tr}(u^\dagger T_A K_i)\); the two directional derivatives reproduce \(\beta^2\) times its squared matching difference. The denominator is strictly positive for every real exterior. Conditional independence and variance decomposition now give for marks supported on \(\mathcal C\)
\[
 \operatorname{Var}(r_f)=\sum_{b\in\mathcal C}f_b^2
       \mathbb E\operatorname{Var}(r_b\mid\mathcal E)
       +\operatorname{Var}\left(\sum_{b\in\mathcal C} f_b m_b(\mathcal E)\right).
 \tag{SINGLE-LINK-TOWER}
\]
The corresponding identity for \(h_f\) has exactly the same retained-field term. Thus boundedness of the ordinary susceptibility reduces to this particular explicit local field on the unselected links, under their actual Wilson marginal.

There is a sharp weak-coupling asymptotic for the first term. Use the invariant metric of the paper, \(s(e^A)=(\tau/2)|A|^2+O(|A|^4)\), and \(d_G=\dim SU(N)\). Under FIRST and the marked fourth-moment bound of §4.22, on its compatible weak reference trajectory,
\[
 \mathbb E\operatorname{Var}(r_b\mid\mathcal E)\longrightarrow8\tau^2 d_G,
 \qquad
 \mathbb E\operatorname{Var}(h_b\mid\mathcal E)\longrightarrow0.
 \tag{SINGLE-LINK-INNOVATION-LIMIT}
\]
The errors are uniform along the mesh sequence for each selected link. We give the argument because the leading ordinary variance is real local noise, despite the vanishing leading conditional variance of the frustration.

Set \(u_0=W_{1,+}\). With exterior probability at least \(1-C/D^2\) all six staples are within distance \(D/\sqrt\beta\) of \(u_0\), increasing the geometric constant if necessary. In the full Wilson field the distance of each staple to the actual link is controlled by its incident plaquette, \(d(U_b,W_{i,\pm})^2\le Cs_p\), by compactness and the local quadratic minimum. Use FIRST and the triangle inequality; the resulting good event is exterior-measurable. For fixed \(D\) write \(W_{i,\pm}=u_0\exp(Z_{i,\pm}/\sqrt\beta)\), with \(Z_{i,\pm}\) bounded by \(C D\), and define \(Z_i=(Z_{i,+}+Z_{i,-})/2\), \(\bar Z=(Z_1+Z_2+Z_3)/3\).

In \(u=u_0\exp(X/\sqrt\beta)\) coordinates the conditional action tends, up to a constant, to \((\tau/2)\sum_{i,\pm}|X-Z_{i,\pm}|^2\). The corresponding limiting Gaussian has mean \(\bar Z\) and covariance \((6\tau)^{-1}I\). The \(\sqrt\beta\)-rescaled matching gradient in common color coordinates is \(2\tau(X-Z_i)\), up to the fixed adjoint rotation caused by \(u_0\). The total link Laplacian tends to \(6\tau d_G\). Consequently the two ordinary functions converge in these coordinates to
\[
 r_b\ \rightsquigarrow\
 12\tau^2|X-\bar Z|^2+4\tau^2\sum_i|Z_i-\bar Z|^2-2\tau d_G,
 \qquad
 h_b\ \rightsquigarrow\ 4\tau^2\sum_i|Z_i-\bar Z|^2.
\]
All moment comparisons here are uniform for \(|Z_{i,\pm}|\le CD\). For details one can use the Wilson action lower bound \(s(uv^\dagger)\ge c d(u,v)^2\), with \(d\) a fixed bi-invariant distance. The good conditional action then bounds the scaled density by \(C_D e^{-cD(u,u_0)^2\beta}\), with \(D(u,u_0)\) denoting this distance. Its Haar integral has lower bound \(c_D\beta^{-d_G/2}\) from a ball of radius \(\beta^{-1/2}\). In the principal compact chart the Jacobian is bounded and converges to its value at zero. The link force is bounded by a fixed multiple of the sum of the six incident distances, so the required squares are dominated by fixed polynomials of \(|X|+D\) times a Gaussian. The rest of the compact group outside that chart has an exponential tail even after these polynomial factors. Taylor's formula on fixed bounded \(X,Z\) followed by uniform tail truncation proves the two moment limits without choosing convergent exterior sequences.

The Gaussian variance of \(12\tau^2|X-\bar Z|^2\) is \(8\tau^2d_G\); the frustration limit is constant on this fiber. On the bad exterior, Cauchy–Schwarz and the uniform full-Wilson fourth moment of each original insertion bound its contribution to the averaged conditional variance by \(C/D\). Let \(\beta\to\infty\) at fixed \(D\), then \(D\to\infty\). This proves SINGLE-LINK-INNOVATION-LIMIT. It also identifies the exterior mean's leading value \(4\tau^2\sum_i|Z_i-\bar Z|^2\) on each bounded good exterior. No claim about the variance of the sum of the local approximation errors follows from a one-link limit.

In particular, uniformly for all marks supported on this one class, the extensive ordinary-minus-frustration contact equals \((8\tau^2 d_G+o(1))\sum_b f_b^2\). The entire uncontrolled part of the comb susceptibility is common to \(r\) and \(h\) and is the ordinary covariance sum of SINGLE-LINK-MEAN. The positive ordinary lower bound here is an innovation under the original real law. It does not give a reflected Gram lower bound.

**A sharp obstruction on fixed exterior fields.** There are admissible compact exteriors on which the unamplified comb cannot have a background-uniform zero-free disc or a uniform conditional one-link variance. Fix one selected \(b\), take all adjacent spatial links in the two endpoint slices to be identity, and choose its two neighboring temporal links in spatial direction \(i\) so that the two staples are both \(V_i\). They are unselected distinct links on a sufficiently large even torus. For \(SU(2)\) put \(V_i=\exp(2\pi i(i-1)\sigma_3/3)\), with \(\sigma_3\) the Pauli matrix. The total staple matrix is zero, so the conditional law of \(u\) is Haar and the total-force gradient and Laplacian vanish identically. Hence \(r_b=h_b\).

Write \(u\in SU(2)\) as a unit quaternion \((u_0,u_1,u_2,u_3)\), and \((i\sigma_1,i\sigma_2,i\sigma_3)\) times the common speed \(v>0\) for the invariant-generator frame, following any orthogonal color rotation. The matching action is a constant minus \(4u\cdot V_i\). The squared spherical gradient of \(u\cdot V_i\) is \(1-(u\cdot V_i)^2\), with an extra factor \(v^2\) for the chosen generator speed. The three unit vectors \(V_i\) span the \(0,3\) plane and form a tight frame there, giving
\[
 h_b/\beta=16v^2\left(3-\tfrac32(u_0^2+u_3^2)\right).
\]
For uniform \(S^3\), \(u_0^2+u_3^2\) is uniform on \([0,1]\), as follows by normalizing four independent standard real Gaussians and taking the ratio of the two independent equal-scale \(\chi^2_2\) variables. Thus the conditional variance is \((24v^2\beta)^2/12\) and the conditional exponential moment has zeros at \(2\pi i m/(24v^2\beta)\), \(m\in\mathbb Z\setminus\{0\}\). The zeros are simple. Real exterior perturbations by \(o(1/\beta)\) alter the rescaled-source integrals uniformly on compact sets in the variable \(\beta z\) by \(o(1)\) because the original total tilt becomes \(o(1)\); the matching force polynomials are uniformly continuous. Rouché's theorem on a fixed small circle preserves a nearby zero. For each sufficiently large \(\beta\), such open neighborhoods have positive full Wilson marginal mass.

There is also an obstruction for every \(SU(N)\), \(N\ge3\). Take \(V_1=I,V_2=W,V_3=W^\dagger\), with \(W\) diagonal of eigenvalues \(\omega,\omega^{-1}\), \(\omega=e^{2\pi i/3}\). Choose the number of \(\omega\) entries in \([0,N]\) congruent to \(2N\) modulo three, ensuring \(\det W=1\). Again \(K=0\). The variable \(h_b/\beta\) is nonconstant under Haar. Indeed, along diagonal \(u\) with phases \(\theta_h\) of sum zero, all off-diagonal gradients vanish, and summing the squared traceless diagonal gradients in the three directions gives, up to a fixed positive metric factor,
\[
 N-\frac1N\left[\left(\sum_h\sin\theta_h\right)^2+
                       \left(\sum_h s_h\cos\theta_h\right)^2\right],
\]
where \(s_h=\pm1\) is the sign of the corresponding eigenphase of \(W\). Choose two entries of the same sign, possible for \(N\ge3\), with phases \(t,-t\); keep the others zero. The last squared sum varies with \(t\). Nonconstancy on the compact group gives positive Haar variance. The exponential moment of any nonconstant bounded real variable has a complex zero: otherwise the Schwarz and Cauchy estimate in §4.56 on arbitrary large discs forces its log's second derivative at zero to vanish. For this fixed Haar variable one such zero rescales to \(O_N(1/\beta)\) for \(h_b\), and its conditional variance is of order \(\beta^2\). Numerical zero locations for \(N\ge3\) are unnecessary.

For a source on all selected links the conditional moment is the product of the single-link moments, so the zero from this one link persists. The example proves failure of uniform *conditional* bounds even though the averaged innovation is controlled by SINGLE-LINK-INNOVATION-LIMIT. The small mass and correlations of the corresponding exterior records must be retained in the full-law analysis.

### 4.58 Sharp factorial order of absolute conditional jets in the Wilson comb (P)

There is an all-order consequence for any proof that sums the absolute derivatives of the normalized single-link histories. Under the marked-moment tiling of §4.22, for either \(X_b=r_b\) or \(X_b=h_b\),
\[
 \mathbb E|\kappa_m(X_b\mid\mathcal E)|
       \le C^m(m!)^2,\qquad
 \mathbb E|\kappa_m(X_{f_1},\ldots,X_{f_m}\mid\mathcal E)|
       \le C^m(m!)^2\sum_{b\in\mathcal C}\prod_i |f_{i,b}|.
 \tag{ANNEALED-CONDITIONAL-JETS}
\]
Indeed the exponential moment for the finite plaquette stencil bounds \(\mathbb E|X_b|^m\le C^m m!\). In the conditional partition formula for a cumulant, the product of the absolute conditional moments for every partition is at most \(\mathbb E(|X_b|^m\mid\mathcal E)\), by conditional Hölder. The sum of the absolute partition coefficients is at most \(\sum_{k=1}^m k^m/k\le C^m m!\), since \(k!\) times the Stirling number counts onto maps from a labeled \(m\)-set to a labeled \(k\)-set. Conditional independence of the selected links gives the second inequality. All these are finite-order assertions about the actual Wilson marginal.

For \(SU(2)\) the exponent two in this absolute conditional bound is necessary. Take the compact exterior from §4.57 and write \(w=\beta z\). At its exact center the one-link generating function of \(X_b/\beta\) is
\[
 M_0(w)=e^{a_0 w}(e^{\Delta w}-1)/(\Delta w),\qquad \Delta=24v^2,\quad s=2\pi/\Delta .
\]
Here \(a_0\) is the lower endpoint of the interval. Let \(m\) be even and require each of the fixed finitely many unselected links in its determining stencil to lie in a Haar ball of radius \(\delta=(\beta m^2)^{-1}\) around its prescribed value. The full Wilson probability of this exterior event is bounded below by
\[
 e^{-C\beta}(c\delta)^{C_1}.
\]
To verify this under the actual law, condition on the complement of this fixed set of links. Only a fixed number of Wilson plaquettes depend on them and \(0\le s_p\le2N\). The local Boltzmann factor is at least \(e^{-C\beta}\), and its normalized Haar integral is at most one. Haar volumes of the finite product of small balls give the remaining power, uniformly in all exterior links and in the torus side. No macroscopic sector partition function is used.

On this event \(K=O(\delta)\) and the conditional Wilson density of \(u\) differs from Haar by \(O(\beta\delta)\) uniformly. The compact symbol \(X_b/\beta\) differs uniformly from its exact-stripe value by \(O(\delta)\); for the ordinary row its extra Laplacian is zero at the exact exterior and contributes only \(O(\delta/\beta)\). For either row its conditional generating function \(M(w)\) therefore satisfies \(\sup_{|w|\le3s/2}|M-M_0|\le C/m^2\). Rouché's theorem gives exactly two zeros there, \(\zeta_+,\zeta_-\), conjugate to each other and within \(C'/m^2\) of \(is,-is\), respectively. For the displacement, use small circles of radius \(K_0/m^2\) around those two simple zeros and take \(K_0\) larger than the uniform perturbation constant divided by their nonzero derivative. On \(|w|=3s/2\) the unperturbed function has positive minimum modulus.

Factor \((1-w/\zeta_+)(1-w/\zeta_-)\) from \(M\). The remaining analytic factor tends uniformly on \(|w|\le 5s/4\) to the corresponding nonvanishing factor of \(M_0\), by the boundary estimate on \(|w|=3s/2\) and the maximum principle. Its log normalized at zero is bounded uniformly there. Thus the conditional cumulant has the exact dominant-zero estimate
\[
 \frac{\kappa_m(X_b\mid\mathcal E)}{\beta^m}
 =-(m-1)!(\zeta_+^{-m}+\zeta_-^{-m})
           +O\bigl(m!(5s/4)^{-m}\bigr).
\]
For even \(m\) the two leading terms add in absolute value up to a relative \(O(1/m)\), because \(\zeta_\pm=\pm i s+O(1/m^2)\). The remainder is smaller by \(O(m(4/5)^m)\). It follows throughout this event that
\(\left|\kappa_m(X_b\mid\mathcal E)\right|\ge c (m-1)!(\beta/s)^m\) for all sufficiently large even \(m\).

Take \(m=2\lfloor\beta/2\rfloor\) on the weak trajectory. The event probability estimate gives
\[
 \mathbb E|\kappa_m(X_b\mid\mathcal E)|
 \ge e^{-C\beta}(c/(\beta m^2))^{C_1}
             c(m-1)!(\beta/s)^m
 \ge c_2^m(m!)^2
 \tag{CONDITIONAL-GEVREY-LOWER}
\]
after decreasing \(c_2>0\). In the last inequality \(\beta\in[m,m+2)\), \(\beta^m\ge m!\), and a fixed polynomial is absorbed in an exponential. Consequently no \(C^m(m!)^p\) with \(p<2\) bounds these **absolute normalized conditional jets** uniformly in the cutoff. This gives an actual reason to retain Gevrey order or undivided measure expansions at mixed entries. It does not establish such growth for the unconditional logarithm: the latter also contains all connected cumulants among the exterior conditional coefficients, with their signs.

### 4.59 Explicit full-law \(SU(2)\) retained field and covariant Hessian (P)

The matrix integral in SINGLE-LINK-MEAN has a useful positive form for \(SU(2)\). In quaternion coordinates denote the unit staples by \(w_{i,\pm}\), put \(k_i=w_{i,+}+w_{i,-}\), \(k=\sum_i k_i\), \(\gamma=2\beta |k|\), and \(e=k/|k|\) for \(k\ne0\). The conditional spherical density is proportional to \(e^{\gamma u\cdot e}\) on \(S^3\). For each \(\Delta_{ij}=k_i-k_j\) write its parallel and perpendicular components relative to \(e\). With \(v\) the invariant-generator speed of §4.57, the exact scalar is
\[
 m_b=\frac{4v^2\beta}{3}\sum_{i<j}
       \big[(1-a_\gamma)|\Delta_{ij}^{\perp}|^2+
                              3a_\gamma|\Delta_{ij}^{\parallel}|^2\big],
 \qquad
 a_\gamma=\frac{\mathbb E_\gamma(u\cdot e)}{\gamma}.
 \tag{SPHERICAL-RETAINED-MEAN}
\]
At \(\gamma=0\) take \(a_0=1/4\), and the result is independent of \(e\). Indeed the two-force difference is the spherical gradient of \(-2u\cdot\Delta_{ij}\). Its squared length in the chosen frame is \(4v^2(|\Delta_{ij}|^2-(u\cdot\Delta_{ij})^2)\). With \(t=u\cdot e\), the marginal base density is proportional to \((1-t^2)^{1/2}\,dt\). Integration of the derivative of \(e^{\gamma t}(1-t^2)^{3/2}\) gives \(1-\mathbb E_\gamma t^2=3a_\gamma\). Spatial symmetry puts \(a_\gamma\) on each of the three perpendicular diagonal second moments. This proves the formula.

Uniformly \(c/(1+\gamma)\le a_\gamma\le\min(1/4,1/\gamma)\) for \(\gamma>0\). The upper \(1/\gamma\) follows from \(t\le1\); for the other upper bound, \(\mathbb E_\gamma t^2\) is increasing since the law of \(|t|\) has tilt \(\cosh(\gamma |t|)\), whose logarithmic derivative is increasing in \(|t|\). Its value at zero is \(1/4\). For \(\gamma\ge1\), the mean \(\mathbb E_\gamma t\) is increasing with derivative \(\operatorname{Var}_\gamma(t)>0\), so it is at least its positive value at one. Continuity at zero and positivity on the remaining compact interval give the lower bound.

The differences in this formula have an exact linear covariant expression, with no small-field approximation. Let \(u(x)\) denote the temporal link field between the two consecutive spatial slices. Write
\[
 (T_i u)(x)=U_{x,i}(t)u(x+e_i)U_{x,i}(t+1)^\dagger,\qquad
 L_i=T_i+T_i^*-2I .
\]
The shifts are orthogonal in quaternion coordinates with the spatial sum inner product. The two staples in direction \(i\) are \(T_i u,T_i^*u\), and hence
\(\Delta_{ij}=(L_i-L_j)u(x)\). The central \(u(x)\) cancels, consistent with its absence from the exterior. Define the nonnegative exterior observable
\[
 P_b=\frac{4v^2\beta}{3}\sum_{i<j}|(L_i-L_j)u(x)|^2,\qquad
 e_b=\sum_{p\ni b}s_p .
\]
On **every** full real configuration,
\[
 0\le P_b-m_b\le C(e_b+\beta e_b^2),\qquad
 \|P_b-m_b\|_{L^p(\mu_\beta)}\le C_p/\beta .
 \tag{SPATIAL-HESSIAN-REMAINDER}
\]
For the deterministic bound, the incident Wilson energies equal the squared quaternion distances \(|u-w_{i,\pm}|^2\). The point \(e\) minimizes the sum of these six squared distances on the unit sphere, choosing any minimizer when \(k=0\), so \(\sum_\alpha|w_\alpha-e|^2\le e_b\). In particular \(\sum|\Delta_{ij}|^2\le C e_b\). Since \(e\cdot w_\alpha=1-|w_\alpha-e|^2/2\), also \(|e\cdot\Delta_{ij}|\le C e_b\). If \(|k|\ge1\), the term \(\beta a_\gamma\sum|\Delta_{ij}^{\perp}|^2\) is bounded by \(C e_b\). If \(|k|<1\), the minimum squared-distance sum \(12-2|k|\) implies \(e_b\ge10\), so the same term is bounded by \(C\beta e_b^2\). The longitudinal correction is bounded by \(C\beta e_b^2\) in either case. Both signs follow from \(a_\gamma\le1/4\). The \(L^p\) estimate uses the full Wilson marked exponential bound on this fixed stencil and the deterministic inequality; it is uniform under the tiling and trajectory hypotheses of §4.22.

Thus the residual susceptibility in SINGLE-LINK-TOWER involves the explicit squared differences of the three spatial covariant second differences and a positive subtraction with a quantitative extra inverse-coupling factor in each local \(L^p\) norm. For a sum over the torus the covariance among these local terms is still needed. A pointwise \(O(\beta^{-1})\) moment bound is insufficient to sum all separated pairs.

### 4.60 An exact Wilson-loop part and compact quartic remainder for every \(SU(N)\) (P)

There is an all-field identity before any conditional integration. Regard complex \(N\times N\) matrices as a real Hilbert space with \(\langle A,B\rangle=\operatorname{Re}\operatorname{Tr}(A^\dagger B)\). The generators satisfy \(\langle T_A,T_B\rangle=\tau\delta_{AB}\). For any oriented bond \(b\) let \(u=U_b\), let \(w_{i,+},w_{i,-}\) be its two oriented staples in each transverse plane, and put \(K_i=w_{i,+}+w_{i,-}\), \(\Delta_{ij}=K_i-K_j\). Both \(u\) and all staples run between the same endpoints. The tangent space to the embedded gauge group at \(u\) is the span of the orthogonal vectors \(T_Au\). Since \(X_A(S_i-S_j)=-\langle T_Au,\Delta_{ij}\rangle\),
\[
 h_b=P_b-N_b,\qquad
 P_b=\frac{\tau\beta}{3}\sum_{i<j}\|\Delta_{ij}\|_{\rm HS}^2,\qquad
 N_b=\frac{\tau\beta}{3}\sum_{i<j}
       \|\Pi_{(T_uSU(N))^\perp}\Delta_{ij}\|_{\rm HS}^2 .
 \tag{EXACT-WILSON-LOOP-SPLIT}
\]
Both terms are gauge invariant and nonnegative. The first is independent of \(u\). Each \(\Delta_{ij}\) is a sum of four staples with coefficients \(c_\alpha=+1,+1,-1,-1\). Since the coefficients sum to zero,
\[
 \|\Delta_{ij}\|^2
  =-\sum_{\alpha<\gamma}c_\alpha c_\gamma\|w_\alpha-w_\gamma\|^2,\qquad
 \|w_\alpha-w_\gamma\|^2
  =2[N-\operatorname{Re}\operatorname{Tr}(w_\alpha w_\gamma^\dagger)] .
\]
Thus \(P_b\) is an explicit signed linear combination of single-trace closed Wilson paths of length at most six. For a temporal bond \(\Delta_{ij}=(L_i-L_j)u(x)\) under the same left and right spatial transports as §4.59, now acting unitarily on matrices. Its cancellation of the common spin is exact for general spatial backgrounds.

The second term has a compact algebraic representation of degree at least four in the six incident plaquette defects. To see this set \(A_\alpha=(w_\alpha-u)u^\dagger\). The matrix \(I+A_\alpha=w_\alpha u^\dagger\) is a plaquette holonomy or its reversal based at the proper endpoint. Unitarity gives \(\operatorname{Herm}A_\alpha=-A_\alpha A_\alpha^\dagger/2\). The determinant gives \(\operatorname{Tr}A_\alpha=-\sum_{j=2}^N e_j(A_\alpha)\), with \(e_j\) the elementary characteristic coefficients of degree \(j\). The real normal projection at identity retains the Hermitian part and the scalar anti-Hermitian trace. Its norm is therefore bounded by \(C_N\|A_\alpha\|^2\) on the compact group and is a finite polynomial in \(A_\alpha,A_\alpha^\dagger\) starting in degree two. Multiplication by \(u^\dagger\) carries the tangent and normal projections at \(u\) to the corresponding projections at identity. Since \(\Delta_{ij}u^\dagger=\sum_\alpha c_\alpha A_\alpha\), squaring this normal projection proves the claimed quartic start. Moreover, for every real lattice field,
\[
 0\le N_b\le C_N\beta\left(\sum_{p\ni b}s_p\right)^2
                \le C_N'\beta\sum_{p\ni b}s_p^2.
 \tag{COMPACT-QUARTIC-H-ROW}
\]
This bound and its sign hold even when every local analytic chart fails.

Taking the actual conditional expectation over \(u\) at a selected bond gives \(m_b=P_b-\mathbb E[N_b\mid\mathcal E]\). The full marked-moment estimate and conditional Jensen give \(\|P_b-m_b\|_p+\|P_b-h_b\|_p\le C_p/\beta\) for each fixed \(p\), now for every \(SU(N)\). The SU(2) integral in §4.59 additionally gives a pointwise comparison with the *actual* incident energy of each configuration. For all groups the source problem has thereby been reduced algebraically to a finite Wilson-loop combination and an explicit strictly higher-degree compact correction. A variance estimate for the latter's full sum still requires connected spatial control; the positive local bound alone cannot supply it.

### 4.61 A second full-Wilson heatbath innovation of the retained comb mean (P)

On \(4\mid n\) take the selected spatial parity class to be \((0,0,0)\bmod2\) and let \(\mathcal D\) consist of temporal links at spatial sites \((1,0,0)\bmod4\) at every time. Each \(d\in\mathcal D\) neighbors precisely two selected \(\mathcal C\)-links, \(b_-,b_+\), at spatial displacement \(\pm e_1\). Different \(d\)'s have no nearest-neighbor edge and no common \(\mathcal C\)-neighbor. No elementary temporal plaquette couples different time layers of temporal links. Thus given \(\mathcal E'=\sigma(U_{(\mathcal C\cup\mathcal D)^c})\), the missing-link conditional law factors into independent three-link stars \((d,b_-,b_+)\) and isolated \(\mathcal C\)-links. The latter have no \(\mathcal D\) dependence. This second step concerns the exact original compact law on all sectors; it uses a coordinate disintegration distinct from the multiscale constraints of §§4.26–4.31.

For the unit comb define \(M=\sum_{b\in\mathcal C}m_b(\mathcal E)\). In its second conditional variance,
\[
 J_2=\mathbb E\,\operatorname{Var}(M\mid\mathcal E')
 =\sum_{d\in\mathcal D}\mathbb E
      \operatorname{Var}\bigl(m_{b_-}+m_{b_+}\mid\mathcal E'\bigr).
\]
In each star the density of the central link is the product of its direct exterior Wilson factors and the two positive single-link integrals of its neighboring selected spins. For any fixed \(\beta\) these are literal integrals against normalized Haar over the compact group. By Jensen and the single-site fourth or second moment bounds, each summand is at most \(C\) uniformly on average. For every \(SU(N)\) there is also a quantitative lower bound
\[
 \liminf_{\beta\to\infty}\frac{J_2}{|\mathcal D|}
             \ge \frac{32}{289}\,\tau^2\,d_G.
 \tag{SECOND-COMB-INNOVATION}
\]
It does not assert that the conditioned mean is constant across \(\mathcal E'\).

Here is a local uniform chart proof. In a fixed rectangle containing such a star and the plaquettes incident to its three variables, choose spatial coordinate trees separately on both time slices and join them with one exterior temporal link. All gauge choices depend on fixed exterior links only. The determinant-one site gauges put these tree links at identity. Loops for fixed non-tree links can be filled with a bounded number of plaquettes in a slightly larger fixed rectangle. For the chosen \(\mathcal D\) grid the temporal tree connector can always be taken outside both missing classes. The same is true when another isolated missing link lies in the larger rectangle: the spatial trees and their connector never use it. Only the exterior links in the three-star action need to be controlled. If all plaquettes of the enlarged rectangle have distance at most \(D/\sqrt\beta\) from identity, all those fixed star-stencil links are within \(C D/\sqrt\beta\) of identity in the chosen gauge. This yields an \(\mathcal E'\)-measurable good set of at least that probability. FIRST and the bounded number of plaquettes imply its probability is at least \(1-C/D^2\), uniformly in the star and the torus. The possible small finite sides with colliding rectangles are irrelevant to the mesh limit.

For fixed \(D\), scale the three time-link logarithms to \(X_d,X_-,X_+\) by \(\sqrt\beta\). Their joint conditional integral tends to a finite Gaussian with precision
\[
 \tau\begin{pmatrix}6&-1&-1\\-1&6&0\\-1&0&6\end{pmatrix}\otimes I_{d_G}.
\]
In fact every incident temporal plaquette yields \((\tau/2)|X_x-X_{x+e}+b_{x,e}|^2\), with a bounded fixed translation from its exterior links. Six neighbors occur for each vertex, and only the two displayed edges join two missing variables. All other neighbor spin values are bounded exterior coordinates. In the common tree gauge the transport frames tend to identity. Schur complement therefore gives central covariance \((3/(17\tau))I\); its mean depends on the exterior.

The Laplace comparison is uniform over bounded exterior coordinates. For dominated convergence, each missing link has at least four incident exterior temporal neighbors. The corresponding fixed-staple Wilson factors give a joint bound \(C_D e^{-c\beta\sum_x d(U_x,I)^2}\) up to the constant reference action, using the squared-distance lower bound and the small fixed links. The normalization is at least \(c_D\beta^{-3d_G/2}\) by restricting each variable to a radius-\(\beta^{-1/2}\) Haar ball. Conditional integrals over the two leaves at fixed \(X_d\) have exactly the one-link comparison in §4.57, uniform for bounded \(X_d\). To control the tails of their conditional means when comparing second moments, conditional Jensen bounds \(\mathbb E(|m_{b_\pm}|^4\mid\mathcal E')\) by the fourth moments of the original \(h_{b_\pm}\) in the same three-link integral. Those are bounded by \(C_D\) via the Gaussian tail just established and the polynomial force bound in the scaled variables. This proves \(L^2\) comparison by truncating \(X_d\) and then taking the cutoff to infinity.

In the leading formula of §4.57 for a leaf \(b_\pm\), precisely one of the six staple logarithms contains \(X_d\) with coefficient one. Hence its corresponding pair-mean \(Z_1\) is \(X_d/2\) plus a fixed exterior vector. The other \(Z_i\) are fixed. In \(4\tau^2[\sum_i|Z_i|^2-|\sum_i Z_i|^2/3]\), the coefficient of \(|X_d|^2\) is \(2\tau^2/3\). The two leaves therefore supply \(4\tau^2|X_d|^2/3\) plus a linear function and a constant. For a Gaussian central spin of covariance \(3I/(17\tau)\), its centered linear part is orthogonal to the centered quadratic in the spin about its mean. The variance is at least \(2d_G(4\tau^2/3)^2(3/(17\tau))^2=32d_G\tau^2/289\), for every choice of the bounded exterior translations. Uniform comparison gives this lower bound up to \(o_D(1)\) on the good set. Keep the nonnegative contribution of its complement and send \(D\) to infinity after taking the weak limit.

The exact full variance consequently contains the first single-link innovation of §4.57, this nonzero second innovation, and the variance of \(\mathbb E(M\mid\mathcal E')\). The new retained field is explicit: it sums the original isolated-leaf \(m_b\)'s and the normalized three-link expectations of \(m_{b_-}+m_{b_+}\). Each summand is local in the remaining exterior, with the original Haar and Wilson factors. This calculation quantifies the between-link covariance that would be lost by discarding the first conditional means.

### 4.62 Growing spatial intervals on the full compact Wilson law (P)

The next positive innovation can be bounded through an increasing number of actual temporal links, including all compact exterior fields. Fix the temporal orientation of the eight-site mark and take spatial lines in direction one with coordinates two and three even. At each time integrate the temporal spins on these lines in intervals separated by single retained odd-coordinate sites. Thus all selected comb links (even first coordinate) are inside intervals, and the sigma-field \(\mathcal E_{\rm line}\) of the remaining links is contained in the first heatbath exterior \(\mathcal E\). Different lines have no nearest-neighbor interaction, and different intervals on the same line are separated by a retained spin. Conditional on \(\mathcal E_{\rm line}\) the exact positive Wilson law factors over these intervals. Take their lengths at most \(m\), with the usual periodic endpoint convention. Odd-coordinate separators of comparable spacing exist on large even lines; one shorter final interval is harmless.

For sufficiently weak \(\beta\), and uniformly for \(m\le c_0\beta/\log\beta\), there is an extensive estimate
\[
 \mathbb E\,\operatorname{Var}(r_f\mid\mathcal E_{\rm line})
       \le C\sum_{b\in\mathcal C}f_b^2 .
 \tag{GROWING-LINE-INNOVATION}
\]
It holds on the full reference law under the marked-exponential and FIRST trajectory hypotheses already used in §4.22. It includes both the first single-link innovation and the subsequent innovation of its retained means. The length here increases with the inverse bare coupling. It is shorter than a fixed physical interval on the continuum trajectory.

For clarity fix one interval \(I\), with \(m_I\le m\) spins \(u_x\). Its conditional action is a sum of six incident Wilson terms at each vertex, counting internal edges only once. Four directions lead to lateral exterior staples. Internal neighboring temporal spins couple via the orthogonal left/right transport \(R_x u_{x+1}=U_{x,1}(t)u_{x+1}U_{x,1}(t+1)^\dagger\); an endpoint has an analogous fixed separator term. For each \(x\) choose one lateral exterior staple \(v_x\in SU(N)\) as reference. It is measurable in \(\mathcal E_{\rm line}\). Put \(\delta_\beta^2=A\log\beta/\beta\) with \(A\) a fixed sufficiently large number. Call the interval exterior good if each of its other lateral staples is within \(C\delta_\beta\) of \(v_x\), its neighbor references obey \(d(v_x,R_xv_{x+1})\le C\delta_\beta\), and its endpoint references match the fixed separator transports to this precision. Distances use a fixed bi-invariant metric.

This exterior fails with probability at most \(C m_I\beta^{-B}\), where \(B\) can be chosen bigger than six by increasing \(A\). Indeed in the actual joint Wilson field, if all incident plaquettes of this interval are within \(\delta_\beta\) of identity, every reference and lateral staple is within \(\delta_\beta\) of the actual \(u_x\); the actual neighboring spins also match up to \(\delta_\beta\). The triangle inequality gives the stated good exterior conditions. Only \(C m_I\) plaquettes occur, and the one-plaquette exponential moment bounds their individual probabilities of failure by \(C\exp[-c\beta\delta_\beta^2]\). Goodness itself uses only exterior variables. No product independence of the plaquette indicators is required.

On a good exterior put \(u_x=v_x e^{A_x}\) and take the inner product chart \(\mathcal D_\epsilon=\{\max_x |A_x|\le\epsilon\}\), for a sufficiently small fixed physical \(\epsilon\). In this chart the exact conditioned action including Haar has log-density Hessian of negative logarithm at least \(c\beta I\), uniformly in \(m_I\). To verify the matrix bound, at matching references and zero \(A\) the four lateral terms at each site contribute \(4\tau I\). Every internal edge adds a nonnegative quadratic form \(\tau|A_x-O_x A_{x+1}|^2\), where \(O_x\) is the adjoint rotation of its spatial endpoint frame; separator terms are also nonnegative. For a general good exterior, each product is an analytic fixed group word in its two endpoint logs, its fixed adjoint rotation, and the reference plaquette within \(C\delta_\beta\) of identity. Its Hessian differs from this value by \(O(\epsilon+\delta_\beta)\), uniformly over rotations by compactness. Only two endpoints and a bounded number of edges occur per row, so the entire Hessian perturbation has operator norm at most \(C(\epsilon+\delta_\beta)\). The Haar logarithmic Jacobian adds a uniformly bounded diagonal Hessian. The stated convexity follows for small \(\epsilon\) and all sufficiently large \(\beta\). Hence the normalized positive conditional law restricted to the product of Lie-algebra balls has Poincaré constant \(C/\beta\), by the convex-domain argument in §4.43.

The full compact law differs from this chart by an explicitly small probability for every good exterior. Indeed if any \(u_x\) leaves the chart, its Wilson term against the chosen lateral reference is at least \(c_\epsilon>0\), while all other action terms are nonnegative. The unnormalized outer mass is at most \(e^{-c_\epsilon\beta}\). Restricting all \(u_x\) to distance \(c/\sqrt\beta\) of their references instead gives a lower bound
\[
 Z_I(\mathcal E_{\rm line})
 \ge \exp[-C m_I(\beta\delta_\beta^2+1+\log\beta)]
\]
for the conditional normalizer with exterior-only terms removed. Each of its action terms is then at most \(C(\delta_\beta^2+1/\beta)\), and each of the \(m_I\) Haar balls has mass at least \(c\beta^{-d_G/2}\). Choose \(c_0\) using \(A,\epsilon\) and these fixed constants. For \(m_I\le c_0\beta/\log\beta\) the conditional outer probability is at most \(e^{-c'_\epsilon\beta}\).

Let \(F_I=\sum_{b\in I\cap\mathcal C} f_b r_b\), \(M_I=\sum_{b\in I\cap\mathcal C}f_b^2\). On the inner chart its ordinary Euclidean gradient obeys
\[
 |\nabla F_I|^2\le C\sum_{b\in I\cap\mathcal C}
           f_b^2\left[1+\beta^2\sum_{p\ni b}s_p\right].
\]
Indeed a marked force has size bounded by \(C\sum_{p\ni b}\sqrt{s_p}\), its derivative in any neighboring link is bounded by a constant, and the Casimir term and its derivative are bounded. Only a fixed number of positions occurs at every gradient slot, and logarithmic differentials are bounded on the chart. On good exteriors multiply the inner-law Poincaré estimate by its true conditional probability, then integrate over the original exterior law. The gradient bound and FIRST make this contribution at most \(C M_I\), with no division by a rare sector probability.

To include all the other terms, compare \(F_I\) to its normalized inner mean on good exteriors, and to zero on bad ones. The conditional variance is bounded above by the corresponding conditional mean squared difference. Everywhere \(|F_I|\le C(\beta+1)\sqrt{m_I M_I}\) by compactness. The good-exterior outer error and the bad-exterior error are bounded by
\[
 C(\beta+1)^2m_I M_I
             [e^{-c'_\epsilon\beta}+C m_I\beta^{-B}]
 \le C M_I .
\]
Thus the complete interval innovation is bounded by \(C M_I\) on average. Sum the independent conditional intervals to get GROWING-LINE-INNOVATION. In particular the same upper bound holds for
\(\mathbb E\operatorname{Var}(\sum_{b\in\mathcal C} f_bm_b\mid\mathcal E_{\rm line})\) by the exact positive variance tower. Covariance of the newly retained interval means across \(\mathcal E_{\rm line}\) is still required for full SUS.

### 4.63 Exponentially long \(SU(2)\) temporal-spin intervals on the actual Wilson law (P)

For \(SU(2)\) the length restriction in GROWING-LINE-INNOVATION can be enlarged to \(m\le e^{c_1\beta}\) for a fixed \(c_1>0\), retaining the full compact Wilson measure. The reason is the exact one-site spherical field rather than a global lower bound on the normalizer. Identify \(SU(2)\) with unit quaternions \(S^3\) with their round metric. Keep the four fixed lateral staples per interval site and the same first-direction transport rotations as in §4.62. Say the exterior of an interval is good if all four lateral staples at \(x\) lie within a small fixed angular distance \(\delta\) of its chosen reference \(v_x\), and \(\angle(v_x,R_xv_{x+1})\le\delta\) along its internal edges. One can include compatibility with the end separators, though it is unnecessary below. As in §4.62, a union over \(C m_I\) true incident Wilson plaquettes gives a bad-exterior probability at most \(C m_I e^{-b\beta}\), \(b>0\), by the one-plaquette exponential moment. The fixed angular threshold is decreased by the bounded triangle-inequality factor before applying the plaquette tail.

Fix \(\theta=7\pi/30\) (42 degrees) and restrict spin \(u_x\) to the spherical cap of radius \(\theta\) about \(v_x\). Even with both interacting neighbors arbitrary, their sum has length at most two. The sum of the four lateral staples differs from \(4v_x\) by at most \(C\delta\). Thus the exact local field \(K_x\) obeys \(|K_x|\ge2-C\delta\) and
\[
 \angle(K_x,v_x)\le
   \arcsin((2+C\delta)/4)<\theta-\theta_0
\]
for some fixed \(\theta_0>0\) when \(\delta\) is small enough. This geometric bound uses the ball of radius \(2+C\delta\) centered at \(4v_x\); the angle of a tangent ray from the origin is the indicated arcsine. The conditional one-site weight is \(e^{2\beta K_x\cdot u_x}\). The probability of \(\angle(u_x,v_x)>\theta\), uniformly in all its fixed neighbors, is at most \(C e^{-b'\beta}\). Indeed there the angle to \(K_x\) exceeds \(\theta_0\), whereas a fixed smaller cap about \(K_x/|K_x|\) has positive Haar measure and strictly higher dot product. This argument includes endpoints with a fixed separator. Averaging over neighbors and taking the union bound shows that the conditional probability of leaving the product of caps is at most \(C m_I e^{-b'\beta}\). No factor growing exponentially with the number of spins divides this tail bound.

The exact negative log-density on the product caps has uniformly positive Riemannian Hessian. Write \(h_x\) for the lateral four-staple sum. For tangent velocities \(X_x\perp u_x\), the Hessian divided by \(2\beta\) has lateral term \(\sum_x(h_x\cdot u_x)|X_x|^2\). A neighboring pair \(x,y\) contributes
\[
 (u_x\cdot R_x u_y)(|X_x|^2+|X_y|^2)-2X_x\cdot R_xX_y.
\]
These formulas follow by differentiating \(e^{2\beta h_x\cdot u_x}\) and \(e^{2\beta u_x\cdot R_xu_y}\) along the spherical geodesics, whose second derivatives at zero are \(-|X_x|^2 u_x\). In each cap the lateral mass is at least \(4\cos(\theta+\delta)\). The pair dot product is at least \(\cos(2\theta+\delta)\). Using \(2|X_x||X_y|\le |X_x|^2+|X_y|^2\), each internal edge can thus lose at most \(1-\cos(2\theta+\delta)\) at either endpoint. A fixed separator contributes only its own dot product at the endpoint, bounded below by \(-1\). There are at most two such contributions in total per site, so the Hessian is bounded below by \(2\beta\) times
\[
 4\cos(\theta+\delta)-
           2\max(1,1-\cos(2\theta+\delta))>0
\]
for small fixed \(\delta\). The product sphere has nonnegative Ricci curvature, and each cap boundary is geodesically convex since \(\theta<\pi/2\). The weighted Neumann Poincaré constant is consequently at most \(C/\beta\) uniformly in the interval length. One can obtain the same bound by the integrated Bochner identity used in §4.43, with the additional nonnegative Ricci and outward convex-boundary terms. The product boundary has coordinate faces. Integration by parts on each smooth face gives these same terms for smooth Neumann test functions; equivalently approximate the caps by increasing smooth convex penalties on their geodesic neighborhood and pass by the quadratic-form approximation. The Haar measure here is exactly the product spherical volume; no coordinate Jacobian is omitted.

The spherical gradient of the marked \(r\)-sum satisfies the bound from §4.62 with a fixed change of metric constant. On good exteriors multiply the inner Poincaré estimate by its true conditional cap probability and integrate with FIRST. This gives \(C M_I\). Comparison with zero on bad exteriors and with the inner mean on good ones now costs at most \(C\beta^2 m_I^2 e^{-b''\beta}M_I\), by compactness and the two tail bounds. Choose \(0<c_1<b''/3\), decreasing it to absorb the polynomial in \(\beta\). For compatible intervals this proves
\[
 \mathbb E\operatorname{Var}(r_f\mid\mathcal E_{\rm line})
  \le C M_f,\qquad m\le \min(n-1,e^{c_1\beta}),\quad SU(2).
 \tag{EXPONENTIAL-LINE-INNOVATION}
\]
On a logarithmic weak trajectory this reaches a positive power of the inverse lattice spacing. The value of \(c_1\) is limited by the fixed plaquette and cap tail constants. The bound does not claim that the interval length has already reached every physical scale. Even if an entire spatial line is integrated, the transverse temporal links, the spatial slices and their retained mean covariance still enter the complete Wilson susceptibility.

### 4.64 Full periodic lines in the \(SU(2)\) Wilson measure (P on the marked-moment tori)

For \(SU(2)\) one can integrate the **entire** spatial lines from §4.62, on reference tori of arbitrary side satisfying MARKED-EXP. Let \(\mathcal L\) comprise all temporal spins at all times with spatial coordinates two and three even; their first spatial coordinate is unrestricted. Let \(\mathcal E_\perp\) fix all spatial links and all temporal links outside \(\mathcal L\). Conditioned on \(\mathcal E_\perp\), the exact Wilson law on \(\mathcal L\) is a product of periodic nearest-neighbor spin chains, one for each such spatial line and time level. On a line the density is proportional to
\[
 \exp\left(2\beta\sum_x[h_x\cdot u_x+u_x\cdot R_x u_{x+1}]\right)
\]
relative to the Haar spheres, with the four lateral quaternion staples in \(h_x\) and the actual orthogonal transport \(R_x\). We prove the absolute conditional covariance sum and its consequence
\[
 \sup_{x\in\mathcal C}\ \sum_{y\in\mathcal C}
    \mathbb E\left|\,\operatorname{Cov}(r_x,r_y\mid\mathcal E_\perp)\,\right|\le C,
 \qquad
 \mathbb E\operatorname{Var}(r_f\mid\mathcal E_\perp)\le C M_f .
 \tag{FULL-LINE-INNOVATION}
\]
All exterior averaging here uses the full original law. Cross-line covariances vanish conditionally. The transverse and spatial retained means still enter full SUS.

**Correlation estimate inside a good bridge.** Call an interval of spins good when its four lateral staples are aligned to \(\delta\) and its consecutive references are compatible, as in §4.63. Goodness depends only on \(\mathcal E_\perp\), and need not involve endpoint spins. Fix any two exterior endpoint spins. In the product caps the exact fiber has, for observables \(F,G\), the weighted estimate
\[
 |\operatorname{Cov}_{D}(F,G)|
 \le (C/\beta)\sum_{i,j}e^{-c|i-j|}
              \|\nabla_i F\|_{L^2(D)}\|\nabla_j G\|_{L^2(D)} .
 \tag{CAP-WEIGHTED-COVARIANCE}
\]
Here \(D\) indicates the normalized cap law, and the distance is on the interval. For a direct justification, differentiate the scalar weighted Neumann Poisson equation. On one-forms the resulting operator is the product weighted rough Laplacian plus \(\mathrm{Ric}+\operatorname{Hess}V\), with the absolute boundary condition. Its quadratic form includes the convex face second fundamental form, and its spectral lower bound is \(c_0\beta\) by §4.63. The covariance is \(\langle dF,\mathscr L_1^{-1}dG\rangle\), from integration by parts as in T1 Lemma 7.52. The diagonal weight on the \(i\)-th tangent component \(e^{c|i-j|}\) commutes with the product connection, the coordinate Ricci operators and the face conditions. Indeed the normal to each cap face belongs to that site's sphere only, and its shape operator is supported in that same tangent component. The sole off-diagonal blocks are the nearest-neighbor Hessian blocks of norm at most \(C\beta\). Conjugation changes the operator by at most \(C\beta(e^c-1)\). Choose \(c\) so this is below \(c_0\beta/2\), invert the conjugate by a Neumann series, and evaluate its \((i,j)\) block. This yields the bound. The product-face identities follow by integrating in the coordinate factors with the stated Neumann conditions; edge intersections have zero boundary surface measure. Smooth functions and the corresponding form-domain approximation justify the same estimate for our local functions. This is a spatial estimate for a conditioned positive law, not a spectral gap assumption for the four-dimensional theory.

On a good interval of length \(s\), the conditional cap-failure probability is at most \(C s e^{-b\beta}\), uniformly in the two endpoints (§4.63). For bounded \(F,G\) the change in covariance from the normalized cap law to the full conditional interval law has modulus at most \(C s e^{-b\beta}\|F\|_\infty\|G\|_\infty\), by elementary expansion of the two means and the two-product moment.

**Small log cross-ratio.** Take \(s=\lceil C_2\beta\rceil\) for a fixed \(C_2>0\), increasing the weak threshold if necessary. Let \(K_I(l,r)>0\) be the integral over \(s\) spins in a good interval with endpoint spins \(l,r\). The mixed derivative of \(\log K_I\) in unit tangent directions at the two endpoints is the exact covariance of their two scores. Each score is a nearest-end spin function with sup norm and spherical gradient at most \(C\beta\). There is no direct mixed boundary term when the interval contains at least two spins. The preceding two bounds therefore make this mixed derivative at most
\[
 C\beta e^{-c(s-1)}+C\beta^2s e^{-b\beta}\le C e^{-b_1\beta}.
\]
Integrate along two endpoint geodesics, whose lengths are at most \(\pi\). The log cross-ratio obeys
\[
 \sup_{l,l',r,r'}
 |\log K_I(l,r)+\log K_I(l',r')-\log K_I(l,r')-\log K_I(l',r)|
       \le C e^{-b_1\beta}.
 \tag{GOOD-BRIDGE-RATIO}
\]
Multiplication of \(K_I\) by one-end weights makes no difference. More importantly, for *any* positive future weight \(H(r)\), compare the transition probabilities proportional to \(K_I(l,r)H(r)\) for two different \(l\)'s. By (GOOD-BRIDGE-RATIO) their normalized density ratio lies between \(e^{-\Delta}\) and \(e^\Delta\), \(\Delta=C e^{-b_1\beta}\). Their total variation distance (supremum over events) is at most \(e^\Delta-1\le e^{-b_2\beta}\) on the weak trajectory after lowering \(b_2\). The estimate is therefore available in a chain conditioned on any data further to the right, and also in the reverse orientation. A bad bridge always has the trivial contraction coefficient one.

**Products of bridges and the actual exterior law.** For a succession of disjoint good or bad bridges on an arc, the total variation influence of one endpoint on observables at the other is bounded by the product of their contraction coefficients. Indeed condition on each successive cut spin. The transition kernels are the bridge kernels multiplied by the remaining positive future integrals and normalized. Total variation between two incoming laws contracts by at most the supremum total variation between two rows of the kernel, by integrating their difference or coupling. Ordinary intervening links have coefficient at most one. Repeated application proves the product assertion.

Choose bridges with at least \(s\) unused sites between them. If a specified bridge is bad, at least one of \(Cs\) Wilson plaquettes in its bounded-width cylinder must have energy \(\ge \epsilon_\delta>0\) in the actual joint field, by the triangle argument of §4.62. Cylinders of the designated bridges are disjoint for sufficiently large \(s\). For any \(h\) of them, sum over one witnessing plaquette in each. MARKED-EXP and Markov's inequality imply
\[
 \mathbb P_{\rm Wilson}(\text{these }h\text{ bridges are bad})
 \le (Cs e^{-b_3\beta})^h.
\]
This uses the expectation of the joint event, not a product approximation for the exterior spins. With \(\rho_I=e^{-b_2\beta}\) on good bridges and \(1\) on bad ones, expansion of \(\prod_I(e^{-b_2\beta}+1_{\{I\ {\rm bad}\}})\) now gives, for \(h_0\) designated bridges,
\[
 \mathbb E\prod_I\rho_I
 \le(e^{-b_2\beta}+Cs e^{-b_3\beta})^{h_0}
 \le e^{-b_4\beta h_0}.
 \tag{ANNEALED-BRIDGE-PRODUCT}
\]

**Long distances on the periodic line.** The ordinary \(r_x\) depends only on the fixed spatial data and temporal spins at the site and its nearest neighbors on the line; its lateral temporal neighbors are already exterior. Its norm is at most \(C\beta\) for \(\beta\ge1\). Condition further on all spins in the support of \(r_x\). The remaining chain on the circle between its two bordering sites is an open chain with the corresponding two endpoints fixed. Varying one endpoint, while keeping the other fixed, changes the expectation of \(r_y\) by at most \(2\|r_y\|_\infty\prod_I\rho_I\), using bridges on the arc to the edge of its support. The transition argument holds equally for the whole neighboring triple needed to evaluate \(r_y\). Varying the two endpoints separately gives a sum over the two arcs. The covariance with \(r_x\) is bounded by its norm times this oscillation (up to a fixed numerical factor). If the shorter circular distance \(d(x,y)\ge16s\), each arc contains at least \(c d(x,y)/s\) designated bridges, away from both supports. Equation (ANNEALED-BRIDGE-PRODUCT) therefore gives
\[
 \mathbb E|\operatorname{Cov}(r_x,r_y\mid\mathcal E_\perp)|
       \le C\beta^2 e^{-c'd(x,y)} .
\]
Because \(d(x,y)\ge16s\) and \(s\) is proportional to \(\beta\), these tails have uniformly bounded sum.

**Short distances without the loss \(\beta^2s\).** For \(d(x,y)<16s\), take an interval containing the two supports with buffers of at least \(s\) on both ends and total size at most \(20s+O(1)\). When the whole periodic line is shorter than this, use that line itself with no end terms. Its cap Hessian, weighted covariance in circular distance and union bound have the same proofs, without any boundary-influence term. In the open case, conditioning on the two endpoint spins gives their interior covariance plus the covariance of the two interior means under the endpoint law.

Goodness in this larger interval still fails with probability at most \(Cs e^{-b\beta}\) in the full exterior average. On it the cap-failure probability has the same bound uniformly over endpoints. On good exteriors apply CAP-WEIGHTED-COVARIANCE with \(F=r_x,G=r_y\). Their gradients live within one site of their respective roots and satisfy \(\sum_i|\nabla_i r_x|^2\le C(1+\beta^2 e_x)\). The cap probability exceeds \(1/2\) there, so integrating its normalized gradient moments over the original exterior and endpoint law costs at most twice their full Wilson moments. Cauchy–Schwarz and FIRST give a product bound \(C\beta\), canceling the \(1/\beta\) covariance factor. The contribution is at most \(Ce^{-c d(x,y)}\) after a fixed stencil enlargement. Replacing the cap covariance by the full interior one, or encountering a bad exterior, costs at most \(C\beta^2s e^{-b'\beta}\) using the bounded sup norms.

For the two retained endpoint means, differentiating the mean of \(r_x\) in either boundary spin gives its covariance with the corresponding endpoint score. The root is at least \(s\) sites away. CAP-WEIGHTED-COVARIANCE with the uniform gradient bound \(C\beta\), plus the compact cap-failure estimate, bounds this derivative by \(C\beta e^{-cs}+C\beta^2s e^{-b\beta}\). The same holds for \(r_y\). Thus on good exteriors the endpoint means have oscillation \(Ce^{-b_5\beta}\); their covariance is uniformly small. On bad exteriors use the compact norm and the same rare-exterior cost. Summing the short-distance bound over at most \(Cs\) sites is uniform. This proves the absolute covariance row in FULL-LINE-INNOVATION for all sufficiently weak \(\beta\), and the variance statement follows by the symmetric Schur bound.

For \(\beta\) in any fixed interval from one to the weak threshold, one elementary edge kernel between temporal spins has a positive finite ratio of its largest and smallest entries, uniformly over all transports and lateral fields after putting the latter in one-end factors. Consequently even after multiplication by arbitrary future weights its transition coefficient is at most \(1-c\) with \(c>0\) depending only on that bounded coupling interval. Repeating the two-arc argument gives exponential conditional decay at long distances; the bounded number of overlapping spin supports is covered by the uniform compact norms. Thus this bounded-coupling range also causes no length restriction.

The positive tower identity gives the same upper bound for the entire innovation of the first heatbath means when all remaining first-direction temporal spins of these lines are integrated. The next retained field is \(\mathbb E(r_f\mid\mathcal E_\perp)\). Its covariance across different transverse lines and spatial slices is not bounded by this theorem. No four-dimensional mass gap or unconditional correlation decay was used.

### 4.65 Exponentially large two-dimensional \(SU(2)\) spin regions (P)

A positive innovation estimate also holds for two-dimensional rectangles on the true compact law. On each plane of even third spatial coordinate at fixed time, partition the temporal spins into rectangles with single retained separator rows and columns at odd coordinates. All selected points of the comb lie in their interiors, with an appropriate periodic partition. Fix all spatial links, all odd-third-coordinate temporal spins, and the separators. Call this exterior \(\mathcal E_{\rm rect}\). Given it, the compact conditional law factors over rectangles. For sufficiently weak \(\beta\) and rectangles of at most \(e^{c_2\beta}\) sites,
\[
 \mathbb E\operatorname{Var}(r_f\mid\mathcal E_{\rm rect})\le C M_f
 \qquad (SU(2)).
 \tag{PLANE-RECTANGLE-INNOVATION}
\]
The two lateral staples in the third direction give the needed pinning. A one-site bound with four arbitrary internal neighbors would not prove this estimate. We use a finite neighborhood variational comparison to establish the compact tail.

In a rectangle \(I\) let \(v_x\) be one fixed lateral staple, use the actual in-plane transport rotations \(R_{xy}\), and call the exterior good if both lateral staples at every site lie within \(\delta\) of \(v_x\), each internal edge has \(\angle(v_x,R_{xy}v_y)\le\delta\), and every fixed separator spin across a boundary edge matches the transported adjacent reference within \(\delta\). For small fixed \(\delta\), exactly the triangle and marked plaquette argument of §4.62 yields \(\mathbb P(I\text{ bad})\le C|I|e^{-b\beta}\). There are only \(C|I|\) incident plaquettes. When these are all small the actual spins first match their lateral staples and then their in-plane neighbor transports, proving the exterior condition.

We claim that every center spin in a good rectangle has conditional probability at most \(Ce^{-b'\beta}\) of exceeding the cap angle \(\theta=\pi/8\), with no restriction on the size of \(I\). First consider perfect alignment \(\delta=0\). Fix a center \(x\), a square neighborhood of integer radius \(R\) intersected with \(I\), its other spins' arbitrary boundary data inside the plane, and the matched true separator spins. For a minimizing configuration of this finite conditional action set
\[
 E_j=\sum_{\substack{y\in I\\ |x-y|_\infty\le j}}(1-u_y\cdot v_y).
\]
Replacing all these spins by \(v_y\) is an admissible variation for \(j<R\). Its onsite energy equals zero relative to the aligned spin, since each site has two lateral fields equal to \(v_y\). Each internal interaction written as \(1-u_y\cdot R_{yz}u_z\) is nonnegative and becomes zero between two replaced spins. Crossing to a site \(z\) of the next shell, the new value is exactly \(1-u_z\cdot v_z\); crossing to a matched fixed separator it is zero. Minimality thus gives \(2E_j\le4(E_{j+1}-E_j)\) since each outer shell site has at most four such neighbors. Iteration yields \(E_0\le (2/3)^R\,2(2R+1)^2\). The argument remains valid for squares meeting edges or corners, including empty outer shells. It does not assume that the in-plane rotations are identity; preserving the respective reference vectors suffices.

Choose \(R\) fixed and large enough that every such minimizer is strictly within angle \(\theta/2\) at the center. There is a uniform strictly positive energy gap to a central angle \(\ge\theta\). For a formal verification the finite neighborhood has bounded size determined by \(R\), finitely many possible intersections with rectangular boundaries and periodically identified small sides, and compact spaces of rotations, references and arbitrary boundary spins. The minimum value with that closed central constraint and the unrestricted minimum are continuous in these parameters by compactness. Equality would contradict the just established strict angle bound. The gap persists for small enough fixed \(\delta>0\), by taking a convergent subsequence if it failed as \(\delta\downarrow0\). Compact group Haar mass in a fixed small neighborhood of a minimizer gives a uniform lower bound \(c_R e^{-\beta(\min S+\mathrm{gap}/2)}\) on the local normalizer, since all these finite actions have a uniform Lipschitz bound. The constrained numerator is at most \(e^{-\beta(\min S+\mathrm{gap})}\). This proves the central cap tail uniformly even after conditioning all spins outside the neighborhood. Averaging and taking a union bound gives conditional probability \(C|I|e^{-b'\beta}\) of any cap failure.

The positive law on the product caps has a Hessian bound independent of both side lengths. In the spherical Hessian calculation of §4.63 the lateral mass is now at least \(2\cos(\theta+\delta)\). There are at most four internal neighbors; each can lose at most \(1-\cos(2\theta+\delta)\). A fixed matched separator has a positive diagonal contribution because \(\theta+\delta<\pi/2\). At \(\theta=\pi/8\),
\[
 2\cos(\theta+\delta)-4[1-\cos(2\theta+\delta)]>0
\]
for sufficiently small \(\delta\). The product-cap Poincaré constant is therefore \(C/\beta\). On good exteriors the original gradient bound and FIRST, with the true cap probabilities, give at most \(C\sum_{b\in I}f_b^2\) on average. The remaining errors are bounded by \(C\beta^2|I|^2 e^{-c\beta}\sum_{b\in I}f_b^2\), using compact sup norms and the two failure probabilities. Take \(c_2\) smaller than a fixed fraction of \(c\) and sum the independent rectangles. This proves PLANE-RECTANGLE-INNOVATION. The residual is the covariance of the conditional means on the separator lattice, the other temporal planes and the spatial slices.

### 4.66 Full-length strips of increasing transverse width on the \(SU(2)\) law (P)

The plane pinning estimate and the positive bridge argument can be combined. In the even-third-coordinate temporal-spin planes keep odd-second-coordinate separator rows, so that the integrated regions are strips periodic in direction one with transverse width \(w\). All widths may be at most \(e^{c_3\beta}\) for a sufficiently small fixed \(c_3>0\), while their periodic longitudinal length has no restriction. Let \(\mathcal E_{\rm strip}\) retain the separators and the other temporal and spatial data. On the same weak trajectory,
\[
 \sup_{x\in\mathcal C}\sum_{y\in\mathcal C}
  \mathbb E|\operatorname{Cov}(r_x,r_y\mid\mathcal E_{\rm strip})|\le C,\qquad
 \mathbb E\operatorname{Var}(r_f\mid\mathcal E_{\rm strip})\le C M_f .
 \tag{FULL-STRIP-INNOVATION}
\]
The width refers to the number of spins in one column of this actual strip. The proof below keeps its factors explicit. One may omit separators when the entire transverse side is already below the width bound, using periodic rather than fixed edges there.

**A strip bridge with arbitrary outer columns.** Take \(s=\lceil C_2\beta\rceil\) columns with the two endpoint columns fixed arbitrarily, and assume the strip exterior is good in that cylinder: the two lateral staples at all sites, the intervening reference transports and any true top/bottom separators obey the small \(\delta\) conditions of §4.65. This excludes no condition on its two end columns. Extract two interior cut columns at distances between \(s/4\) and \(s/3\) from the respective ends. Every spin from the first cut to the second is more than the fixed variational radius \(R\) from either arbitrary end for sufficiently weak \(\beta\). By the finite-neighborhood argument of §4.65, uniformly in the outer columns, the probability that any spin in this central slab (including its cuts) is outside its reference cap is at most \(Csw e^{-b\beta}\).

Upon restricting the central slab to its product caps, the two cut columns take values in their own caps. The central transfer kernel \(K_{\rm mid}(l',r')\) integrates the spins strictly between the two cuts on their original spherical measures restricted to caps. Its Hessian lower bound is that of §4.65: an internal edge loses at most \(1-\cos(2\theta+\delta)\), while a fixed cap-column neighbor has positive dot product with the adjacent cap spin. The exponentially weighted covariance proof of §4.64 works with strip graph distance, since the off-diagonal Hessian now has at most four neighbors; the Schur commutator still has norm at most \(C\beta(e^c-1)\). A component variation in each cut enters only its nearest central spin score. Integrating the mixed derivatives along cap geodesics for all \(w\) components, with each component speed at most \(2\theta\), gives
\[
 \operatorname{diam}_{\rm cross}\log K_{\rm mid}
       \le C\beta w^2 e^{-c s/3}.
\]
Here the diameter is the supremum absolute four-term difference in GOOD-BRIDGE-RATIO. The cut-column caps are geodesically convex and connected, which permits those paths. Choose \(c_3\) below a fixed fraction of \(c C_2\). The normalized passage across the middle slab therefore has total variation coefficient at most \(C\beta w^2 e^{-c s/3}\), even with arbitrary positive chambers to its left and right.

For the kernel of the **entire unrestricted** bridge take outer endpoint derivatives along unit-speed paths in each sphere of an endpoint column. Their scores have sup norms at most \(C\beta w\). The mixed derivative of the full log kernel is their covariance. Changing to the law with only its middle slab restricted costs at most \(C\beta^2w^2 sw e^{-b\beta}\) by the uniform cap-failure probability. On that restricted law the two endpoint chambers communicate only through \(K_{\rm mid}\); the conditional expectation of the right score has oscillation at most twice its sup norm times the middle variation coefficient. This bounds the score covariance by \(C\beta^3w^4 e^{-c s/3}\). Thus the full four-term log cross-ratio is at most
\[
 C\beta^2 w^3 s e^{-b\beta}+C\beta^3 w^4 e^{-cs/3}
      \le e^{-b_6\beta}
\]
after decreasing \(c_3\) and passing to the weak range. All outer endpoint configurations were allowed, so the resulting contraction survives any positive column message. This intermediate-cap construction is necessary: arbitrary outer columns need not be compatible with a small cap at the very ends of the original bridge.

**Longitudinally distant sites.** On a strip with the exterior fixed the column process is a periodic nearest-neighbor chain, now with state space \((S^3)^w\). A bad bridge entails at least one threshold Wilson plaquette in its cylinder of \(Csw\) candidate plaquettes. Designate bridges separated by \(s\) unused columns; their candidates are disjoint. For \(h\) specified bad bridges, MARKED-EXP bounds the full probability by \((Csw e^{-b_7\beta})^h\). Taking \(c_3<b_7/2\), the product of variation coefficients averages to at most \(e^{-b_8\beta h_0}\) for \(h_0\) designated bridges as in §4.64. Condition on the three columns in the longitudinal support of \(r_x\), keeping all neighboring rows needed by the insertion within those columns. On the two complementary arcs the same column transition comparison gives
\(\mathbb E|\operatorname{Cov}(r_x,r_y\mid\mathcal E_{\rm strip})|\le C\beta^2e^{-c'd_1(x,y)}\) for \(d_1\ge16s\), where \(d_1\) is longitudinal periodic distance. There are at most \(2w\) sites per longitudinal shell. Further reducing \(c_3\), their whole distant contribution to the row sum is bounded.

**Nearby columns.** For \(d_1<16s\) take a strip window of at most \(20s+O(1)\) columns with buffers of size \(s\) from the two supports. If the whole longitudinal circle is shorter, use the periodic strip with no end chambers. The exterior goodness condition for this window fails with probability \(Csw e^{-b\beta}\) under the full law. For good data and arbitrary end columns, choose interior cuts in the two buffers at distance at least \(s/3\) from the supports and at least \(s/3\) from the outer ends. The probability of any cap failure between the cuts, including on their columns, is at most \(Csw e^{-b\beta}\) as above. Replacing the conditioned full window by its central-cap law therefore changes covariances by at most \(C\beta^2sw e^{-b\beta}\).

Given its cut columns in the caps, the interior weighted covariance of \(r_x,r_y\) has the factor \(C\beta^{-1}e^{-c d(x,y)}\) times the product of the two local gradient norms. Here \(d\) is the two-dimensional strip distance. The means of either interior observable vary across all cap cut-column values by at most \(C\beta w e^{-c s/3}\), from differentiating in the cuts and using the same weighted covariance with the crude compact gradient norms. Therefore the retained covariance across the two cuts is at most a polynomial in \(\beta,w\) times \(e^{-c s/3}\). The interior means differ from their values at the two reference cut columns by this same bound, uniformly in arbitrary chambers. On passing back to the unrestricted window, their expectations acquire at most \(C\beta sw e^{-b\beta}\). Thus varying the arbitrary outer endpoints has only this combined small effect on the two means. This also bounds the extra covariance when conditioning down from the whole periodic law to the window. In the short-circle case take all its caps at once, using the circular two-dimensional distance, with no such endpoint terms.

On good exteriors the probability of the central caps exceeds \(1/2\) uniformly in the outer values. Integrating its normalized gradient second moments, with its true random cut columns, therefore costs at most twice the full Wilson moments. As in §4.64, FIRST and the local gradient formula cancel the \(1/\beta\) prefactor by Cauchy–Schwarz. Each near-site bound is \(Ce^{-c d(x,y)}\) plus a fixed polynomial in \(\beta,w\) times \(e^{-b'\beta}\); the bad exterior is included through its probability and the compact insertion bound. There are at most \(Csw\) near sites. The powers of \(w\) here are fixed (the cap-replacement error is \(C\beta^2sw e^{-b\beta}\), and the cut-mean error uses at most \(w^2\)). Taking \(c_3\) smaller than the corresponding fixed tail ratios keeps their total bounded independently of strip width and length. The two-dimensional spatial exponential itself has uniformly summable rows. This proves FULL-STRIP-INNOVATION. Distinct strips have conditional covariance zero. What remains for SUS is the signed covariance between the actual conditional means on the retained transverse separator planes, odd-third-coordinate temporal spins and spatial links.

### 4.67 Uniform innovation after retaining sparse temporal separators, every \(SU(N)\) (P)

There is a stronger result for three-dimensional temporal-spin boxes with increasing thickness. On each time layer retain temporal links on separator planes in the three spatial directions, taking the separator coordinates odd so none is a marked comb site. Also fix all spatial links. Let \(\mathcal E_{\rm sep}\) be the sigma-field of these retained variables. The remaining spins are in disjoint boxes, independent conditionally on \(\mathcal E_{\rm sep}\). Suppose every box has vertical thickness at most \(h\), meaning at most \(h-1\) spins between fixed third-direction separator planes, and at most \(M\) sites in total. The ranks and group conventions are fixed. For sufficiently weak \(\beta\) and
\[
  2\le h\le \beta^{1/24},\qquad M\le \exp(c_0\beta h^{-16}),
\]
on the same reference tori as MARKED-EXP, the **full compact Wilson law** satisfies
\[
 \mathbb E\,\operatorname{Var}(r_f\mid\mathcal E_{\rm sep})
       \le C_N M_f .
 \tag{SPARSE-SEPARATOR-INNOVATION}
\]
The constant is independent of \(h,M,\beta\), the side and the mesh. For example \(h\to\infty\) below the displayed threshold and increasing horizontal side lengths allow the fraction of retained temporal links to tend to zero. All fixed spatial links and their conditional-mean covariance remain. A small fraction of retained coordinates does not imply a small variance of functions of those coordinates.

**Reference and bad exterior.** A temporal spin \(u_x\in SU(N)\) at a spatial site interacts with the next spin \(u_y\) by \(s_p=\frac12\|u_x-R_{xy}u_y\|_{\rm HS}^2\), where \(R_{xy}\) is left and right spatial parallel transport, an isometry of the embedded group and matrix Hilbert space. Define \(v_x\) by exact vertical transport of the fixed temporal spin on the bottom separator to \(x\), using only these fixed spatial links. Internal vertical references match exactly. Set \(\delta=\epsilon_0 h^{-7}\), with \(\epsilon_0>0\) chosen below. A box is good when all its other reference bonds and its true boundary separator spins match under the respective transports within distance \(\delta\), in the Hilbert–Schmidt norm. The condition involves only \(\mathcal E_{\rm sep}\). If all actual temporal plaquettes on the determining columns and their bounded horizontal collar have \(\|u_x-R_{xy}u_y\|_{\rm HS}\le\delta/(C h)\), telescoping along the vertical paths puts each actual spin within \(\delta/C'\) of its reference, and the indicated compatibility follows, including top and side separators. The number of plaquettes in this check is at most \(C hM\), allowing all collars. Thus
\[
 \mathbb P(\text{bad box})\le C hM e^{-b\beta h^{-16}}
\]
by the full one-plaquette exponential tail. No product approximation is made for the retained exterior.

**A quantitative pinning estimate.** Use the intrinsic bi-invariant metric induced by the embedding and geodesic caps \(d(u_x,v_x)\le\theta=\theta_0 h^{-2}\), with \(\theta_0\) small. On every good exterior the compact conditional probability that any spin leaves its cap is at most
\[
 C M\exp(-b'\beta h^{-6}+C h^7\log(h+1)).
 \tag{VERTICAL-PINNING-TAIL}
\]
Here are the details uniform in thickness. Fix a spin and take a horizontal square of radius \(R=\lceil K h^3\rceil\), intersected with the true box and including its full vertical columns. Condition on every spin beyond this neighborhood. Boundary data beyond the horizontal square can be arbitrary. Write \(B_j\) for the corresponding neighborhood at radius \(j\le R\), with full vertical columns. It has at most \(M_R\le C_K h^7\) sites. For any local configuration put \(E_j=\sum_{x\in B_j}\|u_x-v_x\|^2\). The exact vertical reference and the fixed bottom spin give
\[
 E_j\le C h^2
     \sum_{\text{vertical edges from bottom in }B_j}
                     \|u_x-R_{xy}u_y\|^2
\]
by telescoping on each column and Cauchy–Schwarz. Suppose the local action of the configuration is within \(\Delta\) of its conditional minimum in \(B_R\). Replace the spins in \(B_j\), \(j<R\), by their references. Internal reference action and reference action against true separators are at most \(C M_R\delta^2\). At crossing edges to the next horizontal shell, the replacement cost is at most \(C(\delta^2+\|u_y-v_y\|^2)\). Only a bounded number of edges meets each shell site. All original changed-edge costs are nonnegative, and the vertical energies above are included. Comparison with this admissible modification gives
\[
  c h^{-2}E_j\le C(E_{j+1}-E_j)+C M_R\delta^2+\Delta .
\]
Consequently \(E_0\le q_h^R C M_R+C h^2(M_R\delta^2+\Delta)\), with \(1-q_h\ge c h^{-2}\). Choose \(K\) sufficiently large to make the first term below a small fixed multiple of \(\theta_0^2 h^{-4}\) for all \(h\ge2\). Then choose \(\epsilon_0\) small and \(\Delta=\epsilon_2 h^{-6}\) with \(\epsilon_2\) small. The other terms fit the same bound. Uniform comparison of intrinsic and chord distance near identity on the compact group gives \(d(u_x,v_x)<\theta\) at the center. Thus a central cap failure costs an action gap at least \(\Delta\), independently of the conditioning beyond \(B_R\).

Every local action is \(C M_R\)-Lipschitz in the supremum of the site geodesic distances, since it is a sum of fixed smooth Wilson terms. Small Haar balls of radius \(c\Delta/M_R\) about a minimizer give a denominator lower bound at least \(\exp[-\beta(\min S+\Delta/2)-C_N M_R\log(C M_R/\Delta)]\). The cap-failure numerator is bounded by \(\exp[-\beta(\min S+\Delta)]\). This proves the individual-site bound uniformly in the arbitrary conditioning. Average and sum the sites for VERTICAL-PINNING-TAIL. For the stipulated \(h\), its entropy term is smaller than half the negative exponent at sufficiently large \(\beta\).

**Coercivity of the actual cap law.** Let \(X_x\in T_{u_x}SU(N)\) be tangent velocities, extended by zero on retained sites. Denote the full covariant edge norm in the box and on its incident bonds by
\[
 \mathcal D(X)=\sum_{\langle x,y\rangle}\|X_x-R_{xy}X_y\|_{\rm HS}^2 .
\]
The same vertical telescoping yields \(\sum_x\|X_x\|^2\le C h^2\mathcal D(X)\), independently of the rotations. For one edge the Riemannian Hessian of \(\tfrac12\|u_x-R_{xy}u_y\|^2\) is \(\|X_x-R_{xy}X_y\|^2\) plus the scalar product of \(u_x-R_{xy}u_y\) with the difference of the two geodesic accelerations. On the compact embedded group the latter are bounded by \(C_N(\|X_x\|^2+\|X_y\|^2)\), by its bounded second fundamental form. On the good caps each edge chord is at most \(C_N(\theta+\delta)\), including a fixed separator edge with exterior velocity zero. Summing the bounded-degree errors and using the vertical inequality proves
\[
 \operatorname{Hess}(\beta S)[X,X]\ge c_N\beta\,\mathcal D(X)
\]
when \(\theta_0,\epsilon_0\) are small. This is a lower bound in the *edge norm*, stronger for the present purpose than replacing it by the smallest Dirichlet eigenvalue. Small geodesic caps are convex on this fixed compact group; the bi-invariant Ricci curvature is nonnegative. The one-form covariance identity of §4.64 then gives the following variational bound: if \(|dF(X)|^2\le B(u)^2\mathcal D(X)\) pointwise, then \(\operatorname{Var}_{\rm cap}F\le C_N\beta^{-1}\mathbb E_{\rm cap}B(u)^2\). Indeed apply Cauchy–Schwarz in the quadratic form to the inverse one-form operator, whose other rough-gradient, Ricci and convex-boundary terms are nonnegative. The cap probability itself is not absorbed into any inverse covariance.

**Gradient of the ordinary temporal mark.** On the fixed spatial transport graph put \(L_i=T_i+T_i^*-2I\), as in §4.60. Because its tangent projection kills \(u_x\), the squared matching force is \(\tau\|\Pi_{T_{u_x}}L_i u(x)\|^2\). Write this as the full squared norm minus the squared normal projection. The Casimir \(\ell_x\) differs from a fixed constant by a fixed multiple of \(e_x=\sum_{p\ni x}s_p\). For an arbitrary sign-changing comb mark the ordinary sum \(F=\sum_{x\in I\cap\mathcal C}f_x r_x\) satisfies
\[
 |dF(X)|^2\le C_N\beta^2\mathcal D(X)
  \sum_{x\in I\cap\mathcal C}f_x^2(e_x+e_x^2+h^2e_x^3)
 \qquad(\beta\ge1).
 \tag{EDGE-DUAL-ORDINARY-GRADIENT}
\]
To check the main squared norm differentiate it once: Cauchy–Schwarz puts \(\sum f_x^2\|L_i u(x)\|^2\le C\sum f_x^2 e_x\) in the first factor and \(\sum_{x,i}\|L_i X(x)\|^2\le C\mathcal D(X)\) in the second. The last inequality follows on the entire slice after zero extension because \(L_i=-(I-T_i)^*(I-T_i)\) and \(\|I-T_i\|\le2\) on the matrix Hilbert space. For the normal term, §4.60 gives \(\|\Pi_N L_i u(x)\|\le C e_x\). Its variation is bounded by \(C(\|L_i X(x)\|+\|X_x\|\sqrt{e_x})\), using the smooth tangent projection on the compact group and \(\|L_i u(x)\|\le C\sqrt{e_x}\). The first summand supplies the \(e_x^2\) term. For the second use the vertical bound \(\|X\|_2\le C h\mathcal D(X)^{1/2}\), supplying \(h^2 e_x^3\). Differentiating the actual Casimir energy uses only the first edge variation of \(\tfrac12\|u_x-Ru_y\|^2\), also controlled by the first term. This proves the gradient bound with a constant independent of the number of columns and the slab thickness.

Apply the variational cap inequality, multiply by its original conditional probability on good boxes and integrate. MARKED-EXP gives \(\mathbb E e_x^j\le C_j\beta^{-j}\) for \(j=1,2,3\) on the fixed stencil. Hence the annealed cap contribution is bounded by
\[
 C_N(1+\beta^{-1}+h^2\beta^{-2})\sum_{x\in I\cap\mathcal C}f_x^2
      \le C_N' \sum_{x\in I\cap\mathcal C}f_x^2.
\]
For the other terms use the inner mean on a good exterior and zero otherwise, as in §4.62. The compact bound on \(F^2\) is \(C\beta^2 M\sum_{x\in I}f_x^2\). Both the exterior failure and the inner compact tail are absorbed uniformly: \(M\le e^{c_0\beta h^{-16}}\), \(\beta h^{-16}\ge\beta^{1/3}\), and \(c_0\) is chosen smaller than the fixed tail constants. Box independence completes the proof. The calculation covers the whole innovation of the already retained SINGLE-LINK-MEAN on these boxes as well, by the positive tower. A full Wilson Poincaré estimate has not been used.

### 4.68 Four-dimensional Wilson boxes with sparse retained faces (P)

One can integrate all four orientations in each microscopic box with a side increasing along the weak trajectory. Partition the four-dimensional fine torus by coordinate hyperplanes into rectangular cells of maximum side \(s\ge2\). Retain all links *tangential* to any cell face. Spatial separator coordinates are odd in the three directions transverse to the chosen temporal comb. Thus every marked temporal bond is free inside precisely one cell and all of its incident plaquettes belong to that same closed cell, even at a time boundary. All remaining plaquettes live in a single closed cell or consist entirely of retained links. With \(\mathcal E_{\rm face}\) the retained sigma-field, conditional Wilson integrals over the free links of different cells are independent. Under MARKED-EXP and FIRST, uniformly for \(s\le\beta^{1/30}\) and all sufficiently weak \(\beta\),
\[
 \mathbb E\operatorname{Var}(r_f\mid\mathcal E_{\rm face})
                 \le C_N M_f
 \quad\text{for every real mark supported on the comb.}
 \tag{FOUR-DIMENSIONAL-BOX-INNOVATION}
\]
In compatible partitions with all side lengths comparable and tending to infinity, the face links are a vanishing fraction of the original links. They include links in every orientation. This is an actual positive-coordinate disintegration of the Wilson measure, distinct from the prescribed Balaban block-spin variables.

**Boundary gauge and exact free-coordinate measure.** In one box \(B\), choose a tree spanning its boundary vertices using only boundary links, with paths of length \(C s\). For example a breadth-first tree has this property since the graph diameter of the boundary of a four-dimensional coordinate box is \(O(s)\). One can join each boundary point to a corner along a boundary face of fixed coordinate, and join corners along the edges. Attach interior vertices by time-direction paths to their bottom face roots, making a forest; its union with the boundary tree is a spanning tree of depth \(C s\). For boxes with no interior vertices omit this forest. The boundary gauge setting the boundary tree to identity uses retained data only. It may be chosen separately in each conditional integral, since the integrand and readout are gauge invariant. Now integrate the based interior site gauges by fixing the forest links to identity. Product Haar invariance gives exactly normalized Haar on the non-tree free chords: successively use the tree links as independent site gauge variables and translate each chord at its endpoints. No Faddeev–Popov weight depending on the chords is introduced. Non-tree boundary links stay at their actual boundary-gauged values.

Say the boundary is good and the cell lies in its inner chart when respectively all its non-tree boundary logs, and all non-tree free logs, have norm at most \(\epsilon_s=\epsilon_1 s^{-8}\) in these gauges, with \(\epsilon_1\) small. A configuration with all its cell plaquette defects below \(c\,\epsilon_s/s^2\) in matrix norm satisfies both requirements. Indeed each chord after tree fixing is the holonomy around a tree-chord loop of length \(O(s)\). A closed coordinate word of that length in a rectangular box admits an elementary filling with at most \(C s^2\) plaquettes in the box: interchange neighboring steps of distinct axes to sort the word, then erase backtracking. Each interchange stays in the rectangle since each coordinate follows its own original sequence of positions. The successive changes differ by conjugated plaquette holonomies. The unitary matrix norm gives a sum bound by those defects, without multiplying their errors. This argument also applies to a boundary loop filled using the actual interior field. It implies the **full-law**, undivided probability estimate
\[
 \mathbb P_{\rm Wilson}(\text{bad boundary or failed free chart in }B)
       \le C_N s^4\exp[-c_N\beta s^{-20}] .
 \tag{BOX-CHART-TAIL}
\]
There are \(O(s^4)\) plaquettes and \(s_p=\tfrac12\|U_p-I\|_{\rm HS}^2\). Above-threshold defects accordingly use the one-plaquette Wilson exponential bound. We do not divide this tail by a conditioned boundary mass.

**Curvature coercivity on the exact chart.** In the real logarithmic coordinates of the free chords, let \(X\) be a velocity array, extended by zero to all fixed tree and boundary links. The flat linearized curl is \(dX\) on the plaquettes of the box. Every chord component is the sum of \(dX\) over its same oriented filling because tree and boundary variations vanish. It follows that
\[
 \|X\|_2\le C s^4 \|dX\|_2.
\]
Indeed a component is at most \(C s^2\|dX\|_\infty\) by counting the filling with multiplicity, and there are \(O(s^4)\) links. A fixed orientation subset of plaquettes, such as one of the three matchings, gives the restricted differential \(d_i\) with \(\|d_i X\|\le\|dX\|\).

The physical Wilson action Hessian at the all-identity configuration is \(\tau d^*d\) in these coordinates. Each plaquette is a smooth fixed group word with bounded third derivatives on a fixed small ball. With every boundary and free log of size at most \(\epsilon_s\), the Hessian error has row and column absolute sums bounded by \(C_N\epsilon_s\), because each link touches only a fixed number of plaquettes. Restriction to tree-fixed velocities preserves this bound. The Haar logarithmic Jacobian Hessian has norm at most \(C_N\) as it is a sum of independent chord terms. Therefore on the actual conditional product of convex log balls the Hessian of the negative logarithm of the density satisfies
\[
 \operatorname{Hess}(-\log w_B)[X,X]\ge c_N\beta\|dX\|_2^2 .
\]
Here \(C_N\epsilon_s s^8\) is made small by choosing \(\epsilon_1\), and \(C_Ns^8/\beta\) is small for \(s\le\beta^{1/30}\). These constants do not increase with the side in the final curl-norm lower bound. Reflection positivity or a full-lattice spectral gap does not enter this calculation.

**Dual curl bound for the original ordinary insertion.** For \(F=\sum_{b\in B\cap\mathcal C} f_b r_b\) and \(e_b=\sum_{p\ni b}s_p\), the same inner chart satisfies
\[
 |dF[X]|^2\le C_N\beta^2
        \left(\sum_{b\in B\cap\mathcal C} f_b^2 e_b\right)\|dX\|_2^2 .
 \tag{BOX-CURL-DUAL}
\]
To verify the force term, differentiate its actual link gradient \(F_{b,i}=X_b S_i\) in the chosen physical logarithms. At identity the resulting matrix is \(\tau d_i^*d_i\). The left-invariant gradient and logarithmic derivative agree there; the conversion of generators away from identity is a local analytic matrix with bounded derivatives, and the action's first jet vanishes at identity. Each row of the force derivative involves only the original plaquette stencil and fixed smooth functions of its logs. Its deviation from this flat matrix thus has Schur norm at most \(C_N\epsilon_s\) on this chart. Only rows for the marked bonds are needed; their full stencils lie inside the cell. Also \(\|d_i^*d_i X\|\le C\|dX\|\) since the elementary incidence matrices have bounded degree and \(\|d_i X\|\le\|dX\|\). The perturbation \(C_N\epsilon_s\|X\|\) is paid by the linear curl inequality. Finally \(\sum_i |F_{b,i}|^2\le C_N e_b\) pointwise. Cauchy–Schwarz in differentiating \(\beta\sum f_b|F_{b,i}|^2\) now yields (BOX-CURL-DUAL) for this term.

For the Laplacian part the Casimir identity makes \(\ell_b\) a constant minus a fixed multiple of \(e_b\). The derivative of a plaquette energy has modulus at most \(C_N\sqrt{s_p}\,\|D P_p[X]\|\), by the matrix squared-distance formula. The collection of plaquette variations \(D P_p[X]\) differs from the flat curl by a bounded-degree matrix error of Schur norm \(C_N\epsilon_s\). Thus its squared sum is at most \(C_N\|dX\|^2\). Applying Cauchy–Schwarz in the incidences of the marked bonds, each with a bounded number of plaquettes, proves the same dual bound for the Laplacian term. This completes (BOX-CURL-DUAL) for arbitrary signs of the mark.

The convex product-chart covariance inequality in its matrix form now gives
\[
 \operatorname{Var}_{\rm chart}F
 \le C_N\beta\sum_{b\in B\cap\mathcal C}f_b^2
                                  \mathbb E_{\rm chart}e_b .
\]
For example this follows by the same one-form inverse variational argument as §4.67, now on the ordinary Euclidean log-coordinate space with lower quadratic form \(c_N\beta d^*d\). Multiply by the true conditional chart probability on a good boundary, then integrate over the original Wilson boundary law. FIRST cancels the one remaining \(\beta\), uniformly in side and cutoff.

On a bad boundary compare \(F\) with zero. On a good boundary compare to its normalized chart mean, retaining the complete compact complement in the error. The squared sup norm of \(F\) is bounded by \(C_N\beta^2 s^4\sum_{b\in B} f_b^2\). BOX-CHART-TAIL bounds the integrated cost of these two events by
\[
 C_N\beta^2 s^8 e^{-c_N\beta s^{-20}}\sum_{b\in B} f_b^2
       \le C_N'\sum_{b\in B} f_b^2 ,
\]
since \(\beta s^{-20}\ge\beta^{1/3}\). Summing the independent boxes proves FOUR-DIMENSIONAL-BOX-INNOVATION. In particular, on the weak trajectory the only remaining part after this permitted integration is
\(\operatorname{Var}(\mathbb E[r_f\mid\mathcal E_{\rm face}])\).
That boundary functional retains the physical low modes. The vanishing density of the faces alone makes no estimate of its covariance.

### 4.69 The actual face conditional mean at an increasing box scale (P)

The boundary quantity left in FOUR-DIMENSIONAL-BOX-INNOVATION has a computable leading term on the complete finite box. Use the same exact tree fixing, put \(g=\beta^{-1/2}\), and write the boundary non-tree links as \(\exp(gD_e)\) on their principal chart. Take \(2\le s\le\beta^{1/200}\), \(P=\log\beta\) for sufficiently large \(\beta\). Except on a full-law boundary event of probability \(C_Ns^4e^{-c_NP^2}\), all these canonical boundary logs have \(\|D\|_\infty\le C_Ns^2P\). Indeed each boundary chord has the filling in §4.68, and a failure requires a cell plaquette defect of size at least \(c gP\). This check uses the original Wilson marginal.

Let \(H=\tau d^*d\) in the Gaussian action on the complete box, with the tree components pinned to zero. Denote by \(E D\) the flat harmonic minimizing extension with the specified boundary values, and by \(C=(H|_{\rm free})^{-1}\) the free-coordinate covariance, extended by zero on the fixed slots. Write \(H_i=d_i^*d_i\) for the incidence operator of matching \(i\), including the marked output row and all its actual plaquettes. For an original marked temporal link \(b\), define
\[
 m_b^{G}(D)=\tau^2\sum_i
     \left[|(H_i E D)_b|^2+
       \operatorname{tr}_{\rm col}(H_i C H_i^*)_{bb}\right]-\ell_b(I)/3 .
 \tag{FACE-GAUSSIAN-ROW}
\]
This is the exact Gaussian conditional mean with a boundary-independent trace. The harmonic term uses actual boundary data. On the stated good boundary the true compact Wilson conditional mean satisfies
\[
 \left|\mathbb E[r_b\mid\mathcal E_{\rm face}]-m_b^{G}(D)\right|
 \le C_N\beta^{-1/2}s^{44} P^5+C_N\beta e^{-c_NP^2}.
 \tag{FACE-MEAN-COMPARISON}
\]
The constants are independent of the cell and torus sides. The per-link bound tends to zero at this increasing box scale. It also holds in full-law \(L^2\) up to an additional \(C_N s^C e^{-c_N'P^2}\) if the approximant is set to \(m_b^G(0)\) outside the good boundary event. This is not yet an \(L^2\) bound for the sum over the torus.

Here are the finite-dimensional estimates including their volume powers. Extend \(D\) by zero on the free slots to \(\widetilde D\). The minimizing extension obeys \(\|d E D\|_2\le\|d\widetilde D\|_2\le C s^2\|D\|_\infty\). Applying the flat curl bound of §4.68 to the free part \(E D-\widetilde D\) gives \(\|E D-\widetilde D\|_2\le C s^6\|D\|_\infty\le C s^8P\), and \(\|C\|_{\rm op}\le C s^8\). Take \(T=C_4s^8P\) with a sufficiently large fixed \(C_4\). Under the actual Gaussian conditional density the probability of any canonical free coordinate exceeding \(T\) is \(C s^4e^{-cP^2}\) or smaller, by the one-coordinate Gaussian tail. Fixed polynomial moments of \(H_i B\) on this tail are suppressed by the same estimate at a slightly reduced rate.

The compact Wilson complement is small relative to the same Gaussian integral. If a free chord lies outside the real chart of radius \(gT\), its tree path forces a plaquette defect at least \(c gT/s^2\). Thus its unnormalized compact mass is at most \(e^{-c T^2/s^4}\), since all action terms are nonnegative. For the Gaussian integral in the same physical normalization (including the common leading Haar and canonical factors) a lower bound follows by taking every free canonical coordinate in a fixed unit ball:
\[
 Z^G(D)\ge
    \exp[-C_N s^4(\log\beta+1)-C_N s^8P^2].
\]
The term \(s^8P^2\) bounds the canonical energy of the boundary extended by zero. With the chosen \(T\), the compact complement relative to this lower bound is at most \(e^{-cP^2}\), after increasing \(C_4\). Group coordinates outside any principal log are counted in this same compact bound.

On the inner canonical region write the free links as \(e^{gB_e}\). Taylor expansion of each fixed plaquette word on its common small ball gives total exponent error at most \(C_N g s^4T^3\), while the Haar logarithmic correction is at most \(C_N g^2s^4T^2\). Uniformity uses \(gT\ll1\) and the bounded stencil multiplicity. Their sum is \(O_N(g s^{28}P^3)=o(1)\) at the chosen side. Hence the ratio of the true normalization to \(Z^G(D)\) is \(1+O_N(g s^{28}P^3+e^{-cP^2})\). The compact insertion outside this chart is bounded by \(C_N\beta\).

The original \(r_b\) on the chart differs from \(\tau^2\sum_i |(H_i B)_b|^2-\ell_b(I)/3\) by \(O_N(gT^3)\): the matching force has first jet \(g\tau H_i B\), with error \(O_N(g^2T^2)\), and the Casimir is a bounded smooth function. Here \(B\) includes the prescribed boundary values. The leading insertion has absolute size at most \(C_N(1+T^2)\). Combining with the relative normalization estimate and the tail bounds yields (FACE-MEAN-COMPARISON). The trace in (FACE-GAUSSIAN-ROW) is uniformly bounded per marked root since the covariance is the inverse of \(\tau d^*d\) on the free space and \(d_i^*\) has bounded incidence norm. This also bounds \(m_b^G(0)\). Jensen, the full fourth moment of \(r_b\), and the previously bounded bad-boundary probability prove the asserted \(L^2\) version.

Fixed derivatives in finitely many **canonical boundary slots** have the same comparison on an interior real good chart with a spare constant in its \(C_Ns^2P\) bound. Here is the complex-radius check. Vary \(D\) in those slots by uniformly bounded complex coordinates. For the compact integral extend the Wilson trace by its usual holomorphic inverse-word formula. Relative to the real part of the varied logarithms, an imaginary variation has zero first real exponent derivative and a bounded second derivative on the fixed complex group neighborhood. The change in real exponent is therefore \(O_m(\beta g^2)=O_m(1)\), with only the finite varied stencils involved; this also controls the compact complement. In the Gaussian integral the modulus of the real-free-coordinate density changes by at most \(e^{C_m}\), because only the imposed boundary directions are imaginary and the incidence matrix has bounded norm. Its exact normalization has modulus at least the one for the corresponding real part, by the harmonic minimizing quadratic formula. The inner Taylor comparison is consequently still \(O_m(g s^{28}P^3)\) relative to the nonvanishing complex Gaussian, on that fixed comparison polydisc. Compact nonvanishing there and Cauchy's formula on a smaller disc give the fixed-slot derivative claim. This does not supply a uniform bound after summing arbitrary boundary anchors with their true correlated Wilson law.

Subtracting the identity trace leaves an explicit quadratic harmonic face functional and the indicated small local error. Thus the missing sum in the variance tower can now be approached on the actual sparse Wilson face marginal. Independence of interior boxes does not give independence of the face data or of their accumulated comparison errors.

### 4.70 The harmonic face response costs only surface area (P)

For a rectangular Dirichlet cell let \(D\) be arbitrary real linear boundary link data and \(F=d E D\) the curvature of its harmonic minimizing extension. Then the convergent boundary operator in FACE-GAUSSIAN-ROW obeys
\[
 \sum_{\text{free }b,i}|(H_i E D)_b|^2
       \le C\sum_{\text{boundary plaquettes }p}|(d_\partial D)_p|^2 .
 \tag{HARMONIC-FACE-FORCE}
\]
The constant is independent of side length and aspect ratios. A boundary plaquette here is one wholly contained in the boundary; the tangential curvature equals \(d_\partial D\). The assertion holds before tree fixing since the curvature is invariant. Indeed every interior variation is a tree-fixed variation plus an interior vertex gradient with zero boundary values, by integrating that gradient on the attached forest. Stationarity therefore implies \(d^*F=0\) on every free edge, and \(dF=0\) holds on every elementary three-cell by exactness.

To prove the bound, double every side of the rectangle periodically by reflecting it. On each reflection extend \(F\) by minus the pullback of the reflected two-form, including the usual sign for reversing an oriented cell. Set its tangential boundary plaquette values to zero first. The resulting \(\widetilde F\) is well-defined on the doubled torus. An oriented plaquette contained in a reflecting hyperplane must vanish by this parity; a plaquette normal to the plane is sent to its adjacent mirror. On free edges of each copy, \(d^*\widetilde F=0\) by stationarity, because none of their incident plaquettes lies entirely in the boundary. On any boundary edge lying in a reflecting hyperplane, the relative parity of \(d^*\widetilde F\) forces it to vanish. Thus \(d^*\widetilde F=0\) everywhere. The exterior derivative \(d\widetilde F\) inside each copy differs from zero only by the boundary plaquettes that were set to zero. Each contributes to a bounded number of three-cells over the \(2^4\) copies. Hence
\[
 \|d\widetilde F\|_2^2+\|d^*\widetilde F\|_2^2
 \le C\sum_{p\subset\partial B}|(d_\partial D)_p|^2 .
\]
The left side equals \(\sum_{\mu,I}\|\partial_\mu\widetilde F_I\|_2^2\) on the periodic cubical lattice. For completeness, at each momentum the exterior differential is exterior multiplication by the vector of forward-difference symbols (with the convention's unit cell phases); the adjoint is contraction by its complex conjugate. Their squared norms add to the squared length of that vector times the squared form norm. This is the displayed identity by Fourier inversion. For a free bond each matching contains just one incident plane, so \(H_i E D\) is a first difference of one curvature component at its two opposing plaquettes. These values are not changed by the boundary prescription. The periodic identity therefore bounds the desired sum, proving (HARMONIC-FACE-FORCE).

On the true good Wilson boundary of §4.69, each boundary plaquette logarithm expands as \(g (d_\partial D)_p+O_N(g^2\|D\|_\infty^2)\). The group word has only four factors and its principal chart holds on that set. It follows for every fixed \(p_0\ge1\) that
\[
 \left\|1_{\rm good}\sum_{p\subset\partial B}
                |(d_\partial D)_p|^2\right\|_{L^{p_0}(\mu_\beta)}
 \le C_{N,p_0}s^3 .
\]
Indeed the sum is bounded by \(C\beta\sum_{\partial B}s_p+C s^3g^2 s^8P^4\), and each \(\beta s_p\) has uniformly bounded fixed moments by MARKED-EXP. Combining with FACE-MEAN-COMPARISON gives an actual surface estimate. Subtract the field-independent \(c_b=m_b^G(0)\); then on the shrinking-mesh sequence of §4.69,
\[
 \left\|\sum_{b\in B\cap\mathcal C}
       |\mathbb E(r_b\mid\mathcal E_{\rm face})-c_b|
       \right\|_{L^{p_0}(\mu_\beta)}
         \le C_{N,p_0}s^3 .
 \tag{WILSON-FACE-SURFACE}
\]
The summed local error has size \(O(s^4g s^{44}P^5)\le Cs^3\); on the bad set use conditional Jensen, the true higher fixed moment of \(r_b\) and the superpolynomial marked tail. In particular the nonidentity face term has surface rather than volume order even in absolute per-box norm. A constant-curvature bulk mode need not have surface-order *energy*, but (HARMONIC-FACE-FORCE) estimates directional forces, which is precisely what this ordinary source requires.

### 4.71 Surface suppression of the next real Wilson innovation (P)

Take two nested compatible 4D grid partitions with fine cell sides comparable to \(s\) and outer sides comparable to \(S\), \(2\le s\le S\le\beta^{1/200}\). Keep the spatial grid faces off the marked comb sites as before. Write \(\mathcal F_s,\mathcal F_S\) for the respective true face link sigma-fields, with \(\mathcal F_S\subset\mathcal F_s\). For the unit comb, or any comb weights \(|f_b|\le1\),
\[
 \mathbb E\,\operatorname{Var}\left(
          \mathbb E[r_f\mid\mathcal F_s]\ \middle|\ \mathcal F_S\right)
               \le C_N n^4/s .
 \tag{NESTED-FACE-INNOVATION}
\]
This identifies a genuinely decreasing innovation in the real full-sector Wilson tower. The estimate uses \(n^4\) for the full reference lattice and does not claim the same relative improvement for a mark concentrated on faces.

Work in one outer box and write \(F\) for its marked sum. Use an adapted outer tree: keep the outer boundary tree, attach a shortest rooted forest spanning vertices on the whole inner face grid, and finally attach the ordinary short forests inside its subcells. Paths from inner face vertices to the outer boundary have length \(O(S)\), since one can travel along a coordinate face to an outer face by varying a coordinate tangent to it. A forest of shortest paths to the outer boundary realizes this bound; the additional subcell paths have length \(O(s)\). This tree has depth \(O(S)\), so every estimate in §§4.68–4.69 for the outer integral still holds. The gauge on the retained inner skeleton uses only its own links and outer boundary data. Conditioning on that skeleton thus leaves the independent subcell integrals in their usual gauges. In the linear Gaussian integral the same statement follows by the exact linear tree change of variables. Conditional Gaussian curvature inside each subcell depends on its boundary through \(E D\), modulo a gradient. Its conditional covariance trace is precisely that in FACE-GAUSSIAN-ROW.

In the actual compact field define the inner Gaussian row on *all* configurations by using principal real boundary logarithms in each subcell's boundary tree (choose any bounded Borel branch on its cut). Canonical boundary logs then have size \(O_N(\sqrt\beta)\). The harmonic estimate \(\|E D-\widetilde D\|_2\le C s^6\|D\|_\infty\) shows that its value and its square grow at most polynomially in \(\beta,s\) on the bad event. Thus (FACE-MEAN-COMPARISON), the true fourth moment and the true bad-boundary probability bound the \(L^2\) difference between \(\mathbb E(F\mid\mathcal F_s)\) and the sum of these inner Gaussian rows by
\[
 C S^4[g s^{44}P^5+\mathrm{poly}(\beta,S)e^{-cP^2}].
 \tag{INNER-FACE-ERROR}
\]
Only a fixed-degree polynomial occurs here; \(P=\log\beta\). This uses the actual full Wilson average. No independence of those errors is assumed.

Inside the outer canonical comparison window of §4.69 let \(B\) include its real link logarithms in canonical units, \(\|B\|_\infty\le T_S=C S^8P\). The inner boundary-tree words have length at most \(Cs\). Taylor expansion of their group products and logarithms gives
\[
 \|D_{\rm actual}-D_{\rm lin}\|_\infty\le C g s^2 T_S^2,\qquad
 \|D_{\rm actual}\|_\infty+\|D_{\rm lin}\|_\infty\le C s T_S ,
\]
where \(D_{\rm lin}\) is their true signed linear path sum in \(B\). These estimates follow by multiplying the exponentials on their common \(g s T_S\ll1\) ball; the second word derivative costs at most the number of ordered pairs of its factors. In a single squared harmonic force the associated error is at most \(C g s^{15}T_S^3\), since each boundary-to-root linear operator has norm at most \(C s^6\) from sup norm to a single root. The Gaussian traces stay unchanged. Summed over this outer box the difference from the true **outer Gaussian** conditional polynomial \(\mathcal M_G(B)=\mathbb E_G(F^G\mid\text{inner skeleton})\) is at most \(C g S^{43}P^3\). Here \(F^G\) is the linearized ordinary quadratic mark in the outer cell. The compatible tree ensures the observed skeleton coordinates are actual linear observations of that Gaussian; replacing them by independent boundary samples would give a different quantity.

We next bound the variance of this polynomial at fixed good outer boundary \(D_S\). Represent the outer Gaussian free coordinates as \(E D_S+C_S^{1/2}Z\), \(Z\) standard normal. The quadratic matrix \(A\) of \(F^G\) in \(Z\) has operator norm bounded by \(C_N\): each \(H_i C_S^{1/2}\) is bounded because \(C_S\) is the inverse of \(\tau d^*d\) on free coordinates, \(d_i\) restricts \(d\), and \(d_i^*\) has bounded incidence norm. Multiplication by the marks has norm at most one. Its linear coefficient has squared norm at most \(C_N\sum_{b,i}|(H_iE D_S)_b|^2\), with the sum over free marked bonds. Project \(Z\) onto the subspace determined by the retained inner degrees. Its rank is at most \(C_N S^4/s\), the number of inner face links times the fixed color dimension. The exact variance of the retained quadratic is twice the squared Hilbert–Schmidt norm of its projected quadratic matrix plus the squared norm of its projected linear coefficient. Therefore
\[
 \operatorname{Var}_G\mathcal M_G(B)
   \le C_N S^4/s+
             C_N\sum_{p\subset\partial B_S}|(d_\partial D_S)_p|^2
\]
by HARMONIC-FACE-FORCE. The latter term has true good-exterior expectation at most \(C_N S^3\).

Finally center at the outer Gaussian mean of \(\mathcal M_G\), a function of \(D_S\). On the good outer boundary and its canonical window the normalized actual Wilson density is bounded by twice the corresponding Gaussian density by §4.69. Thus the expected square of the centered polynomial there costs at most twice the displayed Gaussian variance, rather than the square of its extensive identity value. On its complement at good outer boundary the conditional compact probability is \(O(e^{-cP^2})\) and the polynomial absolute bounds in \(\beta,S\) suffice, choosing bounded canonical branches if necessary. On a bad outer boundary compare to zero; the true fourth moment of the local sum and its marked bad-boundary probability again absorb its contribution. The squared error from (INNER-FACE-ERROR) and the word comparison is at most \(C S^4/s\) on this range: in particular \(g^2 S^4s^{89}P^{10}\) and \(g^2 S^{82}sP^6\) are bounded. The conditional variance is no larger than the squared error about this chosen outer center. Integrating gives \(C_N S^4/s\) per outer box. Its complete positive conditional law is independent of the other outer interiors. Summing proves NESTED-FACE-INNOVATION.

With the first innovation from §4.68 the exact identity is
\[
 \operatorname{Var}(r_f)=
 \mathbb E\operatorname{Var}(r_f\mid\mathcal F_s)
 +\mathbb E\operatorname{Var}(\mathbb E[r_f\mid\mathcal F_s]\mid\mathcal F_S)
 +\operatorname{Var}(\mathbb E[r_f\mid\mathcal F_S]).
\]
The first term is extensive, the second is smaller by \(1/s\) for the comb on the stated increasing scales, and the final term is retained explicitly.

### 4.72 Pointwise decay from the retained faces and concentration of the spectral exceptions (P)

There is a pointwise strengthening of the doubled-cell estimate for boxes with comparable sides. Write \(d_b\) for the distance of a free bond to the boundary in lattice units. For fixed \(p_0\ge1\), the actual Wilson face row of §4.69 obeys
\[
 \|\mathbb E[r_b\mid\mathcal F_s]-m_b^G(0)\|_{L^{p_0}}
 \le \frac{C_{N,p_0}}{(1+d_b)^2}
       + C_{N,p_0}\,[g s^{44}P^5+\mathrm{poly}(\beta,s)e^{-c_{p_0}P^2}]
 \tag{FACE-DEPTH-ROW}
\]
on the same increasing scales. All constants are independent of the torus side and the position of the box. This gives a quantitative full-law spectral consequence even though the zero momentum remains unresolved.

For details, on the relative doubled torus \(d^*\widetilde F=0\) implies
\(\nabla_\mu\widetilde F=\nabla_\mu\Delta^{-1}d^*(d\widetilde F)\), with the zero mode omitted; a constant harmonic component is killed by \(\nabla_\mu\). The matrix kernels of these multipliers obey
\[
 |K(x)|\le C[(1+|x|_{\rm per})^{-4}+s^{-4}] .
\]
To verify the bound, at nonzero momentum their symbols are products of two forward or backward difference factors divided by \(\sum_j|e^{ip_j}-1|^2\), up to fixed cell phases and shifts. A smooth dyadic cutoff at frequency \(\rho\) has symbols with derivative order \(a\) bounded by \(C_a\rho^{-a}\) on its annulus (use a fixed smooth periodic cutoff at the top annulus). Integrating their continuous torus Fourier coefficients by parts \(J>4\) times gives \(C_J\rho^4(1+\rho|x|)^{-J}\). Discrete Fourier sampling periodizes these coefficients over the doubled side lengths. For \(\rho s\ge c\), the copies beyond the nearest images have total bound \(C_J\rho^4(\rho s)^{-J}\) using comparable sides. The lowest frequencies \(O(1/s)\) contain only a bounded number of discrete modes and cost \(Cs^{-4}\). Summing the dyadic annuli proves the displayed kernel estimate. This elementary argument uses only the flat periodic lattice and includes the corners and the finite number of reflected images.

As in §4.70, \(d\widetilde F\) is a signed sum of the boundary curvature values with bounded multiplicity, supported one lattice step from the faces. A face of dimension three contributes at most \(C/(1+d_b)\) to the sum of the absolute kernel at \(b\), since \(\sum_{z\in\mathbb Z^3}(1+d_b+|z|)^{-4}\le C/(1+d_b)\). The constant term \(s^{-4}\) on \(O(s^3)\) boundary plaquettes has the same bound. On the actual good gauge-fixed boundary \(\|1_{\rm good}(d_\partial D)_p\|_{L^{2p_0}}\le C_{p_0}\) per plaquette, from its short logarithmic expansion, MARKED-EXP and \(g s^4P^2\ll1\). Minkowski's inequality thus gives \(\|1_{\rm good}(H_i E D)_b\|_{2p_0}\le C_{p_0}/(1+d_b)\). Square, use FACE-MEAN-COMPARISON, and bound the bad boundary by the full higher moment and its superpolynomial probability. This proves FACE-DEPTH-ROW.

Consequently, on a comparable-side compatible grid,
\[
 \operatorname{Tr}\operatorname{Cov}\bigl(
       (\mathbb E[r_b\mid\mathcal F_s])_{b\in\mathcal C}\bigr)
        \le C_N n^4/s .
 \tag{RETAINED-SPECTRAL-TRACE}
\]
Indeed each distance layer in a box has at most \(C s^3\) marked roots, and \(\sum_{z\ge0}(1+z)^{-4}\) is finite. The squared local error summed over \(O(s^4)\) roots still costs \(O(s^3)\) on the specified growing scales. The trace is the sum of the true nonnegative ordinary variances; it is not an assertion about their off-diagonal signs.

Use the orthonormal Fourier basis of the comb lattice, all times and spatial sublattice of step two. The full comb covariance is translation invariant on this lattice. Its quadratic form equals the averaged conditional covariance plus the positive retained covariance. By FOUR-DIMENSIONAL-BOX-INNOVATION the first operator has norm at most \(C_N\), for all marks and also for the complex Fourier basis by taking real and imaginary parts. Summing the diagonal matrix elements of the retained positive operator in this basis gives exactly (RETAINED-SPECTRAL-TRACE), without requiring translation covariance of the chosen face grid. Thus the fraction of comb frequencies with structure factor exceeding \(C_N+\epsilon\) is bounded by
\[
 \frac{C_N'}{\epsilon s}.
 \tag{VANISHING-EXCEPTIONAL-FRACTION}
\]
On the full lattice, each oriented structure factor is at most eight times the corresponding aliased comb factor by positivity of every term in the alias identity of §4.32. Each comb frequency has eight antecedents, preserving the fractional count. Permuting axes and using \(\|K(p)\|_{\rm op}\le\sum_\nu K_{\nu\nu}(p)\) for the positive orientation matrix gives the same vanishing-fraction statement, with a fixed threshold enlarged by these finite factors, for all lattice momentum bins. Compatible partitions of comparable even cell widths below the given bound can be chosen on large even sides without requiring \(s\) to divide \(n\), by distributing the even lengths between neighboring separators. Along the trajectory choose \(s\) growing below \(\beta^{1/200}\). This proves a common finite susceptibility threshold outside a vanishing fraction of bins, including bins close to coordinate planes. A fraction bound allows the single comb zero mode to remain exceptional, and so does not prove full SUS.

### 4.73 An absolutely summable part of the actual periodic zero-mode sum (P)

The zero-frequency comb needs the signed covariance sum over **all separations**. There is a stronger direct estimate for its off-diagonal terms out to a growing lattice scale. Write \(d=d_{\rm per,\infty}(x,y)\) in fine sites for two bonds of the same temporal comb, and \(L_\beta=\lfloor c\,\beta^{1/200}\rfloor\), taking the smaller compatible geometric sizes when necessary. Under the hypotheses of §§4.68–4.69,
\[
 |\operatorname{Cov}_{\mu_\beta}(r_x,r_y)|
       \le C_N[1+\min(d,L_\beta)]^{-14/3} .
 \tag{ZERO-MODE-PAIR}
\]
In particular the diagonal and every signed or unsigned off-diagonal term of the actual zero-mode sum with \(d\le L_\beta\) have a uniformly bounded sum per anchor. This improves the estimate on the specified zero mode itself; it still leaves separations beyond this increasing scale.

**A thin Wilson rectangle on the finite torus.** Normalize its fundamental Wilson expectation by \(W(l,1)=N^{-1}\mathbb E\operatorname{Re}\operatorname{Tr}U_{\rm rect}\) for a rectangle of length \(l<n\) and width one. Then
\[
 W(l,1)\ge W(1,1)^l .
 \tag{THIN-RECTANGLE}
\]
Here is the finite-volume transfer check, in the setting of the reflection-positive Wilson loop inequality of [Bachas, *Convexity of the Quarkonium Potential*](https://www.slac.stanford.edu/pubs/slacpubs/3750/slac-pub-3814.pdf). Use the length direction as transfer time and the single fixed spatial bond from \(x_0\) to \(y_0\) as the open path. Multiplication by \(U_{x_0y_0}/\sqrt N\) is an isometry \(O\) from invariant scalar slice functions into matrix-valued slice functions transforming by the fundamental endpoint rotations \(g_{x_0}\,\cdot\,g_{y_0}^{-1}\); use the matrix Hilbert–Schmidt inner product. Gauge averaging combined with these endpoint matrix rotations is an orthogonal projector \(\mathcal P_{xy}\). It commutes with the positive unprojected kinetic convolution and the invariant spatial potential. Thus the transfer \(T_c=V^{1/2}K_\beta\mathcal P_{xy}V^{1/2}\) in this charged sector is positive by the same character expansion as in §4.29. The transverse spatial slices have the same periodic convention as the original Wilson law.

Inserting the two endpoint projections in the ordinary transfer integral, the site gauge rotations on the two propagated color indices multiply along the two temporal sides. The open spatial path at each end closes the normalized fundamental trace. This gives
\[
 W(l,1)=\frac{\operatorname{Tr}(T^{n-l}O^* T_c^l O)}
                      {\operatorname{Tr}T^n}.
\]
There is no long-time limit here. Expand both positive compact transfers spectrally, with eigenvalues \(\lambda_i\) of \(T\) on the physical sector and \(\mu_j\) of \(T_c\) on its charged sector. For \(l<n\), zero \(\lambda_i\) terms vanish. The weights \(\lambda_i^n|\langle j,O i\rangle|^2/\operatorname{Tr}T^n\) sum to one, and the trace is the \(l\)-th moment of the nonnegative numbers \(\mu_j/\lambda_i\) with those weights. Its first moment is \(W(1,1)\). Jensen's inequality proves (THIN-RECTANGLE).

Since FIRST bounds \(1-W(1,1)\le C_N/\beta\), it follows that
\[
 \|\sqrt\beta\,(U_{\rm rect}-I)\|_{L^2({\rm HS})}\le C_N\sqrt l .
\]
On the other hand a thin rectangle is the product of \(l\) conjugated elementary plaquettes. The marked single-plaquette moments and Minkowski give \(\|\sqrt\beta\,(U_{\rm rect}-I)\|_{L^8({\rm HS})}\le C_N l\). Interpolation yields the \(L^4\) bound \(C_N l^{5/6}\), without any independence assumption for neighboring plaquettes.

**A representative for the deep conditional mean.** In the *whole* box take the coordinate path from its root corner to a vertex, moving through the coordinates in a fixed order, and set this path tree to identity. Every chord loop is a product, up to unitary conjugations, of at most three width-one rectangular loops of length at most \(s\). Indeed commute its single extra coordinate step past each later coordinate run in the root path; commuting past a whole straight run produces one such rectangle. For boundary links in this representative, choose bounded traceless real logarithms agreeing with the small chart at identity. Their norm is at most a fixed multiple of the group chord distance globally (by compactness away from identity). The resulting canonical boundary fields therefore satisfy
\[
 \|D_e\|_{L^4(\mu_\beta)}\le C_N s^{5/6}.
 \tag{THIN-TREE-BOUNDARY}
\]

This gauge can depend on interior links; we use it to estimate a scalar, not to alter what is conditioned on. For each actual field, the conditional mean on its fixed face data is invariant under every boundary site gauge, by changing variables in the full compact conditional integral. Thus at that field we may evaluate it on the boundary representative just constructed. The box Laplace comparison still holds on \(\|D\|_\infty\le C s^2P\), even when its boundary tree links are not exactly identity. Freeze those boundary values and fix only the same based interior forest as in §4.68. The linear coercivity is unchanged since the boundary *variations* are zero. For the compact tail, a free chord is a product of a tree-path loop of at most \(C s^2\) plaquette defects and a boundary path of length \(C s\). The latter deviates from identity by at most \(C g s^3P\ll gT\) on this event. Thus a free chord outside \(gT\) again forces a plaquette defect \(\ge c gT/s^2\), exactly as in §4.69. All other comparisons use the explicit boundary extension by zero and need no identity assumption on its tree. The Gaussian trace with the boundary frozen is independent of its representative at zero data. The true probability of failing this boundary-size condition is superpolynomial in \(\beta\), because the full coordinate tree uses only the thin strips already controlled by the original marked plaquette tail. Full-law higher moments of the invariant conditional scalar control its contribution there.

**One derivative tangential to each face.** For a bond at distance at least \(c s\) from every face the doubled kernel of §4.72, as a linear map from \(d_\partial D\), has modulus at most \(C s^{-4}\). Its first difference in a direction tangent to a face has modulus at most \(C s^{-5}\). For the latter, the same frequency proof inserts one forward-difference factor on each annulus, gaining \(\rho\); the lowest frequencies now cost \(C s^{-5}\). On each fixed face and orientation the coefficients of the boundary plaquettes have these bounds. More explicitly \(d\widetilde F\) is a signed sum of the omitted boundary values on their incident three-cells. Along a face its reflected locations and signs are fixed translates or reflected translates, so the tangential difference bound applies; only the face's finite edges can terminate an incidence pattern.

Write each boundary curvature component as the oriented sum of its four link logs and sum by parts **on that face**. For its interior edge positions the two opposing plaquettes supply a first difference of the kernel, at most \(C s^{-5}\). At its ridges use \(C s^{-4}\) without subtraction. There are \(O(s^3)\) face positions and \(O(s^2)\) ridge positions, counting each of the finitely many faces and orientations. The total absolute coefficient on the boundary *link* field is therefore at most \(C s^{-2}\). With THIN-TREE-BOUNDARY this gives
\(\|1_{\rm good}(H_i E D)_b\|_4\le C s^{-7/6}\). FACE-MEAN-COMPARISON and the bad-event bound imply
\[
 \|\mathbb E(r_b\mid\mathcal F_s)-m_b^G(0)\|_2\le C_N s^{-7/3}
 \quad\text{when } d(b,\partial B)\ge c s,\ s\le\beta^{1/200}.
 \tag{DEEP-FACE-ORDINARY}
\]
Indeed \(g s^{44}P^5\le C s^{-7/3}\) on this range at weak coupling.

For \(d\) larger than a fixed constant choose comparable even box widths of order \(s=\min(d/C_0,L_\beta)\), with \(C_0\) large. Translate the partition so that both marked bonds are at distance at least \(c s\) from each face. Such a translation exists: for a random translation preserving the spatial parity class, the fraction of sites within \(c s\) of a face in one coordinate is at most \(C c+O(1/s)\); take the union bound over the two sites and four coordinates. The maximal-coordinate separation then puts the bonds in different cells. Their exact conditional covariance given the entire face data vanishes by compact cell independence. The full covariance thus equals that of their conditional means on those faces. Apply Cauchy–Schwarz and (DEEP-FACE-ORDINARY); for bounded \(d\) use the fixed Wilson moments. This proves (ZERO-MODE-PAIR). No sign of the separated covariance has been presumed. In four dimensions \(\sum_{d\ge1}d^3(1+d)^{-14/3}<\infty\). Consequently only the genuinely longer-range sum must be paid for the zero mode:
\[
 \frac{\operatorname{Var}(r_{\rm comb})}{|\mathcal C|}
 =O(1)+\frac1{|\mathcal C|}\!
       \sum_{\substack{x,y\in\mathcal C\\ d(x,y)>L_\beta}}
                   \operatorname{Cov}(r_x,r_y).
 \tag{ZERO-MODE-LONG-TAIL}
\]
The available absolute bound on this last part is at most \(C n^4 L_\beta^{-14/3}\) per anchor. This is an improved but nonuniform upper bound; none of the trace or almost-every-frequency results replaces the signed long-tail estimate. On the exact Wilson measure there is also a complete finite-size regime: if the whole even torus side is at most \(c\beta^{1/200}\) under the marked-moment hypotheses, every separation is covered by (ZERO-MODE-PAIR). The signed comb row is then uniformly summable and EIGHT-SITE-COMB gives \(\operatorname{Var}(r_f)\le C_N M_f\) for arbitrary marks. The stipulated asymptotically free fixed-volume trajectory has \(n\) exponentially larger than this scale, so this corollary does not remove its distant tail.

### 4.74 The finite signed contribution to the original zero mode (P)

The bounded term in ZERO-MODE-LONG-TAIL has a limit fixed by the actual Wilson law. Let \(P_{\rm curl}\) be the orthogonal projection in \(\ell^2\) of two-cochains on the infinite unit cubic lattice onto the closure of curls of compactly supported one-cochains. Let \(\psi_{bi}\) be the signed two-plaquette vector implementing the derivative at bond \(b\) for matching \(i\), so \((H_i A)_b=\langle\psi_{bi},dA\rangle\). Define
\[
 C_G(y)=2d_G\tau^2\sum_{i,j}
                  |\langle\psi_{0i},P_{\rm curl}\psi_{yj}\rangle|^2,
 \qquad
 \chi_G^{\mathcal C}=\sum_{y\in\mathbb Z\times(2\mathbb Z)^3} C_G(y).
 \tag{GAUSSIAN-COMB-CONSTANT}
\]
The origin signifies the temporal bond based there. The sum is finite and positive. On the fixed reference trajectory, with the same \(L_\beta\) as §4.73, translation invariance on the comb gives the **signed** identity with asymptotic evaluation
\[
 \frac{\operatorname{Var}_{\mu_\beta}(r_{\rm comb})}{|\mathcal C|}
  =\chi_G^{\mathcal C}+
       \sum_{d(0,y)>L_\beta}\operatorname{Cov}_{\mu_\beta}(r_0,r_y)
       +o(1).
 \tag{SIGNED-ZERO-SPLIT}
\]
Moreover the liminf of the displayed signed long-distance sum is nonnegative. An upper bound on that sum is still required.

For each fixed displacement \(y\), place the two temporal bonds in the deep interior of the same increasing box of side \(s\) comparable to a sufficiently small multiple of \(\beta^{1/200}\). This can be done with both roots far from all faces, and \(s\ll n\) on the weak reference trajectory. The conditional compact law depends on the outside only through these faces. On the good boundary its covariance agrees, up to \(o(1)\) after averaging, with that of the ordinary quadratic marks on the Dirichlet Gaussian with its actual harmonic boundary shift. Indeed on the canonical box window the relative density error is \(O(g s^{28}P^3)\), the product of two quadratic marks is \(O(1+T^4)\), and the individual insertion Taylor errors are \(O(gT^3)\). Thus the two-moment error and the centered product error are bounded by \(C g s^{60}P^7=o(1)\), plus the superpolynomial tails as in §4.69. On the bad exterior use the actual higher moments of the two insertions, conditional Jensen, and the boundary tail; the Gaussian zero-boundary comparison is bounded there. The noncentral quadratic covariance terms vanish after averaging: they contain a product of the two harmonic force means, with a bounded Gaussian covariance, and their \(L^4\) norms tend to zero by the deep boundary estimate of §4.73. The covariance of the two conditional means also tends to zero by DEEP-FACE-ORDINARY. All of these comparisons may be made in the full coordinate-tree representative for the invariant scalar, as justified there.

In the centered flat Gaussian, the curvature covariance equals \(\tau^{-1}P_B\), with \(P_B\) the projection onto curls of interior variations vanishing tangentially at the boundary. This follows directly from the canonical Gaussian density \(\exp(-\tau\|dA\|^2/2)\) on the injective tree-fixed coordinates. The gauge-fixed curvature space equals that from all free interior variations. Zero extension to the infinite lattice gives exactly that subspace, since exterior plaquettes contain no free edges. For increasing boxes with the two roots deep, \(P_B\psi\to P_{\rm curl}\psi\) in norm for each fixed local \(\psi\): every fixed compactly supported potential is eventually among the interior variations, and \(P_B\) projects into \(\operatorname{ran}P_{\rm curl}\). Approximate \(P_{\rm curl}\psi\) by such curls to bound the distance to \(\operatorname{ran}P_B\). Wick's formula for the two matched squared forces now gives \(\operatorname{Cov}_{\mu_\beta}(r_0,r_y)\to C_G(y)\) at each fixed displacement.

For \(d\le L_\beta\), ZERO-MODE-PAIR gives the summable majorant \(C(1+d)^{-14/3}\) independent of cutoff. Periodically unfold the fixed growing neighborhood about the origin. Dominated convergence proves that its **actual signed** sum tends to \(\chi_G^{\mathcal C}\), and also proves absolute finiteness of that constant. Its positivity follows already from the \(y=0\) diagonal summand: at least one two-plaquette test has nonzero overlap with a compact curl, as seen by testing a single edge in its plane. This proves (SIGNED-ZERO-SPLIT).

For the last assertion recall that the comb structure factor attains its maximum at zero (§§4.29–4.32). Therefore for every finite cube \(B_m\) in the comb lattice,
\[
 \frac{\operatorname{Var}(r_{\rm comb})}{|\mathcal C|}
 \ge |B_m|^{-1}\operatorname{Var}\!\left(\sum_{x\in B_m}r_x\right).
\]
This is Parseval's inequality with the maximum structure factor. At fixed \(m\) the right side tends to the corresponding Gaussian covariance sum by the fixed-displacement result. Its limit as \(m\to\infty\) is \(\chi_G^{\mathcal C}\) by absolute summability and the ordinary cube overlap weights. Take the liminf first in the mesh and then in \(m\) to obtain \(\liminf \operatorname{Var}(r_{\rm comb})/|\mathcal C|\ge\chi_G^{\mathcal C}\). The nonnegative liminf of the signed tail follows from (SIGNED-ZERO-SPLIT). This establishes the short- and intermediate-distance contribution including its signs and specifies exactly where a possible excess of the zero mode can reside.

### 4.75 The real pressure of the literal periodic zero mode (P)

There is a thermodynamic statement for the genuine unamplified source, including the ordinary version. Put \(V=n^4\), \(Y^h=\sum_{b\in\mathcal C}h_b\), \(Y^r=\sum_{b\in\mathcal C}r_b\). For \(Y=Y^h\) or \(Y^r\), there is \(t_0>0\) independent of the ultraviolet mesh such that, locally uniformly on the **real** interval \((-t_0,t_0)\),
\[
 p_a^Y(t):=V^{-1}\log\mathbb E_{\mu_\beta}e^{tY}
       \longrightarrow p_G^Y(t).
 \tag{REAL-ZERO-PRESSURE}
\]
The limit is the pressure per fine site of the periodic comb in the infinite unit-lattice Gaussian curl field, analytic on that neighborhood. For \(r\) it includes its exact Casimir identity per selected link. The convergence uses \(n\to\infty,\ \beta\to\infty\) with room for cells of side \(s\to\infty,\ \log\beta=o(s),\ s\le\beta^{1/200}\), as on the reference trajectory. This is a pressure statement at the actual constant mask on the full compact Wilson measure.

**Positive local groups for the real tilt.** A selected temporal bond's six incident plaquettes form a disjoint group of plaquettes as \(b\) ranges over the comb. Write \(e_b=\sum_{p\ni b}s_p\) and \(d_b=h_b/\beta\). For the \(h\) source the tilted action on such a group is \(e_b-t d_b\), in Wilson action units. For \(r\), use \(\ell_b=C_F(6N-e_b)\), remove the deterministic source contribution \(-2NC_F t|\mathcal C|\) from the logarithm of the partition function, and use \(e_b-t[D_b+(C_F/(3\beta))e_b]\) on the group. The remaining individual plaquettes have action \(s_p\). Since \(0\le d_b\le D_b\le C_N e_b\), each group is nonnegative and is at least \(e_b/2\) for \(|t|\le t_0\) with \(t_0\) small enough and \(\beta\ge1\). In particular we may delete whole groups for an upper partition bound, for either sign of the real source. The ordinary identity is put back exactly at the end.

Take disjoint rectangular vertex cubes of comparable side \(s\) separated by corridors of one or two lattice spacings, with spatial boundary coordinates odd. Such cubes cover all but \(O(V/s)\) sites and links on sufficiently large even tori, by distributing even interval lengths of order \(s\) between the gaps in each coordinate. If a temporal plaquette in a cube belongs to a selected group, its marked temporal edge is strictly inside all its spatial faces. Its whole six-plaquette group therefore belongs to the cube. Time edges are normal to time faces. Thus the reduced action within a cube comprises precisely its complete plaquette action and the actual restricted comb; there is no partial charged group needing a sign estimate.

Let \(Z_{\rm red}(t)\) denote the unnormalized full tilted integral with the above deterministic identity removed, and \(Z_{B,\rm free}(t),Z_{B,D}(t)\) denote the corresponding cube integrals with respectively all links free or boundary tangential links fixed to identity. Deleting all nonnegative terms outside the disjoint cubes gives the upper bound \(\prod_B Z_{B,\rm free}(t)\). For the lower bound restrict every boundary and corridor link outside the nonboundary cube interiors to a Haar ball of radius \(\beta^{-2}\) about identity. There are \(O(V/s)\) such links. Changing the fixed boundary links back to identity in the cube costs at most \(C_N\beta^{-1}\) per changed link in the exponent, uniformly in the compact interiors: every group is a bounded-degree smooth function on its fixed stencil. All remaining terms involve only restricted links, since every plaquette touching a nonboundary link lies in the same cube. They cost at most \(C_N\beta^{-1}\) per such link as well. The Haar balls give the logarithmic cost \(C_N(V/s)\log\beta\). Hence
\[
 e^{-C_N(V/s)(1+\log\beta)}\prod_B Z_{B,D}(t)
       \le Z_{\rm red}(t)\le \prod_B Z_{B,\rm free}(t).
 \tag{REAL-ZERO-BRACKETS}
\]

**Uniform evaluation of the bracket gap.** Use one tree in each cube, first a boundary spanning tree and then the attached interior forest. For the free integral tree fixing leaves all free chords including the boundary non-tree ones. For the Dirichlet integral the latter are fixed at zero in its flat log chart; the interior forest is precisely its permitted based gauge. The same \(O(s)\) path lengths and \(O(s^2)\) fillings as §4.68 apply. The flat quadratic tilted precision lies between fixed multiples of the Wilson precision for both brackets. Indeed the positive group action bound holds under scaling every fine link to identity, and its Hessian upper bound follows from the same fixed quadratic source. Exactly as in §4.69 with zero boundary and \(T=C s^8\log\beta\), the ratio of each original cube integral to its Gaussian integral with the common leading Haar and \(g\)-normalization is \(1+O_N(g s^{28}(\log\beta)^3+\mathrm{poly}(\beta,s)e^{-c_N(\log\beta)^2})\), uniformly on the real interval. The local cubic and higher derivatives have uniform coefficients for \(|t|\le t_0\); the full compact tail still uses \(S_{\rm red}\ge S/2\). In the ordinary case its small field-dependent Casimir term changes the relative Gaussian precision by \(O_N(1/\beta)\) in Wilson quadratic-form units, at most \(C_Ns^4/\beta\) in the log Gaussian integral. This term vanishes per fine site in the limit.

The reduced Gaussian free and Dirichlet brackets differ only by integrating the \(O(s^3)\) additional boundary chords. In the tree coordinates all eigenvalues of the free precision are between \(c_Ns^{-8}\) and \(C_N\), by the same filling bound; this applies also to the small relative tilts. Its boundary Schur complement has the same interval, by minimizing the quadratic form over the free interior (use zero interior as the upper trial). The extra \(g\) and leading Haar factors and the Gaussian determinant therefore cost at most \(C_N s^3(1+\log\beta+\log s)\) in logarithm per cube. This comparison keeps the tree-gauge constants and counts only the additional independent coordinates. Using the same disjoint cubes for both bounds avoids a mismatch of bulk vacuum constants. In particular,
\[
 p_a^Y(t)
 =\frac1V\sum_B \log\frac{Z_{B,D}^{G,Y}(t)}{Z_{B,D}^{G}(0)}
       +o(1)
\]
uniformly on any smaller real interval, when \(s\to\infty\) with \(\log\beta=o(s)\) in the allowed range. In this formula the ordinary Gaussian integrals include their identity subtraction on each cube; the omitted corridor fraction \(O(1/s)\) of that fixed source scalar is included in the error. One can take an even \(s\) comparable to \(\beta^{1/200}\).

**Identification of the limit.** On Dirichlet Gaussian curvature the covariance is \(\tau^{-1}P_B\) as in §4.74. The \(h\) quadratic form in the curl field counts the matching differences, and the ordinary positive part counts the three matching forces; both are uniformly bounded positive finite-range operators with the same fixed-period comb coefficient. Denote their conjugates by the square root covariance on the curl space by \(K_B^Y\), with the convention \(Y^G=Z^TK_B^Y Z+c_B^Y\) for a standard real Gaussian. Then the log integral ratio is \(t c_B^Y+\frac12\sum_{m\ge1}(2t)^m\operatorname{Tr}[(K_B^Y)^m]/m\). All \(\|K_B^Y\|\) are bounded by the same constant, and the trace per site of each fixed power converges to the corresponding trace per site of the infinite periodic comb operator with \(P_{\rm curl}\). To check this last fact, extend the cube kernels by zero and move a marked period cell to the origin. Along every sequence of roots escaping all boundaries, the translated \(P_B\)'s converge strongly to \(P_{\rm curl}\) by the compact-curl argument of §4.74. The finite-range masked matching operators converge on compact supports to the corresponding periodic operators along each period class. Boundedness gives the same result for their fixed products and their diagonal matrix elements. The proportion of roots within any fixed distance of the boundary tends to zero, and the finitely many period classes have their correct limiting proportions. This proves trace convergence without assuming periodicity of a single Dirichlet cube. Dominated convergence in the geometric trace series gives \(p_G^Y\) and proves REAL-ZERO-PRESSURE.

Several implications concern the zero-frequency variable itself. Convexity and differentiability of this real limit imply \((p_a^Y)'(t)\to (p_G^Y)'(t)\) pointwise in the interval (and uniformly on compact subintervals by monotonicity and continuity). The positive measures
\[
 (p_a^Y)''(t)\,dt=V^{-1}\operatorname{Var}_{\mu_{\beta,t}}(Y)\,dt
    \ \Longrightarrow\ (p_G^Y)''(t)\,dt
 \tag{AVERAGED-ZERO-SUSCEPTIBILITY}
\]
converge weakly on compact subintervals, by distributional differentiation and positivity. Here \(\mu_{\beta,t}\) is the true normalized law tilted by its named \(Y\). In particular the limiting pressure has no first-derivative jump at the original source \(t=0\). For any fixed \(\epsilon>0\) the unperturbed mean density also satisfies
\(\mathbb P_\beta(|Y/V-(p_G^Y)'(0)|>\epsilon)\le 2e^{-c_\epsilon V}\) for sufficiently fine meshes, by the two real Chernoff bounds and strict directional separation at zero. These are full-law statements even when some local conditional sources have zeros tending to zero as in §4.57.

The weak convergence of second derivatives does not give their value at a prescribed point. A positive variance spike of narrowing source width at \(t=0\) has not been excluded by these real brackets. Likewise the disappearance of macroscopic coexistence still permits deviations on scales strictly between \(\sqrt V\) and \(V\). An upper bound on the last signed sum of (SIGNED-ZERO-SPLIT), or a bound on the original zero-source second derivative itself, remains necessary for SUS.

### 4.76 Severe compact exteriors and large energetic components in the actual zero mode (P)

The conditional single-link obstruction can occur simultaneously on the **entire periodic mask**. In §4.57 take all spatial links to be identity. For each time layer set every temporal link at a spatial site with precisely one odd coordinate \(i\) to the same \(V_i\) used there; the remaining exterior temporal links may be identity. Each selected site then has the two staples \(V_i,V_i\) in each direction and \(K=0\). The conditional law is exactly a product of Haar measures over all selected spins. For \(SU(2)\) its ordinary constant-mode variance divided by \(|\mathcal C|\) is \((24v^2\beta)^2/12\), and its generating function has the displayed zeros of order \(\beta^{-1}\). This is a full-mask example in a genuine compact Wilson conditional fiber. It is not a counterexample for the full Wilson marginal.

In fact a sufficiently severe part of that exterior can be excluded from the **unconditioned** zero-mode variance under an explicit trajectory inequality. On a torus with \(4\mid n\), the \(1\times2\times2\times2\) comb cells form the even native reflection tiling of §4.38. Distinct marked \(b\)'s have disjoint sets of incident plaquettes, although some spatial links are shared. For every \(0<t<1\) the chessboard estimate and the real Wilson partition comparison give
\[
 \mathbb E_{\mu_\beta}\exp\left(t\beta\sum_{b\in A}e_b\right)
              \le e^{C_t |A|},\qquad A\subset\mathcal C .
 \tag{SHARP-COMB-STAR-MOMENT}
\]
Indeed the six-plaquette energy \(e_b\) is in its closed cell and reflected copies disseminate to precisely the selected six-plaquette stars. Their sum is at most \(S\) by disjointness. The full single-star replica is bounded by \(Z_{(1-t)\beta}/Z_\beta\), whose log is at most \(C'_t n^4\) under the tree and temporal-forest bounds of §4.11 with the stated trajectory growth condition. Each chessboard root takes the \(1/|\mathcal C|\) power, proving the inequality. The rate \(t\) can approach one because there is no sixteenfold overlap cost for these stars.

Let \(\lambda_0=\liminf \beta/\log n>0\). If \(X_b\) is any quantity with \(|X_b|\le C\beta\,1_{\{e_b\ge E_0\}}\) and \(E_0\lambda_0>2\), then
\[
 \frac1{|\mathcal C|}\mathbb E\left|\sum_{b\in\mathcal C}X_b\right|^2
                              \longrightarrow0 .
 \tag{SEVERE-ZERO-REMOVAL}
\]
Choose \(t<1\) with \(t E_0\lambda_0>2\). Markov's inequality with (SHARP-COMB-STAR-MOMENT) gives the bounds \(e^{C_t-t\beta E_0}\) and \(e^{2C_t-2t\beta E_0}\) for one and two distinct required stars. The squared sum divided by \(|\mathcal C|\) is therefore bounded by \(C'\beta^2[e^{-t\beta E_0}+n^4e^{-2t\beta E_0}]\). The strict trajectory inequality makes this vanish. If \(\beta/\log n\) grows without bound, the same conclusion follows directly from the exponential. The estimate includes all signed off-diagonal contributions in this severe part and needs no correlation assumption. In particular its variance seminorm is \(o(\sqrt{|\mathcal C|})\), so removal preserves boundedness or unboundedness of the normalized full zero-mode variance.

For the compact heatbath degeneracy, \(e_b=6N-\operatorname{Re}\operatorname{Tr}(u^\dagger K)\ge6N-\sqrt N\|K\|_{\rm HS}\) on every real spin. Consequently the conclusion applies to \(r_b\), \(h_b\), or the bounded heatbath mean \(m_b\) restricted to a sufficiently small *exterior-measurable* \(\|K\|_{\rm HS}\) event whenever \(6N\lambda_0>2\). In the standard bare Wilson convention this threshold is met on the stated weak trajectory. To make the normalization explicit, the standard action is \((2/g_{\rm std}^2)\sum_p(N-\operatorname{Re}\operatorname{Tr}U_p)\), so \(g_0^2=N g_{\rm std}^2\) for the \(g_0\) of §1 and the coefficient here is \(\beta=2/g_{\rm std}^2\). The one-loop inverse-\(g_{\rm std}^2\) coefficient is \(11N/(24\pi^2)\), equivalently the log coefficient for \(g_{\rm std}^2/(4\pi)\) in [Lüscher and Weisz, eq. (7.1)](https://arxiv.org/pdf/hep-lat/9505011). Using the supplied I-0c real flow rather than a higher perturbative assumption, the sum of the \(O(g_j^2)\) remainders is \(O(\log(2+K))\) at sufficiently weak endpoint by §4.46. Thus \(\lambda_0\ge 11N/(12\pi^2)\) with this action normalization. One may choose
\[
 24\pi^2/(11N)<E_0<6N ,
\]
also for \(SU(2)\). The general result (SEVERE-ZERO-REMOVAL) itself uses only the explicitly displayed slope criterion. It does not erase a bad selected star with a lower action cost merely because it is called large in an RG history.

There is a related removal for large *connected* energetic components on the microscopic comb. Give the comb its nearest-cell graph. Mark a star bad when \(e_b\ge\delta\), or by an exterior condition which implies this inequality. If the bad component containing \(b\) has size at least \(m\), it contains a connected marked witness of exactly \(m\) sites through \(b\) within graph radius \(m-1\). The number of such witnesses is at most \(C_d^m\), by traversing a rooted spanning tree in at most \(2m\) steps. For two sites farther than \(2m\) in this graph their chosen witnesses must be disjoint. For any bounded contributions \(|X_b|\le C\beta\) supported on such large components, the same calculation gives
\[
 \frac1{|\mathcal C|}\mathbb E\left|\sum_{b\in\mathcal C}X_b\right|^2
 \le C\beta^2\big[(1+m)^4 e^{-(t\beta\delta-C_t')m}
            +n^4 e^{-2(t\beta\delta-C_t')m}\big].
 \tag{LARGE-COMB-COMPONENT-REMOVAL}
\]
The first term counts the near pairs by a single witness. The second sums all possibly long-distance pairs using their distinct witnesses. For each fixed \(\delta>0\), a sufficiently large *fixed* \(m\) with \(t\delta m\lambda_0>2\) makes the entire bound vanish. One can also use cutoff-dependent \(\delta,m\) when the displayed right side tends to zero, for example with \(\beta\delta\to\infty\), polynomially bounded \(m,\beta\) in \(\log n\) on the fixed-endpoint trajectory, and \((t\beta\delta-C_t')m\ge(2+\epsilon)\log n\). These are microscopic plaquette-star components, not arbitrary multiscale return records. Isolated moderate components and the long covariance of their surrounding regular fields remain in SIGNED-ZERO-SPLIT.

### 4.77 Stable Gaussian innovation and the positive remainder of the signed zero mode (P)

Take comparable four-dimensional boxes of side \(s\to\infty\), \(s\le\beta^{1/200}\), as in §§4.68–4.69, on the reference trajectory. Put \(M=|\mathcal C|\), \(Y=Y^r\), \(m_s=\mathbb E[Y\mid\mathcal F_s]\). Then the full compact Wilson conditional terms satisfy
\[
 M^{-1}\operatorname{Var}(Y\mid\mathcal F_s)
       \longrightarrow \chi_G^{\mathcal C}\quad\hbox{in }L^1,
 \qquad
 \mathbb E\!\left[\left.e^{it(Y-m_s)/\sqrt M}\right|\mathcal F_s\right]
       \longrightarrow e^{-t^2\chi_G^{\mathcal C}/2}
       \quad\hbox{in }L^1 .
 \tag{STABLE-ZERO-INNOVATION}
\]
Thus the fluctuation integrated inside the boxes has a Gaussian limit even when observed jointly with bounded functions of all the retained Wilson faces: multiplication of the conditional characteristic-function error by any such uniformly bounded function tends to zero in expectation. The face variable itself need not have a limit. In particular the signed residual in (SIGNED-ZERO-SPLIT) has the positive representation
\[
 \sum_{d(0,y)>L_\beta}\operatorname{Cov}_{\mu_\beta}(r_0,r_y)
       =M^{-1}\operatorname{Var}_{\mu_\beta}(m_s)+o(1).
 \tag{POSITIVE-ZERO-LONG-TAIL}
\]
This is an equality for the actual constant mode, with all diagonal and separated signs accounted for.

Here is the conditional variance check. Write \(F_B=\sum_{b\in B\cap\mathcal C}r_b\). At fixed good boundary its Gaussian variance splits into \(2\operatorname{Tr}(A_B^2)\) for the centered quadratic and the squared norm of the noncentral linear coefficient. The latter is at most \(C_N\sum_{p\subset\partial B}|(d_\partial D)_p|^2\) by the operator bound and HARMONIC-FACE-FORCE in §4.71. Its averaged good-boundary contribution is \(O(s^3)\). The centered trace divided by \(|B\cap\mathcal C|\) tends to \(\chi_G^{\mathcal C}\): this is the second Gaussian trace-power convergence in §4.75, or the projection-and-Wick proof of §4.74. It is uniform along any sequence of comparable boxes with side tending to infinity because all period classes have the same limiting proportions and all deep translated projections converge strongly.

On the actual good exterior, compare conditional moments inside the canonical window of §4.69. The sum of the leading quadratic insertions is bounded there by \(C s^4(1+T^2)\); its Taylor error is bounded by \(C g s^4 T^3\). Multiplying its squared sup by the relative density error \(C g s^{28}P^3\), and comparing the insertion squares and the squared means, costs at most \(C g s^{68}P^7\) plus fixed-polynomial times \(e^{-cP^2}\). This is \(o(s^4)\) uniformly at \(s\le\beta^{1/200}\). The conditional compact and Gaussian outside-window errors use the tail bounds already proved there. On the bad exterior the expectation of the actual conditional variance there is at most \((\mathbb E F_B^4)^{1/2}\,\mathbb P({\rm bad})^{1/2}\le C s^8\,\mathrm{poly}(s)e^{-cP^2}\) by the full higher moments. This proves that the \(L^1\) distance between the conditional variance and its centered deterministic Gaussian trace is \(o(s^4)+O(s^3)\) per box. Conditional independence and summation yield the first assertion in (STABLE-ZERO-INNOVATION).

Given \(\mathcal F_s\) the centered box variables \(F_B-\mathbb E(F_B\mid\mathcal F_s)\) are independent. Their full fourth moments are at most \(C s^{16}\) by Jensen and the single-site marked moments. The sum of their conditional fourth moments divided by \(M^2\) tends to zero in \(L^1\), since there are \(O(M/s^4)\) boxes and \(s^{12}/M\to0\) on the reference trajectory. Expanding each conditional characteristic function through second order, the sum of the third absolute errors after scaling by \(M^{-3/2}\) tends to zero in probability by Hölder with the variance and fourth-moment sums. The sum of the squared scaled conditional variances also tends to zero, so taking the product has precisely the Gaussian limit displayed above. Boundedness of characteristic functions upgrades convergence in probability to the stated \(L^1\) convergence. The tower formula for \(Y\), its computed conditional variance and (SIGNED-ZERO-SPLIT) give (POSITIVE-ZERO-LONG-TAIL).

The same calculation applies to any fixed linear combination of \(Y^r,Y^h\). Indeed their face conditional means agree exactly by single-link Haar integration at every selected bond. The heatbath contact of §4.57 shows that in the limiting joint innovation \(Y^r-Y^h\) has variance per comb site \(8\tau^2d_G\) and zero limiting covariance with \(Y^h\): conditioned on the exterior of the marked sites, distinct bond noises are independent, their conditional means for the difference vanish, and the averaged single-link frustration variance tends to zero. Cauchy–Schwarz with the bounded ordinary innovation handles the common bond. Consequently, for real \(t,u\), the full-law joint characteristic function of the centered, \(\sqrt M\)-scaled pair differs by \(o(1)\) from
\[
 \exp\!\left[-\tfrac12\bigl(8\tau^2d_G\,t^2+
       (\chi_G^{\mathcal C}-8\tau^2d_G)(t+u)^2\bigr)\right]\,
 \mathbb E e^{\,i(t+u)(m_s-\mathbb E m_s)/\sqrt M}.
\]
Here \(t\) multiplies the ordinary source and \(u\) the frustration. The limiting Gaussian contact has thus been separated from their common, potentially non-Gaussian long-distance component. Controlling the variance of that final component is still the outstanding zero-mode estimate.

### 4.78 A zero-mode estimate for protected late first-touch pieces (P on the named geometry)

There is a limited deterministic long-distance estimate for one class of old real readouts. Its source scaling is weaker than the dimension-six projection norm. Use the genuine protected first-touch situation of T2 Proposition 4.26: the *entire* old stencil, its needed raw descendants and its incidence star missed the previous large domain, the current patch is contractible, and the replayed coarse row obeys the original identity \(M^jW=M^j\Gamma\) where that identity is invoked. Put \(r=L^{j-e}\) for its old-to-entry ratio. In a legitimate gauge on such a patch T2 obtains old link logs bounded by \(C r\tau_e\). Indeed its original fine curvature bound on the full patch gives a fine strip-filling gauge bound, and the positive linear part of the actual repeated contour averages has norm one; the product of the nonlinear excesses and the restored endpoint frames are controlled there as stated in T2. A previously live compact stencil touching the patch only at its root is not covered.

On this actual real readout each incident plaquette defect is at most \(C r\tau_e\), by multiplying four unitary links in that gauge. The force estimate of §4.60 and the Casimir formula therefore give
\[
 |h_b|+|r_b-r_b(I)|\le C(\beta_j+1)r^2\tau_e^2 .
\]
The same bound with \(r^4\) holds on a completed stencil whose **actual plaquette** defects are bounded by \(C r^2\tau_e\), for example if the original protected fine curvature collar and all necessary averaging stencils fit so that CURL-STEP-BUDGET applies. No claim is made for a compact bond outside these hypotheses.

Suppose a difference supported on such sheet stencils compares two admitted protected readouts and involves at most \(A_{e,Q} r^{-3}\) old marks per current cell \(Q\). The two individual bounds just proved give
\[
 |\mathrm{sheet}_{e,j,Q}|
       \le C(\beta_j+1)\tau_e^2 A_{e,Q} r^{-1}
\]
for bounded marks. These are *unamplified* real coefficients; multiplying by an additional \(r^{-2}\) would test a different interface. Let
\(\sup_Q\|(\beta_j+1)\tau_e^2 A_{e,Q}\|_2\le P(K)\) for the actual class under consideration, with \(P\) polynomial. For a fixed finite-area sheet with fixed charged geometry this is an explicit counting condition (the geometric area may be included in \(P\)). Regardless of correlations or signs, the squared \(L^2\) norm of the whole sheet sum divided by \(n^4\) is at most
\[
   C_{N_*}P(K)^2 L^{\,4K-6e-2j}.
 \tag{LATE-SHEET-ZERO-COST}
\]
Indeed the number of current cells is \(n^4 L^{-4e}\), and Minkowski gives the squared count times the one-cell square. Thus a polynomial number of these protected terms from \(e\ge(2/3+\epsilon)K\) makes a vanishing zero-mode contribution even at perfect positive correlation. If full old plaquette defects have the stronger two-power bound, a whole \(O(r^{-4})\)-root volume costs only \(C(\beta_j+1)\tau_e^2 A_{e,Q}\) per cell. Its analogous exponent is \(4K-8e\), already vanishing for \(e\ge(1/2+\epsilon)K\).

These calculations show precisely why a return-normalized \(r^{-1}\) discrepancy need not by itself disprove the real variance estimate. They do not assert that all late histories consist of these protected sheets or satisfy the displayed area count, and make no multiplicity charge for their many old roots. For T2's specific waiting profile only its actual single component and original waiting reserve are available. Arbitrarily early surviving compact components and the general signed tail in (POSITIVE-ZERO-LONG-TAIL) still require control.

### 4.79 The signed face-pair operator of the constant mask (P)

The actual leading term of \(m_s\) has an additional cancellation important for its possible off-diagonal covariance. On a comparable-side box write \(F_p=(d_\partial D)_p\) on each oriented tangential face plaquette. By the doubled-cube construction there is a real matrix \(L_{bi,p}\), depending only on the flat cell geometry, such that
\[
 (H_i E D)_b=\sum_{p\subset\partial B}L_{bi,p}F_p,\qquad
 |L_{bi,p}|\le C[(1+|b-p|)^{-4}+s^{-4}].
\]
The image-distance convention in this bound can be taken in the original cube: each of the finitely many reflected images is at least the original separation up to a fixed stencil displacement. Crucially,
\[
 \sum_{\substack{p\subset\partial B\\\operatorname{orient}p=I}} L_{bi,p}=0
             \quad\text{for each two-form orientation }I.
 \tag{FACE-CONSTANT-CANCELLATION}
\]
Indeed prescribe the constant two-form with arbitrary fixed color in orientation \(I\) and zero in all others. It is exact on a rectangular box (use a linear vector potential), closed and co-closed at all free edges. Its actual harmonic extension curvature is exactly that constant form by the same variational uniqueness. Each opposing-plaquette difference \(H_i E D\) vanishes. This proves the separate cancellation including all corners and sides.

For the nonnegative constant comb define \(A_{pq}=\sum_{b\in B\cap\mathcal C,i}L_{bi,p}L_{bi,q}\). It is a positive matrix, real symmetric, with vanishing row sums separately in every orientation. Its off-diagonal entries need not be positive. The exact Gaussian nonidentity coefficient of the **sum** of the boundary conditional means is
\[
 \tau^2\sum_{p,q}A_{pq}\langle F_p,F_q\rangle
       =-\frac{\tau^2}{2}\sum_{p,q}A_{pq}|F_p-F_q|^2 .
 \tag{SIGNED-FACE-PAIR}
\]
The equality is expansion of the square and the exact row cancellation; it is not an assumption about signs of Wilson correlations. More generally any orientation-dependent constant can be subtracted from \(F_p\) in the left side without changing it. The kernel satisfies
\[
 |A_{pq}|\le C\frac{\log(2+|p-q|)}{(1+|p-q|)^4}.
\]
For the convolution proof split the four-dimensional sum over \(b\) into balls of radius \(|p-q|/2\) about the endpoints, the intermediate annulus and the farther exterior. Each endpoint sum costs \(C\log(2+|p-q|)\); the remaining shells with both distances large cost \(C(1+|p-q|)^{-4}\). A constant \(s^{-4}\) term costs at most \(C s^{-4}\log(2+s)\), absorbed by the same bound on a comparable-side box. In particular a perfectly uniform random curvature in any one orientation cannot generate the harmonic face variance.

One may keep differences only between plaquettes of the *same* orientation by polarizing each individual force row before multiplying. For a fixed orientation with \(W_I=\sum_{p:I}|L_{bi,p}|>0\), replace \(\sum_{p:I}L_{bi,p}F_p\) by
\[
 \sum_{p,q:I} L_{bi,p}\frac{|L_{bi,q}|}{W_I}(F_p-F_q).
\]
An orientation with \(W_I=0\) contributes nothing. For \(0<\gamma<1\) the weighted absolute coefficient of this difference row with weight \((1+|p-q|)^\gamma\) is at most
\[
 C_\gamma\sum_{p:I}|L_{bi,p}|(1+|p-b|)^\gamma
      \le C_\gamma(1+d_b)^{\gamma-1}.
\]
The first inequality is the triangle inequality and the normalized weights; the second is summation over three-dimensional faces as in §4.72. For the quadratic sum multiply two such difference rows. Its total absolute coefficient including those two fractional weights is at most \(C_\gamma s^3\sum_{j=0}^{Cs}(1+j)^{2\gamma-2}\), in particular \(C_\gamma s^3\) for \(\gamma<1/2\). This supplies explicit sign, location and support-length information for the surface operator entering the actual constant mode. It does not control the full joint law of those transported curvature differences on distinct faces. The compact comparison errors and the correlations of the signed pairs must still be summed under the true marginal in (POSITIVE-ZERO-LONG-TAIL).

### 4.80 A local-gradient replacement fails on actual regular Wilson boundaries (P)

The signed face-pair kernel cannot be uniformly replaced, even for this constant mark, by a fixed coefficient times the nearest-neighbor tangential differences of curvature on the faces. The obstruction can be realized by actual compact boundary data within FACE-MEAN-COMPARISON, rather than at a singular large-field record.

In an even side-\(s\) box choose a unit Cartan generator and prescribe canonical boundary values sampled from the real potential
\[
 A_4(x)=(x_1^2-x_2^2)s^{-2}T,\qquad A_1=A_2=A_3=0 .
\]
Translate the origin to a corner. This field is uniformly bounded. Its flat discrete divergence is zero and its Laplacian is zero on every free edge. Indeed the two opposing second differences in directions one and two are \(2T/s^2\) and \(-2T/s^2\); all other differences vanish. At a time-normal free edge reaching a time face its transverse differences are still both present; tangential variations on the time face are fixed. Equivalently \(d^*dA=0\) on all free edges. Thus its harmonic extension from those actual boundary values has exactly this curvature, independent of the interior tree representative. At a marked temporal bond the squared sum of the three matching forces is \(8/s^4\) in these canonical units. There are \(\asymp s^4\) such bonds, so the vacuum-subtracted harmonic face contribution for the **unit** comb is bounded below by a positive constant independent of \(s\).

On the other hand every first tangential difference of a given component of the prescribed face curvature has norm at most \(2/s^2\), with at most \(C s^3\) such positions. Its squared sum is at most \(C/s\). The conclusion persists for the *true compact conditional mean*: use the actual boundary links \(\exp(gA_e)\). In the regular arbitrary-representative version of FACE-MEAN-COMPARISON, sum the errors over the cell and subtract the conditional value at identity boundary. The error is bounded by \(C g s^{48}(\log\beta)^5+\mathrm{poly}(\beta,s)e^{-c(\log\beta)^2}=o(1)\) for the increasing sizes of §4.69. This leaves a strictly positive compact conditional difference. Hence a proposed constant-mode estimate paying only the ordinary nearest-neighbor face-gradient energy, with coefficient independent of cell side, fails already on regular input. The weighted, longer face differences of SIGNED-FACE-PAIR are substantive. This example is a bound obstruction for a candidate argument; those fixed boundary values do not carry a claimed positive microscopic probability sufficient to prove unbounded unconditional susceptibility.

### 4.81 A coherent periodic regular boundary obstructs a historywise zero-mode bound (P)

The true conditional mean has a concrete obstruction to a deterministic \(O(\sqrt{|\mathcal C|})\) bound over even its regular face data. Take \(s\) even dividing the torus side on compatible refinements, \(s\to\infty\), \(s\le\beta^{1/200}\); with even stopped side one may use \(s=2L^j\) in the stated range. Align the seams with odd spatial coordinates. On the periodic fine lattice set
\[
 q_s(y)=v(v-s)/s^2,\quad v=y\bmod s\in\{0,\ldots,s-1\},\qquad
 A_4(x)=[q_s(x_1-x_{1,{\rm seam}})-q_s(x_2-x_{2,{\rm seam}})]T ,
\]
and set the other components to zero. The Cartan generator has the unit convention of §4.80. The polynomial vanishes at both ends of the fundamental interval, so it glues at every seam. Use the genuine compact boundary links \(\exp(g A_e)\) and denote these full face data by \(D^{\rm per}\). The polynomial has second difference \(2/s^2\) at every spatial coordinate off its seams. Each temporal comb bond is off every spatial seam. Inside each box the full extension is therefore exactly harmonic for its boundary, as in §4.80. The relative Wilson box comparison gives, uniformly on all the marked bonds,
\[
 \mathbb E[r_b\mid D^{\rm per}]-\mathbb E[r_b\mid I]
       =8\tau^2/s^4+O_N(g s^{44}P^5+\mathrm{poly}(\beta,s)e^{-cP^2}).
\]
The error is \(o(s^{-4})\). Both sides are evaluating compact conditional laws with their true normalizers; identity traces cancel in the difference. In particular the response is coherent in the **constant** direction across the entire torus. Summation gives
\[
 |\mathbb E[Y^r\mid D^{\rm per}]-\mathbb E[Y^r\mid I]|
       \ge c_N n^4/s^4 .
 \tag{COHERENT-REGULAR-FACE}
\]
The same holds for \(h\), since the face means are equal. Dividing by \(\sqrt{|\mathcal C|}\) gives an unbounded quantity on the asymptotically free sequence. By continuity of finite compact conditional expectations the effect persists on open neighborhoods, with positive Wilson marginal mass at every fixed cutoff. Consequently a proposed uniform recordwise bound on the full face conditional mean or its oscillation would fail even within the regular chart. Nonzero Fourier aliases cannot detect this leading uniform profile.

The measure of extremely smooth face orbits is small enough to distinguish that obstruction from an unconditional counterexample. In the displayed configuration all tangential boundary plaquettes have \(s_p\le C/(\beta s^2)\). More generally on comparable boxes the probability that a fixed positive fraction of the \(O(n^4/s)\) distinct tangential face plaquettes have \(s_p\le C/(\beta s^2)\) is at most
\[
 \exp[-c (n^4/s)\log s]
 \tag{SMOOTH-FACE-RARITY}
\]
for large \(s\), with constants depending on the fraction, group and threshold. To verify it, from any such set select at least \(c n^4/s\) plaquettes separated by a fixed lattice distance and choose one distinguished link in each. No action plaquette contains two of those links, and all other links of each selected plaquette are exterior. Given that exterior the selected group integrals are independent. Each one-link conditional density has sup norm at most \(C_N\beta^{d_G/2}\): its Gibbs exponent is the real linear staple functional with uniformly bounded physical Hessian; at its compact maximizer a ball of radius \(c/\sqrt\beta\) gives the matching normalizer lower bound, even if that maximum is degenerate. The small plaquette event imposes on this link a group ball of radius \(C_N/(s\sqrt\beta)\) about a prescribed staple. It has conditional probability at most \(C_N's^{-d_G}\). Multiplying these bounds, and summing over at most \(2^{C n^4/s}\) possible subsets on the faces, gives (SMOOTH-FACE-RARITY). The same argument applies to a gauge-saturated orbit condition whenever it implies the stated elementary plaquette inequalities.

On that event the entire zero observable or its conditional mean has squared magnitude at most \(C_N\beta^2n^8\). Its contribution divided by \(|\mathcal C|\) vanishes on the trajectory. Thus both the severely misaligned compact windows of §4.76 and these extremely smooth coherent windows can be removed in the actual zero-mode \(L^2\) estimate. A weak coherent component superimposed on typical rough boundary curvature is not excluded by the two removals. This is exactly where a bound on the genuine covariance in (POSITIVE-ZERO-LONG-TAIL) is still needed.

### 4.82 Quantitative real-source width of the retained zero-mode response (P)

The actual positive remainder can be bounded after integration in the real constant source, with a rate. Fix a sufficiently small \(t_1>0\), \(4\mid n\), and a compatible face partition of comparable even sides \(s\to\infty,\ s\le\beta^{1/200}\) as above. For \(Y=Y^r\) or \(Y^h\) let \(\mathbb E_t\) denote the exact full compact Wilson law tilted by \(tY\), and put \(m_{s,t}=\mathbb E_t[Y\mid\mathcal F_s]\). Then
\[
 \sup_{|t|\le t_1}|(p_a^Y)'(t)-(p_G^Y)'(t)|\le C/s,\qquad
 \sup_{|t|\le t_1}\left|V^{-1}\mathbb E_t\operatorname{Var}_t(Y\mid\mathcal F_s)
                        -(p_G^Y)''(t)\right|\le C/s .
 \tag{TILTED-ZERO-RATE}
\]
In particular every subinterval \(I\subset[-t_1,t_1]\) satisfies
\[
 0\le \int_I V^{-1}\operatorname{Var}_t(m_{s,t})\,dt \le C/s .
 \tag{RETAINED-SOURCE-WIDTH}
\]
This is a quantitative bound on the genuine signed long-distance response after source averaging. Its integrated bound does not give the height of a possible spike precisely at zero.

First, the real comb tilt preserves reflection positivity at the planes of its eight-site cells. At such a reflection the complete exponential is the product of a real positive-half factor and its reflected factor, with their supported closed-cell links; the ordinary row and the frustration row both have the required scalar reflection rule. Thus the same chessboard proof works on this fixed even cell grid for the tilted measure. A small fixed plaquette-energy exponential, disseminated from such a cell, has a bounded-overlap action sum. The reduced action of §4.75 lies between \((1-C_N|t|)S\) and \((1+C_N|t|)S\). Therefore the fully disseminated tilted moment is bounded by the ratio of two partition functions with positive fixed proportional Wilson couplings, times at most \(e^{C V}\); the scalar identity in the ordinary tilt cancels in normalization. The tree/forest pressure comparison gives log ratio \(O(V)\) uniformly on this interval. This proves the marked plaquette moments, FIRST and the bad-boundary tail under the **actual tilted law**, with constants uniform in \(t\). Every unit plaquette fits in at least one closed cell, and the finite overlap changes only the small chosen plaquette-exponential coefficient.

The good-boundary compact Laplace proof of §4.69 also holds uniformly in these tilts. For \(r\), the field-dependent part of its Casimir relative to its value at identity is \(O_N(g^2s^4T^2)\) in the total source on the comparison window, so it may be absorbed in the same Taylor error. The tilt's surviving quadratic is the sum of matched force squares (or their frustration differences). The exact reduced compact tail still uses \(S_{\rm red}(t)\ge S/2\). Thus moments of the whole box sum through order two incur error at most \(C g s^{68}P^7+\mathrm{poly}(\beta,s)e^{-cP^2}=o(s^3)\), as in §4.77. The uniform tilted fourth moments handle bad exteriors before dividing by any rare mass.

For the noncentral Gaussian bound write \(B A=(H_i A)_i\) on the selected bonds, and \(M\) for the matching identity or the orthogonal matching-difference projection, with fixed constants absorbed in its coefficient. At fixed boundary \(D\), the minimizing extension in the tilted Gaussian is \(E_tD\). Stationarity on free variations and the untilted covariance \(C_B\) give
\[
 B E_tD = B E D + 2t\tau^2 B C_B B^* M B E_tD .
\]
The source operators are bounded in the needed norm: \(\|B C_B^{1/2}\|\le C_N\) by the free curl identity. Therefore \(\|BE_tD\|_2\le C_N\|BE D\|_2\) after reducing \(t_1\). The minimizing quadratic form and covariance remain comparable to the original ones, also giving the same \(s^8\) covariance bound and good-window tail. By HARMONIC-FACE-FORCE and the tilted boundary moments, the entire noncentral mean correction and the noncentral linear variance have averaged size \(O(s^3)\). In the variance bound use the same uniform norm for the tilted covariance. The boundary-free first and second quantities are exactly the deterministic derivatives of the zero-boundary Gaussian log determinant. We have therefore compared each actual global pressure derivative in (TILTED-ZERO-RATE) to the corresponding sum of Dirichlet traces with error \(O(V/s)\) before normalization.

For the rate in comparing to the infinite trace, regard a rectangular Dirichlet cell as a periodic cube of the same side lengths with its seam tangential links fixed to zero. Curls of these zero-boundary variations embed isometrically into the periodic curvature space; seam-tangential plaquettes are zero, and no marked temporal bond lies tangential to a spatial seam. The complementary curvature rank is at most the number of constrained seam link coordinates, \(O(s^3)\). The force insertion is the same bounded periodic operator on that subspace, since the true opposing plaquettes at a marked link agree also across a time seam. Consequently the positive quadratic matrices \(K_D=P_D Q P_D\) and \(K_{\rm per}=P_{\rm per}Q P_{\rm per}\) differ in trace norm by \(O(s^3)\), with uniformly bounded operator norms. Their resolvents \((I-2tK)^{-1}\) are uniformly bounded for \(|t|\le t_1\); the resolvent identity and multiplication by \(K\) give the same trace-norm difference for \(K(I-2tK)^{-1}\) and its square. These are the two centered Gaussian traces in question.

For completeness the periodic Riemann-sum error per site is \(O(1/s)\). For a temporal bond put \(a_\mu(q)=4\sin^2(q_\mu/2)\), \(a(q)=\sum_\mu a_\mu(q)\). Its matched linear-force spectral covariance, apart from the common color and metric factor, is the \(3\times3\) matrix
\[
 G_{ij}(q)=\frac{a_i(q)a_j(q)+\delta_{ij}a_i(q)a_0(q)}{a(q)},
 \qquad G(0)=0,\quad 1\le i,j\le3 .
\]
Indeed \(H_i e_0\) is transverse and has zeroth component \(a_i\) and \(i\)-component of modulus \(\sqrt{a_i a_0}\), with no other component. Projection of the free covariance on these vectors gives the displayed expression. Restriction to the comb averages this matrix over its eight spatial aliases. Each symbol has bounded first derivative, including at the origin where its size is \(O(|q|^2)\) and its directional derivative is \(O(|q|)\). Taking the fixed matching projection, metric factor and the two bounded resolvent functions preserves a uniform Lipschitz bound for the traced Fourier integrands. Finite Riemann sums on comparable-side boxes thus have the stated \(O(1/s)\) per-site error, uniformly in \(t\). The ordinary identity contribution has its exact parity-cell proportion. This proves both inequalities (TILTED-ZERO-RATE).

At each finite mesh, differentiating the real compact integral gives \((p_a^Y)''(t)=V^{-1}\operatorname{Var}_t(Y)\). Integrate its positive decomposition over \(I=[u,v]\). The left side of (RETAINED-SOURCE-WIDTH) equals \((p_a^Y)'(v)-(p_a^Y)'(u)-\int_I V^{-1}\mathbb E_t\operatorname{Var}_t(Y\mid\mathcal F_s)\,dt\). Applying the two uniform estimates proves the bound, with \(C\) independent of the chosen subinterval. Thus the Lebesgue measure of source parameters where the retained variance per site exceeds \(B>0\) is at most \(C/(sB)\). This rules out any broad large-susceptibility interval in the real unamplified parameter. The original pressure derivative is fixed at \(t=0\), so an exceptional shrinking set still matters.

### 4.83 Shrinking-disc test and the signed contribution of actual full-law zeros (P)

Set \(V=n^4\), let \(s\asymp\beta^{1/200}\) be an admissible side in §4.82, and let \(Y\) be either unamplified unit comb \(Y^r,Y^h\). Write \(F(z)=\mathbb E_W \exp[z(Y-\mathbb E_WY)]\) and let \(\rho\) be the infimum of the moduli of its zeros, interpreted as infinity if there are none. For \(0<r\le t_1/2\), (TILTED-ZERO-RATE) implies
\[
 \sup_{|z|\le r}\log|F(z)|\le V C_N(r^2+r/s).
 \tag{CENTERED-COMB-GROWTH}
\]
Indeed the modulus is bounded by the positive integral at \(\Re z\). Integrate the first estimate of §4.82 between 0 and \(\Re z\) after subtracting the exact slope at zero. The limiting Gaussian pressure has a bounded second derivative on this interval.

If \(r\le\rho\), a centered log exists on the open disk. For any analytic \(g\) with \(g(0)=0,\ \Re g\le A\), Schwarz's lemma applied to \(g/(2A-g)\) and Cauchy's estimate on the half disk give \(|g''(0)|\le16A/r^2\). Apply this to \(g=\log F\). In particular
\[
 \operatorname{Var}_W Y/V\le C_N(1+1/(sr)),\qquad 0<r\le\min(\rho,t_1/2).
 \tag{SHRINKING-COMB-DISC}
\]
A zero-free radius \(c/s\) already suffices for the actual comb and hence for the ordinary all-mark conclusion of §4.38, using either the ordinary comb directly or its exact Ward comparison with frustration. Conversely, on any sequence with \(B_a=\operatorname{Var}_W Y/V\to\infty\), the full partition function must have \(\rho\le C/[s(B_a-C)]\). In particular \(s\rho\to0\). The assertion concerns the undivided compact Wilson integral, including the retained face law.

Even this shrinking disc can contain zeros without causing a large positive susceptibility. There is a quantitative signed test. At any \(0<R\le t_1/4\) with no zero on its boundary, let \(\mathcal D_R\) be the zeros of \(F\) inside the disk with multiplicity. Then
\[
 \left| \frac{\operatorname{Var}_W Y}{V}
      +\frac1V\sum_{\zeta\in\mathcal D_R}\Re(\zeta^{-2})\right|
 \le C_N\big(1+(sR)^{-1}\big).
 \tag{SIGNED-COMB-ZEROS}
\]
To prove it, Jensen's formula at \(2R\), using (CENTERED-COMB-GROWTH), gives
\(\#\mathcal D_R\le C V(R^2+R/s)\). A zero on the outer circle is handled by continuity from radii around \(2R\). Divide \(F(z)\) by the finite product of normalized factors
\[
 b_\zeta(z)=(1-z/\zeta)/(1-\bar\zeta z/R^2).
\]
Each has boundary modulus \(R/|\zeta|\ge1\) and value 1 at zero. The quotient is analytic and nonvanishing in the disk, and its normalized log has real part at most \(C V(R^2+R/s)\) by the maximum principle. The same Schwarz bound controls its second derivative. The second derivative of \(\log b_\zeta\) at zero is \(-\zeta^{-2}+\bar\zeta^2/R^4\); the absolute sum of the latter corrections is bounded by \(R^{-2}\#\mathcal D_R\). Adding the derivatives and taking real parts proves the estimate.

Choosing \(R\in[1/s,2/s]\) off the finitely many zero radii leaves a bounded error in (SIGNED-COMB-ZEROS). Thus divergence at the precise real base point would require a diverging signed sum weighted by \(-\cos(2\arg\zeta)/|\zeta|^2\) per site; zeros closer to the real than the imaginary axis have a negative contribution. Jensen also bounds the zero count in this window by \(C V/s^2\). Neither a severe exterior's local zeros (§4.59) nor the physical \(a^{-2}\)-amplified zeros (§4.56) are entries in this sum by virtue of those separate results. Verifying an upper bound on the signed sum for the full law, or excluding all true zeros on \(c/s\), is open on the required trajectory.

### 4.84 Deep-root tilted comparison on the true comb and a smaller sufficient disc (P)

The full-law first slope in (TILTED-ZERO-RATE) has a smaller error than its fixed-partition boundary count. Each individual marked expectation may use a different translated box, with that root deep inside the box. For either unit comb \(Y^r,Y^h\), on the trajectory and compatible mesoscopic sizes of §4.82, one has
\[
 \sup_{|t|\le t_1}|(p_a^Y)'(t)-(p_G^Y)'(t)|\le C_N s^{-3}.
 \tag{DEEP-TILTED-COMB-SLOPE}
\]
Here \(t_1\) is a sufficiently small fixed constant. Consequently the factor \(1/(sR)\) in (SHRINKING-COMB-DISC) and (SIGNED-COMB-ZEROS) can be replaced by \(1/(s^3R)\). A full zero-free radius \(c/s^3\), or a bounded signed inverse-square zero sum at \(R\asymp s^{-3}\), suffices for ordinary SUS.

**Thin rectangles under the actual comb tilt.** The charged transfer argument of §4.73 has a real-tilted version. In a chosen propagation direction put subdivision planes two sites apart, spatial planes at odd coordinates. Every term of the marked action fits in one closed slab. Terms carried entirely by a subdivision plane can be split in half between its adjacent slabs. The ordinary Casimir, the three force squares, and the full force square in frustration are individually invariant under coordinate reflections as scalar functions at the reflected bond. Reflection in a plane through a spatial site preserves the even spatial mark, and time reflection reverses the temporal bond while preserving its mark. For reversal of an oriented link the three gradients are simultaneously rotated and sign-changed at the reversed endpoint, leaving their contracted products invariant. In particular reflection about a slab midpoint preserves the slab action. 

Integrating a two-site slab gives a bounded real symmetric transfer \(T_2\) on invariant slice functions. In the endpoint color sector retain parallel transport of the two straight propagation segments in the slab, acting on the left and right matrix indices as in §4.73. Reversing the slab replaces these unitary factors by their adjoints, so its charged transfer \(T_{2,c}\) is self-adjoint too. This construction uses the original compact measure on each slice and internal link and the half weights of entirely boundary terms. Integration over common slices composes the kernels by Fubini, including the concatenated transport indices. Slice gauge covariance preserves the two indicated subspaces. Thus the four-site transfers \(T_4=T_2^2,\ T_{4,c}=T_{2,c}^2\) are positive. The subdivision starts on any admissible odd spatial or any temporal plane. At \(4\mid n\) the exact loop expectation between two such planes separated by \(4l\) is
\[
 W_t(4l,1)=
 \frac{\operatorname{Tr}(T_4^{n/4-l}\,O^*T_{4,c}^{\,l}O)}
      {\operatorname{Tr}(T_4^{n/4})}
 \ \ge\ W_t(4,1)^l,\qquad 1\le l<n/4 ,
\]
with \(O\) multiplication by the normalized unit transverse link. The spectral weights are the nonnegative weights from §4.73 and sum to one by \(O^*O=I\). The uniform tilted plaquette first moment in §4.82 gives \(1-W_t(4,1)\le C/\beta\) by expressing the perimeter word as a product of four conjugated plaquettes and applying the triangle inequality in \(L^2\). Therefore \(\sqrt\beta\|U_{\rm rect}-I\|_{L^2(\mu_t)}\le C\sqrt l\). For arbitrary thin rectangles of lengths \(1\le j\le Cs\), trim boundedly many unit plaquettes at the two ends to leave a length divisible by four starting on an admissible plane. The removed plaquettes cost \(O(1)\) in this normalized \(L^2\) norm. The same estimate \(C\sqrt j\) follows, including bounded \(j\). Orientation and translations need only respect the actual parity of the slab endpoints. The coordinate-tree construction in §4.73 now gives
\[
 \|D_e\|_{L^2(\mu_t)}\le C\sqrt s
 \tag{TILTED-THIN-TREE}
\]
for each boundary link in that particular boundary representative. The unnormalized gauge chord log is globally bounded by a constant times its distance to identity; the finite product of thin rectangles uses no independence. Ordinary fixed higher moments follow from the elementary strip bound \(\|D_e\|_{p}\le C_p s\). On the good set the canonical boundary is in the chart of the actual tilted box comparison. Its complement still has superpolynomial probability by the tilted marked exponential estimate on the strips. Evaluation of the invariant conditional scalar on this orbit is valid even if its representative was chosen with interior links.

**Decay of the matching-force resolvent.** On the doubled torus of §4.70 use the relative extension of free one-forms by minus reflected pullback across each face. Tangential variations on that face vanish; every other free edge has exactly \(2^4\) copies. The extended curl norm and the sum of matched source squares are both \(2^4\) times their Dirichlet norms. Marked temporal bonds are strictly off the spatial seams, and temporal normals have distinct mirror images across a time seam. The extension commutes with \(H_i=d_i^*d_i\), and the matching projection \(M\) commutes with these reflections because all three force components at the reflected temporal bond transform by the same sign. The relative subspace consists precisely of these extensions before taking the gauge quotient. Orthogonal projection by the signed reflection average commutes with the periodic Gaussian precision. Thus the Dirichlet matching-force covariance on the comb is the signed sum of the periodic kernel over the \(2^4\) reflected source positions. Equivalently one can work on curls or discard the null-gradient space throughout, since every force annihilates it. The orientations of reflected bonds are included in those signs.

Write \(G\) for the positive matrix of unrestricted matched force covariances on the comb, with all fixed color and metric constants included. Its symbol is the eight-alias average in §4.82. The tilted matching resolvent is \((I-2t\tau^2 G M)^{-1}\), and the tilted covariance is \((I-2t\tau^2 G M)^{-1}G\). The same expressions on the relative subspace give the reflected Dirichlet kernels. For both periodic operators every nondiagonal kernel is bounded, up to fixed within-cell coordinates, by \(C(1+d)^{-6}\) on the infinite comb. To check the decay, the sole nonsmooth term in the folded \(G\) symbol at zero is the unaliased numerator of degree four divided by the lattice Laplacian symbol of degree two. Its \(j\)-th derivative is bounded by \(C_j|q|^{2-j}\) on a punctured small ball. Subtract a smooth background matrix there, including all smooth aliases, and retain these derivative bounds on the difference. Matrix inversion preserves them after subtracting the smooth-background inverse: use the resolvent identity and the uniformly bounded inverses for \(|t|\le t_1\). The covariance symbol has the same property by multiplication. A smooth dyadic annulus of size \(\rho\) therefore contributes \(C_J\rho^6(1+\rho d)^{-J}\) for any fixed \(J>6\), by the integration by parts in §4.72. The smooth part has faster decay. Summing proves the claim. On a comparable doubled cell the periodic kernel is the absolutely convergent image sum, thus bounded by \(C[(1+d_{\rm per})^{-6}+s^{-6}]\) away from its diagonal. The infinite diagonal and periodic diagonal differ by \(O(s^{-6})\). Imposing the relative reflections changes the diagonal at a root at least \(cs\) from the faces by another \(O(s^{-6})\); every nonidentity mirror image is at distance at least \(c's\). These estimates concern actual covariance and its resolvent action on the force, not the long-range inverse precision on arbitrary gauge links.

At a deep root \(x\), the untilted harmonic force \(u_y=(B E D)_y\) has \(L^2(\mu_t)\) norm on the good event bounded by \(C s^{-3/2}\) for all \(y\) within \(c's\) of \(x\). Indeed integration by parts over each face in §4.73 gives the total boundary-link coefficient \(C s^{-2}\), and (TILTED-THIN-TREE) supplies \(C\sqrt s\) per link. At every other marked root the good-event \(L^2\) norm is bounded by a constant, by the boundary-curvature kernel of §4.72 and the tilted plaquette moments of §4.82. On the tilted Gaussian, with boundary \(D\), the noncentral matched force equals \((I-2t\tau^2G_D M)^{-1}u\), as proved in §4.82. Its \(L^2(\mu_t)\) norm on the good event at \(x\) is at most \(C s^{-3/2}\). For the near terms use the uniform absolute row sum of the relative resolvent and the deep estimate on \(u\). Far terms have absolute coefficient sum \(O(s^{-2})\) in four dimensions by the \(d^{-6}\) tail; any nontrivial mirror image seen from \(x\) is at least \(cs\) away and contributes at most \(C s^4s^{-6}\). These bounds allow the same actual boundary law for every \(u_y\) in this linear combination.

The expected quadratic noncentral contribution at \(x\) is consequently \(O(s^{-3})\). The Dirichlet covariance trace at that root differs from the infinite tilted Gaussian trace by \(O(s^{-6})\) from the image estimates above. The exact tilted compact one-root comparison on a good boundary has error \(C_N g s^{44}P^5+\mathrm{poly}(\beta,s)e^{-cP^2}=O(s^{-3})\) on the specified range. The proof is the single-insertion estimate of §4.69 with the uniform real tilt of §4.82, using coercivity on the tilted quadratic form, and includes the ordinary Casimir about its identity value. On a bad boundary the unconditional error is superpolynomial by the higher true tilted moments and conditional Jensen. The infinite reference expectation is \(8(p_G^Y)'(t)\) per marked site, including the scalar row, since the comb has density \(1/8\). Place each root in turn deep inside its chosen compatible translated partition, apply the local estimate and take the average over the genuine full compact torus. This proves (DEEP-TILTED-COMB-SLOPE). No change of the global Wilson law is made when changing the partition for a different root.

Integrating this sharper real slope as in (CENTERED-COMB-GROWTH) gives \(\log|F(z)|\le C V (R^2+R/s^3)\). The entire argument of §4.83 applies verbatim with \(s^3\) in place of \(s\). In particular an unbounded excess at zero requires \(s^3\rho\to0\) for genuine full-law zeros, and \(\#\mathcal D_R\le C V/s^6\) at \(R\asymp s^{-3}\). The remaining test is still on exactly the unamplified constant comb and is distinct from any no-go theorem for the physical source.

### 4.85 A based column gauge increases the proven distance and zero-free test scales (P)

The comparison of one tilted root in §4.84 admits larger boxes. Put \(P=\log\beta\) and choose comparable even sides of order
\[
 S_\beta=\left\lfloor c\,\beta^{1/35}P^{-6/35}\right\rfloor .
 \tag{COLUMN-BOX-SCALE}
\]
Use sizes \(2\le s\le S_\beta\) which fit the trajectory torus. Then (DEEP-TILTED-COMB-SLOPE) continues to hold, as does (ZERO-MODE-PAIR) with \(L_\beta\) comparable to \(S_\beta\). In particular it suffices to prove a true zero-free disc \(c S_\beta^{-3}\) for the unamplified full comb. The larger scale pertains to the one-root comparison and its direct consequences.

Here is the exact physical change of variables. Choose the boundary representative by the full coordinate tree of §4.73. On the event that every plaquette in the box obeys \(\sqrt\beta\|U_p-I\|\le P\), every boundary link in this representative is a product of at most three strips of at most \(Cs\) elementary plaquettes. Hence its canonical logarithm satisfies \(\|D\|_\infty\le C sP\). Failure of this event costs \(C s^4e^{-cP^2}\) in the actual tilted law by §4.82. For each such fixed representative, integrate interior gauges using a different forest, based on the bottom time face. In every column at a spatially interior vertex fix the temporal bonds from the bottom through the last interior vertex to identity, leaving only the final temporal bond to the top free. Each interior vertex has one parent, so these changes exhaust the allowed interior site gauges with unit Haar factors. All links lying in any boundary face stay prescribed.

Every free spatial bond at height \(t\) can now be compared to the corresponding edge on the bottom by the single width-one curtain of height \(t\); the two vertical sides below the top are in the based forest or on a prescribed spatial face. Its boundary reference path has length at most \(Cs\), with every factor either the identity or prescribed. For a last free vertical bond, take a straight spatial path from its column to one side at the same top time. The full-time curtain over this path gives the top, side and bottom boundary return, with all other links in the original column fixed. Every curtain has at most \(C s^2\) distinct plaquettes, each used once. Telescoping the oriented holonomy across these rectangles and applying Cauchy–Schwarz gives for each physical free chord \(e\)
\[
 \|U_e-I\|\le C s\Big(\sum_{p\subset B}\|U_p-I\|^2\Big)^{1/2}
                      + C g s\|D\|_\infty .
 \tag{COLUMN-CURTAIN}
\]
This also covers spatial free edges meeting a side, since a side column's vertical sides are prescribed. In the exact linearized inequality for a real one-form replace the group distance by the absolute free component, the plaquette defects by \(dB\), and the last term by \(Cs\|D\|_\infty\). In particular each free coordinate at zero boundary, as a functional on the curl energy space, has norm at most \(Cs\). Its variance under the homogeneous or tilted Gaussian is at most \(Cs^2\), by uniform quadratic comparability. This is an individual-coordinate bound and needs no operator norm bound on the full link covariance.

The zero extension of prescribed boundary links has curl norm at most \(C s^{3/2}\|D\|_\infty\), since only \(O(s^3)\) stencils meet it. The tilted minimizing curvature has at most a constant multiple of that norm by quadratic comparability. Its mean in every individual free component is consequently bounded by \(C(s^{5/2}+s)\|D\|_\infty\le C s^{7/2}P\). Choose \(T=C_*s^{7/2}P\) with a sufficiently large constant. Gaussian tails of the largest free component outside \(T\) are at most \(C s^4e^{-cP^2}\). In the compact integral, outside the free ball of physical radius \(gT\), (COLUMN-CURTAIN) implies \(\beta\sum_p s_p\ge cT^2/s^2\). Chord distance and bounded principal logarithm on the compact group are comparable with fixed constants, including at the chart cut. The globally reduced compact tilted exponent has positive action \(\ge c\beta\sum_p s_p\) after removal of its fixed identity scalar. Integrating over compact probability Haar variables bounds the complement's mass by \(e^{-cT^2/s^2}\). On the other hand the zero-boundary extension plus all free Gaussian coordinates in canonical unit balls give, in the common physical normalization,
\[
 Z_{G,t}(D)\ge
 \exp[-C s^4(1+\log\beta)-C s^3\|D\|_\infty^2]
 \ge \exp[-C s^4(1+\log\beta)-C s^5P^2].
\]
Because \(T^2/s^2=C_*^2s^5P^2\), the compact complement relative to this Gaussian is superpolynomial for large \(C_*\). These bounds treat the entire compact complement, including different branches of the link logarithm.

Throughout the canonical ball the physical word expansion and Haar factor give a uniform log-density error
\[
 \Delta\le C(g s^4T^3+g^2 s^4T^2)
       \le C g s^{29/2}P^3\le C s^{-3}
 \tag{COLUMN-DENSITY-ERROR}
\]
by (COLUMN-BOX-SCALE); here \(g=\beta^{-1/2}\). This includes the Taylor expansion of the real reduced action, whose force insertions have fixed smooth words and uniformly bounded Taylor remainders after their quadratic terms. The exact original observable at one root differs from its Gaussian quadratic plus the indicated bounded identity term by \(C gT^3\). Relative density comparison and the two tail estimates then give on a good representative
\[
 |m_{t,x}(D)-m_{G,t,x}(D)|
 \le C gT^3+C\Delta\,[1+|(B E_tD)_x|^2]
                +\mathrm{poly}(\beta,s)e^{-cP^2}.
 \tag{COLUMN-ONE-ROOT}
\]
Indeed the Gaussian expectation of the absolute local quadratic is bounded by \(C[1+|(B E_tD)_x|^2]\) using the bounded diagonal covariance. One need not pay the supremum \(CT^2\) of that quadratic to compare the normalized integrals. Tail Gaussian moments satisfy the same superpolynomial bound by the canonical coordinate estimates; the exact compact one-root observable is bounded by \(C\beta\).

The actual good-boundary curvature in linear coordinates still has fixed entrywise \(L^p\) moments: the short-word error between \(d_\partial D\) and the canonical plaquette log is \(O(g s^2P^2)\), and the tilted marked moments control the latter. Thus the deep \(L^2\) harmonic estimate and the relative resolvent proof of §4.84 apply without changing constants. For the \(L^4\) version interpolate (TILTED-THIN-TREE) with the elementary \(L^8\) strip bound \(Cs\), giving \(C s^{5/6}\) for each boundary link. The deep \(L^4\) harmonic force after face integration by parts and the resolvent tail is \(O(s^{-7/6})\), while at other sites it has bounded good-event \(L^4\) norm by the curvature kernel. Taking true tilted expectations in (COLUMN-ONE-ROOT) now gives an \(L^1\) and an \(L^2\) comparison error \(O(s^{-3})\) at a deep root. The bad event is absorbed by the true higher moments and conditional Jensen. This proves the enlarged first-slope estimate. At \(t=0\), two roots at separation \(d\) can again be placed deep in distinct cells of width comparable to \(\min(d/C,S_\beta)\); their conditional means differ in \(L^2\) from their deterministic Dirichlet traces by \(O(s^{-7/3})\). Conditional independence and Cauchy–Schwarz give (ZERO-MODE-PAIR) on the claimed longer distance scale. In fact this last argument works at every \(|t|\le t_1\) for the corresponding tilted observable. The Gaussian far trace and near covariance signs in §4.74 are unaffected.

One obtains a quantitative unconditional bound even without control of the true zeros at the sufficient radius. Around each real \(t\in[-t_1/2,t_1/2]\), integrate the sharp slope on both sides of \(t\) for the centered variable \(X=Y-\mathbb E_tY\), obtaining \(\mathbb E_t e^{\pm uX}\le\exp[C V(u^2+|u|s^{-3})]\). Taking \(u=c\min(V^{-1/2},s^3/V)\) and using \(\cosh v\ge1+v^2/2\) gives
\[
 \frac{\operatorname{Var}_t Y}{V}\le C(1+V/s^6).
 \tag{FULL-TILTED-ZERO-UPPER}
\]
In particular the true \(F(t+iv)\) is nonzero throughout
\(\lvert v\rvert<c\min(V^{-1/2},s^3/V)\), since the real part of its centered tilted characteristic function is at least \(1-v^2\operatorname{Var}_t Y/2\). At \(s\asymp S_\beta\) this is still far smaller than the sufficient radius \(S_\beta^{-3}\) on the required trajectory. The unknown is the ordinary excess at that specified zero mode.

### 4.86 Removing all rare one-link conditional zeros at negligible cost to the true comb variance (P)

There is an exact modification of the observable which leaves the entire retained mean intact while regularizing the conditional source on every exterior. Let \(\mathcal E\) be all links except the temporal comb links. For a selected bond there are six oriented staples \(K_1,\dots,K_6\in SU(N)\) such that the incident action is \(\sum_j(N-\Re\operatorname{Tr} U_bK_j)\). All six depend only on \(\mathcal E\), and distinct selected links are conditionally independent. Define the gauge-invariant mismatch
\[
 d_b^2=\min_{V\in SU(N)}\sum_{j=1}^6\|V K_j-I\|_{\rm HS}^2 .
\]
For fixed small \(\delta>0\) call the exterior at \(b\) regular if \(d_b\le\delta\). In the full original law, or its real tilt by either unamplified comb with \(|t|\le t_1\), \(d_b^2\le 2e_b\) at every actual fine field, where \(e_b\) is the sum of the six plaquette energies. The tilted marked moments therefore give
\[
 \mathbb P_t(d_b>\delta)\le C e^{-c\beta},\qquad
 \mathbb E_t(\beta d_b^2)\le C .
 \tag{STAR-MISMATCH-TAIL}
\]
This even controls joint bad sets: the incident plaquette groups of distinct comb roots are disjoint and the fixed-grid disseminated marked moment bound of §§4.22,4.76,4.82 applies with a fixed small positive exponential coefficient. Thus \(\mathbb P_t(d_b>\delta,\ b\in A)\le (C e^{-c\beta})^{|A|}\). Only the single-site estimate is needed below.

Choose \(Y_b=r_b\) or \(h_b\), the same choice at every root, and put \(m_{b,t}=\mathbb E_t[Y_b\mid\mathcal E]\). Within this fixed actual tilted law define
\[
 \widetilde Y_b=1_{\{d_b\le\delta\}}Y_b+1_{\{d_b>\delta\}}m_{b,t}.
\]
This construction is used at \(t=0\) for the physical susceptibility. At other real \(t\) it describes that tilted law's conditional innovation. Its conditional mean equals \(m_{b,t}\) on all histories. Conditional independence, conditional centering on every replaced star, and the variance tower give exactly
\[
 0\le \operatorname{Var}_t\Big(\sum_b Y_b\Big)
        -\operatorname{Var}_t\Big(\sum_b\widetilde Y_b\Big)
    =\sum_b\mathbb E_t[1_{\{d_b>\delta\}}
                      \operatorname{Var}_t(Y_b\mid\mathcal E)]
    \le C |\mathcal C|\beta^2e^{-c\beta}.
 \tag{REGULARIZED-COMB-VARIANCE}
\]
For arbitrary real comb marks, multiply the summand by \(f_b^2\). No sign assumption on any distant covariance has been used. In particular the possibly correlated means of even the moderately bad records remain present. Removing a whole bad local observable including its mean would not give this identity.

There are constants \(r_*>0,C_N<\infty\) independent of cutoff, exterior and volume such that the centered conditional log of each modified variable has a single-valued branch at zero with
\[
 \left|\log\mathbb E_t\big[e^{z(\widetilde Y_b-m_{b,t})}\mid\mathcal E\big]\right|
       \le C_N |z|^2(1+\beta d_b^2),\qquad |z|\le r_* .
 \tag{REGULAR-STAR-LOG}
\]
On bad stars this log vanishes identically. To prove the claim on regular stars choose a minimizer \(V\) defining \(d_b\) and write \(U_b=X V\). Each \(V K_j\) is within \(d_b\) of \(I\). Use the analytic action and compact Haar Jacobian on one fixed exponential chart of \(SU(N)\) as in §4.21; real traces have their holomorphic trace-plus-inverse continuation. At \(d_b=0\) the reference action on the group is \(6(N-\Re\operatorname{Tr} X)\), with a unique minimum at \(I\), positive definite Hessian there and a positive gap outside a smaller fixed chart. At that point \(D_b\) and \(P_b\) have vanishing value and first jet. The Casimir contribution divided by \(\beta\) has zero first jet too. Write \(q=Y_b/\beta\), a uniformly smooth holomorphic word with a possible \(\beta^{-1}\) Casimir. After tilting, the phase is \(S_b-(t+z)q\). On a regular star, at \(X=I\) the first jets of \(S_b\) and \(q\) are \(O(d_b)\). The exponent is thus uniformly coercive on this chart and has its exterior gap for sufficiently small \(\delta,t_1,|z|\) (for complex \(z\) this refers to the real part on the compact real complement). The analytic critical point \(a(w)\) of \(S_b-wq\) exists for \(|w|\le 2r_0\) in fixed logarithmic coordinates by the uniform inverse Hessian theorem, \(a(w)=O(d_b)\). Its Hessian \(H(w)\) has positive real part, and \(\nabla q(a(w))=O(d_b)\). In particular \(a'(w)=H(w)^{-1}\nabla q(a(w))=O(d_b)\).

For clarity the finite-dimensional saddle comparison is relative to the same conditional normalization. In the fixed real coordinate chart translate a smaller integration ball to \(a(w)\) plus that ball. The holomorphic Haar form on the swept side has a uniform action gap, by the real gap at the boundary of the ball and the small displacement; the remaining compact complement has the same gap relative to the critical scalar. In centered coordinates \(y\) the phase difference is \(y^TH(w)y/2+O(|y|^3)\). On a smaller fixed ball its real part is at least \(c|y|^2\). Integrating with \(y=\beta^{-1/2}v\) gives the Gaussian determinant and a uniform relative error \(O(\beta^{-1/2})\), by truncation at a fixed small coordinate radius and Gaussian polynomial domination of the first Taylor remainder. The Haar Jacobian near the saddle is bounded away from zero. Thus on a fixed complex disc the exact log partition conditional on \(\mathcal E\) has the form
\[
 -\beta(S_b-wq)(a(w))-\tfrac12 d_G\log\beta+c_N
       +\log j(a(w))-\tfrac12\log\det H(w)+R_\beta(w),
 \qquad |R_\beta|\le C\beta^{-1/2}.
\]
It is analytic, with all logs chosen continuously on the disc. All estimates are uniform over the compact regular staple parameters. A bounded initial interval of \(\beta\ge1\) can instead use the elementary conditional near-one estimate on a smaller common source disc. The second derivative of the critical exponent is \(\beta\nabla q(a(w))^T H(w)^{-1}\nabla q(a(w))=O(\beta d_b^2)\). The remaining analytic terms have bounded second derivatives on a smaller fixed disc by Cauchy. Subtract value and the exact first derivative at the real \(t\), then integrate the second-derivative bound twice. This proves (REGULAR-STAR-LOG), shrinking \(t_1,r_*\) if necessary. The compact saddle uses only one actual group integral; no external normalization or global analytic continuation enters.

Consequently all modified conditional cumulants of order \(m\ge2\) satisfy
\[
 \sum_b\mathbb E_t\left|
    \kappa_m(\widetilde Y_b\mid\mathcal E)\right|
       \le |\mathcal C| C_N^m m!.
 \tag{ANNEALED-REGULAR-STAR-JETS}
\]
The exact real-law expectation of \(\beta d_b^2\) was essential here. The literal variables instead have the bad-star high-order behavior proved in §4.58. One can quantify the local zeros that the replacement removes. Write \(\zeta_{b,j}\) for the zeros of the centered conditional partition function of the **original** \(Y_b\) at the fixed tilted exterior. On a regular star there are none for \(|z|\le r_*\). On every star \(|\Im\zeta_{b,j}|\ge c/\beta\), since the range of \(Y_b\) has length \(C\beta\) and a phase interval shorter than \(\pi\) makes the tilted integral nonzero after one rotation. Jensen's formula at \(2r_*\) and the elementary bound \(\log|F_{b,t}(z)|\le C\beta|z|\) give at most \(C\beta\) zeros inside \(r_*\), counted with multiplicity. Therefore
\[
 \frac1{|\mathcal C|}\mathbb E_t\sum_b
       \sum_{|\zeta_{b,j}|<r_*}|\zeta_{b,j}|^{-2}
       \le C\beta^3 e^{-c\beta}.
 \tag{CONDITIONAL-ZERO-MASS}
\]
The conditional product zeros are exactly the pooled local zeros. In contrast (SIGNED-COMB-ZEROS) involves zeros of the expectation of this product over the actual exterior. Its signed contribution is still uncontrolled. The comparison (REGULARIZED-COMB-VARIANCE) allows the ongoing susceptibility argument to work with uniformly regular conditional factors, while continuing to integrate the true exterior and its unchanged retained mean.

### 4.87 The literal frustration comb has a small extensive heatbath noise on a fixed real interval (P)

For \(Y=\sum_{b\in\mathcal C}h_b,\ M=\mathbb E_0(Y\mid\mathcal E)\), with the full original Wilson law at zero source, one has on a fixed sufficiently small real interval
\[
 \log\mathbb E_0 e^{t(Y-M)}\le C V t^2/\beta,\qquad
 0\le V^{-1}\bigl(\log\mathbb E_0e^{tY}-\log\mathbb E_0e^{tM}\bigr)
                \le C t^2/\beta .
 \tag{FULL-RETAINED-FRUSTRATION-PRESSURE}
\]
The susceptibility decomposes as
\[
 0\le \operatorname{Var}_0(Y)-\operatorname{Var}_0(M)
       =\mathbb E_0\operatorname{Var}_0(Y\mid\mathcal E)\le C V/\beta .
 \tag{FULL-RETAINED-FRUSTRATION-VARIANCE}
\]
Thus for this precise zero-mode observable the microscopic noise discarded in passing to the exact exterior source has a uniform quantitative bound. These inequalities use the literal frustration observable on every star. They do not apply with the same small right side to the ordinary one-link innovation, whose nonzero limit is computed in §4.57.

To see the stronger source scaling, work in the staple chart of §4.86. In matching \(i\) the temporal-link force is linear in the sum of its two staples as a function of their matrix entries. The three forces use the same left generators and the same multiplication by the varied link \(U_b\). For each pair \(i,j\) their difference therefore has norm \(O(d_b)\), with the same bound on all derivatives in a fixed complex link chart. This follows directly by subtracting the two linear expressions when all six \(V K_j\) equal the identity; the difference coefficients consist only of deviations from that common matrix. The exact identity
\(q=h_b/\beta=\frac13\sum_{i<j}|F_{b,i}-F_{b,j}|^2\)
shows that \(q\) and its continuation have all fixed chart derivatives \(O(d_b^2)\). At \(d_b=0\) the entire observable vanishes. For \(0<d_b\le\delta\), apply the same single compact integration as in §4.86 to the uniformly bounded analytic function \(q/d_b^2\), using source parameter \(w=z d_b^2\). Compact complement estimates hold because the bound \(C d_b^2\) on \(q\) also holds on the whole real group. The analytic critical exponent and the bounded determinant and remainder then give for the original conditional centered log
\[
 K_b(z)=\log\mathbb E_0[e^{z(h_b-m_{b,0})}\mid\mathcal E],
 \qquad
 |K_b(z)|\le C\beta d_b^4 |z|^2,\qquad |z|d_b^2\le c .
 \tag{MISMATCH-SCALED-FRUSTRATION}
\]
Indeed in the \(w\) parameter the second derivative of the critical term is bounded by \(C\beta\), and all other second derivatives are bounded uniformly on the smaller disc. This argument does not assert the local normalized conditional log is regular on a large disc at a misaligned exterior. For real \(t\) on any exterior one still has \(0\le K_b(t)\le C\beta^2 t^2\), since the second derivative along the real line is a conditional variance bounded by the squared range. For the exponential moment argument itself use the sharper elementary bound on \(e^{K_b(t)}-1\) given below.

On the regular stars the single-site conditional variance is at most \(C\beta d_b^4\); on the others use \(C\beta^2\). The full-law marked moments and (STAR-MISMATCH-TAIL) give an average \(O(1/\beta)\) per root, even when averaging those conditional variance bounds under a small true real tilt. Conditional independence proves (FULL-RETAINED-FRUSTRATION-VARIANCE) at zero. At any fixed order \(m\ge2\), Cauchy's estimate on the scaled disc gives \(C^m m!\beta d_b^{2m}\) on regular stars. The marked exponential yields \(\mathbb E_0 d_b^{2m}\le C^m m!\beta^{-m}\). On bad stars the elementary radius \(c/\beta\) gives the bound \(C^m m!\beta^m\). Thus the original annealed absolute one-site conditional jet is at most
\(C^m(m!)^2\beta^{1-m}+C^m m!\beta^m e^{-c\beta}\).
This fixed-order gain is compatible with the high-source-order obstruction of §4.58.

For the full real pressure let \(K_{\mathcal E}(t)=\sum_b K_b(t)\ge0\). Exact conditional multiplication gives \(\mathbb E_0[e^{tY}\mid\mathcal E]=e^{tM+K_{\mathcal E}(t)}\). Consequently
\[
 \frac{\mathbb E_0e^{tM}}{\mathbb E_0 e^{tY}}
       =\mathbb E_t e^{-K_{\mathcal E}(t)}
       \ge e^{-\mathbb E_t K_{\mathcal E}(t)}
\]
with the original compact law tilted by \(tY\), for which §4.82 proved the required mark moments. By (MISMATCH-SCALED-FRUSTRATION) and the real conditional range bound,
\(\mathbb E_t K_{\mathcal E}(t)\le
 C t^2\sum_b[\mathbb E_t\beta d_b^4+
 \beta^2\mathbb P_t(d_b>\delta)]\le C V t^2/\beta\).
The lower pressure difference follows from \(K_{\mathcal E}(t)\ge0\). This proves the second part of (FULL-RETAINED-FRUSTRATION-PRESSURE) without assuming any separate positivity or chessboard estimate for the law tilted by \(M\).

For the first part define \(v_b=e^{K_b(t)}-1\ge0\). At regular stars use \(e^x-1\le x e^x\), the boundedness of \(d_b\) and (MISMATCH-SCALED-FRUSTRATION). For a sufficiently small fixed \(|t|\) and a small fixed \(\alpha>0\) this gives
\[
 v_b\le (C t^2/\beta)e^{\alpha\beta d_b^2}.
\]
Indeed \(\beta d_b^4=(\beta d_b^2)^2/\beta\) and the exponential absorbs the square. At bad stars the centered variable has range at most \(C\beta\); the elementary inequality \(|e^x-1-x|\le x^2 e^{|x|}/2\) gives \(v_b\le C t^2\beta^2 e^{C|t|\beta}\). Since \(d_b>\delta\), the same displayed bound follows there after reducing \(|t|\), absorbing \(\beta^3 e^{C|t|\beta}\) in \(e^{\alpha\beta\delta^2}\) with a fixed prefactor. By the joint marked-set exponential bound,
\(\mathbb E_0 e^{\alpha\beta\sum_{b\in A}d_b^2}\le C^{|A|}\) for sufficiently small \(\alpha\). Expand the finite product:
\[
 \mathbb E_0 e^{t(Y-M)}
    =\mathbb E_0\prod_b(1+v_b)
    \le \sum_{A\subset\mathcal C}(Ct^2/\beta)^{|A|}
    \le \exp(C V t^2/\beta).
\]
This integrates all exterior configurations with their genuine Wilson weights. It gives in particular a coupling error \(C/\sqrt\beta\) for the two centered variables divided by \(\sqrt V\) in \(L^2\). The pressure of \(M\) can still have a narrow large curvature at the exact origin, as can the original unamplified pressure.

### 4.88 Exact Wilson entropy cost of a coherent twist on the full field (P)

The coherent regular face orbit of §4.81 changes a conditional mean. One can test a different mechanism directly on the full, typically rough Wilson field, without taking a rare face event. Fix arbitrary deterministic \(g_e\in SU(N)\) on all positively oriented links, and let \(\mu_g\) be the pushforward of the original \(\mu\) by \(U_e\mapsto g_e U_e\). For \(e=(x,\mu)\) choose a nearest center element \(z_e\in Z_N\), let \(d_e\) be its bi-invariant group distance from \(g_e\), and write \(B_z=\#\{p:z_{\partial p}\ne1\}\) for the count of plaquettes with nontrivial oriented center product. For \(\beta\) sufficiently large along the trajectory,
\[
 c_N\beta\left(\sum_e d_e^2+B_z\right)
 \le D(\mu_g\|\mu)\le C_N\beta\left(\sum_e d_e^2+B_z\right).
 \tag{WILSON-TWIST-ENTROPY}
\]
For \(Y\) either original unamplified comb, or any bounded deterministic mark of the same oriented row,
\[
 |\mathbb E_{\mu_g}Y_f-\mathbb E_\mu Y_f|
          \le C_N\|f\|_\infty\,D(\mu_g\|\mu).
 \tag{TYPICAL-TWIST-COMB}
\]
Thus a bounded-entropy coherent twist of the actual full law has only a bounded shift in its global comb mean. Its contrast after division by \(\sqrt V\) vanishes. The conclusion applies with arbitrary link-dependent directions, magnitudes, center windings and simultaneous long-wave shifts, as long as the twist is fixed independently of the sampled field.

Write \(\operatorname{tr}=\operatorname{Tr}/N\). Since the linkwise translation preserves product Haar, its exact relative entropy is \(\beta(\mathbb E S(gU)-\mathbb E S(U))\). For \(p=(x;\mu,\nu)\) with positive orientation, independent site gauge averaging gives
\[
 \mathbb E\,\operatorname{tr} (gU)_p =
 W(1,1)c_p,\qquad
 c_p=\operatorname{tr}(g_{x,\nu}^{-1}g_{x,\mu})\,
       \operatorname{tr}(g_{x+\hat\mu,\nu})\,
       \overline{\operatorname{tr}(g_{x+\hat\nu,\mu})}.
\]
Indeed at the two singleton corners the two inserted matrices are separately conjugated by independent Haar rotations, hence replaced by their normalized traces times the identity. At \(x\) the trace is cyclic and the two factors there are consecutive, giving their indicated joint trace. The fourth gauge cancels. The unshifted fundamental plaquette expectation is \(W(1,1)\), real by charge conjugation. Thus \(D=\beta N W(1,1)\sum_p(1-\Re c_p)\). FIRST gives \(W(1,1)\ge1-C/\beta\) at the cutoffs under consideration.

For \(g\in SU(N)\), \(1-|\operatorname{tr}g|\ge c\,\operatorname{dist}(g,Z_N)^2\). Its zeros are exactly the center by equality in the unitary trace bound; the expansion about any such element is nondegenerate quadratic because the tangent generators are traceless; compactness handles their complement. Consequently \(1-\Re c_p\ge1-|c_p|\) controls the squared distances of both singleton entries at that plaquette. Each positive link occurs as a singleton on a bounded positive number of plaquettes, so the sum controls \(\sum_e d_e^2\). If all four entries lie within a sufficiently small fixed distance of their chosen centers, then \(c_p\) is close to \(z_{\partial p}\). Each nontrivial center flux in this case costs at least a fixed positive \(1-\Re c_p\). The other flux plaquettes contain a link with \(d_e\) bounded below and have bounded incidence per such link. This proves the lower bound including \(B_z\). For the upper bound, write \(g_e=z_e\exp(A_e)\) with \(|A_e|=d_e\) in the fixed metric. Normalized traces of products of a bounded number of these exponentials have zero linear term at the identity by tracelessness. Therefore \(|c_p-z_{\partial p}|\le C\sum_{e\in p}d_e^2\), also globally by a bounded second-derivative estimate on the compact group. This proves (WILSON-TWIST-ENTROPY).

It remains to compute a response bound with the original observable. Replacing \(U\) first by \(zU\) changes its argument only on stencils meeting a plaquette with nontrivial center flux. Indeed all plaquette traces and their link-generator derivatives are invariant under the flat center multiplication on each such word. There are at most \(C B_z\) affected roots and the full root observable is bounded by \(C\beta\). The remaining rotation sends \(zU_e\) to \(\exp(A_e)zU_e\). The law of \(zU\) is still locally gauge invariant, even with nontrivial center plaquette flux. At any single oriented edge the expected first left derivative of a scalar gauge-invariant root in a deterministic Lie algebra direction vanishes: varying the site gauge at its base conjugates that direction by the defining group, and the adjoint representation of \(\mathfrak{su}(N)\) has no invariant vector. Along the simultaneous fixed orbit \(\exp(vA_e)zU_e\), the second derivative of each original \(r_b\) or \(h_b\) is bounded in modulus by \(C\beta\sum_{e\in D(b)}d_e^2\), since it is a smooth bounded-degree local group word and its stencil size is fixed. Taylor's formula, compact integration and the bounded number of stencils per edge give a total change at most \(C\|f\|_\infty\beta(\sum_e d_e^2+B_z)\). This proves (TYPICAL-TWIST-COMB).

The same upper bound for the mean difference holds for mixtures of deterministic twists with the mean of the individual entropy costs on its right, by linearity in the pushed-forward laws. It gives no entropy lower bound for the mixture and makes no claim for changes that depend on the sampled links. In particular it does not bound the pressure's optimal exponential tilt by \(Y\). The exact signed distant covariance remains necessary.

### 4.89 Full exterior action after exact comb decimation, including compact singular staples (P)

The first physical integration has an explicit positive effective action on all its spectator links. Work with the literal frustration tilt on \(|t|\le t_1\), and write \(s_b(U)=\sum_j(N-\Re\operatorname{Tr} U K_j)\), \(q_b(U)=h_b(U)/\beta\). For the fixed exterior \(\mathcal E\) define
\[
 \phi_b(\mathcal E,t)=\min_{U\in SU(N)}\{s_b(U)-t q_b(U)\},\qquad
 a_{b,\beta}(\mathcal E,t)=\beta^{d_G/2}
       e^{\beta\phi_b(\mathcal E,t)}
       \int_{SU(N)}e^{-\beta(s_b(U)-tq_b(U))}\,dU .
\]
At \(t=0\) the actual minimum is \(\phi_b=d_b^2/2\). Every plaquette meeting the comb belongs to exactly one star; let \(S_{\rm rest}\) include all the others. The exact original tilted exterior law \(\nu_t\) has density, up to its normalization, relative to exterior product Haar
\[
 \exp[-\beta(S_{\rm rest}+\textstyle\sum_b\phi_b(\mathcal E,t))]
              \prod_b a_{b,\beta}(\mathcal E,t).
 \tag{EXACT-DECIMATED-ACTION}
\]
For comparison define \(\nu_t^{\rm min}\) by the same normalized expression with the product of \(a\)'s omitted. This second law is positive on the whole compact exterior. All minima here are global minima of a one-link problem. A measurable selecting map is unnecessary for this definition.

Uniformly for every exterior, including degenerate minima,
\(c_N\le a_{b,\beta}\le \beta^{d_G/2}\) at \(\beta\ge1\). The upper bound follows by the definition of a minimum. The real group phase has a uniform Hessian bound and its gradient vanishes at any minimizer. A group ball of radius \(c/\sqrt\beta\) at that point has Haar mass at least \(c'\beta^{-d_G/2}\) and exponent within a fixed constant of the minimum, proving the lower bound. On the regular star of §4.86 the minimizer \(U_t^*\) is unique in the raised chart. One has
\[
 \left|\log\frac{a_{b,\beta}(\mathcal E,t)}
                    {a_{b,\beta}(I,t)}\right|\le C d_b^2,\qquad
 \big|m_{b,t}-\beta q_b(U_t^*)\big|\le C d_b^2 .
 \tag{REGULAR-DECIMATED-ROWS}
\]
Here \(I\) denotes six equal unit staples after the common translation; \(a_{b,\beta}(I,t)\) is independent of \(t\) because the frustration vanishes identically on that star. For the first inequality, rotate the six staples to \(\|V K_j-I\|\le d_b\). The uniform one-link saddle proof of §4.86 applies with these six near-identity Lie algebra coordinates also complex on a fixed ball. Indeed the entire exponent and Haar form are analytic in those parameters, the exterior gap and steep Gaussian contour have uniform margins there, and after extracting the analytic critical value the remaining determinant and normalized compact remainder have bounded nonzero modulus on a smaller ball. Thus the log of this extracted factor has a uniform Hessian in the real staple coordinates by Cauchy. At the identity the first jet in each staple Lie algebra slot vanishes by common conjugation invariance and tracelessness. This proves the first estimate. For large \(\beta\) the contour yields these bounds directly. A compact bounded initial \(\beta\) interval is handled by continuity near the identity and the positive real normalizer. For the second inequality differentiate the log of the one-link normalizer in the real source. On a regular star differentiation of the critical scalar gives \(\beta q_b(U_t^*)\) by stationarity. In the scaled parameter \(t d_b^2\) the determinant, Jacobian and analytic relative remainder have bounded first derivative on their fixed common disc by §4.87. This supplies exactly \(C d_b^2\) for the remaining unscaled derivative. In particular at \(t=0\) the physical star gradient \(\sum_i F_{b,i}(U_0^*)\) vanishes, so its leading retained source is exactly \(\beta\sum_i|F_{b,i}(U_0^*)|^2\).

Put \(R_b=\log(a_{b,\beta}(\mathcal E,t)/a_{b,\beta}(I,t))\) and \(R=\sum_b R_b\). Then the actual full tilted law satisfies for any fixed \(u_0<\infty\)
\[
 \log\mathbb E_{\nu_t}\exp\bigl(|u|\textstyle\sum_b|R_b|\bigr)
       \le C_{N,u_0} |u| V/\beta,\qquad |u|\le u_0 .
 \tag{DECIMATED-DETERMINANT-MOMENT}
\]
To verify it choose the small \(\alpha\) of the tilted marked-set exponential. On regular stars \(e^{|u||R_b|}-1\le(C_{u_0}|u|/\beta)e^{\alpha\beta d_b^2}\), using (REGULAR-DECIMATED-ROWS) and absorbing \(\beta d_b^2\). On the complement \(|R_b|\le C(1+\log\beta)\) by the uniform compact bounds, and \(d_b>\delta\); any fixed polynomial factor in \(\beta\) is absorbed by \(e^{\alpha\beta\delta^2}\) with an adjusted constant. The same upper bound therefore holds on every exterior. Expand the product over marked sites and use \(\mathbb E_t e^{\alpha\beta\sum_{b\in A}d_b^2}\le C^{|A|}\) as in §4.87. This proves the claim including the full prefactor product on correlated exteriors.

In particular the two actual finite-volume normalizations in (EXACT-DECIMATED-ACTION), after extracting the constant \(a_{b,\beta}(I,t)\) per marked site, differ in their log divided by \(V\) by at most \(C/\beta\). Both relative entropies satisfy
\[
 D(\nu_t\|\nu_t^{\rm min})+D(\nu_t^{\rm min}\|\nu_t)\le C V/\beta .
 \tag{DECIMATED-ENTROPY}
\]
Indeed \(\nu_t^{\rm min}/\nu_t=e^{-R}/\mathbb E_{\nu_t}e^{-R}\). Put \(F(v)=\log\mathbb E_{\nu_t}e^{vR}\); the moment estimate and Jensen give \(|F(v)|\le C V/\beta\) for \(|v|\le2\), and \(\mathbb E_{\nu_t}|R|\le CV/\beta\). The first entropy bound follows at once. For the reverse entropy use \(-F'(-1)-F(-1)\le F(-2)-2F(-1)\) by convexity. These are pressure and entropy bounds per site. They need not compare the variances of the two laws uniformly. The exact source \(\phi_b(\mathcal E,t)\) at degenerate staples can even have different one-sided derivatives when there is a family of minimizing links with different frustration values. Formula (EXACT-DECIMATED-ACTION) retains each compensating factor in the true law.

This gives an all-exterior next integration target with the actual action and the actual retained source. Its determinant correction has a uniformly small pressure cost and a real regular source row. The connected variance of that retained source under the original marginal remains open.

### 4.90 The actual first exterior coupling and frustration rows through one loop (P)

At \(t=0\) on a regular star let \(U^*=U_0^*\), \(\phi=d_b^2/2\), \(q_*=q_b(U^*)\), with \(\operatorname{Tr}(T_A T_B)=\tau\delta_{AB}\) and \(d_G=N^2-1\). Both lower coefficients of the actual one-link integration are explicit:
\[
 \begin{aligned}
 R_b&=\frac{N^2-1}{12N}\,\phi
             + O_N(d_b^4+d_b^2/\beta),\\
 m_{b,0}&=\left(\beta-\frac{N^2-2}{12N}\right)q_*
             + O_N(d_b^4+d_b^2/\beta).
 \end{aligned}
 \tag{ONE-STAR-LOWER-ROWS}
\]
Thus after extraction of the vacuum constant the real effective star action has inverse coupling \(\beta-(N^2-1)/(12N)\) multiplying \(\phi\). The retained frustration multiplying \(q_*\) has the distinct coefficient in the second line. These are coefficients of this particular exact comb integration.

Translate to \(U=\exp(iX)U^*\) and let \(M_*=\sum_j U^*K_j\). Each \(U^*K_j-I\) has size at most \(d_b\). Vanishing of the full star gradient gives \(M_*=H_*+i\lambda I\), \(H_*\) Hermitian. Each factor is special unitary close to \(I\); its Hermitian part differs from \(I\) by \(O(d_b^2)\) and its trace imaginary part is \(O(d_b^3)\) by its traceless logarithm. Hence \(H_*-6I=O(d_b^2)\), \(\lambda=O(d_b^3)\) and \(\operatorname{Tr}(H_*-6I)=-\phi\). The translated Haar density \(j(X)\) is even. The action \(6N-\Re\operatorname{Tr} e^{iX}M_*\) has \(H_{AA}=\Re\operatorname{Tr}(T_A^2 M_*)\) in its Hessian; at the flat star \(H_0=6\tau I\). By \(\sum_A T_A^2=(d_G\tau/N) I\),
\[
 \operatorname{Tr}_{\mathfrak g}[H_0^{-1}(H-H_0)]
     =-\frac{d_G}{6N}\phi .
\]
Therefore \(-\frac12\log\det(H/H_0)=d_G\phi/(12N)+O(d_b^4)\).

The remaining finite-\(\beta\) determinant correction gains a factor \(d_b^2\) even at arbitrarily small mismatch. Regard the translated phase as a function of \(H_*-6I\) and scalar \(\lambda\) on a fixed small complex ball. Its critical coordinate stays zero since the linear term in any traceless \(X\) vanishes throughout this family; complexify the real-linear expression in these parameters. After extracting the critical scalar, Gaussian determinant and Haar density at zero, the relative integral is \(1+O(1/\beta)\) uniformly holomorphic. On the Gaussian scale subtract the cubic term times the centered Gaussian. Its integral over the centered real ball vanishes also for complex symmetric Hessian. The quartic Taylor remainder, square of the cubic and even Haar Jacobian cost \(C/\beta\) by Gaussian moment domination on a smaller ball with quadratic reserve. The complement has a uniform gap. Cauchy gives derivative \(O(1/\beta)\) of the normalized log remainder. Its difference from the flat remainder is therefore \(O(d_b^2/\beta)\), proving the first row.

For \(d_b>0\) the same parity estimate holds after moving the saddle under \(w=t d_b^2\) using the uniformly bounded word \(q_b/d_b^2\) of §4.87. A linear Haar term at the moving saddle also integrates to zero against the centered Gaussian, with its cubic cross term costing \(O(1/\beta)\). The remainder derivative at \(t=0\) is \(O(d_b^2/\beta)\). In translated coordinates the saddle variation is \(a'=H^{-1}\nabla q_b(0)=O(d_b^2)\). The Haar derivative vanishes at zero. The third action jet is \(O(d_b^3)\): for one Hermitian \(X\) the cubic trace against \(H_*\) is purely imaginary, and only \(i\lambda I\) contributes; polarize to obtain all entries. Differentiation of the determinant consequently gives
\[
 -\tfrac12\operatorname{Tr}(H^{-1}\partial_t H(t)|_0)
   =\frac{1}{12\tau}\Delta_G q_b(0)+O(d_b^4).
\]
Indeed \(H'(0)=S_b'''[a']-q_b''\) in the fixed coordinates and \(H^{-1}=(6\tau)^{-1}I+O(d_b^2)\). At zero the sum of diagonal exponential-coordinate second derivatives is the generator Casimir.

For a pair of matchings form their staple-sum difference \(A=iB+C\) at \(U^*\), with \(B,C\) Hermitian and \(C=O(d_b^2)\). Its contribution before the pair factor \(1/3\) is \(q_A(X)=\sum_a f_a(X)^2,\ f_a(X)=\Re\operatorname{Tr}(iT_a e^{iX} A)\), up to a common sign immaterial for squares. Each fundamental coefficient has \(\Delta_G f_a=-C_F f_a,\ C_F=d_G\tau/N\). At zero its derivative in direction \(c\) is \(-\Re\operatorname{Tr}(T_a T_c A)\). Its \(iB\) part is \((2i)^{-1}\operatorname{Tr}([T_a,T_c]B)\), antisymmetric in \(a,c\); the \(C\) part is symmetric. Their cross sum vanishes. For \([T_a,T_c]=i f_{acj}T_j\) one has \(\sum_{a,c} f_{acj} f_{ack}=2N\tau\delta_{jk}\), by expanding \(\sum_a[T_a,[T_a,T_j]]\) with \(\sum_a T_a X T_a=\tau(\operatorname{Tr}X\, I-X/N)\). Hence the \(iB\) derivative squares sum to \(N\tau q_A(0)/2\); the \(C\) squares cost \(O(d_b^4)\). The Casimir product rule gives
\[
 \Delta_G q_b(0)=(-2C_F+N\tau)q_*+O(d_b^4)
                =\tau(2/N-N)q_*+O(d_b^4).
\]
Combining the determinant coefficient and critical derivative \(\beta q_*\) proves the second row. At \(d_b=0\) it holds exactly.

The extracted action remainder now has true full pressure cost \(O(V/\beta^2)\). At regular stars \(e^{|u||R_b-d_G\phi/(12N)|}-1\le(C_{u_0}|u|/\beta^2)e^{\alpha\beta d_b^2}\) for bounded \(|u|\), absorbing \((\beta d_b^2)^2+\beta d_b^2\). On bad stars use \(O(1+\log\beta)\) and \(d_b>\delta\). The product expansion of §4.89 applies. Both relative entropies per site between the true exterior law and the law with the extracted star coefficient \(\beta-d_G/(12N)\) are \(O(1/\beta^2)\) by the same convexity argument.

For the retained source pick any measurable minimizing \(U^*\) on bad exteriors (a Borel choice exists by compactness and continuity), and put \(M^\sharp=(\beta-(N^2-2)/(12N))\sum_b q_b(U^*)\). The true \(M=\sum_b m_{b,0}\) is a sum of reflection-covariant real scalars on the same eight-site cells: the normalized compact integration at each root respects the star reflection. Pointwise \(|m_{b,0}|\le C\beta d_b^2\le C\beta e_b\) by the force differences. Thus the law tilted by small real \(tM\) has the same reflection-positive cell factorization and marked-set exponential as in §4.82, by the positive action comparison and dissemination argument. No such property is needed for an arbitrary measurable minimizer. On regular stars \(|m_{b,0}-m^\sharp_b|=O(d_b^4+d_b^2/\beta)\). On bad stars it is at most \(C\beta d_b^2\). For sufficiently small \(|u|\),
\(e^{|u||m_{b,0}-m^\sharp_b|}-1\le(C|u|/\beta^2)e^{\alpha\beta d_b^2}\): on the bad set the unused exponent absorbs the polynomial factor since \(d_b>\delta\). Expand the product under the \(tM\) tilt and use Jensen for the lower logarithmic bound. For small real \(t\),
\[
 \left|V^{-1}\log\frac{\mathbb E_0 e^{tM^\sharp}}
                           {\mathbb E_0 e^{tM}}\right|
       \le C |t|/\beta^2 .
 \tag{ONE-STAR-SOURCE-PRESSURE}
\]
With §4.87 this is a real-pressure approximation to the original frustration comb with error \(C(|t|/\beta^2+t^2/\beta)\) per site. These comparisons have yet to control the curvature at the prescribed source zero.

### 4.91 A second power of the coupling in the full frustration noise (P)

There is another exact cancellation in the one-link conditional source. At a regular exterior and its true unperturbed minimum \(U^*\) use the pair decomposition \(A=iB+C\) of §4.90. For a Hermitian direction \(Z\), the derivative of \(\sum_a f_a^2\) at zero has no contribution quadratic in \(B\). Indeed \(f_a(0)=-\operatorname{Tr}(T_a B)\), and the part of \(D_Z f_a\) from \(iB\) is \((2i)^{-1}\operatorname{Tr}(T_a[Z,B])\). The contracted product is proportional to \(\operatorname{Tr} B_0[Z,B]=0\), with \(B_0\) its traceless part. Only the Hermitian part \(C=O(d_b^2)\) remains, multiplied by \(f_a(0)=O(d_b)\). In particular
\[
 |\nabla q_b(U^*)|\le C d_b^3 .
\]
On the fixed chart all other derivatives of \(q_b\) remain \(O(d_b^2)\). In the scaled source \(w=z d_b^2\) of §4.87 the gradient of \(q_b/d_b^2\) is \(O(d_b)\) at the unperturbed minimum. Its critical point moves \(O(|w|d_b)\) on a fixed small \(w\)-disc: solve the stationarity equation by the uniform Hessian bound there, or integrate \(a'(w)=H(w)^{-1}\nabla(q_b/d_b^2)(a(w))\) and use the bounded Hessian of \(q_b/d_b^2\). The gradient at the moving point is consequently \(O(d_b)\). The second derivative of the critical exponent in \(w\) is \(O(\beta d_b^2)\), and the analytic determinant, Jacobian and relative compact remainder have uniformly bounded second derivatives there. Returning to \(z\), the centered conditional log satisfies the sharper
\[
 |K_b(z)|\le C |z|^2(\beta d_b^6+d_b^4),
           \qquad d_b\le\delta,\quad |z|d_b^2\le c .
 \tag{STAR-FRUSTRATION-CANCELLATION}
\]
The same bound about any fixed small real tilt uses the same scaled disc and centers at that tilt's exact conditional mean.

For the actual frustration comb, both right sides of (FULL-RETAINED-FRUSTRATION-PRESSURE) improve to \(C V t^2/\beta^2\) for the unnormalized logs, and
\[
 \operatorname{Var}_0(Y)-\operatorname{Var}_0(M)
              \le C V/\beta^2 .
 \tag{SHARP-FRUSTRATION-NOISE}
\]
Indeed \(\beta d_b^6+d_b^4=[(\beta d_b^2)^3+(\beta d_b^2)^2]/\beta^2\). In the product argument, on regular stars use (STAR-FRUSTRATION-CANCELLATION) to obtain \(e^{K_b(t)}-1\le (C t^2/\beta^2)e^{\alpha\beta d_b^2}\), shrinking \(t_1\) since \(d_b\) is bounded. On bad stars the same bound follows from the centered compact range as in §4.87, absorbing one additional polynomial power with \(d_b>\delta\). The true small real tilted moments prove the sharper Jensen pressure comparison as well. At fixed \(m\ge2\), the regular contribution to the true annealed conditional cumulant is bounded by \(C^m m!(m+1)!\beta^{-m}\), as follows by Cauchy on the scaled disc and the marked moments. The bad contribution \(C^m m!\beta^m e^{-c\beta}\) is still present.

This gain works through any positive full-law history filtration. For nested conditional projections, including their terminal projection on centered variables, the sum of squared \(L^2\) differences between all martingale increments for \(Y\) and \(M\) is at most \(C V/\beta^2\) by orthogonality. No shape-by-shape absolute estimates are required for that difference. Also, for every law \(\nu\ll\mu\) with finite relative entropy \(D\), the variational entropy inequality and the sharper global noise log moment give
\[
 |\mathbb E_\nu(Y-M)|\le C\left(\sqrt{VD}/\beta+D\right).
\]
For a true event of probability \(p\), take \(D=\log(1/p)\). The claim concerns the change carried by the discarded noise; \(\mathbb E_\nu M-\mathbb E_\mu M\) is retained. With (ONE-STAR-SOURCE-PRESSURE), the total per-site real-pressure error in replacing \(Y\) by \(M^\sharp\) is \(C(|t|+t^2)/\beta^2\).

### 4.92 Local Wilson curl limit and the positive coefficient of the discarded noise (P)

At any fixed fine-lattice stencil, the original canonical plaquette logarithms \((ig)^{-1}\log U_p,\ g=\beta^{-1/2}\), transported along fixed finite paths to a common base point, converge jointly in moments along the reference trajectory to the corresponding infinite-lattice Gaussian curls. Each plaquette uses its original orientation, including reversal or transport when required. The Gaussian covariance on two-forms is \(\tau^{-1}\) times the orthogonal projection onto the closure of compact lattice curls, separately in the \(d_G\) orthonormal colors. Common conjugation is interpreted in the original Wilson law.

Here are the boundary and gauge details for this additional limit. Put the whole finite stencil deep in a cell with \(s\to\infty,\ s\le\beta^{1/200}\). On the relative doubled cell of §4.70, the constant two-form component of \(\widetilde F\) vanishes: for any orientation there is a reflection across a coordinate absent from its two indices, under which its relative extension is odd. Consequently the harmonic curvature itself satisfies \(\widetilde F=d^*\Delta^{-1}d\widetilde F\). The source \(d\widetilde F\) is the same signed boundary curvature as in §4.70. The kernel with one derivative in the numerator has size \(C[(1+d)^{-3}+s^{-3}]\), and its first tangential difference \(C[(1+d)^{-4}+s^{-4}]\). The dyadic proof of §4.72 applies with symbol of order \(-1\), the zero frequency omitted. At a deep target, integration by parts on each fixed face thus gives a total absolute coefficient \(C(s^3s^{-4}+s^2s^{-3})=C/s\) on the canonical boundary links, including the ridges. The actual thin-rectangle estimate \(\|D_e\|_2\le C\sqrt s\) proves \(\|1_{\rm good}(d E D)_p\|_2\le C s^{-1/2}\). This removes the random conditional mean even for the curl without an extra derivative.

The centered Gaussian Dirichlet curl covariance is the signed relative-image projection on the doubled torus. Its periodic multiplier is the ordinary curl projection with its zeroth frequency omitted. The periodic kernel at fixed displacement converges by bounded Riemann sums to the full infinite projection. Nonidentity deep images have modulus \(O(s^{-4})\) by the bounded order-zero symbol estimate of §4.72. Gauge gradients are annihilated, so the tree used in computing the Gaussian does not affect this covariance. The compact conditional comparison of §§4.69,4.85 holds on the common canonical window; its normalized density has relative error \(o(1)\), with the entire tail integrated. Any fixed short word giving a based plaquette differs in canonical log from its linear curl by \(O(gT^2)=o(1)\) there, including its path transport. For bounded continuous tests of these vectors one may first average the test under common Haar conjugation. The resulting scalar conditional expectation is invariant under every change of the boundary representative; thus the full coordinate tree in the deep bound need not be chosen from the face sigma-field. The original Wilson law is invariant under gauge rotation at the common base, and the limiting joint Gaussian is color invariant, so this Haar averaging does not change either unconditional expectation. The true marked exponential bounds on the fixed plaquettes give all higher absolute moments of their canonical logarithms, by a bounded logarithm convention away from identity. These bounds yield uniform integrability and prove the stated moment convergence.

In particular there is a finite explicit constant \(\gamma_N>0\) such that
\[
 \lim_{\beta\to\infty}
  \frac{\beta^2}{|\mathcal C|}
       [\operatorname{Var}(Y^h)-\operatorname{Var}(M)]=\gamma_N .
 \tag{SHARP-STAR-CONSTANT}
\]
The constant is a Gaussian polynomial expectation specified below. This proves exact order of the microscopic noise, including its sign in the full susceptibility decomposition. It does not assign that coefficient to the retained variance.

For a marked temporal link let \(X_j\), \(1\le j\le6\), be the six Gaussian limits of \((ig)^{-1}\log(U_b K_j)\), each plaquette based and oriented with \(b\) positive. Put \(D_j=X_j-\frac16\sum_k X_k\). The three pairs \(I_i\) are the two staples in each matching. For \(i<j\) set
\[
 B_{ij}=\sum_{k\in I_i}D_k-\sum_{k\in I_j}D_k,\qquad
 C_{ij}=-\tfrac12\Big(\sum_{k\in I_i}D_k^2-
                             \sum_{k\in I_j}D_k^2\Big).
\]
With \(A_{ij}\) the exact staple difference at \(U^*\), \(g^{-1}\Im A_{ij}\) and \(g^{-2}\Re A_{ij}\) converge jointly in moments to \(B_{ij}\) and \(C_{ij}\) on regular stars, taking them as zero otherwise. Here \(\Re,\Im\) on matrices mean Hermitian parts \((A+A^*)/2,(A-A^*)/(2i)\). Indeed relative to the actual \(U_b\), the minimizing rotation has log \(-ig\bar X_\beta+O(g^2\max_k |X_{k,\beta}|^2)\), where \(X_{k,\beta}\) are the actual six plaquette logs in canonical units and \(\bar X_\beta\) their mean. This follows by the critical equation and flat Hessian \(6\tau I\), or by linearizing the vanishing traceless anti-Hermitian part of the aggregate. Thus the individual rotated staple logs in canonical units converge to \(D_j\). The expansion of each unitary Hermitian part begins with \(-g^2 D_j^2/2\). The moment passage follows by truncating \(\max|X_{k,\beta}|\), using the rough bounds on the scaled parts by \(C d_b/g\) and \(C d_b^2/g^2\) and the true marked moments. All group words and orientations here are those of the original star.

Let \(Z=\sum_c Z_c T_c\) with \(Z_c\) independent centered normals of variance \(\sigma^2=(6\tau)^{-1}\), independent of the above Gaussian stencil. For a pair \(B=B_{ij},C=C_{ij}\) define the following real polynomial and sum it over matching pairs with weight \(1/3\):
\[
 \begin{aligned}
 L_{B,C}(Z)
 &=\sum_a \bigg[
       \big(\Im\operatorname{Tr}(T_a ZB)\big)^2
       -2\operatorname{Tr}(T_a B)
          \left(-\Re\operatorname{Tr}(T_a Z C)
                    +\tfrac12\Re\operatorname{Tr}(T_a Z^2 B)\right)
        \bigg],\\
 L(Z)&=\tfrac13\sum_{i<j} L_{B_{ij},C_{ij}}(Z),\qquad
 \gamma_N=\mathbb E\,\operatorname{Var}_Z L(Z).
 \end{aligned}
\]
For verification, evaluate each force coefficient at \(U=\exp(igZ)U^*\), writing the exact pair difference as \(A=i g B_\beta+g^2 C_\beta\). Its constant term is \(-g\operatorname{Tr}(T_a B_\beta)\). The linear change is \(g^2\Im\operatorname{Tr}(T_a ZB_\beta)-g^3\Re\operatorname{Tr}(T_a ZC_\beta)\), and the quadratic change at the required degree is \(g^3\Re\operatorname{Tr}(T_a Z^2 B_\beta)/2\). Squaring, the \(g^3\) term cancels after summing \(a\), by §4.91. Thus \(g^{-4}[q_b(U)-q_*]\) tends to \(L(Z)\). Under the true conditional law the centered canonical coordinate at \(U^*\) has bounded fixed moments on regular stars, and its conditional polynomial moments tend to those of this independent \(Z\) whenever \(d_b\to0\) as \(\beta\to\infty\). This follows directly from the translated compact saddle: the Hessian tends to \(6\tau I\), the quartic and cubic Taylor tails are Gaussian dominated, and all compact exterior tails are uniform. For moment convergence of the displayed polynomial use the finite-order word Taylor remainder on bounded \(Z,B_\beta,C_\beta\), followed by their higher moments. More explicitly the scaled difference is bounded on the local chart by \(C[(d_b/g)^3|Z|+(d_b/g)^2|Z|^2]\) using the gradient and Hessian bounds of §4.91 and Taylor along the segment. The true omitted compact tail and nonregular stars remain negligible after any fixed polynomial \(\beta\) factor. Conditional centering subtracts \(\mathbb E_Z L\) in the limit; the conditional first and second moments converge with the random external coefficients by the same truncation. Since \(\beta(h_b-m_{b,0})\) is precisely this centered scaled difference, conditional independence and Wilson translation symmetry prove (SHARP-STAR-CONSTANT).

To see strict positivity, put \(Q=\frac13\sum_{i<j,a}(\operatorname{Tr}(T_a B_{ij}))^2\). The quadratic part of \(L\) has scalar Laplacian \(\tau(2/N-N)Q\) by the computation in §4.90 on its leading homogeneous coefficients. This is nonzero whenever \(Q>0\). At least one matching difference has a strictly positive color variance in the infinite free curl law: vary a spatial link of one chosen temporal plaquette on the lower time slice that belongs to no other plaquette in that pair difference. Its compactly supported curl has a nonzero pairing with the difference. Thus \(\mathbb E Q>0\), and the nondegenerate Gaussian \(Z\) gives \(\mathbb E\operatorname{Var}_Z L>0\).

The mixed ordinary/frustration contact has a signed subleading coefficient as well:
\[
 \lim_{\beta\to\infty}\beta\,\mathbb E\operatorname{Cov}
             (r_b,h_b\mid\mathcal E)
     =\frac{\tau}{3}(2/N-N)\,\mathbb E Q <0 .
 \tag{SIGNED-STAR-CROSS}
\]
In fact the centered ordinary innovation tends in joint second moments to \(12\tau^2(|Z|_{\mathrm{coord}}^2-d_G\sigma^2)\), using the three equal link-coordinate first variations and the vanishing total force at \(U^*\) as in §4.57. The Casimir variation vanishes in that limit. Combine it with the preceding centered \(L\), then integrate by parts in \(Z\): \(\operatorname{Cov}_Z(|Z|_{\mathrm{coord}}^2,L)=\sigma^4\mathbb E_Z\Delta_Z L\). This yields the displayed coefficient. The remaining signed covariance of the retained exterior is common to the two observables and has not been replaced by this local contact.

### 4.93 Exact second comb innovation with its retained exterior contribution (P)

In the three-link integration of §4.61 the lower bound (SECOND-COMB-INNOVATION) can now be replaced by an explicit strict asymptotic. Keep its second sublattice \(\mathcal D\) and let \(J_2=\mathbb E\operatorname{Var}(M\mid\mathcal E')\). Enumerate the matched directions at either \(b_-,b_+\) with the central neighbor \(d\) in direction 1. Set
\[
 a=(-2/3,1/3,1/3),\quad u=(a,a),\quad c_d=3/(17\tau).
\]
Let \(G\) be the per-color six-by-six full infinite covariance of the linear matching forces \((H_i A)_{b_\pm}\), for Gaussian curl norm \(\tau\|dA\|^2/2\). Then
\[
 \lim_{\beta\to\infty}\frac{J_2}{|\mathcal D|}
   =2\tau^4d_G\,[\,2 c_d\,u^T G u-c_d^2 |u|^4\,] .
 \tag{SECOND-COMB-EXACT}
\]
In particular the noncentral exterior adds at least \(3\tau^2d_G/136\) above the former lower constant \(32\tau^2d_G/289\). The same \(J_2\) enters the ordinary and frustration towers, because their first retained means are equal at zero source.

For a single three-link cell, use the actual pair frustration \(F=h_{b_-}+h_{b_+}\). Its first-link conditional variance after revealing \(d\) is \(O(\beta^{-2})\) on average by §4.91. The other isolated first-comb means are constant when varying \(d\), so the second innovation equals the sum of the triple conditional variances minus these first noises. Let \(\mathcal B\) denote the six actual color-force vectors \(F_{b,i}/(g\tau)\). Then \(F=\tau^2\mathcal B^T Q\mathcal B\) exactly, with \(Q\) the matching difference projection at both roots and identity on colors. Use a common base point for the two sets of colors, transporting along fixed spatial edges on the lower time slice, which are in the fixed exterior of the temporal stars. This changes no contracted quadratic. Their full second moment tends to \(G\otimes I_{d_G}\) by the local curl theorem, the first-jet expansion of the matched forces and color symmetry. Each star is in a finite contractible rectangle with the exact based exterior gauge of §4.61.

Condition on the exterior of the three links. On its good canonical chart, the original conditional Gaussian comparison of §4.61 applies to every fixed polynomial jet of these forces. At bounded canonical exteriors the two neighbor variations change each of their three plane forces by twice their own link coordinate, which \(Q\) kills. The central coordinate changes the direction-1 force by minus that coordinate at both roots. After \(Q\) the resulting projected fluctuation is \(u\) times this central coordinate. Its variance at fixed exterior is \(c_d I_{d_G}\), the Schur complement of the displayed three-link precision in §4.61. Thus the projected conditional covariance is \(c_duu^T\otimes I_{d_G}\). Pinning the two selected links while varying \(d\) would give a different variance. To pass to the unconditional limit, restrict first to bounded canonical exterior coordinates in the finite tree chart of §4.61. Their true tail is controlled by the fixed-stencil marked exponential moments. On that chart the compact Gaussian polynomial comparison is uniform at each bound; send the bound to infinity using the higher full moments. Relative spatial transports between the two roots are within the canonical small chart there. Equivalently one may Haar-average common-frame color contractions as in §4.92.

For a Gaussian quadratic with mean \(m\) and covariance \(C=c_duu^T\otimes I_{d_G}\) on the projected forces, its conditional variance is \(\tau^4[2\operatorname{Tr}C^2+4m^T C m]\). The mean term is not zero on fixed exterior data. Its needed averaged second moment is determined by the full covariance tower just computed: projected unconditional second moment tends to \(QGQ\otimes I_{d_G}\), and the conditional covariance to \(C\). This argument requires no assumption that the conditional mean is independent of the Wilson exterior. Subtracting the first noises and using translation symmetry now gives (SECOND-COMB-EXACT).

For an explicit check on all Fourier conventions write \(a_\mu(q)=4\sin^2(q_\mu/2)\), \(s(q)=\sum_\mu a_\mu(q)\). Then
\[
 \tau u^TGu=\int_{[-\pi,\pi]^4}\frac{d^4q}{(2\pi)^4}
      |1+e^{2iq_1}|^2
      \frac{(-2a_1+a_2+a_3)^2+a_0(4a_1+a_2+a_3)}
           {9s(q)} .
\]
The integrand at zero is defined by continuity. The doubled phase is the fine displacement of the two marked bonds. To lower-bound the noncentral term rigorously, write \(\ell=B^*u\), where \(B\) is the linear matching-force map restricted to the two roots. The quadratic form \(u^T(G-c_duu^T)u\) equals \(1/\tau\) times the squared dual-curl distance from \(\ell\) to the span of \((d^*d)v\) with \(v\) supported on the three free temporal links. This is the Gaussian energy projection, and \(u\) lies in the range of \(Q\). In Fourier variables the dual-curl norm of each such residual is at least its ordinary \(\ell^2\) norm divided by four since \(d^*d\preceq16I\) and the residual is transverse. On the two outer temporal neighbors \(b_- -e_1,\ b_-+e_2\), the entries of \(\ell\) are \(-a_1,-a_2\) with \(a_i\) now denoting the entries of the fixed vector \(a\). Those of \((d^*d)v\) both equal \(-v_{b_-}\). The sum of the two squared residuals is at least \(1/2\). Hence \(u^T(G-c_duu^T)u\ge1/(32\tau)\). With \(|u|^2=4/3\), its contribution \(4\tau^4d_G c_du^T(G-c_duu^T)u\) gives the stated strict improvement. This is a signed constant-mode calculation for the genuine second integration; later retained exterior variation is still present.

### 4.94 Testing a face-projection contraction on typical rough Wilson fields (P)

A scale iteration cannot assume a uniform contraction of conditional expectation on the whole space of quadratic curvature observables. This can be tested directly on the original Wilson law and on arbitrarily many fixed shifted grids, without prescribing coherent exterior values. Let \(S\asymp\beta^{1/200}\), \(R\asymp S^{1/50}\), and \(s\to\infty,\ s/R\to0\). Round to compatible lattice boxes as in §4.71. Choose any fixed finite number of translated \(s\)-face partitions with comparable even cell sides, and let \(P_j\) be conditional expectation onto their tangential link sigma-fields on the full Wilson space. Then there are actual centered gauge-invariant quadratic observables \(X_R\) with
\[
 \liminf\|X_R\|_2>0,\qquad
 \max_j\|(I-P_j)X_R\|_2\longrightarrow0 .
 \tag{ROUGH-FACE-SLOW-SECTOR}
\]
In particular \(\|P_1\cdots P_m X_R\|_2/\|X_R\|_2\to1\) for each fixed \(m\). The observables come from smooth averages of ordinary ultraviolet plaquette fluctuations at their typical Wilson size. This establishes a failure of the indicated general annealed \(L^2\) contraction, independent of the special deterministic face profiles in §4.81.

Choose real nonzero \(f\in C_c^\infty(\mathbb R^4)\) on a fixed coordinate patch. For each spatial \(12\)-plaquette \(p\) rooted at \(x\) in the rescaled patch, transport its canonical logarithm \((ig)^{-1}\log U_p\) along a fixed path of length \(O(R)\) to one base point. Let \(Z_R\) be the sum of these transported logs with scalar weights \(R^{-2}f(x/R)\), and set \(X_R=|Z_R|_{\rm coord}^2-\mathbb E|Z_R|_{\rm coord}^2\). The logarithm can be chosen conjugation-equivariantly away from a Haar-null branch boundary and extended measurably there. Its invariant norm square is well-defined. Place the patch deep in one true outer box of side comparable to \(S\). In its good column or tree chart all relevant link logs are at most \(gT,\ T=C S^8\log\beta\), and the conditional density has the Gaussian relative error of §4.69. Replacing a transported canonical plaquette by its linear curl in this chart costs \(C g R T^2\) per plaquette: the fixed plaquette word costs \(CgT^2\), and conjugating around a path with \(O(R)\) such links changes the canonical field by at most \(CgRT^2\). Thus \(Z_R\) differs from the linear curl smearing there by \(O(gR^3T^2)\). Its true compact tail, even with polynomially many terms, is superpolynomially suppressed in the full law. For invariant joint scalar tests these estimates may again be made in any chosen boundary representative, as in §4.92.

The conditional noncentral Gaussian curl mean at a deep plaquette has \(L^4\) norm \(O(S^{-1/6})\): §4.92 gave total boundary-link coefficient \(C/S\), and the true thin-rectangle interpolation gives \(O(S^{5/6})\) in \(L^4\) per link. Consequently the noncentral part of the smearing is \(O(R^2 S^{-1/6})=o(1)\) in \(L^4\). The relative Gaussian covariance converges to
\[
 v_f=\tau^{-1}\int_{\mathbb R^4}\frac{d^4k}{(2\pi)^4}
             |\widehat f(k)|^2\frac{k_1^2+k_2^2}{|k|^2}>0
\]
per orthonormal color. In fact the nonidentity deep images of the bounded curl-projection kernel cost \(O(R^4S^{-4})\) in the smeared covariance. In the ordinary periodic part use Fourier inversion: the lattice smearing has transform \(R^2\sum_{m\in\mathbb Z^4}\widehat f(R(p+2\pi m))\), with the chosen Fourier convention. Substitution \(k=Rp\) in the doubled periodic sum gives grid spacing \(O(R/S)\to0\), bounded multipliers converging off zero to the stated continuum projection and rapid decay from \(f\). The omitted single zero mode costs \(O((R/S)^4)\). These facts prove the limit by truncating the \(k\)-integral and then taking Riemann sums. The normalized-density error times any fixed fourth moment is negligible, either by Gaussian moment domination or the chart bound \(C(R^2T)^4\) times \(O(gS^{28}\log^3\beta)\). Hence \(\operatorname{Var}X_R\to 2d_G v_f^2>0\).

For a given smaller face grid define an explicit measurable approximation. Replace \(f(x/R)\) in each \(s\)-cell by its center value. On each planar \(12\) slice of that cell, take the canonical log of the Wilson rectangle around the whole \(12\)-rectangle, with consistent orientation. Its four sides are tangential links on the retained faces, including slices at fixed third and fourth coordinates lying within the cell. Transport each rectangle along retained skeleton links to a common skeleton vertex within the patch, at path cost \(O(R+s)\); apply the same normalization \(R^{-2}\) and sum all rectangles. Its squared norm \(\widehat X_{R,j}\) (centered by its own mean) is a measurable scalar on that grid. Linearized, the rectangle is exactly the sum of all linear plaquette curls in its slice by telescoping. At most \(C R^4/s^2\) rectangles are used; each untransported word costs \(C g s^2T^2\) in canonical units, and transport costs \(C g R s T^2\). Thus the normalized word and transport error is \(o(1)\), and this persists in fourth moments. Different grids can choose different reference vertices because only their gauge-invariant norm squares are compared. On the chart all of their spatial transports are within the indicated error of the same linear coordinate convention.

For the remaining difference of linear smearings the \(\ell^2\) norm of the normalized weights is \(O(s/R)\) by smoothness. The centered Dirichlet curl covariance has bounded norm, giving a Gaussian fourth-moment norm \(O(s/R)\). The noncentral cost is at most \(C R^2 S^{-1/6}s/R\). All compact-chart and Gaussian-tail errors tend to zero also for these words, by the polynomial bounds above and the marked bad-boundary estimates. We get \(\|X_R-\widehat X_{R,j}\|_2=o(1)\) by Cauchy–Schwarz and the bounded fourth moments of the two vectors. Orthogonal projection then gives (ROUGH-FACE-SLOW-SECTOR), and telescoping a finite product of norm-one projections gives its consequence. This proof concerns actual rough exterior fluctuations. It does not say that their projection onto the global comb carries a divergent susceptibility.

### 4.95 What the true comb sees in the slowly varying rough sector (P)

There is nonzero but suppressed coupling to the sector in §4.94. This can be checked with the same physical roots and the zero-frequency comb density, restricted for the calculation to the mesoscopic patch. Let \(w\ge0\) be smooth and compactly supported in that patch and
\(Y_{R,w}=\sum_{b\in\mathcal C}w(x_b/R)h_b\). Define \(\psi\) as the inverse continuum Fourier transform of
\(i k_0 k_1 k_2\,\widehat f(k)/|k|^2\); its sign depends only on the chosen plaquette orientation and is immaterial below. Then
\[
 \lim R^2\operatorname{Cov}_\mu(Y_{R,w},X_R)
     = \frac{d_G}{4}\int_{\mathbb R^4}
                     w(x)\,[|\psi(x)|^2+|-\psi(x)|^2]\,d^4x .
 \tag{SLOW-SECTOR-COMB-OVERLAP}
\]
Choose \(f,w\) with positive right side. For the actual geometry of any one smaller grid \(j\) in §4.94 there are constants independent of \(s,R\) with
\[
 \frac{c}{R^2}\le
 \operatorname{Cov}_\mu(P_jY_{R,w},\widehat X_{R,j})
 =\operatorname{Cov}_\mu(Y_{R,w},\widehat X_{R,j})
 \le \frac{C s}{R^2}.
 \tag{RETAINED-SLOW-OVERLAP}
\]
The upper bound allows the extra fluctuations introduced by abrupt cellwise replacement of a smooth smearing. Both computations use the true annealed Wilson law.

In the outer Gaussian comparison write \(\mathcal B_{bi}=H_i A_b\) for the three directional temporal forces, and \(Z_{f}\) for the linear magnetic curl smearing. On the infinite lattice the per-color cross symbol between a temporal \(H_i A\) and the spatial \(12\)-curl is zero for \(i=3\). Up to elementary unit-cell phases, the two others have opposite signs and modulus
\[
 \tau^{-1}\frac{|\widehat q_0\widehat q_1\widehat q_2|}
                         {\sum_\mu|\widehat q_\mu|^2},
 \qquad \widehat q_\mu=e^{iq_\mu}-1 .
\]
Indeed contracting \(d_i^*d_i e_0\) with the \(12\)-curl row kills its time component and leaves only the direction-1 or direction-2 term. The sum of the three cross symbols is zero exactly: the full \(d^*d\) applied at a temporal edge has zero covariance with a purely spatial curl, by cancellation with the inverse on the transverse subspace. The frustration matching projection therefore acts as identity on this cross vector. The modulus bound \(C|\widehat q_0|\) holds for all momenta, including spatial aliases. Finite relative images at a deep root cost \(O(R^2 S^{-5})\) in the smeared cross covariance, using the order-one dyadic estimate as in §4.84. In the ordinary periodic part the Poisson-summed smearing computation in §4.94 now gives, uniformly on the fixed rescaled patch,
\[
 R^3\operatorname{Cov}_G(\mathcal B_{bi},Z_f)
  \ \longrightarrow\ \tau^{-1}(\psi(x_b/R),-\psi(x_b/R),0)_i
\]
up to one common sign. The color contraction of the two centered Gaussian squares is twice the squared cross covariance. The comb has density \(1/8\), so the true local sum, after scaling by \(R^2\), has precisely the coefficient in (SLOW-SECTOR-COMB-OVERLAP).

Here are error checks on this small covariance. All variables lie in one genuine box of side \(S\) with its complete compact boundary law. The largest product needed on the good outer chart is bounded by \(C R^8 T^4\) for the unapproximated linear force and curl squares. Multiplying by the density error \(C g S^{28}\log^3\beta\) gives \(o(R^{-2})\) for \(S\asymp\beta^{1/200}\) and \(R\asymp S^{1/50}\). The word Taylor and path-transport errors in §4.94 and the \(O(g T^3)\) local force-square error satisfy the same stronger bound after multiplication by the other polynomial factors (one may bound by \(C g R^{12}S^{60}\log^7\beta\)). Bad-event and compact-tail contributions remain superpolynomial. The good outer mean force has \(L^4\) norm \(O(S^{-7/6})\) per root, and the magnetic smearing mean has norm \(O(R^2 S^{-1/6})\). Hence the covariance of their squared conditional means costs at most \(C R^8 S^{-8/3}=o(R^{-2})\). The noncentral cross term in the inner Gaussian covariance has the two means times the centered force–curl cross covariance. Its absolute sum is \(o(R^{-2})\) even using the step-smearing norm \(C R\sqrt s\) for the sum of the absolute cross covariances on the patch, proved below. These estimates handle the true correlated exterior rather than replacing it by zero; their strong smallness is particular to the stated patch scale.

For (RETAINED-SLOW-OVERLAP) use the genuine skeleton rectangles of §4.94, whose linear smearing has the step weights \(f_{R,s}\), including the \(R^{-2}\) normalization. They satisfy
\(\|f_{R,s}-f_R\|_{\ell^2}\le C s/R\) and \(\|\partial_0 f_{R,s}\|_{\ell^2}\le C\sqrt s/R\). The latter follows from jumps of size at most \(C s R^{-3}\) on \(O(R^4/s)\) time-seam sites. The cross multiplier bound \(C|\widehat q_0|\) implies squared cross norm at all roots bounded by \(C s/R^2\); on \(O(R^4)\) patch roots its absolute sum is at most \(C R\sqrt s\). This proves the upper bound after the same compact and noncentral estimates.

For the positive lower bound take a smooth vector test \(\gamma\) compactly supported where \(w>0\), pairing nontrivially with \((\psi,-\psi,0)\). Put \(\alpha_b=R^{-2}\gamma(x_b/R)\) on the unit comb. The smooth force-to-curl limit gives \(|\sum_b\alpha_b\cdot\operatorname{Cov}(\mathcal B_b,Z_f)|\ge c/R\) at the linear Gaussian level. The step replacement costs \(O(s/R^2)\) in this pairing, because \(\|\partial_0\alpha\|_2\le C/R\) (there is no temporal subsampling in this actual comb), and the cross multiplier bounded by \(C|\widehat q_0|\) can put that derivative on the test. The finite periodic relative-image errors vanish at the indicated rate. Cauchy–Schwarz using \(\sum|\alpha_b|^2/w(x_b/R)\le C\) therefore gives squared cross sum at least \(c/R^2\). The actual expansion errors above are \(o(R^{-2})\). Finally \(\widehat X_{R,j}\) is measurable on the retained faces, proving the equality in (RETAINED-SLOW-OVERLAP).

This test rules out a uniform maximal-correlation gap for a proposed iteration of face resamplings. It also shows why that failure alone does not refute the comb susceptibility: its measured overlap with this typical slow sector decreases, and the link matching supplies a time derivative even on the seven spatial aliases. Extending the weighted estimate to the complete correlated retained source, through separations beyond \(S_\beta\), remains necessary for a global zero-mode bound.

### 4.96 Two shifted integrations suppress the true correlated rough face row (P)

The unweighted contraction fails, but the comb row itself gains another inverse side on the typical rough sector. Partition the torus into comparable outer boxes of side \(S\), then inside each outer box use two \(s\)-face grids with their interior subdivision planes displaced by a fixed fraction of \(s\) in every direction. Keep the common outer faces in both. Require \(2\le s,\ 8s\le S\le\beta^{1/2000}\); besides bounded geometric changes all inner boxes have comparable sides of order \(s\). Such grids are obtained by putting their first interior planes roughly \(s/2\) apart, retaining the odd spatial seams of the comb, and distributing bounded even remainders at the last cells. Interior parallel planes of opposite grids stay separated by \(cs\); common outer faces are treated separately. Let \(P_1,P_2,P_S\) be conditional expectations on these three genuine tangential face fields, with \(P_S\) the outer one. For either original comb \(Y^r,Y^h\),
\[
 0\le \operatorname{Var}(P_2P_1Y)-\operatorname{Var}(P_SY)
   =\mathbb E\operatorname{Var}(P_2P_1Y\mid\mathcal F_S)
   \le C V\log(2+s)\left(s^{-2}+S^{-1}\right).
 \tag{SHIFTED-ROUGH-CONTRACTION}
\]
This is a bound on the aligned/shifted response of the actual correlated smaller-grid exterior under the full Wilson law. Both operators integrate real conditional laws. In particular the common outer variance remains with coefficient one.

**Gaussian trace estimate inside one outer cell.** At fixed boundary \(D\), denote by \(v_{b,i}\) the Riesz vectors in the centered Gaussian energy space representing the original directional linear forces \(H_i A_b\). Their analysis operator has bounded norm, since \(\|H_i C^{1/2}\|\le C_N\) in the Dirichlet space. Write \(Q_j\) for orthogonal projection of these linear variables onto the face observations of the \(j\)-th inner grid. The first retained linear force is the harmonic extension from the boundary of its cell. On its centered part,
\[
 Q_1 v_{b,i}=\sum_{p\in\partial B_1(b)} L_{bi,p}\,v_p,\qquad
 |L_{bi,p}|\le C[(1+d(b,p))^{-4}+s^{-4}],
\]
where \(v_p\) represents the oriented linear curl on a boundary plaquette. This is precisely the doubled-cell formula of §§4.70–4.72 with its incidence signs. The sum of the absolute coefficients is bounded per root, and for one boundary plaquette their sum over all roots in its incident cells is at most \(C\log(2+s)\), by the four-dimensional shell count. For the second grid,
\[
 \|Q_2 v_p\|^2\le C[(1+d(p,\mathcal F_2))^{-4}+s^{-4}].
\]
Here \(d(p,\mathcal F_2)\) is distance to its nearest geometric face. A retained boundary plaquette uses the bounded unprojected norm. Otherwise the centered projection variance is the difference between the outer Dirichlet covariance and the second-cell zero-boundary covariance. Variational projection bounds this difference by infinite curl variance minus the second-cell Dirichlet value. The latter is bounded by the displayed expression: its nonidentity reflected images use the order-zero curl-projection kernel estimate of §4.72. The periodic diagonal differs from the infinite one by \(O(s^{-4})\). For this last rate, sum the image errors \(C_J\rho^4(\rho s)^{-J}\) on smooth Fourier shells \(\rho\gtrsim1/s,\ J>4\), and bound the remaining continuous and discrete low frequencies directly by \(Cs^{-4}\). This reasoning works for tangential and normal plaquettes.

Cauchy–Schwarz with the absolute \(L\)-row, then summation over roots, gives
\[
 \sum_{b,i}\|Q_2Q_1 v_{b,i}\|^2
 \le C\log(2+s)\sum_{p\in\mathcal F_1}
            [(1+d(p,\mathcal F_2))^{-4}+s^{-4}]
 \le C\log(2+s)(S^4/s^2+S^3).
\]
For the last count the first-grid interior faces have \(O(S^4/s)\) plaquettes. On a first-grid face, parallel interior planes of the second grid stay \(cs\) away. Transverse second planes cut out a fraction at most \(C(1+r)/s\) within distance \(r\le cs\). Sum the fourth-power decay there and add the \(O(S^3)\) possible outer-face and adjacent irregular positions. Constants absorb the bounded cell aspect ratios.

Conditional expectations of Gaussian quadratic variables are Gaussian quadratics plus their exact traces. After the two operations their centered quadratic matrix is the sum of the weighted outer products of the \(Q_2Q_1v_{b,i}\) with the fixed matching matrix, of bounded norm. Its trace is bounded by the preceding sum because the unit comb is nonnegative. Thus its squared Hilbert–Schmidt norm satisfies the same estimate. The shifted conditional linear part from the true outer boundary is bounded in squared Gaussian norm by \(C\sum_{b,i}|(H_i E D)_b|^2\), using the bounded analysis norm and the two norm-one projections. HARMONIC-FACE-FORCE has true averaged bound \(CS^3\) for this sum. Scalar identity rows have no conditional variance. We have therefore bounded the averaged conditional variance of the composing Gaussian polynomials on an entire outer box, including the noncentral part.

**Transfer to genuine nonnested Wilson face observations.** The second grid must be an actual sigma-field for the comparison. Fix outer boundary gauges, and use an outer based forest which first joins the vertices of the second skeleton to prescribed outer vertices within that skeleton, then joins each remaining interior tree to it. The skeleton graph admits paths of length \(O(S)\) to the outer faces, for example by moving along an available skeleton plane to the outer boundary. Multi-root shortest-path trees and then cell trees have this diameter. Subsequent free chording and fixed-boundary curl coercivity use the same \(O(S^2)\) fillings as §4.68. The independent Haar gauge variables based on the interior vertices integrate out. For gauge-invariant scalars, observing the physical second skeleton in this forest is exactly observing its residual link coordinates: its other original vertex frames do not occur in the conditional scalar. In the linearized Gaussian the same skeleton coordinates give its usual linear conditional projection. This choice is required only for the second grid; it imposes no simultaneous tree condition on the first.

On an outer good boundary the normalized compact law of these coordinates and its Dirichlet Gaussian have total variation \(O(\Delta+\mathrm{poly}(\beta,S)e^{-cP^2})\), where \(P=\log\beta,\ T=C S^8P,\ \Delta=C g S^{28}P^3\), by §4.69. One may use bounded logarithm coordinates outside the canonical ball, and use the real Gaussian coordinates on the common chart. In this forest the first *actual* conditional expectation is approximated by its Gaussian first-grid polynomial. In detail first fix a tree in each first-cell boundary using only its boundary links, with \(O(s)\) paths. With true probability \(1-\mathrm{poly}(S)e^{-cP^2}\) all these first-boundary representatives lie within the good \(Cs^2P\) bound (use the fixed-cell filling and true star moments). There the one-root comparison of §4.69 gives error \(C g s^{44}P^5\). On the outer canonical ball each such boundary path word has log in canonical units equal to its linear path sum up to \(C g s^2T^2\); the sum has modulus \(CsT\). The harmonic one-root operator in boundary sup norm is at most \(Cs^6\). Comparing its squares on these two inputs costs \(C g s^{15}T^3\) per root as in §4.71. The linear path sums give exactly the first-grid Gaussian boundary observation, expressed in the second-compatible outer forest. The first-grid identity traces match. Thus the full first-grid polynomial approximates \(P_1Y\) with root errors just displayed. The true full-law complements have superpolynomial cost before taking conditional variances; the actual compact root has size \(C\beta\). No independence between crossing first and second cells is used.

For precision in comparing conditional operators under two densities, if \(P,Q\) are laws of total variation \(\delta\) and \(|X|\le H\), then for any common observation \(\mathcal A\),
\[
 \|\mathbb E_P(X\mid\mathcal A)-\mathbb E_Q(X\mid\mathcal A)\|_{L^2(P)}
       \le C H\sqrt\delta .
\]
Indeed the signed \(X\)-weighted observation marginals differ in total variation by \(O(H\delta)\), and so do the unweighted marginals multiplied by the bounded second conditional mean. This gives an \(L^1(P)\) bound followed by the sup bound \(2H\). On a set unseen by \(Q\) choose any bounded version. Apply the estimate in each good outer cell to the first Gaussian polynomial clipped at \(H=C S^{45}P^3\), which exceeds its whole outer canonical-window bound \(C S^4s^{14}T^2\). Clipping costs superpolynomial Gaussian-tail moments, and in the true law all comparison errors are bounded as above or by the original compact bound off the good event. For the bounded resulting second Gaussian observation its variance under \(P\) differs from that under \(Q\) by at most \(C H^2\delta\). All these absolute squared errors are \(O(1)\) per outer cell on \(s\le S\le\beta^{1/2000}\): in particular \(H^2\Delta\le C g S^{118}P^9\), and the squared sum of first-root errors has bound \(C S^8g^2(s^{88}P^{10}+s^{30}T^6)\). On bad outer boundaries one uses the true compact polynomial bound and their superpolynomial unconditional probability. This proves the comparison after integration over the actual outer boundary data.

Finally both smaller skeletons contain the entire outer skeleton, so their repeated conditional mean given that skeleton equals \(P_SY\) exactly. At fixed outer faces the original box interiors are independent; both operations factor by outer cells, including their common faces. Sum the preceding estimates over boxes to obtain (SHIFTED-ROUGH-CONTRACTION). This annealed gain is additional to the one-grid estimates. Iterating such gains to the physical torus would require control of the projected full exterior at larger scales, since the common outer variance is returned exactly at each stage.

### 4.97 A true local magnetic reflection Gram at the mesoscopic comparison scale (P)

There is a direct reflected consequence of the compact rough-field comparison, using a genuine local plaquette rather than a Gaussian readout. Take \(R,S\) as in §4.94 and a smooth nonnegative compactly supported \(w\) in the rescaled positive time half, at positive distance from the reflection planes. With the reflected weight in the opposite half set
\[
 A_R^+=\sum_x w(x/R)\,\beta s_{12}(x),\qquad A_R^-=\theta A_R^+ .
\]
The reflected Gram of the centered variables obeys
\[
 \lim \operatorname{Cov}_\mu(A_R^+,A_R^-)
  =\frac{\tau^2d_G}{2}\int d^4x\,d^4y\
    w(x)\,w(\theta y)\,|C_{12}(x-y)|^2 ,
 \tag{MESOSCOPIC-LOCAL-REFLECTION}
\]
where \(C_{12}\) is the per-color continuum magnetic covariance with Fourier multiplier
\(\tau^{-1}(k_1^2+k_2^2)/|k|^2\), evaluated at nonzero separation. The sum has the original dimension-four engineering smearing normalization on the rescaled unit coordinates. For a bump of positive mass supported sufficiently close to a positive time point \((t_0,0)\), the displayed limit is strictly positive.

Place both supports deep in one outer \(S\)-box. On its good compact chart the oriented \(\beta s_{12}\) equals \(\frac{\tau}{2}|(dB)_{12}|_{\rm coord}^2+O(gT^3)\), with the same global density and tail estimates as §4.95. Four-dimensional support sizes contribute at most \(C R^8\) to product errors, and the compact comparison bound \(C g R^{12}S^{60}\log^7\beta\) still tends to zero. The \(L^4\) norm of a deep outer conditional mean curl is \(O(S^{-1/6})\). Thus the covariance of the sums of its squares is at most \(C R^8S^{-2/3}=o(1)\). The noncentral Gaussian cross terms cost at most \(C R^4 S^{-1/3}=o(1)\), using the separated curl kernel bound \(C R^{-4}\). This treats the actual correlated exterior. Boundary-independent traces cancel upon centering.

For two sites at separation comparable to \(R\), the centered Dirichlet per-color curl covariance is \(R^{-4}(C_{12}((x-y)/R)+o(1))\) uniformly on the separated compact supports. The nonidentity reflected images and the periodic correction to the infinite local kernel are \(O(S^{-4})\) by the dyadic image proof of §4.96, also at displacements \(O(R)\ll S\). On the infinite lattice compare the smooth low-frequency cutoff of the degree-zero continuum multiplier to the lattice multiplier. Their difference on small annuli has \(j\)-th derivatives bounded by \(C_j|k|^{1-j}\) (in this same-orientation row the gain can even be two). Dyadic integration by parts gives kernel error \(O((1+|x-y|)^{-5})\); smooth high-frequency parts have faster decay. The continuum homogeneous multiplier away from its origin in position space is the differentiated four-dimensional fundamental solution. Smooth cutting off its high frequencies affects its large-distance value faster than any fixed power, by distributional differentiation or summing the dyadic integrations by parts. This proves the stated uniform limit. Wick's two cross contractions now give (MESOSCOPIC-LOCAL-REFLECTION) by Riemann summation. At a purely temporal separation \(t\ne0\), the differentiated kernel is \(1/(\pi^2\tau t^4)\), by applying \(-(\partial_1^2+\partial_2^2)\) to \(1/(4\pi^2\tau |x|^2)\). It stays nonzero on a neighborhood. Both observables are in their respective true Wilson half algebras, so the resulting positive limit is an ordinary physical reflection test at these scales.

Here \(R\) diverges in fine lattice units but \(aR\to0\). This verifies a local reflection witness in the actual Wilson law on the mesoscopic range. I-3 requires uniform nondegeneracy for fixed positive physical smearing scale on \(T^*\); that extension and its interacting operator normalization remain open.

### 4.98 Uniform holonomy mixing on long private Wilson lines in the full rough law (P)

There is an actual large-distance bound beyond the mesoscopic Gaussian comparison. It applies to the sector transported along a thin group line. Given every other link, a single Wilson link has probability density \(\nu(dU)\propto e^{-\beta s_*(U)}dU\), where here \(s_*(U)\) is its sum of incident plaquette energies. On all exteriors the real logarithm has geodesic Hessian bounded in magnitude by \(C_N\beta\), because there are six fixed group words of bounded second derivative. Fix the bi-invariant metric and \(\beta\ge1\). For any unitary representation \(\pi\) with no invariant vectors,
\[
 \left\|\int_G\pi(U)\,\nu(dU)\right\|_{\rm op}
       \le 1-c_N/\beta .
 \tag{UNIFORM-LINK-CONTRACTION}
\]
The constant is independent of the representation, volume, and the actual exterior staples.

Indeed the mean left derivative of \(\log\nu\) vanishes by compact Haar integration. For a left translate \(h\nu\) with \(\operatorname{dist}(h,I)\le\epsilon=c_0/\sqrt\beta\), Taylor along its geodesic gives \(D(\nu\|h\nu)\le C_N\beta\epsilon^2\). The total variation bound from this relative entropy makes the overlap mass of \(\nu,h^{-1}\nu\) at least \(1/2\) for a fixed sufficiently small \(c_0\). For any unit vector \(w\), the Haar integral of \(\|\pi(g)w-w\|^2\) equals 2 since its Haar projection is zero. Thus some \(g\) moves \(w\) by at least one. Write it as \(h^m\) along a shortest group geodesic with \(m\le C_N/\epsilon\) and \(\operatorname{dist}(h,I)\le\epsilon\). Telescoping gives \(\|\pi(h)w-w\|\ge c_N\epsilon\). For another unit vector \(v\), put \(p(U)=\pi(U)v\) and take \(w\) in the direction of its average unless that average is zero. Integrate
\[
 \|p(U)-w\|^2+\|p(hU)-w\|^2
       \ge \tfrac12\|\pi(h)w-w\|^2
\]
against the overlap below \(\nu,h^{-1}\nu\). Both its original and \(h\)-translated measures are dominated by \(\nu\). Consequently \(2\int\|p(U)-w\|^2\,d\nu\ge c_N\epsilon^2\). The latter integral is \(2(1-\|\int p\,d\nu\|)\), giving the claimed bound. This works in particular in the regular representation on mean-zero \(L^2(G)\).

Now take a simple fine path and a set of \(j\) private links on it, each used once. Suppose no action plaquette contains two of these links. Given every other link they are independent with the preceding one-site laws. Their product along the path, including the fixed intermediate factors and any orientation reversals, has a conditional density \(p_\gamma\) relative to probability Haar satisfying
\[
 \|p_\gamma-1\|_\infty
       \le C_N\beta^{d_G/2}e^{-c_N(j-2)/\beta},
       \qquad j\ge2 .
 \tag{PRIVATE-LINE-HAAR}
\]
For each one-site density the sup norm is at most \(C_N\beta^{d_G/2}\): integrate a physical ball of radius \(c/\sqrt\beta\) about its compact maximizer, using the logarithmic Hessian bound and the zero gradient there. Its \(L^2\) norm is at most \(C_N\beta^{d_G/4}\). Convolution by every internal increment contracts mean-zero \(L^2(G)\) by (UNIFORM-LINK-CONTRACTION); translations are isometric, and reversed increments give the adjoint contraction. Use the first and last increment in \(L^2\) and Cauchy–Schwarz for the resulting sup norm of the convolution difference from Haar. The estimates are pointwise in all unselected link data.

As an immediate charged-sector consequence, let \(B_\gamma=\langle A,\operatorname{Ad}(U_\gamma)B\rangle\) with local traceless endpoint fields whose fixed moments are bounded. Examples are canonical plaquette logs transported along fixed local endpoint collars. Assume a simple path of length \(l\) outside those bounded collars. Greedily choose a private subset of at least \((l-C)/C_N\) links with no two in a plaquette. For each original \(r_b,h_b\) remove its fixed-size stencil from this subset. Its factor and the endpoint factors are now fixed in the conditioning. Applying the representation contraction and then Hölder in their actual Wilson law gives
\[
 |\operatorname{Cov}_\mu(Y,B_\gamma)|\le C_N V e^{-c_N l/\beta}
 \tag{FULL-COMB-CHARGED-LINE}
\]
for the entire unit comb, including its constant fine Fourier component; a fixed polynomial loss applies if the endpoint moments have such a loss. A nontrivial representation carrying a single unpaired line is suppressed. A color singlet product on distinct local plaquettes has no such private line hypothesis.

### 4.99 The actual zero-mode variance retained by all thin macroscopic coarse links vanishes (P)

Fix an aligned fine rectangular grid of comparable large sides \(l\), and keep every coarse edge product \(W_c\) along its straight fine path. Let \(\mathcal W_l=\sigma(W_c:\text{all coarse edges})\), \(m\le C V/l^4\) the number of these paths. This is a genuine sub-sigma-field of the full tangential faces. It includes winding coarse loops and arbitrary joint functions of the complete raw coarse graph. Put
\[
 \epsilon_l=C_N\beta^{d_G/2}\exp(-c_N l/\beta).
\]
When \(m\epsilon_l\le1/4\), the true full Wilson law obeys
\[
 \sup_w\left|\mathbb E[Y\mid\mathcal W_l=w]-\mathbb E Y\right|
        \le C V m\epsilon_l,\qquad
 \frac1V\operatorname{Var}(\mathbb E[Y\mid\mathcal W_l])
        \le C V(m\epsilon_l)^2
 \tag{THIN-GRAPH-ZERO-MODE}
\]
for either original unit comb \(Y^r,Y^h\), with a continuous-density conditional version. For \(l\ge A_N\beta(1+\log V+\log(1+\beta))\) with \(A_N\) sufficiently large, the latter is \(o(1)\) on the required fixed-volume trajectory. Thus this full large-scale piece of the correlated exterior cannot carry an extensive excess in its ordinary zero mode.

To prove it, choose the middle portion of each coarse edge path as private links; one may keep, for example, its middle third with integer rounding. The middle parts of different coarse paths are sufficiently far apart that no elementary action plaquette sees two different parts. Along one straight line no plaquette contains two of its collinear longitudinal edges. This remains valid at periodic seams and for winding paths on a coarsest one-site graph when the fine length is large. For a fixed selected root \(b\) delete the links of its stencil from the private set; at most a fixed number is lost on any path. Given the remaining links the private variables are independent, the root value is fixed, and (PRIVATE-LINE-HAAR) gives each \(W_c\) density \(1+O(\epsilon_l)\), uniformly on arbitrary rough exterior values. Distinct paths have independent conditional holonomies. Their joint conditional density against product Haar is therefore \(1+O(m\epsilon_l)\), both above and below. The same holds after any averaging of the exterior.

Let \(Y_b=r_b\) or \(h_b\). Multiplying this density estimate by the fixed \(Y_b\), integrating over the true exterior, then dividing by the lower-bounded marginal density of \(w\), gives
\[
 |\mathbb E(Y_b\mid w)-\mathbb E Y_b|
       \le C m\epsilon_l\,\mathbb E|Y_b|\le C m\epsilon_l
\]
by the full marked moments. This is a pointwise statement for every coarse graph in the density version, not just a typical fixed holonomy. Sum it over the original comb. More generally the variance bound for marks \(f\) is \(C V(m\epsilon_l)^2\sum_b|f_b|^2\). For the true \(M=\mathbb E(Y^h\mid\mathcal E)\) of §4.87 the identical argument applies, since its single-star row \(m_{b,0}\) is again a fixed-stencil exterior function with bounded first moment. Bounds on the second conditional row follow by deleting both stencils for \(Y_bY_{b'}\) and using their bounded product moment. In particular
\(\sup_w|\operatorname{Var}(Y\mid w)-\operatorname{Var}(Y)|\le C V^2m\epsilon_l\).
At fixed positive physical coarse edge length the errors vanish faster than powers of the cutoff.

The decoupling also works in a larger conditional sector. Let \(\mathcal A\) be any observations measurable off the chosen private middle parts before deleting local source stencils. The same conditional density bounds hold given \(\mathcal A\), pointwise on its real records. Therefore
\[
 |\mathbb E(Y\mid\mathcal A,\mathcal W_l)-\mathbb E(Y\mid\mathcal A)|
 \le C m\epsilon_l \sum_b\mathbb E(|Y_b|\mid\mathcal A).
\]
Taking squares and true expectations bounds the variance increment of the thin coarse holonomies amid these additional spectators by \(C V^2(m\epsilon_l)^2\). This specifies when a long line can be removed in a mixed or rough exterior.

The distinction between this sector and the full residual is material. The full face sigma-field contains every tangential fine link and small singlet loops inside its faces, including loops incident to the would-be private middles. The nonlinearly averaged Balaban coarse graph also differs from this graph of straight thin Wilson products. Equation (THIN-GRAPH-ZERO-MODE) bounds an actual macroscopic subspace at the required cutoff and volume; a bound for the remaining correlated singlet face fields is still needed for SUS.

### 4.100 The complete fine one-skeleton and dense winding lines (P)

The vanishing sector in §4.99 also includes every fine link on the macroscopic one-skeleton \(\mathcal F_l^{(1)}\). For a gauge-invariant \(Y\),
\[
 \mathbb E[Y\mid\mathcal F_l^{(1)}]=\mathbb E[Y\mid\mathcal W_l]
 \quad\text{almost surely}.
 \tag{COMPLETE-ONE-SKELETON}
\]
Indeed fix site gauges at coarse vertices and change variables by arbitrary site gauges at all intermediate vertices of the observed paths, extending them to the whole lattice. This preserves the full Wilson law and \(Y\). Two one-skeleton configurations with the same oriented edge products are on the same such orbit: starting at each coarse endpoint, recursively match all but the last fine link; equality of the product matches the last one. Each intermediate vertex belongs to only one straight channel. This also applies to a closed path with a single coarse endpoint. Compact orbit averaging or the exact corresponding tree gauge now proves the identity of conditional expectations. Consequently at a fixed physical grid the *entire* one-skeleton contributes \(o(V)\) to the unamplified zero variance.

If \(\mathcal F_l^{(2)}\) and \(\mathcal F_l^{(3)}\) are the fine tangential links on all two- and three-dimensional faces of this grid, the exact remaining positive decomposition is
\[
 \operatorname{Var}(\mathbb E[Y\mid\mathcal F_l^{(3)}])
   = \mathbb E\operatorname{Var}(\mathbb E[Y\mid\mathcal F_l^{(3)}]
                                                \mid\mathcal F_l^{(2)})
    +\mathbb E\operatorname{Var}(\mathbb E[Y\mid\mathcal F_l^{(2)}]
                                                \mid\mathcal F_l^{(1)})
    +o(V)
\]
at the lengths of (THIN-GRAPH-ZERO-MODE). This confines the possible macroscopic face excess to the two- and three-face interiors. Controlling the bulk innovation up to such a spacing is a further finite-scale requirement.

There is a simultaneous strengthening that does not sparsify the transverse directions. Partition **every** fine coordinate line into segments of length comparable to \(l\), in one or in all four orientations. Keep the product on each segment at every fine transverse position. All the conclusions of §4.99 hold with number of observed products \(m\le C V/l\). To construct private links even for densely adjacent parallel lines, set
\[
 r(x)=\sum_{i=1}^4 d_{\rm per}(x_i,0)\pmod {16}
\]
and retain as private, in the middle of an orientation-\(\mu\) segment, its links with \(r(x)=4\mu\pmod {16}\), indexing the orientations from 0. On the even torus a single coordinate step changes each corresponding distance by \(+1\) or \(-1\). Parallel edges of one plaquette are transversely neighboring, so their residues differ by one. The base points of perpendicular edges of one plaquette give total residue difference at most two, whereas two different chosen orientations have residues separated by at least four modulo 16. Thus no elementary action plaquette meets two private links. On any long straight portion the periodic-distance coordinate is piecewise monotone with at most two reversals, so there are at least \(c l-C\) private links on every segment. Different segment products depend on disjoint private link sets. Deleting any fixed number of local source stencils changes these counts only by a constant. The conditional convolution proof of §4.99 thus applies to this dense family simultaneously.

In particular all temporal Polyakov products, at every fine spatial site and with the full spatial link history held as an arbitrary spectator, contribute only \(o(V)\) *additional* zero-mode variance above the spatial data. The other fine temporal links outside the designated private middles can also be spectators. This is a statement about the true macroscopic winding sector in its rough spatial environment. Local singlet correlations among the spectator spatial links themselves are retained.

### 4.101 A true \(SU(2)\) path with its local singlet energies revealed (P)

The private-link argument can survive exact local singlet observations, on a specified two-dimensional face. Choose long simple straight paths with sufficiently many private links in the interior of the face, so that each private link meets at most two of the revealed face plaquettes. The plaquette trace in \(SU(2)\) is real. Conditional on all unselected links and on the two incident face traces, the quaternion \(u\in S^3\) of a private link lies on a circle. Write \(a\) for the length of the projection to the two constrained quaternion directions and \(r\) for the radius in their orthogonal plane, \(a^2+r^2=1\). Each trace equation is a real linear quaternion coordinate. If their rank is smaller than two, additionally reveal coordinates in any measurable two-plane completing their span. The estimates below can later be marginalized over these auxiliary observations.

Before imposing these traces the exact conditional density is proportional to \(e^{h\cdot u}\) with \(|h|\le C\beta\). Uniformly on every choice of the other links and plane,
\[
 \mathbb P\bigl(\min(a,r)<c_0/\sqrt\beta\mid\text{unselected links}\bigr)
      \le C c_0^2
 \tag{CIRCLE-GOOD-PROBABILITY}
\]
for each private coordinate (at \(\beta\ge1\)). Indeed with Haar measure \(z=r^2\) is uniform on \([0,1]\) and the two angles are uniform. The tilted \(z\)-density is proportional to
\(I_0(|h_\parallel|\sqrt{1-z}) I_0(|h_\perp|\sqrt z)\), where \(I_0(v)\) is the circle average of \(e^{v\cos\theta}\). The second factor is increasing and can only decrease the lower-tail probability compared with setting it to 1, by the elementary covariance inequality for two oppositely monotone functions. The first factor is at most \(I_0(|h_\parallel|)\); for \(0\le z\le c/(1+|h_\parallel|)\) it is at least \(e^{-C} I_0(|h_\parallel|)\), since the log derivative of \(I_0\) has modulus at most one. Dividing the numerator and denominator proves \(P(r<c_0/\sqrt\beta)\le C c_0^2\). Swap the two planes for the other tail. Different private coordinates are independent in this original conditional law. For small fixed \(c_0\), a path with \(j\) private coordinates therefore has at least \(j/2\) good circles, \(a,r\ge c_0/\sqrt\beta\), except on true joint records of probability \(Ce^{-cj}\), uniformly before the traces are revealed.

On a good circle the conditional group law \(\nu_\circ\) has a uniform polynomial mixing rate. Up to left and right quaternion rotations it is
\[
 u(\theta)= a+r(i\cos\theta+j\sin\theta),\qquad
 d\nu_\circ(\theta)\propto e^{b\cos(\theta-\theta_*)}d\theta,\quad
       0\le b\le C\beta r .
\]
The reduction uses the left and right unit-quaternion realization of orientation-preserving rotations of \(\mathbb R^4\); alternatively complete the real offset and the two orthogonal circle directions to an oriented orthonormal quaternion frame. Translations and inversions preserve the convolution contraction norm. For any unitary representation without invariant vectors,
\[
 \left\|\int\pi(u)\,d\nu_\circ(u)\right\|
        \le 1-c\,\beta^{-65}.
 \tag{CONSTRAINED-CIRCLE-GAP}
\]
The exponent here is only a convenient finite constant. Here is a quantitative proof that is uniform in representation and in the actual singlet values on good circles.

Choose \(\alpha=c_1(1+b)^{-1/2}\) with fixed small \(c_1\). At and near \(\theta_*,\theta_*\pm\alpha\) the circle density is at least a fixed constant (indeed it is larger for large \(b\)). In fixed quaternion coordinates the right tangent velocities at \(\theta\) are
\(u^{-1}u'= ar(-i\sin\theta+j\cos\theta)-r^2 k\).
The determinant of the three velocities at those angles has modulus \(2 a^2 r^4|\sin\alpha|(1-\cos\alpha)\ge c\beta^{-9/2}\). Their smallest singular value is at least \(c\beta^{-5}\), since the velocities have bounded norm. Consider the map of six angles given by
\(\prod_{k=1}^3 u(\xi_k)^{-1}u(\eta_k)\). Choose each \(\xi_k\) within \(c\beta^{-5}\) of its respective one of the three centers, and initially \(\eta_k=\xi_k\). Then the product is \(I\) and its three even-angle derivatives have smallest singular value at least \(c'\beta^{-5}\). All second derivatives are bounded independently of these parameters. The quantitative inverse function estimate, in fixed smooth coordinates about \(I\), consequently maps an even-angle ball of radius \(c''\beta^{-5}\) onto a set containing the group ball of radius \(c'''\beta^{-10}\). To check this estimate directly, precompose with the inverse linear derivative, and solve for the even-angle displacement by contraction inside that ball; the derivative error there is at most a fixed fraction of the smallest singular value. The Jacobian on this inverse branch has a uniform upper bound. All six angle densities have the indicated lower bound there. Integrating the three odd angles now gives
\[
 (\check\nu_\circ*\nu_\circ)^{*3}
          \ \ge\ c\beta^{-15}\,1_{\{d(g,I)\le c\beta^{-10}\}}\,dg
\]
where \(\check\nu\) is the inversion image of \(\nu\). Left/right rotations merely conjugate the resulting ball.

For any unit vector \(w\) in a representation without invariants, its average squared displacement on a normalized Haar ball of radius \(\epsilon\) is at least \(c\epsilon^2\). Indeed choose a rotation \(h\) of radius at most \(\epsilon/4\) moving \(w\) by at least \(c\epsilon\) by the geodesic argument of §4.98. For \(g\) in the half-radius ball, compare \(g\) and \(gh\): the difference of their represented vectors is exactly \(\|\pi(h)w-w\|\), and both elements lie in the full ball. The volume ratio of the two balls is bounded below. Apply this to the displayed minorization. With Haar ball volume \(c\epsilon^3\) on \(SU(2)\), it bounds \(1-\langle w,(T^*T)^3 w\rangle\) below by \(c\beta^{-15}\beta^{-30}\beta^{-20}\), where \(T=\int\pi(u)d\nu_\circ\). Taking the sixth root proves (CONSTRAINED-CIRCLE-GAP).

### 4.102 Removing long color transports without discarding the revealed singlet sheet in \(SU(2)\) (P)

Keep all the elementary plaquette traces on specified two-face sheets and any other data off the chosen private paths. Denote these spectator observations by \(\mathcal A\). Let \(W\) be the products on \(m\) edge-disjoint paths, each with at least \(cl\) noninteracting private links, each private link incident to at most two of the revealed plaquettes. The stars of distinct paths' private coordinates must not meet in any Wilson plaquette. This includes long rows in the interior of physical two-faces with enough room or the private coloring of §4.100 on their eligible parts. It does not include an edge lying on several sheets with more than two independent traces revealed there. Then for either original full unit comb
\[
 0\le
 \operatorname{Var}(\mathbb E[Y\mid\mathcal A,W])
       -\operatorname{Var}(\mathbb E[Y\mid\mathcal A])
 \le C\beta^2 V^2\, m\,C\beta^{C_0}e^{-c l/\beta^{65}} .
 \tag{SINGLET-CONDITIONAL-COLOR-SUPPRESSION}
\]
In particular the increment is \(o(V)\) at fixed physical path length on the Wilson trajectory. All singlet records in \(\mathcal A\) keep their true weights; a scalar correlation among those records is not removed.

For a proof in total variation despite the singular one-circle laws, first note that three arbitrary good circles in succession, allowing arbitrary fixed group factors between them, have a smoothing component of probability at least \(p=c\beta^{-45}\) whose normalized Haar density is at most \(C\beta^{64}\). In the product map of the three angles use its three *left* tangent velocities transported by their preceding factors to a common frame. For any one circle its three left velocities at the angular mode and its two neighbors span with smallest singular value \(c\beta^{-5}\), just as in §4.101 (the constant normal term has the opposite sign). Choose the first angle to obtain a velocity of norm at least \(c\beta^{-5}\). At the second angle the preceding rotation is already fixed: one of its three possible velocities has component perpendicular to the first of size at least \(c\beta^{-5}\). At the third angle choose a component perpendicular to the preceding plane in the same way. The resulting three-column determinant has modulus at least \(c\beta^{-15}\). The derivatives have bounded norm and bounded Lipschitz constants. A sufficiently small three-angle ball of radius \(c'\beta^{-15}\) about this choice is an injective patch of the product map with Jacobian at least \(c''\beta^{-15}\), by the same inverse-derivative estimate as §4.101. All three angle densities there are bounded below and have upper bound \(C\sqrt\beta\); the latter follows by integrating the von Mises density within a \(c/\sqrt{1+b}\) interval about its mode. The patch thus has probability at least \(c\beta^{-45}\), and after normalization its image density is at most \(C\beta^{64}\). This argument allows arbitrary relative circle orientations and inversions, unlike a smoothing argument based on identical successive increments.

Conditional on all nonprivate links, and then on their trace observations and any auxiliary projections, private variables on different paths are independent. On a path with \(j/2\) or more good circles, fix all its other private variables temporarily. Group good increments in the first third of their ordered list into disjoint triples. Each triple convolution can be decomposed into the smoothing component just proved and a residual probability measure. Multiplication by interspersed fixed group factors changes no bound. The probability in this mixture that no smoothing component was chosen is at most \(C e^{-c j/\beta^{45}}\). Conditional on the first smoothing component, the running product density has bounded \(L^2\) norm \(C\beta^{64}\); subsequent probability convolutions do not increase this norm. Leave at least the last third of the good circles undecomposed. Their independent convolutions contract mean-zero \(L^2\) by (CONSTRAINED-CIRCLE-GAP). Thus the final path law has distance from Haar in total variation at most \(C\beta^{64}e^{-c j/\beta^{65}}\), including the possible nonsmoothing remainder. Unfixing the other private variables preserves this bound. Bad-circle count records cost \(C e^{-cj}\) *before* revealing their trace values by (CIRCLE-GOOD-PROBABILITY) and independent Bernoulli domination. Averaging over these actual records and using the product total variation bound handles \(m\) paths.

For any chosen original \(Y_b\), omit its bounded stencil from the private set at the start. Then that variable is fixed before the path convolution. We have proved that the law of \((\mathcal A,Y_b,W)\) differs in total variation by at most \(\epsilon=C m\beta^{C_0}e^{-c l/\beta^{65}}\) from the law of \((\mathcal A,Y_b)\) times independent product Haar on \(W\). Marginalizing all auxiliary coordinates used to treat rank-deficient trace constraints preserves this distance. Under the independent comparison law the conditional mean given \((\mathcal A,W)\) is just \(\mathbb E(Y_b\mid\mathcal A)\) from the original law. Apply the conditional-expectation stability bound of §4.96 with \(|Y_b|\le C\beta\), obtaining \(C\beta\sqrt\epsilon\) in true \(L^2\) for the difference of these means. Sum over the comb and square using the exact variance decomposition for nested observations. This proves (SINGLET-CONDITIONAL-COLOR-SUPPRESSION). It gives an all-field physical-scale estimate without replacing the singlet sheet by an independent or Gaussian law.

### 4.103 Removing the entire temporal holonomy projection from the susceptibility (P)

For this real zero-mode calculation one can pass to an unprojected temporal transfer on the full periodic spatial link space. This is a quantitative equivalence for the specified observables, including all rough fields. At each fine spatial site \(x\) let \(W_x\) be the ordered full temporal Polyakov product. For either original comb tilt by \(tY\), \(|t|\le t_1\), its joint density relative to product Haar on \(G^{n^3}\) satisfies
\[
 \sup_{w,t}|\log p_{W,t}(w)|\le
       C n^3\beta^{d_G/2}e^{-c_N n/\beta}=:\delta_n .
 \tag{AXIAL-HOLONOMY-DENSITY}
\]
To see this also at nonzero real tilt, color the fine spatial sites so sites within periodic graph distance two have different colors. A greedy coloring uses only a fixed number \(m_0\) of colors by the bounded degree. A temporal edge at \(x\) is private at times in its own color residue modulo \(m_0\). Each full line has at least \(n/m_0-1\) such times. Wilson plaquettes and every individual star in the real tilt involve at most one private edge: all the temporal edges of such a star have one time and their spatial separation is at most two. The one-private-link tilted phase has uniformly bounded log Hessian \(C_N\beta\), including its fixed number of source words. Hence §§4.98–4.99 apply unchanged, after any two local source stencils are deleted. Every individual \(\mathbb E_t Y_b\) and \(\mathbb E_t Y_bY_c\) conditioned on \(w\) differs from its unconditional value by at most \(C\delta_n\) by the marked tilted moments and the same local numerator density argument.

Choose the continuous compact conditional fiber \(w_x=I\) at every site. Gauge transformations successively along the time columns, identity on their bottom vertices, set every temporal link to identity on this fiber. The unit Haar Jacobians can equivalently be checked by integrating the first \(n-1\) links of each time column as gauge variables while using the product for its final variable. All original scalar insertions are evaluated *after* their unprojected link derivatives in the original Wilson law have been formed. Writing \(\sigma_{u,e}\) for spatial links on time slice \(u\), the exact zero-source fiber density is
\[
 \prod_{u=0}^{n-1}e^{-\beta S_{\rm sp}(\sigma_u)}
       \prod_{e} e^{-\beta s(\sigma_{u+1,e}\sigma_{u,e}^{-1})}
           \prod_{u,e}d\sigma_{u,e},\qquad \sigma_n=\sigma_0
\]
up to normalization. For a temporal root \(b=(u,x)\), the two oriented staple matrices of spatial direction \(i\) are exactly
\(\sigma_{u+1,x i}\sigma_{u,x i}^{-1}\) and
\(\sigma_{u+1,x-i,i}^{-1}\sigma_{u,x-i,i}\).
Thus the original \(r_b\) or \(h_b\) is an explicit scalar of the two neighboring slices. Let \(F_{\rm ax}(t)\) be its normalized moment function on this fiber. Then
\[
 |\log F_{\rm ax}(t)-\log\mathbb E e^{tY}|\le 2\delta_n,\qquad
 |\operatorname{Var}_{{\rm ax},t}(Y)-\operatorname{Var}_t(Y)|
       \le C V^2\delta_n=o(V).
 \tag{AXIAL-ZERO-EQUIVALENCE}
\]
The first estimate is the exact ratio \(p_{W,t}(I)/p_{W,0}(I)\). The second uses the separately proved uniform first and second conditional rows. We do not differentiate an approximation on a real interval to obtain a point curvature. Upper bounds of the size displayed hold at every real \(t\) in the indicated fixed interval. In particular ordinary all-mark SUS on this trajectory is equivalent to the extensive variance of this literal axial fiber comb.

There is a special product structure in the unprojected two-slice transfer. Each selected spatial site has six incident spatial bonds, and the six-sets of distinct even selected sites are disjoint. For the three outward bonds keep the spatial variable \(v_e=\sigma_e\); for the three inward bonds take \(v_e=\sigma_e^{-1}\). All original staples at the selected site are then left increment matrices \(u_e=v_e'v_e^{-1}\). Write \(B(v)=e^{-\beta S_{\rm sp}(\sigma(v))}\). For one marked star let
\[
 c_Y(z)=\int_{G^6}\exp[-\beta\textstyle\sum_{j=1}^6s(u_j)+zY_b(\mathbf u)]\,d\mathbf u .
\]
Divide its kernel by \(c_Y(z)\), and divide each remaining one-bond kinetic kernel by its own mass. The full resulting \(\mathsf K_z\) is a tensor product of independent normalized group convolutions. The positive spatial multiplication is unchanged. With \(T_z=B^{1/2}\mathsf K_z B^{1/2}\), the exact axial pressure identity is
\[
 \log F_{\rm ax}(z)=|\mathcal C|\log[c_Y(z)/c_Y(0)]
                     +\log\frac{\operatorname{Tr}T_z^n}
                                     {\operatorname{Tr}T_0^n}
 \tag{AXIAL-PRODUCT-TRANSFER}
\]
as a germ at zero, or as an identity before taking logarithms wherever the local masses are nonzero. No temporal gauge projection occurs in this expression.

The one-star mass is zero-free on a fixed complex disc. Its phase for the relative source uses the original fixed six compact increments and has a critical point at identity on that whole disc, with positive real quadratic part. The real Wilson complement has an action gap relative to this critical point, by the pointwise source domination and the compact unique minimum of the six independent kinetic energies; the constant ordinary Casimir is removed first. Centering on one small coordinate ball and integrating the complex Gaussian gives the same uniform \(O(1/\beta)\) relative remainder by parity as in §4.90. On the canonical scale the six increments are independent tangent Gaussians of coordinate variance \(1/\tau\), and each matching uses the sum of two. Consequently the logarithms of the mass ratios tend on a smaller disc to
\[
 -d_G\log(1-4\tau z)\quad (Y^h),\qquad
 -2\tau d_G z-\tfrac32 d_G\log(1-4\tau z)\quad (Y^r)
\]
with locally uniform \(O(1/\beta)\) error. These bulk kinetic identity rows do not give the total susceptibility. The magnetic trace in (AXIAL-PRODUCT-TRANSFER) contains the remaining interacting response.

### 4.104 A volume-independent complex kinetic-form estimate and its magnetic limitation (P)

In the exact unprojected description of §4.103 the normalized kinetic source is small in a stronger sense than a scalar exponential-volume estimate. On a fixed complex disc \(|z|\le r_0\),
\[
 \mathsf K_z-\mathsf K_0
       =(I-\mathsf K_0)^{1/2}\mathsf D_z(I-\mathsf K_0)^{1/2},
 \qquad \|\mathsf D_z\|_{2\to2}\le C_N|z| ,
 \tag{GLOBAL-KINETIC-FORM}
\]
uniformly in all spatial sites, \(\beta\) and \(n\). In particular for the actual magnetic transfer,
\[
 |\langle f,(T_z-T_0)g\rangle|
   \le C |z|\,\langle f,(I-T_0)f\rangle^{1/2}
                \langle g,(I-T_0)g\rangle^{1/2}.
 \tag{MAGNETIC-ABSOLUTE-FORM}
\]
The operators in the first estimate are genuine transfer kernels for the unit comb, and \(I-\mathsf K_0\) is understood on the mean-zero subspace and zero on constants.

For one six-bond star write \(\nu_z\) for its normalized kinetic probability continued in its complex source. At zero it is a product of six central Wilson link kernels, and on any irreducible representation its Fourier multiplier is \(kI\) with \(0\le k\le1\). Nonnegativity follows because \(e^{\beta\Re\operatorname{Tr}u}\) is a positive-definite class function: expand the exponential in characters of the defining representation, its conjugate and their tensor powers with nonnegative coefficients. For all \(z\), the density is invariant under simultaneous inversion on \(G^6\): each force changes sign, its scalar square and the Casimir stay unchanged. By the mass comparison of §4.103 and \(|Y_b|\le C(1+\beta S_*)\), \(S_*=\sum_j s(u_j)\),
\[
 |d\nu_z-d\nu_0|\le C|z|(1+\beta S_*)e^{c\beta S_*}\,d\nu_0
\]
with \(c<1\) by reducing the disc. The two measures have equal unit mass. In a matrix coefficient against a unit vector \(v\), inversion symmetry expresses their Fourier difference as minus one half the integral of \(\|\pi(u)v-v\|^2\) against this signed difference.

Uniformly for every representation, the latter weighted quadratic deficit is bounded by \(C\) times its ordinary zero-source deficit. Indeed \(S_*(u)\asymp d(u,I)^2\) globally by compactness and the nondegenerate minimum. Set \(\epsilon=\beta^{-1/2}\) up to a fixed small factor. The \(\nu_0\) density is bounded below by \(c_N\epsilon^{-6d_G}\) on a ball of radius \(\epsilon\), and the weighted density above, without its factor \(|z|\), is bounded by \(C\epsilon^{-6d_G}(1+\beta d^2)e^{-c'\beta d^2}\). For any \(\operatorname{dist}(h,I)\le\epsilon/2\), averaging the triangle inequality for \(g,gh\) with \(g\) in the half-radius ball bounds \(\|\pi(h)v-v\|^2\) by a constant times the mean deficit on the entire ball. Reach general \(u\) by at most \(C(1+d(u,I)/\epsilon)\) such equal geodesic steps and telescope. The weighted Gaussian integral of the square of this number is uniformly bounded. This proves the deficit comparison. Consequently the numerical radius of the Fourier difference is at most \(C|z|(1-k)\), and its operator norm at most twice this bound. This includes arbitrarily high representations.

Every global representation of the product spatial link group decomposes into tensor factors on these disjoint stars and the untouched single bonds. On each irreducible block expand the difference of the tensor product from its zero value. If its scalar zero-source multipliers are \(k_j\in[0,1]\), the norm is bounded by
\[
 \prod_j[k_j+C|z|(1-k_j)]-\prod_j k_j
       \le C|z|\,(1-\prod_j k_j),\qquad C|z|\le1 .
\]
The last inequality is the elementary expansion according to the nonempty subsets of failed independent trials with probabilities \(1-k_j\). There is no multiplicative volume constant. On each block divide by the scalar \(1-\prod k_j\), using zero on the trivial block. The uniformly bounded Fourier direct sum proves (GLOBAL-KINETIC-FORM); it is holomorphic on any smaller disc by uniform Cauchy estimates. Finally \(B^{1/2}(I-\mathsf K_0)B^{1/2}=B-T_0\preceq I-T_0\) since \(0<B\le1\). This proves (MAGNETIC-ABSOLUTE-FORM) by polarization of the displayed operator factorization.

There is a quantitative reason that this bound alone does not close the magnetic trace curvature. Its zero reference is the absolute spectral value one, whereas the actual leading eigenvalue of \(T_0\) obeys
\[
 e^{-C_N n^3}\le\lambda_{\max}(T_0)\le e^{-c_N n^3}
 \tag{MAGNETIC-VACUUM-SCALE}
\]
for \(\beta\) sufficiently large. For the upper bound, the Schur test gives at most the sup of the row mass of the symmetric positive kernel \(T_0\). At every fixed initial spatial configuration the independent kinetic increments produce final links. From \(B^{1/2}\) keep just a positive density of disjoint final spatial plaquettes. For each, fixing three increments, the fourth has sup density \(C\beta^{d_G/2}\). The chance the plaquette lies within \(c'/\sqrt\beta\) of identity is at most \(1/2\) for sufficiently small fixed \(c'\). Hence its averaged factor \(e^{-\beta s_p/2}\le1\) has mean at most \(1-c_N\). Disjoint plaquettes use independent increments. Drop the initial \(B^{1/2}\le1\) to get the upper exponential. For the lower bound test the Rayleigh quotient on the indicator that every spatial link is within \(c'/\sqrt\beta\) of identity. There the initial and final \(B^{1/2}\) factors cost at most \(e^{-C n^3}\). From any state in that set, each single kinetic increment has probability bounded below to stay in its own allowed final ball, by its fixed scaled lower density near identity and the Haar-ball volume. Their product gives the lower exponential.

The relative resolvent at the *absolute* spectral value one is therefore controlled by (MAGNETIC-ABSOLUTE-FORM). Dividing by the true vacuum size in (AXIAL-PRODUCT-TRANSFER) can lose \(e^{C n^3}\) in this estimate. The missing signed quantity is the curvature of the logarithm of the normalized magnetic transfer trace at its actual spectral scale. A uniform complex comparison with \(I-\mathsf K_0\), without further magnetic normalization or a weighted spectral sum, does not supply this curvature.

### 4.105 Exact remaining spatial-star exterior in the unprojected transfer (P)

In the true axial fiber of §4.103 condition on every spatial link trajectory except the six bonds incident to each all-even marked spatial site. These retained exterior trajectories will be denoted by \(E\). A spatial plaquette has at most one all-even vertex, hence meets at most one of the selected stars; when it meets one, its two edges there are in that same six-set. The complete length-\(n\) star trajectories are consequently independent conditional on \(E\), including in the presence of the real unit source. The conditional log generating function is a sum over spatial sites of one-dimensional magnetic star transfer logarithms with the specified, generally rough time-dependent \(E\). In particular
\[
 \operatorname{Var}_{\rm ax}(Y)
 =\sum_{x\ {\rm even}}\mathbb E_{\rm ax}\operatorname{Var}
       \left(\sum_t Y_{t,x}\,\middle|\,E\right)
 +\operatorname{Var}_{\rm ax}\left(\sum_{x\ {\rm even}}
             \mathbb E_{\rm ax}\left[\sum_t Y_{t,x}\,\middle|\,E\right]\right).
 \tag{SPATIAL-STAR-EXTERIOR}
\]
These are independent conditioned stars; their means are not independent in the last term.

At one star write \(v_{t,i}\) for the six spatial spokes oriented out of the chosen site, and take \(g_t=v_{t,1}\), \(w_{t,i}=g_t^{-1}v_{t,i}\), \(w_{t,1}=I\). The changes at each slice have unit Haar Jacobian. Spatial plaquette terms in the star are functions of the relative shapes only: each has the cyclic trace of \(w_{t,i}L_{ij,t}w_{t,j}^{-1}\) where \(L_{ij,t}\) is its fixed middle exterior path (invert orientation as needed). The graph of such magnetic pair constraints is the octahedral graph on the six directed spatial neighbors: perpendicular directions are adjacent and opposite directions are not. The angular coordinate \(g_t\) is absent from all these magnetic terms. Let \(\xi_t=g_t^{-1}g_{t+1}\) and \(K_{t,i}=w_{t+1,i}w_{t,i}^{-1}\). After conjugation by \(g_t\), the six temporal increments are \(\xi_t K_{t,i}\). The original simultaneous force norms and their Casimir are unchanged by that common conjugation. The \(g_t\) integral is the product-Haar integral of the \(\xi_t\)'s with the single periodic constraint \(\prod_{t=0}^{n-1}\xi_t=I\), times the harmless global Haar integral of \(g_0\).

For any fixed shape history the unconstrained \(\xi_t\)'s are independent real one-link Wilson integrals with the six given staples and their own local \(tY\) sources (denote the real source parameter by \(z\) here). All these smooth real phases have log Hessian bounded \(C\beta\), uniformly in the shapes and small \(|z|\). Thus the density at \(I\) of the product of these \(n\) increments differs from one by at most \(C\beta^{d_G/2}e^{-c n/\beta}\), uniformly even on singular shape records. Deleting one or two local observable slots proves the corresponding uniform first- and second-row comparisons with bounds \(C\beta n\epsilon_n\) and \(C\beta^2 n^2\epsilon_n\) for the whole star, where \(\epsilon_n=C\beta^{d_G/2}e^{-c n/\beta}\). Multiplying the shape marginal by the periodic correction of every star changes bounded global first and second moments by at most another polynomial in \(n,\beta\) times \(\epsilon_n\), since there are \(n^3/8\) stars and each correction is pointwise uniform. Consequently (SPATIAL-STAR-EXTERIOR), to error \(o(V)\) for the full variance, may use independent \(\xi_t\)'s even after conditioning on all the arbitrary magnetic exterior histories. This removes the possible slow common site-gauge rotor within each star; it does not remove the dynamics of the relative magnetic spokes.

Explicitly, with the periodic correction dropped the real shape transfer at a star has temporal kernel
\[
 D_z(w,w')=\int_G
      \exp[-\beta\sum_{i=1}^6s(\xi w'_i w_i^{-1})
                         +zY_{b}(\{\xi w'_i w_i^{-1}\}_{i=1}^6)]\,d\xi
\]
multiplied on its two sides by the square roots of the adjacent slice magnetic weights just described. This is an actual finite-width temporal shape problem with five compact group coordinates per site of the time chain. The exterior \(E\) has no links incident to an all-even spatial site and no Polyakov variables. At aligned exterior references the flat on-site magnetic Hessian on these five shapes is the rooted octahedral graph Laplacian times \(\tau\), strictly positive: its energy is the sum of squared adjacent differences, and \(w_1\) is pinned. The temporal Hessian at a compatible reference is a sum of squares including \(|\xi_t|^2\) from \(K_{t,1}=I\). Thus on a fixed sufficiently small neighborhood of a compatible shape reference the joint Hessian has a positive lower quadratic constant independent of the temporal length, by bounded-degree continuity. Irregular time records and the last spatial exterior covariance in (SPATIAL-STAR-EXTERIOR) are still present. In particular this local Hessian statement has not been used as a uniform gap of the magnetic transfer.

### 4.106 A magnetic shape bridge with arbitrary endpoints in the true axial problem (P)

The relative star in §4.105 has a good-exterior bridge estimate for every fixed \(SU(N)\), despite arbitrary endpoint shapes. All time lengths below are fine time steps. Call an exterior interval good if there exist references \(a_{u,i}\) with \(a_{u,1}=I\), every \(a_{u,i} L_{ij,u} a_{u,j}^{-1}\) within \(\delta\) of identity on octahedral edges, and every \(a_{u+1,i}a_{u,i}^{-1}\) within \(\delta\) of identity. Use a sufficiently small fixed \(\delta=\delta_N\). For an interval of \(m=\lceil C_2\beta\rceil\) relative shape spins, its positive released bridge kernel \(K(l,r)\) with arbitrary endpoint shapes has
\[
 \sup_{l,l',r,r'}
 \left|\log K(l,r)+\log K(l',r')-\log K(l,r')-\log K(l',r)\right|
        \le C e^{-c\beta}
 \tag{MAGNETIC-SHAPE-BRIDGE}
\]
on a good interval. This is uniform in the time-dependent rough exterior whenever it meets this explicit test.

Write \(V_u(w)=\sum_{i\sim j}s(w_i L_{ij,u}w_j^{-1})\). There are constants with
\(V_u(w)\ge c\,d(w,a_u)^2-C\delta^2\), for all compact \(w\). Indeed \(w_i a_{u,i}^{-1}\) and \(w_j a_{u,j}^{-1}\) differ by at most the actual magnetic defect plus \(C\delta\); connect every site to the pinned spoke through the fixed graph and square. Chord and geodesic distances are comparable on the compact group. The nonnegative temporal energy \(\sum_i s(\xi w'_i w_i^{-1})\) is uniformly bounded and contains \(s(\xi)\). When shapes are within \(\eta_0\) of successive references and \(\xi\) is within \(\eta_0\) of \(I\), all the local energies are at most \(C(\eta_0^2+\delta^2)\).

Fix small outer cap radii for the shapes and the \(\xi\)'s on which the physical log-coordinate Hessian is at least \(c\beta I\). This follows from the rooted octahedral quadratic energy, the \(|Z_u|^2\) temporal pin, and bounded temporal degree as in §4.105. The compatible reference errors perturb the Hessian by \(O(\beta\delta)\) and Haar log Jacobians have bounded Hessians. Choose a cut radius much smaller than both cap radii, then a near radius \(\eta\) much smaller than the cut radius. In a buffer of fixed length \(L_0\), the conditional probability that every shape is outside the near radius is \(Ce^{-c\beta}\), uniformly in both endpoint shapes. In fact its numerator is at most \(\exp[-\beta L_0(c\eta^2-C\delta^2)]\). For a denominator lower bound take all interior shapes and temporal coordinates within a smaller fixed radius \(\eta_0\) of their references and \(I\). The two arbitrary endpoint interactions then cost at most a fixed total \(C_1\); the other actions cost \(C L_0(\eta_0^2+\delta^2)\). The fixed Haar volumes give another positive factor depending on \(L_0,\eta_0\), independent of \(\beta\). Choose \(L_0\) large enough against \(C_1/\eta^2\), and then \(\eta_0,\delta\) sufficiently small. This proves the buffer assertion.

For two near endpoints separated by at most \(4L_0+4\), a specified internal shape outside the cut radius, or temporal coordinate outside its cap, likewise has probability \(Ce^{-c\beta}\). Its respective magnetic or temporal energy costs a fixed positive multiple of the squared target radius. In the same denominator comparison the two endpoint costs are now \(C(\eta^2+\eta_0^2+\delta^2)\), and the fixed bulk cost \(C L_0(\eta_0^2+\delta^2)\) can be made smaller than half the numerator exponent. For endpoints within the cut radius one obtains the same assertion for excursions outside the larger full cap by choosing the cut radius small first. To apply it at a point at least \(2L_0+2\) from the arbitrary original endpoints, take one fixed buffer on each side of that point. Except with \(Ce^{-c\beta}\), both contain a near endpoint. Union over the bounded number of possible endpoint pairs, condition on just those endpoints, and apply the short-interval bound. No conditioning on how an endpoint pair was first found is necessary. This proves that two fixed cuts at distance \(3L_0+3\) from the opposite ends are both in their cut caps except with \(Ce^{-c\beta}\), uniformly on arbitrary exterior endpoints. Between cut-cap endpoints, a union bound gives probability \(C m e^{-c\beta}\) for any full-cap excursion: use near buffers on both sides when available, or use a known endpoint already in the cut cap near a boundary. If the interval is short both such endpoints suffice directly.

On this inner bridge with cut-cap endpoints the normalized convex product chart obeys the spatially weighted covariance bound (CAP-WEIGHTED-COVARIANCE), now in the one-dimensional *time* distance for the shape variables and their temporal auxiliaries. Indeed the Euclidean positive Hessian lower bound is \(c\beta\); a diagonal exponential time weight commutes with the product Laplacian, coordinate-ball Neumann boundary and diagonal Jacobian terms, and changes the bounded-degree off-diagonal Hessian by \(C\beta(e^\alpha-1)\). The Poisson one-form inverse proof of §4.64 applies with sufficiently small \(\alpha\). Endpoint-score sup and first gradients are \(O(\beta)\), and the two endpoints have no direct mixed interaction in this long bridge. Differentiating its log in the two endpoints gives the score covariance. It has modulus \(C\beta e^{-c m}\) in the convex chart plus \(C\beta^2 m e^{-c\beta}\) from the actual compact complement. Integrate over bounded paths within the small cut caps. The inner kernel consequently factors, up to relative \(1+O(e^{-c'\beta})\), into a single left function and a single right function for all cut-cap endpoint pairs (fix one reference endpoint on each side in the log cross-ratio). Multiplying and integrating the two outside buffers preserves this factorization. The removed outside-cut-cap event costs a relative \(O(e^{-c\beta})\) on the original bridge for each arbitrary pair of outer endpoints. This proves (MAGNETIC-SHAPE-BRIDGE) without presuming convexity about incompatible outer endpoints.

### 4.107 Macroscopic temporal response of the actual correlated spatial exterior (P)

In (SPATIAL-STAR-EXTERIOR) write \(m_{x,t}(E)=\mathbb E_{\rm ax}[Y_{t,x}\mid E]\) at zero source, and \(M_{\rm sp}(E)=\sum_{x,t}m_{x,t}(E)\). Use a unit left derivative \(D_e\) in a spatial exterior link on slice \(u\) and canonical factor \(g=\beta^{-1/2}\). The actual full axial exterior law satisfies
\[
 \begin{split}
 &\sup_{x,t}\sum_{u,e\ {\rm incident\ exterior}}
             \|g D_{u,e}m_{x,t}(E)\|_{L^2(E)}\le C_N,\qquad
 \sup_{x,u,e}\sum_t\|gD_{u,e}m_{x,t}(E)\|_{L^2(E)}\le C_N,\\
 &\mathbb E_{\rm ax}\sum_{u,e,A}|gD_{u,e}^A M_{\rm sp}(E)|^2\le C_N V,\qquad
 \sum_x\mathbb E_{\rm ax}\operatorname{Var}(\sum_t Y_{t,x}\mid E)\le C_N V .
 \end{split}
 \tag{SPATIAL-EXTERIOR-SCORE}
\]
In particular the first spatial integration is complete for the entire time period of the required torus, for all \(SU(N)\). The derivative estimates concern the genuine normalized, correlated real exterior readout. The terminal variance \(\operatorname{Var}_{\rm ax}M_{\rm sp}\) still requires a bound for this specific scalar under its spatial exterior law.

First the marked plaquette moments used below hold in the full axial model itself. Real Wilson measure with *all temporal links fixed to \(I\)* is reflection positive on the same coordinate site planes: enforce the pin by a product of reflection-symmetric one-link positive weights tending to the compact delta, factor on the closed halves, and take the normalized limit. This equals the axial spatial law by its explicit action. Its ratios of partition functions at proportional positive Wilson couplings equal the corresponding full-Wilson ratios times the ratios of the Polyakov product densities at \(I\); the latter have uniformly bounded logarithms by §4.103, also at each proportional coupling. The chessboard and forest pressure argument of §§4.11,4.22 therefore yields the same joint fixed-small-exponential marked estimates. In particular all fixed moments of \(\beta s_p\) are bounded. This proof does not require conditioning simultaneously on an arbitrarily large list of energy witnesses when using the private paths.

If an exterior interval at a star fails the good test of §4.106, at least one of \(C m\) plaquettes in that actual axial space-time tube has \(s_p\ge\epsilon_N>0\). Indeed if all these plaquette words are close to identity, take the actual spoke shapes as a witness for the magnetic test. Each relative temporal increment is close to identity because both its true temporal word and the reference-spoke temporal increment are close to identity. Thus the property, which asks only for existence of references in the exterior data, holds. For disjoint well-separated bridges the witness sets have bounded multiplicity, and choosing separated sets on one arc makes them disjoint. For \(h\) specified such bridges, summed witness placements and the axial marked-set estimate give probability at most \((Cm e^{-c\beta})^h\). These events depend only on \(E\); their probabilities in the released joint law obey the same estimate with a bounded global prefactor by the pointwise periodic density comparison of §4.105.

On each good bridge the positive-kernel ratio in (MAGNETIC-SHAPE-BRIDGE) bounds the total variation influence through that bridge by \(e^{-c\beta}\) even after multiplying by an arbitrary positive future weight. A bad bridge uses coefficient one. On any long periodic arc place separated bridges of length \(m=C_2\beta\), with one comparable spacer between consecutive bridges. As in the exact Markov proof of §4.64, one-endpoint boundary influences multiply along the arc. The true exterior average of that product, or of its square, is bounded by \(C e^{-c\beta h}\) for \(h\) designated bridges: expand the product of \(e^{-c\beta}+1_{\rm bad}\) and use the just-proved joint witness bound. Thus local bounded observables at distance \(d\ge16m+O(1)\) on the periodic star chain have conditional covariance with \(L^2(E)\) norm at most \(C\,\mathrm{poly}(\beta)e^{-c'd}\), by the two arcs, including observables of the internal \(\xi_t\) at their time index. One may condition first on all coordinates in the first support and then apply the endpoint transition kernels on both sides of the second support. This uses the actual positive conditional normalization rather than a product approximation for \(E\).

For the required local magnetic response insert
\(J_{x,u,e}=-g\beta D_{u,e}V_u(w_u)\), for an exterior link entering that star. It has sup norm \(C\sqrt\beta\) and chart gradient bounded by \(C\sqrt\beta\). For either source row \(Y_{t,x}\), sup norm is \(C\beta\) and the squared chart gradient is bounded by \(C\beta^2 e_{t,x}+C\) with its true incident plaquette-energy sum \(e_{t,x}\). This is the finite smooth-word force derivative estimate, using \(|F_{b,i}|^2\le C e_b\); the Casimir has a bounded chart derivative. The same statements hold in compatible nonflat cap coordinates because only fixed translated compact words occur.

At distances \(d<16m+O(1)\) take an enclosing interval with buffers of length at least \(m\) on both sides and total length \(O(m)\). Its bad-exterior probability is \(C m e^{-c\beta}\). On a good exterior, cut away arbitrary endpoint buffers as in §4.106 and consider the inner cap endpoints with both supports a distance at least \(c m\) inside. Under any exterior endpoint law the probability these cuts are outside their small caps is \(C e^{-c\beta}\) by the preceding buffer proof. On the cut-cap interval the weighted covariance bound gives for the mixed insertion a bound
\[
 C e^{-c d}\big(1+\sqrt{\beta\,\mathbb E_{\rm cap}e_{t,x}}\big)
              +C\,\mathrm{poly}(\beta)e^{-c\beta}.
\]
The analogous \(Y,Y\) bound has the product of the two energy gradient norms divided by \(\beta\). In the full inner law the same bounds hold up to the displayed compact-tail errors. When averaging over varying cut endpoints one must also include covariance of the two conditional means. Their oscillations over the allowed cut-cap endpoints are \(C\,\mathrm{poly}(\beta)e^{-c\beta}\): differentiate each local mean in those endpoints, use the endpoint score of §4.106 and the distance \(cm\) in the weighted covariance estimate, bounding the local gradients by \(C\beta\) if necessary. This also handles the arbitrary outer endpoint law on the periodic complement. If the entire time circle is shorter than those buffers, the same positive chart argument on that circle or the direct finite short-interval comparison applies; on the stated asymptotic trajectory \(n\gg m\).

The normalized cap probability is bounded below uniformly for its cut endpoints. Thus its energy moments, integrated over those actual endpoint records, are bounded by the corresponding full conditional moments times a fixed constant. The released and axial laws have the same bounded fixed moments for local quantities here: at fixed shapes the local numerator comparison after omitting the relevant one or two temporal slots costs \(C\,\mathrm{poly}(\beta,n)e^{-cn/\beta}\), and the shape/exterior marginals have the uniform density ratio of §4.105. Squaring and averaging the short-distance bounds uses the axial marked moments (fourth or higher for the two-source product) and conditional Jensen. This yields \(\|\operatorname{Cov}(Y_{t,x},J_{x,u,e}\mid E)\|_{L^2(E)}\) and the corresponding \(Y,Y\) norm bounded by \(C e^{-cd}+C\,\mathrm{poly}(\beta)e^{-c\beta}\) on the stated short range. Together with the long arcs, these norms have uniformly summable time rows and columns. Statements first obtained in the released law return to the original axial conditional covariances: the joint moments with one \(J\), or a second \(Y\), differ pointwise at fixed shape/exterior by a polynomial times \(e^{-cn/\beta}\), and the conditional shape-law ratio satisfies the same estimate. There are only polynomially many temporal slots.

At fixed \(E\) the actual integral is differentiable in each exterior coordinate. Its normalized derivative is precisely
\[
 gD_{u,e}m_{x,t}(E)=
       \operatorname{Cov}_{\rm ax}(Y_{t,x},J_{x,u,e}\mid E).
\]
The original \(Y_{t,x}\) has no \(E\) dependence after the explicit star variables have been chosen. Pure exterior magnetic factors cancel in the conditional normalization. Only boundedly many neighboring \(x\)'s use a given spectator link, and a fixed \(x\) sees boundedly many such links per time. Sum the row and column norms just established; Minkowski for each exterior derivative then gives the Dirichlet energy in (SPATIAL-EXTERIOR-SCORE). The two-source row summed in the true variance decomposition gives the final extensive innovation. This result removes time-long correlations at fixed actual magnetic spectator, including its canonical source response. It has not asserted a Poincaré inequality for \(M_{\rm sp}\) under the remaining interacting spectator law.

### 4.108 Magnetic trace domination for temporal currents and the singlet fourth derivative (P)

The interacting magnetic potential can be kept exactly in a near-identity twist comparison. In the unsourced axial representation choose arbitrary deterministic translations of the spatial group at each time slice, left or right in each oriented link variable, implemented by unitaries \(U_t\). The central kinetic convolution \(\mathsf K_0\) commutes with these translations and is positive. Set \(C=\mathsf K_0^{1/2}B^{1/2}\) and \(D=CC^*\). The trace with these kinetic drifts satisfies
\[
 \left|\operatorname{Tr}\prod_t(C^*U_t C)\right|
 =\left|\operatorname{Tr}\prod_t U_t D\right|
 \le\prod_t\|U_tD\|_n
 =\operatorname{Tr}D^n=\operatorname{Tr}T_0^n .
 \tag{AXIAL-TWIST-DOMINATION}
\]
This is Schatten Hölder; the kernels give the equality with the original drifted two-slice action. In particular each group difference \(u_{t,e}=v_{t+1,e}v_{t,e}^{-1}\) in the independent kinetic factors may be multiplied by a prescribed \(e^{iA_{t,e}}\), with cyclic choice giving a left multiplication inside its class trace. The magnetic factor is kept at its true Wilson coupling.

Let \(L_{t,e}^a=\sqrt\beta\Re\operatorname{Tr}(iT_a u_{t,e})\). For any deterministic real test array \(\zeta\) the full interacting axial law obeys
\[
 \log\mathbb E_{\rm ax}
       \exp\!\left(\sum_{t,e,a}\zeta_{t,e}^a L_{t,e}^a\right)
       \le C_N\sum_{t,e,a}|\zeta_{t,e}^a|^2 .
 \tag{MAGNETIC-LINEAR-CURRENT}
\]
Indeed expand the twist exponent with \(A_{t,e}=\beta^{-1/2}\sum_a\zeta_{t,e}^a T_a\). Its real Taylor error is bounded by \(C_N\beta\sum|A_{t,e}|^2\) everywhere, because the second derivative of the group exponential along a fixed real generator has norm at most its generator norm squared. Apply (AXIAL-TWIST-DOMINATION). In particular the current has zero mean and its covariance on arbitrary deterministically marked linear combinations has a uniform operator bound. The matching combinations use only bounded incidence multiplicity. This comparison is at the true magnetic trace scale, not at the absolute reference one of §4.104.

Here is the exact second-order observable generated by Gaussian mixing of these deterministic rotations. Independently on the selected sites and time slabs take centered real Gaussian Lie coordinates \(\eta_{b,i}^a\) with matching covariance \(P_{ij}=\delta_{ij}-1/3\) and color covariance \(\delta_{ac}\). Apply the same drift \(A=\sqrt{s/\beta}\sum_a\eta_{b,i}^aT_a\) to both increments of matching \(i\) at that star. Let \(\Phi(s)\) be the Gaussian average of the normalized twisted partition at real \(s\ge0\). Then \(0<\Phi(s)\le1\), \(\Phi(0)=1\), and
\[
 (\log\Phi)'(0)=\tfrac12 \mathbb E_{\rm ax}
                 \sum_b(h_b-\tfrac23\ell_b),\qquad
 \left|(\log\Phi)''(0)-
       \tfrac14\operatorname{Var}_{\rm ax}
                 \left(\sum_b(h_b-\tfrac23\ell_b)\right)\right|\le C V .
 \tag{SINGLET-TWIST-CURVATURE}
\]
Here \(\ell_b=C_F\sum_{i,\pm}\Re\operatorname{Tr}u_{i,\pm}\), with the precise original Casimir sign. To check these derivatives, average the drift exponential locally first, writing \(\phi_b(s)\) for its factor at a fixed set of six increments. Its first derivative is half the covariance-\(P\) contraction of the linear change squared plus the action Hessian change. The former is \(h_b\), the latter is \(-\sum_i P_{ii}\ell_{b,i}=-(2/3)\ell_b\). To second order in \(s\), the Gaussian moments through four of the Taylor coefficients in \(\sqrt s\) suffice. Their magnitudes are bounded respectively by \(C\sqrt{\beta e_b}|\eta|,\ C|\eta|^2,\ C\beta^{-1/2}|\eta|^3,\ C\beta^{-1}|\eta|^4\), where \(e_b\) is the six-plaquette energy. Odd powers average to zero. Thus \(|(\log\phi_b)''(0)|\le C(1+(\beta e_b)^2)\). Taylor differentiation is justified at each fixed lattice by Gaussian moment domination of these finite derivatives; alternatively use \(s\downarrow0\) with an even real \(\sqrt s\) expansion. Differentiating the log expectation of the product of the \(\phi_b\)'s adds the *full* variance of its first row, plus the sum of the local second log rows. The true marked moments bound the latter by \(CV\).

This comparison exposes a specific limitation of deterministic-twist domination for the quadratic source. The real upper bound is on \(\Phi(s)\), whose linear response includes the magnetic/Casimir deficit. It does not bound the second curvature at zero by \(CV\). Even a uniformly sub-Gaussian vector can have a superextensive squared-norm variance: take a single independent fair Bernoulli \(B_*\) and set all coordinates \(X_i=B_* Z_i\) for independent unit Gaussians \(Z_i\). Its linear Laplace transform is at most \(e^{\|\zeta\|^2/2}\), whereas \(\operatorname{Var}\sum_i X_i^2\) contains the square of their count divided by four. This elementary example only tests the inference from a linear-current bound; the Wilson statement above is the actual sharp trace inequality and exact curvature identity. The true magnetic singlet response in (SPATIAL-STAR-EXTERIOR) remains necessary.

### 4.109 A slow singlet in the exact remaining spatial exterior, with its measured source response (P)

The canonical Dirichlet estimate (SPATIAL-EXTERIOR-SCORE) cannot be completed by a uniform scalar Poincaré inequality on its actual exterior law. For \(R,S\) of §4.94 there are smooth gauge-invariant scalars \(X_R^{\rm sp}\) depending only on the retained magnetic spatial histories \(E\), with
\[
 \liminf\operatorname{Var}_{\rm ax}X_R^{\rm sp}>0,\qquad
 \mathbb E_{\rm ax}\sum_{u,e,A}|gD_{u,e}^A X_R^{\rm sp}|^2
                         \le C R^{-2}.
 \tag{SPATIAL-EXTERIOR-SLOW-SINGLET}
\]
For the localized constant-pattern comb of §4.95 one also has
\[
 \lim R^2\operatorname{Cov}_{\rm ax}
       \left(\mathbb E_{\rm ax}[Y_{R,w}\mid E],X_R^{\rm sp}\right)
      =\frac{d_G}{4}\int w(x)\,2|\psi(x)|^2\,d^4x>0
 \tag{SPATIAL-EXTERIOR-SLOW-OVERLAP}
\]
with the same choice of \(f,w\) giving a positive overlap there. Thus the slow exterior sector is present in the physical source response, but the response in this probe decreases with \(R\).

Use the smooth canonical magnetic field \(g^{-1}C_N(U_p)\), with \(C_N(U)\) the traceless Hermitian part of \((U-U^\dagger)/(2i)\), agreeing to first order with the plaquette logarithm. Replace the smearing of §4.94 by \(2R^{-2}f(x/R)\) on \(12\)-plaquettes at odd \(x_3\) and zero at even \(x_3\). Each such plaquette is in a spatial plane containing no all-even spatial vertex. For transport to a common spatial base choose paths of length \(O(R)\) staying on the spectator graph: move within an odd \(x_3\) plane to a fixed odd \(x_1\), use that odd \(x_1\) to move between planes, and choose a common base within the resulting spectator planes. For comparisons to the full Wilson model choose short temporal segments at the common spatial base joining the different times; their holonomies are identity in the actual axial fiber. Let \(Z_R^{\rm sp}\) be the summed transported vector and \(X_R^{\rm sp}\) its centered squared coordinate norm. It is a function solely of \(E\).

The underlying full-field gauge-invariant patch observables, their products and the squared norm of their spatial canonical derivatives have the same expectations in the axial fiber and full Wilson law up to a superpolynomially small error. Indeed all their temporal links are in one interval of length \(O(R)\ll n\). Omit that interval from the private times of every column in §4.103. Conditional on all other links, the \(W\) density remains \(1+O(\delta_n e^{C R/\beta})\) uniformly, and the patch functions have at most polynomial sup norms in \(\beta,R\). The sum of squared derivatives is invariant under fine site gauges (the color directions at each spatial base rotate orthogonally). This gives the same comparison for that sum before and after axial gauge fixing.

In the free curl comparison, the added spatial alias is at momentum \(q_3+\pi\). Its contribution to the magnetic variance vanishes: near that point the \(12\)-curl projection has numerator \(a_1+a_2=O(|q|^2)\) while its denominator stays bounded below. Its force-to-magnetic cross symbol has numerator containing \(\widehat q_0\widehat q_1\widehat q_2\), hence is \(O(|q|^3)\) there, two powers smaller than the unaliased linear behavior. The smearing Poisson sum, deep relative images, true noncentral mean and compact-tail errors of §§4.94–4.95 therefore give the same positive limiting variance and cross coefficient. Using \(C_N\) changes only higher-order short-word errors. The conditional expectation in (SPATIAL-EXTERIOR-SLOW-OVERLAP) is exact because this probe is an exterior function.

For the canonical spatial derivatives work pointwise in a good outer chart, with \(\|B_e\|\le T=C S^8\log\beta\) on the relevant paths. Upon differentiating a plaquette factor at canonical velocity \(gT_A\), its leading term is its signed elementary curl incidence. Its adjoint transport on a path of length \(O(R)\) differs from the common chart frame by \(O(gRT)\). The contributions from differentiating the transport itself are commutators bounded by \(C gT\) per traversal. The chosen paths have uniformly bounded multiplicity through any one edge per plaquette; a piecewise coordinate path as above suffices. After summing all plaquette weights the error per used edge in the derivative of \(Z_R^{\rm sp}\) is at most \(C g R^2T\) (the direct local-incidence errors are smaller). Only \(O(R^4)\) spatial edges occur. The leading derivative is the spatial \(12\)-curl adjoint applied to the normalized weights. It differentiates in directions \(1,2\) only: the parity mask in direction 3 costs no derivative. Its squared \(\ell^2\) norm is \(O(R^{-2})\) by smoothness. Thus the true summed squared coordinate errors are \(O(g^2R^8T^2)=o(R^{-2})\) on this chart. The normalized scalar quadratic has gradient bounded by twice \(|Z_R^{\rm sp}|\) times the vector gradient norm; its full fourth moments are bounded by the preceding comparison. The smooth clover word has global derivative bounds polynomial in \(\beta,R\), so compact and bad-boundary tails remain negligible. These estimates prove (SPATIAL-EXTERIOR-SLOW-SINGLET).

In particular any Poincaré constant for all differentiable scalars with the canonical exterior gradient is at least \(cR^2\). The required upper bound is on the covariance of the specific retained \(M_{\rm sp}\) and its full zero mode. The slow-singlet construction alone neither gives nor contradicts that upper bound.

### 4.110 Full-law infrared estimate for the colored connection Laplacian (P)

Let \(T_\mu\) be unitary adjoint parallel shift on site colors of the fine torus, \(H_U=\sum_{\mu=1}^4(2-T_\mu-T_\mu^*)\), and \(P_U=I-H_U/16\). This is the positive lazy covariant walk, with probability \(1/2\) of a hold and \(1/16\) per nearest-neighbor direction. Write \(p_m(x)\) for its scalar free transition probabilities. The actual full Wilson law, including all field histories, satisfies for \(1\le m\le n^{7/3}\)
\[
 \frac1V\mathbb E\operatorname{Tr}P_U^m
 \le C_N p_m(0)\left[e^{-c_N m/\beta}
       +C\exp\!\left(-\frac{c m^{1/4}}{\sqrt{\log(2+m)}}\right)\right].
 \tag{ANNEALED-COLORED-RETURN}
\]
At a fixed root the same upper absolute estimate holds with an additional local factor \(F\) depending on a bounded fixed stencil, times \(C\mathbb E|F|\) with the constant allowed to depend on its stencil size. For all fixed positive integers \(k\),
\[
 \frac1V\mathbb E\operatorname{Tr}(H_U+n^{-2})^{-k}
   \le C_{N,k}\begin{cases}
       1,&k<2,\\
       \log(2+\beta),&k=2,\\
       (1+\beta)^{k-2},&k>2 .
   \end{cases}
 \tag{COLORED-RESOLVENT-MOMENTS}
\]
These estimates are for the lattice covariant one-color propagation. They are integrated trace estimates; no deterministic lower eigenvalue or physical singlet mass gap is asserted.

Expand the diagonal kernel in bridge paths returning to the root. Each nonholding step carries its original adjoint parallel transport. Suppose a bridge has at least \(c m\) unordered edges traversed exactly once in its entire trajectory. A greedy independent subset has at least \(c' m\) members no two of which belong to a common Wilson action plaquette, by the bounded link conflict degree. Remove also the fixed local stencil of \(F\). Given all other links, the private links occur once each in the ordered path word and are conditionally independent. All intermediate matrices are fixed unitaries even if other links recur. The operator norm of the conditional ordered product is therefore at most \(C e^{-c_N m/\beta}\) by §4.98, including inversions. On any other path use the trivial unitary norm one. The path selection is made from the free random walk independently of the Wilson field.

Here are the required finite-torus walk estimates. The lazy scalar characteristic function is \(1-\sum_\mu 4\sin^2(q_\mu/2)/16\in[0,1]\). Fourier summation gives
\[
 \sup_x p_j(x)\le C[(1+j)^{-2}+V^{-1}],\qquad
 p_j(0)\ge c[(1+j)^{-2}+V^{-1}].
\]
For the upper bound dominate nonzero modes by a periodic Gaussian in \(|q|^2 j\). For the lower bound keep the zero mode and momenta of size at most a small constant divided by \(\sqrt{1+j}\). Now consider the unconditioned walk of length \(m\). Split its increments into \(B\asymp m^{1/4}\) disjoint chunks of comparable length \(L\asymp m^{3/4}\le C n^{7/4}\), allowing bounded \(m\) to be absorbed in the final constant.

In any such chunk the expected number of internally once-used edges is at least \(cL\). A given interior step has a fixed probability of being nonholding and never using its unoriented edge again on the preceding and following arms, which have independent increments conditional on the step. Uniformly for these lengths the avoidance has positive probability. To verify it, on \(\mathbb Z^4\) transience follows from \(\sum_jp_j(0)<\infty\). Starting at an endpoint after crossing the chosen edge, require escape from that endpoint with the first step on another edge, an event of positive probability by directional symmetry. The same argument applies backwards. For fixed large \(J\) the torus agrees with the infinite walk on the first \(J\) steps for large \(n\); the probability of a later traversal up to \(L\) is at most \(C/J+C L/V\) by the displayed kernel estimate. Choose \(J\) first. Each chunk therefore has at least \(c'L\) internally once-used edges with probability bounded below, since the count is at most \(L\). These chunk counts are independent. A binomial exponential bound shows their sum exceeds \(c m\) except with probability \(C e^{-cB}\).

It remains to remove edges also visited in another chunk. Their number among the counted steps is bounded by a fixed multiple of the total intersections of vertex visits in different chunks. For two chunks, reverse the earlier one about its final vertex. Its reversed increments, the later chunk increments and the intervening displacement are independent. Thus, uniformly in the relative displacement, the intersection variable \(J_{12}\) has the same upper moment estimate as that of two independent length-\(L\) walks started at arbitrary sites:
\[
 \|J_{12}\|_p\le C p^2\log(2+L),\qquad p\ge1 .
\]
For integer \(p\), expand the \(p\)th moment and order the \(p\) times along each walk, giving at most \((p!)^2\) pairs of orders. Sum the intermediate times of the Markov kernels by \(G_L=\sum_{j=0}^{\lceil C L\rceil}p_j\). Each order pair gives a sum over the \(p\) common sites of the product of two chains of \(G_L\)'s, with arbitrary starts and a permutation of those sites. Cauchy–Schwarz bounds it by \(\|G_L\|_2^{2p}\), since the squared chain sums factor by its increments. But \(\|G_L\|_2^2=\sum_{j,k\le CL}p_{j+k}(0)\le C(\log(2+L)+L^2/V)\le C\log(2+L)\). The bound for other \(p\) follows by increasing to the next integer. Minkowski over all chunk pairs now bounds the \(p\)-norm of the total intersections by \(C p^2 B^2\log(2+m)\). Take \(p\) of order a sufficiently small \(m^{1/4}/\sqrt{\log(2+m)}\). Markov's inequality makes the probability of losing a fixed fraction of \(m\) at most \(C e^{-c m^{1/4}/\sqrt{\log(2+m)}}\). Conditioning the entire trajectory on its return costs at most \(C(1+m)^2\) by the scalar bridge lower bound, absorbed by a smaller stretched-exponential constant. This proves the unique-edge estimate used above and (ANNEALED-COLORED-RETURN).

For (COLORED-RESOLVENT-MOMENTS), expand \((H_U+n^{-2})^{-k}\) as \((16+n^{-2})^{-k}\) times the sum of \(\binom{m+k-1}{k-1}(16/(16+n^{-2}))^m P_U^m\). Up to \(m=n^{7/3}\) the factor \(p_m(0)e^{-c m/n^2}\) is at most \(C(1+m)^{-2}\), including \(m\ge n^2\). Thus the term \(e^{-cm/\beta}\) in the return bound costs the indicated power, critical logarithm or constant, and the stretched exponential has all finite moments. Beyond \(n^{7/3}\) the unitary-path bound \(C p_m(0)\) and the physical regulator give at most \(C_k n^{2k-4}e^{-c n^{1/3}}\). The marked diagonal version follows by the same positive expansion or by taking absolute values of the marked path bound. The proof applies equally to any fixed unitary representation without invariant vectors, with its dimension in the trace constant.

For the full unit comb the covariance with the long-return part of a *single traced covariant propagator* also has an absolute bound obtained by summing the marked diagonal estimate and its product of first moments. For example
\[
 V^{-1}|\operatorname{Cov}(Y,\operatorname{Tr}P_U^m)|
   \le C V p_m(0)[e^{-c m/\beta}
               +C e^{-c m^{1/4}/\sqrt{\log(2+m)}}] .
\]
It is negligible on the macroscopic return range when both exponents dominate \(\log V\). Short returns and singlet products are not covered by that conclusion.

### 4.111 A bounded Wilson-divergence component of the exact zero observable (P)

Let \(\Omega,d_U,D_\mu,F=\tau d_U^*\Omega\) be the original covariant two-form and Wilson link force of §4.39. Define \(\mathsf M\Omega\) as its matching rows \(-D_\nu^*\Omega_{\mu\nu}\), so all three actual directional forces are the vector \(\mathcal F=\tau\mathsf M\Omega\). Write \(\mathsf P\) for the matching difference projection at the actual temporal comb and zero at its other roots. On two-forms take \(H=H_U\) componentwise and \(R_\lambda=(H+\lambda)^{-1}\). At \(\lambda=\beta^{-1/2}\ge n^{-2}\) along the trajectory there is an exact decomposition
\[
 \mathcal F=A_\lambda F+B_\lambda,\quad A_\lambda=\mathsf M R_\lambda d_U,
 \qquad \|A_\lambda\|\le C_N,\qquad
 \mathbb E\|B_\lambda\|_2^2\le C_N V\beta^{-3/2}.
 \tag{REGULATED-HODGE-ROW}
\]
In particular define \(K=A_\lambda^*\mathsf P A_\lambda\) and the original group vector field \(v=KF\) in left-trivialized coordinates. Then the normalized Wilson divergence
\(\delta_\mu v=\beta\langle F,v\rangle-\operatorname{div}v\) has exactly zero mean and satisfies
\[
 \mathbb E(\delta_\mu v)^2\le C_N V .
 \tag{HODGE-WARD-SCORE}
\]
The entire fine torus, all exterior histories and all entries of the matching stencil enter these two assertions.

Indeed \(d_Ud_U^*+d_U^*d_U=H+\mathcal K\), with the bounded-degree commutators \(\mathcal K\) in §4.39. Consequently
\[
 B_\lambda=\tau\mathsf M R_\lambda
          [\,d_U^*d_U\Omega-\mathcal K\Omega+\lambda\Omega\,].
\]
All \(d_U\), \(d_U^*\), \(\mathsf M\) on the corresponding form slots are fixed finite sums and selections of the covariant differences or their adjoints; \(\|D_\nu^*v\|=\|D_\nu v\|\). Hence compositions such as \(\mathsf M R_\lambda d_U\) or \(\mathsf M R_\lambda d_U^*\) have bounded norm by the two \(R_\lambda^{1/2}\) energy bounds. The earlier exact cube word gives \(\mathbb E\|d_U\Omega\|^2\le CV/\beta^2\). Likewise \(\mathcal K\Omega\) is, at each root, a sum of fixed local products bounded by \(C\sqrt{s_p}|\Omega_{p'}|\); its squared expected norm is \(CV/\beta^2\) by the true marked moments. Using \(\|\mathsf M R_\lambda\|\le C/\sqrt\lambda\) and \(\mathbb E\|\Omega\|^2\le CV/\beta\) yields
\[
 \mathbb E\|B_\lambda\|^2
 \le C V(\beta^{-2}+\lambda^{-1}\beta^{-2}+\lambda/\beta),
\]
which proves the specified choice. The full original \(Y^h=\beta\langle\mathcal F,\mathsf P\mathcal F\rangle\) differs from \(\beta\langle F,KF\rangle\) by a variable \(E_\lambda\) with \(\mathbb E|E_\lambda|\le C V\beta^{-1/4}\), by Cauchy–Schwarz and the first force moment. This raw density error is separated from any unproved centered estimate.

Here are derivative bounds for the score. For a unit group derivative in link \(e\) write \(\partial_e\), suppressing its fixed color index. Each \(\partial_eD,\partial_e d_U,\partial_e\mathsf M\) and their adjoints is supported on a fixed neighborhood of \(e\), has bounded norm and finite rank, and their squared actions summed over \(e\) are bounded by \(C\) times the input squared norm by finite overlap. Also
\[
 \|\mathsf M R_\lambda\,1_{N(e)}\|+
       \|d_U^*R_\lambda\,1_{N(e)}\|\le C_N
\]
on any such fixed-size coordinate neighborhood. For example the squared first norm is bounded by a fixed sum of diagonal entries of \(R_\lambda H R_\lambda\preceq R_\lambda\), and \((R_\lambda)_{xx}\) has bounded norm uniformly for \(\lambda\ge n^{-2}\) by scalar free-walk domination in four dimensions, including its zero-mode contribution. No favorable sign of a non-Abelian commutator is needed.

For any vector \(a\), differentiating \(A_\lambda\) gives the four terms with \(\partial_e\mathsf M\), with \(\partial_e d_U\), and with
\(-\mathsf M R_\lambda[(\partial_eD)^*D+D^*(\partial_eD)]R_\lambda d_U\).
The first term summed in squares is at most \(C\|R_\lambda d_U a\|^2\le C\lambda^{-1}\|a\|^2\). For the second use the fixed-neighborhood column bound above. In the subsequent two terms use respectively that column bound and \(\|DR_\lambda d_U\|\le C\), or \(\|\mathsf M R_\lambda D^*\|\le C\) and the bound on \(R_\lambda d_U a\). Thus
\[
 \sum_e\|(\partial_e A_\lambda)a\|^2+
 \sum_e\|(\partial_e A_\lambda^*)b\|^2
     \le C(1+\lambda^{-1})(\|a\|^2+\|b\|^2).
\]
The adjoint estimate follows by the same four displayed factors with \(\mathsf M,d_U^*\) interchanged. By the product rule the same bound holds for \(K\). The derivative array of the actual \(F\) has squared Hilbert–Schmidt norm \(O(V)\) by its fixed stencil and bounded physical Hessians. Further \(\mathbb E\beta\|F\|^2\le CV\) by the original link Ward identity. It follows that \(\mathbb E\|\nabla v\|_{\rm HS}^2+\beta\mathbb E\|v\|^2\le CV\) at this \(\lambda\). The product group Levi–Civita correction to derivatives in the left frame has squared norm \(O_N(\|v\|^2)\).

Finally, integration by parts on the product compact group gives
\[
 \mathbb E(\delta_\mu v)^2
 =\mathbb E\sum_{a,b}(\nabla_a v_b)(\nabla_b v_a)
    +\mathbb E[\operatorname{Ric}(v,v)+\beta\nabla^2 S(v,v)] .
\]
This identity follows by commuting the two covariant derivatives after one further integration by parts; its sign agrees with the scalar weighted Bochner formula on gradient fields. The product Ricci and the Wilson Hessian have uniform operator upper bounds by the group metric and fixed incidence degree. The derivative estimates prove (HODGE-WARD-SCORE). Thus an exact signed full-volume rearrangement is
\[
 Y^h=\delta_\mu v+
         \operatorname{Tr}(K\,\nabla F)+
         (\operatorname{div}K)\cdot F+E_\lambda ,
 \tag{SINGLET-HODGE-RESIDUAL}
\]
where the trace and divergence use covariant derivative in the same group frame. The first summand has extensive variance. The variation of the remaining correlated singlet trace, coefficient divergence and nonlinear residual is still required. A small raw expectation per site does not assert extensive variance.

### 4.112 The covariant terminal low-frequency field on the required physical torus (P)

The long colored propagation estimate controls open paths in moments, which is needed when the adjoint endpoints are actual Wilson curls. On the trajectory \(\beta=O(\log n)\), take \(n^{-2}\beta^{-2}\le\lambda\le1\) and \(R_\lambda=(H_U+\lambda)^{-1}\). For every fixed positive integer \(p\),
\[
 \begin{aligned}
 \big\|\beta\,\|\lambda R_\lambda\Omega\|_{\ell^2}^2\big\|_{L^p(\mu)}
     &\le C_p V\lambda^2\min(\lambda^{-1},1+\beta)^2,\\
 \big\|\beta\,\|\lambda\mathsf M R_\lambda\Omega\|_{\ell^2}^2
                                                   \big\|_{L^p(\mu)}
     &\le C_p V\lambda^2\min(\lambda^{-1},1+\beta).
 \end{aligned}
 \tag{TERMINAL-COLORED-LOWPASS}
\]
At \(\lambda=n^{-2}\) the first bound is \(O_p(\beta^2)\), negligible on the \(\sqrt V\) scale of the zero comb. At \(\lambda=n^{-2}\beta^{-2}\) it is \(O_p(\beta^{-2})\), and the second is \(O_p(\beta^{-3})\). In particular deleting just this artificial mass term from the exact directional-force reconstruction changes the full quadratic comb by \(o(\sqrt V)\) in \(L^2\) at the latter regulator. This is an actual full-law estimate on a possible infrared sector; the nonlinear Bianchi and commutator terms and the singlet trace are separate.

To prove the bounds, the open kernel expansion for \(\langle\Omega,R_\lambda^k\Omega\rangle\) has paths with two true local curl endpoints and coefficient bounded by \(C_k(m+1)^{k-1}(16/(16+\lambda))^m\). For a \(p\)-fold product take independent free walks with the specified lengths and arbitrary starting points; sum those starts over \(V^p\). Their endpoints are determined by the walks. If \(M=\max m_j\le n^{7/3}\), the longest path has at least \(c_p M\) unordered edges used just once in the union of all the paths, except with probability
\(C_p e^{-c_p M^{1/4}/\sqrt{\log(2+M)}}\).
For details, split the longest path into \(O(M^{1/4})\) independent chunks of comparable length as in §4.110. Split all other paths into chunks of length at most the same. The longest path has at least \(cM\) internally once-used edges except on the stated small-probability event. Intersections with the other paths cost in moment order \(h\) at most \(C_p h^2 M^{1/2}\log(2+M)\). Indeed for chunks of different paths their relative starting displacement is independent of both chunks' own increments, so the two-Green-chain estimate of §4.110 applies uniformly. Within the long path use reversal about the end of its earlier chunk as before. Choose the same high moment and subtract the possible lost edges. Short other paths require at most one extra chunk each.

Choose a noninteracting private subset of the surviving edges and delete all \(2p\) endpoint stencils. Conditional on the other links, every chosen group variable occurs once, in only one of the ordered matrix factors; integration contracts the product of the absolute endpoint-contraction bounds by \(e^{-c_N M/\beta}\). At the true endpoints the expectation of the product of their \(2p\) curl norms is at most \(C_p\beta^{-p}\) by the marked moments and Hölder. This estimate is uniform over the walk endpoints, also when they coincide. On the exceptional walks use their trivial unitary bound instead. Thus after summing the path lengths, the exponential in \(M\) costs \(C_p\min(\lambda^{-1},1+\beta)^{kp}\); the stretched exponential costs only a fixed constant at fixed \(k,p\). For lengths beyond \(n^{7/3}\), the geometric factor even at the smallest \(\lambda\) costs \(e^{-c n^{1/3}/\beta^2}\), dominating every fixed power of the volume. Consequently
\(\|\langle\Omega,R_\lambda^k\Omega\rangle\|_{L^p}\le C_{k,p}(V/\beta)\min(\lambda^{-1},1+\beta)^k\) for \(k=1,2\), and likewise for each fixed \(k\). Use \(k=2\) for the first displayed bound and \(R_\lambda\mathsf M^*\mathsf M R_\lambda\preceq C R_\lambda\) with \(k=1\) for the second. These are moment estimates of actual positive quadratic forms.

Finally \(\|\beta\|\mathcal F\|^2\|_{L^2}\le CV\) by the fixed local marked moments. The change in its projected quadratic on subtracting \(B_{\rm mass}=\tau\lambda\mathsf M R_\lambda\Omega\) is bounded in \(L^2\) by \(C\sqrt V\|\beta\|B_{\rm mass}\|^2\|_{L^2}^{1/2}+C\|\beta\|B_{\rm mass}\|^2\|_{L^2}\), using Cauchy–Schwarz twice. This proves the claimed negligible change. Smallness of a charged covariant lowpass does not give smallness for a color-singlet squared field after the two colors have already been contracted.

### 4.113 The microscopic singlet plaquette row from the admitted smooth action source (P under the stated I-1 clause)

One scalar nuisance in the global twist/score reduction does have an extensive bound under the allowed interface. Take the fixed finite family of six *smooth constant-test, dimension-four* oriented Wilson action densities, normalized as \(a^4\sum_x 1\,(Na^4)^{-1}s_{p_\alpha(x)}=N^{-1}S_\alpha\), \(\alpha=(\mu,\nu)\), \(S_\alpha=\sum_x s_{p_\alpha(x)}\). I-1's fixed pressure polydisc for this finite family gives a zero-free disc of fixed radius \(R_\alpha>0\) for \(\mathbb E e^{zS_\alpha}\), after putting back the fixed \(N\). This use concerns the ordinary smooth tensor components of the additive action density. It neither uses a physical dimension-six source disc nor treats an oscillatory comb as a smooth physical test. If only the scalar action rather than the six tensor components is admitted, the following full mixed-mark conclusion requires the corresponding orientation extension.

On the reference trajectory and the even tori considered above, for *every* microscopic real plaquette mark \(f\) we obtain
\[
 \operatorname{Var}_\mu\!\left(\sum_{x,\alpha}f_{x,\alpha}s_{p_\alpha(x)}\right)
      \le \frac{C_{N,R}}{\beta}\sum_{x,\alpha}|f_{x,\alpha}|^2 .
 \tag{ADDITIVE-PLAQUETTE-SUS}
\]
To verify the constant-source estimate first, for \(|z|\le R\le\min_\alpha R_\alpha/2\) use positivity of all plaquette energies and
\[
 \log|\mathbb E e^{z S_\alpha}|
 \le\log\mathbb E e^{R S}
 =\int_0^R \mathbb E_{\beta-u} S\,du
 \le C_R V/\beta .
\]
The last comparison is §4.11's full-tree/temporal-forest plaquette first moment, valid also at each fixed additive shift of the coupling for large \(\beta\). Cauchy on the normalized holomorphic log with this one-sided bound gives \(\operatorname{Var}S_\alpha\le C_R V/\beta\).

It remains to infer the microscopic marks without using a microscopic source disc. A single oriented plaquette has slab width at most **one** in every axis. For an axis in its plane the insertion lies between successive site slices and is a self-adjoint insertion kernel after real smearing in transverse coordinates: reversal of the slab swaps the ends and reverses the loop orientation, leaving its real trace unchanged. For a transverse Fourier smearing \(k\) its adjoint is the insertion for \(-k\). At distinct slab separation \(1\le l\le n-1\), the spectral trace contains terms
\[
 \lambda_i^{\,n-l-1}\lambda_j^{\,l-1}
          |\langle j,O_k i\rangle|^2 /\operatorname{Tr}T^n\ge0 .
\]
When \(k=0\), centering the diagonal summands leaves the variance of \(O_{ii}/\lambda_i\) with weights \(\lambda_i^n/\operatorname{Tr}T^n\), and the off-diagonal terms stay nonnegative. Zero eigenvalues can equivalently be handled by continuity; the positive Wilson transfer is on its physical sector as in §4.29. For an axis outside the plane this is a one-slice multiplication insertion and the same nonnegative spectral covariance follows with the extra ordinary transfer step. The \(l=0\) contact is independent of the longitudinal Fourier frequency. Consequently the single-orientation structure factor is bounded above upon setting *any* one longitudinal Fourier coordinate to zero. Repeat for all axes to get \(S_{s_\alpha}(p)\le S_{s_\alpha}(0)=\operatorname{Var}S_\alpha/V\) on the original unsampled lattice. Parseval proves the result for one oriented mark. The triangle inequality in \(L^2\) followed by Cauchy–Schwarz across the six orientations proves (ADDITIVE-PLAQUETTE-SUS), with their fixed factor in \(C_{N,R}\). Unlike the frustration star there is no two-wide transverse support requiring a parity alias in this argument.

In particular the original centered Casimir sum on the unit comb is a bounded-multiplicity linear plaquette mark. Its \(L^2\) norm is \(O(\sqrt{V/\beta})\). Thus on the allowed smooth-action input the variance in (SINGLET-TWIST-CURVATURE) differs in square-root norm from the actual full \(Y^h\) by \(O(\sqrt{V/\beta})\); the extensive SUS conditions are equivalent. The same conclusion holds in the axial fiber by the local second-moment comparison of §4.103, also for a product of a plaquette mark and a root. The smooth constant action estimates therefore dispose of this definite singlet linear row, including microscopic placements on a two-face sheet. Nonlinear correlated singlet traces and the magnetic spectral curvature remain.

### 4.114 A local curvature regulator in the genuine Wilson Hodge score (P)

The arbitrary intermediate mass in §4.111 can be replaced by the actual local curvature size, with the remaining fixed infrared regulator below the physical scale. Set \(\epsilon=n^{-2}\beta^{-2}\) and let
\[
 W_x=C_N\sum_{p\ {\rm within\ fixed\ distance\ of}\ x}
                  \sqrt{s_p+\epsilon^2},\qquad R=(H+W)^{-1}.
\]
Use a fixed neighborhood containing all the plaquettes of each commutator term in \(\mathcal K\Omega(x)\). \(W\) acts by scalar multiplication at each site. Its link derivatives have fixed support and uniformly bounded norm because \(|D_e s_p|\le C\sqrt{s_p}\). It is smooth at every finite cutoff. With \(A=\mathsf M R d_U,\ K=A^*\mathsf P A\), both (REGULATED-HODGE-ROW) and (HODGE-WARD-SCORE) hold with this field-dependent choice, the same \(CV\beta^{-3/2}\) error for the directional force and the same \(CV\) score variance. The proof provides full-law estimates for the random propagators created by differentiating the coefficient.

Since \(H,W\preceq H+W\), the operators \(\mathsf M R d_U\), \(\mathsf M R d_U^*\) and \(\mathsf M R W^{1/2}\) have uniformly bounded norms by the energy factorization. The remainder is now
\[
 \tau\mathsf M R [\,d_U^*d_U\Omega+(W-\mathcal K)\Omega\,].
\]
The first part is bounded by \(C\|d_U\Omega\|\). At each root \(W_x^{-1/2}\mathcal K\Omega\) is bounded by a fixed sum of \((s_p+\epsilon^2)^{1/4}|\Omega_{p'}|\) on neighboring plaquettes, by the definition of \(W\) and the commutator estimate of §4.39. \(W^{1/2}\Omega\) has the same bound. The expected squared norms are \(O(V\beta^{-3/2})\) by the full marked moments, including \(\epsilon\). This proves the new directional-force row. It remains important to control its derivative in the actual fields rather than freezing \(W\).

Here is a convenient propagator estimate. In the symmetric walk expansion write \(H+W=D^{-1}(I-16D P_U D)D^{-1}\) with \(D=(16+W)^{-1/2}\). Each visited site therefore contributes a scalar factor \((1+W_x/16)^{-1}\), up to bounded endpoint factors. In a path expansion containing a fixed finite number of resolvents and bounded fixed-range shift matrices between them, the longest independent free walk segment of length \(m\le n^{7/3}\) visits \(c m\) distinct sites except with the stretched-exponential error proved in §4.110. Other segments and a bounded number of fixed local jumps need not avoid any of these sites. From them choose at least \(c'm\) separated sites and for each one choose a fixed incident plaquette and a private link in it. Keep these links out of any specified local endpoint stencils. They can be chosen so that the plaquettes are disjoint, each contains only its own private link, and no two private links share an action plaquette. Given the complement in the full Wilson law, their kernels are independent, with sup Haar densities \(C_N\beta^{d_G/2}\). With conditional probability bounded below each witness has \(\sqrt{s_p}\ge c_0/\sqrt\beta\), since a smaller defect would force a group ball of radius \(C c_0/\sqrt\beta\) in its private link. Therefore the *absolute value* of the averaged walk weight costs
\[
 C e^{-c m/\sqrt\beta}
       +C e^{-c m^{1/4}/\sqrt{\log(2+m)}} .
 \tag{ADAPTIVE-WALK-KILLING}
\]
For the first part drop all other killing factors and all parallel-transport norms, and multiply the independent bounds on \((1+W_x/16)^{-1}\), one per witness. Local endpoint marks remain in the exterior; Hölder bounds them by their true marked moments. This argument also works for products of finitely many words by using the longest segment anywhere in the expansion. Beyond \(n^{7/3}\) the deterministic \(W\ge c\epsilon\) gives the previously sufficient factor \(e^{-c n^{1/3}/\beta^2}\). Thus a word containing \(k\) resolvents and a fixed number of finite local shift insertions costs at most \(C_k(1+\sqrt\beta)^k\) after summing path lengths and endpoints per starting site, times the true Hölder bounds of its local endpoint fields. This estimate does not replace the rough law by a model of independent site masses.

For the derivative calculation write \(u=R d_U F\). The exact Hodge identity gives
\[
 u=\tau\,[\,\Omega+R j\,],\qquad
 j=(\mathcal K-W)\Omega-d_U^*d_U\Omega .
\]
The local field \(j\) has each fixed \(L^p\) norm \(O_p(1/\beta)\): the differentiated cube remainder still has bounded degree and the \(W\Omega\) term uses neighboring \(\sqrt{s_p}|\Omega|\). Meanwhile \(\Omega\) has local norm \(O_p(1/\sqrt\beta)\). Apply (ADAPTIVE-WALK-KILLING) to the two endpoint local fields in \(\|R j\|^2\), using two resolvents. This gives
\[
 \mathbb E\|u\|^2\le C V/\beta .
\]
Let \(u'=R\mathsf M^*\mathsf P A F=R O u\) with \(O=\mathsf M^*\mathsf P\mathsf M\), a sum of finitely many bounded local shifts (comb zero rows included). In \(\|R O\Omega\|^2\) there are two resolvents, hence cost \(O(V)\) using the two \(\Omega\) endpoints. In \(\|R O Rj\|^2\) there are four and the two \(j\) endpoints give the same \(O(V)\). The finite shift terms in \(O\) can simply be bounded in norm in these positive absolute estimates. Thus \(\mathbb E\|u'\|^2\le CV\).

Differentiate \(A\) using \(H=D^*D\) and the additional term \(-\mathsf M R(\partial_e W)R d_U\). The two-sided energy bounds remain true. The local-column bound for \(\mathsf M R\) and \(d_U^*R\) also remains true, since \(R H R\preceq R\) and \(R\preceq(H+c\epsilon)^{-1}\); its diagonal is bounded in four dimensions, including the constant mode \(O((V\epsilon)^{-1})\). The derivative calculation of §4.111 therefore gives the sharper pointwise estimate
\[
 \sum_e\|(\partial_e A)a\|^2
    \le C(\|a\|^2+\|R d_Ua\|^2),
\]
with the corresponding adjoint estimate using \(R\mathsf M^* b\). In fact the \(\partial_e W\) term uses its bounded local rank and \(\mathsf M R\) on that fixed support, and all the remaining terms are exactly those already bounded. Use \(a=F\), then \(b=\mathsf P A F\). The two previous estimates on \(u,u'\) yield \(\mathbb E\sum_e\|(\partial_e K)F\|^2\le CV\). The true compact weighted divergence identity of §4.111 proves the claimed extensive score for this curvature-adapted field. The remaining scalar trace and nonlinear residual are still correlated singlets; this calculation does not claim their variance is extensive.

### 4.115 A signed second-divergence reduction with an \(O(V)\) contact (P)

A second integration by parts can remove the leading score from the *signed* covariance, without leaving a factor \(\sqrt{\operatorname{Var}Y}\) in its bound. Use \(K=A_\lambda^*\mathsf P A_\lambda\) of §4.111, now with \(\lambda=\beta^{-1/100}\), and \(E_\lambda=Y^h-\beta\langle F,KF\rangle\). In the true full Wilson law one has
\[
 \begin{split}
 \operatorname{Var}Y^h
   ={}& \frac1\beta\mathbb E\!\left[
          \operatorname{Tr}(K\nabla^2Y^h)
            +2\langle\nabla Y^h,\operatorname{div}K\rangle\right]\\
     &+\operatorname{Cov}\left(Y^h,\,
       \operatorname{Tr}(K\nabla^2S)+\beta^{-1}\operatorname{divdiv}K+E_\lambda
                         \right),\\
 &\left|\frac1\beta\mathbb E[
          \operatorname{Tr}(K\nabla^2Y^h)
              +2\langle\nabla Y^h,\operatorname{div}K\rangle]\right|\le C V .
 \end{split}
 \tag{SIGNED-HODGE-COVARIANCE}
\]
All divergences use the product group Levi–Civita connection and volume. The raw bound from (REGULATED-HODGE-ROW) gives \(V^{-1}\mathbb E|E_\lambda|\le C\beta^{-1/200}\) at this choice. A uniformly bounded covariance of the three scalar residuals, after summing them with their original signs, is sufficient for the exact targeted zero.

For the identity, integration by parts twice for the symmetric contravariant tensor \(K\) and any scalar \(G\) gives
\[
 \mathbb E\operatorname{Tr}(K\nabla^2 G)
 =\mathbb E G[
  \operatorname{divdiv}K-2\beta(\operatorname{div}K)\cdot F
  -\beta\operatorname{Tr}(K\nabla^2S)+\beta^2\langle F,KF\rangle] .
\]
This is the product rule for the double divergence of \(e^{-\beta S}K\); in particular the entire row has mean zero at \(G=1\). Apply it to centered \(Y^h\). One more ordinary score identity for \(\operatorname{div}K\) gives
\(\beta\operatorname{Cov}(Y^h,(\operatorname{div}K)\cdot F)=
 \mathbb E\langle\nabla Y^h,\operatorname{div}K\rangle+
 \operatorname{Cov}(Y^h,\operatorname{divdiv}K)\). This proves the formula, including the plus sign of its double-divergence residual.

For uniform estimates \(\|K\|\le C,\ \operatorname{Tr}K\le CV\) and \(\|\nabla^2Y^h\|\le C\beta\) by the finite stencil. Also \(\mathbb E\|\nabla Y^h\|^2\le C\beta V\) by the true force gradient bound. The absolute row and column sums of the block norm of \(R_\lambda\) are bounded by \(1/\lambda\), directly by the scalar walk majorant. Corresponding absolute norms of \(d_U,\mathsf M\) and their adjoints are bounded. For a derivative on an edge, \(d_U,\mathsf M,H\) have finite local derivative matrices whose absolute sum over all edge/color choices still has bounded row and column norms. In a first derivative of \(K\) there are at most three resolvent factors, via \(\partial R_\lambda=-R_\lambda(\partial H)R_\lambda\). Sum the absolute derivative matrices over their anchoring links *before* the row and column sums; the local bound just noted applies inside each product. Thus each entry of the vector divergence has sup norm at most \(C(1+\lambda^{-3})\). Product-group frame connection terms have the same bound by their fixed link support. Two derivatives similarly give total scalar absolute size \(C V(1+\lambda^{-4})\) for \(\operatorname{divdiv}K\). The first of these estimates gives
\(\beta^{-1}|\mathbb E\langle\nabla Y^h,\operatorname{div}K\rangle|
 \le C V(1+\lambda^{-3})/\sqrt\beta\), proving the claimed contact estimate.

One can bound the vacuum-subtracted scalar trace pointwise without assuming analyticity of its full sourced pressure. Set \(T_\lambda=\operatorname{Tr}(K\nabla^2 S)+\beta^{-1}\operatorname{divdiv}K\). On the periodic torus
\[
 |T_\lambda(U)-T_\lambda(I)|\le
    C \lambda^{-20}\sum_p s_p
       +C V\lambda^{-20}e^{-c\lambda n}.
 \tag{HODGE-TRACE-ENERGY}
\]
Here are explicit loose powers sufficient for the displayed estimate. Expand its two resolvents as covariant lazy path sums. For total walk length \(m\) the absolute coefficient sum per spatial root is at most \(C(m+1)^3e^{-c\lambda m}\): one factor \(m+1\) for the split between the two resolvents and at most \((m+C)^2\) derivative placements. Finite local shifts in \(d_U,\mathsf M\), the single Wilson Hessian and the two connection coefficients have only bounded multiplicity. Divergence contractions force the differentiated edge to coincide with its position in the word, so they do not add independent free anchor sums. Equivalently expand each original path polynomial first and differentiate its bounded-degree occurrences termwise. For each rooted path and placement sum the generator/color contractions before estimating; it is a gauge-invariant scalar, from the covariant path rule and the bi-invariant connection. In the case of differentiated generators this means summing their complete orthonormal frames at their actual anchors. Each resulting word with \(m+C\) factors has bounded sup and a bound \(C(m+1)^2\) on its second derivative along simultaneous bounded link displacements. At identity its first derivatives vanish by common conjugation invariance and the absence of an invariant linear form on \(\mathfrak{su}(N)\).

For \(m<n/C\), tree-gauge its contractible coordinate box of side \(C(m+1)\). Each chord has a filling of at most \(C(m+1)^2\) plaquettes, so its bounded logarithm squared is at most \(C(m+1)^4\sum_{p\in B(x,C(m+1))}s_p\), also when a principal chart is left by compactness and the telescoping unitary-word bound. Taylor on the simultaneous geodesic from the identity therefore costs at most \(C(m+1)^6\) times that local sum. After summing roots, each plaquette occurs at most \(C(m+1)^4\) times. Summing the path coefficients costs at most \(C\lambda^{-14}\sum_p s_p\), smaller than the conservative displayed power. For \(m\ge n/C\) just use the bounded word terms and the exponential path tail. This proves (HODGE-TRACE-ENERGY). The optional real \(L^p\) statement at each fixed order follows with the marked moments, giving at this \(\lambda\) an \(O(\beta^{-4/5})\) upper bound on its normalized raw size at any fixed order after vacuum subtraction.

The linear plaquette row separately has the centered estimate (ADDITIVE-PLAQUETTE-SUS). The pointwise energy majorant for the entire trace does not transfer that centered bound to every nonlinear loop in it. The last covariance in (SIGNED-HODGE-COVARIANCE), rather than the contact or the terminal colored regulator, is the outstanding signed term in this formulation.

### 4.116 Complete quadratic covariance estimates for total Wilson forces (P under the smooth plaquette clause)

One extensive singlet class within the Hodge expansion can be controlled exactly. For every deterministic real matrix \(K\) on the original left-trivialized link/color space,
\[
 \operatorname{Var}_\mu\bigl(\beta\langle F,KF\rangle\bigr)
          \le C_N\|K\|_{\rm HS}^2 .
 \tag{TOTAL-FORCE-QUADRATIC-SUS}
\]
Only (ADDITIVE-PLAQUETTE-SUS) uses the admitted smooth oriented action inputs; the score contribution is an unconditional Wilson estimate. It is enough to take \(K\) symmetric. In particular every deterministic quadratic Fourier or Riesz form of the *total* force with Hilbert–Schmidt norm \(O(\sqrt V)\) has extensive ordinary variance. An adapted \(K(U)\) is not covered simply by evaluating this estimate configuration by configuration.

The exact identity \(\beta\mathbb E F_a F_b=\mathbb E X_a F_b\) follows by Haar integration by parts. Its matrix has bounded row and column sums from the fixed Wilson stencil. It follows that \(\beta\mathbb E\|K F\|^2\le C\|K\|_{\rm HS}^2\). The total squared derivatives of \(v=K F\) are bounded by \(C\|K\|_{\rm HS}^2+C\|v\|^2\) in the product connection, since the left-frame derivative of \(F\) has bounded operator norm. The divergence identity of §4.111 therefore gives \(\mathbb E(\delta_\mu v)^2\le C\|K\|_{\rm HS}^2\).

In the left invariant frame the remaining divergence is \(Z=\sum_{a,b}K_{ab}X_a X_b S\); the compact unimodular frame has zero divergence in each of its basis directions. Group the summands by action plaquette. Under independent site gauge averaging two generator indices at different base sites give zero scalar component. At the same base, averaging the two indices gives their invariant contraction by the trace against \(\delta_{AB}/d_G\), since the adjoint representation of \(SU(N)\) is irreducible. For repeated differentiation in one edge the color sum is its original plaquette Casimir times \(\Re\operatorname{Tr}U_p\). For the two distinct positively oriented edges with the same base and in one plaquette, the generator insertions are adjacent cyclically at that common vertex with opposite orientation sign, and their color sum is again a fixed signed Casimir times that same real trace. Thus the invariant part of \(Z\) is exactly a deterministic linear plaquette mark plus an identity constant; its squared mark norm is \(C_N\|K\|_{\rm HS}^2\) or smaller by finite incidence. Section 4.113 bounds its variance accordingly.

For the noninvariant remainder subtract the site gauge average separately at each plaquette. Two such zero-average terms on disjoint site sets have zero expectation of their product: independently average their gauge variables in the same Wilson integral. Only boundedly many neighboring plaquettes per root can contribute. Each local term has sup norm bounded by a constant times the sum of absolute \(K\)-entries on that plaquette's fixed link/color stencil. The sum of their squared sup norms is at most \(C_N\|K\|_{\rm HS}^2\). This proves the same variance bound for all nonsinglet terms. Together with the exact score decomposition it proves (TOTAL-FORCE-QUADRATIC-SUS).

There is a useful covariant extension for a prescribed family of simple paths. Index pairs \((b_i,c_i)\) of distinct Wilson link origins, with fixed bounded multiplicity at each endpoint. Let \(\gamma_i\) transport from the base of \(b_i\) to that of \(c_i\), avoid both marked links, and have length \(l_i\). If the endpoints share no action plaquette, then
\[
 \operatorname{Var}_\mu\left(\beta\sum_i f_i
       \langle F_{b_i},\operatorname{Ad}(U_{\gamma_i})F_{c_i}\rangle\right)
     \le C\sum_i |f_i|^2(1+l_i/\beta).
 \tag{TRANSPORTED-TOTAL-FORCE-SUS}
\]
This part does not require the smooth action disc. Use the vector field which at \(b_i\) places \(f_i\operatorname{Ad}(U_{\gamma_i})F_{c_i}\). Its ordinary group divergence is zero: the path avoids \(b_i\) and \(F_{c_i}\) is independent of that link. Its Wilson divergence is the displayed observable exactly. The expectation of \(\beta\|v\|^2\) is \(C\sum_i f_i^2\) by endpoint multiplicity and the original local force moments. Derivatives hitting \(F_{c_i}\) cost the same fixed sum by finite degree. Each differentiated simple path contributes its length times \(C f_i^2\mathbb E|F_{c_i}|^2\) to the squared derivatives, after Cauchy–Schwarz only over the bounded number of terms at the same vector endpoint. The compact score formula gives the result without any requirement of disjoint paths in the rest of the lattice.

One may also allow an incident pair when its connecting path avoids both marked links and is the intervening plaquette segment between their generator insertions. Its divergence trace then contributes a fixed signed Casimir times \(\Re\operatorname{Tr}U_p\), and (ADDITIVE-PLAQUETTE-SUS) pays the additional marks with bounded incidence. For example take opposite parallel edges of one plaquette and connect their bases by its lower transverse edge: parallel transport brings the two generators adjacent in its cyclic trace. These estimates eliminate explicit principal score and elementary contact sectors of (SIGNED-HODGE-COVARIANCE). They do not identify the full field-dependent loop trace there with a deterministic matrix.

### 4.117 The actual compact quartic diagonal and its constant singlet component (P under the stated smooth families)

The diagonal part of the exact compact normal correction \(N_b\) from §4.60 has uniform susceptibility including the microscopic comb. For a single based plaquette \(P\), let
\[
 n(P)=\Pi_\perp(P-I),\qquad Q(P)=\|n(P)\|_{\rm HS}^2
       =2s(P)-\operatorname{Tr}(C_N(P)^2).
\]
Here \(\Pi_\perp\) projects off the traceless anti-Hermitian tangent matrices using the real Hilbert–Schmidt metric. The two terms on the right have already specified smooth constant-test dimension-four lattice action densities: the additive Wilson action of §4.113 and the canonical \(F_{\mu\nu}^2\) discretization of §2.1. Their joint I-1 polydisc gives a fixed *additive* zero-free radius for \(\sum_x Q(P_\alpha(x))\), with no fine oscillation in its test. Moreover \(0\le Q(P)\le C_N s(P)^2\) globally, since the normal projection has zero first jet at identity. For any fixed real radius \(r\) within this additive disc,
\[
 \log\mathbb E e^{r\sum_x Q(P_\alpha(x))}\le C_r V/\beta^2 .
\]
Indeed \(e^{r Q(P)}-1\le(C_r/\beta^2)e^{\epsilon\beta s(P)}\) for a small fixed \(\epsilon\), using \((\beta s)^2\) under the exponential. Expand the positive product and apply the true marked-set exponential to every subset of plaquettes; then sum its binomial majorant. Cauchy for the one-sided log gives \(\operatorname{Var}\sum_x Q(P_\alpha(x))\le C V/\beta^2\). This real scalar is inversion invariant and has width at most one in every axis. The unsampled transfer argument of §4.113 therefore gives, for every real microscopic mark,
\[
 \operatorname{Var}_\mu\left(\beta\sum_p f_p Q(U_p)\right)
       \le C\sum_p f_p^2 .
 \tag{COMPACT-NORMAL-DIAGONAL-SUS}
\]
Each actual diagonal term of \(N_b\) is such a mark with bounded incidence, including an arbitrary parity pattern. In \(SU(2)\), \(Q=s^2/2\) exactly. For every \(SU(N)\) a parallel statement for \(s^2\) follows from the fixed smooth family of additive action densities in the fundamental and its two tensor products, using
\(s^2=2N s-\tfrac12(s_{F\otimes F}+s_{F\otimes\bar F})\), \(s_\rho=d_\rho-\Re\chi_\rho\). Each of these fixed one-plaquette actions has the usual dimension-four quadratic classical limit. No fixed disc for the physical \(a^{-4}\)-amplified sum of squares is used.

There is also a constant-test result for the *entire* normal correction. Specify the finite smooth additive family precisely: take, besides the elementary actions, the local actions \(s(PQ),s(PQ^\dagger)\) and
\(s_\otimes(P,Q)=N^2-\Re(\operatorname{Tr}P\operatorname{Tr}Q)\),
\(s_\otimes(P,\bar Q)=N^2-\Re(\operatorname{Tr}P\,\overline{\operatorname{Tr}Q})\), for each pair of original based, oriented plaquette words at a mark. Each \(a^4\sum a^{-4}\) times one such action is a fixed short-loop or tensor-product dimension-four lattice discretization with a smooth constant test. Its classical leading terms are quadratic in the two continuum curvatures, by expansion at identity and tracelessness. Apply the I-1 smooth finite-family clause to exactly these realizations; if an amended I-1 is restricted to only a smaller list of lattice realizations, this particular cross-term conclusion requires their admission.

There is an exact all-field identity
\[
 \langle n(P),n(Q)\rangle
  = s(P)+s(Q)-\tfrac12[s(PQ)+s(PQ^\dagger)]
       +\frac{s_\otimes(P,Q)-s_\otimes(P,\bar Q)}{2N}.
 \tag{CROSS-NORMAL-ACTION-FAMILY}
\]
In fact \(n(P)=\Re P-I+i(\Im\operatorname{Tr}P/N)I\) in Hermitian matrix conventions. The real Hilbert–Schmidt inner product of the Hermitian parts gives the first three terms; the two imaginary trace components give the last term. Thus \(N_b/\beta\) for the original sum of squared matching normal differences is a fixed linear combination of these additives, while \(0\le N_b/\beta\le C\sum_{p\ni b}s_p^2\). With all temporal sites included, its constant-test partition function has the stated fixed additive disc. The same marked-product bound, now using bounded overlap, gives
\[
 \operatorname{Var}_\mu\left(\sum_{\text{all temporal }b}N_b\right)\le C V .
 \tag{UNIFORM-NORMAL-SINGLET}
\]
This specifically pays the constant fine Fourier component of the quartic correction. The mixed pairs in its parity aliases have a different support/reflection geometry from a single plaquette, so (COMPACT-NORMAL-DIAGONAL-SUS) has not been extended to them by the same argument.

Likewise \(h_b/\beta\) can be expanded in a fixed sum of additive local dimension-four action realizations of this kind: contract the real generator parts of the same plaquette words, or use §4.60's complex staple Hilbert–Schmidt squares minus the displayed normal squares. Terms \(\Re\operatorname{Tr}(P^\dagger Q)\) are the same fixed closed actions up to their constants. Its all-sites constant-test variance, under that finite family's I-1 disc, is at most \(C V/\beta\) before multiplication by \(\beta^2\), since \(h_b/\beta\le C\sum_{p\ni b}s_p\). Thus the unamplified **uniform** temporal frustration sum has the global bound \(C\beta V\). This is weaker than the requested \(CV\), and controlling the seven nonconstant aliases is still necessary for the unit comb. These conclusions separate exactly which singlet rows use smooth actions and which still depend on full microscopic exterior transport.

### 4.118 Testing an absolute staple recursion on typical \(SU(2)\) Wilson records (P)

The uniform one-link representation contraction of §4.98 does not give a contraction when its average is split into individual neighboring staples. In fact the natural absolute row expands on the *true typical* weak-coupling exterior, already at its first correction. Use the six unit quaternion staple vectors \(w_j\) from §4.59, \(k=\sum_j w_j\), \(e=k/|k|\) when nonzero, \(\gamma=2\beta|k|\), and \(m(\gamma)=\mathbb E_\gamma(u\cdot e)\). The exact one-link mean is \(m(\gamma)e\). Then
\[
 \mathbb E_\mu\frac{6m(2\beta|k|)}{|k|}
       =1+\frac{1}{8\beta}+o(\beta^{-1}).
 \tag{UNSPLIT-STAPLE-ROW}
\]
Even allowing for each input's actual tangent-plane constraint does not reverse that sign. For a uniform unit \(v\in e^\perp\), the maximum directional derivative of the mean along \(v\) over independent unit tangent variations at each of the six neighbors is
\[
 L_v=\frac{m(2\beta|k|)}{|k|}
                 \sum_{j=1}^6\sqrt{1-(v\cdot w_j)^2},\qquad
 \mathbb E_{\mu,v} L_v=1+\frac{1}{24\beta}+o(\beta^{-1}) .
 \tag{ROUGH-TANGENT-NONCONTRACTION}
\]
For temporal spins with fixed spatial links, varying their six neighboring temporal spins varies these six transported staples by independent tangent isometries, so this is an actual conditional response row. It rules out a proof based on a strict average contraction of its absolute one-step tangent coefficients. It does not show that the signed scalar frustration susceptibility diverges.

To check the constants set \(\phi=12-2|k|=\sum_j|w_j-e|^2\), the true minimum of the star energy. Formula §4.92 gives \(\lim\mathbb E\beta e_b=9/2\): the limiting canonical curl covariance per fixed plaquette and per color has diagonal \(1/(2\tau)\) by the symmetry of its Fourier multiplier \((a_\mu+a_\nu)/a\). The plaquette energy gives \(\tau/2\) per squared coordinate and \(d_G=3\), hence \(3/4\) for each of six plaquettes. On this very same star, conditionally \(e_b=12-2u\cdot k\). Uniformly away from degenerate \(k\), \(m(\gamma)=1-3/(2\gamma)+O(\gamma^{-2})\), by the one-dimensional Laplace expansion of its density \(e^{\gamma z}(1-z^2)^{1/2}\) at \(z=1\). The difference in expected \(\beta e_b\) from \(\beta\phi\) therefore tends to \(3/2\). Nonregular stars have true probability \(Ce^{-c\beta}\), the compact energy is bounded, and \(\mathbb E\phi^2=O(\beta^{-2})\) by (STAR-MISMATCH-TAIL) and the marked moments. In particular \(\mathbb E\beta\phi\to3\).

Since \(|k|=6-\phi/2\), one obtains on regular exteriors
\[
 \frac{6m(2\beta|k|)}{|k|}
    =1+\phi/12-1/(8\beta)+
                     O(\phi^2+\phi/\beta+\beta^{-2}).
\]
On the other records \(m(\gamma)/|k|\le C\beta\) by the smooth finite-\(\gamma\) formula, so the expansion suffices in expectation and gives (UNSPLIT-STAPLE-ROW). For \(v\perp e\), the radial derivative drops out and the tangential differential of the normalized vector mean is \(m(\gamma)/|k|\) times the projection orthogonal to \(e\). Project each independently varied input onto its own tangent plane, obtaining \(L_v\). Averaging the square of \(v\cdot w_j\) over its three-dimensional sphere gives \([1-(e\cdot w_j)^2]/3\); summed over \(j\) this equals \(\phi/3+O(\phi^2)\). The fourth-power Taylor errors are \(O(\phi^2)\) on regular stars. Therefore the sum of the six square roots is \(6-\phi/6+O(\phi^2)\) after this angular average. Multiplying and using \(\mathbb E\beta\phi\to3\) proves (ROUGH-TANGENT-NONCONTRACTION).

The dangerous common tangent cannot be identified with the physical scalar without its relative signs. At fixed exterior the exact \(SU(2)\) frustration mean depends only on the Gram data of the six staple quaternions, as in §4.59. It is invariant under a common orthogonal rotation of all of them. Hence for its derivative one may subtract any common skew rotation from all six tangent variations exactly. Absolute scalar row summation before this subtraction discards precisely the cancellation which (ROUGH-TANGENT-NONCONTRACTION) tests.

### 4.119 Arbitrarily exterior-adapted, off-diagonal total-force kernels on the true comb (P)

Let \(\mathcal E\) fix all links except the selected temporal comb. Set \(X_b=\sqrt\beta F_b\), the full Wilson force, and permit an arbitrary real symmetric matrix \(K(\mathcal E)\) on these link/color slots, measurable in the entire actual rough exterior. Conditional independence gives the exact singlet separation
\[
 \begin{split}
 \mathbb E[X^TKX\mid\mathcal E]
    &=\sum_b\operatorname{Tr}\big[K_{bb}(\mathcal E)\,
                   \mathbb E(\nabla_b^2 S\mid\mathcal E)\big],\\
 \mathbb E\operatorname{Var}(X^TKX\mid\mathcal E)
    &\le C_N\,\mathbb E\|K(\mathcal E)\|_{\rm HS}^2 .
 \end{split}
 \tag{ADAPTED-COMB-TOTAL-FORCE}
\]
Hence if the diagonal blocks vanish, the displayed upper bound controls the *full* ordinary variance of this nonlocally adapted scalar, without an independence assumption on the exterior. The remaining response for other such matrices is exactly the covariance of the indicated diagonal exterior Hessian row.

For each selected link, conditional Haar integration gives \(\mathbb E(F_b\mid\mathcal E)=0\) and
\(\beta\mathbb E(F_b^a F_b^c\mid\mathcal E)=\mathbb E(X_b^a F_b^c\mid\mathcal E)\), with antisymmetric connection part zero by the first identity. The Hessian has a uniform norm bound on every compact exterior, including degenerate staples. Also \(\mathbb E(\beta^2|F_b|^4\mid\mathcal E)\le C\) uniformly: apply the same divergence identity to \(|F_b|^2 F_b\) and use its bounded physical force derivative along with the just-proved second moment. Thus the \(X_b\) are independent centered color vectors conditional on the exterior, each with uniformly bounded fourth moment. Expanding the covariance of their diagonal quadratic terms gives at most \(C\sum_b\|K_{bb}\|_{\rm HS}^2\). Off-diagonal pairs have mean zero, are uncorrelated with the diagonal terms, and only an identical or reversed pair survives by independence and centering. Their total variance is at most \(C\sum_{b\ne c}\|K_{bc}\|_{\rm HS}^2\). This proves the formulas. A general curvature or matching force is not itself one of these conditionally centered total forces; that is why an adapted diagonal row or another singlet can survive in the original \(Y^h\).

### 4.120 The smooth additive energy route and its exact non-Abelian remainder (P reduction)

The \(1/\beta\) in (ADDITIVE-PLAQUETTE-SUS) is enough for the original Casimir but would need another power to give extensive susceptibility after multiplying a plaquette mark by \(\beta\). A much weaker additional thermal input than a proportional complex coupling disc would suffice for this scalar: on the fixed additive source interval suppose the actual oriented mean satisfies \(\mathbb E_{\beta,z} S_\alpha/V=c_\alpha/\beta+O(\beta^{-2})\) uniformly, where \(z\) couples additively only to the chosen orientation and the same leading \(c_\alpha\) holds. Then integrating this slope after subtracting its exact zero value yields a one-sided centered log bound \(C V/\beta^2\) on the already admitted additive disc. Cauchy and the original one-plaquette transfer imply \(\operatorname{Var}(\beta\sum f_p s_p)\le C\sum f_p^2\). The displayed real next-order error on that anisotropic interval is not an I-1 clause. Knowing only the scalar isotropic thermal energy would not control each anisotropic response if off-diagonal terms cancel.

For the isotropic mean one principal vacuum term in a proposed proof cancels *exactly*, including on rough fields. Let \(v=d_U^*R_\lambda\Omega\), with \(R_\lambda=(H+\lambda)^{-1}\) on color-site fields acting identically on the 2-form components. With the original generator norm, let \(\mathrm d\Omega[X]\) denote the left link variation of the based plaquette field. At identity it is \(d_U X\). Away from identity its difference \(L_U=\mathrm d\Omega-d_U\) is supported on the original plaquette stencil and has entries bounded by fixed neighboring plaquette defects: this follows by differentiating the four ordered group factors, transporting each generator to its base and comparing the two possible plaquette paths; any mismatch is multiplication by that plaquette or its adjoint minus identity. Equivalently the two paths differ by its holonomy, and differentiating \(C_N(P)\) at \(P\) differs from its Lie projection at \(I\) by \(O(\|P-I\|)\). Then the first term in \(\operatorname{div}v\) is
\[
 \operatorname{Tr}_{2{\rm -forms}} R_\lambda d_U d_U^*
   =3\sum_{\mu=1}^4\operatorname{Tr}_{\rm sites,color}
                     R_\lambda D_\mu D_\mu^*
   =3\,[d_G V-\lambda\operatorname{Tr}_{\rm sites,color}R_\lambda] .
 \tag{EXACT-ENERGY-RANK-TRACE}
\]
To check it, the trace over the six 2-form component indices of
\(\varepsilon_\mu\iota_\nu\) is \(3\delta_{\mu\nu}\). Each unitary shift gives \(D_\mu D_\mu^*=D_\mu^*D_\mu\), without commutation of different shifts. The other two contributions in the divergence are precisely
\[
 \operatorname{Tr}(d_U^*R_\lambda L_U)
  -\sum_{e,A}
     [\,d_U^*R_\lambda(\partial_e^A H)R_\lambda\Omega\,]_{e,A}.
\]
Indeed \(\partial_e^A d_U^*\) has zero row at that same link: the matched codifferentials there involve only shifts in the *other* directions. The left invariant frame has zero basis divergence.

Under full Wilson integration \(\mathbb E\operatorname{div}v=\beta\mathbb E\langle F,v\rangle\). Its left energy pairing is
\[
 \tau^{-1}\langle F,v\rangle
   =\|\Omega\|^2
       -\langle d_U\Omega,d_U R_\lambda\Omega\rangle
       +\langle\mathcal K\Omega,R_\lambda\Omega\rangle
       -\lambda\langle\Omega,R_\lambda\Omega\rangle .
\]
At \(\lambda=n^{-2}\beta^{-2}\) the last term has normalized expectation times \(\beta\) bounded by \(C\lambda\beta\) by §4.112. Also \(\operatorname{Tr}R_\lambda/V\le C\) by scalar diamagnetic domination including its finite-box zero mode. The actual difference between \(S\) and \((\tau/2)\|\Omega\|^2\) has per-site expectation \(O(\beta^{-2})\) by the compact normal projection and marked moments. The remaining mixed curvature terms and differentiated inverse in these two identities have not been shown to cancel to the required next relative order, uniformly in the microscopic torus. This records exactly which part of the rank/equipartition argument is proved and which signed estimate would still be needed even before its anisotropic version.

### 4.121 Positive inverse on the exact spatial exterior and an axial Ward identity on every spectral band (P)

Use exactly the temporal axial fiber and spatial spectator marginal of (SPATIAL-STAR-EXTERIOR). Write \(V=n^4\), \(w(E)\,dE=d\nu\), \(F=M_{\rm sp}-\nu M_{\rm sp}\), \(g=\beta^{-1/2}\). On each finite torus \(w\) is smooth and strictly positive, by integrating the compact smooth strictly positive joint density. Put \(d=g\nabla\) on scalars and \(L=d^*d\) in \(L^2(\nu)\). This elliptic operator on the connected product of compact groups has a complete eigenbasis \(1,\phi_j\), with positive eigenvalues \(\lambda_j\) off the constants. On the closure of exact one-forms put \(L_1=dd^*\), equivalently use the weighted Hodge Laplacian restricted there. Its positive eigenforms \(d\phi_j/\sqrt{\lambda_j}\) are orthonormal and complete on that space. With \(P\) and \(P_1\) the two spectral resolutions, the positive inverse formula and its exact dyadic version are
\[
 \begin{split}
 \operatorname{Var}_\nu M_{\rm sp}/V
 &=V^{-1}\langle dF,L_1^{-1}dF\rangle
 =\int_{(0,\infty)}\lambda^{-1}d\sigma(\lambda),\\
 \sigma(B)&=V^{-1}\|P_1(B)dF\|^2
 =V^{-1}\sum_{\lambda_j\in B}\lambda_j|\nu(F\phi_j)|^2 .
 \end{split}
 \tag{MAGNETIC-EXTERIOR-SPECTRAL}
\]
Real eigenfunctions may be chosen throughout. The integral on \([1,\infty)\) is uniformly bounded by (SPATIAL-EXTERIOR-SCORE). On \((0,1)\) it is comparable within a factor two to \(\sum_{j\ge0}2^j\sigma((2^{-j-1},2^{-j}])\). This formula uses the positive inverse on *one-forms*. Applying the scalar inverse to \(F\) itself instead computes its integrated dynamical correlation. Time translation, spatial translations by two cells and all residual time-independent spatial gauge transformations act isometrically on \(d\nu\) and commute with \(L\). The source lies in their common invariant sector, including any degenerate singlets there.

For any spatial axial vector field \(v\) on the full joint group, let \(G\) be its centered joint weighted divergence with canonical derivative \(g\nabla\), and \(v_E\) its components on the retained links. Then
\[
 \mathbb E(G\mid E)=d^*\mathbb E(v_E\mid E),\qquad
 V^{-1}\|P((0,r])\mathbb E(G\mid E)\|^2
       \le r V^{-1}\mathbb E|v_E|^2 .
 \tag{ALL-SINGLET-WARD-BAND}
\]
Integration by parts against each smooth spectator test gives the first equality in the distributional sense. Bessel's inequality on the displayed orthonormal exact forms gives the second. In particular an interior-only axial divergence has zero projection on *every* spectator eigenspace, without any gap assumption. Applying the original unfixed Wilson temporal-link divergence to arbitrary axial spectator eigenfunctions would require a different derivative and is unnecessary here.

There is a concrete family of such fields for the actual comb. Orient all six incident spokes out of each marked spatial vertex as in §4.105, and orient the spectator edges arbitrarily. In these spatial group coordinates \(v_{t,e}\), set \(u_{t,e}=v_{t+1,e}v_{t,e}^{-1}\), \(s(u)=N-\Re\operatorname{Tr}u\), and \(J_{t,e}^a=\sqrt\beta(\partial^a s)(u_{t,e})\) for a left derivative. Reversing a spoke conjugates or inverts its increment as already accounted for by the outgoing coordinate. All colors at a marked vertex use that vertex's frame. Let \(K\) be the fixed symmetric nonnegative matrix on each time slice which takes the six currents at each marked site, adds the two in each opposing pair, and takes the squared norm of their three-way difference projection \(I-\mathbf1\mathbf1^T/3\). It is zero on spectator slots. Thus \(Y=\langle J,KJ\rangle\) is exactly the unamplified frustration comb. Its diagonal on each spoke is \(2/3\) times color identity.

For \(1\le R\le n\) put \(A_R B_t=R^{-1}\sum_{j=0}^{R-1}B_{t-j}\). Choose the periodic mean-zero temporal primitive \(D_R\) solving \((D_R B)_{t+1}-(D_R B)_t=(I-A_R^*A_R)B_t\). It has a real convolution kernel \(k_j\) with \(\sum_j k_j^2\le C R\). To see this, on the integer line take the cumulative sums of \(\delta_{j0}-(R-|j|)_+/R^2\) with the index shifted by one. They vanish outside \([-R,R]\), have modulus at most one, and solve \(k_{j+1}-k_j=\delta_{j0}-(R-|j|)_+/R^2\). Periodize and subtract their mean; overlap is bounded for \(R\le n\). The two coincident derivative coefficients obey \(k_1-k_0=1-1/R\) also at \(R=n\).

Write \(\mathcal B_{t,e}=\sqrt\beta\,\partial_{t,e}S_{\rm sp}\) for the actual spatial Wilson force on its time slice, and \(v=D_R KJ\) for a canonical vector field whose values are tangent vectors in those group coordinates. In the axial conditional expectation the full identity is
\[
 M_{\rm sp}=
 \mathbb E\!\left[
 \|K^{1/2} A_R J\|^2-\langle\mathcal B,D_RKJ\rangle
 +(1-R^{-1})\sum_{t,e}K_{ee}^{\rm dir}\,
                    C_F\Re\operatorname{Tr}u_{t,e}\;\middle|\;E\right].
 \tag{MAGNETIC-FILTER-WARD}
\]
Here \(K_{ee}^{\rm dir}\) is the scalar diagonal of \(K\) at the spatial edge. Indeed the canonical kinetic action gradient at \((t,e)\) is \(J_{t-1,e}-J_{t,e}\): the Lie current of the class function \(s\) commutes with its increment, so the left and right endpoint derivatives have precisely opposite signs. Pairing that gradient with \(D_R KJ\) gives \(Y-\|K^{1/2}A_RJ\|^2\) on the periodic time circle. In the canonical divergence of this field, only \(J_{t-1,e}\) and \(J_{t,e}\) are differentiated. Their color traces are respectively \(+C_F\Re\operatorname{Tr}u_{t-1,e}\) and \(-C_F\Re\operatorname{Tr}u_{t,e}\); summing at all times gives the displayed Casimir coefficient. The spatial part of the action gradient contributes exactly \(\langle\mathcal B,D_RKJ\rangle\). All components of \(D_RKJ\) are on integrated spokes, so its normalized divergence has zero conditional expectation. This proves the equality on the true compact marginal including at \(R=n\).

The cost of this primitive is controlled on rough records after averaging: \(\mathbb E|D_R KJ|^2\le CVR\) by (MAGNETIC-LINEAR-CURRENT) applied to its deterministic rows. The same proof with a bounded deterministic time-independent spatial matrix having spectator rows, bounded operator norm and color-scalar entries gives \(V^{-1}\|P((0,r])\mathbb E(G\mid E)\|^2\le C rR\) for its actual joint divergence \(G\). This is a low-band bound simultaneously on all singlets and on every torus. For the displayed comb its divergence projection vanishes exactly. Also the sub-Gaussian fourth moment for each row gives
\[
 \big\|\,\|K^{1/2}A_RJ\|^2\,\big\|_{L^2}\le CV/R .
\]
Indeed each temporal average has fourth-root fourth moment at most \(C/\sqrt R\), and the number of slots is \(O(V)\). At \(R=n\) the first term of (MAGNETIC-FILTER-WARD) is supported entirely on the static temporal currents. Its raw second-moment bound per volume is \(O(V/n^2)\). This fact and the band bound on divergences alone leave the centered mixed spatial stress and the correlations of the static singlets. They cannot be discarded by counting the \(O(n^3)\) static slots. The signed Casimir row has extensive variance under the particular smooth orientation-resolved plaquette clause used in §4.113, independently of this exact Ward identity.

### 4.122 All low singlets of the quadratic spectator problem on the full torus (P, quadratic comparison)

The whole spectral projection can be computed in the quadratic axial Wilson problem at every torus size. This is a benchmark for (MAGNETIC-FILTER-WARD), including the spatially varying longitudinal polarizations that would be missed by inspecting a transverse wave packet. It does not assume that the nonlinear Wilson density is Gaussian. In canonical spatial link coordinates the Fourier Hessian at temporal momentum \(p_0\) is
\[
 H(p)=a_0 I+d_s^*d_s,\qquad a_0=4\sin^2(p_0/2).
\]
Freeze the static null directions (or retain the independent massive static Gaussian coordinates). The source is independent of *all* static coordinates because its current is \(J=\partial_0 A\). Spatial period two of \(K\) merely mixes its spatial aliases. No temporal alias is introduced. For \(p_0\ne0\), \(H\ge a_0 I\); the spectator precision \(S(p_0)\), obtained by integrating the spokes, thus also satisfies \(S(p_0)\ge a_0 I\), by minimizing the full quadratic form over the other coordinates.

Whiten the full Gaussian field. Its source is then \(z^TCz\), where \(C\ge0\), \(\|C\|\le C_N\): explicitly \(C=H^{-1/2}\partial_0^*K\partial_0 H^{-1/2}\) and \(H\ge\partial_0^*\partial_0\). The centered conditional source on whitened spectator coordinates is given by the compression of this same matrix to the Euclidean subspace measured by those coordinates (the other Gaussian trace is constant). Its matrix \(C_E\) therefore has the same norm bound. Diagonalize the true *quadratic spectator* generator \(L_{\rm q}\) using real normal coordinates of its precision \(S\), with eigenvalues \(s_i\) on the first chaos. The complete centered source lies in its second chaos. The off-diagonal products \(z_i z_j\), \(i<j\), and the diagonal \((z_i^2-1)/\sqrt2\) have eigenvalues \(s_i+s_j\) and \(2s_i\). The degree-two source is orthogonal to every other Hermite degree. Consequently for \(0<r\le1\)
\[
 \begin{split}
 \frac{1}{V}\|P_{L_{\rm q}}((0,r])F_{\rm q}\|^2
 &= \frac{2}{V}\sum_{s_i+s_j\le r}|(C_E)_{ij}|^2
 \le \frac{C}{V}\#\{i:p_0(i)\ne0,\ a_0(i)\le r\}\\
 &\le C\sqrt r .
 \end{split}
 \tag{QUADRATIC-COMPLETE-SINGLET-BAND}
\]
For real sine/cosine blocks one can choose the diagonalization in the subspaces with the same \(a_0\). The nonzero temporal frequencies satisfying \(a_0\le r\) number at most \(C n\sqrt r\) including when \(n\sqrt r<1\), by the elementary sine bound on the periodic grid. There are at most \(C n^3\) spatial/color modes per frequency. The row-square sum of the matrix is at most \(\|C_E\|^2\) per low coordinate. This proves the estimate for the entire projection, including all spatial alias and polarization combinations, with the static sector absent for the stated reason. In one-form conventions it gives \(\sigma_{\rm q}((0,r])\le C r^{3/2}\), which is summable with the inverse weight down to arbitrarily small eigenvalues on the growing tori. Translation symmetries allow restriction to the singlet of the constant mask throughout.

On the actual compact law the currents are Lie gradients of the group increments, and the marginal generator has an interacting, field-dependent drift even at zero total translation momentum. In particular \(S(p_0)\ge a_0 I\) is a bound on a quadratic *field* Hessian; it has not been proved for the scalar eigenmodes of \(L\) on compact spin networks. Equation (MAGNETIC-FILTER-WARD) specifies what the compact replacement must estimate: with \(R=n\), all \((0,r]\) projections of the centered conditional static current square minus the mixed magnetic stress, with the Casimir retained whenever its smooth source clause is unavailable. A uniform summable dyadic bound for that actual signed combination remains open.

### 4.123 Localization of the true conditional static current row in the spectator spectrum (P)

Let \(Z_n(E)=\mathbb E(\|K^{1/2}A_n J\|^2\mid E)\) be the static term of (MAGNETIC-FILTER-WARD). On the stated tori, for large \(\beta\) with \(\beta=O(\log n)\), the full spatial exterior law obeys
\[
 \frac{1}{V}\|dZ_n\|_{L^2(\nu)}^2\le C_N\,\frac{\beta^7}{n^2},\qquad
 \frac{1}{V}\|P([u,\infty))(Z_n-\nu Z_n)\|^2
      \le \frac{C_N\beta^7}{n^2 u}\quad (u>0).
 \tag{STATIC-CURRENT-SPECTRAL-WINDOW}
\]
In particular all eigenmodes with \(\lambda\ge n^{-2+\epsilon}\) together contribute \(o(V)\) to the variance of this row for each fixed \(\epsilon>0\). These estimates concern arbitrary singlet eigenfunctions of the true nonlinear marginal, irrespective of their particle number or field content.

Expand the static square into \(n^{-1}\sum_{x,t,s}(J_{x,t},K_xJ_{x,s})\) with the fixed-dimensional bounded matrix \(K_x\). Conditional on the entire relative shape history \(w\) at \(x\), use the angular variables of §4.105. In a frame based at \(g_t\), each outgoing current on slab \(t\) has size at most \(C\sqrt\beta\) and is a function of \(\xi_t,w_t,w_{t+1}\). The change of frame from time \(s\) to time \(t\) in the scalar product inserts the adjoint of the intervening product of \(\xi\)'s. Choose a shorter periodic arc of length \(\ell=d_n(t,s)\). Integrate first the complementary angular variables. Uniformly in the shapes their convolution density on the prescribed closing element is \(1+O(\mathrm{poly}(\beta)e^{-cn/\beta})\), since the complementary unmarked arc has length at least \(n/2-2\); this is the private-product bound of §§4.98,4.105. The denominator has the same uniform comparison. On the remaining arc the individual increments can now be integrated independently. Each unmarked intermediate slot has adjoint mean of operator norm at most \(1-c/\beta\), including for noncentral staples. The \(SU(N)\) adjoint has no trivial summand. The two endpoint insertions are bounded by \(C\beta\) in product. Thus, up to uniform error \(\mathrm{poly}(\beta)e^{-cn/\beta}\), the conditional scalar product is a function \(b_{ts}(w)\) of just the shapes on this arc with its one-slice collar, satisfying
\[
 |b_{ts}(w)|\le C\beta e^{-c\ell/\beta}.
\]
The two choices at an even temporal antipode obey the same estimate. The periodic rotor correction to the shape law also has the uniform comparison of §4.105. All these normalization factors depend only on shapes; estimates of their omitted contribution to a covariance with a magnetic exterior derivative can therefore be made by multiplying their uniform errors by the sup norms of the insertions.

Fix a neighboring spectator edge \(e\) on slice \(u\). The canonical derivative of the conditional static mean at this star is exactly \(n^{-1}\sum_{t,s}\operatorname{Cov}(b_{ts},J_{x,u,e}\mid E)\), up to a polynomial in \(n,\beta\) times \(e^{-cn/\beta}\). Here \(J_{x,u,e}=-g\beta D_{u,e} V_u(w_u)\) is the exterior magnetic score of §4.107 with sup norm \(C\sqrt\beta\), distinct from the temporal current \(J_{t,e}\). This assertion follows by differentiating the original compact positive normalized integral: the observable and its rotor integral do not explicitly involve \(E\), and the pure spectator magnetic and kinetic weights cancel. Release comparisons are made at the level of covariances, so the proof requires no bound on the derivative of a small relative error.

For distance \(d\) from \(u\) to the arc support, the \(L^2(E)\) covariance norm is at most \(C\beta^{3/2}e^{-c\ell/\beta}\), directly by the two sup norms. For \(d\ge16m+O(1)\), \(m=\lceil C_2\beta\rceil\), it is at most this bound times \(Ce^{-c'd}\). Indeed freeze the whole arc support. Only its two endpoints transmit boundary influences to the remaining open periodic arc. The positive-kernel contraction across its separated good bridges on *each* side of \(u\) gives precisely the product estimate of §4.107. Conditioning on a whole contiguous interval introduces two endpoints, regardless of the length of the interval. The joint rare-witness bound applies on those two remaining arcs under the genuine \(E\) average. For each \(\ell\) there are at most \(C(\ell+\beta)\) choices of the initial time whose support is within this short distance of \(u\); the exponential tails in \(d\) add only a bounded number in the weighted sum. The number of shorter-arc orientations is at most two. Hence the derivative at this edge has norm at most
\[
 \frac{C\beta^{3/2}}{n}\sum_{\ell\ge0}(\ell+\beta)e^{-c\ell/\beta}
          +\mathrm{poly}(n,\beta)e^{-cn/\beta}
 \le C\beta^{7/2}/n .
\]
Only a bounded number of stars use each exterior edge, there are \(O(V)\) edge/color/time slots, and spectral comparison above \(u\) uses \(\|dZ_n\|^2=\int\lambda\,d\|P(\lambda)Z_n\|^2\). This proves the window estimate. It uses the time-dependent angular conditional law on the full rough exterior throughout. The estimate leaves the static row below the window and leaves the mixed magnetic stress of (MAGNETIC-FILTER-WARD) on both sides. An energy bound on \(Z_n\) does not control the inverse-weight integral at the lower endpoint.

### 4.124 Removing the entire static sector by a separated Ward test (P)

A temporal filter with a signed remainder removes the static-current term on *all* magnetic spectator eigenmodes. For \(1\le m\le n/2-2\) put \(v_{t}=\sum_{j=1}^m KJ_{t-j}\) and \(L_{\rm C}=\sum_{t,e}K_{ee}^{\rm dir} C_F\Re\operatorname{Tr}u_{t,e}\). The same compact integration by parts as in §4.121, now with \(v_{t+1}-v_t=K(J_t-J_{t-m})\), gives exactly
\[
 M_{\rm sp}=
 \mathbb E[L_{\rm C}-\langle\mathcal B,v\rangle\mid E]+e_m(E),\qquad
 e_m(E)=\mathbb E\!\left[\sum_t\langle J_t,KJ_{t-m}\rangle\mid E\right].
\]
For every compact exterior, with no smooth-source polydisc,
\[
 |e_m(E)|\le C V\beta
       \big[e^{-c m/\beta}+\mathrm{poly}(\beta)e^{-cn/(C\beta)}\big] .
 \tag{SEPARATED-MAGNETIC-WARD}
\]
This follows from the same conditional adjoint-product calculation as in §4.123, applied to each of the \(O(V)\) root-time pairs at their *single* separation \(m\). No near-diagonal temporal products occur. The bound is pointwise because only the angular integrations were used, before the arbitrary shape and spectator averages. Take \(m=\lceil A\beta\log n\rceil\) with \(A\) a sufficiently large fixed constant. Then \(\|e_m-\nu e_m\|_{L^2(\nu)}=o(\sqrt V)\) on the trajectory, including its projection at every eigenvalue below the diffusion scale. The primitive itself satisfies \(\mathbb E\|v\|^2\le C Vm\) by the actual deterministic-current sub-Gaussian estimate. Here the source remains precisely the original unit comb. Only the Ward vector field has temporal range \(m\).

There is also an exact spatial decomposition of the remaining virial. Each one-odd spatial site \(y\) has precisely two incoming marked spokes \(e,e'\) from neighboring all-even sites. At each time pull the desired velocities from their outgoing frames into the common endpoint frame by \(q_e=-\operatorname{Ad}(\sigma_e^{-1})v_e\), where \(\sigma_e\) is the current spatial group variable. Choose a slice site-gauge velocity \(a_y=(q_e+q_{e'})/2\) at each such \(y\), zero at other sites. Write \(G(a)_e=a_x-\operatorname{Ad}(\sigma_e)a_y\) for its induced edge velocity on any oriented \(e:x\to y\), and put \(D_e=v_e-G(a)_e\) on the internal spokes \(I\). In endpoint frames the two residual velocities at \(y\) are \((q_e-q_{e'})/2\) and its negative. On spectators let \(W=G(a)_E\), extending by zero on the internal spokes. These fields satisfy
\[
 \begin{split}
 \|P((0,r])\,\mathbb E[d_{\rm ax}^*W\mid E]\|^2/V&\le C r m,\\
 M_{\rm sp}
 =\mathbb E[L_{\rm C}-\langle\mathcal B_I,D\rangle
       -\langle J_{t-1,E}-J_{t,E},W_{t,E}\rangle_{t,E}
       +d_{\rm ax}^*W\mid E]+e_m(E).
 \end{split}
 \tag{SPATIAL-GAUGE-WARD-SPLIT}
\]
Here \(d_{\rm ax}^*\) is the canonical adjoint for the full axial joint density. To verify signs, slice gauge invariance implies \(\langle\mathcal B,G(a)\rangle=0\) pointwise, even for a field-dependent gauge velocity. Hence \(\langle\mathcal B_I,v\rangle=\langle\mathcal B_I,D\rangle-\langle\mathcal B_E,W\rangle\). The ordinary spectator Haar divergence of \(W\) is zero: the site velocities depend only on the discarded spokes, and for fixed such velocities \(W\) is an infinitesimal left/right Haar-preserving transformation on spectator edges. Therefore \(d_{\rm ax}^*W=\langle\mathcal B_E+J_{t-1,E}-J_{t,E},W\rangle\). The degree bound of the spatial graph and unitarity of each endpoint transport give \(\mathbb E\|W\|^2\le C\mathbb E\|v\|^2\le CVm\). Apply (ALL-SINGLET-WARD-BAND). For instance the divergence has only \(o(V)\) squared projection on all eigenvalues \(\lambda\le n^{-\epsilon}\) together at any fixed \(\epsilon>0\).

The two unresolved terms are spatially explicit. Write \(\tilde B_e=-\operatorname{Ad}(\sigma_e^{-1})\mathcal B_e\) at the common endpoint. The internal stress at each \((t,y)\) is exactly \((\tilde B_e-\tilde B_{e'})\cdot(q_e-q_{e'})/2\). Conditional on \(E\) the two neighboring star trajectories are independent, since a spatial plaquette touches only one star. Consequently its conditional expectation is the sum of the two single-star covariances \(\operatorname{Cov}(\tilde B_i,q_i\mid E)/2\) and the product \((\overline{\tilde B}_e-\overline{\tilde B}_{e'})\cdot(\bar q_e-\bar q_{e'})/2\), with bars denoting the respective conditional means and the color covariances contracted. The spectator kinetic term is an actual time-current pairing with the endpoint mean; its electric currents belong to \(E\) itself. The minimizing property of the arithmetic average is exact: the sum of the two squared velocity discrepancies for any site velocity \(a\) is \(|q_e-q_{e'}|^2/2+2|a-(q_e+q_{e'})/2|^2\). Thus the two neighboring directional velocities cannot both be transferred by that single site gauge rotation unless their transported values agree. Neither this pointwise discrepancy nor a torus-volume count bounds the variance of its signed magnetic stress. A summable low-band or centered norm bound on the remaining two terms is required for the original Wilson susceptibility.

### 4.125 Eliminating all parity aliases by a one-slice directional Ward replacement (P under the smooth plaquette clause)

Let \(S_h(p)=V^{-1}\operatorname{Var}_{\mathbb C}(\sum_{b\parallel0}e^{ipx_b}h_b)\) be the ordinary fine-lattice structure factor of the full Wilson measure; the complex variance uses the squared modulus after centering. Then for all temporal and spatial fine momenta and all admissible even tori,
\[
 \sqrt{S_h(p)}\le C_N+\sqrt{S_h(0)},\qquad
 \operatorname{Var}_\mu(r_f)\le C_N[1+S_h(0)]\sum_b|f_b|^2 .
 \tag{FINE-UNIFORM-WARD-REDUCTION}
\]
Here the pressure clause used for ordinary plaquettes is the six-component smooth additive action clause of §4.113. The converse implication is necessary as well: take \(f=1\) on all temporal links and zero otherwise and apply the bounded Ward contact to pass between \(r\) and \(h\). Thus a single *fine-uniform*, smooth constant temporal \(h\) susceptibility suffices. No microscopic or cell-comb source analyticity is used in this reduction.

Fix a spatial axis \(i\), with \(j,k\) the other two, in the original Wilson link variables. Put \(R_b=F_{b,j}+F_{b,k}\), with the *unscaled* directional Wilson forces from §2.3, and set
\[
 q_{i,b}=\beta\,[\,|F_{b,j}|^2+|F_{b,k}|^2+|R_b|^2\,].
\]
Because \(F_{b,i}=F_b-R_b\), one has the exact pointwise identity
\[
 h_b-q_{i,b}
  =\beta F_b\cdot[(2/3)F_b-2R_b] .
\]
For all deterministic complex coefficients \(f_b\) supported on temporal bonds,
\[
 \operatorname{Var}_{\mathbb C}
        \sum_b f_b(h_b-q_{i,b})\le C_N\sum_b|f_b|^2 .
 \tag{DIRECTIONAL-WARD-COST}
\]
Indeed take the ordinary physical vector field \(v_b=f_b[(2/3)F_b-2R_b]\) on these bonds and zero elsewhere. The normalized Wilson divergence \(\delta_\mu v=\beta\nabla S\cdot v-\operatorname{div}v\) has squared norm at most \(C\sum_b|f_b|^2\). The compact group score identity of §4.111 bounds its second moment by the expected squared covariant derivatives of \(v\) plus the Ricci and Wilson-Hessian form on \(v\). Each \(v_b/f_b\) is a fixed-stencil sum of compact forces, with \(\beta\mathbb E|v_b|^2\le C|f_b|^2\) by the original plaquette moments. Its derivative is bounded on that fixed stencil and vanishes off it; the product metric connection adds a bounded multiple of \(\|v\|\). The physical action Hessian has bounded operator norm by finite incidence. These estimates cover real and imaginary parts. In the ordinary divergence only the same link derivative enters: its color trace is the original plaquette Casimir, restricted to the selected directional actions. The result is an identity constant and a linear plaquette mark with squared coefficient norm at most \(C\sum_b|f_b|^2\). Its centered variance obeys (ADDITIVE-PLAQUETTE-SUS). This proves the claimed cost even though the partial directional force alone is not the total conditional score.

The replacement \(q_{i,b}\) lies entirely on *one* \(i\)-slice, since its only plaquettes are in the \(0j,0k\) planes. It is a gauge-invariant multiplication insertion on the spatial \(i\)-transfer slice and is even under reflection in that slice. For a fixed transverse Fourier mark, every separated-slice connected covariance in its longitudinal Fourier transform is nonnegative. Indeed the positive transfer trace has nonnegative spectral terms \(\lambda_\alpha^{n-l}\lambda_\gamma^l |\langle\gamma,O\alpha\rangle|^2\) at separation \(l\), using the transverse adjoint mark. For transverse momentum zero, center the insertion in this trace; for other momenta its mean vanishes by translation invariance. The \(l=0\) term is independent of the longitudinal momentum. Consequently \(S_{q_i}(p)\le S_{q_i}(p|_{p_i=0})\). Apply (DIRECTIONAL-WARD-COST), the triangle inequality in centered \(L^2\), and the same cost at the new momentum. This gives \(\sqrt{S_h(p)}\le 2C_N+\sqrt{S_h(p|_{p_i=0})}\). Repeating the argument for each of the three spatial axes removes their momenta one at a time without requiring all the replacements to be the same local function.

In the temporal axis \(h_b\) occupies a *single* slab and its reflection in the slab midpoint preserves it: reversal of the temporal bond rotates and reverses all three forces together. With zero spatial momentum the centered slab insertion is self-adjoint. At separations \(1\le l\le n-1\) the positive trace uses powers \(n-l-1,l-1\) and squared matrix elements, exactly as for the temporal plaquette slab in §4.113. More explicitly center by replacing the insertion kernel \(O\) by \(O-(\mathbb E h_{\rm slice})T\); the sum of the two-insertion traces at distinct slabs is then precisely the connected covariance. The coincident-slab contact is independent of temporal momentum. Thus \(S_h(p_0,0,0,0)\le S_h(0)\). Parseval, the established finite-incidence \(r,h\) covariance contact, lattice rotations and Cauchy–Schwarz over the four link orientations give the all-mark assertion. In particular the original eight-site temporal mask, including all seven spatial aliases and its constant component, obeys it.

Under the additional smooth *finite family of concrete loop and tensor-product action realizations* in §4.117, the resulting full-law bound at this stage is quantitatively
\[
 \operatorname{Var}_\mu(r_f)\le
 C\,[1+\beta S_\beta^{-3}]\sum_b|f_b|^2,\qquad
 S_\beta\asymp\beta^{1/35}(\log\beta)^{-6/35}.
 \tag{SUBLINEAR-COMB-SUS}
\]
Use the tori and comparable boxes of §§4.84–4.85, in particular \(4\mid n\). Let \(Y_0=\sum_{b\parallel0}h_b\), a sum of the eight translated black combs \(Y_v\) in the original Wilson law. Hölder and translation invariance give for real \(s\)
\[
 \log\mathbb E e^{s(Y_0-\mathbb E Y_0)}
 \le \log\mathbb E e^{8s(Y_{\rm black}-\mathbb E Y_{\rm black})}.
\]
The existing centered real comb slope estimate (DEEP-TILTED-COMB-SLOPE) and the bounded second derivative of its limiting Gaussian pressure give an upper bound \(CV(s^2+|s|S_\beta^{-3})\) on the right for \(|8s|\) in its fixed real interval. The exact smooth additive finite-family clause of §4.117 yields a fixed-radius zero-free disc for \(Y_0/\beta\), since its one- and two-plaquette trace contractions are a fixed linear combination of those additive action realizations. This gives a disc of radius \(c/\beta\) for \(Y_0\); it does not give a fixed disc for the unamplified observable. The centered analytic log on a circle of half this radius has real part bounded by the same estimate with \(s=\Re z\), by positivity of the real Wilson law. The one-sided analytic Cauchy estimate gives \(S_h(0)\le C(1+\beta S_\beta^{-3})\), proving the bound. If only the six fundamental additive plaquette sources are admitted, the exact fine-uniform reduction remains valid and this quantitative finite-family conclusion is conditional on the specified additional realizations.

The same calculation shows that it suffices for full susceptibility to have a zero-free disc of radius \(c S_\beta^{-3}\) for the **fine-uniform unamplified** \(Y_0\). This radius tends to zero, and is larger than the admitted additive-loop radius after rescaling by \(\beta\). The estimate proved here grows at most as \(\beta^{32/35}(\log\beta)^{18/35}\); a uniform bound for the remaining fine-uniform scalar has not been obtained. This distinction keeps the physical \(a^{-2}\) multiplier and the independently refuted fixed physical source polydisc out of the zero-mode argument.

### 4.126 Exact quotient and the endpoint mismatch in the true magnetic spectator (P)

At each time the retained spatial edges in (SPATIAL-STAR-EXTERIOR) have exactly one endpoint \(z\) with two odd spatial coordinates. Four spokes out of \(z\) end at sites with one odd coordinate (middle edges), and two end at all-odd sites. Write \(U_{z,y}=h_z w_{z,y}\) on the four middle edges by choosing any one of them as \(h_z\) and setting its \(w\) to identity. Then the complete measurable source \(M_{\rm sp}\) depends only on the three remaining \(w\)'s at every \(z,t\). Indeed each middle magnetic path of an all-even star goes from a one-odd site to another via just one \(z\). Its product is \(w_{z,y}^{-1}w_{z,y'}\), with the irrelevant interior frame canceled. The other spectator magnetic and kinetic terms cancel when computing the normalized conditional mean of the black star. The two spokes to all-odd sites do not enter such a path.

In particular \(9n^3/8\) group coordinates per slice suffice for this entire source instead of the \(9n^3/4\) original spectator coordinates. In \(L^2(\nu)\) its inner product with *every* function conditionally centered on these \(w\)'s is zero. This eliminates the entire conditional orthogonal complement, including products and gauge singlets on macroscopic time intervals. The spectral projectors of \(L\) need not preserve that complement; an individual eigenfunction can have a nonzero conditional mean.

The true density on the quotient has an explicit positive expression. Every spatial plaquette contains precisely one all-even or one all-odd corner, never both. At fixed middle edges the entire time trajectories of the six-spoke stars at *both* types of corners are conditionally independent. Denote their positive full temporal/magnetic integrals by \(Z_x(U)\). Up to normalization the density on \(w\) relative to product Haar is
\[
 \bar w(w)=\prod_{x\ {\rm all\ even}} Z_x(w)
       \int\!\prod_{t,z}dh_{t,z}\;
       e^{-\beta S_{\rm kin}^{\rm mid}(hw)}
       \prod_{x\ {\rm all\ odd}}Z_x(hw).
 \tag{MAGNETIC-QUOTIENT-LAW}
\]
Interchanging the two types of corners also exhibits why the opposite-star factor can still depend on the frames: the interior point of its middle paths is one-odd rather than two-odd. Product Haar in the new coordinates follows separately at each \(z,t\). For a smooth scalar \(f(w)\), the exact compressed Dirichlet form of the original spectator generator is
\[
 g^2\mathbb E_{\bar\nu}\sum_{z,t,A}
  \left[\sum_{i=2}^4|X_i^A f|^2+
                \left|\sum_{i=2}^4X_i^A f\right|^2\right].
\]
Here \(X_i^A\) differentiates the \(i\)-th relative spoke by left multiplication. Varying one nonreference middle edge produces its own derivative rotated by the common frame; varying the reference edge produces the simultaneous negative sum with that rotation. Summation over the orthonormal Lie generators removes the common rotation. The two unused edges have zero derivative. Thus the elliptic coefficient on the relative indices is \(I+\mathbf1\mathbf1^T\), uniformly between one and four, on the exact quotient density. Centered variance of the source is identical on the two spaces. The two generators' individual spectral measures have not been equated.

The mismatch in (SPATIAL-GAUGE-WARD-SPLIT) is present under actual thermal averaging. For a unit color generator \(T_A\) in the shared one-odd endpoint frame and \(m\) in §4.124,
\[
 \mathbb E\,\operatorname{Var}\big((q_e-q_{e'})^A\mid E\big)\ge c_N>0
 \quad\hbox{for sufficiently large }\beta .
 \tag{THERMAL-ENDPOINT-MISMATCH}
\]
Work with the right derivative on the integrated spoke \(\sigma_{t,e}\) along \(iT_A\), and pair with the right canonical total axial force \(H=g\,\partial^R(\beta S_{\rm ax})\) in that coordinate. Integration by parts gives \(\mathbb E(H\mid E)=0\) and \(\mathbb E H^2=g^2\mathbb E\,(\partial^R)^2(\beta S_{\rm ax})\le C_N\) by bounded plaquette degree. In differentiating the \(A\) component of \(-\operatorname{Ad}(\sigma_{t,e}^{-1})v_{t,e}\), the derivative of the outer rotation drops out: a rotation about \(T_A\) preserves its \(A\) component exactly. All past terms except the same-edge \(J_{t-1,e}\) are independent of this group coordinate, including the term on the other spoke \(e'\). The canonical derivative of that last current in the same rotated direction is the Wilson second directional derivative of \(s(u_{t-1,e})\). At identity it equals \(\operatorname{Tr}(T_A^2)\); its difference is bounded by \(C\|u_{t-1,e}-I\|\), also after any current frame rotation. The true axial plaquette moments bound this difference in mean by \(C/\sqrt\beta\). Hence
\[
 \mathbb E[H(q_e-q_{e'})^A]
     =-K_{ee}^{\rm dir}\operatorname{Tr}(T_A^2)+O(\beta^{-1/2}).
\]
Cauchy–Schwarz after subtracting the conditional mean proves (THERMAL-ENDPOINT-MISMATCH). This is a lower bound on directional *interior noise*, not a lower bound on slow spectator variance.

One also has an exact time derivative for the between-star magnetic mean in that split. Put \(P_{t,e}=-\operatorname{Ad}(\sigma_{t,e}^{-1})J_{t,e}\) in the one-odd endpoint frame. The right total physical gradient has zero conditional mean at every integrated spoke. Since \(J_{t-1,e}\) commutes with \(u_{t-1,e}\), its endpoint transport is identical using \(\sigma_{t,e}\) or \(\sigma_{t-1,e}\). The decomposition of the full gradient into its temporal and magnetic parts gives \(\overline{\tilde B}_{t,e}=\bar P_{t,e}-\bar P_{t-1,e}\). Thus the exact product-of-means term of §4.124 contains a time difference of the conditional electric current. The signed sum with its endpoint velocity still needs an extensive variance estimate.

### 4.127 Deep-root compact Ward comparison on larger balanced boxes (P)

For the actual positive comb tilt of §§4.82–4.85 one can improve the real slope estimate to
\[
 \sup_{|t|\le t_1}|(p_a^{Y^h})'(t)-(p_G^{Y^h})'(t)|
 \le C s_*^{-3},\quad
 s_*=\left\lfloor c\,\beta^{1/10}(\log\beta)^{-3/5}\right\rfloor .
 \tag{BALANCED-BOX-SLOPE}
\]
Use \(4\mid n\), reduce the fixed \(t_1\) if necessary, and round comparable box sides to compatible even sizes. The resulting bound in (SUBLINEAR-COMB-SUS) improves to \(C[1+\beta^{7/10}(\log\beta)^{9/5}]\sum|f_b|^2\) under the same concrete smooth source clauses. A disc of radius \(c s_*^{-3}\) for the fine-uniform unamplified observable suffices. The proof estimates a single normalized Ward test against the real compact measure. It avoids an estimate of the total variation distance between the box density and a multidimensional Gaussian.

**Coordinates and their sections.** Put \(P=\log\beta\) and take a box of side comparable to \(s\) centered on the chosen deep marked root, with its spatial faces on the admissible odd planes. The complement of the event that all box plaquette defects obey \(\sqrt\beta\|U_p-I\|\le P\) has probability at most \(Cs^4 e^{-cP^2}\) in the true comb tilt by §4.82. For this argument \(g=\beta^{-1/2}\), with the fixed generator metric in the linear form. Tree fix the vertical bonds first up to the top, so the last vertical bond carries the whole column holonomy \(H_x\). Based gauge transformations can then distribute this holonomy as \(\exp(\log H_x/s_0)\) on every vertical bond of its column, \(s_0\asymp s\) the actual temporal length. This last transformation is identity at the bottom and at the top. Prescribed side columns can be balanced by the same operation on the boundary gauge representative. In these coordinates write every spatial link as \(\exp(gB_i)\) and every repeated interior vertical link as \(\exp(gB_0(x))\). Integration over the based gauges has unit constant; in each free column the Haar volume is \(dH_x\), giving the exponential-chart Jacobian \(j(s_0gB_0)\); each free spatial edge has \(j(gB_i)\). The powers of \(s_0g,g\) are independent of the integrated configuration. This follows directly by consecutive Haar changes along each column followed by the prescribed gauge translations of its spatial bonds. Only the near-identity branch will enter the Ward test.

The following details of the boundary section matter. On every good full configuration the coordinate-tree boundary representative in §§4.73,4.84 has link logarithms bounded by \(Cs gP\), and each of its normalized boundary links has \(L^2\) norm \(C\sqrt s\) by (TILTED-THIN-TREE). In that representative the adjacent column holonomies differ in norm by \(Cs gP\): the width-one full-time curtain gives their difference up to the two bottom/top spatial endpoint links. A side column holonomy is within \(Cs^2gP\) of identity by multiplying its prescribed vertical links. Propagating the neighboring estimate from a side gives the same bound for every interior \(H_x\). The Lipschitz constant of the principal logarithm and of its fractional powers is bounded on this neighborhood provided \(s^2gP\) is sufficiently small. In the bottom-based gauge each spatial link is the bottom link up to a width-one partial curtain. On balancing, only the difference of the fractional powers at adjacent columns adds to its norm, in addition to a unitary conjugation. All balanced links therefore have logarithms \(O(sgP)\). The same argument on this *competitor* gives \(L^2\) norm \(C\sqrt s\) for its normalized boundary links on the good event: the partial- and full-curtain defects have normalized \(L^2\) norm \(C\sqrt s\) by the tilted rectangle estimate of §4.84, including the two endpoint link terms. For a side vertical balance use \(\|\log H_x\|/s_0\) and the sum of the original prescribed link norms. Increasing the fixed bound \(C\) absorbs the finite choices of direction and corner.

For a legitimate conditional integration choose a measurable section using only the boundary data. Among its gauge representatives satisfying the balanced side condition, the fixed small-column branch there, and \(\max_{\partial B}|D_e|\le CsP\) in normalized coordinates, minimize \(|\Lambda_x E_t D|^2\). Here \(E_tD\) is the *linear* Gaussian minimizing extension for the tilted quadratic and \(\Lambda_x\) is its local matching projection, so that the root quadratic is \(|\Lambda_x B|^2\). The admissible set is compact inside the logarithmic chart and a measurable minimizer exists (one may use a fixed measurable near-minimizer with extra cost \(s^{-4}\)). If there is no representative, set the test to zero. The competitor above is available on every full good configuration. Its deep harmonic bound \(\|\Lambda_x E_tD\|_{L^2(\mathrm{good})}\le Cs^{-3/2}\) follows exactly as in §4.84: the deep boundary-link coefficient sum is \(O(s^{-2})\) and the finite-tilt matching resolvent is absolutely summable; near other faces use their boundary curvatures. On the good event their normalized square moments are bounded, since \(d_\partial D\) differs from the true normalized boundary curvature in its own frame by \(O(gs^2P^2)\). The choice by minimization inherits this expected squared bound *on the full good event*. On the admissible but bad complement the deterministic field \(\Lambda_x E_tD\) has at most polynomial size in \(s,P\), by a zero-interior trial and the bounded matching operator in the energy norm. Thus the bad-event contribution is superpolynomially small. Conversely for any chosen admissible section every full configuration with good plaquettes has all its balanced interior links bounded by \(Cs gP\): use the small side column, the same adjacent full curtains with the small prescribed bottom/top links, and the partial curtains just proved. In normalized coordinates \(\|dB\|_\infty\le CP\) there by the plaquette BCH bound \(O(gs^2P^2)\). This is the place where \(s^2gP\ll1\) is used. The boundary representative is allowed to differ between estimates of different roots; no source derivative of this section is taken.

**The linear box inverse.** For zero-boundary variations \(v\) the balanced vertical component \(v_0(x)\) is constant in time and vanishes on the spatial side. Summing \((dv)_{0i}\) over time gives \(-s_0\nabla_i v_0\) by the zero bottom and top spatial variations. The spatial Dirichlet sum and integration of \(v_i\) from the bottom give
\[
 \sum_{\rm physical\ links}|v_e|\le Cs\sum_p|(dv)_p|,\qquad
 \|v\|_2\le Cs\|dv\|_2 .
 \tag{BALANCED-POTENTIAL-BOUND}
\]
The repeated vertical value is counted \(s_0\) times on the left. For example \(s_0\sum_x|\nabla_i v_0|\le\sum_{t,x}|(dv)_{0i}|\), then \(\sum_x|v_0|\le Cs\sum_x|\nabla v_0|\). The \(L^2\) proof uses Cauchy–Schwarz in the same sums. These variations parametrize the full relative curvature space: any zero-boundary one-form can be balanced by a scalar vanishing on the boundary, distributing its column sum uniformly. Thus its Gaussian curvature covariance and minimizing extension agree with those in §4.84 before gauge fixing.

Let \(H_t\) be the positive Hessian of the tilted Gaussian on these independent coordinates and use the ordinary Euclidean pairing there. Uniformly on the boxes,
\[
 \|dH_t^{-1}\Lambda_x^* b\|_1\le C|b|
 \tag{BALANCED-SOURCE-INVERSE}
\]
for any root color/matching vector \(b\). At zero tilt the operator on the doubled periodic cube is the two-form projection onto curls applied to one finite difference at the prescribed root, with the fixed finite component matrices. Its symbol has derivative of order \(k\) bounded by \(C_k |p|^{1-k}\) near zero: the curl projection is \(dd^*/\sum_\mu|\widehat D_\mu|^2\), and the incident matching force supplies one additional difference. The zero value is zero. A smooth dyadic frequency partition bounds the kernel of a shell of radius \(u\) by \(C_M u^5(1+u|y|)^{-M}\) by repeated integration by parts. Summation in \(u\) gives \(C(1+|y|)^{-5}\). Absolute summability allows exact periodization on the sampled torus. Relative face reflection as in §4.84 adds at most \(2^4\) reflected images; alternatively restrict the periodic curvature projection to its reflection subspace. With the tilt, apply the untilted inverse to the sources multiplied by the matching resolvent \((I-2t G_D M)^{-1}\) of §4.84, with its fixed metric factors. On a sufficiently small fixed real interval its \(\ell^1\) column bound follows also by the Neumann series from the summable untilted matching kernel. This proves (BALANCED-SOURCE-INVERSE).

**Actual compact Ward test.** In the chart write \(B=E_tD+x'\) and \(Q_x(B)=|\Lambda_x B|^2\). Use a smooth cutoff \(\chi(B)\) which equals one on the good bounds just proved and is supported on their double: \(\|B\|_\infty\le C sP\), \(\|dB\|_\infty\le C P\), with enlarged fixed constants. A product of smooth coordinate and plaquette-coordinate bumps suffices. All its derivatives have polynomial bounds in \(s,\beta\); every nonzero first derivative occurs only when at least one genuine box plaquette fails the good test. The chart cutoff extends by zero on the compact integral. In particular the column log never reaches its cut since \(s^2gP\ll1\). Test the compact logarithmic density with the vector
\[
 v=H_t^{-1}\Lambda_x^* b,\qquad
 b=\Lambda_x x'+2\Lambda_x E_tD=\Lambda_x B+\Lambda_x E_tD .
\]
At fixed chosen boundary its ordinary coordinate divergence is \(\operatorname{Tr}(\Lambda_x H_t^{-1}\Lambda_x^*)\), while \(\langle H_t x',v\rangle=Q_x(B)-Q_x(E_tD)\). All terms can be tested as \(\chi v\) before integration; there is no division by a possibly tiny good-box probability.

For clarity let \(U(B)\) denote the actual negative log density in this chart, with the compact Haar Jacobians and the real comb tilt, and \(U_2(B)\) its tilted quadratic part. On the cutoff support its first derivative in a zero-boundary variation \(v\) satisfies
\[
 |D(U-U_2)[v]|
 \le C g s^2P^2\|dv\|_1+C g sP^2\|v\|_{1,\rm links}
      +C g^2s^3P\sum_x |v_0(x)| .
\]
Indeed the normalized compact plaquette current equals its linear curl plus \(O(gs^2P^2)\), by expanding the four factors with \(|B|\le CsP\), and its derivative equals \(dv\) plus \(O(gsP)\) times the sum of the four incident link variations. The same estimates for the projected Lie current give the derivative of each quadratic frustration term, with only bounded repetition of any plaquette. They also give \(|h_x-Q_x(B)|\le C gs^2P^3\) on this support. For the unperturbed action one may differentiate the real trace directly: its Lie current differs from the linear plaquette curl by the same \(O(gs^2P^2)\), with the fixed linear normalization included in \(U_2\). Spatial Haar derivatives are \(O(g^2sP)|v_e|\). The last displayed term is the column Haar contribution from \(j(s_0gB_0)\). Combining the two inverse estimates bounds this error by \(C g s^2P^2 |b|\) on the test. Under the true tilted integral with \(\chi\) inserted, \(\mathbb E[\chi |b|]\le CP+Cs^{-3/2}+o(1)\) by the minimizing section estimate. The discarded \((1-\chi)\) root and all differentiated cutoff terms are bounded by a polynomial times the actual bad-box probability; the uncut compact \(h_x\) itself is bounded by \(C\beta\). Constants do not depend on the number of boxes or on their exterior data. This argument takes expectations with the *actual* normalized boundary marginal.

Compact integration by parts for \(\chi v\) now gives
\[
 \left|\mathbb E_t h_x-
       \operatorname{Tr}(\Lambda_x H_t^{-1}\Lambda_x^*)\right|
 \le C\big(s^{-3}+gs^2P^3\big)
           +\mathrm{poly}(\beta,s)e^{-cP^2}.
\]
Here \(Q_x(E_tD)\) contributes \(O(s^{-3})\); the trace itself is uniformly bounded by the matching energy inequality. The deep relative Gaussian trace differs from the infinite tilted trace by \(O(s^{-6})\) by the reflected resolvent of §4.84. Summing the single-root estimate and normalizing by \(V\), with the original fraction of marked sites, proves (BALANCED-BOX-SLOPE) by setting \(s\asymp s_*\), since \(g s^5P^3=O(1)\). The same centered Hölder and one-sided Cauchy proof as in §4.125 then gives the claimed all-mark improvement. The genuine small-frequency excess of the fine-uniform source can still exceed this width estimate; uniform boundedness has not been concluded.

### 4.128 Paying compact source footprints through the early mesoscopic scale (P with the stated native occupied-volume import)

Here a real source estimate is taken in the *unmarked* positive joint law of fields and histories. No reflection positivity of history selectors is needed. Partition into comparable \(J\)-tiles of side \(\ell=L^J\) with \(\ell^4\gg\log\beta\), or use bounded-overlap enlarged tiles. Let \(W\) be any random collection of these tiles and put \(E_c=\sum_{p\ {\rm incident\ to}\ c}s_p\) using a fixed bounded enlargement. The unmarked fine Wilson marginal obeys, for every fixed \(\kappa>0\),
\[
 \log\mathbb E\exp\!\left[\kappa\sum_{c\in W} E_c\right]
 \le \tfrac12\log\mathbb E\exp[C_\kappa(\ell^4/\beta)|W|]
            +C_\kappa (V/\ell^4)e^{-c\ell^4}.
 \tag{ADAPTIVE-FOOTPRINT-ENERGY}
\]
For any deterministic family \(A\) of tiles, (MARKED-EXP) gives \(\mathbb E e^{\delta\beta\sum_{c\in A}E_c}\le e^{C\ell^4|A|}\) for fixed small \(\delta\), including the bounded overlap. Set \(K=K_0\ell^4/\beta\) with a sufficiently large fixed \(K_0\). Expand the product generating function of \(\sum_c(E_c-K)_+\). Whenever all terms in a nonempty subset \(A\) are nonzero, \(\sum_{c\in A}E_c>K|A|\). The expectation of their product \( \prod_{c\in A}(e^{2\kappa(E_c-K)_+}-1)\) is at most \(e^{-\delta\beta K|A|/2}\mathbb E e^{(\delta\beta/2+2\kappa)\sum_{c\in A}E_c}\le e^{-c\ell^4|A|}\). Sum over subsets, use \(\sum_{c\in W}E_c\le K|W|+\sum_c(E_c-K)_+\), and apply Cauchy–Schwarz. This proves the estimate even when \(W\) depends on the entire configuration and its history. A bare \(\beta^{-1}|h_b|\) costs at most \(C\sum_{p\ni b}s_p\), so the estimate includes all microscopic descendants in these tiles.

For illustration, if a tile must contain a true fine plaquette with \(\sqrt\beta\|U_p-I\|>\log\beta\), joint MarkedExp and summed witness choices give a bound \((C\ell^4 e^{-c(\log\beta)^2})^{|A|/C}\) on simultaneous failures in prescribed tiles; use a bounded coloring for overlap. Thus their centered additive source costs \(o(V/\beta^2)\) in the real log moment at either sign, for any polynomial \(\ell\) with \(\ell^4=O(\beta)\). The full native coarse selectors are a different class of events.

For the latter use the positive unmarked history and empirical volume \(V_{\le J}\) of genuine occupied native cubes through scale \(J\), counted once at each actual scale, of T1 (7.226). Its early-volume version on the same native exponential and terminal margins is
\[
 \mathbb E e^{s_0 V_{\le J}}\le
 \bar B_{\rm stop}\exp\!\left[
 C M_{\rm early}e^{-a p_J^2}\sum_{\ell'=1}^K e^{-p_{\ell'}}\right],
 \tag{EARLY-RELEASE-VOLUME}
\]
for fixed \(s_0\), where \(M_{\rm early}=O(V)\) counts the possible early native homes and \(p_j\) is the original decreasing squared-birth threshold notation of T1. To get this refinement from the affine-tag proof of (7.226), use on a simultaneous release at \(\ell'\) the factor \(1+u(e^{s_0 V_X^{\rm early}}-1)\) on each released body \(X\). A nonconstant factor entails a continuing genuine occupied home at some scale \(\le J\), so that release has an ordinary birth at \(h\le J\). Different released bodies have disjoint unbroken ancestral components at this release. Use one spare fraction of the original *squared birth reserve* for each nonconstant factor, preserving the original linear release reserve from (1.95). The two native exclusion estimates of (7.226) therefore hold on the larger disc \(|u|\le c e^{p_{\ell'}+a p_J^2}\). Its polynomial degree is at most \(M_{\rm early}\), since each disjoint release carrying a tag must have an earlier realized home. The same polynomial zero-radius argument and sequential conditional integrations as in (7.226) bound the normalized log at \(u=1\) by \(C M_{\rm early}e^{-a p_J^2-p_{\ell'}}\) at that release. Terminal survivors retain the original fixed terminal ratio on the enlarged stability margin. A birth used at a release is not reused by a later disjoint release. This proves the displayed refinement under the hypotheses of that native estimate. The proof charges a single squared factor per released body even if it touches many earlier tiles. It does not assign independent failures to their roots.

Suppose \(W\) consists of \(J\)-tiles touched by such an occupied cube at a scale \(\le J\), with an optional collar of \(b\ge1\) in \(J\)-units. Then \(|W|\le C b^4 V_{\le J}\) by geometry alone. If \(b^4\ell^4/\beta\le C\) on the fixed native margin, (ADAPTIVE-FOOTPRINT-ENERGY) and (EARLY-RELEASE-VOLUME) give \(o(V/\beta^2)\) for the log moment of the positive bare additive source on this entire random footprint, up to the fixed terminal log ratio. Here \(p_J\) is at least a fixed multiple of a positive power of \(\log\beta\) whose square dominates \(\log\beta\) on the early weak trajectory; \(K=O(\beta)\), and \(V/\beta^2\to\infty\). The same conclusion for a centered source follows by Jensen and the positive majorant. In particular \(b=C\log\beta\) is allowed at \(\ell\asymp\beta^\gamma\), \(0<\gamma<1/4\). This pays even arbitrary mergers in a genuine bad footprint at the real pressure scale of interest. Pure fine plaquette defects and the genuine native occupied-volume import exhaust only their stated fields; a claimed additional selector must be shown to belong to one of them before using this estimate.

What remains is a concrete clean-core bound. For the complement of these footprints one needs the log moment, centered in the actual unmarked law, of the additive uniform or real comb source bounded by \(CV/\beta^2\), on the source interval of fixed additive strength in §4.125. Hölder would then reinstate the paid footprints. A scalar retained bound of size \(O(L^{-sJ}+\beta^{-1})\) times polylogarithms per clean current site would suffice after the microscopic vacuum term and all centered clean innovations are accounted for, by taking \(1/(4+s)<\gamma<1/4\). The stated homogeneous estimates concern their admitted unpunctured domains. Applying them on a punctured clean core with its actual exterior pins and the proper replacement differences remains open. An unmarked estimate on occupied volumes alone does not give that scalar comparison.

### 4.129 The signed cubic correction in the balanced Ward test (P)

One additional integration by parts improves the true fine-uniform reduction quantitatively:
\[
 \begin{split}
 s_{**}&=\left\lfloor c\,\beta^{1/7}(\log\beta)^{-8}\right\rfloor,\\
 \sup_{|t|\le t_1}|(p_a^{Y^h})'(t)-(p_G^{Y^h})'(t)|&\le C s_{**}^{-3},\\
 \operatorname{Var}_\mu(r_f)&\le
 C[1+\beta^{4/7}(\log\beta)^{24}]\sum_b|f_b|^2 .
 \end{split}
 \tag{CUBIC-CORRECTED-SUS}
\]
The pressure and variance use the tori and the same respective hypotheses as §§4.127 and 4.125. The last bound grows with \(\beta\). Its improvement uses the vanishing of a specific color contraction in the actual comparison, not an equality of the compact and Gaussian laws.

Work on the balanced chart with the same root \(x\), cutoff \(\chi\), boundary section, and \(m=E_tD\). Denote the homogeneous cubic terms of the Taylor expansions by \(A_3(B)\) for the real tilted action and \(C_{3,x}(B)\) for the root observable, so their coefficients in the canonical chart are \(gA_3\) and \(g C_{3,x}\). They are finite-stencil cubic polynomials in the physical bond variables, including the fixed boundary values. The action cubic at each plaquette consists of a curl times a quadratic polynomial in the bonds. The quadratic-frustration tilt adds finite sums of the same form at incident plaquettes. The root cubic is a matching linear force times a quadratic in the same fixed neighborhood. Every color tensor is proportional to the antisymmetric Lie bracket tensor in an orthonormal invariant metric. Indeed the second term of the Lie part of a product of group exponentials is the BCH commutator. The real trace action has zero cubic contribution from the trace of the cube of a single skew-Hermitian plaquette logarithm. Transporting a generator past one group factor produces another commutator at this order. The compact Haar log in exponential coordinates starts at even order.

On the cutoff the Taylor remainder in the observable is bounded by \(C g^2s^4P^4\). The action derivative after removing \(U_2+gA_3\) obeys
\[
 |D(U-U_2-gA_3)[v]|
 \le C g^2\big[s^4P^3\|dv\|_1+s^3P^3\|v\|_{1,\rm links}
                         +s^3P\textstyle\sum_x |v_0(x)|\big].
\]
To verify the powers, the second-order normalized plaquette current after the quadratic term has size \(O(g^2(sP)^3)\). Products of two quadratic currents in the action give a derivative of size \(O(g^2(sP)^3)\) on a single undifferenced bond variation. Differentiating the remaining products with respect to a curl costs at most \(O(g^2s^4P^3)\); all higher group-word terms are geometrically smaller on \(g sP\ll1\) with \(|dB|\le CP\). The bounded multiplicity of plaquettes/matching rows gives the two sums. The last term covers the column Jacobian. Thus the first Ward test of §4.127 has the same deterministic trace and noncentral term, plus \(g\,\mathbb E[\chi\,T_3(B)]\), with residual \(O(g^2s^4P^6)\) and a superpolynomial tail. Here
\[
 T_3(B)=C_{3,x}(B)-DA_3(B)[V(B)],\qquad
 V(B)=H_t^{-1}\Lambda_x^*(\Lambda_x B+\Lambda_x m).
\]
It is polynomial of degree at most three at fixed boundary. In particular it is legitimate to test its centered Gaussian part by a second Ward identity.

Here are the needed uniform box estimates for that identity. On the cutoff \(\|dm\|_\infty\le C P(1+\log s)\) and \(\|m\|_\infty\le C s P(1+\log s)\). For the untilted extension, reflect its curvature as in §4.70: its divergence vanishes and its exterior differential consists of fixed boundary curvature sources in the one-layer collar. The inverse gradient kernel on the doubled periodic lattice is bounded by \(C[(1+d)^{-3}+s^{-3}]\), by the dyadic proof of §4.72 now at order minus one. Its sum on any three-dimensional face is \(O(1+\log s)\). The possible constant curvature is at most \(CP\) by the energy of the cutoff trial configuration and minimality. Each linear boundary curvature is \(O(P)\) on this cutoff. This proves the untilted curvature bound. The small real tilt adds \(dH_0^{-1}\Lambda^*\) applied to the bounded matching resolvent of the untilted matched mean. The finite-volume kernels have uniformly bounded absolute row sums by the proof of (BALANCED-SOURCE-INVERSE), which gives the tilted bound. Reconstruct \(m_0\) from its time-averaged spatial gradients and side values; the top-minus-bottom spatial boundary differences in that reconstruction have size at most \(CsP\). Then reconstruct \(m_i\) from its bottom value. This proves the stated potential bound.

For the Gaussian with mean \(m\) and covariance \(H_t^{-1}\), curvature-coordinate variances are uniformly bounded by the energy comparison; individual balanced bond variances are \(O(s^2)\) by the following reconstruction. Each zero-boundary balanced coordinate is a linear combination of curls with coefficient absolute sum \(Cs\): use a fixed side path and the time average to reconstruct \(v_0\), then its spatial gradient and the bottom-to-\(t\) sum for \(v_i\). Gaussian maxima over \(O(s^4)\) coordinates cost at most \(C_k(1+\log s)^{1/2}\) in any fixed \(L^k\) norm by the elementary Gaussian tail and a union bound. Also \(dH_t^{-1}d^*\) has \(\ell^1\) operator norm at most \(C(1+\log s)\). The untilted curl projection kernel is order zero and bounded on the finite doubled lattice by \(C[(1+d)^{-4}+s^{-4}]\) as in §4.72; the small-tilt correction has the summable \(dH_0^{-1}\Lambda^*\) kernel on both sides and the summable matching resolvent between them. Consequently, for any linear functional \(DV[v]=\langle a,dv\rangle+\langle b,v\rangle\), the curl of its \(H_t^{-1}\) representative has \(\ell^1\) norm at most \(C(1+\log s)(\|a\|_1+s\|b\|_1)\). The last bound holds for the independent coordinates by applying the reconstruction to each \(b\)-slot separately.

Let \(Z\) be a centered free Gaussian with covariance \(H_t^{-1}\) and put \(B_u=m+e^{-u}(B-m)+(1-e^{-2u})^{1/2}Z\), preserving the fixed boundary. In the independent box coordinates take
\[
 V_3(B)=H_t^{-1}\int_0^\infty e^{-u}\mathbb E_Z[\nabla T_3(B_u)]\,du .
\]
Differentiating the Gaussian averaging formula in \(u\), or checking on monomials up to degree three, gives
\(\langle H_t(B-m),V_3\rangle-\operatorname{div}V_3
=T_3(B)-\mathbb E_Z T_3(m+Z)\).
Throughout the cutoff, \(\|dV_3\|_1\le C s^2P^9\) and \(\|V_3\|_{1,\rm links}\le Cs^3P^9\). For details, at \(B_u\) the maximum curvature has bounded fixed moments \(CP^3\), the maximum bond has bounds \(CsP^3\), and \(\|dV(B_u)\|_1,\ s^{-1}\|V(B_u)\|_1\) have bounds \(CP^3\) by (BALANCED-SOURCE-INVERSE). Differentiating the cubic action directionally produces terms bounded by the pairings \((B_u)^2 dV(B_u)\) and \(B_u dB_u V(B_u)\) in absolute coefficient norm. A second derivative in a test direction costs at most \(Cs^2P^6\) in the curl coefficient and \(CsP^6\) in the undifferenced coefficient. The derivative falling on \(V(B_u)\) instead gives a root matching adjoint with coefficient \(Cs^2P^6\); its fixed-stencil curl coefficient has the same bound. The root cubic satisfies these same estimates directly. These bounds for products follow by Cauchy–Schwarz at the indicated fixed moment orders, so they hold inside the Gaussian integral. Apply the preceding inverse estimate and \(1+\log s\le C P\), then the balanced potential inequality. The stated powers leave spare logarithms.

Apply the compact integration by parts to \(\chi V_3\). The nonlinear first derivative estimate of §4.127 and these last bounds give
\[
 \left|\mathbb E\,\chi[T_3(B)-\mathbb E_Z T_3(m+Z)]\right|
 \le C g s^4P^{12}+\mathrm{poly}(\beta,s)e^{-cP^2}.
\]
All expectations here use the true comb tilt and its actual boundary disintegration, exactly as for the first test. Derivatives of the cutoff only occur on the genuine bad event. Polynomial bounds on the compactly supported tests and the finite Gaussian moments suffice for those tails.

In the Gaussian mean of \(T_3\), every contraction of two fluctuating color slots is a scalar multiple of \(\delta_{AB}\), even with the tilted matching resolvent, which is color diagonal. The remaining cubic tensor is antisymmetric in those slots, so all such contractions vanish. Terms with three centered fluctuations vanish by Gaussian parity. Thus \(\mathbb E_ZT_3(m+Z)=T_3(m)\), including the terms of degree two multiplied by the *fixed* root vector \(\Lambda_xm\). The root cubic at \(m\) and \(DA_3(m)[V(m)]\) both contain a factor \(\Lambda_xm\). The field and inverse bounds give \(|T_3(m)|\le C s^2P^7|\Lambda_xm|\). The same boundary section estimate as §4.127 then bounds its true cutoff expectation by \(C s^2P^7s^{-3/2}\) plus the bad-event tail. In total the local slope error is bounded by
\[
 C[s^{-3}+g s^{1/2}P^7+g^2s^4P^{14}]
       +\mathrm{poly}(\beta,s)e^{-cP^2}.
\]
The choice \(s\asymp s_{**}\) puts both extra terms below \(C s^{-3}\). The centered Hölder/Cauchy and fine-uniform Ward reduction of §4.125 finish the proof. This calculation controls an actual signed interaction correction in the compact-law slope. It does not supply a bounded extensive susceptibility at zero.

### 4.130 The direct classical term on a protected pre-healing cube (P/L on the genuine regular graph)

Take \(J=\lfloor\gamma\log_L\beta\rfloor\) with \(1/(4+s)<\gamma<1/4\), using any positive exponent \(s\) no larger than the scalar classical exponent of T1 (7.108). Write \(B_\beta=(\log\beta)^q\) for a fixed sufficiently large collar power. A root here is protected in the physical sense: its complete \(J\)-top cube of radius \(B_\beta\), every required raw descendant and synthetic determining collar are contained in the genuine regular part of the mixed graph. In particular the top target agrees with the literal coarse constraint on this whole interior, and the physical minimizers on the comparison graph meet the real CMP102 (7),(9),(172) margins. The statement concerns their actual classical readout. It does not replace a previously integrated kernel, its selector or its normalized fluctuations by that readout.

There is a useful exact choice of homogeneous comparison target. Reflect the coarse gauge connection on the regular integer cube successively in its site faces and repeat it on the doubled periodic cube; reverse group elements on reversed bonds. On each elementary plaquette the resulting holonomy is a conjugate of an original plaquette or its inverse. A straight loop across the doubled cube from a seam returns along the reflected reverse path, so its transport is identity. A coordinate tree on this torus therefore has link logarithms bounded by \(C B_\beta\delta\) when the plaquette defect bound is \(\delta\): express a nontree link by at most \(C B_\beta\) plaquettes in a fixed number of width-one strips, with the trivial winding included. The common coarse target on the original cube is preserved *as given*, prior to this tree gauge. The construction neither enlarges a plaquette threshold by a cut-off interpolation nor requires commuting global links. It is made on the raw coarse target, not by presuming that an arbitrary fine blocking convention commutes with reflection.

Let \(\Gamma\) be the actual mixed constrained minimum and \(\Gamma'\) the homogeneous minimum for this reflected target, in a physical interface frame. Inside the protected cube their invariant curvature/current readouts through the fixed orders needed for the classical value differ by at most
\[
 C\,\mathrm{poly}(\beta,B_\beta)L^{C J} e^{-c B_\beta}.
 \tag{PROTECTED-CLASSICAL-MINIMUM}
\]
Here are the precise import and scope. Use the localized determining graph with its *own finer collar* as in the real comparison of T2 §4.76 and CMP102 (172),(190). Variations compactly supported on this graph preserve the common top rows and the prescribed collar. For \(\Gamma'\) extend by zero into the homogeneous variational problem; for \(\Gamma\) these variations preserve every original higher-depth constraint, since those are means of the untouched full rows and the protected stars. Thus both restrictions are local critical orbits on the same determining graph. Their interior target rows coincide. Only the outer synthetic finer rows can differ. In a block-based frame fixing the top anchors, the real regular plaquette estimate and the raw-prefix strip bounds put each such target into the same fixed local small ball with size \(C\,\mathrm{poly}(B_\beta)g_Jp_J^{C}\); this tends to zero. This last membership and equality of the genuine interior rows are essential hypotheses of the protected chart, beyond merely having a small plaquette at the tested root. Interpolate these independent collar targets in this local target ball; the native response (190) to each collar slot at distance at least \(cB_\beta\) has its exponential decay. Counting even all fine collar slots and taking the fixed physical differences for the curvature/current costs at most the displayed polynomial and \(L^{CJ}\). No common global complex path through a rough exterior is used. This proves the zeroth-order physical comparison on such graphs; derivatives would additionally require common admitted local analytic directions and spare radius.

CMP119 (2.4),(2.5) imposes \(R_b\ge(\log g_b^{-2})^r\), \(r\ge1\), on the original weak margins. With empty initial geometry and the present \(J\) this precludes a healing *before* \(J\): all running inverse couplings on this prefix are comparable to \(\beta\), and the stated \(J\) is strictly shorter than an earliest original wait. A genuine rough component there is unprocessed. This simplifies the protected comparison; an unprocessed exterior can still affect a sharp integration domain.

At each protected fine root T1 (7.108), restricted to the *real* reflected homogeneous graph, bounds the unscaled classical frustration by \(C\,\mathrm{poly}(B_\beta,p_J) g_J^2 L^{-(4+s)J}\). Multiplication by \(\beta\) gives the true unamplified classical term. A fixed compact polynomial in a completed stencil is Lipschitz for its finitely many physical curvature rows, so (PROTECTED-CLASSICAL-MINIMUM) adds only its stated exponentially small loss times \(\beta\) in comparing back to the genuine mixed minimum. Since the number of fine roots is at most \(CV\), the total classical term multiplied by an additive-source parameter \(O(1/\beta)\) is bounded by
\[
 C V\,\mathrm{poly}(\log\beta)\,\beta^{-1}L^{-(4+s)J}
       +CV\,\mathrm{poly}(\beta,B_\beta)L^{CJ} e^{-cB_\beta}
       =o(V/\beta^2)
 \tag{PROTECTED-CLASSICAL-PRESSURE}
\]
for sufficiently large fixed \(q\). This pays the direct classical term on the stated protected roots at the pressure scale of §4.128. The deterministic reflection extension and physical saddle comparison do not give the complete marked scalar on those roots. The still missing comparison includes the integrated fluctuation determinant on its actual old physical/current graph, the statistical scalar generated at each new integration, and any response of the original sharp selector.

### 4.131 Tilted early occupancy and the new homogeneous scalar endpoint (P/L on the specified processes)

The real Wilson comb tilt gives a bound on the *actual* early history occupation without reflection of its selectors. Disintegrate the original positive unmarked history law over its fine Wilson configuration and keep that conditional history law when tilting by \(e^{tY^h}\). Its entropy relative to the unmarked joint law is exactly the fine-field relative entropy,
\[
 D_t=t\,\mathbb E_tY^h-\log\mathbb E e^{tY^h}
       \le CV(t^2+|t|s_{**}^{-3}).
\]
Indeed the difference between the true and Gaussian pressure slopes at all real \(u\) between zero and \(t\) is at most \(C s_{**}^{-3}\). Integrating \(p'(t)-p'(u)\) with this bound and the bounded Gaussian second derivative proves the inequality for both signs. The entropy variational inequality applied to \(s_0 V_{\le J}\) and (EARLY-RELEASE-VOLUME) now gives
\[
 V^{-1}\mathbb E_t V_{\le J}\le
 C\left[t^2+|t|s_{**}^{-3}
  +e^{-a p_J^2}\sum_{\ell'=1}^K e^{-p_{\ell'}}
  +V^{-1}\log\bar B_{\rm stop}\right].
 \tag{TILTED-EARLY-OCCUPANCY}
\]
A uniformly sampled \(J\)-tile with \(b\)-tile collar therefore has bad-footprint probability at most \(C b^4\ell^4\) times the displayed right side, by counting the intersected tiles. Translation by an allowed joint blocking cell gives the same bound at any equivalent tile. For \(b\) a fixed logarithmic power, \(\ell\asymp\beta^{1/3}\), and \(|t|\le c/\beta\), this is \(O(\beta^{-2/21}\mathrm{poly}(\log\beta))+o(1)\) on the required weak trajectory. This bound averages over the genuine tilted exterior; an exterior forcing an occupied tile need not have a small conditional probability. It gives no concentration assertion for an unverified auxiliary selector.

For comparison, the earlier *new first scalar* endpoint terms can be paid on a complete homogeneous matched hierarchy at an early stop. Normalize the bare direction as \(Y^h/\beta\), so its vacuum-subtracted initial fixed-chart amplitude at an old root is \(O(1)\). Use the original scalar carriers and (7.175),(7.178) in T1, with their common physical current graph, fixed-selector margins and real weak terminal chart. At a scale \(k\) a new statistical first-row carrier gains \(C_h g_k\) relative to the previous total amplitude. Summing its old rooted weights over descendants costs only the inverse old-root count already canceled by the fourth-power estimate of (7.175). Thus along \(J=O(\log\beta)\) the new amplitudes per current home satisfy \(a_k\le C g_0(1+Cg_0)^J\le C' g_0\). Here \(a_k\) denotes only the newly born scalar at its own scale; the initial deterministic classical tag is separate. For each new \(k\)-scalar the terminal zero-fluctuation evaluation, after its own vacuum subtraction, has the factor \(L^{-4(J-k)}\epsilon_J^2\) from (7.175) and the zero first raw jet on the stated fixed chart. Here \(\epsilon_J\le C g_J\mathrm{poly}(\log\beta)\) is the physical terminal field/current radius. This extra \(\epsilon_J^2\) follows by Taylor on a fixed smaller fraction of that chart; it cannot be taken on a shrinking-radius replacement. Summing the \(O(V L^{-4k})\) homes at each old scale gives
\[
 \left|\sum_{\rm new\ homogeneous\ first\ rows}
          (\text{endpoint value}-\text{vacuum})\right|
 \le C V\,J\, g_0^3\,\mathrm{poly}(\log\beta)\,L^{-4J}
       =o(V/\beta^2)
 \tag{EARLY-HOMOGENEOUS-SCALAR-ENDPOINT}
\]
when \(\gamma>1/8\). The absolute estimate holds on the indicated admitted homogeneous terminal graph, and refers to \(Y^h/\beta\). It does not compare history-dependent vacuum scalars, a sharp site selector, or the source-shifted exterior density. The pre-healing protected mixed minimum in §4.130 pays its direct classical term, but transferring (EARLY-HOMOGENEOUS-SCALAR-ENDPOINT) and the required scalar log moments to the punctured physical integral still requires the corresponding fluctuation-carrier comparison there.

### 4.132 The first protected integration with its actual denominator and fixed selector (P/L on the ordinary first-step graph)

Normalize a microscopic mark as \(D_x=h_x/\beta\), and let \(\xi\) denote the complete unmarked exterior retained by the *first* operation: its coarse target, original history determination and unintegrated exterior coordinates (later randomness may also be retained). Consider a set \(I=I(\xi)\) of marked roots whose complete native-coordinate annuli of radius \(b\) lie in the regular original first-step domain. Use \(b=(\log\beta)^q\) with fixed sufficiently large \(q\), and the compatible protected real chart of §4.130. Write \(D_I=\sum_{x\in I}D_x\). At real fixed \(|z|\le c_0\), define \(K_\xi(z)=\log\mathbb E_0(e^{zD_I}\mid\xi)\). On the matched graph one has
\[
 \begin{split}
 |K_\xi(z)-zK_\xi'(0)|
 &\le C z^2 g^2\left[g^2V+\mathbb E_0(S\mid\xi)\right]
                 + C |z|V\,\mathrm{poly}(\beta,b)e^{-c b},\\
 \log\mathbb E_0 e^{z(D_I-\mathbb E_0(D_I\mid\xi))}
 &\le C V/\beta^2 .
 \end{split}
 \tag{PROTECTED-FIRST-INNOVATION}
\]
Here \(g=\beta^{-1/2}\), \(S\) is the original compact Wilson energy, and empty or excluded roots can be assigned coefficient zero. The second assertion holds after averaging the same real exterior; for a subfamily of exteriors use zero marked set on its complement. This is an innovation estimate; \(\log\mathbb E_\xi e^{K_\xi(z)}\) still contains the fluctuations of the retained means.

**The selector.** CMP119 printed pp.249–250 solves the \(QA'=0\) equations on \(b_0(c)\) and integrates the independent \(A(b)\) on the remaining coordinates. The starred sets in (1.18) contain precisely these independent slots. The passing conditions are products of their original norm balls with real radius \(P=A_1p_0(g)\). In the protected region the duplicate physical characteristic function in (1.19) is one by its strict margin. The analogous statement on higher top interiors is (3.16),(3.19). Comparing two original regular top integrands at common **canonical \(A\)**, after aligning their admissible real frames, uses the same product of balls. The transformation of the slots under a real site gauge is orthogonal by (1.17). The physical readouts, Jacobians and densities can differ. Holding the physical microscopic \(U\) instead when changing the minimum generally moves the ball and does not support this argument. An incoming mark is inserted on the original fibers throughout; no source-dependent critical point or differentiation of a hard indicator is performed.

**A normalized annular integral.** Fix \(x\in I\) and an annulus contained in its protected chart. Condition on all first-step independent coordinates outside the interior of this annulus. When \(A\) is varied inside, the original first-step Wilson/axial and single-link Haar/constraint Jacobian integrands have fixed range in native units: each eliminated corridor bond is solved from its own block-average equation and uses its two adjacent blocks, as in T1 Lemma 7.19 and CMP109 (2.11)–(2.12). The top independent coordinates and their external collar have magnitude at most \(P\). At fixed \(\xi\) all raw background-only scalar factors cancel in the normalized ratio, including any vacuum/determinant constant depending on \(\xi\). The conditional integrals still include the \(A\)-dependent Jacobians, the true gauge action and the real marked terms. The unmarked conditional stationary action has no constrained linear term, as in CMP119 after (1.16).

For specificity, on this real first-step annulus the Hessian in the independent variables is bounded above and below by fixed positive constants; the lower bound concerns the constrained fluctuation coordinates. The flat precision on the independent \(QC A=0\) slice with its native exponential axial gauge has a fixed positive gap, and a principal submatrix keeps this lower bound. In a common real gauge on the protected cube the local physical saddle links and their current have size \(o(1)\) on every complete stencil (the polylogarithmic size of the cube is allowed). The difference of the stationary Hessian from the flat one has finite-range row and column norm \(o(1)\), by analytic differentiation of the fixed-range physical map and the actual gauge term, including its current times second-readout term. On the full first-step product balls the Taylor remainder has Hessian norm \(O(g(1+P)^C)\): expand each fixed plaquette or gauge contour on the physical chart \(gCA-hD(gCA)\), retaining its quadratic part; each cubic or higher term costs that factor after two canonical derivatives. The fixed-range Haar and constraint Jacobians have bounded analytic physical derivatives and canonical Hessian \(O(g^2)\). Summation uses only a fixed number of stencils at each bond. A source \(zD_x\) adds \(O(|z|g^2)\) to that row norm even for bounded coefficients on all roots. All these perturbations tend to zero compared with the gap. The same assertions hold with arbitrary admissible pinned collar fields. This first-step proof does not infer a gap for an inherited action at \(j>0\).

On a convex product of these norm balls, the positive Hessian and its fixed range give
\[
 |\operatorname{Cov}(F,G)|\le C\sum_{i,j}e^{-c d(i,j)}
                     \|\partial_i F\|_2\|\partial_j G\|_2 .
\]
Use the one-form Poisson inverse with a small exponential index weight as in §4.64; sitewise convex barrier approximations to the balls preserve the estimate. Weights commute with the diagonal barrier Hessian; the bounded-range row change is \(O(\alpha)\) for weight exponent \(\alpha\). This proof keeps both numerator and denominator of the real conditional law.

In particular canonical second moments at a slot a distance \(d\) from the pinned boundary are bounded by \(C+C P^C e^{-c d}\). For the variance this follows at once from the preceding identity. For the mean, interpolate the conditional negative log density between the centered zero-pin Gaussian quadratic on the same balls and its true stationary quadratic and remainder, treating nonzero pins as boundary fields. One can start from the true quadratic at zero pins, which is centered by parity. The gradient of the nonlinear remainder has sup norm \(C g(1+P)^C\) per slot, the real source adds \(C c_0 g(1+P)^C\), and the pin terms are supported on the collar with polynomial sup norm. Along this interpolation the Hessian remains bounded below. Pair the slot against each local action derivative by the covariance inequality; the bulk bound is \(o(1)\) and the boundary sum decays exponentially with \(d\). This gives the moment assertion. More generally differences between *arbitrary* admissible pins have exponentially small effect on the root normalized mean by interpolating the two actions on the *same* product balls, with their difference supported on the collar. No ratio of two unrelated small conditional masses is taken.

The physical map gives \(\|\partial_iD_y\|_2\le C g(\sqrt{e_{\Gamma,y}}+g)+\mathrm{poly}(\beta)e^{-c d}\) on a slot incident to \(y\), zero outside its fixed range. Here \(e_{\Gamma,y}\) sums the true saddle plaquette energies in that stencil. Indeed \(|F_{y,i}|\le C\sqrt{e_y}\), the physical readout derivative costs \(g\), and the difference of the compact plaquette at \(U(A)\) from its saddle value is bounded by \(C g\sum_{\rm incident}|A|\). The moment bound just proved applies on the deep sites; on the remote collar the global compact force and derivative bounds suffice. At fixed pins differentiating the normalized root expectation along the real source gives exactly the sum of the connected \(\operatorname{Cov}(D_x,D_y)\)'s. The exponential estimate, and \(2ab\le a^2+b^2\), bound it by
\[
 C g^2\sum_{p}e^{-c'd(x,p)}(s_p(\Gamma)+g^2)
       +\mathrm{poly}(\beta)e^{-c'b}.
\]
The exterior annulus pins need not have the same distribution at \(z\) and at zero. The uniform pin-oscillation bound compares any two of them at the root, so the same estimate integrated over the real segment from zero to \(z\) holds with an additional exponentially small error for the two different pin laws. This argument is applied separately at each root; there is no independence assumption on the exteriors of the annuli.

On deep plaquettes the unmarked bound on \(A\) and the physical map give \(s_p(\Gamma)\le C\mathbb E_0(s_p(U)\mid\xi)+Cg^2+\mathrm{poly}(\beta)e^{-c'b}\). This uses the actual compact measure, not a gauge-fixed minimizing competitor that might fail a selector. Remote compact saddle plaquettes are bounded and their weighted contribution is exponentially small. Sum the exponential kernels over the marked roots and integrate the first-derivative comparison to prove the first line of (PROTECTED-FIRST-INNOVATION). For the second line use conditional Jensen on \(e^{C g^2\mathbb E_0(S\mid\xi)}\). The unmarked marked-set estimate and convex scaling give \(\log\mathbb E_0 e^{C g^2 S}\le C V/\beta^2\); the polylogarithmic collar error is smaller. This pays the genuine first-layer scalar fluctuation, including the normalization of the original exterior, at the required additive scale.

**What actually happens on the unprocessed exterior.** On a shell the second factor in (1.19) need not be redundant. CMP119 printed p.269 identifies the nonlocal dependence of \(\chi'_k\) in (3.21) through \(V^{(k)}\), then uses the actual change of the \(S_{k+1}^*\) variables in (3.22) to replace it by the restricted determining-background factor. The other indicators are unchanged; the action acquires a localized smooth change involving \(H^{(k)}\) and the corresponding measure changes must remain in the density. At fixed first-layer targets these are external to the annular integration above. Repeating the proof at a later stage must use the post-change determining data and inherited kernels. A comparison at fixed old physical links without that change could cross the discontinuity at an arbitrarily small displacement; the pass/fail function itself has no pointwise Lipschitz bound at its threshold. Localization of the original unmarked (3.47) on a common carrier states equality as a function of its physical arguments; evaluating the normalized source on a different graph and changing the exterior law are further operations.

### 4.133 Normalized summation, the remaining source comparison, and which disc is available (P reduction)

Use the reverse hierarchy through the early stop, retaining the full physical history determination. For the additive good mark let \(D_j=\mathbb E_0(D_I\mid\mathcal F_j)\) with \(\mathcal F_0\supset\cdots\supset\mathcal F_J\). The indicator selecting its marked roots is fixed on each such history. Write \(\Delta_j=D_j-D_{j+1}\) and
\(\psi_j(t)=\log\mathbb E_0(e^{t\Delta_j}\mid\mathcal F_{j+1})\).
Iteration of normalized conditional expectations and Cauchy–Schwarz give the exact exponential-martingale estimate
\[
 \mathbb E_0\exp\!\left[\sum_j(2t\Delta_j-\psi_j(2t))\right]=1,\qquad
 \log\mathbb E_0 e^{t(D_0-D_J)}
     \le \tfrac12\log\mathbb E_0\exp\!\left[\sum_j\psi_j(2t)\right].
 \tag{NORMALIZED-REVERSE-SUM}
\]
Nonindependent predictable energy costs can therefore be paid under the original joint law; multiplying worst-case bounds on unrelated normalized histories is unnecessary. The first term is controlled by (PROTECTED-FIRST-INNOVATION). The terminal \(D_J\) is still a random scalar and its centered log moment remains in the problem. In particular replacing the exterior by a reflected homogeneous law and averaging its covariance would omit this part of the sum.

To state the sufficient scalar comparison precisely, suppose the normalized good-branch integrals at both signs of a fixed real additive parameter, and the small interpolation interval between them, have an upper bound \(z m_{\rm vac}+CV/\beta^2\) after integration in the original exterior. The scalar \(m_{\rm vac}\) must be a single deterministic microscopic vacuum response, with the missing-root/vacuum differences of the excluded footprints paid as in §4.128. That section pays the bare additive source there at either sign and at fixed larger strengths, so Hölder can put it back. Jensen at both parameter endpoints then also controls the difference between \(m_{\rm vac}\) and the actual additive mean by \(CV/\beta^2\). Equivalently one can prove the centered real log bound directly with \(D_J\) retained in (NORMALIZED-REVERSE-SUM).

At the final step in this implication, the positive real pressure bound and the complex input refer to different operations. First use Hölder over the eight translated weighted combs to obtain \(CV/\beta^2\) for the centered real log of the **fine-uniform** \(Y_0/\beta\) on a fixed interval. For the analytic one-sided Cauchy estimate it is the full *fine-uniform* complex moment generating function of \(Y_0/\beta\) that must be zero-free on a fixed disc there. This follows only on the exact smooth finite family of short loop and tensor-product actions in §4.117; even the Ward alias reduction uses the six smooth oriented plaquette clauses separately. With both hypotheses the real-part bound on the complex circle gives \(\operatorname{Var}(Y_0/\beta)\le CV/\beta^2\), so (FINE-UNIFORM-WARD-REDUCTION) proves the desired all-mark bound. No fixed comb-source disc is needed in this implication. On the strength already proved, (CUBIC-CORRECTED-SUS) gives the growing bound; a larger *fine-uniform unamplified* disc of radius \(c\,s_{**}^{-3}\) is sufficient but has not been proved. The available additive smooth disc in that parameter has radius only \(c/\beta\).

For example a symmetric scalar \(X=\pm V/\beta\) has centered log at real strength \(z/\beta\) bounded by \(|z|V/\beta^2\), yet variance \(V^2/\beta^2\); its additive generating function has zeros at distance \(\pi\beta^2/(2V)\). This only verifies the need for the same-source complex hypothesis in the preceding inference. It is not a claim about the Wilson measure.

The interpolation left by the actual first step has an identifiable extra term at the next stage. On a fixed differentiable physical target path \(q(\theta)\) and the original coordinate balls, for a normalized previous-root mean \(m(q)=\langle D_x\rangle_q\),
\[
 \partial_\theta m
 =\langle\partial_\theta D_x\rangle_q+
       \operatorname{Cov}_q(D_x,\partial_\theta\log w_q).
 \tag{INHERITED-NORMALIZED-SCORE}
\]
A second derivative also contains the connected three-insertion term with two \(\partial_\theta\log w_q\)'s. Constants in this log density cancel, but the actual derivative of its field-dependent determinant, gauge action and the smooth correction left by (3.22) do not. A Hessian estimate on the new bare quadratic form alone omits these insertions. An accepted comparison would have to bound the inherited first rows on their actual \(U,J,A\) arguments and pay their second centered conditional response with the density normalized on precisely those arguments. The homogeneous vacuum/endpoint estimate in §4.131 supplies a reference after this matching; it has not proved that all the normalized source integrals on the punctured prefix satisfy the required real bound.

### 4.134 The protected coarse Wilson energy has a uniform fine-energy payment (P)

For the actual symmetric block average of CMP109 (0.11)–(0.12), let \(I\) be any set of oriented coarse plaquettes with complete fixed-size determining stars in a regular region of the incoming lattice. Let \(\widehat I\) contain their fine determining plaquettes, of all orientations, and let \(\epsilon\) bound the incoming plaquette defects on those stars. Then
\[
 \sum_{p\in I}s_p(MU)\le (1+C_L\epsilon)\sum_{q\in\widehat I}s_q(U).
 \tag{COCHAIN-WILSON-ENERGY}
\]
The constant is independent of the torus and of the number of scales. The factor tending to one is important; a fixed constant greater than one iterated at every step would not give the following conclusion.

At the identity let \(Q_1\) be the linearized link average. Its \(\mu\)-component is the uniform average over \(x\in B(y)\) of the straight \(L\)-step \(\mu\)-line from \(x\), plus the difference of the two site contour averages at \(y\) and \(y+L e_\mu\). Indeed (0.11) is permutation symmetric and equivariant; its first derivative at equal identity arguments is their arithmetic mean (each derivative is identical and their sum is the identity). In (0.12) the linear reference straight transport cancels against the same reference inside the logarithm. The site-contour terms disappear on taking the coarse curl. Thus \(dQ_1=Q_2 d\), where on a \(\mu\nu\)-plaquette rooted at \(y\)
\[
 (Q_2 F)_{\mu\nu}(y)=L^{-d}\sum_{x\in B(y)}
       \sum_{u,v=0}^{L-1}F_{\mu\nu}(x+u e_\mu+v e_\nu).
\]
This is the exact rectangle identity for the linear curl. The positive matrix has row sum \(L^2\) and column sum \(L^{2-d}\), counting wrap-around with multiplicity. Its \(\ell^2\) norm is at most one in four dimensions by Schur. [Bałaban, CMP109, pp.252–254](https://doi.org/10.1007/BF01215223).

For each output plaquette tree gauge its own fixed-size contractible determining star. Every required link logarithm is bounded by \(C_L\sum_{q\in Y_p}|F_q|\), and by \(C_L\epsilon\), where \(F_q\) is the principal Lie logarithm of its holonomy. Fixed strips fill the fundamental cycles; enlarge the determining star by a fixed number of layers if needed. Taylor's theorem in this chart and the preceding derivative identity show
\[
 |F_p(MU)|\le (Q_2|F|)_p+C_L\epsilon\sum_{q\in Y_p}|F_q|.
\]
In fact the quadratic Taylor errors are bounded by the product of the two link-size bounds, and \(dA-F=O_L(\epsilon)\sum_{q\in Y_p}|F_q|\) in the same chart. Different local tree gauges cause no problem for this scalar norm inequality. The error incidence matrix has bounded row and column sums for fixed \(L\), and its norm is \(O_L(\epsilon)\). Restrict the output rows to \(I\) and set the unneeded input norms to zero. Finally the real plaquette action equals the fixed metric multiple of \(|F|^2\) with relative error \(O(\epsilon^2)\) on both input and output (the coarse defect is at most \(C_L\epsilon\)). This proves the claim.

On a genuinely protected prefix every relevant \(W_i\) on these complete stars is the raw average of the preceding field, up to its allowed endpoint gauge. Expand the required stars backward; their total extra radius in the final units is bounded by a geometric series. On the actual regular inputs through \(J=O(\log\beta)\), \(\epsilon_i\le C g_i p_i^C\) and \(\sum_{i<J}\epsilon_i=o(1)\). Iteration gives
\[
 \sum_{p\in I_k}s_p(W_k)\le C S(U)
 \tag{RAW-PROTECTED-ENERGY}
\]
for any union of such protected sets at a *single* scale and their complete clean descendants, in the full positive joint law. Raw data not related by the physical averaging are excluded. The proof does not substitute a different minimizing competitor, altered gauge density or reinitialized interior.

For later reference suppose a protected canonical step has bounded second moments for its interior coordinates (a fixed small positive quadratic test in the normalized unmarked integral suffices). Its true regular background \(V^{(k)}\) and its actual \(W_k\) differ on a plaquette by at most \(C g_k\sum_{\rm local}|A|\) in chord norm. Hence for any such set \(I_k\) measurable in the retained exterior,
\[
 \sum_{p\in I_k}s_p(V^{(k)})\le
 C\,\mathbb E_0[S(U)\mid\mathcal F_{k+1}]
       + C g_k^2 |I_k|+\text{summable collar error}.
\]
The raw fine-energy inequality is applied to the same unmarked observations, including the chosen set; there is no requirement that the sets be independent. If the coefficient at stage \(k\) is \(g_k^2 w_k\) with deterministic \(w_k\ge0,\ \sum w_k\le C\), Hölder or convexity and conditional Jensen pay all these first terms together by \(\log\mathbb E_0 e^{C' g_0^2 S(U)}\le C V/\beta^2\). This is precisely the kind of random payment needed in (NORMALIZED-REVERSE-SUM).

### 4.135 Real replacement of inherited means on a pre-healing collar (P reduction with explicit graph and reference conditions)

At scale \(k\), retain the original unmarked exterior and all future determination. For a fine root \(o\) persistently protected through \(J\), put \(m_{k,o}=\mathbb E_0(h_o/\beta\mid\mathcal F_k)\). Denote by \(f_{k,o}^{\rm hom}(W)\) the normalized first row of the homogeneous process at current target \(W\), *including its vacuum*. The homogeneous process must have the same unmarked coupling and selector normalizations on the compared ordinary top carriers. Let \(\mathcal R_o W\) be the site reflection extension of a deterministic protected cube in the current graph. The following comparison uses real sup errors, so it never differentiates an inherited mixed marked coefficient on an old \(B\)-member.

Fix \(r=D(\log\beta)^2\) and a larger fixed power \(b=(\log\beta)^q\) dominating \(r^4(1+P_{\max}^2)\), the finite-history growth \(O(J^2)\), and the original determining collars. Reserve sufficient additional collars at the few scale endpoints; even \(O(Jb)\) in \(J\)-units is permitted by §4.128. The following two matters need separate verification on the original processes.

1. On each two-way ordinary integration the unmarked local test estimate (7.269) of T1 is used with the actual coupled coefficient difference \(\Delta_b\). The smallness sufficient here is \(\Delta_b\le e^{C J^2}e^{-c b}\) on a fixed smaller fraction of the collar. The test is an arbitrary bounded function of at most \(O(r^4)\) *real* independent slots with one extra fixed layer. Their determinant and Gaussian normalizations cancel against the original denominator. CMP116 (2.3)–(2.8) keeps these slots inside the conditioned Gaussian domain; only its exterior variables undergo the whitening change. The test is never differentiated in a complex weakening. The first localized kernels of CMP119 agree with the homogeneous kernels on the common complete top graph as functions of their arguments, and (3.22) is included at the actual shell. The tail of a carrier traversing this collar is exponentially small by the ordinary walk norm. If the actual analytic unmarked coefficients share their stated spare chart, their difference at the near physical arguments costs the corresponding Cauchy radius and a polynomial in the old mesh/counting factors. Equality of a single critical action by itself is not a bound on all these coefficients; \(\Delta_b\) includes the conditional precision, its walks, the inherited unmarked terms and their determining graphs.

2. For matched upper data on the whole collar, the real synthetic-collar comparison in §4.130 applies to each actual top lift \(V^{(k)}=M^k\Gamma\), including its full fixed current-block contours. CMP119 printed pp.266,268, (3.10),(3.17)–(3.19) uses exactly this current readout. If a site gauge \(\gamma\) aligns the two lifts to error \(d\) throughout one such block, their two untransformed based contour values are both identity. Endpoint covariance and the fixed contour Lipschitz bound give \(\|\gamma(x)-\gamma(y_{\rm block})\|\le C_L d\). The blockconstant lift of the coarse-site gauge therefore aligns their local data to the same accuracy. Its rotations on the independent slots preserve their product balls and have unit Jacobian. It can agree with the identity at the actual retained exterior by terminating the lift in another outer collar; wall-reaching clusters are counted before that collar. Equivalently one can rotate the stated exterior arguments as a change of representation, but one must not hold a different exterior law fixed. This is a one-step physical comparison at real data. No derivative of a global Landau-to-axial gauge is inferred here.

On the registered regular graphs with these common margins, and with a homogeneous source reference admitting the localized bounds of T1 (7.108),(7.143),(7.175),(7.178) for its *actual* cutoff, the comparison satisfies
\[
 \left|m_{k,o}- f_{k,o}^{\rm hom}(\mathcal R_o W_k)\right|
 \le k\,C\big[e^{-c r}+\exp(CJ^2+C(1+P_{\max}^2)r^4-c'b)\big].
 \tag{REAL-MEAN-INDUCTION}
\]
The constants allow the fixed number of steps between the \(h\)-block endpoints in T1. The tori, reflection placements and anchor phases are chosen deterministically at each scale. For the proof at \(k=0\) the raw source is on its complete fine stencil. At the next step substitute the real estimate at \(k\) inside the *normalized* actual expectation: this costs at most its sup error, without amplification. Truncate the homogeneous first-row carrier at radius \(r\) in current coordinates after its vacuum has been recorded. Its removed real sup is \(O(e^{-c r})\) on the admitted homogeneous target. In particular changing a more distant periodic closure changes its localized evaluation by this bound, including its vacuum winding terms when their localized comparison holds. For each retained piece \(W_k(A)\) uses only the fixed current constraint corridors around its real support at fixed upper data. Compare first its physical value at the same real coordinates using item 2. The first-step analytic word and corridor maps have fixed-scale Lipschitz bounds; at earlier scales even a factor \(e^{CJ^2}\) fits the collar. Apply item 1 to the *reference* real function on these slots. The outcome is the homogeneous unmarked conditional expectation, supplying the next first-row comparator. Current-to-fine expansion of all required complete collars over \(J\) levels is bounded by a geometric scale sum (the more conservative \(Jb\) also suffices). This proves the displayed induction. It requires no bound on derivatives of the difference on the left and no equality of full conditional partition functions at unlike exteriors.

**A route from these comparisons to a centered real pressure.** On the same homogeneous margins the initial deterministic \(H\) endpoint has the extra age in T1 (7.108). Its improved full-function sup is converted to an anchored carrier norm by applying T1 (7.143) once after removing the rough \(L^{-4k}\) factor from (7.175) and using spare decay. This loses a fixed fraction of the positive exponent. After summing fine roots into a current home, this gives \(C L^{-s'k}\), \(s'>0\), for this initial origin. All the new first-row origins together have at most \(Ck g_0(1+Cg_0)^J\) by (7.178); the physical current slots are evaluated on their own homogeneous graph. Thus one may use the deterministic envelope
\[
 a_k=C[L^{-s'k}+k g_0],\qquad \sum_{k<J}a_k^2\le C .
 \tag{EARLY-SOURCE-WEIGHTS}
\]
Carrier rates and physical radii must be those of the homogeneous reference throughout this calculation. The terminal *classical* estimate still uses (7.108) itself when choosing \(\gamma\); a loss of exponent in (EARLY-SOURCE-WEIGHTS) does not change the terminal classical criterion.

At fixed actual upper data, replace \(D_k=\sum_{o\in I}m_{k,o}\) by the proxy sum via (REAL-MEAN-INDUCTION). Multiplication of the real exponential by \(e^{\pm |z|V\epsilon_{\rm ind}}\) pays the entire sup error without a comparison of two small denominators. The deterministic zero-fluctuation value of the proxy may be removed inside a centered conditional moment. Its remaining true single-step expression can be tested on the original coordinate balls, with any root-specific blockconstant rotation as in item 2. T1's bounded-real test estimate (7.270) requires a simultaneous source budget, not merely two independent single-vertex estimates. On a fixed physical coordinate disc the test in T1 (7.271) is particularly convenient. Taylor the *whole* proximal scalar at its fixed background \(W_*=V^{(k)}\). Its first derivative on each bond is now an exterior coefficient, multiplied by one local physical bond displacement of size \(O(g_k|A|)\). The squared sum of these coefficients is bounded by the stated \(a_k^2\) times a local plaquette-energy sum, with exponentially small tails, via a separate rooted gauge for estimating each fixed derivative. The second-order Taylor parts of individual analytic carriers cost \(C g_k^2 a_{X}\sum_{b\in X}|A_b|^2\) on their original finite supports. The potentially long tree used to estimate the *deterministic* gradient is not inserted in the random test. The incoming decay must exceed the \(C^{|X|}\) root cost of the mixed Gaussian expansion. On the real paths, the elementary gauge/map nonlinear remainder is included in this same budget. With that budget the unmarked Gaussian reserve gives, on both signs of a small fixed real tilt, the centered variance bound (7.270), and hence
\[
 \psi_k(2z)\le C_z a_k^2\big[g_k^2 S^{\rm prot}_{\Gamma,k}
                                    +g_k^4 V_k\big]
       + C_z V\epsilon_{\rm ind}+O(V e^{-c r}) .
\]
Here \(V_k\le C V L^{-4k}\); \(S^{\rm prot}_{\Gamma,k}\) sums only the genuinely protected determining stencils. The bound on the top coarse canonical second moments follows by the same one-slot bounded/exponential test with its fixed Gaussian reserve. Section 4.134 then bounds the resulting conditional background energies by conditional fine energy plus \(C g_k^2 V_k\) and exponentially small tails. Equations (EARLY-SOURCE-WEIGHTS), (NORMALIZED-REVERSE-SUM) and unmarked MarkedExp give \(CV/\beta^2\) for the log moment of \(D_0-D_J\).

For \(D_J\) the actual real comparison, the classical bound (PROTECTED-CLASSICAL-PRESSURE), and the *new* homogeneous scalar endpoint (EARLY-HOMOGENEOUS-SCALAR-ENDPOINT) are all needed. Record the vacuum at a fixed deterministic reflected size and at each root phase. Its sum over **all** fine roots is deterministic. The part missing from \(I\) is a random field: the size per missing additive root is \(O(g_0^2\mathrm{poly}(\log\beta))\) on the same homogeneous margins, from the zero-target moment of the fine insertion and its proper scalar increments. Its entire real log cost is paid by (EARLY-RELEASE-VOLUME), since \(L^{4J}(Jb)^4g_0^2\mathrm{poly}(\log\beta)\to0\). This accounts for the actual retained mean without replacing it by a typical stop field. Hölder restores the raw compact source on the bad footprint via §4.128. Under the common graph and homogeneous reference hypotheses specified above, this proves \(CV/\beta^2\) for the centered real additive log, first on the original comb and then on the fine-uniform source by the eight translates. Section 4.133 specifies the additionally required *same fine-uniform* complex disc, and only under its stated smooth action clauses does the inference to the ordinary variance follow.

This implication is not yet asserted for an unmatched homogeneous reference. In particular (1.18) uses \(\delta_0/g_0\) in the independent variables, while printed (3.16) writes \(\delta_k\) after introducing \(g_k A_k\) in (3.15). The physical threshold \(\delta_k\) corresponds to canonical radius \(\delta_k/g_k\); the actual squared large-field factor \(\delta_j^2/g_j^2\) on LFR II printed p.380 uses this convention. The broad physical starred-coordinate selector in CMP109 (2.9) differs from the narrow independent canonical window in radius. The determined corridor bonds are controlled by the starred coordinates (CMP109 printed pp.266–267). A homogeneous fixed-chart estimate on the former must be re-established on the latter, or transferred by a normalized estimate including the accumulated vacuum and field-dependent log. A different cutoff cannot be treated as a common physical conditional kernel. The formula for \(\Delta_b\) and the full real product budget must also be checked on every protected class used, including sharp exterior and current arguments; a single fixed-site comparison is insufficient.

### 4.136 Closing the early positive estimate on the specified native margins (P/L with the named imports)

T1 §§7.134–7.139 supply more than single-probe comparisons. Under their stated ordinary mixed convergence margins, the real Borel source-weight budget, and the homogeneous fixed-block analytic/precision margins, the early independent-window reference, the protected sup induction and the two-marked-integral estimate in §4.135 all hold. On the prescribed reference trajectory with these margins,
\[
 \log\mathbb E_\mu\exp\!\left[
      z\left({Y_0\over\beta}-\mathbb E_\mu{Y_0\over\beta}\right)\right]
     \le C V/\beta^2 \qquad (z\ {\rm real},\ |z|\le c_0).
 \tag{EARLY-FINE-UNIFORM-REAL}
\]
Use \(Y_0=\sum_{b\parallel0}h_b\) directly. This proof includes all compact configurations in the exterior law and uses unmarked rather than tilted reflection positivity. The conclusion with the smooth analytic clauses is
\[
 S_h(0)\le C,\qquad
 \operatorname{Var}_\mu(r_f)\le C\sum_b|f_b|^2 .
 \tag{EARLY-ORDINARY-SUS}
\]
The first inequality additionally requires the fixed analytic pressure disc for the concrete finite smooth additive loop/tensor-product family realizing \(Y_0/\beta\) in §4.117. The second also uses the six oriented smooth plaquette clauses in §4.113. The corresponding physical multiplier is \(c_\beta^{-2}a^{-4}\). This theorem does not give a fixed microscopic comb-source disc, a fixed physical dimension-six source disc, or reflected nondegeneracy.

Here is the verification of the previously separated conditions and the limits of the assertion.

* **Actual cutoffs and scalar normalization.** T1 Proposition 7.209 constructs the homogeneous reference on the same physical maps, independent canonical parameters and no-reset pre-healing prefix. The starred variables in the CMP109 broad cutoff also determine its dependent bond via the constraint (printed pp.266–267). The significant distinction is the radius. On the independent \(P_i\)-ball the larger physical window is satisfied for the chosen weak parameters. For a common broad reference with its verified margins the exact \(h\)-block scalar difference obeys
\[
 \delta E_{k+h}(q)=\log\mathbb E_{\rm broad}
   \left[e^{\delta E_k(W_k)}
       \prod_{i=k}^{k+h-1}\mathbf1_{\{\max|A_i|\le P_i\}}
                   \,\middle|\,q\right]
\]
with the full original constrained Jacobians and conditional normalizers. The extra failed-coordinate species have Gaussian cost \(e^{-c P_{\min}^2}\). Including the vacuum, the rooted change through the early prefix is at most \(\exp(CJ-cP_{\min}^2)\). Proposition 7.209 also gives a direct construction without comparing different coupling filings: keep \(\beta_0 S_i\) and its genuine nested minimum, use stationarity to start each \(i\)-th action excess at degree two in its own canonical field, and retain the field-dependent determinants and previously generated scalars. On its fixed homogeneous chart the norm recurrence is \(a_N\le C_h+C_h g_{\max}P_{\max}\sum_{j<N}a_j\), bounded uniformly since \(Jg_{\max}P_{\max}\to0\). Thus the original independent-window version of (7.175),(7.178) is available on those margins. The repeated canonical threshold is the physically consistent choice \(P_i=\delta_i/g_i\) discussed in §4.135, as used by the original LFR II squared reserve; this choice matters.

* **Coverage of a genuinely protected core.** Use only the actual occupied domains retained in the positive history, not previously resummed finer labels. Exclude all \(J\)-tiles whose complete determining stars and buffer encounter such a domain through \(J\). The original grid lengths \(M R_j\), the test radius \(r\), and all the added collars are fixed polylogarithmic lengths in the relevant scales. The geometric scale sum or \(O(Jb)\) inflation fits (ADAPTIVE-FOOTPRINT-ENERGY) with \(\gamma<1/4\). In the complement the original top-row regularity and redundancy statements are CMP119 (1.18),(1.19),(3.5)–(3.10),(3.16),(3.19). For a common raw target cube reflect all of its coarse links before comparing physical minima, as in §4.130. Complete local synthetic collars in block-based trees have target size at most \(C\,\mathrm{poly}(b)\,g_jp_j^C\), which tends to zero on this prefix. On the genuine CMP102 (7),(172) determining graphs the relative response (190) then gives differences \(C\,\mathrm{poly}(b)L^{Cj} e^{-cb}\) of the old physical links and their properly normalized currents at the complete stencils. Extra fine differences or collar slot counts cost \(L^{Cj}\), not a torus volume. This use is at real top rows; it is not an admission result for arbitrary complex mixed-wall data. The comparison of the two *raw current* links \(V^{(k)}=M^k\Gamma\) is also the finite-mesh comparison in CMP119 (3.17)–(3.19). On the matched current contour, both stationary representatives have contour value \(I\). Hence an aligning real fine gauge on a complete block differs from its blockconstant coarse lift by \(O_L(d)\) when the aligned link error is \(d\). One may change this gauge on the current nodes by \(O_L(d)\) while keeping the fine \(U,J\) data close; the genuine current slots have the stated polynomial fine-unit conversion. Its exact lift rotates the independent \(A\) without moving their radial window. No probability on a new exterior is used. Bałaban, CMP119, pp.265–269.

* **Normalized unmarked coefficient comparison.** A cluster with a near root either reaches outside the common collar, or has only ordinary matched determining stencils. For the latter CMP119 printed p.276 supplies the top homogeneous preintegration kernels; pp.278–279 give their counterparts in the already integrated action. Before the first possible healing there is no previous \(R\)-origin to propagate: the second term of (3.26) explicitly contains \(R''_k\), zero until one has been generated. The terms involving the actual \(B_k\), external \(A\), and the (3.22) smooth shell correction carry a true boundary support. Walking out through the protected region spends the spare ordinary decay; there is no resummed interior shortcut there. For the common local unmarked coefficient, compare its two physical arguments in its *same* enlarged analytic domain. At a protected real tuple the spare fractions of the native \(\alpha_{0,j},\alpha_{1,j},P_j\) windows cost at most \(L^{Cj}\mathrm{poly}(\beta,b)\) for one Cauchy difference in the correct old units. The analytic tuple includes the physical current and all original slots. The adjustment to the current gauge just described preserves the compact gauge saturation and the starred coordinate measure. Resolvent/precision walks are telescoped on the same ordinary covers; a differing physical coefficient costs the same small argument difference and a differing far walk reaches the collar. Their absolute sums have the same spare native rate, allowing the finite old-row choices to cost \(\exp(CJ^2)\) by conservative counting over all early stages. This yields the \(\Delta_b\) test of T1 (7.269),(7.272) on those common protected graphs. It is essential that the comparison is on the *unmarked* kernels; a new off-shell assertion about an old source-dependent \(B/J/A\) vertex would not follow. T1 (7.276) makes these same comparisons for two homogeneous tori as well as a mixed and a homogeneous one. Therefore a root at distance \(b\) can use its own real reflected current torus; truncation at \(r\) changes the sup by \(e^{-cr}\). The error in (REAL-MEAN-INDUCTION) follows with \(b\) large relative to the entire root expense. Bałaban, CMP119, pp.270–279.

* **Actual tilted tests and exterior energy.** Conditional on the unmarked upper state, choose each reflected root's small physical tree gauge at its zero-fluctuation field *before* integrating \(A\). At nonzero \(A\) the raw perturbation is \(O_L(g_k\max|A|)\) in that same chart. A folded support uses at most \(C|X|\) actual slots. Bound the linear coefficient by the complete rooted gradient estimate (7.271), retaining the true physical plaquette energies; its coefficients are deterministic in this conditional. The quadratic Taylor remainder of each original carrier has its own \(O(|X|)\) support. These facts prevent the spurious area-squared support loss that a fresh random tree gauge for every \(A\) would produce. T1 (7.270) at nonzero tilt uses a spare exponentially summable carrier budget **larger than the fixed real-test root cost**. With the corresponding margin the simultaneous perturbation has small summed constant/quadratic cost, since its nonconstant canonical coefficients are \(O(g_k\sqrt{s_p})\) and \(O(g_k^2)\), \(\sum_{X\ni e} e^{a|X|}\|f_X\|\le C a_k\), and \(|z|\le c_0\). The selected inner Gaussian integrals keep their quadratic reserve; their first two differentiated weights have norm \(C(g_k\sqrt{s_p}+g_k^2)\), independent of \(P_k\). Thus the centered conditional \(\psi_k\) bound in §4.135 holds. Every root-specific frame and mask is fixed in this conditional. This is a test on the original real independent coordinates, not an assumption that the true inherited mixed function is holomorphic in the same chart. By (COCHAIN-WILSON-ENERGY) the background term is charged through \(\mathbb E[S(U)\mid\mathcal F_{k+1}]\), with summable weights \(a_k^2\). The martingale exponential in (NORMALIZED-REVERSE-SUM) pays the accumulated conditional fluctuations on the actual unmarked law.

* **Terminal integration and inference.** For the classical original tag use the exponent in (PROTECTED-CLASSICAL-PRESSURE); for all new nonconstant first-row endpoints use (EARLY-HOMOGENEOUS-SCALAR-ENDPOINT). Choose \(\gamma>\max(1/(4+s),1/8)\) strictly below \(1/4\). Vacuum per missing additive root is \(O(g_0^2\mathrm{poly}(\log\beta))\) on the homogeneous reference (at the terminal identity the regular fine plaquettes are on the canonical small scale); differences of reflected sizes are included in the simultaneous comparison. The weighted count \(g_0^2\mathrm{poly}(\log\beta)L^{4J}(Jb)^4 V_{\le J}\) fits the early occupied-volume reserve. This leaves only a single deterministic vacuum sum, with the actual \(\mathcal F_J\) integration intact. Hölder restores all bad-footprint source terms, including the centered missing vacuum, and Jensen at both real parameter endpoints replaces this vacuum by the actual mean. This proves (EARLY-FINE-UNIFORM-REAL). A one-sided Cauchy bound on the fixed smooth disc for this **same** \(Y_0/\beta\), followed by (FINE-UNIFORM-WARD-REDUCTION), gives (EARLY-ORDINARY-SUS).

The scope is the early weak window on the reference tori and the stated original convergence, cutoff, and spare carrier margins in T1 (7.269)–(7.276) and T2's protected real comparison. The proof uses no assumption that every rough graph admits a complex marked readout. If only qualitative unmarked exponential decay is provided, rather than the needed spare support budget, or if the smooth additive pressure clauses are unavailable, the corresponding implication must remain conditional. Uniform all-history interacting composite mixing, higher cumulants and a physical reflected lower bound are separate obligations.

### 4.137 A nonzero action-density response on the genuine early physical graph (P/L on the same complete protected chart)

The susceptibility proof has a separate implication for physical action matching through the early stop. Fix one current \(J\)-plaquette \(p\) strictly inside a protected coarse cube. Take a nonnegative bounded fine action test \(f\) equal to one on the complete fine determining plaquettes for that \(p\), supported within a fixed number of \(J\)-cells around it. The support enlargement in (COCHAIN-WILSON-ENERGY) is bounded in \(J\)-units by the geometric scale sum; \(f\) may be the restriction of a smooth plateau on those units. Consider the original additive insertion \(A_f=\sum_{p'} f_{p'}s_{p'}\). In the same fixed history prescribe two real coarse targets on the common cube: \(W^0=I\), and \(W^t\) obtained by placing \(e^{itT}\) on just one of the bonds of \(p\), with \(T\) a fixed nonzero traceless Hermitian generator. Keep the true exterior beyond the cube the same. Use the regular comparison only when the complete original, synthetic and current stencils are present. Take \(t=\varepsilon g_J\) with a fixed sufficiently small \(\varepsilon>0\). Both local targets meet the real native regularity tests; the reflected comparison carries its extension at the boundary. The conditional means are values of the continuous physical conditional integral on these admitted targets, not probabilities of two individual configurations.

Their contrast satisfies, for all sufficiently large \(\beta\),
\[
 \mathbb E_0(A_f\mid W^t,\xi_{\rm out})
       -\mathbb E_0(A_f\mid W^0,\xi_{\rm out})
       \ \ge\ c_T t^2.
 \tag{PROTECTED-ACTION-CONTRAST}
\]
For the deterministic classical term at \(W^t\), apply (COCHAIN-WILSON-ENERGY) backward along its complete raw determining graph. At every scale the corresponding true local constrained minimum is a competitor with the required \(M^J\) value; the same repeated local energy inequality holds for that regular fine field. Consequently its \(f\)-weighted action is at least \(C^{-1}s_p(W^t)\ge c_T' t^2\). This use needs only the actual minimum/readout on the finite cube and the selected plaquette's complete stars. At \(W^0\) the reflected homogeneous field is flat. The real comparison of the original mixed minimum and its old current on the cube bounds its full fine \(f\)-weighted action by \(C L^{4J}\mathrm{poly}(\beta,b)e^{-c b}\). The number of fine roots in the test is \(O(L^{4J})\), not \(O(V)\).

For the statistical scalars apply the same real first-row induction at fixed sources, now to the finite local plaquette insertion. Its initial fixed-chart amplitude is \(O(1)\). A new scalar at each old home has amplitude \(C g_0(1+C_hg_0)^J\) in the homogeneous reference. The vacuum-subtracted endpoint has the additional factor \(L^{-4(J-k)}\|W^t-I\|^2\) with the fixed physical chart radius by (7.175). On the reflected cube \(\|W^t-I\|\le C|t|\). There are at most \(C L^{4(J-k)}\) old homes from the support at stage \(k\); summing all births gives \(C J g_0 t^2\). The same vacuum cancels at both endpoints because the physical marked roots, phase and reflected reference size are identical. The full actual comparison error is \(C L^{4J}J[e^{-c r}+\exp(CJ^2+C(1+P^2)r^4-c'b)]\), negligible relative to \(t^2\). Thus the direct classical lower contrast survives through the early statistical integrations on the stated genuine graphs.

This is a direction measurement for a specified action density with a fixed unamplified additive normalization. It is not yet the desired reflected lower bound. The test support has physical diameter \(O(aL^J)\), which tends to zero, and the assertion is a conditional contrast on selected target values. To obtain a fixed-separation reflected Gram one still needs the later \(K-J\) steps, a genuine positive-mass boundary event or transfer estimate, and matching to the normalized local operators at positive physical time. Ordinary variance alone cannot substitute for those steps.

### 4.138 Higher cumulants of the tight frustration rescaling (P/C on the same real margins and stated smooth profiles)

There is a simple real exponential bound for the ordinary/frustration difference on the original Wilson law. With the definitions of §2.3, for arbitrary bounded real bond weights and \(|t|\|f\|_\infty\le c_N\),
\[
 \log\mathbb E_\mu
   \exp\!\left[t\sum_b f_b(\beta|F_b|^2-\ell_b)\right]
        \le C t^2 \sum_b |f_b|^2 .
 \tag{REAL-TOTAL-FORCE-SQUARE}
\]
This uses no analytic smooth-source assumption. Color one orientation's links into finitely many classes so that no plaquette contains two members of a class; on the compatible even torus the usual transverse parity coloring suffices. Including the four orientations only changes the fixed class count. Conditional on all other links, the class links are independent and carry their true one-link Wilson densities. On each conditioned compact group the Hessian of its action has bounded norm, independently of the exterior. Haar integration of the vector field \(F_b |F_b|^{2m-2}\) gives
\[
 \beta\,\mathbb E(|F_b|^{2m}\mid{\rm out})
 \le C_N(2m-1)\mathbb E(|F_b|^{2m-2}\mid{\rm out}) .
\]
At \(m=1\) the equality before bounding the trace is \(\mathbb E(\beta |F_b|^2-\ell_b\mid{\rm out})=0\). Thus the conditional centered scalar has \(m\)-th absolute moment at most \(C_N^m m!\), since the local Casimir is bounded. Its centered one-link log is at most \(C t^2\) in a fixed interval. Multiply within one class, then use Hölder over the fixed number of classes in the original measure. This proves the claim, including its zero mean.

Write \(B_f=\sum_b f_b r_b\) for any fixed finite family of smooth physical profiles (link orientations can be declared separately). The real proof of §4.136 applies to bounded fixed coefficients in the frustration source, since all norms there are bounded by their absolute root envelopes. By (REAL-TOTAL-FORCE-SQUARE) and Hölder it therefore gives \(CV/\beta^2\) on a small fixed centered real interval for \(B_f/\beta\), on the same early native margins. For complex Cauchy require I-1 on the concrete joint finite family of smooth local loop/tensor-product action realizations of the profiles, with the linear oriented plaquette directions. Indeed \(r_b/\beta=D_b-\ell_b/(3\beta)\) is a fixed sum of contractions of such short plaquette words plus an identity and the indicated bounded coefficient on the linear action. Scalar analytic contacts cannot alter zeros. With these precise additive-profile discs, the centered joint log has one-sided real-part bound \(CV/\beta^2\) on a smaller polydisc, by taking \(\Re z_i\) in the real estimate. Cauchy after the one-sided analytic bound gives
\[
 \left|\kappa_m(c_\beta^{-1}a^2 B_{f_1},\ldots,
                         c_\beta^{-1}a^2 B_{f_m})\right|
       \le m!\,C_{\mathcal F}^{\,m}(a^2\beta)^{m-2},
       \qquad m\ge2 .
 \tag{TIGHT-H-GAUSSIAN-CUMULANTS}
\]
Here the profiles are chosen from the fixed finite family \(\mathcal F\), its radius is in \(C_{\mathcal F}\), the torus has fixed physical size \(V=O(a^{-4})\), and the convention factor \(c_\beta\) is bounded above and below. The variable in this formula is \(a^4 r_H\), the additional tightness rescaling, rather than the unscaled physical dimension-six source.

Along any subsequence on which its finite covariance matrix converges, the centered finite family of these rescaled insertions consequently converges in law to a centered Gaussian vector, possibly degenerate. For a fixed linear combination the generating log is analytic out to radius \(c/(a^2\beta)\) and the Taylor terms of order at least three at bounded arguments are \(O(a^2\beta)\) by the displayed factorial estimate; the quadratic coefficient converges by hypothesis. Equivalently apply the characteristic-function convergence criterion. The proof does not identify the limiting covariance as a contact distribution. In particular the reflected norm at fixed separated supports is an additional question even for this Gaussian family. Nor does this result extend the refuted fixed physical-polydisc claim to higher-degree composites.

### 4.139 The exact Ward component has positive white-noise covariance and vanishing reflected norm (P)

Consider the full Wilson trajectory under the elementary plaquette bound (FIRST), with fixed physical volume, \(\beta\to\infty\) and \(a\to0\). Put \(T_b=\beta|F_b|^2-\ell_b=3(r_b-h_b)\). For smooth real orientation-dependent weights define \(T_a(f)=a^2\sum_b f_b T_b\). Its joint finite-dimensional distributions converge to centered Gaussian white noise with covariance
\[
 C_{TT}(f,g)=2d_G\tau^2\int \sum_{\mu,\nu}f_\mu(x)g_\nu(x)
 \big[42{\bf1}_{\mu=\nu}+4{\bf1}_{\mu\ne\nu}\big]\,d^4x .
 \tag{WARD-WHITE-NOISE}
\]
Here \(d_G=N^2-1\), and \(\tau\) is the trace metric factor in the flat physical Hessian \(\tau d^*d\). In contrast, \(T_a(f)\) has zero reflected pairing with **every** observable on the opposite separated half of the original lattice, for every cutoff. This identifies a specific nonzero ordinary contact component in the equation-of-motion quotient. The proof uses neither a pressure disc nor high-order transport.

On the compact group define \(\Delta_b=\sum_A(X_b^A)^2\), with the metric convention of §2.3. Direct differentiation of the Wilson density and two Haar integrations by parts give the exact identity
\[
 \mathbb E[T_b\Phi]=\beta^{-1}\mathbb E[\Delta_b\Phi].
 \tag{WARD-LAPLACIAN-TEST}
\]
For a test independent of link \(b\) the right hand side vanishes identically. The same holds after centering, and with a reflected test separated from the marked bond. It also applies to any product of such opposite-half tests. Cumulants with one Ward insertion have only the local contacts obtained by differentiating the factors which actually use that bond.

Let \(K_{bc}=(X_b^A X_c^B S)_{AB}\) in left frames and \(K^i_{bc}\) the corresponding Hessian of \(S_i\). All derivatives up to any fixed order are bounded uniformly, with a fixed plaquette star. For \(b,c\) beyond that star the differentiated expressions below vanish exactly. The product rule yields
\[
 \beta^{-1}\Delta_b T_c=2\|K_{bc}\|_{\rm HS}^2+
 2\sum_B F_c^B \Delta_b F_c^B-\beta^{-1}\Delta_b\ell_c .
\]
The last two terms are \(O(\beta^{-1/2})\) in \(L^1\), by the local force bound and (FIRST). A tree gauge on a fixed cubical enlargement of this two-link star puts every link within \(C\sum_{p}\|I-U_p\|\) of the identity: the fixed chord loops fill by finitely many plaquettes in that cube. The squared Hessian norm is invariant under the separate endpoint frame rotations, including when \(b=c\). Bounded third derivatives and (FIRST) therefore put its \(L^1\) distance from its value at the identity at \(O(\beta^{-1/2})\), uniformly in position. This argument permits arbitrary global flux and all history sectors. In flat color coordinates the Hessian is \(\tau d^*d\) times color identity. For equal orientations its stencil has central coefficient six and six unit neighbor coefficients in the transverse directions. For unequal orientations its four entries have magnitude one. Summing their squares gives \(42\) and \(4\), respectively. Taking \(\Phi=T_c\) gives convergence of the covariance in (WARD-WHITE-NOISE), after the finite translation shifts in a smooth test and the periodic Riemann sum.

For Gaussianity take \(Y=T_a(f)\). In (WARD-LAPLACIAN-TEST) choose \(\Phi=e^{itY}\). The product-rule term containing \(it\Delta_bY\), multiplied by \(a^2f_b/\beta\) and summed, is \(it C_{TT}(f,f)\mathbb E e^{itY}+o(1)\) uniformly for bounded \(t\), by the preceding local \(L^1\) estimates. For the second term, \(\|\nabla_bY\|_{L^2}\le C_f a^2\sqrt\beta\), by the finite star and \(\|\nabla_bT_c\|_{L^2}\le C\sqrt\beta\). Consequently \(a^2\beta^{-1}\sum_b |f_b|\mathbb E|\nabla_bY|^2=O_f(a^2)\). For \(\varphi(t)=\mathbb E e^{itY}\) this gives \(\varphi'(t)=-t C_{TT}(f,f)\varphi(t)+o(1)\) on compact \(t\)-sets. Integrating from \(\varphi(0)=1\) gives the claimed scalar limit. Real linear combinations yield the joint limits. The orientation matrix is strictly positive, with least eigenvalue \(38\) before multiplication by \(2d_G\tau^2\).

There is also a joint conclusion for the remaining frustration row. Set \(H_a(g)=a^2\sum_c g_c(h_c-\mathbb E h_c)\). The identical product calculation gives
\[
 \beta^{-1}\Delta_b h_c =
 2\sum_i\|K^i_{bc}\|_{\rm HS}^2-\tfrac23\|K_{bc}\|_{\rm HS}^2
 +O_{L^1}(\beta^{-1/2}),\qquad
 \|\nabla_bh_c\|_{L^2}\le C\sqrt\beta .
\]
Define \(C_{TH}(f,g)\) by summing this displayed flat squared-Hessian stencil against \(f_\mu(x)g_\nu(x)\), over relative translations and the physical volume. It is a contact form. With \(\varphi_a(t,s)=\mathbb E\exp[itT_a(f)+isH_a(g)]\), the same Ward test gives uniformly on compact real \(s,t\)
\[
 \varphi_a(t,s)
 =e^{-t^2 C_{TT}(f,f)/2-ts C_{TH}(f,g)}
          \varphi_a(0,s)+o(1).
 \tag{WARD-JOINT-FACTOR}
\]
In particular on every tight joint subsequence one may subtract from \(H\) its projection \(T(C_{TT}^{-1}C_{TH}g)\), where the inverse is just the positive constant orientation matrix. The resulting limit is independent of the Ward white noise, by the joint characteristic function for all profiles. This statement needs no information about the law of that independent residual. Since \(T_b\) is exactly null in separated reflection tests, a positive ordinary local limiting variance alone cannot supply the physical reflected lower bound.

For the three plane matchings this contact matrix is explicit. At equal orientations each matching contributes \(2^2+1+1=6\) to its own squared stencil, hence \(18-42/3=4\) after the total-force subtraction. For unequal orientations just one matching contains that plane, giving \(4-4/3=8/3\). Thus \(C_{TH}\) has diagonal \(4\) and off-diagonal \(8/3\) times \(2d_G\tau^2\), with the spatial integral as in (WARD-WHITE-NOISE). The ordinary \(R_a=a^2r_g=H_a+T_a(g)/3\) after centering consequently has cross-matrix \(C_{TR}=C_{TH}+C_{TT}/3\), with entries \(18\) and \(4\) in the same units. Positivity of ordinary variance and the trial projection \(f=C_{TT}^{-1}C_{TR}g\) give without any tightness or smooth-pressure assumption
\[
 \liminf_{a\to0}\operatorname{Var} R_a(g)
 \ \ge\  (2d_G\tau^2)\int
  \left[\frac{30^2}{54}|g_{\parallel}(x)|^2+
              \frac{14^2}{38}|g_\perp(x)|^2\right]d^4x .
 \tag{ORDINARY-H-WARD-FLOOR}
\]
Here \(g_\parallel\) is the orthogonal projection of the four orientations on the all-ones line. Indeed use \(\operatorname{Var}R\ge 2\operatorname{Cov}(R,T)-\operatorname{Var}T\) at finite cutoff, and take the established limits of the two local terms by (WARD-LAPLACIAN-TEST). The normalization of the tight physical ordinary source adds \(c_\beta^{-2}\) to its variance. The measured component in this lower bound has exactly zero separated reflected norm, so it cannot count toward I-3(iii).

**Higher Ward cumulants on a growing complex disc.** The isolated Ward component permits a uniform analytic estimate without extending I-1. Fix a smooth \(f\), and write \(G_a(z)=\mathbb E e^{zT_a(f)}\), \(C_f=C_{TT}(f,f)\). On the present asymptotically free tori, \(G_a\) has no zero on \(|z|\le c_f\sqrt{\log\beta}\) for all sufficiently large \(\beta\). To prove this, first apply (REAL-TOTAL-FORCE-SQUARE) to \(a^2 f\). Then \(\mathbb E e^{2\Re(z)T_a(f)}\le e^{C_f' |z|^2}\) for \(2a^2|z|\|f\|_\infty\le c_N\). In the Ward exponential test use Cauchy–Schwarz with this bound. The local \(\beta^{-1}\Delta_bT_c-2\|K_{bc}(I)\|^2_{\rm HS}\) error is also \(O(\beta^{-1/2})\) in \(L^2\), by the same finite tree estimate and (FIRST). The one-link moment recursion in §4.138 gives \(\|\nabla_bT_c\|_{L^4}\le C\sqrt\beta\). For \(q_a=\beta^{-1/2}+a\), the finite smooth periodic Riemann error included, this yields
\[
 |G_a'(z)-z C_f G_a(z)|
 \le C_f'' (|z|+|z|^2)q_a\,e^{C_f''|z|^2}.
\]
Integrate the derivative of \(e^{-z^2 C_f/2}G_a(z)\) on a radial segment. Its distance from \(1\) on \(|z|\le R\) is bounded by \(C_f''q_a(1+R)^3e^{C_f'''R^2}\). Since \(a=O(\beta^{-1/2})\) on the logarithmic bare trajectory, a sufficiently small \(c_f>0\) gives distance less than \(1/2\) on the stated growing disc. In particular every fixed Ward cumulant of order greater than two tends to zero. On its concentric half-disc the analytic logarithm of the Gaussian-normalized factor is bounded by a constant, giving the sharper bound \(|\kappa_m(T_a(f))|\le m!(C_f''''/\sqrt{\log\beta})^m\) for \(m\ge3\). Finite families follow by polarization with uniform constants for unit linear combinations; for joint complex directions one can instead run the same radial interpolation with a complex linear combination of the real test profiles and bound its real exponential by (REAL-TOTAL-FORCE-SQUARE). The disc in this argument belongs only to the Ward difference. Its derivation makes no zero-free assertion about the remaining frustration source.

**Ward contact rows for compact local composite representatives.** Let \(P_{\alpha,x}\) be a finite family of fixed, smooth, real gauge-invariant functions on fixed contractible microscopic stencils, translated by \(x\). On \(SU(N)\) its first tangent jet at the identity is zero: each Lie-algebra slot of that jet is invariant under the global adjoint group, which has no invariant covector. Define
\[
 B_{\alpha,a}(g)=a^2\beta\sum_x g(x)(P_{\alpha,x}-\mathbb E P_{\alpha,x}).
\]
Then the joint characteristic factor (WARD-JOINT-FACTOR) holds with \(H_a\) replaced by any fixed linear combination of these variables. Its cross-form is
\[
 C_{T\alpha}(f,g)
 =\int\sum_\mu f_\mu(x)g(x)\sum_{b\parallel\mu}
                          (\Delta_bP_{\alpha,0})(I)\,d^4x .
 \tag{COMPACT-COMPOSITE-WARD-ROW}
\]
The inner sum is limited to the fixed stencil at a representative root. Indeed its compact tree gauge puts \(|\nabla_b P_\alpha|\) within \(C\sum_p\|I-U_p\|\) of zero, hence \(\|\nabla_b B_{\alpha,a}\|_{L^2}\le C_g a^2\sqrt\beta\). Its bounded Lipschitz Laplacian tends in \(L^1\) to the displayed identity value, by (FIRST). These are exactly the two estimates used for (WARD-JOINT-FACTOR). This finite family need not possess its own complex disc. Along any tight joint subsequence the residuals after projecting out the explicit Ward rows are jointly independent of the Ward noise. For a quartic vacuum jet the Ward row here vanishes. The factor \(a^2\beta\) is part of this statement: these are fluctuation-scale projections of fixed microscopic representatives, not uniform estimates for arbitrary physical renormalized fields.

For \(P_{\mu\nu,x}=s_{\mu\nu,x}\) each of its four incident bonds contributes \(d_G\tau\) to the flat Laplacian. Thus the oriented action row has cross-form \(2d_G\tau\int(f_\mu+f_\nu)g\). The scalar Wilson action summed over all six planes has cross-vector \((6d_G\tau,\ldots,6d_G\tau)\) multiplying \(g\). Projecting against (WARD-WHITE-NOISE) gives
\[
 \liminf_{a\to0}\operatorname{Var}
 \left(a^2\beta\sum_{x,\mu<\nu} g(x)s_{\mu\nu,x}\right)
       \ge {4d_G\over3}\int |g(x)|^2\,d^4x .
 \tag{SCALAR-ACTION-WARD-FLOOR}
\]
This is an ordinary lower bound in the full compact theory. The trial Ward profile is \(f_\mu=g/(18\tau)\) for each orientation. Its exact separated reflected norm is zero in every finite-cutoff physical action pairing. The nonzero stopped-scale action contrast in §4.137 must therefore be transported in the complementary physical sector to obtain a fixed positive-time bound.

### 4.140 Fixed physical intermediate scale: actual mass and classical contrast (P/L under the original weak stopping convention)

Let \(d\ge0\) be fixed, \(k=K-d\), and \(s=L^{-d}\ell_0\). Thus the retained mesh \(s\), the number \(v_s=(t^*/s)^4\) of retained sites, and the distance of a chosen positive-time slab from both reflection planes are independent of \(a\). Work at a fixed weak stopped coupling \(g_K=g_*>0\) (or in a compact subinterval of the weak regime). I-0c over the last \(d\) steps puts \(g_k\) in another compact subinterval. Take compatible original regional grids. Write \(\mu^{\rm nat}_{a,k}\) for the normalized, source-free marginal in the actual retained variables of the first \(k\) operations on the reference torus. Vacuum scalar factors cancel in this single marginal.

There is a radius \(r_s>0\), fixed independently of \(K\), such that every Haar-measurable subset \(E\) of the product link ball \(\mathcal C_s=\{\max_e\|W_e-I\|<r_s\}\) satisfies
\[
 \mu^{\rm nat}_{a,k}(E)\ \ge\ e^{-C(g_*,d)v_s}\,{\rm Haar}(E).
 \tag{FIXED-CYLINDER-MASS}
\]
Indeed the primary pointwise (0.1) bounds the **same** bare-scalar-normalized density above by \(e^{E_+v_s}\), and below by \(\chi_k e^{-g_k^{-2}A(U_k)-E_-v_s}\). The selector in CMP119 (2.16),(2.17) tests local regional minimizing-field plaquettes, with threshold \(\epsilon_k\eta^2,\ \eta=L^{-k}\). T1 Proposition 7.152 checks the global and all the synthetic regional simple-lift configurations on this ball: their local plaquette defects are bounded by \(C r_s\eta^2\), with the same complete native determining stencils. Decrease \(r_s\) uniformly over the indicated compact coupling interval so this lies below the selector threshold. Summing squared plaquette defects on the global regular field gives \(A(U_k)\le Cr_s^2 v_s\); the number of fine plaquettes is \(6\eta^{-4}v_s\). Integrate the lower bound over \(E\), divide by the integral of the upper bound, using normalized product Haar. This proves (FIXED-CYLINDER-MASS), including when some earlier histories healed. The estimate holds for the complete density at this scale; it does not select a history in which every fine plaquette was small. Bałaban, LFR II, pp.355–356, (0.1); CMP119, pp.257,263–265.

Fix a spatial plaquette in the positive slab and choose a smooth nonnegative positive-time test \(f\), at a fixed physical time and equal to one on all its descendants as in §4.54. Choose \(0<u<r_s/8\); at \(W^u\) only one of that plaquette's links is \(e^{uT}\) for a fixed nonzero Cartan generator. Its energy is at least \(c u^2\). Let \(E_u,E_0\) be full product balls of radius \(\delta\) about \(W^u,I\). For any fixed sufficiently small \(\delta\ll u\) they have fixed positive Haar measure in \(\mathcal C_s\). On \(E_u\), reduce \(\delta\) so the chosen plaquette has energy at least \(c u^2/2\). The actual regular minimizing-field diagnostic \(D_s(W)=g_k^{-2}S_f(U_k(W))\) then satisfies \(D_s(W)\ge c_s g_k^{-2}u^2\) on \(E_u\) by (LOCAL-CLASSICAL-ENERGY). On \(E_0\), the global regularity bound just used with \(r_s=\delta\) gives \(0\le D_s(W)\le C_sg_k^{-2}\delta^2\). With \(\delta\) chosen still smaller the two ranges are separated by \(c_s' g_k^{-2}u^2\) uniformly in \(K\). Thus two windows of the **actual fixed-scale retained law** have uniform mass and distinguish this classical diagnostic. This upgrades the shrinking support of §4.137 for the classical term only.

There are two independent obstructions to turning these facts into a reflected estimate. First, \(D_s(W)\) is the minimizing-field evaluation and the target row is the actual normalized conditional mean of the fine quantum insertion. Their vacuum-subtracted difference includes derivatives of the fluctuation density, inherited effective action and history normalizations. An actual derivative test for a stopped window would be \(\partial_z\log[\Pr_z(E_u)/\Pr_z(E_0)]_{z=0}\) with the positive-time fine source held fixed. Formula (0.1) at zero source does not control that derivative. Second, even an exact contrast on two **full** stopped windows is an ordinary contrast: the windows include positive and negative variables. Already at its flat first derivative the original four-dimensional spatial-link average on a reflection plane contains translated spatial lines on off-plane time layers, as (COCHAIN-WILSON-ENERGY) verifies explicitly. Consequently its plane coordinate is not measurable in the original reflection-plane algebra. On rough histories an R operation may also reinstall fields. A gauge-invariant positive-half fine observable in (BOUNDARY) requires an actual half-supported testing variable or the true microscopic boundary marginal. Neither issue is resolved by the lower bound on the complete stopped cylinder. In particular (0.1) also admits constant density as far as this scalar comparison alone is concerned, which illustrates why it gives no separated signs. This observation is about the information in the inequality, not a claim that the Wilson law has constant density.

### 4.141 A physical boundary witness with uniform mass and vanishing contrast (P for the full Wilson law)

Consider the genuine microscopic spatial links \(B\) on a reflection plane. Embed a fixed physical cubical spatial graph with edge length \(s>0\) on that plane, using compatible nearest lattice paths (straight edges and disjoint interiors). Retain the ordered product \(Y_e(B)\in SU(N)\) on each long edge, with one orientation chosen per undirected edge. Its graph and physical placement stay fixed as \(a\to0\). For any measurable event \(E\) of these products and any integrable observable \(A\) on a separated time slab the full Wilson law satisfies
\[
 \begin{split}
 |\Pr(Y\in E)-{\rm Haar}^{\otimes m}(E)|&\le \varepsilon_a,\\
 |\operatorname{Cov}(1_{\{Y\in E\}},A)|&\le
          2\varepsilon_a\,\mathbb E|A-\mathbb E A|,\\
 \varepsilon_a&=C_{s,m}(1+\beta)^{d_G/2}
             \exp[-c_s/(a(1+\beta)^2)] .
 \end{split}
 \tag{STRAIGHT-BOUNDARY-HOLONOMY}
\]
In four dimensions \(\beta=O(\log(1/a))\) makes this error smaller than every fixed power of \(a\). This result supplies genuinely plane-measurable physical windows of uniformly positive mass and tests their separated conditional contrast on the original law.

On the central third of each retained edge choose \(M\ge c_s/a\) fine links. Collinear links on the same line never lie together on a plaquette. The selected central thirds of distinct edges are separated by more than one fine step. Thus each plaquette contains at most one selected link. Given all other links, the selected ones are independent and each has normalized Haar density \(p(u)\propto\exp[\beta\Re\operatorname{Tr}(uK)]\) up to orientation, with a bounded staple matrix \(K\). In particular \(|\log p(vu)-\log p(u)|\le C_N\beta\|v-I\|\). A Haar ball of radius \(r=(1+\beta)^{-1}\) about a maximizer has measure at least \(c_N r^{d_G}\); normalization gives \(\|p\|_2\le C_N r^{-d_G/2}\).

Let \(h_{r^2}\) be the central heat probability at time \(r^2\) for the bi-invariant metric, generator \(\Delta/2\). The Lipschitz estimate implies \(h_{r^2}*p\le C_N p\): indeed \(\int e^{C_N\beta\|v-I\|}h_{r^2}(v)\,dv\le C_N'\). To verify the last bound, run the matrix Brownian motion \(dV=\sum_A T_AV\,dB^A+\tfrac12\sum_A T_A^2V\,dt\) from \(I\). Its drift entries are bounded, and the quadratic variation of each real or imaginary matrix-entry martingale is at most \(C_N t\) because \(V\) is unitary. The scalar exponential martingale inequality and a finite sum over entries give the required uniform exponential moment at \(t=r^2\). Choose \(0<c<1\) so \(p=c\,h_{r^2}*p+(1-c)p'\) with \(p'\) another probability density. On any nontrivial irreducible representation with positive Casimir \(\lambda\), the heat multiplier is \(e^{-r^2\lambda/2}I\). The smallest such \(\lambda\) has a positive lower bound (the first positive eigenvalue of the compact connected group Laplacian). Since a probability multiplier has operator norm at most one, this gives
\[
 \|\widehat p(\pi)\|_{\rm op}
 \le {1-c\over 1-c e^{-r^2\lambda/2}}\le1-c_N' r^2 .
\]
The bound is uniform in the staple, and is invariant under inversion, orientation and fixed left or right endpoint factors.

Conditional on the unselected links, one edge product is a convolution of \(M\) such independent laws with fixed group factors. On every nontrivial Peter–Weyl summand the remaining \(M-1\) contractions multiply the Hilbert–Schmidt norm of the first multiplier by at most \((1-c_N'r^2)^{M-1}\). The Haar Plancherel identity and the preceding \(\|p\|_2\) estimate give \(L^2\), hence total variation, distance to Haar at most \(C_Nr^{-d_G/2}e^{-c_N'Mr^2}\). Distinct edge products are conditionally independent. Summing their fixed number of total-variation distances proves the first line even conditional on the whole unselected exterior. The separated \(A\) is measurable in that exterior; use the same conditional estimate after subtracting the mean of \(A\). This proves (STRAIGHT-BOUNDARY-HOLONOMY).

In particular for any two fixed positive-Haar neighborhoods \(E_i\), both \(\Pr(Y\in E_i)\) stay bounded below and \(\mathbb E[A\mid Y\in E_i]-\mathbb E A\to0\) for every physical local action test whose centered \(L^1\) norm grows at most polynomially in \(1/a\), including the bare smooth action. Subtracting the exactly reflection-null Ward component does not alter this conclusion. Here loss of contrast occurs on a bona fide full-law boundary readout, even though the windows have positive mass and the smearings are at fixed physical separation. It excludes straight coarse products with any bounded reweighting; it leaves open a boundary variable that smooths its links at each scale or a true low-energy transfer overlap.

In fact the entire conditional-mean projection on these plane products vanishes at this rate. Reserve one independent link density at each end of a long product. Haar Young's inequality \(\|u*v\|_\infty\le\|u\|_2\|v\|_2\), applied to the nonconstant parts with the remaining contractions between them, bounds its conditional density difference from \(1\) pointwise by \(C_Nr^{-d_G}e^{-c_N'Mr^2}\). This uses the same uniform \(\|p\|_2\) estimate for both end factors. Multiplying the fixed number of such densities gives \(|p(Y=y\mid{\rm unselected})-1|\le\delta_a=C_{s,m}r^{-d_G}e^{-c_s r^2/a}\) uniformly. The marginal density is at least \(1-\delta_a\) for small \(a\). Bayes' identity gives
\[
 \|\mathbb E[A\mid Y]-\mathbb E A\|_\infty
 \le {\delta_a\over1-\delta_a}\mathbb E|A-\mathbb EA|.
 \tag{STRAIGHT-BOUNDARY-PROJECTION}
\]
Thus all centered \(L^2\)-normalized functions of this fixed physical boundary graph, including rare-event tests with cutoff-dependent weights, give vanishing overlap. If the reference-torus reflected form has a positive limit, its conditional mean in (BOUNDARY) must retain information outside this complete straight-graph sigma algebra. The conclusion does not require a bound on the uniform fine-field transfer gap.

### 4.142 A fixed physical spatial heat test on the actual reflection plane (P)

A natural plane-measurable test is to smooth adjoint curvature using the spatial covariant heat semigroup of the *raw* Wilson links. For this particular smoothing there is an additional obstruction. On one fine reflection plane let \(H_{\rm sp}=\sum_{j=1}^3(2-T_j-T_j^*)\), with \(T_j\) the adjoint parallel shift. For each fixed positive physical \(t\) and every \(q<\infty\), on the logarithmic trajectory and fixed physical torus,
\[
 \mathbb E_{\mu_a}\operatorname{Tr}\exp[-tH_{\rm sp}/a^2]
          \le C_{q,t} a^q .
 \tag{RAW-PLANE-HEAT}
\]
The expectation uses the entire four-dimensional Wilson law. This estimate concerns transport in the colored representation of the unmodified fine spatial connection; it imposes no gap on physical singlets.

Here are the dimensional details supplementing §4.110. Set \(P=I-H_{\rm sp}/12\), a positive semidefinite contraction. Its diagonal walk kernel is a scalar lazy three-dimensional bridge multiplied by the ordered parallel transports. For \(m\asymp n^2\), where \(n=t^*/a\), the scalar bound is \(p_j(x)\le C[(1+j)^{-3/2}+n^{-3}]\), with matching lower bound at zero by Fourier summation. Split the unconditioned walk into \(B\asymp m^{1/8}\) independent chunks of length \(L'\asymp m^{7/8}\). Within each chunk a positive fraction of edges are traversed exactly once with probability at least a fixed positive constant: three-dimensional transience gives a positive probability to avoid a specified traversed edge in each direction of time, and the torus correction after \(J_0\) early steps is \(C J_0^{-1/2}+CL'/n^3\). A binomial estimate makes the total number of internally single edges at least \(cm\) except with probability \(e^{-cB}\).

For two different chunks the \(p\)-norm of their common vertex visits is at most \(Cp^2(\sqrt{L'}+(L')^2/n^3)\le C'p^2\sqrt{L'}\), uniformly in their displacement. Indeed the ordered-time moment calculation in §4.110 uses the squared \(L^2\) norm of \(G_{L'}=\sum_{j\le CL'}p_j\), now bounded by \(C(\sqrt{L'}+(L')^2/n^3)\) from the three-dimensional return estimate. Use reversed increments for the earlier chunk. By Minkowski all chunk-pair intersections have \(p\)-norm at most \(Cp^2B^2\sqrt{L'}\). With \(p\asymp m^{1/8}\) this is \(O(m^{15/16})\). Markov's inequality shows that fewer than \(cm/2\) of the counted steps are lost to other chunks except with probability \(Ce^{-c m^{1/8}}\) (change the fixed \(c\) when counting endpoints). Conditioning the trajectory on its return costs at most \(Cp_m(0)^{-1}\le C'm^{3/2}\), absorbed into the exponential. Thus, except for this small fraction of bridges, at least \(c m\) edges are traversed only once in the whole walk.

Select a fixed fraction of those edges so none share a four-dimensional plaquette, and condition on all other Wilson links. The adjoint has no invariant vector. Independence and the one-link contraction in §4.141 bound the expected path multiplier by \(Ce^{-cm/(1+\beta)^2}\); on the remaining bridges its norm is at most one. Hence
\[
 n^{-3}\mathbb E\operatorname{Tr}P^m
 \le C p_m(0)[e^{-c m/(1+\beta)^2}+e^{-cm^{1/8}}],
 \qquad c_t n^2\le m\le C_t n^2 .
\]
The desired heat operator is the average of \(P^m\) at Poisson mean \(12t/a^2\). The probability outside such a fixed-factor window is \(O(e^{-c_t n^2})\), where the elementary trace bound \(d_G n^3\) suffices. Multiplying the preceding bound by \(n^3\) proves (RAW-PLANE-HEAT).

For example if a boundary curvature vector \(J_a\), even one depending on those same links, has deterministic \(\|J_a\|_2\le a^{-C}\), then \(\langle J_a,e^{-tH_{\rm sp}/a^2}J_a\rangle\) and every fixed polynomial rescaling thereof converge to zero in \(L^2\), by positivity, the trace bound and \(0\le e^{-tH_{\rm sp}/a^2}\le I\). This includes an actual covariant curvature probe on the correct time plane at a fixed physical smoothing radius. The difficulty is in its transport with the raw colored field. Spatial smoothing that simultaneously changes the transporting connection at successive scales is a different construction and is not covered by (RAW-PLANE-HEAT).

### 4.143 A bounded true-plane test and its fixed-scale Gaussian overlap (P for support and reference calculation; O for its Wilson overlap)

There is a plane test outside the two classes in §§4.141–4.142. On the original time-zero spatial links iterate only the **three-dimensional** version of the group block average to fixed physical spatial mesh \(s=L^k a\). Each step uses the native centered paths with their endpoints in the three-dimensional spatial blocks. Define a Borel equivariant extension when the average logarithm is outside its compact admissible chart, by using the straight center-to-center transport on that bond. The failure flag may be kept. This operation is offered as a test function of the microscopic reflection-plane links only; it does not replace any transformation or density in the four-dimensional Wilson law. At the final spatial mesh parallel-transport each \(12\)-plaquette curl \(C_N(W_{12})\) to one root by a fixed coarse spatial tree, and take a normalized real transverse cosine mode with momentum \((2\pi/N_s,0,0)\), \(N_s=t^*/s\). Square its invariant color norm and denote the resulting random variable by \(\Psi_a(B)\). A coarse site gauge changes the common root frame by one adjoint rotation. Thus \(\Psi_a\) is gauge invariant, measurable on the genuine microscopic plane, and bounded by a constant depending only on the fixed spatial grid and \(G\). The root transports in this definition use the *nonlinearly averaged* spatial links, not microscopic straight-edge products. At the identity they affect the curl only beyond its first jet.

For clarity compute the actual tangent overlap in the periodic fine Gaussian of §4.35. Write \(h=s/a,\ n=hN_s,\ k_0=2\pi/N_s,\ q=k_0/h\), and \(D_h(p)=h^{-1}\sum_{j=0}^{h-1}e^{ijp}\) up to the centered unit phase. Let \(Y\) be one color's linearized real mode on the plane; its second-jet square is the corresponding term of \(\Psi_a\). The curl kills endpoint frame gradients as in §4.134, now in three dimensions and without any temporal averaging. The \(h^2\) fine square flux has a spatial block average and a rectangle average in axes \(1,2\). For its normalized spatial mode, the transverse aliases in directions \(2,3\) vanish, and an alias \(q_r=(k_0+2\pi r)/h\) in direction one has coefficient of modulus \(\sqrt h\,|D_h(q_r)|^2\) on the normalized original spatial \(12\)-curl mode \(Z_0(q_r)\). This follows by multiplying the \(h^2\) flux by the \(h^{-3/2}\) spatial Fourier normalization and the two normalized direction-one averages. The centered real cosine, or its unit-norm phase-rotated partner, can be used throughout.

For the base alias at time \(m\), the periodic free curl covariance is \(\tau^{-1}|\widehat q|^2 G_{n,\omega}(m)\) in the notation of §4.35. Its modulus at fixed physical time is bounded below by \(c/h\), since \(|\widehat q|\asymp h^{-1}\), \(G_{n,\omega}(m)\ge c_s h\) and \(|D_h(q)|\ge 2/\pi\). Hence the squared cross-covariance of \(Y\) with the base fine mode (summing its two real components if a phase is present) is at least \(c/h\). Also \(\operatorname{Var}Y\le C\) uniformly: with the wrapped alias index \(j_r\) of least magnitude, \(h|\widehat q_r|\le C(1+|j_r|)\), \(|D_h(q_r)|\le C/(1+|j_r|)\), and \(|\widehat q_r|^2G_{n,\omega_r}(0)\le C|\widehat q_r|\). The variance sum is bounded by \(C\sum_j(1+|j|)^{-3}\). This verifies a plane-supported test at one time slice, where the temporal smoothing used in §4.35 is unavailable.

Choose a single nonnegative smooth \(f\) spatially constant and bounded below on a closed physical time interval strictly inside the positive half. The centered positive action in the fine Gaussian contains the spatial sum of \(12\)-curl squares on at least \(c_f h\) time layers. Parseval and Gaussian contraction give twice the sum of squared cross-covariances, all nonnegative. Retaining the base alias just computed and summing those layers shows, in canonical action units,
\[
 \operatorname{Cov}_{G}
  \left(\sum_{m,x,\alpha<\gamma} f(am)|dA_{\alpha\gamma}(m,x)|^2,
                 \sum_A |Y^A|^2\right)\ \ge\ c_{s,f}>0 .
 \tag{TRUE-PLANE-GAUSSIAN-OVERLAP}
\]
Both the time support and the spatial mesh are fixed independently of \(a\).

For the full Wilson law let \(A_a\) be the proposed physical action smearing in these units after operator matching, with any justified Ward row removed. Since \(\Psi_a\) is bounded and belongs to the true boundary algebra, (BOUNDARY) and ordinary Cauchy–Schwarz give
\[
 G^\theta_a(A_a,A_a)\ \ge\
       |\operatorname{Cov}_{\mu_a}(A_a,\Psi_a)|^2/
                          \operatorname{Var}_{\mu_a}\Psi_a
\]
when the denominator is positive. The Ward row has zero pairing exactly because the fine supports are separated. An absolute Wilson cross-error less than half the properly normalized overlap in (TRUE-PLANE-GAUSSIAN-OVERLAP) would suffice. Unlike the genuine four-dimensional \(W_k\), this test is already in the correct plane algebra, with no terminal flag or puncture to reinterpret. The required quantity is the signed mixed derivative of the actual fine action and this one bounded spatial test. The original I-0c and I-1 do not give the spatial-only nonlinear readout comparison or a lower bound on that derivative. Its Gaussian tangent and the positive terminal mass cannot be substituted for it. This is a concrete unresolved contrast for an admissible physical alternative after (STRAIGHT-BOUNDARY-PROJECTION) and (RAW-PLANE-HEAT).

**Actual early segment of this spatial test.** The nonlinear plane map can be controlled on a growing number of its *own* steps in the full law; importing I-2 for it would be unjustified. Let \(A_L\ge2\) dominate the supremum derivative of one spatial block-link map and its quadratic Taylor remainder coefficient on a fixed small identity chart. It is finite, since this single map uses a bounded number of fixed-length group words, their local logarithms and one exponential. Fix \(\gamma>0\) with \(2\gamma(1+\log_L A_L)<1/2\). For \(j\le\gamma\log_L\beta\), a fixed early output link or plaquette and all of its ancestors fit inside a contractible spatial box of side \(C_Lr\) fine sites, \(r=L^j\). Take \(P=\log(2+\beta)\). By (MARKED-EXP) and a union bound, with probability \(1-O(r^3e^{-cP^2})\) every fine plaquette in that box has \(\|I-U_p\|\le P/\sqrt\beta\) (fixed constants allowed). This uses the original four-dimensional Wilson law on the genuine plane.

In a coordinate tree gauge on the box each fine link then obeys \(\|\log U_e\|\le y_0=C_L rP/\sqrt\beta\). Moving a tree path by one lattice edge fills at most \(C_Lr\) plaquettes, with bounded multiplicity. In this fixed gauge write \(A=\log U\) and let \(w_i\) denote the actual recursively blocked logarithms on the nested stencil. While in the chart, \(\|w_i\|_\infty\le A_L^i y_0\); the last bound tends to zero even at \(i=j\), so no chart fallback is used there. For the linearized plane map \(Q_1^{(3)}\), successive Taylor estimates give
\[
 \|w_j-(Q_1^{(3)})^jA\|_\infty
     \le C_L A_L^{2j}y_0^2,\qquad
 \sqrt\beta\,C_L A_L^{2j}y_0^2=o(1).
 \tag{EARLY-TRUE-PLANE-TANGENT}
\]
Indeed the error recursion is \(e_{i+1}\le A_L e_i+C_L(A_L^i y_0)^2\). The same bound applies to the difference between the true final compact curl and the linear curl on the right, by one last finite plaquette Taylor formula. The failure probability is smaller than every inverse power of \(\beta\), uniformly for the stated root. This is a genuine Wilson comparison with a linear function of its **own** fine links in a local tree frame. It neither makes those links Gaussian nor compares the entire positive-time mixed derivative. At a fixed mesh \(s\) the remaining \(k-j\) steps grow without bound; the above small-chart argument on raw plane data cannot be continued by replacing \(r\) with \(s/a\). The new observable would need renormalized spatial-step control there. This locates the missing input in an actual half-supported test rather than in an assumed identification of the four-dimensional terminal plane with \(B\).

### 4.144 The normalized source derivative on the true spatial annuli (P)

Take a fixed periodic \(0\le f\le1\) depending only on physical time, supported in \((3t^*/16,5t^*/16)\), equal to one on \([7t^*/32,9t^*/32]\). Put \(A=\beta_a\sum_p f(t_p)s_p\). This convention tests the canonical action: the perturbed Wilson plaquette coefficient is \(\beta_a(1-z f(t_p))\) under the additive weight \(e^{zA}\), not \(\beta_a+z\). A final physical triangular action normalization multiplies this row by its actual coefficient and adds any genuine lower rows. No normalization or positivity of that coefficient follows from the source identity. The centered Ward difference has exactly zero correlation with any function of the time-zero plane, by (WARD-LAPLACIAN-TEST); strictly local scalar contacts have disjoint arguments. The physical interval in \(f\) stays fixed as \(a\to0\).

Let \(W_0\) be all fine spatial links at time zero, \(W_j\) their genuine three-dimensional recursive blockings with the extension of §4.143, \(\mathcal F_j=\sigma(W_j)\), and \(\pi_j(W_j)=W_{j+1}\). Write \(\nu_{j,z}\) for the marginal under \(e^{zA}d\mu/\mathbb E e^{zA}\). In finite volume the following identities hold for every \(j\), including all failed charts:
\[
 {d\nu_{j,z}\over d\nu_{j,0}}
     ={ \mathbb E[e^{zA}\mid\mathcal F_j]\over \mathbb E e^{zA}},
 \qquad S_j=\left.\partial_z\log {d\nu_{j,z}\over d\nu_{j,0}}\right|_0
        =\mathbb E[A\mid\mathcal F_j]-\mathbb EA,\qquad
 S_{j+1}=\mathbb E[S_j\mid\mathcal F_{j+1}].
 \tag{PLANE-ANNULUS-SCORE}
\]
Here \(S_j\) denotes this score only, not a component of the Wilson action. Pushforward and differentiation of a bounded window test prove the identities without any smoothness of the spatial block map or a common reference-coordinate density. The normalized derivative of the intervening conditional kernel is \(S_j-S_{j+1}\); it has zero pairing with every function of the final plane field, not an independent positive contribution at each step.

For the same physical low spatial frequency define \(\Psi_j\) by the tree-transported mode-square prescription of §4.143 on the \(j\)-grid, using any declared deterministic normalization. Then
\[
 \operatorname{Cov}(A,\Psi_k)-\operatorname{Cov}(A,\Psi_J)
 =\sum_{i=J}^{k-1}
     \mathbb E\!\left[S_i\big(\Psi_{i+1}(\pi_i W_i)-\Psi_i(W_i)\big)\right].
 \tag{SIGNED-PLANE-ANNULI}
\]
If only the final \(\Psi_k\) is used, its covariance is exactly its pairing with the conditional score at every earlier step, with the whole composite pulled back there. These formulas use neither four-dimensional terminal Haar windows nor a substitution of a classical minimum for a conditional mean. The terms on the right of (SIGNED-PLANE-ANNULI) can have either sign. The next estimate tests the long tree paths in precisely this recursion.

### 4.145 Nonlinear early spatial blocks lose their long colored cross term in the actual mixed covariance (P)

Use \(\beta=O(\log n)\), the tori and (MARKED-EXP) of §4.22, \(h=L^j\le\beta^\gamma\), where \(\gamma\) satisfies the strict margin of (EARLY-TRUE-PLANE-TANGENT). Let \(P_{xy}^{(j)}\) be the product along the simple coarse tree path between the roots of two coarse magnetic curls \(J_x=C_N(W_{j,\partial p_x})\), \(J_y=C_N(W_{j,\partial p_y})\), with \(M\) edges. A part of the squared cosine mode has exactly this form, since the common initial parts of the root paths cancel. For \(M\) larger than a fixed constant, the full Wilson measure obeys
\[
 \left|\operatorname{Cov}_{\mu}
  \big(A,\langle J_x,\operatorname{Ad}(P_{xy}^{(j)})J_y\rangle\big)\right|
 \le C_N\|A-\mathbb EA\|_\infty
       \left[e^{-c M/((1+\beta)^2h^4)}
                      +e^{-cM\log^2(2+\beta)}\right] .
 \tag{EARLY-NONLINEAR-PLANE-TRANSPORT}
\]
The same proof applies to any separated bounded bulk test, and the action just fixed has norm \(O(\beta n^4)\). The estimate covers the sign and all field sectors. It is substantially stronger than a tangent estimate on one small block.

Choose a positive fraction of path edges with disjoint determining cubes and their one-step collars, away from the two end plaquettes. This is possible by a bounded-degree greedy selection since the tree path is simple. In the common face of the two endpoint \(h\)-blocks of each chosen edge choose one fine crossing link. Internal frame paths in any one of those two blocks do not use a crossing link. Only the one final coarse bond through that face sees that link: at the previous level only the crossing bond in its own transverse subblock sees it, and one iterates this observation. The determining stencil of any other final spatial edge either lies on one side of this face or crosses a different face. This uses the actual centered spatial average, with its straight translated middle segments and frame connectors contained in the endpoint blocks. Thus the chosen variables affect neither endpoint curl nor any other coarse path edge. Given all other fine links, these chosen fine links are independent, with their true one-link Wilson densities as in §4.141.

For one chosen link let \(G_i\) be the event that all fine plaquette defects on its determining cube and collar are at most \(P/\sqrt\beta\), \(P=\log(2+\beta)\). Use a local tree frame of that good configuration and keep that frame fixed for a small subsequent perturbation. In this frame all fine links have size \(y_0\le C hP/\sqrt\beta\) and all successively blocked links have size \(y_l\le A_L^l y_0\). A left perturbation \(u\mapsto e^{rX}u\) of that fine slot with \(r=(1+\beta)^{-1}\), \(\|X\|\le1\), changes the fine chart bound only by \(O(r)\). It need not preserve the particular plaquette threshold, but the enlarged charts for the derivative still hold, without differentiating a failure flag.

At identity, the left derivative of one spatial blocking step in a single crossing slot is \(\alpha I,\ \alpha=L^{-2}\), after orienting the step in the path direction. Exactly \(L\) of the \(L^3\) translated straight segments traverse that slot, once; all the within-block connectors avoid it. The derivative of the group average at the identity is its arithmetic tangent average. At a nonidentity input with all links of size \(y_l\), the ordinary analytic finite-block map changes this derivative by at most \(C_L y_l\) in left-trivialized frames. Only its unique crossing descendant is perturbed. Composing those derivatives gives \(h^{-2}(I+E)\), \(\|E\|\le \exp[C_L\sum_{l<j}y_l]-1=o(1)\), along the entire fine-slot perturbation; at \(j=0\) the derivative is identity. Orientation reversal at a selected edge uses its inverse and the corresponding unitary frame rotation. The bound is uniform on each actual \(G_i\). In particular it is the product of relative errors along one descendant, rather than an additive error compared with the possibly tiny \(h^{-2}\).

Write \(U_i(u)=\operatorname{Ad}(W_{j,e_i}(u))\), or its inverse for the opposite orientation, and let \(\bar U_i=\mathbb E(U_i\mid {\rm out})\) with all unchosen links fixed. Suppose \(\Pr(G_i\mid{\rm out})\ge1/2\). For every unit adjoint vector \(v\) the conditional variance of \(U_i(u)v\) is \(1-\|\bar U_i v\|^2\). The conditional one-link log density is \(C_N\beta\)-Lipschitz, so left rotation through \(rX\) has uniformly bounded density ratio. Use an isotropic \(X\) in a unit ball in the Lie algebra. The average squared displacement \(\mathbb E_{u,X}\|U_i(e^{rX}u)v-U_i(u)v\|^2\) is bounded **above** by a constant times that variance, by subtracting its conditional mean in both terms. It is bounded **below** by \(c_N r^2 h^{-4}\) by restricting \(u\) to \(G_i\): the preceding derivative, integrated along the short rotation, is \(rh^{-2}\,d\operatorname{Ad}(X)\) up to frame rotations and relative \(o(1)\) operator error in the good frame. The quadratic Casimir is strictly positive on the adjoint. A gauge selected at \(u\) only rotates the isotropic directions in this pointwise lower estimate; the domination of the shifted marginal is applied to the original isotropic independent \(X\). This proves \(\|\bar U_i\|_{\rm op}\le 1-c_Nr^2h^{-4}\) for such outside data.

It also costs exponentially to have many slots with \(\Pr(G_i\mid{\rm out})<1/2\). For distinct selected stencils, \(\Pr(\bigcap_{i\in I}G_i^c)\le (C h^3e^{-cP^2})^{|I|}\): choose a bad fine spatial plaquette in each of the disjoint stencils and apply (MARKED-EXP) to that set. Given the unselected links the \(G_i\) are independent since each depends only on its own remaining slot. For \(b_i=\Pr(G_i^c\mid{\rm out})\), \(\mathbb E\prod_{i\in I}b_i=\Pr(\bigcap_{i\in I}G_i^c)\). Counting subsets with at least half of the selected \(b_i>1/2\) now costs at most \(e^{-cMP^2}\), including the binomial entropy. On all other outside configurations the conditional path expectation is the ordered product of at least \(c M\) contracting matrices with unitary factors. The separated \(A\) and the endpoint curls are fixed in this conditioning. Combining the two regions proves (EARLY-NONLINEAR-PLANE-TRANSPORT).

In fine units the observed range is at most \(C h(1+\beta)^2h^4\log n\) for this estimate with any fixed desired inverse power of \(n\), choosing \(C\) accordingly. Its physical size tends to zero uniformly through the stated early window. Even after summing polynomially many pairs and multiplying by polynomial normalization, all pairs with a fixed positive physical separation have vanishing covariance with \(A\). Near-diagonal scalar plane contributions and covariance created by later spatial reblocking are not estimated by this open-path contraction.

**A strictly signed failure of an early Gaussian comparison.** Take two small disjoint spatial balls at fixed positive distance on the time-zero plane, close enough that the chosen cosine has the same positive sign on both. Restrict the two factors in the mode square to those balls. One convenient physical normalization for this bilinear constituent is \(\beta(ah)^6(ah)^{-4}\) multiplying the two spatial sums of the tree-linked curls and the two cosine factors. The theorem shows that its covariance with \(A\) tends to zero faster than every inverse power of \(n\). In contrast its canonical periodic Gaussian tangent has a positive limiting mixed covariance for suitable such balls. Indeed in the free law the tree transports drop out of the quadratic jet. At separated time the fine field-strength covariance in physical units converges uniformly to its smooth periodic kernel \(C_{\mu\nu,12}(t,z-x)\). To check this directly, use \(G_{n,\omega}\) from §4.35 and the two curl multipliers. For \(t\) in the fixed support of \(f\) the spatial Fourier series after physical rescaling is dominated by \(C(1+|\mathbf p|)^C e^{-c_f|\mathbf p|}\), including discrete temporal differences of \(G_{n,\omega}\); the zero spatial curl mode does not enter. A normalized early \(12\)-flux is a positive spatial average of the fine curls in a box of width \(O(ah)\to0\). The Wick contraction for plane positions \(x,y\) is therefore a positive constant times
\[
 K_f(x,y)=\int f(t)\sum_{\mu<\nu}\int
 C_{\mu\nu,12}(t,z-x)C_{\mu\nu,12}(t,z-y)\,d^3z\,dt .
\]
At \(y=x\) this is strictly positive, by the nonzero transverse mode in (TRUE-PLANE-GAUSSIAN-OVERLAP). Continuity and spatial translation allow the two **disjoint** balls with \(\inf_{x,y}K_f(x,y)>0\); the spatial Riemann sums and positive cosine factors preserve that lower bound. Hence a uniform relative Gaussian estimate for these genuine long tree terms on the early annuli is false. This counterexample concerns a constituent of the fixed physical frequency square. The sought \(\Psi_k\) uses a fixed physical terminal mesh, where the number of tree edges is fixed and the early open-path estimate cannot remove their overlap. To control (SIGNED-PLANE-ANNULI) one must bound the generation of the gauge-invariant near-diagonal plane rows and their reconnections at the later scales. Neither a common unmarked density bound on four-dimensional stopped balls nor the correct sign of the Gaussian tangent gives that signed remainder.

**The complete bounded early mode, including its near-diagonal row.** Choose the compatible bounded convention
\(\overline\Psi_j=|n_j^{-3}\sum_x w_x\operatorname{Ad}(P_x)J_x|^2\), \(n_j=n/h\), \(|w_x|\le1\). At the fixed terminal mesh this is a fixed positive multiple of the test in §4.143. Under the oriented additive-plaquette susceptibility clauses of §4.113, without a pressure disc for the plane variable, the full positive-time source just defined obeys \(\|A-\mathbb EA\|_2\le C_f\beta n^2\). Indeed apply (ADDITIVE-PLAQUETTE-SUS) to the actual oriented fine plaquettes and sum over the six orientations. Put \(R=C(1+\beta)^2h^4\log(2+n)\). Pairs at tree distance at most \(R\) have total coefficient sup norm at most \(C(R+1)^3/n_j^3\): at each root the number of spatial sites within this tree distance is bounded by its ordinary three-dimensional ball. This count includes the coincident pair. For all remaining pairs use (EARLY-NONLINEAR-PLANE-TRANSPORT); their total absolute coefficients are bounded, and the action has the polynomial deterministic bound used above. Choosing \(C\) for any fixed \(b>0\) gives
\[
 |\operatorname{Cov}_{\mu}(A,\overline\Psi_j)|
   \le C_{f,b}\beta n^2 (R+1)^3/n_j^3+O_{f,b}(n^{-b})
   = n^{-1}\operatorname{poly}(\beta,\log n)+O_{f,b}(n^{-b})
     \longrightarrow0
 \tag{EARLY-COMPLETE-PLANE-SCORE}
\]
uniformly for \(h\le\beta^\gamma\). Here the unspecified polynomial is bounded explicitly by \(C\beta h^3[(1+\beta)^2h^4\log(2+n)+1]^3\). Multiplying every \(\overline\Psi_j\) by the same terminal normalization preserves this conclusion. Multiplying **each early scale** by \((ah)^{-4}\beta\) defines a different magnitude; the near-diagonal bound must not be transferred with that extra factor. The remote-patch counterexample above used precisely the latter physical bilinear normalization and remains valid there.

It follows that for the original fixed bounded terminal statistic
\[
 \operatorname{Cov}_\mu(A,\overline\Psi_k)
   =o(1)+\sum_{i=J}^{k-1}
        \mathbb E S_i[\overline\Psi_{i+1}(\pi_i W_i)-\overline\Psi_i(W_i)],
 \qquad J=\lfloor\gamma\log_L\beta\rfloor .
 \tag{FIXED-PLANE-LATE-SCORE}
\]
This is a vanishing estimate for the **whole genuine early score** rather than for a collection of favorable histories. Thus the late sum is the entire candidate fixed-distance overlap up to \(o(1)\). A small-error argument around an already nonzero early bounded score has no such starting value.

For the physically normalized separated-patch constituent, one can also quantify a limitation on the signed late-error comparison itself. Denote its full and Gaussian cross-covariances by \(W_i,G_i\) with their own fixed action metric normalization. At the above \(J\), \(W_J=o(1)\) whereas \(\liminf G_J\ge c_0>0\). At the physical terminal mesh the elementary triangle inequality gives
\[
 |W_k-G_k|+
 |(W_k-W_J)-(G_k-G_J)|\ \ge\ c_0-o(1).
 \tag{LATE-PLANE-COMPARISON-DICHOTOMY}
\]
Consequently a perturbatively small comparison of both the terminal patch overlap and the cumulative late signed correction, in this physical normalization, is impossible. This does not exclude a positive terminal overlap: if it is comparable with its Gaussian value, the late connected response must supply a nonperturbatively different correction from that of the Gaussian telescope. Even assuming successful weak charts everywhere, contraction of the single fine slot per face by this method gives exponent at most \(C n/[(1+\beta)^2h^5]\) on a path of \(O(n/h)\) edges, which loses force for late \(h\). The signs and the magnitude of (FIXED-PLANE-LATE-SCORE) in the actual law are still unknown.

## 5. Imports and sources

The covariance literature input to §4.14 is Balaban CMP 99 (1985), Theorem 3.15, equation (3.187), for the physical constrained Gaussian covariance. Its statement, covariance dictionary (3.157)–(3.158), and flat-background regularity hypotheses are verified as described there. All finite-dimensional algebra, source identities, Fourier and harmonic-coefficient estimates, Gaussian contractions, and conditional-expectation identities used here are proved in the text. Gaussian-step results are kept separate from the nonlinear compact-law estimates. Section 4.22 additionally uses the general chessboard inequality with its full proof and even-torus/block-support hypotheses verified; Wilson site-reflection positivity is independently proved there.

| Item | Source | Status used here |
|---|---|---|
| Regular classical minimizing orbit | Balaban CMP 102 (1985), Theorem 1 and Proposition 9, (2),(7)–(10),(19)–(21),(172)–(173); printed pp.279,309 | L on the homogeneous compatible hierarchy in §4.41; classical window only |
| General chessboard inequality | Biskup (2006), §4.3, Theorem 4.8, (4.31); proof valid for arbitrary even factor torus and shared block faces | L; used only after proving the Wilson link-algebra reflection hypothesis in §4.22 |
| First-step constrained covariance | Balaban CMP 99 (1985), pp. 428,432; (3.157)–(3.158), Theorem 3.15 (3.187); regularity (3.35)–(3.36) verified at the identity | L at the specified flat regular domain; used for §§4.14–4.16 and §4.19 Gaussian locality and kernels |
| Complete RG representation and flow | Program interface I-0c | Assumed program interface; conclusions conditional on it |
| Transport, P6 estimate, source derivatives, analyticity | Program interface I-1 | Assumed program interface; no norm strengthening |
| Ordinary/frustration Fourier reduction | Standard reduction | Proved in §4.4 |
| Fixed-volume analytic reduction and extra lattice-mark requirement | Standard fixed-volume analytic reduction | Sharpened in Theorem 3.4 |
| Bare H physical coefficient and normalization | [Source estimates](source_estimates/README.md) §155, PD12.4–PD12.18 | Exact coefficient derived in §4.7 |
| Ward/contact distinction | Ward identity | Proved as H-COV |
| Ordinary variance is not reflected excitation | [Source estimates](source_estimates/README.md) §32.6 | Respected; stronger boundary identity proved here |
| Real source pressure and first plaquette-action moment | Direct full-tree and temporal-forest proof in §4.11 | P under REG; no extra moment import is needed for this paper |
| T1 clean mixing/contact rows | T1 equations (3.3), (3.7), (3.11), Remark 3.5 | Algebra absorbed only if their actual coefficients and estimates are supplied; other source and normalization statements of T1 are not used |

The direct H calculation has fixed source order two. Its constants depend on the group metric, fixed original pointing/stencil convention, and $c_\beta$ for the physical normalization. The all-m extension of Theorem 3.6 records dependence on $C_{D,m}$ explicitly; it makes no unproved factorial-growth claim for that constant.

Finite-cutoff well-definedness of the representatives is proved for compact Wilson fields. Their smooth classical limits identify the intended classical types. Neither statement proves interacting normalization, an equations-of-motion quotient, or continuum tensor covariance.

## 6. Interface statement and sufficient inputs

**Assumed:** I-0c and I-1 as stated. No additional moment estimate is assumed: §4.11 proves the real pressure and first action moment needed for the susceptibility and bare contact arguments.

**Proved here (P):** compatible finite formal gauge-invariant type spaces and compact lattice representatives; exact scalar/operator-valued contact algebra and reflection-positive local nonlinear source composition under FULL-SPLIT; triangular inversion and compatibility algebra; quantitative all-q age summation; all-order Cauchy implication under a displayed locally bounded analytic norm; Fourier/Ward reduction; improved zero-free criterion with only ZF open, since M and the Ward row are proved under REG; exact site-reflection boundary conditional-mean formula; quantitative boundary noncollapse criterion; first-step constrained action/H/ordinary-Ward rows, anchored all-order Gaussian cycle/chain bounds, uniform sourced Gaussian covariance locality, and a single-factorial analytic-polymer derivative theorem; diagonal Taylor contact extraction with summable remainders; exact bare H two-source coefficient and pointwise force-factor bound; uniform flat-background quadratic source stability and Gaussian determinant domain; an explicit positive Gaussian reflected test; an actual compact-law fixed-cell reflected witness with a quantified error and cutoff-scaling limitation; actual nonflat compact-cell ordinary innovations with annealed background-energy control; higher-degree Gaussian anchored cumulants with degree-dependent factorial order and a compatible Wick mixing prescription; actual compact-cell all-order higher-composite cumulants and fixed-order Gaussian convergence; full-torus marked plaquette exponential moments and all-order pointwise bare-composite cumulants under the displayed even block-tiling condition; the exact moving-cutoff coupling-derivative flux; full-sector fixed-cell innovations and a finite shifted-grid decomposition covering every original stencil; a volume-uniform native physical-chart construction using the actual augmented Hessian and based-gauge critical-point identification; a localized scalar-difference implication with the rooted scalar and physical-source matching explicitly conditional; full two-step covariance and Ward budgets, Gaussian retained-volume decay, the joint two-clean-step quadratic source bound, the full-law off-plane susceptibility bound and reduction to one eight-site temporal mark; extensive real innovations on two admitted nonflat clean steps; a full Wilson covariant Hodge bound, nonlinear critical source gain and a first nonidentity fluctuation bound on the matched gauge-saturated native fiber, its homogeneous classical propagation with the original minimizing current and an actual flat or small nonflat clean innovation with current-volume order; a periodic blocked Gaussian witness including flat Cartan sectors; uniform regular classical window and coarse energy estimates; the exact first Gaussian physical-action row with auxiliary gauge directions separated and the physical dimension counted.

**Not proved here:** I-3 in full. The interacting mixing matrices for all dimensions, all-history contact bounds, higher cumulants for the general renormalized family, and uniform physical reflected nondegeneracy remain open. Ordinary susceptibility has the conditional status of Theorem 3.15, including its actual smooth-pressure premises.

**ICR-3-MIX:** For every D, provide the actual finite retained-jet mixing matrices, including identity and dimension-four rows of dimension-six insertions and all tensor/anisotropic completions allowed by lattice symmetry, with diagonal block estimates and a common extraction prescription compatible in D. The P6 estimate alone leaves these rows unrestricted. The present paper then supplies the exact inverse normalization and compatibility algebra. Restoration of full rotational tensor laws is a separate problem, not a consequence of this algebra.

**ICR-3-CON:** Supply the operator-valued nonlinear source map $\Psi_a$ and scalar $L_a$ of §4.17, or an equivalent full product prescription, with coefficientwise compatibility in D. For each completed connected m-source birth, supply its actual source-anchor kernel and a bound on its *summed absolute* retained scalar/contact coefficients, including all denominator responses and between-history covariances. At m=2 and dimensions d1,d2, the precise sufficient input is anchored row total variation $C_{D,2}\ell_k^{-w}$, range or summable displacement moments of order $\lfloor w\rfloor+1$, with $w=d_1+d_2-4$. Theorem 3.6 turns this into a genuine diagonal subtraction plus a summable remainder. For physical H–H, w=8; for action-density pairs, w=4. A bound on the completed scalar after cancellations is not a bound on this absolute kernel.

**ICR-3-ALL:** Section 4.55 supplies a single Gevrey test norm and the explicit all-order factorial exponent from CONTACT-ALL-KERNEL.  Either prove AN-D for the contact-renormalized functional on a specified source norm ball, or supply all source-order derivative estimates with quantified factorial growth and compatible local contact algebra. The latter permits p>1 and need not assert an analytic generating function for every irrelevant composite. The existing first/second derivative clause does not by itself close this requirement.

**ICR-3-ZF (reduced to one mark):** PHYSICAL-H-ZERO in §4.56 excludes a fixed disc for the unrescaled physical source already at a constant smooth mark.  On the commensurate reference tori of §4.32, identify the actual admitted I-1 source norm for the single nonnegative microscopic comb and prove (SHRINKING-COMB-DISC) with zero-free radius \(r\ge c/S_\beta^3\), using the sharper §§4.84–4.85 bound and (COLUMN-BOX-SCALE); the fixed radius in COMB-ZF suffices as well. The signed sum in (SIGNED-COMB-ZEROS) gives the exact weaker zero-counting alternative. A direct real bound $\operatorname{Var}(r_{f^{\rm comb}})\le B N_{\rm cell}$ also suffices. Section 4.46 gives a sufficient real two-jet iteration permitting polynomial growth in scale number. On even tori §4.38 chooses the single time-independent eight-site pattern and computes its exact temporal electric insertion. A common stride $L^s$ reduces to one coarse-cell period after s blockings. The eight-site rectangle of §4.38 keeps a fixed transverse period two under odd native blocking factors. On tori to which the sublattice construction does not apply, Theorem 3.4 retains its all-plane-wave sufficient criterion.

**Real moments:** no separate real-moment input (ICR-3-MOM) is needed for susceptibility or the bare H contact. The exact full-tree/temporal-forest partition comparison of §4.11 proves M and the required first action moment under REG, and H-LOCAL gives the Ward contact row. Section 4.22 further proves marked-set exponential plaquette estimates under its explicit even block-tiling condition, and converts them to all-order pointwise bare-composite cumulants. No anchored connected summability or renormalized continuum hierarchy is inferred.

**ICR-3-UNIFORM (sharper sufficient smooth-source input).** Under the oriented smooth plaquette clause, (FINE-UNIFORM-WARD-REDUCTION) eliminates the need to extend the source norm to microscopic aliases. It suffices to control the single smooth constant fine-uniform unamplified temporal frustration at zero, or to prove a complex disc of radius \(c s_{**}^{-3}\) for that one source. The compact-law Ward/real-slope estimate of §4.129, not a disc for the physical dimension-six source, underlies this criterion. Alternatively bound the centered additive real log at strengths \(|t|=O(\beta^{-1})\) by \(CV/\beta^2\). Section 4.128 pays the compact bare source on genuine early rough footprints on the stated terminal and occupancy margins; the complementary punctured clean-core scalar and its conditional means have not been bounded.

**Further result.** Section 4.136 proves the centered fine-uniform real estimate on the named independent-window and spare native margins. On the same-source smooth pressure clauses, Theorem 3.15 gives the ordinary susceptibility corollary; if those concrete clauses do not survive, the directional reduction still records exactly which additional pressure statement is needed. The new action contrast and tight rescaled Gaussian result are in §§4.137–4.138.

**ICR-3-REF (physical two-source input):** Sections 4.35–4.36 give a periodic physical-scale reference witness for all original linearized blockings and a bounded-event route. Prove WINDOW-COMPARISON and WINDOW-ERROR for the actual positive-time readouts, or prove either BND for a fixed nonconstant physical test family and a genuine boundary readout, or REF for the explicitly chosen reflected action-density bump, with the same operator normalization used in the mixing construction. The error must refer to the actual jointly transported physical product. Finite-cutoff invertibility, a positive reference density, or an ordinary variance lower bound is insufficient.

## 7. Residual propositions and open targets

**R3-1 (O): complete mixing rows.** Construct and bound the interacting retained coefficients through every source/history transition, not merely their P6 projection. The first concrete calculation is the two-dimensional identity/action row generated by a physical H insertion, with the exact pointings and normalization retained. Theorem 3.2 will then normalize the row without hiding logarithmic factors.

**R3-2 (O through the general nonlinear history): newly generated two-source kernels.** In the exact conditional-cumulant tower of §4.7, bound the scalar kernel from $\operatorname{Cov}(r_1,r_2\mid Y)$ in the anchored absolute norm KT, including mixed and large-field histories. The previously born H contact already has a proved microscopic row bound under REG; repeating that bound does not control the new covariance term. The required estimate is a locality statement for the conditional covariance at each constrained fluctuation scale. Sections 4.13–4.15 supply its first-step Gaussian rows and all-order anchored estimates. Sections 4.26–4.34 give the paired constrained innovations, the full Ward tower, the two-clean-step estimate at flat terminal field, and a nonflat critical-value estimate with the original Wilson energy. Sections 4.33 and 4.37 quantify the dimension gain of the retained Gaussian force row at arbitrary linearized blocking depth. Section 4.16 transfers actual local analytic polymer bounds to the same norm with one factorial; the complete nonlinear/all-history hypothesis remains to be proved.

**R3-3 (O for the full interacting history): all source orders.** The first-step quadratic Gaussian source kernels and analytic-polymer factorial implication are proved in §§4.14–4.16. Section 4.19 extends the Gaussian calculation to arbitrary fixed-degree local polynomials with the necessary degree-dependent factorial exponent, and §4.20 proves the same factorial order for full compact Wilson cells, uniformly in beta. Section 4.22 upgrades bare local moment and pointwise cumulant bounds to the full torus, but does not bound their anchored connected sums. Section 4.42 verifies on the full Wilson law why a common bare exponential source disc fails for some higher-degree types. Establish the required source-local analytic or factorial derivative control with explicit dependence on D and m, and a contact prescription whose restriction in D is exact. Sections 4.28 and 4.31 give the joint two-clean-step quadratic source class and the consequences of T1’s flat-terminal expansion, with both selectors and the variance of the first retained mean. Theorem 3.6 supplies fixed-order diagonal Taylor extraction once its kernel is known. For d>4 the naive Taylor order grows with m; a proof of uniform product test norms must handle this rather than suppress it in a constant.

**R3-4 (alternative open route without the smooth pressure clauses): one periodic frustration variance.** Sections 4.29–4.32 prove OFF-PLANE-SUS and reduce the complete susceptibility to the single nonnegative rectangular comb variance. Its fine-lattice physical smooth-source norm grows at least as in COMB-SMOOTH-COST. QREL proves an n-independent quadratic source domain even in flat toron backgrounds. The next precise step is to use the **constrained**, fixed-scale fluctuation form to absorb the nonlinear source Hessian without a whole-torus inverse. At a fixed Dirichlet block, a strictly positive constrained Hessian can support a local Laplace comparison. For the torus/all-history theorem one must retain live fields and source-dependent denominator responses, assemble a common logarithm, and show its analytic continuation does not approach a zero. The old flat-block regime requiring a power of the block side in the lower bound on beta cannot be extrapolated to a fixed physical block along beta of order log(1/a).

**R3-5 (O): actual reflected error.** The genuine bounded microscopic-plane test in §4.143 has an explicit nonzero free overlap; bound its actual signed Wilson cross-error after the physical normalization. The straight graph and raw connection heat test have the full-law obstructions in §§4.141–4.142. Use the explicit bump of §4.9 with t comparable to $\ell_0$. Jointly transport the positive-time test and its reflection, compute the stopped-scale leading coefficient in the chosen normalization, and bound the full signed remainder by $\lambda_0/2$. Local diagonal contacts do not enter this separated matrix element. The finite physical-range remainder from Theorem 3.6 does enter and must be retained. Sections 4.35–4.36 give the periodic blocked covariance and reduce a lower bound to a finite-window probability and separated contrast of the actual matched row. Equivalently construct the actual boundary readout in BND and prove the nonconstant component of its conditional mean survives with a quantitative lower bound.

**R3-6 (O): identities, operator-valued contacts, and anisotropy.** The scalar-contact prescription must be supplemented by the nonlinear local source map and PARTITIONS formula of §4.17. At D>4, the dimensionally allowed output contact types grow with source order according to CONTACT-DEGREE; this closure and its quantitative bounds are not yet constructed. No equations-of-motion quotient is made before the Ward contact identities are proved for every joint product. Hypercubic dimension-four tensor completions cannot be dropped merely by labeling them irrelevant. Their mixing coefficients and tensor transformation laws require a joint construction of the mixing and tensor-covariance analyses.

**R3-7 (O beyond the stated first-step geometry): physical source and retained means.** Section 4.24 constructs the physical coarse chart with the actual augmented Hessian and its based-gauge identification. Section 4.25 computes the physical Gaussian action row, including its physical rather than auxiliary dimension. T1 Theorems 7.32 and 7.35 now supply the physical first and second clean constant-action rows under their stated native margins. Extension of these estimates to complete nonflat and mixed histories remains necessary. An argument that instead substitutes g(w) must retain both the cutoff flux of §4.21 and all gauge/normalization derivatives. For full-law ordinary susceptibility, §4.23 already controls every fixed-cell innovation and reduces the remaining problem precisely to the covariance of its explicit sum of retained conditional means. Neither repeated local moment estimates nor another fixed-cell Gaussian witness bounds that retained covariance.

**R3-8 (alternative open route; susceptibility has Theorem 3.15 on its stated hypotheses).** Section 4.38 computes the operator for the comb needed on even tori. Bound the equal-time two-insertion kernel and the integrated spectral sum of COMB-TRANSFER-SPECTRUM per selected spatial site, or prove COMB-ZF. This controls the explicit single real variance now equivalent to full SUS. Section 4.37 supplies the retained Gaussian complex force gain and §4.34 bounds the regular nonflat critical contribution by an actual Wilson energy. Sections 4.39–4.40 further bound the full Wilson matching force by a covariant Hodge estimate and give the actual first clean nonidentity source row an $L^{-2}+C_L/\beta$ relative-action bound. Section 4.43 proves both admitted nonflat clean innovations for all marks by the exact joint constrained Hessian and undivided Wilson averaging. Section 4.57 evaluates the full single-link innovation and expresses the whole remaining comb variance as the covariance of its explicit exterior heatbath field. It also proves the failure of a background-uniform conditional bound on compact exteriors. Section 4.58 proves exact factorial order two for absolute conditional jets in the \(SU(2)\) Wilson comb. Sections 4.68–4.72 also integrate full four-dimensional growing boxes, compute a suppressed next face innovation and isolate a vanishing fraction of possibly exceptional Fourier bins. Sections 4.73–4.85 compute the signed sum through \(S_\beta\), bound the full real pressure slope error by \(C/S_\beta^3\) there, and give (SIGNED-COMB-ZEROS) at \(R\asymp S_\beta^{-3}\). Sections 4.91–4.96 compute the strict frustration noise at order \(V/\beta^2\), exhibit the true slow curvature sector and prove (SHIFTED-ROUGH-CONTRACTION) above a common outer grid. The full one-skeleton and long colored sectors are removed by §§4.98–4.112. The remaining normalized spatial exterior scalar has bounded Dirichlet energy (SPATIAL-EXTERIOR-SCORE), while (SPATIAL-EXTERIOR-SLOW-SINGLET) prevents using a general Poincaré constant. Sections 4.121–4.124 give its positive inverse spectral formula on the genuine marginal, the complete low-band comparison on the quadratic torus, and the compact separated temporal Ward reduction. Section 4.125 proves that the single fine-uniform temporal frustration variance suffices, eliminates all parity aliases by a spatial one-slice Ward replacement, and bounds all fine-mark variances by (CUBIC-CORRECTED-SUS) under the stated smooth additive finite-family clause. Theorem 3.15 and §4.136 establish its real pressure estimate on the specified native margins, and its ordinary variance when the displayed smooth same-source pressure clause holds.

**R3-9 (O): physical window normalization and observable contrast.** The regular classical action now has the uniform canonical expansion of §4.41 and the coarse curvature lower bound of §4.44, and the reference Gram survives arbitrary flat toron mixtures by §4.45. Section 4.47 performs the regular-holonomy normal integration conditionally on the precise fieldwise TERMINAL-DENSITY, fixed positive endpoint, and positive-half readout. Match those hypotheses to the original construction and then bound the physical separated contrast in WINDOW-ERROR. Section 4.54 gives the true positive-time minimizing-field action row and its strictly positive window contrast under TERMINAL-DENSITY. Section 4.97 also gives a positive reflected local magnetic Gram in the full Wilson law on a growing fine-lattice scale with \(aR\to0\). The remaining fixed-physical-scale signed fluctuation and history correction requires the same operator normalization as the mixing construction.

**Overall status.** The real early-prefix pressure and ordinary susceptibility have the stated native and smooth-source hypotheses. Section 4.137 gives an action contrast through the growing protected prefix; it has not controlled the remaining physical scale. Section 4.138 gives Gaussian subsequential limits for the additionally rescaled tight frustration under the named smooth profile discs. Section 4.139 identifies its explicit Ward contact component and proves exact reflection nullity of that component. Sections 4.140–4.143 give fixed-physical-scale retained windows, two full-law obstructions for actual plane probes and a surviving bounded spatial test with positive Gaussian reference overlap. Sections 4.144–4.145 prove a vanishing bound for its entire bounded early mode and a Wilson/Gaussian obstruction for its physically amplified separated-patch constituent. The later signed response, and hence the interacting physical overlap, remain open. General interacting I-3 and Yang–Mills existence remain unproved.

## 8. Summary

On the reference torus a directional Ward identity replaces temporal frustration by a density on one spatial slice at bounded variance cost. Positive transfer removes its spatial momentum. Repeating in each direction reduces every microscopic weighting to one uniformly weighted temporal source.

On the specified native margins its centered additive real log is bounded by the lattice volume divided by beta squared. The proof keeps the independent fluctuation cutoffs and the normalized exterior measure. Occupied-volume moments pay the additive source on rough footprints through an early stop. Real conditional comparisons transport homogeneous first-row estimates on the protected complement. The symmetric Wilson average satisfies a nonlinear curvature-energy inequality with leading constant one in four dimensions. Summable source coefficients then pay the conditional fluctuations using the original fine energy. The terminal response includes the random vacuum contribution of missing roots.

Under the specified smooth additive loop pressure disc this gives extensive variance for fine-uniform frustration. Six oriented additive plaquette clauses extend it to every microscopic weighting. The physical dimension-six normalization is restored separately.

The magnetic exterior has a positive inverse spectral formula on forms. Two fixed physical stopped windows distinguish the minimizing-field action. Bounded early plane modes lose their separated contrast. The total-force Ward component converges to explicit Gaussian white noise. Its separated reflected norm vanishes identically at every cutoff.

Under the corresponding smooth profile discs, the additionally rescaled tight frustration has vanishing higher cumulants and centered Gaussian subsequential limits. Its limiting covariance and its reflected part have not been identified.

Anchored kernel estimates give scalar and operator-valued contact prescriptions on one Gevrey test norm. The physically amplified bare frustration has complex pressure zeros approaching zero despite linear plaquette mixing. Full interacting mixing, arbitrary-history higher cumulants and a reflected lower bound at fixed physical separation remain open. No mass gap is assumed.
