# A quadratic gauge projector with an actual low-momentum gain

The fixed finite-probe projector SE is a bounded scalar/identity
extraction. It does not annihilate the physical marginal Taylor jet of
every field in its domain. This note supplies a different, explicitly
defined projector at the quadratic level and proves its scaling gain.
It is an elementary lattice Ward-identity argument, not a claim of a new
general classification theorem.

The assertion is for a translation-invariant exponentially local
quadratic action on the infinite homogeneous lattice, or for a family
proved to be its compatible periodizations. It is not inferred for a
sharp-Q branch whose requisite second derivatives or infinite-volume
quadratic kernel have not been constructed. The distinction is part of
the statement.

A local microscopic insertion has an additional source-position
dependence. Translation invariance of the integrated action treats only
its zero source momentum. The local marked application also needs the
source-anchor moments and the appropriate higher nonabelian Ward
identities; they are not supplied merely by the quadratic projector.

## 1. Exact assumptions and edge-centered Fourier variables

Rescale the lattice spacing to one temporarily. Let `A_mu(n)` be a real
Lie-algebra variable on the oriented edge from n to `n+e_mu`, with its
Fourier coordinate located at the edge center `n+e_mu/2`. The Lie algebra
is `su(N)` with a fixed positive invariant inner product. Consider

\[
 \mathcal Q_K(A)=\frac12\sum_{n,m\in\mathbb Z^4}
    \sum_{\mu,\nu=1}^4
       \langle A_\mu(n),K_{\mu\nu}(n-m)A_\nu(m)\rangle .
 \tag{WQ.1}
\]

Initially A has finite support. Assume:

1. The real kernel defines a self-adjoint quadratic form and is invariant
   under simultaneous global adjoint colour rotations.
2. It is invariant under lattice translations and the full hypercubic
   group, including coordinate reflections, with edges transforming as
   oriented vectors.
3. It has a positive exponential locality radius. In edge-center
   displacements, for some `rho>0`,

\[
 \|K\|_\rho:=max_\mu\sum_{\nu,z}
   e^{\rho|z+(e_\mu-e_\nu)/2|_1}
                     \|K_{\mu\nu}(z)\|<\infty.
 \tag{WQ.2}
\]

4. Its exact quadratic gauge identity is
   `Q_K(A+d omega)=Q_K(A)` for every finitely supported A and omega,
   where `(d omega)_mu(n)=omega(n+e_mu)-omega(n)`.

The last assumption follows for the Hessian of an analytic
gauge-invariant action at the identity, provided that Hessian and its
locality have actually been constructed. Its first derivative at the
identity is zero: a linear colour functional invariant under every
adjoint rotation on the simple Lie algebra vanishes. Differentiating
the gauge invariance once in a gauge direction and once in an arbitrary
field direction then makes the Hessian annihilate `d omega`. This
argument requires the stated differentiability; a Lipschitz branch
cannot be substituted for it.

Global colour invariance makes the kernel scalar in colour. One way to
see this is to complexify the commuting coefficient operator: invariant
subspaces of the adjoint representation of the simple complex Lie
algebra are ideals, so the adjoint representation is irreducible and
its commutant consists of scalars. The real structure gives a real
scalar coefficient. We suppress that common colour identity below.

The edge-centered multiplier is

\[
 \mathscr K_{\mu\nu}(p)
   =\sum_z e^{-ip\cdot[z+(e_\mu-e_\nu)/2]}
                      K_{\mu\nu}(z),\qquad
 \widehat p_\mu=2\sin(p_\mu/2).
 \tag{WQ.3}
\]

With this convention the Fourier multiplier of d is `i hat p`. The
quadratic gauge identity and absolute Fourier convergence imply

\[
 \mathscr K(p)\widehat p=0.
 \tag{WQ.4}
\]

This is an identity for every real p, not just a fixed finite set of
torus momenta. It extends locally to complex p by analyticity. The
hypercubic covariance is

\[
 \mathscr K(Rp)=R\mathscr K(p)R^T
 \tag{WQ.5}
\]

for signed permutation matrices R. Edge-centering is necessary to avoid
discarding orientation-dependent phase factors in this formula.

Exponential locality implies analyticity on a complex momentum strip
and bounded derivatives of any fixed order on a smaller strip. For
example, the sum of absolute fourth-derivative coefficients is bounded
by `C_rho ||K||_rho`, since
`sup_{u>=0} u^4 exp(-rho u/2)<infinity`. The same statement holds for
orders zero through four. These are actual kernel moment estimates.

## 2. The marginal quadratic coefficient is unique

### Lemma WQ.1

