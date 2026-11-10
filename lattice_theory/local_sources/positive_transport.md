# Positive transport, nonlinear remainders and admissible curvature

## Part I. Exact positive transport

**Scope.** This note completes the probability-theoretic transport mechanism used in the observable route ([Yang–Mills existence through observable derivatives](../observable_route.md)): one compatible positive history law, genuine reverse-martingale differences, orthogonality, depth-maximal bounds for fields and entire finite jets, admissible stopping/selection, and the fixed-law infinite-tail limit. It does not establish the spatial or coarse-scale estimates required by S2/M. Every cutoff factor in [Wilson tensor witnesses and large-field suppression](tensor_witnesses.md) remains explicit.

Compared with the per-level estimates of [Wilson tensor witnesses and large-field suppression](tensor_witnesses.md), the bounds below hold for a **maximum over all transport depths on one common probability space**, rather than separately under different output measures. That common lift also makes the additive variance budget genuinely orthogonal.

### 1. Exact hypotheses and a compatible common lift

Let \((E_k,\mathcal E_k)\), \(k=0,\ldots,J\), be standard Borel state spaces. The state may include any retained history variables needed to express a source-free operation as a kernel. Let \(\mu_k\) be the normalized positive measure at level \(k\). Assume each route transport is represented by a probability kernel
\[
K_k(y,dx),\qquad y\in E_{k+1},\ x\in E_k,
\]
such that
\[
\mathcal Q_k f(y)=\int f(x)K_k(y,dx),\qquad
\mu_{k+1}K_k=\mu_k.
\tag{PT1}
\]
These are precisely the conditional-expectation and expectation-preservation properties already supplied by the route's positive joint-law interpretation. A merely positive unital map without countable-additive kernel representation is not substituted for this hypothesis. Signed polymer activities are not kernels in (PT1).

Define the joint law on \(E_0\times\cdots\times E_J\) by
\[
d\mathbb P^{(J)}(x_0,\ldots,x_J)
=\mu_J(dx_J)K_{J-1}(x_J,dx_{J-1})\cdots K_0(x_1,dx_0).
\tag{PT2}
\]
It is a probability measure. Repeated use of \(\mu_{k+1}K_k=\mu_k\) shows that its \(k\)-th marginal is \(\mu_k\) and its adjacent-pair law is exactly
\[
\pi_k(dx_k,dx_{k+1})
=\mu_{k+1}(dx_{k+1})K_k(x_{k+1},dx_k).
\]
On standard Borel spaces, disintegration of this pair law also supplies a forward kernel \(R_k\) satisfying
\[
\mu_k(dx)R_k(x,dy)=\mu_{k+1}(dy)K_k(y,dx).
\tag{PT3}
\]
Thus the same common law can be realized as the forward Markov chain \(\mu_0R_0\cdots R_{J-1}\). This is a positive realization of the specified exact kernels; any extra construction history needed for their meaning belongs in the state spaces.

Let \(X_k\) denote the coordinate state, complete all sigma-algebras with respect to this one measure, and put
\[
\mathcal G_k=\sigma(X_k,X_{k+1},\ldots,X_J),\qquad
T_k=\mathcal Q_{k-1}\cdots\mathcal Q_0,\qquad T_0=I.
\]
The filtration is decreasing. Integrating the earlier coordinates in (PT2) proves, for every integrable initial observable \(F\),
\[
\boxed{M_k^F:=T_kF(X_k)=\mathbb E[F(X_0)\mid\mathcal G_k].}
\tag{PT4}
\]
The tower property then holds on one actual probability space. In particular \(\mathbb E[M_k^F\mid\mathcal G_{k+1}]=M_{k+1}^F\). Supremums over \(k\) below always refer to this common lift, not to independent drawings from the different marginals.

### 2. Orthogonal shell differences and the exact variance allocation

For \(F\in L^2(\mu_0)\), define
\[
\Delta_k^F=M_k^F-M_{k+1}^F,\qquad k<J.
\]
Then \(\Delta_k^F\) is \(\mathcal G_k\)-measurable and
\[
\mathbb E[\Delta_k^F\mid\mathcal G_{k+1}]=0.
\tag{PT5}
\]
If \(k<\ell\), then \(\Delta_\ell^G\) and \(M_J^G\) are measurable with respect to \(\mathcal G_{k+1}\). Consequently
\[
\mathbb E[\Delta_k^F\Delta_\ell^G]=0,
\qquad
\mathbb E[\Delta_k^F M_J^G]=0.
\]
This is genuine orthogonality on the common history lift. The exact decomposition is
\[
F(X_0)-\mathbb EF
=\sum_{k<J}\Delta_k^F+(M_J^F-\mathbb EF),
\]
and
\[
\operatorname{Var}_{\mu_0}F
=\sum_{k<J}\mathbb E|\Delta_k^F|^2
+\operatorname{Var}_{\mu_J}(T_JF).
\tag{PT6}
\]

For two real marks, the route's shell kernel
\[
D_k^{FG}
=\mathcal Q_k[(T_kF)(T_kG)]-(T_{k+1}F)(T_{k+1}G)
\]
satisfies the stronger conditional identity
\[
\boxed{D_k^{FG}(X_{k+1})
=\mathbb E[\Delta_k^F\Delta_k^G\mid\mathcal G_{k+1}].}
\tag{PT7}
\]
To verify it, use the conditional law \(K_k(X_{k+1},dx_k)\) of \(X_k\) given its entire future and expand the product of the two differences. The cross terms are exactly the products of the conditional means.

For a finite vector of observables, the matrix \(D_k\) is the conditional covariance matrix of the corresponding reverse-martingale increment. Thus it is positive semidefinite, and the matrix identity
\[
\operatorname{Cov}_{\mu_0}(F)
=\sum_{k<J}\mathbb E D_k+\operatorname{Cov}_{\mu_J}(T_JF)
\]
holds in the positive-semidefinite order as well as entrywise. The absolute covariance estimate of [Wilson tensor witnesses and large-field suppression](tensor_witnesses.md) follows again:
\[
\sum_{k<J}\mathbb E|D_k^{FG}|
+|\operatorname{Cov}_{\mu_J}(T_JF,T_JG)|
\le\sqrt{\operatorname{Var}F\operatorname{Var}G}.
\tag{PT8}
\]

#### Coarser-measurable selectors

If \(a_k\) is real and \(\mathcal G_{k+1}\)-measurable and \(|a_k|\le1\), then \(a_k\Delta_k^F\) remains a reverse-martingale difference. Its cross terms with every differently indexed such difference vanish. Therefore
\[
\boxed{\mathbb E\left|\sum_{k<J}a_k\Delta_k^F\right|^2
=\sum_{k<J}\mathbb E[a_k^2|\Delta_k^F|^2]
\le\operatorname{Var}F.}
\tag{PT9}
\]
This permits bounded selections depending on the coarser output/history. Applying it to a specific selector requires checking that measurability. An arbitrary fine-field-dependent selector cannot be declared predictable.

### 3. A self-contained maximal inequality

For finite \(J\), reverse the filtration: \(\mathcal H_j=\mathcal G_{J-j}\), \(0\le j\le J\). For nonnegative integrable \(Y\), let \(Z_j=\mathbb E[Y\mid\mathcal H_j]\), and let \(Z^*=\max_{j\le J}Z_j\).

