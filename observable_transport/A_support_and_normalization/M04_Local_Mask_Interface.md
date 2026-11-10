# An explicit local-mask interface for the actual positive RG law

This is an **amended interface**, not a proof of the M04
statement. It changes the ambient support convention for the present
integration mask and specifies a corresponding off-support conditional
version. On the actual supported state it preserves the original
positive law, every marked integral, and every finite source jet.

The selection/lift answer is exact: adding history and mask labels while
retaining all old coordinates costs nothing in the value/direct/current
norm of a history-independent incoming raw mark, provided the old
regulator is retained at that intermediate stage. Coordinate pullback
and actual elimination remain separate operations and need their own
bounds. Merely appending redundant mask bits, without changing which
ambient data the conditional formula uses, does not remove the previous
obstruction.

## 1. The amended coordinates

Fix a finite cutoff and one ordinary regular step. Let J be the finite
universe of possible **present** independent free-coordinate slots after
the actual source exceptional-bond elimination. Its slot labels include
the native scale, coupling, storage block, Lie-algebra convention, and
physical bond footprint. These labels are external and do not change
when a mask value changes.

For each i∈J introduce two independent ambient coordinates:

\[
 r_i\in E_i,
 \qquad m_i\in\{0,1\}.
 \tag{LM.1}
\]

Here m_i=1 means that this slot is integrated in the present regular
step, while m_i=0 means that its value r_i is retained. The mask is a
primitive coordinate of the **ambient product**, with footprint equal
to the fixed physical slot footprint. One may bundle the finitely many
such slots in one current block into a finite mask vector. The number
per block at this one ordinary scale is bounded in terms of fixed L
and the gauge group. No bounded count is asserted for an arbitrary
collection of all historical modes.

Keep the original retained data θ, including all live source histories,
older coordinates, coarse fields and required gauge conventions. Their
old dependency footprints are unchanged. In particular a global old
history flag or a whole-component response has not been declared local.
The amended ambient output is

\[
 \widetilde{\mathsf Y}
 =\mathsf Y_{\rm other}\times
       \prod_{i\in J}(E_i\times\{0,1\}).
 \tag{LM.2}
\]

The original source determines a mask M(θ) from its live geometry,
including the literal bond-incidence convention. The **actual law** is
supported on

\[
 m=M(\theta),\qquad r_i=0\quad\hbox{when }m_i=1,
 \tag{LM.3}
\]

as well as all original source admissibility conditions. The value zero
is the old reference padding. There is no assertion that the masks are
stochastically independent of θ. Ambient coordinate independence and
probabilistic independence are different statements; only the former
is used in (LM.2).

This note promotes only the **present integration/retention mask**.
It does not automatically make the old determining geometry Ω_j,
component identity, hull, eligibility history, tree choice, or reference
field a local function. If a later argument wishes to promote additional
typed occupancy fields, it must specify the corresponding primitive
slots and repeat the conditional equivalence check. Encoding a whole
component descriptor in one locally stored value is not the construction
in (LM.1).

### 1.1 Full padded native regulator

At the output use the actual native compact-coordinate list, padded by
identity where inactive, and the **full padded retained free list**:

\[
 R^{\rm mask}_{h,X}
 =1+\sum_{p:\,\operatorname{foot}(p)\subset X}
          \beta_p s(V_p)
    +\sum_{i:\,\operatorname{foot}(i)\subset X}|r_i|^2.
 \tag{LM.4}
\]

The second sum has no factor 1−m_i. On the actual law (LM.3), it is
exactly the native retained free-coordinate energy. Off support it also
counts arbitrary numerical values in slots whose mask is one. This is
an explicit part of the amendment to the ambient regulator.

That convention matters for the summed mask-current envelope. If a
state has m_i=1 at many slots and arbitrary padded values r_i, separate
one-mask changes can expose each of their |r_i|² contributions. A
regulator Σ_i(1−m_i)|r_i|² followed by a supremum over **one** edit
would see at most the largest newly exposed value, rather than their
sum. The full padded list in (LM.4) does not have this defect.

No eliminated microscopic energy is added to the actual output law.
On support the newly counted inactive entries are zero. During a
passive lift before elimination, the regulator is instead the unchanged
**incoming** native regulator, as explained in Section 3.

## 2. Exact measurable equivalence on the supported state

