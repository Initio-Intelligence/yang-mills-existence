# The complete restored source quadratics come from one constrained energy

This note identifies the quadratic energy before estimating the readout
maps. It concerns the first-reset, first-R-only branch with Ω1 full, a
fixed fresh class and a finite admitted restoration of its later ordinary
variables. The first innovation A0 is kept in its separate first factor.
It is not charged again to the later energy.

The exact quadratic identity below is proved from the actual source
normal form and its untruncated Gaussian completion. A nonlinear
comparison is then proved on the admitted finite chart, using the
source classical-action remainders. This does not identify two far
cutoff completions, or establish an inherited microscopic scalar budget.

The finite chart here is the specified native source operation after
the chosen complete partial integrations have been undone. Its
promoted readouts and its exact constraint maps must be those of
that operation. Replacing it by the final variational minimum of
an arbitrarily chosen physical master after additional far
completions are unwound is a different construction. Its
chronological readout/coarea identification is not proved here.
In particular the conclusions below hold for each declared
admitted restoration chart; they do not themselves construct a
common physical fiber for two complete histories.

## 1. The common minimum and the relevant tangent space

Fix the current retained data outside the prepared core Λ, the actual
reference orbit/representative, and every other feature in the fresh
class. Let U0 be the source minimum with those terminal constraints.
Work on its physical constraint manifold, after a valid gauge quotient.
The terminal-preserving forest and TQ give such local coordinates on
the declared admitted chart. Soft gauge samplers remain as actual
additional variables; they are not removed by physical gauge invariance.

Write the homogeneous Wilson functional as S. At U0 the ambient
gradient need not vanish. If Φ denotes the fixed terminal constraints
and λ their true multipliers, its physical constrained Hessian is

\[
 H=\left.(S''-\lambda\cdot\Phi'')\right|_{\ker D\Phi}.
 \tag{SE.1}
\]

For normalization, u below is the dimensionless tangent vector
whose physical displacement is gu. Thus
\(g^{-2}[S(U(gu))-S(U0)]=\frac12\langle u,Hu\rangle+O(g)\).
The matrix H in SE.1 is the physical Hessian, and the factors g²
from the displacement and g^{-2} from the action cancel. The
readout derivative A acts on this normalized u; its output z is
the relative readout angle divided by g. No additional g^{-2}
is missing from SE.2.

The source variational minimum is nondegenerate on this quotient.
The local positivity in the freed current core is the one proved in
LFR II (1.7)–(1.9); the remaining constrained ordinary modes have their
original positive fluctuation forms. Equivalently one may first work
on the finite quotient with the null gauge directions removed and
then use the source positive decomposition below.

Let r* be the promoted **later** raw readout. It consists of variables
determining V1 and the later physical fields, together with the genuine
padded samplers. It excludes the first innovation A0. At the reference
all its physical values are the actual averages/readouts of U0.
After removing redundant entries let A=Dr*(U0). The physical part of
the common quadratic is

\[
 q_*(z)=\inf_{Au=z}\frac12\langle u,Hu\rangle .
 \tag{SE.2}
\]

Add to SE.2 the positive quadratic of each actual independent soft
sampler, once. This convention will be understood in what follows.
The variables z are relative native angles divided by one common
coupling g=g_k. Changing this normalization to the source g_j is
treated explicitly in Section 5.

Within this native finite operation, PM gives the exact nonlinear
factorization of the original later readouts that the chosen
promotion actually determines. Its derivative is therefore A_i=L_i A. Hence the
quadratic minimum for the original history obeys

\[
 q_i(L_i z)\le q_*(z).
 \tag{SE.3}
\]

This is an inclusion of actual constraint fibers. It does not use
a bound on the Euclidean operator norm of L_i.

## 2. The multiplier term is already in the source Gaussian

The required identification is visible in the primary formula, not
an inference from the flat action. CMP119 printed p.249, (1.16), says

