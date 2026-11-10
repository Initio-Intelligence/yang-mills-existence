# Cross-shell Gaussian source transport and local vacuum

## 1. Result, exact model, and scope

This note closes the cross-shell gap left in [Finite-source Gaussian vacuum locality](gaussian_source_locality.md) for the **whole flat quadratic curvature model**, including its terminal coarse Gaussian. It does not replace the literal physical source by a sum of separate shell sources. The argument retains every bilinear cross term, proves an exact Schur-complement flow on a fixed source ball, and gives a torus-independent cell-collar vacuum with a remainder bounded by the number of active physical cells.

The model is the product of the source-zero, identity-background Gaussian fluctuation references, read back into the original fine curvature space by the flat constrained minimizers. The terminal physical Gaussian is also included. Arbitrary positive shell coefficients bounded below are allowed. If all coefficients are equal, the resulting curvature law is exactly the finite-torus free Maxwell Gaussian on exact two-forms, with one copy per color. The quotient by gauge and harmonic potential directions is taken before writing this curvature Gaussian; no physical curvature mode is deleted.

The new mechanism is energy orthogonality. The reconstructed covariance of each normalized shell is an orthogonal projection in the physical curvature energy space. These projections are mutually orthogonal. Consequently their weighted sum has a cutoff-independent operator norm, even though the sum of the absolute row norms of the scale kernels can grow with the number of scales. The proof uses the former fact throughout.

For the full source determinant, loops escaping a physical cell collar are estimated with **two localized Hilbert–Schmidt factors** and bounded operators between them. A smooth finite-range Schur multiplier supplies a near/far decomposition with norms independent of cutoff. The proof never replaces a product of operator kernels by an uncontrolled absolute row sum. Exact projection identities also give trace-class decay between separated copies, which controls the periodization error. The terminal Gaussian has a bounded physical rank per cell; its source-dressed quadratic form remains supported on the original source sites. This controls its entire determinant at physical volume.

The labels are **P** for a proof in the stated model, **L** for a primary result at the cited printed location with its hypotheses checked, **C** for an explicitly conditional application, and **O** for an unproved full-theory step. The B99 derivative and unit-covariance estimates used below are those on pp.422 and 432. Section 6 records the gauge conversion and normalization in detail.

**Full R1 and R2 remain O.** The theorem here proves a genuine all-scale Gaussian source locality and normalization statement. Nonlinear reconstruction, cutoffs, mixed regular/erased-R histories, their old physical readouts, and their vacuum and dimension-four projections are absent from this quadratic model. Their admission cannot be inferred from Gaussian orthogonality. The theorem also does not identify the running Gaussian coefficient with N2-F without the remaining R0 dictionary.

## 2. Orthogonal physical shells and the literal quadratic source

### 2.1 The energy space and nested constraints

Use the physical fine inner product \(a^4\sum_x\), with a fixed orthonormal color basis for \(\operatorname{tr}=\operatorname{Tr}/N\). Let \(\mathscr H_a\) be the real Hilbert space of six positively ordered curvature components per color. Let \(\mathscr E_a=\operatorname{ran}d_a\) be the subspace of exact lattice two-forms. All spaces in this paragraph are finite-dimensional on the torus.

Let \(Q_r\), \(0\le r\le K\), be the composed flat straight block constraints, in consistent physical coordinates, with \(Q_0=I\). Multiplication by a nonzero scale factor in the value of an individual constraint does not change its kernel. The nesting is \(Q_{r+1}=Q_{1,r}Q_r\). Define the physical fluctuation subspaces and their orthogonal complements by

\[
 \mathscr K_r=\{d_aA:Q_rA=0\},\qquad
 \mathscr M_r=\mathscr E_a\cap\mathscr K_r^\perp,\qquad
 \mathscr S_r=\mathscr K_r\cap\mathscr K_{r-1}^{\perp}
 \quad(1\le r\le K).
 \tag{CSG.1; P: definitions}
\]

The fine potential may be quotiented by any remaining zero-energy directions when constructing its minimizer. The definition of \(\mathscr K_r\) is a definition by actual admissible potentials; it does not discard a coarse constraint merely because it is gauge related to another one. The physical equivalence of the covariant and straight constraints is checked in §6.

Let \(H_rB\) be an energy minimizer subject to \(Q_rA=B\), where the energy is \(\|d_aA\|_{\mathscr H_a}^2\). Its physical curvature is unique. First variation against \(Q_rA=0\) proves that its curvature lies in \(\mathscr M_r\). Every admissible \(A\) decomposes into \(H_rQ_rA\) and a \(Q_r\)-zero fluctuation, with orthogonal curvatures. Consequently

\[
 \mathscr E_a
  =\mathscr S_1\mathbin{\perp}\cdots\mathbin{\perp}\mathscr S_K
      \mathbin{\perp}\mathscr M_K,\qquad
 P_rP_s=0\ (r\ne s),\qquad
 \sum_{r=1}^KP_r+P_{\rm t}=P_{\mathscr E_a}\le I .
 \tag{CSG.2; P}
\]

Here \(P_r\) and \(P_{\rm t}\) are the orthogonal projections onto \(\mathscr S_r\) and \(\mathscr M_K\).

For completeness, the physical range of the \(r\)-th one-step fluctuation is exactly \(\mathscr S_r\), not merely a subspace of it. If \(Q_{1,r-1}B=0\), then \(H_{r-1}B\) satisfies \(Q_rH_{r-1}B=0\), and its curvature is perpendicular to \(\mathscr K_{r-1}\). Conversely, for \(d_aA\in\mathscr S_r\) with \(Q_rA=0\), decompose at level \(r-1\). Orthogonality to \(\mathscr K_{r-1}\) forces the old fluctuation curvature to vanish. Hence \(d_aA=d_aH_{r-1}Q_{r-1}A\), with \(Q_{1,r-1}Q_{r-1}A=0\).

