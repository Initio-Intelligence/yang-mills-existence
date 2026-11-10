# A finite certificate for the Wilson thermal increment

## 1 The same transfer operator at every auxiliary temporal length

Fix one spatial torus with lattice spacing $a$⁠, physical side $T$⁠, and an even number $M = T/a \geq 4$ of sites per direction. This excludes no eventual cofinal members. Its actual Wilson coupling is the one selected by the matched construction; it does not change when the temporal length below changes. Write

$$s(U) = N - ReTrU,\quad\quad\beta = Y_{0}/N = 2Nx_{0} > 0,\quad\quad d = N^{2} - 1.$$

(TS20.1)

The trace is the ordinary fundamental matrix trace; Haar measure has total mass one. The numbers of spatial links and spatial plaquettes are both $L_{s} = P_{s} = 3M^{3}$⁠. Use the retained exact transfer construction of Annex M (1.1)--(1.2):

$$\begin{matrix}
Z_{1}(\beta) = \int_{SU(N)}^{}e^{- \beta s(U)}dU, \\
\left( C_{\beta}f \right)(u) = Z_{1}(\beta)^{- 1}\int e^{- \beta s\left( uv^{- 1} \right)}f(v)dv, \\
K = \bigotimes_{l = 1}^{L_{s}}C_{\beta},\quad\quad V_{s} = \beta\sum_{p\ spatial}^{}s\left( U_{p} \right), \\
A = e^{- V_{s}/2},\quad\quad\mathsf{T}_{0} = AKA.
\end{matrix}$$

(TS20.2)

Let $\mathsf{T}$ be the physical gauge-invariant restriction, let $\lambda_{0} > 0$ be its largest eigenvalue, and set $P = \mathsf{T}/\lambda_{0} = e^{- aH}$⁠, $H \geq 0$⁠. The retained positivity, compactness and character-coefficient facts make these positive trace-class operators at the finite cutoff, with a simple physical ground state. All traces below are physical traces. Equivalently the physical operator may be extended by zero on the gauge-null complement.

For $u \geq a$⁠, define

$$F(u) = \log Tr\mathsf{T}^{u/a},\quad\quad f(u) = \log Tre^{- uH} = F(u) - \frac{u}{a}\log\lambda_{0}.$$

(TS20.3)

Thus $f$ is nonnegative and nonincreasing. The desired increment is

$$\Gamma(T) = f(T/2) - f(T).$$

(TS20.4)

The powers used below have integer exponent when $M$ is even. These are exact powers of **one spatial operator**, not an asserted extension of a source-free RG theorem from cubes to rectangles. Spatial volume and coupling remain fixed within each dyadic sum; they change with the cofinal index.

## 2 An explicit entropy reserve for the interacting Wilson transfer

The next bound is extensive and cannot by itself close E-05. Its role is to give a uniform explicit error for truncating a positive dyadic sum.

### Lemma TS20 1 normalized Haar ball

Give $SU(N)$ the bi-invariant metric $ds^{2} = - Tr\left\lbrack \left( U^{- 1}dU \right)^{2} \right\rbrack$⁠. Set

$$v_{d} = \frac{\pi^{d/2}}{\Gamma(1 + d/2)},\quad\quad V_{N} = \frac{\sqrt{N}(2\pi)^{N(N + 1)/2 - 1}}{\prod_{j = 1}^{N - 1}j!},$$

$$c_{N} = \min\left\{ 1,\frac{2^{- N(N - 1)}v_{d}}{V_{N}} \right\},\quad\quad b_{N} = 4^{- d}c_{N}.$$

(TS20.5)

For $0 < r \leq 1$⁠, normalized Haar measure of

$$B_{r} = \{ e^{iX}:X = X^{*},\ TrX = 0,\ TrX^{2} \leq r^{2}\}$$

is at least $c_{N}r^{d}$⁠.

