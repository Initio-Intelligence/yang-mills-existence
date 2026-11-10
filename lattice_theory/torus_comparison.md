# Scalar comparison across tori

**Status: (A3′) remains open.** This note examines the Gaussian part of the cross-torus scalar comparison used in [infinite_volume.md](infinite_volume.md), cited below as T6. It does not promote the conditional result of T6 to an unconditional one. P means proved below; L means a checked primary-source statement; C means an application requiring displayed extra hypotheses; O means unresolved.

## 1. Target and allowed inputs

The target is the comparison of the *specified complete scalar*, including the identity contributions from the large-field R-operation:

\[
\left|A_a(R)/\operatorname{Vol}(R)-A_a(T^*)/\operatorname{Vol}(T^*)\right|
\le C_{\rm sc}\ell_0^{-4}.
\]

No interface from another note is assumed to be completed. The abstract copying and scale-summation argument in [infinite_volume.md](infinite_volume.md) §4.4 is available as a proposed reduction and is checked where used. Its application to Gaussian normalizers requires an additional argument: uniform exponential decay of a matrix does not make it finite-range. In Bałaban, CMP 99 (1985), printed p.428, equations (3.156)–(3.158), the constrained fluctuation quadratic form contains an inverse compressed propagator; the text supplies exponential decay and a uniform positive lower bound. Those assertions alone do not verify the finite-range hypothesis of T6 Lemma 4.5.

This restriction concerns the application, not the elementary finite-range lemma. Section 3 below supplies a replacement for exponentially decaying translation-invariant kernels that are periodizations of one common kernel. The exact identification of each Balaban identity-background determinant with that construction remains an explicit obligation.

The relevant source results are those of Bałaban in CMP109, CMP116 and CMP119.

## 2. Definitions and conventions for the replacement lemma

Fix dimension d≥1 and h≥1 real or complex coordinates per cell. Let K(x), x∈Z^d, be h×h matrices with K(−x)=K(x)*. Assume, for fixed κ,B,m>0,

\[
\sum_{x\in\mathbb Z^d}e^{\kappa|x|_1}\|K(x)\|\le B,
\qquad \widehat K(\theta):=\sum_xK(x)e^{ix\cdot\theta}\ge m I_h
\quad(\theta\in\mathbb R^d).                                      \tag{2.1}
\]

The sum is an operator-norm sum, and positivity is Hermitian positivity. Necessarily B≥m. For an integer n≥1 define the matrix on Γ_n=(Z/nZ)^d by periodization:

\[
K_n(x,y)=\sum_{z\in\mathbb Z^d}K(x-y+nz).                         \tag{2.2}
\]

The series converges absolutely. All tori in this lemma use this *same kernel*. The lemma does not infer (2.2) from positivity or exponential decay of independently constructed finite-volume operators. Parameters of K may include a scale k and a coupling; the result is uniform in those parameters only if h,κ,B,m are uniform.

Define the determinant density d_n=n^{-d}\log\det K_n, with the real logarithm of the positive determinant. For application to a Gaussian normalization, multiply by −1/2 and include the explicitly chosen Gaussian coordinate-volume factor. That factor cancels per cell when h and the coordinate measure agree on the two tori.

## 3. Main theorem: quasi-local determinant comparison (P)

**Theorem 3.1.** Under (2.1)–(2.2), put

\[
\eta=\min\{\kappa/2,m\kappa/(4B)\},\quad
M_f=h\left[\max\{|\log(m/2)|,|\log(B+m/2)|\}+\pi/2\right].
\]

Then for every n≥1 and integer q≥1,

\[
|d_n-d_{qn}|\le
2M_f\left[\left(\frac{1+e^{-\eta n}}{1-e^{-\eta n}}\right)^d-1\right]
\le C(d,\eta)M_f e^{-\eta n}.                                    \tag{3.1}
\]

One valid constant is

\[
C(d,\eta)=4d\,(1+e^{-\eta})^{d-1}(1-e^{-\eta})^{-d}.
\]

In particular the estimate is independent of q, and finite-range support of K is unnecessary.

