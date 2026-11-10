# Proper-mesh coordinate counts, common positive domination and native jets

## Scope

The main body of this note treats the native side of the C05
boundary estimate independently of the positive-catalog closure. It supplies an
explicit proof of the normalization step, identifies the exact
primary-source geometry it uses, and separates that geometry from a false
argument for arbitrary branching prefixes. Section 10 separately checks
the positive transfer PC.6–PC.6a of
[Coarsened protected atoms and the positive catalog](positive_catalog_coarsening.md).
Throughout, Q denotes [Positive attachment bounds and the quotient forest](quotient_forests.md),
M denotes [Majorants for marked atoms and composition of prefixes](marked_atoms.md),
and S denotes [Summable reserves in the native norm](summable_reserve.md).

The following are distinct assertions.

1. The source operation admits a bounded, componentwise rectangular
   preparation sequence on every component to which the preliminary
   R operation is applied.
2. That geometry gives a polynomial number of actual integration
   coordinates, on their respective meshes, through one whole prefix.
3. The complete ordinary source action on those coordinates has a
   uniformly small complex phase on the enlarged native contour.
4. The phase bound gives a common positive dominating probability
   measure on the working contour.
5. The same measure preserves a positive catalog whose native
   supremum is inside its coefficient sum.

Assertions 2, 4 and 5 are proved explicitly below. Assertion 3 uses
the complete ordinary source estimates and their actual E subtraction,
not a Gaussian replacement. Assertion 1 must be read as a fact about
the printed source operation, using the componentwise convention on
LFR I p.177 and the actual nested domains on pp.192 and 195. It does
not follow merely by bounding each member of an arbitrarily branching
ancestral family.

No conclusion in this note removes the separate positive-catalog
obligation for completed relative activities. The note does not by itself
prove C05.

## 1. What the primary text actually supplies

The relevant primary references are:

- Bałaban, *Large field renormalization I*, CMP 122 (1989), 175–202,
  pp.177–180, 188–192 and 195.
- Bałaban, *Large field renormalization II*, CMP 122 (1989), 355–392,
  pp.384–387.
- Bałaban, *Convergent renormalization expansions for lattice gauge
  theories*, CMP 119 (1988), 243–285, pp.259–261 and 275–283.
- Bałaban, *Renormalization group approach to lattice gauge field
  theories. I. Generation of effective actions in a small field
  approximation and a coupling constant renormalization in four
  dimensions*, CMP 109 (1987), and its cluster-expansion sequel
  in CMP 116 (1988), 1–22, especially (1.24)–(1.36).

LFR I p.177 specifies an eligible component by (i) its containment
in a cube of side \(100MR_k\), and (ii) the last \(N\) steps and the
corresponding size conditions on the preceding regions. Immediately
afterward it states the rectangular-parallelepiped property for
the regions connected with those last \(N\) steps. It then adopts
the convention \(Z_j=Z_j\cap Z\) and factors the operation over
selected current components in (1.1).

There are two useful subsequent checks of what construction that
assertion means. LFR I p.192 identifies the final region \(Z_k''\)
and \(\Lambda\) as rectangular parallelepipeds. Page 195 says that
the gauge construction makes essential use of the nested rectangular
sequence
\[
 \Lambda\supset Z_k''\supset\cdots\supset Z_{h+1}'',
 \qquad h=k-N.
 \tag{ND.1}
\]
The construction is componentwise in the factorization (1.1).

The weaker sentence on p.179 that all *components* of \(Z_j''\)
are rectangular is not, on its own, a bound for their number in one
later component. A proof must retain the actual componentwise
sequence (ND.1). In particular, “each ancestral component is small”
is not an admissible replacement for the source admission statement.

LFR II pp.385–386 independently distinguishes an unchanged
one-predecessor step \(Z=S(Z_0)\), (1.83), a failed preparatory
attempt carrying a new suppression, and a merger of several
preceding components, (1.85)–(1.87). This supports keeping the
component ancestry and failed-attempt records explicitly.
It should not be paraphrased as a theorem that absence of one
particular new selector automatically rules out every merger.

The C05 history class also contains ordinary branching histories.
The preceding rectangular statement concerns only a component
on which the source actually performs the preliminary R sequence.
Unselected regions remain in the exact old operation and in
the exterior data. They are not forced into a single rectangle.

## 2. Proper-mesh coordinate count

Fix one source-admitted attempted component \(P\) at scale \(r\)
and one of its actual stopped preliminary sequences. Write
\(h=r-N_r\). At stage \(j\), the coordinate changes are the ones
in LFR I (1.15)–(1.17), (1.27)–(1.29) and (1.53)–(1.60).
Coordinates not integrated by the chosen prefix, including the
deep \(T_h\) variables, are parameters.

### Lemma ND.1

On the componentwise bounded rectangular sequence used by the
source, the number \(D_j\) of real free coordinates integrated at
stage \(j\) satisfies
\[
 D_j\le C_{\mathrm{coord}}(LMR_{j+1}+1)^4.
 \tag{ND.2}
\]
The constant includes the fixed Lie-algebra dimension, coordinate
types, bonds per site and finite stencil enlargement. It is
independent of \(r-j\), the microscopic volume and the number of
other current components.

**Proof.** The stage-\(j\) variables lie in the actual
\((j+1)\)-region, or in a fixed stencil enlargement of it:
the integration strip is a subset of
\(Z_{j+1}\setminus Z_{j+1}''\), with the corresponding free
constraint coordinates. The admitted preceding rectangle has
side at most \(100MR_{j+1}\) in the \((j+1)\)-mesh.
It therefore has side at most \(100LMR_{j+1}\) in the
\(j\)-mesh. A rectangular subset of that mesh contains at most
\(C(LMR_{j+1}+1)^4\) sites and bonds. Removing dependent
constraint coordinates cannot increase that number.
The free \(A_j\) and \(B_j\) systems contribute a fixed finite
number of coordinates per such site or bond. Fixed boundary
stencils only change the constant. This proves (ND.2).
\(\square\)

