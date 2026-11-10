# What a uniform-depth Q-core certificate must retain

This note examines an iteration of the CA and TD proofs. It does not modify either proof or claim that their fixed-depth constants are uniform in the number of blockings. Two results below are exact: a trace/operator-norm bound for one normalized Gaussian comparison, and preservation of a born flat Gaussian innovation under arbitrary later reweighting. They identify a concrete way to avoid spending the same birth tail repeatedly. The corresponding nonlinear, common-carrier comparison is not yet proved.

## 1. Birth budget, final footprint, and the actual repeated bound

Let a Q defect be born at level k, with normalized radius P_k and n defect occurrences. A stored QC/TD payload has a bound of the form

\[
 A_X\exp(\eta_0 r_0)\exp(-c_0 nP_k^2),
 \tag{UD.1}
\]

with strict Gaussian and spatial margins. Here r_0 is its actual old marginal rank, including distinct latent copies in a logarithmic product. It is not the cardinality of the current core.

The geometric result CGD.2--CGD.7 gives, with h_{j+1}=Lh_j,

\[
 r_{j+1}^{\rm core}\le L^{-1}r_j^{\rm core}
                         +C_L(R_{j+1}+m+1),\qquad
 |K_N^{\rm core}|\le C_L nR_N^4\le C'_L nR_k^4.
 \tag{UD.2}
\]

All actual frame and Q-reference inputs are retained. Only analytic connectors receive fixed collars. Thus one birth reserve can pay the *final* core-volume weight uniformly in age. It does not pay a new copy of that volume every time an absolute integral estimate is used.

For comparison, the displayed CA estimates introduce

\[
 \delta_j=C(u_{m_j}+q_j),\qquad
 q_j=C_L(\epsilon_{j+1}+g_jP_{Q,j}),
 \tag{UD.3}
\]

for an old normalized covariance, and a new frame displacement

\[
 a_j\le C_L{\epsilon_{j+1}\over g_j}e^{-cR_{j+1}}.
 \tag{UD.4}
\]

In the two-step proof the buffers are fixed and then the coupling is made small; delta_j is small, not shown summable in j. CA.20 gives a rank factor and a quadratic tilt. CA.23 gives another small rank tilt and, after replacing a_j by a fixed ceiling, a factor exp(C|S_j|). CA.6 also spends part of the analytic carrier rate through exp(Cq_j|X_j|).

If these absolute comparisons are successively composed in a common old energy coordinate, their literal ledger has the form

\[
 t_{k,N}=t_{k,k}+
       C\sum_{j=k}^{N-1}\delta_{k,j},
\]
\[
 \mathcal L_{k,N}=
 C\sum_{j=k}^{N-1}\delta_{k,j}r_{k,j}^{\rm latent}
 +C\sum_{j=k}^{N-1}|S_j|
 +C\sum_{j=k}^{N-1}q_j n(X_j)
 +\text{the explicitly retained current costs}.
 \tag{UD.5}
\]

Here t is the positive tilt spent in the stored Gaussian energy, and exp(L) is the resulting amplitude loss. The subscripts k,j allow for the correctly transported birth coordinates; their equivalence is itself required before using this formula. Every latent rank remains explicit. Equation (UD.5) describes the bound obtained if the available comparison inequalities can be applied at each step. It is not an established admissibility theorem for arbitrarily many steps.

Even a constant small delta and a bounded nonzero current core give losses growing with N. Once t reaches the original reserve, that comparison proof stops. A positive spatial weight may telescope along a fixed lineage; none of the nonnegative sums in (UD.5) thereby telescopes. The fixed fraction of spatial rate discarded in a two-level proof also cannot be discarded infinitely often.

This is a limitation of the displayed bounds, not a lower bound on the true physical losses.

## 2. An exact Gaussian comparison with trace cost counted once

Let Sigma_0 be a real positive covariance on a finite physical/gauge-fixed coordinate space. Let Sigma be a complex symmetric covariance, and put

\[
 E=\Sigma_0^{-1/2}(\Sigma-\Sigma_0)\Sigma_0^{-1/2},
 \qquad \|E\|_{\rm op}\le\delta<1/4.
 \tag{UD.6}
\]

