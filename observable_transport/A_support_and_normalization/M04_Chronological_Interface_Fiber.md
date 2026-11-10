# Exact chronological fiber charts at a mixed interface

This note proves a local interface rank statement and an exact triangular
coordinate construction for the common chronological physical fiber. The
construction works at actual admitted paths. It does not replace a Schur
conditional mean by zero, and it does not identify a completed hard-cutoff
density with a smooth function. Its application to a global relative
completion estimate still requires the appropriate selector enclosures.

The source scope is the first family: h=1, Ω₁ full, initial P/Q good, a
specified bounded first R pattern, and no varying pre-h memory. The
microscopic A₀ law remains factored conditional on the full V₁. All charts
below start at the physical first-coarse field V₁ and involve j≥1.

## 1. Why the usual exceptional bond is not enough

For a coarse bond c, the original source exceptional bond b₀(c) is the
fine face-crossing bond in the straight coarse contour c. CMP109 printed
p.267 defines it explicitly. The corresponding coarse average contains
no b₀(c′) for c′≠c, so this is an especially convenient local constraint
solve.

At a fixed mixed raw interface, however, b₀(c) can already be held. A
coarse c crossing from a finer recorded block to an unrecorded block may
be an independent coarse readout, while its face bond intersects the
finer raw shell and is also recorded. Its whole averaging footprint is
not fixed, because the other block still contains unrecorded fine links.
The constraint is then not redundant. The incident-bond convention does
not by itself remove this case.

The terminal coarea construction TQ had the finite raw variables still
available for integration. It therefore does not, by itself, settle this
stronger question in which the physical master raw data are fixed. A
different, explicit connector inside the unrecorded block is useful.

## 2. The flat center-star connector

Let an L-block have center y. Write L=2m+1, with the source L>11. Orient
the 2d fine bonds incident to y outward. For each coordinate μ, denote
their Lie-algebra variations by u_{μ,+}, u_{μ,−}; in particular u_{μ,−}
is the variation on the oriented bond from y to y−e_μ, not on its
oppositely oriented standard representative.

Hold every other fine bond fixed and linearize all 2d outward coarse
averages incident to y at the identity field. The literal source average,
CMP109 (0.11)–(0.12), has first derivative equal to the average of the
corresponding contour sums. This follows from (0.8). The central U(c)
in (0.12) cancels the −c contribution at first order.

There are two contributions from this one block.

First, the averaged center-to-x contour contributes the same linear
functional

\[
 q(u)=\sum_{\mu,\sigma}p_{\mu,\sigma}u_{\mu,\sigma}
                                                               \tag{CF.1}
\]

to every outward coarse readout. Here p_{μ,σ} is the probability that a
uniform x in the L-block, followed by the source average over the
prescribed shortest center-to-x contours, begins with that star bond.
Every nontrivial shortest contour has exactly one first star bond and
never returns to the center. Hence

\[
 p_{\mu,\sigma}\ge0,\qquad
 \sum_{\mu,\sigma}p_{\mu,\sigma}=1-L^{-d}.              \tag{CF.2}
\]

No equality of the different p's is needed. Thus the argument also
covers a fixed shortest-contour prescription; the Euclidean average in
the source certainly satisfies (CF.2).

Second, consider the translated straight segment in the +μ coarse
average. Exactly m+1 starting points in the μ direction make it traverse
the outward +μ star edge, and m starting points make it traverse the
opposite of the outward −μ star edge. The transverse coordinates must
all equal the center coordinates. Dividing by the L^d starting points
gives the two coefficients (m+1)L^{-d} and −mL^{-d}. The −μ coarse
average has the reversed pair. Consequently the full derivative is

\[
 T=D+\mathbf 1p^{\mathsf T},\qquad
 D=\operatorname{diag}_{\mu=1}^d
 \left\{L^{-d}
 \begin{pmatrix}m+1&-m\\-m&m+1\end{pmatrix}\right\}.
                                                               \tag{CF.3}
\]

It acts identically on each Lie-algebra component. The two eigenvalues
of each block of D are L^{-d} and L^{1-d}. In particular

\[
 D^{-1}\mathbf1=L^d\mathbf1,
 \qquad
 1+p^{\mathsf T}D^{-1}\mathbf1=L^d>0.                  \tag{CF.4}
\]

The Sherman–Morrison formula now gives the explicit inverse

\[
 T^{-1}=D^{-1}
  -\frac{D^{-1}\mathbf1p^{\mathsf T}D^{-1}}{L^d}.
                                                               \tag{CF.5}
\]

Both T and T^{-1} have bounds depending only on fixed L and d. Any
subset J of the 2d coarse boundary readouts consequently has the right
inverse T^{-1}E_J, where E_J inserts the requested coordinates and sets
the other coordinates to zero. One can equivalently use the full
invertible star coordinate system Tu, solve its J coordinates, and leave
the complementary coordinates free.

