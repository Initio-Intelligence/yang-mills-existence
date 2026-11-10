# Density lifts, common smooth normalization, and deterministic propagation

**Current status:** A8 supplies the actual regular class. T9-G records the now-admitted one-source smooth normalization theorem in all 21 channels. N9/P9 supply the original-kernel bounded-seed phase estimate. The stronger point endpoint and mixed-history hierarchy are not inferred from either theorem.

**Status:** The deterministic regular bulk step now has an explicitly constructed marked marginal kernel with exact row balance and a proved localized first physical moment. The intrinsic admitted class from Gate 1 supports common smooth-source normalization with full remainder feedback. The joint-source finite-jet extension below retains the required \(O(g^2)\) marginal size, and arbitrary-profile bulk propagators have only polynomial growth in inverse-coupling ratios. Actual historical-kernel identification remains A7.58. The original point-source and all-history normalization gates are not declared complete. A separately analyzed translation-mixture kernel has an exact source-gradient quotient, but creates a nonlocal absolute conditional-covariance defect and does not close S2.

### 1. Which normalization is being constructed

Use the fixed 21-dimensional space \(E\) of curvature-bilinear fields for one compact simple gauge group. The identity field is tracked separately. A source coefficient is a column vector in \(E\); a field family is a linear map from \(E\) to scalar observables. Matrix order below follows this convention.

Fix the deterministic regular bulk map \(\mathcal T_k^{\mathrm b}\), with its unmarked couplings, averaging map, minimizing maps, and cutoff frozen. It is the normalized source map of the admitted full-torus small-field model, or its infinite-volume local-kernel limit. It does not include a chosen large-field history. The source makes a precise covariance split: sufficiently old R terms are absorbed into the regular E action once their partition is finer than the current blocking lattice; recent R terms and boundary terms are retained separately in the normalized interpolation (CMP119, pp.270–271, (3.26)–(3.27)). An augmented E reference may include those old terms **once its required analytic-norm bounds are verified**. Covariance restoration alone does not enlarge a birth domain whose radius depends on the coupling, as in (2.28). Until that norm comparison is supplied, the theorem uses the matched regular E reference, and every unverified R change remains a forcing term. In either case the full actual map is compared with one fixed deterministic reference; it does not receive a separate normalization.

The bulk map is covariant under compatible translations:

\[
\mathcal T_k^{\mathrm b}\tau_{Lm}
 =\tau_m\mathcal T_k^{\mathrm b},\qquad m\in\mathbb Z^4.
\tag{N7.1}
\]

This follows directly by changing the integration variables in the frozen regular integral: the averaging paths, the regular cutoff, and the action transform together. The small-field source assumes the current-lattice Euclidean invariance of its effective action and verifies preservation by the next integral; see CMP109, pp.263–264 and p.269, especially (2.17). This is a statement about the complete bulk integral. A localizing partition used to estimate that integral does not change it.

One must not replace (N7.1) by covariance that also changes an arbitrary fixed nonconstant background or a geometrical history. Such covariance does not make a row sum constant with that background or history held fixed. CMP119 distinguishes the complete regular E density, (2.29), (3.39)–(3.42), from the more restricted partition covariance of the R terms, (2.32)–(2.33).

All exact marginal identities below use a bulk realization with the matched curvature projection of JA1–JA7. An infinite-volume quantum kernel is not inferred merely from a volume-uniform analytic bound. If it is constructed as a limit of periodic kernels, one must also verify the local compatibility of the rooted coefficients and their wrapping-tail comparison: a local coefficient could otherwise contain an uncontrolled volume-dependent scalar. On periodic tori, affine curvature tests require the finite-volume comparison from JA8–JA9 and CC59/CP28. Those errors are carried as forcing; no continuous affine flux family is imposed on a torus. The algebraic row and moment arguments remain valid for any admitted matched bulk realization; existence and volume comparison of that realization remain part of the regular-class/source verification.

### 2. Extract the kernel from the actual frozen insertion

Choose translated fixed-support seed maps

\[
q_x:E\longrightarrow\mathscr F_k,
\qquad q_x=\tau_xq_0,
\qquad q_x(1)=0,
\qquad \Pi q_x=I_E.
\tag{N7.2}
\]

Here \(\Pi\) is the full 21-component curvature-quadratic jet in current units. The Wilson/clover basis is made to satisfy (N7.2) by one fixed finite basis change, determined by its nondegenerate classical curvature Hessian. This is part of choosing the field basis, not a scale- or history-dependent change of the observable.

For a scalar observable, \(\Pi\) is obtained by applying the Hessian at the trivial connection to two affine constant-curvature test directions, using cutoff affine fields and the convergent spatial-moment limit. Constants are killed by \(\Pi\). For invariant localized functions, \(\Pi\) is unchanged by moving the test origin: the difference of the two affine fields is a constant one-form, hence a local linearized gauge direction; the Ward identity annihilates it in the Hessian. These are the conventions proved in the source-jet analysis JA1–JA9.

Define the exact engineering-rescaled one-step field family

\[
\Phi_{k,x}(v;V)
  =L^4\mathcal T_k^{\mathrm b}(q_xv)(V),
\qquad
c_k(x)v=\Phi_{k,x}(v;1),
\qquad
a_k(x)v=\Pi\Phi_{k,x}(v).
\tag{N7.3}
\]

The factor \(L^4\) compares dimension-four densities. The normalized integral is the actual frozen one. Equivalently, \(\mathcal T_k^{\mathrm b}(q_xv)\) is the derivative at zero of the logarithm with \(tq_xv\) inserted into the integrand. No coupling derivative or derivative of the physical blocking kernel is substituted for it.

