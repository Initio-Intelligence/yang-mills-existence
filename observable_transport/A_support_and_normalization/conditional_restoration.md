# Conditional restoration of erased regular fluctuations

This note separates three statements. The finite-dimensional convex-cutoff
restoration lemma is proved without a lower bound on a cutoff probability.
It applies to the complete first ordinary Wilson chart already verified in
RMg, with every original density factor kept. The common quadratic model
also admits a direct two-mask comparison. Applying either argument to the
actual nonlinear last-N history refinement still requires a specified
simultaneous coordinate/energy construction; the separate source bounds
for two histories are not that construction.

The later first-birth factor is treated at the normalization level of LE.4:
the common measure includes the original all-P first integral Z_P(V1).
Nothing below replaces that factor by one or by a new Gaussian normalizer.

## 1. A moment bound on the actual convex cutoff

Let C be a bounded convex product domain in R^n, with 0 in its interior.
Each coordinate block has fixed dimension. Let K be positive definite and
let V be C^2 on a neighborhood of C, with

\[
 \nabla^2V\ge aK,\qquad h=-\nabla V(0),\qquad a>0.
 \tag{CR.1}
\]

Let q be the normalized density 1_C exp(-V). Then, for
0<=theta<=a/4,

\[
 \boxed{\quad
 \log q\exp\{\theta b^T Kb\}
 \le C\theta\left({n\over a}
              +{h^TK^{-1}h\over a^2}\right).
 \quad}                                             \tag{CR.2}
\]

The numerical C is independent of the size of C and its Gaussian mass.
The assertion also holds for an unbounded convex C when the integrals
exist, by exhaustion.

**Proof.** At a regular boundary point of a convex domain containing zero,
b dot n is nonnegative. The divergence theorem applied to b exp(-V)
gives

\[
 q[b\cdot\nabla V]\le n.                             \tag{CR.3}
\]

Approximation by smooth convex domains gives the same inequality for
products of norm balls. No boundary term is silently set to zero. By the
fundamental theorem of calculus and (CR.1),

\[
 b\cdot\nabla V(b)
 \ge a\,b^TKb-h\cdot b
 \ge {a\over2}b^TKb-{1\over2a}h^TK^{-1}h.
\]

Consequently

\[
 q[b^TKb]\le {2n\over a}+{h^TK^{-1}h\over a^2}.
 \tag{CR.4}
\]

For q_t proportional to 1_C exp(-V+t b^TKb), the Hessian lower bound is
(a-2t)K and the gradient at zero is still -h. Apply (CR.4), use
a-2t>=a/2, and integrate
(d/dt)log q exp(t b^TKb)=q_t[b^TKb] from zero to theta. This proves
(CR.2). All normalizers are those of the stated cutoff measures. The
argument does not divide by the probability of C. Square completion or
a shift of C is unnecessary. QED.

The same proof allows an arbitrary convex domain containing zero, not
only a product. The product form matters for the actual source interface
and for conditioning a subset of its independent free coordinates.

## 2. Exact Gaussian Schur restoration

Write the common quadratic variables as (u,b), and suppose

\[
 mI\le
 \mathcal K=\begin{pmatrix}K_{UU}&K_{UB}\\K_{BU}&K_{BB}\end{pmatrix}
 \le MI .                                           \tag{CR.5}
\]

The constants here belong to the specified common normalized coordinate
system. They must not be inferred for an arbitrary badly conditioned
change of basis. Define

\[
 S_U=K_{UU}-K_{UB}K_{BB}^{-1}K_{BU},\qquad
 E_U(u)={1\over2}u^TS_Uu,\qquad
 m_B(u)=-K_{BB}^{-1}K_{BU}u.
 \tag{CR.6}
\]

Restore b on its same centered convex product cutoff C_B. Its exact
conditional density is proportional to

\[
 1_{C_B}(b)\exp\{-\tfrac12 b^TK_{BB}b-b^TK_{BU}u\}.
 \tag{CR.7}
\]

