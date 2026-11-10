# Exact scalar transfer response and the field domain

**Annex C.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Status

The reduced interacting periodic OS quadratic inequality is **not proved** here. The available source-free Wilson stability, bare transfer estimates, finite native jets and numerical coupling trajectory do not control its arbitrary-vector norm after physical renormalization.

This annex supplies two exact further results and a diagnostic:

1. A scalar Wilson coupling insertion is related to the logarithmic response of the normalized transfer operator by an explicit completely positive real-time averaging map. The inverse has a controlled imaginary-time strip. Thus the physical scalar slab target can be stated as a local coupling-response bound, with exact identity subtraction and no assumed differentiability of an unbounded logarithm.
2. The full Schwartz Borchers domain is an energy graph core. Once the bounds and canonical identification are available, covariance, locality and the minimal closed field realization extend to the whole smooth-energy domain. This supplies the domain argument; it is not an interacting estimate.
3. A central random rescaling can preserve the entire two- and three-point functions, including their quantitative short-distance laws, while violating every polynomial energy bound in the mixed theory. A related additive construction preserves all connected functions of order at least three. These examples are not Wilson limits; they test the proposed inference from vacuum information to operator estimates.

The source geometry check still does not license independent temporal enlargement. CMP109 specifies common side parameter $L_\mu=L^m$; CMP119 explicitly inherits that geometry. A rectangular extension may be possible, but is not imported as an already proved result.

Status notation: **P** means a proof from the displayed hypotheses is supplied; **L** means a scoped primary-source statement; **O** means an unproved Yang–Mills estimate. No novelty claim is made.

### 1. Exact normalized scalar source in the full compact transfer kernel

Fix a finite spatial lattice, spacing $a>0$, and the physical gauge-invariant Hilbert space. Use the full compact Wilson transfer operator $T_\theta$, with no small-field restriction. A real time-independent spatial profile $f$ changes the scalar plaquette couplings from $\beta$ to $\beta+\theta f_p$, with $\theta$ small enough that all temporal couplings remain positive. The spatial action is distributed equally between the two ends of a time step. The temporal-link integrations give the usual gauge projection. One-link scalar normalization factors may be held fixed during the source variation. A different scalar convention multiplies $T_\theta$ by an overall positive scalar, which cancels in $P_\theta=T_\theta/\lambda_0(\theta)$; it only shifts the unnormalized raw insertion by a known identity term.

At fixed cutoff $T_\theta$ is a positive selfadjoint trace-class operator, is injective on the physical space, and has a simple positive largest eigenvalue $\lambda_0(\theta)$. Its kernel and its source derivative are bounded on the compact configuration space. Write

\[
P_\theta=\frac{T_\theta}{\lambda_0(\theta)},\qquad
P=P_0=e^{-aH},\qquad H\ge0,
\qquad \dot P=\left.\frac{dP_\theta}{d\theta}\right|_{0}.
\tag{1.1}
\]

The derivative $\dot P$ is a bounded selfadjoint operator. No global differentiability statement for the unbounded family $-a^{-1}\log P_\theta$ is assumed.

Let $\mathcal D_{\rm fin}$ be the finite span of spectral vectors of $H$. At fixed spatial cutoff every bounded-energy spectral projection has finite rank. Define the centered one-step midpoint insertion as a form on this domain by

\[
\mathcal O=-P^{-1/2}\dot P P^{-1/2}.
\tag{1.2}
\]

If $T_f=-\dot T$ denotes the transfer kernel with the full one-step scalar action mark, then

\[
\mathcal O
=P^{-1/2}\frac{T_f}{\lambda_0}P^{-1/2}
 +\frac{\dot\lambda_0}{\lambda_0}I.
\tag{1.3}
\]

Thus the identity term is fixed by normalization of the actual transfer operator. In particular, with $P\Omega=\Omega$ and $\|\Omega\|=1$,

\[
\langle\Omega,\mathcal O\Omega\rangle=0.
\tag{1.4}
\]

To see this without differentiating the vacuum vector, use the simple-eigenvalue formula $\dot\lambda_0=\langle\Omega,\dot T\Omega\rangle$. The two terms in (1.3) cancel in the vacuum expectation.

