# Promoting the two finite raw/free lists to one raw determining set

This note proves the geometric and information-preserving part of the
common-chart construction. It also identifies the exact coarea factors
which must accompany the change. It does not identify two different
completed cutoff integrals with one density. That separate issue is
recorded in Section 6.

## 1. The literal interlaced domains

The primary image of CMP119, printed p.254, gives (2.1) as

\[
 \Omega_1\supset\Lambda_1\supset\Omega_2\supset\Lambda_2
       \supset\cdots\supset\Omega_k\supset\Lambda_k.       \tag{PM.1}
\]

This is stronger than separate nesting of the two sequences. In the
j-to-j+1 operation, the independent ordinary free field A_j is on

\[
 F_j=(\Omega_{j+1}\setminus\Lambda_{j+1})^{(j)},             \tag{PM.2}
\]

with the prescribed exceptional bonds removed. The raw determining
field is on

\[
 \Gamma_j=(\Omega_j\setminus\Omega_{j+1})^{(j)},
 \qquad \Gamma_k=\Omega_k^{(k)}.                           \tag{PM.3}
\]

Here the superscript includes the source point/bond/plaquette
convention, not a new endpoint convention. Formula (2.21), p.258,
retains exactly these two kinds of integrations. The source Gaussian
completion in that formula is part of the measure.

Since \(\Omega_{j+2}\subset\Lambda_{j+1}\), the coarse readout of a
promoted field on F_j belongs to the old raw layer \(\Gamma_{j+1}\).
It is not another free field at the next scale. This interlacing is
what permits simultaneous promotion without introducing inconsistent
coarse readouts.

For the first-family application, first A_0 has already been factored
as in FR/RB/LE. One may start this construction with the physical
first-coarse field V_1 and promote only A_j, j≥1. The local first
A_0 coordinates, if needed for a separate marginal calculation, have
rank O(R⁴); the complete global first all-P law is not part of the
finite count.

## 2. One-history promotion

Set \(\Psi_j=\Lambda_j\). Consider the mixed raw determining set

\[
 \mathbb B_\Psi=\bigcup_j
       (\Psi_j\setminus\Psi_{j+1})^{(j)},
 \qquad \Psi_{k+1}=\varnothing.                            \tag{PM.4}
\]

At the first scale in use, replace the lower endpoint \(\Psi_h\) by
the common ambient domain, keeping any prescribed exterior entries.
For h=1, Ω_1 is full and there are no microscopic Γ_0 data.

The actual nonlinear constraint chart in CMP119 (1.14)–(1.15), or
(3.15) at a later step, reconstructs the physical field on F_j as

\[
 V_j(b)=\exp\{i[g_jC_jA_j-h_jD_j(g_jC_jA_j)](b)\}
                  V_j^{\min}(b).                         \tag{PM.5}
\]

Its one-step average is exactly the prescribed V_{j+1}; the formula
is not a replacement of the nonlinear constraint by Q_jC_jA_j=0.
The latter only describes the independent chart coordinates after
the exceptional-bond solve. Retain the source's original gauge
representative, or retain its normalized gauge auxiliary explicitly.

The union of old raw V_j and (PM.5) gives V_j on
\(\Omega_j\setminus\Lambda_{j+1}\). In particular it gives the
entire new raw layer \(\Lambda_j\setminus\Lambda_{j+1}\).
The old raw entries in \(\Omega_j\setminus\Lambda_j\) become
redundant: they are the exact one-step averages of the lower fields
which have just been promoted there. Removing those redundant
entries means integrating their normalized averaging deltas, not
integrating them as new independent Haar variables.

Conversely, from the new raw data reconstruct every old raw datum
by the recursion in Section 4. Construct the original minimum from
those old raw data, using its original determining set Ω. Equation
(PM.5) then gives A_j directly: take the small relative logarithm
and restrict to the original independent nonexceptional entries.
The nonlinear correction is supported on the exceptional entries,
which are not new independent coordinates. Any original
relocalization must first be undone with its full Jacobian; its
inverse can subsequently be composed once.

Thus the promotion is an exact coordinate change on the original
admitted chart, with the gauge variables and coarea factors retained.
It does not require an iteration of inverse variational charts through
all N scales.

## 3. The two-history master and its rank

For two histories s,t with the same final fresh class and retained
exterior, take

\[
 \Psi_j=\Lambda_j^s\cap\Lambda_j^t.                        \tag{PM.6}
\]

These sets are nested by (PM.1). The usual mixed separation is
preserved under intersections: the complement of an outer
intersection is the union of the two complements, so its distance
from the inner intersection is at least the smaller of the original
distances. In the actual ordinary construction the stronger
interlevel buffer is visible directly in CMP119 pp.264–265:
the next Ω_{j+1} avoids a buffered cover of Z_j=Λ_j^c. A same-level
identity Λ_j=Ω_j after a reset does not remove that interlevel gap.

