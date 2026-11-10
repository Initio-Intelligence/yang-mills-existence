# Periodization of the whole-torus flat Gaussian

## 1. Result and the important distinction between the two gauge formulas

**Result:** the source-free, identity-background, whole-torus **reference Gaussian** in B109 (2.11)–(2.13), pp.267–268, has a physical curvature covariance obtained by exact periodization of one infinite block kernel. This assertion includes its literal symmetrized averaging constraint, exponential gauge, free coordinates, and zero-mode convention. The proof below derives the actual linear stencils from B109 (0.8), (0.12), pp.253–254, before using the massive B95 representation. It does not include the cutoff χ_k or the nonlinear interaction inside (2.12)–(2.13), a source-dependent background, or an arbitrary source-resolved Schur complement.

There is an important gauge distinction. B96 (2.155)–(2.157), pp.249–250, first deletes the axial-tree variables and then the averaging pivots. B109 does **not** use that same coordinate set: (2.5), p.266, retains the tree variables with an exponential quadratic gauge penalty. Equation (2.11), p.267, explicitly notes the replacement of the delta gauge by this exponential gauge. The B96 formula therefore supplies a coercivity comparison, not the literal B109 free-coordinate matrix.

Use unit spacing at step k, fine spacing η=L^{-k}, and physical step length h=L^ka. Let Q_k denote the centered straight-path fine-to-step-k average. Write Q_1 for its one-step version and \(\widetilde Q_1\) for B109's actual covariant linear average. They are different operators before gauge fixing; their exact relation is derived in §3. Let T be the **symmetrized** block path average appearing in the quadratic part of B109 (2.5). Let C_Q embed the remaining unit-lattice coordinates after eliminating **only** the \(\widetilde Q_1\)-pivot bonds. At the identity background the actual reference quadratic form is

\[
 \mathcal M_k=C_Q^*(\Delta_k+T^*T)C_Q,\qquad
 \Delta_k=H_k^*d_\eta^*d_\eta H_k,\qquad
 B=C_Qb,\qquad \mathbb E[bb^*]=\mathcal M_k^{-1}.
 \tag{PZ1; P from B109 (2.5), (2.11)–(2.12), with the flat specialization}
\]

Here the field b is the normalized Gaussian variable after B109's coupling rescaling. At the identity the background force J vanishes, so the J-dependent quadratic corrections in B99 (3.128), p.421, and (3.156), p.428, vanish. Section 3 proves why the physical flat minimum and curvature readout agree with the straight-average representation in B95 (1.65), p.29, despite the different gauge and covariant average. The nonlinear constraint correction begins at quadratic order and therefore does not change the linear curvature readout.

All formulas below use the original weighted adjoints: fine measure η⁴ and unit coarse measure. Equivalently one can conjugate every matrix by the square roots of its coordinate volumes and work in ordinary counting-coordinate inner products. Periodization commutes with those diagonal, periodically repeated volume factors.

**Use in the cross-shell analysis.** The algebraic flat dictionary below is used in [Cross-shell Gaussian source transport and local vacuum](cross_shell_gaussian_source.md). That note checks the uniform B99 kernel estimates, proves physical shell orthogonality, and controls the full flat cross-shell source and cell-collar vacuum. Thus the full flat Gaussian application is not wholly open. The actual nonlinear kernels, terminal interacting law, running N2 identification, strict full-source contact refinement and source-anchor reflection still require their stated proofs.

## 2. The common-kernel construction uses no massless inverse

The formulas with Δ^{-1} in B95 (1.59)–(1.60) separate constant configurations explicitly. They are unnecessary for this dictionary. Use instead the following equivalent nonsingular chain, with Balaban's auxiliary positive mass parameter set to one:

\[
 \begin{aligned}
 G'_k&=(\Delta_0+Q_k'^*Q_k')^{-1},\\
 R_k&=I-G'_kQ_k'^*(Q'_k(G'_k)^2Q_k'^*)^{-1}Q'_kG'_k,\\
 G_k&=(d_\eta^*d_\eta+d_\eta R_kd_\eta^*+Q_k^*Q_k)^{-1},\\
 S_k&=Q_kG_kQ_k^*,\qquad H_k=G_kQ_k^*S_k^{-1},\\
 \Delta_k&=S_k^{-1}-I.
 \end{aligned}
 \tag{PZ2; L for the first four lines; P for the last line}
\]

