# Localizing the actual moving Q cutoff after first-step R averaging


## 1. Purpose, exact operation, and scope

The actual first regular R-history average has a remaining Q cutoff whose center depends on the retained coarse field. A sharp indicator is not a holomorphic function of that field or of a localization parameter. The construction below localizes its **integral**, using a local compact frame and the boundary of a complex integration chain. Each resulting defect remains at a large fluctuation, so that its Gaussian tail pays the full raw spatial support of the Q reference.

Keep the original first Wilson step, with no inherited effective activities, and fix the globally P/Q-regular branch \(\Omega _1\) equal to the periodic lattice. Write \(g=g_0\), \(P=\delta _0/g_0\), and let \(R_1\) be the literal source geometric scale. All source parameters and cutoffs are specified at zero physical source. The source assumption \(p_0\ge5r\) implies

\[
 P\longrightarrow\infty,\quad gP^jR_1^k\longrightarrow0
 \text{ for fixed }j,k,\quad P^2/R_1^4\longrightarrow\infty.
 \tag{QC.1}
\]

In the original independent nonexceptional free coordinates, the exact complete first density and reconstruction are

\[
 D_V(z)=\exp\{-\tfrac12z^{\mathsf T}K(V)z+W_V(z)\},
 \qquad U=\Phi_V(z).
 \tag{QC.2}
\]

They include the Wilson action, averaged soft gauge, Haar, coarea, constraint correction, and their Jacobians once. The quadratic form contains the constrained critical-point correction. No classical residual force is deleted after changing a frame. A field-only classical factor \(C_0(V)\) is outside (QC.2).

Let \(B_P\) be the literal source-norm ball in one copy of the free Lie algebra, whose real dimension is the fixed integer \(q\). Then

\[
 Z_P(V;t)=\int\prod_e\mathbf1_{B_P}(z_e)D_V(z)
              e^{tF(\Phi_V(z))}\,dz,
\]
\[
 Z_Q(V;t)=\int\prod_e\rho_e(z_e,V)D_V(z)
              e^{tF(\Phi_V(z))}\,dz.
 \tag{QC.3}
\]

The one-coordinate factorization in (QC.3) is exact: the source Q tests are maxima over starred free bonds, and the exceptional bonds are omitted. A bond belongs to a bounded number of the original test boxes. Thus \(\rho_e\) is the intersection of those one-link group-norm tests; this does not assert independence of their probabilities.

The exact sum of all first R histories, with the retained bad free coordinates integrated against their actual masses and all relocations undone, is \(Z_Q\); see (AS.5)–(AS.7) in [M04 Averaged First Step Scalar](M04_Averaged_First_Step_Scalar.md). Its conditional scalar is

\[
 \overline Q_RF(V)=\partial_t\log Z_Q(V;t)\big|_{t=0},
 \qquad Q_PF(V)=\partial_t\log Z_P(V;t)\big|_{t=0}.
 \tag{QC.4}
\]

The problem addressed here is the physical-carrier localization and first raw coarse currents of (QC.4). It is not the original fixed-R-history operation. It does not by itself estimate the complementary P/Q sectors, a completed later effective action, or the full outer connected logarithm. The actual coarse density remains \(C_0(V)Z_Q(V;0)\).

## 2. Inputs and what they already establish

The following are primitive inputs, not assumptions about the desired marked output.

1. **Positive Gaussian marginals.** The first-step precision and its positive local restriction family have common physical-carrier coefficients. Their exact marginal continuation \(C_I(s)\) is (GM.13), with determinant branch (GM.16), strict positive reference gap, the small-rank density estimate (GM.18), and exact component consistency. The outside parameter radius and outside cube side can be fixed independently of g.
2. **Complete interactions and root.** The native complete \(W\), its supported Mayer factors, and the exact microscopic Wilson scalar reconstruction obey the first-clean LC/GM budgets. They are holomorphic in the free coordinates on any stated fixed multiple of P inside the native small physical chart. Raw first currents of the same coefficients have summable supported majorants. The primitive root \(F_h=\alpha\beta_0\sigma_h-c\), \(b=|\alpha|+h^4|c|\), has the local energy and quadratic-coordinate budgets (GM.31)–(GM.33).
3. **Actual minimum in a compact local frame.** [moving q reconstruction input analysis](moving_q_reconstruction_input_analysis.md), (MQ.3)–(MQ.13), provides a common Hermitian logarithm family

