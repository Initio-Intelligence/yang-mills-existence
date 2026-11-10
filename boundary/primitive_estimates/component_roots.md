# Physical root sums and exact rebasing

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

Status: supporting theorems proved below; the actual-model C-05 conclusion remains unproved.

## 1. The specific alternative

The repeated-history problem need not be estimated by multiplying the norms of the normalized kernels at every ancestral completion. At a fixed real reference one can put the entire already-integrated history into one positive reference measure. The current dependence is then a single complete density ratio. Integrating more of the history is a conditional expectation of that same ratio. This exact operation has norm one, regardless of the number of earlier steps or the smallness of their masses.

This observation is useful only after the whole density ratio is written correctly. It includes old Gaussian and Schur coefficients, current-dependent native maps, failed-preparation changes of variables, their Jacobians, and any genuinely moving support after its transport to a common support. It does not allow any of these terms to be deleted.

The new quantitative point below is an arbitrary-depth, zero-free complex estimate obtained from a *single complete relative-action bound*. It can be combined with a current-map localization to prove a physical weighted Hessian without an age count. There is no separate analyticity-in-operator-norm assumption on every ancestral kernel. There is still an actual-model obligation: establish that complete pointwise relative-action bound and its present-component localization.

## 2. Exact normalization and arbitrary-depth elimination

Let \((\Omega,\mathcal F,m)\) be a finite-measure or sigma-finite measure space carrying all old continuous fields, discrete preparation labels and history labels to be eliminated. The finite lattice makes the number of variables finite; countably many labels are also harmless under the domination hypotheses below. Let \(D\subset\mathbb C^n\) be an open current/native domain containing a real reference \(0\).

Assume the *complete transported density* \(w_z(\omega)\) has common support, \(w_0\ge0\), and
\[
0<Z_0:=\int w_0\,dm<\infty.
\tag{F1}
\]
Whenever \(w_0=0\), assume \(w_z=0\) for every \(z\in D\). On the positive support write
\[
\frac{w_z(\omega)}{w_0(\omega)}
=e^{c(z)+S(z,\omega)},\qquad c(0)=0,
\tag{F2}
\]
where \(c\) is scalar holomorphic and \(S(\cdot,\omega)\) is holomorphic for almost every \(\omega\). It is sufficient to have this identity almost everywhere for the probability
\[
d\mu_0=Z_0^{-1}w_0\,dm.
\]
The function \(c\) is a real factor at the physical parameters if the original ratio is positive. It stays in the outer density. It is not silently discarded. Its current and native derivatives must be estimated separately whenever nonzero.

### Theorem F1 (complete-history contraction)

Suppose
\[
\sup_{z\in D}\operatorname*{ess\,sup}_{\mu_0}|S(z,\omega)|\le\eta<\log2.
\tag{F3}
\]
Then
\[
Z(z)=\int w_z\,dm=Z_0e^{c(z)}\mu_0(e^{S(z)}),
\tag{F4}
\]
and \(Z(z)\ne0\) on \(D\). The branch
\[
F(z)=\log\frac{Z(z)}{Z_0}-c(z)
=\log\mu_0(e^{S(z)})
\tag{F5}
\]
satisfies
\[
|F(z)|\le A(\eta):=-\log(2-e^\eta).
\tag{F6}
\]
The logarithm is the series branch about \(1\). No lower bound on \(Z_0\) enters (F6).

If \(\mathcal G\subset\mathcal F\) is any retained sigma algebra, the same statement holds fiberwise for
\[
R_{\mathcal G}(z)
=\mathbb E_{\mu_0}[e^{S(z)}\mid\mathcal G],
\tag{F7}
\]
with exactly the same \(\eta\) and \(A(\eta)\). Every chain
\(\mathcal G_q\subset\cdots\subset\mathcal G_1\subset\mathcal F\)
gives
\[
\mathbb E_0[R_{\mathcal G_j}(z)\mid\mathcal G_{j+1}]
=R_{\mathcal G_{j+1}}(z).
\tag{F8}
\]
There is no constant raised to the number of eliminations.

