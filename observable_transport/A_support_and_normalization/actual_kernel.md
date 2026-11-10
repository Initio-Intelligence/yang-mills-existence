# M-04: a marked Gaussian reserve and the exact current it pays

Scope: the scalar root at the actual regular Gaussian integration.

## 1. Primary construction

The following source statements are used, with their printed equation and page labels.

* Bałaban, CMP 116 (1988), pp. 2–5, (1.1)–(1.12): the nonlinear constrained minimizer is a function of local analytic maps and quasilocal propagators. The localization parameters are attached to generalized random walks. Setting them to zero outside a component disconnects the nonlinear equations, so the localized expression has actual external-field support in the root component. This is an actual dependence statement, not an interpretation of a numerical decay bound.
* The same paper, pp. 10–11, (1.37)–(1.42): the Wilson contribution is localized before integration. The inverse-coupling factor is handled by the vanishing Taylor terms and a quadratic form in the normalized fluctuation. A bare supremum proportional to the square of the small-field cutoff is not necessary at this stage.
* The same paper, pp. 15–17, (2.14)–(2.26): absolute localized integrands are dominated by a real joint Gaussian after extracting small quadratic errors. The error coefficient called alpha_5 is chosen small enough to retain a fixed positive Gaussian reserve. The source then integrates this Gaussian and pays a determinant cost exponential in the localization volume.
* CMP 119 (1988), pp. 277–279, (3.44)–(3.47): a localized insertion is carried in one distinguished numerator activity H'(Z_0), while the other activities coincide with those of the denominator. The quotient is formed with the same regular integral. The assertion that H' obeys the same bound there applies to the action-response insertion constructed in that source. It does not by itself prove the desired scalar bound.
* CMP 119, p. 262, immediately after (2.42): before an optional regrouping, B-terms have full d_j(X) decay; regrouping terms to contain entire large-field components changes the available decay to d_j(X minus Z_j). The latter cannot be read as a full physical-volume bound.

The new estimate below addresses the polynomial insertion cost in the third bullet. It removes an unnecessary logarithmic small-field-radius loss. It does not reconstruct physical supports lost in the last bullet.

## 2. A finite-rank Gaussian insertion lemma

All norms in this section are ordinary Euclidean operator norms. A rank or trace appearing below is the rank or trace on the actual finite integration space; it is not the number of microscopic links in a fixed physical region unless those are precisely the integration coordinates.

### Theorem G1 (polynomial roots use only a trace cost)

Let A be a real positive-definite matrix on a finite-dimensional space, with A >= a I for a fixed a>0. Let nu_A be its centered normalized Gaussian. Let P>=0, and let r>=0. If a possibly complex root f obeys

    |f(u)| <= B [r + u^T P u],

then

    integral |f| dnu_A <= B [r + a^(-1) Tr P].                 (G1.1)

More generally, for every integer n>=1,

    integral (r+u^T P u)^n dnu_A
      <= [r + 2n a^(-1) Tr P]^n.                            (G1.2)

If additionally ||P||<=p_0 and rank P<=r_0, the right side of (G1.1) is at most B[r+a^(-1)p_0 r_0]. All constants are independent of the ambient dimension.

**Proof.** Write u=A^(-1/2)g with g standard Gaussian. The nonnegative matrix D=A^(-1/2)PA^(-1/2) has eigenvalues lambda_j. Then u^TPu has the law of sum_j lambda_j g_j^2. Its mean is Tr D<=a^(-1)Tr P, proving (G1.1). Minkowski gives

    ||sum_j lambda_j g_j^2||_n
      <= sum_j lambda_j ||g_j^2||_n
      <= 2n sum_j lambda_j.

The last inequality follows from E g_j^(2n)=(2n-1)!! <= (2n)^n. Another application of Minkowski proves (G1.2). No determinant comparison on all integration variables has been used. QED.

### Theorem G2 (exponential insertion uses a finite-rank determinant)

Under the assumptions of G1, for 0<=theta with 2theta ||A^(-1/2)PA^(-1/2)||<1,

    E_nu_A exp(theta u^TPu)
      = det(I-2theta A^(-1/2)PA^(-1/2))^(-1/2).

If 2theta a^(-1)||P||<=1/2, then

    E_nu_A exp(theta u^TPu)
      <= exp(2theta a^(-1)Tr P).                            (G2.1)

**Proof.** Diagonalize D as above and use the one-dimensional Gaussian integral. Since -log(1-x)<=2x for 0<=x<=1/2, half the logarithm of the determinant is at most 2theta Tr D. QED.

This is the appropriate source tilt for a localized root. Scaling the entire Gaussian precision to pay one root would introduce an unnecessary ambient-rank factor. If the root energy has rank O(|Z|), (G2.1) costs only exp(C theta |Z|).

