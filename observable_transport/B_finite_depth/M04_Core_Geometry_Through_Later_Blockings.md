# Core geometry through later blockings

This note examines a possible all-depth use of the two-step proofs CA/TD. It proves a geometric recurrence and distinguishes three costs: the final carrier footprint, repeated analytic normalization losses, and the number of birth positions contributing to a later anchor. Only the first is controlled by contraction of physical cores alone.

## 1. Exact scope and support bookkeeping

At level j let the physical block side be h_j, with h_{j+1}=L h_j. All sizes below are in the current level's units. This is the convention of Annex Y, M.2: the carrier weight is exp(kappa times [block cardinality plus connecting-tree length]), not a count of original microscopic links.

CA.7 defines a core enlargement by taking the actual old nonanalytic input boxes C, all independent next coordinates in the fixed-L exceptional/gauge reconstruction stencil S, every next Q-reference box read at a slot of S, and the next R collar. The enlargement is a union of cubes. Merging overlapping components does not replace that union by its rectangular hull. Ordinary analytic connector supports receive only a fixed collar.

After a step, the chosen local core frame itself depends on the raw retained variables throughout D_C. Thus a later implementation must carry D_C as part of the nonanalytic dependency footprint when needed. It cannot keep only the original small birth box and silently discard the intermediate Q references or frame inputs. This is the conservative repeated rule analyzed below.

Every old latent integration variable remains in its certificate. The statements below do not bound the total old latent rank by the current core volume. They also do not compactly support the minimizing field: its analytic response tails remain in their full tagged connector carriers.

## 2. A geometric recurrence with all fixed constraint stencils

Let B_j(E) be the level-(j+1) block cover of a physical set E. Assign a coordinate to every block touched by its actual stencil; include boundary-crossing incidences. A fixed-L averaging, gauge, or exceptional-bond stencil enlarges the level-(j+1) cover by at most a fixed number of level-(j+1) blocks. The Q defining boxes and the source buffer add at most c_L R_{j+1} blocks in radius. The fixed outside grid and other fixed collars can be included by increasing this constant and adding a fixed m.

Define an overinclusive core envelope recursively by

\[
 K_{j+1}= B_j(K_j)+B^{(j+1)}_{\rho_{j+1}},
 \qquad
 \rho_{j+1}=c_L(R_{j+1}+m+1),                 \tag{CGD.1}
\]

where plus means the union of all blocks within the specified sup-norm distance. This operation includes the complete CA stencils. It is deterministic, additive under unions, and does not use an inverse dilation or distribute an erosion over unions.

For a birth defect at physical point x, suppose its initial core lies in a box of radius r_k h_k about x. The level-(j+1) cover of a box of radius r_j h_j lies in a box about the same physical x of radius at most (r_j/L+c_d)h_{j+1}. Absorb c_d in rho. Consequently

\[
 r_{j+1}\le L^{-1}r_j+c_L(R_{j+1}+m+1),       \tag{CGD.2}
\]

and after N blockings

\[
 r_{k+N}\le L^{-N}r_k+
 c_L\sum_{i=1}^{N}L^{-(N-i)}(R_{k+i}+m+1).
                                                       \tag{CGD.3}
\]

This follows by induction and is valid for arbitrary positive radii, without a monotonicity assumption. The sum is taken in final units: a buffer created i steps after birth is reduced by L^{N-i} in the final description.

For n birth occurrences, run this construction about each birth point and take the union. Because cover and dilation commute with unions, induction gives the same envelope for a merged family. Coincident occurrences may be counted more than once for an upper bound. Their latent copies are not identified. Thus

\[
 |K_{k+N}|\le C_L\sum_{a=1}^{n}(1+r^{(a)}_{k+N})^4.
                                                       \tag{CGD.4}
\]

For separated cores this is a volume bound only. Their connecting tree is not free. The actual old analytic connectors and any new connector tags must remain in the complete carrier; they supply the connections used in its weight.

