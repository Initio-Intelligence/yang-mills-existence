# Regular atlas and shrinking-domain foundation

**Current status:** A8 supplies the regular comparison requested in A7.58. T9/N9 use the admitted current response to prove the required finite magnetic jets and actual mean-metric identity. Persistent mixed-boundary admission remains open.

**Scope:** Full-torus regular source functions and frozen regular kernels admitted on the fixed domains defined below, with the source block geometry. The new construction works on nonflat regular background charts. A shrinking birth-domain obstruction for historical activities is isolated in §8; mixed regular/large-field boundaries are not included.

### 1. The change of representation

There are two different locality questions. A coefficient obtained after setting a reference field to one need not be invariant under an inhomogeneous transformation of a coarse field with that reference held fixed. That is the unresolved fixed-section question CC62. It is unnecessary for the following regular construction.

Keep source functions as functions of the **intrinsic fine background pair** \((U,J)\), as in CMP109 (1.8)–(1.19) and the birth-indexed terms in CMP119 (2.26)–(2.32). The field \(U\) remains defined on the original fine bonds. The units of \(J\), the localization blocks, and the regularity domain change with the current physical scale. Thus this representation is not obtained by freezing a reference field and subsequently forgetting its dependence.

The construction below supplies five results for this regular class. Applying it to every density in the final construction still requires the exact bulk identification in §10.5 and the mixed-boundary interfaces of Gate 3.

1. A nonflat, localized connection/current response that is exactly the identity at zero fluctuation, including off the physical current section and at arbitrary switches.
2. An intrinsically gauge-invariant normalized rooted operation on these source functions, with a fixed analytic margin and a regenerated spatial weight.
3. A classical restriction/rescaling estimate in the same intrinsic variables, proved with a mesh-uniform polynomial-jet gauge and a bounded finite-volume projection. It keeps the old fine links and rescales the independent current.
4. Classical and pure-bulk quantum maturation from a shrinking birth domain to a fixed domain, with only a fixed inverse-radius loss.
5. A common-narrow-chart estimate for the complete regular \(R\)-potential and a graded-age feedback bound, including the four-dimensional birth-root density conversion.

The distinction between these intrinsic functions and chart-dependent coarse localizers is essential. A family of unrelated local decompositions in different reference charts would not prove this result.

### 2. Units, local domains, and the source norm

Fix the original fine physical spacing \(a\). At step \(k\), let

\[
h_k=L^ka,\qquad \xi_k=a/h_k=L^{-k}.
\tag{A7.1}
\]

The source coordinate is \(x/h_k\). The underlying bond variable \(U_b\) is unchanged when units change. The current is a dimension-three variable, so

\[
J_k=L^{-3}J_{k+1}.
\tag{A7.2}
\]

This formula concerns the same physical current written in different units. It is also the prescribed rescaling of the independent current variable in the analytic extension.

#### 2.1 A strengthened local orbit domain

Fix \(0<\beta<1\). Use a smaller open domain inside the source's regular orbit domain, with a fixed margin. Retain the source global compatibility conditions for the reference and relative fields; the following local regularity conditions do not replace them or assert a new local-to-global gluing theorem. On every fixed-size current-scale coordinate patch, require a real reference representative

\[
\bar U=\exp(i\xi_k A_0),\qquad
\|A_0\|_{C^{1,\beta}}<b_0,
\tag{A7.3}
\]

and a complex relative field

\[
U=\exp(i\xi_k a_1)\bar U,\qquad
\|a_1\|_{C^{1,\beta}}<b_1,\qquad
\|J_k\|_\infty<\gamma.
\tag{A7.4}
\]

The Hölder norm uses current physical distances. Local patches and protective collars are fixed multiples of the localization block size. Equivalent covariant norms may be used; their equivalence constants are fixed by \(b_0,b_1\) and the patch geometry. Take the union of the complex gauge orbits of these pairs. Denote this domain, restricted to a protected support \(X\), by \(\mathscr D_k(X)\).

The constants are chosen so that (A7.3)–(A7.4) imply the smaller versions of CMP109 conditions (i)–(iii). The paragraph following its definition proves that these smaller constants also imply condition (iv). The new Hölder condition only restricts the domain further. Actual regular minimizing backgrounds satisfy the required local Hölder bounds by CMP102 Theorem 1, (9), with a fixed choice of its patch size; the weak-coupling threshold puts them strictly inside (A7.3).

For finite lattices these are open finite-dimensional complex domains. Holomorphy and directional Cauchy estimates therefore have their usual meaning. A support-independent margin is part of the definition; no ball of radius decreasing with the number of fine bonds is used.

The domains are gauge-orbit domains, not small-link balls held at one fixed gauge. Invariant functions may therefore be evaluated after a local axial gauge change. This is not a Haar average of functions outside their domains.

#### 2.2 Intrinsic local families

A rooted source is represented by

\[
f_k(U,J_k)=\sum_{X\ni x}f_{k,X}(U|_X,J_k|_X),
\tag{A7.5}
\]

where every coefficient is intrinsically gauge invariant and holomorphic on \(\mathscr D_k(X)\). All stencils and the fixed protective collar are included in \(X\) once. Let \(n_k(X)\) be its current localization-block count. Define

\[
\|f_k\|_{k,\kappa,x}
=\inf\sum_{X\ni x}e^{\kappa n_k(X)}
\sup_{\mathscr D_k(X)}|f_{k,X}|.
\tag{A7.6}
\]

The infimum is over intrinsic representations of the form (A7.5). It is not over decompositions defined only at independently chosen fixed reference sections. The distinction prevents nonlocal dependence on a hidden reference from being counted as local dependence on \(U\).

At each finite cutoff the sum may first be taken finite. The exponential norm then gives absolute convergence and permits passage to completed families.

### 3. The nonflat constrained equation

This section uses the old current units, so the averaging scale is one and the fine mesh is \(\eta\). Let \((U_0,J_0)\) be an admitted source background pair. The current \(J_0\) is independent on the analytic atlas. On the physical section it equals the source current of \(U_0\).

On the physical section, \(\Delta\) is the unprojected Wilson quadratic operator at \(U_0\), and \(A^{(2)}\) is the constraint-Hessian correction in CMP102 (79), (127). Off that section, all these symbols denote the **source analytic extensions as functions of \(U_0,J_0\)**. CMP109, p.261, replaces the physical second-difference current in the propagator construction by the independent variable. An unmodified raw Wilson Hessian on an arbitrary \(C^{1,\beta}\) field is not being substituted for that extension. Set

\[
\begin{aligned}
\mathcal L&=\Delta+DRD^*,&
G_0&=(\mathcal L+\mathfrak a Q^*Q)^{-1},\\
W_0&=(QG_0Q^*)^{-1},&
H_0&=G_0Q^*W_0,\\
C_0&=G_0-G_0Q^*W_0QG_0,&
\Delta_c&=W_0-\mathfrak a I.
\end{aligned}
\tag{A7.7}
\]

Here \(\mathfrak a>0\) is the fixed averaging penalty, distinct from the microscopic spacing \(a\) in §2. Stars are bilinear transposes with the normalized fine and coarse pairings, analytically continued. They are not complex conjugations of switch variables. The operator \(C_0\) is the constrained inverse with the coarse condition imposed; it is not the Landau-projected covariance denoted by a different symbol in CMP99.

For the actual minimizing solution in the linearized constraint coordinate, CMP102 (127) gives

