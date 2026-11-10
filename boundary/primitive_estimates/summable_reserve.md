# Summable reserves in the native norm

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

This note proves a quantitative norm-budget lemma. It is part of the actual-model argument; the new-record attachment bound stated below must be checked on the literal source expansion before the lemma can close that proof.

## 1. The precise loss this addresses

A fixed old dependency footprint may admit many new localization attachments. Even when the intensity per possible attachment is small, summing a family can give

\[
 \exp\{C\epsilon_k[n(G)+q(G)]\},
\]

where `n(G)` counts the old active cells and `q(G)` counts retained old component records. Neither count is guaranteed to decrease strictly at every step. Calling the new factor small does not preserve an unchanged exponential norm through arbitrarily many steps.

The remedy is a *summable* change of auxiliary weights. The source geometry, physical cutoffs, analytic charts and action remain unchanged. Only the weights used to estimate the expansion vary. They stay above fixed positive lower bounds independent of the depth.

An unsummable error such as `epsilon_k=C g_k` does not qualify. Every use of this lemma must retain a superlogarithmic collar factor, or establish another summable bound.

## 2. The exact retained AF envelope suffices

Write `t_j=g_j^{-2}`. The retained trajectory envelope, in the notation of CMP109, printed p.259, (0.31), is

\[
 t_K+a(K-j)\le t_j\le t_K+A(K-j),
 \qquad 0<a\le A,                                      \tag{S1}
\]

where `a=beta log L`, `A=beta' log L`. This note uses (S1) as the already stipulated trajectory input. The source says that its proof is to appear separately; this note neither supplies that proof nor establishes the trajectory for the Wilson construction.

For `b<=k<=K`, (S1) gives the useful comparison

\[
 t_b\ge c_{\rm AF}t_k+a(k-b),\qquad
 c_{\rm AF}=a/A.                                      \tag{S2}
\]

Indeed,

\[
 t_b\ge t_K+a(K-k)+a(k-b)
 \ge (a/A)[t_K+A(K-k)]+a(k-b)
 \ge (a/A)t_k+a(k-b).
\]

No positive one-step decrement of the uncorrected coupling has been inferred.

For chronological bookkeeping it is useful to introduce the **auxiliary** monotone profile

\[
 \underline t_j=t_K+a(K-j).
 \tag{S2a}
\]

This is a weight used in the proof, not a replacement for the actual coupling or any physical cutoff. The retained envelope gives

\[
 \underline t_j\le t_j\le(A/a)\underline t_j,
 \qquad
 \underline t_b=\underline t_k+a(k-b)
 \ge c_{\rm AF}t_k+a(k-b).
 \tag{S2b}
\]

If `f` is in its decreasing range, a source tail bounded by `f(t_j)` is therefore bounded by `f(underline t_j)`, and these auxiliary tail bounds are nondecreasing in chronological scale `j`. In particular for `b<=r`,

\[
 f(\underline t_b)\le f(\underline t_r).
 \tag{S2c}
\]

This avoids repeatedly weakening a collar exponent merely to compare a recent input's profile with the current one. Over a polynomial-length prefix window the logarithms of `underline t_j` and the actual `t_j` are comparable, with constants fixed in advance. An extra polynomial number of recent labels still needs to be counted explicitly. Likewise (S2c) does not authorize charging that polynomial repeatedly to an unchanged creation record; the component-lineage argument is a separate required input.

Let

\[
 f(t)=C t^s(1+\log t)^p\exp[-c(\log t)^r],
 \qquad r>1,
\tag{S3}
\]

with fixed constants, `s,p>=0`, `c>0`. For sufficiently large `t`, this is decreasing. Its logarithmic derivative, multiplied by `t`, is

\[
 s+\frac{p}{1+\log t}-cr(\log t)^{r-1},
\]

which is negative eventually. It is integrable at infinity: substituting `u=log t` gives

\[
 \int_T^\infty f(t)\,dt
 =C\int_{\log T}^\infty
 (1+u)^p\exp[(s+1)u-cu^r],du<\infty.
\]

For a cutoff-independent lower endpoint `T` in the decreasing range, (S2) and the integral test give

\[
 \sum_{b=0}^{k}f(t_b)
 \le f(c_{\rm AF}t_k)
       +a^{-1}\int_{c_{\rm AF}t_k}^\infty f(t)\,dt.
\tag{S4}
\]

The right side tends to zero as the common coupling ceiling tends to zero. In particular,

