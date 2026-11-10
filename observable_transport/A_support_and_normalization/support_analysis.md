# M-04 support and ambient-current analysis

Scope: the original M-03 norm and the actual scalar regular-step output. The default inactive-fiber extension in M.1 already obstructs the requested M-04 bound at a first regular step. This is a statement about that chosen ambient version. M.1 explicitly permits a documented better extension; the repaired-version M-04 problem remains open.

## 1. Exact definitions that matter

The main mathematical construction, Annex Y, fixes the following conventions.

1. The ambient state is a product of retained raw continuous and discrete history coordinates, M.1. Primitive chart formulas are zero-extended where they have no meaning. A normalized conditional kernel at an inactive or zero-normalizer retained datum is assigned the reference-input point mass. Coordinate maps outside their admitted chart are assigned their old-state reference value. Generated outputs use these recursive versions.
2. M.1 also says: an actual proof using a better extension must record the choice explicitly. Thus the reference extension is the default, not an invariant physical property of Wilson conditional expectation.
3. The finite difference M.4 divides by the real increment parameter, with a supremum over all nonzero increments of magnitude at most one. M.11 takes its pointwise supremum on the ambient versions, not only almost everywhere under the physical outer law.
4. The direct and current records satisfy M.10, separately counted in M.12. Cancellation between them cannot reduce the norm.
5. The positive native regulator is finite and locally bounded on every fixed compact subset of any finite-dimensional coordinate chart at fixed cutoff. The full carrier weight M.2 is at least one.

These facts imply that the original current norm imposes a trace-matching condition across every artificial inactive/chart boundary. This condition comes before spatial localization or ultraviolet estimates.

## 2. Finite norm forces ambient continuity (proved here)

### Proposition 2.1

Let an output scalar have an absolutely convergent compatible carrier representation

\[
 A(y)=\sum_X A_X(y),\qquad \delta_{d,t}A_X=B_{X,d,t}+J_{X,d,t}.
\]

Assume its M-03 norm is finite. Fix one elementary direction and a compact portion of its coordinate curve on which all relevant native regulators are bounded. Then A is locally Lipschitz there, with a bound obtained by summing the M.11 gradient and current bounds. In particular, if A has a nonzero jump across a finite native-energy point, every compatible representation has infinite combined direct/current norm.

### Proof

For a continuous elementary direction d and t nonzero, M.10 and the triangle inequality give

\[
 |\delta_{d,t}A_X(y)|\le B_X^\natural(y)+J_X^\natural(y).
\]

At fixed cutoff the number of coordinates is finite. On a compact coordinate neighborhood every native energy in M.5 and all its unit-shift versions are bounded by a finite number R_* independent of t and X. (One may bound each carrier regulator by the full finite-cutoff list.) M.11 consequently implies

\[
 \sum_X |\delta_{d,t}A_X(y)|
 \le h^{-4}(3/2)^{3/2}R_*^{3/2}
       \sum_X\bigl[g_{h,1,X}(B)+j_{h,1,X}(J)\bigr].
\]

Because w_h(X) is at least one, the right side is bounded by the complete M.12 norm. Value convergence follows similarly from its pointwise value component. Hence the summed difference is uniformly bounded, and A is Lipschitz along the curve. If y_t tends to y_0 while A(y_t) tends to a value different from A(y_0), the difference quotient diverges, contradicting the bound. This conclusion is independent of the chosen spatial decomposition. QED.

### Corollary 2.2

Subtracting a finite scalar multiple of a continuous current scalar basis field and a constant identity coefficient cannot repair such a jump. More generally, subtracting any output with finite M-03 norm cannot do so.

The same proof applies if a jump is shared between the direct and current records. There is no need to determine in which record it occurs: finite norms of both would force continuity of their sum.

## 3. A source-specific selector-boundary test

This is the exact test to apply to the actual Wilson construction; unlike the parity model in SR20.31–34 it uses the literal hard source selectors and the original scalar.

### Source facts

