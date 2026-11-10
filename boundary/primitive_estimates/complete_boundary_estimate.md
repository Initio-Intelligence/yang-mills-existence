# The complete boundary estimate on coarsened atoms

## 1. The statement and the atomic representation

The C-05 statement of the catalogue asks for the same local derivative
bounds for the actual boundary activities as for the regular activities,
including collars, constraints and current-coordinate dependence. Its
constants must be independent of total volume and hidden carrier distance.
The identified C01 construction, its admitted positive histories and its
stipulated trajectory are retained as inputs. The desired boundary
estimate is not assumed.

One passage of the positive norm needs care. A linear prefix block is
summed with cancellation, and one must prove that its sum, rather than its
separately localized pieces, can be carried through every later
localization and Gaussian construction. A common future self/nonself
status alone does not prove that passage.

The passage is handled by an explicit atomic representation. A complete internally
resummed protected block is one atom. Its remaining physical connector,
actual raw-variable owners, native dependence and original creation
capacity are retained. Coarsening is performed before any later native
Taylor expansion or Gaussian conditioning. The common Gaussian family
is then selected from the genuine new map-factor supports.

This representation is permitted by the source. CMP119, printed p.262,
allows resumming boundary terms meeting a given large-field component,
with declared domains containing the component or missing it, and states
that the constructions and estimates continue to hold with the resulting
outside-tree bound. The convention is selected once for the iteration.
It is not a claim that independently chosen historical localization
families have identical intermediate coefficients.

This scalar resummation permission does not make an arbitrary large-field
component a free core of the additional positive norm. Only the bounded
source-eligible protected components receive that role. Unbounded
ordinary regions retain their physical support and paid connectors;
the non-small ordinary \(B/C_0\) family remains in its ordinary
reference and native bookkeeping.

The proof below combines the coarsening and normalization lemmas
with the current and native endpoint estimates of
[Current endpoint estimates for boundary activities](../current_endpoints.md)
and [Summation at a native root on a two-sided trajectory](native_roots.md).
It addresses the unchanged C05 target, including its unsubtracted native
clause. The separate existence requirements are not
used as assumptions that would imply C05.

## 2. Statement with the original quantifiers

Fix the gauge group, blocking factor, source geometric constants and
cutoff exponents. Use the actual C01 conditional density, with its
constrained quadratic form, retained exterior force, complete action,
Haar/coarea terms, selectors and boundary Jacobian in their identified
positions. Retain the source trajectory envelope
\[
 t_K+a(K-j)\le t_j\le t_K+A(K-j),\qquad
 t_j=g_j^{-2},\quad 0<a\le A.
 \tag{FC.1}
\]
Put
\[
 \ell_j=\log t_j,\qquad P_j=A_1\ell_j^{p_0},\qquad
 c_R\ell_j^r\le R_j\le C_R\ell_j^r,\qquad r>1.
 \tag{FC.2}
\]
The source rounded radii, actual domains and preparation schedule are
unchanged. Raw retained fields and discrete history labels have exactly
the fixed roles assigned to them in C01. Native variables include the
independent current and every genuinely surviving preparation slot.

### Theorem FC.1 — the complete C05 boundary estimate

There is one common weak-coupling ceiling and fixed positive spatial
rates such that the following statements hold for every finite admitted
torus, every cutoff depth, every scale, and every admitted ordinary,
preliminary, failed and completed history.

