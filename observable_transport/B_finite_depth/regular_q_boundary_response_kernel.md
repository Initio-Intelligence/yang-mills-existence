# Ordinary boundary primitives in the exact regular Q kernel

This note addresses the regular one-step operation in M04. It does not replace its incoming transported scalar by a fresh plaquette, and it does not integrate a surviving old variable against a new reset posterior. The complete current density remains the C07/C08 density.

There is a useful source-specific result for the ordinary, uncontracted boundary primitives. Their current-independent parts cancel exactly from the normalized kernel. A genuine larger current tube, the raw-local variational component family, and the original full-tree bound then give small, actually supported current interactions. This is stronger than a bound on the sum of their endpoint derivatives.

The result does **not** cover a completed-component activity for which the primary source has contracted an entire old component for free. It also does not infer old-A derivatives from analyticity in the separate native pair (U,J). Those two distinctions remain material.

## 1. The exact sector and the source inputs

Fix an admitted geometry of the regular step k+1. Let z denote its integrated independent current coordinates. All other current coordinates, all surviving older free variables a, all raw determining entries v, and the fixed geometric data are retained.

The current density has the complete form

\[
 q_{v,a}(dz)=
 \frac{{\bf1}_{D}(z)
  \exp\{-\tfrac12 zK_{II}z+b\cdot z+W(z;v,a)\}\,dz}
 {\int_D\exp\{-\tfrac12 zK_{II}z+b\cdot z+W(z;v,a)\}\,dz}.
 \tag{BQ.1}
\]

Here D is the literal product cutoff, b=-K_{IO}y is retained, and W includes every assigned E/B/R, measure, constraint, old-density and relocation response. The proof below uses only the conservative inclusion |z_i|<=C P_k. It remains valid if the literal radii are smaller; it does not replace a printed shrinking radius by P_k.

An ordinary inherited boundary primitive is precisely a summand in CMP119 (2.40)–(2.42):

\[
 F_{j,X}(z;v,a)=
 B^{(j)}\bigl(X,(\Phi_k(z;v),J_k(z;v)),a|_X,S|_X\bigr),
 \qquad j\le k.
 \tag{BQ.2}
\]

The actual exterior relocation and the actual fixed-old-field gauge converter are included in the notation Phi_k. In particular (BQ.2) is the complete shifted function of C05, AB17.14–AB17.15; it is not a Taylor truncation of that shift.

The primary input is the uncontracted source bound

\[
 |B^{(j)}(X,(U,J),a,S)|
       \le B_0 e^{-\kappa_0 d_j(X)}.
 \tag{BQ.3}
\]

It holds on the stated native (U,J) domain, with the old a variables held real. The domain and gauge covariance are the literal clauses following CMP119 (2.41), printed p.261. Its support contains the actual old slots in X. The primitive meets the corresponding old boundary Z_j. The alternative discussed on p.262 replaces d_j(X) by d_j(X\setminus Z_j); that alternative is not an input to this theorem.

The other inputs are already separate primitive results:

1. The genuine simultaneous native ball NP.5 and the fixed-old-field identity AB17.11. They include the joined reconstructed predicates in (2.34)–(2.39), all independent current slots, and the real exterior relocation. A real bound at one center is not substituted for this ball.
2. The actual normalized mixed-map endpoint estimates BM.7–BM.13 and AB17.9, with a strict part of their exponential reserve left after preparation.
3. The raw-local regular reference GR.1, followed by the source force-containing fixed point and its component identity. Its reference force is retained. The complex family is an extension of the already specified normal form, not a new stationary point at each decoupler value.
4. The actual updated old-slot geometry, when an old Gaussian endpoint is used, is OS.1–OS.6 in M04_Surviving_Old_Slot_Geometry.md. Erased slots are absent. No collar is assigned on the strength of a retained age label alone.

These are assumptions on the source operation and its ordinary primitive action. They do not assume a marked numerator, a normalized scalar output, or SR20.23.

## 2. The larger current tube is real information

Write ell_k=log(g_k^{-2}), P_k=A_1 ell_k^{p_0}, and fix the source exponent q>p_0. There is a constant c_*>0, fixed after the spatial preparation constants, for which the ordinary sector admits