\[
J_0+(\Delta-A^{(2)})A'+V'(A')=Q^*\Lambda,
\qquad QA'=B.
\tag{A7.8}
\]

There is no extra gauge multiplier in this equation: the argument preceding (127) extends stationarity from the Landau slice to every variation with \(Q\delta A'=0\). The actual representative still obeys the Landau condition, allowing \(\Delta\) in (A7.8) to be replaced by \(\mathcal L\) when the constrained inverse is applied.

If the reference is itself a minimizing background for these constraints, CMP102 (178) implies

\[
C_0J_0=0,\qquad
J_0=Q^*\Lambda_0,\qquad
\Lambda_0=H_0^*J_0.
\tag{A7.9}
\]

The coarse constrained inverse therefore yields

\[
\begin{aligned}
A'&=H_0B+C_0A^{(2)}A'-C_0V'(A'),\\
\Lambda&=\Lambda_0+\Delta_cB-H_0^*A^{(2)}A'+H_0^*V'(A').
\end{aligned}
\tag{A7.10}
\]

This is the nonflat counterpart of CP13. It is equivalent to the alternative source equations (179)–(180) on their physical minimizing section. It is not inferred by treating the gauge-extended quadratic operator as the unprojected operator.

The source estimates needed for these equations are

\[
\|A^{(2)}A'\|_3\le C\alpha\|A'\|_{C^1},
\quad
\|V'(A')\|_3\le C\|A'\|_{C^1}^2,
\tag{A7.11}
\]

and their analytic Lipschitz versions. The first estimate is CMP99 **(3.137)**; the second is CMP102 Proposition 4, (97)–(98). The operator bounds for (A7.7) are the corresponding source bounds for the unprojected inverse and averaging operators. The current-unit factors are one in the full-torus specialization, independently of the number of fine bonds.

### 4. The base-preserving current extension

#### 4.1 Why a direct nonflat use of CP20 is insufficient

Away from the physical section, \(J_0\) need not belong to \(\operatorname{Ran}Q^*\). A direct multiplier formula at zero fluctuation would give \(Q^*H_0^*J_0\), which need not equal \(J_0\). This could create an order-one difference in an insertion even when the fluctuation parameter is zero. It would invalidate the required \(g_kr_{\chi,k}\) quantum smallness.

The extension below corrects this exactly. The correction changes only the off-physical analytic extension; on every physical minimizing reference it vanishes by (A7.9).

#### 4.2 Definition with common switches

Localize all operators in (A7.7), the operator \(A^{(2)}\), and the source's rearranged analytic force with one common system of geometric switches. Use the same complete-force convention as CP14: after switching, one uses the bounded source formula rather than differentiating a newly switched action and appealing to inverse identities that may no longer hold.

The source includes the coarse inverse in its random-walk/operator-localization class. Products and the \(A^{(2)}\) insertion have the tree localization described after CMP99 Theorem 3.14. Thus, for a fixed complex switch radius and sufficiently small fixed \(\alpha\), the switched bounds remain

\[
\begin{aligned}
&\|H_{0,s}b\|_{C^{1,\beta}}+
 \|C_{0,s}F\|_{C^{1,\beta}}
 \le K_s(\|b\|+\|F\|_3),\\
&\|H_{0,s}^*F\|+\|\Delta_{c,s}b\|
 \le K_s(\|F\|_3+\|b\|),\\
&\|A^{(2)}_s A'\|_3\le K_s\alpha\|A'\|_{C^1}.
\end{aligned}
\tag{A7.12}
\]

Define

\[
\begin{aligned}
A'_s&=H_{0,s}B+C_{0,s}A^{(2)}_sA'_s-C_{0,s}V'_s(A'_s),\\
A_s&=A'_s-H_sD_s(A'_s),\qquad U_s=e^{i\eta A_s}U_0,\\
\Lambda_{0,s}&=H_{0,s}^*J_0,\\
\delta\Lambda_s&=\Delta_{c,s}B-H_{0,s}^*A^{(2)}_sA'_s
                    +H_{0,s}^*V'_s(A'_s).
\end{aligned}
\tag{A7.13}
\]

