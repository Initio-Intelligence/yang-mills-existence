# C-05 through normalized-kernel response and block oscillations

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

**Scope:** New proved finite-dimensional lemmas, followed by an explicit conditional route to the C-05 current Hessian budget. This is not an actual-model closure of C-05.  
**Primary purpose:** Replace a possible circular appeal to posterior moment bounds by deterministic bounds on the primitive action, its kernel scores, and its block influences.

## 1. What this route accomplishes

There is a rigorous way to integrate arbitrarily complicated positive internal block laws and obtain a small external Hessian without first proving a moment theorem for those internal laws. It uses the oscillations of the external scores in each block, together with weak interactions between distinct blocks.

The resulting bound is a matrix estimate

\[
\bigl|D_iD_jF\bigr|
\le h_{ij}+\frac14\bigl(A(I-R)^{-1}A^{\mathsf T}\bigr)_{ij}.
\tag{K1}
\]

Here \(A\) is a deterministic matrix of block oscillations of current scores, \(R\) is a deterministic inter-block influence majorant, and \(h\) bounds the direct second derivative. Large current-independent self-actions can be absorbed into the block reference measures; their magnitude never enters the estimate.

The theorem pays for current endpoints and the physical diameter of any freely traversed component. It does not replace physical distances by minimum distances to a component and incorrectly assume the triangle inequality. It also does not discard derivatives of the normalized integration kernel.

All actual-model content lies in proving the stated \(A,R,h\) bounds uniformly for the complete action and its actual current map. In particular, the theorem does not assume a downstream posterior moment conclusion or the coercivity conclusion whose application was supposed to follow from C-05.

## 2. Exact response of a current-dependent normalized kernel

Let \(z\) range over an open subset of a finite-dimensional real current space. Let \(m(dy)\) be a fixed reference measure and let

\[
T_zf=\int w(z,y)f(y)\,m(dy),\qquad
\tau(z)=T_z1>0,\qquad
\nu_z(dy)=\tau(z)^{-1}w(z,y)m(dy).
\tag{K2}
\]

Assume a common integration support, positivity for real \(z\), twice differentiable dependence, and sufficient local domination to justify the derivatives below. If a support or a selector moves, it must first be transported to a common support with every resulting Jacobian and response retained. The following formulas do not authorize differentiating through an unaccounted moving hard boundary.

For a real insertion \(B(z,y)\), put

\[
L(z)=\log \nu_z(e^{B(z,\cdot)})
=\log T_z(e^{B(z,\cdot)})-\log T_z1.
\tag{K3}
\]

Let \(\langle\cdot\rangle_t\) be expectation under the probability proportional to
\(e^{tB(z,y)}w(z,y)m(dy)\). Write

\[
u_i=D_i\log w,\qquad
u_{ij}=D_iD_j\log w,\qquad
A_i^{(t)}=tB_i+u_i.
\]

### Proposition K2. Exact Hessian with the denominator retained

Under the assumptions above,

\[
\begin{aligned}
L_{ij}
={}&\langle B_{ij}+u_{ij}\rangle_1
+\operatorname{Cov}_1(B_i+u_i,B_j+u_j)\\
&-\langle u_{ij}\rangle_0
-\operatorname{Cov}_0(u_i,u_j).
\end{aligned}
\tag{K4}
\]

**Proof.** For an unnormalized positive weight \(e^{V(z,y)}m(dy)\), differentiation of its finite integral gives
\[
D_i\log Z=\langle V_i\rangle,\qquad
D_iD_j\log Z=\langle V_{ij}\rangle+
\operatorname{Cov}(V_i,V_j).
\]
Apply this once to \(V=B+\log w\) and once to \(V=\log w\), then subtract.

In particular, \(B=0\) gives zero identically, as required. Omitting the denominator response in (K4) can destroy this exact cancellation.

Equivalently, with normalized scores
\(s_i=D_i\log(d\nu_z/dm)\) and
\(s_{ij}=D_iD_j\log(d\nu_z/dm)\),
\[
L_{ij}=\langle B_{ij}+s_{ij}\rangle_1+
\operatorname{Cov}_1(B_i+s_i,B_j+s_j),
\]
where normalization implies
\(\langle s_i\rangle_0=0\) and
\(\langle s_{ij}\rangle_0+\operatorname{Cov}_0(s_i,s_j)=0\).

