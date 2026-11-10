# A buffered resolvent expansion with genuine physical carriers

Working theorem for catalogue theorem M-04. The result below is a matrix theorem with explicit local-coefficient hypotheses. It does not replace the task of identifying the complete Wilson precision in those hypotheses.

## 1. Hypotheses and the carrier algebra

Let I be a finite subset or periodic quotient of a fixed-dimensional lattice of bounded degree, with a fixed finite number of free real components per site. Let A(v) be a real symmetric or complex Hermitian matrix on these coordinates. On the admitted real retained data G suppose

\[
 A(v)\ge mI,\qquad
 A_{ij}(v)=0\quad\hbox{if }d(i,j)>r,\qquad
 \sup_i\sum_j\sup_{v\in G}\|A_{ij}(v)\|\le K.       \tag{PR.1}
\]

The numbers m>0, K and the finite range r do not depend on total volume. The supremum is deliberately inside the row sum. If only a uniform row-sum bound with the supremum outside is supplied, finite range gives this version with an additional factor equal to the fixed stencil cardinality D_r. Each entry is an actual function of retained variables in a specified bounded footprint within distance r_0 of its endpoints. The sites, endpoints and retained footprints are all included in every carrier. No independently variable native minimizing background is identified with raw retained links in this hypothesis.

For an explicit connected-carrier representation T=Σ_X T_X, with T_X(i,j)=0 unless i,j∈X, use the two-sided row/column norm

\[
 \|T\|_\nu
 =\max\left\{
 \sup_i\sum_{X\ni i}e^{\nu|X|}\sum_j\sup_{v\in G}\|T_X(i,j;v)\|,
 \sup_j\sum_{X\ni j}e^{\nu|X|}\sum_i\sup_{v\in G}\|T_X(i,j;v)\|
 \right\}.                                           \tag{PR.2}
\]

If preferred, use e^{ν(|X|+t(X))}; for connected carriers this only changes the numerical exponent. A matrix product joins two carriers at its summed matrix index, so their union is connected and its weight is at most the product of the two weights. Therefore (PR.2), with the induced product representation, is submultiplicative. This is an absolute coefficient norm, not the norm of the summed matrix after cancellations.

## 2. Local inverses have a uniform entrywise decay bound

For a cube Q let A_Q=P_QAP_Q be its principal compression. Then A_Q≥mI for every admitted v. For t≥0 put R_Q(t)=(A_Q+tI_Q)^{-1}. Choose γ>0 with

\[
 K(e^{\gamma r}-1)\le m/2.
\]

Conjugation by the scalar diagonal weight e^{-γd(i,·)} changes A_Q in operator norm by at most m/2, using its absolute row and column sums. Its resolvent has norm at most 2/(m+t), by the resolvent identity and a Neumann series around the positive A_Q+t. Taking a single entry gives

\[
 \|R_Q(t;i,j)\|\le\frac{2}{m+t}e^{-\gamma d(i,j)}.   \tag{PR.3}
\]

Since lattice spheres have fixed polynomial growth,

\[
 \sup_i\sum_j\|R_Q(t;i,j)\|
 \le\frac{C_\gamma}{m+t}.                             \tag{PR.4}
\]

The constants are independent of Q and total volume. In particular this argument works for every t≥0 with the same γ. It does not infer an absolute path expansion from spectral convergence: (PR.3) concerns each already defined finite local inverse.

## 3. A genuinely local parametrix and an absolutely small error

Choose a fixed family of cubes Q of side O(M), with real multipliers χ_Q satisfying Σ_Qχ_Q^2=1. Their overlap is bounded, each χ_Q is supported at distance more than r from ∂Q, and

\[
 |\chi_Q(i)-\chi_Q(j)|\le C d(i,j)/M.
\]

Define

\[
 P(t)=\sum_Q\chi_Q R_Q(t)\chi_Q,
 \qquad E(t)=\sum_Q[A,\chi_Q]R_Q(t)\chi_Q.             \tag{PR.5}
\]

The support buffer makes the exact identity

\[
 (A+t)P(t)=I+E(t)                                    \tag{PR.6}
\]

valid on the full space. Indeed Aχ_QR_Qχ_Q=χ_QA_QR_Qχ_Q+[A,χ_Q]R_Qχ_Q, and the t term completes A_Q+t. No boundary coupling is omitted.

Using (PR.4), the finite range, the Lipschitz bound and fixed overlap,

