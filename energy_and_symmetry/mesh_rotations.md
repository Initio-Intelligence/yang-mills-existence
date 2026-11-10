# Rotations of the Wilson comparison hierarchy

The selected B-02 Wilson family of the corresponding estimate has a quantitative rotation estimate on all coincidence-flat joint tests, including tests whose supports approach a partial diagonal. The estimate is uniform along each rotation path and over moment order with a fixed factorial exponent. It applies to the 21 measured fields on that family. Its terminal coupling tends to zero. R-04 still requires the physically matched hierarchy and control of the action, observable and contact terms there. the corresponding estimate comparison, especially (1) · R-02 through R-04

## Mesh estimate

Use the fixed units, central-box embedding, centered trace-completed stencils and seven reflected normalizations of the corresponding estimate. Write \(S_m^W,S_m^{G,a},S_m^0\) for the selected ordinary Wilson, infinite-lattice Gaussian and continuum Wick full moments in those conventions. The continuum tensor space is \(\operatorname{Sym}^2(\Lambda^2\mathbb R^4)\). There is a constant \(C\), independent of \(a\le a_0\le1\) and \(m\), such that
\[
 |(S_m^W-S_m^0)(F)|\le a C^{m+1}(m!)^3\nu_{6m+2}(F)
 \qquad (F\in\mathcal S_0).
 \tag{1}
\]
For tensors take the maximum seminorm over ordered component tests in a fixed orthonormal basis. The sum over the labels costs at most \(21^m\). The choice of the bare couplings as a function of mesh remains the existence selection of the corresponding estimate. Equation (1) gives no effective bound on the bare coupling required for that selection.

Here are the mesh details. For a pair of elementary curls the separated continuum kernel is \(K(x)=\Lambda^2(I-2\hat x\hat x^t)/(\pi^2|x|^4)\). At separation \(z\) in lattice units the boundedly shifted lattice kernel equals \(K(z)+O(|z|^{-5})\). This is the estimate used for the shifted faces in the earlier Annex O. One can also see the power directly from the lattice multiplier. Near zero the discrete curl projectors use \(e^{ip_j}-1=ip_j+O(|p|^2)\) and denominator \(4\sum_j\sin^2(p_j/2)\). Subtracting the homogeneous curl projector leaves a symbol with derivatives of order \(k\) bounded by \(C_k|p|^{1-k}\). On a smooth dyadic shell of radius \(t\) its Fourier coefficient is bounded by \(C_B t^5(1+t|z|)^{-B}\), by rescaling and integration by parts. Summing shells with \(B>5\) gives the stated power. Smooth terms away from zero decay faster, and the removal of the low-frequency cutoff on the continuum homogeneous symbol has a rapidly decreasing error away from the origin at large separation (integrate its high-frequency derivatives of order greater than four). A bounded stencil shift costs the same order by the first derivative of \(K\). At all separations use the absolute bound \(C(1+|z|)^{-4}\). Earlier Annex O, especially §§21 and the Wilson trace calculations

First give every discrete channel multiplier its continuum value \(1/2\) in the orthonormal color convention. For \(m\ge2\) put \(d(X)=\min_{i<j}|x_i-x_j|\). Wick expansion of centered full products pairs the \(2m\) curl factors across distinct insertions, including disconnected pairings. There are at most \(2^m m!\) pairings. Each insertion has boundedly many face offsets and contractions. The trace completion agrees with the continuum tensor at coalesced offsets. Thus the continuum kernel is bounded by \(C^m m!d^{-4m}\), and the discrete kernel by \(C^m m!(a+d)^{-4m}\) at the mesh sites.

Compare each lattice cell value to the continuum integrand throughout its product cell, where each site moves by at most \(2a\). Choose a fixed \(D\) larger than four times the cell and stencil radii combined. At cell centers of least separation \(d>Da\), all relevant distances remain comparable to their center distances. The error per engineering-normalized curl pair is bounded by \(Ca d^{-5}\), including the cell displacement. Telescoping the \(m\) factors bounds the kernel difference by \(a m C^m m! d^{-4m-1}\). On a cell with \(d\le Da\), the continuum least separation throughout the cell is at most \((D+4)a\).

To integrate, put \(w(X)=\prod_i(1+|x_i|^2)^{-5/2}\). For \(d\le1\), flatness on the nearest diagonal gives
\[
 |F(X)|+\max_j|\partial_j F(X)|
 \le C^{m+1}\nu_{6m+2}(F) w(X) d^{4m+1}.
\]
Indeed only the two entries of a nearest pair move to their midpoint in Taylor's formula. The highest derivative used is \(4m+2\). With displacements of bounded size, the product weights change by at most \(C^m\), and \(w(X)^{-1}\le(1+|X|^2)^{5m/2}\). For \(d>1\) the same estimate holds with the last factor replaced by 1. These bounds apply along each cell interpolation. On the far cells they pay both the kernel telescoping error and the \(O(ma)\) first-derivative cost of moving the test. On the near cells the discrete integrand is bounded by \(C^{m+1}m!\nu_{6m+2} w\,Da\) and the continuum integrand by the corresponding bound with \((D+4)a\). The statements also hold on cells centered on a diagonal, where the sampled flat test vanishes. The integral of \(w\) and its cell-weighted lattice sum are bounded by constants to the power \(m\), uniformly in the mesh. Absorbing \(m\) into that exponential gives a Gaussian comparison error of \(a C^{m+1}m!\nu_{6m+2}(F)\). For \(m=1\) the centered moments are zero.

For the seven reflected tests the lobes are fixed, smooth and separated. The same two-insertion estimate before applying the multipliers gives \(D_h^G(a)=4\lambda_h(\mu)+O(a)\). Their finite list has positive minimum \(\lambda_h(\mu)\). The inverse-square-root formula now gives \(t_h(a)=1/2+O(a)\) uniformly. Restoring these multipliers in the \(m\)-fold tensor product costs at most \(ma C^m\) times the absolute Wick estimate on flat tests derived above. This proves the lattice-Gaussian rate with the prescribed normalization. Applying the actual Wilson comparison (1) of the corresponding estimate finishes (1). Reflected measurements and trace normalization

## Rotation paths and their derivatives

Let \(U_R\) rotate all arguments and tensor labels together for \(R\in SO(4)\). Orthogonality preserves \(d(X)\), the joint Euclidean weight, and flatness to every order. Each rotated coordinate derivative mixes at most four derivatives and each tensor factor has fixed dimension. Consequently \(\nu_{6m+2}(U_RF)\le C^{m+1}\nu_{6m+2}(F)\) uniformly in \(R\). The continuum Wick full moments are invariant by the tensor transformation of \(K\). Equation (1) gives
\[
 \sup_{R\in SO(4)} |S_m^W(U_RF-F)|
 \le a C^{m+1}(m!)^3\nu_{6m+2}(F).
 \tag{2}
\]
For a unit plane generator \(D\), the derived action on tests sums a first-order coordinate rotation and a bounded rotation of each tensor index. The Leibniz rule differentiates the linear coordinate coefficient at most once, at cost polynomial in \(m\) at the displayed seminorm order. One extra weight power and one extra derivative suffice. Thus (1) also bounds \(\sup_R |S_m^W(U_R DF)|\) by \(a C^{m+1}(m!)^3\nu_{6m+4}(F)\), since \(S_m^0(U_R DF)=0\). Integration along a rotation path costs at most its length. This controls the angular variation of the full ordinary moments on the selected comparison family. Separating action and field variations on the positive-endpoint trajectory remains an open requirement of R-02 through R-04.
