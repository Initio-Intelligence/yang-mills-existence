# Normalized microscopic defects, source jets and exact matching

**Annex O.** All estimates have the hypotheses stated below. Applications to the complete Wilson conditional law use the common assumptions in [the theorem catalogue](../THEOREMS_AND_OPEN_PROBLEMS.md).


### Result and scope

The complete-history obligations C0/H0 and the exact transported-field matching obligation M0 remain open. This note proves a new microscopic, fully interacting statement that addresses one of their genuine local obstructions: cancellation of the staples in a conditional link law.

For the full compact SU(2) Wilson measure:

1. The conditional minimum of the incident plaquette energy is an explicit nonnegative function of the surrounding links. Joint low-staple events, for arbitrarily dependent link neighborhoods, have a normalized exponential bound controlled by that minimum energy.
2. Whenever the resultant staple has a fixed positive lower bound, the centered one-link source logarithm has a common complex source ball and a bound **linear in the conditional minimum energy**. Consequently every conditional scalar cumulant has a factorial bound with that same linear dependence. No small plaquette condition on the boundary, Gaussian replacement, or removal of exceptional interior configurations is used.
3. Averaging the remaining low-staple sector against the actual Wilson law controls every conditional scalar response, uniformly in volume and coupling. A family of links with no plaquette containing two of them gives an exact, local, all-order elimination layer.

These are initial-lattice statements. The exact coarse constrained fibers in the RG/R construction are not one-link Wilson laws. The result therefore does not identify coarse inherited low-margin events with these microscopic defects, and does not remove the physical factor \(a^{-4}\) in a dimension-four field.

Here **P** denotes a proof below, **L** a scoped standard special-function input, and **O** an application still missing for the Yang–Mills construction.

### 1. The actual Wilson law and the already-proved reserve

Let \(d\ge2\), \(M=2(d-1)\), and let the periodic lattice have an even side \(n\ge4\). Use normalized Haar measure and the exact compact SU(2) Wilson law

\[
d\mu_{\beta,n}(U)
=Z_{\beta,n}^{-1}\exp\!\left[-\sum_p e_p(U)\right]\,dH(U),
\qquad
e_p=\beta\left[2-\operatorname{Re}\operatorname{Tr}U_p\right].
\tag{1.1}
\]

The coefficient dictionary remains
\(\beta=2Nx_0=4x_0\) for \(N=2\), and
\(X_B=N\beta=2\beta\).

We use the constant local exponential reserve proved in Annex A:

\[
\mathbb E_{\mu_{\beta,n}}
 \exp\!\left(\eta\sum_{p\in X}e_p\right)
\le K^{b(X)}.
\tag{1.2}
\]

Here \(\eta>0\) and \(K\) are fixed along the cofinal family, \(b(X)\) is the unit-cube cover count, and the sufficient geometric condition is
\(\sup \log(1+\beta)/n<\infty\). In dimension four one may take
\(0<\eta\le1/8\). At a single finite lattice the same proof uses
\(K_{\beta,n}=C_{2,d}(1+\beta)^{3d/(2n)}\); all statements below remain true with that explicit value.

Equation (1.2) is a bound for the normalized full Wilson probability law. It retains every compact field configuration. In particular, for any fixed plaquette stencil \(X\),

\[
\left\|\sum_{p\in X}e_p\right\|_{L^r(\mu_{\beta,n})}
\le C_X r,\qquad r\ge1.
\tag{1.3}
\]

The only earlier constructive input in this note is (1.2). Its proof uses the actual Wilson reflection/chessboard geometry and matched partition-function powers, as in Annex A. No reflection property of an auxiliary RG history law is assumed here.

### 2. An exact conditional minimum at one link

Fix an oriented link \(l\), and condition on every other link. Identifying SU(2) with the unit quaternions \(S^3\), write its remaining quaternion as \(u\). Every incident plaquette contribution has the form

\[
e_{l,p}(u)=2\beta(1-v_{l,p}\cdot u),
\qquad v_{l,p}\in S^3,\qquad p\ni l.
\tag{2.1}
\]

Orientation or an inverse occurrence of \(U_l\) is absorbed into the unit vector \(v_{l,p}\). The real part of the fundamental trace is twice the quaternion scalar product. Define

\[
v_l=\sum_{p\ni l}v_{l,p},\qquad
\rho_l=|v_l|\in[0,M],\qquad
B_l=2\beta(M-\rho_l).
\tag{2.2}
\]

These quantities depend on the links other than \(l\). The norm \(\rho_l\), and hence \(B_l\), is gauge invariant: a gauge transformation rotates all the relevant quaternion vectors by the same orthogonal left/right multiplication at the endpoints of \(l\).

