# Positive comparison and discrete currents for successful-component exclusion

This note isolates the change in the successful-component **admissibility mask** caused by replacing a bounded prepared-core label. It proves an exact positive normalization comparison, and shows that the physical footprint and enumeration cost of that mask change are paid by the actual successful-component masses. The old component laws, their fields, the cross interaction, and the current background are held fixed during this part of the comparison. Their separate changes have their own exact records; they are not absorbed into the mask calculation.

The source facts used are HS20.1-2, HS20.7 and RA20.7 of Annexes [BI](../../history/Annex_BI.md)–[BM](../../history/Annex_BM.md), together with the unnormalized energy and physical-volume reserve NR20.11-19. The result is compatible with the bounded-core code of CG.3-4. It does not prove the still missing raw-retained interaction expansion or a localized microscopic scalar moment bound.

## 1. Exact positive setup

Fix the native source-free real data and fix every residual old state u. Let P be one common finite universe of candidate successful geometric species. Each species X has its actual positive unnormalized old measure M_X(d eta_X), including its internal-history sum, reference ratios, self action, and normalization factors. There is no division by M_X(1).

Let A and B be two downward-closed collections of compatible successful families. Their pairwise successful-component compatibility is the same; only compatibility with the changed fixed residual-core configuration differs. Use the same positive weights

\[
 W_u(C,d\eta_C)
   =e^{H_C(u,\eta_C)}\prod_{X\in C}M_X(d\eta_X)
\]

on this common universe. Put

\[
 Z_A(u)=\sum_{C\in A}\int W_u(C,d\eta_C),
 \qquad K_A^u=Z_A(u)^{-1}\mathbf1_AW_u,
 \tag{EC.1}
\]

and similarly for B. The common family I=A intersect B contains the empty family and has positive partition function. The empty-family interaction H_empty(u) need not vanish.

This is an exact substep in a two-copy comparison. One may first change the local old measures and the interaction, and then change the admissibility mask while those new quantities are held fixed. Such an add-and-subtract does not alter the actual conditional law or discard any term.

## 2. Positivity ratio lemma

Let Bad_A be the set of species that are allowed by A but forbidden by B. Every family in A\I contains a member of Bad_A. Define Bad_B similarly. Assume the actual deletion inequality gives

\[
 K_A^u(X\in C)\le e^{\lambda_R}m_X,
 \qquad m_X=M_X(1),
 \tag{EC.2}
\]

uniformly in u, and likewise for B. This is the one-pinned-species case of RA20.7. Then

\[
 p_A(u):=K_A^u(A\I)\le
 \delta_A:=e^{\lambda_R}\sum_{X\in\mathrm{Bad}_A}m_X,
 \tag{EC.3}
\]

and the analogous bound holds for p_B. These are ordinary union bounds on the actual positive probability laws.

### Theorem EC.1

If delta=max(delta_A,delta_B)<1, then, uniformly in the fixed residual old state u,

\[
 1\le\frac{Z_A(u)}{Z_I(u)},\frac{Z_B(u)}{Z_I(u)}
      \le\frac1{1-\delta},
\]

\[
 \left|\log\frac{Z_A(u)}{Z_B(u)}\right|
       \le-\log(1-\delta)
       \le2\delta\quad(\delta\le\tfrac12).
 \tag{EC.4}
\]

No residual mass or successful mass is inverted.

**Proof.** Because the same weights are used on I,

\[
 \frac{Z_I(u)}{Z_A(u)}=1-p_A(u),
 \qquad \frac{Z_I(u)}{Z_B(u)}=1-p_B(u).
\]

The first pair of inequalities follows. Both logarithms log(Z_A/Z_I) and log(Z_B/Z_I) lie in the interval [0,-log(1-delta)], so their difference has absolute value at most the interval length, not twice its length. This proves (EC.4). \(\square\)

In particular, integrating the successful gas produces a uniformly bounded log-density perturbation of the remaining residual old law. This is an actual relative statement, independent of how small any residual old normalization is. It is not yet a carrier expansion of that perturbation.

There is an exact total-variation comparison as well. Let K_I^u be the common conditional law restricted to I. Then

\[
 K_A^u=(1-p_A)K_I^u+p_AK_{A\setminus I}^u
\]

and similarly for B. Hence

\[
 \|K_A^u-K_B^u\|_{\rm TV,variation}
       \le2(p_A+p_B)\le4\delta.
 \tag{EC.5}
\]

Here the convention is the total mass of the signed variation measure. For a nonnegative weight F, the same decomposition gives

\[
 \int F\,|K_A^u-K_B^u|
 \le K_A^u(F;A\setminus I)+K_B^u(F;B\setminus I)
       +|p_A-p_B|K_I^uF.
 \tag{EC.6}
\]