\[
 \langle A,\Delta_1 A\rangle
 =\langle A,\Delta A\rangle
   -2\langle h C^{(2)}(A),J_1\rangle+\mathcal G^{(2)}(A).
 \tag{SE.4}
\]

Here C^(2) is the quadratic part of the nonlinear averaging-constraint
correction, J1 is the actual Wilson force, and G^(2) is the genuine
inserted gauge quadratic. The subsequent free-coordinate elimination
is the source map C with QCA=0, giving the precision C*Δ1C in (1.15).
The use of the same letter C in these source expressions should not
confuse the nonlinear correction with the linear free-coordinate map.

To verify SE.4 directly, parametrize the exact constraint fiber by

\[
 U(a)=\exp i\{Ca-hC^{(2)}(Ca)+O(a^3)\}\,U_1 .
\]

The linear Wilson term vanishes for Ca in the tangent of the fixed
average fiber. In the quadratic term the linear force applied to the
second derivative of the parametrization contributes precisely
the second term of SE.4. This is the coordinate expression of
S''−λΦ'', rather than S'' alone. Expanding the source gauge insertion
adds the last term. Haar and exceptional-bond determinants are
measure/action factors; they are not part of this leading physical
quadratic.

CMP119 (3.10) chooses the next field as the actual minimum of the
preceding constrained Wilson functional. The text preceding (3.15)
then applies exactly the same constraint linearization and quadratic
expansion on that mixed determining set. It explicitly says that the
operators are the corresponding mixed operators. Therefore SE.4
identifies every ordinary leading precision with the relevant
restriction Hessian, including its actual multiplier and gauge term.

At the common reference, adding any finer readout with its value
chosen from U0 does not change the minimizing field. On the terminal
manifold S is already critical, so the new readout multipliers there
are zero. The Hessian of each subsequent minimizing value is thus
the minimum of the same H subject to its linear readout. This is the
nonlinear constrained-envelope argument NE.7–NE.9, applied to the
actual source minima.

## 3. Every complete Gaussian elimination is a Schur elimination

For one ordinary step write the restriction Hessian in its actual
linearized free and retained coordinates as

\[
 \frac12
 \begin{pmatrix}x\\y\end{pmatrix}^{T}
 \begin{pmatrix}K&B\\B^T&D\end{pmatrix}
 \begin{pmatrix}x\\y\end{pmatrix}
 =
 \frac12(x+K^{-1}By)^T K(x+K^{-1}By)
 +\frac12 y^T(D-B^TK^{-1}B)y .
 \tag{SE.5}
\]

The source conditional integral CMP119 (1.26) produces exactly the
second term in SE.5, together with its Gaussian determinant and the
complete conditional cutoff/interaction integral. The retained
quadratic (1.29) has this Schur form. The general-step (3.23)–(3.25)
and the annular formula LFR I (1.60) use the same operation; the
latter displays both the A and B Gaussian forms.

The cutoff completion does not alter the algebraic Schur identity.
It remains an additional factor in the measure. In particular an
untruncated marginal precision is not the Hessian of the logarithm
of the cutoff marginal. No derivative estimate for that logarithm
is needed here.

Restoring a conditional integral restores both terms of SE.5 and
removes the same completed integral from the old action. Repeated
Schur minimizations are independent of their order, because they
are successive infima over the same Cartesian linear fiber. Thus
restoring any finite union of the actual lists, with its exact
terminal constraints, gives the simultaneous minimum over the
remaining unexposed modes.

The component convention in CMP119 (2.21) assigns off-diagonal
Schur terms between different old components to B. Those terms
must be restored to the common quadratic. If components are merged
in the auxiliary list, use their joint Schur form. For separated
components one can instead retain the proved exponentially small
difference on the actual cutoff. Deleting the terms without either
operation is not allowed.

Consequently the second-order part of the complete restored
Wilson-plus-gauge energy at U0 is exactly

