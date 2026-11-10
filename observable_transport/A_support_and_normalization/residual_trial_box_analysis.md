# The actual residual trial box: flat positive action and strict cutoffs

the trial in [residual trial mass](residual_trial_mass.md). The primary formulas used here are
LFR I (1.81)--(1.98), LFR II (1.20)--(1.21) and (1.46)--(1.48), CMP102
Theorem 1 and Proposition 9, and the exact free-coordinate reconstruction in
CMP119 (3.15)--(3.19).

**Current geometric scope.** The cutoff/energy calculation is first made
for the unmerged trial. Lemma MW.1 and Theorem
MW.2 in [residual merger witness](residual_merger_witness.md) now extend its trial scope to every
complete fresh-reference class in the literal one-component
rectangular-chain preparation of LFR I pp.195--196. They bound the total
number of early ancestor cubes by the inner preparation rectangle, then
clone **all** the original early components. The entire later geometry and
fresh kernel are preserved. The full old sum still contains all its
histories; only a positive lower trial is replaced. This is not an extension
to an unspecified forest version of the preparation, and it is not inferred
from the size of the final prepared core alone.

## 1. The decisive literal simplification

The positive term called `S` in the final old operation is **not** the Wilson
action of the joined reference field `U_0`. The primary image of LFR II
p.368, (1.46), expands the reference-potential dependence off the local
configuration. Its remaining real field is explicitly

\[
 U''_{h+2}(\exp(i g_k B),V''),
\]

and (1.48) puts precisely this field in the nonnegative Wilson term. The
reference-potential correction belongs to the bounded terms denoted `O(1)`
there and subsequently included in the actual self interaction. It is not
still present in this positive `S`.

For the fresh `R`-only birth under consideration, `Ω_h` remains full in the
local old core. Hence no local raw determining coordinate of scale below
`h` remains: the birth fluctuation `A_{h-1}` is a coordinate in `T_h`, not a
`Γ_{h-1}` determining datum. The inner `V''` argument of the above minimum
therefore consists of the old current variables `V_h` on this core. It
follows that

\[
 B=0,\qquad V_h=I
 \quad\Longrightarrow\quad
 U''_{h+2}(\exp(i g_kB),V'')=I,
 \qquad S=0.                                         \tag{TB.1}
\]

The equality is exact. It is the identity minimizing configuration with all
its actual determining data equal to the identity. The background-dependent
gauge transformation in (1.46) does not affect the Wilson action.

Choosing this old-coordinate center does not change the fresh reference
class, the external retained shell, or the operation being normalized. The
original joined field is reconstructed through its same `U_0` and the same
preparation maps. Only its permitted old integration coordinates have been
chosen. The background action canceled in the source algebra still occurs
in the original outer density.

## 2. Strict preparation admission at the flat center

The independent preparation variables are those of the literal integral
(1.71) of LFR II: the tree-fixed `B` coordinates, the old raw current
coordinates `V_h`, and the surviving coordinates of `T_h`. On

\[
 \Lambda_0=\Lambda\cap\Omega_{h+1}^{\prime\prime\,\sim2},
 \qquad \mathbb B_0=\mathbb B''_k\cap\Lambda_0,
\]

the preparation variable is `V'=exp(i g_k B)`. Thus `B=0` makes `χ'=1`
with strict margin. The other preparation selector is a test of the filled
field `(1,V_h)`. For `V_h=I` the entire filled field is the identity, so
`χ_{h,1/2}=1` exactly, including every artificial seam. This avoids the
need to estimate the reference average at that seam.

The common shell selector `χ_{k,Λ}` is already fixed to its good alternative
for this complete fresh-reference class. The source identity LFR I (1.89)
then restores the original `χ''_k` on the joined background. It is this
literal implication, including all compensating gauge transformations,
that proves admission. A separate estimate using a different old cutoff is
not substituted for it.

The `R`-birth seed is reconstructed by CMP119 (3.15), including its nonlinear
constraint correction. Its prescribed `h`-average is therefore exactly
`V_h`, even though the microscopic field is changed. The seed does not alter
either of the preceding preparation tests.

## 3. A joint positive-volume box

Let `a_N=c(1+N)^{-2}`. Use the following product neighborhood in the final
independent variables:

* each independent tree-fixed `B` coordinate has norm at most `a_N`;
* each old raw `V_h` link is `exp(i g_h b_h)` with `|b_h|≤a_N`;
* each birth free coordinate lies in an `a_N` neighborhood of its prescribed
  seed or zero center.

These are separate independent coordinates in the final source integral.
They are not obtained by multiplying inverse condition numbers for `N`
successive coordinate changes.