- CMP119, printed p.246, (1.4), uses a hard good/bad selector on the curvature of a local constrained minimizing field determined by retained coarse links.
- CMP119, printed p.248, (1.12), identifies the constrained critical background. The page states it is a minimum of the displayed action-plus-gauge functional with strictly positive second differential. It also states that on the corresponding axial gauge subspace the critical point is that of the Wilson action alone. Do not silently replace action-plus-gauge minimality by Wilson minimality without the axial reduction.
- CMP119, printed pp.249–250, (1.14)–(1.18), solves exceptional constraints and leaves independent free-bond fluctuation coordinates. In particular (1.18) is an actual sharp free-fluctuation selector.
- CMP119, printed pp.267–270, (3.15)–(3.25), repeats this structure in a general regular step. Its (3.16) tests individual free-bond coordinates, its (3.21)/(3.23) puts bad tests in the exterior, and (3.25) keeps fixed inner free-field cutoffs.
- C7.1 supplies the actual regular conditional density on every active fixed-geometry fiber:

\[
 q_v(dA)=Z(v)^{-1}{\bf1}_K(A)e^{\mathscr L_{\rm reg}(A;v)}dA,
\]

where K is a nondegenerate fixed product of free-bond balls. Every inherited term stays in the density. The background map and exponent extend smoothly into their native buffered domain.
- The F-01 repaired scalar satisfies Tr(tilde q)=2w. Summing its local scalar stencils over the periodic lattice therefore gives a fixed nonzero multiple of the total Wilson action, up to its fixed centering constant. See Annex BK SR20.1.

### Exact finite-dimensional criterion

Suppose an allowed fixed geometry has an elementary retained-coordinate curve v(t) crossing an actual outer selector boundary at t=0, with active fibers for t>0 and inactive fibers for t<0. Suppose the native q_v and microscopic pullback extend continuously to v(0) through the buffer. Let A_ref denote the reference input prescribed by M.1, and let F be a centered scalar insertion or finite sum of such insertions. Define

\[
 \Delta_F=\int F(U(A,v(0)))q_{v(0)}^{\rm native}(dA)
          -F(U(A_{\rm ref},v(0))).
\]

If \(\Delta_F\ne0\), the default ambient version of the scalar output has a jump and violates Proposition 2.1. Its M-03 remainder cannot have a finite bound after continuous scalar/identity extraction.

This statement is an immediate exact consequence of the default reference-kernel rule; it does not invoke a probabilistic smallness estimate for the inactive sector. A zero probability boundary is enough because M.11 uses an ambient pointwise supremum.

### The primitive branch denominator, before cancellation

The relevant density for a fixed all-regular live history h is

\[
 r_h(A,v)={\bf1}_{\{h\}}\,\chi_1(v)\,{\bf1}_K(A)
                 e^{\mathscr L(A;v)}
\]

times strictly positive retained-only factors, with any such factors left in both numerator and denominator. Consequently its literal conditional denominator is

\[
 Z_h^{\rm branch}(v)=\chi_1(v)\int_K e^{\mathscr L(A;v)}dA.
\]

On active fibers, χ1 cancels and one obtains C7.2. On the other side of the selector the branch denominator is zero. M.1 explicitly chooses the reference point mass on an inactive **or** zero-normalizer datum. Continuing the canceled ratio smoothly across the zero is a possible better extension, but is different from the default version. This is why an outer selector cannot simply be ignored in an argument about the ambient supremum.

### A primary-source proof that the retained coarse selector has a boundary

No transversality assumption or numerical minimizer computation is needed. Bałaban, CMP98, printed pp.25–26, Proposition 1, (50)–(51), proves the local estimate

