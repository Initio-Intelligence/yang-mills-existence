# A localized value, gradient and current norm for transported marks

**Annex Y.** The conclusions below hold on the stated source domains. Applying them to the complete Wilson law requires compatibility of the conditional representation (CL), including the retained variables, densities, and marked transport. See [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Finite norm and uniform transport

This note completes the **finite specification** in M-03. It gives a concrete carrier norm for value, retained-coordinate difference and normalized-kernel current records; proves initial bounds for the scalar-repaired 21-field family used by F-01; and gives exact product, source-jet and conditional-expectation rules. The one-step operator costs are explicit integrals of the actual normalized kernels. They are not asserted to be bounded uniformly, or even finite in the strong current norm, on every selected history.

**M-06 remains open.** Its required all-order carrier-bound sum for the actual RG/R step has not been proved. The algebraic identities below are not its actual-model estimate. In particular, the new norm does not turn the existing bare \(a^{-4}\) budget into a current-scale \(h^{-4}\) budget.

This distinction is part of the result: M-03 asks for a finite norm construction and its initial bounds; it does not assert the boundedness of the actual RG/R operator in that norm. A discontinuous selected kernel can have an infinite current cost in the construction below. The norm detects that failure instead of assuming a smooth score that does not exist.

### 1. Coordinates, carriers and reference points

At a fixed cutoff and fixed stage, let \(h\) be the current physical block size and let \(\mathcal B_h\) be the finite periodic block graph. Use the augmented source-free state, including every retained continuous coordinate and every history variable needed by a later map. Inactive variables in a history sector are padded by fixed values. The resulting ambient space is a finite product
\[
 \mathsf X_h=\prod_{b\in\mathcal B_h}\mathsf X_{h,b}.
 \tag{M.1}
\]
Its probability law \(\mu_h\) is the actual normalized law, supported on its admissible subset. No independence of these blocks is assumed. A finite tuple of group, Lie-algebra and discrete coordinates may be assigned to a block. A coordinate whose definition uses several blocks is assigned its full dependency footprint, even if it is stored at one block. A carrier must contain that footprint. The storage block of a variable and its full dependency footprint are distinguished. A global history flag therefore has a global footprint unless an actual locality identity reduces it. Write \(\operatorname{cl}(Y)\) for the deterministic footprint closure of a block set: start with \(Y\), add the full footprints of all coordinates stored in its blocks, and repeat until stable. This finite construction may yield the full torus.

Fix the ambient reference configuration \(x_*\): identity group variables, zero Euclidean coordinates, and the first discrete value in the already specified enumeration of each history coordinate. A marked expression that has a natural global compact-link formula retains that formula, independently of any auxiliary history labels. This applies in particular to the microscopic F-01 fields, including after a positive history lift. Only a primitive expression that is defined solely in a restricted coordinate chart is extended by zero where its chart formula has no meaning. Fix these primitive versions once. A normalized conditional kernel on an inactive or zero-normalizer retained datum is extended by the point mass at its reference input; a coordinate map outside its admitted chart is extended by its old-state reference value. Every generated output is thereafter defined recursively by these chosen kernel and coordinate formulas on the whole ambient space. It is not independently re-zeroed on inactive sectors. This convention keeps the constant jet equal to one and makes the exact identities valid also at the reset reference points used below. These are conventions for a norm and a localization formula, not changes to the probability law on its support. An actual proof that uses a better extension must record that choice explicitly.

For a finite block set \(X\), let \(\mathsf t_h(X)\) be the number of edges in a shortest connected subgraph of the block graph containing \(X\). Set \(\mathsf t_h(\varnothing)=0\), and use
\[
 w_h(X)=\exp\{\kappa[|X|+\mathsf t_h(X)]\},\qquad \kappa>0.
 \tag{M.2}
\]
In every displayed carrier array the field-insertion anchors and all dependency footprints are contained in its carrier. A constant identity subtraction can be placed on its insertion anchor. Carrier size and distance are measured in current units \(h\), not in the original number of fine links.

The norm below is a norm of a **specified carrier representation**. Cancellation between two different activities is not used to reduce its size. This is the usual purpose of keeping the marked activities and generated responses as separate vertices.

### 2. Allowed differences and native regulators

For a group coordinate with source-free inverse-coupling label \(\beta_e\ge0\), choose a fixed Hilbert--Schmidt orthonormal basis of its Lie algebra and use the left-invariant perturbations
\[
 U_e\longmapsto \exp\left(\frac{tT}{\sqrt{1+\beta_e}}\right)U_e,
 \qquad |t|\le1.
 \tag{M.3}
\]
Each elementary perturbation acts only in its storage block. Its basis, scale label and \(\beta_e\) in (M.3) are fixed external labels of that padded coordinate, independent of the values of all other coordinates and history tags. If a chart uses moving conventions, their changes belong to the separate coordinate pullback, not to these elementary perturbations. This ensures the commuting reset identities in Section 7. For a Euclidean coordinate already in the source-free dimensionless free-field convention, use \(z_i\mapsto z_i+t e_j\). A different physical chart is first pulled back to that specified convention; its Jacobian or finite difference is not replaced by one. Discrete history changes are replacements of one coordinate by another value in its finite enumeration, with denominator one. Their whole dependency footprint is retained.

Write \(\tau\) for one such elementary perturbation. For a continuous perturbation with parameter \(t\ne0\), set
\[
 \delta_\tau A(x)=\frac{A(\tau x)-A(x)}t;
 \tag{M.4}
\]
for a discrete change omit the division by \(t\). The supremum over \(t\) below is a genuine supremum of finite differences; it is not an assumption of differentiability. Supremum envelopes can be interpreted by upper measurable envelopes if necessary. All input Wilson functions are continuous, so this qualification has no effect on their initial estimates.

Use a fixed native energy regulator
\[
 R_{h,X}(x)=1+
 \sum_{p:\,\operatorname{foot}(p)\subset X}\beta_p s(V_p(x))
 +\sum_{i:\,\operatorname{foot}(i)\subset X}|z_i(x)|^2,
 \qquad s(V)=N-\operatorname{Re}\operatorname{Tr}V.
 \tag{M.5}
\]
The plaquette and free-coordinate list is the actual retained/native list in the source-free representation, with its stated scale labels. It does not contain an unobservable eliminated microscopic energy. If no such coordinate is present, its sum is empty. At the microscopic input it is simply one plus the local Wilson plaquette energy. The list is finite at each cutoff; an extensive inherited list is not silently replaced by a bounded one.

Let \(\mathscr T_X\) contain the identity and all elementary perturbations whose footprints lie in \(X\). Define
\[
 A_X^\sharp(x)=\sup_{\tau\in\mathscr T_X}|A_X(\tau x)|,
 \qquad
 \widehat R_{h,X}(x)=R_{h,X}(x)+
 \sup_{\tau\in\mathscr T_X}R_{h,X}(\tau x).
 \tag{M.6}
\]
For a difference record \(B_{X,\tau}\), put
\[
 B_X^\natural(x)=
 \sum_{d:\,\operatorname{foot}(d)\subset X}
 \sup_{0<|t|\le1}|B_{X,d,t}(x)|,
 \tag{M.7}
\]
with the analogous finite sum over discrete replacements. Each Lie-algebra basis direction is counted separately. This keeps dependence on all retained directions, including directions on which a selected background depends.

### 3. The graded value/gradient/current norm

For \(d>0\), define the averaged moment norm
\[
 \mathfrak m_d(F;\mu)=
 \sup_{p\ge1}(dp)^{-d}\|F\|_{L^p(\mu)}.
 \tag{M.8}
\]
Degree zero uses the essential supremum. A source coefficient with \(m\ge1\) labels is assigned value grade \(m\) and difference/current grade \(m+\tfrac12\). The half grade permits the normalized-kernel gradient to carry a natural square-root energy factor; it is not an assertion that every actual kernel has that bound.

A decorated coefficient is a triple
\[
 \mathbf A_{I,X}=(A_{I,X},B_{I,X},J_{I,X}),\qquad |I|=m,
 \tag{M.9}
\]
with the exact compatibility identity for each tagged activity
\[
 \delta_\tau A_{I,X}=B_{I,X,\tau}+J_{I,X,\tau}.
 \tag{M.10}
\]
It follows that the summed coefficient has the same identity after summing its records. A coordinate difference can enlarge the declared carrier, in which case the whole compatible triple is assigned that enlarged carrier. Multiple activities with the same carrier retain distinct activity tags and are summed in the norm before cancellation. Thus \(X\) in a carrier sum can occur more than once with different tags. The compatible localization rule in Section 7 is chosen specifically to preserve (M.10); naive localization of all three components by the same reset operator would not do so. Here \(B\) records direct differences of the insertion and its explicit pullbacks; \(J\) records currents generated when a normalized conditional law, selector, reference law or support changes. They are retained separately even when their sum simplifies. Initially \(B=\delta A\) and \(J=0\).

For a fixed triple, put
\[
\begin{aligned}
 v_{h,m,X}(A)={}&h^{4m}\left[
   \mathfrak m_m(A_X^\sharp;\mu_h)
  +\frac1{m^m}\sup_x\frac{A_X^\sharp(x)}{
                          \widehat R_{h,X}(x)^m}\right],\\
 g_{h,m,X}(B)={}&h^{4m}\left[
   \mathfrak m_{m+1/2}(B_X^\natural;\mu_h)
  +\frac1{(m+1/2)^{m+1/2}}
       \sup_x\frac{B_X^\natural(x)}{
                      \widehat R_{h,X}(x)^{m+1/2}}\right],\\
 j_{h,m,X}(J)={}&h^{4m}\left[
   \mathfrak m_{m+1/2}(J_X^\natural;\mu_h)
  +\frac1{(m+1/2)^{m+1/2}}
       \sup_x\frac{J_X^\natural(x)}{
                      \widehat R_{h,X}(x)^{m+1/2}}\right].
 \end{aligned}
\tag{M.11}
\]
The supremum is over the specified ambient versions. Each term is a norm on the finite-valued records for which it is finite. On arbitrary measurable records it is an extended norm and may be infinite. Define the carrier norm, for a fixed label/anchor tuple, by
\[
 \boxed{
 \|\mathbf A_I\|_{h,\kappa}=
 \sum_{X\supset\operatorname{anchors}(I)}w_h(X)
   [v_{h,m,X}(A)+g_{h,m,X}(B)+j_{h,m,X}(J)].
 }
 \tag{M.12}
\]
For a uniformly anchored family take the supremum over its first anchor and translate the other fixed relative positions with it. A full exponential jet may retain a forest of disconnected carriers; the weight of such a forest is the product of the weights of its connected components. Joining components into one connected response requires an actual kernel localization estimate and pays the connector lengths in (M.2).

This is not a renamed bare \(L^p\) norm. It contains a native-scale polynomial regulator, all retained finite differences, separately measured kernel currents, actual history variables, and a spatial weight. The physical factor is \(h^{4m}\). Conditional contraction of a microscopic bound alone leaves the explicit loss \((h/a)^{4m}\) in this norm.

### 4. The microscopic input, including the F-01 coefficients

Use exactly the scalar-repaired clover matrix \(\widetilde q_a\) of F-01, in its orthonormal 21-component basis. Put
\[
 E_X=\beta_a\sum_{p\in\mathcal P(X)}s(U_p),
 \qquad
 O_{\alpha,a}=\beta_a\widetilde q_{\alpha,a}
              -\mathbb E[\beta_a\widetilde q_{\alpha,a}].
 \tag{M.13}
\]
Here \(\mathcal P(X)\) is a fixed enlarged plaquette stencil containing the clover support and every plaquette affected by the allowed perturbations of its links. Its size depends only on the fixed stencil and \(N\). The retained compact Wilson reserve gives
\[
 \|E_X\|_p\le C p,\qquad p\ge1,
 \tag{M.14}
\]
on its stated cofinal/AF-bounded geometry. At a single arbitrary finite cutoff the same statements are finite, with the compact bound replacing the uniform reserve constant if its hypotheses have not been checked.

#### Proposition M.1 -- an initial retained-link difference estimate

For the scalar-repaired 21 fields and the perturbations (M.3), uniformly in \(|t|\le1\),
\[
 |O_{\alpha,a}(\tau U)|
 \le C a^{-4}(1+E_X(U)),
 \tag{M.15}
\]
\[
 |\delta_\tau O_{\alpha,a}(U)|
 \le C a^{-4}[\sqrt{E_X(U)}+1],
 \tag{M.16}
\]
and hence
\[
 a^4\|O_{\alpha,a}^\sharp\|_p\le C(p+1),
 \qquad
 a^4\| (\delta O_{\alpha,a})^\natural\|_p
 \le C(\sqrt p+1).
 \tag{M.17}
\]
The initial current record is zero. Consequently the initial one-field carrier norm is bounded by a constant depending on \(N\), the fixed stencil and \(\kappa\), not on the cutoff or torus, under (M.14).

**Proof.** For a unitary plaquette,
\[
 \|U_p-I\|_{\rm HS}^2=2s(U_p).
 \tag{M.18}
\]
Changing one link by (M.3) changes any affected plaquette by a left or right multiplication, or a conjugate multiplication, with tangent norm at most \((1+\beta_a)^{-1/2}\). The first derivative of \(s(P_t)\) is bounded by
\(C(1+\beta_a)^{-1/2}\sqrt{s(P_t)}\); its second derivative is bounded by \(C(1+\beta_a)^{-1}\). Taylor's formula at zero therefore gives
\[
 \beta_a\left|\frac{s(P_t)-s(P_0)}t\right|
 \le C\sqrt{\beta_a s(P_0)}+C|t|,
 \tag{M.19}
\]
because \(\beta_a/(1+\beta_a)\le1\). It also gives
\(\beta_a s(P_t)\le C[\beta_a s(P_0)+t^2]\).

For a clover curvature, the unitary product rule gives
\(\|C_A(t)-C_A(0)\|_{\rm HS}\le C|t|/\sqrt{1+\beta_a}\).
The exact compact inequality used in the earlier field construction gives
\(\beta_a\|C_A(0)\|_{\rm HS}^2\le C E_X\).
Expanding the two factors of
\(\beta_a\operatorname{Tr}(C_A(t)C_B(t))\) yields the same right side as (M.19). The scalar repair is a fixed linear combination of these bilinears and the action density, so it obeys the same estimate. Its orthonormal off-diagonal factors \(\sqrt2\) change only the fixed constant. The centering term is independent of the link variables; its magnitude is bounded by (M.14).

There are only a fixed number of directions in the stencil. Taking their maximum or sum preserves the estimates with a fixed constant. Taking moments in (M.15)--(M.16), and using (M.14), proves (M.17). The regulator (M.5) and its shifted version dominate the pointwise right sides; the initial carrier has bounded diameter in units \(h=a\). This proves the norm bound. \(\square\)

Now use the **actual proposed F-01 prescription**, wherever its finite nondegeneracy test holds:
\[
 \Phi_a=Z_{a,T,\mu}\widetilde q_a-c_{a,T,\mu}e_S,
 \qquad Z=\sum_h z_hP_h.
 \tag{M.20}
\]
The seven \(z_h\) and the scalar \(c\) are the real finite coefficients specified there. The same norm statement also applies to the total finite-cutoff definition F.35, with its explicitly marked fallback on a zero normalization measurement. That fallback is not an inverse or a solution of the failed normalization equation. For \(\beta_a>0\), define the exposed coefficient budget
\[
 b_a=\frac{\|Z_{a,T,\mu}\|}{\beta_a}+a^4|c_{a,T,\mu}|.
 \tag{M.21}
\]
Then the same proof gives
\[
 \|\mathbf\Phi_{\alpha,a}\|_{a,\kappa}\le C b_a,
 \qquad
 a^4\|(\delta\Phi_{\alpha,a})^\natural\|_p
 \le C\frac{\|Z\|}{\beta_a}(\sqrt p+1).
 \tag{M.22}
\]
For the F-01 centering equation \(c=z_Sm_{a,T}\), the reserve also gives
\(a^4|c|\le C\|Z\|/\beta_a\). Thus (M.22) is finite for every nondegenerate finite normalization system, with its coefficient dependence shown. **No uniform or logarithmic bound on \(b_a\) is asserted.** That remains F-05. The construction does not define an inverse when the F-01 normalization determinant vanishes. The diagonal Wick phases of F.37 have modulus one, so the estimates also hold in that convention, with its transformed identity vector retained. If \(\beta_a=0\), the simple compact bound gives a finite input estimate proportional to \(\|Z\|+a^4|c|\); the asymptotically free application uses the positive-coupling formula (M.21).

### 5. Product and finite source-jet compatibility

#### Lemma M.2 -- graded Holder multiplication

For \(d,e>0\),
\[
 \mathfrak m_{d+e}(FG;\mu)
 \le \mathfrak m_d(F;\mu)\mathfrak m_e(G;\mu).
 \tag{M.23}
\]
**Proof.** Holder with exponents \((d+e)/d\) and \((d+e)/e\) gives
\[
 \|FG\|_p\le
 \|F\|_{p(d+e)/d}\|G\|_{p(d+e)/e}
 \le[(d+e)p]^{d+e}\mathfrak m_d(F)\mathfrak m_e(G).
\]
Divide and take the supremum. \(\square\)

For compatible records \(\delta A=B_A+J_A\) and \(\delta C=B_C+J_C\), the exact finite-difference product rule is
\[
\begin{aligned}
 B_{AC,\tau}&=B_{A,\tau}\,C\circ\tau+A\,B_{C,\tau},\\
 J_{AC,\tau}&=J_{A,\tau}\,C\circ\tau+A\,J_{C,\tau}.
 \end{aligned}
\tag{M.24}
\]
Their sum equals \(\delta_\tau(AC)\). The value envelopes multiply, and the difference/current envelopes are bounded by the corresponding two products of an envelope of grade \(r+1/2\) and one of grade \(s\), or vice versa. Lemma M.2 bounds their averaged parts. For the regulator parts use
\(\widehat R_X,\widehat R_Y\le\widehat R_{X\cup Y}\), and
\(d^d e^e\le(d+e)^{d+e}\). Thus the same source grades are preserved by multiplication, with the two displayed Leibniz terms retained.

If \(X\cap Y\ne\varnothing\), then
\[
 w_h(X\cup Y)\le w_h(X)w_h(Y).
 \tag{M.25}
\]
If they are disjoint, the same inequality has the additional explicit factor
\(\exp[\kappa\operatorname{dist}_h(X,Y)]\), obtained by joining shortest carrier trees by a shortest connecting path. One may instead keep the two carriers as a forest. These formulas expose the exact geometric cost of multiplying or joining vertices; they do not bound an actual sum over connecting kernels.

For the initial exponential jet
\[
 G_0(t)=\exp\left(\sum_i t_i\Phi_i\right)
 \tag{M.26}
\]
the coefficient with \(m\) distinct labels is \(\prod_i\Phi_i\). Lemma M.2 and (M.22), or direct Holder, give
\[
 \left\|\prod_{i=1}^m\Phi_i\right\|_p
 \le C^m b_a^m a^{-4m}(mp)^m
 \le (Ce)^m b_a^m a^{-4m}m!p^m.
 \tag{M.27}
\]
The direct-difference record is the sum of the \(m\) terms in (M.24); it has the corresponding fixed grade \(m+1/2\) and the same factorial type. Initially every current record is zero. These statements hold coefficientwise for every finite truncation, and truncating a higher-order jet gives exactly the lower-order jet. They do not assume convergence of an infinite exponential series.

The logarithm and exponential in the algebra of source jets are finite polynomial operations once a maximal source order is fixed. Consequently the decorated product rule preserves compatibility under both operations. The conditional cumulant partition formulas retained from the earlier passes then give the exact response coefficients. No finite bound on the number of one-field labels truncates the number or valence of the generated vertices.

### 6. Conditional expectation with the exact kernel current

Write one actual source-free integration, replacement or reset in common coordinates as
\[
 (QA)(y)=\int A(u,y)\,q_y(du),\qquad q_y(1)=1.
 \tag{M.28}
\]
All discrete labels and all constraints belong either to \(u\), to \(y\), or to the kernel. The common input space for \(u\) can be a disjoint union of padded sectors. Domains, coarea factors, selectors and all normalization constants are part of \(q_y\). A fixed coordinate pullback \(x=\chi(u,y)\) is performed before (M.28); it is an explicit substitution, whose finite differences are retained in the direct record. No derivative of a coordinate map is discarded. The norm of \(A\circ\chi\) is **not** automatically controlled by the previous elementary-coordinate norm. The additional data are the regulator pullback \(\widehat R_{h,X}(\chi(u,y))\), the dependency footprint of \(\chi\), and its normalized coordinate increments along \(y\mapsto\tau y\). One sufficient bound is obtained by joining \(\chi(u,y)\) to \(\chi(u,\tau y)\) through the explicit sequence of old coordinate changes: sum their normalized lengths times the old regulator to the difference grade along that sequence, and divide by the new step size. The old pointwise difference bound then controls the pullback by telescoping. If no such controlled path is available, its cost is recorded as infinite. The exact change of rank is treated by the padded sectors and discrete steps, not by an assumed common-rank differential. These path/regulator costs must be bounded in the actual matching theorem; (M.38) below does not pay them on its own.


For an explicit path version of this cost, choose a finite sequence
\(z^0=\chi(u,y),z^1,\ldots,z^J=\chi(u,\tau_t y)\)
of old elementary coordinate changes, with normalized step sizes
\(|s_j|\le1\); a discrete replacement has size one. With
\(d=m+\tfrac12\), define
\[
 \mathcal L^{(d)}_{\chi,X,\tau}(u,y)
 =\frac1{|t|}\sum_{j=1}^{J}|s_j|
       \widehat R_{h,X}(z^{j-1})^d.
 \tag{M.28a}
\]
If the new change is discrete, its denominator is one. A source-order-
\(m\) input activity whose total pointwise difference record has coefficient
\(c_X\) in (M.11) obeys, by telescoping,
\[
 \left|\frac{A(\chi(u,\tau_t y))-A(\chi(u,y))}{t}\right|
 \le c_X h^{-4m}d^d
        \mathcal L^{(d)}_{\chi,X,\tau}(u,y).
 \tag{M.28b}
\]
The two types of record remain separate under this pullback. If the
\(j\)-th old step is \(z^j=\tau_{d_j,s_j}z^{j-1}\), use
\[
 B^\chi_{\tau_t}(u,y)=\frac1t\sum_{j=1}^{J}s_j
        B_{d_j,s_j}(z^{j-1}),\qquad
 J^\chi_{\tau_t}(u,y)=\frac1t\sum_{j=1}^{J}s_j
        J_{d_j,s_j}(z^{j-1}).
 \tag{M.28c}
\]
For a discrete old step take \(s_j=1\); for a discrete new change omit
the overall division by \(t\). The sum is exactly
\(\delta_{\tau_t}(A\circ\chi)\) by telescoping, and (M.28a)
bounds both records with their respective input coefficients. No previous
kernel current is folded into a putative bare gradient.

The regulator pullback and (M.28a), including their actual carriers, are
explicit extra data to be bounded, not unit-cost coordinate changes.
If a continuous curve is used instead, the right side is the corresponding
weighted path-length integral, justified by finite-difference bounds along
its elementary subdivisions.

There is also an exact representation requiring no controlled chart path:
push \(q_y\) to the full old-coordinate state,
\(\widetilde q_y=\chi(\cdot,y)_*q_y\), and apply (M.29) to
\(\widetilde q_y\) with the old mark independent of \(y\).
All chart motion is then in the normalized-kernel current. Its total-
variation upper bound can be infinite even for a smooth deterministic
coordinate change, because distinct point masses are mutually singular.
That is a valid diagnostic representation, not a finite bound; a useful
application must supply the path/gradient control or another rigorous
estimate. Neither choice assumes a constant rank or a unit Jacobian.

For a continuous retained perturbation \(y_t=\tau_t y\), define the signed normalized-kernel current
\[
 \mathcal K_{y,\tau}=
 \frac{q_{y_t}-q_y}{t},\qquad \mathcal K_{y,\tau}(1)=0.
 \tag{M.29}
\]
For a discrete change use the difference without division. This signed measure always exists for fixed nonzero \(t\), even for hard selectors, changing supports or mutually singular conditional laws. Its total variation is at most \(2/|t|\); this elementary bound is not a useful uniform gradient estimate.

#### Theorem M.3 -- exact decorated conditional transport

Assume the displayed integrals are absolutely defined under both the unshifted and shifted kernels. This holds for the bounded marked coefficients at every fixed compact cutoff and fixed nonzero difference step. If \(\delta_\tau A=B_\tau+J_\tau\), set
\[
\begin{aligned}
 A'(y)&=Q_yA,\\
 B'_\tau(y)&=\int B_\tau(u,y)\,q_{y_t}(du),\\
 J'_\tau(y)&=\int J_\tau(u,y)\,q_{y_t}(du)
               +\int A(u,y)\,\mathcal K_{y,\tau}(du).
 \end{aligned}
\tag{M.30}
\]
Then
\[
 \delta_\tau A'=B'_\tau+J'_\tau.
 \tag{M.31}
\]
Furthermore the newly generated term can be written in the centered form
\[
 \int [A(u,y)-Q_yA]\,\mathcal K_{y,\tau}(du).
 \tag{M.32}
\]
The unshifted value obeys conditional-expectation contraction under the actual incoming and outgoing marginal laws. The shifted values, direct differences and currents obey (M.30), with their actual shifted kernels; contraction does not replace those kernels by \(q_y\).

**Proof.** Subtract \(Q_yA\) from \(Q_{y_t}A(\cdot,y_t)\), add and subtract \(Q_{y_t}A(\cdot,y)\), and divide by \(t\). This gives
\[
 \delta_\tau(QA)=Q_{y_t}(\delta_\tau A)+\mathcal K_{y,\tau}(A).
\]
Substitute the compatible record. Normalization gives (M.32). The proof for a discrete change is the same subtraction without division. Conditional Jensen proves the value contraction. \(\square\)

On a common smooth support, with a positive unnormalized density \(w(u,y)\), the limit of (M.29), when justified in the required norm, is
\[
 Dq_y=q_y\,[D\log w-Q_yD\log w],
\]
so the new current reduces to
\[
 \operatorname{Cov}_{q_y}(A,D\log w).
 \tag{M.33}
\]
The finite-difference theorem is stronger in scope: it does not infer this smooth formula at a moving selector boundary. Boundary flux and changes in the conditional normalizer are already present in (M.29).

For the frozen positive R quotient, the conditional mark is
\[
 (Q_RF)(u',v)=
 \frac{\int\rho(u,v)F(u,v)\,du}{\int\rho(u,v)\,du}.
 \tag{M.34}
\]
The normalized replacement factor cancels. Thus the mark is independent of the freshly sampled \(u'\), and its finite difference in that variable is exactly zero. Its retained-\(v\) current remains (M.29). This cancellation does not set the retained current or the higher source responses to zero.

### 7. Explicit carrier costs for the actual kernel

There is a finite, fully specified carrier decomposition even when locality is poor. For a function of retained blocks, let
\[
 (E_b f)(y)=f(y\text{ with block }b\text{ reset to }y_{*,b}),
\]
and set
\[
 L_Y=\prod_{b\in Y}(I-E_b)\prod_{b\notin Y}E_b.
 \tag{M.35}
\]
The operators commute, and
\[
 f=\sum_{Y\subset\mathcal B_{h'}}L_Yf.
 \tag{M.36}
\]
For a total compatible output record \((A',B',J')\), localize its value by \(A^{[Y]}=L_YA'\). **The operator \(L_Y\) need not commute with \(\delta_\tau\).** The precise compatible rule uses the storage block \(b\) of the varied ambient coordinate. If \(b\notin Y\), set both localized difference and current records to zero. If \(b\in Y\), define
\[
 L^{(b)}_{Y\setminus\{b\}}
 =\prod_{c\in Y\setminus\{b\}}(I-E_c)
   \prod_{c\notin Y}E_c,
 \tag{M.36a}
\]
which leaves block \(b\) free, and put
\[
 B^{[Y]}_{b,t}=L^{(b)}_{Y\setminus\{b\}}B'_{b,t},
 \qquad
 J^{[Y]}_{b,t}=L^{(b)}_{Y\setminus\{b\}}J'_{b,t}.
 \tag{M.36b}
\]
Then, exactly,
\[
 \delta_{b,t}L_YA'=
 \begin{cases}
  0,&b\notin Y,\\
  L^{(b)}_{Y\setminus\{b\}}\delta_{b,t}A',&b\in Y,
 \end{cases}
 \tag{M.36c}
\]
so \(\delta_{b,t}A^{[Y]}=B^{[Y]}_{b,t}+J^{[Y]}_{b,t}\). To prove (M.36c), observe that a finite difference in block \(b\) annihilates \(E_bf\) and commutes with every \(E_c\), \(c\ne b\). In particular \(L^{(b)}_{Y\setminus\{b\}}=L_Y+L_{Y\setminus\{b\}}\); this formula accounts for the localization commutator without losing its contribution. It holds for continuous and discrete coordinate perturbations alike.

The value index \(Y\) need not contain the insertion anchors. Declare the actual carrier to be
\[
 \overline Y_I=\operatorname{cl}(Y\cup\operatorname{anchors}(I)).
 \tag{M.36d}
\]
It contains the full footprint of each varied coordinate stored in \(Y\), as well as every insertion anchor. Regroup the compatible triples on these declared carriers, retaining distinct activity tags before taking absolute norms. Use \(w_{h'}(\overline Y_I)\), not \(w_{h'}(Y)\), in (M.12). This deterministic enlargement is part of the cost. It is used for this output localization and can be overinclusive or global. It is not imposed on an already localized microscopic activity independent of other, globally supported flags that happen to be stored at the same block. In particular, the empty index \(Y=\varnothing\) is retained and assigned to \(\operatorname{cl}(\operatorname{anchors}(I))\); constant components are not lost from the anchored norm.

If \(QA_X\) is independent of a block, all its value coefficients containing that block vanish by (M.35). If the actual conditional law has global dependence, the formula produces global carriers instead of claiming local ones.

For clarity, the cost is given by actual signed kernels, not an unnamed operator constant. Write \(y^Z\) for the configuration with the blocks in \(Z\) retained and all others reset to the reference point. On the common \((u,v)\) input chart define
\[
 K^V_{Y\leftarrow X}(y;du,dv)=
 \sum_{Z\subset Y}(-1)^{|Y|-|Z|}
 q_{y^Z}(du)\,\delta_{y^Z}(dv),
 \tag{M.37}
\]
restricted to the actual coordinates needed by the pulled-back input carrier. For a difference/current direction stored in block \(b\), both record kernels are zero when \(b\notin Y\). When \(b\in Y\), the compatible direct kernel is
\[
 K^B_{Y\leftarrow X,b,t}(y;du,dv)=
 \sum_{Z\subset Y\setminus\{b\}}(-1)^{|Y|-1-|Z|}
 q_{\tau_{b,t} y^{Z\cup\{b\}}}(du)
 \,\delta_{y^{Z\cup\{b\}}}(dv),
 \tag{M.38}
\]
and the new kernel-current part is
\[
 K^J_{Y\leftarrow X,b,t}(y;du,dv)=
 \sum_{Z\subset Y\setminus\{b\}}(-1)^{|Y|-1-|Z|}
 \mathcal K_{y^{Z\cup\{b\}},b,t}(du)
 \,\delta_{y^{Z\cup\{b\}}}(dv).
 \tag{M.39}
\]
These are the inclusion-exclusion formulas for (M.36b); retaining block \(b\) in \(Z\cup\{b\}\) is essential. Their declared carriers are enlarged by (M.36d).
Thus, if an input value coefficient obeys
\(|A_X|\le a_X h^{-4m}m^m\widehat R_{h,X}^{m}\), its output value is bounded by
\[
 |L_YQA_X|
 \le a_X h^{-4m}m^m
       \int\widehat R_{h,X}^{m}\,|K^V_{Y\leftarrow X}|.
 \tag{M.40}
\]
The direct record is bounded using
\(\int\widehat R_{h,X}^{m+1/2}|K^B_{Y\leftarrow X,\tau}|\).
The current record has both this term applied to the previous current and
\(\int\widehat R_{h,X}^{m}|K^J_{Y\leftarrow X,\tau}|\)
applied to the previous value. The changed inclusion-exclusion operator in (M.38)--(M.39) already accounts for the noncommuting localization reset. Multiplication by the precise output weights in (M.11)--(M.12), taking the displayed supremum envelopes and the actual \(\mu_{h'}\) moment norms, gives a nonnegative matrix of transport costs depending only on the **actual source-free kernels, charts, regulator and geometry**. Every factor \((h'/h)^{4m}\) is retained.

These formulas can be evaluated before choosing a marked input. No spatial bound on their sum has been inserted. In particular, the current entries can be infinite after the supremum over \(t\to0\). Proving useful bounds on these data is precisely the content of M-04--M-07, C-02--C-08 and H-02--H-05. An effective locality proof may replace the reference-point expansion by a sharper explicit carrier expansion, but must control the same exact output.

### 8. A nonvacuity and failure test

The norm is nonvacuous on the actual microscopic field family by Proposition M.1 and (M.22). It also detects a failure that the bare moment norm misses.

Let \(y\) be uniform on \((-1,1)\) and let the conditional variable \(u\in\{-1,1\}\) have law
\[
 q_y=\begin{cases}\delta_{-1},&y<0,\\ \delta_{1},&y\ge0.\end{cases}
\]
The input mark \(A(u,y)=u\) is bounded, independent of \(y\), and has zero direct difference and zero initial current. But
\[
 QA(y)=\operatorname{sgn}(y),
\]
and for \(t>0\), on \(-t<y<0\),
\[
 \mathcal K_{y,t}(A)=2/t.
 \tag{M.41}
\]
For any fixed \(p>1\), its \(L^p\) norm grows like \(t^{-1+1/p}\), and its pointwise norm grows like \(t^{-1}\). The strong current norm is infinite. Formula (M.30) is still exact. This is why a hard-selector current cannot be replaced by a formal smooth log score without a support theorem.

The example is not asserted to model a Yang--Mills selector. It proves that the finite construction does not smuggle in a false universal contraction statement.

### 9. Exact residual obligation for M-06

For every finite source order, exact transport remains
\[
 G'=QG,\qquad \Psi'=\log(Qe^\Psi),
\]
and hence, writing \(A_I=\partial_I\Psi(0)\),
\[
 A_I'=\sum_{\pi\in\Pi(I)}
  \kappa_Q(A_B:B\in\pi).
 \tag{M.42}
\]
The existing moment estimate gives magnitudes of conditional cumulants after outer averaging, and Sections 5--7 give exact carrier/current bookkeeping. These facts alone do **not** establish the M-06 hypotheses.

The missing statement is an all-order estimate of the actual carrier-cost sums arising from (M.37)--(M.42), with constants independent of current scale, UV depth, volume and admitted history, after the stated current-field matching and local subtractions. It must include:

- every higher vertex already present in the incoming jet;
- the conditional cumulants joining input carriers;
- all selector, coordinate, coarea and normalized-reference currents;
- the reset responses and their possibly global conditional dependence;
- the physical current-scale budget and a fixed factorial exponent in \(m\).

Neither the initial bound (M.27), a formal partition count, nor an infinite diagnostic current cost is that estimate. The statement therefore remains **open**.

### 10. Application conditions

| Requirement | Result in this annex |
|---|---|
| Explicit current-scale value norm | (M.5), (M.8), (M.11); scale factor \(h^{4m}\), native regulator and actual full-law moments. |
| Retained-variable gradients | Exact dimensionless finite differences (M.3)--(M.7), including discrete history variations. |
| Currents and hard support changes | Normalized signed kernel differences (M.29)--(M.32); no common-support score assumption. |
| Initial finite-cutoff fields | Proposition M.1 for all 21 scalar-repaired fields; F-01 coefficients exposed in (M.20)--(M.22). |
| Carrier geometry | Dependency footprints, current block tree weight, forest convention and exact localization (M.35)--(M.39). |
| Conditional-expectation compatibility | Exact transport (M.30); actual kernel/regulator integrals (M.40) and their direct/current analogues. |
| Full finite-jet algebra | Graded Holder/product rules (M.23)--(M.27), exact finite cumulant rule (M.42), compatibility under truncation. |
| Actual bounded transport in this norm | **Not proved; not part of the finite M-03 statement.** |
| M-06 uniform actual carrier-bound sum | **Not proved; statement remains open.** |

The only imported estimates in the initial bound are the compact Wilson energy reserve of Annex A and the already specified scalar-repaired clover inequalities. All other identities and norm estimates in this note are proved directly. No new primary-source theorem about marked Balaban histories is claimed.


---
