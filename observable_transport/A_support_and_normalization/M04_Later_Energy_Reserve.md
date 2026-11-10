# A first-birth factor can be retained in the later-energy upper bound

This note proves the canceled-first-energy SELF bound and then restores
the actual first R-birth factor before integrating the later data. It
also gives the matched later-only lower bound. The result concerns the
original h=1, Ω₁-full, globally P/Q-regular first-birth family with a
bounded R neighborhood and the literal quiet rectangular-chain
preparation. It is a theorem for the whole first R-pattern event in
that family, not a replacement of that event by its trial box.

The complete old posterior can additionally contain initial P/Q sectors,
other first components outside this bounded family, and inherited
histories after earlier replacements. Those scope changes are not
covered by the result below. The comparison of two different quiet
masks also needs the common-refinement estimate stated in Section 7.

## 1. One normalization and one common first baseline

Fix the current retained data v, one complete fresh-reference class r,
and the actual unreplaced exterior. The class records the prepared
core, fresh graph, reference/cutoff choices and all the fixed source
rules. Let s denote an entire admissible first R pattern leading to
this class after a quiet window. All overlapping good and bad first
tests remain in s. The union of its first retained coordinates is D_s;
write n₀ for its scalar rank. The source bounded geometry gives

\[
 n_0\le C R^4,\qquad
 \sum_{j=1}^k\bigl(|Z_j|+D_j\bigr)\le C R^5,
 \qquad k=N+1,
 \tag{LE.1}
\]

where volumes and independent ranks use their own source lattices.
Constants may include the fixed number of ancestral rectangles. There
are no surviving pre-first-step coordinates in this scope.

Use the post-classical-cancellation convention of LFR II (1.71), as in
RT.1–RT.4. Factors depending only on the retained data and the fixed
unreplaced exterior are divided out once. The same factors are divided
out for every s with this r. In particular this convention is not
changed after a first Gaussian energy is inserted.

Let M_s^self be the positive self-operation restricted to s and the
prescribed later quiet/preparation outcomes. The complete component
mass has the form

\[
 M_s^{\rm full}(F)=M_s^{\rm self}(F e^{H_Y}),
 \tag{LE.2}
\]

after the cross terms independent of Y have been factored into the
outside density. The actual H_Y is retained. The absolute source
carrier sum HS20.6–HS20.7 gives, uniformly in the remaining internal
states and compatible exterior,

\[
 |H_Y|\le C\lambda_R,
 \qquad \lambda_R=C(1+R)^b e^{-cR}.
 \tag{LE.3}
\]

If the interaction is specified only up to a state-independent offset,
choose one common offset for the whole fixed Y state space and keep
that offset in the outside factor. This is the usual conditional
oscillation convention. It must not be chosen separately for different
first patterns.

Undo the complete first complement identity, not only the last annular
Gaussian integrations. FR.1–FR.8 then gives a positive common space of
later physical data and normalized gauge auxiliaries y, with actual
quiet mask H_s(y). Its retained readout is the same chronological
average on the fixed core exterior, in the common reference gauge.
Let Π_r,v be the later measure in this reassembly, including the
inverse of the just specified retained-only outside factor. In
particular it need not be a probability measure. Put

\[
 d\nu_0(y)=Z_P(V_1(y))\,\Pi_{r,v}(dy),
 \tag{LE.4}
\]

where Z_P is exactly RB.10, the original all-small first integral.
No extensive part of Z_P is omitted. The exact full operation is

\[
 M_s^{\rm full}(F)
   =\int H_s(y)\,b_s(V_1(y);F)\,d\nu_0(y).
 \tag{LE.5}
\]

Here b_s is the original first integral on the entire R event divided
by that same Z_P, with the insertion pulled back through all exact
coordinate maps. Source vacuum terms, exceptional-bond Jacobians and
the first complement completion factor are part of the equality.

Formula (LE.5) is for the full operation. A self-only source action is
not asserted to have the same primitive factorization. It is (LE.2)–
(LE.3) that will transfer a self upper bound to the correctly factored
full operation. At h=1, Γ₀ is empty, so every later test and every
later positive form is independent of the first fluctuation at fixed
y. This is the functional independence in FR.2, not probabilistic
independence of the interacting density.

## 2. The positive energy to be canceled

