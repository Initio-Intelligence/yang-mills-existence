# Quasilocal normalized kernels: a connected expansion with local current supports

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

**Status:** A proved conditional extension of the finite-component theorem in *A direct multi-component theorem for C-05*. It does not assert that the complete Balaban current pullback satisfies the required hypotheses.

## 1. The issue addressed

A kernel local in native background variables generally becomes only exponentially local after composition with the actual current-to-background map. Declaring its current support equal to its native carrier is therefore invalid.

This note supplies a replacement. Normalize first, construct normalized local approximants, and expand their zero-mass differences **after** the dependency-graph cancellations in the cumulant have been performed. This produces a normally convergent sum of scalar terms with genuine finite current supports. Their weighted root norm includes all kernel responses.

The resulting estimates use current incidence, not original birth labels.

## 2. Assumptions and notation

Let \(\mathcal V\) be a finite family of integrated components, and let \(\mathcal I\) be the finite set of scalar current coordinates of a cutoff volume. Work on a common complex current polydisc \(D\), uniformly in any retained parameters under discussion.

For component \(v\), suppose normalized holomorphic integration operators \(\Pi_{v,z}\) admit approximants \(\Pi_{v,z}^{[r]}\), \(r\ge0\), such that:

1. Every operator acts on the same block variables and common support; products over distinct components factorize.
2. \(\Pi_{v,z}^{[r]}1=\Pi_{v,z}1=1\).
3. \(\Pi_v^{[r]}\) depends only on current coordinates in a finite nested set \(H_{v,r}\).
4. The operator-norm expansion
   \[
   \Pi_{v,z}=\sum_{r\ge0}\pi_{v,z}^{r},
   \qquad
   \pi_v^0=\Pi_v^{[0]},
   \quad
   \pi_v^r=\Pi_v^{[r]}-\Pi_v^{[r-1]}\ (r\ge1)
   \tag{Q1}
   \]
   converges uniformly on \(D\).
5. There are bounds \(\sup_D\|\pi_v^r\|\le c_{v,r}\).

All operators act on compatible common unital Banach algebras of functions with the supremum norm; the interactions, their products, and their norm-convergent exponentials belong to those algebras. Holomorphy is in operator norm. Assume explicitly that every mixed iterated product functional used below exists on the joint function algebra, is holomorphic in the external parameters, and obeys
\[
\left|\left(\bigotimes_{v\in I}\pi_{v,z}^{r_v}\right)G\right|
\le\left(\prod_{v\in I}c_{v,r_v}\right)\|G\|_\infty.
\tag{Q1a}
\]
The product operation is multilinear and continuous in the factor functionals on these compatible spaces; in particular it commutes with the operator-norm sums in (Q1). Thus the expansion in (Q14) below equals the original product functional. The original normalized products have the corresponding factorization on disjoint internal slot sets. Kernel coefficients may depend on the fixed external parameters, but not on another component's integrated variable; such cross-component dependence belongs in the interactions. Complex integral kernels on fixed supports with the corresponding total-variation bounds satisfy these requirements. For abstract functionals, (Q1a), this compatibility, and joint holomorphy are assumptions, not consequences of writing a formal tensor product. If a source operator evaluates analytic functions at complex arguments, its common analytic function algebra must be used; no analyticity on all bounded nonanalytic functions is asserted.

Normalization gives \(\pi_v^r1=0\) for \(r\ge1\). It also implies \(c_{v,0}\ge1\) if the bound is chosen at least as large as the operator norm.

Let \(V_e(z,\omega_{I_e})\), \(e\in\mathcal E\), be holomorphic interactions. Their nonempty integrated supports are \(I_e\subseteq\mathcal V\), their genuine finite current supports are \(S_e^V\subseteq\mathcal I\), and
\[
v_e=\sup_D\|V_e(z)\|_\infty.
\tag{Q2}
\]
Current-independent internal terms can be absorbed into the component operators only when the stated normalized bounds remain valid. Terms with empty integrated support are external scalar terms and are treated separately.

