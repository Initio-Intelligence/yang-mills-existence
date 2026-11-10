# Generic nondegeneracy on stopped sequences

**Gaussian calibration hypothesis (GC).** For the signed Gaussian increments of the actual stationary source section in its thermodynamic normalization, assume $\sum_{k<n}d_k^G=d_Bn+\vartheta_n$ with $d_B>0$ and $\sup_n|\vartheta_n|\le B_G$. The coupling and stopping conclusions use this calibration and the specified source readout and replay. A physical continuum limit also requires the stated uniform normalization and full-law hierarchy estimates.

**Finite-cutoff scope.** Nonzero reflected measurements at each cutoff allow finite normalization. Uniform bounds for the seven normalizing factors along one physical sequence and passage of the full normalized hierarchy have separate hypotheses.

This note adds a qualitative, finite-cutoff result to
physical normalization. It combines the already verified
actual-Wilson ultracold witness with the stopped sequence of
[A stopped sequence with a positive weak endpoint](positive_stopped_endpoint.md). It uses the fixed F01 clover
fields, reflection measurements, target values and subtraction scheme.

The conclusion is that **one cofinal stopped sequence can be chosen with
all seven actual physical normalization measurements strictly positive
at every retained cutoff**. No continuity of the stopped depth or of the
rounded radius prescription is required. The construction does not give
the quantitative logarithmic coefficient budget in F05, and does not
shoot to a prescribed scalar endpoint in B05.

**Governing subsequent result.** Section 6 records the stronger
reflection-slab theorem in finite reflected witnesses.
It removes this note's enlarged-volume restriction and supplies
the same qualitative finite normalization on the original slow-volume
PE sequence. Sections 1–5 remain a correct independent fallback.

## 1. The fixed finite measurements

Fix \(SU(N)\), the odd block factor \(L\), the physical unit \(\ell_0\),
the physical normalization scale \(\mu\), and the actual F01 fields and
tests in Annex X (F.19)–(F.37).

For integers \(K,H\), use
\[
 a_K=\ell_0L^{-K},\qquad T_H=2L^H\ell_0,\qquad
 N_f=T_H/a_K=2L^{H+K}.
 \tag{GN.1}
\]
Let
\[
 n_{h;K,H}(\beta),\qquad
 h\in\{S,T_d,W_d,T_o,W_s,P,W_p\},
 \tag{GN.2}
\]
be the seven centered reflected measurements of that exact finite
Wilson law
\[
 d\mu_{\beta;K,H}
 =Z_{K,H}(\beta)^{-1}
    \exp\!\left[-\beta\sum_p
       \bigl(N-\operatorname{Re}\operatorname{Tr}U_p\bigr)\right]dU.
 \tag{GN.3}
\]
In particular \(\beta\) is the coefficient of this displayed Wilson
action, not a separately normalized inverse coupling.

The test lobes are the fixed smooth physical lobes in F.19–F.20.
Enlarge a fixed lower bound on \(K\) so that their complete clover
footprints lie in their required open reflection half-tori. Enlarge a
fixed \(H_0\) so that the physical test supports fit in the original
cubic tori. Reflection positivity gives
\[
 n_{h;K,H}(\beta)\ge0,\qquad\beta>0.
 \tag{GN.4}
\]
All raw stencils, paths, weights and projectors are the original ones.
The centering in (GN.2) is performed in the same actual finite law.

### Lemma GN.1 — finite-cutoff analyticity

At each such fixed \((K,H)\), every \(n_{h;K,H}\) is real analytic on
\((0,\infty)\).

**Proof.** There are finitely many compact link variables. The Wilson
action is bounded on their product, as is each fixed-cutoff raw clover
stencil. For every bounded observable \(F\) used in the finite
measurement, the integral
\[
 I_F(z)=\int F(U)e^{-zS(U)}\,dU
 \tag{GN.5}
\]
is entire in \(z\): on any compact complex disk its power series and all
derivatives are uniformly dominated by a finite constant. The
partition function \(I_1(\beta)\) is strictly positive for real
\(\beta>0\). Thus each ratio \(I_F/I_1\) is analytic in a neighborhood
of every such real point.