A centered Gaussian on a subspace with quadratic density \(\exp(-\|F\|^2/2)\), relative to its induced Euclidean volume, has covariance equal to the orthogonal projection onto that subspace. Thus, after integrating pure gauge coordinates, the normalized flat shell curvature covariance is precisely \(P_r\). Its physical scale is \(h_r=L^ra\): the older step length \(h_{r-1}\) in the one-step formula differs by the fixed factor \(L\), which only changes the constants in the kernel bound.

The terminal space is the physical image of the retained coarse potentials. Therefore

\[
 \operatorname{rank}P_{\rm t}
      \le 4(N^2-1)N_T,\qquad
 N_T=(T/\ell_0)^4 .
 \tag{CSG.3; P}
\]

Gauge and harmonic redundancies can reduce this rank. The upper bound alone is used.

### 2.2 The quantitative shell kernel

The argument in §6 gives a common infinite-lattice projection \(P_r^\infty\), its exact finite-torus periodization \(P_r^T\), and

\[
 \begin{aligned}
 \|P_r^\infty(x,y)\|
   &\le A h_r^{-4}e^{-\mu|x-y|_1/h_r},\\
 P_r^T(x,y)
   &=\sum_{n\in\mathbb Z^4}P_r^\infty(x,y+nT).
 \end{aligned}
 \tag{CSG.4; P from the checked flat B99 bounds and the common-kernel dictionary}
\]

The constants depend on \(N,L\) and the fixed blocking choices, not on \(a,r,K,T\). All \(P_r^\infty\) are mutually orthogonal projections on the common fine curvature Hilbert space. Each has block period \(h_r\). The proof of orthogonality is algebraic as above; the exponential estimate is a separate quantitative input, not a consequence of orthogonality.

### 2.3 Full source and optional clover readout

Let \(X_r,X_{\rm t}\ge X_*>0\). Let \(\zeta_r\) and \(\zeta_{\rm t}\) be independent centered Gaussians with covariances \(P_r\) and \(P_{\rm t}\). Let \(\mathcal B\) be either the identity curvature readout or the stacked plaquette/clover readout \(\mathcal B F=(F,\mathcal A_{\rm cl}F)\). At flat background, \(\mathcal A_{\rm cl}\) is the arithmetic average of the four correctly oriented neighboring plaquette curvatures. It is a fixed finite stencil with norm at most one. In particular \(\|\mathcal B\|\le\sqrt2\) in the stacked convention. Define

\[
 \begin{aligned}
 \xi&=\mathcal B\left(
       \sum_{r=1}^KX_r^{-1/2}\zeta_r
                 +X_{\rm t}^{-1/2}\zeta_{\rm t}\right),\\
 C_{\rm u}
    &=\mathcal B\left(\sum_{r=1}^KX_r^{-1}P_r\right)\mathcal B^*,\qquad
 C_{\rm t}=X_{\rm t}^{-1}\mathcal BP_{\rm t}\mathcal B^*,\qquad
 C=C_{\rm u}+C_{\rm t},\\
 V_J(\xi)&=\tfrac12\langle\xi,J\xi\rangle
          =\tfrac{a^4}{2}\sum_x\xi(x)^{\mathsf T}J(x)\xi(x).
 \end{aligned}
 \tag{CSG.5; P: the full physical Gaussian model}
\]

The bounded complex symmetric matrix \(J(x)\) acts by multiplication on the readout space. All cross-shell terms in \(V_J\) are present. Orthogonality gives the crucial uniform bounds

\[
 0\le C_{\rm u},C_{\rm t},C\le M I,\qquad
 M=\|\mathcal B\|^2X_*^{-1}.
 \tag{CSG.6; P}
\]

At constant \(X_r=X_{\rm t}=X\), the unstacked covariance is \(X^{-1}P_{\mathscr E_a}\). This is the full free Maxwell curvature Gaussian, rather than a set of independent surrogate curvature components.

In the literal P2 source normalization, use the same fine source locations as the plaquettes and clovers. With \(I=(\mu,\nu)\), \(\mu<\nu\), the stacked matrix is

\[
 J_{\rm phys}(x)=
   \operatorname{diag}\!\left(
      N j^{(0)}(x) I_{6(N^2-1)},
      -8N\,[j^{IJ}(x)]_{I,J}\otimes I_{N^2-1}
   \right).
 \tag{CSG.7; P: the scalar/clover quadratic-source conversion}
\]

Indeed the plaquette quadratic term is
\(s_p^{[2]}=Na^4|\xi_{\rm pl}(p)|^2/2\), while
\(Q_{IJ}^{[2]}=-Na^4\,\xi_{{\rm cl},I}\cdot\xi_{{\rm cl},J}\).
P2 sums over all ordered antisymmetric index pairs, giving the factor four; the source convention in (CSG.5) supplies the additional factor two. The actual curvature fluctuation multiplier is \(X_r^{-1/2}\). At bare level \(X_0=N\beta_a=2N^2x_0\). No running identification with N2-F is made here.

## 3. Exact Schur transport retains every cross-shell term

Let \(C_A\) be the covariance of any already integrated subset of the independent flat shells, after the common readout \(\mathcal B\). Let \(v\) denote the sum of all remaining readouts, or a fixed retained curvature. If \(\|C_A\|\|J\|<1\), define

\[
 \mathfrak J_A[J]=J(I-C_AJ)^{-1}
      =(I-JC_A)^{-1}J,\qquad
 \mathfrak F_A[J]=-\tfrac12\log\det(I-C_AJ),
 \quad \mathfrak F_A[0]=0 .
 \tag{CSG.8; P: definitions on the branch at zero}
\]

Determinants are finite-dimensional; zero covariance directions contribute the eigenvalue one. The exact Gaussian integral is

\[
 \mathbb E_A
   \exp\!\left(\tfrac12\langle v+\xi_A,J(v+\xi_A)\rangle\right)
  =\exp\!\left(
       \mathfrak F_A[J]
       +\tfrac12\langle v,\mathfrak J_A[J]v\rangle
     \right).
 \tag{CSG.9; P}
\]

