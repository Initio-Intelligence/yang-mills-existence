# Regular conditional and minimizing-reference energy regulators

**Annex BD.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### 0. Selected estimate and exact scope

This annex concerns theorem **M-04** of the catalogue, whose exact statement is:

> At one RG step, expand the actual transported scalar insertion in the fixed incoming reference basis of F-01, under an explicit one-step induction budget, into the current scalar basis, identity term and a localized remainder. Include constrained background, E/B/R responses and coarea terms present in that sector. This does not assume the final running Z from F-05.

The required scope is:

> Equality with Q_k F_k and a remainder estimate in M-03, uniform in scale; the left side is not a freshly inserted coarse plaquette.

The following estimates use the regular-law moment bounds of Annex AY, with all its hypotheses. The conditional expectation still requires a separate carrier expansion.

The scalar matching problem requires the specified incoming norm and the conditional moment bounds of Annex AY.

### 1. The actual regular law used here

Use the reduced regular law of Annexes W, AW and AX subject to CL and the derivative estimates under CR.

\[
 Q_v(dz)=Z_v^{-1}\mathbf1_D(z)
 \exp\{-\tfrac12 z^{\mathsf T}Kz+b^{\mathsf T}z+W(z;v)\}\,dz,
 \qquad b=-K_{IO}y.
 \tag{NP19.1}
\]

Here \(I\) is the set of integrated current free coordinates, \(O\) the retained exterior coordinates of the **same current chart**, and \(y=(y_j)_{j\in O}\). Older-layer variables remain parameters of \(W\); they are not inserted into \(y\). The literal product support \(D\), constrained precision \(K\), full \(W\), and source assumptions are those in Annex AY, Sections 1–4. In particular no current-independent exterior Schur scalar is lost from the outer law.

C-08 supplies fixed positive rates, a covariance majorant \(G\), a nonnegative entrywise Hessian majorant \(A\), and

\[
 H=(I-GA)^{-1}G,\qquad
 \|H\|_a\le C_H,\qquad
 \|K_{IO}\|_a\le C_K,
 \tag{NP19.2}
\]

for one fixed \(a>0\), uniformly over its admitted retained data. With \(d_i=|D_iW(0)|\),

\[
 \sup_{s,t}|Q_{v;s,t}z_i|
 \le\sum_lH_{il}
 \left(|b_l|+d_l+\sigma\sum_n A_{ln}\right),
 \quad
 d_l+\sigma\sum_n A_{ln}\le C/P,
 \tag{NP19.3}
\]

and

\[
 \|z_i-Q_{v;s,t}z_i\|_{L^r(Q_{v;s,t})}\le C\sqrt r,
 \qquad r\ge1.
 \tag{NP19.4}
\]

The interpolation \((s,t)\) and all additional real linear tilts have the same estimates, with their actual force in (NP19.3). These are RC18.28–RC18.36, not additional assumptions about transported observables.

### 2. A pointwise conditional regulator with the exterior field retained

The coarse bound \(P e^{-c\,d(i,O)}\) is useful for collars. For a native polynomial regulator one should retain the actual exterior amplitudes.

#### Theorem NP19.1 — force-resolved local free-coordinate regulator

There are fixed \(C,c>0\) and a nonnegative kernel \(L_{ij}\), \(i\in I,\ j\in O\), such that

\[
 L_{ij}\le C e^{-c\rho(i,j)},\qquad
 \sup_i\sum_j L_{ij}\le C,
 \tag{NP19.5}
\]

and, pointwise at every admitted retained datum,

\[
 |Q_vz_i|\le C/P+\sum_{j\in O}L_{ij}|y_j|,
 \tag{NP19.6}
\]

\[
 \|z_i\|_{L^r(Q_v)}^2
 \le C\left[r+\sum_{j\in O}e^{-c\rho(i,j)}|y_j|^2\right],
 \qquad r\ge1.
 \tag{NP19.7}
\]

For a finite set \(X\) of current free-coordinate blocks put

\[
 E_X(z)=1+\sum_{i\in X\cap I}|z_i|^2,\qquad
 n_X=1+|X\cap I|,\qquad
 a_{Xj}=\frac1{n_X}\sum_{i\in X\cap I}e^{-c\rho(i,j)}.
 \tag{NP19.8}
\]

