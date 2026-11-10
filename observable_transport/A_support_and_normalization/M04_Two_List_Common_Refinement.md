# Two actual annular lists have a finite mixed refinement

This note records the exact geometric and readout part of the proposed
two-mask comparison. It keeps the admitted N=R waiting rule. The common
mixed list has polynomial native rank even though the finest-lattice
volume of the whole current core is exponential in N. The remaining
analytic problem is a density and cutoff theorem on this list; the
rank statement alone does not prove that theorem.

## 1. Refine both domain sequences

Take two original ordinary/preparatory histories s,t with the same
current core, fresh-reference class and retained exterior. Work in
common physical coordinates. For their ordinary sequences define

\[
 \Omega_j^\wedge=\Omega_j^s\cap\Omega_j^t,
 \qquad
 \Lambda_j^\wedge=\Lambda_j^s\cap\Lambda_j^t.
 \tag{CR.1}
\]

Intersections are taken in the common aligned block partition. The
source inclusions and separation inequalities are preserved. For
example, if dist(Ω_{j+1}^a,(Ω_j^a)^c)≥δ_j for a=s,t, then

\[
 \operatorname{dist}(\Omega_{j+1}^\wedge,
                         (\Omega_j^\wedge)^c)
  \ge\min_{a=s,t}
       \operatorname{dist}(\Omega_{j+1}^a,(\Omega_j^a)^c)
  \ge\delta_j.
 \tag{CR.2}
\]

The same proof applies to the Ω/Λ margins in CMP119 (2.1).

At the point-set level, both relevant types of list obey a union bound:

\[
 \Omega_j^\wedge\setminus\Omega_{j+1}^\wedge
  \subset
   (\Omega_j^s\setminus\Omega_{j+1}^s)
      \cup(\Omega_j^t\setminus\Omega_{j+1}^t),
 \tag{CR.3}
\]

\[
 \Omega_j^\wedge\setminus\Lambda_j^\wedge
  \subset
   (\Omega_j^s\setminus\Lambda_j^s)
      \cup(\Omega_j^t\setminus\Lambda_j^t).
 \tag{CR.4}
\]

The first list supplies raw determining fields V_j. The second
supplies the surviving independent ordinary free fluctuations. Keeping
only the first would miss variables used by the original Q/R and
preparation tests.

### Bond and plaquette precision

CMP109 Sect.0, printed p.251, assigns a bond or plaquette to a
continuous domain when it intersects that domain. CMP119 (2.2), p.255,
applies the determining-set definition with this convention. One
should not silently commute this incidence map with intersections of
continuous domains at an interface.

There are two equivalent safe bookkeeping choices. Apply (CR.3)–
(CR.4) first to the continuous shell and then include all incident
bonds and plaquettes. Or use the literal source Boolean bond sets
and retain their fixed interface collar. In the latter description a
new incidence can arise only within one lattice cell of a boundary
where the two original inner domains differ. Because the next-domain
margin is much larger than one lattice cell, a bond at such a crossing
is within at most two cells of a bond of an original shell. Thus the
refined list is contained in a fixed local thickening of the union
of the original lists. This changes its cardinality only by C_d.
In particular boundary-crossing bonds are retained, not erased by
an informal open-set convention.

If a geometric convention additionally requires a small connected
hole to be rectangular, overlapping holes can be replaced by their
connected-component rectangular hull, and touching hulls closed
iteratively. At one scale there are only a fixed source number of
ancestral rectangles. Each has side at most C MR_j. Any cluster
which is connected through intersections has total diameter at most
C MR_j, with a constant depending on that fixed ancestor count.
Its hull therefore has at most C R_j⁴ native sites. Far separated
components remain separate. This is an auxiliary refinement; it does
not change the actual historical labels s or t.

Consequently the complete refined raw/free list has scalar rank

\[
 D_\wedge\le C\sum_{j=h}^k R_j^4\le C R_k^5.
 \tag{CR.5}
\]

The bound counts native coordinates at their own scales. It does
not replace the mixed list by all first-scale sites in Λ.

## 2. The original retained readouts are functions of the refined data

The exact one-step average on a coarse bond uses paths inside its two
adjacent blocks; see CMP98 (14)–(15). This locality, the aligned domain
partitions and the source boundary-bond convention give the following
recursive fact.

Suppose a desired j-scale bond does not belong to Ω_j^∧. Its two
adjacent averaging blocks lie in the lower complement. The j−1
values needed for its one-step average are either present directly
as refined raw data, or are already obtained from still lower refined
data. If it does belong to Ω_j^∧ and belongs to an original shell,
it is in the refined shell unless it is covered by an even finer
stored layer. In the latter case use the same recursion. Starting
from the lowest raw layer produces every original raw determining
datum. Interface bonds are present by the preceding convention.

Thus the maps to the original determining sets are literal
chronological averaging maps on the appropriate patches. They are
not obtained by equating an unproved direct j-average with a
composition. The corresponding original free coordinates are then
obtained from the actual original nonlinear constraint chart, using
the reconstructed original lower field, original background and
coarse datum. Its exceptional correction and coarea determinant
are the ones in CMP119 (1.14)–(1.15)/(3.15).

