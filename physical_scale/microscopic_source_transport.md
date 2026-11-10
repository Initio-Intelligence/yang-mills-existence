# Microscopic source transport and contact neutrality

## Assumptions and conclusions

There is a full-history statement for the actual microscopic fields that does not require replacing them by current-scale stencils or differentiating hard selectors separately. Freeze the positive source-free RG/history construction, insert the same physical microscopic source on its common raw lattice, and transport its finite source jet by the exact conditional kernels. This gives exact moment and conditional-cumulant identities through every regular step, preparation, completed operation and final averaging.

For coincidence-flat joint tests, the compact microscopic moment reserve then gives a useful uniform estimate: the portion of the actual transported \(m\)-point jet within a physical collar \(r_a=a^\theta\) of a coincidence diagonal tends to zero, with a test derivative order linear in \(m\), uniformly in the number of RG steps. Strictly diagonal source contacts of order at least two are exactly neutral on these tests. The corresponding reflection-positivity forms retain their physical meaning.

This is a statement about the actual transported microscopic **source jet in averaged norms**, including the full history law. It is not the full retained-data carrier estimate of M03, the scalar extraction of M04, the running normalization of F05, or an off-diagonal Schwinger bound. Those distinctions remain explicit below.

## 1. The microscopic fields and their identity budget

Work on the admitted cofinal/AF-bounded geometries for which the original compact Wilson reserve (M.14) holds. Let \(a\) be the microscopic physical mesh. First use the centered fixed representatives

\[
 O_{\alpha,a}(x)=
 \beta_a\widetilde q_{\alpha,a}(x)
       -\mu_a[\beta_a\widetilde q_{\alpha,a}(x)],
 \qquad \alpha=1,\ldots,21.
 \tag{CS.1}
\]

These are exactly the scalar-repaired F01 clovers of (M.13), including their specified finite stencils. The compact identity
\(\|U_p-I\|_{HS}^2=2s(U_p)\), the finite clover estimates and the actual normalized energy reserve give

\[
 \|O_{\alpha,a}(x)\|_{L^p(\mu_a)}
               \le C a^{-4}p,\qquad p\ge1.
 \tag{CS.2}
\]

This is the original (M.14)–(M.17), rather than a new regular-sector hypothesis. At an arbitrary finite cutoff outside the stated reserve class one has only the finite compact bound, with its corresponding constant.

For any specified finite F01 prescription

\[
 \Phi_a=Z_{a,T,\mu}\widetilde q_a-c_{a,T,\mu}e_S,
 \qquad
 b_a=\frac{\|Z_{a,T,\mu}\|}{\beta_a}+a^4|c_{a,T,\mu}|,
 \tag{CS.3}
\]

the same proof gives

\[
 \|\Phi_{\alpha,a}(x)\|_p
                   \le C b_a a^{-4}p.
 \tag{CS.4}
\]

Every estimate below includes \(b_a^m\) for this choice. No uniform or logarithmic estimate on \(b_a\), no inverse normalization determinant, and no nondegenerate cofinal tail is inferred. Those are precisely F05. The unconditional uniform statement in this note uses (CS.1), for which the exposed budget is fixed.

A degree-one identity subtraction is not a coincidence contact. It contributes away from every diagonal in higher full moments and must be specified explicitly. For (CS.1) it is the actual microscopic expectation; its size is bounded by \(C a^{-4}\). For the finite prescription (CS.3), its stated identity budget remains in \(b_a\). A later conditional first moment is generally nonzero even when the full microscopic field has been centered.

## 2. Freeze the source-free lift before adding the source

Fix the complete source-free construction: its couplings, maps, cutoffs, history partition, real reference variables and all normalizers. At finite cutoff its positive augmented law has the original Wilson marginal \(\mu_a\) on the raw microscopic field \(U\). Let \(\eta_k\) denote the full retained state after a chosen cut, including whatever history information is needed for a later operation. Disintegration gives an actual normalized kernel

\[
 \mathcal Q_{a,k}G(\eta_k)
       =\mathbb E[G(U)\mid\eta_k].
 \tag{CS.5}
\]

