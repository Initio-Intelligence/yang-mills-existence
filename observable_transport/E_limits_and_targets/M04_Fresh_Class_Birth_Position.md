# What a fresh support class records about an old birth position

This note answers a geometric question left by the support-class cancellation theorem. With the literal finite graph average and fixed fresh cutoff rules, a fresh class contains no information about an earlier birth position beyond the prepared core itself. That statement does **not** imply that the conditional law of birth positions is diffuse. The map from fine birth geometry to a coarse core can have thin fibers, and the actual positive old weights need a separate comparison.

## 1. The source separates the fresh graph from the old annular graph

The displayed sum in LFR I (1.100), printed p.201, has separate graph arguments `G_i` and `T_i`. The fresh numerator and denominator use `delta_{G_i}` on the current core `Lambda_i`; the old integral uses `delta_{T_i}` on the mixed determining set `B_i`. The latter set and its old rectangular annuli can change with the internal history while the fresh core and fresh graph stay fixed.

The source then replaces the graph-family average by the finite average over the coordinate permutations and coordinate reflections. Every admitted rectangular chain admits the old construction in each of these coordinate systems. This follows directly from the p.196 construction: the outer corner, the auxiliary number inside the inner first-coordinate interval, and the detoured tree are chosen for the rectangles of that history. They are not extra restrictions requiring those rectangles to have predetermined endpoints.

Thus fixing a coordinate orientation fixes a rule for constructing the old tree. It does not fix the old tree as an embedded set independently of the history. The actual embedded old tree remains an internal variable, as is also explicit in LFR II (1.71), printed p.379. The finite orientation weights are the same for every admitted history. Whether duplicate orientations give the same fresh graph only changes their finite multiplicity.

The fresh graph is an axial graph of the full current rectangle `Lambda`. Its inputs are that rectangle and the chosen orientation/anchor convention. It has no argument consisting of `B''_k`, an older annulus, or an old birth endpoint. The fresh homogeneous determining map, the minimal reference orbit, and the quotient `h/H` likewise have the inputs identified in FS.4. In particular, the fresh reference does not import the old mixed tree through its gauge representative.

## 2. Exact class-map factorization

Write `gamma` for the complete internal old geometric history and preparation choices, before the finite orientation is selected. Fix the source scale parameters and a deterministic choice of the fresh localized-action cutoff and representative rules. Let `Theta` be the finite coordinate orientation set. The literal construction gives

\[
 \Phi(\gamma,\theta)
  =\bigl(\Lambda(\gamma),\,
          Y(\Lambda(\gamma)),\,
          G_\theta(\Lambda(\gamma)),\,
          \text{fixed fresh rules}\bigr).
 \tag{FP.1}
\]

Here `Y(Lambda)` is the exact quiet-component map CG.2. Any reference-shell argument is a retained field argument, not an old geometric label.

### Proposition FP.1 — no additional birth-location label

Conditional on outer component admission, the complete fixed-rule fresh class map factors as (FP.1). At a fixed core and class `r`, the permitted orientation set

\[
 \Theta_r(\Lambda)
  =\{\theta\in\Theta:
        \Phi(\gamma,\theta)=r
        \text{ for histories with core }\Lambda\}
 \tag{FP.2}
\]

does not depend on the older history. Accordingly the complete old measure of the class has the exact form

\[
 M_r
  =\sum_{\theta\in\Theta_r(\Lambda)}w_\theta
       \sum_{\gamma:\,\Lambda(\gamma)=\Lambda}
         M_{\gamma,\theta},
 \tag{FP.3}
\]

with the actual old native selectors, all continuous old integrations, successful-component summation and all cross interactions retained in `M_{gamma,theta}`.

**Proof.** The p.201 factorization first separates the outer component collection from its internal localized histories. For each such history, the p.196 tree construction and every finite coordinate orientation are available. The fresh factor of (1.100) has exactly the arguments in (FP.1), whereas all old graph and preparation changes occur in the old integral. CG.2 removes the separate final-component argument. Grouping the actual positive summands by their common fresh factor gives (FP.3). No old history or selector is replaced by a trial law. \(\square\)

The proposition is an identity of the allowed index set and of the decomposition of the positive measure. It does not say that every summand has the same mass, or even that every geometrically possible history is positive at every fixed retained field. Such questions concern the actual old integral in (FP.3).

If the selected convention leaves a fresh cutoff, a localized-action function, or another fresh choice genuinely dependent on an old descriptor, that choice must remain in `Phi`. Its dependence must be examined rather than declared local by its name. FS.4 and FP.1 apply to fixed fresh rules; equal-support but unequal-kernel choices retain their actual within-support posterior.

## 3. Why finite local coding alone does not prove dilution