Expanding the centered measurements expresses them as finite linear
combinations of uncentered second moments and products of first
moments. Their coefficients include only fixed finite lattice sums,
test values and channel projectors. They are therefore real analytic.
\(\square\)

## 2. An actual Wilson witness on every geometry in a countable family

The needed witness is already established in
the clover comparison, Section “A separate interacting comparison
for the separated reference measurements,” including its final
paragraph on a test coupling independent of the physical bare coupling.
Its inputs are the compact Wilson reserve and the actual clover
comparison of Annex O §§22, 26 and 29. In its action convention,
\[
 \beta^2n_{h;K,H}(\beta)\longrightarrow4\lambda_h(\mu)>0
 \tag{GN.6}
\]
on the stated ultracold comparison family. The factor \(4\) is the
verified generator/action conversion in that comparison; it is not
used to change the physical normalization targets.

For clarity, its uniformity supplies the following particular family.
Put \(\epsilon_0=10^{-6}\), and at depth \(K\) choose the test coupling
and comparison box size
\[
 \beta_{\rm test}(K)=L^{110K/\epsilon_0},
 \qquad l_K=L^{110K}.
 \tag{GN.7}
\]
For every integer
\[
 H\ge H_*(K):=\max\{H_0,110K+2\},
 \tag{GN.8}
\]
the period \(2L^{H+K}\) is divisible by \(l_K\) and is at least
\(3l_K\). The physical lobe separation in fine units is bounded by
\[
 R_K=C_\mu/a_K\le \beta_{\rm test}(K)^{\epsilon_0/100}
 \tag{GN.9}
\]
for all sufficiently large \(K\), since the two sides grow as
\(O(L^K)\) and \(L^{1.1K}\), respectively. These are precisely the
geometric and coupling conditions of the quoted Wilson comparison.

Here is why the conclusion is uniform over all \(H\) in (GN.8), rather
than merely along one chosen volume sequence. The comparison bound
uses the period only through divisibility, the lower bound \(3l_K\),
and the uniform compact-moment reserve. Its dimensionless centered
pair error is bounded by
\[
 C_\mu\!\left[
 \beta_{\rm test}^{-\epsilon_0/6}
 +R_K/l_K+
 R_K\bigl(l_K^{18}\beta_{\rm test}^{-1/4}
              +\beta_{\rm test}^{-15/32}\bigr)\right],
 \tag{GN.10}
\]
with the stated negligible chart tails. Multiplication by \(a_K^{-8}\)
pays the engineering factor. The four displayed terms then tend to
zero: their respective powers of \(L^K\), up to fixed constants, are
\[
 L^{-31K/3},\quad
 L^{-101K},\quad
 L^{(1989-110/(4\epsilon_0))K},\quad
 L^{(9-1650/(32\epsilon_0))K}.
 \tag{GN.11}
\]
The compact-moment reserve is uniform because
\(\log(1+\beta_{\rm test})/N_f\) is bounded on the whole family.
The finite physical smearing has bounded absolute total weight and
introduces no additional count of sites. The lattice Gaussian
symbol/shift error and ordinary separated Riemann error are \(O_\mu(a_K)\).
All these estimates are independent of the larger allowed \(H\).
Thus (GN.6) holds uniformly over (GN.8).

Because there are only seven fixed positive targets, there is one
integer \(K_0\) such that
\[
 \beta_{\rm test}(K)^2n_{h;K,H}(\beta_{\rm test}(K))
 \ge 2\lambda_h(\mu)>0
 \quad
 (K\ge K_0,\ H\ge H_*(K),\ \text{every }h).
 \tag{GN.12}
\]
The constant \(2\) is only a convenient strict lower fraction of the
limit \(4\lambda_h\).