**Proof.** The essential bound gives
\[
|e^{S(z,\omega)}-1|\le e^\eta-1=:q<1.
\]
Expectation and conditional expectation are contractions in \(L^\infty(\mu_0)\). Consequently every expression in (F7), as well as \(\mu_0e^S\), belongs to the closed disk \(|u-1|\le q\). It is nonzero. The power series for \(\log(1+u)\) converges absolutely and normally for \(|u|\le q\), with absolute sum \(-\log(1-q)=A(\eta)\). Dominated integration of holomorphic functions proves holomorphy; on finite coordinate domains this follows directly from Morera and Fubini, or from Cauchy's formula on compact polydiscs and dominated convergence. Conditional versions follow by applying the same argument to a regular conditional law on the fixed reference fiber. Finally (F8) is the tower property. \(\square\)

The statement for conditional laws is understood on common full-measure fibers of \(\mu_0\); in the finite-dimensional application one can use an explicit positive density on each nonzero-mass fiber. A zero-mass fiber need not be assigned a normalized law for the identity of unnormalized measures.

### Corollary F2 (Cauchy without a depth or endpoint factor)

Suppose \(D\) contains \(\{z:\|z\|_\infty<P\}\). For \(\|z\|_\infty\le\theta P\), \(0\le\theta<1\), put \(p=(1-\theta)P\). Then
\[
\sup_i\sum_j|D_iD_jF(z)|\le\frac{4A(\eta)}{p^2}.
\tag{F9}
\]
For directions \(\|v_a\|_\infty\le1\),
\[
|D^mF(z)[v_1,\ldots,v_m]|
\le\frac{m^mA(\eta)}{p^m}
\le\frac{e^m m!A(\eta)}{p^m}.
\tag{F10}
\]

**Proof.** For (F9), Cauchy applied to \(F(z+s e_i+t v)\) on \(|s|,|t|<p/2\) gives \(4A(\eta)/p^2\). Choose the phases of \(v_j\) to align the Hessian entries. For (F10), use \(m\) Cauchy variables of radius \(p/m\); the corresponding translated polydisc lies in the original current domain. The inequality \(m^m\le e^m m!\) follows, for example, by integrating \(\log x\) to lower-bound \(\log m!\). \(\square\)

Finite internal dimension is never an input to these constants. Internal degrees of freedom can grow with the age or the ultraviolet cutoff.

## 3. Why moving normalizers are retained

For a single step let \(K_z(x,dy)=k_z(x,y)m_x(dy)\), with mass
\(\tau_z(x)=K_z1\) and normalized kernel \(P_z=K_z/\tau_z\). Then
\[
\tau_zP_zf=K_zf
\tag{F11}
\]
is the exact identity. If an earlier factor is represented using \(P_z\), the corresponding \(\tau_z\) remains at the point in the joint density at which the identity placed it. Multiplying the actual joint density and applying (F11) restores the unnormalized kernel. Repetition cancels only the normalizers genuinely paired by (F11). It does not declare a normalizer to be constant in \(z\), and it does not move a parent-dependent mass outside a parent integral.

An alternative check uses likelihood-ratio martingales. If
\(R_{\mathcal G_j}=\mathbb E_0[e^S\mid\mathcal G_j]\), the normalized conditional density ratio between two consecutive retained levels is
\[
\frac{R_{\mathcal G_j}}{R_{\mathcal G_{j+1}}}.
\tag{F12}
\]
The product of these ratios telescopes. Estimating every numerator and denominator separately would introduce avoidable repeated constants; using (F8) estimates their exact combined effect.

On the physical real slice the first two derivatives are
\[
\begin{aligned}
D_iF&=\langle S_i\rangle_z,\\
D_iD_jF&=\langle S_{ij}\rangle_z
 +\operatorname{Cov}_z(S_i,S_j),
\end{aligned}
\tag{F13}
\]
where \(\langle\cdot\rangle_z\) has density \(e^S/\mu_0e^S\). All kernel and Jacobian responses sit in \(S_i,S_{ij}\). Thus (F13) includes both the direct Hessian and the moving-law covariance. It supplies no covariance estimate by itself. The complex estimate (F6), followed by Cauchy, is an independent way of bounding their combined value.

