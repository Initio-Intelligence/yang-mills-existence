# A common Gaussian reference transfers nonlinear quiet-mask comparisons

The theorem below is a finite-rank comparison theorem. Its hypotheses
are a common positive density, quantitative bounds on that density and
on the actual selector maps, and covariance bounds for specified linear
test rows. It does not assume a comparison of the two history masses.
It permits a nonzero reference shift and does not require the logarithmic
density error to tend to zero: an error smaller than the preparation
failure exponent suffices.

The final sections identify its actual h=1 source interface and its
one-step marked consequence. They do not assert that the nonlinear
common refinement has already been constructed. The source uses N=R;
no shorter preparation window is substituted.

## 1. Reference law and exact nonlinear selectors

Let z belong to a finite-dimensional linear quotient with positive
Gaussian precision K. Let C be a centrally symmetric convex set of
positive Gaussian measure. Denote by mu the centered Gaussian restricted
and normalized on C. All linear gauges and common exact retained
constraints have already been imposed on this quotient.

Let rho be the actual common finite measure, on the same space and
support, of the form

\[
 d\rho=c_*e^{W(z)}d\mu(z),\qquad
 \operatorname{osc}_{\mathcal C}W\le D.
 \tag{CE.1}
\]

The constant c_*>0 is arbitrary and remains common to the two masks.
W is real. Only its oscillation matters; no new normalization is chosen
for either history.

For i=s,t let its actual quiet mask be

\[
 H_i=\bigcap_{a\in I_i}
       \{\|T_{i,a}(z)\|_a<r_{i,a}\}.
 \tag{CE.2}
\]

Each target norm has fixed dimension, with uniform norm-equivalence
constants. Assume on the whole comparison domain C that

\[
 T_{i,a}(z)=L_{i,a}z+b_{i,a}+\mathcal R_{i,a}(z),
 \qquad
 \|b_{i,a}\|_a+\sup_{z\in\mathcal C}
                   \|\mathcal R_{i,a}(z)\|_a\le d_{i,a}
                   \le\tfrac14r_{i,a}.
 \tag{CE.3}
\]

The deterministic b term is the allowed nonzero reference displacement.
Thus the theorem is not restricted to test maps vanishing exactly at the
common Gaussian center. A nonzero Gaussian mean may likewise be removed
by changing variables; its contribution to each test is then included
in b. The support C must be centered in those same variables, or its
shift must be included as another selector with the same type of
sandwich. A shifted nonsymmetric base domain is not silently treated as
symmetric.

Define the centered convex masks

\[
 G_i^-:=\bigcap_a\{\|L_{i,a}z\|_a<r_{i,a}-d_{i,a}\},\qquad
 G_i^+:=\bigcap_a\{\|L_{i,a}z\|_a<r_{i,a}+d_{i,a}\}.
 \tag{CE.4}
\]

Then G_i^- subset H_i subset G_i^+ on C. For every scalar component
ell of the row L_i,a assume

\[
 \ell K^{-1}\ell^T\le v_{i,a}.
 \tag{CE.5}
\]

Let

\[
 \eta_i=C_0\sum_{a\in I_i}
       \exp\left[-c_0{(r_{i,a}-d_{i,a})^2\over v_{i,a}}\right],
 \tag{CE.6}
\]

with constants depending only on the fixed target dimension and norms.
A zero row is interpreted directly: its lower centered test is always
satisfied, and it contributes zero to eta.

## 2. The nonlinear two-mask theorem

### Theorem CE.1

If eta_s,eta_t<1, then

\[
 {\rho(H_s\setminus H_t)\over\rho(H_s)}
    \le e^D{\eta_t\over1-\eta_s},\qquad
 {\rho(H_t\setminus H_s)\over\rho(H_t)}
    \le e^D{\eta_s\over1-\eta_t}.
 \tag{CE.7}
\]

Put delta=e^D max(eta_s,eta_t)/(1-max(eta_s,eta_t)). If delta<1,

\[
 \boxed{\quad
 1-\delta\le{\rho(H_s)\over\rho(H_t)}
                   \le(1-\delta)^{-1},\qquad
 \left|\log{\rho(H_s)\over\rho(H_t)}\right|
                   \le-\log(1-\delta).
 \quad}                                             \tag{CE.8}
\]

**Proof.** The intersection C cap G_s^+ is centrally symmetric and
convex. By CR.12 its conditional Gaussian law has the same sub-Gaussian
linear-functional majorant K^{-1} as the unrestricted Gaussian. The
ordinary finite-dimensional norm tail estimate and a union bound give

\[
 \mu((G_t^-)^c\mid G_s^+)\le\eta_t,
 \qquad
 \mu(G_s^-\mid G_s^+)\ge1-\eta_s.
 \tag{CE.9}
\]

