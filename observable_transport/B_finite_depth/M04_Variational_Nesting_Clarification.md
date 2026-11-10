# Variational nesting: the criticality argument required by the source regularity classes

This note supplies a scope-preserving proof of the nesting statements used in CB and the real ancestral comparison AP. The relevant minimal orbits do agree. Their equality should be proved from criticality and uniqueness, rather than from an unqualified comparison of global minima over regularity classes at different scales. This note supplies that argument.

## 1. Exact nested constraints, different regularity classes

Let S be the microscopic Wilson action, and let M^j denote the literal recursively defined source averaging map through j levels. Work on its admitted smooth local chart. For integers r<j the source recursion gives

\[
 M^j=M^{j-r}\circ M^r.
 \tag{VN.1}
\]

The notation on the right denotes the remaining averaging operations on the r-th lattice, with the same gauge-covariant convention. It is not a claim that arbitrary group averaging operations are associative.

If F_j=U_j(V_j), then M^j F_j=V_j. Prescribing the finer data M^r F_j does indeed imply the same j-th data. However, the source regularity inequalities used to define the r-th variational problem can be weaker than those at level j. A finer admissible competitor therefore need not belong to the j-th regularity class. Fiber containment alone is not a valid comparison of these two globally restricted minimizations.

## 2. A nesting lemma based on criticality

Assume the following actual source hypotheses.

1. F_j is an interior critical point of S on the smooth fiber M^j U=V_j, modulo the permitted gauge transformations.
2. F_j belongs to the regularity class of the r-th variational problem, with strict room in its defining inequalities.
3. On the prescribed r-th fiber in that class, the source variational theorem has a unique critical orbit, represented by U_r(M^r F_j).

Then

\[
 F_j\sim U_r(M^rF_j),
 \tag{VN.2}
\]

where the equivalence is the source gauge equivalence on the prescribed fiber.

**Proof.** The chain rule applied to the actual recursion gives

\[
 D M^j(F_j)
 =D M^{j-r}(M^rF_j)\,D M^r(F_j).
 \tag{VN.3}
\]

Consequently every tangent vector v satisfying D M^r(F_j)v=0 also satisfies D M^j(F_j)v=0. Since F_j is an interior critical point of the j-th constrained problem, DS(F_j)[v]=0 for every such finer tangent vector. Thus F_j is a critical point of the r-th constrained problem. Hypothesis 2 places this critical point in the class where uniqueness applies. Hypothesis 3 then proves (VN.2). Gauge fixing chooses a representative of this orbit; it does not alter the Wilson action. ∎

This proof is local at the actual stationary point. It neither compares inadmissible competitors nor assumes convexity of the whole nonlinear fiber.

## 3. Why the hypotheses hold in the applications made here

In the homogeneous admitted branch, CMP102 Theorem 1 and Proposition 7 provide the regular critical orbit and its uniqueness. The improved regularity estimates place the constructed field strictly inside the larger source chart. The relative-field formulation and its analytic dependence are in Proposition 9, printed pp.305–309. The exact recursive averaging and gauge covariance are those of CMP98 and the averaging conventions retained in CMP109.

A field regular at spacing h_j is regular at a finer spacing h_r in the homogeneous setting used here. Restrict each source local regular gauge to the smaller patch and compare its bounds. For a relative potential and its first and second covariant operators the bounds have factors h_j^{-1}, h_j^{-2}, and h_j^{-3}; each is at most the corresponding finer-scale bound when h_r<=h_j. The same restriction applies to the small plaquette and force bounds. No global small-link gauge is required. This supplies the regular-class inclusion of the actual field, not inclusion of all possible finer competitors.

The exact exceptional-bond chart gives the smooth fiber and its tangent description on the relevant tube. At each actual admitted background the nonlinear averaging derivative has the required local right inverse. The identity of tangent kernels in (VN.3) is therefore used on the source constraint manifolds, not on a formal unconstrained coordinate list.

## 4. Two specific consequences

At the two-level classical background, apply (VN.2) with j=2 and r=1:

\[
 U_1(MU_2(W))\sim U_2(W).
 \tag{VN.4}
\]

This is the orbit identity used in the last paragraph of CB Section 3. Its classical energy conclusion remains valid, with the above criticality proof replacing the terse global-minimum comparison. A gauge-invariant microscopic Wilson scalar has exactly the same value on the two representatives.

For the fixed birth b in AP, apply the lemma with r=b and r=b+1 to every F_j with j>=b+1. It follows that F_j is the required finer minimal orbit in each case. In particular V_* = M^b F_j is stationary for the inherited birth classical action V -> S(U_b(V)) under the exact next constraint M V = M^{b+1}F_j. To see the stationarity directly, differentiate U_b along a tangent to that next constraint. The induced microscopic tangent lies in ker D M^{b+1}(F_j), so its pairing with DS(F_j) vanishes.

The complete constrained Hessian, including the force paired with the second derivative of the constraint chart, consequently annihilates the center-fixed gauge tangents and their mixed pairings. This is the fact needed when the axial source gap is combined with the averaged soft-gauge quadratic. Dropping the force term would not be justified by the orbit identity.

## 5. Scope

This clarification proves the stated nesting identities in the homogeneous admitted class. It supplies no comparison across changing hole geometries, no new large-field admission, and no uniform-depth interacting density theorem. It also does not turn a nonphysical complex decoupled coefficient into a minimum: criticality and minimal-orbit interpretations in this note concern the actual real source background.

Companions: [M04 Fixed Two Level Classical Energy Bridge](../A_support_and_normalization/M04_Fixed_Two_Level_Classical_Energy_Bridge.md) (CB Section 3); [M04 Real Ancestral Precision Comparison](../C_quadratic_transfer/M04_Real_Ancestral_Precision_Comparison.md) (AP.3 and its gap argument); [M04 Second Step Analytic Base Analysis](M04_Second_Step_Analytic_Base_Analysis.md) (the inherited classical action and full constraint-force Hessian).
