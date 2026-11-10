# Positive-chain tails and exact mesoscopic Wilson matching

**Annex T.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Status, scope, and overlap conditions

The following results concern **M-01** and
**M-02**. M-01 is an abstract positive-kernel theorem. M-02 is an exact matching
theorem on the compact Wilson measure, including all compact configurations.
Neither theorem supplies current-scale moment bounds for the conditional means,
complete-history decay, or the physical renormalization. The full Yang--Mills
existence theorem and the estimates M0/H0 remain open.

The finite-step covariance telescope has a conditional-cumulant interpretation;
a shell estimate of order \(h^{-8}e^{-cr/h}\) controls its separated contribution.
The
history reset and its finite source-jet rule are already proved in Annex I.
Annex O proves one-link-color matching.


The additions are:

1. a reverse-tail realization for arbitrary positive RG/R chains, with
   orthogonal innovations, absolute \(L^2\) summability, and the exact
   infinite-depth terminal term;
2. a matching theorem valid for a growing number of exact eliminations with
   their **true inherited factors**, and for direct mesoscopic block
   elimination. The discrepancy is controlled on joint coincidence-flat tests
   with constants uniform in the elimination depth, cutoff, volume, and source
   order. A reflection-compatible block choice preserves the positive-time
   observable algebra for each fixed support margin.

All length estimates below use the fixed physical reference length as the unit.
Thus \(0<a\le1\). Restoring that length only changes the displayed fixed
constants and the corresponding powers of the reference length.

### 1. M-01: the tail term of a positive RG/R chain

#### Statement and requirements

Let \(X_0,X_1,\ldots\) be a Markov chain on standard Borel spaces, with
source-independent kernels \(P_k\), initial law \(\mu_0\), and marginals
\(\mu_k\). Its state at each step includes every input used by the next
operation, including any retained history variables. The operation may
integrate variables, add labels, change coordinates, or replace variables by
fresh reference variables. It need not be deterministic.

The target is to realize the exact marked transports on a decreasing
path-space filtration, prove their \(L^2\) tail limit, and identify the
terminal covariance without assuming nested state spaces or discarding
replacement noise. The accepted result must retain the tail covariance and
state exactly when it is zero.

#### 1.1 The path-space construction

The same construction starts directly from the observable interface.
Suppose \(Q_k(y,dx)\) is a probability kernel satisfying
\[
\int\mu_{k+1}(dy)Q_k(y,A)=\mu_k(A).
\]
Disintegrate the joint probability
\(\mu_{k+1}(dy)Q_k(y,dx)\) in the opposite direction as
\(\mu_k(dx)P_k(x,dy)\). Standard Borel state spaces ensure that this
forward kernel exists. Thus every such integral-preserving positive
observable kernel, including the exact frozen RG/R kernels, has a
forward Markov realization with the required one-step joint law.

Equip the product path space with the iterated-kernel probability law
\[
\mathbb P(dx_0\,dx_1\cdots)
 =\mu_0(dx_0)P_0(x_0,dx_1)P_1(x_1,dx_2)\cdots .
\tag{1.1}
\]
For a finite chain, extend it by identity kernels after its last state. This
does not change any finite-cutoff observable or the terminal term.

The reverse kernel is the conditional expectation
\[
Q_k f(x_{k+1})
 =\mathbb E[f(X_k)\mid X_{k+1}=x_{k+1}].
\tag{1.2}
\]
The definition is up to \(\mu_{k+1}\)-null sets, which do not affect any
identity. Put \(Q_{0:k}=Q_{k-1}\cdots Q_0\), and \(Q_{0:0}=I\).

For \(F\in L^2(\mu_0)\), define
\[
F_k=Q_{0:k}F,\qquad
M_k^F=F_k(X_k).
\tag{1.3}
\]
Let
\[
\mathcal G_k=\sigma(X_k,X_{k+1},\ldots),\qquad
\mathcal G_\infty=\bigcap_{k\ge0}\mathcal G_k,
\tag{1.4}
\]
where all sigma fields are completed in the path law. The filtration
\(\mathcal G_k\) decreases. It is the **future path** filtration, not the
generally nonnested family \(\sigma(X_k)\).