For $t\ge a/2$, its heat sandwich is the bounded exact marked transfer slab

\[
e^{-tH}\mathcal Oe^{-tH}
=-P^{t/a-1/2}\dot P P^{t/a-1/2}.
\tag{1.5}
\]

This formula includes all spatial interactions, gauge projection, large fields and the identity subtraction. It establishes boundedness at each fixed cutoff, not a bound uniform after physical normalization.

#### 1.1 Spectral logarithmic response

Choose an orthonormal spectral basis with

\[
H e_i=E_i e_i,\qquad p_i=e^{-aE_i}>0.
\]

Define a Hermitian form $\mathfrak h$ on $\mathcal D_{\rm fin}$ by

\[
\mathfrak h_{ij}
=-\frac1a\,
\frac{\log p_i-\log p_j}{p_i-p_j}\,\dot P_{ij},
\tag{1.6}
\]

where the diagonal divided difference is $1/p_i$. The definition is basis independent within degenerate energy eigenspaces. It is the divided-difference logarithmic response of the normalized transfer operator. Whenever an unbounded logarithmic derivative is separately justified, it agrees with that derivative on these matrix elements. Equation (1.6) itself requires no such unproved differentiability theorem.

Put

\[
k_a(\omega)=\frac{a\omega/2}{\sinh(a\omega/2)},\qquad
\rho_a(s)=\frac{\pi}{2a}\operatorname{sech}^2(\pi s/a).
\tag{1.7}
\]

Then $\rho_a\ge0$, $\int\rho_a(s)\,ds=1$, and

\[
\int_{\mathbb R}\rho_a(s)e^{is\omega}\,ds=k_a(\omega).
\tag{1.8}
\]

For example, after $x=\pi s/a$ and $u=e^{2x}$ the integral becomes
$\int_0^\infty u^{ia\omega/(2\pi)}(1+u)^{-2}du$; the beta-integral evaluation gives (1.8).

**Proposition 1.1 (P: exact response transforms).** On every finite-energy spectral band,

\[
\boxed{
\mathfrak h
=\frac1a\int_{\mathbb R}\rho_a(s)
e^{isH}\mathcal Oe^{-isH}\,ds,
}
\tag{1.9}
\]

and

\[
\boxed{
\frac{\mathcal O}{a}
=\int_{-1/2}^{1/2}
e^{asH}\mathfrak h e^{-asH}\,ds.
}
\tag{1.10}
\]

**Proof.** Writing $\Delta=E_i-E_j$ and using (1.2),

\[
\mathfrak h_{ij}
=\frac1a\frac{a\Delta/2}{\sinh(a\Delta/2)}\mathcal O_{ij}.
\tag{1.11}
\]

Equation (1.9) follows from (1.8). The coefficient of $\mathfrak h_{ij}$ on the right of (1.10) is
$\int_{-1/2}^{1/2}e^{as\Delta}ds=\sinh(a\Delta/2)/(a\Delta/2)$, proving the inverse formula. All expressions on a bounded-energy band are finite dimensional and the zero-gap values are obtained continuously. ∎

The map in (1.9), apart from its factor $a^{-1}$, is unital and completely positive on bounded operators, since it is an average of unitary conjugations. In particular it is contractive in operator norm. This property is stronger than an entrywise divided-difference bound, which would not by itself control matrix operator norms.

#### 1.2 Uniform slab comparison with no loss of a spatial volume factor

Let $Q_E=1_{[0,E]}(H)$. On a finite-energy band,

\[
\|Q_E\mathfrak hQ_E\|
\le a^{-1}\|Q_E\mathcal OQ_E\|,
\qquad
\|Q_E\mathcal OQ_E/a\|
\le e^{aE/2}\|Q_E\mathfrak hQ_E\|.
\tag{1.12}
\]

The second estimate uses the spectral range $[0,E]$ in (1.10). For a more quantitative low-energy comparison,

\[
\left\|Q_E(\mathcal O/a-\mathfrak h)Q_E\right\|
\le \frac{(aE)^2}{24}e^{aE/2}
\|Q_E\mathfrak hQ_E\|.
\tag{1.13}
\]

