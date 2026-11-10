# Clean mergers, fresh reset moments, and local energy comparison

**Current status:** Parts IV–VI extend these results to the specified early prefix, every marked order, and all-depth physical Q/R births on strict regular carriers. They do not remove the full-history boundary and terminal restrictions.

**Status:** This note extends the normalized initial-birth analysis to unresolved ancestries with arbitrary mergers of clean initial components. It proves a normalized occupied-cell bound, an ordinary-size exponential moment, a sharp scale-summed two-root bound, and a selected terminal old-field \(L^2\) bound for that sector. Separately, it derives uniform Gaussian moments for the actual fresh reset draw using its own denominator, and proves causal marked bounds for those innovations. General later coarse-background births and failed preparations are not identified with those fresh draws. The last section states the normalized comparison still needed for them.

The frozen forward kernels, running trajectory, original Wilson measure, and deterministic physical subtraction are unchanged. All probabilities below refer to the actual positive joint lift \(\Pi\), unless a particular conditional reset kernel is explicitly indicated. This note does not replace an old observable by a freshly sampled field.

### 1. Initial normalized input and geometric units

Use the actual initial source cubes \(C\) of side \(LM_2R_0\) in fine units, and their bad events \(E_C\) from CMP119 (1.1). H7-E gives

\[
\mu_0\!\left(\bigcap_{C\in\mathcal S}E_C\right)
\le e^{-c_0Q|\mathcal S|},
\qquad Q=p_0(g_0)^2.
\tag{H8.1}
\]

The same inequality holds under \(\Pi\), since its original marginal is \(\mu_0\). H7-E now uses fixed tiles of side \(L\), so its chessboard proof applies to the literal source tori with fine side lengths \(2L^{m_\mu+n}\). No altered torus family is needed.

Let

\[
h_j=aL^j,\qquad s_j=Mh_jR_j.
\tag{H8.2}
\]

Thus \(s_j\) is the physical side length of an active-region \(MR_j\)-cube; it is not the engineering scale of the dimension-four field. Geometric balls and diameters in the witness argument use the sup norm; converting the final separation bound to Euclidean distance only changes fixed constants. Constants may depend on the fixed source choices \(L,M,M_2\), the group, and the fixed logarithmic seed exponent. They do not depend on the cutoff, \(j\), or torus volume.

CMP119 (2.5)–(2.7), with rounding to powers of \(L\), gives constants \(C_R,b_R\) such that

\[
R_j\le C_RR_i,\qquad
\frac{s_j}{s_i}\le C_RL^{j-i},\qquad
\frac{s_i}{s_j}
\le C_R(1+j-i)^{b_R}L^{-(j-i)}
\quad(i<j).
\tag{H8.3}
\]

In particular, \(\sum_{i\le j}s_i\le C_s s_j\). For every sufficiently large fixed \(w\), successive \(w\)-step scales obey \(s_{j-w}/s_j\le1/4\). We choose the weak-coupling threshold so that the macrostep length selected below has this property. The usual cofinal coarse-size condition on the torus can be increased by a fixed factor to contain the finite geometric neighborhoods used below.

### 2. The sector: clean initial ancestry, with mergers allowed

A current unresolved component has **clean initial ancestry** if every large-field creation in its unresolved ancestry belongs to the initial \(P_0\) family, every preparation attempted in that ancestry succeeds, and no ancestor has already undergone a successful reset. Mergers of any number of components with that same property are allowed.

This sector excludes a merger with a component containing a later birth or a preparation failure. Such a merger would import that history into the ancestry. Other histories elsewhere in the system are unrestricted.

Let \(\mathscr A_j\) be the union of current \(MR_j\)-cells belonging to these components. It is an actual history event, not an independently sampled occupied-cell model. All descendants and ancestors used in the argument retain their original labels; they are not recentered or renormalized by their individual history masses.

#### 2.1 Three deterministic properties of the source geometry

The proof uses the following properties.

**Finite propagation.** In a window with no new large-field creation in the selected ancestry, a descendant cell can be traced to a cell at the beginning of the window at physical distance at most \(C_{\rm prop}s_{\rm end}\). The same assertion holds after the optional rectangular fill. To see this, each covering and fixed layer addition moves a boundary by at most a fixed multiple of the next \(s_j\), and a rectangular fill of a component of diameter at most \(100s_j\) moves a point by at most \(100s_j\). Sum these distances using (H8.3).