The source finite padded state spaces are standard Borel. A finite
history decomposition is a positive kernel, and its actual coordinate,
gauge/coarea and normalized conditional operations are the fixed ones
from B-01/H-01 and C-01/C-07.

First suppose m=M(y) is a function of the geometry already retained in
the original output y. Define

\[
 \iota(y)=(y,M(y)),\qquad
 \pi(y,m)=y,
 \qquad \widetilde\mu=\iota_*\mu.
 \tag{LM.5}
\]

Redundant original geometric coordinates can be retained in y. They
still carry their original footprints. The graph Γ=ι(Y) is Borel;
π∘ι is identity, and ι∘π is identity on Γ. Thus the original supported
probability space and the amended supported probability space are
measurably isomorphic. Nothing was conditioned away or resampled.

Let P(dx,dy) be the original joint law before/after a regular step, and
q_y(dx) its actual backward conditional. The lifted joint law is

\[
 \widetilde P(dx,d\widetilde y)
  =(\operatorname{id},\iota)_*P.
 \tag{LM.6}
\]

For any positive probability kernel extension satisfying

\[
 \widetilde q_{\iota(y)}=q_y
 \quad\hbox{on the actual admitted support},
 \tag{LM.7}
\]

one has

\[
 (\widetilde QF)(\iota(y))=(QF)(y),
 \qquad
 \int G\,\widetilde QF\,d\widetilde\mu_{
 \rm out}
 =\int G(\iota(y))F(x)\,P(dx,dy).
 \tag{LM.8}
\]

This is just the defining disintegration identity, so it also covers
singular coarea measures and changing ranks. If the incoming stage is
lifted as well, push q_y forward by its incoming embedding. Repeating
this operation along the finite path gives conjugate Markov operators
on the supported graphs. Hence all tower identities, joint marked
moments, and finite formal source jets agree exactly. In particular

\[
 \int e^{\sum_a t_aF_a}\,d\widetilde\mu
 =\int e^{\sum_a t_aF_a}\,d\mu
 \tag{LM.9}
\]

whenever the displayed finite-cutoff integrals are defined; the same
identity coefficientwise needs only the corresponding finite moments.

Condition (LM.7) does **not** bound an ambient norm. There are many
off-graph probability extensions, and some have arbitrarily bad or
infinite currents. Sections 4–5 specify how the masks have to be used
for a substantive amendment.

### 2.1 Do not reveal already averaged histories

The preceding isomorphism requires that M be a function of the state
which the original operation already retains. It does not permit
recovering a hidden successful component descriptor after H03/C08 has
averaged it. Revealing such a descriptor can change the conditional mark.
An independent posterior resampling can preserve an already transported
mark, but needs its own exact source identity and compatibility with the
next operation. That different construction is not assumed here.

## 3. Passive selection and lift have exactly zero new mark current

Let x be the complete incoming raw state, still retained. Let
ℓ_x(dh) be any normalized positive source history-selection kernel;
it can be discontinuous and nonlocal. Include any actual normalized
gauge-choice auxiliaries in h. Let m=M(x,h) be its generated mask.
The lifted law is

\[
 \mu^+(dx,dh,dm)
  =\mu(dx)\,\ell_x(dh)\,\delta_{M(x,h)}(dm).
 \tag{LM.10}
\]

For every old mark F(x), its lift is

\[
 (LF)(x,h,m)=F(x).
 \tag{LM.11}
\]

The exact reverse kernel is the point mass at the **retained current
old state x**. Choose that same version on every ambient label:

\[
 q^{\rm lift}_{x,h,m}(dx')=\delta_x(dx').
 \tag{LM.12}
\]

This is a probability kernel even on an inconsistent or zero-selection-
weight label. It is not the specified inactive extension δ_{x_*}. The
choice (LM.12) is recorded as part of the amended interface.

For the direct/current filing, use its equivalent common-coordinate
presentation with a single dummy input u=*, reconstruction χ(*,x,h,m)=x,
and the constant kernel δ_*. The old B/J records then belong to the
direct coordinate pullback exactly as before, and no new kernel current
is created. If instead one keeps the physical point masses δ_x in a
pushforward-only filing, an old x variation is represented by a
point-mass kernel difference and its total-variation derivative can be
infinite. That different majorization is not used in the norm theorem.

