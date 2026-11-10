# Reflection positivity after blocking

**Current status:** No conditional reflection positivity of the reset or mixed law is assumed by the new normalized birth estimates. The reset reflection-factorization problem below remains separate.

**Status:** The deterministic averaging step has the required support geometry on its stated source domain. This does not establish reflection positivity of the actual full \(RT\) evolution. The reset normalizer and its random component/collar geometry prevent a direct half-space pullback argument. This appendix does not modify the frozen H7 module.

### 1. A precise sufficient condition

Let \(\mu\) be reflection positive under a reflection \(\vartheta\), and let \(\mathcal A_+\) be the algebra of observables using only fine links in the positive half. Let a deterministic blocking map \(\mathcal B\) satisfy:

- \(F\circ\mathcal B\in\mathcal A_+\) for every observable \(F\) on coarse links internal to the positive coarse half.
- \(\mathcal B(\vartheta U)=\vartheta\mathcal B(U)\), almost surely.

Then its actual pushforward \(\nu=\mu\circ\mathcal B^{-1}\) is reflection positive on that coarse algebra, because

\[
\int F(V)\overline{F(\vartheta V)}\,d\nu(V)
=\int (F\circ\mathcal B)(U)
\overline{(F\circ\mathcal B)(\vartheta U)}\,d\mu(U)
\ge0.
\tag{RP7.1}
\]

For a stochastic kernel \(K\), a sufficient replacement is half-space conditional factorization and locality:
\[
K(F\,\vartheta\overline F)
=(KF)\,\vartheta\overline{KF},
\qquad KF\in\mathcal A_+ .
\tag{RP7.2}
\]
The first identity follows, for example, from independent reflection-paired output randomizations in the two halves. Positivity of \(K\), normalization \(K1=1\), and reflection covariance alone do not imply it. A reflection-invariant positive kernel that outputs two opposite spins has \(\mathbb E[V_+V_-]=-1\), despite having a trivial reflection-positive input.

### 2. What the actual averaging formulas verify

CMP109, printed pp.252–254, (0.3)–(0.12), defines endpoint blocks and shortest coordinate-order contours. Every contour associated with an averaged bond stays inside the union of its two endpoint blocks. All coordinate permutations are included to obtain lattice Euclidean covariance.

Thus, for a reflection plane on a block boundary, an averaged bond internal to the positive coarse half uses only positive-half fine links. On the domain where the source average is defined and Euclidean covariant, it has exactly the two properties in (RP7.1).

The full uncut \(T\)-operation is deterministic pushforward: CMP119, printed p.243, (0.1), uses \(\delta(\overline U V^{-1})\). Therefore, **if the actual globally defined frozen average is verified to retain those support and reflection properties**, \(T\) preserves reflection positivity on the stated coarse algebra. No separate positivity argument for the delta kernel is needed.

There is a domain qualification. The group-valued means in CMP109 (0.5)–(0.10) are introduced for sets with sufficiently small diameter; the displayed logarithms are analytic on the specified small neighborhoods. Their local covariance does not automatically certify the chosen global measurable continuation on arbitrary large fields. One should verify the actual continuation, rather than replace it with a convenient new average.

[Primary CMP109 paper, pp.252–254](https://doi.org/10.1007/BF01215223).

### 3. The exact reset dependency that blocks the same proof

The actual reset in LFR I, printed p.201, (1.100), contains a normalized local resampling integral for each eligible component \(X_i\). Its denominator is an integral over replacement fields, with a cutoff and a Wilson action evaluated at the minimizing field determined jointly by the replacement field and the retained boundary field. Schematically, with the same source variables and no deletion of boundary dependence,

\[
Z_{X_i}(V_{\Lambda_i})
=\int dW_i\,
\delta_{G_i}(W_i)\chi_i(W_i,V_{\Lambda_i})
\exp\!\left[
-g_k^{-2}A\!\left(
\zeta_i,U_{k,X_i}(W_i,V_{\Lambda_i})
\right)\right].
\tag{RP7.3}
\]

The source makes these denominators local to neighborhoods of \(X_i\); it does not factor them across an arbitrary reflection plane. If \(X_i\) or its retained collar intersects both half-spaces, a positive-half output can depend on the negative-half retained field through the minimizing boundary-value problem and through this same normalizer. Both halves can also share the eligible component and its resampling variables. Consequently neither the locality condition nor (RP7.2) follows for the full reset.

The component selection is itself part of the input dependence: eligibility uses the connected region, its size, and the preceding clean window. Averaging axial graphs to restore Euclidean covariance, as described immediately after (1.100), does not prove a positive reflection factorization of this conditional law.

This identifies a missing theorem, not a proof that the reset law fails reflection positivity. Restricting attention to a fixed component entirely inside one half with its collar does not settle the actual sum, which includes crossing components and other histories.

### 4. Implication for later birth selectors

The original H7-E theorem remains valid because it uses reflection positivity before any reset and bounds the actual initial plaquette event. To repeat its proof for later births, one must additionally establish all of the following on the same actual law:

1. Reflection positivity at the required coarse or buffered reflection planes, including the reset and its complete normalization.
2. The reflection-local support of the actual birth selector. CMP119 (1.4), unlike (1.1), involves a minimizing field on an enlarged determining domain.
3. An energy or constrained-partition cost for the completely disseminated later selector, strong enough compared with the corresponding normalized free-energy cost.

The global upper density stability bound alone does not supply item 3. A kernel that is positive, or even Euclidean covariant, does not supply item 1. The cited source clauses therefore support a conditional \(T\)-preservation lemma and a concrete reset obstruction, but do not close normalized later births.

---
