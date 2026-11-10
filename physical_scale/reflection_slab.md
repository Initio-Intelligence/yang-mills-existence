# Reflection-slab geometry and gauge reduction

**Finite-cutoff scope.** Nonzero reflected measurements at each cutoff allow finite normalization. Uniform bounds for the seven normalizing factors along one physical sequence and passage of the full normalized hierarchy have separate hypotheses.

## Assumptions and conclusions

The specified boundary problem has one nondegenerate
flat orbit at zero boundary amplitude. For every fixed finite slab
and every fixed boundary cochain, it has a unique global minimizing
orbit for sufficiently small amplitude. That orbit has an analytic
representative near zero, and its first variation solves precisely
the stated quadratic Dirichlet problem. Actual compact Wilson
conditional measures concentrate on that orbit as the bare
coefficient tends to infinity.

The proof contains no assumption that a general boundary gauge
configuration can be put in temporal gauge. It has no continuous
flat modulus left over: the spatial periods are fixed by the bottom
boundary, and the common gauge freedom on the top boundary removes
the remaining open-slab temporal transport. The required small
amplitude and large bare coefficient may depend on the finite
geometry. No uniform dependence is needed for a finite analytic
nonidentity witness.

## 1. Exact configuration space and gauge group

Let the slab have times \(0,\ldots,m\) and a spatial cubic torus of
period \(J\). Fix every spatial link on time zero to
\(\exp(i\epsilon b_i(x)\mathsf H)\), and every spatial link on
time \(m\) to \(I\). The variable links are the temporal links
joining consecutive times and all spatial links at times
\(1,\ldots,m-1\).

The allowed gauge group is

\[
 \mathcal K=SU(N)^{(m-1)J^3}\times SU(N).
\]

Its first factors act independently at the interior vertices.
Its final factor acts by one common matrix at every top vertex.
Every bottom vertex has gauge matrix \(I\). This preserves the
fixed boundary links for every \(\epsilon\), and its action on the
variable-link product does not depend on \(\epsilon\).

If \(g\) stabilizes any variable-link configuration, propagation
along the temporal links above each bottom vertex gives

\[
 g(0,x)=I\ \Longrightarrow\ g(1,x)=I
 \ \Longrightarrow\cdots\Longrightarrow\ g(m,x)=I.
\]

Thus the action is free for every configuration. In particular
there is no residual central stabilizer.

## 2. An explicit global analytic quotient

A concrete finite tree construction removes any need to assume
an analytic quotient theorem.

Contract all bottom vertices to one pinned root and all top
vertices to one vertex. Retain the interior vertices and every
variable edge, with its endpoint mapped under those contractions.
This produces a finite connected multigraph. The group
\(\mathcal K\) is exactly its rooted vertex gauge group. The
fixed bottom links are decorations at the pinned root; fixed top
links are identity decorations. They are not transformed or
removed from the action by this device.

Choose a spanning tree of the variable-edge multigraph. Starting
with gauge \(I\) at the root, successively choose the unique gauge
at each new vertex that sends its incoming tree edge to \(I\).
For an edge oriented the other way use its inverse. These gauges
are finite products and inverses of the tree-edge matrices.
They therefore depend real analytically on the original variables.

Every gauge orbit intersects the resulting tree slice once. To
check uniqueness, a gauge preserving identity on all tree edges
and fixed at the root must be identity along the entire tree.
Consequently

\[
 \mathcal C/\mathcal K
 \simeq SU(N)^{\,|E_{\rm var}|-\dim_{\rm vert}\mathcal K},
\]

where \(\dim_{\rm vert}\mathcal K=(m-1)J^3+1\) counts group
factors, rather than real Lie algebra dimensions. The exponent
is the number of non-tree variable edges. The quotient is thus
a compact analytic manifold with a global product-group slice,
independent of \(\epsilon\).

Product Haar measure on the variable edges pushes to full-support
measure on this slice. In fact its non-tree coordinates have
product Haar law: conditional on the tree edges, the gauge
changes at the endpoints are fixed, and left/right invariance
preserves the independent Haar laws of the remaining edges.
Only full support is needed for the concentration argument.

