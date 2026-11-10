# A terminal-preserving mixed forest gauge using fixed virtual averages

The ordinary forest argument MT assumed a connected tree of actually fixed raw boundary edges. In the prepared operation some fixed quantities are higher averages instead. This note repairs that distinction. Fixed current averages are used as virtual boundary edges only in the holonomy comparison. The actual coordinate forest still consists solely of raw graph edges, so its Haar identity is unchanged.

## 1. Scope and the two edge types

Use the finite admitted mixed graph G and convex graded cover of MT, with at most D cells and edges, and a small native curvature ceiling ε. The source current reference U_0 is regular on a buffered current-scale box containing the construction. Its master raw values are `v_*=M_master(U_0)`. The current source preparation supplies this regular reference on the relevant core and collar; this assumption is not asserted for an arbitrary strong exterior.

Let v be other admitted master data on the same graph, with the same fixed terminal current averages. The exact raw-master determination lemma gives

\[
 \Phi(v)_c=\Phi(v_*)_c=v_{{\rm term},c}
                 \quad(c\text{ a held terminal bond}).
 \tag{VG.1}
\]

Every current endpoint is a vertex of the mixed graph because the aligned odd-L grids are nested. Add a virtual edge for each fixed current bond, with matrix `v_term,c`. It is endpoint covariant, since it is the literal chronological average. It is not asserted to equal the holonomy of the graded connection along the corresponding straight segment.

In the literal rectangular prepared shell, the graph of retained current centers outside Λ is connected by those held current bonds. Choose a tree T_B in that graph. Include any genuinely fixed raw boundary edges as well when they agree with the chosen reference and are required by the conditioning. All retained boundary roots of the final forest must be connected in this fixed augmented graph. An extra fixed raw boundary datum which does not agree with U_0 must instead be included in the reference constraint problem; it cannot be silently identified with a current average.

## 2. First bound the virtual-edge defect in an analysis gauge

Let `H_v(c)` be the holonomy of the GR connection of v on the geometric straight current segment c. We prove

\[
 \|\Phi(v)_c-H_v(c)\|\le C\varepsilon D^4,
 \tag{VG.2}
\]

with an inessential increase of the power if the fixed geometric box diameter is recorded separately. The estimate is endpoint gauge covariant and is thus independent of the gauge used in its proof.

For this proof only, use an ordinary spanning tree with one root and apply MT's cone argument to v and v_*. There is a gauge g_0 for which the transformed raw data satisfy

\[
 \|v^{g_0}v_*^{-1}-I\|_\infty
                           \le C\varepsilon D^2=:\delta.
 \tag{VG.3}
\]

This is an analysis gauge. It is not used as the final coordinate change and need not fix the terminal centers. It is legitimate for an endpoint-covariant estimate such as (VG.2).

At the reference, the master minimum is U_0 by variational uniqueness on nested constraint fibers. Proposition 9 applied to the data in (VG.3), followed by WA's actual raw-average estimate, gives

\[
 \|\Phi(v^{g_0})_c-\Phi(v_*)_c\|
                              \le C D^2\delta
                              \le C\varepsilon D^4.
 \tag{VG.4}
\]

Here `δ≤cD^{-2}` is required, or sufficiently `εD^4<c`. It holds on the source weak-coupling regime with ε equal to g times a fixed logarithmic polynomial. The inverse axial gauge in WA is included; the new Q average is not substituted for Φ.

The local Kato comparison of the two GR projections, with raw matrices differing by δ, identifies their bundle connections with a difference bounded by `Cδ/h_Q` on native cell Q. The identification is exactly the identity at every graph vertex. A current straight segment meets at most O(D) convex native cells, and its length in Q is at most `C h_Q`. Duhamel's formula for real unitary parallel transport consequently gives

\[
 \|H_{v^{g_0}}(c)-H_{v_*}(c)\|
                              \le C D\delta
                              \le C\varepsilon D^3.
 \tag{VG.5}
\]

This comparison uses the explicit local projection/Kato formulas; it is not an inference from derivative decay alone. There is no endpoint-frame error, because the Kato identification is the identity at both current endpoints.

It remains to compare the reference connection with its own current average. A current-regular U_0 on the containing box has, by the source local regularity theorem, a gauge with a bounded current-scale connection. If the current diameter of the box is M_B, one can take a bound `C M_B ε/H`, where H is the current mesh. This is the reference-only use of CMP102 (9); it does not assert a global weak-link gauge for arbitrary mixed data. Its ordinary averages at a native scale h have angle `O(M_B ε h/H)`. The GR formulas on these reference data therefore give a connection of size `O(M_B ε/H)`, since their local derivative costs h^{-1}. Both its current holonomy and the actual reference current average differ from I by `O(M_B ε)` in that gauge. Therefore

