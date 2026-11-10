# All-order clean and controlled-prefix marked histories

**Status.** The result below closes a further marked sector of the actual positive history law. Sections 1–6 give a fixed factorial bound, at one weak-coupling threshold, for all separated old insertions retained from initial large-field components and subsequently joined by clean mergers. The component need not have been processed by a reset, and the exterior is unrestricted. Section 7 extends this result to the controlled early prefix of H9, allowing roots first swallowed there and the specified early births and preparation failures; every ordinary birth used in that prefix must have an unchanged complete causal stencil. The theorem is a normalized expectation, not an unnormalized activity estimate. General later births, failed preparations after the controlled prefix, and between-sector posterior cumulants remain outside the result.

The inputs are the actual normalized initial chessboard bound H8.1, the clean-merger geometry H8-A, and the occupied-cell theorem H8-B. The new point is to combine witness trees at different stopping times without paying a number-of-insertions dependent age cost.

### 1. Roots, scales, and the selected event

Use terminal units, so that \(h_j=aL^j\le1\), and write

\[
T(h)=1+\log(1/h),\qquad
Q=p_0(g_0)^2,\qquad
w=\lceil C_RR_0\rceil+u_0+C_w,
\qquad \sigma_j=2^{\lfloor j/w\rfloor}.
\tag{R9.1}
\]

All constants below may depend on the fixed source choices, the field family, and its fixed logarithmic exponent \(s\ge0\). They are independent of the cutoff, the horizon, the volume, and the number \(m\) of marks. The standing trajectory gives
\(Q/w\to\infty\) and \(Q/R_0^4\to\infty\) at the weak endpoint.

Use the compatible source tori and the cofinal coarse-size condition of H8, enlarged by the same fixed factor to contain the contractible witness neighborhoods. All references to an unrestricted exterior mean that its history and fields are integrated in the original normalized law. No estimate here is claimed uniformly after conditioning on arbitrary exterior values.

Fix \(m\ge2\) microscopic marks with deterministic envelopes

\[
|F_i|\le A_i a^{-4}T(a)^s,
\qquad
\delta=\min\{1,\min_{i\ne l}\operatorname{dist}(x_i,x_l)\}>0.
\tag{R9.2}
\]

Distances are periodic distances on the original torus. Include the fixed microscopic support collars in the root definition. Initially assume their diameters are at most \(\delta/4\); if \(\delta\le C a\), the envelope itself supplies \(a^{-4}\le C\delta^{-4}\), and the same conclusion follows directly from the clean survival bound.

Let \(\mathcal C_{j,I}\) require all of the following:

1. Each entire root support belongs to an initial large-field component and remains retained in its unresolved descendant throughout the selected interval.
2. Every selected ancestor is clean in the sense of H8: its only births are initial births, every attempted preparation succeeds, and no successful reset has occurred in that ancestry.
3. At scale \(j\), one such unresolved component contains all the roots.

Mergers with unmarked clean components are allowed, as are arbitrary histories outside the selected ancestry. This is a sector of the original positive lift \(\Pi\); it is not normalized by its own probability.

For each root \(i\), let \(\tau_i\) be the first scale at which its component contains any other marked root, including a root whose own stopping time is already past. Set \(\tau_i=0\) if the initial component already contains another mark. On \(\mathcal C_{j,I}\), all \(\tau_i\le j\). Write

\[
\tau_* = \min_i\tau_i.
\tag{R9.3}
\]

Stopping when meeting an already stopped root is essential: it makes the singly charged ancestry intervals disjoint.

### 2. The multiscale witness certificate

#### Lemma R9-A: disjoint leaves at different first-meeting times

For a specified stopping-time vector \(\boldsymbol\tau\), let \(A_{\boldsymbol\tau}\) be the event that the retained clean components realize these first meetings. There are fixed \(c,C>0\) such that

\[
\Pi(A_{\boldsymbol\tau})
\le
\exp\!\left[-cQ\sum_{i:\tau_i>0}
 2^{\lfloor(\tau_i-1)/w\rfloor}\right].
\tag{R9.4}
\]

Roots stopped at scale zero are omitted from this charge. No assertion of one rare initial cube per such root is made.

**Proof.** Before a successful reset, the source covers, fixed layers, and optional rectangular fills preserve predecessor connected components. They can merge them but cannot split a retained clean component. The initial ancestor sets of the components immediately before the positive stopping events are therefore pairwise disjoint. If an initial ancestor belonged to two of these components, the earlier retained root would also belong to the later one, and that later root would already have stopped. This contradicts its first-meeting definition. The same argument applies to the different components immediately preceding a simultaneous merger.