For a real symmetric \(J\) with sufficiently small norm, diagonalize \(C_A\) on its range and complete the square. The constant term is the determinant in (CSG.8). The extra retained quadratic form is
\(JC_A^{1/2}(I-C_A^{1/2}JC_A^{1/2})^{-1}C_A^{1/2}J\).
Adding \(J\) and using a convergent Neumann series gives \(\mathfrak J_A[J]\). Absolute Gaussian domination by \(\|J\|I\) proves holomorphy on the same complex ball, so the identity extends to complex symmetric \(J\). This proves (CSG.9) without assuming \(J\) is invertible.

For another independent covariance \(C_B\), direct matrix multiplication and (CSG.8) give

\[
 \begin{aligned}
 I-(C_A+C_B)J
   &=(I-C_B\mathfrak J_A[J])(I-C_AJ),\\
 \mathfrak J_B[\mathfrak J_A[J]]
   &=J(I-(C_A+C_B)J)^{-1},\\
 \mathfrak F_A[J]
     +\mathfrak F_B[\mathfrak J_A[J]]
   &=-\tfrac12\log\det(I-(C_A+C_B)J).
 \end{aligned}
 \tag{CSG.10; P}
\]

The last equality uses the analytic branch at zero. Consequently the order of Gaussian integrations does not change the final answer. The source after the first integration is \(\mathfrak J_A[J]\), not \(J\); replacing it by \(J\) would discard the cross-shell interactions.

Every partial covariance is bounded above by \(C\), hence by \(MI\). Thus for \(M\|J\|\le1/4\),

\[
 \begin{aligned}
 \|\mathfrak J_A[J]\|
   &\le \frac{\|J\|}{1-M\|J\|},\\
 \|C_B^{1/2}\mathfrak J_A[J]C_B^{1/2}\|
   &\le \frac{M\|J\|}{1-M\|J\|}\le\tfrac13,\\
 \|D^m\mathfrak J_A[0](J_1,\ldots,J_m)\|
   &\le m!M^{m-1}\prod_{i=1}^m\|J_i\|,
       \qquad m\ge1 .
 \end{aligned}
 \tag{CSG.11; P}
\]

The last line follows by differentiating the homogeneous term
\(J(C_AJ)^{m-1}\); there are \(m!\) ordered assignments of the directions. The bound applies to every integration depth. It does not use a source radius proportional to the inverse number of scales.

There is also an exact support statement. If \(S\) is the union of the fine source sites and \(P_S\) is their multiplication projection, then

\[
 \mathfrak J_A[J]
     =J+JC_AJ+JC_AJC_AJ+\cdots,\qquad
 P_S\mathfrak J_A[J]P_S=\mathfrak J_A[J].
 \tag{CSG.12; P}
\]

The effective source is generally nonlocal **between** points of \(S\). The two outer factors of \(J\) preserve its support in both arguments. This distinction is what permits the terminal trace estimate in §5.5.

Equation (CSG.11) is an exact bounded-operator admission theorem for the physical quadratic source through the complete flat Gaussian sequence. It does not assert that \(\mathfrak J_A[J]\) has already been decomposed into the particular local Wilson, tensor and irrelevant activities required in the nonlinear R1 norm.

## 4. Local vacuum and physical-volume theorem for the whole Gaussian source

Use cells of side \(\ell_0\), collar width \(\delta=\ell_0/16\), and root weights \(\omega_c(x)\) equal to one in a cell interior and \(2^{-s}\) at a point on \(s\) of its faces. Periodic copies are understood. They satisfy \(\sum_c\omega_c=1\) and \(a^4\sum_x\omega_c(x)=\ell_0^4\). Put \(D_c=c^\delta\cap a\mathbb Z^4\). Since \(T\ge2\ell_0\), this collar has an injective lift to the infinite lattice.

Use the common infinite ultraviolet covariance
\(C_{\rm u}^\infty=\mathcal B(\sum_rX_r^{-1}P_r^\infty)\mathcal B^*\).
For a source given on \(D_c\), define the deterministic local recipe

\[
 \begin{aligned}
 C_{{\rm u},D_c}^\infty
     &=P_{D_c}C_{\rm u}^\infty P_{D_c},\\
 \mathcal L_{a,c}^{\rm fullG}[J]
     &=\frac12\sum_{m\ge1}\frac1m
          \operatorname{Tr}_{D_c}\!
           \left[\omega_c
                 (C_{{\rm u},D_c}^\infty J_{D_c})^m\right].
 \end{aligned}
 \tag{CSG.13; P: prescribed local full-source Gaussian vacuum}
\]

The trace is the Hilbert-space trace with fine measure \(a^4\). This is a single determinant-loop recipe for the summed physical ultraviolet covariance. It is not the sum of determinants for separately sourced shells. The local covariance is compressed to the cell collar; no outside extension of \(J\) is used.

**Theorem 4.1 (P: full flat Gaussian source locality and normalization).**
There are \(\rho_*>0\) and \(C_*<\infty\), depending only on the fixed projection-kernel constants, \(N,L,X_*\), the readout stencil and the cell-margin ratio, such that for every \(K\), every compatible torus, every set of real \(X_r,X_{\rm t}\ge X_*\), and every complex symmetric source with \(\|J\|_\infty\le\rho_*\),

\[
 \begin{aligned}
 \log\mathbb E e^{V_J(\xi)}
      &=\sum_c\mathcal L_{a,c}^{\rm fullG}[J]
                   +\mathcal R_{a,T}^{\rm fullG}[J],\\
 |\mathcal R_{a,T}^{\rm fullG}[J]|
      &\le C_*\,n_{\rm act}(J)\le C_*N_T .
 \end{aligned}
 \tag{CSG.14; P}
\]

