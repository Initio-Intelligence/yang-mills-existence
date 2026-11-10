# A bounded young witness from the literal inner preparation rectangle

Source analysis and constructive geometric lemma by the

## 1. What the merger cases actually establish

LFR II pp.385--386, (1.83)--(1.85), separates an inherited component
`Z=S(Z_0)` from a component assembled from older components and newly
created bad regions. Formula (1.85) has separate sums for these two kinds of
ancestor. The formula itself does not require the sum over newly created
regions to be nonempty. It is therefore unsafe to infer from the absence of
new `P,Q,R` tests alone that a component has a single unmerged ancestor.

CMP119 p.269 also takes the smallest rectangular parallelepiped of each
small connected component after (3.20). A general algebraic proof using an
idempotent rectangular-hull operator must first justify that convention:
one pass of hull replacement and saturated hull closure are different on
arbitrary sets. The proof below does not use a hull-commutation identity or
thin an ancestral history.

The stronger fact used by the **literal prepared operation** is on LFR I
pp.195--196. For one final component, it uses a single nested sequence of
rectangular parallelepipeds

\[
 \Lambda\supset Z''_k\supset\cdots\supset Z''_{h+1}
        \supset\text{the last inner hole}
\]

to construct the annular tree. It constructs one tree on each successive
rectangular annulus and links them in one chain. It does not describe a
forest construction for an arbitrary collection of separated inner holes.
In particular, `Z''_{h+1}` is a single rectangle in this per-component
construction. This inner property, rather than the eventual small size of
`Λ` alone, controls the total early ancestry.

The theorem below applies to every complete fresh-reference class produced
by that literal rectangular-chain preparation. It does not silently extend
the operation to a more general forest interpretation of eligibility.

## 2. Source geometry and physical meshes

Use the common physical lattice of the source and put

\[
 h=k-N,\qquad a_j=L^{j-k}MR_j.
\]

Thus `a_j` is the physical side of an `MR_j` region cube at scale `j`.
The admitted one-step coupling comparison and the rounded-power definition
of `R_j` give a fixed constant `K_R` such that

\[
 a_{j+1}/a_j\le K_R.                                 \tag{MW.1}
\]

Only this bounded ratio is needed. More explicitly, write
`x_j=log(g_j^{-2})`. The source one-step coupling comparison bounds
`|x_{j+1}-x_j|` by a fixed constant. For sufficiently weak coupling,
`|log_L(x_{j+1}^r/x_j^r)|<1`. Since `R_j` is the least power of `L`
above `x_j^r`, their exponents differ by at most one. Thus
`R_{j+1}/R_j≤L`, and `K_R=L^2` is a safe choice in (MW.1). The
constant is independent of `g,k,N` and total volume.

Let `C_h` be the next-grid cover of the union of **all** `h`-scale ancestors
of the chosen final component `Y`. The last `N` ordinary factors are the
good factors in LFR I (1.3)--(1.9). The quiet CMP119 geometry therefore gives

\[
 \Omega_{h+1}^{c}\cap Y=C_h^{+8}.                     \tag{MW.2}
\]

The `+q` notation here means addition of `q` layers of cubes of side
`a_{h+1}`. Formula (1.11) of LFR I applies at `j=h+1`, because the source
requires `N>N_0`. Its enlargement of the regular domain by five layers
erodes the old hole by five. For a possibly disconnected union it gives
the inclusions

\[
 C_h\subset C_h^{+3}\subset Z''_{h+1}
             \subset C_h^{+8}\subset Z_{h+1}\cap Y.  \tag{MW.3}
\]

The first nontrivial inclusion follows from a direct distance calculation:
every point within three layers of `C_h` has its full five-layer
neighborhood inside `C_h^{+8}`. Erosion of an enlarged arbitrary union
need not equal a smaller enlargement; no such equality is used.

These identities include all ancestors, not one selected lineage. Physical
nesting prevents clipping by `Y`: a connected old cover-and-padding piece
which contributes to a final component belongs wholly to that component.
An earlier component that eventually joins `Y` is already among these
ancestors.

## 3. The bounded-ancestor lemma

### Lemma MW.1