## 3. The joint Gaussian in CMP 116 really has the required reserve

The unperturbed joint Gaussian underlying (2.23) can be written, before normalization, as

    exp[-1/2 |X|^2
        -1/2 (B+C Gamma X)^T C^(-1)(B+C Gamma X)] dB dX,

where C is the relevant restricted covariance and Gamma is the conditioning operator. This is precisely the completion of the cross term: expanding the second square produces the bilinear B^T Gamma X and the compensating quadratic form in X. It is not a replacement covariance.

Let

    Q_0(B,X)=|X|^2+|C^(-1/2)(B+C Gamma X)|^2.

Suppose ||C||<=c_C and ||C Gamma||<=c_G, as supplied by the bounded propagator/conditioning estimates used at this integration. Then

    |B|^2 <= 2 c_C Q_0+2 c_G^2 |X|^2,

and consequently

    Q_0(B,X) >= a_0 (|B|^2+|X|^2),
    a_0=(1+2c_C+2c_G^2)^(-1).                              (G3.1)

If the extracted error in the quadratic form is at most alpha(|B|^2+|X|^2), alpha<=a_0/2, the Gaussian majorant retains precision at least a_0/2. Its mass is exactly the determinant factor already paid in CMP 116 (2.24)–(2.26); inserting a root does not require paying it again.

Thus if the absolute scalar integrand for a tag with carrier Z is bounded by

    b h^(-4) c_tag [R_Z(v)+u^T P_Z u],
    ||P_Z||<=C,  Tr P_Z<=C(1+|Z|),                         (G3.2)

the same tag's Gaussian integral is bounded by

    C b h^(-4) c_tag [R_Z(v)+1+|Z|]
       times its existing unmarked Gaussian mass.          (G3.3)

Here R_Z is a genuine externally supported energy function of that tag, and u=(B,X). The inequality is termwise. It therefore remains valid before absolute summation, which a bound on the completed conditional expectation would not guarantee.

For any fixed spare localization rate delta>0,

    (1+|Z|) exp[-delta |Z|]
      <= 1+(e delta)^(-1).                                 (G3.4)

Hence the trace cost can be paid by a fixed part of the source's unused decay. There is no factor p(g)^2 and no factor equal to the volume of the whole integration domain.

### Exact application boundary

This proves the insertion cost for every actual localized tag for which (G3.2) has been established, using its actual Gaussian majorant. It does **not** assert that arbitrary inherited normalized component factors satisfy (G3.2), nor that the support of R_Z or P_Z is its small storage domain. Those questions are upstream of this integration lemma.

## 4. Why the microscopic scalar has the required quadratic energy form before nonlinear localization

Let V_1,...,V_l be compact link factors forming one plaquette, and let

    U_i=exp(X_i) V_i,

where X_i is anti-Hermitian. Telescoping products, unitarity, and
||exp(X)-I||_HS<=||X||_HS imply

    ||U_1...U_l-V_1...V_l||_HS <= sum_i ||X_i||_HS.

Since 2s(P)=||P-I||_HS^2 for compact P, for l fixed,

    beta s(U_p)
       <= 2 beta s(V_p)+C beta sum_i ||X_i||_HS^2.          (G4.1)

For X_i=(1+beta)^(-1/2) T_i(z), with each T_i linear in normalized fluctuation coordinates,

    beta s(U_p)
       <= 2 beta s(V_p)+C sum_i |T_i(z)|^2.                (G4.2)

The inequality holds for all real normalized fluctuation values; it is not a small-field Taylor asymptotic. The identity term of a centered scalar costs only h^4|c| in its exposed budget.

A complex version on a fixed normalized fluctuation tube follows by Taylor's formula about the real compact configuration, as in SR20.1. For each fixed local stencil,

    |h^4 F_h(U(z+i eta))|
       <= C_rho b [1+E_S(U(z))]

when the total normalized imaginary increment is bounded by rho. Combining this with (G4.2) gives the real-centered complex quadratic root majorant needed for a local linear fluctuation map.

For the actual nonlinear constrained map, a further estimate on the map is required. If T(z) has a represented local analytic expansion with

    sum_{links in root} |T_link(z)|^2
       <= C [R_Z(v)+z^T P_Z z]

on the localization polydisc, with the genuine carrier and the same trace bound as (G3.2), G3 applies without any additional source-specific Gaussian estimate. The physical-support and regulator assertion in this displayed condition is **not proved here for arbitrary completed-R histories**. CMP 116's componentwise decoupling argument verifies support for its regular propagator/minimizer localization; transferring that support through the full retained-history reconstruction is precisely where further work is needed.