Let E₀^diag be the sum of the actual first diagonal Schur quadratics
in the old T₁ operations, including their original coefficient 1/2.
Let E₀ be the joint first retained Schur form on D_s, pulled back
through the first relocalization if needed. The note
[first schur cancellation source analysis](first_schur_cancellation_source_analysis.md) identifies these forms and
proves

\[
 |E_0-E_0^{\rm diag}|\le\delta_0,
 \qquad \delta_0\le C n_0P^2e^{-cMR}=o(1)
 \tag{LE.6}
\]

for several separated first components inside the bounded neighborhood.
For one first component they agree before the relocalization. The
additional relocalization error has the same bound; it is zero on the
5P/4 trial box used in EC0. The complement-cutoff factor is retained.

Fix the finite positive-form list actually present in the final source
operation (1.71), with the source independent-coordinate ranks. Define
its later energy by

\[
 E_{{\rm late},s}
    =Q_s+S_s+\sum_{j\ge1}\mathcal G_{j,s}.
 \tag{LE.7}
\]

Q is the final positive B form, S is the real positive Wilson term
left after the actual classical cancellation, and the sum includes
only ordinary positive Gaussian forms after the first step that are
still explicitly present in the specified source operation. In the
literal h=1 final formula the inner T₁ contributes only E₀, so this
additional sum is empty. No part of E₀ occurs in (LE.7). All entries
of (LE.7) depend only on y on this Ω₁-full branch.

In particular, the definition does not add all previously integrated
regular modes to the energy. Their rank could be extensive. A finite
restoration may augment this list only after its exact determinant,
cutoff completion and positive reserve have been proved to obey the
same count and upper bound. That is the separate obligation in
Section 7, not a convention built into (LE.7).

The form S is the one in LFR II (1.46)–(1.48), not the Wilson action of
the original reference-centered microscopic field. At the later trial
center B=0 and V₁=I it vanishes exactly. This distinction is essential
for the lower bound in Section 5.

## 3. The direct SELF canceled-energy upper

Set

\[
 D_{\rm late}
   =1+R^6\log(1+R)+R^5\log g_k^{-1}.
 \tag{LE.8}
\]

### Proposition LE.1

For a fixed small θ>0, independent of s, k and the cutoff, in the
preceding source scope,

\[
 M_s^{\rm self}
       (e^{E_0+\theta E_{{\rm late},s}})
       \le e^{C D_{\rm late}}.
 \tag{LE.9}
\]

**Proof.** Work first in the literal integration variables of (1.71).
Multiplication by exp(E₀^diag) cancels exactly the negative first
retained Gaussian exponent in its T₁ factor. Equation (LE.6) costs at
most exp(δ₀) when the intended joint form is used.

The actual first support is bounded by |a_b|≤CP on every independent
coordinate: a good R test gives P, and the remaining starred Q test
gives (2+o(1))P. The exceptional entries are reconstructed by C and
are not extra integration directions. The now unweighted first
Lebesgue integral is consequently at most (CP)^{n₀}. Its powers of
g, coarea constants and vacuum counterterms stay in their displayed
source normalization. They are not replaced by an additional
normalized Gaussian density.

Every later form in (LE.7) retains the fraction 1−θ of its negative
exponent. The nonnegative Q and S may be dropped for an upper bound.
Each remaining ordinary Gaussian still has a fixed positive gap, so
its integral costs at most a fixed constant per independent scalar
coordinate. This is exactly the integration estimate on LFR II p.383
after (1.78), with a smaller fixed reserve.

The absolute self-interaction bound (1.69), its vacuum terms and the
normalization paragraph on p.380 charge at most

\[
 C\sum_{j=1}^k |Z_j|\log g_j^{-2}
 \tag{LE.10}
\]

to the exponent. The group-valued integrals use normalized Haar and
are bounded by one after their actual graph deltas have removed the
tree coordinates. For B use its actual bounded domain and σ(g_kB),
keeping the displayed logarithmic Haar-coordinate factor in the last
line of (1.71). The p.383 estimate bounds their combined contribution
by the same scale-count charge. It does not count the g power twice.
Finite orientation averages cost at most one. The remaining admissible
history sums have the source bound exp[CΣ_j(MR_j)^{-4}|Z_j|]; retaining
one fixed quiet geometry can only decrease this count.

By (LE.1), source coupling comparability in this window and the literal
rectangular-chain rank estimate, all these charges are bounded by
CD_late. The first added volume n₀ log(CP) is also bounded by CD_late.
No first-birth small factor is extracted: its entire quadratic was
canceled. No inverse birth mass occurs. Combining the inequalities
proves (LE.9). ∎

