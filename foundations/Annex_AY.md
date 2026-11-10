# Conditional regular-law moments, native fields and spatial cumulants

**Annex AY.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).

**Scope of the inference.** The endpoint, stopped-prefix and repeated positive carrier estimates on actual all-history data are assumptions in this application. The native estimates cited below apply on their own admitted domains. In particular a derivative of an isolated minimizing map does not establish the derivative of a composed field at fixed older variables.


### 0. Conditional moment problem

The regular-law conclusion is the following.

> Combine the actual quadratic lower bound and complete perturbation budget to prove current-scale mean, all-p field/gradient moments, and spatial cumulant decay for the selected regular conditional law.

The required scope is:

> The law is the one in C-01, with fixed factorial growth and volume-uniform constants; its remaining application to all histories is H-04.

The selected conditional law must satisfy the C-04 perturbation budget, the complete boundary estimates under CL and CR, heterogeneous coercivity, and the convex support/Neumann hypotheses. The Wilson-normalized trajectory and its calibration are additional hypotheses.

The distinction is reflected in the conclusions. The note proves bounds for the actual constrained current field, its covariant current-scale gradient and the native scalar/tensor stencils of that field. It also proves an operator inequality for arbitrary marks in the stated weighted Sobolev spaces. A projected augmented mark can be put into that inequality only with its actual norms; its smoothness is not inferred from the smoothness of the marginal density.

The one-point envelope retains the exterior field. In particular, it is not asserted that every coordinate next to a conditioned exterior has a uniformly bounded mean independent of the logarithmic field radius. Such a statement would fail even for a strictly convex Gaussian law.

### 1. The exact law after the C-05 reduction

Fix one active retained datum in the admitted source representation. The datum contains the actual determining geometry, coarse fields, surviving older variables, selectors and the current exterior free coordinates. It is held fixed throughout the conditional estimates.

Let `I` be the current free bonds integrated in the regular interior of CMP119 (3.25). Let `O` denote the other free coordinates of the same current fluctuation chart and write `y` for their retained values. No older-layer fluctuation is inserted into `y`: older variables are parameters of the complete perturbation. Distances `rho` are shortest periodic current-lattice distances. Lie-algebra block dimension is fixed.

The exact C-01 law, with the coefficient-response factorization of Annex AX and the completed-component choice, is

\[
 d\nu_v(z)=Z_v^{-1}\mathbf1_D(z)
 \exp\{-\tfrac12z^TKz+b^Tz+W(z;v)\}\,dz,
 \qquad b=-K_{IO}y,
 \tag{RC18.1}
\]

where `K=K_II` is the principal block of the actual constrained precision `C* Delta C`. It includes the quadratic correction caused by the nonlinear averaging constraint. The constraints are solved before the interior/exterior split; they are not solved again after conditioning. The product domain is

\[
 D=\prod_{i\in I}D_i,\qquad
 D_i=\{z_i:\|z_i\|_{\rm source}<r_{k,i}\}.
 \tag{RC18.2}
\]

These are the literal independent-bond norm balls in C-07. They are symmetric and convex and do not vary with retained field values inside the fixed geometry/coupling chart. Write

\[
 P=P_k=A_1\ell_k^{p_0},\quad \ell_k=\log g_k^{-2},\quad g=g_k.
 \tag{RC18.3}
\]

Assume the literal support in (RC18.2) is contained in the common current contour with the stated margin. This is a hypothesis on the complete conditional representation.

The exact completed-R alternative LFR II (1.103)–(1.104) integrates each normalized completed operation with its entire incoming boundary exponential. This equality moves its scalar effects into `W`. The remaining canonical raw-data masses are independent of this inner current. It is an equality after those integrations, not a pointwise factorization of an unintegrated marked posterior. Ordinary older operations and failed prefixes retain their full current coefficient responses and Jacobians in `W`, as in Annex AW and the C-01 erratum. Constants independent of `z`, including the correct exterior Schur scalar, remain in the outer law. They cancel only from the normalized ratio (RC18.1).

Thus the choice made in C-05 changes no current coordinate, principal precision, retained force or product support in the law now being estimated. It does change which hidden variables have already been integrated, and an observable must pass through those same exact conditional expectations. That observation explains the separate marked application; it does not add a hypothesis to the scalar law (RC18.1).

For the interpolation used below set

\[
 d\nu_{s,t}(z)=Z_{s,t}^{-1}\mathbf1_D(z)
 \exp\{-\tfrac12z^TKz+t b^Tz+sW(z)\}\,dz,
 \quad 0\le s,t\le1.
 \tag{RC18.4}
\]

Additional arbitrary real linear tilts are permitted. They change neither the Hessian nor the domain. At finite cutoff all these normalizers are strictly positive and finite on an active fiber.

### 2. Actual force and complete perturbation envelopes

For a nonnegative scalar matrix define

\[
 \|A\|_a=\sup_i\sum_j e^{a\rho(i,j)}A_{ij}.
 \tag{RC18.5}
\]

The same notation for a block matrix means the corresponding absolute block norms. On the current four-dimensional lattice,

\[
 S_a=\sup_i\sum_j e^{-a\rho(i,j)}<\infty
 \tag{RC18.6}
\]

with constants independent of volume and of a restriction to an admitted subset. Counting shortest displacement representatives proves the same bound on periodic tori.

#### Lemma RC18.1 — the actual derivative and force data

After a fixed reduction of the common coupling ceiling, there are fixed constants `C`, `delta>0` and nonnegative, symmetric, coordinate-independent majorants `A_ij` such that throughout the real support and its relevant straight segments

\[
 \|D_iD_jW(z)\|\le A_{ij},\qquad
 \|A\|_\gamma\le C P^{-2},\qquad
 |D_iW(0)|\le C P^{-1}.
 \tag{RC18.7}
\]

The ceiling can make `||A||_gamma` smaller than any prescribed positive constant fixed in advance. The exterior force obeys

\[
 |y_j|\le C P,\qquad
 |b_i|\le C P\,e^{-\delta d_O(i)},\qquad
 d_O(i)=\operatorname{dist}(i,O).
 \tag{RC18.8}
\]

If `O` is empty, set `d_O=+infinity` and `b=0`.