#### Theorem 1.1 -- reverse-tail realization and orthogonal innovations

For every \(F\in L^2(\mu_0)\):

1. The transported field is the path-space conditional expectation
   \[
   M_k^F=\mathbb E[F(X_0)\mid\mathcal G_k].
   \tag{1.5}
   \]
2. In \(L^2(\mathbb P)\),
   \[
   M_k^F\longrightarrow
   M_\infty^F:=\mathbb E[F(X_0)\mid\mathcal G_\infty].
   \tag{1.6}
   \]
3. Define the innovation
   \[
   \eta_k^F=M_k^F-M_{k+1}^F .
   \tag{1.7}
   \]
   Then
   \(\mathbb E[\eta_k^F\mid\mathcal G_{k+1}]=0\).
   For \(j\ne k\),
   \[
   \mathbb E[\overline{\eta_j^F}\eta_k^G]=0
   \tag{1.8}
   \]
   whenever \(F,G\in L^2(\mu_0)\). Each innovation is also orthogonal to
   every \(\mathcal G_\infty\)-measurable \(L^2\) variable.
4. The exact \(L^2\) expansion is
   \[
   F(X_0)=M_\infty^F+\sum_{k\ge0}\eta_k^F,
   \tag{1.9}
   \]
   and
   \[
   \sum_{k\ge0}\|\eta_k^F\|_2^2
    =\|F\|_{L^2(\mu_0)}^2-\|M_\infty^F\|_2^2.
   \tag{1.10}
   \]

**Proof.** First, the reverse-kernel composition equals conditional
expectation of \(F(X_0)\) given \(X_k\). This follows inductively from the
Markov property: conditioning on \(X_k\), the future transition is
independent of the past. For a bounded cylinder function
\(H(X_k,\ldots,X_N)\), its conditional expectation given
\(X_0,\ldots,X_k\) is a function only of \(X_k\). Hence
\[
\mathbb E[F(X_0)H]
 =\mathbb E[F_k(X_k)H].
\]
A monotone-class argument extends the equality to every bounded
\(\mathcal G_k\)-measurable \(H\), proving (1.5).

For completeness, the \(L^2\) convergence can be seen directly through
orthogonal projections. Let \(V_k=L^2(\mathcal G_k)\); these are decreasing
closed subspaces. If \(l\ge k\), the nesting and the projection identity give
\[
\|M_k^F-M_l^F\|_2^2
 =\|M_k^F\|_2^2-\|M_l^F\|_2^2.
\tag{1.11}
\]
The squared norms decrease to a nonnegative limit, so \(M_k^F\) is Cauchy.
Its limit \(M\) belongs to every \(V_k\), since a tail of the sequence lies
in \(V_k\) and \(V_k\) is closed. One may also choose an almost surely
convergent subsequence of \(M_k^F\). Its pointwise limit, defined by the
limsup of the real and imaginary parts and set to zero on the null
exceptional set, is measurable with respect to every \(\mathcal G_k\):
discarding the finitely many earlier subsequence terms leaves only
\(\mathcal G_k\)-measurable variables. Thus \(M\) has a
\(\mathcal G_\infty\)-measurable version. For every tail-measurable
\(L^2\) variable, the projection identity at finite \(k\) passes to the
limit. It follows that \(M\) is the conditional expectation in (1.6).

Conditioning (1.7) on \(\mathcal G_{k+1}\) gives zero by the nested
projection identity. If \(j<k\), then \(\eta_k^G\) is
\(\mathcal G_{j+1}\)-measurable, so conditioning \(\eta_j^F\) on that sigma
field proves (1.8). The same argument handles a tail-measurable variable.
The finite telescope and (1.6) prove (1.9); orthogonality proves (1.10).
\(\square\)

