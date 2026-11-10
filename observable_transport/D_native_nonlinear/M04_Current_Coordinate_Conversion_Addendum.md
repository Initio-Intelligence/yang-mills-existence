# Logarithm coordinates and the literal left raw current

OP and SD use ordinary logarithm coordinates to exploit a complex polydisc and the dilation parity. The literal physical path of DP/TR is a normalized left link path. The conversion acts within every owned current label and does not transfer a derivative between labels.

On one link write `U=exp(g a)`. For the physical path `U(s)=exp(s g h)U`, let

\[
 a(s)=g^{-1}\log(e^{sg h}e^{ga}),\qquad
 T_g(a)h=a'(0).
 \tag{CJ.1}
\]

The BCH logarithm is analytic on the fixed physical tube. Consequently

\[
 T_g(0)=I,\qquad
 T_g(a)=I+O(g\|a\|),
 \tag{CJ.2}
\]

with a uniformly bounded operator norm on each smaller tube. It acts on the same bond and its complete colour fiber, so it introduces no outside raw support. Its entrywise coordinate sums cost only a fixed group constant.

If \(j^r_{\log}(a;h)\) is any one of the literal copy-owned covectors, its left-raw version is exactly

\[
 j^r_{\mathrm{left}}(a;h)
       =j^r_{\log}(a;T_g(a)h).
 \tag{CJ.3}
\]

This equation is a coordinate change of that origin, not an identity obtained after adding different origins. It holds for the microscopic insertion derivative and for each density/domain/normalizer derivative with its prescribed test held fixed.

The OP/SD parity families have `j^r_log(0;h)=0` separately for each r, by their constant simultaneous colour argument. Differentiating (CJ.3) at zero gives

\[
 D_a j^r_{\mathrm{left}}(0;h)[k]
   =D_a j^r_{\log}(0;h)[k]
       +j^r_{\log}(0;D_aT_g(0)[k]h)
   =D_a j^r_{\log}(0;h)[k].
 \tag{CJ.4}
\]

Thus the per-origin **linear output jet** in OP.25--OP.26 and SD.28--SD.29 is exactly the literal left-raw jet. There is no correction to the two-coupling-power estimate. The same applies to the specified actual/Gaussian comparison because the Gaussian owned currents also have zero constant value.

For full current functions on the small-link slice, apply (CJ.3) to both the actual current and its compared Gaussian covector. Their difference is evaluated on the same `T_g(a)h`. Its deterministic first-current bound therefore changes only by the uniform fixed-colour factor. A comparison made in logarithm coordinates must not instead leave one of the two covectors in left coordinates. In particular OP.28 has its left-raw interpretation with this common pullback.

The ratio factors between the auxiliary b coordinate and the literal normalized a coordinate are still explicit: OP uses `b=(g_3/g_2)a`, and SD uses `b=(g_3/g_0)a`. One factor occurs for the owned current direction and a second for its linear field jet. The bond-local BCH conversion above is in addition to those already recorded scalar factors.

This addendum clarifies the coordinate convention. It does not assert a field-dependent gauge cancellation or an age gain for a fixed old innovation.
