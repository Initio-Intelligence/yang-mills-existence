# Coarsened protected atoms and the positive catalog

This note establishes the additional positive invariant used in the C-05
boundary estimate of the catalogue. The original Wilson operation and the
C-05 target statement are unchanged. Throughout, Q denotes
[Positive attachment bounds and the quotient forest](quotient_forests.md)
and M denotes [Majorants for marked atoms and composition of prefixes](marked_atoms.md).

## 1. Result

The linear-block norm passage is made precise by specifying the source representation and the order of the
operations. The atoms are the complete coarsened protected blocks. The
block is summed before its native Taylor expansion; the new Gaussian
parametrix is chosen only after the genuine map-factor insertion support
is fixed. The proof uses neither a sum of the old individual suprema nor
an identity between independently localized covariance and precision
families. PC.6 below states the resulting transfer theorem.

The ancestral-dimension question is resolved on the literal operative
source family by [CT.1](operative_source_scope.md). It is not resolved for a substituted history class
with an arbitrary number of independently admitted fine ancestors.

Two different issues must be separated.

1. The degree-one prefix cancellation in Q §18.7/M §28 is a statement about
   a sum of functions. It does not, by itself, control the sum of the norms
   of the individually localized functions. There is an exact finite
   localization-coarsening identity that can bridge this distinction when
   the localized functions come from a common master operator family.
2. The kernel estimate requires the literal source admission, not a class
   enlarged to arbitrary collections of small fine ancestors. The
   operative source scope supplies the proper-scale dimension bound for the
   complete intersections used by the actual component operation. Section 9
   records this resolution and preserves an abstract counterexample showing
   why the distinction is necessary.

Sections 9–11 resolve these concerns. The Gaussian
insertion-support issue is resolved as follows: keep the old coarsened coefficient
external, hold its new map records fixed, and condition only on their
genuine new Gaussian support. Section 10 proves the resulting common
operator construction. Neither resolution follows merely from a scalar bound.

## 2. What the source actually supplies at the final ordinary linear stage

LFR II, pp.375–377, first proves native admission (1.65), then tracks the
old-carrier exponent and the new localization-volume exponents in (1.66).
It defines the relative physical tree length in (1.67). The final
resummation gives one coefficient V(Y) per final domain, bounded in
(1.68); self coefficients obey the distinct, extensive estimate (1.69).

For ordinary inputs satisfying the source's full-tree hypotheses, keeping
the entire resummed V(Y) as one atom is legitimate. It does not imply an
absolute sum over its internal signed localization histories. If Y contains
a complete touched enlarged component and has nonempty exterior, the
physical tree visits its exterior shell and has a length of order R_k.
This gives a small ordinary nonself atom after part of the source exponent
is spent. This argument does not prove the same statement for an arbitrary
selectively free-core input.

The final paragraph on p.392 says that representation (1.104) may be used
in the inductive description. Completed retained components then have
multipliers depending on the new V_k and no old integral operation left.
This proves the disappearance of old integrated variables in a completed
component. It is not a bound on an additional positive norm of raw-slot
catalogs during a partially completed prefix.

## 3. Exact finite localization coarsening

The following lemma supplies a useful replacement for an unjustified
interchange of cancellation and absolute values.

### Lemma PC.1 — coarsening an excluded localization region

Let A be a finite set of localization labels and let f be a function of
parameters s_a, a in A, continuously differentiable to every required
order on the unit cube. Define commuting operators

\[
 E_a f=f\big|_{s_a=0},\qquad
 D_a f=\int_0^1\partial_{s_a}f\,ds_a.
 \tag{PC.1}
\]

The other parameters are retained until their own operators are applied.
For J contained in A, write

\[
 L_Jf=\Bigl(\prod_{a\in J}D_a\Bigr)
       \Bigl(\prod_{a\in A\setminus J}E_a\Bigr)f.
 \tag{PC.2}
\]

Let B be a subset of A. For every J contained in A minus B,

\[
 \sum_{I\subset B}L_{J\cup I}f
 =\Bigl(\prod_{a\in J}D_a\Bigr)
  \Bigl(\prod_{a\in A\setminus(B\cup J)}E_a\Bigr)
           f\big|_{s_b=1,\ b\in B}.
 \tag{PC.3}
\]

