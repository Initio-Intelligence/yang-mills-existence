# Relative old mass, normalized energy, and a conditional current criterion

The lemmas below are proved. Their application to the completed Wilson residual quotient requires the explicitly identified matching, trial-history, and score estimates. No old mass is replaced by a fresh reference normalizer.

## 1. Matching the two masses is part of the hypothesis

Fix a retained datum v and a fresh reference class r. Let M_{r,v} be the actual positive measure on precisely the old variables and old histories that are integrated in that class, with every old selector, coarea factor, effective density, and reference factor retained. Its normalization is

\[
 m_{r,v}=M_{r,v}(1)>0,\qquad
 \nu_{r,v}=m_{r,v}^{-1}M_{r,v}.
 \tag{RM.1}
\]

Let E≥0 be a specified old energy/rank envelope on these variables. A useful pair of estimates would be

\[
 M_{r,v}(e^{tE})\le A_{r,v}e^{-P},\qquad
 M_{r,v}(1)\ge A_{r,v}e^{-D},
 \quad t>0,
 \tag{RM.2}
\]

with exactly the same positive factor A_{r,v}. The numbers P,D may depend on the displayed scale and retained datum; uniformity of later consequences depends on the bounds imposed on them. The factor A may contain a genuine common vacuum/reference factor. It cancels only if it is literally common to the same two old integrals.

An estimate that has already integrated additional fresh current variables is not the first inequality in (RM.2). A lower estimate for the newly sampled reference integral H_r is not the second. Neither can be substituted without a separate disintegration identity.

Since E≥0, (RM.2) can hold only with D≥P at the precision of the displayed constants; harmless fixed prefactors can be included by increasing D. Put

\[
 \Delta=D-P\ge0.
\]

## 2. The normalized moment theorem

### Lemma RM.1

Under (RM.2), for every s≥0,

\[
 \nu_{r,v}(E\ge s)\le\min(1,e^{\Delta-ts}).
 \tag{RM.3}
\]

For every real p≥1,

\[
 \|E\|_{L^p(\nu_{r,v})}
 \le\frac{\Delta+2p}{t}.
 \tag{RM.4}
\]

**Proof.** Markov's inequality applied to the numerator of (RM.1), followed by the two estimates in (RM.2), gives (RM.3). Let Y=(E−Δ/t)_+. Then ν(Y≥s)≤e^{-ts}. The tail integral gives EνY^p≤Γ(p+1)t^{-p}, and Γ(p+1)^{1/p}≤2p for p≥1. Minkowski's inequality yields (RM.4). The argument needs no independence of old coordinates and no lower mass for each old history separately. ∎

The conclusion is polynomial in the logarithmic lower-mass loss Δ, although the normalized exponential moment may be as large as e^Δ. Bounding the first few moments directly by that exponential would discard the useful information.

Suppose the actual output-native regulator R_out(v) obeys

\[
 1+\Delta\le C_\Delta R_{\rm out}(v).
 \tag{RM.5}
\]

Then RM.4 implies

\[
 \|1+E\|_{L^p(\nu_{r,v})}
       \le C p R_{\rm out}(v).
 \tag{RM.6}
\]

Thus an old normalized energy bound can follow from a relative trial mass. The small unnormalized mass is not simply left over after dividing by itself; its quantitative logarithmic comparison with a valid trial mass is what is used.

## 3. What the source exponents could pay

The last N=O(R_k) eligible shells have total surviving rank O(R_k^5). If a valid fresh-birth trial in the same class gave

\[
 D\le C\{P(g_k)^2+R_k^5\log(g_k^{-1})\},
 \tag{RM.7}
\]

and the source exponent hierarchy made the second term at most a fixed multiple of P(g_k)^2, then a residual native witness

\[
 R_{\rm out}(v)\ge cP(g_k)^2
 \tag{RM.8}
\]

would imply (RM.5). The old-history sum could still contain arbitrarily old and high-rank branches; the exponentially tilted upper bound includes their true masses. The lower bound need only use one admissible trial branch or one positive trial submeasure.

The unresolved source work is substantial: that trial must produce the exact same r, Y, and shell; its genuine old density must have the bound claimed; and the upper reserve must apply at the same conditioning level. A dimensionless Gaussian box should be measured against its normalized source transition, so explicit powers of g and vacuum factors are not counted twice. The trial argument is not complete merely because a geometrically similar pure-gauge history exists.

## 4. A separate score criterion gives the expected current grade

The following conditional lemma identifies a useful quantitative target. It concerns a fixed old-coordinate support. Moving old selectors or rank changes require their own terms and are not silently differentiated as smooth densities.

