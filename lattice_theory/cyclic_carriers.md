# Uniform cyclic Gaussian carriers

## 1. Result, exact scope and notation

**Status: P for the quadratic Wilson family defined below; O for the full mixed E/R/B transition.** This note removes the fixed-size restriction from the cyclic determinant calculation in Exterior holonomy in a cyclic patch. It treats arbitrarily large simultaneous parallel-link Gaussian integrations, arbitrary real exterior connections, independent plaquette sources, and a fixed complex exterior neighborhood. Its constants do not depend on the number of integrated links. Its local activities include the exterior holonomy that an internal-minimum-only estimate misses.

This is an actual quadratic expansion of a Wilson integration, not a model for an arbitrary positive history kernel. It does not identify hard constraints or nonlinear compact-group integrations with that expansion. The final section states the remaining difference from R1 and R2.

Fix SU(N), an integer M≥3, and a transverse three-dimensional torus with n sites per side, where n is a multiple of M and n≥2M. Let H be the sublattice with all three coordinates divisible by M. Choose any set D of transverse sites disjoint from H. A site outside D is pinned. Let T_xy∈SU(N) be an arbitrary exterior connection on the nearest-neighbor transverse edges, with T_yx=T_xy⁻¹. Each site has six edge incidences, including edges leading to pinned sites. For a directed edge use the adjoint orthogonal transformation R_xy=Ad(T_xy) on the Lie algebra, with its real inner product −tr(AB), tr=Tr/N. Write d_A=N²−1 and a(U)=1−Re tr U.

Introduce group variables Q_x at x∈D and set Q_x=I outside D. The affected Wilson action, each unoriented edge counted once, is

\[
 {\cal S}_T(Q)=
 \sum_{\{x,y\}:\{x,y\}\cap D\ne\varnothing}
 a(Q_xT_{xy}Q_y^{-1}T_{xy}^{-1}).
 \tag{W.1; P: definition and Wilson realization}
\]

To realize (W.1) in the original four-dimensional Wilson action, integrate the links in one fixed direction and one fixed longitudinal slab, with their transverse starting points in D. Put all other links in that direction equal to I. Choose the exterior transverse links independent of the longitudinal coordinate. The affected plaquettes are exactly the edges in (W.1). All purely transverse plaquettes remain in the exterior action. In particular, their curvature cost is not part of the minimum of (W.1), and must not be discarded.

Every term is nonnegative, and Q=I has zero action. The periodically available pins give a unique zero: along any path from a site in D to a pin, zero edge energy recursively forces Q=I. Expanding Q_x=exp(A_x) in anti-Hermitian Lie coordinates gives the exact quadratic term

\[
 {\cal S}^{[2]}_T(A)=\frac12\langle A,H_TA\rangle,
 \qquad H_T=6I-{\cal A}_T,\qquad
 ({\cal A}_TA)_x=\sum_{\substack{y\sim x\\y\in D}}R_{xy}A_y.
 \tag{W.2; P}
\]

Thus this family has zero internal minimum for every exterior T, while its Gaussian determinant can still depend on T. The proof below accounts for that dependence by closed Wilson loops and their exterior curvature carriers.

Give each affected plaquette an independent literal source j_e. In P2 normalization put τ=Nβ and z_e=Nj_e, so its dimensionless quadratic weight is w_e=1−z_e/τ. Let d_x(w) be the sum of the six weights incident to x, including pinned edges. The sourced Hessian and Gaussian partition function are

\[
 \begin{aligned}
 H_T(w)_{xx}&=d_x(w)I,\qquad
 H_T(w)_{xy}=-w_{\{x,y\}}R_{xy}\quad(x\sim y,\ x,y\in D),\\
 Z_T^{\rm G}(z)&=(2\pi/\tau)^{d_A|D|/2}\det H_T(w)^{-1/2}.
 \end{aligned}
 \tag{W.3; P}
\]