Let \(B_k(z,\xi)\) be the complete boundary scalar in the consistently
chosen source representation. The current chart contains the full
unprimed real support \(|z_i|\le P_k\) and a common complex \(2P_k\)
neighborhood. On that support and a common smaller native chart,
\[
 \sup_{(z,\xi)}\sup_i
   \sum_j e^{\gamma\rho_k(i,j)}
          \|D_iD_jB_k(z,\xi)\|_{\mathrm{op}}
 \le C K_{B,k}P_k^{-2},
 \qquad
 K_{B,k}=O(1),\quad K_{B,k}P_k^{-2}\longrightarrow0.
 \tag{FC.3}
\]
The supremum is outside the endpoint sum. For every integer \(m\ge1\),
with the same ceiling and constants independent of \(m\), the
corresponding all-current estimate is
\[
 \sup_{(z,\xi)}\sup_{i_1}
 \sum_{i_2,\ldots,i_m}
 e^{\gamma\tau_k(i_1,\ldots,i_m)/m}
 \|D_{i_1}\cdots D_{i_m}B_k(z,\xi)\|
 \le C^{m+1}(m!)^5K_{B,k}P_k^{-m}.
 \tag{FC.4}
\]
For local joint native directions on the original strong chart
\(\alpha^-_j=Cg_j\ell_j^q\), \(q>p_0+r+2\), the unsubtracted
scalar has a positive local activity representation satisfying
\[
 \sum_G w_G
   |D_{h_1}\cdots D_{h_m}F_G|
 \le C^{m+1}m!K_{\mathrm{nat}}\,
       N_{\mathrm{nat}}(S_1)
       \prod_{\ell=1}^m\|h_\ell\|_{\mathrm{slot}} .
 \tag{FC.5}
\]
Here \(S_1\) is the actual source support of the first direction and
\(N_{\mathrm{nat}}(S_1)\) counts its native cells with the fixed
partition/stencil enlargement, rather than a fine subdivision of
a coarse native cell. Equation (FC.5) holds for every integer
\(m\ge1\), uniformly in all points, fixed real raw tuples and
histories just quantified, with \(C,K_{\mathrm{nat}}\) and the
ceiling independent of \(m\). The first direction may have zero
current component. In particular,
the estimate includes \(B_k(0,\xi)\). Every preparation direction
uses its actual disk and native map, rather than being assigned a
field-direction radius by definition.

All constants are independent of total volume, depth, the number of
attempts and the number of completed components. Their allowed
dependence on the fixed source constants and trajectory constants
is chosen before the ceiling.

## 3. Exact coarsening, before an absolute estimate

At a finite cutoff, let \(s_\Delta\) be the source localization
parameters. Define
\[
 E_\Delta f=f|_{s_\Delta=0},\qquad
 D_\Delta f=\int_0^1\partial_{s_\Delta}f\,ds_\Delta.
 \tag{FC.6}
\]
For a finite protected set \(\mathcal D\) of these labels,
\[
 \prod_{\Delta\in\mathcal D}(E_\Delta+D_\Delta)f
       =f|_{s_\Delta=1,\ \Delta\in\mathcal D}.
 \tag{FC.7}
\]
This follows from the fundamental theorem of calculus and commutation
of distinct parameter operations. The equality holds on the complete
native family. In particular it is stronger than equality of the final
physical function at one field.

The internal localizer pieces of a zero-remote prefix block have
carriers between an original carrier \(X\) and its protected
completion \(X\cup D(P)\). Summing the internal choices by (FC.7)
leaves one bounded analytic insertion \(F\). For every remaining
external localization choice, the coefficient is obtained by applying
the common external operators to \(F\). There is no factor equal to
the number of internal labels.

The positive norm is therefore
\[
 \mathcal A=
 \sup_{\mathfrak h,a_{\mathrm{ext}}}\sup_x
 \sum_{G\ni x}
 e^{\nu n(G)+\eta q(G)+\lambda L(G)}
 M_{\mathrm{pref}}^{u(G)}
       \sup_{\xi\in\mathcal D^+}|F_G(\xi;a_{\mathrm{ext}})|.
 \tag{FC.8}
\]
Here \(F_G\) is a complete resummed block, not one of its canceled
internal pieces. The real exterior supremum remains outside the
positive sum. Its native supremum remains inside. The protected
footprint is support data; only the actual bounded component core
may be traversed without a paid connector.

