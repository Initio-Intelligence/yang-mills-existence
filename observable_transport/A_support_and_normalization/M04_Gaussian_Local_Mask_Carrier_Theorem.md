# A full physical-carrier theorem for the flat Gaussian step with local masks

## Status and precise scope

This note proves a uniform value and current theorem for the exact
untruncated flat Gaussian conditional with arbitrary local integration
masks. Its carrier weight charges physical volume and tree length.
It therefore proves more than exponential decay in the distance from
one varied mask.

The mask is an independent primitive coordinate of the amended ambient
state, as specified in M04_Local_Mask_Interface.md. The actual retained
fluctuation slots are padded by zero when integrated. All padded slots
are included in the ambient native regulator. These are explicit
interface choices, not a new locality identity for the source-derived
domains of the specified M03 definition.

The theorem applies to the Gaussian part of the first ordinary source
step at full determining domain and flat coarse field: its common
constraint embedding C is retained in the scalar quadratic form.
It does not remove the actual broad product cutoff, establish a
complete non-Gaussian source expansion, vary the determining geometry,
or prove the old completed boundary activity estimates. Those remain
separate statements.

## 1. Common padded physical kernels

Let G be a finite periodic block graph of fixed dimension d and uniformly
bounded polynomial growth. At each site i let x_i have dimension at most
d_*. Let K be the common real symmetric precision, with
\[
 \lambda I\le K\le\Lambda I,\qquad
 K_{ij}=0\quad\hbox{if }d(i,j)>r_0.
 \tag{GMK.1}
\]
All constants here are independent of the torus and the chosen mask.
The grouping into current physical blocks can include the fixed number
of fine independent coordinates per L block.

Let m_i be either zero or one, with one meaning integrated. Write
\[
 D_m=\operatorname{diag}(m_iI_i),\qquad E_m=I-D_m.
 \tag{GMK.2}
\]
The retained array is a=(a_i). On the actual padded support, a_i=0
whenever m_i=1. In the ambient product it is an arbitrary real array.
Use the full padded regulator
\[
 R_X(a,m)=1+\sum_{i\in X}|a_i|^2.
 \tag{GMK.3}
\]
It is deliberately not multiplied by E_m off support. On actual
states (GMK.3) is exactly one plus the retained native free energy.
It contains no sampled eliminated microscopic energy.

Put T=I-K/\Lambda and q=1-\lambda/\Lambda. If q=0 the following
inverse is already local. Otherwise 0<q<1. Define
\[
 T_m=D_mTD_m,\qquad
 K_m=\Lambda(I-T_m),\qquad R_m=K_m^{-1},
 \tag{GMK.4}
\]
\[
 C_m=D_mR_mD_m,\qquad
 \bar x_m=E_ma-C_mKE_ma.
 \tag{GMK.5}
\]
For every mask, \(0\le T_m\le qI\) and \(K_m\ge\lambda I\).
Its active block is K_II and its inactive block is \(\Lambda I\);
there are no cross blocks. Hence C_m is K_II^{-1} on the
integrated set and zero on its complement.

Define the physical kernel
\[
 \mathsf q_{m,a}=\mathcal N(\bar x_m,C_m)
 \tag{GMK.6}
\]
as a possibly degenerate Gaussian probability on the full old
coordinate space. Inactive physical coordinates are exactly a_i;
their fluctuation variance is zero. This is precisely the Gaussian
conditional obtained by integrating the active coordinates and
retaining the others.

The artificial inactive block \(\Lambda I\) in K_m is only an
inverse-calculation device. An inactive dummy Gaussian is never
inserted into the physical kernel or exposed to a cross-copy mark.
Both D_m factors in C_m are essential.

## 2. A local resummation which gives absolute physical carriers

A spectral Neumann series by itself is not an absolute carrier
expansion. We first group a fixed number of its powers into genuine
local coefficient functions.

