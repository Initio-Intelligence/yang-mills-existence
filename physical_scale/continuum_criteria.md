# Sufficient conditions for a continuum hierarchy

**Gaussian calibration hypothesis (GC).** For the signed Gaussian increments of the actual stationary source section in its thermodynamic normalization, assume $\sum_{k<n}d_k^G=d_Bn+\vartheta_n$ with $d_B>0$ and $\sup_n|\vartheta_n|\le B_G$. The coupling and stopping conclusions use this calibration and the specified source readout and replay. A physical continuum limit also requires the stated uniform normalization and full-law hierarchy estimates.

## 1. Conditional consequences of finite-scale bounds

This note states a sufficient remaining estimate for a common continuum
hierarchy. It also proves the reduction to that estimate. The remaining
estimate itself is not proved here, and the note does not claim
Yang--Mills existence.

The reduction keeps the original Wilson measures, their microscopic
insertions and one common cofinal sequence. It uses three actual results
proved elsewhere in this collection:

1. B03 and the stopped-sequence construction give the actual weak
   trajectories and a positive weak subsequential endpoint.
2. The active-history survival reserve makes a specified very old
   unreplaced sector negligible even with the original microscopic
   insertions attached. Completed archives remain part of the exact
   transported source.
3. Exact microscopic source transport and coincidence-flat Taylor
   estimates remove a shrinking source-position collar, while keeping
   the full positive history law and all outer conditional means.

The two negligible pieces need only tend to zero at each fixed insertion
order. Their intermediate constants need not already satisfy the
uniform-in-order bound sought for the limiting hierarchy. This is useful
because the original frozen full-carrier norm asks for stronger
intermediate estimates than these two limit operations require.

## 2. The actual decomposition

Use the stopped sequence with ultraviolet depth \(K_n\), mesh
\(a_n=\ell_0L^{-K_n}\), and growing compatible cubic tori. Choose their
terminal volumes to satisfy \(V_n=o(K_n)\), as permitted in the endpoint
construction. All expectations below refer to its original full
positive Wilson/history law.

Let \(\Phi_{\alpha,n}\) be a stated finite F01 prescription and retain
its actual coefficient and identity budget
\[
 b_n=\|Z_n\|/\beta_{W,n}+a_n^4|c_n|.
 \tag{ER.1}
\]
The fixed energy-normalized centered representatives have a fixed
budget. For the physically prescribed fields, a sufficient additional
assumption for this reduction is
\[
 b_n\le C a_n^{-\gamma}
 \quad\hbox{for one fixed finite }\gamma\ge0 .
 \tag{ER.2}
\]
No F05 bound or invertibility is asserted by writing (ER.2).
The usual fixed logarithmic budget would be stronger than needed here.

For \(m\ge2\), let \(\chi_n(X)\) indicate that a pair of microscopic
physical source positions has separation at most \(a_n^\theta\),
where \(0<\theta<1\) is fixed. Put \(\chi_n=0\) for \(m=1\).
Let \(E_n\) be the very old active-history event from H2S, with its
single common age threshold. Its fixed-weight diagonal construction
already suffices; the stronger scale-dependent reserve gives an explicit
choice. Every completed archive and every recent bad sector remain in
\(E_n^c\).

For a smooth coincidence-flat joint test \(F\), define
\[
 \begin{split}
 S_{m,n}(F)
 &=a_n^{4m}\sum_{\boldsymbol\alpha,X}
     F_{\boldsymbol\alpha}(X)
       \mathbb E_n\prod_{i=1}^m\Phi_{\alpha_i,n}(x_i),\\
 R_{m,n}(F)
 &=a_n^{4m}\sum_{\boldsymbol\alpha,X}
     (1-\chi_n(X))F_{\boldsymbol\alpha}(X)
       \mathbb E_n\!\left[
          \mathbf1_{E_n^c}\prod_{i=1}^m
                                  \Phi_{\alpha_i,n}(x_i)\right].
 \end{split}
 \tag{ER.3}
\]
Initially take \(F\) compactly supported in the central half of the
physical torus in every source position. This avoids introducing
periodic-image coincidence surfaces. Each fixed compact test meets that
condition eventually.

