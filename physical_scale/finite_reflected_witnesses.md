# Reflection witnesses at finite cutoff

**Gaussian calibration hypothesis (GC).** For the signed Gaussian increments of the actual stationary source section in its thermodynamic normalization, assume $\sum_{k<n}d_k^G=d_Bn+\vartheta_n$ with $d_B>0$ and $\sup_n|\vartheta_n|\le B_G$. The coupling and stopping conclusions use this calibration and the specified source readout and replay. A physical continuum limit also requires the stated uniform normalization and full-law hierarchy estimates.

**Finite-cutoff scope.** Nonzero reflected measurements at each cutoff allow finite normalization. Uniform bounds for the seven normalizing factors along one physical sequence and passage of the full normalized hierarchy have separate hypotheses.

This note proves a qualitative nondegeneracy theorem for the original
F01 clover measurements on every sufficiently fine finite cubic
Wilson torus. The proof uses the exact reflection-plane conditional
square, a finite-dimensional classical boundary problem, and two
explicit boundary fields. It does not use the ultracold comparison
window of the separate GN construction.

The consequence is that the countable exceptional-set construction
can use the original slow-volume stopped sequence. It does not give
the logarithmic coefficient estimates required by the remaining
quantitative part of F05.

## 1. Actual observables, geometry and target

Use the Wilson law, raw clovers, scalar repair, seven projectors and
physical positive lobe of Annex X (F.1), (F.4)–(F.20), without changing
their normalization. Let the fine torus have an even period \(J\) in
each of its four directions, physical spacing \(a\), and physical side
\(T=Ja\). Put \(m=J/2\). Assume
\[
 T>8/\mu,\qquad a<(1-\varepsilon_f)/(2\mu),\qquad
 \varepsilon_f=1/64,
 \tag{FN.1}
\]
and that at least one lattice site has \(f_\mu(x)>0\). The latter
holds for all sufficiently small \(a\), for example after requiring
\(a<\varepsilon_f/(2\mu)\). These conditions put every field stencil
used by the positive lobe inside the positive reflection half-torus.
They also ensure \(J\ge4\).

For a channel \(h\), let
\[
 \mathcal F_h(U)=P_h\,a^4\sum_xf_\mu(x)\widetilde q_a(x;U),
 \qquad
 \mathcal F_h^c=\mathcal F_h-\mathbb E_\beta\mathcal F_h .
 \tag{FN.2}
\]
Let \(\mathcal B\) be the spatial links on the two site-reflection
planes \(t=0\) and \(t=m\). The exact positive-half square gives
\[
 n_h(\beta)=\frac1{d_h}
 \mathbb E_\beta\!
  \left\|\mathbb E_\beta[\mathcal F_h^c\mid\mathcal B]\right\|_E^2.
 \tag{FN.3}
\]
This is exactly the measurement in F.22–F.24. In particular it uses
the full vector conditional mean, with the original reflected tensor
convention; it is not an ordinary local variance.

We prove the following finite-cutoff statement.

### Theorem FN.1

For every fixed finite cubic geometry satisfying (FN.1) and the
nonempty-lobe condition, there exists a finite number
\(\beta_0(a,T,\mu,N)\) such that
\[
 n_h(\beta)>0\qquad
 (\beta\ge\beta_0,\ \text{all seven channels }h).
 \tag{FN.4}
\]
No uniform bound on \(\beta_0\) is asserted.

## 2. A finite reflection-slab minimization lemma

Write the positive closed slab as
\[
 \Lambda_+=\{0,\ldots,m\}\times(\mathbb Z/J\mathbb Z)^3.
 \tag{FN.5}
\]
All spatial links on its two boundary planes are fixed. Its variable
links are all temporal links between consecutive planes and all
spatial links on planes \(1,\ldots,m-1\).