\[
 |z_i|<Q_k,\qquad Q_k=c_*\ell_k^q,
 \qquad
 \vartheta_k=P_k/Q_k\longrightarrow0.
 \tag{BQ.4}
\]

This statement concerns the analytic current coordinate, not the literal integration radius.

To verify it, repeat the already proved native admission estimate with g_k Q_k in place of g_k P_k. On an earlier physical layer n its normalized size is bounded by

\[
 C_R c_*(1+k-n)^b
          e^{-\Gamma(k-n-c_0)_+}.
 \tag{BQ.5}
\]

The fixed dyadic source-domain gap adds at most 2^{j-n}; the supremum is finite when the retained Gamma exceeds log 2. The joined reconstructed clauses use the same genuine NP.5 ball, and the nodal gauge converter has the same bounded native norm. The exterior relocation is a retained parameter and already uses a fixed smaller share of that ball. Choose c_* below the remaining common margin. This proves (BQ.4) simultaneously in all the native slots. It does not apply Cauchy first and then try to pay an order-dependent domain loss by one age exponential.

The same assertion holds on the enlarged spatial decoupler domain used below. Its fixed constants are included in C_R before c_* is chosen. Thus a bound only on the real cutoff, or only on an old-A interval, is not being promoted to a large complex tube.

## 3. Decouple in current physical cubes

Use one common partition into fixed cubes at the current physical scale. The full old primitive support X, including its actual older-coordinate footprints, is covered by a connected root set S_X of those cubes.

In the source mixed walk expansions, multiply a coefficient by the product of the parameters of the current cubes met by its **full** coefficient carrier. A native source cube has mesh at most the current mesh, and meets at most a fixed number of current cubes. Consequently the number of distinct current cubes met by a native coefficient tree is at most C times its native cube count. The source exponential therefore pays an enlarged fixed parameter radius R>1 after its native localization block size is fixed sufficiently large.

This grouping is useful: an arbitrarily large number of earlier fine coordinates inside one current cube does not create an arbitrarily large number of current decoupling parameters. Internal sums remain inside the analytic primitive coefficient, where the source operator norms already use the correct physical measures.

The GR reference and its coefficients depend only on their displayed raw native neighborhoods. The fixed-point equations and the old-slot gauge conversion are local on their corresponding native blocks. When all parameters outside a union of current cubes are zero, their root component therefore depends only on the raw retained data, current z entries, and actual old a slots in that component and its fixed collar. This is an exact component identity. It is not inferred from the numerical endpoint estimate.

For every ordinary primitive let F_{j,X}(s,z) be this common analytic family. It agrees with (BQ.2) at s=1. By Section 2 it obeys (BQ.3) on

\[
 |s_\Delta|\le R,\qquad \|z\|_\infty\le Q_k .
 \tag{BQ.6}
\]

The full current physical footprint of each fundamental-theorem coefficient is retained. One coefficient is one tag, together with its ordinary primitive and endpoint labels. Internal walk, fixed-point and Taylor indices are not claimed as separately absolutely summable tags.

## 4. Remove only the retained constant

Define

\[
 H_{j,X}(s,z)=F_{j,X}(s,z)-F_{j,X}(s,0).
 \tag{BQ.7}
\]

At s=1 the term F_{j,X}(1,0;v,a) is independent of the integrated z and cancels exactly between the numerator and denominator of (BQ.1). It remains in the outer density. No current-dependent factor, exterior force or old-coordinate dependence is removed from the probability law.

There is a dimension-free bound for (BQ.7). For fixed z with ||z||_infinity<=C P_k, apply the one-variable Cauchy estimate to lambda -> F_{j,X}(s,lambda z), on a circle of radius proportional to Q_k/P_k. It gives

\[
 |H_{j,X}(s,z)|
 \le C B_0\vartheta_k e^{-\kappa_0d_j(X)}.
 \tag{BQ.8}
\]

There is no factor equal to the number of fine field slots in this argument. In particular it is unnecessary to expose every coefficient of a multivariable Taylor series and then bound their sum.

