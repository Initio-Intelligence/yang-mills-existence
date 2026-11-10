# Normalizing a retained merged Q core against the actual Q gas

## 1. Result and the primitive interface

This note closes the normalization algebra for the retained-core operation in NP.29, conditional on the actual common integral family being constructed for NP.3 and the stated unmarked Q-gas convergence bound. It does not assume a normalized marked carrier estimate.

The next analytic base and exact physical averaging operation are those of BA.5a. The marked object is an old core payload, or a specified connected component of several old payloads. All next Q factors on its independent-coordinate set S are kept whole. Only the factors outside S are expanded. The denominator is the same unmarked next Q integral throughout.

Three ingredients are used:

1. an exact, absolutely convergent component expansion of that unmarked integral;
2. the exact root-deletion identity for the common coefficient, Gaussian marginal, determinant, coordinate and domain family;
3. the unnormalized core bound NP.27 and its supported analytic connector envelopes.

The cancellation uses no decay approximation, no probability lower bound for an individual core, and no separately normalized core law. Once the three primitive ingredients are supplied, all conclusions below follow by exact finite-volume identities and convergent series.

## 2. Common unmarked registry and supports

Let \(\mathcal L\) be a finite set of current blocks. A polymer species \(\gamma\) includes every source/localization tag needed to define its activity \(z_\gamma(v)\). Its carrier \(X_\gamma\) contains its full raw-field, integration-coordinate, gauge and local-reference footprints. Include a fixed incidence collar in these carriers so that incompatibility is represented by intersection:

\[
 \gamma\not\sim\gamma'
       \quad\Longleftrightarrow\quad
       X_\gamma\cap X_{\gamma'}\ne\varnothing.
 \tag{CN.1}
\]

More general finite-range incompatibility is reduced to this convention by the same fixed collar. This does not mean that a growing Q-reference box may be discarded.

The carrier and incompatibility choices here are determined by the fixed species tags and source scales, not by the value of v. Currents of a changing retained history geometry require that geometry's actual footprint and are not supplied by this fixed-family argument.

After a common retained-only prefactor has been separated, the actual unmarked next Q integral has the expansion

\[
 Z=\sum_{\Gamma\ {\rm compatible}}\prod_{\gamma\in\Gamma}z_\gamma,
 \qquad Z(\varnothing)=1.
 \tag{CN.2}
\]

The prefactor includes whatever classical action, zero-fluctuation inherited value, Gaussian normalization and coarea convention the actual construction assigns to it. It is identical in the marked and unmarked integrals, so it cancels in their conditional ratio. It must be restored in the transported source density.

All activities in (CN.2), and their component restrictions, come from one registry. In particular, the precision and determinant of each marginal are formed from the same continued covariance. A disjoint component is not assigned a newly chosen Gaussian or determinant branch.

For a cluster \(\boldsymbol\gamma=(\gamma_1,\ldots,\gamma_n)\), put
\[
 t(\boldsymbol\gamma)
 =\frac1{n!}\phi^T(\gamma_1,\ldots,\gamma_n)
                     \prod_{i=1}^n z_{\gamma_i},
 \qquad
 X(\boldsymbol\gamma)=\bigcup_iX_{\gamma_i},
 \tag{CN.3}
\]
where
\[
 \phi^T(\gamma_1,\ldots,\gamma_n)
 =\sum_{G\ {\rm connected\ on}\ [n]}
        \prod_{\{i,j\}\in E(G)}
                    \bigl[-\mathbf1_{\gamma_i\not\sim\gamma_j}\bigr].
 \tag{CN.4}
\]
A nonzero cluster has connected incompatibility support. Species repetitions in this logarithmic series are kept with their displayed combinatorial weights.

Let \(w_\kappa(X)=e^{\kappa |X|}\), or the fixed physical carrier weight already in use. The only algebraic property needed is
\[
 w_\kappa(X\cup X')\le w_\kappa(X)w_\kappa(X').
 \tag{CN.5}
\]
If a tree-distance factor is included, use (CN.5) for overlapping or touching connected carriers, with the fixed joining collar recorded. Every union to which this connected-weight estimate is applied below has that connection property. The disconnected root families in §8 retain their separate forest weights.

## 3. The marked component is not normalized separately

Let C be a merged old nonanalytic core. Use the kernel construction's S: all independent next coordinates in the full exceptional/gauge stencil needed to reconstruct C. Its enlarged core \(D_C\) includes S, every next Q-reference box at S, and the prescribed buffer. Components are merged when their constraint halos overlap; their union is used, not an enclosing rectangle. Analytic connectors do not alter this core-frame choice.

For a fixed old payload \(H_C\), the pointwise identity is exactly NP.29:

\[
 H_C\prod_e\rho_e
  =\left(H_C\prod_{e\in S}\rho_e\right)
                            \prod_{e\notin S}\rho_e.
 \tag{CN.6}
\]

The entire parenthesis is an unnormalized insertion. There is no division by its own integral. If it is ever written using a conditional core law, that law's exact mass must be multiplied back into the insertion.

Expand the analytic interactions and the cutoff alternatives outside S using the common registry. Attach a distinguished root node to \(D_C\), the complete old latent payload and all analytic connector support of the selected term. After component localization, write Y for the full carrier of the component containing that node. In particular,

\[
 D_C\subset Y.
 \tag{CN.7}
\]

A component meeting an old analytic connector belongs to Y even when it does not meet S. Cancellation based on distance from S alone would be wrong.

Let \(a_H(Y)\) be the sum of the actual unnormalized root-component integrals with carrier Y, retaining their individual tags if a carrier/current norm requires them. It includes every next Q factor on S, the root's exact coordinate Jacobian, all old latent integrations and all interactions assigned to that component.

### Lemma CN.1 — the root-deletion identity

Under the common integral-family prescription above, any other component disjoint from Y has exactly its activity from (CN.2).

**Proof.** On that component the core coordinate change is the identity: it acts only on the independent coordinates in S. Its Jacobian is also confined to S. The exceptional entries are physical readouts determined by the fixed-target solve, not additional integration variables.

The common Gaussian registry restricts to precisely the same covariance, precision, normalized marginal and determinant branch as in the unmarked construction. The common additive localization region has the same intersection with every complete primitive cube halo of the separated component. All remaining smooth-action coefficients are therefore the same entries of the unmarked registry.

Every Q factor retained whole by (CN.6) has its coordinate and full reference footprint in \(D_C\subset Y\). Thus a separated component has only the ordinary outside-S Q alternatives, with exactly their unmarked domains and coefficients. Every old latent variable, old real domain, and old analytic connector is assigned to Y. No old factor remains in the separated component.

The component equations and integration measures consequently agree term by term, including normalization. This proves equality of activities, not merely smallness of their difference. ∎


## 4. Exact cancellation against the same denominator

For a carrier Y define the restricted *gas sum*

\[
 Z_{\perp Y}
  =\sum_{\substack{\Gamma\ {\rm compatible}\\
                    X_\gamma\cap Y=\varnothing\
                    \text{for every }\gamma\in\Gamma}}
                     \prod_{\gamma\in\Gamma}z_\gamma.
 \tag{CN.8}
\]

Its coefficients are the same \(z_\gamma\) as in Z. This is not a new physical core normalizer or a newly chosen outside conditional law.

Every term in the marked expansion has one root component and a unique compatible family of other components. Lemma CN.1 gives

\[
 N_H=\sum_Y a_H(Y)Z_{\perp Y}.
 \tag{CN.9}
\]

There is no combinatorial multiplicity in the choice of the distinguished root component. Standard unmarked component symmetry factors remain those already contained in the activities.

Assume the strict unmarked cluster bound, so that the logarithms of Z and every restricted sum in (CN.8) are given by their absolutely convergent connected expansions. Then

\[
\begin{split}
 \log Z_{\perp Y}-\log Z
   &=-T_Y,\\
 T_Y
   &=\sum_{\boldsymbol\gamma:\,
                 X(\boldsymbol\gamma)\cap Y\ne\varnothing}
                       t(\boldsymbol\gamma).
\end{split}
 \tag{CN.10}
\]

Indeed a cluster disjoint from Y has exactly the same coefficient in the two logarithms. Every remaining cluster is absent from the first one. This is an exact coefficient cancellation.

Thus the normalized marked insertion is

\[
 \boxed{\quad
 \frac{N_H}{Z}
      =\sum_Y a_H(Y)e^{-T_Y}.
       \quad}
 \tag{CN.11}
\]

The denominator is the actual unmarked next Q operation from start to finish. Adaptive resummation inside S changes \(a_H\), not Z. For the identity insertion, the same derivation yields \(N_1/Z=1\), even if the chosen S is nonempty.

## 5. A quantitative bound for the excluded vacuum clusters

Here is a sufficient explicit weighted KP margin. Let
\[
 \zeta_\gamma=w_\kappa(X_\gamma)\sup |z_\gamma|
 \tag{CN.12}
\]
on the common admitted parameter domain. Suppose, for some \(a>0\),
\[
 \sup_{b\in\mathcal L}
       \sum_{\gamma:\,b\in X_\gamma}
                   \zeta_\gamma e^{a|X_\gamma|}
          \le\varepsilon,\qquad
 \varepsilon\le a.
 \tag{CN.13}
\]
The same condition can be imposed with a larger carrier rate to leave a strict margin for currents and incidences. With a different fixed incompatibility collar, replace \(\varepsilon\) by the corresponding fixed incidence multiple.

Condition (CN.13) implies the usual KP inequality
\[
 \sum_{\gamma\not\sim\gamma_0}
              \zeta_\gamma e^{a|X_\gamma|}
       \le a|X_{\gamma_0}|.
 \tag{CN.14}
\]
The hard-core tree majorant gives the rooted-cluster bound
\[
 \zeta_{\gamma_0}
 \sum_{n\ge1}\frac1{(n-1)!}
       \sum_{\gamma_2,\ldots,\gamma_n}
       |\phi^T(\gamma_0,\gamma_2,\ldots,\gamma_n)|
                      \prod_{i=2}^n\zeta_{\gamma_i}
       \le \zeta_{\gamma_0}e^{a|X_{\gamma_0}|}.
 \tag{CN.15}
\]

For completeness, the tree recursion is
\(T_\gamma=\zeta_\gamma\exp(\sum_{\gamma'\not\sim\gamma}T_{\gamma'})\).
Iteration from zero is bounded above by
\(\zeta_\gamma e^{a|X_\gamma|}\), by (CN.14). The rooted connected-graph sum is bounded by this tree sum: partition hard-core connected graphs by a rooted spanning-tree exploration, and sum the remaining permitted edges within each class. This is the hard-core tree-graph bound, with no division by an activity that might vanish.

In a cluster touching Y choose a polymer occurrence containing a block of Y. Summing over all such choices only overcounts it. Equations (CN.13)–(CN.15) and weight submultiplicativity yield

\[
 \sum_{\boldsymbol\gamma:\,X(\boldsymbol\gamma)\cap Y\ne\varnothing}
      w_\kappa(X(\boldsymbol\gamma))\,|t(\boldsymbol\gamma)|
       \le\varepsilon |Y|.
 \tag{CN.16}
\]

In particular \(|e^{-T_Y}|\le e^{\varepsilon|Y|}\), uniformly in total volume. This is a bound on clusters incident to Y, not on the extensive full vacuum logarithm.

Expand the exponential in (CN.11) into its tagged series. Each vacuum cluster in a product touches Y. Consequently its complete carrier, joined to Y, is connected whenever Y is connected. Equation (CN.16) gives the stronger coefficient bound

\[
 \sum_{\text{tags of }e^{-T_Y}}
       w_\kappa\!\left(Y\cup
                  \bigcup_{\text{clusters in tag}}X(\boldsymbol\gamma)\right)
                  |\text{coefficient}|
 \le w_\kappa(Y)e^{\varepsilon|Y|}.
 \tag{CN.17}
\]

This is the normalization carrier estimate. It keeps the added vacuum supports visible. A value bound on \(e^{-T_Y}\) alone would not prove it.

## 6. The core and connector budget after normalization

Let \(A_I\) be the primitive analytic connector envelope of a root term, as in NP.27, and let \(Y_I\) be its true full carrier after the source localization. That lemma supplies, before conditional normalization, envelopes of the form

\[
 |a_{H,I}|
 \le C A_I
       \exp\{\eta(r_{0,I}+r_{1,I})+C_a|S|\}
                            e^{-c_0 nP_0^2}.
 \tag{CN.18}
\]

The exact construction can retain additional nonnegative local energy regulators on this right-hand side; they are not replaced by a global supremum after normalization. The ranks and complete coordinate domains are those of the actual integral.

Combining (CN.17) with (CN.18) proves

\[
 \left\|\frac{N_H}{Z}\right\|_{\kappa,\rm carrier}
 \le C e^{C_a|S|-c_0nP_0^2}
        \sum_I A_I\,
          e^{\eta(r_{0,I}+r_{1,I})}
          w_\kappa(Y_I)e^{\varepsilon|Y_I|}.
 \tag{CN.19}
\]

For a regulated mark the norm on the left uses its original engineering normalization and the enlarged carrier regulator. Local nonnegative energy sums, including their permitted shifted versions, are monotone under carrier enlargement; the regulator on \(Y_I\) is therefore bounded by that on the full tagged union in (CN.17). No new normalization of the scalar is introduced. In particular a root \(h^{-4}F\) remains \(h^{-4}F\); a later \(L^4\) conversion comes from the ordinary change of scale, not from (CN.11).

The extra factor in (CN.19) has two different payments.

* The core has
  \[
   |D_C|+|S|\le C_L n(R_1/L+R_2+m)^4.
   \tag{CN.20}
  \]
  Its volume and the fixed displacement cost are paid together from one allocated part of the old reserve \(e^{-c_0nP_0^2}\).
* An arbitrary long analytic connector gets only its fixed primitive collar. The factor \(e^{\varepsilon|Y_I\setminus D_C|}\), and the small rank loss there, are paid by a strict primitive carrier-rate margin in \(A_I\).

For example, if the primitive connector sum in (CN.19) is bounded at rate \(\kappa+\tau\), with \(\tau>\varepsilon\) after the fixed incidence conversion, its connector part is finite at rate \(\kappa\). Since \(P_0^2/R_1^4\to\infty\) and the adjacent source radii are comparable, the combined core cost is at most \((c_0/2)nP_0^2\) at weak coupling. Then

\[
 \left\|\frac{N_H}{Z}\right\|_{\kappa,\rm carrier}
          \le C A_{\rm conn}e^{-(c_0/2)nP_0^2}.
 \tag{CN.21}
\]

The value \(c_0\) is the reserve remaining after the already declared NP.3 estimates. Equation (CN.21) spends that remaining reserve once on the combined core and normalization cost. It does not independently reuse the original tail for each added estimate.

## 7. First currents and existing records

The same algebra applies to first finite currents if the unmarked gas has a strict decorated KP bound. The current envelope uses the same carrier weight as the value envelope:

\[
 u_\gamma
  =w_\kappa(X_\gamma)\sup_v
       \sum_d\sup_{\tau\ne0}
            |\Delta^{\rm norm}_{d,\tau}z_\gamma(v)|.
 \tag{CN.21a}
\]

Here the finite difference has the prescribed native direction normalization and both endpoints lie in the stated domain. If the activity has separately retained direct/kernel records, use the sum of their absolute envelopes with their prescribed direction weights in (CN.21a). No already separated records are canceled to reduce this envelope.

One sufficient strict decorated bound is that (CN.13) remains valid after replacing \(\zeta_\gamma\) by \(\zeta_\gamma+t_*u_\gamma\), for some fixed \(t_*>0\). A coefficientwise derivative of this nonnegative majorant shows

\[
 \sum_{\boldsymbol\gamma\ {\rm touching}\ Y}
       w_\kappa(X(\boldsymbol\gamma))
       \bigl|\text{one current of }t(\boldsymbol\gamma)\bigr|
       \le\varepsilon_J|Y|,
 \tag{CN.22}
\]

with \(\varepsilon_J\le \varepsilon^+/t_*\), where \(\varepsilon^+\) is the enlarged anchored bound. This argument also covers zeros of individual activities.

Use the exact endpoint product rule
\[
 \Delta(a_H e^{-T_Y})
  =(\Delta a_H)e^{-T_Y(v')}
       +a_H(v)\Delta(e^{-T_Y}).
 \tag{CN.23}
\]
Termwise telescoping of the exponential series gives the carrier majorant
\[
 e^{\varepsilon|Y|}
       \left(|\Delta a_H|
                  +\varepsilon_J|Y|\,|a_H|\right),
 \tag{CN.24}
\]
with the supports of the changed vacuum factors attached to the tag. A strict additional rate loss pays the factor \(|Y|\).

Keep every inherited direct and kernel record in its existing filing. The denominator/excluded-vacuum response in the second term of (CN.23) is a new density-kernel current. In a primitive physical-pushforward convention, any reconstruction response already belongs to the numerator's kernel record; it is not moved into a direct record by this normalization argument.

The total density must still be multiplied back when a source-density transport is required. This conditional normalization identity is not a replacement for the outer connected generating function.

## 8. Several disjoint old cores

For disjoint merged core stencils, retain distinct roots until actual interactions connect them. For a fixed finite labelled collection of old insertions, let \(\pi\) describe the partition of these labels into the root-containing connected components of a term. The exact analogue of (CN.11) is

\[
 \frac{N_{\mathbf H}}{Z}
 =\sum_{\pi}\ \sum_{\{Y_B:B\in\pi\}\ {\rm compatible}}
       \left(\prod_{B\in\pi}a_B(Y_B)\right)
                  e^{-T_{\cup_{B\in\pi}Y_B}}.
 \tag{CN.25}
\]

A vacuum cluster touching two root components occurs once in the last exponent. Replacing that factor by a product of the separate single-root ratios would generally be incorrect. Its exponential expansion describes a forest until the attached vacuum clusters actually join components. An arbitrary union of far-separated roots is not assigned a connected carrier.

The bound (CN.16) with the union gives
\(\varepsilon|\cup_B Y_B|\le\varepsilon\sum_B|Y_B|\).
Thus joint core reserves pass through the same algebra without Hölder inequalities or repeated division by rare masses. Uniform source-order growth still requires the corresponding joint primitive insertion bounds; normalization does not supply those bounds by itself.

## 9. What would break the cancellation

Separate factorization statements for two different registries are insufficient. On two disjoint one-site polymers let the unmarked sum be
\(Z=(1+z_A)(1+z_B)\). If a root on A is assigned
\(N_H=a_H(1+\widetilde z_B)\), then
\[
 \frac{N_H}{Z}
   =\frac{a_H}{1+z_A}
                    \frac{1+\widetilde z_B}{1+z_B}.
 \tag{CN.26}
\]
Even perfect component factorization does not remove the remote factor unless \(\widetilde z_B=z_B\).

In the actual application, such a mismatch would arise if deleting the core changed an outside determinant branch, reference law, local-Q comparison choice, geometry convention or coefficient restriction. Lemma CN.1 requires their literal equality. Kernel's fixed core frame, identity map off S, common Gram/covariance registry and inclusion of all analytic connector support are designed to establish precisely this equality. Mere exponential decay would not suffice.

## 10. Scope of the completed gate

The normalization gate is therefore an exact consequence of the actual common primitive integral family and the unmarked weighted KP margin. No extra lower bound on a rare core denominator is needed.

For the analytic-base next Q operation, Z is its actual unmarked Q gas and the selected old payload is an insertion. If an entire old-source exponential is included in the physical denominator, its unmarked core species must first be included in that same gas and its KP bound verified. One may not normalize that different law using the analytic-base Z by accident.

This note does not prove the physical frame, complex native admission or joint old Gaussian reserve that enter NP.3. It proves their normalization consequence, including true carriers and first currents, once supplied. It does not close complementary P/Q histories, all source orders, all depths, or the fixed-history M04 statement.

## References

* M04_Next_Step_Regularity_and_Core_Payload.md: NP.24–NP.29, whole Q factors on S, merged-core frame, unnormalized reserve and exact resummation.
* [M04 Second Step Analytic Base Analysis](M04_Second_Step_Analytic_Base_Analysis.md): BA.5a and §§3–5, the actual next analytic base, determinant convention, common native components and admission.
* M04_Moving_Q_Cutoff_Localization.md and M04_Q_Boundary_Shells.md: original Q species, full footprints, component identities and defect reserve.
* M04_Density_Weighted_Transport_Interface.md: keeping one density weight, labelled products and connected logarithms in the correct order.
* CMP116 (1.3)–(1.10), (2.5)–(2.13): exact component equations, normalized Gaussian marginal localization and polymer logarithm. These source identities are the model for the common-registry condition, rather than a substitute for checking it for the new core frame.