The point of (ND.2) is its mesh. Counting the whole outer
\(r\)-component on the \(j\)-mesh would instead introduce
\(L^{4(r-j)}\). That is a different region and does not count
the source's actual stage-\(j\) strip.

Put \(\ell_j=\log g_j^{-2}\). On the finite preparation window
the retained profile comparison gives
\[
 N_r\le C\ell_r^{p_N},\qquad
 R_j\le C R_r\le C\ell_r^{r_0},\qquad
 P_j\le C\ell_r^{p_0}
 \quad(h\le j\le r).
 \tag{ND.3}
\]
Consequently, for every fixed cutoff degree \(d\),
\[
 \sum_{j=h}^{r-1}D_jP_j^d
 \le C\ell_r^{p_N+4r_0+dp_0}.
 \tag{ND.4}
\]
The constants can absorb fixed \(L,M\). A finite number of
stage, localization and recent-birth labels multiplies (ND.4)
by a fixed additional power of \(N_r\).

The top overlap band does not change this conclusion.
LFR I p.192 gives
\[
 L^{N_0-1}=R_{r-N_0+1}
 \le (L+1)(N_0+1)^{\beta_0}R_r.
 \tag{ND.5}
\]
Thus every fixed \(L_0^{cN_0}\) from the actual insertion
map is a fixed polynomial in \(R_r\) and \(N_0+1\).
No exponent in (ND.4) or (ND.5) depends on the analytic
enlargement exponent chosen below.

## 3. The complete ordinary action and its phase

On the actual fixed real coordinate support, write the mark-zero
ordinary density as
\[
 w_\zeta(a)
 =c_\zeta\,{\bf1}_{S}(a)
       \exp[-q_\zeta(a)+V_{\mathrm{exp},\zeta}(a)
                         +V_{\mathrm{ord},\zeta}(a)].
 \tag{ND.6}
\]
Here \(\zeta\) denotes the external native field, independent
current and the permitted new localization parameters.
The tuple \(a\) includes all coordinates integrated by this one
prefix and any internal discrete label that is actually summed
there. Only factors independent of every component of \(a\)
may be put into \(c_\zeta\).

The quadratic \(q_\zeta\) includes the actual Gaussian precision,
principal inverse or Schur block, retained linear force and cross
quadratic terms. Terms coupling distinct attempted components
remain cross interactions before this factorization. The explicit
part includes the real constraint-elimination maps, Haar/coarea
factors, Wilson remainder and failed-relocation Jacobian when
present. This is not a Gaussian comparison law.

The support is fixed only after the source changes of variables:
LFR I (1.27)–(1.29) and the failed-selector relocation (1.59).
Differentiation before that step would differentiate a moving hard
selector and would not prove the native assertion considered here.

Choose once
\[
 \alpha_j^-=c g_j\ell_j^q,\qquad
 \alpha_j^+=\ell_j^{Q_1}\alpha_j^-,
 \qquad
 \alpha_j^{++}=\ell_j^{Q_2}\alpha_j^+.
 \tag{ND.7}
\]
The \(++\) contour is needed only for the independently controlled
ordinary family. It is not a new domain assumed for an unknown
completed relative activity. The latter remains on \(+\).

### 3.1 The E term must be its complete renormalized difference

At one stage, LFR I (1.60) extracts the action evaluated at the
next background. Iterating that exact equality through the
prefix gives
\[
 E_r(U^{[0]}(\zeta,a))
 =E_r(U^{[s]}(\zeta))
   +\sum_{n=0}^{s-1}
       [E_r(U^{[n]}(\zeta,a))
                   -E_r(U^{[n+1]}(\zeta,a))].
 \tag{ND.8}
\]
The first term on the right is independent of the variables
integrated by the prefix and factors out of its normalized
kernel. It remains in the outer action.

Every difference in (ND.8) uses the full source \(E_r\) of
CMP119 (2.25), including each birth's own vacuum and Wilson
subtractions. The vacuum cancels in the difference. The own
marginal curvature coefficient cancels against its own Wilson
term before the old-birth sum. In particular,
\[
 |\beta_b|\le C E_0(\alpha_b^{++})^{-2}
 \tag{ND.9}
\]
is permitted; \(\beta_b=O(1)\) is not required or inferred.

The radius-preserving Ward ledger retains a coefficient of
order \(p\) with its actual field degree \(d\ge p\). Its
schematic bound is
\[
 C E_0(\alpha_b^{++})^{-p}
          (Q_n^{++})^d,\qquad 2\le p\le5,\quad d\ge p.
 \tag{ND.10}
\]
The fifth-order integral remainder has \(p=d=5\). Replacing
every denominator by \((\alpha_b^{++})^{-5}\) and then keeping
only two field powers would be invalid.

The E14 calculation and the source transfer in CMP119
pp.275–277 retain the near-birth gain
\(L^{-(5-\vartheta)(n-b)}\), \(0<\vartheta<1\), after the
own marginal subtraction, and the far-carrier gain
\(e^{-cML^{n-b}}\).
The actual AF comparison gives
\[
 \frac{\alpha_n^{++}}{\alpha_b^{++}}
 \le C\sqrt{1+n-b},\qquad b\le n.
 \tag{ND.11}
\]
Constants in (ND.11) may depend on the once-selected powers.
They do not add a running logarithmic power proportional to
\(Q_2\). After the four-dimensional old-root count, the sums are
bounded by fixed multiples of
\[
 \sum_{a\ge0}(1+a)^{b_*+5/2}
          L^{-(1-\vartheta)a},
 \qquad
 \sum_{a\ge0}\sqrt{1+a}\,L^{3a}e^{-cML^a}.
 \tag{ND.12}
\]
Both converge.

