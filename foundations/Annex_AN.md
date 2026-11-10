# Direct boundary derivatives, all-order summation and explicit application gates

**Annex AN.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 1. Target and the alternative considered

The original C-05 statement is to establish the same local derivative bounds for the actual B and boundary-induced activities, including collars, constraints and current-coordinate dependence. It requires constants independent of total volume and hidden carrier distance, with any source formula not verified here retained as a premise. Its catalogue dependency is C-01.

One sufficient way to establish the boundary contour and carrier estimates is a prepared joined reconstruction theorem, with arbitrary complex decoupling parameters. That is stronger than the input required for the derivative argument below. The argument uses the true unlocalized current-to-background map, its common complex contour, and a one-endpoint bound for each primitive boundary activity. It requires no new complex decoupling identity for that map.

This distinction is useful only if the true map is actually checked. In particular, the normalized reconstructed-current restrictions of CMP119 (2.37), the independent-current extension, the fine collars, the fixed coordinate map and the boundary relocation remain part of the application. They cannot be replaced by an estimate for an unrelated scalar analytic function.

### 2. Source estimates for the direct product-domain shortcut

CMP119, printed pp.261–262, defines the primitive B functions on a multiscale domain containing the original field and independent current, the reconstructed fields and currents, local gauge representatives, and complex relative fields. The source's full primitive carrier bound is (2.42). The component-resummed alternative on p.262 has a weaker carrier weight and is not silently substituted for the full primitive bound.

Printed p.276 is stronger than a statement of primitive analyticity. It explicitly assigns the already localized fluctuation expressions, including those arising from inherited B by the transformations corresponding to CMP109 (3.6)–(3.7), to the product domain (3.43). Its current-variable factor is

\[
 \{A:\operatorname{supp}A\subset Y\cap\Lambda_{k+1}^{(k)*},
                \ |A|<C_1p_1(g_k)\}.
 \tag{BC16.1}
\]

The following paragraph on p.277 describes the use of the decreasing multiscale margins, inherited B bounds, heterogeneous Wilson coefficients and the full relocation action. Thus (3.43), if its radius were matched to the actual current support, would be a genuine direct source input. There would be no reason to re-prove every internal reconstruction solely to differentiate the final functions.

The radius identification is not established. CMP119 p.265 gives the unprimed fluctuation cutoff through

\[
 \delta_k=(A_1/A_0)g_kp_0(g_k),\qquad
 P_k=\delta_k/g_k=A_1(\log g_k^{-2})^{p_0}.
 \tag{BC16.2}
\]

The occurrence of an apparent polynomial/constant typo in the first-step formula on p.247 does not define the symbol in (3.43). In CMP116 the precursor domain (1.34) instead has the absolute current radius \(\epsilon_1/g_k\); CMP119 changes that domain at its multiscale boundary. A later LFR polynomial with exponent \(p_1<p_0\) belongs to a primed preparation threshold and cannot cover (BC16.2) by increasing a fixed coefficient. If that later polynomial were inserted in (BC16.1), the radius-to-support ratio would tend to zero.

Consequently this note does **not** infer a full-support current contour from (BC16.1), nor enlarge its radius by analytic continuation without estimates. Its alternative is the true-map endpoint theorem below. See CMP119, pp.247, 261, 276 and 277.

### 3. A finite-volume endpoint theorem

#### 3.1 Hypotheses and notation

Let \(I\) be the current free-bond coordinate set, with a fixed number \(D\) of scalar Lie-algebra coordinates per bond. Distances are periodic lattice distances in current units. All constants below may depend on \(D\), dimension and the fixed localization geometry, but not on the number of coordinates or torus volume.

Let \(F_X(z,\eta)\) be the pullback of one primitive activity. The symbol \(X\) records its original carrier and old scale. The current field is \(z\); \(\eta\) records the admitted native background and independent-current variables. Old history selectors and old real fluctuation coordinates are fixed input parameters. If the actual source operation changes their arguments, that change is part of \(F_X\), not a reason to suppress its derivative. Consider the simultaneous contour

\[
 \|z\|_\infty<2P,
 \qquad \eta\in\mathcal D^+.
 \tag{BC16.3}
\]

Here the sup norm is a scalar-coordinate norm with a fixed conversion from the Lie-algebra norm. The actual support is contained in \(\|z\|_\infty\le P\). In \(\eta\), use a smaller domain \(\mathcal D\) with fixed positive native radii to the boundary of \(\mathcal D^+\). All the following estimates must hold on the full larger contour.

Associate to \(X\) a nonempty set \(S_X\) of current-unit cells covering its physical carrier. Write

\[
 d_X(i)=\operatorname{dist}(i,S_X),\qquad
 D_X=\operatorname{diam}(S_X).
\]

Assume the **one-endpoint gradient estimate**

\[
 |\partial_iF_X(z,\eta)|
 \le \frac{K_X\vartheta_X}{P}\,e^{-c d_X(i)}
 \quad\hbox{on (BC16.3)},
 \tag{BC16.4}
\]

where \(c>0\) is fixed and \(K_X,\vartheta_X\ge0\). The coordinate \(i\) includes its Lie-algebra component; changing to block norms changes fixed constants only. No assumption that \(F_X\) depends on only finitely many current coordinates near \(X\) is made. Its dependence can propagate through the actual minimizing map.

For \(m\) current positions let \(\tau(i_1,\ldots,i_m)\) denote minimum spanning-tree length in the periodic current metric, with \(\tau(i)=0\).

#### Proposition BC16.1 — pointwise jets from one endpoint

For \(\|z\|_\infty\le P\), \(\eta\in\mathcal D^+\), and every \(m\ge1\),

\[
 |\partial_{i_1}\cdots\partial_{i_m}F_X|
 \le K_X\vartheta_X\,(m-1)!
       (2/P)^m
       e^{-c\max_s d_X(i_s)}.
 \tag{BC16.5}
\]

**Proof.** Choose any of the \(m\) differentiated coordinates as the first derivative. Estimate that derivative by (BC16.4). A simultaneous scalar polydisc of radius \(P/2\) about the real point lies in (BC16.3). Apply the multivariable Cauchy formula to the remaining \(m-1\) derivatives. The product of the repeated-coordinate factorials is at most \((m-1)!\). This yields the bound with \(e^{-cd_X(i_s)}\) for every chosen first coordinate. Mixed derivatives commute, so take the minimum of these bounds. The harmless factor 2 in (BC16.5) also covers \(m=1\). No power of \(|I|\) occurs. \(\square\)

For \(m=2\), the estimate gives in particular

\[
 |\partial_i\partial_jF_X|
 \le \frac{4K_X\vartheta_X}{P^2}
 e^{-\frac c2(d_X(i)+d_X(j))}.
 \tag{BC16.6}
\]

This is the precise use of mixed-derivative symmetry: a one-endpoint estimate is sufficient for a two-endpoint Hessian bound. It does not manufacture a missing endpoint estimate for the actual map.

#### Proposition BC16.2 — a weighted Hessian row

For \(0<\gamma<c/2\), set \(t=c/2-\gamma\). There is a fixed current-lattice counting constant \(N_4(t)\) such that

\[
 \sum_j e^{\gamma\rho(i,j)}
       |\partial_i\partial_jF_X|
 \le\frac{4N_4(t)K_X\vartheta_X}{P^2}
       |S_X|e^{\gamma D_X}e^{-t d_X(i)}.
 \tag{BC16.7}
\]

