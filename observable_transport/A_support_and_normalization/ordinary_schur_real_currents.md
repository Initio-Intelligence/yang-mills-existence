# Real old-coordinate currents of an ordinary Schur vertex

This note treats the explicit retained free-coordinate slots of the
ordinary Gaussian response. It requires no holomorphic extension of
those slots. It does not estimate a hidden old-coordinate dependence
of the coefficient or an arbitrary inherited boundary activity.
Those coefficient responses remain explicit in the statement.

## 1. The actual quadratic and its coefficient response

CMP119 (2.21), with the complete background-current correction
in CMP99 (3.156), retains an ordinary Schur quadratic. Its localized
terms have the form recorded in Annex AS (OR17.9):

\[
 q_X(a,v)=-\frac12 a_r^{\mathsf T}D_X(v)a_s.
 \tag{SC.1}
\]

Here r and s are actual independent old free coordinates, the
source tree/walk tag remains part of X, and X includes the physical
footprints of both endpoints and of the coefficient. For the
interaction in the current regular integral, D_X is the difference
of the same precision coefficient at the actual current field and
at zero current. Thus current-independent quadratic factors are
canceled only where the exact normalized ratio cancels them.

If the full precision is K and the eliminated block is I, write
\[
 S=K_{OO}-K_{OI}K_{II}^{-1}K_{IO},\qquad
 {\cal E}a=(-K_{II}^{-1}K_{IO}a,a).
 \tag{SC.2}
\]
At a real or admitted complex parameter variation,
\[
 DS={\cal E}^{\mathsf T}(DK){\cal E}.
 \tag{SC.3}
\]
Indeed the I component of K{\cal E}a is zero and the O component
of (D{\cal E})a is zero. Differentiating
\(a^{\mathsf T}Sa=({\cal E}a)^{\mathsf T}K({\cal E}a)\)
therefore cancels the two derivatives of the harmonic extension.
The inverse-block derivative has been included, not omitted.

The local coefficient expansions and the new current pullback
must supply the actual D_X(v) and its response. SC.3 is not a
locality estimate for a nonlocal function K(v).

## 2. A support-preserving real extension of the endpoint variables

On the actual ordinary support, suppose \(|a_r|,|a_s|\le P\),
where P is the literal source bound for those slots and P≥1.
Choose one smooth radial map \(\zeta_P:\mathbb R^{d_G}\to
\mathbb R^{d_G}\), identity for \(|a|\le P\), with
\[
 |\zeta_P(a)|\le 2P,\qquad
 |\zeta_P(a)|\le C|a|,\qquad
 \|D\zeta_P(a)\|\le C .
 \tag{SC.4}
\]
For example use a fixed smooth radial interpolation between the
identity and radial projection, after scaling a by P. The
interpolation can be chosen with the displayed universal bounds.
No new coordinate dependence is introduced.

Put \(b_r=\zeta_P(a_r)\), \(b_s=\zeta_P(a_s)\) and use
\[
 \widetilde q_X(a,v)=-\frac12 b_r^{\mathsf T}D_X(v)b_s
 \tag{SC.5}
\]
off the active support. This agrees with the exact quadratic
there. It is a specified possible endpoint extension, not yet
an extension of the entire interacting conditional kernel.
Its uniform value bound is
\[
 |\widetilde q_X|\le CP^2\|D_X\|.
 \tag{SC.6}
\]

The choice of P may be a conservative upper bound. A literal
shrinking cutoff can also use P=1. No assertion that all
normalized cutoffs grow is required.

## 3. Exact finite differences separate the two mechanisms

For any elementary allowed perturbation \(\tau\), with its
continuous parameter t when applicable, the product identity is
\[
\begin{split}
 \widetilde q_X(\tau x)-\widetilde q_X(x)
 =-\frac12\{&
 (b_r^\tau-b_r)^{\mathsf T}D_X^\tau b_s^\tau\\
 &+b_r^{\mathsf T}D_X^\tau(b_s^\tau-b_s)\\
 &+b_r^{\mathsf T}(D_X^\tau-D_X)b_s\}.
\end{split}
 \tag{SC.7}
\]
This identity also covers r=s. Divide by t in a continuous
direction and omit the division in a discrete one.

The first two terms are explicit endpoint currents. A unit
Euclidean direction at r or s has
\(|b^\tau-b|\le C|t|\). They consequently obey
\[
 \sum_{\text{endpoint basis directions}}
 \sup_{0<|t|\le1}|\delta_\tau^{\rm end}\widetilde q_X|
 \le C a_X\,\widehat R_X^{1/2},
 \tag{SC.8}
\]
if \(\sup\|D_X\|\le a_X\). Here \(\widehat R_X\) is the
actual shifted M.5–M.6 regulator. It contains the retained
free-coordinate energies at r and s, and their relevant shifts.
The fixed Lie-algebra dimension is included in C.

