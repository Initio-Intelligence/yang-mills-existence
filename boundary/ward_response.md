# Wilson-subtracted primitive response and interpolation

**Composed-response hypothesis (CR).** Each complete boundary conclusion below assumes the displayed native-chart and spatial response estimates for the actual iterated reconstruction, with the prescribed earlier innovations and raw variables fixed, uniformly over the admitted histories. A sufficient estimate for the latent contribution is (A.8) in [Conditional-law estimates and the continuum application](../continuum/conditional_to_continuum.md), refined for the anchored exterior derivative in PG.18–PG.20. The two endpoint bounds concern the identical Wilson-subtracted primitive, its actual cutoff and its independently extended current. A direct minimizing-field derivative alone does not establish this hypothesis. The application to every required original Wilson history remains open. Complete boundary estimates and their C06/C08 applications in this chapter are conditional on CR and the other displayed source, AF, domain and support assumptions. Exact density identities and abstract inequalities retain their individually stated hypotheses.

In the projective density formulation, a sufficient comparison is
\[
 \sup_{\zeta,x,a}\left|
 \log\frac{W_\zeta(x,a)W_0(x,a_*)}
               {W_0(x,a)W_\zeta(x,a_*)}
 \right|\le\delta_r<\pi/2,
\]
on the stipulated chart with the required uniform rates and actual fixed support. The composed ordinary response is the unresolved input in its derivation. The exact partial-gauge transport and the surviving fixed-exterior derivative are given in the chapter [Gauge covariance of partial integrals and exterior scores](../continuum/partial_gauge_transport.md), equations PG.2–PG.6 and the subsequent anchored-score criterion.

## Assumptions and scope

This note does **not** infer OR.19 by replacing the evaluation grade by the forcing grade. The replacement is not justified by the cited Ward estimate. It isolates a useful way to avoid that replacement: apply the Ward estimate only at the two actual stopped configurations, obtain a second estimate on their **same difference** by ordinary primitive analyticity, and interpolate the two estimates. The analytic interpolation used for the second estimate need not satisfy a Ward estimate.

The elementary finite-difference and interpolation statements below are proved. The application uses the retained C01/C02/PF source hypotheses: the literal ordinary source families, their strong external core, and the actual normalized reconstruction rows. Section 2.2 makes the common-margin argument quantitative; Section 3.3 constructs the spatial row after interpolation; Section 6.2 gives the recent-boundary estimate actually used in the final repair. Section 6.1 is an optional marginal-response route and is not a premise of that repair. These statements concern the original pre-integration bank. They do not use a post-integration C bound. The final source-scoped conclusion is in Section 8; this note does not certify every other C-05 interface.

The normalization, final stopped mass and positive local cumulant estimates are not reconsidered here.

## 1. Exact source object and scales

Fix a history H, including its geometrical domains, cutoff profiles, birth labels, stopping branch, and the earlier raw tuple x. Let a and a_* be two actual tuples on the support of the stopped operation. The geometric grade n of a root z is a property of H. Changing a while keeping H fixed does not rerun the history selectors or change n. If an implementation compares different geometry labels, that comparison requires its own decomposition; it is not covered by declaring those labels equal.

Write b for the birth of an inherited E bank, n for the actual evaluation grade of z, and j for the grade of a forcing leaf from the stopped integration. The disputed range is

\[
 b\le n<j,\qquad a_0=n-b,\qquad c_0=j-n.
 \tag{ST.1}
\]

The same rootwise bank, before a change of minimizing representation, is

\[
 \mathcal R_{b,z}^{H}(U)
 =E^{(b)}(\Lambda_b,U,z)-E^{(b)}(\Lambda_b,1,z)
   -\beta_b A(h_z\phi_b,U).
 \tag{ST.2}
\]

Here E^{(b)}(Λ_b,U,z) includes its sum over localization domains X. The coefficient β_b is the coefficient extracted from this birth-b bank, and φ_b and h_z are the actual fixed birth cutoff and partition function. None depends on the endpoint a versus a_*. The relevant difference is

\[
 \Delta\mathcal R_{b,z}
 =\mathcal R_{b,z}^{H}(U^{a})-
   \mathcal R_{b,z}^{H}(U^{a_*}).
 \tag{ST.3}
\]

The elementary cancellation of the vacuum value in (ST.3) does not remove a Wilson term, an archived mass, or any variable-dependent factor.

For an interior root, h_z φ_b=h_z. CMP119, (3.49)–(3.64), obtains the Euclidean invariant quadratic expression **after the necessary sum over X**, identifies its coefficient with the original β_b, and (3.65)–(3.67) cancels that expression against the same Wilson functional. Thus the source statement concerns (ST.2), not an arbitrary assignment of a fraction of β_b to each primitive X.

With λ=5−θ, 0<θ<1, the endpoint Ward bound for an ancient interior root whose n-patch is separated from the fixed birth cutoff has the form

\[
 |\mathcal R_{b,z}^{H}(U^\sigma)|
 \le C E_0\,\ell_r^{D_W}(1+a_0)^{q_W}
              L^{-\lambda a_0},\qquad \sigma\in\{a,a_*\}.
 \tag{ST.4}
\]

Consequently,

