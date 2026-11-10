# Conditional means, native moments and Gaussian comparison

**Annex F.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Conditional moment estimate

The full transported-observable matching theorem M0 remains open. This note closes a quantitative premise that had been left explicit in the native moment theorems: the local mean of the nonlinear conditional fluctuation field. It also proves a volume-uniform, all-order comparison of the native marked cumulants with their constrained truncated-Gaussian counterparts.

Both conclusions apply to the **specified homogeneous, fixed-domain, no-R regular integral** with the complete inherited regular E action and the new coarea factor retained. They do not apply to an arbitrary CMP119 multiscale history merely because its current large-field set is empty. In particular, the fixed-domain CMP109/CMP116 activity norm used below must not be transplanted to a changed CMP119 domain with a different activity prefactor.

The labels are P for a result proved from the displayed source-specific inputs, L for those scoped primary inputs, and O for an estimate not proved for the full Wilson/RG law. No novelty or independent formal-validation claim is made.

The new mean estimate is stronger than substituting the cutoff into the field bounds:

\[
\boxed{
\sup_i|\mathbb E_\nu z_i|\le Cg,\qquad
\sup_i\|z_i\|_{L^p(\nu)}\le C\sqrt p,\quad p\ge1.
}
\tag{0.1}
\]

It holds uniformly in volume and in every admissible common symmetric product cutoff \(P\) with \(gP\le\delta\), where \(\delta>0\) is fixed and sufficiently small. No auxiliary condition \(gP^2\to0\) is needed. The actual logarithmic window is included.

For a native field at physical scale \(h\), this yields

\[
\boxed{
\|O_{\alpha,x}\|_p
\le Ch^{-4}(B_x+\sqrt p)^2,
}
\tag{0.2}
\]

\[
\boxed{
\|O_{\alpha,x}-\mathbb E O_{\alpha,x}\|_p
\le Ch^{-4}\bigl[(1+B_x)\sqrt p+p\bigr],\qquad
\|\|\nabla O_{\alpha,x}\|_{\gamma,x}\|_p
\le Ch^{-4}(B_x+\sqrt p).
}
\tag{0.3}
\]

Here \(B_x\) is the actual reference-curvature bound divided by \(g\), with the fixed local enlargement required by the stencil. It has not been bounded in the outer history law. If the admitted background has \(B_x\le CP(g)\), the resulting conditional bounds have the corresponding explicit logarithmic background factor. A fixed physical regularity bound alone permits \(B_x\) to grow like \(g^{-1}\).

### 1. The actual conditional density and its source inputs

Let the free-coordinate block set \(\mathcal I\) be a finite homogeneous current lattice or torus. Each block has dimension bounded by a fixed number, and the current metric satisfies

\[
\sup_i\sum_j e^{-c d(i,j)}<\infty
\quad(c>0)
\tag{1.1}
\]

uniformly in volume. The current lattice has dimension four. Group and admitted block-size constants are fixed.

The domain is a common symmetric convex product

\[
\mathcal D_P=\prod_{i\in\mathcal I}
\{z_i:|z_i|\le P\}.
\tag{1.2}
\]

Scalar coordinate cubes or the source's finite-dimensional norm balls are allowed. Every norm used on an individual block is fixed, so their equivalence constants are independent of volume. The domain and selector are independent of the interpolation parameter introduced below.

The reference field, exact averaging chart and gauge are frozen. Let

\[
d\nu(z)=Z^{-1}\mathbf1_{\mathcal D_P}(z)
J(gz)\exp\{-S_g(z)+E_k(U(gz))\}\,dz.
\tag{1.3}
\]

The classical action is the exact source-free constrained action, including the particular gauge-fixing term if that version is used. Its stationary point is at \(z=0\). Write

\[
H_0=D^2 S_g(0),\qquad
R_{\rm cl}(z)=S_g(z)-S_g(0)-\tfrac12\langle z,H_0z\rangle.
\tag{1.4}
\]

Thus \(DR_{\rm cl}(0)=D^2R_{\rm cl}(0)=0\). The term \(E_k\) is the full inherited regular action **after its coupling subtractions**, so the flowed classical coefficient in \(H_0\) is not counted a second time. The new coarea factor \(J\) occurs once.

Define

\[
W(z)=-R_{\rm cl}(z)+E_k(U(gz))+\log J(gz).
\tag{1.5}
\]

