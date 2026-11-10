# Integrated covariance and retained data

The bounds involving an actual Wilson boundary derivative require the same chart, conditional law and configuration of fixed earlier innovations as the derivative being estimated. In particular, the all-history application requires the [anchored composed-response estimate](../../continuum/partial_gauge_transport.md); the [two-age estimate](../ordinary_oscillation.md) concerns the identical subtracted quantity at both endpoints. Exact finite-dimensional identities do not depend on these two application bounds.

A finite-dimensional proof and its application route.

## 1. Why this route is different

The original source representation retains integral operations \(T'_j(Y)\). The alternative at LFR II (1.103)–(1.104) integrates them and produces scalar boundary activities whose estimate no longer covers the component interiors. If one uses that alternative at every scale, a strengthened invariant for these scalar activities is needed.

A possible way to avoid that invariant is to keep the original representation for the entire published RG induction and integrate the completed kernels only when estimating the *final current conditional law*. That final integration does not feed a weakened scalar estimate into another RG step. The unresolved obstacle in Annex AT §6 is then the current/native chart of the complete kernel, with its old variables still present.

The key distinction is between pointwise covariance with hidden variables frozen and covariance of their complete integral. Only the latter is needed for the reduced current law. Hidden variables may be changed under a real gauge transformation. Surviving exterior variables must remain numerically fixed, or their genuine response must be retained.

## 2. A rigorous finite-dimensional covariance statement

Let \(x\) denote external parameters and \(\omega=(\omega_1,\ldots,\omega_q)\) all hidden variables of a completed component. Write its actual unnormalized integral as
\[
T_xF_x=\int F_x(\omega)\,W_x(\omega)\,dm(\omega).
\tag{G1}
\]
The measure can include compact group Haar variables, real Lie-algebra variables, counting measures on histories and graph choices, and constraint measures. A hard cutoff belongs to \(W_x\) or to its common integration support; neither is discarded.

Let \(x\mapsto x^u\) be an external real gauge transformation, and suppose a measurable bijection \(\Theta_{u,x}\) of the hidden variables obeys the equality of measures
\[
(\Theta_{u,x})_*(W_xm)=W_{x^u}m.
\tag{G2}
\]
Assume the complete test family is covariant:
\[
F_{x^u}(\Theta_{u,x}\omega)=F_x(\omega).
\tag{G3}
\]
Then
\[
T_{x^u}F_{x^u}=T_xF_x,
\qquad T_{x^u}1=T_x1.
\tag{G4}
\]
The same identities hold for the normalized quotient. This is an immediate change of variables, with no small-mass estimate and no pointwise claim about a frozen hidden coordinate.

### Lemma G1 (triangular composition of exact stage transformations)

Suppose the hidden variables can be ordered from coarse to fine so that the change of \(\omega_t\), conditional on already transformed coarser variables, is an exact measure-preserving bijection on its actual fiber. Suppose the transported stage weight and its actual selectors/constraints satisfy (G2) fiberwise. Then composition of the stage changes gives (G2) for the complete history integral, with no factor depending on \(q\).

**Proof.** Use Fubini in the positive reference integral and make the exact fiber change first at the finest integration, conditional on all coarser parameters. This replaces that stage by the transformed stage and leaves its coarser parameters intact. Repeat up the finite history. Equivalently one can use downward induction on the conditional kernel composition. Each step is an identity of measures. There is no estimate at an intermediate step and therefore no norm amplification. \(\square\)

For group variables, a left/right multiplication by fixed group elements has Haar Jacobian one. For Lie-algebra variables, a unitary adjoint transformation is an isometry and has real determinant one on the compact Lie algebra. These facts apply to a triangular family only when the multiplying gauge at a stage is fixed conditional on its coarser data; a gauge depending on the very variable being changed needs its actual Jacobian.

The constraint part must also be checked. A group delta at the identity is invariant under conjugation. A relative Lie-algebra tree condition \(A_e=0\) is invariant under an adjoint transformation. A raw tree condition \(V_e=1\) is not invariant under arbitrary independent endpoint multiplication. It needs the compensating gauge/relative-coordinate transformation or the actual Faddeev–Popov identity. This is the nontrivial issue, not a harmless determinant convention.

## 3. Holomorphic extension without complexifying the hidden integration variables

Let \(z\) be the current coordinates in a polydisc. Suppose for every *real* \(z\) an exact identity (G4) carries the physical external arguments \(x_{\rm phys}(z)\) to an admitted smooth native family \(\Phi(z)\). Suppose all surviving raw and old adjoint parameters are numerically fixed by that transformation. The hidden variables are changed by \(\Theta_z\).

Assume the source kernel on this native chart has the positive-reference representation
\[
T_{\Phi(z)}F_{\Phi(z)}
=T_*1\;\mathbb E_*\!left[e^{\sigma(\Phi(z),\omega)}
 F_{\Phi(z)}(\omega)\right],
\tag{G5}
\]
with \(\omega\) integrated over a fixed real support, \(\sigma\) holomorphic on the entire complex chart, and
\[
\sup_{z,\omega}|\sigma(\Phi(z),\omega)|\le\epsilon<\log2.
\tag{G6}
\]
Suppose the same joint chart admits every factor in the complete test \(F\), and gives locally uniform domination of the integrand. Then the right side of (G5) is a holomorphic extension of the *actual integrated physical function*. One does not need to evaluate \(\Theta_z\omega\) for complex \(z\), nor to prove an analytic domain for arbitrary complex hidden old fields.

**Proof.** Holomorphic dominated integration gives analyticity of the right side. For real \(z\), (G4) proves equality with the physical quantity. The real open current family determines its physical derivatives and the unique analytic continuation on the connected common chart. The formula keeps every hidden variable real in the chosen reference integral. \(\square\)

Normalized kernel bounds follow directly. If \(\|F\|_\infty\) is taken over the same complex native domain and real hidden support, then
\[
\left|\frac{T_{\Phi(z)}F_{\Phi(z)}}{T_{\Phi(z)}1}\right|
\le\frac{e^\epsilon}{2-e^\epsilon}\|F\|_\infty.
\tag{G7}
\]
Indeed the numerator is at most \(T_*1 e^\epsilon\|F\|_\infty\), while the denominator is at least \(T_*1(2-e^\epsilon)\). The common small real mass cancels.

The test \(F\) must be the whole incoming exponential or its actual connected-expansion products. It is not legitimate to prove (G4) only with \(F=1\), then use it for \(F=e^{B_{\rm in}}\) without (G3).

## 4. Primary-source statements actually located

The following are stated directly in LFR I.

1. **Printed p.179.** The source explicitly says its factors (1.5)–(1.9) are not gauge invariant under transformations of the \(V_j\) variables alone. The preparatory integrations near the component boundary are partly introduced to make a suitable gauge fixing possible. Therefore a proof treating all old cutoffs as individually gauge invariant is false.

2. **Printed p.182, after (1.25).** The full expressions and functions in that integral are invariant under the stated shell gauge transformations that are identity on the coarser lattice. The source uses this invariance to introduce the gauge-fixing factors by Faddeev–Popov. This is a genuine stagewise covariance statement with the required boundary restrictions.

3. **Printed pp.194–196, (1.76), (1.81)–(1.82).** The final prepared integral contains a deep \(V_h,T_h\) integral and an independent annular integral. The latter is free of the earlier delta functions. The new fluctuation is the *relative* field \(V''=V V_0\); a tree \(T_0\) fixes its gauge. The small-field cutoff is on the logarithm of this relative field.

4. **Printed p.197, after (1.87).** Changing the background \(U_0\) to the axial/Landau gauge requires a compensating transformation of \(V_h\), restricted to the specified boundary of the deep region, and an adjoint transformation of the relative field \(V\). The source explicitly says that the expressions in integral (1.76) are invariant under these paired transformations. It also permits choosing \(U_0\) in that gauge from the beginning.

5. **LFR II printed pp.379–380, (1.71)–(1.75).** After the exact rearrangement, only the displayed quadratic form and the full component selfaction depend on the independent native continuation. Their total complex change is a uniformly small pointwise \(\sigma\); the real reference density is positive. This supplies (G5)–(G7) on the published native chart.

6. **LFR II printed p.378.** Removal of the final gauge-fixing delta in the first-class components requires integration over the corresponding output \(V_k\); the source expressly says the resulting densities are equivalent after integration, not pointwise equal. A covariance proof at fixed \(V_k|Y\) must leave that delta unchanged or transform it by a valid fixed-output identity. It cannot use this removal at fixed output.

These facts are substantially stronger than the assertion that a scalar mass is gauge invariant. They do not by themselves verify (G2) for the exact gauge family used in every later current pullback.

## 5. How an actual proof could finish this route

The required check is specific. For the current smooth gauge converter and the nodal compensation already constructed in AQ/AR, compose them into one real frame change \(u_z\). It must equal the identity at every surviving fixed raw endpoint, and compensate every fixed old adjoint slot. The hidden fine endpoints need not obey this restriction: their variables are integrated and are changed in (G2).

Then verify, by induction through the actual original history, that:

- the raw coarse variables and their averaging constraints use the actual endpoint action;
- each relative old fluctuation uses the accompanying adjoint action;
- the actual graph/tree and cutoff factors are transformed by the paired source identities above;
- the coarser transformations supply exactly the boundary values needed by the finer stage, so that the map is triangular;
- no output variable that is fixed in the present conditional law has been integrated or transformed;
- every boundary interaction in \(e^{B_{\rm in}}\) transforms simultaneously, by the source scalar covariance (CMP119 (2.40)–(2.42)).

If those statements hold, Lemma G1 and (G5) prove the common native/current contour of the complete integrated operation. The current derivatives of its \(\sigma\) can then be bounded using the actual current-to-native endpoint rows, without assigning complex values to hidden old coordinates.

### What is not verified here

The p.197 transformation is explicitly tied to the source's chosen change of \(U_0\). The later nodal current-dependent converter is a different constructed family. A proof that the full p.197 identity applies to that family at every nested preparation stage, preserving the fixed-output constraints, has not been written from the printed definitions here. Lemma G1 cannot supply that missing stagewise identity. In particular, the noncovariant factors identified on p.179 cannot be skipped.

Thus this route remains promising and narrower than a general marked-history theorem, but the all-history matching clause is still open in this contribution.

## 6. Age labels if the covariance check succeeds

The useful roots are the *outermost active completed operations*, labelled by their latest completion. If a later operation consumes one of them, it is part of the new complete hidden integral, not an additional old rooted factor. If it survives, its actual native argument remains at its birth grade or a finer admitted layer.

This is different from keeping the birth of a scalar activity after its original anchor has been consumed. For a genuine surviving operation, a current-to-native endpoint estimate can be tested on the actual native endpoint. If it supplies
\[
\|D_i\Phi_{j,k}\|_{\rm native}
\le C\frac{\theta_k}{P_k}(1+k-j)^A
e^{-\Gamma(k-j)}e^{-c\rho(i,Y_j)},
\tag{G8}
\]
with \(\Gamma>4\log L\) plus the needed fixed polynomial reserve, then the source pointwise \(\sigma\) bound gives the ordinary score bound in OT.9 and the root sum pays \(L^{4(k-j)}\). The source coupling prefactor in OT.4 is \(g_j\) times fixed logarithmic powers, so it is uniformly small at a sufficiently small common ceiling.

The grade statement in (G8) must be checked for every surviving fixed-output component. An arbitrary physical path through current-sized cells does not establish it. If that actual endpoint statement is proved, the abandoned scalar CR.22 birth assignment is no longer needed in this route.

## 7. Analysis of the stronger halo proposal

For a fresh nonself term in the LFR II p.377 statement, the carrier \(Y\) contains each whole component of \(Z^{\sim}\) that it meets, and the weight uses the shortest tree visiting all exterior \(M\)-cubes of \(Y\setminus Z\). If \(Z^{\sim}\) is the positive one-layer dilation and an eligible rectangular component has all side lengths at least \(cMR\), its exterior halo contains at least \(c'R^3\) distinct \(M\)-cubes in four dimensions. A connected lattice tree visiting them has at least \(c'R^3-1\) edges up to fixed rounding. Thus the fresh reserve can pay an \(O(R)\) connector into that component, with a large margin as \(R\to\infty\).

A connected union of carriers that all contain the same whole halo can be connected at a common exterior cube; there is no need to traverse a latent component for free. This strengthens the original two-attachment diagnostic and is a valid geometric observation.

The remaining logical check is later localization with changed determining sets. Preserving a whole birth halo as an overcarrier supplies ordinary physical length. It does not by itself specify the scaled metric or native grade of a newly attached current/kernel endpoint, nor does it pay the number \(L^{4(k-b)}\) of old fine roots. The proposal works if it proves that every untouched tag's attachment uses an endpoint at its actual surviving birth grade, and that any consumed tag is fully rebased before the next root count. That exact matching remains the place to test the strengthened scalar invariant.

The application to every Wilson history is conditional on the composed response for the actual stopped integral.