\[
 \widehat E_*^{(2)}(z)=q_*(z).
 \tag{SE.6}
\]

The equality is for the chosen independent later readout and the
actual soft samplers. It holds for the mixed source operators; no
flat or translation-invariant covariance has been substituted.

### The first canceled innovation is absent

In the Ω1-full branch all later readouts factor through the full V1.
The first fluctuation A0 has zero first coarse average and remains
only in the first factor b_s and its first Schur form E0,*.
For SE.2, minimize over that innovation before making the later
readout, or equivalently start with the constrained Wilson minimum
as a functional of V1. These two descriptions have the same
quadratic by SE.5. Thus SE.6 does not restore a first rare energy
that ER has already canceled.

Additional first modes exposed to compare the two first factors
are treated in precisely this way. Their determinants/completion
remain in b_s. They are not extra positive terms in q* or E*.

## 4. Native Taylor bounds on the admitted finite chart

Here is the quantitative scope needed for the nonlinear comparison.
The restored list has D native cells/independent coordinates, with
N≤R, and the fixed enlargement/collars described in PM and ER.
Its original maps and minimum problems lie in their source regular
domains. After the terminal-preserving change of variables its
physical relative angles and normalized soft coordinates are
bounded by

\[
 |x|_\infty\le g P_*,
 \qquad P_*\le \operatorname{poly}(R,P_0,P_1).
 \tag{SE.7}
\]

All variable later inputs, including restored ordinary entries,
are supported in a declared region T inside Y with the unchanged
source buffer to the support of the outer cutoff derivative.
More precisely their current-scale distance from that derivative
and from the outer localization boundary is at least cMR after
the fixed or logarithmic collar enlargement. Inputs outside T
are held fixed in the reference comparison. This is satisfied
by the proposed core restoration and its O(M log R) current
enlargement when the original Y collar has width of order MR.
It is an actual support condition. Restoring modes near the
boundary of Y would not satisfy it and is not covered by SE.10.

TQ imposes the exact terminal constraint; its graph correction has
polynomial derivatives. WA and the mixed variational theorem give
polynomial reciprocal radii and fixed-order derivative bounds for
the finite readout/minimum primitives. The branch joining U0 to
these small relative data consequently remains in the primitive
variational tube when g is sufficiently small. It need not remain
inside every original hard selector: those selectors are not being
analytically continued or differentiated in this Taylor argument.

The relevant Wilson-action estimate counts native cells, not all
microscopic plaquettes. For a native cell of size h and microscopic
mesh η, the source mixed minimum and its fixed-order variations
have plaquette-size factors η²/h². The quadratic action therefore
has the cancellation

\[
 (h/\eta)^4(\eta^2/h^2)^2=1
 \quad(d=4).
 \tag{SE.8}
\]

The same counting applies to the third variation: one second
variation of the plaquette and one first variation both retain
η²/h². The analytic variational estimates bound their coefficients
by a fixed polynomial in the finite native data norm. Sum over the
declared D cells and the at most N layers. There are therefore fixed
integers a,b, independent of depth and coupling, for which the
cubic remainder of each fully restored leading Wilson/gauge
expression, after division by g², is bounded by

\[
 Cg(1+D+N)^a(1+P_*)^b .
 \tag{SE.9}
\]

This is the same scale count made explicitly in LFR II printed
p.361, (1.20): the source bound contains the number of native
variables, a power of R, N and the third power of the relative
angle, with no L^{cN} factor. A finite union of admitted components
changes its native count, not its scale cancellation. Ordinary
source remainders in CMP119 (1.15), (3.15) have order at least
three after SE.4 and obey the corresponding native estimate.
The source relocalizations (1.22), (3.18) contribute their stated
exponential collar remainder.
The native cover also includes the current-size cells carrying
the decaying outer tails of the mixed minimum. They are summed
with the actual Prop.9 exponential factor. Counting only the
smallest inner cells while omitting these tail cells would not
justify SE.8–SE.10.