It includes its complete cutoff normalizer. Applying (CR.2), with
h=-K_BU u, gives

\[
 \log q_u\exp\{\theta b^TK_{BB}b\}
       \le C\theta\{|B|+E_U(u)\},\qquad 0\le\theta\le c.
 \tag{CR.8}
\]

Indeed, mI<=S_U<=MI by compression of the inverse matrix, and

\[
 h^TK_{BB}^{-1}h
 \le (M^2/m)|u|^2\le (2M^2/m^2)E_U(u).
 \tag{CR.9}
\]

Thus a normalized reserve for E_U transfers to the joint energy at the
cost exp(C|B|). A restoring block is not charged a P^2 cost merely
because its allowed cutoff is P.

There is an exact centered version of the energy identity:

\[
 \tfrac12 (u,b)^T\mathcal K(u,b)
 =E_U(u)+\tfrac12(b-m_B(u))^TK_{BB}(b-m_B(u)).
 \tag{CR.10}
\]

The identity is valid on the cutoff as well as off it; the two terms are
nonnegative. If two histories are represented in one common Gaussian
refinement, completing the square in either order gives the same left
side. Hence one must apply the argument to the joint refinement once.
Repeatedly replacing an energy by a constant multiple at N consecutive
steps would generate an unnecessary C^N and is not justified by this
note.

A t-test given by a linear functional ell of the common coordinates
has the deterministic bound

\[
 |\ell(u,b)|^2\le
 2(\ell\mathcal K^{-1}\ell^T)
          \tfrac12(u,b)^T\mathcal K(u,b).
 \tag{CR.11}
\]

Consequently a threshold p1 and a variance bound
ell K^{-1}ell^T<=C R^9 give the desired energy threshold
c p1^2/R^9. The covariance, coordinates and positive form in this
statement must all belong to the same refinement.

## 3. A sharper flat Gaussian comparison of convex quiet masks

There is a useful argument which avoids restoring a large list
explicitly in the common quadratic model. Let mu be the centered Gaussian
on the actual linear physical quotient after the common retained
constraints have been imposed. A fixed linear gauge can be used to
identify this quotient with R^d; its covariance is denoted C. Degenerate
ambient coordinates are first restricted to this quotient.

Let G be any centrally symmetric convex set of positive mu mass.
For every real linear functional ell and every real t,

\[
 \boxed{\quad
 \mu(e^{t\ell z}\mid G)
       \le \exp\{t^2\ell C\ell^T/2\}.
 \quad}                                             \tag{CR.12}
\]

**Proof.** Approximate 1_G by even convex barriers exp(-V_n). The potential
has Hessian at least C^{-1}. Its covariance, including after adding the
linear tilt t ell z, is bounded by C. One direct proof of that covariance
inequality is the Poisson/Bochner argument in ST.4, applied to the tilted
potential. Therefore the second derivative of the log moment-generating
function is at most ell C ell^T. Its value and first derivative at zero
are zero; the latter uses the central symmetry of G. Integrating twice
and passing to the hard-domain limit gives (CR.12). This proof keeps the
actual conditional normalization and requires no positive lower bound
on mu(G). QED.

For a linear vector Lz with LC L^T<=I_n, the Gaussian auxiliary-integral
identity and (CR.12) imply

\[
 \mu(e^{\theta|Lz|^2}\mid G)
       \le (1-2\theta)^{-n/2},\qquad 0\le\theta<1/2.
 \tag{CR.13}
\]

No independence of the entries of Lz is asserted. In particular a rank-n
orthogonal Gaussian projection of erased annular data has an exp(Cn)
quadratic reserve under every centered convex quiet mask.

Now let G_s and G_t be two centered convex quiet masks on this same
Gaussian fiber. Suppose G_t is an intersection of m_t linear norm tests
with thresholds a_{t,j}, where every scalar component of the jth test
has Gaussian variance at most v_{t,j}. Fixed-dimensional Euclidean nets
or coordinate norm equivalence give

