# A first Schur tilt preserves the localized scalar root

This note proves an actual first-step conditional estimate, and then an explicit conditional consequence for a compared family of residual histories. The first estimate uses the same complete product-domain Wilson density as RMg and the same literal bounded R-only event as RB. The history-family conclusion requires its stated later reserve and mass comparison; it does not assume that those two-history source obligations have already been proved.

The point is to bound one scalar root together with arbitrarily many powers of the old energy. Applying an unweighted root estimate followed by Hölder would lose an unnecessary extra power of the energy budget. A small positive Schur tilt avoids that loss.

## 1. The original first-step objects

Fix admitted coarse data V on the globally P/Q-regular first branch, with one bounded h=1 R-only neighborhood. Use the original independent free coordinates z. On the encompassing product domain C_D of RB, with radius 3P on a set D of O(R^4) blocks and radius P elsewhere, put

\[
 q_V(dz)=Z_D(V)^{-1}{\bf1}_{C_D}(z)
 \exp[-\tfrac12z^{\mathsf T}K(V)z+W_V(z)]\,dz.
 \tag{TM.1}
\]

K is the actual constrained first precision, including its background-current terms. W contains all the original Wilson, soft-gauge, Haar, coarea and exceptional-constraint Jacobian terms, in the critical-cancelled source normal form. This is precisely the common-domain law verified in RMg. Every coefficient and cutoff is specified as there.

Let E_i(V) be the complete actual first R-pattern event, including the remaining starred Q-good tests. At fixed V it is measurable in z_D. The exact free-bond identity and radial sandwich are RB.3–RB.7. Its probability is positive. No new approximate R event is substituted.

Let D_0 be the first retained fluctuation list in this component, enlarged into D if necessary. Write the actual untruncated Schur quadratic as

\[
 E_0(z)=\tfrac12z_{D_0}^{\mathsf T}S_{D_0}(V)z_{D_0},
 \quad
 S_{D_0}=K_{D_0D_0}-K_{D_0O}K_{OO}^{-1}K_{OD_0}.
 \tag{TM.2}
\]

The outside good-cutoff completion is still inside (TM.1); it is not removed in defining E_0. The source identifies this quadratic at CMP119 (1.29), with the positive Schur sign, as checked in [first schur cancellation source analysis](first_schur_cancellation_source_analysis.md). Undoing the exact source relocalization (1.22) leaves the literal native first energy within o(1) of (TM.2) on the encompassing 3P tube. That harmless comparison can be restored at the end.

The first-step gap, finite stencil and massive inverse imply, uniformly in the choice of D_0,

\[
 cI\le S_{D_0}\le CI,
 \qquad
 \sup_a\sum_b e^{\kappa d(a,b)}\|S_{D_0,ab}\|\le C.
 \tag{TM.3}
\]

Indeed K_{OO} has the same lower gap as K, its inverse has exponential rows by the massive resolvent expansion, and the two interface factors K_{D_0O}, K_{OD_0} have finite range. This argument applies to the **one component's full retained Schur list**, not a sum of unrelated diagonal energies with omitted cross terms.

## 2. A bounded tilt is another admitted complete first-step law

For 0≤t≤t_0, with a fixed sufficiently small t_0, define

\[
 q_{V,t}(dz)={e^{tE_0(z)}q_V(dz)\over q_V(e^{tE_0})}.
 \tag{TM.4}
\]

Its precision is

\[
 K_t=K-t\,\iota_{D_0}S_{D_0}\iota_{D_0}^{\mathsf T}.
 \tag{TM.5}
\]

By (TM.3), K_t has a fixed positive gap and fixed exponentially weighted row bounds throughout this interval. W and the product domain are unchanged. In particular all the complete derivative estimates of RMg remain valid with constants independent of t, D, and total lattice volume:

\[
 \sup_a\|\partial_aW\|\le C(gP^2+g^2P),\qquad
 \sup_a\sum_b e^{\kappa d(a,b)}\|\partial_a\partial_bW\|
 \le C(gP+g^2).
 \tag{TM.6}
\]

The tilted Gaussian with precision K_t and the same convex symmetric product cutoff is centered. Its fixed-dimensional coordinate marginals have bounded quadratic moments by the Gaussian convex-mask estimate CR.12. Applying RMg's relative marginal comparison to a fixed coordinate neighborhood therefore gives

\[
 \sup_{0\le t\le t_0}\sup_a q_{V,t}(\|z_a\|^2)\le C.
 \tag{TM.7}
\]

This uses only a fixed local marginal, so the exponent is O(gP^3+g^2P^2), not that quantity times the total volume. Summing the absolute rows of S_{D_0} and using (TM.7) yields

\[
 q_{V,t}(E_0)\le C|D_0|,
 \qquad
 \log q_V(e^{tE_0})\le Ct|D_0|.
 \tag{TM.8}
\]

