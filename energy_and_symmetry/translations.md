# Fine translations of Wilson moments

Annex X, (P.2), asks for a common seminorm on differences of translated joint tests. For ordinary Wilson products there is a direct bound on these differences, even when an absolute bound for the moments on general tests is unavailable. The common shift of all insertions is one four-dimensional variable at every order. This permits a uniform estimate of the error made by sampling it on the fine lattice.

## Hypotheses and estimate

Use the real centered fields in (F.30) on a finite periodic Wilson cube, with the actual positive coefficients (F.33) or their finite totalization (F.35). Fix units with \(a\le1\). Assume the compact reserve (3.3) and, for a fixed integer \(d\ge0\), the numerical coefficient budget

\[
 \max_h |z_{h,a,T}|/\beta_W\le C a^{-d}.
 \tag{1}
\]

On the enlarged Wilson cubes of the observable proof, (1) holds with \(d=0\) on the tail because each ratio tends to \(1/2\). On a physically matched sequence (1) is a separate input. The same estimate applies to moments obtained by exact transport of the whole product. Reflected estimates, equation (3) · construction manuscript, compact reserve and Annex X

Write \(S^{\rm per}_{m,a,T}\) for the periodic lift of the ordinary full moment functional to Schwartz tests on \(\mathbb R^{4m}\). Its kernel on the infinite fine lattice is the finite-cube expectation evaluated modulo the period in each argument. For a common shift \(b\) and any fine shift \(b_a\in a\mathbb Z^4\), put \(G=\tau_b F-\tau_{b_a}F\). For \(m\ge1\), there are constants independent of cutoff, volume, order and shifts such that

\[
 |S^{\rm per}_{m,a,T}(G)|\le
 a^5 C_1^{m+1}(m!)^{d+5}\nu_{(d+9)m}(G).
 \tag{2}
\]

Here \(\nu_s\) is the manuscript’s joint Schwartz seminorm. With the central-box embedding of the torus, the conclusion holds on each fixed compact test and its fixed translates once their supports fit. For all Schwartz tests the same conclusion holds, with a possibly larger seminorm index linear in \(m\), if \(T\ge c a^{-\delta}\) for fixed \(c,\delta>0\) and the embedding cutoff equals one on \(\|x\|_\infty<T/8\).

## Proof

The compact reserve and the finite stencil bound of Corollary 3.2 give \(\|\Phi_\alpha(x)\|_m\le C m a^{-(4+d)}\). The scalar identity is included by centering the microscopic scalar before applying its multiplier. Hölder bounds each full product by \((C a^{-(4+d)})^m m!\), uniformly in the sites. The choice of tensor basis and the finite sum over component labels cost at most a fixed exponential in \(m\).

For a joint test \(H\), set \(Q_H(u)=S^{\rm per}_{m,a,T}(\tau_uH)\). Exact fine-translation invariance makes \(Q_H\) periodic in each of the four entries of \(u\), with period \(a\). Thus \(Q_G\) has zero mean on a period cell, because it is the difference of two translates of \(Q_F\). Derivatives converge absolutely under the lattice sum. For a coordinate \(l\), the \(k\)-th derivative applies \((\sum_{i=1}^m \partial_{x_i^l})^k\) to the joint test, up to sign. The sum of multinomial coefficients is \(m^k\). For \(s\ge\max(k,5m)\) this gives

\[
 \sup_u|\partial_l^k Q_G(u)|
 \le C^{m+1} m! a^{-(4+d)m}m^k\nu_s(G).
\]

Indeed \((1+\sum_i|x_i+u|^2)^{-5m/2}\le\prod_i(1+|x_i+u|^2)^{-5/2}\), and each translated four-dimensional lattice sum with its \(a^4\) weight is bounded uniformly in the shift and mesh. For each nonzero Fourier mode \(v\in\mathbb Z^4\), integrate by parts \(k\) times in a coordinate with \(|v_l|=\|v\|_\infty\). This gains \((a/(2\pi\|v\|_\infty))^k\). The sum of the frequency weights is bounded uniformly for \(k\ge5\). Choose \(k=(4+d)m+5\). Then \(k\le(d+9)m\) and \(m^k\le C_d^m(m!)^{4+d}\). The zero mode vanishes and the other modes sum absolutely, proving (2) at \(u=0\).

For the central embedding, the omitted lattice points (including those where the cutoff differs from one) have \(|X|\ge T/8\). In the unshifted evaluation on \(G\), spend an additional \(t m\) powers of the joint weight. Their contribution is at most \(C^{m+1}m!a^{-(4+d)m}T^{-tm}\nu_{(d+9+t)m}(G)\). Choose an integer \(t\) with \(t\delta\ge d+9\). This absorbs both the microscopic loss and five additional powers of \(a\), with constants uniform in \(m\). No derivative of the cutoff is used.

