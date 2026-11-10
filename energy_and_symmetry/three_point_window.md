# A Wilson three-point test on a weak-coupling window

The physical target in the manuscript, §23 (292)–(304), is scalar. In its Hermitian trace convention \(Q=\tfrac12\sum_{b,\mu<\nu}(F^b_{\mu\nu})^2\), \(d=N^2-1\), \(b_0=11/(48\pi^2)\). Its separated Gaussian two-point coefficient is \(c_2=3d/\pi^4\); its scalar connected Gaussian three-point function is zero. Its **perturbative** three-point coefficient for \(Q\) is \(c_3g^2\), \(c_3=3db_0/\pi^6=11d/(16\pi^8)\). A readout with leading factor \(g^2Q\) instead has order \(g^8\). These factors follow directly from (298)–(300). Historical K-23's reference to a nonzero *Gaussian* scalar coefficient conflicts with (298). the corresponding estimate manuscript, §23

## 1. Six-leg estimate for the compact Wilson measure

Use exactly the compatible even cubic tori of Annex O §22, its local energy/moment bound, \(\epsilon=10^{-6}\), \(l=L^{\lfloor\epsilon\log_L\beta\rfloor}\mid n\), \(n\ge3l\). Here \(\beta\) multiplies the once-counted action \(s_p=\|1-U_p\|_{\rm HS}^2/2\). Use the real site-centered trace-completed tensor of Annex O §29, \(A_H(x)=a^4 H:\widetilde q(x)\), and the centered canonical comparison variable
\[
 X_H(x)=\tfrac12\beta(A_H(x)-\mathbb E A_H(x)).
\]
The factor \(1/2\) converts O.43's orthonormal color-coordinate quadratic to \(Q_H=\tfrac12\sum_b F_b^\top H F_b\). For \(H=I\), \(A_{I/2}=a^4w_a\), so \(X_I\) is the centered \(\beta a^4w_a\). In the lattice Gaussian \(X_H^G\), use each of the four clover curls at its actual midpoint, and independently average the four Wilson square placements in the trace repair. All field factors in the following constants have bounded \(H\). Assume the diameter of the three vertex stencils in one lift is at most \(C_0R\), \(1\le R\le\beta^{\epsilon/100}\). Then
\[
 |\kappa_3(X_{H_1},X_{H_2},X_{H_3})-
   \kappa_3(X^G_{H_1},X^G_{H_2},X^G_{H_3})|
 \le C_{N,L,C_0}\,[\beta^{-\epsilon/6}+R/l].
 \tag{1}
\]
The same bound holds for the pair covariance, and for the uncentered products needed to center all factors. It is uniform over the specified vertices. This is an absolute error in lattice units.

**Proof.** Randomly offset the boxes of O §22. The placements cutting the joint stencil have probability \(O((1+C_0R)/l)\); their gauge-invariant Wilson integrals are bounded by the single-plaquette moment estimates and are independent of the offset. Gaussian moments have the same uniform bounds. On other placements there is a common forest frame. Delete the conditional matrix mean of \(\sqrt\beta(U_p-I)\) after subtracting identity at each of up to six positions. Its averaged squared displacement is \(O(\beta^{-\epsilon/3})\) by O §22. Each telescoping product uses one \(L^2\) norm and at most five \(L^{10}\) norms. Those norms are uniformly bounded by the compact local reserve and conditional Jensen, including centered matrices, inverses and cyclic base conventions. Real parts, traceless projections, finite clover sums and conjugate factors preserve these bounds. A Wilson square uses its exact matrix-norm identity. This step costs \(O(\beta^{-\epsilon/6})\).