\[
 \sup_i\sum_Q\sum_j\|E_Q(t;i,j)\|
 \le\frac{C K r C_\gamma}{M(m+t)}.                    \tag{PR.7}
\]

Choose M, once and for all, so the right side is at most 1/4 at t=0. Each coefficient P_Q or E_Q depends only on the entries of A_Q, and hence only on raw retained data in Q enlarged by its fixed entry footprints. Declare this enlarged cube to be its physical carrier. Its volume is at most V_M=C(M+r+r_0)^d. Choose a strictly positive ν small enough that e^{ν V_M}/4≤1/2. Then

\[
 \|E(t)\|_\nu\le\tfrac12,
 \qquad \|P(t)\|_\nu\le\frac{C}{m+t}.               \tag{PR.8}
\]

The column bound follows in the same way: a nonzero local term in column j has j in its cube, so fixed overlap applies, and (PR.3) also supplies the local inverse column sum. All sums in this estimate retain the individual local coefficients. The smallness is present **before** summing their signed or matrix-valued contributions.

## 4. The physical-carrier resolvent theorem

### Theorem PR.1

Under (PR.1) and the stated actual dependency footprints, there is ν>0 and an exact expansion

\[
 (A+tI)^{-1}=P(t)\sum_{n\ge0}[-E(t)]^n,\qquad t\ge0, \tag{PR.9}
\]

converging absolutely in the connected physical-carrier norm, with

\[
 \|(A+tI)^{-1}\|_\nu\le\frac{C}{m+t}.                \tag{PR.10}
\]

Every term is a function of the raw retained variables in its declared union of overlapping local cubes. Constants depend on the fixed local data m,K,r,r0 and lattice dimension, not on volume.

**Proof.** Equations (PR.6) and (PR.8) show that P(I+E)^{-1} is a right inverse of A+t. The finite matrix A+t is invertible, so this is its inverse. Submultiplicativity and ||E||ν≤1/2 prove absolute convergence and (PR.10). Matrix multiplication supplies the claimed connected unions and introduces no variables outside them. ∎

The representation pays e^{ν volume} because each step of the convergent series adds only a fixed-size local cube with a genuinely small absolute coefficient. A distance-decay estimate for a global kernel alone would not give this conclusion.

## 5. Fractional powers and retained derivatives

The scalar identity λ^{-1/2}=π^{-1}∫_0^∞ t^{-1/2}(λ+t)^{-1}dt follows by t=u². Spectral calculus and (PR.10) therefore give the absolutely convergent carrier representation

\[
 A^{-1/2}=\frac1\pi\int_0^\infty
              t^{-1/2}P(t)\sum_{n\ge0}[-E(t)]^n\,dt,
 \qquad \|A^{-1/2}\|_\nu\le C m^{-1/2}.              \tag{PR.11}
\]

Multiplying by the finite-range A gives A^{1/2} with actual carriers as well. In particular, apply the theorem to A=K−σI for a fixed 0<σ<inf spec K. It constructs the localized Gram factor B=(K−σI)^{1/2} needed in the positive extension, without assuming that an unweighted spectral binomial series is an absolutely summable path series.

On any local buffered retained domain on which the coefficient derivatives exist,

\[
 D R_Q(t)=-R_Q(t)(D A_Q)R_Q(t).                       \tag{PR.12}
\]

Differentiating (PR.5) and (PR.9) retains explicit local supports. The differentiated geometric series has sum bounded by Σ_{n≥1}n||E||^{n−1}≤4. Thus fixed local first-derivative coefficient bounds produce a convergent differentiated carrier series, after reducing ν to pay any fixed polynomial carrier count. This statement requires the actual derivative budget for A; it does not silently prove the complete Wilson retained score. A discrete geometry or rank change is not covered by (PR.12).

## 6. A small supported perturbation

If A=A_0+H, with A_0 satisfying the preceding finite-range hypotheses, H possessing a specified absolute physical-carrier expansion, and

\[
 \sup_{t\ge0}\|H\|_\nu\|(A_0+t)^{-1}\|_\nu<1,
\]

then

\[
 (A+t)^{-1}
 =\sum_{n\ge0}[-(A_0+t)^{-1}H]^n(A_0+t)^{-1}          \tag{PR.13}
\]

converges with the same physical-support property. This is the correct use of a small nonlinear background correction: smallness is measured in the absolute supported-coefficient algebra. Spectral smallness of H alone is insufficient.