The determinant branch is the positive branch at z=0, continued on the domain proved below. A superscript G always denotes this Gaussian integral. No statement about the full compact-group integral is hidden in this notation.

All subsequent assertions are proved here unless explicitly marked O. They use finite matrix algebra, a killed nearest-neighbor walk, the exact Wilson plaquette algebra, and elementary complex analysis. They do not assume another program interface.

## 2. A uniform gap and a common complex domain

Let P_D be the substochastic matrix of simple random walk on D killed on leaving D: P_D(x,y)=1/6 for neighbors in D, and zero otherwise. From every site, a coordinate path reaches H in at most 3M steps. If that path leaves D earlier, killing occurs earlier. The probability of following the specified path is at least 6⁻ʰ, with h=3M. Applying the same observation after each h steps gives

\[
 \sup_x(P_D^m1)(x)\le(1-6^{-h})^{\lfloor m/h\rfloor}
 \le C_M\rho_M^m,\qquad
 \rho_M=(1-6^{-h})^{1/h}<1.
 \tag{W.4; P}
\]

The estimates deliberately use a crude constant depending on M. They require no favorable boundary shape for D and no bound on its diameter.

For real exterior T, products of its adjoint transports have norm one. Absolute path expansion therefore dominates the matrix kernel of (A_T/6)ᵐ by P_Dᵐ. Since A_T is self-adjoint, taking m-th roots of the resulting operator bounds in finite dimension proves

\[
 H_T\ge 6(1-\rho_M)I .
 \tag{W.5; P}
\]

For clarity, the finite-dimension factor converting an ℓ∞ bound to an ℓ² bound disappears under the m-th root; the surviving spectral bound is uniform in |D|. This is a spectral argument, not a claim that every row has strict contraction in one step.

Define P_T(w) by dividing row x of the weighted adjacency matrix by d_x(w). If sup_e|z_e|≤rτ with r<1, then |d_x(w)|≥6(1−r), while |w_e|≤1+r. Consequently

\[
 \|[P_T(w)^m]_{xy}\|
 \ \le\left(\frac{1+r}{1-r}\right)^m[P_D^m]_{xy}.
 \tag{W.6; P: entrywise domination for real T}
\]

Now allow a complex exterior chart T_e↦T_e exp(B_e), with B_e in the complexified Lie algebra and sup_e||B_e||≤ε. The adjoint norm of an edge factor is at most exp(C_Nε); the reverse edge is its inverse and has the same bound. Formula (W.6) then acquires only exp(C_Nεm). Choose fixed r_M, ε_M>0 so small that

\[
 \frac{1+2r_M}{1-2r_M}\,e^{2C_N\varepsilon_M}\rho_M
 <\sqrt{\rho_M}<1.
 \tag{W.7; P: choice of fixed domain}
\]

There is room for two copies of each domain, which will be used for Cauchy estimates. On this doubled domain the Neumann series for (I−P_T(w))⁻¹ converges uniformly in the block ℓ∞ norm. Thus H_T(w)=diag(d_x(w))(I−P_T(w)) is invertible and has a holomorphic logarithmic determinant with its branch continued from zero source and the real chart center. The convergence is uniform in n, D and the real exterior center T.

One can also keep the Gaussian integral itself on the real Lie-algebra contour. Bounded degree and the block row/column Schur bounds give
\[
 \|H_T(w,B)-H_T(1,0)\|_2
       \le C_N(r_M+\varepsilon_M).
 \tag{W.7a; P}
\]
Decrease the fixed radii once more so the right side is below 3(1−ρ_M). Equation (W.5) then gives Re H_T(w,B)≥3(1−ρ_M)I. The real-contour Gaussian is absolutely convergent and its value is the stated holomorphic determinant. Thus complex invertibility is not being mistaken for contour convergence.

