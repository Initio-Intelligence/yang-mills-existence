# Exact first-step history averaging and a marked R-sector mass reserve

## Result and limits

This note establishes two actual-source facts, rather than assuming a marked conditional estimate.

* All first \(R\) histories can be summed **before normalization**, after their retained free variables have also been integrated. Their selectors then cancel exactly. The result is the original globally \(P/Q\)-regular first-step integral, with its remaining \(Q\) restriction, complete gauge/coarea density and normalizer. All finite marked source jets satisfy the same equality.
* Every nonempty actual first \(R\) pattern has a **joint-mass-weighted energy and marked-moment reserve** of size
  \[
  \exp\{-c\,n_{\rm bad}P^2+C\,n_{\rm bad}R_1^4\}.
  \]
  It is uniform in admitted first coarse fields and total volume. No rare branch mass or global clean-event probability is inverted. Since the source assumes \(p_0\ge5r\), the available rarity pays the full \(MR_1\)-region volume, shape entropy, and any fixed number of local scalar insertions; a fixed exponential energy reserve gives all orders at once.

At \(V_1=1\), the remaining \(Q\) restriction is a product of fixed one-slot cutoffs between radii \(P\) and \(3P\). The verified first-clean failed-cutoff expansion then proves a volume-uniform \(O(e^{-cP^2})\) difference between the actual \(R\)-averaged scalar and its all-\(R\)-good counterpart.

The mass reserve is **not** a proof that a branch mass, as a function of raw \(V_1\), has local support. The physical connected density-cluster and coarse-boundary-current steps remain distinguished below. In particular the hard moving \(Q\) boundary cannot be differentiated by pretending it is a holomorphic potential.

## 1. Exact source conventions

Use the original first ordinary step, before any large-field replacement or inherited effective activity. Fix \(\Omega_1\) to be the whole periodic lattice and let \(V=V_1\) be an admitted coarse field in this branch. Put
\[
 g=g_0,\qquad P=\delta_0/g_0=A_1(\log g_0^{-2})^{p_0}. \tag{AS.1}
\]
The source has \(p_0\ge5r\), \(r\ge2\), and \(R_1\) is a rounded \(L\)-power comparable to \((\log g_1^{-2})^r\). Fixed first-step coupling comparison therefore gives
\[
 R_1\le C_L(\log g_0^{-2})^r,\qquad
 P^2/R_1^4\longrightarrow\infty.                    \tag{AS.2}
\]

Undo the first exterior relocation (CMP119 (1.22)) with its actual inverse, Jacobian and marked pullback. Undo the *whole* conditional-integration equality (1.26)–(1.30) when reintroducing the already integrated free coordinates. The resulting common independent variables are the original \(A\) of (1.15), with exact reconstruction
\[
 U=\Phi_V(A).
\]
Its exceptional-bond correction solves the actual nonlinear group constraint. The ordinary block average is exactly \(V\).

After keeping all factors independent of \(A\) in \(C_0(V)\), the complete primitive density is
\[
 D_V(A)=\exp\{-\tfrac12 A^TK(V)A+W_V(A)\}.           \tag{AS.3}
\]
It contains Wilson, the source averaged soft gauge, Haar, coarea and the exceptional-coordinate determinant, each once. The current-dependent constraint Hessian belongs in \(K\). Because the source expands at its constrained critical point, there is **no residual classical \(g^{-1}J\cdot A\) force** in this common full first-fluctuation integral. Any perturbative linear Haar/coarea term remains in \(W_V\) and is included in its gradient bound.

The actual source \(R\) tests are the maxima of norms of the independent free coordinates on the prescribed enlarged starred cubes in (1.18). Write \(\mathscr R\) for a complete primitive pattern of bad test cubes, and \(E_{\mathscr R}(A)\) for the product of all of its good and bad alternatives. Thus
\[
 \sum_{\mathscr R}\mathbf1_{E_{\mathscr R}}(A)=1.     \tag{AS.4}
\]
This is the literal finite partition. Grouping several primitive patterns with the same derived geometry means summing their positive measures, not selecting one representative.

