## Analysis of the normalized preparatory cutoffs


**Status:** a literal-source normalization issue in the printed formulas. It does not invalidate the exact partition identities, the law-level H-03 identities, or the first-step results using CMP119 (1.18). It prevents assigning a large logarithmic failure threshold to every later quiet selector without an explicit convention repair.

## 1. What the primary formulas say

Let

\[
 P_1(g_j)=A_1p_1(g_j),\qquad
 \delta'_j=g_j P_1(g_j).
 \tag{CN.1}
\]

This is the explicit definition at the top of LFR I, printed p.183, immediately after (1.27). Here `p_1(g)=(log g^{-2})^{p_1}` and the exponent satisfies `p_1<p_0`.

On printed p.187, (1.53) defines the unscaled logarithmic fluctuation `B'_j=(1/i)log V'_j`. The paragraph after (1.54) then states the scaling transformation

\[
 B'_j=g_j B_j.
 \tag{CN.2}
\]

The immediately following page, printed p.188, displays

\[
 \chi'^{(j)}
 =\mathbf 1\{\,|B_j(b)|<\delta'_j
       \text{ on the stated free bonds}\,\}.
 \tag{CN.3}
\]

This is literal (1.55). The same page uses `exp(i g_j B_j)` in (1.59), and its (1.60) has the normalized Gaussian form

\[
 -\tfrac12\langle B_j,C^*\Delta^{(j)} C B_j\rangle,
 \tag{CN.4}
\]

with no extra factor `g_j^{-2}`. Thus a reversion to the unscaled `B'_j` notation cannot explain (CN.3) while keeping the other formulas on that page unchanged.

The dimensionless radius corresponding to the unscaled radius `delta'_j` would instead be

\[
 |B_j|<g_j^{-1}\delta'_j=P_1(g_j).
 \tag{CN.5}
\]

Equations (CN.3) and (CN.5) are different selectors. The present analysis does not silently replace one by the other.

Primary pages:

- Bałaban, Large Field Renormalization I, p. 183;
- Bałaban, Large Field Renormalization I, pp. 187–188.

## 2. The general ordinary-step ambiguity is already recorded

The discussion of the exact marked kernel near formula (3.14) explicitly records the following source facts:

1. CMP119 printed p.267 scales `A'_k=g_k A_k`.
2. Its (3.16), printed p.268, displays the good-field radius `|A_k|<delta_k`.
3. The initial-step (1.18) instead explicitly uses `|A|<g_0^{-1}delta_0`.
4. The source text does not identify these two normalized radii; its exact identities use the actual selected domain.

Annex BD, immediately after (BD.11), again leaves the normalization check open. It also distinguishes the unprimed `p_0` cutoff from the primed preparation polynomial. No correction of LFR I (1.55), or blanket convention resolving both printed formulas, is given in the H-03 analysis or the related reset-normalization arguments.

This is therefore not a permission to alter the stated operation. The source formula and the existing text both require the convention to remain explicit.

## 3. Why the distinction changes the proposed energy comparison

Consider a fixed nonzero normalized Gaussian coordinate `b` with density proportional to `exp(-kappa b^2/2)`, where `0<c<=kappa<=C`. A bad event for the literal selector (CN.3) has threshold

\[
 |b|\ge gP_1(g).
 \tag{CN.6}
\]

For any fixed `g` choose `b=2gP_1(g)`. Its normalized quadratic energy is

\[
 E(b)=2\kappa g^2P_1(g)^2.
 \tag{CN.7}
\]

In particular, if `R(g)` is a fixed power of `log g^{-2}`,

\[
 \frac{E(b)}{P_1(g)^2/R(g)^9}
 =2\kappa g^2R(g)^9\longrightarrow0.
 \tag{CN.8}
\]

Consequently the implication

\[
 \text{failure of (CN.3)}
 \quad\Longrightarrow\quad
 E\ge cP_1(g)^2/R(g)^9
 \tag{CN.9}
\]