Fix a nonzero traceless Hermitian color matrix \(\mathsf H\) with
\(\operatorname{Tr}\mathsf H^2=1\). For a real spatial one-cochain
\(b=(b_1,b_2,b_3)\) on the three-dimensional periodic boundary, impose
\[
 U_i(0,x)=\exp(i\epsilon b_i(x)\mathsf H),\qquad
 U_i(m,x)=I,\qquad i=1,2,3.
 \tag{FN.6}
\]
The variable-link configuration space \(\mathcal C\) is a finite
product of copies of \(SU(N)\), independent of \(\epsilon\).
Let \(S_\epsilon\) be the sum of the Wilson plaquette energies in
this slab that contain a variable link. Plane-only plaquettes are
fixed factors and cancel from the slab conditional law.

The gauge group used in this proof is precisely
\[
 \mathcal K=
 \left\{g:
 \begin{array}{l}
 g(0,x)=I,\\
 g(t,x)\text{ arbitrary for }1\le t\le m-1,\\
 g(m,x)=g_m\text{ independent of }x
 \end{array}\right\}.
 \tag{FN.7}
\]
The common \(g_m\) is a variable in \(SU(N)\). It preserves every
opposite-plane boundary link because those links equal \(I\).
This group preserves (FN.6) for every \(\epsilon\), and its action
on the variable-link product is independent of \(\epsilon\).

### Lemma FN.2 — one nondegenerate vacuum orbit

The action of \(\mathcal K\) on \(\mathcal C\) is free. At
\(\epsilon=0\), the zero set of \(S_0\) is one \(\mathcal K\)-orbit.
The Hessian of \(S_0\) at that orbit is strictly positive on the
quotient tangent space.

**Proof.** Suppose a gauge transformation fixes a configuration of
the variable links. Each temporal link gives the relation between
the gauge matrices at its two ends. Starting with \(g(0,x)=I\)
and following the temporal path above each \(x\) forces every
interior gauge matrix and the terminal \(g_m\) to equal \(I\).
This proves freeness.

The quotient can be represented explicitly. Contract all vertices
of plane \(0\) into one pinned root, and all vertices of plane \(m\)
into one gauge vertex. Keep every interior vertex and every variable
link, obtaining a finite connected multigraph. The group (FN.7) is
exactly its rooted lattice gauge group. Choose a spanning tree of
its variable edges. There is a unique gauge transformation setting
every tree link to \(I\): propagate the gauge matrix from the pinned
root along the tree. All remaining link matrices are unconstrained
coordinates. Thus the quotient is globally a finite product of
copies of \(SU(N)\), with analytic gauge fixing independent of
\(\epsilon\). The fixed bottom links are decorations at the pinned
root, and the fixed top links remain \(I\); neither boundary
condition is changed by this construction.

The Wilson plaquette energy \(N-\operatorname{Re}\operatorname{Tr}U\)
is nonnegative and vanishes only at \(U=I\). At \(\epsilon=0\) the
boundary links are all \(I\). Hence a zero-action slab has identity
holonomy around every plaquette, including the boundary plaquettes.
Its three spatial fundamental holonomies are identity on plane
\(0\), and plaquette flatness transports that assertion throughout
the slab. A path between two vertices therefore has a
path-independent parallel transport, since every closed path is
generated by plaquette boundaries and those spatial fundamental
cycles.

Choose a base vertex on plane \(0\) and use these parallel
transports to write the flat connection as a pure gauge. Its
gauge values are constant on each boundary plane, because the
spatial links on those planes are \(I\). Fix the constant on
plane \(0\) to be \(I\). The resulting gauge transformation belongs
to (FN.7), so the flat connection is gauge equivalent to the
identity connection. This proves the single-orbit assertion.
The independent constant at plane \(m\) is essential here: it
removes the open-slab temporal flat mode.

At the identity, write an infinitesimal link field as a traceless
Hermitian matrix-valued one-cochain \(A\). The fixed boundary
spatial components of \(A\) are zero. The quadratic term in the
Wilson action is
\[
 Q(A)=\frac12\sum_{p\text{ in the slab}}
                \operatorname{Tr}(dA)_p^2.
 \tag{FN.8}
\]
Adding the plane-only plaquettes does not change this form on
variable tangents. Therefore its kernel consists of closed
one-cochains.