Let \(\chi_Q(A,V)\) be the actual remaining approximate-fluctuation selector from (1.8), before it is dropped on \(R\)-good cubes. Its defining tests omit the exceptional bonds, as stated in (1.9) and after (1.14). On this \(\Omega_1\)-full branch the initial microscopic plaquette and axial cutoffs are redundant once the approximate \(Q\) tests hold, by the paragraph after (1.10). Their exponential gauge density is still in (AS.3).

## 2. What summation cancels exactly

For fixed gauge-invariant microscopic marks \(F_1,\ldots,F_q\), define the unnormalized source integral
\[
 Z_{\mathscr R}(V;t)
 =\int \mathbf1_{E_{\mathscr R}}(A)\chi_Q(A,V)
       D_V(A)\exp\{\textstyle\sum_jt_jF_j(\Phi_V(A))\}\,dA.
                                                               \tag{AS.5}
\]
All coordinate maps, cutoffs, couplings, gauge weights and reference normalizers are specified at zero source.

Each source branch ordinarily integrates only the \(R\)-good free coordinates and retains the others. Integrating those retained coordinates against their **actual branch mass**, and undoing the exact source changes of variables, gives (AS.5). This follows from positive Fubini at zero source and ordinary finite-dimensional integration for source derivatives. The complete \(E/B\), vacuum and normalization factors in the source equality are kept, rather than identified termwise with independent Gaussian factors.

Consequently
\[
 \sum_{\mathscr R} Z_{\mathscr R}(V;t)
 =Z_Q(V;t):=\int\chi_Q(A,V)D_V(A)
             e^{\sum_jt_jF_j(\Phi_V(A))}\,dA.         \tag{AS.6}
\]
The actual \(R\)-averaged source generating function is
\[
 \overline G_R(V;t)=
 \frac{\sum_{\mathscr R}Z_{\mathscr R}(V;t)}
      {\sum_{\mathscr R}Z_{\mathscr R}(V;0)}
 =\frac{Z_Q(V;t)}{Z_Q(V;0)}.                         \tag{AS.7}
\]
This sums masses before division. An unweighted sum of separately normalized branch marks is not (AS.7). The factor \(C_0(V)\) cancels in this single conditional ratio; it remains in the actual coarse density \(C_0(V)Z_Q(V;0)\).

All finite source derivatives and logarithmic cumulant jets agree in (AS.6)–(AS.7). No source-dependent saddle or cutoff has been chosen.

The \(R\) partition alone removes **only** the \(R\) cutoffs. It does not remove \(\chi_Q\). If the complete initial \(P_0,P_1,Q_1\) decompositions and their normalized gauge insertions are also summed and all their retained microscopic fields integrated, their defining partitions of unity restore the original ordinary Wilson coarse integral,
\[
 C_{\rm bare}\int
 e^{-\beta_0S(U)}
 \delta_G(\mathcal M_0(U)V^{-1})
 e^{\sum_jt_jF_j(U)}\,dH(U),                         \tag{AS.8}
\]
with the original blocking map and Haar-normalized group delta. The inserted gauges fix coarse centers, so they preserve that readout; gauge-invariant marks preserve the gauge-disintegration identity. Equation (AS.8) is an exact measure identity. Its large-\(P/Q\) sectors are not quantitatively estimated merely by proving the \(R\)-only result below.

## 3. Source-verified comparison laws

The first-step primitive estimates, on any fixed enlargement \(bP\) of the original free-coordinate box, give
\[
 \lambda I\le K(V)\le K_*I,\qquad
 K(V)\ \hbox{has fixed range and bounded absolute rows},          \tag{AS.9}
\]
and
\[
 \sup_i\|\partial_iW_V\|_\infty\le\epsilon_1=CgP^2,\qquad
 \sup_i\sum_j e^{\nu d(i,j)}
       \|\partial_i\partial_jW_V\|_\infty
       \le\epsilon_2=CgP.                           \tag{AS.10}
\]
Harmless higher-order \(g^2P\) and \(g^2\) terms can be included. In particular \(\epsilon_1\le1\) and \(\epsilon_2\le\lambda/4\) at sufficiently small coupling.