Original internal labels remain available to identify the literal
self sum. If a later self region contains \(X\), the deep owner and
ordinary buffer force it to contain \(P\) and \(D(P)\). Otherwise
no member of this block is self. The projection thus commutes with
the block sum. At an interior R step the first source completion
fills that same component, so the determining maps in LFR II
(1.61)–(1.65) are common as well.

These are PC.1, PC.2 and PC.5 in
[Coarsened protected atoms and the positive catalog](positive_catalog_coarsening.md).
All identities refer to one consistently chosen source
representation. No equality with a differently localized historical
representation is needed.

## 4. The Gaussian step does not reopen the canceled pieces

At the next ordinary step the protected footprint is behind the
ordinary large-field enclosure. It has no newly integrated current
Gaussian coordinate.

First expand the whole \(F\) through its actual current map:
\[
 F(U_0+v(A))
 =\sum_{m\ge0}\frac{1}{m!}
       D^mF(U_0)[v(A),\ldots,v(A)].
 \tag{FC.9}
\]
The old coefficient is external to \(A\). For a fixed tuple of
new map records, let \(J\) be their genuine Gaussian supports,
together with any explicit primitive factors occurring in that
same term. Choose the conditioning and generalized-walk family
once for this \(J\), after summing the old coefficient.

Gaussian conditioning is the unlocalized identity CMP116 (2.5).
Its extension to the admitted native family is made before the
new localization parameters are introduced. The subsequent
covariance, precision and square-root families are the source
ones on this single choice of support. No independently
localized inverse identity is asserted.

The algebra
\[
 D^m\Bigl(\sum_iF_i\Bigr)=\sum_iD^mF_i
 \tag{FC.10}
\]
then survives the conditional integral and every new localization
coefficient, because those operations are linear in the external
multilinear coefficient. The map factors retain their true
endpoint locations and physical decay.

Consequently the Gaussian comparison uses
\[
 |J_0|\le C\,[L_{\mathrm{paid,current}}+1+V_{\mathrm{new}}],
 \tag{FC.11}
\]
with no artificial volume from \(D(P)\). The source normalized
cluster expansion keeps the distinguished numerator insertion
and the same denominator, CMP119 (3.44)–(3.47). Its zero-new-map
term is exactly the carried scalar.

This proves the ordinary-step compatibility required by the
norm argument. PC.4 and ND.4 give the complete construction and
an independent verification.

## 5. Whole-prefix normalization on the actual source geometry

For an eligible attempted component \(P\), LFR I p.177 adopts
the componentwise intersection convention \(Z_j=Z_j\cap P\)
and the bounded rectangular ancestral sequence. Its operative
domains are continued on pp.179–180, 192 and 195. Counting the
actual stage strip on its own mesh gives
\[
 D_j(P)\le C_G(1+100LMR_{j+1})^4.
 \tag{FC.12}
\]
Both the \(A_j\) and \(B_j\) free coordinates are included.
The deep \(T_h\) variables remain external. [CT.1](operative_source_scope.md) and ND.1
prove the grid conversion explicitly.

This does not restrict ordinary histories to a single component.
It uses the source's own condition only where that source
performs a preliminary R sequence. A collection of arbitrarily
many unrelated ancestors cannot be substituted for the complete
source intersection in (FC.12).

Use the exact ordinary-tilted law of the entire stopped prefix.
Its Gaussian, Schur, constrained classical, Haar/coarea,
ordinary boundary and complete inherited \(E_r\) terms remain.
Three fixed profiles \(-,+,++\) give a phase bound
\[
 \eta_r\le
 Cg_r\ell_r^{D_1}
 +C(Q_2)\ell_r^{D_2-Q_2}
 +Cg_r^{-u}\ell_r^{D_3}e^{-cR_r}.
 \tag{FC.13}
\]
The proper-strip count (FC.12), the own Wilson subtraction
for each \(E\) birth, and the fixed old-grade sums are
performed before selecting \(Q_2>D_2+2\). The integer
\(D_2\) does not grow with that choice. The full phase
bookkeeping is ND.6–ND.17.

