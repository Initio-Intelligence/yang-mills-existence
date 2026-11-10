# A sharp limitation of logarithmic rarity estimates

**Annex BF.** Exact finite conditional identities apply to the specified positive kernel. A uniform Wilson application requires CL on the same retained sigma-field, the relevant complete-potential estimates under CR and the stated spatial and energy budgets. [History estimates](../history/README.md) · [Observable transport](../observable_transport/README.md).

The normalized coupling and geometric hypotheses are retained throughout. Whenever the Wilson trajectory is identified through Gaussian calibration, GC includes the error bounded uniformly in depth. [Theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Proposition RG19.1

Fix c>0 and r>1. There is a family of finite positive probability laws with a nonnegative bounded mark X_l, indexed by l>=1, for which

\[
 0\le X_l\le e^l,\qquad
 \mathbb P(X_l\ne0)=e^{-c l^r},
 \tag{RG19.1}
\]

but no constants C,p independent of the integer m can satisfy

\[
 \sup_{l\ge1}\mathbb E[X_l^m]\le C^{m+1}(m!)^p
 \quad\hbox{for every }m\ge1.
 \tag{RG19.2}
\]

**Proof.** Take a two-point law with X_l=e^l on the indicated rare event and X_l=0 otherwise. Then

\[
 \mathbb E[X_l^m]=\exp\{ml-cl^r\}.
 \tag{RG19.3}
\]

For sufficiently large m choose l=(m/(cr))^(1/(r-1)), which is at least one. Its exponent is

\[
 (r-1)c\left(\frac m{cr}\right)^{r/(r-1)}.
 \tag{RG19.4}
\]

This grows faster than (m+1)log C+p log(m!) for every fixed C,p, since r/(r-1)>1 and log(m!)<=m log m. Thus (RG19.2) is impossible. ∎

### The averaged M-03 grade is also stronger than fixed-order rarity

For the same family and a fixed positive integer m, consider X_l^m with value grade m. Whenever c l^r/m>=1, take the probability moment order q=c l^r/m in (M.8). Direct substitution gives

\[
 \mathfrak m_m(X_l^m)
 \ge \frac{\exp(ml-m)}{(c l^r)^m}.
 \tag{RG19.5}
\]

It diverges as l tends to infinity. Thus the rare-event bound in (RG19.1) does not yield a uniform averaged M-03 bound even at one fixed source order. The pointwise regulator part requires additional control as well.

### Implication for the proof strategy

A compact insertion can have a crude bound proportional to g^-2, with l=log g^-2. Combining that crude supremum with a source small factor exp[-c(log g^-2)^r] may control each fixed derivative order with order-dependent constants, but it does not prove fixed-factorial control of the full hierarchy. The calculation above gives the precise growth obstruction to that deduction.

An actual exponential reserve in a nonnegative coercive energy E supplies the needed different information. If an unnormalized positive measure M satisfies M(exp(theta E))<=A for fixed theta>0, then

\[
 M(E^m)\le A\,m!\,\theta^{-m},
 \tag{RG19.6}
\]

because (theta E)^m/m!<=exp(theta E). This bound preserves a fixed factorial exponent. Applying it to the source operation requires identifying which actual energy has the reserve and which incoming marks or regulators it controls. A reserve for an outer quadratic/Wilson energy does not automatically cover every older hidden native coordinate.