These are actual native first-step estimates, not assumed marked output bounds. Their ingredients are the local \(C\) and nonlinear correction acting only at \(b_0(c)\), finite Wilson and averaged-gauge stencils, critical cancellation with the \(J\cdot D''\) term retained, and the finite local Haar/coarea logarithms. The positive Hessian and uniform local-gauge comparison are supplied by the first-step variational construction and the PG/LC estimates. They are uniform under block-adjoint gauge transformations and do not require a globally small-link coarse gauge. There are no inherited completed factors at this step.

For a product of source norm balls with individual radii \(P\) or \(3P\), use (AS.3) to define the **comparison law**
\[
 \mu_B(dA)=Z_B(V)^{-1}\mathbf1_B(A)D_V(A)\,dA.       \tag{AS.11}
\]
This is not declared to equal the actual moving \(Q\)-good domain. It is an auxiliary full-first-fluctuation law used to bound that domain. In particular it is not the generally forced conditional obtained after holding some \(R\)-bad coordinates fixed.

### Lemma AS.1 — centered product comparison reserve

There are fixed \(a_*>0,C,c>0\), uniform in \(B,V\) and volume, such that for every finite set \(D\) of coordinate blocks,
\[
 \log\mu_B e^{aE_D}\le Ca|D|,\qquad
 E_D=\sum_{i\in D}|A_i|_{\rm Eucl}^2,\quad
 0\le a\le a_*,                                    \tag{AS.12}
\]
and
\[
 \mu_B\{|A_i|_{\rm source}>P\}\le Ce^{-cP^2}.         \tag{AS.13}
\]

**Proof.** The core centered Gaussian on any such symmetric convex product has mean zero. Its precision, including an additional tilt \(-2aP_D\), retains a fixed positive gap if \(a_*\) is sufficiently small. The \(W_V\) interpolation changes each coordinate mean by at most \(C\epsilon_1\): differentiate its mean, use the force-uniform exponentially summable covariance bound from HC/RMg, and sum the bounded gradient in (AS.10). The same statement holds under the quadratic tilt because its gap and Hessian-row constants remain uniform. Further real linear tilts preserve strong convexity, hence centered sub-Gaussian coordinate moments.

It follows that \(\mu_{B,a}|A_i|^2\le C\) for every coordinate under the quadratic tilt. The derivative of the log moment generating function in (AS.12) is \(\mu_{B,a}E_D\le C|D|\). Integrate from zero. The sub-Gaussian coordinate tail, its \(O(\epsilon_1)\) mean, and fixed-dimensional norm equivalence give (AS.13). Convex barrier approximation justifies the covariance statements on the literal hard balls. Every normalization remains the exact one in (AS.11). ∎

### Lemma AS.2 — enlarging any finite set has a small normalization cost

Let \(B_D\) have radius \(3P\) at \(D\) and radius \(P\) elsewhere; let \(B_P\) have radius \(P\) everywhere. Then
\[
 1\le\frac{Z_{B_D}(V)}{Z_P(V)}
 \le\exp\{C|D|e^{-cP^2}\},\qquad
 Z_P(V)=\int_{B_P}D_V(A)dA.                         \tag{AS.14}
\]

**Proof.** Shrink one coordinate block at a time from \(3P\) to \(P\). Every intervening law is one of the product comparison laws in Lemma AS.1. The exact ratio of successive partition functions is its probability of \(|A_i|_{\rm source}\le P\), at least \(1-Ce^{-cP^2}\). Multiply these ratios, take logarithms, and use \(-\log(1-u)\le2u\) for small \(u\). There is no assumption that \(|D|e^{-cP^2}<1\), and no denominator involving the probability that the entire torus is good. ∎

## 4. The actual first R-pattern reserve

