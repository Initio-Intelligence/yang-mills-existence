# The complete positive reset posterior and all-order spatial responses — H-03

The purpose of this estimate is to estimate the **actual reset law**. The native source coordinates used below are not identified with independent physical retained links after a minimizing-field pullback. The resulting distinction is stated explicitly in Section 8.

Every probability statement is on the genuine real compact source-free slice, with the auxiliary analytic current J=0, as in LFR II p.380. The analytic native chart is used only for the already admitted uniform majorants; a general complex or analytically deformed pair (U,J) is not assigned a probability law.

### 1. The three kinds of history in the literal source operation

Use Balaban, *Large Field Renormalization II*, CMP122 (1989), printed pp.378–392, especially (1.71)–(1.72), before any signed Mayer expansion. The notation in this note is:

- `Zbar`: the unreplaced region omitted from the eligible R operation;
- `Y_1,...,Y_s`: eligible components for which the final fresh small-field test fails; their geometry remains in the output;
- `C={X_1,...,X_n}`: eligible components for which that final test succeeds; their geometry is summed in the braces of (1.72).

The internal state `eta_D` of a completed component D includes **all** old variables, old restricted domain sequences, surviving older T operations, graph choices and gauge-fixing variables integrated by (1.71). It does not mean only the final B fluctuation. Printed p.378 defines the same T-prime operation for a component of either the X or the Y class.

#### The exact marked meaning of the successful-component Haar restoration

Printed p.378 calls the removal of the fresh axial delta functions an integrated equivalence, not equality of the prior gauge-fixed densities. The following argument specifies the positive marked coupling used here.

At a fixed complete reference descriptor gamma, the literal R quotient in LFR I (1.100) has joint density