**Corollary 3.2 (P as an implication).** Suppose every step-k Gaussian scalar in dimension four, after choosing compatible coordinates, is a fixed finite sum of determinants of the form (2.2), with (2.1) uniform in k and a. Suppose also that the number of coordinates per cell and all coordinate-volume terms agree on covers. Then the sum of the Gaussian scalar-density differences over 0≤k≤K is bounded by C_G ℓ₀^{-4}, uniformly in cutoff and covering degree, for ℓ_k=L^k a and L^K a=ℓ₀.

This corollary repairs the analytic comparison once the periodization dictionary is proved. It is **not** yet a claim that every determinant occurring in the complete Balaban scalar satisfies that dictionary.

## 4. Proofs

### 4.1 Holomorphic logarithm and Fourier decay

The matrix series for K̂(z) converges absolutely and locally uniformly whenever |Im z_i|<κ, since |x·Im z|≤|x|₁ max_i|Im z_i|. If z=θ+iy and |y_i|≤η≤κ/2, then

\[
\begin{aligned}
\|\widehat K(\theta+iy)-\widehat K(\theta)\|
&\le\sum_x\|K(x)\|(e^{\eta|x|_1}-1)\\
&\le\eta\sum_x |x|_1e^{\kappa|x|_1/2}\|K(x)\|
\le (2\eta/\kappa)B\le m/2.
\end{aligned}
\]

The penultimate inequality uses r e^{−κr/2}≤2/κ for r≥0. Thus the Hermitian part of K̂(θ+iy) is at least (m/2)I, and its norm is at most B+m/2. All eigenvalues lie in the right half-plane, with moduli between m/2 and B+m/2. The principal matrix logarithm is holomorphic there, so

\[
f(z)=\operatorname{tr}\operatorname{Log}\widehat K(z)
\]

is periodic, holomorphic on a neighborhood of the closed η-strip, real for real z, and satisfies |f(z)|≤M_f. The neighborhood assertion follows by compactness of the real period cell and the strictly positive lower bound m/2. Equivalently, one can first use any smaller strip and then pass to η by a limit.

For the Fourier coefficients f̂(v), v∈Z^d, shift each contour by −iη sign(v_i) in the integral with exponential e^{−iv·θ}. Periodicity cancels the opposite vertical edges. This gives

\[
|\widehat f(v)|\le M_f e^{-\eta|v|_1}.                            \tag{4.1}
\]

This step concerns a scalar analytic function; it requires no commutativity of the matrices K(x).

### 4.2 Sampling and the covering comparison

Finite discrete Fourier transformation diagonalizes the convolution (2.2) into the h×h blocks K̂(2πj/n), j∈{0,…,n−1}^d. Each is positive, so

\[
d_n=n^{-d}\sum_j f(2\pi j/n)=\sum_{v\in\mathbb Z^d}\widehat f(nv).
\]

The second equality follows by the elementary finite geometric-series identity in each coordinate; exchanging sums is legitimate by (4.1). Consequently

\[
|d_n-\widehat f(0)|\le
M_f\sum_{v\ne0}e^{-\eta n|v|_1}
=M_f\left[\left(\frac{1+e^{-\eta n}}{1-e^{-\eta n}}\right)^d-1\right].
\]

Apply this on n and qn and use q≥1 for the first inequality in (3.1). For t=e^{−ηn}≤e^{−η}, the difference (1+t)^d−(1−t)^d is at most 2dt(1+t)^{d−1}, by the mean value theorem. Division by (1−t)^d proves the displayed constant. This proves Theorem 3.1.

### 4.3 Summing the ultraviolet scales

Write r=K−k and x₀=t*/ℓ₀. There are ℓ_k^{-4}=ℓ₀^{-4}L^{4r} cells per physical volume, and the reference lattice has side n_k=x₀L^r. The determinant comparison is at most C exp(−ηx₀L^r) per cell. Hence the complete sum of these differences is bounded by

\[
C\ell_0^{-4}\sum_{r=0}^{K}L^{4r}e^{-\eta x_0L^r}
\le C\ell_0^{-4}\sum_{r=0}^{\infty}L^{4r}e^{-\eta x_0L^r}<\infty.
\]

The convergence follows, for example, from the ratio of successive terms, L⁴ exp[−ηx₀(L−1)L^r], which tends to zero. The same argument handles a fixed finite number of determinant factors and their fixed powers. This proves Corollary 3.2. No equality between pointwise field-local functions on different tori was assumed: the common periodized kernel is the explicit cross-torus input.