This notation also covers a cut after history erasure. Added reference variables can be kept in the common joint space before disintegration. The resulting forward/backward kernels satisfy the exact tower identities appropriate to the positive Markov construction. At an R operation where gauge restoration is an integrated Faddeev–Popov identity, use the gauge-invariant physical insertion and that integrated identity; do not identify unintegrated gauge-fixed densities pointwise. These are the qualifications already retained in C07, H03 and the source discussion following LFR II (1.72), printed pp.378–379.

Choose finitely many labeled microscopic insertions
\(\Phi_i=\Phi_{\alpha_i,a}(x_i)\), and commuting nilpotent variables
\(\varepsilon_i^2=0\). Define the finite source jet

\[
 \mathcal Z_{a,k}(\varepsilon;\eta_k)
  =\mathcal Q_{a,k}
        \prod_i(1+\varepsilon_i\Phi_i).
 \tag{CS.6}
\]

Equivalently this is the finite jet of
\(\mathcal Q_{a,k}\exp(\sum_i\varepsilon_i\Phi_i)\).
It is a polynomial identity at finite cutoff; it requires no uniform zero-free complex source disk.

### Theorem CS.1 — exact transport of the same physical source

For every nonempty label set \(I\),

\[
 M_{I,k}(\eta_k)
 :=[\varepsilon_I]\mathcal Z_{a,k}
 =\mathcal Q_{a,k}\prod_{i\in I}\Phi_i,
 \tag{CS.7}
\]

\[
 \mu_{a,k}M_{I,k}
       =\mu_a\prod_{i\in I}\Phi_i.
 \tag{CS.8}
\]

If \(Q_{k+1}\) is the next exact backward conditional kernel, then

\[
 \mathcal Z_{a,k+1}=Q_{k+1}\mathcal Z_{a,k}.
 \tag{CS.9}
\]

Its conditional connected jet is the formal logarithm
\(\mathcal H_{a,k}=\log\mathcal Z_{a,k}\), whose coefficients are

\[
 H_{I,k}
 =\sum_{\pi\in\Pi(I)}
    (-1)^{|\pi|-1}(|\pi|-1)!
                         \prod_{B\in\pi}M_{B,k}.
 \tag{CS.10}
\]

Consequently the complete update is

\[
 \mathcal H_{a,k+1}
            =\log Q_{k+1}e^{\mathcal H_{a,k}}.
 \tag{CS.11}
\]

Every pre-existing higher vertex and every conditional-mean contribution remains in this identity. In particular the average of a conditional covariance is not being substituted for the full covariance.

**Proof.** Multiply the common raw Wilson integrand by the same polynomial
\(\prod_i(1+\varepsilon_i\Phi_i(U))\) before applying any source-free identity. Conditional integration is linear in its coefficients. The marked density at a retained cut is the unmarked density multiplied by (CS.6), so its numerator and denominator use exactly the same underlying conditional law. The normalization of that law proves (CS.8), and disintegration proves (CS.9). The logarithm is defined algebraically because the constant coefficient is one. Its finite partition formula is (CS.10), proving (CS.11). No coefficient is replaced by a new current-scale observable. \(\square\)

The localized numerator construction in CMP119, printed pp.277–278, (3.44)–(3.47), may be applied to this actual insertion once its analytic/localized estimate is proved. Equations (CS.6)–(CS.11) identify the insertion that such a proof must estimate; they do not infer that estimate merely from the source's action-response calculation.

### Complete-label selector cancellation

The lift is source-free, so the \(\varepsilon_i\)-derivatives in (CS.6) never differentiate its selectors. There is also an exact common-raw-variable cancellation if one first sums the complete branch partition. In a finite presentation with weights \(w_h(U)\) satisfying \(\sum_h w_h(U)=1\),

\[
 \sum_h w_h(U)\prod_i(1+\varepsilon_i\Phi_i(U))
              =\prod_i(1+\varepsilon_i\Phi_i(U)).
 \tag{CS.12}
\]

The same statement holds with integrated reference kernels instead of scalar weights, since their total mass is one. For an ambient raw finite difference, the telescoping product rule gives