**Proof of the exterior bound.** CMP119 (3.12)–(3.14) bounds the physical current fluctuation on its complete new active domain before the free-coordinate split. The exact local constraint chart and fixed Lie-algebra norm conversions therefore give `g|y_j|<=C epsilon_k`, hence `|y_j|<=CP`. The fixed constant includes the source cutoff constants; it is not declared small. The actual exterior relocation (3.22) has its admitted small relative-field correction, and the C-05/C-06 compatibility check retains the same bound at the real exterior datum. Surviving variables outside this current chart belong to `W`, not to an unbounded extension of `y`.

C-06 supplies the absolute precision estimate on the full current free-coordinate matrix before restriction,

\[
 \|(K_{IO})_{ij}\|\le K_0e^{-\delta_K\rho(i,j)}.
 \tag{RC18.9}
\]

Consequently

\[
 |b_i|\le C P\sum_{j\in O}e^{-\delta_K\rho(i,j)}
 \le C P S_{\delta_K/2}e^{-\delta_K d_O(i)/2}.
 \tag{RC18.10}
\]

This proves (RC18.8), including the actual exterior coefficient. No Gaussian recentering or denominator comparison has been used.

**Proof of the perturbation bounds.** Use the exact ownership of sectors in C-01/C-05/C-06. In a split

\[
 W=W_{ER}+W_B+W_{\rm cl}+W_{\rm meas},
 \tag{RC18.11}
\]

each scalar term is included once. A local classical or measure term already assigned to the complete C-05 boundary perturbation is omitted from the last two terms. The estimates in the predecessor proofs are sums of absolute primitive majorants, so removing a duplicated subset only improves them.

For `W_ER`, C-04 gives first-derivative and fixed entrywise Hessian majorants with anchored sums

\[
 d_{ER}\le C K_{ER}P^{-1},\qquad
 \|A_{ER}\|_\gamma\le C K_{ER}P^{-2},
 \quad K_{ER}=\mathfrak K_E+C_Rg^{\kappa_0-11},\quad \kappa_0\ge12.
 \tag{RC18.12}
\]

For `W_B`, Theorem AB17.1 and its primitive endpoint/carrier proof give

\[
 d_B\le C\mathcal K_{B,k}P^{-1},\qquad
 \|A_B\|_\gamma\le C\mathcal K_{B,k}P^{-2}.
 \tag{RC18.13}
\]

The majorants in these two formulas are formed **before** summing the carriers and taking the supremum over real current points. This distinction matters: a bound for `sup_z sum_j |D_iD_j W(z)|` would not by itself bound `sum_j sup_z |D_iD_j W(z)|`. In particular the dimension-free row estimate DS.11 does not justify exchanging these operations. Instead use its individual coordinate Cauchy bound and define

\[
 (A_{ER})_{ij}=\frac{C}{P^2}
   \sum_{Y:\,i,j\in I_Y}\widehat K_{ER}e^{-\widehat\kappa n(Y)}.
 \tag{RC18.13a}
\]

The fixed Lie-algebra block dimension is in `C`. The actual current carrier contains at most `C_M(n(Y)+1)` free blocks. Its weighted row sum is therefore bounded by the C-04 anchored carrier series with one additional factor `C_M(n+1)`. Reserve a fixed positive part of the source exponential to pay that factor. The resulting constant is larger than DS.10's convenient dimension-free constant, but is still independent of volume, depth and history and has precisely the `P^{-2}` smallness in (RC18.12). In C-05, (AB17.27) is already a fixed endpoint majorant; its `m=2` layer-cake/carrier sum supplies `A_B` directly. These are the fixed matrices used here. Symmetrizing them costs at most a fixed factor.

The explicit prefactor is uniformly bounded as `g` decreases. Indeed, with `D_k<=C g ell_k^q`, its local terms satisfy

\[
 g^{-2}D_k^3\le Cg\ell_k^{3q}\longrightarrow0,
 \qquad D_k\longrightarrow0,
 \qquad \theta_k=\ell_k^{p_0-q}\longrightarrow0.
 \tag{RC18.14}
\]

The apparently singular heterogeneous term is bounded by a polynomial in `ell_k` times

\[
 g^{-1}e^{-c\ell_k^r}
 =\exp\{\ell_k/2-c\ell_k^r\}\longrightarrow0,
 \qquad r>1.
 \tag{RC18.15}
\]

The completed and failed older-operation terms have the uniform chronological bounds in (AB17.7h)–(AB17.7i). Thus all terms in (AB17.24), including the old-density responses, are at most one fixed `K_*`. This is a bound on the actual complete prefactor, not merely on a homogeneous specialization.

For completeness, the remaining local gradient is obtained without assigning a coupling-dependent value to an unverified analytic-domain constant. The degree-three ownership is fixed **before** splitting the classical localizations into bulk and boundary families. The exact source algebra, as given in Annex AI, is as follows. Before the final constraint substitution write the classical function as `F(0)+ell(q')+(1/2)<q',K_raw q'>+R_3(q')`, and write `D=D_2+D_{>=3}`. With `q=gC_vt`, its remainder after subtraction of the complete constrained quadratic is

\[
 \begin{split}
 g^{-2}\big\{&R_3(q-hD(q))
 -\ell(hD_{\ge3}(q))
 -\langle q,K_{\rm raw}hD(q)\rangle\\
 &+\tfrac12\langle hD(q),K_{\rm raw}hD(q)\rangle\big\}.
 \end{split}
 \tag{RC18.15a}
\]

Every displayed function starts at degree three (the last at degree four). The removed quadratic includes `-ell(hD_2)`; the stationary first derivative on free coordinates is zero. CMP109 (2.5)–(2.12) gives this algebra; CMP116 (1.37)–(1.39) localizes the representative remainder, and its paragraph before Lemma 2 applies the same localization to the other classical terms. C-06 has checked the actual heterogeneous admission of those localizations.

For clarity one can impose a carrierwise convention which makes the cancellation independent of any shorthand in the localization. Let `f_Y(t)` be the exact localized functions of the complete classical remainder (RC18.15a), before bulk/boundary assignment. Replace each by its integral third-order Taylor remainder

\[
 f_Y^{[3]}(t)
 =\frac12\int_0^1(1-s)^2D^3f_Y(st)[t,t,t],ds
 =f_Y(t)-\sum_{r=0}^2\frac1{r!}D^rf_Y(0)[t^r].
 \tag{RC18.15b}
\]