For \(\lambda>0\), partition \(\{Z^*\ge\lambda\}\) by the first crossing time. Each event \(A_j\) lies in \(\mathcal H_j\), so
\[
\lambda\mathbb P(Z^*\ge\lambda)
\le\sum_j\mathbb E[\mathbf1_{A_j}Z_j]
=\mathbb E[Y\mathbf1_{\{Z^*\ge\lambda\}}]
\le\mathbb EY.
\tag{PT10}
\]
For \(p>1\), integrate the stronger middle inequality against \(p\lambda^{p-2}\,d\lambda\). Fubini and Hölder give
\[
\mathbb E(Z^*)^p
\le\frac p{p-1}\mathbb E[Y(Z^*)^{p-1}]
\le\frac p{p-1}\|Y\|_p\|Z^*\|_p^{p-1}.
\]
Hence
\[
\boxed{\left\|\max_{k\le J}|T_kF(X_k)|\right\|_p
\le\frac p{p-1}\|F\|_p,\qquad p>1.}
\tag{PT11}
\]
For a signed or complex \(F\), use \(|T_kF|\le T_k|F|\). The proof is independent of \(J\), of whether a step is an ordinary integration or a positive R operation, and of changes in state-space dimension.

#### 3.1 A depth-maximal exponential envelope

Suppose \(R\ge0\) and
\[
\mathbb E e^{R/\tau}\le e^A,\qquad A\ge0.
\]
Let \(R_k=T_kR(X_k)\). Conditional Jensen gives \(e^{R_k/\tau}\le T_ke^{R/\tau}(X_k)\). Apply (PT10) to the positive martingale of conditional exponential moments. For every \(t\ge0\),
\[
\boxed{\mathbb P\left(\max_{k\le J}R_k>\tau(A+t)\right)\le e^{-t}.}
\tag{PT12}
\]
In particular,
\[
\boxed{\left\|\max_{k\le J}R_k\right\|_m
\le\tau\bigl[A+(m!)^{1/m}\bigr]
\le\tau(A+m),\qquad m\ge1\text{ an integer}.}
\tag{PT13}
\]
This follows by integrating the exponential tail of \((\max R_k/\tau-A)_+\), then applying Minkowski. There is no union-bound factor counting levels.

For the normalized special case \(A=1,\tau=\sigma\), one also has
\[
\mathbb E e^{\theta\max R_k/\sigma}\le\frac{e^\theta}{1-\theta},
\qquad 0<\theta<1.
\tag{PT14}
\]
Indeed use \(\mathbb P(\max R_k/\sigma>u)\le\min\{1,e^{1-u}\}\) in the tail-integral formula. For example the same \(e\)-bounded exponential norm survives the maximum after enlarging the scale by a factor 3: \(\mathbb E e^{\max R_k/(3\sigma)}\le\frac32e^{1/3}<e\).

#### 3.2 Application with the actual Wilson constants

[Wilson tensor witnesses and large-field suppression](tensor_witnesses.md) proves the unscaled moment-generating estimate
\[
\mathbb E\exp\left(\frac{\beta a^4}{96}q_W(z)\right)\le e^{K_\beta-1},
\qquad K_\beta\ge1,
\]
directly from its cube exponential theorem and convexity over the 24 incident plaquettes. The centered family is dominated by
\[
R_a(z)=q_W(z)+\frac{\mathbb E q_W(z)}6.
\]
Put \(\tau_0=96/(\beta a^4)\), \(\tau_\circ=112/(\beta a^4)=7\tau_0/6\). Jensen gives \(\mathbb E q_W\le\tau_0(K_\beta-1)\). Hölder/concavity at exponent \(6/7\) therefore yields
\[
\mathbb E e^{R_a/\tau_\circ}
\le\exp[(K_\beta-1)/7]\left(\mathbb E e^{q_W/\tau_0}\right)^{6/7}
\le e^{K_\beta-1}\le e^{K_\beta}.
\tag{PT15}
\]
For the whole tensor family at a fixed site, \(|\Phi_{k,AB}(z)|\le T_kR_a(z)\), so
\[
\boxed{\mathbb P\left(\max_{k\le J}\max_{A,B}|\Phi_{k,AB}(z)|
>\frac{112(K_\beta+t)}{\beta a^4}\right)\le e^{-t},}
\tag{PT16}
\]
and
\[
\boxed{\left\|\max_{k\le J}\max_{A,B}|\Phi_{k,AB}(z)|\right\|_m
\le\frac{112(K_\beta+m)}{\beta a^4}.}
\tag{PT17}
\]
Thus the earlier per-level numerical bound now controls the depth maximum as well. The 21 labels incur no separate factor because a single positive scalar dominates them all. The raw positive matrix entries obey the corresponding 96 bound.

### 4. Bad-event posteriors over all depths and adaptive marked estimates

For an initial event \(B\) with probability \(p_B\), let
\[
b_k=T_k\mathbf1_B(X_k)=\mathbb P(B\mid\mathcal G_k).
\]
The weak maximal inequality gives
\[
\boxed{\mathbb P\left(\max_{k\le J}b_k\ge\lambda\right)
\le\min\{1,p_B/\lambda\},\qquad 0<\lambda\le1.}
\tag{PT18}
\]
This is a uniform bound for a single history ever assigning posterior probability at least \(\lambda\) to the initial bad event. It is not a claim that different RG-scale bad events are one event.

Let \(H_i^*=\max_k\max_{A,B}|\Phi_{k,AB}(z_i)|\). Cauchy–Schwarz and Hölder give
\[
\mathbb E\left[\prod_{i=1}^mH_i^*\,
\mathbf1_{\{\max_k b_k\ge\lambda\}}\right]
\le\prod_i\|H_i^*\|_{2m}\sqrt{p_B/\lambda}.
\]
For a prescribed microscopic carrier \(\Gamma\), [Wilson tensor witnesses and large-field suppression](tensor_witnesses.md) gives \(p_B\le e^{-\kappa|\Gamma|}\), hence
\[
\boxed{\mathbb E\left[\prod_{i=1}^mH_i^*\,
\mathbf1_{\{\max_k b_k\ge\lambda\}}\right]
\le\left[\frac{112(K_\beta+2m)}{\beta a^4}\right]^m
\lambda^{-1/2}e^{-\kappa|\Gamma|/2}.}
\tag{PT19}
\]
The indicators and the marks may be inspected at arbitrary history-dependent depths; the maxima cover that selection. The event remains the posterior of the original microscopic carrier. Identifying actual coarse R selectors with such controlled probabilities remains a dynamical/geometric task.

### 5. The entire finite-log-jet hierarchy has depth-maximal bounds

Let \(F_1,\ldots,F_m\) be initial marks satisfying
\[
\mathbb E e^{|F_i|/\sigma_i}\le e.
\tag{PT20}
\]
At level \(k\), use distinct formal labels and define the finite jet
\[
\Psi_k(t)=\log T_k\exp\Bigl(\sum_i t_iF_i\Bigr).
\]
Its mixed coefficient is the conditional cumulant
\[
\Psi_k^I
=\sum_{\pi\in\Pi_m}(-1)^{|\pi|-1}(|\pi|-1)!
\prod_{B\in\pi}T_k\Bigl(\prod_{i\in B}F_i\Bigr).
\tag{PT21}
\]
The coefficient of \(t_1\cdots t_m\) is the mixed derivative, with no extra factorial, because the labels are distinct.