There is no old-A Cauchy estimate in SC.8. The coefficient is
held at its displayed shifted value in these endpoint terms.
Any dependence of that coefficient on the same old coordinate
belongs to the third term of SC.7.

Let
\[
 G_X=\sup_x\sum_d\sup_t
 \|\delta_{d,t}D_X(x)\|
 \tag{SC.9}
\]
with exactly the same allowed continuous/discrete conventions,
and all of the coefficient's genuine dependency directions.
Then SC.4 gives
\[
 |b_r|\,|b_s|\le CP(|a_r|+|a_s|)
              \le CP\,\widehat R_X^{1/2}.
 \tag{SC.10}
\]
The coefficient-current part of SC.7 therefore has bound
\[
 \sup_x\sum_d\sup_t
 \frac{|\delta_{d,t}^{\rm coeff}\widetilde q_X(x)|}
      {\widehat R_X(x)^{1/2}}
 \le CP\,G_X .
 \tag{SC.11}
\]

Combining the two parts yields the genuine half-grade
background-current estimate
\[
 (\widetilde q_X)^\natural
       \le C(a_X+P G_X)\,\widehat R_X^{1/2}.
 \tag{SC.12}
\]
Replacing the product \(a_ra_s\) by a uniform \(P^2\)
bound in every current would lose this useful half grade.
Keeping one endpoint energy in SC.10 is what preserves it.

For a padded discrete geometry change, SC.7 is still valid
when endpoints and coefficient tags have been represented on
a common fixed list. It does not establish such a list or a
small geometric footprint. The actual directions in SC.9
must be bounded before using SC.12 for those changes.

## 4. Consequence for the regular marked product estimate

Suppose the actual coefficient family has
\[
 \sum_X w_\kappa(X)P_X^2 a_X\le\varepsilon_0,\qquad
 \sum_X w_\kappa(X)(a_X+P_XG_X)\le\varepsilon_1.
 \tag{SC.13}
\]
Use the source-dependent P_X for the endpoints of each tag.
Equations SC.6 and SC.12 supply respectively a uniform
value interaction budget and the pointwise half-grade
current budget for these Gaussian vertices. The averaged
half grade additionally needs the actual outer endpoint
moments; a pointwise native regulator is not that moment
bound.

There is an alternative which avoids an old conditional
moment premise for this explicit Gaussian factor. SC.4
also gives the uniform bound
\[
 (\widetilde q_X)^\natural\le CP(a_X+PG_X).
 \tag{SC.13a}
\]
Thus the stronger weighted coefficient sum with this
additional fixed power of P supplies the averaged norm
under any probability law. OS.6 can pay that fixed power
when its actual spatial connector is present. One must
use either the true outer moment estimate or this stronger
coefficient budget in the product theorem.

If a marked root has grade one, its product with the current
in SC.12 has grade \(3/2\), using the real shifted union
regulator and Hölder with the actual joint law. For example,
if \(\|F\|_{L^p}\le Cp\) and
\(\|G\|_{L^p}\le C\sqrt p\), then
\[
 \|FG\|_{L^p}
 \le \|F\|_{L^{3p/2}}\|G\|_{L^{3p}}
 \le C' p^{3/2}.
 \tag{SC.14}
\]
The current and direct records remain separately tagged.
No cancellation between them or between different X is used.

For a genuinely surviving ordinary slot, OS.4–OS.6 in
M04_Surviving_Old_Slot_Geometry.md pay the explicit powers
of P_j and the density \(L^{4(k-j)}\), provided the source
coefficient connector carries the actual mixed distance.
That is a concrete way to sum SC.13. The full raw
coefficient/current construction is not inferred from this
endpoint algebra.

## 5. Exact remaining boundary

This result settles the explicit old free-coordinate
derivative of a correctly localized ordinary Schur vertex,
on an ambient endpoint extension that agrees on its actual
support. It also specifies the coefficient-response term
which cannot be specified.

It does not prove SC.9 or SC.13 for the complete inherited
boundary action. In particular it supplies no complex
old-A domain for a hard-cutoff completion, no derivative
bound for an arbitrary bounded B activity, no full
completed-component raw reference kernel, and no
discrete-history support theorem. These remain source
applications of the regular M04 calculation.
