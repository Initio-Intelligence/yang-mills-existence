# Two-step QQ currents with their origins retained along one physical path

This note establishes a **path-integrated current convention** for the two homogeneous, R-averaged native regular steps of CA/TD/MS. Its three records retain the original microscopic-readout, first normalized-kernel, and second normalized-kernel origins. The convention is an explicit amendment: it is not the endpoint-rectangle convention of MS.24 and RC.7. The original M04 assertion is not changed.

The main point is that the actual first derivatives can be localized on the diagonal. They do not require a single frame fixing two distinct retained copies. Their existence and additivity are proved from the actual cutoff geometry. They are not inferred from a generic Lipschitz function's partial derivatives on a diagonal.

## 1. The two actual laws and the three physical origins

Use the native buffered domain and all source conventions of BA, CA and MS. Put `h_1=Lh_0`, `h_2=L^2h_0`. All running couplings, localization grids, source gauges and geometric parameters stay fixed during a current. The microscopic mark is

\[
 F(U)=\alpha\beta_0\sigma_{h_0}(x;U)-c,
 \qquad b=|\alpha|+h_0^4|c|.
 \tag{DP.1}
\]

Write `a` for the next independent free coordinates and `z` for the first independent free coordinates. Exceptionals are reconstructed variables, not extra integration coordinates. Let

\[
 V_W(a)=\Psi_W(a),\qquad f(z,a,W)=F(\Phi_{V_W(a)}(z)).
 \tag{DP.2}
\]

Let `q_{0,P}` and `q_{0,Q}` be the actual first normalized conditionals. Let `nu_W` be the second analytic-base conditional with its **actual next Q cutoff**. It already contains the first P coarse density once. With the exact first mass ratio,

\[
 m_P(V)=1,\qquad
 m_Q(V)=\frac{Z_{0,Q}(V)}{Z_{0,P}(V)}=e^{H_1(0;V)},
\]
\[
 q_{1,\eta,W}(da)
 =\frac{m_\eta(V_W(a))\,\nu_W(da)}
        {\nu_W[m_\eta(V_W)]},\qquad \eta=P,Q.
 \tag{DP.3}
\]

Thus `eta=P` denotes first P/second Q, and `eta=Q` denotes first Q/second Q. Their conditional microscopic means are

\[
 F_{2,\eta}(W)
 =q_{1,\eta,W}\left[
       q_{0,\eta,V_W(a)}[f(z,a,W)]\right].
 \tag{DP.4}
\]

Every first/second normalizer, determinant, Haar/coarea term and required normalized gauge-preimage factor remains in these laws. A retained-only factor common to numerator and denominator is canceled exactly before defining a normalized kernel. For the gauge-invariant mark (DP.1), the independent normalized preimage Haar variables do not change any formula.

Fix one buffered elementary retained path `W(theta)=tau_{d,theta}W`, `|theta|<=1`. Define the following derivatives in the **original coordinates**, before any localization change of variables:

\[
 j^M_\eta(\theta)
 =q_{1,\eta,W(\theta)}q_{0,\eta,V_{W(\theta)}(a)}
       [\partial_\theta f(z,a,W(\theta))|_{z,a}],
 \tag{DP.5}
\]
\[
 j^0_\eta(\theta)
 =q_{1,\eta,W(\theta)}
       \left[(\partial_\theta q_{0,\eta,V_{W(\theta)}(a)}|_a)
                    [f(z,a,W(\theta))]\right],
 \tag{DP.6}
\]
\[
 j^1_\eta(\theta)
 =(\partial_\theta q_{1,\eta,W(\theta)}|_a)
       \left[q_{0,\eta,V_{W(\theta)}(a)}[f(z,a,W(\theta))]\right].
 \tag{DP.7}
\]

In (DP.6) the kernel derivative holds the original `z,a` coordinates fixed and differentiates its density, domain and normalization; its displayed test function is held fixed at the current parameter. In (DP.7) the entire first conditional mean is held fixed as a function of `a`. In particular **all first-Q factors occurring inside the second density or its normalizer belong to origin 1**, including their derivative through `m_Q(V_W(a))`. They do not belong to origin 0. Normalizer derivatives of these two origins may cancel in the sum, but are retained and bounded separately.

Sections 2--3 prove the existence of the relevant weak derivatives and the identity, for almost every path time,