For each positive \(\tau_i\), apply the H8-A witness construction inside its actual predecessor component at time \(\tau_i-1\). The retained root anchors that component. The initial-scale and first-active-scale cases use H8 initial anchoring directly. The tree has at least
\(c\,2^{\lfloor(\tau_i-1)/w\rfloor}\) distinct initial bad cubes. Witnesses descending from different predecessor components have disjoint initial leaves, even if their geometric cones overlap at different scales.

If \(N\) is the sum of their leaf counts, the ordered embedding count is at most \(\exp(CwN)\). Requiring the leaves of different trees to be distinct only decreases that count. Apply H8.1 to the union of the specified leaves and sum over embeddings. Since \(Q\gg w\), the exponent \(-c_0QN+CwN\) retains a fixed negative fraction of \(-QN\). All later positive history probabilities sum to at most one. This proves (R9.4) with no history multiplicity or posterior denominator. \(\square\)

This lemma uses actual ancestry, not just the same-scale probability H8.8. A root entering a component only later has no such certificate for the interval before entry; that case is excluded in the definition of \(\mathcal C_{j,I}\).

#### Lemma R9-B: the earliest meeting supplies geometry

Let \(B_t\) be the event that a clean component at scale \(t\) contains at least two of the marked root supports. H8.17, summed over at most \(m^2\) root pairs, implies

\[
\Pi(B_t)
\le C m^2
\exp[-cQ\sigma_t-c\delta/h_t].
\tag{R9.5}
\]

Indeed, the original exponent contains
\(Q\sigma_t\delta/(M R_t h_t)\). Since \(R_t\le C R_0\) and \(Q/R_0\) is uniformly large, it pays \(c\delta/h_t\) while leaving a fixed rare reserve. The same initial-component animal argument proves the case \(t=0\). A component containing two collars separated by \(\delta\) has diameter at least a fixed multiple of \(\delta\).

Finally, the selected event at scale \(j\) entails survival of the first retained root, so

\[
\Pi(\mathcal C_{j,I})\le C\exp[-cQ\sigma_j].
\tag{R9.6}
\]

These three estimates need no independence. For any events \(A,B,C\),
\(\Pi(A\cap B\cap C)\le[\Pi(A)\Pi(B)\Pi(C)]^{1/3}\). Use that inequality with the multiscale certificate, the earliest-meeting geometry, and terminal survival.

### 3. Paying ages before meetings, uniformly in the order

For each positive stopping time,

\[
a^{-4}T(a)^s
\le h_{\tau_i}^{-4}T(h_{\tau_i})^s
e^{D_s\tau_i},
\qquad
D_s=4\log L+s\log(1+\log L).
\tag{R9.7}
\]

The same relation with factor one holds at \(\tau_i=0\). Choose the weak-coupling endpoint once so that the fixed fraction of \(Q\) remaining after the preceding Hölder step satisfies

\[
\sum_{t\ge1}
\exp\!\left[D_st-cQ2^{\lfloor(t-1)/w\rfloor}\right]
\le C_s.
\tag{R9.8}
\]

This bound is uniform in \(w,Q\). To verify it, group the sum into windows
\(nw+1\le t\le(n+1)w\). The exponent is at most
\(D_s(n+1)w-cQ2^n\). Since \(n+1\le C2^n\) and \(Q/w\) is sufficiently large, it is at most \(-c'Q2^n\). The factor \(w\) is absorbed into \(e^{c'Q/2}\), giving (R9.8). This choice depends on the fixed \(s\), not on \(m\).

Summing every positive stopping-time charge therefore costs at most \(C_s^m\). The scale-zero choices cost no age factor; allowing each root either choice changes only that same exponential-in-order constant. The vector need not be geometrically realizable when summed: enlarging to all vectors only increases the bound.

After paying these ages, all remaining physical scale factors are bounded using the *single earliest meeting*:

\[
\prod_{i=1}^m h_{\tau_i}^{-4}T(h_{\tau_i})^s
\le h_{\tau_*}^{-4m}T(h_{\tau_*})^{sm}.
\tag{R9.9}
\]

This avoids trying to charge a large previously merged component again each time another root joins it.

Put \(u=\delta/h_{\tau_*}\). For \(u\ge1\),
\(T(h_{\tau_*})=T(\delta)+\log u\), while for \(u\le1\) the factor on the left of (R9.9) is already bounded by
\(\delta^{-4m}T(\delta)^{sm}\). For fixed \(s\),
\((1+\log u)^s\le C_su\) on \(u\ge1\). Hence

\[
\sup_{u>0}
u^{4m}(1+\log_+u)^{sm}e^{-cu}
\le C_s^m(m!)^5.
\tag{R9.10}
\]

When \(s=0\), the right side can be improved to \(C^m(m!)^4\). The inequality follows by maximizing \(u^{5m}e^{-cu}\) and using Stirling's elementary factorial bound. This is a fixed factorial exponent; neither \(w\) nor \(m\) enters its value.