All conditionings here also contain C through the definition of mu.
Using the two sandwiches and the density oscillation,

\[
 {\rho(H_s\setminus H_t)\over\rho(H_s)}
 \le e^D{\mu(G_s^+\cap(G_t^-)^c)\over\mu(G_s^-)}
 \le e^D{\eta_t\over1-\eta_s}.
\]

The reverse inequality is identical. Let I=H_s cap H_t. Positivity gives
rho(I)/rho(H_i)>=1-delta for both i. Comparing both masses through the
same rho(I) proves (CE.8). Neither rho(H_i) nor mu(G_i^+) needs a
separate positive lower estimate. QED.

The own-mask comparison in the second part of (CE.9) is important. It
controls the uncertainty strip between G_i^- and G_i^+ by a large-field
tail. No unproved boundary anti-concentration statement for the actual
nonlinear selector is needed.

### Union-only density variant

It is enough to have the common actual density only on
U=H_s union H_t. More precisely, suppose its restrictions to the two
masks agree on their overlap and together define one positive measure
rho_U on U, with

\[
 d\rho_U=c_*e^{W_U}d\mu\quad\hbox{on }U,\qquad
 \operatorname{ess\,osc}_{U}W_U\le D.
 \tag{CE.9a}
\]

Keep the actual sandwiches G_i^- subset H_i subset G_i^+ in C. Choose
any constant in the essential range interval of W_U and set W equal
to it on C minus U, while retaining W_U on U. This is a measurable
extension with the same oscillation. The measure c_*e^W mu agrees
with rho_U on both masks, so Theorem CE.1 applies without changing
either actual history mass. QED.

This argument requires no analytic continuation of an inherited E/B
term off the actual union and no enlargement of its source analytic
exponent. Only a common density and its bounded oscillation on the
actual union are used. The primitive reconstruction and selector
sandwiches still have to be proved on the necessary comparison
domains. Equality of the two density restrictions on their overlap
is substantive: two unrelated completed self densities cannot be
made common by extending their separate logarithms.

The direct sandwich inclusions suffice for this variant. Formula
(CE.3) on the whole convex domain is a convenient sufficient way to
prove them, not an extra necessary premise if a more direct source
admission argument establishes the two inclusions.

### Quantitative source-shaped version

If |I_s|+|I_t|<=C R^5, r_i,a>=c p1(g),
v_i,a<=C R^9, and (CE.3) holds, then

\[
 \delta\le C R^5
      \exp\{D-cp_1(g)^2/R^9\}.                    \tag{CE.10}
\]

Thus D=o(p1^2/R^9) suffices. In particular a verified common absolute
source ledger D=O(D_late), with
D_late=1+R^6 log(1+R)+R^5 log(g^{-1}), is enough under the hierarchy
recorded in LE.18. Proving an o(1) pointwise log-density error would be
stronger than required for this comparison.

A finite pair-dependent reference is allowed, provided it represents
both restrictions of the SAME common measure rho and all constants
are uniform over pairs. There is no need to combine all candidate birth
locations in one coordinate list or to multiply the tail bound by the
number of candidate locations.

The theorem also disintegrates over additional common finite gauge or
orientation choices. Apply it at each fixed auxiliary choice, with
uniform constants, and integrate against the same positive auxiliary
weights. Those weights need not be Gaussian. Choosing different
history-dependent auxiliary weights would require its own comparison.

## 3. Restore the actual rare first factor

At the normalization of LE.4--LE.5 let the complete first sector weight
satisfy, uniformly on the actual later data,

\[
 e^{-\epsilon_b}w_i\le b_i(y)\le e^{\epsilon_b}w_i,
 \qquad
 M_i=\int H_i(y)b_i(y)\,d\rho(y).
 \tag{CE.11}
\]

Here rho includes the same original Z_P(V1). Its conditional first
normalizer is not replaced by a reference probability. For a pair with
w_s=w_t, (CE.8) gives

\[
 e^{-2\epsilon_b}(1-\delta)
 \le{M_s\over M_t}
 \le {e^{2\epsilon_b}\over1-\delta}.
 \tag{CE.12}
\]

The actual RB.15 supplies (CE.11) for the first-step,
globally P/Q-regular R-only sector; exact compatible translations have
equal flat w_i. The remaining source input is the common later
reference of Sections 1--2, not a new first-birth probability estimate.

Suppose J disjoint primitive first events in one complete fresh class
obey the same uniform pair bound. Even if the complete class contains
additional positive histories, its total mass Z_class is at least the
sum of these J masses. Therefore

\[
 {M_i\over Z_{\rm class}}
 \le {e^{2\epsilon_b}\over J(1-\delta)}.
 \tag{CE.13}
\]