Let \(k=|\mathscr R|>0\) be the number of bad test cubes. Let \(D=D(\mathscr R)\) be the union of their actual enlarged starred free-coordinate footprints. Each coordinate belongs to at most a fixed number \(B_*\) of test footprints. This number depends on the fixed source enlargement convention, not on \(R_1\) or volume. Norm equivalence and the bad alternatives therefore imply
\[
 \mathbf1_{E_{\mathscr R}}\ne0
 \quad\Longrightarrow\quad E_D\ge c_*kP^2.          \tag{AS.15}
\]
Indeed, each bad test has a free coordinate of source norm at least \(P\), so its sum of squared Euclidean coordinates is at least a fixed multiple of \(P^2\). Sum over bad tests and use the bounded overlap.

The exact remaining \(Q\) condition on the independent, nonexceptional entries is bounded above by radius \(3P\) for all sufficiently small coupling. On good \(R\) entries the radius is \(P\) and the \(Q\) test is exactly redundant by (1.19). Thus the **whole actual pattern**, not merely a trial subset, is contained in \(B_D\). Keep its good tests and exact \(\chi_Q\) inside the numerator.

Define its relative joint mass with an energy tilt by
\[
 b_{\mathscr R}(V;a)
 =\frac{1}{Z_P(V)}
   \int\mathbf1_{E_{\mathscr R}}(A)\chi_Q(A,V)
        e^{aE_D}D_V(A)\,dA.                         \tag{AS.16}
\]

### Theorem AS.3 — actual first R mass and all energy moments

For fixed \(0\le a\le a_*/4\),
\[
 \boxed{\quad
 b_{\mathscr R}(V;a)
 \le\exp\{-c_1kP^2+C_1|D|\}.
 \quad}                                            \tag{AS.17}
\]
All constants are uniform in admitted native \(V\), \(\mathscr R\), volume and coupling once the stated source smallness holds.

**Proof.** Choose \(t=a_*/4\). On the event, (AS.15) gives
\[
 \mathbf1_{E_{\mathscr R}}e^{aE_D}
 \le e^{-tc_*kP^2}e^{(a+t)E_D}.
\]
Enlarge its support to \(B_D\), retain the same density, and bound \(0\le\chi_Q\le1\). Lemma AS.1 bounds the exponential moment by \(e^{C|D|}\), and Lemma AS.2 bounds the exact change of denominator from \(Z_{B_D}\) to \(Z_P\). This gives (AS.17). No rare-pattern denominator occurs. ∎

In particular, after keeping a fixed positive part of the same reserve,
\[
 \frac1{Z_P}\int\mathbf1_{E_{\mathscr R}}\chi_Q
       E_D^mD_V\,dA
 \le m!C^m e^{-c_2kP^2+C_1|D|},
 \qquad m=0,1,\ldots.                               \tag{AS.18}
\]
The energy in this statement is the actual free-coordinate quadratic reserve, including directions controlled by the soft gauge. It is not only the Wilson plaquette energy. Pure-gauge \(R\) births show why a Wilson-only implication in (AS.15) would be false.

## 5. Exact scalar marks use the same reserve

For the F01 primitive scalar
\[
 F_h(U)=\alpha\beta_0\sigma_h(U)-c,\qquad
 b=|\alpha|+h^4|c|,
\]
the exact Wilson trace formula and the admitted first regular chart give, on the entire encompassing \(3P\) product,
\[
 |F_h(\Phi_V(A))|\le C b h^{-4}P^2.                 \tag{AS.19}
\]
Here the minimizing field curvature is bounded by the source regularity ceiling, whose ratio to \(gP\) is fixed by \(A_0/A_1\) and fixed block constants. The fluctuation reconstruction changes each local plaquette by \(O(gP)\). Thus \(\beta_0s(U_p)\le CP^2\), since \(\beta_0g^2\) is fixed. The identity term is included in \(b\). This uses the actual scalar, not a new coarse observable.