The anchored analytic sums converge at each finite cutoff. The sums of their zero-, first- and second-order coefficients are zero because the constant, stationary linear term and constrained quadratic have already been removed in (RC18.15a). Hence the sum of (RC18.15b) is the same complete classical remainder. The Taylor remainder depends on the same current carrier, and its norm on a fixed smaller absolute ball is bounded by a fixed multiple of the original analytic carrier norm. Its third-derivative bound on that smaller ball gives the cubic norm on every still smaller running ball. Thus this choice preserves the source exponential majorants and, in particular, the classical contribution in AB17.21 up to fixed constants. It is not an assertion that the cancellation persists after deleting an arbitrary noncubic subset.

Now assign these individually cubic carriers to their actual bulk or boundary family. Evaluate the actual exterior relocation in each assigned function. Every induced lower-order current response from that shifted evaluation is retained in `W_B`, as in AB17.21; it is not discarded as a vanishing remainder. The remaining unrelocated local `W_cl(t)` is a sum of individually cubic functions. It therefore has vanishing first and second full-current jets at `t=0`. This fixes the ownership used in (RC18.11) and below.

Fix once the absolute source domain used in HC.19–HC.22. On that fixed domain, the localized classical remainder has an anchored third-derivative majorant

\[
 \sup_i\sum_{j,l}e^{\gamma\tau(i,j,l)}
 \sup_t\|D_iD_jD_l W_{\rm cl}(t)\|
 \le Cg.
 \tag{RC18.16}
\]

Here `t` is the full current free field, including the later retained exterior. To see the estimate, take three coordinate Cauchy derivatives of the fixed-contour bound HC.20 on a fixed smaller absolute ball. Its value factor is `C g^{-2} epsilon_abs^3` and each derivative costs `C g/epsilon_abs`. The product is `Cg`. The local bulk source expansion is into actual current-layer carriers: the underlying large-field/proper-scale boundary terms belong to `W_B`. At a compact current carrier of tree length `n`, the two summed current-coordinate indices cost at most `C(n+1)^2`, with the fixed `M`-cube block multiplicity included. A fixed share of the source carrier exponential pays this polynomial, the tree weight and the anchored carrier count. If the equivalent endpoint-kernel form of the same localization is used instead, retain its three endpoint exponentials and sum their fixed-order lattice tails; the one-layer endpoint/volume proof of AB17.27–AB17.31 gives a fixed constant at order three. It does not insert the number of microscopic fine bonds. The constants are fixed before `g` varies.

By the carrierwise ownership just specified, the remaining unshifted local classical sum has zero first and second jets in the full current at `t=0`. Taylor's integral formula on the admitted segment from `0` to `t` gives

\[
 |D_iW_{\rm cl}(y)|\le CgP^2,
 \qquad
 \sup_{z\in D}\|D^2_{I}W_{\rm cl}(z+y)\|_\gamma
 \le CgP.
 \tag{RC18.17}
\]

The proof of (RC18.16) also supplies fixed entrywise majorants for the second formula. Boundary-classified classical terms, if their relocation produces lower-order responses, are kept in `W_B` and are not subjected to the vanishing-jet assertion.

The Haar and nonlinear exceptional-constraint logarithms have the fixed absolute analytic neighborhood and local trace-loop expansion used in HC.21–HC.22. One and two Cauchy derivatives there give

\[
 \sup_{z\in D}|D_iW_{\rm meas}(z+y)|\le Cg,
 \qquad \|A_{\rm meas}\|_\gamma\le Cg^2.
 \tag{RC18.18}
\]

The constants absorb the one fixed absolute radius. The background-only linear coarea determinant stays in the outer factor. Neither an extensive determinant nor its volume is used in (RC18.18).

The support and the exterior amplitude imply `g||z+y||_infinity<=CgP`, so the entire segment used above lies in the fixed absolute neighborhood for one small enough ceiling. Combining (RC18.12)–(RC18.18) gives

\[
 \begin{split}
 d_k&:=\sup_i|D_iW(0)|
       \le C\{P^{-1}+gP^2+g\},\\
 \eta_k&:=\|A\|_\gamma
       \le C\{P^{-2}+gP+g^2\}.
 \end{split}
 \tag{RC18.19}
\]

Since `P=A_1 ell_k^{p_0}`, `gP^3` tends to zero. After fixing a ceiling with `P>=1`, (RC18.19) proves (RC18.7) and its arbitrary smallness. This proof retains the actual first derivative; a Hessian estimate alone would not prove it. ∎

### 3. The full weighted covariance operator on the actual support

C-06 supplies `K>=lambda_0 I` and the weighted principal conjugation estimate. Choose one `gamma>0` so that

\[
 a_K(\gamma):=
 \sup_i\sum_j\|K_{ij}\|(e^{\gamma\rho(i,j)}-1)
 \le\lambda_0/4.
 \tag{RC18.20}
\]

Reduce it, if necessary, to fit the fixed carrier and chart rates. By Lemma RC18.1 choose the common coupling ceiling so that

\[
 \eta_k\le\lambda_0/4,
 \qquad
 c_0:=\lambda_0-a_K(\gamma)-\eta_k\ge\lambda_0/2.
 \tag{RC18.21}
\]

The same inequalities hold for every `s,t` in (RC18.4) and every additional real linear tilt. Write `lambda=lambda_0-eta_k>=3lambda_0/4` for a fixed unweighted lower bound, decreasing it to `lambda_0/2` when one common constant is preferable.

#### Lemma RC18.2 — block resolvent and covariance bound

For every measure in that family, there is a vector Neumann covariance operator `A_nu^{-1}` with

\[
 \operatorname{Cov}_\nu(F,G)
 =\langle\nabla F,\mathcal A_\nu^{-1}\nabla G\rangle_{L^2(\nu)},
 \tag{RC18.22}
\]

and block operator estimates

\[
 \|\Pi_i\mathcal A_\nu^{-1}\Pi_j\|_{L^2\to L^2}
 \le c_0^{-1}e^{-\gamma\rho(i,j)}.
 \tag{RC18.23}
\]

Consequently

\[
 |\operatorname{Cov}_\nu(F,G)|
 \le \sum_{i,j}G_{ij}
       \|\nabla_iF\|_{L^2(\nu)}
       \|\nabla_jG\|_{L^2(\nu)},
 \quad
 G_{ij}=\frac{2}{\lambda_0}e^{-\gamma\rho(i,j)}.
 \tag{RC18.24}
\]