The exact conditional law is

\[
Q_l(du\mid U_{\ne l})
=\frac{\exp(2\beta v_l\cdot u)}
 {\mathcal Z(2\beta\rho_l)}\,d\sigma_{S^3}(u),
\qquad
\mathcal Z(r)=\frac{2I_1(r)}r,\qquad \mathcal Z(0)=1.
\tag{2.3}
\]

The normalization identity follows by integrating the normalized \(S^3\) marginal \((2/\pi)(1-t^2)^{1/2}\,dt\); it is also the \(\nu=1\) case of the integral representation in NIST DLMF 10.32.2.

#### Lemma 2.1 — conditional minimum, P

\[
\boxed{
B_l=\min_{u\in S^3}\sum_{p\ni l}e_{l,p}(u)
\le E_l(U):=\sum_{p\ni l}e_p(U).
}
\tag{2.4}
\]

If \(\rho_l>0\), the minimizing direction is \(u_l^*=v_l/\rho_l\). Put
\(a_{l,p}=v_{l,p}\cdot u_l^*\) and
\(v_{l,p}^{\perp}=v_{l,p}-a_{l,p}u_l^*\). Then

\[
\boxed{
\sum_{p\ni l}|v_{l,p}^{\perp}|^2
\le2(M-\rho_l)=B_l/\beta.
}
\tag{2.5}
\]

The last expression is used only for \(\beta>0\); for \(\beta=0\) every marked energy is zero.

**Proof.** The incident energy equals
\(2\beta(M-v_l\cdot u)\). Its minimum is achieved by maximizing the scalar product, which gives (2.4). Also
\(\sum_p a_{l,p}=\rho_l\) and
\(1-a_{l,p}^2\le2(1-a_{l,p})\) for
\(-1\le a_{l,p}\le1\). Sum this inequality. \(\square\)

The boundary may be very far from a regular plaquette configuration. In particular, the canceled-staple example \(\rho_l=0\) is included. It has \(B_l=2\beta M\), so its arbitrary-boundary conditional fluctuations can be large while its occurrence in the normalized outer law can be estimated.

### 3. Joint normalized probabilities of low-staple events

Let \(\Gamma\) be any finite set of distinct links. Define

\[
X_\Gamma=\{p:\partial p\cap\Gamma\ne\varnothing\},
\qquad
m_\Gamma=\max_p|\partial p\cap\Gamma|\le4.
\tag{3.1}
\]

For a nonempty \(\Gamma\), \(1\le m_\Gamma\le4\). No disjoint-neighborhood or independence assumption is imposed.

#### Theorem 3.1 — full-law low-staple suppression, P

For prescribed \(0<\delta_l\le M\),

\[
\boxed{
\mathbb P_{\mu_{\beta,n}}
 \left(\rho_l\le M-\delta_l\ \text{for every }l\in\Gamma\right)
\le
K^{b(X_\Gamma)}
\exp\!\left[
-\frac{2\eta\beta}{m_\Gamma}
 \sum_{l\in\Gamma}\delta_l
\right].
}
\tag{3.2}
\]

One always has \(b(X_\Gamma)\le M|\Gamma|\). In particular, for a fixed
\(\rho_*\in(0,M)\), with \(\delta=M-\rho_*\),

\[
\mathbb P(\rho_l<\rho_*\text{ for all }l\in\Gamma)
\le
\exp\!\left[
-|\Gamma|\left(\frac{\eta\beta\delta}{2}-M\log K\right)
\right].
\tag{3.3}
\]

**Proof.** Pointwise on the full configuration space,

\[
\sum_{l\in\Gamma}B_l
\le\sum_{l\in\Gamma}E_l
\le m_\Gamma\sum_{p\in X_\Gamma}e_p.
\tag{3.4}
\]

On the event in (3.2), its left side is at least
\(2\beta\sum_l\delta_l\). Apply exponential Markov with (1.2). A link has \(M\) incident plaquettes, and covering each such plaquette separately proves
\(b(X_\Gamma)\le M|\Gamma|\). Use \(m_\Gamma\le4\) for (3.3). \(\square\)

This is a normalized, volume-uniform estimate. It applies to the original configurations on the joint space of any later positive history coupling because that coupling preserves their Wilson marginal. It is not a claim that a coarse current-selector failure implies \(\rho_l<\rho_*\) at some original link.

#### Corollary 3.2 — marked version with the full rarity factor, P