The expectation in \(R_{m,n}\) is deliberately **unnormalized on
\(E_n^c\)**. There is no new conditional denominator and no assertion
that this restricted law is reflection positive.

### Proposition ER.1 — the two removed pieces vanish

Assume (ER.2), or use the centered fixed representatives. For every
fixed \(m\), there is a fixed linear-order seminorm index
\(r_m\le r_*m+r_*\) and a number \(\epsilon_{m,n}\to0\) such that
\[
 |S_{m,n}(F)-R_{m,n}(F)|
       \le\epsilon_{m,n}\nu_{r_m}(F).
 \tag{ER.4}
\]
The same conclusion holds in every fixed outer \(L^q\) norm after
transport through an actual source-free conditional cut, with its
corresponding exact marked jet.

**Proof.** Split the difference exactly into the full moment in the
collar and the ancient-history contribution outside that collar.

For the first piece, CS.17 gives
\[
 C^m(mq)^m(b_n a_n^\delta)^m\nu_{s_m}(F),
 \qquad s_m=O(m).
 \tag{ER.5}
\]
Choose one fixed \(\delta>\gamma\). This tends to zero for every
fixed \(m,q\).

For the second piece, H2S.26 and the weighted physical source-position
sum used in CS.22 give
\[
 (Cmq)^m b_n^m a_n^{-4m}
                  \mathbb P_n(E_n)^{1/(2q)}
                    \nu_{6m+2}(F).
 \tag{ER.6}
\]
The H2S age threshold can be chosen once so that its survival exponent
dominates every fixed multiple of \(K_n\). Thus it pays
\(b_n^m a_n^{-4m}\le C^m
\exp[(4+\gamma)mK_n\log L]\) for every fixed \(m,q\).
Alternatively use the fixed-weight diagonal with the bound
\((4+\gamma)m\) in its choice of weights. No microscopic insertion is
replaced by a new current stencil in this argument.

Conditional expectation is an \(L^q\) contraction in the actual joint
law, so the same estimates hold at an exact cut. Combining the two
bounds proves (ER.4). \(\square\)

## 3. The precise estimate still needed

The remaining hierarchy estimate in this route is
\[
 \boxed{\quad
 |R_{m,n}(F)|
       \le C^{m+1}(m!)^p\nu_{qm}(F),
 \quad m\ge1 ,
 \quad}
 \tag{ER.7}
\]
for fixed \(C,p,q\), uniformly along one cofinal sequence, for the
actual physically prescribed fields and all compact coincidence-flat
tests in the preceding central-torus convention.

This is still a substantial actual-model estimate. It contains:

* the exact microscopic source transported through the earlier kernels;
* recent and intermediate-age regular, successful, residual and
  unreplaced sectors;
* the outer conditional means and every generated higher source vertex;
* the actual linear normalization and identity subtraction.

The new AC carrier algebra is one possible tool for proving (ER.7).
Its successful-sector joint energy estimate does not yet supply the
transported marked catalog or the remaining residual-sector comparison.
The probability compactness of local active records is also insufficient:
the unbounded physical insertion is not a bounded continuous function
of that local geometry.

Equation (ER.7) is weaker than demanding every frozen M03
pointwise/current/full-volume-carrier estimate at every intermediate
history. It is not obtained from those estimates by assertion, and it
does not retrospectively complete the original M04, M07 or H02 statements.
It is an explicitly different sufficient route to the hierarchy part
of the existence target.

## 4. The common-hierarchy consequence is rigorous

### Theorem ER.2 — conditional continuum compactness