For clarity, the polynomial-box Laplace estimates also cover six centered factors. On the visible good exterior use its common real forest coordinates and the normalized Gaussian in \(y=\sqrt\beta(u-u_*)\). The two discarded tails beat polynomial weights. On \(|y|\le\beta^{1/32}\) the relative density error is \(O(l^4\beta^{-13/32})\); the centered Taylor error per matrix has leading bound \(C\beta^{-1/2}|y|^2\), and the product of six linearizations and Taylor remainders uses moments at most 12. The Gaussian \(L^j\) norm of \(|y|\) is \(C_j l^{12}\) there or without truncation. Expanding the centered products (conditional means subtract their own expectations), replacing one plaquette derivative costs \(Cl^{18}\beta^{-1/4}\); replacing one covariance costs \(Cl^{58}\beta^{-1/4}\) in operator norm. Each of at most three Gaussian pair factors before replacement is bounded crudely by \(C l^{24}\). These bounds together cost at most \(C l^{300}\beta^{-1/4}+C l^{300}\beta^{-13/32}\), hence \(O(\beta^{-1/32})\). Higher moments on the bad exterior are absorbed by its exponential probability. The resulting projected box curl covariances differ from the full lattice ones in offset-averaged absolute value by \(O(1/l)\), by projection positivity and the diagonal rank deficit. Wick products of at most three bounded covariances have the same error by telescoping. This argument can be restricted to the good offsets because the estimate uses the average of the *absolute* entry error. Combining the product comparisons of orders one through three of the quadratic insertions proves (1) by the moment-cumulant polynomial. Annex O §§22, 26 and 29 · Growing-box proof, §§10–11, especially (36), (38) and its polynomial constants

## 2. Second-order mesh accuracy and a single-sector nonzero coefficient

At separated rescaled vertices \(u_i=x_i/R\) in a fixed compact set with pair distances bounded below, put \(K(v)=\Lambda^2(I-2vv^\top/|v|^2)/(\pi^2|v|^4)\). In the Gaussian representative for either the centered scalar or a diagonal \(H\), the lattice two- and three-point kernels, multiplied by \(R^8\) and \(R^{12}\), differ from the continuum Wick kernels **at those vertices** by \(O(R^{-2})\).

To see the additional power, express each lattice curl covariance in midpoint coordinates. At small momentum the midpoint projection uses exterior multiplication by \(\hat k_i=2\sin(k_i/2)\) and its adjoint, divided by \(|\hat k|^2\). Its difference from the continuum projection is \(O(|k|^2)\) with order-\(m\) derivatives \(O_m(|k|^{2-m})\). A dyadic partition near zero, followed by six or more integrations by parts (take eight), gives entry error \(O(|r|^{-6})\) after keeping the midpoint displacement in the leading kernel. Away from zero integrate the periodic *anchored* symbol with its smooth cutoff, before interpreting the low-frequency midpoint shift. This avoids a spurious boundary term from nonperiodic half-lattice phases. In each clover the midpoint offsets have zero barycenter with their oriented positive averaging weights. A four-vertex Wilson square uses one shared offset for the two legs, also of mean zero. For the scalar or diagonal tensor every component pair has precisely such weights, possibly multiplied by a signed coefficient. Taylor expansion of the cyclic product around the vertices kills its terms linear in any leg offset; shared offsets do not affect this first-order identity. The remaining two derivatives cost \(R^{-2}\). This proves the comparison including its trace repair, at distinct vertices. For fixed compact smooth separated profiles the continuum Riemann sum error is \(O_f(R^{-2})\) by midpoint integration. Annex O §§18, 29

For a new one-sector measurement choose
\[
 H=\Lambda^2\operatorname{diag}(-1,1,1,1).
\]
Its six diagonal entries are \(a_\mu+a_\nu\) with \(a=(-3/2,1/2,1/2,1/2)\); hence it lies entirely in the diagonal stress channel and has zero trace. Take the three sites at \(0,Re_0,3Re_0\), with integer \(R\). In this direction \(HK(te_0)=I/(\pi^2|t|^4)\). Writing \(t=(0,1,3)\), the compact Wilson estimates are
\[
 \begin{split}
 R^8\kappa_2(X_H(x_i),X_H(x_j))
 &=\frac{3d}{\pi^4|t_{ij}|^8}+O(E_R),\\
 R^{12}\kappa_3(X_H(x_1),X_H(x_2),X_H(x_3))
 &=\frac{6d}{1296\pi^6}+O(E_R),\\
 E_R&=R^{-2}+R^{12}(\beta^{-\epsilon/6}+R/l).
 \end{split}\tag{2}
\]
The second constant uses \(1^4 2^4 3^4=1296\). Pair Wick contractions give \(d\,\mathrm{tr}(HKHK)/2\); at order three the two cyclic orders of the half-quadratics give \(d\,\mathrm{tr}(HK_{12}HK_{23}HK_{31})\) on this axis. The exact centering makes the third full moment equal to the third cumulant, including for the compact Wilson law. The common error tends to zero for all \(R\to\infty\) in the window. For instance \(R=\lfloor\beta^{\epsilon/100}\rfloor\) gives \(E_R=O(\beta^{-\epsilon/50})\). If this window is to shrink in *physical* length also require \(aR\to0\). Diagonal-stress decomposition, Annex X (F.15)

