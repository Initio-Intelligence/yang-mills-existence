# Alternative age summation and parameter selection

**Composed-response hypothesis (CR).** Each complete boundary conclusion below assumes the displayed native-chart and spatial response estimates for the actual iterated reconstruction, with the prescribed earlier innovations and raw variables fixed, uniformly over the admitted histories. A sufficient estimate for the latent contribution is (A.8) in [Conditional-law estimates and the continuum application](../continuum/conditional_to_continuum.md), refined for the anchored exterior derivative in PG.18–PG.20. The two endpoint bounds concern the identical Wilson-subtracted primitive, its actual cutoff and its independently extended current. A direct minimizing-field derivative alone does not establish this hypothesis. The application to every required original Wilson history remains open. Complete boundary estimates and their C06/C08 applications in this chapter are conditional on CR and the other displayed source, AF, domain and support assumptions. Exact density identities and abstract inequalities retain their individually stated hypotheses.

In the projective density formulation, a sufficient comparison is
\[
 \sup_{\zeta,x,a}\left|
 \log\frac{W_\zeta(x,a)W_0(x,a_*)}
               {W_0(x,a)W_\zeta(x,a_*)}
 \right|\le\delta_r<\pi/2,
\]
on the stipulated chart with the required uniform rates and actual fixed support. The composed ordinary response is the unresolved input in its derivation. The exact partial-gauge transport and the surviving fixed-exterior derivative are given in the chapter [Gauge covariance of partial integrals and exterior scores](../continuum/partial_gauge_transport.md), equations PG.2–PG.6 and the subsequent anchored-score criterion.

## 0. Result and its exact status

There is an alternative to proving that the Ward gain and the response gain
multiply in a derivative of the renormalized expression.  Bound the **same
complete scalar difference twice**, then interpolate the two bounds:

1. the two endpoint Ward bounds supply decay in the actual evaluation age
   \(a=n-b\);
2. a crude derivative of the primitive E terms and their own Wilson term
   supplies decay in the response age \(c=j-n\).

The resulting numerical summation is proved in Section 3.  It supplies the
required old-birth part of OR.19 if the explicitly stated endpoint and pointed
response estimates hold for the actual stopped family.  In particular, no
identity is asserted on a Ward chart inferred from its values on a smaller
physical-current graph.

The useful quantitative point is that even a crude response with **no remaining
birth-age gain** suffices.  For a Ward exponent \(\lambda=5-\theta>4\), the
required response rate is

\[
 \Gamma>\frac{4\lambda}{\lambda-4}\log L.                 \tag{AR.1}
\]

This is stronger than the boundary-induction argument's displayed
\(\Gamma>4\log L+\varepsilon_0\).  It must be imposed and verified before
using this route.  Source geometric parameters can be chosen larger, but that
fact does not itself establish that the response estimate applies to every
stopped configuration in the submitted history class.

**Final status:** the interpolation and radius calculations below are
proved.  Section 10 records the later parameter analysis, resolution of the
recent truncated-tensor error, and independent verification of the
integrated OR.19 repair in its stipulated AF, C01, C02, PF and actual
native-response scope.  Section 8 keeps the source dependencies explicit.
This note does not certify the remaining C-05 lemmas or declare the
Yang–Mills existence problem solved.

## 1. The scalar to which both estimates must apply

Fix a literal history branch and all variables held fixed by its conditional
law.  In particular fix the old E bank, its birth domains \(\Lambda_b\), its
cutoffs \(\phi_b\), and its coefficients \(\beta_b\).  For an interior root
\(z\in\Lambda_b^0\), set

\[
 \begin{split}
 R_{b,z}(W)={}&
 \sum_{\substack{X\ni z\\X\subset\Lambda_b}}
       \bigl[E^{(b)}(X,W,z)-E^{(b)}(X,1,z)\bigr]
       -\beta_b A(h_z,W),\\
 \Delta R_{b,z}={}&R_{b,z}(W^1)-R_{b,z}(W^0).
 \end{split}                                                   \tag{AR.2}
\]

Here \(W^0,W^1\) are the actual stopped endpoint configurations, including
the native pair/preparation used by the original source formula.  Equation
(AR.2) is a root aggregate, not one primitive localization-domain term.

CMP119 (2.26)–(2.29) gives the root and localization representations.  The
Euclidean covariance needed to identify the marginal tensor is available
after summing the localization domains.  CMP119 (3.56)–(3.64) performs that
sum and identifies the coefficient with the original \(\beta_b\).  The
subtraction in (3.65)–(3.67) then cancels it.  Assigning an independently
chosen Wilson coefficient to each \(X\) would not reproduce this argument.

### The cutoff remainder must be retained

The exact source Wilson partition is

\[
 A(\phi_b,W)=\sum_z A(h_z\phi_b,W).
\]

For \(z\in\Lambda_b^0\), the source proves \(h_z\phi_b=h_z\).  Consequently
the complete birth bank decomposes as