For `B`, the literal cutoff is `g_k|B|<δ'_k`. Its normalized threshold
diverges, so the first box is strictly inside it. For the filled `V_h`
test, every raw link differs from identity by at most `C g_h a_N`, including
the artificial seam. The local variational response about identity gives

\[
 |U_{h,\square}((1,V_h);\partial p)-I|
       \le C g_h a_N\,(L^{k-h}\eta)^2
       <\tfrac14\varepsilon_h\,(L^{k-h}\eta)^2        \tag{TB.2}
\]

for sufficiently weak coupling. Here the full determining footprint of a
nontrivial seam test lies inside the prepared domain; the source old-core
collars and `N≫N_0` give this inclusion. As before, (1.89) proves all the
original joined-background preparation restrictions.

The birth free-coordinate seed has magnitude `3δ_{h-1}/(2g_{h-1})` on one
fixed physical direction. Its `a_N` neighborhood retains a fixed fractional
margin from the `R` threshold. The exact constraint map has uniform local
row bounds, and its nonlinear correction is `O(δ_{h-1}^2)`. Hence the
reconstructed relative links remain below the `2δ_{h-1}` approximate `Q`
threshold. The discrepancy between the true reference and the local test
reference is the source exponentially small error in (3.17)--(3.19), not a
new accumulation over chronological steps. The curvature and soft-gauge
variation of this fixed-stencil seed is `O(δ_{h-1})`, below the `ε`
threshold by the fixed `A_1/A_0` hierarchy. Noise of size `a_N` in all
remaining free coordinates preserves these bounds by the same local row
estimates.

Thus the product box is a joint admissible positive-volume box once the
source geometric seed placement and its exact `R` cover have been matched.
Those matching facts are separately proved in RT.1. The statement does not
cover a history whose earlier raw determining variables remain in this core.

## 4. The positive Wilson energy on the whole box

Set `ℓ_j=L^jη`, so that `ℓ_k=1`. Every determining link of the remaining
real minimum in (1.48) is either `exp(i g_k B)` or a `V_h` link. The
couplings `g_k,g_h` are comparable on the admitted `N=O(R_k)` segment.
Consequently each such link differs from identity by at most `C g_h a_N`.

The mixed plaquettes in CMP102 condition (7) use a fixed number of these
links; at an interface a coarse edge is replaced by its fixed `L`-scale
subdivision. The number of factors is bounded by a constant depending on
the fixed `L,d`, not on `N`. Their regularity parameter is therefore

\[
 \varepsilon_1\le C_L g_h a_N.
\]

CMP102 Theorem 1, (8), applies to this actual determining set and gives, on
a region of determining scale `j≥h`,

\[
 |U''_{h+2}(\partial p)-I|
       \le C g_h a_N\,\eta^2\ell_j^{-2}
       \le C g_h a_N\,\eta^2\ell_h^{-2}.             \tag{TB.3}
\]

One may equivalently integrate the derivative estimate (190) from the
identity. The direct real regularity theorem is enough here. The absence
of scales below `h` is essential to the last inequality.

On this fresh branch the remaining local inverse coupling is bounded by
`C g_h^{-2}`. The support of the literal `ζ_1` has physical volume at
most `C_M R_h^4 ℓ_h^4`. For a unitary plaquette,

\[
 s(P)=N-\operatorname{Re}\operatorname{Tr}P
     =\tfrac12\|P-I\|_{\mathrm{HS}}^2.
\]

Using `0≤ζ_1≤1`, (TB.3), and the fine plaquette count therefore gives

\[
 \begin{split}
 S&\le Cg_h^{-2}\,
       \frac{\operatorname{Vol}(\operatorname{supp}\zeta_1)}{\eta^4}
       \left(g_h a_N\eta^2\ell_h^{-2}\right)^2\\
  &\le C_M a_N^2 R_h^4.                              \tag{TB.4}
 \end{split}
\]

The fine-lattice count cancels exactly in four dimensions. There is no
`R_h^4 P(g_h)^2` loss. Using the whole cutoff ceiling `ε_h` in place of
the actual box size in (TB.3) would incorrectly introduce that loss.

The birth fluctuation has not been hidden in (TB.4): it contributes its
`C P(g_h)^2` quadratic/soft-gauge cost in `T_h`, as RT.1 records. It does
not enter the determining field of this remaining positive Wilson term.

## 5. The outer preparation quadratic

The other positive term is the literal form LFR II (1.21), up to its fixed
coefficient convention,