**Proof.** Expand the sum on the left as a product of E_b+D_b over
b in B. The fundamental theorem of calculus gives
(E_b+D_b)f=f|_{s_b=1}. All operators concern different variables and
commute. This proves (PC.3). No absolute value has been taken and no
factor depending on the number of labels in B occurs. The same identity
holds for Banach-valued functions, and under a finite measure integral
whenever the derivatives have an integrable common majorant. QED.

### Corollary PC.2 — a cancelled block can be localized as one atom

Suppose f_i are restrictions of a common type of master operator family,
their excluded sets E_i differ only inside a fixed region D, and
\(\sum_i f_i=f\) holds on that master family. Coarsen every output domain
by filling D. Sum all coefficients having the same coarsened domain
**before** taking a norm. The coarsened coefficients are exactly the
coefficients obtained by excluding all of D from the localization of f.

**Proof.** Use (PC.3) separately for each i on the labels in D not
already excluded by E_i. They are fixed to one. All i then have the same
outside localization operators. Sum i by linearity. QED.

The positive norm in this statement is the sum of norms of the new
coarsened atoms. It is not the sum of norms of the original individual
terms. For example, the two constant functions A and minus A have zero
sum but total absolute norm 2A. Common later self/nonself status does not
change this elementary fact.

## 4. Source application and the exact compatibility test

CMP116, pp.3–5, defines one generalized-walk operator family by attaching
the parameter s(Delta) to every walk whose support meets Delta. Excluding
a cube means omitting its multiplier, which is exactly setting that
parameter to one. Formula (1.9) is the product identity (PC.1)–(PC.2);
(1.10) discards disconnected terms that vanish. Thus PC.1 applies to this
literal fixed-walk localization family. The nonlinear source map is a
function of those same propagators by (1.5), and (1.13)–(1.18) construct
it on the parameter family. PC.1 remains valid after this nonlinear
composition; it does not require the source map itself to be linear.

For the proposed zero-remote prefix block, all carriers satisfy

\[
 X\subset Y_i\subset\operatorname{cover}(X\cup D(P)),
 \qquad F=\sum_iF_i.
 \tag{PC.4}
\]

If the entire block is carried as the single bounded insertion F, and
every later localization is coarsened by the same protected D(P), PC.2
gives an exact common-localizer passage. This is stronger than the
common-self-status statement in Q §18.7. A valid proof must explicitly
use these coarsened atoms as the atoms of its sufficient norm.

There is a useful exact check at an R interior branch. LFR II p.373
defines Y_1 as the smallest domain containing the input carrier and
every touched current component. If a current component H contains
D(P), then every Y_i in (PC.4) has the same first completion: filling H
erases the difference inside D(P). Consequently the determining set
B_1(Y_1) in (1.61) is the same. If subsequent nonempty localization
labels are also held fixed, the successive unions Y_2,Y_3,Y_4 and the
maps in (1.62)–(1.65) are the same. The linear block identity therefore
survives these substitutions on their common admitted chart.

At a branch external to the protected component, the same conclusion
requires the literal master-family identification of PC.2. Equality at
s=1 alone is insufficient. In particular, the source's independent
current extension and its domain-dependent projected reference cannot
be replaced merely because physical sums agree. The master-family
identity, or a separately bounded commutator, must be recorded for
every such operation.

The Gaussian localization in CMP116 §2 additionally chooses a special
localization domain X_0 tied to the insertion support Z_0, p.13. Thus its
operator family is not automatically identical for different insertion
supports. PC.1 applies after a common insertion support and common
generalized-walk family have been chosen. It does not, by itself, prove
that independently constructed source families with different X_0 have
the same coarsened coefficients. This compatibility needs either a
direct source identity or a separate argument carrying the block as
one insertion before Gaussian conditioning.

## 5. The geometric cost cannot disappear in the coarsening

Filling D(P) is an algebraic grouping operation. It does not turn every
point of D(P) into a free edge of the physical connector graph. A usable
coarsened norm must retain the actual protected core P, its real owner,
and the paid connector outside it. The footprint D(P) is support data.

For a fixed current root, moving it within D(P) costs at most a fixed
polynomial in R_r and a diameter factor exp(c_d R_r). The latter can be
paid by a spare collar exponent once. For several disjoint directly
used components, a crossed component releases a distinct paid collar
of length at least c R_r. Those released collars pay their individual
tag and diameter costs. A whole old carrier lying inside one component
has no such crossing and needs its once-allocated creation reserve.

