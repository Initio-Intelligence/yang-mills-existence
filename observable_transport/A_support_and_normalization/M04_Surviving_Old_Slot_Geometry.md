# Surviving old Gaussian slots in the actual regular step

This note concerns the regular conditional Q step, not the old-state
posterior of an R replacement. It identifies the geometric suppression
available for a genuinely surviving ordinary old Gaussian slot after
the determining sequence has been updated. It also separates this
statement from the unresolved full-component normalized response.

## 1. What is actually retained by the regular Q step

The C-01/RC18 regular conditional law integrates the current free
coordinates in Λ_{k+1}. The other free coordinates of that same current
chart, the old raw variables, the surviving older fluctuation variables,
and the appropriate geometry/selector data are retained parameters.
Older fluctuations are not appended to the current exterior vector y.
They occur as parameters of the complete perturbation.

Consequently an old Gaussian density cannot be specified simply because
its integration variable is retained. If its precision depends on the
new background, its exact contribution is the logarithm of the ratio
at that background to the ratio at zero current, as stated in the C-01
identification (Annex AX) and Annex AS. At the same time, a regular Q step does not
integrate that surviving old variable by an old reset posterior. Its
pointwise cutoff and any incoming marked dependence remain part of
the regular calculation.

The actual ordinary operation is CMP119 (2.20)–(2.21). Its independent
old fluctuation A_j is supported on

\[
 F_j=(Z_{j+1}\cap\Omega_{j+1})^{(j)}
     =(\Omega_{j+1}\setminus\Lambda_{j+1})^{(j)}.
                                                               \tag{OS.1}
\]

The interlacing in (2.1) therefore puts it outside Ω_{j+2}. The same
page, printed p.258 after (2.21), explicitly says that an R-modified
ordinary operation has the same general form, with changed
characteristic functions and a possibly empty domain. These are the
actual updated sequences of the induction, not historical sets which
have been retained after their variables were removed.

## 2. Erasure and rebasing are visible in the source

For a completed prepared component Z, LFR II (1.33)–(1.35), printed
p.365, gives the new determining set explicitly:

\[
 \Gamma_j^{\rm new}=\Gamma_j'\cap Z^c\quad(j<k),
 \qquad
 \Gamma_k^{\rm new}=\Gamma_k''\cup Z^{(k)},            \tag{OS.2}
\]

with the new current V_k inserted on Z. Thus the old determining
coordinates inside the replaced component are removed. Its primitive
old integration is performed as part of the R operation; those erased
continuous variables do not remain ordinary slots of the next Q
operation merely because a retained history label remembers them.

The alternative completed representation LFR II (1.103)–(1.104)
integrates the whole incoming boundary exponential with the normalized
component operations. Printed p.392 then says that the remaining
T′_k(Y)1 functions depend only on the new V_k restricted to Y and do
not participate in the next renormalization transformations. These
multiplication factors are distinct from a surviving ordinary Gaussian
slot. Their scalar boundary responses have been moved into the
completed boundary activities and require their own analysis.

Outside a component modified by R, its old variables are unchanged.
After partial preparation the retained sequence is again explicitly
admissible; LFR I (1.10)–(1.12) describes the new domains. The last
N₀ constructed annuli can have only one M-layer of separation. It is
therefore unsafe to assign every later annulus its old MR_l width.

## 3. An actual annular-distance bound

Let h_l be the physical spacing at level l. The mixed distance used
by the propagator/minimum estimates is, up to the fixed source
equivalent convention,

\[
 d_\Omega(x,y)=\inf_\gamma
   \sum_l h_l^{-1}
       |\gamma\cap(\Omega_l\setminus\Omega_{l+1})|.
                                                               \tag{OS.3}
\]

This is CMP96 printed p.231, (2.46), with the source graded block
notation suppressed. CMP102 (1) requires a fixed sufficiently large
native separation between successive admissible determining domains.
In the present source construction it can be taken as cM. The
preparation construction retains at least its stated one M-layer.

### Lemma OS.1

Fix an actual surviving ordinary old slot r in (OS.1), and a new
current free direction i in Ω_{k+1}. In the updated source geometry,

\[
 d_\Omega(r,i)
 \ge c_0M(k-j-c_1)_+ + c_2MR_k-c_3,                  \tag{OS.4}
\]

with fixed constants, whenever the source R_k and R_{k+1} are
identified by their bounded one-step comparison. Fixed averaging
footprints change only c₁,c₃ and fixed scale factors.

**Proof.** By the literal interlacing, r lies outside Ω_{j+2}.
The point i lies inside Ω_{k+1} and therefore inside every intervening
Ω_l. For each l from j+2 through k−1, a continuous path from r to i
must cross the separating annulus Ω_l\Ω_{l+1}. The native separation
between its two boundaries is at least cM h_l. The last entrance
into Ω_l before the first entrance into Ω_{l+1} contains a segment
of this length inside that annulus. The segments for different l
occupy disjoint graded layers. Their contributions to (OS.3) sum
to at least cM per layer. Reentries or other connected components
cannot reduce this lower bound.