For \(B\) in one fixed small complex ball, the first equation is a contraction on \(\|A'_s\|_{C^{1,\beta}}\le C_s\|B\|\). The linear perturbation has size \(O(\alpha)\); the nonlinear force has Lipschitz constant \(O(\|B\|)\). Choose \(\alpha\) first, then the radius of \(B\), after fixing the switch radius. The source's estimates then prove

\[
\|A'_s\|_{C^{1,\beta}}+\|A_s\|_{C^{1,\beta}}
 +\|\delta\Lambda_s\|
\le C_s\|B\|.
\tag{A7.14}
\]

In particular all three quantities vanish at \(B=0\), for **every** admitted switch configuration. This remains true for arbitrary independent \(J_0\) in the source atlas.

Let \(\mathcal E_A\) be the differential of the exponential in CP16, and let \(Q+\mathcal C'(A)\) be the differential of the actual nonlinear averaging map at \(A\). Define the current by

\[
\boxed{
\mathcal J_s
=J_0+
(\mathcal E_{A_s}^*)^{-1}
\bigl(Q+\mathcal C'(A_s)\bigr)^*
(\Lambda_{0,s}+\delta\Lambda_s)
-Q^*\Lambda_{0,s}.
}
\tag{A7.15}
\]

The local evaluator \(Q+\mathcal C'(A_s)\) is not a second derivative of \(A_s\). The final two terms at \(A_s=0\), \(\delta\Lambda_s=0\) cancel exactly. Thus

\[
\boxed{\mathcal J_s(0)=J_0.}
\tag{A7.16}
\]

To bound the difference, write it as

\[
\begin{aligned}
\mathcal J_s-J_0
={}&\left[(\mathcal E_{A_s}^*)^{-1}
(Q+\mathcal C'(A_s))^*-Q^*\right]\Lambda_{0,s}\\
&+(\mathcal E_{A_s}^*)^{-1}
(Q+\mathcal C'(A_s))^*\delta\Lambda_s.
\end{aligned}
\tag{A7.17}
\]

The bracket has norm \(O(\|A_s\|_{C^1})\). The averaging-derivative adjoint is uniformly bounded by the normalized kernel estimate CMP102 (72), and \(\|\Lambda_{0,s}\|\le C_s\|J_0\|_3\). Therefore

\[
\boxed{
\|A_s\|_{C^{1,\beta}}+
\|\mathcal J_s-J_0\|_3\le C_s\|B\|.
}
\tag{A7.18}
\]

The fine-volume factor in \(H_0^*\) cancels the fine-site count. In the averaging adjoint, a fixed fine bond is incident to only a fixed number of coarse averaging blocks. Consequently neither part introduces an ultraviolet power.

#### 4.3 Exact physical identity

At \(s=1\), when \(U_0\) is an actual minimizing reference and \(J_0\) its physical current, (A7.9) removes the correction \(J_0-Q^*\Lambda_0\). Equations (A7.10) and the same chain rule as CP17–CP19 give

\[
\mathcal J_1(B)=J(U_1(B)).
\tag{A7.19}
\]

This is literal in the Landau representative. The axial representative gives the same value for an invariant joint insertion after transforming both variables together. At zero fluctuation, the background \(U_{k+1}\) in a regular RG step is a minimizing field also for the old averages \(M_k(U_{k+1})\); source CMP109 (2.3) and its following saddle-point construction identify this physical section.

For independent \(J_0\), (A7.15) is an analytic extension. No physical-current identity is asserted there, and none is needed for estimates of a holomorphic insertion.

### 5. Fixed analytic margins under one regular step

Take an output pair in \(\mathscr D_{k+1}\). In the old units its local potential and independent current are

\[
A^{\rm old}(x)=L^{-1}A^{\rm new}(x/L),\qquad
J^{\rm old}(x)=L^{-3}J^{\rm new}(x/L).
\tag{A7.20}
\]

The potential, gradient, and gradient-Hölder seminorm contract respectively by \(L^{-1},L^{-2},L^{-(2+\beta)}\). In particular the old-unit pair has strict margins inside the input domain (A7.3)–(A7.4).

Use \((U_0,J_0)=(U,L^{-3}J)\) in (A7.13)–(A7.15). The fluctuation source \(B'=g_kCA-\mathfrak hD(g_kCA)\) is the actual local source expression, with \(A\) on the real cutoff. There is a fixed constant \(C_B\) such that \(\|B'\|\le C_Bg_kr_{\chi,k}\). The source estimate remains valid on a fixed larger complex \(B\)-ball.

For example, choose a fixed \(r_B>0\) so that the norm-composition constants satisfy

\[
c_{\rm an}L^{-1}b_1+C_s r_B+C_s r_B c_{\rm an}L^{-1}b_1<b_1,
\qquad
c_{\rm an}L^{-3}\gamma+C_s r_B<\gamma.
\tag{A7.21}
\]

Here \(c_{\rm an}>1\) includes the fixed background-domain enlargement used by the rooted source expansion. Choose \(L>c_{\rm an}\) first. Additional fixed constants in the covariant-to-coordinate norm comparison are included in \(C_s\). The real-reference condition has the corresponding inequality \(c_{\rm an}L^{-1}b_0<b_0\). Thus the source hierarchy conditions retain their fixed margin, including the larger background domain used before the final Cauchy estimate. Require

\[
C_Bg_kr_{\chi,k}\le r_B/4.
\tag{A7.22}
\]

Then every switched pair entering the old insertion lies inside \(\mathscr D_k\), with a fixed analytic margin independent of scale, age, and volume. At the next step the rescaling regenerates the same margin. The radius is not divided by a fixed factor at each iteration.

For a local input coefficient, the entire difference

\[
f_X(U_s,\mathcal J_s)-f_X(U_0,J_0)
\tag{A7.23}
\]

is holomorphic in \(B\), vanishes at \(B=0\), and is bounded by twice its input supremum on \(\|B\|<r_B\). Directional Cauchy therefore gives

\[
\sup_{s,A\in D_\chi}
|f_X(U_s,\mathcal J_s)-f_X(U_0,J_0)|
\le C\frac{g_kr_{\chi,k}}{r_B}M_X.
\tag{A7.24}
\]

This estimate includes the independent-current variation. It would not follow from the naive nonflat multiplier substitution discussed before (A7.15).

### 6. Intrinsic locality, gauge gluing, and normalized transport

The localized operators in this construction are functions of the restrictions of the **variable pair** \((U_0,J_0)\) to their localization domains. The background is not frozen to one. Every switch is scalar and geometric. Covariance of \(Q,H_0,C_0,A^{(2)}\) and of the local nonlinear vertices therefore gives covariance of the entire pair (A7.13), (A7.15). With an invariant \(f_X\), each switched expression (A7.23) is invariant under simultaneous transformations of \(U_0,J_0\) and the fluctuation variables.

The connected-component property follows from the same localized fixed-point argument used in CP24. When switches disconnect a component from the protected root, the coefficient restricted to that component is independent of the root expression. The extra multiplier terms are made from the same localized kernels and local averaging derivative, so the property is unchanged.

Apply the rooted FTC/Cauchy expansion to the entire difference (A7.23). It produces local coefficients \(I_{X,Y}(U_0,J_0,A)\) with the bound (A7.24), times the usual switch-decay factor. All dependence on the variable source pair outside \(Y\) is absent. Thus this is intrinsic locality in \(U_0,J_0\), rather than locality only in increments at a fixed nonlocal reference.

The bound does not count the number of original fine background links. Directional Cauchy controls the complete composition \(f_X(U_s,\mathcal J_s)\); the FTC expansion differentiates scalar block switches. The integrated fluctuation coordinates are on the current lattice, with \(O(M^4n_k(X))\) coordinates in a prescribed carrier. The much larger original fine-link collection remains a background parameter. Thus importing the rooted construction introduces no hidden \(\xi_k^{-4}\) factor.

Now introduce \(t\sum I_{X,Y}\) into the **frozen** fluctuation integral. Assume its unmarked potentials obey the source expansion bounds on the enlarged fixed background domain just specified. This is the actual hypothesis of the regular-kernel theorem; §8 explains why it is not automatic for historical activities from CMP119. The covariance, cutoff, physical forward kernel, running coupling, and background maps are not differentiated. The derivative of the normalized expansion is the actual regular rooted integral. RX18 and RX34 apply, with \(r_B\) in place of the single connection-chart radius. This gives

\[
\mathscr T_k f=\mathscr T_{0,k}f+\mathscr Q_k f,
\qquad
(\mathscr T_{0,k}f)(U,J)=f(U,L^{-3}J),
\tag{A7.25}
\]

and, for compatible support weights specified below,

\[
\boxed{
\|\mathscr Q_k f\|_{k+1,\kappa,x}
\le C g_kr_{\chi,k}\|f\|_{k,\kappa,x}.
}
\tag{A7.26}
\]

The output coefficients are intrinsically invariant local functions of \((U,J)\). Indeed, the source localization and Gaussian/polymer operations preserve simultaneous gauge invariance; this is the content of CMP116 Lemma 2 and the final discussion on pp.21–22. The same proof applies to an auxiliary invariant bounded insertion because it changes only a local potential and the normalization is differentiated at zero. Invariance first holds for compact gauge changes preserving the real integration contour, then extends by analyticity to the source complex orbit domain.

Consequently the coefficients glue on overlaps as functions of the same physical fine-link pair. There is one formula in \((U,J)\), not a choice of a reference-dependent coefficient at each point. The equality of physical restrictions on different minimizing representatives follows from source orbit uniqueness and gauge invariance. No assertion is made that the old flat-reference coarse-\(V\) localizers themselves have acquired fixed-section invariance.

#### 6.1 The spatial reserve can be regenerated

Use the notation of RX4, RX11, RX21. Let

\[
p=(1-2\delta)\kappa_{\rm src},\qquad
\beta_{\rm act}=(1-8\delta)\frac L2\kappa_{\rm src}.
\tag{A7.27}
\]

Reserve a stronger source decay exponent \(\kappa_{\rm total}\) for the unmarked \(E,R\) activities, and run the marked expansion using a deliberately smaller \(\kappa_{\rm src}\). This is a division of one source spatial reserve; it does not assume an independently stronger theorem for \(R\). The source localization scale is chosen to support \(\kappa_{\rm total}\). Let \(C_{\rm prot}\) be the fixed protective-support conversion, \(C_a\) the extension counting constant, \(c_n\) the comparison between block count and polymer length, and \(A_A\) the animal-counting constant. A sufficient pair of strict inequalities is

\[
\begin{aligned}
\kappa&>C_{\rm prot}p+\log C_a+1,\\
\beta_{\rm act}-c_n\kappa-a_0c_n&>\log A_A+1.
\end{aligned}
\tag{A7.28}
\]

The source choice \(\delta=\frac1{10}(1-2/L)\) gives

\[
p=(0.8+0.4/L)\kappa_{\rm src},\qquad
\beta_{\rm act}=(0.1L+0.8)\kappa_{\rm src}.
\tag{A7.29}
\]

The constants in (A7.28) can be chosen independently of \(L\). This needs a geometric check; treating all of them as unspecified source constants would not suffice. Use the convention of §2 in which the protected collar is included in \(X\) once. Then \(C_{\rm prot}=1\). Connected extensions are counted on the graph of touching localization blocks, whose degree is at most \(3^4-1\), independently of the block side. A depth-first traversal of a spanning tree gives fixed constants \(C_a,A_A\). The comparison \(n\le c_n(d+1)\) is CMP116 (2.30); its constant is dimension-dependent, and the same inequality holds after replacing \(M\) by \(LM\). Fixed collars measured in block layers change these constants by fixed dimension-dependent factors, not by \(L\). If another convention is used, it must exhibit the same uniformity or retain (A7.28) as an additional condition.

Choose, for example, \(\kappa=p+\log C_a+2\) and a fixed KP exponent \(a_0\). Then the coefficient of \(\kappa_{\rm src}\) in the second left side of (A7.28) is

\[
0.1L+0.8-c_n(0.8+0.4/L).
\tag{A7.29a}
\]

It is positive for sufficiently large fixed \(L\); increasing \(\kappa_{\rm src}\) then pays the remaining fixed entropy and KP constants. Choose \(\kappa_{\rm total}=C_*\kappa_{\rm src}\), with a fixed sufficiently large \(C_*\), so that \(\kappa_{\rm total}/c_n\) also exceeds the marked block exponent and all fixed support-conversion and entropy costs. This additional reserve is used in §10. It avoids the incorrect requirement that a source tree exponent equal a block-count exponent when the comparison constant is larger than one. The \(L/2\) gain is the source geometric inequality (2.36). The factor \((L+2)^4\) appearing subsequently in its counting is an activity prefactor, paid by the weak-coupling threshold; it is not a new coefficient multiplying the support exponent. Thus the interval (A7.28) is nonempty for one sufficiently large admissible blocking factor. Choose the block size afterward to pay the switch rate, then choose domain radii and the weak-coupling threshold. All these are fixed independently of the number of RG steps.

If a particular route has already fixed a smaller blocking factor, (A7.28) must be checked for that choice; no unproved regrouping of steps is used here. With (A7.28), the quantum operation returns to the **same** exponential norm, rather than losing a fixed positive amount of decay at every step.

### 7. Classical restriction and the full 21-component projection

The classical map in (A7.25) is the intrinsic representation of the old insertion on the next minimizing background. The fine link field is unchanged; the current units and support units change. This is the same mechanism by which CMP119 retains an old \(E^{(j)}\) term and evaluates it on a later minimizing field.

For \(N\) steps put \(\lambda=L^{-N}\). The current rescaling is \(J_k=\lambda^3J_{k+N}\). A fixed original fine plaquette polynomial \(\mathcal W_\alpha(U)\), normalized to have the desired curvature-quadratic jet, defines the current-unit representative

\[
\iota_{k,\alpha}(U)=\xi_k^{-4}\mathcal W_\alpha(U).
\tag{A7.30}
\]

All 21 curvature-bilinear representatives use fixed microscopic stencils and the same physical root. Their parallel transports and supports are included in the root carrier. Then exactly

\[
L^{4N}\mathscr T_{0,k}^{(N)}\iota_{k,\alpha}
=\iota_{k+N,\alpha}.
\tag{A7.31}
\]

This identity does not choose a new nearest coarse root. Source-position redistribution is a separate matter in Gate 2.

Define \(P_k\) by the constant and 21 quadratic directional coefficients at \((U,J)=(1,0)\). On infinite space the tests are affine current-unit potentials on the support under consideration. On a finite physical torus of side \(D\), choose once a smooth physical cutoff \(\chi\), supported in the ball of radius \(D/4\) about the fixed physical root and equal to one in the ball of radius \(D/8\). Use the globally defined tests

\[
(a^{\rm cut}_{k,F})_\mu(x)
=\chi(h_kx)\left(-\frac12\sum_\nu F_{\mu\nu}x_\nu\right).
\tag{A7.31a}
\]

The root is the coordinate origin; periodic extension is smooth because the cutoff vanishes before the chart boundary. Use the same physical cutoff at every scale. Then

\[
a^{\rm cut}_{k+N,F}(\lambda x)
=\lambda a^{\rm cut}_{k,F}(x).
\tag{A7.31b}
\]

Consequently the quadratic projection has the exact classical scaling \(\Pi_{k+N}\mathscr T_{0,k}^{(N)}=\lambda^4\Pi_k\). The tests use the independent current \(J=0\). This convention is not globally identified with the physical current of the cutoff field, whose linear part can be nonzero in the cutoff annulus. The fixed microscopic marginal stencils lie in the plateau and retain their normalized jets; there the affine physical current has zero linear part. Long supports are controlled by their support tail, not by identifying these two current conventions. Constant gauge invariance kills every linear connection and current jet. The color bilinear form is fixed by simplicity of the gauge algebra, leaving the symmetric bilinear form on the six curvature labels, hence 21 coefficients. For a coefficient whose support lies in the plateau these are exactly its constant-curvature quadratic coefficients. The cutoff definition also defines a bounded projection for a wrapping coefficient; it does not claim that such a coefficient possesses a local constant-curvature interpretation.

For a support of current diameter \(R\), a directional Cauchy estimate on the fixed local potential domain bounds its curvature coefficient by

\[
C(1+R)^2M_X.
\tag{A7.32}
\]

The source norm absorbs this polynomial, and the output representative has fixed root support. Its supremum is uniform in \(\xi_k\): on the normalized \(C^1\) domain a plaquette differs from one by \(O(\xi_k^2)\), and the trace or paired-plaquette polynomial defining \(\mathcal W_\alpha\) starts quadratically in that difference. Hence \(\xi_k^{-4}\mathcal W_\alpha=O(1)\). Thus the nonconstant part of \(P_k\) is uniformly bounded. The identity coefficient is tracked separately in centered observables. No discontinuous periodic sawtooth test is used. In the cutoff annulus its normalized \(C^{1,\beta}\) norm is bounded polynomially in current support diameter, uniformly in the fine mesh. For a support meeting that annulus the diameter is already comparable to the cutoff radius. Thus the same polynomial support bound applies there; the exponential support tail pays it. The current output torus is assumed to admit the fixed root patch required by the source block geometry. This is the finite-volume condition used below, and excludes applying an additional RG block after the terminal geometry has ceased to admit that patch.

#### 7.1 Value gain on the same strengthened domain

One must not infer a \(C^{1,\beta}\) estimate for an exact axial representative from a bound on its link values. A rough axial gauge can differentiate curvature and lose a derivative. The following polynomial-jet gauge avoids that step.

**Local jet-gauge lemma.** Let the output connection have bounded normalized \(C^{1,\beta}\) norm on a fixed patch. On an old-unit support of diameter \(R\), with \(\lambda(1+R)\) sufficiently small, write

\[
A^{\rm old}_\mu(x)
=\lambda a_\mu+\lambda^2\sum_\nu M_{\mu\nu}x_\nu+R_\mu(x),
\qquad
\|R\|_{C^{1,\beta}}\le C\lambda^{2+\beta}(1+R)^{1+\beta}.
\tag{A7.33a}
\]

Here \(a=A^{\rm new}(0)\), and \(M\) is its first discrete jet, with forward differences at mesh \(\xi_{k+N}=\lambda\xi_k\). Discrete telescoping along coordinate paths proves the value estimate; the Hölder estimate for the first differences proves the gradient estimate and seminorm. The constants are independent of \(0<\xi_k\le1\).

Put \(\xi=\xi_k\), \(S=(M+M^T)/2\), and define two smooth polynomial gauge changes

\[
\begin{aligned}
u_1(x)&=\exp\!\left(i\lambda\sum_\nu a_\nu x_\nu\right),\\
q_S(x)&=\frac12\sum_{\mu,\nu}S_{\mu\nu}x_\mu x_\nu
       -\frac{\xi}{2}\sum_\mu S_{\mu\mu}x_\mu,\\
u_2(x)&=\exp(i\lambda^2q_S(x)).
\end{aligned}
\tag{A7.33b}
\]

Use the convention \(U_\mu^u(x)=u(x)U_\mu(x)u(x+\xi e_\mu)^{-1}\). For the polynomial part of (A7.33a), the Baker–Campbell–Hausdorff formula through order two gives, after \(u_1\), the coefficient

\[
T_{\mu\nu}=M_{\mu\nu}+\frac i2[a_\nu,a_\mu].
\tag{A7.33c}
\]

Its symmetric part is \(S\). The linear correction in \(q_S\) is necessary on the lattice: it gives the exact forward-difference identity
\(D_{\xi,\mu}q_S=\sum_\nu S_{\mu\nu}x_\nu\).
The second gauge therefore removes \(S\), leaving

\[
(a_F)_\mu(x)=-\frac12\sum_\nu F_{\mu\nu}x_\nu,
\qquad
F_{\mu\nu}=M_{\nu\mu}-M_{\mu\nu}+i[a_\mu,a_\nu].
\tag{A7.33d}
\]

The normalized logarithm has no hidden inverse-mesh loss. For the polynomial jet, the exact transformed link is analytic in \(\xi\), and its logarithm vanishes at \(\xi=0\). Factor \(\xi\) by the integral of its \(\xi\)-derivative **before** dividing by \(\xi\). Apply the same identity after up to two derivatives in \(x\). Taylor's formula in \(\lambda\) then bounds the remaining normalized logarithm in \(C^{1,\beta}\) by \(C\lambda^3(1+R)^q\), uniformly in \(\xi\). The calculation is finite-dimensional matrix calculus on a fixed neighborhood of the identity; the domain condition \(\lambda(1+R)\ll1\) keeps all logarithms in that neighborhood.

Next restore the rough remainder \(R\). The normalized link composition, with the smooth gauges in (A7.33b), is a smooth analytic function of the local value of \(R\), with uniformly bounded coefficients and their first two spatial derivatives. The same factor-of-\(\xi\) identity bounds its derivative with respect to \(R\). The \(C^{1,\beta}\) composition inequality therefore uses only \(R\) and its first Hölder derivative; no second derivative of \(R\) occurs. Combining this with (A7.33a), and using \(\lambda^3\le\lambda^{2+\beta}\), proves

\[
\begin{aligned}
a^{\rm jet}&=\lambda^2a_F+r,\qquad
\|r\|_{C^{1,\beta};X}
 \le C\lambda^{2+\beta}(1+R)^{q_\beta},\\
\|a^{\rm jet}\|_{C^{1,\beta};X}
&\le C\lambda^2(1+R)^{q_\beta},\qquad
\|J_k^{\rm jet}\|\le C\lambda^3.
\end{aligned}
\tag{A7.33}
\]

For the current, simultaneous conjugation by \(u_2u_1\) is bounded because \(\lambda(1+R)\) is small. The complex gauge change is allowed by the orbit domain. Only the smooth polynomial jet was gauged; no regularity assertion about an exact rough axial connection is used.

The radial affine representative (A7.33d) and an ordered axial affine representative have the same linearized curvature. Their difference is the discrete gradient of a quadratic polynomial, with the corresponding mesh correction. Gauge invariance identifies their quadratic jets: apply a gauge transformation of size \(t\) to \(t a_F\), and observe that its order-\(t^2\) correction contributes only through the already vanishing linear jet. Thus this choice extracts the same 21 curvature coefficients used in \(P_k\).

For a local invariant remainder \(q_X\in\ker P_k\), Taylor expansion and the removed jets give

\[
\sup_{\mathscr D_{k+N}}|q_X(U,\lambda^3J)|
\le C\lambda^{4+\beta}(1+R)^qM_X
\tag{A7.34}
\]

when \(\lambda(1+R)\) is sufficiently small. Mixed connection/current terms start at \(\lambda^5\), current-current terms at \(\lambda^6\), and the connection-quadratic Hölder error starts at \(\lambda^{4+\beta}\).

The use of an input analytic norm on current-potential charts rather than a raw fine-link product ball removes any fine-volume dependence from the Cauchy estimates. The direction \(a_F\) has norm polynomial in current support size, independently of \(\xi_k\).

#### 7.2 Tree norm and large supports

For a connected support, the current coarse cover satisfies

\[
n_{k+N}(\overline X)
\le c_0+c_1\lambda n_k(X).
\tag{A7.35}
\]

A spanning-tree traversal and a cover by current coarse blocks prove this inequality. Fixed protective collars change only \(c_0,c_1\).

Decompose an invariant family in \(\ker P_k\) piecewise as \(q_X=f_X-\iota_k\Pi_kf_X-f_X(1,0)\); the extracted coefficients sum to zero. The subtraction has only polynomial support cost. For \(n_k(X)\le A N\), use (A7.34). The fixed physical cutoff is identically one on these supports when \(N\) is sufficiently large and the output geometry admits its root patch: its old-unit plateau radius is of order \(\lambda^{-1}\), whereas their diameter is \(O(N)\). For the remaining supports, including wrapping supports, use the trivial supremum bound and the unused exponential input reserve. Choose \(A\) so that this reserve contributes at least \(\lambda^{4+\beta}\), and choose \(N\) so that \(c_1\lambda\kappa<\kappa/2\). The small-support polynomial-jet chart is nonwrapping for all sufficiently large fixed \(N\).

This proves, for one fixed sufficiently large \(N_0\),

\[
\boxed{
\|(1-P_{k+N})L^{4N}\mathscr T_{0,k}^{(N)}
  |_{\ker P_k}\|_{k\to k+N}
\le C_\beta L^{-\beta N},\qquad N\ge N_0.
}
\tag{A7.36}
\]

Unlike the old fixed-reference coarse-localizer statement, both sides use intrinsic local functions of the same fine background pair, and the rescaling preserves their invariance. No loss of analytic radius is accumulated.

This is an operator estimate for regular sources. It does not assert common point-root normalization or identify the actual phase-dependent marginal matrix; those are Gate 2 obligations. For the stronger \(O(g_k^2)\) estimates on the finite marginal and reverse blocks, use Gate 2 §10, N7.40–N7.44. That argument differentiates the joint-pair extension at the flat background and uses the actual flat-measure moment estimate. The cubic potential is extended by subtracting its degrees zero, one, and two on the full analytic atlas; its third-order vanishing is then an identity, with physical equality supplied by the minimizing-section equations. Thus it does not require an unproved positive-measure bound at independent nonflat \(J=0\). The full analytic operator bound in (A7.26) remains \(O(g_kr_{\chi,k})\).

### 8. The regular marked induction and its limits

The initial Wilson/clover insertion is an intrinsic local function of the fine links and has no independent-current dependence. For a frozen regular kernel admitted on the enlarged fixed domain, (A7.25)–(A7.26) give an intrinsic local analytic extension whose physical restriction is the actual transported insertion. Iterating gives the same statement for sequences of such kernels, with the same domain radii and support exponent. The kernel-admission qualification cannot be dropped merely because every step is on a full torus. The engineering factor is included explicitly in the rescaled map; the quantum perturbation is \(O(L^4g_kr_{\chi,k})\), with \(L\) fixed.

One may either retain the resulting functions at each current scale or record the quantum differences by their birth scales. In the latter representation,

\[
f_k
=\mathscr T_{0,b}^{(k-b)}f_b
 +\sum_{j=b}^{k-1}
  \mathscr T_{0,j+1}^{(k-j-1)}\mathscr Q_j f_j,
\tag{A7.37}
\]

with the source positions and engineering factors kept in the chosen convention. This is an exact Duhamel identity for the regular operator family, not a derivative of a source-dependent coupling trajectory.

The norm alone bounds a raw sequence by a product of operator norms; useful uniform physical bounds still require the marginal/stable normalization in Gate 2. Nor does this regular induction prove the field representation after core entry, reset, or boundary transfer. The source's boundary domains have additional scale and history dependence; they are addressed by Gate 3.

#### 8.1 Shrinking birth domains and classical maturation

CMP119 (2.28) gives the birth radii \(\alpha_{0,j},\alpha_{1,j}\) proportional to \(g_j\) times logarithmic powers. Its asserted extension for both the \(E^{(j)}\) and \(R^{(j)}\) coefficients is on those domains. Boundedness there does **not** imply analytic continuation to the fixed-radius domain in §2. Absorbing an old \(R\) term into the regular action does not create that continuation. One must either retain a valid larger-domain construction of that coefficient, or keep its birth domain explicitly.

There is, however, a direct useful restriction result. Suppose a birth domain contains normalized connection/reference/current balls with positive radii \(\rho_{0,j},\rho_{1,j},\gamma_j\). The constants may depend on the birth coupling. Set \(\lambda=L^{-n}\). If

\[
c_{\rm an}\lambda b_0\le\rho_{0,j}/2,\qquad
c_{\rm an}\lambda b_1\le\rho_{1,j}/2,\qquad
c_{\rm an}\lambda^3\gamma\le\gamma_j/2,
\tag{A7.38}
\]

then classical restriction maps the enlarged fixed output domain into the birth domain, with a definite margin. Consequently

\[
\sup_{\mathscr D_{j+n}}|R^{(j)}(U,L^{-3n}J)|
\le \sup_{\mathscr D^{\rm birth}_j}|R^{(j)}|.
\tag{A7.39}
\]

This is restriction of an already holomorphic function, not analytic continuation. It holds coefficientwise and preserves intrinsic locality and gauge invariance. The same statement applies to an \(E^{(j)}\) coefficient when its birth estimate is the only available estimate.

An explicit sufficient maturation age is the ceiling of the maximum of

\[
\log_L\frac{2c_{\rm an}b_0}{\rho_{0,j}},\quad
\log_L\frac{2c_{\rm an}b_1}{\rho_{1,j}},\quad
\frac13\log_L\frac{2c_{\rm an}\gamma}{\gamma_j},\quad0.
\tag{A7.40}
\]

If a birth localization block has side \(MR_j\), include also the support-conversion condition \(c_1L^{-n}R_j\kappa_{\rm out}\le\kappa_{\rm birth}/2\). The spanning-tree argument then transfers the weighted sum with a fixed constant. Radii of the form \(g_j\) times logarithmic powers, and polylogarithmic \(R_j\), give \(n_j=O(\log(1/g_j))\). The engineering factor \(L^{4n_j}\), fixed-degree Cauchy losses, and support conversion cost at most a fixed inverse power of the birth radii. Thus the arbitrarily high fixed power in the source estimate (2.31) can pay these **classical** maturation costs.

#### 8.2 Quantum maturation under admitted bulk kernels

Classical restriction alone is not the only available mechanism. A source on a shrinking birth domain can be propagated through **pure admitted bulk kernels** while its analytic radius grows geometrically. This statement requires that the unmarked kernels already have the fixed-domain admission of §6; a recent \(R\) term is not inserted into their action outside its own domain.

For clarity take one common normalized radius \(r\) for the real reference, complex relative connection, and independent current, with fixed comparison factors. Let \(b\) be a fixed allowed radius and choose

\[
L^{-1}<\theta<c_{\rm an}^{-1},\qquad
r_{t+1}=\min\{b,\theta L r_t\}.
\tag{A7.41}
\]

Assume throughout the finite maturation interval that

\[
C_Bg_{j+t}r_{\chi,j+t}\le c_*r_t,
\tag{A7.42}
\]

where \(c_*\) is a fixed sufficiently small constant. For the enlarged output domain, the old-unit reference and relative connection have radii at most \(c_{\rm an}\theta r_t\), and the old-unit current radius is at most \(c_{\rm an}\theta L^{-2}r_t\). These leave a fixed relative margin. In (A7.13)–(A7.18) take the fluctuation \(B\)-ball radius to be a fixed small multiple of \(r_t\). The uniform operator constants come from the unmarked fixed bulk domain, so this choice introduces no additional inverse radius. Directional Cauchy gives

\[
\|\mathscr Q^{\rm bulk}_{j+t}f\|_{r_{t+1},\kappa}
\le C\frac{g_{j+t}r_{\chi,j+t}}{r_t}
       \|f\|_{r_t,\kappa},
\qquad
\|L^4\mathscr T^{\rm bulk}_{j+t}f\|_{r_{t+1},\kappa}
\le K L^4\|f\|_{r_t,\kappa}.
\tag{A7.43}
\]

Here \(K\) is fixed, independent of the radius, fine mesh, age, and volume. The same spatial reserve from §6.1 is used at every step. This estimate applies to a mark; the bulk density itself has not been analytically continued from a smaller domain.

Let

\[
n_j=\left\lceil\frac{\log(b/r_0)}{\log(\theta L)}\right\rceil_+.
\tag{A7.44}
\]

After \(n_j\) steps the output mark belongs to the fixed-radius class. Multiplying (A7.43) gives

\[
\left\|\prod_{t=0}^{n_j-1}
 L^4\mathscr T^{\rm bulk}_{j+t}f\right\|_{b,\kappa}
\le C\left(\frac b{r_0}\right)^p\|f\|_{r_0,\kappa},
\qquad
p=\frac{\log(KL^4)}{\log(\theta L)}.
\tag{A7.45}
\]

Increasing \(p\) if necessary covers the fixed support-grid conversion. The loss is a fixed power of the birth radius, rather than a product of an inverse birth radius at every step. In particular a radius comparable to \(g_j\) times a logarithmic power gives a fixed inverse-coupling power, which (2.31) can pay by choosing \(\kappa_0\) sufficiently large.

Condition (A7.42) is explicit. On an asymptotically free segment of length \(O(\log(1/g_j))\), adjacent inverse couplings change by a bounded amount and \(g_{j+t}r_{\chi,j+t}\le Cg_jr_{\chi,j}\) for sufficiently small \(g_j\). Thus it suffices that the birth radius dominate that fluctuation size by the fixed factor in (A7.42). This must be checked against the chosen source logarithmic exponents; the fact that a radius tends to zero is not itself enough.

The theorem proves quantum maturation of a shrinking-domain **mark under bulk propagation**. It does not prove that the full recent-\(R\) action is admitted on each enlarged ramp domain. Section 10 supplies a normalized comparison on a common narrower domain and controls the resulting age-zero forcing. A rare-event amplitude is never used to supply analytic continuation. The remaining exact regular identification is stated in (A7.58); mixed-boundary entry is an additional Gate 3 interface.

For activities already admitted on the fixed regular domain, evaluation at a later regular background has only fixed unit and support conversion costs, and (A7.36) gives age decay after removing the 21 jets. This established case must be distinguished from the shrinking-domain case above.

#### Exact status of Gate 1

The original strongest version of CC62, demanding individually invariant coefficients as functions of a fixed-reference coarse variable, is not proved here. Instead, the intrinsic source representation supplies a closed regular source operation for the admitted fixed-domain kernels, with nonflat background dependence kept as a variable, a base-preserving current extension, a mesh-uniform polynomial-jet contraction, fixed analytic margins, and a fixed spatial reserve.

The full Gate 1 claim for every density of the final construction is not yet complete. Classical maturation and pure-bulk quantum maturation resolve eventual entry into the fixed class with fixed-power losses, and §10 proves the regular \(R\)-potential admission and feedback on a common narrow domain. What remains is to identify the fixed-domain pure bulk with the actual final regular kernel through the rare correction (A7.58), including the historical absorption and counterterm convention. Before using the regular theorem in the complete S2 theorem one must also verify Gate 2 normalization and Gate 3 transfer of mixed-history contributions. No estimate for these interfaces is obtained by changing the name of the source norm.

### 9. Sources and remaining checks

- **CMP102 (1985), 277–309**: Theorem 1 (9) for real minimizing-field Hölder regularity; Proposition 4 (97)–(98) for the analytic nonlinear force; (127)–(133) for the unprojected constrained equation; (178)–(180) for the minimizing-reference cancellation; Proposition 9 for analytic nonflat background response.
- **CMP99 (1985), 389–434**: normalized inverse and adjoint bounds; (3.137) for the small constraint-Hessian correction; Theorem 3.14 and its following discussion for localized inverses and tree-shaped products.
- **CMP109 (1987), 249–301**, [DOI](https://doi.org/10.1007/BF01215223): (1.8)–(1.19), intrinsic independent-current orbit domains; the paragraph after (1.16), smaller-domain inclusion; (2.3) and the following physical fluctuation-field identification.
- **CMP116 (1988), 1–22**, [DOI](https://doi.org/10.1007/BF01239022): switched nonlinear response (1.3)–(1.21), Lemma 2, Lemma 3, and pp.21–22 for intrinsic gauge invariance of localized output.
- **CMP119 (1988), 243–285**: birth-indexed intrinsic regular terms (2.26)–(2.32), actual rooted normalized insertion (3.44)–(3.47), and the treatment of old regular terms following (3.48).

The remaining identification is (A7.58), together with checking the chosen source radii against (A7.47); mixed-boundary transfer and common point-source normalization remain in Gates 3 and 2 respectively.

### 10. Common narrow charts, regular \(R\)-density conversion, and age feedback

This section gives a quantitative comparison theorem on the actual shrinking charts. It establishes the regular \(R\) norm needed by H7-A and a closed representation with birth ages. The final identification of the pure bulk reference with the regular sector of the complete construction is kept separate in §10.5.

#### 10.1 The metric and birth hypotheses

The source metric \(d_j(X)\) is the length, in units of \(M\), of a shortest tree touching the fixed \(M\)-blocks in \(X\); see CMP109, p.257. The \(R^{(j)}\) domains in CMP119 are unions of \(MR_j\)-cubes but use this same metric. An \(MR_j\)-cube contains \(R_j^4\) underlying \(M\)-blocks. It is not a single zero-cost vertex for \(d_j\).

For every birth coefficient use the supplied estimate

\[
\sup_{\mathscr D^{\rm birth}_j(X)}
 |R^{(j)}_X(U,J)|
\le M_{j,X}:=g_j^{\kappa_0}
                 e^{-\kappa_{\rm total}d_j(X)}.
\tag{A7.46}
\]

The coefficient is intrinsically gauge invariant. At the flat pair its linear differential in both connection and current is therefore zero: the differential would be a color-invariant linear functional on copies of a simple Lie algebra. Vacuum subtraction gives
\(\widetilde R^{(j)}_X=R^{(j)}_X-R^{(j)}_X(1,0)\). The removed value cancels in a single frozen normalized regular operator and is used here to estimate its fluctuation difference. If it depends on a carrier or history, its original factor remains in that carrier or history weight; it is not discarded from the joint positive law or from conditional-mean comparisons.

Choose radii \(r_j>0\) so that the birth domain contains the normalized reference/relative/current ball of radius \(c r_j\), with fixed comparison factors. CMP109's convention is that the independent-current amplitude bound is \(\gamma_0=\alpha_0\). Thus the same scalar radius can be used for these three amplitudes; the current has dimension three under rescaling, not a radius that must be cubed. For the source radii in CMP119 (2.28), one may take a fixed small multiple of their minimum. We require

\[
\frac{r_{j+1}}{r_j}\le A<L/c_{\rm an},
\qquad
C_Bg_jr_{\chi,j}\le c_*r_j,
\qquad
0<r_j\le b.
\tag{A7.47}
\]

The constants are fixed. For radii \(g_j\) times fixed logarithmic powers, the adjacent ratio is bounded, and approaches one in the weak-coupling regime. The fluctuation condition is satisfied when the chosen birth logarithmic power exceeds the cutoff power and its fixed constant is large enough. These are explicit radius requirements. Applying the theorem to a source convention with other exponents requires checking them; a bound on a real physical cutoff alone is insufficient.

#### 10.2 Admission of all ages on one current narrow chart

Let \(\mathscr N_k\) be the strengthened local orbit domain with radii a fixed small fraction of \(r_k\), including the source's enlarged background factor. For \(j\le k\) put \(s=k-j\), \(\lambda=L^{-s}\). A pair in \(\mathscr N_k\), written in birth units, has connection/reference size at most \(C\lambda r_k\) and current size at most \(C\lambda^3r_k\). From (A7.47),

\[
\lambda r_k\le(A/L)^s r_j,
\qquad
\lambda^3r_k\le(A/L^3)^s r_j.
\tag{A7.48}
\]

The same estimate holds for the switched field/current pair entering the one-step integral: its current-scale norm increases by at most \(C g_kr_{\chi,k}\), which (A7.47) pays. The fixed prefactors in the definition of \(\mathscr N_k\) leave a uniform relative margin inside every birth domain. No historical coefficient is continued past that domain.

Consequently all terms \(\widetilde R^{(j)}_X\), of every age, have legitimate evaluations on the same current narrow chart and the same switched fluctuation domain. Their complete-force localizations are holomorphic there. This admission statement concerns intrinsic regular coefficients; a mixed-boundary coefficient with a different source domain is not included.

#### 10.3 The action-density conversion has no exponential age loss

The estimate must count all birth roots in a current block. Let \(\overline X\) be the current protected block cover of a birth support. The spanning-tree cover gives

\[
n_k(\overline X)\le c_0+c_1\lambda n_j(X).
\tag{A7.49}
\]

Assign every current localized term to a block meeting its support, using one fixed deterministic convention. A localized extension can hit the target current block even if the original birth root is outside its fixed collar. Retain the reserved decay connecting the birth root to that block and use the convolution estimate

\[
\sum_{\text{birth blocks }b}
 e^{-c\,\operatorname{dist}_{k}(b,\Delta_k)}
 \le C\lambda^{-4}.
\tag{A7.49a}
\]

The near collar contains \(O(\lambda^{-4})\) birth blocks; the outer shells give a convergent exponential sum with the same factor. If the chosen anchor is far inside its birth support, its distance is paid by that support's tree decay, or the activity can be reanchored at a nearest block with a polynomial support multiplicity. At zero age the original support cover is unchanged; at positive age choose \(L\ge c_1\). The reserve \(\kappa_{\rm total}\) from §6.1 pays the current support weight, the fixed collars, the connecting distance just used, and the connected-animal entropy at every age.

The factor \(\lambda^{-4}\) is canceled by a genuine value gain. If \(\lambda\operatorname{diam}_jX\) is small, use the polynomial-jet gauge of §7.1 for the current pair, whose normalized connection and current are bounded by \(Cr_k\). It gives a birth connection of size
\(C\lambda^2r_k(1+\operatorname{diam}_jX)^q\) and a current of size \(C\lambda^3r_k\). Since the constant has been subtracted and both linear jets vanish, directional Cauchy on the birth ball gives

\[
|\widetilde R^{(j)}_X(U,J)|
\le C M_{j,X}\lambda^4
\left(\frac{r_k}{r_j}\right)^2
(1+\operatorname{diam}_jX)^{q'}.
\tag{A7.50}
\]

If the upper bound for the gauged field is larger than the Cauchy radius, use the trivial \(2M_{j,X}\) instead. The same displayed inequality, with its upper-bound polynomial enlarged, remains true because the squared radius ratio of that upper bound is then bounded below. Gauge invariance keeps the evaluated point in the birth orbit domain; no Taylor expansion outside the ball is used.

For the remaining supports, \(\lambda\operatorname{diam}_jX\ge c\). Connectedness implies \(n_j(X)\ge c'/\lambda\). An unused fixed fraction of the source exponential bounds their anchored sum by \(C e^{-c''/\lambda}\). Thus \(\lambda^{-4}\) times this tail is uniformly bounded. This argument uses the fixed \(M\)-block metric; the \(MR_j\) geometry introduces no uncontrolled inflation.

The same bounds hold uniformly on the switch polydisc. Apply the whole-value localization estimate RX39–RX43 to retain their gain, then sum the birth roots. For the actual current local-potential norm this proves

\[
\boxed{
\|R_{j\to k}\|_{\rm pot,\mathscr N_k}
\le C g_j^{\kappa_0}
       \left[1+\left(\frac{r_k}{r_j}\right)^2\right]
\le C g_j^{\kappa_0}(1+r_j^{-2}).
}
\tag{A7.51}
\]

Here \(R_{j\to k}\) denotes either the vacuum-subtracted activity evaluated on the current background, or its difference between the fluctuated pair and that background. The latter is the perturbing potential in the normalized kernel; its bound follows by applying the former bound twice. The gain in (A7.50) and the birth-root count are both necessary. Omitting the count would give the wrong density normalization; omitting the gain would leave a false exponential age loss.

For \(r_j\ge c g_j\) times a nonnegative logarithmic power and \(x_j=g_j^{-2}\), the last bound is at most \(C x_j^{-(\kappa_0-2)/2}\). The asymptotically free comparison \(x_j\ge x_k+c_-(k-j)\) then gives, for any desired fixed \(q\),

\[
\epsilon_k:=\sum_{j\le k}
\|R_{j\to k}\|_{\rm pot,\mathscr N_k}
\le C_q x_k^{-q},
\qquad \kappa_0>2q+4.
\tag{A7.52}
\]

No recent-age cutoff is needed for this summation. Additional fixed-degree projection or coordinate losses can be paid by increasing \(\kappa_0\) once. An exponent growing with age would not be covered by this assertion.

#### 10.4 Exact narrow-chart forcing and the age convolution

Fix an admitted bulk kernel \(\mathscr T_k^{\rm bulk}\) with the fixed-domain properties above. Suppose the physical kernel under comparison has exactly the same frozen maps, covariance, cutoff, and source-independent factors, and differs by the localized potential \(R_k\) just bounded. On \(\mathscr N_{k+1}\) interpolate only that potential. The theorem H7-A applies because both the reference kernel and \(R_k\) are analytic on this common chart. All historical marked pieces whose radii have followed the ramp are admitted there: choose \(\theta L>A\) in (A7.41), and use (A7.47) inductively. A matured piece has the fixed radius \(b\).

For the engineering-rescaled operators, put

\[
\widehat D_k
=L^4(\mathscr T_k^{\rm full}-\mathscr T_k^{\rm bulk}).
\tag{A7.53}
\]

The normalized interpolation is an equality of the actual kernels on their common physical section, and it gives the rooted bound

\[
\|\widehat D_k f\|_{\mathscr N_{k+1},\kappa}
\le C L^4\epsilon_k\|f\|_{\rm admitted\ mark}.
\tag{A7.54}
\]

For a sum of birth pieces, sum their admitted norms on the right. The constants do not contain inverse narrow radii: the mark is evaluated through the pair map with a fixed relative domain margin, and the only fluctuation-to-radius quotient is bounded by (A7.47). Cauchy in the potential interpolation parameter costs \(\epsilon_k\), not a derivative of the running coupling or of the forward kernel.

Write \(\widehat P^{\rm bulk}_{k,j}\) for pure bulk transport from scale \(j\) to \(k\). The actual marked recursion has the exact decomposition

\[
f_k=\widehat P^{\rm bulk}_{k,b}f_b
 +\sum_{j=b}^{k-1}
   \widehat P^{\rm bulk}_{k,j+1}\widehat D_j f_j.
\tag{A7.55}
\]

Each summand is born on its valid narrow chart. It follows the pure bulk radius ramp and enters the fixed class after (A7.44), with amplification at most
\(\Omega_{j+1}=C(b/r_{j+1})^p\).
The full perturbed kernel is never applied on a chart where its recent activities are undefined. Equation (A7.55) is the required separation of actual narrow-chart forcing from broad-chart bulk propagation.

This proves closure as a **graded regular source representation**, at each finite number of steps, provided the stated bulk comparison is the actual one. A uniform estimate must use a propagation bound valid for arbitrary profiles: the forcing in (A7.54) need not be a smooth source profile.

The moving block norm in Gate 2, N7.45–N7.49, gives the sufficient mature bulk bound

\[
\|\widehat P^{\rm bulk}_{k,j}\|
\le C\left(\frac{x_j}{x_k}\right)^{p_b}
\tag{A7.56a}
\]

for the admitted regular class, including arbitrary profiles. This follows from the \(O(g^2)\) marginal/reverse blocks and the strict stable contraction; it is weaker than the still-missing common point-source normalization. Any normalization change during a maturation interval costs at most a further fixed inverse-radius power, included in \(\Omega_j\).

Give each immature piece a weight equal to its remaining maximal maturation amplification. Let \(\mathcal F_k\) be the sum of these reserved norms and the mature norm. For a desired incoming benchmark \(w_k=(x_k/x_*)^s\), write \(\mathcal A_k=\mathcal F_k/w_k\), and let \(\mathcal A_k^{\rm bulk}\) be the corresponding pure bulk contribution. Equations (A7.54)–(A7.56a) give

\[
\mathcal A_k
\le\mathcal A_k^{\rm bulk}
 +C\sum_{j=b}^{k-1}
  \Omega_{j+1}\epsilon_j
  \left(\frac{x_j}{x_k}\right)^{p_b+s}\mathcal A_j.
\tag{A7.56}
\]

This is the weighted age convolution; Gate 2, N7.50–N7.51, gives the same scalar row estimate for arbitrary profiles. If \(\Omega_j\le Cx_j^v\), with fixed \(v\), choose the freely selectable decay in (A7.52) so that
\(q>v+p_b+s+1\).
The asymptotically free scale comparison then bounds every row by

\[
C x_k^{-(p_b+s)}
 \sum_{j<k}x_j^{-q+v+p_b+s}
\le C_q x_k^{1-q+v}
\le C_q x_*^{1-q+v}.
\tag{A7.57a}
\]

At sufficiently weak coupling the last expression is at most \(1/2\). Taking the supremum over any finite scale interval and then increasing that interval proves

\[
\boxed{\sup_k\mathcal A_k
\le 2\sup_k\mathcal A_k^{\rm bulk}.}
\tag{A7.57}
\]

Thus these admitted regular \(R\) corrections preserve any established bulk benchmark, after the fixed source choices. They do not create an exponential loss with ultraviolet depth or mark age. This conclusion is not a proof of the bulk benchmark itself: in particular the common point-source normalization issue in Gate 2 remains. The generic polynomial bound (A7.56a) does show, even without such a benchmark, that the age convolution can be treated by a factorized polynomial weight rather than by an exponential-in-age bound.

#### 10.5 The remaining bulk identification

There is an actual fixed-domain reference available: CMP109 (1.18), p.263, constructs the pure regular \(E^{(j)}\) activities on absolute \(\alpha_0,\alpha_1\) domains, with constants independent of \(j,X\) and with the stated small-coupling parameter range. Thus the reference in §10.4 need not be a hypothetical analytic potential.

It remains necessary to identify its relation to the regular \(E\) used in the final CMP119 density. The latter's formula (3.26) first absorbs sufficiently old \(R\)-terms into \(E_k\), then interpolates the remaining \(R\)-terms. Earlier such absorptions can already affect later birth coefficients \(E^{(j)}\). The shrinking-domain estimate (2.28) alone does not say that every one of those coefficients is the restriction of the fixed-domain pure coefficient. Nor may a recent pure-vacuum coefficient of size \(O(g_j^2)\) be declared rare and charged to the freely selectable \(\kappa_0\).

The exact remaining identification is a decomposition, at the **frozen actual coupling trajectory**,

\[
E_k^{\rm final}=E_k^{\rm pure}+\Delta E_k,
\tag{A7.58}
\]

in which \(E_k^{\rm pure}\) is the fixed-domain source sequence and \(\Delta E_k\), together with the explicitly retained \(R_k\), has the common narrow-chart local-potential bound used in (A7.52). A sufficient construction would retain the birth labels of every cluster containing an \(R\)-vertex, keep the corresponding coefficients in the narrow sector until maturation, and include only admitted mature coefficients in the fixed bulk. Source (3.26) supplies the exact one-step interpolation identity, while §§10.1–10.4 supply its missing regular chart conversion and marked age estimates. The full unmarked relabeling and the equality (A7.58), including its counterterm convention, are not proved merely by that identity and are not claimed here.

Accordingly, this appendix completes the regular intrinsic \(R\)-density conversion and the graded-age comparison mechanism. It reduces the remaining regular issue to the concrete bulk identification (A7.58) and the explicitly stated radius choices. The arbitrary-profile mature propagator estimate is supplied by Gate 2; preservation of a particular observable benchmark still requires that benchmark for the pure reference source. Mixed-boundary admission is still outside its scope.

---