Additive constants in W do not matter. No R activity, boundary B activity, nonconstant old coupling, moving selector or arbitrary conditioned exterior is hidden in this notation.

The classical argument and the fixed-domain regular activity lemma supply the following actual estimates, for \(gP\le\delta\) inside a sufficiently small physical analytic neighborhood.

#### 1.1 Classical and Gaussian input

The true constrained precision has a uniform positive gap and the weighted locality needed for the previous real covariance theorem. The complete homogeneous classical calculation gives a nonnegative tree majorant K such that

\[
|D_iD_jD_l R_{\rm cl}(z)|
\le Cg\,K(i,j,l),
\tag{1.6}
\]

\[
\sup_i\sum_{j,l}e^{\gamma_0\tau(i,j,l)}
K(i,j,l)\le C.
\tag{1.7}
\]

Replace an initially obtained majorant by the sum of its six permutations in the indices \(i,j,l\). This makes K symmetric, preserves (1.6), and changes the uniform sum in (1.7) by only a fixed factor. One may equivalently take a fixed exponential tree majorant with a smaller decay rate. The source of (1.6)–(1.7) is the homogeneous specialization of CMP102 Proposition 9 and (190), together with the exact curvature cancellation and \(\eta^4\)-weighted fine plaquette sum proved. The complete third chain rule is retained.

Since \(R_{\rm cl}\) has zero first and second jets,

\[
|D_iR_{\rm cl}(z)|
\le Cg\sum_{j,l}K(i,j,l)|z_j||z_l|,
\tag{1.8}
\]

\[
|D_iD_jR_{\rm cl}(z)|
\le Cg\sum_l K(i,j,l)|z_l|.
\tag{1.9}
\]

These follow by Taylor's integral formula along \(sz\), \(0\le s\le1\). They are bounds for the actual remainder, not only its cubic Taylor polynomial.

#### 1.2 The inherited E first derivative is controlled as well as its Hessian

On the **fixed small-field analytic domain**, CMP116 Lemma 1 bounds the complete regular fluctuation activities by

\[
|V'_{k,Y}(B)|
\le C E_0\epsilon_1 e^{-\kappa_*d_k(Y)}
\quad\text{for } \|B\|_\infty<\epsilon_1/g.
\tag{1.10}
\]

The exact free-coordinate argument already contains the nonlinear chart. The base value subtracted in the source identity is constant in B.

Choose \(\delta<\epsilon_1/2\). Coordinate Cauchy estimates at every real point of \(\mathcal D_P\) then give

\[
|D_iV'_{k,Y}(z)|
\le C E_0g\,e^{-\kappa_*d_k(Y)},\qquad
|D_iD_jV'_{k,Y}(z)|
\le C E_0g^2\epsilon_1^{-1}e^{-\kappa_*d_k(Y)}.
\tag{1.11}
\]

The current M-cell carrier summation has the same entropy reserve as in the source lemma. Therefore

\[
\sup_i|D_iE_k(U(gz))|\le C E_0g,\qquad
\sup_i\sum_j e^{\gamma_0d(i,j)}
|D_iD_jE_k(U(gz))|
\le C E_0g^2/\epsilon_1.
\tag{1.12}
\]

The old-scale sum is the source's already-renormalized sum. No new unweighted sum of \(g_j^2\) is introduced.

The constant \(C E_0g\) in the first estimate may depend on the fixed admitted source parameters. It does not depend on P, the shell depth or the number of current blocks within this fixed-domain scope. A value bound on a different domain does not imply (1.12).

#### 1.3 The exact coarea first derivative

In the actual chart,

\[
a(z)=gCz-hD(gCz),\qquad
J(gz)=\text{constant}\,
\frac{J_{\rm Haar}(a(z))}
{\det[I+DN(a(z))h]}.
\tag{1.13}
\]

The physical chart and its weighted derivatives are uniform in the homogeneous regular template. Put
\(A(z)=DN(a(z))h\). Its weighted row and column norm is below \(1/2\) after reducing the physical radius.

For the Haar logarithm, differentiate its local analytic summands and use \(D_ia=O(g)\) with exponential localization. For the determinant,

\[
D_i\log\det(I+A)=
\operatorname{Tr}[(I+A)^{-1}D_iA].
\tag{1.14}
\]

The inverse is a convergent weighted Neumann series. Each term in \(D_iA\) has a factor g and a tree connection from i to its two matrix indices. The closed-walk trace sum is therefore bounded by \(Cg\); there is no volume factor. Differentiating once more gives either one second derivative or two first derivatives, each with total order \(g^2\). The same anchored sums give

