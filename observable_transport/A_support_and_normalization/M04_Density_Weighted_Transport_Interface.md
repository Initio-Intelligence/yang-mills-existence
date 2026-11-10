# Density-weighted transport: exact jets, rare components, and the connected-output gate

## Outcome and scope

There is an exact alternative to taking a supremum of a normalized
conditional mark on every rare history: transport its **complete
unnormalized source-coefficient measure**, including the actual history
weight. Its positive forward transport is linear and contracts total
variation. The full source jet survives history averaging exactly.
An exponential energy-and-rank reserve pays all polynomial insertion
orders with one rare-event factor per distinct component.

This is a substantive change of interface. It does not give a bounded
conversion into the stated M03 norm, does not undo GO, and does not
claim a proof of M04. The pointwise conditional expression
can still have the obstructions already proved in GO and BC.

The useful actual source input is already available for successful
replacement components: NM20.7--NM20.13 in [Annex BM](../../history/Annex_BM.md).
It pays their complete physical
footprints in the true mixed posterior, with all old internal
histories and the same full normalizer retained. It does not control
fixed residual components or establish raw retained-field locality.

The new interface becomes sufficient for the existing Schwinger
hierarchy route if the actual source densities admit the connected
local expansion specified in Sections 7--9, with the stated uniform
matching and scale-summability bounds. Those are explicit analytic
obligations, not conclusions of probability alone. A finite hard-core
polymer criterion proving the required connected algebra is given
below. Its factorization must be verified for the actual complete
density before applying it.

### What is proved here

1. Exact coefficient-measure transport, including every full-jet
   coefficient and every normalized reset.
2. Total-variation contraction and the absence of a rare conditional
   denominator in that transport.
3. A single-store all-order energy/rarity theorem; its application to
   the actual successful-component posterior pays full footprints.
4. Exact normalizer and outer-log algebra, including outer conditional
   means and all higher cumulants.
5. A linked-cluster theorem with a fixed factorial exponent, under a
   precise density-factorization and activity criterion.
6. Conversion of a weighted connected-density bound into the physical
   kernel bound used by S05/S02; a quantitative shrinking-contact
   Taylor estimate; and a uniform-depth transport criterion.
7. Exact preservation of physical source currents under specified
   forward kernels, together with the precise limitations of that
   statement for retained-coordinate/interface currents.

No claim is made that the outstanding source hypotheses in item 5
or the uniform-depth hypotheses in item 6 have been proved for every
admitted Yang--Mills history.

## 1. Source identities that must remain intact

The relevant specified definitions are:

- Annex W, (4.1)--(4.2): positive unnormalized branch measures
  \(r_{k,\gamma}\), their sum \(\rho_k\), and the common Wilson
  partition function \(\mathscr Z\).
- Annex W, (4.3)--(4.5): the old--fresh replacement coupling. The fresh
  reference denominator, the old conditional denominator, and the
  history-posterior denominator are different quantities.
- Annex W, (4.6)--(4.9): a reset averages the complete finite source
  jet. It does not average one-field marks and then multiply them.
- Annex Y, M.42: conditional logarithms generate every partition
  cumulant; M06/M07 additionally demand a fixed all-order and
  all-depth budget.
- H03, HS20.4: the actual mixed reset posterior includes successful
  geometry and old states, together with the old internal states of
  fixed residual components.
- Annex BM, NM20.7--NM20.13: the successful-component exponential
  energy/rank reserve and its full-jet consequences.

History-dependent vacuum factors, full E/B/R densities, every
coarea/Jacobian factor, real selectors, and genuine fresh kernels stay
inside these measures. None is replaced by a probability assigned to
a signed polymer activity.

## 2. Full source jets as signed coefficient measures

At a fixed finite cutoff let \(R_j\) be the actual unnormalized
source-free state measure at step \(j\). Its mass is \(\mathscr Z\).
Let \(T_j(x,dy)\) be the actual source-free positive forward kernel,
including deterministic maps, exposed selectors and any fresh draws.
Thus
\[
 R_{j+1}=R_jT_j.
 \tag{DW.1}
\]

One may work on the full latent path space when a smaller retained
state has not been proved sufficient for the future kernels. This
avoids changing the process by an unjustified history erasure.

Use finitely many labeled nilpotent source variables \(t_i\), so
\(t_i^2=0\). This is a convenient exact encoding of the mixed finite
jet, not an assumption of convergence of an infinite source series.
Write
\[
 G_j(t,x)=\sum_{I}t_I G_{I,j}(x),\qquad G_{\varnothing,j}=1,
 \qquad
 U_{I,j}(dx)=G_{I,j}(x)R_j(dx).
 \tag{DW.2}
\]
For the original exponential of one-field marks,
\(G_{I,0}=\prod_{i\in I}F_i\). If the incoming logarithm already has
higher vertices, \(G_{I,j}\) is its full partition coefficient. Those
vertices are not discarded.

### Theorem DW.1 — exact linear transport of every coefficient

For the backward conditional \(Q_j\) of the actual joint law
\(R_j(dx)T_j(x,dy)\),
\[
 U_{I,j+1}=U_{I,j}T_j,\qquad
 \frac{dU_{I,j+1}}{dR_{j+1}}=Q_jG_{I,j}
 \quad R_{j+1}\text{-almost everywhere}.
 \tag{DW.3}
\]
For a branch decomposition \(T_j=\sum_\gamma T_{j,\gamma}\) into
nonnegative subkernels,
\[
 U_{I,j+1,\gamma}=U_{I,j}T_{j,\gamma},\qquad
 \sum_\gamma U_{I,j+1,\gamma}=U_{I,j+1},
 \tag{DW.4}
\]
and
\[
 \|U_{I,j}T_j\|_{\rm TV}\le\|U_{I,j}\|_{\rm TV},
 \qquad
 \sum_\gamma\|U_{I,j}T_{j,\gamma}\|_{\rm TV}
 \le\|U_{I,j}\|_{\rm TV}.
 \tag{DW.5}
\]
The same statements hold after any finite number of operations.