This form makes any necessary residual marked moment explicit.

## 3. The actual affected-species geometry

Use the local core code from CG.4: a block coordinate specifies empty or a rectangle of diameter at most 100M anchored at that block, its fresh graph/orientation, and the remaining actual finite fresh choices. On an admitted output, its completed component is Y=D_k(Lambda). The source size bound gives

\[
 \operatorname{diam}Y\le C_MR,
 \qquad |Y^+|\le C_M(1+R)^4,
 \tag{EC.7}
\]

including the fixed actual collars. A one-block code replacement changes only a bounded number of prepared cores in a bounded neighborhood, even after the local overlap-priority operation. Let W be the union of the corresponding old and new completed Y domains and their actual compatibility collars. Add fixed paths between the nearby core anchors if necessary. Then

\[
 |W|+\mathsf t(W)\le C_M(1+R)^4.
 \tag{EC.8}
\]

A successful species changes its residual compatibility only if its source compatibility footprint meets the changed excluded region. A sufficient, deliberately overinclusive test is X^+ meeting W; a sharper symmetric-difference test may be used when the exact compatibility convention permits it. Since every successful X also has diameter O(R), its anchor then lies in a current ball of radius O(R) about the changed core. There are O((1+R)^4) possible anchor blocks and at most exp(C_M(1+R)^4) geometric species per anchor. Internal histories have already been integrated in M_X and must not be counted again.

There is also a direct cylinder statement. For a fixed candidate X, its compatibility with the encoded residual cores can be decided by reading only core labels with anchors in the O(R) neighborhood of X. If an excluded Y intersects X, its bounded-core anchor must lie there because Y itself has diameter O(R). Thus the admissibility mask I_ell(X) is a function of an actual finite cylinder with at most C_M(1+R)^4 current blocks. It is not a function of one globally stored history flag. This radius is allowed to grow with R; its cost will be paid by the successful activity.

Compatibility with the **unreplaced** fixed exterior is held fixed in this calculation. A variation of that exterior requires its own declared footprint and cannot be included merely by calling it a fresh-core change.

## 4. Source mass pays the full geometric cost

Write P_k=p_0(g_k), as in the source. HS20.10 gives m_X<=exp(-P_k), uniformly in the admitted real data and all fixed residual old states after the deletion comparison. The source hierarchy gives

\[
 \frac{P_k}{(1+R_k)^4}\longrightarrow\infty.
 \tag{EC.9}
\]

Equations (EC.3),(EC.7)-(EC.9) therefore imply

\[
 \delta\le C_M(1+R)^4
         \exp\{C_M(1+R)^4+\lambda_R-P_k\}
       \le e^{-P_k/2}
 \tag{EC.10}
\]

after reducing the common coupling ceiling. This bound is independent of the residual old normalization and the total volume.

More importantly, the actual M-03 carrier enlargement is also paid. For any fixed kappa, assigning the change its entire W and the whole successful species footprint costs at most

\[
 \exp\{C_{M,\kappa}(1+R)^4\}.
 \tag{EC.11}
\]

This remains dominated by a fixed part of exp(-P_k). The point is not to pretend that exclusion is D0-local; its complete O(R^4) physical region is retained.

For marked species the sharper existing NR20.19 bound gives, with its genuine energy envelope F_X^natural and for every integer m>=0,

\[
 \sup_b\sum_{X\ni b}
       e^{a(|X^+|+\mathsf t(X^+))}
       M_X[(F_X^{\natural})^m]
 \le C^{m+1}m!e^{-P_k/2},
 \tag{EC.12}
\]

for any fixed permitted a after using the source reserve. The same estimate follows directly from NR20.12/16 and the actual shape count, with no repeated history enumeration. Summing over the polynomial number of affected anchors and inserting (EC.11) yields

\[
 \sum_{X\ {
m affected}}
  e^{\lambda_R}
  e^{\kappa(|\operatorname{cl}(W\cup X)|+
                    \mathsf t(\operatorname{cl}(W\cup X)))}
       M_X[(F_X^{\natural})^m]
 \le C_1^{m+1}m!e^{-P_k/4}.
 \tag{EC.13}
\]

All fixed compatibility collars are included in cl here. The old microscopic observable is not automatically equal to F_X^natural; it requires its actual pointwise or moment domination, as in NR20.13. Equation (EC.13) pays the source energy/rank class and the geometric mask enlargement. It does not assert a new native-energy dictionary.

## 5. Exact mask telescoping on connected expansion tags