Let
\[
A_m=\sum_{\pi\in\Pi_m}(|\pi|-1)!\le2^{m-1}m!,
\qquad N_{i,k}=T_k|F_i|^m(X_k).
\]
The combinatorial bound follows by counting ordered partitions by positive ordered block sizes and using \(m!/(n_1!\cdots n_r!)\le m!\). Conditional Hölder gives the pointwise estimate
\[
|\Psi_k^I(X_k)|\le A_m\prod_{i=1}^mN_{i,k}^{1/m}.
\tag{PT22}
\]
For any \(p>1\), Hölder followed by (PT11) yields
\[
\boxed{\left\|\max_{k\le J}|\Psi_k^I(X_k)|\right\|_p
\le\frac p{p-1}A_m\prod_{i=1}^m\|F_i\|_{mp}.}
\tag{PT23}
\]
Indeed the \(L^p\) norm of \(\prod_i(\max_kN_{i,k})^{1/m}\) is at most \(\prod_i\|\max_kN_{i,k}\|_p^{1/m}\), and the factors are positive reverse martingales with terminal variable \(|F_i|^m\).

The exponential hypothesis gives \(\mathbb E|F_i|^r\le e\,\Gamma(r+1)\sigma_i^r\). For an integer \(p\ge2\), use the multinomial bound \((mp)!/(m!)^p\le p^{mp}\) to obtain
\[
\boxed{\left\|\max_{k\le J}|\Psi_k^I(X_k)|\right\|_p
\le\frac p{p-1}e^{1/p}2^{m-1}p^m(m!)^2\prod_i\sigma_i.}
\tag{PT24}
\]
In particular, the useful \(p=2\) statement is
\[
\boxed{\left\|\max_{k\le J}|\Psi_k^I(X_k)|\right\|_2
\le\sqrt e\,4^m(m!)^2\prod_i\sigma_i.}
\tag{PT25}
\]
It also bounds the \(L^1\) norm of the maximum. For the centered Wilson tensor entries one may take every \(\sigma_i=112K_\beta/(\beta a^4)\), including repeated sites or labels.

These bounds control whole conditional jet coefficients after their partition terms have been assembled. They do not control the sum of absolute values of localized signed polymer terms. Extra source counterterms must be incorporated into the initial jet if a renormalization prescription introduces them.

### 6. Stopping and selection: exact conservation versus maximal control

On the finite reversed filtration \(\mathcal H_j=\mathcal G_{J-j}\), let \(\tau\) be a bounded stopping time. Put \(\kappa=J-\tau\). Equivalently,
\[
\{\kappa\ge k\}\in\mathcal G_k\quad\text{for every }k.
\tag{PT26}
\]
The stopped sigma-algebra \(\mathcal H_\tau\) has the usual piecewise measurability property. For any integrable initial \(F\), partitioning by \(\{\tau=j\}\) and using conditional expectations proves
\[
M_\kappa^F=\mathbb E[F(X_0)\mid\mathcal H_\tau].
\tag{PT27}
\]
Therefore expectation preservation, matrix positivity, and Jensen hold at such a stopped history level, with the same initial-law constants. Raw moment conservation refers specifically to \(\mathbb E[T_\kappa(F_1\cdots F_m)(X_\kappa)]=\mathbb E[F_1\cdots F_m]\), applying (PT27) to that initial product. It does not assert conservation of the expectation of \(\prod_iT_\kappa F_i\) or of a higher conditional cumulant. No optional-stopping theorem beyond this finite partition identity is needed.

An arbitrary path-measurable choice of depth need not satisfy (PT26), so its expectation need not be preserved. Nevertheless (PT12), (PT17), (PT19), and (PT25) apply to its selected fields and jets because their absolute values are bounded by the proved maxima. This distinction prevents an adaptive selection from silently being treated as another exact transport.

### 7. A fixed-law infinite-depth completion

Assume now that the spaces, measures and kernels in (PT1) are specified for every \(k\ge0\). This is one compatible infinite chain with a fixed initial law; it is not a sequence of different cutoff theories.

The finite laws (PT2) are consistent: integrating the last coordinate of the depth-\(J+1\) law replaces \(\mu_{J+1}K_J\) by \(\mu_J\), giving exactly the depth-\(J\) law. The standard countable extension of probability measures on standard Borel product spaces yields a common infinite law. The equivalent construction uses the forward kernels (PT3).

Set \(\mathcal G_k=\sigma(X_k,X_{k+1},\ldots)\), completed, and \(\mathcal G_\infty=\bigcap_k\mathcal G_k\). Equation (PT4) holds first against every bounded finite future-cylinder function and then against all bounded \(\mathcal G_k\)-measurable functions by the monotone-class argument.

For every \(F\in L^2(\mu_0)\),
\[
\boxed{M_k^F\longrightarrow M_\infty^F
=\mathbb E[F(X_0)\mid\mathcal G_\infty]
\quad\text{almost surely and in }L^2.}
\tag{PT28}
\]
Here is a proof using only the maximal estimate already established. Let \(P_k\) denote conditional projection onto \(L^2(\mathcal G_k)\). For \(j\ge k\), nested projections give
\[
\|P_kF-P_jF\|_2^2=\|P_kF\|_2^2-\|P_jF\|_2^2.
\]
The right side tends to zero because the squared norms decrease. Thus \(P_kF\) has an \(L^2\) limit lying in every closed subspace \(L^2(\mathcal G_k)\). Orthogonality identifies it with \(P_\infty F\). Apply the finite maximal bound to \(P_nF-P_\infty F\) on the decreasing block \(n,\ldots,J\), and then let \(J\) increase:
\[
\mathbb E\sup_{k\ge n}|P_kF-P_\infty F|^2
\le4\|P_nF-P_\infty F\|_2^2\longrightarrow0.
\]
The tail supremums decrease with \(n\), so their limit is zero almost surely. This proves (PT28).

For every finite \(p\ge1\), the analogous \(L^p\) and almost-sure convergence follows by approximating \(F\) by bounded truncations. Conditional expectations contract in \(L^p\); the weak maximal bound applied to the absolute truncation error makes the probability of an uncontrolled tail at most its \(L^1\) norm divided by the threshold. Letting the truncation level increase completes the argument.

The orthogonal series and covariance identity become
\[
F(X_0)-\mathbb EF
=\sum_{k\ge0}\Delta_k^F+(M_\infty^F-\mathbb EF),
\]
with convergence in \(L^2\) and almost surely in its displayed order, and
\[
\operatorname{Cov}(F,G)
=\sum_{k\ge0}\mathbb E[\Delta_k^F\Delta_k^G]
+\operatorname{Cov}(M_\infty^F,M_\infty^G).
\tag{PT29}
\]
The covariance series is absolutely convergent. Also \(\sum_k|\Delta_k^F|^2<\infty\) almost surely because its expectation is finite. The terminal contribution is the tail covariance; it vanishes if the relevant tail conditional expectations are constants, not merely because the kernels are positive.

#### 7.1 Every finite jet has a tail limit

If the initial marks have the exponential moments (PT20), each product \(\prod_{i\in B}F_i\) belongs to every finite \(L^p\). Its conditional moment converges by (PT28) and its \(L^p\) extension. A finite conditional cumulant is a polynomial in these finitely many conditional moments, so
\[
\Psi_k^I\longrightarrow
\kappa(F_i:i\in I\mid\mathcal G_\infty)
\]
almost surely and in every finite \(L^p\). The depth-maximal bounds (PT24) provide the required uniform integrability; for a desired \(L^p\) limit one may use a larger integer moment. A countable initial family and all its finite label sets can be treated on one common full-measure event.

