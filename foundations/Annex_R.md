# Three continuum seed estimates for the full tensor energy bound

**Annex R.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Scope

**P: a finite tensor-orbit theorem and its energy-bound implication.**
**C: application to the requested continuum theory.**
Once a Poincare-covariant 21-component curvature-bilinear field family
has been reconstructed, its spacetime-field energy estimates can be
reduced to three specified seed fields: the scalar, the pseudoscalar,
and one off-diagonal magnetic component. This is not a proof of any
of those three renormalized estimates, or of rotation restoration.

The reduction uses finitely many fixed Lorentz transformations. It
does not infer operator bounds by differentiating unbounded boost
generators, or by choosing a different time direction at the cutoff.

### 1. A real Lorentz orbit has dimension nineteen

Use the Minkowski field labels
\[
E=(F_{01},F_{02},F_{03}),\qquad
B=(F_{23},F_{31},F_{12}).
\tag{L.1}
\]
In this section a quadratic monomial means its symmetric color
bilinear, for example \(B_1B_2=\operatorname{Tr}(B_1B_2)\).
The cyclic trace makes the two factors symmetric. There are
\(21\) such labels, the real vector space
\[
\mathcal E=\operatorname{Sym}^2(\mathbb R^6).
\]
This is the Wick-continued version of the Euclidean tensor family;
the appropriate fixed phases of components containing time indices
are included in its Minkowski field convention.

Choose the infinitesimal rotations and boosts to act by
\[
J_aE=e_a\times E,\qquad J_aB=e_a\times B,
\]
\[
K_aE=e_a\times B,\qquad K_aB=-e_a\times E.
\tag{L.2}
\]
They act on the quadratic labels by the Leibniz rule. Reversing all
boost conventions gives the same invariant spans.

The scalar and pseudoscalar labels are
\[
s=|B|^2-|E|^2,\qquad p=E\cdot B.
\tag{L.3}
\]
They are invariant under the connected proper Lorentz group.
They remain separate fields because their transformation under
the disconnected parity operation is different.

#### Theorem 1.1

Let \(v=B_1B_2\). Its real linear orbit under the connected proper
Lorentz group spans a nineteen-dimensional subspace \(\mathcal W\).
Together with \(s\) and \(p\), it spans all of \(\mathcal E\):
\[
\boxed{
\mathcal E=\mathbb R s\oplus\mathbb R p\oplus\mathcal W.
}
\tag{L.4}
\]
Consequently there are nineteen fixed finite Lorentz transformations
\(\Lambda_1,\ldots,\Lambda_{19}\) such that
\[
s,\ p,\ D(\Lambda_1)v,\ldots,D(\Lambda_{19})v
\]
are a basis. No limit of these transformations is needed in the
operator argument below.

**Proof.** Work first with the invariant span of the generator
actions on \(v\).

Spatial rotations of \(B_1B_2\) generate every off-diagonal
\(B_iB_j\). A rotation by \(\pi/4\) in a coordinate plane generates
a difference of diagonal squares. Therefore the span contains the
five-dimensional space
\[
\mathcal B_0=\{B^\mathsf T M B:M=M^\mathsf T,\
\operatorname{Tr}M=0\}.
\tag{L.5}
\]
The exact boost identity \(K_1(B_1B_2)=E_3B_1\), followed by spatial
rotations, gives all off-diagonal \(E_iB_j\), \(i\ne j\).
Applying a \(\pi/4\) coordinate rotation to one such label gives a
diagonal difference \(E_iB_i-E_jB_j\), after subtracting the
off-diagonal terms already in the span. Thus it contains the
eight-dimensional space
\[
\mathcal C_0=\{E^\mathsf T M B:\operatorname{Tr}M=0\}.
\tag{L.6}
\]
No symmetry of \(M\) is imposed in (L.6).