There is no claim in SE.9 about third derivatives of an integrated
hard-cutoff completion or about an arbitrary inherited B term.
Those factors stay in the exact nonenergy action used by ER.

## 5. From the unlocalized leading energy to the actual positive Q+S

Before the classical cancellation, keep the complete ordinary
leading forms and the actual Wilson minimizing value. Subtract
only the common retained reference value. On the exact terminal
manifold its linear term is zero by the true variational equation.
Sections 1–4 give its expansion as q* plus the remainder SE.9.

For a primitive whose actual background uses exterior data beyond
the local Y problem, first use the source localized comparison
around U0. Its inputs differ only beyond the unchanged buffer.
The Prop.9 localization estimate (190), used in LFR II (1.16),
(1.22) and (1.26), gives the exponentially small error below.
On the common localized reference, all nested minima selected at
their U0 readouts coincide by uniqueness. This is why SE.6 uses
one H rather than unrelated backgrounds.
The support condition following SE.7 also ensures that the
variation of the unlocalized Wilson energy omitted by the
outer ζ0 cutoff has this same tail estimate. Without that
condition a varying boundary mode could have an order-one
energy outside supp ζ0.

Now perform the actual source classical rearrangement. The
identities (1.20)–(1.32) split the Wilson action into the retained
reference constant, the nonnegative outer gradient form Q, the
inner Wilson action, and controlled remainders. The force term is
treated by (1.29) and (1.4), not set to zero off shell. Equations
(1.46)–(1.48) remove the reference A0 from the inner field, leaving
the real positive S used in ER.3. The source bound (1.47) shows
that this removal costs a polynomial times L^{-N}. It does not
erase the first fluctuation A0 from its separate first factor.

For restored inputs in Y outside Λ the order of this force
argument matters. The original sufficient condition "B is
supported in Λ" is no longer available. First impose the exact
terminal constraints by TQ and take the first variation on that
manifold. Its global linear term against the true U0 force is
zero. Only then insert the ζ cutoffs. The remaining terms are
the cutoff commutators/localization tails of a variation with
all inputs in T; their outer contribution is small by the
stated T-to-boundary gap. The inner contribution uses the same
current-regular reference scale factor L^{-N} as (1.29).
Merely declaring a restored raw B outside Λ to be tangent
would not justify this cancellation.

With finitely many restored inner components, sum the same local
cutoff identities over the disjoint component collars. The source
mixed variational estimates are for arbitrary admitted determining
sets. The number of components is bounded by the counted native
geometry. In particular the force equation with the same fixed
terminal constraints is unchanged.

For a fixed source M and the prescribed N=R, the combined value
remainder is bounded by

\[
 \delta_* \le
 C(1+D+N+P_*)^b
 \{g+\varepsilon_{\max}+e^{-cMR}+L^{-N}\}=o(1).
 \tag{SE.10}
\]

Here ε_max is the admitted weak-coupling curvature ceiling, itself
g times a fixed logarithmic polynomial in this window. An extra
fixed power of R or of a source logarithm is included in b.
The L^{-4N} reference inner action in (1.31) is smaller than this
bound. The source coupling-profile correction in (1.37), and
its printed p.366 estimate, is likewise g² times a fixed
logarithmic polynomial. Exponentially separated component Schur
terms and the small relocalization maps are included in SE.10
when they were not restored exactly.

The running couplings do not create a product of fixed constants.
Their source recursion changes g_j^{-2} by a bounded amount per
step, with the spatial cutoff coefficient between zero and one.
Thus over this N-step window

\[
 \omega=\sup_j|g_k^2g_j^{-2}-1|\le CNg_k^2=o(1).
 \tag{SE.11}
\]