For a new history or mask perturbation, the old state x does not move,
the kernel in (LM.12) does not move, and F does not move. Both direct
and kernel-current records are therefore exactly zero. For an old
coordinate perturbation, the old direct and current records are simply
carried along. No derivative of ℓ or of M is needed.

The same cancellation can be seen without a reverse kernel. A signed
finite difference of the normalized selection measure has total mass
zero. Pairing it with the mark F(x), constant in its selection variables,
gives F(x) times zero. This applies to hard selector jumps as well as
smooth positive selection probabilities. It must be done before any
absolute-value majorization of the separate unnormalized branches.

### Theorem LM.1 — exact norm preservation at passive lift

At the passive stage keep the full incoming native coordinate and
energy list, its external scale/coupling labels and its carrier
footprints. Give (LF)_X the same carrier as F_X. Lift each old compatible
record and put every newly introduced history/mask record equal to zero.
Then the M.11–M.12 value/direct/current norm, using the amended
coordinate inventory, is exactly the incoming norm.

**Proof.** The lift ignores all the new coordinates. Its value envelope
under old or new single-coordinate perturbations is exactly the old
value envelope, and the extra difference directions contribute zero.
The regulator is the unchanged incoming regulator and likewise ignores
the new coordinates, so its shifted envelope is unchanged. The x
marginal of (LM.10) is μ, giving equality of every averaged moment.
Carriers, weights and the physical unit h are unchanged. This proves
each summand of the norm identity. The product rule shows the same
statement coefficientwise for every finite jet. ∎

This theorem in particular covers the microscopic F01 Wilson functions,
which have their global compact-link formula independently of the
auxiliary history labels. It also covers an old mark already depending
on retained old history, with that dependence's **existing** cost kept.

It would be wrong to remove the soon-to-be-integrated energies from
the regulator at this passive stage, while the corresponding raw
coordinates are still present in F. It would also be wrong to cite
LM.1 after discarding x and conditioning only on the new masks. Those
are actual integration operations; their conditional marks need not be
constant in the mask.

Keeping x here is an intermediate exact disintegration, not permission
to keep eliminated microscopic fields or their energies in the final
coarse native list.

## 4. Rank padding and the complete conditional current algebra

Write the old current field in a common noise space. For each slot
take a fixed normalized reference probability π_i on its source free
cutoff domain. If a coordinate is integrated use its noise z_i; if it
is retained use r_i:

\[
 a_i(z,r,m)=
 \begin{cases}z_i,&m_i=1,\\r_i,&m_i=0.
 \end{cases}
 \tag{LM.13}
\]

Unused z_i are dummy internal noises with probability π_i and are
ignored by this assembly. They are not new retained state coordinates
and do not enter the output native regulator. This normalized padding
is optional: one may instead use point masses on inactive noise slots
and the finite signed-measure formulas below still hold.

Let χ_m(z,r,θ) be the **actual complete source reconstruction**, including
the exceptional solve, any coordinate relocation and every gauge
convention which has not already been undone by its exact identity.
Let ν_{θ,r,m} be its complete normalized conditional law, represented
on the common noise space with its actual density, constraints,
coarea factors, determinants, selectors and normalizer. On the graph
(LM.3) require the exact match (LM.7).

For a discrete one-mask change τ write ν'=ν_{τy} and ν=ν_y. Then