Here \(n_{\rm act}(J)\) counts cells containing a source site with positive root weight. Both sides use the branch of the logarithm that is zero at \(J=0\). The source ball has a larger open neighborhood on which the local recipe and remainder are holomorphic. They are real for real symmetric \(J\). The local functional vanishes at zero, is independent of \(T\), and is the same after a translation by one physical cell. It depends on the source only in \(D_c\).

In particular,

\[
 \left|
 e^{-\sum_c\mathcal L_{a,c}^{\rm fullG}[J]}
       \mathbb E e^{V_J(\xi)}
 \right|
       \le e^{C_*n_{\rm act}(J)} .
 \tag{CSG.15; P}
\]

For real \(J\), the logarithm of the positive expression in (CSG.15) has absolute value at most the same bound. This is the Gaussian version of the post-vacuum physical normalization estimate. The ultraviolet covariance and source in it are the full ones in (CSG.5).

If the common physical covariance and the literal source placement intertwine a cell-face reflection, then \(\mathcal L^{\rm fullG}\) is invariant under that reflection with the corresponding tensor transformation. A cell-supported source with margin \(\ell_0/8\) therefore has the same local functional in every reflected chessboard copy. This statement is conditional only on the specified exact reflection intertwiner; the lower-vertex plaquette-anchor issue is not removed by a covariance estimate.

For every finite source family, the remainder has the fixed factorial derivative bound

\[
 \left|D^m\mathcal R_{a,T}^{\rm fullG}[0]
              (J_1,\ldots,J_m)\right|
 \le C_*m!(C_*/\rho_*)^m
       n_{\rm act}(J_1,\ldots,J_m)
          \prod_{i=1}^m\|J_i\|_\infty .
 \tag{CSG.16; P}
\]

The count refers to the union of the direction supports. The same statement holds for C⁵ directions, since their prescribed norm controls the supremum norm. The theorem does not assert that differentiating (CSG.13) produces a strict contact distribution at one spacetime point: it is a cell-collar functional. A strict source-jet replacement for this full cross-shell recipe remains a separate assertion.

## 5. Proof of the full-source locality theorem

### 5.1 Summing scales preserves the operator norm and gives a physical-distance kernel

The operator bound is already (CSG.6); it is not estimated by summing the individual operator norms. For the kernel, the finite readout stencil changes the constants in (CSG.4) only by a fixed factor. Splitting the geometrically spaced \(h_r\) at \(\max(a,|x-y|)\), and reserving half of the exponential for the largest scale, gives

\[
 \|C_{\rm u}^\infty(x,y)\|
   \le A_1X_*^{-1}
        (a+|x-y|_1)^{-4}e^{-c|x-y|_1/\ell_0}.
 \tag{CSG.17; P}
\]

For \(h_r\ge |x-y|\), the sum of \(h_r^{-4}\) is a geometric series. For \(h_r<|x-y|\), write
\(h_r^{-4}e^{-\mu|x-y|/(2h_r)}
=|x-y|^{-4}(|x-y|/h_r)^4e^{-\mu|x-y|/(2h_r)}\)
and sum over the geometric ratios. The remaining half-exponent is at most
\(e^{-\mu|x-y|/(2\ell_0)}\). The diagonal case is bounded by a constant times \(a^{-4}\). This proves (CSG.17).

A second bound will control periodization in trace norm. Let \(A,B\) be finite sets of fine readout sites with positive separation \(d\), and let \(v(A)=a^4|A|\). Put \(F_r=\mathcal BP_r^\infty\), so that
\(\mathcal BP_r^\infty\mathcal B^*=F_rF_r^*\), using \(P_r^2=P_r\).
The kernel of \(F_r\) obeys the same scale bound as \(P_r\).
Split its intermediate fine coordinates into
\(Z=\{z:\operatorname{dist}(z,A)<d/2\}\) and \(Z^c\).
In each of
\(P_AF_rP_ZF_r^*P_B\) and \(P_AF_rP_{Z^c}F_r^*P_B\),
one factor has a separation at least \(d/2\). Squaring its exponential kernel and summing gives a Hilbert–Schmidt bound with that exponential reserve. The other factor is bounded by its unrestricted local Hilbert–Schmidt norm. Schatten Hölder therefore yields

\[
 \|P_AC_{\rm u}^\infty P_B\|_1
 \le A_2X_*^{-1}\sqrt{v(A)v(B)}
        \sum_{r=1}^K h_r^{-4}e^{-c d/h_r}.
 \tag{CSG.18; P}
\]

Here and below \(\|\cdot\|_1\) denotes trace norm and \(\|\cdot\|_2\) denotes Hilbert–Schmidt norm when applied to an operator. Explicitly,
\(\|P_AF_r\|_2^2\le C v(A)h_r^{-4}\), while restricting its second argument to points at distance at least \(d/2\) improves this by \(e^{-cd/h_r}\). The product of the square roots gives (CSG.18), after adjusting \(c\). Thus the trace-class estimate uses the projection factorization, not a finite-rank bound involving \(a^{-4}\).

### 5.2 Local finite-torus covariance versus its common infinite kernel

For a lifted collar \(D=D_c\), exact periodization gives
\(P_DC_{\rm u}^TP_D-P_DC_{\rm u}^\infty P_D\)
as the sum of the image kernels with nonzero winding vector \(n\).
Each image term is unitarily identified with
\(P_DC_{\rm u}^\infty P_{D+nT}\).
The collar width is \(9\ell_0/8\) in each coordinate, whereas \(T\ge2\ell_0\); hence the distance to a nearest nonzero translate is at least \(7\ell_0/8\).
For farther translates it is bounded below by a positive constant times \(|n|_\infty T\).
Applying (CSG.18), summing \(n\ne0\), and then summing the geometric scales gives

\[
 \left\|P_DC_{\rm u}^TP_D
              -P_DC_{\rm u}^\infty P_D\right\|_1
       \le A_3 .
 \tag{CSG.19; P}
\]

