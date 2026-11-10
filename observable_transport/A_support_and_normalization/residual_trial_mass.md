# Residual old mass: a matched source operation and a fresh-fluctuation trial

This note addresses the normalization of every complete fresh-reference class produced by the **literal rectangular-chain preparation** of LFR I pp.195–196. Section 3 uses the bounded-ancestor witness of [residual merger witness](residual_merger_witness.md); the earliest ancestral union need not be one component. The actual old operation still sums all histories in its class; only the lower-bound trial replaces the pre-birth history. The note distinguishes the positive self-operation in LFR II (1.71) from the complete old conditional, which also contains the boundary interactions displayed in (1.72)/(1.103). It never replaces an old normalizer by the fresh reference integral. Section 6 gives the lower-bound proof with a deliberately weak but affordable trial thickness. Its selector/energy, normalization, and geometric steps are analysed separately. A broader preparation with an unspecified forest of inner holes is outside this theorem, and the theorem does not complete M-04.

## 1. Which quantity the source upper bound controls

Fix an eligible component Y, the current step k, the unreplaced exterior, and the actual new current field v on Y. Work in one of its actual residual coarea strata. Fix a **complete fresh-reference class** r: the prepared core Λ, graph G and its anchor/orientation convention, reference-orbit and representative rule, fresh cutoff, localized action cutoff ζ, scale/coupling labels, and every other choice entering the same fresh h/H factor. Old histories with different r are not combined before cancellation.

The primary formula LFR II (1.71), printed pp.378–379, defines a positive old operation. With its history sum restricted to r, write it schematically, but with all integration types displayed, as

\[
 \mathcal M^{\rm self}_{r,v}F
 =\sum_{\gamma:\,r(\gamma)=r}w_\gamma
   \int dB\,\sigma(g_kB)\,\delta_{T_\gamma}(B)\,
                 \chi'_\gamma
   \int dV_h\,\chi_{h,1/2}\,
     T_{h,\gamma}\!left[
       F\,e^{-Q_\gamma-S_\gamma+V_\gamma^{\rm self}
                         +C_\gamma^{\rm norm}}
                      \right].
 \tag{RT.1}
\]

Here h=k−N. The B coordinates are the actual mixed preparation coordinates on B₀, with its literal tree removed. The V_h integral is the old core integral on the region in (1.71). T_h contains precisely its surviving earlier raw/group and ordinary fluctuation coordinates. The positive weights wγ include the source's finite axial-orientation averages. The exponent contains the two nonnegative source energies Q and S of NR20.2, the self interaction of (1.69), and the exact normalization/vacuum terms in the last line of (1.71). In particular the displayed factor

\[
 \exp\left[\left(-\tfrac12\dim G\log g_k^{-2}
                              +\log\sigma_0\right)
                |(B_0\setminus T_0)\cap Y|\right]
 \tag{RT.2}
\]

is kept in Cnorm. It is the physical Haar-coordinate factor for B, not an additional Gaussian probability to be inserted later.

There is **no integration over the fresh field** V′_k in (RT.1). The residual selector, χk,Λ, fresh χ, and δG(V′k) are outside T′ after r has been fixed. Printed pp.391–392 make this unambiguous: (1.104) contains T′k(Y)1 as a multiplier depending on the new V_k restricted to Y. Consequently NR20.5/9a apply pointwise at this conditioning level. Positivity permits restriction to a reference class:

\[
 \mathcal M^{\rm self}_{r,v}
       e^{\theta\mathcal F+uD_{\rm old}}
       \le e^{-P_0(g_k)}
 \quad(u\ge0\hbox{ fixed}),
 \tag{RT.3}
\]

whenever r is a restriction of that actual internal sum and the external data are in its admitted real domain. Its old energy and rank are the actual NR20 quantities. No fresh/core integration is added before applying this inequality.

There is a further necessary distinction. In (1.72), the old operations still act on the cross-domain terms V(X). In (1.103), their normalized product acts on exp ΣB′(X). Thus (RT.1) alone is the **self-operation**, and its normalization is not automatically the full conditional normalizer in RS.1. For a fixed complete exterior and fixed r, write the latter, at the same post-cancellation stage, as

\[
 \mathcal M^{\rm full}_{r,v}F
       =\mathcal M^{\rm self}_{r,v}
                      [F e^{\mathcal V_{\rm cross}}].
 \tag{RT.4}
\]