**Small-envelope reset.** Fix \(D<\infty\). A collection of ancestors contained in one cube of side \(Ds_i\), with no merger from outside that collection, enters a cube of side strictly less than \(100s_n\) after a fixed \(u_0(D)\) further steps. It remains within the small-size criterion while it continues without an outside merger or new birth. Here one uses the source's more precise \(S\)-envelope estimate, not the rough finite-propagation constant: LFR II pp.384–385 gives the limiting \(64MR_n\) envelope. The descendant bounding-box side is at most \(Ds_i+64s_n\), after a harmless fixed adjustment of \(D\) for the first cover. By (H8.3), choose \(u_0(D)\) so that \(Ds_i/s_n\le20\) for every \(n-i\ge u_0(D)\). The bound is then \(84s_n<100s_n\).

The optional rectangular fill does not invalidate this envelope. Filling each small component adds points only inside that component's bounding box, hence leaves the bounding box of the whole collection unchanged. Taking the next grid cover and its fixed layers has the same bounding box whether applied to the collection or to its bounding box. Removing a reset component can only shrink the collection. Thus iteration is bounded by the same \(S\)-evolution of the initial bounding box. Internal mergers do not enlarge this bound.

After an additional \(C_RR_0+1\) clean steps, every required predecessor region satisfies the small-size condition and the clean window is long enough. LFR I p.177 takes the union of all eligible components, and pp.200–201 performs the reset. Since a failed preparation is excluded in this sector, the component must then leave the unresolved class.

**Initial anchoring.** Every cell in \(\mathscr A_j\) with \(j\le w\) has an initial bad source cube within distance \(C_{\rm init}s_j\). This is finite propagation through the first construction and the next \(j\) covers. The number of candidate source cubes in such a neighborhood is at most \(\exp(Cw)\). The first-step covers and the bounded rectangular fill only change the fixed constants.

These are support-level statements. A large component is not treated as a single indivisible parent: its widely separated occupied cells are separate possible witnesses.

### 3. A deterministic two-witness lemma

Choose \(C_{\rm loc}>10C_{\rm prop}+10\), enlarge it to cover the first-step neighborhoods, and then choose a fixed
\(D>20C_{\rm loc}\). Take

\[
w=\left\lceil C_RR_0\right\rceil+u_0(D)+C_w,
\tag{H8.4}
\]

with fixed \(C_w\) large enough for the source's eligibility window and for
\(s_{j-w}/s_j\le\min(1/4,1/D)\). The latter follows from (H8.3) and ensures that the diameter \(Ds_{j-w}\) is smaller than \(s_j\) in the isolation argument below.

#### Lemma H8-A: survival forces two separated active cells

If a cell containing \(x\) belongs to \(\mathscr A_j\) and \(j-i=w\), then there are two cells of \(\mathscr A_i\), with centers \(x_1,x_2\), satisfying

\[
x_1,x_2\in B(x,C_{\rm loc}s_j),\qquad
|x_1-x_2|>D s_i.
\tag{H8.5}
\]

Their components need not be different.

**Proof.** Let \(A\) be the union of all active cells at time \(i\) ancestral to the selected component at time \(j\). Every cell of \(A\) belongs to \(\mathscr A_i\). Finite propagation supplies an ancestor within distance \(C_{\rm prop}s_j\) of \(x\).

Suppose that \(A\cap B(x,C_{\rm loc}s_j)\) has diameter at most \(Ds_i\). The ancestors in this intersection then lie in one fixed-size cube. Any other ancestor lies outside the displayed ball. Because the near ancestor is within \(C_{\rm prop}s_j\) of \(x\), the gap between the near collection and the outside collection is greater than twice the entire propagation distance over the window. They cannot merge during the window.

If a single component of \(A\) were to run from the near collection to outside the ball, its connected cell path would already give two cells in the ball separated by more than \(Ds_i\). Thus this case also contradicts the supposition.

The near collection therefore evolves in isolation. By the small-envelope property it becomes small after \(u_0(D)\) steps, stays small, and then completes the required clean window. It must reset before time \(j\), contradicting the existence of the selected unresolved descendant. Hence the two cells in (H8.5) exist. Moving to canonical cell centers changes only the fixed constants. \(\square\)

This argument includes a single huge earlier component: two separated cells on its connected support give the two witnesses. It does not require two separate component parents.

#### 3.1 Distinct initial leaves and the embedding count

For a given \(j\ge1\), set \(n=\lfloor (j-1)/w\rfloor\) and choose equally spaced backward times
\(t_\ell=t_0+\ell w\), with \(1\le t_0\le w\) and \(t_n=j\). Thus the base is always at or after the first actual active scale. Apply H8-A at every internal vertex of an ordered binary tree. Since
\(2^n\ge\tfrac12\,2^{\lfloor j/w\rfloor}\), the final estimates below can use \(2^{\lfloor j/w\rfloor}\) after changing their fixed constants.