\[
\sup_i|D_i\log J(gz)|\le Cg,\qquad
\sup_i\sum_j e^{\gamma_0d(i,j)}
|D_iD_j\log J(gz)|\le Cg^2.
\tag{1.15}
\]

This extends the previously proved coarea Hessian estimate by the first derivative needed here. The determinant is the new exact constraint determinant; older measure terms remain in E.

#### 1.4 One uniform covariance estimate for the full interpolation

For \(0\le t\le1\), define

\[
d\nu_t(z)=Z_t^{-1}\mathbf1_{\mathcal D_P}(z)
\exp[-\tfrac12\langle z,H_0z\rangle+tW(z)]\,dz.
\tag{1.16}
\]

The Hessian estimate gives

\[
\eta_{\gamma_0}(W)
\le C\delta+Cg^2(1+E_0/\epsilon_1).
\tag{1.17}
\]

Choose a fixed small \(\delta\), then a sufficiently small g, so this budget fits inside the true constrained gap. Choose \(0<\gamma<\gamma_0\) so that the weighted conjugation error of \(H_0\) is also inside that gap. The previous vector-resolvent proof then supplies constants \(\lambda,c>0\), independent of t, P and volume, with

\[
D^2\!\left(\tfrac12zH_0z-tW(z)\right)\ge\lambda I,
\tag{1.18}
\]

\[
|\operatorname{Cov}_{\nu_t}(F,G)|
\le C\sum_{i,j}e^{-\gamma d(i,j)}
\|D_iF\|_{L^2(\nu_t)}
\|D_jG\|_{L^2(\nu_t)}.
\tag{1.19}
\]

The product convex boundary is part of this statement. An arbitrary selected interface does not inherit it. The fixed source-dependent cutoff has not been differentiated.

### 2. A volume-uniform mean theorem

#### Theorem 2.1 — nonlinear conditional means and all-p fluctuations, P

For the exact density (1.3) in the scope above,

\[
\sup_{0\le t\le1}\sup_i
|\mathbb E_{\nu_t}z_i|
\le Cg,
\tag{2.1}
\]

\[
\sup_{0\le t\le1}\sup_i
\|z_i\|_{L^p(\nu_t)}
\le C\sqrt p,\qquad p\ge1.
\tag{2.2}
\]

The constants are independent of volume and of the admissible symmetric cutoff P. The reference density \(\nu_0\) is the actual constrained Gaussian restricted to the same product domain, not an unconditioned replacement on a different domain.

**Proof.** A linear real tilt leaves the Hessian lower bound (1.18) unchanged. For any scalar component \(X=v\cdot z_i\), the unweighted covariance inequality in the tilted measure gives

\[
\frac{d^2}{ds^2}\log\mathbb E_{\nu_t}e^{sX}
=\operatorname{Var}_{\nu_{t,s}}(X)
\le\lambda^{-1}|v|^2.
\tag{2.3}
\]

Integrating twice proves

\[
\mathbb E_{\nu_t}
e^{s(X-\mathbb EX)}
\le e^{s^2|v|^2/(2\lambda)},\qquad
\|z_i-\mathbb E_{\nu_t}z_i\|_p\le C\sqrt p.
\tag{2.4}
\]

The block dimension is fixed. These estimates do not yet bound the mean.

Put

\[
m_i(t)=\mathbb E_{\nu_t}z_i,\qquad
M(t)=\max_i|m_i(t)|.
\tag{2.5}
\]

At finite volume, every function is integrable on the bounded domain, and

\[
m_i'(t)=\operatorname{Cov}_{\nu_t}(z_i,W).
\tag{2.6}
\]

Using (2.4) at order four,

\[
\|z_jz_l\|_2
\le \|z_j\|_4\|z_l\|_4
\le C[1+M(t)^2].
\tag{2.7}
\]

Equations (1.8), (1.12), (1.15) and the summability of K therefore imply

\[
\sup_j\|D_jW\|_{L^2(\nu_t)}
\le Cg[1+M(t)^2].
\tag{2.8}
\]

Insert (2.8) into (1.19), with \(F=z_i\), and sum the exponentially decaying kernel:

\[
|m_i'(t)|\le Cg[1+M(t)^2].
\tag{2.9}
\]