At the continuous-set level,

\[
 \Psi_j\setminus\Psi_{j+1}
  \subset (\Lambda_j^s\setminus\Lambda_{j+1}^s)
          \cup(\Lambda_j^t\setminus\Lambda_{j+1}^t),        \tag{PM.7}
\]

and

\[
 \Lambda_j^i\setminus\Lambda_{j+1}^i
       \subset \Gamma_j^i\cup F_j^i.                     \tag{PM.8}
\]

The source incidence convention adds only a fixed interface collar.
Include the one- and two-block averaging footprints at each such
interface. The domains are aligned unions of large source blocks,
and their separation is much larger than that collar, so this
increases the native count by a fixed L-dependent factor.

Every last-window layer has native volume at most C R_j⁴. Hence

\[
 D_{\rm raw}\le C\sum_{j=h}^{k}R_j^4\le C R_k^5.           \tag{PM.9}
\]

Restoring the entire preliminary annular list, rather than only its
surviving final B coordinates, still obeys this count: those
annular fields were subsets of the original last-window raw/free
lists. One may enlarge the changed-domain neighborhood by a fixed
multiple of M R_j at each native level without changing the power
in (PM.9).

This is a native mixed count. The whole current core must not be
filled at the first lattice spacing. At earlier ages that would have
exponential volume in N.

## 4. Exact determination of every original readout

The source one-step average on a coarse bond uses paths in the two
blocks adjacent to that bond; see CMP98 (14)–(15). We use its literal
chronological composition.

### Lemma PM.1

If two fine fields satisfy the same master constraints (PM.4), then
all their original raw readouts and all their promoted raw readouts
for either history coincide, up to the identical recorded gauge
convention.

**Proof.** Consider a desired j-bond. If it belongs to the master
j-shell, its value is prescribed. If it lies outside Ψ_j, use its
one-step average from scale j−1. The two adjacent averaging blocks
lie in the lower complement because Ψ_j is a union of aligned
blocks; all required lower values are either master data or are
obtained by the same recursion. A boundary bond and every crossing
footprint are kept by the source incidence collar.

For an original raw bond in Γ_j^i which lies in Ψ_j, it cannot lie
in Ψ_{j+1}, since Ψ_{j+1}⊂Λ_{j+1}^i⊂Ω_{j+1}^i. It therefore
belongs to the master shell. The same argument applies to a
promoted bond in F_j^i, since it is outside Λ_{j+1}^i. All other
cases reduce to a lower scale. Induction proves the claim.

No direct j-average is identified with a distinct averaging formula.
The proof only uses the successive normalized one-step constraints.
Center-fixed gauge transformations preserve the next average by
CMP98 (11), so the recorded gauge changes preserve the same
readouts. ∎

Let U_Ψ(v) be the regular minimizing field for the master determining
set. It satisfies the master constraints by CMP119 (2.11)–(2.12).
By Lemma PM.1 it has exactly the original raw readouts of any
admitted fine representative with those master data. It can therefore
be used to evaluate these readouts without replacing their law.

An original free coordinate is then extracted directly using its
original minimum U_{Ω^i}, formed from the recovered original raw
data, and the relative logarithm in (PM.5). Thus the required maps
are one master variational map, one original variational map, the
actual averaging readouts, and a direct one-step inverse constraint
chart. Source Proposition 9 supplies uniform-depth analytic
variational bounds on its admitted mixed domain. Quantitative
readout bounds still have to use the native averaging estimates;
raw dimension alone is not a derivative estimate.

### Terminal constraint precision

In the reset integral, the current field is fixed outside the
prepared core Λ, not merely outside the old region Y. A promoted
raw list based on the old Λ_j may have finer entries in Y\Λ.
The prescribed current field there remains the exact constraint

\[
 \delta_G\!\left(
     (\mathcal A_{h:k} V_h)|_{\Lambda^c}\,v^{-1}\right).
                                                               \tag{PM.10}
\]

Intermediate redundant higher readouts can be removed by their
deltas. The fixed terminal deltas (PM.10) cannot be discarded.
They add no independent rank, but they determine the physical
constraint quotient and its coarea normalization. The final
Gaussian comparison has to retain that quotient.

### Lemma PM.2 — terminal constraints have only logarithmic depth

Let n=k−N₀+1 and let C be the next-grid cover of all old
Z_{n−1} ancestors inside the final component. Its mesh in current
physical units is M. Quiet geometry gives

\[
 S=\Omega_n^c\cap Y=C+B_{8M},\qquad
 \Lambda=S\mathbin{\ominus}B_{4M}.                         \tag{PM.12}
\]

The exact formulas are LFR I (1.10), (1.73), with the source
complement/enlargement convention. Erosion need not distribute over
a union; only the always-valid inclusion