Such a closed cochain has zero spatial periods: those periods
are equal at different times by closedness, and vanish at
plane \(0\). Discrete path integration then gives \(A=d\phi\).
The vanishing spatial boundary components make \(\phi\) constant
on each boundary plane. Set its constant at plane \(0\) to zero.
Its constant at plane \(m\) is arbitrary. These are exactly the
infinitesimal gauge transformations in (FN.7). Conversely each
such infinitesimal gauge transformation has zero curl. Thus the
Hessian kernel is exactly the gauge-orbit tangent space.

The tangent space is finite dimensional, so the quadratic form
is strictly positive on any complement of that kernel, hence on
the quotient tangent space. \(\square\)

### Lemma FN.3 — unique small-boundary minimizing orbit

For each fixed boundary cochain \(b\), there is an
\(\epsilon_b>0\) such that, when \(|\epsilon|<\epsilon_b\),
\(S_\epsilon\) has a unique global minimizing \(\mathcal K\)-orbit.
That orbit has a representative analytic in \(\epsilon\) in a
local slice near the identity orbit. Its first-order curvature
is the curvature of the unique quadratic Dirichlet minimizer of
(FN.8), with boundary values \(A_i(0,x)=b_i(x)\mathsf H\) and
\(A_i(m,x)=0\), modulo the gauge group (FN.7).

**Proof.** Use the global tree coordinates just constructed for
the quotient. It is a compact finite product of matrix groups.
Local exponential coordinates on its remaining link variables
give an analytic chart at the identity, and the gauge-invariant
action \(S_\epsilon\) is analytic in that chart and in \(\epsilon\).

Lemma FN.2 gives a positive definite Hessian at its zero minimum
when \(\epsilon=0\). The analytic implicit function theorem applied
to the slice gradient yields one analytic critical point for small
\(\epsilon\), the unique critical point in a fixed smaller slice
neighborhood. Its Hessian remains positive definite.

Choose a smaller open neighborhood of the identity whose closure
lies inside the implicit-function uniqueness neighborhood. There
is a positive action gap on its complement in the compact quotient:
otherwise a sequence in that closed complement would have a limit
at a second zero-action orbit. Uniform continuity of \(S_\epsilon\)
in \(\epsilon\) preserves a positive part of that gap. The action at
the analytic critical point tends to zero. Every global minimum is
therefore in the smaller neighborhood, inside the region where
the critical point is unique. This proves global uniqueness of
its orbit.

Differentiate the critical-point equations at \(\epsilon=0\).
The resulting linear equations are exactly the Euler equations of
the quadratic form (FN.8) with the stated linear boundary values.
The positive quotient Hessian makes their solution unique modulo
the displayed gauge group. Thus any cochain satisfying those
linear equations and boundary values has the correct first-order
curvature. \(\square\)

This argument does not impose temporal gauge on an arbitrary
perturbed-boundary configuration. The particular \(A_0=0\)
cochains below solve the full linear Euler equations, including
the temporal-link Gauss equations.

## 3. Conditional Laplace concentration and full-law centering

For fixed boundary data (FN.6), the actual positive-half conditional
law is
\[
 d\nu_{\beta,\epsilon}
 =Z_{\beta,\epsilon}^{-1}e^{-\beta S_\epsilon}\,dU_{\rm var}.
 \tag{FN.9}
\]
Here \(dU_{\rm var}\) is the product of the original normalized
compact Haar measures. There is no Gaussian replacement.

### Lemma FN.4 — a nonzero classical boundary witness gives a positive norm

If, for one channel \(h\) and a sufficiently small fixed
\(\epsilon\), the uncentered vector \(\mathcal F_h\) at the
minimizing orbit of Lemma FN.3 is nonzero, then \(n_h(\beta)>0\)
for all sufficiently large \(\beta\), at this fixed geometry.