These payments are valid only if the original creation label survives,
components are used once along that raw-slot lineage, and no new remote
raw dependency is hidden inside the grouped atom. The exact remote
normalized-kernel identity in M §24.2 keeps the denominator and is the
appropriate way of recording such a dependency. PC.1 does not establish
the smallness of its density difference.

## 6. Why the partial-prefix bounded-test estimate needs more

A bound on the number of all integration coordinates at a fine stage j
within an attempted component P by a fixed polynomial in R_j uses the
following printed facts. LFR I p.177(ii) says that no new large-field regions were created
there during the preceding N steps and that previous regions obey the
size condition on their corresponding scales. Page 179 says that all
components of the new regions are rectangles. Page 195 uses a nested
rectangular sequence for its gauge construction.

These printed statements need a source-matched argument that either
rules out multiple fine ancestor components in P or sums their effects
with a sufficiently strong depth weight. The fact that each component
is a small rectangle does not alone bound the number of components in
one later coarse block. Section 9 supplies the required argument.

### Lemma PC.3 — many small phases can produce an unbounded operator norm

For a real epsilon in (0,pi/2), put A_n={-1,1}^n and define the
normalized holomorphic kernel

\[
 (\Pi_zF)
 =\frac{2^{-n}\sum_{a\in A_n}
       e^{\varepsilon z\sum_{i=1}^na_i}F(a)}
       {\cosh(\varepsilon z)^n}.
 \tag{PC.5}
\]

For real z its density is positive. At z=i,

\[
 \|\Pi_i\|_{L^\infty(A_n)\to\mathbb C}
       =\sec(\varepsilon)^n.
 \tag{PC.6}
\]

**Proof.** The absolute value of each numerator weight at i is one,
and the denominator is cos(epsilon)^n. Hence the total variation of
the normalized density is sec(epsilon)^n. Equality is attained by the
bounded test F(a)=exp(-i epsilon sum_i a_i), which is fixed as a function
of a and has norm one. QED.

Every individual factor has an arbitrarily small phase when epsilon
is small. Nevertheless no fixed M_pref controls the joint operator
uniformly in n. The example is not a counterexample to the Wilson
construction. It proves that a branchwise small-phase claim and one
original coarse-block mark do not imply the kernel estimate used in
Q31h and Q44–Q45.

The common-reference strip lemma M §27.1 is correct when its joint
phase hypothesis holds. The issue is the actual-model verification of
that hypothesis uniformly over the source's full geometry.

## 7. A precise sufficient condition for the branching issue

Let B_j(P) denote the fine ancestor components at stage j in P. One
sufficient source-specific estimate is an oscillatory-phase ledger

\[
 \sum_j\sum_{Q\in B_j(P)}
       \operatorname{osc}_a\operatorname{Im}
             V_{j,Q}(\xi,a)
       \le \eta_r,
 \qquad \eta_r\longrightarrow0,
 \tag{PC.7}
\]

uniformly on the actual enlarged native/current/localizer chart,
including the Gaussian, Schur, constraint, Haar, ordinary interaction,
and internal-history factors. A bound of this kind must include actual
branch multiplicity. A reconstruction factor exp[-Gamma(r-j)] could
pay a factor of order L^{4(r-j)} if Gamma is large enough and if that
factor applies to every phase term on the actual independent native
family. It cannot be assigned to an arbitrary fine native variation
without proving its source origin.

Alternatively one may replace the arbitrary bounded-test norm by a
source-derived insertion norm carrying fine-branch energy or dependence
costs, and prove that the actual boundary atoms satisfy it. That changes
the sufficient intermediate norm but need not change the C05
target. It requires a model-specific estimate; a coarse value bound
for one resummed atom does not supply it.

## 8. Status before the source checks of Sections 9–10

PC.1–PC.3 are proved above. PC.1 gives a useful exact way to carry a
cancelled local prefix as a single atom. The fixed-walk source
localization and the R interior first-completion check support its use;
the complete Gaussian/domain-reference compatibility is proved
separately in Section 10.

The actual branching estimate (PC.7), or a sufficient structured-test
replacement, is not proved here. The repeated-history positive invariant is therefore
not obtained from (PC.7); Section 9 uses the operative source domains
instead. The C-05 target remains the stated target; no restricted-history
substitute is counted as a proof of it.

## 9. Resolution of the dimension question on the operative source family