### 4. The actual normalized all-order theorem

#### Theorem R9-C: a scale-summed marked bound before any reset

At one weak-coupling threshold, for every \(m\ge2\),

\[
\boxed{
\sum_{j:\,h_j\le1}
\mathbb E_\Pi\!\left[
1_{\mathcal C_{j,I}}\prod_{i=1}^m|F_i|
\right]
\le
C_s^{m+1}(m!)^{\nu_s}
\left(\prod_{i=1}^m A_i\right)
\delta^{-4m}T(\delta)^{sm}e^{-cQ},
\quad
\nu_0=4,\quad \nu_s=5\ (s>0).
}
\tag{R9.11}
\]

**Proof.** Partition the selected event by its actual stopping-time vector. On each part use the deterministic envelopes, (R9.7), and (R9.9). Its probability is bounded by the geometric mean of (R9.4), (R9.5) at \(t=\tau_*\), and (R9.6). Absorb the factor \(m^{2/3}\) into \(C^m\). Retain the terminal factor \(e^{-cQ\sigma_j}\), and use the earliest-meeting spatial factor with (R9.10). The remaining sum over stopping vectors is bounded by (R9.8) independently for each charged root. For uncharged roots the time is exactly zero. Thus the fixed-scale bound is

\[
C_s^{m+1}(m!)^{\nu_s}
\left(\prod_i A_i\right)
\delta^{-4m}T(\delta)^{sm}e^{-cQ\sigma_j}.
\tag{R9.12}
\]