\[
 \|H_{v_*}(c)-\Phi(v_*)_c\|
                              \le C M_B\varepsilon.
 \tag{VG.6}
\]

The counted box permits M_B≤C D after a harmless increase of the constant. The source smallness condition for this reference-only gauge is satisfied because M_B ε is a fixed polynomial times g. Combining (VG.4)–(VG.6) and then undoing g_0 proves (VG.2).

The use of current regularity in (VG.4) and (VG.6) is explicit. WA.10 is not a bound for an arbitrary graded reference with a nonsummable sequence of homogeneous-scale curvature ceilings.

## 3. The final forest fixes every terminal center

Now choose a forest F consisting of actual raw edges, with one component rooted at each retained terminal/boundary vertex. Its interior vertices are all the remaining mixed vertices. Such a forest is obtained by extending the fixed augmented tree T_B to a spanning tree and discarding T_B itself. The virtual edges are in T_B, not in F.

Define the relative gauge outward from the roots by

\[
 g_x=I\quad(x\text{ a root}),\qquad
 g_y=v_{*,xy}^{-1}g_xv_{xy}\quad((x,y)\in F).
 \tag{VG.7}
\]

It puts each forest edge equal to its reference value. Because g is the identity at all retained current centers, the actual averaging covariance gives

\[
 \Phi(v^g)=\Phi(v)=v_{\rm term}
                     \text{ on every held terminal bond}.
 \tag{VG.8}
\]

Thus this final gauge preserves the terminal constraints exactly. It is distinct from the auxiliary gauge g_0 used in the proof of (VG.2).

To bound a nonforest edge, close its forest path using the fixed augmented tree. The loop has O(D) actual or virtual edges. Replace each virtual edge by the GR holonomy on its straight segment. The total replacement error is at most `CεD^5` by (VG.2). The resulting geometric loop has O(D) segments and is inside the admitted convex box. The GR curvature/cone bound controls its holonomy by `CεD²`. Apply the same reasoning to v_*, using the identical fixed virtual matrices. Comparing the two closed loops yields

\[
 \boxed{\quad
 \|(v^g)_e v_{*,e}^{-1}-I\|
                        \le C\varepsilon D^5
                       \quad(e\in G).
 \quad}
 \tag{VG.9}
\]

The power is deliberately conservative. For `ε=g P·poly(R)` it still gives a normalized Lie chart of fixed polynomial size, and the small-angle domain follows at sufficiently weak coupling.

## 4. Exact measure and constraints after the final change

The coordinate change uses only (VG.7), an actual raw-edge forest with fixed roots. Consequently the exact Haar identity MT.10–MT.12 applies with no additional virtual-edge determinant. The virtual edges were used to prove the estimate, not introduced as independent integration coordinates.

Every normalized gauge sampler and every Q/R/preparation selector is retained in the transformed integrand. The fixed terminal deltas are unchanged by (VG.8). One may then impose those deltas by the exact section/coarea chart of TQ, or use the original source constraint sequence. Their original coupling powers and finite Jacobian remain present.

The explicit forest products have length O(D), so their fixed-order derivatives obey the polynomial word bounds in MT.8. No differentiation of an artificial virtual-edge density is involved. The reconstruction of the original source samplers uses the exact small-w formulas MT.13–MT.17; the scalar's gauge invariance does not remove those weights.

This completes the terminal-preserving gauge part on the declared source-admitted finite chart. It does not identify two outside completion factors, prove a full restored energy reserve, or identify the positive energy with its common constrained Schur form. Those are separate analytic statements.

## References

- [mixed tree chart](mixed_tree_chart.md), MT.1–MT.12: finite graded cone bound, actual forest Haar identity and polynomial word derivatives.
- [graded bundle reference](graded_bundle_reference.md), GR.8–GR.13: explicit local projection, exact graph transport and Kato comparison.
- [mixed weighted averaging](mixed_weighted_averaging.md), WA.17–WA.22: actual raw readout bound with the inverse axial gauge retained.
- [M04 Raw Master Determination](M04_Raw_Master_Determination.md), PM.1 and PM.10: exact original/current readouts and fixed terminal constraints.
- CMP102 (9), (181), Proposition 9: reference-only current weak gauge, endpoint covariance and the mixed variational family.
- [terminal constraint chart](terminal_constraint_chart.md): exact terminal section and coarea bound on the resulting admitted Lie chart.