Let

\[
p_L(z\mid x)=\prod_{\mu=1}^4
\left(1-\left|x_\mu/L-z_\mu\right|\right)_+.
\tag{N7.4}
\]

The following is an exact decomposition of the transported field:

\[
\boxed{
\Phi_{k,x}(v)
=c_k(x)v+
\sum_zp_L(z\mid x)q_z\bigl(a_k(x)v\bigr)
+r_{k,x}(v),
\qquad \Pi r_{k,x}=0.
}
\tag{N7.5}
\]

It is a definition of the remainder using the actual numerator and denominator. Its zero curvature jet follows from \(\sum_zp_L(z\mid x)=1\) and \(\Pi q_z=I_E\). The remainder is retained in every later statement. Since the hats involve a fixed number of coarse corners near \(x/L\), subtracting the displayed seeds preserves rooted exponential locality, with a fixed support cost. The full remainder is invariant whenever the actual transported field is invariant; no claim about invariant individual localizing activities is needed for this identity.

Define the actual one-step **marginal coefficient kernel** by

\[
\mathsf K_k(z,x)=p_L(z\mid x)a_k(x).
\tag{N7.6}
\]

This is a legitimate choice of the spatial representation of the projected coefficient. It is not a claim that the entire transported observable has kernel (N7.6): the exact additional term is \(r_{k,x}\) in (N7.5).

### 3. The marginal coefficient is \(I+O(g_k^2)\), including the old action scores

For the above fixed-support seeds, the real finite-jet argument J6–J18 applies to the frozen regular integral. Its amplitude interpolation keeps the actual cutoff and all old couplings fixed. At zero amplitude, the insertion is fluctuation-independent, and its first amplitude derivative is odd under the centered truncated Gaussian. Thus the first derivative of the normalized expectation vanishes exactly.

The second amplitude derivative contains the insertion derivative, both covariance terms, and the connected three-score term in J11. The weighted covariance and fixed-order cumulant bounds sum the score locations. With two background derivatives, this gives the curvature-Hessian estimate J15. Classical affine reproduction JA7 gives the identity coefficient at zero amplitude. Consequently

\[
\boxed{
\sup_x\|a_k(x)-I_E\|\le C_q g_k^2.
}
\tag{N7.7}
\]

The constants are uniform in the root phase, microscopic depth, and bulk volume within the previously stated source class. A period cell contains only the fixed number \(L^4\) of phases. Fixed polynomial spatial moments used by \(\Pi\) are paid by the rooted localization reserve.

More generally, if \(f_x\) is an admitted localized input with \(\Pi f_x=0\), then

\[
\|\Pi(L^4\mathcal T_k^{\mathrm b}f_x)\|
\le C g_k^2\|f_x\|_{\mathrm{input}}.
\tag{N7.8}
\]

This is the small reverse block. For a bounded family \(q_x+s_x\), with \(\Pi s_x=0\), the same proof gives (N7.7) with a factor \(1+\sup_x\|s_x\|\). It does not say that the required input norm is already preserved through arbitrary old histories. That preservation is exactly the unresolved Gate 1/3 interface.

The sharper order \(g_k^2\) is retained here. The complex rooted bound RX34 gives a useful full-norm perturbation of order \(g_kr_{\chi,k}\), but using that weaker size for the common marginal product would not in general give the fixed logarithmic power needed for the stated pointwise S2 target. The finite-jet argument is what supplies the logarithmic marginal normalization.

### 4. Exact row balance and localized first moments are now verified for (N7.6)

Covariance (N7.1), seed covariance, and the translation-invariance of the full curvature projection imply

\[
a_k(x+Lm)=a_k(x).
\tag{N7.9}
\]

This does not make \(a_k(x)\) independent of its phase modulo \(L\).

For each residue \(r\in\{0,\ldots,L-1\}^4\), the hats satisfy

\[
\sum_{n\in\mathbb Z^4}p_L(z\mid Ln+r)=1.
\tag{N7.10}
\]

In one coordinate, the two possible nonzero contributions have weights \(r/L\) and \(1-r/L\); for \(r=0\), only the unit contribution remains. Multiplication proves the four-dimensional identity.

It follows that the row matrix is exactly

\[
\boxed{
M_k:=L^{-4}\sum_x\mathsf K_k(z,x)
=L^{-4}\sum_{r\in\{0,\ldots,L-1\}^4}a_k(r),
\qquad \|M_k-I_E\|\le C_qg_k^2.
}
\tag{N7.11}
\]

It is independent of \(z\), and is a single deterministic matrix on the fixed bulk trajectory. Define

\[
\mathsf E_k(z,x)
=\mathsf K_k(z,x)-p_L(z\mid x)M_k.
\tag{N7.12}
\]

The row sum is zero. On the support of \(p_L\),
\(|h_kx-h_{k+1}z|_1\le4Lh_k\). Moreover \(\|a_k(x)-M_k\|\le2C_qg_k^2\). Therefore

\[
\boxed{
L^{-4}\sum_x\|\mathsf E_k(z,x)\|
 |h_kx-h_{k+1}z|_1
 (1+|h_kx-h_{k+1}z|_1)^N
\le C_{N,L,\ell_0}g_k^2h_k
}
\tag{N7.13}
\]

for every fixed \(N\), uniformly when \(h_k\le\ell_0\). Thus both SP42 and SP55 are verified for the actual projected one-step kernel (N7.6), rather than postulated.

For its source-coefficient action

\[
(\mathsf S_k\phi)(z)
=L^{-4}\sum_x\mathsf K_k(z,x)\phi(h_kx),
\tag{N7.14}
\]

the exact cancellation gives