Indeed \(v(D)\le C\ell_0^4\), and
\(\sum_r(\ell_0/h_r)^4e^{-c\ell_0/h_r}\) is bounded independently of \(K\).
The additional image sum is bounded by another fixed constant because \(T/\ell_0\ge2\).
All source-independent constants here may depend on \(X_*\). No trace estimate with the fine rank of \(D\) is used.

Both compressed covariances have operator norm at most \(M\). If \(r=\|J\|_\infty\), the elementary telescoping identity for powers gives

\[
 \left|
 \operatorname{Tr}\omega_c
 \left[
   (P_DC_{\rm u}^TP_DJ_D)^m
    -(P_DC_{\rm u}^\infty P_DJ_D)^m
 \right]\right|
 \le m A_3 r(Mr)^{m-1}.
 \tag{CSG.20; P}
\]

The proof is
\(A^m-B^m=\sum_{i=0}^{m-1}A^i(A-B)B^{m-1-i}\),
followed by trace-ideal Hölder. The weight \(\omega_c\) has operator norm at most one. Summing (CSG.20) with coefficient \(1/(2m)\) gives a cutoff-independent cost per active cell.

### 5.3 An exact near/far decomposition with cutoff-independent norms

It remains to compare the complete torus trace rooted in \(c\) with the trace restricted to \(D_c\). This step is where an absolute multiscale row-norm estimate would lose a factor depending on \(K\).

Choose once and for all an even smooth function \(\chi\) on \(\mathbb R^4\), equal to one on the max-norm ball of radius \(1/2\), supported in the ball of radius one, with \(0\le\chi\le1\). For \(R<T/4\), periodize \(\chi((x-y)/R)\) on the torus and multiply each matrix kernel entry of \(C_{\rm u}^T\) by it. Denote the resulting near operator by \(C_R^{\rm n}\), and put \(C_R^{\rm f}=C_{\rm u}^T-C_R^{\rm n}\).

This is a Schur multiplier, not multiplication by a spatial projection. Its norm bound follows from its Fourier representation. On the infinite lattice it is an integral of the conjugates
\(U_p C_{\rm u}^\infty U_p^*\), with total coefficient mass
\((2\pi)^{-4}\int|\widehat\chi(p)|\,dp\).
On the torus use the Fourier series of the periodized cutoff. Its coefficient absolute sum is bounded uniformly for \(R/T<1/4\), by the Schwartz decay of \(\widehat\chi\). Sampling on the fine lattice only aliases these coefficients, and cannot increase their absolute sum. Consequently there is a fixed \(Q_\chi\) such that

\[
 \begin{aligned}
 \|C_R^{\rm n}\|&\le Q_\chi M,\qquad
 \|C_R^{\rm f}\|\le(1+Q_\chi)M,\\
 C_R^{\rm n}(x,y)&=0
     \quad\text{if }\operatorname{dist}_T(x,y)_\infty>R,\\
 C_R^{\rm f}(x,y)&=0
     \quad\text{if }\operatorname{dist}_T(x,y)_\infty\le R/2,\\
 \|P_EC_R^{\rm f}\|_2+
       \|C_R^{\rm f}P_E\|_2
     &\le A_4 X_*^{-1}\sqrt{v(E)}\,R^{-2}
 \end{aligned}
 \tag{CSG.21; P}
\]

for every set \(E\) of fine sites and \(0<R\le\ell_0/16\).
For the last line, periodize (CSG.17), square its norm, and sum over points at torus distance at least \(R/2\). The four-dimensional tail of
\((a+|x-y|)^{-8}\) is bounded by \(C R^{-4}\).
The exponentially decaying image terms have the same bound because \(T\ge2\ell_0\).
The estimate also holds when \(R<a\): its right side is then larger than the corresponding \(a^{-4}\) diagonal-scale estimate. This establishes all constants uniformly in \(a,R,T,K\).

### 5.4 Every escaping trace word has two controlled far factors

Fix a power \(m\ge2\), take \(R=\delta/(4m)\), and let
\(E=c^{\delta/4}\cap\Lambda_{a,T}\).
Expand every covariance factor as \(C_R^{\rm n}+C_R^{\rm f}\).
At every source vertex except the root, insert exactly
\(I=P_D+(I-P_D)\).
The difference between the full rooted trace and the trace compressed to \(D\) is the sum of the words with at least one outside vertex.
There are at most \(2^m2^{m-1}\le4^m\) such near/far and inside/outside words.

This expansion is an exact product of bounded operators. The vertex indicators are orthogonal multiplication projections of norm one. They are not arbitrary entrywise cutoffs of an operator product. Multiplication by the source has norm at most \(r\).

A word containing no far edge vanishes when it has an outside vertex: every vertex is within \(mR\le\delta/4\) of its root. The same is true for a word with only one far edge. Removing that edge leaves a connected chain of at most \(m-1\) near edges containing every vertex and the root, so again every vertex is within \(\delta/4\) of the root. Thus every nonzero escaping word has at least two far edges.

Take the first far edge in forward order from the root and the first far edge in reverse order. They are distinct. All edges between each of these and the root are near, so their root-side endpoints lie in \(E\). Therefore one may insert \(P_E\) next to the corresponding end of each selected far operator without changing that word. More explicitly, combine the root-containing near segment into \(K_0\), the other intervening factors into \(K_1\), and put the two selected far factors with their source/projection multipliers into \(F_i,F_j\). Then \(K_0=P_EK_0P_E\), and cyclicity and Schatten Hölder give

\[
 \left|\operatorname{Tr}(K_0F_iK_1F_j)\right|
  =\left|\operatorname{Tr}
         (K_0P_EF_iK_1F_jP_E)\right|
  \le\|K_0\|\|P_EF_i\|_2\|K_1\|\|F_jP_E\|_2 .
 \tag{CSG.22a; P: the exact two-Hilbert--Schmidt factorization}
\]

