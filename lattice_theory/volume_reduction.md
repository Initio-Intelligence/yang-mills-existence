# Exhaustion and conditional infinite-volume reduction

**Status convention.** **(P)** means proved below, including a proved implication between stated hypotheses. **(L)** means a literature theorem, with its hypotheses and exact locator. **(C)** means a conclusion conditional on explicitly stated inputs. **(O)** means an outstanding claim in this construction, not a claim that no possible proof exists elsewhere. Definitions and bibliographic metadata are not assertions of existence.

**(C) Main conclusion.** The proposed fixed-physical-scale argument proves S94 if the original partition functions admit **one common bulk vacuum subtraction** and uniform integrated stability at the stopping scale. Pointwise stability everywhere is unnecessary. **(L)** Bałaban's published stability constants are already uniform in RG depth and torus size [B122II, Theorem 1 and (0.1)]. **(O)** This note does not complete the additional identification of his entire finite-torus scalar normalization with a common bulk density, nor the required renormalized observable hierarchy. Consequently it does not prove item 6 for Wilson Yang–Mills.

## 1. The precise theorem needed for item 6

**(C) Theorem A — simultaneous continuum and infinite-volume extraction.** Fix a countable family of Hermitian gauge-invariant fields and one volume-independent renormalization prescription. For each finite set of field types, require the following bounds uniformly over all insertion orders and type assignments from that set. Suppose that, on compatible tori, the **mixed** Schwinger distributions satisfy:

1. Uniform distribution bounds, for every finite type list and every joint test \(F\), independent of \(a,T\). For reconstruction require the OS II condition
   \[
   |S_{m,a,T}(F)|\le A B^m(m!)^p\,p_{sm}(F),                 \tag{1}
   \]
   with fixed finite \(p,s\), on the Schwartz space flat on coincidence diagonals. Here
   \(p_r(F)=\max_{|\alpha|\le r}\sup_{x\in\mathbb R^{4m}}(1+|x|^2)^{r/2}|\partial^\alpha F(x)|\), as in OS II (2.1), (4.1). An alternative seminorm must be bounded by \(C^m(m!)^r p_{s'm}\) with fixed \(C,r,s'\). Bounds on all joint tests are needed if convergence of contact extensions is claimed; flat-test bounds construct only the restricted hierarchy and do not determine those extensions.
2. Normalization, Hermiticity, permutation symmetry, and reflection positivity on the **actual renormalized mixed algebra**, with compatible embeddings of tests into large tori.
3. The selected limiting hierarchy is covariant under the full Euclidean group, with the prescribed transformation laws for its field types. This is a separate input. Approximation of continuous translations by lattice translations must be justified by uniform test continuity.

Then any sequence \(a_j\downarrow0,T_j\uparrow\infty\) has a subsequence yielding a hierarchy satisfying these bounds and positivity properties. With assumption 3 it reconstructs a local positive-energy Wightman theory, possibly with several vacuum vectors. A nontrivial Yang–Mills theory requires additional noncollapse and Yang–Mills identification inputs.

**(P) Compactness proof.** For every order and type list choose countably many dense joint tests, using a countable compact-support exhaustion when necessary. Uniform bounds make each scalar sequence bounded. Successive subsequences followed by diagonal extraction give convergence on their union. For an arbitrary test \(F\), approximate by a selected \(G\); uniform continuity gives
\[
|S_j(F)-S_k(F)|\le 2C_m p_m(F-G)+|S_j(G)-S_k(G)|.
\]
First choose \(G\), then \(j,k\): this proves convergence and the same continuity bound. Every finite reflection-positivity Gram matrix formed from the allowed OS test algebra converges entrywise; its quadratic forms remain nonnegative. Symmetry and other linear identities pass identically. This constructs one common hierarchy; it does not assert agreement of different subsequences. ∎

**(L) Reconstruction qualification.** OS I, Remark 3(b), p.89, permits dropping clustering; OS II, Introduction Remark 6, p.283, preserves these subset implications. Use its corrected growth hypothesis, §IV.1, p.287, (4.1), and Theorem \(E'\to R'\); Remark 5 covers countably many fields. Finite factorial powers are allowed. An unspecified product norm, or estimates only for separated supports, do not state this hypothesis. A product bound for all tests in one fixed Schwartz norm may supply it, but the norm-to-joint-test implication must be verified.

**(C) Pure-phase supplement.** For the reconstructed finite-component theory assume, for each component and every Schwartz \(f\) with compact Fourier support, a strictly positive nonincreasing \(F_f\) such that, with closures from the common polynomial domain,
\[
F_f(H)\mathcal H\subset D(\overline{\phi(f)}),\qquad
\overline{\phi(f)}F_f(H)\text{ is bounded}.                 \tag{2}
\]
**(L)** Driessler–Summers, Definition 2.1 and Theorem 2.3, pp.334–336, then give a central direct integral whose almost-everywhere components satisfy all Wightman axioms, including unique vacuum and clustering. Their alternative is a specifically intrinsically local smeared field with the cyclicity and nowhere-vanishing-Fourier-transform requirements of Theorem 2.3(2). No rate of clustering follows. They warn that arbitrary extremal polynomial-algebra decompositions need not cluster. **(O)** A whole countable operator hierarchy needs a compatible common-algebra extension; decomposing finite families separately does not establish it.

## 2. Arrows (i)–(iii): the valid source reduction

Write \(V_T=T^4\), \(p_{a,T}=V_T^{-1}\log Z_{a,T}\). Work first with the pressure formulation of S94. Translation to the vacuum functional of the underlying construction additionally uses its stated absolute stability comparison between that functional and \(\log Z\).

**(L) Arrow (i), with geometry.** FILS, Theorem 4.1, gives the abstract chessboard inequality under reflection positivity. For a tiling by \(M\) reflection cells, localized insertions \(F_c\) obey
\[
\left|\left\langle\prod_cF_c\right\rangle\right|
 \le\prod_c\left\langle\mathcal D F_c\right\rangle^{1/M},   \tag{3}
\]
where \(\mathcal D\) disseminates by reflection and complex conjugation. The required positive replicated quantities, support algebra, and even reflection tiling are hypotheses, not automatic for arbitrary sources.

**(P) Source identity.** For a linear, reflection-compatible source insertion \(X(J)\), if \(F=e^{X(J)}\), dissemination gives the exponential of the sum of the reflected sources. Directly dividing the two defining Haar integrals yields
\[
\langle\mathcal DF\rangle=Z_T[J^{\rm dis}]/Z_T[0]
=e^{V_T(p_T[J^{\rm dis}]-p_T[0])}.
\]
Taking the \(1/M\) power replaces \(V_T\) by the cell volume \(v=V_T/M\). Omitting that root loses the useful volume cancellation. ∎

**(P) Arrow (ii) and its direction, using the literature transfer construction.** For a fixed transverse torus \(\Sigma\), the physical positive transfer operator gives
\(Z_{t_*\times\Sigma}=\operatorname{Tr}K\) and
\(Z_{qt_*\times\Sigma}=\operatorname{Tr}K^q\), with \(K\ge0\) trace class. For eigenvalues \(\lambda_i\ge0\),
\(\sum_i\lambda_i^q\le(\sum_i\lambda_i)^q\).
Division by the respective volumes proves \(p_{qt_*\times\Sigma}\le p_{t_*\times\Sigma}\). Enlarge the four coordinates successively:
\[
0\le p_{a,T_*}[0]-p_{a,qT_*}[0].                          \tag{4}
\]
The same proof applies to a source pattern whose paired slab is \(A^*A\), using identical source-free cutting kernels. The physical transfer construction is [OSl; Lü, Proposition 1, (17), (20)–(23)]. ∎

**(C) Scope of sourced (ii).** The collars, reflected-conjugate replication, and gauge projection of the underlying construction supply the intended geometry. Temporal plaquettes inside slabs are allowed. An arbitrary homogeneous source need not preserve positivity; a general complex pressure is not even ordered. Thus unrestricted \(p_T[J]\le p_{T_*}[J]\) is not established.

**(P) Arrow (iii).** For an admissible replicated pattern, subtract \(p_T[0]\) from (ii) and add/subtract \(p_{T_*}[0]\):
\[
p_T[J]-p_T[0]\le p_{T_*}[J]-p_{T_*}[0]
                         +p_{T_*}[0]-p_T[0].             \tag{5}
\]
If \(\mathcal G_T(J)=e^{-L_a(J)}Z_T[J]/Z_T[0]\), assume the same contact functional on both tori, additive on disjoint cell interiors and compatible with reflection/conjugation. Writing \(\mathcal D_R\) for dissemination on torus \(R\), this means
\(L_a(\mathcal D_RJ)=(V_R/v)\operatorname{Re}L_a(J)\).
The copied pattern is the same on the two tori; (3)–(5) and S94 give
\[
\log|\mathcal G_T(J)|\le
\frac v{V_{T_*}}\log\mathcal G_{T_*}(J^{\rm dis})+vC_0.   \tag{6}
\]
Here the disseminated reference functional is real and positive on the domain used for comparison; a zero is handled by an extended-real limit. This proves the local-source transfer under exactly those hypotheses. Cauchy estimates apply to the holomorphic original functional, although reflected-conjugate dissemination need not be holomorphic in its seed. ∎

**(P) From source bounds to coefficients.** For ordinary real random variables, bounds
\(\mathbb E e^{\pm tX_i/s_i}\le B\) imply
\(\mathbb E|X_i|^m\le2B m!t^{-m}s_i^m\), since \(y^m\le m!e^y\) and \(e^{|y|}\le e^y+e^{-y}\). Hölder then bounds the mixed product by \(2B m!t^{-m}\prod_i s_i\), without independence. Alternatively, a holomorphic functional bounded by \(B\) on \(\|J\|<\rho\) obeys, by Cauchy on radii \(\rho'/(m\|f_i\|)\),
\[
|D^m\mathcal G(0)[f_1,\ldots,f_m]|
 \le B(m/\rho')^m\prod_i\|f_i\|
 \le Bm!(e/\rho')^m\prod_i\|f_i\|.                       \tag{7}
\]
Here \(0<\rho'<\rho\); \(m!\ge(m/e)^m\) follows by integrating \(\log x\) over \([1,m]\). ∎

**(P) Joint-test promotion for a precise product norm.** Set \(H_0=1-\Delta+|x|^2\) on \(\mathbb R^4\), \(h_s(f)=\|H_0^s f\|_2\), with fixed integer \(s\ge0\). Suppose the tensor bound is \(C^m(m!)^p\prod_i h_s(f_i)\) for all tests. In the Hermite basis, \(H_0e_k=w_ke_k\), \(w_k=5+2|k|\), and \(A_3=\sum_{k\in\mathbb N^4}w_k^{-6}<\infty\), because the multiplicity at level \(j\) is \(O((1+j)^3)\). Expanding a joint \(F\) and applying Cauchy–Schwarz bounds its pairing by
\[
C^m(m!)^p A_3^{m/2}
\left\|\prod_{i=1}^m H_{0,i}^{s+3}F\right\|_2.
\]
This absolutely convergent expansion defines the unique continuous extension. Compact tests suffice: expanding smooth cutoffs converge to each Schwartz test in \(h_s\), and the multilinear bound extends the pairing. Put \(t=s+3\). Expanding each fixed differential operator \(H_{0,i}^t\) gives at most \(C_t^m\) in total absolute coefficient weight, total polynomial degree at most \(2tm\), and differential order at most \(2tm\). Hence its product applied to \(F\) is bounded pointwise by
\(C_t^m p_{(2t+6)m}(F)(1+|x|^2)^{-3m}\).
The squared weight integrates to
\(\pi^{2m}\Gamma(4m)/\Gamma(6m)\le\pi^{2m}\).
Thus (1) follows with a larger \(B\), the same factorial exponent, and fixed seminorm order coefficient \(2t+6\). ∎

**(O) Remaining source lemma.** Prove a common holomorphic source domain, the fixed-torus bound in (6), transport of the physical observables, and promotion to (1) for the full mixed hierarchy. A precise sufficient source-level target is
\(\left|\mathcal G_{a,T}(\sum_{i=1}^m z_i f_i)\right|\le B^m\)
whenever \(\sum_i|z_i|h_s(f_i)<\rho\), with \(B,\rho,s\) independent of \(a,T,m\), the oscillator norm just defined (or a norm it dominates), and all compactly supported \(f_i\), including overlapping supports. Equation (7) and the Hermite argument prove (1) from this target; the actual mixed OS positivity remains an independent input. For the contact-normalized H package, extending (6) to this full mixed source statement is not ordinary probabilistic Hölder.

**(P)** This analytic-source target is only sufficient: (7) gives factorial exponent 1, whereas Theorem A allows any fixed finite exponent. Direct bounds on renormalized derivatives can therefore replace holomorphy if they imply (1). ∎

**(P)** Nonlinear contact subtraction does not itself preserve ordinary moment positivity: \(X=0,L(t)=t^2\) gives \(\mathcal G''(0)=-2\). This is not a counterexample to OS positivity: diagonal contacts may be invisible on its flat-test algebra. In fact, if
\(L(\theta\overline J_i+J_j)=\overline{L(J_i)}+L(J_j)\)
for sources in the open positive-time halfspace, the renormalized reflection kernel is
\(K'_{ij}=e^{-\overline{L(J_i)}}K_{ij}e^{-L(J_j)}\).
It is a diagonal congruence of the bare positive kernel. Finite differences and their analytic derivative limits preserve positive Gram matrices. Thus this precise halfspace factorization proves positivity for the corresponding derivative algebra; it must be checked for the actual contacts and observable identification. ∎

## 3. Arrow (iv): the precise sufficient RG theorem

**(C) Theorem B — common-subtraction stability.** Fix \(\ell_0>0\) and compatible tori or intermediate rectangles with minimum period at least \(T_*\). Suppose exact RG, with all original scalars retained, gives
\[
Z_{a,R}=e^{E_a V_R}\Xi_{a,R},\qquad
\Xi_{a,R}=\int\rho_{a,R}\,d\nu_R,\qquad
e^{-BN_R}\le\Xi_{a,R}\le e^{BN_R},\quad
N_R=V_R/\ell_0^4,                                      \tag{8}
\]
where \(E_a\) is independent of \(R\), and \(B\) independent of \(a,R\). Then the pressure form of S94 holds with constant \(2B\ell_0^{-4}\). Under the additional premise of the underlying construction
\(|\log Z_{a,R}-V_{a,R}|\le C_{\rm st}V_R\), its vacuum-functional version holds with constant \(2B\ell_0^{-4}+2C_{\rm st}\).

**(P) Proof.** Taking logarithms gives \(|p_{a,R}-E_a|\le B\ell_0^{-4}\). Subtract the two estimates and use (4). The two absolute-comparison errors contribute at most \(2C_{\rm st}\). No infrared mixing estimate enters, and the residual density need not be a Wilson density. ∎

**(P) Sufficient pointwise version.** For a probability reference measure, assume \(\rho\le e^{b_+N_R}\) everywhere, and \(\rho\ge e^{-b_-N_R}\) on a set of measure at least \(e^{-b_0N_R}\). Integration gives (8), with \(B=\max(b_+,b_-+b_0)\). For example, if that set contains a product of fixed Haar balls for at most \(cN_R\) coarse links, its measure is at least \(h^{cN_R}\), where \(h>0\) is the ball's Haar measure. ∎

**(P) Coarse seam alternative.** Suppose instead the exact remaining action, over a common normalized product reference measure, is a sum of uniformly bounded interactions of fixed range in coarse lattice units, with uniformly bounded incidence per site and identical recipes on both tori. Rewiring changes only interactions within that range of a seam: their count per physical volume is \(O((T_*\ell_0^3)^{-1})\). The two integrands have ratios between \(e^{-C N_{\rm seam}^{\rm coarse}}\) and \(e^{C N_{\rm seam}^{\rm coarse}}\); integration gives the same logarithmic bound. Since compatible \(T_*\ge\ell_0\), it is \(O(\ell_0^{-4})\). This proof assumes those coarse interaction bounds; it does not derive them from the number of variables. ∎

**(C) Necessary implementation conditions.** The RG runs \(K\sim\log_L(\ell_0/a)\) steps, not a fixed number. All effective couplings must remain in the admitted weak interval, with terminal parameters uniformly controlled; a lower bound on terminal coupling is sufficient when the lower-core estimate depends on its inverse. The question's weak-flow assumption must match these recursive couplings; a leading bare asymptotic alone would be weaker. An integer-scale cofinal sequence suffices for existence; all-cutoff S94 additionally needs the corresponding stopping-scale convention. A bounded number of coarse variables alone says nothing about their density or its normalization.

**(L) What Bałaban actually supplies.** [B122II, Theorem 1, p.355; (0.1), pp.355–356] bounds the full effective density above exponentially in coarse volume and below on a small-field set, with constants independent of depth \(k\), torus, and coarse field, assuming the effective couplings remain sufficiently small. [B119, Corollary 3, (2.50), p.264] gives integrated bounds, with dependence on terminal coupling. These are genuinely volume-uniform results.

**(L)** [B122II, p.356] leaves physical observables to further analysis. **(O)** The source lemma of §2 is an additional estimate, not an assertion already contained in that density theorem.

**(L) Which normalization is bounded.** [B109, (0.17), (0.19), pp.255–256; p.258] uses fluctuation normalizations evaluated at the identity configuration. [B119, paragraph before Theorem 1, p.262; p.279 following (3.47)] specifies the initial vacuum scalar by the finite-torus construction and subtracts newly generated \(E\)- and \(R''\)-values at identity. Uniform bounds after those subtractions do not by themselves identify one \(E_a\) in (8).

**(O) Remaining vacuum lemma — complete scalar compatibility.** For a verified exact native representation
\(Z_{a,R}=e^{A_a(R)}\Xi^{\rm native}_{a,R}\), with the native integrated bounds, prove
\[
\left|A_a(R)/V_R-E_a\right|\le C\ell_0^{-4}              \tag{9}
\]
for one \(E_a\), uniformly in \(a,R\). This is the missing implication here, not a claim that Bałaban's constants depend on volume.

**(C) A sufficient local formulation of (9).** At each physical scale \(s_j=aL^j\), require identical complete scalar recipes for carriers that lift without winding, and a bound on the remaining density error
\[
 C s_j^{-4}(1+r)^u
 \exp\!\left[-\frac{cT_*}{s_j(1+r)^v}\right],\qquad
 r=\log_L(\ell_0/s_j),                                 \tag{10}
\]
including Gaussian determinants, coordinate measures, nonlinear terms, and all \(R\)-history weights. Set \(E_a\) to the sum of the common bulk coefficients.

**(P) Summability proof.** Since \(s_j=\ell_0L^{-r}\), the sum in (10) is bounded by \(C\ell_0^{-4}\sum_{r\ge0}L^{4r}(1+r)^u e^{-c(T_*/\ell_0)L^r/(1+r)^v}\). Eventually \((1+r)^v\le L^{r/2}\); the resulting exponential beats every geometric factor, so the series converges independently of the cutoff and number of copies. This proves (9). ∎

**(L) Substantial published locality inputs exist.** [B99, Theorem 3.14, (3.154), pp.426–427] compares propagators for admissible regular backgrounds and domain sequences with exponential distance suppression. [B119, pp.278–279 after (3.47)] states interior-domain independence for localized \(E\) and \(R''\) terms; (3.34)–(3.38) localize a Gaussian log determinant in the regular fluctuation integral. [B116] supplies the small-field cluster expansion. **(O)** Closing the comparison for the **complete scalar** across ambient tori has not been established here. For the final \(R\) terms, specifically check equality under nonwinding embeddings of the normalized finite-region operations entering [B122II, (1.90)–(1.100)], including their coordinate maps, inherited activities, numerator/denominator integrals, and all identity values retained in the scalar normalization. Individual exponential bounds do not establish that equality.

**(P) Why “local” alone is insufficient.** Multiplying any local density by \(e^{c_R V_R}\) preserves its field dependence and normalized expectations but shifts pressure by arbitrary \(c_R\). Thus locality of field dependence cannot identify vacuum constants. ∎

**(C) Holonomies and renormalization.** The exact RG must retain torus holonomies, gauge projection, constrained measures, and every removed-zero-mode determinant factor. Keeping compact holonomies in the coarse integral is sufficient only if (8) bounds that actual integral. A finite number of modes can still carry cutoff-dependent normalization. Volume-independent renormalization is a hypothesis to implement, not a contradiction: **(L)** [B109, §5, (5.1), pp.292–293, and (5.16)] already uses an infinite-volume polarization prescription. Its announced SU(2) coupling-flow theorem is not an unconditional substitute: [B122II, p.355] explicitly retains the weak-coupling hypothesis because that proof had not been published there.

**(C) Resulting reduction.** A verified common scalar comparison plus the required observable bounds gives item 6's compactness without infrared mixing. Euclidean covariance then supplies reconstruction through Theorem A. Pure-phase selection and a nontrivial Yang–Mills component additionally require the energy/locality and identification inputs stated above. Calling the remaining task “RG with observables plus covariance” is accurate only if that RG package includes these precise obligations.

## 4. Arrow (v): what elementary comparisons and equivalent targets prove

### 4.1 Gluing and its surface cost

**(P)** Put \(n=t_*/a\), \(M=q^4\), with \(n,q\ge2\). Label \(M\) independent periodic blocks on the same Haar space as the large torus, and let \(\Delta S\) replace their seam plaquettes. For each of six orientations, the union of the two boundary-base layers has \(2n^3-n^2\) plaquettes. Hence
\[
N_{\rm seam}=M(12n^3-6n^2),\qquad
G:=M\log Z_*-\log Z_{q*}=-\log\mathbb E_0e^{-\beta\Delta S}.
\]
Every new seam plaquette contains an open path in an independently gauge-invariant block. Averaging a gauge transformation at its unmatched endpoint gives zero in the nontrivial fundamental representation. Therefore
\[
\mathbb E_0\operatorname{ReTr}U_p^{\rm new}=0,\quad
\mathbb E_0 S_p^{\rm new}=N,\quad
\mathbb E_0\Delta S=N_{\rm seam}(N-\bar s).
\]
The constant is \(N\), not 1, for the action in the question. Since \(|\Delta S|\le2NN_{\rm seam}\), or by Jensen, the resulting bound costs \(O(\beta/(t_*a^3))\) per physical volume. Even granting \(\bar s=O(\beta^{-1})\) does not remove that surface cost. ∎

**(P)** For \(d\mu_t\propto e^{-\beta(S_0+t\Delta S)}dU\), differentiation of the finite compact integral gives
\[
G=\beta\int_0^1\mathbb E_t\Delta S\,dt
=\beta\mathbb E_0\Delta S-D(\mu_0\Vert\mu_1)
=\beta\mathbb E_0\Delta S-\beta^2\int_0^1(1-t)\operatorname{Var}_t(\Delta S)dt. \tag{11}
\]
The last identity integrates \(d\mathbb E_t\Delta S/dt=-\beta\operatorname{Var}_t\Delta S\). Thus SV11 is exactly the signed cancellation \(G\le CV_{q*}\); an upper variance bound has the wrong sign to prove it. ∎

### 4.2 Why the transfer bound costs \(a^{-3}\log\beta\)

**(P)** On a transverse volume \(A\), there are \(E=3A/a^3\) spatial links. The unprojected Wilson transfer kernel has form
\(b(U)\prod_e k_\beta(U_eV_e^{-1})b(V)\), with
\(k_\beta(W)=e^{-\beta(N-\operatorname{ReTr}W)}\) and \(k_\beta(1)=1\).
A compact Lie group of dimension \(d_G\) has a cover by at most \(C(1+\beta)^{d_G/2}\) sets of diameter \(c(1+\beta)^{-1/2}\): use finitely many smooth coordinate charts and Euclidean cubes. On a common product cell the kernel product is at least \(e^{-c'E}\), by the quadratic Taylor bound on the plaquette action near identity.

**(P)** Among the \(Q\) product cells one carries \(\int_D b^2\ge\operatorname{Tr}T/Q\). The unit trial vector \(b1_D/\|b1_D\|_2\) gives
\(\|T\|\ge e^{-c'E}\operatorname{Tr}T/Q\).
A top eigenvector can be chosen nonnegative by replacing it by its absolute value in the Rayleigh quotient. Gauge averaging preserves its eigenvalue and is nonzero; therefore \(\|T_{\rm phys}\|=\|T\|\). Also \(\operatorname{Tr}T_{\rm phys}\le\operatorname{Tr}T\), and normalized eigenvalues lie in \([0,1]\). Thus, for any integer \(n\ge1\),
\[
\log\operatorname{Tr}\!\left[(T_{\rm phys}/\|T_{\rm phys}\|)^n\right]
\le\frac{3A}{a^3}\left[C+\frac{d_G}{2}\log(1+\beta)\right]. \tag{12}
\]
Division by \(t_*A\) gives the **one-direction** coefficient 3. Four enlargements give **12**, the actual coefficient in the spectral/purity estimate (8.11). ∎

### 4.3 Spectral count, overlap, and information

**(P)** Set \(K=T_{\rm phys}^{t_*/a}\), \(\widehat K=K/\|K\|\), and \(R=\operatorname{Tr}\widehat K\). Since its eigenvalues belong to \([0,1]\) and include 1,
\[
(1-1/q)\log R\le\log R-q^{-1}\log\operatorname{Tr}\widehat K^q\le\log R. \tag{13}
\]
Indeed \(1\le\operatorname{Tr}\widehat K^q\le R\). The middle expression divided by \(t_*A\) is the directional pressure gap. Four nonnegative directional gaps prove that S94 is equivalent, up to constants, to
\(\log R\le Ct_*A\) on the actual transverse family with zero through three sides enlarged. Conversely each gap is at most the isotropic gap; \(q/(q-1)\le2\). The reference transverse torus is covered at \(q=2\). This proves the SV16/(9.2) equivalence. ∎

**(P)** Define \(P=\operatorname{Tr}K^2/(\operatorname{Tr}K)^2\). Since
\(1\le\operatorname{Tr}\widehat K^2\le R\),
\[
\log R\le-\log P\le2\log R.                              \tag{14}
\]
Thus (9.6), \(P\ge e^{-Ct_*A}\), is equivalent. Its numerator is \(\int K(U,V)^2dUdV\) for the original symmetric kernel. If \(K=\sum_hK_h\), squaring includes every pair \(h,h'\); dropping cross terms changes the target. Theorem B therefore implies SV11, SV16 and (9.6), without separately proving their microscopic cancellations. ∎

**(P) Information inequality, not its converse.** Normalize a nonnegative symmetric half-slab kernel \(B\) by \(\operatorname{Tr}B^2=1\); put \(M=B^2\), \(J(x,z)=B(x,z)^2\), \(p(x)=\int J(x,z)dz\), \(p_x=J(x,\cdot)/p(x)\), \(I=D(J\Vert p\otimes p)\), and \(v=\sqrt p\). Jensen gives \(\int\sqrt{p_xp}\ge e^{-D(p_x\Vert p)/2}\). Hence
\[
e^{-I}\le\langle v,Mv\rangle
\le\|M\|_{\rm HS}=\sqrt{\operatorname{Tr}M^2}=\sqrt P,
\quad -\log P\le2I.                                    \tag{15}
\]
The middle inequality is Hilbert–Schmidt Cauchy–Schwarz with \(vv^*\). The replica identity follows as well:
\[
\int\sqrt{p_x(z)p_y(z)}\,dz
=\frac{(B^2)(x,y)}{\sqrt{p(x)p(y)}},\qquad
\mathbb E_{p\otimes p}\left[\int\sqrt{p_xp_y}\right]^2
=\operatorname{Tr}B^4=P.
\]
Zero-marginal rows are null. This proves the replica identities (48) and (50), retaining the essential square root in the latter's proof. ∎

**(P)** Bounded pressure/purity does not bound this information. Let
\(B_n=(\mathbf1\mathbf1^t/n+I_n/\sqrt n)/\sqrt{2+2/\sqrt n}\).
Its eigenvalues before normalization are \(1+n^{-1/2}\) and \(n^{-1/2}\), the latter \(n-1\) times. Consequently \(\operatorname{Tr}(B_n^2/\|B_n^2\|)\to2\) and \(\operatorname{Tr}B_n^4\to1/4\). The squared-entry joint distribution has uniform marginals and diagonal mass \(d_n=(1+n^{-1/2})/2\). Its relative entropy equals
\(d_n\log(nd_n)+(1-d_n)\log[n(1-d_n)/(n-1)]\), which is \((1/2+o(1))\log n+O(1)\). Thus (8)'s partition-function conclusion cannot imply a native-boundary \(I\) estimate. ∎

## 5. What HC and the underlying construction already provide

**(P) Gaussian comparison under explicit hypotheses.** Let real square matrices \(K_n,K_{qn}\) on the \(n^4\) and \((qn)^4\) periodic cells \(\Gamma_n,\Gamma_{qn}\) arise by periodizing one identical finite-range matrix recipe on a repeated background, including every coefficient and coordinate type. Assume range \(R\ge1\), at most \(d_0\) coordinates per cell, and singular values in \([m,M]\), uniformly. Put \(B_n=I-M^{-2}K_n^tK_n\), \(\rho=1-m^2/M^2<1\). Diagonalization and the convergent logarithm series give
\[
\log|\det K_n|=D_n\log M-\frac12\sum_{k\ge1}\operatorname{Tr}B_n^k/k.
\]
For \(k<k_0=1+\lfloor(n-1)/(4R)\rfloor\), every rooted walk has an identical injective lift to the larger torus. Normalized traces agree. Bounding the two remaining tails by their dimensions gives the per-cell estimate
\[
\left|\frac{\log|\det K_n|}{|\Gamma_n|}
-\frac{\log|\det K_{qn}|}{|\Gamma_{qn}|}\right|
\le\frac{d_0\rho^{k_0}}{k_0(1-\rho)}.
\]
The case \(\rho=0\) is immediate. Physical density introduces the additional factor \(s_j^{-4}\); summation over scales is §3's proof. ∎

**(C) Actual HC application.** This proves a matrix theorem, not identification of the entire Yang–Mills effective density with those matrices. The native clean Gaussian comparison in §110 depends on its CL/MB/MC hypotheses, including constrained coordinate identification and uniform right inverses. §111's scope is the clean current covariance and Gaussian normalizers. **(O)** It does not supply all nonlinear \(E/R\) births, common integration domains, transported history arguments, or their scalar normalizations.

| Node | Status |
|---|---|
| Present status | **(O)** S94 and full continuum construction remain open; mesoscopic comparison is not a fixed physical scale theorem. |
| Volume interface | **(C)** S94–S99: source transfer conditional on the vacuum bound. S102–S104 formulate an alternative source-zero stability route. |
| Pressure equivalence | **(C)** SV3–SV4 use the absolute stability premise; the native source response is a separate question. |
| Direct comparison | **(P)** Proofs above reproduce SV5–SV16, with the action normalization \(1\mapsto N\). **(O)** SV11/SV16 remain unproved in that derivation. |
| Spectral/purity route | **(P)** (8.11), (8.17), (9.1)–(9.8): verified implications, with coefficient 12 in (8.11). **(O)** (9.2)/(9.6) remain estimates to establish. |
| Replica route | **(P)** (47)–(51): original-kernel identity and (15). **(O)** No uniform \(I_m\) bound. |
| HC construction | **(C)** HC32–HC49, clean Gaussian construction. **(P)** V6.3–V6.11, matrix argument above. **(O)** V6.33: mixed/R measures, nonlinear admission, readouts/selectors, regular/R births, complete-state TD2/TD5 and terminal scalar control. |
| Compactness | **(C)** Proposition 32.1 and (123)–(128): compact coarse laws and reference-law noncollapse; physical insertions must be transported jointly. |
| Phase selection | **(C)** SC1–SC3: scalar theorem assumes physical two-point matching, full flat-test growth, and an actual-field energy bound. The absolute-vacuum obstruction also applies. |

## 6. Alternatives, pitfalls, and open questions

**(C) Finite-temperature free energy / spectral counting.** A uniform bound
\(A^{-1}\log\operatorname{Tr}e^{-t_*H_{a,\Sigma}}\le C\), with
\(H_{a,\Sigma}=-a^{-1}\log(T_{\rm phys}/\|T_{\rm phys}\|)\), proves S94 by (13). It is precisely the required thermal excess, not a consequence of finite-cutoff trace class. **(P)** Even a gap \(\Delta>0\) permits \(D_a\) excited states at that energy, giving trace \(1+D_ae^{-t_*\Delta}\); unbounded \(\log D_a/A\) defeats the target. ∎ **(O)** Finiteness separately on each continuum torus would still need uniformity over transverse sizes and a justified relation to cutoff partition functions.

**(L)** Faria da Veiga–O'Carroll, Theorems 1–3, (71)–(81), bound the scaled free energy per retained **fine lattice bond**, extracting a common leading singular factor but leaving distinct constants \(c_l,c_u\). Their displayed proof concentrates on \(U(N)\). **(P)** Even granting the indicated \(SU(N)\) extension, the interval's physical-density width is \((c_u-c_l)O(a^{-4})\), because fine bonds have density \(O(a^{-4})\). Thus these inequalities do not imply S94. Their scaled plaquette generating function is not automatically the renormalized physical \(\operatorname{Tr}F^2\) hierarchy. ∎

**(P) Which correlation inequality fails.** Universal nonnegative covariance for arbitrary Wilson-loop traces already fails for Haar \(SU(2)\). For eigenangles \(\pm\theta\), let
\(F=\operatorname{Tr}U^2=\chi_2-1\),
\(G=\operatorname{Tr}U^4=\chi_4-\chi_2\).
The characters \(\chi_j=\sin((j+1)\theta)/\sin\theta\) are orthonormal under \((2/\pi)\sin^2\theta\,d\theta\), by sine orthogonality. Thus \(\mathbb EF=-1\), \(\mathbb EG=0\), \(\mathbb EFG=-1\), and covariance is negative. At zero coupling these are twice- and four-times-traversed loop observables. This refutes an unrestricted Griffiths-type inference, not every restricted nonabelian correlation inequality. ∎

**(P) Limit order.** Theorem A uses one diagonal subsequence, so neither uniqueness nor interchange of \(a\to0\) and \(T\to\infty\) is required. Its proof does not give either: diagonal extraction only selects convergent coordinates. Estimates whose constants depend on \(T\) cannot be substituted in that proof. ∎

**(P) Trivial phases remain possible.** A probability mixture of constant fields \(\phi_c(f)=c\int f\), with bounded nonconstant random \(c\), has positive variance and reflection positivity: its OS quadratic form is the integral of a squared polynomial in \(c\). Every pure component is one-dimensional. Once the direct integral above is available, a positive reconstructed norm of a spatial translation difference excludes all components being constant: that difference vanishes in every constant component, while squared norms integrate. ∎

**(P) Generalized free phases remain possible.** For a massive free covariance \(C=(-\Delta+\mu^2)^{-1}\), \(\mu>0\), its reflected quadratic form is
\[
\int\frac{d^3p}{(2\pi)^3\,2\omega_p}
\left|\int_0^\infty e^{-\omega_p t}\widehat f(t,p)\,dt\right|^2\ge0,
\qquad \omega_p=\sqrt{|p|^2+\mu^2}.
\]
Wick's formula lifts this positivity to symmetric tensor powers and bounds each \(2k\)-point function by \((2k-1)!!\) products of covariance bounds. In massive free Fock space, sectorwise Cauchy–Schwarz gives
\(\|a(h)\psi\|\le\|h\|\|\mathsf N^{1/2}\psi\|\) and
\(\|a^*(h)\psi\|\le\|h\|\|(\mathsf N+1)^{1/2}\psi\|\).
Together with \(H\ge\mu\,\mathsf N\), these imply (2) with \(F_f(H)=(1+H)^{-1/2}\); truncating particle sectors proves the closure-domain inclusion. Every nonvacuum sector has energy at least \(\mu\), so the vacuum is unique. Finite positive sums of massive free covariances supply generalized free examples by the same construction. Also a mixture of centered Gaussian variables with conditional variance \(v\) has fourth cumulant \(3\mathbb E v^2-3(\mathbb E v)^2=3\operatorname{Var}(v)\). Thus these hypotheses, or a nonzero mixed-state fourth cumulant, do not force phasewise interaction. ∎

**(O)** Phasewise Yang–Mills identification remains separate. **(L)** Jaffe–Witten §4 requires the specified gauge-invariant operator and short-distance content, beyond an abstract scalar Wightman model [JW].

## 7. Primary sources and exact checking targets

The **(L)** entries identify the results used; **(O)** identifies a locator not verified here, not a negative theorem.

- **(L) [B99]** T. Bałaban, *Propagators for lattice gauge theories in a background field*, CMP **99** (1985), 389–434, [DOI](https://doi.org/10.1007/BF01240355). Theorems 3.9, 3.14; (3.107)–(3.108), (3.154): domain comparison.
- **(L) [B109]** Bałaban, *Renormalization group approach to lattice gauge field theories I*, CMP **109** (1987), 249–301, [DOI](https://doi.org/10.1007/BF01215223). (0.17), (0.19), Theorem 3; §5 (5.1), (5.16): normalization and coupling prescription. **(C)** Theorem 2, p.259, is the announced flow claim whose deferred proof is noted above.
- **(L) [B116]** Bałaban, *… II. Cluster expansions*, CMP **116** (1988), 1–22, [DOI](https://doi.org/10.1007/BF01239022). Completion of I's Theorem 3; §2 (2.38)–(2.41).
- **(L) [B119]** Bałaban, *Convergent renormalization expansions for lattice gauge theories*, CMP **119** (1988), 243–285, [DOI](https://doi.org/10.1007/BF01217741). Theorems 1–2, Corollary 3 (2.50); (3.34)–(3.47) and subsequent scalar subtractions.
- **(O) [B122I]** Bałaban, *Large field renormalization I*, CMP **122** (1989), 175–202, [DOI](https://doi.org/10.1007/BF01257412). The defining \(R\)-operation and mass-preservation/normalization formulas must be checked directly; the proposed locators (0.4), (1.102) are not verified here.
- **(L) [B122II]** Bałaban, *Large field renormalization II*, CMP **122** (1989), 355–392, [DOI](https://doi.org/10.1007/BF01238433). Theorem 1, (0.1), (1.90)–(1.102), pp.388–391: final \(R\) construction and stability after the native normalization.
- **(L) [OSl; Lü]** Osterwalder–Seiler, *Gauge field theories on a lattice*, Ann. Phys. **110** (1978), 440–471, [DOI](https://doi.org/10.1016/0003-4916(78)90039-8); Lüscher, CMP **54** (1977), 283–292, [DOI](https://doi.org/10.1007/BF01614090), Proposition 1, (17), (20)–(23). The former's strong-coupling infinite-volume result is not an asymptotically-free continuum theorem; exact transfer locators here use Lüscher.
- **(L) [FILS]** Fröhlich–Israel–Lieb–Simon, *Phase transitions and reflection positivity I*, CMP **62** (1978), 1–34, [DOI](https://doi.org/10.1007/BF01940327), Theorem 4.1; [primary preprint](https://repo-archives.ihes.fr/FONDS_IHES/I_Prepublications/FROHLICH/1978-1980/P_78_224/P_78_224_web.pdf).
- **(L) [OS; DS]** Osterwalder–Schrader I, CMP **31** (1973), 83–112, [DOI](https://doi.org/10.1007/BF01645738), Remark 3(b); II, CMP **42** (1975), 281–305, [DOI](https://doi.org/10.1007/BF01608978), §IV.1 (4.1). Driessler–Summers, Helv. Phys. Acta **59** (1986), 331–348, [DOI](https://doi.org/10.5169/seals-115699), Definitions 2.1–2.2, Theorem 2.3.
- **(L) [FVO; Dimock]** [arXiv:2205.07376v2](https://arxiv.org/abs/2205.07376), Theorems 1–4, especially (71)–(81). Dimock [1108.1335](https://arxiv.org/abs/1108.1335), Theorem 1, (7), and [1212.5562](https://arxiv.org/abs/1212.5562), Theorem 3.1, (201)–(205), concern scalar \(\phi^4_3\); I explicitly defers the proof of (7) to the final paper. These are normalization examples, not a four-dimensional nonabelian observable theorem.
- **(L) [JW]** Jaffe–Witten, [*Quantum Yang–Mills Theory*](https://www.claymath.org/wp-content/uploads/2022/06/yangmills.pdf), §4 and §6.5: required continuum content and scope of ultraviolet constructions.

## Consequences

**(C)** The fixed physical scale strategy suffices if exact renormalization expresses the Wilson partition function as a common bulk exponential times a coarse integral bounded above and below exponentially in coarse volume. **(P)** Taking logarithms, dividing by physical volume, and subtracting proves the pressure form of S94. A lower bound on a coarse set whose measure is bounded below exponentially suffices.

**(L)** Bałaban’s density estimates are uniform in renormalization depth and torus size under his weak coupling hypothesis [B122II, Theorem 1, (0.1)]. **(O)** This note does not establish that the complete finite torus scalar normalization differs from one common bulk density by a uniformly bounded physical density. Every Gaussian, nonlinear, and large field normalization must enter that comparison; locality estimates provide ingredients.

**(P)** Reflection positivity gives the pressure comparison with the reference torus in the required direction. **(C)** With reflected source geometry, compatible contacts, fixed volume source estimates, and S94, chessboard inequalities transfer local generating function bounds. Full mixed observable control remains necessary. **(P)** A fixed oscillator norm tensor estimate implies the joint test growth needed for reconstruction.

**(P)** Elementary gluing encounters fine boundary plaquettes whose expectation across independent blocks is \(N\) under the specified action. Transfer matrix covering replaces the linear coupling cost by a logarithm but retains the divergent boundary density. Spectral counting and two copy overlap are equivalent pressure targets. The information estimate is sufficient; its converse fails.

**(P)** Uniform bounds permit simultaneous subsequential limits without uniqueness or exchanging limits. **(L)** The corrected Osterwalder–Schrader axioms permit reconstruction without clustering [OS II, Remark 6, (4.1)]. Driessler–Summers requires additional hypotheses [DS, Theorem 2.3]. **(O)** Neither extraction nor decomposition excludes trivial or generalized free components. Scalar compatibility, physical observable bounds, phasewise Yang–Mills identification, and Euclidean covariance remain obligations. This note establishes conditional reductions, not Yang–Mills existence or a mass gap.