\[
 \sum_h\delta_\tau(w_h F)
  =\left(\sum_h w_h\circ\tau\right)\delta_\tau F
       +\left(\sum_h\delta_\tau w_h\right)F
  =\delta_\tau F.
 \tag{CS.13}
\]

Thus the complete selector-current contribution vanishes before absolute estimates on this common physical expression. This identity fails after restricting to an event-marked subset of histories or changing the insertion from branch to branch. It is not an estimate for the absolute sum of separate M03 selector-current records. At a fixed retained datum the different branches may also have different conditional functions, so (CS.13) is not asserted there.

## 3. A uniform shrinking-collar estimate for the transported microscopic jet

Let \(F=(F_{\alpha_1\ldots\alpha_m})\) be a smooth joint test. Use tests in a central torus chart, or compactly supported tests whose support lies inside that chart; eventual enlargements of the physical torus then preserve this convention. The field and source sums may equivalently be periodized with their true periodic coincidence diagonals.

Let \(\Delta_{ij}=\{x_i=x_j\}\). A coincidence-flat test has every derivative zero on every \(\Delta_{ij}\). For a nonnegative integer \(s\), use the explicit seminorm

\[
 \nu_s(F)=\max_{\boldsymbol\alpha}\max_{|\gamma|\le s}
     \sup_X (1+|X|^2)^{s/2}
                   |\partial^\gamma F_{\boldsymbol\alpha}(X)|.
 \tag{CS.14}
\]

Finite tensor-label sums cost at most a fixed constant to the power \(m\).
Fix \(0<\theta<1\) and \(\delta>0\), and set

\[
 r_a=a^\theta,\qquad
 N_m=\left\lceil\frac{(4+\delta)m}{\theta}\right\rceil,
 \qquad
 s_m=\max\{N_m,6m\}+2.
 \tag{CS.15}
\]

For \(m\ge2\), let \(\chi_{a,m}(X)\) indicate that at least one pair has
physical separation at most \(r_a\). Define the actual smeared conditional
moment in this collar by

\[
 \mathcal C^{\rm mom}_{a,k,m}(F)
 =a^{4m}\sum_{\boldsymbol\alpha,X}
       \chi_{a,m}(X)F_{\boldsymbol\alpha}(X)
                            M_{\{1,\ldots,m\},k}(X).
 \tag{CS.16}
\]

All source positions in this expression are still microscopic physical
positions. The kernel \(\mathcal Q_{a,k}\) acts on the field/history variables,
not on those positions.

### Theorem CS.2 — depth-uniform contact-collar erasure

For every \(q\ge1\), every exact cut \(k\), and every coincidence-flat test,

\[
 \|\mathcal C^{\rm mom}_{a,k,m}(F)\|_{L^q(\mu_{a,k})}
 \le C_{\theta,\delta}^m(mq)^m
          (b_a a^\delta)^m\,\nu_{s_m}(F).
 \tag{CS.17}
\]

For the centered fixed representatives (CS.1), set \(b_a=1\). In particular,

\[
 \mathfrak m_m(\mathcal C^{\rm mom}_{a,k,m}(F))
 \le C_{\theta,\delta}^m a^{\delta m}\nu_{s_m}(F)
 \tag{CS.18}
\]

uniformly in the total RG depth and volume, with all retained geometries and
all successful or residual operation counts included in the stated actual
outer law. This is not conditioning on a prescribed rare geometry.

The corresponding smeared conditional connected coefficient obeys

\[
 \|\mathcal C^{\rm conn}_{a,k,m}(F)\|_q
 \le C_{\theta,\delta}^m m!(mq)^m
           (b_a a^\delta)^m\,\nu_{s_m}(F).
 \tag{CS.19}
\]

These are averaged estimates; they do not give a supremum at a selected
retained configuration.

**Proof.** Conditional expectation is an \(L^q\) contraction between the
actual two marginals. By Hölder and (CS.4),

\[
 \|M_{I,k}(X)\|_q
 \le\left\|\prod_{i\in I}\Phi_i\right\|_q
 \le (C b_a a^{-4}mq)^m,\qquad |I|=m.
 \tag{CS.20}
\]

