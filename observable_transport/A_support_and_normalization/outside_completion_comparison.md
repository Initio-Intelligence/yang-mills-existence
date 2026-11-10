# Compare outside cutoff completions without their probabilities

This note supplies a quantitative way to handle hard cutoffs which
remain integrated outside a finite common refinement. Two completed
history densities are not automatically one density on their overlap.
The exact lemma below instead compares their completion factors, with
the original conditional normalizer retained. It applies directly to
one complete regular Wilson chart of RMg. Its multiscale application
requires the source localization and score estimates stated explicitly
in Section 5.

## 1. A product-domain mass comparison

Let z=(z_i) be finitely many real coordinate blocks of dimensions
1<=d_i<=d_*, with fixed homogeneous norms. Put

\[
 C^-:=\prod_i\{\|z_i\|<P_i-\delta_i\},\qquad
 C^+:=\prod_i\{\|z_i\|<P_i+\delta_i\},
 \quad 0\le\delta_i\le P_i/4.
 \tag{OC.1}
\]

Let D(z)>0 be a differentiable density on C^+. Include every smooth
Haar/coarea/constraint factor in D. Suppose its coordinate gradients,
in the dual norms, satisfy

\[
 \sup_{C^+}\|\nabla_i\log D\|_*\le G_i.
 \tag{OC.2}
\]

For I(A)=int_A D(z)dz, define

\[
 \mathcal E:=\sum_i
       \left[2G_i\delta_i+3d_i\delta_i/P_i\right].
 \tag{OC.3}
\]

### Theorem OC.1

If C^- subset A_s,A_t subset C^+, then

\[
 \boxed{\quad
 e^{-\mathcal E}\le {I(A_s)\over I(A_t)}
                         \le e^{\mathcal E}.
 \quad}                                             \tag{OC.4}
\]

This remains true after dividing both integrals by any same conditional
normalizer. No lower bound on the mass of any cutoff event is used.

**Proof.** Define the blockwise radial contraction

\[
 (Tz)_i=\alpha_i z_i,\qquad
 \alpha_i={P_i-\delta_i\over P_i+\delta_i}.
\]

It maps C^+ bijectively onto C^-. Its straight interpolation stays in
C^+, and ||z_i-(Tz)_i||<=2delta_i. Hence

\[
 |\log D(Tz)-\log D(z)|\le2\sum_iG_i\delta_i.
\]

The Jacobian is prod alpha_i^{d_i}. For delta_i/P_i<=1/4,
log[(P_i+delta_i)/(P_i-delta_i)]<=3delta_i/P_i.
Changing variables therefore gives I(C^-)>=exp(-E)I(C^+).
The two domain inclusions prove (OC.4). QED.

The norm need not be Euclidean, and no differentiability of its unit
sphere is needed. The map scales the whole fixed-dimensional block,
so its Lebesgue Jacobian is exactly alpha_i^{d_i}.

### Common intersection and conditional laws

The same argument gives

\[
 {I(A_s\cap A_t)\over I(A_i)}\ge e^{-\mathcal E},
 \qquad i=s,t.                                    \tag{OC.5}
\]

Thus the two normalized restricted laws have a common positive part.
For the total-mass convention of signed variation,

\[
 \|\mu_s-\mu_t\|_{\rm variation}
                \le 2(1-e^{-\mathcal E}).         \tag{OC.6}
\]

Indeed both laws restricted and normalized on their intersection are
the same, and the discarded mass in each is at most 1-e^{-E}.
Equivalently, their common overlap density has total mass at least
e^{-E}; this proves the stated factor two directly. This is a mass
comparison, not a marked transport identity. A mark moved by T must
retain its actual pullback or derivative.

## 2. Slightly different free-coordinate tests

Suppose the first domain is the literal product event
A_s={||z_i||<P_i for every i}. Suppose the second is

\[
 A_t=\{\|\Phi_i(z)\|<P_i\text{ for every }i\},
 \qquad
 \sup_{C^+}\|\Phi_i(z)-z_i\|\le\delta_i.
 \tag{OC.7}
\]

Here the two events are regarded as subsets of the same encompassing
domain C^+. If A_t was originally defined on a larger chart, its
containment in C^+ must also be proved, for example by the analogous
inverse-displacement bound. A bound for Phi only on C^+ does not by
itself rule out additional preimages outside C^+.

With this enclosure, both satisfy the sandwiches in OC.1. Therefore (OC.4)--(OC.6)
apply to the SAME positive physical density without first changing it
to a second chart. The Phi_i may depend on all coordinates; only the
uniform displacement is used for the domain comparison. If one instead
changes integration coordinates by Phi, its exact Jacobian must be
included; it is unnecessary for the proof above.

