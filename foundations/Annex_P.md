# Seven-channel running normalization and weighted remainders

**Annex P.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md). Identifying the calibrated Gaussian marginal with the Wilson trajectory also requires GC, including the bounded error uniform in depth.


### Purpose

**P: finite-dimensional product theorem. C: its application to the actual
Yang--Mills observable induction.** The tensor decomposition of Annex D
has a useful consequence for the running product: on the 21 curvature-bilinear components, the full hypercubic
commutant is commutative. A controlled order-\(g^4\) error in an
equivariant *mixing matrix* can therefore be summed without a
noncommuting conjugation loss. This does not establish that the exact
transported fields have the required mixing matrices, and does not sum
arbitrary additive observable remainders.

All assertions here are finite-dimensional derivations. No anomalous
dimension or beta-function coefficient is imported or computed.

### 1. Fixed projectors, including reflections

Let
\[
E=\operatorname{Sym}^2(\Lambda^2\mathbb R^4),\qquad
\dim E=21,
\]
with its invariant Euclidean inner product, and let
\(H_4=(\mathbb Z_2)^4\rtimes S_4\) act by the tensor representation.
The decomposition proved in Annex D consists of seven inequivalent,
absolutely irreducible real summands, with dimensions
\[
1,\ 3,\ 2,\ 6,\ 6,\ 1,\ 2.
\tag{R.1}
\]
Let \(P_\rho\), \(1\le\rho\le7\), be their orthogonal projectors.
They are fixed once the tensor convention is fixed, satisfy
\[
P_\rho P_\sigma=\delta_{\rho\sigma}P_\rho,\qquad
\sum_\rho P_\rho=I,
\]
and every real \(H_4\)-equivariant endomorphism has the form
\[
M=\sum_{\rho=1}^7 m_\rho P_\rho,\qquad m_\rho\in\mathbb R.
\tag{R.2}
\]
Absolute irreducibility is relevant: there are no complex or quaternionic
endomorphism algebras hidden inside the individual summands.
Consequently every two such endomorphisms commute.

The identity field is not included in \(E\). Its additive mixing is
handled in Section 4. The full group includes coordinate reflections;
restricting to a smaller symmetry group can change the commutant.

### 2. Product theorem with a varying leading coefficient

Let \(u_j\ge0\), \(j\ge0\), satisfy
\[
\sum_{j=0}^\infty u_j^2<\infty.
\tag{R.3}
\]
Suppose that the real equivariant matrices \(M_j,\Gamma_j,R_j\) obey
\[
M_j=I+u_j\Gamma_j+R_j,\qquad
\|\Gamma_j\|\le G,\qquad
\|R_j\|\le B u_j^2,
\tag{R.4}
\]
and
\[
0\le u_j\le1,\qquad G u_j+B u_j^2\le\frac12.
\tag{R.5}
\]
A finite initial segment that does not meet (R.5) can instead be
retained as a fixed positive definite equivariant prefactor, provided
that property is separately known. Its constants are then included
in the bounds. It is not discarded. An arbitrary invertible prefactor
preserves convergence and invertibility but need not preserve the
positivity conclusions below.

Define
\[
T_0=I,\qquad
T_n=M_{n-1}\cdots M_0,\qquad
A_n=\sum_{j=0}^{n-1}u_j\Gamma_j,\qquad
V=\sum_{j=0}^\infty u_j^2.
\tag{R.6}
\]

#### Theorem 2.1

Every \(M_j\) and \(T_n\) is positive definite as a matrix on \(E\).
There is a positive definite, equivariant, invertible matrix
\(\mathsf R_\infty\) such that
\[
\boxed{
e^{-A_n}T_n=\mathsf R_n\longrightarrow\mathsf R_\infty.
}
\tag{R.7}
\]
For constants \(C_1,C_2\) depending only on \(G,B\) and the smallness
ceiling in (R.5),
\[
\|\mathsf R_n\|+\|\mathsf R_n^{-1}\|
\quad +\|\mathsf R_\infty\|+\|\mathsf R_\infty^{-1}\|
\le4e^{C_1V},
\tag{R.8}
\]
\[
\|\mathsf R_\infty-\mathsf R_n\|
\le C_2 e^{C_1V}\sum_{j=n}^\infty u_j^2,
\tag{R.9}
\]
and
\[
\boxed{
\|T_n\|+\|T_n^{-1}\|
\le2\exp\!\left(G\sum_{j<n}u_j+C_1V\right).
}
\tag{R.10}
\]
No convergence of \(\Gamma_j\) is required.