### Proposition K3. An interpolation formula exposing every occurrence of \(B\)

If the required third moments and differentiated expectations are dominated on \(0\le t\le1\), then

\[
\begin{aligned}
L_{ij}
=\int_0^1\bigl[&
\langle B_{ij}\rangle_t
+\operatorname{Cov}_t(B_i,A_j^{(t)})
+\operatorname{Cov}_t(B_j,A_i^{(t)})\\
&+\operatorname{Cov}_t(B,tB_{ij}+u_{ij})
+\kappa_t(B,A_i^{(t)},A_j^{(t)})
\bigr]\,dt.
\end{aligned}
\tag{K5}
\]

Here \(\kappa_t(f,g,h)=\langle(f-\langle f\rangle_t)(g-\langle g\rangle_t)(h-\langle h\rangle_t)\rangle_t\).

**Proof.** Since
\[
L=\int_0^1\langle B\rangle_t\,dt,
\]
differentiate twice in \(z\). The identities
\[
D_i\langle f\rangle_t
=\langle f_i\rangle_t+\operatorname{Cov}_t(f,A_i^{(t)})
\]
and
\[
D_j\operatorname{Cov}_t(f,g)
=\operatorname{Cov}_t(f_j,g)+\operatorname{Cov}_t(f,g_j)
+\kappa_t(f,g,A_j^{(t)})
\]
give (K5).

Formula (K5) preserves the pure-kernel cancellation: every term contains \(B\) or one of its derivatives. Estimating it still requires a connected three-point bound or another adequate norm. Merely writing the formula does not provide that bound. The second-order criterion below uses a different, sometimes less sharp, bound and does not assume such a three-point estimate.

## 3. A comparison and covariance lemma proved from finite-block coupling

Let \(V\) be a finite set of blocks, with \(n=|V|\), and let
\(\mathsf X=\prod_{v\in V}\mathsf X_v\). Assume standard Borel block spaces and probability laws admitting the conditional kernels used below on a common product support. For a real function \(f\), define