**Proof.** First, a continuous gauge-invariant function on the
variable-link space has a single value at the unique minimizing
orbit. The measures (FN.9) concentrate on every neighborhood of
that orbit as \(\beta\to\infty\).

To verify this last assertion directly, fix such a neighborhood.
Compactness and uniqueness give a positive gap between its
complement's minimum action and the global minimum. A smaller
neighborhood of the minimizing orbit has positive product Haar
measure and action within half that gap of the minimum. Comparing
the two integrals bounds the complement probability by a finite
constant times an exponentially decreasing function of \(\beta\).
Uniform continuity of the observable gives
\[
 \lim_{\beta\to\infty}\nu_{\beta,\epsilon}(\mathcal F_h)
       =\mathcal F_h(U_{\min,\epsilon}).
 \tag{FN.10}
\]

The full finite-torus Wilson law also concentrates on its
zero-action configurations. Every such configuration is flat,
even if its global torus holonomies are nontrivial. Every F01
plaquette clover and Wilson scalar is zero on a flat configuration.
The same compactness/gap argument, now using the whole flat
minimum set, consequently proves
\[
 \mathbb E_\beta\mathcal F_h\longrightarrow0.
 \tag{FN.11}
\]
Thus the conditional mean of the centered vector at (FN.6)
tends to the nonzero vector in (FN.10). It is nonzero for all
sufficiently large \(\beta\).

At any fixed finite \(\beta>0\), the slab conditional expectation
is continuous in the plane links. Its numerator and denominator
are compact integrals of continuous functions, and the denominator
is strictly positive. The plane-link marginal under the full
Wilson law has a strictly positive continuous density with respect
to its product Haar measure. Hence a nonzero conditional mean at
the prescribed plane data remains nonzero in an open set of
strictly positive marginal probability. Its squared norm has
positive integral in (FN.3). \(\square\)

## 4. Constant electric boundary data: the first five channels

Use the boundary cochain
\[
 b_1=1,\qquad b_2=1,\qquad b_3=0.
 \tag{FN.12}
\]
The quadratic Dirichlet minimizer has the representative
\[
 A_0=0,\qquad
 A_i(t,x)=(1-t/m)b_i\mathsf H,\qquad i=1,2,3.
 \tag{FN.13}
\]
Its spatial divergence is zero, its temporal differences are
constant, and its spatial curls vanish. It solves the spatial-link
Euler equations and the temporal-link Gauss equations of (FN.8).
Lemma FN.3 therefore identifies its curvature with the first-order
curvature of the actual nonlinear minimizing orbit.

The linearization of the literal F.4 clover gives
\[
 C_{01}=-\epsilon\mathsf H/m+O(\epsilon^2),\qquad
 C_{02}=-\epsilon\mathsf H/m+O(\epsilon^2),
 \tag{FN.14}
\]
and the other four components are \(O(\epsilon^2)\), uniformly
over this fixed finite lattice. Put
\[
 u=(1,1,0,0,0,0)
 \quad\text{in the ordered basis }(01,02,03,12,13,23),
 \qquad Q_*=uu^t.
 \tag{FN.15}
\]
The quadratic term of the raw clover tensor is
\[
 q_a(x)=\frac{\epsilon^2}{a^4m^2}Q_*+O(\epsilon^3).
 \tag{FN.16}
\]

