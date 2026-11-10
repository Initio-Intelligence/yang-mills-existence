# Cyclic defects, periodization and full Gaussian sources

## 4.41 A cyclic patch forces an exterior-holonomy carrier

The all-real star theorem cannot simply be iterated with the internal minimum energy as its only reserve. A four-link actual SU(2) patch gives an explicit obstruction, even with a unique nondegenerate minimum. The full proof and exterior-link realization are in Cyclic Patch Obstruction, §§1–4.

Use normalized a=s/2 and τ=2β. Integrate the four direction-1 links based at 0,e₂,e₂+e₃,e₃ on a periodic lattice with n≥3. Fix every other direction-1 link to I. Put a noncentral g∈SU(2) on the exterior direction-2 links based at te₁ for every t, and every other exterior link to I. The transverse connection is independent of coordinate 1, with holonomy g around that square. The actual conditional phase is

\[
 S_g(Q)=4\sum_{i=0}^3a(Q_i)
      +\sum_{\{i,j\}\in C_4}
          a(Q_iT_{ij}Q_j^{-1}T_{ij}^{-1}),
 \qquad Z_g(\tau)=\int e^{-\tau S_g}dQ.
 \tag{4.254; P: an actual cyclic Wilson conditional phase}
\]

There are four shared plaquettes and sixteen one-link pinning plaquettes; none has been discarded. The cycle transports are g,I,I,I after orientation. At Q_i=I every affected plaquette is flat. The pinning terms show that this is the unique minimum and that its energy m_g is exactly zero.

In coordinates orthonormal for −tr(XY), the Hessian is H_g=6I−Adj_g(C₄), with its adjoint edge transports. Its lower bound is 4I. Three internal conjugations remove three transports; the remaining edge has adjoint holonomy with eigenvalues 1,e^{iθ},e^{-iθ}. The twisted four-cycle eigenvalues are 2cos((2πk+φ)/4). Put P(t)=t⁴−4t² and q=2−2cosθ>0. Multiplying the four factors in each color sector gives

\[
 \det H_g=P(6)[P(6)+q]^2,\quad
 \det H_0=P(6)^3,\quad P(6)=1152,\qquad
 \log\frac{Z_0(\tau)}{Z_g(\tau)}
     \longrightarrow
       \log\frac{1154-2\cos\theta}{1152}>0.
 \tag{4.255; P: nonzero exterior determinant at }m_g=0
\]

The limit follows from the finite-dimensional Laplace estimate: both integrals have the same Haar-density factor and τ⁻⁶ prefactor, while their determinant factors differ. The unique minimum and global pinning gap make the remainder O(τ⁻¹). Thus a proposed bound Γ≤Cτm_g would have a zero right side and a strictly positive left side for all sufficiently large τ. It fails already on this finite actual patch.

The source response can also detect the missing term. Give one positive (1,4) pinning plaquette at each vertex the same normalized source z. These four distinct actions are a(Q_i). This is a direction in the independent-plaquette source family of the patch theorems; it is not asserted to equal one isotropic scalar profile in P2. If Φ_g is the logarithmic source response with its flat-patch vacuum subtracted, the diagonal Hessian parameter changes from 6 to 6−z/τ. Differentiating the same uniform holomorphic Laplace estimate yields