One can also keep this displayed supremum until the recursion is
applied. Replacing the common coupling in any positive ordinary
form or soft sampler by its actual g_j multiplies that form by
a number between 1−ω and 1+ω, in the same physical-angle
coordinates. The positive inner Wilson term has the same
pointwise comparison with its positive spatial profile. The
retained reference constant and the small profile remainder
have already been handled by the exact cancellation above.

It follows that the actual restored positive energy in ER.3,
with every required Schur cross term retained, satisfies

\[
 \boxed{\qquad
 E_*(z)\ge(1-\omega)\,q_*(z)-\delta_* .
 \qquad}
 \tag{SE.12}
\]

For sufficiently weak coupling the coefficient is at least a
fixed positive constant. The proof requires the admitted finite
source chart and buffer in SE.7, not a conjectured energy bound
for a general history. All source determinants/coarea and
completion factors remain in ER's exact measure and nonenergy
ledger. SE.12 does not declare them constant.
The same value estimates and the upper coupling comparison
also give

\[
 E_*(z)\le(1+\omega)\,q_*(z)+\delta_*,
 \tag{SE.12a}
\]

after increasing the common remainder constant. This bilateral
comparison is useful for transferring the source's already
pointwise test estimate without inferring a separate derivative
bound for an integrated completion.

## 6. Consequence for the sharp original test inequality

Suppose an original t test, linearized in its own source chart at
the same reference, has the source estimate

\[
 |T_t y|^2\le C R^9 q_t(y).
 \tag{SE.13}
\]

Then the exact readout factorization and SE.3 give

\[
 |T_t L_t z|^2\le C R^9 q_*(z)
                   \le C R^9\{E_*(z)+\delta_*\}.
 \tag{SE.14}
\]

No norm of L_t and no extra power of D enters SE.14.
The t readout here must be one of the readouts literally
determined by this native finite operation. A test of an
alternative fully restored physical history is not included
until its exact fiber/readout identification has been supplied.

For the preparatory χ′ test this is the linear content of the
original LFR II (1.77)–(1.78) proof, including its actual gauge
condition and the positive gradient form. The source allows its
inner cutoff ζ1 to be shifted to the test collar. Repeating the
same classical splitting changes the full Q+S representation
only by the controlled remainder SE.10; it does not change the
common minimizing Hessian in SE.6. A test of an actual padded
soft sampler is paid by that sampler's positive block.

There is a precision in deriving the homogeneous estimate
SE.13. The printed (1.77) has an additive error after the source
has used its cutoff bound on B. One must not differentiate
that final value bound and infer an exact quadratic inequality.
Immediately before (1.77), printed p.382, the source instead
bounds the background correction homogeneously by
\(\|B\|^2 C\varepsilon_k\operatorname{poly}(R)\).
Retain that estimate. On the original finite t geometry the
fixed tree gauge and the source Poincare estimates bound the
native coordinate norm by a fixed polynomial times its flat
complete physical quadratic. Summing the one-bond estimates
adds at most the native rank; the ordinary innovation blocks
have their fixed-L flat gap (IG.7–IG.9). The same leading
variational expansion compares the remaining quadratic
coefficients with their flat coefficients. Thus

\[
 |q_t-q_{t,\mathrm{flat}}|
 \le C\varepsilon_k\operatorname{poly}(R,D)\,
                         q_{t,\mathrm{flat}} .
 \tag{SE.13a}
\]

The small coefficient can be made less than 1/2, because
ε_k is g times a fixed logarithmic polynomial. This
polynomial loss is used only to absorb the background
perturbation; it does not multiply the final test exponent.
The flat source bound (1.77)–(1.78) therefore gives SE.13
with at most a fixed factor two. The inner axial part of
the χ′ proof is controlled by its inner Wilson quadratic
and its same fixed tree gauge. No such comparison is
asserted for a completed nonlinear-action Hessian.