Although the range of the local core/graph code has bounded current physical support and only finitely many shape values at a fixed anchor, one particular value can have a small inverse image among fine birth positions. There is no counting principle that forces every fiber of a finite map to be large. Nested grid rounding is a concrete source of this effect.

For a constant-`R` quiet interval, write

\[
 a_j=M R L^{j-k},\qquad
 k_0=k-N_0,\qquad a_{k_0+1}=M.
 \tag{FP.4}
\]

For one rectangular predecessor with lower endpoint `t`, width `w`, and total subsequent one-sided padding `A`, its final current-`M` cover in that coordinate is

\[
 [M\lfloor(t-A)/M\rfloor,
   M\lceil(t+w+A)/M\rceil].
 \tag{FP.5}
\]

If that cover is `[b,b+qM]`, the allowed real translation interval is the intersection

\[
 [b+A,b+M+A)
   \ \cap\
 (b+(q-1)M-w-A,\ b+qM-w-A].
 \tag{FP.6}
\]

Its length is

\[
 \bigl[M-|\,(q-1)M-w-2A\,|\bigr]_+.
 \tag{FP.7}
\]

Endpoint conventions affect only boundary points. Thus a rounding resonance can make the interval microscopic even though its final core label has bounded current support. The finite graph average does not repair or create that resonance.

## 4. A geometric extension from one ancestor to the literal inner chain

The following observation reduces a multiple-ancestor concern to the same endpoint arithmetic. It concerns allowed geometries, without asserting comparability of their old weights.

By MW.1, all `h`-ancestors in one literal eligible prepared component lie in **one** actual rectangular component at scale `h+1`. Let that rectangle have coordinate widths at most `100 a_{h+1}`. Translate the entire collection of `h`-ancestor rectangles by a vector in `a_{h+1} Z^4`. On a constant-`R` interval this is also an allowed `h`-grid translation. The `h` to `h+1` cover, padding, component joining and rectangular hull commute with this translation. Hence the first merger pattern is unchanged exactly. This is why the translation step is `a_{h+1}`, not the smaller `a_h`.

From scale `h+1` onward there is one rectangle. Its later quiet evolution consists of covers and added layers. The nested grids give (FP.5), now with

\[
 A=10\sum_{j=h+2}^{k_0} a_j
   =\frac{10M}{L-1}
       -\frac{10L a_{h+1}}{L-1},
 \qquad w=O_L(a_{h+1}).
 \tag{FP.8}
\]

This follows by composing the one-dimensional floor/ceiling cover maps; each subsequent grid is an integer coarsening, and its endpoints are endpoints of the preceding grid. The rectangular hull is already inert after `h+1`.

Suppose

\[
 \delta_L=\operatorname{dist}\left(\frac{20}{L-1},\mathbb Z\right)>0.
 \tag{FP.9}
\]

Since `w+2A=(20/(L-1))M+O_L(a_{h+1})`, every nonempty cover fiber in (FP.7), for `a_{h+1}/M` sufficiently small, has length at least

\[
 \delta_L M-O_L(a_{h+1}).
 \tag{FP.10}
\]

It therefore contains order `M/a_{h+1}` permitted whole-cluster translations in each coordinate. All those translations give the same final `M` cover, hence the same `Lambda` and the same fresh class at fixed orientation. The rectangle size condition stays valid: after the initial admitted `h+1` rectangle, one quiet step has width in its next-grid units at most `100/L+22`, which is strictly below 100 for the source's `L>11`; later steps satisfy the same bound. The entire previous cluster is simply translated, so the `h`-scale size conditions are unchanged.

For the source restriction that `L` is odd and greater than 11, the elementary resonance `20/(L-1)` being an integer occurs at `L=21`. This statement identifies a possible geometric exceptional value; it is not a permission to change a specified selected `L`. The fixed-rule class factorization FP.1 holds at that value as well, while the broad-fiber conclusion (FP.10) does not.

One can realize these shifted geometries by the same young R-only replacement method as MW.2: reproduce the complete shifted `h`-ancestor collection and follow its quiet sequence. The same final core and the fixed fresh conventions give the same fresh factor. Admission of the actual old continuous trial boxes remains the separate source-specific assertion of the young-trial theorem; the geometric calculation itself is independent of those estimates.

### 4.1. Two adjacent radius levels remove the plateau assumption

There is a useful stronger version, valid for the literal padding convention. It permits the radius sequence to move in either direction between two adjacent powers of `L`.

First, the actual native coupling comparison supplies this two-level property on the source's chosen preparation horizon `N=O(R_k)`. Put `x_j=log g_j^{-2}`. CMP119 (2.6) gives, for `k-N<=j<=k`,