On a nonempty \(R\) pattern, (AS.15) makes the right side of (AS.19) bounded by \(Cbh^{-4}E_D\). Therefore all marked moments are paid by **one** energy store. For marks \(F_\ell\) with budgets \(b_\ell\), and \(m,q\ge0\),
\[
 \boxed{\quad
 \frac1{Z_P}\int\mathbf1_{E_{\mathscr R}}\chi_Q
 E_D^m\prod_{\ell=1}^q|F_\ell(\Phi_V(A))|D_V\,dA
 \le (m+q)!C^{m+q}
      \left(\prod_{\ell=1}^q b_\ell h^{-4}\right)
      e^{-c_2kP^2+C_1|D|}.
 \quad}                                            \tag{AS.20}
\]
The \(q=0\) convention is understood. The proof is the pointwise bound just described followed by (AS.18) at order \(m+q\). This does not independently spend the same rarity factor for each mark.

Equivalently, on a fixed \(\ell^1\) source ball
\(\sum_\ell|t_\ell|b_\ell h^{-4}\le\rho_*\), the actual unnormalized marked numerator retains
\[
 \left|Z_P^{-1}\int
  \mathbf1_{E_{\mathscr R}}\chi_Q
  e^{aE_D+\sum_\ell t_\ell F_\ell}D_V\,dA\right|
 \le e^{-c_3kP^2+C_1|D|}.                           \tag{AS.21}
\]
The maps and selectors are unchanged. This is an actual fixed source radius for a *rare joint mass*, not a claimed source radius for its separately normalized conditional law.

## 6. Full footprint and shape costs are paid

Let \(Y_{\mathscr R}\) include the true test footprints, the \(MR_1\) covering, the source padding, and the permitted small-component rectangular hull. Each primitive test has size \(O(R_1)\) in current units. Fixed \(L,M,M_2\), padding widths and the \(100MR_1\) small-component rule imply
\[
 |D|+|Y_{\mathscr R}|
 \le C_{\rm geom}kR_1^4.                            \tag{AS.22}
\]
For components too large to be hulled, the padded union has this bound directly. For each component that is hulled, its diameter is at most a fixed number of covering cells and it contains at least one bad test, giving the same bound with a larger fixed constant. If several such hulls touch, their union satisfies the sum bound; no inverse-dilation identity is needed.

For a connected \(Y_{\mathscr R}\), its unit-block tree length is bounded by a fixed multiple of its volume. Hence for any fixed \(\kappa>0\), (AS.2),(AS.17) give, at sufficiently weak coupling,
\[
 e^{\kappa(|Y_{\mathscr R}|+t(Y_{\mathscr R}))}
 b_{\mathscr R}(V;a)
 \le e^{-c_4kP^2}.                                 \tag{AS.23}
\]
Fixed algebraic rank and coordinate factors are paid in the same way.

The \(MR_1\) covering grid contains only a fixed number of primitive test cubes per cell, independent of \(R_1\). Connected padded/hulled patterns can be encoded by connected animals on a fixed finite-range enlargement of that grid, together with a fixed finite collection of within-cell choices. Their rooted count at \(k\) bad tests is therefore at most \(C_{\rm geom}^k\), after enlarging the fixed connection range to cover the small hull rule. If an anchor lies in a hull, some original bad cell is within a fixed number of covering cells, which only changes the constant.

Consequently the **geometric joint-mass ledger** for connected patterns anchored at \(x\) obeys
\[
 \sum_{\substack{\mathscr R\ne\varnothing,\ Y_{\mathscr R}\ {\rm connected}\\
                  x\in Y_{\mathscr R}}}
 e^{\kappa(|Y_{\mathscr R}|+t(Y_{\mathscr R}))}
 b_{\mathscr R}(V;a)
 \le C e^{-c_5P^2}.                                \tag{AS.24}
\]
The same sum with the marked integrals in (AS.20) has its displayed factorial/budget factor. Marks whose stencils lie in a fixed enlargement of \(Y_{\mathscr R}\) add only fixed footprint costs.

This is an actual full-footprint *mass* estimate. It does not assign a local raw-\(V\) cylinder support to \(b_{\mathscr R}(V)\). A mark arbitrarily far from the bad region also needs a connected root-to-defect estimate before its connector can be charged; its disconnected product with a vacuum rare event must not be called a connected kernel.

## 7. The baseline is part of the actual law