For one component in the literal rectangular-chain preparation, the total
number of `h`-scale region cubes in its ancestral union `Z_h∩Y` is bounded
by a fixed source constant. In particular, the number of ancestral
components is bounded independently of `g,N,k` and total volume.

**Proof.** By the literal inner-chain property,

\[
 A:=Z''_{h+1}                                       \tag{MW.4}
\]

is one rectangle, hence connected. By (MW.3) it contains every `h`-ancestor
and is itself contained in the actual `h+1` large-field region. Consequently
there is one connected component `K_{h+1}` of that actual region such that

\[
 Z_h\cap Y\subset C_h\subset A\subset K_{h+1}.
                                                               \tag{MW.5}
\]

This is a preceding component to which the eligibility size condition
applies. It lies in a cube of side `100 a_{h+1}`. The proof does not need
to know which hull replacements occurred in constructing it.

Every `h`-ancestor is contained in `C_h`, hence in this same box. Since
the ancestors are unions of cubes of side `a_h`,

\[
 \#\{h\text{-region cubes in }Z_h\cap Y\}
    \le (100a_{h+1}/a_h+2)^d
    \le (100K_R+2)^d=:J_* .                          \tag{MW.6}
\]

The harmless two accounts for endpoint conventions. Each nonempty ancestor
contains at least one such cube, so its count is bounded as well. No
assumption that the ancestors were already one component at scale `h` is
used. \(\square\)

The conclusion is stronger than a bound on the number of eventual coarse
cores. It bounds the number of actual `MR_h` cubes at the earliest scale
of the quiet window. This is why it gives a bounded birth-energy cost.

## 4. Reproduce every early component instead of deleting ancestors

Fix one complete fresh-reference class `r` and one actual chronological
witness for it. Keep its exact ancestral union `Z_h∩Y`. Each of its
components is rectangular and satisfies the old scale size condition, by
the source's eligible history assumptions. Every nonempty component has
the minimum padding required by the ordinary region construction; in
particular it can be written as the one-layer enlargement of a nonempty
union of `MR_h` cubes when it is reproduced by an `R` birth.

For each component `Z_h^{(i)}`, take its one-layer erosion and put the
strict local `R` seed of RT.1 in every cube of that erosion. Place the
seed away from cube boundaries by the fixed source test/constraint collar.
The hierarchy `M≫LM_2` makes these placements possible and their
stencils disjoint up to a fixed incidence constant. The seed is in the
actual independent constraint chart, including the nonlinear correction,
and keeps the exact `h`-average unchanged.

Its relative links stay below the `2δ_{h-1}` approximate `Q` threshold,
its curvature and soft-gauge variation are below the `ε` threshold, and
its literal free-coordinate `R` threshold fails strictly. Hence the exact
`R'_h` cover is the union of these erosions, and its one-layer enlargement
is **the original entire union** `Z_h∩Y`. No rectangularization changes
the result: its components are the original disjoint rectangles.

By (MW.6), the number of such seeds is at most `J_*`, up to fixed stencil
and convention factors. Their total quadratic/soft-gauge energy is

\[
 \mathcal E_{\rm birth}\le C J_*P(g_h)^2+CJ_*
                         \le C_*P(g_k)^2+C_* .       \tag{MW.7}
\]

The precision upper bound used in RT.1 applies to the whole seed vector;
it is not necessary to discard covariance between seeds. The couplings
on the admitted last-`N` window are comparable as in the original trial.

This replacement changes only the pre-`h` internal history in a positive
trial term. It is not a replacement of the full old operation, which
continues to sum all histories in `r`.

## 5. Exact matching of the later history and fresh reference

Starting with the identical set `Z_h∩Y`, follow the original quiet ordinary
region construction. Since there are no new bad selectors in the last
`N` ordinary steps, the deterministic cover, padding and actual hull
rules produce the **same** subsequent sets as in the chosen original
witness. There is no need to decide whether that original evolution is
best described as a merger: all its geometric operations are preserved.

The new `R`-only birth leaves `Ω_h` full locally, removing older raw
determining coordinates. It does not change the quiet domains
`Ω_{h+1},…,Ω_k`, which are constructed from the same `Z_h` and subsequent
regions. The source preparation (1.10)--(1.13) therefore has the same
later determining domains and the same available choices of interpolating
rectangles. Choose the original choices. This gives exactly the same
prepared `Λ`, final `Y`, and localization cutoff `ζ_Y`.

