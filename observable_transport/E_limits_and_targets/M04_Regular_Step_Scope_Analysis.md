# M-04 is a regular one-step operator estimate under an incoming budget


**Conclusion.** The M-04 statement does not require proving the entire old-history reset estimate or the propagation of the microscopic scalar through the preceding depth. It requires the exact next regular output of an already specified incoming scalar, under an explicit, independently stated input budget. The first-birth dilution and microscopic background-root questions are useful for later reset/full-history work, but they are not logically necessary for every proof of this regular-step statement. The complete inherited boundary action, its actual current dependence, physical carriers and the full M-03 output norm remain necessary.

This is a scope analysis, not a completion of M-04.

## 1. The stated problems are separate

The M-04 statement in the scalar insertion problem asks for:

> At one RG step, expand the actual transported scalar insertion in the fixed incoming reference basis of F-01, under an explicit one-step induction budget, into the current scalar basis, identity term and a localized remainder.

Its required conclusion is equality with `Q_k F_k`, with a uniform M-03 remainder estimate. The words “one regular step” are part of its title. The required density includes the constrained background, inherited E/B/R responses and coarea terms present in that sector.

The distinct H-04 statement asks to sum **regular, repaired, residual and inherited bad sectors** in the full normalized law for inputs satisfying the M-03/M-06 induction budget. M-07 asks to iterate the actual steps with a current-scale budget uniformly in total depth. H-05 asks for the outer retained-mean covariance and cumulants.

These statements allow a regular one-step theorem to assume a genuine input budget. They do not allow that theorem to assume its own marked output estimate, erase current dependence from the density, or substitute a newly inserted coarse scalar for `F_k`.

## 2. What is the actual incoming field?

Let the source-free positive construction have augmented states `X_k` and transition kernels `P_k(X_k,dX_{k+1})`. The augmentation retains the continuous and discrete data needed by the subsequent maps. Let `q_k(dx|y)` be the actual reverse conditional law of `X_k` given `X_{k+1}=y` under that construction. Then

\[
 (Q_k F_k)(y)=\int F_k(x)q_k(dx\mid y).
 \tag{MS.1}
\]

The incoming scalar is the already specified function `F_k` on the incoming augmented state. If it is the exact transported microscopic scalar,

\[
 F_k=Q_{k-1}\cdots Q_0 F_0,
 \tag{MS.2}
\]

then its earlier conditional integrations are part of that function. The Markov/tower identity gives

\[
 Q_k F_k=Q_k Q_{k-1}\cdots Q_0F_0.
 \tag{MS.3}
\]

There is no requirement to undo all earlier integrations and re-prove a bound for the bare microscopic insertion in order to prove a one-step operator theorem for (MS.1). The input budget may be hard to establish for (MS.2); that is a propagation problem, and must be recorded as such.

Conversely, a theorem proved only for a fresh plaquette `phi_k` cannot be applied to (MS.1) by declaring `F_k=phi_k`. One must either prove the theorem for the stated incoming class and insert the actual `F_k`, or provide the actual prior matching expansion and its budget.

## 3. The incoming budget in Annex BK is expressly an induction hypothesis

[Annex BK](../../history/Annex_BK.md) §1 gives the concrete representative

\[
 F_h(U)=h^{-4}\alpha\beta
           \sum_{p\in\mathcal P(S)}a_p s(U_p)-c
 \tag{MS.4}
\]

and proves its compact-centered local analytic bound

\[
 \sup_{|\zeta|\le\rho}|F_h(U(\zeta))|
 \le C_\rho b h^{-4}\,[1+E_S(U)],
 \qquad b=|\alpha|+h^4|c|.
 \tag{MS.5}
\]

Immediately after that proof the annex says that actual support, a bound of this kind, its exposed coefficient sum and the specified direct/current records form a nonvacuous incoming one-step hypothesis. It explicitly does **not** prove that every previously transported scalar has this hypothesis; propagation remains an induction task.

