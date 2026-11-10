# Shooting at common Gaussian record depths

The identification of the cumulative Gaussian marginal with a linear drift up to a uniformly bounded remainder is a separate hypothesis (GC). An arithmetic consequence of that drift does not prove GC or match a prescribed physical endpoint.

**Status.** The fixed Gaussian calibration selects cofinal cutoff depths at which the literal terminal source inequality holds simultaneously for every admitted bare shot. There are explicit bare brackets of width \(O(\log K)\) at these depths. A jump in the terminal readout from below the chosen target to above it remains possible with the presently proved estimates. B-05 remains open. The target below is the preassigned inverse coupling in the source units of B-03.

## Common depths before choosing any bare parameter

Write \(b=Y_0=N\beta_W\), \(y=Y_{\rm phys}>F\), where \(F\) is a fixed stopping floor above all source ceilings in inverse-coupling units, with the one-step buffer of Appendix F. In the fixed scheme the uncut Gaussian increments have deterministic prefix \(G_j=dj+q_j\), \(q_0=0\), \(|q_j|\le Q\), \(d=d_B>0\). Every causal Wilson prefix with inputs \(Y_i\ge F\) has the provisional physical update
\[
 Y_{i+1}=Y_i-(G_{i+1}-G_i)-e_i,\qquad |e_i|\le A/Y_i .
\]
The same \(G\) for different bare values is essential here. It comes from the fixed uncut stationary Gaussian, including its gauge/coarea and thermodynamic readout. Fix \(F>2Q\) sufficiently large that \(\varepsilon=A/F<d\), set \(d_\pm=d\pm\varepsilon\), and take \(0<a<d_-\). Keep the source's fixed \(L\), charts and rounding rule.

Let \(K\) range over running maxima of \(V_j=G_j-(a+\varepsilon)j\), ties allowed. With \(c=d-a-\varepsilon>0\), \(V_j=cj+q_j\). If \(r\) is the last record through \(n\), then \(0\ge V_n-V_r\ge c(n-r)-2Q\). In particular a record occurs in every interval of \(1+\lfloor2Q/c\rfloor\) consecutive nonnegative indices. At a record, the Gaussian suffix has slope at least \(a+\varepsilon\). For every admitted shot to this *same* \(K\),
\[
 a(K-j)\le Y_j-Y_K=G_K-G_j+\sum_{i=j}^{K-1}e_i
       \le(d_++2Q)(K-j),\qquad 0\le j\le K.                       \tag{1}
\]
For the upper bound absorb \(2Q\) at positive integer age, and use equality at age zero. The lower bound pays the worst possible signed interacting errors over this suffix. Thus the sharp terminal lower envelope no longer requires trimming **after** choosing the shooting parameter. At a shot with terminal value in a fixed compact interval above \(F\), (1) also gives Appendix H's period/divisor bound uniformly. One can use \(a_K=\ell_0 L^{-K}\), the centered compatible periods of PE.19–24, and the original finite-torus replay. Source envelope and geometry, Appendix H §§3–5

## A bracket that handles premature stopping

Define a scalar function \(T_K(b)\) for \(b\ge F\). Follow the actual source until \(K\) or the first provisional \(Y_t<F\). In the latter case put \(e_i=0\) for \(i\ge t\) in the numerical recursion and take its value at \(K\). This completion only defines the scalar bracket. The pre-exit coefficients and \(Y_t\) are the original ones. The completed array still has \(|e_i|\le\varepsilon\) everywhere. Equation (1) therefore holds even beyond an exit. In particular \(T_K(b)\ge F\) at a record implies \(Y_j\ge F\) at every \(j\le K\), and this shot and all of its replay are genuine.

Let \(u\) be the last admitted input index used before \(K\), with \(u\le K-1\). For \(i\le u\), the corrected drift gives \(Y_i\ge F-2Q+d_-(u-i)\). With \(h=F-2Q>0\), put
\[
 M_K=\frac{A}{h}+\frac{A}{d_-}\log(1+d_-K/h).
\]
Summing the decreasing reciprocal majorant and bounding its tail by an integral gives \(|\sum_{i<K}e_i|\le M_K\). Consequently for every sufficiently large record and any fixed \(s>0\), the explicit bare values
\[
 b_\pm=G_K+y\pm(M_K+s)
\]
satisfy \(b_-\ge F\), \(T_K(b_-)\le y-s\), \(T_K(b_+)\ge y+s\). In particular the upper shot is always physical. The bracket is centered at \(dK+q_K+y\) and has width \(2(M_K+s)\) in native bare units.

