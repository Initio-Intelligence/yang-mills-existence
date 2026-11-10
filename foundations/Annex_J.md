# The even native expansion and its fourth-order remainder

**Annex J.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Result and scope

This note strengthens the native Gaussian comparison in one precise case. At the identity retained background, freeze the inherited regular action at its actual shell value, and use the same symmetric product cutoff throughout a signed computational coupling interpolation. Then every integrated native cumulant is even in that interpolation parameter. Its second coefficient has an explicit constrained truncated-Gaussian formula, and the remainder after that coefficient is \(O(g^4)\), uniformly in volume, cutoff size, and source order with the same factorial exponent two.

The theorem is P using the fixed-domain regular inputs already specified in Annex F. It does not differentiate the inherited action along the RG trajectory, remove the Gaussian cutoff, cover a nonzero retained background, or identify native fields with \(Q_{0:k}F_0\). The complete-history M0/C0/H0 obligations remain open.

The improvement is an actual second-order expansion of the nonlinear conditional integral, including its exact classical action, inherited E, nonlinear constraint chart, and new coarea. It does not come from replacing the full integral by its quadratic approximation.

### 1. Freeze the shell before varying the computational parameter

Fix one admitted homogeneous, no-R regular integral, with the retained background equal to the identity. All old couplings, the physical nonlinear chart, the minimizing map, and the inherited regular action \(E_*\) are frozen at their actual values in that shell. Let \(\mathcal I\) be its finite four-dimensional current coordinate lattice. Its metric satisfies

\[
\sup_x\sum_{y\in\mathcal I}e^{-a d(x,y)}
\le C(1+a^{-4}),\qquad 0<a\le1,
\tag{1.1}
\]

uniformly over the admitted tori. Coordinate-block dimension is fixed.

Write \(U(q)\) for the exact physical chart, including the constraint correction and minimizing-field pullback, with \(U(0)=1\). Write

\[
\mathcal A(q)=A^\eta(U(q))+G(q),\qquad
\mathcal A(0)=D\mathcal A(0)=0,\qquad
H=D^2\mathcal A(0)>0.
\tag{1.2}
\]

Here \(G=0\) in the hard-gauge version; the specified analytic soft-gauge term of the previous proof may instead be included. The true constrained precision \(H\), including the constraint contribution, has the uniform gap and weighted decay retained in the earlier covariance theorem.

Let \(\mathcal E(q)=E_*(U(q))\), and let \(J(q)\) be the new exact coarea factor. Older measure terms occur in \(\mathcal E\), so they are not included a second time in \(J\). Define

\[
\mathcal K(q)=\mathcal E(q)-\mathcal E(0)
+\log J(q)-\log J(0).
\tag{1.3}
\]

The logarithm is the real branch at the positive local density, continued on the admitted complex chart. Its nonvanishing follows from the Haar chart and the same small Neumann determinant used in the coarea proof.

Choose a common symmetric convex product

\[
\mathcal D_P=\prod_{i\in\mathcal I}\{z_i:|z_i|\le P\}.
\tag{1.4}
\]

The signed parameter \(g\) varies over \([-g_*,g_*]\), where \(g_*\) is the actual positive shell coupling, \(g_*\) is below a fixed small ceiling, and \(g_*P\le\delta\). The value of \(P\) is fixed during this interpolation. Set

\[
W_g(z)=
-\left[g^{-2}\mathcal A(gz)-\tfrac12 zHz\right]
+\mathcal K(gz),
\tag{1.5}
\]

\[
d\nu_g(z)=
Z_g^{-1}\mathbf1_{\mathcal D_P}(z)
\exp\{-\tfrac12zHz+W_g(z)\}\,dz.
\tag{1.6}
\]

The removable value at \(g=0\) is \(W_0=0\). Thus \(\nu_0\) is exactly the constrained Gaussian restricted to this same product cutoff. Overall coordinate Jacobian powers of \(|g|\) cancel from normalized expectations and are not part of \(W_g\).

For each native curvature-bilinear stencil or scalar Wilson-action stencil at \(x\), let \(\mathcal P_{\alpha,x}(q)\) be its physical numerator. At the identity,

\[
\mathcal P_{\alpha,x}(0)=D\mathcal P_{\alpha,x}(0)=0.
\]