\[
 U_{1,e}=e^{i\Theta_e}U_{f,e},\quad
 \Theta_e=\sum_{X\supset S_e}\Theta_{e,X}(V_X),
 \quad U_f=Q^fV,
 \tag{QC.5}
\]

with connected raw carriers, real Hermitian coefficients, weighted value budget \(CgP_0\), and summed normalized raw-current budget \(Cg\), where \(P_0/P\) is a fixed source constant. This uses the actual first-step weak-curvature construction. Small plaquettes are not replaced by a global small-link gauge assumption.
4. **Literal local Q references.** On the source domain, the same analysis, (MQ.15)–(MQ.18), supplies the exponential comparison of \(U_1\) and every actual \(U_{1,\square}\), including its supported summed current. Each local reference depends only on its stated enlarged Q box.

The Gaussian and complete-interaction statements are used in their existing primitive form, including their strict decay and Gaussian-reserve margins. They are not obtained by placing an unsupported exponential label on a nonlocal function.

We first prove the result on the native admitted coarse domain and its specified analytic buffer. A whole-compact-domain extension requires a **single common positive kernel and reconstruction**, not separate extensions of already integrated outputs. That further construction is explicitly separated in Section 10.

## 3. The mixed initial enlargement

Fix the outside-decoupler radius \(R_o>1\) and then a sufficiently large fixed grid side \(m\), exactly in the order used in GM.2. Let \(I_{\rm reg}\) contain every ordinary Mayer/root raw footprint and every ordinary integration slot, including each fixed failed-P slot \(T\) introduced in Section 6. Thus every nondefect marginal endpoint receives its fixed m buffer. Let \(S\) be the set of Q-defect coordinate slots. For each \(e\in S\), let \(Q_e\) contain every full raw reference box used by its literal Q tests, the bond, and its fixed local-lift/gauge footprint.

Choose

\[
 \ell=\left\lceil C_\ell\log(2+P_0)\right\rceil
 \tag{QC.6}
\]

and form, with all enlargements rounded to the fixed m-grid,

\[
 D=D_m(I_{\rm reg})\ \cup\!
       \bigcup_{e\in S}D_\ell(Q_e).
 \tag{QC.7}
\]

This rule is additive under unions of the underlying species. Every ordinary coordinate is a fixed distance m from \(D^c\), while each Q-defect bond has distance at least \(\ell\). The actual source Q boxes already contain a large internal buffer; (QC.6) can use that buffer instead whenever it suffices. In either case

\[
 |D|\le C m^4|I_{\rm reg}|+
          C|S|(R_1+\ell+m)^4.
 \tag{QC.8}
\]

Only the Q defects pay the growing term. Applying a growing halo to every regular carrier would be invalid: its volume weight could defeat a fixed primitive decay rate for arbitrarily large ordinary carriers. Nor may the outside grid side grow with P; a fixed Cauchy factor per ever larger outside cube could not pay a fixed positive physical-volume weight.

Restrict the fixed family (QC.5) by

\[
 \Theta_e^D=\sum_{X\subset D}\Theta_{e,X},
 \qquad U_{*,e}=e^{i\Theta_e^D}U_{f,e}.
 \tag{QC.9}
\]

The field \(U_*\) is a compact raw-local coordinate frame, not a claimed new minimum or a field satisfying the nonlinear block constraint. At Q-defect bonds attach the outside monomial to each omitted connected coefficient, as in (MQ.10), giving \(U_{1,e}(s)\). On the fixed closed polydisc,

\[
 \sup_{|s|\le R_o}g^{-1}
       \|\Log(U_{*,e}U_{1,e}(s)^{-1})\|\le a,
 \tag{QC.10}
\]

where a is any fixed sufficiently small constant after choosing \(C_\ell\). The analogous summed raw-current bound holds. The connected-set cube count pays the monomials with a fixed part of the primitive carrier decay. The physical endpoint is \(U_1(1)=U_1\).