The fresh minimum is the one defined in LFR I (1.74), (1.77)--(1.79), from
the same current shell on `Y\Λ`. It does not depend on which pre-`h`
history was used in the trial. Choose the same fresh graph, anchors,
orientation and every other fresh-reference feature. All scale and
coupling labels are unchanged. The normalized fresh factor is therefore
literally the same one, so this trial belongs to the same complete class
`r` and the same coarea stratum.

All intermediate eligibility size conditions are inherited **exactly**,
since their region sets were not changed. Their count is also uniformly
bounded: there are at most `J_*` components before their possible joining,
and there are no new births in the window. The dimension and geometric
counts consequently obey the same estimates as RT.13 and TB.6, with a
fixed enlarged constant:

\[
 D_{\rm tr}+D_{\rm geo}
       \le C_*\sum_{j=h-1}^{k}R_j^4
       \le C_*R_k^5.                                \tag{MW.8}
\]

The homogeneous Wilson initialization has no preexisting nonempty `T_0`
core. A nonempty component with a full quiet window therefore has `h≥1`,
as used by the birth construction. A model with an externally prescribed
initial bad core requires a separate base case.

### Theorem MW.2 — a bounded same-class young trial

Every complete fresh-reference class produced by the literal one-component
rectangular-chain preparation of LFR I pp.195--196 admits a positive
young `R`-birth trial with the same `r`, exact later region sequence, and
the bounds (MW.7)--(MW.8). It is unnecessary to assume that its `h`-scale
ancestral union was one rectangle.

**Proof.** Apply Lemma MW.1, reproduce every ancestral component as in
Section 4, and retain the exact later geometry and fresh-reference choices
as in Section 5. The strict birth selectors and the identity-centered
prepared box are the source-coordinate checks RT.1 and TB.1--TB.7.
Multiplying their positive neighborhoods gives the required trial. All
constants acquire at most the fixed factor from `J_*`. \(\square\)

Thus the normalization estimate RT.17, its matched energy/rank moment
bound, and its weighted native consequence extend from the previously
stated unmerged witness scope to this full **literal rectangular-chain
prepared scope**. Their other source hypotheses and their exclusions of
raw/discrete carrier conclusions remain unchanged.

## 6. The precise boundary of the conclusion

The argument has not shown that the words “no new large-field regions”
alone prohibit all mergers. The formulas around LFR II (1.85) should not
be used to manufacture that implication.

Nor is eventual rectangularity of `Λ` sufficient for (MW.6). A history
with many separated old holes can have a small current-scale prepared
cover after enough coarsening. Without the inner rectangle at `h+1`,
packing only in `Λ` can cost a factor comparable to `L^{dN}`. That is
precisely the factor the old lower-bound trial cannot pay by one
`C P(g_k)^2` energy cost.

If a broader ledger treats arbitrary merging forests as eligible despite
not satisfying the inner annular-chain geometry printed on pp.195--196,
the present theorem does not supply that missing forest preparation.
Its exact gauge fixing, inner-coordinate split, trial matching and count
must then be specified and proved. No such extension has been inferred
from the source's rectangular construction.

This distinction is operationally checkable: inspect the actual prepared
descriptor's `Z''_{h+1}` on one final component. The literal source
operation uses one rectangle. A descriptor with several separated inner
pieces is not justified by the displayed one-chain annulus construction
without an additional argument.

## Primary pages

* CMP119 pp.251 and 258: smallest rectangular hull operation and the stated
  small-component rectangularity invariant.
* CMP119 pp.265--269: quiet `C^{+8}` and `C^{+10}` geometry; exact free
  constraint chart and separate approximate `Q`/literal `R` tests.
* LFR I pp.177--179: eligibility, all-good last-window factors, and the
  definition of `Z''_{h+1}`.
* LFR I pp.194--196: one-component convention, exact fluctuation domain,
  explicit nested rectangular annuli and the one linked tree.
* LFR II pp.384--386: operation `S`, one-ancestor case (1.83), and the
  separate old-component/new-region sums in (1.85).