Thus an admissible M-04 theorem can begin with a specified carrier representation

\[
 F_k=\sum_{X,\ell}F_{k,X,\ell}
 \tag{MS.6}
\]

and a source-independent input budget on its local analytic values, direct records, old current records and actual native regulators. The activity tags `ell` must remain distinct before taking absolute sums. The budget can include the fixed incoming scalar coefficient and a previously generated localized remainder. It is not restricted to a bare plaquette.

The crucial restrictions are:

- the carrier and analytic estimates concern the input functions before the current integration;
- the budget exposes all physical scale factors and coefficient magnitudes;
- the current coordinate pullback is proved or charged through its actual source map;
- the budget is not defined to be the unknown current root-activity sum or output norm.

For example, `B_in=||Q_k F_k||_{M03}` would be tautological. A prescribed local input bound like (MS.5), summed over the known input carriers and combined with their existing direct/current records, is not tautological. Establishing its next-step preservation is exactly the substantive operator estimate.

The factor converting a known microscopic bound to an input-scale bound also remains explicit. A bound `b_0 a^{-4}` expressed at scale `h` has input coefficient `(h/a)^4 b_0`; it is not a depth-uniform current-scale `b_0` budget.

## 4. A regular primitive step can retain the old payload

In common coordinates for a primitive regular operation write the input as `(a,y)`, where `a` is the current regular free field to be integrated and `y` includes the actual retained old payload, geometry, coarse field and exterior. With the exact coordinate map `chi`,

\[
 (Q_kF_k)(y)
 =\frac{\int_{\mathcal D_y}
             F_k(\chi(a,y))\,e^{L(a,y)}\,da}
            {\int_{\mathcal D_y}e^{L(a,y)}\,da}.
 \tag{MS.7}
\]

All current constraints, coarea factors, old fluctuation responses and selectors remain in `L` or `D_y`. Holding an old coordinate `w` in `y` fixed does not mean that its density coefficient is independent of `a`. For example a retained old Gaussian factor `exp[-w K(a,y)w/2]` still contributes its exact current-field ratio to `L`.

The C-01 identification, §3, and Annex AX state this explicitly. Older `T_k` factors which the source actually keeps outside the current integral remain in the outer law. When a coordinate choice makes an old factor depend on the current free field, its logarithmic ratio must be included. Source support, rather than notation, decides which case holds.

Consequently a valid regular-step proof can condition on retained old payloads and bound the current integral uniformly in those payloads, using their actual native energy and carrier data. It need not average those payloads again under an old reset posterior. Their outer averaged contribution to the M-03 norm still has to be bounded under the true outer law, by the stated input and zero-source assumptions; arbitrary conditioning cannot replace that law.

There is an exact qualification. If a particular zero-source filing has already integrated a payload which the proposed input mark still uses, one cannot simply regard that payload as retained. Either:

1. the input `F_k` is already the exact marked conditional value after that integration, with its budget stated as an input hypothesis; or
2. the proof restores the actual old integration, including its mark, cutoffs, normalizer and current responses.

Option 2 is a different marked calculation and can require the reset estimates pursued in the first-birth notes. It is not automatically forced upon option 1.

## 5. A regular E/B/R response is not the same operation as a reset posterior

Annex BK §2 begins by fixing **one geometry and one actual source-free regular integral**. Its zero-source gas is `Xi(v)`, with every inherited activity's complete field and history dependence. Its one-root numerator is

\[
 N_F(v)=\sum_Z R_Z(v)\,\Xi_{\not\sim Z}(v),
 \qquad Q_vF=N_F(v)/\Xi(v).
 \tag{MS.8}
\]

The root is linear in the actual incoming `F`. Its maps are the same specified source maps as in the denominator. The inherited R activities are functions in this density; their presence does not by itself instruct the current regular kernel to resample an old component.