At zero source the all-\(R\)-good numerator is exactly \(Z_P(V)\), because \(\chi_Q=1\) on that domain. Restore the retained-only factor and the normalized microscopic Wilson measure:
\[
 d\nu_P(V)=C_0(V)Z_P(V)\,dH(V).                      \tag{AS.25}
\]
This is the actual all-first-\(P/Q/R\)-good submeasure, with its original coarse selectors and global normalization; its mass is at most one. It is not reset to a probability measure.

The full globally \(P/Q\)-regular coarse contribution is exactly
\[
 d\nu_P(V)\sum_{\mathscr R}b_{\mathscr R}(V;0).
                                                               \tag{AS.26}
\]
Thus integrating (AS.20),(AS.23),(AS.24) against \(\nu_P\) yields actual original-law joint-mass bounds with the same constants. No factor inverse to the probability of a clean torus appears. The common \(Z_P\) is kept exactly once in the outer measure, as required by the RB/FR analysis.

## 8. A concrete actual flat R-averaged scalar consequence

At \(V=1\), both the global minimizing field and every local reference in the \(Q\) tests are identity. The constraint correction changes only exceptional bonds, which the tests omit. All repeated starred tests therefore reduce to a product
\[
 \chi_Q(A,1)=\prod_i\rho_g(A_i),                     \tag{AS.27}
\]
where each one-slot cutoff is independent of all retained variables,
\[
 0\le\rho_g\le1,\qquad
 \rho_g=1\text{ on }|A_i|_{\rm source}\le P,\qquad
 \rho_g=0\text{ outside }|A_i|_{\rm source}<3P.        \tag{AS.28}
\]
For an operator-norm convention its exact radius is \(2g^{-1}\arcsin(\delta_0)\). The argument only needs (AS.28), so no special norm identity or convexity of the group-distance sublevel set is assumed.

### Lemma AS.4 — fixed-cutoff replacement with a marked root

In the verified native first-clean Gaussian/Mayer construction, replace every product cutoff \(\mathbf1_{|A_i|\le P}\) by any fixed measurable \(\rho_i\) satisfying (AS.28), keeping the original density, reconstruction and source. On the fixed enlargement \(3P\), the primitive analytic budgets still tend to zero. The normalized marked source-log difference admits the same connected physical localization, and each difference term has a failed-cutoff factor. For the scalar root its sum costs
\[
 C b h^{-4}e^{-cP^2},                               \tag{AS.29}
\]
with constants independent of total volume.

**Proof.** Interpolate each product factor between the two cutoffs, or take their exact finite product difference before expanding. Every differentiated/difference factor is supported at \(|A_i|>P\) and has magnitude at most a fixed constant. Include that coordinate in the actual Gaussian marginal's initial support. The exact complex marginal majorant GM.18–GM.21 bounds it by
\(\exp(-aP^2)\exp(a|A_i|^2)\), using a fixed part of the positive Gaussian reserve. The determinant loss is only proportional to the localized rank.

The higher Wilson, gauge, Haar and coarea vertices have the same primitive analytic/carrier estimates on \(3P\), with only fixed factors such as \(3^3\) in the vanishing \(gP^3\) budget. The LC scalar source has its original linear/quadratic reserve and trace bound. The Mayer expansion, Gaussian-marginal localization and connected logarithm therefore apply with the same strict margins. Each surviving difference in the source-containing logarithm contains both a marked root and at least one cutoff difference. Disconnected vacuum factors cancel in this logarithmic difference, rather than being bounded by a global ratio of partition functions. The rooted connected sums retain a fixed fraction of the failed-cutoff exponential. Source Cauchy gives (AS.29), including exact tagged coefficients. This is precisely the LC.5/GM.4 mechanism with a different bounded one-slot cutoff factor; it does not alter the Gaussian baseline or saddle. ∎