The completed tail sigma field in this theorem is the decreasing
intersection in the path probability space. No assertion that it equals an
uncompleted coordinate tail sigma field is needed.

#### Corollary 1.2 -- absolutely summable covariance and the exact tail term

Use the sesquilinear convention
\[
\operatorname{Cov}(F,G)
=\mathbb E[\overline{F-\mathbb EF}(G-\mathbb EG)].
\]
Then
\[
\boxed{
\operatorname{Cov}_{\mu_0}(F,G)
=\sum_{k\ge0}
  \mathbb E[\overline{\eta_k^F}\eta_k^G]
 +\operatorname{Cov}(M_\infty^F,M_\infty^G).
}
\tag{1.12}
\]
The series converges absolutely, with
\[
\begin{aligned}
\sum_{k\ge0}
\left|\mathbb E[\overline{\eta_k^F}\eta_k^G]\right|
&\le
\left(\sum_k\|\eta_k^F\|_2^2\right)^{1/2}
\left(\sum_k\|\eta_k^G\|_2^2\right)^{1/2}
\\
&\le
\sqrt{\operatorname{Var}_{\mu_0}(F)
      \operatorname{Var}_{\mu_0}(G)}.
\end{aligned}
\tag{1.13}
\]
The individual term is exactly the integrated one-step conditional
covariance:
\[
\mathbb E[\overline{\eta_k^F}\eta_k^G]
=\int
\left[
Q_k(\overline{F_k}G_k)
-\overline{Q_kF_k}\,Q_kG_k
\right]\,d\mu_{k+1}.
\tag{1.14}
\]
For a finite list of fields the matrix of these terms is positive
semidefinite at every scale.

**Proof.** Apply the orthogonal expansion to the centered fields.
Cauchy--Schwarz first in \(L^2\), then in the scale index, proves (1.13).
Expanding (1.7), conditioning on \(X_{k+1}\), and using (1.2) proves
(1.14). A finite linear combination of innovations has nonnegative
squared norm, giving the matrix assertion. \(\square\)

There is also the stronger unweighted \(L^1\) estimate. Write
\[
D_k(F,G)=
Q_k(\overline F_kG_k)-\overline{Q_kF_k}Q_kG_k.
\]
Then
\[
\boxed{
\begin{aligned}
\sum_{k\ge0}\int |D_k(F,G)|\,d\mu_{k+1}
\le{}&
\bigl[\operatorname{Var}_{\mu_0}(F)
      -\operatorname{Var}(M_\infty^F)\bigr]^{1/2}
\\
&\quad\cdot
\bigl[\operatorname{Var}_{\mu_0}(G)
      -\operatorname{Var}(M_\infty^G)\bigr]^{1/2}.
\end{aligned}
}
\tag{1.14a}
\]
To prove it, use conditional Cauchy--Schwarz:
\[
|D_k(F,G)|\le
\sqrt{D_k(F,F)D_k(G,G)}.
\]
Both diagonal terms are nonnegative and their integrals are
\(\|\eta_k^F\|_2^2,\|\eta_k^G\|_2^2\), respectively. Cauchy--Schwarz
first in the output measure and then in the scale index, followed by
(1.10), proves (1.14a).

This is genuine absolute \(L^1\) summability at each fixed cutoff. It
contains no spatial decay weight and its right side is not automatically
uniform in the ultraviolet cutoff.

#### Corollary 1.3 -- the precise condition for discarding the terminal term

For a specified class \(\mathcal A\subset L^2(\mu_0)\), the terminal
covariance in (1.12) is zero for every pair \(F,G\in\mathcal A\) if and
only if
\[
\mathbb E[F(X_0)\mid\mathcal G_\infty]=\mathbb EF
\quad\text{for every }F\in\mathcal A.
\tag{1.15}
\]
Triviality of \(\mathcal G_\infty\) is sufficient, but is stronger than
needed: it is enough that this tail carries no information about the
chosen initial observable class.