If only the first derivative is desired, conditional expectation gives the genuine score contraction
\[
\inf_a\|\mathbb E_0[S_i\mid\mathcal G]-a\|_\infty
\le\inf_a\|S_i-a\|_\infty.
\tag{F14}
\]
There is no analogous unconditional contraction of the Hessian: its covariance term in (F13) is indispensable.

## 4. A local relative action can be substituted for a normalized operator tail

This section proves a concrete sufficient localization statement. It does not assume that a bound on one scalar test automatically controls every test in an operator norm.

Let \(Y\) be a finite set of native sites associated to one present component. Let \(\mathcal B\) be the Banach space of its normalized native field/gradient/current coordinates, with supremum norm. Let \(U\subset\mathcal B\) be an open domain. For each \(\xi\in U\), assume a complete ratio as in (F2) with
\[
\sup_{\xi\in U,\omega}|S(\xi,\omega)|\le\eta<\log2.
\tag{F15}
\]
Set \(G(\xi)=\log\mu_0e^{S(\xi)}\). Thus \(|G|\le A(\eta)\).

Let \(\Phi:D_P\to U\) be the actual holomorphic native map from current variables on a unit four-dimensional lattice \(I\). For a radius \(r\ge0\), let \(z^{[r]}\) agree with \(z\) on
\(N_r(Y)=\{i:\rho(i,Y)\le r\}\)
and vanish elsewhere. This truncation is in \(D_P\) automatically. Write
\(\Phi_r(z)=\Phi(z^{[r]})\).

Assume every \(\Phi_r(z)\), \(\Phi(z)\), and segment needed below stays at native distance at least \(\delta>0\) from \(U^c\), and
\[
\|\Phi_r(z)-\Phi_{r-1}(z)\|_{\mathcal B}
\le T e^{-\mu r},\qquad r\ge1,
\tag{F16}
\]
uniformly on the *full complex current polydisc*. Also assume \(\Phi_r\to\Phi\) uniformly. These are estimates for the actual current map and its joint native margin, not assumptions about physical values alone.

### Theorem F3 (localized scalar after complete-history averaging)

Define
\[
f_0(z)=G(\Phi_0(z)),\qquad
f_r(z)=G(\Phi_r(z))-G(\Phi_{r-1}(z))\ (r\ge1).
\tag{F17}
\]
Then
\[
G(\Phi(z))=\sum_{r\ge0}f_r(z),
\tag{F18}
\]
normally on smaller current polydiscs, with
\[
\|f_0\|\le A(\eta),\qquad
\|f_r\|\le\frac{A(\eta)T}{\delta}e^{-\mu r}\quad(r\ge1).
\tag{F19}
\]
Each \(f_r\) depends only on the current variables in \(N_r(Y)\), and
\[
\operatorname{diam}\operatorname{supp}f_r
\le\operatorname{diam}Y+2r.
\tag{F20}
\]

**Proof.** Cauchy in a native direction gives
\(\|DG(\xi)\|_{\mathcal B^*}\le A(\eta)/\delta\)
on the stipulated common interior. Integrate this derivative along the segment from \(\Phi_{r-1}(z)\) to \(\Phi_r(z)\) and use (F16). The resulting series converges uniformly by (F19); its partial sums telescope to \(G\circ\Phi_r\), which tends to \(G\circ\Phi\). The current supports and (F20) follow from the definition of truncation. \(\square\)

The whole history has been averaged before this localization. In particular no normalized-kernel increment is multiplied once per historical occurrence, and there is no requirement to analytically apply a kernel to an arbitrary incoming Banach-algebra element. The actual function integrated is exactly the complete relative density.

One elementary way to prove (F16) is to prove on the same complex domain a native-to-current row bound
\[
\sup_{y\in Y}\sum_{i:\rho(i,Y)>r}
P\|D_i\Phi(y;z)\|
\le T'e^{-\mu r}.
\tag{F21}
\]
Integration along the segment between consecutive current truncations yields (F16), with adjusted constants. The physical mesh factors must be included in the native norm in (F21); they cannot be inferred from unweighted raw derivatives.

## 5. Physical root sums for present components

Here is a rigorous quantitative consequence if the previous theorem can be established for the actual present components. It makes explicit which geometric toll has to be paid.

