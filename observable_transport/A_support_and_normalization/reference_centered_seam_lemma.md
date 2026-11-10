# A reference-centered trial satisfies the literal filled-field cutoff

This lemma isolates a source-coordinate check useful for an
old residual-component denominator trial. It does not estimate that
denominator by itself.

## Statement

Fix an admitted prepared component of LFR I, with its actual shell, prepared
core `Λ`, old inner scale `h`, final scale `k`, and chronological separation
`N=k-h`. Let

\[
 U_0=U_{k,Y}(V_\Lambda)
\]

be the literal classical reference minimum of LFR I (1.77)--(1.79). Choose
its axial/Landau representative from (1.85)--(1.87). On the mixed annular
coordinates choose the trial `B'=0`. On the old `h`-current determining data
entering the preparation choose the reference average

\[
 V_h=M^h(U_0^{AL}).                                   \tag{SC.1}
\]

Assume the full determining footprint of each nontrivial
`χ_{h,1/2}` seam test cube lies inside `Λ`. This holds for the source's
old/prepared collars once `N` is sufficiently large: the old `h`-scale test
diameter in final units is `O(M_2R_h L^{-N})`, whereas `Λ` has its fixed
`M` collar around the prepared core.

Then, for all sufficiently large admitted `N`, the literal field `(1,V_h)`
satisfies `χ_{h,1/2}=1` with a strict margin. The assertion is uniform over
the admitted shell and does not require a remote-pulse or flat-shell
construction.

## Proof

The source AL bound is

\[
 U_0^{AL}=e^{i\eta A_0},\qquad
 \|A_0\|+\|\nabla A_0\|+\|\nabla^*\nabla A_0\|
           \le C_M\varepsilon_k                     \tag{SC.2}
\]

on the domain needed here; see LFR I (1.87). Its constant may include the
fixed source `B_3,B_5,M` factors. Formula (1.92) identifies the corresponding
old average with the exponential of its `h`-average. Equivalently, apply
CMP98 Proposition 6, (164), to the identity reference and the relative
potential `A_0`. Since the final current unit is `L^kη=1`, this yields

\[
 \sup_{b\text{ in a seam determining footprint}}
        |V_h(b)-I|
       \le C_M L^h\eta\,\varepsilon_k
       = C_M L^{h-k}\varepsilon_k.                   \tag{SC.3}
\]

The filled field has identity links on the filled side and the links (SC.3)
on the other side. Consequently **every** determining link obeys the same
bound, including links incident to the artificial interface. This handles
the seam at the level of raw links; it does not incorrectly identify its
plaquettes with the original reference plaquettes.

The local analytic variational map around the identity, with its actual
`h`-scale determining set, obeys the source curvature response estimate

\[
 \sup_{p\text{ in the tested cube}}
 |U_{h,\square}(W;\partial p)-I|
 \le C_{\mathrm{var}}\,\sup_b|W(b)-I|\,
                         (L^{k-h}\eta)^2.           \tag{SC.4}
\]

This is the small real specialization of the normalized derivative bound
in CMP102 Proposition 9, (190), at the flat reference. The bound (SC.3) is
inside its fixed small geometric domain. Substituting `W=(1,V_h)` gives

\[
 \sup_p|U_{h,\square}((1,V_h);\partial p)-I|
 \le C_{\mathrm{var}}C_M L^{-N}\varepsilon_k
                      (L^{k-h}\eta)^2.              \tag{SC.5}
\]

The source weak-coupling comparison used in LFR I (1.94) gives
`ε_k/ε_h≤C(1+N)^{1/2}` on this finite admitted segment. Hence choose `N`
large enough that

\[
 C_{\mathrm{var}}C_M C L^{-N}(1+N)^{1/2}<\tfrac14.
\]

Equation (SC.5) is then less than
`(1/4) ε_h (L^{k-h}η)^2`, strictly below the literal half-threshold in
`χ_{h,1/2}`. A test whose entire determining footprint is on the identity
side gives the identity minimizing configuration and needs no estimate.
This proves the claim. \(\square\)

## Source-coordinate qualifications

The preparation relative coordinate is on the exact domain

\[
 \Lambda_0=\Lambda\cap\Omega_{h+1}^{\prime\prime\,\sim2},
 \qquad\mathbb B_0=\mathbb B''_k\cap\Lambda_0.
\]

Outer boundary-crossing bonds belong to it; inner boundary-crossing bonds
do not. The AL change requires the compensating transformation of the old
`V_h` specified after LFR I (1.87). Thus (SC.1) is imposed in that actual
coordinate system, not before an omitted gauge compensation.

The lemma is stable under an old birth fluctuation whose exact block average
is unchanged. In particular, if an `R`-only birth is realized in the source
free coordinates with `Q a=0` and reconstructed by the exact nonlinear
constraint map, it preserves the current average (SC.1). Its internal
fluctuation changes the old core integrand but not this preparation test.
The linear condition `Qa=0` alone is not substituted for the nonlinear
constraint identity; the latter is part of the reconstruction.

Finally, neither setting `B'=0` nor this strict cutoff check gives a positive
volume contribution until one takes an actual old-coordinate neighborhood,
checks the original birth selectors there, and includes its coarea/Jacobian
and action. The lemma supplies one of those checks; it does not replace the
remaining mass calculation.