\[
 -2\log(1+\beta_0)
 \le x_j-x_k
 \le\log(1+g_k^2\beta' N).
 \tag{FP.11}
\]

Thus the complete range of `x_j` has bounded width and `x_k` tends to infinity. The ratio of the largest and smallest `x_j^r` tends to one. Since `R_j` is the least power of `L` above `x_j^r`, all `R_j` in this interval belong to two adjacent powers, once the weak-coupling ceiling has been reduced. This conclusion uses neither monotonicity of the radius sequence nor positive-terminal-coupling control.

Let `n=k0+1` be the actual source preparation index with `a_n=M`. The grids remain nested because their successive ratios are in `{1,L,L^2}`. Starting from the scale `h+1` rectangle, the padding is exactly

\[
 A=10\sum_{j=h+2}^{n-1}a_j,
 \qquad
 \frac{2A}{M}
   =20\sum_{q=1}^{n-h-2}
          L^{-q}\frac{R_{n-q}}{R_n}.
 \tag{FP.12}
\]

In particular no final `M`-mesh padding is inserted before the cover in (FP.5). There are at least two terms for the source's sufficiently weak preparation, because `N-N0` tends to infinity.

Write `alpha=2A/M`. The following intervals contain it:

| Final radius and immediately preceding radius | Interval for `alpha` |
| --- | --- |
| Final radius is the larger of the two levels | `[20/L^2, 20/(L-1)]` |
| Final radius is the smaller level; previous radius is also smaller | `[20/L, 20/L+20/(L-1)]` |
| Final radius is the smaller level; previous radius is larger | `20+[20/L^2, 20/(L-1)]` |

These bounds follow by separating the first term in (FP.12); in the last row, the second term supplies the displayed positive lower bound on the tail. For every `L>=41`, all three intervals stay at distance at least `20/L^2` from an integer. The only tight comparison is

\[
 \frac{20}{L}+\frac{20}{L-1}+\frac{20}{L^2}<1,
 \tag{FP.13}
\]

which holds at `L=41` and improves with increasing `L`.

Consequently every nonempty final-cover fiber has translation length at least

\[
 \frac{20}{L^2}M-O_L(a_{h+1}),
 \tag{FP.14}
\]

uniformly over these two-level radius sequences. The conclusion is the same many-shift geometric fiber as before.

The intermediate size condition is also preserved. A step with mesh ratio one can occur only on a transition from the larger radius to the smaller radius and cannot occur twice consecutively. If it is the first step after `h+1`, our translations are multiples of that unchanged mesh, so its original admissibility is preserved exactly. After the first genuine coarsening, every translated rectangle has width at most `100/L+22` in its new mesh units. A possible subsequent ratio-one step adds at most 20, still leaving a strict margin below 100 for `L>=41`. This controls every later scale without a monotonicity assumption.

CMP109 p.251 permits an odd integer `L>11`, and CMP119 p.245 then chooses the block constants, including `M=L^m`, sufficiently large. The illustrative `L=13` is only an example checking elementary inequalities, while its geometry theorem chooses one admitted odd `L`. Thus selecting an admitted odd `L>=43` is compatible with these source restrictions when the construction parameters remain selectable. This is not a replacement of any numerical `L` already specified in a separate implementation.

## 5. Remaining analytic issue

Equations (FP.3) and (FP.10) remove a possible hidden **geometric** source of birth-position pinning for the stated nonresonant quiet geometry. They do not give a bound of the form

\[
 \mathbb P(\text{birth near a specified microscopic cell}
        \mid \text{fresh class and retained output})
 \lesssim a_{h+1}^{4}.
\]

Such a bound would require comparing the actual normalized old weights under the admissible shifts, including their old Schur precisions, the retained background, all old selectors, and all cross interactions. A positive trial event or a bound `exp[-C P(g)^2]` for each trial is insufficient: its unspecified exponential constant can dominate the geometric multiplicity. The current raw-carrier and microscopic marked-moment gaps therefore remain separate.

## Sources

- LFR I, printed pp.195-196: mixed annular tree construction for every admitted rectangular chain.
- LFR I, printed p.201, (1.100)-(1.101): separate fresh and old graphs, common finite coordinate-orientation average, and fresh kernel arguments.
- LFR II, printed p.379, (1.71): localized old histories and the coordinate-rotated old tree stay in the old component operation.
- CMP119, (2.5)-(2.6), (3.2)-(3.5): quantized radius, native coupling comparison, and quiet next-grid cover/layer rules.
- CMP109, printed p.251: `L` is an odd integer greater than 11.
- [M04 Bounded Core Source Map](../A_support_and_normalization/M04_Bounded_Core_Source_Map.md), CG.2-3; [M04 Fresh Support Class Cancellation](../A_support_and_normalization/M04_Fresh_Support_Class_Cancellation.md), FS.4; [residual merger witness](../A_support_and_normalization/residual_merger_witness.md), MW.1-2.