This form is especially useful when some cutoffs remain integrated out.
At fixed master data u, use their complete conditional density D_u.
If (OC.2),(OC.7) hold uniformly in u, their two completion factors obey

\[
 e^{-\mathcal E}\le
 {C_s(u)\over C_t(u)}\le e^{\mathcal E}.            \tag{OC.8}
\]

The factors C_s and C_t can themselves be arbitrarily small. Equation
(OC.8), not an assertion that they are equal, is what permits one to
retain a chosen common completion in the base measure.

## 3. The exact free-bond source relation

In a common representative at one ordinary source layer, the
nonexceptional independent free entry has the reconstruction

\[
 V_e=e^{i g a^s_e}(U_s)_e
     =e^{i g a^t_e}(U_t)_e.
 \tag{OC.9}
\]

The nonlinear constraint correction acts only on the source exceptional
bonds. Therefore, on the bonds actually used by the free R tests,

\[
 a^t_e={1\over i g}
       \log\bigl(e^{i g a^s_e}(U_s)_e(U_t)_e^{-1}\bigr).
 \tag{OC.10}
\]

On a fixed small physical logarithm tube, the log/exponential maps have
uniform derivatives. If the two reference matrices are compared in
compatible center-fixed gauges, (OC.10) gives

\[
 \|a^t_e-a^s_e\|
       \le C g^{-1}\|(U_s)_e(U_t)_e^{-1}-I\|.
 \tag{OC.11}
\]

The inverse relation interchanges s and t and gives the same estimate.
It therefore proves the outer enclosure as well whenever either true
good coordinate has norm below P in the common small logarithm tube.

Any required frame change must also act on the physical field and the
source gauge variables, preserving the held averages and their exact
weights. Merely choosing different convenient gauges for U_s and U_t
without this common identification would not prove (OC.11) for their
original tests.

For a region on which all relevant R tests are good, their product is
exactly a product of free-coordinate balls. Restore the full footprints
of tests meeting the chosen interface collar. On the remaining outside
coordinates the threshold is P. The approximate Q cutoff is redundant
on a slightly enlarged radius P+delta because its threshold is 2P and
the source local-reference discrepancy is much smaller than P; this is
the argument of CMP119 (3.16)--(3.19), including its starred exceptional-
bond convention. The ordinary finer plaquette and gauge restrictions
which the source removes under these hypotheses must be removed by
that same literal implication. Additional nonproduct hard restrictions
cannot simply be included in the smooth density D.

## 4. An actual complete regular-layer application

For the complete regular Wilson chart verified in RMg, at fixed held
coarse variables and any declared fixed outside free entries,

\[
 D(z)=\exp[-\tfrac12 z^TKz+W(z)]
\]

up to its retained-only positive factor. K has bounded absolute rows,
and W contains the full Wilson, soft-gauge, Haar, coarea and exceptional
constraint-Jacobian terms. On a common encompassing product domain with
coordinate radii at most P_*, RMg gives

\[
 \|\nabla_i\log D\|_*
 \le C P_*+C(gP_*^2+g^2P_*)\le C P_*             \tag{OC.12}
\]

for weak enough coupling in that admitted chart. Conditional linear
forces from the fixed entries are included in the first term; they
are bounded by the same absolute row estimate when those entries have
the stipulated P_* bound.

Thus the actual one-layer completion comparison is

\[
 |\log[C_s(u)/C_t(u)]|
 \le C\sum_i\delta_i(P_*+1/P_i).                 \tag{OC.13}
\]

This applies to the original complete positive density, not an isolated
Gaussian approximation. It does not require a zero-free complex source
disc, a probability-one replacement of a cutoff, or a lower bound on
the cutoff completion. All constants are uniform in the number of
outside coordinates as long as the displayed sum is uniform.

## 5. The multiscale outside-tail criterion

Suppose a two-history refinement has exposed every noncommon hard test
inside its declared native collars. Suppose on the unexposed regular
complement of layer j the remaining differing tests satisfy OC.7, with

\[
 \delta_{j,i}\le A(R,P)\sum_{b\in B_j}
                 e^{-\kappa d_j(i,b)},
 \qquad d_j(i,B_j)\ge c M R_j,
 \tag{OC.14}
\]

where B_j is the actual finite changed determining footprint. Suppose
also that the complete conditional log-density score at that stage is
bounded by a fixed polynomial G(R,P), after all earlier regular
integrations have been completed, with every surviving old factor kept.
Distances and block counts use that layer's own lattice.

