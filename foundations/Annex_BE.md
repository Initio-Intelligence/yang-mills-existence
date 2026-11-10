# Constrained stationarity: an auxiliary conditional theorem

**Annex BE.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Weighted inverse for an averaged constrained Hessian

Let a finite block graph have distance rho and bounded exponential volume sums. Write the variables as t=(z,y), with free interior blocks I and collar/exterior blocks O. Each coordinate block has a fixed Euclidean norm, or more generally a Hilbert norm with uniform row/column estimates. Let S be a real C² function on a neighborhood of the segment joining 0 to t*. The coordinates are assumed to parameterize the **exact constraint**, not just its tangent space.

Suppose, throughout that segment, the interior Hessian satisfies

\[
 S''_{II}(s t^*)\ge\lambda I,
 \qquad
 \sup_{i\in I}\sum_{j\in I}
    \|S''_{ij}(s t^*)\|\big(e^{a\rho(i,j)}-1\big)
 \le\lambda/2,
 \tag{LS19.1}
\]

with the symmetric column estimate. Assume also

\[
 \sup_{0\le s\le1}\|S''_{ij}(s t^*)\|
 \le K e^{-b\rho(i,j)},\qquad i\in I,\ j\in O,
 \tag{LS19.2}
\]

for fixed a,b,lambda,K>0. Put

\[
 \overline K=\int_0^1S''(s t^*)\,ds.
 \tag{LS19.3}
\]

Both hypotheses pass to this average. For a real one-Lipschitz spatial function f, multiply coordinate block i by M_i=exp(a f_i). The norm of M Kbar_II M^-1-Kbar_II is at most lambda/2, by the row/column Schur estimate in (LS19.1). Hence

\[
 \|M\overline K_{II}^{-1}M^{-1}\|\le2/\lambda,
 \qquad
 \|(\overline K_{II}^{-1})_{ij}\|
 \le(2/\lambda)e^{-a\rho(i,j)}.
 \tag{LS19.4}
\]

The first statement follows by a bounded perturbation of the positive matrix Kbar_II, or directly from the real-part coercivity inequality. Choose f_l=rho(l,j) for the second. No diagonal dominance of Kbar_II is assumed.

### 2. Stationary interior and boundary response

#### Theorem LS19.1

Suppose t*=(z*,y*) is stationary in the free interior variables, so D_I S(t*)=0. Let d=D_I S(0). Under (LS19.1)–(LS19.2),

\[
 z^*=-\overline K_{II}^{-1}
             \big(d+\overline K_{IO}y^*\big).
 \tag{LS19.5}
\]

Consequently, for any c<min(a,b)/2,

\[
 |z_i^*|
 \le C\sum_{j\in I}e^{-a\rho(i,j)}|d_j|
       +C\sum_{j\in O}e^{-c\rho(i,j)}|y_j^*|.
 \tag{LS19.6}
\]

If d is supported in a collar B and bounded by D there, and |y_j*|<=Y, then