Choose n_0 large enough that
\[
 D_{n_0}q^{n_0}\le\tfrac18,
 \tag{GMK.7}
\]
where D_n bounds the number of block sites within distance nr_0.
Polynomial growth makes this possible. Set
\[
 U_m=T_m^{n_0},\qquad
 H_m=\sum_{r=0}^{n_0-1}T_m^r.
 \tag{GMK.8}
\]
For each matrix entry (i,j), the coefficient \((U_m)_{ij}\) depends
only on mask variables in the connected ball B(i,n_0r_0); it is zero
outside that range and obeys
\[
 \sup_m\|(U_m)_{ij}\|\le q^{n_0}.
 \tag{GMK.9}
\]
The same assertions with the obvious finite bound hold for H_m.
We keep each already defined local entry as one coefficient. This is
a finite local resummation; it is not a claim that the sum of the
absolute values of its individual short walks is small.

For a tagged matrix carrier family A_X(i,j), whose carrier contains
both endpoints and every mask it uses, let its absolute norm be the
maximum of the weighted row and column sums, with
\[
 w_\kappa(X)=e^{\kappa(|X|+\mathsf t(X))}.
 \tag{GMK.10}
\]
All balls used in (GMK.9) have volume at most a fixed V_0. Choose a
fixed \(\kappa_0>0\) so small that their weight is at most two.
Equations (GMK.7)--(GMK.9) then give
\[
 \|U\|_{\kappa_0}\le\tfrac14,\qquad
 \|H\|_{\kappa_0}\le C.
 \tag{GMK.11}
\]
Column sums have the same bound: for a fixed j, only D_{n_0}
possible i contribute. The declared carrier need not be centered at
j for this counting argument.

Matrix multiplication joins carriers at the contracted endpoint.
Their union is connected and its weight is no greater than the
product of their weights. This absolute coefficient algebra is
therefore submultiplicative.

### Theorem GMK.1: uniform inverse and mask-current carriers

For every binary mask,
\[
 R_m=\Lambda^{-1}H_m\sum_{s\ge0}U_m^s
 \tag{GMK.12}
\]
is an exact absolutely convergent physical-carrier representation,
uniformly in the mask and volume. Its weighted row and column norm
is at most a fixed C.

The same representation has a uniformly bounded sum of its finite
differences over all elementary mask flips, with each difference
carrying the full original coefficient carrier.

**Proof.** The identity
\((I-T_m)H_m=I-U_m\) and (GMK.11) prove (GMK.12) and the value
bound. Each primitive coefficient of H or U uses at most V_0
binary variables. Its sum of mask differences is therefore finite
and uniformly bounded before any long series is taken.

For a product use the exact telescoping identity
\[
 \delta_b(AB)=(\delta_bA)B(m^b)+A(m)\delta_bB.
 \tag{GMK.13}
\]
The supremum bounds on both endpoint masks are the same. Summing
over b and all tags gives the usual product rule for the absolute
current norm. The differentiated geometric series is bounded by
\[
 \sum_{s\ge1}s\|U\|_{\kappa_0}^{s-1}\le(1-\|U\|_{\kappa_0})^{-2}.
 \tag{GMK.14}
\]
Thus the total current norm of (GMK.12) is bounded by
\[
 C\left[
 \frac{\|DH\|_{\kappa_0}}{1-\|U\|_{\kappa_0}}
 +\frac{\|H\|_{\kappa_0}\|DU\|_{\kappa_0}}
 {(1-\|U\|_{\kappa_0})^2}\right].
 \tag{GMK.15}
\]
Here D means the sum of actual binary finite differences, not a
derivative on a fictitious fixed-rank manifold. Every term has
genuine local mask support. All constants involve fixed n_0 and
V_0, never the torus volume or a source R scale. This proves the
theorem. ∎

Multiplication by the local D_m, E_m and finite-range K preserves
these conclusions. In particular C_m and
\[
 P_m=E_m-C_mKE_m
 \tag{GMK.16}
\]
have absolute physical-carrier and mask-current expansions with
uniform two-sided coefficient norms. The mean is \(\bar x_m=P_ma\).

## 3. Exact quadratic transport and its supported representation