For example one may take a fixed bond-counting constant times
\((1+2/(e^t-1))^4\) for \(N_4(t)\).

**Proof.** Connecting each bond to a nearest point of \(S_X\) gives
\(\rho(i,j)\le d_X(i)+D_X+d_X(j)\), with fixed endpoint constants absorbed in the counting convention. Multiply (BC16.6) by the requested weight. For each \(j\), assign a nearest cell of \(S_X\). The sum of \(e^{-td_X(j)}\) is at most \(|S_X|N_4(t)\). The same argument works on a torus, since a periodic lattice shell contains no more points than the corresponding covering-lattice shell up to a fixed bond convention. \(\square\)

The carrier factor in (BC16.7) is explicit. It must be summed; it is not called a constant independent of carrier size before that summation.

### 4. Old-scale and carrier sums, including all orders

#### 4.1 Concrete sufficient source majorants

Set \(a=k-j\ge0\) for a primitive activity at old scale \(j\). Let \(n(X)\) be its equivalent cube-edge tree length, after the fixed comparison with the source's \(d_j(X)\). Assume

\[
 K_X\le K\,e^{-\kappa n(X)},\qquad
 \vartheta_X\le\vartheta_k(1+a)^b e^{-\Gamma a}.
 \tag{BC16.8}
\]

The primitive carrier encoding gives at most \(B A^n\) carriers of length \(n\) rooted at any one old localization cell. A root means a fixed chosen incident old cell of the carrier; overcounting all such roots only increases the bound. In current units that old grid has mesh \(ML^{-a}\). Thus, for any fixed \(u>0\),

\[
 \sup_i\sum_{r\text{ at age }a}e^{-u\rho(i,r)}
 \le C_{M,u}L^{4a}.
 \tag{BC16.9}
\]

To prove (BC16.9), divide the current lattice into unit cells. The number of old roots in each such cell is at most \(C_M L^{4a}\). The current-cell exponential sum is finite uniformly on periodic tori. This proof does not count all old roots in the entire volume without an anchor.

A carrier of tree length \(n\) has

\[
 D_X\le C_M(n+1),\qquad
 \#\{i:d_X(i)\le R\}\le C_M(n+R+1)^4.
 \tag{BC16.10}
\]

The actual old carrier is smaller by \(L^{-a}\); discarding that improvement gives (BC16.10). The estimate follows by covering the old carrier by a ball of radius \(C_M(n+1)\) in current units. It is a counting estimate, not a claim that a ball is an admissible polymer carrier with exponential-volume weight.

The exponent \(\Gamma\) must exceed \(4\log L\), so that

\[
 S_{b,\Gamma}=\sum_{a\ge0}(1+a)^b
                  e^{-(\Gamma-4\log L)a}<\infty.
 \tag{BC16.11}
\]

These inequalities are deliberately stated as source application requirements. The primitive carrier count is proved by the usual bounded-degree tree encoding. The missing part is to prove (BC16.4) and the age factor in (BC16.8) for the actual complete pullback; neither follows from the root count.

#### Theorem BC16.3 — anchored all-order derivative kernels

Assume (BC16.3)–(BC16.4) and (BC16.8)–(BC16.10), with \(\Gamma>4\log L\). Fix the source carrier parameters with \(\kappa>\log A+2\). If necessary decrease the available endpoint rate \(c\), after those parameters are fixed, so that the fixed losses \(cC_M\) and the endpoint convention leave a positive carrier reserve. This is always possible because an endpoint estimate with rate \(c_0\) also holds with every smaller positive rate. Fix \(0<\sigma<c/8\). Then there is a fixed \(C\), independent of \(m,k\), volume and history, such that the normalized interaction

\[
 W(z,\eta)=\sum_X[F_X(z,\eta)-F_X(0,\eta)]
 \tag{BC16.12}
\]

satisfies, for \(m\ge1\),

\[
 \boxed{
 \sup_{i_1}\sum_{i_2,\ldots,i_m}
 e^{\sigma\tau(i_1,\ldots,i_m)/m}
 |\partial_{i_1}\cdots\partial_{i_m}W|
 \le C^{m+1}(m!)^5\,
        K\vartheta_k S_{b,\Gamma}P^{-m}.
 }
 \tag{BC16.13}
\]

The finite-volume sum defines (BC16.12) directly. The estimates also justify normal convergence of its anchored differentiated sums and passage to expanding volumes whenever the primitive functions themselves are consistently embedded.

**Proof.** We give the counting detail because it controls the factorial exponent. For a fixed \(X\), put
\(R=\max_s d_X(i_s)\). Connecting all positions through nearest points in \(S_X\) gives

\[
 \tau(i_1,\ldots,i_m)\le 2mR+mD_X,
 \tag{BC16.14}
\]

after a fixed enlargement of the endpoint convention, if necessary. Hence the product of the weight in (BC16.13) and the exponential in (BC16.5) is bounded by

\[
 e^{\sigma D_X}e^{-(c-2\sigma)R}.
\]

Set \(v=(c-2\sigma)/2>0\). Split this last exponential into
\(e^{-vd_X(i_1)}e^{-v\max_{s\ge2}d_X(i_s)}\). For \(m=1\) the empty maximum has value zero. The exact layer-cake identity

