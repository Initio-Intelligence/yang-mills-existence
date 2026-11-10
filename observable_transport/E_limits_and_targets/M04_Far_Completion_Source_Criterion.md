# Source control for the far cutoff completion

This note supplies the source geometric reserve and a primitive-density
score estimate for the outside-completion comparison OC. It keeps two
different issues separate. The mixed variational locality estimate is
available from the source once the actual held raw data are matched.
A common conditional chart must additionally retain the original
terminal and exterior conditioning when completed operations are
unwound. The latter identification is not a consequence of the rank
of the finite master list.

## 1. Same final core fixes the later domains and raw data

Let n=k−N₀+1, so the n-scale MR_n mesh has current physical size M.
CG.6a–CG.8, using the exact erosion/dilation identity, give

\[
 \Omega_n^c\cap Y=\Lambda+B_{4M},\qquad
 Z_n\cap Y=\Lambda+B_{6M}.                                \tag{FC.1}
\]

All subsequent quiet domains are determined by these sets. Hence
histories s,t in the same complete fresh class have identical
Ω_j and Γ_j inside Y for j≥n. On one common *physical* promoted raw
readout, PM.1 gives identical values on these common Γ_j. Thus
the differences in their original determining data occur only at
levels at most n−1. The old global tree representatives must first
be undone, or converted using their actual normalized gauge identity;
equal geometric sets alone do not identify arbitrary gauge
representatives of the data.

The source minimum U_k depends on Ω and its raw data, not on the
retained ordinary A variables by themselves; see CMP119 (2.10)–
(2.12), (2.23). To compare two such minima, refine their Ω
sequences, rather than silently prescribing additional A-dependent
raw data. For each original minimum assign its own exact averages
on the extra slots of the finer Ω determining set. The original
minimum remains stationary under these stronger constraints because
every new tangent variation preserves the old constraints. It is
in the refined regular domain, so uniqueness of the regular critical
orbit identifies it with the minimum for those refined data. Outside
the changed early determining region the refined data coincide.

This supplies a legitimate application of CMP102 Proposition 9,
(190), to differing geometries. One must not apply that derivative
formula to two different domains without this common refinement.
Compatible local center-fixed gauges are used for the comparison;
fixing the final one-step axial representatives uses only fixed-L
paths, and preserves the same exponential estimate.

## 2. The late memory crosses logarithmically many separated annuli

The primary CMP96 p.231, (2.46), defines the mixed distance by