This step uses an already proved actual finite-Wilson comparison. It
does not claim that its ultracold quantitative estimate holds at the
physical logarithmic bare coupling. The role of \(\beta_{\rm test}\)
is solely to prove that a finite analytic function is not identically
zero. Every positive \(\beta_{\rm test}\) is an allowed parameter of
the compact law (GN.3). It need not stop at depth \(K\), have the
desired physical running, or belong to the eventual stopped sequence.

### Corollary GN.2 — a countable universal exceptional set

There is a countable set \(\mathcal B\subset(0,\infty)\) such that
\[
 \beta\notin\mathcal B
 \ \Longrightarrow\
 n_{h;K,H}(\beta)>0
 \quad\text{for every }K\ge K_0,\ H\ge H_*(K),\ h.
 \tag{GN.13}
\]
Its complement is dense and has full Lebesgue measure.

**Proof.** For a fixed pair define
\[
 \Delta_{K,H}(\beta)=\prod_h n_{h;K,H}(\beta).
 \tag{GN.14}
\]
Lemma GN.1 makes it real analytic; (GN.12) makes it nonidentically zero.
Its zeros in \((0,\infty)\) are isolated. In particular each zero set
is countable: on each compact interval contained in \((0,\infty)\)
it is finite, since an infinite set there would have an interior
accumulation point. Take \(\mathcal B\) to be the union of these zero
sets over the countably many integer pairs in (GN.13). It is
countable and hence has measure zero and cannot contain any open
interval. Outside it, every product (GN.14) is nonzero; the
nonnegativity (GN.4) gives strict positivity of each factor.
\(\square\)

## 3. Choose the bare sequence before running the stopping rule

Use the actual-map assumptions and the fixed scheme of PE.1–PE.14.
Write \(Y_0=N\beta\), and fix \(Y_{\rm base}\) larger than the PE
stopping threshold. For a single number \(\delta\in(0,1)\), consider
the entire arithmetic prescription
\[
 Y_{0,n}=Y_{\rm base}+n+\delta,\qquad
 \beta_n=(Y_{\rm base}+n+\delta)/N,\qquad n=1,2,\ldots .
 \tag{GN.15}
\]

### Lemma GN.3 — one offset works at every prospective depth and volume

There exists a single \(\delta\in(0,1)\) for which every \(\beta_n\)
in (GN.15) lies outside \(\mathcal B\). Almost every \(\delta\) works.

**Proof.** The forbidden offsets form the countable set
\[
 \mathcal D=
 (0,1)\cap\bigcup_{n\ge1}
       \{N b-Y_{\rm base}-n:b\in\mathcal B\}.
 \tag{GN.16}
\]
Choose \(\delta\notin\mathcal D\). Its definition excludes exactly
the asserted bad equalities, simultaneously for every \(n\).
\(\square\)

The choice can be fixed once as a deterministic set-theoretic
prescription, rather than made anew after observing each stop.
For example enumerate the countable triples \((n,K,H)\) in the
allowed family and their corresponding analytic functions
\[
 \delta\longmapsto
 \Delta_{K,H}((Y_{\rm base}+n+\delta)/N).
 \tag{GN.17}
\]
Begin with a closed rational interval strictly inside \((0,1)\).
At each enumerated function, take the first closed rational
subinterval, in a fixed enumeration, lying in the interior of
the preceding interval, of length at most \(2^{-j}\), on which
that function is strictly positive. Such an interval exists by
analyticity and nonidentity. The nested intervals have a single
common point. That point stays in the positive interval selected
for each function and hence supplies the required \(\delta\).
This prescription asserts existence; it gives no effective
algorithm, numerical lower bound, or efficient way to locate
the interval. Countable exceptional sets can contain every
computable candidate; countability alone does not prove that
an effectively computable \(\delta\) works.