**Proof.** The exponential map is injective here: all eigenvalues of $X$ lie in $\lbrack - 1,1\rbrack$⁠, within the principal Hermitian logarithm interval. If they are $x_{1},\ldots,x_{N}$⁠, the exponential-coordinate volume Jacobian is

$$J(X) = \prod_{i < j}^{}\left\lbrack \frac{\sin\left( \left( x_{i} - x_{j} \right)/2 \right)}{\left( x_{i} - x_{j} \right)/2} \right\rbrack^{2}.$$

(TS20.6)

To see this, left translate the differential of the exponential to the identity; it is the integral of $Y \mapsto e^{- itX}Ye^{itX}$ over $0 \leq t \leq 1$⁠. It is the identity on diagonal directions, and its determinant on each off-diagonal real two-plane is the corresponding square in (TS20.6). Since $\left| x_{i} - x_{j} \right|/2 \leq 1/\sqrt{2} < 1$ and $\sin z/z \geq 1/2$ on that interval, $J(X) \geq 2^{- N(N - 1)}$⁠. Integrating over the Euclidean $d$-ball and dividing by $V_{N}$ proves the claim.

The metric volume $V_{N}$ can be checked explicitly. In $SU(k - 1) \rightarrow SU(k) \rightarrow S^{2k - 1}$⁠, the quotient metric at the identity has factor $2$ in the $2k - 2$ off-diagonal real directions and factor $k/(k - 1)$ in the last phase direction relative to the unit round sphere. Its volume is

$$2^{k - 1}\sqrt{\frac{k}{k - 1}}\frac{2\pi^{k}}{(k - 1)!} = \sqrt{\frac{k}{k - 1}}\frac{(2\pi)^{k}}{(k - 1)!}.$$

Multiplication from $k = 2$ to $N$ gives (TS20.5). The trace-metric conventions also agree with G. Moore's notes, (12.10)--(12.13), cited below. ∎

### Theorem TS20 2 explicit actual Wilson trace reserve

With (TS20.1)--(TS20.5), put

$$\boxed{B_{N,\beta,M} = 3M^{3}\left\lbrack \frac{17}{32} + 3\log\left( b_{N}^{- 1} \right) + \frac{3d}{2}\log(1 + \beta) \right\rbrack.}$$

(TS20.7)

Then

$$0 \leq f(u) \leq f(a) \leq B_{N,\beta,M}\quad\quad(u \geq a).$$

(TS20.8)

**Proof.** Set $r_{\beta} = \left\lbrack 4\sqrt{1 + \beta} \right\rbrack^{- 1}$⁠. On $B_{r_{\beta}}$⁠,

$$s\left( e^{iX} \right) = \frac{1}{2} \parallel I - e^{iX} \parallel_{HS}^{2} \leq \frac{1}{2}TrX^{2} \leq \left\lbrack 32(1 + \beta) \right\rbrack^{- 1}.$$

The Haar-ball estimate therefore gives

$$Z_{1}(\beta) \geq e^{- 1/32}b_{N}(1 + \beta)^{- d/2}.$$

(TS20.9)

On the event that every spatial link belongs to $B_{r_{\beta}}$⁠, unitary telescoping along a plaquette yields $\parallel I - U_{p} \parallel_{HS} \leq 4r_{\beta}$⁠, hence $\beta s\left( U_{p} \right) \leq 1/2$⁠. Consequently $A \geq e^{- P_{s}/4}$ on that event and

$$\int A\, dU \geq e^{- P_{s}/4}b_{N}^{L_{s}}(1 + \beta)^{- dL_{s}/2}.$$

(TS20.10)

The one-link convolution has eigenvalue one on constants and nonnegative eigenvalues on their orthogonal complement. Thus $K \geq \Pi_{\mathbf{1}}$⁠. Both the constant function and $A$ are gauge invariant. The physical Rayleigh principle gives

$$\begin{matrix}
\lambda_{0} \geq \langle\mathbf{1},AKA\mathbf{1}\rangle = \langle A,KA\rangle \geq (\int A\, dU)^{2} \\
 \geq e^{- P_{s}/2}b_{N}^{2L_{s}}(1 + \beta)^{- dL_{s}}.