This closes the exact positive-transport algebra and its fixed-law limit. It does not identify the tails for Yang–Mills or compare different initial cutoff measures.

## Part II. a full-law nonlinear observable remainder

**Status.** The theorem below is exact at finite cutoff for the actual SU(N) Wilson measure. It closes a concrete local nonlinear observable remainder: replacing the Wilson-compatible tensor multiplet by a multiplet quadratic in its 24 local sine-plaquette variables has an explicit small error in the microscopic factorial norms. It does not replace the Wilson probability law by a Gaussian law or estimate the whole nonlinear RG interaction remainder.

### 1. The global SU(N) quartic remainder

Let
\[
s(U)=N-\operatorname{ReTr}U,\qquad
H(U)=\pi_0\frac{U-U^\dagger}{2i},\qquad
\pi_0 A=A-\frac{\operatorname{Tr}A}{N}I.
\]
Thus \(H(U)\) is traceless Hermitian. Put
\[
R(U)=s(U)-\frac12\|H(U)\|_{\mathrm{HS}}^2.
\]

**Proposition 1.** For every \(U\in SU(N)\),
\[
\boxed{0\le R(U)\le C_N s(U)^2,}
\tag{N1}
\]
where one explicit admissible constant is
\[
L_N=\sum_{r=2}^N\binom Nr2^{r-2}
=\frac{3^N-1-2N}{4},\qquad
C_N=\frac12+\frac{2L_N^2}{N}.
\tag{N2}
\]
The constants are deliberately not optimized.

**Proof.** Choose eigenangles \(\theta_j\) of \(U\). The exact identity is
\[
R(U)=\frac12\sum_{j=1}^N(1-\cos\theta_j)^2
+\frac{(\operatorname{ImTr}U)^2}{2N}.
\tag{N3}
\]
Indeed \(\|H(U)\|^2=\sum_j\sin^2\theta_j-(\sum_j\sin\theta_j)^2/N\), and
\((1-\cos\theta)-\tfrac12\sin^2\theta=\tfrac12(1-\cos\theta)^2\). This proves nonnegativity.

To bound the second term globally without defining a logarithmic field, write \(A=U-I\). Since \(\det U=1\), the elementary-symmetric expansion of the determinant gives
\[
\operatorname{Tr}A=-\sum_{r=2}^N e_r(A).
\]
Normality of \(A\), \(\|A\|_{\mathrm{op}}\le2\), and the elementary coefficient bound imply
\[
|e_r(A)|\le\binom Nr\|A\|_{\mathrm{op}}^r
\le\binom Nr2^{r-2}\|A\|_{\mathrm{HS}}^2.
\]
Thus
\[
|\operatorname{ImTr}U|
\le|\operatorname{Tr}A|\le L_N\|A\|_{\mathrm{HS}}^2=2L_N s(U).
\]
Also \(\sum_j(1-\cos\theta_j)^2\le s(U)^2\). Substitution in (N3) proves (N1). No branch choice or exceptional set is used. \(\square\)

The SU(N) condition is relevant: projection onto traceless matrices can remove a first-order U(1) curvature, so this precise remainder statement is not automatically a U(N) statement with the same projected field.

### 2. Splitting the scalar correction into two positive pieces

Use the exact definitions from [Wilson tensor witnesses and large-field suppression](tensor_witnesses.md). For each of the six planes \(A=(\mu,\nu)\) and four signed leaves, put
\[
Y_{A,\epsilon,\delta}(z)
=a^{-2}\epsilon\delta H(P_{\epsilon e_\mu,\delta e_\nu}(z)),
\qquad F_A^C(z)=\frac14\sum_{\epsilon,\delta}Y_{A,\epsilon,\delta}(z).
\]
Define
\[
q_{\rm leaf}(z)=\sum_A\frac14\sum_{\epsilon,\delta}
\|Y_{A,\epsilon,\delta}(z)\|_{\mathrm{HS}}^2,
\qquad q_C(z)=\sum_A\|F_A^C(z)\|_{\mathrm{HS}}^2.
\tag{N4}
\]
This has the same engineering dimension as \(q_W\). The exact Hilbert-space variance identity gives
\[
\boxed{q_{\rm leaf}(z)-q_C(z)
=\sum_A\frac14\sum_{\epsilon,\delta}
\|Y_{A,\epsilon,\delta}(z)-F_A^C(z)\|_{\mathrm{HS}}^2\ge0.}
\tag{N5}
\]
On the other hand, the new nonlinear residual is
\[
D(z)=q_W(z)-q_{\rm leaf}(z)
=\frac1{2a^4}\sum_{p\ni z}R(U_p).
\tag{N6}
\]
Here the sum contains the 24 ordinary plaquettes incident on \(z\), based and oriented at \(z\); trace quantities are unchanged by that rebasing. Proposition 1 gives
\[
\boxed{0\le D(z)\le\frac{C_N}{2a^4}\sum_{p\ni z}s_p^2
\le2C_Na^4q_W(z)^2.}
\tag{N7}
\]
The last inequality uses \(\sum_{p\ni z}s_p=2a^4q_W(z)\). Also \(D\le q_W\). Consequently
\[
q_W-q_C=D+(q_{\rm leaf}-q_C)
\]
is an exact decomposition into a controlled nonlinear term and a leaf-variation term.

### 3. An entire quadratic tensor multiplet

Let \(Q^C_{AB}=\operatorname{Tr}(F_A^CF_B^C)\). Define
\[
\boxed{Q^{\rm leaf}_{AB}(z)
=Q^C_{AB}(z)+\frac{\delta_{AB}}6\,[q_{\rm leaf}(z)-q_C(z)].}
\tag{N8}
\]
Every entry is a quadratic polynomial in the 24 local Hermitian variables \(Y_{A,\epsilon,\delta}\). The exact properties are
\[
Q^{\rm leaf}\succeq0,\qquad
\operatorname{tr}_6Q^{\rm leaf}=q_{\rm leaf}\le q_W,\qquad
|Q^{\rm leaf}_{AB}|\le q_W,
\tag{N9}
\]
\[
\boxed{Q^W_{AB}-Q^{\rm leaf}_{AB}=\frac{\delta_{AB}}6D.}
\tag{N10}
\]
The construction preserves all 21 components, the local stencil, gauge invariance, full hypercubic covariance and the tensor reflection action. These follow from the same exact geometric transformation of the leaves as in [Wilson tensor witnesses and large-field suppression](tensor_witnesses.md). In particular the two multiplets agree in all nonscalar channels. The replacement affects only the scalar representation.

The word *quadratic* here describes the observable's dependence on these sine-plaquette variables. Their joint Wilson distribution is interacting and is not made Gaussian by the definition.

### 4. Full-law bounds on the nonlinear remainder

All expectations are under the complete normalized Wilson law at \(\beta=2Nx_0\ge1\). Use the proved preceding estimate
\[
\|s_p\|_m\le\frac{8(K_\beta+m)}\beta,
\qquad
\mathbb E e^{q_W(z)/\sigma_{\beta,a}}\le e,
\qquad
\sigma_{\beta,a}=\frac{96K_\beta}{\beta a^4},
\tag{N11}
\]
with \(K_\beta=C_G+2(N^2-1)\log\beta\ge1\).

