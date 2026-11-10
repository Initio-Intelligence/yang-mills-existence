# A raw-local regular reference across one actual mixed-scale interface

This note extends the homogeneous bundle reference to a determining set containing two adjacent scales. It makes the boundary-bond convention explicit. The construction preserves all prescribed lower-grid links in an auxiliary cochain, admits arbitrary weak-curvature gauges, and has constants independent of the absolute fine depth. It is not an iteration over the number of scales.

## 1. The source geometry and the two kinds of coarse plaquettes

Let the lower determining mesh be `ℓ=L^jη` and the upper mesh `Lℓ`, with L fixed. Let D be the set of upper-grid centers in the upper-scale domain, and let `B(D)` be its union of L-blocks on the lower grid. Assume the source block alignment and a fixed local halo. In particular a block belongs wholly to D or wholly to its complement.

The convention matters: CMP96 p.224, (2.3), defines the determining shells separately for **site sets and bond sets**, after defining a domain's bond set by at least one endpoint in that domain. Consequently subtracting the upper domain's bond set leaves lower determining bonds with **both endpoints outside `B(D)`**. A lower-grid bond touching `B(D)` is free in this auxiliary extension. It is not a specified lower determining entry. Upper determining bonds are those with at least one endpoint in D.

Write `v` for the given lower-grid field on those outside bonds, and `V` for the given upper determining bonds. The admitted data satisfy:

- The given lower plaquettes have holonomy defect at most ε.
- Every upper plaquette touching D satisfies the literal mixed condition CMP102 (7): use V on its prescribed upper bonds, and use the **one-step nonlinear average** `Μ(v)` on a missing outer bond. That average is available because both endpoint L-blocks of the missing bond lie outside `B(D)`.

Define a full upper-grid field

\[
 \widetilde V_c=
 \begin{cases}
 V_c,&c\hbox{ has an endpoint in }D,\\
 \mathcal M(v)_c,&c\hbox{ has both endpoints outside }D.
 \end{cases}
 \tag{MI.1}
\]

For a plaquette touching D, its holonomy in `Ṽ` is **exactly** the expression in source condition (7). For a plaquette entirely outside D, it is a plaquette of `Μ(v)`, and CMP98 Proposition 1 bounds it by `C_Lε`. Thus

\[
 \sup_p\|\widetilde V(\partial p)-I\|\le C_L\varepsilon.
 \tag{MI.2}
\]

This argument does not replace the average by a straight path in the mixed condition. The average is retained exactly in (MI.1); the comparison to a straight path is used only in the next estimate.

## 2. A local center-fixed gauge on the lower blocks

On each outside L-block choose the fixed ordinary block axial tree, rooted at its upper-grid center. Let τ be the product of the given lower links along that tree, with orientation chosen to set the tree links of `v^τ` to I. It has value I at the root. Set τ=I in the upper-domain blocks. This defines a block-local gauge on all lower vertices; it is allowed to jump at a block boundary. Every upper-grid center is fixed, so

\[
 \mathcal M(v^\tau)=\mathcal M(v),\qquad
 \widetilde V\hbox{ is unchanged at its endpoints}.
 \tag{MI.3}
\]

No gauge has been applied to the actual prescribed data permanently: it is a device in the definition, and is undone below.

Inside an outside block, a non-tree lower bond closes a loop with the two tree paths. The loop is filled by at most `C_L` lower plaquettes. Hence its gauged value is `I+O(C_Lε)`.

For a bond crossing between two outside L-blocks, compare it to the central straight transport between their centers. The connecting tree paths and this comparison form a loop in the union of those two outside blocks, filled by `C_L` lower plaquettes. The central path transport and the literal one-step average differ by `C_Lε`, directly from the averaging definition CMP98 (42). The source step lift `Q^f` is I on internal bonds and the coarse matrix on each corresponding face-crossing bond. Therefore, on every prescribed lower bond,

\[
 \|v^\tau_b-(Q^f\widetilde V)_b\|\le C_L\varepsilon.
 \tag{MI.4}
\]

All loop fillings used here stay in the lower determining data. No path enters an upper-domain block whose lower links have not been given.

## 3. The full lower-grid auxiliary cochain

In the τ gauge define

\[
 W^\tau_b=
 \begin{cases}
 v^\tau_b,&b\hbox{ is a prescribed lower bond},\\
 (Q^f\widetilde V)_b,&b\hbox{ touches }B(D).
 \end{cases}
 \qquad W=(W^\tau)^{\tau^{-1}}.
 \tag{MI.5}
\]

This is an exact prescription of every lower-grid bond. By (MI.4) it differs from `Q^f Ṽ` by `C_Lε` in that gauge, even at an interface plaquette. The step lift itself has plaquette holonomies equal either to I or to transported upper plaquette holonomies. A product of four unitary matrices changes by at most the sum of their changes. Thus

\[
 \sup_p\|W(\partial p)-I\|\le C_L\varepsilon,
 \qquad W_b=v_b\quad\hbox{on every prescribed lower bond}.
 \tag{MI.6}
\]

The equality on the right holds after undoing τ and is exact. We did not change a lower determining link to obtain the bound.

The cochain W is a local analytic function of the actual data. Its construction uses only the fixed block trees, one-step averaging stencils, the upper step lift and products/inverses. The logarithms in the one-step average are in the uniform small-loop branch because the lower curvature is small. Its footprint is a fixed number of upper-scale blocks, independent of j and volume.