An application to a nonlinear failed test must additionally use
its actual reference offset and Taylor remainder. WA supplies
polynomial fixed-order bounds for a fixed number of primitive
readout/minimum operations; multiplying by g makes those
remainders o(1) on SE.7. This is not a substitute for listing
which original tests are being evaluated or for proving their
required reference margins. Once the actual tested quantity has
size at least cP1 after those errors, SE.14 yields

\[
 E_*\ge cP_1^2/R^9-o(1).
 \tag{SE.15}
\]

### A direct transfer for the actual preparatory χ′ failure

The bilateral value comparison also gives a direct proof
for this test. Let the t readout be one literally determined
by the admitted native finite operation, and suppose the
earlier t preparation tests hold. Evaluate its actual
variables by the original source readout and gauge maps.
LFR II printed pp.381–383 considers exactly a bond with
\(|B'_t(b)|\ge\delta'_k\). On the inner axial part it uses
the positive inner Wilson action; on the remaining part
it uses (1.77) and (1.78), with the permitted shifted
inner cutoff. Its pointwise conclusion, before integration,
is

\[
 E_t(r_t(z))\ge cP_1^2/R^9-o(1).
 \tag{SE.16}
\]

E_t is the complete positive later energy for that source
representation, with its ordinary positive forms added.
The shifted cutoff changes the full value representation
only by the controlled source remainder. The source
reference terms, including the actual inner axial Vo
term, remain in the o(1); they are not assigned zero.

The exact finite readout has, in normalized coordinates,

\[
 r_t(z)=L_tz+
         g\,O\!\left(\operatorname{poly}(D,N,P_*)\right).
 \tag{SE.17}
\]

WA and TQ give SE.17 for its fixed number of primitive
maps. The native second-derivative estimate in Section 4
bounds the matrix of q_t by a fixed polynomial. Replacing
r_t(z) by L_tz in that quadratic therefore costs o(1).
The upper comparison SE.12a for the t representation
and the exact fiber inequality SE.3 imply

\[
 E_t(r_t(z))
 \le Cq_t(L_tz)+o(1)
 \le Cq_*(z)+o(1)
 \le C E_*(z)+o(1).
 \tag{SE.18}
\]

Equations SE.16–SE.18 prove SE.15 for the actual χ′
failure with the original exponent 9. They need no
derivative of a hard-cutoff completion. They do need
the exact native t-readout identification and the
earlier t preparation hypotheses just stated; neither
is silently extended to an arbitrary unwound physical
completion.

Other ordinary/preparatory failures require their
own source-test and reference-margin catalog. The
stronger source extractions on pp.380–381 alone
do not identify those pullbacks on a new common
physical fiber.

Combining SE.15 with ER.11 gives the intended relative failure
bound using the original exponent 9. Far unexposed ordinary
cutoffs still require their relative completion comparison.
Neither SE.12 nor Schur associativity supplies that comparison.

## Source analysis record

- CMP119 printed pp.249–250, (1.14)–(1.16): exact multiplier
  correction and genuine gauge quadratic; (1.26), (1.29):
  untruncated Schur completion with full cutoff integral.
- CMP119 (2.21): component cross terms move to B; (3.10),
  (3.15), (3.23)–(3.25): actual mixed minimum and general
  ordinary normal form.
- LFR I printed pp.188–189, (1.60)–(1.62): complete A/B
  annular integration.
- LFR II (1.3)–(1.9), (1.16)–(1.37), (1.46)–(1.48):
  actual partial-core criticality, local gap, force cancellation,
  scale-counted Taylor errors and positive Q+S representation.
- LFR II printed pp.382–383, (1.77)–(1.78): original test
  exponent and the fixed gauge used to obtain it.
- PM, TQ, VG and WA: exact later readouts, terminal coarea,
  terminal-preserving finite chart and quantitative native
  primitive bounds.

Scope: fixed first-reset admitted finite restoration, with no
pre-first-step inherited history. Full M04 and the microscopic
scalar/current carrier estimates are not concluded here.