If LFR II (1.103)–(1.104) has already been used, the entire old boundary exponential and normalized fixed-component operations are part of the same zero-source baseline. Annex BK correctly insists that the numerator use that baseline too. This does not require re-inserting an old microscopic mark whose earlier effect is already contained in the input function. It does require proving all actual current variations of the completed baseline which the regular step uses.

By contrast the reset map in M-03 (M.34) is

\[
 (Q_RF)(u',v)
 =\frac{\int\rho(u,v)F(u,v)\,du}
        {\int\rho(u,v)\,du}.
 \tag{MS.9}
\]

Here old internal states `u` are currently integrated. The fresh reference cancels from this old marked quotient, but the old mass, descriptor mixture and retained currents remain. A rare-sector normalizer and birth-position comparison can be essential for (MS.9). Formula (MS.9) is a separate operation from the fixed regular integral (MS.7).

## 6. What the first-birth route is proving

The first-birth notes study a component whose old microscopic scalar is averaged during a later prepared reset. They compare translated initial R histories in the same fresh-reference class and seek a pointwise old-root estimate after that averaging. This helps with:

- a reset operator estimate for a particular microscopic/old-root class;
- the full shifted-regulator/current application downstream of the law-level H-03 theorem;
- H-04's sum over repaired/residual/inherited sectors;
- verification of a future incoming budget for M-07.

It is stronger than what is needed merely to apply a regular-step estimate to an `F_k` whose legitimate input budget is already hypothesized. In particular, the currently unresolved birth-weight comparison and nonlinear microscopic background-root bound should not be treated as mandatory lemmas for every regular M-04 proof.

This conclusion does not promote the existing first-clean result to all regular scales. It only identifies which remaining estimates are actually regular-step estimates.

## 7. The regular M-04 gates which remain

The following obligations cannot be bypassed by this scope distinction.

### 7.1 Exact physical carriers for the complete inherited action

Numerical decay of a native coefficient does not prove that it is a function of raw retained data only in that carrier. Its constrained background, old fluctuations, graph choices, current and all coordinate maps must have the declared actual support after localization. This remains a genuine boundary-action problem.

### 7.2 An actual marked-root bound from the input budget

The pre-normalization root activities in (MS.8), with their separate value/direct/current records, must be estimated from the stated input budget on the complete regular density. One cannot assume Annex BK's final root sum as an additional input and call that the proof.

### 7.3 The full ambient M-03 norm

M-03 includes elementary continuous shifts, discrete history replacements, shifted native regulators, separately measured direct and kernel-current records, and ambient versions. An estimate restricted to one buffered native chart or one fixed descriptor proves only that restricted theorem. Any extension must be specified and shown to agree on the actual regular support. Selector jumps, raw-coordinate chart changes and physical boundary footprints remain concrete issues.

### 7.4 The complete outer law

The averaged portion of M-03 uses the true outgoing law. A conditional fixed-history moment bound does not automatically produce the required bound after all outer data are averaged. The one-step hypothesis may provide the actual input moments; it may not substitute an unrelated conditional law or reset reference for them.

### 7.5 Extraction in the fixed incoming F-01 basis

Scalar and identity coefficients must be extracted from the same exact output, with the conversion from the fixed incoming normalization exposed. Any remaining term must satisfy the same M-03 bound. A finite-pulse projection can be a legitimate algebraic extraction if its basis, symmetries and coefficient conversion are fixed; no running F-05 normalization may be assumed.

## 8. Recommended logical order

Prove a uniform regular operator theorem for a precisely specified incoming analytic/carrier class and the actual regular kernel, including genuine inherited B dependence. Apply scalar/identity extraction to that same output. State the input-budget hypothesis and the actual zero-source assumptions separately. Keep the first-birth and reset work as progress on the later full-history application rather than a prerequisite inserted into the regular theorem.

This ordering preserves the exact `Q_kF_k` required conclusion. It reduces neither the required M-03 norm nor the inherited regular boundary responses, and it makes no claim that the all-scale input induction or full Yang–Mills construction is complete.