\[
 \partial_z\Phi_g(\tau,0)
   =-\frac{qP'(6)}
           {\tau P(6)[P(6)+q]}+O(\tau^{-2}),
 \qquad P'(6)=816.
 \tag{4.256; P: nonzero field-valued determinant source response}
\]

It is nonzero although m_g=0. Consequently the analogous source majorant Cm_g|z| fails for general independent plaquette sources as well. This is an exterior-dependent activity, not a deterministic source-only vacuum.

The surrounding Wilson field does contain the missing cost: the transverse exterior plaquette has holonomy g. For g=e^{iθσ₃/2}, q≤8a(g). A correctly enlarged carrier can therefore charge the determinant response to exterior curvature. The actual averaged energy theorem controls such a bare budget once assigned. It does not perform the carrier assignment, source projection or mixed analytic estimate.

There is a constructive carrier theorem for this same fixed pinned family. Uniformly in every real g∈SU(2), for sufficiently large τ and independent sources on its twenty plaquettes,

\[
 |\Gamma_g(\tau)|\le Ca(g),\qquad
 |\Phi_g(\tau,z)|\le Ca(g)\|z\|_1/\tau
      \quad(\|z\|_1<c\tau),\qquad
 |D^m\Phi_g(0)[f_1,\ldots,f_m]|
      \le m!C^{m+1}a(g)\tau^{-m}\prod_i\|f_i\|_1.
 \tag{4.256a; P: corrected exterior-curvature reserve for this cycle}
\]

For all positive coefficient arrays near one and all g, the identity remains the exact minimum, and the four pinning terms at each vertex keep a uniform gap. The compact Laplace theorem is uniform in g and the coefficient array; its ground energy is zero. The flat-relative determinant is bounded, and its remainder is O(τ⁻¹), with coefficient derivatives. Near g=I, simultaneous color conjugation kills their linear log g terms, so their differences have an a(g) factor. Away from that chart a(g) is bounded below, and compactness supplies the same bound. A source change costs 1/τ in the weights, proving the source estimate and all jets by Cauchy. This proves a usable exterior-curvature budget for the example; it does not assert the same uniform constants for all cyclic history geometries.

This counterexample and its corrected reserve change the next calculation concretely. A successful extension must carry the holonomy-dependent fluctuation determinant and its source derivatives in a collar, even when all plaquettes containing an integrated link can be made flat. The acyclic theorem remains valid because its tree has no such transport holonomy. The example is not a counterexample to R1, R2, N1-S or YM-E. It rules out the ground-energy-only iteration of the finite star argument and identifies an explicit nonidentity term required by the complete induction.

## 4.42 Exact periodization and source pullback for the actual flat reference Gaussian

One algebraic application gap in §4.38 is closed for the frozen whole-torus identity-background reference Gaussian. The detailed source list and proof are in [Periodization of the whole-torus flat Gaussian](flat_gaussian_periodization.md), §§1–5. This is the reference measure in B109 (2.11)–(2.13), not the cutoff and interacting integrand multiplying it.

Two literal distinctions matter. B109 uses an exponential symmetrized gauge, not the axial delta gauge of the earlier B96 free-coordinate formula. Its covariant linear constraint also differs from the straight average before gauge fixing. Let T be the arithmetic average of the within-block path sums, as follows from B109 (0.8), (0.11), p.253, and let mT be its block average. In step-k unit lattice coordinates, with d_c the adjacent-root difference divided by L, direct linearization of B109 (0.12), p.254 gives

\[
 \widetilde Q_1=Q_1-d_c mT,\qquad
 D[(1/i)\log M(e^{iB})]_{B=0}=L\widetilde Q_1,\qquad
 \widetilde Q_1d_1\lambda=d_c(\lambda|_{\rm roots}).
 \tag{4.257; P: literal symmetrized constraint and raw factor}
\]

Here Q_1 is the normalized straight-path average. The other exact identities are T(d_1λ)(y,x)=λ(x)−λ(y) and Q_1d_1λ=d_cQ'_1λ. No individual tree path has been substituted for the symmetrized average.

The straight and covariant constraints nevertheless have the same feasible physical curls. On Q_1A=B, subtract d_1λ with λ=TA−mTA; its block mean is zero, so the straight constraint is preserved and the new T field is zero. On Q_tilde A=B, instead use λ=TA, whose root values are zero; this preserves the covariant constraint and again sets T to zero. On that slice both averages coincide. Curvature is unchanged in both constructions. Applying this correspondence at each step, using gauge invariance and transitivity of constrained quadratic minimization, identifies the physical fine curvature of the actual reconstruction with d_ηH_k from the centered straight-average representation. It does not identify the un-fixed coordinate maps.

At identity the background force is zero. B109 (2.5), p.266, and (2.11)–(2.12), pp.267–268, therefore give the actual Gaussian matrix

\[
 \mathcal M_k=C_Q^*(\Delta_k+T^*T)C_Q,\qquad
 \Delta_k=H_k^*d_\eta^*d_\eta H_k,\qquad
 C_Q=(I-hL\widetilde Q_1)\iota_F,\qquad
 (L\widetilde Q_1)h=I.
 \tag{4.258; P: actual exponential-gauge reference matrix}
\]

Only averaging pivots are eliminated; the exponential-gauge variables remain. A corridor pivot belongs to L of the averaged parallel paths and no within-block path. Thus its normalized coefficient is L⁻⁴, its raw coefficient L⁻³, and the printed right inverse h has pivot value L³. The delta Jacobians are respectively L^{4d_A n_c} and L^{3d_A n_c}, with n_c the number of next-step positive bonds. The coupling rescaling contributes q_k^{D_fl}. These source-independent factors cancel in the normalized quadratic-source expectation in this same fixed chart; they are not replaced by a physical-site count.

The B95 massive formulas (1.44), pp.25–26, (1.69), p.29, (1.89)–(1.90), p.33, and (1.100)–(1.103), p.34, construct the straight H_k from derivatives, block averages and gapped inverses. They imply Δ_k=(Q_kG_kQ_k^*)⁻¹−I when the auxiliary mass is one. Centered and lower-corner blocks differ by the fixed integer translation (L^k−1)a/2 in each coordinate; conjugate all primitives and restore the physical source coordinates. No massless inverse or extra mean-zero projection is needed. The printed constant response is retained.

The gap for the actual exponential-gauge form follows directly. The fixed-L Bloch symbol of C_Q^*(d_1^*d_1+T^*T)C_Q is a finite continuous matrix. Zero energy would give a closed field with TB=0: within each simply connected block all path integrals coincide, so every internal link is zero. Cross-face closedness makes each corridor's crossing links equal, and its remaining straight constraint forces that common value to zero. Hence every fiber has trivial kernel, including zero momentum. Compactness gives a positive fixed-L gap. The checked B95 (1.67), p.29, supplies Δ_k≥γ_0d_1^*d_1 uniformly in k; the physical-minimum identification above transfers that inequality to (4.258).

Construct the infinite operators from these same periodic finite-range primitives and their gapped Bloch inverses. At each fixed k their kernels are absolutely summable. Periodization commutes with products and weighted adjoints by absolute convergence; it commutes with each inverse by periodizing both inverse identities and using uniqueness. In particular,

\[
 \mathcal M_k^T=P_T\mathcal M_k^\infty,\qquad
 (\mathcal M_k^T)^{-1}=P_T(\mathcal M_k^\infty)^{-1},\qquad
 \Gamma_k^T(x,y)=\sum_{n\in\mathbb Z^4}
                  \Gamma_k^\infty(x,y+nT).
 \tag{4.259; P: common periodization of this actual reference family}
\]

Fixed-k analyticity of the Bloch inverse alone is not the uniform quantitative curvature bound (4.242); that bound remains the separate B99 regularity/decay import with its scale conversion.

The source pullback is also explicit. Use B99's Hermitian basis normalized by tr(T_AT_B)=δ_AB, with tr=Tr/N. Let q_k be B109's multiplier in B'=q_kC_Qb, h=L^ka and η=a/h. Stack the plaquette and clover linear curvature readouts,

\[
 \xi^{\rm pl}=q_kh^{-2}d_\eta H_kC_Qb,\quad
 \xi^{\rm cl}=q_kh^{-2}A_{\rm cl}d_\eta H_kC_Qb,\quad
 \xi=(\xi^{\rm pl},\xi^{\rm cl}),\qquad
 J_{\rm phys}=
 \operatorname{diag}\!\left(
 Nj^{(0)}I,\,-8N(j^{IJ})\otimes I_{d_A}\right).
 \tag{4.260; P: literal fresh quadratic P2 source}
\]

Here A_cl is the one-quarter oriented clover average. The two readouts are correlated components of one 12d_A-dimensional vector; their covariance keeps every cross-correlation. The quadratic terms are s_p^[2]=(Na⁴/2)|ξ_pl|² and Q_IJ^[2]=−Na⁴ξ_cl,I·ξ_cl,J. The tensor's all-ordered sum is four times the independent-pair sum. Therefore (a⁴/2)Σ_xξ^TJ_physξ is exactly the literal fresh quadratic source, with its stated sign and factors.

The natural block period of this fluctuation is Lh=h_{k+1}. Reindex the K transformation shells by r=k+1 so that the terminal period is ℓ₀; the extra factor L⁴ in the h⁻⁴ covariance is fixed. All weighted fine adjoints and coordinate volumes are retained in the detailed formula. The coefficient is q_k²=X_{B,k}⁻¹; at bare level X_{B,0}=Nβ_a=2N²x_0. This conversion does not settle R0's running trajectory match.

Thus exact common periodization and the fresh quadratic-source dictionary are proved for this one reference family. Section 4.46 supplies the separate uniform B99 decay check and controls the full flat cross-shell source by exact Schur transport. Its literal reflection conclusion still needs the source-anchor intertwining. The nonlinear cutoff, inherited non-Gaussian fields and their reconstructed source interactions remain in the true mixed problem. No nonlinear sourced sequence, mixed-history bound or N1-S conclusion is inferred from this reference dictionary alone.

## 4.43 Uniform cyclic Gaussian carriers on growing Wilson patches

The four-link example in §4.41 is not merely a fixed-size exception. Its Gaussian correction has a uniform local treatment on a growing family of actual Wilson Hessians. The complete proof is in [Uniform cyclic Gaussian carriers](../cyclic_carriers.md). The scope is the quadratic family specified here, not a nonlinear constrained E/R/B integral.

Fix M≥3 and a transverse three-torus of side n, with n a multiple of M and n≥2M. Let D avoid the periodic pin set (Mℤ)³. Integrate parallel links Q_x for x∈D in one longitudinal slab; all other parallel links are I. Choose exterior transverse links T_xy independent of the longitudinal coordinate. The affected Wilson action is Σ_{edges touching D}a(Q_xT_xyQ_y⁻¹T_xy⁻¹), with a=1−Re tr and Q=I at pins. It has zero minimum for every exterior. Its Lie quadratic form, in the metric −tr, is

\[
 {\cal S}^{[2]}_T(A)=\tfrac12\langle A,H_TA\rangle,
 \qquad H_T=6I-{\cal A}_T,\qquad
 ({\cal A}_TA)_x=\sum_{\substack{y\sim x\\y\in D}}
                               \operatorname{Ad}(T_{xy})A_y .
 \tag{4.261; P: actual parallel-link Wilson Hessian}
\]

The purely transverse plaquettes stay in the exterior action. Their curvature is the needed determinant carrier.

A simple random walk on D, killed on leaving D, can follow a path to a pin in at most 3M steps with probability at least 6⁻³ᴹ. Hence its survival probability is at most C_Mρ_M^m with ρ_M<1. Absolute path expansion dominates (A_T/6)ᵐ by this killed walk for every real exterior. Therefore H_T≥6(1−ρ_M)I, uniformly in the size and shape of D.

For independent literal plaquette sources j_e, put τ=Nβ, z_e=Nj_e, w_e=1−z_e/τ and d_x(w)=Σ_{e∋x}w_e. The diagonal of the sourced H_T(w) is d_x(w), and its off-diagonal blocks are −w_e Ad T_xy. If ||z||∞<r_Mτ, its normalized adjacency has absolute paths bounded by [(1+r_M)/(1−r_M)]ᵐP_Dᵐ. A complex exterior chart of fixed radius ε_M adds only exp(Cε_Mm). Choose r_M,ε_M sufficiently small to leave an exponential survival margin. This proves a common holomorphic domain for arbitrarily many Gaussian variables. A further fixed decrease of the radii keeps the Hermitian part positive, since bounded degree gives ||H_T(w,B)−H_T(1,0)||₂≤C_N(r_M+ε_M); the same determinant is therefore the convergent real-contour Gaussian integral.

The diagonal factors cancel from the flat-relative determinant. The exact, absolutely convergent trace-log expansion is

\[
 \begin{aligned}
 \Gamma_T(z)&=\log{Z_1^{\rm G}(z)\over Z_T^{\rm G}(z)}
   =\frac12\sum_{m\ge1}\frac1m\sum_{\gamma:\,|\gamma|=m,\ {\rm closed}}
       \omega_\gamma(w)
       \{d_A-\operatorname{tr}_{\rm Ad}\operatorname{Ad}T_\gamma\},\\
 \omega_\gamma(w)&=\prod_{i=0}^{m-1}
            {w_{\{x_i,x_{i+1}\}}\over d_{x_i}(w)},\qquad d_A=N^2-1 .
 \end{aligned}
 \tag{4.262; P: rooted closed-walk expansion}
\]

The sum includes repetitions. A term depends only on the exterior walk edges and source plaquettes incident to its vertices. Its rooted absolute sum, weighted by exp(κm), is bounded uniformly in D. This gives explicit analytic local activities, with Cauchy control of every source derivative and fixed-order exterior derivatives. The flat source vacuum is L_D^G(z)=log[Z_1^G(z)/Z_1^G(0)], while the retained exterior source is Φ_T^G(z)=−Γ_T(z)+Γ_T(0).

For a real exterior, the adjoint character defect satisfies d_A−tr_Ad Ad G=N²−|Tr G|²≤2Ns(G). A nonwinding cubic walk of length m can be contracted by at most m² elementary plaquette interchanges. The product inequality ||ΠG_i−I||_HS≤Σ||G_i−I||_HS bounds its character defect by Cm⁴ times the exterior plaquette action in distance m of its root. The polynomial is absorbed by the killed-walk decay. Winding walks have length at least n. Thus

\[
 0\le\Gamma_T(0)\le C\sum_f s_f(T)+C|D|e^{-cn},
 \qquad
 |\Phi_T^{\rm G}(z)|
 \le {C\|z\|_\infty\over\tau}
       \left\{\sum_f s_f(T)+|D|e^{-cn}\right\}.
 \tag{4.263; P: curvature carrier, not internal minimum energy}
\]

The sum uses actual transverse exterior plaquettes. It is not declared to be an identity counterterm.

Differentiating a scalar walk weight marks an incident vertex. Cyclic re-rooting cancels its count against the trace-log factor 1/m. This retains the source anchor and proves the stronger estimate

\[
 |\Phi_T^{\rm G}(z)|
 \le {C\over\tau}\sum_e|z_e|
       \left\{\sum_f e^{-c\,\operatorname{dist}(e,f)}s_f(T)+e^{-cn}\right\}.
 \tag{4.264; P}
\]

Every q-th source derivative has the analogous bound with q!C^{q+1}τ⁻ᑫ, one localized source slot and sup norms for the others. In literal source units this is β⁻ᑫ. For a simultaneous constant source, H_T(w)=wH_T and the determinant ratio is unchanged: Φ_T^G(t1)=0 exactly. Individual spatial derivatives need not vanish.

On the cofinal subfamily with T/ℓ₀ a multiple of 2M, the same pins are available at every scale. Summing the winding contribution over longitudinal slabs and scales gives

\[
 \sum_{k=0}^{K}N_k e^{-cT/h_k}
 \le N_T\sum_{r=0}^{K}L^{4r}e^{-2cL^r}
 \le C N_T,\qquad h_k=L^ka,\quad T\ge2\ell_0 .
 \tag{4.265; P}
\]

This proves the physical-volume count for that remainder. The curvature term still requires the actual field projection and normalized exterior estimate.

The uniform growing-patch Gaussian carrier is therefore completed. A general Balaban averaging constraint must be treated with its own covariance; the nonlinear compact-group remainder, old E/B coefficients, hard selectors and mixed-scale boundary readouts remain outside this theorem. It supplies a concrete uniform analytic activity family for one recurrent output of R1, not the complete mixed induction or R2.

## 4.44 A necessary quadratic source contact in the actual Wilson law

The previous action lower bound detects the first vacuum derivative. The second derivative also necessarily diverges before contact subtraction. The complete proof, including a finite-jet normalization alternative, is in [Pressure and scalar contact terms](../pressure_contacts.md).

Let F_f=Σ_pf(x_p)s_p with the literal scalar anchors, and let B_f be the fine links whose six incident source values are all one. For every SU(N) there are β_N<∞ and c_N>0, independent of n≥2 and f, such that

\[
 \operatorname{Var}_{\mu_{n,\beta}}F_f
       \ge c_N {|B_f|\over\beta^2},
 \qquad \beta\ge\beta_N .
 \tag{4.266; P}
\]

For a fixed smooth cell-supported profile equal to one on an open subcube, |B_f|≥c_fa⁻⁴. N2-F gives β_a≤C(K+1). Thus the lower bound diverges at least as c_fa⁻⁴/(K+1)². A fixed amplitude rescaling to the admitted source norm preserves the divergence.

Here is the proof. Restricting each of the 4n⁴ links to an identity ball of radius cβ⁻¹ᐟ² gives Z_n(β)≥exp(−Cn⁴)β⁻²ᵈᴬⁿ⁴. Monotonicity of μ_βS, obtained by differentiating it as −Var S, then gives μ_βS_b≤C log(2+β)/β uniformly for each star. For the actual exterior v, put A_v(U)=Σ_{i=1}⁶s(UV_i) and W(v)=min A_v. Since W≤S_b, Markov's inequality shows that W≤δ_N has actual exterior probability at least one half for sufficiently large β.

At a minimizing U_*, set B_i=U_*V_i. If W≤δ_N, every B_i is within O(√δ_N) of I. The centered potential is 6s(Q)+E_B(Q), with E_B(I)=DE_B(I)=0 and C² norm O(√δ_N). The global comparison s(Q) comparable to dist(I,Q)² on the compact group implies, after choosing δ_N small,

\[
 3s(Q)\le A_v(QU_*)-W(v)\le9s(Q),\qquad
 \operatorname{Var}_{\pi_{\beta,v}}A_v\ge c_N\beta^{-2}.
 \tag{4.267; P: near-flat actual conditional star}
\]

For the variance bound, take an inner ball of radius β⁻¹ᐟ² and an annulus with radii Rβ⁻¹ᐟ² and (R+1)β⁻¹ᐟ². Choose fixed R so their energy ranges are separated by c/β. The comparison in (4.267) bounds the conditional normalizer by Cβ⁻ᵈᴬᐟ² and gives both sets a positive probability independent of β and v. Two independent samples prove the variance lower bound. No differentiated asymptotic expansion is needed.

A link shares a plaquette with at most 18 other links. Choose at least |B_f|/19 plaquette-disjoint links from B_f and condition on every other link. Their conditional Wilson laws are independent, and F_f is a fixed exterior term plus the sum of their star energies. Total variance is at least expected conditional variance. Using the preceding one-half actual exterior probability proves (4.266), without assuming any sign for covariances between different stars.

Now let C_a[j] be a deterministic prescribed source counterterm and H_a(j)=exp(−C_a[j])μ_a exp(F_j), with C_a[0]=0. If H_a(zf) is holomorphic and bounded by M on a fixed disk |z|<r, then Cauchy applied to H_a itself, followed by (log H_a)''(0)=H_a''(0)−H_a'(0)², gives

\[
 \left|\operatorname{Var}F_f-D^2C_a(0)[f,f]\right|
       \le{2M+M^2\over r^2},\qquad
 D^2C_a(0)[f,f]\ge c_N{|B_f|\over\beta_a^2}
                         -{2M+M^2\over r^2}.
 \tag{4.268; P: necessary consequence of a uniform source bound}
\]

Only a local logarithm at zero is used; no fixed zero-free disk is assumed. The same necessity follows directly from a bounded renormalized two-jet. A subtraction of the mean alone is therefore insufficient.

Positivity also gives an exact warning about a proposed complex-pressure shortcut:

\[
 |H_a(j)|\le
 \exp\{C_a[\operatorname{Re}j]-\operatorname{Re}C_a[j]\}
                  H_a(\operatorname{Re}j).
 \tag{4.269; P}
\]

For j=itf, the exponent has quadratic coefficient D²C_a(0)[f,f]/2. Its higher-order remainder can depend on a, so (4.268) alone does not prove divergence at fixed t. Nevertheless the modulus bound has already lost the required quadratic cancellation. [Pressure and scalar contact terms](../pressure_contacts.md) gives an exact Gaussian example where H≡1 but this majorant is (1+t²/β²)^{m/4}, which diverges with the number m of fine modes. Real pressure control alone cannot be promoted by this argument to the same-vacuum complex estimate.

The actual remaining second-jet object is explicit. With O_a(x)=a⁻⁴Σ_{μ<ν}s_{p_{μν}(x)} and κ_a,T(x,y)=Cov(O_a(x),O_a(y)),

\[
 D^2\log H_a(0)[f,g]
   =a^8\sum_{x,y} f(x)\kappa_{a,T}(x,y)g(y)
                      -D^2C_a(0)[f,g].
 \tag{4.270; P: complete normalized covariance identity}
\]

If the prescribed contact term has no mixed contribution for the two separated supports, the right-hand side is their actual covariance. An energy-size bound is not such a covariance bound.

[Pressure and scalar contact terms](../pressure_contacts.md) proves a concrete conditional route: subtract a symmetric source Taylor jet through degree four from the actual kernel; a dimension-eight ultraviolet annular bound makes the fifth-order remainder summable. Matching the resulting local coefficients to the prescribed counterterm remains an explicit input. A separate macroscopic smeared bound can control large separations without imposing clustering. The stronger global power-decay variant is optional. None of these actual normalized-kernel or matching inputs is inferred from (4.266); the variance theorem is a lower bound and identifies the contact that a successful R2 proof must cancel.

## 4.45 Actual strict-core sources through the erased-R operation

A genuine raw-input part of the mixed operation is admitted. The proof is in [Raw core sources in the large-field operation](../raw_core.md), based on the LFR II history bound and connected expansion. It applies to the admitted source-free R operator with its stated weak-coupling reserve; its identification with the proposed physical trajectory remains conditional on R0.

A strict-core source plaquette has all four original links still explicit, with its entire support contained in one actual component operation and kept together until its first integration. A plaquette crossing between two component operations belongs to the complementary readout, even if all its links are individually still explicit. At fixed history h, split the literal source into this strict-core part and the exact rest. This is a history-dependent splitting of the original observable, not a new physical source.

B119 (1.29), p.254, retains V₀ on Ω₁ᶜ; (2.2)–(2.3), p.255, give Γ₀=Ω₁ᶜ⊂Z₁=Λ₁ᶜ. Assign each strict-core plaquette once to the operation actually integrating its complete support. If H(h)=Σ_{j≤k}M⁴R_j⁵d'_j(Z_j) is the positive capacity in LFR II (1.79), then

\[
 V_{\rm raw}(z;h,U_0)=\sum_{p\ {\rm strict\ core}}z_p s_p(U_0),
 \qquad
 n_{\rm raw}(h)\le C_L|Z_1|_1
       \le C_LM^4R_1^4d'_1(Z_1)\le C_LH(h),
 \qquad
 |e^{V_{\rm raw}}|\le e^{C_{N,L}\|z\|_\infty H(h)} .
 \tag{4.271; P: literal old readout and once-owned capacity}
\]

The fixed factor L⁴ converts layer-one volume to fine volume. The volume comparison is the one used on LFR II p.380. Budgets are partitioned when integrations are partitioned; the same original plaquette is not recharged at every later scale.

The source-free proof of (1.79) has a positive cost exp(A₀H) and negative ordinary/preparatory birth reserves. The extra source changes only A₀ to A=A₀+C_N,Lr_c. The proof of (1.80)–(1.89) remains valid for this fixed A: (1.81) bounds all future costs by C A M⁴L⁵R_j⁶(d'_j+1); ordinary births supply cP_j²(d'_j+1), and preparatory/merger reserves supply a fixed multiple of P_j, where P_j=p₀(g_j). The sufficient inequalities are cP_j²≥C A M⁴L⁵R_j⁶ and c'P_j≥C' A M⁴L⁵R_j⁶. They hold in a sufficiently weak fixed interval when the construction exponents have p₀>6r, or whenever the already chosen constants directly satisfy them. No coefficient grows with the source's age.

For the actual exterior analytic continuation, LFR II (1.73), pp.379–380, compares T'_{k,c}F with the positive real kernel T'_{k,r}(e^σF), with its controlled σ. The strict-core readout remains a function of the old real group variables in that representation. Insert its capacity majorant before performing the integrations and history sums of (1.79). On ||z||∞≤r_c this proves

\[
 |T'_{k,c}(X;z)F|
 \le e^{\varepsilon_c}
      e^{-2(1+\beta_0)^{-1}P_k},
 \qquad |F|\le1 ,
 \tag{4.272; P: marked erased-component bound on the printed domain}
\]

for erased components meeting the actual geometry and reserve hypotheses. This is a reweighted-kernel proof, not an inference that an unweighted mass upper bound controls every reweighting.

The source jets preserve the physical old readout exactly:

\[
 T'_{k,f}(X)F=T'_k(X)(V_fF),\qquad
 T'_{k,fg}(X)F=T'_k(X)(V_fV_gF).
 \tag{4.273; P}
\]

Appending a normalized fresh reference q_v yields q_vT'_k1, q_vT'_kV_f and q_vT'_k(V_fV_g). The reference removes none of the old masses or covariance. Cauchy's formula applied before any quotient gives every source derivative with m!(e/r_c)ᵐ times the right side of (4.272). The number of original anchors was paid by the once-owned reserve before differentiating.

Now use exactly LFR II (1.90)–(1.91), replacing each erased-component operation by T'_k(X;z) and leaving the source-free admitted interactions V(Y) unchanged. Their factorization is preserved by the whole-support ownership condition. The proof of (1.92) uses the absolute operator bound just established; the subsequent tree estimates (1.93)–(1.97) are unchanged. Consequently the actual marked bracket has the connected representation

\[
 {\cal C}_k(z)=\exp\{\sum_XR'_k(X;z)\},\qquad
 |R'_k(X;z)|\le
 Cc_1(X)e^{-(1+\beta_{\rm geom}/2)\kappa d_{k,\mathcal Y}(X)} .
 \tag{4.274; P}
\]

Here c₁=exp(−P_k) for carriers disjoint from the compulsory surviving components 𝒴, and c₁=α¹ᐟ³ for the boundary alternative, as in the printed estimates. The parameter β_geom is the decay margin, not the Wilson coefficient. Boundary terms retain their exterior-aware metric.

For the nonboundary R class selected on LFR II p.390, one obtains the stronger bound and all source jets

\[
 |D_z^mR_k^{\rm raw}(X;0)[f_1,\ldots,f_m]|
 \le C\,m!(e/r_c)^m e^{-P_k}e^{-\kappa d_k(X)}
                        \prod_i\|f_i\|_\infty .
 \tag{4.275; P}
\]

The connected series gives its logarithm only after summing erased components. No fixed zero-free logarithm of an individual conditional mass is asserted.

Its actual identity extraction is v_k(X;z)=R_k^raw(X;1,z)−R_k^raw(X;1,0), with all determining fields flat. This is the marked version of B119 (2.30), p.260. The second derivative is the flat connected coefficient, including the genuine V_fV_g term in (4.273) and the product terms from different component operations. It is not a product of separately normalized means. Let R̂ be the source difference minus v_k. Gauge invariance eliminates its color-linear field coefficient; Cauchy on a normalized inner field chart gives

\[
 |\widehat R_k(X;\xi,z)|
 \le C e^{-P_k}e^{-\kappa d_k(X)}
                \|\xi\|^2\,{\|z\|_\infty\over r_c},
 \quad \|\xi\|\le\tfrac12,\quad\|z\|_\infty\le r_c/2 .
 \tag{4.276; P}
\]

The full quadratic field output is retained. Its subsequent dimension-four projection and endpoint-layer norm require the actual reconstruction map. Boundary terms are not assigned this bulk vacuum subtraction. A bounded strict-core clover readout has the same raw admission by its fixed compact-field bound; tensor marginal transport does not follow.

This completes a source-dependent actual R-operation module at arbitrary history age. It leaves the source readouts already converted to E/B functions, cross-operation supports, nonadmitted reconstructed boundary factors, and compulsory terminal survivors to be handled in their correct representation. It also leaves the torus-independent physical-cell comparison of the polymer-local vacua. These remaining problems are narrower than a general marked R admission, but they still prevent a full R1 or R2 conclusion.

## 4.46 The full cross-shell Gaussian source and its local vacuum

The cross-shell issue left open in §4.38 is resolved for the complete flat quadratic curvature model. The full proof is in [Cross-shell Gaussian source transport and local vacuum](cross_shell_gaussian_source.md). It includes the actual flat fluctuation references with their linear physical reconstruction, and a terminal Gaussian completion of that quadratic model. Balaban's actual terminal interacting or Haar density is not replaced by this completion.

Let Q_r be the nested flat block constraints on fine potentials, and let E_a=ran d_a be the physical exact-curvature space with fine inner product a⁴Σ_x. Put K_r={d_aA:Q_rA=0}. Energy minimization shows that a constrained minimizing curvature is orthogonal to K_r. Since the kernels of the nested constraints increase, their successive orthogonal differences are exactly the reconstructed one-step fluctuation spaces. Integrating pure gauge coordinates leaves a Gaussian with energy ||F||²/2 on each such space. Its covariance is the corresponding orthogonal projection P_r. Therefore

\[
 E_a=S_1\perp\cdots\perp S_K\perp M_K,\qquad
 P_rP_s=0\ (r\ne s),\qquad
 \sum_{r=1}^{K}P_r+P_{\rm t}=P_{E_a}\le I,\qquad
 \operatorname{rank}P_{\rm t}\le4(N^2-1)N_T .
 \tag{4.277; P}
\]

The proof retains the actual admissible potentials in defining K_r; it does not drop a constraint by a gauge argument. The equality of the exponential-gauge physical covariance and the axial physical covariance is proved by a linear gauge-orbit change preserving the physical curl and the constraint, with a constant Jacobian. Their coordinate covariance matrices need not agree.

Let B be the identity curvature readout or the stacked plaquette/clover averaging stencil. With arbitrary fixed positive coefficients X_r,X_t≥X_*, the independent reconstructed shells have summed readout covariances C_u=B(Σ_rX_r⁻¹P_r)B* and C_t=X_t⁻¹BP_tB*. Orthogonality proves ||C_u+C_t||≤M=||B||²/X_*, independent of K. The physical quadratic source is V_J=〈ξ,Jξ〉/2 with J a multiplication operator. Every cross-shell term is retained. In the literal stacked P2 convention, J_phys is diag(Nj^(0)I,−8N[j^{IJ}]⊗I_dA), using positively ordered plane pairs I,J. This is the same sign and factor conversion as (4.260).

For any integrated subset with covariance C_A, the exact Gaussian integral is

\[
 \begin{aligned}
 \mathbb E_A
 e^{\frac12\langle v+\xi_A,J(v+\xi_A)\rangle}
 &=\det(I-C_AJ)^{-1/2}
          e^{\frac12\langle v,\mathfrak J_A[J]v\rangle},\\
 \mathfrak J_A[J]&=J(I-C_AJ)^{-1},\qquad
 \|\mathfrak J_A[J]\|\le{\|J\|\over1-M\|J\|}.
 \end{aligned}
 \tag{4.278; P: exact source transport on a fixed disk}
\]

Complete the square first for real symmetric J and extend by Gaussian-dominated holomorphy. The identity does not require invertible J. Schur maps compose because I−(C_A+C_B)J=(I−C_B𝔍_A[J])(I−C_AJ). Thus one fixed disk M||J||≤1/4 works through any number of integrations. For source support S, the series J+JC_AJ+JC_AJC_AJ+⋯ also proves P_S𝔍_A[J]P_S=𝔍_A[J]. It is generally nonlocal between points of S; these entries are retained.

The required uniform shell kernel is checked as follows. At the identity, B99's regularity conditions (3.35)–(3.36), p.396, hold with zero left sides. Its minimizer derivative estimate (3.133), p.422, and unit constrained covariance Theorem 3.15, (3.187), p.432, have uniform constants. The physical shell curvature is h⁻²d_ηH_kB with h=Lᵏa. Convolving the two derivative kernels with the unit covariance gives the h_r⁻⁴ exponential kernel, h_r=Lh. The common-kernel dictionary of §4.42 supplies exact periodization. Infinite orthogonality follows either by the same energy argument or by taking the dense finite-volume momentum grids in the common Bloch representation. Hence

\[
 \begin{aligned}
 |P_r^\infty(x,y)|&\le A h_r^{-4}e^{-\mu|x-y|/h_r},
 \qquad P_r^T(x,y)=\sum_{n\in\mathbb Z^4}P_r^\infty(x,y+nT),\\
 |C_u^\infty(x,y)|&\le C X_*^{-1}(a+|x-y|)^{-4}
                                         e^{-c|x-y|/\ell_0}.
 \end{aligned}
 \tag{4.279; P from the checked flat imports and orthogonal dictionary}
\]

The full covariance operator norm comes from orthogonality, not from summing absolute row norms.

Choose δ=ℓ₀/16, let D_c be the lifted cell collar c^δ, and let ω_c be the cell root weights summing to one. The deterministic counterterm is the single full-covariance loop recipe

\[
 {\cal L}_{a,c}^{\rm fullG}[J]
   =\frac12\sum_{m\ge1}{1\over m}
      \operatorname{Tr}_{D_c}\!
        \left[\omega_c
          (P_{D_c}C_u^\infty P_{D_c}J_{D_c})^m\right].
 \tag{4.280; P: source-local Gaussian prescription}
\]

It depends only on the source in that collar, is independent of T, and is covariant under physical-cell translations. It is not a sum of independently sourced shell determinants. There is a fixed complex source ball on which

\[
 \log\mathbb E e^{V_J(\xi)}
       =\sum_c{\cal L}_{a,c}^{\rm fullG}[J]+{\cal R}_{a,T}^{\rm fullG}[J],
 \qquad
 |{\cal R}_{a,T}^{\rm fullG}[J]|\le C n_{\rm act}(J)\le C N_T .
 \tag{4.281; P: full flat Gaussian physical-volume theorem}
\]

Here n_act counts the physical cells with a nonzero source at a point of positive root weight. The proof has three parts.

First, exact projection factorization P_r²=P_r gives trace-class decay between separated sets: split the intermediate coordinates halfway between them and use one separated Hilbert–Schmidt factor and one unrestricted local Hilbert–Schmidt factor in each part. The resulting bound is C√(vol A vol B)Σ_rh_r⁻⁴exp(−c dist(A,B)/h_r). It makes the difference between the finite-torus covariance compressed to D_c and the common infinite compression bounded in trace norm. Summing h_r gives Σ_r(ℓ₀/h_r)⁴exp(−cℓ₀/h_r)<∞. Telescoping powers costs only m r(Mr)^{m−1}, where r=||J||.

Second, compare the full torus trace rooted in c with the trace confined to D_c. At order m, use a smooth near/far Schur multiplier with range R=δ/(4m). Its Fourier coefficients have uniformly bounded absolute sum, so both resulting operators have norm at most a fixed multiple of M. Insert the exact spatial projections P_D and I−P_D at source vertices. A nonzero escaping word has at least two far edges; otherwise all vertices are joined to the root by at most m near edges and remain in the collar. The root-side endpoints of the first and last far edge lie in E=c^{δ/4}. Their localized Hilbert–Schmidt norms are at most C√vol(E)R⁻² by (4.279). All intervening factors remain in operator norm. The at most 4ᵐ exact words therefore satisfy

\[
 \left|\operatorname{Tr}\omega_c(C_u^TJ)^m
       -\operatorname{Tr}_{D_c}\omega_c
            (P_{D_c}C_u^TP_{D_c}J_{D_c})^m\right|
       \le C m^4(C'r)^m .
 \tag{4.282; P}
\]

This is a product/projection argument; an arbitrary entrywise restriction of a composite kernel is not used. The m=1 escape error is zero. A sufficiently small fixed source radius makes the series summable. A cell with zero source at all its roots contributes zero.

Third, integrate the terminal quadratic-model Gaussian using the exact Schur source J_u=𝔍_u[J]. The original C_t is positive and cell translation covariant. The rank bound in (4.277) gives Tr(ω_cC_t)≤C for each physical cell. Since J_u is supported on the original S in both arguments,

\[
 \begin{aligned}
 \|C_t^{1/2}J_uC_t^{1/2}\|_1
     &\le\|J_u\|\operatorname{Tr}(P_SC_t)
       \le C n_{\rm act}(J),\\
 \left|-\tfrac12\log\det(I-C_t^{1/2}J_uC_t^{1/2})\right|
     &\le C n_{\rm act}(J).
 \end{aligned}
 \tag{4.283; P}
\]

The source ball also bounds this operator by 1/2. Its trace norm controls the determinant. No local trace estimate for an unproved source-dressed covariance is assumed. The three parts prove (4.281) with every physical cross term present.

Cauchy on a larger fixed source ball gives every remainder jet:

\[
 |D^m{\cal R}_{a,T}^{\rm fullG}[0](J_1,\ldots,J_m)|
       \le C\,m!C_1^m
          n_{\rm act}(J_1,\ldots,J_m)\prod_i\|J_i\|_\infty .
 \tag{4.284; P}
\]

Reality, translation covariance and vanishing at zero follow directly from (4.280). Reflection/chessboard covariance follows if the literal readout and source placement intertwine the intended reflection; the existing anchor issue remains. A strict point-contact replacement for this full cross-shell cell-collar recipe is not supplied by the earlier separate-shell Taylor theorem.

The flat Gaussian source transport and integrated local-vacuum estimate are therefore closed. For a fixed interacting terminal curvature, (4.278) instead leaves its field-valued quadratic readout to be bounded under the actual law. Nonlinear reconstruction, old E/B sources, selectors, compulsory masses, the running physical dictionary and full interacting normalization still require the complete R1/R2 estimates. Gaussian orthogonality is not a substitute for those inputs.
