# Compare two history masks by a positive energy reserve

This abstract reduction removes an unnecessary requirement from the
first-birth comparison: a common finite density need not itself be
proved Gaussian, nor must its entire support be convex. A positive
exponential energy reserve and a deterministic energy cost for a
failed alternative test suffice. The actual Wilson application is
conditional on the explicit source inputs in Section 5. No M-04
status changes.

## 1. Retain the two outside completion factors

Let \(\rho\) be a positive measure on a common finite readout space,
\(H_s,H_t\) measurable sets, and \(C_s,C_t>0\) the actual factors
from unexposed integrations. Put

\[
 d\mu_i=1_{H_i}C_i\,d\rho,\qquad m_i=\mu_i(1)>0.
 \tag{AE.1}
\]

Assume only the relative completion comparison

\[
 e^{-\epsilon}\le C_s/C_t\le e^\epsilon
 \quad\hbox{on }H_s\cup H_t .
 \tag{AE.2}
\]

This hypothesis concerns the complete factors. It is not supplied
by a finite rank bound, Fubini, or geometric refinement. OC.1 gives
one route to it. A positive near-density correction may be included
in \(C_i\), if its whole ratio has the stated bound.

Let \(E_i\ge0\) on \(H_i\). Suppose

\[
 H_s\setminus H_t\subset\{E_s\ge H\},\qquad
 H_t\setminus H_s\subset\{E_t\ge H\},
 \tag{AE.3}
\]

and, for some \(\theta>0\),

\[
 \int e^{\theta E_i}\,d\mu_i\le A_i e^{D_i^+},
 \qquad m_i\ge A_i e^{-D_i^-}.
 \tag{AE.4}
\]

The positive \(A_i\) must be identical in the upper and lower
bound for each \(i\). A very small birth factor cannot occur in
only one bound. Agreement between \(A_s\) and \(A_t\) is not needed.

## 2. Exact comparison theorem

Set

\[
 \delta_i=\exp(D_i^++D_i^- -\theta H),\qquad
 \delta=\max(\delta_s,\delta_t)<1.
 \tag{AE.5}
\]

Then

\[
 \boxed{\quad
 e^{-\epsilon}(1-\delta_s)
 \le {m_t\over m_s}
 \le {e^\epsilon\over1-\delta_t}.
 \quad}
 \tag{AE.6}
\]

Consequently,

\[
 |\log(m_t/m_s)|\le\epsilon-\log(1-\delta)
 \le\epsilon+2\delta\quad(\delta\le1/2).
 \tag{AE.7}
\]

**Proof.** Markov's inequality and (AE.3)--(AE.4) give
\(\mu_i(H_i\setminus H_j)\le\delta_i m_i\). On the intersection,

\[
 m_t\ge\int_{H_s\cap H_t}C_t\,d\rho
 \ge e^{-\epsilon}\int_{H_s\cap H_t}C_s\,d\rho
 \ge e^{-\epsilon}(1-\delta_s)m_s.
\]

Interchanging the indices gives the upper bound. There is no
signed cancellation or lower bound on an extensive all-good
probability. QED.

The two energies may differ. Each must control failure of the
other exposed mask in its own actual measure. A common quadratic
is a useful way to verify that fact, not an extra premise of AE.6.

### Fractional masks: compare only on a low-energy set

There is an even less restrictive version. Disintegrate a common
positive full path measure over a finite readout \(u\), and let

\[
 h_i(u)=\mathbb E[1_{\mathcal H_i}\mid u],\qquad
 d\mu_i=h_i(u)\,d\rho(u),\qquad 0\le h_i\le1.
 \tag{AE.7a}
\]

These are the exact fractional masks of FD.2. Let \(L\) be any
common measurable set such that

\[
 e^{-\epsilon}h_s(u)\le h_t(u)\le e^\epsilon h_s(u)
 \quad(u\in L),\qquad
 \mu_i(L^c)\le\delta_i m_i.
 \tag{AE.7b}
\]

Then AE.6 follows verbatim by comparing the masses on \(L\).
Zeros on \(L\) are permitted; the inequalities, rather than a
ratio with zero denominator, are the correct formulation.

A useful sufficient source construction is \(L=\{E_{\rm ref}<H\}\).
If every exposed near selector of both histories is true on \(L\)
uniformly over the admitted far fiber, then \(h_i\) on \(L\)
contains only the corresponding far cutoff completion. OC may
compare those two factors without making near selectors measurable
in \(u\) outside \(L\). A matched restored-energy reserve bounds
\(\mu_i(L^c)\).