All initial leaves descending from a child at scale \(t_{\ell-1}\) lie within a ball of radius \(C_{\rm cone}s_{t_{\ell-1}}\) about that child, where \(C_{\rm cone}<D/3\) after fixing the constants in the preceding order. Indeed, sum the successive displacement radii \(C_{\rm loc}s_{t_r}\) using \(s_{t_{r-1}}/s_{t_r}\le1/4\), and include the initial anchoring radius. The two children are separated by \(Ds_{t_{\ell-1}}\), so the two descendant leaf neighborhoods are disjoint. Induction gives \(2^n\) distinct initial bad source cubes.

At an internal vertex there are at most
\[
C\left(\frac{s_{t_\ell}}{s_{t_{\ell-1}}}\right)^{2d}
\le e^{Cw}
\tag{H8.6}
\]
ordered child choices. At each leaf, initial anchoring has at most \(e^{Cw}\) choices. Therefore the number of embedded, fully specified witness trees is at most
\[
\exp(C_{\rm emb}w\,2^n).
\tag{H8.7}
\]
The factors count possible initial positions hierarchically. There is no factor obtained by choosing arbitrary initial seeds from the full ball of radius \(L^j\).

### 4. A normalized occupied-cell bound through clean mergers

#### Theorem H8-B: joint cell rarity

For every specified finite family \(\mathcal S\) of scale-\(j\) active-grid cells,

\[
\boxed{
\Pi(\mathcal S\subset\mathscr A_j)
\le
\exp\{-c_1Q\,2^{\lfloor j/w\rfloor}|\mathcal S|\}.
}
\tag{H8.8}
\]

The weak-coupling threshold is independent of \(j\) and of \(\mathcal S\).

**Proof.** A bounded-degree geometric coloring of the current cell grid gives a subfamily \(\mathcal S_*\subset\mathcal S\), with \(|\mathcal S_*|\ge|\mathcal S|/C_{\rm sep}\), whose distinct centers are farther apart than \(3C_{\rm cone}s_j\). All initial witness neighborhoods for different roots in \(\mathcal S_*\) are then disjoint. This coloring can be done on the periodic grid itself, so a modular-coordinate coloring with a possible wraparound collision is unnecessary.

The forest has \(|\mathcal S_*|2^n\) distinct initial bad cubes and at most
\(\exp(C_{\rm emb}w|\mathcal S_*|2^n)\) embeddings. Apply (H8.1) to each specified leaf family and sum:
\[
\Pi(\mathcal S\subset\mathscr A_j)
\le
\exp\{-(c_0Q-C_{\rm emb}w)|\mathcal S_*|2^n\}.
\tag{H8.9}
\]
The source choice \(p_0(g_0)\asymp(\log g_0^{-2})^P\), \(P\ge5r\), and \(R_0\asymp(\log g_0^{-2})^r\) gives \(Q/w\to\infty\). Absorb the embedding cost and the fixed coloring loss. This proves (H8.8).

For each original configuration, all allowed choices of the later positive lift have total conditional probability at most one. Thus the union bound is on original initial events only; it introduces no count of later histories or their posterior denominators. \(\square\)

### 5. Ordinary component size, marked masses, and terminal means

Let \(Y\) be a connected component of \(\mathscr A_j\), let \(m_j(Y)\) count its current \(MR_j\)-cells, and let \(\ell_j(Y)\) be an ordinary current localization size in fixed \(M\)-blocks. The latter is the size convention of CMP109 and CMP119, not a count of \(MR_j\)-blocks. Therefore

\[
\ell_j(Y)\le C_\ell R_j^d m_j(Y).
\tag{H8.10}
\]

A fixed root cell has at most \(A_{\rm an}^{m}\) connected \(m\)-cell animals. The event that such an animal is an actual component implies that all its cells belong to \(\mathscr A_j\), so (H8.8) applies. For every fixed \(\lambda>0\),

\[
\mathbb E_\Pi
\sum_{\substack{Y\ {\rm component\ of}\ \mathscr A_j\\Y\ni x}}
e^{\lambda\ell_j(Y)}
\le
C_\lambda
\exp\{-c_2Q\,2^{\lfloor j/w\rfloor}\}.
\tag{H8.11}
\]

