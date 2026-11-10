# A completed Gaussian cutoff belongs in the reference law

This note records a concrete limitation of an old-fluctuation Cauchy argument and an exact remedy at the Gaussian level. It is not a counterexample to the actual source kernel: a separately proved strict conditional-mean margin could exclude the example in a particular source chart. It shows why the displayed real boundary-action bound alone cannot supply the required analytic disk.

## 1. A bounded completion can have order-one boundary derivatives

Consider the positive two-variable quadratic action

\[
 \tfrac12(z-a)^2+\tfrac12a^2.
 \tag{GC.1}
\]

Its precision is [[2,-1],[-1,1]] in the order (a,z), with a fixed positive gap. The conditional law of z at fixed a is N(a,1). Impose the good cutoff |z|<P and integrate z. After removing the exact untruncated Schur action a²/2, its normalized completion is

\[
 I_P(a)=\Phi(P-a)-\Phi(-P-a),
 \qquad |a|\le P.
 \tag{GC.2}
\]

It is even. On the whole interval |a|≤P it lies between 1/2−o(1) and 1, so |log I_P| is bounded independently of P. Nevertheless

\[
 (\log I_P)'(P)\longrightarrow-\sqrt{2/\pi},
 \qquad
 (\log I_P)''(P)\longrightarrow-2/\pi.
 \tag{GC.3}
\]

Indeed I_P(P)=Phi(2P)−1/2, I'_P(P)=−phi(0)+phi(2P), and I''_P(P)=−2P phi(2P). The formulas in GC.3 follow directly.

Thus a uniform O(1) real log-completion bound does not imply O(P^{-1}) first derivatives or O(P^{-2}) second derivatives. Nor can that real bound be used as a uniform complex bound for log I_P on disks of radius cP centered at all admitted real a: Cauchy would contradict GC.3. This example satisfies uniform positive precision and fixed-dimensional local conditioning.

A strict margin such as |E(z|a)|≤(1−epsilon)P on the full admitted external domain would change the situation: the cutoff is then uniformly far in a Gaussian tail and a proportional complex tube can be proved. That margin is a substantive extra estimate. It is not implied by a spectral gap alone.

## 2. Exact Gaussian completions preserve convexity

For a general positive quadratic in retained u and integrated z, complete the square:

\[
 \tfrac12(u,z)^{\mathsf T}K(u,z)
 =\tfrac12u^{\mathsf T}Su+
   \tfrac12(z-m(u))^{\mathsf T}K_{zz}(z-m(u)).
 \tag{GC.4}
\]

Let C_z be a fixed centrally symmetric convex cutoff set. Its exact completion is

\[
 I(u)=\int_{C_z}
 e^{-\frac12(z-m(u))^{\mathsf T}K_{zz}(z-m(u))}\,dz.
 \tag{GC.5}
\]

The integrand is jointly log-concave in (u,z), including the indicator of C_z. Marginalization of a log-concave function gives that I is log-concave; equivalently this follows from the Brascamp–Lieb covariance bound for the conditional truncated Gaussian and direct differentiation of log I. Therefore

\[
 V_{\rm marg}(u)=\tfrac12u^{\mathsf T}Su-\log I(u)
 \quad\hbox{has}\quad \nabla^2V_{\rm marg}\ge S.
 \tag{GC.6}
\]

I and V_marg are even. The completion's possibly order-one derivatives strengthen the convex reference potential; they need not be a small perturbation.

For completeness, writing m(u)=Hu and differentiating gives

\[
 \nabla^2\log I
 =-H^{\mathsf T}K_{zz}H+
 H^{\mathsf T}K_{zz}\operatorname{Cov}(z\mid u,C_z)K_{zz}H
 \le0,
\]

because the truncated Gaussian on a convex domain has covariance at most K_zz^{-1}. This proves GC.6 without requiring smooth cutoff boundaries; convex barrier approximation gives the same inequality.

Local linear root bounds can be obtained directly before integrating z: condition the joint Gaussian on the convex symmetric product event and apply CR.12. This retains all cutoff completion factors exactly and gives the same energy-based variance estimate as GB.6–GB.9. No analyticity of log I in a P-sized complex tube is needed.

## 3. What the actual comparison has to control

At one actual complete regular layer, RMg compares the nonlinear Wilson marginal to the Gaussian marginal with **the same product cutoff**. Its proof keeps the conditional boundary-score covariance. It never differentiates log I as though I were a small boundary perturbation. Consequently that theorem already uses the correct reference-law convention.

For a restored multiscale operation, the analogous sufficient strategy is:

1. Keep its complete Gaussian conditional completions in the reference law, including their off-diagonal Schur means and terminal constraints.
2. Compare the actual remaining density to this reference, controlling the nonlinear and coefficient perturbations. Prove real derivative or relative marginal bounds for that difference, not for the entire completed Gaussian boundary action.
3. Handle any genuinely changed outside cutoff products by the relative OC transport, retaining the same conditional normalization.

Restoring a finite collar does not alone remove this issue. The newly exposed outermost variables are adjacent to the remaining integrated variables, so a completion like GC.2 can reappear at the new interface. The original inner variables may have exponentially weak influence across the collar, but that statement is distinct from a uniform small-derivative assertion for **all** variables in the enlarged finite list.

The source smooth relocalization switch is a separate matter. Undoing its exact change of variables eliminates it, or its finitely many derivatives can be tracked as independent bounded control parameters multiplied by the exponentially small displacement. Neither operation supplies the missing old-A complex domain for an unrelated cutoff completion.

This note leaves the actual source-fit question open: whether its conditional means have the necessary strict cutoff margin, or whether the full first-family comparison can retain the exact Gaussian completions as the convex reference and estimate only their nonlinear difference. It rules out inferring that answer solely from CMP119's bounded B term and its stated U/J analyticity.