Taking the \(L^m\) norm of (N6) and using (N1) yields, for integers \(m\ge1\),
\[
\boxed{\|D(z)\|_m
\le768C_Na^{-4}\left(\frac{K_\beta+2m}{\beta}\right)^2.}
\tag{N12}
\]
The factor follows from 24 leaves, the prefactor \(1/(2a^4)\), and \(\|s_p^2\|_m=\|s_p\|_{2m}^2\). This is a volume-uniform, unconditioned estimate. No removal of a bad set was needed.

For the tensor residual, set
\[
\alpha_N=C_N/3,\qquad
\varepsilon_\beta=\alpha_Na^4\sigma_{\beta,a}
=\frac{32C_NK_\beta}{\beta}.
\tag{N13}
\]
Equations (N7) and (N10) imply, componentwise,
\[
|Q^W_{AB}-Q^{\rm leaf}_{AB}|
\le\alpha_Na^4q_W^2.
\tag{N14}
\]
The parameter \(\varepsilon_\beta\) tends to zero at weak coupling because \(K_\beta=O(1+\log\beta)\).

#### 4.1 Products at arbitrary sites, including coincidences

For any \(m\) sites and component labels, telescope the difference of products. Each summand contains one residual bounded by (N14), and the other fields are bounded by their corresponding \(q_W\) envelopes. The total envelope degree is \(m+1\). Hölder with weights \(2/(m+1)\) at the residual and \(1/(m+1)\) at each other mark gives
\[
\mathbb E\left[q_W(z_r)^2\prod_{i\ne r}q_W(z_i)\right]
\le e\,(m+1)!\,\sigma_{\beta,a}^{m+1}.
\]
Therefore
\[
\boxed{\mathbb E\left|
\prod_{i=1}^m Q^W_i-\prod_{i=1}^m Q^{\rm leaf}_i\right|
\le e\,m(m+1)!\,\varepsilon_\beta\sigma_{\beta,a}^m.}
\tag{N15}
\]
Here each \(Q_i\) denotes its selected component at its selected point. There is no separation assumption and the same bound holds if points coincide.

#### 4.2 Connected coefficients have a small remainder with one fixed factorial exponent

The cumulant is multilinear, so telescope the field replacement inside it. In a partition term, let the block containing the residual have size \(b\). Its moment is bounded by
\(\alpha_Na^4 e(b+1)!\sigma^{b+1}\); all other block moments are bounded by \(e|B|!\sigma^{|B|}\). Since \(b+1\le m+1\), the weighted partition identity from [Wilson tensor witnesses and large-field suppression](tensor_witnesses.md) gives
\[
\boxed{
|\kappa_m(Q^W_1,\ldots,Q^W_m)-\kappa_m(Q^{\rm leaf}_1,\ldots,Q^{\rm leaf}_m)|
\le\varepsilon_\beta(m+1)m!\big[(1+e)^m-1\big]\sigma_{\beta,a}^m.}
\tag{N16}
\]
To check the count, for \(r\) blocks,
\[
\sum_{|\pi|=r}\prod_{B\in\pi}|B|!
=\frac{m!}{r!}\binom{m-1}{r-1},
\]
and the partition sum with cumulant coefficient \((r-1)!\) equals
\((m-1)![(1+e)^m-1]\). The additional factors are the \(m\) possible residual locations and the upper bound \(m+1\) for its enlarged block factorial.

At connected orders \(m\ge2\), deterministic identity subtractions leave both sides' cumulants unchanged. Thus (N16) is also the replacement estimate for the separately centered fields.

For each fixed order, the dimensionless plaquette marks \(\beta a^4Q\) obey
\[
|\Delta\kappa_m(\beta a^4Q)|
\le C_{N,m}\frac{K_\beta^{m+1}}\beta\longrightarrow0
\quad(\beta\to\infty).
\tag{N17}
\]
The analogous product statement follows from (N15). These are microscopic dimensionless normalizations, not an identification with a prescribed physical running field \(Z_aQ\).

There is also a uniform all-order formulation in the microscopic factorial norm:
\[
\sup_{m\ge1}
\frac{|\Delta\kappa_m|}{m![2(1+e)\sigma_{\beta,a}]^m}
\le\varepsilon_\beta,
\tag{N18}
\]
because \((m+1)/2^m\le1\) for all \(m\ge1\). This makes the fixed factorial budget explicit.

#### 4.3 Marked bad-set version

Let \(B_\Gamma\) be a prescribed microscopic bad-cube event with
\(\mu_\beta(B_\Gamma)\le e^{-\kappa|\Gamma|}\), as in the preceding theorem. Apply Cauchy–Schwarz to each telescoping summand and Hölder at total doubled envelope degree \(2(m+1)\). Since
\(\sqrt{(2m+2)!}\le2^{m+1}(m+1)!\),
\[
\mathbb E\left[\left|\prod_iQ_i^W-\prod_iQ_i^{\rm leaf}\right|
\mathbf1_{B_\Gamma}\right]
\le\sqrt e\,m2^{m+1}(m+1)!\,
\varepsilon_\beta\sigma_{\beta,a}^m e^{-\kappa|\Gamma|/2}.
\tag{N19}
\]
Thus the small nonlinear remainder can be combined with the actual full-law microscopic large-field suppression without requiring independence.

### 5. Propagation through every exact positive transport

Let \(T_k\) denote the composition of the route's normalized positive kernels, all acting under the same original Wilson law. Transport both alternative observable families with this same frozen kernel:
\[
Q^W_{k,i}=T_kQ^W_i,\qquad Q^{\rm leaf}_{k,i}=T_kQ^{\rm leaf}_i,
\qquad D_k=T_kD.
\]
Then
\[
Q_k^W-Q_k^{\rm leaf}=I_6D_k/6\succeq0,
\qquad \|D_k\|_m\le\|D\|_m.
\tag{N20}
\]
The same full-law error bound (N12) therefore holds at every positive history level, with no depth loss.

Both (N15) and (N16) remain valid for the **individually transported marks** under \(\mu_k\). For a summand with a residual at \(r\), positivity gives
\[
|Q^W_{k,r}-Q^{\rm leaf}_{k,r}|
\le\alpha_Na^4 T_k(q_r^2),\qquad |Q^W_{k,i}|,|Q^{\rm leaf}_{k,i}|\le T_kq_i.
\]
Hölder exponents \((m+1)/2\) and \(m+1\), followed by conditional-expectation contraction, bound the product expectation by
\[
\alpha_Na^4\|q_r^2\|_{(m+1)/2}\prod_{i\ne r}\|q_i\|_{m+1}
\le\alpha_Na^4 e(m+1)!\sigma^{m+1}.
\]
The blockwise cumulant proof is identical. Notice that no incorrect inequality \(T_kq^2\le(T_kq)^2\) is used.

#### 5.1 Entire logarithmic-jet replacement