This bounds the mass of each specified event. It does not say that the
J events exhaust the entire class or control the marked numerator of
uncompared histories.

## 4. The exact common-refinement requirements in the actual source

For two quiet rectangular chains let their ordinary regular sets be
Omega_j^s and Omega_j^t, with the source free-fluctuation domains
Omega_j^i minus Lambda_j^i. Define the finer candidate

\[
 \Omega_j^{\rm ref}=\Omega_j^s\cap\Omega_j^t,\qquad
 \Lambda_j^{\rm ref}=\Lambda_j^s\cap\Lambda_j^t.
 \tag{CE.14}
\]

Both source sequences use the same j-scale block grid. Their intersection
is a union of those blocks. If each sequence has an r_j collar between
Omega_{j+1} and the complement of Omega_j, so does (CE.14): every point
of the intersection of the two smaller sets has its r_j neighborhood in
both larger sets. Moreover

\[
 \Omega_j^{\rm ref}\setminus\Omega_{j+1}^{\rm ref}
 \subset
 (\Omega_j^s\setminus\Omega_{j+1}^s)
 \cup(\Omega_j^t\setminus\Omega_{j+1}^t).
 \tag{CE.15}
\]

Thus the declared native shell rank is bounded by the sum of the two
ranks, O(R^5) on this first-birth window. The free slots satisfy the
analogous inclusion

\[
 \Omega_j^{\rm ref}\setminus\Lambda_j^{\rm ref}
 \subset(\Omega_j^s\setminus\Lambda_j^s)
       \cup(\Omega_j^t\setminus\Lambda_j^t).
 \tag{CE.15a}
\]

Both lists are needed: retaining only the raw Gamma shell would omit
ordinary R/Q variables. Source bond-interface conventions add a fixed
collar, paid in the same count. If a source geometric convention requires
rectangular hulls for overlapping small holes, take that further
auxiliary refinement and retain its additional coordinates. A connected
union of the two bounded j-scale holes has a rectangular hull of
O(R_j^4) own-scale volume; separated holes stay separate. The bound
remains O(R^5), but the original history masks are still pulled back
unchanged. Rectangularity of every joined
shell is not needed for this set-theoretic conclusion. The variational
problem CMP102 begins with arbitrary admissible nested block domains,
not just one rectangle chain. In contrast, the particular LFR I
preparatory tree construction is stated for a rectangle chain; it must
not be applied to a two-hole refinement without describing its actual
gauge interface.

The remaining required statements are concrete:

1. An exact simultaneous disintegration on (CE.14), or a further bounded
   collar refinement, preserves both chronological averages, both old
   primitive history events, the common retained readout, and every
   Jacobian, normalized gauge weight, first complement factor and E/B/R
   term. The common density is the one multiplying Z_P(V1) in LE.4.
2. In one declared normalized chart its positive quadratic reference
   and the complete residual log density satisfy (CE.1). A verified
   bound D=O(D_late) is sufficient. A separate bound for two self
   operations is not an identity of one common density.
3. Each actual ordinary/preparatory test pulled to this chart satisfies
   (CE.3), with the true gauge convention and source reference shift.
   Taking the same test name in two different charts is insufficient.
4. The specified row covariance bounds (CE.5) and finite test count
   cover the whole difference of the two masks. If remote determining
   maps differ outside the explicit union, their tails require a
   summable estimate; they cannot be declared identical without proof.

The complete one-layer conditional restoration CR.17--CR.21 is one
available analytic input. The arbitrary-domain variational and
propagator results of CMP99/CMP102 are another. Neither has yet been
identified here with the full nonlinear common density in item 2.

## 5. The one-step engineering budget and a localized marked consequence

This paragraph records the precise marked statement that a completed
exchange theorem would imply. It concerns the specified first R-family,
not all older histories.

Let F_x be the actual primitive microscopic scalar, with microscopic
spacing a and coefficient b0. At fixed first coarse field V1, let
F_P,x(V1) be its expectation in the ORIGINAL all-P first law. A local
first-chart conditional-influence estimate of the form RMg.22 gives

\[
 \left|E(F_x\mid E_i,V1)-F_{P,x}(V1)\right|
 \le C b_0a^{-4}P^2
       \sum_{z\in D_i}e^{-\kappa d(x,z)}.
 \tag{CE.16}
\]

The comparison to F_P uses the same enlarged product domain followed by
two local conditionings, E_i and the all-P event; their common outside
law and the conditional-mean derivative proof are unchanged. The fixed
original identity subtraction in F_x cancels in this difference. It is
not changed to a new counterterm.

For a region-spaced translation family, the D_i have bounded overlap in
the first free-coordinate lattice. Hence

\[
 \sum_i\sum_{z\in D_i}e^{-\kappa d(x,z)}\le C.
 \tag{CE.17}
\]