The current RG construction, CMP119 (3.2)–(3.5), builds Ω_{k+1}
away from a buffered cover of the actual current Z_k. The old slot
belongs to Z_k by physical nesting. The new regular domain lies
beyond the stated large MR_{k+1} collar. In the current coarsest
part of (OS.3) this contributes a fixed multiple of MR_k. Reserve
this top collar separately from the preceding layers. Interface
and averaging stencils have fixed relative width and remove at
most fixed amounts from these estimates. This proves (OS.4). ∎

The proof uses the current actual sequence at every step. It does
not assign an old birth label to a newly formed domain and claim
that its former collars survived. If a slot has been erased by
(OS.2), it is absent from the sum. If it survives, its position in
(OS.1) and the actual admissibility force the crossings in the proof.

The stronger lower bound c Σ_l MR_l is available only through
layers which really retain those wider collars. Partial preparation
does not justify it uniformly. The weaker fixed-large-M age bound
is already sufficient for the usual fine-position entropy.

## 4. What the age factor pays

Write n=k−j. A conservative count of old j-grid positions per
current cell is C L^{4n}, with fixed polynomial factors for the
source carriers and cutoffs. The admitted coupling comparison gives

\[
 P_j^a\le C_a P_k^a(1+n)^{b_a},                       \tag{OS.5}
\]

for each fixed exponent a. If a coefficient has a fixed power of
g_j^{-1}, the same comparison gives a fixed current g_k^{-1}
power times another fixed polynomial in 1+n.

Hence for any fixed a,b and fixed decay exponent μ>0,

\[
 \begin{aligned}
 &\sum_{j<k}L^{4(k-j)}(1+k-j)^b P_j^a
          e^{-\mu c_0M(k-j-c_1)_+}
          e^{-\mu c_2MR_k}\\
 &\hspace{2em}\le C_{a,b,M}P_k^a e^{-\mu c_2MR_k},     \tag{OS.6}
 \end{aligned}
\]

after the fixed admissible M is chosen so that μc₀M>4 log L
with a positive reserve. The remaining g_k^{-B} times fixed
polylogarithms are absorbed by the current e^{-cMR_k} collar
because the specified regime has R_k≥(log g_k^{-2})^r with r>1.
No M depending on the age, derivative order, or cutoff depth is
chosen.

Equation (OS.6) pays old rank by actual coefficient localization.
It is not a pointwise bound on the total number of old variables
inside a surviving component. That number may still be arbitrarily
large.

## 5. The precise coefficient-level input

For an ordinary source precision K_j=C_j*Δ^(j)C_j, the actual
retained Schur form is

\[
 S_j=K_{RR}-K_{RI}K_{II}^{-1}K_{IR}.                  \tag{OS.7}
\]

Its derivative includes the derivative of K_{II}^{-1}; support of
the retained a_j does not make it constant. On a fixed native chart
the exact scalar response is

\[
 -\tfrac12 a_j^{\mathsf T}
       [S_j(\Phi(A))-S_j(\Phi(0))]a_j.               \tag{OS.8}
\]

CMP99 Theorems 3.9, 3.10 and 3.15, used in Annex AS/OR17.9,
provide local-background walk/tree expansions for the actual
operators and principal restriction. A proof applying (OS.4) must
keep the full localized coefficient carrier, including its two
old endpoints. If the current native response is attached at a
different point of that carrier, the source tree path from that
attachment to an old endpoint is used together with the minimum's
current-response path. Their combined paid length must dominate
the distance in (OS.4). Off-diagonal decay of a matrix entry alone
does not prove this local-background statement.

With that genuine source connector, the geometric and age part of
the ordinary Gaussian response estimate is justified by (OS.4)–
(OS.6). The pointwise field factor is P_j², from the actual ordinary
cutoff; it is not an uncontrolled old posterior moment. Continuous
current derivatives are taken on the same source contour with all
coefficient and constraint responses included.

For a full M-03 assertion, one must additionally retain the actual
raw dependency footprints and all discrete geometry differences.
An uncontracted source walk/tree can be resolved into local raw
geometry membership tests on its carrier. A global history flag
does not acquire a small footprint merely by this observation.
The ambient extension and all rectangular two-copy paths must
still be specified as in Annex Y.

## 6. What is not paid by this lemma

This result does not assign a new internal-tree cost to a completed
normalized component in LFR II (1.103). Printed p.391 explicitly
omits those costs because the component domains are fixed. Its
outer multiplication mass is retained by the next Q step, but the
scalar boundary interaction created by its normalized integral can
still respond to current data. Such an interaction is a different
object from the two-endpoint unintegrated Gaussian primitive
(OS.8).

Likewise, an incoming transported scalar mark may already depend
on retained old coordinates. Its actual M-03 carrier/energy budget
can be used as an incoming budget in M-04. One cannot infer that
budget by substituting a fresh scalar, and one cannot charge a new
kernel dependence on a previously absent component solely to the
incoming mark. The normalized kernel response needs its own
absolute supported estimate.

The present note therefore resolves the geometric old-age question
for surviving ordinary slots and states exactly which source
coefficient localization is needed with it. It does not complete
C-05/C-08 for completed normalized components or the full M-04
scalar extraction/current theorem.