\[
 |z_i^*|\le C(D+Y)e^{-c'\operatorname{dist}(i,O\cup B)}
 \tag{LS19.7}
\]

for any fixed c'<c. Constants are independent of the total volume, provided the stated graph exponential sums and Hessian estimates are uniform.

**Proof.** The fundamental theorem of calculus gives

\[
 0=D_I S(t^*)
  =d+\overline K_{II}z^*+\overline K_{IO}y^*.
\]

Invert with (LS19.4) to obtain (LS19.5). The matrix product between the inverse and Kbar_IO is bounded by a convolution of two exponential kernels. The triangle inequality and one fixed rate loss give (LS19.6). A further rate loss leaves a summable kernel and proves (LS19.7). The exact constraint has already been built into S, so its first and second derivatives include the corresponding constraint-current terms. Omitting those terms would change the hypotheses and the equation. ∎

The theorem concerns a path in an exact free-coordinate chart on a local patch. It does not require a path connecting arbitrary global determining data to a globally flat configuration. This avoids that particular topological assumption, but it does not verify the local chart or its Hessian by itself.

#### Fine-mesh qualification and weighted-form alternative

The absolute matrix hypothesis (LS19.1) is suitable for fixed-spacing coordinate blocks. It must **not** be claimed automatically uniform on a refining fine lattice. A physical fine Laplacian has neighbor entries of order eta^-2. With distance in physical units, the absolute conjugation sum in (LS19.1) then has a bound of order a/eta. Physical elliptic weighted estimates instead use form cancellations, or the source's uniform Green-function norms.

There is an exact abstract alternative. If the averaged constrained operator has the weighted coercivity property

\[
 \operatorname{Re}\langle Mw,M\overline K_{II}w\rangle
 \ge c\|Mw\|^2
 \tag{LS19.11}
\]

for every admissible spatial weight M, on its actual common form domain, then its weighted inverse has norm at most c^-1. Equations (LS19.5)–(LS19.9) follow with that inverse and the corresponding mixed collar kernel bounds. The proof tests the inverse equation with the weighted vector and applies Cauchy–Schwarz. A weighted **form** estimate of this kind must include constraint/projection commutators and domain preservation; positivity of an unweighted fine Hessian alone does not prove it. Grouping fine variables into coarse blocks likewise does not automatically bound the interface block operators.

In the actual variational source, the global right inverse H and nonlinear correction A'=A-H D(A) are distinct from C-08's local one-step exceptional-bond chart. A multidepth fine-grid application must use the true H, its tails and the source physical norms, or prove a different uniformly controlled exact chart. The one-step h cannot be substituted silently.

### 3. A local observable and its curvature interpretation

Let Phi_i(t) be a local observable in the same chart with Phi_i(0)=0 and an anchored derivative bound

\[
 \|D_j\Phi_i(s t^*)\|\le C_\Phi e^{-b_\Phi\rho(i,j)}.
 \tag{LS19.8}
\]

Integrating along the segment and inserting (LS19.6) gives an exponentially localized bound for |Phi_i(t*)| in terms of d and the retained y*. If both are confined to a collar at distance r, then

\[
 |\Phi_i(t^*)|\le C C_\Phi(D+Y)e^{-c_\Phi r}.
 \tag{LS19.9}
\]

A plaquette curvature of an exactly flat reference is an example only after its actual constrained chart derivative has been checked. If a current-normalized curvature has an additional factor g^-1, that factor must remain on the right. For a collar R=(log g^-2)^r0 with r0>1, a boundary budget bounded by g^-A times a fixed polynomial in log g^-2 is then suppressed by exp(-cR). This last numerical statement follows from

\[
 A\log g^{-1}+q\log\log g^{-2}
       -c(\log g^{-2})^{r_0}\longrightarrow-\infty.
 \tag{LS19.10}
\]

### 4. Exact application checks still needed for M-04

For the background field in CMP119, the notation U_(k+1) denotes a minimizing fine configuration determined by retained coarse averages. Its fine plaquette energies cannot be inserted into the M-03 output regulator merely by renaming them retained coordinates. The following source-specific checks are necessary to use the theorem above:

1. A local patch whose interior determining averages are flat admits an exact free-coordinate chart for the actual fine minimizer, with the boundary and any crossing constraints confined to a stated collar.
2. The actual minimizer and the radial path in that chart lie in the admitted source domain, uniformly in the fine mesh, including the required curvature/current norms and the nonlinear constraint correction.
3. The fine constrained Hessian and its mixed collar block satisfy the required uniform weighted inverse and collar estimates on that path in the correct physical normalization, through (LS19.1)–(LS19.2) when those absolute bounds hold or the weighted-form alternative (LS19.11) with its domain and commutator checks. A current-lattice C-08 estimate alone is not a fine-grid minimizing-field theorem.
4. The local reference produces d=0 in the interior, and its boundary d and y budgets have the explicit polynomial/coupling costs used in (LS19.10).
5. The curvature derivative estimate (LS19.8) holds for the actual averaging and reconstruction map. Its endpoints, scales and all retained field slots must be identified.

If those are verified, the flat-inner-patch field decays into the interior by (LS19.9). Combining it with a local gauge-covariant response to nonflat determining data can give the desired weighted output-energy bound. None of the five checks is silently imported from the finite-dimensional algebra.