The scalar repair is part of the actual field and must also be
checked. Each of the four oriented plaquettes for a fixed
nonzero electric component has quadratic Wilson energy
\(\epsilon^2/(2m^2)\). Hence
\[
 w_a(x)=\frac{\epsilon^2}{a^4m^2}+O(\epsilon^3),
 \qquad
 \operatorname{Tr}q_a(x)
       =\frac{2\epsilon^2}{a^4m^2}+O(\epsilon^3).
 \tag{FN.17}
\]
Thus \(2w_a-\operatorname{Tr}q_a=O(\epsilon^3)\).
The leading tensor in (FN.16) is also the leading tensor of
\(\widetilde q_a\). Its original positive smearing is
\[
 a^4\sum_x f_\mu(x)\widetilde q_a(x)
      =\epsilon^2c_E Q_*+O(\epsilon^3),
 \qquad
 c_E=\frac1{m^2}\sum_x f_\mu(x)>0.
 \tag{FN.18}
\]
All constants in these expansions may depend on the fixed cutoff;
no uniform perturbative radius is required.

The exact F01 projectors give
\[
 P_SQ_*=\tfrac13 I_6\ne0,
 \tag{FN.19}
\]
\[
 \operatorname{diag}(P_{T_d}Q_*)
       =(\tfrac12,\tfrac12,0,0,-\tfrac12,-\tfrac12),
 \tag{FN.20}
\]
\[
 \operatorname{diag}(P_{W_d}Q_*)
       =(\tfrac16,\tfrac16,-\tfrac13,-\tfrac13,\tfrac16,\tfrac16).
 \tag{FN.21}
\]
For the shared-index block with \(i=1,j=2\) and complementary
indices \(0,3\), the two F.12 coordinates are
\[
 x=Q_{10,20}=1,\qquad y=Q_{13,23}=0.
 \tag{FN.22}
\]
Their sum and difference projections are both nonzero. Therefore
\[
 P_hQ_*\ne0\quad
 (h=S,T_d,W_d,T_o,W_s).
 \tag{FN.23}
\]
Choose a sufficiently small nonzero \(\epsilon\) so that the five
nonzero leading vectors in (FN.18) cannot be canceled by their
remainders. Lemma FN.4 proves strict positivity of all five
corresponding measurements for sufficiently large \(\beta\).

## 5. Helical boundary data: pseudoscalar and disjoint Weyl channels

Let \(z=x_3\) be the third spatial lattice coordinate, and put
\[
 q=\frac{2\pi}{J}\in(0,\pi),\qquad
 b_1(x)=\cos(qz),\quad
 b_2(x)=\sin(qz),\quad b_3(x)=0.
 \tag{FN.24}
\]
This is spatially periodic and divergence free in the discrete
link sense: the first component is independent of \(x_1\), and
the second is independent of \(x_2\).

Choose \(\rho>0\) by
\[
 \cosh\rho=1+2\sin^2(q/2)
 \tag{FN.25}
\]
and define
\[
 h_t=\frac{\sinh(\rho(m-t))}{\sinh(\rho m)},
 \qquad 0\le t\le m.
 \tag{FN.26}
\]
Then \(h_0=1\), \(h_m=0\), and
\[
 h_{t+1}-2h_t+h_{t-1}
        =4\sin^2(q/2)h_t.
 \tag{FN.27}
\]
The quadratic Dirichlet solution is
\[
 A_0=A_3=0,\qquad
 A_1(t,x)=h_t\cos(qz)\mathsf H,\qquad
 A_2(t,x)=h_t\sin(qz)\mathsf H.
 \tag{FN.28}
\]
Indeed the spatial Laplacian of each displayed component is
\(-4\sin^2(q/2)\) times that component, so (FN.27) gives its
spatial-link Euler equation. Discrete spatial divergence zero
gives the temporal-link equation, and the omitted component
equations are zero. Again uniqueness modulo gauge in Lemma FN.3
identifies its curvature with the nonlinear minimizer's first
variation.