This proves more than a fixed-dimensional Laplace-domain assertion: it gives a single analytic field/source domain for arbitrarily many integrated Gaussian variables. It does not use a global complex logarithm chart for the gauge group; separate edge charts around arbitrary real centers suffice. Gauge covariance follows from the exact connection transformation and the conjugation invariance of each closed-loop trace below.

## 3. Exact loop activities and a size-independent analytic norm

Let Γ_T(z) be the Gaussian exterior penalty, with the flat exterior denoted by 1. The diagonal factors d_x(w) are identical for T and 1 and cancel. Expanding log(I−P) on the domain of §2 yields the absolutely convergent identity

\[
 \begin{aligned}
 \Gamma_T(z)
 &:=
 \log\frac{Z_1^{\rm G}(z)}{Z_T^{\rm G}(z)}
 =\frac12\{\log\det H_T(w)-\log\det H_1(w)\}\\
 &=\frac12\sum_{m\ge1}\frac1m
   \sum_{\substack{\gamma=(x_0,\ldots,x_m)\\
                    x_m=x_0,\ x_i\in D,\ x_i\sim x_{i+1}}}
 \omega_\gamma(w)
 \{d_A-\operatorname{tr}_{\rm Ad}R_\gamma\},\\
 \omega_\gamma(w)&=\prod_{i=0}^{m-1}
       \frac{w_{\{x_i,x_{i+1}\}}}{d_{x_i}(w)},\qquad
 R_\gamma=\prod_{i=0}^{m-1}R_{x_i x_{i+1}} .
 \end{aligned}
 \tag{W.8; P}
\]

The trace uses rooted oriented walks; the factor 1/m is precisely the trace-log factor. Repeated vertices and edges are allowed. No simple-cycle approximation is being made. A term reads only the exterior edges on its walk and the source weights on plaquettes incident to its visited vertices. Including those neighboring source anchors enlarges its connected carrier by at most a fixed factor of its walk length.

For real positive weights and real T, every term is nonnegative, because an orthogonal adjoint matrix has trace at most d_A. In particular Γ_T(0)≥0. For complex weights or a complex exterior chart, termwise positivity is not asserted.

Let a_γ be the summand in (W.8), including 1/(2m). The path estimate (W.4), the doubled domains (W.7), and the bound ||R_γ||≤exp(C_Nεm) imply, for some fixed κ>0,

\[
 \sup_{x\in D}\ 
 \sum_{m\ge1}\ \sum_{\gamma:x_0=x,\ |\gamma|=m}
       e^{\kappa m}|a_\gamma(z,T)|
 \le C_{N,M}.
 \tag{W.9; P}
\]

Indeed, after dropping the return restriction, the sum of the absolute scalar path weights is at most C_M[(1+r)/(1−r)]ᵐρ_Mᵐ. Multiplying by the adjoint trace bound still leaves an exponential margin by (W.7). The resulting geometric series proves (W.9). The constants and domains do not deteriorate as D grows.

Subtract the same exterior-free source vacuum at every T:

\[
 L_D^{\rm G}(z)=\log\frac{Z_1^{\rm G}(z)}{Z_1^{\rm G}(0)},
 \qquad
 \Phi_T^{\rm G}(z)=
 \log\frac{Z_T^{\rm G}(z)}{Z_T^{\rm G}(0)}-L_D^{\rm G}(z)
 =-\Gamma_T(z)+\Gamma_T(0).
 \tag{W.10; P}
\]

Thus the source-dependent exterior activity is exactly the difference of the weights in each loop of (W.8). The adjoint holonomy is not replaced by an identity-valued counterterm. Applying Cauchy's formula on the doubled source domain in the Banach space of the rooted sums in (W.9) gives, after reducing κ if necessary,

\[
 \begin{aligned}
 \|\Phi_T^{\rm G}(z)\|_{\rm loop,\kappa}
     &\le C_{N,M}\|z\|_\infty/\tau,\\
 \|D_z^q\Phi_T^{\rm G}(0)[f_1,\ldots,f_q]\|_{\rm loop,\kappa}
     &\le q!C_{N,M}^{q+1}\tau^{-q}
                     \prod_{i=1}^q\|f_i\|_\infty,\qquad q\ge1.
 \end{aligned}
 \tag{W.11; P}
\]