In particular the three pair covariances are positive for sufficiently large \(R,\beta\). In the exact Wilson law their geometric normalization gives
\[
 \frac{\kappa_3(X_H(x_1),X_H(x_2),X_H(x_3))}
 {\sqrt{\kappa_2(1,2)\kappa_2(2,3)\kappa_2(3,1)}}
 =\frac{2}{\sqrt{3d}}+O(E_R). \tag{3}
\]
An arbitrary common positive deterministic field multiplier, including the measured stress channel factor at that cutoff, cancels **exactly** from this ratio. Centering cancels additive constants. Thus (3) needs neither an asymptotic for that multiplier nor the full mixing matrix. It refers to its specified one-channel field and does not assert invariance under arbitrary nonlinear changes of observable.

## 3. A zero-mean profile and the physical scalar test

Use the profile specified in §23 (302): centers \(v_i=t_i e_0\), normalized \(C^\infty\) nonnegative bump supported in the unit ball, \(f_i=-\partial_0\eta_\sigma(\cdot-v_i)\). An explicit width is \(\sigma=10^{-24}\) in rescaled units. For stress write \(J_H(u)\) for the continuum three-point kernel divided by \(d/\pi^6\), and \(J_I^{\rm pert}(u)=\prod_{i<j}|u_i-u_j|^{-4}\). On the temporal axis these functions are \(6k\) and \(k\) respectively, \(k=\prod |t_{ij}|^{-4}\). The mixed time derivative of \(k\) at the given centers is \(25/729\), by (303). Thus the smeared \(J_H\) is positive with value within \(10^{-6}\) of \(150/729\), and the smeared \(J_I^{\rm pert}\) is within \(10^{-6}\) of \(25/729\).

Here are quantitative bounds that fix the profile width independently of a Taylor convention. Take complex coordinate radii \(1/64\) about any real points within \(\sigma\) of the three prescribed centers. For every pair, its complex squared separation \(v\cdot v\) has modulus at least \(0.8\,|t_{ij}|^2\), by the triangle inequality before and after the displacement. The reflection factor \(I-2vv^\top/(v\cdot v)\) has operator norm below 5 there, and its exterior square has norm below 25. Each kernel with \(\pi^2\) removed has norm below 40. The absolute trace of a triple is below \(6\cdot40^3<10^6\), also sufficient for the scalar benchmark. Cauchy's formula bounds any fourth derivative by \(4!\,64^4\,10^6\). Moving the real arguments over the supports costs at most \(12\sigma\) times this bound for the mixed third derivative. Integrating by parts three times proves both bounds. The Wilson cumulant of \(\sum_x f_i(x/R)X_H(x)\) thus tends to a *specified positive smeared connected stress coefficient* in these units, with error \(O_f(E_R)\); the three engineering factors \(R^4\) cancel the three cell volumes \(R^{-4}\). The signed smooth profiles are disjoint and have zero integral. At finite mesh the variables remain centered directly; no exact sampled zero sum is needed.

For the actual **scalar**, the Hodge star anticommutes with every \(\Lambda^2(I-2vv^\top/|v|^2)\). A Gaussian cyclic product of three has zero trace identically at all separated vertices. The same proof yields
\[
 \left|\kappa_3\!\left(\sum_x f_i(x/R)X_I(x):\,1\le i\le3\right)\right|
 \le C_f E_R. \tag{4}
\]
At point vertices the scalar two-point law in (2) still has coefficient \(3d/\pi^4\). For any integer \(R\) in the window the discrete Gaussian centered scalar cumulant is also explicitly computable from its three midpoint projections and the prescribed four-vertex weights. Subtracting **this exact lattice value** inside (4) removes \(R^{-2}\) from the error estimate. The remaining \(O_f(R^{12}[\beta^{-\epsilon/6}+R/l])\) upper bound has no identified sign or first nonzero interacting coefficient.