\[
 \frac{d}{d\theta}F_{2,\eta}(W(\theta))
       =j^M_\eta(\theta)+j^0_\eta(\theta)+j^1_\eta(\theta).
 \tag{DP.8}
\]

The rare correction and its origin derivatives are

\[
 \mathcal E=F_{2,Q}-F_{2,P},\qquad
 j^r_\Delta=j^r_Q-j^r_P,\quad r=M,0,1.
 \tag{DP.9}
\]

Subtraction in (DP.9) is performed within each physical origin before absolute estimates.

## 2. Actual shape differentiation, including coincident Q faces

The literal starred Q tests have the form

\[
 \|e^{igu_e}M_{e,\ell}(y,\theta)-I\|<2gP,
 \qquad 1\le\ell\le J_*.
 \tag{DP.10}
\]

Here `y` comprises the other real latent coordinates and the native retained data needed by the actual reference maps. The number of tests at one slot is bounded. Their full reference boxes are included in the corresponding core. For the source operator norm, not a substituted scalar norm, these are real semianalytic domains on the principal logarithm chart. Indeed for a unitary `U` the squared norm bound is equivalent to positivity of the Hermitian matrix

\[
 (2gP)^2I-(2I-U-U^*),
\]

which is a finite set of analytic principal-minor inequalities. The Hilbert--Schmidt convention, if used in an intermediate source coefficient, is simpler and causes no extra difficulty. The distinction between the operator norm and Hilbert--Schmidt norm is explicit in CMP98, printed p.21, (18)--(20).

We use the compatible semianalytic stratification theorem of E. Bierstone and P. D. Milman, *Semianalytic and subanalytic sets*, Publications Mathématiques de l'IHÉS **67** (1988), printed p.14, Proposition 2.10 and Corollary 2.11; [primary PDF](https://www.numdam.org/item/PMIHES_1988__67__5_0.pdf). It gives a locally finite analytic-stratum cover compatible with the finite collection of domains and their boundaries. A countable chart cover suffices below. There is no assumption that an operator-norm sphere is pointwise smooth.

Each individual test is the analytic diffeomorphic image, in its own independent slot, of one fixed small group-norm ball. On a regular boundary stratum its spatial normal in that slot is nonzero. Thus a spatial slot coordinate can be solved for with theta retained as a graph parameter; this is not a chart whose only normal is the time direction. The actual starred free chart and eliminated exceptional variables are material here: there is no remaining delta constraint identifying an old slot with a next slot. On the physical supports and on the relevant whole-Q core coordinates the caps are the identity, so all these reference and boundary maps are analytic in the real variables used in the strata.

### Lemma DP.1 — an almost-everywhere linear shape current on the actual path

For a finite collection of tests (DP.10), the integral against a smooth density on the admitted chart is locally absolutely continuous in `theta`. At almost every `theta`, its shape derivative is a signed boundary measure. On a regular part of the boundary of the intersection, its normal velocity is the velocity of any active face defining that regular part, counted once. This velocity is linear in the actual parameter/spatial transport direction. The assertion holds for the original two-layer product and for the localized real-core domains used below.

**Proof.** QS.6 gives an `O(|t|)` symmetric-difference bound, locally uniform in the parameters. The same bound after multiplication by a smooth bounded density proves local absolute continuity at finite volume.

Consider two regular boundary sheets on one spacetime graph chart,

\[
 x_1=h_i(x',\theta),\qquad x_1=h_j(x',\theta).
 \tag{DP.11}
\]

If `h_i-h_j` is not identically zero in `x'` at a fixed `theta`, its analytic zero set has zero graph measure. If it vanishes identically in `x'` at a positive-measure set of path times, every `x'` Taylor coefficient vanishes identically in `theta`; hence the two graphs agree jointly on the chart. More explicitly, if joint equality fails, one nonzero analytic Taylor coefficient has only isolated zeros on the path interval, and all times of identical graph equality lie among those zeros. Taking the countable union over charts and pairs leaves a null exceptional set of times.

Thus at almost every time, two faces can share positive boundary measure only when their local graphs agree jointly in `(x',theta)`. In that case their theta derivatives and all graph-variable derivatives agree. Their intrinsic normal velocities are consequently equal for every linear combination of those real tangent directions. Count the shared face once, using a fixed local ordering of the defining tests. A change of defining equation by a nonvanishing positive analytic factor does not change that normalized velocity or the boundary measure.