## 3. Exactly one zero-action orbit

At \(\epsilon=0\), every fixed boundary spatial link equals \(I\).
The plaquette energy is nonnegative, and

\[
 N-\operatorname{Re}\operatorname{Tr}U=0
 \quad\Longleftrightarrow\quad U=I.
\]

Thus zero slab action makes every variable-containing plaquette
flat. The boundary-only plaquettes are already flat, so the
connection is flat on the entire slab cell complex.

The slab retracts onto its spatial torus. Its fundamental closed
paths are the three spatial cycles, represented on the bottom
plane. Each has identity holonomy because all of that plane's
links equal \(I\). Plaquette flatness and these three identities
make parallel transport independent of the path between fixed
vertices.

Choose a base bottom vertex. Its path transports give a pure
gauge representation. The gauge is constant on each boundary
plane because that plane's spatial links are \(I\). Normalize
the bottom constant to \(I\). The top value remains one spatially
constant group element and is allowed by \(\mathcal K\).
Therefore every zero-action configuration lies in the identity
orbit.

This argument kills nontrivial central spatial holonomy as well
as ordinary noncentral holonomy: the boundary condition is
identity in the original group, rather than merely identity in
its adjoint representation. If the top gauge had instead been
fixed pointwise to \(I\), an open temporal transport modulus
would remain. The stated group correctly includes the factor
needed to remove it.

## 4. Hessian kernel and first variation

At the identity, extend a variable tangent \(A\) by zero on the
fixed boundary spatial edges. The quadratic action is

\[
 Q(A)=\frac12\sum_p\operatorname{Tr}(dA)_p^2.
\]

All weights are positive. Hence \(Q(A)=0\) precisely when
\(dA=0\). Closedness equates the spatial periods at different
times; their bottom values are zero. Discrete path integration
therefore gives \(A=d\phi\). The zero tangential boundary values
make \(\phi\) constant separately on each boundary plane.
Set \(\phi=0\) on the bottom plane. Its remaining top constant
and its interior values are exactly the Lie algebra of
\(\mathcal K\).

Conversely these gauge gradients have zero curl, so the Hessian
kernel is exactly the gauge tangent space. In the tree slice a
gauge gradient with all tree components zero must vanish: its
potential is zero at the root and remains zero along every
tree edge. Thus the quotient Hessian is positive definite.

Differentiating the analytic critical-point equations with
respect to \(\epsilon\) gives the Euler equations of this
quadratic form with boundary values

\[
 A_i(0,x)=b_i(x)\mathsf H,\qquad A_i(m,x)=0.
\]

Positive definiteness gives uniqueness modulo the displayed
gauge group. It follows that any explicitly proposed solution
of all those linear equations, including the temporal-link
equations, has the same first-order curvature as the actual
nonlinear minimizing orbit. This conclusion does not justify
omitting a Gauss equation; the note explicitly checks it in
the proposed fields.

## 5. Local implicit solution is the global minimum

On the quotient slice, \(S_\epsilon\) is real analytic in the
configuration and in \(\epsilon\). Its zero-amplitude minimum
has invertible Hessian. The analytic implicit function theorem
therefore gives one critical point \(q_\epsilon\), analytic in
\(\epsilon\), unique in a fixed neighborhood \(U\) of the
identity quotient point \(q_0\). Its Hessian remains positive
for sufficiently small \(\epsilon\).

For the global step, choose an open neighborhood \(V\) with
\(q_0\in V\) and \(\overline V\subset U\). Compactness and the
unique zero orbit give

\[
 \gamma=\min_{(\mathcal C/\mathcal K)\setminus V}S_0>0.
\]

Uniform convergence \(S_\epsilon\to S_0\) on the compact
quotient makes this lower bound at least \(2\gamma/3\) outside
\(V\), after reducing \(|\epsilon|\). Meanwhile
\(S_\epsilon(q_0)<\gamma/3\). Every global minimizer must
therefore lie in \(V\). It is an interior critical point and
equals the unique IFT point in \(U\). This proves global
uniqueness, not just a locally stationary branch.

There is no uniform quotient spectral gap in the slab size in
this reasoning. All uses of compactness and the implicit
function theorem occur at one fixed finite geometry.

