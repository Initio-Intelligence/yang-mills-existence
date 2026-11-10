# Exterior holonomy in a cyclic patch

## 1. Exact scope and an actual lattice realization

This note gives a counterexample to extending the all-real acyclic patch theorem using only the minimum energy of the plaquettes incident to the integrated links. It is an actual SU(2) Wilson conditional integral, with four integrated links. It is not a counterexample to R1, R2, N1-S, or Yang–Mills existence. Its conclusion is that a subsequent induction must retain the exterior curvature/holonomy carrier and its determinant activity.

Use normalized trace tr=Tr/2 and a(P)=1−Re tr P. The literal preamble action is s(P)=2a(P), and its coefficient is τ=2β. Work in fine lattice units on a periodic lattice with n≥3 sites per direction. Let e_1,…,e_4 be the coordinate vectors. Integrate the four positive direction-1 links starting at

\[
 x_0=0,\qquad x_1=e_2,\qquad
 x_2=e_2+e_3,\qquad x_3=e_3.
 \tag{C.1; P: the four-link cyclic patch}
\]

Their internal link matrices are Q_0,…,Q_3. Fix every other direction-1 link to I. Choose a noncentral g∈SU(2). Set the exterior direction-2 links starting at t e_1 equal to g for every t modulo n; set all other exterior links to I. Thus the exterior transverse connection is independent of x_1, and its holonomy around the displayed transverse square is g.

For two neighboring patch sites x,y=x+e_ν, ν=2,3, their shared plaquette is exactly

\[
 P_{1\nu}(x)=Q_x A_{xy}Q_y^{-1}A_{xy}^{-1},
 \qquad A_{xy}=U_\nu(x)=U_\nu(x+e_1).
 \tag{C.2; P}
\]

Along the cycle 0→1→2→3→0 the four transports can be taken as g,I,I,I. Reversing an edge inverts its transport and its plaquette, which does not change a. Each patch link shares exactly two plaquettes with another patch link, and has four other incident plaquettes. Those other plaquettes contain one patch link and one identity direction-1 link; their actions are a(Q_i), by conjugation and inversion invariance. No plaquette contains three patch links. Thus there are four shared and sixteen single-link plaquettes, for twenty distinct affected plaquettes in total.

The exact conditional phase, with no factors discarded, is

\[
 S_g(Q)=4\sum_{i=0}^3a(Q_i)
     +\sum_{\{i,j\}\in C_4}
          a(Q_iT_{ij}Q_j^{-1}T_{ij}^{-1}),\qquad
 Z_g(\tau)=\int_{SU(2)^4}e^{-\tau S_g(Q)}\,dQ.
 \tag{C.3; P}
\]

The edge labels T are the transports just described, with cycle holonomy g. The exterior-only plaquettes remain in the outer Wilson law; they are not part of this conditional phase. At Q_i=I every affected plaquette is I, irrespective of g. Nonnegativity and the sixteen pinning terms therefore give

\[
 m_g:=\min_Q S_g(Q)=0,\qquad
 Q_0=Q_1=Q_2=Q_3=I
       \text{ is its unique minimum}.
 \tag{C.4; P}
\]

The same lattice patch with every exterior link I has phase S_0 and integral Z_0. It is the flat comparison used below. Unlike an acyclic star, the twisted cycle cannot have all its transports removed by one independent conjugation at each internal vertex: their product retains Ad(g).

**Related result.** Uniform cyclic Gaussian carriers ([cyclic_carriers.md](cyclic_carriers.md)) extends the Gaussian exterior-carrier argument to arbitrarily large parallel-link Wilson patches with a fixed periodic pin grid. It gives a common analytic domain, exact local loop activities, source jets, curvature carriers and a physical-volume winding estimate. The fixed-patch nonlinear theorem below remains distinct: a uniform compact-group or general constrained-history extension is not claimed from the Gaussian result.

## 2. Exact Hessian determinant and the nonzero flat-relative vacuum

Use anti-Hermitian coordinates X_i with inner product −tr(X_iX_j), so a(e^X)=|X|²/2+O(|X|⁴). At the minimum the phase has quadratic part

\[
 \frac12\left[
       4\sum_i|X_i|^2+
       \sum_{\{i,j\}\in C_4}
                  |X_i-\operatorname{Ad}(T_{ij})X_j|^2\right].
 \tag{C.5; P}
\]

Its real twelve-dimensional Hessian is H_g=6I−A_g, where A_g is the cycle adjacency matrix with its orthogonal adjoint transports. The norm of A_g is at most two: on each edge 2|⟨X_i,RX_j⟩|≤|X_i|²+|X_j|², and every vertex has degree two. Thus H_g≥4I for every g. Also S_g≥4Σ_i a(Q_i), so there is a fixed positive global gap away from the unique identity minimum. The normalized Haar density is smooth and positive there.