Its normalized native field at physical scale \(h\) is

\[
O_{\alpha,x}(g,z)
=h^{-4}g^{-2}\mathcal P_{\alpha,x}(gz).
\tag{1.7}
\]

Again, its value at zero is defined by the removable Taylor continuation. Every finite component in the specified native family is included.

This is a computational interpolation of one frozen shell. In particular,
\(\partial_g\mathcal E(gz)=D\mathcal E(gz)[z]\), without a term
\(\partial_g E_*\). The latter would belong to a different, presently unproved coupling-flow derivative theorem.

### 2. The physical derivative bounds needed through order six

The following finite-order extension of the previous physical-chart estimates is useful because it preserves the polynomial degree of each coupling derivative.

#### Lemma 2.1 — fixed-order physical locality, P with the earlier scoped inputs

On a fixed smaller physical complex neighborhood, there are \(C_n,c_n>0\), for \(1\le n\le6\), such that the native numerators obey

\[
\left|
\partial_{i_1}\cdots\partial_{i_n}
\mathcal P_{\alpha,x}(q)
\right|
\le C_n e^{-c_n\tau(x,i_1,\ldots,i_n)}.
\tag{2.1}
\]

For the extensive functions \(\mathcal A,\mathcal K\), their differentiated tensors, with at least one fixed coordinate index, obey the corresponding volume-independent tree majorants

\[
\left|
\partial_{i_1}\cdots\partial_{i_n}\mathcal F(q)
\right|
\le C_n e^{-c_n\tau(i_1,\ldots,i_n)},
\qquad \mathcal F=\mathcal A,\mathcal K.
\tag{2.2}
\]

At order one, the right side means a uniform bound for each fixed derivative. Constants may depend on the fixed group, block size, physical analytic radius and regular-action parameters. They do not depend on \(P\), volume, fine spacing \(\eta\), or shell depth within the fixed-domain scope.

**Proof.** The native exact chart has an analytic first derivative with exponential localization on a fixed physical complex neighborhood. Coordinate Cauchy estimates for the other \(n-1\) derivatives preserve the exponential involving any selected one of the input indices. Symmetry of mixed derivatives permits taking the minimum of these bounds. Since

\[
\tau(x,i_1,\ldots,i_n)
\le\sum_a d(x,i_a)
\le n\max_a d(x,i_a),
\]

one obtains tree decay with a fixed loss in exponent. The same argument applies after composing the finite plaquette and transport stencil. Only the finite orders through six are used here.

For the complete classical action, use precisely the curvature normalization retained in the proof:

\[
\mathcal A(q)=
\sum_p\eta^4\mathcal L_\eta(\mathfrak F_p(q))+G(q),
\qquad
\mathfrak F_p(q)=\frac{\log U(q)_p}{i\eta^2}.
\tag{2.3}
\]

The homogeneous specialization of CMP102 Proposition 9 and (190) supplies the physical first-variation and spatial-gradient bounds. They give exponential localization for \(D\mathfrak F_p\), with no inverse power of \(\eta\). Repeated coordinate Cauchy, as above, extends the already proved orders one through three to the finite orders through six.

Every derivative through order six of
\[
\mathcal L_\eta(F)=
\eta^{-4}\left[
1-\frac1{2N}\operatorname{Tr}
(e^{i\eta^2F}+e^{-i\eta^2F})
\right]
\]
is uniformly bounded on the smaller physical curvature ball. This follows either from its convergent even power series or from its analytic bound on a slightly larger fixed ball. The full chain rule retains the factor \(\eta^4\) in every term. After fixing one current coordinate, the fine-plaquette sum satisfies
\(\sum_p\eta^4e^{-c d(x_p,i_1)}\le C\).
The remaining current-coordinate sums are exponential. This proves (2.2) for \(\mathcal A\), retaining all nonlinear chain-rule terms. The specified block-local analytic \(G\) has the same finite-order bounds.

For \(\mathcal E\), apply coordinate Cauchy to the fixed-domain CMP116 regular activity bound used. Differentiation adds at most a fixed power of the activity-carrier size. Its exponential carrier entropy reserve absorbs each such power through order six. The inherited old-scale sum is the one already performed in that regular bound.