All actual cross terms must be retained, or compared by a separately proved C-08 bound. A bound already integrated over fresh variables would not establish (RT.3) or (RT.4).

The common retained h/H factor can be moved between the outer density and the old operation only by the exact source algebra. LFR II (1.10), (1.14)–(1.37) carries out the large classical cancellation before (1.71). This note uses that final convention throughout. An alternative convention multiplies both (RT.3) and a lower bound for (RT.1) by the same explicit retained-only factor; it cancels in the quotient, as in RM.2. A lower bound for H itself is not used.

## 2. A physical R birth realizes the thin rectangles

The strict pure-gauge Q birth of NR20.4 realizes large rectangles but is not the minimal geometry. With no earlier local bad region and no P/Q birth, CMP119 (3.5), (3.16), (3.20), printed pp.265–269, gives an R-only birth with Ω_h unchanged locally and

\[
 Z_h=(R'_h)^{+1}.
 \tag{RT.5}
\]

The superscript adds one MR_h-cube layer. Every nonempty rectangle admitted by these constructions has side lengths at least three such cubes; R birth is the minimal padding, while P/Q/inherited regions have more. Thus R′h can be the one-layer erosion of a prescribed admissible rectangular Z_h.

### Lemma RT.1 — a strict local R seed in the actual free chart

For sufficiently weak admitted background curvature and the fixed source hierarchy A₁≪A₀, one MR_h cube contains a positive-volume event that creates an R_h test but no new P_h or Q_h test. The event is supported on a fixed number of (h−1)-scale averaging blocks, has dimensionless positive quadratic energy at most CP(g_{h−1})²+C, and keeps the exact h-average unchanged.

**Proof.** First work at flat data in one L-block. It has 4L³(L−1) internal bonds and L⁴−1 bonds in an internal spanning axial tree. Choose an internal one-cochain a which vanishes on that tree, vanishes on all exceptional interblock bonds, and satisfies Qa=0. Only the at most eight coarse averaging constraints incident to this block can be nonzero. Hence the available scalar dimension is at least

\[
 4L^3(L-1)-(L^4-1)-8>0
 \tag{RT.6}
\]

for the source's fixed large L. Choose a nonzero vector and one fixed Lie generator. Normalize max|a|=1. It is physical: a curl-free cochain with zero axial tree values would vanish on every internal bond by discrete Stokes.

In the actual independent-coordinate chart put

\[
 A=\frac{3\delta_{h-1}}{2g_{h-1}}\,a.
 \tag{RT.7}
\]

At the flat center C₀a=a. At a weak real background, the exact map C differs locally from C₀ by a quantity tending to zero with the background curvature, after a local block gauge. Its independent entries remain the specified free entries. Exceptional entries may now be nonzero; they are O(curvature) times the seed and lie in the fixed adjacent-block stencil. The nonlinear constraint correction hD(gCA) is O(δ²), and is kept. The reconstructed field is exactly

\[
 V_{h-1}=\exp\{i[g_{h-1}C A-hD(g_{h-1}CA)]\}\,V^{(h-1)},
 \tag{RT.8}
\]

as in CMP119 (3.15). Its h-average is the prescribed V_h. This is the exact nonlinear constraint chart; no abelianized averaging identity is substituted for it.

The literal free R test (3.16) fails because max|A|=3δ/(2g)>δ/g. On the other hand, the relative link variation in (RT.8) is below 7δ/4 for sufficiently small coupling. The approximate local reference differs from the exact reference by the source error in (3.17)–(3.19), which is o(δ). Thus every approximate Q test is strictly below its 2δ threshold. Its plaquette and soft gauge variations are at most C_Lδ, strictly below the ε threshold after the fixed A₁/A₀ choice. This proves all the strict selector assertions.

The source unit-lattice precision has a uniform upper bound as well as a gap: CMP99 p.428, after (3.158), gives its uniform exponential kernel bound. Its Schur compression therefore has a uniform upper bound. The seed uses a fixed number of coordinates and has size O(P); its quadratic energy is CP². Actual Haar/coarea/nonlinear factors remain in the full density and are bounded on this small chart.

Place the seed farther than 2LM₂R_h, plus its fixed constraint stencil, from the boundary of the chosen MR_h cube. M≫LM₂ makes this possible. Every enlarged R test containing its support then belongs to that same coarse covering cube. The inequalities survive fixed sufficiently small dimensionless free-coordinate balls. In a soft-gauge chart the tree coordinates, if integrated, receive such balls about zero; they are not fixed on a zero-measure subset. In a hard-tree chart they are absent by definition. ∎

Putting one seed in every MR_h cube of the erosion of Z_h makes the exact R′ cover equal that erosion. Eligibility bounds the number by a fixed constant, at most a fixed enlargement of 100⁴. Thus the total birth energy is still CP(g_h)². It does not grow as R_h⁴P(g_h)²: the seed count is in MR_h cubes, not in the fine bonds of the rectangle.

### The determining-data distinction

An R-only birth has Ω_h full locally. CMP119 (2.2) therefore gives no local Γ_{h−1} raw determining datum. The seed is the retained A_{h−1} coordinate in T_h, by (2.20)–(2.22), on Z_h∩Ω_h. It is not an extra V_{h−1} datum in the subsequent determining set. All V_j determining fields for j≥h may consequently remain the reference chain. The microscopic field after inserting the seed is of course different, and a transported microscopic mark must still be evaluated on that field.

## 3. Matching all ancestors in the literal rectangular-chain preparation

Fix an actual history producing r. The relevant source operation is the one in LFR I pp.195–196: for one final component it has one nested sequence of inner rectangular parallelepipeds, including a single rectangle Z″_{h+1}. This is more specific than eventual smallness of Λ or absence of new P/Q/R tests. The proof uses that literal inner-chain property and does not infer it for an unspecified forest preparation.

Here is the bounded-ancestor argument of Lemma MW.1 in [residual merger witness](residual_merger_witness.md). In common current physical units put a_j=L^{j-k}MR_j, and let C_h be the next-grid cover of **all** h-scale ancestors of Y. The one-step rounded radius comparison gives a_{h+1}/a_h≤K_R, with K_R=L² sufficient at weak coupling. The quiet ordinary geometry and LFR I (1.11) give

\[
 C_h\subset C_h^{+3}\subset A:=Z''_{h+1}
              \subset C_h^{+8}\subset Z_{h+1}\cap Y.
 \tag{RT.8a}
\]

Only these inclusions are used: erosion of an enlarged arbitrary union is not asserted to undo the enlargement. The rectangle A is connected, contains every h ancestor, and is contained in one actual h+1 component. The eligibility bound for that component gives a containing cube of side 100a_{h+1}. Hence the total number of h-region cubes in the ancestral union is at most

\[
 J_*=(100K_R+2)^4.
 \tag{RT.8b}
\]

Reproduce **every** original rectangular h component by the strict R seeds of Section 2, one in each cube of its one-layer erosion. This preserves the entire union Z_h∩Y exactly; it does not replace a union by its hull. There are at most C J_* seeds and their total birth energy is C J_*P(g_k)²+C J_*. Keep the original deterministic cover, padding, hull operations and all source preparation choices during the quiet window. Since their initial set is unchanged, every later set is unchanged, including any merger. The preparation therefore gives exactly the same Λ, Y and cutoff ζ. Choose the same G, anchors, orientation and all other fresh features. The fresh homogeneous reference and h/H factor are consequently identical. This is Theorem MW.2's same-r trial.


The updated determining sequence is the one meant here. Interior histories erased by an earlier R operation are not reinstated. The construction uses h≥1. In the source's homogeneous Wilson initialization this is automatic for a nonempty eligible component: there is no preexisting nonempty T₀ core, and the labels P₀,P₁,Q₁,R₁ are all created by the first transformation. A nonempty component at k≤N therefore cannot have had N preceding transformations with no birth. An externally prescribed initial bad core would require a separate base case.

## 4. An identity-centered box after the actual classical cancellation

At the fixed current shell the actual source reference is

\[
 U_0=U_{k,Y}(V_\Lambda)
 \tag{RT.9}
\]

from LFR I (1.77)–(1.79). It depends on the shell, not on an old continuous integration variable. Use the source AL representative of (1.86)–(1.87). Its potential obeys |A₀|+|∇A₀|≤C_Mε_k on the prepared core.

The positive Wilson term finally retained in (1.71) is **not** the Wilson action of the original reference-centered mixed field. LFR II p.368, (1.46), factors off the A₀-dependent perturbation, and (1.48) leaves the real field

\[
 U''_{h+2}(\exp(i g_kB),V'')
 \tag{RT.9a}
\]

in the positive action. Its reference A₀ is absent; those terms have been estimated and included in the self interaction, as stated after (1.48). On a fresh R-only branch there are no old determining data at scales j<h inside this core, so V″ there consists only of V_h. Set

\[
 B=0,\qquad V_h=I.
 \tag{RT.9b}
\]

All the determining data of (RT.9a) are then identity. Its unique regular minimizing field is identity, hence **S=0 exactly** at this center. The birth A_{h−1} is still a variable in T_h, and does not enter these determining data. It is not set to zero.

The delicate old-core selector is χh,1/2 of **(1,V_h)**. At (RT.9b) it is exactly one with full strict margin, including the artificial seam. Also χ′=1 at B′=g_kB=0. The literal source identity (1.89) therefore restores the original complete χ″k selector in the actual U₀ exterior. No assertion that the original mixed field is identity is made.

For comparison, the reference-centered alternative would also have been admitted: its AL representative gives

\[
 |V_h-I|\le C_M L^{h-k}\varepsilon_k.
 \tag{RT.10}
\]

This is the source average estimate applied to (1.92); compare CMP98 Proposition 6, (164). Filling the old hole by identity preserves this link bound, including at the artificial seam. The local variational map near identity gives

\[
 \sup_p|U_{h,\Box}((1,V_h);\partial p)-I|
 \le C_M L^{-N}\varepsilon_k\,(L^{k-h}\eta)^2
 <\tfrac14\varepsilon_h\,(L^{k-h}\eta)^2.
 \tag{RT.11}
\]

The last inequality uses εk/εh≤C√N and N large. Cubes entirely in the filled region are flat. This is the B′=0 mechanism in LFR I (1.94), but the actual trial below uses the simpler identity center (RT.9b). An R-only birth leaves V_h unchanged, so it does not change either seam argument.

For a quantitative positive-volume event, use the independent source coordinates at (RT.1), after the exact preparation transformations. Let

\[
a_N=c\,g_k^{c_0}\,[C_0(1+R_k)^{c_1}]^{-c_2(N+1)}.
 \tag{RT.12}
\]

Put each independent B coordinate in an aN ball about zero, each raw old V_h coordinate in a Haar-coordinate ball of physical radius g_haN about identity, and each birth free A coordinate in an aN ball about its seed or zero center. The positive fixed constants in (RT.12) are chosen large enough as follows. This deliberately crude exponential-in-age radius avoids a stronger, unnecessary polynomial-thickness claim.

Each ordinary averaging/constraint operation and its inverse in the admitted chart has a fixed derivative bound in its own normalized lattice units, by the actual local C map and CMP102 Proposition 9/(190). A local axial or mixed annular gauge transformation is a product along a path of at most C_MR_j bonds. The derivative of a product of unitary factors is bounded by the sum of its factor derivatives. Thus one step, including its gauge representative, costs at most C₀(1+R_k)^{c₁}; converting between adjacent lattice units costs only a fixed power of L. There are at most C(N+1) such transformations after the fresh birth. Their composition and inverse therefore cost at most [C₀(1+R_k)^{c₁}]^{C(N+1)}, with fixed powers of g from physical/dimensionless conversions. There is no iteration through h earlier scales: those have been integrated into the renormalized action, and the source minimizing-map bounds are independent of that depth. Taking c₂ and c₀ large enough gives a box whose image stays within every required strict margin.

Keep every literal selector radius in its actual post-scaling variable. In particular a later printed restriction |A_j|<δ_j or |B_j|<δ′_j is allowed to be smaller than one; it is not replaced by δ_j/g_j or δ′_j/g_j. Choose the fixed exponent c0>1 and the constants in (RT.12) so that, after the stated pullback/composition allowance, each aN ball is smaller than a fixed fraction of the minimum of all the actual radii and strict margins used by that coordinate. The extra fixed power of g_k in aN pays the literal δ_j=g_j times a logarithmic factor and δ′_j of the same kind. Its logarithmic volume cost is already included in RT.14. The source analytic bounds in the literal preparation coordinates, including (1.91)–(1.98), then give strict admission. The two final preparation tests are direct coordinate tests: B′ is g_kB, and the old core test sees (1,V_h). The original combined quiet tests follow from the exact implication (1.89), not from a new independent product of such tests. The remaining birth P/Q/R tests have the strict margins proved in Lemma RT.1. The larger composition allowance also pays their pullback to the actual background used in T_h. This box calculation does not settle the distinct complete unmarked source estimates under every literal cutoff convention.

This argument only needs a controlled exponential-in-age distortion. Its logarithm is O(Nlog(1+R)+log g⁻¹), so it does not introduce an exponential-in-age entropy exponent. It would fail if an unrecorded pre-h coordinate chain were reconstructed; that is why the fresh birth and the final-coordinate representation matter.

## 5. Counts and the normalization terms

For the fresh-birth trial there is no local pre-birth history. The birth at operation h does retain its actual A_{h−1} coordinate in T_h; it is included in the count. At each of h,…,k, its actual region fits in the source cube of side 100MR_j in that scale. Hence

\[
 D_{\rm tr}\le C_M\sum_{j=h-1}^{k}R_j^4
              \le C_M R_k^5.
 \tag{RT.13}
\]

This counts each coordinate in the final prepared representation once: the old core V_h, its unchanged T_h birth factor, and B₀ minus its literal tree. Coordinates already integrated into E/R/B or normalization constants are not reintroduced.

The coupling comparison on this N=O(R_k) interval makes g_j/g_k and R_j/R_k uniformly comparable after reducing the common weak-coupling ceiling. Thus the selected coordinate-box volume, including the exact physical g factors where they actually occur, has logarithmic loss at most

\[
 C D_{\rm tr}[(N+1)\log(1+R_k)+\log g_k^{-1}]
 \le C_M\{R_k^6\log(1+R_k)+R_k^5\log g_k^{-1}\}.
 \tag{RT.14}
\]

On a factor whose actual dimensionless cutoff contains a fixed-radius ball, such as the broad initial j=0 free factor, normalizing its Gaussian first makes that box cost exp(−CD). This optional improvement is not available for every literal later shrinking cutoff. The weaker (RT.14), with aN chosen below every literal radius as above, is already sufficient. To make its counting unambiguous, use the following assignment: the B integral dB σ(g_kB)δT contributes at least (c aN)^{D_B}; its g_k^{D_B} factor is kept only in (RT.2). The raw V_h Haar balls contribute at least (c g_h aN)^{D_V}. The ordinary birth free A balls contribute at least (c aN)^{D_A}; their displayed normalization constants remain with the source normalization terms. Local coarea/coordinate Jacobians on the admitted small chart have per-coordinate bounds e^{±C}; their log cost is included once. This convention does not count a second g_k^{D_B} in the B-box volume.

The pre-h density is not the probability that an exponentially large microscopic volume was entirely good. The trial is a term of the already renormalized action at its birth. CMP119 pp.263–264, (2.43)–(2.49), bounds the full E/R/B remainder and vacuum counterterm in absolute value by the actual determining-volume sum, with the coupling logarithms displayed separately. LFR II p.380 applies these bounds to precisely the non-Wilson/nonquadratic exponents of (1.71): every actual large-field domain Z_j costs at most C|Z_j|log g_j⁻². Applied to this fresh-birth branch, that yields

\[
 |V_\gamma^{\rm self}+C_\gamma^{\rm norm}|
 \le C_M R_k^5\log g_k^{-1}
 \tag{RT.15}
\]

with the explicit diagonal factor (RT.2) included here, rather than in the Lebesgue B-box volume. This is a two-sided exponent estimate, since the source inequalities are absolute bounds; their use is not limited to an upper bound for the full integral.

There is a useful exact collar check. The prescribed component is contained in a neighborhood where Ω_h is full in the fresh R-birth branch, so Γ_j vanishes there for j<h. Moreover the fixed current-M collar of Y lies in Ω_k: Z_k=Λ_k^c already contains the two MR_k buffer layers outside Ω_k^c. This collar can therefore contribute current-scale volume, but cannot import arbitrary pre-h exterior determining counts into (1.69). Terms reaching another component are cross terms and remain in (RT.4).

Equivalently, combining the box coordinate volumes and the actual nonenergy density **once**, their restricted integral is at least

\[
 \exp\{-C_M[R_k^6\log(1+R_k)+R_k^5\log g_k^{-1}]\}.
 \tag{RT.15a}
\]

Here the measure includes the exact Haar/coarea factors and the two E_k terms and diagonal normalization of (1.71). Positive quadratic and Wilson energies have not yet been included. Equation (RT.15a), rather than two independent extra Gaussian normalizers, is the quantity used below.

## 6. The lower self-mass estimate

On the box, the old birth quadratic forms have total energy at most CP(g_h)²+CDtr, by the uniform upper precision bound and the bounded number of seeds. For the outer preparation quadratic keep a separate geometric count

\[
 D_{\rm geo}:=\sum_{j=h}^k
     \frac{\operatorname{Vol}(\text{actual }j\text{-scale region})}
          {\ell_j^4}
       \le C_M R_k^5,
 \tag{RT.15b}
\]

where ℓj is that scale's spacing in the common physical units. No equality with the post-tree independent-coordinate rank is presumed. Sum the per-scale derivative row bounds of CMP102 Proposition 9/(190) before using any extra decay. On a region of scale j they give the conservative estimate |DH B|≤C(1+N)aN ℓj⁻². Therefore

\[
 Q\le C(1+N)^2a_N^2D_{\rm geo}\le C D_{\rm geo}.
 \tag{RT.15c}
\]

This is the actual D*ζD form in LFR II (1.20)–(1.21), with 0≤ζ≤1. It requires neither a determinant lower bound nor a count equivalence between Dgeo and Dtr.

The remaining positive Wilson term S is exactly zero at (RT.9b), as proved from (1.46)–(1.48). Every determining link of its minimum on the box is either exp(i g_kB) or V_h, hence differs from identity by at most Cg_haN. The mixed determining plaquettes in CMP102 (7) contain only a fixed number C_L of such links, including interface links; their regularity parameter is therefore ε₁=C_Lg_haN. The actual variational Theorem 1, (8), or Proposition 9 at identity, gives on a region of determining scale j≥h

\[
 |U(\partial p)-I|\le Cg_ha_N(\eta/\ell_j)^2.
 \tag{RT.15d}
\]

The square of this plaquette factor cancels the fine plaquette count in four dimensions. The inner ζ₁ support has at most C_MR_h⁴ h-scale sites, and there is no older Γ_j in this trial. The inverse coupling on this branch is at most Cg_h⁻²: it has already run regularly through h−1, and the remaining N+1 couplings are comparable. Thus S≤CaN²R_h⁴≤C Dgeo. No full-cutoff ε_h estimate, and hence no R⁴P² loss, is used. Consequently

\[
 Q+S+\mathcal G\le C P(g_k)^2+C(D_{\rm tr}+D_{\rm geo})
 \quad\hbox{on the trial box}.
 \tag{RT.16}
\]

### Proposition RT.2 — trial lower mass on the literal prepared scope

For every complete fresh-reference class of the literal rectangular-chain prepared operation specified in Section 3, under the inherited source coupling/domain assumptions,

\[
 \boxed{\quad
 \mathcal M^{\rm self}_{r,v}(1)
 \ge \exp\{-C[P(g_k)^2+R_k^6\log(1+R_k)
                            +R_k^5\log g_k^{-1}]\}.
 \quad}
 \tag{RT.17}
\]

**Proof.** By MW.1–MW.2 and Section 3, restrict the positive history sum to the fresh R births reproducing all h ancestors, their unchanged later geometry, and the same-r finite graph choices. Their number is bounded by J_*. Restrict the final independent integrals to the admitted box of Section 4. The positive energies obey (RT.16), with both counts bounded by C_*R_k⁵, and the full coordinate measure and nonenergy exponent have the combined bound (RT.15a). Multiplication proves (RT.17). The finite orientation weights and the fixed ancestor count change only C. The full upper measure and its normalization still contain all merged or arbitrarily old histories; this positive trial does not remove them. ∎

This proof uses the same post-cancellation convention as (RT.3), and no fresh reference lower bound. A common retained-only factor, if another convention retains it, must be included on both sides of the matched upper/lower pair before applying RM.1. The analyses in [residual trial box analysis](residual_trial_box_analysis.md) and [residual trial normalization analysis](residual_trial_normalization_analysis.md) check the final-coordinate box and literal selectors, the identity center of S in (1.46)–(1.48), the once-only normalization assignment, and the MW scope extension. None of those checks is replaced by an output-moment assumption.

## 7. Normalized energy/rank consequence and its scope

For reference classes in the preceding scope, the source hierarchy p₀≥5r, with positive integer r, implies both R⁵log g⁻¹=o(P²) and R⁶log(1+R)=o(P²). Indeed their logarithmic powers are respectively 5r+1 and 6r with a loglog factor, whereas 2p₀≥10r. The residual fresh selector supplies the current native witness Rout≥cP², as in AH.1. Thus the matched bounds (RT.3), (RT.17), together with RM.1, imply for the self posterior

\[
 \|1+\mathcal F+D_{\rm old}\|_{L^p(\nu^{\rm self}_{r,v})}
       \le C[p+P(g_k)^2]\le CpR_{\rm out}(v),
       \qquad p\ge1.
 \tag{RT.18}
\]

The full numerator includes arbitrary old branches; their large ranks remain paid by the actual NR20 tilted upper bound. Only the lower estimate uses a young trial. This is how a short trial can control a posterior whose support contains much older histories.

For the complete conditional, retain (RT.4). HS20.7 supplies the needed comparison in the actual component posterior: conditional on every other old component, the successful geometry and retained r, the state-dependent cross action of Y has oscillation at most Cλ_R, where λ_R=C(1+R)^bα_k and α_k≤Ce^{-cR}. For every nonnegative f, its conditional expectation is consequently at most e^{Cλ_R} times the self expectation. This bound is uniform in those other component states, and remains true after averaging them and the successful geometry. Since λ_R is uniformly small, (RT.18) holds for the complete conditional energy/rank class as well. This is a positive moment comparison, not a bound on the raw derivative of the cross action. The full cross score and physical carriers remain required for currents.

Finally, LFR II pp.379–380, (1.73)–(1.75), provides a separate relative analyticity fact. On its fixed native chart, the complete **self** integrand changes by exp σ with sup|σ| small, because only the B quadratic form and the resummed self V depend on the native pair (U,J). This comparison remains true after restricting the history sum to r. Its normalized total variation is therefore bounded independently of how small its old mass is. It is useful for native analytic source/response work, but the pullback to raw retained coordinates, moving selectors, complete cross interactions, and physical carriers remain separate tasks.

Equation (RT.18) does not alone prove M-03's exponential physical-volume carrier estimate or its discrete history currents. Its conclusion removes the logarithmic old-normalizer gap for this energy/rank class on every reference class of the literal rectangular-chain prepared operation, including merged ancestry covered by MW.1–MW.2, under the same inherited source assumptions. It does not extend the source operation to an unspecified forest of separated inner holes. Its regulator may be supplied by a witness anywhere in Y; no local core-energy moment or microscopic a⁻⁴-to-h⁻⁴ improvement follows from this total-energy statement.

## 8. Weighted native holomorphy and separate native current bounds

This is a further consequence of the matched mass estimate on its preceding geometric scope and the **relative** analytic comparison on LFR II pp.379–380. It uses the native chart exactly as the source defines it. It is not a pullback theorem for independently varied raw retained links.

Let ξ₀ be an admitted real center in one fixed-support native chart and let ξ vary on a smaller complex chart on which

\[
 \mathcal M^{\rm self}_{r,\xi}(d\eta)
       =e^{\sigma_\xi(\eta)}
                    \mathcal M^{\rm self}_{r,\xi_0}(d\eta),
 \qquad \sigma_{\xi_0}=0,\qquad
 \sup_{\xi,\eta}|\sigma_\xi(\eta)|\le\delta<\log2.
 \tag{RT.19}
\]

The literal source gives (RT.19) because only its B quadratic form and resummed self V change with the native pair; the old selectors, old operation and positive inner S have fixed arguments on this native continuation. Restricting the old history sum to r preserves the pointwise comparison. Let E≥1 be the common native old energy/rank envelope of NR20.15, with the rank store retained. By (RT.3), (RT.17), and RM.1, for K=1+P(g_k)²,

\[
 \nu_0(E>s)\le\min\{1,e^{C K-ts}\},\qquad t>0,
 \tag{RT.20}
\]

with fixed t and C. In particular, for fixed sufficiently small c>0,

\[
 \nu_0 e^{cE/K}\le C_1,
 \qquad \nu_0(Ee^{cE/K})\le C_1K.
 \tag{RT.21}
\]

To prove these estimates, dominate E in distribution by CK/t plus an exponential variable of rate t, increasing C if necessary, and integrate its exponential moments. No normalized exponential moment of order one is claimed to be uniformly bounded.

### Theorem RT.3 — weighted normalized native analyticity

Suppose the **incoming** marked function Fξ(η) is analytic on this native chart and has the explicit common bound

\[
 |F_\xi(\eta)|\le b E(\eta).
 \tag{RT.22}
\]

Then the self expectation νξFξ is analytic, and

\[
 \sup_\xi|\nu_\xi F_\xi|\le CbK.
 \tag{RT.23}
\]

The exact marked source Zξ(λ)=νξ exp(λFξ) has a nonzero analytic continuation on

\[
 |\lambda|<\frac{c_*}{bK},
 \qquad |Z_\xi(\lambda)-1|<\tfrac12,
 \qquad
 |\kappa_m^{\nu_\xi}(F_\xi)|
      \le m!(C bK)^m\quad(m\ge1).
 \tag{RT.24}
\]

For b=0 the mark is zero and the source assertion is trivial.

**Proof.** Divide (RT.19) by the positive real mass m₀. Its relative normalization satisfies

\[
 \left|\nu_0(e^{\sigma_\xi})-1\right|
        \le e^\delta-1<1.
\]

It is therefore nonzero. The normalized complex measure has the weighted domination

\[
 |\nu_\xi|(d\eta)
       \le\frac{e^\delta}{2-e^\delta}\,\nu_0(d\eta).
 \tag{RT.25}
\]

This proves (RT.23) and justifies analytic differentiation by the common integrable envelope. Moreover

\[
 |Z_\xi(\lambda)-1|
 \le\frac{e^\delta}{2-e^\delta}
        |\lambda|b\,\nu_0(Ee^{|\lambda|bE}).
\]

Use (RT.21) and choose c* sufficiently small. The stated disk is zero-free and the branch log Zξ(0)=0 is analytic with a fixed bound there. Cauchy's inequality gives the cumulant estimate. Both zero-free statements are proved from the actual relative density and energy tail; neither is an additional hypothesis about a marked numerator. ∎

### Separate direct and kernel records on an admitted native disk

Take any one native variation whose complex parameter lies in |z|<ρ inside the preceding chart, and work on the inner disk |z|≤ρ/2. Keep insertion and kernel arguments separate:

\[
 H(z_{\rm ins},z_{\rm ker})
       =\nu_{z_{\rm ker}}F_{z_{\rm ins}}.
 \tag{RT.26}
\]

Cauchy on the insertion and on σ, followed by (RT.25), gives on the real positive slice

\[
 B_z=\nu_z(\partial_zF_z),\qquad
 J_z=\operatorname{Cov}_{\nu_z}
                   (F_z,\partial_z\sigma_z),
 \tag{RT.27}
\]

\[
 |B_z|\le CbK/\rho,\qquad
 |J_z|\le C\delta bK/\rho.
 \tag{RT.28}
\]

The kernel formula retains the derivative of the normalization, through its covariance. A retained-only factor in σ cancels from J exactly. Higher native derivatives of H obey the corresponding Cauchy factorial bounds on smaller disks. For several directions, their actual native-domain radii and direction budget must be retained; no volume-free sum of raw-link derivatives is inferred just from (RT.28).

For finite real differences use the exact M.30 rectangular endpoints

\[
 B_t=\frac{H(z_t,z_t)-H(z,z_t)}t,\qquad
 J_t=\frac{H(z,z_t)-H(z,z)}t.
 \tag{RT.29}
\]

Integrating the corresponding separate derivatives along each of these two paths proves the same bounds whenever their rectangles lie in the admitted chart. This is a fixed-support native statement. Varying a raw current link can also change the reference, selectors, old S and old T coordinates; a discrete reference/history change can change the support itself. Those extra operations are not covered by (RT.19) and have not been declared controlled here. The exact cross-action comparison in Section 7 proves positive moments for the full posterior; its raw differentiated score and carrier bounds remain separate.

## Primary sources

- CMP119 (1988), pp.249, 255–258, 263–269: exact constraint/free map, determining set, old operation, absolute E/R/B and vacuum estimates, and P/Q/R geometry.
- CMP99 (1985), pp.427–428, (3.155)–(3.158): actual unit-lattice precision, free coordinates, uniform gap and exponential kernel bound.
- LFR I, CMP122 (1989), pp.177–180, 192–200, (1.2)–(1.12), (1.73), (1.76)–(1.98): literal eligible sequence, preparation variables, reference minimum, AL gauge, tree and seam cutoffs.
- LFR II, CMP122 (1989), pp.356–380 and 391–392, (1.10), (1.20)–(1.37), (1.69)–(1.75), (1.103)–(1.104): exact classical cancellation, post-cancellation positive old operation, pointwise normalization level, and residual boundary quotient.
- Annex BJ, NR20.1–NR20.18: the already established unnormalized old energy/rank reserve and its native envelope.