Here the norm means the supremum of the rooted absolute sums of the displayed loop decomposition, not the absolute value of the full determinant divided by the number of sites. Mixed field derivatives also obey Cauchy bounds on the fixed inner exterior chart. A field derivative can act only on an edge actually read by the walk; a source derivative can act only at an incident plaquette. These support statements follow directly from (W.8), before any estimate.

The literal P2 source conversion is exact: z=N j and τ=Nβ. Consequently the q-th literal source derivative has β⁻ᑫ, with the factors N canceling. This fact does not authorize replacing a general renormalized old source by a fresh plaquette source.

## 4. The exterior-curvature carrier and winding remainder

For a transverse plaquette f, let s_f(T)=N−Re Tr T_∂f. This is the literal Wilson action of a plaquette made entirely of exterior links. Give vertices, edges and plaquettes their nearest-neighbor torus distances, allowing a fixed additive difference between these choices.

For any G∈SU(N), the adjoint character identity and the Hilbert–Schmidt identity give

\[
 \begin{aligned}
 d_A-\operatorname{tr}_{\rm Ad}\operatorname{Ad}G
 &=N^2-|\operatorname{Tr}G|^2
 \le 2N\{N-\operatorname{Re}\operatorname{Tr}G\},\\
 \|G-I\|_{\rm HS}^2&=2\{N-\operatorname{Re}\operatorname{Tr}G\}.
 \end{aligned}
 \tag{W.12; P}
\]

The character identity follows by decomposing the conjugation action on all complex N×N matrices into its scalar and traceless parts. The first inequality follows from |Tr G|²≥(Re Tr G)² and N+Re Tr G≤2N.

Lift a nonwinding closed lattice walk γ of length m to the cubic lattice. Its word in the six coordinate steps has total displacement zero. Interchanging adjacent steps in different coordinate directions reduces the word to grouped coordinate steps, after which neighboring inverse steps cancel. There are at most m² such interchanges. Each interchange inserts a conjugate of one oriented elementary plaquette holonomy; all these plaquettes lie within distance m of the root. Thus the loop holonomy is a product of at most m² conjugated elementary holonomies. The telescoping product inequality and Cauchy–Schwarz prove

\[
 d_A-\operatorname{tr}_{\rm Ad}R_\gamma
 \le C_Nm^4
       \sum_{\substack{f\\\operatorname{dist}(x_0,f)\le m+C}}
                         s_f(T).
 \tag{W.13; P: real exterior, nonwinding walk}
\]

Repeated filling plaquettes cause no difficulty: bounding their multiplicity by the total number of interchanges explains the deliberately generous m⁴. This proof does not assume a small exterior curvature and does not choose logarithms of plaquette matrices. The filling is used to bound the activity; its functional dependence remains the original walk dependence in (W.8).

A winding walk has length at least n. Its character defect is at most 2d_A, so the exponential walk estimate bounds all winding terms rooted at x by C exp(−cn). Combining the two cases gives

\[
 \begin{aligned}
 \sum_{\gamma:x_0=x}|a_\gamma(z,T)|
 &\le C\sum_f e^{-c\,\operatorname{dist}(x,f)}s_f(T)
          +Ce^{-cn},\\
 0\le\Gamma_T(0)
 &\le C\sum_f s_f(T)+C|D|e^{-cn}.
 \end{aligned}
 \tag{W.14; P}
\]

The first inequality holds for real T and complex sources throughout a smaller fixed disk. The constants depend only on N and M. To prove it, multiply (W.13) by the absolute scalar walk weights and sum lengths m. The polynomial m⁴ is paid by a portion of the exponential margin. Summing x then uses the uniform bound on the number of torus sites at a given distance from a plaquette. No volume factor remains in front of the curvature sum.