There is a matching-independent way to *state a necessary physical test*. Form the ratio on the left of (3) with the scalar at the same vertices, or take the third cumulant on the §23 profiles and normalize by the square root of three pair covariances on nonnegative separated profiles for which the Gaussian pair integrals \(I_{ij}^{(2)}\) are positive. In the smeared version the factors \(R\) and any common positive scalar multiplier cancel exactly. If the physical two- and three-point readouts have (304) and its two-point analogue with a common \(z_\rho\) to the necessary accuracy, then the predicted ratio divided by \(g_\rho^2\) is
\[
 \frac{b_0}{\sqrt{3d}}\,
 \frac{\int J_I^{\rm pert}\prod f_i}
 {\bigl(\prod I_{ij}^{(2)}\bigr)^{1/2}}+o(1).
 \tag{5}
\]
Here \(I_{ij}^{(2)}\) integrate \(|u_i-u_j|^{-8}\) with the chosen pair probes. The point version has the last profile quotient equal to one; the smeared version avoids asking for pointwise convergence of continuum distributions. This cancellation removes scalar multiplicative matching from **this diagnostic**. The running coupling and its relative error, the connected scalar signal itself, and the order of limits survive the cancellation.

Neither (1) nor (4) resolves the interacting order in (5). Already with the *tree-level* convention \(\beta=2Nx,\ g^2=x^{-1}\), the bare comparison error \(\beta^{-\epsilon/6}\) is larger than \(\beta^{-1}\) even before the factor \(R^{12}\). Nothing in subtracting the exact midpoint Gaussian improves that power. Also a comparison on a growing number of microscopic spacings with \(aR\to0\) provides no uniform fixed-\(\rho\) continuum limit or positive-endpoint trajectory. Equations (1)–(4) are compact-Wilson conclusions on the specified weak families. Equation (5) isolates a quantitative condition for further work. **U-01 and U-02 remain open at their frozen scopes.**

## 4. Extracting the first interacting scalar correction on a fixed compact subregion

There is an independent finite-volume computation of the order discarded in (4). Pin the boundary of a simply connected finite four-dimensional cube \(B\) to identity; use the source's boundary-fixed spanning forest on its interior. Let \(w_{ip}\) be **any three specified** real plaquette-weight arrays on interior stencils (the four-vertex placement and the sampled signed profiles are allowed). Write \(Y_i=\beta\sum_p w_{ip}s_p\). For \(t\) in a fixed small complex polydisc let \(c_p(t)=1-\sum_i t_iw_{ip}\), with \(\Re c_p\ge3/4\). In forest coordinates \(u\) define the homogeneous forms by Taylor expansion
\[
 \sum_p c_p(t)s_p(\exp u)=\tfrac12u^\top D_tu+S_{3,t}(u)+S_{4,t}(u)+\cdots,\quad
 dU=\text{const}\,(1+J_2(u)+O_B(|u|^4))\,du .
\]
The forms are directly determined by the four ordered fundamental Wilson matrices on every plaquette. The Haar term in skew-Hermitian coordinates is \(J_2=\tfrac1{24}\sum_e\operatorname{Tr}_{\rm ad}((\operatorname{ad}u_e)^2)\), from the product exponential Jacobian; it is nonpositive on real coordinates. Let \(\mathbb G_t\) be normalized Wick contraction with covariance \(D_t^{-1}\), and put
\[
 \mathcal L_B(t)=\mathbb G_t[J_2-S_{4,t}]
                      +\tfrac12\mathbb G_t[S_{3,t}^2].
\]
Then the actual centered scalar third cumulant is
\[
 \kappa_{3,B}(Y_1,Y_2,Y_3)
 =-\tfrac12\partial_{123}\log\det D_t\big|_0
   +\beta^{-1}\partial_{123}\mathcal L_B(t)\big|_0
   +O_{B,w}(\beta^{-2}). \tag{6}
\]
Thus the finite **interacting connected** coefficient is a specified finite Gaussian polynomial, including the variations of its propagator, both action vertices, its Haar term, and the normalization. It uses no presumed renormalization projection. Failing to differentiate the source-dependent covariance would omit contributions at separated vertices.