is false even for a fixed positive Gaussian form. No dimension or denominator estimate repairs this deterministic implication.

There is a corresponding probability test. In a fixed positive-dimensional Gaussian block,

\[
 \mathbb P\{|b|<gP_1(g)\}=O(gP_1(g))\longrightarrow0,
 \qquad
 \mathbb P\{|b|\ge gP_1(g)\}\longrightarrow1.
 \tag{CN.10}
\]

For a fixed `m`-dimensional nondegenerate block, the small-ball probability is of order `(gP_1(g))^m`. Therefore a failure bound of the form `exp(D-cP_1(g)^2/R(g)^9)` with `D=o(P_1(g)^2/R(g)^9)` cannot hold for this literal normalized selector merely from Gaussian positivity.

This diagnostic uses the same normalization as (CN.4). It is not a counterexample to the source's complete multiscale theorem under an intended corrected convention, nor a proof that every such Gaussian point is a complete eligible history.

At the level of the local chart the discrepancy is also visible directly: `B_j=2delta'_j v` gives a physical relative bond angle of order `g_j delta'_j=g_j^2P_1(g_j)`. It can fail (1.55) while remaining far inside the earlier group-valued test `|exp(i g_jB_j)-1|<2delta'_j` in (1.59). Thus that earlier test does not automatically remove the low-energy discrepancy.

## 4. What LFR II actually supplies

LFR II, printed pp.381–383, explicitly discusses preparation failures from:

- the improved background selectors;
- LFR I (1.27);
- the second term of LFR I (1.28);
- the shell selector (1.75);
- the final axial selector (1.82).

For the final axial selector the source explicitly converts the normalized bad coordinate as `|B(b)|>=g_j^{-1}delta'_j=A_1p_1(g_j)` on p.383. The source then obtains the weakest listed exponential rate of order `p_1(g_j)^2/R_j^{d+5}`.

The displayed catalog on p.381 does not separately list the failed annular selector (1.55). Therefore that paragraph cannot be cited, without an additional identification, as a proof of (CN.9) for the literal (1.55).

The successful factors (1.55) are integrated in LFR I (1.60) and their exact completion factors enter the boundary action through (1.62). They must be retained with their actual radii when restored. Integration into a completion factor does not change the selected set or supply a large failure threshold.

## 5. Consequences for the present first-family route

The following proved parts survive unchanged:

- the first birth comparison, which uses the unambiguous initial CMP119 (1.18);
- exact first-energy cancellation and the separation of the first rare birth from later variables;
- exact Fubini/restoration identities with all original cutoffs kept;
- convex-cutoff reserves that do not assume a lower bound for cutoff probability;
- source energy/Schur identities on their admitted charts;
- the direct final-axial `chi'` failure argument using the explicitly normalized p.383 threshold;
- all abstract mass-exchange theorems with their stated hypotheses.

What is not yet justified is a catalog assertion that every alternative-history quiet failure has energy at least `H_R=c p_1(g)^2/R^9`. In particular, literal restored factors (1.55), and the general-step (3.16) convention, must not be included in that assertion by analogy with the initial step.

There are three logically distinct possible next steps:

1. Locate and document a source convention or correction making the intended normalized radii explicit, then prove that the specified operation uses it.
2. Keep the literal radii and compare the corresponding small-ball completion factors relatively, without treating their complements as rare high-energy events.
3. Prove that the particular comparison under study exposes only a verified subset of selectors, and carries every remaining literal cutoff in an exact common or separately controlled completion factor.

This analysis supplies none of these additional identifications automatically. It records the source issue before it can be hidden in a selector-energy catalog.

## 6. Conclusion

The normalization discrepancy is verified, and the large-deviation substitution is invalid without further input. The exact native first-step results and the law-level normalized identities retain their stated scopes. No full M-04 closure, no redefinition of the source operation, and no failure of the actual intended Yang–Mills construction is claimed here.