The domain is symmetric and the quadratic reference density is even, so \(m_i(0)=0\). Consequently

\[
M(t)\le Cg\int_0^t[1+M(s)^2]\,ds.
\tag{2.10}
\]

Let the right side be \(y(t)\). Then \(M\le y\), \(y(0)=0\), and

\[
y'(t)\le Cg(1+y(t)^2).
\]

Thus \(\arctan y(t)\le Cgt\), and

\[
M(t)\le\tan(Cgt)\le2Cg,\qquad0\le t\le1,
\tag{2.11}
\]

after fixing a small coupling ceiling. Combining (2.11) with (2.4) gives (2.2). All constants used before taking the maximum are uniform in the finite block set, so no factor of its size occurs. This proves the theorem. \(\square\)

The Riccati comparison is useful here because the crude cutoff estimate would give \(gP^2\), which need not be small on the largest fixed physical window. The exact quadratic drift bound and the centered concentration estimate remove that artificial restriction.

### 3. Verification of the native moment budget

Let \(O_{\alpha,x}\) be any of the 21 native curvature-bilinear stencils in the exact nonlinear chart, with physical factor \(h^{-4}\) retained. The scalar Wilson-action mark is also included. The deterministic theorem supplies

\[
|O_{\alpha,x}(z)|
\le Ch^{-4}[B_x+Z_x(z)]^2,\qquad
Z_x(z)=\sum_j e^{-2\gamma d(x,j)}|z_j|,
\tag{3.1}
\]

\[
\|\nabla O_{\alpha,x}(z)\|_{\gamma,x}
:=\left(\sum_j e^{2\gamma d(x,j)}
|D_jO_{\alpha,x}(z)|^2\right)^{1/2}
\le Ch^{-4}[B_x+Z_x(z)].
\tag{3.2}
\]

The first two native derivative estimates and finite local template also give the corresponding mean-value inequality along a segment in the convex product domain.

#### Theorem 3.1 — all-p native field and gradient norms, P

Uniformly for \(\nu_t\), \(0\le t\le1\), and \(p\ge1\),

\[
\|O_{\alpha,x}\|_p
\le Ch^{-4}(B_x+\sqrt p)^2,
\tag{3.3}
\]

\[
\|O_{\alpha,x}-\mathbb E_{\nu_t}O_{\alpha,x}\|_p
\le Ch^{-4}\bigl[(1+B_x)\sqrt p+p\bigr],
\tag{3.4}
\]

\[
\|\|\nabla O_{\alpha,x}\|_{\gamma,x}\|_p
\le Ch^{-4}(B_x+\sqrt p).
\tag{3.5}
\]

In particular one can take the quadratic-growth cumulant budget

\[
B_{i,m}\le A_i m,\qquad D_{i,m}\le A_i\sqrt m,\qquad
A_i=C h^{-4}(1+B_{x_i})
\tag{3.6}
\]

for centered marks. The uncentered full-product budget has
\(A_i^{\rm full}=Ch^{-4}(1+B_{x_i})^2\).

**Proof.** Minkowski and (2.2) give \(\|Z_x(z)\|_p\le C\sqrt p\). This proves (3.3) and (3.5).

For the sharper centered bound, write \(m=\mathbb E_{\nu_t}z\), \(\xi=z-m\), and
\[
X_x(\xi)=\sum_j e^{-\gamma d(x,j)}|\xi_j|.
\]
Then \(\|X_x\|_p\le C\sqrt p\), and \(\sum_j e^{-2\gamma d(x,j)}|m_j|\le Cg\). The segment from m to z remains in \(\mathcal D_P\), because a mean of a measure supported in a convex set lies in that set.

Apply the fundamental theorem of calculus to \(O(z)-O(m)\). Cauchy–Schwarz with the reciprocal gradient weight, followed by (3.2), gives

\[
|O_{\alpha,x}(z)-O_{\alpha,x}(m)|
\le Ch^{-4}\bigl[(B_x+Cg)X_x(\xi)+X_x(\xi)^2\bigr].
\tag{3.7}
\]

Taking \(L^p\) norms, using the \(2p\) norm for the square, and then subtracting the expectation costs at most a factor two. This proves (3.4). Substitution of \(p=2m\) gives (3.6). \(\square\)

This is an actual conditional norm theorem, with the complete inherited regular E and exact new coarea retained. It is no longer a hypothesis about an unspecified conditional mean. The reference-curvature factor and the restriction to the selected homogeneous regular law remain explicit.