**Proof.** Pair both sides of (DW.3) with a bounded measurable test.
The defining disintegration identity proves the equality and the
Radon--Nikodym formula. For a signed or complex measure \(U\),
\(|UT_{j,\gamma}|\le |U|T_{j,\gamma}\). Integrating and summing the
branches gives (DW.5), since their total kernel has mass one.
These arguments apply to every coefficient independently and commute
with reducing the source truncation order. Iteration proves the final
claim. No density against Haar measure is required. ∎

In particular, if a branch has output mass \(r_\gamma(dy)\) and
conditional full coefficient \(Q_\gamma G_I(y)\), the actual object is
\[
 U_{I,\gamma}(dy)=Q_\gamma G_I(y)\,r_\gamma(dy).
 \tag{DW.6}
\]
Its defining numerator contains no inverse rare mass. An arbitrarily
large conditional mean on a rare branch need not have a large
coefficient-measure norm.

The contraction alone does not improve the engineering scale. A
bound on \(a^{4m}\|U_{I,0}\|/\mathscr Z\) becomes a bound with the
factor \((h_j/a)^{4m}\) when measured at \(h_j\). The actual relevant
mixing, identity extraction and irrelevant gains still have to
produce the current-scale budget.

### Products use the density once

For two disjoint source label sets \(A,B\), the full coefficient at
their union is generally not the product of their transported
one-set coefficients. Even on one branch,
\[
 (r_\gamma G_A)(r_\gamma G_B)
       =r_\gamma^2G_AG_B
\]
is not its coefficient measure. This display refers to densities
against one common reference, when those densities exist. The
correct primitive product is formed before integration and carries
\(r_\gamma\) once. Equivalently, transport the already formed
coefficient \(G_{A\cup B}\).

This is essential both for conditional covariance and for rare-event
bookkeeping. Dividing a product of weighted coefficients by
\(r_\gamma\) to repair this mistake would reintroduce precisely the
rare denominator the interface is designed to avoid.

## 3. A density-weighted carrier ledger, with an honest support gate

Suppose a coefficient measure has an exact tagged decomposition
\[
 U_{I,j}=\sum_\alpha U_{I,j,\alpha},\qquad
 \mathcal D_{j,m}
 =\frac{h_j^{4m}}{\mathscr Z}
   \sum_\alpha e^{\kappa(|X_\alpha|+\mathsf t(X_\alpha))}
                 \|U_{I,j,\alpha}\|_{\rm TV}.
 \tag{DW.7}
\]
The weight is the same full physical volume/tree weight as before.
There is no \(\sup_p\), no pointwise supremum of a normalized
conditional, and no conditional branch probability raised to \(1/p\).

A tag must come with a **density-construction certificate**. It names
the actual primitive insertion factors, component owners, interaction
vertices and connecting response factors from which its measure was
constructed. Its carrier contains their physical scopes and the
insertion anchors. Common background density is kept as the
reference measure, not asserted to be a local function.

This is different from assigning a small carrier to the globally
dependent function
\(\pi_v(\mathbf1_{\{X\in C\}}F_X)\). NM20 bounds that function's
absolute mass; it does not prove that it is a cylinder function on
\(X\). Likewise (DW.5) does not by itself tell us which output carriers
can be assigned after a pushforward.

For (DW.7) to imply a statement about **connected correlations**, the
certificate must also specify the connected density expansion. Its
components must factor in the exact linked-cluster sense, or its
reference cumulants must already carry the required connecting
responses. Sections 7--9 state and prove sufficient versions of that
additional requirement. Merely renaming a scalar probability bound a
carrier norm is not such a certificate.

### Why a weighted Orlicz norm is not the replacement

For an event \(E\) of small probability, the quantity
\[
 \sup_{p\ge1}(mp)^{-m}\|\mathbf1_E B^m\|_p
\]
need not retain an exponential factor in \(\mathbb P(E)\): the
probability is taken to the power \(1/p\). The viable estimate below
keeps one event indicator inside an actual integral and uses a
single exponential energy reserve before extracting all source
coefficients.

## 4. One exponential store pays all source orders

Let \(\mu\) be an actual normalized joint law. A finite family
\(\mathcal D\) consists of **distinct** component owners. Let
\(E_{\mathcal D}\) be their simultaneous occurrence and let \(B_X\ge0\)
be their positive native energy/rank envelopes. Suppose
\[
 \int \mathbf1_{E_{\mathcal D}}
       \exp\!\left(t\sum_{X\in\mathcal D}B_X\right)d\mu
 \le e^{-S(\mathcal D)},\qquad t>0.
 \tag{DW.8}
\]

### Theorem DW.2 — joint density insertions without a second rarity charge

For nonnegative integers \(m_X\),
\[
 \int\mathbf1_{E_{\mathcal D}}\prod_X B_X^{m_X}\,d\mu
 \le e^{-S(\mathcal D)}
           \prod_X t^{-m_X}m_X!,
 \tag{DW.9}
\]
and, for \(m=\sum_Xm_X\),
\[
 \int\mathbf1_{E_{\mathcal D}}
       \left(\sum_X B_X\right)^m d\mu
 \le e^{-S(\mathcal D)}t^{-m}m!.
 \tag{DW.10}
\]
For a real degree \(q\ge1\), the last factor can be replaced by
\((q/(et))^q\). Thus degree \(m+1/2\) costs at most \(C_t^{m+1}m!\).

**Proof.** Use \(u^n\le n!t^{-n}e^{tu}\) in each distinct owner, or
once in their total energy. For a real degree maximize
\(u^q e^{-tu}\). For \(q=m+1/2\), comparison with Stirling's bound
absorbs the fixed half degree in \(C_t^{m+1}m!\). ∎