\[
 \begin{split}
 E^{(b)}(\Lambda_b,W)-E^{(b)}(\Lambda_b,1)
       -\beta_b A(\phi_b,W)
 ={}&\sum_{z\in\Lambda_b^0}R_{b,z}(W)+C_b^{\rm cut}(W),\\
 C_b^{\rm cut}(W)={}&-\beta_b
        \sum_{z\notin\Lambda_b^0} A(h_z\phi_b,W).
 \end{split}                                                   \tag{AR.3}
\]

This is an exact decomposition.  The endpoint estimate (3.67) does not
directly estimate \(C_b^{\rm cut}\).  If that term has already been assigned
to the heterogeneous Wilson or boundary decomposition, its assignment and bound
must be retained there.  It cannot disappear when (AR.2) is introduced.

CMP119 (2.1) gives the nesting
\(\Omega_b\supset\Lambda_b\supset\Omega_{b+1}\), but the paper permits
\(\Lambda_b=\Omega_b\) after an R operation.  Nesting alone therefore does
not prove that every root of \(C_b^{\rm cut}\) has bounded \(n-b\).
Section 9 below supplies a stronger argument using the surviving ancient
determining geometry.  It does not use nesting alone.

## 2. Two bounds, with different sources

Write

\[
 a=n-b\ge0,\qquad c=j-n\ge0,
 \qquad \lambda=5-\theta\in(4,5).
\]

The discussion concerns the unresolved stratum \(b\le n\le j\).  Births
\(b>j\) and other recent strata keep their existing finite-window treatment.

For adjacent prefix steps, LFR I (1.15)–(1.17) retains the already prepared
lower determining strata while replacing the current layer.  Thus, in
the problematic stratum \(n<j\), the two adjacent stopped configurations
have the same literal lower geometric layer \(n\); the field on that
layer changes nonlocally.  On a fixed history branch the domain and
selector records are also held fixed when the free current tuple varies.
This source fact is the appropriate reason for using a common \(n\) in
(AR.4).  An arbitrary pair of differently labeled histories would require
a separate common-cover argument and is not silently included.

### 2.1 Endpoint estimate

For the same \(R_{b,z}\) and the two actual endpoint values, require

\[
 |R_{b,z}(W^\epsilon)|
 \le C_W(Q)E_0(1+a)^u L^{-\lambda a},
 \qquad \epsilon=0,1.                                    \tag{AR.4}
\]

It immediately follows that

\[
 |\Delta R_{b,z}|
 \le 2C_W(Q)E_0(1+a)^u L^{-\lambda a}.                    \tag{AR.5}
\]

The actual scale in CMP119 (3.67) is \(n\), not \(j\).  Equation (AR.5)
uses precisely that scale.  Its origin is the endpoint Ward cancellation,
including the far-domain error in (3.48), followed by the degree-preserving
running-radius comparison in E14.36–E14.38.

For OR.19, (AR.4) has to hold at the actual complex ordinary \(++\)
endpoints.  A version only on the real physical-current graph is
insufficient.  This requirement does **not** ask that the Ward estimate hold
along the interpolation used to prove the next bound.

### 2.2 Crude response estimate

Let \(S_j\) be the actual stage-\(j\) integration/forcing cells, counted in
their native measure, and \(D_j=|S_j|\).  Suppose the actual source response
gives

\[
 |\Delta R_{b,z}|
 \le C_R(Q)E_0\ell_r^d(1+a+c)^v L^{-p a}
                  \sum_{s\in S_j} K_{j,n}(z,s),             \tag{AR.6}
\]

with \(0\le p<4\).  The robust choice in this note is \(p=0\).

The kernel must retain its positive spatial and annular majorant.  For the
fixed interpolation parameter \(0<\eta<1\) used below, require

\[
 \sum_{z\in\mathcal Z_{b,n}}
          K_{j,n}(z,s)^{1-\eta}
 \le C_\eta
       L^{4(a+c)}e^{-(1-\eta)\Gamma c},                    \tag{AR.7}
\]

where \(\mathcal Z_{b,n}\) denotes birth-\(b\) roots whose actual evaluation
layer is \(n\).  The factor \(L^{4(a+c)}\) is the four-dimensional root
density at a fixed stage-\(j\) forcing cell.  It is retained until the
annular exponential and Ward decay have been combined.

An ordinary unweighted row-sum bound for \(K\) does not imply (AR.7).
For example, \(N\) entries equal to \(N^{-1}\) have row sum one but their
\((1-\eta)\)-powers sum to \(N^\eta\).  The source's pointwise spatial
decay, with a positive reserve left after all allocations, is necessary.

The kernel is normalized **after** the source input density \(h_j^{-4}\)
has been paired with its native input measure \(h_j^4\).  Taking a
fractional power of an unpaired density would change the measure and
invalidate the calculation.

## 3. The summation theorem

### Proposition

Assume (AR.4), (AR.6), and (AR.7), uniformly in the fixed raw variables and
in the relevant ordinary \(++\) endpoints.  Suppose there is an
\(\eta\in(0,1)\) such that

\[
 \eta\lambda+(1-\eta)p>4,
 \qquad (1-\eta)\Gamma>4\log L.                            \tag{AR.8}
\]