\[
 C+B_{4M}\subset\Lambda                                  \tag{PM.13}
\]

is needed here. Physical nesting puts every Z_j, j≤n−1, inside C.
Hence every promoted variable at a strictly earlier level than n−1
is at least 4M current units inside Λ. All current average
footprints on Λ^c, including the possible crossing bonds, have
fixed O(L) current width. M was chosen much larger than this
footprint. They consequently meet native levels only

\[
 j\ge k-N_0-O(1).                                         \tag{PM.14}
\]

The fixed N₀ is O(log R). Thus the terminal average constraints
in (PM.10) need no chain of inversions through all N=R old scales.
Their actual local one-step constraints can be solved through at
most O(log R) levels. If one adds T_j=A R_j log(1+R_j) collars,
the finest newly exposed level meeting a terminal footprint is
lower by at most O(log log R), so the same conclusion holds.

This is a geometric statement about where the constraints occur.
A quantitative coarea bound must still use the genuine one-step
exceptional solves there, keep any gauge anchors, and remove
redundant constraints by disintegration. Evaluating a redundant
Haar delta at the identity is not a finite Jacobian bound.

For completeness, (PM.12) also gives the later-domain redundancy:
for S=C+B_{8M}, the parallel-set identity
S=(S⊖B_{4M})+B_{4M} implies
Ω_n^c=Λ+B_{4M} and Z_n=Λ+B_{6M}. All later quiet domains
are determined by Λ. The changed domains of two equal-Λ histories
therefore occur only before n. Their T_j collars have current
radius O(Mlog R), and lie inside the common Y buffer of radius
M R for weak coupling.

## 5. Exact measure statement

At one promoted block, use the literal normalized group delta and
source coordinate map. The identity is of the form

\[
 dH(V_j)\,
 \delta_G(\mathcal M_j(V_j)V_{j+1}^{-1})
   =J_j(A_j,V_{j+1})\,dA_j,
                                                               \tag{PM.11}
\]

with the displayed source powers of g_j, the Haar density, the
linear exceptional-bond determinant, and the nonlinear constraint
Jacobian all included in J_j. A background translation is Haar
invariant at fixed coarse datum. Dependence of the background on
the coarse variable does not permit dropping J_j; the conditional
coarea identity already accounts for it.

Undo a completed integration only together with its full E/B/R,
vacuum and cutoff-completion identity. Then apply (PM.11), retain
the gauge samplers, and remove only truly redundant intermediate
deltas. This proves that the promoted description has the exact
pushforward of the original operation, with any unexposed
completion factors carried along.

No dimensionful factor is hidden in an assertion of Jacobian one.
The physical forest gauge and group connector transformations may
have Haar Jacobian one, as MT proves; the Lie/free-coordinate and
constraint transforms in (PM.11) have their actual nontrivial source
Jacobians.

## 6. What this settles and what remains

The finite promoted raw state determines both original finite lists
and their final retained readout. It supplies a direct route to
uniform-depth analytic readout estimates through the mixed
variational theorem. It avoids an N-fold succession of inverse
charts, and preserves the actual terminal constraints and gauge
factors.

It does not prove that completed ordinary cutoffs outside this finite
list are identical. The later Ω_j depend on the preceding Λ_j even
when no new P/Q fields occur. Consequently an ordinary small R
cutoff can use a different background in s and t far from the
changed region, although that difference is expected to decay
exponentially. The complete source factors generated by integrating
such a cutoff must either be restored or compared relatively.

The current route is to retain M R_j collars of every changed domain
and use the actual variational locality estimate outside them.
There the two free-coordinate descriptions differ by a summable
shift of size poly(R,P)e^{-cR}. A product-ball radial comparison can
control the corresponding completion ratio without dividing by its
possibly very small mass. This requires the exact common physical
fiber and a complete density score bound on its admitted cutoff
buffer. Those are additional estimates, not consequences of
(PM.9).

## Primary sources

- CMP119 p.254, (2.1): exact interlacing (PM.1).
- CMP119 pp.255–258, (2.2), (2.10)–(2.12), (2.20)–(2.22): raw
  fields, minima and retained independent fluctuations.
- CMP119 pp.248–250, (1.14)–(1.15), and pp.267–270, (3.15),
  (3.25): actual nonlinear constraint and coarea identities.
- CMP119 pp.264–265, (3.2)–(3.5): the next Ω domain includes the
  eight-layer buffered cover of the preceding Z_j=Λ_j^c.
- CMP98 (11), (14)–(15), and Proposition 6: covariance, local
  averaging footprints and native analytic average bounds.
- CMP102 pp.277–279 and Proposition 9, p.309: admissible mixed
  constraints, unique minimal orbit and analytic variational map.
- LFR I (1.14)–(1.29), (1.53)–(1.62): the full preliminary
  annular fields and their completed cutoff factors.