If a product has several marks on the same component, that component
appears only once in \(\mathcal D\); add its polynomial degrees.
If two expansions meet the same owner, merge their owner records
before applying (DW.8). There is no assertion that two uses of the
same rare event produce the square of its probability.

Suppose a full incoming coefficient obeys on this event
\[
 |G_I|\le A^m(m!)^s h^{-4m}
                   \left(\sum_XB_X\right)^m .
 \tag{DW.11}
\]
Then its weighted coefficient measure has mass at most
\[
 e^{-S(\mathcal D)}(A/t)^m(m!)^{s+1}h^{-4m}.
 \tag{DW.12}
\]
If instead logarithmic vertices obey the corresponding bound with
degree \(d\), coefficient growth \((d!)^s\), and \(s\ge1\), form the
full jet first. The elementary labeled-partition inequality
\[
 \sum_{\pi\in\Pi_m}\prod_{B\in\pi}(|B|!)^s
       \le C^m(m!)^s,\qquad s\ge1,
 \tag{DW.13}
\]
and (DW.10) give the same conclusion with \(A\) changed by a fixed
factor. This proves the full-jet bound, including all higher partners,
using one event indicator and one common exponential store.

**Partition proof.** For \(s=1\), ordering blocks of sizes
\(d_1+\cdots+d_r=m\) gives
\[
 \sum_{\substack{\pi\in\Pi_m\\|\pi|=r}}\prod_{B\in\pi}|B|!
   =\frac{m!}{r!}\binom{m-1}{r-1}.
 \tag{DW.14}
\]
Sum over \(r\). For \(s>1\), use
\(\prod_B(|B|!)^{s-1}\le(m!)^{s-1}\). ∎

An external partner depending on retained data \(v\) can be included
if the reserve is uniform in \(v\) and that partner has a stated
outer moment bound. An arbitrary old-state-dependent partner cannot
be inserted for free. A universal inequality
\(\mathbb E[W\mathbf1_E]\le q\mathbb EW\) for every old measurable
\(W\ge0\) is equivalent to
\(\mathbb P(E\mid\mathcal F_{\rm old})\le q\); for an old-determined
event it fails unless \(q\ge1\). This is precisely the inherited-event
qualification in Section 5 of the main paper, (5.1)--(5.2).

### Do not add one factorial at every depth

(DW.12) converts a polynomial pointwise energy description into an
integrated coefficient estimate. Applying that conversion anew at
each scale, with an extra \(m!\) each time, would give a factorial
exponent growing with depth.

The safe architecture is to create and estimate a genuine density
atom with its exponential reserve, then transport its **full
coefficient measures** by (DW.3). Their linear transport does not
repeat the partition/energy conversion. Any actual carrier transport
estimate used in an induction must preserve the chosen fixed
factorial class. A precise sufficient condition is stated in
Section 10.

## 5. Actual successful-component application

Use exactly the posterior NM20.1. For successful components let
\[
 B_X=\mathcal F_X^\natural+D_X,
 \qquad
 S(\mathcal D)=\tfrac12\mathfrak P_k|\mathcal D|,
 \qquad \mathfrak P_k=P_0(g_k).
 \tag{DW.15}
\]
Here \(D_X\) is the actual surviving Gaussian rank and
\(\mathcal F_X^\natural\) is the common positive native envelope.
It is not an assumed microscopic Wilson energy.

NM20.7 proves (DW.8) with these quantities, uniformly in the admitted
remaining datum \(v\), total volume and old depth. Its source proof
deletes the pinned successful components before dividing by the
**same full partition function**. The remaining positive sum is a
sub-sum of that partition function. Fixed residual bases and their
normalizers remain unchanged. No inverse successful mass appears.

For an eligible component the full footprint and number of shapes
through one current block cost at most \(\exp(C_\kappa R_k^4)\).
The source hierarchy gives \(\mathfrak P_k\gg R_k^4\). Therefore
NM20.10, or directly (DW.9) with that count, gives
\[
 \sup_b\sum_{X\ni b}
 e^{\kappa(|X^+|+\mathsf t(X^+))}
 \mathbb E_{\pi_v}\!\left[\mathbf1_{\{X\in C\}}B_X^m\right]
 \le C^{m+1}m!\,e^{-\mathfrak P_k/4}.
 \tag{DW.16}
\]

The available factor \(e^{-\mathfrak P_k/2}\) has been split once:
part pays geometry and enumeration, and the displayed part remains.
Internal histories were already summed in the actual \(M_X\).
They are not counted a second time as independent shapes.

This proves an actual full-physical-footprint bound for these
**integrated density atoms**, including arbitrary finite source
order dominated by their native envelope. It does not identify a
local cylinder function of \(v\), supply a marked old numerator not
known to obey (DW.11), or pay an arbitrary fixed residual component.
The added connecting responses are precisely part of Section 7's
source-density certificate.

### First regular R births: a second actual input

The companion proof M04_Averaged_First_Step_Scalar.md, AS.12--AS.24,
establishes for the first globally \(\Omega_1\)-full P/Q-regular
step, uniformly in its admitted native coarse field,
\[
 Z_{\rm all\text{-}P}^{-1}
 \int_{\text{actual R pattern}}e^{tE_D}\,dR
 \le \exp[-c n_{\rm bad}P_{\rm free}^2+C|D|],
 \qquad P_{\rm free}=\delta_0/g_0 .
 \tag{DW.17}
\]
Here \(D\) is the union of the actual bad-test footprints and \(E_D\)
is free-coordinate/gauge energy. The source geometric count
\(|D|\le Cn_{\rm bad}R_1^4\), together with
\(P_{\rm free}^2\gg R_1^4\), pays the full first-hole footprint.

