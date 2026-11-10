# Complex radius reserve for the phase cone

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

This note proves an analytic lemma. Its source application remains conditional on the enumerated chart, reality, and coefficient inputs. In particular a bound for the pure Gaussian kernel does not, by itself, bound the same normalized kernel after ordinary interactions are restored.

## 1. A phase bound controls normalization without a lower mass estimate

Let `(X,mu)` be a finite positive measure space, or a sigma-finite space on which the displayed integrals converge. Let `w_xi(a)` be the exact unnormalized density on a support independent of the complex external parameter `xi`. Suppose that for each `xi` there is a real scalar `phi_0(xi)` such that, almost everywhere on the support,

\[
 w_\xi(a)=|w_\xi(a)|\exp i[\phi_0(\xi)+\theta_\xi(a)],
 \qquad |\theta_\xi(a)|\le\eta<\pi/2.
 \tag{PC1}
\]

Assume `0<integral |w_xi| dmu<infinity`. Then

\[
 |\tau_\xi|=\left|\int w_\xi\,d\mu\right|
 \ge\cos\eta\int|w_\xi|\,d\mu,
 \qquad
 \tau_\xi:=\int w_\xi\,d\mu.
 \tag{PC2}
\]

Indeed the real part after multiplication by `exp(-i phi_0)` is at least the right-hand side. Thus the exact normalized functional

\[
 \Pi_\xi f=\frac{\int w_\xi(a)f(a)\,d\mu(a)}{\tau_\xi}
 \tag{PC3}
\]

obeys

\[
 \Pi_\xi1=1,\qquad
 \|\Pi_\xi\|_{L^\infty\to\mathbb C}\le\sec\eta.
 \tag{PC4}
\]

The same bound applies to `xi`-dependent tests with their uniform norm, and to positive internal history sums included in `mu`. The positive comparison `|w_xi| mu` may depend on `xi`; no holomorphy of this comparison is needed. Real variations of the density may be arbitrarily large. Neither a ratio to one fixed real-center density nor a positive uniform lower bound for `tau_xi` is assumed.

If the exact density is holomorphic and locally integrably dominated on the fixed support, its unnormalized integral is holomorphic. Equation (PC2) makes its reciprocal holomorphic. On a compatible common function algebra this proves operator-norm holomorphy, using dominated Cauchy integrals and (PC4). A pointwise choice of `phi_0` does not define the operator and need not be analytic.

The mass `tau_xi` remains in the exact action wherever the identity `T=tau Pi` puts it. The estimate does not remove or freeze its derivatives.

## 2. A larger radius bounds the phase of a real analytic scalar

Let `F` be holomorphic on a complex Banach ball `B(x_0,R)`, real at the real point `x_0`, and bounded in modulus by `B`. If `||v||<=delta<R`, one-dimensional Cauchy estimates along `x_0+t v` give

\[
 |\Im F(x_0+v)|
 \le |F(x_0+v)-F(x_0)|
 \le B\frac{\delta}{R-\delta}.
 \tag{PC5}
\]

For a family of local coefficients `F_gamma`, apply this estimate on each actual admitted local ball. If `delta_gamma/R_gamma<=zeta<1` and the deterministic sum of their large-chart bounds is `sum B_gamma<=B_tot`, then

\[
 \left|\Im\sum_\gamma F_\gamma(x_0+v)\right|
 \le B_{\rm tot}\frac{\zeta}{1-\zeta}.
 \tag{PC6}
\]

Absolute convergence justifies the sum. The centers may depend on the real integrated variables. They may also be selected pointwise at the external complex point, provided they are real, the exact scalar is real there, and the stated ball and distance inequalities actually hold. The analytic family itself remains the exact fixed-support source family.

For a real quadratic form `a^T K(xi) a/2`, with real coordinates `|a_i|<=P` and the native weighted row bound `sup_i sum_j |Im K_ij|<=delta_K`,

