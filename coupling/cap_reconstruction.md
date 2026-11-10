# Global cap reconstruction and boundary estimates

The estimates below concern the stated law. For all-history application, see [the composed-response criterion](../continuum/partial_gauge_transport.md).

**Catalogue item:** C-05.\
**Scope.** The proper-join constraint-fiber coherence follows from the cap identity. A full native comparison-frame/readout theorem, including its retained arguments and complete sector first-response bounds, is still missing. C-06 and C-08 receive no completion claim.

## 1 The source domain question has a definite answer

On CMP119, printed p.261, the native variable is a pair $\left( \mathbf{U},\mathbf{J} \right)$⁠. The current $\mathbf{J}$ in (2.36) is an independent variable. In contrast, every current in (2.37) is written

$$J_{p,X}\left( M^{\bullet}\left( \mathbf{U} \right) \right).$$

(GC.1)

It is the current of the corresponding minimizing reconstruction. It is not an additional independently assignable current slot. CMP109, printed pp.262--263, (1.15)--(1.16), makes this explicit: $J_{n}\left( M^{\bullet}\left( \mathbf{U} \right) \right)$ is obtained from the physical-current formula (1.8), with the reconstructed field substituted and the prescribed $L^{- n}$ normalization. The paragraph following (1.16) says that those pairs will themselves be substituted for the original variables.

Thus a proposed proof cannot simply declare all the currents in (2.37) to be independent extensions and choose their values freely. The independent extension of CMP109 (3.13) concerns the direct current slot in that formula. It does not erase (GC.1).

The alternative examined here is to make the field supplied to the primitive B activity a genuine minimum throughout its complex continuation. Only that unprepared minimum is differentiated with a physical second-order current operator. The original independently prepared field is used as determining data.

## 2 Global capping avoids the artificial reconstruction boundary

Let $\eta$ be the fixed fine spacing and $h_{r} = L^{r}\eta$⁠. The original nested regions and determining layers are those of C-01 and CMP119 (2.1)--(2.12). Fix an old birth scale $j \leq k$⁠.

The **complete global cap at** $j$ retains every original determining layer below $j$⁠, and prescribes the complete $j$-averaged field on the remaining region $\Omega_{j}$⁠. Let

$$C_{j}(W) = M_{\mathcal{B}^{\lbrack j\rbrack}}W,\quad\quad R_{j}(b) = U_{\mathcal{B}^{\lbrack j\rbrack}}(b),\quad\quad Q_{j}(W) = R_{j}\left( C_{j}(W) \right).$$

(GC.2)

Here $R_{j}$ is the unprepared source minimizing map for that determining geometry; it is not a random-walk-prepared map. Existing fine exterior data, including fixed bad-core bonds, are kept fixed. All fields in (GC.2) are on the same underlying fine lattice.

Theorem BC.1, proved the complete-global-cap identity: for a genuine admitted minimum $W$ of the original problem,

$$Q_{j}(W) = W$$

(GC.3)

after an orbit-identifying comparison gauge. Equation (GC.3) is not an identity of two independently prescribed source axial representatives. The uniform analytic comparison needed to use it inside the actual boundary integrand is the remaining issue in Section 11. The orbit-level proof uses the exact iteration of nonlinear averaging in CMP98 (43), the full endpoint-block convention following that formula, inclusion of the refined fiber in the original fiber, and uniqueness of the regular minimal orbit. This note does not replace that nonlinear average by a linear average.

The cap has no new boundary inside $\Omega_{j}$⁠. Its local mesh is the old mesh in the old layers below $j$⁠, and is $h_{j}$ throughout $\Omega_{j}$⁠. In particular, the output weights of CMP102 (190) on the observation region of a birth-$j$ boundary activity are exactly $h_{n}^{- 1},h_{n}^{- 2},h_{n}^{- 3}$⁠, for $n \leq j$⁠, with the terminal clause $n = j$ applying to the whole of $\Omega_{j}$⁠. There is no artificially refined collar at which a third inverse mesh power has to be paid.

### 2 1 Two elementary geometry facts

The weighted metric of the cap is denoted $d_{\lbrack j\rbrack}$⁠; the original metric is $d_{\Omega}$⁠. Their paths are on the same fine lattice and use the same permitted region. At every point the capped mesh is no larger than the original mesh. Consequently

$$d_{\lbrack j\rbrack}(x,y) \geq d_{\Omega}(x,y).$$

(GC.4)

This follows path by path by comparing the inverse mesh weights and then taking infima. No Euclidean substitute for either weighted metric is used.

There is also a useful general fact about admissible nested domains. If $\left( A_{r} \right)$ and $\left( D_{r} \right)$ are two aligned nested source block families with

$$dist\left( A_{r},A_{r - 1}^{c} \right) \geq M_{1}h_{r},\quad\quad dist\left( D_{r},D_{r - 1}^{c} \right) \geq M_{1}h_{r},$$

then $E_{r} = A_{r} \cap D_{r}$ is an aligned block family with the same separation. Indeed

$$E_{r - 1}^{c} = A_{r - 1}^{c} \cup D_{r - 1}^{c}$$

and each of the two distances from $E_{r}$ is at least $M_{1}h_{r}$⁠. Intersection therefore supplies an admitted candidate geometry for the common refinement of a global cap with a maximal local block family. This statement proves the geometric separation, but does not, by itself, identify every endpoint constraint of that candidate with the source's proper joined determining set. The actual proper-join refinement is proved in Section 8; no intersection identity is used.

## 3 A cap chart theorem with only one averaging power