The theorem applies to the indicated weighted Sobolev functions. In particular the stronger bilinear estimate required in CM.9a has now been derived for the actual law.

**Proof.** Start with smooth convex approximations of each literal bond ball and use their product. For `V= -log` of the smooth density inside the support, let

\[
 L=-\Delta+\nabla V\cdot\nabla
 \tag{RC18.25}
\]

with scalar Neumann boundary condition. The positive form on vector fields tangent to each boundary face is

\[
 \begin{split}
 \mathfrak a(w,w)={}&\int\sum_\alpha|\partial_\alpha w|^2\,d\nu
     +\int\langle w,V''w\rangle\,d\nu\\
 &+\sum_i\int_{\partial D_i\times D_{\ne i}}
       \mathrm{II}_i(w_{i,\tan},w_{i,\tan})\,d\nu_{\partial i}.
 \end{split}
 \tag{RC18.26}
\]

Its boundary term is nonnegative by convexity. The associated operator is the differentiated Neumann realization of `L tensor I+V''`. Solving `Lu=G-nu G` and differentiating the weak equation gives `nabla u=A_nu^{-1}nabla G`. The usual scalar integration-by-parts identity proves (RC18.22).

For a real one-Lipschitz spatial function `f_i`, multiply a whole Lie-algebra block by `M_i=exp(gamma f_i)`. This multiplier is constant in the integration variables. It preserves each face's tangent/normal constraint because it is scalar on that face's block. The scalar differential part commutes with `M`; the boundary form stays nonnegative after the weighted test. The principal conjugation loss is at most `a_K(gamma)` and the complete perturbation costs at most `eta_k`. Thus, for every vector source `h`, the form equation `A_nu w=h` gives

\[
 c_0\|Mw\|_2^2\le |\langle Mw,Mh\rangle|,
 \qquad
 \|M\mathcal A_\nu^{-1}M^{-1}\|\le c_0^{-1}.
 \tag{RC18.27}
\]

This argument is for arbitrary vector sources, not just gradients. Choosing `f_i=rho(i,j)` proves (RC18.23). Splitting the gradients into their finitely many block components and applying Cauchy–Schwarz in `L^2(nu)` proves (RC18.24).

The smooth approximations can be chosen symmetric and increasing to the literal convex balls. Their product boundary forms have the same sign and the same constants. At fixed cutoff the density and the relevant smooth functions are bounded on the compact product. Dominated convergence proves the covariance inequalities on the actual product support. Approximation in the displayed weighted Sobolev norms gives the general domain. Corners and nonsmooth norm spheres introduce no negative boundary term. This is precisely where C-07's product-support identification is used. ∎

### 4. Current-scale means and all-p field fluctuations

Let `a` be a fixed positive number less than `gamma/4`. Fix `G` as in (RC18.24). The scalar kernel norm is bounded by

\[
 \|G\|_a\le \frac{2}{\lambda_0}S_{\gamma-a}=:G_a.
 \tag{RC18.28}
\]

Using the arbitrary smallness in (RC18.7), reduce the coupling ceiling once more until

\[
 \|GA\|_a\le G_a\eta_k\le1/2.
 \tag{RC18.29}
\]

This is a fixed numerical choice, independent of moment order, cutoff depth, volume and retained history. Define the nonnegative resolvent kernel

\[
 H=(I-GA)^{-1}G,\qquad \|H\|_a\le2G_a.
 \tag{RC18.30}
\]

#### Theorem RC18.3 — actual mean profile and all-p coordinate moments

For the actual selected regular law and for the interpolation (RC18.4), there are fixed `C,c>0` such that

\[
 |\nu_{s,t}z_i|
 \le C\{P^{-1}+P e^{-c d_O(i)}\}=:M_i,
 \tag{RC18.31}
\]

and, for every `p>=1`,

\[
 \|z_i-\nu_{s,t}z_i\|_p\le C\sqrt p,
 \qquad
 \|z_i\|_p\le M_i+C\sqrt p.
 \tag{RC18.32}
\]

More precisely the mean is bounded by the actual force convolution

\[
 \sup_{s,t}|\nu_{s,t}z_i|
 \le\sum_j H_{ij}
 \left(|b_j|+|D_jW(0)|+sigma\sum_lA_{jl}\right),
 \qquad \sigma=\sqrt{d_{\mathfrak g}/\lambda}.
 \tag{RC18.33}
\]

Here `d_g` is the fixed real block dimension. In particular there is no extensive force norm in the estimate.

**Proof.** An arbitrary real linear tilt leaves the Hessian and product support unchanged. Applying the unweighted covariance estimate in that tilted law to `u dot z_i`, where `|u|=1`, gives

\[
 \frac{d^2}{dt^2}\log\nu e^{t u\cdot z_i}
 =\operatorname{Var}_{\nu_t}(u\cdot z_i)\le\lambda^{-1}.
 \tag{RC18.34}
\]

Integrating twice yields a centered sub-Gaussian moment-generating bound. Exponential Markov inequality and integration of its tails prove (RC18.32) componentwise, and the fixed block dimension gives the vector estimate. In particular `||z_i-nu z_i||_2<=sigma`.

At `s=t=0` the density and support are even, so the coordinate mean is zero. At `s=0`, interpolate `t` from zero to one. The normalized derivative is `Cov(z_i,b dot z)` and (RC18.24) gives the reference bound `|nu_0,t z_i|<=sum_j G_ij |b_j|`.

For `sW`, convexity of the support and Taylor's integral formula give

\[
 |D_jW(z)|\le |D_jW(0)|+\sum_lA_{jl}|z_l|.
 \tag{RC18.35}
\]

Write `M_i^*=sup_s,t |nu_s,t z_i|`. Differentiate the normalized mean in `s`, apply (RC18.24), and use (RC18.32) at `p=2`. The resulting componentwise inequality is

\[
 M^*\le G|b|+Gd+GA(M^*+\sigma\mathbf1).
 \tag{RC18.36}
\]

All vectors are finite at each cutoff. The positive convergent Neumann series in (RC18.30) proves (RC18.33). Lemma RC18.1 bounds the nonforce term by `C/P`. The row norm of `H` then bounds its convolution by `C/P`.

For the exterior term use `H_ij<=2G_a exp(-a rho(i,j))` and (RC18.8). The inequality `d_O(i)<=rho(i,j)+d_O(j)` and a fixed smaller exponential rate imply