The relevant admission is the literal component operation printed in
LFR I, not a new history class defined by a weakened verbal reading of
conditions (i),(ii). Page 177 states that the preceding regions for a
selected component are rectangles, then declares its notation Z_j to
mean the full intersections with the attempted union. Equation (1.1)
factorizes over attempted components. Thus within the factor for P the
operative domain is the complete intersection Z_j[P]. Page 192 bounds
the final Lambda and p.195 uses the nested rectangular sequence. Lemma
[CT.1](operative_source_scope.md) makes this scope explicit and proves

\[
 D_j(P)\le C_G[1+100LMR_{j+1}]^4.
 \tag{PC.8}
\]

Both sets of newly integrated coordinates A_j and B_j belong to the
actual stage strip within Z_{j+1}[P]; changing to the j grid costs the
fixed L^4 factor already displayed. The deep T_h operation remains
external to the partial prefix. This does not count the whole current P
at the fine j mesh. No new cutoff, eligibility schedule, or parameter
choice is introduced.

LFR II pp.385–386 also distinguishes the one-parent evolution
Z=S(Z_0) in (1.83) from a merger in (1.85). However its index j(Z) is a
first-large-field index, not an automatically identified eligibility
clock. The proof of (PC.8) uses the operative LFR I domains directly;
it does not silently change that index into a no-merger clock.

With (PC.8), the phase count in M §§21,29 is a fixed logarithmic
polynomial in the actual stage window. The strip lemma M §27.1 can
therefore be applied after its existing phase estimate. PC.3 remains
a useful exclusion: the same operator estimate has not been proved for
arbitrary many-branch histories substituted for these source domains.

## 10. Common Gaussian conditioning uses only genuine new variables

This section resolves the Gaussian-family compatibility question of Section 4.
The crucial point is that the support of the old native coefficient is
not the support of the newly integrated Gaussian variables.

### Proposition PC.4 — common support for a protected linear block

Consider a zero-remote linear block (PC.4) produced by a retained failed
component P at attempt r. Assume the actual source ordinary-growth and
preparation geometry used in Q §§12,16: D(P) uses at most two proper
layers, while the next ordinary enclosure supplies four. Until complete
consumption, D(P) is inside the retained large-field region and is disjoint
from the newly integrated ordinary Gaussian coordinates.

At the next ordinary step, perform the following operations in this order.

1. On the common admitted native family, sum all internal-localizer
   pieces of the block by PC.1. Its external insertion is F=sum_i F_i,
   with its old raw variables fixed.
2. Expand the new native response in its actual map records. For each
   fixed Taylor degree and fixed tuple of those records, sum the old
   coefficients before Gaussian integration.
3. Let J be the union of the genuine new Gaussian supports of those map
   records and any other explicit ordinary primitive factors in the
   same marked term. Condition on J and use one fixed Gaussian
   localization family for this term.

The result is an exact representation of the marked ordinary operation.
It uses one Gaussian operator family for each fixed tuple of new records,
and its determinant/trace support cost does not include D(P).

**Proof.** Write the actual source response as v(A), where A denotes
the new Gaussian field and old raw variables remain external. At finite
volume, Taylor expansion on the admitted common affine chart gives

\[
 F_i(U_0+v(A))
 =\sum_{m\ge0}\frac1{m!}
       D^mF_i(U_0)[v(A),\ldots,v(A)].
 \tag{PC.9}
\]

The equality sum_i F_i=F holds as an equality of analytic functions on
this same chart after the internal localization choices have been summed.
Consequently

\[
 \sum_iD^mF_i(U_0)=D^mF(U_0).
 \tag{PC.10}
\]

Fix m and expand each occurrence of v into its newly constructed map
records. The coefficient D^mF(U_0) depends on external native/raw data.
It is independent of A. All A dependence is in the fixed new map
records, so their actual union J, rather than the union of old native
carriers Y_i, is an insertion support for the Gaussian conditional
integral. The same statement holds after ordinary primitive factors
are included: enlarge J by their actual A supports only.

For real data, Gaussian conditioning is the exact Fubini/Schur identity
used in CMP116 (2.5), on this common J. The retained compact cutoffs are
included in the source expansion (2.3); their actual Gaussian variables
are included when they occur in a marked primitive. The identity is an
identity of the unlocalized Gaussian integral before any new decoupling
parameter is introduced. The source holomorphy and its common
integrable Gaussian majorants extend that identity to the admitted
independent native/current chart. It is not obtained by equating a
separately localized inverse with the inverse of a localized precision.