## 6. Actual compact conditional law and full-law centering

For fixed boundary data the half law has exactly the density

\[
 Z_{\beta,\epsilon}^{-1}e^{-\beta S_\epsilon}\,dU_{\rm var}.
\]

The omitted plane-only plaquette factors are constants in this
conditional integral and cancel. No Gaussian law is substituted.

Fix an open neighborhood of the minimizing orbit. Its compact
complement has action at least \(\eta>0\) above the minimum.
A smaller open neighborhood of the orbit has positive Haar
measure and action at most \(\eta/2\) above the minimum.
The ratio of the two integrals bounds the complement
probability by \(C_\eta e^{-\beta\eta/2}\). Thus the conditional
expectation of any continuous gauge-invariant clover observable
converges to its value at the unique minimizing orbit.

The full finite-torus centering used in FN.11 is also valid.
The original Wilson action has global minimum zero, and its
entire minimum set consists of flat configurations. Although
that set can have nontrivial global holonomies, every local
plaquette clover and the scalar Wilson repair vanish there.
Compact concentration on that entire minimum set therefore
sends the uncentered physical smeared observable's mean to
zero.

Finally, for every finite positive \(\beta\), the boundary
conditional expectation is continuous in all the fixed plane
links, as a ratio of compact continuous integrals with a
strictly positive denominator. The actual boundary marginal
has a strictly positive continuous density relative to product
Haar. A nonzero centered conditional mean at the prescribed
boundary datum therefore remains nonzero on an open set of
positive marginal probability. Its squared conditional norm
has strictly positive full-law expectation.

These steps establish Lemma FN.4 from a nonzero classical
clover witness without treating a single boundary configuration
of Haar measure zero as an event of positive probability.

## 7. The original slow-volume replay is the required interface

The inference to FN.39–FN.40 uses the **specific** slow-volume
finite replay already stated in PE.22–PE.23. Mere permission to
enlarge the final torus after an unspecified replay lower bound
would not prove this conclusion: such a lower bound might force
faster volume growth.

Here PE.19–PE.21 supplies a fixed lower exponent \(H_0\).
Indeed its stopped suffix bound gives

\[
 Y_j\le Y_++D(K'-j),\qquad
 L^{j-K'}R_j\le
 C_R L^{-(K'-j)}
       [\log(Y_++D(K'-j))]^r.
\]

The supremum of the right side over all ages is finite. Its
constants are fixed by the source scheme and stopping ceiling,
independently of the bare offset \(\delta\), stopped depth, or
individual admitted trajectory. All required divisors and source
neighborhoods therefore fit above one fixed \(H_0\).

PE explicitly permits the replay choice

\[
 H_n=\max\{H_0,\lfloor\theta\log_L(2+K'_n)\rfloor\},
 \qquad 0<\theta<\tfrac14.
\]

FN.39 uses that choice without adding any further
cutoff-dependent enlargement. The finite reflection witness
requires only that a fixed physical lobe and its clovers fit,
and that the sufficiently fine lattice meets that lobe.
These impose fixed lower bounds on \(H_0\) and \(K_0\), not a
relation \(H\ge cK\). Enlarging the fixed \(H_0\) to satisfy
those conditions preserves

\[
 V_{{\rm term},n}\le C(2+K'_n)^{4\theta}=o(K'_n).
\]

Thus this proof removes the ultracold geometric cost
at precisely the inherited PE slow-volume replay scope. It
restores the volume hypothesis used by the existing ancient
sector reduction; it does not independently prove that
reduction's additional marked or normalization estimates.

## Conclusion for the new route

The finite geometric obstruction is closed. A nonzero electric
or helical projected clover value at the analytic minimum is a
valid witness that the corresponding exact finite Wilson
reflected measurement is positive for all sufficiently large
bare coefficients on that fixed torus. Once those explicit
projected values are verified, finite analyticity gives a
countable exceptional-set argument on every eligible geometry,
with no ultracold size condition on the torus.

This removes the need for the enlarged-volume cost. It
does not give a bound on the witness threshold or on the
positive measurements at the physical logarithmic coupling.