Set

\[
 \mathcal R_X(y)
 =n_X\left(1+\sum_{j\in O}a_{Xj}|y_j|^2\right).
 \tag{NP19.9}
\]

Then, for all real \(q\ge1\) and \(p\ge1\),

\[
 \|E_X^q\|_{L^p(Q_v)}
 \le C^q(qp)^q\,\mathcal R_X(y)^q.
 \tag{NP19.10}
\]

In particular

\[
 Q_v(E_X^q)\le C^q q^q\mathcal R_X(y)^q.
 \tag{NP19.11}
\]

The constants are independent of the number of integration variables, volume, RG depth, retained history admitted to this regular law, \(p\), and \(q\). The factor \(n_X^q\) is explicit. No moment estimate for the outer law of \(y\) is assumed.

**Proof.** Define

\[
 L=H\,|K_{IO}|,
 \tag{NP19.12}
\]

where absolute values mean block operator norms. Weighted row norms are submultiplicative by the triangle inequality for \(\rho\); hence \(\|L\|_a\le C_HC_K\). This proves (NP19.5), after decreasing the rate if needed. Insert the exact inequality
\(|b_l|\le\sum_j|(K_{IO})_{lj}||y_j|\) in (NP19.3). The nonforce term is at most \(C/P\) by the row bound on \(H\), proving (NP19.6).

By weighted Cauchy–Schwarz and the uniform row bound,

\[
 \left(\sum_jL_{ij}|y_j|\right)^2
 \le\left(\sum_jL_{ij}\right)
       \left(\sum_jL_{ij}|y_j|^2\right)
 \le C\sum_je^{-c\rho(i,j)}|y_j|^2.
 \tag{NP19.13}
\]

Combine this with (NP19.4), \(P\ge1\), and the triangle inequality to obtain (NP19.7). Minkowski's inequality, applied to the finite positive sum defining \(E_X\), gives for every \(r\ge1\)

\[
 \begin{aligned}
 \|E_X\|_{L^r(Q_v)}
 &\le1+\sum_{i\in X\cap I}\|z_i\|_{L^{2r}(Q_v)}^2\\
 &\le C\left[r n_X+
       \sum_{i\in X\cap I}\sum_{j\in O}
             e^{-c\rho(i,j)}|y_j|^2\right]\\
 &\le Cr\,\mathcal R_X(y).
 \end{aligned}
 \tag{NP19.14}
\]

Take \(r=qp\) and use \(\|E_X^q\|_p=\|E_X\|_{qp}^q\). This proves (NP19.10) and (NP19.11). \(\square\)

The earlier logarithmic support bound \(|y_j|\le CP\) would turn the last term in (NP19.7) into \(CP^2\). The new bound avoids that loss by keeping the native retained energies themselves. This matters for the pointwise polynomial part of M-03.

#### Corollary NP19.2 — admitted unit shifts

If one integrated free coordinate is changed by a vector of norm at most one, its local input energy satisfies \(E_X(\tau z)\le3E_X(z)\), whenever that coordinate is in \(X\). Also, if one exterior free coordinate is changed by a vector of norm at most one,

\[
 \mathcal R_X(\tau y)\le C\mathcal R_X(y).
 \tag{NP19.15}
\]

More precisely,

\[
 \left\|\sup_{\tau_I}E_X(\tau_I z)^q\right\|_{L^p(Q_v)}
 \le C^q(qp)^q\mathcal R_X(y)^q,
 \qquad
 \sup_{\tau_O\ {\rm admitted}}
      \|E_X^q\|_{L^p(Q_{\tau_Ov})}
 \le C^q(qp)^q\mathcal R_X(y)^q.
 \tag{NP19.15a}
\]

In the first expression \(\tau_I\) changes one integrated free coordinate. In the second it changes one exterior free coordinate and the actual shifted datum must remain in the same admitted regular family. In particular the latter formula at \(p=1\) is a pointwise bound for the supremum of the conditional values. No outer-law moment is inferred from that pointwise statement.