Choose the single special domain X_0 and the accompanying walk family
of CMP116 p.13 for this J. They are now the same for every term in the
already summed old block. Introduce the new localization parameters
only after this choice. The covariance, precision and square-root
families may be localized exactly as the source prescribes, independently
where the source does so. No inverse identity at nonphysical parameter
values is invoked. There is only one family to estimate.

In particular D(P) has added no A coordinate. A determinant comparison
has traces on the actual projected Gaussian subspace. A native site in
D(P) which carries no A variable is absent from that trace. Equivalently,
if one pads an insertion support by an unused Gaussian coordinate,
integrate that coordinate in the exact conditional identity before
taking absolute values; its normalized constant insertion is one.
There is no reason to pad by D(P) in the first place.

The exact construction is linear in each marked insertion before its
finite source products and convergent cluster sums are performed.
Internal coarsening is performed at finite volume and before an absolute
estimate, so (PC.10) does not exchange a cancellation with a sum of
norms. The positive Taylor majorant Q26 controls the single F after this
step and justifies the remaining normally convergent sums. QED.

The support estimate used in the Gaussian comparison is therefore

\[
 |J_0|\le C\,[L_{\rm paid,current}+1+V_{\rm new}],
 \tag{PC.11}
\]

as in Q §17.3. The new localization records account for V_new.
Exposed ordinary Gaussian vertices are on the paid old connector;
the protected D(P) contributes neither a new Gaussian volume nor a
factor exp(C R_r^4). Its external native footprint is retained for
derivative and future-support bookkeeping.

### Proposition PC.5 — compatibility with source resummation and self sums

Use the source-permitted boundary resummation of CMP119 p.262 as the
scalar representation convention. Carry the finer protected blocks of
PC.2 as an additional decomposition of those scalar coefficients. At
every operation, coarsen inside a protected block before its Gaussian
conditioning, and retain literal source self terms at a complete R step.
Then the block representation has the same unlocalized boundary scalar
and the same complete self scalar as the one chosen, coarsened source
representation. This convention is fixed before iteration and is not
changed between steps. No equality of self scalars from independently
chosen historical localization conventions is asserted.

**Proof.** The p.262 resummation groups boundary coefficients meeting a
given large-field component; the new declared domains either contain
that component or are disjoint from it. The printed bound replaces
d_j(X) by d_j(X minus Z_j), and the source explicitly states that its
constructions and proofs can be carried on with this convention. Our
finer block summation is an intermediate summation of the same finite
or normally convergent coefficient family. The final sum for a given
component is unchanged by associativity. The published scalar invariant
is retained separately; it is not inferred for arbitrary elements of
the additional selective positive norm.

The operations in PC.4 act on the same unlocalized scalar and use one
allowed source localization family after the input block has been
resummed. Native-current analytic identities are made before introducing
new localization parameters, and PC.1 identifies the coarsened coefficients
for this fixed family. This is the source representation selected for the
whole iteration. It does not compare unrelated localized inverses or
identify the self coefficients of independently localized historical
catalogs. The source scalar invariant and canonical bound are applied
to the literal self coefficients of this selected representation.

For the self projection at a later component H, a protected block has
one old deep owner. If its base carrier X is not contained in H enlarged,
no member of the block is self. If X is contained, ordinary whole-component
growth implies that H contains the old protected P and its D(P). Thus
every member is self. The projection commutes with the block sum.
For the interior R source maps, first completion fills H, so (PC.4)
gives the same Y_1 and determining set in (1.61). This common map can
be substituted into (PC.10); subsequent union/localization steps have
the same property by PC.1. The literal complete self scalar is therefore
unchanged. Its normalized canonical operation retains the source
bound (1.73)–(1.75).

If P is consumed successfully, it ceases to be an old protected block;
the output is assigned the separate successful-component mass budget.
If new raw dependence leaves D(P), its exact normalized density
difference is a separately marked remote response. Neither operation
creates an uncharged copy of the old block. QED.

## 11. The positive-catalog conclusion

The sufficient norm must be defined on the coarsened atoms of PC.2,
not on each of their internal localizer terms. The norm is

\[
 \sup_{\mathfrak h,a_{\rm ext}}\sup_x
 \sum_{G\ni x}w(G)
        \sup_{\xi\in\mathcal D^+}|F_G(\xi;a_{\rm ext})|,
 \tag{PC.12}
\]

