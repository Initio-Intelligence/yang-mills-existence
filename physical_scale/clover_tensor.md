# Clover linearization and tensor-channel witnesses

**Finite-cutoff scope.** Nonzero reflected measurements at each cutoff allow finite normalization. Uniform bounds for the seven normalizing factors along one physical sequence and passage of the full normalized hierarchy have separate hypotheses.

## Assumptions and conclusions

The two boundary-field witnesses in
`finite reflected witnesses`, FN.12–FN.35, are
correct for the actual F01 observables. The signed four-plaquette
clover, the Wilson scalar repair, the orientations in the
disjoint-index sector, and the original positive smearing all
give the asserted nonzero channel vectors.

The constant electric witness detects
\(S,T_d,W_d,T_o,W_s\). The helical witness detects both \(P\)
and \(W_p\). Neither conclusion substitutes a continuum
curvature for the discrete F01 stencil.

FN.1 contains a necessary geometry qualification: the sampled positive lobe must be
nonempty. The displayed F01 stencil-separation
inequality alone does not guarantee that a very narrow bump
contains a lattice vertex. The additional condition in FN.1,
for example \(a<\varepsilon_f/(2\mu)\), ensures nonemptiness
and is automatic along the sufficiently fine tail.

## 2. Exact source conventions

The definitions used are those of Annex X of
the Wilson observable definitions:

- F.3 uses the ordered pair basis
  \((01,02,03,12,13,23)\) and the Frobenius inner product
  on symmetric six-by-six matrices.
- F.4 uses the factor \((8i)^{-1}\), the sign
  \(\sigma\tau\), and the four oriented rooted plaquettes.
- F.5 defines \(q_{AB}=a^{-4}\operatorname{Tr}(C_A C_B)\).
- F.6 adds \(I_6(2w-\operatorname{Tr}q)/6\), where \(w\)
  is the literal four-vertex Wilson scalar.
- F.9–F.14 give the seven exact orthogonal projections.
- F.19–F.24 define the positive lobe and the centered
  reflected measurement.

Annex O Section 29, especially O.42, verifies that the
reflected conditional-square convention includes the
tensor reflection signs. The conditional square FN.3
uses this same original convention.

Fix the Hermitian traceless color matrix \(\mathsf H\)
with \(\operatorname{Tr}\mathsf H^2=1\). The color
projection \(\pi_0\) does not change the first-order
curvature because \(\operatorname{Tr}\mathsf H=0\).
The normalization \(\operatorname{Tr}\mathsf H^2=1\)
is retained in every quadratic coefficient below.

## 3. Linearization of the actual signed clover

Write the link potential at a positive link's initial
vertex as \(A_\mu(x)\). Its forward plaquette curl is

\[
 F^+_{\mu\nu}(x)
 =A_\nu(x+e_\mu)-A_\nu(x)
  -A_\mu(x+e_\nu)+A_\mu(x).
 \tag{CT.1}
\]

At first order about the identity, the signed plaquette
with directions \(\sigma e_\mu,\tau e_\nu\) is
\(\sigma\tau\) times this positively oriented curl
at its lower corner. The additional \(\sigma\tau\)
in F.4 removes that orientation sign. Consequently
the exact linearization of F.4 is

\[
 C_{\mu\nu}(x)
 =\frac\epsilon4
 \sum_{u\in\{0,-e_\mu\}}
 \sum_{v\in\{0,-e_\nu\}}
 F^+_{\mu\nu}(x+u+v)+O(\epsilon^2).
 \tag{CT.2}
\]

All the curvature terms are based at the common vertex
in the nonlinear definition. Their parallel-transport
corrections do not alter (CT.2), since the background
links are identity. Pure infinitesimal gauge changes
of the potential also leave its curl unchanged.

For \(A_0=0\), and \(A_i\) independent of its own
coordinate \(x_i\), the four-corner average gives

\[
 C_{0i}(t,x)
 =\epsilon\frac{A_i(t+1,x)-A_i(t-1,x)}2
   +O(\epsilon^2).
 \tag{CT.3}
\]

There is no extra temporal half-step factor. For
\(A_3=0\), with \(A_i\) depending only on \(x_3\),
the spatial clover similarly uses minus the centered
\(x_3\)-difference of \(A_i\). These two facts give
the factors and signs in both witnesses.

## 4. Constant electric seed and the scalar repair

For the seed \(b=(1,1,0)\), the stated quadratic
Dirichlet representative is

\[
 A_0=0,\qquad
 A_i(t,x)=(1-t/m)b_i\mathsf H.
 \tag{CT.4}
\]

Every nonzero electric plaquette curl equals
\(-\mathsf H/m\); all magnetic curls vanish. Thus

\[
 C_{01}=C_{02}=-\epsilon\mathsf H/m+O(\epsilon^2),
\]