Center-fixed gauge transformations preserve the next average by
CMP98 (11). The annular gauge freedom is explicitly center-fixed
on LFR I p.182 after (1.25). Store the normalized gauge auxiliaries
and the original graph/representative choices. The final AL change
is the common fresh-reference change already recorded in FR.1.
There is consequently one common retained current readout outside
Λ, and each original test is evaluated on its own reconstructed
field and its own gauge convention.

This is a statement about exact maps on the common physical path
space. It does not say that a t test is the same scalar function as
an s test in s's final B coordinates.

## 3. Exact positive reinstatement, and what it does not estimate

At finite cutoff the complete effective action is defined by positive
conditional integrations. Undo each required integration together
with its whole E/B/R identity, vacuum term, coarea determinant and
cutoff completion factor. Retain all constraints in the common list.
Fubini gives a common positive mixed path measure. Its two projections
are precisely the two original disintegrations. Every hard old test
is still evaluated on the physical field prescribed by its own
history. This construction does not replace the full density by
the product of its named self terms.

The finite list in (CR.5) is the correct target for doing this
reinstatement locally. If one chooses to keep additional intermediate
readouts as redundant coordinates, their normalized group deltas
must be retained; they are not extra independent Haar variables.
If one removes a conditional integration, its normalizing factor
must cancel the corresponding completed-action factor exactly.
Neither factor may be discarded separately.

A normalized conditional restoration can also be described without
claiming a new chart: disintegrate the original complete path law
over the refined raw/free readouts and original gauge auxiliaries.
The identities above show that both original lists are measurable
projections. This yields an exact positive measure, including any
residual coarea singularity. A subsequent common analytic Gaussian
chart for that measure is an additional theorem, not a consequence
of the existence of the disintegration.

## 4. The remaining common quantitative theorem

To finish the two-mask use of LE.19 one needs an actual coordinate
representation of this finite measure with the following properties:

- A positive joint quadratic form whose Schur restrictions are the
  forms belonging to the two original lists. Its conditional means
  and determinant normalizations are retained, rather than
  iteratively estimated with a loss C^N.
- The complete nonlinear and inherited E/B/R correction, expressed
  in those same coordinates, has quantitative oscillation or
  derivative bounds on a common enclosing domain. The native
  background bound (1.69) alone does not identify this pullback.
- The pulled-back original cutoff domains have a common enclosure
  and a lower trial. The first failed t test on H_s must imply a
  lower bound of order H_R for the common reserved energy, with
  its actual relative/gauge variables and reference shifts.

For an exactly Gaussian joint law, completing the square once
proves the required common energy identity. Repeated conditional
estimates are unnecessary. A first-step type relative comparison
would transfer it to the actual measure if the complete joint
nonlinearity were uniformly o(1), or if its loss were o(H_R).
The polynomial rank in (CR.5) makes bounds of the form
g_k poly(R_k,P(g_k)) useful. It does not by itself rule out a
history-depth dependence in a chart derivative or inverse.

## 5. Why the short-window shortcut changes the specified construction

The local analytic preparation conditions allow a waiting time
of order log log g⁻²: LFR II p.363 requires
L^{−N}≤(log g⁻²)^{−ν} with ν≥2p₀+dr₀, while LFR I p.198 gives
an upper bound by a positive power of log g⁻² and a lower
absolute threshold. A shorter window is therefore a plausible
alternative construction.

The admitted ledger used here nevertheless retains the source
N=R_j rule from LFR II p.384, (1.80). This is explicit in NR20
([Annex BJ](../../history/Annex_BJ.md)) and in RN19
([Annex BC](../../foundations/Annex_BC.md)).
The p.384 induction is phrased with this waiting depth, and p.385
budgets at most R_j further quiet steps. Shortening the required
wait would reduce that budget, but would change the times at
which the actual reset kernel is applied. It needs a recorded
construction/version change and a matched proof; it is not an
identity for the specified law.

The finite refinement (CR.1)–(CR.5) avoids that change. Its rank
remains polynomial with the original N=R_j.

## Primary sources

- CMP109 Sect.0, p.251: literal point/bond/plaquette incidence convention.
- CMP119 pp.254–258, (2.1)–(2.12), and (2.19)–(2.22): mixed
  determining sets, raw fields, free coordinates and factorization.
- CMP98 (11), (14)–(15): exact gauge covariance and the local
  averaging paths.
- LFR I pp.178–183, (1.2)–(1.29): the original annular lists,
  their characteristic functions and exact positive integrations.
- LFR II pp.363, 384–385: preparation lower bound and the retained
  N=R_j chronological budget.
- [M04 First Birth Reassembly](M04_First_Birth_Reassembly.md) and
  [M04 Later Energy Reserve](M04_Later_Energy_Reserve.md): common first normalization and
  the still-needed two-mask energy implication.