Assume the positive old measure has density w_v on a common reference support and can be differentiated under the integral. Let F_v be an incoming scalar expression and let h be its physical unit. Suppose

\[
 |F_v|\le b h^{-4}(1+E),\qquad
 \sum_d|D_dF_v|\le b h^{-4}(1+E),
 \tag{RM.9}
\]

where d ranges over the relevant normalized retained directions. Suppose for each d there is a retained-only constant c_d(v) and a nonnegative a_d with

\[
 |D_d\log w_v-c_d(v)|
       \le a_d\{1+\sqrt E+gE\},
 \qquad \sum_da_d\le A_1.
 \tag{RM.10}
\]

The constants c_d include any purely retained normalization factor and disappear from the covariance. The term √E is the usual mean/linear-force response; gE allows a normalized derivative of a quadratic precision. These bounds are hypotheses on the complete actual score, not consequences of a Gaussian covariance estimate alone.

Set B_d=ν(D_dF) and J_d=Cov_ν(F,D_d log w). From RM.4, with K=1+(Δ+4)/t,

\[
 |\nu F|+\sum_d|B_d|\le Cb h^{-4}K,
 \tag{RM.11}
\]

\[
 \sum_d|J_d|\le C A_1 b h^{-4}
               (K^{3/2}+gK^2).
 \tag{RM.12}
\]

**Proof.** The value/direct estimate is RM.9 and the first moment. For the current subtract c_d in its covariance, apply Cauchy–Schwarz, and use

\[
 |\operatorname{Cov}(F,S)|\le2\|F\|_2\|S\|_2.
\]

RM.4 bounds the second energy moment by CK, the square-root energy norm by C√K, and the quadratic-score term by CgK. Sum the a_d. ∎

If K≤C R_out and g√K≤C, (RM.12) has the required pointwise energy grade R_out^{3/2}. In a residual regime with K=O(P(g)^2), the latter condition follows from gP(g) bounded. These observations explain which lower-mass and score bounds would suffice; they do not verify them for the Wilson old operation.

For exact finite differences, the insertion and kernel are treated on two separate retained copies as in M.30. The energy and score hypotheses must hold on both rectangular paths with a common shifted native regulator. A diagonal derivative of the summed output would not establish the separate direct and kernel estimates.

## 5. Embedding a self-law moment in the actual component posterior

### Lemma RM.2

Suppose the actual positive posterior has a fixed residual component i with self measure M_i. Conditional on all other old variables and successful-component choices ω, suppose its old conditional law is

\[
 q_i(du_i\mid\omega,v)
   =\frac{e^{H_i(u_i,\omega,v)}M_i(du_i;v)}
           {M_i(e^{H_i(\cdot,\omega,v)};v)}.
 \tag{RM.13}
\]

If the actual incident cross action has oscillation at most λ,

\[
 \sup_{u_i}H_i(u_i,\omega,v)
       -\inf_{u_i}H_i(u_i,\omega,v)\le\lambda
 \tag{RM.14}
\]

uniformly in ω and all admitted old states, then every nonnegative f satisfies

\[
 q_i(f\mid\omega,v)\le e^\lambda\nu_i(f),
 \qquad \nu_i=M_i/M_i(1).
 \tag{RM.15}
\]

The same bound remains after averaging ω in its true posterior. For a pth moment, the loss in the Lᵖ norm is e^{λ/p}≤e^λ.

**Proof.** Bound e^{H_i} in the numerator by its supremum and in the denominator by its infimum. Their ratio is at most e^λ. Then use the exact conditional-expectation identity to average the bound. ∎

The hypotheses concern the complete incident cross action, not a globally summed extensive action. An absolute incident bound λ₀ implies (RM.14) with 2λ₀. HS20's cross-action comparison is the source estimate to match to this lemma. It permits a self-law energy result to be embedded without discarding the cross terms. It does not control a raw retained derivative of H_i; the full posterior score and its physical carriers remain additional obligations.

## 6. The physical carrier issue remains after this lemma

Even if RM.2 and RM.10 are proved, the lemma controls a conditional value and its score. It does not construct an absolute carrier expansion. Assigning the whole residual Y as one carrier still incurs exp{κ(|Y|+t(Y))}. That factor is absent from RM.11–RM.12 and cannot be inferred from a polynomial native regulator.

The next task would be to localize the same normalized old quotient in its actual raw retained variables, or to prove a stronger exact cancellation/local input budget that pays that full cost. A fresh reference-class label can separate singular support strata, but changing it is a discrete M-03 direction with its entire genuine dependency footprint. No norm is changed by this conditional criterion.