The multiplication factors commute with \(P_E\) where needed, so (CSG.21) controls each selected Hilbert–Schmidt factor with its source norm included. Every other factor is estimated only in operator norm. This gives, word by word, a bound of the form
\(C v(E)R^{-4}r^m[(1+Q_\chi)M]^{m-2}X_*^{-2}\).
Since \(v(E)\le C\ell_0^4\), the exact expansion proves

\[
 \left|
 \operatorname{Tr}\omega_c(C_{\rm u}^TJ)^m
   -\operatorname{Tr}_{D}
      \omega_c(P_DC_{\rm u}^TP_DJ_D)^m
 \right|
       \le A_5 m^4(A_6 r)^m .
 \tag{CSG.22; P}
\]

The case \(m=1\) has zero escape difference: the unique source vertex is the root. Choose \(\rho_*\) so that
\(2A_6\rho_*<1/4\) and \(2M\rho_*<1/8\).
Then the series of (CSG.22), multiplied by \(1/(2m)\), converges uniformly on the larger ball \(r\le2\rho_*\).

Every trace considered above contains the source value at the root. If \(J\) vanishes at all points with positive \(\omega_c\), both rooted traces and their difference vanish. Thus only \(n_{\rm act}(J)\) cells contribute. Combining (CSG.20) and (CSG.22) gives

\[
 -\tfrac12\log\det(I-C_{\rm u}^TJ)
      =\sum_c\mathcal L_{a,c}^{\rm fullG}[J]
             +R_{\rm u}[J],\qquad
 |R_{\rm u}[J]|\le A_7 n_{\rm act}(J).
 \tag{CSG.23; P}
\]

This proof retained the cancellations encoded in the bounded full covariance between the two controlled far factors. It did not estimate all covariance edges by their absolute row sums.

### 5.5 The terminal Gaussian costs physical cells

Integrate the ultraviolet Gaussian first and let
\(J_{\rm u}=\mathfrak J_{\rm u}[J]\).
By (CSG.12), \(J_{\rm u}=P_SJ_{\rm u}P_S\) for the original source-site set \(S\).
Its operator norm is at most \(r/(1-Mr)\).
The terminal covariance stays the original positive \(C_{\rm t}\); it is not silently replaced by a source-dressed covariance.

Every object defining \(P_{\rm t}\) is covariant under physical-cell translations. The readout \(\mathcal B\) has the same property. Hence \(\operatorname{Tr}(\omega_cC_{\rm t})\) is independent of \(c\).
Summing over cells, using (CSG.3) and the positivity of \(P_{\rm t}\), gives

\[
 \operatorname{Tr}(\omega_cC_{\rm t})
    =N_T^{-1}\operatorname{Tr}C_{\rm t}
    \le 4(N^2-1)\|\mathcal B\|^2X_*^{-1},\qquad
 \operatorname{Tr}(P_SC_{\rm t})
    \le A_8 n_{\rm act}(J).
 \tag{CSG.24; P}
\]

The second inequality follows pointwise from
\(P_S\le\sum_{c\ {\rm active}}\omega_c\), before taking a positive trace.
This is a local diagonal-trace estimate derived from the actual cell-covariant projection, not a use of total rank alone for an arbitrary source subset.

Set \(H=C_{\rm t}^{1/2}J_{\rm u}C_{\rm t}^{1/2}\). Its operator norm is at most \(Mr/(1-Mr)<1/2\). Factoring on the original support \(S\), trace-ideal Hölder gives

\[
 \begin{aligned}
 \|H\|_1
   &\le\|J_{\rm u}\|\operatorname{Tr}(P_SC_{\rm t})
      \le A_8\frac{r}{1-Mr}\,n_{\rm act}(J),\\
 \left|-\tfrac12\log\det(I-H)\right|
   &\le\frac{\|H\|_1}{2(1-\|H\|)}
      \le A_9 n_{\rm act}(J).
 \end{aligned}
 \tag{CSG.25; P}
\]

No off-diagonal locality of \(J_{\rm u}\) inside \(S\) is required for this estimate. Its bilateral support and bounded operator norm suffice. By the exact Schur identity (CSG.10), the logarithm in the second line is precisely the remaining terminal factor. Adding it to (CSG.23) proves (CSG.14) for the complete Gaussian law.

### 5.6 Analyticity, covariance, replication and derivatives

All finite determinants and compressed local operators are analytic on the fixed larger source ball. The trace series defining (CSG.13) converges normally there for each fixed \(a\). The estimates above are uniform for the remainder on that ball. For real symmetric \(J\), \(I-C^{1/2}JC^{1/2}\) is positive, so the full logarithm is real. Every local series term is real as well.

Cell translations conjugate the common covariance, collar and root weight into those of the translated cell. This proves translation covariance and torus independence of the prescribed local functional. Under an exact face-reflection intertwiner, the same conjugation preserves the trace in (CSG.13), proving reflection covariance. The margin \(\ell_0/8\) exceeds the collar width \(\ell_0/16\), so a reflected neighboring source copy vanishes in the part of a collar lying outside its own cell. This proves the claimed replication property with no unrecorded neighboring source contribution.

Finally apply multivariable Cauchy to
\(J=\sum_i z_iJ_i\) on radii
\(\rho_*/(m\|J_i\|_\infty)\).
The support is contained in the fixed union of the direction supports. The uniform remainder estimate and \(m^m\le e^m m!\) give (CSG.16).
Directions of zero norm vanish by multilinearity.
Exponentiating (CSG.14) proves (CSG.15). This completes the theorem. \(\square\)

## 6. Application to the frozen Balaban flat reference: checked dictionary

This section verifies the projection and quantitative inputs for the **flat reference family**. It does not identify that family with the complete interacting integrand.

### 6.1 Why the exponential gauge and axial covariance give the same physical projection