Suppose original marks obey
\(\|A_i\|_r\le Cb_i r\) for all \(r\ge1\).
Let \(\mathcal Q\) be any composite frozen positive transport on an augmented output that retains the event in (3.3) as a history label. Thus \(\mathcal Q\) denotes conditional transport to that augmented output; it is not an unchanged conditional kernel subsequently conditioned on an omitted event. Put

\[
\sigma_\beta=\frac{\eta\beta\delta}{2}-M\log K,
\qquad r_\Gamma=|\Gamma|.
\]

When \(\sigma_\beta\ge0\),

\[
\boxed{
\mathbb E\!\left[
\mathbf1_{\{\rho_l<\rho_*:\ l\in\Gamma\}}\,
\left|\kappa_{\mathcal Q}(A_1,\ldots,A_m)\right|
\right]
\le
e^{-\sigma_\beta r_\Gamma}
C^{m+1}m!\,
(m+\sigma_\beta r_\Gamma)^m
\prod_i b_i.
}
\tag{3.5}
\]

For a full transported product coefficient, omit the extra \(m!\).

**Proof.** Use the arbitrary-event estimate with the true event probability \(q\). The function
\[
e^{-\lambda}(m+\lambda)^m
\]
is nonincreasing for \(\lambda\ge0\), since its logarithmic derivative is
\(-1+m/(m+\lambda)\le0\). Hence the upper bound
\(q\le e^{-\sigma_\beta r_\Gamma}\) may replace \(q\) in that estimate. Conditional contraction applies to the composite positive transport. \(\square\)

For dimension-four bare fields \(b_i\) still contains \(a^{-4}\). The theorem does not assert that an isolated bad-link event absorbs this factor for every source order. It supplies the actual normalized probability that the earlier generic rare-event lemma required for this specific microscopic event.

### 4. A common complex source ball with linear background-energy cost

The next estimate uses the exact compact conditional integral, rather than a Gaussian approximation. Fix
\[
0<\rho_*<M.
\]
The constants below may depend on \(d,\rho_*\), but not on \(\beta,n\), boundary data, or the number of source labels.

#### Theorem 4.1 — regular-resultant conditional log jets, P with a scoped L input

Suppose \(\rho_l\ge\rho_*\). Let \(p_1,\ldots,p_m\) be any incident plaquettes, with repetitions permitted, and set
\[
\widetilde e_i=e_{l,p_i}-Q_l e_{l,p_i}.
\]
There is \(r_*>0\), independent of \(m\), such that

\[
\Phi_l(t)
:=
\log Q_l\exp\!\left(\sum_{i=1}^m t_i\widetilde e_i\right)
\tag{4.1}
\]

has its branch \(\Phi_l(0)=0\) throughout the complex \(\ell^1\) ball
\(\sum_i|t_i|<r_*\), and

\[
\boxed{
|\Phi_l(t)|
\le C(1+B_l)\left(\sum_i|t_i|\right)^2.
}
\tag{4.2}
\]

Consequently, for every \(m\ge2\),

\[
\boxed{
|\kappa_{Q_l}(e_{l,p_1},\ldots,e_{l,p_m})|
\le C^{m+1}m!\,(1+B_l).
}
\tag{4.3}
\]

This is not a uniform source logarithm for arbitrary coarse Wilson actions. It is a theorem about the explicit one-link law (2.3).

#### Proof: the exact complex reduction

Suppress the link index, put \(v=\rho u_*\), and write
\[
w(t)=\sum_i t_i v_{p_i},
\qquad
w_\parallel=u_*\cdot w,
\qquad
w_\perp=w-w_\parallel u_*.
\]
The dot product in the following expression is the complex bilinear extension of the real Euclidean scalar product. For sufficiently small
\(s=\sum_i|t_i|\), define

\[
q(t)
=\sqrt{(\rho-w_\parallel)^2+w_\perp\cdot w_\perp},
\qquad q(0)=\rho.
\tag{4.4}
\]

Choose a fixed \(s_0>0\), depending only on \(\rho_*\), small enough that
\[
|q-\rho|\le Cs,\qquad
\operatorname{Re}q\ge\rho/2,\qquad
|\arg q|\le\pi/4,\qquad
|q+\rho-w_\parallel|\ge c\rho
\tag{4.5}
\]
whenever \(s<s_0\). These follow by the analytic square root around
\(\rho^2\) and \(|w|\le s\).

The source integral is exactly

\[
Q_l\exp\!\left(\sum_i t_i e_{l,p_i}\right)
=
\exp\!\left(2\beta\sum_i t_i\right)
\frac{\mathcal Z(2\beta q(t))}{\mathcal Z(2\beta\rho)}.
\tag{4.6}
\]

