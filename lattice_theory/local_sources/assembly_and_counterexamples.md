# Conditional reconstruction from Wilson source derivatives

Fix \(SU(N)\), \(N\ge2\), and count each unoriented plaquette once. Write \(s_p=N-\operatorname{ReTr}U_p\) and take the Wilson weight \(\exp(-\beta_a\sum_p s_p)\), with \(\beta_a=2Nx_{0,a}\). The inverse coupling multiplying \(\sum_p s_p/N\) is \(N\beta_a\). The fields take values in \(E=\operatorname{Sym}^2(\Lambda^2\mathbb R^4)\), of dimension 21. The following implication concerns a single cofinal family of these Wilson measures. Its analytic hypotheses include all large-field histories and the same physical normalization for all source orders.

## Finite source derivatives and local products

For a source \(j\) in a finite-dimensional test family, write \(Z_n[j]\) for its cutoff Wilson integral. Let \(C_n[0]=0\) and put
\[
 \mathcal M_n[j]=e^{-C_n[j]}Z_n[j]/Z_n[0],\qquad
 W_n[j]=\log\mathcal M_n[j].
\]
At any fixed order these identities also make sense as identities of Taylor polynomials, using the truncated exponential and logarithm. Let \(S_{m,n}\) and \(S^c_{m,n}\) be the degree-\(m\) derivatives at zero of \(\mathcal M_n\) and \(W_n\), respectively. For elementary tests,
\[
 S_{m,n}(f_1,\ldots,f_m)
 =\sum_{\pi\in\mathcal P_m}\prod_{B\in\pi}
     S^c_{|B|,n}(f_i:i\in B).
 \tag{1}
\]
This follows by differentiating the exponential. Reflection positivity involves the full moments on the left. Applying (1) to joint Schwartz tests requires a continuous distribution associated with each partition term and estimates for their sum.

Fix a physical scale \(\mu\). The one-field prescription can include a matrix \(Z_{\alpha\beta}(a,\mu)\) and identity terms \(c_{\alpha,a}\int f\). Products can also have local subtractions on partial diagonals. A finite-order distribution supported on a partial diagonal vanishes on a Schwartz test which is flat there. A cutoff approximation with shrinking support needs a quantitative distribution bound to justify that conclusion in the limit. Dependence on source values throughout a fixed physical cell is a different support condition, as the example below shows.

## A sufficient set of hypotheses

Let \(a_n\downarrow0\) and \(T_n\uparrow\infty\) be the spacings and periods of one admitted family. For example \(a_n=L^{-K_n}\ell_0\) and \(T_n=2L^{M_n}\ell_0\) give cofinal sizes for an admitted \(L\) when \(K_n,M_n\to\infty\). Admissibility includes the actual geometric, small-coupling and trajectory conditions of the construction. Write \(\mathcal S_0((\mathbb R^4)^m)\) for Schwartz functions flat with all derivatives on every coincidence \(x_i=x_j\). Give tensor-valued tests the fixed component norm and set
\[
 \nu_s(F)=\max_{|\alpha|\le s}\sup_X
 (1+|X|^2)^{s/2}|\partial^\alpha F(X)| .
 \tag{2}
\]

**J0. Wilson law and trajectory.** The source-free integrations, changes of coordinates, reference measures and positive history decomposition represent the normalized Wilson law exactly on this sequence. The physical-scale trajectory is identified in the same coupling convention, including any uniform Gaussian calibration needed to obtain it.

**J1. Compatible renormalized fields.** At every finite order the full source derivatives on this Wilson law, including the averages over its histories, give distributions \(S_{m,n}\) for a common one-field and product prescription. The subtractions have coincidence support in the limit. The fields obey the specified tensor rules and the finite normalization conditions at \(\mu\).

**J2. Uniform joint-test estimate.** There are fixed constants \(C,p,q\), independent of \(n,m\), for which
\[
       |S_{m,n}(F)|\le C^{m+1}(m!)^p\,\nu_{qm}(F)
       \qquad (F\in\mathcal S_0((\mathbb R^4)^m)).
 \tag{3}
\]
The cutoff distributions here act on a common test space, for example through a periodization compatible with the stated bounds. A derivation starting with separate test factors must justify the passage to this joint-test norm.

**J3. Euclidean symmetries and the positive-time form.** Reality, permutation symmetry and reflection positivity, including the tensor signs, hold in the limit on the Osterwalder–Schrader test algebra. More explicitly, for each finite positive-time vector the cutoff reflected quadratic form has nonnegative limit inferior. Translation defects and, for each fixed \(R\in O(4)\), the defects \(S_{m,n}(R\cdot F)-S_{m,n}(F)\) tend to zero. The tensor action on each field is \(A\mapsto(\Lambda^2R)A(\Lambda^2R)^t\).

**J4. Ultraviolet identification.** In the normalization of J0–J1 the cutoff and increasing-volume limits precede the short-distance limit. Uniform remainders identify the stipulated scalar two-point coefficient and the first nonzero interacting connected three-point coefficient on separated tests. The selected phase must retain these same coefficients. The canonical comparison for \(Q=F^2/4\) has \(c_2=3(N^2-1)/\pi^4\) and \(c_3=11(N^2-1)/(16\pi^8)\) at order \(g^2=N g_{\rm YM}^2\), with the finite matching factors of the physical scalar applied before the comparison.