Under the preceding assumptions there is one real number `c_K` such
that, as p tends to zero,

\[
 \mathscr K_{\mu\nu}(p)
   =c_K\bigl(|p|^2\delta_{\mu\nu}-p_\mu p_\nu\bigr)
       +O(C_\rho\|K\|_\rho|p|^4).
 \tag{WQ.6}
\]

For any distinct mu and nu,

\[
 c_K=\frac12\partial_{p_\nu}^2
                         \mathscr K_{\mu\mu}(0),
 \qquad |c_K|\le C_\rho\|K\|_\rho.
 \tag{WQ.7}
\]

**Proof.** Taking p along each coordinate axis in WQ.4 and letting it
approach zero shows that every column of `K(0)` is zero. Hence the
constant term vanishes. Taking `R=-I` in WQ.5 gives `K(-p)=K(p)`, so
all odd homogeneous Taylor terms vanish.

For a diagonal entry, reflection in each axis makes it even in that
coordinate. Permutation covariance then makes its quadratic part

\[
 [\mathscr K_{\mu\mu}]_2
       =a p_\mu^2+b\sum_{\nu\ne\mu}p_\nu^2.
 \tag{WQ.8}
\]

For an off-diagonal entry, reflection in mu or nu makes it odd in that
coordinate; the remaining reflections make it even in the other
coordinates. Its quadratic part is consequently

\[
 [\mathscr K_{\mu\nu}]_2=c p_\mu p_\nu,
       \qquad\mu\ne\nu,
 \tag{WQ.9}
\]

with the same constants in every coordinate pair. Self-adjointness,
reality and inversion covariance make this real symmetric at real p.

Since `hat p=p+O(|p|^3)`, the degree-three term of WQ.4 is

\[
 a p_\mu^3+(b+c)p_\mu\sum_{\nu\ne\mu}p_\nu^2=0.
 \tag{WQ.10}
\]

Thus a is zero and c is minus b. Set `c_K=b`. The uniform
fourth-derivative estimate and the absence of degrees zero, one and
three give the fourth-order Taylor remainder in WQ.6. WQ.7 follows
from WQ.8 and the second kernel moment bound. The argument is linear
in K. No positivity of K is needed. \(\square\)

The full reflection group matters. If fewer symmetries are imposed,
additional tensor channels must be retained rather than silently folded
into one scalar coefficient.

## 3. An exact lattice projector and its remainder

Let the unit-normalized lattice Wilson/Maxwell multiplier be

\[
 \mathscr K_W(p)=|\widehat p|^2I
                         -\widehat p\widehat p^T.
 \tag{WQ.11}
\]

This is the Hessian of the sum of squared oriented plaquette curls,
with the normalization of WQ.1. It is finite range, has the stated
symmetries, and annihilates `hat p` exactly. Its coefficient in WQ.7
is one. Define

\[
 \Pi_{\mathrm{quad}}K=c_KK_W,\qquad
 R_K=K-c_KK_W.
 \tag{WQ.12}
\]

This is a linear idempotent projector on the specified quadratic class.
For a fixed rho its norm is bounded, since WQ.7 bounds `c_K` and `K_W`
has fixed finite support. The remainder satisfies the exact Ward
identity and

\[
 \|\mathscr R_K(p)\|_{\mathrm{op}}
        \le C_\rho\|K\|_\rho|p|^4
       \quad (|p|\le p_*),
 \tag{WQ.13}
\]

where `p_*>0` is a fixed sufficiently small number.

The stronger energy form is useful. For real `p!=0` let P be the
orthogonal projection onto `hat p`-perpendicular vectors. Hermiticity
and the exact Ward identity give `R_K=P R_K P`. Moreover

\[
 v^*\mathscr K_W(p)v=|\widehat p|^2|Pv|^2.
 \tag{WQ.14}
\]

On the fixed small momentum ball, `|hat p|` and `|p|` are comparable.
Therefore WQ.13 implies

\[
 \boxed{\quad
 |v^*\mathscr R_K(p)v|
  \le C_\rho\|K\|_\rho |p|^2
                         v^*\mathscr K_W(p)v.
 \quad}
 \tag{WQ.15}
\]

At zero both sides vanish. Colour components are summed with the same
positive invariant inner product. The estimate also follows for a
general self-adjoint remainder of either sign; a positivity claim for
that remainder is not required.

## 4. A genuine two-power gain, with its proper domain

Restore the lattice spacing h. Let A be square summable with Fourier
support in `|p|<=h/H`, where `H>=h/p_*`. Fourier Plancherel and WQ.15
give

