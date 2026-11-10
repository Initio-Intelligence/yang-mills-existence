# Actual component history influence, spatial tails and retained currents

**Annex AG.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

**H-03 remains open.** This note proves new estimates for an actual part of the
positive source construction: averaging the variables of one fixed selected
component in Balaban's LFR II (1.71)--(1.72). The estimates concern its actual
normalized posterior, including its old histories and its interaction with the
other components. They are not estimates for a newly sampled independent
reference field.

The results are:

1. An exact positive component-posterior representation, with the large
   self-component action retained in its base measure.
2. A quantitative influence bound for changing another component's history,
   obtained directly from the published interaction bound (1.68). It includes
   the conditional denominator.
3. A complete source-jet comparison and a local truncation of that actual
   posterior. The bounds retain a fixed factorial exponent.
4. Native-background-coordinate current bounds for the same component reset,
   including a current bound for its localization error. The admitted radius,
   rather than only the supremum of the action, is displayed.
5. A geometric summation of the actual relative-tree carrier bound for a
   reset restricted to eligible components. It gives a radius of order
   \(MR_kh\), followed by exponential tails, uniformly over the remaining
   fixed eligible geometry. The reset need not average a giant component.

The eligible-component spatial bound is uniform over the admitted remaining
geometries in the source coordinate description. The native analytic bounds
are uniform over the values admitted by their stated charts. They do not
prove the full retained-coordinate carrier/current bound of the
H-03 statement. The exact outstanding inequality is stated in Section 8.

The primary source input is source-free;
its small-coupling and geometric hypotheses are retained. Identifying
the Wilson trajectory with those hypotheses is not discharged here.

### 1. Primary source formulas and the particular reset

The following published formulas specify the support and the component operations.


| Source | Exact input and its scope |
|---|---|
| CMP 109 (1987), p.257, geometric definitions before (0.24), article | A localization domain is a finite face-connected union of \(M\)-cubes. The neighborhood operation is the fixed cube enlargement.  |
| LFR I, CMP 122 (1989), pp.177 and 201, conditions (i)--(ii), (1.100)--(1.102) | The selected components fit in cubes of side \(100MR_k\); the actual local replacement uses its localized reference density and preserves the integral. Components outside the selected union are not replaced. |
| LFR II, CMP 122 (1989), pp.376--377, (1.67)--(1.69) | The cross-component functions \(V(Y)\) have a uniform analytic bound in a specified relative tree size. A function whose carrier is a whole component has a different, generally nonsmall, bound. |
| LFR II, pp.378--379, (1.71)--(1.72) | The component integrations and old-history sums factor over fixed components. Each component operation is localized in that component. The cross action depends on the old histories of components contained in its carrier, and the old-history sum acts on this action too. |
| LFR II, pp.379--380, (1.73)--(1.75) | The real component operation is positive. Its analytic deformation is a small exponential tilt. Its normalized analytic operation obeys the stated supremum bound even when its real unnormalized mass is very small. |
| LFR II, pp.388--389, (1.92)--(1.97) | The unmarked expansion pays a component-volume cost with the small unnormalized component mass. This payment is not available after conditioning on the component. |
| LFR II, pp.391--392, (1.103)--(1.104) | The normalized component operations can be integrated out. The remaining domains are fixed in that expansion; the source explicitly does not require their own tree-decay factors for that unmarked convergence statement. |