## 4. Keep the moving boundary real and local

For fixed real V, define the literal Q domain in this local frame by

\[
 D_e(V)=\left\{u:\
   \|e^{igu}U_{*,e}U_{1,\square,e}^{-1}-I\|<2gP
     \text{ for every original test }\square\ni e\right\}.
 \tag{QC.11}
\]

The principal coordinate chart is the fixed one about the identity. By the actual global/local comparison, (QC.10), and \(gP\to0\), the domain satisfies, for sufficiently small g,

\[
 B_{3P/2}\subset D_e(V)\subset B_{3P}.
 \tag{QC.12}
\]

The ball notation uses the source Lie-algebra norm; Euclidean norm equivalence has only fixed group-dependent constants. The domains are finite intersections of a bounded number of group-ball preimages. They have finite perimeter

\[
 \operatorname{Per}(D_e)\le C P^{q-1}.
 \tag{QC.13}
\]

Indeed each near-identity group ball is a uniformly bi-Lipschitz image of a fixed-dimensional norm ball at radius O(P); translation in the compact group and the logarithm chart have uniformly bounded derivatives here. Perimeter is subadditive under a finite intersection. No smoothness at intersecting faces or norm corners is assumed. The current companion note establishes the corresponding direct shell bound.

The domain is real, fixed under the outside parameters, and depends only on raw V in D. Put

\[
 F_{e,s}(u)=\frac1{ig}
       \Log\left(e^{igu}U_{*,e}U_{1,e}(s)^{-1}\right).
 \tag{QC.14}
\]

It is holomorphic in u and s on the requisite complex coordinate tube, and, for \(|u|\le3P\),

\[
 |F_{e,s}(u)-u|\le Ca,\quad
 \|D_uF_{e,s}-I\|\le Cga,
 \tag{QC.15}
\]

with fixed norm-equivalence constants. Decrease a once so the first bound is at most one. These follow from the analytic group logarithm/BCH map; no factor \(g^{-1}\) is left unpaid because the relative group shift is O(g a). At s=1, (QC.14) is the exact change from the local frame u to the original global free coordinate z.

For a holomorphic q-form \(\omega(z)=f(z)\,dz_1\wedge\cdots\wedge dz_q\), define the one-slot defect functional

\[
 \mathfrak D_{e,s}f
 =\int_{D_e}f(F_{e,s}(u))\det D_uF_{e,s}(u)\,du
       -\int_{B_P}f(z)\,dz.
 \tag{QC.16}
\]

The determinant is the exact coordinate Jacobian. At s=1, (QC.16) is integration against the original \(\rho_e-\mathbf1_{B_P}\). At general complex s it is an analytic **integral functional**. Neither the sharp indicator nor its dependence on raw V is being declared holomorphic.

## 5. A boundary-chain defect lemma

### Lemma QC.1 — annulus plus boundary chain

Assume (QC.12)–(QC.15), and assume f is holomorphic in a fixed tube containing the whole closed ball \(B_{3P+1}\) and all the homotopies used below. Set \(H_t(u)=u+t(F_{e,s}(u)-u)\), \(0\le t\le1\). As an identity of oriented integration currents,

\[
 \mathfrak D_{e,s}f
   =\int_{D_e\setminus B_P}\omega
       +\int_{[0,1]\times\partial D_e}H^*\omega.
 \tag{QC.17}
\]

The orientation of the second term is the one induced by the standard homotopy formula. Its absolute bound is independent of that convention. Every point on the first chain has norm at least P. Every point on the second has real norm at least \(3P/2-C\) and imaginary norm at most C. Its absolute q-dimensional Jacobian is bounded by a fixed constant times a, times the ordinary boundary area element and dt.

**Proof.** A holomorphic top form in q complex variables is closed as a real differential form: each holomorphic derivative wedges a repeated \(dz_j\), and the antiholomorphic derivatives vanish. Apply Stokes to the chain \([0,1]\times D_e\). Its two end faces give \(F_{e,s\,*}[D_e]-[D_e]\), and its side gives the boundary homotopy. Subtract \([B_P]\); containment in (QC.12) gives the annulus term. The displacement bound gives the location of the side. One tangent vector in the pulled-back top form is \(\partial_tH=F-id\); all remaining tangent derivatives are uniformly bounded, proving the Jacobian estimate. For finite-perimeter domains, approximate or use the standard distributional Stokes identity on the logarithm chart; the uniform perimeter bound permits the limit. ∎

