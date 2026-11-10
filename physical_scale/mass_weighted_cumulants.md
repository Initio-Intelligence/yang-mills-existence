# Continuity of mass-weighted canonical cumulants

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

## 1. The precise issue

A completed component can have a very small positive canonical mass.
Its normalized conditional law therefore need not be uniformly
continuous in an absolute norm on unnormalized measures. In a complete
activity or a complete physical branch, however, the original component
mass may multiply the canonical connected coefficient. That expression
has a stronger continuity property.

The theorem below is an elementary finite-measure statement. Its
application requires verification that the literal source record keeps
the stated mass, that the two measures have been placed on the same raw
space, and that the insertions have the stated uniform envelopes. It
does not assert these properties for every C05 boundary record or every
term of a transformed logarithm.

## 2. A uniform real-measure theorem

Let \(\mu\) be a finite positive measure on a common measurable space
\(\Omega\), and let \(F_1,\ldots,F_m\) be bounded measurable functions,
where \(m\ge1\). Write \(F_B=\prod_{i\in B}F_i\). For \(\mu(1)>0\), set
\[
 \Phi_m(\mu;F_1,\ldots,F_m)
 =\mu(1)\,
   \kappa_{\mu/\mu(1)}(F_1,\ldots,F_m).
 \tag{MW.1}
\]
At \(\mu=0\), define \(\Phi_m=0\).
The total-variation norm convention is
\(\|\sigma\|_{\rm TV}=\sup_{|f|\le1}|\sigma(f)|\).

### Theorem MW.1

For finite positive \(\mu,\nu\),
\[
 \boxed{\quad
 |\Phi_m(\mu;F)-\Phi_m(\nu;F)|
 \le 2^m m!\,\|\mu-\nu\|_{\rm TV}
                       \prod_{i=1}^m\|F_i\|_\infty .
 \quad}
 \tag{MW.2}
\]
In particular the bound is independent of lower bounds for
\(\mu(1)\) and \(\nu(1)\).

**Proof.** The exact cumulant partition identity gives
\[
 \Phi_m(\mu;F)=
 \sum_{\pi\in\Pi_m}(-1)^{|\pi|-1}(|\pi|-1)!\,
   \mu(1)^{1-|\pi|}
            \prod_{B\in\pi}\mu(F_B).
 \tag{MW.3}
\]
First suppose both masses are positive. On
\(\mu_t=(1-t)\mu+t\nu\), put \(a_t=\mu_t(1)\) and
\(\sigma=\nu-\mu\). For a partition with \(r=|\pi|\), differentiation
of its unsigned rational monomial gives one mass derivative and
\(r\) moment derivatives. Positivity gives
\[
 |\mu_t(F_B)|\le a_t\prod_{i\in B}\|F_i\|_\infty,\qquad
 |\sigma(F_B)|\le\|\sigma\|_{\rm TV}
                         \prod_{i\in B}\|F_i\|_\infty .
\]
The derivative is consequently bounded by
\[
 (2r-1)\|\sigma\|_{\rm TV}
                         \prod_i\|F_i\|_\infty.
 \tag{MW.4}
\]
All powers of \(a_t\) cancel. Integrate in \(t\) and sum partitions.
The elementary ordered-partition estimate is
\[
 \begin{aligned}
 \sum_{\pi\in\Pi_m}(2|\pi|-1)(|\pi|-1)!
 &\le 2\sum_{\pi\in\Pi_m}|\pi|!\\
 &=
 2m!\sum_{r=1}^m\
       \sum_{\substack{n_1+\cdots+n_r=m\\n_i\ge1}}
             \frac1{n_1!\cdots n_r!}\\
 &\le 2m!\sum_{r=1}^m{m-1\choose r-1}
 =2^m m!.
 \end{aligned}
 \tag{MW.5}
\]
This proves (MW.2). If one measure is zero, take the same interpolation
on the open interval and use (MW.3) together with
\[
 |\Phi_m(\mu;F)|
 \le \mu(1)\prod_i\|F_i\|_\infty
       \sum_{\pi}(|\pi|-1)! .
 \]