For \(\log J\), the differentiated Haar terms are local analytic terms. The constraint determinant has its convergent trace/Neumann expansion. Each first derivative anchors the trace; each second derivative has the weighted decay already proved. These estimates hold on a smaller complex neighborhood. Applying Cauchy to a second derivative preserves decay between any selected pair of indices. Taking the largest pair distance gives tree decay, since the tree on \(n\) points has length at most \((n-1)\) times their diameter. This proves the remaining finite-order bounds without a volume factor. \(\square\)

The restriction to the fixed homogeneous analytic domain is essential. This lemma does not assert the missing complex tube for arbitrary CMP119 histories.

### 3. Coupling derivatives are controlled polynomial marks

Write

\[
O_i^{(a)}(g,z)=\partial_g^a O_i(g,z),
\qquad
W_r(g,z)=\partial_g^rW_g(z).
\tag{3.1}
\]

For \(0\le a\le4\), Taylor's integral identity gives

\[
O_i^{(a)}(g,z)
=h^{-4}\int_0^1(1-t)t^a
D^{a+2}\mathcal P_i(tgz)[z^{a+2}]\,dt,
\tag{3.2}
\]

and the particularly useful first-gradient identity is

\[
D_{z_y}O_i^{(a)}(g,z)
=h^{-4}\int_0^1t^a
D^{a+2}\mathcal P_i(tgz)[e_y,z^{a+1}]\,dt.
\tag{3.3}
\]

To obtain (3.3), first write
\(D_{z_y}(g^{-2}\mathcal P_i(gz))
=g^{-1}D_y\mathcal P_i(gz)\), use \(D\mathcal P_i(0)=0\), and only then differentiate in \(g\). This avoids an unnecessary apparent extra polynomial degree.

Likewise, for \(1\le r\le4\),

\[
D_{z_y}\partial_g^r[g^{-2}\mathcal A(gz)]
=\int_0^1t^r
D^{r+2}\mathcal A(tgz)[e_y,z^{r+1}]\,dt.
\tag{3.4}
\]

For the second coordinate derivative there is a simpler exact identity:
\[
D_{z_i}D_{z_y}\partial_g^r[g^{-2}\mathcal A(gz)]
=D^{r+2}\mathcal A(gz)[e_i,e_y,z^r].
\tag{3.4a}
\]
Indeed, taking the two coordinate derivatives first cancels \(g^{-2}\), leaving \(D^2\mathcal A(gz)[e_i,e_y]\); then differentiate \(r\) times in \(g\). This gives a degree-\(r\) majorant directly and needs no seventh physical derivative. The identities extend to \(g=0\) by their removable continuations.

For the analytic remainder,
\[
\partial_g^r\mathcal K(gz)=D^r\mathcal K(gz)[z^r].
\]
Its first two coordinate derivatives have lower polynomial degree than the bounds just described; factors \(gz_j\) are treated in the same way.

Choose one sufficiently small decay rate \(\gamma>0\) below all the finite-order rates in Lemma 2.1 and the covariance rate. Put
\[
Z_x(z)=\sum_j e^{-2\gamma d(x,j)}|z_j|.
\]

The mean and concentration proof applies uniformly to all signed \(g\) in the present interval: the classical Hessian perturbation is \(O(|g|P)\), the E/coarea perturbation is \(O(g^2)\), and the linear-to-full-density interpolation has the same gap. Its first-gradient argument uses \(|g|\) and yields

\[
\sup_{g,i}\|\;z_i\;\|_{L^p(\nu_g)}
\le C\sqrt p,\qquad p\ge1.
\tag{3.5}
\]

Consequently (3.2)--(3.3), Lemma 2.1 and Hölder/Minkowski give

\[
\boxed{
\|O_i^{(a)}\|_p
\le C_a h^{-4}p^{1+a/2},\qquad
\left\|\|\nabla O_i^{(a)}\|_{\gamma,x_i}\right\|_p
\le C_a h^{-4}p^{(1+a)/2}.
}
\tag{3.6}
\]

The weighted gradient norm is the one used in the real cut theorem. Centering the first quantity costs at most a factor two.

#### 3.1 Exact anchored decomposition of every \(W_r\)

Since \(W_r(g,0)=0\), define