Combining (CE.13), (CE.16), and (CE.17) bounds the contribution of this
family to the normalized birth-defect numerator by

\[
 C b_0a^{-4}\,{P^2\over J}.
 \tag{CE.18}
\]

The actual all-P field F_P,x(V1) remains to be transported and estimated.
Equation (CE.18) does not remove it, and does not estimate contributions
from initial P/Q sectors or other old histories.

At one current step of spacing h, a legitimate incoming deterministic
budget may already contain B_in=(h/a)^4 b0. Then
h^{-4}B_in=b0 a^{-4}; a bound P^2/J<=C is enough for the birth-defect
part of that one-step budget. It is NOT necessary for this particular
statement to obtain a current-density bound h^{-4}b0. Conversely,
(CE.18) supplies no depth-uniform budget: multiplying by h^4/a^4 after
claiming an h-scale estimate would be an error. The broad source family
has J exponential in N=R, so it beats every fixed logarithmic power in
P for this one-step comparison, once the actual common-reference
hypotheses are proved.

The all-order energy-weighted marked estimate is a further statement.
An unweighted first-moment influence bound must not be promoted to all
mixed factorial moments, to independent retained currents, or to full
M-04 without their separate estimates.

## Mathematical sources

- CMP102 pp.277--280, (1)--(14): admissible arbitrary nested block
  domains and the actual constrained variational map.
- CMP119 pp.255--257, (2.2), (2.10)--(2.15): determining sets, exact
  averages, and joined/local determining constructions.
- LFR II pp.381--384, (1.77)--(1.80): preparation coercivity and the
  actual choice N=R in the large-field induction.
- CR.12--CR.16: centered convex-mask concentration proved in
  [conditional restoration](conditional_restoration.md).
- RB.15, LE.4--LE.19: actual first-factor comparison, original common
  first normalizer, and later-only reserve.
- BD.1a--BD.1b: broad same-class families for an admitted sufficiently
  large fixed odd L, with the true R-test and MR-cover distinction.

## 6. A convex-potential alternative to the density-ratio hypothesis

There is a second proved interface for the same selector sandwich. It
requires a Hessian/force estimate instead of (CE.1). It is useful when
the actual density is not symmetric and its pointwise comparison with
a Gaussian would be unnecessarily expensive.

Let rho have density 1_C exp(-V), where C is convex, centrally symmetric,
and contains zero. Assume on C

\[
 \nabla^2V\ge aK,\qquad
 h=-\nabla V(0),\qquad
 h^TK^{-1}h\le D_f,
 \tag{CE.19}
\]

with fixed a>0 and K positive definite. Keep (CE.2)--(CE.5). Let n be
the actual rank of this common chart and put

\[
 \widehat\eta_i
 =C\sum_{a\in I_i}
   \exp\left[C_a(n+D_f)
           -c_a{(r_{i,a}-d_{i,a})^2\over v_{i,a}}\right].
 \tag{CE.20}
\]

Constants depend only on the fixed coercivity and target norms.

### Theorem CE.2

If max(widehat eta_s,widehat eta_t)<1, the conclusion (CE.7) holds with
its e^D factor replaced by one and eta replaced by widehat eta. Therefore
(CE.8) holds with

\[
 \widehat\delta=
 {\max(\widehat\eta_s,\widehat\eta_t)
       \over1-\max(\widehat\eta_s,\widehat\eta_t)}.
 \tag{CE.21}
\]

**Proof.** On C cap G_s^+ the actual potential and its gradient at zero
are unchanged. This is a convex domain containing zero. CR.2 gives,
for a fixed small theta depending only on a,

\[
 \rho(e^{\theta z^TKz}\mid G_s^+)
          \le \exp[C(n+D_f)].
 \tag{CE.22}
\]

For each scalar component ell, Cauchy--Schwarz gives
|ell z|^2<=v_i,a z^TKz. Finite-dimensional norm equivalence therefore
makes failure of a lower centered test imply
z^TKz>=c(r_i,a-d_i,a)^2/v_i,a. Markov's inequality and (CE.22) prove
the two counterparts of (CE.9), with widehat eta. The same sandwich and
intersection argument completes the proof. QED.

For rank n=O(R^5), D_f=O(D_late) and the source row bounds, this gives
widehat delta=o(1). The actual potential need not be even. The force
at the reference is explicitly paid rather than discarded by an
unproved stationarity assertion.

Neither alternative automatically supplies its own source hypotheses.
In particular a lower bound for the quadratic term at one background
is not a Hessian bound for the complete density on the enlarged common
chart. The nonlinear constraint Jacobian, Haar density, source
completion terms and inherited E/B/R derivatives must occur in V when
(CE.19) is verified.