Its proof keeps the complete primitive density. Enlarge only the
coordinates in \(D\) from radius \(P_{\rm free}\) to
\(3P_{\rm free}\). Uniform convexity and the verified small complete
gradient give a fixed exponential quadratic reserve on every
intermediate symmetric product. Shrinking coordinates one at a time
shows that the exact partition-function ratio is at most
\(\exp[C|D|e^{-cP_{\rm free}^2}]\), without a small-volume
restriction. Bounded overlap of the bad-test footprints implies
\(E_D\ge c n_{\rm bad}P_{\rm free}^2\). A fixed Chernoff tilt proves
(DW.17). The same reserve pays every finite product of the actual
first-step scalar marks by AS.19--AS.21.

The true all-P baseline, restored with its original coarse factor
and Wilson normalization, is a submeasure of the actual law. It is
not normalized again. Integrating these relative numerators against
that submeasure gives actual joint-mass estimates. Connected
**complete** bad patterns have the stated full-footprint animal
bound. Summing arbitrary additional disconnected patterns still
requires the density factorization/cluster step in Section 7.

No Wilson-only energy
implication is substituted: pure-gauge R seeds are included through
their free-coordinate/soft-gauge reserve. Native boundary and outer
P/Q-current obligations remain as stated in §9 of
[M04_Averaged_First_Step_Scalar.md](../B_finite_depth/M04_Averaged_First_Step_Scalar.md).

## 6. Exact normalizers, erasure, and physical source currents

### 6.1 One final source partition function

At every stage,
\[
 \mathcal Z(t)=\sum_\gamma\int G_{j,\gamma}(t,y)\,
                                  r_{j,\gamma}(dy),
 \qquad \mathcal Z(0)=\mathscr Z .
 \tag{DW.18}
\]
The exact normalized full-moment jet is
\(\mathcal M(t)=\mathcal Z(t)/\mathscr Z\). Its connected jet is
\[
 \mathcal W(t)=\log\mathcal Z(t)-\log\mathscr Z
             =\log\mathcal M(t).
 \tag{DW.19}
\]
These are finite formal identities, so no zero-free complex-source
neighborhood is needed merely to define any fixed finite order.

On erasing an auxiliary history, sum the coefficient measures in
(DW.18) before normalization or logarithmic extraction. If the
source construction resamples a fresh history, its normalized kernel
is included in \(T_j\), and (DW.3) applies unchanged. A fresh history
does not license replacing the old averaged mark by the mark of the
fresh descriptor.

The old conditional denominator cancels inside (DW.6). The true
fresh-reference denominator remains in \(T_j\). The global
\(\mathscr Z\) is removed only in (DW.19). A history-dependent vacuum
factor remains in \(r_{j,\gamma}\) throughout.

### The actual HS20 posterior denominator cancels in its physical coefficient measure

This cancellation can be stated directly for the published reset,
not only for an abstract Markov kernel. Use the full fixed residual
bases \(\mathcal B_i(v,d\eta_i)\) of HS20.3, with
\(b_i(v)=\mathcal B_i(v,1)\) and \(\nu_i=\mathcal B_i/b_i\).
Let \(\omega(dv)\) denote the genuinely common outer measure in
the positive source integral. No Haar density is assumed for it.
The physical output marginal, with the averaged reset coordinates
erased, is
\[
 R_{\rm out}(dv)=\omega(dv)\Bigl(\prod_i b_i(v)\Bigr)\mathcal Z_v,
 \tag{DW.18a}
\]
where \(\mathcal Z_v\) is the HS20.4 posterior denominator.
Therefore, for its complete incoming full-jet coefficient \(G_I\),
\[
 \begin{split}
 (\pi_vG_I)R_{\rm out}(dv)
 ={}&\omega(dv)
 \sum_{C\ {\rm admissible}(v)}
 \int G_I(v,C,\eta_Y,\eta_C)e^{H_C}\\
 &\hspace{12mm}\cdot
       \prod_i\mathcal B_i(v,d\eta_i)
       \prod_{X\in C}M_X(v,d\eta_X).
 \end{split}
 \tag{DW.18b}
\]

**Proof.** Substitute HS20.4 into the left side, cancel the one
\(\mathcal Z_v\), and use \(b_i\nu_i=\mathcal B_i\) for each fixed
residual base. This is positive disintegration before expansion,
so it is also valid for signed coefficient integrals whenever their
absolute moments are finite. Apply it to every finite source
coefficient. ∎

Thus neither a residual-base inverse \(b_i^{-1}\) nor the mixed
posterior inverse \(\mathcal Z_v^{-1}\) occurs in this complete
physical coefficient density. Every actual old or fresh
descriptor-dependent factor already present in the full
\(\mathcal B_i\) remains there. In particular no genuine fresh
reference denominator has been canceled against an unrelated old
mass.

If an auxiliary new descriptor is resampled from \(\pi_v\) and
retained in the augmented state, its normalized sampling factor
still belongs to the forward kernel. Formula (DW.18b) applies after
that auxiliary variable is integrated out. It does not authorize
discarding it in a future transition which uses it. The full
coefficient-measure identity (DW.3), or a separately proved
sufficiency identity, handles that case.

Differentiating (DW.18b), when justified in a common chart, acts on
the full primitive densities, cross action and admissibility
indicators. There is no normalized-posterior score to estimate
separately. This is a useful exact rearrangement of the source
response problem, not a proof that those remaining density
derivatives or their carriers are small.

### 6.2 The outer term is retained, not estimated away

Writing \(G_j=e^{\Psi_j}\), (DW.19) is
\[
 \mathcal W(t)=\log\mathbb E_{\mu_j}e^{\Psi_j(t)}.
 \tag{DW.20}
\]
At order two this is the exact total-covariance identity
\[
 \operatorname{Cov}(F_1,F_2)
 =\mathbb E[\operatorname{Cov}(F_1,F_2\mid Y_j)]
  +\operatorname{Cov}(QF_1,QF_2).
 \tag{DW.21}
\]
At general order the coefficient is the sum, over partitions, of
outer cumulants of the corresponding inner log coefficients. This
follows by expanding the finite formal logarithm of the exponential
in (DW.20). Thus the interface retains all of H05. It does not infer
an H05 estimate from an H03 within-posterior estimate.

