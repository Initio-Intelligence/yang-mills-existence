# Local compactness of active-history laws

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

## 1. Result and exact inputs

The extensive active-history estimate has a useful local consequence which does not require a local deletion ratio. On the actual cofinal stopped sequence, the laws of the restrictions of the active large-field geometry to finitely many physical cells and finitely many native ages are tight. Moreover, an ancient **literal active footprint** meeting a fixed window has a uniformly vanishing probability. Compact group coordinates and the identified ordinary free coordinates can be included. A diagonal subsequence therefore defines a probability law of these local restrictions, with consistent restriction maps.

This is a probability-law limit of part of the actual mixed state, rather than a limit only of homogeneous analytic coefficients. It does not supply tightness of the entire connected component touching a window, continuity of the full source operation, a local exponential moment, or a local H02 deletion theorem.

The actual-source inputs are:

1. The stopped sequence and original cubic grids of the positive-endpoint note, PE.12–PE.23. At every fixed physical offset \(s\), the current coupling lies in a compact weak interval. The old physical grid periods have a common cutoff-independent bound.
2. The positive active-history cost and normalized marked pressure estimate H2S.1–H2S.3, H2S.13–H2S.14 in [Survival estimates for the unreplaced history](unreplaced_history.md). All old normalizers, vacuum terms and history weights remain in the positive law.
3. Whole-component persistence through a failed preparation, and enlargement or merger under ordinary growth. A completed operation ends the old internal genealogy. If a second-class \(Y\) remains with its raw \(V_b\) and multiplier \(\tau_b(V_b)\) in LFR II (1.102)–(1.104), it starts a new active lineage of birth \(b\), paid by the actual \(\tau_b\) reserve. This is the original external large-field bookkeeping, not the smaller prepared determining complement.
4. The native volume bound from LFR II p.380. The paragraph preceding the characteristic-function extraction bounds the old vacuum and normalization contributions using
   \[
   |Z_j|_j\le C(MR_j)^d\bigl(d'_j(Z_j)+1\bigr).
   \tag{LC.1}
   \]
   This is a geometric volume bound for the region itself, not an estimate of the rank of its remaining Gaussian integral.
5. Translation covariance under translations preserving the complete block partition. Section 3 constructs one fixed common physical period preserving all source partitions. The spatially averaged statements need no translation assumption.

Here \(d=4\), with \(d\) retained in elementary counting formulas.

### 1.1 Full normalization and current volume

Let \(V_{k,n}\) be the number of unit cells on the current lattice of the \(n\)-th cutoff theory. The pressure input is
\[
\mathbb E_n e^{u\mathcal C_{k,n}}
 \le e^{C_{u,s}V_{k,n}},
 \qquad u>0\ \hbox{fixed}.
\tag{LC.2}
\]
The constant may depend on the fixed physical offset \(s\) and its compact current weak interval, but not on the microscopic cutoff or torus volume.

CMP119 Corollary 3, (2.50), prints a lower bound on the density. To obtain the lower partition bound used here, integrate it on a fixed small product ball of terminal group bonds. On that ball the current characteristic function is one. The regular minimizing field has fine curvature of order \(\eta^2\), so its Wilson action is at most \(C_sV_{k,n}\): the \(\eta^4\) plaquette action cancels the fine plaquette density. The Haar mass of the terminal product ball is at least \(e^{-C_sV_{k,n}}\). Thus the integral is bounded below by \(e^{-C_sV_{k,n}}\). The marked upper bound is H2S's positive chronological estimate.

The volume is the current unit-lattice count. In the all-regular case, the native-layer count in CMP119 (2.45)–(2.49) reduces to \(|\Gamma_k|\); CMP109 (0.30) uses the same current-scale volume. No microscopic point count is substituted for \(V_{k,n}\). No posterior already conditioned to contain a bad component is used in (LC.2).

## 2. Count native cells before assigning physical roots

For \(j\le k\), let \(Z^{\mathrm{act},k}_j\) be the union of the actual grade-\(j\) ancestors of the current unreplaced components, stopping each ancestry at its most recent completed renewal. Completed older archives are omitted. A retained raw multiplier on a second-class \(Y\) belongs to its new active birth and is not omitted merely because its older integral has been completed. Define
\[
\mathcal V_k=\sum_{j\le k}R_j|Z^{\mathrm{act},k}_j|_j ,
\tag{LC.3}
\]
with each volume counted on its own native \(j\)-grid. H2S.2 defines
\[
\mathcal C_k
 =\sum_{j\le k}\sum_{Q\in\mathscr A_j(D_k)}
    M^dR_j^{d+1}\bigl(d'_j(Q)+1\bigr).
\tag{LC.4}
\]
Distinct ancestors at one grade have disjoint interiors. Equation (LC.1) gives
\[
0\le\mathcal V_k\le C_{\mathrm{cov}}\mathcal C_k.
\tag{LC.5}
\]
The added one handles a singleton coarse cube with zero tree length; its chronological payment is H2S.6–H2S.7.

Use half-open unit cells so assignment is unique. For a current cell \(x\), set
\[
v_k(x)=\sum_{j\le k}R_j
 \#\{q:\ q\hbox{ is an occupied native }j\hbox{-cell of }
             Z^{\mathrm{act},k}_j,\ q\subset x\}.
\tag{LC.6}
\]
The elementary grids are nested, hence
\[
\sum_xv_k(x)=\mathcal V_k.
\tag{LC.7}
\]
For a union \(B\) of current cells write \(v_k(B)=\sum_{x\subset B}v_k(x)\). We may sum the same charge over a common-period tile.

This pays the fine-root multiplicity. A current cell contains \(L^{d(k-j)}\) possible native \(j\)-cells, and (LC.6) counts every occupied one before assigning its root. There is no later unweighted sum over those fine roots. The charge does not count signed polymers or repeated representations of one physical region.

## 3. First moments with the actual grid symmetry

Jensen's inequality and (LC.2), (LC.5) give
\[
\mathbb E_n\mathcal V_k
 \le C_{\mathrm{cov}}\mathbb E_n\mathcal C_k
 \le \frac{C_{\mathrm{cov}}C_{u,s}}u V_{k,n}
 =:C_sV_{k,n}.
\tag{LC.8}
\]
Without any invariance assumption, an independent uniform current root \(X_n\) satisfies
\[
\mathbb E_n v_k(X_n)\le C_s.
\tag{LC.9}
\]

### 3.1 A cutoff-independent common physical period

Let the terminal spacing be \(\ell_0\). At age \(a=K'_n-j\), PE.19–PE.21 give
\[
R_j\le C_R[\log(Y_++Da)]^{r_0},
\qquad
\sup_{n,j}L^{j-K'_n}R_j<\infty.
\tag{LC.10}
\]
All variable partition sizes are powers of the same odd \(L\), times the source's fixed compatible divisors. Choose the fixed period
\[
p_*=2L^{H_0}\ell_0
\tag{LC.11}
\]
from PE.21, with those divisors included. It is divisible by every elementary, \(MR_j\) and \(LM_2R_j\) partition used in every prefix. The growing tori are tiled by these \(p_*\)-tiles.

Translation by \(p_*\) relabels each source block, its relative tree, the history geometry, constraints, selectors and variables. Haar measure and the Wilson action are invariant. Every history-dependent normalization moves with its record. This proves covariance of the complete literal positive history law under these translations; individual signed localization coefficients need not separately be covariant.

At offset \(s\), a tile contains
\[
N_s=(p_*/h_s)^d,\qquad h_s=\ell_0L^{-s},
\tag{LC.12}
\]
current cells. This is finite independently of \(n\). Symmetry and (LC.8) yield, for each such tile \(Q\),
\[
\mathbb E_n v_k(Q)\le C_sN_s.
\tag{LC.13}
\]
For any fixed finite union \(B\) of the tiles,
\[
\mathbb E_n v_k(B)\le C_s|B|_k,\qquad
\mathbb P_n(v_k(B)>t)\le C_s|B|_k/t.
\tag{LC.14}
\]
Covering an arbitrary compact window by finitely many tiles gives the same conclusion, with its fixed cover included in the constant.

If a different augmentation chooses noncovariant representatives, retain the spatial-average statement (LC.9), or explicitly average the common grid phase. A phase average preserves the physical Wilson marginal but changes the augmented law.

### 3.2 This is not a local exponential-moment theorem

On \(V\) cells choose a uniform cell \(X\), put \(v(X)=V\), and put zero elsewhere. This translation-invariant example has
\[
\mathcal V=V,\qquad
\mathbb E e^{u\mathcal V}=e^{uV},\qquad
\mathbb E v(x)=1,
\tag{LC.15}
\]
but
\[
\mathbb E e^{tv(x)}
 =1-\frac1V+\frac{e^{tV}}V\longrightarrow\infty
 \quad(t>0).
\tag{LC.16}
\]
Thus an extensive pressure bound does not give a uniform local exponential moment even with exact translation invariance.

## 4. A local age tail for literal active footprints

Actual active ancestry satisfies the physical inclusion
\[
Z^{\mathrm{act},k}_j\subset Z^{\mathrm{act},k}_{j+1},
\qquad j<k.
\tag{LC.17}
\]
Ordinary growth contains the old region; failure keeps its original whole component. At a renewal the old archive is omitted from the current active ancestry, and the retained second-class region is a new birth. Thus (LC.17) concerns only the current unintegrated ancestry after its last renewal. Replacing a failed component by its smaller determining \(Z''\) would invalidate this argument.

For a union \(B\) of current cells let \(E_{k,A}(B)\) be the event that an occupied cell of a literal active ancestor at some grade \(b\le k-A\) is assigned to \(B\) in (LC.6). For a closed-set intersection event, use the one-current-cell enlargement \(B^+\).

Choose an interior physical point \(q\) of the old occupied cell. It lies in the active region at every grade \(b,\ldots,k\) by (LC.17). At every grade its native cell lies in the same current parent cell. Therefore
\[
v_k(B)\ge\sum_{j=b}^kR_j
 \ge\sum_{a=0}^{A}\underline R_s(a)=:r_s(A)
 \quad\hbox{on }E_{k,A}(B),
\tag{LC.18}
\]
where \(\underline R_s(a)\) is a uniform lower bound for the actual rounded radius at age \(a\). Always \(\underline R_s(a)\ge R_{\min}>0\), so
\[
\sup_n\mathbb P_n(E_{k,A}(B))
 \le \frac{C_s|B|_k}{R_{\min}(A+1)}.
\tag{LC.19}
\]
The accepted signed-AF envelope additionally gives
\[
Y_{k-a}\ge c_s+c_{\mathrm{AF}}a,\qquad
R_{k-a}\ge c_R[\log Y_{k-a}]^{r_0},
\tag{LC.20}
\]
with a harmless fixed initial-age adjustment. Summing over \(A/2\le a\le A\) shows, for large \(A\),
\[
r_s(A)\ge c_sA[\log(2+A)]^{r_0},\qquad
\sup_n\mathbb P_n(E_{k,A}(B))
 \le\frac{C_s|B|_k}{A[\log(2+A)]^{r_0}}.
\tag{LC.21}
\]
The weaker (LC.19) suffices for compactness.

No \(L^{dA}\) factor is missing. Every native occupied cell was counted in (LC.6); (LC.18) then uses a deterministic persistent point. Enumerating hypothetical microscopic anchors again would double-count the event.

### 4.1 What the age statement excludes

The event in (LC.19) differs from the event that a current component touching \(B\) has an ancient ancestor somewhere. Its seed can be far away and the component can grow or merge into \(B\) only recently. Its ancient footprint need never have met \(B\).

An extensive cost allows one current component of macroscopic diameter with an old, concentrated seed whose accumulated cost is only of order the total volume. Uniformly translating it keeps its expected local charge bounded, while the age of the whole component can diverge at every point it currently touches. We therefore do not attach an entire remote carrier or its unbounded oldest global birth date as a local mark.

### 4.2 The stronger weighted reserve improves the local conclusion

H2S.35–H2S.39 now supply the fixed-fraction weighted store
\[
w_j=\delta\frac{P_j}{M^dR_j^{d+2}},\qquad
\mathcal W_k=\sum_{j,Q}w_jc_j(Q),\qquad
\log\mathbb E e^{\mathcal W_k}
 \le C(1+\ell_k)V_k.
\tag{LC.27}
\]
Its pressure constant is independent of the growing weights. This specific theorem, rather than an unspecified bound \(C(w_k)\), is used here.

Replace the contribution \(R_j\) in (LC.6) by \(w_jR_j\), obtaining the additive local charge \(v_k^w\). Equation (LC.1) gives
\(\sum_xv_k^w(x)\le C\mathcal W_k\). Jensen and the same common-period symmetry therefore give
\[
\mathbb E v_k^w(B)\le C(1+\ell_k)|B|_k.
\tag{LC.28}
\]
The persistence proof is unchanged. Since
\[
w_jR_j\asymp
\frac{\delta}{M^d}
 \ell_j^{\,t_1},
\qquad t_1=p_0-(d+1)r_0>1,
\]
the retained AF lower envelope gives, for \(A\) beyond a fixed initial range,
\[
\sup_n\mathbb P_n(E_{k,A}(B))
\le
\frac{C(1+\ell_k)|B|_k}
 {A[\log(Y_k+A)]^{t_1}}.
\tag{LC.29}
\]
The constant includes the fixed \(\delta\) and grid divisors.

There is also a direct moment consequence. Let \(A_B\) be the oldest age of a literal active footprint meeting \(B\), and set \(A_B=-1\) when the window has no active cell. The same persistent point gives a pathwise lower bound on \(v_k^w(B)\). With the fixed initial range absorbed,
\[
\mathbb E\!\left[
(A_B+1)\,[\log(2+Y_k+A_B)]^{t_1}
\,\mathbf1_{\{A_B\ge0\}}\right]
\le C_s|B|_k.
\tag{LC.30}
\]
In particular the local oldest literal age is uniformly integrable. This strengthens Theorem LC.1 without changing its scope: it is still not the oldest remote ancestor of an entire current component.

## 5. Retained coordinates

### 5.1 Compact raw group variables

At fixed native depth and in a fixed physical window there are finitely many actual raw group bonds. They take values in a finite product of the compact gauge group. Missing coordinates use a separate absent symbol. This uses group variables themselves, not a logarithm selected across a branch cut.

### 5.2 Identified ordinary free coordinates

H2S.9 retains the actual surviving old precision energies with their reference normalizers unchanged. NR20.1a supplies, on its admitted ordinary native free coordinates,
\[
K_{j,C}\ge\lambda_0I.
\tag{LC.22}
\]
Its actual real-background current and second-order admission is included. Consequently
\[
\mathcal E_{\rm ord}\ge\frac{\lambda_0}{2}
       \sum_{(j,C)}\|a_{j,C}\|^2.
\tag{LC.23}
\]
An ordinary \(A_j\) is carried in \(Z_{j+1}\cap\Omega_{j+1}\). The active-age bound is therefore used with at most one native grade of padding, rather than identifying its index with that of its supporting large-field region.

The positive energy insertion and the same full upper/lower partition comparison give
\[
\mathbb E_n\mathcal E_{\rm ord}\le C_sV_{k,n}.
\tag{LC.24}
\]
Assign each native free coordinate to its bond's common-period tile. From (LC.23), translation covariance, and (LC.24),
\[
\mathbb E_n\!
 \sum_{\substack{\text{ordinary active free coordinates}\\
                 \text{assigned to }B}}
 |a_\ell|^2
 \le C_s|B|_k.
\tag{LC.25}
\]
This makes every finite list tight. Physical-scale conversion factors are bounded on a fixed age interval, but no estimate on arbitrary ancient physical rescalings is claimed.

An actual finite source cutoff is another direct compactness proof. The current regular coordinates can use their literal cutoff or the accepted fixed-fiber C08 bounds. A differently transformed \(R\)-coordinate is included only with its own verified cutoff or coercive energy; the word “Gaussian” alone does not identify it with (LC.22).

## 6. A common local state space

Pass to the subsequence with stabilized rounded labels at each fixed physical offset, as in the endpoint and homogeneous source-probe notes. Retain the labels at thresholds rather than recomputing them from the limiting coupling.

Fix an offset \(s\), a bounded union \(B_m\) of common-period tiles and a native depth \(A\). Retain:

* the occupation of native cells in \(B_m\) at ages \(0,\ldots,A\);
* literal selector and preparation-substep labels attached to those cells or to bonds in a fixed finite stencil enlargement;
* raw group coordinates and the ordinary free coordinates of Section 5;
* finite incidence relations between these cells, replacing arbitrary global component names by the finite equivalence relation they induce.

There are at most
\[
C_{s,m}\sum_{a=0}^{A}L^{da}
\tag{LC.26}
\]
native cells, independently of the microscopic cutoff. Source waiting times and preparation lengths at these finitely many grades are bounded by the fixed-offset compact coupling intervals. The geometry and selector alphabet is finite. The field space is a finite product of compact groups and finite-dimensional Euclidean spaces, each with an absent symbol.

An entire remote component, its unbounded global birth date and completed archives are not added as one local label. They are not controlled by (LC.19). A finite equivalence relation inherited from remote connectivity may be retained as metadata, but its identification with geometric connectedness of the limiting set is not automatic.

Let ages and windows increase through countable exhaustions. The ambient space is the countable product of these coordinates with the natural restrictions. Finite-cutoff configurations use the absent symbol beyond their bare depth. It records local active ancestry, not the existence of forgotten completed archives.

## 7. Tightness and a probability-law limit

### Theorem LC.1

At the actual normalized source scope of Section 1, the local active records at any fixed output offset are tight. For finitely or countably many offsets, the same assertion holds jointly when their finite-cutoff records are retained on the common positive chronological source space. There is a subsequential probability law with consistent finite-window restrictions. Its active geometry is locally of finite native age almost surely.

**Proof.** Fix a window \(B_m\). Given \(\varepsilon>0\), choose \(A\) with the right side of (LC.19), for the required fixed stencil enlargement, at most \(\varepsilon/2\). Outside this exceptional event, no active cell in the window has age greater than \(A\). Only the finite-depth alphabet and coordinates of Section 6 remain.

The group factors are compact. By (LC.25) or the actual finite cutoffs, choose a Euclidean coordinate ball with complementary probability at most \(\varepsilon/2\). The resulting set of finite-depth records is compact. This proves local tightness with the depth retained. In particular an explicit retained \(V_b\) or \(\tau_b(V_b)\) footprint cannot have age larger than this bound: even a completed internal integral restarts, rather than erases, the active clock of its retained second-class raw region.

For countably many windows and offsets use error allowances \(\varepsilon2^{-(m+s+2)}\). The intersection of the corresponding closed coordinate restrictions is compact in the countable product and has probability at least \(1-\varepsilon\). Tightness and diagonal extraction give a probability limit \(\mathbb P_\infty\).

Restriction maps are coordinate projections, hence continuous. Their exact finite-cutoff consistency passes to the limiting marginals. These are not unrelated diagonal limits of separate expectations.

For local finite age, first consider the cylinder event that an occupied active cell occurs at one of the finitely many ages \(A,\ldots,A'\). Pass (LC.19) to the limit in this discrete alphabet, then let \(A'\to\infty\). The same bound holds for an occupied cell at any age at least \(A\). Let \(A\to\infty\), and then take the countable union over windows. Almost surely each window has finite maximal active age. ∎

### 7.1 Common positive space and limits of selectors

At finite cutoff the source can retain a chronological positive history space: partitions of unity retain their labels; changes of free coordinates retain their exact Jacobians and domains; integrated Faddeev–Popov restoration retains its normalized compact orbit variable. The original full partition function normalizes this positive construction, as in H03 and H2S. Joint offsets must be retained on this common source space, not sampled independently from their separate posteriors.

The entire finite-cutoff archive need not be tight. Only the displayed active projections enter Theorem LC.1. If a representation has been chosen only at one output scale, its one-scale conclusion requires no additional joint-space assertion.

The theorem passes bounded continuous functions of the retained local coordinates, and occupation events in the discrete alphabet. A hard selector recomputed from the limiting fields need not agree with its retained label if a boundary has positive limiting mass. The theorem retains the literal limiting label; it does not assume absence of boundary mass.

## 8. Relation to the homogeneous source-probe limit

Refine the same diagonal to retain both the compatible homogeneous source probes/kernels and the local probability law just proved. This adds a probability-bearing mixed component to the earlier unmarked homogeneous limit.

It does not yet make the full mixed \(R\) bank a function of this local probability state. Passing that operation requires uniform control of its dependence on remote carriers, selectors and completed archives, or a stronger jointly retained integration-kernel state with a proved continuity theorem.

| Proved here | Not supplied here |
|---|---|
| Uniform first moment of additive native-cell cost per compatible tile | A uniform local exponential moment or normalized deletion ratio |
| Tail for an ancient literal active footprint meeting a window | Tail for the oldest distant ancestor of every current component touching it |
| Tight local finite-age geometry, raw group coordinates and identified ordinary free coordinates | Entire remote carriers, arbitrary transformed coordinates or completed archives |
| A consistent subsequential probability law of these restrictions | Continuity of the full normalized \(R\) operation or automatic recomputation of hard labels |
| Refinement of the actual stopped positive-endpoint sequence | Prescribed B05 normalization, uniqueness, full continuum observables or Yang–Mills existence |