One does not need the local two-power axial-gauge argument to place the global cap in its absolute minimizing-map chart. This is a material difference from trying to estimate a generic fine-collar reconstruction directly.

Let $U_{0}$ be the actual real genuine minimum at the fixed retained datum. In an admitted relative chart write

$$V = e^{i\eta A}U_{0}.$$

(GC.5)

For the source's unmodified nonlinear relative average, CMP102 (44) and CMP99 p.406 after (3.78), with the last fixed averaging step included, give

$$\left| \frac{1}{i}\log\left\lbrack M^{q}(V)M^{q}\left( U_{0} \right)^{- 1} \right\rbrack \right| \leq C_{av}h_{q}\sup_{st(q,y)}|A|.$$

(GC.6)

The comparison gauges and transports in this formula are the source's relative-average convention. The constant is independent of the number of fine bonds. Its proof, including the final fixed block step, is recorded in Annex AD (E14.39)--(E14.40). A bounded fixed chart factor is absorbed in $C_{av}$⁠.

For clarity, the following theorem states the precise data estimate it uses. It is a theorem about the actual global capped minimizing map, not a theorem about an arbitrary prepared physical current.

### Theorem GC 1 a global capped output estimate

Suppose that the complete relative determining data of the cap lie in a fixed smaller absolute chart of CMP102 Proposition 9. Suppose their logarithmic difference from $C_{j}\left( U_{0} \right)$⁠, on every determining layer $q \leq j$⁠, satisfies

$$\left| B_{q}(y) \right| \leq b_{*}e^{- \sigma(k - q)},\quad\quad 0 < \sigma < \nu,$$

(GC.7)

where $\nu$ is a reserved age-decay rate for the normalized row of the unprepared cap kernel. Then the relative capped minimum $W = R_{j}\left( e^{iB}C_{j}\left( U_{0} \right) \right)$⁠, represented in the source Landau/relative chart of CMP102 Proposition 9, satisfies

$$\begin{matrix}
h_{n}\left| A_{R} \right| + h_{n}^{2}\left| \nabla A_{R} \right| + h_{n}^{3}\left| D^{*}DA_{R} \right| \\
 \leq C_{cap}b_{*}e^{- \sigma(k - n)},\quad\quad n \leq j.
\end{matrix}$$

(GC.8)

The first-difference Hölder and covariant-Laplacian output norms in (190) obey their corresponding normalized bounds as well. The derivative in (GC.8) is that of the unprepared minimizing map in this source relative representative. Its constants are uniform in the cutoff, volume and admitted old geometry. This is not yet an admission of the actual B-frame tuple: the comparison gauge and retained covariant arguments are treated in §11.

**Proof.** The cap preserves every surviving nested-region separation. Thus the normalized row argument of CMP96 (2.46)--(2.59), already checked in Annex AF (BM.3)--(BM.7), applies to its geometry. In the kernel (190), the input-cell measure $h_{q}^{d}$ cancels the displayed factor $h_{q}^{- d}$⁠; the output factors are exactly the inverse powers shown in (GC.8). Reserve a fixed part of the exponential to sum the spatial row, and another part for the layer difference. The contribution from cap input layer $q$ to output layer $n$ is at most

$$C_{H}e^{- \nu|q - n|}\sup_{y \in \Gamma_{q}^{\lbrack j\rbrack}}\left| B_{q}(y) \right|.$$

(GC.9)

All fixed endpoint changes can be included in $C_{H}$⁠. Integrate the derivative of the actual minimizing map along $tB$⁠, $0 \leq t \leq 1$⁠, inside the smaller absolute chart. Using (GC.7), the resulting scalar sum is bounded by

$$\begin{matrix}
\sum_{q = 0}^{j}e^{- \nu|q - n|}e^{- \sigma(k - q)} \leq e^{- \sigma(k - n)}\left\lbrack \sum_{a \geq 0}^{}e^{- (\nu - \sigma)a} + \sum_{a \geq 1}^{}e^{- (\nu + \sigma)a} \right\rbrack.
\end{matrix}$$

(GC.10)

The bracket is finite because $\nu > \sigma$⁠. The same calculation applies to each of the source output norms. It proves (GC.8). Absolute chart admission precedes integration; the desired smaller B domain is not used to justify the kernel estimate. $▫$

The $D^{*}D$ term in (GC.8) is legitimate for this map: it is explicitly among the outputs of CMP102 (190), printed p.308. Nothing in this theorem asserts a $D^{*}D$ estimate for a separately prepared map or an individual random-walk term.

### 3 1 A useful exact data propagation lemma

The endpoint convention permits a precise refinement lemma independent of the minimizing-map estimates. It is useful in checking the candidate joined geometry.

**Lemma GC.0 (refined data determine the old data).** On aligned nested block grids, let $E_{1} \supset \cdots \supset E_{p}$ be a source-admitted nested family, and put $E_{p + 1} = \varnothing$⁠. Write $E_{r}^{b}$ for the source endpoint-lifted $r$-bond set, and use the actual determining rows $E_{r}^{b} \smallsetminus E_{r + 1}^{b}$ in that lattice. An **exterior** $r$**-bond relative to** $E_{r + 1}$ in this lemma has neither endpoint in the site domain $E_{r + 1}$⁠; it belongs to the complement of the endpoint-lifted bond set. This is weaker than requiring recovery of all bonds with at least one exterior endpoint.