Then

\[
 \sum_{b\le n\le j}\sum_{z\in\mathcal Z_{b,n}}
                |\Delta R_{b,z}|
 \le C(Q)E_0\ell_r^{d'} D_j,                               \tag{AR.9}
\]

where the constant and the exponent are independent of the total old
depth.  If \(u,v,d\) are independent of the profile-enlargement exponent
\(Q\), so is \(d'\).  Polynomial factors in a fixed prefix-window length
can be included in \(\ell_r^{d'}\).

### Proof

For nonnegative \(A,B_s\),

\[
 \min\left(A,\sum_s B_s\right)
 \le\sum_s\min(A,B_s)
 \le A^\eta\sum_s B_s^{1-\eta}.                             \tag{AR.10}
\]

The first inequality holds because either some \(B_s\ge A\), in which case
the right side is at least \(A\), or all \(B_s<A\), in which case the
right side is \(\sum_sB_s\).  The second inequality is the elementary
\(\min(A,B)\le A^\eta B^{1-\eta}\).

Apply (AR.10) to (AR.5) and (AR.6).  Both are bounds for exactly the
same \(\Delta R_{b,z}\).  In particular it is irrelevant that the first
bound was proved by cancellation and the second by estimating the
primitive and Wilson derivatives separately.  The common factor \(E_0\)
remains linear.  After summing the roots using (AR.7), the result is
bounded by

\[
 \begin{split}
 C(Q)E_0\ell_r^{d(1-\eta)}D_j
 \sum_{a,c\ge0}&(1+a)^{\eta u}
              (1+a+c)^{(1-\eta)v}\\
 &\times L^{-[\eta\lambda+(1-\eta)p-4]a}
       e^{-[(1-\eta)\Gamma-4\log L]c}.
 \end{split}                                                \tag{AR.11}
\]

Both exponential rates are positive by (AR.8).  Since
\(1+a+c\le(1+a)(1+c)\), the double series is bounded by a product of two
convergent polynomial-times-geometric series.  This proves (AR.9).

The sum over forcing cells is exactly \(D_j\); it has not been replaced by
\(D_j^{1-\eta}\), by a fine enclosing volume, or by a separate choice of raw
tuple for each root.  All inequalities hold pointwise for each common raw
tuple before taking the allowed exterior supremum.  \(\square\)

### 3.1 The parameter condition

For \(p<4\), an \(\eta\) satisfying (AR.8) exists precisely when

\[
 \frac{4-p}{\lambda-p}
       <1-\frac{4\log L}{\Gamma},
 \quad\text{equivalently}\quad
 \Gamma>\frac{4(\lambda-p)}{\lambda-4}\log L.                \tag{AR.12}
\]

Thus \(p=0\) gives (AR.1).  If a fully justified \(p=1\) response is
available for the complete root aggregate, the threshold improves to
\(4(\lambda-1)\log L/(\lambda-4)\).

A convenient nonoptimal explicit choice for the robust \(p=0\) route is

\[
 \theta=\tfrac12,\quad \lambda=\tfrac92,\quad
 \eta=\tfrac{11}{12},\quad \Gamma\ge60\log L.
\]

Then the two remaining decay factors in (AR.11) are at most

\[
 L^{-a/8}L^{-c}.                                            \tag{AR.13}
\]

All the permitted fixed polynomial factors are summable against (AR.13).

### 3.2 Why the stronger response rate is a real requirement

The two separate numerical bounds alone do not prove convergence at the
weaker rate used in RL.8.  Consider nonnegative numbers

\[
 d_{a,c}=\min\{L^{-\lambda a},L^{-pa}e^{-\Gamma c}\}.
\]

Along integers \(c\) within one of
\((\lambda-p)a\log L/\Gamma\), the two alternatives are comparable.
The density-weighted term \(L^{4(a+c)}d_{a,c}\) has exponential rate in
\(a\) proportional to

\[
 4-\lambda+\frac{4(\lambda-p)\log L}{\Gamma}.
\]

If (AR.12) fails, these terms need not even tend to zero.  This is a sharp
obstruction for this pair of numerical bounds.  It is not a counterexample
to the Wilson theory; it explains exactly why strengthening the retained
annular rate is needed for this alternative argument.

## 4. Crude primitive E response: keep the physical coupling

This section gives the radius calculation behind (AR.6).  Its source
interface is the actual pointed native response, not a Gaussian
replacement.

Take the ordinary profile

\[
 \alpha_b^{++}=c_b g_b\ell_b^{q+Q},
\]

with the fixed source constants and the smaller analytic margin included
in \(c_b\).  Suppose a primitive satisfies its original source estimate

\[
 \sup_{\mathcal U_b^{++}(X)}|E^{(b)}(X,W,z)|
       \le E_0e^{-\kappa d_b(X)}.                           \tag{AR.14}
\]

On a fixed smaller native chart, a Banach directional Cauchy estimate
gives

\[
 |DE^{(b)}(X,W,z)[v]|
 \le CE_0(\alpha_b^{++})^{-1}
                  e^{-\kappa d_b(X)}\|v\|_{{\rm nat},b;X}.
                                                               \tag{AR.15}
\]

All native components needed by the source must be included in this norm:
the field, its appropriate derivatives, and the independent/reconstructed
current.  No sum of absolute fine-coordinate derivatives is introduced.

For a response attachment at actual layer \(t\ge b\), the source row has
the physical size

\[
 Cg_jP_j (h_b/h_t)^m K^{\rm map}_{t,j},\qquad m\ge1,          \tag{AR.16}
\]

in the corresponding native component.  This is the scale conversion in
RL.25, with its actual force \(g_jB_j\) or \(g_jA_j\), and with the
input measure already paired.  Because \(t\ge b\), discarding
\((h_b/h_t)^m\le1\) is valid.  The two-sided AF comparison gives

\[
 \frac{g_jP_j}{\alpha_b^{++}}
 \le C_Q(1+j-b)^{1/2}P_j
 \le C_Q(1+a+c)^{1/2}\ell_r^{d_P}.                          \tag{AR.17}
\]

The nonnegative logarithmic power in the denominator was only discarded;
it was never turned into a positive power proportional to \(Q\).  There
is no bare inverse coupling in (AR.17).

Integrating (AR.15) along the actual source's admitted interpolation gives
a crude bound for the difference of this primitive.  The source
interpolation must hold its prescribed old raw data fixed and retain the
literal determining-data conversion.  No identity between a minimizing
map for one determining geometry and a dilation of another map is needed
or asserted.  Their difference has not been set to zero: the actual map
and its actual response row are used throughout.

Summing the primitive domains with their retained carrier decay, and
joining the carrier from the root \(z\) to its actual attachment, yields
the E part of (AR.6), subject to the geometric kernel statement in Section
6.  The use of the \(p=0\) version is deliberate: if \(t<n\), the
factor \(L^{-(t-b)}\) need not be bounded by \(L^{-(n-b)}\).

## 5. The matching Wilson derivative has no inverse-coupling loss

The coefficient bound is the original projection estimate

\[
 |\beta_b|\le CE_0(\alpha_b^{++})^{-2}.                      \tag{AR.18}
\]

It would be incorrect to combine this with a unit-size derivative of the
Wilson action.  The trace has a quadratic zero and must retain its two
physical factors.

Let \(F\) be the small logarithm of a plaquette.  For the holomorphic
Wilson trace function \(w\), semisimplicity/tracelessness gives
\(w(0)=Dw(0)=0\).  On a fixed small matrix ball,

\[
 |w(F_1)-w(F_0)|
 \le C(\|F_0\|+\|F_1\|)\|F_1-F_0\|.                       \tag{AR.19}
\]

Indeed, integrate \(Dw(F_0+u(F_1-F_0))[F_1-F_0]\) over
\(u\in[0,1]\); boundedness of the second derivative and \(Dw(0)=0\)
give (AR.19).  The estimate does not require commuting matrices.

On a layer-\(t\) patch the regularity and actual smooth response bounds
read

\[
 \|F_\epsilon\|\le C\alpha_t^{++}(\eta_0/h_t)^2,
 \qquad
 \|F_1-F_0\|\le Cg_jP_j(\eta_0/h_t)^2K^{\rm map}_{t,j},
                                                               \tag{AR.20}
\]

where \(\eta_0\) is the fine mesh, not the interpolation exponent.  The
source gauge comparison must be the same one in both norms.  A birth-\(b\)
Wilson root has \(C(h_b/\eta_0)^4\) plaquettes, up to its fixed cutoff and
stencil constants.  Thus (AR.18)–(AR.20) imply

\[
 |\beta_b\,\Delta A(h_z\phi_b)|
 \le CE_0\,
       \frac{\alpha_t^{++}}{\alpha_b^{++}}
       \frac{g_jP_j}{\alpha_b^{++}}
       L^{-4(t-b)}K^{\rm map}_{t,j}.                        \tag{AR.21}
\]

The fine volume has canceled exactly against the four curvature mesh
powers.  In particular (AR.21) contains neither a remaining fine volume
nor a naked \(g_b^{-2}\).

The same-profile AF comparison gives

\[
 \frac{\alpha_t^{++}}{\alpha_b^{++}}
       \le C_Q(1+t-b)^{1/2}.
\]

Since
\(\sup_{u\ge0}(1+u)^{1/2}L^{-4u}<\infty\), combining this with
(AR.17) gives the required crude \(p=0\) response uniformly in the
attachment layer.  On a patch with \(t=n\), (AR.21) retains the stronger
marginal factor \(L^{-4a}\), but the proof does not rely on assigning that
factor to every attachment in a mixed-layer carrier.

This calculation uses the same \(\beta_b\) as (AR.2).  The coefficient is
fixed while the present prefix variables vary.  If a proposed comparison
also changes the source selector, birth domain, or coefficient, it is not
the same scalar difference and must first be decomposed by the literal
history-incidence rule.

## 6. The response kernel and the larger geometric constant

### 6.1 Carrier and map path

In the crude E derivative, a primitive domain \(X\) contains the original
root \(z\) and the response attaches at some point of \(X\).  The retained
carrier tree joins the root to that point.  Concatenate it with the actual
source map path to the forcing cell \(s\).

If the attachment has layer \(t\le n\), the map path must pay the required
annuli above \(n\).  If \(t>n\), the carrier path and the source path
together must pay them.  The geometric statement needed is that these
are **actual prepared annuli**, with no unpaid shortcut inside a protected
footprint or an arbitrarily relabeled boundary collar.  This is the
same issue that the boundary-induction RL.8 path argument has to address.

After reserving independent shares for domain entropy, spatial summation,
and any other required connector, this gives a pointwise kernel of the
form used in (AR.7).  A scalar signed operator norm is not a substitute
for this positive pointed estimate.

The \((1-\eta)\)-power in (AR.7) spends a fixed additional share of the
remaining spatial exponent.  The carrier/localizer constants must be
chosen to leave that share summable.  This is a fixed parameter change,
not a scale-dependent loss.

### 6.2 What the primary papers permit

CMP119, printed p.245, fixes the variational block constant \(M_1\), then
sets \(M_2=L^2M_1\), and subsequently takes \(M\) sufficiently larger.
LFR I, printed p.186, (1.45)–(1.47), retains the scaled distance for a
localized determining-data perturbation.  Its annular lower bound gives
an exponent proportional to \(\delta(M/M_1)(j-i)\), and the text
explicitly chooses \(M\) large enough to dominate a prescribed finite
rate.  It states that these conditions are independent of all scale
indices.  The localization exponent \(\kappa\) also has a large-parameter
reserve in the source construction; see CMP119 p.260 after (2.31).

Accordingly, if the actual source/history path lemma yields

\[
 \Gamma\ge
 \min\{\text{reserved carrier crossing rate},
       \text{reserved }\delta M/M_1\text{ rate}\},
                                                               \tag{AR.22}
\]

both reserves can be required to exceed the finite threshold (AR.12).
Choosing \(M\) alone does not enlarge a carrier reserve that has already
been exhausted; the two allocations have to be recorded.

This is a permitted **initial choice of fixed parameters** for a theorem
whose admissible histories are defined after those parameters are
chosen.  It is not a proof for a previously fixed class with a smaller
value of \(M\), and it does not establish (AR.22) for boundary labels
which have not been related to the actual prepared determining geometry.

## 7. Recovery of the old-birth part of OR.19

Once the hypotheses in Section 3 are verified, summing (AR.9) over the
actual prefix stages gives

\[
 \sup_{++}|D^{E,\mathrm{interior\ old}}_{\rm ord}|
 \le C_QE_0\ell_r^{d'}\sum_{j=h}^{r-1}D_j(P).                \tag{AR.23}
\]

The finite stage/proper-layer multiplicities and the existing top-band
factor may equivalently be written in the boundary-induction argument's form

\[
 C_Q E_0 N_r^{s'}L_0^{cN_0}\sum_{j=h}^{r-1}D_j(P).
                                                               \tag{AR.24}
\]

Their logarithmic degree must remain independent of \(Q\), as in the
retained profile count.  The source cutoff remainder (AR.3), recent births,
and the other ordinary sectors are then added from their own established
decompositions.  If those decompositions and the Section 8 interfaces are verified,
(AR.24) is the required substitute for the invalid use of a direct
\(j-b\) Ward gain in OR.15.

This proof is entirely preintegration.  It neither changes the canonical
mass nor estimates an integrated C output in place of the integrand.
The already-repaired moving denominator and final mass argument are not
used as substitutes for (AR.23).

## 8. Source applicability decomposition and remaining checks

One part of the endpoint check deserves explicit attention.  The source
passes from the restricted \(X\)-sum to the whole-lattice marginal tensor;
the omitted domains must be far relative to the genuine evaluation patch.
For \(b<h\), the unchanged \(\Omega_{b+1}\subset\Lambda_b\) and the
graded separation protect deep prepared patches inside \(\Lambda_b\).
For a recent \(h\le b\le n<j\), preparation can change the intervening
domains.  One must keep the source boundary assignment or establish its
replacement estimate before applying the interior endpoint Ward bound.
Merely saying that there are at most \(N_r\) recent births would not
control a crude primitive E value together with an unpaid
\(L^{4(n-b)}\) root density.  The pure Wilson calculation in Section 9 is
different because it retains its marginal fourth-power scale factor.

| Item | What is established | What is still needed for the all-history claim |
|---|---|---|
| Rootwise own subtraction | CMP119 (2.26)–(2.29), (3.56)–(3.67) identify the aggregate and its own \(\beta_b\). | Verify that both stopped endpoints use this identical fixed aggregate, including literal cutoff and source selector. |
| Evaluation-age decay | CMP119 (3.67) gives \(L^{-(5-\theta)(n-b)}\) at a genuine layer \(n\). | Apply the source's complex/native preparation statement at both actual \(++\) endpoints, including independent currents; do not infer it from a physical-current identity alone. |
| Primitive response radius | (AR.15)–(AR.17) remove a potential inverse-coupling loss, using the physical \(g_j\). | The actual fixed-raw source path must remain in the admitted primitive chart with the source field, derivative, and current norms. |
| Wilson response radius | (AR.19)–(AR.21) prove the quadratic-zero calculation and cancellation of the fine measure. | Use the actual smooth field response and the same gauge comparison at the two endpoints. |
| Two different attachments | The robust \(p=0\) calculation does not pretend that every attachment is at layer \(n\). | Prove the concatenated carrier/map annular estimate for the actual stopped determining geometry and retain a positive fractional-power spatial row. |
| Stronger rate | (AR.12) is the exact sufficient threshold for the two-bound argument; the source permits larger fixed geometric/localization parameters. | Record their simultaneous choice, remaining shares, and the precise history class to which the resulting \(\Gamma\) applies. |
| Wilson cutoff remainder | (AR.3) keeps the exact residual term; Section 9 proves an ancient/recent summation using the surviving determining geometry. | Identify the actual stopped source domains with that geometry and retain the local smooth response row; nesting alone is insufficient. |
| Summation | (AR.9)–(AR.13) are proved with the complete four-dimensional root count visible. | No further summation lemma is needed once the preceding interfaces hold. |

The advantage of this route is specific: it does not require a Ward estimate
for the derivative of the subtracted term, or a common Ward-valid contour
joining the two endpoints.  It still requires the endpoint estimates and
the crude response to concern **the same source scalar**.  If either
endpoint cannot be placed in the source's native Ward domain, interpolation
cannot repair that failure.

**Remark.** Section 10 resolves the recent truncated-tensor
issue with the original source preparation-window relation.  It also
records the conclusion on the integrated repair.  The
table above distinguishes the ingredients rather than replacing that
conclusion.

## 9. Additional cutoff calculation: ancient and recent births

The following estimate concerns the age weights.  It gives a
way to estimate the exact residual in (AR.3) without assigning it an
unproved irrelevant Ward gain.

### 9.1 A surviving ancient exterior point bounds the possible layer

Let \(h=r-N_r\) be the lower endpoint of the current preparation window.
For an ancient birth \(b<h\), LFR I (1.11) leaves the domains at indices
\(i\le h\) unchanged.  Its intermediate determining sets (1.14)–(1.17)
also leave the lower determining strata untouched.  Thus
\(\Omega_{b+1}\) remains the same domain throughout the current prefix.

Take a label \(z\notin\Lambda_b^0\) with a nonzero cutoff contribution.
The partition label itself can lie just outside \(\Lambda_b\).  Choose
an actual support anchor \(z^\#\in\operatorname{supp}(h_z\phi_b)
\subset\Lambda_b\), within \(O(h_b)\) of \(z\), and grade this anchor.
This is a bounded-displacement, bounded-multiplicity change of root, so
it preserves the birth-cell count.  In particular its actual layer is at
least \(b\).  By the definition of \(\Lambda_b^0\), which removes one
layer of \(MR_b\)-cubes, there is a point \(y\notin\Lambda_b\) with

\[
 |z^\#-y|\le C M R_b h_b.                                  \tag{AR.25}
\]

Because \(\Omega_{b+1}\subset\Lambda_b\), this point is outside the
unchanged \(\Omega_{b+1}\).  Suppose that the actual prepared determining
geometry gives \(z^\#\) layer \(n\).  For \(n\ge b+2\), nestedness gives
\(y\notin\Omega'_{n-1}\) and \(z^\#\in\Omega'_n\).  The admissible-domain
separation in CMP102 p.277, (1), is

\[
 \operatorname{dist}((\Omega'_i)^c,\Omega'_{i+1})
     >R M_1h_i.
\]

Consequently

\[
 R M_1h_{n-1}\le |z^\#-y|\le C M R_bh_b,
 \qquad L^{n-b}\le C_*R_b.                                 \tag{AR.26}
\]

The cases \(n=b,b+1\) are included by enlarging the fixed constant.
No claim that the entire old boundary collar is itself a prepared annulus
was used.  Only a genuine surviving exterior point and the actual
admissible determining-set separation were used.

For a Wilson root the support of \(h_z\) has diameter \(O(h_b)\).  The same
separation shows that the native layers met by this fixed local stencil
are comparable to the root layer up to fixed grade changes; for a much
larger layer, its required separation from the lower-layer exterior would
exceed the stencil diameter.  Thus the layer-\(n\) curvature and response
version of (AR.20), with fixed constants, is legitimate on this local
stencil whenever the actual source smooth row is available there.

### 9.2 The missing birth sum is now summable

For this local Wilson stencil, retain the \(L^{-4a}\) in (AR.21), where
\(a=n-b\), and the response age \(c=j-n\).  The four-dimensional root
count cancels the \(L^{-4a}\) and leaves, apart from fixed polynomial
factors,

\[
 C_QE_0\ell_r^{d_W}
       e^{-[\Gamma_W-4\log L]c}
       \mathbf1_{\{L^a\le C_*R_b\}}.                       \tag{AR.27}
\]

Here only \(\Gamma_W>4\log L\) is needed.  The ancient-cutoff constraint
can be used without solving an implicit inequality for \(a\):

\[
 \mathbf1_{\{L^a\le C_*R_b\}}
       \le C_*R_b L^{-a}.                                 \tag{AR.28}
\]

The source profile has \(R_b\le C\ell_b^{\rho}\) for a fixed exponent
\(\rho\).  Two-sided AF gives, for \(b\le j\) in the present notation,

\[
 \ell_b\le C+\ell_j+\log(1+j-b)
          \le C+\ell_j+\log(1+a+c).
\]

For example this implies the sufficient polynomial estimate

\[
 R_b\le C\ell_r^{\rho}(1+a+c)^{\rho},                       \tag{AR.29}
\]

with a harmless adjustment for the fixed prefix-window comparison.
Substituting (AR.28)–(AR.29) in (AR.27) leaves

\[
 C_QE_0\ell_r^{d_W+\rho}
 \sum_{a,c\ge0}(1+a+c)^{v_W+\rho}
             L^{-a}e^{-[\Gamma_W-4\log L]c}<\infty.          \tag{AR.30}
\]

Thus the ancient cutoff residual is bounded per actual forcing cell by a
fixed logarithmic power.  This argument is independent of the Ward
interpolation in Section 3.

For recent births \(b\ge h\) with \(b\le n\le j\), one has
\(0\le a\le j-h\le N_r\).  The marginal Wilson gain
\(L^{-4a}\) cancels the birth-cell density, and the remaining finite
birth sum costs at most a fixed polynomial in \(N_r\).  Births \(b>j\)
retain the existing coarse-cell treatment of OR.17–OR.18.  There is no
reason to demand an irrelevant gain from the pure cutoff Wilson term.

### 9.3 Why the cutoff is the canonical current one

LFR II p.377 explicitly completes the new action by adding missing
localization-domain terms and subtracting them into the residual
interaction.  At pp.390–391, the completed action is stated to satisfy
the full CMP119 induction hypothesis.  Therefore, after each completed
earlier R operation, the bank to be used in (AR.3) is the canonical bank
on the current admitted \(\Lambda_b\) domains.  It is not a sum over a
second catalog of obsolete cutoff domains.

This matters when invoking (AR.25): the cutoff whose boundary is being
used must be the cutoff in the actual current bank.  Once that exact
source identification is made, the ancient/recent argument above removes
the proposed cutoff remainder as an independent summation obstruction.

## 10. Final analysis: the recent E boundary error and the original N profile

### 10.1 Do not shorten the preparation window

A suggested shortcut was to choose \(N_r\) proportional to \(\ell_r\),
so that an \(e^{-cR_b}\) error with \(R_b\gtrsim\ell_b^2\) would easily
pay \(L^{4N_r}\).  That shortcut is unnecessary and should not replace
the retained waiting rule.

The actual source and retained decomposition say more:

- LFR II p.361, immediately after (1.20), explicitly assumes
  \(N\le R_k\).
- LFR II p.384, immediately before (1.80), uses the waiting criterion
  \(N=R_j\) in the chronological induction.
- The retained main manuscript, R14.32–R14.36, keeps this choice and
  checks \(r/2<p_0-p_1-1\) for \(R_j\asymp\ell_j^r\).
- The retained *First Constrained Boundary Readout* explicitly uses
  \(N\le C R_k\), citing both source statements.

The other displayed restrictions are compatible: LFR I (1.94) gives a
fixed polynomial upper bound for \(N\), plus a fixed lower bound; LFR II
after (1.29) asks for a lower bound of order \(\log\ell_k\); and (1.47)
requires a fixed polynomial in \(\ell_k\) times \(L^{-N}\) to be small.
The retained \(N\asymp R\), with \(r\ge2\), satisfies these conditions
at a common sufficiently weak coupling ceiling.  The rare-history power
condition \(2p_0>r(d+2)\) is also retained.  There is no need to introduce
a different waiting profile.

For the present proof, retain the resulting relation

\[
 N_r\le C_N R_r                                             \tag{AR.31}
\]

with the fixed comparison constant allowed by the source conventions.

### 10.2 Keep the finite-domain tensor error at the endpoint

For recent \(h\le b\le n\le j\), the root \(z\) is in
\(\Lambda_b^0\), but the actual prepared layer need not lie deeply inside
the old cutoff.  In CMP119 (3.56)–(3.57), keep the difference between the
restricted coefficient sum and the full-lattice tensor.  Every omitted
carrier crosses the original \(MR_b\) buffer.  Summing its spatial
moments with a reserved share of the carrier exponential gives
\(e^{-\kappa_{\rm cut}R_b}\).

These coefficients are calculated at the flat primitive reference
\((1,0)\).  This step does not evaluate a missing primitive at an actual
field outside its admitted domain.  The coefficient-order and physical
field-degree decomposition bounds the remaining curvature factors by fixed age
polynomials, as in (AR.4).  Thus the endpoint estimate has the form

\[
 |\Delta R_{b,z}|
 \le C_QE_0\ell_r^{d_0}(1+a)^{s_0}
       \left[L^{-\lambda a}+e^{-\kappa_{\rm cut}R_b}\right]
       =A_1+A_2.                                          \tag{AR.32}
\]

The coefficient \(\beta_b\) remains the original source coefficient.
The second term is the retained truncated-tensor error, not a newly
chosen counterterm.

Use the original crude response bound for the **whole** difference.
There is no need for a separate response estimate for the error in
(AR.32), because

\[
 \min(A_1+A_2,B)
 \le (A_1^\eta+A_2^\eta)B^{1-\eta}.                        \tag{AR.33}
\]

The \(A_1\) contribution is Section 3.  For the \(A_2\) contribution,
the actual recent window has \(a\le N_r\), and uniform AF/profile
comparison gives \(R_b\ge c_RR_r\) with a fixed \(c_R>0\).
No monotonicity of the rounded radii is assumed.  For example, if
\(\ell_s^r\le R_s<L\ell_s^r\) and the common ceiling ensures
\(\ell_b\ge\ell_r/2\), one may take \(c_R=2^{-r}/L\).

After the complete root count, the extra contribution is at most

\[
 \begin{split}
 C_QE_0\ell_r^{d_1}D_j(1+N_r)^{s_1}
 &\exp\{4N_r\log L-\eta\kappa_{\rm cut}c_RR_r\}\\
 &\times\sum_{c\ge0}(1+c)^{s_1}
       e^{-[(1-\eta)\Gamma-4\log L]c}.
 \end{split}                                                \tag{AR.34}
\]

The \(c\)-series already converges by (AR.8).  In view of (AR.31), choose
the **remaining** carrier-tail rate so that

\[
 \eta\kappa_{\rm cut}c_R>4C_N\log L+\epsilon,
 \qquad \epsilon>0.                                       \tag{AR.35}
\]

Then (AR.34) is bounded by a fixed polynomial times
\(e^{-\epsilon R_r}\).  This closes the recent E cutoff summation using
the original waiting profile.

### 10.3 The larger tail rate is a permitted fixed source choice

There is no hidden requirement here to make \(\kappa\) large relative to
a simultaneously increasing \(\log L\).  CMP116 p.21, after (2.41),
explicitly chooses \(M\) sufficiently large that \(\delta_0M\ge\kappa\)
to obtain the ordinary activity bound (1.1.18).  This is consistent with
CMP119 p.245, where \(M_1\) is fixed, \(M_2=L^2M_1\) is chosen, and then
\(M\) is enlarged.  Thus one can first fix the finite rates required by
(AR.12) and (AR.35), reserve their separate spatial/entropy shares, and
then choose the larger fixed block parameters and common coupling
ceiling.  No parameter depends on the history depth.

The fixed analytic exponent \(Q\) affects constants and the final weak
coupling ceiling.  It does not change the finite coefficient orders, the
carrier-tail power requirement, or the degree of the running polynomial.
The retained R14.32–R14.36 compatibility check allows the larger finite
ordinary analytic profiles used for this purpose.

### 10.4 Conditional implication for ordinary oscillation

I read [Ordinary stopped-density oscillation on mixed scales](ordinary_oscillation.md) through (SR.24), including its actual
profile reserve, the original-primitive response, the root-to-attachment
geometry, the corrected recent error (SR.15a)–(SR.15d), and the final
coarser-output treatment in its Section 8.1.

That last case keeps the actual output layer \(n>j\): the birth-root
count is \(L^{4(n-b)}\) on the proper \(n\)-cell cover.  It is paired
with \(L^{-\eta\lambda(n-b)}\), leaving a summable
\(L^{-(\eta\lambda-4)(n-b)}\).  The recent truncated-tensor error is
still paid by (AR.35), since \(n-b\le N_r\) there.  Pure Wilson cutoff
terms retain their fourth-power factor and the ancient indicator bound.
This verifies the remaining stratum \(b\le j<n\) separately from
\(b\le n\le j\) and the existing coarse-birth case \(j<b\).  Weakening
the field regularity must never silently change the physical root mesh;
the final integrated version does not do so.

**conclusion: the displayed OR.19 bound follows under CR in the stated stipulated
AF, C01, C02, PF and actual native-response scope, with the explicit fixed
rate choices recorded in that repair.**  The repair does not need a new
estimate that multiplies the Ward cancellation and response for a
derivative of a renormalized term.  It instead uses two independently
available bounds on the same finite difference, retaining the literal
cutoff error and its measure cost.

This conclusion uses the predecessor theorems exactly in their declared
scope: actual stopped native cores and their complete smooth/current
response rows.  It is not a proof of those predecessor results for a
larger, unspecified family of histories or arbitrary independently
chosen continuations.  The stronger carrier and annular rates are fixed
source-parameter requirements, explicitly permitted by the construction,
not hypotheses equal to the desired stopped-density conclusion.

The age summation yields the ordinary estimate under CR and the stated root, radius and cutoff hypotheses.
