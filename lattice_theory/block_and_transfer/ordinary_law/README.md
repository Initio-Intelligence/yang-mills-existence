# Contacts, compact source jets and retained susceptibility

Let the physical source be fixed before conditioning. The compact Wilson law determines its conditional mean, its source jets, and the numerator and denominator of the next integration. These derivations give estimates at specified cutoff, support, and background.

- [Bare contacts, averaged susceptibility and native scales](bare_contacts.pdf) derives the force-factor and connected-support bounds at every fixed order, with the local-moment and finite-size hypotheses retained. Sections 4 and 5 distinguish positive transport of the unnormalized coefficient from transport of logarithmic derivatives. Convexity gives a susceptibility bound averaged over a real source interval. A bound at the origin requires additional control.
- [Conditional estimates at source zero, complete current transport, and native target lifts](source_zero_conditional_estimates.pdf) derives the fixed-exterior influence and score identities, the quadratic projection budget, and the source-zero effective response. Theorem 9.1 gives factorial control of bare contacts by a support count and ordered derivatives of a plaquette word. The weighted native wall estimate in §10.1 retains the physical-volume cost, and §10.2 lists the remaining obligations. In its bracketed citations, [2] is the note on bare contacts above and [W] denotes the [Wilson-source estimates](../../source_estimates/README.md), cited by source page.
- [Projected cross terms and compact retained-source jets](compact_source_jets.tex) treats the projected energy and the numerator and denominator of a compact marginal. Its infrared estimates use the complete compact quadratic jet with the actual cross terms. The nonlinear remainder and the retained susceptibility have separate hypotheses.
- [Conditional variance and the retained susceptibility](retained_susceptibility_criteria.tex) gives the source and its three rows, the two terms of total variance, and the resolvent criterion for the ordinary connected estimate. A fixed-depth resampling estimate bounds the removed variance. The dependence of the residual conditional mean on its exterior still enters the full variance.

For a conditional expectation $K$ and a square-integrable source $r_f$, orthogonality gives the law of total variance.

$$
\operatorname{Var}(r_f)
=\mathbb E\!\left[K(r_f^2)-(Kr_f)^2\right]
 +\operatorname{Var}(Kr_f).
$$

A uniform bound for the first term leaves the second term to estimate. Similarly, for a finite positive law with a real exponential source, the second derivative of its logarithmic partition function is a variance. An integral estimate on that derivative controls its average over the real source interval. Obtaining a uniform value at source zero is the pointwise susceptibility problem.