Prescribe the actual nonlinear averages $M^{r}W$ on every determining row, and the source's fixed fine exterior. Then any other field obeying these data has the same $M^{r}$ as $W$ on every exterior $r$-bond relative to $E_{r + 1}$ whose actual source averaging stencil and branch are admitted, for $0 \leq r \leq p$⁠. In particular its $p$-average equals that of $W$ on every admitted stencil needed by the cap and old determining constraints. No nonlinear averaging operation is asserted to be globally defined through arbitrary bad fine exterior data.

If $E_{r} \subseteq \Omega_{r}$ for $r \leq p$⁠, those data imply every determining constraint of a global old family $\left( \Omega_{r} \right)$⁠, with arbitrary terminal level at least $p$⁠.

**Proof.** The assertion at level zero is part of the prescribed fine exterior. Suppose it has been proved at level $r$⁠. Take an $(r + 1)$-bond with neither endpoint in $E_{r + 2}$⁠. If at least one endpoint belongs to $E_{r + 1}$⁠, the bond belongs to $E_{r + 1}^{b} \smallsetminus E_{r + 2}^{b}$⁠, so its value is one of the prescribed $(r + 1)$-determining values. This includes a bond crossing the boundary of $E_{r + 1}$ under the stated no-endpoint condition at the next region.

If neither endpoint belongs to $E_{r + 1}$⁠, its two complete endpoint blocks lie outside $E_{r + 1}$⁠. This is where alignment and the actual paths of CMP98 (42)--(43) are used: $E_{r + 1}$ is a union of whole $(r + 1)$-blocks, an excluded endpoint center has an excluded endpoint block, and every child bond in the averaging paths has its endpoints in those two complete blocks. Thus each required $r$-bond has neither endpoint in $E_{r + 1}$ and is determined by the induction hypothesis. The exact nonlinear averaging operation determines the $(r + 1)$-value. These two cases prove the induction.

At $r = p$⁠, there is no remaining geometric exclusion, since $E_{p + 1} = \varnothing$⁠; recovery is asserted only on the actual admitted source averaging stencils just specified. A bond in an old determining row $r < p$ belongs to $\Omega_{r}^{b} \smallsetminus \Omega_{r + 1}^{b}$⁠, so neither endpoint belongs to $\Omega_{r + 1}$⁠. Because $E_{r + 1} \subseteq \Omega_{r + 1}$⁠, neither endpoint belongs to $E_{r + 1}$⁠, and the induction determines its $r$-average. For $r \geq p$⁠, apply the literal successive averaging operation on the stencils of that old constraint, using the recovered required $p$-data. This preserves every old determining value without defining a new average on an unadmitted bad region. $▫$

The lemma concerns actual determining bonds. It does not replace bond sets by intersections of endpoint-lifted point sets: those operations need not commute. In particular it is a criterion that the native join must meet, not a license to omit its crossing bonds.

### Corollary GC 2 one power cap data already give a useful age rate

Suppose the actual prepared input has old-layer potential response

$$\left| A(x) \right| \leq h_{\ell}^{- 1}C_{prep}g_{k} \parallel z \parallel_{\infty}e^{- \gamma\left( k - \ell - c_{0} \right)_{+}}$$

(GC.11)

on the complete averaging stencils. For unchanged determining layers $q < j$⁠, those stencils are the original determining stencils. On a terminal cap stencil, let $\ell \geq j - c_{1}$ be its smallest old regularity index, and suppose its endpoint blocks lie in the corresponding fixed two-layer source chart. The fixed integer $c_{1}$ accounts for the source endpoint convention. Then

$$\left| B_{q}(y) \right| \leq Cg_{k} \parallel z \parallel_{\infty}e^{- \sigma_{1}\left( k - q - c_{2} \right)_{+}},\quad\quad\sigma_{1} = \min\{\gamma,\log L\}.$$

(GC.12)

**Proof.** For $q < j$⁠, (GC.6) and the original proper-scale stencil give the original estimate, with a fixed adjacent-layer change. For the terminal layer $q = j$ and $\ell \geq j$⁠, (GC.6) gives the factor

$$\frac{h_{j}}{h_{\ell}}e^{- \gamma\left( k - \ell - c_{0} \right)_{+}} = L^{- (\ell - j)}e^{- \gamma\left( k - \ell - c_{0} \right)_{+}} \leq Ce^{- \sigma_{1}\left( k - j - c_{0} \right)_{+}}.$$

(GC.13)

This is the elementary convolution of the two age intervals $k - \ell$ and $\ell - j$⁠. The finitely many adjacent-layer cases only change $C,c_{2}$⁠. $▫$

Consequently $\gamma > \log L$ and $L > 2$ give $\sigma_{1} = \log L > \log 2$⁠, which is enough for the dyadic native-domain reserve. The local two-power improvement would improve this rate to $2\log L$⁠, but is unnecessary for cap-domain admission.

Using the ordinary relative average also avoids imposing a global axial gauge merely to improve a local averaging estimate. Such a gauge would require its own compatibility and torus-holonomy argument; none is implicit in (GC.6).

### 3 2 Independent native background and current slots

The same calculation handles a genuine independent background perturbation without falsely setting the retraction's base equal to that background. If the current-scale relative background coordinate has

$$h_{k}|b| + h_{k}^{2}\left| \nabla_{U_{0}}b \right| \leq c_{ext}\alpha_{0,k},$$

(GC.14)

then (GC.6) gives, on a cap determining stencil at level $q$⁠,

$$\left| B_{q}^{\, b} \right| \leq Cc_{ext}\alpha_{0,k}L^{q - k}.$$

(GC.15)