and the remaining four clovers have zero first-order
coefficient. With \(u=(1,1,0,0,0,0)\) and
\(Q_*=uu^t\), this gives

\[
 q_a(x)=\frac{\epsilon^2}{a^4m^2}Q_*
            +O(\epsilon^3).
 \tag{CT.5}
\]

For each one of the four signed plaquettes of either
nonzero electric orientation, the Wilson energy has
quadratic coefficient

\[
 s(P)=\frac{\epsilon^2}{2m^2}
            \operatorname{Tr}\mathsf H^2+O(\epsilon^3)
       =\frac{\epsilon^2}{2m^2}+O(\epsilon^3).
\]

There are two such orientations. The actual prefactor
\(1/(4a^4)\) in F.6 therefore gives

\[
 w_a=\frac{\epsilon^2}{a^4m^2}+O(\epsilon^3),
 \qquad
 \operatorname{Tr}q_a
       =\frac{2\epsilon^2}{a^4m^2}+O(\epsilon^3).
 \tag{CT.6}
\]

Hence the scalar repair has no quadratic coefficient
on this witness. Equation (CT.5) is also the leading
term of the actual \(\widetilde q_a\), including its
scalar channel. This is a property of the constant
electric first variation; it is not an assertion
that clover trace and Wilson energy agree on arbitrary
lattice fields.

### 4.1 All first five projections are nonzero

The diagonal entries of \(Q_*\) are
\((1,1,0,0,0,0)\), with sum two. F.9 gives
\((r_0,r_1,r_2,r_3)=(1,0,0,-1)\). The resulting
projections are exactly

\[
 P_SQ_*=\frac13I_6,
\]

\[
 \operatorname{diag}(P_{T_d}Q_*)
 =\left(\tfrac12,\tfrac12,0,0,-\tfrac12,-\tfrac12\right),
\]

\[
 \operatorname{diag}(P_{W_d}Q_*)
 =\left(\tfrac16,\tfrac16,-\tfrac13,-\tfrac13,
          \tfrac16,\tfrac16\right).
 \tag{CT.7}
\]

For the shared-index block \((i,j;k,l)=(1,2;0,3)\),
pair antisymmetry gives

\[
 x=Q_{10,20}=Q_{01,02}=1,
 \qquad y=Q_{13,23}=0.
\]

The two projections are \((1/2,1/2)\) and
\((1/2,-1/2)\), respectively. The off-diagonal
Frobenius factor of two is retained. As a useful
normalization check, the squared projection norms are

\[
 \bigl(\|P_hQ_*\|_E^2\bigr)_{h=S,T_d,W_d,T_o,W_s}
   =\left(\tfrac23,1,\tfrac13,1,1\right).
 \tag{CT.8}
\]

Their sum is four, equal to \(\|uu^t\|_E^2\).
No sign or off-diagonal normalization ambiguity
remains in these five channels.

### 4.2 The actual smearing preserves each vector

The leading tensor is constant over the positive
lobe, so

\[
 a^4\sum_xf_\mu(x)\widetilde q_a(x)
 =\epsilon^2c_EQ_*+O(\epsilon^3),
 \qquad c_E=\frac1{m^2}\sum_xf_\mu(x)>0.
 \tag{CT.9}
\]

At a fixed finite cutoff the remainder is uniform
over the finitely many sampled sites. Choosing
\(\epsilon\ne0\) sufficiently small preserves all
five nonzero projected vectors simultaneously.
This proves the witness claim FN.18–FN.23.

## 5. Helical seed, exact clover averaging, and both remaining channels

Use integer spatial coordinate \(z\), set
\(q=2\pi/J\in(0,\pi)\), and take

\[
 A_0=A_3=0,\qquad
 A_1=h_t\cos(qz)\mathsf H,\qquad
 A_2=h_t\sin(qz)\mathsf H,
\]

\[
 h_t=\frac{\sinh(\rho(m-t))}{\sinh(\rho m)},
 \qquad \cosh\rho=1+2\sin^2(q/2).
 \tag{CT.10}
\]

\[
 d_th=\frac{h_{t+1}-h_{t-1}}2
 =-\frac{\sinh\rho\cosh(\rho(m-t))}{\sinh(\rho m)}<0.
 \tag{CT.11}
\]

Combining (CT.2)–(CT.3) with the centered spatial
trigonometric differences yields

\[
\begin{aligned}
 C_{01}&=\epsilon d_th\cos(qz)\mathsf H+O(\epsilon^2),\\
 C_{02}&=\epsilon d_th\sin(qz)\mathsf H+O(\epsilon^2),\\
 C_{23}&=-\epsilon h_t\sin q\cos(qz)\mathsf H+O(\epsilon^2),\\
 C_{13}&=+\epsilon h_t\sin q\sin(qz)\mathsf H+O(\epsilon^2),\\
 C_{03}&=O(\epsilon^2),\qquad C_{12}=O(\epsilon^2).
\end{aligned}
 \tag{CT.12}
\]