Define the whole finite jets
\[
\Psi_k^W(t)=\log T_k e^{\sum_i t_iQ_i^W},\qquad
\Psi_k^{\rm leaf}(t)=\log T_k e^{\sum_i t_iQ_i^{\rm leaf}},
\]
with distinct labels, and let \(\Psi_k^{[m]}\) be the coefficient of \(t_1\cdots t_m\). Conditional cumulants are multilinear, so their difference is a sum over residual locations. For each partition and residual location, conditional Hölder at total envelope degree \(m+1\), then outer Hölder and preservation of expectation, gives an \(L^1\) bound
\(\alpha_Na^4e(m+1)!\sigma^{m+1}\).
There are \(m\) residual locations and
\(\sum_\pi(|\pi|-1)!\le2^{m-1}m!\). Consequently,
\[
\boxed{
\mathbb E_{\mu_k}|(\Psi_k^W)^{[m]}-(\Psi_k^{\rm leaf})^{[m]}|
\le e\,m(m+1)2^{m-1}(m!)^2\,
\varepsilon_\beta\sigma_{\beta,a}^m.}
\tag{N21}
\]
This closes the local replacement in a depth-independent microscopic factorial norm with exponent two. Higher connected jets are unchanged by deterministic centering, and the first centered coefficient can be handled by the ordinary centered \(L^1\) estimate.

For example, dividing by \((8\sigma)^m(m!)^2\) makes the supremum of the right side at most a fixed numerical constant times \(\varepsilon_\beta\), uniformly in every finite order and transport depth. This bound is on assembled conditional coefficients; it does not bound the absolute sum of their subsequent signed localized terms.

#### 5.2 Uniform maximum over the whole positive history

Use the common positive-history construction from Part I: for a finite depth \(J\), the decreasing filtration \(\mathcal G_k\) realizes
\(T_k f(X_k)=\mathbb E[f(X_0)\mid\mathcal G_k]\). Set
\[
N_{i,k}=\mathbb E[q_i^{m+1}\mid\mathcal G_k],\qquad 0\le k\le J.
\]
For a residual at label \(r\), let \(w_r=2\), \(w_i=1\) otherwise. Conditional Hölder bounds every absolute partition term of that residual's conditional cumulant by
\[
\alpha_Na^4\prod_iN_{i,k}^{w_i/(m+1)}.
\]
The weights sum to one. Reverse the finite filtration and apply the elementary \(L^2\) martingale maximal inequality:
\[
\left\|\max_{0\le k\le J}N_{i,k}\right\|_2
\le2\|q_i^{m+1}\|_2.
\]
Hölder for the weights \(w_i/(m+1)\) gives the stronger \(L^2\) estimate
\[
\left\|\prod_i\left(\max_kN_{i,k}\right)^{w_i/(m+1)}\right\|_2
\le2\sqrt e\sqrt{(2m+2)!}\,\sigma^{m+1}
\le2\sqrt e\,2^{m+1}(m+1)!\,\sigma^{m+1}.
\]
Summing the \(m\) residual locations and the partition coefficient bound \(2^{m-1}m!\) proves
\[
\boxed{\left\|\max_{0\le k\le J}
|(\Psi_k^W)^{[m]}-(\Psi_k^{\rm leaf})^{[m]}|\right\|_2
\le2\sqrt e\,m(m+1)4^m(m!)^2
\varepsilon_\beta\sigma_{\beta,a}^m.}
\tag{N21a}
\]
There is still no factor of \(J\). The same upper bound applies to the \(L^2\) norm at any measurable history-selected index \(\tau\in\{0,\ldots,J\}\), since its absolute value is bounded by this maximum. That observation concerns the estimate; it does not identify a new optional conditional-expectation formula for an arbitrary non-stopping index. Moreover, weighting the depth maximum by the original microscopic event \(B_\Gamma\) multiplies its \(L^1\) bound by \(e^{-\kappa|\Gamma|/2}\), by Cauchy–Schwarz in the common history law.

The only additional input in (N21a), beyond the preceding proof, is the common-history reverse-martingale construction and its \(L^2\) maximal inequality, both explicitly proved in Part I. It does not add a spatial or coarse-scale gain.

### 6. The leaf variance is an essential remaining term

The identity (N5) cannot be discarded as part of the quartic error. There is an elementary small-field counterexample.

Fix a site \(z\), choose a traceless Hermitian diagonal matrix \(T\) supported on an SU(2) subgroup, and set exactly one link leaving \(z\), say the positive 2-link, equal to \(e^{itT}\); set all other links to identity. At \(z\), in each of the three planes containing direction 2, two signed clover leaves are \(+a^{-2}H(e^{itT})\) and \(-a^{-2}H(e^{itT})\), while the other two vanish. Every clover average at \(z\) is zero. Hence
\[
q_C(z)=0,\qquad
q_{\rm leaf}(z)=\frac{3}{2a^4}\|H(e^{itT})\|^2,
\qquad q_W(z)=\frac3{a^4}s(e^{itT}).
\]
As \(t\to0\), both \(q_{\rm leaf}\) and \(q_W\) are of order \(t^2a^{-4}\), and their ratio tends to one. Their difference is only \(O(t^4a^{-4})\). Thus the leaf variance \(q_{\rm leaf}-q_C\) is a leading quadratic term even for arbitrarily small links. This is why the scalar replacement in (N8) retains it.

The example does not establish a lower bound on its Wilson expectation. It establishes that no pointwise higher-order estimate can remove this term without additional spatial regularity or dynamics.

The stronger current-scale consequence for the specified admitted minimizing background is proved in Part III below.

## Part III. the admitted-background curvature input

**Scope.** This note supplies a concrete scale-improved estimate for the specified real minimizing background in Balaban's admitted R construction. It closes the retained-background size input on that carrier. It does not identify an exact transported Wilson insertion with its value on the minimizer, remove the complementary histories, or establish the nonlinear and hard-cutoff contributions to S2.

### 1. Primary formulas used

The following equations are taken from the printed papers.

1. **CMP119 (1988), printed p.255, (2.4):**
   \[
   \epsilon_k=g_k A_0(\log g_k^{-2})^{p_0}=g_k p_0(g_k).
   \]
   We write this source coupling as \(g_{B,k}\) below to avoid confusing it with a differently normalized physical coupling. Set
   \[
   P_k=A_0(\log g_{B,k}^{-2})^{p_0},\qquad
   \epsilon_k=g_{B,k}P_k.
   \tag{R1}
   \]
   The source works at sufficiently small admitted positive coupling, so the logarithm is positive. The fixed constants and exponent are those of its construction.
2. **LFR I, printed p.193, (1.75):** the selector \(\chi_{k,\Lambda}\) depends on the exterior field \(V_k|_{Z\cap\Lambda^c}\). It requires an extension to \(Z\) whose interpolated background has the stated small plaquette curvature. This is a retained-data selector; it is different from the later fluctuation cutoff \(\chi'\).
3. **LFR I, printed pp.194–195, (1.78)–(1.80):** \(V_\Lambda\) is the specified constrained minimizing orbit, extended by the exterior field, and
   \[
   U_0=U_{k,Z}(V_\Lambda).
   \tag{R2}
   \]
   On the stated selector support,
   \[
   |U_0(\partial p)-I|
   <\left[2+C B_3B_5M^5e^{-\delta\operatorname{dist}(p,\Lambda)}\right]
       \epsilon_k\eta^2,
   \qquad p\in\Omega_k.
   \tag{R3}
   \]
   The constants and admitted block parameter \(M\) are fixed. Norm conversion between the source's fixed matrix norm and Hilbert–Schmidt norm changes a group-dependent constant only.
4. **LFR I, printed p.196, (1.82):** the additional hard cutoff is
   \[
   \chi'=\mathbf1\{|B'(b)|<\delta'_k\text{ for }b\in B_0\},
   \qquad V'=e^{iB'}.
   \tag{R4}
   \]
   Its set \(B_0\) is the construction's multiscale set of fluctuation bonds. It is not silently replaced below by a single fixed-size cube.