where F_G is the complete internally resummed protected block, its paid
physical connector and old creation label remain in G, and D(P) is
external support metadata with the once-paid costs of Section 5.
This makes precise the phrase 'retain the original labels while using
the block norm.' The labels remain available
for the source self sum, but are not individually normed after their
exact internal sum has been used.

With the operative dimension bound [CT.1](operative_source_scope.md), the common positive-prefix
measure of M §27, PC.1–PC.5, and the original-block/no-resurrection ledger,
the two issues identified in Section 1 no longer require a new history
class, a fine-coordinate mark factor, or a volume cost for a decorative
native footprint. The remaining positive forest and chronological
capacity estimates must be applied to (PC.12). This note establishes these
interfaces; it does not itself establish the other C-05 map, native-jet
and endpoint estimates.

### Lemma PC.6a — the added footprint has a once-paid physical root cost

Suppose a protected block of original creation b is used by a direct
prefix at r. Retain the source window r-b<N_r, the actual ancestor
dimension bound [CT.1](operative_source_scope.md), the source ordinary-growth buffer, and the
original-block ownership rule Q §16.10. For a wholly contained
unguarded use, this block is a relative creation carrying its genuine
fresh collar-tail budget. A non-small original ordinary B or C_0 term
wholly contained in P belongs to the zero-mark ordinary reference law,
not to this reserved relative block. An ordinary term coupling P to an
exterior integration component has its own paid crossing and remains
in the guarded interaction catalog. In the coarsened norm (PC.12),
the added native footprint D(P) costs at most

\[
 C(1+\ell_b)^{D_*}\exp(c_*R_b)
 \tag{PC.13}
\]

once for a wholly contained creation, and a fixed factor times
exp(c_*R_r) per crossed component. The constants can be selected so
that a fixed spare part of the original collar reserve pays these
costs. No factor L^{4(r-b)} is required for an unguarded direct prefix.

**Proof.** A new root inside D(P) must be attached to a genuine old
raw endpoint in P. At creation grade b, that endpoint is in the
complete admitted ancestor Z_b[P]. [CT.1](operative_source_scope.md) bounds its b-block cover by
C R_b^4. It is not allowed to range over every b-cell in the coarse
current rectangle. All possible r for this unchanged creation obey
r-b<N_r; the AF window comparison bounds their number by a fixed
power of ell_b. The native integration/localization stage labels
and bounded stencil choices contribute another fixed power. The
number of current cells in D(P) and the root witnesses contribute
a further fixed polynomial in R_r, comparable to a fixed polynomial
in ell_b throughout this window. This proves the polynomial part
of (PC.13).

Any two current points in one D(P) are separated by at most C R_r.
For m endpoint directions there is a connecting tree with length
at most C m R_r; hence its divided-tree weight exp(gamma tau/m)
costs at most exp(C gamma R_r). The same diameter cost bounds
the change of a single physical current root. Choose gamma and
the connector-rate allowance below a fixed available collar share.
Window comparison then gives the exponential in (PC.13).

If the input graph has a terminal outside a directly used P, its
paid connector crosses the ordinary collar. After P is installed
as a protected core, that interior paid segment is removed from
the surviving exterior connector. Its released length is at least
c R_r. Distinct simultaneously used components give disjoint
segments. Later overlapping uses of the same raw-slot creation
would have to contain the previous retained failed P; its failure
clock puts their prefix lower endpoint above every old slot of
this creation. Such a use is impossible. Complete successful
consumption ends the lineage instead. Thus the released lengths
are not charged a second time.

At most one directly used component can contain the whole old
carrier. Its diameter and polynomial cost are reserved at creation
b from that relative creation's proved small tail. The constant
ordinary input B_0 is not used as if it supplied a fresh collar factor.
Since R_b grows faster than log ell_b, a fixed spare exponential
share pays every fixed polynomial in (PC.13). The unspent original
block marks pay the bounded operator factor separately. A remote
new raw response receives a new creation label only after its own
collar cost is paid.

The native footprint is not a free connector: paths between points
of overlapping footprints still use the actual protected cores and
their paid bridges. Any future forcing from the ordinary region
to D(P) crosses the remaining ordinary layers, so the same collar
estimate applies to its new response. This prevents coarsening from
creating a zero-cost connection between different cores. QED.

### Theorem PC.6 — protected-block transfer for the actual repeated history