The argument includes the full conditional boundary score of RMg.12; replacing it by only the direct derivative would not prove the spatial estimates below.

## 3. Conditioning on the rare first event costs only P² in the logarithm

The normalized probability of E_i(V) under (TM.1) satisfies

\[
 q_V(E_i(V))\ge \exp[-C(P^2+|D|)].
 \tag{TM.9}
\]

Here is the normalization check. RB.15 and RB.18 compare the event's unnormalized integral with the **original common all-P integral** Z_P(V), giving a ratio at least exp(-CP²). The factor Z_P(V)/Z_D(V) is the probability that the D-coordinates also lie below P under (TM.1). For the centered Gaussian with precision K(V) and support C_D, the convex-mask tail estimate gives this probability at least 1-C|D|exp(-cP²). RMg's relative comparison on D multiplies that lower bound by exp[-C(gP³+g²P²)|D|]. It is at least 1/2 at sufficiently weak coupling. The weaker bound (TM.9) is convenient and also covers fixed finite geometric enlargements.

Let

\[
 K_*=1+P^2+|D|.
 \tag{TM.10}
\]

At t=t_0, (TM.8) and (TM.9) give

\[
 \log q_V(e^{t_0E_0}\mid E_i)\le CK_*.
\]

The logarithm of this conditional moment generating function is convex and vanishes at zero. Consequently

\[
 \log q_V(e^{tE_0}\mid E_i)\le CtK_*\quad(0\le t\le t_0),
 \qquad
 q_V(e^{tE_0}\mid E_i)\le C\quad(0\le t\le c/K_*).
 \tag{TM.11}
\]

The rare-event probability occurs only inside a logarithm and is multiplied by the small tilt. It is never used to divide an absolute approximation error. Under the source hierarchy P² dominates |D|=O(R^4), so K_* is comparable to P².

## 4. Keep the scalar root local under this same tilt

Let F_x be the actual microscopic scalar at a fixed fine root x, with its original coefficient and identity term:

\[
 F_x=c_x+\alpha a^{-4}\mathcal E_x(V,z).
 \tag{TM.12}
\]

Here \mathcal E_x is the exact local Wilson-energy stencil, not merely its quadratic Taylor term. Its free-coordinate stencil X_x has fixed size, including the exceptional reconstruction footprint. Put b≥|α| and assume the already incoming identity coefficient satisfies |c_x|≤ba^{-4}; if it does not, retain |c_x| separately in every bound below. Define the nonnegative majorant

\[
 A_x=|c_x|+|\alpha|a^{-4}\mathcal E_x.
\]

Let e_{\mathrm{bg},x}(V) be the nonnegative local Wilson-energy stencil of the actual first background, with a fixed stencil enlargement. The exact first reconstruction and Taylor's formula on its admitted geometric tube give

\[
 A_x\le Cba^{-4}\Bigl[1+e_{\mathrm{bg},x}(V)
                  +\sum_{a\in X_x}\|z_a\|^2\Bigr],
 \qquad
 \|\nabla A_x\|\le Cba^{-4}P
\]

on C_D; the latter uses the source bound e_bg≤CP². These are the same complete first-step scalar estimates used in LC and RMg. The identity c_x is unchanged.

From (TM.7),

\[
 q_{V,t}(A_x)\le Cba^{-4}[1+e_{\mathrm{bg},x}(V)].
 \tag{TM.13}
\]

The weighted covariance proof of RMg.21 is uniform for K_t. For the conditional mean at fixed z_D=u, it gives