\[
 |\Delta\mathcal R_{b,z}|
 \le 2C E_0\,\ell_r^{D_W}(1+a_0)^{q_W}
              L^{-\lambda a_0}.
 \tag{ST.5}
\]

The degree-preserving radius decomposition in E14.36–E14.37 is needed in (ST.4). It retains coefficient order p with its own inverse radius α_b^{-p}, and at least p physical field factors. Its use in (ST.4) changes the harmless polynomial and logarithmic factors, not the geometric exponent n−b. For recent interior roots whose n-patch crosses the old cutoff, (ST.4)–(ST.5) must include the additional tensor-tail term of (ST.30) below; being in Λ_b^0 alone does not remove that issue.

**Source limit.** CMP119, p.276, expressly replaces the homogeneous scale by the actual layer scale. Its (3.56) and (3.67) therefore supply n−b, not j−b. At roots outside the interior set Λ_b^0, (ST.4) is not obtained simply by citing (3.67); the leftover cutoff/boundary terms must be retained and estimated in their actual boundary sector.

## 2. A direct primitive finite-difference lemma

The following lemma requires no Ward identity and no analyticity in an old raw coordinate.

### Lemma 2.1: common native chart

Let f be holomorphic on a complex Banach chart containing, for every t∈[0,1], the ball of radius ρ>0 around ξ(t). Assume

\[
 |f|\le A\quad\hbox{on those balls},\qquad
 \xi:[0,1]\to\mathcal B\text{ is piecewise }C^1.
\]

Then

\[
 |f(\xi(1))-f(\xi(0))|
 \le {A\over\rho}\int_0^1\|\dot\xi(t)\|\,dt.
 \tag{ST.6}
\]

If the native norm already divides each coordinate by its analytic radius, the right side is C A times the integral of that normalized norm, with C determined by the fixed chart margin.

**Proof.** For a unit vector v, the function w↦f(ξ(t)+wv) is analytic on |w|<ρ. Its first derivative at zero is bounded by A/ρ by Cauchy's formula. Apply the resulting operator-norm estimate to \(\dot\xi(t)\), and integrate. No sum over individual fine coordinates occurs. ∎

For a primitive E_b(X,z), set A=C E_0 exp[−κ d_b(X)] and use its own native analytic chart. Applying Lemma 2.1 to this **original primitive** is legitimate without first replacing it by a nearby local minimizing representative. Accordingly, there are no unmarked nearby-replacement errors in this branch of the proof.

### What the path is, and is not

The useful path is in the actual **native determining data**, with H and x fixed. For a local input comparison V^1,V^0 in the source chart, use the branch of

\[
 V(t)=\exp\bigl(t\log(V^1(V^0)^{-1})\bigr)V^0
 \tag{ST.7}
\]

inside the common native domain, and compose the literal source maps. All unaffected determining data stay fixed. For several forcing leaves one may interpolate their native inputs together and differentiate the composition by the chain rule. The physical differences, rather than the normalized raw variables, are the small quantities in (ST.7).

The source facts required to admit (ST.7) are:

1. The physical j-fluctuation appearing in LFR I (1.60) is \(g_j C B_j-h\widetilde D(g_j C B_j)\), with the corresponding normalized A_j variable carrying the same physical g_j. Its admitted physical size is C g_j P_j. The nonlinear correction is quadratic on the same fixed analytic margin.
2. CMP102, Proposition 9, extends the actual minimizing map analytically in its small native determining data and in its regular external field. Equation (190) bounds its potential, gradient/Hölder and second-order output rows, with the actual source measure. It is not only a potential-value estimate.
3. LFR I (1.64)–(1.69) uses the true prepared-layer radii and provides the successive-insertion domain conditions. Earlier layers keep their own radii; the exceptional amplification is in the fixed top band.
4. The ordinary ++ admission must retain a fixed native margin for these compositions. A bound only at the two endpoints, with no shared native margin, would not imply (ST.6).

The path is an analytic tool, not a new integration over a larger real support. No selector is differentiated, no raw cutoff is smoothed, and no conditional density is assumed analytic in every raw coordinate. Fixed old raw variables are parameters throughout. For the gauge-invariant ordinary E bank one can choose the output gauge needed by its native chart: differentiating a simultaneous gauge change of its native arguments does not alter the scalar. This is not an instruction to rotate the fixed old raw tuple in the integration.

### 2.2 Quantitative margin from the retained strong-core hypotheses

There is a useful distinction between the external/map profile and the primitive ordinary profile. With fixed exponents chosen before the coupling ceiling, write

\[
 \gamma_n=g_n\ell_n^{q+Q},\qquad
 \alpha_n=g_n\ell_n^{q+Q+D_{\rm prep}+2}.
 \tag{ST.7a}
\]

The auxiliary γ-profile is the common external/map profile. The α-profile is the once-selected primitive ordinary analytic profile. This selection concerns the independently constructed ordinary source family; it does not enlarge an unknown completed-relative family. In the retained C02/PF strong-core inclusion, the actual composed output jets at a prepared layer n are at most \(C\ell_r^{D_{\rm prep}}\gamma_n\). Since n≤r and the AF logarithms satisfy \(\ell_n\ge\ell_r-C\), their ratio to α_n is \(O(\ell_r^{-2})\). The fixed coefficient in the external core is chosen after the source localization constants. Lowering the common coupling ceiling then leaves, for example, one quarter of the primitive radius unused, uniformly in n, r and the history.

