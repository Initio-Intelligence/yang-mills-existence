# The finite-probe complement and the missing engineering jet

The scalar projector SE is a bounded complement to the fixed scalar and identity directions. This note proves an exact limitation: its kernel need not annihilate even the zero-momentum Wilson quadratic jet. The example uses the actual repaired F01 plaquette scalar and belongs to the same local energy/current class. It does not assert that the third-step microscopic output is this example, and it does not rule out a different renormalized quotient norm.

There are also two positive results: an exact second-moment subtraction and smearing estimate for translated scalar stencils, and fixed-order field-jet bounds for the actual smooth three-step baseline. Neither is promoted to an engineering contraction for the full microscopic carrier norm.

## 1. The exact scalar and its local class

At spacing \(h\), use the repaired F01 scalar and its energy coordinate:
\[
 \varphi_h(x)=\beta_h\sigma_h(x),\qquad
 \sigma_h(x)=\frac{2}{\sqrt6}\frac1{4h^4}
       \sum_{\mu<\nu}\sum_{\epsilon,\epsilon'=\pm1}
         s(P_{\epsilon e_\mu,\epsilon'e_\nu}(x)),
 \qquad s(P)=N-\operatorname{ReTr}P .
 \tag{EJ.1}
\]
Each of the twenty-four terms is the energy of a geometric plaquette with \(x\) as one vertex. The four vertex placements of each plaquette give the exact identity
\[
 h^4\sum_x\varphi_h(x)=\frac{2\beta_h}{\sqrt6}\sum_ps(U_p).
 \tag{EJ.2}
\]
This is SE.1 and is exact, without a clover approximation.

Define the symmetric nearest-neighbor average
\[
 (\mathsf T_h\varphi_h)(x)
     =\frac18\sum_{\mu=0}^3
            \{\varphi_h(x+he_\mu)+\varphi_h(x-he_\mu)\}.
 \tag{EJ.3}
\]
This is a gauge-invariant, reflection-even, hypercubic scalar family. It is translation covariant with the same anchor convention as \(\varphi_h\). Its full carrier is the fixed union of the eight neighboring scalar stencils, with the paths to the original anchor retained.

Both fields have a pointwise native energy/current budget independent of \(h\), volume and \(\beta_h\ge1\), apart from the displayed factor \(h^{-4}\). Indeed \(s\ge0\), so their values are bounded by a fixed multiple of the retained plaquette energy on that union. For a normalized link displacement of physical size \(g_h\), a plaquette response satisfies
\[
 |\delta(\beta_hs(P))|
       \le C\{1+\sqrt{\widehat E_{\partial P}}\},
 \qquad \beta_hg_h^2=1/N.
 \tag{EJ.4}
\]
This follows by expanding the first Wilson derivative about \(P=I\), where it vanishes, and retaining the bounded second-order remainder along the shifted path. Each link meets finitely many stencil plaquettes. Summing directions therefore gives the native current grade \(3/2\), in fact a stronger grade on these elementary fields.

The finite average preserves any separately established outer moment budget by the triangle inequality and the union regulator. No such outer-law hypothesis is needed for the pointwise statements here.

These fields have the same two-curvature-leaf structure used by the marked estimates: the exact holomorphic Wilson trace is quadratic in \(P-I\), and translating or averaging its stencil does not remove those leaves. They are thus members of the actual gauge-invariant local readout class; no hypothetical non-gauge-invariant potential is being substituted.

## 2. Exact finite-probe calculation

Use the SE probe at anchor \(x\): every link is identity except
\[
 e=(x,x+he_0),\qquad
 U_e=\exp\{tH/\sqrt{1+\beta_h}\},
 \quad H=\frac{i}{\sqrt2}\operatorname{diag}(1,-1,0,\ldots,0),
 \quad 0<t\le1/4 .
 \tag{EJ.5}
\]
Assume the torus is large enough that the stencils below do not wrap onto themselves. Let \(s_*>0\) be the common nontrivial plaquette energy of this pulse. Exactly six geometric plaquettes contain \(e\): one in each of the two transverse directions for each of the three transverse axes.

For a scalar anchored at \(y\), count which of these six plaquettes have \(y\) as a vertex. The complete neighbor incidence is

| Anchor \(y\) | Number of affected plaquettes in its scalar stencil |
|---|---:|
| \(x\) | 6 |
| \(x+he_0\) | 6 |
| \(x-he_0\) | 0 |
| Each \(x\pm he_\nu\), \(\nu\ne0\) | 1 |

The sum in the eight neighboring stencils is therefore \(6+0+6=12\). All terms have the same scalar normalization and the same \(s_*\). It follows exactly that
\[
 \frac{(\mathsf T_h\varphi_h)(x;U^{\rm pulse})}
                  {\varphi_h(x;U^{\rm pulse})}
       =\frac{12}{8\cdot6}=\frac14 .
 \tag{EJ.6}
\]
The all-identity value is zero. Reversing the pulse axis, permuting coordinates, or conjugating its colour generator does not change the count or the Wilson energy. Hence the actual finite symmetry average in SE has the same coefficient.

### Proposition EJ.1 — the probe kernel retains a marginal Wilson component

SE's scalar/identity extraction applied to \(A_h=\mathsf T_h\varphi_h\) gives
\[
 a_{\rm SE}=\frac14,\qquad c_{\rm SE}=0,\qquad
 \mathcal R_{\rm SE}
       =\mathsf T_h\varphi_h-\frac14\varphi_h.
 \tag{EJ.7}
\]
Its remainder vanishes at the reference and the averaged pulse, but
\[
 h^4\sum_x\mathcal R_{\rm SE}(x)
       =\frac34\,h^4\sum_x\varphi_h(x)
       =\frac34\frac{2\beta_h}{\sqrt6}\sum_ps(U_p).
 \tag{EJ.8}
\]

**Proof.** Equation (EJ.6) is exactly SE's coefficient formula, and the reference gives \(c=0\). Translation is a bijection on the periodic lattice, so summing the normalized neighbor average gives the same sum as \(\varphi_h\). Subtract its one-quarter multiple. ∎

Centering the incoming scalar by a constant changes only the identity coordinate and leaves this remainder calculation unchanged. Converting to the prescribed F01 normalization rescales both scalar coordinates by the same nonzero factor; it also does not repair the discrepancy.

To state the quadratic-jet consequence explicitly, let \(A\) be an anti-Hermitian lattice one-form and \(U_e(\tau)=\exp(\tau A_e)\). At the identity,
\[
 s(U_p(\tau))
      =\frac{\tau^2}{2}\|(dA)_p\|_{\rm HS}^2+O(\tau^3).
 \tag{EJ.9}
\]
Thus the quadratic Taylor coefficient of the integrated scalar is
\[
 {\cal J}_2(\varphi_h)[A]
 :=\frac12\left.\frac{d^2}{d\tau^2}
       h^4\sum_x\varphi_h(x;U(\tau))\right|_{\tau=0}
 =\frac{\beta_h}{\sqrt6}\sum_p\|(dA)_p\|_{\rm HS}^2 .
 \tag{EJ.10}
\]
It is nonzero on a cochain with nonzero curl. Equation (EJ.8) gives
\[
 {\cal J}_2(\mathcal R_{\rm SE})
          =\frac34\,{\cal J}_2(\varphi_h).
 \tag{EJ.11}
\]
In particular the zero-source-momentum Wilson quadratic jet is not annihilated. This conclusion is not an inference from the probe alone: it follows from the exact integrated identity (EJ.8). It even holds for the whole integrated quadratic functional, before taking a low-gauge-momentum limit.

The example disproves the implication

> gauge invariance + hypercubic scalar symmetry + the proved local energy/current and curvature-leaf bounds + membership in the finite-probe kernel imply removal of the marginal Wilson jet.

It does not prove that no iterated operator with such a complement can contract in a different quotient norm. Nor does it identify the actual conditional output with this stencil average.

## 3. The correctly subtracted stencil and its exact second difference

Define the lattice Laplacian
\[
 (\Delta_h f)(x)=h^{-2}\sum_{\mu=0}^3
       \{f(x+he_\mu)+f(x-he_\mu)-2f(x)\}.
 \tag{EJ.12}
\]
The exact algebraic identity is
\[
 \mathsf T_h\varphi_h-\varphi_h
       =\frac{h^2}{8}\Delta_h\varphi_h.
 \tag{EJ.13}
\]
Consequently the SE remainder has the explicit decomposition
\[
 \mathcal R_{\rm SE}
       =\frac34\varphi_h+\frac{h^2}{8}\Delta_h\varphi_h.
 \tag{EJ.14}
\]
The coefficient that removes the zero-momentum Wilson component of this particular family is 1, not \(1/4\).

The second term is a total lattice second difference. In a smooth long-distance expansion it has two more spatial derivatives than the scalar. This is the precise dimension-six interpretation used here. It is not a pointwise regularity assertion about arbitrary microscopic gauge configurations.

### Proposition EJ.2 — exact smearing gain

Let \(f\) be the restriction of a periodic \(C^2\) function to a finite periodic lattice. Alternatively take a compactly supported \(C^2\) test on the infinite lattice, with absolute convergence of the sums below. Then
\[
 h^4\sum_x f(x)\{\mathsf T_h\varphi_h-\varphi_h\}(x)
       =\frac{h^2}{8}\,h^4\sum_x(\Delta_hf)(x)\varphi_h(x).
 \tag{EJ.15}
\]
If
\[
 \sum_{\mu=0}^3\|\partial_\mu^2 f\|_\infty
          \le C_f H^{-2},
 \tag{EJ.16}
\]
then
\[
 \left|h^4\sum_x f(x)
             \{\mathsf T_h\varphi_h-\varphi_h\}(x)\right|
 \le\frac{C_f}{8}\left(\frac hH\right)^2
        h^4\sum_{x\in{\rm supp}(\Delta_hf)}\varphi_h(x).
 \tag{EJ.17}
\]
The set on the right may be replaced by the one-link enlargement of the support of \(f\).

**Proof.** Shift the lattice sums in (EJ.13); \(\Delta_h\) is self-adjoint for the periodic counting measure, or for the convergent compact-support pairing. For each coordinate,
\[
 h^{-2}\{f(x+he_\mu)+f(x-he_\mu)-2f(x)\}
   =\int_{-1}^1(1-|s|)
           \partial_\mu^2 f(x+she_\mu)\,ds.
 \tag{EJ.18}
\]
The triangular kernel has mass one, so (EJ.16) bounds
\(\|\Delta_h f\|_\infty\). Use \(\varphi_h\ge0\) in (EJ.15). ∎

For \(H=Lh\), (EJ.17) displays \(L^{-2}\). It arises by moving a second difference onto a \(C^2\) test. It does not estimate the absolute microscopic carrier sum of a conditional expectation, its kernel response or an unsmeared field. In particular (EJ.17) is not the missing M07 operator contraction.

## 4. A whole translated-stencil class

The same exact mechanism extends beyond the nearest-neighbor example. Let \(k(y)\) be a real finite-support kernel on \(\mathbb Z^4\), or an absolutely summable kernel with
\[
 \sum_y|k(y)|(1+|y|^2)<\infty,\qquad
 m_0=\sum_yk(y),\qquad
 \sum_y y_\mu k(y)=0\quad(\mu=0,1,2,3).
 \tag{EJ.19}
\]
An even kernel has the last property. Set
\[
 F_k(x)=\sum_yk(y)\varphi_h(x+hy),\qquad
 I_k=F_k-m_0\varphi_h .
 \tag{EJ.20}
\]
Its integrated sum and Wilson quadratic jet vanish exactly. For a periodic or convergent compact-support pairing, Taylor's integral remainder and the vanishing first moment give
\[
 \begin{split}
 \left|h^4\sum_x f(x)I_k(x)\right|
 \le{}&\frac{h^2}{2}
       \left(\sum_y|k(y)||y|^2\right)
       \|\nabla^2 f\|_{\mathrm{op},\infty}
       h^4\sum_{x\ {\rm met\ by\ the\ translated\ test}}\varphi_h(x).
 \end{split}
 \tag{EJ.21}
\]
For a finite kernel this is immediate by shifting \(f(x)\) to \(f(x-hy)\); for an infinite kernel use dominated convergence with the displayed second moment and the assumed convergence of the energy pairing.

When the kernel has the corresponding exponential carrier budget, assign each translated scalar its full stencil and a connecting carrier to \(x\). The local value and first-current bounds follow by the same absolute sum as in Section 1. Thus moment subtraction is a genuine bounded operation for this simple scalar class, and it has the proved smearing gain. No conditional normalizer is involved in this example.

The finite-probe coefficient on that class is instead the linear functional
\[
 a_{\rm SE}(F_k)=\sum_y k(y)\frac{n_y}{6},
 \tag{EJ.22}
\]
where \(n_y\) is the number of pulse plaquettes incident to \(x+hy\), with the finite symmetry average understood. This overlap functional is generally different from \(m_0\). The failure is therefore structural, not an error in the pulse denominator.

## 5. What finite field jets the actual smooth third baseline already has

There is a useful positive input beyond the stencil example. The actual all-auxiliary three-step baseline in TR has fixed free-coordinate domains and one common analytic coefficient/normalization family. It therefore has finite raw field jets at the flat final field, with full carrier moments.

For a final link/Lie-coordinate list \(\mathbf a=(a_{e\ell})\), use
\[
 W_e(\mathbf a)
   =\exp\!\left(g_3\sum_\ell a_{e\ell}T_\ell\right),
 \tag{EJ.23}
\]
where \(T_\ell\) is a fixed anti-Hermitian basis. Let \(A_Z^A\) be TR's common smooth-baseline value tags, and let \(x^{(3)}\) be the insertion anchor. For \(1\le q\le5\) define their normalized field jets by
\[
 K_{Z;\mathbf e,\boldsymbol\ell}^{(q)}
    =\left.
       \partial_{a_{e_1\ell_1}}\cdots
       \partial_{a_{e_q\ell_q}}
             A_Z^A(W(\mathbf a))\right|_{\mathbf a=0}.
 \tag{EJ.24}
\]

### Lemma EJ.3 — fixed-depth smooth field jets and second spatial moments

For a strictly smaller carrier rate \(\kappa'<\kappa\), the fixed-three construction gives
\[
 h_3^4\sum_{Z\ni x^{(3)}}e^{\kappa'n(Z)}
       (1+\operatorname{diam}_{h_3}(Z)^2)
       \sum_{\mathbf e,\boldsymbol\ell}
               |K_{Z;\mathbf e,\boldsymbol\ell}^{(q)}|
       \le C_{L,q,\kappa-\kappa'}L^{12}b,
 \quad 1\le q\le5.
 \tag{EJ.25}
\]
Directions not read by \(Z\) have zero derivative. The constants are for three fixed levels.

**Proof.** Keep the same source-root and unmarked component registries used in TR.33. Continue at most five normalized final coordinates simultaneously on fixed small discs. Their physical size is \(O(g_3)\); the finite compositions in TC/NC remain in the same fixed native tube for sufficiently small coupling. The first and second inner domains and the newest auxiliary P domain remain fixed. The coefficient caps are fixed in the real integration variables, so no nonholomorphic guard is continued in the raw coordinates.

At the flat real center, those finitely many discs add only a fixed amount to the positive final-energy allowance. Choose the source radius from that one enlarged box before any derivative. The same D0,D1,D2 stores and the three exact normalizations in TR apply. Repeated Cauchy on those fixed coordinate discs bounds a specified derivative tuple by the same absolute tagged majorant times a constant depending on q. This also covers repeated coordinates.

The number of possible coordinate tuples read by a carrier is at most \(C_L^q(1+n(Z))^q\). The diameter of a connected carrier is bounded by a fixed multiple of its volume-plus-tree size. The smaller exponential rate pays these polynomial factors. Source Cauchy is performed once, to recover the microscopic insertion; field derivatives do not introduce new independent marked stores. Restore the classical background coefficient with its analytic matrix/force/mismatch family, using the same finite coordinate discs. This proves (EJ.25). ∎

This supplies existing fixed-depth derivatives and moments of the smooth baseline. It does not show that the finite-probe remainder has vanishing low-order jets, as Proposition EJ.1 already disproves in the readout class. Nor does (EJ.25) exhibit a sharp power of L or constants uniform in the number of integrations.

The lemma is deliberately not stated for the completed sharp-Q density or its entire conditional scalar. Those were proved with primitive real-domain first jets, not with a higher raw-derivative theorem. The old cutoff cores must remain as their exact integral payloads unless additional regularity is proved.

## 6. The primary-source renormalization mechanism is a different operation

The relevant unmarked mechanism can be located precisely in CMP109:

- Section 3, printed pp.270--280, constructs the background/force analytic extension and the finite Taylor expansion (3.34). Its admission is checked before bounding the Taylor remainder.
- Section 4 uses gauge identities and spatial Taylor localization on those tensors; the nonlocal terms and their genuine derivative locations are retained.
- Section 5, printed pp.296--298, isolates the Wilson polarization tensor in (5.36)--(5.37). The coefficient is obtained from the appropriate derivatives at zero momentum, (5.39)--(5.42). The residual tensor has the higher-derivative representation (5.38), used in (5.43)--(5.44).
- The last paragraph on printed p.298 explicitly distinguishes the analytic/irrelevant reorganization from the later physical localization and cluster bounds supplied by CMP116.

These are source claims about the complete unmarked action in its declared class. They are not a theorem that a local inserted scalar with an arbitrary bounded complementary projector has a dimension-six remainder. In particular their polarization extraction is not the finite-pulse overlap functional (EJ.22).

A constant coupling/source derivative would address an integrated zero-source-momentum insertion. A local microscopic scalar needs the source-anchor dependence and its spatial moments as well. One cannot silently replace that local-source problem by the translation-invariant constant-coupling problem, or differentiate adaptive running maps and cutoffs while claiming a specified-source transport identity.

## 7. The exact remaining marked jet statement

To turn the current fixed-depth result into an engineering contraction, a further theorem must do more than bound another finite projection. In the actual common primitive marked family it must:

1. **Define the marginal jet.** Identify the identity and the zero-momentum Wilson scalar jet in the source-position-dependent field vertices, with all gauge Ward identities, reflection/placement conventions, and any other allowed dimension-four channels kept. Matching the quadratic scalar coefficient alone must be accompanied by the identities tying its nonabelian lower field vertices to the same invariant.
2. **Subtract that jet in the same actual source family.** The remainder must have the appropriate vanishing low field/momentum moments before the absolute carrier sum. The exact own-normalizer and path-origin records must be retained; a value-level Taylor subtraction cannot silently reassign a kernel current.
3. **Prove a scale-sharp transfer bound.** After the actual conditional integration and rescaling, the vanishing-jet family must gain a power such as \(L^{-2}\), with constants controlled as L is chosen and uniformly through the admissible depths. A bound written merely as \(C_L\) cannot supply that gain. It must include both force and average-mismatch reconstruction leaves, all physical \(g_i\) factors, joint Gaussian stores, and the inherited denominator.
4. **Keep the nonanalytic core ledger separate.** Sharp Q payloads presently have real first-jet integral certificates and birth reserves. Higher raw Taylor regularity for their integrated values is not supplied by TS. A valid induction must either prove such a theorem or continue their exact primitive core representation with its reserves and source/current labels.

Lemma EJ.3 supplies finite smooth field derivatives and moments at three levels. The source equations above suggest a concrete route for their Ward/momentum organization. The scale-sharp marked transfer, its uniform-depth constants, and the complete hard-core treatment are not proved by that lemma.

The exact example (EJ.7)--(EJ.14) explains why the gap cannot be filled by calling the already bounded SE remainder “irrelevant.” SE and TS remain valid bounded extraction results. The additional engineering statement needs a different quantitative jet argument and, if a different projector is used, an explicit comparison of its scalar and identity coordinates with the prescribed incoming basis.