\[
 \sum_j e^{-a\rho(i,j)}e^{-\delta d_O(j)}
 \le C e^{-c d_O(i)}.
 \tag{RC18.37}
\]

For example take `c<min(a,delta)/2` and retain the remaining `exp[-(a-c)rho]` for the lattice sum. This proves (RC18.31). ∎

The term `P exp(-c d_O)` is essential. It permits a conditioned boundary layer with means of order `P` while providing an order-one bound in the bulk at distance of order `log P`. Neither a zero retained mean nor a uniform rare-collar estimate at every boundary bond is asserted.

A local collar consequence is nevertheless available. Suppose the literal bond ball contains a Euclidean ball of radius `c_D P`. If `d_O(i)>=d_0`, where `d_0` is a fixed sufficiently large constant, then (RC18.31) gives `|nu z_i|<=c_D P/4` for a sufficiently small common ceiling. The concentration argument yields

\[
 \nu\{z_i\notin\tfrac12D_i\}\le C e^{-cP^2}.
 \tag{RC18.38}
\]

This last conclusion uses the stated lower radius comparison and therefore is not invoked under a convention in which the literal support radius is smaller than `P`. The mean and moment theorem itself requires only the verified upper support inclusion and applies to either conservative support convention.

### 5. The actual nonlinear constrained field and its covariant gradient

This section verifies the field maps on which the law acts. The map is the one in CMP119 (3.15), including its nonlinear constraint correction. It is not replaced by the linear chart `exp(i g C z)V`.

Let `V` be the retained reference current configuration, and let the exact local average constraint be

\[
 \Phi_v(a)=Q_va+N_v(a),\qquad N_v(0)=DN_v(0)=0.
 \tag{RC18.39}
\]

With the actual exceptional-bond right inverse `h_v` and kernel injection `C_v`, the physical current chart is

\[
 q=gC_vt,\qquad
 a_v(t)=q-h_vD_v(q),\qquad
 D_v(q)=N_v(q-h_vD_v(q)),\qquad
 U_e(t)=\exp(i a_{v,e}(t))V_e.
 \tag{RC18.40}
\]

Here `t=y+iota_I z`. Source normalization factors, including the fixed one-step averaging factor, are in the definition of `Q_v,h_v`. Their local inverses are the ones admitted in C-06, HC.10. The derivative kernels below refer to free `z` coordinates while `v,y` stay fixed.

All the current free blocks share this one-step local chart, even when the retained determining geometry has older layers. The source regular collar admits the local averaging paths and exceptional stencils. The native stencils below are anchored where their whole fixed footprint lies in that admitted current chart. A field whose footprint enters an old nonregular component belongs to the history/matching analysis rather than to the selected regular field family of this theorem.

#### Lemma RC18.4 — uniform current-chart derivative kernels

For fixed positive rates, after one further fixed ceiling reduction,

\[
 |D_i a_{v,e}(y+z)|\le Cg e^{-c\rho(e,i)},
 \tag{RC18.41}
\]

\[
 \sup_e\sum_{i,j}e^{c\tau(e,i,j)}
       \sup_{z\in D}\|D_iD_j a_{v,e}(y+z)\|
 \le Cg^2,
 \tag{RC18.42}
\]

with the analogous anchored row and column sums. These estimates hold uniformly over the admitted actual heterogeneous class.

**Proof.** The finite averaging paths and the analytic group mean have uniform local derivatives in the fixed small physical neighborhood. The exceptional linear block is uniformly invertible by HC.10. A constraint row uses a fixed number of current coordinates in a fixed number of adjacent unit blocks, and a current coordinate occurs in a fixed number of such rows. Its second derivative uses the same finite dependency footprint. Thus both the row and column matrix sums and each anchored second-derivative tensor sum are bounded uniformly before any inverse is taken. These are current-block counts; no count of microscopic bonds in the reconstructed fine field enters. These facts give fixed weighted matrix and second-derivative tensor bounds for `C_v,h_v,N_v` in every current block; no global gauge choice or old-coordinate inversion is used.

The full current support obeys `g||y+z||_infinity<=CgP`, hence tends to zero. For one fixed spatial exponential norm, `||N'_v(a)h_v||<=C gP` on that support and a fixed surrounding physical neighborhood small enough for the local inverse. Choose the absolute neighborhood so the norm is at most `1/2`. Differentiation of the actual fixed-point equation gives

\[
 D'_v=(I+N'_v(a)h_v)^{-1}N'_v(a),
 \tag{RC18.43}
\]