This is a full row-rank proof for all the boundary constraints meeting
one block. Checking one nonzero derivative would not have sufficed.

## 3. Exact weak-field continuation and interface incidence

The source average is analytic in the finite two-block footprint, by
CMP98 Proposition 3 and CMP109 (0.8), (0.11)–(0.12). On an admitted
native regular neighborhood, put the finitely many blocks into a local
axial gauge solely for estimating this derivative. The path lengths and
loop areas are bounded by constants depending on L. Their plaquette
regularity therefore makes the derivative, after endpoint frame
conjugations, a perturbation of (CF.3) of size C_L ε_j. For sufficiently
small fixed regularity bound, the chosen boundary right inverse and its
nonlinear analytic solve have uniform fixed-L bounds.

The gauge used to estimate the rank is a fixed coordinate frame on the
local neighborhood. It need not be applied as a change of the held raw
data. Unit adjoint conjugations do not change the singular-value bound.
All gauge degrees of freedom of the actual primitive integral remain
present. In particular a later T₀ delta gauge must first be undone by its
full normalized Faddeev–Popov identity; one cannot use a center-star
variable which has simultaneously been fixed by an unrelated tree gauge.

For a fixed chronological level, the finer recorded region is a union of
aligned L-blocks after including the stated incidence collar. Classify a
coarse averaging constraint by its two blocks:

* If both blocks are fixed by finer master data, the coarse value is
  their actual chronological average. The constraint is a compatibility
  identity and is removed as a redundant normalized delta.
* If both blocks are unrecorded at this fine level, retain the ordinary
  source b₀(c) solve.
* If exactly one block is finer and fixed, its face bond may be held.
  Use the center-star connector in the other block for this boundary
  constraint.

For one unrecorded block, collect every constraint of the third type
into its set J. Equation (CF.5) proves their simultaneous independent
solvability. Center stars belonging to different blocks are disjoint, and
the two-block averaging footprint implies that they affect no boundary
constraint assigned to a different unrecorded block.

After solving those boundary equations, solve the constraints of the
second type using their face bonds. A face b₀(c′) for an internal coarse
bond does not occur in a different coarse averaging footprint, including
any boundary footprint. Thus these later solves do not undo the boundary
constraints. The full local Jacobian is block triangular, with the
center-star block and the ordinary exceptional blocks on its diagonal.

The source aligned geometry is essential here. If a proposed raw list
cuts the inside of an averaging block, first retain its full fixed-L
footprint in the near list. In the current application all changed
interfaces lie in the buffered source regions, so this increases the
finite native count by a fixed L-dependent factor. The center stars lie
strictly inside their unrecorded blocks, because L>11; they are not held
fine boundary bonds. This is the additional incidence fact missing from
the simple b₀ argument.

## 4. The chronological triangular chart

Let Ψ_j be the common finer determining sequence, with all ordinary
averaging footprints and interface collars included. Its raw master
values are the **actual chronological** physical readouts of the full
primitive path. They are not defined by setting all later ordinary
innovations to zero in a final minimum.

At a given level j, the master data determine V_j outside Ψ_{j+1}:
on the j-shell this is recorded directly, and in the still finer
complement it follows by literal successive averaging of lower recorded
data. The incidence recursion in PM applies to these physical readouts.
There is no assertion that distinct nonchronological averaging formulas
are associative.

Start at the highest level, with the fixed terminal field and the
recorded current raw variables. Descend in j. Suppose the complete
required V_{j+1} has been reconstructed. The older raw determining
variables for the source s minimum are already functions of the held
master data. Thus the ordinary source background at this level is known.
On a genuine source starred free bond b, its exceptional correction
vanishes exactly, and the inverse coordinate is

\[
 A_j(b)=g_j^{-1}\frac1i\log
 \left[V_j(b)\big(M^jU_{j+1}\big)(b)^{-1}\right].       \tag{CF.6}
\]

The complete source gauge convention is understood in this equation.
Any earlier localized coordinate change is undone with its Jacobian
before (CF.6) is used. There is no Taylor approximation in (CF.6).

Assign the unrecorded ordinary free entries, except the finite selected
interface compensators. Assign every held fine master bond its prescribed
physical value. Section 3 solves exactly the remaining boundary and
interior averaging constraints. It yields V_j and the required selected
compensating source coordinates. Continue to j−1.

This constructs a local coordinate system on the **same physical fiber**
for either history. The fixed master data and terminal constraints are
preserved exactly. All solving variables at a mixed interface lie in the
finite near list; the rest of the ordinary variables can retain one
history's actual free coordinates as the far parameters.