For the anchored sum retain the exact identity

\[
 H_{j,X}(s,z)=
 \sum_{i\in I}z_i\int_0^1
             \partial_iF_{j,X}(s,tz)\,dt .
 \tag{BQ.9}
\]

Lie-algebra components can be split into their fixed finite multiplicity. The differentiated source map, its actual gauge converter and the primitive native Cauchy bound give the endpoint/age estimate of AB17.19, now on (BQ.6) with reserved rates. In this estimate a native attachment earlier than j is paid by its actual mixed-map path; an attachment later than j is paid by that path together with the original full primitive tree joining it to Z_j. The current-to-old-boundary collar is an additional available factor when its anchor is present. It is not assigned to newest boundary terms which lack that old anchor.

## 5. An ordinary physical-carrier interaction theorem

For a connected current carrier Y write

\[
 w_\nu(Y)=\exp\{\nu(|Y|+t(Y))\}.
 \tag{BQ.10}
\]

### Theorem BQ.1

On the fixed admitted ordinary source geometry, the exact sum of the responses (BQ.7) has a representation

\[
 \Theta_{\rm ord}(z;v,a)
   =\sum_\alpha V_\alpha(z_{Y_\alpha};v_{Y_\alpha},a_{Y_\alpha}),
 \tag{BQ.11}
\]

with connected full current physical footprints, and a rate nu>0 independent of volume, fine depth and k, such that

\[
 \sup_b\sum_{\alpha:\,b\in Y_\alpha}
 w_\nu(Y_\alpha)\,
 \sup_{\rm admitted}|V_\alpha|
       \le C B_0\vartheta_k .
 \tag{BQ.12}
\]

Every displayed V_alpha is the coefficient of the actual response in (BQ.9). There is a compatible, separately tagged first current-coordinate derivative expansion; at a smaller fixed carrier rate it obeys