For real source vectors this follows by rotation of the quaternion integral. Both sides are holomorphic near zero, and the power-series rotational identity extends it to the stated complex neighborhood. Equivalently, \(\mathcal Z(\sqrt{z\cdot z})\) is entire in the four complex components of \(z\), because \(\mathcal Z\) has an even power series.

#### Proof: the large-argument branch and its estimate

The only additional literature input is the fixed-order modified-Bessel asymptotic in a closed sector:

\[
I_1(z)=\frac{e^z}{\sqrt{2\pi z}}\,[1+O(|z|^{-1})],
\qquad |\arg z|\le\pi/4,\quad |z|\longrightarrow\infty,
\tag{4.7}
\]

with a uniform remainder there. This is NIST DLMF 10.40.1; the error-bound discussion is in 10.40(iii). It implies that, on this sector above a fixed radius,

\[
\log\mathcal Z(z)
=z-\frac32\log z+c_0+R(z),
\qquad |R(z)|\le C/|z|,
\tag{4.8}
\]

with a holomorphic bounded remainder and no zeros. The zero-free statement here follows directly from the relative error \(1+O(1/z)\) after increasing that fixed radius; a zero theorem outside the sector is not used.

If \(2\beta\rho\) is above a sufficiently large fixed threshold, (4.5) puts every \(2\beta q(t)\), \(s<s_0\), in this same domain. Therefore (4.6) has a well-defined logarithm on the full source ball. Up to a linear term, the logarithm is the sum of
\[
2\beta q(t),\qquad
-\frac32\log(q(t)/\rho),\qquad
R(2\beta q(t))-R(2\beta\rho).
\tag{4.9}
\]

The first term has an exact quadratic remainder:

\[
q-\rho+w_\parallel
=\frac{w_\perp\cdot w_\perp}{q+\rho-w_\parallel}.
\tag{4.10}
\]

By (2.5),
\[
|w_\perp|^2
\le s^2\sum_{p\ni l}|v_p^\perp|^2
\le s^2 B_l/\beta.
\tag{4.11}
\]
Together with (4.5), this bounds the centered contribution of the first term in (4.9) by \(CB_l s^2\).

The other two terms in (4.9) are uniformly bounded holomorphic functions on the larger source ball \(s<s_0\). Subtracting their constant and linear terms leaves a bound \(Cs^2\) on a fixed smaller ball. To see the dimension independence explicitly, fix a source direction \(t\) with \(\|t\|_1=s\) and apply the one-variable Taylor estimate to
\(z\mapsto f(zt/s)\), on a disc of radius \(s_0\). The bound depends only on the \(\ell^1\) radius, not on the number of coordinates.

Subtracting the full linear term in the logarithm of (4.6) is exactly the centering in (4.1). This proves (4.2) in the large-argument regime.

#### Proof: bounded arguments and cumulants

If \(2\beta\rho\) stays below the fixed threshold, then
\(\beta\le C/\rho_*\). All incident energies and their centered versions are uniformly bounded. On a sufficiently small common \(\ell^1\) source ball,
\[
\left|Q_l e^{\sum_i t_i\widetilde e_i}-1\right|<1/2.
\]
The logarithm is then holomorphic and uniformly bounded. Its constant and linear terms vanish, so the same one-variable Taylor estimate proves (4.2), with \(1+B_l\ge1\).

Finally apply multivariable Cauchy to (4.2) on coordinate radii
\(r_*/(2m)\). The mixed derivative is bounded by
\[
C(1+B_l)(2m/r_*)^m.
\]
Use \(m^m\le e^m m!\) and enlarge \(C\). For \(m\ge2\), centering does not change the cumulant. This proves (4.3). \(\square\)

#### Corollary 4.2 — actual conditional centered moments, P

For \(\rho_l\ge\rho_*\), every incident plaquette satisfies

\[
\boxed{
\|e_{l,p}-Q_l e_{l,p}\|_{L^r(Q_l)}
\le C\bigl[r+\sqrt{(1+B_l)r}\bigr],
\qquad r\ge1.
}
\tag{4.12}
\]

**Proof.** The real-source case of (4.2) gives
\(\log Q_l e^{t\widetilde e}\le C(1+B_l)t^2\) for
\(|t|\le r_*/2\). Chernoff optimization with
\[
|t|=\min\{r_*/2,\,u/[2C(1+B_l)]\}
\]
gives a two-sided tail
\[
Q_l(|\widetilde e|\ge u)
\le2\exp\{-c\min(u^2/(1+B_l),u)\}.
\]
Tail integration yields (4.12). \(\square\)