Nonidentical sheets meet in a set of zero boundary measure. Their two thin shells therefore have intersection `o(|t|)`, by the one-shell bound and dominated convergence on regular graph patches. Only cooriented sheets can define the same positive-volume side of a reduced boundary; oppositely oriented coincident sheets do not contribute an additional reduced-boundary face.

The absence of hidden first-order mass at singular strata uses more than their dimension. In its small logarithm chart the fixed group operator-norm ball is the exponential image of a convex operator-norm ball: `||exp(iH)-I||=2 sin(||H||/2)` in this range. It has finite perimeter, and compact regular boundary patches exhaust its perimeter measure. Each actual single-test domain is its translated analytic image, with bounded chart/velocity Jacobians on the current compact parameter set. The finite-perimeter change-of-variables/Gauss--Green formula, or the corresponding swept-layer area formula on a regular exhaustion, bounds the first-order variation carried by the omitted boundary patches by their perimeter measure times the velocity bound. This can be made arbitrarily small. The QS.6 shell bound supplies the uniform domination. Since an intersection's symmetric difference is contained in the union of its single-test differences, this also controls the singular remainder for the intersection. Thus the regular graph calculation accounts for the entire first-order measure.

Distinct old slots, and an old face versus a new face, have a stronger transversality property: the old face has a nonzero normal in its own old `z_e` block, whereas a new face has no old-z dependence. Their joint shell volume is `O(t^2)` on regular compact patches, with a finite chart constant. Independent old integration copies used by normalization have their own distinct z blocks and obey the same argument. No uniform angle independent of the cutoff is needed for the derivative-existence statement.

One may verify the formula by replacing each constraint with a monotone smooth transition and then removing its thickness. At jointly identical faces the product of transitions has total unit jump, so the common face is counted once rather than once per duplicate test. The shell estimates provide the dominated bounds. All cross-level first-order product terms vanish as just described. This proves the actual shape/product rule, including corners and coincident faces. ∎

The linearity assertion is deliberately restricted. It does not say that arbitrary independent-copy velocities at a diagonal cusp agree. The velocities used below are linear combinations of the real specified-chart tangent vectors appearing in (DP.11). This distinction is what excludes the invalid generic `|u-v|` argument.

### Normalized kernels

If `N_theta` is any of the actual finite positive measures and `Z_theta=N_theta(1)>0`, its weak derivative on this path is

\[
 \dot q_\theta=Z_\theta^{-1}\dot N_\theta
           -q_\theta Z_\theta^{-1}\dot N_\theta(1).
 \tag{DP.12}
\]

The first term contains the smooth-density and boundary measures. Positivity and continuity give a positive local lower bound on `Z_theta` at fixed finite volume, sufficient for this identity and absolute continuity. No volume-uniform estimate is inferred from that lower bound. The uniform estimates below instead use the exact connected normalization, with the same denominator on both sides.

First conditional means have continuous, locally Lipschitz versions by the same shell estimates. Their values on a next-Q boundary are therefore unambiguous. Applying Lemma DP.1 first to the conditional old integrals and then to the joint `(z,a)` domain gives (DP.8). This also justifies the derivative of the old mass inside (DP.3). It is an actual product rule for these domains, not an invocation of almost-everywhere differentiability in a larger copy space followed by restriction to its diagonal.

## 3. Exact transport of each origin to the diagonal core frame

For each primitive old-core component use exactly CA's core `C`, full independent constraint stencil `S`, additive halo `D_C`, and common coefficient registry. The carrier includes every old analytic connector. Keep next Q whole on `S`, and expand it only off `S`. No enclosing rectangle is substituted for the union of the core halos.

On the next variables the exact map is CA.11,

\[
 a=A_s(B,\theta),\qquad
 A_{s,e}(B_e,\theta)=\frac1{ig_1}
   \Log(e^{ig_1B_e}V_{D,e}(\theta)V_{s,e}(\theta)^{-1})
 \quad(e\in S).
 \tag{DP.13}
\]

It is the identity outside the prescribed slots. The first QC change of frame on each old Q-defect slot must also be retained. Use the canonical local old reference of NP.14--18: one literal Q comparison box is chosen by a fixed geometric rule, independently of every analytic connector. Write the map `z=T_{0,s}(u,B,theta)`; it is the exact first free-link logarithm comparing that real local old reference with the continued old global frame. It is the identity on ordinary old slots. Together they give one triangular coordinate map