\[
\delta_v f
=\sup\{|f(x)-f(x')|:x_w=x'_w\text{ for }w\ne v\}.
\tag{K6}
\]

All oscillations below are finite. For finitely many blocks this implies bounded total oscillation, so additive constants do not create integrability problems.

Use total variation in the convention
\[
\|\lambda-\lambda'\|_{\mathrm{TV}}
=\sup_A|\lambda(A)-\lambda'(A)|
=\frac12\int|p-p'|\,d\eta
\]
when densities exist.

### Lemma K4. One-block exponential tilting

If \(q_t(dy)=e^{tg(y)}q(dy)/q(e^{tg})\), with bounded oscillation \(\operatorname{osc}g\), then

\[
\|q_t-q_0\|_{\mathrm{TV}}
\le \frac{|t|}{4}\operatorname{osc}g.
\tag{K7}
\]

**Proof.** The derivative of the density is
\((g-q_tg)q_t\), so its total variation speed is
\(\frac12 q_t|g-q_tg|\). For a random variable whose range has length \(d\), its variance is at most \(d^2/4\), hence its mean absolute deviation is at most \(d/2\). Therefore the speed is at most \(d/4\). Integrate between \(0\) and \(t\). No small-\(t\) assumption is needed.

### Lemma K5. One-sided comparison

Let \(\mu,\widehat\mu\) have one-block conditional kernels \(P_v,\widehat P_v\). Suppose

\[
\begin{aligned}
\|P_v(\cdot\mid x)-P_v(\cdot\mid x')\|_{\mathrm{TV}}
&\le C_{vw}
&&\text{if only block }w\text{ differs},\\
b_v&=\sup_x\|P_v(\cdot\mid x)-\widehat P_v(\cdot\mid x)\|_{\mathrm{TV}},
\end{aligned}
\tag{K8}
\]

where \(C\ge0\), \(C_{vv}=0\), and \(\|C\|_\infty<1\). Then

\[
|\mu f-\widehat\mu f|
\le \sum_{v,w}\delta_v f\,[(I-C)^{-1}]_{vw}\,b_w.
\tag{K9}
\]

**Proof.** Start any coupling of \(X_0\sim\mu\) and \(\widehat X_0\sim\widehat\mu\). At each step choose a uniform block \(v\) and maximally couple updates from \(P_v(\cdot\mid X)\) and \(\widehat P_v(\cdot\mid\widehat X)\). These updates preserve the two marginal laws. Telescoping through the exterior coordinates gives
\[
\|P_v(\cdot\mid x)-\widehat P_v(\cdot\mid\widehat x)\|_{\mathrm{TV}}
\le b_v+\sum_w C_{vw}\mathbf1_{\{x_w\ne\widehat x_w\}}.
\]
Writing \(p_v^{(r)}=\Pr(X_r^v\ne\widehat X_r^v)\), one obtains
\[
p^{(r+1)}
\le Qp^{(r)}+\frac1n b,\qquad
Q=\left(1-\frac1n\right)I+\frac1n C.
\]
Since \(\|Q\|_\infty<1\),
\[
\limsup_{r\to\infty}p^{(r)}
\le(I-C)^{-1}b.
\]
For every \(r\), telescoping \(f\) over blocks yields
\[
|\mu f-\widehat\mu f|
\le\sum_v\delta_v f\,p_v^{(r)}.
\]
Take the limit superior. This proves (K9). Standard Borel kernels with common dominating measures admit the maximal couplings used here; finite block spaces are an immediate special case.

### Theorem K6. Covariance from block oscillations

With \(\mu,C\) as in Lemma K5, put \(D=(I-C)^{-1}\). Then

\[
|\operatorname{Cov}_\mu(f,g)|
\le\frac14\sum_{v,w}\delta_v f\,D_{vw}\,\delta_w g.
\tag{K10}
\]

**Proof.** Apply (K9) to
\(\widehat\mu_t=e^{tg}\mu/\mu(e^{tg})\).
Its block conditional law is the corresponding one-block tilt of \(P_v\). Lemma K4 gives
\[
b_v(t)\le |t|\delta_vg/4.
\]
Divide the comparison bound by \(|t|\) and let \(t\to0\). The derivative of \(\widehat\mu_t f\) at zero is \(\operatorname{Cov}_\mu(f,g)\).

Only the coefficient matrix of \(\mu\) is used in this proof. A separate Dobrushin hypothesis for every perturbed law \(\widehat\mu_t\) is unnecessary: Lemma K5 is explicitly one-sided. This avoids concealing an unverified uniform perturbation assumption.

The proof is a finite-block form of the Dobrushin comparison method. For broader formulations see the primary paper by Rebeschini and van Handel listed below; no external comparison theorem is needed for the finite statement proved here.

## 4. A primitive influence bound that ignores the size of self-actions

Let

\[
\mu_z(dy)
=Z(z)^{-1}e^{\Phi(z,y)}
\prod_{v\in V}\mu_v(dy_v),
\tag{K11}
\]

where each \(\mu_v\) is any probability measure on its block. The measures may already contain large internal self-actions, hard constraints confined to that block, and positive mixtures of its internal histories.

For \(v\ne w\), define the mixed oscillation

\[
\Delta_{vw}\Phi
=\sup
\bigl|\Phi(x^{v,w})-\Phi(x^{v',w})
-\Phi(x^{v,w'})+\Phi(x^{v',w'})\bigr|,
\tag{K12}
\]

with every other coordinate held fixed. If
\(\Phi=\sum_A\phi_A(z,y_A)\), then

\[
\Delta_{vw}\Phi
\le\sum_{A\ni v,w}\Delta_{vw}\phi_A.
\]

For a common real current domain \(\mathcal D\), let

\[
R_{vw}
=\frac14\sup_{z\in\mathcal D}
\sum_{A\ni v,w}\Delta_{vw}\phi_A(z,\cdot),
\qquad R_{vv}=0.
\tag{K13}
\]

The sums must be finite or justified absolutely; this statement does not create the underlying expansion.

### Proposition K7. \(R\) dominates the conditional influence matrix

For every \(z\in\mathcal D\), the block conditional law of \(\mu_z\) has \(C(z)\le R\).

**Proof.** Changing block \(w\) changes the unnormalized log density in block \(v\) by a function with oscillation at most \(\Delta_{vw}\Phi\). Apply Lemma K4 at \(t=1\).

Terms depending on just one integrated block have zero mixed oscillation between distinct blocks. Thus arbitrarily large self-actions do not directly enter \(R\). This statement does not say that their external derivatives are harmless; those derivatives enter the endpoint matrix and direct Hessian below.

If \(\|R\|_\infty<1\), then
\[
(I-C(z))^{-1}\le(I-R)^{-1}
\]
entrywise, by the nonnegative Neumann series. The covariance estimate is consequently uniform in \(z\).

## 5. The direct current-Hessian theorem

Let \(a(z)\) be a scalar retained factor and define

\[
F(z)=a(z)+\log\int e^{\Phi(z,y)}
\prod_v\mu_v(dy_v).
\tag{K14}
\]

Assume common supports, positivity on the real domain, \(C^2\) dependence, and dominated differentiation on compact subsets of \(\mathcal D\). All statements are in the actual chosen normalized current coordinates. For vector-valued current blocks, the following suprema include unit directions in those blocks.

Suppose the influence majorant \(R\) from Proposition K7 satisfies \(\|R\|_\infty<1\). Set

\[
A_{iv}
=\sup_{z\in\mathcal D}\delta_v(D_i\Phi(z,\cdot)),
\tag{K15}
\]

and choose nonnegative \(h_{ij}\) such that

\[
\sup_{z\in\mathcal D,y}
\bigl|D_iD_j a(z)+D_iD_j\Phi(z,y)\bigr|
\le h_{ij}.
\tag{K16}
\]

### Theorem K8. Deterministic Hessian majorant

With \(D=(I-R)^{-1}\),

\[
\sup_{z\in\mathcal D}
\|D_iD_jF(z)\|_{\mathrm{op}}
\le h_{ij}+\frac14(ADA^{\mathsf T})_{ij}.
\tag{K17}
\]

**Proof.** Differentiation gives
\[
D_iD_jF
=D_iD_j a+\langle D_iD_j\Phi\rangle_{\mu_z}
+\operatorname{Cov}_{\mu_z}(D_i\Phi,D_j\Phi).
\]
The first two terms together are bounded by \(h_{ij}\). Apply Theorem K6 and Proposition K7 to the covariance. For vector current blocks, apply the scalar inequality to arbitrary unit directions and take the supremum.

For any actual external metric \(\rho\), the desired weighted row budget follows from the explicit condition

\[
\sup_i\sum_j e^{\chi\rho(i,j)}
\left[h_{ij}+\frac14(ADA^{\mathsf T})_{ij}\right]
\le\varepsilon.
\tag{K18}
\]

Equation (K18) is the primary form of the criterion. It contains no implicit assumption that a set-distance is a metric. It is a deterministic condition on primitive oscillations and their resolvent, rather than an assumed posterior covariance estimate.

If its constants are uniform in cutoff, volume, admitted history, and current domain, so is the conclusion. If the right-hand side tends to zero with the coupling ceiling, this sector supplies a small Hessian budget.

### 5.1 Optional factorization using a genuine augmented metric

Suppose there is a metric or pseudometric \(d\) on the union of external indices and integrated-block labels, whose restriction to the external indices is \(\rho\). Define

\[
\begin{aligned}
\kappa_\chi&=\sup_v\sum_w e^{\chi d(v,w)}R_{vw}<1,\\
A_{\to,\chi}&=\sup_i\sum_v e^{\chi d(i,v)}A_{iv},\\
A_{\leftarrow,\chi}&=\sup_v\sum_j e^{\chi d(v,j)}A_{jv}.
\end{aligned}
\tag{K19}
\]

Then

\[
\sup_i\sum_j e^{\chi\rho(i,j)}
(ADA^{\mathsf T})_{ij}
\le
\frac{A_{\to,\chi}A_{\leftarrow,\chi}}{1-\kappa_\chi}.
\tag{K20}
\]

**Proof.** The weighted row norm is submultiplicative because the metric satisfies the triangle inequality. Hence
\[
\sup_v\sum_w e^{\chi d(v,w)}D_{vw}
\le\sum_{n\ge0}\kappa_\chi^n
=\frac1{1-\kappa_\chi}.
\]
Use \(d(i,j)\le d(i,v)+d(v,w)+d(w,j)\), then sum successively over \(j,w,v\).

One legitimate construction places a block label at a chosen anchor \(x_v\) in the physical metric. The resulting endpoint norms explicitly pay the distance to that anchor.

The rule \(d(i,v)=\operatorname{dist}(i,Y_v)\), with \(d(v,v)=0\), generally does **not** extend the physical metric. If \(i,j\) lie near opposite ends of a large \(Y_v\), both distances to \(Y_v\) can vanish while \(\rho(i,j)>0\). Substituting that rule into (K20) would recreate the missing free-traversal estimate.

### 5.2 A finite-footprint corollary

Suppose every current index meets at most \(M\) integrated blocks, each block meets at most \(N\) current indices, \(A_{iv}\le a_*\) on those incidences, and their distances to genuine block anchors are at most \(D_*\). Then

\[
A_{\to,\chi}\le Ma_*e^{\chi D_*},
\qquad
A_{\leftarrow,\chi}\le Na_*e^{\chi D_*},
\]

so the covariance contribution to the Hessian row is at most

\[
\frac{MN a_*^2e^{2\chi D_*}}{4(1-\kappa_\chi)}.
\tag{K21}
\]

This does not require decay within an individual block. It pays explicitly for its current footprint and geometric size. The actual proof must establish the incidence counts, physical units, and the weighted inter-block condition.

## 6. A sharper diameter-toll bound for independent blocks

The next result is useful when the completed-component integral factorizes after all terms joining distinct components have been separately controlled.

Let \(\Lambda\) be a fixed-dimensional unit lattice, finite box, or periodic torus with its ordinary ambient lattice graph distance \(\rho\), and let \(I\subseteq\Lambda\) be the active current sites. Let \(Y_v\subseteq\Lambda\) be nonempty pairwise disjoint lattice subsets, with
\[
|Y_v|\le N,\qquad\operatorname{diam}(Y_v)\le D_*.
\]
Suppose the posterior law factorizes over \(v\), so \(R=0\), and
\[
A_{iv}\le a_*e^{-m\,\operatorname{dist}(i,Y_v)}.
\tag{K22}
\]
Let
\[
C_s=\sup_x\sum_{y\in\Lambda}e^{-s\rho(x,y)}<\infty,
\]
uniformly in the finite boxes or tori considered. The proof below uses the ordinary lattice metric; it does not assume that a history-dependent distance with collapsed components has the same growth or triangle properties.

### Corollary K9. Physical weighted row with a paid component diameter

For \(0\le\chi<m\),

\[
\sup_i\sum_j e^{\chi\rho(i,j)}
\frac14(AA^{\mathsf T})_{ij}
\le
\frac14a_*^2 e^{\chi D_*}N\,C_{m-\chi}^{\,2}.
\tag{K23}
\]

**Proof.** For every \(v\),
\[
\rho(i,j)
\le\operatorname{dist}(i,Y_v)+D_*+
\operatorname{dist}(j,Y_v).
\]
This inequality includes the diameter that a false set-distance triangle would omit. Thus
\[
e^{\chi\rho(i,j)}A_{iv}A_{jv}
\le a_*^2e^{\chi D_*}
e^{-(m-\chi)\operatorname{dist}(i,Y_v)}
e^{-(m-\chi)\operatorname{dist}(j,Y_v)}.
\]
For fixed \(v\),
\[
\sum_j e^{-s\operatorname{dist}(j,Y_v)}
\le\sum_{y\in Y_v}\sum_j e^{-s\rho(j,y)}
\le NC_s.
\]
For fixed \(i\), choose a nearest point \(y_v\in Y_v\). Disjointness makes these points distinct, so
\[
\sum_v e^{-s\operatorname{dist}(i,Y_v)}
=\sum_v e^{-s\rho(i,y_v)}
\le C_s.
\]
Combine the three inequalities.

There is no birth-index sum in this lemma. Its input concerns the full score of each present component. Establishing that input from the original construction remains essential.

### 6.1 Explicit collar reserve

Suppose in addition that every active current site \(i\) satisfies
\[
\operatorname{dist}(i,Y_v)\ge r
\quad\text{for every relevant }v.
\]
On the \(d\)-dimensional unit lattice, or a uniformly periodic lattice with its graph metric, there is a constant \(C_{s,d}\) such that
\[
\sum_{\rho(x,y)\ge r}e^{-s\rho(x,y)}
\le C_{s,d}(1+r)^{d-1}e^{-sr}.
\]
Indeed the shell of radius \(n\) has at most \(C_d(n+1)^{d-1}\) sites. Write \(n=\lceil r\rceil+q\), bound
\((n+1)^{d-1}\le C(1+r)^{d-1}(q+1)^{d-1}\), and sum \(q\).

Applying this tail estimate in both sums in the proof of Corollary K9 gives the sharper bound
\[
\sup_i\sum_j e^{\chi\rho(i,j)}
\frac14(AA^{\mathsf T})_{ij}
\le
\frac14a_*^2 e^{\chi D_*}N\,C_{m-\chi,d}^{\,2}
(1+r)^{2(d-1)}
e^{-2(m-\chi)r}.
\tag{K23b}
\]

Thus the two external endpoints supply an explicit collar reserve. The hypothesis concerns the actual active current indices and the actual component in the same physical mesh units. It must not be asserted for an old component that has been erased from the current excluded set without verifying what replaces it.

For a periodic torus, choose the unique shortest coordinate representatives of lattice differences, breaking ties consistently when a side length is even. This injects each distance shell into the corresponding shell of \(\mathbb Z^d\), so the shell constants are uniform in the periods. Restricting the sum to active current sites only decreases it. If the \(Y_v\) overlap with multiplicity at most \(q\), the same proof gives an additional factor \(q\); disjoint interiors alone are not silently substituted for disjoint lattice supports. A fixed finite number of current components or oriented bonds per site can likewise be included in the lattice constant.

### 6.2 How an actual collar estimate would close this numerical part

Suppose actual eligible components satisfy
\[
D_*\le c_D R_k,\qquad N\le C(1+R_k)^d,
\]
and the complete score endpoint amplitude has been proved to satisfy
\[
a_*\le P(g_k^{-1},R_k)\,e^{-c_*R_k}
\tag{K24}
\]
with a fixed polynomial \(P\). Then (K23) is bounded by a fixed polynomial times
\[
e^{-(2c_*-\chi c_D)R_k}.
\]
For \(\chi c_D<2c_*\), this can dominate fixed powers of \(g_k^{-1}\) if \(R_k\) grows faster than \(\log g_k^{-1}\), as in the superlogarithmic collar regime.

This is a concrete sufficient alternative to paying every old birth separately. It does not follow merely from a bound on the number or diameter of components, and an unlocalized \(g_k\)-times-polylogarithm score bound may be insufficient for the physical exponential weight. The actual collar factor in (K24) must be established.

Alternatively, a proved separation \(r\ge c_rR_k\) in (K23b) supplies the needed exponential even if \(a_*\) has only polynomial size. The resulting exponent is favorable when \(2(m-\chi)c_r>\chi c_D\). The same qualification about actual current geometry and all other direct Hessian terms remains.

## 7. A uniform normalized-kernel contour lemma

The smallness of the normalizing mass itself is not an obstruction if the logarithmic variation is controlled relative to a real positive reference.

Let \(\mu\) be any probability measure. Suppose \(\psi(z,y)\) is holomorphic on a common complex parameter domain and
\[
\sup_{z,y}|\psi(z,y)|\le\delta<\log2.
\]
Define
\[
Z(z)=\int e^{\psi(z,y)}\mu(dy),\qquad
q_z(dy)=Z(z)^{-1}e^{\psi(z,y)}\mu(dy).
\]

### Lemma K10. Zero-free relative normalization and bounded scores

One has
\[
|Z(z)-1|\le e^\delta-1<1,
\]
so the branch of \(\log Z\) based at \(1\) exists and
\[
|\log Z(z)|\le-\log(2-e^\delta).
\tag{K25}
\]
Consequently
\[
\ell(z,y)=\psi(z,y)-\log Z(z)
\]
is holomorphic and
\[
|\ell(z,y)|\le
M_\delta:=\delta-\log(2-e^\delta).
\tag{K26}
\]

**Proof.** The first inequality follows from
\(|e^\psi-1|\le e^\delta-1\). The disc \(|Z-1|<1\) is zero-free. The power series for \(\log(1+w)\) gives
\(|\log Z|\le-\log(1-|Z-1|)\), which yields (K25).

If a current direction \(i\) has an admissible complex radius \(r_i\) within this domain, Cauchy's estimate gives
\[
\operatorname{osc}_y(D_i\ell)
=\operatorname{osc}_y(D_i\psi)
\le\frac{2\delta}{r_i}.
\tag{K27}
\]
The scalar \(\log Z\) cancels from the oscillation exactly.

On a valid two-direction contour, second derivatives are bounded by the corresponding Cauchy estimate for \(M_\delta\). For example, if the domain contains
\(|t|/r_i+|s|/r_j<1\) along the two directions, the bidisc of half-radii gives
\[
|D_iD_j\ell|\le
\frac{4M_\delta}{r_ir_j}.
\tag{K28}
\]
These statements apply to current blocks through their complexified unit directions.

For an unnormalized weight
\[
w(z,y)=w(z_0,y)e^{c(z)+\psi(z,y)},
\]
the scalar \(c(z)\) cancels from \(q_z\), regardless of its size. It remains in
\(\log T_z1\). Thus the lemma does not estimate a retained-only scalar in the outer action.

To turn (K27) into the spatial endpoint bound (K22), one needs a proved localized current pullback or appropriate source-localized complex contours. A global contour with a fixed radius bounds individual derivatives but does not by itself yield physical exponential localization.

## 8. Why positivity and small individual attachments are insufficient

Consider one integrated block carrying a fair spin \(\sigma=\pm1\), and external currents \(z_1,\ldots,z_N\). Let
\[
B(z,\sigma)=\varepsilon\sigma\sum_{i=1}^N z_i.
\]
The reference probability is positive, normalized, independent of \(z\), and its integration operator has norm \(1\). Every individual attachment has coefficient \(\varepsilon\). Nevertheless,
\[
F(z)=\log\cosh\!\left(\varepsilon\sum_i z_i\right),\qquad
F_{ij}(0)=\varepsilon^2.
\tag{K29}
\]
The unweighted Hessian row is \(N\varepsilon^2\). The physical weighted row can be larger still.

Theorem K8 detects this exactly: \(R=0\), \(A_{i1}=2\varepsilon\), and the covariance majorant is
\(\frac14 A_{i1}A_{j1}=\varepsilon^2\).

A strictly positive local-spin realization is also available. Let the internal block be a one-dimensional Ising chain of \(N\) spins with probability proportional to
\[
\exp\!\left(\beta_N\sum_{r=1}^{N-1}\sigma_r\sigma_{r+1}\right)
\]
and take \(B=\varepsilon\sum_i z_i\sigma_i\). Then
\[
F_{ij}(0)=\varepsilon^2(\tanh\beta_N)^{|i-j|}.
\]
To verify the covariance formula, use the bijective variables \(\sigma_1\) and \(\eta_r=\sigma_r\sigma_{r+1}\): \(\sigma_1\) is fair and the \(\eta_r\) are independent, with mean \(\tanh\beta_N\).

Taking \(\beta_N=\frac12\log N\), \(N\ge2\), gives
\[
(\tanh\beta_N)^{|i-j|}
=\left(\frac{N-1}{N+1}\right)^{|i-j|}
\ge e^{-2}.
\]
The final inequality follows from
\(\log(1-x)\ge-x/(1-x)\), with \(x=2/(N+1)\), and \(|i-j|\le N-1\).
Each Hessian row is therefore at least \(e^{-2}N\varepsilon^2\). Every internal configuration still has positive probability.

These are counterexamples to a general inference from normalization, positivity, and individually small attachments. They are not admitted Wilson-history counterexamples. In the actual construction, eligible-component size restrictions, source localization, and collar factors may pay this susceptibility. The point is that those payments must be shown. A fixed-component estimate that permits free internal traversal does not make them unnecessary.

## 9. Relation to the actual Balaban construction

LFR II, printed pp.379–380, includes component self-terms in the operation (1.71), constructs a small complex variation, and bounds the normalized operation in (1.75). At pp.391–392, (1.103)–(1.104) integrates the boundary exponential with normalized component operators and leaves retained-field multipliers. [B89-II]

The spatial conventions require care. The connected norm in (1.67) charges full connected-tree length, including connecting paths through a component; it does not declare those paths to have zero length. The later second-exponentiation convention does not require trees to span every interior cube of each already fixed component. Those are different statements. Any comparison with a disconnected exterior-size convention, or any claim that two exterior attachments can be joined through the component at no additional spatial cost, requires a separate checked geometric estimate. The counterexamples in Section 8 test a general inference and are not counterexamples to the actual norm in (1.67).

This supports the form of the proposed analysis. It does not by itself verify (K15), (K18), or (K24) for arbitrary repeated completed-component histories.

For the remaining multiplier \(T'_Y1\), the primary text identifies dependence on the retained raw field restricted to \(Y\). Therefore a physical variation that truly holds that raw field fixed has no multiplier response. This does **not** show that the normalized kernel itself is independent of that variation, nor does it identify the jets of an arbitrary independent-current extension. Formula (K4) must be used unless independence is established in the exact current parametrization.

The following actual-model verifications are still required before this lemma can be used to close the relevant sector:

1. **Exact common-support representation.** The actual completed-component operation must be written with its full positive kernel, all selectors, and all coordinate/Jacobian responses. Any product factorization must be proved for that representation.
2. **Primitive endpoint oscillations.** Obtain \(A_{iv}\) for the full current score, including the kernel response, on a common current/native domain. The bound must concern the full inherited scalar input, not merely one recent vertex.
3. **Direct second derivatives.** Bound the complete \(h_{ij}\), or use a rigorously estimated cancellation-preserving version of (K4)–(K5).
4. **Weak coupling between different integrated blocks.** Verify a uniform influence majorant \(R\), or another proved susceptibility operator. Arbitrary hard constraints joining blocks do not automatically satisfy the criterion.
5. **Physical endpoint geometry.** Pay current footprints and component diameters in the metric required by C-05/HC. Use a genuine augmented metric or the direct matrix condition (K18), not a false minimum-distance triangle.
6. **The rest of C-05.** A real current-Hessian theorem alone does not establish the all-order, native-only, value, and moving-map statements that may be required by C-05.

The determinant and Schur responses of the ordinary old operation are not discarded by any of these formulas. They either belong to the full primitive kernel scores or to an explicitly estimated separate sector.

## 10. Result

The finite-block theorem is proved and noncircular. It supplies a concrete direct alternative to the old per-birth comparison:

\[
\boxed{
\text{complete primitive score bounds}
\;+\;
\text{weak inter-block influences}
\;+\;
\text{paid physical component geometry}
\;\Longrightarrow\;
\text{small current Hessian}.
}
\]

The proof permits arbitrarily large internal self-actions and needs no prior posterior moment bound. Its quantitative footprint/diameter corollaries show exactly how a valid collar estimate could absorb the missing free-traversal cost.

The actual complete-score and geometry bounds for all admitted repeated histories have not been established in this note. C-05 remains open. 

## Sources

- T. Balaban, *Large Field Renormalization. II. Localization, Exponentiation, and Bounds for the R Operation*, Communications in Mathematical Physics **122** (1989), 355–392. [DOI](https://doi.org/10.1007/BF01238433). Relevant printed pages: 379–380 and 391–392.
- P. Rebeschini and R. van Handel, *Comparison Theorems for Gibbs Measures*, Journal of Statistical Physics **157** (2014), 234–281. [DOI](https://doi.org/10.1007/s10955-014-1087-7). The finite comparison argument needed here is proved directly in Section 3.