Use the analytic determinant branch continuing from Sigma_0. The same Sigma defines the inverse in the quadratic form and the determinant. Write ||.||_1 for the trace norm.

### Lemma UD.1

The normalized densities satisfy, for real x,y,

\[
 |p_\Sigma(x+iy)|\le p_{\Sigma_0}(x)
   \exp\!\left\{C\|E\|_1+
      C\delta|\Sigma_0^{-1/2}x|^2+
      C|\Sigma_0^{-1/2}y|^2\right\}.
 \tag{UD.7}
\]

A real frame displacement v can also be included, at the cost

\[
 C\tau|\Sigma_0^{-1/2}x|^2+
 C(1+\tau^{-1})|\Sigma_0^{-1/2}v|^2
 \tag{UD.8}
\]

in the exponent, for any fixed small positive tau. No rank factor is necessary if the trace norm is known directly.

**Proof.** The convergent matrix logarithm gives

\[
 |\log\det(I+E)|
 \le\sum_{m\ge1}{|\operatorname{Tr}E^m|\over m}
 \le{\|E\|_1\over1-\delta}.
 \tag{UD.9}
\]

Indeed ||E^m||_1<=delta^{m-1}||E||_1. Also
||(I+E)^{-1}-I||_op<=delta/(1-delta).
After setting x_0=Sigma_0^{-1/2}x and y_0=Sigma_0^{-1/2}y, expand the quadratic at x_0+iy_0. The reference real part is |x_0|^2-|y_0|^2; the inverse discrepancy is bounded by C delta(|x_0|^2+|y_0|^2). The determinant contributes half of (UD.9). This proves (UD.7). The real cross term with v is bounded by Young's inequality, proving (UD.8). ∎

The usual estimate exp(C delta r) is the special case ||E||_1<=r delta. Keeping the trace norm can be strictly better, particularly when only a small part of a large old space is changed.

For a differentiable family with Sigma_0 fixed in these coordinates, the determinant and inverse responses are exactly

\[
 d\log\det(I+E)=\operatorname{Tr}[(I+E)^{-1}dE],
 \qquad
 d(I+E)^{-1}=-(I+E)^{-1}(dE)(I+E)^{-1}.
 \tag{UD.10}
\]

They are controlled respectively by C||dE||_1 and C||dE||_op. A changing real reference also has its own explicit derivative; (UD.10) does not erase it. These identities give the correct matrix targets for once-current estimates.

### What really telescopes

For positive precisions on the same coordinates,

\[
 {p_{K_N}(z)\over p_{K_k}(z)}
 =\left({\det K_N\over\det K_k}\right)^{1/2}
                   \exp[-\tfrac12z^{\mathsf T}(K_N-K_k)z].
 \tag{UD.11}
\]

This is an exact identity. If all intermediate integrations are exact Schur eliminations of one joint Gaussian, their determinant normalizations agree with a single simultaneous elimination, by NE.6. Thus one should estimate the *final* relative covariance in (UD.6), instead of multiplying a fresh absolute majorant at every step.

This cancellation requires a common joint measure and coordinate identification. A series of separately normalized reference kernels with different cutoffs, gauge sections or omitted cross terms does not satisfy it merely because all of them have a gap.

If a common covariance path is available, a sufficient summability condition is

\[
 \sum_{j=k}^{N-1}
 \|\Sigma_0^{-1/2}(\Sigma_{j+1}-\Sigma_j)\Sigma_0^{-1/2}\|_{\rm op}
       \le\delta_*,
\]
\[
 \sum_{j=k}^{N-1}
 \|\Sigma_0^{-1/2}(\Sigma_{j+1}-\Sigma_j)\Sigma_0^{-1/2}\|_1
       \le T_k.
 \tag{UD.12}
\]

Then (UD.7) costs exp(CT_k) and one tilt C delta_*, independently of N. This condition is sufficient, not necessary: the final signed matrix difference can be smaller than the sum of increment norms.

## 3. The flat source has an exact joint birth certificate

This part needs no assumed nonlinear age decay.

Let A be one centered physical Gaussian field after the fixed terminal constraints and gauge null directions have been removed. Let F_j be its nested linear readout sigma-algebras, F_j containing F_{j+1}. Put