## Scope

Equation (2) proves the (P.2) shift estimate for the actual the corresponding estimate comparison sequence with the seven measured normalizations, and reduces this part of the physical problem to (1) on suitably growing cubes. Fine translations and permutations of the whole-product Wilson expectation were already exact. The common bound on general tests, the physical choice of coefficients, and the comparison with generated contact or approximate transport terms remain separate requirements for the target hierarchy. **P-02 remains open.**

## A finite Wilson estimate for a reflection-odd block

There is a second use of translating the same block. Work in the real Euclidean component convention of Annex X. Choose a coordinate reflection \(s\), a real compact polynomial block \(F\), and form \(D=sF-F\) with the specified tensor action. Center the reflection plane at zero. Enclose both supports and the fine field stencils strictly inside a slab of width \(l\) transverse to the reflection axis. Choose \(l/a\) even. On the periodic cube take \(M\) consecutive disjoint translates of this slab, with \(Ml<T/3\). Denote their identically distributed insertions by \(D_i\). Use their actual two boundary site planes to define

\[
 Y_i=\mathbb E_{W}[D_i\mid\text{tangential links on both slab faces}],
 \qquad C_a(k)=\mathbb E_W[D_iD_{i+k}].
\]

For every such cube the following bound holds with coefficient one, independent of the group rank, bare coupling and volume:

\[
 2\sum_{k=1}^{M-1}(1-k/M)|C_a(k)|\ \le\ \mathbb E_W Y_1^2 .
 \tag{3}
\]

Indeed, conditional on the links on all separating planes, the Wilson plaquette density factors over the slab interiors and the complementary region. The conditional integral of \(D_i\) reads only its own two faces. Thus \(\mathbb E_W Y_iY_j=\mathbb E_W D_iD_j\) when \(i\ne j\). The midpoint plane for those two blocks is a site plane; after reflection the insertions differ by a minus sign. The site-reflection square implies \(C_a(k)\le0\), including the sign on field labels. The strict support margins and \(Ml<T/3\) put the entire reflected pair on opposite halves of this plane and its periodic partner. Expanding \(\mathbb E_W(\sum_i Y_i)^2\ge0\) now proves (3). It replaces the same-slab contact cost \(\mathbb E_W D_i^2\) by the squared conditional mean on the two faces. The statement holds at any fixed degree for the literal full-product Wilson mark.

If that two-face mean has a uniform squared norm for each block on the physical sequence, (3) forces every convergent separated limiting sequence \(C(k l)\) to be absolutely summable in \(k\). First keep \(M\) fixed in the cutoff limit, taking even fine step widths tending to \(l\), then let \(M\to\infty\). This passage requires convergence on the translated tests, including their rounding errors. In OS reconstruction along this reflection axis, \(-C(kl)\) is the positive reflected two-block pairing for the translated odd block at large separation. It tends to the squared zero-energy projection. Summability forces that projection to vanish. With a valid phase disintegration and phasewise connected Euclidean covariance, a proper rotation takes this axis to the chosen OS time axis, and translation puts the test in its positive half. The same conclusion then applies to the squared phase defect of the original block in Annex V. Real and imaginary test coefficients can be treated separately in the real Euclidean field basis. Construction manuscript, Annex V (V.8)–(V.9) and Annex X (F.36)–(F.37)

For a **single smeared field on the enlarged the corresponding estimate cubes**, the right side of (3) is bounded uniformly. Suppose its stencil support and its reflection are at distance at least \(\rho>0\) from the slab faces. Around each anchor take the literal box of radius \(r\asymp\rho/a\) inside that margin. Annex O §62 gives \(\|\mathbb E[\beta_W(A_H-\mathbb E A_H)\mid\text{box exterior}]\|_2\le C_H r^{-4}\) for the trace-completed per-site stencil \(A_H=a^4 H:\widetilde q\) in the window \(1\ll r\le\beta_W^{\epsilon/100}\). The enlarged cubes and weak couplings in the measurement satisfy the window and divisibility conditions. Both slab faces are visible in this exterior. The tower property, the ratio \(z_h/\beta_W\to1/2\) and the bounded discrete \(L^1\) norm of the smooth test therefore give \(\|Y_1\|_2\le C_{F,\rho}\), uniformly in cutoff. This yields a finite uniform budget for the *sum* of the separated odd-field correlations. Full Wilson exterior estimate, Annex O §62 (O.79) · the corresponding estimate reflected Wilson measurements

On a physically matched trajectory the available box window is shorter than \(\rho/a\). The uniform two-face estimate for every normalized polynomial and identification of these blocks with the target hierarchy remain open. **V-04 remains open.**