Write B99 for
\(\texttt{Balaban\_1985\_CMP99\_389-434\_Propagators\ Background}\)
and B109 for \(\texttt{Bałaban, CMP 109 (1987), 249–301}\).
The linear stencil and common-kernel derivation are proved in
Flat Gaussian Periodization, §§2–4.
The actual B109 reference, at identity, has the quadratic form

\[
 \tfrac12\langle B,\Delta_kB\rangle+\tfrac12\|TB\|^2,
 \qquad \widetilde Q_1B=0,\qquad
 \Delta_k=H_k^*d_\eta^*d_\eta H_k ,
 \quad \eta=L^{-k}.
 \tag{CSG.26; P: the already established literal flat reference dictionary}
\]

Here \(T\) is the symmetrized within-block path average, not an axial delta gauge.
The raw constraint is \(L\widetilde Q_1B=0\); its constant Jacobian and the coupling-rescaling Jacobian cancel in a normalized quadratic-source expectation.
The dictionary gives
\(\widetilde Q_1=Q_1-d_c mT\),
\(T(d\lambda)=\lambda-\lambda|_{\rm roots}\), and
\(\widetilde Q_1d\lambda=d_c(\lambda|_{\rm roots})\).

On the covariant zero-constraint space, put \(\lambda=TB\), extended blockwise with zero root values. Then
\(B=B_0+d\lambda\), where
\(\widetilde Q_1B_0=0\), \(TB_0=0\), and the physical curl of the reconstruction is unchanged. On this slice \(\widetilde Q_1=Q_1\).
The reference energy splits exactly into the physical energy of \(B_0\) and \(\|\lambda\|^2\).
The change of linear coordinates has a constant Jacobian.
Integrating \(\lambda\) therefore leaves the standard Gaussian on the physical curvature image with energy \(\|d_\eta H_kB_0\|^2/2\).

One can instead choose an axial within-block gauge while preserving the straight constraint: subtract \(d\lambda_{\rm ax}\), where \(\lambda_{\rm ax}\) is the axial path integral minus its block average. Its block average is zero, so \(Q_1d\lambda_{\rm ax}=0\), and its differences from the block root equal the axial path integrals. This sets the axial gauge to zero without changing physical curvature. A closed coarse field with zero constraint has no remaining physical harmonic component; the fixed-block gap proved in the flat dictionary makes the physical quotient nonsingular.

Thus the physical curvature covariance of (CSG.26) equals the one obtained from B99's **axial** unit covariance. Equality here is only after the physical curl map and normalized gauge integration. It is not equality of the two free-coordinate matrices. The projection identification in §2 now applies directly.

### 6.2 The uniform kernel bound from B99

At \(U=I\), take the gauge potential \(A=0\). Both regularity conditions (3.35)–(3.36), printed p.396, hold with zero left-hand sides. The force-dependent quadratic corrections vanish. Choose the fixed \(M\) large and \(\alpha_0\) small as required by the printed theorems; their values are independent of \(k\).

B99 (3.133), p.422, bounds the minimizer kernel and its first fine covariant derivative. In the whole-torus one-scale specialization, \(L^k\eta=1\) at both unit-scale endpoints. Every scale factor in that displayed derivative bound is therefore one. At identity the covariant derivative is the ordinary derivative. B99 Theorem 3.15, (3.187), p.432, bounds the unit constrained covariance. These consequences are

