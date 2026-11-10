# Quasilocal current pullbacks: a direct rooted scalar estimate

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

Status: proved analytic reduction under explicit map and scalar-norm hypotheses. The hypotheses still have to be matched to the admitted Yang–Mills maps. This note does not close C-05.

## 1. Purpose

A local function of native fields need not be a function of finitely many current coordinates after composition with a background or preparation map. Exponential locality of that map is not exact support. This note supplies an explicit replacement: telescope the composed scalar into genuinely local current functions and estimate the resulting rooted scalar norm.

The scalar can be an input boundary activity or a connected coefficient produced by the normalized-operator theorem in [A direct multi-component theorem for C-05](connected component expansion). In the latter use, its native support must include the parameter dependence of every touched normalized kernel. This is how moving kernels remain present in the argument.

## 2. Setup

Work first on a finite metric lattice \((\Lambda,\rho)\), with constants independent of its size. **In Sections 2–5, native and current sites use the same underlying unit lattice and counting measure.** Distinct finer native meshes or a union of native scales require the separate mixed-incidence condition in Section 5.1; they are not silently covered by a volume-independent lattice constant. Assume

\[
\sup_i\sum_{j\in\Lambda}e^{-s\rho(i,j)}=:Q_s<\infty
\quad\text{uniformly in the lattice for every fixed }s>0.
\tag{QP1}
\]

Polynomial ball growth implies this condition. Scalar coordinates are used below; a fixed finite block dimension changes only numerical constants.

The current domain is the polydisc

\[
D_P=\{z:|z_j|<P\text{ for all }j\}.
\]

Retained parameters \(\xi\) are fixed during current differentiation; every bound below is uniform over their declared common domain.

Let \(U(z,\xi)=(U_x(z,\xi))\) be a holomorphic native-field map. For every carrier \(X\), assume that \(U_X(z,\xi)\) lies in the concentric \(\theta_N R\) subball of a native \(\ell^\infty(X)\) ball of radius \(R\), where \(0<\theta_N<1\). Put

\[
\Delta=(1-\theta_N)R.
\tag{QP2}
\]

The centers of these native balls may depend on fixed retained data. They must not move with \(z\). A carrier-dependent radius is also possible, provided the dimensionless constants used below remain uniform.

Assume the native-to-current endpoint estimate

\[
\sup_{z\in D_P,\,\xi}\sup_x
\sum_j e^{\mu\rho(x,j)}
\|D_jU_x(z,\xi)\|\le L,
\qquad \mu>0.
\tag{QP3}
\]

This is a statement on the whole complex domain. A bound only on real fields is not substituted for (QP3). All fields and derivatives must be in the actual scaled coordinates: physical mesh factors and coupling factors belong in \(L,P,R\) exactly once.

If the native data include field, gradient, and second-order curl/current slots, take their direct sum with its prescribed scaled Banach norm. For example, if slot \(a\) at site \(x\) has physical coordinate \(\widehat U_{x,a}\) and declared positive normalization \(r_{x,a}\), the coordinate entering this note is \(U_{x,a}=\widehat U_{x,a}/r_{x,a}\). The factors \(r_{x,a}\) must contain the actual powers of the mesh and coupling. Equation (QP3) is then a statement about this complete normalized vector and the actual normalized current variable. It does not follow from a bound for only the unscaled field slot.

For each nonempty native carrier \(X\), let \(A_X(u_X,\xi)\) be holomorphic on that native ball, with

\[
\sup |A_X|\le b_X.
\tag{QP4}
\]

The function \(A_X\) may already have had a scalar \(c_X(\xi)\), independent of the current coordinates, subtracted. This allows the theorem to use a genuine native oscillation bound instead of charging a large constant to current derivatives. The omitted scalar remains part of the original outer weight whenever that weight is needed; its convergence and pure retained-data derivatives are not inferred here.

Write \(d_X=\operatorname{diam}_\rho X\). Assume the native rooted scalar norm

\[
N_\chi:=\sup_x\sum_{X:x\in X}b_Xe^{\chi d_X}<\infty.
\tag{QP5}
\]

For a uniform small current Hessian budget, the resulting constant divided by \(P^2\) must tend to zero in the specified coupling regime. Finiteness alone is not that smallness assertion.

## 3. Exact local approximation of the pullback

Let \(X^{[r]}=\{j:\operatorname{dist}_\rho(j,X)\le r\}\), for integers \(r\ge0\), and let \(P_{X,r}z\) reset every current coordinate outside \(X^{[r]}\) to zero. Assume the lattice metric is normalized so that \(X^{[0]}=X\); otherwise use the smallest declared neighborhood in place of \(X\).