**Proof.** The condition immediately makes every terminal covariance zero.
Conversely take \(G=F\). Zero terminal variance says exactly that the
conditional expectation is almost surely constant; its constant is its
preserved mean. \(\square\)

For the identity chain \(X_k=X_0\), every innovation is zero and the entire
original covariance is the tail term. Therefore arbitrarily many positive
steps do not, by themselves, eliminate the terminal contribution.

#### 1.2 Consequence and remaining spatial input

For finitely many scales, (1.12) reduces to the already-proved finite
telescope. Its additional content is the tail realization and the absolute
unweighted \(L^1\) summability of the conditional covariance kernels,
valid with replacement noise and arbitrary positive history resets included.

Suppose the exact renormalized transported fields additionally satisfy the
localized shell and terminal bounds M2a--M2b of the earlier reduction:
\[
\int|D_{k,n}(x,y)|\,d\mu_{k+1,n}
\le B h_k^{-8}(1+\log(\ell_0/h_k))^b e^{-c|x-y|/h_k},
\tag{1.16}
\]
and a terminal covariance bound of order \(B\ell_0^{-8}\).
The previously proved geometric scale sum then gives the separated
\(|x-y|^{-8}\) bound with the corresponding logarithm.


The new \(L^2\) identity does not prove (1.16). At a microscopic cutoff the
available bound on a dimension-four insertion still carries \(a^{-4}\),
so its squared \(L^2\) norm can carry \(a^{-8}\). Absolute summability at
each fixed cutoff does not make its total uniform as \(a\to0\), and no
spatial distance appears in (1.13). In the stopped physical-scale
construction the identity extension retains exactly the coarse covariance
that must be bounded.

### 2. M-02: exact elimination with the inherited factors retained

#### Statement and requirements

Start from the actual compact \(SU(N)\) Wilson law and the explicit
dimension-four field family with the already-proved microscopic moment
budget. Eliminate local variables through their **actual** conditional laws.
The target is an all-order matching estimate for repeated eliminations,
with an explicit locality radius and fixed \(q,p\) in the joint test norm.

The statement requires: exact formulas for the inherited marginal factors;
no assumption that they remain Wilson plaquette factors; a support proof
for the full-product discrepancy; constants independent of the number of
layers in the stated range; and a concrete admissible geometry. The
renormalized coefficient budget is not to be silently supplied by the
word “field.”

#### 2.1 Finite positive factor laws

Consider a finite collection \(\mathcal V_r\) of remaining compact link
variables. Suppose its actual marginal has density
\[
\mu_r(dU)
=Z_r^{-1}
\prod_{A\in\mathcal F_r}\psi_A(U_A)
\prod_{l\in\mathcal V_r}dU_l,
\qquad \psi_A>0,
\tag{2.1}
\]
where the \(\psi_A\) are continuous on their compact domains. Multiplicity
of factors with the same scope is allowed. This class includes the original
Wilson law and all marginals constructed below.

Choose \(\Gamma_r\subset\mathcal V_r\) such that
\[
|A\cap\Gamma_r|\le1
\quad\text{for every }A\in\mathcal F_r.
\tag{2.2}
\]
For \(l\in\Gamma_r\), set
\[
N_r(l)=
\bigcup_{\substack{A\in\mathcal F_r\\l\in A}}(A\setminus\{l\}),
\qquad
\Psi_l(U_{N_r(l)})
=\int\prod_{A\ni l}\psi_A(U_A)\,dU_l .
\tag{2.3}
\]
An isolated eliminated variable contributes the constant factor one.

#### Lemma 2.1 -- exact inherited factors and locality recurrence

The true marginal on \(\mathcal V_{r+1}=\mathcal V_r\setminus\Gamma_r\)
has exactly the factors
\[
\{\psi_A:A\cap\Gamma_r=\varnothing\}
\quad\text{and}\quad
\{\Psi_l:l\in\Gamma_r\}.
\tag{2.4}
\]
Its conditional elimination kernel is a product over \(l\in\Gamma_r\),
with the exact normalized local factors in (2.3).