\[
 k_\gamma(u'\mid v_\gamma)\,
       \rho_\gamma(u,v_\gamma)\,du\,du'\,dv_\gamma,
 \qquad
 k_\gamma=h_\gamma/H_\gamma.
 \tag{HS20.0a}
\]

Here u' is the **fresh** current field on Lambda_gamma, u contains the old integrated field on that domain and every earlier hidden variable, and v_gamma is the retained exterior. A transported old marked numerator multiplies this density by F(u,v_gamma). It is independent of u'. This is the actual fixed-reference identity MG19.1, before replacing it by a refactorization of the effective action.

LFR I p.201 specifies that G_gamma is an axial gauge graph in Lambda_gamma and that the reference denominator integrates precisely the fresh variables on Lambda_gamma. Take real gauge transformations supported on that domain and fixed at its exterior boundary. They leave v_gamma unchanged. The constrained reference minimizing orbit is gauge covariant under these transformations: its determining data transform at their endpoints, the Wilson action is invariant, and the minimizing orbit is the unique orbit supplied by the source variational construction. Thus the localized Wilson factor in h_gamma is invariant along these fresh gauge orbits. No transformation of an old raw field is needed.

On the successful sector, LFR II p.378 proves that the extra fresh cutoff chi(Lambda_gamma) equals one. The exterior cutoff chi_(k,Lambda) is already fixed by v_gamma, and the remaining successful small-field factors are gauge invariant. Therefore the source Faddeev–Popov restoration is the following positive operation: draw the normalized compact gauge-orbit variable and apply it only to u', leaving gamma,u,v_gamma fixed. Haar invariance and the tree gauge identity give the restored reference density. Since every old mark F(u,v_gamma) is fixed during this operation, the same identity holds with **any** old marked numerator and coefficientwise for every full finite jet. Old archived selectors are untouched.

This is not an assertion of pointwise equality between the old gauge-fixed density and the restored one. It is the explicit positive coupling realizing the source's integrated equivalence. If an analysis coordinate is subsequently changed, its old mark is pulled back through that exact component coordinate change. It must not be replaced by an unchanged function of a freshly inserted coarse plaquette. The extra compact gauge variable is component-local; conditional on the source component coordinates its old preimage is a local lift. It introduces no cross-component factor into the source action.

The lemma concerns the **full** transported jet. A prior artificial decomposition into separate fresh-field-dependent records may require recombination or the corresponding orbit averages before this operation; those separate records are not individually declared invariant. This restriction prevents a hidden assumption about the stronger M-03 current norm.

At this stage the new field and the residual output data are common to the successful-component sum. Denote them by v. More precisely, v includes the actual new background U_k, the new current field V_k where it occurs explicitly, the unreplaced Zbar history data, and the Y geometry. Internal eta_Y variables are **not** included in v for the full posterior below.

The exact common-background statement is LFR II (1.33)–(1.35), printed p.365: the new determining set keeps the old data outside the eligible Z region and uses the current k-grid throughout Z. Its new raw current field there is V'_k V_Lambda. Thus the same complete new V_k and unreplaced exterior define U_k, independently of the internal component histories. The classification on p.378 combines the successful components' final small-field factors into the common new small-field factor. Varying C in (1.72) therefore does not vary v. This is a statement about the exact source representation, not a claim that the old and fresh integration windows were the same before the R operation.

For a successful component X write its real positive unnormalized operation as

\[
 M_X(v,d\eta_X)=T'_k(X;v)(d\eta_X),\qquad
 m_X(v)=M_X(v,1).
 \tag{HS20.1}
\]

All reference ratios, vacuum constants and old normalization factors in (1.71) stay in M_X. Its self activity V(X-tilde) is included there, using exactly the component and fixed-collar convention of (1.71). A carrier touching more than one source component is a cross activity; it is not reclassified as an independent self term by enlarging two collars until they meet. The p.379 localization of every expression in (1.71) is the component-locality statement used below.

The residual Y base needs additional care. The factors written outside T-prime(Y_i) in (1.72), including chi_(k,Lambda_i), chi_i and the fresh axial delta on G_i, can depend on the internal descriptor which determines Lambda_i and G_i. They are **not** all v-only constants and may not be dropped. Put every such positive component-local factor into the full residual base \(\mathcal B_i(v,d\eta_{Y_i})\). Only factors genuinely independent of the internal state are canceled as common factors.

The gauge deltas in this assertion are positive coarea/gauge-slice measures, not functions evaluated at a point. A precise common version is obtained componentwise as follows. At a fixed cutoff there are finitely many graph/domain descriptors in Y_i. For each descriptor, first fill the current shell Y_i minus Lambda by normalized Haar measure, and then use its conditional fresh gauge-slice reference on Lambda. LFR I Proposition 1, p.194, (1.77)–(1.78), identifies V_Lambda as a function of V_k restricted to Z intersect Lambda-complement, independent of the hidden continuous old variables; its axial representative is fixed at p.197, (1.83). Thus each descriptor supplies one well-defined positive measure on the full Y_i current variables, even though its axial stratum varies with the shell values. A finite mixture of these measures with strictly positive coefficients is a common dominating reference. This mixes the measures after including their shells; it does not incorrectly mix pointwise slices at one frozen full current field. Use the Radon–Nikodym density of each descriptor's measure with respect to that reference, and multiply it into the corresponding old positive component measure. Include the remaining descriptor-dependent cutoffs there as well. Different Y_i have disjoint source component domains; conditioning on their exterior gives the product of these local references by the p.201 factorization. Local collars are included in the fixed exterior or component domain according to the source convention.

This constructs \(\mathcal B_i(v,\cdot)\) by positive disintegration for almost every v under the actual output law. Any soft self factor depending on the common U_k is part of that component base. The local reference mixture is the same for every successful family C. Its normalization depends only on v and the fixed Y geometry, so it cancels from the conditional law. No bound on a descriptor count, an inverse Radon–Nikodym density, or a residual component mass is used below.

The remaining interaction is

\[
 H_C(v,\eta_Y,\eta_C)
   =\sum_A V_C(A;v,\eta_Y,\eta_C),
 \tag{HS20.2}
\]

where the sum excludes those self activities. The carrier convention is exactly the convention of (1.68)–(1.72).

Normalize only these **full** fixed Y bases:

\[
 b_i(v)=\mathcal B_i(v,1)>0,\qquad
 \nu_i=\mathcal B_i/b_i.
 \tag{HS20.3}
\]

On active positive-mass fibers, the full conditional reset posterior is

\[
 \boxed{
 \pi_v(dC,d\eta_Y,d\eta_C)
  =\mathcal Z_v^{-1}\,\mathbf1_{\{C\ {\rm admissible}\}}
      e^{H_C(v,\eta_Y,\eta_C)}
       \prod_{i=1}^s\nu_i(d\eta_{Y_i})
       \prod_{X\in C}M_X(v,d\eta_X).
 }
 \tag{HS20.4}
\]

The products of fixed masses b_i and genuinely outer v-dependent factors cancel from this conditional law. The successful-component masses **do not cancel individually**. All conditional normalizers in (HS20.4) are retained. Zero-mass candidate X species have no contribution and can be omitted. Positive-mass active fibers suffice; null disintegration fibers have no effect on the marked integrals.

Equation (HS20.4) follows by disintegrating the positive integrand of (1.72). It is not a probability assigned to a signed polymer activity. The source's statement on p.379 that the internal history sums act also on the cross exponential is precisely why H_C remains inside this posterior.

### 2. The actual component family has a common local coordinate representation

#### Lemma HS20.1 — deletion and gluing of completed components

For fixed v as above, the successful-component family in (1.72) contains C=empty and is closed under deleting any subset of its whole components. The remaining component measures and coordinates are unchanged. The only compatibility condition between separate successful components is their source geometric compatibility with one another and the fixed outside components; it is independent of their internal eta states.

**Source-level proof.** LFR I p.201, before (1.100), first separates the sum over the outer component domains from the remaining sums. It then explicitly factorizes those remaining sums and integrations in the component domains. Their local indices are the restricted sequences `(Omega_j^c intersect D, Z_j intersect D)` and the local graph choices. CMP119 (2.19)–(2.22), printed p.258, gives the corresponding component factorization of older positive T operations. These are factorization statements about the whole operations, including their cutoffs and delta constraints.

Here is why deletion preserves the actual index family, rather than only a formal product. Every earlier large-field region inside a given final component stays in that component: the nested sequence in CMP119 (2.1)–(2.3) places the older holes in the later large-field regions. The preparatory sequence in LFR I (1.10)–(1.12) has the same property. Delete all old holes and all old large-field labels belonging to one final X. This removes whole old-region components or whole sets of their descendant cubes; it does not cut through a surviving grid cube. Every remaining region is still a union of cubes in its original admitted partition. The nesting relations, buffer inequalities and rectangle conditions for the remaining components are unchanged. Filling the removed holes cannot create a new small gap between two remaining holes.

The forward construction gives the same conclusion. The cover-and-padding operation S in LFR II pp.384–385 distributes over the union of the ancestor cubes, as used explicitly in (1.81). A merger or a rectangular completion is performed within one connected descendant component. Ancestors of a deleted final component do not participate in any other final component's mergers; otherwise those components would already be connected. Removing that genealogy therefore leaves every other component's geometric operations unchanged. The component eligibility tests on LFR I p.177 concern its own size and its own preceding history. They do not introduce a global count or a condition on a disjoint component's state.

Conversely, the component-local histories appearing in the factorized sum can be combined whenever their final domains have the source geometric compatibility. All their earlier regions and local characteristic functions remain in the assigned components. The geometric exclusion is imposed by the outer sum; state-dependent cutoffs remain within each local T-prime measure. The only remaining coupling in (1.72) is the displayed exponential of V activities. In particular there is no additional hard cutoff involving eta_X and eta_Y outside those measures.

The operation T-prime(D) itself is unchanged when another component is deleted. Its formula (1.71) uses the local history, the local graphs and the common new field v. The residual component factors and dominating reference just specified are local to their fixed Y_i and unchanged as well. The p.379 localization statement and the omission of self activities from the cross exponential fix precisely this convention. The empty family is the displayed n=0 term in (1.72); it has no successful-component factor. Its cross interaction can still depend on the fixed Y states and is not set to zero. This proves the assertions. \(\square\)

This lemma does not say that all internal histories of a **selected** component sum to one. That assertion would be false. Deletion compares different terms in the successful-component sum, keeping the exact positive masses.

#### Lemma HS20.2 — a common carrier family and local differences

Index the cross interactions by all finite current localization domains A, using zero for a domain not occurring in the particular component family or history. For two admissible component configurations which agree on every completed component meeting A and on the common v restricted to A, their A activity is identical. Consequently a change of a component D changes only activities whose full source carriers meet D (with the fixed source collar included).

**Proof.** The localization is constructed before the final resummation. LFR II pp.373–374, (1.61)–(1.64), enlarges each carrier to include every component it intersects and localizes the remaining background dependences. Its final Y_4 expression uses only the new field and the remaining old variables in Y_4. On p.377 the terms are summed by this final localization domain; the self terms are assigned to their own component operation. Printed p.379 adds the explicit history statement: V(A) depends on the old sequences restricted to the completed components contained in A.

Thus both a primitive localization term and its admissibility test are the same when those local component data are the same. A component outside A cannot change which primitive terms are summed into A. Zero-padding the ambient family of A domains therefore gives the asserted common function, rather than comparing unrelated choices of a scalar decomposition. The subsequent subtraction of the reconstructed new action on p.377 uses the same new field v and is local on the same domain, so it preserves this identity.

Deletion can create A activities which run through part of the removed component, because that region is now ordinary exterior. Such A meets that component and is included in the affected set. It is not claimed that the A index families are otherwise literally equal. The common-family statement only identifies terms whose full carriers miss the changed region. \(\square\)

The full carrier here includes the source collar, graph/data footprint and any old component which the localization completes. It is not the fixed small continuous integration core of the corresponding estimate.

### 3. Uniform one- and two-component interaction budgets

Use current M-cube units and write R=R_k. Every eligible completed component has diameter at most D_R=C_d R and at most C_d R^d M-cubes, by LFR I p.177. The constants may include the fixed source collars. Choose one anchor z_D in each component and put

\[
 L_R=1+D_R.
 \tag{HS20.5}
\]

The final nonself source bound is

\[
 |V_C(A)|\le \alpha_k e^{-\kappa_a d_{k,Z_C}(A)},
 \qquad \alpha_k\le C e^{-cR},
 \tag{HS20.6}
\]

uniformly in the states still integrated. The first part is LFR II (1.68); the fixed decay reserve and the completed-carrier extraction in CR.15/HR18.26 give the second part under the admitted source parameter choices. Here Z_C is the union of the completed eligible components involved in the literal operation, not Zbar or an arbitrary collection of older tags.

For a carrier meeting an eligible component, the source tree count HL.G3 gives at most C(1+R)^d A_d^(n+1) domains with n<=d_(k,Z_C)(A)<n+1. A carrier rooted at a specified exterior cube has the same proof without the component root-choice factor: its tree already meets that cube. These bounds remain valid for the carriers newly appearing after a deletion. They are rooted in a cube of the deleted component, which has become exterior.

It follows that, for some fixed integer b, all of the following are bounded by

\[
 \lambda_R=C(1+R)^b\alpha_k:
 \tag{HS20.7}
\]

- the cross-action change upon inserting one compatible X;
- the state-dependent part of the conditional interaction of one fixed Y;
- the sum of the absolute affected activities when deleting a component.

For later use, let J_(DE) bound the oscillation in the D-conditional interaction caused by changing E, after discarding terms independent of D. If either change toggles a successful species, take the relevant four-configuration difference. Lemma HS20.2 cancels every term whose carrier misses D or E. Summing the remaining source bounds gives

Here independence of an X coordinate includes its empty/present state. A term constant in the internal present-state variable eta_X, but different from its absent-state value, is **not** discarded: it changes the presence activity and remains in the full four-configuration difference.

\[
 J_{DE}\le C(1+R)^b\alpha_k
             e^{-c_1|z_D-z_E|/L_R}.
 \tag{HS20.8}
\]

To justify the distance factor, the original source-tree enclosure HL.G4 puts a carrier of relative length n meeting D in the n+C_d R neighborhood of D. A carrier also meeting E must therefore have n at least their separation minus C_d R. Reserve a fixed part of the source exponential for this constraint and sum the remainder with the tree-count entropy. Weakening the resulting rate to c_1/L_R absorbs the additive C_d R with a fixed constant. No component interior is declared to have zero physical diameter.

The same argument supplies spatial row sums. There are at most C(1+r)^d fixed disjoint Y anchors in a radius-r region in M-cube units. The number of candidate successful component shapes per anchor is bounded by

\[
 N_R\le e^{C(1+R)^d}.
 \tag{HS20.9}
\]

Indeed an eligible component is contained in a cube of side C R; counting all subsets of that cube is an upper bound on the allowed shapes. Internal history labels are already integrated in M_X and are **not** counted again in N_R.

The source unnormalized estimate (1.89), with the common native-domain reserve in (1.73), gives after reducing the coupling ceiling

\[
 m_X(v)\le e^{-P_k},\qquad
 P_k=p_0(g_k),\qquad P_k/(1+R_k)^d\longrightarrow\infty.
 \tag{HS20.10}
\]

These are uniform in the remaining source-admitted history data. No corresponding lower bound is needed for m_X or m_Y.

### 4. Coordinate representation of the full posterior

Let the coordinate set contain one coordinate for each fixed Y_i and one coordinate for each candidate successful X. A Y coordinate has state space eta_(Y_i) and base law nu_i. An X coordinate has state space `{0} disjoint-union eta_X`, where 0 means absent. Its unnormalized base measure is

\[
 \delta_0+M_X(v,d\eta_X).
 \tag{HS20.11}
\]

The coordinate index set is finite at every cutoff, even though its number of possible X geometries can be large and its component state spaces need not be finite. The allowed occupancy configurations are exactly the source geometric compatible families. The proof uses only admissible outside configurations and the deletion paths below. It does not assume any arbitrary extension of the source potentials to mutually incompatible padded states. No signed activity enters this coordinate law.

For a compatible outside family C not containing X, the exact X conditional is

\[
 \gamma_X^C(d\zeta)
 =\frac{\delta_0(d\zeta)+
       e^{H_{C\cup\{X\}}-H_C}
          M_X(v,d\eta_X)}
       {1+M_X(v,e^{H_{C\cup\{X\}}-H_C})}.
 \tag{HS20.12}
\]

If X is geometrically incompatible with an occupied outside component, its conditional is delta_0. Thus

\[
 \gamma_X^C(X\ {\rm present})\le e^{\lambda_R}m_X(v).
 \tag{HS20.13}
\]

The empty state in (HS20.12) has weight exactly one after dividing by the actual outside density. It is not supplied by an artificial reference denominator. The Y conditional is its fixed base nu_i tilted by the interactions which depend on eta_(Y_i); its state-dependent exponent has oscillation at most a fixed multiple of lambda_R.

#### Admissible paths for single-coordinate comparison

Two allowed outside configurations can be connected by deleting components present only in the first, changing common components' internal states, and adding components present only in the second. Lemma HS20.1 makes all intermediate occupancy families admissible. An internal-state change leaves geometric compatibility unchanged. Thus the usual telescoping comparison of conditional kernels is legitimate on this hard-core family. It does not require passing through a forbidden overlap configuration, and the proof below does not use the arbitrary values of a padded off-support kernel.

### 5. Weighted influence estimate

For two distinct reset coordinates i,j let c_(ij) be an upper bound on the total-variation change of the i conditional when an admissible outside state is changed only at j. These coefficients are bounded only on the actual admissible pairs; an off-support product-space extension is unnecessary.

The exact conditional formulas and (HS20.7)–(HS20.8) give

\[
\begin{array}{ll}
 c_{ij}\le C J_{ij},
      &i\text{ a fixed }Y\text{ coordinate},\\[2mm]
 c_{ij}\le C m_i J_{ij},
      &i\text{ an }X\text{ coordinate and both occupancies are allowed},\\[2mm]
 c_{ij}\le C m_i,
      &i,j\text{ incompatible }X\text{ geometries}.
\end{array}
\tag{HS20.14}
\]

In the last line a change at j switches the i law between a delta at the empty state and a law with presence probability at most (HS20.13). Such incompatible geometries have anchors separated by at most C D_R. Candidate X geometries incompatible with a fixed Y or Zbar geometry have already been excluded from the candidate set.

For the first line, the two positive Y conditionals have the same arbitrary base nu_i and a change of the state-dependent logarithm bounded by J_(ij), after removing its additive constant. Their normalized densities differ in total variation by at most exp(C J_(ij))-1<=C J_(ij). This estimate is independent of b_i. For the second line compare the two numerator measures in (HS20.12). Their absent part is identical, their denominator is at least one, and
\[
 M_i|e^{D_i}-e^{\widetilde D_i}|
       \le C m_i\|D_i-\widetilde D_i\|_\infty .
\]
The two normalization errors have the same bound. This proves (HS20.14), including the full conditional normalizers.

Define fixed weights at the chosen v by

\[
 a_i(v)=
 \begin{cases}
 1,&i=Y_i,\\
 \sqrt{m_X(v)},&i=X.
 \end{cases}
\tag{HS20.15}
\]

They are positive after the zero-mass species have been removed. They may depend on v; no derivative of these weights is used. Choose one fixed theta>0 smaller than the spatial reserve in (HS20.8). Then

\[
 \sup_i\frac1{a_i}
       \sum_j c_{ij}a_j
            e^{\theta|z_i-z_j|/L_R}
 \le \varepsilon_R,
\qquad
 \varepsilon_R\le
 C(1+R)^{b_1}\alpha_k+
 C(1+R)^{b_1}e^{-P_k/2+C(1+R)^d}.
\tag{HS20.16}
\]

Here b_1 is fixed. In particular a single sufficiently small common coupling ceiling makes epsilon_R<=1/4 at every admitted scale.

**Proof.** For Y-to-Y rows sum (HS20.8) over the disjoint fixed Y anchors; the spatial lattice row sum costs at most C L_R^d. For Y-to-X rows the additional factor sqrt(m_X) pays the candidate-shape multiplicity (HS20.9). For X-to-Y rows division by a_X changes the factor m_X in (HS20.14) to sqrt(m_X). For X-to-X rows the factor is sqrt(m_X)sqrt(m_(X')), including the hard geometric exclusion. Its finite interaction radius costs at most C(1+R)^d; the remaining exponential tail has the same lattice row sum. These are bounded by the two terms on the right. The strict source separation P_k>>R_k^d and alpha_k<=C exp(-cR_k) pay every fixed polynomial and shape factor. No count of the old internal history depth enters: those states are inside the already estimated positive component measures. \(\square\)

The square-root choice is useful even though this source has geometry-only compatibility. It makes both directions of a rare X versus an ordinary Y influence small. No inverse component mass occurs in the final row bound.

### 6. A spatial cut coupling for the actual posterior

For a set I of reset coordinates define its reset-variable support and its weight by

\[
 S(I)=\bigcup_{i\in I}D_i,\qquad
 n_v(I)=\sum_{i\in I}a_i(v),
\tag{HS20.17}
\]

where D_i is the **full** source component footprint, with its fixed collar. A coordinate representing an old history or graph has that whole component footprint. It is not assigned only the location of one stored variable. For a candidate X coordinate the absent state and the present state are parts of the same coordinate.

#### Theorem HS20.3 — true-marginal cut coupling

Let I,J be two finite sets of reset coordinates. Under (HS20.16), the actual joint marginal of (eta_I,eta_J) under pi_v and the product of its two **actual** marginals admit a coupling with disagreement probability bounded by

\[
 \epsilon_{I,J}(v)
 \le \min\left\{1,\,
      C\,n_v(I)\,
       \exp\!\left[-\frac{\theta\,
          {\rm dist}(S(I),S(J))}{L_R}\right]\right\}.
\tag{HS20.18}
\]

The same assertion with a harmless additional constant covers overlapping coordinate sets. Constants are uniform in the remaining admitted history and total volume. The theorem concerns the full posterior (HS20.4), not a conditional law selected on the presence of a rare X.

**Proof.** We give a finite-coordinate coupling argument. Condition on the J coordinates. For two admissible boundary values beta,beta-prime, use their respective Gibbs conditionals on the complement of J. Couple single-coordinate heat-bath updates by maximal coupling, choosing a coordinate uniformly for each update. Each update preserves the two required conditional marginals.

For two allowed outside configurations the deletion path in Section 4 changes each differing coordinate once and stays admissible. Thus their conditional total-variation difference at i is at most
\[
 \sum_{j}c_{ij}\mathbf1_{\{\eta_j\ne\eta'_j\}}.
\tag{HS20.19}
\]
Write F for the complement of J and N for its finite number of coordinates. Start with any coupling of the two actual conditional marginals, for example their independent product. After averaging the boundary choices below, let delta_i(t) be the disagreement probability at time t and let b_j be the fixed boundary disagreement probability. The exact numerical recursion is
\[
 \delta_i(t+1)\le
 (1-N^{-1})\delta_i(t)+N^{-1}
 \left(\sum_{j\in F}c_{ij}\delta_j(t)
                 +\sum_{j\in J}c_{ij}b_j\right).
\tag{HS20.19a}
\]
Conjugating the F matrix by the positive diagonal a makes its row norm at most epsilon_R<1. Hence the powers of
\(T_N=(1-N^{-1})I+N^{-1}C_{FF}\)
decay in that weighted norm. Iterating (HS20.19a) gives
\[
 \delta_F(t)\le T_N^t\delta_F(0)
        +N^{-1}\sum_{\ell=0}^{t-1}T_N^\ell C_{FJ}b_J .
\tag{HS20.19b}
\]
Its limit upper bound is \((I-C_{FF})^{-1}C_{FJ}b_J\). This is a limit of finite numerical inequalities, not a construction of a stationary coupling or an infinite product. At every time the observed first-copy/boundary marginal and the observed second-copy/boundary marginal have the same required distributions, so their fixed total-variation distance is bounded by the error of that time's coupling. Taking the infimum of these bounds proves the limit estimate. Maximal coupling of those two fixed observed laws then realizes it. A very small positive minimum a_X can change the time needed for the first term to decay, but does not appear in the final bound. When F is empty only the boundary estimates are used.

Now draw beta and beta-prime independently from the **true pi_v marginal** on J and average these inequalities. If j is a Y coordinate, its boundary disagreement probability is at most one. If j is an X coordinate, the two copies agree at their empty state unless at least one is present, so by (HS20.13)
\[
 {\mathbb P}(\beta_j\ne\beta'_j)
 \le2\pi_v(X_j\ {\rm present})
 \le C m_j\le C a_j .
\tag{HS20.20}
\]
The identical bound supplies an initial a-weighted bound for every free X coordinate in the two conditional marginals. This is the step that prevents a hidden inverse rare-event mass.

Inserting (HS20.20) into the resolvent and using the spatially weighted row bound gives, for i outside J,
\[
 p_i\le C a_i
        \frac{\varepsilon_R}{1-\varepsilon_R}
       e^{-\theta\,{\rm dist}(z_i,\{z_j:j\in J\})/L_R}.
\tag{HS20.21}
\]
For i in J use (HS20.20) directly. The triangle inequality for anchor distances pays the exponential along every path in the matrix series. Summing the observed disagreement probabilities over i in I proves the displayed bound, because all anchors lie in their declared supports.

Finally, let the first observed copy be sampled conditionally on beta and the second conditionally on beta-prime. After beta-prime is averaged, the second observed copy has the true pi_v I-marginal and is independent of beta. Hence the comparison is between the true joint law and the product of its true marginals. A union bound on the observed coordinates, or maximal coupling of the resulting finite observed marginals, gives (HS20.18). This argument never replaces a rare-sector conditional moment by an unconditional moment. \(\square\)

If the inputs are specified by physical locations rather than full component-coordinate footprints, their reset-variable supports must first be enlarged to contain every completed component on which they actually depend. The enlargement has radius at most C M R_k h for a mark which depends only on components meeting its initial local set. This is the explicit reset radius; it is not a bound on a nonlocal minimizing-field pullback.

### 7. All conditional cumulants and the complete finite reset jet

Let F_1,...,F_r be real or complex functions under the actual posterior pi_v. Suppose F_l depends on the reset coordinates in I_l, with v fixed. Write

\[
 S_l=S(I_l),\qquad
 \mathcal S_l(v)=\sqrt{\,1+n_v(I_l)\,}.
\tag{HS20.22}
\]

Let T(S_1,...,S_r) be the minimum spanning-tree weight on these r support sets, with edge weight dist(S_i,S_j). This definition is valid even when sets overlap; the edge weights need not themselves define a metric.

#### Theorem HS20.4 — spatial cumulants of the full reset law

For r>=2 and F_l in L^(2r)(pi_v),

\[
 \boxed{
 |\kappa_{\pi_v}(F_1,\ldots,F_r)|
 \le C^r r!\,
      \prod_{\ell=1}^r
       \left[\mathcal S_\ell(v)
                   \|F_\ell\|_{L^{2r}(\pi_v)}\right]\,
       \exp\!\left[
        -\frac{c\,T(S_1,\ldots,S_r)}
                    {(r-1)L_R}\right].
 }
\tag{HS20.23}
\]

Every input norm is in the **same actual full posterior**. The bound is uniform in the remaining admitted history. It includes descriptor-mean fluctuations as well as old fluctuations inside a component.

**Proof.** Choose a minimum spanning tree on the support sets and delete its longest edge. The resulting nontrivial cut A union B has all cross distances at least the length of that edge; otherwise replacing the edge would reduce the tree weight. Its length is at least T/(r-1). Apply Theorem HS20.3 to the unions of the coordinate sets on the two sides.

Couple the resulting true joint law with the product across the cut. Denote its failure probability by epsilon. A moment of a block K of labels differs between the two laws by at most
\[
 2\epsilon^{1/2}
       \prod_{\ell\in K}\|F_\ell\|_{L^{2r}(\pi_v)}.
\tag{HS20.24}
\]
Indeed the products agree on the coupling success event; on its complement use Hölder with the indicator in L^2 and each of the at most r input factors in L^(2r). The product-across-the-cut law has the same individual input marginals, so the same norms bound both terms. A block contained on one side has no difference.

The mixed cumulant of all r variables under the product law is zero. In the cumulant partition formula, telescope each product of block moments. This costs at most the number of blocks. Consequently its coefficient sum is bounded by
\[
 2\epsilon^{1/2}\sum_{\pi\in\Pi_r}|\pi|!\,
           \prod_{\ell=1}^r\|F_\ell\|_{2r}
 \le 2^r r!\epsilon^{1/2}
           \prod_{\ell=1}^r\|F_\ell\|_{2r}.
\tag{HS20.25}
\]
The last inequality follows by encoding ordered set partitions by a permutation and cuts. The support factor in the cut bound satisfies
1+sum_(l in A) n_v(I_l)<=product_l(1+n_v(I_l)); using (HS20.18) and taking its square root proves (HS20.23), with a fixed changed rate. \(\square\)

The decay rate has the explicit r-1 denominator. No stronger tree-product or order-independent rate is claimed. At one component's own scale the theorem permits unrestricted internal dependence; its physical component diameter supplies the reset radius.

#### Full-law moments without conditioning on a rare event

Let mu(dv,deta)=nu(dv) pi_v(deta) be the actual positive source-free joint law, and suppose the support factors in (HS20.22) have their indicated uniform bounds. If supports or candidate species depend on v, choose a deterministic lower bound
\(T_*\le T(S_1(v),\ldots,S_r(v))\)
on the active fibers. At one fixed scale L_R is common; otherwise its uniform upper bound is used. Applying (HS20.23) with the larger input exponents 2rp and then conditional Hölder gives, for p>=1,

\[
 \|\kappa_{\pi_v}(F_1,\ldots,F_r)\|_{L^p(\nu)}
 \le C^r r!\,
   \left(\prod_\ell\sup_v\mathcal S_\ell(v)\right)
     e^{-cT_*/((r-1)L_R)}
      \prod_{\ell=1}^r
           \|F_\ell\|_{L^{2rp}(\mu)} .
\tag{HS20.26}
\]

Without such a uniform lower bound, the spatial factor stays inside the Lp(nu) estimate; it is not removed from a v-dependent integrand. For fixed initial physical supports and their uniform component-radius enlargements, the corresponding deterministic separation supplies T_* whenever those enlarged supports are separated.

To see the measure step explicitly, bound each conditional factor by
(pi_v |F_l|^(2rp))^(1/(2rp)), raise their product to p, apply Hölder over v, and use concavity of the remaining square root. No conditional mass is divided out in this estimateage.

For M-03's averaged grade seminorm, input source grades d_l summing to m give, up to the same explicit support and spatial factors,
\[
 \mathfrak m_m\!
     \left(\kappa_{\pi_v}(F_1,\ldots,F_r);\nu\right)
 \le C^m\,m!\,r!\,
           \prod_{\ell=1}^r
                       \mathfrak m_{d_\ell}(F_\ell;\mu).
\tag{HS20.27}
\]
This follows by substituting the input grade bounds into (HS20.26), using
product_l d_l^(d_l)<=m^m and r^m<=m^m<=e^m m!. The h^(4m) factors multiply correctly because this is an R reset at one current scale. This is only the averaged moment part of M-03, not its pointwise regulator, ambient-shift or full carrier-weight assertion.

#### The complete logarithmic source jet

Work in the polynomial source algebra through an arbitrary finite order M. If the incoming logarithmic jet is
\[
 \Psi(t)=\sum_{\varnothing\ne B}t_B A_B,\qquad
 t_B=\prod_{i\in B}t_i ,
\]
define
\[
 \Psi^+(t)=\log\pi_v(e^{\Psi(t)}).
\tag{HS20.28}
\]
The output coefficient with label set I is exactly
\[
 A_I^+
   =\sum_{\mathcal P\in\Pi(I)}
      \kappa_{\pi_v}(A_B:B\in\mathcal P).
\tag{HS20.29}
\]

Every higher incoming vertex A_B is retained. The spatial bound (HS20.23) applies to each generated cumulant, using the actual support of each such vertex; its order-one term is the exact conditional mean and need not create a new connection. If the incoming grade moment and support budgets have fixed factorial growth, (HS20.27), the ordered-partition count and the grade multiplication rule give a fixed changed factorial power for the entire finite jet. For example, input bounds of the form
\[
 \mathcal S_B(v)\|A_B\|_{L^p(\pi_v)}
 \le K^{d+1}(d!)^{p_0}b^d(dp)^{s d},
 \quad d=|B|,\quad p_0\ge1,\quad s\ge0,
\tag{HS20.30}
\]
give the conservative value bound C^m(m!)^(p_0+2s) b^m at total order m, with the partition-specific spatial factor in (HS20.23). The input budget in this example is explicit; it is not inferred from unnormalized component masses. Alternatively (HS20.26) uses the actual full-law grade budgets directly.

These definitions and estimates are compatible under reducing the source truncation order. They require no common convergent exponential-source series. Since (HS20.4) is the full mixture, (HS20.29) retains, in particular,
\[
 \operatorname{Cov}_{\pi_v}(F,G)
  =\mathbb E_C\operatorname{Cov}(F,G\mid C,v)
     +\operatorname{Cov}_C
        \bigl(\mathbb E[F\mid C,v],\mathbb E[G\mid C,v]\bigr),
\tag{HS20.31}
\]
and every higher analogue. Descriptor-mean cumulants have not been dropped.

### 8. Exact transport, support qualifications and scope

The source's complete R operation already sums the successful geometries and integrates the old internal Y states. Thus (HS20.4) is an explicit positive disintegration of that exact integration, not a new source-dependent action. If an augmented path space is to retain a history coordinate for later use, resample a fresh copy from pi_v independently conditional on v. This preserves the complete augmented source-free law. The corresponding marked quotient is pi_v F, independent of the newly resampled history. It is the normalized history operation required for the reverse-tail construction M-01.

The fresh Haar restoration described in Section 1 is performed with the whole transported jet. Therefore multiplying the actual numerator by its exact old marked expression, followed by (HS20.28), preserves all integrated source coefficients. No fresh coarse plaquette is substituted for an old transported mark.

The physical supports in Theorems HS20.3–HS20.4 are the unions of the **actual reset-coordinate component footprints**. They give a physical reset radius O(M R_k h) and an exponential spatial response outside it, uniformly in the remaining admitted history, with the stated order loss and support factors. All internal old labels in both X and Y components are included. Unreplaced Zbar labels and the output Y geometry are retained, not silently reset. Their later marked summation is part of H-02/H-04.

The proof does **not** identify a source background U_k coordinate with an independently variable raw retained link. A projected microscopic insertion can depend on U_k through a nonlocal minimizing map; its actual pullback, localization, old-current records and native regulator must still be supplied. Applying the finite cumulant inequality to pre-existing direct/current records is legitimate if their actual reset-variable support and moment budgets are supplied. The theorem does not bound the new response obtained by differentiating the posterior with respect to every raw retained coordinate or moving across an ambient selector/chart boundary.

Accordingly the following stronger conclusions are not asserted:

- a cutoff-uniform pointwise quotient by the complete shifted output native regulator;
- the full physical exponential **volume** carrier norm M-03 for an arbitrary transported insertion;
- the complete scalar matching theorem M-04, tensor matching M-05, or one-step response/current algebra M-06;
- the full-history summation H-04 or the all-scale induction M-07.

Theorems HS20.3–HS20.4 and the reset jet (HS20.29) give the spatial result for the mixed posterior under their support and moment hypotheses. KT19.3 is a stronger transport estimate.

### Primary source locations used

- CMP119 (1988), pp.254–258, (2.1)–(2.3), (2.19)–(2.22): nested geometries, old component factorization and full local positive operations.
- LFR I (1989), pp.177, 179–180, 192–201, particularly (1.10)–(1.12), (1.73), (1.76), (1.99)–(1.102): eligibility, preparation, complete reference quotient, local history sums and the fresh axial graph.
- LFR II (1989), p.365, (1.33)–(1.35): the common rebuilt determining field on every eligible component.
- LFR II pp.373–380, (1.61)–(1.75): common localized interaction family, positive completed component operation, successful Haar restoration and the exact joint sum.
- LFR II pp.383–392, (1.79)–(1.104): unnormalized component mass, the successful geometry sum, and the fixed residual alternative. In (1.92) the free set is explicitly the union of selected X and Y components; in (1.97) and (1.103) it is the fixed union of eligible Y components. The unreplaced Zbar region is not added to that free set.

The source scopes and coupling/geometry hypotheses are the already declared ones of C-01 and the preceding hypotheses. No unpublished Yang–Mills construction is invoked.

---