The same argument remains valid on the fixed-geometry auxiliary
all-small-first domain used below. Removing a bad R alternative only
strengthens the coordinate upper cutoffs. The source analytic
identities and their interaction bounds were proved on the whole
encompassing regular chart; the lower-threshold event is used to
extract a small factor, not to define those identities.

## 4. Restore the rare first factor before the later integration

Let w_s^G be RB.14, the flat first R-defect weight with the same all-P
baseline. The two pointwise estimates are

\[
 b_s(V;1)\le e^{\varepsilon_R}w_s^G,
 \qquad
 b_s(V;e^{E_0})\ge e^{-Cn_0-\varepsilon'_R},
 \qquad \varepsilon_R+\varepsilon'_R=o(1).
 \tag{LE.11}
\]

The second is EC0.12, with the actual complement cutoff and the source
Schur form. Combining these inequalities at the same V gives

\[
 b_s(V;1)
   \le w_s^G e^{Cn_0+\varepsilon_R+\varepsilon'_R}
                      b_s(V;e^{E_0}).
 \tag{LE.12}
\]

This is the required disintegration inequality. Multiply it by the
nonnegative factor H_s(y) exp(θ E_late,s(y)), then integrate against
the same measure ν₀ in (LE.4). The result is

\[
 M_s^{\rm full}(e^{\theta E_{{\rm late},s}})
  \le w_s^G e^{Cn_0+o(1)}
           M_s^{\rm full}(e^{E_0+\theta E_{{\rm late},s}}).
 \tag{LE.13}
\]

Now, and only now, apply the complete cross-action comparison
(LE.2)–(LE.3) and the self bound (LE.9). It proves

\[
 \boxed{
 M_s^{\rm full}(e^{\theta E_{{\rm late},s}})
       \le w_s^G e^{C D_{\rm late}+C\lambda_R}.}
 \tag{LE.14}
\]

No P² term occurs in its exponent. The small original birth mass has
been retained as w_s^G, rather than divided out after an absolute
failure estimate. The cross-action loss is exponentially small in R;
in particular λ_R=o(H_R) for the preparation threshold below.

## 5. A matched lower bound uses an auxiliary first all-small operation

Define

\[
 L_s=\int H_s(y)\,d\nu_0(y).
 \tag{LE.15}
\]

There is an exact fixed-geometry representation of L_s: replace only
the first R-pattern selector in the source operation by the complete
all-P first free-coordinate cutoff. Keep D_s, every later mask, every
map, determinant, orientation weight and normalization unchanged.
Undoing the complete first complement identity makes the first
integral Z_P(V₁), which proves (LE.15). This is an auxiliary positive
integral; its first label need not be an actual all-small geometric
history. It is not substituted for the old conditional.

The first all-P domain lies strictly inside the surviving Q-good
domain. Hence the fixed-geometry analytic identities continue to
hold there. Choose its first retained coordinates in fixed small
balls about zero. Its E₀ cost is O(n₀), with no P² seed. The first
relocalization is the identity on these balls. Keep the actual
complement integration/completion factor through its source E/B
representation and the same renormalization constants; do not bound
an extensive all-P probability in isolation.

For the later variables use the RT identity-centered trial: B=0,
V₁=I, with its sufficiently thin positive-volume neighborhoods and
the literal mixed tree and seam conventions. Its admission is
unchanged because the later functions do not read the first
fluctuation. The positive Wilson term is zero at the center by
(1.46)–(1.48), the B form is zero, and their costs on the trial are
O(D_late). The two-sided combined measure-plus-nonenergy estimate
RT.15a applies on the identical fixed geometry. Its original CP²
term was solely the first large witness, which is absent here.
Consequently the auxiliary self integral is at least exp(−CD_late).
The actual nonself source bound also holds on this smaller first
domain, so (LE.3) gives

\[
 L_s\ge e^{-C D_{\rm late}-C\lambda_R}.
 \tag{LE.16}
\]

Use the lower half of RB.15 in (LE.5). This proves the matched lower
bound and hence the normalized later reserve

\[
 \boxed{
 M_s^{\rm full}(1)\ge
       w_s^G e^{-C D_{\rm late}-C\lambda_R},
 \qquad
 \frac{M_s^{\rm full}(e^{\theta E_{{\rm late},s}})}
      {M_s^{\rm full}(1)}
       \le e^{C D_{\rm late}+C\lambda_R}.}
 \tag{LE.17}
\]

This lower bound uses the whole first R event through RB.15. Applying
the original seeded RT lower bound directly would retain an unwanted
CP² in the exponent; that is why the auxiliary integral (LE.15) is
introduced explicitly.

## 6. What the reserve pays, quantitatively

On this source window the smallest preparation-failure extraction is
the one on LFR II p.383, (1.77)–(1.78), of order

\[
 H_R=cR^{-9}p_1(g_k)^2\qquad(d=4).
 \tag{LE.18}
\]

Its source hypothesis is 2p₁−9r₀>p₀ with p₁<p₀, where r₀ is the
radius-majorant exponent used in that estimate. In particular p₀>9r₀.
With the stated radius majorant r₀≥r, this strict hierarchy gives
D_late=o(H_R). Equivalently one can retain the operational inequalities
H_R≫D_late directly instead of identifying an unseen definition of r₀.
The additional λ_R=o(H_R) is immediate from (LE.3).

For any event B in this same measure for which the literal source
forms imply E_late,s≥cH_R, (LE.17) gives

\[
 \nu_s(B)\le
      \exp\{C D_{\rm late}+C\lambda_R-c\theta H_R\}=o(1).
 \tag{LE.19}
\]

This is a genuine relative estimate with the first birth factor
canceled beforehand. The energy in the premise must include the
actual relative/gauge forms. A physical Wilson-only witness cannot
replace the χ′ or old free-coordinate failure inequalities.

## 7. The sharp remaining two-mask obligation

Equation (LE.19) is not by itself an exchange theorem for two birth
geometries. Suppose s and t are whole-cluster translations with the
same r; RB gives w_s^G=w_t^G. FR supplies a common primitive readout
and a positive common space. The desired deletion-ratio argument needs
the following additional source statement on that space:

1. Reintroduce the union of the two actual annular coordinate lists,
   with every constraint, Jacobian and normalized gauge weight. Its
   source count remains O(R⁵); no union over all candidate locations
   is required.
2. On H_s\H_t, the first failed t test must give a lower bound of
   order H_R for an energy carrying a fixed reserve in that common
   s-conditioned integral. The test is evaluated using the actual
   t determining map and t gauge convention. It cannot be replaced
   by the corresponding s test.
3. The same canceled-energy upper must hold for that common positive
   reserve, uniformly for the two-list refinement, and conversely
   with s and t interchanged.

For intrinsic failures represented on the original s list, the source
proof already supplies the required implication. For a hypothetical
alternative list, it is not enough to know that each list separately
has a positive form and a bounded rank. One needs an exact simultaneous
disintegration, or a proved comparison of the two actual forms and
reference shifts. No such comparison is inferred here from an assumed
associativity of averages or from bare Gaussian independence.

If these three conditions are proved, (LE.19) on the two difference
sets gives ν₀(H_s∩H_t)/ν₀(H_s)=1−o(1) and its reverse, after the
pointwise first-weight comparisons. Thus L_s/L_t=1+o(1), and then
M_s(1)/M_t(1)=1+o(1). The remaining issue is this concrete masked
source-energy comparison; the rare first-birth denominator and the
later-only normalization cost have been removed at the scope of
Sections 1–5.

## Sources and companion proofs

- CMP119 (1.14)–(1.30), (2.19)–(2.22): independent chart, actual
  first Schur/completion identity and component factorization.
- LFR II (1.46)–(1.48), (1.69), (1.71)–(1.79), especially pp.380
  and 383: actual positive forms, absolute normalization ledger,
  measure bounds and smallest preparation-failure extraction.
- [M04 First Birth Reassembly](M04_First_Birth_Reassembly.md), FR.1–FR.8: full common path and
  Ω₁-full functional independence.
- [first birth relative weights](first_birth_relative_weights.md), RB.10–RB.16, and
  [first energy cancellation](first_energy_cancellation.md), EC0.9–EC0.12: pointwise first
  weights and the same Z_P denominator.
- [first schur cancellation source analysis](first_schur_cancellation_source_analysis.md): signed quadratic,
  collar, free-coordinate and normalization analysis.
- [residual trial mass](residual_trial_mass.md), RT.9b, RT.15a–RT.17, and the residual trial
  normalization and box analyses: later identity-centered trial.
- Annexes BI–BM, HS20.6–HS20.7: the actual full conditional cross
  action, retained in (LE.2)–(LE.3).