For example the boost identities give
\[
K_1(E_3B_2)=B_2^2+E_3^2,\qquad
K_3(E_2B_1)=B_1^2+E_2^2.
\tag{L.7}
\]
Subtract these and use the magnetic diagonal differences in
\(\mathcal B_0\). The result includes \(E_3^2-E_2^2\).
Its spatial rotations generate
\[
\mathcal E_0=\{E^\mathsf T M E:M=M^\mathsf T,\
\operatorname{Tr}M=0\},
\tag{L.8}
\]
another five-dimensional space. Finally subtract
\(B_2^2-|B|^2/3\) and \(E_3^2-|E|^2/3\) from the first expression
in (L.7). This supplies \((|B|^2+|E|^2)/3\).

The displayed spaces and that last line are linearly independent.
Their dimensions sum to \(5+8+5+1=19\).
Their span is exactly the simultaneous kernel of the two linear
coefficient functionals
\[
\ell_s(Q)=
\sum_i[ B_i^2 ]Q-\sum_i[ E_i^2 ]Q,\qquad
\ell_p(Q)=\sum_i[ E_iB_i ]Q,
\tag{L.9}
\]
where brackets denote the coefficient in the monomial basis.
Direct substitution in (L.2) gives
\(\ell_s(J_aQ)=\ell_s(K_aQ)=
\ell_p(J_aQ)=\ell_p(K_aQ)=0\).
This codimension-two kernel is invariant and contains \(v\);
the orbit span has no additional directions. Also
\(\ell_s(s)=6\), \(\ell_p(p)=3\), and the cross evaluations vanish.
This proves (L.4).

To pass from generators to finite transformations, the linear span
of a group orbit is a subspace of a finite-dimensional space and
is closed. It contains the derivative at zero of every curve
\(D(e^{tX})w\) with \(w\) already in that span. Hence it contains
all the generator directions just exhibited. Conversely the
generator-invariant finite-dimensional span is invariant under
their exponentials and under the connected group they generate.
The two spans agree. A basis can therefore be selected from
nineteen actual finite orbit elements. \(\square\)

As a separate exact-arithmetic check, integer generator matrices in
the ordered monomial basis
\((E_1^2,E_1E_2,\ldots,B_3^2)\) give nineteen independent generator
words on \(B_1B_2\). Adding \(s,p\) gives determinant \(-36\).
The proof above does not depend on a numerical rank tolerance or
on treating a generator derivative as an energy-bounded operator.

### 2. Energy bounds pass through a fixed Lorentz transformation

Assume a reconstructed covariant field family \(v\mapsto\Phi_v(f)\)
with a common invariant field core, a unitary Poincare representation
\(U\), and joint translation spectrum in the closed forward cone.
Require this core also to be graph dense for the energy powers used
below, as in the established common smooth-energy core construction.
This makes the passage from core equalities to the closed-field
domains explicit.
Write \(H=P^0\ge0\). Use the convention
\[
\Phi_{D(\Lambda)v}(f)
=U(\Lambda)\Phi_v(f_\Lambda)U(\Lambda)^{-1}
\tag{L.10}
\]
on that core. The transformation \(f\mapsto f_\Lambda\) is a fixed
linear change of spacetime variables and is continuous on Schwartz
space.

Suppose a seed field has an actual one-sided bound, with \(r\ge0\),
\[
\|\Phi_v(f)(1+H)^{-r}\|
\le C_v\rho_s(f),
\tag{L.11}
\]
including a justified bounded extension and operator-domain
interpretation on the common core. More precisely, the closed
seed field has
\(D((1+H)^r)\subset D(\overline{\Phi_v(f)})\), and its restriction
to the specified common core is the reconstructed field.
A formal vacuum estimate is not the hypothesis (L.11).

#### Lemma 2.1

For each fixed proper orthochronous Lorentz transformation \(\Lambda\), there is
\(c_\Lambda\ge1\) such that
\[
c_\Lambda^{-1}H
\le U(\Lambda)HU(\Lambda)^{-1}
\le c_\Lambda H
\tag{L.12}
\]
in the joint translation spectral calculus. Consequently
\[
\boxed{
\|(1+H)^rU(\Lambda)^{-1}(1+H)^{-r}\|
\le c_\Lambda^r.
}
\tag{L.13}
\]
The transformed field in (L.10) therefore has the same energy
exponent \(r\), with a different finite constant and Schwartz
seminorm.