\[
 \begin{split}
 \widetilde QF(\tau y)-\widetilde QF(y)
 ={}&\nu'\big[F\circ\chi_{\tau y}-F\circ\chi_y\big]\\
    &+(\nu'-\nu)\big[F\circ\chi_y\big].
 \end{split}
 \tag{LM.14}
\]

The first term is a direct reconstruction/rank response. The second
is the normalized-kernel response. Since (ν'−ν)1=0, the second can
be centered by subtracting ν(F∘χ_y). No denominator other than one
is used for a discrete mask replacement.

This direct/kernel assignment is for the explicitly pulled-back
common-noise filing of (LM.13). In the physical pushforward filing
used by the Gaussian local-mask theorem and the primitive physical
quadratic-mask estimate, both the embedding and density changes
belong to J. The two exact filings are alternatives; their direct
and current records are not silently identified term by term.

More generally, if the pulled-back mark has compatible records
δA=B+J, its transported records are exactly

\[
 \begin{split}
 A'&=\nu_yA,\\
 B'_{\tau}&=\nu_{\tau y}B_{\tau},\\
 J'_{\tau}&=\nu_{\tau y}J_{\tau}
                    +(\nu_{\tau y}-\nu_y)A,
 \end{split}
 \tag{LM.15}
\]

with division by the native step for continuous directions. These are
M.30's identities on the new product coordinates. They neither discard
old currents nor assume a constant physical rank.

One may push ν_y through χ_y and work directly with physical old-state
probabilities. A bare physical mark then has no explicit retained-data
dependence and the new response is entirely a kernel current. In that
filing, changing masks may produce mutually singular physical kernels;
the finite signed-measure difference is still exact. A continuous
total-variation derivative may be infinite, so that filing does not
replace a needed chart-path estimate for a general incoming mark.

The product rules, finite jet logarithms/exponentials and Hölder grade
identities of M.23–M.25 remain unchanged. The regulator (LM.4) is
monotone under carrier union, and the same physical weight
exp{κ(|X|+t_h(X))} is used. Consequently the **support/current algebra**
is preserved. No uniform operator estimate follows merely from this
algebra.

### 4.1 Coordinatewise localization avoids unrelated storage closure

A global old flag may be stored in the same block as a local mask.
Blindly taking the full storage closure of that block can charge the
unused global flag again. Use instead one reset projector E_c for each
primitive coordinate c, including the mask coordinates. They commute.
For a finite coordinate set S define

\[
 L_S=\prod_{c\in S}(1-E_c)\prod_{c\notin S}E_c,
 \qquad f=\sum_SL_Sf.
 \tag{LM.16}
\]

Its declared carrier contains the insertion anchors and the full
footprints of the coordinates in S. The footprints of the original
non-mask coordinates have not been shortened. If f is independent of
a global flag c, every term with c∈S is zero. Thus unrelated metadata
stored at the same block cannot create an artificial carrier cost.

For a direction in coordinate c, set its localized records to zero
when c∉S. When c∈S omit the factor 1−E_c from the record-localizing
operator. The identity

\[
 \delta_c L_Sf
 =\Big[\prod_{d\in S\setminus\{c\}}(1-E_d)
       \prod_{d\notin S}E_d\Big]\delta_cf
 \tag{LM.17}
\]

follows because δ_cE_c=0 and δ_c commutes with every other reset.
It proves compatibility of the separately localized direct and kernel
records. This is the coordinatewise version of M.36a–c. It is a
supported representation, not a claim that every term has a small
carrier or that the resulting absolute sum converges uniformly.

## 5. A concrete positive all-mask extension at the first flat step

The first-step geometry obstruction has a particularly transparent
amended version. Fix Ω₁ full, V₁=1, and the literal soft-gauge operation.
Undo the exterior relocation if necessary. At these flat data it is
already exactly the identity. The complete primitive free-coordinate
density is a strictly positive smooth function

\[
 W_g(a)=\exp\{-\tfrac12a^*Ka+\mathcal W_g(a)\}
 \tag{LM.18}
\]

on a fixed small physical chart. Here W_g includes Wilson, soft gauge,
Haar, coarea and exceptional-coordinate factors, each once. The
source R-good product cutoffs are imposed separately. All current
R-bad and remaining approximate-fluctuation factors are retained-only
on an actual source geometry; the normalized conditional cancels them.
Initial redundant P/gauge selectors are one there. This is the source
factorization used in C7 and in the GO analysis.

Choose P=δ₀/g₀ and a fixed buffered radius bP containing every actual
retained first-chart value in this sector. Let s:E_i→E_i be a bounded
coordinatewise smooth saturation, identity on that admitted retained
domain, with image in a slightly larger b'P ball. For sufficiently
small g₀, g₀b'P lies inside the same fixed constraint chart. Its
Lipschitz constant is fixed. Use s(r_i) instead of r_i off that domain.
This is an explicit ambient continuation; it is not an estimate of the
original field at arbitrarily large ghost values.

Let π_i be normalized Lebesgue measure on the literal norm ball C_P.
For **every** ambient mask, define

\[
 \begin{split}
 a_i^s(z,r,m)&=m_i z_i+(1-m_i)s(r_i),\\
 \nu_{r,m}(dz)&=
 \frac{W_g(a^s(z,r,m))}
      {\int W_g(a^s(w,r,m))\prod_i\pi_i(dw_i)}
                        \prod_i\pi_i(dz_i).
 \end{split}
 \tag{LM.19}
\]

The denominator is positive and finite at every fixed finite cutoff.
Unused π_i integrate to one. On a consistent actual retained datum,
s(r)=r and (LM.19) is precisely the actual source conditional over
the coordinates I_m, with its product cutoff. Constants such as the
Lebesgue volume of C_P, Gaussian normalizations and source scale
powers cancel within this fixed-fiber ratio. They remain in the
unchanged actual outer law μ_out; no history-dependent factor is
removed from its branch probabilities.

Current R-history labels do **not** appear in (LM.19). Their exact
selection probabilities and their consistency with m are retained in
the outer law, not inserted as a zero-normalizer gate in this ambient
conditional. At fixed r,m, changing such an otherwise redundant label
therefore has zero output current in this first sector. A change of m
has the genuine direct/kernel responses (LM.14).

The physical reconstruction in this first chart uses the local C and
exceptional solve at the same fixed Ω₁,V₁. A one-mask assembly change
alters only one independent coordinate before those fixed-L maps.
Thus its **direct** physical reconstruction footprint is a fixed-L
neighborhood. The normalized conditional law can still respond
throughout the system. Bounding that response, its absolute supported
expansion, shifted envelopes and all source orders is an analytic
problem; it is not asserted by (LM.19).

This explicit construction shows that the proposed repair is more than
renaming the old global flag. At the two active GO data, the local mask
near the root differs. A nearby carrier can now distinguish them.
Changing a remote R label while holding the independent local mask
fixed leaves (LM.19) unchanged. The old lower-bound premise no longer
holds for this amended conditional version.

### 5.1 What would make the repair only notational

There are two ineffective alternatives:

1. Append m but continue to evaluate Q using the derived set Λ(H),
   ignoring the new mask. Then the lifted output is the same old
   function of H, with the same nonlocal dependency. Nothing was
   repaired.
2. Set the ambient conditional equal to the source ratio only when
   m=M(H), and use δ_reference otherwise. The consistency indicator
   itself then remains in the output formula. A remote H change at
   fixed m can create an order-one response, and the full footprint
   cost can return. Positivity and on-law equivalence alone do not
   bound that version.

The useful extension (LM.19) instead makes the independent mask the
actual rank argument off support and removes the canceled retained-only
selection gates from the normalized conditional. The outer supported
law is still exactly the original law.

## 6. The source-coordinate costs which remain

The following distinctions are essential beyond the flat first sector.

**Actual coordinate pullback.** A raw incoming F(x) becomes
F(χ_m(z,r,θ)). Even if F originally ignores history, χ_m can depend
on the geometry, old reference fields and coarea conventions. The
direct record in (LM.14) and the M.28a weighted chart path must be
estimated. Passive lift theorem LM.1 does not make χ local or give it
unit cost.

**Exterior relocation.** CMP119 (1.22), and its later analogue, change
retained exterior coordinates using a geometry-dependent reference.
At the GO centers they are identity. In general one can undo the exact
change, including its Jacobian, and use a pre-relocation retained chart
whose ordinary background is attached to Ω rather than the new Λ.
That is an equality of measures. Its pullback footprint and normalized
coordinate-path bounds are additional obligations. Treating the two
retained coordinate arrays as identical without that map would be false.

**Inherited complete density.** At a later step, old Gaussian
coefficients and completed E/B/R responses can depend on the live old
history and on the current reconstructed field. Merely replacing the
current integration mask does not remove those dependencies. All
source factors and normalizations must remain. A claim that the
conditional factors through only local masks requires an actual
factorization identity for that density, not a relabeling of its
geometrical arguments.

**Arbitrary nonflat ambient data.** Formula (LM.19) has a complete
positive extension on the fixed first flat chart. For a general native
background, source minima and coordinate charts have admission
conditions. A piecewise reference extension exists measurably, but can
have infinite continuous currents. A useful global extension needs a
buffered chart/patch construction and actual estimates. None is assumed
for an unproved complete-history family.

**History erasure and future operations.** Consistency remains in the
outer law. If a later operation averages masks or primitive histories,
its posterior depends on that actual law and can create nonlocal
normalized currents. A full revised induction must bound them. The
passive-selection cancellation does not apply after the physical
variables on which F depends have been discarded.

**Rank and moment budgets.** The final regulator contains only retained
native fields on support. Conditional moments of the eliminated
variables, changed-rank normalizers and direct path lengths are still
to be paid. The full padded off-support extension in (LM.4) handles
ghost retained values, not the actual eliminated microscopic energy.

## 7. The amended norm is not equivalent to the specified norm

The repair is deliberately substantive. For one mask slot b, the
function

\[
 f_b(r,m,\theta)=m_b
 \tag{LM.20}
\]

has a bounded local carrier in the amended interface. Its values and
one-mask differences are at most one, its other coordinate differences
are zero, and its moment norms are bounded for every actual supported
law. With a local anchor its M.11–M.12 norm is bounded by a fixed
constant.

Its restriction to the original graph is the derived membership
function M_b(H). In the actual pair of source histories constructed in
[M04 First Step Geometry Obstruction](M04_First_Step_Geometry_Obstruction.md), this bit near the extended
hole face changes when a remote R seed is added. All nearby primitive
data are unchanged and the native regulators are only polynomial in P.
The supported-carrier lemma GO.19 therefore forces an old-interface
cost at least c exp(cκMR₁)/(1+P²).

Thus restriction along the consistency embedding is not a uniformly
bounded map from the amended norm to the specified M03 norm. There is
no contradiction with the exact law isomorphism in Section 2: the
probability laws agree on their graphs, while the pointwise ambient
support/current norms are different. Nor is there a contradiction with
LM.1: its isometry concerns marks independent of the newly added
coordinates, whereas (LM.20) depends on a new mask.

A physical perturbation which changes a primitive R test **and then
updates all masks to restore consistency** is a composed path in the
new coordinates. It can change many nearby mask bits at once. The
amended elementary current at fixed independent masks is not a bound
for that composed path. Any downstream requirement for such a
consistency-preserving response must include its true path/current
cost. The previous obstruction cannot be hidden in a claimed bounded
change of norm.

## 8. Exact changes from the original interface

| Item | Original construction | Amendment in this note |
|---|---|---|
| Present Λ/activation data | Derived from primitive P/Q/R geometry, with full construction footprint | Independent ambient per-slot mask; its actual law remains constrained to that same derived value |
| Other histories and descriptors | Original full footprints | Unchanged; no whole-component payload is made local |
| Passive-lift null labels | Default reference-input extension can create an unnecessary version jump | Reverse kernel δ_x at the retained old state for every new label |
| Present conditional off support | Original generated version or consistency-gated ratio | Independent mask supplies the rank argument; canceled retained-only gates stay only in the outer law; (LM.19) is an explicit first-chart example |
| Padded retained energy off support | History-sensitive native-list reading can omit inactive ghost values | Full padded Σ|r_i|² regardless of m; identical to the actual native energy on support |
| Carrier construction | Blockwise reset/closure can overcharge unrelated stored flags | Coordinatewise supported reset representation (LM.16)–(LM.17) |
| Physical law and marked integrals | Original exact positive law | Unchanged on support, by (LM.5)–(LM.10) |
| Downstream completion | Original M03/M04 obligations | Requires an explicitly revised induction and norm-conversion/dependency analysis; no proof claimed |

The outcome is an exact, explicit alternative interface. Its passive
selection step introduces no hidden mark cost. Its genuinely difficult
steps remain the source reconstruction, complete conditional response,
physical carrier sums, and later averaging of the constrained history
law. Those estimates must be proved in the amended interface before
it can support a proof of M04.

### Sources and companion results

* Annex W §2.2: exact positive primitive
  history inventory and derived geometric domains.
* Annex Y (M.1)–(M.12), (M.23)–(M.39): native regulators, padded
  sectors, finite current identities, and compatible localization.
* C7.1 and CMP119 (1.18)–(1.26): actual fixed free-product regular
  conditional and retained-only selector cancellation.
* [M04 First Step Geometry Obstruction](M04_First_Step_Geometry_Obstruction.md) and its companion
  analyses: actual active pair, source normalization, and the old-norm
  lower bound which this amendment does not purport to prove away.