\[
 \sup_K\sum_{k=0}^{K}
 Cg_k^{-u}(1+\ell_k)^p e^{-c'R_k}=o(1),
 \qquad \ell_k=\log g_k^{-2},\quad R_k\ge c_R\ell_k^r,
\tag{S5}
\]

for every fixed `u,p,c'>0`. Fixed fractional powers of this expression have the same property. All constants must be fixed before the ceiling is reduced.

## 3. Weighted attachment transfer

For a record `G`, let `n(G),q(G)` be nonnegative integer counts. Suppose a source step attaches a finite family of genuinely new records to `G`. Let `a_{k,G}(F)` be a deterministic positive majorant for an attachment family `F`, including its actual factorial or forest factor. Suppose the verified rooted attachment calculation gives

\[
 \sum_F a_{k,G}(F)\,
 e^{\nu_k\Delta n(F)+\eta_k\Delta q(F)+
       \lambda\Delta\ell_k(F)}
 \le \exp\{D\epsilon_k[n(G)+q(G)+1]\}.                \tag{S6}
\]

Here the new connector costs are paid by new source exponents; an old connector is carried with its exact physical rescaling. Formula (S6) is a concrete input inequality, not a consequence of the definition of an attachment.

Assume also that the zero-attachment branch is the actual unchanged scalar composed with the admitted source map, hence has norm at most its old norm with factor **one**. No constant is multiplied once per step in this branch.

Choose initial auxiliary rates `nu_0,eta_0>0` and put

\[
 \nu_k=\nu_0-D\sum_{j\le k}\epsilon_j,
 \qquad
 \eta_k=\eta_0-D\sum_{j\le k}\epsilon_j.               \tag{S7}
\]

If

\[
 D\sum_j\epsilon_j\le\tfrac12\min(\nu_0,\eta_0),     \tag{S8}
\]

then both rates remain above one-half of their initial values. The loss in (S6) proportional to `n(G)+q(G)` is canceled exactly by

\[
 e^{\nu_k n(G)+\eta_k q(G)}
 e^{D\epsilon_k[n(G)+q(G)]}
 =e^{\nu_{k-1}n(G)+\eta_{k-1}q(G)}.                  \tag{S9}
\]

Only the factor `exp(D epsilon_k)` remains. Across arbitrary depth its product is bounded by

\[
 \prod_k e^{D\epsilon_k}
 =\exp\left(D\sum_k\epsilon_k\right),                \tag{S10}
\]

which is uniformly bounded and tends to one at a smaller coupling ceiling. A carried activity with arbitrarily many old cells or tags is therefore covered without assuming strict coarsening of every count.

The same argument applies to a finite vector of auxiliary counts and rates. One may decrease each rate by the coefficient actually multiplying its count in (S6). Only the positive lower floors enter the final cluster convergence and derivative estimates.

There is a useful slightly more general form. If the attachment bound contains

\[
 \exp\{d_k\ell_b(G)+D\epsilon_k[n(G)+q(G)+1]\},
 \qquad d_k\le\tfrac12(1-L^{-1})\lambda,
\tag{S6a}
\]

the first factor is paid by half the physical coarsening reserve in (S12); only the second uses the summable rate changes. This distinction matters for an old long carrier already reaching the new regular region. Repeated local T attachments along its paid portion may have a bare `O(g_k P_k)` intensity. Their number is controlled by the paid connector and their cost can use (S6a). One old collar crossing must not be charged separately to every such attachment. For old fixed tags or cells whose count is not controlled by a paid connector, the remaining per-site intensity still has to be genuinely summable.

## 4. Connector rate and physical coarsening

The physical connector rate can remain fixed. For an inherited graph of birth `b<k`, its paid physical length in current units is exactly `L^{-(k-b)} ell_b`. With the same old zero-cost cores and actual paid joins,

\[
 \ell_k(G_{\rm out})
 \le \sum_\alpha L^{-(k-b_\alpha)}\ell_{b_\alpha}(G_\alpha)
       +\sum_i\ell_k(W_i).                            \tag{S11}
\]

The coefficient of each old length is one. At a new scale there is consequently a reserve at least

\[
 (1-L^{-1})\lambda\sum_\alpha\ell_{b_\alpha}(G_\alpha)
\tag{S12}
\]

after the output connector weight has been paid. New map/localization pieces pay their own lengths and domain entropy. An inequality with an unexplained constant multiplying every old connector would not establish this fixed-rate conclusion.

Retain the old input birth labels through the ordinary T and subsequent R calculation. An intermediate conventional label `B_T^(k)` does not erase the coarsening reserve of an inherited completed input. Only the final completed output receives the new birth label.

## 5. Strong positive activity norms are allowed here

The current target needs a supremum outside its weighted row sum, as corrected in the pointwise-majorant note. Nevertheless a stronger norm

\[
 \sup_{\text{admitted histories}}
 \sup_{\text{local roots }r}
 \sum_{a\ni r}w_k(a)\,\|F_a\|_{\mathcal D_k}
\tag{S13}
\]

is a legitimate sufficient invariant when it is derived directly. The original ordinary inputs have deterministic individual source bounds. A whole old scalar can be kept as one atom; exact old/new reference equality is used before absolute values, and only genuinely new localization/walk records are expanded. Their uniform Cauchy bounds are proportional to the old atom's admitted supremum norm. Positive reference integration and the explicit Mayer/connected-forest majorants then act on deterministic nonnegative bounds.

This route does not deduce a sum of suprema from a supremum of a signed sum. It also does not reopen an old completed scalar into an uncontrolled sum over its internal histories. If its actual new-record estimate is proved, it supplies (S13) directly and removes the need to use independent phase marks for that transfer.

## 6. Exact remaining application check

The unresolved application in this note is (S6) for every literal nonempty attachment, including descendants of an old completed scalar in the ordinary T step. The source's bare `O(g_k P_k)` response alone is not summable over the ultraviolet scales. For that sector one must retain the extra old-port/current-small-field collar or another proved summable factor. Pure forcing terms without an inherited completed input have their separate ordinary full-tree estimate and must not be mistaken for repeated attachments to an old free core.

Once the actual incidence/attachment estimate gives `epsilon_k` of the form in (S5), the auxiliary norm loss does not accumulate with depth. Equations (S7)–(S10) prove this quantitatively, with one coupling ceiling and fixed positive final rate floors.

## 7. Extracting a fresh small coefficient needs a larger summable reserve

The exact cancellation in (S9) suffices to preserve a carried norm. It does **not** by itself leave a factor `O(epsilon_k)` on its nonempty attachment branch. Indeed, for arbitrarily large old count `n`,

\[
 e^{-D\epsilon n}(e^{D\epsilon n}-1)
 =1-e^{-D\epsilon n}
 \longrightarrow1.
 \tag{S14}
\]

Calling this uniformly `O(epsilon)` would be wrong. To prove a separate fresh-output bound, allocate a slightly larger, still summable, decrement.

Let `0<epsilon<=epsilon_0` and set `rho=K sqrt(epsilon)`, with fixed `K>0`. Reduce `epsilon_0` so that `rho>=2D epsilon`. For every real `n>=0`,

\[
 \begin{aligned}
 e^{-\rho n}(e^{D\epsilon n}-1)
 &\le D\epsilon n\,e^{-(\rho-D\epsilon)n}\\
 &\le D\epsilon n\,e^{-\rho n/2}
 \le \frac{2D\epsilon}{e\rho}
 =\frac{2D}{eK}\sqrt\epsilon.
 \end{aligned}
 \tag{S15}
\]

If the generating bound uses `n+q+1`, put `x=n+q` and use

\[
 e^{D\epsilon(x+1)}-1
 =e^{D\epsilon}(e^{D\epsilon x}-1)
     +(e^{D\epsilon}-1).
\]

Equation (S15) and `e^{D epsilon}-1<=C epsilon` give

\[
 \sup_{x\ge0}e^{-\rho x}
       [e^{D\epsilon(x+1)}-1]
 \le C_{D,K}\sqrt\epsilon.
 \tag{S16}
\]

Consequently use, for this stronger application,

\[
 \nu_k=\nu_0-\sum_{j\le k}\rho_j,
 \qquad
 \eta_k=\eta_0-\sum_{j\le k}\rho_j,
 \qquad \rho_j=K\sqrt{\epsilon_j}.
 \tag{S17}
\]

The zero-attachment term still carries coefficient one. The entire nonempty near-attachment family, in the new norm, has an extra factor at most `C sqrt(epsilon_k)` times the old norm. This conclusion is uniform in the number of old cells and component tags. There is no bound on that number hidden in its proof.

The AF calculation (S3)--(S5) applies equally to `sqrt(epsilon_j)`, with half the fixed exponents. Thus `sum rho_j=o(1)` and the positive floors for all auxiliary rates remain uniform in the depth. A finite number of subsequent fixed fractional-power extractions changes the collar coefficient and inverse-coupling/logarithmic powers, but preserves the same summable class.

More generally, a decrement `K epsilon^a`, `0<a<1`, leaves a fresh factor `C epsilon^{1-a}`. The square-root choice treats the two budgets symmetrically. It is an estimate on the auxiliary expansion weights; it makes no change to the current cutoff, native profile, physical geometry or source action.

For mixed far/near attachments, the far factor `exp(d_k ell_old)` is first paid from the physical coarsening reserve as in (S6a). A family with a near attachment then uses (S16). A nonempty family containing only far attachments needs its separately proved global old-port/ordinary-buffer crossing, paid from the remaining connector reserve. Formula (S16) does not supply that geometric crossing.