Indeed the norm of $\operatorname{ad}_{H|_{Q_E}}$ is at most $E$, after subtracting $E/2$ from $H$, and the odd term in the symmetric integral vanishes. Taylor's remainder bounds the rest by the displayed constant.

For heat sandwiches, the completely positive transform gives

\[
\boxed{
\|e^{-tH}\mathfrak h e^{-tH}\|
\le a^{-1}\|e^{-tH}\mathcal Oe^{-tH}\|.
}
\tag{1.14}
\]

This is first proved by spectral truncation and then by the bounded unitary average of the right-hand sandwich. It is valid whenever that sandwich is bounded, in particular at finite cutoff for $t\ge a/2$ by (1.5).

Conversely, suppose a compatible family of bounded form sandwiches satisfies

\[
\|e^{-uH}\mathfrak h e^{-uH}\|\le C u^{-\kappa}\rho_s(f)
\quad (0<u\le1).
\tag{1.15}
\]

For $0<t-a/2\le1$, insert (1.10) and write every integrand as

\[
e^{-(t-as)H}\mathfrak h e^{-(t+as)H}.
\]

Both heat times are at least $t-a/2$. Factor out the symmetric sandwich at that smaller time; the remaining semigroups are contractions. This gives

\[
\boxed{
\|e^{-tH}(\mathcal O/a)e^{-tH}\|
\le C(t-a/2)^{-\kappa}\rho_s(f).
\quad (0<t-a/2\le1)
}
\tag{1.16}
\]

For arbitrary $t>a/2$, the same argument uses the sandwich at $u=\min(t-a/2,1)$ and gives the bound $C[\min(t-a/2,1)]^{-\kappa}\rho_s(f)$. Therefore, at fixed physical time, a uniform bound for the centered scalar slab and one for its logarithmic coupling response are equivalent up to a harmless time shortening. In the small-time range $a<t\le1$, the loss relative to $Ct^{-\kappa}$ is at most $2^\kappa$.

#### 1.3 The physical normalization and what remains unknown

The plaquette coefficient convention is the one retained throughout:
$s_p=N-\operatorname{Re}\operatorname{Tr}U_p$ has coefficient $\beta=2Nx_0$, and Balaban's normalized-trace coefficient is $X_B=N\beta=2N^2x_0$.

For a spatial profile $f$, the dimension-four physical normalization of a one-step coupling insertion has spatial smearing

\[
a^3\sum_{\mathbf x} f(\mathbf x)
\bigl(a^{-4}Z_a\,\text{ground-centered plaquette insertion}\bigr)
=\frac{Z_a}{a}\mathcal O_a(f),
\tag{1.17}
\]

with the finite orientation and half-step weights absorbed in the definition of the source. Ground centering is not silently identified with the chosen finite normalization prescription at $\mu$. Let

\[
\mathcal A_a(f)=P^{-1/2}(T_f/\lambda_0)P^{-1/2},\qquad
m_{a,V}(f)=\langle\Omega,\mathcal A_a(f)\Omega\rangle
          =-\dot\lambda_0/\lambda_0.
\tag{1.18}
\]

If the prescribed scalar insertion is
$\mathcal Q_a^R(f)=Z_a\mathcal A_a(f)/a-c_{a,\mu}(f)I$, then exactly

\[
\mathcal Q_a^R(f)=Z_a\mathcal O_a(f)/a+d_{a,V,\mu}(f)I,
\qquad
d_{a,V,\mu}(f)=Z_am_{a,V}(f)/a-c_{a,\mu}(f).
\tag{1.19}
\]

The source prescription must control this remaining identity coefficient. The formulas do not establish its volume independence or equality with a periodic-state subtraction. Define
$\mathfrak h_a^R(f)=Z_a\mathfrak h_{a,f}+d_{a,V,\mu}(f)I$.
Let $\Theta_a(X)=\int\rho_a(s)e^{isH_a}Xe^{-isH_a}ds$ and, on finite-energy bands, $\Psi_a(X)=\int_{-1/2}^{1/2}e^{asH_a}Xe^{-asH_a}ds$. Both maps preserve the identity, so exactly $\mathfrak h_a^R=\Theta_a(\mathcal Q_a^R)$ and $\mathcal Q_a^R=\Psi_a(\mathfrak h_a^R)$. In particular the forward comparison is $\|e^{-tH_a}\mathfrak h_a^R e^{-tH_a}\|\le\|e^{-tH_a}\mathcal Q_a^R e^{-tH_a}\|$, with no additional factor $a^{-1}$. The inverse comparison has the time shortening in (1.16). The exact scalar response target is therefore

