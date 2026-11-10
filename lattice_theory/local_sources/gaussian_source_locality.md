# Finite-source Gaussian vacuum locality

## 1. Target, status and scope

This note proves a finite-source Gaussian counterterm theorem, including a torus-independent local cell functional, an ultraviolet-summable copying error and exact reflection replication when the covariance has the stated symmetry. The covariance may connect arbitrarily distant sites with exponential decay. No finite-range approximation is assumed.

The theorem is **P as an operator statement under the explicit covariance hypotheses in §2**. Its application to every Gaussian factor in the actual Balaban construction is **C** until the exact covariance/coordinate/periodization dictionary is checked for those factors. It does not establish the nonlinear E/R/B vacuum locality or normalize compulsory histories. Full R1 and R2 therefore cannot be declared complete from this theorem.

The new point relative to a global finite-dimensional determinant estimate is that the Gaussian trace is organized by its physical source roots. The divergent local vacuum is retained explicitly. Only loops that leave a fixed physical cell collar or wind around the torus are placed in the remainder. Their exponential suppression is summable against the ultraviolet root density.

The source matrix can act on all curvature components and is allowed to depend on position and orientation. Its supremum norm is sufficient for this Gaussian theorem; smoothness is not used to obtain the cell-local functional. A slowly varying C⁵ source is a subclass. Source tensor normalizations must still be converted to the actual quadratic form: in the literal P2 clover convention, independent-pair coefficients are four times the all-ordered coefficients; using normalized trace adds N. The present quadratic-source convention has a factor one half and is defined explicitly below.

Status labels are P for proved operator facts, L for checked primary statements in their hypotheses, C for an application with an unverified physical input, and O for a remaining actual-theory estimate. The only allowed numerical program interface remains N2-F. The Gaussian hypotheses below are hypotheses of the theorem, not additional assumed Yang–Mills interfaces.

**Relation to the cross-shell theorem.** The separate-shell theorem and its strict source-jet refinement below retain their stated scope. [Cross-shell Gaussian source transport and local vacuum](cross_shell_gaussian_source.md) proves the full flat physical Gaussian source with every cross-shell term, exact Schur transport, a torus-independent cell-collar vacuum and an active-cell remainder. That full-source counterterm does not have the strict point-contact refinement proved here for the earlier operator family. Its nonlinear and literal reflection applications remain separate.

## 2. Covariance hypotheses, source convention and cell roots

Fix dimension four, an odd scale factor L≥3 and a physical cell length ℓ₀. Let a=L⁻ᴷℓ₀ and h_k=Lᵏa, 0≤k≤K. The torus side T is an even integer multiple of ℓ₀. All constants below are independent of a,K,T,k. Let d be a fixed finite curvature-component dimension, for example 6(N²−1).

For each k, let Γ_k^∞(x,y) be a real d×d matrix kernel on aZ⁴, symmetric by transposition and covariant under simultaneous translations by h_kZ⁴. Suppose X_k≥X_*>0 and

\[
 \|\Gamma_k^\infty(x,y)\|
 \le C_0X_k^{-1}h_k^{-4}
             e^{-\mu|x-y|_1/h_k},\qquad \mu>0.
 \tag{G.1; C: explicit covariance hypothesis}
\]

For each admitted torus require the exact periodization

\[
 \Gamma_k^T(x,y)
   =\sum_{n\in\mathbb Z^4}\Gamma_k^\infty(x,y+nT),
 \qquad \Gamma_k^T\ge0.
 \tag{G.2; C: common-kernel and positivity hypotheses}
\]

Positivity is that of the finite covariance matrix. Degeneracy is allowed. The sum converges absolutely. Simultaneous T-periodicity makes the expression independent of the chosen lifts. The kernel is the covariance of a centered finite Gaussian curvature vector ξ_k: E[ξ_k(x)ξ_k(y)ᵀ]=Γ_k^T(x,y). No independence between fields at different scales is needed; the theorem adds their separate logarithmic factors.

A source J(x) is a complex symmetric d×d matrix. Define the actual source exponent and the Gaussian logarithm near zero by