The uniformity over the far fiber is substantive. An averaged
background displacement or a statement valid only at one far
reference field does not supply it. The relative completion
comparison is still about the same physical conditional fiber.

## 3. Birth factors, a whole family, and tilts

If the actual first-sector factor satisfies

\[
 e^{-\eta}w_i\le b_i(v)\le e^\eta w_i ,
 \tag{AE.8}
\]

compare reduced masses \(m_i/w_i\), including \(b_i/w_i\) in the
completion factor. The exponent in AE.2 increases by at most
\(2\eta\). For whole-pattern translations with equal \(w_i=w\),
AE.6 compares the actual masses. Replacing \(b_i\) by \(w_i\)
without its relative error is not an exact identity.

If \(J\) disjoint original histories have all pairwise mass ratios
in \([K^{-1},K]\), their sum is at least \(Jm_i/K\). Thus, even
if other histories occur,

\[
 \frac{\text{mass of history }i}{\text{total mass}}\le K/J.
 \tag{AE.9}
\]

Disjointness refers to the original first R patterns. The later
masks after factoring that R integral need not be disjoint.

Let \(E\ge0\) be a common finite readout and replace \(\rho\) by
\(e^{tE}\rho\). If the upper bounds AE.4 hold with this insertion
and the same budgets, the lower bounds still hold. Completion
ratios and set inclusions do not change. Hence AE.6--AE.9 hold
also for the tilted masses. This requires a genuinely common
\(E\); distinct projected Schur energies cannot be substituted
without a further comparison.

## 4. Deterministic linear test bounds suffice

Suppose that, on the actual union of masks in a common chart,

\[
 E_i(z)\ge\tfrac12 z^\mathsf TKz-\varepsilon_E ,
 \tag{AE.10}
\]

where \(K>0\). Suppose an alternative test requires
\(\|Lz+b+R(z)\|\le p_1\), with
\(\|b\|+\|R(z)\|\le p_1/2\), and

\[
 \|Lz\|^2\le v\,z^\mathsf TKz .
 \tag{AE.11}
\]

Failure implies

\[
 E_i(z)\ge p_1^2/(8v)-\varepsilon_E .
 \tag{AE.12}
\]

For a fixed-dimensional test, AE.11 is checked by
\(\|LK^{-1}L^*\|\). Gauge null directions must first be removed
or proved invisible to \(L\).

In a correctly identified flat joint quadratic, exact Schur
minimization transfers the corresponding original test-energy
bound to AE.11. This is a statement about energy alone. It needs
neither a determinant comparison nor a convex nonlinear mask.
The source estimate \(v\le CR^9\), if verified for this same
restored quadratic, gives \(H=cR^{-9}p_1^2-o(1)\).
Replacing the exponent 9 by an unspecified larger polynomial
requires a fresh check of the parameter hierarchy.

## 5. Actual source interface still to be proved

The LE result proves AE.4 for the positive energies
explicitly present in its original fixed list. It does not
automatically prove it for newly restored alternative modes.
The proposed shorter application has five specific inputs:

1. Expose both finite raw/free lists with declared collars by
   complete conditional identities, retaining terminal average
   deltas, coarea and normalization factors.
2. Bound that same restored integral with \(e^{\theta E_{\rm ref}}\).
   FD suggests dropping remaining positive forms after LE's
   first-energy cancellation. The nonenergy bound, coordinate
   volume and normalization must hold for this enlarged
   measure, not only its unextended predecessor.
3. Match that upper bound with LE's lower bound for the original
   mass. Both must have the same birth weight and retained
   reference factor. The target loss is \(O(D_{\rm late})\),
   or an explicitly verified fixed logarithmic enlargement.
4. Check every literal alternative test against this energy,
   directly or through AE.10--AE.12. WA provides a polynomial
   analytic radius; it does not identify \(K\) or prove AE.11.
5. Compare every unexposed completion relatively by OC or an
   equivalent argument. Later Omega domains still depend on
   the first R position.

These inputs are less than a full common Gaussian density theorem,
but remain substantive. This note proves the reduction, not the
complete source application.

## Dependency record

- M04_Later_Energy_Reserve.md, LE.4--LE.19: matched birth
  weight, original fixed-list energies and later reserve.
- M04_Refined_Forest_Density.md, FD.2, FD.7--FD.10: proposed
  restored-energy ledger and its completion boundary.
- outside_completion_comparison.md, OC.1--OC.16: exact
  moving-cutoff completion comparisons.
- mixed_weighted_averaging.md, WA.16--WA.22: analytic radius
  and literal raw/gauge conversion.
- common_reference_exchange.md: the stronger Gaussian-based
  sufficient route.