Conjugations at three vertices reduce three transports to I, leaving the fourth equal to Ad(g). Write the three complex eigenvalues of Ad(g) as 1,e^{iθ},e^{-iθ}, with 0<θ≤π for a nontrivial adjoint holonomy. On the eigenspace of phase e^{iφ}, the four adjacency eigenvalues are 2cos((2πk+φ)/4), k=0,1,2,3. This follows by solving the four-step plane-wave recurrence with twisted closing condition e^{4ip}=e^{iφ}.

Let P(t)=t⁴−4t² and q=2−2cosθ>0. Multiplying these four eigenvalue factors gives

\[
 \prod_{k=0}^3
  \left[t-2\cos\frac{2\pi k+\phi}{4}\right]
     =2\{T_4(t/2)-\cos\phi\}
     =P(t)+2-2\cos\phi,
 \quad T_4(u)=8u^4-8u^2+1.
 \tag{C.6; P}
\]

Therefore, with P(6)=1152,

\[
 \det H_g=P(6)[P(6)+q]^2,\qquad
 \det H_0=P(6)^3,\qquad
 \frac{\det H_g}{\det H_0}
    =\left(\frac{1154-2\cos\theta}{1152}\right)^2>1.
 \tag{C.7; P}
\]

The ordinary finite-dimensional Laplace estimate applies to both exact compact integrals: expand at the unique minimum, integrate the positive Gaussian Hessian, and bound the complementary integral by the fixed gap. The odd cubic term integrates to zero against the even Gaussian; the next terms give relative O(τ⁻¹). Their common Haar-density factor and common twelve-dimensional scaling τ⁻⁶ cancel. Thus

\[
 \Gamma_g(\tau):=\log Z_0(\tau)-\log Z_g(\tau)
     =\frac12\log\frac{\det H_g}{\det H_0}+O(\tau^{-1})
     \longrightarrow
       \log\frac{1154-2\cos\theta}{1152}>0.
 \tag{C.8; P}
\]

For example g=iσ_3 has θ=π and the limit is log(1156/1152). Consequently there is no estimate Γ_g(τ)≤Cτm_g for this family, for any finite C: its right side is identically zero. The contradiction already occurs at four integrated links, with a strictly positive Hessian and no unresolved stationary-phase or zero-mode issue.

## 3. A nonzero inherited source term at zero internal minimum energy

The same example also defeats a bound |Φ_g(z)|≤Cm_g|z| for arbitrary independent plaquette coefficients. Choose one pinning plaquette at each vertex: explicitly use the four positive (1,4)-plaquettes based at the four sites in (C.1). They are distinct, each contains exactly its one internal link Q_i, and all their exterior links are I. Their actions are exactly a(Q_i). Give these four plaquettes the common normalized source z, keeping every other affected source zero. Define

\[
 \begin{aligned}
 Z_g(\tau,z)&=\int
       e^{-\tau S_g(Q)+z\sum_i a(Q_i)}\,dQ,\\
 \Phi_g(\tau,z)&=
       \log\frac{Z_g(\tau,z)}{Z_g(\tau,0)}
        -\log\frac{Z_0(\tau,z)}{Z_0(\tau,0)}.
 \end{aligned}
 \tag{C.9; P: actual pinning-plaquette source and flat subtraction}
\]

This is an allowed direction in the independent-plaquette source family of the finite-patch admission theorems. It is not an identification of this selective source with one isotropic scalar source at those sites.

The source leaves the critical point at the identity and changes the Hessian to H_g(t)=tI−A_g with t=6−z/τ. A fixed complex neighborhood of t=6 has a positive real quadratic reserve. The centered compact Laplace proof is therefore uniform and holomorphic in t. Its logarithmic remainder and its first t derivative are O(τ⁻¹). Differentiating with respect to z costs a further factor τ⁻¹, giving