5. **CMP99 (1985), printed p.432, Theorem 3.15/(3.187):** the unit-lattice fluctuation covariance satisfies
   \[
   |C^{(k)}(\Lambda;y,y')|\le B_0e^{-\delta_0|y-y'|}
   \tag{R5}
   \]
   for the stated Dirichlet domain and backgrounds satisfying the source's regularity hypotheses with \(M\alpha_0\) sufficiently small. The constants depend on dimension and admitted block factor. The underlying quadratic form, constraints and parametrization are stated on printed pp.427–428, (3.155)–(3.158).

Only (R1)–(R3) are needed for the unconditional admitted-background theorem below. Formula (R5) does not by itself identify the curvature response of an arbitrary transported insertion with a nearest-neighbor curl. Formula (R4) is retained as a separate cutoff operation.

### 2. Exact admissible carrier and the physical scaling dictionary

The source's \(\eta\)-lattice is expressed in units of the current coarse scale. Let that physical scale be \(h\), so the physical fine spacing is
\[
a=\eta h.
\tag{R6}
\]
The source coupling satisfies \(g_{B,k}^{-2}=X_{B,k}\). At the original scale the exact dictionary is \(X_{B,0}=N\beta=2N^2x_0\); no identification with a differently named physical coupling is made without this factor.

For a physical fine-lattice site \(x\), let \(\mathcal L(x)\) be the set of its 24 signed clover plaquette leaves, six planes and four quadrants in each plane. Define the admissible event \(\mathcal A_k(x)\) by all of the following:

- The current retained data are on the real compact-group slice of the R construction.
- The specified background is exactly \(U_0\) in (R2), with \(\chi_{k,\Lambda}=1\).
- Every leaf in \(\mathcal L(x)\), mapped into source coordinates by division by \(h\), lies in \(\Omega_k\), so (R3) applies to it.
- The fixed geometry and small-coupling conditions required for the source construction are satisfied.