For the additional comparison path of the two stopped tuples, use (ST.8) before dividing by the primitive radius. At each fixed output point, sum the source row in its actual source measure before taking the output supremum. This gives

\[
 {\|D_j\Phi_n\|_{n,\rm strong}\over\alpha_n}
 \le C_Q\ell_r^{D_0+p_0-q-Q-D_{\rm prep}-2}
       (1+j-n)^v e^{-\gamma_0(j-n)},\qquad j>n.
 \tag{ST.7b}
\]

The fixed exponent D_prep is chosen to include the actual top-band/composition loss D_0. Choose the already fixed q larger than p_0, and reserve γ_0>log 2 with a strict surplus to absorb the polynomial. The common coupling ceiling can then make the right side at most (β/8)2^{-(j−n)}. Summing over later grades consumes at most β/8, and the finitely many same-grade endpoint conventions are paid by the fixed remaining margin. This is the dyadic reserve appearing in the LFR I prepared-space conditions. The estimate uses source-field rows only and makes no use of OR.19 or of a stopped-density bound.

The current slot is essential in this assertion. The exact CMP109 (3.13) extension is

\[
 E^{(b)}\!\left(X,e^{i\xi_b A}U,
       \tau_b J+\Delta_U^{\xi_b}A-P_1A+F_1(U,A)\right),
 \tag{ST.7c}
\]

where \(\tau_b=(L^{b-1}\eta)^3\) in the printed convention, and F_1 is the local nonlinear expression specified there. Equation (190) controls the potential, first-difference/Hölder, projection and Laplace rows required by this substitution. The current's unit conversion is of physical order three (E14.45). Consequently (ST.7b) is a joint native/background/current statement. It would be false to deduce it from a potential-only estimate.

The retained C02 smaller-basic-domain theorem supplies the reconstruction tests once these strong input bounds and margins hold. No claim is made that every point of an entire modified prefix space is an unrestricted strong ball. Only the literal composed family from the genuine external strong core is used. Likewise, the near Ward expression is the source-defined analytic composition: CMP109 (4.3) evaluates its coefficient identities at U=1,J=0 and then substitutes the actual regular A, which may depend analytically on the independent external J. The argument does not use uniqueness of an extension from the physical-current graph.

In the disputed range n<j, LFR I (1.14)–(1.17) retains the already prepared determining component at n when changing a later j-component. Thus the two endpoint maps and the path in this argument have one fixed lower geometry. If a geometry change occurs at the current strip, its true layer is j or later and belongs to the c_0=0/coarse-containment branch, not to an alleged change of n midway through (ST.7b).

## 3. The crude response of an original E primitive

Let s be one actual forcing cell of grade j, and let y be an output point of a primitive. Denote its original native grade by i and its prepared grade by m. The relevant interior relation is i≤m. For a birth-b primitive, its inner convention caps the original grade by b.

The complete smooth row of the physical source map takes the schematic, dimensionally explicit form

\[
 h_m^p|D_s\operatorname{out}_p(y)|
 \le C\,g_jP_j\,\mathcal P_r\,
           K_H(y,s),\qquad p=1,2,3,
 \tag{ST.8}
\]

where K_H is an actual normalized positive absolute reconstruction row and \(\mathcal P_r\) is a fixed logarithmic/top-band factor. The current and second-order rows are included. The factor h_s^{-4} in a kernel representation is paired with the source's own h_s^4 measure; it does not produce another count of fine coordinates.

In the primitive's native normalization, (ST.8) becomes

\[
 \alpha_i^{-1}(h_i/h_m)^p g_jP_j\,
           C\mathcal P_r K_H(y,s).
 \tag{ST.9}
\]

The physical g_j in (ST.9) is essential. With α_i=g_i times its prescribed logarithmic profile, the AF comparison gives

\[
 {g_j\over g_i}\le C(1+j-i)_+^{1/2}
\]

in the old-grade range; finitely many reversed-grade/top-band comparisons are carried by their actual source factors. Since p≥1 and i≤m, the exponential factor L^{-p(m−i)} absorbs every fixed polynomial in m−i. Thus (ST.9) is bounded by a fixed polynomial in the remaining grade distances and logarithms, times K_H(y,s). There is **no naked inverse power of g_r**.

For a literal birth-b/native-b output with m≥b, the simpler expression is

\[
 C\mathcal P_r\,{g_jP_j\over\alpha_b}
             L^{-p(m-b)}K_H(y,s).
 \tag{ST.10}
\]

Keeping L^{-p(m−b)} can sharpen the final interpolation. Dropping that favorable factor gives a safe response estimate with no required Ward gain in b→n.

Apply (ST.6) on the original primitive chart. After the positive decomposition into actual forcing leaves, its response is bounded by

\[
 C E_0\mathcal P_r e^{-\kappa d_b(X)}
 \sum_{j,s}\sup_{y\in X^+}
       \bigl[\text{the normalized row in (ST.9)}\bigr].
 \tag{ST.11}
\]

The supremum is a Banach directional norm. Replacing it by an unnormalized sum over all microscopic y would add an unsupported fine-lattice density.

### 3.1 Connecting the root to the responding output

The output grade m need not equal the root's evaluation grade n. The factor exp[−Γ(j−n)] cannot be read off from exp[−Γ(j−m)] alone.