**Proof.** Use \(|u+t|^2\le2|u|^2+2\), \(E_X\ge1\), and
\(\sum_j a_{Xj}\le C\), which follows from the fixed lattice exponential row sum. Apply Theorem NP19.1 at each shifted admissible datum. The constants are uniform, so the pointwise supremum obeys the same bound. \(\square\)

This corollary is not an ambient-chart extension theorem. M-03 also takes shifts crossing a chart or selector boundary, with its recorded conventions. Such shifts are not included by asserting that all points of a real interior chart are admissible.

### 3. The positive regulator majorant has a thin-path summation

The next result concerns the explicit positive majorant (NP19.9), not the still-unknown support of \(Q_vF\).

#### Proposition NP19.3 — exponential carrier payment for the retained energy majorant

Suppose \(X\) is a connected current block set containing the insertion anchor and the footprints of the listed free coordinates have uniformly bounded current diameter. For every integer \(m\ge1\), expand

\[
 \mathcal R_X(y)^m
 =n_X^m
 \sum_{(j_1,\ldots,j_m)\in(O\cup\{*\})^m}
       \left(\prod_{\ell=1}^m a_{Xj_\ell}\right)
       \prod_{\ell:\,j_\ell\ne *}|y_{j_\ell}|^2,
 \tag{NP19.16}
\]

where \(a_{X*}=1\). For each nonstar index choose one summand in \(a_{Xj}\), with starting point \(i\in X\), and connect \(i\) to \(j\) by a fixed shortest path. Let \(Z\) be \(X\), those paths, and the fixed coordinate-footprint enlargements. For sufficiently small fixed \(\kappa>0\), the sum of the resulting coefficients multiplied by
\(w_h(Z)/w_h(X)\), with \(w_h\) exactly as in M-03, is at most

\[
 C^m n_X^m.
 \tag{NP19.17}
\]

Each energy monomial in (NP19.16) is bounded by
\(R_{h,Z}(y)^m\), provided those \(y_j\)'s are entries in the actual surviving native list. One must include every such entry's full footprint. If a coordinate has a growing or global footprint, its extra cost is not bounded by this proposition.

**Proof.** Adding a path of length \(r\) and a fixed local endpoint footprint increases \(|Z|+\mathsf t_h(Z)\) by at most \(c_1(r+1)\), for one fixed \(c_1\). The ratio of weights is therefore at most the product of
\(\exp[\kappa c_1(\rho(i,j)+1)]\) over the chosen paths. Choose
\(\kappa c_1<c/2\). The weighted sum of one endpoint coefficient is bounded by

\[
 \frac1{n_X}\sum_{i\in X\cap I}\sum_{j\in O}
       e^{-c\rho(i,j)}
       e^{\kappa c_1(\rho(i,j)+1)}
 \le C.
 \tag{NP19.18}
\]

Including the star option changes \(C\) by one. Sum the \(m\) endpoint choices independently; shared paths and repeated indices only reduce the union's weight. This proves (NP19.17). The regulator inequality follows because each \(|y_j|^2\) is one of its nonnegative summands. \(\square\)

This proves a concrete carrier payment for the **majorant**. It avoids the volume of balls of growing radius. It does not identify a term of \(Q_vF\) that depends only on a particular \(Z\). For that, an actual rooted expansion of the marked conditional integral is still needed. Assigning \(Q_vF\) to the small carrier of a pointwise upper bound would be an invalid support claim.

### 4. Precise source opening for a rooted insertion expansion