On one fixed larger domain, rotate out the common scalar phase.
The positive real-center probability \(\mu_0\) then dominates
the normalized complex density on the working domain:
\[
 |d\Pi_\zeta|\le M_{\mathrm{pref}}\,d\mu_0,
 \qquad M_{\mathrm{pref}}=e^{C\eta_*}\longrightarrow1.
 \tag{FC.14}
\]
ND.2 proves this from the holomorphic strip
\(\operatorname{Im}\log(p_\zeta/p_0)\in[-2\eta_*,2\eta_*]\)
and Schwarz's lemma. Thus, for the coarsened atom family,
\[
 \sum_Gw_G\sup_\zeta|\Pi_\zeta F_G|
 \le M_{\mathrm{pref}}\int
       \sum_Gw_G\sup_\zeta|F_G(\zeta,a)|\,d\mu_0(a).
 \tag{FC.15}
\]
Internal histories are averaged in this formula. They are not
separately counted with independent real-data suprema.
The moving normalizer is retained throughout.

## 6. The positive recurrence closes on these atoms

A direct prefix consumes an original source-block mark.
The whole block containing the used old coordinate lies in
the attempted component. After a retained failure its old
slots are protected by the actual source preparation rule;
after complete consumption they disappear. An unguarded
linear transport cannot recreate that mark.

The new root and diameter cost of \(D(P)\) is paid once.
For a creation at \(b\) directly used at \(r\), the actual
window and ancestor count give a fixed polynomial in
\(\ell_b\), not \(L^{4(r-b)}\). The divided-tree endpoint
weight adds at most \(e^{C\gamma R_r}\).
If the carrier exits \(P\), a distinct released paid collar
supplies that reserve. If the whole relative carrier is
contained in \(P\), its original fresh creation tail supplies
the one reserved cost. Non-small ordinary \(B/C_0\) terms
wholly inside \(P\) belong to the ordinary reference law
and are not assigned a fictitious fresh tail. PC.6a
proves these alternatives.

The positive native-map expansion is now applied to one
bounded atom. Its two connected forest sums and the
normalized component integrations are the constructions
already established in Q §§15–18 ([Positive attachment
bounds and the quotient forest](quotient_forests.md)). Source volume pays new
localizers; exact coefficient-one coarsening pays exposed
old connectors. For protected noncoarsening counts,
spending \(C\sqrt{\epsilon_k}\) extracts the nonempty
attachment contribution, where
\[
 \epsilon_k=
 Cg_k^{-u}(1+\ell_k)^v e^{-cR_k}.
 \tag{FC.16}
\]
The degree-one direct-prefix part is the carried block,
not a new source. For the degree-at-least-two part the
common-mark Cauchy estimate is
\[
 \|F_{\ge2}\|_{\mathrm{rooted}}\le CK^2/\sigma_k.
 \tag{FC.17}
\]
With \(K\) of order a fixed logarithmic polynomial times
\(\epsilon_k^{1/18}\), choose \(\sigma_k\) of order a
fixed logarithmic polynomial times \(\epsilon_k^{1/72}\).
Since \(2/18-1/72=7/72>1/18\), the new response retains
the same fresh-tail exponent.

Keep spatial positions inside each rooted catalog.
The creation-capacity sum is over the scale/operation
families after their spatial root estimates; it is not
a sum of one supremum for every spatial component.
Actual owner labels and consumed marks remain attached
to the individual records.