The BCH comparison is the uniform native first-difference comparison of Annex AD (E14.28)--(E14.31). The normalized row calculation with $\sigma = \log L$ yields

$$\parallel Q_{j}\left( e^{i\eta b}U_{0} \right) - U_{0} \parallel_{out,n} \leq Cc_{ext}\alpha_{0,k}L^{n - k}.$$

(GC.16)

Here the output norm is the one in (GC.8), not a raw link supremum norm. The AF comparison then gives

$$\frac{Cc_{ext}\alpha_{0,k}L^{n - k}}{\alpha_{0,n}} \leq CC_{AF}c_{ext}\sqrt{1 + k - n}\, L^{- (k - n)}.$$

(GC.17)

The supremum of the last factor is finite. Thus one fixed reduction of $c_{ext}$ controls this nonzero offphysical base displacement uniformly in depth.

In particular, this is not the invalid assertion $Q_{j}(U) = U$ for arbitrary independent $U$⁠. It estimates $Q_{j}(U)$ from the fixed admitted genuine center $U_{0}$⁠. The independently extended current affects the prepared input through its actual source preparation. At zero fluctuation that preparation has zero relative field for every allowed independent current, so there is no extra independent-current displacement in (GC.16). Uniformity in its nonzero fluctuation contribution still requires the actual prepared bounds on the joint native contour; those are an input of (GC.11), not a consequence of replacing $J$ by a physical current.

## 4 Physical current normalization on a coherent cap family

Let $W$ be a genuine capped minimum as above. Suppose a required local $p$-reconstruction, $p \leq j$⁠, is the actual coherent refinement/localization of this same $W$⁠, with its endpoint constraints and fixed exterior retained. Then Theorem BC.1, applies to it. The reconstructed fine field equals $W$ in the prescribed comparison gauge.

In the source units,

$$J_{p}(W) = L^{3(p - j)}J_{j}(W).$$

(GC.18)

Thus a normalized physical-current response $u_{n}$ on an old layer $n \leq j$ has

$$\left| \delta J_{p} \right| \leq u_{n}L^{3(p - n)} \leq u_{n}L^{3p - 2n - \min(p,n)}.$$

(GC.19)

The last weight is precisely (2.37). The two powers agree if $n \leq p$⁠, and otherwise their ratio is $L^{p - n} \leq 1$⁠. Curvature is unchanged on the same fine plaquettes and has the source weight $L^{- 2n}$⁠.

The physical current of the cap itself is bounded by (GC.8) and the exact local expansion CMP109 (3.11), including its local lower-order remainder. That remainder uses the field and first-difference norms and only changes the fixed constant. There is no replacement of $D^{*}D$ by a bare Laplacian. The identity

$$D^{*}D + DRD^{*} = \Delta - P_{1} + \mathcal{K}_{U}$$

and the associated $\mathcal{K}_{U}A$ in the source $F_{1}$ remain intact.

For complex determining data, the coherent identity first holds on an open real chart of those determining data and then continues holomorphically. Composition with a separately analytic input depending on $U,J,s$ is legitimate once its entire image is admitted. This does not apply the identity theorem on the physical-current graph in the larger independent $(U,J)$ space.

## 5 The stronger boundary anchor estimate

The one-power cap rate of Section 3 is sufficient for domain admission, but by itself would not pay a raw four-dimensional count $L^{4(k - j)}$⁠. An actual boundary anchor supplies a stronger estimate for the activity sum.

Let $X \in \mathcal{D}_{j}$ meet the actual source set $Z_{j} = \Lambda_{j}^{c}$⁠, and choose a point $w \in X \cap Z_{j}$⁠, with the source endpoint convention. Let $x \in X$ be an output/readout point, and let $y$ be a cap determining point in a strictly deeper old region $\Omega_{\ell}$⁠. Use $\ell \geq j + 2$⁠, so that the source nesting $\Omega_{j + 1} \subseteq \Lambda_{j}$ places $Z_{j}$ outside $\Omega_{\ell - 1}$⁠. The finitely many adjacent-level cases are handled without this stronger estimate. Retain the actual source separation

$${dist}_{phys}\left( \Omega_{\ell},\Omega_{\ell - 1}^{c} \right) \geq c_{sep}MR_{\ell}h_{\ell}$$

(GC.20)

whenever that running collar is available; if only the fixed variational separation is being used, replace $R_{\ell}$ by its fixed lower bound. Since $Z_{j} \subseteq \Omega_{\ell - 1}^{c}$ for the stated nonadjacent levels, a physical path from $y$ to $w$ must traverse that separation. Every cap-metric weight is at least $h_{j}^{- 1}$⁠. The source tree in $X$ connects $x$ to $w$ with physical length at most $C_{tree}Mh_{j}\left( d_{j}(X) + 1 \right)$⁠. Therefore

$$d_{\lbrack j\rbrack}(y,x) + C_{tree}M\left( d_{j}(X) + 1 \right) \geq c_{sep}MR_{\ell}L^{\ell - j}.$$

(GC.21)

This is a physical triangle-inequality argument, so it remains true even if the carrier tree enters a finer old layer. It does not require bounding that part of the tree in the cap metric by its Euclidean length: the cap distance is first bounded below by physical distance divided by $h_{j}$⁠.

Splitting fixed fractions of a cap-kernel exponential and the primitive B carrier exponential thus gives

$$e^{- ad_{\lbrack j\rbrack}(y,x)}e^{- bd_{j}(X)} \leq Ce^{- cR_{\ell}L^{\ell - j}}e^{- a'd_{\lbrack j\rbrack}(y,x)}e^{- b'd_{j}(X)},$$