For \(1\le t\le m-1\), write
\[
 d_th=\frac{h_{t+1}-h_{t-1}}2
       =-\frac{\sinh\rho\cosh(\rho(m-t))}{\sinh(\rho m)}<0.
 \tag{FN.29}
\]
Directly summing the four oriented plaquettes in F.4 gives the
following first-order clovers:
\[
\begin{aligned}
 C_{01}&=\epsilon d_th\cos(qz)\mathsf H+O(\epsilon^2),\\
 C_{02}&=\epsilon d_th\sin(qz)\mathsf H+O(\epsilon^2),\\
 C_{23}&=-\epsilon h_t\sin q\cos(qz)\mathsf H+O(\epsilon^2),\\
 C_{13}&=+\epsilon h_t\sin q\sin(qz)\mathsf H+O(\epsilon^2),\\
 C_{03}&=O(\epsilon^2),\qquad C_{12}=O(\epsilon^2).
\end{aligned}
 \tag{FN.30}
\]
For example, the temporal clover is the centered temporal
difference of \(A_i\), because \(A_0=0\) and \(A_i\) is independent
of its own spatial coordinate. Similarly \(C_{23}\) is minus the
centered \(z\)-difference of \(A_2\), and \(C_{13}\) is minus the
centered \(z\)-difference of \(A_1\). This verifies both the signs
and the \(\sin q\) factor in (FN.30).

The original disjoint-index coordinates in F.13 are
\[
 p_1=q_{01,23},\qquad p_2=-q_{02,13},\qquad p_3=q_{03,12}.
 \tag{FN.31}
\]
Set
\[
 k_t=-a^{-4}h_t d_th\sin q>0
       \qquad(1\le t\le m-1).
 \tag{FN.32}
\]
Equations (FN.30)–(FN.31) imply
\[
 p_1(x)=\epsilon^2k_t\cos^2(qz)+O(\epsilon^3),\quad
 p_2(x)=\epsilon^2k_t\sin^2(qz)+O(\epsilon^3),\quad
 p_3(x)=O(\epsilon^3).
 \tag{FN.33}
\]
The scalar repair adds only a diagonal tensor, so it changes none
of these coordinates.

Let \(\bar p_i=a^4\sum_xf_\mu(x)p_i(x)\). Since the original
smearing weights are nonnegative and not all zero,
\[
 \bar p_1+\bar p_2
      =\epsilon^2 c_H+O(\epsilon^3),\qquad
 \bar p_3=O(\epsilon^3),\qquad
 c_H=a^4\sum_x f_\mu(x)k_t>0.
 \tag{FN.34}
\]
The pseudoscalar projection has three equal disjoint coordinates
with leading value \(\epsilon^2c_H/3\), which is nonzero.
The third coordinate of the disjoint Weyl projection has leading
value \(-\epsilon^2c_H/3\), which is also nonzero. Thus
\[
 P_P\,a^4\sum_x f_\mu(x)\widetilde q_a(x)\ne0,\qquad
 P_{W_p}\,a^4\sum_x f_\mu(x)\widetilde q_a(x)\ne0
 \tag{FN.35}
\]
at the actual minimizing orbit for sufficiently small nonzero
\(\epsilon\). Lemma FN.4 proves strict positivity of the remaining
two measurements for sufficiently large \(\beta\).

The two families of boundary witnesses may use different small
\(\epsilon\). There is no requirement that one boundary
configuration witness every channel. Taking the larger of the
two finite \(\beta\) thresholds proves Theorem FN.1.

## 6. Consequence on the original slow-volume stopped sequence

### Corollary FN.5 — nondegenerate normalization with the original slow volume