### Theorem GN.4 — a nondegenerate stopped physical sequence

There is one sequence of actual bare Wilson coefficients and original
cubic tori with all of the following properties:

1. Its actual PE stopping and bounded trimming give
   \(K'_n\to\infty\), and its final scale is exactly \(\ell_0\).
2. Every used source prefix is admitted, and the retained terminal
   inverse couplings stay in the fixed interval \([Y_-,Y_+]\) of PE.13.
3. Its bare coefficients have the physical logarithmic order and,
   with the stated sharper PE recurrence, the asymptotic formula
   \[
    \beta_n=
     \frac{d_B}{N\log L}\log(\ell_0/a_n)
       +O\!\bigl(\log\log(\ell_0/a_n)\bigr)+O(1).
    \tag{GN.18}
   \]
4. All seven actual F01 measurements are strictly positive at every
   retained cutoff.

**Proof.** Fix \(\delta\) from Lemma GN.3 and run the same actual causal
source prescription on (GN.15). PE's stopping proof applies to any
unbounded sequence of admitted bare inputs. It supplies \(K_n,K'_n\),
the unchanged retained prefix, the terminal interval, and (GN.18).
Discard the finitely many initial indices with \(K'_n<K_0\).
If desired, retain the deterministic first subsequence of strictly
increasing \(K'_n\), as in PE.

The order of operations matters here. PE uses the homogeneous
infinite-volume coupling readout at each finite prefix. Its retained
replay convention chooses the finite torus after that prefix has
been computed. In particular \(K_n\) and \(K'_n\) in this proof are
computed without using a subsequently selected finite \(H_n\).
This is PE's actual prescription, not a new assumption of continuity
of a finite-volume stopped trajectory in its volume.

Set
\[
 a_n=\ell_0L^{-K'_n},\qquad
 T_n=2L^{H_n}\ell_0,
 \tag{GN.19}
\]
where \(H_n\) is any integer at least \(H_*(K'_n)\), enlarged further
if required for that finite-prefix replay convention.
PE Section 5 allows these larger original cubic tori: the same
fixed period divisors hold, the required neighborhoods fit, and
the finite-torus replay uses the same prescribed scalar readout.
There is no upper bound on \(H_n\) in that construction.
Since \(K'_n\to\infty\), these volumes also tend to infinity.

The bare value \(\beta_n\) was chosen outside \(\mathcal B\) for
every possible eligible integer geometry, before the trajectory
was computed. Apply (GN.13) to the geometry that actually resulted:
\[
 n_{h;K'_n,H_n}(\beta_n)>0\qquad\text{for all seven }h.
 \tag{GN.20}
\]
No comparison of nearby stopping times, no persistence of a
particular rounded-radius chart, and no prescribed-depth shooting
is used. PE already supplies the other assertions.
\(\square\)

The bounded terminal interval still gives a subsequence with
\(g_{K'_n}\to g_\infty>0\), at the retained weak ceiling. All finite
positivity statements remain true on that subsequence.

## 4. Consequences for the exact finite normalization

On the sequence of Theorem GN.4, the exact F01 prescription is now
well-defined without its zero-channel fallback:
\[
 z_{h,n}=\sqrt{\lambda_h(\mu)/n_{h;K'_n,H_n}(\beta_n)}>0,
 \qquad
 Z_n=\sum_hz_{h,n}P_h,
 \qquad
 c_n=z_{S,n}m_n.
 \tag{GN.21}
\]
The matrix \(Z_n\) and its inverse are finite at every retained cutoff.
The seven target equations and the scalar centering equation hold in
the original scheme. In the scaled variables of PN.5,
\[
 D_{h,n}=\beta_n^2n_{h;K'_n,H_n}(\beta_n)>0,
 \quad
 t_{h,n}=z_{h,n}/\beta_n,
 \quad
 \widehat c_n=a_n^4c_n,
 \tag{GN.22}
\]
their actual finite Jacobian satisfies
\[
 \det J_n=-2^7\prod_h\sqrt{\lambda_hD_{h,n}}\ne0.
 \tag{GN.23}
\]
This is qualitative nonsingularity of the actual normalization
system. The identity coefficient still has the companion
comparison \(a_n^4c_n=e_nz_{S,n}/\beta_n\), with fixed positive upper
and lower bounds on \(e_n\), from PN.1–PN.3.

## 5. Exact limitations and compatibility cost

The result eliminates exact zero measurements from one admissible
stopped sequence. It supplies no rate at which its positive
\(D_{h,n}\) can approach zero, and no uniform upper bound on them.
The quantitative F05 requirements remain:
\[
 D_{h,n}\ge c\,\lambda_h L_n^{-2}
 \quad\text{and the needed upper bounds,}
 \tag{GN.24}
\]
for the actual prescribed logarithmic coefficient budget \(L_n\).
Generic avoidance of a discrete zero set does not establish (GN.24).

The larger volumes in (GN.8) are permitted by PE, but they forfeit
PE's optional slow-volume choice \(V_{{\rm term},n}=o(K'_n)\).
In particular the current ER.1/H2S global ancient-sector deletion
uses precisely that slow-volume relation. A bound of the form
\(\exp\{CV_{\rm term}-cK'\}\) does not tend to zero on the enlarged
volume family here. That global deletion cannot be imported into
Theorem GN.4. Retaining the old sector is permitted by the exact
positive construction, but its required marked estimate remains
an additional obligation. A proof needing both finite positivity
and the earlier global deletion needs a positivity witness on the
slower volume family, or a new ancient-sector estimate.

The bounded-probe kernel compactification is not based on that
global ancient-sector deletion and may still retain the complete
old sector. This structural bounded-probe statement gives neither
the unbounded physical moments nor the missing ER.7 estimates.

The emergent positive scalar endpoint remains an emergent endpoint;
this proof does not impose a preassigned B05 physical coupling.
It does not replace the actual F03 mixing matrices by the free
comparison, prove an ER.7 hierarchy bound, or infer convergence of
the normalized fields from their finite positivity. PN.7 continues
to state the separate exact implication from a convergent normalized
hierarchy to a nondegenerate limit.

## 6. Governing slow-volume strengthening

Theorem FN.1 in finite reflected witnesses proves,
for every sufficiently fine fixed original cubic torus with a
nonempty sampled F01 lobe, that all seven actual reflected
measurements are positive for sufficiently large \(\beta\).
Its proof uses the exact reflection-plane conditional square and
explicit small boundary fields for the actual Wilson action.
The threshold may depend on that fixed geometry.

This provides a nonidentity witness for each analytic product
\(\Delta_{K,H}\) on **all** integer geometries \(K\ge K_0\),
\(H\ge H_0\), without the restriction \(H\ge110K+2\).
The countable exceptional-set argument of Sections 2–3 then
applies to this larger geometry family. Corollary FN.5 chooses
one offset before stopping and retains
\[
 H_n=\max\{H_0,\lfloor\theta\log_L(2+K'_n)\rfloor\},
 \qquad 0<\theta<\tfrac14,
 \qquad V_{{\rm term},n}=o(K'_n).
 \tag{GN.25}
\]
Every actual finite F01 normalization is nonsingular on that
sequence.

Thus the enlarged-volume compatibility cost stated in Section 5
belongs to the independent ultracold fallback proved in this file.
For the main construction it is removed by the separate
reflection-slab theorem. The geometry premise of the ER.1/H2S
ancient-sector reduction can be retained; that observation supplies
no new marked estimate. The quantitative logarithmic bounds
(GN.24), actual F03/F04 mixing, the prescribed B05 endpoint and
the full ER.7 hierarchy remain separate obligations.