**Proof.** If \(p\) lies in the closed forward cone, then
\(|\mathbf p|\le p^0\). The time component of a fixed Lorentz
transform lies between positive fixed multiples of \(p^0\);
for a boost of rapidity \(\chi\), \(e^{-|\chi|}\) and
\(e^{|\chi|}\) suffice. The translation spectral theorem proves
(L.12). Both linear combinations of the \(P^\mu\) in that
inequality commute. The identity
\[
(1+H)^rU(\Lambda)^{-1}
=U(\Lambda)^{-1}
(1+U(\Lambda)HU(\Lambda)^{-1})^r
\]
reduces (L.13) to the pointwise ratio of their positive spectral
powers. It also preserves the required energy domains. Finally
factor, on the common core,
\[
\begin{aligned}
\Phi_{D(\Lambda)v}(f)(1+H)^{-r}
={}&U(\Lambda)\Phi_v(f_\Lambda)(1+H)^{-r}\\
&\mathrel{}\cdot
(1+H)^rU(\Lambda)^{-1}(1+H)^{-r}.
\end{aligned}
\tag{L.14}
\]
The two bounded factors give the extension and its norm bound.
Covariance on the core identifies that extension with the
specified field. \(\square\)

### 3. Reduction to three renormalized seed fields

#### Theorem 3.1

Under the covariance, spectrum and domain hypotheses above,
assume (L.11) for the three seeds
\[
s=|B|^2-|E|^2,\qquad p=E\cdot B,\qquad v=B_1B_2.
\tag{L.15}
\]
The exponents and seminorms may differ between seeds.
Then there are a common finite energy exponent
\(r=\max(r_s,r_p,r_v)\), a Schwartz seminorm \(\rho\), and a
constant \(C\) such that every one of the 21 tensor components
satisfies
\[
\boxed{
\|\Phi_\alpha(f)(1+H)^{-r}\|\le C\rho(f).
}
\tag{L.16}
\]
The same conclusion holds for a finite direct sum of fixed group
or color-bilinear sectors when the corresponding seeds are supplied.

**Proof.** Increasing a seed exponent to \(r\) only composes its
bounded extension with a contraction. Use the nineteen finite
transformations in Theorem 1.1 and Lemma 2.1. Every field label
is a finite linear combination of those nineteen transformed
labels and \(s,p\). The finite coefficient matrix and finitely
many pullback seminorms can be dominated by one fixed Schwartz
seminorm with one constant. Summing the bounds gives (L.16).
The equality is first an equality on the common covariant field
core, so the bounded extensions have the required field
identification. \(\square\)

This is a spacetime-smeared field theorem. It neither constructs
a sharp-time continuum field nor infers an operator norm from a
vacuum moment. The common invariant smooth-energy domain can
then be obtained through the already proved field/domain
assembly once its remaining hypotheses are in place.

### 4. How this changes the problem, and what it cannot remove

The full tensor energy conclusion need not require 21 independent
analytic estimates after covariance has been proved. Three
canonically identified, renormalized seed estimates suffice.
The scalar and pseudoscalar cannot be dropped: the magnetic
off-diagonal orbit misses precisely those two invariant directions.

The compact spatial theorem of Annex Q applies directly to the bare
off-diagonal magnetic clover seed, which is one of the five
trace-free magnetic combinations left unchanged by the scalar
repair. Its physical renormalized estimate is still missing.
In particular the running mixing matrix can mix bare magnetic
and temporal components within the stress and Weyl sectors.
The continuum seed \(\Phi_v\) need not be represented by a pure
magnetic cutoff multiplication operator after that mixing.
The exact F0 prescription must be retained in using (L.11).

Nor may (L.10) be used before full covariance R0 has been
established. A finite hypercubic cutoff symmetry does not provide
the boosts, the spectrum comparison, or the nineteen-dimensional
continuous orbit. The cutoff magnetic estimate and this continuum
reduction are distinct statements with distinct hypotheses.

The result reduces the field-count part of E0 once J0--J3 and the
seed estimates hold. It does not supply their ultraviolet
cancellation, the periodic-state passage, the phase decomposition,
or the required interacting ultraviolet coefficients. E0, R0 and
the full existence theorem remain open.


---