The dependence on \(B_l\) cannot simply be discarded: a large retained boundary mismatch can generate large individual-plaquette fluctuations even though the conditional total excess has good moments. The result identifies that dependence and supplies its actual outer-law control.

### 5. Averaging every conditional response over the full Wilson law

#### Theorem 5.1 — averaged conditional scalar hierarchy, P

For every one-link conditional kernel and every tuple of its incident plaquettes,
\[
J_{m,l}=
\kappa_{Q_l}(e_{l,p_1},\ldots,e_{l,p_m}),
\qquad m\ge2,
\]
the full Wilson law obeys

\[
\boxed{
\mathbb E|J_{m,l}|
\le C^{m+1}(m!)^2.
}
\tag{5.1}
\]

More precisely,

\[
\mathbb E[
\mathbf1_{\{\rho_l\ge\rho_*\}}|J_{m,l}|]
\le C^{m+1}m!,
\tag{5.2}
\]

while, for every fixed \(m\),

\[
\boxed{
\mathbb E[
\mathbf1_{\{\rho_l<\rho_*\}}|J_{m,l}|]
\le C^{m+1}m!\,\beta^m e^{-c\beta}.
}
\tag{5.3}
\]

Constants are independent of cutoff and volume along the cofinal reserve family. The last estimate shows that the degenerate-resultant contribution is smaller than every inverse power of \(\beta\) at every fixed source order.

**Proof.** On \(\rho_l\ge\rho_*\), use (4.3), \(B_l\le E_l\), and the fixed-stencil reserve. This gives (5.2).

For arbitrary boundary data, \(0\le e_{l,p}\le4\beta\). A centered bounded family has a uniformly bounded logarithmic generating function on an \(\ell^1\) source ball of radius \(c/\beta\), so Cauchy gives
\[
|J_{m,l}|\le C^{m+1}m!\,\beta^m.
\tag{5.4}
\]
At \(\beta=0\) this is immediate. The one-link case of (3.2) gives
\(\mathbb P(\rho_l<\rho_*)\le C e^{-c\beta}\), proving (5.3). Finally,
\[
\sup_{\beta\ge0}\beta^m e^{-c\beta}
=\left(\frac m{ce}\right)^m\le c^{-m}m!,
\tag{5.5}
\]
where the last inequality follows from
\(\log m!\ge\int_1^m\log x\,dx=m\log m-m+1\).
Combining (5.2)–(5.5) proves (5.1). \(\square\)

The general conditional-cumulant contraction bound already gave a magnitude estimate of the form (5.1). The new content here is the explicit linear-\(B_l\) bound before outer averaging, its sharper \(m!\) regular-resultant part, and a normalized exponentially small estimate for the degenerate-resultant part. These statements do not assume a uniform good boundary.

### 6. An exact local elimination layer

Let \(\Gamma\) now satisfy the concrete geometry condition

\[
\text{no plaquette contains two distinct links of }\Gamma.
\tag{6.1}
\]

Condition on all links outside \(\Gamma\). Every Wilson plaquette factor then depends on at most one remaining link. Thus

\[
\mu(dU_\Gamma\mid U_{\Gamma^c})
=\prod_{l\in\Gamma}Q_l(dU_l\mid U_{\Gamma^c})
\tag{6.2}
\]

exactly, including all compact configurations. In particular, the staples \(v_{l,p}\), and the functions \(\rho_l,B_l\), depend only on the retained links.

For sources on scalar plaquette energies, partition the marked plaquettes according to the unique eliminated link they meet, leaving the plaquettes meeting no eliminated link as retained-data functions. The normalized source functional factors:

\[
Q_\Gamma e^{\sum_p t_p e_p}
=
e^{\sum_{p:\,\partial p\cap\Gamma=\varnothing}t_p e_p}
\prod_{l\in\Gamma}
Q_l e^{\sum_{p\ni l}t_p e_p}.
\tag{6.3}
\]

The identity holds for actual finite sources and hence coefficientwise for every finite source jet.

#### Corollary 6.1 — local all-order responses, P

Every logarithmic response of order at least two created by this elimination vanishes unless all its marked plaquettes meet the same eliminated link. Each surviving response depends only on the retained links in that link's plaquette star. On \(\rho_l\ge\rho_*\) it satisfies (4.3), and its full-law average satisfies (5.1)–(5.3).

**Proof.** Take the logarithm of (6.3) and differentiate. Each summand has only the corresponding one-link source arguments. The scalar plaquette data entering (2.1) use the other three links of the incident plaquette, so the response support is precisely local in the stated retained variables. \(\square\)