The inherited bank in a stage-\(j\) preparation is \(E_r\),
not \(E_j\). Births \(b>j\) therefore cannot be omitted.
There are at most \(N_r\) such births. Keep each as a whole
proper-scale primitive with its own Wilson term. On a
\(b\)-cell, the curvature clause and the quadratic zero of the
Wilson action give
\[
 |A(\phi_b,U;\text{\(b\)-cell})|
 \le C(\alpha_b^{++})^2,
 \qquad
 |\beta_b A(\phi_b,U;\text{\(b\)-cell})|\le C E_0.
 \tag{ND.13}
\]
The factor \((h_b/\eta)^4\) counting fine plaquettes cancels
the curvature factor \((\eta/h_b)^4\). The source normalized
map row is applied before summing its positions. A stage-\(j\)
endpoint belongs to a bounded number of \(b\)-cells when
\(b>j\). Thus these finitely many later births cost a fixed
power of \(N_r\), not \(L^{4(b-j)}\).

These observations justify the structure of the E contribution
used in the phase calculation. They also identify precisely
which source estimate is needed: the complete pre-integration
renormalized fluctuation family on the external strong \(++\)
contour. A bound only for the final integrated \(C\) coefficient
would not establish this step.

### 3.2 The logarithmic power gained by Cauchy

At a fixed real external center and fixed real tuple \(a\),
the actual source coefficients are real. The specified
independent-current extension commutes with complex conjugation,
because it is built from the real source formulas, real Taylor
operations and the real branch of the logarithm. An arbitrary
holomorphic extension agreeing only on the physical graph
would not suffice.

On the external strong \(++\) contour, the complete composed
ordinary scalar has a summed bound
\[
 \sum_\gamma\sup_{++}|G_\gamma(\zeta;a)|
 \le C(Q_2)\ell_r^{D_0}.
 \tag{ND.14}
\]
The actual integration-root count is (ND.4); ordinary full-tree
root sums and the E sums (ND.12) precede it. The top-band
factor is (ND.5). The finite integer \(D_0\) is fixed before
\(Q_2\).

The source successive-insertion inclusion and the strong-core
map admission put the full composed coefficient, with all
real \(a\) fixed, on this contour. They are used once for
the composition. A fixed Lipschitz loss is not multiplied
once per stage.

Cauchy along the line from the real center to a \(+\) input
therefore gives
\[
 \left|\Im\sum_\gamma G_\gamma(\zeta;a)\right|
 \le C(Q_2)\ell_r^{D_0+D_{\mathrm{map}}-Q_2}.
 \tag{ND.15}
\]
The exponent \(D_{\mathrm{map}}\) is the fixed proper-mesh
map conversion degree. To see that this selection is not
circular, the preparation window has \(N_r\) polynomial in
\(\ell_r\), while \(g_r^{-2}=e^{\ell_r}\). The two-sided
retained profile implies
\[
 \ell_j/\ell_r=1+O(1/\ell_r)
 \quad(r-N_r\le j\le r).
 \tag{ND.16}
\]
For any one fixed \(Q_2\), the corresponding power of this
ratio is bounded after reducing the common ceiling.
There is no factor \(\ell_r^{p_NQ_2}\).

For the Gaussian/Schur and explicit classical terms, retain
their actual fixed absolute coefficient domains. Their
normalized rows, the bounded cutoffs and (ND.4) give
\(C g_r\ell_r^{D_1}\).
New complex localization parameters outside the protected
component collar have their actual walk/connector bound
\(C g_r^{-u}\ell_r^{D_3}e^{-cR_r}\).
Realness at arbitrary complex localizers is not used.

Consequently, after removal of the single \(a\)-independent
phase from \(c_\zeta\), the full ordinary density satisfies
\[
 |\arg w_\zeta(a)|\le\eta_r,\qquad
 \eta_r\le C g_r\ell_r^{D_1}
       +C(Q_2)\ell_r^{D_2-Q_2}
       +C g_r^{-u}\ell_r^{D_3}e^{-cR_r}.
 \tag{ND.17}
\]
Choose \(Q_2>D_2+2\), then reduce the common ceiling.
The result is uniform in every real tuple on the actual
support. It concerns the entire normalized prefix,
not a product of \(N_r\) independently bounded kernels.

## 4. Common positive domination, with a complete proof

### Lemma ND.2

Let \(w_\zeta(a)\) be a holomorphic density on one fixed
measure space and fixed support. Suppose that on a larger
complex parameter domain a scalar phase independent of \(a\)
can be removed so that
\[
 |\arg w_\zeta(a)|\le\eta<\pi/4.
 \tag{ND.18}
\]
At a fixed real center \(0\), suppose \(w_0(a)>0\) on that
support. Set
\[
 Z_\zeta=\int w_\zeta(a)\,da,\qquad
 p_\zeta(a)=w_\zeta(a)/Z_\zeta .
 \tag{ND.19}
\]
On any fixed homothetic smaller domain, with ratio
\(0<q<1\),
\[
 |p_\zeta(a)|
 \le
 \exp\!\left[
   \frac{4\eta}{\pi}\log\frac{1+q}{1-q}
 \right]p_0(a).
 \tag{ND.20}
\]