On the collar choose a close pair and move it to its midpoint, changing only
the eight coordinates of that pair. Taylor's theorem normal to its diagonal,
with the first \(N_m-1\) jets zero, yields

\[
 \chi_{a,m}(X)|F(X)|
 \le C_{\theta,\delta}^m r_a^{N_m}\nu_{s_m}(F)
                                      (1+|X|^2)^{-3m}.
 \tag{CS.21}
\]

One can sum over all at most \(m(m-1)/2\) choices instead of selecting a pair;
this factor is absorbed in \(C^m\). The Taylor displacement is bounded by one,
so comparison of the Schwartz weights costs only \(C^{s_m}=C_{\theta,\delta}^m\).
The derivative order is linear in \(m\), not quadratic.

The current physical Riemann sum satisfies

\[
 a^{4m}\sum_X(1+|X|^2)^{-3m}\le C^m,\qquad 0<a\le1,
 \tag{CS.22}
\]

uniformly in the finite periodic restriction. For example,
\((1+\sum_i|x_i|^2)^{3m}\ge\prod_i(1+|x_i|^2)^3\), and each
four-dimensional weighted lattice sum is uniformly bounded. Minkowski for
this **physical source-position sum**, followed by (CS.20)–(CS.22), gives
\((C b_a mq)^m a^{-4m}r_a^{N_m}\nu_{s_m}(F)\).
Since \(r_a^{N_m}\le a^{(4+\delta)m}\), this is (CS.17).
It is not a Minkowski sum over rare carrier shapes.

For a term of the partition formula (CS.10), assign to a block \(B\) of size
\(n_B\) the moment order \(q_B=mq/n_B\). Then

\[
 \|M_{B,k}\|_{q_B}
                \le(C b_a a^{-4}mq)^{n_B}.
\]

Hölder bounds the whole product by
\((C b_a a^{-4}mq)^m\). Finally
\(\sum_{\pi\in\Pi_m}(|\pi|-1)!\le 2^{m-1}m!\).
The same Taylor and source-position sum prove (CS.19). \(\square\)

For a finite F01 prescription, (CS.17)–(CS.19) retain \(b_a^m\).
If F05 later proves a fixed logarithmic budget \(b_a\le C(1+|\log a|)^r\),
the per-label factor \(a^\delta\) pays it at a smaller fixed power of \(a\).
This implication is explicit; the required F05 premise has not been supplied
by the contact calculation.

No extra moment grade is needed for (CS.18). The margin is the extra normal
Taylor order \(\delta m/\theta\), hence still a test seminorm of order linear
in the number of fields. This differs from spending a moment-grade surplus
to obtain a polynomial rare-component gain.

## 4. The exact contact-neutral source quotient

At each finite cutoff, consider scalar source counterterms of order at least
two supported strictly on coincidence diagonals. A typical term is

\[
 L_{a,r}(J)=\sum_x a^4 c_{a,r,\boldsymbol\gamma}(x)
                   \prod_{\ell=1}^r\partial^{\gamma_\ell}J(x),
 \qquad r\ge2.
 \tag{CS.23}
\]

The derivatives \(\partial^{\gamma_\ell}\) in (CS.23) act on the
continuum source/test arguments. They are not lattice finite
differences: a finite difference can move a source point by a nonzero
lattice spacing and therefore produces a shrinking stencil rather
than a strictly diagonal distribution.

Its source derivatives are distributions supported where those \(r\)
source positions coincide. Finite tensor labels and finitely many derivatives
at each order are permitted. Coefficients can also be retained-state-valued
when the statement concerns a conditional jet, provided the indicated
finite-cutoff moments exist.

### Theorem CS.3 — diagonal contacts are neutral on the flat hierarchy

Multiplying the exact source jet by \(e^{-L_a(J)}\), where \(L_a\) has no
constant or linear term and every higher coefficient has the support just
specified, leaves every \(m\)-point coefficient unchanged on coincidence-flat
joint tests. The statement holds both for the exact conditional jet and for
its actual full-law average.

Likewise, a local nonlinear source substitution with prescribed linear part,

\[
 \Psi_a(J)(x)=Z_aJ(x)
                +\sum_{r\ge2}\Psi_{a,r}(J,\ldots,J)(x),
 \tag{CS.24}
\]