The source notation for the component operation is denoted here by
\(\mathsf T_i=\mathsf T'_k(X_i)\). The index \(i\) fixes a component, not an
individual microscopic plaquette.

Fix a term of the positive source representation with its outer component
geometry, gauge choices that remain external, and retained field data \(v\).
Only sectors with positive real normalizers are used. Let \(\eta_i\) comprise
**all** variables still integrated or summed by \(\mathsf T_i\): its old local
histories, continuous integration variables, and local graph choices. These
variables can be placed in the common padded disjoint union of sectors already
specified in H-01. The operation defines a finite positive measure
\[
 \mathsf T_iF=\int F(\eta_i)\,M_i(d\eta_i;v),\qquad
 m_i(v)=M_i(1;v)>0,\qquad
 \nu_i(d\eta_i;v)=m_i(v)^{-1}M_i(d\eta_i;v).
 \tag{HL.1}
\]

The self-component expression \(V(X_i^{\sim})\), whose bound is (1.69), is inside
\(M_i\). It has not been omitted or estimated as a small perturbation. The same
is true of the old characteristic functions, local reference factors,
integration Jacobians and graph averages present in (1.71).

Let \(\mathscr Y\) be the finite family of the remaining carriers in (1.72).
Write \(J(Y)\) for the components whose variables occur in \(V_Y\). A carrier
may involve one component and retained fields outside it; it need not involve
two distinct components. The source locality statement gives
\[
 V_Y=V_Y\bigl(v|_Y,(\eta_j)_{j\in J(Y)}\bigr).
 \tag{HL.2}
\]
Here locality is in the source variables appearing in that formula. In
particular, replacing a minimizing background by a storage label is not a
proof that its footprint in the actual retained-link coordinates equals \(Y\).

#### Theorem HL.1 -- the fixed-geometry posterior

On this fixed positive sector, the conditional law of the variables
\(\eta=(\eta_i)\), given \(v\), is
\[
 \pi_v(d\eta)=
 \frac{\exp\{\sum_{Y\in\mathscr Y}V_Y(v,\eta)\}
             \prod_i\nu_i(d\eta_i;v)}
      {\displaystyle
       \int\exp\{\sum_{Y\in\mathscr Y}V_Y(v,\eta)\}
             \prod_i\nu_i(d\eta_i;v)}.
 \tag{HL.3}
\]
In particular, conditioning on all components other than \(i\) gives
\[
 \pi_i(d\eta_i\mid\zeta)=
 \frac{e^{H_i(\eta_i;\zeta)}\nu_i(d\eta_i;v)}
      {\nu_i(e^{H_i(\cdot;\zeta)})},\qquad
 H_i=\sum_{Y:\,i\in J(Y)}V_Y ,
 \tag{HL.4}
\]
where \(\zeta\) denotes the retained data and the other component variables.

**Proof.** On a fixed term of (1.72), the operations (1.71) are integrations
against the product of the positive measures \(M_i\). The only remaining
dependence on their integration variables is the last exponential in (1.72);
the source expressly says that the local history sums act on it. Thus the
joint density before normalization is precisely the numerator of (HL.3)
with \(M_i\) in place of \(\nu_i\). The factor \(\prod_i m_i(v)\) cancels
between its numerator and denominator. The terms of its exponent independent
of \(\eta_i\) cancel on forming the conditional law, giving (HL.4).
No cancellation has been made in a sum over different outer geometries.
\(\square\)

The reset considered below averages the complete incoming source jet using
(HL.4). If a new component label is retained, it can subsequently be sampled
from the chosen source-independent replacement law; the marked quotient is
still the conditional expectation under the old posterior (HL.4). In
particular, this old posterior is not replaced by that new sampling law.

All incoming marks in this note are the exact marks already transported to
the positive representation (1.72). If earlier gauge averaging or an exact
change of variables has occurred, its projected mark is used. Reinserting an
original microscopic observable into this representation without its
transport would not be Theorem HL.1.

The product-base representation is a scoped primary input from
(1.71)--(1.72), not a consequence of the small cross-interaction bound
alone. We apply it only to geometries admitted by that source
factorization. If a different proposed geometry has a nonsmall self
interaction coupling several claimed component blocks, that interaction
must be included in their common base, or that cluster must be left live.
It cannot be discarded or charged to (1.68). The abstract carrier count
in Section 6 also covers merging collars, but does not extend the
source's posterior factorization to such a different geometry.

### 2. A direct influence bound from the actual interaction

Set
\[
 b_Y=\alpha\exp\{-\bar\kappa\,d_{k,Z}(Y)\},\qquad
 \bar\kappa=(1+2\beta)\kappa ,
 \tag{HL.5}
\]
for the non-self carriers of (1.68). The published estimate is
\(\sup|V_Y|\le b_Y\), on its stated domain and uniformly in the variables
still integrated by the component operations. The real slice suffices for
this section.

The relative size in (1.67) is the length, divided by \(M\), of a shortest
tree contained in \(Y\) meeting the specified \(M\)-cubes of \(Y\setminus Z\).
The required terminals do not include arbitrary insertion points inside
components of \(Z\). This omission, rather than an assumed identification
with an ordinary physical metric, is used in the argument below.

We use
\(\|P-Q\|_{\mathrm{TV}}=\sup_E|P(E)-Q(E)|\) for two probability measures.
For a finite complex measure, the distinct notation
\(\|\mu\|_{\mathrm{var}}=|\mu|(\Omega)
 =\sup_{\|F\|_\infty\le1}|\mu(F)|\) is its variation norm.
A positive probability has variation norm one, and
\(\|P-Q\|_{\mathrm{var}}=2\|P-Q\|_{\mathrm{TV}}\).

#### Lemma HL.2 -- a normalized exponential tilt

Let \(P\) be a probability measure and
\(Q=e^D P/P(e^D)\), with \(D\) real and of finite essential oscillation
\(\omega=\operatorname{ess\,sup}D-\operatorname{ess\,inf}D\). Then
\[
 \|P-Q\|_{\mathrm{TV}}
 \le \tanh(\omega/4).
 \tag{HL.6}
\]

**Proof.** After subtracting the essential infimum, put
\(T=e^D\in[1,R]\), \(R=e^\omega\), and \(a=P(T)\). If \(R=1\) the result is
immediate. The chord bound for the convex function \((T-a)_+\) gives
\[
 \|P-Q\|_{\mathrm{TV}}
 =a^{-1}P[(T-a)_+]
 \le\frac{(R-a)(a-1)}{a(R-1)} .
 \tag{HL.7}
\]
The right side is largest at \(a=\sqrt R\), where it is
\((\sqrt R-1)/(\sqrt R+1)=\tanh(\omega/4)\). This includes the conditional
normalizer exactly. \(\square\)

#### Theorem HL.3 -- one-component posterior influence

Suppose two external data sets \(\zeta,\zeta'\) keep the geometry and the
component base \(\nu_i\) fixed. Let \(\mathscr A_i(\zeta,\zeta')\) be the
carriers in \(H_i\) that can change under this replacement. Then
\[
 \|\pi_i(\cdot\mid\zeta')-\pi_i(\cdot\mid\zeta)\|_{\mathrm{TV}}
 \le
 \tanh\left(\sum_{Y\in\mathscr A_i(\zeta,\zeta')}b_Y\right).
 \tag{HL.8}
\]
For replacement of only another fixed component history \(\eta_j\), with
native background data held fixed, one obtains the actual influence
coefficient bound
\[
 c_{ij}\le
 \tanh\left[
   \alpha\sum_{Y:\,i,j\in J(Y)}
      e^{-\bar\kappa d_{k,Z}(Y)}
       \right],\qquad i\ne j .
 \tag{HL.9}
\]
The supremum defining \(c_{ij}\) is over all admissible values in those fixed
sectors; the right side does not contain the conditional masses \(m_i(v)\).

**Proof.** Relative to the law at \(\zeta\), the law at \(\zeta'\) is the
normalized exponential tilt with
\[
 D(\eta_i)=H_i(\eta_i;\zeta')-H_i(\eta_i;\zeta).
 \tag{HL.10}
\]
All unaffected terms cancel. Each affected summand has supremum at most
\(2b_Y\), and hence oscillation at most \(4b_Y\). Apply Lemma HL.2.
For a change of \(\eta_j\), (HL.2) limits the affected set to the one in
(HL.9). \(\square\)

This is an estimate for the actual conditional posterior. A hypothetical
posterior mixing certificate is not a premise of (HL.8). However, its
numerical carrier sum is still geometry dependent. It is not, by itself, an
estimate uniform in physical separation for every allowed remaining history.

### 3. Entire finite jets, rather than only single marks

For a finite label set \(I\), let
\[
 \Psi(t)=
 \sum_{\varnothing\ne J\subseteq I}t_J A_J
 \tag{HL.11}
\]
be its square-free logarithmic source jet; \(A_J\) is the derivative
coefficient, so \(t_J=\prod_{j\in J}t_j\) has no additional factorial.
For repetitions one first distinguishes the labels and then identifies the
arguments. All formulas take place in the finite truncated source algebra.

Under a probability measure \(P\), the reset coefficient is
\[
 A_I^P=\left.\partial_I\log P(e^\Psi)\right|_{t=0}
 =\sum_{\mathcal P\in\Pi(I)}
   \kappa_P(A_B:B\in\mathcal P).
 \tag{HL.12}
\]
Every incoming higher vertex is present in (HL.12).

#### Lemma HL.4 -- bounded full jets under a change of posterior

Suppose \(P,Q\) are two probability measures on a common input space and
\(\delta=\|P-Q\|_{\mathrm{TV}}\). Suppose, for every nonempty \(J\subseteq I\),
\[
 \|A_J\|_\infty
 \le C^{d+1}(d!)^{p_0}b^d,\qquad
 d=|J|,\quad C\ge1,\quad p_0\ge1 .
 \tag{HL.13}
\]
Then, for \(m=|I|\),
\[
 |A_I^P-A_I^Q|
 \le \delta\,[C(1+2C)]^m(m!)^{p_0}b^m .
 \tag{HL.14}
\]

**Proof.** For bounded \(F_1,\ldots,F_k\), the moment of a product changes by
at most \(2\delta\prod_\ell\|F_\ell\|_\infty\). Telescoping a product of
moments in the cumulant partition formula therefore gives
\[
 |\kappa_P(F_1,\ldots,F_k)-\kappa_Q(F_1,\ldots,F_k)|
 \le 2\delta
       \sum_{\pi\in\Pi_k}|\pi|!\prod_\ell\|F_\ell\|_\infty
 \le 2^k\delta\,k!\prod_\ell\|F_\ell\|_\infty.
 \tag{HL.15}
\]
The last count uses the injection of ordered set partitions into
permutations with cuts.

For partitions of the \(m\) source labels into \(k\) blocks, ordering the
blocks and then their sizes gives
\[
 k!\sum_{\substack{\mathcal P\in\Pi(I)\\|\mathcal P|=k}}
       \prod_{B\in\mathcal P}(|B|!)^{p_0}
 =
 m!\sum_{\substack{d_1+\cdots+d_k=m\\d_\ell\ge1}}
       \prod_{\ell=1}^k(d_\ell!)^{p_0-1}
 \le (m!)^{p_0}\binom{m-1}{k-1}.
 \tag{HL.16}
\]
The remaining sum is
\[
 C^m\sum_{k=1}^m(2C)^k\binom{m-1}{k-1}
 =2C^{m+1}(1+2C)^{m-1}
 \le[C(1+2C)]^m.
 \tag{HL.17}
\]
Combining (HL.12), (HL.15), and (HL.16) proves the result. \(\square\)

Thus the actual coefficient change from a remote component replacement,
with the incoming coefficients unchanged by that replacement, is bounded
by (HL.14) with the right side of (HL.8) for \(\delta\). If the incoming
coefficients themselves change, their direct and previous-current records
must also be transported. This theorem does not discard those records.

The bounded hypothesis is automatic at a single finite compact cutoff for
the exact bounded incoming expressions that admit such a representation,
but the constants can depend badly on that cutoff. It does not establish
the desired current-scale \(h^{-4m}\) budget. The more general actual-law
moment bounds remain useful when a uniform supremum
budget is unavailable; replacing the supremum hypothesis by such bounds
requires the corresponding coupling/Holder estimate.

#### Corollary HL.5 -- actual local truncation of one reset

Fix a source-coordinate region \(E\) containing the source dependence of
the component base (including its stated collar) and the external
dependency footprints of the incoming coefficients under consideration.
Form an auxiliary conditional law by retaining only the
terms of \(H_i\) whose carriers lie in \(E\):
\[
 H_i^E=\sum_{\substack{Y:\,i\in J(Y)\\Y\subseteq E}}V_Y,\qquad
 \pi_i^E=\frac{e^{H_i^E}\nu_i}{\nu_i(e^{H_i^E})},\qquad
 \lambda_i(E)=
 \sum_{\substack{Y:\,i\in J(Y)\\Y\not\subseteq E}}b_Y .
 \tag{HL.18}
\]
Then the exact reset jet obeys
\[
 |A_I^{\pi_i}-A_I^{\pi_i^E}|
 \le [C(1+2C)]^m(m!)^{p_0}b^m
          \tanh\bigl(\lambda_i(E)/2\bigr).
 \tag{HL.19}
\]
The approximating coefficient depends only on the source variables in
\(E\), with their actual dependency footprints retained.

**Proof.** The difference of the exponents in (HL.18) has supremum at most
\(\lambda_i(E)\), hence oscillation at most \(2\lambda_i(E)\). Apply
Lemmas HL.2 and HL.4. Locality follows from (HL.1)--(HL.2), with the stated
assumption about the incoming coefficients. \(\square\)

The auxiliary law in (HL.18) is used only to estimate the unchanged exact
reset. It is not a proposed replacement of the Wilson measure. Nested
regions give an exact finite telescoping carrier decomposition of the
reset coefficient. A useful norm estimate still requires summing its
actual carrier costs; replacing those costs by one would lose H-03.

### 4. The normalized analytic component operation is a source input

The source provides more than real positivity for a fixed component.
LFR II (1.73)--(1.75), printed p.380, explicitly gives
\[
 \left|
   [\mathsf T_i(U,J)1]^{-1}\mathsf T_i(U,J)F
 \right|
 \le e^{3\sup|\sigma_i|}\sup|F|.
 \tag{HL.20}
\]
Here \(\mathsf T_i(U,J)\) is represented by the real positive component
integral at \((U,0)\), multiplied by \(e^{\sigma_i}\). The small complex
variation \(\sigma_i\) is described on p.379, including the variation of
the large self-component term \(V(X_i^{\sim})\).

Equation (HL.20) controls the **normalized old component operation**. Its
normalizer may be very small; its reciprocal is not separately bounded.
This is a different input from the earlier estimate for the freshly
sampled reference density in LFR I (1.100).

The domain in (HL.20) is the domain actually admitted by the source. It does
not assert an entire function of arbitrary retained-link coordinates, or
of variations that change the outer selectors and component geometry.

The following argument includes the cross action \(H_i\), which need not
have been part of the isolated normalized operation (HL.20).

#### Theorem HL.6 -- a quantified analytic tube for the actual posterior

Fix a real source datum and a one-complex-parameter native chart
\(|z|<\rho\) admitted by the source with the geometry and the other
component histories fixed. Suppose its integral representation is the one
used in (HL.20):
\[
 M_i(z;d\eta_i)=e^{\sigma_i(z,\eta_i)}M_i(0;d\eta_i),
 \quad \sigma_i(0,\eta_i)=0,\quad
 \sup_{|z|<\rho,\eta_i}|\sigma_i|\le s_i .
 \tag{HL.21}
\]
The source supplies this representation on a common fixed support in its
admitted native chart. At a real datum with a nonzero current coordinate,
one recenters the source exponent: if its unrecentered form is
\(\sigma_i^{\mathrm{src}}(z)\), the exponent in (HL.21) is
\(\sigma_i^{\mathrm{src}}(z)-\sigma_i^{\mathrm{src}}(0)\).
Thus \(s_i\) can be taken as twice the source supremum bound on that
chart. The real measure at its center is positive. Neither recentering
nor a common support is assumed across a selector or geometry change.
Define the explicit cross-action majorant
\[
 \lambda_i=\sum_{Y:\,i\in J(Y)}b_Y,\qquad
 r_*=\log(3/2),\qquad
 \rho_i=\frac{\rho\,r_*}{s_i+\lambda_i+r_*}.
 \tag{HL.22}
\]
For every \(0\le t\le1\), let
\[
 H_{i,t}=H_i^E+t(H_i-H_i^E)
 \tag{HL.23}
\]
and let \(Q_{i,t,z}\) be the normalized component integral with this
cross action and the base (HL.21). Then throughout \(|z|<\rho_i\) its
normalizer is nonzero, and its complex measure has total variation norm
\[
 \|Q_{i,t,z}\|_{\mathrm{var}}\le3 .
 \tag{HL.24}
\]
The constants are uniform over \(t\), the integrated component variables,
and the remaining variable values admitted by the fixed chart.

**Proof.** At \(z=0\), \(Q_{i,t,0}\) is a real probability measure. Relative
to this measure the complex operation is exactly
\[
 Q_{i,t,z}F=
 \frac{Q_{i,t,0}(e^{\theta_{i,t}(z)}F)}
      {Q_{i,t,0}(e^{\theta_{i,t}(z)})},
 \quad
 \theta_{i,t}(z)=
 \sigma_i(z)+H_{i,t}(z)-H_{i,t}(0).
 \tag{HL.25}
\]
The analytic function \(\sigma_i+H_{i,t}\) has supremum at most
\(s_i+\lambda_i\) on the disc of radius \(\rho\). Its power series and
Cauchy's coefficient bound give
\[
 \sup_{\eta_i}|\theta_{i,t}(z)|
 \le(s_i+\lambda_i)\frac{|z|}{\rho-|z|}
 \le r_*,\qquad |z|\le\rho_i .
 \tag{HL.26}
\]
For any probability measure \(\mu\) and \(|\theta|\le r_*\),
\[
 |\mu(e^\theta)|\ge1-\mu|e^\theta-1|
 \ge2-e^{r_*}=\tfrac12,\qquad
 \mu|e^\theta|\le e^{r_*}=\tfrac32 .
 \tag{HL.27}
\]
Their ratio proves (HL.24). Every small real component mass has already
cancelled in (HL.25). \(\square\)

The radius \(\rho_i\) is an output of the estimate, not a fixed universal
radius. If the actual carrier sum \(\lambda_i\) grows, the derivative
cost grows. If no admitted native chart is available for a proposed
retained-coordinate perturbation, Theorem HL.6 does not apply to it.

### 5. Source-coordinate currents and a current bound for the tail

Assume the incoming coefficients have analytic versions in the chart of
Theorem HL.6 and obey (HL.13) there, with the supremum taken over that
chart and the integrated variables. The argument also applies with
the coefficients frozen at any fixed real datum; that version isolates
the newly generated kernel current from direct input derivatives.

For a complex measure \(Q\) of mass one and variation norm at most \(K\ge1\),
the cumulant partition formula gives
\[
 |\kappa_Q(F_1,\ldots,F_k)|
 \le k!2^{k-1}K^k\prod_{\ell=1}^k\|F_\ell\|_\infty.
 \tag{HL.28}
\]
Indeed, each product of moments has at most \(k\) factors, each costing
at most \(K\). The same ordered-composition calculation as (HL.16) implies
for \(K=3\)
\[
 |A_I^{Q_{i,t,z}}|
 \le B_C^m(m!)^{p_0}b^m,\qquad
 B_C=C(1+6C),\qquad |z|<\rho_i .
 \tag{HL.29}
\]
Consequently Cauchy's formula yields, for \(q\ge0\),
\[
 \left|\left.\frac{d^q}{dz^q}
 A_I^{Q_{i,t,z}}\right|_{z=0}\right|
 \le q!\rho_i^{-q}B_C^m(m!)^{p_0}b^m .
 \tag{HL.30}
\]
For a real segment in the concentric half-disc, the corresponding
first finite-difference bound has \(2/\rho_i\) in place of
\(\rho_i^{-1}\). These bounds include every source order \(m\) with
the same factorial exponent \(p_0\).

#### Theorem HL.7 -- localization of the native kernel currents

Let \(\lambda_i(E)\) be the explicit discarded-carrier majorant in
(HL.18). With the same analytic input budget and the radius (HL.22),
there is \(D_C\), depending only on \(C\), such that
\[
 \sup_{|z|<\rho_i}
 |A_I^{Q_{i,1,z}}-A_I^{Q_{i,0,z}}|
 \le D_C^{m+1}(m!)^{p_0}b^m\,\lambda_i(E),
 \tag{HL.31}
\]
and, for every \(q\ge0\),
\[
 \left|\left.\frac{d^q}{dz^q}
   (A_I^{Q_{i,1,z}}-A_I^{Q_{i,0,z}})
        \right|_{z=0}\right|
 \le q!\rho_i^{-q}
       D_C^{m+1}(m!)^{p_0}b^m\,\lambda_i(E).
 \tag{HL.32}
\]

**Proof.** Put \(R_i=H_i-H_i^E\), with
\(\|R_i\|_\infty\le\lambda_i(E)\) on the admitted chart. Differentiating
the normalized finite integral in \(t\), or its bounded holomorphic
integral version, gives the exact centered formula
\[
 \partial_t Q_{i,t,z}F
 =Q_{i,t,z}(FR_i)
   -Q_{i,t,z}F\,Q_{i,t,z}R_i .
 \tag{HL.33}
\]
For a bounded \(F\) independent of \(t\), (HL.24) therefore implies
\[
 |(Q_{i,1,z}-Q_{i,0,z})F|
 \le12\lambda_i(E)\|F\|_\infty.
 \tag{HL.34}
\]
When a product of \(r\) moments in a cumulant is telescoped, the
difference costs at most
\(12\lambda_i(E)\,r\,3^{r-1}\prod\|F_\ell\|_\infty\).
Summing its cumulant coefficients bounds it by
\[
 12\lambda_i(E)\,k!6^{k-1}
       \prod_{\ell=1}^k\|F_\ell\|_\infty .
 \tag{HL.35}
\]
Use (HL.16) once more in the complete reset formula (HL.12).
For example, \(D_C=12C(1+6C)\) is more than sufficient for (HL.31).
Analyticity and Cauchy's formula prove (HL.32). \(\square\)

For a retained variation outside the incoming source carriers, the input
coefficients are fixed and (HL.32) directly bounds the kernel part of the
response. For variations inside those carriers, one must separately carry
the direct and previous-current records of the inputs. Freezing their
values while differentiating the kernel gives the new current in isolation;
the remaining derivative is handled by the exact decorated product and
conditional-transport rules of M-03. A bound on the total derivative alone
is not used to bound two separately measured records through cancellation.

In particular, in one source direction the single-mark current is
\[
 (D Q_i)F
 =Q_i(F\,D\log w_i)-Q_iF\,Q_i(D\log w_i)
 \tag{HL.36}
\]
on the common source chart. The normalizer's derivative is present.
When a current-direction change alters a hard selector, the component
geometry, or the underlying padded support outside this analytic chart,
the finite signed-kernel difference of M-03 must be used instead.
Equations (HL.30)--(HL.36) make no assertion about such a change.

### 6. An eligible-only reset and a geometric tail bound

The source permits a precise reset design: average the old component
variables only for the eligible components selected by LFR I (i)--(ii).
Retain the other histories for later steps. This is an exact choice of
conditional projection and does not require averaging an arbitrarily
large component at this step. Consequently the shared-sign test below
does not obstruct a bounded-radius statement for this particular design.

This section proves that the relative-carrier sum in (HL.18) can be
controlled uniformly in the **source coordinates** for that design.
No independence hypothesis, contractive influence matrix, or small
conditional component mass is used.

Let \(h\) be the physical lattice unit at the step, so that the source
\(M\)-cube has physical side \(Mh\). Distances in the following counting
argument are measured in units of \(M\)-cubes. Write \(R=R_k\ge1\).
Every selected component \(X_j\) has
\[
 |X_j|_M\le(100R)^d,\qquad
 \operatorname{diam}_M(X_j)\le100\sqrt d\,R ,
 \tag{HL.G1}
\]
where \(|X_j|_M\) counts its \(M\)-cubes. The constants can be enlarged
by a dimension-only factor for closed-cube boundary conventions.

The superscript in LFR II p.377 is \(Z^{\sim}\), a neighborhood, not a
negative exponent denoting a shrunken set. Its stated carrier rule
implies that a carrier \(Y\) contains a whole selected component
whenever it meets that component. It may contain its larger
neighborhood as well. In particular
\[
 Y=(Y\setminus Z)\ \cup\
       \bigcup_{j:\,X_j\subseteq Y}X_j .
 \tag{HL.G2}
\]
Every \(Y\in\mathscr Y\) is a connected localization domain, and a
non-self carrier touching \(X_i\) has \(Y\setminus Z\ne\varnothing\).
These are source geometric properties, not probabilistic assumptions.
No bound on the diameter of a component of \(Z^{\sim}\) is used below.
Even if several enlarged components join, all their new collar and
connector cubes outside \(Z\) belong to \(S=Y\setminus Z\) and are
terminals that the relative tree must meet. The remaining pieces are
the original eligible components \(X_j\), each satisfying (HL.G1).
This observation concerns the counting lemma. Its posterior application
still retains the source-factorization guard stated after Theorem HL.1.

#### Lemma HL.8 -- counting relative carriers around an eligible component

There are dimension-only constants \(A_d>1\), \(B_d<\infty\), and \(D_d\)
such that, for every fixed admissible selected geometry, component
\(X_i\), and integer \(n\ge0\),
\[
 \#\{Y\in\mathscr Y:\ i\in J(Y),\
                 n\le d_{k,Z}(Y)<n+1\}
 \le B_d(1+R)^d A_d^{\,n+1}.
 \tag{HL.G3}
\]
Every such carrier satisfies
\[
 Y\subseteq N_{\,n+1+D_dR}^{\,M}(X_i),
 \tag{HL.G4}
\]
where \(N_r^M\) is the physical \(rMh\)-neighborhood in the periodic
metric on the finite torus. A nonwrapping Euclidean lift gives the
same estimate whenever it contains the carriers in question. No
distance across a chosen fundamental-box seam is treated as a
large Euclidean separation.
Both estimates are independent of the volume, the number and positions
of the other components, and their internal history values.

**Proof.** Put \(S=Y\setminus Z\). Choose a tree of length less than
\(n+1\), in \(M\)-units, meeting every closed cube of \(S\), as in
(1.67). An arbitrarily small extra length can be allowed if the infimum
is not initially attained.

A finite tree of length at most \(n+1\) admits a traversal of length at
most \(2(n+1)\). Sampling that traversal at intervals of \(1/4\) shows
that all cubes it meets lie in a connected set \(W\) of at most
\(K_d(n+2)\) cubes, for a dimension-only constant \(K_d\).
One can take adjacency by intersecting closures for this counting
upper bound; that graph has bounded degree. Enlarging the sampled
cubes by one fixed layer ensures connectedness and covers cubes met
only on a boundary. In particular \(S\subseteq W\).

Because \(Y\) is connected, contains \(X_i\), and is not contained in
that component, \(S\) includes a cube adjacent to \(X_i\). There are
at most \(C_d|X_i|_M\le C_d(100R)^d\) choices for this root cube.
The number of connected cube sets of size at most \(K_d(n+2)\)
containing a fixed root is at most a constant to that size: choose
a spanning tree and encode its depth-first traversal in the
bounded-degree graph. Choosing \(S\) within such a \(W\) adds at most
another factor \(2^{|W|}\).

Each selected component included in \(Y\) is adjacent to \(S\).
Indeed, distinct components of \(Z\) are not face-connected; a path
in \(Y\) leaving any one of them must enter \(S\). There are at most
\(2d|S|\) components adjacent by a face to \(S\). The choices of
which are present add at most \(2^{2d|S|}\). Once \(S\) and these
components are chosen, (HL.G2) determines \(Y\). Multiplying these
counts proves (HL.G3), after changing the dimension-only constants.
This is an upper bound and may count a carrier more than once.
For the shell \(n=0\), the same construction uses a dimension-only
number of cubes: a length-zero tree can meet only the bounded family
of closed cubes incident to its point. Thus no positive minimum
tree length is assumed. For example, the sampling and traversal
argument permits the deliberately generous choices
\[
 K_d=10\cdot7^d,\qquad
 A_d=\bigl[2^{\,2d+4}(3^d+1)^2\bigr]^{K_d},
 \tag{HL.G3a}
\]
with a larger dimension-only \(B_d\) absorbing a single extra factor
\(A_d\) and the root count. Optimizing this entropy constant is not
needed here.

For (HL.G4), fix a cube of \(S\) adjacent to \(X_i\) and a point of
the tree in that cube. Every point of any cube of \(S\) lies within
the tree's total length plus a dimension-only distance from \(X_i\).
A point of \(Y\setminus S\) is in a selected component touching
one of those cubes, and (HL.G1) bounds its extra distance by
\(D_dR\). This proves (HL.G4). \(\square\)

The proof only used the length of the tree that actually appears in
(1.67). It did not replace that length by a quotient metric in which
travel through a component is free.

#### Theorem HL.9 -- an actual eligible-component source-coordinate tail

Choose the source decay constant with the explicit lattice-entropy
margin
\[
 \omega=\bar\kappa-\log A_d>0 .
 \tag{HL.G5}
\]
This is a displayed additional parameter condition to be checked
jointly with all other source parameter constraints. The note does
not assert that the already retained J0 parameter tuple has passed
that extra check. There is \(C_{d,\bar\kappa}\), independent of volume
and the remaining history, such that
\[
 \lambda_i\le
 C_{d,\bar\kappa}\alpha(1+R_k)^d ,
 \tag{HL.G6}
\]
and
\[
 \sum_{\substack{Y:\,i\in J(Y)\\
          Y\not\subseteq N_r^M(X_i)}} b_Y
 \le
 C_{d,\bar\kappa}\alpha(1+R_k)^d
       e^{-\omega[\,r-D_dR_k-2\,]_+}.
 \tag{HL.G7}
\]

**Proof.** In the \(n\)-th shell, (HL.G3) and (HL.5) bound the sum by
\[
 B_d(1+R_k)^d A_d^{n+1}\alpha e^{-\bar\kappa n}.
\]
Its geometric sum proves (HL.G6). By (HL.G4), a carrier exiting
\(N_r^M(X_i)\) can occur only in a shell with
\(n+1+D_dR_k\ge r\). Starting the same geometric sum at that shell
proves (HL.G7), with the harmless integer-rounding factor included
in \(C_{d,\bar\kappa}\). \(\square\)

Combining (HL.G7) with (HL.19) proves a spatial response estimate for
the actual **full finite reset jet** in source coordinates. If an
incoming jet has source carrier \(S_I\), use the approximation region
\(E=S_I\cup X_i^{\sim}\cup N_r^M(X_i)\), retaining any stated
base-kernel collar. Its error has the bound (HL.G7) multiplied
by the explicit jet factor in (HL.19). The output carrier is
\(S_I\cup X_i^{\sim}\cup N_r^M(X_i)\), not a reassigned point anchor.

Combining the same tail with (HL.32) gives the native current estimate,
including all source orders, with an admitted radius at least
\[
 \frac{\rho\,r_*}
 {s_i+C_{d,\bar\kappa}\alpha(1+R_k)^d+r_*}.
 \tag{HL.G8}
\]
The cutoff dependence displayed in (HL.G8) is retained. This proof
does not need \(\alpha(1+R_k)^d<1\): positivity, the exact tilt
formula, and a possibly smaller analytic radius suffice for a
single-component reset.

This result answers the geometric part of the eligible-only design.
The reset can leave giant histories live for H-04/H-05. The remaining
gap for the H-03 statement is the transport of these estimates to
the actual retained coordinates and their separate current records,
including the boundaries between the locally selected sectors.
Even if a source expression is localized in \(E\), its true
dependency footprint after such a pullback must still be bounded.

### 7. What the new estimates do not justify

#### 7.1 The self-component law has not become independent

All internal old histories in \(X_i\) are still integrated jointly in
\(\nu_i\). It can be a highly correlated law. The non-small bound (1.69)
is specifically why its action was put in the base rather than discarded.

As a logical test of the scope, take one component with a single shared
random sign \(H\) and assign \(F_x=H\) to every site in that component.
Take all cross interactions to vanish. Then every cross bound (HL.5)
holds with \(\alpha=0\), the normalized base operation is entire in
unused external parameters, and
\[
 \kappa(F_x,F_y)=1
 \tag{HL.37}
\]
for every pair of internal sites. Thus the stated positive-product and
cross-interaction hypotheses alone imply no decay between arbitrary
interior insertion points. This is not a Yang--Mills counterexample. It
shows exactly which stronger conclusion cannot be extracted from these
source facts alone.

The component size restriction in LFR I bounds selected components by
\(100MR_k\), not by a scale-independent number of current blocks.
Theorem HL.9 retains precisely that radius. Unselected components are
left live under the design in Section 6. Thus internal giant-component
mixing is not required for that reset; it would be needed, or replaced
by an appropriate full-law reserve, for a later reset that actually
averages a giant component.

#### 7.2 The published unmarked expansion uses an unavailable conditional payment

LFR II p.389 combines the component cost
\[
 \exp\{2\kappa(100R_k)^d\}
 \tag{HL.38}
\]
with the unnormalized bound for \(\mathsf T'_k(X)1\). The source chooses
parameters so that, as displayed immediately before (1.95),
\[
 -2(1+\beta_0)^{-1}p_0(g_k)+1
       +2\kappa(100R_k)^d
 \le-\tfrac32 p_0(g_k).
 \tag{HL.39}
\]
This is a concrete place where probability mass pays for geometric
entropy in the source-free expansion. In the fixed-component posterior
(HL.3)--(HL.4), that mass cancels. It cannot then be used again as a
small conditional reset probability.

An unconditional marked proof can instead try to retain the actual
probability of such a sector and pay (HL.38) before conditioning. It
must prove that probability estimate with the exact marked law. The
rare-edit and counted-carrier results specify a
sufficient payment mechanism, but do not give its missing inherited
probabilities.

#### 7.3 Erasing a geometry label is a different posterior

To see the distinction without notation from the action, suppose an old
sector \(h\) has unnormalized density \(\rho_h(u,v)\), and the frozen
replacement draws \(u'\) from a normalized reference kernel
\(k_h(u'\mid v)\). Let
\[
 N_h(v)=\int\rho_h(u,v)\,du .
 \tag{HL.40}
\]
After forgetting \(h\), its posterior is
\[
 \Pr(h\mid u',v)=
 \frac{N_h(v)k_h(u'\mid v)}
      {\sum_{\widetilde h}
             N_{\widetilde h}(v)k_{\widetilde h}(u'\mid v)}.
 \tag{HL.41}
\]
The reference factor cancels in the old-field conditional expectation
at a fixed \(h\); it does not cancel across the sum in (HL.41).
If geometries change with \(h\), both the base measures and their
dependency footprints change. Theorem HL.3, whose comparison keeps the
base fixed, is not an estimate for (HL.41).

#### 7.4 Source background locality is not yet current-link locality

The source activity \(V_Y\) is local in the admitted background variables
\((U,J)\). The current norm M-03 assigns a coordinate its complete
dependency footprint, not merely its storage block. A minimizing
background field can depend on retained links outside the displayed
source carrier. Its pullback, its derivative bounds, the coarea
normalization and all selection changes must be carried.

Theorem HL.6 makes this distinction quantitative: its derivative bound
contains the admitted source radius \(\rho\) and the actual interaction
sum \(\lambda_i\). It does not set either to a favorable constant.
Furthermore the analytic input bound (HL.13) has not been derived for
all actual renormalized incoming jets in the required current-scale
regulator norm.

The source's normalized expansion (1.103) is compatible with these
observations. Its fixed residual domains are not summed there, so the
source does not need their own tree factors for that unmarked
convergence proof. A bound with insertion anchors and current
directions must pay the additional geometry it actually uses.

### 8. Exact residual inequality

The remaining estimate concerns a spatial estimate for the complete reset
jet, uniform in the remaining history, including derivative/current
marks. It is not just an estimate on the normalized value of a
single fixed component operation.

One sufficient form, in the already fixed M-03 norm, is the following.
For every admissible incoming decorated jet, the exact reset must admit
compatible carrier records such that
\[
 \sum_{X\supset\operatorname{anchors}(I)}
 w_h(X)\left[
    v_{h,m,X}(A_I^{\rm reset})
   +g_{h,m,X}(B_I^{\rm reset})
   +j_{h,m,X}(J_I^{\rm reset})\right]
 \le C_*^{m+1}(m!)^{p_*}\mathcal B_I .
 \tag{HL.42}
\]
Here \(C_*,p_*\) are independent of the cutoff depth, volume, current
scale and admitted remaining history, and \(\mathcal B_I\) is the
specified incoming current-scale carrier budget with its actual
running mixing coefficients. The current-scale normalization and the
native regulators are those already fixed in M-03. All higher input
vertices are included.

To obtain (HL.42) from the actual one-component estimates above still
requires the following concrete bounds:

- A source-to-current-coordinate carrier and radius bound for the
  normalized component law, including every direct and current
  pullback in the strong norm.
- A carrier-norm summation after the actual coordinate pullback, with
  the insertion anchors included. Theorem HL.9 already supplies a
  spatial source-coordinate tail for every eligible component.
  It does not replace a proof for the actual retained-coordinate
  footprints, regulators and separate difference/current records.
- If a later reset averages the remaining giant components, either
  a local/internal marked estimate for those laws or an actual
  full-law probability reserve sufficient to pay their carrier
  size and marked losses. The eligible-only reset may instead
  leave these histories to H-04/H-05.
- A treatment of any geometry-changing or geometry-erasing reset,
  including the applicable finite-difference currents, and, for
  (HL.41), its old masses, reference likelihoods and support currents.
- The stipulated current-scale input budget for the actual complete
  renormalized jet. A compact bare bound at scale \(a\) does not turn
  into a budget at scale \(h\) just because a conditional expectation
  was taken.

An alternative route would prove a sufficiently weighted influence or
cut-coupling theorem for the full physical posterior and combine it
with the cumulant theorem. The actual one-component
influences (HL.9) are inputs to such a route. A contractive row sum
uniform in the physical geometry, or an appropriate replacement for
it, has not been established here.

### 9. Application conditions

| H-03 requirement | Result of this argument |
|---|---|
| The actual posterior, rather than the fresh reference distribution | Identified in (HL.3)--(HL.4), directly from the positive component operations. |
| Conditional covariance and all higher reset responses | Full formula (HL.12), bounds (HL.14), (HL.19), (HL.29)--(HL.32); all incoming vertices retained. |
| A genuine spatial input from the source | Actual remote-component influence (HL.9); Theorem HL.9 sums the discarded-carrier bound uniformly for eligible-only resets, with radius \(O(MR_kh)\) and exponential tails. |
| Normalizer and self-action control | Exact normalization throughout; the self action remains in \(M_i\); source (1.75) used only on its admitted native domain. |
| Current response control | Proved in admitted native charts, with the explicit radius (HL.22); physical pullbacks and geometry-changing currents remain unbounded. |
| Uniformity in the remaining fixed eligible geometry | Proved in source coordinates by (HL.G3)--(HL.G8), with the source entropy condition (HL.G5) displayed. |
| Actual retained-coordinate carrier/current norm, including sector changes | **Not proved.** The missing inequality is (HL.42), with the listed pullback, current and sector costs. |


### References

1. T. Balaban, *Large Field Renormalization. I. The Basic Step of the R
   Operation*, Communications in Mathematical Physics **122** (1989),
   175--202.


2. T. Balaban, *Large Field Renormalization. II. Localization, Exponentiation,
   and Bounds for the R Operation*, Communications in Mathematical Physics
   **122** (1989), 355--392, The scope of every
   imported statement is specified in Section 1.


4. T. Balaban, *Renormalization Group Approach to Lattice Gauge Field
   Theories. I*, Communications in Mathematical Physics **109** (1987),
   249--301, p.257, DOI
   https://doi.org/10.1007/BF01215223 .
   Only its connected-cube and tree-size definitions are used as an
   additional input in Section 6; the counting proof is given here.

### Supplement AG.1: Application to the actual old-component posterior


The completed regular E and R theorems remove two useful native-contour obligations. Their scope does not yet identify an admitted current-coordinate contour for the archived-component posterior of HL.4.

#### The operation that still needs a current pullback

The reset of Annex AG averages an arbitrary incoming full jet under the old component operation \(\mathsf T'_k(X_i)\) in LFR II (1.71), tilted by the cross action in (1.72). The component's nonsmall self action from (1.69), old selectors, graph choices, local integrations and old-history sums remain inside that operation. Its joint analytic domain is inherited from the source's prepared multiscale map, including (1.65); its normalized native analytic estimate is (1.75).

The concrete application would be:

1. Compose the **actual current/native external coordinate map**, at the full real support and with fixed admitted outer geometry, into the input of LFR II (1.65).
2. Verify a simultaneous quantitative image reserve for every argument of the component operation (1.71) and its cross action (1.72), including the independent current and the complete self-component exponent. The estimate must hold for every old component history still integrated by that operation.
3. Use the resulting actual radius in HL.22. HL.6 then provides the normalized complex posterior bound and HL.7 its derivative/current-tail bound; HL.9 already supplies the eligible-component source-coordinate spatial tail.
4. Localize that coordinate pullback in the fixed M-03 norm, retaining the direct input derivative, the new conditional-kernel current, the previous currents, and any finite differences caused by sector changes.

These are actual applications to the source operation, not a request for another abstract cumulant theorem.

#### Why the completed regular R bound is not already this application

Theorem R14.3 concerns the regular R activities after the source has completed the component integrations and returned to its E/R/B normal form. The source assigns its boundary-intersecting outputs to B. The proof therefore uses the returned regular primitive domain for those R activities. It does not identify that regular domain with the prepared multiscale domain of the unintegrated \(\mathsf T'_k(X_i)\).

Consequently its holomorphic norm controls the already integrated action. A derivative bound on that action cannot simply be reused as a bound for the same component integral with an arbitrary incoming marked numerator. In particular it does not justify changing the current radius in HL.22 to the regular R radius without checking the input map above.

The finite-core reference estimate in Annex AE is also valuable but concerns a different probability kernel. In the exact frozen R quotient, the newly sampled reference factor cancels from the old conditional expectation. Its complex total-variation estimate cannot replace the normalized old-component estimate (1.75), whose base includes the old histories and self action. Both kernels are retained, with their distinct roles.

#### Exact remaining scope

The first two steps of the concrete application share the multiscale-domain transfer issue isolated in Supplement AF.3. The remaining spatial pullback, regulator and sector-current estimates in HL.42 are additional requirements; neither current contour theorem declares them proved.

The source-factorization guard in Annex AG remains unchanged. The product-base posterior is used only on geometries admitted by LFR II (1.71)–(1.72). A hypothetical nonsmall interaction joining different proposed component blocks must be placed in their common base or that cluster must be left live. The geometric carrier count does not authorize a new factorization.

The use of (1.65)–(1.75) requires admission on the actual multiscale domain and the strong retained-coordinate bound (HL.42).

See LFR II, CMP 122 (1989), pp. 374–380 and 390–392, Annex AD, Theorem E14.3, and Annex AE, Theorem R14.3 and Section 10.6.


---