### 6.3 Physical source derivatives commute with the specified kernel

Let an external physical parameter \(s\) enter the original marked
coefficient measure \(U_I(s)\), while the source-free kernel \(T_j\)
is kept fixed as required by the route. If the coefficient derivative
exists as a finite signed measure in total variation, then
\[
 \partial_s(U_I(s)T_j)=(\partial_sU_I(s))T_j,\qquad
 \|(\partial_sU_I)T_j\|_{\rm TV}
       \le\|\partial_sU_I\|_{\rm TV}.
 \tag{DW.22}
\]
This follows by applying the contraction to the difference quotient.
For finite physical source jets it is already the coefficientwise
identity (DW.3). Compact-link Ward/variation insertions can be kept
as their actual microscopic density derivatives before transport.
Every coefficient remains present; no physical source response is
discarded by avoiding a conditional logarithm.

This is not a bound on an arbitrary retained-coordinate derivative
of \(QF\). In a common retained chart, with \(N=r\,QF\),
\[
 \delta_\tau N=r_{\tau}\,\delta_\tau(QF)
                         +(\delta_\tau r)\,QF .
 \tag{DW.23}
\]
Density estimates may use cancellation in this exact combination.
They need not bound either term separately. The original M03 norm explicitly
retains separate pointwise direct and normalized-kernel currents,
so (DW.23) is not a norm conversion into M03.

Likewise, a small event probability alone does not bound the surface
measure produced by differentiating a hard selector. Fixed free-field
R domains may remove that particular moving boundary, but outer
P/Q tests, changed charts and coarea constraints require their exact
density response. If weak derivatives are used, their pairing class
and later pullbacks must be specified; a distributional derivative
cannot simply be paired with another discontinuous selector.

### 6.4 An exact first-step regrouping

Before the first R partition, let the actual positive fluctuation
integrand at fixed coarse datum be \(dR(a;V)\). The literal selector
partition has \(\sum_\gamma\chi_\gamma(a;V)=1\). Each branch may
subsequently use its own source coordinate change, Jacobian and
partial integration. Undoing those exact changes and erasing all
R-dependent intermediate outputs gives
\[
 \sum_\gamma\int
       \chi_\gamma(a;V)\,G(t,a;V)\,dR(a;V)
   =\int G(t,a;V)\,dR(a;V).
 \tag{DW.24}
\]
The identity holds coefficientwise at every finite order, with the
full marked integrand. At the first \(\Omega_1\)-full step it
recovers the original fluctuation integral with its stationary,
centered quadratic form; the complete interacting mean is not
asserted to be zero. It does not condition on a retained rare-hole
boundary value.

This explains a concrete advantage of summing source densities
before taking absolute values. It is not permission to run later
history-dependent kernels on the smaller state \(V\) unless their
sufficiency or their exact latent-path integration is established.
Nor does (DW.24) remove the P/Q branches or inherited terms at later
steps.

## 7. A concrete sufficient connected-density factorization

The following theorem is an algebraic/analytic bridge. Its
factorization hypothesis must be supplied for the actual source
density, including integration over outer retained fields.

At one scale let \(\Gamma\) be a finite set of polymers. A polymer
\(\gamma\) has a nonempty physical block carrier \(X_\gamma\). Incompatibility
means overlapping enlarged carriers; a fixed finite-range
incompatibility can be put in this form by the stated collar
enlargement. Suppose the actual complete source partition function,
up to a source-independent factor and any explicitly retained local
source term, has the exact form
\[
 \Xi(t)=\sum_{\mathcal A\ {\rm compatible}}
                    \prod_{\gamma\in\mathcal A}z_\gamma(t).
 \tag{DW.25}
\]
The activities may be signed. They must be obtained by exact
factorization/integration of the original densities; an arbitrary
list of component probabilities does not establish (DW.25).
In particular, a correlated reference measure cannot be replaced by
a product reference without its connected interaction factors.

Let
\[
 W_\kappa(X)=e^{\kappa(|X|+\mathsf t(X))}.
 \tag{DW.26}
\]
Assume, with fixed \(a>0\) and a strict margin,
\[
 \sup_b\sum_{\gamma:\,b\in X_\gamma}
       |z_\gamma(0)|\,W_\kappa(X_\gamma)e^{a|X_\gamma|}
                  \le a/4 .
 \tag{DW.27}
\]
For a nonempty labeled source set \(I\), \(|I|=m\), assume
\[
 \sum_\gamma W_\kappa(X_\gamma)e^{a|X_\gamma|}
       |\partial_Iz_\gamma(0)|
       \le B^m(m!)^p h^{-4m}\eta_I,\qquad p\ge1,
 \tag{DW.28}
\]
where every nonzero derivative's carrier contains the physical
anchors of all its source labels. For a fixed anchor family the
right side is volume independent. The factors \(\eta_I\) may be
taken at most one for the basic assertion.

### Theorem DW.3 — linked clusters preserve the fixed factorial class

Under (DW.25)--(DW.28), the finite formal source coefficients of
\(\log\Xi(t)-\log\Xi(0)\) have an absolutely convergent connected
carrier expansion, with
\[
 \sum_\alpha W_\kappa(X_\alpha)
          |C_{I,\alpha}|
       \le C^m(m!)^p h^{-4m}.
 \tag{DW.29}
\]
The constants are uniform in the volume and the number of polymers.
If one distinguished density perturbation is multiplied by a small
parameter \(\varepsilon\), coefficients containing it acquire that
factor, under the same strict margin.