The complete carrier X contains the root z and the responding output y, up to the fixed dependency collar. Retain a reserved share of its **full physical carrier length**. For m>n, a connection from a true grade-n root to grade m crosses the intervening actual prepared collars. For m≤n, the source response already crosses at least j−n grades. The resulting geometric inequality has the form

\[
 \kappa_1 d_b(X)+\delta_1 d_H(y,s)
 \ge \Gamma(j-n)_+-C_\Gamma.
 \tag{ST.12}
\]

This uses a real root of grade n. A birth label b attached to a high-grade point is not a grade-b port. Nor may X be replaced by an uncharged enlarged region or by a quotient connector that crosses current high-grade holes for free.

There are two quantitatively valid ways to arrange a prescribed finite Γ:

* Work with the actual birth-b full carrier and prove its annular lower bound. When b≤n, crossings up to a genuinely larger grade m cost at least geometric birth-b length; a reserved full-carrier exponential can then pay any prescribed finite Γ(m−n), at a constant depending on Γ.
* If only a linear-in-grade connector lower bound is being used, choose the carrier decay parameter κ large enough for the allocated share to pay the required Γ, as well as the source block parameter M large enough that the reserved propagator share does so.

A naive metric triangle with unspecified constants does not show that Γ is arbitrarily large. LFR I (1.47) makes the source contribution quantitative: its grade exponent is proportional to the reserved source decay rate times M/M_1. The source expressly chooses M large, independently of the scale. The corresponding carrier reserve must still be checked separately.

### 3.2 Spatial reserve

The shares used in (ST.12) do not consume all the carrier and source decay. Sum the remaining carrier kernels and actual native reconstruction rows in their original measures. For a fixed interpolation parameter η∈(0,1), it is convenient to state the resulting positive envelope as

\[
 B_{b,z;j,s}
 \le C E_0\ell_r^{D_B}(1+a_0+c_0)^{q_B}
          e^{-\Gamma c_0}\,w_j(z,s)^{1/(1-\eta)}.
 \tag{ST.13}
\]

Here w_j is a final spatial kernel whose normalized physical-root sum obeys

\[
 \sup_s\sum_{\substack{z\text{ a birth-}b\text{ root}\\
                         z\text{ of grade }n}}
       w_j(z,s)
 \le C L^{4(j-b)},\qquad b\le n\le j.
 \tag{ST.14}
\]

One way of recording (ST.14) is to partition into proper j-cells: there are at most C L^{4(j−b)} birth-b roots per cell, and the residual coarse-cell kernel has an absolute row sum bounded independently of the history. The row is the original positive reconstruction/full-carrier convolution. It must not be obtained by renaming an integrated C estimate or by forgetting native cell measures.

Equation (ST.13) deliberately reserves more spatial decay than the final row needs. If a crude estimate were recorded merely with w_j, interpolation would produce w_j^{1−η}; summability of w_j does not by itself imply summability of that power. The source parameters and reserved rates must be chosen for the weakened final rate before the coupling ceiling is chosen.

The input required for (ST.13)–(ST.14) is a common fixed-geometry primitive path with the complete row (ST.8), the genuine-root connector inequality (ST.12), and the absolute native row sum for the remaining rates. The Cauchy argument itself does not manufacture any of these geometric facts.

### 3.3 A constructive residual row, including the power loss

Here is a way to record the spatial estimate without assuming that the original row survives taking a fractional power. After reserving the age factors in (ST.12), let

\[
 V_{b,n;j}(z,s)=\sum_{X\ni z}e^{-\kappa_2d_b(X)}
       \sup_{y\in X^+}e^{-\delta_2d_H(y,s)}.
 \tag{ST.14a}
\]

All finite source stencil and normalized-cell constants are included; the physical g_jP_j and the radius polynomial have already been extracted. The native current and higher smooth rows have the same positive kernel after that extraction. Put ε=1−η. Subadditivity gives

\[
 V_{b,n;j}(z,s)^\epsilon
 \le\sum_{X\ni z}e^{-\epsilon\kappa_2d_b(X)}
       \sup_{y\in X^+}e^{-\epsilon\delta_2d_H(y,s)}.
 \tag{ST.14b}
\]

On the proper birth-b block cover of X^+, bound the supremum by the sum over its finitely many block representatives. The comparison within each block has a fixed source constant: ordinary E carriers remain in Ω_b, so no arbitrarily finer prepared grading is introduced there. This is a sum over the carrier's b-blocks, not over microscopic coordinates. Its block multiplicity and fixed collars are absorbed by a further reserved carrier share.

Interchange the positive carrier and root sums. The absolute full-tree sum over carriers containing a fixed representative is bounded at the rate ε κ_2, after its fixed volume moment is paid. The remaining normalized reconstruction sum at rate ε δ_2 is exactly the native absolute row sum of CMP96 Lemma 2.1/(2.59)–(2.61), with the source's proper cell measures. At source grade j, converting birth-b roots to proper j-cell volume contributes L^{4(j−b)}. In a coarser output layer m>j, the additional factor L^{4(m−j)} is paid by the remaining true-layer annular response. This is the usual source grade-volume sum; it is bounded when the remaining exponent exceeds 4 log L. It is not a factor L^{4N_r} assigned to the enclosing component.

