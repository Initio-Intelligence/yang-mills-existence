# The actual tensor coefficient and its gauge, source, and regulator identities

**Scope:** The phase-averaged regular observable map at the actual frozen physical data. The actual matching is derived in T9/N9/U9, rather than assumed.

This module removes the old covariant regular action from the critical one-loop coefficient, decomposes the complete mean operator into its actual lattice symmetry channels, protects the pseudoscalar mean, and proves the magnetic-symbol and gauge/coarea identities needed for the actual Gaussian matching. The proof uses the physical current-link action and the actual constrained minimizing response; it does not assume that an intrinsic activity on its original fine lattice has a translation-invariant Hessian there. The companion U9 computes the continuum principal trace directly, and N9 combines it with the retained finite parts to close the regular mean-metric subgate. The full renormalized tensor point-family and historical obligations remain separate.

### 1. Physical current-link coordinates

At scale \(k\), write \(V\) for the links on the current lattice and \(U_k(V)\) for the source minimizing field on the original lattice. Let

\[
\widehat B_k(V)=B_k\bigl(U_k(V),J_k(V)\bigr),\qquad
\widehat S_k(V)=S\bigl(U_k(V)\bigr).
\tag{T9.1}
\]

Here \(B_k\) is the covariant fixed-domain reference identified in A8, and \(S\) is the leading Wilson action in its fixed source convention. Both functions in (T9.1) are gauge invariant and covariant under the current lattice translations and reflections. This follows for \(\widehat S_k\) from covariance of the minimizing orbit and for \(\widehat B_k\) from the same covariance at every frozen regular step. The source counterterms preserve these symmetries. It is not a statement of translation covariance of every individual localized coefficient.

The source minimizing-field and local-potential bounds imply exponentially summable current-link Hessian kernels at the flat configuration. All arguments below can first be applied to whole-lattice coefficient families, whose localized expansions have the stated summability. Finite compatible tori and smooth cutoff-affine directions are treated in §4.

Use bond-centered linear connection coordinates. For either action \(H=\widehat B_k\) or \(H=\widehat S_k\), constant color invariance gives

\[
DH(1)=0.
\tag{T9.2}
\]

Its quadratic Hessian has the translation-invariant convolution form \(K_H\). The linearized gauge identity gives
\(K_H(p)d(p)=0\), with the centered lattice gradient
\(d_\mu(p)=2i\sin(p_\mu/2)\), in the corresponding site/bond Fourier convention. Analyticity at zero and the expansion \(d(p)=ip+O(|p|^3)\) imply \(K_H(0)=0\): divide the identity along \(p=tv\) by \(t\), then let \(t\to0\), for every vector \(v\).

Full coordinate inversion sends a centered vector connection to its negative at the inverted bond. Its action on the two quadratic legs therefore has positive sign and yields \(K_H(-p)=K_H(p)\). Consequently

\[
K_H(0)=0,\qquad \partial_{p_\rho}K_H(0)=0.
\tag{T9.3}
\]

These are exact zeroth and first moment identities for its exponentially summable kernel. For every affine centered connection \(a_\mu(x)=a_\mu^0+M_{\mu\nu}x_\nu\),

\[
K_Ha=0.
\tag{T9.4}
\]

Indeed a convolution applied to an affine function is the zeroth moment times its value minus the first moment times its slope. Both moments vanish by (T9.3). The Ward identity also gives \(K_Hd\omega=0\) for every admissible linear gauge direction.

### 2. The actual constrained affine response

The background in the one-step fluctuation integral is not chosen arbitrarily on the current links. It is

\[
\overline V_k(V')=M_k\bigl(U_{k+1}(V')\bigr),
\tag{T9.5}
\]

which minimizes \(\widehat S_k(V)\) subject to the next coarse constraint. This follows by the nested constrained variational characterization: minimize the original Wilson action at fixed current average first, then minimize over that average with the next average prescribed. The source uniqueness of the minimizing orbit identifies the result with \(U_{k+1}\).

The flat differential \(Q_k\) of the source next-block average reproduces an affine connection with the required engineering rescaling. This can be checked directly from CMP109 (0.4), (0.11)–(0.12). The linearization of the group average is the arithmetic average of path integrals. For an affine connection, averaging over the permitted coordinate-order paths cancels their antisymmetric area discrepancies. In the coarse bond average, the remaining constant-curvature loop contribution is linear in the displacement of the fine path from the centered coarse bond. The average of these displacements over the centered block is zero. A gradient part is reproduced by endpoint covariance. Thus the appropriately scaled affine current connection has exactly the prescribed coarse affine average.