Use the literal source/C01 admitted histories and AF envelope, the
source native/chart and absolute map bounds retained in the boundary
construction, [CT.1](operative_source_scope.md) for the operative prefix strips, and the already derived
ordinary-prefix phase estimate M §§21,27,29. Use the source-permitted
component resummation of CMP119 p.262 consistently, with a single
chosen convention throughout the iteration. Define the additional
positive norm by (PC.12), with complete protected blocks as atoms
and the original creation capacities retained.

Then the degree-one direct-prefix sector passes through every later
ordinary step, admitted preliminary step, retained failure and complete
component integration with its original capacity and no repeated fixed
normalization or localization loss. The primitive fresh-response bounds
Q43 and the chronological capacity recurrence A15–A16 apply to this
explicit norm. In particular this argument does not require an absolute
sum of the old internal source/localizer histories.

**Proof.** There are four exhaustive uses of a block.

First, it can be transported with no new forcing and no genuinely
integrated old variable. The block then remains exactly the same
analytic scalar. It contributes factor one.

Second, a new native map acts on it, while its raw variables remain
external. PC.1 and PC.4 allow the internal sum to be made before
Taylor expansion. Q26 now estimates the new records of the one
bounded atom. The Gaussian support is its actual map-factor
support, so Q §17.3 pays exposed vertices from the old coarsening
reserve and new vertices from new localization volume. Protected
attachments retain Q24's collar factor. The operation creates only
the new guarded load already listed in Q43.

Third, a prefix directly integrates some of its old raw variables.
The source whole-prefix common measure acts on the complete bounded
block, with the real exterior tuple fixed. Its M_pref factor is paid
by a distinct original-block mark. PC.1 retains the complete local
degree-one output as a block; PC.6a pays its genuine root and footprint
costs once. Any raw dependence created outside the protected footprint
uses the exact numerator-minus-denominator identity of M §24.2 and
has its own fresh guarded record. The retained failure clock prevents
reuse of the same original mark. No polynomial window count is
multiplied anew at every later transport.

Fourth, a complete R operation uses the block. PC.5 permits the
coarsened block sum to be taken before the literal self projection
and its native substitutions in the chosen source representation.
The canonical operation is its source operation with its source
bound (1.73)–(1.75). Complete consumption removes all old A variables,
as in (1.103)–(1.104). A successful component has the separate
volume-paying mass of (1.89), (1.95)–(1.99); a retained complete
component has the actual new coarse raw multiplier. Neither is a
continuation of an unpaid old direct-prefix event.

All nonlinear occurrences of blocks are handled after these linear
identities. Their products carry the union of the retained physical
graphs and submultiplicative weights. Creation labels and integration
marks retain their multiplicities in such a product: the mark ledger
is a multiset, with u_product at most the sum of the input counts,
not a set union that erases repeated paid reserves. Creation-capacity
indices are global grade/operation-sector indices; all spatial
component positions stay inside each rooted positive catalog.
One never sums a separate root supremum for every spatial component.
The two positive forest sums
use the genuine unordered-family factors of Q §§17.2–17.4.
The recent-input degree-at-least-two estimate uses one common
mark as in Q §17.6; no fresh fractional-power loss is assigned to
the degree-one sector just proved. PC.6a leaves the same fixed
positive rate floors and the same summable classes of fresh
loads. Therefore the primitive estimate and capacity recurrence
are unchanged, with only fixed constants and fixed logarithmic
powers enlarged once. Their AF sum closes exactly as in A15–A16.
QED.

### Scope of this theorem

PC.6 establishes the additional positive invariant on the unchanged
operative source family. It is not a theorem for arbitrary
abstract norm-ball inputs, arbitrary many-branch substitutes, arbitrary
complex old raw fields, or differentiated hard selectors. Those were
not obtained by the source admission or by this coarsening argument.
The original pointwise current and unsubtracted-native C05 targets
require the endpoint and native-jet arguments on this same norm,
given in [The complete boundary estimate on coarsened atoms](complete_boundary_estimate.md)
and [Proper-mesh coordinate counts, common positive domination and native jets](native_domain_count.md).

## 12. Consistency with the complete boundary estimate

This section checks [FC.1](complete_boundary_estimate.md)–[FC.22](complete_boundary_estimate.md) of
[The complete boundary estimate on coarsened atoms](complete_boundary_estimate.md)
against the coarsened-atom convention above, interface by interface.