## 5. Centering the Gaussian current prevents a spurious grade-two loss

The norm M-03 gives a one-mark current grade 3/2. Bounding an uncentered product of two energies can incorrectly suggest grade 2. The exact normalized Gaussian current has cancellation inside the current record itself.

Let q_y=N(m(y),C(y)), K=C^(-1), j=Km, all differentiable along a retained direction. Let the specified insertion be

    F(z)=f_0+a^T z+(1/2)z^T A z,

with A symmetric and with its own direct derivative handled separately. A prime denotes the retained direction, and define ell=j'-K'm. The normalized score is

    S(z)=ell^T(z-m)
          -(1/2)[(z-m)^T K'(z-m)-Tr(CK')].                 (G5.1)

It has q_y mean zero. The new normalized-kernel current is exactly

    J=Cov_q(F,S)
      =(a+Am)^T C ell-(1/2)Tr(A C K' C).                   (G5.2)

**Proof.** Differentiate the Gaussian density and its normalizer. The formula for S follows by writing z=m+xi and subtracting the mean. The centered insertion is

    (a+Am)^T xi+(1/2)(xi^T A xi-Tr(AC)).

Odd Gaussian moments vanish. Wick's identity gives
Cov(xi^T A xi,xi^T K' xi)=2Tr(ACK'C). This proves (G5.2). QED.

The consequent bound is

    |J| <= ||C^(1/2)(a+Am)|| ||C^(1/2)ell||
            +(1/2)||C^(1/2)AC^(1/2)||_HS
                      ||C^(1/2)K'C^(1/2)||_HS.            (G5.3)

The right side has at most quadratic external-field growth when m is affine, a has at most linear growth and ell has at most linear growth. It fits a grade-3/2 native regulator whenever those linear coefficients and their physical support sums are controlled. This calculation retains the precision response and the Gaussian normalization response; neither is silently discarded.

For a finite difference, integrate (G5.2) along the actual retained path, keeping the insertion specified. A fixed-path scalar multiplication identity does not justify a path that leaves the admitted chart. For hard selector changes or rank changes, a separate signed-kernel difference remains necessary.

The formula is for the Gaussian factor. E/B/R and coarea responses contribute additional scores, and live selectors contribute additional signed measures. Those are not zero and are not covered merely by calling the whole regular measure Gaussian.

## 6. Precise contribution to M-04

Proved here:

1. A dimension-independent, termwise marked Gaussian majorant with a trace cost. It applies to the actual joint Gaussian in the CMP 116 localization step whenever its root energy is given in that step's coordinates.
2. An exact compact Wilson inequality furnishing the quadratic root energy before nonlinear pullback/localization.
3. The exact centered current for the variable Gaussian precision and force, including its normalizer, with no artificial quartic external growth.

Still not proved:

1. The source-specific nonlinear pullback/localization bound (G3.2), with full physical support and native-regulator control, for all completed retained histories allowed in the current M-04 statement.
2. The complete ambient raw/selector/history finite-difference estimate. Analyticity on an admitted chart does not bound the M-03 ambient supremum across a hard selector or the prescribed inactive-kernel extension.
3. The physical incident background bounds SR20.22a after normalized fixed-component operations. The source's relative d(X minus Y) estimate does not pay exp(kappa |Y|).
4. Scalar/identity extraction of this same full output and the resulting M-03 remainder.

The Gaussian insertion itself is no longer a reason to introduce p(g)^2 or an ambient-volume factor. The unresolved part is the actual supported nonlinear root and its full-history/current budget.

## 7. Subspaces, hard cutoffs and nonquadratic roots

### 7.1 The covariance acts on the actual free subspace

G1–G3 do not require a nonsingular covariance on an artificially padded ambient space. Let E be the actual free integration subspace, with its inherited Euclidean metric. Apply the theorems to A_E on E. If P is specified in the ambient space, replace it by P_E=Pi_E P Pi_E restricted to E. Then

    ||P_E||<=||P||,  Tr_E P_E<=Tr P,  rank P_E<=rank P.

The determinant in G2 is the determinant on E. The exceptional-bond elimination in the primary construction is specifically intended to leave such independent free coordinates. An arbitrary padded gauge zero mode must not be assigned a fictitious precision.

If the actual coercivity estimate is A>=a D^2 rather than A>=a I, use w=Du. The required root trace is then Tr(D^(-1)P D^(-1)), not Tr P. A local rank alone is insufficient: its weighted eigenvalues must be bounded. Thus the uniform operator assumptions on C and C Gamma in G3 must be checked in the same normalized coordinates as the insertion and the current. The printed CMP116 Gaussian estimate verifies its own regular chart; this note does not infer the heterogeneous all-history bounds from it.

### 7.2 Exact Gaussian response for a nonquadratic insertion

Let q=N(m,C) on a fixed free space, and let F be twice continuously differentiable with polynomially bounded derivatives. For a varying mean and covariance,

    (d/dt) q_t F |_(t=0)
      = m' . q(grad F)+(1/2) C' : q(Hess F).               (G7.1)

The insertion is specified in this formula. Any explicit t-derivative of F is a separate direct record.

**Proof.** The normalized score identity is valid first for smooth compactly supported F. Write the score as (G5.1), and apply one Gaussian integration by parts to its linear part and two to its centered quadratic part. Since m'=C(j'-K'm) and C'=-CK'C, (G7.1) follows. Approximate a polynomial-growth F by compactly supported functions and use Gaussian integrability of the derivatives to pass to the limit. QED.

Consequently, if a localized nonquadratic scalar has

    |grad F(z)| <= M [r+z^T P z]^(1/2),
    ||Hess F(z)|| <= M,

then

    |J| <= M |m'| [r+m^T P m+Tr(PC)]^(1/2)
               +(M/2)||C'||_trace.                        (G7.2)

For a local dependence F(z)=f(Lz), use the corresponding bound in L-coordinates. The trace cost becomes ||L C' L^T||_trace, avoiding an ambient-rank estimate. The compact Wilson scalar composed with a fixed local affine normalized fluctuation map has these derivative bounds: its first derivative has the square-root-energy bound from SR20.1, and its second derivative is bounded by a fixed constant because each pair of normalized link derivatives contributes beta/(1+beta)<=1. Nonlinear map Hessians add their exact chain-rule term and must be estimated separately.

**Hard-cutoff warning essential to the proof:** (G7.1) is not automatically the response formula for the source's truncated Gaussian on K. Integration by parts there has boundary terms. Treating the cutoff as part of F makes its distributional derivatives appear in (G7.1), so it does not remove those terms. The next inequality avoids that error.

### 7.3 The actual fixed-support convex law has a dimension-free score estimate

Let q(dz)=Z^(-1) exp(-V(z)) 1_K(z) dz on a fixed convex domain K in E. Assume the complete Hessian satisfies Hess V>=a I, with the reflecting covariance realization of C-07/C-08. Let

    S_0(z)=j'^T z-(1/2)z^T K' z

be the actual precision/force part of the retained score; its centered form is S=S_0-qS_0. Let m=qz. Then every differentiable F with finite displayed quantities obeys

    |Cov_q(F,S)|
      <= a^(-1) [q|grad F|^2]^(1/2)
          [|j'-K'm|^2+a^(-1)||K'||_HS^2]^(1/2).           (G7.3)

**Proof.** Cauchy–Schwarz for covariance and the convex-domain Poincare inequality yield

    |Cov(F,S_0)|<=a^(-1)[q|grad F|^2]^(1/2)
                             [q|j'-K'z|^2]^(1/2).

The cross term in z=m+(z-m) vanishes after taking q. For each row r of K', the same Poincare inequality applied to the linear functional r.z gives Var(r.z)<=a^(-1)|r|^2. Summing the rows proves

    q|j'-K'z|^2<=|j'-K'm|^2+a^(-1)||K'||_HS^2.

This proves (G7.3). The use of the reflecting covariance/Poincare theorem is justified by the fixed convex K; no vanishing boundary density is assumed. QED.

For the nonquadratic compact scalar, q|grad F|^2 is bounded by its actual first-order energy moment, rather than by a second energy moment. If that energy moment is O(R), the response in (G7.3) has size O(R) whenever |j'-K'm| and the local Hilbert–Schmidt score cost are O(sqrt(R)). More generally O(R) for those two score costs gives O(R^(3/2)), which is exactly the allowed M-03 current grade. This is a proved reduction of the current's polynomial cost; it does not prove the required score coefficients or their carrier sums.

The same reasoning applies to an additional smooth score term S_W=partial_v W:

    |Cov_q(F,S_W)|
      <= a^(-1)[q|grad F|^2]^(1/2)[q|grad S_W|^2]^(1/2).

Thus E/B/R/coarea scores can be retained explicitly when their mixed derivative costs are known. Moving selectors, rank changes and inactive-kernel extensions are not smooth scores and remain outside this inequality.

Finally, a spatial covariance bound may replace the scalar a^(-1) Poincare constant to preserve decay between the insertion gradient and the score gradient. Such a bound still gives decay of a numerical response. An actual decomposition into supported functions, and hence the full M-03 carrier norm, requires the separate localization construction. This is why neither G7.2 nor G7.3 alone completes SR20.23.