**Proof.** The logarithm of the finite hard-core gas has the formal
connected-graph expansion
\[
 \log\Xi
 =\sum_{n\ge1}\frac1{n!}
       \sum_{\gamma_1,\ldots,\gamma_n}
       \phi^T(\gamma_1,\ldots,\gamma_n)
                       \prod_{\ell=1}^nz_{\gamma_\ell},
 \tag{DW.30}
\]
where \(\phi^T\) sums products of the factors
\(-\mathbf1_{\{\gamma_i\not\sim\gamma_j\}}\) over connected graphs.
The hard-core tree bound is
\[
 |\phi^T(\gamma_1,\ldots,\gamma_n)|
 \le\sum_{T\ {\rm tree}}\prod_{\{i,j\}\in T}
                     \mathbf1_{\{\gamma_i\not\sim\gamma_j\}}.
 \tag{DW.31}
\]
One proves it by assigning every connected graph its canonical
breadth-first rooted tree, with a fixed order for ties. Graphs with
the same tree form intervals between that tree and its allowed
extra edges. Summing the signs on an interval gives a product of
factors \(1-1\), or a single term of modulus one. Summing the
remaining trees gives (DW.31).

For a rooted tree at \(\gamma\), the positive offspring sum obeys
\[
 T_\gamma
 \le \exp\!\left(\sum_{\gamma'\not\sim\gamma}
              |z_{\gamma'}(0)|W_\kappa(X_{\gamma'})
                         T_{\gamma'}\right).
 \tag{DW.32}
\]
Truncate the depth and start at one. Since overlap with \(X_\gamma\)
can be charged to a block of \(X_\gamma\), (DW.27) inductively bounds
\(T_\gamma\) by \(e^{a|X_\gamma|}\), with room for perturbations.
The rooted graph sum is therefore absolutely convergent. For a
connected overlap cluster,
\[
 W_\kappa\!\left(\bigcup_\ell X_{\gamma_\ell}\right)
            \le\prod_\ell W_\kappa(X_{\gamma_\ell}),
 \tag{DW.33}
\]
because its internal spanning trees can be joined through the
overlaps. Thus the argument controls the actual union carrier,
not only a contracted component distance.

For a variation \(v=(v_\gamma)\), use the norm
\[
 \|v\|_*=\sum_\gamma
       W_\kappa(X_\gamma)e^{a|X_\gamma|}|v_\gamma|.
 \tag{DW.34}
\]
The rooted bound shows that the connected-cluster array for
\(\log\Xi(z+v)-\log\Xi(z)\) has weighted norm at most \(C\|v\|_*\)
in a fixed ball \(\|v\|_*<c_a\). There is no extensive vacuum term:
every term in the difference has a distinguished variation.
Mixed Cauchy estimates on the polydisc with directional radii
\(c_a/(2r)\), followed by \(r^r\le e^r r!\), give
\[
 \|D^r\log\Xi(z)[v_1,\ldots,v_r]\|_{\kappa}
          \le C^r r!\prod_{\ell=1}^r\|v_\ell\|_*.
 \tag{DW.35}
\]
The strict margin in (DW.27) is used here. This is an analytic
statement in the activity variations; it does not assume a
convergent series in the physical sources. The convergent cluster
identity also supplies the branch of the logarithm: its exponential
equals the finite gas partition polynomial by the formal identity
near zero activities and analytic continuation inside this norm
ball.

Finally substitute the finite jets of the activities. The
Faà di Bruno partition formula and (DW.28) give the sum
\[
 C^m B^m h^{-4m}
       \sum_{\pi\in\Pi_m}|\pi|!\prod_{D\in\pi}(|D|!)^p.
 \tag{DW.36}
\]
By (DW.14), with its factor \(r!\), this is bounded by
\(C_1^m(m!)^p h^{-4m}\). Every source anchor is in its marked
polymer and hence in the connected union. Absolute convergence and
compatibility under truncation follow from the same majorant.
Keeping one distinguished perturbation throughout the rooted
argument proves its linear \(\varepsilon\) factor. ∎

If activities are integrals of signed coefficient measures, replace
their absolute values in (DW.27)--(DW.28) by the corresponding total
variations. The same proof applies by the triangle inequality.
The source-density factorization (DW.25) remains an independent
requirement; replacing numbers by measures does not manufacture it.

The theorem gives an explicit mechanism by which successful
component masses from (DW.16) can pay full footprints without a
second normalization loss. It does not prove that all actual
regular, residual, inherited, boundary and retained-field
interactions satisfy (DW.25)--(DW.28).

If (DW.25) has only been proved with an exterior \(v\) held fixed,
then (DW.29) is only a conditional connected estimate. The actual
outer logarithm is still (DW.20). Its connecting factors must be
included by a further density expansion or by the specified terminal
joint-cumulant bounds. Taking an ordinary average of the conditional
logarithm would not be the connected coefficient and would lose
H05. The conclusion used in Section 9 is expressly the full-law
connected certificate, with that outer step included.

## 8. Normalization and factorial budgets on joint tests

For normalized full scalar coefficients \(M_I\), the final connected
coefficient is exactly
\[
 C_I=\sum_{\pi\in\Pi(I)}
       (-1)^{|\pi|-1}(|\pi|-1)!\prod_{B\in\pi}M_B.
 \tag{DW.37}
\]
Suppose \(|M_I|\le A^{m+1}(m!)^p\), \(p\ge1\). Equation (DW.14)
implies
\[
 \sum_{\pi\in\Pi_m}(|\pi|-1)!
                         \prod_{B\in\pi}(|B|!)^p
             \le 2^m(m!)^p.
 \tag{DW.38}
\]
Thus taking this **one final logarithm** preserves a fixed factorial
class. The reverse exponential passage does also. This assertion is
about coefficient growth, not spatial clustering.

For distributions the inputs must be bounds on joint tests, not
only simple tensor tests. The existing proved S01 theorem supplies
the corresponding tensor-product/distribution argument and inverse
stability with unchanged fixed \(q,p\). Consequently a connected
joint-test density certificate below can be fed to that theorem
without a new hierarchy definition. No claim that a scalar
probability estimate alone is already a joint-test estimate is made.

## 9. Physical connected kernels and shrinking contacts

### 9.1 A sufficient connected-measure output

Assume the actual exact connected density expansion has been
assigned to shells \(j\), by a fixed rule applied to its full
connected tags, and a terminal term. Suppose a shell coefficient
with insertion positions \(\mathbf x=(x_1,\ldots,x_m)\) has signed
measure tags \(\mathcal C_{j,I,\alpha}(\mathbf x)\), with
\[
 \frac1{\mathscr Z}\sum_\alpha
       W_\kappa(X_\alpha)
       \|\mathcal C_{j,I,\alpha}(\mathbf x)\|_{\rm TV}
 \le A^{m+1}(m!)^{p_0}h_j^{-4m}w_j.
 \tag{DW.39}
\]
Every \(X_\alpha\) contains all insertion anchors, all current or
contact insertions in that tag, and the physical scopes of its
connecting factors. Its integral is a term in the exact connected
coefficient of (DW.19).

Then its actual physical kernel satisfies
\[
 |t_{j,I}(\mathbf x)|
 \le A_1^{m+1}(m!)^{p_0}h_j^{-4m}w_j
       \exp[-c\,\tau(\mathbf x)/h_j].
 \tag{DW.40}
\]

**Proof.** A block tree containing all anchors induces a physical
tree of length at most \(C h_j(\mathsf t(X_\alpha)+m)\), with a
fixed lattice constant. Hence
\(W_\kappa(X_\alpha)\ge e^{c\tau/h_j-C_\kappa m}\).
Apply (DW.39) and the triangle inequality to the integrated
coefficient measures. ∎

This is stronger than the order-dependent tree rate required by
S05. If the available connected certificate only has
\(\kappa/(m+d_0)\), the same argument gives exactly that stated S05
rate instead. The actual measured carrier and its assigned rate
must be used; a component-contracted distance is not substituted.

If the exact shell identity, terminal and one-point budgets, and
\[
                         \sum_j h_j w_j<\infty
 \tag{DW.41}
\]
hold uniformly, the proved S02/S01 bridge gives the full hierarchy
on joint coincidence-flat tests, its uniform tail and cofinal
convergence under the stated resolved-shell convergence. Its
factorial and spatial orders are the recorded S02 ones:
\[
 q=\max(6,q_1,q_T),\qquad
 p=\max(1,p_T,p_0+5),
 \tag{DW.42}
\]
enlarged for any actual contact/error budget. This is a concrete
downstream implication; the density interface has not changed what
S02 consumes.

### 9.2 A direct shrinking-contact estimate

Let \(\eta_I\) be a finite signed measure on \(m\) spatial insertion
positions, supported where every \(x_i\) lies within physical
distance \(\rho\) of \(x_1\). Taylor-expand a smooth joint test
around \((x_1,\ldots,x_1)\) in the \(4(m-1)\) relative coordinates,
through order \(r=qm\), with fixed integer \(q\ge1\).
Integrating that polynomial against \(\eta_I\) defines explicit
contact coefficients, supported on the complete diagonal, and
\[
 |\eta_I(F)-\eta_I(T_{qm}F)|
 \le C_q^m\rho^{qm+1}\|\eta_I\|_{\rm TV}\,
           \nu_{(q+1)m}(F)
 \tag{DW.43}
\]
Here \(\nu_{(q+1)m}\) dominates the displayed derivative supremum.
This statement uses the finite total variation of this measure.
A spatially weighted version requires the corresponding weighted
variation estimate; it is not inferred from an extensive total mass.

**Proof.** The one-dimensional Taylor formula along the segment of
relative coordinates bounds the remainder by
\[
 \frac{\left(\sum_{\ell=1}^{4(m-1)}|y_\ell|\right)^{r+1}}
      {(r+1)!}
       \max_{|\alpha|=r+1}|\partial^\alpha F|.
 \tag{DW.44}
\]
The numerator is at most \([C m\rho]^{qm+1}\).
Stirling's lower bound for \((qm+1)!\) makes its coefficient at
most \(C_q^m\rho^{qm+1}\). Integrate against \(|\eta_I|\).
Since \(qm+1\le(q+1)m\), the displayed joint seminorm suffices. ∎

The coefficients have differential order at most \(qm\), linear in
source order. If the extraction is defined label-by-label from the
same full connected array, reducing a source truncation retains the
same lower-order coefficients. The same construction applies on a
specified partial diagonal for a labeled subcluster; compatible
overlap subtractions still require a fixed forest/extraction rule.

For the actual rare component geometry a radius of order
\(MR_kh_j\) is allowed only when it tends to zero in the intended
limit and its powers satisfy the summed error budget. A fixed
physical-cell contact is not obtained from (DW.43). The identities
above do not by themselves construct the actual F06 extraction,
inverse-running weights or F07/S06 summability.

## 10. A uniform-depth criterion, and what it does not prove

Let \(\mathbf A_j\) denote the complete coefficient-measure arrays.
Write their exact recurrence as
\(\mathbf A_{j+1}=\mathbb T_j\mathbf A_j+\mathbf R_j\).
Let \(\mathsf P_j\) be the verified invertible running change of
field/basis coordinates, extended labelwise to the full coefficient
array. Set
\(\mathbf U_j=\mathsf P_j^{-1}\mathbf A_j\),
\(\mathcal S_j=\mathsf P_{j+1}^{-1}\mathbb T_j\mathsf P_j\), and
\(\widehat{\mathbf R}_j=\mathsf P_{j+1}^{-1}\mathbf R_j\).
These definitions retain the actual inverse-running weights.
Use a
factorial seminorm
\[
 \mathcal N_j(\mathbf U)
 =\sup_{m\ge1}\sup_{\text{anchored }I}
       \frac{\mathcal D_{j,m}(\mathbf U_I)}
            {A^m(m!)^p},
 \tag{DW.45}
\]
with one fixed \(A,p,\kappa\) and the appropriate connected/forest
version of the density certificate.

Suppose the **actual matched** scale step, including its physical
factor, coarea, all old vertices and density currents, admits
\[
 \mathcal N_{j+1}(\mathcal S_j\mathbf U)
       \le (1+\varepsilon_j)\mathcal N_j(\mathbf U),
 \qquad
 \mathcal N_{j+1}(\widehat{\mathbf R}_j)\le r_j,
 \tag{DW.46}
\]
and
\[
 \sum_j\varepsilon_j<\infty,\qquad
 \sum_j r_j<\infty.
 \tag{DW.47}
\]
Then the matched full density arrays have a uniform-depth bound
with the same factorial exponent. The contribution of all
remainders born after step \(J\), propagated to any later step, is
bounded by \(e^{\sum_j\varepsilon_j}\sum_{j\ge J}r_j\).

**Proof.** Iterate the exact linear transport and the additive
telescope. The product of operator norms is at most
\(\exp(\sum_j\varepsilon_j)\). Apply the triangle inequality to
the stated inverse-weighted remainder array. The supremum over \(m\) uses
the same fixed denominator in every step. No new partition count
is applied at each depth. ∎

A bounded product norm alone does not imply convergence of the
multiplicative part; for example, isometries can rotate indefinitely.
Resolved-shell and terminal convergence, or a separately justified
near-identity summable operator difference on a common space, is
still required for the cofinal limit.

This is a sufficient induction statement, not a proof of
(DW.46)--(DW.47) for Yang--Mills. In particular, a bound \(C^m\) with
the same \(C>1\) lost at every scale would replace \(A\) by \(C^jA\)
and would not pass. Neither TV contraction nor the successful
component reserve alone establishes the matched scale step.

An inherited component cannot have its original rarity spent anew
at each later stage. A valid genealogical ledger must either prove
new conditional suppression at the stated renewal operations, or
allocate nonnegative costs \(s_{j,X}\) to that owner with
\(\sum_j s_{j,X}\) bounded by its proved total reserve. The source
H02/unreplaced-history problem is not solved by retaining an old
birth label in the notation.

## 11. Exact interface changes and remaining actual-law gates

| Interface | Density formulation | What remains to prove |
|---|---|---|
| Original M03 pointwise conditional norm | Replaced by actual signed coefficient measures and integrated carrier costs. | No bounded conversion back is claimed; GO prevents the naive one. |
| M04 scalar matching | Must be an equality of the complete weighted scalar coefficient, current scalar basis, identity and remainder. | Actual coefficients and a current-scale density remainder, with all E/B/R and coarea terms. |
| M06 full jets | Full coefficients are transported linearly; linked-cluster extraction preserves a fixed factorial class. | Actual local density factorization and response bounds, not merely single-field estimates. |
| M07 depth | Criterion (DW.46)--(DW.47) keeps one fixed factorial and spatial budget. | Uniform actual carrier transport, running matrices, irrelevant gains and inherited ownership. |
| H03 resets | The exact complete posterior is preserved in (DW.3), (DW.18). | Its physical density-connector/current costs in the enlarged expansion. |
| H04 bad sectors | NM20 proves the successful-sector energy/rank/footprint budget. | Residual, inherited and unreplaced sectors, and mixed incoming marked partners. |
| H05 outer means | Included exactly by the single outer logarithm. | The actual retained-field interaction/cumulant certificate; no within-sector replacement. |
| Physical currents | Frozen-kernel physical source derivatives obey (DW.22). | Any native retained-coordinate, interface or reference-change response used to prove the density expansion. |
| F06/F07/S06 contacts | (DW.43) gives a joint-test shrinking-stencil mechanism with linear order. | The actual extraction forest, inverse-running weights and summable errors. |
| S04/S05/S02 hierarchy | (DW.39)--(DW.42) give the precise conversion to the existing physical kernel/terminal tests. | Actual connected density arrays, shell identity and terminal bounds. |

In particular, the following are genuine source tasks rather than
norm definitions:

1. **A complete marked density expansion.** It must retain the
   primitive selectors, coordinate maps, old Gaussian forms,
   inherited E/B/R terms, fresh and old normalizers and cross actions.
   A successful mass estimate as a function of \(v\) is not that
   expansion.
2. **Mixed marked reserves.** Old inputs correlated with a bad event
   need the joint energy/current bounds of their specified class.
   An unmarked probability cannot be multiplied by an arbitrary
   incoming weight.
3. **Outer connected responses.** The shared retained background
   has to supply the true connecting density factors. Treating it
   as fixed and discarding its covariance would lose H05.
4. **Residual and genealogical suppression.** NM20's successful
   deletion theorem does not supply these sectors.
5. **Physical matching and summability.** The factor \(h^{-4m}\),
   actual mixing matrices, compatible contact coefficients and
   inverse-running-weighted gains remain necessary.

The route is mathematically coherent and preserves the exact
positive law and every physical source coefficient. It removes the
need to demand a uniformly small normalized mark on a rare history.
The existence proof would be advanced by proving the listed actual
density expansion and matching estimates, rather than by claiming
that a weakened conditional norm already implies them.

Exact coefficient-measure transport also preserves the original
finite-cutoff physical moment functionals, hence their existing
reality, symmetry and reflection-positivity identities on the
original observable algebra. Passing those statements through
contact subtractions and the limit still requires the stated
positive-time compatibility and convergence estimates. The
positive-endpoint coupling trajectory, invertibility/nondegeneracy
of the physical running normalization, terminal/infrared passage,
and nontriviality requirements are unchanged. None is proved by
the density interface alone.