Indeed on this fixed forest there is one flat configuration, by simple connectivity and the connected fixed boundary, and the Hessian \(D_0\) is positive on the forest slice. Compactness bounds the outside of a fixed neighborhood by \(O_B(e^{-c_B\beta})\), uniformly on the chosen complex source polydisc. After \(u=\beta^{-1/2}y\), expand through third order in \(\beta^{-1/2}\). The integral remainder is \(O_B(\beta^{-2})\) by restricting first to \(|y|<\beta^{1/32}\), using fourth-order Taylor remainders with polynomial Gaussian moments there and Gaussian tails on its complement. The odd homogeneous contributions integrate to zero on a symmetric ball. The source-dependent leading factor is a nonzero multiple of \((\det D_t)^{-1/2}\), uniformly bounded away from zero at fixed \(B,w\) on a smaller polydisc. Taking the logarithm leaves the displayed first-order correction; Cauchy gives the same error after the three source derivatives. Subtract the source-zero logarithm to form the normalized generating function. This extracts a particular derivative one order beyond the leading Gaussian in the finite-box calculus of §24 and Annex J; it gives no bound uniform in cube size. Finite-box source and normalized Wilson action, §24

This extraction also holds after restricting an ordinary periodic Wilson measure to the event that the boundary of this fixed box is gauge-equivalent to links individually within \(\beta^{-4}\) of identity. The event has positive probability at finite \(\beta\). Conditional on that boundary, the actual interior law is compact Dirichlet Wilson. In the stated boundary gauge the total action differs from its identity-boundary version by \(O_B(\beta^{-4})\), uniformly in all interior links, by the finite plaquette product and smooth real trace. Its **normalized** density ratio differs from one by \(O_B(\beta^{-3})\). For interior stencils the two variables use identical functions; moments through degree three of \(\beta s_p\) are bounded in the identity-boundary law by the same Laplace bound. All required conditional moments therefore differ by \(O_{B,w}(\beta^{-3})\) uniformly on the event; averaging them first also gives (6) for the event-conditioned cumulant. This does not assign a useful uniform weight to the event.

An exact check distinguishes this interacting correction from the Gaussian coefficient. In \(SU(2)\), condition all links except one to identity (or take their above shrinking neighborhoods). Each of the six incident plaquettes has the same action \(s=2-\operatorname{ReTr}U\). Pick three distinct incident plaquettes, with arbitrary unit weights, and put \(c=6\). The one-link partition function is proportional to \(e^{-2v}I_1(2v)/v\), \(v=\beta(c-\sum t_i)\). Equivalently it is the integral of \(e^{-2v(1-\cos\theta)}\sin^2\theta\,d\theta\); substituting \(z=2\sqrt v\sin(\theta/2)\) yields the weight \(z^2 e^{-z^2}(1-z^2/(4v))^{1/2}\) on \([0,2\sqrt v]\). The first relative correction is \(-3/(16v)\), since the ratio of the fourth and second half-line Gaussian moments is \(3/2\). Hence
\[
 \kappa_3(\beta s,\beta s,\beta s)
 =3c^{-3}-\frac{9}{8c^4}\beta^{-1}+O(\beta^{-2}).
\]
Uniform complex source differentiability follows from (6) or directly on a smaller disc by the same Laplace proof. This nonzero correction is a compact Wilson contact sharing one bond; its sign and geometry give no inference for \(c_3\) of the separated physical scalar. What (6) supplies for genuinely separated fixed-box stencils is an explicit expression and a relative-order remainder. The large-box limit of that expression, its uniform error, and the integral over unrestricted exterior data remain to be proved.

## 5. A positive first correction for three disjoint Wilson scalar stencils on a specified conditional sector

The coefficient in (6) can also be computed in a finite **separated scalar** example. Use \(SU(2)\), any even periodic side \(n\ge12\), and seven independent positive spatial 1-links, departing from \(x_j=je_0\), \(j=0,\ldots,6\). Retain these seven links as the integration variables. Set the other links in all incident plaquettes and in the following three stencils to identity for the moment. Insert the *actual four-vertex* scalar \(Y_j=\beta a^4 w_a(x_j+e_2)\) at \(j=0,3,6\). Their closed stencils are mutually disjoint in time. In the stencil at \(x_j+e_2\) precisely one plaquette contains a live link, namely the positive \(12\) square from \(x_j\); consequently \(Y_j=\beta s(U_j)/4\). The other parts of that scalar have zero action here. This geometry avoids identifying a single plaquette with a full scalar without its four-vertex factor.