Keep one common universe of species and attach the factor I_ell(X) to the activity of each successful X. Pairwise successful compatibility and all genuine interaction factors remain separate. For any ordered monomial with species occurrences X1,...,Xn, including repeated occurrences in a logarithmic/Mayer expansion, the exact identity is

\[
 \prod_{i=1}^n I_{\ell'}(X_i)-\prod_{i=1}^n I_\ell(X_i)
 =\sum_{j=1}^n
   \left(\prod_{i<j}I_{\ell'}(X_i)\right)
   [I_{\ell'}(X_j)-I_\ell(X_j)]
   \left(\prod_{i>j}I_\ell(X_i)\right).
 \tag{EC.14}
\]

Every nonzero summand has a distinguished affected successful occurrence Xj. No reciprocal indicator occurs; a zero indicator presents no difficulty. Retain j as an activity tag. Its actual carrier contains the unmodified connected-expansion carrier together with the full W and the compatibility cylinder for Xj. Formula (EC.13) pays precisely this extra geometric cost using the distinguished successful mass.

The identity applies term by term to a finite formal fugacity expansion, without any convergence assumption. For an absolutely convergent connected expansion it can be summed and differentiated with respect to the finite discrete replacement. This gives an actual tagged current expansion, with no division by a continuous parameter. The same rule applies to products involving already transported higher source vertices: their degrees and tags are retained, and the mask difference is performed before the finite logarithm or by differentiating that same logarithm.

## 6. The precise quantitative connected-expansion implication

The following formulation identifies the remaining hypothesis instead of hiding it inside a marked estimate.

Assume a source-free connected log/normalized-quotient expansion has been constructed from the **same positive component measures and interaction coefficients** in raw retained variables, with:

1. an absolute physical-carrier norm for its interaction coefficients;
2. a fixed convergence reserve in the successful-species activities, sufficient to distinguish one occurrence and sum the resulting n possible tags;
3. exact common carrier identities for each interaction and for each raw coordinate pullback, including changes in a core label;
4. the endpoint/reference budgets needed for the incoming marks.

Then the contribution to the discrete current produced solely by changing successful-species admissibility satisfies the same supported expansion estimate, multiplied by the finite pinned-activity factor on the left of (EC.13). In particular its extra full-Y enumeration/enlargement cost is uniformly bounded and is exponentially small as the coupling goes to zero.

**Proof.** Apply (EC.14) to every connected monomial. Mark the first distinguished changed species occurrence as part of its tag. Use (EC.13) for that occurrence and its extra footprint. Bound all remaining measures, interaction factors, and unmarked occurrences by the assumed absolute expansion norm. The convergence reserve sums the possible distinguished positions; equivalently it is the usual derivative of the convergent majorant with respect to a common successful fugacity. The connected union weight is submultiplicative, so appending the actual W/cylinder contributes no additional unidentified geometry. The direct/current compatibility is preserved because the same monomial difference, with the same tag j, is used in the exact two-copy add-and-subtract formula. \(\square\)

This implication assumes **unmarked source-free** expansion control and the explicit incoming endpoint budgets. It does not assume the desired marked numerator or the M-04 conclusion. The missing actual raw interaction expansion is still a real task: the currently proved native expansion uses completed components in its carriers and a relative metric contracting their interiors. That published bound alone does not satisfy hypothesis 1. The present argument closes the additional successful-mask enumeration cost once that carrier bridge is supplied; it does not claim that the bridge has been constructed here.

## 7. What the positivity result already gives without that expansion

Even before full carrier localization, (EC.4) is an unconditional finite-measure theorem for the actual native positive law. It gives a uniformly small log-ratio of the gas partition functions, pointwise in all residual old states. Thus successful-component support changes do not introduce an inverse rare-residual-mass factor. Equations (EC.10)-(EC.13) show that the complete physical size of the affected Y domains is affordable whenever an actual supported term is supplied.

Neither result supplies a local bound on a residual microscopic scalar. A remote fresh residual witness may control the full-Y native regulator while the regulator on the prepared core is one. That distinct marked-moment problem remains visible in CG.4 and is not solved by the successful gas's small masses.

## Sources

- Annexes [BI](../../history/Annex_BI.md)–[BM](../../history/Annex_BM.md): HS20.1-4, HS20.7-10, NR20.11-19, RA20.7. These formulas retain the actual successful masses and the full residual old posterior.
- LFR I, pp.177 and 201: eligible component size, factorization of the component-local sums and integrations.
- LFR II, pp.365, 377-380 and 391-392: common post-R background, the old positive operation, the successful-family sum and its actual cross exponential.
- [M04 Bounded Core Source Map](M04_Bounded_Core_Source_Map.md): CG.2-4, local core encoding, index/support identity conditional on outer admission, and padded discrete-current algebra.