\[
 \mu(G_t^c\mid G_s)
 \le C\sum_{j=1}^{m_t}
        \exp[-c a_{t,j}^2/v_{t,j}]=:\eta_{s,t}.
 \tag{CR.14}
\]

One can omit all tests that are literally already implied by G_s.
If the same bound is at most eta<1 in both directions, positivity gives

\[
 1-\eta\le {\mu(G_s)\over\mu(G_t)}
                 \le (1-\eta)^{-1}.
 \tag{CR.15}
\]

Both measures are compared through the identical intersection. This is
an exact relative estimate, irrespective of how small their separate
masses are.

### Source meaning of the quadratic statement

At zero retained field, freeze each source geometry and take its actual
quadratic limit. Block averages, local minimizing maps, the relative
fluctuation maps, and a fixed axial/tree gauge are linear maps on one
physical Gaussian quotient. Every **good** ordinary or preparatory
norm test is then a centered convex condition. The first bad R event
must already have been removed to the explicit first-birth factor; it
is not a convex condition and is not included in G_s here. The source's
fresh residual selector is fixed with the retained output and is not
an additional condition on these old Gaussian variables.

The bounds for a test row must be checked on this same physical Gaussian
fiber. LFR II (1.77)--(1.78), after the flat quadratic specialization,
gives exactly the required polynomial control for the mixed preparation
bond test: its square is bounded by C R^9 times the positive quadratic
energy. The first case on pp.381--382 gives the corresponding bound for
the finest annular bonds using the physical curvature. The ordinary
fluctuation tests have the source blocked Gaussian covariance bound.
All these statements concern the literal fixed geometry and normalized
scale of each tested variable.

Thus, for any specified finite collection of those tests for which
these row bounds have been verified, (CR.14) yields

\[
 \eta\le C m\exp[-c p_1(g)^2/R^9].                 \tag{CR.16}
\]

For a simultaneous annular list of rank and test count O(R^5), the source
strict logarithmic hierarchy makes this tend to zero. If one uses the
entire finite common path instead, its actual number of tests must be
kept in m. In particular no total-volume-uniform assertion follows by
silently replacing a global test count by O(R^5). Proving that the two
actual history masks differ only by a specified finite collection, or
controlling the tails of nonidentical distant test maps, remains part of
constructing the common refinement.

## 4. Actual Wilson extension for one regular source layer

The RMg first-step theorem supplies an actual regular conditional
chart, not merely its quadratic limit:

\[
 d\mu_V(z)\propto 1_{\mathcal C}(z)
       \exp\{-\tfrac12 z^TK(V)z+W_V(z)\}\,dz,
 \tag{CR.17}
\]

where C is the SAME product of source free-coordinate balls used in that
theorem. K has uniform gap and upper bound, and the complete W includes
Wilson, soft gauge, Haar, coarea and the exceptional-coordinate Jacobian.
On a fixed-factor larger analytic domain RMg proves

\[
 \sup_i |\partial_iW|\le\epsilon_1=C(gP^2+g^2P),\qquad
 \sup_i\sum_j|\partial_i\partial_jW|
       \le\epsilon_2=C(gP+g^2).
 \tag{CR.18}
\]

Condition on the complement u of any finite independent-coordinate set B,
without changing its product cutoff. For small enough g the conditional
potential V_u(b) satisfies

\[
 \nabla_b^2V_u\ge\tfrac12 K_{BB},\qquad
 h=-K_{BU}u+\partial_BW(0,u).
 \tag{CR.19}
\]

The source gap and (CR.18) give

\[
 h^TK_{BB}^{-1}h
 \le C\,u^T S_Uu+C|B|\epsilon_1^2,
 \tag{CR.20}
\]

with the same Gaussian Schur matrix S_U as in (CR.6). Hence (CR.2) proves