#### Corollary 3.2 — native cumulants and full products, P

For \(m\ge2\), the previous real cut theorem now gives

\[
\boxed{
|\kappa_{\nu}(O_{\alpha_1,x_1},\ldots,O_{\alpha_m,x_m})|
\le C^{m+1}(m!)^2 h^{-4m}
\prod_{i=1}^m(1+B_{x_i})
\exp\!\left[
-\frac{\gamma\,\tau(x_1,\ldots,x_m)}{m-1}
\right].
}
\tag{3.8}
\]

The full moments satisfy

\[
\left|\mathbb E_\nu\prod_{i=1}^mO_{\alpha_i,x_i}\right|
\le C^m m!\,h^{-4m}
\prod_i(1+B_{x_i})^2.
\tag{3.9}
\]

For (3.8), center the marks and insert (3.6) into the already proved real cut estimate. The two differentiated factors contribute \(\sqrt m\) each, the other \(m-2\) factors contribute m each, and the partition coefficient is bounded by \((m-1)!2^{m-2}\). Deleting the longest edge of a minimum spanning tree supplies the stated range; \(m^m\le e^m m!\) yields the fixed factorial exponent two. Formula (3.9) is Hölder with exponent m, (3.3), and the same elementary factorial inequality.

These are point-mark conditional estimates. They have not been identified with a joint OS test-space bound on the complete Wilson hierarchy. The current \(h^{-4m}\), the outer background distribution and the change from native to exactly transported marks still have to be treated.

### 4. An all-order, volume-uniform comparison with the actual Gaussian reference

The same estimates give a quantitative comparison theorem for the real conditional cumulants, without requiring a common exponential-source disc. It retains the same product cutoff in the reference Gaussian.

#### 4.1 A local decomposition of the complete perturbation

For each coordinate block j put

\[
R_j(z)=\int_0^1
\langle z_j,D_jW(sz)\rangle\,ds.
\tag{4.1}
\]

Then, at every finite volume,

\[
W(z)-W(0)=\sum_{j\in\mathcal I}R_j(z).
\tag{4.2}
\]

This identity is the radial fundamental theorem of calculus. It does not replace W by its Taylor polynomial or assume a source-dependent minimizing map.

For \(p\ge1\), (1.8) and the all-p coordinate moments give

\[
\|D_jW\|_{L^p(\nu_t)}\le Cgp.
\tag{4.3}
\]

Differentiate (4.1):

First decrease the working \(\gamma\), if necessary, so that \(4\gamma\) is strictly smaller than every tree and Hessian decay rate used in (1.7), (1.12), (1.15), and the native derivative bound. All earlier covariance estimates remain valid at this smaller weight. The unused exponential decay pays the anchor weights and subsequent convolutions in this section.

\[
D_iR_j(z)=\delta_{ij}\int_0^1D_jW(sz)\,ds
+\int_0^1s\,D_iD_jW(sz)z_j\,ds,
\tag{4.4}
\]

with the evident block contraction. Using (1.9), the E/coarea Hessian estimates and the tree weights yields

\[
\boxed{
\|R_j-\mathbb E_{\nu_t}R_j\|_p\le Cg p^{3/2},\qquad
\|\|\nabla R_j\|_{\gamma,j}\|_p\le Cgp.
}
\tag{4.5}
\]

For the first bound, \(z_jD_jW\) contains at most cubic products of coordinates in its majorant. For the second, the nontrivial term is \(z_jD_iD_jR_{\rm cl}\), a quadratic product times g. The exponential tree majorant makes the weighted sum over i finite. The E/coarea terms have first derivative \(O(g)\) and Hessian \(O(g^2)\); they fit the same estimates. The evaluation at \(sz\) does not change the coordinate moment majorants, since \(0\le s\le1\).

The summability in (4.5) is the needed locality of the perturbation current. Merely knowing that W has zero mean, or is small as an extensive scalar, would not prove it.

#### Theorem 4.1 — native cumulant comparison, P

For the same native marks and the same fixed reference Gaussian \(\nu_0\),