The conditional action is a seven-site chain. Each consecutive pair contributes \(s(U_iU_{i+1}^{-1})\). Four spatial neighbors at each site and the missing end temporal neighbors contribute pinned edges to a common identity spin, of total weights \(w_i=4+\mathbf 1_{i\in\{0,6\}}\). To generate \(\beta s(U_j)\) first use \(w_j(t)=w_j-t_j\) for \(j=0,3,6\); divide the resulting mixed derivative by \(4^3\). In north coordinates on \(SU(2)=S^3\), a live quaternion is \((\sqrt{1-|y_i|^2/(2\beta)},y_i/\sqrt{2\beta})\). The three components of the tangent Gaussian have the same covariance \(G_t=D_t^{-1}\), where \(D_0\) has diagonal 6 and neighboring entries \(-1\), and \(D_t=D_0-\operatorname{diag}(t)\). The root pinned spin has \(y_*=0\). In these coordinates an edge contributes
\[
 \beta s(U_iU_j^{-1})=\tfrac12|y_i-y_j|^2+
 \tfrac1{16\beta}(|y_i|^2-|y_j|^2)^2+O(\beta^{-2}\mathrm{poly}(y)).
\]
The product surface Jacobian contributes \(\sum_i|y_i|^2/(4\beta)\) at first order. Therefore the first log-partition correction is the explicit function
\[
 L(t)=\frac34\sum_i G_{ii}
 -\frac1{16}\sum_{e=(i,j)}w_e(t)
 [9(G_{ii}-G_{jj})^2+6(G_{ii}^2+G_{jj}^2-2G_{ij}^2)] ,
 \qquad G=G_t,\quad G_{i*}=G_{**}=0.
\]
Unpinned chain edges have weight one. The pinned weights are positive at zero, and the flat minimum is unique. The same compact Laplace argument as (6) gives
\[
 \boxed{\displaystyle
 \kappa_3(Y_0,Y_3,Y_6)=
 \frac1{6688154748928}
 +\frac{1318200203}{3633942857366347382784}\,\beta^{-1}
 +O(\beta^{-2}).}\tag{7}
\]
Both coefficients are strictly positive. The signs are sensitive to the surface Jacobian and the source variation of the edge weights.

To reproduce the rational arithmetic put \(h_0=1,h_1=6,h_{r+2}=6h_{r+1}-h_r\), so \(h_7=235416\). For \(i\le j\), \(g_{ij}=(D_0^{-1})_{ij}=h_i h_{6-j}/h_7\). In the ring \(t_0^2=t_3^2=t_6^2=0\), the coefficient of \(t_S\) in \(G_{ij}\) for \(S\subset\{0,3,6\}\) is \(\sum_{\pi\in\mathrm{Perm}(S)}g_{i\pi_1}g_{\pi_1\pi_2}\cdots g_{\pi_{|S|}j}\), with the empty product interpreted as \(g_{ij}\). Apply this to \(L(t)\), multiplying coefficients by \([t_S]uv=\sum_{A\subset S}[t_A]u[t_{S\setminus A}]v\). Before the four-vertex division, \(3g_{03}g_{36}g_{60}=1/104502417952\) and \([t_0t_3t_6]L=1318200203/56780357146349177856\). No floating point or diagram truncation enters these numbers.

The calculation applies to a positive-probability condition in the full periodic Wilson measure: require the non-live links in the specified finite collars to be simultaneously gauge-equivalent to links within \(\beta^{-4}\) of identity. Conditional on such exterior links, normalized density ratios for the seven live variables are \(1+O(\beta^{-3})\); replacing the three actual scalar stencils by their identity-collar expressions costs \(O(\beta^{-3})\) pointwise after their \(\beta\) factor, by the Lipschitz plaquette trace. All moments required for the cumulant are uniformly bounded as in §4. Averaging those moments on this event leaves (7) intact. Constants here depend only on the fixed collar, independent of the other torus links and of \(n\ge12\). For instance if \(m\) collar links meet \(p\) plaquettes, conditioning on all remaining links and using \(0\le s_p\le4\) yields the crude explicit lower bound \(e^{-4p\beta}(c\beta^{-12})^m\) for the event, by the Haar volume of \(m\) fixed-frame \(SU(2)\) balls of radius \(\beta^{-4}\). This proves volume-uniform positivity at finite \(\beta\) and gives no useful positive asymptotic fraction. The sites stay a fixed number of spacings apart, and the strongly pinned surroundings change the limiting propagator. In particular its Gaussian triple is nonzero. A full-Wilson scalar extraction would have to average the unrestricted exterior and reproduce the separated Gaussian cancellation before identifying its surviving first correction. Equation (7) establishes a positive coefficient and sign-controlled remainder for a restricted conditional Wilson measurement, without identifying it with (299).