Under the actual-map and replay convention of PE, one can choose a
single bare prescription, perform its actual stopping and bounded
trimming, and retain the original slow-volume cubic geometry so that
every seven-channel F01 measurement is strictly positive at every
retained cutoff. The same sequence has \(V_{{\rm term},n}=o(K'_n)\),
the PE logarithmic bare order, and its emergent positive weak endpoint.
This conclusion does not prescribe that endpoint or give a
quantitative lower bound on the positive measurements.

**Proof.** At each fixed geometry, the original compact Wilson measurements
are real analytic functions of \(\beta>0\): their uncentered
compact integrals are entire, their real partition function is
strictly positive, and centering uses only finite products and
ratios. Theorem FN.1 shows that
\[
 \Delta_{K,H}(\beta)=\prod_h n_{h;\ell_0L^{-K},\,2L^H\ell_0}(\beta)
 \tag{FN.36}
\]
is not identically zero on every integer geometry with \(K\ge K_0\),
\(H\ge H_0\), where \(K_0,H_0\) are chosen just for (FN.1),
the nonempty-lobe condition and the retained PE geometry.
There is no requirement \(H\ge110K+2\).

For each pair \((K,H)\), the zero set of (FN.36) is discrete in
\((0,\infty)\). Their union \(\mathcal B_{\rm all}\) over these
countably many integer pairs is countable. Fix \(Y_{\rm base}\)
above the PE stopping threshold and choose one
\[
 \delta\in(0,1)\setminus
 \bigcup_{n\ge1}\{N b-Y_{\rm base}-n:b\in\mathcal B_{\rm all}\}.
 \tag{FN.37}
\]
Then all the bare coefficients
\[
 Y_{0,n}=Y_{\rm base}+n+\delta,\qquad
 \beta_n=Y_{0,n}/N
 \tag{FN.38}
\]
avoid every exceptional geometry simultaneously.

Run the original actual causal PE construction on (FN.38), obtain
its stopped and trimmed depths \(K'_n\), and then use its permitted
finite-torus replay. PE computes its homogeneous infinite-volume
coupling prefix before choosing the finite replay volume. The
exceptional-set exclusion has already covered every possible
integer output depth and volume, so no continuity of those choices
is needed.

In particular take the original slow-volume prescription
\[
 a_n=\ell_0L^{-K'_n},\qquad
 H_n=\max\{H_0,\lfloor\theta\log_L(2+K'_n)\rfloor\},
 \quad 0<\theta<\tfrac14,
 \qquad T_n=2L^{H_n}\ell_0.
 \tag{FN.39}
\]
For all sufficiently large \(n\), the exact measurements satisfy
\[
 n_{h;a_n,T_n}(\beta_n)>0
       \quad\text{for all seven }h,
 \qquad
 V_{{\rm term},n}\le C(2+K'_n)^{4\theta}=o(K'_n).
 \tag{FN.40}
\]
All the original PE conclusions remain: admitted prefixes, the
terminal compact inverse-coupling interval, logarithmic bare order,
and an emergent strictly positive terminal subsequential coupling.
The compatible slow volume preserves the geometry hypothesis of
the ER.1/H2S global ancient-sector reduction. It does not supply
any additional marked estimate used in that reduction.

The choice of \(\delta\) is existential. As in GN.3, nested rational
intervals on which successive finite analytic products are
positive give a deterministic set-theoretic prescription, but no
effective computation or quantitative coefficient lower bound is
asserted. \(\square\)

## 7. The actual increment to F05

On the sequence in (FN.38)–(FN.40), the original physical
normalization coefficients exist, are finite, and have no zero
channel:
\[
 z_{h,n}=\sqrt{\lambda_h/n_{h;a_n,T_n}(\beta_n)}>0,\qquad
 c_n=z_{S,n}m_n.
 \tag{FN.41}
\]
Consequently the actual finite normalization determinant is nonzero,
and the totalized fallback in F.35 is never used on the retained
tail. This is a finite-cutoff nonsingularity result for the
prescribed Wilson observables, compatible with the same slow-volume
PE geometry used elsewhere.

There is still no estimate of how small these positive measurements
may be at the logarithmic bare values \(\beta_n\). In particular
Theorem FN.1's geometry-dependent \(\beta_0\) is a witness of
nonidentity, not a claim that the physical \(\beta_n\) exceeds it.
The generic exceptional-set argument proves positivity at
\(\beta_n\), and proves no quantitative lower bound there.
The remaining F05 work is the stated logarithmic budget for the
actual positive normalization data and their inverse products.
The finite prescription, the original physical targets, and
the still-unproved prescribed B05 endpoint are not changed.