\[
 \|\partial_{u_a}q_{V,t}(A_x\mid z_D=u)\|
   \le Cba^{-4}P e^{-\kappa' d(X_x,a)}.
 \tag{TM.14}
\]

The direct derivative is retained when a meets X_x, and the boundary-score covariance is retained otherwise. Since the diameter of each D-coordinate ball is O(P), any measurable event in z_D, including the exact E_i(V), obeys

\[
 q_{V,t}(A_x\mid E_i)
 \le Cba^{-4}[1+e_{\mathrm{bg},x}(V)+P^2w_x(D)],
 \quad
 w_x(D)=\sum_{a\in D}e^{-\kappa'd(X_x,a)}.
 \tag{TM.15}
\]

Use the exact change of conditional measure induced by (TM.4):

\[
 q_V(A_xe^{tE_0}\mid E_i)
  =q_V(e^{tE_0}\mid E_i)\,q_{V,t}(A_x\mid E_i).
\]

Equations (TM.11) and (TM.15) prove the actual first-step result.

### Theorem TM.1: one marked root with all first-energy moments

Uniformly on the admitted first-step R-only branch,

\[
 \boxed{\quad
 q_V(|F_x|e^{tE_0}\mid E_i(V))
 \le Cba^{-4}[1+e_{\mathrm{bg},x}(V)+P^2w_x(D)],
 \qquad 0\le t\le c/K_*.
 \quad}
 \tag{TM.16}
\]

In particular, for every integer n≥0,

\[
 q_V(|F_x|E_0^n\mid E_i(V))
 \le C^{n+1}n!K_*^n ba^{-4}
       [1+e_{\mathrm{bg},x}(V)+P^2w_x(D)].
 \tag{TM.17}
\]

The last step is the pointwise inequality E_0^n≤n!t^{-n}e^{tE_0}. No Cauchy estimate for a signed exponential integral is needed. Restoring the native source E_0 after (1.22) changes constants by a bounded factor and replaces K_* by K_*+1. The theorem is stronger than an (n+1)! bound in the energy index, but concerns only one scalar root and the stated first component.

## 5. What mass dilution and the later reserve now give

Here is a precise conditional consequence for a family of J compared histories. Assume the original exact branch integral has the disintegration

\[
 M_i(dy,dz)=M_i(dy)\,q_{V(y)}(dz\mid E_i(V(y))),
 \tag{TM.18}
\]

after undoing the exact first relocalization. The first all-P normalization is retained in M_i(dy), exactly as in RB and LE. Let E_{\mathrm{late},i}(y) be independent of z, and suppose the already proved or separately verified branch reserve gives

\[
 {M_i(e^{tE_{\mathrm{late},i}})\over M_i(1)}\le C,
 \qquad 0\le t\le c/K,
 \quad K\ge K_*.
 \tag{TM.19}
\]

For the source first-reset branch, LE's upper and lower give log M_i(e^{θE_late})/M_i(1)≤CD_late at fixed θ, hence (TM.19) by convexity whenever K≥D_late. The source hierarchy allows K=CP². This inference uses the finite later list in LE; it does not add an extensive collection of arbitrary restored modes.

Assume the family has the **unweighted** mass comparison

\[
 {M_i(1)\over Z_r}\le C/J,
 \tag{TM.20}
\]

where Z_r is the complete same-class normalizer, and the translated footprints have bounded overlap:

\[
 \sum_{i=1}^Jw_x(D_i)\le C_{\rm ov}.
 \tag{TM.21}
\]

Then (TM.16) can be integrated before summing i. The flat-background case here means that the **first actual minimizing background U_1(V_1(y)) is flat for almost every y in the later measure**, so e_bg,x(V_1(y))=0 there. A flat final retained field V_k does not imply this: the intervening V_1 is still integrated and can fluctuate. Under that explicitly stronger first-background premise this proves

\[
 \boxed{\quad
 {1\over Z_r}\sum_{i=1}^J
 M_i\bigl(|F_x|e^{t(E_{0,i}+E_{\mathrm{late},i})}\bigr)
 \le Cba^{-4}[1+C_{\rm ov}P^2/J],
 \qquad 0\le t\le c/K.
 \quad}
 \tag{TM.22}
\]

There is no need to prove a new CE comparison under the tilted later law: the uniform branch estimate (TM.19), the pointwise first estimate (TM.16), and the original unweighted bound (TM.20) suffice. Extra positive histories can stay in Z_r; they only improve (TM.20). Their own marked numerators are not bounded by (TM.22).

For a nonflat background retain, exactly, the additional term

\[
 {Cba^{-4}\over Z_r}\sum_i
 M_i\bigl(e_{\mathrm{bg},x}(V(y))e^{tE_{\mathrm{late},i}}\bigr).
 \tag{TM.23}
\]

A uniform appropriate bound for this term closes the corresponding nonflat estimate. This term remains present even at a flat final retained V_k when the intermediate V_1 is integrated. It cannot be dropped merely because a local gauge makes the first precision close to the flat precision: the actual scalar has its own background value. This is a marked transport obligation, not a cutoff normalization error.

Finally, differentiating the positive exponential majorant in the elementary inequality sense used for (TM.17) gives

\[
 {1\over Z_r}\sum_iM_i\bigl(|F_x|(E_{0,i}+E_{\mathrm{late},i})^n\bigr)
 \le C^{n+1}n!K^n ba^{-4}[1+C_{\rm ov}P^2/J]
 \tag{TM.24}
\]

under the flat-background or separately controlled-background premise. The root has no extra K factor. The legitimate one-step incoming budget may be B_in=(h/a)^4b, for which h^{-4}B_in=ba^{-4}. Since J grows exponentially in the waiting depth while P is a fixed logarithmic power, P²/J≤C is sufficient at this one step. This does not assert a depth-uniform M07 budget or a result for arbitrary energy-bounded sums of old marks.

## 6. Exact limits of the new result

Theorem TM.1 is an actual complete first-step theorem on the stated original product support and bounded R-only event. The family result additionally needs (TM.18), the later reserve, and the mass comparison. The currently unresolved two-history completion/refinement comparison is not assumed proved here. First-layer background energy is retained explicitly in (TM.23). Continuous or discrete current estimates and arbitrary earlier histories require their own differentiated conditional statements; they do not follow from the positive one-root moment estimate alone.