\end{matrix}$$

(TS20.11)

The diagonal of the full-link kernel of $K$ equals $Z_{1}(\beta)^{- L_{s}}$⁠. Since $0 < A \leq 1$ and the physical space is reducing for the positive operator,

$${Tr}_{phys}\mathsf{T} \leq Tr\mathsf{T}_{0} = Z_{1}(\beta)^{- L_{s}}\int A^{2}\, dU \leq Z_{1}(\beta)^{- L_{s}}.$$

(TS20.12)

Combining (TS20.9)--(TS20.12),

$$\begin{matrix}
f(a) = \log{Tr}_{phys}\mathsf{T} - \log\lambda_{0} \\
 \leq P_{s}/2 + L_{s}/32 + 3L_{s}\log\left( b_{N}^{- 1} \right) + \left( 3dL_{s}/2 \right)\log(1 + \beta).
\end{matrix}$$

This is (TS20.7), since $P_{s} = L_{s} = 3M^{3}$⁠. A positive contraction with eigenvalue one has $f(u) \geq 0$ and nonincreasing in $u$⁠, completing the proof. ∎

This proof uses the full interacting transfer, including gauge and harmonic sectors. No Gaussian replacement, removal of physical flat holonomies, weak-coupling expansion, or spatially uniform gap is assumed. The bound is nevertheless too large to prove the desired rate: $B_{N,\beta,M}/T$ is of order $T^{2}a^{- 3}\left\lbrack 1 + \log(1 + \beta) \right\rbrack$⁠.

## 3 Positive temporal dilation defects cancel the ground energy

For $t > a$⁠, let $\rho_{t} = e^{- tH}/Tre^{- tH}$⁠. Trace class at $a$ controls every $H^{k}e^{- tH}$ at strictly later times by a scalar exponential majorant, so the derivatives below exist.

### Theorem TS20 3 ground independent dyadic identity

Define

$$\begin{matrix}
D(t) = F(t) - \frac{3}{2}F(2t) + \frac{1}{2}F(4t) \\
 = \frac{1}{2}\log\frac{\left\lbrack Tr\mathsf{T}^{t/a} \right\rbrack^{2}Tr\mathsf{T}^{4t/a}}{\left\lbrack Tr\mathsf{T}^{2t/a} \right\rbrack^{3}}.
\end{matrix}$$

(TS20.13)

Then $D(t) \geq 0$⁠. For $t_{j} = 2^{j}T/2$ and each integer $J \geq 0$⁠,

$$\boxed{\Gamma(T) = \sum_{j = 0}^{J - 1}2^{- j}D\left( t_{j} \right) + 2^{- J}\left\lbrack f\left( t_{J} \right) - f\left( 2t_{J} \right) \right\rbrack.}$$

(TS20.14)

In particular,

$$\boxed{0 \leq \Gamma(T) - \sum_{j = 0}^{J - 1}2^{- j}D\left( t_{j} \right) \leq 2^{- J}B_{N,\beta,M}.}$$

(TS20.15)

Thus the increasing positive partial sums determine the increment with an explicit error requiring neither the largest eigenvalue, ground vector, nor a finite-volume gap.

**Proof.** The linear term in (TS20.3) cancels because $t - 3t + 2t = 0$⁠, so $D$ is unchanged if $F$ is replaced by $f$⁠. Set $\mathcal{E}(u) = Tr\left( H\rho_{u} \right)$⁠. The spectral theorem gives

$$f'(u) = - \mathcal{E}(u),\quad\quad\mathcal{E}'(u) = - {Var}_{\rho_{u}}(H) \leq 0.$$

Therefore

$$\begin{matrix}
D(t) = \left\lbrack f(t) - f(2t) \right\rbrack - \frac{1}{2}\left\lbrack f(2t) - f(4t) \right\rbrack \\
 = \int_{t}^{2t}\left\lbrack \mathcal{E}(u) - \mathcal{E}(2u) \right\rbrack\, du \\
 = \int_{t}^{2t}{\int_{u}^{2u}{Var}_{\rho_{v}}}(H)\, dv\, du \geq 0.
