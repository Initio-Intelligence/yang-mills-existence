# A retained-Schur tilt preserves a quantitative first-step seed box

This note proves a finite-dimensional normalized Gaussian lemma useful for the proposed first-birth/later-energy comparison. It keeps the outside cutoff factor exactly. It does not identify the post-localization source quadratic form with the primitive Schur form without checking the changes of variables in CMP119 (1.22).

## 1. Exact marginal and cutoff factor

Let `z=(a,b)` correspond to retained coordinates `D` and their complement `O`. Suppose the real symmetric precision satisfies

\[
 mI\le K\le MI,
 \qquad
 S=K_{DD}-K_{DO}K_{OO}^{-1}K_{OD}.
 \tag{ST.1}
\]

The empty-complement case is interpreted in the evident way. Let `Ω_D,Ω_O` be products of symmetric convex norm balls, with fixed coordinate dimensions. The D radii are at most `b_*P`, and the O radii can be P. Use the normalized Gaussian law restricted to this exact product support. Completing the square gives its D marginal

\[
 p_D(a)=\frac{1_{\Omega_D}(a)e^{-a^TSa/2}I(m(a))}
 {\int_{\Omega_D} e^{-u^TSu/2}I(m(u))\,du},
 \qquad m(a)=-K_{OO}^{-1}K_{OD}a,
 \tag{ST.2}
\]

where

\[
 I(q)=\int_{\Omega_O}
       e^{-(b-q)^TK_{OO}(b-q)/2}\,db.
 \tag{ST.3}
\]

It is generally wrong to omit `I(m(a))` and identify this marginal with the unrestricted Gaussian of precision S.

### Cutoff lemma

For every q,

\[
 e^{-q^TK_{OO}q/2}I(0)\le I(q)\le I(0).
 \tag{ST.4}
\]

For the lower bound, factor out the displayed quadratic and average
`exp(b^T K_OO q)` against the centered even cutoff Gaussian. Its expectation is at least one, by symmetry and `cosh≥1`.

For completeness, the upper bound follows from evenness and log concavity. One can verify the latter through convex smooth barriers without assuming it: replace `1_Ω` by `exp(−V_n)` with even convex barriers. The associated shifted potential has Hessian at least `K_OO`, and its covariance is bounded by `K_OO^{-1}`. This covariance bound follows from the Poisson equation and the integrated Bochner identity: if `−Lu=f−Ef`, then

\[
 \operatorname{Var}(f)=E(\nabla f\cdot\nabla u),\qquad
 E(Lu)^2\ge E(\nabla u^T K_{OO}\nabla u).
\]

For linear f, Cauchy–Schwarz in the K metric gives
`Var(ℓ·b)≤ℓ^T K_OO^{-1}ℓ`. Differentiating the shifted logarithmic integral therefore gives

\[
 \nabla_q^2\log I_n(q)
   =-K_{OO}+K_{OO}\operatorname{Cov}_q(b)K_{OO}\le0.
\]

Since `I_n` is even, its maximum is at zero. Passing to the barrier limit proves the upper bound in (ST.4). All these assertions concern a finite-dimensional positive integral, and the constants do not depend on the outside rank.

## 2. The tilted seed lower bound

Let E be any event in the retained coordinates. Suppose a product box `A⊂E∩Ω_D` has volume at least `c_*^{n_D}` and

\[
 \sup_{a\in A}m(a)^TK_{OO}m(a)\le C_*n_D,
 \tag{ST.5}
\]

where `n_D` is the actual number of scalar retained coordinates. Then

\[
 \mu_K^{\rm box}
   \left[e^{a^TSa/2}1_E\right]\ge e^{-C n_D}.
 \tag{ST.6}
\]

Indeed, by (ST.2)–(ST.4), its numerator is at least
`Vol(A) exp(−C_*n_D/2)I(0)`. Its denominator is at most

\[
 I(0)\int_{\mathbb R^{n_D}}e^{-a^TSa/2}\,da
   = I(0)(2\pi)^{n_D/2}(\det S)^{-1/2}.
\]

The principal covariance inequalities imply `mI≤S≤MI`, so this determinant costs at most a fixed constant per retained coordinate. This proves (ST.6). A box of radius `P^{-c}` instead of a fixed radius gives the weaker but still explicit lower bound `exp(−C n_D log P)`.

### Why an interior P-sized seed does not cost P² here

Suppose K has fixed finite range and

\[
 a=a^{\rm seed}+u,\qquad
 \operatorname{dist}(\operatorname{supp}a^{\rm seed},O)
        >\operatorname{range}K,
 \qquad \|u\|_\infty\le c_*.
 \tag{ST.7}
\]

The seed can have amplitude proportional to P. Nevertheless
`K_OD a_seed=0` exactly. Hence

\[
 m(a)^TK_{OO}m(a)
   =u^T K_{DO}K_{OO}^{-1}K_{OD}u
   \le C\|u\|_2^2\le C n_D.
 \tag{ST.8}
\]