In particular, the magnetic multiplier is exactly
\(\sin q\), rather than the forward-difference
modulus \(2\sin(q/2)\). The latter enters the
Dirichlet difference equation, while the former
enters the site-centered clover. Both are retained
in their correct places.

F.13 defines the oriented disjoint coordinates as

\[
 p_1=q_{01,23},\qquad p_2=-q_{02,13},\qquad p_3=q_{03,12}.
\]

Thus, with
\(k_t=-a^{-4}h_td_th\sin q>0\) for
\(1\le t\le m-1\),

\[
 (p_1,p_2,p_3)
 =\epsilon^2k_t(\cos^2(qz),\sin^2(qz),0)
       +O(\epsilon^3).
 \tag{CT.13}
\]

The sign in \(p_2\) is essential and has been
included. The leading \(p_3\) is zero. Its actual
error is at most \(O(\epsilon^4)\) from the displayed
clover orders, so the weaker \(O(\epsilon^3)\) used
in FN.33 is valid. The scalar repair is diagonal
and leaves all three coordinates unchanged exactly.

### 5.1 Positive smearing prevents cancellation

Define the leading smeared coefficients

\[
 K_1=a^4\sum_x f_\mu(x)k_t\cos^2(qz),\qquad
 K_2=a^4\sum_x f_\mu(x)k_t\sin^2(qz).
\]

All sampled roots lie strictly between the two
planes. Therefore \(k_t>0\) on every root with
positive weight, and

\[
 K_1,K_2\ge0,\qquad
 K:=K_1+K_2=a^4\sum_x f_\mu(x)k_t=c_H>0.
 \tag{CT.14}
\]

The leading smeared disjoint vector is
\((K_1,K_2,0)\). Its pseudoscalar projection is
\((K/3,K/3,K/3)\). Its disjoint Weyl projection
has third coordinate \(-K/3\). Both are nonzero
for every nonempty positive sampling of the
original lobe, independently of its spatial
phase relative to the helical mode.

The corresponding Frobenius norm checks are

\[
 \|P_P(K_1,K_2,0)\|_E^2=\frac23K^2,
\]

\[
 \|P_{W_p}(K_1,K_2,0)\|_E^2
 =2\left(K_1^2+K_2^2-\frac{K^2}{3}\right)
 \ge\frac13K^2>0.
 \tag{CT.15}
\]

These norms include both symmetric off-diagonal
matrix entries. Alternatively, the single
zero-sum test vector \((1,1,-2)\) in the
disjoint-coordinate representation has strictly
positive contraction with the leading vector,
which directly detects \(W_p\).

At fixed cutoff the positive coefficient \(K\)
may be very small. This is harmless for the
qualitative argument: choose a sufficiently
small fixed \(\epsilon\), depending on that
cutoff, to dominate the higher-order remainder.
No uniform scale estimate follows from this
choice.

## 6. The sampled-lobe condition and final implication

The original bump is strictly positive when
\(|\mu x-e_0|<\varepsilon_f\), with
\(\varepsilon_f=1/64\). A nearest temporal
lattice vertex to \(1/\mu\), with the three
spatial coordinates zero, is at distance at
most \(a/2\) from the center. Therefore, for
example, the added condition
\(a<\varepsilon_f/(2\mu)\) guarantees a
strictly positive sampled weight. The torus
and half-space margins in FN.1 keep this
vertex and all relevant stencils away from
the seams and reflecting planes.

Without nonempty sampling, every smeared vector
could be zero even if the continuum bump is
nonzero. That issue is now excluded explicitly.

For each witness, the actual classical
minimizer has the displayed nonzero smeared
channel vector. FN.4 then passes this value
through the actual compact conditional law
as \(\beta\to\infty\). The full-law centering
term tends to zero because all F01 plaquette
stencils vanish on every flat torus
configuration, including those with
nontrivial global holonomies. Continuity in
the plane links converts the boundary
witness into a nonzero conditional mean on
a set of positive plane-marginal probability.
The original reflected square is consequently
strictly positive.

The electric and helical witnesses can use
different small amplitudes and different
boundary configurations. Their two finite
large-\(\beta\) thresholds have a finite
maximum at each fixed cutoff. This is exactly
the qualitative seven-channel conclusion
needed to show that the finite analytic
determinant is not identically zero on every
admissible sufficiently fine geometry.

The finite-cutoff implication uses the actual F01 smearing and the nonempty-lobe condition. The argument supplies
no logarithmic coefficient budget or
cutoff-uniform distance from degeneracy.