\[
\boxed{
\begin{aligned}
&
\left|
\kappa_{\nu_1}(O_{\alpha_1,x_1},\ldots,O_{\alpha_m,x_m})
-\kappa_{\nu_0}(O_{\alpha_1,x_1},\ldots,O_{\alpha_m,x_m})
\right|\\
&\quad\le
g C^{m+1}(m!)^2 h^{-4m}
\prod_{i=1}^m(1+B_{x_i})
\exp\!\left[
-\frac{\gamma\,\tau(x_1,\ldots,x_m)}{4m}
\right],
\qquad m\ge1 .
\end{aligned}
}
\tag{4.6}
\]

Set \(\tau(x_1)=0\) for \(m=1\). Constants are independent of the volume, cutoff P and source order m.

**Proof.** For fixed m and finite volume, differentiate the finite moments defining the cumulant:

\[
\frac{d}{dt}\kappa_{\nu_t}(O_1,\ldots,O_m)
=\kappa_{\nu_t}(O_1,\ldots,O_m,W)
=\sum_j\kappa_{\nu_t}(O_1,\ldots,O_m,R_j).
\tag{4.7}
\]

The marks do not depend on t. An additive constant in W contributes zero.

Apply the real cut theorem to \(m\) quadratic-growth marks and the one cubic-growth mark \(R_j\). At order \(2(m+1)\), (3.6) and (4.5) give

\[
B_i\le C A_i(m+1),\quad D_i\le C A_i\sqrt{m+1},
\qquad
B_R\le Cg(m+1)^{3/2},\quad D_R\le Cg(m+1).
\]

Whether the differentiated pair consists of two O marks or one O mark and R, the polynomial factor before the pair count is bounded by
\[
C^{m+1}g(m+1)^{m+1/2}\prod_i A_i.
\]
The partition coefficient is at most \(m!2^{m-1}\), and there are at most \((m+1)^2\) crossing pairs. The inequality \(m^m\le e^m m!\) absorbs this into \(gC^{m+1}(m!)^2\prod_i A_i\).

Delete a longest edge of a minimum spanning tree on \(x_1,\ldots,x_m,j\). The resulting cut gives

\[
|\kappa_{\nu_t}(O_1,\ldots,O_m,R_j)|
\le gC^{m+1}(m!)^2
e^{-\gamma\tau(x_1,\ldots,x_m,j)/m}\prod_i A_i.
\tag{4.8}
\]

The tree length with the additional point obeys

\[
\tau(x_1,\ldots,x_m,j)\ge\tfrac12\tau(x_1,\ldots,x_m),
\qquad
\tau(x_1,\ldots,x_m,j)\ge d(j,x_1).
\tag{4.9}
\]

The first inequality follows by doubling the enlarged tree, traversing it through the marked vertices, and shortcutting the walk; the second follows from its path from j to \(x_1\). Consequently

\[
e^{-\gamma\tau(x_1,\ldots,x_m,j)/m}
\le
e^{-\gamma\tau(x_1,\ldots,x_m)/(4m)}
e^{-\gamma d(j,x_1)/(2m)}.
\]

The sum over j is at most \(C(m+1)^4\) on a four-dimensional current lattice. This polynomial is absorbed into another fixed exponential in m. Integrate (4.7) from zero to one. This proves (4.6). \(\square\)

The same interpolation and the product covariance formula give

\[
\left|
\mathbb E_{\nu_1}\prod_iO_i-
\mathbb E_{\nu_0}\prod_iO_i
\right|
\le gC^{m+1}m!h^{-4m}
\prod_i(1+B_{x_i})^2.
\tag{4.10}
\]

For the first moment, the sharper direct estimate is
\[
|\mathbb E_{\nu_1}O_{\alpha,x}
-\mathbb E_{\nu_0}O_{\alpha,x}|
\le Cg h^{-4}(1+B_x).
\tag{4.11}
\]

To prove (4.10), differentiate the product expectation and use the vector covariance representation. In each of its m terms there is one native gradient, \(m-1\) native values and a first gradient of W. Apply Hölder at order \(2m\) to the native factors, use (4.3) at order two for W, and sum the exponentially localized covariance kernel. The resulting \(g\,m^{m+1/2}\) factor is bounded by \(gC^m m!\).

#### Scope of this comparison

The Gaussian reference is constrained and truncated on the same domain. The theorem does not remove that cutoff, expand the native marks into a polynomial, or identify the Gaussian comparison with the exact microscopic transport through prior RG steps. Such additional identifications require their own estimates.

In particular, (4.6) is not a theorem that the full Yang–Mills hierarchy differs from a free Gaussian hierarchy by O(g). It is a theorem about one specified current conditional law and its actual native marks. The explicit physical and reference-curvature factors remain.