Let a physical incoming mark, supported in a connected set S containing
its anchor, be
\[
 F_h(x)=h^{-4}\{c+\ell^Tx+x^TAx\}.
 \tag{GMK.17}
\]
Only entries with indices in S occur. Put
\[
 b_F=|c|+\sum_i|\ell_i|+\sum_{i,j}\|A_{ij}\|.
 \tag{GMK.18}
\]
This is an explicit input coefficient budget. It is specified before
the Gaussian integration and does not contain its output norm.
The exact conditional expectation is
\[
 QF_h(m,a)=h^{-4}
 \{c+\ell^TP_ma+a^TP_m^TAP_ma+\operatorname{Tr}(AC_m)\}.
 \tag{GMK.19}
\]

Substitute the carrier representations of P_m and C_m. Each trace
path starts at S, each linear mean path is attached to S, and the two
paths in the quadratic mean term meet the fixed root carrier S.
Thus every tagged coefficient has a connected physical carrier Y
containing S and its actual retained endpoints.

For a scalar coefficient with absolute magnitude t_Y, the associated
monomial is bounded by
\[
 |a_i|\le 1+|a_i|^2,\qquad
 |a_i^TMa_j|\le \tfrac12\|M\|(|a_i|^2+|a_j|^2).
 \tag{GMK.20}
\]
Consequently its value is at most
\[
 h^{-4}C t_YR_Y(a,m).
 \tag{GMK.21}
\]
Absolute matrix multiplication gives
\[
 \sum_Yw_{\kappa_0}(Y)t_Y
 \le Cb_Fw_{\kappa_0}(S).
 \tag{GMK.22}
\]
The trace term includes its actual local rank through the coefficient
sum (GMK.18). No volume-independent trace estimate is applied to an
extensive identity matrix.

## 4. All local mask and retained-coordinate currents

We use the physical-kernel option expressly allowed after (M.28c)
in Annex Y: push the conditional law to the full old
coordinate state and keep the original mark independent of retained
y=(m,a). For the bare quadratic mark, all newly generated responses
are then in
\[
 J_\tau(m,a)=
 \int F_h(x)\,
 \frac{\mathsf q_{\tau(m,a)}-\mathsf q_{m,a}}{t}(dx),
 \tag{GMK.23}
\]
with denominator one for a mask flip. The new direct record is zero
in this filing. No pre-existing direct/current record is relabeled:
this theorem concerns the specified primitive mark; carrying an old
decorated input requires carrying its existing records separately.

The kernels in (GMK.23) can be mutually singular. We do not bound
their total variation divided by t. Formula (GMK.19) computes their
action on the actual quadratic mark exactly.

For mask flips use Theorem GMK.1 and (GMK.13) on each tagged
coefficient in (GMK.19). The retained a array is held fixed. Its
monomials are still of degree at most two and obey (GMK.20).
The sum of all mask currents therefore has the same energy degree
as the value.

For a retained increment a_i→a_i+te, |t|≤1, use the exact difference
of each linear or quadratic monomial. Division by t gives a linear
term and, for the quadratic diagonal term, a bounded multiple of t.
Only the finitely many endpoints of that tagged monomial contribute.
Summing all basis directions costs the fixed block dimension.

The shifted value envelope and the summed continuous/discrete current
envelope of each tag consequently obey
\[
 A_Y^\sharp\le Ch^{-4}t_Y\widehat R_Y,\qquad
 J_Y^\natural\le Ch^{-4}j_Y\widehat R_Y,
 \tag{GMK.24}
\]
\[
 \sum_Yw_{\kappa_0}(Y)(t_Y+j_Y)
 \le Cb_Fw_{\kappa_0}(S).
 \tag{GMK.25}
\]
The current in (GMK.24) is stronger than the pointwise grade-3/2
bound required in M03, since \(\widehat R_Y\ge1\). Compatibility
\(\delta A_Y=J_Y\) is exact tag by tag; the same tag is retained
through its coefficient differences.

The full padded energy convention matters here. If the ambient
regulator ignored a_i whenever m_i=1, many off-support nonzero
ignored a_i could be exposed in the sum over mask flips while one
shift in the regulator sees only a maximum. Equation (GMK.3)
prevents this omission and agrees with the native energy on
physical padded states.

## 5. The complete M03-form estimate under an actual outer reserve