has, on this quotient, only the effect of that linear part when every
\(\Psi_{a,r}\) is a finite differential expression at the same physical point.
The linear \(Z_a\) and the linear identity subtraction are retained exactly.

**Proof.** Differentiate the finite formal product or composition to order
\(m\). Every term other than the prescribed linear transport contains a
counterterm block with at least two source labels. That block is supported
on its coincidence diagonal, and the other blocks involve disjoint label
sets. Tensoring with the latter cannot remove the diagonal support.
Every derivative of the test vanishes there, so the term pairs to zero.
This is a finite-cutoff distributional identity before taking a limit.
Conditional integration acts only on its coefficient and leaves the source
support unchanged. \(\square\)

This is contact neutrality, not a construction or estimate of the actual
F06 extraction coefficients. A source term supported throughout a fixed
physical cell is not a diagonal contact. A lattice stencil supported within
a shrinking collar is not exactly neutral either; it requires an amplitude
and derivative budget, with a bound such as Theorem CS.2. That theorem applies
directly to the actual raw moment/conditional-cumulant coefficients, not to
arbitrary larger subtraction coefficients chosen afterward.

The quotient also does not identify the retained-data carrier of a
conditional coefficient. Source-position support and dependence on retained
raw fields are different questions. A diagonal source contact can have
nonlocal retained coefficients; conversely a localized retained function
need not be a source contact.

## 5. Reflection positivity on the separated flat tests

Use the actual Wilson reflection and the F01 tensor reflection law. At finite
cutoff take a finite polynomial of the physical centered fields whose
smearing kernels are coincidence-flat and supported at positive physical
time at distance at least \(\epsilon>0\) from the reflection plane. Include
the fixed microscopic stencil padding, which fits for sufficiently small
\(a\). The original Wilson reflection positivity gives

\[
 \mu_a[(\Theta P)P]\ge0.
 \tag{CS.25}
\]

A kernel in this quadratic form is the tensor product of a reflected
negative-half kernel and a positive-half kernel. It is flat at coincidences
within each half. Cross-half diagonals have an open neighborhood disjoint
from its support, because the halves are separated by \(2\epsilon\).
Thus it belongs to the full coincidence-flat class.

Theorem CS.3 shows that strict diagonal scalar or operator-valued source
contacts of degree at least two do not change (CS.25). The explicit physical
centering in (CS.1) also preserves positivity: it subtracts a real constant
inside the original positive-half algebra. The exact transported moment
identity (CS.8) gives the same number after complete history integration.
It is unnecessary, and generally incorrect, to assert reflection positivity
of an individual conditional history law.

Removing the shrinking collar in Theorem CS.2 need not preserve finite-cutoff
positivity exactly. Its error in each fixed reflection form tends to zero
with the displayed bound, so any limit of the remaining separated hierarchy
inherits nonnegativity. This preserves the corrected OS meaning of the
flat-test route without asserting a probability law for an arbitrarily
contact-subtracted field.

## 6. What has and has not moved

The following bridge is now explicit:

1. Start from the actual centered microscopic F01 reference fields, with the
   exact finite identity coefficient and the compact moment reserve.
2. Apply the source-free positive kernels to the whole finite jet. The same
   microscopic insertion, every higher vertex and every outer conditional
   mean remain in the exact identity.
3. Sum complete physical history labels before any physical selector-current
   estimate. Source derivatives never vary that frozen partition.
4. Remove a shrinking source-position collar on coincidence-flat tests with
   the uniform, all-order estimates (CS.17)–(CS.19).
5. Work modulo genuinely diagonal higher source contacts while retaining the
   linear normalization and identity budgets. Reflection positivity on the
   separated flat tests is unchanged.

There is still no cutoff-uniform estimate on the complementary region
\(\min_{i<j}|x_i-x_j|>a^\theta\) for the physically matched interacting
hierarchy. The shrinking-collar estimate cannot be used to bound that
complement by the same crude \(a^{-4m}\) bound. In particular it does not
control the full outer means merely because all conditional laws are
well behaved.