Hence the right side of (ST.14b) has root sum at most C L^{4(j−b)}. Taking w_j=V_{b,n;j}^ε yields (ST.13)–(ST.14) in the required form. The source assumptions permit κ to be chosen arbitrarily large with the other fixed parameters chosen in order (CMP119, discussion after (2.31)); LFR I (1.47) permits the block parameter M to pay the required finite reduced source rate. Choose these fixed parameters to satisfy both the age reserve and this ε-rate volume sum, and only then choose the strong-core coefficient and the common coupling ceiling. This makes the row construction independent of the total number of scales.

This construction applies to the literal full-carrier E representation. Replacing d_b(X) by a quotient length through a current high-grade component would remove the just-used representative/root convolution and requires a separate argument.

## 4. The matching Wilson term in the crude branch

In this branch only, estimate the E difference and the Wilson difference separately. This does not change which scalar is estimated in (ST.3).

Let F_p^σ be the small traceless logarithm of a plaquette at either endpoint. For matrices F_0,F_1 in a fixed small complex ball,

\[
 |\operatorname{tr}(e^{F_1}-e^{F_0})|
 \le C(\|F_1\|+\|F_0\|)\,\|F_1-F_0\|.
 \tag{ST.15}
\]

**Proof.** Put F_t=(1−t)F_0+tF_1. Under the trace, the derivative of exp F_t is tr(exp F_t(F_1−F_0)). The trace of F_1−F_0 is zero. Subtract the identity from exp F_t, use its fixed-ball Lipschitz bound, and integrate. ∎

For a b-cell evaluated in an n-regular field, the endpoint plaquette bound and the physical response bound are, with microscopic spacing ε,

\[
 \|F_p^\sigma\|\le C\alpha_n(\varepsilon/h_n)^2,
 \qquad
 \|\Delta_sF_p\|\le C g_jP_j\mathcal P_r
        (\varepsilon/h_n)^2\,\mathcal K(z,s).
 \tag{ST.16}
\]

There are C(h_b/ε)^4 plaquettes in a proper b-cell. Since h_z φ_b is fixed and bounded, (ST.15)–(ST.16) give

\[
 |\Delta_s A(h_z\phi_b,U)|
 \le C\alpha_n g_jP_j\mathcal P_r
             L^{-4(n-b)}\,\mathcal K(z,s).
 \tag{ST.17}
\]

The source coefficient is

\[
 |\beta_b|\le C E_0\alpha_b^{-2}.
 \tag{ST.18}
\]

Thus the coupling factor in the crude Wilson response is

\[
 C E_0\,{\alpha_n\over\alpha_b}
              {g_jP_j\over\alpha_b}\,
              \mathcal P_r L^{-4(n-b)}.
 \tag{ST.19}
\]

Both factors of the coefficient radius are paired with physical fields. AF bounds the two ratios by fixed polynomials/logarithms. There is no substitution β_b=O(1), and no loss of an inverse coupling. The actual response kernel and the same full-root/spatial reserves give a contribution of the form (ST.13); the factor L^{-4(n−b)} may be discarded for the conservative interpolation.

The locality of the Wilson plaquette simplifies its response connector. If its fixed support meets a lower actual layer, use that actual layer's radius and response row; do not assign the root's n-radius to all nearby plaquettes without the source collar comparison. A support that reaches the birth boundary is among the boundary checks listed below.

## 5. Interpolation of two bounds on the same difference

Assume (ST.5) at the two actual endpoints and the crude estimate obtained by adding the original E and the matching Wilson responses,

\[
 |\Delta\mathcal R_{b,z}|
 \le C E_0\ell_r^{D_B}
 \sum_{j,s}(1+n-b+(j-n)_+)^{q_B}
     e^{-\Gamma(j-n)_+}\,
       w_j(z,s)^{1/(1-\eta)}.
 \tag{ST.20}
\]

For the range b≤n≤j, interpolation gives

\[
 |\Delta\mathcal R_{b,z}|
 \le C E_0\ell_r^D
 \sum_{j,s}(1+a_0+c_0)^q
 L^{-\eta\lambda a_0}
 e^{-(1-\eta)\Gamma c_0}
 w_j(z,s).
 \tag{ST.21}
\]

**Proof.** For nonnegative A,B and 0<η<1, min(A,B)≤A^ηB^{1−η}. Apply this to (ST.5) and (ST.20). Then use

\[
 \Bigl(\sum_\nu u_\nu\Bigr)^{1-\eta}
       \le\sum_\nu u_\nu^{1-\eta},\qquad u_\nu\ge0.
 \tag{ST.22}
\]

This produces exactly the spatial power displayed in (ST.21). Both estimates refer to (ST.3), so no cancellation from one function has been multiplied by a response estimate for a different function. ∎

### Why the order of these operations matters

An individual marked integral

\[
 \int_0^1D\mathcal R(\Phi_t)[D_s\Phi_t]dt
\]

is not automatically bounded by twice the endpoint Ward value. Do not apply (ST.5) separately to every marked cell s, or to an artificial hybrid tuple obtained by replacing only some old raw coordinates. The safe proof applies the Ward bound once to the complete actual endpoint difference, applies the crude response estimate to that same complete difference, and only then distributes the positive majorant over forcing leaves by (ST.22). Thus the auxiliary path and its intermediate configurations require ordinary primitive analyticity, but no unproved Ward estimate on hybrid configurations.