Here one sums
\(\sum_{m\ge1}A_{\rm an}^m
\exp[-c_1Q2^n m+\lambda C_\ell R_j^d m]\).
Since \(R_j\le C_RR_0\) and \(Q/R_0^d\to\infty\) in \(d=4\), the ordinary-size weight is paid before the sum. This is an actual normalized exponential moment for this family of unprocessed components.

Let \(F_x\) be the complete old centered microscopic seed, including its common deterministic physical subtraction, with

\[
|F_x|\le A_x a^{-4}T(a)^s,\qquad T(h)=1+\log(1/h),
\tag{H8.12}
\]

in terminal units \(h\le1\). Define \(C_j(x)=\{x\in\mathscr A_j\}\), with a fixed support collar included in the constants.

#### Theorem H8-C: normalized marked ordinary-size moment

\[
\boxed{
\mathbb E_\Pi
\sum_{\substack{Y\ {\rm component\ of}\ \mathscr A_j\\Y\ni x}}
|F_x|^2e^{\lambda\ell_j(Y)}
\le
C_{\lambda,s}A_x^2h_j^{-8}T(h_j)^{2s}
e^{-c_3Q\,2^{\lfloor j/w\rfloor}}.
}
\tag{H8.13}
\]

**Proof.** Multiply (H8.11) by the seed bound. The conversion from \(a\) to \(h_j\) costs
\[
L^{8j}\left(\frac{T(a)}{T(h_j)}\right)^{2s}
\le
\exp\{D_sj\},\qquad
D_s=8\log L+2s\log(1+\log L).
\tag{H8.14}
\]
Writing \(j<(n+1)w\), the exponent is at most
\(D_sw(n+1)\le C_sw2^n\). Absorb it in a further fixed portion of \(Q2^n\). \(\square\)

For any retained sigma algebra \(\mathscr G_j\), put
\[
M_j(x)=\mathbb E_\Pi[1_{C_j(x)}F_x\mid\mathscr G_j].
\tag{H8.15}
\]
Conditional Jensen and (H8.13) at \(\lambda=0\) give
\[
\boxed{
\|M_j(x)-\mathbb EM_j(x)\|_2
\le C_sA_xh_j^{-4}T(h_j)^s
e^{-\frac12c_3Q\,2^{\lfloor j/w\rfloor}}.
}
\tag{H8.16}
\]
This is the actual selected posterior old-field mean. Its event weight has not been divided out. At the terminal scale \(h_K=\ell_0\), restoring units gives \(C_sA_x\ell_0^{-4}\) times the displayed rare factor. It is a terminal theorem for the clean-initial component contribution, including all its mergers.

### 6. The sharp two-root scale sum for clean initial mergers

If one component of \(\mathscr A_j\) contains roots at distance \(r\), it contains at least \(c(1+r/s_j)\) current cells. The same animal sum, using (H8.8), gives

\[
\Pi(C_j(x,y))
\le
C\exp\{-cQ2^{\lfloor j/w\rfloor}(1+r/s_j)\},
\tag{H8.17}
\]

where \(C_j(x,y)\) requires both root supports to lie in the same such component. This derivation uses the joint cell theorem, whose separated witness forests have disjoint initial leaves; it does not assume probabilistic independence of neighboring occupied cells.

Pay the seed-age conversion exactly as in (H8.14). Using \(s_j\le CMR_0h_j\), retain separate portions of the exponent for rarity and separation:

\[
\mathbb E_\Pi[1_{C_j(x,y)}|F_xF_y|]
\le
C_sA_xA_yh_j^{-8}T(h_j)^{2s}
e^{-cQ}
\exp\!\left[-c\,\frac r{h_jR_0}\right].
\tag{H8.18}
\]

The dyadic scale sum is bounded by
\(C_sr^{-8}R_0^8[T(r)+\log(CR_0)]^{2s}\).
The fixed powers and logarithms of \(R_0\) are absorbed into another portion of the rare reserve. Consequently,

\[
\boxed{
\sum_{j:\,h_j\le1}
\mathbb E_\Pi[1_{C_j(x,y)}|F_xF_y|]
\le
C_sA_xA_y r^{-8}T(r)^{2s}e^{-c_4Q}.
}
\tag{H8.19}
\]

Sector-weighted absolute conditional covariances obey the same bound with a factor at most two. Precisely, for any retained sigma algebra \(\mathscr G\) and \(p_j=\Pi(C_j(x,y)\mid\mathscr G)\), the deterministic seed envelopes give
\[
\mathbb E\!\left[
p_j\left|\operatorname{Cov}(F_x,F_y\mid\mathscr G,C_j(x,y))\right|
\right]
\le
2A_xA_y a^{-8}T(a)^{2s}\Pi(C_j(x,y)).
\]
Apply (H8.17) and the same age conversion and scale sum to this right side. No inequality comparing a product of conditional means with the conditional mean of an absolute product is assumed. This extends H7-G by allowing arbitrary clean initial mergers.