## 5. Checked imports and source scope

### 5.0 A precise route to the missing kernel dictionary (P)

For absolutely summable matrix kernels A and B on Z^d, periodization is a convolution homomorphism:

\[
P_n(A*B)=(P_nA)(P_nB).
\]

Indeed both sides have entry at (x,y) equal to the absolutely convergent sum of A(x−u+nz)B(u−y+nw) over u∈Γ_n and z,w∈Z^d; regroup by the lifted intermediate point u−nz. It also preserves sums, adjoints and the identity kernel. If A has an absolutely summable convolution inverse B, then P_nB is the inverse of P_nA. Rectangular kernels allow the same argument for compositions of block averages and their adjoints, after choosing a common block cell.

The hypothesis (2.1) itself implies an exponentially summable inverse: K̂(z)^{-1} is holomorphic and bounded by 2/m on the η-strip from §4.1. Its Fourier coefficients decay exponentially by the same contour shift. Their convolution with K has Fourier symbol I_h, so these coefficients give the convolution inverse, with absolute convergence. Thus repeated finite compositions, sums, and uniformly invertible convolutions preserve exact periodization, if each operation is specified in these coordinates.

Consequently an identity-background operator assembled from common translation-covariant block kernels using these operations has the required covering dictionary. This is a finite algebraic verification, not a probabilistic comparison. Its outstanding part in the present application is the complete identification of all constrained spaces, inverses, graph choices, and scalar measures in the primary representation. A globally fixed gauge with a torus-dependent distinguished link, or an inverse with a removed zero mode, cannot be inserted into this lemma without a separate treatment.

**L, CMP99, printed pp.427–429.** Equations (3.156)–(3.158) describe the constrained quadratic form and the parametrization B=C B̄. The paragraph following (3.158) supplies a positive lower bound independent of k and the regular background, together with exponential decay. It does not assert finite-range support of C*Δ_k C. Theorems about its localized random-walk expansion must be used to identify its behavior on coverings. The printed statement, not an inference from the words “local stencil”, governs this distinction.

**L, flat-background operator identified more precisely.** Bałaban's CMP95, printed p.29, (1.65)–(1.67), defines Δ_k by the energy of its constrained minimizer and gives a Fourier representation and uniform two-sided comparison to the unit-lattice curl energy. CMP96, printed pp.249–250, (2.152)–(2.157), eliminates block axial-gauge and averaging constraints by B=C B′. At zero source its Gaussian integral is the coordinate factor L^{d|Λ′|} times the ordinary integral with positive quadratic form C*Δ_k C. Equation (2.157) supplies the lower bound γ′₀=γ₀ L^{−d−1}/(12d²). The final paragraph calls C short-ranged and C*Δ_k C exponentially decaying. This identifies the candidate matrix and a coordinate factor that must be counted; it still requires the full CMP109 scalar recipe to show that these are exactly all factors used there. The torus-independent Fourier-symbol construction, including its zero-mode convention, is the concrete place to verify the common-kernel condition of §5.0.

**L, LFR II, printed pp.355–356.** Equation (0.1) supplies a pointwise upper bound and a lower bound containing χ_k and the Wilson action divided by g_k². The following page states the independence of the displayed constants from k, the torus lattice and the field. The introduction explicitly keeps the small-effective-coupling assumption; the announced coupling theorem's proof was not published at the time of that 1989 article. This is not a finding about all subsequent literature.

**L, LFR II, printed pp.389–390.** The R-contribution after exponentiation has the estimate (1.100), with rare factor exp[−p₀(g_k)] and spatial decay. Its dependence on the field restricted to its carrier is stated before (1.99). Field locality alone does not prove naturality of the scalar under changing the torus. In particular, a torus-dependent additive constant would leave field locality unchanged.

**L, CMP119 and CMP116; full application not checked.** CMP119 §2 identifies the regular, R and boundary terms; its scalar recipe must be matched literally to the A_a(R) appearing in the target. CMP116 (2.38)–(2.41) provides localized activity bounds, but the conversion of its domain metric and carrier sum to the exact uniform scalar-density bound remains to be checked. No theorem in Sections 3–4 depends on treating these uncompleted source matches as established.