\[
 e^{-v\max_{s\ge2}d_X(i_s)}
 =\int_{\max_{s\ge2}d_X(i_s)}^\infty
            v e^{-vR'}\,dR'
\]

and (BC16.10) give

\[
 \sum_{i_2,\ldots,i_m}
 e^{-v\max_{s\ge2}d_X(i_s)}
 \le C_M^{m-1}\int_0^\infty v e^{-vR'}
                 (n+R'+1)^{4(m-1)}dR'.
 \tag{BC16.15}
\]

For a chosen root \(r\) of \(X\),
\(d_X(i_1)\ge\rho(i_1,r)-C_M(n+1)\).
Thus root summation is controlled by (BC16.9), at the cost of
\(e^{vC_M(n+1)}\). The factor \(e^{\sigma D_X}\) has another fixed exponential cost in \(n\). Choose \(\kappa\) leaving a positive rate \(\lambda\) after both costs and the entropy \(A^n\). The old-age sum is (BC16.11). Apart from constants to the power \(m\), the remaining joint size integral is

\[
 \sum_{n\ge0}e^{-\lambda n}
 \int_0^\infty v e^{-vR'}(n+R'+1)^{4(m-1)}dR'.
 \tag{BC16.16}
\]

Let \(a_*\) be half the minimum of \(\lambda,v,1\), and let
\(r_m=4(m-1)\). Split off \(e^{-a_*(n+R')}\) from the exponential. The exponential power series implies

\[
 (n+R'+1)^{r_m}e^{-a_*(n+R')}
 \le e^{a_*}r_m!a_*^{-r_m}.
\]

The remaining geometric sum and integral are finite fixed constants. Consequently (BC16.16) is at most \(C^{m+1}(4(m-1))!\). The multinomial inequality
\((4m)!\le4^{4m}(m!)^4\), together with the Cauchy factor \((m-1)!\) in (BC16.5), gives (BC16.13). The Lie-algebra component multiplicities are at most \(D^{m-1}\) and are absorbed into \(C^m\). Absolute convergence permits the differentiated sum. \(\square\)

In dimension \(d\), the same proof gives the factorial power \(d+1\). The value five is not an uncontrolled order-dependent exponent.

For \(m=2\), (BC16.13) gives a weighted Hessian row with weight \(e^{\sigma\rho(i,j)/2}\). Alternatively (BC16.7) gives a sharper explicit second-order constant. In either form, a bounded \(K\vartheta_k\) and \(P_k\to\infty\) make the Hessian budget arbitrarily small. If the primitive value prefactors vary among the sectors, the right side is summed over the finitely many sector classes before choosing the common coupling ceiling.

#### 4.2 Local value densities and native external jets

On a finite lattice the exact radial identity is

\[
 W(z,\eta)=\sum_i b_i(z,\eta),\qquad
 b_i=z_i\int_0^1\sum_X\partial_iF_X(tz,\eta)\,dt.
 \tag{BC16.17}
\]

It supplies a spatially anchored value budget

\[
 \sup_i|b_i|\le C K\vartheta_k S_{b,\Gamma}
 \quad(\|z\|\le P).
 \tag{BC16.18}
\]

This follows from the same root sum with \(m=1\). The density is quasilocal; it is not asserted to have exact compact carrier support. Its derivatives are controlled by (BC16.13) and differentiation of (BC16.17). The subtraction \(F_X(0,\eta)\) cancels only in the conditional current normalization and remains in the outer retained-data marginal.

If a native external slot has a common radius \(r\) between \(\mathcal D\) and \(\mathcal D^+\), ordinary Cauchy gives external coordinate jets of these anchored quantities with factor \(u!r^{-|u|}\). For \(t\) unit directions in a norm ball, use parameter radii \(r/t\), giving \(t^tr^{-t}\le e^tt!r^{-t}\). Applying this jointly with the current-coordinate argument proves fixed-factorial mixed jets. The radii are those of the actual admitted background and independent-current slots. No arbitrary raw retained-coordinate direction is identified with a native unit direction, and no selector derivative is inferred.

### 5. How the endpoint premise can follow from an actual map theorem

Let the primitive source function \(b_X\) be bounded by
\(K_X\) on its original multiscale complex domain. Suppose the actual true-map pullback \(\Phi_{k,X}(z,\eta)\) lies in a smaller subdomain, leaving a fixed relative margin in each of the restrictions (2.34)–(2.39), simultaneously on (BC16.3). These restrictions include nonlinear reconstructed outputs. Their first derivatives and their value margins do **not** by themselves constitute a primitive Cauchy radius.

The additional **local native-chart certificate** used here has the following exact meaning. For every admitted center and every strong native direction \(v\) of norm at most one, there is a holomorphic curve \(\chi_v(w)\), defined on one fixed disc \(|w|<r_0\), with \(\chi_v(0)\) equal to that center and \(\chi_v'(0)=v\). Every point of the curve belongs to the full primitive B domain, including all reconstructed-field/current restrictions and the specified old-fluctuation arguments. The same fixed \(r_0>0\) works for every carrier, old scale and admitted center. A verified native-coordinate ball contained in the full domain is a sufficient certificate. A first-order inequality for the derived outputs alone is not.

Assume this certificate and measure a current-induced primitive argument tangent in its strong native norm, with the actual normalization radii included. If the actual map theorem proves

\[
 \|\partial_i\Phi_{k,X}\|_{\mathrm{margin},X}
 \le \frac{\vartheta_X}{P_k}e^{-cd_X(i)},
 \tag{BC16.19}
\]

then Cauchy on the certified curve gives (BC16.4), up to the fixed factor \(r_0^{-1}\). Indeed apply it to \(b_X\circ\chi_v\), where \(v\) is the normalized tangent. Its derivative at zero is the required primitive derivative in that tangent. The estimate is dimension independent. Uniform chart constants and admission of the whole curve must be checked in the actual geometry.

The need for this distinction has a simple exact counterexample. Put

\[
 D_N=\{u\in\mathbb C:|u|<1,\ |Nu^2|<1\},
 \qquad f_N(u)=\sqrt N\,u.
 \tag{BC16.19a}
\]

Then \(|f_N|<1\) on \(D_N\). At zero the defining outputs \(G_N(u)=(u,Nu^2)\) have derivative \(G_N'(0)=(1,0)\), and each output threshold is one, yet \(f_N'(0)=\sqrt N\). A nonlinear output condition can therefore shrink the actual directional disc while being invisible to its first derivative. This counterexample concerns the proposed Cauchy inference, not Yang–Mills or the actual source map.

The needed age comparison is also explicit. If, in the exact physical normalizations of the source restrictions, an output on layer \(n\le j\) has endpoint response bounded by

\[
 Cg_kP_k e^{-\Gamma_0(k-n)}e^{-cd_X(i)}
\]

and its old-domain margin is at least
\(c\alpha_{*,n}2^{-(j-n)}\), the verified AF comparison and \(q>p_0\) give the candidate normalized factor

\[
 C\ell_k^{p_0-q}\sqrt{1+k-n}\,
       2^{j-n}e^{-\Gamma_0(k-n)}.
 \tag{BC16.20}
\]

Writing \(a=k-j\) and \(r=j-n\), then fixing
\(\Gamma_0>4\log L+\log2+2\), bounds (BC16.20) by

\[
 C\ell_k^{p_0-q}(1+a)^{1/2}
       e^{-\Gamma a}
\]

for a fixed \(\Gamma>4\log L\), after summing or maximizing over \(r\). Thus it supplies (BC16.8) with a vanishing \(\vartheta_k\). This is a numerical deduction from the correctly normalized response. It does not repair a missing two-power factor in the reconstructed current or establish that the true joined map has the stated response.

The important change from the earlier prepared route is precise: (BC16.19) is needed for the actual analytic true-map family and the native external slots. It need not hold for arbitrary new complex decoupling operators. If an exact refinement/consistency identity is valid for the true family and remains valid on its analytic continuation, it can be used here without extending that identity to a different prepared operator family.

#### 5.1 A different auxiliary-current extension that preserves physical jets

CMP119, p. 261, permits a useful distinction. In (2.34)–(2.39), the auxiliary current \(J\) is restricted by (2.36). The reconstructed current in (2.37) is \(J_{p,X}(M^\bullet U)\): it is a function of the determining field \(U\), not of the independently supplied \(J\). Thus changing the auxiliary \(J\) while fixing \(U\) does not change the reconstructed-field/current requirements.

Write \(\mathscr J(U)\) for the physical Wilson current in the source normalization. On a complex field neighborhood this notation means its holomorphic extension, using matrix inverses and the complex-linear Lie-algebra projection. In particular the real expression involving \(\operatorname{Im}P\) is extended by \((P-P^{-1})/(2i)\), not by complex conjugation of a complex variable. On real group-valued fields this agrees with the physical current.

Let \(U(z,b)\) be an actual true-map family with \(U_0(b)=U(0,b)\). The parameter \(b\) is the specified native physical background or retained-coarse datum. This subsection assumes that this family is holomorphic on the required joint \(z,b\) contour and that all U-dependent restrictions of the primitive B domain, including (2.35) and (2.37), have a fixed reserve there. It also assumes a common admitted gauge/chart and the normalized current bound below. The subsection does not prove those true-map facts.

Define the layer-weighted current norm

\[
 \|\zeta\|_{\mathfrak J}
  =\max_n\frac{h_n^3\|\zeta\|_{\infty,\Omega_n\setminus\Omega_{n+1}}}
                    {\alpha_{0,n}},
 \tag{BC16.21}
\]

with the source's innermost-region convention on the final actual layer. For a primitive activity of scale \(j\), the source instead uses the \(j\)-norm in its entire innermost region \(\Omega_j\). Denote that norm, restricted to the primitive argument set, by \(\|\cdot\|_{\mathfrak J,j}\). On an actual layer \(n\ge j\), the ratio of its weight to the weight in (BC16.21) is

\[
 \frac{h_j^3\alpha_{0,n}}{h_n^3\alpha_{0,j}}
 \le C(1+n-j)^{b_q}L^{-3(n-j)}.
 \tag{BC16.21a}
\]

The admitted AF comparison gives the fixed polynomial bound used here. Hence
\(\|\zeta\|_{\mathfrak J,j}\le C_{\rm emb,J}\|\zeta\|_{\mathfrak J}\)
for one fixed \(C_{\rm emb,J}\). To use a common contour for every old primitive, define
\(\|\zeta\|_{\mathfrak J}^{\rm com}=\sup_j\|\zeta\|_{\mathfrak J,j}\).
This is bounded above by \(C_{\rm emb,J}\) times (BC16.21), and includes the final actual-layer norm. In the rest of this subsection the displayed current inequalities and radii use this common norm. Equivalently every radius in (BC16.21) may be reduced once by \(C_{\rm emb,J}\). This fixed reduction is necessary; the innermost convention is not silently identified across old scales.

Set \(s_*=1-\beta>0\), so every coefficient \(1-\beta(1-2^{-(j-n)})\) in (2.36) is at least \(s_*\). Suppose the actual joint true-map contour satisfies

\[
 \|\mathscr J(U(z,b))\|_{\mathfrak J}^{\rm com}\le s_*/4.
 \tag{BC16.22}
\]

For an auxiliary complex current \(\zeta\) define

\[
 \widehat F_X(z,b,\zeta)
  =b_X\bigl(U(z,b),\mathscr J(U(z,b))+\zeta,
                   \mathbf A_{\rm old},\mathbf S\bigr),
 \qquad \|\zeta\|_{\mathfrak J}^{\rm com}<s_*/4.
 \tag{BC16.23}
\]

#### Proposition BC16.4 — auxiliary-current admission and jet identity

Under the stated true-map hypotheses, (BC16.23) is a holomorphic extension of the actual physical primitive pullback, bounded by the same primitive carrier majorant. It retains a current-slot margin at least \(s_*/2\) in every primitive normalized current norm. Its auxiliary-current dependence is exactly localized to \(X\). If the true-map endpoint estimate (BC16.19) holds for \(U\) and \(\mathscr J(U)\) and the local native-chart certificate of Section 5 has been proved, it yields the same one-endpoint estimate uniformly on (BC16.23), without differentiating a minimizing operator in an independent off-physical current.

**Proof.** By (BC16.22) and the radius in (BC16.23), the J argument has normalized size at most \(s_*/2\). This is strictly below every source threshold in (2.36), with a margin at least \(s_*/2\). Every other source clause is a restriction on \(U\), its reconstructions or relative-field chart, so it is unchanged by adding \(\zeta\). The arguments therefore lie in the primitive domain. Holomorphy and the value bound follow from primitive holomorphy and composition.

Only the restriction of \(\zeta\) to \(X\) occurs in the primitive function. Consequently a derivative in \(\zeta(x)\), for \(x\notin X\), vanishes exactly. In a current coordinate, \(\partial_i\zeta=0\), so the derivative of the output argument is precisely \((\partial_iU,\partial_i\mathscr J(U))\). Under the additional native-chart certificate, the one-dimensional Cauchy bound of Section 5 gives (BC16.4), uniformly in \(\zeta\). At \(\zeta=0\), the expression is the physical primitive activity evaluated on its actual current graph. \(\square\)

The point of this proposition is that the original analytic extension of the **primitive activity** is retained. The new choice concerns how its auxiliary current is pulled back along a true minimizing family. It does not replace the primitive current by an unrelated constant.

To use the original base-current coordinate instead of the centered variable \(\zeta\), set

\[
 J_{\rm base}=\mathscr J(U_0(b))+\zeta.
 \tag{BC16.24}
\]

The pullback then reads

\[
 \widehat F_X(z,b,J_{\rm base})
 =b_X\bigl(U(z,b),\mathscr J(U(z,b))
             +J_{\rm base}-\mathscr J(U_0(b)),
             \mathbf A_{\rm old},\mathbf S\bigr).
 \tag{BC16.25}
\]

At \(z=0\), this is exactly \(b_X(U_0(b),J_{\rm base},\ldots)\), including its native current dependence. At the physical base-current graph \(J_{\rm base}=\mathscr J(U_0(b))\), it equals the actual physical pullback for every admitted \(z,b\).

The change (BC16.24) is triangular and analytic, with derivative equal to the identity in the auxiliary current. Its mixed/background derivatives are precisely the derivatives of \(\mathscr J(U_0(b))\). If that map is bounded on a larger native \(b\) ball, ordinary Cauchy supplies their fixed-factorial bounds. A product contour in \(b,J_{\rm base}\) is obtained by taking, for example, an \(s_*/16\) current radius about the original center and a \(b\) radius small enough that the normalized change of \(\mathscr J(U_0(b))\) is at most \(s_*/16\). Their sum is at most \(s_*/8\), leaving half of the auxiliary radius in (BC16.23). The reduction of the \(b\) radius is a fixed fraction when the true-map bound and its larger native radius are uniform.

For a holomorphic curve of physical parameters \(t\mapsto(z(t),b(t))\), the identity

\[
 \widehat F_X\bigl(z(t),b(t),\mathscr J(U_0(b(t)))\bigr)
 =F_X^{\rm physical}\bigl(z(t),b(t)\bigr)
 \tag{BC16.26}
\]

holds throughout its admitted neighborhood. Its derivative of every finite order is therefore identical on both sides, with all chain-rule terms from the base current retained. This proves compatibility of the physical finite jets and the triangular native-coordinate change.

It does **not** assert that arbitrary off-physical J derivatives of (BC16.25) equal those of a different source-defined off-physical minimizing family. Such numerical equality is unnecessary for a bound obtained using a new explicitly specified analytic extension, but it must not be falsely claimed. If an application demands that particular off-physical family, its matching theorem is still required. No auxiliary variable is integrated or changed in the Wilson measure here; this is an extension used to estimate the same physical functions.

The construction also preserves the relevant gauge rule. In a common fixed chart, \(\mathscr J(U)\) is gauge covariant. Transforming \(\zeta\) by the same adjoint action makes (BC16.23) inherit the primitive gauge invariance. A parameter-dependent change between charts must carry its actual analytic adjoint factors and derivative costs; the proposition does not hide those costs in the word covariance. Real compact gauge changes preserve the norm. Bounded complex chart changes modify it by the verified fixed chart constant.

#### 5.2 A uniform numerical slack condition

There is no need to spend only the exponentially shrinking difference between two maximal source domains if the actual true-map family lies much farther inside them. Suppose its physical normalized current is bounded on the proposed contour by

\[
 h_n^3\|\mathscr J(U(z,b))\|_{\infty,n}
 \le C_{\rm bg}g_n\ell_n^{p_0}
       +C_{\rm resp}g_kP_k e^{-\Gamma_0(k-n)}
       +C_b r_b\alpha_{0,n}.
 \tag{BC16.27}
\]

The last term records a retained/background ball of normalized radius \(r_b\), if it has not already been included in the first two bounds. This is an actual map estimate to be checked, not a new regularity assertion. The AF comparison and \(\alpha_{0,n}=C_0g_n\ell_n^q\), \(q>p_0\), imply

\[
 \|\mathscr J(U(z,b))\|_{\mathfrak J}
 \le C_*\ell_*^{p_0-q}
       \left(1+\sup_{a\ge0}\sqrt{1+a}e^{-\Gamma_0a}\right)
       +C_b r_b,
 \tag{BC16.28}
\]

where \(\ell_*\) is the lower bound on \(\log g_n^{-2}\) over the admitted trajectory. Multiply the constants in (BC16.28) by the fixed \(C_{\rm emb,J}\) to bound the common norm. First choose \(r_b\le s_*/(16C_{\rm emb,J}C_b)\). Then choose one coupling ceiling making the common-norm first term at most \(s_*/16\). This proves (BC16.22) with a reserve. The choices do not depend on old-layer depth or later derivative order. The analogous U-dependent bounds, especially the normalized reconstructed-current one, still have to be proved before applying this construction.

This auxiliary-current lemma requires the actual B-domain bounds and true-map physical current control. It does not require an off-physical consistency identity. Exact refinement/minimum consistency is one possible way to prove those true-map bounds; it is not a hypothesis needed merely to add the admitted independent current once the bounds are known.

#### 5.3 Two distinct analytic application routes

The local native-chart certificate and a bounded holomorphic actual pullback are different statements. Neither should be substituted for the other without the following additional information.

**Primitive-chart route.** The actual complete argument map \(\Phi_{k,X}\), including any old-field pullbacks, is holomorphic on the joint contour (BC16.3), takes its values in the primitive domain with the specified reserves, and has the normalized endpoint tangent (BC16.19). A uniform local native-chart certificate then bounds the primitive derivative in that tangent. BC16.1–BC16.3 apply. Exact consistency of true minima can simplify the admission check: when the source reconstructed minimum is exactly the original minimum in the required gauge, its reconstructed curvature/current restrictions become the corresponding original-field restrictions, after the explicit scale conversion. The identity must hold for the actual determining tuple and analytic continuation. It does not by itself supply a local directional disc for an arbitrary off-minimum input, nor control a parameter-dependent gauge conversion or an old-field argument.

**Direct-pullback route.** One may instead establish holomorphy and a bound for the actual scalar function \(F_X\), including all native slots, without parametrizing a local primitive chart. A bound \(|F_X|\le K_X\) merely on the common \(2P\) current cube gives ordinary Cauchy estimates \(m!K_XP^{-m}\). It does not give the endpoint factor in (BC16.4), and summing that bound over all old carriers can introduce a volume factor. A sufficient direct replacement is a uniformly local centered-difference bound. More precisely, on the larger current contour, suppose each actual one-coordinate slice admits a complex disc \(|t|<rP\), with one fixed \(r>0\), on which

\[
 |F_X(z+t e_i,\eta)-F_X(z,\eta)|
 \le K_X\vartheta_X e^{-c d_X(i)}.
 \tag{BC16.28a}
\]

The disc must be admitted for every center used by the subsequent Cauchy estimate; choose one larger fixed cube if needed. Cauchy gives (BC16.4) with the fixed factor \(r^{-1}\). This route requires no separate primitive chart. An actual localized expansion of the scalar pullback, with a common current/native contour and a primitive carrier majorant that pays the root and endpoint sums, is another sufficient direct replacement. In particular the source's already localized (3.43) could serve this role if its radius and its complete parameter/sector scope were identified. Its unresolved \(p_1\) radius remains an obstruction to importing that result here.

These are exact sufficient alternatives, not new estimate definitions. The first route must prove the native-chart/endpoint hypotheses; the second must prove its actual complex centered-difference or localized-carrier bound. A verified bounded physical-current pullback without either local ingredient is progress but does not close C-05. A real-only exact-minimum identity can be analytically continued once both actual families are holomorphic on the same connected neighborhood and agree on its real open family. It cannot establish the existence or size of that neighborhood by the identity theorem.

### 6. Actual geometry: the age gain is shared by a path and the old carrier

The numerical hypothesis (BC16.8) must not be justified by incorrectly assigning every point of an old B carrier to a layer \(n\le j\). Its innermost source region is \(\Omega_j\), and that region contains actual determining layers \(n>j\). A point close to the current input can have no large kernel age separation. In this case the primitive carrier's connection to the old bad set pays the missing age.

#### Proposition BC16.5 — the combined age payment

Use the actual nested determining geometry and metric of CMP96 (2.2), (2.46)–(2.59), as given in BM.1–BM.5. Write \(h_r=L^rh_0\). The physical separation of consecutive regions is at least \(RMh_r\). Let a primitive B carrier of scale \(j\) meet its source boundary anchor near \(Z_j=\Lambda_j^c\). This anchor is outside \(\Omega_{j+1}\), after the fixed endpoint convention in the source collar. Let \(y\in X\) belong to actual layer \(n\), and let the current input lie in the admitted deepest layer \(k\), allowing the fixed adjacent-step/stencil offset \(c_0\). Then

\[
 \begin{split}
 d_\Omega(y,i)&\ge RM(k-n-c_0)_+,\\
 C_{\rm tree}d_j(X)+C_{\rm end}
       &\ge R(n-j-2)_+.
 \end{split}
 \tag{BC16.29}
\]

The second inequality is only needed for \(n>j\). It is conservative: the physical shell lengths actually grow geometrically relative to \(h_j\).

**Proof.** The first inequality is the weighted-age path decomposition BM.3, with the fixed current-stencil offset. For the second, connect the primitive boundary anchor to the source cube containing \(y\) along a connecting tree. The part of the tree connecting those two points is a path. It starts outside \(\Omega_{j+1}\), ends in \(\Omega_n\), and therefore crosses at least \((n-j-2)_+\) complete successive collars. A physical crossing of the \(r\)-th collar has length at least \(RMh_r\). Since \(r\ge j\), dividing by the old carrier unit \(Mh_j\) gives at least \(R\) per crossing. The fixed source comparison between a tree meeting localization cubes and paths between points in those cubes yields \(C_{\rm tree}\) and \(C_{\rm end}\). Neither depends on carrier distance, age or total volume. Repeated crossings only increase length. \(\square\)

Let the original endpoint bound have rate \(\delta>0\), and retain the primitive factor \(e^{-\kappa d_j(X)}\). Allocate one quarter of each exponent to age. Since

\[
 (k-n-c_0)_++(n-j-2)_+\ge k-j-c_0-2,
\]

that allocation supplies

\[
 e^{-\frac\delta4d_\Omega(y,i)}
 e^{-\frac\kappa4d_j(X)}
 \le C\,e^{-\Gamma_0(k-j)},\qquad
 \Gamma_0=\min\{\delta RM/4,\ \kappa R/(4C_{\rm tree})\}.
 \tag{BC16.30}
\]

For \(n\le j\), the kernel age alone gives the same conclusion with a changed fixed endpoint constant. The source normalized-row entropy condition is imposed on another reserved endpoint share, as in BM.5. A further share retains spatial decay: every physical path weight is at least \(h_k^{-1}\), up to the fixed adjacent-step conversion, so

\[
 d_\Omega(y,i)\ge c_L\rho_k(y,i)-C_L.
 \tag{BC16.31}
\]

One quarter of each exponent can still be used for the current-to-old-bad-set collar when needed. The remaining primitive exponent is positive and can be chosen to pay its carrier entropy. More shares, with smaller fixed fractions, can be used if a particular source localization requires them; \(R\) is then increased by the corresponding fixed factor before the coupling ceiling is chosen.

Consequently one may first fix the actual primitive decay/localization constants, then fix the admitted geometric separation large enough that \(\Gamma_0\) exceeds any prescribed finite number, in particular \(4\log L+\log2+2\), while meeting the source row condition. The running source collars admit that fixed separation after reducing the common coupling ceiling. This does not replace the weighted multiscale metric by an old-scale Euclidean metric.

#### 6.1 Application to the actual inherited B gradient, with its precise remaining chart premise

The original-geometry response BM.6–BM.11, following CMP102 (190), has physical output normalization \(h_n^s\) with \(s=1,2,3\), and its input integration measure cancels the source kernel's input volume factor. For a marked current coordinate it retains

\[
 Cg_k e^{-\delta d_\Omega(y,i)}
 \tag{BC16.32}
\]

in those normalized output norms. It is not a sum over unnormalized fine bonds. The local constraint linearization \(g_kCz-hD(g_kCz)\) has the actual proper-scale stencil and fixed analytic inverse reserve; it changes only \(c_0\) and the fixed constant.

If the true joined consistency statement JR.2 is verified in the actual source gauge, the reconstructed curvature and current on this family are the original physical outputs, with their actual unit conversion. For the reconstructed current, JR.2 gives the target physical normalization \(h_n^{-2}h_{\min(p,n)}^{-1}\), which is no stronger than \(h_n^{-3}\). Thus no stand-alone inverse fine-mesh bound is substituted for (BC16.32).

For the inner part of an old \(j\)-domain, an actual layer \(n>j\) is tested at the coarser source label \(j\). Its field/current norm gains at least \(L^{-(n-j)}\), and the current gains three powers before any finer reconstructed normalization. This is sufficient for domain admission but, by itself, insufficient to pay the four-dimensional density of old roots. Proposition BC16.5 supplies the additional age factor at the activity level.

Under the local native-chart certificate of Section 5 and a verified marked gauge conversion, multiply the directional Cauchy estimate by the primitive factor \(B_0e^{-\kappa d_j(X)}\). The output point \(y\) may be anywhere in \(X\). Apply (BC16.30)–(BC16.31) before taking its supremum. The AF radius comparison then gives

\[
 |\partial_iF_X|
 \le \frac{C B_0\theta_k}{P_k}
       (1+k-j)^{b_*}e^{-\Gamma(k-j)}
       e^{-\kappa' n(X)}e^{-c d_X(i)},
 \quad \theta_k=\ell_k^{p_0-q},
 \tag{BC16.33}
\]

with fixed \(\Gamma>4\log L\), \(\kappa'>\log A+2\), and \(c>0\). Polynomial radius/gauge losses which are actually verified are included in the fixed exponent \(b_*\); an unproved loss is not declared polynomial. A residual dyadic domain factor \(2^{j-n}\), if that smaller margin is used, is paid by the extra \(\log2\) in the fixed rate choice. Strong physical-center slack avoids that factor entirely.

This derives the age/carrier form required by BC16.3 for inherited B from the actual boundary anchor and normalized kernel. The remaining primitive native-chart and marked gauge hypotheses are explicit. They are not consequences of (BC16.32) alone, as the example (BC16.19a) shows.

#### 6.2 The heterogeneous coefficient really begins at the geometrical layer

CMP119 (2.24) uses \(\phi_l=1\) on the prescribed one-layer interior of \(\Lambda_l\). Its construction (3.2)–(3.5) removes several layers of \(LMR_{l+1}\)-cubes around \(Z_l\) before defining \(\Omega_{l+1}\). For a sufficiently small common coupling ceiling, the adjacent-scale bounds (2.6)–(2.8) and the rounding convention (2.5) give
\(R_l\le L R_{l+1}\). Indeed the ratio of the underlying adjacent logarithmic powers is less than \(L\); rounding to powers of \(L\) can then change their exponent by at most one. The new collar contains the old one-layer \(MR_l\)-collar. Hence

\[
 \Omega_{l+1}\subset\Lambda_l^{-1}.
 \tag{BC16.34}
\]

The fixed endpoint conventions are handled by reducing to the prescribed interior collar. Rectangular enlargement of the bad complement shrinks the regular set and does not invalidate this inclusion. Thus for a point in actual layer \(n\), every \(l<n\) has \(\phi_l(x)=1\). The exact heterogeneous coefficient difference therefore has the form

\[
 w_k(x)-w_k=\sum_{l=n}^k\beta_l(1-\phi_l(x)),\qquad
 |w_k(x)-w_k|\le C(1+k-n)^2g_k^{-2},
 \tag{BC16.35}
\]

with at most the already specified fixed layer offset at a localization-cube boundary. This uses the absolute coupling comparison, not a beta-function sign.

For this sector a primitive B-chart argument is unnecessary: its plaquette function is explicit. On one proper-scale cube, BC15.1 and the normalized curvature derivative (BC16.32) give

\[
 |\partial_iF_{\Delta}^{\rm het}|
 \le Cg_k^{-1}(1+k-n)^2
           e^{-\delta d_\Omega(\Delta,i)}.
 \tag{BC16.36}
\]

The fourth curvature power pays the number of fine plaquettes; there is no inverse fine-spacing remainder. The coefficient support lies in the prescribed old-bad neighborhood, whereas the admitted current support has the current collar. Separate endpoint shares pay this collar, the age, and the spatial anchor. Consequently the sector fits the endpoint theorem with

\[
 K_{{\rm het},k}
  \le C g_k^{-2}\delta_k e^{-cR_k},
 \qquad \delta_k=g_kP_k,
 \tag{BC16.37}
\]

and a fixed polynomial old-age factor. Its weighted current Hessian is bounded by
\(C g_k^{-1}P_k^{-1}e^{-cR_k}\), which tends to zero for the admitted \(R_k\ge\ell_k^r\), \(r>1\). This deduction uses the existing original-geometry kernel scope and common physical current contour; it does not rely on the unresolved joined primitive B Cauchy disc. Native derivatives still use their actual common parameter radii.

#### 6.3 Native projection: exact retraction, with the input norm check retained

One possible extension to an off-minimum strong-native background \(U\) is

\[
 \Pi_B(U)=U_B(M_BU),
 \tag{BC16.38}
\]

using the identical original source minimizing function, its determining map, and its fixed gauge slice. Its retraction property is exact on that slice:

\[
 \Pi_B(U_B(V))=U_B(M_BU_B(V))=U_B(V).
 \tag{BC16.39}
\]

Thus this construction need not rotate old fluctuation arguments merely to recover equality at the physical center. If the baseline in C-01 is the next-scale minimum, use that exact baseline function first, followed by the actual current insertion into the preceding-scale determining data. Do not replace either map by an unnamed representative of its gauge orbit.

The source support geometry for estimating \(M_B\) is concrete. A determining bond in
\(\operatorname{st}_j\Omega_j\setminus\operatorname{st}_j\Omega_{j+1}\)
has both endpoints outside \(\Omega_{j+1}\). Its two-endpoint-block averaging footprint misses that inner domain by block alignment. If the fixed separation obeys \(RM>C_{\rm foot}L\), the footprint cannot reach a layer finer than \(j-1\), because it lies within distance \(C_{\rm foot}h_j\) of \(\Omega_j\). Only the \(j\) and adjacent \(j-1\) norms enter. The endpoint-block footprint uses the actual nonlinear averaging operation and its iterated dependency cone; it is not the support of a straight-line substitute for that operation.

Once the actual relative-average analytic norm is verified for this source family, a strong-native input of radius \(r_b\) yields normalized determining increments at most \(C r_b\alpha_{0,j}\). The source original-geometry map then sums these increments with

\[
 C\sum_{j}(1+|j-n|)^{b_q}
             e^{-\Gamma_1|j-n|}<\infty,
 \tag{BC16.40}
\]

where a fixed polynomial bounds \(\alpha_{0,j}/\alpha_{0,n}\) by the admitted AF comparison, and the age rate is the same fixed geometric rate as above. This gives a uniform native projection radius after a fixed reduction of \(r_b\). The common contour is chosen first on the absolute variational map domain; the smaller running B thresholds are tested only afterward.

The support calculation and the sum (BC16.40) are proved deductions. They do not identify a relative-average estimate for a different \(Q\) or reference average with the actual symmetric \(M\). That source-family identification and the common gauge chart remain checks in this projection route.

Even a proved global projection radius would not, by itself, be the local primitive-chart certificate in Section 5. The projection can transmit an input outside \(X\) into \(X\). Using its global boundedness to claim a local primitive directional disc would lose the endpoint estimate. A local matched-lift argument, or an equivalent verified directional disc, is still required for (BC16.33).

### 7. Complete boundary ledger and current application status

The following source sectors remain in the application:

| Sector | Required input to this direct route |
|---|---|
| Inherited primitive B | Its actual multiscale domain and full primitive carrier bound, followed by (BC16.19) for the true pullback; old retained coordinates are fixed inputs and any change of their arguments is retained. |
| E and R terms assigned to B | Their source assignment, old-scale subtractions and boundary localizations; regular E/R estimates alone do not remove these terms. |
| Classical/constraint and measure boundary pieces | The complete constrained action and the local Haar/coarea factors; the bulk estimate does not include unexamined boundary-change determinants. |
| Heterogeneous Wilson coefficient | The exact coefficient difference, physical plaquette normalization and four-dimensional fine-cell cancellation from BC15.1, combined with a current-to-old-boundary endpoint estimate. |
| Relocation | The full action change and Jacobian caused by the actual localized change of variables; smooth old selectors are fixed real parameters, not complex analytic variables. |
| Current Gaussian exterior force | Retained exactly in the conditional Gaussian split. It is linear in current coordinates, has zero current Hessian, and is not discarded from the conditional mean. |

The primitive source ledger and the fixed scalar sector budget are unchanged. The direct endpoint theorem can replace the need for a new prepared thin-carrier expansion when proving the current derivative and weighted Hessian output. It does not itself verify all entries of this table.

The old-fluctuation arguments require an explicit distinction. In the C-01 normal form the old coordinates are retained integration data. The current localized gauge/constraint operations cannot be presumed to leave them fixed merely because they are old. CMP102 (4) fixes a variational gauge transformation at determining sites; if an old fluctuation bond has its endpoints at those sites, its adjoint rotation is exactly the identity. The admitted separation between its old bad support and the current inner region must be used to verify those endpoints. Any additional source coordinate change not having this property must retain its old-field pullback and its derivative. The reconstruction gauge converter used only to check a reconstructed-current norm is not automatically applied to the primitive B old-field arguments.

The current relocation in CMP119 p.269 changes the current-scale exterior fluctuation coordinates on \(S_{k+1}\). Its complete induced action and Jacobian remain in the ledger above. Its exponentially small shift gives small coefficients only after the differentiated action terms, including inherited B, are controlled. It is not enough to bound the displacement and omit a derivative of the displaced primitive activity.

The complete local native B-domain chart has not been established. True-minimum consistency and an original-geometry endpoint estimate would resolve the physical reconstructed-output branch, but they do not alone prove the primitive Cauchy disc. The marked source-gauge conversion and every actual old-field/relocation pullback must also be checked. A generic bounded constraint-current coefficient is insufficient for projected derivative terms; the actual matching issue exposed in Annex AM is retained. The local multiplier-majorant issue is more specific and has been resolved at its proper reference-average scope: the printed CMP99 bound (3.137), which already inserts a global multiplier norm, is not sufficient, but the reproduced CMP102 (72) gives the missing local pointwise derivative. Lemma CC.3a in Annex AM extracts its quadratic coefficient by Cauchy on the value-only ball, then inserts the exact determining measure factor from (3.136). This supplies the local \(h_a|\lambda|\sup|A|\) bound without importing the averaging formula (149). It still does not identify that reference-average map with the raw symmetric source map.

**C-05 remains open.** The new results proved here are the endpoint-to-kernel theorem, the auxiliary-current admission and physical-jet identity, the combined actual path/carrier age payment, and the heterogeneous coefficient/normalization deduction. The sufficient application still needs an exact local native B-domain chart (or equivalent uniformly admitted holomorphic directional discs), the actual source gauge/coordinate conversions and old-field slots, and a checked true-map joint contour. These premises are stronger than first-order output inequalities and are not supplied by assumption.

If those checks are completed, (BC16.33), the complete sector estimates retained from BC15.14, and BC16.3 give a sufficient closure theorem with a fixed prefactor

\[
 K_{B,k}\le C(1+S_{b,\delta})\left[
  \mathfrak K_E+C_Rg_k^{\kappa_0-11}+B_0\ell_k^{p_0-q}
  +g_k^{-2}\delta_k^3+\delta_k
  +g_k^{-2}\delta_ke^{-cR_k}+g_k^\nu\right].
 \tag{BC16.41}
\]

The weighted Hessian is then at most \(C K_{B,k}/P_k^2\); the direct all-order current kernel version has factorial exponent five and decay length proportional to the order, as in (BC16.13). Choose the source carrier/localization parameters first, the admitted separation \(R\) next to pay the combined age and row losses, one fixed \(q>p_0\), and then the coupling ceiling to meet all absolute/native radii and the desired Hessian budget. No parameter is changed with derivative order or cutoff.

The native derivative branch is part of this conditional conclusion. It is not removed to declare completion of the current Hessian branch alone. Accordingly **C-06 remains a theorem conditional on C-05 while C-05 is open**. A proved physical-current Hessian subcase would not establish every native conclusion of C-06.

For clarity, the still unverified application is finite and concrete:

1. Identify the actual true reconstructed minimum with the original one on the mixed determining tuple, in the required analytic source gauges, and establish the joint current/native contour with normalized physical current reserves. An alternative direct source proof with the same full domain is allowed; (3.43) is not yet such a proof because of its radius ambiguity.
2. On that contour prove either the local primitive directional-disc certificate plus endpoint tangent, or a direct centered-difference/localized scalar bound as in Section 5.3. If the former uses a projected matched lift, verify the actual symmetric-average/reference-gauge identification and its source-coordinate matching; the local multiplier bound CC.3a is available at the reference-average scope. First-order reconstructed-output margins do not suffice.
3. Check the actual transformation of every old fluctuation, constraint/measure factor, independent current and relocation term, including their native complex radii and endpoint costs. The auxiliary-current construction above can supply the independent slot once the U-dependent contour is available; it does not supply the remaining U/chart checks.

The age, carrier, derivative and Hessian sums are conditional on these three source applications with the same parameters.

### Sources

- T. Balaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP 119 (1988), 243–285: especially pp.247, 261–262 and 276–277; (2.34)–(2.42), (3.43).
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. I*, CMP 109 (1987), 249–301: around (3.6)–(3.17). DOI: https://doi.org/10.1007/BF01215223
- T. Balaban, *Renormalization Group Approach to Lattice Gauge Field Theories. II. Cluster Expansions*, CMP 116 (1988), 1–22: especially (1.34), Lemmas 1–2 and the localization construction. DOI: https://doi.org/10.1007/BF01239022

### Supplement AN.1. Complex-domain assumptions for the localized boundary term


This supplement identifies which complex-domain assumptions enter the boundary estimate.

#### 1. A first-response bound is not a complex-domain certificate

The primitive boundary activities are bounded holomorphic functions on a domain defined in part by nonlinear reconstructed-field and reconstructed-current restrictions. Their arguments cannot be treated as independent product coordinates merely because the restrictions have separate displayed bounds.

##### Proposition DA16.1 — a nonlinear-domain counterexample

For an integer $N\geq1$, define

\[
 D_N=\{u\in\mathbb C: |u|<1,\ |Nu^2|<1\},
 \qquad f_N(u)=\sqrt N\,u,
 \qquad G_N(u)=(u,Nu^2).
 \tag{DA16.1}
\]

The function $f_N$ is holomorphic on $D_N$ and satisfies $|f_N|<1$. Both inequalities defining the domain have threshold one. At zero,

\[
 G_N(0)=0,\qquad DG_N(0)v=(v,0),
 \qquad Df_N(0)v=\sqrt N\,v.
 \tag{DA16.2}
\]

Consequently, the first derivative of the constrained output tuple, normalized by its displayed margins, does not bound the first derivative of an arbitrary bounded primitive function on that domain by a constant independent of $N$.

**Proof.** The second inequality defining $D_N$ is equivalent to $|u|<N^{-1/2}$, which proves the value bound. The derivative identities follow by direct differentiation. The last derivative diverges for $v=1$. $\square$

This is a counterexample to an analytic inference. It is not a counterexample to the Yang–Mills model or to the proposed observable route. Its role is to identify the additional certificate needed before applying primitive Cauchy estimates to a boundary function.

#### 2. A sufficient certificate that does permit primitive Cauchy

The relevant statement is quantitative and can be checked without demanding an entire source-dependent renormalization construction.

Let $E$ be a finite-dimensional complex normed coordinate space. Let $U_*$ be a baseline point. Suppose each map $G_r$ is holomorphic on the absolute coordinate ball $\|U-U_*\|_E<R_0$. Let the primitive domain be specified by $\|G_r(U)\|<a_r$, together with any independently admitted product slots. Assume

\[
 \|G_r(U_*)\|\le (1-\epsilon)a_r,
 \qquad
 \sup_{\|U-U_*\|_E<R_0}
       \|DG_r(U)v\|/a_r\le K\|v\|_E
 \tag{DA16.3}
\]

for all the relevant restrictions, with fixed $\epsilon>0$ and $K<\infty$. The absolute ball must be defined before assuming membership in the smaller primitive domain.

##### Proposition DA16.2 — uniform native ball and directional derivative

Set

\[
 r_* = \min\{R_0/2,\epsilon/(2K)\},
 \tag{DA16.4}
\]

with the second term omitted if $K=0$. Then the ball $\|U-U_*\|_E<r_*$ lies in the primitive domain, leaving at least $\epsilon a_r/2$ reserve in every displayed restriction. If $b$ is holomorphic on that domain and $|b|\le B$, then

\[
 |Db(U_*)v|\le B r_*^{-1}\|v\|_E.
 \tag{DA16.5}
\]

The analogous order-$m$ directional estimates have a fixed factorial bound with cost $r_*^{-m}$.

**Proof.** Integrate the derivative of $G_r(U_*+tV)$ over $0\leq t\leq1$ to obtain
$\|G_r(U_*+V)-G_r(U_*)\|\le Ka_r\|V\|_E$.
For $\|V\|_E<r_*$, this is at most $\epsilon a_r/2$, proving the admitted ball. Apply one-variable Cauchy to $b(U_*+zv)$ on the disc $|z|<r_*/\|v\|_E$ for (DA16.5). For mixed directions, parameter radii $r_*/m$ give the elementary cost $m^m\le e^m m!$, after normalizing their norms. $\square$

One can replace (DA16.3) by a proved analytic chart with a comparable admitted radius. One can also use a directly proved endpoint derivative of the complete pullback. What is invalid is replacing the uniform native-ball assertion by the derivative at its center alone.

#### 3. Consequence for the proposed C-05 proof

The direct endpoint summation theorem of Sections 3–4 (Theorem BC16.3) is useful and has a complete proof. To apply it to the actual primitive B activity, its endpoint hypothesis must be established using a certificate such as Proposition DA16.2, a verified source-native chart, or an independent direct estimate. A bound on the first derivative of the reconstructed outputs along the physical minimizing family does not alone provide this certificate.

Likewise, a holomorphic retraction onto the physical minimizing family can preserve every physical jet, but it must have the required local domain and endpoint estimates. A global projection can introduce dependence outside a primitive carrier; exact locality of the unprojected primitive does not automatically survive that projection. If a local projection is used instead, its fine-collar current and chart estimates must be proved.

The matched-lift calculation in Annex AM supplies a concrete part of this step. In its actual regularized averaging coordinates it controls the projected tangent using a scalar gauge equation and the Wilson Ward identity. It does not identify the derivative of the raw nonlinear determining average with that regularized operator without the corresponding gauge conversion.

#### 4. Representative conventions

The CMP102 variational paper explicitly distinguishes its axial representative from the relative Landau field. Its Proposition 9 and formula (190) must be read with that distinction. The axial condition is referred to CMP99, 75–102, equation (1.19), a different paper from the CMP99, 389–434, propagator paper.

That paper is T. Bałaban, *Spaces of regular gauge field configurations on a lattice and gauge fixing conditions*, CMP 99 (1985), 75–102; DOI https://doi.org/10.1007/BF01466594. Its equation (1.19) is not used here, and no secondary source replaces that definition.

The explicit block-transport gauge constructed in Annex AL can be checked algebraically. Calling it the particular source axial gauge requires a checked identification or a separately bounded conversion. Equality of real gauge orbits and unitary invariance of real current norms do not by themselves give that complex representative estimate.

#### 5. Dependence on the boundary estimate

The heterogeneous coercivity implication in Annex AI requires the complete boundary derivative estimate on the same law.
