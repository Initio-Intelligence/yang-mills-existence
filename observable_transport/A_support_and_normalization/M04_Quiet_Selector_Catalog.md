# Exact quiet-selector reduction and its normalization caveat

This note records which selectors remain when the actual last-window
operation is restored to a positive primitive integral. It does not replace
an integrated small-field completion by the number one. The first-family
scope is h=1, Ω₁ full, initial P/Q good, a specified first R pattern, and a
fixed final fresh-reference class. All statements below refer to the literal
source maps and their recorded gauge representatives.

## 1. The seven groups before preliminary integration

LFR I, printed p.178, (1.3)–(1.9), lists the following seven groups in each
quiet one-step operation. The domain qualifications in that display are
part of each function.

| Source | Actual function | Fate in the successful preliminary operation |
|---|---|---|
| (1.3) | Fine local-minimum plaquette test at ε_j | Replaced by the stronger successive χ_k^(n) tests and proved redundant in (1.29). |
| (1.4) | Next-scale local-minimum plaquette test at ε_{j+1} | Proved redundant in (1.29), except the terminal χ_k(Ω_k^~4) factor explicitly retained there. |
| (1.5) | Small gauge-averaging variable | Proved redundant by the approximate fluctuation restriction (1.27), as explained on p.184. |
| (1.6) | The positive normalized soft-gauge density | Remains a positive factor; the Faddeev–Popov insertion extends it over the integration region. It is not a hard success event. |
| (1.7) | Approximate Q-type relative-link test with radius 2δ_j | Proved redundant in (1.29), using (1.27), (1.40)–(1.43). |
| (1.8) | Reconstructed free-field Q-type test with radius 2δ_j | Proved redundant in (1.29), using the free cutoff (1.9) and the estimates (1.32)–(1.42). |
| (1.9) | Original ordinary free-field R-good product | **Retained.** Equation (1.28) completes this product to the whole relevant domain. It is integrated in (1.60) and its exact completion is included in (1.62). |

In particular, the sentence immediately preceding (1.29) lists
(1.3), (1.4), (1.5), (1.7), (1.8), and χ_k^(n), but not (1.6) or
(1.9). This is an exact algebraic reduction. It does not assert that the
ordinary free-field cutoff is a likely event under a different law.

The literal statement of (1.9) is

\[
 \chi\{\sup_b |A_j(b)|<g_j^{-1}\delta_j\},
 \qquad \delta_j=g_j A_1p_0(g_j),                     \tag{QS.1}
\]

on the stated starred free domains. Thus this particular displayed
cutoff has dimensionless radius A₁p₀(g_j). Later normalized notation must
be checked separately; the source does not license changing the variable
while retaining its old radius.

## 2. The actual new preliminary masks

The successive determining sets are (1.14)–(1.20). At stage j the source
introduces, in order:

1. The next localized curvature function χ_k^(n+1), (1.24).
2. The approximate fluctuation test χ′_j, (1.27), comparing V_j with the
   actual localized reference V_Z^(j), with physical link radius 2δ′_j.
3. The added ordinary free-field good product (1.28).
4. After the exact averaging-constraint change and scaling, the free
   preparation test χ′^(j), printed in (1.55).

The approximate test has

\[
 \delta'_j=g_j A_1p_1(g_j),\qquad p_1<p_0,             \tag{QS.2}
\]

as stated on printed p.183. The exact relative field in (1.53) is

\[
 V'_j=V_j(V^{(j)})^{-1},\qquad
 V^{(j)}=M^j(U_k^{(n+1)}),\qquad
 B'_j=(1/i)\log V'_j.                                \tag{QS.3}
\]

The paragraph on printed p.187 then linearizes the actual group deltas,
uses the exceptional-bond solve, and scales B′_j=g_j B_j. The successful
integral (1.60) contains both the ordinary A_j cutoff and χ′^(j), together
with their two full positive quadratic forms and the interaction. The
conditional completion of this integral is the boundary term in (1.62).
Undoing that completion restores its actual two-variable integral and
both actual cutoffs. Its logarithmic boundary expansion is not a
pointwise replacement for those events.

On the unsuccessful χ′^(j) sector only, (1.58)–(1.59) make the usual
localized variable change. Its complete Jacobian must be kept when that
sector is restored. The source does not perform this extra change on the
successful sector.

## 3. The final preparation and the identity-filled seam

After the preliminary annular integrations, LFR I (1.74)–(1.79) defines
the fixed reference U₀ and the retained-field regularity function χ_{k,Λ}.
The final old integral in (1.76) uses the mixed determining variables V″.
On the literal set

\[
 \Lambda_0=\Lambda\cap\Omega_{h+1}^{\prime\prime\,\sim2},
 \qquad B_0=\mathbb B_k^{\prime\prime}\cap\Lambda_0,
                                                               \tag{QS.4}
\]

with the printed tilde convention, (1.81) defines
V″=V′V₀, V₀=M_{B″}(U₀). The source explicitly includes the outer Λ
boundary-crossing bonds and excludes the inner Ω″_{h+1}^{~2} boundary-crossing
bonds. The single mixed tree T₀ fixes the relative gauge of V′. The final
test (1.82) is the physical-field condition