### Lemma QP1. Uniform map tail

For \(r\ge0\),

\[
\sup_{D_P,\xi}\|U_X(z,\xi)-U_X(P_{X,r}z,\xi)\|_\infty
\le PL e^{-\mu r}.
\tag{QP6}
\]

**Proof.** Join \(P_{X,r}z\) to \(z\) by the straight segment in \(D_P\). For \(x\in X\), all changed coordinates satisfy \(\rho(x,j)>r\). Integrating the derivative along that segment gives

\[
\begin{aligned}
\|U_x(z)-U_x(P_{X,r}z)\|
&\le P\int_0^1\sum_{j\notin X^{[r]}}\|D_jU_x(z(t))\|\,dt\\
&\le PL e^{-\mu r}.
\end{aligned}
\]

Take the supremum over \(x\in X\). No factor \(|X|\) is needed because (QP3) is a row bound in the native endpoint and the native norm is \(\ell^\infty\).

### Lemma QP2. Analytic scalar tail

Set \(f_X(z,\xi)=A_X(U_X(z,\xi),\xi)\). Then

\[
\sup_{D_P,\xi}|f_X(z,\xi)-f_X(P_{X,r}z,\xi)|
\le b_X a e^{-\mu r},
\qquad a=\frac{PL}{\Delta}.
\tag{QP7}
\]

**Proof.** Banach-space directional Cauchy on the native ball gives \(\|DA_X\|\le b_X/\Delta\) throughout its inner \(\theta_NR\) ball. The segment joining the two native images stays in that inner ball because the ball is convex. Integrating \(DA_X\) along this segment and using (QP6) proves (QP7).

The assumptions concern a fixed complex chart or a Banach ball of scaled coordinates. The proof does not treat a nonconvex gauge manifold as though it were that ball; the actual chart and its margins must be supplied.

## 4. Rooted current scalar norm

Define genuinely local scalar functions

\[
\begin{aligned}
h_{X,0}(z,\xi)&=f_X(P_{X,0}z,\xi)-f_X(0,\xi),\\
h_{X,r}(z,\xi)&=f_X(P_{X,r}z,\xi)-f_X(P_{X,r-1}z,\xi),
\quad r\ge1.
\end{aligned}
\tag{QP8}
\]

They have current support in \(X^{[r]}\), and

\[
f_X(z,\xi)-f_X(0,\xi)=\sum_{r\ge0}h_{X,r}(z,\xi)
\tag{QP9}
\]

normally on the common domain. The bounds are

\[
\|h_{X,0}\|\le2b_X,
\qquad
\|h_{X,r}\|\le ab_X(1+e^{\mu})e^{-\mu r}
\quad(r\ge1).
\tag{QP10}
\]

Let \(0\le\chi<\mu/2\), set \(\nu=\mu-2\chi>0\), and define

\[
C_{\mathrm{loc}}=2+
\frac{a(1+e^{\mu})Q_\nu}{1-e^{-\nu}}.
\tag{QP11}
\]

### Theorem QP3. Native-to-current rooted norm transfer

The localized current scalars satisfy

\[
\sup_i\sum_{X,r:\,i\in X^{[r]}}
e^{\chi\operatorname{diam}(X^{[r]})}
\|h_{X,r}\|
\le C_{\mathrm{loc}}N_\chi.
\tag{QP12}
\]

**Proof.** Since \(\operatorname{diam}(X^{[r]})\le d_X+2r\), the \(r=0\) contribution is at most \(2N_\chi\). For \(r\ge1\), membership of the root implies \(r\ge\operatorname{dist}(i,X)\). Summing the geometric series gives

\[
\begin{aligned}
\sum_{X,r\ge1:\,i\in X^{[r]}}
e^{\chi\operatorname{diam}(X^{[r]})}\|h_{X,r}\|
&\le\frac{a(1+e^\mu)}{1-e^{-\nu}}
\sum_X b_X e^{\chi d_X}e^{-\nu\operatorname{dist}(i,X)}\\
&\le\frac{a(1+e^\mu)}{1-e^{-\nu}}
\sum_x e^{-\nu\rho(i,x)}
\sum_{X:x\in X}b_Xe^{\chi d_X}\\
&\le\frac{a(1+e^\mu)Q_\nu}{1-e^{-\nu}}N_\chi.
\end{aligned}
\]

The middle inequality uses nonempty carriers and
\(e^{-\nu\operatorname{dist}(i,X)}\le\sum_{x\in X}e^{-\nu\rho(i,x)}\).
This proves (QP12).