\[
 \left|\Im\tfrac12 a^T K(\xi)a\right|
 \le\tfrac12 N P^2\delta_K,
 \tag{PC7}
\]

where `N` is the actual coordinate count with its native integration measure. The imaginary part of every genuine cross block is included; the real size of that cross block need not be small. Determinant/coarea logarithms require their actual trace estimate or an independently verified application of (PC5). A density that has not been expressed on a fixed real support is not covered by this lemma.

## 3. Why three radii can be useful

Suppose the target native jets use

\[
 \alpha^-_j=g_j\ell_j^q,
 \qquad \ell_j=\log g_j^{-2},
\]

and the scalar estimate used for those jets is on the larger chart

\[
 \alpha^+_j=\ell_j^{Q_1}\alpha^-_j.
 \tag{PC8}
\]

A separate, independently established ordinary-source bound may be run on

\[
 \alpha^{++}_j=\ell_j^{Q_2}\alpha^+_j.
 \tag{PC9}
\]

Assume that an actual composed prefix input on the `+` chart is within native distance `C ell_r^d alpha_j^+` of a real input, with an admitted affine `++` radius `c alpha_j^{++}`. Assume also that the sum of the ordinary scalar bounds participating in that prefix is at most `C ell_r^D`. With the actual window profile comparison, (PC6) gives

\[
 |\Im V_{\rm ord}|\le C\ell_r^{D+d-Q_2}
 \tag{PC10}
\]

for a fixed sufficiently small coupling ceiling. Choose `Q_2>D+d+2` once. The right side tends to zero. A real ordinary action of size `C ell_r^D` causes no difficulty for (PC2).

This device must not create an infinite hierarchy of induction assumptions. It applies here only if the `++` bound for the ordinary sector is available independently of the unknown completed-scalar transfer. Unknown fresh completed interactions remain outside that phase estimate and require their proved small positive interaction norm on the `+` chart. In particular a proof of a completed bound on `+` cannot be justified by assuming that same bound on `++` and leaving the latter unproved.

All exponents, polynomial losses, and fixed constants are chosen before reducing the one common coupling ceiling. Since every radius is `g` times a fixed logarithmic power, this choice is compatible with finite smallness inequalities of that form. This observation does not by itself verify a particular source's admitted domains.

## 4. Full localization disks are a separate check

Small complex background phase does not imply small phase for an arbitrary directly decoupled Gaussian precision `K(s)`. At real background, complex decoupling variables can already give `Im K(s)=O(1)`.

For a conditional partial prefix, the source proposal is to stop at the last directly integrated old raw slot and exclude the whole actual attempted component from the localization set. If every affected coefficient row then carries a path across a true guard of width `cR_r`, and the full source disks preserve that row with a fixed residual rate, their contribution to the phase can be bounded by `poly(ell_r) exp(-cR_r)`. This requires the actual integrated support and all scalar/coarea factors to lie behind that guard. It must not be asserted for a top current fluctuation at the component boundary or for arbitrary inside-component decoupling.

## 5. Exact application checklist

To apply (PC1)--(PC10) to the C05 partial-prefix issue, one must verify the following mathematical inputs, rather than infer them from normalization alone:

1. The fixed real free-coordinate support after the literal selector relocation, including real old-adjoint arguments of the test function.
2. The exact factorization into a positive ordinary reference density, its mass, and the remaining fresh interactions, with every cross term retained.
3. A polynomial count of all integrated stage coordinates at their own native scales, using the actual eligible ancestral chain.
4. Real values of every included scalar at real native data, and its independently established large-chart local norm.
5. A real tube and affine margin for the actual composed source maps, including all fixed old-slot gauge conversions.
6. A phase bound on every required localization disk, with the full component excluded where the deep-support argument is used.
7. A small rooted norm for the fresh interactions left outside the reference; a Gaussian-only estimate does not supply this.

The phase-cone lemma and radius estimate above are proved. The complete actual-prefix transfer is not claimed merely by writing these inputs down.