(GC.22)

for some fixed $a',b',c > 0$⁠. In choosing $c$⁠, the factor $C_{tree}M$ is explicitly paid from $b - b'$⁠; one does not pretend that all constants are independent of $M$⁠.

### Proposition GC 3 no age rate ceiling in the anchored two map sum

For any $\lambda > 0$⁠, $c > 0$⁠, $L > 1$⁠, and fixed $r \geq 0$⁠,

$$\sum_{v = 0}^{a}(1 + v)^{r}e^{- \lambda(a - v)}e^{- cL^{v}} \leq C_{\lambda,c,L,r}e^{- \lambda a},\quad\quad a \geq 0.$$

(GC.23)

**Proof.** Factor out $e^{- \lambda a}$⁠. The remaining sum is bounded by

$$\sum_{v \geq 0}^{}(1 + v)^{r}e^{\lambda v - cL^{v}} < \infty.$$

The exponential $L^{v}$ dominates the linear term and the logarithm of the polynomial; comparison with a convergent geometric series proves finiteness. $▫$

In an actual cap/original-map composition, $v = \ell - j$ and $a = k - j$⁠. The original prepared map supplies $e^{- \lambda(k - \ell)}$⁠; for the nonadjacent levels the cap-to-boundary connection supplies $e^{- cL^{\ell - j}}$ from (GC.22). The omitted $v = 0,1$ terms are at most a fixed multiple of $e^{- \lambda a}$⁠, so they obey the same conclusion. The factors from ordinary averaging are at most one up to the fixed stencil constant and only improve the estimate. Consequently the combined boundary-anchor estimate retains the original reserved age rate $\lambda$⁠, rather than being limited to $\log L$⁠.

This deduction concerns the actual path factors after both normalized rows and their stencil attachments have been retained. It is not permission to replace the cap map by a global-support activity. Its usefulness is that the $\log L$ domain-admission rate and the summable boundary-activity rate have different proofs and need not be the same number.

## 6 A direct quasilocal Hessian device

There is a useful alternative to assigning a global footprint to a retracted primitive activity. The following elementary analytic estimate keeps its actual spatial response.

### Lemma GC 4 two first response bounds give a weighted second response

Let $f$ be holomorphic on a complex coordinate polydisc of radius $2r$ about a real product support. Suppose, uniformly on the smaller radius-$r$ product neighborhood,

$$\left| \partial_{i}f \right| \leq Aa_{i},\quad\quad a_{i} \geq 0.$$

(GC.24)

Then on a fixed further smaller neighborhood,

$$\left| \partial_{i}\partial_{m}f \right| \leq \frac{CA}{r}\min\left( a_{i},a_{m} \right) \leq \frac{CA}{r}\sqrt{a_{i}a_{m}}.$$

(GC.25)

**Proof.** Cauchy applied to the $m$-coordinate derivative of $\partial_{i}f$ gives the first bound with $a_{i}$⁠. Commuting the derivatives and applying the same argument in the $i$-coordinate gives it with $a_{m}$⁠. Their minimum is at most their geometric mean. The fixed contour reserve gives the constant $C$⁠. $▫$

For example, if $a_{i} = e^{- \delta d(i,X)}$⁠, then (GC.25) carries both endpoint factors

$$e^{- \frac{\delta}{2}d(i,X)}e^{- \frac{\delta}{2}d(m,X)}.$$

(GC.26)

After retaining the primitive tree joining the two readout points in $X$⁠, the triangle inequality bounds the desired current-coordinate weight $e^{\gamma\rho_{k}(i,m)}$ by fixed fractions of the two endpoint exponentials and the carrier-tree exponential. Summing the remaining endpoint rows and the anchored primitive carriers then gives a volume-independent Hessian row, whenever those actual first-response rows and carrier prefactors have been verified. The device does not introduce a spurious torus-volume factor and does not require pretending that a quasilocal function has finite support.

The same first-response estimate, followed by Cauchy in the remaining admitted slots, gives local higher directional jets with a fixed factorial budget. However, neither statement supplies an unproved first-response bound or changes the specified native radii.

## 7 Application and its hypotheses

The global route removes two conceptual problems of a local retraction construction:

1.  no bounded enlargement $Y$ is needed to avoid an artificial fine collar; the cap is a genuine admitted global determining geometry;
2.  its independent-background base is bounded from the fixed genuine center by (GC.16), rather than being declared equal to the arbitrary independent input.

Section 8 identifies the constraint fiber. The remaining exact application checks are:

- Equality of minimal orbits must be implemented in the actual comparison frame, including every retained covariant argument. This is the substantive unresolved point in Section 11.
- Every terminal cap averaging stencil must be checked against the actual two-layer source charts, including bonds meeting the boundaries of the original determining layers. Corollary GC.2 explicitly retains that check. It is easier than constructing an arbitrary local enclosing collar, but it has not been replaced by a drawing or a pointwise mesh label.
- The whole native $b,J,s$ tube must obey the prepared first-output bound used in (GC.11) with its actual source coordinate conventions. The independent-background cap estimate itself is (GC.16); it does not declare an arbitrary external coordinate to have norm (GC.14).
- The combined path rows in (GC.22)--(GC.23) must be applied to every sector in the source boundary ledger: inherited B differences, classical/constraint/Haar contributions, E/R terms assigned to B, heterogeneous Wilson coefficients, complete relocation terms and historical Gaussian cross terms. Newest-boundary E/R terms use their regular prefactor and do not receive an old-boundary collar factor.
- The first-response hypotheses needed for GC.4 must hold for the actual retained native derivatives as well as the free current directions. Exact Gaussian exterior forces and their Schur scalar remain in their proper Gaussian/outer-marginal split.

