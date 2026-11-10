# A local positive extension of a finite-range precision

Working lemma for catalogue theorem M-04. This is a proved matrix lemma, not a claim that the complete Bałaban precision has already been put into its hypotheses in raw retained coordinates.

## Statement

Let the free-coordinate index graph have bounded degree. Let A(v) be a Hermitian matrix family, with A_ij=0 for dist(i,j)>r, and with

\[
 \sup_v\sup_i\sum_j\|A_{ij}(v)\|\le K.
\]

Suppose every entry has a specified finite raw-retained-variable dependency footprint. Let G be the admitted set on which A(v)≥mI, with m>0. The matrix entries need to be defined and continuously differentiable on the whole retained-coordinate ambient space for this statement. This preliminary extension need not be positive. If the entries are initially defined only on local charts, their extension with the same local footprints and bounds is a separate premise.

Choose a fixed overlapping partition of unity by real spatial multipliers χ_Q, with sum_Q χ_Q(i)^2=1, support χ_Q contained in a bounded cube Q, and

\[
 \sum_Q |\chi_Q(i)-\chi_Q(j)|^2
 \le C_\chi\frac{\operatorname{dist}(i,j)^2}{M^2}
 \quad\text{when dist(i,j)≤r}.
\]

Such partitions can be chosen with fixed overlap on the lattice, for fixed cube side M. Put

\[
 A_Q=P_QAP_Q,
 \qquad E=\sum_Q\chi_Q A_Q\chi_Q-A.
\]

Let φ be a smooth real function equal to the identity on [m,∞) and satisfying φ≥m/2 on [-K,K]. Define

\[
 A^{\rm ext}(v)=\sum_Q\chi_Q\phi(A_Q(v))\chi_Q-E(v).
 \tag{PE.1}
\]

If C_χKr²/(2M²)≤m/4, then:

1. A^ext(v)=A(v) on G.
2. A^ext(v)≥mI/4 at every ambient v.
3. Every summand in (PE.1) has a bounded local raw-variable footprint, namely the union of the entry footprints of A_Q, together with Q. E is finite range and has the original entry footprints.
4. First retained derivatives obey bounds in terms of the corresponding local derivatives of A, with constants depending on m,K,r,M and the fixed partition, not total volume.

## Proof

For v∈G, principal compression gives A_Q(v)≥mI on its coordinate subspace. Functional calculus therefore gives φ(A_Q)=A_Q. Formula (PE.1) then returns A exactly.

For arbitrary v, the spectrum of A_Q lies in [-K,K], by the Schur bound, so φ(A_Q)≥mI/2. Since the χ_Q squares sum to one,

\[
 \sum_Q\chi_Q\phi(A_Q)\chi_Q\ge mI/2.
\]

The error has entries

\[
 E_{ij}=A_{ij}\left(\sum_Q\chi_Q(i)\chi_Q(j)-1\right)
       =-\tfrac12 A_{ij}\sum_Q(\chi_Q(i)-\chi_Q(j))^2.
\]

Thus its absolute row and column sums are at most C_χKr²/(2M²). The symmetric Schur estimate gives the same upper bound for ||E||. Subtraction in (PE.1) leaves A^ext≥mI/4.

A_Q uses only entries whose two indices lie in Q. Smooth functional calculus can mix every index in Q but introduces no retained variable outside the union of their actual footprints. The error E uses only the entry A_ij multiplied by deterministic spatial numbers. This proves the locality statement. In particular the construction does not take a global square root of A and then falsely label it local.

For the derivative bound, select a compactly supported smooth function ψ agreeing with φ on a neighborhood of [-K,K]. The spectral families A_Q remain in this interval. Fourier functional calculus and Duhamel's formula yield

\[
 D\phi(A_Q)[H]
 =\frac1{2\pi}\int\widehat\psi(t)\,i
       \int_0^t e^{i(t-u)A_Q}H e^{iuA_Q}\,du\,dt,
\]

with the integral over a negatively oriented interval when t<0. Consequently

\[
 \|D\phi(A_Q)[H]\|
 \le \frac1{2\pi}\int |t\widehat\psi(t)|\,dt\,\|H\|.
\]

The finite constant is independent of the dimension of A_Q. Set H=∂_v A_Q, differentiate the finite-overlap sum and E, and use the same Schur estimate for ∂_vE. This gives the asserted local derivative control. Finite differences follow by integrating along the stated retained-coordinate curve. ∎

## Application boundary

This construction repairs positivity of a **genuinely local, already defined** precision family. It does not localize a nonlocal minimizing background, supply a common active chart, control a score or a normalizer, or make a global spectral gap imply absolute convergence of an entrywise path expansion. For M-04 it becomes applicable only after the raw-variable finite-range representation and its uniform preliminary extension are actually obtained from the source. A native-background precision is not automatically such a representation.

The extension is smooth rather than analytic in raw v. That is sufficient for the first ambient finite-difference norm, but any argument using complex raw-field analyticity must retain the original analytic local charts or establish a different analytic continuation. Exact equality to an analytic function on an open set together with a nontrivial analytic spectral clipping cannot be asserted.