If every old factor scope has torus diameter at most \(d_ra\), then every
new factor scope has diameter at most
\[
d_{r+1}a,\qquad d_{r+1}\le2d_r.
\tag{2.5}
\]
If a mark is supported within radius \(R_ra\) of its original anchor,
its conditional expectation is supported within radius \(R_{r+1}a\),
where
\[
R_{r+1}\le R_r+d_r.
\tag{2.6}
\]
Consequently one may take
\[
d_r=2^r d_0,\qquad
R_r=R_0+d_0(2^r-1).
\tag{2.7}
\]

**Proof.** Because of (2.2), every affected factor is assigned to a unique
eliminated variable. The conditional density is therefore the product
of its one-variable factors and the integrals factor. This gives
(2.3)--(2.4) exactly. Every new factor is finite, strictly positive and
continuous by compactness and integration.

Two variables in \(N_r(l)\) lie in old scopes that both contain \(l\),
so their distance is at most \(2d_ra\), proving (2.5). A mark only uses
the elimination kernels of the variables in its own current support.
Each such kernel depends on retained variables at distance at most
\(d_ra\) from the eliminated variable. This proves (2.6) and then (2.7).
\(\square\)

There is no uniform lower bound on the local denominator in this proof,
and none is needed for the later \(L^p\) estimate. Conditional contraction
is with respect to the actual joint law.

Admissible nonempty layers always exist. Form the graph whose vertices are
remaining links and whose edges join links in a common factor scope. Its
degree is at most the number of lattice links in a radius-\(d_ra\) ball,
minus one, hence at most \(C_d(1+d_r)^4\), independently of the torus
volume. A greedy proper coloring has at most one more than this many
colors. Each color class satisfies (2.2); the largest has at least the
reciprocal fraction of all remaining links. This proves existence of a
layer at each step, not a fixed positive elimination fraction uniformly in
the number of steps.

#### 2.2 The full-moment discrepancy

Let the original finite family satisfy
\[
\|O_{\alpha,a}(x)\|_{L^p(\mu_0)}
\le C_0 a^{-4}p,\qquad p\ge1,
\tag{2.8}
\]
and have support radius \(R_0a\). The explicit field budget is that of
Annex O, Theorem 6.2:
\[
O_{\alpha,a}
=\beta\widetilde q_{\alpha,a}
-\mathbb E[\beta\widetilde q_{\alpha,a}]
\tag{2.9}
\]
for the scalar-repaired 21-component family. A different field
normalization must satisfy its own version of (2.8).

Let \(Q_r\) be the true conditional expectation eliminating
\(\Gamma_r\), and put
\[
O^{(r)}_{\alpha,a}=Q_{r-1}\cdots Q_0 O_{\alpha,a}.
\tag{2.10}
\]
The marginal sigma fields are nested for these deterministic eliminations,
so (2.10) is also the direct conditional expectation of the original mark
given all variables remaining after \(r\) steps. In particular,
\[
\|O^{(r)}_{\alpha,a}(x)\|_{L^p(\mu_r)}
\le C_0a^{-4}p
\tag{2.11}
\]
with no loss depending on \(r\).

Define
\[
D^{[r]}_{m,a}(\boldsymbol x)
=
\mathbb E_{\mu_0}\prod_{i=1}^m O_{\alpha_i,a}(x_i)
-
\mathbb E_{\mu_r}\prod_{i=1}^m O^{(r)}_{\alpha_i,a}(x_i).
\tag{2.12}
\]

#### Theorem 2.2 -- repeated exact matching in a shrinking strip

For every finite \(r\), every \(m\ge2\), and every field-label tuple,
\[
\boxed{
|D^{[r]}_{m,a}(\boldsymbol x)|
\le C^{m+1}m!\,a^{-4m}
\mathbf 1_{\{\min_{i<j}d_T(x_i,x_j)\le2R_ra\}} .
}
\tag{2.13}
\]
The constant is independent of \(r\), the volume, \(a\), and \(m\).
Moreover \(D^{[r]}_{1,a}=0\).