Accordingly, **C-05 is not yet claimed complete by this note**. C-06 and C-08 likewise receive no closure. The global cap argument gives its explicit unprepared output theorem, its control of the offphysical base from an admitted center, the one-power-versus-boundary-age distinction, and the quasilocal second-response device.

## 8 The completed proper join constraint fiber argument

The following is the constraint-fiber version of Section 4. The intersection candidate of Section 2 is **not** identified with the source's join. Such equality can fail: a proper $n$-collar ends before a maximal local $(n + 1)$-layer begins, and the source restores old interior data in the intervening strip.

Read the actual local $p$-problem from CMP119 (2.14) and its subsequent several-patch prescription. In its retained interior, old determining rows below $p$ remain, and deeper rows are capped at $p$⁠. On a boundary patch in old layer $n$⁠, it uses the local maximal prefix through $\min(n,p)$⁠. Every local index is therefore at most the old index. The patchwise construction is restricted to its corresponding old-layer domain before it is combined with the other patches. The fine exterior and bad-core data remain fixed.

For the nested site family $\left( E_{r} \right)$ of this **actual source-admitted proper join**, this gives

$$E_{r} \subseteq \Omega_{r},\quad\quad r \leq p.$$

(GC.27)

One next uses the actual determining bond rows; no endpoint lift is distributed through an intersection. Lemma GC.0, applied to a competitor extended by $W$ outside the local problem, recovers every required old constraint, including the admitted averaging stencils that cross the local boundary. Hence the local constraint fiber is contained in the global capped fiber.

Suppose $W$ is a strict real regular genuine minimum of the global cap, and give the local problem its actual determining averages. The same Wilson functional, with all incident boundary plaquettes, is used in both problems. The exterior action is constant under the local variation. A sufficiently small neighborhood of $W$ in the refined fiber still satisfies the stronger old regularity inequalities, because they have strict margins at $W$⁠. Therefore $W$ is a local minimum of the local problem. It obeys the finer regularity restrictions, which are weaker, and uniqueness identifies the two **minimal orbits**.

This is precisely the argument after CMP102 (150). It does not say that the entire finer regularity space lies in the old space. Holomorphic continuation is first in global capped determining data, before an independent $(U,J,s)$ input is composed. The current unit conversion in (GC.18)--(GC.19) then holds in a common comparison frame. Establishing the required actual frame and all its analytic bounds remains separate.

## 9 Domain estimates and an explicit scalar domain reserve

### 9 1 Zero preparation is an identity of the actual source extension

CMP116 (1.2), with the independent $U,J$ dependence suppressed in its notation as stated there, gives