\[
 D''_v=(I+N'_v(a)h_v)^{-1}
 N''_v(a)[I-h_vD'_v,I-h_vD'_v].
 \tag{RC18.44}
\]

The inverse is a convergent weighted Neumann series. Finite-range composition and the triangle inequality for the connecting-tree length preserve the corresponding matrix and anchored tensor norms. The substitution `q=gC_vt` gives one factor `g` in (RC18.41) and two factors in (RC18.42). All local constants depend only on the admitted block size, group and source regularity ceiling. The older geometry enters only through the uniformly admitted retained coefficients. This proves the asserted extension of the earlier native chart calculation to the actual current region. ∎

Define the normalized constrained fluctuation around its fixed exterior reference by

\[
 \mathcal A_e(z)=g^{-1}
    [a_{v,e}(y+z)-a_{v,e}(y)],\qquad
 U_{\rm ref}=U(y).
 \tag{RC18.45}
\]

The difference of link exponentials is kept as such when forming group observables; (RC18.45) is not an assertion that `exp(i a(y+z)) exp(-i a(y))` equals the exponential of a difference in a noncommutative group.

For neighboring oriented current links, let `nabla_ref` denote any one of the fixed covariant finite-difference stencils with the unitary background `U_ref`. The stencil has uniformly bounded range and coefficients. Physical first differences have the extra factor `h_k^{-1}`; (RC18.46) is in current lattice units.

#### Theorem RC18.5 — constrained field and gradient moments

For `p>=1`,

\[
 \begin{split}
 \|\mathcal A_e-\nu\mathcal A_e\|_p
 +\|\nabla_{\rm ref}\mathcal A_e
       -\nu\nabla_{\rm ref}\mathcal A_e\|_p
 &\le C\sqrt p,\\
 |\nu\mathcal A_e|+|\nu\nabla_{\rm ref}\mathcal A_e|
 &\le C\{P^{-1}+P e^{-c d_O(e)}\}.
 \end{split}
 \tag{RC18.46}
\]

The uncentered `L^p` bound is the sum of the two displayed right sides. For the full current field `g^{-1}a_v(y+z)`, its fixed reference value `g^{-1}a_v(y)` and its fixed covariant derivative are added explicitly.

**Proof.** The coordinate mean `m=nu z` belongs to the convex product support. By (RC18.41),

\[
 |\mathcal A_e(z)-\mathcal A_e(m)|
 \le C\sum_i e^{-c\rho(e,i)}|z_i-m_i|.
 \tag{RC18.47}
\]

Minkowski and (RC18.32) give an `L^p` bound `C sqrt p`. Centering costs at most a factor two. The same proof applies to the finite covariant difference stencil.

For the mean, expand about `m`. The linear term has zero expectation. Equation (RC18.42), divided by `g`, and `||z_i-m_i||_2<=sigma` bound the expected quadratic remainder by `Cg`. The value `mathcal A_e(m)` is bounded by the exponential convolution of `|m_i|`, by integrating (RC18.41) from `0` to `m`. Theorem RC18.3 and (RC18.37) bound that convolution by `C[P^{-1}+P exp(-c d_O(e))]`. Finally `g<=C/P` at the fixed small ceiling. The same argument applies to the covariant difference. ∎

If a physical canonically normalized potential is defined by `mathcal A_e/h_k`, multiply the potential estimate by `h_k^{-1}` and its physical gradient estimate by `h_k^{-2}`. The corresponding unrescaled connection has an additional factor `g_k`. These dimensional factors have not been absorbed into the constants.

### 6. Native scalar/tensor fields in the exact selected law

Use the fixed clover family of Annex E, with the scalar trace replaced by the Wilson action density, including its genuine off-diagonal tensor components. Equivalently, take any of its finitely many curvature-bilinear stencils and the Wilson action density. Let `P_{alpha,x}(U)` denote its dimensionless finite-loop polynomial, with the fixed parallel transports to a common base point retained. Set

\[
 O_{\alpha,x}(z)=h_k^{-4}g^{-2}P_{\alpha,x}(U(y+z)).
 \tag{RC18.48}
\]

The fixed normalization conversion between the Wilson action and `g^{-2}` belongs to the declared coupling dictionary and changes only fixed constants. An additional running mixing matrix is not bounded by this theorem.

Let `B_x` be `g^{-1}` times a fixed local sum of the reference plaquette distances `||U_ref,p-I||` over the actual stencil and the fixed additional plaquettes needed by its transport paths. By the real source regularity in CMP119 (3.12)–(3.14), the uniform-depth current averaging bound checked below, and `|y|<=CP`,

\[
 B_x\le CP.
 \tag{RC18.49}
\]

This conclusion concerns stencils in the admitted current chart. It does not bound an arbitrary old retained field by `P`. The current reference is the actual `V=V^(k)=M^k(U_{k+1})` of CMP119 (3.10); its full averaging depth `k` must be retained. Here is the precise local application which bounds it.

Take one fixed physical cube, in current units, containing the entire actual `k`-fold averaging footprints of all bonds in the native stencil and its fixed transport paths. The dependency cone of the actual average has physical diameter at most a fixed multiple of its output spacing, as in the two-endpoint-block convention of BM.2. The native stencil is finite. Thus this cube has side `C_b`, independent of `k`. The source current regular region has several `MR_k`-cube collars inside `Omega_{k+1}`; for the same small ceiling used in C-05, `R_k` exceeds the fixed footprint constant. Hence the whole cube and a fixed additional margin lie in the regular current patch on which (3.12) holds. No averaging footprint crosses an old determining interface in this application.

Write `eta` for the fine spacing in current units. CMP119 (3.12) gives `||U_{k+1}(partial p)-I||<=C epsilon_k eta^2` throughout that cube. Apply one ordered axial gauge on the cube, anchored at a fixed fine vertex. The exact plaquette path-interchange argument in BM.20 gives `||U_{k+1}^u(e)-I||<=C epsilon_k eta` and hence a fine potential of magnitude `C epsilon_k`. Now apply the actual uniform-depth average estimate BM.21 with `h_p=h_n=1` and `p=k`. Its proof uses CMP99 p.406 after (3.78), followed by the fixed final averaging step (E14.39)–(E14.41); it does not iterate a constant greater than one `k` times. It yields

\[
 \|\log M^k(U_{k+1}^u)_b\|\le C\epsilon_k.
 \tag{RC18.49a}
\]

Raw averaging is gauge covariant with the restriction of the fine gauge to the coarse endpoints. All four coarse plaquette links use the same cube gauge. Multiplying them and using real unitarity shows `||V_p-I||<=C epsilon_k` in the original gauge as well. This uses the true `M^k`, not a substitution by a one-step average or an unrelated corrected operator. CMP102 p.278, immediately after (7), also records the source consequence that regular configurations have regular determining averages, consistently with this local calculation.

Finally telescope the finite current plaquette products from `V` to `U(y)`. The correction `|a_v(y)|<=CgP` follows from (RC18.40)–(RC18.44). Unitarity bounds the product differences by the sum of their link differences. Since `epsilon_k/g<=CP`, this proves (RC18.49). Conjugating a curvature along a finite parallel transporter changes neither its real matrix norm nor this conclusion.

Fix a rate `theta>0` smaller than the derivative-kernel and covariance rates. Put

\[
 Z_x(z)=\sum_i e^{-2\theta\rho(x,i)}|z_i|,
 \qquad
 M_x=\sum_i e^{-2\theta\rho(x,i)}M_i,
 \qquad Q_x=1+B_x+M_x.
 \tag{RC18.50}
\]

The actual derivative kernels prove the deterministic estimates

\[
 |O_{\alpha,x}(z)|\le C h_k^{-4}[B_x+Z_x(z)]^2,
 \tag{RC18.51}
\]

\[
 \left(\sum_i e^{2\theta\rho(x,i)}
        |D_iO_{\alpha,x}(z)|^2\right)^{1/2}
 \le C h_k^{-4}[B_x+Z_x(z)].
 \tag{RC18.52}
\]

Indeed matrix telescoping and (RC18.41) give one factor `g` for each differentiated link and an exponentially local first derivative. Each undifferentiated curvature is at most `Cg(B_x+Z_x)`. A parallel-transport derivative multiplies an already small curvature. Its possible contribution after the `g^{-2}` normalization is `C g(B_x+Z_x)^2`, rather than the linear expression from differentiating a curvature factor. On the actual support, however, `B_x+Z_x<=CP` and `gP` is uniformly small. Consequently this term is at most `C(B_x+Z_x)` with the same endpoint decay. Differentiating the two curvature factors and their finite transporters therefore proves (RC18.52); multiplying them proves (RC18.51). For the Wilson scalar use `||U_p-I||_HS^2=2s(U_p)` and its first derivative. The scalar repair is a fixed linear combination and hence satisfies the same estimates. This verifies all components of the fixed native family rather than only its trace.

#### Theorem RC18.6 — all-p native values and gradients

For every native component and every `p>=1`,

\[
 \|O_{\alpha,x}\|_p
 \le C h_k^{-4}(B_x+M_x+\sqrt p)^2,
 \tag{RC18.53}
\]

\[
 \|O_{\alpha,x}-\nu O_{\alpha,x}\|_p
 \le C h_k^{-4}\{Q_x\sqrt p+p\},
 \tag{RC18.54}
\]

\[
 \left\|\left(\sum_i e^{2\theta\rho(x,i)}
      |D_iO_{\alpha,x}|^2\right)^{1/2}\right\|_p
 \le C h_k^{-4}(B_x+M_x+\sqrt p).
 \tag{RC18.55}
\]

All constants are uniform over the actual selected regular laws. Their displayed background envelopes obey

\[
 M_x\le C\{P^{-1}+P e^{-c d_O(x)}\},\qquad Q_x\le CP.
 \tag{RC18.56}
\]

**Proof.** Theorem RC18.3 and Minkowski's inequality give `||Z_x||_p<=M_x+C sqrt p`. Equations (RC18.51)–(RC18.52) prove (RC18.53) and (RC18.55).

For the centered estimate write `xi=z-m`, where `m=nu z`, and set `X_x=sum_i exp(-theta rho(x,i))|xi_i|`. Then `||X_x||_p<=C sqrt p`. The segment from `m` to `z` lies in the actual convex product domain. The fundamental theorem of calculus, (RC18.52), and Cauchy–Schwarz in the reciprocal spatial weight give

\[
 |O_{\alpha,x}(z)-O_{\alpha,x}(m)|
 \le C h_k^{-4}\{(B_x+M_x)X_x+X_x^2\}.
 \tag{RC18.57}
\]

Taking moments and subtracting its expectation proves (RC18.54). The first formula in (RC18.56) is the convolution inequality (RC18.37); the second uses (RC18.49) and `P>=1`. ∎

### 7. Spatial cumulants, arbitrary Sobolev marks and fixed factorial growth

This section works with the actual complete interacting law (RC18.1), not with its Gaussian reference. For a mark `F_i` anchored at `x_i` and `m>=2`, define

\[
 B_{i,m}=\|F_i-\nu F_i\|_{2m},\qquad
 D_{i,m}=\left\|\left(\sum_b e^{2\theta\rho(b,x_i)}
                       |\nabla_bF_i|^2\right)^{1/2}\right\|_{2m}.
 \tag{RC18.58}
\]

These are actual conditional norms. No assertion about an unexamined projected mark is hidden in their definition.

#### Theorem RC18.7 — cut estimate for the exact regular conditional cumulants

For any nontrivial label partition `[m]=A disjoint-union B`,

\[
 |\kappa_\nu(F_1,\ldots,F_m)|
 \le C_0 c_{m-1}
 \sum_{i\in A,j\in B}e^{-\theta\rho(x_i,x_j)}
    D_{i,m}D_{j,m}\prod_{l\ne i,j}B_{l,m},
 \tag{RC18.59}
\]

where `c_n=sum_{pi in Pi_n}(|pi|-1)!<=n!2^{n-1}` and `C_0` is fixed. The theorem is valid whenever the displayed weighted Sobolev moments are finite.

**Proof.** Center every mark; cumulants of order at least two are unchanged. Lemma RC18.2 gives the covariance resolvent for arbitrary vector sources. Let `W_i` multiply block `b` by `exp(theta rho(b,x_i))`. Weighted conjugation and the triangle inequality give

\[
 \|W_i^{-1}\mathcal A_\nu^{-1}W_j^{-1}\|
 \le C_0 e^{-\theta\rho(x_i,x_j)}.
 \tag{RC18.60}
\]

For example factor the operator as `(W_i^{-1} A_nu^{-1} W_i)(W_i^{-1}W_j^{-1})`. The first factor is bounded by the same form argument; the second is a block diagonal multiplier of norm at most the displayed exponential.

For disjoint label sets `E,F` with at most `m` labels in their union, expand the gradients of the two products in the covariance identity. Apply (RC18.60) to each differentiated pair. Hölder with the available `L^{2m}` norms gives

\[
 \left|\operatorname{Cov}_\nu
   \left(\prod_{i\in E}F_i,\prod_{j\in F}F_j\right)\right|
 \le C_0\sum_{i\in E,j\in F} e^{-\theta\rho(x_i,x_j)}
 D_{i,m}D_{j,m}
 \prod_{l\in(E\cup F)\setminus\{i,j\}}B_{l,m}.
 \tag{RC18.61}
\]

Write `M_E=nu product_{i in E} F_i` and `M_E^0=M_{E intersect A}M_{E intersect B}`. The latter are the moments of the product of the two marginal laws. Their mixed cumulant is zero. Subtract the two cumulant partition formulas and telescope the product over blocks of each partition. A differing block is exactly the covariance in (RC18.61); all other blocks cost the product of the corresponding `B_l,m`.

For a fixed crossing pair `i,j`, only partitions placing them in one block occur. Merging these two labels identifies that coefficient sum with `c_{m-1}`. There is no additional independent block-count factor. This proves (RC18.59). The coefficient inequality follows, for instance, by encoding ordered partitions as permutations with cuts. Smooth bounded approximation, followed by convergence in the displayed Sobolev norms, proves the asserted domain. ∎

#### Corollary RC18.8 — native all-order decay in the actual law

Let `tau(x_1,...,x_m)` be the length of a minimum spanning tree of the current anchors. Then for `m>=2`,

\[
 \boxed{
 |\kappa_\nu(O_{\alpha_1,x_1},\ldots,O_{\alpha_m,x_m})|
 \le C^{m+1}(m!)^2 h_k^{-4m}
     \prod_{i=1}^m Q_{x_i}
     \exp\left[-\frac{\theta\tau(x_1,\ldots,x_m)}{m-1}\right].}
 \tag{RC18.62}
\]

The full native moments satisfy

\[
 \left|\nu\prod_{i=1}^mO_{\alpha_i,x_i}\right|
 \le C^m m!h_k^{-4m}\prod_{i=1}^m Q_{x_i}^2.
 \tag{RC18.63}
\]

The same estimates hold uniformly for the interpolation laws. Constants may depend on the fixed group, block size, source parameters and prescribed rates, but not on `m`, total volume, cutoff depth or the admitted retained history. The explicit `Q_x`, `P_k` and physical factors are not hidden in those constants.

**Proof.** From Theorem RC18.6, at moment order `2m`, one can take

\[
 B_{i,m}\le C h_k^{-4}Q_{x_i}m,
 \qquad
 D_{i,m}\le C h_k^{-4}Q_{x_i}\sqrt m.
 \tag{RC18.64}
\]

Delete a longest edge of a minimum spanning tree. Every edge crossing the resulting cut is at least as long as the deleted edge; otherwise replacing it lowers the tree length. That edge has length at least `tau/(m-1)`. The cut sum in (RC18.59) has at most `m^2` terms. Its moment factor is `m^{m-1}` and its partition coefficient is at most `(m-1)!2^{m-2}`. Thus the total is bounded by `C^m(m!)^2`, using `m^m<=e^m m!` and absorbing the remaining fixed polynomial factor in `C^m`. This proves (RC18.62). For the full moments, use Hölder at order `m`, (RC18.53), `Q_x>=1` and `m^m<=e^m m!`. ∎

The order-dependent range in (RC18.62) has controlled summability. In four current dimensions,

\[
 \sup_{x_1}\sum_{x_2,\ldots,x_m}
 \exp\left[-\frac{\theta\tau(x_1,\ldots,x_m)}{m-1}\right]
 \le C_\theta^m(m!)^5.
 \tag{RC18.65}
\]

To prove it, dominate the minimum-tree exponential by the sum over all labelled trees. Successively sum each tree's leaves; each edge costs at most `C((m-1)/theta)^4`. Cayley's count `m^{m-2}` and the same factorial inequality give (RC18.65), including periodic tori. Combining with (RC18.62), after division by the displayed envelopes, gives an anchored cumulant sum of fixed factorial power seven. No cutoff-independent exponential-source series is required.

### 8. Application boundary and exact application conditions

Under the common complete-potential, coercivity and support hypotheses, the following estimates apply to the selected regular law.

| Requirement | Result |
|---|---|
| C-01 law with all current responses | Equation (RC18.1), using the factorization of Annex AX and exact completed-R reduction; all scalar effects retained in `W`. |
| Actual selected support | Literal independent-bond convex product from C-07; the vector Neumann boundary form is retained with its nonnegative sign. |
| Retained current force | Source bound (RC18.8), with its spatial boundary profile and its nonzero conditional mean. |
| Complete first derivative and Hessian | Lemma RC18.1 derives actual fixed majorants, including ordinary/failed/completed old operations, local classical and measure terms. |
| Current-scale conditional mean | Theorem RC18.3 and its explicit force-resolvent formula. |
| All-p constrained field and covariant gradient | Theorem RC18.5 uses the exact nonlinear constraint chart. |
| All native scalar/tensor field and gradient moments | Theorem RC18.6 treats the whole fixed native family, with the actual reference envelope. |
| Spatial cumulants and fixed factorial growth | Theorem RC18.7 and Corollary RC18.8; volume-uniform constants and summable order-dependent range. |
| Arbitrary input marks | Theorem RC18.7 applies with their actual Sobolev norms; no native replacement or projection-regularity assertion. |

The mean, gradient moment and cumulant estimates use the complete conditional Hessian bound, the retained exterior force, and the regular support hypotheses. Their uniform Wilson application requires CR, CL and the complete sector budgets above.

The remaining conditions include actual projected-mark bounds. That requirement concerns applying the conditional-law theorem in the marked induction; it is not an assertion that those bounds have been proved here. The catalogue dependency graph places M-04, the actual native/transported-mark matching, downstream of C-08, and likewise uses C-08 in the later M-06 induction. Requiring their completed matching as an input to C-08 would reverse that graph. The C-08 statement and its application conditions are met at their law-level scope by the results above, while the precise operator inequality (RC18.59) exposes the Sobolev inputs that those later applications must supply. No criterion is removed and no projected mark is replaced by a native mark.

The conclusion does not finish H-04 or H-05: the conditional background envelope and the resulting retained conditional means still have to be integrated against the complete outer history law. Nor does it finish M-04/M-06: (RC18.48) is the native field in the actual nonlinear current chart, not the unidentified conditional expectation of an arbitrary original microscopic observable. A projected mark with poor Sobolev regularity is not repaired by applying (RC18.59) to a different function. H-03 supplies a different missing estimate for exact history-reset responses. The full continuum Schwinger hierarchy, rotations, ultraviolet identification, energy estimates and phase selection remain outside C-08.

### 9. Source and proof references

- Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP **119** (1988), 243–285: (3.12)–(3.15), pp.267–268, for the actual physical current bound and nonlinear constraint chart; (3.16)–(3.25), pp.268–270, for selected support, exterior relocation and exact regular integral.
- Balaban, *Propagators for Lattice Gauge Theories in a Background Field*, CMP **99** (1985), 389–434: (3.155)–(3.158), p.428, and Theorem 3.15, p.432, for the actual constrained precision, heterogeneous gap and exponential locality. Used in the already checked C-06 scope.
- Balaban, CMP **99**, p.406 after (3.78), and CMP **102**, p.278 after (7): the actual uniform-depth relative-average bound and the printed regularity consequence for determining averages. The normalized local application is the already proved BM.20–BM.21 in Annex AF; its exact `M^k` and footprint margin are retained in (RC18.49a).
- Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories II*, CMP **116** (1988), 1–22: the exact fluctuation decomposition, nonlinear constraint terms, and localized classical remainder in Section 1, especially (1.37)–(1.43). The fixed absolute-domain and carrier use is the one as given in C-06.
- Balaban, *Large Field Renormalization II*, CMP **122** (1989), 355–392: (1.103)–(1.104), pp.391–392, for the exact completed-component alternative used in Section 1.