\[
\boxed{
\|e^{-tH_a}\mathfrak h_a^R(f)e^{-tH_a}\|
\le C t^{-\kappa}\rho_s(f),
\quad 0<t\le1,
\quad\text{uniformly in cutoff and expanding volume}.
}
\tag{R}
\]

This is still **O**. The transform proves that (R) is an alternative formulation of the scalar physical slab estimate; it does not supply the norm on its left. The microscopic power cancellation is now contained in the logarithmic response and the explicitly retained identity term, rather than proved by rewriting them. If the prescribed scheme is separately proved to agree with this ground-state centering, then $d_{a,V,\mu}=0$; that agreement is not assumed here.

The numerical AF trajectory controls a scalar coupling recursion. It does not control arbitrary-vector matrix elements of $\mathfrak h_{a,f}$, nor derivatives of the transfer eigenvectors. Bounds on eigenvalues or partition functions alone would not control those off-diagonal responses. A local source theorem in an operator or boundary-kernel norm is additional information.

The definition in (1.17) covers the scalar coupling-derivative channel. It does not identify the other tensor sources with a variation through positive transfer operators, or establish their running mixing. An actual tensor estimate must retain their Wick/adjoint conventions and their marked half-step placements.

Finally, (R) is a Hamiltonian norm estimate. The periodic-state transfer issue remains separate: a ground-state norm bound cannot simply be substituted into the periodic OS quadratic inequality without controlling the exact thermal factors or proving an admissible temporal diagonal-limit argument.

### 2. The Schwartz Borchers domain is an energy graph core

This section fills a domain detail in the identification. It assumes that the reconstruction and the energy graph bounds have already been obtained. It does not help prove the interacting hypothesis used to obtain them.

Let $\mathcal D_0$ be the canonical Wightman domain generated by the **full Schwartz Borchers algebra**: vectors are finite sums $\Psi_n(F_n)$ with joint $F_n\in\mathcal S(\mathbb R^{4n})$, together with the vacuum. It is important to use this full domain, not merely algebraic finite sums of tensor-product tests. Put $R=1+H$.

**Lemma 2.1 (P).**

1. $\mathcal D_0\subset\mathcal D_\infty=\bigcap_{r\ge0}D(R^r)$.
2. If $\rho\in C_c^\infty(\mathbb R)$, then $\rho(H)\mathcal D_0\subset\mathcal D_0$.
3. $\mathcal D_0$ is a graph core for $R^r$ for every fixed integer $r\ge0$.

**Proof.** Common time translation acts on $F_n$ by translating all its time variables. The Schwartz-valued map is $C^\infty$. The Hilbert-valued Wightman map is continuous, because its squared norm is a tempered $(2n)$-point distribution. Thus $t\mapsto U(t)\Psi_n(F_n)$ is norm $C^\infty$, proving the first assertion by the generator criterion.

For the second, write $\rho(H)$ as the common-time Fourier integral of the Schwartz function $\widehat\rho$. The resulting test is

\[
F_{n,\rho}(x_1,\ldots,x_n)
=c\int_{\mathbb R}\widehat\rho(t)
F_n(x_1-te_0,\ldots,x_n-te_0)\,dt,
\tag{2.1}
\]

which is a joint Schwartz test. The integral converges in Schwartz topology and hence in Hilbert norm. Therefore $\rho(H)\Psi_n(F_n)=\Psi_n(F_{n,\rho})$.

Choose smooth energy cutoffs $\rho_M$ equal to one on $[0,M]$ and supported in $[-1,2M]$. For $\psi\in D(R^r)$, spectral calculus gives $\rho_M(H)\psi\to\psi$ in the $R^r$ graph norm. For fixed $M$, choose $v_j\in\mathcal D_0$ tending to $\psi$ in Hilbert norm. Then $\rho_M(H)v_j\in\mathcal D_0$ and