\[
 \boxed{\quad
 |\mathcal Q_{R_K}(A)|
   \le C_\rho\|K\|_\rho (h/H)^2
                            \mathcal Q_{K_W}(A).
 \quad}
 \tag{WQ.16}
\]

Common physical factors of h and coupling are kept identical on both
sides and cancel in this ratio. The extension from finite support to
these square-summable fields follows from boundedness of the
translation-invariant kernels. An exactly band-limited nonzero field
need not have finite spatial support; the proof does not require both.

This is an actual low-momentum gain after subtracting the physical
quadratic marginal coefficient. It is not a small bound on arbitrary
native field configurations. High lattice momenta are present in the
ordinary M03 supremum, so WQ.16 cannot be substituted for a full carrier
norm contraction without an actual reconstruction/smoothing theorem.

For compatible periodizations, the same argument applies on the
available discrete momenta. An arbitrary single finite-torus kernel is
not automatically such a periodization. In particular, discrete Ward
identities at finitely many momenta alone do not determine derivatives
at zero of an unspecified interpolation. Winding/holonomy terms require
their own treatment.

## 5. Relation to the finite-probe example

Use the exact repaired F01 scalar `phi_h=beta_h sigma_h` from SE.1.
Its lattice sum is a fixed multiple of the Wilson action. Define

\[
 (\mathsf T\phi_h)(x)
   =\frac18\sum_{\mu=1}^4
       [\phi_h(x+he_\mu)+\phi_h(x-he_\mu)].
 \tag{WQ.17}
\]

Periodic summation gives `sum_x T phi_h=sum_x phi_h` exactly. The
translation-summed quadratic action consequently has physical
coefficient `c_K=1` in Wilson units. The finite-pulse probe instead
returns `a_SE(T phi_h)=1/4`: its anchor sees six nontrivial plaquette
occurrences, whereas the eight neighboring anchors see twelve in
total. Hence its complement retains three quarters of that marginal
action. The separate finite-probe scaling note gives the complete count
and the exact discrete-Laplacian decomposition.

The projector WQ.12 removes that quadratic marginal term. In this
example the correctly normalized local difference is
`T phi_h-phi_h`, whose lattice sum is zero and whose smearing has the
two-power estimate proved in that companion note. That smearing
estimate and WQ.16 have different hypotheses: one controls a slowly
varying test against a density, and the other controls a quadratic form
on low-momentum fields. Neither is asserted to be the full microscopic
M03 operator estimate.

## 6. The actual Yang--Mills application still to be proved

This lemma specifies an appropriate quadratic extraction once an actual
analytic, gauge-invariant, exponentially local Hessian is available.
For the continued source program the remaining application must prove
all of the following from its own physical integral representation:

* existence of the needed quadratic field jet with its common supported
  kernel and first-current compatibility;
* the Ward and full scalar symmetry identities in that same family,
  including any boundary-sector recombination required for smoothness;
* a uniform kernel moment/tube bound and consistent thermodynamic
  interpretation, rather than an arbitrary finite-torus interpolation;
* the nonlinear remainder and its actual reconstruction or smearing
  estimates, in the norm required downstream;
* uniform treatment of the vacuum, marginal coefficient and inherited
  rare components through the complete density recursion.

TC supplies a fixed-depth analytic comparison and keeps sharp-Q
corrections as real-domain integral payloads. It does not by that fact
alone supply all these quadratic jets for the full branch. The actual
continuum construction is not concluded here. The useful change is that
the desired marginal coefficient and the precise two-power estimate are
now explicit, rather than being conflated with SE's bounded finite-probe
complement.

Companion definitions: [scalar extraction](../A_support_and_normalization/scalar_extraction.md), SE.1--SE.11;
[M04 Finite Probe and Engineering Jet Gate](../E_limits_and_targets/M04_Finite_Probe_and_Engineering_Jet_Gate.md), EJ.6--EJ.25;
[M04 Three Step Regular Density and Scalar](../B_finite_depth/M04_Three_Step_Regular_Density_and_Scalar.md), TS.22--23;
[M04 Coarse Carrier Contraction](../C_quadratic_transfer/M04_Coarse_Carrier_Contraction.md), CC.14--21. The classification and
Fourier estimates WQ.6--16 are proved in this note.

Primary comparison source: Bałaban, CMP 109 (1987), Section 5,
especially (5.21), (5.34)--(5.42), obtains its polarization coefficient
from gauge identities and derivatives at zero momentum. Equations
(5.43)--(5.44) and printed p.298 distinguish the remaining derivative
terms and the subsequent localization problem. WQ is a self-contained
quadratic argument in the edge-centered convention above; it does not
replace that source's complete nonlinear action analysis.