More explicitly, for a fixed origin family \(c=(b,\text{sector})\),
let \(\mathcal S_c(y)\) be its rooted input sum. At an actual
direct-prefix output root \(x\) of grade \(r\), choose witnesses
in the original \(b\)-block cover of \(Z_b[P]\). The proper-mesh
count and the possible direct-use window give an incidence kernel
\[
 \sum_{r\in\mathcal I_b}\sup_{x\in\mathcal R_r}\sum_y\mathsf K_{b,r}(x,y)
       \le C(1+\ell_b)^{D_*}.
 \tag{FC.18a}
\]
Here \(\mathcal I_b\) is the finite direct-use window and \(\mathcal R_r\) is the root set at grade \(r\). At a fixed grade only polynomially many eligible bounded
component footprints meet a root, each has the stated actual
ancestor cover, and only polynomially many direct-use grades
occur. After canceling consumed marks and released crossing
segments pointwise, the new-root sum is bounded by
\[
 \mathcal S^{\mathrm{out}}_{c,r}(x)
 \le e^{c_*R_b}\sum_y
      \mathsf K_{b,r}(x,y)\mathcal S^{\mathrm{in,res}}_c(y).
 \tag{FC.18b}
\]
The remaining polynomial and one exponential are the reserved
creation costs of PC.6a. These are rows in the root's actual
geometric grade, not rows formed by filling a later coarse
cell with all fine origins. An unchanged transported atom
retains its grade; its later physical-current root conversion
uses the independent endpoint age kernel in Section 7.
Taking the root supremum and then summing \(c\) therefore
introduces no spatial-volume factor.

The four exhaustive block uses in PC.6 give
\[
 A^{[k]}\le e^{C\sigma_k}A^{[k-1]}
       +f_k(F_0,A_*),
 \tag{FC.18}
\]
where
\[
 f_k(F_0,A_*)\le
 C(1+F_0+A_*)^p e^{C(F_0+A_*)}
       \epsilon_k^{1/18}.
 \tag{FC.19}
\]
The unchanged branch has factor one. The new native-map
branch has the actual guard. The direct prefix uses
(FC.15) and a consumed mark. A complete R step uses
the literal self kernel in the selected representation;
successful masses pay restored interiors, and retained
completed components have their actual new raw multipliers.

The AF envelope (FC.1) makes every fixed positive fractional
power of (FC.16) summable uniformly in depth. Indeed
\[
 \int_T^\infty t^u(1+\log t)^v
                   e^{-c(\log t)^r}\,dt\longrightarrow0
 \quad(T\longrightarrow\infty),
 \tag{FC.20}
\]
because \(r>1\). At the original bare Wilson start there is no
completed relative family, so \(A^{[0]}=0\). If the proof is
started at an intermediate scale, its initial capacity is the
one already obtained by the same induction through the earlier
steps, not an additional assumed C05 estimate. Choose \(A_*\)
strictly above that proved initial capacity, then one ceiling
such that
\[
 e^{C\sum_k\sigma_k}
       \left(A^{[0]}+\sum_k f_k(F_0,A_*)\right)<A_*.
 \tag{FC.21}
\]
This proves the uniform repeated-history positive norm.
No step assumes C05, an arbitrary marked-kernel bound,
or a sum of separately normed canceled pieces.

## 7. Native and current readout of the closed norm

The native-root argument of
[Summation at a native root on a two-sided trajectory](native_roots.md) now
applies to the atoms in (FC.8). The actual root/port
estimate pays the fine density before summing ages.
The sole possible prefix top-band loss and the Gaussian
\(P_n^2\) value factor are fixed logarithmic polynomials.
The first \(+\) enlargement pays them in Cauchy's formula
while the derivative is measured in the original
\(-\) norm. The positive sum is taken on one common
contour. This proves (FC.5), including every
current-independent native scalar. ND §§6–7 record
the independent-current, preparation and four-output
checks.

For current derivatives, apply the verified actual
reconstruction row, with its physical field, gradient,
curvature and current weights. Combining the true port
and its paid carrier gives an age rate
\(\Gamma>4\log L+\log2+2\), which pays the actual
four-dimensional root density. The source current
input is \(g_kz\); the resulting normalized first-leg
factor is \(\theta_k=\ell_k^{p_0-q}\).