\[
\|R^r\rho_M(H)(v_j-\psi)\|
\le\|R^r\rho_M(H)\|\,\|v_j-\psi\|\longrightarrow0.
\]

A diagonal choice proves graph-core density. ∎

**Corollary 2.2 (P: domain completion).** Suppose the realization agrees with the canonical fields on $\mathcal D_0$, and has, for each integer $r\ge0$,

\[
\|R^r\phi_\alpha(f)R^{-(r+b)}\|
\le c_{r,\alpha}\,\mathcal N_r(f)
\tag{2.2}
\]

with one finite $b$ (the construction has $b=2\ell$). Then:

- The closure of the field restricted to $\mathcal D_0$ equals the closure of its $\mathcal D_\infty$ realization.
- Spacelike commutativity holds on all of $\mathcal D_\infty$.
- Poincare covariance holds on all of $\mathcal D_\infty$, with the stipulated finite tensor transformation matrices.

**Proof.** For $\psi\in\mathcal D_\infty$, approximate in the graph norm of $R^b$ by $v_j\in\mathcal D_0$. The $r=0$ bound gives convergence of the field values, so $\mathcal D_0$ is a core for the field on $\mathcal D_\infty$. The reverse closure inclusion is immediate.

For a product $\phi_\alpha(f)\phi_\beta(g)$, approximate in the graph norm of $R^{2b}$; apply (2.2) with $r=b$ to the inner field and $r=0$ to the outer field. Both orderings converge in Hilbert norm. Their difference vanishes on $\mathcal D_0$ for spacelike separated supports, so it vanishes on $\mathcal D_\infty$.

The forward-cone spectrum implies $U(\Lambda)^*HU(\Lambda)\le c_\Lambda H$ in joint spectral calculus, and the inverse Lorentz transformation gives the reverse domain comparison. Thus $U(\Lambda)$ is continuous between the corresponding energy graph norms and preserves $\mathcal D_\infty$. Approximate there by $\mathcal D_0$ and pass the canonical covariance identity using (2.2). Translations commute with $H$ and are simpler. ∎

This strengthens the conclusion to the actual minimal closed canonical fields on the common smooth-energy domain. It still does not identify arbitrary other closed extensions of those operators.

### 3. Exact two- and three-point data do not imply the operator bound

The old constant-Gaussian example showed that excellent vacuum regularity alone need not give an $H$-bound. The following example shows that even preserving prescribed two- and three-point functions exactly is insufficient before controlling the center or phase transfer.

#### 3.1 Random rescaling

Let $\psi_\alpha$ be a nontrivial centered Wightman field family with unique vacuum $\Omega_0$, positive Hamiltonian $H_0$, corrected OS bounds and a polynomial energy estimate. Assume some real smear $f$ of a Hermitian component has $\psi(f)\Omega_0\ne0$ and nonzero even vacuum moments. A concrete scalar dimension-four choice is the Wick fourth power of a massive free scalar field; curvature Wick bilinears of free Maxwell fields provide another dimension-four example. No Yang–Mills claim is made for either.

Let $G$ be an independent standard Gaussian and define

\[
A=m+\sigma G,\qquad
m=\frac{\sqrt3-1}{2},\qquad \sigma^2=\frac{\sqrt3}{2}.
\tag{3.1}
\]

Direct calculation gives

\[
\mathbb EA^2=m^2+\sigma^2=1,
\qquad
\mathbb EA^3=m^3+3m\sigma^2=1.
\tag{3.2}
\]

On $L^2(\mathbb P_A)\otimes\mathcal H_0$ put

\[
\Phi_\alpha(f)=M_A\otimes\psi_\alpha(f),\qquad
U=I\otimes U_0,\qquad H=I\otimes H_0,\qquad
\Omega=1\otimes\Omega_0,
\tag{3.3}
\]

and restrict to the cyclic Wightman subspace generated by these fields.