One can also obtain genuine lower and upper shots on common cofinal record depths when \(y\) has extra weak reserve. Take \(Z_*>F+Q+d_+\), \(J=\lfloor 2Q/c\rfloor\), and assume
\[
                     Z_*+d_+(1+J)+Q<y .
\]
Run any Appendix H sequence \(b_n\to\infty\) to its last corrected index \(U_n\) above \(Z_*\). Let \(K_n\) be the last Gaussian record through \(U_n\). Then \(U_n-K_n\le J\) and
\[
 F<Z_*-Q\le Y_{K_n}< Z_*+d_+(1+J)+Q<y .
\]
Indeed \(Z_{U_n}<Z_*+d_+\) and each preceding corrected step costs at most \(d_+\). These lower shots are actual. Their bare parameters lie below the explicit \(b_+\) at the same \(K_n\) by the total-error bound. Choose a strictly increasing subsequence of \(K_n\). This proves a genuine two-sided bracket without assuming every intermediate shot survives. The extended scalar bracket above requires only \(y>F\).

## The sign of a crossing that shooting actually needs

Bisect the bare bracket at a record depth, retaining a low-value left endpoint and high-value right endpoint. Either a tested bare value hits \(y\), or nested intervals shrink to some \(b^*\). Include constant sequences at \(b^*\) when a bracket endpoint stops moving. A sufficient exact test at every possible straddling limit is
\[
 \liminf_m T_K(x_m^-)\ \ge T_K(b^*)\ \ge\limsup_m T_K(x_m^+),\qquad
 x_m^-\uparrow b^*,\quad x_m^+\downarrow b^*,                      \tag{2}
\]
where only straddling endpoint sequences need to be tested. Indeed the low values give \(T_K(b^*)\le y\) and the high ones give \(T_K(b^*)\ge y\). The actual equality label at a rounded threshold occurs in the middle of (2). Downward jumps in increasing bare parameter are allowed. If both inequalities hold up to additive \(\delta_K\), the actual value at \(b^*\) is within \(\delta_K\) of \(y\). For \(\delta_K<y-F\) the record certificate guarantees physical admission. A cofinal \(\delta_K\to0\) would tune the scalar in the limit. Exact finite-cutoff normalization requires exact hits or a separate exact calibration. Any physical state compatibility required by the frozen normalization would still have to use these same tuned shots.

For a bound available on **both** sides, take two actual shots to a record \(K\), with physical terminal values at least \(w\ge F\). At any common comparison index \(j\le K\), telescoping and canceling the common Gaussian sequence give
\[
 |Y_K^+-Y_K^-|\le |Y_j^+-Y_j^-|
    +2A\sum_{s=1}^{K-j}\frac{1}{w+as}
 \le |Y_j^+-Y_j^-|+\frac{2A}{a}\log(1+a(K-j)/w).                 \tag{3}
\]
This uses (1) separately on each actual history, including histories with different mature resets. If the first differing incoming grid has index \(j\) and the preceding construction has a common limiting \(Y_j\), the input-difference term vanishes in that limit. An outgoing grid change alone, at the very step that installs \(Y_j\), does not alter that step's provisional germ by BP.24 and the subsequent replay argument. The later steps in (3) can use different incoming grids and mature banks. Even a single subsequent step leaves a fixed positive upper bound at fixed \(w\). At large remaining depth the bound grows. It supplies neither the orientation in (2) nor an error tending to zero with cutoff depth. Appendix I passes HS.23–27 on each extracted, labeled branch with the mature reset bank as forcing. Its assertion about one branch supplies no ordering between the two sides in (2). Causal replay, Appendix F pp. 79–80 · Threshold labels and limiting equation, Appendix I §§8–9 · Bałaban, CMP 119, pp. 278–279

The target test (2), or a physical matching estimate that bypasses it, remains a concrete missing input. Cases in which the lower side of a straddle exits before the terminal step are included in the completed bracket and must be covered by a proof of (2). The record argument alone gives no such crossing comparison.