\[
 \boxed{\quad
 \log \mu_V\bigl(e^{\theta b^TK_{BB}b}\mid u\bigr)
       \le C\theta\{|B|+u^TS_Uu\},
 \qquad 0\le\theta\le c.
 \quad}                                             \tag{CR.21}
\]

The harmless term |B|epsilon1^2 has been absorbed since epsilon1 tends
to zero. This is a quantitative **actual one-layer conditional
restoration** estimate. It is uniform in the outside cutoff mass, in the
total volume, and in the admitted real native background of the
first-step chart. It leaves every density and normalization factor in
place. It does not require reflection symmetry of the Wilson correction.

If the conditioned outside energy is itself given a normalized exponential
reserve, (CR.21) transfers that reserve to the restored variables with a
cost exp(C|B|), exactly as in (CR.8). This last statement requires the
outside reserve for the displayed energy; it is not a claim that an
arbitrary inherited scalar supplies one.

## 5. Why this does not yet identify the complete nonlinear refinement

For two distinct source histories, the additional t-annular variables are
not automatically a subset of one final s chart. They may have been
integrated out in an earlier ordinary step. Conditional restoration must
undo those precise integrations, including their group constraints,
Haar/coarea factors, gauge choices, cutoff completion terms and all
E/B/R pieces. FR.2 excludes direct first-A0 dependence at h=1, but does
not make the later density a product of independent normalized Gaussians.

There is a concrete reason the original finite s energy alone is
insufficient. In the quadratic limit, take a physical, zero-block-average
ordinary fluctuation in a fine annular block read by t but already regular
and integrated out for s. Its amplitude can lie between the preparation
threshold p1 and the ordinary R threshold P, since p1<<P. Its higher
averages vanish. It can therefore fail t's preparation norm test while
leaving the surviving s variables, their final positive energy, and all
s ordinary good tests unchanged. The missing energy is the energy of the
erased fluctuation itself. This observation is not a counterexample to
the conditional probability estimate: (CR.8), (CR.13) or (CR.21) is the
mechanism that would pay that fluctuation after it is restored.

To apply CR.21 through a full last-N actual history, one must exhibit a
joint normalized chart for the needed restored variables whose complete
conditional Hessian and force obey the stated uniform bounds, or prove
a joint energy comparison with the same strength. Applying the separate
one-layer bounds successively with unrestricted constants would produce
C^N. The quadratic identity (CR.10) avoids that loss at the Gaussian
level; it does not by itself control the accumulated nonlinear maps and
Jacobian terms. Similarly, actual nonlinear quiet cutoffs are not known
to form a convex set in one common coordinate system, so CR.12 is not
asserted for them.

A valid actual refinement with rank O(R^5), a fixed joint reserve, and the
source threshold implication gives the desired estimate immediately from
LE.17:

\[
 \nu_s(H_t^c)\le
       \exp\{C D_{\rm late}-c p_1(g)^2/R^9\}=o(1).
 \tag{CR.22}
\]

Together with its reverse, the exact intersection identity compares the
common later masses; RB then reinstates equal flat first-birth weights.
The unresolved step is the actual joint nonlinear source interface, not
an inverse rare-event normalization or the Gaussian cutoff probability.

## Source and comparison record

- CMP119 (1.14)--(1.30): exact independent chart, constraint Jacobian,
  complement integration, and retained Schur form.
- LFR I pp.195--199, (1.81)--(1.98): literal mixed annular variables,
  fixed tree, preparation cutoff and old-core seam.
- LFR II pp.380--383, (1.77)--(1.78): actual positive forms and the
  smallest preparation failure penalty.
- RMg.1--RMg.35: complete first ordinary normal form, convex-product
  domain, derivative rows, and native local precision comparison.
- LE.4--LE.19: common first baseline and matched later-only reserve.
- ST.4: convex-barrier covariance proof; FR.1--FR.8: exact common
  primitive readout and the h=1 first-fluctuation independence.
