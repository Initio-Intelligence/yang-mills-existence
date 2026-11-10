# Raw-data matching and bounded source gauge conversion

**Annex AP.** The complete Wilson application assumes CL (compatibility of the conditional representation) and CR (uniform composed reconstruction response with the prescribed earlier innovations and raw variables fixed). The ordinary and completed sectors must control the same subtracted primitive, with its actual support, tags, connectors, stopped prefixes and repeated histories. The two-age estimate must retain both the evaluation and forcing ages. These are uniform hypotheses for the all-history application. [Boundary induction](../boundary/boundary_induction.md) · [Conditional response and the continuum application](../continuum/conditional_to_continuum.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

The first route in this note distinguishes the actual symmetric raw average from its associated reference-corrected relative average. It does not equate those maps. The main new route instead takes an arbitrary admitted input configuration as the reference background and prescribes its own exact determining data. The relative datum is then exactly zero. This removes the need to match derivatives of two separately gauged input families.

The estimates below concern the analytic variational problem on one admitted determining geometry. Their application to the actual tuple, complete B domain and selected source representative is retained separately. This annex does not complete C-05.

### 1. The symmetric operator family must be selected consistently

CMP109, pp.253–254, defines the symmetric averaged transports in (0.11) and the raw block average in (0.12). The same text states that the preceding averaging results apply to this average. This is a primary-source transfer statement. Thus one may use the reference-corrected averaging construction associated with this actual symmetric average and its transports. One may not silently identify the corrected derivative with the uncorrected raw derivative, or combine kernels from different choices.

At one step, write \(M\) for the raw source average and \(T_U(y,x)\) for its endpoint-equivariant averaged transport. Its associated corrected relative map has the form displayed in CMP99 (3.113): the raw relative average is conjugated at its two endpoints by the averages of the relative transported fields. At a fixed real background its linearization obeys

\[
 q(A)=m(A)+D^{\rm coarse}\xi(A),\qquad
 |\xi(A;y)|\le Ch\sup_{B(y)}|A|.
 \tag{RM.1}
\]

Here \(m\) is the derivative of the raw average, \(q\) the corrected derivative and \(h\) the physical coarse spacing. The bound follows by differentiating the path logarithms and summing their physical lengths. For this associated family, differentiated gauge covariance gives \(QD=D^{\rm coarse}Q'\).

These are levelwise identities. A complete arbitrary-tangent proof still has to match the endpoint corrections on the mixed determining geometry. A coarse determining bond can have an endpoint which belongs to an earlier, finer shell. Independently chosen corrections at every level are not automatically one gauge on that mixed set.

### 2. Exact zero relative datum

Fix an admitted background \(U_0\), and prescribe the raw determining data

\[
 V=M_{\mathcal B}U_0.
 \tag{RM.2}
\]

In the relative coordinate \(U=U'U_0\), the input point is \(U'=1\). Every relative transport, relative average and endpoint correction is the identity there. Consequently the corrected determining datum used in the variational problem is exactly

\[
 B=0.
 \tag{RM.3}
\]

This is an equality at the defining relative map, rather than an equality of two different tangent operators. It is valid on a mixed determining set because every component is evaluated at the identical reference field. The assertion does not require an arbitrary off-minimum input to equal its reconstructed minimum.

The constructed correction may use a different analysis coordinate while producing the same physical critical orbit. CMP102 p.287 explicitly permits a different linearizing right inverse \(h\) in the map \(A=A'-hD(A')\). This freedom is used below to obtain a regular current kernel without an unproved profile extension of a global estimate.

### 3. A right inverse with checked current kernels

Let \(\mathsf H\) be the dimensionless-data version of the source operator \(H_1\). Thus

\[
 h_b(Q\mathsf H B)(b)=B(b),\qquad RD^*\mathsf H B=0.
 \tag{RM.4}
\]

The source expansion CMP102 (174)–(177) states that its physical relative-Landau field satisfies

\[
 \mathcal A(B)=\mathsf H B+O(B^2).
 \tag{RM.5}
\]

The physical field, including the linearizing correction, is used in this expansion. CMP102 (190) gives its value, first-gradient, \(D^*D\) and component-Laplacian derivative kernels. Page 309 explicitly extends those bounds to the admitted arbitrary regular external background. Differentiating (RM.5) at zero therefore supplies

\[
 |\mathcal L_r\mathsf H(x,b)|
 \le C h_a^{-1-r}h_b^{-d}e^{-\delta d(a,b)},
 \quad x\in\Delta(a),\quad d=4,
 \tag{RM.6}
\]

where \(r=0,1\) means value and covariant first gradient. For \(r=2\), one may use \(D^*D\), the component covariant Laplacian, or the physical quadratic Wilson Hessian \(\Delta\). The last follows from the source local bounded curvature correction relating \(\Delta\) to \(D^*D\). The field \(\mathcal A(B;U_0)\) used to read this linear kernel need not be interpreted as a physical minimum for an off-minimum external \(U_0\). Only its explicitly stated analytic kernel estimate is used.

#### Which external-background extension is used

The right-inverse and Landau identities in (RM.4) are available before the nonlinear minimizing problem. CMP99 (3.127)–(3.129) defines \(H_1\), for an arbitrary admitted regular external \(U_0\), as the solution of its quadratic variational problem with the restrictions \(QA=B\), \(RD^*A=0\). Its formula is \(G_1Q^*(QG_1Q^*)^{-1}\), with the dimensionless-data conversion indicated there. These identities do not assume that \(U_0\) is a minimum.

For the current kernel we use specifically the formal analytic extension of the family (174), (175) licensed by CMP102 p.309 and Proposition 9. In that family the remainder \(V\) is cubic for every admitted external background: in particular its current-dependent term is \(-\langle HD_3,J_0\rangle\), not a linear term. Therefore the fixed-point solution \(\mathcal A_1(B)\) has \(\mathcal A_1(0)=0\) and \(\mathcal A_1'(0)=0\), even when \(J_0\ne0\). The exact expression (174) then gives \(\mathcal A'(0)=H_1\). The bound (190) is used as the explicitly stated primary bound on this analytic extension.

We do not identify the off-minimum continuation defined by (174), (175) with any continuation obtained from (179), (180) merely because both describe the physical family when the reference is minimal. The selected formal continuation here is used only to read the linear operator kernel; it is not used as an off-minimum physical minimizer.

Its external-background assumptions are the full ones printed in CMP99 (3.35)–(3.38). A real reference has local gauges with value, first difference and \(d^*d\) bounds \(CM\alpha_0(h^{-1},h^{-2},h^{-3})\). A complex reference \(e^{i\eta A_0}U_*\), with \(U_*\) real, has value, covariant first-gradient and \(D_{U_*}^*D_{U_*}\) bounds \(\alpha_1(h^{-1},h^{-2},h^{-3})\). The source smallness conditions on \(M\alpha_0,\alpha_1\) are retained. A native ball used in the application must imply these conditions.

All transposes below use the physical fine measure \(\eta^d\) and determining measure \(h_b^d\). On a complex chart they are analytic bilinear transposes.

### 4. Profiles and the exact linearizing map

Let \(h_a\) be the local joined determining mesh, \(h_n\) the old physical mesh at that point, and assume

\[
 h_a\le h_n,\qquad
 w_a=\alpha_nh_n^{-3},\qquad
 e_a=h_a^3w_a,\qquad
 e_*=\sup_a e_a\le\alpha_*.
 \tag{RM.7}
\]

Use the admitted profile comparison and exponential row-sum reserves for \(w,e,e^2\). These follow from the source metric and a fixed sufficiently large layer separation, just as in CC.1–CC.4. No reserve depends on derivative order or total volume.

Set

\[
 \|A'\|_{X_w}
 =\sup_a\max\left\{
   \frac{\|A'\|_{\infty,\Delta(a)}}{h_a^2w_a},
   \frac{\|\nabla A'\|_{\infty,\Delta(a)}}{h_aw_a}
 \right\}.
 \tag{RM.8}
\]

Assume \(\|A'\|_{X_w}\le\rho\), and that the physical input current satisfies \(|J_0|\le\mu w\). The small parameters \(\rho e_*\) and \(\mu e_*\) are required to fit one fixed absolute source radius.

Write the source averaging remainder as in CMP102 (44),

\[
 \mathcal Q_j(A)=h_jQ_jA+C_j(h_jA).
\]

Use \(\mathsf H\) in the exact fixed-point equation

\[
 D(A')_b
 =C_j\!\left(h_b[A'-\mathsf H D(A')]\right)_b.
 \tag{RM.9}
\]

Then the field

\[
 A=A'-\mathsf H D(A')
 \tag{RM.10}
\]

has corrected nonlinear determining datum \(hQA'\). The identity is algebraic: apply \(hQ\mathsf H=I\) and (RM.9). In particular \(QA'=0\) gives the desired zero relative datum. Since \(RD^*\mathsf H=0\), a Landau field \(A'\) produces a Landau field \(A\).

#### Lemma RM.1 — the quadratic profile is retained

For \(\rho e_*\) sufficiently small, independently of the number of layers, (RM.9) has a unique analytic solution in the fixed-point ball, and

\[
 |D(A')_b|\le C\rho^2e_b^2.
 \tag{RM.11}
\]

Consequently

\[
 \begin{split}
 |\mathsf H D(A')|(x)&\le C\rho^2h_a^{-1}e_a^2,\\
 |\nabla\mathsf H D(A')|(x)&\le C\rho^2h_a^{-2}e_a^2,\\
 |\Delta\mathsf H D(A')|(x)
   +|\Delta_{\rm cov}\mathsf H D(A')|(x)
   &\le C\rho^2h_a^{-3}e_a^2.
 \end{split}
 \tag{RM.12}
\]

The last line is at most \(C\rho^2e_*w_a\).

**Proof.** The source local remainder bound (44) is quadratic in the actual local dimensionless input. The value kernel in (RM.6), summed against \(e^2\), gives
\[
 |\mathsf H D|(x)\le C h_a^{-1}e_a^2\|D\|_{e^2}.
\]
The local stencil comparison makes the normalized argument of \(C_j\) at \(b\) at most
\(C(\rho e_b+\|D\|_{e^2}e_b^2)\). On a ball
\(\|D\|_{e^2}\le C_D\rho^2\), its square is at most \(C\rho^2e_b^2\), provided \(\rho e_*\) is small. Choose \(C_D\) first and the common smallness ceiling next.

For two candidates, the local analytic derivative of the quadratic remainder is bounded by a constant times the sum of the two local argument norms. The difference of their arguments is bounded by \(Ce_b^2\|D_1-D_2\|_{e^2}\). After division by \(e_b^2\), the Lipschitz constant is at most \(C\rho e_*\). Reduce the ceiling to make it less than \(1/2\). This proves existence, uniqueness and analyticity in the fixed-point ball. The remaining rows of (RM.6) give (RM.12). All sums use the actual physical determining measure. \(\square\)

#### The change of analysis coordinate is locally invertible

On one fixed smaller ordinary source ball, \(A=A'-\mathsf H D(A')\) is an analytic bijection onto a neighborhood of zero. To see this directly, set \(A'=A+\mathsf H X\) and solve
\[
 X=D(A+\mathsf H X).
 \tag{RM.12a}
\]
The quadratic value bound and the first derivative estimate below make this a contraction on the ordinary dimensionless coarse-field ball, exactly as in CMP102 (59)–(62). Its derivative is \(O(\epsilon)\), with \(\epsilon\) the absolute source size. The first-gradient bounds of \(\mathsf H\) show that the map and inverse preserve the smaller ordinary strong ball.

The identity \(\mathcal Q(A)=hQA'\) shows that this bijection maps every linear determining fiber onto the corresponding nonlinear corrected fiber. Both directions preserve the Landau condition because \(RD^*\mathsf H=0\). Consequently a previously constructed physical critical solution, after its source reduction to this corrected fiber, is carried to a critical solution in these coordinates. This change does not alter its physical orbit, nor any old integration variable.

### 5. Derivative kernels of the changed linearizing map

The proof of CMP102 (65)–(73) uses the value/gradient kernel of its chosen right inverse and the pointwise derivative (72) of the local averaging remainder. The same differentiation of (RM.9), with (RM.6), gives

\[
 |D'(A';b,x)|
 \le C\epsilon\,h_a^{1-d}e^{-\delta_1d(a,b)},
 \qquad \epsilon=C\rho e_*,
 \tag{RM.13}
\]

where \(x\in\Delta(a)\). The constant \(\delta_1>0\) is a fixed smaller rate.

For completeness, the first term in the differentiated equation is the local kernel
\(h_b C_j'(h_b[A'-\mathsf H D])\); the checked source bound (72) makes it at most \(C\epsilon h_b^{1-d}\) on its actual stencil. Composing it with \(\mathsf H\) gives a determining-space kernel bounded by
\(C\epsilon h_c^{-d}e^{-\delta_1d(b,c)}\). Its Neumann series converges by the fixed source row-sum reserve. The resulting local-to-global composition is (RM.13). Thus no pointwise transpose estimate for the bare raw averaging operator is inserted.

Let \(D_3=D-C^{(2)}\), with the quadratic normalization used in CMP102 (56). The quadratic coefficient of (RM.9) is still \(C^{(2)}\), independently of the selected right inverse. Analytic coefficient extraction from (RM.13), on a fixed larger absolute value ball, gives

\[
 |D_3'(A';b,x)|
 \le C\epsilon^2 h_a^{1-d}e^{-\delta_1d(a,b)}.
 \tag{RM.14}
\]

Indeed the linear term of \(D'(tA')\) is the derivative of \(C^{(2)}\). Cauchy on a circle of radius proportional to the fixed absolute analytic radius divided by \(\epsilon\) bounds the remaining terms by \(C\epsilon^2\), with the same smaller rate. This is the same coefficient argument stated after CMP102 (73), now with the selected right inverse.

### 6. The full unrestricted action, with no discarded gauge term

Use the actual quadratic Wilson Hessian \(\Delta\). Define the action in the changed coordinate exactly:

\[
 \mathcal F(A')
 =S\!\left(\exp(i\eta[A'-\mathsf H D(A')])U_0\right).
 \tag{RM.15}
\]

Expand the original Wilson action as
\(S(\exp(i\eta A)U_0)=S(U_0)+\langle A,J_0\rangle+
\frac12\langle A,\Delta A\rangle+V_0(A)\). Then

\[
 \mathcal F(A')
 =S(U_0)+\langle A',J_0\rangle+
   \frac12\langle A',(\Delta-D_{2,\mathsf H})A'\rangle+
   V_{\mathsf H}(A'),
 \tag{RM.16}
\]

where
\[
 \langle A',D_{2,\mathsf H}A'\rangle
 =2\langle\mathsf H C^{(2)}(A'),J_0\rangle
\]
and
\[
 \begin{split}
 V_{\mathsf H}(A')={}&-\langle\mathsf H D_3(A'),J_0\rangle
 -\langle A',\Delta\mathsf H D(A')\rangle\\
 &+\tfrac12\langle\mathsf H D(A'),\Delta\mathsf H D(A')\rangle
 +V_0(A'-\mathsf H D(A')).
 \end{split}
 \tag{RM.17}
\]

This identity is defined for unrestricted sufficiently regular \(A'\). It does not replace \(\Delta\) by a gauge-invariant extension off the Landau slice, and it does not delete the cross term using an orthogonality valid only on a restricted tangent space.

The local Hessian estimate CC.3a applies with the selected right inverse: its proof uses the local averaging derivative and the actual multiplier. The adjoint row in (RM.6) gives
\[
 |(\mathsf H^*J_0)(b)|\le C\mu h_b^{-1}w_b.
\]
Equivalently the dimensionful multiplier has size \(C\mu w_b\). Thus
\[
 |D_{2,\mathsf H}A'|(x)
 \le C\mu\rho e_a w_a
 \le C\mu\rho e_*w_a.
 \tag{RM.18}
\]

#### Lemma RM.2 — weighted remainder gradient

On \(\|A'\|_{X_w}\le\rho\), with the above fixed smallness reserves,
\[
 \|V_{\mathsf H}'(A')\|_{F_w}
 \le C\rho^2e_*(1+\mu e_*),
 \qquad
 \|f\|_{F_w}=\sup_a w_a^{-1}\|f\|_{\infty,\Delta(a)}.
 \tag{RM.19}
\]
On a smaller fixed-fraction ball its derivative has norm
\[
 \|V_{\mathsf H}''(A')\|_{X_w\to F_w}
 \le C\rho e_*(1+\mu e_*).
 \tag{RM.20}
\]

**Proof.** Differentiate every term of (RM.17). The exact contributions are
\[
 \begin{split}
 &-D_3'(A')^*\mathsf H^*J_0,\\
 &-\Delta\mathsf H D(A')-D'(A')^*(\Delta\mathsf H)^*A',\\
 &D'(A')^*\mathsf H^*\Delta\mathsf H D(A'),\\
 &(I-D'(A')^*\mathsf H^*)\,V_0'(A'-\mathsf H D(A')).
 \end{split}
 \tag{RM.21}
\]
The equality \(\mathsf H^*\Delta A'=(\Delta\mathsf H)^*A'\) is an adjoint-kernel identity with the fixed source boundary conditions. It moves the second-order operator onto the checked current kernel, rather than requiring a generic second derivative of \(A'\).

The physical-measure row sums of (RM.6) and (RM.13) give the following mapping rules:
\[
 \begin{array}{ll}
 \mathsf H^*:F_w\longrightarrow h^{-1}w,&
 (\Delta\mathsf H)^*:h^2w\longrightarrow h^{-1}w,\\
 D'(A')^*:h^{-1}w\longrightarrow C\epsilon\,w,&
 D_3'(A')^*:h^{-1}w\longrightarrow C\epsilon^2w.
 \end{array}
 \tag{RM.22}
\]
For example the second rule contains the sum
\[
 h_b^{-1}w_b
 \sum_a(h_a/h_b)^{d-1}
     e^{-\delta d(a,b)}\,w_a/w_b,
\]
which is bounded by the reserved metric rate. This displays the physical-volume factors; no fine-bond counting factor is hidden.

The first line of (RM.21) is bounded by \(C\mu\epsilon^2w\). By (RM.12), the first term in its second line is at most \(C\rho^2e_*w\); the second is at most \(C\rho\epsilon w\). The third line is at most \(C\epsilon\rho^2e_*w\).

For the final line, write \(A=A'-\mathsf H D(A')\). It has value and first-gradient bounds \(C\rho h^2w,C\rho hw\). The local Wilson remainder estimates of CMP102 (39)–(40), (90)–(96) give
\[
 |V_0'(A)|(x)\le C\rho^2h_a^3w_a^2
              =C\rho^2e_aw_a.
 \tag{RM.23}
\]
The leading cubic terms are bounded by \(C|A||\nabla A|\); the remaining analytic plaquette terms have the additional local small-field or \(\eta/h_a\) factors described there. The finite fine-stencil sums preserve the old profile, and \(\eta\le h_a\). The prefactor \(I-D'^*\mathsf H^*\) multiplies this by at most \(1+C\epsilon\), using (RM.22). Combining the four lines proves (RM.19).

All functions are holomorphic on a fixed larger \(X_w\) ball because the absolute source radius is fixed and \(\rho e_*\) is small. One-dimensional Cauchy in a normalized \(X_w\) direction, using (RM.19) on that larger ball, proves (RM.20). The constants include only fixed radius fractions. \(\square\)

### 7. What this gives to the zero-data bootstrap

For an actual physical critical configuration in the relative Landau slice, the unrestricted constrained first variation of (RM.16) gives
\[
 \langle v,J_0+(\Delta-D_{2,\mathsf H})A'
                       +V_{\mathsf H}'(A')\rangle=0
 \quad\text{for every }Qv=0.
 \tag{RM.24}
\]
With \(QA'=0\) and \(RD^*A'=0\), the regular constrained covariance yields
\[
 A'=-C_0J_0+C_0D_{2,\mathsf H}A'
                    -C_0V_{\mathsf H}'(A').
 \tag{RM.25}
\]
Equations (RM.18)–(RM.20), together with CC.3, give a contraction on a ball of radius \(C\mu\) in the weighted value/gradient norm, with the component-Laplacian estimate supplied by \(C_0\). The small coefficient is \(C\mu e_*\), after fixed constants have been chosen.

Equation (RM.25) by itself does not impose the Landau gauge. The correct identification step is to use the actual physical source solution, transform it by the invertible analytic map (RM.9)–(RM.10), and verify that it satisfies the same equation in the enclosing ordinary source ball. Uniqueness there identifies it with the weighted fixed point. This step, and the holomorphic continuation in the actual input chart, belong to the enclosing bootstrap theorem.

Once that identification is supplied, the physical field correction \(A=A'-\mathsf H D(A')\) has the old-layer field, gradient and current profiles. In particular the extra linearizing current is bounded by \(C\mu^2e_*w\), with no \(h_n/h_a\) loss. The exact current chart conversion and source representative must still be carried into the complete B-domain application.

### 8. Remaining scope and source analysis

The zero relative datum (RM.3) avoids the arbitrary raw-data tangent matching problem. It does not assert that the associated corrected derivative equals the raw symmetric derivative. The mixed endpoint issue in Section 1 remains relevant to any proof using that stronger tangent identification.

The proof uses the following checked primary statements:

- CMP109 pp.253–254, (0.11)–(0.12), symmetric transport/averaging and the explicit transfer of earlier averaging results.
- CMP99 (3.113)–(3.117), corrected relative averages and physical Ward identities.
- CMP102 pp.285–289, (44), (49), (55), (65)–(73), exact analytic linearization and reproduced pointwise derivative; p.287, freedom to choose the linearizing right inverse.
- CMP102 pp.305–309, (174)–(177), (190), and Proposition 9, the first coefficient \(H_1\) and its regular current kernels, including the stated regular external-background extension.
- CMP102 (39)–(40), (90)–(98), local nonlinear Wilson derivative estimates.
- The checked CC.3/CC.3a covariance and local multiplier bounds.

An independent check is still required that the enclosing bootstrap uses the admitted actual geometry and exact boundary data, that its real critical solution is the physical source solution in the chosen common chart, and that the final B activity argument, including old-field and current slots, remains in its required domain.

### 9. A blockwise normalized inverse gauge

This section supplies a concrete inverse-gauge bound for the associated symmetric averaging family. The source convention is essential: the designated endpoint transport in the old formula CMP99 (3.113) is replaced throughout by the same symmetric averaged transport \(T_U(y,x)\) used in CMP109 (0.11), (0.12) and its symmetric axial gauge. It is not asserted that every individual path holonomy is one in that gauge. The source transfer statement on pp.253–254 is used with this single consistent choice of averaging and reference operations.

The associated-family dictionary can be derived explicitly. For the actual raw average \(M\) in CMP109 (0.12), put
\[
 E_y(U';U)
  =\exp\!\left[L^{-d}\sum_{x\in B(y)}
       \log\bigl(T_{U'U}(y,x)T_U(y,x)^{-1}\bigr)\right].
\]
Use the relative endpoint correction of CMP99 (3.113), with every designated transport replaced by this same \(T\):
\[
 \mathcal U'_c
 =E_{c_-}^{-1}\,[M(U'U)]_c[M(U)]_c^{-1}
                \operatorname{Ad}_{[M(U)]_c}E_{c_+}.
\]
For a pure relative gauge, \(U'U=U^u\), transport covariance and the analytic logarithm identity give
\(E_y=u(y)(\mathfrak R_Uu)(y)^{-1}\). Substitution into the last display shows that \(\mathcal U'\) is the coarse pure relative gauge generated by \(\mathfrak R_Uu\) with reference \(M(U)\). Repeating the same correction on the active blocks therefore gives the iterated normalization in the source. This derives the nonlinear gauge operator attached to the actual raw average; it does not identify a raw derivative with an older regularized operator.

Write this associated one-step gauge average, as displayed in CMP99 (3.113), as
\[
 (\mathfrak R_Uu)(y)
 =u(y)\exp\!\left[
    L^{-d}\sum_{x\in B(y)}
       \log\bigl(u(y)^{-1}T_U(y,x)u(x)T_U(y,x)^{-1}\bigr)
            \right].
 \tag{RM.26}
\]
The source normalization is its iterated version at each actual determining root, denoted \(\overline{R_0u}^{\,s}(y)=1\) in CMP102 Proposition 2. The successive reference backgrounds are the corresponding raw averages of \(U_0\). This is the normalization to be used, not a separately invented average of the whole terminal block.

Fix one terminal block \(B^s(y)\). First work in a gauge in which the reference \(U_0\) satisfies the absolute hierarchical transport condition on this block. Every one-step designated transport on every active subblock is then one. For
\[
 L=e^{i\eta A}U_0
\]
put \(R_x=\mathcal T_L(y,x)\), the actual hierarchical transport from the terminal root. The source estimates (3.55)–(3.59) imply
\[
 \sup_{x\in B^s(y)}|R_x-1|\le C h_s K,\qquad
 |R_x-R_z|\le C h_r K
 \quad (x\in B^r(z)\subset B^s(y)),
 \quad K=\sup_{B^s(y)}|A|.
 \tag{RM.27}
\]
For the second bound, factor the displayed hierarchical chain at \(z\). The shorter relative transport differs from the corresponding reference transport, which is one, by \(Ch_rK\). The remaining factor has bounded norm. Thus this step uses associativity of the chain, not multiplicativity of the group mean.

In this reference gauge, (RM.26) becomes the anchored logarithmic mean
\[
 \mathfrak m(\{r_x\};r_z)
 =r_z\exp\!\left[L^{-d}\sum_{x\in B(z)}
                        \log(r_z^{-1}r_x)\right].
 \tag{RM.28}
\]
It is exactly left equivariant. On a fixed sufficiently small matrix ball about the identity its derivative, in the supremum norm of its \(L^d\) entries, has norm at most \(2\). Indeed its derivative at a constant identity tuple is the normalized arithmetic mean, of norm one; analyticity on the finite one-step product gives the fixed neighborhood with derivative norm at most two. The neighborhood depends on \(d,L,G\), not on the depth \(s\).

Let \(r^{(0)}(x)=R_x\), and obtain \(r^{(r)}\) by applying the actual mean (RM.28) at the successive levels. Define
\[
 E_r=\sup_z|r^{(r)}(z)-R_z|.
\]
The comparison with the tuple of original values at the previous-scale sites, followed by comparison with the constant tuple \(R_z\), gives
\[
 E_r\le 2E_{r-1}+C h_r K,\qquad E_0=0.
 \tag{RM.29}
\]
Since \(h_r=L^r\eta\) and \(L\ge3\),
\[
 E_r\le C K\sum_{\ell=1}^r2^{r-\ell}h_\ell
      \le \frac{C}{1-2/L}h_rK .
 \tag{RM.30}
\]
Choose the common smallness bound on \(h_sK\) after this fixed constant. Induction then keeps every tuple inside the neighborhood used above. In particular
\[
 F_s=r^{(s)}(y)=1+O(h_sK).
 \tag{RM.31}
\]

Set \(c_y=F_s^{-1}\) and
\[
 u(x)=c_y R_x\quad(x\in B^s(y)).
 \tag{RM.32}
\]
Exact left equivariance of (RM.28) at every stage gives
\[
 \overline{R_0u}^{\,s}(y)=c_yF_s=1.
\]
Also the hierarchical transport transforms as
\(\mathcal T_{L^u}(y,x)=u(y)\mathcal T_L(y,x)u(x)^{-1}=1\).
Therefore this gauge satisfies both the actual terminal normalization and the relative axial condition. Its bounds are
\[
 |u(x)-1|+|u(x)^{-1}-1|\le C h_sK.
 \tag{RM.33}
\]
The map is holomorphic on the fixed small domain: it is a finite composition of the admitted means and transports, followed by inversion, and the uniform estimates keep the composition in their domains.

For a reference not already in the displayed gauge, the covariant form is
\[
 u(x)=\mathcal T_{U_0}(y,x)^{-1}
           c_y\,\mathcal T_L(y,x).
 \tag{RM.34}
\]
Here is the full covariance check needed for this formula. If \(\widetilde U=U^g\) and \(\widetilde u(x)=g(x)u(x)g(x)^{-1}\), endpoint covariance of the same designated transport gives
\[
 \mathfrak R_{\widetilde U}\widetilde u(y)
   =g(y)(\mathfrak R_Uu)(y)g(y)^{-1}.
 \tag{RM.35}
\]
Indeed every matrix inside the logarithm in (RM.26) is conjugated by \(g(y)\); its exponential and the left root factor transform accordingly. Raw-averaging covariance gives this identity at every successive level. Therefore the terminal normalization is unchanged by a rooted frame change.

Set \(g_0(x)=\mathcal T_{U_0}(y,x)\) on each terminal block, so \(g_0(y)=1\). Apply this frame change to the normalization equations only. The reference is in the hierarchical transport slice, so each of its designated symmetric endpoint transports is one. The preceding mean proof gives \(\widetilde u=c_y\mathcal T_{L^{g_0}}\); pulling it back by (RM.35) gives exactly (RM.34). Thus the covariant iterates are controlled, rather than being replaced by unrelated means in different frames. No assertion that all individual path holonomies are one is used.

For a real reference \(g_0\) is unitary. For a complex reference near a fixed real \(U_*\), compare its transports with those of \(U_*\). The source estimate gives
\[
 \mathcal T_{U_0}(y,x)\mathcal T_{U_*}(y,x)^{-1}
       =1+O(h_s\|E\|),\qquad U_0=e^{i\eta E}U_*.
\]
Thus \(g_0,g_0^{-1}\) have bounded matrix norms, uniformly in the depth. Likewise the joint local analytic bound, with the fixed real reference, gives
\[
 \left|\mathcal T_L(z,x)\mathcal T_{U_0}(z,x)^{-1}-1\right|
       \le C h_r\|A\|
 \quad (x\in B^r(z)).
\]
One obtains this by differentiating the holomorphic transport map in its common absolute ball, or by applying its bound to the local BCH chart relative to \(U_*\). Its derivative has size \(Ch_r\) by the same local Cauchy estimate. These comparisons justify (RM.27) in the transformed frame with only fixed norm factors.

This algebraic canonicalization is not an application of a propagator theorem to the axially transformed background. That background may have fine-edge potential spikes. The stationary equation and every propagator remain in the original admitted smooth native chart. The frame change is used only to evaluate the normalization and to bound the auxiliary reconstructed curvature/current.

On a smaller fixed domain, local holomorphic differentiation of (RM.33) gives, for a fixed reference and a perturbation direction \(\dot A\),
\[
 \|u^{-1}\dot u\|_{\infty,B^s(y)}
      \le C h_s\|\dot A\|_{\infty,B^s(y)}.
 \tag{RM.36}
\]
For a varying reference the corresponding joint derivative estimate follows in the common two-input chart; a derivative of the reference is retained, rather than silently omitted. In the fixed-reference current family, (RM.36) is the normalized endpoint estimate needed at older fluctuation sites.

Apply the construction independently on the disjoint actual terminal blocks and set \(u=1\) on the fixed level-zero exterior. This defines one fine-lattice gauge. Each determining site has its own terminal normalization at its own level. No equality of independently prescribed coarse values at two levels is assumed.

#### Theorem RM.3 — bounded passage to the actual auxiliary raw-data representative

Use the actual symmetric raw average, its associated corrected map just derived, and the corresponding source relative axial condition. Let \(U_0\) be an admitted reference with prescribed data \(V=M_{\mathcal B}U_0\). Let \(L=e^{i\eta A}U_0\) be the actual relative Landau critical configuration on the zero corrected fiber, in the common ordinary radius of CMP102 Proposition 2, and suppose \(h_s\|A\|\) is uniformly small on all terminal blocks.

Then the gauge (RM.34), assembled as above, maps \(L\) to the relative axial critical configuration with the exact original raw data \(V\). The rooted gauge \(g_0(x)=\mathcal T_{U_0}(y,x)\) subsequently maps that configuration to the adopted absolute hierarchical axial representative:
\[
 W=(L^u)^{g_0}=L^{g_0u},\qquad
 M_{\mathcal B}W=V,\qquad \mathcal T_W(y,x)=1.
 \tag{RM.37}
\]
On a common admitted complex chart, the maps are holomorphic and
\[
 \|\operatorname{Ad}_{g_0u}\|+
 \|\operatorname{Ad}_{(g_0u)^{-1}}\|\le C.
 \tag{RM.38}
\]
Consequently all physical curvature and current profile bounds for \(L\) pass to \(W\) with a fixed factor. For a fixed real reference the parameter-dependent part of this converter also satisfies the local endpoint estimate (RM.36).

**Proof.** First take real inputs. The constructed \(u\) satisfies the actual normalized-average equations and the relative axial equations, exactly, on every terminal block. The uniqueness part of the source axial/Landau reduction identifies it with its normalized inverse gauge. CMP102 Proposition 2 then identifies \(L^u\) with the actual raw-data critical configuration for \(V\). This invocation includes the source's special crossing-bond correspondence: no rule replacing a crossing endpoint's actual normalization by a normalization at a different level is inserted.

Every endpoint of an actual mixed determining bond is a determining root at its own level. The nested-grid convention and the terminal partition used here are the ones verified in Annex AO. The gauge \(g_0\) is one at all of these roots, so raw gauge covariance preserves the entire determining datum. Relative axial means \(\mathcal T_{L^u}=\mathcal T_{U_0}\). Thus the final rooted transformation makes its transport one and proves (RM.37).

The real source solution, the weighted Landau solution after physical identification, the associated averaging maps and the displayed converter all lie on the same admitted finite-cutoff analytic chart. Their real identities continue by the holomorphic identity theorem. The bounds for \(g_0,g_0^{-1}\) follow by comparison with a fixed real reference, and (RM.33)–(RM.35) bound \(u,u^{-1}\). Their products give (RM.38). Physical curvature and Wilson current transform by conjugation, which proves the stated profile transfer. This transformation is used only to evaluate the auxiliary reconstructed output. It does not replace the actual primitive input or change any old integration variable. \(\square\)

The associated-family convention must remain fixed in all uses of this result. Using the literal old individual-path gauge-average formula while imposing only the new averaged-transport axial condition would invalidate the reduction to (RM.28); the old individual paths need not be one. The proof above instead derives the gauge average from the actual raw average and its same symmetric endpoint transports, using the explicit primary transfer statement in CMP109 pp.253–254. No numerical equality with an unrelated older operator is claimed.

The theorem remains conditional on actual common admission of the reference, the raw determining data and the physical critical branch. Those hypotheses are the source and native-ball checks in the enclosing projection theorem. It is a scoped intermediate step in that argument, not a completed catalogue estimate.