\[
\mathsf S_k\phi-M_k\mathsf Q_k\phi
=L^{-4}\sum_x\mathsf E_k(z,x)
 [\phi(h_kx)-\phi(h_{k+1}z)],
\tag{N7.15}
\]

and hence the one-step error is at most \(Cg_k^2h_k\operatorname{Lip}\phi\), including fixed Schwartz weights.

**Completed scope.** This is an actual regular bulk one-step marginal theorem for fixed current-scale analytic inputs. In particular, the missing first-moment estimate is not a separate unknown for this projected step. Iterating only (N7.6) would still discard the exact remainders in (N7.5). The next section retains them.

### 5. An exact density lift that keeps the irrelevant remainder

The argument in this section is an operator theorem. Its hypotheses are precisely the closed-class estimates being sought in Gate 1; it does not assume a marked kernel after the fact.

Let \(\mathscr B_{k,x}\) be a rooted analytic class of invariant fields, modulo one deterministic scalar identity, with bounded projection \(\Pi\), a translated local embedding \(\iota_x:E\to\mathscr B_{k,x}\), and a stable subspace \(\mathscr R_{k,x}=\ker\Pi\). Require a common input/output norm with positive regenerated localization reserve. The scalar terms are recorded independently throughout; no history-dependent scalar is removed.

For a rooted family \(f_x=\iota_xm_x+r_x\), apply the exact frozen map to each field. Write