CMP119, printed pp.277–278, (3.44)–(3.47), gives a useful exact construction. Its numerator has one marked factor \(H'(Z_0)\), and its other activities are the denominator activities. Exponentiating the polymers disjoint from \(Z_0\) cancels those denominator components; the surviving expansion is anchored at the marked root. This is an appropriate starting point for the transported scalar, with every coefficient of its actual projected numerator retained.

The construction there is applied to the specified action-derivative insertions in (3.26), (3.28) and (3.37). Its bounds include the source insertion's own polynomial cutoff factors. It does not state a bounded transport theorem in M-03 for an arbitrary marked input.

CMP116, Section 2, especially (2.14)–(2.26), performs the Gaussian majorant estimates before the final polymer sum. This is the location at which a fixed-degree marked polynomial can in principle be charged to reserved Gaussian energy, rather than bounded by the support radius. The exact current map, physical reference field, and current records must still be carried through that argument. The scalar unmarked activity estimate alone does not do this.

Published sources for these hypotheses:

- T. Bałaban, *Convergent renormalization expansions for lattice gauge theories*, CMP 119 (1988), 243–285, pp.277–278.
- T. Bałaban, *Renormalization group approach to lattice gauge field theories. II. Cluster expansions*, CMP 116 (1988), 1–22, DOI 10.1007/BF01239022, especially pp.12–20.
- T. Bałaban, *The variational problem and background fields in renormalization group method for lattice gauge theories*, CMP 102 (1985), 277–309, Proposition 9 and (190).

### 5. A source-scoped physical-reference regulator on a deep regular patch

Theorem NP19.1 controls the actual integrated free coordinates. A physical incoming plaquette also sees its constrained reference field. In C-08 the current connection has the form

\[
 U_e(t)=e^{ia_{v,e}(t)}V_e,\qquad
 a_v(t)=gC_vt-h_vD_v(gC_vt).
 \tag{NP19.19}
\]

The source derivative estimate gives

\[
 g^{-1}|a_{v,e}(t)|
 \le C\sum_i e^{-c\rho(e,i)}|t_i|,
 \tag{NP19.20}
\]

on its admitted current segment. For a fixed plaquette, the compact product inequality therefore bounds its normalized energy by the reference energy and a fixed exponential convolution of \(|t_i|^2\). Combining that inequality with Theorem NP19.1 controls the fluctuating part.

The reference field here is the actual
\(V^{(k)}=\mathcal M^k(U_{k+1})\). In the source notation \(U_{k+1}\) is a minimal fine configuration depending on the retained determining averages. CMP102 p.305 explicitly distinguishes \(U_k(V)\) from its determining coordinates \(V\). Thus the fine plaquettes of \(U_{k+1}\) cannot simply be inserted into the surviving independent-coordinate regulator.

C-08's RC18.49a proves the absolute estimate
\(g^{-2}s(V^{(k)}_p)\le CP^2\). That estimate is insufficient by itself for the cutoff-uniform pointwise quotient in M-03. The stronger bridge considered here is

\[
 g^{-2}s(V^{(k)}_p)
 \le C\left[
       1+\sum_{p'\ {\rm surviving}}
          e^{-c\rho(p,p')}\beta_{p'}s(V^{\rm out}_{p'})
       \right].
 \tag{NP19.21}
\]

The positive constant in (NP19.21) pays the distant boundary of the large regular patch. Every plaquette on the right belongs to the actual surviving determining configuration, with its stated scale and footprint.

#### Theorem NP19.4 — the actual local minimizing-field energy bound

Work in the current physical units and fix a plaquette \(p\) whose complete current averaging stencil is inside a regular cube. The entire cube and the fixed source margins used below must be contained in the **deepest original determining region \(\Omega_{k+1}\)**. Suppose the cube has a margin of \(M\) current units, where \(M\) is an allowed multiple of the fixed source block constant. Use the actual minimizing fine configuration and actual determining averages of CMP119 (3.10), with the source local regularity conditions on that enlarged cube. Write \(\epsilon_0\) for their current normalized bound. Assume

\[
 C_{\rm loc}M\epsilon_0\le\epsilon_*,
 \tag{NP19.22}
\]

where the two constants are fixed sufficiently small/large according to the source local minimizing-map domains. The bound \(\epsilon_0\) covers both curvature and the source covariant-divergence regularity in CMP102 (2); the curvature inequality CMP119 (3.12) alone is not substituted for that full admitted regularity class. No bound is imposed on a number of microscopic bonds.

Then, with fixed \(C,c>0\),

\[
 \left\|V^{(k)}(\partial p)-1\right\|
 \le C\sum_{p'\in\mathcal P_M}
       e^{-c\rho(p,p')}
       \left\|V^{\rm out}(\partial p')-1\right\|
      +CM\epsilon_0e^{-cM}.
 \tag{NP19.23}
\]

Here \(\mathcal P_M\) consists of the actual next-scale determining plaquettes in the chosen cube, not fine plaquettes of the minimizing field. Their current distances are converted to next-scale distances only by the fixed block factor \(L\). Constants depend on the source group and fixed geometric parameters, not \(M\), the fine mesh, depth, volume or the exterior history.

On an actual deep regular patch one can choose \(M\asymp R_k\asymp\ell_k^r\), \(r>1\), with \(\epsilon_0\le Cg_k\ell_k^q\) from the admitted current regularity class. Then (NP19.22) holds at a fixed sufficiently small coupling ceiling. If the next-step native inverse coupling obeys the source-normalized comparison

\[
 c_\beta g_k^{-2}\le\beta^{\rm out}\le C_\beta g_k^{-2},
 \tag{NP19.24}
\]

the bound (NP19.21) follows, with a uniform constant. The comparison (NP19.24) is part of the same admitted one-step coupling trajectory; this theorem does not prove B-03 or identify a new bare coupling.

**Proof.** The local construction needed here is already in CMP102, Section F, rather than an unproved interpolation from an arbitrary global field to the identity. Its precise roles are the following.

1. In (144)–(150) the source restricts the actual minimum to a nested family of local cubes and fixes its own auxiliary boundary averages. The source explains immediately after (150) that it remains a minimum for this more restricted local problem. The determining coordinates in the inner deepest grid are the original ones. Artificial finer determining grids occur only in the constructed boundary region. Our deep-patch choice makes the original mixed set \(\square'_k{}^{(k-1)}\) in the proof of (160) empty: the whole inner determining grid is the actual next-scale \(V_{k+1}\) grid. The artificial finer boundary data are retained and estimated separately below.

2. Equations (151)–(157) put this local problem, after the stated gauge changes, into the **exact** nonlinear constraint chart about the identity. No one-step exceptional-bond map is substituted for the fine multiscale constraint. In the source notation,

\[
 A=A_1+HB-HD(A_1+HB),\qquad
 A_1+\mathcal G\,V'(A_1+HB)=0.
 \tag{NP19.25}
\]

These are (158)–(159), with \(\mathcal G\) denoting the source's constrained covariance operator. The functional \(V\) in (157) begins cubically. Its derivative at zero is zero and its derivative Lipschitz constant on the relevant small ball is \(C\epsilon\), where \(\epsilon=C_{\rm loc}M\epsilon_0\). The exact constraint correction \(D\) begins quadratically. The source explicitly states below (158) that these operators have identity external field. The constructed source coordinates satisfy all the required physical first-, second-, and higher regularity norms with bound \(C_{\rm loc}M\epsilon_0\).

3. The defining gauge is a generalized axial gauge rooted at a point next to the marked plaquette. In (154) the field \(B\) is the actual logarithmic determining input for this local problem. Equation (155) bounds it globally by \(CM\epsilon_0\). On the inner determining grid, the path argument preceding (160) expresses it in terms of the actual determining plaquettes. Its usual uniform \(\epsilon_1\) bound can be sharpened by retaining each plaquette separately, as below.

We first make the weighted estimate in (NP19.25) explicit. Let \(d_{\Omega'}\) be the source weighted metric for the nested local cubes, and put

\[
 w(y)=e^{-\sigma d_{\Omega'}(x_p,y)}
 \tag{NP19.26}
\]

for a fixed sufficiently small \(\sigma>0\). Weight the source physically normalized field norms by \(w\). For example, on a determining block of proper size \(h_j\), the value and first-gradient weights are \(h_j|A|\) and \(h_j^2|\nabla A|\). The corresponding forcing norm has weight \(h_j^3\). Use those physical factors, not the norm of an unrescaled matrix on the fine lattice.

The triangle inequality gives \(w(y)/w(y')\le e^{\sigma d_{\Omega'}(y,y')}\). The pointwise kernels of \(H,\mathcal G\), and their required output derivatives have a fixed exponential in this metric. Reserving \(\sigma\) of that exponential and applying the same physical weighted row sums used in CMP102 (161)–(162) therefore gives uniform operator bounds on these weighted norms. In particular, the factors \(h_j^{-1}\) occurring explicitly in the sum in (161) are retained and summed by that source estimate; they are not replaced by a microscopic counting measure. The geometry of the nested cubes is exactly the source geometry in (144), so these row constants do not grow with \(M\) or fine depth.

For the nonlinear functions one uses the same argument as for the weighted contraction in BM.8–BM.9. To specify the factors covered by that argument, let \(\mathscr D=\partial^{\eta *}\partial^\eta\) be the identity-background quadratic operator and set \(F(A)=A-HD(A)\). The exact functional in source (157) gives

\[
 \begin{aligned}
 V(A)&=\tfrac12\langle F(A),\mathscr D F(A)\rangle
        +V_0(F(A))-\tfrac12\langle A,\mathscr D A\rangle,\\
 V'(A)&=-\mathscr D HD(A)
        -D'(A)^*H^*\mathscr D F(A)
        +(I-D'(A)^*H^*)V_0'(F(A)).
 \end{aligned}
 \tag{NP19.26a}
\]

All adjoints are in the source physical scalar products. The adjoint, derivative, and propagator compositions in this display are the ones estimated in the source's actual derivative calculation (85)–(97); their differentiated physical kernels and measures are retained. The exponential Hessian estimate (189) is a further explicit source bound for this derivative calculation, with the proper \(h_j^{-3}\) forcing factor and the source input norms retained. It supports the same physical weighted contraction; it is not an identification with the derivative of a different composed map. Thus “every occurrence” includes those compositions, not only the undifferentiated \(H\). The local nonlinear averaging equation for \(D\) has \(N(0)=DN(0)=0\) and
\(D=N(A-HD)\); its derivative solves
\((I+N'(F)H)D'=N'(F)\). Its weighted Neumann series has the same small fixed ceiling.

Every local analytic factor has bounded proper-scale footprint. In a difference, assign the weight to the differing factor and use the source global small bound for all its other factors. Every physical kernel, including the adjoint/derivative kernels just specified, loses only \(\sigma\) of its exponential. Its row sums, with the source measure weights, remain bounded as above. The cubic \(V_0\), the quadratic \(D\), and their exact products in (NP19.26a) then give one factor of the global small radius in the derivative Lipschitz bounds. This proves, on the actual source ball,

\[
 \begin{split}
 \|\mathcal G[V'(A')-V'(A'')]\|_w
     &\le C\epsilon\|A'-A''\|_w,\\
 \|HD(A')\|_w&\le C\epsilon\|A'\|_w.
 \end{split}
 \tag{NP19.27}
\]

All these are physical source norms. The derivation uses the actual factors in the nonlinear source equations, rather than identifying the derivative of a different composed map with \(V'\). An absolute fine-mesh Schur bound for a matrix with entries of size \(\eta^{-2}\) is neither asserted nor needed.

Choose the fixed ceiling in (NP19.22) so that \(C\epsilon\le1/4\). Since \(V'(0)=0\), (NP19.25) and (NP19.27) imply

\[
 \|A_1\|_w\le
 \frac{C\epsilon}{1-C\epsilon}\|HB\|_w,\qquad
 \|A\|_w\le C\|HB\|_w\le C\|B\|_w.
 \tag{NP19.28}
\]

The final input norm is explicitly
\(\|B\|_w=\sup_c w(y_c)|B(c)|\), where \(y_c\) is the source determining-block label of \(c\). Thus \(B\) has no extra microscopic power. This is the weighted version of the dimensionless input norm in CMP102 (45)–(46). The preceding kernel argument, and the physical row sum in (161)–(162), specify how the scale factors in the operator are paid.

It remains to estimate this input using actual curvature. On this inner deepest grid the source has \(B(c)=i^{-1}\log V'(c)\), as in the first case immediately preceding (160). The generalized axial gauge writes the group element \(V'(c)\) as a product of conjugates of the actual determining plaquette holonomies in an axial surface \(\Sigma_c\). All conjugating factors are compact and unitary at the real retained data. The elementary telescoping inequality for products of unitaries yields

\[
 |B(c)|
 \le C\sum_{p'\in\Sigma_c}
       \|V^{\rm out}(\partial p')-1\|.
 \tag{NP19.29}
\]

The fixed principal logarithm exists by (155) and (NP19.22), and its norm is bounded by a fixed multiple of the group difference. The surface lies in a coordinate rectangle rooted at \(x_p\); every \(p'\in\Sigma_c\) has distance at most \(C[\rho(x_p,c)+1]\) from that root. Its multiplicity is bounded by a fixed polynomial in that distance. Multiplying by \(w(c)\), spending half its exponential to pay this polynomial, and then taking the supremum in \(c\) gives

\[
 \|B_{\rm inner}\|_w
 \le C\sum_{p'\in\mathcal P_M}
       e^{-c\rho(p,p')}
       \|V^{\rm out}(\partial p')-1\|.
 \tag{NP19.30}
\]

There is no assertion here that the second, adjacent-original-layer case of source (160) is an exact holonomy product of \(V_{k+1}\) plaquettes. That case uses the additional finer input and the one-step estimate of the cited gauge-fixing lemma. Applying the present theorem to a cube meeting such an original layer would require retaining its actual finer inputs and scales. The deep-patch hypothesis excludes that extension.

For the auxiliary boundary determining grids use (155), retaining the actual root-to-boundary distance in the first sum of (161). That distance is at least \(cM\); the final uniform estimate in the printed (161) had replaced it by a fixed minimum because it was estimating every point of a large cube simultaneously. A fixed further exponential-rate reserve pays the finer-layer physical factors exactly as in (162). The result is

\[
 \|HB_{\rm boundary}\|_w\le CM\epsilon_0e^{-cM}.
 \tag{NP19.31}
\]

One may use (NP19.31) directly in (NP19.28); no claim that an unweighted fine-node sum is bounded is involved.

At the marked root and a fixed neighborhood the weight in (NP19.26) is bounded below. The bounds on \(A,\nabla A\), and the elementary plaquette expansion of \(e^{i\eta A}\), give fine curvature bounded by \(\eta^2\) times the sum of (NP19.30) and (NP19.31). The quadratic terms cost one extra small global norm and are absorbed in \(C\). Finally apply the actual uniform-depth averaging estimate BM.20–BM.21 on the fixed current stencil. Its entire footprint lies in the marked neighborhood. This gives the actual averaged plaquette bound (NP19.23), not a linearized or a newly inserted average.

For (NP19.21), use \(\|U-1\|_{\rm HS}^2=2s(U)\), fixed norm equivalence, the uniform row sum of the exponential plaquette kernel, and weighted Cauchy–Schwarz. The square of the first term in (NP19.23), divided by \(g_k^2\), is at most
\(C\sum_{p'}e^{-c\rho(p,p')}\beta^{\rm out}s(V^{\rm out}_{p'})\) by (NP19.24). The squared boundary error divided by \(g_k^2\) is bounded by
\(C M^2\ell_k^{2q}e^{-2cM}\) on the chosen patch, hence by a fixed constant. This proves the claimed energy inequality. \(\square\)

The theorem uses the original source local-minimizer construction and its weighted physical kernels. It does not enlarge a current scalar density theorem to arbitrary raw marked kernels. It supplies a value-regulator estimate on a deep admitted regular patch. The separate derivative/support/history records in M-03 still require their actual constructions.

### 6. Application conditions

The regulator estimates apply on the stated conditional law and minimizing-reference patch.

For the estimate, the following still require proof for the **same** actual incoming scalar mark:

1. A root-insertion expansion with termwise native-regulator bounds, complete current records and an M-03 carrier sum; the already-proved positive majorant is not this expansion. A source completed-operation norm that does not charge a fixed nonsmall component's interior cannot simply pay the full M-03 physical carrier weight.
2. The retained-coordinate pullback, common support or compatible extension, and shifted-envelope bounds for all actual directions included in M-03. The stated native inner-current contour does not stand for every raw retained or history direction.
3. The scalar/identity extraction from that exact output in the F-01 reference basis, with the remaining localized terms bounded in the same norm.