\[
R_{r,y}(g,z)
=\int_0^1\langle z_y,D_yW_r(g,sz)\rangle\,ds.
\tag{3.7}
\]

The radial fundamental theorem of calculus gives the exact identity

\[
W_r(g,z)=\sum_{y\in\mathcal I}R_{r,y}(g,z).
\tag{3.8}
\]

The degree bounds following (3.4), and exponential summation of their fixed-order tensors, imply

\[
|R_{r,y}(g,z)|
\le C_r[1+Z_y(z)]^{r+2},
\]
\[
\|\nabla R_{r,y}(g,z)\|_{\gamma,y}
\le C_r[1+Z_y(z)]^{r+1}.
\tag{3.9}
\]

For the gradient, differentiate (3.7). The two terms are \(D_yW_r\) and \(z_yD_iD_yW_r\); their degrees are at most \(r+1\). The unused exponential decay pays the gradient weight. The estimates for \(\mathcal K\) are of lower degree and fit (3.9).

Thus

\[
\boxed{
\|R_{r,y}-\mathbb E_{\nu_g}R_{r,y}\|_p
\le C_rp^{1+r/2},\qquad
\left\|\|\nabla R_{r,y}\|_{\gamma,y}\right\|_p
\le C_rp^{(1+r)/2}.
}
\tag{3.10}
\]

All these estimates are uniform in \(P\), volume, and the computational parameter. They concern the actual nonlinear functions, not just their Taylor polynomials at zero.

### 4. Four parameter derivatives retain factorial exponent two

Let

\[
K_m(g)=\kappa_{\nu_g}
\bigl(O_1(g),\ldots,O_m(g)\bigr),
\qquad m\ge1,
\tag{4.1}
\]

with anchors \(x_1,\ldots,x_m\). For \(m=1\), the cumulant means expectation and \(\tau(x_1)=0\).

#### Proposition 4.1 — localized derivative bound, P

For \(0\le k\le4\),

\[
\boxed{
|K_m^{(k)}(g)|
\le C^{m+1}(m!)^2 h^{-4m}
\exp\!\left[
-\frac{\gamma\,\tau(x_1,\ldots,x_m)}{4(m+4)}
\right].
}
\tag{4.2}
\]

The constant can be chosen simultaneously for those five derivative orders, for all source orders \(m\), and for all admitted finite volumes and common cutoffs.

**Proof.** At finite volume the domain is fixed and bounded. The removable continuations are smooth, and ordinary differentiation of finite moments is legitimate. If \(\mathbf a=(a_1,\ldots,a_m)\) and \(b_r\) is the multiplicity of the inserted response \(W_r\), the exact formula is

\[
\begin{aligned}
K_m^{(k)}(g)
={}&
\sum_{\substack{a_i,b_r\ge0\\
\sum_i a_i+\sum_{r=1}^k r b_r=k}}
\frac{k!}{\prod_i a_i!\prod_{r=1}^k b_r!(r!)^{b_r}}
\\
&\quad\cdot
\kappa_{\nu_g}\!
\left(
O_1^{(a_1)},\ldots,O_m^{(a_m)},
W_1^{[b_1]},\ldots,W_k^{[b_k]}
\right).
\end{aligned}
\tag{4.3}
\]

The notation \([b]\) means \(b\) repeated cumulant arguments, not a product inserted as one argument. Formula (4.3) follows by expanding, at the current \(g\),

\[
\log\mathbb E_{\nu_g}
\exp\!\left[
W_{g+v}-W_g+\sum_i t_iO_i(g+v)
\right]
\]

and extracting the coefficient \(v^k\prod_i t_i\). The normalization term with no \(t_i\) has no effect for \(m\ge1\).

Let \(n=\sum_r b_r\le k\), \(N=m+n\), and replace every \(W_r\) by (3.8). At fixed inserted anchors \(y_1,\ldots,y_n\), there are \(N\) polynomial-growth cumulant arguments. Their total growth degree is

\[
\sum_i(2+a_i)+\sum_r b_r(2+r)=2N+k.
\tag{4.4}
\]

Apply the real cut theorem at moment order \(2N\). Its two gradient factors reduce the total power of \(N\) by one. The product of the value/gradient budgets is therefore at most