For distinct slots the maps act on disjoint coordinates. Applying (QC.17) in each slot gives a product of chains with at most \(2^{|S|}\) choices. It introduces no \(|S|!\). Each slot contributes one annulus or one boundary chain, and keeps its own Gaussian tail.

### Lemma QC.2 — quantitative Gaussian bound with one tail per defect

Let the Gaussian marginal and ordinary integrand obey the GM.18–GM.20 reserve, also on the defect-coordinate tube, with sufficient strict slack. Let T be a set of fixed failed-P slots disjoint from S. Suppose the ordinary/source majorant is \(a_I e^{b|z|^2}\), with b within that reserve. Then, for all outside parameters in the fixed polydisc,

\[
 \left|\left(\prod_{e\in S}\mathfrak D_{e,s}\right)
    \int_{\text{other coordinates}}
       G_I(z;s,V)\,d\mu_{I,s}(z)\right|
 \le a_I e^{\epsilon r_I}
       C^{|S|}P^{C|S|}
       e^{-cP^2(|S|+|T|)}.
 \tag{QC.18}
\]

Here the notation means applying the defect integration functionals to the **density times integrand**, with all differential factors included once. The determinant loss coefficient \(\epsilon\) is tunably small from the original Gaussian/Mayer reserve, and \(r_I\) is the local integrated rank. It is not the whole lattice volume. Fixed polynomial roots are permitted by the same reserve.

**Proof.** Expand the product by Lemma QC.1. Along a resulting chain write \(z=x+iy\); y is supported on S, with \(|y|^2\le C|S|\). The complex Gaussian bound extends from the real locus by its explicit quadratic formula. If \(A_s=C_I(s)^{-1}\), then

\[
 \operatorname{Re}(z^{\mathsf T}A_sz)
 \ge x^{\mathsf T}C_{I,0}^{-1}x
         -C u_m|x|^2-C|S|.
 \tag{QC.19}
\]

The mixed imaginary term is bounded by a fixed multiple of \(u_m(|x|^2+|y|^2)\). The determinant is still (GM.17), so it costs \(e^{Cu_mr_I}\). The ordinary integrand contributes a small additional quadratic tilt and \(e^{C|S|}\). Pay fixed failed-P slots by the standard exponential Markov factor before integrating the other real coordinates.

After that tilt, the centered real Gaussian still has uniform upper and lower covariance bounds. Integrate all unmarked coordinates exactly. Its marginal on S has density at most

\[
 C^{|S|}\exp\{-c\sum_{e\in S}|x_e|^2\}.
 \tag{QC.20}
\]

Only this marginal contributes the fixed-per-slot constant; one must not replace the entire rank-r_I Gaussian by a crude \(C^{r_I}\) bound. The tilt determinant is \(e^{\epsilon r_I}\), with the specified small coefficient. On the annuli, volumes are O(P^q); on the side chains, (QC.13), the bounded displacement and bounded derivative give O(P^{q-1}) measure. The real-part map has uniformly controlled local distortion; alternatively the same bound follows directly in the original chain coordinates since their displacement is O(1). Every such factor is at radius at least P-C, so decreasing c once gives (QC.18). Quadratic or fixed polynomial insertions consume a further fixed part of the positive Gaussian reserve. ∎

In particular, after increasing the small-coupling threshold,