\[
 Q_B=\tfrac12\sum_p\eta^4\zeta(x(p))
                     |D H''_{k,Z}B(p)|^2.
\]

For a conservative estimate, sum the normalized per-scale response bounds
of CMP102 (190) before using their interscale decay. On an output region
with determining scale `j`, this gives

\[
 |D H''_{k,Z}B|\le C(1+N)a_N\ell_j^{-2}.             \tag{TB.5}
\]

The background is in the admitted source regular class, so the same bounds
hold at its actual reference. This is a single response operator on a mixed
determining set, not a product of `N` unrelated inverse maps.

Define the actual mixed determining-volume count

\[
 D_{\rm geo}=\sum_{j=h}^{k}
    \frac{\operatorname{Vol}(\text{relevant }j\text{-scale region})}{\ell_j^4}.
\]

Equations (TB.5) and the trial radius imply

\[
 Q_B\le C(1+N)^2a_N^2D_{\rm geo}\le C D_{\rm geo},
 \qquad D_{\rm geo}\le C_M\sum_{j=h}^{k}R_j^4
                        \le C_M R_k^5.              \tag{TB.6}
\]

If the post-tree independent-coordinate count is explicitly shown comparable
to this determining volume, one may replace `D_geo` by `D_tr`. That
comparison is not necessary for the proposed lower bound: retaining both
counts still gives the same `C_M R_k^5` cost.

Together with RT.1, the verified positive-energy bound is therefore

\[
 Q+S+\mathcal G
       \le C P(g_k)^2+C(D_{\rm tr}+D_{\rm geo})
       \le C P(g_k)^2+C_M R_k^5.                     \tag{TB.7}
\]

## 6. What this analysis accepts and what it leaves to the full mass proof

This check accepts the positive-action and joint-cutoff parts of the fresh
`R`-birth trial, with the improved center `(B,V_h)=(0,I)`. It corrects the
earlier reference-centered wording: the literal positive `S` has already
lost its `A_0` dependence, so its zero center and small-box estimate are
direct consequences of the source minimum.

To conclude RT.17, the separate action/normalization analysis must still keep
every Haar-coordinate power, Gaussian normalization, vacuum term and old
boundary/self term exactly once. A term depending on unreplaced exterior
data can be canceled only when it is a common retained-only factor in the
matched numerator and denominator convention. The cross-component
interaction in RT.4 must also be retained for the complete conditional law.

The argument is restricted to the literal fresh-birth eligible branch with
`h≥1`, no earlier internal raw determining data, and the same complete
fresh-reference class. It does not supply the separate `h=0` case or change
the physical carrier cost of the normalized residual quotient.

## 7. analysis of the weighted native source consequence

The subsequent algebra in [residual trial mass](residual_trial_mass.md), RT.19--RT.29, is valid
at its stated native fixed-support scope. For clarity, its two inputs are
the proved matched energy/rank tail for the actual old posterior, and the
source's pointwise relative native density comparison
`dM_ξ=e^{σ_ξ}dM_0`, `sup|σ_ξ|≤δ<log 2`.

The latter gives

\[
 |\nu_0(e^{\sigma_\xi})-1|\le e^\delta-1<1,
 \qquad |\nu_\xi|\le
      \frac{e^\delta}{2-e^\delta}\,\nu_0.
\]

The matched tail at scale `K=1+P(g_k)^2` gives bounded
`ν_0 exp(cE/K)` and `ν_0(E exp(cE/K))≤CK`. Hence an incoming native
analytic mark with its explicit pointwise envelope `|F_ξ|≤bE` has
`|ν_ξ F_ξ|≤CbK`, and

\[
 |\nu_\xi(e^{\lambda F_\xi})-1|
       \le C|\lambda|b\,\nu_0(Ee^{|\lambda|bE})
       <\tfrac12
\]

on a fixed sufficiently small disk `|λ|<c/(bK)`. Thus the marked source
disk and its cumulant bounds follow from the actual posterior comparison;
they are not inserted as a new zero-free hypothesis.

Independent insertion and kernel parameters give the direct expectation
and normalized score covariance separately. Cauchy bounds the insertion
derivative by `CbK/ρ` and the score by `Cδ/ρ`. The exact rectangular
endpoint formulas RT.29 then give the M.30 decomposition on paths inside
that native chart.

The mark envelope `|F_ξ|≤bE` is an explicit **input** condition. It has
not been established for an arbitrary microscopic mark transported through
all prior steps. Likewise the native parameter `ξ` is not an independent
raw retained link or a discrete reference-class change. The theorem's
stated exclusions of those extra pullbacks, scores and physical carrier
costs are necessary and correctly preserved.