Suppose
\[
R_{r(a)}a\le R_*a^\alpha,\qquad 0<\alpha\le1,
\tag{2.14}
\]
with \(R_*\) fixed. For any fixed \(\delta>0\), set
\[
q=\max\left\{5,\,
\left\lceil\frac{4+\delta}{\alpha}\right\rceil+1\right\}.
\tag{2.15}
\]
Use the joint Schwartz seminorm
\[
\nu_s(F)=\max_{|\gamma|\le s}\sup_{X\in\mathbb R^{4m}}
(1+|X|^2)^{s/2}|\partial^\gamma F(X)|.
\]
Coincidence flatness means that every derivative vanishes on each pair
diagonal \(x_i=x_j\).
Then on coincidence-flat joint Schwartz tests, embedded in a central
nonwrapping torus patch,
\[
\boxed{
\left|
a^{4m}\sum_{\boldsymbol x}
D^{[r(a)]}_{m,a}(\boldsymbol x)F(\boldsymbol x)
\prod_i\zeta_T(x_i)
\right|
\le
a^\delta C_{\alpha,\delta}^{m+1}m!\,\nu_{qm}(F).
}
\tag{2.16}
\]
Here \(0\le\zeta_T\le1\) is supported in a central cube of side at most
\(T/2\), and may equal one on expanding compact subsets. The result holds
without \(\zeta_T\) for compact tests in the same nonwrapping patch.
The constants can depend on \(R_*\) and on the fixed original stencil.
The torus side is assumed larger than a fixed multiple of these radii.

**Proof of support.** At one step, if the current supports of the marks
share no eliminated variable, their conditional expectations factor
because the elimination kernel is a product. Hence the full-moment
discrepancy at that step vanishes unless two current marked stencils
overlap on an eliminated variable. Their anchors must then be at distance
at most \(2R_ka\). Telescoping the full-moment expectations for
\(0\le k<r\), and using \(R_k\le R_r\), proves the support assertion.
This use of the telescope keeps every generated product response.

**Proof of magnitude without a depth loss.** Estimate (2.12) directly at
its two endpoints, rather than summing the separate magnitude bounds:
\[
\begin{aligned}
|D^{[r]}_{m,a}|
&\le
\prod_i\|O_{\alpha_i,a}\|_m
+\prod_i\|O^{(r)}_{\alpha_i,a}\|_m
\\
&\le 2C_0^m m^m a^{-4m}
\le C^{m+1}m!a^{-4m}.
\end{aligned}
\tag{2.17}
\]
Thus no factor \(r\) appears, even if \(r=r(a)\to\infty\). The one-point
identity is preservation of each mean.

**Proof on joint tests.** At a contributing configuration choose one pair
with separation at most \(2R_*a^\alpha\). Move only the four-vector
coordinate of one member of that pair to the other. Put
\[
N_m=\left\lceil\frac{4m+\delta}{\alpha}\right\rceil.
\tag{2.18}
\]
Every Taylor coefficient of lower order is zero by coincidence flatness.
The integral Taylor remainder and \(N_m\le qm\) give
\[
|F(X)|
\le
C_{\alpha,\delta}^{m+1}a^{4m+\delta}
(1+|X|^2)^{-qm/2}\nu_{qm}(F)
\tag{2.19}
\]
on the strip. The displacement is in a single four-dimensional
coordinate; its directional multi-index sum costs a constant to the
power \(N_m\), rather than an additional \(m^{N_m}\). The factorial in
the Taylor remainder only improves the bound. The intermediate points
are at a fixed bounded distance from \(X\), so replacing their Schwartz
weight by the one at \(X\) costs \(C^{qm}\).