Such layers exist on every sufficiently large periodic cubic lattice: greedily color the finite link-conflict graph in which two links are adjacent if they lie in one plaquette. Its degree is bounded only by dimension. Each color class obeys (6.1). This observation proves existence of a uniformly finite number of admissible *first* layers; it does not make successive conditional laws after eliminating different colors remain Wilson one-link laws.

This is a genuine local source-jet calculation for the complete microscopic measure. It supplies no long-distance decay for the covariance of the resulting retained-data means. After the retained variables are integrated further, their law has new interactions; restarting (2.3) without accounting for those interactions would be incorrect.

#### 6.2 Full tensor products: the one-layer error is a controlled contact strip

The conditional product structure has a consequence for the actual finite field family, beyond the scalar logarithmic jets. It is an application of the earlier flat-test estimate to a newly identified exact response kernel; the Taylor estimate itself is not being claimed as a new mechanism.

Let \(\{O_{\alpha,a}(x)\}\) be a fixed finite family of microscopic gauge-invariant fields. Assume:

1. Each \(O_{\alpha,a}(x)\) depends only on links in a stencil contained in a physical ball of radius \(R a\), with \(R\) independent of the cutoff.
2. On the actual Wilson law,
   \[
   \|O_{\alpha,a}(x)\|_{L^r(\mu_{\beta,n})}
   \le C a^{-4}r,\qquad r\ge1,
   \tag{6.4}
   \]
   uniformly in labels and positions.

The explicit instance is
\(O_{\alpha,a}=\beta\widetilde q_{\alpha,a}
-\mathbb E[\beta\widetilde q_{\alpha,a}]\)
for the 21-field family of Annex E (scalar trace replaced by the Wilson action density). It satisfies these
two hypotheses: unitary parallel transports preserve curvature norms,
\(|\widetilde q_{AB,a}|\le2w_a\), and (1.2) gives (6.4).
Vacuum centering preserves the bound with a fixed constant. A different
running normalization requires its own coefficient budget and is not
included merely by calling the field renormalized.

For a set \(\Gamma\) obeying (6.1), define the projected fields by the **actual conditional expectation**

\[
\widehat O_{\alpha,a}(x)
=Q_\Gamma O_{\alpha,a}(x)
=\mathbb E[O_{\alpha,a}(x)\mid U_{\Gamma^c}],
\tag{6.5}
\]

and their full-moment difference kernel by

\[
D_{m,a}(\boldsymbol x)
=
\mathbb E\!\left[\prod_{i=1}^mO_{\alpha_i,a}(x_i)\right]
-
\mathbb E\!\left[\prod_{i=1}^m
 \widehat O_{\alpha_i,a}(x_i)\right].
\tag{6.6}
\]

The field in (6.5) is a function of retained links in a stencil enlarged by only a fixed number of lattice spacings: only the conditional kernels of eliminated links actually appearing in the original mark need to be integrated, and each such kernel depends on its plaquette star.

#### Theorem 6.2 — exact one-layer matching on coincidence-flat tests, P

For \(m\ge2\),

\[
\boxed{
D_{m,a}(\boldsymbol x)=0
\quad\text{if the original marked stencils share no eliminated link},
}
\tag{6.7}
\]

and

\[
\boxed{
|D_{m,a}(\boldsymbol x)|
\le C^{m+1}m!\,a^{-4m}
\mathbf1_{\{\min_{i<j}d_T(x_i,x_j)\le 2Ra\}}.
}
\tag{6.8}
\]

Here \(d_T\) is the torus distance. The equality \(D_{1,a}=0\) is exact.

For a joint Schwartz test \(F\) that is coincidence-flat, use an interior torus embedding: choose fixed weights \(0\le\zeta_T\le1\) supported in a central cube of side at most \(T/2\), and assume \(T\ge T_0(R)\), \(0<a\le1\), so that two anchors in that cube which share one microscopic stencil link are also within \(2Ra\) in the ordinary physical metric. Then

\[
\boxed{
\left|
a^{4m}\sum_{\boldsymbol x}
D_{m,a}(\boldsymbol x)
F(x_1,\ldots,x_m)\prod_i\zeta_T(x_i)
\right|
\le
a\,C^{m+1}m!\,\nu_{6m}(F),
}
\tag{6.9}
\]

where

\[
\nu_s(F)=
\max_{|\alpha|\le s}\sup_X
(1+|X|^2)^{s/2}|\partial^\alpha F(X)|.
\tag{6.10}
\]

