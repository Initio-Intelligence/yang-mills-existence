# A normalized quotient with a bounded core and supported exterior perturbations

This is a sufficient theorem with a direct proof. Its source-free perturbation hypothesis is more primitive than an assumed marked numerator estimate. The actual residual source fit is not yet verified.

## 1. Exact setup

Let D₀ be a fixed connected set of current physical blocks, with |D₀|≤V₀ independent of the scale. Let ν₀(v_{D₀},du) be a positive probability law on any old-variable space. That space may contain many coordinates or a finite mixture of histories. Its dependence on retained variables is confined to D₀.

Suppose the actual new normalized old law is

\[
 q_v(du)=\frac{e^{\Sigma(v,u)}\nu_0(v_{D_0},du)}
                   {\nu_0(e^{\Sigma(v,\cdot)})},
 \qquad
 \Sigma=\sum_{X\supset D_0}\sigma_X(v_X,u).
 \tag{BC.1}
\]

Every X is a connected actual retained carrier, and σ_X is bounded uniformly over the old integration variables on their genuine support. All factors independent of u have already been canceled between numerator and denominator. No positivity or small mass has been dropped. On real v, Σ is real.

Use the weight w_κ(X)=exp{κ(|X|+t(X))}. Assume

\[
 \sum_X w_\kappa(X)\sup_{v,u}|\sigma_X(v_X,u)|
       \le\varepsilon,
 \qquad e^{\varepsilon}-1<1.
 \tag{BC.2}
\]

The important point is that ε bounds the absolute coefficient sum before cancellations and is uniform in the entire old state. Numerical closeness of the summed kernels is not (BC.2).

For an incoming mark let

\[
 F(v,u)=\sum_{Y\supset D_0}f_Y(v_Y,u),
\]

with a specified absolute value budget

\[
 \sum_Y w_\kappa(Y)
       \sup_v\nu_0(v_{D_0},|f_Y(v_Y,\cdot)|)
       \le B_F.
 \tag{BC.3}
\]

For regulated versions, the same proof applies with a monotone local envelope R_Y, whenever products with σ_X leave that envelope unchanged and R_Y≤R_{X∪Y}. Conditional Lᵖ budgets can be used in place of the displayed L¹ budget. Such budgets must be proved for the actual ν₀; they are not inferred from positivity.

## 2. Direct absolute expansion of the exact quotient

### Theorem BC.1

Under (BC.1)–(BC.3), q_vF has an actual connected-carrier expansion whose weighted absolute value budget is at most

\[
 \frac{e^{\varepsilon}}{2-e^{\varepsilon}}\,B_F.
 \tag{BC.4}
\]

All coefficients depend only on their declared raw retained carriers. No estimate of an inverse old mass is used after ν₀ is normalized.

**Proof.** Expand the numerator as the absolutely convergent series

\[
 N_F(v)=\sum_{n\ge0}\frac1{n!}
       \sum_{Y,X_1,\ldots,X_n}
        \nu_0\left(f_Y\prod_{j=1}^n\sigma_{X_j}\right).
 \tag{BC.5}
\]

Every support union is connected because every factor contains D₀. The weight of that union is at most the product of its factor weights. Integrate the absolute value using (BC.3), and use (BC.2) for each bounded perturbation factor. The weighted numerator budget is at most B_F e^ε.

Put d(v)=ν₀(e^Σ−1). The same expansion without f gives a supported coefficient budget at most e^ε−1. Since this is less than one,

\[
 \frac1{1+d}=\sum_{m\ge0}(-d)^m
 \tag{BC.6}
\]

converges in the absolute carrier algebra. Its norm is at most (2−e^ε)^{-1}. Multiplying (BC.5) and (BC.6) gives the exact normalized quotient and (BC.4). Dependence of ν₀ contributes only D₀, already present in every union. The product representation retains individual tags. ∎

This elementary core expansion does not require a cluster theorem over an extensive product of old coordinates. Arbitrarily many old modes can remain inside ν₀; their effect enters only its explicitly supplied marked moment and current budgets. It also does not claim that a generic residual quotient admits (BC.1) with a uniformly bounded core.