\[
 \|\overline U(\partial p')-I\|
 \le L^2a+C_0(L^2a)^2,                                    \tag{SA.1}
\]

where a bounds the fine plaquette curvature on the fixed local block stencil surrounding the coarse plaquette p'. Its locality is explicit. The required block stencil is contained in a source test cube with its prescribed large collars. The determining-set constraint in CMP119 (1.2), and the precise inner determining region in (2.11), identify the average of the local minimizing field with the specified retained field V on that inner coarse plaquette.

If the all-good selector χ1 in CMP119 (1.4) held, the fine bound would be a<r=ε1 L^{-2}. Equation (SA.1) would imply

\[
 \|V(\partial p')-I\|<\varepsilon_1+C_0\varepsilon_1^2.
                                                               \tag{SA.2}
\]

Now keep every retained coarse link equal to the identity except one, and choose its small one-parameter pulse so that the curvature of an adjacent coarse plaquette has norm 2ε1. Such a pulse exists in every SU(N), N≥2, by taking a nonzero generator in an SU(2) subgroup. For C0ε1<1, (SA.2) is impossible. Hence this endpoint is outside the all-good sector. The entire one-link path lies inside the larger geometric minimizing-field chart for sufficiently small admitted coupling; its endpoint amplitude is O(ε1).

At the identity, χ1=1. The finitely many tested minimizing-field curvatures are continuous along the path. Let t* be the first parameter where their maximum reaches r. Then every earlier point is active, and at t* the strict good-field inequality is false. Thus χ1(V(t*))=0 exactly, while V(t_n) tends to V(t*) through active configurations. This one inactive equality point is sufficient for the divided finite-difference obstruction. No open inactive interval, regularity of a selector level surface, or nonzero derivative of its maximum is required.

The elementary M.3 parameter differs from this raw one-link parameter by the fixed finite factor sqrt(1+β_e). Both tend to zero at the boundary, so the divergence of the difference quotient is unchanged.

The support check uses the source's parameter order. In its first-step convention the physical fluctuations on K are O(δ0), with δ0/ε0=A1/A0 small. The source chooses A0 sufficiently larger than A1 and proves on CMP119 pp.248–251 that the earlier curvature/gauge and approximate-fluctuation selectors are identically one on the regular free-field domain. Their strict margin persists at the coarse χ1 boundary; this selector changes the retained outer history, not K. The same first-step bounds put all fine curvature and covariant-divergence quantities in the fixed geometric variational class: their sizes are O(C(L)(ε1+δ0)) and tend to zero as the admitted coupling tends to zero. This checks both parts of the regular class in CMP102 p.278, (2), rather than checking curvature alone. The source-admitted label comparison ensures the O(ε1) coarse path also stays inside the earlier, weaker coarse bound 2L²ε0. A different proposed running-label convention must supply that overlap explicitly.

### Theorem 3.1 (actual first-step obstruction for the default version)

Fix SU(N), N≥2, an admitted source block integer and a sufficiently large compatible finite periodic torus. Use the original compact Wilson scalar, the first all-regular source history, its exact regular conditional kernel, and the default inactive-fiber reference version of Annex Y M.1. For sufficiently small admitted coupling, at least one nonzero normalized local scalar has an output QF_x whose combined direct/current M-03 norm is infinite. Subtraction of a field-independent scalar coefficient times the current compact scalar basis and a constant identity coefficient leaves this obstruction.

### Proof

Choose the retained coarse-link path and first inactive boundary v*=V(t*) just constructed. On active fibers the exact conditional density is the fixed positive product-domain density q_v. The primitive branch denominator is χ1(v)Z(v), so at v* it is zero and M.1 assigns the reference input. In the common fluctuation coordinates of C7.2 this is δ_{A=0}. The native reconstruction remains within its buffered chart at this point, hence A=0 reconstructs the constrained Wilson background U1(v*), not an unrelated field. If the reference rule is instead applied before this pullback in the old raw compact-link coordinates, its reference is the entire identity configuration; the final paragraph below handles that convention too.

The native density and microscopic reconstruction are continuous up to v*. K is bounded with compact closure inside the native chart at fixed coupling, its measure is nonzero, and the density is strictly positive. Its native normalizer remains positive. Dominated convergence therefore gives the one-sided limit

\[
 \lim_{n\to\infty}QF_x(v_n)=q_{v_*}^{\rm native}F_x,
 \qquad QF_x(v_*)=F_x(U_1(v_*)).                            \tag{SA.3}
\]

CMP119 p.256, (2.12), identifies the background with the set of Wilson minima on its regular fixed-average fiber. CMP102 pp.278–281, (2)–(6), Theorem 1 and the axial reduction establish the physical Wilson minimal orbit; this is stronger than minimality of the soft-gauge augmented functional. The support check above puts the entire chosen K inside that regular fiber. Thus

\[
 S(U(A,v_*))\ge S(U_1(v_*))
\]

on K. There are non-gauge physical fluctuation directions: the independent fine free-bond space in a block has positive-dimensional curvature directions after the coarse constraints and center-fixed gauge directions are removed. The constrained positive quadratic form, CMP102 p.299, (141)–(142), gives strictly larger action on a nonempty open subset of K. One may also count dimensions: for n_f fine and n_c coarse sites, exceptional-bond elimination leaves 4(n_f−n_c) Lie-algebra directions, of which n_f−n_c are center-fixed gauge directions. The remaining 3(n_f−n_c)(N²−1) real directions are nonzero because L>1. Exact positive Haar/coarea/gauge weights give the larger-action open set positive conditional mass. Therefore

\[
 q_{v_*}^{\rm native}S-S(U_1(v_*))>0.                       \tag{SA.4}
\]

For the actual F-01 scalar σ_h=2w_h/sqrt(6), the exact stencil identity is

\[
 h^4\sum_x\sigma_h(x)=\frac2{\sqrt6}S(U).
\]

With F_x=αβσ_h(x)−c and α nonzero, (SA.4) implies the following identity. For the fixed incoming F-01 scalar coefficient take α=z_S^{in}/β; no running normalization bound is needed.

\[
 h^4\sum_x\bigl[q_{v_*}^{\rm native}F_x-F_x(U_1(v_*))\bigr]
 =\frac{2\alpha\beta}{\sqrt6}
       [q_{v_*}^{\rm native}S-S(U_1(v_*))]\ne0.             \tag{SA.5}
\]

Hence at least one local scalar has a nonzero jump in (SA.3). In the raw old-state reference convention, replace S(U1(v*)) by S(I)=0; the positive-measure physical fluctuation set has strictly positive Wilson action, so the same nonzero total scalar mismatch follows directly from S≥0. Thus the conclusion is unaffected by these two implementations of the reference input. Its native regulator is finite at v* and on its unit-shift neighborhood because the cutoff, torus and coordinate list are finite. Proposition 2.1 gives an infinite combined gradient/current norm for every compatible representation. The current scalar is a continuous compact-link function, independent of auxiliary history labels under M.1, and the identity is constant. Corollary 2.2 proves the assertion after scalar/identity subtraction. QED.

This theorem uses a first-step all-regular history, so it needs no unproved repeated-history localization, residual-component mass estimate, or all-scale coupling-flow theorem. It is a failure of the chosen off-support reference version, not a counterexample to Yang–Mills existence or to a possible smoothly extended M-04 theorem.

### Wilson action-gap verification

On a constrained axial fiber for which the Wilson background is a strict local minimum on the entire selected fluctuation domain,

\[
 S(U(A,v_0))\ge S(U(0,v_0))
\]

with strict inequality on a positive-measure set of physical fluctuations. The exact density is positive on that set. Consequently

\[
 \int S(U(A,v_0))q_{v_0}(dA)-S(U(0,v_0))>0.
\]

The same conclusion holds before gauge restoration if the center-fixed gauge transformation preserves the blocking constraint and Wilson action and sends the soft-gauge fiber to the constrained axial fiber. This must be checked for the selected native convention. Gauge directions alone give equality, but the product domain contains physical curvature directions; one nonempty physical direction is enough for strictness.

The centering constant cancels in this difference. Hence a nonzero multiple of the total scalar action has a nonzero jump. Since a finite sum of continuous functions is continuous, at least one local scalar insertion has a nonzero jump. A uniform local-scalar theorem would fail for that insertion in the default version.

The retained coarse link in this proof is an actual output coordinate, so no assertion about a retained exterior variable is needed. The first-equality argument also avoids any smoothness assumption on the maximum defining χ1.

## 4. Removing the artificial jump without changing the physical law

The default-version issue is repairable under the explicit permission in M.1 to record a better extension. Such a repair is useful but does not prove the full M-04 bound.

### Proposition 4.1 (a fixed-geometry positive extension)

Let D be the active retained chart and suppose its closure lies in a native buffered chart D+. Let q_v be a continuously differentiable positive normalized conditional density on a fixed integration domain K throughout D+. Choose a smooth cutoff χ, equal to one on a neighborhood of the closure of D, supported inside D+, with 0≤χ≤1. Let q_* be a fixed probability measure on K. Define

\[
 q_v^{\rm ext}=\chi(v)q_v+(1-\chi(v))q_*.
\]

Outside D+ use q_*; χ vanishes before that boundary. Then this is a globally positive normalized kernel agreeing with the actual kernel on D. Its derivative is

\[
 Dq_v^{\rm ext}=\chi(v)Dq_v+(D\chi(v))(q_v-q_*).
\]

The second term is an explicit extension current. For a bounded source F its magnitude is at most 2\|F\|_∞|Dχ|. For a regulated source replace the supremum by the corresponding q_v/q_* regulator integrals. On a collar of width r in the normalized elementary coordinates the extra cost is O(r^{-1}); at fixed cutoff it is finite. The same source-free extension transports every finite source jet and preserves the original marked integrals on the physical support.

### Proof

Positivity and normalization follow from convex combination. Agreement is exact where χ=1. Differentiability follows because χ vanishes in a neighborhood of the boundary where q_v ceases to be defined. The displayed product rule proves the derivative/current formula; integration along elementary coordinate curves gives the finite-difference bound. QED.

### Locality warning and a local alternative

A cutoff χ built from the whole geometry may depend on every block. Its extension current then has a full-torus carrier and is useless for uniform M-03 estimates. Thus Proposition 4.1 is a finite-cutoff regularity repair, not a spatial estimate.

If the complete density has already been decomposed into actual local coefficients W_X, each admitting a buffered local chart and a cutoff χ_X with the same dependency footprint, one may instead extend W_X to χ_XW_X before forming the positive normalized law. This keeps the primitive carrier. A derivative of a product of O(|X|) local cutoff factors costs at most C|X|/r. For any spare carrier rate δ>0,

\[
 |X|e^{-\delta|X|}\le \frac1{e\delta}
\]

(or a harmless larger bound for integer |X|), so an extra exponential carrier reserve absorbs the polynomial overhead. A full proof still must construct these local buffered charts and account for the Gaussian, coarea, boundary and inherited coefficients. Multiplying by an unspecified global cutoff does not meet that requirement.

## 5. The independent fixed-component volume problem persists

Even a smooth ambient extension does not establish the full physical carrier norm. LFR II, printed pp.391–392, (1.103)–(1.104), integrates old fixed components and omits their internal tree costs in its relative localization norm. M-03 charges every raw retained dependency inside a component. The scalar normalized conditional quotient cancels the fixed component's common mass. Outer probability rarity cannot be used to pay the pointwise term in M.11.

The parity diagnostic SR20.31–34 correctly proves that regular moments, an integrated fluctuation gap and relative component localization do not imply the needed physical-volume bound. It is not itself a Wilson counterexample. An actual-model proof must still derive a local factorization or cancellation of the residual dependence, and must do so for the separate current records. Nothing in the extension repair establishes that factorization.

## 6. Status and useful conclusion

Proposition 2.1 and its scalar-subtraction corollary are unconditional consequences of the specified norm. Theorem 3.1 applies them to the literal first-step all-regular Wilson branch using the verified coarse-curvature inequality, primitive zero denominator, constrained Wilson minimal orbit and positive physical fluctuations. It proves failure of bounded transport for the default reference extension already at fixed cutoff. Proposition 4.1 is an unconditional positive-kernel extension lemma that explains how this artificial jump can be removed without altering physical marked integrals.

The current proof target therefore has two logically distinct obligations:

- choose and record an ambient extension whose separate currents are finite, or prove literal trace matching of the default reference extension at every inactive boundary;
- prove the actual absolute marked numerator and full physical-carrier/current sum, including residual fixed components.

The first cannot be inferred from moment/coercivity estimates on active fibers. The second cannot be inferred from a smooth extension. The original default-version M-04 estimate is ruled out by Theorem 3.1; the repaired-extension estimate is still not proved. No statement about nonexistence of the intended continuum theory follows.