The checked primary formulas are B95 (1.44), p.25; (1.69), p.29; (1.89)–(1.90), p.33; and (1.100)–(1.103), p.34. The last identity follows directly by inserting H_k into the positive massive quadratic form, using Q_kH_k=I and R_kd_η^*H_k=0, and comparing with (1.65), p.29. Thus it includes exactly the flat minimum action, rather than an independently chosen lattice Maxwell operator.

Every primitive derivative and straight averaging map in (PZ2) is a finite-range, periodically translated block stencil. These averaging maps satisfy the printed commuting identity Q_kd_η=d_1Q'_k. B109 uses centered odd blocks, whereas B95 initially uses lower-corner blocks. At scale k, translating the fine arguments by the fixed offset with each component (L^k−1)a/2 converts those two straight-average conventions. Conjugate the fine operators by that translation and restore the actual fine coordinates before reading the source. The identities and bounds in (PZ2) transfer under this unitary coordinate change. On the infinite lattice define exactly these centered stencils. The additional symmetrized map T and the covariant one-step constraint are treated separately in §3; they are not silently replaced by a single-tree gauge.

Here is a direct justification of the infinite inverses and their compatibility. At a fixed k, group the η-lattice into unit blocks; the Bloch symbols are finite matrices. The scalar operator Δ_0+Q_k'^*Q_k' has a positive gap by the block Poincaré inequality: zero block averages are controlled by the discrete gradient, and the remaining block averages by Q'_k. The symbol is a matrix trigonometric polynomial. Its inverse is therefore analytic in a strip and has an absolutely summable exponentially decaying block kernel. The same is true of the positive coarse matrix Q'_k(G'_k)^2Q_k'^*. For the remaining inverse operators, B95's bounds just cited give positive lower bounds on every finite-torus momentum grid. Such grids are dense in the block Brillouin torus as the torus grows. Continuity of the already defined symbols transfers the lower bounds to every real momentum. Their inverses are again analytic in a strip and have absolutely summable kernels. This argument constructs the infinite operators from their common primitives; it does not infer compatibility from decay estimates alone.

Let P_T denote summation over images shifted by the physical torus period. For these kernels, absolute summability permits rearrangement of all sums, so

\[
 P_T(AB)=(P_TA)(P_TB),\qquad
 P_T(A^*)=(P_TA)^*,\qquad
 P_T(A^{-1})=(P_TA)^{-1}
 \tag{PZ3; P for the constructed gapped block operators}
\]

whenever the displayed inverse occurs above. The inverse equality follows by periodizing AA^{-1}=A^{-1}A=I and using uniqueness of the finite inverse. Starting with the finite stencils and proceeding through (PZ2), every finite operator is consequently the exact periodization of the corresponding infinite operator.

This also fixes the zero mode. No constant mode is deleted in (PZ2): the averaging mass acts on it. B95 (1.82)–(1.83), p.31, explicitly retains the constant response GJ_0=J_0 when the auxiliary mass is one; p.33 checks that this agrees with the continuous symbol at zero momentum. The final constraint Q_1B=0 and the gauge penalty then make the reference fluctuation form positive. Introducing an additional global mean-zero projection would alter the specified Gaussian and is not part of this construction.

## 3. The literal covariant stencil, exponential gauge, and free coordinates

Let G(y,x) be B109's family of shortest within-block paths. By (0.8), p.253, the linearization of its group average is the arithmetic average. Therefore the actual gauge map and its block average are

\[
 (TB)(y,x)=\frac1{|G(y,x)|}\sum_{\Gamma\in G(y,x)}B(\Gamma),\qquad
 (mT B)(y)=L^{-4}\sum_{x\in B(y)}(TB)(y,x).
 \tag{PZ4a; P from B109 (0.8), (0.11), p.253}
\]

Let d_c denote the difference between adjacent block roots divided by L. Expanding the loop in B109 (0.12), p.254, cancels its final −c segment against the outside U(c). The remaining two endpoint path averages give

\[
 \widetilde Q_1=Q_1-d_c mT,\qquad
 D\!\left[\frac1i\log M(e^{iB})\right]_{B=0}=L\widetilde Q_1.
 \tag{PZ4b; P: exact normalized and raw constraint conventions}
\]

This displays the L factor in B109 p.267. It also shows why replacing the covariant constraint by the straight average while retaining nonzero gauge variables would be incorrect. For a scalar gauge parameter λ, path telescoping gives

\[
 T(d_1\lambda)(y,x)=\lambda(x)-\lambda(y),\qquad
 Q_1d_1\lambda=d_cQ'_1\lambda,\qquad
 \widetilde Q_1d_1\lambda=d_c(\lambda|_{\rm roots}).
 \tag{PZ4c; P}
\]

**Identification of the physical minimum.** On the straight-constraint space Q_1A=B, choose λ=TA−mTA. Its block average is zero. Thus Q_1 is preserved, T(A−d_1λ)=0, and curvature is unchanged. On the covariant-constraint space Q_tilde A=B instead choose λ=TA, whose root values are zero. The last identity in (PZ4c) preserves Q_tilde and again sets T(A−d_1λ)=0 without changing curvature. On the common gauge slice TA=0 the two averages coincide. Hence both constrained problems have exactly the same admissible physical curls and the same physical minimum.

This argument iterates. At each step the preceding effective quadratic action is gauge invariant, and its fine-curvature reconstruction annihilates a coarse gradient. The latter follows from Δ_k=H_k^*d_η^*d_ηH_k and Δ_kd_1=0. Applying the same one-step correspondence and transitivity of constrained minimization proves, inductively from the original Maxwell quadratic form, that the physical linear curvature of B109's reconstruction is d_ηH_k with the centered straight average of §2. B95 (1.16)–(1.20), p.20, identifies the composition of those straight averages. This proves the identification used in (PZ1), including the lower comparison γ_0∥d_1B∥²≤⟨B,Δ_kB⟩ from B95 (1.67), p.29. It is not an identification of the two un-fixed gauge-coordinate maps.

Choose the printed pivot b_0(c) in each corridor. No within-block path uses that crossing bond. Among the parallel paths in the average, exactly L contain it, so its coefficient in Q_tilde is L^{-4}, and its coefficient in the raw constraint LQ_tilde is L^{-3}. Thus the h of B109 p.267 has the value L³ at the pivot, in each color coordinate. If ι_F inserts zero at all pivots,

\[
 (L\widetilde Q_1)h=I,\qquad
 C_Q=(I-hL\widetilde Q_1)\iota_F,\qquad
 \widetilde Q_1C_Q=0.
 \tag{PZ4; P: literal printed pivot elimination in four dimensions}
\]

Both T and C_Q are finite-range stencils with block period L. To prove their actual gap, consider the fixed-L matrix K=C_Q^*(d_1^*d_1+T^*T)C_Q. Its Bloch symbol is a finite continuous matrix. In a quasiperiodic fiber, zero quadratic energy implies d_1B=0 and TB=0 for B=C_Qb. Closedness makes all paths within a simply connected block have the same integral. Consequently the symmetrized condition TB=0 forces every internal link to vanish. Cross-face plaquette identities then force the crossing links in each corridor to have one common value. On TB=0 the constraint is Q_1B=0; its straight average is that crossing value divided by L. Hence every crossing link vanishes too, and B=0. Since C_Q is the identity on the free coordinates, b=0.

Thus K has a positive minimum eigenvalue on the compact Bloch torus. This constant depends only on L and the fixed stencils. The uniform lower half of B95 (1.67), just identified with the actual physical quadratic form, gives

\[
 \mathcal M_k\ge\min(\gamma_0,1)K\ge c_L I.
 \tag{PZ5; P: actual exponential-gauge gap}
\]

\[
 \mathcal M_k^T=P_T\mathcal M_k^\infty,\qquad
 (\mathcal M_k^T)^{-1}=P_T(\mathcal M_k^\infty)^{-1}.
 \tag{PZ6; P: exact periodization of the actual reference matrix}
\]

The inverse statement follows from §2's common-kernel algebra. The gap argument applies in every quasiperiodic fiber, including zero momentum; it uses neither a deleted torus mode nor a nonperiodic global tree.

The delta-coordinate factor is explicit. For δ(Q_tilde B), pivot elimination contributes L^{4(N²−1)n_c}, where n_c is the number of next-step positive bonds. For the raw δ(LQ_tilde B) it contributes L^{3(N²−1)n_c}. Their ratio is the constant L^{-(N²−1)n_c}, absorbed when B109 passes to the normalized linear delta on p.267. The normalized version agrees with the scalar factor (L^d)^{|Λ'|} in B96 (2.155), p.250. The subsequent coupling rescaling contributes q_k^{D_fl}, where D_fl is the real number of free coordinates. Together with the Gaussian determinant these factors specify the unnormalized linear Gaussian normalization. They cancel in a ratio with and without a quadratic source in this same fixed chart. No source-dependent Jacobian cancellation is asserted for a different sourced constraint chart.

## 4. Physical curvature, exact source pullback, and the scale index

Work in B99's Hermitian color basis with tr(T_AT_B)=δ_AB and tr=Tr/N. Write q_k for the multiplier called g_k in B109's change B'=g_kCB; this keeps its normalization distinct from any differently normalized running coupling. The fine linear link angle is ηq_kH_kC_Qb. Let A_cl be the one-quarter average of the four consistently oriented fine plaquette curls in P2's clover. Define the two physical curvature readouts

\[
 \xi^{\rm pl}=q_kh^{-2}d_\eta H_kC_Qb,\qquad
 \xi^{\rm cl}=q_kh^{-2}A_{\rm cl}d_\eta H_kC_Qb,\qquad
 \xi=(\xi^{\rm pl},\xi^{\rm cl}).
 \tag{PZ7; P: derivative of the actual reconstruction and P2 clover at identity}
\]

The physical factor is h^{-2}, because the fine plaquette curl of the link angle ηq_kH_kC_Qb is η²q_kd_ηH_kC_Qb and a=ηh. Use the enlarged fixed curvature dimension 12(N²−1). Its covariance is allowed to be degenerate; the plaquette and clover components are correlated readouts of the same b, not independent Gaussian fields.

If D_k denotes the stacked readout in (PZ7) without q_kh^{-2}, its value covariance is explicitly

\[
 \Gamma_k^T(x,y)=q_k^2h^{-4}
   \sum_{b,b'}D_k^T(x/h,b)
      (\mathcal M_k^T)^{-1}(b,b')D_k^T(y/h,b')^{\mathsf T}.
 \tag{PZ8; P: coordinate-volume-explicit covariance}
\]

The free b coordinates have unit coarse counting measure; the factors η⁴ are already in the fine weighted adjoints when this is written as D_kM_k^{-1}D_k^*. Since D_k is made from the same common kernels, (PZ3) and (PZ6) give

\[
 \Gamma_k^T(x,y)=\sum_{n\in\mathbb Z^4}
                       \Gamma_k^\infty(x,y+nT),\qquad
 \Gamma_k^T\ge0.
 \tag{PZ9; P: exact common periodization for this reference Gaussian}
\]

The natural block period is **Lh=h_{k+1}**, because the next-step constraint and tree gauge repeat on L-blocks. To match [Finite-source Gaussian vacuum locality](gaussian_source_locality.md), index this shell by r=k+1, with its h_r=Lh. The factor h^{-4} then differs from h_r^{-4} by the fixed factor L⁴. For the K actual transformations the shell indices are r=1,…,K; an unused r=0 term can be set to zero. This matters for terminal-cell translation covariance: the last block period is h_K=ℓ₀, not Lℓ₀.

The P2 source normalization can also be recorded exactly. Taylor expansion at the identity gives the homogeneous quadratic terms

\[
 s_p^{[2]}=\frac{Na^4}{2}|\xi_I^{\rm pl}|^2,\qquad
 Q_{IJ}^{[2]}=-Na^4\,\xi_I^{\rm cl}\cdot\xi_J^{\rm cl}.
 \tag{PZ10; P}
\]

The sign comes from the anti-Hermitian P2 curvature being i times the Hermitian curvature used in (PZ7). The all-ordered tensor sum is four times the independent-pair sum. Thus the literal quadratic source exponent is exactly (a⁴/2)Σ_x ξ(x)^TJ_phys(x)ξ(x), with

\[
 J_{\rm phys}(x)=
 \begin{pmatrix}
  Nj^{(0)}(x)I_{6(N^2-1)}&0\\
 0&-8N\,(j^{IJ}(x))_{I,J}\otimes I_{N^2-1}
 \end{pmatrix}.
 \tag{PZ11; P: exact scalar and clover source pullback}
\]

Plaquette source values in the first block are read at their literal P2 anchors. Formula (PZ11) avoids treating the clover average as a pointwise multiple of a single plaquette curl. Equivalently it could be pulled back to a finite-range source matrix on plaquette curvatures, but that would no longer be the pointwise J convention of the Gaussian locality theorem.

With the normalized Wilson coefficient X_B used in [Tensor quadratic admission and the marked transition](tensor_quadratic_admission.md), q_k²=X_{B,k}^{-1}. At the bare level P2 gives X_{B,0}=Nβ_a=2N²x_0. This is a normalization conversion, not an additional coupling-flow assertion. The uniform quantitative kernel bound remains the separate B99 regularity/decay import with this conversion; the exact periodization proof does not manufacture a scale-uniform bound from fixed-k analyticity alone.