\[
 \sup_b\sum_{\alpha:\,b\in Y_\alpha}
 w_{\nu'}(Y_\alpha)
 \sum_{i\in I\cap Y_\alpha}
       P_k\sup|\partial_iV_\alpha|
       \le C B_0\vartheta_k.
 \tag{BQ.13}
\]

The constants expose the ordinary source B_0. If the original current-to-Z_j guard is kept, the corresponding old-anchored subfamily has its additional exp(-c R_k) factor. The theorem does not rely on that factor for a newest primitive without such an anchor.

**Proof.** Apply the product fundamental theorem of calculus in the decouplers to each endpoint-tagged integrand of (BQ.9). By the exact component identity, a nonzero term contains both the ordinary primitive root S_X and its current endpoint i in one connected component, including the fixed collars. That term is a function of precisely the retained and current variables in its declared physical footprint.

For n differentiated cubes, Cauchy on (BQ.6) costs at most (R-1)^{-n}. The whole differentiated coefficient is bounded using (BQ.8), or the endpoint estimate following (BQ.9) when rooting the age and position sum. There is no n! because distinct decouplers are each differentiated once.

The number of connected current-cube sets of n added cubes with a specified root is at most A^n times the usual exponential in the root size. The original full-tree bound absorbs this root-size cost after reserving a fixed part of kappa_0. The full physical footprint has size plus tree length at most C_M(n+|S_X|). Choose R above the fixed connected-set entropy, then choose the source block preparation size, then choose nu sufficiently small that

\[
 A e^{\nu C_M}/(R-1)<1 .
 \tag{BQ.14}
\]

The source bound is on the uncontracted d_j(X). Thus rooted summation over X uses the remaining original tree exponential. Summation over its old birth positions contributes at worst L^{4(k-j)}. Its actual endpoint/tree connection supplies the reserved exp[-Gamma(k-j)] factor. Choose the fixed native separation so that Gamma>4 log L with room for the source's fixed polynomial and dyadic factors. This is the same physical age sum as OS.6 and AB17.25–AB17.26. It is taken after the connector has been identified, not assigned to every old label by convention.

These three absolutely convergent sums give (BQ.12). The endpoint construction allows the root of the norm to lie on the primitive support, on the current endpoint or on its connector; splitting the remaining tree rate pays the corresponding anchored position sums.

For (BQ.13), use Cauchy on a fixed smaller current tube for each coefficient before summing. There are at most C|Y_alpha| current-coordinate blocks in its carrier. A fixed loss nu-nu' pays that polynomial. The first nonzero current jet of (BQ.7) costs Q_k^{-1}; multiplication by P_k gives vartheta_k. All old coordinates remain parameters in this derivative estimate. This proves (BQ.13). ∎

The theorem is an unmarked input-side interaction estimate. Standard polymer majorants can now use these V_alpha as small vertices in the same density as the marked root. It does not use an estimate of QF to bound them.

## 6. Which retained derivatives this theorem has not proved

CMP119 states analyticity of B^(j) in (U,J). It does not in that statement give a complex product neighborhood of all earlier A variables. AB17.11 makes exactly the same distinction. Therefore (BQ.12) does not justify applying Cauchy in an arbitrary retained old-A direction.

This is a substantive issue. A bounded Gaussian completion can have order-one derivatives at its cutoff boundary even when its real logarithm is uniformly bounded: see gaussian_cutoff_completion_reference.md, GC.1–GC.3. A radius proportional to P_j cannot be inferred from that bound.

For the explicit ordinary old Schur sector, differentiation of its displayed endpoint factors is legitimate and elementary. The root note ordinary_schur_real_currents.md treats that sector separately. Derivatives of a complete ordinary cutoff integral can instead be obtained from its real normalized density score, with the boundary completion retained. Section 7 gives the useful exact estimate. Neither argument permits dropping a cutoff-completion term or declaring it independent of a retained variable.

The current coefficient family in Theorem BQ.1 has fixed geometry. A change of an actual discrete geometry record must carry the record's full footprint and the change of its incidence indicators. The theorem does not assign a local footprint to a global history flag.

## 7. A real score lemma for a complete Gaussian cutoff

This lemma supplies a concrete way to estimate retained endpoint response without an old-A complex disk. It applies to the full positive integral, including its cutoff completion.

Let K_t, 0<=t<=1, be positive symmetric matrices on I union O with common bounds m I<=K_t<=M I and uniform exponential row and column bounds. Write a for the fixed O coordinates and integrate z on a fixed product of convex symmetric balls D. Set x=(z,a) and

\[
 Z_t(a)=\int_D e^{-\frac12 x^T K_t x}\,dz,\qquad
 \nu_{t,a}(dz)=Z_t(a)^{-1}
                  e^{-\frac12x^T K_tx}{\bf1}_D(z)\,dz .
 \tag{BQ.15}
\]

The retained-only quadratic is included in Z_t and cancels in nu. Define Q_t(x)=x^T dot K_t x/2. Then

\[
 \partial_t\partial_{a_r}\log Z_t(a)
 =-\nu_{t,a}(\partial_{a_r}Q_t)
   +\operatorname{Cov}_{\nu_{t,a}}
       \bigl((K_t x)_r,Q_t(x)\bigr).
 \tag{BQ.16}
\]

This includes the conditional-mean, inverse and normalization responses. It is valid at a literal hard convex cutoff, because that integration domain does not depend on a or t. Differentiate under the finite integral and use the normalized quotient rule. Smooth convex approximation gives the same formula for nonsmooth balls when needed.

Let G_{uv}<=C exp(-gamma d(u,v)) be the weighted covariance majorant of RC18.24 for this Gaussian family. It holds uniformly under every real linear tilt. The mean is bounded by

\[
 |\nu_{t,a}z_u|
 \le \sum_{v\in I,r\in O}G_{uv}|(K_t)_{vr}|\,|a_r|,
 \qquad
 \|z_u-\nu_{t,a}z_u\|_2\le C.
 \tag{BQ.17}
\]

Indeed the centered box law has zero mean at a=0; interpolate the linear tilt -K_IO a and apply the covariance estimate. Consequently, with

\[
 m_u(a)=
 \begin{cases}
 C+\sum_{v\in I,r\in O}G_{uv}|(K_t)_{vr}|\,|a_r|,
       &u\in I,\\
 |a_u|,&u\in O,
 \end{cases}
 \tag{BQ.18}
\]

one obtains the pointwise bound

\[
 \begin{split}
 |\partial_t\partial_{a_r}\log Z_t(a)|
 \le{}&
 \sum_v |\dot K_{t,rv}|\,m_v(a)\\
 &+C\sum_{u,v\in I}\!
       |K_{t,ru}|G_{uv}
          \sum_w|\dot K_{t,vw}|\,m_w(a).
 \end{split}
 \tag{BQ.19}
\]

**Proof.** In (BQ.16), the direct derivative is sum_v dot K_rv x_v. The z gradient of (K_tx)_r is the row K_rI, and the z gradient of Q_t is dot K_II z+dot K_IO a. Apply RC18.24 and its L2 gradient norms; Minkowski and (BQ.17) give (BQ.19). The retained-only parts of either score have zero covariance and are not counted as random variables. ∎

This formula preserves an actual coefficient connector. For example, if dot K_t has a tagged coefficient carrier joining a native perturbation anchor to its two matrix endpoints, every term of (BQ.19) has that carrier joined to r by one of the explicit K/G kernels. Exponential convolution pays that added connection at a reduced fixed rate. If |a|<=P on the actual retained support, the numerical prefactor is C(1+P), not an inverse probability of the cutoff.

The normalized Gaussian determinant, when one is present in the chosen representation, is differentiated using the same K_t. Its a derivative is zero if K_t is independent of a. If K_t itself depends on a through an actual background map, its derivative is an additional matrix score; (BQ.16) must be applied to that full derivative. This lemma does not freeze that map.

An analytic nonlinear perturbation can be retained in the same argument when its full real-coordinate Hessian remains uniformly small and its mixed endpoint derivatives have a proved supported majorant. The score then contains those derivatives explicitly. This is a possible unmarked derivative induction, not a claim that a bounded B value supplies its premise.

## 8. The completed-component limitation is unchanged

After LFR II (1.103)–(1.104), the complete incoming boundary exponential has been integrated against the normalized component operations. The remaining raw multiplication masses are retained and current-independent in the next regular step. Their scalar interaction response is nevertheless in W of (BQ.1).

For that interaction the source deliberately omits the cost of the fixed component interior. Replacing its contracted carrier norm by (BQ.3) is invalid. Applying the above decoupler proof with the whole component as a root would charge exp(nu |Y|); the source's exp(-c R) small factor does not generally pay exp(nu cR^4).

The bounded-core reference and the energy-weighted quotient route are promising precisely because they seek a different **actual raw** component identity before this whole-Y grouping. GR supplies a local regular reference for its primitive variational maps, and OS supplies real age separation for every surviving old slot. One must still construct the entire coefficient-aligned old Schur/coarea/cross density comparison on that reference. Native (U,J)=(1,0) freezing is not that construction.

Thus this note establishes the ordinary full-tree interaction conversion, and a complete real cutoff score formula which can be used for old endpoint responses. It does not complete the contracted-component kernel estimate or the full M03 history-current theorem.

## Mathematical sources

- CMP119, printed pp.260–262, (2.34)–(2.42): actual native boundary domain, full-tree primitives, old parameters and the explicitly weaker contracted alternative.
- CMP119, pp.253–254, (1.26)–(1.29), and p.258, (2.20)–(2.21): complete conditional Gaussian completion and the surviving old Schur form.
- CMP116, (1.7)–(1.18): common decouplers, enlarged parameter disks and exact component separation.
- C-05 estimates, NP.5, AB17.9–AB17.19, AB17.25–AB17.27: the genuine current/native domain and the source endpoint/age majorants.
- C-08 estimates, RC18.20–RC18.27 and RC18.31–RC18.36: the weighted covariance operator on the actual convex product support.
- graded_bundle_reference.md and flat_chart_variational_carriers.md: primitive raw-local reference and common component construction.
- M04_Surviving_Old_Slot_Geometry.md: actual updated annuli and the rank-versus-age sum, without a fictitious historical collar.