Let \(\{Y_v\}\) be pairwise disjoint, nonempty subsets of the *unit current lattice*. Suppose the unit lattice has uniform polynomial growth (a finite box or torus is sufficient). For every component obtain a decomposition (F17)–(F20), with a common \(\mu\), and set
\[
a_v=A(\eta_v)\max(1,T_v/\delta_v).
\]
Assume \(a_v\le a_*\) and that for every active current site \(i\) and relevant \(v\),
\[
\operatorname{diam}Y_v\le D_*R_v,
\qquad \rho(i,Y_v)\ge c_*R_v.
\tag{F22}
\]
The second condition is the actual shielding collar. Fix \(\lambda>0\) so that
\[
s:=\mu-2\lambda-\lambda D_*/c_*>0.
\tag{F23}
\]

### Theorem F4 (depth-free current-root estimate)

For the sum \(B(z)=\sum_vG_v(\Phi_v(z))\), the localized terms satisfy
\[
\sup_i\sum_{v,r:\ i\in N_r(Y_v)}
e^{\lambda\operatorname{diam}N_r(Y_v)}\|f_{v,r}\|
\le C_{\mu,\lambda}\,a_*\,
\sup_i\sum_ve^{-s\rho(i,Y_v)}.
\tag{F24}
\]
The last sum is bounded by
\[
C_s:=\sup_x\sum_y e^{-s\rho(x,y)},
\tag{F25}
\]
uniformly in the total volume. Consequently
\[
\sup_i\sum_j e^{\lambda\rho(i,j)}|D_iD_jB(z)|
\le\frac{4C_{\mu,\lambda}C_s a_*}{(1-\theta)^2P^2}
\tag{F26}
\]
on \(\|z\|_\infty\le\theta P\). A finite block-coordinate factor can be inserted when using Lie-algebra coordinates.

**Proof.** Put \(d=\rho(i,Y_v)\). Only \(r\ge d\) can contribute to a root at \(i\). From (F19) and (F20),
\[
\sum_{r\ge d}e^{\lambda\operatorname{diam}N_r(Y_v)}\|f_{v,r}\|
\le C_{\mu,\lambda}a_ve^{\lambda\operatorname{diam}Y_v}
e^{-(\mu-2\lambda)d}.
\]
Use (F22) to obtain the summand in (F24). For fixed \(i\), choose a nearest lattice site \(y_v\in Y_v\). Disjointness makes all chosen sites distinct. Thus
\(\sum_ve^{-s\rho(i,Y_v)}\le\sum_y e^{-s\rho(i,y)}\),
which proves (F25). Finally apply the phase-aligned two-direction Cauchy estimate termwise. For a term containing both endpoints, \(\rho(i,j)\le\operatorname{diam}\operatorname{supp}f_{v,r}\). Sum the scalar root bound before differentiating, so no endpoint-volume factor is introduced. \(\square\)