Since \(q>4\),
\[
a^{4m}\sum_{\boldsymbol x}
(1+\textstyle\sum_i|x_i|^2)^{-qm/2}
\le
\left[
a^4\sum_{x\in a\mathbb Z^4}(1+|x|^2)^{-q/2}
\right]^m
\le C_q^m.
\tag{2.20}
\]
Combining (2.13), (2.19), and (2.20) proves (2.16).
No derivatives of \(\zeta_T\) enter. \(\square\)

#### Corollary 2.3 -- logarithmically many admissible layers

With the exact inherited factor recurrence (2.7), any choice
\[
r(a)\le(1-\alpha)\log_2(a^{-1})
\tag{2.21}
\]
satisfies (2.14), after increasing the fixed radius constant. In
particular, for
\[
r(a)\le\tfrac12\log_2(a^{-1})
\]
one obtains
\[
\boxed{
|D^{[r(a)]}_{m,a}(F)|
\le a^{1/2}C^{m+1}m!\,\nu_{10m}(F).
}
\tag{2.22}
\]

This is a growing-depth result for exact microscopic eliminations. It does
not assert that the sequence performs a complete block RG integration or
removes a fixed fraction of all links at every stage. In particular,
(2.21) keeps the total support radius shrinking to zero, rather than
reaching the fixed physical scale \(\ell_0\).

### 3. A concrete mesoscopic block elimination on the Wilson law

The following geometry gives an explicit substantial elimination rather
than only existence of single-link color classes.

Let the periodic fine lattice have \(n\) sites on every axis. Choose an
integer \(b\ge2\) dividing \(n\). Retain every link with at least one
endpoint on one of the coordinate planes
\[
x_\mu=kb,\qquad k\in\mathbb Z,\quad \mu=1,\ldots,4,
\tag{3.1}
\]
in lattice units. Eliminate all other links. They split into the interiors
of the \(b\)-side coordinate blocks.

#### Lemma 3.1 -- exact block conditional independence

Conditional on the retained links, the eliminated variables in different
blocks are independent under the actual compact Wilson law. The factor
inside a block is its complete compact conditional integral with the
specified retained boundary data.

**Proof.** An elementary plaquette has coordinate width at most one fine
lattice unit in each direction. It cannot contain an eliminated interior
link from each of two different blocks: two strictly interior coordinate
levels on opposite sides of a boundary plane are separated by at least
two lattice units. Consequently every Wilson plaquette factor meets
eliminated links in at most one block. Group the plaquette factors
according to that block and integrate product Haar measure. The full
conditional law factors exactly. \(\square\)

An initial radius-\(R_0a\) mark may meet several blocks. Its projected
conditional expectation depends only on the retained links of those
blocks and the original retained stencil. Its support radius is at most
\[
R_0a+2ba+d_0a,
\tag{3.2}
\]
for a fixed plaquette constant \(d_0\).

#### Theorem 3.2 -- full-Wilson mesoscopic matching

Let \(Q_b\) be the exact conditional expectation over all eliminated block
interiors and \(\widehat O_{\alpha,a}=Q_bO_{\alpha,a}\). If
\[
ba\le C_*a^\alpha,\qquad 0<\alpha\le1,
\tag{3.3}
\]
then the full-moment difference between the original fields and the
\(\widehat O_{\alpha,a}\) obeys (2.16), with the same \(q\) in (2.15)
and the same factorial exponent \(1\).

For \(\alpha=\delta=\tfrac12\),
\[
\boxed{
|S_{m,a}(F)-\widehat S_{m,a}(F)|
\le a^{1/2}C^{m+1}m!\,\nu_{10m}(F).
}
\tag{3.4}
\]
All 21 field components and every fixed \(SU(N)\) in the Wilson reserve
are included.

**Proof.** If the sets of eliminated blocks met by distinct original
marks are pairwise disjoint, block conditional independence gives
equality of the conditional product and the product of conditional
means. Otherwise two marks meet the same eliminated block. Their
anchors are at distance at most
\[
2R_0a+2ba.
\]
Thus the difference is supported in a strip of radius \(Ca^\alpha\).
Conditional contraction proves its endpoint magnitude bound (2.17)
without a factor depending on the number of eliminated blocks or on
the number of variables in a block. The proof of (2.16) now applies
unchanged. \(\square\)