\[
 (z,a)=\mathcal T_s(u,B,\theta)
       =(T_{0,s}(u,B,\theta),A_s(B,\theta)).
 \tag{DP.14}
\]

All original source and new frame Jacobians remain in the integrals. On a physical finite-volume identity one may use the complete lists; the carrier estimates use only the declared primitive marginal lists and their common completions. No extensive list is charged to a local core.

Both diagonal blocks of `D_(u,B) T_s` are uniformly invertible on the actual chart and its specified small contour neighborhood. The next block is CA.12. The old block is the fixed-L logarithm-chart Jacobian in QS.11--13. Define

\[
 v_{1,s}=(D_BA_s)^{-1}\partial_\theta A_s,
\]
\[
 v_{0,s}=(D_uT_{0,s})^{-1}
       (\partial_\theta T_{0,s}-D_BT_{0,s}v_{1,s}),
\]
\[
 \mathscr L_s=\partial_\theta-v_{0,s}\cdot\partial_u
                                  -v_{1,s}\cdot\partial_B.
 \tag{DP.15}
\]

For a scalar original-coordinate factor `G`, the chain rule is exactly

\[
 [\partial_\theta G(z,a,\theta)|_{z,a}]\circ\mathcal T_s
                   =\mathscr L_s(G\circ\mathcal T_s).
 \tag{DP.16}
\]

For a density/top-form the corresponding statement is its pullback identity with the Lie/divergence term. The safe convention here is simpler: differentiate the physical factor and its domain **first**, then pull that signed form/current back with its full Jacobian. The Jacobian introduced solely by (DP.14) is not independently differentiated and assigned to a physical origin. If one instead differentiates a pulled-back top form, its Lie term must be retained in full so as to give the same result.

In particular (DP.6) differentiates only the old conditional factors. The new Q indicator multiplying that current is left untouched. A new-Q boundary term must not be attributed to origin 0 merely because the coordinate map in (DP.14) depends on theta.

Here are the explicit triangular density identities. Let `J_0=det D_uT_{0,s}`, `J_1=det D_BA_s`, and, with the respective characteristic domains included distributionally, put
\[
 \widetilde q_0=J_0(q_0\circ\mathcal T_s),\qquad
 \widetilde q_1=J_1(q_1\circ A_s),\qquad
 \widetilde f=f\circ\mathcal T_s.
\]
Because `v_1` has no u dependence, differentiating the two Jacobians gives
\[
 \mathscr L_s\log J_0=\operatorname{div}_u v_{0,s},\qquad
 (\partial_\theta-v_{1,s}\cdot\partial_B)\log J_1
                 =\operatorname{div}_Bv_{1,s}.
 \tag{DP.16a}
\]
Consequently the origin-0 and origin-1 density derivatives are exactly
\[
 J_0[(\partial_\theta q_0)|_{z,a}]\circ\mathcal T_s
       =(\mathscr L_s-\operatorname{div}_u v_{0,s})\widetilde q_0,
\]
\[
 J_1[(\partial_\theta q_1)|_a]\circ A_s
       =(\partial_\theta-v_{1,s}\cdot\partial_B
                   -\operatorname{div}_Bv_{1,s})\widetilde q_1.
 \tag{DP.16b}
\]
The mark uses `mathscr L_s tilde f`. Multiplying by the untouched factors and adding the three expressions gives
\[
 \partial_\theta(\widetilde q_0\widetilde q_1\widetilde f)
       -\operatorname{div}_{(u,B)}
                  (v_s\widetilde q_0\widetilde q_1\widetilde f).
 \tag{DP.16c}
\]
These equations hold as weak first-jet identities, including all domain fluxes. In particular the old density has the **fiber** divergence `div_u v_0`, whereas the outer density has `div_B v_1`. The first/second normalizer derivatives are still the derivatives of their actual factors in these expressions. Fixed original P domains have zero physical shape derivative. If an equivalent transported representation creates a P side-boundary term, its compensating Lie term is retained in the same origin; it is not discarded or assigned to another kernel. Such side terms are also at the original P radius and retain the corresponding Gaussian reserve.

On the full old core the fixed-target exceptional solve gives CA.13:

\[
 \Psi_{s,W(\theta)}(A_s(B,\theta))|_C=V_C^D(B,\theta).
 \tag{DP.17}
\]

Its differentiation yields the useful physical old-input velocity identity