\[
 d_\Omega(y,y')=\inf_\Gamma
    \sum_j (L^j\eta)^{-1}
             |\Gamma\cap B^j(A_j)|.                       \tag{FC.2}
\]

The source proof (2.47)–(2.58) decomposes a contour at the successive
scale surfaces and charges the portion crossing each intervening
annulus. In particular it does not replace this distance by a
current-scale Euclidean distance.

### Lemma FC.1 — late outside distance

Let D be the changed determining region from Section 1. Any admissible
contour from D to Y^c crosses the common separated annuli from n
through k, up to a fixed endpoint collar. The quiet construction
adds at least a fixed positive number of MR_j layers at each
stage. Thus

\[
 d_\Omega(D,Y^c)
       \ge cM\sum_{j=n}^{k}R_j-CM R_k
       \ge c_L M R_k N_0
       \ge c_L' M R_k\log(1+R_k)                          \tag{FC.3}
\]

for sufficiently weak coupling, with a changed fixed constant in the
last two inequalities.

**Proof.** At every intermediate scale the relevant component is a
nested rectangle, by (FC.1) and the quiet construction. Any continuous
path from the inner component to Y^c must cross every separating
surface, regardless of what happens outside Y. The physical gap at
scale j is at least c M R_j L^jη. Its portion in the corresponding
native annulus has weight (L^jη)^{-1}, yielding cMR_j in (FC.2).
Taking the last exit from each inner surface and the first exit
from the next produces disjoint path portions, exactly as in the
source decomposition. Fixed bond/interface collars remove at most
a fixed number of endpoint contributions.

The actual short-window coupling comparison (2.6)–(2.9) makes
R_j comparable to R_k for j in these last N₀ scales. This also
follows from the proved two-level radius lemma used in BD.1a.
Finally N₀=O(log R_k) with a positive comparable lower bound,
by its defining mesh equation. ∎

Consequently the native memory of changed early geometry at an
outside-Y ordinary cutoff has a stronger reserve than e^{−cR}:
it has e^{−cMRlogR}. The statement requires the equality of the
later raw data from Section 1. It cannot be inferred from equal
later geometric sets alone.

## 3. A finite collar measured in the actual mixed metric

One convenient enlargement exposes all native cells within mixed
distance

\[
 T=A R\log(1+R)                                           \tag{FC.4}
\]

of D, with fixed source incidence and averaging collars. Choose A
fixed, then M large enough that the ball remains inside the lower
bound (FC.3). Align and buffer its scale sections by the original
source blocks. Fixed rounding and separation costs are absorbed in
a fixed fractional increase of T.

Each scale section lies in the union of a fixed number of native
cubes of side C(R_j+T). The number of birth ancestors is bounded
in the literal eligible preparation, and the later quiet region
is one rectangle. Thus the exposed rank obeys

\[
 D_*\le C\sum_{j=1}^{k}(R_j+T)^4
        \le C R^5\log^4(1+R).                             \tag{FC.5}
\]

This metric collar is preferable to claiming that no late tail
exists once the domains agree. The late minima can still remember
the earlier raw data. Lemma FC.1 shows that this memory has sufficient
mixed-distance decay before it reaches outside Y. The enlargement
never needs an extensive first-lattice filling of the whole component.

## 4. The native ordinary maps have controlled finite-depth scores

Use the actual primitive maps on an active ordinary j-layer:

- the one-step averaging map and its exceptional-bond solve;
- the exact small-w source gauge sampler;
- the relative fluctuation reconstruction with its C and nonlinear
  exceptional correction;
- the current j-scale readout M^j U_{j+1} of the mixed variational
  minimum, with lower raw determining entries held fixed.

The last item is evaluated on the active Ω_{j+1} domain and its
fixed native collar. Its averaging footprint meets the j/j+1
neighborhood, rather than a deep older fine hole. CMP102 (190)
can therefore be averaged over that j-block before taking native
row and column sums. The input and output scales differ by one
fixed factor L; the microscopic integration factors cancel against
the native cell volume. CMP98 Proposition 6 is the corresponding
nonlinear average estimate. The C/D solve and sampler are fixed-L
local maps. The old mixed T₀ gauge is not inserted as a separate
large tree at every step.

It follows that first and fixed higher derivative rows/columns of
one such native map have bounded exponentially weighted norms on
an admitted buffered regular chart. A conservative notation for a
uniform one-step bound is C(1+R)^q. The actual local estimates
permit a fixed bound when all native norms and gauges are kept in
this one-layer form. No such assertion is made for a coarsened
readout deep inside an older fine hole; that uses the separate WA
mixed estimate.

The weighted norm is submultiplicative: the triangle inequality for
(FC.2) gives e^{μd(x,z)}≤e^{μd(x,y)}e^{μd(y,z)}. Thus an N-step
composition has the bound

\[
 B_N=[C(1+R)^q]^{C N}.                                    \tag{FC.6}
\]

A fixed loss in the decay rate is taken once in the one-step weighted
norm, not once per composition. This is the same convolution argument
used in CMP96 (2.52)–(2.58).

### Lemma FC.2 — score before hard completions are integrated

Consider a specified common conditional primitive chart with its
terminal and retained-data constraints imposed by the genuine
source coarea. Undo the complete ordinary integrations on the
N-step window, and if necessary the auxiliary first all-P integral.
Keep their independent hard selectors outside the smooth density.
Then the smooth conditional density in the far free coordinates
has coordinate scores bounded by

\[
 G_i\le Cg_k^{-B}B_N\,\operatorname{poly}(R,P),             \tag{FC.7}
\]

with fixed B, uniformly in total volume. This lemma assumes that
the conditional chart has the stated primitive construction and
admitted domain; it is not a statement about an arbitrary marginal
logarithm.

**Proof.** Before those integrations the original Wilson energy is
a sum of local group plaquette functions. Its derivative with
respect to a physical link is bounded by Cg_0^{-2}, including
plaquettes meeting fixed exterior fields, because all group
matrices are unitary. The column-sum bound for the composite
reconstruction controls the sum of the derivatives over all fine
links by B_N times the native input increment. This gives the
Wilson contribution in (FC.7) without a total-volume factor.

The soft gauge weights are retained in their exact independent
small-w coordinates. Their local logarithmic derivatives are
bounded by a fixed inverse coupling power. Haar densities and
exceptional coarea determinants are smooth local factors in their
buffered source charts. Their logarithmic derivative sums obey
the same chain/column estimate. Constant powers of the couplings
have zero derivative and remain in the normalization. A terminal
coarea section contributes the polynomial TQ ledger and its
polynomial local derivatives, rather than a discarded delta.

If the first all-P factor Z_P(V₁) is restored, its A₀ cutoff is a
fixed product cutoff independent of the held V₁. Its full Wilson,
gauge and exceptional factors are included as the first primitive
layer. No derivative of a hard completion is taken. If it is left
integrated, differentiation is justified only by this same restored
formula, with the common fixed cutoff, not by ignoring its boundary.

This proof uses the finite ordinary stack with no hidden pre-h
integrated history in the varying component. An inherited T_h is
not covered by the primitive Wilson score assertion merely by
renaming it a boundary factor. ∎

## 5. Conditional far comparison, with all normalizers retained

For the same physical field on an ordinary nonexceptional bond,
the exact relation between the two free coordinates is OC.10.
Section 1 and Proposition 9 give

\[
 \|a_i^t-a_i^s\|
 \le B_N\,\operatorname{poly}(R,P)
       \sum_{b\in D}e^{-\mu d_\Omega(i,b)}.                \tag{FC.8}
\]

The inverse relation has the same estimate. Therefore both good
cutoff domains have the required common inner/outer product
sandwich. Common original P/Q and gauge characteristic functions
must first be removed by their literal small-R redundancy
implications, or remain exposed near tests; an additional hard
restriction cannot be included in the smooth density of FC.2.

For outside cells at mixed distance at least T, summability in the
source mixed metric gives

\[
 \sum_i\delta_i
       \le B_N\,\operatorname{poly}(R,P,T)e^{-\mu' T}.       \tag{FC.9}
\]

The domain size does not occur. Combining the complete score
(FC.7), the radial product theorem OC.1, and (FC.9) gives

\[
 \left|\log{C_s(u)\over C_t(u)}\right|
 \le g_k^{-B} B_N^2\operatorname{poly}(R,P,T)e^{-\mu'T}.
                                                               \tag{FC.10}
\]

Here C_s and C_t are the actual unnormalized completions on the
same admitted conditional fiber, with the same conditional
normalizer. They can be arbitrarily small. There is no division by
an estimated all-good probability.

For N=R and T=A Rlog(1+R), the logarithm of the right side is at
most

B log(g_k^{-1})+[C−μ′A]Rlog(1+R)+O(log(R+P)).

Choose A sufficiently large, and then M so that FC.3 contains the
collar. The admitted R≥(log g_k^{-2})^r, r>1, makes this tend to
−∞. The source hierarchy also makes the enlarged finite ledger
in ER.13 negligible relative to the reserved failure energy.

## 6. The precise remaining identification

Equations FC.7–FC.10 apply only after the conditional chart has
been identified. The following points must be kept in its actual
construction.

1. Fixed current averages on Y\Λ remain the terminal deltas
   PM.10, with the TQ coarea. They do not become independent
   raw Haar entries.
2. If a promoted field is defined from a surviving A_j and the
   *final* reference minimum, it is an exact coordinate change
   of that finite source operation. It is not automatically the
   physical V_j on a fully unwound chronological path. Unwinding
   later completions must carry that reconstruction's pullback.
3. Fixed unreplaced old native variables, especially exterior A
   variables, have their actual source meaning. Holding an entire
   exterior physical path fixed can simplify the score, but one
   must then verify that both histories induce the same retained
   conditioning, or include the exact near-identity transport and
   its coarea between the two fibers.
4. Exposed near tests may still depend on the far fiber through a
   minimum. The fractional-mask version AE.7a–b needs only that
   they are uniformly true on the chosen low-energy set; a
   variational localization sandwich can supply this. They are
   not declared measurable in the finite readout merely by rank.

The existing exact full-path law, PM promotion, TQ terminal section,
and the native ordinary estimates supply the ingredients for these
checks. This note proves the weighted late-memory reserve and the
primitive score/completion implication. It does not silently mark
the remaining full conditional-fiber identification as completed.

## Mathematical sources

- CMP96 p.231, (2.46), and pp.231–233,
  (2.47)–(2.58): mixed distance, separating surfaces and
  exponential convolution summability.
- CMP102 Proposition 9, (190), and uniqueness of the regular
  critical orbit: actual minimum locality on a common determining
  domain.
- CMP98 (11), (122), (125), Proposition 6: exact gauge covariance,
  one-step exceptional solve and native average analyticity.
- CMP119 (1.14)–(1.30), (2.10)–(2.12), (3.15)–(3.25):
  complete primitive and completed actions, with their actual
  changes of variables.
- LFR I (1.10), (1.73): the final core and the common late annuli.
- PM, TQ, ER, OC and AE: separate coordinate, normalization,
  energy and fractional-mask interfaces used above.
