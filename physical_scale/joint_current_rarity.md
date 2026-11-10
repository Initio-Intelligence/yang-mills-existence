# Joint current rarity and outer averaging

**Conditional application.** Use the stated source, support and fixed-chart hypotheses. Any application of the complete C05 boundary estimates or the C06/C08 law to all original Wilson histories assumes spatial and native-domain control of the iterated reconstruction with the earlier innovations fixed. The actual composed response required for that application remains open.

## Assumptions and conclusions

This is a consequence of the conditional C06 coercivity, C07 product support and C08 mean profile at their retained source/C01 scope. It strengthens the single-coordinate collar estimate RC18.38 to an arbitrary prescribed set of current coordinates. No independence of those coordinates is assumed.

It also gives a precise positive-law averaging and insertion version. It does not identify an inherited low-margin or unreplaced-history event with a current regular-coordinate event. That identification, and any physical component weight it must pay, remain obligations of H02/H04.

## 1. Full-vector centered exponential bound

Fix an admitted outer fiber \(v\), and let \(\nu_v\) be its actual regular conditional law on the C07 product of symmetric convex free-bond balls. In the C06 normalization, choose one fixed \(\lambda>0\), for example \(\lambda=\lambda_0/2\), below the real Hessian lower bound. It holds uniformly in volume, cutoff and retained history. Let \(m=\nu_v z\).

For every real finitely supported block vector \(t\),
\[
 \nu_v\exp\langle t,z-m\rangle
 \le \exp\{\|t\|_2^2/(2\lambda)\}.
 \tag{JR.1}
\]

To prove this, put \(\psi(s)=\log\nu_v e^{s\langle t,z\rangle}\). Each real linear tilt has the same Hessian and support. The scalar Neumann/convexity estimate gives
\[
 \psi''(s)=\operatorname{Var}_{\nu_{v,s}}(\langle t,z\rangle)
 \le\lambda^{-1}\|t\|_2^2.
\]
Integrating twice between zero and one gives (JR.1). On literal nonsmooth balls, prove the scalar variance and exponential inequalities on smooth convex product approximants and pass them by dominated convergence at the fixed finite cutoff. The integrand is bounded on that compact product for every fixed \(t\). This uses no identification of an arbitrary-vector differentiated operator on the limiting nonsmooth boundary. [C06 application, CA.15; C08 application; original AY, RC18.21–RC18.34 and the independent support qualification]

The dimension in (JR.1) is the full number of independent coordinates. Its constant does not grow with that dimension.

## 2. Arbitrarily many prescribed high coordinates

Write \(d\) for an upper bound on the fixed real dimension of one free-bond Lie-algebra block. All norms in this section are its Euclidean Hilbert norms; another fixed block norm changes only fixed constants.

Let \(J\) be any finite set of distinct independent coordinates and \(u_i>0\). Then
\[
 \nu_v\{\|z_i-m_i\|\ge u_i\text{ for every }i\in J\}
 \le
 5^{d|J|}
 \exp\left\{-\frac{\lambda}{8}\sum_{i\in J}u_i^2\right\}.
 \tag{JR.2}
\]

For each block choose a \(1/2\)-net \(\mathcal N_i\) of its unit sphere with at most \(5^d\) points. If \(\|x\|\ge u\), some \(e\in\mathcal N_i\) has \(\langle e,x\rangle\ge u/2\). Fix one such direction for each \(i\) and apply (JR.1) with \(t_i=(\lambda u_i/2)e_i\). On the simultaneous directional event,
\[
 \langle t,z-m\rangle\ge\frac{\lambda}{4}\sum_i u_i^2,
 \qquad
 \frac{\|t\|_2^2}{2\lambda}
 =\frac{\lambda}{8}\sum_i u_i^2.
\]
Exponential Markov inequality gives the exponential in (JR.2); the union over the at most \(5^{d|J|}\) direction lists gives its prefactor. The proof never multiplies single-site probabilities.

## 3. A uniform interior high-field penalty

Let \(d_O(i)\) be the current-unit distance to the retained current exterior. The C08 mean profile is
\[
 \|m_i\|\le C_m\{P^{-1}+Pe^{-c_m d_O(i)}\}.
 \tag{JR.3}
\]
Fix any threshold fraction \(a>0\). Choose \(d_0\), independent of cutoff and \(P\), such that
\[
 C_m e^{-c_m d_0}\le a/4,
\]
and reduce the common coupling ceiling so that \(C_m/P\le aP/4\). Thus \(\|m_i\|\le aP/2\) whenever \(d_O(i)\ge d_0\).