\[
\widehat{\mathcal T}_kf_x
=\sigma_x+
\sum_{z'}p_L(z'\mid x)\iota_{z'}a_x
+\rho_x,
\quad a_x=\Pi\widehat{\mathcal T}_kf_x,
\quad \Pi\rho_x=0.
\tag{N7.16}
\]

Here \(\widehat{\mathcal T}_k=L^4\mathcal T_k^{\mathrm b}\). Define the density pushforward

\[
(\mathscr L_kf)_z
=L^{-4}\sum_xp_L(z\mid x)
\bigl(\iota_za_x+\rho_x\bigr).
\tag{N7.17}
\]

The remainder \(\rho_x\), originally rooted within a fixed distance of \(x/L\), is also a valid field rooted at every \(z\) with \(p_L(z\mid x)\ne0\). Reanchoring costs only a fixed norm factor. Summing (N7.17) gives the exact field identity

\[
\sum_z(\mathscr L_kf)_z
=L^{-4}\sum_x
\left(\widehat{\mathcal T}_kf_x-\sigma_x\right).
\tag{N7.18}
\]

For dimension four in four spatial dimensions, the density-volume factor \(L^{-4}\) cancels the engineering factor in the physical smeared observable. Thus (N7.18), with its separately retained identity term, is the actual frozen transport of the source sum.

Assume the closed-class estimates imply the following block bounds for (N7.17), in the supremum over roots of the same rooted norm:

\[
\|A_k-\mathsf Q_k\|\le a t_k,
\quad \|B_k\|\le b t_k,
\quad \|C_k\|\le c,
\quad \|D_k\|\le q<1,
\qquad t_k=g_k^2.
\tag{N7.19}
\]

The first two bounds follow from the finite-jet estimates and the hat probability average once the common class is available. The last two require the actual strong irrelevant contraction and the bounded marginal-to-remainder map in that class. A fixed block of scales may be used to make \(q<1\); every occurrence of \(L\) then denotes that fixed block ratio. None of these constants may depend on the ultraviolet depth or on the source.

On translated uniform densities, \(\mathsf Q_k=I\), and (N7.19) is exactly the CV block system. Starting from the actual microscopic density \(f_{0,x}=q_x\), its bounded stable graph gives translated linear families

\[
f_{k,x}=\iota_x+S_{k,x},\qquad
\Pi S_{k,x}=0,\qquad \sup_{k,x}\|S_{k,x}\|\le K_S,
\tag{N7.20}
\]

and matrices

\[
\boxed{
\mathscr L_k(f_kv)=f_{k+1}E_kv,
\qquad E_k=A_k^{\rm unif}+B_k^{\rm unif}S_k,
\qquad \|E_k-I\|\le C_Et_k.
}
\tag{N7.21}
\]

This is an identity of the chosen localized density representation, and therefore of its summed physical insertion. It includes the feedback of every previously generated regular irrelevant term through \(B_kS_k\).

Put

\[
P_{j,k}=E_{k-1}\cdots E_j,
\qquad Z_K=P_{0,K}^{-1}.
\tag{N7.22}
\]

Then the uniform-source microscopic family, multiplied once on the right by \(Z_K\), has exact current marginal coefficient \(P_{k,K}^{-1}\). Use the explicit two-sided AF spacing

\[
0<c_-\le x_j-x_{j+1}\le c_+,
\qquad x_j=g_j^{-2},\qquad x_K\ge x_*>0.
\tag{N7.22a}
\]

The lower increment controls ordered products, while the upper increment will control the ratio over a fixed number of scale steps in (N7.33). Under (N7.22a),

\[
\|P_{k,K}^{-1}\|
\le C\left(\frac{x_k}{x_K}\right)^s,
\qquad x_k=g_k^{-2},
\tag{N7.23}
\]

with one fixed exponent. This retains the logarithmic normalization required by S2. It does not use the weaker fixed-engineering-loss option in SP54e–SP54g.

### 6. Smooth-source transport with all regular remainders retained

The same lifted density construction handles nonconstant sources without demanding that their projected coefficients form a closed 21-component kernel.

For the uniform seed family in (N7.20), define the exact Banach-valued kernel

\[
\mathcal H_k(z,x)v
=p_L(z\mid x)
\bigl(\iota_za_{k,x}v+\rho_{k,x}v\bigr),
\tag{N7.24}
\]

where \(a_{k,x},\rho_{k,x}\) come from transporting \(f_{k,x}\) in (N7.16). Equation (N7.21) gives the exact row identity

\[
L^{-4}\sum_x\mathcal H_k(z,x)
=f_{k+1,z}E_k.
\tag{N7.25}
\]

The rooted norm of each bracket in (N7.24) is uniformly bounded by the closed-class assumptions and \(K_S\). Its source-position support satisfies \(|x-Lz|_1\le4L\), even though the field itself has an exponentially localized tail. Define

\[
\mathcal E_k(z,x)
=\mathcal H_k(z,x)-p_L(z\mid x)f_{k+1,z}E_k.
\tag{N7.26}
\]

Its row sum is zero. Consequently the exact one-step comparison with the bulk lift obeys

\[
\boxed{
\left\|
\mathscr L_k\bigl(f_k\phi\bigr)
-f_{k+1}E_k\mathsf Q_k\phi
\right\|_{\infty,\mathscr B}
\le C h_k\operatorname{Lip}_{h_k}\phi.
}
\tag{N7.27}
\]

All terms in (N7.16) are included. The bound is generally \(O(h_k)\), not \(O(g_k^2h_k)\): a marginal seed may create an order-one classical irrelevant lattice remainder whose phase dependence contributes to (N7.26). The physical mesh factor is enough for the following iteration.

#### A small growth exponent for the full family operator

From (N7.19), give a field family the norm

\[
\|(m,r)\|_\delta
=\sup_x\|m_x\|+\delta\sup_x\|r_x\|,
\qquad \delta>0.
\tag{N7.28}
\]

Then

\[
\|\mathscr L_k\|_\delta
\le\max\{1+a t_k+\delta c,\ q+b t_k/\delta\}.
\tag{N7.29}
\]

Choose any fixed \(0<\varepsilon<\log L\). Choose \(\delta\) so that \(\delta c\le\varepsilon/2\), and then one weak-coupling threshold so that \(q+b t_*/\delta\le1\). It follows that

\[
\|\mathscr L_{j+1,k}\|_\delta
\le C e^{\varepsilon(k-j)}
\left(\frac{x_j}{x_k}\right)^p.
\tag{N7.30}
\]

This does not require an \(O(g_k^2)\) estimate for the entire analytic operator or an assumed gradient bound on the actual evolved source. It uses the small reverse marginal block, the bounded forward stable block, and the strict stable contraction.

#### The exact ordered comparison

Let \(Q_{j,k}=\mathsf Q_{k-1}\cdots\mathsf Q_j\). For a fixed smooth source \(\phi_0(x)=\phi(h_0x)\), define

\[
v_j=P_{j,K}^{-1}Q_{0,j}\phi_0.
\tag{N7.31}
\]

Since scalar hats commute with channel matrices and \(E_jP_{j,K}^{-1}=P_{j+1,K}^{-1}\), the comparison fields satisfy
\(f_{j+1}v_{j+1}=f_{j+1}E_j\mathsf Q_jv_j\). Exact telescoping therefore gives

\[
\mathscr L_{0,k}(f_0Z_K\phi_0)-f_kv_k
=\sum_{j<k}\mathscr L_{j+1,k}
\left[\mathscr L_j(f_jv_j)-f_{j+1}E_j\mathsf Q_jv_j\right].
\tag{N7.32}
\]

The physical Lipschitz seminorm of \(Q_{0,j}\phi_0\) does not increase. Apply (N7.23), (N7.27), and (N7.30). With \(n=k-j\), the resulting sum is bounded by

\[
C\left(\frac{x_k}{x_K}\right)^s
h_k\operatorname{Lip}\phi
\sum_{n\ge1}
\left(\frac{e^\varepsilon}{L}\right)^n
\left(1+\frac{c_+n}{x_*}\right)^{p+s}.
\tag{N7.33}
\]

The series converges uniformly in the ultraviolet depth because \(e^\varepsilon<L\). Thus

\[
\boxed{
\left\|
\mathscr L_{0,k}(f_0Z_K\phi_0)
-f_kP_{k,K}^{-1}Q_{0,k}\phi_0
\right\|_\delta
\le C\left(\frac{x_k}{x_K}\right)^s
h_k\operatorname{Lip}\phi.
}
\tag{N7.34}
\]

The full transported regular **density family** has the corresponding rooted-family norm bound

\[
C\left(\frac{x_k}{x_K}\right)^s
\bigl(\|\phi\|_\infty+h_k\operatorname{Lip}\phi\bigr).
\tag{N7.35}
\]

This theorem retains all regular remainder feedback. Its common microscopic matrix is \(Z_K\) from (N7.22), independent of root, source, background, and geometrical history. Equation (N7.35) is not a bound on an unrestricted spatial sum: evaluating a physical smeared observable requires the weighted or physical \(L^1\) summation below, together with the restored field dimension at the chosen scale.

For a fixed Schwartz order, attach the weight \((1+|h_kx|)^N\) to the rooted family norm. Hat support gives per-step weight ratios \(1+O_N(h_k)\), whose products are bounded because \(\sum_jh_j<\infty\). The field-tail localization is already included in the rooted norm. The same proof gives (N7.34) with a fixed weighted gradient seminorm. For \(N>4\), the physical lattice sum \(h_k^4\sum_x(1+|h_kx|)^{-N}\) is bounded uniformly for \(h_k\le\ell_0\); this supplies the needed physical \(L^1\) step. Restoring a dimension-four density contributes its explicit \(h_k^{-4}\) factor. No claim of an all-order multiple-source estimate follows merely from this one-source argument.

**What this removes from the open list:** once the closed regular class and its block bounds are proved, a separate hypothesis that the full old mark is governed by a closed finite-dimensional spatial kernel is unnecessary for smooth sources. The exact Banach-valued density lift supplies the needed row identity, and its local source support supplies the physical first moment. The remaining proof is Gate 1's common class, followed by Gate 3's comparison with actual histories.

### 7. Identity terms and comparison with the actual history law

The scalars \(c_k(x)\) or \(\sigma_x\) above are computed in the deterministic bulk reference and retained as the identity component of the exact transport. Passing to a quotient by constants is only a way to compute the 21-channel matrix. It does not authorize replacing the original microscopic field by a differently centered field on each geometrical history.

In a fixed carrier, an expression that is constant with respect to the variables currently integrated may still be a nonconstant function of the exterior. Such a term is an actual old numerator or exterior conditional mean. It must remain in the marked source and in the law of total covariance/cumulance. The common microscopic vacuum subtraction, if used, is one deterministic subtraction for the original field family.

For a regular R perturbation on the same frozen kernel, the Gate 3 two-source argument gives an operator comparison of the form

\[
\|\mathcal T_{E+R}f-\mathcal T_Ef\|_{\rm rooted}
\le C\|R\|_{\rm potential}\|f\|_{\rm input}.
\tag{N7.36}
\]

Its exact derivative is the normalized covariance with the R insertion. Therefore a recent regular R coefficient can be treated as forcing relative to the single bulk cocycle, using its actual potential norm and the previously established weighted forced-cocycle estimates. Fresh reset activities have the stronger source suppression, whereas an accumulated recent R sum must first be bounded after transport. No instantaneous super-logarithmic bound on that complete sum is assumed. This statement requires the same frozen coordinates, minimizing map, and cutoff throughout the interpolation. It does not cover unresolved exterior large-field domains or silently replace a history-dependent kernel by the bulk one.

Write \(\epsilon_{R,j}=\|R_j^{\rm recent}\|_{\rm potential}\). A sufficient remaining-scale condition for the comparison is

\[
\sup_{k,K}\sum_{j<k}\epsilon_{R,j}
\left(\frac{x_j}{x_k}\right)^{p+s}<\infty,
\tag{N7.37}
\]

in the same rooted norm, with the required smallness when a perturbative graph is used. Fresh super-logarithmic bounds meet such fixed-exponent sums; the same conclusion for the accumulated recent R term requires its transported norm estimate. The source’s arbitrary large power in the R bound is also useful once its loss under the recent-scale sum has been recorded. Boundary terms and exterior conditional means still need Gate 3's joint-law estimate.

### 8. Why this still does not finish the point-source normalization

The kernel (N7.6) has column mass

\[
\sum_z\mathsf K_k(z,x)=a_k(x),
\tag{N7.38}
\]

which may depend on the blocking phase. Exact row balance in (N7.11) does not remove that dependence. The positive periodic phase example has precisely this structural form and shows that an \(O(g_k^2)\) phase mass can accumulate over the ultraviolet interval.

A smooth-source estimate such as (N7.34) cannot be applied to a point delta with a cutoff-independent Lipschitz seminorm. Doing so would introduce an inverse microscopic mesh factor and destroy the conclusion. Thus neither the new row theorem nor the lifted smooth-source theorem is a proof of the pointwise S2 norm.

There are two concrete pointwise targets left:

1. Prove that the **complete**, remainder-corrected point-source mass has a phase-independent quotient coordinate; or
2. Construct a bounded local corrector on that actual source class,
   \[
   \sum_zW_{k+1}(z)\mathsf K_k^{\rm eff}(z,x)
   =E_kW_k(x)+R_k^{\rm src}(x),
   \tag{N7.39}
   \]
   with the weighted residual sum and the original microscopic endpoint matching from SP30–SP37.

The effective kernel in (N7.39) must include the feedback of the stable field sector. It is not automatically (N7.6). The error in the endpoint conjugation must remain controlled for the full, possibly noncommuting 21-channel product.

A possible derivation is a local comparison between neighboring blocking origins, or an invariant source-gradient quotient for the actual normalized operation. Either must control the cutoff and normalization-score terms, not only the translation of the summed action. The present work identifies the necessary computation but does not claim that the corresponding Ward/intertwining estimate is available in the cited sources.

### 9. Status summary and source anchors

| Item | Status |
|---|---|
| Definition of the actual one-step marginal coefficient | Exact frozen-source identity in the stated matched bulk realization, N7.3–N7.6 |
| Marginal size \(I+O(g^2)\) | Derived from the previously proved finite-jet theorem and classical affine reproduction, N7.7–N7.8 |
| Deterministic bulk row matrix | Exact translation/residue calculation, N7.9–N7.11 |
| Localized first physical moment and fixed Schwartz moments | Proved for the actual projected kernel, N7.12–N7.15 |
| Full irrelevant feedback in a common uniform-source matrix | Exact density lift and CV graph on the admitted intrinsic bulk class, with its matched projection |
| Smooth-source iteration retaining all regular remainders | Proved operator theorem, N7.24–N7.35, under the explicit admitted bulk hypotheses |
| Joint \((U,J)\) finite-jet extension | N7.40–N7.44 prove the \(O(g^2)\) blocks using positivity only at the flat pair |
| Arbitrary-profile mature bulk propagation | Polynomial operator bound N7.45–N7.49; no source smoothness or exponential age loss |
| Narrow-chart regular forcing | Weighted age comparison N7.50–N7.51, using the actual potential norm and A7.58 identification |
| Common comparison with regular R changes | Same-frozen-carrier perturbation from Gate 3; history boundaries still separate |
| Pointwise common normalization | Open at N7.39 and its endpoint condition |
| Translation-mixture alternative | Exact positive marginal preservation and source-gradient quotient, N7.52–N7.55; the absolute covariance counterexample N7.57 blocks an S2 conclusion |
| All-history Gate 2 / S2 | Not completed by this module |
| Infinite-volume/periodic identification | Requires coefficient compatibility and the wrapping-tail comparison in the actual norm; not inferred from uniformity alone |

Primary source anchors:

- **CMP109 (1987), 249–301:** the small-field RG definitions (0.17)–(0.19); action covariance following (1.19), pp.263–264; Euclidean transformation of the fluctuation integral (2.17), p.269; source historical-coupling dependence following (0.22). [DOI](https://doi.org/10.1007/BF01215223).
- **CMP116 (1988), 1–22:** switched response (1.2)–(1.21), source-potential localization, and normalized rooted expansion used in RX18/RX34. [DOI](https://doi.org/10.1007/BF01239022).
- **CMP119 (1988), 243–285:** E-density covariance (2.29); restricted R covariance (2.32)–(2.33); full-lattice covariance and hats (3.39)–(3.42); rooted expectation expansion (3.44)–(3.47); curvature-jet projection (3.48)–(3.67).
- **Earlier labelled results:** J6–J18 and JA1–JA9 for the actual finite jets and affine comparison; CV1–CV21 for the bounded stable graph and ordered common normalization; RX18/RX34 and CC55/CP28 for the regular source norms; SP30–SP37 for the point-source corrector and endpoint obstruction.

These source clauses support the unmarked analytic and covariance inputs. The marked kernel construction and density-lift arguments above are deductions in this note, not observable theorems quoted as already proved in those papers.

### 10. Joint-source finite jets need positivity only at the flat pair

Gate 1's intrinsic source class consists of functions of the independent pair \((U,J)\), and its finite-volume projection may be defined using cutoff-affine connection tests with **independent current equal to zero**. This is not an instruction to identify those tests with physical-current tests in the cutoff annulus. It also does not require a weighted covariance theorem on every nonflat off-physical pair. The needed finite-jet estimate can be proved entirely under the flat real measure.

Let \(u=(u_1,u_2)\) parametrize two smooth cutoff-affine background connection directions based at the trivial pair, with independent \(J=0\). Use the fixed-cutoff amplitude interpolation of J6–J8, now with the joint insertion supplied by A7.13–A7.16:

\[
\begin{aligned}
\Psi(\tau,u)&=
\frac{\int_D F_{\tau,u}(A)e^{-H_{\tau,u}(A)}\,dA}
     {\int_D e^{-H_{\tau,u}(A)}\,dA},\\
F_{\tau,u}(A)&=f\bigl(\mathcal U_{\tau,u}(A),
                           \mathcal J_{\tau,u}(A)\bigr).
\end{aligned}
\tag{N7.40}
\]

Here the old couplings, integration domain, and physical forward kernel remain frozen. The analytic extension of the classical potential is chosen as its Taylor remainder after subtracting fluctuation degrees zero, one, and two on the entire source atlas. Thus the cubic vanishing used in \(\tau^{-2}W(U,J,\tau A)\) is an analytic identity. At an actual physical minimizing background and \(\tau=g_k\), the source KKT cancellation identifies this expression with the frozen physical kernel. This choice does not claim that a historical potential has a larger domain than its proved birth domain; the fixed-domain bulk admission from Gate 1 is still required.

The joint pair is independent of \(A\) at zero amplitude, and its first amplitude derivative is linear in \(A\). Consequently \(F_{0,u}\) is constant in \(A\), while \(\partial_\tau F_{0,u}\) is odd. The zero-amplitude Gaussian density is even, including for complex background parameters where its normalized integral is defined. Therefore the parity cancellation is an analytic identity:

\[
\partial_\tau\Psi(0,u)=0,
\qquad
\partial_{u_1}\partial_{u_2}\partial_\tau\Psi(0,0)=0.
\tag{N7.41}
\]

At each finite volume a neighborhood of \(u=0\) with nonzero Gaussian denominator exists. Its radius is not used for a uniform estimate of that denominator. Only derivatives at \(u=0\) are taken below.

Differentiate the exact second-amplitude formula J11 twice in \(u\), then set \(u=0\). For normalized cumulants the differentiation rule is

\[
\partial_{u_i}\kappa_n(X_1,\ldots,X_n)
=\sum_{a=1}^n\kappa_n(X_1,\ldots,\partial_{u_i}X_a,\ldots,X_n)
 -\kappa_{n+1}(X_1,\ldots,X_n,\partial_{u_i}H).
\tag{N7.42}
\]

Thus every resulting term is a cumulant of order at most five under the **flat** law with density proportional to \({\bf1}_D e^{-H_{\tau,0}}\). The HC-W and local-moment estimates of J6–J18 apply to this actual real law. No positivity assertion about \(H_{\tau,u}\) for nonzero independent background parameters enters the argument.

The differentiated insertions and scores have the required finite local polynomial bounds by directional Cauchy estimates in Gate 1's fixed source chart and its localized joint pair map. The Taylor-remainder identity makes the first two amplitude derivatives bounded by the same fixed powers of local fluctuation coordinates used in J16; it introduces no inverse running coupling. Affine directions introduce only fixed polynomial spatial moments. Smooth cutoff-affine directions have the same moment bound uniformly in their cutoff radius, and rooted exponential localization pays those moments. The fixed-order cumulant estimate J2–J4 therefore gives

\[
\sup_{|\tau|\le g_k}
\left|\partial_{u_1}\partial_{u_2}
             \partial_\tau^2\Psi(\tau,0)\right|
\le C\|f\|_{\mathrm{joint\ source}}.
\tag{N7.43}
\]

Integrating twice in amplitude and using (N7.41) proves

\[
\left\|\Pi\bigl(L^4\mathcal T_k^{\rm b}
                -L^4\mathcal T_{0,k}\bigr)f\right\|
\le Cg_k^2\|f\|_{\mathrm{joint\ source}}.
\tag{N7.44}
\]

Combined with Gate 1's exact classical filtration for the chosen matched projection, this establishes the \(O(g_k^2)\) marginal and reverse-block bounds for that joint source class. The complex full-norm perturbation remains of size \(O(g_kr_{\chi,k})\); the two estimates have different purposes. Finite-volume cutoff projection and infinite-volume translation-invariant projection must still be compared with their stated wrapping/local-compatibility errors when using the exact bulk row identity. This flat-parameter argument removes an unnecessary off-physical coercivity requirement, while leaving the actual historical-kernel identification and source-phase obligations explicit.

### 11. Arbitrary-profile mature bulk propagation has only polynomial growth

The smooth-source theorem in §6 uses a spatial first moment to pay an exponential-in-age bound. That argument alone must not be applied to an arbitrary newly born forcing profile. The block structure (N7.19), however, gives a stronger general propagator estimate. It requires no spatial smoothness.

For a sequence of full field families put \(m_k=\|\Pi f_k\|\) and \(r_k=\|(1-P_k)f_k\|\). The operator bounds imply

\[
m_{k+1}\le(1+a t_k)m_k+b t_kr_k,
\qquad
r_{k+1}\le c m_k+q r_k,
\quad t_k=x_k^{-1},\quad q<1.
\tag{N7.45}
\]

The norms may be suprema over all source positions; the hat average has norm one. The same argument applies to a single rooted source whenever the corresponding blocks satisfy (N7.19).

Choose a fixed \(\alpha>2b/(1-q)\) and set

\[
W_k=m_k+\alpha t_kr_k.
\tag{N7.46}
\]

The upper AF increment in (N7.22a) gives \(t_{k+1}/t_k\le1+C_+t_k\). For a sufficiently weak fixed endpoint, \(b+\alpha q(t_{k+1}/t_k)\le\alpha\). Inserting (N7.45) into (N7.46) therefore yields

\[
W_{k+1}\le(1+C_0t_k)W_k,
\qquad
W_k\le C\left(\frac{x_j}{x_k}\right)^{p_0}W_j.
\tag{N7.47}
\]

The second inequality uses the lower AF increment to sum \(t_k\). There is no loss of a fixed engineering exponent. One must not recover the stable norm by dividing the last inequality by \(t_k\). Instead use its exact geometric recursion:

\[
r_k\le q^{k-j}r_j+
c\sum_{\ell=j}^{k-1}q^{k-1-\ell}m_\ell
\le q^{k-j}r_j+
C\left(\frac{x_j}{x_k}\right)^{p_0}W_j.
\tag{N7.48}
\]

Since \(W_j\le C(m_j+r_j)\), this proves the full operator bound

\[
\boxed{
\|\mathscr L_{k-1}\cdots\mathscr L_j\|
\le C\left(\frac{x_j}{x_k}\right)^{p_0}.
}
\tag{N7.49}
\]

This estimate is valid for arbitrary spatial profiles in the admitted common class. It strengthens the general bound used to prove (N7.34). It does not provide a common point-source normalization by itself: that still requires matching the actual microscopic root family to a single ordered marginal product.

#### Consequence for the narrow-chart age comparison

Suppose Gate 1's exact narrow-chart decomposition is available, a forcing term born at step \(j+1\) has size at most \(C\epsilon_j A_j\), and its bulk radius maturation costs \(\Omega_{j+1}\le Cx_j^P\) for one fixed \(P\). Let the chosen normalized bulk reference obey \(B_k\le C(x_k/x_K)^s\). This reference bound must be supplied for the source under consideration; §6 supplies it for the stated smooth sources, not for an arbitrary point source.

Combining the radius ramp with (N7.49), and including any fixed additional radius cost in \(P\), gives the Volterra inequality

\[
\frac{A_k}{(x_k/x_K)^s}
\le C+
C\sum_{j<k}\epsilon_j\Omega_{j+1}
\left(\frac{x_j}{x_k}\right)^{p_0+s}
\frac{A_j}{(x_j/x_K)^s}.
\tag{N7.50}
\]

If \(\epsilon_j\le C_Qx_j^{-Q}\), with a freely selectable fixed \(Q>P+p_0+s+1\), the AF lower increment gives

\[
\sup_k\sum_{j<k}\epsilon_j\Omega_{j+1}
\left(\frac{x_j}{x_k}\right)^{p_0+s}
\le C x_*^{-(Q-P-1)}.
\tag{N7.51}
\]

Make the right side, including its fixed prefactor in (N7.50), smaller than one by the weak-coupling choice. Finite-step induction then gives \(A_k\le C'(x_k/x_K)^s\), with the same logarithmic exponent as the reference. An arbitrary forcing profile is allowed in this estimate. Its smallness pays a fixed polynomial maturity and propagation cost; no smoothness of that forcing was used. The actual-kernel decomposition, its narrow-chart potential norm, and the reference bound for the original microscopic source remain separate hypotheses. This supplies the precise mature-propagator interface needed in A7.55–A7.58 without assuming a uniformly bounded mature operator on every spatial profile.

### 12. A translation-mixture alternative and its exact limitation

This section studies a **new** source-independent positive kernel. It is not an identity for the original frozen kernel. It provides an exact source-gradient quotient, while an explicit counterexample shows why it cannot simply be substituted into the absolute S2 shell estimate.

#### 12.1 Positive marginal preservation

Let a probability law \(\mu\) on the old lattice be invariant under its unit translations. Let a stochastic kernel \(K_0(V\mid U)\) push it to \(\mu'\), and let \(Q_0\) denote its normalized backward observable map. Write \(T_r f(U)=f(\tau_{-r}U)\), and suppose the complete frozen map has the compatible covariance
\(Q_0T_{Le_i}=T'_{e_i}Q_0\).
Define

\[
\overline K(V\mid U)
=L^{-4}\sum_{r\in\{0,\ldots,L-1\}^4}
                 K_0(V\mid\tau_rU).
\tag{N7.52}
\]

Every summand is stochastic, so \(\overline K\) is positive and stochastic. Translation invariance of \(\mu\) gives \(\mu\overline K=\mu'\). Changing variables separately in its numerator gives the exact normalized backward map

\[
\overline Q f=L^{-4}\sum_r Q_0T_r f.
\tag{N7.53}
\]

Thus the one-step marginal column for translated seeds is the phase average \(L^{-4}\sum_r a_k(x+r)=M_k\). This calculation includes the actual normalization: all components have the same output marginal \(\mu'\).

#### 12.2 A source-gradient quotient survives full remainder feedback

There is a stronger telescoping identity. For each coordinate direction define
\(G_i=L^{-4}\sum_{r:r_i=0}Q_0T_r\). Then

\[
\boxed{
\overline Q(T_{e_i}-I)
   =(T'_{e_i}-I)G_i.
}
\tag{N7.54}
\]

To prove it, sum first over \(r_i\); the difference telescopes to
\(Q_0(T_{Le_i}-I)\), and compatible covariance moves that difference to the output lattice. Thus the space generated by local translation differences is preserved by the entire averaged operation. This includes all irrelevant-field feedback; no finite-dimensional closure of a projected kernel was assumed.

For a matched bulk projection satisfying \(\Pi(T_{e_i}-I)=0\), the full iterated marginal of translated microscopic seeds is therefore independent of their root. The translation-annihilating hypothesis holds for the local infinite-volume curvature projection with its proved moment limit. It does not hold exactly for an arbitrary fixed finite-torus cutoff-affine test. The A7 finite-volume projection must retain its annular and wrapping comparison error here.

The admitted norm estimates are compatible with the finite averaging in (N7.53). Each input shift is bounded by one blocking cell. Over a fixed block of \(N\) steps, every translation path moves the physical root by at most a constant times the output scale. Apply the polynomial-jet contraction to each shifted support using one common enlarged root collar, and average afterward. Convex averaging does not multiply the per-path constants. The classical stable block can therefore be made contracting by the same sufficiently large fixed \(N\); the quantum perturbation tends to zero with \(g r_\chi\), and the finite marginal jets remain \(O(g^2)\).

In this admitted bulk setting, apply the CV graph theorem to one point root. Identity (N7.54) makes its full marginal product the same for every translated point root. Their stable graphs remain uniformly bounded by the common contracting recursion. Consequently there is one ordered matrix \(\overline Z_K\), independent of the microscopic root, with

\[
\left\|
L^{4k}\overline Q_{k-1}\cdots\overline Q_0
          (q_x\overline Z_K)
\right\|_{k,\mathrm{root}}
\le C\left(\frac{x_k}{x_K}\right)^{\bar s}.
\tag{N7.55}
\]

This is a point-root bulk normalization theorem for the **averaged** kernels under the stated admitted-class and projection hypotheses. It does not establish that every final RT input marginal has the translation invariance required in (N7.52). Conditioning on a fixed historical partition can destroy that invariance. It also does not identify \(\overline Z_K\) with the matrix for the original kernel.

#### 12.3 The added phase covariance is a real obstruction for absolute S2

Let \(Q_r=Q_0T_r\), \(m_r(F)=Q_rF\), and
\(D_r(F,G)=Q_r(FG)-m_r(F)m_r(G)\). The conditional covariance of the averaged map is exactly

\[
\overline D(F,G)
=\mathbb E_r D_r(F,G)
 +\operatorname{Cov}_r\bigl(m_r(F),m_r(G)\bigr).
\tag{N7.56}
\]

The second term uses the same global random phase for both observables. Its absolute expectation need not decay with their separation.

For an explicit diagnostic, take independent symmetric variables \(X_z\in\{-1,1\}\) on a large periodic lattice. Let the original kernel be the identity and average it with its unit translate, each with probability \(1/2\). The original conditional covariance is zero. For coordinate observables at two sites whose translated pairs are disjoint, the new conditional covariance is

\[
\overline D(x,y)
=\frac14(X_x-X_{x+e})(X_y-X_{y+e}),
\qquad
\mathbb E|\overline D(x,y)|=\frac14.
\tag{N7.57}
\]

The value is independent of the distance between the pairs. The signed expectation is zero, but an absolute local shell envelope fails. This example already has a translation-invariant input law and an exactly marginal-preserving positive mixture. Those properties alone cannot preserve S2.

Therefore the mixture theorem is a concrete normalization strategy with a precisely identified additional requirement. Using it in the full construction would require either a proof controlling the global phase-covariance term, a different local phase randomization whose kernel retains the required source-gradient identity and locality, or a route based on signed distributional cancellations. The present absolute pointwise S2 proof does not acquire any of these conclusions from (N7.52)–(N7.55).

---