## 7. Uniformly positive precisions with exponentially supported coefficients

### Theorem PR.2 (inverse closure at a smaller positive carrier rate)

Suppose A=Σ_XA_X is Hermitian, each X is a connected actual physical carrier, the coefficient expansion obeys ||A||_ν≤K for some ν>0, and A(v)≥mI on the real retained domain. Then for some ν'>0 depending only on m,K,ν and the fixed lattice geometry, A has the conclusion of PR.1 at rate ν'. In particular

\[
 \|(A+t)^{-1}\|_{\nu'}\le C/(m+t),\qquad
 \|A^{-1/2}\|_{\nu'}\le C m^{-1/2}.                   \tag{PR.14}
\]

The same applies on the full ambient real domain when the two hypotheses hold there. No spectral contraction is used as a substitute for an absolute carrier contraction.

**Proof.** First pair an activity with its adjoint, if necessary, so each retained tag is Hermitian without changing its carrier or increasing the absolute norm. Let A_n be the sum of tags with |X|≤n and H_n=A−A_n. Then A_n has finite matrix range at most n and its entries have retained footprints within distance n of their endpoints. Moreover

\[
 \|H_n\|_{\nu/2}\le K e^{-\nu n/2},
 \qquad A_n\ge(m-Ke^{-\nu n})I.                       \tag{PR.15}
\]

Choose n initially large enough that the latter gap is at least 3m/4. The constants in the local inverse proof can be made independent of n. Indeed, for γ≤ν/4, the connected-carrier hypothesis implies

\[
 \sup_i\sum_j\sup_v\|(A_n)_{ij}(v)\|
          d(i,j)e^{\gamma d(i,j)}\le C_\nu K,
\]

because d(i,j)≤|X|−1 in each contributing carrier and the factor |X|e^{−ν|X|/2} is bounded. The conjugation error in Section 2 is therefore at most C_νKγ, rather than a constant growing with the range n. Choose γ>0 depending only on m,K,ν so this is at most m/4. The local resolvents have (PR.3)–(PR.4) with constants independent of n.

Use partition cubes with M≥4n, and also large enough to make the commutator estimate at most 1/8. Its bound is C C_νK/[M(m+t)] by the same weighted first-moment estimate. Each local inverse coefficient has its raw footprint in Q enlarged by n, hence has volume at most V_M=C M^d. Take ν'≤min(ν/2,(log 2)/V_M). The weighted parametrix error is at most 1/4 and its resolvent obeys

\[
 \|(A_n+t)^{-1}\|_{\nu'}\le C_R/(m+t),
\]

where C_R depends on m,K,ν but not on n or M. To see the independence, its unweighted local-inverse row constant was already independent of n, fixed overlap is uniform for M≥4n, and the added carrier weight is at most two.

We can therefore increase n, before fixing M and ν', until (C_R/m)K e^{−νn/2}≤1/4. Equation (PR.15) gives ||H_n||_{ν'}≤K e^{−νn/2}. The exact resolvent series (PR.13), now with reference A_n and perturbation H_n, converges absolutely at rate ν' and proves the first assertion of (PR.14). The Stieltjes integral proves the second. Every multiplication uses an actual common matrix index, so all the retained footprints remain in the stated connected union. ∎

This theorem applies, in particular, to a Gram extension K_ext=σI+B_ext*B_ext once its supported coefficient norm is finite. The Gram form supplies the global gap and coefficient multiplication supplies its global carrier norm. It therefore resolves the **real Gaussian resolvent** part of that extension without assuming that the smoothly clipped coefficients still arise from the original source propagators. It does not alone prove the complex interacting polymer expansion or its marked coefficients.

## 8. Application boundary

For the first Wilson step, the local lift Q^fV is a plausible source of the finite-range reference A0. The complete constrained free-coordinate precision must still be identified with A0 plus a small genuinely supported H, including its constraint and soft-gauge terms. Merely observing that the underlying plaquette action is finite range is insufficient after a nonlocal coordinate elimination. The local-compression domains in this note also need the actual source chart and positive margin; null-fiber extensions require their own local buffers.

Once that identification is verified, the theorem supplies the missing **all-t absolute resolvent** step in the local Gram construction. It supplies neither the interacting marked numerator nor residual-history normalization and interface bounds. Those remain distinct from this matrix result.