The AC moment-dependent carrier norm can be used if an actual source-marked
catalog for this complementary region is constructed. The source of that
catalog must be (CS.6), and the joint event/energy reserve must use its actual
full law. The present proof does not supply its complete retained-data
support, its raw/history currents, or the F05 coefficient budget.

No frozen completion is added: M04, M07, F05 and the full continuum existence
problem remain open. The new result is an actual full-history microscopic
source transport and contact-neutral estimate, not a redefinition of those
acceptance tests.

## Appendix. Why a vacuum-only pressure shortcut addresses a different target

The finite-cutoff estimates give
\(\operatorname{Var}_{\mu_{n,\beta}}S\ge c n^4/\beta^2\) for the bare Wilson
action \(S=\sum_p s_p\), on the admitted weak even-torus trajectory (T1,
Proposition 7.103). A deterministic linear vacuum subtraction does not change
that second source coefficient. The divergence is compatible with a contact
term and does not contradict the coincidence-flat hierarchy.

One can sharpen the probabilistic observation without a new source
assumption. Select \(n^4/2\) direction-one links with even transverse parity.
No plaquette contains two selected links. Conditional on all other links,
their one-link laws are independent. The good-staple event and the uniform
one-link Laplace analysis in that proposition give, for the centered scaled
star energy \(Y_b=\beta(\phi_b-\nu\phi_b)\),
\[
 \operatorname{Var}Y_b\ge c,\qquad \mathbb E|Y_b|^3\le C,
 \tag{CS.A1}
\]
uniformly on good stars. The third moment follows by the same quadratic
domination, inserting one more fixed polynomial power. The expected bad-star
fraction is \(O(\beta^{-1})\), so with probability \(1-O(\beta^{-1})\) at least
a fixed positive fraction are good.

Symmetrization and the third moment give a fixed \(t_0>0\) with
\(|\mathbb E e^{itY_b}|\le e^{-ct^2}\) for \(|t|\le t_0\).
For a sum of \(M\) good independent stars this becomes \(e^{-cMt^2}\).
The nonnegative kernel \((\sin u/u)^2\), whose Fourier transform is supported
on \([-2,2]\), then gives its concentration function bound
\[
 \sup_c\mathbb P\!\left(\left|\sum_{b=1}^M Y_b-c\right|\le R\right)
                   \le C(R+1)/\sqrt M .
 \tag{CS.A2}
\]
For completeness, if \(Y_b'\) is an independent copy, then
\[
 |\varphi_{Y_b}(t)|^2
 =\mathbb E\cos(t(Y_b-Y_b'))
 \le 1-t^2\operatorname{Var}Y_b
                +|t|^3\mathbb E|Y_b-Y_b'|^3/6.
\]
This proves the stated fixed small-\(t\) estimate. Write
\[
 K(u)=(\sin u/u)^2
       =\tfrac14\int_{-2}^{2}(2-|s|)e^{isu}\,ds.
\]
It obeys \(K(u)\ge\sin^2(1)\) for \(|u|\le1\). With
\(R'=\max(R,2/t_0)\), its expectation bounds the interval probability by
\[
 C R'\int_{-2/R'}^{2/R'}|\varphi_{\sum Y_b}(t)|\,dt
       \le C R'/\sqrt M.
\]
Thus only \(|t|\le t_0\) is used; no concentration-function theorem is
imported. Independent
bad-star contributions cannot increase the concentration function.
Therefore, for every deterministic centering \(c\),
\[
 \mathbb P_{\mu_{n,\beta}}(|S-c|\le R)
 \le C/\beta+C(\beta R+1)/n^2.
 \tag{CS.A3}
\]

At fixed physical volume with \(\beta=O(\log a^{-1})\) and \(n\asymp a^{-1}\),
the right side tends to zero for fixed \(R\). Thus identity subtraction alone
does not give tightness of this ordinary bare random variable. This stronger
statement is still about a test that is **not** coincidence-flat at second
order. It neither refutes the required separated-point hierarchy nor
requires probability-field tightness as a substitute for the corrected OS
target. Nonlinear diagonal scalar contacts change the second source jet;
their neutrality on the intended tests is the constructive point of
Sections 3–5.