\[
 \begin{aligned}
 \partial_z\Phi_g(\tau,0)
    &=\frac1{2\tau}
       \{\operatorname{Tr}H_g^{-1}-\operatorname{Tr}H_0^{-1}\}
                       +O(\tau^{-2})\\
    &=-\frac{qP'(6)}
       {\tau P(6)[P(6)+q]}+O(\tau^{-2}),
       \qquad P'(6)=816.
 \end{aligned}
 \tag{C.10; P}
\]

Here Tr is the ordinary matrix trace on the twelve real fluctuation coordinates. The second equality follows by differentiating
log(det H_g(t)/det H_0(t))=2log[(P(t)+q)/P(t)].
The leading coefficient is strictly negative when q>0, so the derivative is nonzero for sufficiently large τ. The internal source-zero minimum remains m_g=0. Thus a flat-subtracted source bound with the sole majorant m_g would incorrectly force Φ_g to vanish identically.

This source term is an exterior-holonomy-dependent determinant response. It is not an identity counterterm: it varies with the retained exterior g. In particular a deterministic source-only vacuum cannot remove it on all exteriors.

## 4. The correct implication for the next induction

The acyclic star theorem remains valid. Its normal form can remove every edge transport, and zero internal minimum energy then makes the entire sourced kernel literally flat. The cyclic patch has a gauge-invariant product of transports; it survives every internal change of variables and changes the fluctuation determinant even when all affected plaquettes can simultaneously be flat.

The full surrounding Wilson field is not flat in this example. The transverse (2,3)-plaquette based at the origin has holonomy g and belongs to the exterior, so its action can pay for the new interaction in a larger, correctly assigned carrier. For g=exp(iθσ_3/2),

\[
 q=2-2\cos\theta
       =4(1-\cos(\theta/2))(1+\cos(\theta/2))
       \le8a(g).
 \tag{C.11; P}
\]

Thus the obstruction does not contradict a bound by a suitable collar curvature budget. It shows that the carrier must actually include that exterior curvature and that the associated determinant/source term must be retained and projected. The actual Wilson energy theorem controls such surrounding bare budgets once they have been assigned; it does not assign them or classify their dimension-four projection by itself.

**Corollary 4.1 (P: the correct exterior-curvature carrier for this fixed family).** For the exact twenty-plaquette family (C.3), let g vary over all SU(2), and give its plaquettes independent normalized sources z_p. There are fixed τ_*,c,C>0 such that, for τ≥τ_*,

\[
 |\Gamma_g(\tau)|\le Ca(g),\qquad
 |\Phi_g(\tau,\mathbf z)|
       \le C a(g)\frac{\|\mathbf z\|_1}{\tau}
       \quad(\|\mathbf z\|_1<c\tau).
 \tag{C.12; P: exterior-curvature admission for the pinned cycle}
\]

Here Φ is the actual logarithmic source quotient with the same source array's flat g=I quotient subtracted. It is holomorphic on the displayed source ball. Its derivatives obey

\[
 |D_{\mathbf z}^{\,m}\Phi_g(\tau,0)
                 [f^1,\ldots,f^m]|
       \le m!C^{m+1}a(g)\tau^{-m}
                         \prod_{r=1}^m\|f^r\|_1,\qquad m\ge1.
 \tag{C.13; P}
\]

**Proof.** Give all twenty plaquette actions real weights w_p near one. The four positive pinning sums make Q=I the unique minimum, still of energy zero, for every g. The weighted Hessian has a uniform positive lower bound, and the pinning terms give a uniform global gap. The phase and its derivatives are uniformly bounded on the compact real g family. Extend g to a small complex neighborhood and w to a fixed complex neighborhood of one. The critical point stays I exactly, because the differential of each a^hol at I vanishes. The phase perturbation has zero value and first derivative there, so a uniform C² estimate, the local quadratic bound, and the global pinning gap preserve complex coercivity on a common domain.

The compact holomorphic Laplace proof therefore gives
log Z_g(τ,w)=−6log τ+log A_g(w)+ρ_g(w,τ), with A_g bounded away from zero and ρ_g=O(τ⁻¹), uniformly with fixed-margin w derivatives. Near g=I write g=e^X. Simultaneous conjugation of g and all internal variables leaves each weighted phase invariant. The flat-relative log determinant and remainder vanish at X=0 and have no invariant linear X term. Their bounds are consequently Ca(g) and Ca(g)/τ, respectively, including fixed-margin w derivatives. Away from a small identity neighborhood, a(g) has a positive lower bound, so the uniform compact-family estimates give the same conclusions. No such flatness is required near g=−I.

Subtract the g=I factorization to prove the Γ bound. For the source quotient put w=1−z/τ. Its two flat-relative determinant/remainder differences are bounded by their first w derivatives times ‖z‖₁/τ. This proves (C.12), and fixed-domain Cauchy gives (C.13). ∎

This corollary proves an exterior-curvature estimate for the same fixed pinned family, rather than only ruling out the internal-minimum estimate. Its constants are uniform in g and τ above threshold. It does not extend to arbitrary cyclic graphs, large patches or compulsory internal constraints, which may lack its uniform pinning gap.

Accordingly the next source-carrying step requires more than repeating the finite star minimum-energy inequality. It must keep holonomy-dependent fluctuation activities, their physical source derivatives, their exterior carriers, and their local identity versus field-valued projections. The completed positive raw-density transport theorem preserves an available integrated budget but cannot erase these outputs.

**Status:** all formulas (C.1)–(C.13) are proved finite-lattice statements. The result rules out a ground-energy-only flat-vacuum extension of the acyclic argument and proves the correct exterior-curvature replacement for this fixed family. It leaves full R1, full R2 and the Yang–Mills target untouched, while identifying an explicit additional activity that any extension of the argument must handle.