A quasilocal potential may first be expanded as a convergent sum of local pieces and those pieces used as the labels \(e\). The identities and convergence of that expansion are inputs, not a consequence of the theorem.

### Spatial extent hypothesis

Fix the actual external metric \(\rho\). Assign nonnegative base extents \(\ell_e\) and kernel-layer extents \(\ell_{v,r}\). For a tuple \(e_1,\ldots,e_n\) connected by overlaps of \(I_{e_a}\), let \(\sigma\) be a partition of its vertices into connected blocks. For every block \(C\in\sigma\), write \(I_C=\bigcup_{a\in C}I_{e_a}\) and choose a radius \(r_{v,C}\) for each \(v\in I_C\).

Require that the corresponding current support
\[
S_\Gamma=
\bigcup_{a=1}^nS_{e_a}^V
\;\cup\!
\bigcup_{\substack{C\in\sigma\\v\in I_C}}
H_{v,r_{v,C}}
\]
has diameter at most
\[
L_\Gamma=
\sum_{a=1}^n\ell_{e_a}
+\sum_{\substack{C\in\sigma\\v\in I_C}}\ell_{v,r_{v,C}}.
\tag{Q3}
\]

This is a genuine physical extent statement. It is not a triangle inequality for minimum distance to an excluded component.

One sufficient geometry is as follows. Choose a nonempty base carrier \(G_v\) and an anchor in it, with \(H_{v,r}\subseteq G_v^{+r}\), the radius-\(r\) neighborhood. Include \(S_e^V\), the carriers \(G_v\), and the anchors for \(v\in I_e\) in the base set whose diameter is bounded by \(\ell_e\). Set \(\ell_{v,r}=2r\). Connected interactions share anchors, so their base union has diameter at most \(\sum_a\ell_{e_a}\). Adding the layer neighborhoods increases the diameter by at most twice the sum of their radii, proving (Q3).

This choice charges the base carrier in \(\ell_e\), rather than charging its diameter again in every localization layer.

## 3. Quantitative conditions

Fix a spatial weight \(\lambda\ge0\), and define

\[
\begin{aligned}
M_v(\lambda)&=\sum_{r\ge0}c_{v,r}e^{\lambda\ell_{v,r}}<\infty,\\
N_v(i;\lambda)&=\sum_{\substack{r\ge0\\i\in H_{v,r}}}
c_{v,r}e^{\lambda\ell_{v,r}},\\
\vartheta_v(i)&=\frac{N_v(i;\lambda)}{M_v(\lambda)}.
\end{aligned}
\tag{Q4}
\]

Thus \(M_v\ge1\) and \(0\le\vartheta_v(i)\le1\). Set

\[
w_e=v_e e^{\lambda\ell_e}\prod_{v\in I_e}M_v(\lambda),
\qquad
q_e(i)=\mathbf1_{\{i\in S_e^V\}}+
\sum_{v\in I_e}\vartheta_v(i).
\tag{Q5}
\]

The two hypotheses are

\[
2\sup_{v\in\mathcal V}
\sum_{e:\,v\in I_e}w_e e^{|I_e|}
\le1,
\tag{Q6}
\]

and

\[
K_i=\sum_e w_e e^{|I_e|}q_e(i),
\qquad K_*=\sup_iK_i<\infty.
\tag{Q7}
\]

Smallness of the Hessian will require \(K_*/P^2\) to be small on the actual current polydisc of radius \(P\). The component condition (Q6) alone does not imply this application-specific conclusion.

## 4. The theorem

Define
\[
Z(z)=
\left(\bigotimes_{v\in\mathcal V}\Pi_{v,z}\right)
\exp\left(\sum_eV_e(z)\right).
\tag{Q8}
\]

### Theorem Q1

Under (Q1)–(Q7), \(Z\) is zero-free on \(D\), and its connected logarithm has a normally convergent localized scalar expansion
\[
F(z)=\log Z(z)=\sum_\Gamma F_\Gamma(z),
\]
where each \(F_\Gamma\) has current support contained in \(S_\Gamma\), and