$$\mathcal{H}_{s}(B') = H_{0,s}B' + A_{0,s}(B') - H_{s}D_{s}\left( H_{0,s}B' + A_{0,s}(B') \right).$$

(GC.28)

Its (1.14) and (1.16) give

$$\left| D_{s}(A') \right| \leq 4C_{2}|A'|^{2},\quad\quad\left| A_{0,s}(B') \right| \leq 4C_{4}\left( B_{0}e^{16\kappa_{1}} \right)^{3}|B'|^{2}.$$

(GC.29)

Therefore

$$\mathcal{H}_{s}(0;U,J) = 0$$

(GC.30)

for every admitted independent $(U,J,s)$⁠. The preceding constraint substitution $g_{k}Cz - hD\left( g_{k}Cz \right)$ also vanishes at zero. This proves the centered-input fact used in (GC.16). There is no independent constant $- G_{s}J$ in this actual formula. No assertion that the independent $J$ annihilates a constraint tangent space is needed.

### 9 2 The fine field supplied to inherited B is a minimum at every real current

CMP119 (3.15), printed p.268, supplies the nested argument

$$U_{k}\left( \exp i\left\lbrack g_{k}CA_{k} - hD\left( g_{k}CA_{k} \right) \right\rbrack\, V^{(k)} \right)$$

(GC.31)

to inherited E, R and B. The fluctuating coarse field inside parentheses need not be a minimum. The **outer** $U_{k}$ is the actual fine-lattice minimizing map. Thus the variational premise of global-cap consistency holds for every admitted real current $A_{k}$⁠, not only for $A_{k} = 0$⁠.

This applies to (GC.31), not directly to its coarse fluctuating argument. It verifies the minimum premise for physical agreement. It does not resolve the retained-argument frame issue in Section 11.

### 9 3 A numerical reserve with all adjacent level shifts retained

Let $a = k - n$⁠, absorb the fixed shifts in (GC.12) into $C_{sh}$⁠, and use $\gamma \geq \log L$⁠. Then

$$e^{- \left( \log L \right)\left( a - c_{2} \right)_{+}} \leq L^{c_{2}}L^{- a}.$$

(GC.32)

With the already admitted fixed choices

$$\alpha_{0,n} = C_{0}g_{n}\ell_{n}^{q},\quad\alpha_{1,n} = C_{1}g_{n}\ell_{n}^{q},\quad P_{k} = A_{1}\ell_{k}^{p_{0}},\quad\quad q > p_{0},$$

(GC.33)

the cap response, divided by the appropriate one of the two radii, has the bound

$$C_{abs}\sqrt{1 + a}L^{- a}\left\lbrack c_{ext} + \ell_{k}^{p_{0} - q} \right\rbrack.$$

(GC.34)

The constant retains the fixed ratio $C_{0}/C_{1}$⁠, as well as $C_{sh},A_{1}$⁠, the AF comparison, and the actual averaging and cap-map constants. A current/curvature bound with $\alpha_{0}$ is not silently reused for the relative-field clause with $\alpha_{1}$⁠.

For $L > 2$⁠,

$$T_{L}: = \sup_{a \geq 0}\sqrt{1 + a}(2/L)^{a} < \infty.$$

(GC.35)

Since $j - n \leq a$⁠, the explicit sufficient test

$$C_{abs}T_{L}\left\lbrack c_{ext} + \ell_{k}^{p_{0} - q} \right\rbrack \leq \beta/16$$

(GC.36)

gives

$$\parallel \Delta\Phi_{n} \parallel_{n} \leq (\beta/16)\alpha_{*,n}2^{- (j - n)}.$$

(GC.37)

Choose $c_{ext}$ first as a fixed sufficiently small constant, then reduce the common weak-coupling ceiling. The real-center ratio $\varepsilon_{n}/\alpha_{*,n}$ is also small because $q > p_{0}$⁠. The absolute map chart is admitted before this smaller-output test. No parameter varies with the derivative order.

This proves the scalar reserve for outputs having the actual normalized cap estimates. It does not prove an unverified comparison-gauge estimate by renaming that gauge as $\Phi_{n}$⁠.

## 10 The proposed local readout and the remaining norm test

To turn the cap's field response into a primitive B derivative, a local analytic readout is still needed. Its intended radius can be made explicit.

Let $Y_{X}$ be a fixed $j$-cube padding of $X$⁠. The elementary tree estimate gives

$$d_{j}\left( Y_{X} \right) \leq C_{pad}\left( 1 + d_{j}(X) \right).$$

(GC.38)

Indeed, attach only finitely many neighboring cubes per original cube to its connecting tree. Their number is bounded by a fixed multiple of the original tree length plus one. This controls Euclidean $j$-carrier cost. **It does not itself prove every proper-patch hypothesis of (2.14)** at intersections with old layers.

The intended source proper localization of the global cap on $Y_{X}$ should place all observation and endpoint stencils of $X$ beyond its artificial collars, whose widths are at most $2M_{1}h_{j}$⁠. Existing fine bad-core data are fixed and should be omitted from the free analytic coordinates. No integration over a bad component takes place in this proposed variational readout.

For an actual free local determining point $y$⁠, let $\widehat{q}(y)$ be the local mesh index and $n(y) \leq j$ the old capped index. The candidate radius is

$$w_{y} = c_{rd}\alpha_{0,n(y)}2^{- \left( j - n(y) \right)}\frac{h_{\widehat{q}(y)}}{h_{n(y)}}.$$

(GC.39)

The fine-collar scale factor is retained. A useful rigorous implication is the following: if the actual local metric and weights obey

$$w_{y}/w_{x} \leq C_{w}e^{\epsilon d_{loc}(x,y)},\quad\epsilon < \delta_{loc},$$

(GC.40)

then the normalized source kernel gives

$$\sum_{y}^{}Ce^{- \delta_{loc}d_{loc}(x,y)}w_{y} \leq CC_{w}C_{row}\left( \delta_{loc} - \epsilon \right)w_{x}.$$

(GC.41)

The proof is simply to factor out $w_{x}$ and sum the remaining exponential. The actual normalized integration measure must be used. To establish (GC.40) one must separately retain the path costs of both $\left| \widehat{q}(y) - \widehat{q}(x) \right|$ and $\left| n(y) - n(x) \right|$⁠; the carrier bound (GC.38) does not provide them.

If this local map and its comparison frame were admitted, averaging of a coherent current response would cancel the factor $h_{\widehat{q}}/h_{n}$⁠, leading to the candidate first-response norm

$$CB_{0}e^{- \kappa d_{j}(X)}\sup_{y \in Y_{X}}\frac{2^{j - n(y)}\left| \delta W(y) \right|_{norm,n(y)}}{\alpha_{0,n(y)}}.$$

(GC.42)

The full cap/original path product must be retained until (GC.21)--(GC.23) has paid its stronger age factor; prematurely replacing it by a single original-metric exponential can lose that factor. The old real arguments must remain in the actual allowed chart throughout.

The final complete-action targets include the stronger entrywise-supremum bound

$$\sup_{i}\sum_{m}^{}e^{\gamma\rho_{k}(i,m)}\sup_{\parallel z \parallel \leq P_{k}} \parallel D_{i}D_{m}{\widetilde{B}}_{k}(z) \parallel_{op} \leq C_{B}K_{B,k}P_{k}^{- 2},$$

(GC.43)

and

$$\sup_{i}\sup_{\parallel z \parallel \leq P_{k}} \parallel D_{i}{\widetilde{B}}_{k}(z) \parallel \leq C_{B}K_{B,k}P_{k}^{- 1}.$$

(GC.44)

GC.4 would supply an envelope independent of $z$⁠, making the supremum inside the sum legitimate. It cannot supply the missing actual first-response estimate (GC.42).

Native derivatives must be taken on the current-dependent difference

$$B^{(j)}\left( X,Q_{j}V(z),\ldots \right) - B^{(j)}\left( X,Q_{j}V(0),\ldots \right).$$

(GC.45)

The subtracted scalar remains in the outer marginal. No globally small direct native derivative of that scalar is asserted.

## 11 The comparison frame obstruction and status

### 11 1 Retained covariant arguments matter

CMP119 p.261, item (iii), makes primitive B invariant under simultaneous transformations of $U,J$ and the old fields $\mathbf{A}$⁠:

$$B\left( X,U^{u},{Ad}_{u}J,{Ad}_{u}\mathbf{A},\{ S\} \right) = B\left( X,U,J,\mathbf{A},\{ S\} \right).$$

(GC.46)

Orbit equality does not give this identity with $\mathbf{A}$ held fixed. Transporting a merely smooth old cutoff through a complex gauge is not automatically an analytic substitution.

LFR II p.373, after (1.61), explicitly retains its comparison gauge because its two boundary representations differ; it refers to the blockwise analytic formula (106) in its cited source. CMP102 p.307 explicitly transforms the Landau solution back to a geometry-dependent axial gauge. Thus no verified literal-prefix identity currently makes the frames identical on every required readout.

### 11 2 Exact algebraic alignment is not yet the native analytic estimate

Choose a tree in each determining block, rooted at its determining vertex $y$⁠, and write $\Gamma_{yx}$ for the path to $x$⁠. If $R$ and $V$ belong to the same constrained gauge orbit, define

$$u(x) = V\left( \Gamma_{yx} \right)^{- 1}R\left( \Gamma_{yx} \right),\quad\quad u(y) = 1.$$

(GC.47)

Then $R^{u} = V$⁠. To prove it, let $v$ be the orbit-identifying gauge transformation fixing the roots. Its path identity is $R\left( \Gamma_{yx} \right)v(x)^{- 1} = V\left( \Gamma_{yx} \right)$⁠, which gives $v(x) = u(x)$ at every vertex. Consequently equality holds on all bonds.

Formula (GC.47) is holomorphic for complex links and uses their inverses, not their adjoints. If the relative potentials have total line norm at most $a$⁠, the elementary product bound gives

$$\parallel u(x) \parallel ,\  \parallel u(x)^{- 1} \parallel \leq e^{Ca}.$$

(GC.48)

However, (2.39) requires the first differences of the **transformed relative field**, which involve second differences of $u$⁠. Equation (GC.48) does not control them. Even a first-difference estimate on an incoming potential does not automatically do so for an arbitrary long axial path. In an Abelian local example, $A_{x}(x,y) = u\sin(Ny)/N,\ A_{y} = 0$ has potential and first derivatives bounded by $O(u)$⁠, while its axial parameter $\lambda = xu\sin(Ny)/N$ has $\partial_{y}^{2}\lambda = - xuN\sin(Ny)$⁠.

This example shows the insufficiency of the proposed size/first-derivative proof; it is not a counterexample obeying every higher source-preparation norm. A successful repair must use those additional norms and the actual gauge-fixing construction, or prove literal compatibility of the source frames. That repair has not been established here.

### 11 3 Complete sector estimates

The desired full prefactor is the source-sector expression of Annex AF (BV.17):

$$\begin{matrix}
K_{B,k} \leq C_{src}\left( 1 + S_{b,\delta} \right)\lbrack{\mathfrak{K}}_{E} + C_{R}g_{k}^{\kappa_{0} - 11} + B_{0}\ell_{k}^{p_{0} - q} \\
 + g_{k}^{- 2}\left( g_{k}P_{k} \right)^{3} + g_{k}P_{k} \\
 + g_{k}^{- 2}\left( g_{k}P_{k} \right)e^{- c_{col}MR_{k}} + g_{k}^{\nu}\rbrack.
\end{matrix}$$

(GC.49)

Every following source sector must be included on the same actual contour:

  -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Sector**                                                         **Retained verified input**                                                              **Remaining application here**
  ------------------------------------------------------------------ ---------------------------------------------------------------------------------------- -------------------------------------------------------------------------------
  Inherited B, including historical Gaussian cross-component terms   Full primitive tree bound; actual minimum argument (GC.31); constraint-fiber coherence   Native comparison/readout and first response with all old covariant arguments

  Classical nonlinear fluctuation, constraints, Haar and coarea      Actual constrained current coordinates and source remainder formulas                     Complete application of the joint contour and local norm to every remainder

  E/R terms assigned to B                                            Completed regular prefactors and actual source classification                            Mixed-domain application on that same verified comparison contour

  Heterogeneous Wilson term                                          Actual localized coefficient, quadratic age bound and explicit $g_{k}^{- 2}$             Admitted complete response retaining the running current collar

  Relocation and Jacobian                                            All previous-action/Jacobian terms; old cutoff arguments kept real                       Full comparison and relocation input admission and response
  -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Newest-boundary E/R terms may touch the current support and do not receive an old-$Z_{k}$ collar factor. The heterogeneous $g_{k}^{- 2}$ is paid only by the actual running current collar. The present Gaussian exterior force and Schur scalar remain in their exact Gaussian/outer-marginal split, outside the small perturbation prefactor.

Because the comparison/readout step is unresolved, (GC.49) has not been obtained for the complete actual pullback, and (GC.43)--(GC.44) have not been proved for that family. The newly verified cap and coherence results do not replace those applications.

**Status:** C-05 remains open; no C-06 or C-08 closure follows. The new results are the direct proper-join constraint-fiber proof, the global-cap relative-row theorem, the one-power reserve, the exact zero-preparation and physical minimum checks, the boundary-anchor age estimate, and the quasilocal Hessian implication. The remaining frame, local readout and complete-sector requirements are explicitly retained.