\[
 [\partial_\theta\Psi_{s,W(\theta)}(a)|_a]_{a=A_s}|_C
 =\partial_\theta V_C^D
       -D_BV_C^D(D_BA_s)^{-1}\partial_\theta A_s.
 \tag{DP.18}
\]

The full exceptional/gauge/readout stencil in `S` is essential to both identities. They are not statements only about the starred entries. For real `(u,B,theta)`, the old Q-domain inputs in (DP.17), the local old Q domains in `u`, and the whole next Q domains on `S` are real and independent of the outside parameters `s`.

Equation (DP.18), and more generally (DP.15), expresses every continued physical velocity as a linear combination of real specified-chart `(u,B,theta)` tangent vectors with analytic coefficients in `s`. If two old boundary sheets agree jointly in these variables, their normal velocities agree for every such coefficient combination, even when those coefficients are complex. Lemma DP.1 therefore supplies one well-defined boundary current on that face throughout the outside family. The measure and its normal covector are real and local; only its multiplying velocity and density coefficients are continued. No hard indicator is evaluated at a complex input.

## 4. Supported tangent insertions and their positive reserve

### Lemma DP.2 — the diagonal velocity insertions fit the actual primitive certificates

For one normalized raw direction, the coefficients in (DP.15)--(DP.18) have common supported analytic expansions on the same fixed outside polydiscs as CA. Their direction-summed absolute envelopes cost only a fixed polynomial in the primitive carrier incidences, the two native cutoff parameters, and the two core radii. No growing halo is attached to an ordinary analytic connector.

**Proof.** CA.5 and CA.10 supply the actual normalized raw derivative of the common next background and of its omitted-carrier tail. Inverting `D_BA_s=I+O(g_1a_*)` uses its convergent supported Neumann series. The old frame is the actual map `Log(e^{ig_0u}U_*U_s^{-1})/(ig_0)`; its first coordinate Jacobian and inverse have fixed chart bounds. Its raw derivative includes the actual physical reference derivative, rather than a value bound divided by `g_0`. The normalized raw step contributes `g_2`, so its explicit ratios are `g_2/g_1` and `g_2/g_0`, both bounded at these two fixed levels. Derivatives through `B` carry the physical `g_1` factor. The actual fixed-L exceptional maps and gauge conversions have bounded local analytic derivatives and all their footprints are already included.

The products in (DP.15) are supported products of these very coefficient families. Their absolute convolutions are controlled after a fixed carrier-rate loss. Cauchy on a smaller fixed geometric tube, and the normalized physical raw step, supplies the corresponding derivatives. The number of coordinate/direction incidences is polynomial in the full carrier size. It is paid by another fixed rate loss. Local Q-reference boxes give at most the core-volume and cutoff polynomials already allowed in CA.25. The maps on all moved coordinates stay in the analytic plateau of the caps, by CA.15--16. The constructions remain restrictions of one registry and therefore preserve component identities. ∎

The rare estimates must be taken **after the per-origin subtraction (DP.9)**. In particular one must not split a transported Lie/divergence expression into unrelated whole-Q and whole-P volume terms and bound them independently, which would throw away the old defect.

At a first-Q boundary, the old local real coordinate has norm at least `3P_0/2`; its bounded contour displacement leaves norm at least `P_0-O(1)`. Replacing a first-Q annulus/chain factor by its signed shape current therefore retains the Gaussian tail on that slot. Its perimeter, velocity and fixed polynomial insertions consume only a fixed portion of the same reserve. This is QS.6, QS.8--17 applied to the velocity of Lemma DP.2. Ordinary smooth old derivatives keep an existing old Q defect in the same manner.

For a whole new-Q boundary on `S`, the old certificate CA.22 is uniform in the real new `B`. It can be multiplied by the new surface measure before the new integration. The new centered marginal supplies its own tail/perimeter bound; no conditional old reserve is divided out. Off `S`, the usual next-Q chain is analytic in the old payload's analytic variables, since `S` contains all its nonanalytic physical inputs. Thus that chain has the same admission and reserve as CA.25.

More explicitly, after the **single first-source Cauchy extraction** described in Section 5, for an old-defect primitive with `n>=1` old defect slots, ordinary majorant `A_I`, old/new marginal ranks `r_0,r_1`, and core stencil `S`, each of the three differentiated primitive forms obeys an absolute bound of the type