\[
 V_J(\xi_k)=\frac{a^4}{2}\sum_{x\in\Lambda_{a,T}}
                 \xi_k(x)^\mathsf TJ(x)\xi_k(x),
 \qquad F_k^T[J]=\log\mathbb E e^{V_J(\xi_k)},
 \quad F_k^T[0]=0.
 \tag{G.3; P: definitions}
\]

Write ‖J‖∞=sup_x‖J(x)‖op. The factors a⁴ and 1/2 in (G.3) fix the determinant convention. A physical clover source is matched by inserting its actual matrix into this definition, including its sign and normalization; no numerical factor is absorbed without being recorded.

Cells are closed cubes of side ℓ₀. Put δ=ℓ₀/16 and let c^δ be their closed max-norm collars of width δ. A cell source restriction means its values on c^δ. To avoid an artificial reflection defect at fine sites on cell faces, assign root weights ω_c(x) as follows: ω_c=1 at an interior fine site, ω_c=2⁻ʳ at a site on exactly r faces of c, and zero outside c. Periodic copies are used on the torus. Then

\[
 \sum_c\omega_c(x)=1,
 \qquad a^4\sum_x\omega_c(x)=\ell_0^4.
 \tag{G.4; P}
\]

The second identity is the product of the one-dimensional trapezoidal count with half weights at the two endpoints. Since T≥2ℓ₀, each c^δ has an injective lift to the torus. These weighted roots do not change the partition function or the source convention; they assign each trace root among adjacent cells in a reflection-covariant way.

For reflection conclusions assume, in addition, that every face reflection Θ has an orthogonal component transformation R_Θ satisfying

\[
 \Gamma_k^\infty(\Theta x,\Theta y)
   =R_\Theta\Gamma_k^\infty(x,y)R_\Theta^\mathsf T,
 \qquad
 (\Theta J)(\Theta x)=R_\Theta J(x)R_\Theta^\mathsf T.
 \tag{G.5; C: exact covariance hypothesis for reflection claims}
\]

The reflection may map one grid cell to another. The same source-value convention must be used on both sides. If the literal lower-vertex Wilson placement violates this identity, the theorem does not erase that defect; one must use the corrected placement or prove its error separately.

## 3. The local Gaussian counterterm theorem

Let S_ν be a finite constant such that
\(\sup_{0<a\le h}\sup_x a^4h^{-4}\sum_{y\in a\mathbb Z^4}e^{-\nu|x-y|_1/h}\le S_\nu\).
The product geometric series proves such a constant exists. Choose

\[
 \rho_* =\frac{X_*}{8C_0S_{\mu/2}}.
 \tag{G.6; P: sufficient source radius}
\]

**Theorem 3.1 (P under (G.1)–(G.2)).** There are cell functionals L_a^G and a remainder R_{a,T}^G such that, for every complex symmetric J with ‖J‖∞≤ρ_*,

\[
 \sum_{k=0}^K F_k^T[J]
   =\sum_c L_a^G(J|_{c^\delta})+R_{a,T}^G[J],
 \qquad |R_{a,T}^G[J]|\le C_G n_{\rm act}(J)\le C_GN_T.
 \tag{G.7; P}
\]

Here n_act(J) counts cells containing a nonzero source site, with boundary cells included. The constants depend only on d,L,μ,C₀,X_* and the fixed cell-margin ratio, never on a,K,T,J. The functional is the same on translated cells, is independent of T, and vanishes at zero. It is holomorphic on a neighborhood of the closed source ball, and real for real symmetric J. Its magnitude may diverge as a tends to zero; that is the local vacuum being subtracted, not a failed estimate.

Under (G.5) the functional is exactly reflection covariant. For a source supported in one cell at distance at least ℓ₀/8 from its faces, let WJ be its literal reflected chessboard replication. Then