On the cofinal family \(a=L^{-K}\), \(n=2L^{K+M}\), choose
\[
b=L^{\lfloor K/2\rfloor}.
\tag{3.5}
\]
It divides \(n\), and \(ba\le\sqrt a\), so (3.4) applies.

The retained set is sparse in the following exact quantitative sense.
There are at most
\[
n^4[1-(1-1/b)^4]\le4n^4/b
\tag{3.6}
\]
vertices on the boundary planes. At most eight positively oriented or
incoming links touch each vertex, so the number of retained links is at
most \(32n^4/b\). Since the full lattice has \(4n^4\) links, the retained
fraction is at most \(8/b\). Thus for (3.5) the fraction tends to zero.
This count does not assert any weak-coupling or locality estimate on the
strength of the induced boundary factors.

### 4. Reflection compatibility of the block projection

Assume the original Wilson torus has even side length in fine lattice
sites and carries the standard site-reflection-positive Wilson measure.
The cofinal geometry \(n=2L^{K+M}\) has this property.

Choose the plane family (3.1) with the site-reflection plane at time zero
among its boundary planes. The retained set is invariant under that
reflection. Let \(\Theta\) include the original Wilson reflection and the
specified action on the field labels.

#### Corollary 4.1 -- positive-time algebra for a fixed margin

The block conditional expectation commutes with reflection:
\[
Q_b(\Theta F)=\Theta(Q_bF).
\tag{4.1}
\]
For sources whose original anchors have a fixed positive-time margin
\(\epsilon>0\) from both reflection planes, the projected fields remain
functions of positive-time links when the support bound (3.2) is smaller
than \(\epsilon\). Their polynomial Gram forms are therefore
reflection positive under the original Wilson measure, and hence under
the retained marginal.

**Proof.** Reflection preserves the original law and the retained sigma
field. The defining integral identity for conditional expectation,
tested against retained measurable functions and then reflected, proves
(4.1). The exact support estimate (3.2) places the projected fields in
the same positive-time observable algebra for small enough \(a\).
Every finite polynomial in them is then an allowed positive-time
observable for the original Wilson reflection inequality. Its
expectation under the retained marginal equals its expectation under
the original measure. This proves the claim. \(\square\)

The conclusion is for each fixed positive support margin, as needed in
passage to the continuum OS algebra. The selected block grid does not
preserve every fine-lattice translation. A translation-covariant
continuum limit still requires the common distribution bounds and the
identification with the original hierarchy. Nor is reflection
positivity asserted for arbitrary elimination sequences in Section 2.

### 5. What these two theorems do and do not establish

M-01 identifies exactly where a terminal covariance survives an unlimited
sequence of positive replacements. It removes an ambiguity about
filtrations and gives a useful cutoff-level \(L^2\) accounting identity.
It does not remove the ultraviolet loss or prove spatial decay.

M-02 establishes that the original full hierarchy on coincidence-flat
tests may be replaced, with a quantitative vanishing error, by the
hierarchy of conditional means on an explicitly sparse mesoscopic
skeleton. The effective boundary measure is the exact Wilson marginal,
and all its induced factors are retained. This is an actual-model
matching theorem, beyond the one-link-color layer of Annex O.

The following statements remain false as deductions from M-02 alone:

- that the conditional means now obey an \(h^{-4}\) budget with
  \(h=ba\); their proved budget is still \(a^{-4}\);
- that their retained marginal is a Wilson measure at a new coupling;
- that the resulting effective action obeys the complete Balaban
  activity norms, with all current-coordinate domains admitted;
- that arbitrary fine-lattice running factors preserve (3.4) without
  their own coefficient budget;
- that a uniform Schwinger bound follows from the vanishing matching
  error when neither of the two compared hierarchies has yet been
  bounded uniformly.

These are the remaining analytic problems, not consequences of positivity
or exact conditioning.


---