The latter expression tends to zero with \(\mu(1)\). Thus the extension
at zero is continuous and the same bound follows. \(\square\)

The use of an absolute norm on finite measures is intentional. There is
no claim that the unweighted normalized cumulant itself is Lipschitz
with a mass-independent constant.

### Corollary MW.2 — a removed positive tail

If \(0\le\nu\le\mu\) and \((\mu-\nu)(1)\le\varepsilon\), then
\[
 |\Phi_m(\mu;F)-\Phi_m(\nu;F)|
       \le 2^m m!\,\varepsilon
                           \prod_i\|F_i\|_\infty .
 \tag{MW.6}
\]
No lower bound for the mass of the retained sector is required. In
particular, suppressing old histories inside an unnormalized component
can be estimated this way if the complete output coefficient retains
exactly the mass appearing in (MW.1).

## 3. Changing the bounded insertions

The cumulant is multilinear in its insertions. If
\(\|F_i\|_\infty,\|G_i\|_\infty\le M_i\), the same partition formula and
one telescoping replacement at a time give
\[
 \begin{split}
 |\Phi_m(\mu;F)-\Phi_m(\mu;G)|
 &\le 2^{m-1}m!\,\mu(1)
       \sum_{i=1}^m\|F_i-G_i\|_\infty
                         \prod_{j\ne i}M_j .
 \end{split}
 \tag{MW.7}
\]
Indeed \(\sum_\pi(|\pi|-1)!\le
\sum_\pi|\pi|!\le2^{m-1}m!\).
This separates convergence of the actual integration measure from
uniform convergence of the finite-chart insertions.

For unbounded insertions the displayed theorem cannot simply be cited
with an energy moment in place of an \(L^\infty\) norm. One may truncate
the insertions, apply the theorem, and remove their tails only with a
joint uniform-integrability estimate for the measures under comparison.

## 4. A common phase cone

There is a useful complex extension. Suppose two complex measures
\(\mu,\nu\) take values in the same pointwise sector
\(\{z:|\arg z|\le\eta\}\), with \(0\le\eta<\pi/2\), after a common
constant phase rotation. Their convex interpolation remains in that
sector and satisfies
\[
 \|\mu_t\|_{\rm TV}\le(\cos\eta)^{-1}|\mu_t(1)|.
 \tag{MW.8}
\]
The preceding differentiation proof now gives
\[
 |\Phi_m(\mu;F)-\Phi_m(\nu;F)|
 \le 2^m m!(\cos\eta)^{-(m+1)}
       \|\mu-\nu\|_{\rm TV}\prod_i\|F_i\|_\infty .
 \tag{MW.9}
\]
For the mass-derivative term there are \(r\) undifferentiated moment
factors and at most \((\cos\eta)^{-r}\); for a moment derivative there
are \(r-1\). The larger exponent \(m+1\) in (MW.9) is a harmless common
bound. The same zero-mass extension holds, since a sector measure with
zero total mass is the zero measure.

The common sector is a hypothesis. Separate zero-free normalizers or
separate total-variation bounds do not imply it. A source phase proof
must establish the shared cone for the two measures being compared
before this extension is used.

## 5. What this contributes to the source-limit problem

The H02 survival reserve gives absolute old-history tails for positive
unnormalized source operations. A completed source calculation often
introduces canonical expectations by dividing such an operation by its
mass. Estimating the normalized measure first can lose the very factor
that made the old-history tail small.

Equations (MW.2)–(MW.6) show an exact way to avoid that loss whenever the
literal **complete** source coefficient is mass times a canonical
cumulant. The source proof must first keep that complete coefficient,
or show the required cancellation of its denominators. The theorem
then supplies an absolute continuity bound without inventing a uniform
positive lower bound for every rare sector.

This is also useful on a finite volume: one can keep all unnormalized
branch integrals together and divide only by the full partition function,
whose lower bound is already in H2S.14a. It does not by itself prove
continuity through hard-selector boundaries, construct a common raw
pullback for two different histories, control remote component
dependence, or close the mixed \(R\) recursion. Those remain actual
source-identification and compactness questions.