For several marked sites put \(\mathcal A_k(X)=\bigcap_i\mathcal A_k(x_i)\). This event is determined by retained data once the carrier geometry and external fields are fixed. It does not impose \(\chi'\) on the Gaussian fluctuations. If a marked stencil crosses the admitted domain boundary, its contribution belongs to the complementary carrier and is not covered by the theorem.

After taking the maximum of the boundary-decay coefficient in (R3), there is a constant \(C_b\), independent of \(k,h,\eta\), torus volume and retained configuration, such that on \(\mathcal A_k(x)\)
\[
\|U_0(\partial p)-I\|_{\rm HS}\le C_b\epsilon_k\eta^2,
\qquad p\in\mathcal L(x).
\tag{R7}
\]
One may retain the local coefficient \(2+C B_3B_5M^5e^{-\delta d(\mathcal L(x),\Lambda)}\) instead of its maximum. The uniform estimate below suffices for the local second-moment input.

### 3. The actual background fields gain the current physical scale

Use the fields of [Wilson tensor witnesses and large-field suppression](tensor_witnesses.md) evaluated on the specific \(U_0\):
\[
H(P)=\pi_0\frac{P-P^\dagger}{2i},\qquad
F_A^C(U_0;x)=\frac1{4a^2}\sum_{\epsilon,\delta=\pm1}
\epsilon\delta H(P_{\epsilon e_\mu,\delta e_\nu}(U_0;x)),
\]
\[
q_W(U_0;x)=\frac1{2a^4}\sum_{p\in\mathcal L(x)}s_p(U_0),\qquad
q_C(U_0;x)=\sum_A\|F_A^C(U_0;x)\|_{\rm HS}^2.
\]
The scalar-corrected matrix \(Q^W\) is the already constructed family
\[
Q^W_{AB}=\operatorname{Tr}(F_A^CF_B^C)
 +\frac{\delta_{AB}}6(q_W-q_C).
\]

**Theorem R-G2 (closed on the stated admitted carrier).** Put \(C_*=6C_b^2\). Pointwise on \(\mathcal A_k(x)\),
\[
\boxed{
0\le q_C(U_0;x)\le q_W(U_0;x)
\le C_*g_{B,k}^2P_k^2h^{-4}.}
\tag{R8}
\]
Consequently,
\[
\boxed{|Q^W_{AB}(U_0;x)|\le C_*g_{B,k}^2P_k^2h^{-4},}
\tag{R9}
\]
and for \(B_h(x)=(F_A^C(U_0;x))_{A=1}^6\), with the sum of Hilbert–Schmidt squares as its squared norm,
\[
\boxed{\mathbb E[\mathbf1_{\mathcal A_k(x)}|B_h(x)|^2]
\le C_*g_{B,k}^2P_k^2h^{-4}.}
\tag{R10}
\]
The expectation can be any normalized positive law on the actual retained histories. Thus no additional probabilistic moment hypothesis is needed for this particular admitted minimizing background.

**Proof.** For unitary plaquette holonomy,
\(s_p=\frac12\|U_0(\partial p)-I\|_{\rm HS}^2\).
By (R7), every one of the 24 leaves has
\(s_p\le\frac12C_b^2\epsilon_k^2\eta^4\).
Therefore
\[
q_W\le\frac{24}{2a^4}\frac12 C_b^2\epsilon_k^2\eta^4
=6C_b^2\epsilon_k^2h^{-4}.
\]
Here the equality uses \(a=\eta h\). The prior exact clover inequality gives \(q_C\le q_W\), and the positive matrix bound gives \(|Q^W_{AB}|\le q_W\). Integration against an arbitrary positive probability law preserves the pointwise inequality. \(\square\)

There are also immediate all-order admitted-background moment bounds,
\[
\mathbb E\left[\mathbf1_{\mathcal A_k(x)}q_W(U_0;x)^m\right]
\le[C_*g_{B,k}^2P_k^2h^{-4}]^m.
\tag{R11}
\]
This does not require an estimate for the probability of the admitted event. It does not estimate its complement either.

**Centering caveat.** Equations (R8)–(R9) concern the uncentered field evaluated on \(U_0\). Subtracting the original microscopic expectation can reintroduce a number of order \(a^{-4}\); no \(h^{-4}\) bound is claimed for that centered value as a random variable. Deterministic identity subtractions disappear from every conditional connected order \(m\ge2\), which is the use relevant below.

### 4. The exact leaf-quadratic family has the same background bound

For each signed leaf, use the Hermitian traceless coordinate
\[
L_{A,\epsilon,\delta}(U;x)=\frac{\epsilon\delta}{2a^2}
H(P_{\epsilon e_\mu,\delta e_\nu}(U;x)).
\tag{R12}
\]
Let \(L(U;x)\) denote their vector in the direct sum of 24 copies of the color Lie algebra. The coordinate \(L\) here is \(Y/2\) in Part II. Define the averaging map \(\mathsf A\) by
\[
(\mathsf A L)_A=\frac12\sum_{\epsilon,\delta}L_{A,\epsilon,\delta}.
\]
Then \(\mathsf A L=F^C\) and \(\mathsf A\mathsf A^*=I\). Thus \(\mathsf A^*\mathsf A\) is an orthogonal projection. The quadratic-leaf scalar and matrix are
\[
q_{\rm leaf}(U;x)=|L(U;x)|^2,
\]
\[
Q^{\rm leaf}_{AB}(U;x)
=\langle(\mathsf A L)_A,(\mathsf A L)_B\rangle
 +\frac{\delta_{AB}}6\bigl(|L|^2-|\mathsf A L|^2\bigr).
\tag{R13}
\]
These are the fields of the global scalar-replacement theorem in Part II. In particular,
\[
q_C\le q_{\rm leaf}\le q_W,
\quad Q^{\rm leaf}\succeq0,
\quad\operatorname{tr}_6Q^{\rm leaf}=q_{\rm leaf}.
\]
Every entry is exactly of the form \(\frac12 L^TM_{AB}L\), with a constant real symmetric matrix satisfying
\[
\|M_{AB}\|\le2.
\tag{R14}
\]
For diagonal entries, half of \(M_{AA}\) is the sum of the projection onto the common-leaf color subspace for plane \(A\) and \((I-\mathsf A^*\mathsf A)/6\), two orthogonal subspaces, so its norm is one. For off-diagonal entries, half of \(M_{AB}\) has norm \(1/2\). These statements are independent of the cutoff and the background.

The retained leaf vector \(B_h^{\rm leaf}(x)=L(U_0;x)\) therefore satisfies the same exact regular-carrier estimate:
\[
\boxed{\mathbb E[\mathbf1_{\mathcal A_k(x)}|B_h^{\rm leaf}(x)|^2]
\le C_*g_{B,k}^2P_k^2h^{-4}.}
\tag{R15}
\]
This aligns the background bound with an actual constant-quadratic representative of all 21 fields. The remaining distinction is that the leaf coordinate of the fluctuating group field is nonlinear in the fluctuation variables.

#### 4.1 A genuine \((a/h)^4\) gain for the scalar-replacement error on this background

Part II proves globally
\[
D(U;x):=q_W(U;x)-q_{\rm leaf}(U;x)\ge0,
\qquad D(U;x)\le2C_N a^4q_W(U;x)^2,
\tag{R16}
\]
where one possible constant is
\[
C_N=\frac12+\frac{2L_N^2}{N},\qquad
L_N=\frac{3^N-1-2N}{4}.
\]
Its scalar difference at the matrix level is
\(Q^W-Q^{\rm leaf}=I_6D/6\).
Combining (R16) with (R8) gives, on \(\mathcal A_k(x)\),
\[
\boxed{
0\le D(U_0;x)
\le 2C_N C_*^2g_{B,k}^4P_k^4
\left(\frac ah\right)^4h^{-4}.}
\tag{R17}
\]
This is a real power gain for the particular nonlinear scalar replacement evaluated on the admitted minimizer. It does not assert the same gain after applying the exact full RG transport to the original microscopic observable.

### 5. All conditional Gaussian tensor cumulants: only two background logarithms

Let \(Y\) denote retained data and let \(\xi_h^Y(x)\) be a centered jointly Gaussian vector in the leaf space. Put
\[
O_i=\tfrac12(B_h^Y(x_i)+\xi_h^Y(x_i))^TM_i
                 (B_h^Y(x_i)+\xi_h^Y(x_i)),
\]
where \(B_h^Y=B_h^{\rm leaf}\), and \(\|M_i\|\le z_i\). For the fixed 21-entry family (R13), one can take every \(z_i\le2\). A further running mixing factor must be included explicitly in \(z_i\).

Suppose that the actual conditional Gaussian curvature-response covariance has, on \(\mathcal A_k(X)\), the bound
\[
\|K_h^Y(x,y)\|\le c_Kg_{B,k}^2h^{-4}\mathcal D_h(x,y),
\qquad 0\le\mathcal D_h\le1.
\tag{R18}
\]
The profile may use torus distance or the actual localized source metric. No pure exponential profile is substituted for an unproved one. Write
\[
\mathfrak P_m(X)=\max_{\sigma\in S_m}
\prod_{r=1}^{m-1}\mathcal D_h(x_{\sigma(r)},x_{\sigma(r+1)}).
\tag{R19}
\]

**Corollary R-Gaussian.** The retained-background moment hypothesis for these admitted Gaussian shells can be discharged using (R15). For \(m\ge2\),
\[
\boxed{
\mathbb E\left[\mathbf1_{\mathcal A_k(X)}
|\kappa_m(O_1,\ldots,O_m\mid Y)|\right]
\le m!\left[\frac{d\,c_K^m}{2m}
       +\frac{C_*P_k^2c_K^{m-1}}2\right]
g_{B,k}^{2m}h^{-4m}\left(\prod_i z_i\right)\mathfrak P_m(X),}
\tag{R20}
\]
where \(d=24\dim\mathfrak g\) for the leaf vector. In particular this is
\[
C^m m!(1+P_k^2)g_{B,k}^{2m}h^{-4m}
\left(\prod_i z_i\right)\mathfrak P_m(X).
\tag{R21}
\]

**Proof.** The exact Gaussian cumulant consists of cycles with \(m\) covariance factors and paths with \(m-1\) covariance factors and exactly two retained-background endpoints. The cycle coefficient is \(1/(2m)\) times a sum over \(m!\) permutations. Each trace is bounded by \(d\), the matrix norm factors, and its covariance product. Since \(0\le\mathcal D_h\le1\), removing one edge bounds its profile by (R19).

The path coefficient is \(1/2\) times a sum over \(m!\) permutations. On the common admitted event, (R15), or its stronger pointwise form, gives
\[
\mathbb E\left[\mathbf1_{\mathcal A_k(X)}|B_h(x_i)||B_h(x_j)|\right]
\le C_*g_{B,k}^2P_k^2h^{-4}
\]
by Cauchy–Schwarz. The other \(m-1\) factors are bounded by (R18). Multiplication yields (R20). \(\square\)

The significant improvement is that the retained-field logarithm costs \(P_k^2\), whose degree is independent of \(m\), rather than \(P_k^{2m}\). There are only two background endpoints in every connected Gaussian path.

For two marks the sharper direct expression is
\[
\mathbb E\left[\mathbf1_{\mathcal A_k(x,y)}
|\operatorname{Cov}(O_1,O_2\mid Y)|\right]
\le z_1z_2g_{B,k}^4h^{-8}
\left[\frac d2c_K^2\mathcal D_h(x,y)^2
 +C_*P_k^2c_K\mathcal D_h(x,y)\right].
\tag{R22}
\]
When the proved profile is \(\mathcal D_h(x,y)=e^{-c d(x,y)/(h\mathcal R_k)}\), the spanning-path length is at least the minimum-spanning-tree length \(\mathcal T_d(X)\), so
\(\mathfrak P_m(X)\le e^{-c\mathcal T_d(X)/(h\mathcal R_k)}\).
Any localization factor \(\mathcal R_k\), including logarithmic enlargement, is retained. Summability must be checked for that actual profile.

#### 5.1 What the covariance source does and does not supply

Formula (R5) supplies the unit-lattice link fluctuation covariance under its own regularity and domain hypotheses. If a curvature response is explicitly a bounded-range unit-lattice linear combination of those links, with a uniformly bounded coefficient row sum, two applications of that row sum give (R18) after the factor \(g_{B,k}h^{-2}\) at each endpoint and a fixed change in the decay constant.

For an interpolated or minimized fine-lattice observable, one must instead compose with its actual linear-response operator and prove the corresponding derivative/localization bound. Theorems for an abstract nearest-neighbor curl cannot replace that composition. This note closes the background size input, not the remaining identification and covariance-response theorem.