The exact identity `Μ(Q^f Ṽ)=Ṽ`, the uniform finite-step analyticity of the averaging map, and (MI.4) give

\[
 \|\mathcal M(W)_c-V_c\|\le C_L\varepsilon
 \quad\hbox{on prescribed upper bonds}.
 \tag{MI.7}
\]

The comparison may be made in the τ gauge: all upper endpoints are fixed. Since the difference in (MI.4) is small relative to the compact step lift and all stencils have fixed size, the averaging logarithms remain in their admitted local branches.

## 4. Apply the bundle construction at the lower mesh

Apply Theorem BR.1 of [local bundle reference](local_bundle_reference.md) to W on the uniform lower mesh ℓ, using microscopic mesh η. Denote the resulting field by Uref. It has straight ℓ-edge holonomies exactly W and obeys

\[
 \|U_{\rm ref}(\partial p)-I\|
       \le C_L\varepsilon(\eta/\ell)^2,
 \qquad
 \|D^*\partial U_{\rm ref}\|
       \le C_L\varepsilon\eta^3\ell^{-3}.
 \tag{MI.8}
\]

On the upper region, these imply the required `Lℓ`-scale bounds with the additional fixed factors `L²` and `L³`. Those are fixed source constants, not powers of the absolute depth j. Thus Uref is in the mixed regularity class of CMP102 (14), with a fixed `C_1=C(L)`.

The literal lower-depth average satisfies

\[
 \|\mathcal M^j(U_{\rm ref})-W\|\le C_L\varepsilon
 \tag{MI.9}
\]

by BR.3 after rescaling. On the prescribed lower bonds W=v exactly. On the upper bonds, apply one further finite-step average to (MI.9), and use (MI.7). This gives

\[
 \|\mathcal M^{j+1}(U_{\rm ref})_c-V_c\|
      \le C_L\varepsilon.
 \tag{MI.10}
\]

All references and discrepancies have true local raw footprints. Their complex source-domain admission follows from the BR local bundle identification and the finite block gauge/averaging maps in (MI.1)–(MI.5). At a fixed pair of scales their constants are uniform in j. The actual force-containing mixed variational equation can therefore start from this reference; neither W nor Uref has been declared a critical field.

### Theorem MI.1

For the actual two-adjacent-level determining geometry above, admitted by CMP102 (7), there is a raw-local regular approximate reference satisfying CMP102 (14), uniformly in the absolute depth and volume. It preserves all lower determining bonds in its auxiliary lower cochain, gives the prescribed lower and upper averages within `C_Lε`, and has the corresponding source regularity constants. No global weak-link gauge is used.

This theorem includes unions of upper blocks and their corners; it is not limited to a planar interface. The source geometry's fixed local halos are included throughout. An interface meeting a separate third scale requires the further graded argument, rather than applying this theorem outside its domain.

## 5. Fine specified data and the limit of the present theorem

If `j=0`, the lower mesh is the microscopic mesh η. There is no subsequent smoothing depth: Uref can be taken to be W itself. Its values on all prescribed fine bonds are exactly the original v. In this case arbitrary strong fields far outside the regular region can simply be copied. Only the outside block collar actually used to estimate interface plaquettes needs the weak-curvature bounds; one does not claim regularity in the distant specified core.

The same observation explains how a future graded projection must handle a specified `Γ_0`: it may use the regular buffered collar and must copy the arbitrary exterior fine values exactly. It must not apply a small-plaquette projection to their unrestricted interior. The first source construction supplies such a geometric separation in CMP119 (1.10): the regular domain is at least two `LMR_1` layers from the large-field set. Using that buffer for a particular later determining history still requires its actual inherited geometry and selectors.

For `j>0`, the present theorem assumes that the lower data used in the construction are the admitted weak-curvature determining data. It does not invent lower coarse averages inside an arbitrary specified fine core.

## 6. Why naive iteration is not yet a many-level theorem

Applying (MI.1)–(MI.10) repeatedly would multiply its fixed `C_L` losses. No depth-uniform bound follows from that iteration. A different global graded construction must ensure that each local patch sees only one adjacent-scale interface and pays the interface comparison once. The source separation of consecutive domains suggests such a construction, but its graph, local loop comparisons, partition and exact specified-edge treatment must be supplied explicitly.

The local result above is the useful input for that approach: on an actual adjacent-scale patch it provides a uniformly weak auxiliary cochain agreeing with every lower determining edge, while every upper determining edge differs from its auxiliary straight transport by at most `C_Lε`. It therefore controls the bounded mixed loops needed for a single graded projection, without multiplying constants down the scale hierarchy.

## Mathematical sources

- CMP96 (1984), p.224, (2.1)–(2.4): site/bond shell convention and scale-separated block geometry.
- CMP102 (1985), pp.277–280, (1), (7), (11), (14): actual mixed plaquette convention and regular approximate reference; the distinction between upper mixed plaquettes and pure lower averaged plaquettes is on p.278.
- CMP98 (1985), (42) and Proposition 1: the exact one-step average, its curvature bound and its local small-loop comparison.
- CMP119 (1988), (1.3), (1.10): the step lift and the first regular-domain collar.
- [local bundle reference](local_bundle_reference.md): the homogeneous local projection, exact edge holonomies, fine regularity and uniform literal-average comparison.
