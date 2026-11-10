# C-05: normalized components and a direct rooted analytic norm

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

## Result and scope

This note proves three useful finite-dimensional or geometric statements:

1. A holomorphic normalized completed-component operator with a small **total crosspotential** produces a zero-free scalar partition factor and a bounded holomorphic logarithm. Moving-kernel responses are retained exactly and vanish when the crosspotential vanishes.
2. A rooted scalar oscillation norm gives normal convergence of the normalized action and a weighted Hessian Schur bound, without an original-birth decomposition and without a factor counting derivative endpoints.
3. Bounded, separated excluded components with an active-field buffer permit comparison of physical distance with the metric that traverses excluded components at no cost.

These statements do not yet prove the required uniform norm for Balaban's complete repeated construction. They isolate a possible direct repair of the CR.22 argument, which does not hold as stated. No assertion below is presented as a transcription of that argument.

In particular, the completed-component geometry may exclude arbitrarily large holes at the scale of completion. The counterexample in Section 7 applies to weakened norm assumptions, not to the actual eligible-history class.

**Metric qualification.** This note does not identify Balaban's \(d_k(X\setminus Y)\) with a zero-cost quotient metric. If it is an ordinary shortest-tree length spanning the exterior cubes, a path across the interior can still have its ordinary length charged. In that case the long-hole example in Section 7 does not satisfy the source norm. The precise source metric must be checked before using that example or the comparison in Section 6.

## 1. Source input relevant to this alternative

LFR II pp.379–380 bounds a normalized complex integration operator in (1.75), after controlling its total native-field correction. At pp.391–392, the second exponentiation uses fixed completed components and a weaker tree estimate. CMP119 pp.261–262 specifies analytic boundary activities and explicitly allows the outside-large-field version of their norm. These facts motivate the direct approach; they do not alone verify the rooted bound below.

Primary texts:

- Balaban, *Large Field Renormalization II*, CMP 122 (1989), 355–392, DOI [10.1007/BF01238433](https://doi.org/10.1007/BF01238433).
- Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP 119 (1988), 243–285, DOI [10.1007/BF01217741](https://doi.org/10.1007/BF01217741).

The precise powers in the source's small correction bound are not reproduced here and must be checked against the printed source before being used numerically.

## 2. A complete one-component theorem

Let \(\mathcal A\) be a complex unital Banach algebra with submultiplicative norm, \(\|1\|=1\). For the intended application it can be a space of bounded functions of the old internal variables, with the supremum norm. Let \(D\subset\mathbb C^N\) be an open parameter domain.

Suppose:

- \(z\mapsto\Pi_z\in\mathcal A^*\) is holomorphic in operator norm;
- \(\Pi_z1=1\) and \(\|\Pi_z\|\le M\), uniformly on \(D\), with \(M\ge1\);
- \(z\mapsto V_z\in\mathcal A\) is holomorphic and \(\|V_z\|\le\eta\) uniformly;
- \(q=M(e^\eta-1)<1\).

Define

\[
Z(z)=\Pi_z(e^{V_z}).
\tag{DN1}
\]

### Theorem DN1

On \(D\),

\[
|Z(z)-1|\le q,
\qquad
F(z):=\log Z(z)
\quad\text{is holomorphic},
\qquad
|F(z)|\le-\log(1-q).
\tag{DN2}
\]

The logarithm is the branch given by its convergent series about \(1\).

**Proof.** The exponential series converges in the Banach algebra and obeys

\[
\|e^{V_z}-1\|\le e^\eta-1.
\]

Normalization gives

\[
Z(z)-1=\Pi_z(e^{V_z}-1),
\]

hence the bound in (DN2). The image is contained in the disk \(|w-1|\le q<1\). Therefore

\[
F(z)=\sum_{n\ge1}\frac{(-1)^{n+1}}n[Z(z)-1]^n
\]

converges normally, is holomorphic, and is bounded by
\(\sum_{n\ge1}q^n/n=-\log(1-q)\). This proof includes all dependence of \(\Pi_z\) on \(z\).

For example, if \(\eta\le1\) and \(q\le1/2\), then

\[
|F(z)|\le2M(e^\eta-1)\le2eM\eta.
\tag{DN3}
\]

### Why the theorem is relevant

If \(\Pi_z=T_z/(T_z1)\), the normalized source estimate analogous to (1.75) can supply \(M\), potentially \(M=e^3\) after fixing a small enough common native domain. The theorem does not require a bound on \((T_z1)^{-1}\) separately, and does not discard the kernel's current response.

The required \(\eta\) is the norm of the **whole remaining crosspotential for that component**, after the source-defined internal action has been included in \(T_z\). A bound on every individual summand by \(\eta\) is not enough if the number of summands is unbounded.

An internal-variable-dependent large term cannot be discarded as a scalar constant. Absorbing it into \(T_z\) changes the normalized kernel; the bound on the new kernel and its common complex domain must then be proved.

## 3. Exact moving-kernel response and anchored stability

For \(z,w\in D\), assume \(\|V_z\|,\|V_w\|\le\eta\). Since \((\Pi_z-\Pi_w)1=0\),

\[
Z(z)-Z(w)
=(\Pi_z-\Pi_w)(e^{V_z}-1)
+\Pi_w(e^{V_z}-e^{V_w}).
\tag{DN4}
\]

The Banach-algebra exponential is Lipschitz on this ball with the bound

\[
\|e^{V_z}-e^{V_w}\|\le e^\eta\|V_z-V_w\|.
\tag{DN5}
\]

For a noncommutative algebra this follows from the Duhamel integral; for bounded scalar functions it follows pointwise.

Because the segment between \(Z(z)\) and \(Z(w)\) lies in \(|\zeta-1|\le q\),

\[
|F(z)-F(w)|
\le
\frac{
(e^\eta-1)\|\Pi_z-\Pi_w\|
+Me^\eta\|V_z-V_w\|
}{1-q}.
\tag{DN6}
\]

Thus the response of the normalized kernel is multiplied by a quantity of order \(\eta\). At \(V\equiv0\), \(Z\equiv1\) and every kernel-only derivative vanishes exactly.

The corresponding exact derivative identity is

\[
D_i Z
=(D_i\Pi_z)(e^{V_z}-1)
+\Pi_z(e^{V_z}D_iV_z)
\tag{DN7}
\]

for a commutative algebra. Here \((D_i\Pi_z)1=0\). Differentiating again retains all mixed kernel/potential terms:

\[
\begin{aligned}
D_iD_jZ={}&
(D_iD_j\Pi_z)(e^{V_z}-1)\\
&+(D_i\Pi_z)(e^{V_z}D_jV_z)
+(D_j\Pi_z)(e^{V_z}D_iV_z)\\
&+\Pi_z\!\left(e^{V_z}
  [D_iD_jV_z+D_iV_zD_jV_z]\right).
\end{aligned}
\tag{DN8}
\]

Finally,

\[
D_iD_jF=Z^{-1}D_iD_jZ-Z^{-2}(D_iZ)(D_jZ).
\tag{DN9}
\]

These formulas show explicitly why the normalized representation does not justify declaring all kernel coefficients current-independent. The cancellation is only of their response to the constant function \(1\).

For a spatial application, (DN6) can transfer an independently proved localized variation of the kernel and crosspotential into a localized scalar oscillation. The theorem does not supply that spatial variation from the operator norm \(M\) alone.

## 4. Cauchy gives a Hessian row without counting all endpoints

Here first consider scalar coordinates. Let \(F\) be holomorphic and bounded by \(A\) on

\[
\mathbb D_P(z^0)
=\{z:\max_j|z_j-z_j^0|<P\}.
\]

Fix \(z\) in the smaller disk \(\mathbb D_{\theta P}(z^0)\), \(0\le\theta<1\), and put \(p=(1-\theta)P\). For a fixed root \(i\) and a vector \(v\) with \(|v_j|\le1\), the function

\[
(s,t)\longmapsto F(z+s e_i+t v)
\]

is holomorphic for \(|s|,|t|<p/2\). Cauchy's estimate gives

\[
\left|\sum_jD_iD_jF(z)v_j\right|
\le\frac{4A}{p^2}.
\]

Choose the phases of \(v_j\) to align \(D_iD_jF\). Then

\[
\sum_j|D_iD_jF(z)|
\le\frac{4A}{(1-\theta)^2P^2}.
\tag{DN10}
\]

The bound has no factor equal to the number of endpoint coordinates.

Applying Theorem DN1 gives, for one completed component,

\[
\sup_i\sum_j|D_iD_j\log\Pi_z e^{V_z}|
\le
\frac{4[-\log(1-q)]}{(1-\theta)^2P^2},
\tag{DN11}
\]

provided the common complex current polydisc is verified. This is a complete finite-component conclusion under the explicit hypotheses of DN1.

For every \(m\ge1\), and directions \(\|v_a\|_\infty\le1\), the same construction with \(m\) complex parameters of radius \(p/m\) gives

\[
|D^mF(z)[v_1,\ldots,v_m]|
\le
\frac{m^m[-\log(1-q)]}{p^m}
\le
\frac{e^m m![-\log(1-q)]}{p^m}.
\tag{DN11a}
\]

This is a bound on the multilinear directional norm, and on every fixed-coordinate jet. It is not an assertion that all tensor coefficients have a dimension-free absolute sum.

### Weighted probes

Suppose the scalar function depends on a finite current-coordinate set \(S\). Write

\[
R_i(S)=\sup_{j\in S}\rho(i,j),
\]

where \(\rho\) is the desired spatial metric. For \(|v_j|\le e^{\chi\rho(i,j)}\), take
\(|s|<p/2\), \(|t|<p/[2e^{\chi R_i(S)}]\). The same proof yields

\[
\sum_j e^{\chi\rho(i,j)}|D_iD_jF|
\le\frac{4A e^{\chi R_i(S)}}{p^2}.
\tag{DN12}
\]

For fixed-size vector blocks, replace the left side by the sum of block operator norms. A factor at most the block dimension \(d_*\) suffices, by applying the scalar output estimate to an orthonormal basis of the root block and using
\(\|H_{ij}\|_{\mathrm{op}}\le\sum_{a=1}^{d_*}\|H_{ij}^{\mathsf T}e_a\|_2\).

A stronger direct formulation does not require finite support. If

\[
\Delta_iF(s,t;v)
=F(z+s e_i+t v)-F(z+t v)
\]

has a uniformly bounded analytic bidisc for every finitely supported weighted direction \(|v_j|\le e^{\chi\rho(i,j)}\), Cauchy bounds the weighted row directly. Establishing this anchored complex oscillation bound is a legitimate alternative to tracking original births.

The dimension-free endpoint argument is special to the Hessian row. A bounded multilinear norm for derivatives of order \(m\ge3\) does not automatically equal the absolute sum of all tensor coefficients; no such conversion is asserted here.

## 5. A rooted analytic activity criterion that also justifies differentiation

Let \(\Lambda\) be a finite current-coordinate set. For fixed retained data \(\xi\), suppose a countable family of activities \(B_X(z,\xi)\) is holomorphic on a common polydisc of radius \(P\), uniformly on the allowed retained-data set. Let \(S_X\subset\Lambda\) be its actual current support.

Subtract only the current-independent value:

\[
b_X(z,\xi)=B_X(z,\xi)-B_X(z^0,\xi).
\]

Assume \(\sup_{\mathbb D_P,\xi}|b_X|\le M_X\), and define

\[
\mathcal N_\chi
=
\sup_{i\in\Lambda}
\sum_{X:\,i\in S_X}
M_X
\exp\!\left(\chi\sup_{j\in S_X}\rho(i,j)\right).
\tag{DN13}
\]

### Theorem DN2

If \(\mathcal N_\chi<\infty\), the normalized action

\[
\widetilde B(z,\xi)=\sum_X b_X(z,\xi)
\tag{DN14}
\]

converges normally in finite volume, modulo the terms with \(S_X=\varnothing\), which vanish identically after subtraction. Its termwise current derivatives are justified, and on the smaller polydisc,

\[
\sup_i\sum_j e^{\chi\rho(i,j)}
\|D_iD_j\widetilde B\|_{\mathrm{op}}
\le
\frac{4d_*\mathcal N_\chi}{(1-\theta)^2P^2}.
\tag{DN15}
\]

**Proof.** Each nonzero summand has at least one current coordinate in \(S_X\). Thus

\[
\sum_XM_X\le|\Lambda|\mathcal N_0<\infty.
\]

The Weierstrass theorem gives normal convergence and holomorphy. On each smaller polydisc derivatives converge normally. Applying (DN12) term by term, then summing the nonnegative majorants, proves (DN15).

The hypothesis is a scalar oscillation bound on a common domain, rather than merely an absolute Hessian bound. It consequently controls the lower jets needed to justify differentiation. It allows arbitrary current-independent vacuum terms to be omitted from the normalized current action, but does not control their retained-data derivatives.

Actual scalar amplitudes can replace \(M_X\); however, if a native activity is only localized in its \((U,J)\) arguments, its pullback to the actual current chart can be nonlocal. The support \(S_X\), or a localized expansion of that pullback with summable tails, must be proved. Native carrier support cannot silently be treated as exact current-coordinate support.

## 6. Bounded and separated holes: a useful metric comparison

The following addresses the possibility that the actual completed components are bounded at their completion scale.

Let \(G\) be a unit-edge graph. Let the pairwise disjoint connected holes \(Y_a\) have intrinsic graph diameter at most \(D\), and suppose distinct holes have graph distance at least \(s>0\). Let the active endpoint set \(A\) have distance at least \(r_0>0\) from every hole.

Give edges internal to holes zero cost and all other edges unit cost, and call the resulting quotient distance \(d_Q\). Ordinary graph distance is \(d_G\).

### Lemma DN3

For \(x,y\in A\),

\[
d_G(x,y)\le
\left(1+\frac Ds+\frac{D}{2r_0}\right)d_Q(x,y).
\tag{DN16}
\]

**Proof.** Take a shortest quotient path and erase repeated visits to holes. Let its paid length be \(\ell=d_Q(x,y)\), and let it visit \(m\) holes. If \(m=0\), the conclusion is immediate. Otherwise the gaps between consecutive holes show \((m-1)s\le\ell\). Replacing each free traversal by a path inside its hole costs at most \(D\), so

\[
d_G(x,y)\le\ell+mD
\le(1+D/s)\ell+D.
\]

The endpoint buffer gives \(\ell\ge2r_0\), and absorbs the final \(D\) into (DN16).

If \(D=c_D R\), \(s=c_sR\), and \(r_0=c_rR\), the comparison constant is independent of \(R\). Therefore an outside-hole tree bound can pay a physical endpoint weight by spending a fixed fraction of its decay exponent. This eliminates the particular obstruction caused by an arbitrarily long single free hole.

However, (DN16) does not by itself prove (DN13). One still needs a rooted absolute sum over carriers or cluster records. A fixed hole with a large boundary can admit many different attached outside pieces. Source-specific smallness or an actual rooted cluster estimate must pay that incidence entropy.

For the actual proof, the required separation, endpoint buffer, and diameter statements must be verified for the **surviving holes used by the final norm**, including those inherited from earlier steps. Eligibility at an earlier completion scale alone is not the full verification of (DN16) in a later current chart.

## 7. Why the weak per-carrier norm alone is insufficient

This is an abstract counterexample to weakened norm assumptions, not an admitted Wilson history and not a claim that the actual eligible components have this geometry.

Take a long connected excluded region \(Y_N\) and active sites \(x,y\) on opposite sides, each reached by an exterior corridor of length \(R\). Let \(X\) be \(Y_N\) together with these two corridors. An outside-hole size can be bounded by a constant \(s_R\) independent of \(N\), while the physical distance between \(x,y\) grows with \(N\).

On \(|z_j|<P\), set

\[
b_X(z)=\alpha e^{-\kappa s_R}\frac{z_xz_y}{P^2}.
\tag{DN17}
\]

It is entire, local to the declared carrier, and obeys the uniform per-carrier amplitude bound \(|b_X|\le\alpha e^{-\kappa s_R}\). Nevertheless,

\[
e^{\chi d_G(x,y)}
|\partial_x\partial_y b_X|
=
\frac{\alpha}{P^2}
e^{-\kappa s_R+\chi d_G(x,y)}
\]

has no uniform bound as \(N\to\infty\).

There is also an unweighted rooted-incidence example. Choose \(n\) distinct active sites \(y_j\), each reached from the same excluded region by a corridor of length \(R\), and let \(X_j\) include that region, the common \(x\)-corridor, and the \(y_j\)-corridor. Use (DN17) for every \(j\). Every activity has the same valid bound, but

\[
\sum_j|\partial_x\partial_{y_j}\sum_{\ell=1}^n b_{X_\ell}|
=n\alpha e^{-\kappa s_R}/P^2.
\tag{DN18}
\]

The Hessian has star-graph eigenvalues
\(\pm\sqrt n\,\alpha e^{-\kappa s_R}/P^2\). A total scalar bound proportional to the volume of the excluded region can still hold. Hence a mere extensive scalar estimate also does not supply a uniform rooted Hessian estimate.

Bounded eligible holes may prevent the \(N\to\infty\) version at a fixed scale. Lemma DN3 explains the geometry that can repair the endpoint metric comparison. The incidence sum and its quantitative dependence on the allowed hole size still need to be controlled.

## 8. Several completed components: the exact additional work

A self-contained sufficient theorem for this extension, including the connected-series convergence proof, is now supplied in [A direct multi-component theorem for C-05](connected component expansion). It requires a component-incidence bound and a current-root incidence bound for the actual crosspotentials. It does not assume that those bounds follow from the source's per-carrier estimates.

For independent normalized operators on disjoint internal slots, untouched components disappear because \(\Pi_Y1=1\). If a Mayer factor touches component set \(I\), its elementary operator-norm cost is at most

\[
M^{|I|}.
\tag{DN19}
\]

This is preferable to a factor \(M^{\text{all components in the volume}}\), but it is not free. A connected expansion must pay the factor for the components actually touched, and prove the appropriate rooted summability.

The direct-repair program therefore needs the following concrete source identification:

1. The actual normalized \(\Pi_Y\) has a common analytic domain in the required current/native chart, with a uniform \(M\).
2. The total crosspotential for one eligible component, or the corresponding interaction norm before summing components, is small enough for DN1. Per-summand smallness is not a substitute.
3. For several components, the actual connected Mayer/polymer expansion has a rooted absolute incidence estimate strong enough to imply DN13, including the \(M^{|I|}\) factors.
4. The carrier metric can pay the desired physical endpoint weights. DN3 is one sufficient geometric mechanism, if its premises hold for the relevant final holes.
5. The current chart and its localization tails fit the common analytic domains. Kernel dependence is included by DN4–DN9, not set to zero.

A useful candidate size estimate is a total crosspotential \(\eta_k\le C\alpha_k\,\mathrm{poly}(R_k)\) on each eligible component. If \(\eta_k\to0\), DN1 applies uniformly. This estimate is a proposed target; the inspected pointwise activity bounds have not yet been turned into that total rooted estimate here.

## 9. What has actually advanced

The one-component normalization argument is complete and avoids the rejected per-birth charge assignment. It proves a genuine finite subcase and retains the full moving-kernel response. The rooted scalar criterion and the bounded-hole metric comparison are also complete under their explicit hypotheses.