**Proof.** Write
\[
M_j=\sum_\rho(1+u_j\gamma_{\rho,j}+r_{\rho,j})P_\rho.
\]
All eigenvalues lie in \([1/2,3/2]\). The real matrix logarithm is
therefore well defined in the same commutative algebra. For
\(|x|\le1/2\),
\[
|\log(1+x)-x|
\le \sum_{k\ge2}|x|^k/k
\le |x|^2.
\]
Since \(u_j\le1\), the elementary estimate, with (R.4), gives
\[
\Delta_j:=\log M_j-u_j\Gamma_j,\qquad
\|\Delta_j\|\le C_1u_j^2.
\tag{R.11}
\]
The explicit choice \(C_1=B+(G+B)^2\) suffices. Any finite terms
outside the ceiling are covered by the prefactor convention.

Every \(\Delta_j\) commutes with every \(\Gamma_k\). Thus the product
identity is exact:
\[
T_n
=\exp\!\left(A_n+\sum_{j<n}\Delta_j\right),\qquad
\mathsf R_n=\exp\!\left(\sum_{j<n}\Delta_j\right).
\tag{R.12}
\]
The sums of \(\Delta_j\) converge absolutely. Taking their exponential
gives (R.7), invertibility and (R.8). For selfadjoint matrices in this
fixed commuting algebra, the scalar mean-value estimate for the
exponential gives (R.9), after increasing the constant if needed.
Finally \(\|A_n\|\le G\sum_{j<n}u_j\), which proves (R.10).
\(\square\)

The proof explicitly separates the generally divergent first-order
sum \(\sum u_j\Gamma_j\) from the convergent second-order correction.
Symmetry alone would not bound the former.

### 3. Logarithmic running on a quantified AF sequence

Assume, in addition, that for fixed \(b>0\), \(\kappa\ge1\),
\[
u_j=\frac1{b(j+\kappa)}+\varepsilon_j,\qquad
|\varepsilon_j|
\le C\frac{\log(j+\kappa+1)}{(j+\kappa)^2},
\tag{R.13}
\]
and that one equivariant matrix \(\Gamma\) satisfies
\[
\Gamma_j=\Gamma+\Xi_j,\qquad
\|\Xi_j\|\le C u_j.
\tag{R.14}
\]
The bounded finite-dimensional eigenvalues of \(\Gamma\) are denoted
\(\gamma_\rho\). These numbers must be obtained from the actual
observable matching theorem before this corollary describes its
renormalization.

#### Corollary 3.1

There is an equivariant positive definite matrix \(L_\infty\) such that
\[
\boxed{
\left(\frac{n+\kappa}{\kappa}\right)^{-\Gamma/b}T_n
\longrightarrow L_\infty,
}
\tag{R.15}
\]
and the difference from its limit is
\[
O\!\left(\frac{\log(n+\kappa+1)}{n+\kappa}\right)
\tag{R.16}
\]
in matrix norm. Here \(x^{\Gamma/b}\) means
\(\sum_\rho x^{\gamma_\rho/b}P_\rho\).

**Proof.** The term \(u_j\Xi_j\) is absolutely summable by (R.3).
The series of \(\varepsilon_j\) converges absolutely, with tail
\(O(\log(n+\kappa+1)/(n+\kappa))\). Also
\[
\sum_{j<n}\frac1{j+\kappa}
-\log\frac{n+\kappa}{\kappa}
\]
has a finite limit with tail \(O((n+\kappa)^{-1})\), as follows by
comparing each reciprocal with the integral over its unit interval.
Substitute these statements and (R.11) in (R.12). All exponents
commute, and the remaining exponent has an absolutely convergent
series with the stated tail. Exponentiation proves the result.
\(\square\)

For a geometric ultraviolet sequence \(a_n=\ell_0L^{-n}\), the
factor \(n^{\gamma_\rho/b}\) is a power of
\(\log(\ell_0/a_n)\). A running normalization can therefore be
defined by the exact inverse \(T_n^{-1}\), while its explicit
channel asymptotics are given by (R.15). Neither \(T_n\) nor its
inverse must remain bounded in the original bare basis.

This corollary does not verify (R.13) for the AF input of the construction,
nor (R.14) for its observable matrices. In particular the
native cumulant coefficient is not silently identified with \(\Gamma\).

#### 3.1 What this says about rotations

If two hypercubic pieces belong to one rotational tensor type, the
ratio of their product eigenvalues has the asymptotic form
\[
\frac{t_{\rho,n}}{t_{\sigma,n}}
=C_{\rho\sigma}
\left(\frac{n+\kappa}{\kappa}\right)^{
(\gamma_\rho-\gamma_\sigma)/b}(1+o(1)),
\qquad C_{\rho\sigma}>0.
\tag{R.17}
\]
Equality of the leading exponents removes this particular relative
power. It does not force the finite constants to agree, nor estimate
any nonlocal or irrelevant rotation defect. Conversely, the running
bare-to-renormalized matrix need not itself be a rotational
intertwiner when its normalization compensates anisotropic cutoff
representatives. The required statement is covariance of the
normalized limiting hierarchy. No rotation-restoration theorem is
claimed from (R.17).