\[
 L_a^G((WJ)|_{(c')^\delta})=L_a^G(J|_{c^\delta})
 \quad\text{for every replicated cell }c'.
 \tag{G.8; P under the reflection hypothesis}
\]

The local remainder is holomorphic on the same neighborhood. At zero, for every m≥1 and bounded directions J₁,…,J_m, its derivatives satisfy

\[
 |D^mR_{a,T}^G[0](J_1,\ldots,J_m)|
 \le C_Gm!(C_G/\rho_*)^m n_{\rm act}(J_1,\ldots,J_m)
                         \prod_i\|J_i\|_\infty.
 \tag{G.9; P}
\]

The active-cell count on the right refers to the union of the supports. The bound is also valid with N_T. Fixed finite C⁵ source families therefore have real-analytic local counterterms and fixed factorial remainder bounds.

**Gaussian normalized consequence (P).** Define G_{a,T}^G[J] as the product of the normalized Gaussian source factors multiplied by exp(−Σ_cL_a^G). Then

\[
 G_{a,T}^G[J]=e^{R_{a,T}^G[J]},\qquad
 |G_{a,T}^G[J]|\le e^{C_Gn_{\rm act}(J)}.
 \tag{G.10; P}
\]

For real J its logarithm has absolute value at most the same active-cell cost. This completes the locality and normalization claim for precisely this Gaussian model. It neither bounds a surviving interacting R kernel nor treats a complex field-dependent covariance without (G.1)–(G.2).

## 4. Proof of the Gaussian locality theorem

### 4.1 The determinant and the uniformly convergent loop expansion

Interpret Γ as an operator with counting measure a⁴: (Γf)(x)=a⁴Σ_yΓ(x,y)f(y). Periodization and (G.1) give row and column bounds at most C₀S_μ/X_k. Multiplication by J has operator norm at most ‖J‖∞. The Schur test therefore gives

\[
 \|\Gamma_k^TJ\|_{2\to2}
 \le C_0S_\mu\|J\|_\infty/X_k\le1/8.
 \tag{G.11; P}
\]

The same bound holds with exponent μ/2 in the positive scalar majorant. All statements continue on ‖J‖∞<2ρ_*, with norm at most 1/4. The finite Gaussian integral, including a degenerate covariance, consequently has the analytic branch

\[
 F_k^T[J]=\frac12\sum_{m\ge1}\frac1m
                \operatorname{Tr}[(\Gamma_k^TJ)^m].
 \tag{G.12; P}
\]

For a real source the formula follows by diagonalizing the covariance on its range and evaluating the Gaussian quadratic integral. The source perturbation is smaller than the identity in relative covariance norm. The integral converges absolutely for the stated complex ball, since its modulus is dominated by the real Gaussian with source ‖J‖∞I. Holomorphic continuation, or differentiation under that majorant, proves the same formula for complex J. It is valid even when ΓJ is not normal and different tensor coefficients do not commute.

Expand each matrix product into its site indices. A trace term is a loop with m source vertices, m covariance edges, and measure a⁴ᵐ. Root the loop at x₁; its coefficient is 1/(2m). Insert Σ_cω_c(x₁)=1. Define F_{k,c}^T by keeping the root weight ω_c, so Σ_cF_{k,c}^T=F_k^T exactly.

Absolute convergence at a fixed root follows from the matrix inequality |tr(A₁⋯A_m)|≤d∏‖A_i‖. Bound one closing covariance edge by C h_k⁻⁴/X_k and sum the other m−1 edges in their row norms. For the periodized closing edge its supremum has the same bound: since T/h_k≥2, the sum over its image distances is uniformly bounded. Consequently, on ‖J‖∞≤2ρ_*,

\[
 |F_{k,c}^T[J]|
 \le C\|J\|_\infty X_k^{-1}(\ell_0/h_k)^4
                      \sum_{m\ge1}\frac{q^{m-1}}m,
 \quad q=C_0S_{\mu/2}\|J\|_\infty/X_k\le1/4.
 \tag{G.13; P}
\]

This bound displays the ultraviolet-divergent local vacuum. It does not claim that the sum of these absolute values over k is uniformly bounded.

### 4.2 An exact torus-independent local functional

Choose an injective lift of c^δ to aZ⁴. Expand every periodized edge in the rooted trace into its images. Beginning at the fixed lifted root x₁, lift the successive vertices along those edges. The last vertex is x₁+nT for some winding vector n∈Z⁴. Simultaneous T-periodicity of Γ∞ makes this correspondence exact; absolute convergence permits regrouping.

Define L_{k,c}^G[J] by retaining precisely the lifted loops which close at x₁, have winding n=0 and whose every source vertex lies in c^δ. The covariance factors are Γ_k^∞; the coefficient is 1/(2m), the measure a⁴ᵐ, and the root is weighted by ω_c. Set

\[
 L_a^G(J|_{c^\delta})=\sum_{k=0}^KL_{k,c}^G[J].
 \tag{G.14; P: the prescribed local loop recipe}
\]

This formula uses only source values in the single cell collar. It uses no torus-dependent covariance or exterior completion. It is absolutely convergent by the same row estimate as (G.13), and normally convergent on every smaller source ball. Thus it is holomorphic there, including in every finite linear family. It vanishes at zero and is real for real symmetric source matrices. Reality can also be checked term by term: all kernels and sources in the restricted loop are real, so every trace is real.

The whole-lattice covariance is covariant under h_k-grid translations. A translation by ℓ₀ is an integer multiple of h_k at every k. Translating roots, vertices, source values and root weights in (G.14) therefore gives the identical functional on every cell. It has no dependence on T. The particular choice of lift does not matter, because two lifts differ by an admitted simultaneous translation.

### 4.3 Every omitted loop has a physical-length cost

An omitted loop either has nonzero winding or reaches outside c^δ. Write D for the sum of the lengths of its lifted covariance edges. A winding loop satisfies D≥T≥2ℓ₀. A loop leaving c^δ from a root in c satisfies D≥δ. Hence every omitted loop has D≥δ, and

\[
 \prod_{i=1}^m e^{-\mu|x_i-x_{i+1}|_1/h_k}
 \le e^{-\mu\delta/(2h_k)}
              \prod_{i=1}^m e^{-(\mu/2)|x_i-x_{i+1}|_1/h_k}.
 \tag{G.15; P}
\]

Here x_{m+1}=x₁+nT for a lifted torus loop. For a nonwinding loop this is the ordinary closed path. The product bound requires no finite-range approximation and no lower bound on the length of an individual edge.

Use the half-exponent kernel in the root estimate (G.13). It sums both the possible lifted intermediate vertices and the closing images; T/h_k≥2 keeps the latter sum uniform. This yields

\[
 |F_{k,c}^T[J]-L_{k,c}^G[J]|
 \le C\|J\|_\infty X_k^{-1}
       (\ell_0/h_k)^4 e^{-\mu\ell_0/(32h_k)}.
 \tag{G.16; P}
\]

If J vanishes at every root of c with ω_c>0, both sides before absolute value are zero, since every term contains J at its root. Thus only active source cells contribute. This fact gives the active-cell count instead of total torus volume.

Put r=K−k, so ℓ₀/h_k=Lʳ. The sum

\[
 \sum_{k=0}^K(\ell_0/h_k)^4e^{-\mu\ell_0/(32h_k)}
 \le\sum_{r\ge0}L^{4r}e^{-(\mu/32)L^r}<\infty
 \tag{G.17; P}
\]

is independent of K. The ratio of consecutive summands tends to zero. Sum (G.16) over k and active cells to obtain (G.7). Notice that the local part, rather than an absolute fine-coordinate count, absorbs the divergent vacuum. Only its spatial tail is summed with the exponential suppression.

### 4.4 Reflection, replication and source derivatives

Under (G.5), reflecting every vertex of a local loop conjugates its matrix product by R_Θ. Its trace is unchanged. The collar, zero-winding restriction and weights ω_c are reflection covariant. This proves L_a^G(ΘJ)=L_a^G(J), with the appropriate cell mapping and tensor transformation.

For a source whose distance from its cell faces is at least ℓ₀/8, a neighboring reflected copy is zero within the collar of width ℓ₀/16 outside the original cell. The replicated source on each c'^δ is therefore exactly the reflected source used in its isolated local functional. This proves (G.8). It avoids an implicit identification of a collar restriction containing a neighboring nonzero source with a single supported source.

Normal convergence makes the remainder holomorphic on ‖J‖∞<2ρ_*. For a finite family Σ_i z_iJ_i, choose polydisc radii ρ_*/(m‖J_i‖∞), reducing them slightly before taking a limit. The source in that polydisc stays in the radius-ρ_* ball, and its support lies in the fixed union of the direction supports. Apply (G.7) there and Cauchy's formula. The bound mᵐ≤eᵐm! gives (G.9), after changing the fixed constant. Directions of zero norm are handled by multilinearity. Exponentiating (G.7) proves (G.10). This completes the proof. ∎

### 4.5 Refinement to a strict local source-jet counterterm

For C⁵ sources, a stronger choice is available: the counterterm can depend only on source derivatives through order four at each root. This removes the finite-collar nonlocality of the preceding loop prescription at a uniformly bounded cost. The underlying C⁵ source function, restricted to its cell collar, is part of the data in this refinement.

Use the matrix algebra norm

\[
 \|J\|_{5,\ell_0}^{\rm alg}
 =\sum_{|\alpha|\le5}\frac{\ell_0^{|\alpha|}}{\alpha!}
             \sup_x\|\partial^\alpha J(x)\|.
 \tag{G.18; P: source norm for the jet refinement}
\]

At a root x, consider each infinite nonwinding loop with unrestricted intermediate vertices y_i. Replace the ordered source product along that loop by its joint Taylor polynomial through total degree four along J_t(y_i)=J(x+t(y_i−x)). Covariance matrices are held fixed in this operation. Define L_a^{G,jet} by this new loop recipe, with the same 1/(2m), fine measures and root weights. All Taylor coefficients are finite exponential moments of the same infinite covariance kernels; thus they are independent of T and covariant under cell translations. The resulting expression depends only on the jet (∂^αJ(x))_{|α|≤4}. It is holomorphic on a fixed smaller C⁵ ball.

**Proposition 4.2 (P under (G.1)–(G.2)).** After decreasing ρ_* by a fixed factor if needed, for ‖J‖_{5,ℓ₀}^{alg}≤ρ_* one has

\[
 \sum_{k=0}^KF_k^T[J]
 =\sum_c L_a^{G,\mathrm{jet}}(J|_{c^\delta})
          +R_{a,T}^{G,\mathrm{jet}}[J],
 \qquad |R_{a,T}^{G,\mathrm{jet}}[J]|
             \le C_G n_{\rm act}(J).
 \tag{G.19; P}
\]

The reflection and replication claims hold under (G.5). The finite-family analyticity and derivative estimate (G.9) hold with the C⁵ algebra norms. Derivatives of this counterterm are local source-jet distributions at one root; they do not couple distinct root points inside a cell.

**Proof.** First separate winding loops from all nonwinding loops, without a collar restriction. The winding contribution has the bound already proved, since its total edge length is at least T. The remaining source values can be read from the C⁵ periodic lift to R⁴, even when a nonwinding loop leaves the fundamental torus cell.

For an m-vertex loop put D=Σ_i|y_i−y_{i+1}|₁. Every displacement from the root is at most D. The exact fifth derivative of the ordered product has coefficient 5!/∏_iα_i!, summed over total order Σ_i|α_i|=5. Submultiplicativity of matrix norms and the definition (G.18) bound this whole sum by 5!(D/ℓ₀)⁵(‖J‖_{5,ℓ₀}^{alg})^m; no factor depending polynomially on m is inserted. The integral Taylor remainder divides by 5!.

The displacement moment is paid by a fixed part of the exponential covariance reserve: (D/h_k)⁵e^{−μD/(2h_k)} is bounded uniformly. Use the remaining half-exponent in the root Schur sum as before. For one cell, the Taylor error at scale k is therefore bounded by

\[
 C\big(\ell_0/h_k\big)^4
       \big(h_k/\ell_0\big)^5
       \sum_{m\ge1}\frac1m
          \left(\frac{C\|J\|_{5,\ell_0}^{\rm alg}}{X_k}\right)^m
 \le C_G\frac{h_k}{\ell_0}.
 \tag{G.20; P}
\]

Choosing the source radius so that the displayed geometric series converges handles every order at once. The source factor at the root is independent of t, so a cell with no nonzero source root contributes zero to both the exact loop and its Taylor polynomial. Only active cells are needed. Finally Σ_{k=0}^Kh_k/ℓ₀=Σ_{r=0}^KL⁻ʳ≤L/(L−1). Add the winding remainder to prove (G.19).

The finite Taylor terms of orders zero through four are bounded by the same exponential moments, with (h_k/ℓ₀)^q for total order q. Their source series converges normally on the smaller ball, proving holomorphy. Reflection commutes with the straight-line Taylor operation, because it is an affine isometry and the covariance has (G.5). Root weights handle lattice sites on faces as before. Finally finite-family Cauchy gives the claimed derivative bound. ∎

This is a vacuum source-jet statement. A collision with a nonidentity field-valued output, or a Schur-complement interaction between different Gaussian shells, is not removed merely by this identity-valued counterterm.

## 5. The exact operator dictionary still required for a Balaban application

The proofs in §§2–4 use no primary-source theorem beyond elementary finite Gaussian integration and matrix estimates. They expose their covariance hypotheses so that an application can be checked rather than inferred from a global determinant bound.

Section 4.6.2 of [Gaussian admission, gauge projection and reconstruction](gauge_projection.md) derives the current regular-core curvature covariance estimate from B99 (3.133), Theorem 3.12, pp.422–423, and the constrained form (3.156)–(3.158), p.428, with Theorem 3.15, (3.187), p.432. At the identity background, its stated scaling is of the form (G.1). The covariance in that assertion must be matched to the actual quadratic source and free-coordinate measure before applying the present theorem. A global constrained-Hessian comparison, by itself, proves neither an exponential kernel estimate nor (G.2).

The exact common-kernel condition is a separate algebraic dictionary. The companion note [Periodization of the whole-torus flat Gaussian](flat_gaussian_periodization.md) proves it for B109's actual frozen whole-torus identity-background reference Gaussian. It derives the symmetrized covariant constraint and exponential gauge from the printed formulas, identifies the physical minimum by a gauge-orbit argument, constructs common gapped kernels without deleting a zero mode, and tracks the pivot Jacobian and shell period. The physical source fits (G.3) after stacking correlated plaquette and clover readouts, with matrix diag(Nj^(0)I,−8N(j^(IJ))⊗I). This closes (G.2) for that precise reference family; the quantitative uniform kernel bound and actual reflection/source-placement law remain separate inputs. It does not close the cross-shell or nonlinear source dictionary.

For other proposed factors, the exact common-kernel condition still requires an operator construction. Periodization preserves absolutely summable convolution products, sums, adjoints and uniformly invertible convolutions. This elementary fact is sufficient when every actual covariance and constraint map is assembled from the same infinite block kernels, with a common periodic choice of gauge coordinates and no unhandled zero-mode removal. It does not follow merely because independently constructed finite-torus matrices have exponential bounds.

The relevant source-free flat constrained matrix is identified through B109 (2.11)–(2.13), pp.267–268, B95 (1.65)–(1.67), p.29, and B96 (2.152)–(2.157), pp.249–250. Those statements describe its constrained coordinates, positivity and normalization. A complete application must verify the actual common infinite kernel, all coordinate-volume factors and the exact source pullback. Neither the presence of a Fourier formula nor positivity alone eliminates a torus-dependent graph or a different zero-mode convention.

B116 p.21 directly supplies a localized analytic source-free Gaussian activity assertion. That is a valid L input in its printed scope. Its reference to the generalized random-walk construction in CMP 102, pp.255–275, formula (63), remains a referred proof not independently checked here. It is not a source-resolved version of (G.2), a proof of the entire local source counterterm recipe, or a statement about arbitrary mixed large-field geometries.

For the reflection statements, the exact covariance and source pullback must obey (G.5). A block tree gauge may obscure the symmetry in its coordinates even when the physical curvature covariance is covariant; prove the corresponding intertwining map. The lower-vertex scalar placement issue recorded in ICR-N1-2 remains relevant. The root half-weights fix a distinct counting issue at cell faces and do not repair an incorrect physical source transformation.

## 6. Interface statement and the cross-shell source issue

**Assumed interface:** N2-F only, as quoted verbatim in [Lattice conventions and hypotheses](../lattice_conventions.md), §2. Its lower bound on the admitted inverse coupling can supply X_* after the action-normalization dictionary is fixed. It does not supply the covariance identities (G.1)–(G.5) for a newly sourced theory.

**Delivered operator theorem:** (G.7)–(G.10), and the strict local source-jet refinement (G.19), under their explicit covariance hypotheses. The local vacuum has the desired finite-family analyticity, cell-translation covariance and, under the stated exact symmetry, reflection replication. The remainder and its derivatives are bounded by physical active-cell count. The source-dependent divergent trace remains in the specified local functional.

**Not delivered:** the identification of this product of fixed Gaussian factors with every sourced Gaussian factor in the complete interacting construction. In particular, one physical source coupled to a sum of shell fields contains cross-shell terms. For independent scalar standard Gaussians X and Y,

\[
 \log\mathbb E e^{j(X+Y)^2/2}
       =-\tfrac12\log(1-2j),\qquad
 \log\mathbb E e^{jX^2/2}+\log\mathbb E e^{jY^2/2}
       =-\log(1-j).
 \tag{G.21; P: elementary cross-shell distinction}
\]

These are unequal. Thus the phrase “sum of Gaussian normalizers” does not authorize replacing the actual source by separate diagonal shell sources. Sequential Gaussian elimination must carry the actual Schur-complement source kernel and its retained-field terms. Those kernels can become nonlocal and nonlinear in the source. Their admission and precise covariance/coordinate dictionary must be proved before applying the fixed-multiplication-source theorem to that sequence.

The same restriction applies to a shifted sourced minimum: its field-dependent Hessian is not the source-zero covariance in this note. A full proof can either retain the fixed source-zero Gaussian and treat all additional terms as marked interactions, or prove the required source-dependent Gaussian theorem on its actual domains. Neither choice is silently made here.

The new result therefore closes a defined local Gaussian vacuum calculation, including strict source-jet locality, while retaining the exact bridge still needed by R1. It does not normalize arbitrary compulsory R kernels and is not an additional assumed interface for R2.

## 7. Exact remaining uses and construction

| Required bridge | Status and exact task |
|---|---|
| Actual fixed covariance | C: identify the covariance of the literal quadratic source in the chosen regular Gaussian coordinates and prove (G.1), including its physical powers and component normalization |
| Common torus kernel | P for the frozen whole-torus flat reference family by [Periodization of the whole-torus flat Gaussian](flat_gaussian_periodization.md); O for remaining factors, whose gauge, constraints, inverse and coordinate measure must be matched |
| Reflection | C: prove (G.5) for the physical curvature kernel and actual source placement; root weights alone address only boundary counting |
| Cross-shell source | O: transport the literal source through the actual Gaussian Schur complement, or prove its marked-interaction admission without discarding the cross terms |
| Nonlinear and large-field vacuum | O: reproduce the local source recipe for the actual connected E and erased-R activities, with inherited readouts and all carrier norms |
| Compulsory normalization | O: prove the complete physical packet bound under its actual outer law; the Gaussian active-cell estimate does not replace a survivor mass |

A researcher applying this theorem should provide the actual matrix/operator formula, its coordinate-volume normalization, its infinite-kernel construction and its source pullback in one table. The check is algebraic and analytic, not a declaration that all exponentially decaying finite-volume matrices are compatible periodizations.

The whole-torus identity-background periodization and fresh quadratic-source test are carried out in [Periodization of the whole-torus flat Gaussian](flat_gaussian_periodization.md), with the actual exponential symmetrized gauge retained. The next algebraic application is the actual source-resolved Schur complement and cross-shell source. For each factor whose full hypotheses are verified, the local counterterm and strict contact form are already supplied by §§3–4. For the nonlinear part, the finite-packet source integration notes provide explicit inherited interactions to admit. Their bounds and the actual Wilson averaged-energy estimate are complementary inputs, but neither has yet supplied the complete mixed transition.

This operator theorem requires no further interface change request. It does not alter N2-F or the original N1-S statement. Its exact physical applicability is conditional where the dictionary is unverified, and its mathematical proof does not assume the conclusion of R1 or R2.