### Root and age sums

For fixed j,s, apply (ST.14). The two-age numerical series is

\[
 \sum_{a_0,c_0\ge0}(1+a_0+c_0)^q
 L^{-[\eta\lambda-4]a_0}
 \exp\{-[(1-\eta)\Gamma-4\log L]c_0\}.
 \tag{ST.23}
\]

It converges if

\[
 \eta\lambda>4,\qquad (1-\eta)\Gamma>4\log L.
 \tag{ST.24}
\]

Such an η exists precisely when

\[
 \Gamma>{4\lambda\log L\over\lambda-4}.
 \tag{ST.25}
\]

For example, choose θ=1/2, hence λ=9/2, and η=17/18. Then ηλ=17/4, leaving a birth-age reserve 1/4, and the second inequality requires Γ>72 log L. This is an illustrative conservative choice, not an optimization. Taking η just above 4/λ lowers the required Γ toward the threshold 36 log L for this λ. Any polynomial in a_0+c_0 is absorbed by the strict exponential reserves in (ST.24).

After the sums, each actual source cell contributes \(C E_0\ell_r^D\). Summing over s gives the true D_j(P), and summing j over the finite stopped prefix gives the ordinary E contribution in the form required by OR.19. The recent-birth branch b>j is the separate native-cell estimate OR.17–OR.18; it is not silently included in (ST.23). The case n>j has no missing j−n age and uses the stronger endpoint gain n−b≥j−b with the appropriate actual coarse-containment row.

The conclusion of this interpolation calculation is conditional on the explicit source-to-row checks in Sections 2–3 and the endpoint/boundary check in Section 1. It is not a proof that those checks hold merely because the numerical series converges.

## 6. An alternative: differentiate the Ward remainder itself

There is also precise source support for a direct derivative approach, but it must use the correct chart.

CMP109, (3.30), replaces the actual H_k(B′) fluctuation by an **arbitrary regular complex field A**. Equation (3.31) imposes its potential, gradient and first-Hölder bounds. Equations (3.34)–(3.36), and Lemma 4/(3.53), give an analytic chart for the resulting old minimizing pullback. The paragraph after (3.54) explicitly obtains the extra small factor O(1)α_2^{-1}ε_1 by differentiating with respect to the localized fluctuation parameter. CMP119, immediately after (3.66), says to obtain the fluctuation-integrand expressions by differentiating the already Wilson-subtracted irrelevant terms with respect to t_□.

Therefore the following direct lemma is valid. Suppose a **single** fixed birth-b, root-z Wilson-subtracted function F_{b,z}^{(n)}(A) represents the two stopped evaluations, is analytic for \|A−A_t\|_{n,reg}<cα_n along a path, and satisfies the Ward bound C E_0 poly(n−b)L^{-λ(n−b)} throughout that chart. If

\[
 \|\dot A_t\|_{n,reg}
 \le C g_jP_j\operatorname{poly}(j-n)
                 e^{-\Gamma(j-n)}\mathcal K(z,s),
\]

then Cauchy and integration give

\[
 |\Delta F_{b,z}^{(n)}|
 \le C E_0\operatorname{poly}(j-b)\ell_r^D
 L^{-\lambda(n-b)}e^{-\Gamma(j-n)}\mathcal K(z,s).
 \tag{ST.26}
\]

The ratio g_jP_j/α_n has been retained before the AF comparison; it does not cost an inverse coupling. This lemma is proved by exactly (ST.6), now with the Ward value majorant in place of A.

For application, however, the same localized minimizing pullback and the same Wilson functional must represent both endpoints, and the errors from the replacements in CMP109 (3.18)–(3.25) must retain their marked response. An arbitrary perturbation of the reconstructed fine field is not automatically such a chart. The endpoint-plus-crude method of Sections 2–5 avoids this stronger matching obligation, because its crude branch works on the original E bank and its Ward branch uses only the two actual endpoints.

### 6.1 Optional route: a marginal response for the recent boundary bank

**Not used in the final repair.** The argument in this subsection identifies a source-supported alternative, but the final route below avoids needing its marked near-chart assertion. In particular (ST.28) is not a premise of the conclusion. The per-X marginal value statement and its exact source are useful independently; a future use of its differentiated form must retain the specified near-map chart and far errors.

There is a distinct issue when b is a recent preparation birth, h≤b≤r. Preparation can enlarge the regular region through the old Λ_b boundary. A root of evaluation grade n may then be close to that old boundary even when n−b is large. For such a root, the full-torus Euclidean reduction leading to the single coefficient β_b is not available with the desired age gain. The endpoint Ward estimate (ST.4) must not be asserted there.

Only a **dimension-four marginal response** is needed for this finite recent-birth bank. There is a precise source anchor. In CMP119 p.283, immediately after (3.67), the proof of (2.44) for R terms stops at (3.49), before the full-torus summation and Euclidean tensor reduction. The root z may be any point of a single localized X. Its leading tensor is quadratic in curvature and is therefore bounded by L^{-4(n−b)}; the other terms are more irrelevant. Replacing the R coefficient bound g_b^{10} by the ordinary E coefficient bound E_0 gives the same marginal estimate for each E_b(X). No Wilson subtraction and no extension of the restricted X sum to the whole lattice are involved in this step.