The same assertion holds for compact tests supported in such a nonwrapping patch, without the weights. For comparison along expanding tori one may take \(\zeta_T=1\) on expanding compact subsets of the interior. All constants are independent of the number of eliminated links, volume, cutoff and source order. Every field-label tuple in the finite family is included. An arbitrary choice of \(\Gamma\) is not asserted to preserve finite-cutoff translations or reflection positivity of the projected-field hierarchy.

**Proof of the exact support statement.** Let \(I_i\subset\Gamma\) be the set of eliminated links on which the \(i\)-th mark actually depends. Given the retained variables, (6.2) makes the eliminated variables independent. If the sets \(I_i\) are pairwise disjoint, the conditional expectation of the product is the product of the conditional expectations. This proves (6.7). If two marked stencils share an eliminated link, their anchors have torus distance at most \(2Ra\), proving the support inclusion in (6.8).

**Proof of the magnitude estimate.** Conditional contraction and Hölder give

\[
\begin{aligned}
|D_{m,a}(\boldsymbol x)|
&\le
\mathbb E\prod_i|O_{\alpha_i,a}(x_i)|
+\mathbb E\prod_i|\widehat O_{\alpha_i,a}(x_i)|
\\
&\le 2\prod_i\|O_{\alpha_i,a}(x_i)\|_m
\le 2C^m m^m a^{-4m}
\le C^{m+1}m!a^{-4m}.
\end{aligned}
\tag{6.11}
\]

This bound is for the full products. It already includes every response generated by the one-layer conditional integration; no product of single means has been substituted without estimating its difference.

**Proof of the joint flat-test estimate.** At every point contributing to (6.9), choose one colliding pair with ordinary separation at most \(2Ra\). Taylor-expand \(F\) along the displacement taking one of its coordinates to the other, to order
\[
k_m=4m+1\le6m.
\]
Coincidence flatness annihilates every lower term. The displacement is \(O(a)\), so the integral remainder gives

\[
|F(X)|
\le
C^{m+1}a^{4m+1}
(1+|X|^2)^{-3m}\nu_{6m}(F)
\tag{6.12}
\]

on this collision strip. The intermediate points differ from \(X\) in one coordinate by \(O(a)\); since \(a\le1\), their Schwartz weights differ by a factor at most \(C^{m+1}\). The directional multi-index sum is bounded by the \(k_m\)-th power of the displacement's \(\ell^1\) norm. The Taylor factorial could be retained and only improves the displayed bound.

The elementary weighted lattice estimate is

\[
a^{4m}\sum_{\boldsymbol x}
(1+\sum_i|x_i|^2)^{-3m}
\le
\left[
a^4\sum_{x\in a\mathbb Z^4}(1+|x|^2)^{-3}
\right]^m
\le C^m.
\tag{6.13}
\]

Multiply (6.8) by (6.12), use (6.13), and keep the weights \(\zeta_T\) bounded by one. No derivative of these weights is needed in this estimate. This proves (6.9). \(\square\)

Thus this one microscopic elimination layer preserves the full off-diagonal Schwinger hierarchy up to an error that vanishes in a fixed OS-type seminorm, provided the field budget (6.4) is the one being used. It proves an exact matching statement modulo a controlled contact strip for that layer.

**Group scope of Theorem 6.2.** Its proof uses only the factorization of a Wilson plaquette action under (6.1), conditional contraction, and (6.4). It does not use quaternions, Bessel functions or the scalar-source theorem. Consequently Theorem 6.2 applies unchanged to every fixed \(SU(N)\) covered by the existing Wilson reserve and 21-field moment budget, with \(e_p=\beta[N-\operatorname{Re}\operatorname{Tr}U_p]\). The low-staple and Bessel-source theorems in Sections 2--5 remain SU(2) statements.

The theorem does not show that a second colored elimination has the product conditional law (6.2), nor that an unbounded number of such projections retains a shrinking physical stencil. After a fixed positive physical scale is reached, a local stencil need no longer have radius \(O(a)\). The all-scale matching theorem M0 therefore remains open. This result supplies a verified microscopic starting step, not a replacement for the missing induction.

### 7. Why this does not close the coarse inherited-history theorem

The microscopic estimate resolves the canceled-staple obstruction in an averaged form: arbitrary-boundary conditional bounds can fail, yet the bad boundary geometry has a quantified cost under the actual normalized Wilson law. It also shows that a source logarithm can have a useful common complex radius in a restricted conditional system, with its background dependence kept visible.

Three missing identifications prevent promotion to H0 or M0:

1. **Coarse margins are different objects.** A coarse selector depends on nonlinear constrained minimizing fields, currents, preparatory geometry and old history. No theorem identifies its failure with the events \(\rho_l<\rho_*\) or bounds its retained minimum by the microscopic \(B_l\)'s with a sufficient current-scale factor.
2. **Exact transported marks are different functions.** The one-link marks in (4.1) are original plaquette energies. After RG integration and history resets, the full source jet has generated responses and remainder vertices. They are not automatically native plaquette sources in a new one-link Wilson kernel.
3. **Outer covariance remains.** Even when every conditional fluctuation is controlled, the covariance of the retained conditional means remains in the exact law of total covariance. The local response identity (6.3) does not estimate it.

The actual all-history estimate still needs a current-scale normalization \(h_k^{-4}\), spatial localization for every generated response, and a bound for the complete outer law. The power \(a^{-4}\) on an original physical insertion has not disappeared in this note.

### 8. Assessment of a history-fugacity route

An analytic signed expansion may legitimately compute a generating function of a positive history law. It need not itself be a probability decomposition. That observation suggests inserting local history fugacities

\[
Z(z)=\sum_\omega\int \rho_\omega(V)
\exp\!\left(\sum_B z_B\,\xi_B(V,\omega)\right)\,dV,
\tag{8.1}
\]

where \(0\le\xi_B\le1\) are specified local selector flags.

At every finite cutoff, (8.1) exists and is entire in a finite collection of \(z_B\)'s. For its normalized functional \(M(z)=Z(z)/Z(0)\), boundedness and positivity give the precise uniform estimate

\[
|M(z)-1|
\le e^{\sum_B|z_B|}-1.
\tag{8.2}
\]

Consequently there is a zero-free complex \(\ell^1\) ball, with a bounded logarithm, whose radius is independent of the number of blocks. This useful elementary ball is not a common per-coordinate \(\ell^\infty\) ball: a fixed amplitude at each of many blocks has a growing \(\ell^1\) norm. Nor does (8.2) give a carrier-localized logarithm or spatial decay of its mixed derivatives. The missing history-fugacity theorem concerns those stronger spatial and extensive-source norms, not existence of the elementary \(\ell^1\) ball.

The source-free signed expansion can be used for this purpose only after proving that the fugacity-weighted **same** positive-history kernels obey the required absolute activity norms, with the selectors, current domains and background dependence retained. Multiplication by a real bounded flag preserves a real mass bound, but a flag may be a hard selector depending on a moving background. It does not automatically preserve the complex-background analyticity used in the effective-action cluster norm. Nor does an estimate at \(z=0\) control derivatives in \(z\).

The earlier LFR residual factor supports a localized source theorem for bounded marks at fixed retained data once the cross-interaction norm is verified; the positive-interpolation theorem already captures that restricted use. It does not control fugacities that change the outer selected geometry or the covariance of their retained-data means. None of the published sources used here supplies the missing uniform fugacity induction. The idea remains a possible proof route, not an imported theorem.

### 9. References and completion conditions

The one-link formulas and estimates use:

- the proof of the compact Wilson reserve in Annex A. This is the only prior lattice-probability input to (3.2).
- NIST Digital Library of Mathematical Functions, [10.32.2](https://dlmf.nist.gov/10.32.E2), the modified-Bessel integral representation, and [10.40.1](https://dlmf.nist.gov/10.40.E1), the fixed-order sectorial large-argument asymptotic. The complex error discussion is [10.40(iii)](https://dlmf.nist.gov/10.40.iii). These standard special-function inputs are used only to establish the one-link source ball in Section 4. The normalized probability and locality arguments are proved directly.
- The frozen positive transport and history-resampling identities proved in Annexes A and I. They are used for the explicit marked corollary, not to infer spatial mixing.

| Statement | Status |
|---|---|
| Joint normalized probabilities for arbitrary sets of microscopic low-resultant-staple links | P, Theorem 3.1 |
| Their transported marked contribution with a full rarity factor | P, Corollary 3.2 |
| Common complex source ball for one-link scalar jets, with linear conditional-minimum dependence | P with the stated special-function input, Theorem 4.1 |
| Full-law averaged conditional responses, including canceled-staple sectors | P, Theorem 5.1 |
| Exact spatial locality of an admissible microscopic elimination layer | P, Corollary 6.1 |
| Full 21-field one-layer matching modulo a contact strip with \(aC^{m+1}m!\nu_{6m}\) error | P for the stated actual field budget, Theorem 6.2 |
| Coarse inherited-selector probabilities and full-history spatial responses | O |
| Complete current-coordinate E/R contour and majorant theorem | O |
| Exact transported Wilson-to-native-field matching | O |
| Four-dimensional Yang–Mills existence | Not proved |


---