\[
 P_jA=\mathbb E[A\mid F_j],\qquad
 Y_j=(P_j-P_{j+1})A.
 \tag{UD.13}
\]

Each Y_j is independent of F_{j+1}, and distinct Y_j are independent. This follows because the conditional-mean projections are nested energy-orthogonal projections and all cross covariances vanish. Equivalently, it follows by exact Schur square completion.

For every nonnegative integrable weight w measurable with respect to F_{k+1}, the normalized law proportional to w times the joint Gaussian has **the same** marginal law of Y_k. Therefore any later weights depending only on the later readouts, including hard masks on those readouts, spend no new determinant or quadratic reserve of this born innovation. The statement does not apply to a weight that itself reads Y_k.

In the actual flat ordinary source coordinates, IG.1--IG.9 identifies these innovations and gives their native precision the uniform gap c_L. The source normalized soft-gauge samplers are included as independent Gaussian coordinates with their own costs. A compact gauge variable is not silently identified with a positive Gaussian mode. Every untruncated retained Schur marginal has the same gap. Consequently the Gaussian bound for n born large-fluctuation slots remains

\[
 C^n\exp(-c nP_k^2)
 \tag{UD.14}
\]

under arbitrarily many later Gaussian readouts and later-only weights. There is no constant per depth. The original cutoff-completion or born defect domains, when present, stay in the old insertion; their Gaussian energy is not deleted.

There is also a simple exact nonlinear disintegration fact. If an original birth conditional kernel q_k(du|v) is kept, a later weight that depends only on v does not change that conditional kernel. If an old conditional payload H(v) has a uniform bound epsilon on every v in the later physical support, any normalized later mixture still has value at most epsilon. This is ordinary positivity/Fubini and costs no inverse rare-event mass. It does not by itself localize H in the current raw field, control its currents or logarithmic connected expansion, or pay the number of birth positions per later anchor.

Thus the problem is not an inevitable repeated loss in the exact physical integral. It is construction of a common localized nonlinear certificate that preserves this cancellation.

## 4. Sharpening the frame cost

The factor exp(C|S_j|) in CA.23 can be sharpened without any new source estimate. Its derivation only used

\[
 \|A_s-B\|_2^2\le C a_j^2|S_j|,
 \qquad
 |\log\det DA_s|\le C g_j a_j|S_j|.
\]

Use Young's parameter zeta_j rather than a fixed parameter. The new tilt can be restricted to a subspace of rank at most the number s_j of real coordinates in S_j. To see this, whiten the positive reference Gaussian and let E_S be the range of K_0^{1/2}P_{S_j}. Since the displacement is supported in S_j, its reference quadratic cross term pairs only with the orthogonal projection of the whitened variable onto E_S. Young's inequality therefore spends zeta_j on that projection, rather than on all old latent coordinates. After any already admitted small Gaussian tilt, the covariance of this projection is still uniformly bounded. Its normalized exponential integral costs exp(C zeta_j s_j).

Consequently the displacement contributes a determinant/quadratic-integral cost of the form

\[
 C\left(\zeta_j s_j+
        (1+\zeta_j^{-1})a_j^2|S_j|
              +g_j a_j|S_j|\right).
 \tag{UD.15}
\]

The separate complex covariance discrepancy still has its own rank or trace cost. The displayed improvement concerns the frame cross term only. Since s_j is at most a fixed Lie-algebra multiplicity times |S_j|, choosing zeta_j comparable to a_j gives a cost C a_j|S_j| for small a_j, even if the old latent rank is much larger. No old latent rank has been bounded by the current core size.

This proves that a fixed C|S_j| loss need not be paid at every step. It does **not** prove that the remaining actual sequence of frame costs is summable.

A useful conditional arithmetic statement is precise. Suppose, in addition to the available source bounds, one has a two-sided speed estimate

\[
 c_-(N-j)+g_N^{-2}
 \le g_j^{-2}
 \le c_+(N-j)+g_N^{-2}.
 \tag{UD.16}
\]