**Proof.** Rotation by the removed common phase leaves the
normalized density unchanged. The integral belongs to the
same cone as its pointwise integrand, so
\[
 |Z_\zeta|\ge
 \cos\eta\int|w_\zeta(a)|\,da>0 .
 \tag{ND.21}
\]
Thus the normalized density is holomorphic and
\(|\arg p_\zeta(a)|\le2\eta\).
Fix \(a\) and a complex line from the center to the given
parameter point, with parameter \(z\) in a disk of radius
\(R\). The branch
\[
 f(z)=\log[p_z(a)/p_0(a)]
 \tag{ND.22}
\]
is holomorphic, \(f(0)=0\), and
\(|\Im f(z)|\le2\eta\).
For \(\eta>0\), put
\[
 H(z)=\exp\!\left[\frac{\pi}{4\eta}f(z)\right].
 \tag{ND.23}
\]
It has positive real part and \(H(0)=1\). The Cayley
transform \((H-1)/(H+1)\) maps the disk into the unit disk
and vanishes at zero. Schwarz's lemma gives modulus at most
\(q\) on \(|z|\le qR\). Hence
\[
 |H(z)|\le\frac{1+q}{1-q}.
 \tag{ND.24}
\]
Taking logarithms proves (ND.20). The case \(\eta=0\)
follows because a real-valued holomorphic normalized ratio
is constant. Restriction to complex lines proves the same
statement on a Banach ball or a finite polydisc with the
stated fixed homothetic margin. The estimate is independent
of the number of integration coordinates.
\(\square\)

Zero-density pieces outside the fixed support are omitted
from the logarithm and have zero weight in both sides.
Any required local integrability and holomorphy can first
be checked at the finite cutoff and finite support used
by the source.

### Corollary ND.3

Let \(F_G(\zeta,a)\) be a catalog with nonnegative
parameter-independent weights \(w_G\). Its label set can
depend measurably on \(a\); use the union of labels and set
absent coefficients to zero. If
\[
 \sum_G w_G\sup_\zeta|F_G(\zeta,a)|\le K
 \quad\text{for every actual real tuple }a,
 \tag{ND.25}
\]
then
\[
 \sum_G w_G\sup_\zeta
 \left|\int p_\zeta(a)F_G(\zeta,a)\,da\right|
 \le M_{\mathrm{pref}}K,
 \tag{ND.26}
\]
where \(M_{\mathrm{pref}}\) is the exponential constant in
(ND.20).

**Proof.** Apply (ND.20) inside each integral, then the
triangle inequality, the supremum and Tonelli:
\[
 \begin{split}
 \sum_Gw_G\sup_\zeta\left|\int p_\zeta F_G\right|
 &\le M_{\mathrm{pref}}
       \int p_0(a)
          \sum_Gw_G\sup_\zeta|F_G(\zeta,a)|\,da\\
 &\le M_{\mathrm{pref}}K.
 \end{split}
 \tag{ND.27}
\]
The exterior real tuple is fixed throughout this argument.
Its supremum can be taken afterward. No sum of independent
real-raw suprema is asserted.
\(\square\)

This proof permits arbitrary bounded measurable dependence
on integrated old raw coordinates. It does not assume
analyticity in those coordinates. It also retains every
normalizer derivative: all subsequent Cauchy differentiations
act on the complete quotient (ND.19).

The phase estimate needs a fixed larger parameter domain
than the working one. The new localizer disks can be
enlarged by a fixed factor before choosing \(M\) and the
ceiling, using the source walk bound. This is one reserve
chosen for the whole proof, not one reserve lost at every
history step.

## 5. Why the geometry check is essential

There is a concrete obstruction to replacing the preceding
coordinate count by “every fine branch has a small phase.”
Let \(a_1,\ldots,a_n\in\{-1,1\}\), with uniform counting
probability, and define
\[
 w_z(a)=\exp\!\left(\varepsilon z
                      \sum_{\ell=1}^n a_\ell\right).
 \tag{ND.28}
\]
This is an entire density, positive for real \(z\).
Its normalized density at \(z=i\) satisfies
\[
 p_i(a)=
 \frac{\exp(i\varepsilon\sum_\ell a_\ell)}
      {(\cos\varepsilon)^n},
 \qquad
 \int|p_i(a)|\,da=(\sec\varepsilon)^n.
 \tag{ND.29}
\]
Each single branch has an arbitrarily small fixed phase
when \(\varepsilon\) is small, but the normalized operator
norm is unbounded as the branch number grows.
A single bounded test depending on all the coordinates
attains that norm by taking the opposite phase.

Thus neither a branchwise phase estimate nor a bound for
each ancestral component proves one common prefix factor
independent of their number. The source-admitted proper
strip count in Lemma ND.1 is doing actual work. This
example is a diagnostic for an invalid replacement of
that hypothesis; it is not a counterexample to the source
operation on its stated rectangular preparation class.

## 6. Unsubtracted native jets

The native target is not exhausted by differentiating
\[
 B(z,\xi)-B(0,\xi).
 \tag{ND.30}
\]
A term \(H(\xi)\) independent of the new current survives
in the native problem. The final native argument retains
it as follows.

Let the first direction be supported on actual native
cells and measured on the original strong radius
\(\alpha^-\). The ordinary scalar value bound on the
larger \(\alpha^+\) chart can contain one fixed
preparation-overlap polynomial and the explicit
Gaussian \(P_n^2\) factor. It is sufficient to have
\[
 \sum_{G:S_G\cap Q_n\ne\varnothing}
    w_G\sup_+|F_G|
 \le C(B_0+C_0+1)\ell_n^{D_{\mathrm{nat}}}
       +K_{\mathrm{fresh}}.
 \tag{ND.31}
\]
Choose \(Q_1>D_{\mathrm{nat}}\).
On the common multi-parameter Cauchy torus, give the first
native field/current leg its \(\ell_n^{Q_1}\) larger
radius, and give the remaining legs their fixed
joint-slot margins. Componentwise Cauchy followed by the
positive sum gives
\[
 \sum_G w_G
 |D_{h_1}\cdots D_{h_m}F_G|
 \le C^{m+1}m!\,
  (B_0+C_0+1+K_{\mathrm{fresh}})
  N_{\mathrm{nat}}(S_1)
  \prod_{\ell=1}^m\|h_\ell\|_{\mathrm{slot}}.
 \tag{ND.32}
\]
This is a derivative estimate for the unsubtracted
scalar; an extensive or polynomial value constant has
not been discarded.