\[
 \begin{aligned}
 |d_\eta H_k(x,y)|
     &\le A_H e^{-\mu_H\operatorname{dist}(x,y)},\\
 |C_{\rm ax}^{(k)}(y,y')|
     &\le A_C e^{-\mu_C|y-y'|},
 \end{aligned}
 \tag{CSG.27; L: B99 (3.133), p.422, and Theorem 3.15 (3.187), p.432}
\]

The first line uses unit coordinates and the distance from the unit block containing the fine point \(x\); changing to the Euclidean distance changes the constant only. Color and orientation indices are included in the fixed constants.
The covariance being used is identified on B99 p.428, (3.156)–(3.158): its quadratic form is considered on the straight-average-zero, axial-gauge slice, and its normalized covariance is \(C_{\rm ax}^{(k)}\).
The preceding p.427 assumptions are satisfied by the whole-torus specialization on admitted tori: there is no exterior Dirichlet boundary, hence no violated boundary-separation condition.
For the infinite kernel, take larger admitted tori at fixed \(k\). The common-kernel construction of the flat dictionary makes this limit unique, and the uniform bounds pass to it. Exact periodization then constructs every compatible finite flat torus; it does not require a new all-torus extension of the nonlinear theorem.

Let \(h=L^ka\), so \(r=k+1\) has period \(h_r=Lh\). The physical shell curvature is \(h^{-2}d_\eta H_kB\). Its unit-coupling covariance is consequently

\[
 P_r(x,x')
 =h^{-4}\sum_{y,y'}
       d_\eta H_k(x/h,y)\,
       C_{\rm ax}^{(k)}(y,y')\,
       d_\eta H_k(x'/h,y')^{\mathsf T}.
 \tag{CSG.28; P: the actual physical flat shell covariance}
\]

The coarse sums have unit counting measure. Fine adjoints use \(\eta^4\) before rescaling, or \(a^4\) in physical coordinates.
Convolution of the three exponentials in (CSG.27) gives
\(A h^{-4}e^{-\mu|x-x'|/h}\), after decreasing \(\mu\).
Replacing \(h\) by \(h_r/L\) gives (CSG.4) with new fixed constants.
This supplies the uniform-in-\(k\) decay estimate missing from a fixed-\(k\) Bloch analyticity argument alone.

The infinite projection and periodization identities follow from the already constructed common gapped matrices and physical readout maps. Finite-dimensional energy minimization proves \(P_r^2=P_r\) and \(P_rP_s=0\) on every admitted torus. Equivalently, in the common \(\ell_0\)-periodic Bloch representation these are continuous matrix identities on every finite momentum grid. Such grids are dense as the admitted tori grow, so the identities hold on the full Bloch torus and therefore for the common infinite kernels. Their absolutely summable kernels permit periodization of their products. This proves the asserted infinite orthogonality and compatibility rather than assuming it from decay.

### 6.3 What the checked application includes

The exact Schur theorem applies to the product of these normalized, source-zero flat references, with the physical linear reconstruction summed across scales and with arbitrary specified positive coefficients \(X_r\ge X_*\). It includes:

- the actual symmetrized covariant-constraint stencil through its physical quotient;
- the exponential gauge of B109, with axial covariance used only after proving physical equivalence;
- the full physical plaquette and flat clover readouts, with (CSG.7)'s factors;
- every scalar/tensor cross term between distinct Gaussian shells;
- the actual full-source ultraviolet determinant and its source-supported Schur quadratic form;
- a terminal **quadratic-model** physical Gaussian, if this completion is chosen.

The last item is not a claim that Balaban's actual terminal Haar or interacting density is Gaussian. For a deterministic retained curvature, (CSG.9) is instead the exact applicable formula. Its field-valued quadratic output still requires the nonlinear program's local projections and bounds.

### 6.4 Primary inputs

| Source and location | Imported assertion and checked hypotheses | Exact use |
|---|---|---|
| B99 (3.35)–(3.36), p.396 | Identity background has \(A=0\), hence both regularity conditions with zero left sides | Admits the fixed flat derivative and covariance estimates |
| B99 (3.133), p.422 | The minimizer and first-derivative kernel estimate; \(L^k\eta=1\) in the unit-scale whole-torus specialization | First line of (CSG.27), including all scale factors |
| B99, §E opening, p.427; (3.156)–(3.158), p.428 | Unit covariance on the constrained axial-gauge slice; whole-torus geometry has no exterior separation defect | Identifies the Gaussian used to compute the physical projection |
| B99 Theorem 3.15, (3.187), p.432 | Uniform exponential bound with constants depending only on fixed construction data; \(M\alpha_0\) small | Second line of (CSG.27) and the convolution (CSG.28) |
| [Periodization of the whole-torus flat Gaussian](flat_gaussian_periodization.md), §§2–4, with its B95/B109 source list | Common massive-operator chain, exact covariant stencil, exponential gauge, physical-minimum equivalence, and exact periodization | Transfers the physical covariance and its common kernel; no new sourced operator is imported |

## 7. What is closed, and what remains for R1/R2

### 7.1 Closed by this note

**P — Full physical Gaussian source transport.** Equations (CSG.8)–(CSG.12) are exact at every integration depth. They retain the physical cross-shell terms and preserve a fixed operator source ball. Energy orthogonality supplies the required cutoff-independent bound on every partial covariance.

**P — Uniform flat shell kernel admission.** The uniform-decay requirement is verified for the flat physical reference projections by the checked B99 estimates and the exact gauge/periodization dictionary. The proof distinguishes physical covariance from a coordinate covariance; the exponential-gauge matrix is never silently replaced by the axial matrix.

**P — Whole-source Gaussian cell vacuum and normalization.** The deterministic local recipe (CSG.13), together with (CSG.14)–(CSG.16), treats the summed physical ultraviolet covariance and the remaining coarse Gaussian. It yields a uniform active-physical-cell remainder and factorial source jets. The counterterm is defined on one lifted cell collar using the common infinite kernel, not by setting it equal to a full finite-torus logarithm.

**P — Exact retained quadratic readout.** For a fixed retained curvature, the output source is the symmetric operator \(\mathfrak J_A[J]\) in (CSG.9). It is uniformly bounded and supported, in both arguments, on the original source support. Its nonlocal entries are retained explicitly.

### 7.2 Remaining statements, with exact scope

**O — Nonlinear mixed-source admission.** Replace the independent flat quadratic references by the actual constrained nonlinear kernels, their cutoffs, regular E interactions, recent and erased R operations, and boundary terms. Prove the appropriate analogue of the invariant source/operator bounds while preserving the old physical readouts and every compulsory mass. Gaussian energy orthogonality is not available for those nonlinear source-dependent activities by declaration.

**O — Required local field-valued projections.** Decompose the actual retained readout and its nonlinear analogues into deterministic identity terms, the full dimension-four scalar/tensor space and an irrelevant remainder in the program's complete norm. The global operator bound (CSG.11) is not already that spatially localized projection theorem.

**O — Same-vacuum complete interacting normalization.** The nonlinear source vacuum must follow one deterministic recipe through both regular and erased-R connected integrations. Prove its local comparison and the complete pressure or fractional-patch estimate in the R2 contract. The terminal Gaussian estimate (CSG.25) does not apply to an arbitrary retained-history law or to Balaban's actual interacting terminal density.

**O — Strict contact refinement for the complete physical Gaussian source.** The older strict source-jet argument in Gaussian Source Locality applies to the displayed sum of separate shell logarithms. It does not automatically replace the full cross-shell recipe (CSG.13) by a function of source jets through order four at one point. Such a refinement, or an equivalent compatible contact forest, must be proved before using that stronger downstream conclusion.

**C — Literal reflection application.** The trace recipe is reflection covariant under an exact source/covariance intertwiner preserving the cell collar. The actual lower-vertex Wilson source and clover anchors must satisfy the intended tensor reflection rule, or their placement error must be estimated. An operator norm or exponential kernel bound does not prove that identity.

**O — Running physical normalization and full pointwise stability.** The formula \(X_0=N\beta_a\) is checked at bare level. The assignment of all \(X_r\) to the coefficients of the actual N2-F/Balaban construction still needs R0. This note proves integrated Gaussian pressure and source transport; it does not prove the original N1-S pointwise upper/lower bounds for \(\rho_K[j]\).

No interface change is introduced. In particular, no new sourced stability theorem is assumed as a hypothesis, and the exact N2-F assumption is not strengthened. The mathematical inputs beyond finite Gaussian algebra are the specifically checked **source-free flat** primary estimates in §6.