Finally,
\(\sum_j e^{-cQ\sigma_j}\le Cw e^{-c'Q}\le C e^{-c''Q}\).
This proves (R9.11). All expectations are under the complete normalized positive lift. In particular, arbitrary events and normalizers in the exterior have already been integrated with their true probabilities. \(\square\)

The proof actually bounds the product of deterministic envelopes multiplied by the selected probability. Consequently the same right side controls

\[
\sum_j
\left\|\mathbb E_\Pi\!\left[
1_{\mathcal C_{j,I}}\prod_iF_i\mid\mathscr G_j
\right]\right\|_{L^1(\Pi)}
\tag{R9.13}
\]

for any retained sigma algebras \(\mathscr G_j\). This is useful for exact marked density coefficients. It does not identify a product of different posterior means with one conditional product.

### 5. Selected conditional cumulants, with their probability retained

Write \(p_{j,I}=\Pi(\mathcal C_{j,I}\mid\mathscr G_j)\). When \(p_{j,I}=0\), set the following weighted expression to zero. On positive support take every conditional cumulant under the **same** law
\(\Pi(\cdot\mid\mathscr G_j,\mathcal C_{j,I})\).

The finite moment-cumulant identity and the deterministic seed envelopes give

\[
p_{j,I}\left|\kappa\left(F_1,\ldots,F_m
\mid\mathscr G_j,\mathcal C_{j,I}\right)\right|
\le C^m m!\,p_{j,I}\left(\prod_i A_i\right)a^{-4m}T(a)^{sm}.
\tag{R9.14}
\]

For completeness, the combinatorial coefficient is
\(\sum_{\pi\in\mathcal P_m}(|\pi|-1)!\le C^m m!\).
It is bounded by the ordered Bell number
\(\sum_r r!S(m,r)\); its exponential generating function is
\((2-e^z)^{-1}\), analytic on any fixed circle of radius less than \(\log2\). Equivalently the same bound follows from the positive coefficient expansion on one such real radius. This use of a finite cumulant identity imposes no exponential-source analyticity on the Yang–Mills law.

Taking expectations, using \(\mathbb E p_{j,I}=\Pi(\mathcal C_{j,I})\), and repeating the envelope proof above yields the next actual sector theorem:

\[
\boxed{
\sum_j\mathbb E_\Pi\!\left[
p_{j,I}\left|\kappa(F_1,\ldots,F_m
\mid\mathscr G_j,\mathcal C_{j,I})\right|
\right]
\le
C_s^{m+1}(m!)^{\nu_s+1}
\left(\prod_iA_i\right)
\delta^{-4m}T(\delta)^{sm}e^{-cQ}.
}
\tag{R9.15}
\]

There is no factor \(p_{j,I}^{-1}\) in the conclusion. The selected law is used only inside a cumulant whose posterior probability is retained. This closes normalized connected coefficients **within this one clean component sector**. Cumulants of the different sector means and the reassembly of all histories remain separate obligations.

### 6. What this adds, and where it stops

R9.11 and R9.15 add actual normalized all-order bounds for an unresolved exterior component, with arbitrary clean mergers and no assumption that the rest of the exterior has already been processed. They retain one fixed factorial exponent and one coupling threshold. The earlier processed-core activity theorem and this theorem address different carriers.

The first-meeting proof is deliberately restricted to roots retained from initial components. For a root first entering at scale \(b>0\), its pre-entry transport must first be controlled in a physical \(h_b^{-4}\) incoming norm. Charging its whole microscopic age to a component that did not previously contain it would invalidate R9-A. The later-birth and preparation results elsewhere in the companion notes do not supply that missing incoming norm.

These estimates are inputs to the route's all-order marked hierarchy and to the unresolved-component part of S2. They do not alone prove either the full marked hierarchy or the complete covariance defect estimate.

### 7. Restarting at the proved early-birth prefix

H9-E now supplies a larger actual normalized base law. Its base time and strength are

\[
J=\lfloor\kappa\log\log\beta\rfloor,\qquad
\Pi(\mathcal S\subset\mathscr A_J^{\rm pre})
\le e^{-c\Gamma_*|\mathcal S|},\qquad
\Gamma_*\ge c e^{\gamma J},\qquad
\Gamma_*\gg R_J^4+w_J,
\tag{R9.16}
\]

where \(\beta=g_0^{-2}\) and
\(\gamma=(2P-4r)/\kappa-2\log D\). This base allows ordinary births and preparation failures during the prefix. Every later ordinary birth used by H9 has an **unchanged complete causal patch**: no current-field integration or replacement has affected any of its arguments. In particular, this condition excludes the LFR I (1.76) integration even on a branch whose eventual final reset fails. The base is not enlarged by treating every failed preparation as an identity operation.

After \(J\), impose the H9-F clean evolution, with arbitrary mergers within the restart class. Require each marked root support to belong to that class already at time \(J\), and to remain retained in its selected descendant afterward. Let \(\mathcal C^{\rm pre}_{j,I}\) also require all those roots to belong to one such component at scale \(j\ge J\). A root may have been regular initially and first swallowed during the prefix. No claim that its microscopic seed remained an unintegrated coordinate during that prefix is needed: the following estimate is for the original marks on the positive history lift, with their original deterministic envelopes.

At the restart scale those envelopes read

\[
|F_i|\le A_i e^{D_sJ}h_J^{-4}T(h_J)^s.
\tag{R9.17}
\]

Apply the proof of R9-C from base time \(J\), with \(Q,w,a\) replaced by \(\Gamma_*,w_J,h_J\). Its multiscale witnesses now have distinct occupied current-\(J\) cells as leaves; H9-E bounds their joint probability. All first-meeting times and age charges in that argument are measured after \(J\). The immediate output is

\[
\sum_{j\ge J}\mathbb E_\Pi
\left[1_{\mathcal C^{\rm pre}_{j,I}}\prod_i|F_i|\right]
\le
C_s^{m+1}(m!)^{\nu_s}
\left(\prod_i A_i\right)
\delta^{-4m}T(\delta)^{sm}
e^{mD_sJ-c\Gamma_*}.
\tag{R9.18}
\]

The remaining prefix age is paid once, with an order-independent factorial budget. Choose the fixed \(\kappa\) still smaller, if necessary, so that \(\gamma\ge D_s\), while retaining H9.20. From (R9.16),

\[
e^{mD_sJ-c\Gamma_*/2}
\le C_s^m\Gamma_*^{mD_s/\gamma}e^{-c\Gamma_*/2}
\le C_s^m m!.
\tag{R9.19}
\]

The last step maximizes a fixed positive variable to a power at most \(m\) against its exponential penalty. The source weak endpoint and \(\kappa\) depend on the fixed seed logarithmic order \(s\); neither depends on \(m\).

#### Theorem R9-D: all orders after early births and failures

The enlarged prefix sector consequently obeys

\[
\boxed{
\sum_{j\ge J}\mathbb E_\Pi
\left[1_{\mathcal C^{\rm pre}_{j,I}}\prod_i|F_i|\right]
\le
C_s^{m+1}(m!)^{\nu_s+1}
\left(\prod_i A_i\right)
\delta^{-4m}T(\delta)^{sm}e^{-c'\Gamma_*}.
}
\tag{R9.20}
\]

Its selected conditional cumulants, always retaining the posterior sector probability as in R9.15, satisfy the same statement with factorial exponent \(\nu_s+2\). Thus convenient integer exponents for the normalized product and selected-cumulant bounds are respectively \(5,6\) for bare seeds and \(6,7\) for seeds with the fixed incoming logarithmic power. All hold at one weak-coupling threshold.

This is a strict extension of the retained-initial-root theorem: it permits roots entering during the controlled early prefix, and it permits the early births and failures in the H9 restart class. Roots first entering after \(J\), ordinary births whose causal patches have undergone current-field replacement, and arbitrary later failures remain outside its statement. Its selected conditional cumulants still do not include the cumulants of different history-sector means.

---