## 3. The source radius bound makes the final core size uniform in age

CMP119, printed p.255, (2.6), gives for j<ell in the admitted weak trajectory

\[
 \frac{g_\ell}{\sqrt{1+\beta' g_\ell^2(\ell-j)}}
       \le g_j\le(1+\beta_0)g_\ell .             \tag{CGD.5}
\]

The same page, (2.5), chooses R_j as the least power of L above a fixed logarithmic power x_j^r, where x_j=log(g_j^{-2}). Keep a fixed weak ceiling, so x_j>=x_*>1. Then

\[
 \frac{R_j}{R_\ell}
 \le C\,[1+\log(1+\ell-j)]^r,\qquad j\le\ell.
                                                       \tag{CGD.6}
\]

Indeed, the lower coupling bound gives
x_j<=x_ell+log(1+beta' g_ell squared times (ell-j)); rounding to a power of L costs at most L. Division by x_ell>=x_* yields (CGD.6). No monotonicity of the rounded R_j is used. The upper coupling bound also gives R_ell<=C R_j for j<=ell.

Since the series

\[
 \sum_{q\ge0}L^{-q}[1+\log(1+q)]^r
\]

converges, (CGD.3), (CGD.6), and the birth bound r_k<=C R_k imply

\[
 \boxed{r_{k+N}\le C_L R_{k+N},\qquad
        |K_{k+N}|\le C_L n R_{k+N}^4
                         \le C'_L n R_k^4.}       \tag{CGD.7}
\]

All constants are independent of N and total volume, while depending on the fixed source parameters and weak-coupling ceiling. This is a geometric deduction along trajectories satisfying (CGD.5), not a proof of an all-depth analytic admission theorem.

In particular a single birth reserve exp(-c n P_k squared), with P_k squared/R_k to the fourth tending to infinity, can pay the **final** full core volume at a fixed positive carrier rate, uniformly in its age. Newly introduced reference buffers do not force a final radius proportional to N R_k. The previous buffers contract when expressed on the later lattice.

## 4. What telescopes and what does not

### 4.1 Final carrier weights

For a fixed tagged lineage with declared complete carriers Y_j, its change of carrier weight is exactly

\[
 \prod_{j=k}^{k+N-1}
       \frac{w_{j+1}(Y_{j+1})}{w_j(Y_j)}
       =\frac{w_{k+N}(Y_{k+N})}{w_k(Y_k)}.       \tag{CGD.8}
\]

Therefore a proof that retains the signed change of weight need not charge exp(C R_j to the fourth) afresh just to reweight the same old core at every step. Equation (CGD.7) bounds its final volume contribution. The actual connecting carriers still have to be estimated; neither (CGD.7) nor (CGD.8) discards them.

This identity concerns weights attached to a fixed lineage. It does not turn bounds for different sums, different coefficient registries, or different normalized integral maps into a telescoping identity.

### 4.2 Repeated absolute integral bounds

Iterating the displayed two-step bound CA.23/CA.24 without improvement produces a factor of the form

\[
 \exp\!\left\{\sum_{j=k}^{k+N-1}
     [C_a|S_j|+\eta_j r_j^{\rm latent}+\ell_j^{\rm other}]
       \right\}.                               \tag{CGD.9}
\]

These are amplitude losses, not ratios of spatial weights. There is no algebraic cancellation in (CGD.9) supplied by (CGD.8). A constant-radius envelope satisfying r_{j+1}=r_j/L+cR has r_j comparable to R for every sufficiently large j. Assigning a cost C times its volume at every step then gives a cost proportional to N R to the fourth, despite its bounded final footprint. This is a counterexample to the proposed *deduction from the geometric recurrence*, not a counterexample to the exact Yang--Mills integral.

The displayed two-step constants are upper bounds, not lower bounds on the true losses. A promising refinement is to retain the actual small frame displacement a_j instead of replacing it by a fixed ceiling. Young's inequality then gives a frame cost proportional to a_j squared times |S_j|/zeta_j and a Gaussian tilt zeta_j. CA.10 has an exponentially small omitted-buffer displacement. An all-depth proof could choose and sum these losses, or compare one full joint certificate. Neither summability of all such terms nor cancellation of the complete determinant/covariance costs follows from geometry alone.

## 5. Anchor counting is a separate all-depth issue

Let x range over birth-level blocks. A final block b can lie in the contracted, enlarged envelope K_{k+N}(x) only if x lies within a physical distance C R_{k+N} h_{k+N} of b. The number of such possible birth blocks is at most

\[
 C_L L^{4N}(1+R_{k+N})^4.                       \tag{CGD.10}
\]

The factor L^{4N} is a scale-density factor, not a shape entropy at the final scale. It is already present when no growing buffer is attached: a final block contains L^{4N} birth blocks. Paying the final R-sized halo once does not remove it.

A direct bookkeeping example proves the limitation. Put one tagged constant activity epsilon at each birth block and assign it to that block. A normalized conditional integral leaves the constant unchanged. After coarsening, the descendants of the L^{4N} birth tags inside a given final block contribute L^{4N} epsilon to its anchored absolute sum. Distinct tags may not cancel in that sum. This example has no coordinate-map or hard-boundary complication; it shows that no age-independent anchored transport bound can be deduced from positive normalization and shrinking carriers alone.

For a density, such a constant contribution can be extracted into the vacuum normalization. That is an additional, exact extraction step. A nonconstant action needs the corresponding scaling/extraction argument: a four-dimensional marginal density must carry the appropriate L^{-4N} local scaling gain before summing its possible birth positions, and irrelevant remainders need further decay or another summable mechanism. The two-step TD theorem does not establish this all-depth gain for every inherited nonsmooth density coefficient.

In particular, the available factor exp(-c P_k squared) cannot simply be declared to pay L^{4N} at arbitrary age. Along the weak-coupling relation (CGD.5), log(g_k^{-2}) can grow only logarithmically with the age at a fixed later coupling, while 4N log L is linear. The present rare-factor estimate by itself supplies no uniform domination. This is a statement about the available ledger, not a lower bound on an actual old Yang--Mills coefficient.

## 6. A precise remaining induction premise

The geometric part of a possible all-depth induction is now explicit: retain the full current raw core inputs and constraint stencils, use union enlargement, and use (CGD.1)–(CGD.7). No old latent rank or analytic response tail is erased.

The following analytic/depth input is still needed for an old birth lineage:

1. A common admissible real/complex constrained frame and exact component registry at every later level, preserving the original positive law and all local real domains. Fixed-depth Cauchy and gauge constants may not silently acquire an exponential dependence on age.
2. A joint old-certificate bound uniform in the current real variables, with a complete accounting of accumulated relative covariance, determinant, interaction, and current losses. Either their logarithmic costs are summable within a fixed part of the birth reserve, or an exact normalized joint construction avoids their repetition. Iterating CA.24 with fresh fixed losses is insufficient.
3. Vacuum/marginal extraction and a scaling or summability estimate compensating the birth-to-current anchor factor. One sufficient schematic bound for the non-extracted part is a local transport gain L^{-4N} times a summable age factor, with true connecting carriers and the actual source normalization retained. The appropriate statement for the extracted terms has to keep their running coefficients explicitly.
4. Uniform current and source-order control for these operations. A common coefficient family must retain every physical input footprint and the same normalized denominator; neither the geometric radius bound nor a value estimate proves that control.

These are distinct from the already resolved final core-volume question. The result of this note is positive on geometry: repeated physical blocking does permit a fixed final enlargement cost per birth. It does not make repeated integral losses or the anchored density of old births automatically summable.

References: Annex Y, M.1–M.2; CMP119 printed p.255, (2.5)–(2.6); CA.7–CA.13 and CA.22–CA.25; TD Sections 2–5. The two-step source inputs are those of the BA, CA and TD analysis.