For completeness, carry out that calculation on the same arbitrary-regular-A chart (CMP109 (3.30)–(3.36), Lemma 4), on a proper n-patch containing the near carrier. In the radius decomposition, the leading curvature tensor has coefficient order two and two curvature factors; the cubic/quartic algebra and fifth-order tail retain their own coefficient orders. With all regular input jets on the α_n chart, the resulting complete near function has

\[
 |E_{b,X}^{\rm near}-E_{b,X}^{\rm near}(0)|
 \le C E_0\operatorname{poly}(n-b)\ell_r^{D_M}
             L^{-4(n-b)}e^{-\kappa' d_b(X)}.
 \tag{ST.27}
\]

Unlike the Euclidean cancellation, this marginal statement holds for the individual gauge-invariant X term. The source's (3.49) and the R proof just cited are exactly the needed identities. The fixed external J is admitted through the source's actual regular-A substitution and the strong margin of Section 2.2; no criticality identity is asserted for an arbitrary independent current.

If the fixed-n near function and its two-endpoint marked comparison are verified in this same chart with the profile margin of (ST.7a), Cauchy applied to (ST.27), together with the actual n-normalized j-response, gives

\[
 |\Delta_jE_{b,X}^{\rm near}|
 \le C E_0\operatorname{poly}(j-b)\ell_r^{D'_M}
 L^{-4(n-b)}e^{-\Gamma(j-n)}
             \mathcal W_{b,n;j}(X,z,s).
 \tag{ST.28}
\]

The normalization is g_jP_j/α_n before the AF comparison. The common output strong margin, rather than analyticity in an old raw variable, justifies this Cauchy derivative. The marked source path and remaining full carrier give the same positive spatial row as in Section 3.3, now without fractional-power loss unless a far remainder is being interpolated.

One must also keep the exact nearby-replacement errors from CMP109 (3.18)–(3.25). Their endpoint value bound has an arbitrarily high b→n power, by the actual separation exponential in (3.21)/(3.17). For their crude response, apply ordinary primitive Cauchy to the difference of the two specified maps: both have the physical g_j forcing, the actual n-patch data, and the same strong primitive admission. Thus each error has the analogue of (ST.20). Interpolate those two bounds as in Section 5, choosing any fixed λ_far>4 and sufficient remaining Γ. There is no need to assume that the nearby replacement error is zero, or to multiply its endpoint value bound by an unrelated derivative estimate.

After the four-dimensional birth-root count, (ST.28) leaves

\[
 \operatorname{poly}(a_0+c_0)\ell_r^{D'_M}
       e^{-[\Gamma-4\log L]c_0}.
 \tag{ST.29}
\]

The a_0 sum is over at most N_r+O(1) recent grades. It costs a fixed polynomial in N_r, not L^{4N_r}. The matching recent Wilson term already has the same dimension-four response by (ST.17)–(ST.19), with its unchanged cutoff retained. It can therefore be bounded separately in this finite recent sector. The old, unbounded birth-age sector still uses the genuine same-bank cancellation and the two-age interpolation of Section 5.

This optional recent-sector argument requires verification of the source's literal per-X near function, its shared arbitrary-A chart and its specified far errors. It does not assert a dimension-four bound for an arbitrary analytic function or for an independently chosen extension of a physical graph. The final repair below avoids this extra marked-near-function verification entirely.

### 6.2 Actual route: retain the recent tensor tail and use N_r≤C_N R_r

The final repair does not need (ST.28). Keep the error in extending the restricted X sum to the whole-lattice tensor in CMP119 (3.56)–(3.57). For a root z∈Λ_b^0, an omitted carrier crosses the original MR_b interior buffer. The corresponding Taylor coefficients are evaluated at the flat pair (1,0), where the full homogeneous coefficient catalog is defined. A reserved carrier share therefore bounds the omitted coefficient sum by its Cauchy radius factors times exp(−κ_tail R_b). It is unnecessary to evaluate a missing activity at a field outside its original domain.

The degree-preserving coefficient/field decomposition then gives, for h≤b≤n≤j,

\[
 |\Delta_j\mathcal R_{b,z}|
 \le C E_0\ell_r^{D_A}(1+n-b)^{s_A}
   \left[L^{-\lambda(n-b)}+e^{-\kappa_{\rm tail}R_b}\right].
 \tag{ST.30}
\]

The same β_b remains in both endpoints. The new term is the residual restricted tensor, not a different projection or counterterm. The second bound (ST.20) still bounds the **entire original difference**. Thus use

\[
 \min(A_1+A_2,B)
 \le (A_1^\eta+A_2^\eta)B^{1-\eta}.
 \tag{ST.31}
\]

The A_1 contribution is (ST.23). The A_2 contribution, after the full root count, is bounded by

\[
 CE_0\ell_r^D |S_j|(1+N_r)^{s+1}
 e^{4N_r\log L-\eta\kappa_{\rm tail}c_RR_r}
 \sum_{c_0\ge0}(1+c_0)^s
      e^{-[(1-\eta)\Gamma-4\log L]c_0},
 \tag{ST.32}
\]

where the recent-window AF comparison gives R_b≥c_RR_r with a fixed positive c_R. The preparation-depth condition is genuinely available: LFR II, p.361, immediately after (1.20), explicitly assumes N≤R_k. The waiting-depth statement on p.384, before (1.80), uses N=R_j. With harmless endpoint/rounding conventions, write N_r≤C_NR_r. This is a condition of the retained source construction, not a newly shortened window.

Choose the remaining, already-loss-adjusted coefficient-tail rate so that

\[
 \eta\kappa_{\rm tail}c_R>4C_N\log L+\epsilon,
 \qquad\epsilon>0.
 \tag{ST.33}
\]

Then (ST.32) is at most a fixed polynomial times exp(−εR_r). CMP119 after (2.31) expressly permits the ordinary carrier exponent κ to be chosen arbitrarily large when the other fixed parameters are chosen properly. Allocate its tail, connector and entropy shares first; choose the associated block/localizer constants and the weak-coupling ceiling afterwards. No history-dependent parameter or new logarithmic power proportional to the final Q is introduced.

For ancient births b<h, LFR I (1.11) and (1.15)–(1.17) preserve Ω_{b+1}⊂Λ_b. True-layer admissibility then separates the root n-patch from Λ_b^c by c h_n, outside a fixed adjacent-layer exception. An omitted carrier has birth-b length at least cL^{n−b}, so its tail is already absorbed by the irrelevant value bound (ST.4). This proves why the ancient and recent endpoint formulas differ.

The remaining Wilson cutoff bank, outside the root aggregate, is separate. Its recent part uses the retained L^{-4(n−b)} in (ST.19) and the finite N_r count. Its ancient part uses the unchanged low-grade boundary and L^{n−b}≤CR_b; consequently the indicator of the allowed evaluation ages is at most CR_bL^{-(n−b)}. The AF comparison bounds R_b by a fixed polynomial in \(\ell_r\) and \(j-b\). The resulting age sum is a polynomial times

\[
 \sum_{a_0,c_0\ge0}L^{-a_0}
     e^{-[\Gamma-4\log L]c_0}<\infty.
 \tag{ST.34}
\]

This is the literal cutoff remainder. It has not been assigned an artificial per-X Wilson cancellation.

## 7. Exact primary-source decomposition

The following references are to the papers themselves, not to a general statement of closure.

| Primary source | Exact result used | What it does not by itself prove |
|---|---|---|
| Bałaban, *Convergent Renormalization Expansions for Lattice Gauge Theories*, CMP **119** (1988), pp.275–276 | Mixed-layer cover and the instruction to replace the homogeneous scale by the actual evaluation layer; extra fluctuation/propagator decay is retained for boundary contributions. | It does not identify n with j or state OR.19. |
| Same, (3.49)–(3.56), pp.280–281 | Ward reduction and the irrelevant exponent 5−θ at the evaluation scale. | It is not an arbitrary per-X Wilson cancellation. |
| Same, (3.57)–(3.64), pp.281–283 | Sum over localization domains, Euclidean reduction, and identification of the coefficient with the original β_b. | It does not permit choosing a new β at each stopped endpoint. |
| Same, (3.65)–(3.67), p.283 | Same Wilson subtraction, differentiation of the irrelevant terms for fluctuation integrands, and the rootwise subtracted endpoint estimate on Λ_b^0. | It does not cover a cutoff-boundary root without its boundary decomposition. |
| Bałaban, *Generation of Effective Actions …*, CMP **109** (1987), (3.6)–(3.17), pp.271–273 | Actual nonlinear minimizing-map derivative, all required native norms, and Cauchy with an explicit fixed native margin. | A potential-only response is insufficient for the independent current slot. |
| Same, (3.18)–(3.25), pp.273–275 | Exact nearby pullback transformations and explicit far/localization errors. | Errors cannot be discarded when comparing two pullbacks. |
| Same, (3.30)–(3.36), pp.276–277, and Lemma 4/(3.53)–(3.54), p.280 | Arbitrary regular-A analytic domain; quantified derivative gain from differentiating the fluctuation parameter. | An arbitrary fine output perturbation has to be placed in this actual chart before using the Ward derivative bound. |
| Bałaban, *Variational Problem and Background Fields for Lattice Gauge Theories*, CMP **102** (1985), (179)–(190), pp.306–309; Proposition 9, p.309 | Analytic native determining-data map and the potential, gradient/Hölder and second-order absolute derivative rows with source factor (L^{j′}ε)^{-4}. | It does not justify discarding that source measure or a required output norm. |
| Bałaban, *Large Field Renormalization I*, (1.44)–(1.47), p.186 | Actual weighted-distance response and the grade decay proportional to M/M_1, with scale-independent choice of M. | It does not supply an uncharged carrier connector from a high-grade output to a lower-grade root. |
| Same, (1.60), pp.188–189, and (1.64)–(1.69), pp.190–191 | Physical g_j fluctuation; literal inherited bank; layer-dependent native radii and top-band restrictions. | These inputs must still be composed with one fixed history and a fixed native margin. |
| Bałaban, *Propagators and Renormalization Transformations II*, CMP **96** (1984), Lemma 2.1 and (2.59)–(2.61) | Absolute normalized exponential row sums on the source geometry. | A row after an unspecified loss of exponential rate is not automatically a valid row; the reduced rate must meet the source hypothesis. |