The displayed constant is deliberately convenient rather than optimal. A uniform analytic tail bound (QP7), with any uniform \(a\), is enough for Theorem QP3; proving it by the derivative bound (QP3) is one sufficient route.

## 5. Identified scalar sum and the current Hessian

In a finite volume, (QP5) implies \(\sum_X b_X\le|\Lambda|N_0\), so the full scalar sum \(\sum_Xf_X\) is normally convergent. Constants \(f_X(0,\xi)\) may be extensive and retained-data dependent. They have not been discarded from the measure: subtracting them here only identifies the current-dependent part.

Define

\[
B(z,\xi)=\sum_X[f_X(z,\xi)-f_X(0,\xi)].
\tag{QP13}
\]

By (QP9)–(QP12), this is a normally convergent local current expansion, not merely a formal Hessian series. On the concentric current \(\theta P\) subdomain,

\[
\sup_i\sum_j e^{\chi\rho(i,j)}|D_iD_j B|
\le
\frac{4C_{\mathrm{loc}}N_\chi}{(1-\theta)^2P^2}.
\tag{QP14}
\]

**Proof.** For each local scalar \(h=h_{X,r}\), use two complex directions: the unit direction at root \(i\), and a phase-chosen direction in its support with magnitudes \(e^{\chi\rho(i,j)}\). The two radii \(p/2\) and \(p/[2e^{\chi\operatorname{diam}(X^{[r]})}]\), where \(p=(1-\theta)P\), fit in the common polydisc. Mixed Cauchy gives

\[
\sum_j e^{\chi\rho(i,j)}|D_iD_jh|
\le4p^{-2}e^{\chi\operatorname{diam}(X^{[r]})}\|h\|.
\]

Sum (QP12). Uniform convergence identifies the derivatives with those of (QP13).

For fixed finite coordinate-block dimension \(d_*\), an operator row bound follows with a factor at most \(d_*\) when the current polydisc is stated in scalar coordinates. Other block-radius conventions require the corresponding fixed norm-conversion factor.

### 5.1 Distinct native meshes: the measure cannot disappear

When native sites and current sites differ, place them in the same physical metric space but retain their actual indices and measures. The map-tail and scalar-tail proofs still apply if (QP3) is correctly formulated in the actual current coordinate derivatives. The safe scalar summability hypothesis is then the direct mixed incidence

\[
\mathfrak N_{\chi,\nu}
=\sup_{i\in\Lambda_{\rm current}}
\sum_X b_Xe^{\chi d_X}
e^{-\nu\operatorname{dist}(i,X)}<\infty,
\qquad \nu=\mu-2\chi>0.
\tag{QP17}
\]

The actual carrier labels, physical measures already included in \(b_X\), and multiplicities occur in this sum once. The proof above gives, directly,

\[
\sup_i\sum_{X,r:\,i\in X^{[r]}}
e^{\chi\operatorname{diam}(X^{[r]})}\|h_{X,r}\|
\le
\left[2+\frac{a(1+e^\mu)}{1-e^{-\nu}}\right]
\mathfrak N_{\chi,\nu}.
\tag{QP18}
\]

Here \(X^{[r]}\) means the current sites within distance \(r\) of the native carrier. A bounded number of fine native sites per current cell is **not** assumed. In particular, replacing the actual fine-site count by the coarse-lattice constant \(Q_\nu\) would be invalid.

One explicit sufficient weighted formulation is available. Choose one actual native anchor \(a_X\in X\) for every carrier, and a positive native anchor measure \(m(x)\). Suppose

\[
\begin{aligned}
Q_\nu^{\rm mixed}
&:=\sup_{i\in\Lambda_{\rm current}}
\sum_{x\in\Lambda_{\rm native}}m(x)e^{-\nu\rho(i,x)}<\infty,\\
N^{\rm anchor}_{\chi+\nu}
&:=\sup_{x\in\Lambda_{\rm native}}
\frac1{m(x)}
\sum_{X:a_X=x}b_Xe^{(\chi+\nu)d_X}<\infty.
\end{aligned}
\tag{QP19}
\]

Then

\[
\mathfrak N_{\chi,\nu}
\le Q_\nu^{\rm mixed}N^{\rm anchor}_{\chi+\nu}.
\tag{QP20}
\]

Indeed, \(\rho(i,a_X)\le\operatorname{dist}(i,X)+d_X\), so each summand in (QP17) is bounded by
\(b_Xe^{(\chi+\nu)d_X}e^{-\nu\rho(i,a_X)}\). Group by anchor and apply (QP19).