Thus its P-sized energy has been canceled by the **complete marginal Schur tilt**, while the outside cutoff imposes only the bounded noise cost. No probability approximation or rare-event denominator is involved. For an exponentially localized K, the same proof gives an additional cost bounded by a constant times the squared seed norm times the appropriate exponentially small tail. The finite-range first primitive precision needs no such tail.

An actual source R seed must use the genuine independent coordinates. CMP119 p.249 defines those on `Ω_1^*=Ω_1\{b_0(c)}`; every assignment there is allowed, and the embedding C restores the exceptional entries and satisfies `QCA=0`. No second Q constraint is imposed on that independent vector. Any hard-tree coordinates already removed from the chart are also omitted. It is an assignment to the **full constrained bond field** that requires a separate embedding check. The cochain seed of RT.1 is one convenient sufficient realization, not a necessary additional condition on all independent-coordinate boxes. Strict bad/good margins allow a fixed-radius box for large P once the exact geometric stencil has been verified.

## 3. Transfer through the first-step marginal comparison

Let the actual normalized first-step D marginal `q_{v,D}` and the flat product-cutoff marginal `p_{flat,D}` obey the relative estimate

\[
 e^{-\Delta_D}\le q_{v,D}(a)/p_{flat,D}(a)
                    \le e^{\Delta_D}.
 \tag{ST.9}
\]

Suppose in addition that the actual source energy selected for cancellation has the same coordinates and satisfies on the encompassing product domain

\[
 |E_0(v,a)-\tfrac12a^TS_{flat}a|\le\delta_D.
 \tag{ST.10}
\]

Then (ST.6) gives

\[
 q_{v,D}(e^{E_0}1_E)
       \ge \exp[-C n_D-\Delta_D-\delta_D].
 \tag{ST.11}
\]

This is a direct positive-integrand comparison. It does not replace the actual tilt by a flat tilt without the explicit error (ST.10).

For the primitive Schur form, the buffered precision comparison is sufficient for (ST.10). RMg.31 supplies a local first-step precision discrepancy `O(R²ε)` on an R-buffer, with bounded global rows and a common positive gap. The resolvent/Schur comparison RK.1 then yields

\[
 \|S_D(v)^u-S_{D,flat}\|
    \le C(R^2\varepsilon+e^{-cR}),
 \qquad
 \delta_D\le C n_D P^2(R^2\varepsilon+e^{-cR}).
 \tag{ST.12}
\]

For `n_D=O(R^4)`, `ε=O(gP)`, and the source logarithmic cutoffs, this tends to zero. Block-adjoint invariant seed events and product balls are unchanged by the local coarse gauge used to prove the estimate.

## 4. The exact source check still needed

The proposed later-energy application requires an exact decomposition at the same retained/current conditioning,

\[
 M_s(d a,d y)=1_{E_s}(a,y)\,q_y(da)\,L_s(y)\,\pi(dy),
 \tag{ST.13}
\]

with every factor kept, and a source upper bound after multiplying the same measure by `exp(E_0+θE_late)`. Formula (ST.11) then bounds the remaining y-integral without dividing by the tiny un-tilted birth probability. The marginal comparison separately restores the correct flat birth factor in the un-tilted numerator.

Before using this argument, the following are substantive equalities to check in the source, not consequences of the Gaussian lemma:

1. The energy called E0 is the full first retained Schur quadratic in the same free coordinates. CMP119 (1.26)–(1.29) produces such a form, but its localized coordinate changes in (1.22) must be retained in the comparison. Any induced shift or Jacobian is charged once.
2. Other retained first components and their cross terms are either part of that same canceled quadratic or explicitly controlled in the complete conditional density. They cannot be dropped by calling the form a self-energy.
3. All actual first-coordinate selectors bound the post-cancellation domain; the upper estimate cannot extend an uncanceled positive exponential over an unbounded Gaussian direction.
4. The remaining normalization, E/B/R and later positive-form estimates are for this same mass and conditioning. A fresh reference density is not the old denominator.

The lemma closes the Gaussian tilted-box lower bound under these exact matching conditions. It does not itself establish the complete later source upper estimate.

### Recorded first-step source analysis

The independent signed [first schur cancellation source analysis](first_schur_cancellation_source_analysis.md) verifies these matching points on the original `h=1`, globally P/Q-good bounded R-neighborhood scope. Its primary-page check finds the exact combination `−A^TKA/2+A^TK C^{(0)}(Λ_1)KA/2` in CMP119 (1.29), hence the untruncated marginal Schur form with the sign used here. The outside cutoff/completion factor remains in the effective integral (1.26) and is retained in (ST.2). The later component split in (2.21) moves cross-component entries into the boundary action; their MR-separated matrix tails are controlled in the analysis rather than discarded.

The same analysis checks the actual localization change (1.22), its Jacobian record (1.24), and the genuine independent coordinate boxes. On the strict `5P/4` witness box used there the localization change is exactly the identity; on the larger encompassing domain its small tail is charged explicitly. This verifies the indicated first-step cancellation match. The source upper estimate after the tilt, its full/self embedding, and the later positive reserve remain separate from this Gaussian lower-bound theorem.