\[
C^{N+1}h^{-4m}N^{N+k/2-1}.
\tag{4.5}
\]

The cut partition coefficient is at most
\((N-1)!2^{N-2}\), and there are at most \(N^2\) crossing pairs. Since \(N^N\le e^N N!\), \(k\le4\), and \(N\le m+4\), these factors are bounded by
\[
C^{m+1}(m!)^2h^{-4m}
\]
times a fixed polynomial in \(m+4\). Such a polynomial is absorbed by increasing the fixed exponential constant \(C^{m+1}\).

Delete a longest edge of a minimum spanning tree on all \(N\) anchors. The cut theorem supplies the spatial factor
\[
\exp[-\gamma\tau(x_1,\ldots,x_m,y_1,\ldots,y_n)/(N-1)].
\tag{4.6}
\]

When \(n\ge1\), write the enlarged tree length as \(T\). Doubling and shortcutting its walk through the external anchors shows
\[
T\ge\tfrac12\tau(x_1,\ldots,x_m).
\]
Its paths also give \(T\ge d(y_l,x_1)\) for each \(l\), hence
\[
T\ge\frac1n\sum_{l=1}^n d(y_l,x_1).
\]
Splitting (4.6) between these two bounds gives
\[
e^{-\gamma T/(N-1)}
\le
e^{-\gamma\tau(x_1,\ldots,x_m)/(4(N-1))}
\prod_{l=1}^n
e^{-\gamma d(y_l,x_1)/(2n(N-1))}.
\tag{4.7}
\]

By (1.1), summing the inserted anchors costs at most
\[
C_n[1+N^{4n}],\qquad n\le4,
\tag{4.8}
\]
another fixed polynomial. For \(n=0\), no anchor sum is needed. The case \(N=1\) is the direct first-moment bound (3.6). Finally, the number and coefficients of terms in (4.3), for \(k\le4\), are bounded by a fixed polynomial in \(m+4\). Combining these bounds proves (4.2), with its slightly weakened common range. \(\square\)

This proof does not apply a general degree-six cumulant estimate to every mark. Only at most four coupling derivatives occur. The total degree increment is \(k\), so its cost is polynomial in the source order, preserving the exponent \((m!)^2\).

### 5. Exact parity and the Gaussian second coefficient

#### Theorem 5.1 — even native expansion, P

In the stated fixed zero-background regular law,

\[
K_m(-g)=K_m(g)
\tag{5.1}
\]

for every source order and field-label tuple. Moreover,

\[
\boxed{
K_m(g)=K_m(0)+\frac{g^2}{2}\,\mathcal C_{2,m}
+\mathcal R_{4,m}(g),
}
\tag{5.2}
\]

where \(\mathcal C_{2,m}=K_m''(0)\) and

\[
\boxed{
|\mathcal R_{4,m}(g)|
\le |g|^4 C^{m+1}(m!)^2 h^{-4m}
\exp\!\left[
-\frac{\gamma\,\tau(x_1,\ldots,x_m)}{4(m+4)}
\right].
}
\tag{5.3}
\]

The coefficient \(\mathcal C_{2,m}\) obeys the same bound without the factor \(|g|^4\).

**Proof.** Under \((g,z)\mapsto(-g,-z)\), the physical argument \(gz\) is unchanged, \(g^{-2}\) is unchanged, and \(zHz\) is unchanged. Thus
\[
W_{-g}(-z)=W_g(z),\qquad
O_i(-g,-z)=O_i(g,z).
\]
The domain and Lebesgue measure are invariant under \(z\mapsto-z\). Every joint moment, and therefore every cumulant, satisfies (5.1). In particular \(K_m'(0)=K_m'''(0)=0\).

Taylor's formula with integral remainder gives
\[
\mathcal R_{4,m}(g)
=\frac{g^4}{6}\int_0^1(1-s)^3K_m^{(4)}(sg)\,ds.
\tag{5.4}
\]
Apply Proposition 4.1. Its second-derivative bound also controls the displayed coefficient. \(\square\)

#### 5.1 Explicit coefficient

Use the following polynomials, with all derivatives evaluated at the identity physical field:

\[
O_{i,r}:=O_i^{(r)}(0,z)
=\frac{h^{-4}}{(r+1)(r+2)}
D^{r+2}\mathcal P_i(0)[z^{r+2}],
\qquad r=0,1,2,
\tag{5.5}
\]

\[
W_r:=W_r(0,z)
=-\frac1{(r+1)(r+2)}
D^{r+2}\mathcal A(0)[z^{r+2}]
+D^r\mathcal K(0)[z^r],
\qquad r=1,2.
\tag{5.6}
\]

Here \(O_{i,0}\) is quadratic, \(O_{i,1}\) is cubic, and \(O_{i,2}\) is quartic. \(W_1\) is a sum of cubic and linear terms; \(W_2\) is a sum of quartic and quadratic terms. No first-jet vanishing of E or the coarea is needed.

Write \(\kappa_0\) for cumulants in the actual constrained truncated Gaussian \(\nu_0\). Formula (4.3) at \(k=2\) gives

\[
\begin{aligned}
\mathcal C_{2,m}
={}&
\sum_i
\kappa_0(O_{1,0},\ldots,O_{i,2},\ldots,O_{m,0})
\\
&+2\sum_{i<j}
\kappa_0(O_{1,0},\ldots,O_{i,1},\ldots,
O_{j,1},\ldots,O_{m,0})
\\
&+2\sum_i
\kappa_0(O_{1,0},\ldots,O_{i,1},\ldots,O_{m,0},W_1)
\\
&+\kappa_0(O_{1,0},\ldots,O_{m,0},W_2)
\\
&+\kappa_0(O_{1,0},\ldots,O_{m,0},W_1,W_1).
\end{aligned}
\tag{5.7}
\]

All normalization responses are included through cumulants. For example, for one external field the last term is the third cumulant, not merely the expectation of \(O_{1,0}W_1^2\). The anchored decomposition in Section 3 gives an absolutely summed, volume-uniform meaning to the extensive \(W_r\) insertions after at least one external mark is present.

The leading term is
\[
K_m(0)=\kappa_0(O_{1,0},\ldots,O_{m,0}).
\tag{5.8}
\]

These are exact formulas with the common hard cutoff retained. Ordinary untruncated Wick formulas must not be substituted for \(\kappa_0\) without a separate cutoff-removal estimate.

### 6. What this does and does not settle

The \(O(g)\) native comparison of Annex F is sharpened, at identity retained background and on this fixed law, to an \(O(g^2)\) comparison with the quadratic native Gaussian fields. More precisely, its \(g^2\) coefficient is (5.7), and its remaining error is the localized \(O(g^4)\) bound (5.3), uniformly at every source order.

The new result includes four important restrictions.

- The inherited action is held fixed while computing the parameter derivatives. Its derivatives along the actual coupling trajectory and its dependence on earlier couplings are not bounded here.
- The retained background is the identity. At a nonzero background, \(g^{-2}\mathcal P(gz)\) need not have a removable zero-coupling limit; this proof does not cover that case.
- The cutoff is common and symmetric. If it is changed with \(g\), its boundary derivatives must be restored, and the displayed differentiation formula is no longer the whole response.
- The law is the specified homogeneous regular integral. It includes no arbitrary inherited R/boundary activity, and its native marks have not been identified with exact microscopic transported marks.

In particular, this theorem supplies neither the full coupling-flow derivative theorem nor a multiscale matching theorem. Its second coefficient can depend on the frozen shell action \(E_*\). Calling it the universal beta-function coefficient would require a separate identification.

### Source scope and proof dependencies

The fixed-law density, uniform mean and all-\(p\) coordinate theorem, and weighted covariance budget are those proved in Annex F, Sections 1--4. The native physical chart and coarea hypotheses are those of Annex B, Section 5. The complete classical curvature normalization and homogeneous use of CMP102 are in Annex B, Section 9. The real cut bound is the real-cumulant theorem.

The primary scope remains CMP102 Proposition 9 and (190) for admitted analytic minimizing fields; CMP109/CMP116 for the fixed-domain complete regular activities and their carrier summation; and the exact source-free constraint chart. No complete-history complex domain or coupling derivative is imported from those field-analytic statements.

The extension to six fixed physical derivatives, polynomial coupling-derivative budgets, finite-anchor summation, parity identity, and second-order expansion are proved in this note.


---