**Proposition 3.1 (P).** This hierarchy has the same full two- and three-point functions as $\psi$, retains Euclidean covariance, symmetry and reflection positivity, and retains a fixed factorial OS growth bound. It nevertheless has no polynomial energy estimate for any component smear $f$ with $\psi(f)\Omega_0\ne0$.

**Proof of the hierarchy statements.** Its full Euclidean moments are

\[
S_m^\Phi=\mathbb EA^m\,S_m^\psi.
\tag{3.4}
\]

Centering and (3.2) give exact equality at orders two and three, including connected functions. Tensor covariance and permutation symmetry are unchanged. Reflection positivity follows by integrating the positive quadratic form for the scaled field $a\psi$ over real $a$. Gaussian moments satisfy

\[
\mathbb E|A|^m\le C^m(m!)^{1/2},
\tag{3.5}
\]

so an OS bound with exponent $p$ becomes one with exponent $p+1/2$, with the same linear derivative-order parameter. The bound can instead be rounded to any larger integer exponent.

**Proof of failure of the energy bound.** Let $P_0=I\otimes|\Omega_0\rangle\langle\Omega_0|$. For each $n$, a field word with nonzero even vacuum moment gives

\[
P_0\Phi(f)^{2n}\Omega
=c_{2n}A^{2n}\otimes\Omega_0,\qquad c_{2n}\ne0.
\tag{3.6}
\]

The cyclic space is invariant under time translations and their spectral projections, so these central vectors belong to it. They also belong to the domain of the minimal closed field, rather than merely the tensor-product extension. To verify this, apply common-time heat smearing to the field word: $e^{-TH_0}\psi(f)^{2n}\Omega_0$ tends to $c_{2n}\Omega_0$ in every fixed energy graph norm. For each $T>0$, the multiplier $e^{-TE}$ on $E\ge0$ has a Schwartz extension to $E\in\mathbb R$, so the common-time smear lies in the full Borchers domain. The base polynomial energy estimate shows convergence after applying $\psi(f)$ as well. The factor $A^{2n+1}$ is square integrable. Thus (3.6)'s central vector is obtained in the graph closure of $\Phi(f)$.

Normalize $v_n=A^{2n}\otimes\Omega_0/\|A^{2n}\|_2$. Then $Hv_n=0$, while

\[
\|\overline{\Phi(f)}v_n\|
=\|\psi(f)\Omega_0\|
\left(\frac{\mathbb E|A|^{4n+2}}{\mathbb E|A|^{4n}}\right)^{1/2}
\longrightarrow\infty.
\tag{3.7}
\]

For an unbounded random variable with all moments, these moment ratios diverge: log-convexity makes the successive ratios nondecreasing, and a bounded limit would force the support of $A^2$ to be bounded. Since $(1+H)^{-r}v_n=v_n$, no finite $r$ gives a bounded regularized field. ∎

The base's two- and three-point short-distance asymptotics are preserved **exactly**, whatever their detailed form. For any hypothetical base with the required Yang–Mills ultraviolet coefficients, this operation would preserve those two functions while destroying the mixed-theory energy estimate. For the concrete free composite example the ultraviolet dimension is four and the three-point coefficient is nonzero, but its law is not the Yang–Mills AF law.

In the displayed conditional decomposition at fixed $A=a$, the two- and three-point coefficients become $a^2$ and $a^3$ times the base values. For both prescribed nonzero coefficients to remain unchanged with the fixed field normalization requires $a=1$, a set of zero Gaussian measure. Thus scalar averaged coefficients do not imply an almost-everywhere or positive-measure phase transfer. This does not exclude a conceivable selected zero-weight phase at $a=1$, and does not exclude a new phase-dependent finite normalization. Those are different claims requiring their own specification.

#### 3.2 Additive central noise preserves all higher connected functions

For a scalar field one can instead put

\[
\widetilde\Phi(f)
=I\otimes\psi(f)+M_G\otimes I\int f,
\tag{3.8}
\]

with centered independent Gaussian $G$. Independence gives

\[
S_{2,c}^{\widetilde\Phi}(f,g)
=S_{2,c}^{\psi}(f,g)+\int f\int g,
\qquad
S_{m,c}^{\widetilde\Phi}=S_{m,c}^{\psi}\quad(m\ge3).
\tag{3.9}
\]