\[
\sum_{\Gamma:\,i\in S_\Gamma}
e^{\lambda L_\Gamma}
\sup_D|F_\Gamma|
\le K_i.
\tag{Q9}
\]

If \(D\) contains the current polydisc of radius \(P\), then on its concentric \(\theta P\) subdomain, \(p=(1-\theta)P\), the physical weighted Hessian obeys

\[
\sup_i\sum_j e^{\chi\rho(i,j)}
\|D_iD_jF\|_{\mathrm{op}}
\le\frac{4d_*K_*}{p^2},
\qquad 0\le\chi\le\lambda.
\tag{Q10}
\]

Here \(d_*\) is a fixed upper bound on the dimension of a current block; it is \(1\) for scalar coordinates.

If \(z,z'\in D\) differ only in a finite current-coordinate set \(Q\), the localized expansion also gives
\[
|F(z)-F(z')|
\le2\sum_{i\in Q}K_i.
\tag{Q11}
\]

All moving-kernel terms are included. At \(V\equiv0\), \(Z=1\) exactly.

## 5. Proof

### 5.1 Perform dependency cancellations before localizing kernels

For a tuple \(e_1,\ldots,e_n\), let \(G\) connect vertices \(a,b\) when \(I_{e_a}\cap I_{e_b}\ne\varnothing\). Set
\[
m(C)=
\left(\bigotimes_{v\in I_C}\Pi_{v,z}\right)
\prod_{a\in C}V_{e_a}.
\]

The moment-cumulant formula can be regrouped into partitions \(\sigma\) with connected blocks in \(G\):
\[
\kappa(V_{e_1},\ldots,V_{e_n})
=\sum_{\sigma}c_\sigma(G)\prod_{C\in\sigma}m(C).
\tag{Q12}
\]
The coefficient \(c_\sigma(G)\) is the linear coefficient of the chromatic polynomial of \(G/\sigma\).

The dependency-graph argument in *A direct multi-component theorem for C-05*, Lemma MC1, proves
\[
\sum_{\sigma}|c_\sigma(G)|
\le2^{n-1}\tau(G),
\tag{Q13}
\]
where \(\tau(G)\) is its spanning-tree count, and all coefficients vanish when \(G\) is disconnected. Its proof uses deletion-contraction for the linear chromatic coefficient and the bijection between a spanning tree with a chosen edge subset and the corresponding internal/quotient trees.

That argument is unchanged here: original normalized kernels factorize on disjoint integrated supports. The cancellations in (Q12) are performed before any kernel is replaced by a zero-mass increment. Expanding raw moment-cumulant terms separately and discarding their cancellation would not give (Q13).

### 5.2 Expand each kernel once per connected moment

For each \(C\), substitute (Q1):
\[
m(C)=
\sum_{\{r_{v,C}:v\in I_C\}}
\left(\bigotimes_{v\in I_C}\pi_{v,z}^{r_{v,C}}\right)
\prod_{a\in C}V_{e_a}.
\tag{Q14}
\]
Every integrated component appears once in each such connected moment. The same component can occur in several different moment factors in (Q12), as it already does in the exact cumulant algebra. Those occurrences will be paid explicitly.

A term of the product in (Q12), decorated by these radii, is holomorphic and depends only on \(S_\Gamma\). Its norm, multiplied by \(e^{\lambda L_\Gamma}\), is at most
\[
\left(\prod_a v_{e_a}e^{\lambda\ell_{e_a}}\right)
\prod_{\substack{C\in\sigma\\v\in I_C}}
\left(c_{v,r_{v,C}}e^{\lambda\ell_{v,r_{v,C}}}\right).
\tag{Q15}
\]

Sum the radii. For each fixed \(v\), the number of occurrences \((v,C)\) is at most the number of tuple entries \(a\) with \(v\in I_{e_a}\): assign each occurrence to an incident vertex in \(C\); assignments for different \(C\)'s are distinct. Since \(M_v\ge1\), the resulting product is bounded by
\[
\prod_a w_{e_a}.
\tag{Q16}
\]

This pays each kernel increment once per component occurrence. It introduces no factor involving untouched components elsewhere in the volume.

### 5.3 Keep the root mark through the localization sum

For a fixed current root \(i\),
\[
\mathbf1_{\{i\in S_\Gamma\}}
\le
\sum_a\mathbf1_{\{i\in S_{e_a}^V\}}
+\sum_{\substack{C\in\sigma\\v\in I_C}}
\mathbf1_{\{i\in H_{v,r_{v,C}}\}}.
\tag{Q17}
\]

When summing a marked kernel occurrence, its factor \(M_v\) is replaced by \(N_v(i)\). Consequently, the weighted marked sum is bounded by the product in (Q16) times
\[
\sum_a\mathbf1_{\{i\in S_{e_a}^V\}}
+\sum_{\substack{C\in\sigma\\v\in I_C}}\vartheta_v(i)
\le\sum_a q_{e_a}(i).
\tag{Q18}
\]
The last inequality uses the same injective assignment of each \((v,C)\) to an incident tuple vertex.

Combining (Q13), (Q16), and (Q18), the weighted localized cumulant sum is bounded by
\[
2^{n-1}\tau(G)
\left(\prod_a w_{e_a}\right)
\sum_a q_{e_a}(i).
\tag{Q19}
\]

### 5.4 Sum the rooted trees

After the symmetry factor \(1/n!\), marking a tuple vertex turns it into the usual rooted-tree factor \(1/(n-1)!\). Let \(\mathcal T_e\) be the rooted-tree majorant. Its nonnegative recursion is
\[
\mathcal T_e
=\exp\left(2\sum_{f:\,I_f\cap I_e\ne\varnothing}
w_f\mathcal T_f\right).
\]
Condition (Q6) and induction on tree height give
\[
\mathcal T_e\le e^{|I_e|}.
\tag{Q20}
\]
Therefore (Q19), summed over all tuples, is at most
\[
\sum_e w_e q_e(i)\mathcal T_e
\le\sum_e w_e e^{|I_e|}q_e(i)=K_i.
\]
This proves (Q9).

The analogous unrooted absolute sum is bounded by
\(\sum_e w_e e^{|I_e|}\le|\mathcal V|/2\). Thus all rearrangements and the localizer expansions converge normally in finite volume. The scalar interpolation that multiplies every \(V_e\) by a parameter \(t\), initially near \(0\), identifies the connected series with \(\log Z\). Absolute convergence up to \(|t|=1\) gives \(Z=e^F\) at \(t=1\), hence zero-freeness. This is the same identification argument as in the finite-support theorem, now with the additional absolutely summable kernel decorations.

### 5.5 Derivatives and oscillations

Each localized scalar term has genuine current support \(S_\Gamma\), of diameter at most \(L_\Gamma\). The two-direction Cauchy argument of *C-05: normalized components and a direct rooted analytic norm*, DN10–DN12, gives
\[
\sum_j e^{\chi\rho(i,j)}
\|D_iD_jF_\Gamma\|_{\mathrm{op}}
\le\frac{4d_*}{p^2}
e^{\chi L_\Gamma}\sup_D|F_\Gamma|
\]
when \(i\in S_\Gamma\), and zero otherwise. Summing (Q9) proves (Q10). The same normal convergence justifies termwise differentiation.

For (Q11), a term whose support misses \(Q\) has the same value at \(z,z'\). Bound the remaining differences by twice their supremum norm, mark a coordinate in \(Q\), and use (Q9).

## 6. All-order absolute jets with a divided tree weight

The spatial extent in (Q3) bounds a diameter. It does not necessarily bound the length of a tree spanning every current coordinate in a large localization ball.

Assume the current geometry is a \(d\)-dimensional lattice with a fixed finite number of current coordinates per site, so an anchored support of diameter at most \(L\) has at most \(C_d(1+L)^d\) current coordinates. Let \(\tau(i_1,\ldots,i_m)\) be a shortest tree length connecting the indicated current sites in the genuine ambient metric.

For all endpoints in \(S_\Gamma\),
\[
\frac{\tau(i_1,\ldots,i_m)}m
\le\frac{m-1}{m}L_\Gamma\le L_\Gamma,
\tag{Q21}
\]
using the star through \(i_1\).

Let \(0\le\chi<\lambda\), \(\delta=\lambda-\chi>0\). Scalar Cauchy estimates and (Q9) yield

\[
\begin{aligned}
&\sup_{i_1}\sum_{i_2,\ldots,i_m}
e^{\chi\tau(i_1,\ldots,i_m)/m}
\bigl|\partial_{i_1}\cdots\partial_{i_m}F\bigr|\\
&\quad\le
\frac{K_*m!}{p^m}
C_d^{m-1}e^\delta
[d(m-1)]!\,
\delta^{-d(m-1)}.
\end{aligned}
\tag{Q22}
\]

**Proof.** A scalar derivative of order \(m\) of a term is bounded by \(m!p^{-m}\) times its supremum norm. With \(i_1\) fixed, at most \(|S_\Gamma|^{m-1}\) endpoint tuples contribute. Put \(n=d(m-1)\). The remaining factor is bounded using
\[
(1+L)^n e^{-\delta L}
\le e^\delta n!\delta^{-n},
\]
which follows from the exponential series at \(\delta(1+L)\). Sum the weighted root norm.

In \(d=4\), this gives
\[
\text{left side of (Q22)}
\le K_*\,C_\delta^{\,m}(m!)^5p^{-m}.
\tag{Q23}
\]
Indeed \([4(m-1)]!\le4^{4(m-1)}[(m-1)!]^4\).

The divided tree weight in (Q21) is essential for this general quasilocal statement. A kernel layer supported on a radius-\(r\) ball and bounded only by \(e^{-\mu r}\) cannot automatically pay a fixed positive exponent times the tree length spanning all sites in that ball, which grows like its volume. A stronger undivided tree-weight theorem requires an additional stronger spatial hypothesis.

Current-anchored mixed native derivatives may be obtained by additional Cauchy estimates on a uniform retained-data domain. Pure native derivatives of current-independent scalar terms are not controlled by the rooted current norm.

## 7. Exponential localizer tails give an explicit root kernel

Suppose
\[
H_{v,r}\subseteq G_v^{+r},\qquad
\ell_{v,r}=2r,\qquad
c_{v,0}\le M,\qquad
c_{v,r}\le C e^{-\mu r}\quad(r\ge1).
\tag{Q24}
\]
Take \(2\lambda<\mu\), and set \(\nu=\mu-2\lambda>0\). Then
\[
M_v(\lambda)\le M+C\frac{e^{-\nu}}{1-e^{-\nu}},
\]
and
\[
\vartheta_v(i)\le C' e^{-\nu\,\operatorname{dist}(i,G_v)}
\tag{Q25}
\]
with a constant uniform when \(M,C,\nu\) are uniform. For positive distance, membership in \(H_{v,r}\) requires \(r\ge\operatorname{dist}(i,G_v)\), and (Q25) follows by summing a geometric tail. At zero distance use \(\vartheta_v(i)\le1\).

The current root norm has the exact decomposition
\[
K_i=K_i^V+\sum_v \mathcal L_v\,\vartheta_v(i),
\tag{Q26}
\]
where
\[
K_i^V=\sum_{e:\,i\in S_e^V}w_e e^{|I_e|},
\qquad
\mathcal L_v=\sum_{e:\,v\in I_e}w_e e^{|I_e|}.
\]

For the next two corollaries, let \(\Lambda\) be one common ambient unit lattice (or a finite box or ordinary periodic quotient of it), let the active current sites be a subset \(\mathcal I\subseteq\Lambda\), and let every \(G_v\subseteq\Lambda\) be nonempty. Use the ordinary ambient shortest-path metric, including its periodic version on a torus. A fixed finite number of current coordinates per site is allowed and changes only constants. If the base carriers \(G_v\) have overlap multiplicity at most \(q\) and \(\mathcal L_v\le\varepsilon\), then
\[
\sup_i\sum_v\mathcal L_v\vartheta_v(i)
\le \varepsilon C' q C_{\nu,d}.
\tag{Q27}
\]
Choose a nearest point of \(G_v\) to \(i\). At most \(q\) carriers choose any given lattice point, so the sum is bounded by a lattice exponential sum.

If, additionally, every active current root is at distance at least \(b\) from each contributing base carrier, the same shell-tail estimate gives
\[
\sup_i\sum_v\mathcal L_v\vartheta_v(i)
\le
\varepsilon C''q(1+b)^{d-1}e^{-\nu b}.
\tag{Q28}
\]

These estimates pay the response of quasilocal normalized kernels by a spatial convolution of the actual component loads. They do not require an original-birth multiplicity bound. The original physical measures and all old internal contributions are still part of the exact rebased kernels whose bounds enter \(\mathcal L_v\).

The direct potential-root term \(K_i^V\) remains to be controlled. Nor may bounded overlap of the base carriers be inferred merely from eligibility at some earlier scale; it must hold for the components in the chosen present representation.

The lattice sums in (Q27)–(Q28) are on one common unit lattice with a fixed finite coordinate multiplicity. They apply uniformly to subsets, finite boxes, and ordinary periodic tori with the corresponding ambient shortest-path metric. They are not asserted for a mixture of native lattices at different scales, a quotient metric that collapses completed components, or a history-dependent density of coordinates. Such settings require an explicit pushforward to a common lattice and a checked weighted counting measure before these corollaries apply.

## 8. A construction of normalized local approximants

The assumptions above can be obtained from an independently proved localized current map.

Suppose an exact native operator \(\widehat\Pi_v(U)\) is normalized and holomorphic with operator norm at most \(M\) on a Banach ball of radius \(R\). Suppose the current map \(U_v(z)\) is holomorphic and, together with all its local truncations, stays inside a concentric ball of radius \(R_0<R\).

Let \(T_{v,r}z\) keep current coordinates in \(G_v^{+r}\) and replace all others by their base values. This operation preserves a current polydisc. If
\[
\sup_{z\in D}
\|U_v(z)-U_v(T_{v,r}z)\|
\le A e^{-\mu r},
\tag{Q29}
\]
define
\[
\Pi_{v,z}^{[r]}
=\widehat\Pi_v\bigl(U_v(T_{v,r}z)\bigr).
\tag{Q30}
\]

These approximants are normalized, holomorphic, and have the required finite current supports. A Banach-valued Cauchy estimate gives
\[
\|D\widehat\Pi_v(U)\|
\le \frac{M}{R-R_0}
\]
on the inner ball. Integrating along its straight segments proves
\[
\sup_D\|\Pi_v-\Pi_v^{[r]}\|
\le\frac{MA}{R-R_0}e^{-\mu r}.
\tag{Q31}
\]
Subtracting consecutive approximants gives an increment bound of the form (Q24).

This construction retains normalization exactly. It does not approximate the denominator separately or claim that normalized kernel coefficients are current-independent.

The complete actual-model input is (Q29) on a common analytic current/native chart, including fixed integration supports and all native arguments of the rebased kernel. A bound on an entry of a covariance, or an unweighted native operator norm alone, does not prove (Q29).

## 9. Consequence for the C-05 repair

The finite-support requirement in the analytic-product theorem can be replaced by normalized quasilocal kernel expansions. The expanded scalar action has genuine finite current supports term by term, an explicit root norm, a weighted Hessian bound, and the \(m!^5\) current-jet growth with a divided tree weight in four dimensions.

The remaining source verification has a concrete form:

- Obtain the normalized native kernel bound on the exact rebased common domain.
- Prove the current-map tail (Q29), or directly the normalized operator localizer bounds (Q24).
- Verify the component-load condition (Q6) for the full localized potentials, including weighted kernel costs.
- Verify the potential-root load and present carrier geometry needed for (Q26)–(Q28).
- Retain pure native scalar and any other original C-05 requirements separately.