For r>1, every sum of
g_j^{-A}(1+\log g_j^{-2})^B exp[-c(\log g_j^{-2})^r]
is then uniformly finite over all ultraviolet ages and tends to zero as the final weak ceiling tends to zero, for fixed A,B,c. Compare it with the integral in x=g_j^{-2}; the exponential of -c(log x)^r beats every power of x. This would sum the actual frame tails (UD.4), even with fixed polynomial factors.

CMP119 (2.6) alone does not imply (UD.16): it supplies the upper bound on g_j^{-2} used in CGD, not a positive lower speed. We have not proved the required beta lower bound for the present nonsmooth density class. Even (UD.16) would not make q_j of order g_j times a logarithmic power summable; on that trajectory its sum can grow like sqrt(N-k) times logarithmic powers. Fixed GM localization discrepancies also remain separate.

## 5. What the primary variational bound actually supplies with age

There is a genuine scale factor in the source, but it should not be assigned to the complete covariance without the remaining identification.

Take a homogeneous variational problem at current spacing h_j and microscopic spacing eta. Perturb its admitted current data by exp(iB), with ||B||_infinity<=b in a fixed small physical tube. CMP102 Proposition 9, especially (173), (190) and the regularity bounds (19), supplies a compatible relative Landau gauge in which

\[
 U_j(e^{iB}V)^{u}U_j(V)^{-1}=\exp(i\eta A),
 \qquad
 \|A\|_\infty\le Cb/h_j,\quad
 \|\nabla_{U_j(V)}A\|_\infty\le Cb/h_j^2.
 \tag{UD.17}
\]

The estimates proportional to b follow by integrating the derivative (190) along tB; they are not obtained by replacing b with a larger fixed ceiling. The source row measure in that derivative is included.

Expansion around one fine plaquette, with its actual reference parallel transports, then gives

\[
 \|\operatorname{Hol}_{U_j(e^{iB}V)^u}(p)
       \operatorname{Hol}_{U_j(V)}(p)^{-1}-I\|
                    \le Cb(\eta/h_j)^2.
 \tag{UD.18}
\]

Indeed the first-order sum is the covariant discrete curl of eta A and is bounded by C eta^2 b/h_j^2; quadratic terms are bounded by C eta^2 b^2/h_j^2 and are absorbed for b small. All transports are unitary on this real comparison. This is a single-background response statement, not a composition of C per scale.

The missing promotion is substantial. The birth free precision is the *inherited constrained Hessian*, including its constraint-force term, exceptional map and averaged-gauge quadratic. Its derivative is not just a local plaquette derivative. To use (UD.18) in (UD.12), one must identify the same birth physical/free space for both backgrounds, prove the resulting relative precision or covariance estimate in that energy norm, and make the same identification for the complex outside family and its full raw carriers. A real relative Landau gauge need not preserve a chosen free-coordinate cutoff as a literal domain. Its complex continuation is not an isometry. Neither (UD.18) nor numerical decay of a response kernel proves the component restriction identities.

There is also no strict curvature-energy contraction in the already proved flat averaging inequality. IG.2 is ||Q_2||_2<=1 in dimension four. The row L^2 and column L^{2-d} sums saturate on constant two-form data; the estimate is scale-critical. Therefore it cannot alone provide the desired L^{-(j-k)} contraction of a complete birth energy or precision.

## 6. A concrete common-certificate target

For a fixed born payload and every later level N, retain one joint constrained Gaussian description of its original old coordinates and the intervening ordinary coordinates. Schur-integrate the ordinary coordinates once, preserving all cross terms, the actual terminal constraints and normalized gauge factors. Let Sigma_{k,N} be the resulting born marginal in the declared complex component family, and Sigma^0_{k,N} its centered positive real reference at the same real later variables.

One sufficient missing Gaussian estimate is

\[
 \left\|(\Sigma^0_{k,N})^{-1/2}
       (\Sigma_{k,N}-\Sigma^0_{k,N})
                     (\Sigma^0_{k,N})^{-1/2}\right\|_{\rm op}
                         \le\delta_*,
\]
\[
 \left\|(\Sigma^0_{k,N})^{-1/2}
       (\Sigma_{k,N}-\Sigma^0_{k,N})
                     (\Sigma^0_{k,N})^{-1/2}\right\|_1
                         \le \eta_*r_0+C n\omega_k,
 \tag{UD.19}
\]