### 4. Identity mixing and positivity of a realized field change

At a finite cutoff, an equivariant affine marginal recursion has the
form
\[
X_{j+1}=M_jX_j+c_j\mathbf1.
\tag{R.18}
\]
The vector \(c_j\in E\) lies in the scalar invariant line, because
\(\mathbf1\) is fixed by the full hypercubic group and that line is
the unique trivial summand in \(E\).

For any chosen initial centering \(v_0\) in that line, set
\[
v_{j+1}=M_jv_j+c_j,\qquad
Y_j=T_j^{-1}(X_j-v_j\mathbf1).
\tag{R.19}
\]
Then \(Y_{j+1}=Y_j\) exactly in this finite-dimensional recursion.
No bound on the bare numbers \(c_j,v_j\) is used.

If such a real field mixing and identity subtraction are implemented
on the actual finite-cutoff positive-time polynomial algebra, with the
reflection action respected, reflection positivity is preserved.
Indeed every new polynomial is an old polynomial obtained by the
same real linear-affine substitution; its OS quadratic form is the
old nonnegative form on that substituted polynomial. At finite source
order this is the corresponding finite triangular substitution.
This is the positivity mechanism already proved for the explicit
field/contact architecture, not a proof that a proposed running
normalization meets the required continuum conditions.

### 5. Why summable matrix errors do not finish marked matching

An exact transported observable generally has an additional
field-valued remainder:
\[
X_{j+1}=M_jX_j+c_j\mathbf1+\mathcal R_j.
\tag{R.20}
\]
After (R.19), the exact identity becomes
\[
\boxed{
Y_{j+1}-Y_j=T_{j+1}^{-1}\mathcal R_j.
}
\tag{R.21}
\]
Therefore the relevant sufficient condition in any fixed normed
space of observable distributions is
\[
\sum_j\|T_{j+1}^{-1}\mathcal R_j\|<\infty.
\tag{R.22}
\]
The matrix theorem estimates the weights in (R.22). It does not
supply the spatial norms, history averages or decay of
\(\mathcal R_j\).

#### Proposition 5.1: raw order-\(u_j^2\) summability can fail

Fix \(A\ge1\) and \(\kappa>2A\). In one real channel, put
\[
u_j=(j+\kappa)^{-1},\qquad
M_j=1-Au_j>0,\qquad
\mathcal R_j=u_j^2.
\tag{R.23}
\]
There is no matrix error in (R.4), and
\(\sum_j|\mathcal R_j|<\infty\). Nevertheless, the normalized
additive increments in (R.21) have a divergent sum.

**Proof.** Summing
\(\log(1-A/(j+\kappa))
=-A/(j+\kappa)+O((j+\kappa)^{-2})\)
gives \(T_j\asymp(j+\kappa)^{-A}\). Hence
\[
T_{j+1}^{-1}\mathcal R_j
\asymp(j+\kappa)^{A-2}>0.
\]
The series diverges for \(A\ge1\), logarithmically at \(A=1\).
\(\square\)

An actual irrelevant gain, for example a bound
\(\|\mathcal R_j\|\le C(j+\kappa)^dL^{-\epsilon j}\)
in the same norm with \(\epsilon>0\), survives every fixed polynomial
weight furnished by (R.10) under the AF hypothesis (R.13), and is
summable. Even (R.3) alone gives
\(\sum_{i<j}u_i\le\sqrt{jV}\); the resulting
\(\exp(G\sqrt{jV})\) weight is still beaten by \(L^{-\epsilon j}\).
Such a gain must be proved for the actual transported remainder; it
is not inferred from its engineering name or from an \(O(g^4)\)
number in a one-shell cumulant expansion.

### 6. Consequence for the running-normalization problem

The finite-dimensional noncommuting-product concern is removed for
the specified fully hypercubic equivariant 21-component marginal
matrices, once the quantitative one-step hypotheses are supplied.
This is an improvement in the running-normalization subproblem F0.
It is not a claim that arbitrary history-dependent insertions have
already been projected onto that commutative algebra.

The missing steps remain the identification of the actual matrices,
their coefficient estimates and prescribed finite normalization;
the compatible contact terms; the weighted remainder estimate
(R.22) with spatial and source-order control; and the complete
history law. M0, F0 and R0 remain open in the full Yang--Mills
construction.


---