A purely preparatory first direction does not receive
that gain by renaming it a field direction. Its actual
alternatives are:

- A current localization parameter whose physical
  forcing vanishes at zero new current, on its original
  full disk.
- A genuine failed relocation, whose entire action
  difference and Jacobian have the fresh guarded bound.
- A verified native map \(s\mapsto\Phi_s\), for which
  \[
   D_s(F\circ\Phi_s)=DF(\Phi_s)D_s\Phi_s
   \tag{ND.33}
  \]
  uses the actual native norm and local endpoint row.

Earlier localization integration labels are not
invented as new surviving coordinates. All higher
derivatives of a later nonlinear map remain in the
analytic composition; they are not replaced by the
first derivative (ND.33).

The primary final masses \(T'_b(Y)1\) in LFR II
(1.103)–(1.104) depend on their stated retained raw
arguments. Holding those arguments fixed gives zero
derivative of that factor in the native slots.
This does not remove a native-dependent self term or
normalizer. Its compensating scalar remains in the
unsubtracted action and is included in (ND.31)–(ND.32).

## 7. The four reconstructed outputs and the full current contour

The geometry count above does not replace the native
admission theorem. The composed coefficients must still
meet all of CMP119 (2.34)–(2.39), and their prepared
versions (1.64)–(1.69) in LFR I:

| Output | Required check |
|---|---|
| Original field curvature | Native physical \(h_n^2\) scaling on the actual old layer. |
| Joined reconstructed curvature | Genuine joined determining data and an entire admitted native ball, not only a tangent at the center. |
| Original independent/physical current | Its declared \(h_n^3\) weighting and independent-current extension. |
| Joined reconstructed current | The actual zero-data reconstruction and gauge conversion, with the physical weights retained. |

The map chain uses NP.5, RM.3 and
JI.32–JI.40 for these checks and PF.1 for the prepared
strong core. In that chain the primitive input remains
the smooth field. A potentially spiky axial
representative is used only to identify covariant
auxiliary outputs. Bounded gauge conjugation controls
those curvature and current outputs; it is not a
potential-gradient estimate.

The full current argument then uses the original
unprimed support \(|z_i|\le P_k\) and the common
complex \(2P_k\) contour. It differentiates the complete
normalized scalar after the actual integration.
The Gaussian Schur response retains its \(P_j^2\)
coefficient, and the old scalar value \(B(0,\xi)\)
continues to be covered by the separate native proof.
Current subtraction alone is not the native proof.

## 8. Gaussian localization of a coarsened scalar block

This section supplies the linearity check needed after a cancelled
prefix is kept as one scalar atom. It is important to perform
this operation before choosing a Gaussian conditioning domain
for each separate summand.

### Lemma ND.4 — a common Gaussian localization preserves the block

Fix the actual ordinary current variables \(B\), their source
cutoff, and the actual source map
\[
 \Psi(B,\zeta)=\Psi_0(\zeta)+v(B,\zeta)
 \tag{ND.34}
\]
into a common admitted native chart. Let
\[
 F=\sum_{i=1}^sF_i
 \tag{ND.35}
\]
be an identity of native functions on that chart and on the
common master localization family, not merely at the
unlocalized physical parameter value. Suppose the current
substitution has a fixed relative native margin there, so
the Taylor expansion in \(v\) converges absolutely on the
actual cutoff support.

First expand the whole \(F\) at \(\Psi_0\):
\[
 F(\Psi_0+v)
 =\sum_{p\ge0}\frac1{p!}
                 D^pF(\Psi_0)[v^{\otimes p}].
 \tag{ND.36}
\]
Expand the map factors \(v\) with their actual source
localization. For each fixed product of map records,
choose one Gaussian conditioning set \(Z_0\) containing
its actual \(B\)-dependence and choose one source
parametrix/reference family for that \(Z_0\).
Use that choice for the whole coefficient \(D^pF\).
Then the Gaussian integration, Gaussian localization
and distinguished-insertion normalized expansion are
linear in \(D^pF\), and the identity
\[
 D^pF=\sum_{i=1}^sD^pF_i
 \tag{ND.37}
\]
is preserved coefficientwise by these operations.

**Proof.** Work first at finite volume, finite Taylor
order and finitely many localization records. A term
in (ND.36), after localization of the map factors, is
of the form
\[
 A_F(\zeta)\,K(B,\zeta),
 \tag{ND.38}
\]
where \(A_F\) is a component of \(D^pF(\Psi_0)\).
It is independent of the current integration variables
\(B\), even though it may depend on retained raw
variables and on native/localization parameters.
Thus
\[
 \int d\mu_{C_\zeta}(B)\,\chi(B)
          A_F(\zeta)K(B,\zeta)
 =
 A_F(\zeta)
       \int d\mu_{C_\zeta}(B)\,\chi(B)K(B,\zeta).
 \tag{ND.39}
\]
The cutoff expansion and Gaussian conditioning of
CMP116 (2.3)–(2.6) depend on the chosen
\(B\)-support and on the fixed reference action,
not on the label \(i\) in a later resolution of
\(A_F=\sum_i A_{F_i}\). Choose the special
parametrix domain \(X_0\) of p.13 once for this
support. Every subsequent localization operator
is linear on the product in (ND.39). Its derivatives
may act on \(A_F\) as well as the Gaussian/map
factors; linearity still preserves (ND.37).

For the normalized ordinary expectation, use the
same denominator for all summands. CMP119
(3.44)–(3.47) keeps one distinguished numerator
polymer \(H'\); the ordinary denominator polymers
are the same for each insertion. Their cancellation
and remaining connected expansion are linear in
that distinguished insertion. Therefore (ND.37)
survives this step as well.

Finally, the source absolute Taylor, map and
Gaussian-localization majorants justify the
finite-order and finite-record limits. No new
summation over the old labels \(i\) has been
estimated by separate absolute values: the
coefficient remains \(A_F\). This proves the
claim. \(\square\)

The lemma does **not** say that two different
parametrices, selected independently for two
different historical insertion supports, have
the same localized coefficients. It constructs
one admissible localization of the already
coarsened block, then uses linearity within that
construction.

### Which volume is paid by the Gaussian comparison

The native carrier of \(A_F\) can include a protected
old component \(P\) and its fixed dependency
footprint \(D(P)\). These remain in the native
support ledger. They are not \(B\)-variables.
The next ordinary current is introduced only
on the new regular region. The source's next
four-layer enclosure contains \(D(P)\), so
\[
 D(P)\cap\{\hbox{new free current coordinates}\}
 =\varnothing .
 \tag{ND.40}
\]

The Gaussian determinant factors in CMP116
(2.15)–(2.17) and (2.24) count the actual
conditioned Gaussian coordinates. In the
mixed-region version of CMP119 pp.275–278
these are the regular free coordinates.
In (ND.39), \(Z_0\) is selected from the actual
support of \(K(B,\zeta)\). The large native
footprint of \(A_F\) is not added to that
Gaussian integration set. Enlarging the
native coefficient's carrier cannot by
itself insert a factor
\(\exp(C|D(P)|)\) in this Gaussian estimate.

The Gaussian localization can add regular
walk-support coordinates. Their real volume
remains the same volume cost as in the source
Gaussian comparison and must be paid by the
new localization record. A native carrier
still needs its own connector and root
estimate. Neither obligation is removed
by (ND.40).

### Self coefficients and the representation convention

The identity in (ND.35) must already hold
on the fixed coarsened native master family.
If every summand has the same later self/nonself
classification, linearity gives
\[
 {\bf1}_{\mathrm{self}}\,F
   =\sum_i{\bf1}_{\mathrm{self}}\,F_i
 \tag{ND.41}
\]
within that same family. This proves equality
of the complete self scalar before and after
resolving the block's internal labels.

It does not identify that scalar with the
self scalar of another localization convention
whose individual carriers and determining
sets were independently chosen. If the
inductive representation is changed by
coarsening, the source self term and canonical
operation must thereafter be read in this
one fixed coarsened representation. Their
full normalized masses and compensating
outer factors must be retained there.

Thus the valid statement is preservation of
the literal self sum under regrouping in
the chosen source family. Equality of
separately relocalized historical self
sums is a stronger assertion and is not
used by Lemma ND.4.

## 9. Summary

The common-reference lemma holds. The E phase
estimate retains the correct shrinking source chart,
the own Wilson subtraction and the full inherited
bank. The native argument explicitly retains
\(B(0,\xi)\) and the actual surviving preparation
slots.

The most delicate step is the
source-to-count passage: a bound on separate
ancestral components is insufficient for the
whole-prefix phase estimate. The derivation in
Lemma ND.1 closes that passage on the actual
componentwise bounded rectangular preparation
sequence explicitly used in LFR I. The complete
boundary estimate cites that sequence
directly and retains the source's distinction
between an eligible R prefix and a general
ordinary branching history.

If the C05 class were instead defined to
include an arbitrary branching prefix without
that operative source condition, (ND.29) shows
that the existing arbitrary-test normalization
argument would not apply. That stronger class
would require a genuinely different local
normalized-kernel theorem. It must not be
silently inserted or silently excluded.

The completed relative catalog requires a separate
positive transfer argument. Native analyticity and
normalization do not by themselves prove that estimate.
The quantitative check of the PC.6–PC.6a
argument follows.

## 10. Quantitative check of the coarsened positive transfer

This section checks PC.6–PC.6a
against Q §§16.9–16.10, 17.3–17.6, M §§24–27,
S §§3–7, and A15–A16. It does not reopen the native
or Gaussian proofs above. The coarsened atom is
the complete scalar of PC.12 on the one fixed
source representation. Its spatial graph and
creation annotations are retained.

### 10.1 Creation families are not spatial components

The outer creation index must have the form
\(c=(b,s)\), where \(b\) is an actual creation
grade and \(s\) is an operation sector. The
locations, shapes, component identities and
localization records of that sector are labels
\(G\) **inside** its positive rooted sum. Thus,
for example, the seed capacity has the form
\[
 \kappa_{b,s}=
 \sup_{\mathfrak h,a_{\rm ext}}\sup_y
 \sum_{\substack{G\in\Gamma_{b,s}(\mathfrak h)\\y\in G}}
       W_b(G)\sup_{\xi\in\mathcal D^+}|F_G(\xi;a_{\rm ext})|.
 \tag{ND.42}
\]
It is not a sum, over all spatial components,
of their separate rooted suprema. The finite
list of operation sectors, and any polynomial
list of proper integration/localization grades,
is included in the fixed logarithmic power of
the creation bound. No number of lattice sites
appears in this outer index.

This convention is necessary: even a uniformly
bounded finite-range activity would give an
extensive capacity if each translate were first
assigned its own supremum and those suprema
were then summed. The source rooted activity
estimates sum those translates inside the
rooted norm, exactly as in (ND.42).

### 10.2 An explicit root pushforward

Fix one actual history, one exterior real tuple
and one origin family \((b,s)\). All the
following geometric bounds hold uniformly in
the internal real tuple subsequently averaged
by the common prefix measure.

A direct prefix use at \(r\) requires
\(h_r\le j\le b-1\), hence \(r-b<N_r\).
For a newly installed footprint \(D(P)\),
choose a deterministic genuine old raw endpoint
of the input in \(P\). Its owner is an active
source block; a purely decorative old footprint
cannot supply this endpoint. At the creation
grade it belongs to the complete admitted
ancestor \(Z_b[P]\). Let
\(\mathcal Y_{b,r}(P)\) be the actual \(b\)-block
cover of that ancestor, with the fixed stencil
allowance. [CT.1](operative_source_scope.md) gives
\[
 |\mathcal Y_{b,r}(P)|\le C(1+R_b)^4.
 \tag{ND.43}
\]

For an output block root \(x\) at the record's
actual geometric grade \(r\), define a
nonnegative incidence kernel by
\[
 K_{b,r}(x,y)=
 A_{b,r}\sum_{\substack{P\text{ directly used}\\x\in D(P)}}
       {\bf1}_{\{y\in\mathcal Y_{b,r}(P)\}}.
 \tag{ND.44}
\]
Here \(A_{b,r}\) includes only the fixed stencil
and proper integration/localization label
multiplicities. It is a fixed polynomial in
\(\ell_b\) on the direct-use window. At one
grade the components \(P\) are disjoint and
each occupies an actual current block; their
diameters and footprint radii are \(O(R_r)\).
Consequently at most a fixed polynomial in
\(R_r\) of their footprints can contain one
current block root. At a genuine component
root the component is specified and this
extra covering factor is unnecessary.

The AF window comparison and [CT.1](operative_source_scope.md) therefore
give, with the sum over possible direct-use
grades made once,
\[
 \sup_x\sum_y K_b(x,y)
 \le C(1+\ell_b)^{D_{\rm tr}},
 \qquad
 K_b=\sum_{r:\,r-b<N_r}K_{b,r}.
 \tag{ND.45}
\]
The constants and exponent are independent of
volume, cutoff depth and the number of other
components in the history. An inherited root
which does not enter a new footprint keeps its
old incidence; it uses the already retained
root and connector estimates, with no new
root migration. In particular an unchanged
atom is not promoted to the entire later
coarse cell. Its later physical-current
readout uses the established age kernel.
Equation (ND.45) is a count at its actual
geometric grade, not a claim that an arbitrary
later coarse box contains only polynomially
many fine cells.

After the consumed-mark and crossed-connector
payments below, positivity gives the direct
pushforward bound
\[
 S^{\rm out}_{b,s}(x)
 \le e^{d_*R_b}
           \sum_y K_b(x,y) S^{\rm in,res}_{b,s}(y),
 \tag{ND.46}
\]
where \(S^{\rm in,res}\) denotes the actual
input rooted sum with the unspent source-block
marks retained. The single factor
\(e^{d_*R_b}\) is needed only for the one
wholly contained unguarded use. The weights
for other newly installed components have
already been paid by their distinct released
connector segments. A deterministic witness
choice gives the displayed upper bound;
summing all allowed witnesses only enlarges
its right-hand side and is bounded by (ND.45).

Taking the root supremum in (ND.46) yields
\[
 \|\mathcal L F_{b,s}\|_{\rm rooted}
 \le C(1+\ell_b)^{D_{\rm tr}}e^{d_*R_b}
          \|F_{b,s}\|_{\rm rooted,res}.
 \tag{ND.47}
\]
Only after this bound is established for the
whole spatial family is the outer sum over
\((b,s)\) taken. This is the nonextensive
meaning of summing original creation budgets.

### 10.3 Normalization, raw suprema and mark multiplicity

For fixed \(\mathfrak h,a_{\rm ext}\), ND.27
provides one positive probability measure
\(\mu_0\) dominating the whole complex working
chart. It may depend on that fixed exterior
tuple. For a common catalog of labels, with
absent entries set to zero,
\[
 \sum_G W_G\sup_\xi|\Pi_\xi F_G|
 \le M_{\rm pref}\int
           \sum_G W_G\sup_\xi|F_G(\xi,a)|\,d\mu_0(a).
 \tag{ND.48}
\]
Thus the input uniform bound may be used
inside this probability integral, and the
supremum over the real exterior tuple is
taken afterward. No supremum over raw
variables is moved inside the positive
catalog sum. If the internal history varies
with \(a\), use the common zero-extended
catalog and the pointwise incidence bound
(ND.45), uniform in \(a\). The history is
then averaged, not counted by a second
unweighted sum.

Each directly used component consumes at
least one distinct original source-block
mark, irrespective of the number of fine
raw slots in that block. With \(u\) the
number of unspent marks and \(q\) the
number of components directly used,
\[
 u_{\rm out}+q\le u_{\rm in},\qquad
 M_{\rm pref}^{q}M_{\rm pref}^{u_{\rm out}}
                   \le M_{\rm pref}^{u_{\rm in}}.
 \tag{ND.49}
\]
This is a pointwise weight cancellation before
integration or any root supremum. The whole
original block lies inside the component
which used it; a retained failure encloses
the block and all of its old slots. The
failure clock precludes reuse. A success
consumes the old slots and ends that
lineage. These are precisely the ownership
alternatives of Q §16.10 and M §24.3–24.4.

Products carry the multiset of creation
and mark records. Their physical graphs
may be united, since the physical weights
are submultiplicative, but equal labels
on different input occurrences are not
silently identified. Before further
consumption one may use
\(u_{\rm product}\le\sum_i u_i\), with
equality for the retained multiset. The
source's unordered-family factorials then
handle repeated occurrences in the
ordinary way. Terms with different
reserves are not merged using merely
the union of their marks; either keep
their separate weighted blocks or their
weighted sum.

### 10.4 The footprint reserve is a genuine source reserve

For a crossed component, let the length
released when its actual core is installed
be \(\Delta L_P\ge c_0R_r\). Choose
the allocated footprint diameter and
fixed tag/root costs so that, at the
common lower cutoff on \(R_r\),
\[
 C(1+\ell_r)^D e^{d_0R_r}
              \le e^{\lambda\Delta L_P}.
 \tag{ND.50}
\]
Here \(d_0<\lambda c_0\) is chosen
with a strict spare margin. The divided
physical-current tree of \(m\) endpoints
inside \(D(P)\) has length at most
\(CmR_r\); its weight costs at most
\(e^{C\gamma R_r}\), independently of
\(m\). The allowed fixed small endpoint
rate \(\gamma\) fits the same margin.
The source-block normalization factor
is paid separately by (ND.49).

The released segments are disjoint for
distinct simultaneous components and
cannot be used again along the same
old raw-slot lineage. An overlapping
later attempt would contain the retained
failed component, whose clock excludes
the relevant old slots; successful
consumption instead ends the lineage.
Thus (ND.50) is a cumulative use of
actual removed lengths. It does not
decrease the rate of the surviving
exterior connector at each attempt.

There is at most one directly used
component containing the entire old
carrier. This case has no forced
crossing. PC.6a explicitly restricts
it to a relative creation with its
proved fresh small tail. If that
creation has seed bound
\[
 \kappa_b\le C H(F_0,A_*)
       [g_b^{-u}(1+\ell_b)^v e^{-cR_b}]^{\theta},
 \qquad \theta=1/18,
 \tag{ND.51}
\]
reserve its entire future allowance
\[
 a_b=C(1+\ell_b)^{D_{\rm tr}}
                    e^{d_*R_b}\kappa_b
 \tag{ND.52}
\]
once, at creation. Taking the fixed
diameter share \(d_*<\theta c\), with
a strict margin, leaves
\[
 a_b\le C'H(F_0,A_*)
 [g_b^{-u'}(1+\ell_b)^{v'}e^{-c'R_b}]^{\theta}
 \quad(c'>0).
 \tag{ND.53}
\]
All constants are fixed before choosing
the common coupling ceiling. Since
\(R_b\) is superlogarithmic in
\(\ell_b\), every additional fixed
root/window polynomial fits the same
strict margin.

The non-small ordinary \(B_0,C_0\)
reference cannot be used as though it
had the tail (ND.51). Wholly contained
ordinary terms stay in the zero-mark
reference action, including its exact
normalizer and native-dependent outer
mass. A coupling to an exterior
integration component has a paid
ordinary crossing and belongs to the
guarded interaction catalog. The
ordinary nonself seed is estimated
as a whole coefficient by the source
(1.68), as in Q §18.4 and M §26,
before it is admitted to (ND.51).
This distinction removes the otherwise
invalid use of a new
\(R_b\)-diameter from a bare constant
ordinary bound.

### 10.5 The capacity recurrence follows in the same summable class

An unchanged degree-one family spends
its assigned marks, released lengths
and the single allowance (ND.52).
It is not added again to the fresh
forcing. An exterior raw dependence
newly generated by a prefix has the
exact normalized numerator-minus-
denominator identity of M §24.2 and
its own guarded creation bound.
An actually used successful component
has the distinct source volume-paying
mass; it is not an unpaid continuation
of the previous failure lineage.

New ordinary maps and localized
Gaussian pieces use their actual
new support volume, as established
in ND.4 and PC.4. Auxiliary attachment
entropy is paid by the summable
count-rate decrements; exposed
connector attachments use the exact
physical coarsening reserve of S6a
and S11–S12. These operations do
not add the native footprint as new
Gaussian volume.

Consequently, after summing the finite
operation sectors at a fixed grade,
the root pushforward (ND.47) only
changes the fixed constants and
logarithmic powers of the fresh
profile. The same holds for the
recent nonlinear sector: with recent
load \(K_r\) and cluster radius
\(s_r\), its common-mark estimate
is \(CK_r^2/s_r\), while the
degree-one part uses its old
capacity. For
\(K_r\le\operatorname{poly}(\ell_r)
\epsilon_r^{1/18}\) and
\(s_r\asymp\operatorname{poly}(\ell_r)
\epsilon_r^{1/72}\), the available
power is \(7/72>1/18\). Hence
the fresh exponent is not degraded
at repeated prefixes.

Let \(A^{[k]}\) sum the reserved
capacities of the global creation
families \((b,s)\), with spatial
positions inside their norms as
in (ND.42). The actual catalog
is dominated by this sum before
the final graded root supremum.
The resulting recurrence is
\[
 A^{[k]}\le e^{C\sigma_k}A^{[k-1]}+f_k,
 \qquad
 \sigma_k=C\operatorname{poly}(\ell_k)
                            \epsilon_k^{1/72},
 \tag{ND.54}
\]
with
\[
 f_k\le C H(F_0,A_*)
 [g_k^{-u'}(1+\ell_k)^{v'}e^{-c'R_k}]^{1/18}.
 \tag{ND.55}
\]
The retained AF envelope makes both
\(\sum_k\sigma_k\) and \(\sum_k f_k\)
uniformly small at the common weak
ceiling. The source connector rate
and the auxiliary rates retain their
fixed positive floors. Thus A15–A16
close for the coarsened
catalog, without a volume factor
from the creation index or a renewed
old transport budget.

**Quantitative conclusion.** PC.6–PC.6a
satisfy this bookkeeping
check with the explicit conventions
(ND.42) and (ND.49): global creation
families, actual-grade root incidence,
and retained mark multisets. The
contained-case reserve has
the relative fresh-tail scope
stated in PC.6a. The conclusion
uses the source/map/forest estimates
already named in PC.6; it does not
turn native analyticity alone into
a positive catalog theorem or assert
a norm estimate for arbitrary
abstract ball inputs.