Polynomial lattice growth gives, after reducing the fixed decay rate,

\[
 \sum_{j,i}\delta_{j,i}
 \le C A(R,P)\left(\sum_j|B_j|\right)e^{-\kappa' M R}.
 \tag{OC.15}
\]

For N=R and total native changed count O(R^5), OC.13 yields

\[
 \boxed{\quad
 \epsilon_{\rm out}
   \le\operatorname{poly}(R,P) e^{-\kappa' M R}=o(1).
 \quad}                                             \tag{OC.16}
\]

Here R is a common comparable radius on the window. This is a sum of
conditional logarithmic errors. Uniform pointwise conditional
comparisons may be integrated successively, so their relative errors
multiply as exp(sum epsilon_j), not as C^N. This statement is an exact
positive comparison and does not assert probabilistic independence
between layers.

The actual inputs still requiring verification for the general two-list
source application are precise:

1. A common physical identification outside the exposed collar, with
   the original held averages, gauges and coarea factors.
2. The historical-background localization bound OC.14. One promising
   way is to express both minima on the joined determining set, with
   the additional data set to their own actual averages, and use the
   source variational derivative (CMP102 (190)) away from the changed
   native support. The gauge and admission of that comparison must be
   checked. It is not a consequence of a common Omega sequence; in
   fact translated R births change Omega at the next step through
   CMP119 (3.5).
3. A polynomial score bound for the COMPLETE current ordinary
   integrand, including surviving earlier Schur forms and E/B/R terms.
   OC.12 proves this for the original regular first layer. An absolute
   bound for a later action on one set alone is not a derivative bound
   on a needed buffer; native Cauchy/localization is a possible route.
4. Every noncommon nonproduct selector is either explicitly exposed
   or has its own analogous comparison. A history-dependent completed
   hard factor cannot be renamed a common density without this step.

When these hold, choose one completion as the common factor and retain
the other as a multiplicative weight between exp(±epsilon_out). Apply
CE to the remaining explicit finite masks. The full mass comparison
then acquires only the additional exp(±epsilon_out) factor, and the
original first weights are restored by RB as before.

## 6. Why this is distinct from a rank argument

Consider a common density phi(u,z) and two integrated tests
|z-a_su|<P and |z-a_tu|<P. The completed densities in u are generally
phi_U(u)F_s(u) and phi_U(u)F_t(u), with different F_s,F_t, even when
all remaining explicit masks coincide. A finite common readout of u
does not make these densities agree. OC.8 compares the actual F_s/F_t
when their difference is controlled; otherwise z, or an adequate
joint readout, must be restored. This is exactly the distinction kept
in FD.2.

## 7. Logarithmically thicker auxiliary collars

The radial lemma also tolerates a crude exponential-in-depth score,
provided the auxiliary restored collar is enlarged quantitatively.
This is an alternative sufficient criterion, not an assertion that the
source score has already been verified.

Write ell=log(g^{-2}), retain the actual N=R waiting rule, and suppose

\[
 N\le C R,\qquad R\ge c\ell,
 \qquad
 A(R,P)\,[1+G(R,P)]
 \le \exp\{C_0[N\log(2+R)+\ell]\}.
 \tag{OC.17}
\]

The condition R≥c ell follows from a recorded radius exponent r≥1;
it must not be assumed for an unspecified smaller exponent. Include
every changing native determining footprint and every test meeting
its T_j=A R_j log(2+R_j) collar in the exposed list. For a fixed A
larger than a constant depending on C_0 and the source decay rate,
the remaining tail sum in OC.15 gives

\[
 \mathcal E_{\rm far}
 \le \exp[-c_A R\log(2+R)]=o(1).
 \tag{OC.18}
\]

Polynomial incidence counts and fixed logarithmic P factors are
absorbed into the exponent. This is a quantitative consequence of
OC.17; it does not follow merely from finite differentiability.

The enlarged native count in d=4 is at most

\[
 D_{\rm ext}\le C R^5[\log(2+R)]^4.
 \tag{OC.19}
\]

If the source finite-coordinate trial/cancellation ledger charges at
most C[N log(2+R)+ell+log(2+P)] per exposed coordinate, its resulting
logarithmic normalization loss is bounded by

\[
 \mathcal D_{\rm ext}
 \le C\{R^6[\log(2+R)]^5+
          R^5\ell[\log(2+R)]^4\}.
 \tag{OC.20}
\]

Positive Gaussian and Wilson energies must remain positive forms in
this ledger. Bounding each of them by its cutoff P² and charging
D_ext P² instead would be a different, insufficient estimate.

The operational condition for the exchange proof is

\[
 \mathcal D_{\rm ext}=o(H_R),
 \qquad H_R=cR^{-9}p_1(g)^2.
 \tag{OC.21}
\]

For R comparable to ell^r with r≥1, it follows from the explicitly
recorded hierarchy r_0≥r,
2p_1-9r_0>p_0, and p_1<p_0. Indeed these imply p_0>9r_0, so the
power of ell in H_R strictly exceeds 9r, whereas the polynomial
power in (OC.20) is at most 6r. Fixed additional logarithms are paid
by that strict gap. If r_0 has not been identified with a radius
majorant in the particular specified construction, retain (OC.21) as
the operational premise rather than inventing that identification.

These are auxiliary collars only. The original histories, cutoff
thresholds, waiting rule and kernel are unchanged. The source
geometry fact in CG.2 is especially
useful here: for a same-final-core pair, the final prepared Omega
and Z agree, and all varying ordinary domains occur before that
terminal stage. A T_j collar then has current-scale radius
O(M log R), within the common Y of radius O(MR) at weak coupling.
This avoids crossing arbitrary external strong-field components.
That geometry does not by itself verify the score or common-chart
conditions in OC.17.

## 8. Conditional far completion with an energy test

One can use the exact common **full-path** measure without asserting
that the finite near masks are independent of the far variables.
The following elementary consequence isolates what is required.

Let u be the finite exposed coordinates and z all remaining far
coordinates in one common physical chart, with a common positive
density D(u,z). Write the actual two branch masks as
A_i(u,z)H_i(u,z), where A_i is the outside good-product part and H_i
contains the remaining near quiet tests. At every u the two A_i
obey the sandwiches and score bounds of OC.1 with a uniform error
epsilon. Thus their conditional completion integrals and their
intersection satisfy OC.4--OC.5. Let E(u)≥0 be a finite exposed
energy.

Assume there is a threshold H such that, **for every admitted far
path in the encompassing domain**,

\[
 E(u)<H\quad\Longrightarrow\quad
 H_s(u,z)=H_t(u,z)=1.
 \tag{OC.22}
\]

This is a uniform selector implication. It can follow from actual
localized readouts, small center offsets and Taylor bounds; it is
not a consequence of conditioning on the far path alone. Also assume
the exact normalized branch laws obey

\[
 \nu_i(E\ge H)\le\delta_i<1,
 \qquad i=s,t.
 \tag{OC.23}
\]

With M_i the unnormalized branch mass, the exact common intersection
I satisfies

\[
 I\ge e^{-\epsilon}(1-\delta_i)M_i
 \quad(i=s,t),
\]

and hence

\[
 \boxed{\quad
 e^{-\epsilon}(1-\delta_t)
 \le {M_s\over M_t}
 \le {e^{\epsilon}\over1-\delta_s}.
 \quad}
 \tag{OC.24}
\]

To prove the intersection bound, restrict to E(u)<H. Both near
masks are then identically one, for all z. At each such u, OC.5
retains at least e^{-epsilon} of the i-th outside completion in
the common outside intersection. Integrate u and use (OC.23).
There is no conditional probability lower bound for the far product
event, and no assertion that H_i is an exactly finite-coordinate
function on its high-energy part.

A reserve nu_i(exp(theta E))≤exp(D_ext) gives
delta_i≤exp(D_ext-theta H). Thus (OC.18),(OC.21), and a source
proof of OC.22 and that reserve imply a sharp mass comparison.
The first relative R weights can subsequently be restored with RB.
If a near selector sees an arbitrary unbounded old-energy variable
outside u, OC.22 has not been proved and this conclusion cannot be
used. Enlarging the collar only helps when the source supplies a
uniform regular-tail or energy-controlled readout bound.

## Mathematical sources

- CMP119 (1.14)--(1.19), (3.15)--(3.19): independent nonexceptional
  free entries, the exact nonlinear constraint chart, and Q redundancy
  on the R-good region.
- CMP119 (3.5): later Omega depends on the previous Lambda hole even
  when no fresh P/Q test fails.
- RMg.1--RMg.35: complete regular-layer score/Hessian bounds and
  original product support; RB.1: earlier fixed-radius radial
  comparison, extended here to summable coordinatewise widths.
- CMP102 (190): the potential historical-background localization
  input, whose common-gauge use remains explicit in Section 5.