The original interlacing supplies an important admission fact. With
Ψ_{j+1}⊂Λ_{j+1}^s∩Λ_{j+1}^t, the unrecorded blocks and the fixed-L
interface collar lie in the ordinary regular domains Ω_{j+1}^s and
Ω_{j+1}^t, separated from their old fine holes by the source buffers.
Thus the new solves occur on native regular blocks. Where one history
has an old finer hole, the common finer description simply retains that
finer data; it does not ask for a coarser regular chart inside that hole.
This is a local admission statement at an actual supported path. A
larger proposed integration box still needs its own admission proof.

The local solves are unique on the native small-angle neighborhoods:
their derivatives are uniformly close to the fixed invertible matrices
above. Keeping the nonsolving star combinations as free coordinates
makes the coordinate map square. All compatible redundant deltas are
removed by conditional disintegration, not evaluated at the identity.

## 5. Quantitative transport and measure bookkeeping

Normalize Lie-algebra variations at level j by g_j. Coupling ratios at
adjacent levels are bounded by the source (2.6), so no factor g_j^{-1}
is introduced at every level merely by changing units. The displayed
source powers of g_j in the original coarea measures remain explicit.

Each active native ordinary variational map has the source weighted
exponential row/column bound on its actual regular domain. The local
center-star and exceptional solves add fixed-L finite-footprint maps.
Products are taken in one fixed mixed weighted norm, at an exponent
strictly below the source exponent. Its submultiplicativity gives the
conservative derivative and inverse bound

\[
 B_N\le [C_L(1+R)^q]^{C N}.                            \tag{CF.7}
\]

An N-fold loss is allowed here. This estimate is used only to propagate
a small far forcing. It is not multiplied by a generic nonlinear Taylor
remainder g·poly(R,P). Such a multiplication would be unjustified when
N=R is a high power of log g^{-2}.

In particular, a perturbation of far free coordinates whose influence on
the near constraints is bounded by poly(R,P)e^{-κT} has compensating
near displacement bounded by B_N poly(R,P)e^{-κ'T}. The exact implicit
solves can be continued along this perturbation as long as it stays
inside the native regularity buffers. With T=A R log(1+R), A large, this
quantity is smaller than any required polynomial or fixed inverse power
of g in the admitted source hierarchy. No far coordinate is first set to
zero. All actual conditional means and all positive Schur completions
therefore remain in the density.

At one level the coarea determinant is the product of the fixed-L
interface determinants, the original source exceptional determinants,
the Haar/exponential factors, and the explicit g_j powers. The global
change is triangular in chronological level, so its determinant is the
product of these diagonal determinants. A conservative finite-list
logarithmic ledger is

\[
 C D_{\rm near}\log(P+R+2)+C N D_{\rm near}\log(R+2)
   +C\sum_j D_j|\log g_j|.                            \tag{CF.8}
\]

It is of the type already allowed in ER. The possibly extensive number
of unchanged far coordinates is not included in D_near and is not
charged to that finite ledger. Their complete primitive density, before
hard cutoffs, is retained when applying a score or radial comparison.

For a small transport between two coordinate descriptions at the same
physical master data, the same triangular formula supplies its exact
Jacobian. The smooth score must be computed on the restored primitive
Wilson/coarea/gauge density. Differentiating the logarithm of an
integrated hard-cutoff completion is neither needed nor justified.

## 6. Exact scope

The result proved here is an admitted local common-fiber coordinate
construction, including the fixed-L interface rank
argument. Its quantitative inverse may grow exponentially in the window
length; distant exponential localization can pay that growth. The proof
does not need a polynomial inverse of a map obtained by setting all far
innovations to zero.

It does **not** say that the entire fiber at a fixed master datum is one
full product box. A global completion comparison still has to keep the
actual selector domains and establish inner/outer enclosures, or continue
the displayed exact transports on suitable buffered domains. In
particular the literal narrow (1.55) preparation cutoff recorded in
[M04 Quiet Selector Catalog](M04_Quiet_Selector_Catalog.md) cannot be treated as a high-probability
event by this chart theorem. It must be compared with its actual radius.

Nor does this result by itself prove the finite restored energy transfer,
the microscopic insertion estimate, or the specified M-04 carrier/current
bound. It is an exact residual coordinate result which can be used in
those questions when its hypotheses actually apply.

## Primary sources

* CMP109 printed pp.252–254, (0.3), (0.8), (0.11)–(0.12): the actual
  block, contour and averaging definitions used in (CF.1)–(CF.5).
* CMP109 printed pp.267–268: the actual b₀(c), the exceptional operator
  h, the nonlinear constraint solve, and the remaining starred entries.
* CMP98 Proposition 3, (122)–(126): analytic one-step averaging at a
  weak regular background, with fixed-L bounds.
* CMP119 (2.1), (2.10)–(2.12), (2.21), and (3.2)–(3.5): interlacing,
  old raw data, ordinary free fields, and the native source buffers.
* PM, TQ and FC: the chronological readout recursion, terminal delta
  bookkeeping, and the source mixed-distance estimates. None supplies
  the center-star rank argument in place of the proof above.