The O(g) factor is a one-step perturbation size. It is not a summable multiscale remainder on a typical AF trajectory: \(\sum_jg_j\) need not converge. Extracting the marginal mixing, proving its actual running normalization and assigning irrelevant scale gains to the remainder are still required. No unproved O(g²) marginal improvement or coupling derivative has been inferred from this comparison.

### 5. Why the scalar coupling derivative still does not close full matching

The full Wilson total action has the exact relation

\[
\mathbb E_{\beta}e^{s\beta S}
=Z(\beta(1-s))/Z(\beta).
\tag{5.1}
\]

For a differentiable family of positive integral-preserving maps \(P_\beta\), the earlier exact identity is

\[
Q_\beta S
=-\partial_\beta\log(P_\beta e^{-\beta S})
+\frac{(\partial_\beta P_\beta)e^{-\beta S}}
{P_\beta e^{-\beta S}}.
\tag{5.2}
\]

Freezing the map eliminates its derivative but does not supply an effective-action formula at nearby coupling for that frozen family. Moving with the source-free construction gives the known source-free representation but restores the current in the second term. The normalization derivative of each reference kernel, derivative of any moving coordinates, and selector changes belong in that current.

For an individual positive replacement with normalized reference kernel \(K_\beta(u'|v)\), the current is exactly
\(\partial_\beta\log K_\beta(u'|v)\). The original mark after that replacement is a conditional expectation at fixed v and does not depend on the fresh variable \(u'\). The current cancels the artificial reference-score contribution in the adaptive output density. A zero average of that current does not bound its product with another retained mark, and does not make it contact-local.

The fixed-domain estimates above are derivatives in physical free-field coordinates. They are not estimates of \(\partial_\beta E_k\), the coupling derivative of the renormalized trajectory, or the coupling derivative of the complete normalized history density. Those derivative estimates have not been established here. A small field-analytic remainder may have large parameter derivatives unless a corresponding parameter regularity theorem is proved.

Therefore the scalar total-coupling identity does not currently yield a current-scale bound for \(Q_{0:k}F_0\). Its special fixed-box cancellation is retained, but no new claim of protected scalar transport through the complete construction is made.

### 6. What the argument changes in the decomposition

The following local regular obligations are now P in the displayed fixed-domain, homogeneous, no-R scope:

1. The complete E/coarea perturbation has the first-gradient budget needed by the real conditional mean theorem.
2. The actual conditional fluctuation mean is \(O(g)\), uniformly in volume and in all admissible symmetric product windows \(gP\le\delta\).
3. The native all-p moment and weighted gradient bounds have the quadratic growth exponents needed by the real cumulant theorem, with fixed factorial growth at every source order.
4. Native marked cumulants admit a volume-uniform localized \(O(g)\) comparison with the constrained Gaussian on the same domain.

The following remain O:

- The required estimate for the actual full CMP119 boundary and inherited R law.
- A bound on the reference background \(B_x\) after averaging all retained data and histories.
- Matching the exactly transported microscopic marks to current native fields and generated remainders.
- The full-law product-error or joint-kernel estimate, its contact assembly and its OS growth conclusion.
- The interacting operator estimate, tensor rotation restoration, quantitative ultraviolet identification and phase transfer.

The new conditional moment theorem is useful because it removes an explicit premise from an already established covariance-to-cumulant argument. It does not complete the full M0 or H0 estimate.

### Source scope

- [CMP109 (1987), 249–301](https://doi.org/10.1007/BF01215223): exact fixed-domain homogeneous small-field conditional integral, true constrained quadratic form and free coordinates.
- [CMP116 (1988), 1–22](https://doi.org/10.1007/BF01239022), Lemma 1 and its fixed analytic ball: complete inherited regular E fluctuation activity norm used for (1.10)–(1.12).
- CMP102 (1985), 277–309, Proposition 9 and (190): homogeneous minimizing-field derivative and spatial-gradient input; the curvature-normalized full classical derivative proof is the result.
- The weighted covariance and real cut-cumulant estimates require the product domain, nonlinear chart and coarea density used above.
- Annex B, Section 9: the explicitly specified homogeneous no-R coercivity theorem. A transfer of the same fixed E prefactor to an arbitrary changed CMP119 domain is not used.

No unpublished coupling-response theorem, complete all-source action normal form or unproved tensor-product-to-joint-kernel passage is imported.


---