\end{matrix}$$

(TS20.16)

Writing $\Gamma_{j} = f\left( t_{j} \right) - f\left( 2t_{j} \right)$ gives $D\left( t_{j} \right) = \Gamma_{j} - \Gamma_{j + 1}/2$⁠. Multiplication by $2^{- j}$ and telescoping proves (TS20.14). The remainder is bounded because $0 \leq \Gamma_{J} \leq f\left( t_{J} \right) \leq B_{N,\beta,M}$⁠. This also proves convergence of the series with its finite error; no large-time convergence theorem is needed to discard the tail. ∎

Replacing $\mathsf{T}$ by $c\mathsf{T}$ changes $F(u)$ by $(u/a)\log c$ and leaves $D$ unchanged. An exactly constant contribution to $F$ also cancels, since $1 - 3/2 + 1/2 = 0$⁠. Thus the defect does not charge a raw multiplicity entropy when that entropy has negligible effect on the thermal increment.

### Thermal purity and the checked factor

The normalized thermal state is unchanged by using $\mathsf{T}$ instead of $P$⁠. Its Rényi entropy of order two is

$$S_{2}(t) = - \log Tr\rho_{t}^{2} = 2F(t) - F(2t) = 2f(t) - f(2t).$$

(TS20.17)

Consequently

$$D(t) = \frac{1}{2}\left\lbrack S_{2}(t) - S_{2}(2t) \right\rbrack,\quad\quad\Gamma(2t) = \frac{1}{2}\left\lbrack S_{2}(t) - f(2t) \right\rbrack \leq \frac{1}{2}S_{2}(t).$$

(TS20.18)

Bounding the whole entropy is only sufficient. The positive dyadic series is exact and retains cancellations that such a bound can lose.

## 4 A finite certificate on the changing cubic family

Restore the cofinal index $n$⁠. Put $B_{n} = B_{N,\beta_{n},T_{n}/a_{n}}$ and $t_{n,j} = 2^{j}T_{n}/2$⁠. For arbitrary $\varepsilon_{n} \downarrow 0$ and fixed reference physical length $\ell_{0} > 0$⁠, choose

$$J_{n} = \max\left\{ 0,\left\lceil \log_{2}\frac{B_{n}\ell_{0}}{\varepsilon_{n}T_{n}} \right\rceil \right\},\quad\quad C_{n} = \sum_{j = 0}^{J_{n} - 1}2^{- j}D_{n}\left( t_{n,j} \right).$$

(TS20.19)

The reference length keeps the logarithm dimensionless. Then

$$\boxed{0 \leq \frac{\ell_{0}\Gamma_{n}\left( T_{n} \right)}{T_{n}} - \frac{\ell_{0}C_{n}}{T_{n}} \leq \varepsilon_{n}.}$$

(TS20.20)

The original vanishing trace-rate condition is therefore **equivalent** to $C_{n}/T_{n} \rightarrow 0$ with this explicit finite prescription. The bounded-rate variation in the homogeneous comparison 1 is equivalent to boundedness of $C_{n}/T_{n}$⁠. For $J_{n} \geq 1$⁠, adjacent defects reuse trace values: only $J_{n} + 2$ raw traces are needed, at lengths $T_{n}/2,T_{n},2T_{n},\ldots,2^{J_{n}}T_{n}$ on the same spatial torus. If $J_{n} = 0$⁠, the tail bound alone applies. For example, setting $\varepsilon_{n} = \ell_{0}/T_{n}$ makes the number of trace values $O\left( \log\left( T_{n}/a_{n} \right) + \log\left( 1 + \log\left( 1 + \beta_{n} \right) \right) \right)$⁠.

This argument gives an explicit finite error at each member of the changing family. It does not take a fixed-volume limit and silently substitute a different Hamiltonian. It still leaves the actual positive sum $C_{n}$ to be bounded.