Suppose (ER.2) and (ER.7) hold for the stated physically normalized
fields along the same sequence. Then a subsequence has a common
coincidence-flat mixed hierarchy \(S_m\), for all finite field labels
and all \(m\), with
\[
 |S_m(F)|\le C_1^{m+1}(m!)^{p_1}\nu_{q_1m}(F)
 \tag{ER.8}
\]
for fixed \(C_1,p_1,q_1\). It is a limit of the original Wilson
correlations on every fixed compact coincidence-flat test. The
permutation, continuum translation and separated reflection-positivity
properties pass whenever the chosen finite F01 prescription has their
stated finite-cutoff tensor conventions.

This theorem does not supply full rotation covariance, interacting UV
coefficients, the requested energy/phase properties or a proof of the
remaining corrected reconstruction hypotheses.

**Proof.** Fix \(m\) and a finite tensor-label tuple. Choose a countable
dense set of compact smooth coincidence-flat tests in the completion
for \(\nu_{qm}\), also including rational finite linear combinations.
Every fixed finite collection is eventually supported in the central
half-torus, where (ER.7) applies. A diagonal extraction makes all of
these values converge. Linearity and the uniform seminorm bound pass
because each fixed finite relation is eventually inside that same
domain. The resulting bounded functional extends uniquely by density.
This argument requires no estimate on periodic-image contacts at the
prelimit torus boundary.

Proposition ER.1 identifies the same limit with \(S_{m,n}\). Repeat
the extraction diagonally over all \(m\) and all finite labels. This is
one subsequence of one bare Wilson sequence, not separate retunings for
different observables.

Compact coincidence-flat tests are dense in the Schwartz
coincidence-flat space for each fixed seminorm after increasing the
weight order by one. Multiplication by a smooth spatial cutoff
preserves flatness. Hence the common functionals extend to that full
test space with (ER.8); one may increase the fixed linear index
\(q_1m\) to cover the collar seminorm and this density step.
The limiting constant in (ER.7) is retained. The fixed-order errors
vanish, so no uniform factorial bound on their prelimit age-mark
constants is needed.

More explicitly, a smooth infrared source cutoff supported inside the
central half-torus and equal to one on a growing smaller box can be used
when evaluating Schwartz tests at finite cutoff. It changes neither the
Wilson action nor any eventually fixed compact test. A fixed Gevrey
cutoff has derivative constants of fixed factorial order, which are
absorbed by \(p_1\) if this explicit implementation is used. No periodic
image of a diagonal is treated as an ordinary Euclidean coincidence.

Permutation symmetry is exact for the original full moments and passes
by (ER.4). For a fixed physical translation \(t\), choose lattice
translations \(t_n\to t\). On any fixed compact support the torus
boundary is eventually absent. The finite Wilson law is translation
invariant and the fields have position-independent normalization.
The mean-value estimate for
\(F(\cdot+t)-F(\cdot+t_n)\), together with the uniform seminorm bound,
then makes the difference tend to zero. The error (ER.4) is also
uniform on this bounded test family.

For reflection positivity, take a finite polynomial in the physical
fields, with coincidence-flat kernels at positive time a fixed
distance from a common reflection plane. Its reflected quadratic
form uses joint tests which are flat within each half and separated
across the halves. It is nonnegative in every original Wilson law.
All of its finitely many moments converge by the same extraction,
so it is nonnegative in the limit. This is the CS.25 argument.
No positivity of a history-conditioned law is used. \(\square\)

## 5. What remains for the stated Yang--Mills target

The new reduction provides a precise place to concentrate the next
estimate: (ER.7), with the actual F05 normalization budget and
nondegeneracy. The archived raw-dependent component factors must either
be controlled in that marked estimate or retained in a proved larger
state space; local history compactness alone does not close their
operation.

Even after (ER.7), the original rotation-restoration, UV identification,
nonzero connected three-point, energy/phase and corrected reconstruction
requirements must be discharged. The underlying estimates state those
requirements, and this note does not weaken them. No mass-gap assumption
is introduced.