uniformly in N, volume, admitted real later variables and the fixed outside polydiscs, with delta_* inside the original Gaussian reserve, eta_* inside its original rank/carrier reserve, and n omega_k paid once by a chosen fraction of nP_k^2. The analogous once-current trace/operator sums and the total frame displacement in the same birth energy norm must be controlled. A summable genuine ancestor bound, for example one derived with a factor L^{-a(j-k)} in this *relative energy norm*, would be one way to prove (UD.19). It is not assumed here.

Lemma UD.1 would then preserve the original Gaussian certificate with one tail expenditure. Complete inherited interaction, coarea and analytic-connector majorants must likewise be compared or resummed once. They are not consequences of the matrix bound. The common registry must retain the exact component/root-deletion identity; no independently chosen positive reference at each N can replace that requirement.

CA.19 proves (UD.19)'s two-level analogue with C(u_m+q_new), including the actual raw pullback. It does not establish the uniform-age statement. The precise unresolved step is a common source-constrained covariance/interaction comparison on the born marginal, with the full running action and gauge identification, rather than a further normalized scalar estimate.

## 7. Running action and the remaining anchor extraction

The action normalization cannot be hidden in the identification of coordinates. If the same physical displacement is written g_k z_k=g_j z_j, then

\[
 z_k=(g_j/g_k)z_j,\qquad
 |z_k|^2=(g_j/g_k)^2|z_j|^2.
 \tag{UD.20}
\]

CMP119 (2.6) yields

\[
 (g_N/g_k)^2\le 1+\beta'g_N^2(N-k),
 \tag{UD.21}
\]

not an all-age constant. At two adjacent levels the bounded ratio used in CA is legitimate. Restoring one original microscopic quadratic also restores the actual counterterms that moved the coupling between levels: CMP109 (0.22)--(0.23) writes the leading action as -g_j^{-2}A(U_j) and retains the earlier beta/action terms inside E_j. Dropping those terms while identifying every native Gaussian with one fixed energy would be incorrect.

In four dimensions the Wilson curvature action is marginal. The exact curvature-averaging norm in Section 5 reflects this. A uniform old Gaussian certificate alone would still leave the L^{4(N-k)} possible birth positions per final anchor proved in CGD.10.

The primary source addresses this for its analytic effective actions by a genuine extraction: CMP119 printed pp.280--282, (3.49)--(3.57), uses Taylor and Ward--Takahashi identities to separate the curvature-squared coefficient, with irrelevant terms bounded by a factor of order (L^{j-N})^{5-beta}, for fixed positive beta small enough. That order beats the four-dimensional anchor count after the relevant/vacuum terms have been handled. It is not obtained from positivity or shrinking support.

The retained Q-core corrections have presently been proved with values and first raw currents, not with the Taylor/Ward remainder hypotheses used by that analytic extraction. Branch nonsmoothness cannot be discarded because the coefficient is rare. A valid continuation must either prove an extraction directly for the core-integral representation, recombine complementary sectors where their artificial boundary terms cancel, or establish another actual summable anchored transport mechanism. The current note does not choose one without proof.

## 8. Consequences

The core-volume question is resolved by CGD. The crude repeated frame factor can be improved by (UD.15). The flat source supplies an exact joint certificate, (UD.13)--(UD.14), and the trace/operator lemma gives the correct nonlinear Gaussian target without a gratuitous rank-times-error cost at every step.

What remains unproved is (UD.19) and its complete interaction/component/current version for the actual nonlinear constrained family, followed by the relevant/vacuum and anchored scaling extraction for the nonsmooth core payloads. A small fixed two-step discrepancy cannot be declared summable. The two-step density decomposition AD/TD remains valid as specified; it is not an all-depth Yang--Mills construction.

References: CA.6, CA.10, CA.19--CA.25; TD.8--TD.16; CGD.1--CGD.10; IG.1--IG.10; NE.6--NE.9; CMP102 printed pp.281 and 305--309, (19), (173), (190), Proposition 9; CMP109 printed pp.255--256, (0.18), (0.20), (0.22)--(0.23); CMP119 printed p.255, (2.5)--(2.6), and pp.280--282, (3.49)--(3.57).