\[
 C M_F A_I\,\operatorname{poly}(P_0,P_Q,R_1,R_2,n,|I|)
       e^{\eta r_0+u_{m_1}r_1+C|S|}e^{-c nP_0^2},
 \qquad M_F=b h_0^{-4}P_0^2.
 \tag{DP.19}
\]

The old rank coefficient `eta` and the next marginal buffer loss are tunably small. Rank losses are charged **per primitive Gaussian copy before its connected sum**. Repeated overlapping copies retain their distinct rank charges. The growing stencil cost is additive in the number of actual old defect cores and is paid by their old tails, exactly as in CA/TD. The full microscopic source in `M_F` includes its retained first background, by MS.1. It is a joint pre-integration coefficient bound on the capped native family, not a bound inferred from the already-integrated output.

Only the distinguished source/root copy needs its source reserve. All additional unmarked old copies have CA.22 uniformly in real `B`, with no new `B`-quadratic source loss per copy. Smooth normalized-kernel responses include both covariance-inverse and determinant terms and every inherited action/coarea term. The complete critical-cancelled normal form is differentiated; no uncontrolled bare-force term is reinstated.

## 5. The same denominator, and old rarity separately for each origin

There is a simple exact algebra before any carrier extraction. Write `f_eta(a,theta)=q_{0,eta,V_W(a)}f`. For either old origin `r=M,0`, denote its first conditional current by `D^r f_eta`. Then

\[
 q_{1,Q}D^r f_Q-q_{1,P}D^r f_P
 =q_{1,Q}D^r(f_Q-f_P)+(q_{1,Q}-q_{1,P})D^r f_P.
 \tag{DP.20}
\]

Here `D^r(f_Q-f_P)` means the difference of the same two separately defined origin records, not a reassignment of the derivative of the total field. The first term contains the first Q/P source/current defect. The second contains the old unmarked mass defect from `m_Q-1`, multiplying the full first-P primitive current. The latter includes the first retained background. At one fixed source radius `|t| M_F<=eta_*` that full primitive is covered by MS's pre-Gaussian certificate.

For the new origin,

\[
 (\dot q_{1,Q})f_Q-(\dot q_{1,P})f_P
 = (\dot q_{1,Q})(f_Q-f_P)
           +(\dot q_{1,Q}-\dot q_{1,P})f_P.
 \tag{DP.21}
\]

The first term has a source-containing old defect. In the second, differentiating the exact normalized tilt (DP.3) gives either an old defect, an old defect current, or a new-kernel current multiplied by that defect. Every term retains at least one old Q colour. A derivative of an old mass that occurs here retains origin 1.

For exact normalization keep the original ownership of all first and second factors and their inverses. Use CN's same-gas excluded-vacuum identity and TD's full old-exponential gas. The full physical denominator at old-colour parameter one is `Z(z+u)`, not the analytic-base `Z(z)`. The first normalizer occurring in origin 0 and the old mass inside origin 1 can be algebraically related, but their derivative colours are kept before any such cancellation.

The construction can be stated in a first-jet algebra: attach a nilpotent symbol `epsilon_r` to the actual signed derivative of each factor owned by origin `r`, with the usual product and inverse rules. Transport each factor/current with (DP.14), rather than assigning derivatives by its location after that change. Component extraction and connected-log extraction are algebraic in these jets. The exact root-deletion identity of CA still holds: a vacuum component disjoint from the entire source/current/core/connector carrier is precisely its unmarked component, with the same reference, covariance, determinant and literal cutoffs. It cancels against the same denominator. An excluded vacuum cluster meeting the root costs its anchored small budget on that full carrier, as in CN.

Consequently the positive coloured tree majorant used in TD/MS applies separately to each `epsilon_r` coefficient. By (DP.20)--(DP.21), every surviving connected term contains both the microscopic source and at least one old Q defect or its boundary-current replacement. The fixed polydisc is chosen once over the entire real path and its outside families. For one source it has radius `c/M_F`. Source Cauchy contributes `C M_F` exactly once: this is the factor already displayed in (DP.19), not a second source cost. The polynomial in (DP.19), all core costs, and that `P_0^2` factor are paid by fixed portions of the old tail. Ordinary rank and connector costs are paid from the strict ordinary spatial rate, not by attaching a growing halo to every connector.

This proves, with a fixed positive carrier rate and one common family of tags,