\[
 V'=e^{iB'},\qquad |B'(b)|<\delta'_k\quad(b\in B_0).
                                                               \tag{QS.5}
\]

Here there is no scaling ambiguity: LFR II printed p.362 explicitly
states that the dimensionless field B satisfies |B|<g_k^{-1}δ′_k.

The final inner test (1.88) is not a test of bare V_h. The field denoted
(1,V_h) is filled by the identity on the indicated inner regular set and
by V_h on its complement. The test applies the actual local variational
map U_{h,□} to that filled field and imposes the half-ε_h plaquette bound.
In particular it tests cubes crossing the artificial seam. Cubes wholly
inside the identity-filled domain contribute the number one, as the source
explains on printed p.198.

One must first make the stated AL gauge change of U₀ and its compensating
changes of V_h and V′, as described after (1.87). The identity-filled field
depends on this representative. It is incorrect to call this test
invariant under arbitrary gauge changes of V_h alone. The proof in
(1.90)–(1.96) controls the seam by comparing the actual field with
(1,V_h), using both B′ and the small AL reference. Equations (1.97)–(1.98)
then propagate the bounds through the remaining mixed annuli.

The exact result is (1.89): with χ_{k,Λ}, the final χ′, and the inner
χ_{h,1/2} in place, the old final χ_k″ and χ_h(Ω_h∩Z_h) are redundant.
This proves the removal of the final curvature function; it does not
remove any earlier completed ordinary or preparation product.

## 4. What a restored near-mask catalog can legitimately contain

After the exact identities above, the initial first R pattern can be
factored as b_s conditional on the full V₁, as in FR/RB. The other
history-dependent success factors on the full restored path are:

* the ordinary R-good products remaining from (1.9)/(1.28), with their
  actual source free coordinates;
* the actual free preparation cutoffs χ′^(j) from (1.55), and any
  approximate χ′_j not yet removed by the exact successful free-chart
  identity;
* the final mixed relative cutoff (1.82);
* the identity-filled inner half-curvature test (1.88);
* the retained-only χ_{k,Λ} and terminal regularity functions already
  fixed by the common fresh-reference class.

The soft-gauge factors remain in the positive primitive density. They may
be sampled with the actual small-w law, retaining its support and its
exact normalization. Their independence in the source w variables is
the endpoint-covariance identity recorded in MT; it does not justify
discarding their contribution after a different gauge coordinate change.

For a common finite refinement, all changed test footprints and their
source averaging/interface collars must be exposed. Ordinary products
outside that refinement are completed conditionally and compared by a
relative completion theorem. The present catalog alone supplies neither
such a theorem nor a uniform low-energy implication.

## 5. A literal normalization obstruction to the proposed low-energy shortcut

There is a genuine printed discrepancy at (1.55). The printed p.188
reads

\[
 \chi'^{(j)}=
 \chi\{|B_j(b)|<\delta'_j\text{ on the starred domain}\}.
                                                               \tag{QS.6}
\]

The preceding paragraph has already scaled B′_j=g_j B_j. On the same
page, (1.59) uses exp(i g_j B_j), and (1.60) has the quadratic form
\(\frac12(B_j,K_jB_j)\), with no g_j^{-2}. Together with (QS.2), the
literal dimensionless radius in (QS.6) is g_j A₁p₁(g_j). A same-page
notation reversion does not reconcile these three displays.

Consequently, the literal failure |B_j|≥g_j A₁p₁ can occur with positive
quadratic energy of order g_j²p₁². It cannot be assigned an energy cost
of order p₁²/R⁹. Already on a single fixed-dimensional positive Gaussian
mode, a ball of radius g_jp₁ has probability tending to zero, rather than
a failure probability bounded by exp(−c p₁²/poly(R)). This elementary
comparison is about the printed normalized coordinate; no rare-event
denominator is involved.

LFR II printed p.381 separately discusses failures of (1.27), (1.28),
χ_{j,Λ}, and the final (1.82), but does not provide a separate explanation
of (1.55). The final (1.82) has consistent normalization, as noted above.
The specified statement of the problem also records an analogous unresolved normalized
cutoff issue for CMP119 (3.16). At the time of this analysis, no explicit
correction of (1.55) has been found in the specified reset documents.

The intended formula may well be |B_j|<g_j^{-1}δ′_j. That correction
would make the p₁ energy scale consistent with the construction. It is
not the displayed formula and must be recorded as a convention repair
before it is used in the specified-law proof. Alternatively one must keep
the literal small balls and compare their conditional masses
multiplicatively; a large-probability intersection argument would then
require a different justification.

This discrepancy does not invalidate the exact change-of-variables or
first R-factor identities. It prevents the present source catalog from
proving the proposed statement that every near success factor equals one
on a common set E_*<c p₁²/R⁹.

## Sources

The printed pages used are Large Field Renormalization I, pp. 183, 188. The rest of the reduction follows the
literal LFR I (1.14)–(1.29), (1.53)–(1.62), and (1.81)–(1.98), and LFR II
pp.380–383.