This is a sufficient hypothesis, not a license to insert compensating weights. If \(m(x)\) is a fine-cell physical volume, the division by \(m(x)\) in the second line of (QP19) has to be paid by the actual activity estimate. A union of arbitrarily many native scales can make the first line diverge even when each scale separately has the expected Riemann-sum normalization. Rebasing to one genuine current-scale native representation, proving a summable scale weight, or proving (QP17) directly are possible repairs; none follows from changing labels alone.

## 6. A root-oscillation version when no native carrier decomposition is given

For a holomorphic scalar \(F\), let \(\Delta_iF(z)=F(z)-F(z^{i\to0})\). Let \(P_{i,r}\) reset coordinates outside the radius-\(r\) ball about \(i\). Suppose

\[
\Delta_iF(P_{i,r}z)\longrightarrow\Delta_iF(z)
\]

normally, and the local shell increments \(g_{i,r}\) in this telescoping sequence obey

\[
\sup_i\sum_{r\ge0}e^{\chi r}\|g_{i,r}\|\le A.
\tag{QP15}
\]

Then the same argument gives

\[
\sup_i\sum_j e^{\chi\rho(i,j)}|D_iD_jF|
\le4A/[(1-\theta)^2P^2].
\tag{QP16}
\]

Indeed, \(D_iD_j\Delta_iF=D_iD_jF\), and every shell is supported in the radius-\(r\) ball. This is a minimal direct criterion for the weighted row. A bound on unanchored values of \(F\) alone does not imply (QP15).

## 7. Scope of higher jets

If (QP12) or (QP18) is available at \(\lambda>\chi\), polynomial ball growth and a reserve \(\lambda-\chi\) give absolute all-order bounds weighted by the **maximum distance from the root**. Explicitly, suppose the current local scalar expansion has rooted diameter norm at most \(A_\lambda\), and current balls satisfy \(|B(i,t)|\le C_d(1+t)^d\). Put \(\delta=\lambda-\chi>0\), \(p=(1-\theta)P\), and

\[
r_i(j_2,\ldots,j_m)=\max_{2\le a\le m}\rho(i,j_a),
\]

with the maximum defined to be zero for \(m=1\). Then

\[
\sup_i\sum_{j_2,\ldots,j_m}
e^{\chi r_i(j_2,\ldots,j_m)}
|D_iD_{j_2}\cdots D_{j_m}B|
\le
\frac{A_\lambda m!}{p^m}
C_d^{m-1}e^\delta
\frac{[d(m-1)]!}{\delta^{d(m-1)}}.
\tag{QP21}
\]

For the proof, each local coefficient of support diameter \(t\) has at most \(C_d^{m-1}(1+t)^{d(m-1)}\) ordered endpoint choices at a fixed root. Cauchy contributes at most \(m!p^{-m}\) times its scalar norm. The displayed weight is at most \(e^{\chi t}\). Absorb the endpoint count against \(e^{-\delta t}\) using (MC23), then sum the rooted diameter norm. In four dimensions this is bounded by \(A_\lambda C^m(m!)^5p^{-m}\). Here the locality construction itself also requires \(\mu>2\lambda\).

A fixed-weight **Steiner-tree** norm for arbitrary many current endpoints does not follow merely by replacing this maximum with a tree length. A radius-\(r\) local approximation can contain many endpoints whose total spanning-tree length is much greater than \(r\). Such a stronger norm requires a corresponding multivariate locality estimate for the pullback, or a localization expansion carrying a genuine tree cost. The native connected-tree theorem and the present pairwise quasilocal map estimate must not be conflated at this point.

Likewise, current-anchored derivatives do not control an arbitrary added \(H(\xi)\). Native-anchored estimates of the full action must include the scalar values at \(z=0\) and the separate component masses when the application needs them.

## 8. Actual-model matching still required

The useful sufficient input is now explicit:

1. Native scalar activities, including completed-component responses, have the rooted norm (QP5) on a common native ball.
2. The actual current pullback maps that entire current contour into the stated inner native ball.
3. The actual map has the uniform complex endpoint bound (QP3), or the direct analytic tail (QP7), with the physical mesh and coupling normalization used by C-05.
4. The native/current counting measures really permit (QP12), or the direct mixed incidence (QP17) is proved with the actual multiscale multiplicities.
5. The resulting scalar root bound divided by \(P^2\) is uniformly small on the admitted histories.

These premises can replace the false claim that native carriers are exact current supports. They do not prove themselves from real analyticity, an unweighted real endpoint estimate, or the existence of the unmarked RG/R representation.