Suppose the outgoing law, whatever correlations it has with the masks,
obeys the genuine native moment hypothesis
\[
 \|a_i\|_{L^{2p}(\mu_{\rm out})}\le C_0\sqrt p,
 \qquad i\in G,\quad p\ge1.
 \tag{GMK.26}
\]
No conditional moment bound on an individually rare mask is substituted
for this actual outgoing-law assertion.

Minkowski gives
\[
 \|\widehat R_Y\|_{L^p(\mu_{\rm out})}
 \le C(1+|Y|)p.
 \tag{GMK.27}
\]
The possible one-coordinate shift is bounded directly by the same
full padded energy and a fixed additive constant. The masks themselves
do not change (GMK.3).

Choose any fixed \(0<\kappa<\kappa_0\). The extra factor \(1+|Y|\)
in (GMK.27) is paid by the spare physical carrier weight.
Combining (GMK.24)--(GMK.27), with output spacing h'=Lh, proves
\[
 \boxed{
 \|\mathbf QF_h\|^{\rm local\ mask}_{Lh,\kappa}
 \le C(L,\lambda,\Lambda,r_0,d_*,C_0,\kappa_0-\kappa)
 b_Fw_{\kappa_0}(S).
 }
 \tag{GMK.28}
\]
The explicit physical factor in the proof is \((h'/h)^4=L^4\).
The norm has the M03 value grade one and current grade three-halves,
the full ambient supremum, the sum of all local mask flips and
retained-coordinate divided differences, and the actual outer
moment terms.

Without (GMK.26), the pointwise part of the theorem remains proved;
the averaged assertion is not inferred from a polynomial regulator
alone.

### Corollary: the same theorem with a saturated retained chart

Replace a_i in the physical conditional by a fixed local map s_i(a_i)
which is identity on the specified admitted retained range, satisfies
\(|s_i(a_i)|\le C|a_i|\), and has a fixed Lipschitz constant. No
second derivative bound is needed here. Keep the ambient regulator
(GMK.3) and, when used, the actual outer reserve (GMK.26).

The same carrier coefficients P_m and C_m apply. Their retained
endpoint monomials become s_i(a_i) and
\(s_i(a_i)^TMs_j(a_j)\), still depending only on those endpoints.
Their values satisfy (GMK.20) up to a fixed constant. A unit divided
finite difference is bounded by the Lipschitz constant times
\(1+|a_i|+|a_j|\). Thus (GMK.24)--(GMK.28) hold with fixed changed
constants and no new P factor.

This includes the local smooth saturation used in the positive
first-chart mask extension. On its admitted source states the
retained field is unchanged. It does not extend the Gaussian theorem
to the actual hard-cutoff or nonlinear density.

## 6. Application and what has not been proved

For the first flat Gaussian source step, the physical scalar quadratic
is a fixed positive sum of \(\|dC x\|^2\). The true exceptional
embedding C has a fixed stencil, so it fits (GMK.17)--(GMK.18).
The precision gap, upper bound and finite range are the same ones
checked in the first-step obstruction proof.

Thus the very nested-domain family used to disprove the source-derived
footprint estimate has a bounded full physical-carrier output in this
explicitly amended Gaussian local-mask interface. Its variance jump is
carried by the nearby primitive mask. There is no required connector
to the remote selector which generated that mask in the supported
probability law.

This is substantive progress on a replacement interface, not completion
of the original M04 statement. The following extensions are not supplied
by (GMK.28):

* the actual broad hard cutoff with a potentially displaced retained
  mean, uniformly in every allowed boundary datum;
* the complete non-Gaussian Wilson density and its all-history boundary
  action in this carrier expansion;
* changes of the determining geometry or nonlinear retained compact
  background, which change C and K and need their own true supported
  coefficient family;
* the chart conversion to the source's post-relocation retained filing;
* the actual outgoing moment reserve after every admitted history and
  the induction of a recursively transported marked input.

A distance-decay estimate for the hard-cutoff response does not by
itself imply (GMK.28), because the weight here charges physical carrier
volume. Likewise the literal narrow-cutoff product theorem is a
different argument and cannot silently replace the broad first cutoff.