The added two-point term is smooth, so all leading singular ultraviolet coefficients are unchanged. Reflection positivity, locality, covariance and a fixed factorial OS bound are retained. The same heat-projection argument now gives all Gaussian polynomial vacuum vectors in the cyclic space, and multiplication by $G$ defeats every global energy bound when $\int f\ne0$.

This second example separates a stronger global energy requirement from energy bounds inside a chosen phase: each fixed-$G$ phase has only an identity shift of the base field. A phase-first construction might avoid this particular mixed-center obstruction. It would still need an actual phase-selection theorem and a proof of the required field bounds in the selected phase; it is not supplied by the Wilson vacuum hierarchy alone.

### 4. Geometry conditions of the proposed time-first limit

**L.** CMP109, p.251, defines the torus with common side parameter $L_\mu=L^m$, with odd $L>11$. Its symmetry discussion on p.269 explicitly restricts to Euclidean transformations preserving the chosen torus. CMP119, pp.243–244, says its geometric definitions are those in the introduction of CMP109 and the preceding papers. The available source text therefore does not provide a stated theorem with an arbitrarily long temporal side at each fixed spatial lattice.

At each fixed spatial lattice, the trace-to-vacuum comparison is valid and allows an arbitrarily long time circle. The missing point is uniform local RG and observable control on that enlarged geometry. A proof that every relevant local construction and global polymer count extends to the rectangular sequence would remove this particular geometric condition. It must also account for the lost global time-space permutation symmetries at finite rectangular volume and prove their restoration locally. Neither the mere locality of individual maps nor the cubic stability theorem by itself performs that check.

No anisotropic lattice-spacing or Hamiltonian-limit construction is introduced here. Changing the temporal lattice spacing independently would be an additional universality problem beyond changing only the torus aspect ratio.

### 5. Remaining operator input after the argument

The decisive estimate is still one of the following, with the actual field normalization and complete history law:

1. Directly prove the reduced periodic OS form bound, uniformly in polynomial vector degree and time-mollifier width.
2. Prove a full interacting physical-time slab norm for the renormalized tensor fields, and also justify its passage from the transfer state to the selected periodic hierarchy.
3. In the scalar coupling channel, prove (R), then use the exact response transforms (1.14)–(1.16); the periodic-state passage and tensor extension still remain.

The old local transfer comparison has a local deletion energy increment. It removes an extensive-volume loss, but after physical normalization leaves an ultraviolet power. Centering only cancels the vacuum expectation; it does not bound the logarithmic response on all low-energy vectors. The source-free pressure theorem and the numerical running coupling do not supply that bound.

A uniform source theorem useful here would have to control the normalized **boundary operator or kernel**, with the vacuum identity subtraction inside the derivative and a sufficient boundary norm. A scalar real pressure estimate, even combined with reflection positivity, does not do so. Nonlinear source counterterms also cannot be discarded from a moment argument. These limitations are already demonstrated by the earlier finite probability examples and are strengthened by Section 3.

The domain/core part is complete, conditional on the insertion estimate. The interacting renormalized operator inequality, its full tensor normalization and any needed phase-first alternative remain open. No part of this note proves four-dimensional Yang–Mills existence.

### Primary sources and exact scope

- T. Balaban, CMP **109** (1987), 249–301, *Renormalization Group Approach to Lattice Gauge Field Theories I*: [DOI](https://doi.org/10.1007/BF01215223). Printed p.251 gives the common-side geometry; p.269 specifies the torus-preserving symmetries.
- T. Balaban, CMP **119** (1988), 243–285, *Convergent Renormalization Expansions for Lattice Gauge Theories*: pp.243–244, for the explicit inheritance of geometric definitions. No rectangular extension is asserted.
- The positive Wilson transfer representation and bare operator conventions are those of Lüscher and Sint. The new response formulas above are proved from that representation; they are not quoted as a published interacting renormalization theorem.
- The graph-core argument is an elementary consequence of the canonical Schwartz Borchers domain, translation covariance and the stated energy graph bounds. The analytic identification it completes retains the precise OS II imports stated in the main paper.


---