The statement can incorporate a fresh uniform collar suppression: if every \(d\ge r_0\), spend only part of \(s\) in (F25), giving an additional factor \(e^{-(s-s')r_0}\) for any \(0<s'<s\).

### Important limits of Theorem F4

1. Pairwise disjoint components on mixed fine lattices need not have distinct current lattice representatives. The proof of (F25) then fails. The theorem requires grouping into actual present components or an explicit density estimate. It does not silently cancel \(L^{4(k-b)}\).
2. If two current endpoints may lie next to opposite ends of one component, the diameter toll in (F22) must be paid. A distance to a set is not a substitute for a genuine metric.
3. If present kernels interact, the reference law generally does not factorize into \(\prod_v\mu_{v,0}\). Then (F24) for a sum of independent component logarithms is not the correct formula. The crosspotential must be retained in one joint component, or treated by the connected expansion with its true incidence load. The theorem does not hide a cross-component interaction in a product kernel.
4. A current-independent scalar \(c_v(\xi)\) can still have nonzero native jets. Theorem F4 controls the current-rooted part. C-05's full native-rooted completion test needs the scalar factors too.

## 6. Exact last-consumption rebasing

There is an algebraically safe meaning to assigning an ancestral record to its last consuming operation. For a complete joint reference probability \(\mu_0\), marginalize every already-consumed variable first and set the new density ratio equal to the conditional expectation (F7). This is an *identity of reduced densities*, and (F8) says that the order in which those variables were integrated has no effect. It does not preserve the separate identities of arbitrary terms in the logarithmic expansion.

If (F3) was proved for the complete ancestor ratio, every such rebasing retains (F6) without an age penalty. If the proof is only of separate bounds \(|S_t|\le\eta_t\) for each chronological increment, the immediately justified bound is only
\[
\eta\le\sum_t\eta_t.
\tag{F27}
\]
There is no automatic improvement from \(\sum_t\eta_t\) to \(\sup_t\eta_t\). The tower property removes repeated *normalization amplification*, but it cannot prove summability of primitive responses.

This distinction is useful in deciding what primary-source estimate is needed. One should seek a bound for the complete ratio at the current consuming component, rather than assume a per-step small number survives arbitrarily many steps. If that current complete ratio is controlled on a domain indexed only by the present component, Theorems F1–F4 give the needed analytic transfer without retaining all original births.

## 7. What the cited sources does and does not currently establish

Bałaban, *Large Field Renormalization II*, CMP **122** (1989), 355–392, gives a relevant starting point on printed pp.379–380, equations (1.71)–(1.75). It says that in the component operation only the quadratic form and the complete selfaction \(V(X^-)\) depend on the independent \((U,J)\) continuation. It expands this dependence about a real regular configuration. The resulting small complex correction \(\sigma\) is bounded uniformly on the internal integration variables, and positivity of the real reference density gives the normalized operator estimate (1.75). This is exactly a relative-density mechanism of the form (F2), not merely analyticity of a single scalar output.

The same passage says that \(V(X^-)\) contains boundary terms from all earlier renormalization steps and that its variation creates a connection to the indicated exterior boundary. It invokes the earlier resummation of those connections. This is substantive evidence for seeking the full present-component ratio. It is not, in the material verified here, a displayed uniform physical-current root norm for every repeated alternative representation.

On pp.391–392, (1.103)–(1.104), the source integrates the *whole boundary exponential* under normalized completed-component operations, retains the scalar masses, and gives a reduced density. The scalar masses depend on the retained raw field on the completed component. The new boundary estimate permits traversal of each fixed component without an internal tree cost. Therefore applying Theorem F4 needs either:

- a pointwise complete relative-action estimate for the new joined present component, with its diameter/collar paid and all altered determining data admitted on one contour; or
- a complete interaction list for the resummed boundary with the two connected-expansion incidence sums verified.

Neither the tower property nor the displayed source-free scalar estimates establish those inputs by themselves.

The source matching must also preserve the ordinary quadratic response. With the integrated indices first,
\[
G=K_{II}^{-1},\quad S=K_{OO}-K_{OI}GK_{IO},\quad Ea=(-GK_{IO}a,a),
\]
the exact differential is
\[
D[-\tfrac12a^\mathsf TS a]
=-\tfrac12(Ea)^\mathsf T(DK)(Ea).
\tag{F28}
\]
Thus a shared old support does not imply that its coefficient is current-independent. All contributions in (F28) belong to the complete \(S(z,\omega)\) in (F2) unless an exact recombination proves their cancellation.

## 8. Conclusion for the conditional estimate

The new usable result is a normalization-stable, arbitrary-depth transfer theorem on the full complex contour, together with an explicit present-component localization and physical weighted Hessian estimate. It can replace products of ancestral normalized-kernel bounds if the full primitive ratio is controlled after all factors are recombined.

The unproved actual-model step is now particularly sharp: for every admitted current consuming component, prove a bound of the form (F3), or its localized form (F15)–(F21), for the complete actual density ratio, including every earlier Gaussian/Schur response, failed-preparation Jacobian and current map. It must be a bound on the full joined history, with mixed-mesh multiplicities accounted for. The source supplies a positive-reference ratio mechanism at (1.71)–(1.75), but the all-history physical-current version has not been verified here.

No actual Wilson counterexample was found. These arguments do not close C-05, do not close C-06's actual application, and do not constitute a Yang–Mills existence proof.