\[
 h_2^4\sum_{Z\ni x^{(2)}}e^{\kappa n(Z)}
       \sup_{W}\sum_d\sum_{r=M,0,1}
          |j^r_{\Delta,Z,d}(W)|
 \le C_L L^8 b\,e^{-c'P_0^2}
 \tag{DP.22}
\]

at all regular path times; the statement means the common deterministic envelopes for those almost-everywhere currents, including their limits on regular strata. No derivative of an extensive unlocalized vacuum logarithm is bounded here. All current responses are rooted before the absolute sums are taken.

### Coefficientwise identity

For clarity, start from the following occurrence-level source integral, before canceling any factor:
\[
 \mathcal G_\eta(t,W)=
 \frac{\displaystyle
   \int n_{1,P}(a,W)m_\eta(V_W(a))
       Z_{0,\eta}(V_W(a))^{-1}
       \left[\int n_{0,\eta}(z,V_W(a))e^{t f(z,a,W)}\,dz\right]da}
      {\displaystyle\int n_{1,P}(a,W)m_\eta(V_W(a))\,da}.
 \tag{DP.22a}
\]
The characteristic domains are part of their respective `n` factors. The source factor has origin M; `n_0` and its displayed conditional `Z_0^{-1}` have origin 0; the outer density, `m_eta`, and the outer denominator have origin 1. In particular the occurrence of `Z_{0,Q}` in `m_Q=Z_{0,Q}/Z_{0,P}` and the displayed old conditional occurrence have equal zero-jet values but retain independent ownership labels. Form their values and signed origin jets together, using
\[
 (A+\epsilon a)^{-1}=A^{-1}-\epsilon A^{-2}a,
 \qquad \epsilon^2=0,
 \tag{DP.22b}
\]
before any cancellation, component extraction or connected expansion. Apply the same coordinate map, coefficient substitutions, covariance/determinant continuation and theta differentiation to each occurrence. Thus no independently chosen continuation is supplied only for a derivative.

Each conditional uses identical occurrence-level numerator and denominator jets. Consequently, in each admitted outside family represented by the convergent same-gas expansion,
\[
 q_{0,s}(1)=q_{1,s}(1)=1,\qquad
 \dot q_{0,s}^{\,0}(1)=\dot q_{1,s}^{\,1}(1)=0.
 \tag{DP.22c}
\]
The source-free mark jet is zero as well. This rules out source-free extensive origin currents that disappear only after summing origins. Old normalization derivatives stay in their actual integral/current expansions; (DP.22c) does not promote a moving-Q normalizer to a smooth local coefficient.

The value and all three derivative colours are formed in the **same** primitive/component registry. At every outside parameter the transport identities, including the domain transport and full Jacobians, give the sum of the three physical-origin jets as the theta derivative of that one integral family. This is the exact change-of-variables/product identity, not a choice of three unrelated continuations agreeing only at the physical endpoint. The same real core domains and the same tail envelopes justify differentiation under their integrals. Fixed decoupler coefficient extraction therefore commutes with this derivative. Normal convergence of the connected series then gives

\[
 \frac{d}{d\theta}\mathcal E_Z(W(\theta))
      =\sum_{r=M,0,1}j^r_{\Delta,Z,d}(W(\theta))
       \quad\hbox{for almost every theta}.
 \tag{DP.23}
\]

Tied-face ownership is local to the full fixed reference core and the fixed ordering of its tests. It introduces no new remote flag. All geometric tags and grids are fixed on the path.

## 6. Exact finite path records

For `0<|t|<=1` define

\[
 J^{r,\mathrm{path}}_{Z,d,t}(W)
    =\frac1t\int_0^t
             j^r_{\Delta,Z,d}(W(\theta))\,d\theta,
       \qquad r=M,0,1.
 \tag{DP.24}
\]

Exceptional path times have measure zero and do not affect the definition. The fixed common envelopes justify coefficientwise integration. From (DP.23),

\[
 \Delta^{\mathrm{norm}}_{d,t}\mathcal E_Z(W)
    =J^{M,\mathrm{path}}_{Z,d,t}
       +J^{0,\mathrm{path}}_{Z,d,t}
       +J^{1,\mathrm{path}}_{Z,d,t}.
 \tag{DP.25}
\]

The sign of `t` is handled by the oriented integral. The values of the original kernels at every endpoint are unchanged.

### Theorem DP.3 — rare two-step microscopic correction with origin-preserving path currents

For the actual native homogeneous two-step operation (DP.3)--(DP.4), the first Q/P rare microscopic correction admits connected raw-supported value tags and the three records (DP.24), with

\[
 h_2^4\sum_{Z\ni x^{(2)}}e^{\kappa n(Z)}
 \left[
   \sup_W|\mathcal E_Z(W)|+
   \sup_W\sum_d\sup_{0<|t|\le1}
           \sum_{r=M,0,1}|J^{r,\mathrm{path}}_{Z,d,t}(W)|
 \right]
 \le C_L L^8 b\,e^{-c'P_0^2}.
 \tag{DP.26}
\]

The value estimate is the same source-containing old-colour estimate as MS. The current estimate follows by integrating the common deterministic tangent envelopes from (DP.22). Those envelopes are uniform in native retained data, so summing direction suprema after path integration does not introduce a new factor. Each tag includes all original reference, constraint, gauge, current and connector footprints. The engineering factor is explicitly `h_2^4/h_0^4=L^8`.

This theorem is for one microscopic source derivative. It does not establish an all-order origin-current theorem merely from the first-order proof.

## 7. Relation to the absolute baseline and the specified current convention

The first-P/second-Q baseline of MB has admitted three-copy records and an absolute energy-graded root bound. Its own diagonal derivatives, defined by (DP.5)--(DP.7) with `eta=P`, obey the same bound: the two inner P-copy derivatives are smooth; the sole outer Q derivative uses the same shape lemma and MB's whole-contour coefficient estimates. Integrating those **baseline diagonal derivatives**, rather than substituting the numerical endpoint-rectangle records, gives baseline path records with the original three origins.

Use the baseline value family and the rare value family from these same first-jet constructions, allowing a common reindexing of their tags, to define `A_Z^QQ`. The sum is the actual QQ microscopic output. Adding their path records gives its actual QQ path records, with termwise finite-difference compatibility. We do not attach new currents to an unrelated specified value representation. The rare estimate is unweighted, so `R_Z>=1` and the same shifted regulator absorb it. Hence the absolute two-step estimate is

\[
 h_2^4\sum_Z e^{\kappa n(Z)}
 \left[
  \sup_W\frac{|A_Z^{QQ}(W)|}{R_Z(W)}
  +\sup_W\sum_d\sup_{0<|t|\le1}
       \frac{|J^{M,\mathrm{path}}_{Z,d,t}|
            +|J^{0,\mathrm{path}}_{Z,d,t}|
            +|J^{1,\mathrm{path}}_{Z,d,t}|}
             {\widehat R_Z(W)^{3/2}}
 \right]\le C_L L^8 b.
 \tag{DP.27}
\]

Apply the final scalar/identity projector of MB.29 to this same value family. Absolute convergence and the projector's linearity identify the summed scalar and identity coefficients with those of the actual output. Its scalar subtraction contributes its separate explicit extraction current; all three existing path records remain recorded. The original fixed incoming normalization factor is the one in MB.31.

Equations (DP.24)--(DP.27) do **not** assert equality with the finite endpoint rectangles of MS.24 or RC.7. Integrating a partial response along the diagonal generally differs from evaluating that partial response along the corresponding off-diagonal rectangle. The relative-frame gate in RC.13--14 is not disproved or silently bypassed. What is proved is a different, explicitly defined finite-current interface whose sum is the same actual finite difference and whose origins are the exact physical product-rule origins at every regular path time.

The remaining scope restrictions are unchanged: the operation is the specified homogeneous R-averaged native regular operation; no arbitrary active history, ambient extension, outer-law moment reserve, complementary P/Q sector, all-depth induction, complete outer physical hierarchy or Yang--Mills existence theorem follows. In particular the amended path convention does not prove the original fixed-history M04 statement or its canonical endpoint required conclusion.

## Source and proof inputs

Actual source domains/solves: CMP119 (1.14)--(1.19), (3.7)--(3.9), (3.15), (3.17)--(3.19); CMP98 (18)--(20) for the norm convention. Complete inherited analytic families and gap: BA and the source references stated there. Exact real shells and contour reserves: QS.1--17. Common actual constrained core frame and uniform conditional reserve: CA.11--25. Same-denominator normalization and coloured summation: CN, TD. Full microscopic pre-integration source budget and first source jets: MS.1 and its per-primitive rank convention. Absolute baseline and shifted regulator: MB and RC. No input is an assumed full QQ rectangular-current theorem.