**L, Gaussian identification narrowed.** CMP109, printed pp.267–268, (2.11) explicitly identifies its quadratic form with CMP99 (3.156), changing delta gauge fixing to exponential gauge fixing. After eliminating the averaging constraints, its covariance is \((C^*\Delta^{(k)}C)^{-1}\). Thus the normalizer in (1.4) belongs to the constrained fluctuation construction, rather than an unspecified Dirichlet compression. The text following (2.12) identifies the remaining normalization with the identity-background integral; (2.13) defines the nonlinear logarithm separately. This narrows residual 1 but does not verify common periodization or all coordinate factors. Moreover, printed p.298 explicitly defers localized bounds for that nonlinear integral to the next paper. [CMP109](https://doi.org/10.1007/BF01215223).

## 6. Interface statement

**Assumed interfaces:** none. Sections 3–4 prove an independent analytic matrix theorem under (2.1)–(2.2).

**Proved:** the Gaussian comparison is proved for common periodized exponentially decaying kernels, with all constants independent of covering degree. Its sum over scales is proved under uniform kernel parameters. This strictly enlarges the class covered by the finite-range comparison lemma.

**Not proved:** (A3′), the full scalar dictionary, or I-0a′/I-0c. This note does not supply a proof of those interfaces.

**Interface correction for I-0c:** the generic exp[−c g_k^{-2}] large-field factor in the generic formulation is stronger than the exp[−p₀(g_k)] factor verified in LFR II (1.100). A proof must use the actual factor in each operation, or separately establish the stronger factor in the precise sector where it is claimed.

## 7. Exact residuals and next proof operations

1. **O, Gaussian dictionary.** At the identity background identify all determinant/Jacobian factors entering the *complete* scalar, including their constrained coordinate measures. For each whole-torus factor prove a common-kernel formula (2.2) with uniform (2.1), or prove an equally quantitative covering comparison directly from the localized random-walk expansion. For each finite-domain factor prove exact conjugacy under an injective lift. Uniform positivity alone supplies neither conclusion.
2. **O, scalar naturality.** Track the identity terms of the nonlinear and R activities through the actual localization and exponentiation recipe. Verify that every choice of graph, averaging, boundary data and denominator is copied on nonwinding carriers; record any genuinely global scalar separately. “Depends on U restricted to X” is insufficient.
3. **O, summable scalar tail.** Translate the primary-source activity estimates into the anchored carrier sum with the actual domain metric and polynomial localization radii. The geometric sum must use the slower rate consumed by the nonlinear operations. A pointwise activity bound is not itself the carrier sum.
4. **O, terminal lower bound dictionary.** Before using T6, match the scalar convention and χ_K in LFR II (0.1), and verify a fixed Haar ball at the prescribed terminal coupling g_K=g_*. A bound uniform over arbitrary terminal couplings tending to zero is a stronger assertion and is not obtained by simply dropping the Wilson-action factor.

The next productive step is item 1 using the identity-background operators in CMP95/96/99 and CMP109 (1.4)–(1.5). Items 2–3 require the complete recipe, not a new general determinant estimate.

## 8. Summary

This note addresses a specific gap in the Gaussian portion of the cross-torus reduction: the finite-range comparison lemma does not apply directly to an exponentially decaying constrained fluctuation matrix. The primary source supplies exponential decay and positivity, which are useful but different properties. The new theorem works directly with exponentially decaying matrix kernels and proves an exponentially small determinant-density error between a torus and its covers, provided both matrices are periodizations of one common kernel. Its proof uses a uniform complex strip for the matrix logarithm, Fourier coefficient decay and exact discrete Fourier sampling. The error is summable over all ultraviolet scales, with an explicit cutoff-independent bound.

The important remaining step is identifying the actual Gaussian factors with this class, including their constrained measures. The nonlinear and R scalar terms still require their own copying and carrier-summability checks. Their field locality cannot replace comparison of the scalar recipe. Therefore (A3′) remains open, and the conditional infinite-volume result remains conditional. These distinctions preserve the useful elementary copying reduction while keeping unsupported source identifications out of the observable arguments.