For every finite \(J\) consisting of these interior coordinates,
\[
 \nu_v\{\|z_i\|\ge aP\text{ for every }i\in J\}
 \le \exp\{-c_a P^2|J|\},
 \qquad c_a=\lambda a^2/64,
 \tag{JR.4}
\]
once \(P^2\ge64d\log5/(\lambda a^2)\). Indeed, the event implies \(\|z_i-m_i\|\ge aP/2\); substituting in (JR.2) and absorbing the net entropy proves (JR.4).

If the literal bond ball contains a Euclidean ball of radius \(c_D P\), being outside half that literal ball implies \(\|z_i\|\ge c_D P/2\). Taking \(a=c_D/2\) gives the corresponding simultaneous collar-event estimate. Without that lower radius comparison, use the explicit Euclidean event in (JR.4). No support convention is silently changed.

The interior restriction matters. The retained exterior force may produce a mean of order \(P\) at the boundary. Coercivity by itself does not give (JR.4) there.

## 4. Unions, insertions and positive outer averaging

For a collection \(\mathcal J_n(v)\) of prescribed \(n\)-element interior sets,
\[
 \nu_v\{\text{at least one }J\in\mathcal J_n(v)
                 \text{ satisfies the event in (JR.4)}\}
 \le |\mathcal J_n(v)|e^{-c_aP^2n}.
 \tag{JR.5}
\]
In particular an entropy bound \(|\mathcal J_n(v)|\le e^{bn}\) is paid by decreasing \(c_a\) by a fixed factor at one sufficiently small ceiling. The family is chosen from the retained data; an adaptive choice after observing \(z\) needs its actual enumeration in (JR.5).

Let \(E_J\) denote the event in (JR.4), and let \(F\) be any measurable insertion with finite actual conditional \(L^p(\nu_v)\) norm. For \(1\le q<p<\infty\), Hölder gives
\[
 \left(\nu_v[|F|^q\mathbf1_{E_J}]\right)^{1/q}
 \le \|F\|_{L^p(\nu_v)}
       \exp\{-c_aP^2|J|(1/q-1/p)\}.
 \tag{JR.6}
\]
The insertion norm is not replaced by an unshifted or unrelated mark norm.

Let the exact positive full law have disintegration \(\pi(dv)\nu_v(dz)\), as exposed in H01. Let \(A\) be an event of retained data, and \(J(v)\) a measurable choice of \(n\) eligible interior coordinates on \(A\). Integrating (JR.4) gives
\[
 \mathbb P\{v\in A,\ E_{J(v)}\}
 \le e^{-c_aP^2n}\pi(A).
 \tag{JR.7}
\]
The positive probability \(\pi(A)\) is retained. More generally, (JR.6) gives the full-law insertion bound
\[
 \mathbb E[|F|^q\mathbf1_A\mathbf1_{E_{J(v)}}]
 \le e^{-c_aP^2n(1-q/p)}
       \int_A\|F(v,\cdot)\|_{L^p(\nu_v)}^q\,\pi(dv).
 \tag{JR.8}
\]
These statements allow arbitrary dependence of the chosen set and the insertion on the retained fiber, provided the eligibility and conditional norm hypotheses hold there.

## 5. The exact remaining history step

Equations (JR.5)–(JR.8) are usable once a proposed history sector has been represented by the stated current-coordinate events and its actual combinatorial and insertion costs have been bounded. A cost \(e^{L(v,J)}\) is absorbed if the available conditional estimates prove \(L(v,J)\le c_aP^2|J|/2\), with the corresponding Hölder fraction when required.

No such comparison follows simply from a small normalized component mass: that mass may already have canceled in the posterior. Nor do the estimates apply automatically to old raw coordinates, low-margin labels, archived selectors or failed unreplaced components. Those are the specific remaining geometric/probabilistic identification tasks before this corollary can discharge an H02 or H04 sector.

Thus the proved output is a uniform, simultaneous, insertion-compatible penalty for actual regular current high-coordinate events, together with its exact outer-law averaging formula. It is a concrete input to the next history argument, not a claim that the full history induction or Yang–Mills existence has been completed.

\newpage