**J5. Energy bounds and vacuum phase.** The reconstructed fields satisfy the required polynomial energy estimates on a common invariant domain. The hypotheses for vacuum-phase decomposition, its symmetries including the disconnected operations, uniqueness of the vacuum and clustering in the specified phase hold. There is one phase in which the energy estimates and the ultraviolet identification apply together.

**Conditional assembly theorem.** Under J0–J3 a subsequence defines an infinite-volume continuum hierarchy for the stated fields with bound (3), full Euclidean covariance, permutation symmetry and reflection positivity. Corrected Osterwalder–Schrader reconstruction on the indicated test domain gives a relativistic theory, possibly with a degenerate vacuum. Under J4–J5 this theory has a phase with the energy bounds, symmetries and nonzero ultraviolet coefficient specified in the [continuum theorem](../../paper/Yang_Mills_Existence.pdf).

*Proof.* For each order and each label tuple take a countable dense subset of the coincidence-flat Schwartz space. This space is a closed subspace of a separable Schwartz space. Estimate (3) bounds each numerical evaluation. Simultaneous diagonal extraction gives convergence on all the dense sets. Approximation in \(\nu_{qm}\) extends convergence to each test, on the same subsequence, and preserves (3). For a finite positive-time test vector the Osterwalder–Schrader quadratic form is a finite sum of evaluations of full distributions on the corresponding reflected, time-ordered tests. Convergence and the nonnegative lower bound pass to the sum. Permutation, rotation and translation invariance follow from convergence and J3. Exact fine-lattice translations can also be approximated by translations of a fixed test, using continuity in the seminorm in (3). Apply corrected reconstruction with its order-growth hypothesis to this limiting hierarchy. J4 identifies the short-distance laws, and J5 supplies the common field domain and phase to which that identification applies. The phase and operator requirements are used at this final step. [Osterwalder and Schrader, *Axioms for Euclidean Green’s Functions II*, §IV.1](https://doi.org/10.1007/BF01608978).

## Exact transport of source derivatives

Let \(v\) be retained variables and \(u,u'\) old and replacement variables. Let \(h_0(u',v)\ge0\) be a source-independent kernel with \(0<H_0(v)=\int h_0(u',v)\,du'<\infty\) on the active data. For a density \(\rho\) define
\[
   (P_h\rho)(u',v)=\frac{h_0(u',v)}{H_0(v)}\int\rho(u,v)\,du,\qquad
   QF=\frac{P_h(\rho F)}{P_h\rho}
 \tag{4}
\]
on the nonzero support. Sample \((u,v)\) from the normalized old law \(\mu\) and sample \(u'\) conditionally from \(h_0/H_0\). The output law is \(\mu'\), and \(QF\) is conditional expectation given \((u',v)\). Thus \(Q1=1\), \(\int QF\,d\mu'=\int F\,d\mu\), and \(\|QF\|_{L^r(\mu')}\le\|F\|_{L^r(\mu)}\) for \(1\le r\le\infty\). On a positive history lift this applies sector by sector to the positive density, before any signed polymer expansion. The selected coordinates, selectors and underlying reference kernel are fixed throughout the source differentiation.

For a normalized source polynomial \(G=\exp\Psi\) with \(G(0)=1\), put \(G'=QG\), \(\Psi'=\log G'\), where the prime labels the new variables. The derivative rules are
\[
 A'_i=QA_i,\qquad A'_{ij}=QA_{ij}+\operatorname{Cov}_Q(A_i,A_j),
 \qquad A_i=\partial_i\Psi(0),\quad A_{ij}=\partial_i\partial_j\Psi(0).
 \tag{5}
\]
The conditional cumulants appearing at higher order satisfy, for \(A_i\in L^m(\mu)\),
\[
 \int|\kappa_Q(A_1,\ldots,A_m)|\,d\mu'
 \le m!2^{m-1}\prod_i\|A_i\|_{L^m(\mu)} .
 \tag{6}
\]
Indeed, for a partition block \(B\), Jensen followed by Hölder bounds the \(L^{m/|B|}\) norm of \(Q(\prod_{i\in B}A_i)\) by \(\prod_{i\in B}\|A_i\|_m\). Hölder across blocks gives the same bound for every partition term. The sum of their unsigned coefficients is at most the number of ordered partitions, bounded by \(m!2^{m-1}\) by writing a permutation and inserting cuts. This estimate retains the size of the original insertions on its right-hand side. Obtaining (3) still requires spatial estimates and uniform bounds on the physically normalized derivatives.

## Bounded pressures and separated correlations

**A counterterm on one fixed cell.** Let \(A_{a,c}\) be a linear average of the lattice source in a cell \(c\) of fixed side \(\ell_0\). Choose reflection-symmetric normalized cubature with \(A_{a,c}(f)\to\ell_0^{-4}\int_cf\) for smooth \(f\). In a representation that permits a cell-local pressure term \(L_a\) and a compensating remainder \(R_a\), consider
\[
 F_{a,c}(j)=1-\cos(n(a)A_{a,c}(j)),\qquad
 L'_{a,c}=L_{a,c}+F_{a,c},\qquad R'_a=R_a-\sum_cF_{a,c},
 \quad n(a)\longrightarrow\infty.
 \tag{7}
\]
All real-source pressure changes in the separate terms are bounded by 2 per cell and their sum is unchanged. The modification is analytic at every finite cutoff and respects the cell reflections. Take smooth \(f,g\) with disjoint supports in the interior of the same cell and nonzero integrals. Then
\[
  \partial_s\partial_tF_{a,c}(sf+tg)\big|_{0}
       =n(a)^2 A_{a,c}(f)A_{a,c}(g).
 \tag{8}
\]
Using \(L'\) as the counterterm therefore changes the connected two-point function by the negative of (8), whose absolute value diverges at fixed positive separation. A bounded real-source witness on each cell leaves this freedom. Coincidence support or quantitative control of the counterterm derivatives restricts it.

**Two reflected cells.** Give signs \(\sigma,\tau\in\{-1,1\}\) the joint probability \((1+c\sigma\tau)/4\), \(0<c<1\). Reflection interchanges the cells. For \(f(\sigma)=a+b\sigma\) the reflected quadratic form is \(|a|^2+c|b|^2\). Insert \(X_n=n\sigma\), \(Y_n=n\tau\), and use the cell counterterm \(L_n(s)=\log\cosh(ns)\). Direct summation gives
\[
 \mathcal M_n(s,t)=e^{-L_n(s)-L_n(t)}
    \mathbf E e^{sX_n+tY_n}
     =1+c\tanh(ns)\tanh(nt).
 \tag{9}
\]
On real sources \(\mathcal M_n\in[1-c,1+c]\). Its reflection kernel is positive semidefinite, being the sum of the constant rank-one kernel and the rank-one kernel with feature \(\sqrt c\,\tanh(ns)\). Nevertheless,
\[
 \partial_s\partial_t\log\mathcal M_n(0,0)=cn^2.
 \tag{10}
\]
Since the insertions lie in different cells, adding any sum of single-cell counterterms leaves this mixed derivative unchanged. These two finite examples identify the additional information in the separated and joint derivative bounds of J1–J2.

## Reflection positivity after subtractions

Let \(K_{ij}=\mathcal M_0(\Theta\overline f_i+f_j)\) be positive semidefinite for positive-time sources. Suppose a counterterm satisfies \(C(\Theta\overline f_i+f_j)=\overline{C(f_i)}+C(f_j)\). For \(D_{jj}=e^{-C(f_j)}\) the subtracted kernel is \(D^*KD\), hence positive semidefinite. Its finite statement for polynomial vectors follows either by finite differences near zero or by the induced triangular transformation of the positive-time polynomial algebra. Local counterterms with the appropriate reality and reflection rules have this splitting for sources supported strictly away from the reflection plane. Shrinking stencils have the same separation for each fixed positive-time margin at sufficiently fine cutoff. A local source redefinition also preserves this argument when it intertwines reflection and splits additively across the separated half-spaces. These are sufficient hypotheses on the actual field and product prescription in J3.

## Vacuum moments and energy bounds

Let \(A\) be one standard normal random variable and set \(\phi(x)=A\) at all spacetime points. The moments are invariant under Euclidean motions and permutations. The reflected form is \(\mathbf E\,|P(A)|^2\) on polynomial vectors. The full hierarchy acts by \(S_m(F)=\mathbf E(A^m)\int F(X)\,dX\). For \(q\ge6\), estimate (2) bounds the absolute value of the integral by \(C^m\nu_{qm}(F)\), since
\[
       (1+|X|^2)^{-3m}\le\prod_{i=1}^m(1+|x_i|^2)^{-3}.
\]
The one-variable weight is integrable in four dimensions, and the Gaussian moments have factorial growth. The hierarchy thus satisfies a bound of the form (3).

Reconstruction gives \(L^2(\mathbb R,d\gamma)\) for the standard normal law \(d\gamma\), because the polynomials are dense. Time translations act identically, so \(H=0\). For a test with \(\int f\ne0\), \(\phi(f)\) is unbounded multiplication by \(A\int f\), and
\[
          \|\phi(f)(1+H)^{-r}\|=\infty\qquad(r\ge0).
 \tag{11}
\]
Thus the energy assertion in J5 calls for estimates on general polynomial vectors. The example satisfies the vacuum moment and reflection hypotheses used above.

A related distinction occurs in phase selection. Suppose a translation-invariant theory has been decomposed into translation-invariant phases \(\gamma\) with adequate moment integrability. For scalar tests \(f_i\) with \(\int f_i=0\), every phase one-point function vanishes. The total connected three-point function is then the average of the phase connected three-point functions. A nonzero value implies a nonzero value in at least one phase. Retaining the stipulated short-distance coefficient requires control of the short-distance limits in the chosen phase, as specified in J4–J5.