The same argument followed by Cauchy's formula proves, for q≥1,

\[
 \begin{aligned}
 |\Phi_T^{\rm G}(z)|
 &\le {C\|z\|_\infty\over\tau}
             \left\{\sum_f s_f(T)+|D|e^{-cn}\right\},\\
 |D_z^q\Phi_T^{\rm G}(0)[f_1,\ldots,f_q]|
 &\le q!C^{q+1}\tau^{-q}\prod_i\|f_i\|_\infty
             \left\{\sum_f s_f(T)+|D|e^{-cn}\right\}.
 \end{aligned}
 \tag{W.15; P}
\]

This is the growing-patch replacement for an internal-minimum-only bound. The minimum of (W.1) is always zero; the right-hand side correctly retains surrounding curvature and the possible flat torus holonomies. If all exterior plaquettes are flat, the latter can still affect the determinant, but only through the proved winding remainder.

For an application at every four-dimensional scale h_k, choose the admitted cofinal subfamily with T/ℓ₀ a multiple of 2M. Then every n_k=T/h_k is a multiple of M and at least 2M, so the same pin geometry exists at each scale. One may sum the estimate over the longitudinal slabs. The resulting winding cost is bounded by C N_k exp(−cT/h_k). With h_k=Lᵏa, a=L⁻ᴷℓ₀ and T≥2ℓ₀, it obeys

\[
 \sum_{k=0}^{K}N_k e^{-cT/h_k}
 \le N_T\sum_{r=0}^{K}L^{4r}e^{-2cL^r}
 \le C_{c,L}N_T .
 \tag{W.16; P}
\]

The numerical inequality (W.16) itself holds whenever T≥2ℓ₀; applying this patch construction additionally requires its pin geometry. This physical-volume statement applies to the winding remainder. It does not replace the curvature term in (W.15) by an identity or give the full interacting vacuum subtraction.

## 5. Local marked carriers and exact constant-source cancellation

The curvature bound can retain the location of a source mark. Let q be one affected plaquette, equivalently one edge of the transverse graph, including an edge to a pin. Differentiating its occurrence in the numerator and in the incident row denominators of ω_γ gives

\[
 |\partial_{z_q}\omega_\gamma|
 \le {C\over\tau}|\omega_\gamma|
       \sum_{i=0}^{m-1}1_{\{x_i\text{ is an endpoint of }q\}} .
 \tag{W.17; P}
\]

This is valid throughout the smaller complex source disk; all w_e and d_x(w) stay uniformly away from zero. There is no derivative of an exterior plaquette matrix here.

Cyclically re-rooting the trace walk cancels the factor m from the sum in (W.17) against the 1/m in (W.8). More explicitly, after summing all rooted walks of length m, each of the m possible positions of the marked endpoint gives the same sum of loops rooted at an endpoint of q. The scalar product ω_γ and the holonomy trace are invariant under that cyclic change. There are at most two such endpoints. The curvature-filling argument of §4, now rooted at q, therefore proves

\[
 |\partial_{z_q}\Gamma_T(z)|
 \le {C\over\tau}\left\{
       \sum_f e^{-c\,\operatorname{dist}(q,f)}s_f(T)+e^{-cn}\right\}.
 \tag{W.18; P: real exterior, complex source}
\]

Integrating along t↦tz gives the stronger support-sensitive estimate

\[
 |\Phi_T^{\rm G}(z)|
 \le {C\over\tau}\sum_q|z_q|
       \left\{\sum_f e^{-c\,\operatorname{dist}(q,f)}s_f(T)+e^{-cn}\right\}.
 \tag{W.19; P}
\]

Applying directional Cauchy estimates to (W.18), and using a fixed fraction of the available disk, gives for q≥1 the polarized version