By (T9.4) for \(\widehat S_k\), this affine connection also satisfies the linear constrained Euler equation, with zero multiplier. The source positive quadratic form on \(\ker Q_k\) after removal of the residual gauge directions gives uniqueness of that constrained linear solution modulo gauge. Therefore the derivative of the **actual** minimizing response (T9.5), along a coarse affine curvature test \(u\mapsto V'(u)\), is

\[
\left.\partial_u\overline V_k(V'(u))\right|_{u=0}
=a_F+d\omega_F.
\tag{T9.6}
\]

This is an identity of linear connection coordinates, with the known scale factor included in \(a_F\). The axial gauge used by the source may create a block-dependent representative, but its difference from the affine solution is the displayed gauge direction. There is no physical block-periodic ripple left over in (T9.6). The uniqueness assertion is applied on the constrained fluctuation space; a zero-momentum inverse of the unconstrained Wilson Hessian is not used. On the whole lattice, the source exponentially decaying constrained inverse extends the same argument to affine polynomial data by localization and a limit.

### 3. The old-action score vanishes in the critical one-loop coefficient

Let \(\Xi_k(u,\tau A)\) be the actual current-link fluctuation chart in the one-step integral, after the source constraint has been linearized and the independent coordinates chosen. Its base value is \(\overline V_k(V'(u))\). Put

\[
C_k(u)A=\left.\partial_\tau\Xi_k(u,\tau A)\right|_{\tau=0},
\qquad
H'_{\mathrm{old},u}(A)
=D\widehat B_k\bigl(\overline V_k(V'(u))\bigr)[C_k(u)A].
\tag{T9.7}
\]

An overall sign from the exponent convention does not affect the cancellation. Background subtraction of \(\widehat B_k(\overline V_k)\) is independent of \(\tau\), so it does not alter (T9.7).

At the flat background, (T9.2) gives \(H'_{\mathrm{old},0}=0\). Differentiating in any affine curvature direction gives

\[
\begin{aligned}
\partial_u H'_{\mathrm{old},u}\big|_{0}
&=D^2\widehat B_k(1)[a_F+d\omega_F,C_k(0)A]
  +D\widehat B_k(1)[(\partial_uC_k)(0)A]\\
&=0.
\end{aligned}
\tag{T9.8}
\]

The first term vanishes by (T9.3)–(T9.6) and the Ward identity; the second vanishes by (T9.2). Thus no derivative of the source-dependent fluctuation inclusion has been discarded.

For every invariant intrinsic insertion \(f\), its amplitude derivative \(F'_{0,u}\) also vanishes at the flat background: the first differential of \(f\) at the flat pair is zero by constant color invariance. Therefore \(F'_{0,u}=O(u)\), while (T9.8) gives \(H'_{\mathrm{old},u}=O(u^2)\). The product has no background term of degree two. Taking its normalized Gaussian expectation does not change this conclusion, because the Gaussian law and its normalization are analytic in \(u\). Hence

\[
\boxed{
\Pi\,\mu_{0,u}\!\left(F'_{0,u}H'_{\mathrm{old},u}\right)=0.
}
\tag{T9.9}
\]

The identity also holds for mixed curvature directions: the calculation applies to an arbitrary linear combination of them and then polarization applies. The physical current has zero first variation on an affine curvature field, so the local physical jet agrees with the intrinsic independent-current test at the order used in (T9.8). An arbitrary second-order off-physical extension is not needed.

**Theorem T9-A.** On the whole-lattice regular coefficient family, the complete critical first-amplitude coefficient of every invariant insertion is independent of the old covariant additional action. In N8.14 one may omit its old-action score while retaining the classical cubic, gauge-fixing, Jacobian, and normalization responses:

\[
\mathfrak B_k f
=\frac{L^4}{2}\Pi\left[
\mu_{0,u}(F''_{0,u})
-2\mu_{0,u}\bigl(F'_{0,u}H'_{\mathrm{bare},u}\bigr)
\right]_{u=0}.
\tag{T9.10}
\]

Here \(H'_{\mathrm{bare}}\) contains every score except the old covariant additional action. The zero-amplitude Gaussian precision itself is independent of that additional action because its fluctuation difference begins at order \(\tau\). The classical forward graph \(S_k^0\) is also independent of it. Thus the **complete** first-order mean coefficient

\[
G_k^{\mathrm f}=A_k^1+B_k^1S_k^0
\tag{T9.11}
\]

is independent of the old covariant reference \(B_k\). The notation \(B_k^1\) in (T9.11) is the critical-from-stable linear block; it is distinct from the old action \(B_k\).

### 4. Scope of the cancellation

The proof concerns the full covariant current-link action. It does not require each polymer summand to annihilate affine fields. Nor does it extend the assertion to an arbitrary reset-grid action with spatially varying coefficients.

For the actual regular action, A8 identifies \(E_k+R_k=B_k+\delta_k\), with \(\delta_k\) arbitrarily rare in the common narrow chart. The contribution of \(\delta_k\) therefore remains in the already proved narrow-chart forcing estimates; it is not set to zero by (T9.9).

On a finite torus, an affine field is replaced by the smooth cutoff-affine test. Away from its plateau, (T9.4) no longer applies exactly. Exponential locality bounds that discrepancy by the existing large-support or finite-volume tail, with no original-fine-mesh inverse power. For the fixed-domain reference this uses its fixed-radius derivative bounds. It does not multiply an uncontrolled finite-volume error by the inverse of an old shrinking birth radius.

The cancellation removes a genuine potential dependence from the unresolved tensor coefficient. It does not supply a sign for that coefficient, identify it with a continuum anomalous dimension, or make the bare source constants uniform as \(L\to\infty\).

### 5. Remove the Gaussian cutoff with a controlled error

**Theorem T9-B.** Let \(\mathfrak B_k^D\) denote (T9.10) with the actual frozen cutoff and let \(\mathfrak B_k^\infty\) denote the same expression under the untruncated constrained Gaussian. On the fixed intrinsic mark norm, for every fixed \(Q\),

\[
\|\mathfrak B_k^D-\mathfrak B_k^\infty\|_{\mathrm{mark}\to\mathrm{crit}}
\le C_Q x_k^{-Q},\qquad
\|\mathfrak B_k^\infty\|_{\mathrm{mark}\to\mathrm{crit}}\le C.
\tag{T9.12}
\]

The constants are uniform in the microscopic depth and the admitted volume for the fixed source block parameter \(L\).

To prove this, expand the two background derivatives in (T9.10). They produce a fixed finite collection of connected Gaussian moments of localized polynomial insertions. Their degrees are bounded independently of depth: the amplitude derivatives of the mark have degrees one and two in \(A\), the first bare score has degree at most three, and each background derivative of the Gaussian law adds a quadratic insertion. Analytic source bounds control the coefficient kernels in the current coordinates.

Interpolate the actual Gaussian cutoff factors by the source connected cutoff expansion, CMP119 (3.32). A difference from the untruncated moment has at least one differentiated or missing cutoff factor. The corresponding Gaussian estimate has a boundary-tail factor \(p_k^m e^{-cp_k^2}\); the additional marked polynomials cost only fixed moments. The connected covariance bounds sum the supporting tree. Including the source \(MR_k\)-cell multiplicity and the marked norm gives

\[
\|\mathfrak B_k^D-\mathfrak B_k^\infty\|
\le Cp_k^mR_k^{m'}\exp[-cp_k^2+C_\kappa R_k^4]
\le C_Qx_k^{-Q}.
\tag{T9.13}
\]

The last inequality uses the actual fixed logarithmic exponents, including \(p_0\ge5r\), as in A8.45. This is a direct marked Gaussian moment calculation. It does not assume that the exponential of a positive quartic polynomial has an analytic complex neighborhood under an untruncated Gaussian. The normalized connected expansion also avoids estimating an inverse extensive partition function.

Combining T9-A and T9-B leaves a bare constrained Gaussian tensor coefficient, with all of its gauge, constraint, Jacobian, and minimizing-field responses retained. Old covariant actions and cutoff errors are no longer unidentified contributions to its sign.

The operator in (T9.10) is the coefficient for the original rooted operation before phase averaging. For a covariant density family define its mean coefficient explicitly by

\[
\overline{\mathfrak B}_k f
=L^{-4}\sum_{r\bmod L}\mathfrak B_k(T_rf).
\tag{T9.12a}
\]

The cutoff and uncut versions are denoted by superscripts \(D\) and \(\infty\). Equation (T9.12) also holds for this mean. Total-charge conservation below concerns (T9.12a); it does not make the individual phase coefficients vanish.

### 6. The actual lattice symmetry gives seven orthogonal channels

Let \(\mathcal E=\operatorname{Sym}^2(\Lambda^2\mathbb R^4)\), with the Frobenius inner product on symmetric \(6\times6\) matrices in the oriented two-form basis \(e_{ij}\), \(i<j\). The full signed-permutation group \(\mathcal H_4\), of order \(2^4 4!=384\), acts orthogonally by

\[
J\longmapsto (\Lambda^2R)J(\Lambda^2R)^T.
\tag{T9.14}
\]

The mean phase map is covariant under this group. One can use the centered set of phase representatives because \(L\) is odd. Equivalently, sum the original density family over a complete current cell before extracting its curvature coefficient. The complete source operation, the tensor seed, and the critical projection have this covariance. The classical graph \(S_k^0\) inherits it by its recurrence. Thus the **complete** mean coefficient, including stable feedback, commutes with (T9.14). This covariance is not asserted for an individual phase.

Here is its orthogonal decomposition:

| Sector | Dimension | Concrete realization |
|---|---:|---|
| Scalar | 1 | Multiples of \(I_6\) |
| Pseudoscalar | 1 | Multiples of the Hodge star \(*\) |
| Diagonal stress | 3 | \(J_{ij,ij}=h_i+h_j\), \(\sum_i h_i=0\) |
| Off-diagonal stress | 6 | The shared-index entries of the trace-free metric deformation |
| Diagonal Weyl | 2 | Diagonal matrices with \(\sum_{j\ne i}J_{ij,ij}=0\) for every \(i\) |
| Complementary Weyl | 2 | Complementary-pair entries orthogonal to \(*\) |
| Shared-index Weyl | 6 | Shared-index entries orthogonal to off-diagonal stress |

The two stress sectors combine to the nine-dimensional continuum stress representation. The last three sectors combine to its ten-dimensional Weyl complement. Lattice symmetry alone does not force equality of the eigenvalues within either combination.

For completeness, explicit projectors require only small sums. For the diagonal entries \(d_{ij}=J_{ij,ij}\), define

\[
D=\sum_{i<j}d_{ij},\quad
r_i=\sum_{j\ne i}d_{ij},\quad
c=D/6,\quad h_i=\tfrac12(r_i-D/2).
\tag{T9.15}
\]

The scalar projection is \(cI_6\); the diagonal stress projection has entries \(h_i+h_j\); their subtraction leaves the diagonal Weyl sector. For the complementary pairs, put

\[
b=(J_{12,34},-J_{13,24},J_{14,23}).
\tag{T9.16}
\]

Its mean component gives the pseudoscalar and its mean-zero part gives the complementary Weyl sector. Finally, for fixed \(j<k\), let \(a,b\) be the two remaining coordinate indices and use oriented entries
\(u_a=J_{aj,ak}\), \(u_b=J_{bj,bk}\).
Their average gives the off-diagonal stress entry and their difference gives the shared-index Weyl entry. Antisymmetry of each two-form index supplies the signs when these are written in the \(i<j\) basis.

These seven representations are irreducible and pairwise inequivalent. One direct proof uses the normal subgroup of coordinate sign flips. The diagonal sector has the trivial sign character and is the permutation representation of \(S_4\) on its six unordered pairs; it splits as dimensions \(1,3,2\). The complementary sector has the product of all four signs; its three matchings split into the determinant character and a two-dimensional representation. The shared sector has the six distinct characters \(\epsilon_j\epsilon_k\). For each such character its stabilizer exchanges the two remaining shared indices, giving the symmetric and antisymmetric one-dimensional fibers. Induction over the six characters gives two inequivalent irreducible representations of dimension six. The distinct sign characters separate these cases.

Let \(P_\lambda\) be the seven orthogonal projectors. Since the actual coefficient is real, the multiplicity-one decomposition gives

\[
\boxed{
G_k^{\mathrm f}=\sum_{\lambda}\gamma_{\lambda,k}P_\lambda,
\qquad \gamma_{\lambda,k}\in\mathbb R.
}
\tag{T9.17}
\]

In particular it is selfadjoint in one fixed Frobenius metric, and all these mean coefficients commute across scales. This rules out a nonnormal or Jordan-block obstruction for the covariant mean coefficient. It does not remove phasewise anisotropic noise.

The coefficients have the exact directional formulas

\[
\gamma_{\lambda,k}
=\frac{1}{d_\lambda}\operatorname{Tr}_{\mathcal E}(P_\lambda G_k^{\mathrm f})
=\frac{\langle J_\lambda,G_k^{\mathrm f}J_\lambda\rangle}
       {\|J_\lambda\|^2}
\quad(0\ne J_\lambda\in\operatorname{ran}P_\lambda).
\tag{T9.18}
\]

The same decomposition applies to the backward mean coordinate and to its bounded coordinate change in N8.20a. The exact rational verification script the exact finite computation checks the seven projector covariances for all 384 group elements. It obtains dimensions \((1,1,3,6,2,2,6)\) and character Gram matrix \(I_7\). The representation proof above explains those finite checks.

**Theorem T9-C.** Within the whole-lattice covariant regular family, the mean metric issue reduces to seven real coefficients in a fixed orthogonal decomposition. The scalar coefficient is already neutral by N8.28–N8.38. The next section controls the pseudoscalar coefficient. Five actual tensor coefficients then remain to be signed or otherwise controlled.

### 7. A protected geometric pseudoscalar

#### 7.1 An admitted local charge density

Use Lüscher, *Topology of Lattice Gauge Fields*, CMP85 (1982), 39–48. Its §3 constructs a cellwise bundle cocycle from axial cell loops using group products and real powers of matrices. Its §4, equation (32), gives a gauge-invariant density depending only on the links of one cell; the total is invariant under admissible continuous deformations, and (34)–(36) give its Pontryagin curvature jet.

The directly stated construction is for \(SU(2)\). The admissible-cell version needed here extends as follows. Fix a faithful unitary representation of the compact simple group. On a sufficiently small neighborhood of the identity set \(u^t=\exp(t\log u)\), using the principal matrix logarithm. These powers remain in the group for real group-valued \(u\). They obey \(u^0=1,u^1=u\), inversion compatibility, and conjugation covariance. Lüscher's footnote 6 explicitly identifies these as the only power identities used in the cocycle proof. The same products therefore define a group-valued cell cocycle. Its associated unitary vector bundle has a second Chern character, and the trace formula of §4 computes it. For a simple group the representation trace form is a positive multiple of the fixed invariant form. Divide by that constant to give the desired curvature normalization. The total may then lie in a fixed rescaled integer lattice; deformation invariance is unchanged. No assertion about exceptional configurations outside the small-plaquette neighborhood is needed.

There is also a uniform analytic bound in the present variables. On a microscopic cell of spacing \(\xi\), every axial loop appearing in the construction is a product of a fixed number of plaquettes. On the intrinsic source domain it differs from the identity by at most \(C\xi^2 b\). All principal powers, inverses, and products in the finite cell formula are holomorphic on one fixed complex neighborhood of these loop variables. Its constant term is zero, and its linear term is zero by constant color invariance. Hence its density \(q_{\mathrm{geo},\xi}\) satisfies

\[
\sup_{\mathscr D(b)}|q_{\mathrm{geo},\xi}|
\le C\xi^4 b^2,
\qquad
\|\xi^{-4}q_{\mathrm{geo},\xi}\|_{\mathrm{mark},b}\le C.
\tag{T9.19}
\]

This is a finite-cell principal-power estimate; it does not use a product ball of radius \(O(\xi^2)\) as the norm on arbitrary link fluctuations. Cell-loop control comes from the normalized intrinsic connection domain. Covariance glues the local formulas across its gauge charts.

Average this density over the finite lattice symmetry group with its determinant character, translating the cell root consistently. Denote the result by \(q_{\mathrm{top}}\). It is an exact pseudoscalar, still local and analytic, and its total is still constant on admissible paths. Even without choosing a symmetry convention for the original geometric charge, each summand has that invariance. Its curvature jet is the normalized Hodge-star direction:

\[
\Pi q_{\mathrm{top}}=*,\qquad
\Pi(q_{\mathrm{clover,ps}}-q_{\mathrm{top}})=0.
\tag{T9.20}
\]

#### 7.2 Nonzero-charge tests belong to the actual source domain

Charge conservation in the contractible flat chart alone would not imply (T9.20) is protected. To test its coefficient, use an actual admissible nonzero-charge family.

Choose a nonzero integral Cartan element \(H\), so \(\exp(2\pi H)=1\), in an anti-Hermitian convention. On a periodic torus of side \(R\), take commuting quantized fluxes

\[
F_{12}=2\pi mR^{-2}H,\qquad
F_{34}=2\pi nR^{-2}H,
\qquad mn\ne0,
\tag{T9.21}
\]

with all other components zero. Standard periodic link representatives use transition links at the torus seams. Their plaquette products are the indicated constant commuting matrices at every plaquette. The transition links need not be close to the identity globally.

The Wilson current of this configuration is exactly zero. Each positive plaquette contribution is paired with the opposite adjacent plaquette, and transport does not alter it because the links and fluxes commute. Its first variation therefore vanishes in every link direction. For \(R\) large, its plaquettes meet all of the source smallness conditions. On every fixed local patch a gauge has the affine connection of (T9.21), with norm bounded by \(CR^{-2}\) times the patch radius.

This is precisely the type of nonflat reference permitted by the source. CMP102 (2), (7), and Theorem 1, printed pp.278–279, require plaquette/current regularity and small coarse plaquettes, not globally small links. CMP109 (1.1), printed p.260, repeats the existence and uniqueness of the regular minimizing orbit for every such coarse field. Its analytic-domain definition (1.11)–(1.16) requires gauges only on fixed local cubes.

The centered source averages preserve the constant Abelian flux, with its appropriate scaling: the commuting path logarithms add linearly and their centered area offsets average to zero. The flux field is already a constrained critical configuration, since its full Wilson current vanishes. The source uniqueness of the regular critical orbit therefore identifies it, up to gauge, with the minimizing field at each relevant scale. Its nested minimizing-domain conditions follow at the same time. Thus these tests lie in the actual physical nonflat source atlas; no extension from a globally small-link chart is being assumed.

Their normalized Chern integral is a fixed nonzero number, proportional to \(mn\operatorname{Tr}(H^2)\), independent of \(R\). Lüscher's classical expansion, applied after scaling the torus to unit size, gives the same nonzero limit for the geometric lattice charge. The representation extension above has the same conclusion. It suffices that this number is nonzero; a charge-one instanton is not required.

#### 7.3 Exact regular-fiber conservation fixes the coefficient

The real regular fluctuation domain is contracted by \(A\mapsto tA\), \(0\le t\le1\). The physical minimizing/constraint map along this path remains inside the admissible small-plaquette neighborhood, by the source normalized regularity bound and \(g_kr_{\chi,k}\ll1\). Consequently the total geometric charge of the physical fine configuration is constant on each such fiber. It follows under the **actual normalized kernel**, with any admitted covariant old potential, that

\[
Q_k\!\left[\sum_xq_{\mathrm{top},k}^{\mathrm{cl}}(x)\right]
=\sum_yq_{\mathrm{top},k+1}^{\mathrm{cl}}(y).
\tag{T9.22}
\]

Here \(q_{\mathrm{top},k}^{\mathrm{cl}}(z)\) is the sum of the original fine-cell geometric charges whose fine roots lie in the centered current cell at \(z\), evaluated on \(U_k(V)\). Every fine cell is assigned once. A fine cell contributes \(\xi_k^4\) times its normalized density, and a current cell contains \(\xi_k^{-4}\) fine roots; their factors cancel in its leading curvature coefficient. Thus \(\Pi q_{\mathrm{top},k}^{\mathrm{cl}}=*\), and the next classical lift is the actual mean-density classical recursion \(\mathcal C_k\). The sums in (T9.22) denote the same extensive charge, with no additional engineering factor. Equation (T9.22) uses no invariance of an artificial integration domain under a gauge change.

Let \(h_k\) be the covariant mean density obtained by subtracting the classical output from the left side of (T9.22), before summing over roots. It is an intrinsic local analytic pseudoscalar with an exponentially summable coefficient family, and
\(\sum_yh_k(y)=0\) on every admitted physical background. By the one-dimensional pseudoscalar sector, its leading curvature jet is \(c_k*\).

Evaluate it on (T9.21). The local polynomial-jet estimate used in A7 applies on patches of radius small compared with \(R\), while the remaining supports are bounded by their exponential tail. Gauge invariance removes the lower jets and identifies the quadratic term with the curvature coefficient. Thus its density is \(c_k\) times the Pontryagin density plus a remainder whose sum tends to zero as \(R\to\infty\). More explicitly, fixing \(k\), choose a support cutoff \(\ell_R=C\log R\). The omitted tail summed over \(O(R^4)\) roots is \(O(R^4e^{-c\ell_R})\). On each remaining support, the commuting constant-flux field has an exact affine local gauge, with normalized connection \(O(R^{-2}\ell_R)\) and physical current zero. The cubic Taylor remainder is \(O(R^{-6})\) times a fixed polynomial in \(\ell_R\); after summing it is \(o(1)\). The compatible finite-volume versus whole-lattice localization error has the same vanishing tail property.

Since the total in (T9.22) is zero and the test has nonzero limiting charge, \(c_k=0\). Therefore

\[
\boxed{
\Pi\overline L_k q_{\mathrm{top},k}^{\mathrm{cl}}
=\Pi\mathcal C_kq_{\mathrm{top},k}^{\mathrm{cl}}=*,
\qquad
\overline{\mathfrak B}_k^Dq_{\mathrm{top},k}^{\mathrm{cl}}=0.
}
\tag{T9.23}
\]

The first equality is exact for the whole-lattice regular mean coefficient family. On a finite torus the global charge identity is exact, while the chosen local cutoff-affine projection retains the previously proved exponential finite-volume tails. The second equality follows by differentiating the even amplitude family; charge constancy holds for every sufficiently small real amplitude, independently of the weight assigned to the fiber. The cutoff is retained throughout this proof. The uncut coefficient has only the already controlled difference (T9.12).

#### 7.4 Transfer to the specified clover pseudoscalar

The prescribed microscopic pseudoscalar and the geometric one have the same curvature jet by (T9.20). Their classical mean difference therefore lies in the stable sector. A7's classical contraction, applied after the fixed block grouping if necessary, gives

\[
\|q_{\mathrm{clover,ps},k}^{\mathrm{cl}}
-q_{\mathrm{top},k}^{\mathrm{cl}}\|_{\mathrm{mark},b}
\le C\vartheta^k,\qquad 0<\vartheta<1.
\tag{T9.24}
\]

In the same classical forward coordinate used by N8.17–N8.18, the complete first coefficient is the application of \(\overline{\mathfrak B}_k\) to this classical family. Equations (T9.12), (T9.23), and (T9.24) imply

\[
|\gamma_{\mathrm{ps},k}|
\le C\vartheta^k+C_Qx_k^{-Q}.
\tag{T9.25}
\]

In particular this is a statement about the specified source family with its stable descendants, not only an arbitrarily selected pseudoscalar representative.

Write \(t_k=g_k^2=x_k^{-1}\) and retain the N8 remainder \(O(t_k^2+t_k\varepsilon_k)\), where \(\varepsilon_k=Cg_kr_{\chi,k}\). The pseudoscalar multiplier satisfies

\[
E_{\mathrm{ps},k}^{\mathrm f}
=1+t_k\gamma_{\mathrm{ps},k}
\quad+O(t_k^2+t_k\varepsilon_k).
\tag{T9.26}
\]

The AF scale bounds make the error series summable. To check the additional geometric series uniformly, split at \(n=\lfloor x_0/(2c_+)\rfloor\), where \(c_+\) bounds \(x_k-x_{k+1}\). Before this index \(x_k\ge x_0/2\). After it, use \(x_k\ge x_*\) and the geometric tail \(\vartheta^n\). Both parts give
\(\sum_kt_k\vartheta^k\le C/x_0\); if the horizon ends before \(n\), the second part is absent. Also \(\sum_k t_k^2\le C/x_K\), and \(\sum_k t_k\varepsilon_k\le Cx_K^{-1/2}(1+\log x_K)^{p_0}\). At a sufficiently weak endpoint every factor is separated from zero and the sum of its absolute logarithmic changes is uniformly bounded. Hence

\[
0<c\le
\left|\prod_{k<K}E_{\mathrm{ps},k}^{\mathrm f}\right|
\le C<\infty
\tag{T9.27}
\]

uniformly in the ultraviolet horizon at the chosen weak endpoint. The inverse product has the same bound. N8.20a transfers this conclusion to the backward mean coordinate. Regular noncovariant corrections use A8's identified rare forcing bounds.

**Theorem T9-D.** The pseudoscalar mean normalization is bounded for the actual clover source in the regular family. The proof uses an admitted geometric representative to establish protection, then transfers it through the actual classical stable graph. It does not control phasewise scalar-to-pseudoscalar noise or extend charge conservation through large-field reset/history operations.

### 8. An explicit metric from five cumulative bounds

The equivariance argument in §6 applies to the exact mean critical maps, with their full equivariant forward or backward graphs. Thus

\[
E_k=\sum_\lambda e_{\lambda,k}P_\lambda.
\tag{T9.28}
\]

Suppose, for the five remaining tensor sectors, one proves the real scalar bounds

\[
\sup_{0\le a\le b\le K}
\left|\prod_{i=a}^{b-1}e_{\lambda,i}\right|\le C.
\tag{T9.29}
\]

The scalar and pseudoscalar sectors already have these interval bounds from their absolutely summable logarithmic corrections. Define

\[
h_{\lambda,k}
=\max_{k\le b\le K}
  \left|\prod_{i=k}^{b-1}e_{\lambda,i}\right|^2,
\qquad
H_k=\sum_\lambda h_{\lambda,k}P_\lambda.
\tag{T9.30}
\]

Then \(I\le H_k\le C^2I\), and
\(h_{\lambda,k}=\max(1,|e_{\lambda,k}|^2h_{\lambda,k+1})\) gives
\(E_k^*H_{k+1}E_k\le H_k\) exactly. This supplies the metric required by S8-C without an additional Lyapunov construction. It may depend on the finite horizon, but its equivalence constants do not.

With N8's summable remainder, it suffices to bound the upper interval sums
\(\sum_{i=a}^{b-1}t_i\gamma_{\lambda,i}\) uniformly. Pointwise negativity is one sufficient method; a bounded weighted coboundary is another. The remaining mean problem is therefore five real cumulative growth bounds, not an arbitrary 21-dimensional nonnormal matrix problem.

The actual bounded-coboundary argument is now supplied by N9.19–N9.28, using the U9 principal trace and T9-E/F below. Thus all five bounds in (T9.29) are established for the admitted covariant regular family. Equation (T9.30) applies to that family, not merely to a hypothetical matrix sequence.

### 9. Uniform tensor sources are stationary on Cartan fluxes

There is a further exact reduction of the remaining coefficient. Let

\[
\mathcal H_J(U)=\sum_x\langle J,Q^W(x;U)\rangle
\tag{T9.31}
\]

with its prescribed physical cell-volume factor understood, so its critical density coefficient is \(J\). This is the actual Wilson/clover family, not a replacement continuum operator.

On a constant commuting flux field, each clover curvature is a constant matrix in the same Cartan subalgebra: in Hermitian conventions it is proportional to \(\pi_0\sin(\xi^2F_{\mu\nu})\). Its first variation in (T9.31) is a sum of traces of constant commuting coefficients times the variations of based plaquette loops. An off-Cartan variation has zero trace against these coefficients. For a Cartan variation the plaquette derivative is its oriented lattice curl; summing over roots cancels every bond contribution with the adjacent plaquette contribution. Equivalently it is a covariant divergence of a constant commuting coefficient. The added scalar Wilson correction in \(Q^W\) has the same cancellation. Hence, for every real symmetric tensor \(J\),

\[
D\mathcal H_J(U_F)=0.
\tag{T9.32}
\]

This statement is exact at finite spacing. It is not based only on the leading continuum form of the clover mark. Differentiating a transported based loop also produces parallel-transport commutators; their traces vanish because the background loop factors and their coefficients commute.

The actual classical current action is \(\mathcal H_{J,k}^{\mathrm{cl}}(V)=\mathcal H_J(U_k(V))\), with the same density reassignment as before. The chain rule and (T9.32) show that it too is stationary on the corresponding constant-flux background. Therefore the \(F'_0H'_0\) term of N8.14 vanishes on every such test for the **uniform tensor action**, including its full classical stable descendants.

Let \(M_{J,k}(F)\) be the constrained Hessian of this current action in the independent fluctuation coordinates and let \(C_k(F)\) be the actual uncut Gaussian covariance in those coordinates. The complete mean coefficient is consequently the curvature coefficient of

\[
\boxed{
G_k^{\mathrm f}J
=\Pi_{\mathrm{bulk}}\left[
\frac{1}{2\,\operatorname{Vol}_{k+1}}
\operatorname{Tr}\bigl(C_k(F)M_{J,k}(F)\bigr)
\right]+\mathcal E_{k,J}^{\mathrm{cut}},
\qquad
\|\mathcal E_{k,J}^{\mathrm{cut}}\|\le C_Qx_k^{-Q}\|J\|.
}
\tag{T9.33}
\]

The fixed normalization factors are those of N8.14 and (T9.31); \(\operatorname{Vol}_{k+1}\) counts output current cells, so the four-dimensional density factor is included once. The operation \(\Pi_{\mathrm{bulk}}\) extracts the local curvature coefficient of this compatible trace density. It can be determined by the large-torus quantized-flux tests. It is not differentiation between distinct topological sectors on a fixed finite torus. Allowing all six integer Cartan fluxes determines every quadratic form on \(\Lambda^2\) by polarization.

The Hessian in (T9.33) is the Hessian of the actual classical action mark after constrained minimization, not merely its direct plaquette second derivative with the minimizing response omitted. At these backgrounds the source-dependent base field does not move: it is stationary for \(S+\lambda\mathcal H_J\) for every sufficiently small \(\lambda\). The first-order constrained envelope identity identifies the derivative of the retained action with \(\mathcal H_J\circ U_k\). Terms differentiating the minimizing inclusion in its quadratic form pair a constraint-preserving variation with the constrained Euler multiplier and vanish. This is the usual Schur-complement derivative, with all of its cross terms included.

The uncut trace is also independent of the residual-gauge fixing parameter. The constrained Hessian \(M_{J,k}\) kills the residual gauge generator \(K\), by (T9.32) and gauge invariance. Writing \(A=b+K\omega\) with \(Tb=0\), \(TK=I\), separates the Gaussian into its physical quadratic form in \(b\) and its gauge quadratic form in \(\omega\). The mark quadratic form depends only on \(b\). The coordinate Jacobian and the gauge Gaussian normalization cancel in its normalized expectation. Therefore the uncut expression equals the trace on the physical quotient,

\[
\operatorname{Tr}(C_kM_{J,k})
=\operatorname{Tr}_{\mathrm{phys}}
  \bigl((M_{W,k}|_{\mathrm{phys}})^{-1}
             (M_{J,k}|_{\mathrm{phys}})\bigr).
\tag{T9.34}
\]

The fixed-cutoff difference is already included in (T9.33). A convenient gauge can thus be used to compute the uncut mean trace, provided it parametrizes the same constrained physical quotient and the normalization is retained.

### 10. Actual magnetic-symbol bounds for the retained remainder

This section proves the specific irrelevant-symbol bounds used in a fixed-\(L\) Gaussian matching argument. It does not claim that a formal magnetic symbol is an ordinary Fourier diagonalization at nonzero curvature.

Let \(s_k\) be the current density of the leading classical retained action and let \(h_{J,k}\) be the classical current density of (T9.31). With the same fixed local critical embedding \(\iota_k\) as the source norm, define

\[
r_k=s_k-\iota_k\Pi s_k,\qquad
r_{J,k}=h_{J,k}-\iota_kJ.
\tag{T9.35}
\]

The leading scalar normalization \(\Pi s_k\) is the fixed multiple of \(I_6\) dictated by the Wilson convention. It is not silently changed to the normalization of \(q_W=2S\). Affine reproduction preserves it exactly. The classical marginal-to-stable descendant is bounded, while the stable classical map contracts after the fixed grouping. Therefore

\[
\Pi r_k=\Pi r_{J,k}=0,\qquad
\|r_k\|_{\mathrm{mark},b}\le C,
\qquad
\|r_{J,k}\|_{\mathrm{mark},b}\le C\|J\|.
\tag{T9.36}
\]

These are actual current-density statements. They include the full classical source shape. A finite nonlinear family of anisotropically deformed actions is not needed: the constrained envelope identity identifies \(h_{J,k}\) as its derivative at zero source, and the linear family (T9.36) supplies the required bound on that derivative.

#### 10.1 Midpoint convention and uniform finite jets

Work first on the whole current lattice. On a constant commuting background \(F\), the Hessian kernel of a covariant density is equivariant under magnetic translations. Identify its two adjoint fibers by background parallel transport along the straight segment between the two bond midpoints. Removing that phase defines the midpoint kernel \(K_r(F;z)\), where \(z\) is the midpoint displacement. The straight segment is only a convention for identifying fibers in this symbol; it does not change any lattice averaging or physical action. The symbol is

\[
\Delta_r(F,p)=\sum_z e^{-ip\cdot z}K_r(F;z).
\tag{T9.37}
\]

Equivalently, choose affine radial gauge centered at the midpoint of each pair before differentiating. In that gauge the straight transport along the pair segment is the identity. This convention retains the magnetic phases that reappear when two such kernels are composed.

The localized intrinsic norm and the actual minimizing response give uniform exponentially summable Hessian kernels. Differentiating in a constant-curvature direction uses an affine connection on each finite support and costs a fixed polynomial in its diameter. The same is true of the finite number of momentum moments needed below. The unused spatial reserve pays these factors.

The passage to current-link derivatives uses more than the abstract intrinsic supremum. Compose each localized coefficient with the actual current-to-fine minimizing response and its current component from A7.12–A7.18. That response is holomorphic on one fixed ball of current-link perturbations and has uniformly localized coefficients, independently of \(\xi_k\). A unit perturbation at either of two current bonds has a bounded normalized fine response. Two Cauchy derivatives in those perturbations therefore have a fixed cost; localization forces their connecting support into the same exponentially weighted tree. Two further curvature derivatives use the affine current perturbation on that support and cost at most a fixed diameter polynomial. The additional momentum moments cost another fixed diameter polynomial. The unused tree reserve absorbs their product. In particular this argument supplies all fourth current derivatives and all finite momentum moments actually used in N9.14–N9.18. It does not assume that a raw fine-link product ball has a mesh-independent radius.

Consequently, for \(|\alpha|\le2\) and the required finite set of \(\nu\),

\[
\sum_z(1+|z|)^{|\nu|}
 \|\partial_F^\alpha K_r(0;z)\|
\le C_{\alpha,\nu}\|r\|_{\mathrm{mark},b}.
\tag{T9.38}
\]

This establishes uniform finite Taylor jets. It does not require a constant imaginary magnetic field to lie in one global bounded-relative-connection chart on every support size.

#### 10.2 Weighted Taylor cancellations

Assign weight one to a connection or a momentum and weight two to a curvature. The polynomial gauge-normalization argument of A7 gives, for a zero-critical-jet density and every fixed smooth local connection \(A\),

\[
r[\lambda A(\lambda\cdot)]=O(\lambda^{4+\beta})\|r\|,
\qquad \beta>0.
\tag{T9.39}
\]

The estimate is uniform for \(A\) in a fixed bounded smooth family. Here the critical cancellation is that of the full covariant root-density family, after its localized coefficients have been summed; it is not a zero-critical-jet assertion for every polymer term. One may take a geometric sequence \(\lambda=L^{-n}\); that already determines the vanishing finite Taylor coefficients. Local source analyticity and the exponential support reserve justify the absolutely convergent sums of vertices and momentum moments before coefficient extraction. In particular, introduce two fluctuation parameters into
\(A(x)=a_F(x)+\epsilon a e^{ip\cdot x}+\epsilon' b e^{iq\cdot x}\).
Cauchy in \(\epsilon,\epsilon'\) shows that the quadratic fluctuation vertex has no weighted term of total action degree at most four. Its two fluctuation legs have total weight two, so its Hessian symbol has no term of weighted degree at most two.

Sum the localized vertices of that full covariant family and their finitely many moments first. The gauge scaling and the vanishing total critical projection then remove their low weighted Taylor coefficients. No cancellation is imposed separately on a polymer summand. Moving this summed vertex to the midpoint convention introduces parallel-transport phases whose first curvature contribution has weight two. Such phases cannot create a missing lower-weight term; their low-weight contributions multiply the lower coefficients already shown to vanish. Thus the conclusion applies to the actual symbol (T9.37), including its covariant phase terms.

Coordinate inversion fixes the Cartan curvature, sends \(p\) to \(-p\), and changes the signs of both fluctuation-vector legs. Every constant tensor \(J\) is even under this inversion, so both \(r_k\) and \(r_{J,k}\) satisfy
\(\Delta_r(F,-p)=\Delta_r(F,p)\).
It eliminates the remaining odd weighted degree three. The moment bounds (T9.38) now give

\[
\boxed{
\|\Delta_r(0,p)\|\le C\|r\|\,|p|^4,
\quad
\|\partial_F\Delta_r(0,p)\|\le C\|r\|\,|p|^2,
\quad
\|\partial_F^2\Delta_r(0,p)\|\le C\|r\|,
\qquad |p|\le p_0.
}
\tag{T9.40}
\]

Mixed curvature derivatives satisfy the same bound. For \(r_{J,k}\), every right side is multiplied by \(\|J\|\). The constants are uniform in the microscopic depth at the chosen fixed \(L\). All required first source derivatives are therefore covered.

**Theorem T9-E.** The actual retained classical remainders and the actual uniform-source derivative remainders satisfy the magnetic weighted bounds (T9.40). The comparison with the continuum dimension-four reference has the same weights for the explicit current Wilson/clover discretization error, by its centered small-loop expansion. A coarse infrared penalty, or an independently chosen gauge-fixing operator, is not included in \(r\); its symbol and normalization must be treated explicitly in the Gaussian determinant calculation.

The bounds are the precise input needed to make the curvature coefficient of a one-loop remainder integrable after the covariant inverse and product expansion. Proving that last expansion, and the determinant/Schur matching with its actual normalization, is a separate calculation. A generic norm estimate is not substituted for it here.

### 11. The continuum dimension-four color factor

The continuum target can be stated for a fixed compact simple group without using a large-\(N\) extrapolation of a long operator chain. This statement concerns the continuum one-loop physical bilinears; it does not assign values to the finite lattice coefficients in (T9.18).

Choose an orthonormal Lie-algebra basis for the fixed invariant form and write

\[
[T^a,T^b]=if^{abc}T^c,\qquad
f^{acd}f^{bcd}=C_A\delta^{ab}.
\tag{T9.41}
\]

At order \(g^2\), the two-external-adjoint coefficient of a curvature bilinear has exactly two structure constants. The possible contributions are exhausted by the following expansion of the operator and the action:

| Contribution | Source of the two structure constants |
|---|---|
| Quartic part of the insertion | Its two commutator curvatures |
| Cubic insertion with a cubic action vertex | One from each vertex |
| Quadratic insertion with two cubic action vertices | One from each action vertex |
| Quadratic insertion with a quartic action vertex | The two commutators in that vertex |
| Gluon or ghost external-leg/normalization contribution | The usual two adjoint cubic couplings, or the quartic gluon contraction |
| Gauge/BRST or equation-of-motion mixing needed in an off-shell calculation | The same adjoint contractions; no additional invariant tensor is introduced |

After Wick contraction, every connected two-external-color tensor in this list is zero or a numerical multiple of \(f^{acd}f^{bcd}\). A contraction of two indices on one antisymmetric structure constant vanishes. Disconnected vacuum factors cancel from the normalized insertion. Thus the color dependence of the physical one-loop mixing matrix is exactly \(C_A\), and the remaining coefficients are independent of the group.

There is no independent double-trace dimension-four bilinear: each putative factor \(\operatorname{Tr}F\) is zero for a simple Lie algebra. There is also no gauge-invariant equation-of-motion bilinear of dimension four outside the curvature family. Off-shell gauge-variant equation-of-motion and BRST-exact terms must still be treated in that calculation; they do not change the physical curvature coefficient, and the constant Cartan tests used here have physical current zero. None of these observations removes such terms before the relevant Ward identities are applied.

For \(SU(N)\), (T9.41) gives \(C_A=N\) in the usual canonical convention. Since every dimension-four one-loop diagram already has this exact color factor, a contribution suppressed by an additional power of \(1/N\) cannot be hidden in this two-field physical sector. The color-stripped dimension-four coefficients stated by Ferretti, Heise, and Zarembo, hep-th/0404187v3, equations (6)–(7), therefore give

\[
\gamma_{\mathrm{scalar}}^{\mathrm{can}}
=\gamma_{\mathrm{ps}}^{\mathrm{can}}
=-\frac{11C_Ag^2}{24\pi^2},\qquad
\gamma_{\mathrm{stress}}^{\mathrm{can}}=0,\qquad
\gamma_{\mathrm{Weyl}}^{\mathrm{can}}
=\frac{7C_Ag^2}{24\pi^2}.
\tag{T9.42}
\]

This extension is the color-contraction argument above, not an assertion that the entire large-\(N\) spin-chain result extends to arbitrary operator length or to theories with matter. It also does not imply that every finite lattice matching term has only this color dependence: irrelevant terms in a chosen Wilson representation can affect finite parts.

In the canonical convention of that paper, bare-to-coarse transport uses the inverse operator renormalization. Passing to geometric curvature \(F_{\mathrm{geom}}=gF_{\mathrm{can}}\) contributes one additional coupling-ratio power. In units of the one-loop coefficient \(11C_A/(24\pi^2)\), the geometric transport damping exponents are consequently

\[
0\quad\text{(scalar and pseudoscalar)},\qquad
1\quad\text{(stress)},\qquad
18/11\quad\text{(Weyl)}.
\tag{T9.43}
\]

These signs were the continuum matching target. U9 now derives the same principal coefficients directly from the ordered tensor-source Hessian and the magnetic Gaussian inverse, including the finite-group color trace. The finite lattice stress and Weyl sectors still split as in §6, and their actual coefficients are defined by (T9.33). N9's determinant/finite-part identity puts the direct U9 result in the same frozen normalization and controls the scheme-dependent endpoint difference. Thus the actual mean conclusion no longer depends on importing (T9.42) from the quoted continuum calculation.

### 12. Gauge-coherent Schur factorization and the infrared regulator

This section supplies the measure and gauge identification needed to compare the actual one-step trace with retained Gaussian determinants. Every source derivative below is evaluated at zero source. Finite curvature jets are taken at zero curvature with a positive mass in place; the mass is sent to zero afterwards. No positivity assertion is made about an unconstrained nonabelian constant-magnetic-field Hessian at arbitrarily small mass.

#### 12.1 The quotient and its volume forms are independent of the source

Fix a constant Cartan background, a finite compatible torus, and the tensor perturbation \(S+\lambda\mathcal H_J\). Equation (T9.32) implies that its prescribed constrained base field is independent of \(\lambda\). The local implicit-function construction of the constrained critical orbit identifies this stationary field for sufficiently small \(\lambda\). Thus the differential of the original blocking map, the fine and coarse infinitesimal gauge actions, and all coordinate choices made from those fields are independent of \(\lambda\).

Let \(V_f,V_c\) be the fine and coarse tangent spaces, let \(\mathcal G_f,\mathcal G_c\) be their gauge tangent subspaces, and give the quotient spaces their orthogonal quotient metrics in a fixed bond-coordinate convention. Write \(P_f,P_c\) for the corresponding projections. Gauge covariance of the actual block map implies

\[
Q\mathcal G_f\subset\mathcal G_c,\qquad
\overline Q=P_cQP_f:V_f/\mathcal G_f\longrightarrow V_c/\mathcal G_c.
\tag{T9.44}
\]

This quotient map is onto. Indeed, the source constraint coordinates give surjectivity of the full tangent block map. For a coarse physical vector \(w\), choose \(v\) with \(Qv=w\); then \(P_cQP_fv=w\), because the removed fine gauge part maps to coarse gauge. Global gauge stabilizers are removed from the gauge parameter space, and physical harmonic modes are regulated by the positive mass. These conventions do not depend on \(\lambda\).

Let \(M(\lambda)\) be the physical fine Hessian. Choose, once and independently of \(\lambda\), an inclusion \(I\) of \(\ker\overline Q\) and a right inverse \(R\) of \(\overline Q\). In the coordinates \(v=Ia+Rw\), its matrix and its retained Schur complement are

\[
\mathcal C^*M\mathcal C=
\begin{pmatrix}A&B\\B^*&D\end{pmatrix},\qquad
M'=D-B^*A^{-1}B,\qquad \mathcal C=(I,R).
\tag{T9.45}
\]

Here \(A\) is the actual constrained physical high-mode Hessian and \(M'\) is the Hessian of the retained classical action. The constrained envelope identity identifies \(\partial_\lambda M'\) with the Hessian of the actual transported tensor mark; it includes the minimizing response. This is the same derivative as in (T9.33), not a direct-plaquette replacement.

For any \(m>0\), the regulator \(m^2\overline Q^*\overline Q\) adds only \(m^2I\) to the lower-right block of (T9.45). Therefore

\[
\det(M+m^2\overline Q^*\overline Q)
=c(F)\det A\det(M'+m^2I),\qquad
c(F)=|\det\mathcal C|^{-2}.
\tag{T9.46}
\]

The coarea factor may depend on the background and on the volume. It is independent of the tensor source. Consequently \(\partial_\lambda\log c(F)=0\) identically, before taking any curvature derivative or thermodynamic limit. This removes the induced quotient metric and coarea from the marked determinant identity without asserting that they are background-independent.

The same observation permits a convenient gauge for computing either retained determinant. On a stationary background the gauge-invariant Hessian kills the gauge tangent. Add a source-independent background gauge form, for example \(D D^*\), and use the orthogonal decomposition into physical and gauge tangent spaces. Its determinant is the quotient determinant times a gauge determinant and a coordinate Jacobian. Both extra factors are source-independent. Their source derivatives vanish even though their curvature derivatives need not. The original source contour gauge gives the same marked trace by (T9.34). No Faddeev–Popov equivalence for a noninvariant individual mark is used.

#### 12.2 The exact scale in the raw source convention

Use the source's raw link-angle coordinates and the Euclidean site-counting inner product. In an orthonormal \(L^4\)-cell Bloch basis, a constant fine connection \(a\) has soft coordinate \(L^2a\), whereas its raw coarse link angle is \(La\). Thus

\[
Q_{\mathrm{soft}}(0)=L^{-1}I,
\qquad \widetilde Q=LQ,
\qquad
m=L\mu.
\tag{T9.47}
\]

The fine regulator in (T9.46) is then
\(\mu^2\overline{\widetilde Q}^{\,*}\overline{\widetilde Q}\), with soft limit \(\mu^2I\), while the coarse regulator is \((L\mu)^2I\). This deterministic mass rescaling is retained in the determinant difference. It is the source of the continuum logarithm of \(L\); it is not absorbed into the source-independent coarea factor.

#### 12.3 The actual alias bounds

Use a centered cell and midpoint conventions. At zero curvature, the linearized source average has the form

\[
Q_{\mu\nu}(p)=B_L(p)S_L(p_\mu)\delta_{\mu\nu}
                 -d_{L,\mu}(p)R_\nu(p).
\tag{T9.48}
\]

Here \(B_L\) is the block average, \(S_L\) is the straight bond-path sum, and \(R\) is the average root-to-site path. The second term is a coarse gradient. Centering makes the first displacement moment zero. After (T9.47), the soft branch consequently has \(\widetilde Q_{00}(p)=I+O_L(|p|^2)\). Every nonzero alias has a zero of the block-average factor at coarse momentum zero, and the path term also has its displayed coarse gradient factor. Hence \(\widetilde Q_{0h}(p)=O_L(|p|)\). These statements are about the actual average; no replacement filter is introduced.

The needed uniform gap for high aliases is also an actual free-field fact. Iterating (T9.48) gives the curvature filter
\(s_\xi(p_\mu)s_\xi(p_\nu)\prod_\rho s_\xi(p_\rho)\), where
\(s_\xi(q)=\xi\sin(q/2)/\sin(\xi q/2)\), with its continuous value at zero. Its nonzero-alias factors obey the absolutely summable product bound \(C\prod_\rho(1+|n_\rho|)^{-1}\). This bounds the retained physical covariance above by \(C|d_1(p)|^{-2}\), uniformly in \(\xi\). For the lower bound use only the zero alias: its factors are bounded above and below on the current Brillouin zone, and the diagonal averaging factors map the fine gauge direction to the coarse gauge direction. On the corresponding transverse spaces its map is invertible with bounded inverse. The zero-alias covariance is therefore at least \(c|d_1(p)|^{-2}\); all other aliases add nonnegative forms. Inverting gives
\(c|d_1(p)|^2\le M_k(p)\le C|d_1(p)|^2\) on the physical quotient. At fixed \(L\), every nonzero one-step alias near coarse momentum zero has a uniform positive gap. A bounded irrelevant norm alone would not prove that gap.

For the curvature jets, the block map is a finite local analytic expression. Its midpoint soft defect has magnetic weighted order two and its high-alias component has order one. Orthogonal quotient projection does not spoil these orders. To see this, write a physical projector as
\(P=I-D(D^*D)^{-1}D^*\), using magnetic products. The centered fine and coarse gradients, expressed in the same physical momentum, differ from the common continuum gradient by terms of weighted order three. Their projector difference therefore has weighted order two: either a gradient difference contributes \(3-2+1=2\), or the inverse-Laplacian difference contributes \(1-2+4-2+1=2\). Differentiating in curvature lowers the bound by two powers of momentum. Thus a second curvature derivative of the quotient soft defect may be \(O(|p|^{-2})\); it is not assumed bounded.

Fold into the finite \(L^4\)-alias matrix and eliminate its gapped high block. Use a fixed local identification of the internal cell fibers by background transport; it is source-independent and its finite curvature jets are bounded at the chosen fixed \(L\). At flat background the fine retained action is diagonal between distinct aliases. It is not assumed diagonal at nonzero curvature: the curved off-diagonal terms and the finite derivatives of the internal identification are retained, and they start at weighted order at least two. The regulator's low-high term has order one, its soft defect has order two, and its high-high change is bounded. The Schur formula consequently shows that the difference between the soft operators obtained with \(\mu^2\overline{\widetilde Q}^{\,*}\overline{\widetilde Q}\) and with \(\mu^2I\) is \(\mu^2E_\mu\), where, for \(0<|p|<p_0(L)\),

\[
\|\partial_p^\nu\partial_F^\alpha E_\mu(0,p)\|
\le C_{\alpha,\nu}|p|^{2-2|\alpha|-|\nu|},
\qquad |\alpha|\le2.
\tag{T9.49}
\]

Only finitely many momentum derivatives are used. The same estimates hold for the first tensor-source derivative, multiplied by \(\|J\|\). The reason is that the block map and the projectors have no source derivative, while the source derivative of the action has the principal curvature form and the actual remainder bounds (T9.40). In the Schur difference, terms involving the low-high mass twice carry an additional \(\mu^2\); terms involving a low-high action factor have at least the weights just stated. All high inverses are bounded by the alias gap. The high determinant difference has an integrable curvature-jet bound \(C\mu^2(1+|p|^{-2})\).

#### 12.4 Vanishing regulator discrepancy

For completeness, (T9.49) gives a quantitative mass comparison, rather than only a pointwise assertion. Let \(\rho=(|p|^2+\mu^2)^{1/2}\). The soft inverse with identity mass and source-independent background gauge satisfies the finite magnetic bounds
\(\partial_F^\alpha\partial_p^\nu C_\mu=O(\rho^{-2-2|\alpha|-|\nu|})\), up to the required orders. Its first source derivative has the same orders: the source Hessian has weighted order two. These bounds follow recursively from the symbol inverse equation; the massive ellipticity and (T9.38) give their uniform constants.

The constant-field magnetic product through degree two is obtained by expanding the parallel-transport triangle phase. An order-\(n\) term has \(n\) curvature factors and \(n\) momentum derivatives on each factor. It therefore preserves the sum of the weighted orders. Apply this finite product rule to
\(\log_\star(I+C_\mu\star\mu^2E_\mu)\). Its zero-curvature argument has norm at most \(C\mu^2\), so its power series and the finitely differentiated series converge for small \(\mu\). The term with two curvature derivatives on one factor is bounded by
\(C\mu^2[|p|^2\rho^{-6}+\rho^{-4}+|p|^{-2}\rho^{-2}]\).
Terms with one curvature derivative on each of two factors are bounded by \(C\mu^4\rho^{-4}\); the momentum-derivative terms from the magnetic product obey the same bounds. A first source derivative changes only the constant times \(\|J\|\). Consequently the marked curvature coefficient of the soft determinant discrepancy obeys

\[
|\partial_\lambda\partial_F^2\,\delta\log\det(p)|
\le C\|J\|\frac{\mu^2}{|p|^2(|p|^2+\mu^2)}.
\tag{T9.50}
\]

The notation includes mixed curvature directions. Integrating (T9.50) in four dimensions, and adding the gapped aliases and the region away from zero, gives

\[
\left\|\Pi\,\partial_\lambda
\left[\log\det(M+\mu^2\overline{\widetilde Q}^{\,*}
                       \overline{\widetilde Q})
      -\log\det(M+\mu^2I)\right]\right\|
\le C\|J\|\mu^2\bigl(1+|\log\mu|\bigr)
\longrightarrow0.
\tag{T9.51}
\]

These are trace densities, with the same physical volume convention on both sides. The order is bulk first at fixed \(\mu>0\), followed by \(\mu\downarrow0\). The finite-volume Schur identity holds before that limit; the curvature jets used in (T9.49)–(T9.51) are its bulk local coefficients. No smoothness of the orthogonal physical projector at exactly \(p=0\) is asserted. Gauge stabilizers are omitted consistently and any finite-dimensional physical harmonic contribution is handled with the positive mass before taking the bulk limit. For the smallest nonzero momenta on a torus of side \(R\), the bound in (T9.50), including the volume factor, is \(O(R^{-2})\) at fixed \(\mu\); the other low modes form the integrable Riemann sum displayed above. Equivalently, the source-dependent trace may be computed with the full local gauge-fixed massive operator, whose omitted gauge factor is source-independent. Compatible finite-torus local projections retain their recorded tails. This order also avoids attributing positivity to an unregulated magnetic infrared sector or differentiating between distinct quantized-flux sectors on a fixed torus.

**Theorem T9-F.** At the actual stationary Cartan test backgrounds, the tensor-source derivative of the high Gaussian determinant is exactly the fine-minus-coarse retained derivative with the quotient/coarea factor removed by source independence, as in (T9.46). In the raw source units the masses are \(\mu\) and \(L\mu\). Replacing the fine block regulator by identity mass changes its marked curvature coefficient by a quantity tending to zero, quantitatively (T9.51). The proof uses the actual block filter, the uniform retained ellipticity, and the full low/high alias Schur calculation. It does not assume that the periodic block regulator has a single translation-invariant symbol.

### 13. A separate all-channel smooth-source corollary

The point-family normalization restriction does not leave the already constructed smooth-source argument conditional on an unidentified regular class. A7/A8 now supply that class and the actual covariant regular reference at the prescribed frozen coupling and counterterm sequence. The remaining hypotheses of the N7 density-lift theorem are the proved classical contraction, the finite-jet \(O(g_k^2)\) blocks, and the two-sided asymptotic-freedom spacing.

Let \(f_{k,x}=\iota_x+S_{k,x}\) be its uniformly bounded, normalized covariant density graph, and let \(E_k\) be the full uniform-source matrix, including the stable feedback. Define the ordered products and one microscopic matrix by

\[
P_{j,k}=E_{k-1}\cdots E_j,\qquad
Z_K=P_{0,K}^{-1}.
\tag{T9.52}
\]

This is the same matrix for every root and every test source in this regular reference. It may depend on the ultraviolet cutoff and the fixed normalization endpoint. Its norm need not be bounded in the tensor channels.

For a fixed smooth, possibly 21-component source \(\phi\), the exact lifted density identity N7.25 and its physical first moment N7.27 give

\[
\begin{aligned}
\bigl\|\mathscr L_{0,k}(f_0Z_K\phi_0)
 -f_kP_{k,K}^{-1}Q_{0,k}\phi_0\bigr\|_{\delta,N}
&\le C\left(\frac{x_k}{x_K}\right)^s
       h_k\,\|\phi\|_{N,1},\\
\bigl\|\mathscr L_{0,k}(f_0Z_K\phi_0)\bigr\|_{\delta,N}
&\le C\left(\frac{x_k}{x_K}\right)^s
       \bigl(\|\phi\|_{N,0}+h_k\|\phi\|_{N,1}\bigr).
\end{aligned}
\tag{T9.53}
\]

Here \(\phi_0(x)=\phi(h_0x)\), \(Q_{0,k}\) is the scalar hat average on source profiles, \(\|\cdot\|_{\delta,N}\) is N7's full rooted density-family norm with a fixed polynomial spatial weight, and \(\|\phi\|_{N,j}\) is the corresponding fixed Schwartz seminorm through derivative order \(j\). The hats only represent the exact transported physical sum; they do not replace the original positive kernel by a random-phase mixture.

To recall why the initial inverse-normalizer growth is harmless here, a defect born at step \(j\) has the explicit factor \(h_j\|\nabla\phi\|\). Its full later propagation is bounded by N7.30. With \(n=k-j\), the resulting sum is controlled by
\(h_k(x_k/x_K)^s\sum_{n\ge1}(e^\varepsilon/L)^n(1+c_+n/x_*)^{p+s}\), with one fixed \(\varepsilon<\log L\). This converges uniformly in the ultraviolet horizon. No bounded initial tensor seed or phasewise tensor endpoint estimate is used. The proof includes the complete regular remainder through the Banach-valued density lift.

**Corollary T9-G.** The actual admitted covariant regular reference has a common 21-channel microscopic normalization for one smooth source, with the full-family bounds (T9.53). For a spatial weight order \(N>4\), the bounded physical sum \(h_k^4\sum_x(1+|h_kx|)^{-N}\) converts the family bound into the corresponding smeared estimate, retaining the explicit dimension-four factor \(h_k^{-4}\) when it is restored. This statement is for the regular reference and for the already justified regular-forcing comparisons on their common charts. It does not extend that comparison to a mixed-boundary carrier.

This corollary does not imply a point-delta estimate: its Lipschitz seminorm would then diverge with the original mesh. It also does not construct the multi-source derivatives, collision counterterms, historical conditional means, or limiting operator family needed for the full observable theorem.

### 14. Status and scope

The following subgates are resolved in this module:

1. **Old-action dependence of the critical one-loop coefficient:** removed by T9-A on the actual current-link action, with constrained affine reproduction proved explicitly.
2. **Cutoff dependence of that coefficient:** reduced by T9-B to an arbitrarily rare local Gaussian error.
3. **Mean matrix structure and metric construction:** T9-C gives seven fixed orthogonal symmetry sectors; (T9.30) constructs the required metric from five scalar interval-product bounds after the neutral channels are controlled.
4. **Actual pseudoscalar mean normalization:** T9-D proves its boundedness for the specified clover source through an admitted geometric charge and the actual classical stable graph.
5. **Retained magnetic symbol and source-derivative weights:** T9-E proves (T9.40) from the actual stable analytic norm and the weighted gauge jet, with no assumed continuum matching.
6. **Group scope of the continuum dimension-four one-loop target:** the direct two-structure-constant argument gives (T9.42) for a compact simple group in the fixed trace convention.
7. **Gauge, coarea, and regulator identification in the Gaussian Schur step:** T9-F proves the actual marked quotient identity and the vanishing regulator discrepancy with the correct raw-source mass rescaling.
8. **The five remaining regular mean-growth bounds:** N9 combines T9-E/F with the direct U9 trace and proves the bounded finite-part identity, the interval bounds (T9.29), and the actual metric (T9.30).
9. **One-source smooth normalization in all 21 channels:** T9-G records the now-admitted N7 exact density-lift theorem, including the full regular remainder and the common microscopic matrix.

The regular mean-metric subgate is therefore closed under the standing A7/A8/N7 analytic and asymptotic-freedom premises. The principal sign is not inferred from generic Gaussian positivity: it is computed in U9, and the actual scheme is matched in N9 with a bounded endpoint difference. Together with S8-C and P9, this supplies all-order translation-phase moments for deterministic initial seeds whose admitted norm is uniformly bounded. The scalar and pseudoscalar mean normalizers have bounded inverses, so their mean-normalized regular benchmark families satisfy that initial-norm condition.

These are results for the covariant regular family. They control the anisotropic phase noise reached from those bounded scalar or pseudoscalar seeds through the full mean metric; they do not make an individual phase preserve either neutral channel. The inverse mean products for renormalized stress and Weyl seeds can grow with the ultraviolet range, with the powers corresponding to (T9.43). Their common point-family endpoint/SP37 condition and uniformly renormalized phase moments are not proved by mean dissipativity alone. Mixed-boundary histories, full-law S2, generated source jets, and the later observable/operator existence obligations retain their separately stated requirements. No finite-volume local projection tail is silently changed into an exact identity, and no topological conservation statement is applied to a large-field reset.

#### Primary and source anchors

- **CMP102, printed pp.278–279:** (2), (7), and Theorem 1 for the actual gauge-invariant regular domain and the unique constrained critical orbit; its later minimizing-field derivatives supply the current response used here.
- **CMP109**, [DOI](https://doi.org/10.1007/BF01215223): (0.4), (0.11)–(0.12) for the flat averaging identity; (1.1), (1.11)–(1.18) for nonflat regular fields and local analytic domains; (2.5)–(2.13) for the constrained Gaussian and amplitude expansion.
- **CMP119:** printed p.247 after (1.7) for the Euclidean-invariant gauge-fixing construction; (2.29) and (3.39) for the whole regular density covariance; (3.32) for the Gaussian cutoff expansion.
- **M. Lüscher, CMP85 (1982), 39–48**, [DOI](https://doi.org/10.1007/BF02029132): §3 and footnote 6 for the admissible-cell cocycle and its power identities; §4, (32)–(36), for local gauge invariance, topological invariance, and the curvature jet. The extension and source-domain estimates needed here are supplied in §7 above.
- **G. Ferretti, R. Heise, and K. Zarembo**, [hep-th/0404187v3](https://arxiv.org/pdf/hep-th/0404187): the canonical convention and dimension-four one-loop coefficients (6)–(7); the group extension and its limits are supplied in §11 above.
- **Existing mechanisms:** A7 polynomial gauge normalization and stable contraction; A8 actual regular-action identification and Gaussian cutoff estimates; N7 finite-jet bounds; N8.14–N8.20a for the full mean source coefficient and its forward/backward coordinates; N8.28–N8.38 for scalar neutrality; S8-C for the phase-moment implication.
- **Companion results:** [observable_ii.md](observable_ii.md), U9.1–U9.18, computes the principal tensor trace directly; [observable_iii.md](observable_iii.md), N9.12b and N9.13–N9.28, proves actual retained ellipticity, the bounded finite part, the marked Schur identity, and the interval-product bounds. [observable_vii.md](observable_vii.md) states the all-order phase consequence and its bounded-initial-seed restriction.

---