\[
 C^{|S|}P^{C|S|}e^{-cP^2|S|}
       \le e^{-c'P^2|S|}.
 \tag{QC.21}
\]

## 6. Exact finite Mayer bookkeeping

The expansion uses, coordinate by coordinate, the exact identity

\[
 \rho_e=1+(\mathbf1_{B_P}-1)
                 +(\rho_e-\mathbf1_{B_P}).
 \tag{QC.22}
\]

Thus an expanded term chooses disjoint fixed failed-P slots T and Q-defect slots S. It does not multiply two alternatives on the same coordinate. All interactions and the root are those of the complete density and reconstruction in (QC.2).

One can use the existing smooth coordinate truncation of each ordinary Mayer factor: equal one through \((7/2)P\), zero from \(4P\), with the native analytic factor defined on a slightly larger fixed domain. At the physical Q and P integrals this changes nothing, because all free coordinates lie inside \(3P\). In a defect term all transformed coordinates and their homotopy chains lie inside \(3P+C<(7/2)P\). Consequently every cutoff involving a transformed coordinate is identically one in that variable on the entire contour tube. Cutoffs in untransformed real coordinates stay fixed real functions. This is why no nonholomorphic truncated potential is moved through a complex contour.

After the exact finite expansion, integrate each term using its exact Gaussian marginal. Apply (QC.16) at the selected defect slots and the common covariance family at every term. At s=1 it is exactly the term obtained from (QC.22), including Jacobians. At other s it is analytic because its domains D_e are fixed, its maps and density are analytic, and its remaining coordinate cutoffs are not varied in their real arguments.

All finite-volume identities hold before taking absolute sums. The resulting estimates justify the convergent resummation and thermodynamic uniformity; no large-volume all-good probability is divided out.

## 7. True support, component factorization, and the tail payment

Set all outside parameters to zero except in a cube set A, and put

\[
 Y=D\cup\bigcup_{\Delta\in A}\Delta.
 \tag{QC.23}
\]

The covariance family, every surviving reconstruction-log coefficient, every ordinary raw factor, and every Q reference are supported in Y. A connected coefficient cannot cross between different components of Y. The reference frame (QC.9) and the mixed enlargement (QC.7) restrict exactly to the corresponding independent component construction. A defect's entire Q reference set lies in its own component. Therefore the Gaussian determinant, the ordinary factors, the chain maps, and the fixed integration domains factor over components. This is the equality of component families required by the polymer logarithm, rather than mere block diagonality with hidden exterior data.

Apply the product fundamental theorem of calculus to the outside parameters and Cauchy on their fixed polydisc. A coefficient filed on Y has its true raw support there and gains \((R_o-1)^{-|A|}\). Choose the final physical carrier rate \(\kappa>0\) after fixing the outside grid and its entropy margin. The ordinary initial supports pay their fixed collar from the primitive decay. By (QC.8), a Q defect pays at most

\[
 \exp\{C\kappa(R_1+\ell+m)^4\}
 \tag{QC.24}
\]

for its full initial footprint, before any simplification or quotient of geometry. Equation (QC.1) and \(\ell=O(\log P)\) imply

\[
 -cP^2+C\kappa(R_1+\ell+m)^4+C\log P
       \le-c_0P^2.
 \tag{QC.25}
\]

Thus each Q-defect species has a uniformly small physical-carrier majorant \(e^{-c_0P^2}\), after all full-footprint, shape, surface and coordinate-count losses. The remaining fixed outside-cube entropy is paid in the same order as GM.21. The rate \(\kappa\) is fixed; it does not tend to zero with g.

The exact convergent Mayer logarithms for Q and P now use the same regular and failed-P species registry. Every surviving term in their difference contains at least one Q-defect species. With a source derivative it also contains the marked root. Ordinary connected-cluster bounds sum those terms with their physical union carriers. The source-free logarithmic difference has a volume-independent **anchored polymer norm**; its whole vacuum sum may be extensive. The fixed-root scalar derivative has the genuinely volume-independent bound stated in Theorem QC.3. No estimate of the probability that every lattice coordinate is good is used.

## 8. Raw coarse currents: use real shells

For a normalized raw direction d and \(|t|\le1\), write \(V_t=\tau_{d,t}V\). Keep couplings, geometric grids and source parameters fixed. The local domain (QC.11) depends on the compact center matrices

\[
 H_{e,\square}(V)=U_{*,e}(V)U_{1,\square,e}(V)^{-1}.
 \tag{QC.26}
\]

For two such matrices, the group-norm triangle inequality confines the symmetric difference of the corresponding tests to a shell of normalized thickness

\[
 Cg^{-1}\|H_{e,\square}(V_t)-H_{e,\square}(V)\|.
 \tag{QC.27}
\]

The shell remains at norm at least \(3P/2-C\) for small increments. Its volume is at most

\[
 C P^{q-1}g^{-1}
       \|H_{e,\square}(V_t)-H_{e,\square}(V)\|.
 \tag{QC.28}
\]

This is a finite-difference assertion valid at corners as well as smooth boundary points. For an intersection of a bounded number of tests, sum their shells. The companion shell/current proof records the exact logarithm/Haar coordinate estimate. For increments not covered by the thin-shell estimate, the absolute two-domain tail bound divided by the increment gives the same Lipschitz budget after using the center displacement scale.

The normalized raw current bounds of (MQ.13), (MQ.18), plus the local reference footprints, bound the summed shell thickness by a fixed polynomial budget. The chain-map, covariance determinant, inverse, complete-interaction and root differences are treated by their existing supported derivative budgets. Work with the **full integrated defect** when changing its real domain, before differentiating a chosen boundary parameterization. This avoids any unsupported second derivative of a moving corner.

At complex outside parameters a shell is mapped by (QC.14) to the same fixed tube, and Lemma QC.2 supplies its tail. Cauchy and the outside fundamental-theorem formula commute with these real finite differences by their common majorant. Every resulting current has the same true raw carrier. Summing incident directions and root/normalizer derivative positions costs only the polynomial rank/carrier factors already allowed by the reserve and the strict spatial-rate slack. Each differentiated Q-defect cluster still has at least one Q defect, even when the differentiated species is ordinary.

For exact record identities, introduce the same two-copy integral for every individual localized tag,

\[
 H_a(V_{\rm ins},V_{\rm ker}).
 \tag{QC.29}
\]

The insertion copy controls only the microscopic reconstruction and mark, and the kernel copy controls the density and cutoff domain. Then the coordinate-presentation records are exactly

\[
 B_{a,d,t}^{\rm coord}
  ={H_a(V_t,V_t)-H_a(V,V_t)\over t},\qquad
 J_{a,d,t}^{\rm dens}
  ={H_a(V,V_t)-H_a(V,V)\over t}.
 \tag{QC.30}
\]

They sum to the diagonal finite difference tag by tag. Both records are bounded separately; a cancellation between them is not used to prove the estimate. The microscopic scalar has a genuine old-link difference, which is used when estimating its reconstruction pullback in the canonical direct record. If the local frame changes while the insertion copy is held fixed, the resulting motion of the integration coordinate and hence of the insertion belongs to the density/current record in (QC.30).

There is a separate primitive-only convention in which the old-state kernel includes the entire reconstruction pushforward. A fixed microscopic function then has no explicit dependence on the *coarse parameter* outside that pushforward, so its new direct coarse record is zero and the sum of the two newly proved contributions is filed in the new physical-kernel current. This is a separate filing of a primitive pushforward, not termwise identity with the canonical two-copy filing. No already existing B or J record may be reassigned by this observation. The theorem below concerns a primitive microscopic root, not inherited marked inputs.

## 9. Consequence on the actual native first-step domain

### Theorem QC.3 — first R-averaged moving-cutoff correction

Under the verified native primitive inputs of Section 2, at sufficiently small first-step coupling, the difference

\[
 \Delta_QF=\overline Q_RF-Q_PF
 \tag{QC.31}
\]

for the original primitive Wilson scalar has an absolutely summable connected physical-carrier representation with compatible value and first raw-current records. On the admitted native coarse domain and its specified buffered unit paths,

\[
 (Lh)^4\sum_a e^{\kappa(|Y_a|+\mathsf t(Y_a))}
 \left[
  \sup { |A_a|\over\widehat R_{Y_a}}+
  \sup {\sum_d\sup_{0<|t|\le1}
          (|B_{a,d,t}^{\rm coord}|+|J_{a,d,t}^{\rm dens}|)
       \over\widehat R_{Y_a}^{3/2}}
 \right]
 \le C L^4 b\,e^{-cP^2}.
 \tag{QC.32}
\]

The regulator is the same local coarse Wilson-energy regulator and shifted version as GM.4. The sum is over individual localized tags before cancellation. The rate, constants and source-independent construction are uniform in total volume. In the primitive physical-pushforward presentation the same bound holds for the combined newly generated kernel current, with the new direct coarse record zero. The genuine old-link differences used by the canonical reconstruction estimate remain present in that estimate.

**Proof.** Sections 3–7 construct the exact Q-defect species and their small supported majorants. The LC/GM scalar source construction supplies the root's adaptive analytic radius and its energy grade. Apply the connected expansion to \(\log Z_Q(t)-\log Z_P(t)\); its source derivative has both a root and a defect. The source-containing cluster argument is identical to the first-clean proof after replacing the failed-cutoff bound by Lemma QC.2. The source-independent nonvanishing of the local normalized generating function is a consequence of the convergent expansion, not a hypothesis about an extensive partition function. The root's constant term cancels from the difference exactly. Section 8 supplies both separate current budgets and the exact finite-record identity. Every remaining loss was paid in (QC.25), in the fixed outside grid margin, or in the already specified root Gaussian reserve. This gives (QC.32). ∎

Finite physical source jets can be inserted in the same construction with the fixed maps and domains. Their factorial class must be taken from the explicit root/energy majorants and the single linked-cluster theorem; no additional factorial is allowed merely for traversing another RG step. The one-root assertion (QC.32) is the statement proved here.

The original all-R-good operation already satisfies the native first-clean GM.4 bound. Adding (QC.32) therefore establishes the same native one-root bound for the actual R-averaged operation, with an exponentially small correction. This removes the first-step moving-Q issue **in this history-averaged operation and domain**. It does not repair the disproved fixed-history support convention.

If the actual outer coarse law has the stated unnormalized local-energy moment reserve, the positive tag majorants can also be integrated against that law. This gives averaged values and currents of this conditional transport. It still does not identify the average of a conditional logarithm with the full connected outer logarithm; that separate issue is explicit in DW.20 and DW.39.

## 10. Whole-product extension and downstream gates

The proof above uses real native V and buffered normalized paths. It does not silently assert that the literal local Q references are defined on every compact coarse configuration. A full ambient theorem must supply one of the following before replacing these restricted suprema by whole-product suprema:

* a single source-independent compact extension of the global reconstruction and of the local Q references, equal to the source ones on active data, with a uniformly centered product cutoff and the same supported current budgets; or
* a new stated density-weighted interface whose norms only use the actual admitted density and whose exact downstream kernels and connected-output conditions are separately verified.

Extending each already integrated coefficient independently would not establish a common positive old-state kernel, products, or recursive transport. Such a shortcut is not used here. The possible construction by a restricted global Hermitian log plus a locally extended exponentially small local-reference discrepancy is a separate source/input question.

Even after an ambient extension, the following remain genuine obligations before a Yang–Mills existence claim: the complementary P/Q geometries; completed later interactions and residual components; a valid treatment of retained histories or an exact density-weighted state reduction; uniform depth and running-coupling budgets; and the full physical connected-output/continuum conditions. The present theorem contributes a concrete first-step building block.

## 11. Mathematical sources

Primary source conventions: Balaban, CMP119 (1988), pp.246–251, especially (1.2), (1.8), (1.9), (1.15), (1.18), (1.19), (1.21), and the complete equality (1.22)–(1.30); CMP116 (1988), localized analytic integrals and failed-cutoff expansion.

Companion derivations: [ambient gaussian marginal](../A_support_and_normalization/ambient_gaussian_marginal.md) (GM.1–GM.4); [local extension kernel](../A_support_and_normalization/local_extension_kernel.md); [moving q reconstruction input analysis](moving_q_reconstruction_input_analysis.md) (MQ); [M04 Averaged First Step Scalar](M04_Averaged_First_Step_Scalar.md) (AS); and [M04 Q Boundary Shells](M04_Q_Boundary_Shells.md) (QS).  

This file presents a mathematical derivation and its exact hypotheses. It is not a formal proof-assistant certification and is not a claim of completed four-dimensional Yang–Mills existence.