The ordinary-size moment (H8.13) also provides the normalized size reserve required for collapsing and then restoring distances through these particular unprocessed components. It does not supply that reserve for components with later births or failed preparations.

### 7. A different normalized theorem: the actual fresh reset draw

The source reset denominator gives a normalized probability estimate without any assumption on the old component's probability.

Fix an eligible component and an admitted real retained boundary. After the preparatory operations, LFR I (1.73), p.192, identifies the resampled domain \(\Lambda\) as a rectangular region contained in a cube of side \(100M\). Its number of gauge-fixed coordinates is at most \(N_M<\infty\), independent of \(R_k\), the ultraviolet depth, and the total volume.

Use the actual gauge-fixed coordinate \(V'=\exp(ig_kB')\) in LFR II (1.2). The denominator cutoff there is
\(\chi(\{|B'|<M_0g_k^{-1}\varepsilon_k\})\), coming from LFR I (1.101); it is not the separate ordinary or preparatory fluctuation cutoff involving \(\delta_k\) or \(\delta'_k\). After removing the classical boundary action and the common Haar scale factors, which are constant in \(B'\), the actual reset kernel has density

\[
d\nu_{k,e}(B')
=\frac{1}{Z_{k,e}^{\rm fl}}
1_{D_{k,e}}(B')\,J_{k,e}(B')\,
\exp[-\tfrac12Q_{k,e}(B')+L_{k,e}(B')+W_{k,e}(B')]\,
dB'.
\tag{H8.20}
\]

This is only a coordinate expression for the fixed kernel; the cutoff is not changed. The retained data \(e\) include its geometry and chosen axial graph.

LFR II, pp.357–358, gives the following bounds on that actual domain:

- The linear contribution is bounded by an absolute constant, (1.5)–(1.6).
- The higher-order contribution is bounded by \(C g_k^{1-\beta}|\Lambda|\), explicitly in the paragraph following (1.2) on printed p.357, on that denominator's true cutoff domain; it is uniformly bounded for the source weak-coupling choice.
- The quadratic form has the uniform lower bound
  \(Q_{k,e}(B')\ge c_M\|B'\|_2^2\); in four dimensions (1.9) gives \(c_M=\gamma_0/[2d(100M)^5]\).
- The smooth Haar density is bounded above on the small real group chart.
- The remaining fluctuation integral is bounded below by \(\exp(-C_M)\), as stated before (1.10). The classical action and Haar scale factors in (1.10) are the same ones removed in (H8.20).

Thus

\[
0\le\frac{d\nu_{k,e}}{dB'}(B')
\le C_Me^{-c'_M\|B'\|_2^2}
\tag{H8.21}
\]

on its true support, uniformly in the admitted \(e\).

#### Theorem H8-D: normalized reset moments and tails

There are fixed \(t_M>0,C_M<\infty\) such that

\[
\boxed{
\sup_{k,e}\nu_{k,e}
\exp(t_M\|B'\|_2^2)\le C_M.
}
\tag{H8.22}
\]

In particular, for every integer \(m\ge0\) and \(u\ge0\),

\[
\nu_{k,e}(\|B'\|_\infty\ge u)
\le C_Me^{-t_Mu^2},
\qquad
\nu_{k,e}\|B'\|_2^{2m}
\le C_M t_M^{-m}m!.
\tag{H8.23}
\]

**Proof.** Integrate (H8.21) over at most \(N_M\) real coordinates, choosing \(t_M<c'_M\). Use the exponential Markov inequality for the tail, and \(x^m\le m!t_M^{-m}e^{t_Mx}\) for moments. All constants are independent of \(m\); no order-dependent weak-coupling threshold is introduced. \(\square\)

The theorem concerns the new fluctuation in an actual forward reset. It is not a tail theorem for the old unresolved core conditional on its boundary, and it is not a theorem for the earlier preparation-failure selectors.

### 8. Causal marked bounds for fresh reset innovations

Order actual reset draws in any causal order. Let \(\mathscr F_{a-}\) contain the original input and all earlier draws, including the selected geometry for draw \(a\). Let \(B_a\) be an event of its new draw with

\[
\Pi(B_a\mid\mathscr F_{a-})\le q_a,
\tag{H8.24}
\]

where \(q_a=C_Me^{-t_Mu_a^2}\wedge1\) for the threshold event in (H8.23). The threshold and occurrence of the attempted draw may be predictable.

For every nonnegative \(\mathscr F_{a-}\)-measurable mark \(H_a\),

\[
\mathbb E[H_a1_{B_a}]
\le\mathbb E[H_aq_a].
\tag{H8.25}
\]

The original squared seed \(|F_x|^2\) is such a predictable mark. At a fixed deterministic family of causal draw labels with deterministic bounds \(q_a\), iteration gives

\[
\mathbb E[H_0\prod_a1_{B_a}]
\le\mathbb E[H_0]\prod_aq_a.
\tag{H8.26}
\]

This also combines with an initial bad-cube event, since that event is measurable before all reset draws. Hence joint initial events and specified fresh-reset innovations have genuinely normalized product bounds.

For predictable thresholds and selections, the useful general form is the supermartingale

\[
\mathcal E_n
=\prod_{a\le n}
\frac{\exp(t_a1_{B_a})}
{1+q_a(e^{t_a}-1)},
\qquad t_a\ge0\ \text{predictable},
\qquad
\mathbb E\mathcal E_n\le1.
\tag{H8.27}
\]

This follows directly by conditional expectation and admits bounded stopping lines. It does not require independence between geometries or a reciprocal of a carrier posterior.

If continuation of a specified charged ancestry is proved to require such innovations, (H8.26)–(H8.27) can pay its deterministic age and geometry charges. The required event implication must be proved for that ancestry. In particular, an old preparation failure cannot be renamed a new reset innovation merely because both have unnormalized source smallness.

#### 8.1 Exact screening and the limitation for old terminal means

In a successful reset, let \(E\) include the complete retained boundary, history label, and geometry. The new draw has conditional law \(\nu_E\) independent of the old integrated interior, whose conditional law is denoted \(\pi_E\). For an old mark \(F\),

\[
\mathbb E[F\mid E,V_{\rm new}]
=\mathbb E_{\pi_E}F.
\tag{H8.28}
\]

If \(\zeta(V_{\rm new},E)\) is centered under \(\nu_E\), then
\[
\mathbb E[F\zeta\mid E]=0.
\tag{H8.29}
\]

These are exact screening identities for the actual Markov reset. They explain both the gain and its limit: fresh noise does not retain the old interior information, but the old conditional mean is carried by \(E\). The Gaussian estimate for \(V_{\rm new}\) does not bound that function of the boundary and history. A boundary variable with a large old second moment remains a counterexample to any inference that fresh Gaussian tails alone bound the full old terminal mean.

### 9. Fixed unprocessed components: a denominator cancellation that is legitimate

LFR II (1.103)–(1.104), printed pp.391–392, replaces old integral operations by normalized operations and scalar factors \(z_Y=\mathcal T'_k(Y)1\). The source states after (1.104) that \(z_Y\) depends only on the new \(V_k\) restricted to \(Y\), and therefore does not participate in subsequent regular transformations.

On a fixed remaining-\(Y\) carrier, retain those \(V_k|Y\) among the exterior data \(e\). For the next regular fluctuation integration \(A\), write its actual conditional density schematically as
\[
\left(\prod_Yz_Y(e)\right)
e^{-S_{\rm reg}(A;e)+B(A;e)}\,dA.
\tag{H8.30}
\]
The normalized conditional law is exactly
\[
d\mu_e(A)
=
\frac{e^{-S_{\rm reg}(A;e)+B(A;e)}\,dA}
{\int e^{-S_{\rm reg}(A;e)+B(A;e)}\,dA}.
\tag{H8.31}
\]

Here cancellation is valid because the factors are constant in the variables being conditioned. No lower bound for \(z_Y\) is used.

If the complete multiscale boundary potential \(B\) has the needed analytic margin and weighted Hessian bound in the actual current \(A\) chart, the normalized hard-cutoff covariance theorem HC-W applies to (H8.31), including these arbitrary fixed \(Y\). The source's relative/quotient metric must be retained.

Old insertions are not scalar factors of this form. After normalizing an old operation, its source response is still a function of the retained variables and can enter the subsequent conditional mean. Also, (H8.31) does not bound the annealed probability or ordinary size of the \(Y\)-family. H8-C supplies that size control for clean initial components only.

### 10. The comparison theorem still needed for general births and failures

There is a direct normalized local comparison principle. Suppose the actual conditional law on a birth neighborhood has the representation
\[
dp_e
=\frac{e^{V_e}}{q_e(e^{V_e})}\,dq_e,
\qquad
\operatorname{osc}V_e\le b_e,
\tag{H8.32}
\]
with the same support and the same retained exterior, and with \(q_e\) a normalized reference law. Then
\[
\boxed{
p_e(1_B|F|^2)
\le e^{b_e}q_e(1_B|F|^2).
}
\tag{H8.33}
\]
Indeed, the denominator is at least \(e^{\inf V_e}\), so the likelihood ratio is at most \(e^{\operatorname{osc}V_e}\). This is an explicit sufficient anchored partition-ratio estimate. If \(b_e\) is a fixed polynomial in the local geometric radius and the reference bad event costs \(e^{-c p_0^2}\), the source power choices can preserve a rare factor.

#### 10.1 A normalized finite-patch excess-energy theorem

There is a second anchored comparison that requires no small-field uniqueness theorem. Let \(\mathcal E\) contain \(n\) variable links of a finite patch, hold all other links \(e\) fixed, and let \(A_e(U)\) be the Wilson action of all plaquettes involving those variable links. Each variable link belongs to a bounded number of plaquettes. Let \(W_e\) be any real local perturbation of finite oscillation, and define the actual finite-patch conditional measure
\[
dp_e(U)
=Z_e^{-1}e^{-\beta A_e(U)+W_e(U)}
\prod_{\ell\in\mathcal E}dU_\ell,\qquad
A_{\min}(e)=\min_{U\in G^n}A_e(U).
\tag{H8.34}
\]

The minimum exists by compactness; it need not be unique or have a nonsingular Hessian.

#### Theorem H8-E: local normalization preserves excess-energy rarity

For every measurable event \(B\subset G^n\), every bounded mark \(F\), and
\(\Delta_B(e)=\inf_{U\in B}A_e(U)-A_{\min}(e)\),
\[
\boxed{
p_e(1_B|F|^2)
\le
\|1_BF\|_\infty^2
\exp\!\left[
-\beta\Delta_B(e)
+C_G n(1+\log\beta)
+\operatorname{osc}W_e
\right]
}
\tag{H8.35}
\]
for \(\beta\ge1\). The unmarked bound may also be capped at one.

**Proof.** Choose a minimizing configuration \(U_*\). Each plaquette action is uniformly Lipschitz in its four link variables on the compact group. Restrict each variable link to a geodesic ball of radius \(c/\beta\) around the corresponding \(U_*\)-link. On this product neighborhood,
\(A_e(U)\le A_{\min}(e)+C n/\beta\), uniformly in \(e\). Haar volume is at least
\((c_G\beta^{-\dim G})^n\). Therefore
\[
Z_e
\ge
\exp[-\beta A_{\min}(e)-C_Gn(1+\log\beta)+\inf W_e].
\tag{H8.36}
\]
The numerator is at most
\(\|1_BF\|_\infty^2
\exp[-\beta(A_{\min}(e)+\Delta_B(e))+\sup W_e]\),
since normalized product Haar measure has mass one. Divide by the same \(Z_e\). \(\square\)

For a constrained integration domain the same proof works only after supplying a uniform local-volume lower bound near a constrained minimum. One cannot insert an empty or arbitrarily thin good-cutoff sector into (H8.36). For a fixed-dimensional product norm-ball cutoff such a volume certificate is elementary, but the full history-dependent multiscale cutoff is a different object.

The theorem is a genuine normalized local partition-ratio estimate. Its cost is proportional to the number of patch variables and \(\log\beta\), with the same conditional minimum retained in numerator and denominator. If an actual birth event has
\(\beta\Delta_B\ge c p_0^2\), and \(n(1+\log\beta)+\operatorname{osc}W_e=o(p_0^2)\), it gives the desired exponential marked rarity.

#### 10.2 The source makes the boundary obstruction explicit

LFR I, printed p.193, introduces \(\chi_{k,\Lambda}\) in (1.75). It depends only on \(V_k\) outside \(\Lambda\) within \(Z\), and asks whether that exterior has an extension whose minimizing field satisfies the prescribed \(2\varepsilon_k\) regularity. On its complement, the paper shows that a retained exterior plaquette must satisfy a lower bound of the form
\[
|V_k(\partial p')-1|
\ge c(B_3,M)\varepsilon_k,
\qquad p'\subset Z\cap\Lambda^c.
\tag{H8.37}
\]
It excludes these components from the reset class and obtains an unnormalized Wilson-action small factor.

Once that retained exterior is fixed, the event \(1-\chi_{k,\Lambda}=1\) is compulsory: changing the interior variables of \(\Lambda\) cannot make its conditional probability small. A weakly regular minimizing extension may still exist—Proposition 1, (1.77)–(1.78), p.194, applies under a sufficiently small exterior bound—but this does not produce an extension satisfying the stricter selector (1.75).

Thus the missing step is not merely existence of some local minimum. The comparison neighborhood must include the offending boundary variables, and the source small factor must be converted into an excess-energy or likelihood-ratio bound relative to the minimum for the **new, same retained exterior**. If that exterior is again compulsory, its further boundary ancestry must be included and paid. For arbitrarily large or multiscale unprocessed components, the inspected source clauses do not yet supply this anchored surgery with a cost linear in the retained ordinary component budget.

The successful reset reference measure is a new draw and is not automatically the old pre-reset conditional law. The fixed-family cancellation in (H8.31) does not remove the dependence of old source responses on the exterior.

A relative-entropy bound alone is weaker. If \(D(p_e\Vert q_e)\le D_e\), binary data processing gives
\[
p_e(B)
\le
\frac{D_e+\log2}{\log[1/q_e(B)]}.
\tag{H8.38}
\]
For \(q_e(B)\le e^{-cQ}\), this is only \(O((D_e+1)/Q)\). It cannot replace the exponential rarity needed to pay \(L^{8j}\) over windows of length comparable to a power of \(\log g^{-2}\). One needs a stronger local likelihood-ratio estimate, an anchored surgery theorem, or an equivalently normalized source expansion.

The direct original-Wilson chessboard extension also remains limited by the precise obstruction recorded in [Appendix I](observable_appendix_i.md): the actual reset normalizer and minimizing-field dependence can connect both sides of a reflection plane. Positivity and Euclidean covariance do not prove reflection positivity of the resulting law.

### 11. Summary of results and missing scope

| Item | Result proved here | Scope still missing |
|---|---|---|
| Initial components that merge | H8-A/H8-B give a binary-witness proof and normalized joint cell rarity | Later births and preparation failures in the ancestry |
| Unprocessed component size | H8-C proves an ordinary current-\(M\)-block exponential moment with the actual normalized old marked mass | General unprocessed components |
| Two-root clean initial contribution | H8.19 gives the sharp \(r^{-8}T(r)^{2s}\) absolute scale sum | Cross-sector connected terms and other birth mechanisms |
| Terminal old field | H8.16 bounds the actual selected posterior old-field mean | The complete terminal field and its other history contributions |
| Fresh reset tails | H8-D gives uniform normalized Gaussian moments and tails from the actual denominator | Pre-reset old-core distributions |
| Adaptive innovation families | H8.25–H8.27 give marked causal product bounds and a stopped supermartingale | Identification of every relevant source failure with such an innovation |
| Fixed unprocessed exteriors | H8.31 removes only factors truly constant in the next regular integration | Full boundary chart estimates and annealed exterior normalization |
| Anchored local normalization | H8-E proves the finite-patch excess-energy ratio using the same conditional minimum and partition function | The actual later event must have an excess-energy gap and an admitted constrained volume |
| Full normalized H7.39 | H8.33 and H8-E give concrete normalized comparison criteria; (1.75) identifies the boundary that must enter a surgery | Their source-specific construction for all later births, failures, and mixed boundary sectors |

#### Primary sources

- CMP119 (1988), pp.245–246, (1.1), and pp.255–256, (2.5)–(2.7): initial source events and radius comparisons.
- LFR I (1989), p.177, conditions (i), (ii); pp.192–194, (1.73)–(1.78); pp.200–201, (1.99)–(1.100): eligibility, finite reset domain, the explicit retained-boundary failure of (1.75), and the actual normalized reset.
- LFR II (1989), pp.357–358, (1.2), (1.5)–(1.11): fluctuation denominator, lower quadratic bound, and normalized Gaussian domination.
- LFR II, pp.384–387, (1.80)–(1.88): clean \(S\)-evolution, shrinking envelope, clean eligibility horizon, and the connected merging graph. On printed p.384 the single-cell envelope is strictly smaller than \(63MR_n\), with its central current cell containing the original cell. The new witness proof follows occupied cells rather than requiring distinct component parents.
- LFR II, pp.391–392, (1.103)–(1.104): fixed-family normalized operations and dependence of remaining scalar factors only on \(V_k|Y\).

No signed cluster coefficient is interpreted as a probability. No old component mass is replaced by a fresh reset normalizer, and no full-history theorem is asserted from the conditional comparison criterion alone.

---