## 3. Direct and kernel currents

Suppose the normalized reference law has exact differentiated expectations on a fixed old support. Write its centered score as S⁰_d. Assume the absolute budgets for ν₀(D_df_Y), ν₀(f_Y S⁰_d), and the corresponding unmarked reference derivatives are supplied, with sums over all directions in D₀. Assume also

\[
 \sum_Xw_\kappa(X)
      \sum_d\sup_{v,u}|D_d\sigma_X(v_X,u)|
       \le\varepsilon_1<\infty.
 \tag{BC.7}
\]

Differentiating the actual numerator and denominator series produces the correct two contributions. Differentiating a perturbation word of length n gives n positions, so its scalar majorant is ε₁e^ε. Differentiating (BC.6) costs

\[
 \sum_{m\ge1}m(e^\varepsilon-1)^{m-1}
       =(2-e^\varepsilon)^{-2}.
 \tag{BC.8}
\]

Thus the weighted direct and kernel budgets remain finite, with a constant depending only on ε, ε₁ and the stated reference budgets. No factor Dσ_X/σ_X is introduced. The derivative can be nonzero when σ_X itself vanishes.

For a scalar whose reference value has energy grade one and whose reference score has square-root grade, conditional Hölder gives grade 3/2, exactly as in RM.9–RM.12. The external perturbation score is bounded by (BC.7), so it requires no greater grade. Retained-only terms in the logarithmic density cancel from the centered score.

Introduce two retained copies, one for f and one for ν₀ and Σ. On each localized tag H_a(v_ins,v_ker), use

\[
 B_{a,d,t}=\frac{H_a(v_t,v_t)-H_a(v,v_t)}t,
 \qquad
 J_{a,d,t}=\frac{H_a(v,v_t)-H_a(v,v)}t.
 \tag{BC.9}
\]

The per-tag compatibility identity is exact. Continuous-path estimates require all of the stated reference and perturbation budgets along both rectangular paths. A discrete replacement uses the same endpoint formula without division by t and requires the two-copy admission on the padded common old state space. Its complete dependency footprint must be retained.

## 4. How this could apply to a prepared residual core

LFR I makes the prepared replacement core Λ a rectangle of diameter at most 100M in current units. LFR II (1.73)–(1.75) gives a relative comparison of the native old operation with a positive real operation: its complete density changes by a uniformly small exponent σ on the stated independent native background/current domain. This is a useful source-free input, stronger than an upper bound on a tiny old mass alone.

It does not yet establish (BC.1)–(BC.2) in raw retained variables. The following identities and estimates are needed:

1. A positive reference ν₀ whose raw retained dependence is confined to one uniformly bounded current core D₀. All old normalized measures and necessary reference choices must be included.
2. An exact supported expansion of the difference of the complete old log densities, with each exterior carrier connected to D₀ and with the absolute bound (BC.2), uniform over old variables and histories.
3. Inclusion of the cross-component boundary exponential in that same comparison. The normalized self-operation T′_k(Y)/T′_k(Y)1 is not automatically the full old posterior.
4. Actual reference marked moments and scores, possibly obtained from a matched old trial mass and the tilted energy reserve in [residual relative mass lemma](residual_relative_mass_lemma.md).
5. A locality identity for the retained geometric labels themselves. It is not enough that the newly integrated continuous variables lie in Λ: a coefficient that still depends on a full Y descriptor must pay that descriptor's full footprint.

The cutoff ζ_Y, the exterior-dependent reference minimum, and the hidden-history admission rules are not discarded by calling Λ a bounded core. Their effects must either cancel exactly as old-variable-independent factors or be included with their actual supported perturbations. The published grouped estimate that contracts Y does not prove this list.

If these inputs are verified, Theorem BC.1 would give the normalized marked carrier estimate directly, without assuming the unknown marked numerator bound as an induction hypothesis. At present it is a concrete sufficient route, not a completion of M-04.