### A connected thermal energy criterion

Define the dimensionless total heat capacity $\mathcal{C}_{n}(u) = u^{2}{Var}_{\rho_{n,u}}\left( H_{n} \right)$⁠. If, for fixed $p \geq 0$ and numbers $A_{n} \geq 0$⁠,

$$\mathcal{C}_{n}(u) \leq A_{n}\left( T_{n}/u \right)^{p}\quad\quad\left( u \geq T_{n}/2 \right),$$

(TS20.21)

then

$$\Gamma_{n}\left( T_{n} \right) \leq \left\{ \begin{matrix}
A_{n}\log 2, & p = 0, \\
A_{n}\left( 2^{p} - 1 \right)/\left\lbrack p(p + 1) \right\rbrack, & p > 0.
\end{matrix} \right.\ $$

(TS20.22)

**Proof.** Spectral dominated convergence gives $\mathcal{E}_{n}(u) \rightarrow 0$ as $u \rightarrow \infty$ at the fixed finite operator. Hence

$$\mathcal{E}_{n}(u) = \int_{u}^{\infty}{Var}_{\rho_{n,v}}\left( H_{n} \right)\, dv \leq \frac{A_{n}T_{n}^{p}}{p + 1}u^{- p - 1}.$$

Integrate from $T_{n}/2$ to $T_{n}$⁠, using Annex M (4.21). ∎

Thus $A_{n} = o\left( T_{n}/\ell_{0} \right)$ suffices for a vanishing rate; $A_{n} = O\left( T_{n}/\ell_{0} \right)$ suffices for a bounded rate. No such bound is proved here. The energy is the exact logarithm of the transfer. Its variance is **not** automatically the variance of a sum of bare scalar plaquettes or of the prescribed renormalized scalar field. An anisotropic or logarithmic-transfer identification requires its actual coefficients, counterterms and identity contribution. The finite difference (TS20.13) avoids that unproved identification.

## 5 What temporal polymer cancellation would have to establish

The three-length defect cancels every exactly time-linear contribution, including genuine bulk vacuum normalizations when the same contribution has been identified at all three lengths. A possible route is a linked expansion of the **log partition function** separating its time-linear part from clusters sensitive to the temporal period.

This is stronger than a local polymer decomposition of the **effective action**. After integrating the remaining coarse links and taking a logarithm, correlations of arbitrarily many short supported functions can form long connected chains. Locality of action terms alone does not show that only small time-wrapping contributions survive.

### Conditional cancellation estimate with a power law alternative

Suppose the actual raw trace at a fixed spatial torus has a compatible decomposition, for every $u \geq T/2$⁠,

$$F(u) = ub + R(u),\quad\quad\left| R(u) \right| \leq A\left( T/\ell_{0} \right)^{3}\left( \ell_{0}/u \right)^{p},\quad\quad p > 0.$$

(TS20.23)

Then

$$\boxed{\Gamma(T) \leq \frac{2^{p}\left\lbrack 1 + \frac{3}{2}\, 2^{- p} + \frac{1}{2}\, 4^{- p} \right\rbrack}{1 - 2^{- (p + 1)}}\, A\left( T/\ell_{0} \right)^{3 - p}.}$$

(TS20.24)

**Proof.** The linear term cancels. The three remainder bounds give

$$D\left( t_{j} \right) \leq A\left( T/\ell_{0} \right)^{3}\left( \ell_{0}/t_{j} \right)^{p}\left\lbrack 1 + \frac{3}{2}\, 2^{- p} + \frac{1}{2}\, 4^{- p} \right\rbrack.$$

Multiply by $2^{- j}$ and sum the exact series of Theorem TS20.3. ∎

For fixed $A$⁠, $p > 2$ suffices for the vanishing trace rate; $p = 2$ suffices for a bounded rate. A proved $p = 3$ remainder gives a uniform increment. Thus exponential clustering is more than this route requires.

If a full linked expansion instead yields

$$\left| R(u) \right| \leq A\left( T/\ell_{0} \right)^{3}\left( u/\ell_{0} \right)e^{- cu/\ell_{0}},\quad\quad c > 0,$$

(TS20.25)

then

$$\Gamma(T) \leq 3A\left( T/\ell_{0} \right)^{4}\frac{e^{- cT/\left( 2\ell_{0} \right)}}{1 - e^{- cT/\left( 2\ell_{0} \right)}}.$$

(TS20.26)

Indeed, $D(t) \leq 6A\left( T/\ell_{0} \right)^{3}\left( t/\ell_{0} \right)e^{- ct/\ell_{0}}$⁠, and $2^{j} \geq j + 1$ bounds the resulting series. For varying $A_{n}$⁠, this implies a vanishing rate when $\log^{+}A_{n} = o\left( T_{n}/\ell_{0} \right)$⁠. These are conditional implications, not established expansions for the matched Wilson family.

### The actual stopping scale obstruction

The completed coupling work matches one weak finite coupling at the physical scale $\ell_{0}$⁠. It does not integrate all scales between $\ell_{0}$ and the growing size $T_{n}$⁠. Even if all ultraviolet bulk factors first cancel compatibly in (TS20.13), a terminal compact gauge integral remains at each auxiliary temporal length. Its logarithm is an infrared contribution to the same three-length defect.

The source-free stability bounds control this integral extensively. A separate bound of size $C\left( T_{n}/\ell_{0} \right)^{3}\left( u/\ell_{0} \right)$ at each length proves neither (TS20.23) nor (TS20.25). Subtracting three numbers known only within such errors does not give a subextensive error. The terminal Wilson action at fixed positive coupling, physical flat holonomies, and connected correlations of remaining links cannot be discarded. Fixed physical auxiliary supports and exact coupling shooting ensure compatible definitions, but do not provide these connected infrared estimates.

A valid wrapping argument would require compatible period-independent cluster weights; absolute summability of the connected **log-partition** expansion including terminal integration; and a bound on clusters whose time extent makes them sensitive to the temporal identification. "Wrapping" here must include long clusters that lose a unique short lift, not just loops assigned nonzero winding. These properties have not been verified for the residual terminal measure. A cubic source-free theorem also cannot be applied to all auxiliary rectangles without a separate geometry justification.

## 6 Renormalized marks and the physical scale

The thermal estimate is one part of actual field passage. Annex M (4.5) also requires

$$\frac{\Gamma_{n} + 2\log^{+} \parallel X_{F,n} \parallel}{T_{n}} \rightarrow 0$$

for every fixed polynomial $F$ in the chosen renormalized hierarchy. If the actual mixing, identity and product-subtraction coefficients obey the finite polynomial cutoff budgets of Annex M (4.17)--(4.20), then $\parallel X_{F,n} \parallel \leq C_{F}a_{n}^{- d_{F}}$⁠, with degree-dependent $d_{F}$⁠. A compatible choice $\log\left( 1/a_{n} \right)/T_{n} \rightarrow 0$ pays that budget once the thermal certificate has actually been controlled. Replacing the actual coefficients by bare compact ones does not verify the premise.

For slower geometry, the homogeneous comparison 1's separated-time argument provides another conditional route using renormalized one-field slabs and off-diagonal limiting moment regularity. Its bounded-rate version allows one finite universal factor in the reduced OS inequality. Those premises are not supplied by the finite trace results here. The order of the continuum, smearing and time-shortening limits remains unchanged.

**Proved here:** an explicit trace reserve for the full interacting finite Wilson operator; a nonnegative three-length defect with exact scalar and ground-energy cancellation; an exact finite dyadic certificate with a uniform explicit error; and the stated conditional heat-capacity and period-sensitive remainder implications.

**Still unproved:** a vanishing or bounded cofinal rate for the actual positive certificate, or another original E-05 verification route with the actual hierarchy. **The cofinal E-05 application remains open.**