\[
 \begin{aligned}
 |D_z^q\Phi_T^{\rm G}(0)[f_1,\ldots,f_q]|
 \le {}&q!C^{q+1}\tau^{-q}
           \prod_{i=2}^q\|f_i\|_\infty\\
 &{}\times\sum_e|f_1(e)|
       \left\{\sum_f e^{-c\,\operatorname{dist}(e,f)}s_f(T)+e^{-cn}\right\}.
 \end{aligned}
 \tag{W.20; P}
\]

Any slot can be chosen as the localized one, by symmetry of derivatives. The factorial follows from the ordinary multivariable Cauchy formula with radii proportional to 1/q; qᑫ is bounded by eᑫq!, so the loss is one fixed factorial order.

There is also an exact useful cancellation. If every affected plaquette has the same source z_e=t, then H_T(w)=(1−t/τ)H_T and the same factor multiplies the flat Hessian. The ratio of their determinants is unchanged. Equivalently every factor w_e/d_x(w) in the loop expansion equals 1/6. Hence

\[
 \Gamma_T(t1)=\Gamma_T(0),\qquad
 \Phi_T^{\rm G}(t1)=0 .
 \tag{W.21; P}
\]

Only a simultaneous constant change of all affected weights is covered by (W.21). It is not a statement that individual spatial derivatives or field-valued contact terms vanish. Nor is it the derivative of a full nonlinear sourced background family: the exterior and the Gaussian expansion point have been held fixed exactly as specified in §1.

## 6. What is completed, and what R1/R2 still require

**Completed theorem.** Equations (W.8)–(W.11) give an explicit local, holomorphic, exponentially summable activity representation for the actual Gaussian Hessian of arbitrarily large periodically pinned parallel-link Wilson patches. Equations (W.14)–(W.20) identify and bound their exterior-curvature carriers, keep every spatial source anchor, and control all source orders. Equation (W.16) pays their torus winding terms by physical volume. All constants are independent of the number of integrated links, the torus size, and the real exterior connection.

This closes the growing-geometry Gaussian version of the cyclic issue exhibited by the four-link example. It supplies concrete activities and their domains, rather than a rank estimate or a repetition of a fixed-dimensional Laplace approximation.

**Why this is useful for the next mixed step.** The loop formula makes the relevant output visible. It depends on exterior links even though the internal minimum is zero. Its real bound is paid by exterior plaquette curvature; its analytic norm is controlled by the killed-walk gap. A valid mixed transition must carry this output in its field-valued activity ledger, project the relevant dimension-four part when appropriate, and assign its carrier to an actual reserve. The source-free scalar vacuum L_D^G and the exterior response Φ_T^G are explicitly different terms.

**What is not completed.** A general constrained Balaban Gaussian uses its actual averaging/gauge constraint rather than the periodic pins in this theorem. Its admission must be checked in its own norm. More importantly, the compact-group integral has higher-order terms, old analytic E/B activities, hard selectors, boundary-crossing source readouts, and a history-dependent geometry. None of those is removed by the Gaussian calculation.

The exact remaining nonlinear statement is therefore

\[
 \begin{gathered}
 \text{The full mixed kernel, after its prescribed identity and}\\
 \text{dimension-four extractions, has a common local analytic/raw norm}\\
 \text{with bounds uniform in the entire constrained history.}
 \end{gathered}
 \tag{W.22; O: remaining R1 application}
\]

For R2, the curvature sum in (W.19) must be integrated under the same complete physical exterior law, after the appropriate local extractions. Its bare expectation can count fine plaquettes. The theorem does not convert that count into a physical-cell estimate simply because its coefficient is β⁻¹:

\[
 \text{A physical-cell bound for the complete normalized, locally
 renormalized source remains to be proved.}
 \tag{W.23; O: remaining R2 application}
\]

The proof makes no new assumption about N2-F. Its source normalization is the P2 normalization stated in §1. Its restricted geometry is explicit. It can be reused as a checked component of a larger construction, but it is not a proof of the full R1 or R2 statements.