At the single actual retained value \(V=1\), (AS.27) identifies this fixed-cutoff law with the exact \(R\)-averaged source law. Consequently
\[
 \left|\,\overline Q_R F_h(1)-Q_{\rm all\ R\ good}F_h(1)\,\right|
 \le C b h^{-4}e^{-cP^2}.                            \tag{AS.30}
\]
The same argument applies to every finite marked source jet, with its factorial/source budget. Combining with the proved first-clean block-averaged scalar coefficient gives
\[
 (Lh)^4\overline Q_R\overline F_h(B;1)
 =\alpha\sqrt{\frac32}(L^4-1)(N_c^2-1)-(Lh)^4c
 +O\!\left(L^4|\alpha|
       [gP^3+g^2P^2+e^{-cP^2}]\right),              \tag{AS.31}
\]
where \(N_c\) is the color rank, and the block average respects the fixed blocking convention.

For nonflat \(V\), the actual \(Q\) tests involve different local references and their intersections. The fixed \(\rho_i\) comparison law supplies a useful supported continuation but is not automatically the actual moving-cutoff conditional. Its coarse currents cannot be identified with actual \(Q\)-boundary currents by (AS.30).

## 9. Current records and the remaining connected-density obligation

At fixed source labels \(g,P,R_1\), the exact \(R\) alternatives in the original free \(A\) variables do not move when \(V\) varies. They generate **no moving R-boundary term** in that filing.

Differentiating the primitive density instead produces the actual score
\[
 S_d(A,V)=-\tfrac12 A^T(D_dK)A+D_dW,
                                                               \tag{AS.32}
\]
including the complete coarea contribution. Differentiating a relative mass also subtracts the derivative of the same all-\(P\) denominator. If a localized score coefficient or marked pullback has an actual polynomial energy bound on a genuine carrier, (AS.18)–(AS.20) pay that insertion while retaining a fixed rarity fraction. Source locality of that coefficient is still required; it does not follow merely because its integral is small.

There are two distinct remaining boundary pieces. First, \(\chi_Q(A,V)\) moves; its finite variation or surface current is not controlled by a probability mass estimate alone. Second, the outer coarse \(P\) selectors remain in \(C_0(V)\). Summing their complete complementary sectors cancels them algebraically as in (AS.8), but estimating that sum requires the corresponding actual density response and source geometry.

Finally, (AS.24) gives the absolute budget for labeled joint-measure atoms with their full seed-region costs. It is not yet a decomposition of the mass as a local function of raw retained fields. A connected density-cluster certificate must still:

* identify each primitive factor's actual raw dependency carrier, including reconstruction and reference maps;
* cancel disconnected vacuum contributions before normalizing;
* attach a separated scalar root to the relevant rare component with a true supported connector;
* retain every density/current/source-jet record and the same outer normalization.

The first-clean marginal construction supplies the Gaussian part of this mechanism. Its extension to local rare defects and the remaining moving \(Q/P\) boundaries is a concrete analytic task. The proved mass reserve shows that true \(MR_1\)-footprint and rank costs are affordable; it does not replace that task by a support label.

## Mathematical sources

Primary source: CMP119, pp.245–254, (1.1), (1.4)–(1.22), (1.26)–(1.30); the first \(p_0\ge5r\) hierarchy is printed on p.246. The original ordinary coarse map and delta are in (0.1).

Companion proofs used here:

* M04_First_Birth_Reassembly.md, FR.1–FR.9: exact undoing and common first coordinates.
* first_birth_relative_weights.md, RB.1–RB.15: actual starred \(Q\) support, common \(Z_P\), and the whole-event rather than trial-box interpretation.
* first_step_precision_gap.md and local_extension_kernel.md: constrained first precision, current Hessian and primitive native maps.
* M04_Local_Mask_Scalar_Response.md and first_step_relative_marginal.md: complete first-potential derivative rows, force-uniform convex covariance and local means on product cutoffs.
* ambient_gaussian_marginal.md, GM.18–GM.21 and GM.4; local_coupling_source.md, LC.5–LC.6 and LC.58–LC.59: exact localized Gaussian reserve, marked source, failed-cutoff connected sums and first scalar coefficient.

The new source-specific deductions are the uniform arbitrary-size normalization comparison (AS.14), the complete actual pattern reserve (AS.17)–(AS.21), its full-footprint joint-mass summation, and the exact \(R\)-averaged flat scalar consequence.