**The recurrence is consistent.** In [FC.17](complete_boundary_estimate.md), the quadratic recent-input
bound uses the already summed rooted load K. With K of order a fixed
logarithmic polynomial times epsilon_k^(1/18) and sigma_k of order a
fixed logarithmic polynomial times epsilon_k^(1/72), its small-factor
exponent is 7/72. That is strictly greater than 1/18, so a new fixed
polynomial does not degrade the maintained tail exponent. The
degree-one contribution remains the old atom and is not charged through
this nonlinear bound. Fixed logarithmic powers can be included once
in the exponent v of [FC.16](complete_boundary_estimate.md).

The factor M_pref of a genuine direct prefix consumes an existing
original-block mark. The fixed root/diameter payment is PC.6a, not a
factor charged once per scale to every old component. Creation
capacities are summed after the spatial rooted bounds, so the norm
does not acquire a factor equal to the number of spatial components.
Choose A_* above the initial relative capacity before reducing the
ceiling; the actual bare Wilson relative capacity is zero. [FC.20](complete_boundary_estimate.md) then
makes both the fresh forcing and the accumulated auxiliary-rate loss
small, and [FC.21](complete_boundary_estimate.md) follows.

**The ordinary and relative classes remain distinct.** A non-small
ordinary B/C_0 term entirely internal to a prefix belongs to the
ordinary reference density. A genuinely crossing ordinary interaction
has its own source collar. Only a fresh relative creation uses its
original small tail for the one wholly contained unguarded event.
The p.262 scalar resummation convention does not promote arbitrary
unbounded large-field components to free cores of the selective
positive norm.

**The physical root passage retains the required costs.** The new
native footprint adds a fixed logarithmic root polynomial and an
exp(C gamma R_r) diameter factor, both paid by PC.6a. It adds no
Gaussian integration coordinate. For m current directions in the
same footprint, the divided-tree weight is bounded by exp(C gamma
R_r), not exp(C gamma m R_r). The remaining paid connector supplies
the order-4(m-1) moment used in [FC.4](complete_boundary_estimate.md). Thus this construction introduces no
additional factorial power.

**The native readout does not discard the zero-current term.**
The norm in [FC.8](complete_boundary_estimate.md) uses the common enlarged native contour for the
complete atom. Summing its internal coefficients before differentiation
commutes with a purely native first direction. Native dependence of the
old coefficient is retained when it is external to the Gaussian
integral. The unchanged Gaussian rank is not a claim of unchanged
native support. Consequently the existing native-root argument can
be applied to the whole block, including F_G(0,xi), on the same
contour and with the same native root count.

**The displayed current budget has the required asymptotics.**
In [FC.22](complete_boundary_estimate.md), theta_k tends to zero because q>p_0, and
g_k^(-2)D_k^3 is bounded by a fixed logarithmic polynomial times g_k.
The two remaining displayed inverse-coupling expressions retain
exp(-cR_k), which dominates all fixed coupling and logarithmic
powers because R_k is comparable to ell_k^r with r>1. The regular
boundary budget is bounded, and the R term has kappa_0 at least 12.
Thus K_B,k is uniformly bounded and K_B,k/P_k^2 tends to zero.
No exterior force is reassigned to the boundary scalar by this check.

The positive-catalog construction therefore supplies the
common-localizer/common-Gaussian passage used in the recurrence and
readout. This check does not identify the coefficients
of an independently localized historical representation with those of
the consistently selected source representation.

## Sources

- Bałaban, *Large field renormalization I*, CMP 122 (1989), pp.177–179,
  188–192, 194–195, especially (1.60)–(1.70).
- Bałaban, *Large field renormalization II*, CMP 122 (1989), pp.369–380,
  391–392, especially (1.61)–(1.75), (1.103)–(1.104).
- Bałaban, *Renormalization group approach to lattice gauge field
  theories II*, CMP 116 (1988), pp.3–7 and 12–17, especially (1.5)–(1.18)
  and (2.5)–(2.17).
- Bałaban, *Convergent renormalization expansions for lattice gauge
  theories*, CMP 119 (1988), pp.275–278, especially (3.43)–(3.47).
- Q: [Positive attachment bounds and the quotient forest](quotient_forests.md);
  M: [Majorants for marked atoms and composition of prefixes](marked_atoms.md).
- Lemma CT.1 of [Operative source domains and the ancestral dimension bound](operative_source_scope.md).