The complete sufficient current budget is the sector
budget (CE19) of [Current endpoint estimates for boundary activities](../current_endpoints.md):
\[
\begin{split}
K_{B,k}\le C\bigl[&
\mathfrak K_E+C_Rg_k^{\kappa_0-11}
 +(B_0+C_0)\theta_k+g_k^{-2}D_k^3+D_k\\
&+g_k^{-2}\delta_k(1+\log\ell_k)^{A_\phi}e^{-c_\phi R_k}\\
&+\theta_kP_k^2(1+\ell_k)^{A_G}e^{-c_GR_k}
 +\theta_k(A_*+\mathcal F_*)\bigr],
\end{split}
\tag{FC.22}
\]
where \(\kappa_0\ge12\),
\(D_k\le Cg_k\ell_k^{q+Q_1}\) and
\(\delta_k=Cg_kP_k\). The terms are, respectively,
the boundary-assigned regular activities, ordinary
boundary and prefix terms, constrained classical
remainder, Haar/coarea terms, heterogeneous Wilson
response, old Gaussian/Schur response, and fresh and
failed-preparation families.

The exact retained exterior force stays in its C01
Gaussian position. The complete exterior Jacobian
also remains in the native bookkeeping. No sector has
been removed by subtracting \(B_k(0,\xi)\).

Every term in (FC.22) is bounded at the common ceiling.
After division by \(P_k^2\), each tends to zero.
The only inverse-coupling terms retain
\(e^{-c\ell_k^r}\), which dominates every fixed power
of \(g_k^{-1}\) and \(\ell_k\). Hence (FC.3) follows.

For order \(m\), common current Cauchy contributes
\((m-1)!\); the four-dimensional endpoint sum uses
one connector/diameter moment of order \(4(m-1)\)
and contributes at most \(C^m((m-1)!)^4\).
PC.6a has retained the required physical diameter
reserve for the coarsened atom. This proves (FC.4)
with one fixed factorial power five. One fixed
reduction of the spatial rate gives the stated
Hessian rate as well.

These arguments prove every clause of Theorem FC.1.
\(\square\)

## 8. What the theorem means

The C05 estimate requires the common-localizer/common-Gaussian
passage for the canceled positive-norm blocks. The
proof supplies that passage, identifies the norm
on the complete atoms, and applies the chronological
closure to that norm.

It also uses the exact operative componentwise source geometry
and its explicit proper-mesh count for the preparation size. It neither adds
a new history restriction nor changes a source
eligibility clock.

The resulting conclusion is the original C05 boundary
estimate. C06 and C08 may use it on their stated
conditional-law classes. Physical observable
normalization, complete source/history induction,
continuum identification and the remaining existence
requirements remain separate problems. They are not
additional conditions concealed inside FC.1.

## References and proof dependencies

- Statement and its source interpretation: [Operative source domains and the ancestral dimension bound](operative_source_scope.md),
  especially Lemma [CT.1](operative_source_scope.md) and Section 9.
- Exact localization and positive transfer: [Coarsened protected atoms and the positive catalog](positive_catalog_coarsening.md),
  PC.1–PC.6, including PC.6a.
- Proper-mesh phase and Gaussian compatibility: [Proper-mesh coordinate counts, common positive domination and native jets](native_domain_count.md),
  ND.1–ND.55.
- Main derivations: [Current endpoint estimates for boundary activities](../current_endpoints.md),
  [Summation at a native root on a two-sided trajectory](native_roots.md),
  [Positive attachment bounds and the quotient forest](quotient_forests.md) (Q) and
  [Majorants for marked atoms and composition of prefixes](marked_atoms.md).
- Primary sources: Bałaban, CMP 119 (1988) pp.258–262, 265–278; CMP 116 (1988) pp.3–7 and 12–17;
  *Large field renormalization* I and II, CMP 122 (1989), LFR I pp.177–180, 188–192 and 195;
  LFR II pp.369–380 and 391–392.
