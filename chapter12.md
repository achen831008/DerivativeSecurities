# Chapter 12 - Binomial Trees

A One-step Binomial Model and A No-Arbitrage Argument
=====================================================

A Generalization
----------------

$S_0u \delta - f_u = S_0d \delta - f_d$ or
$\delta = \frac {f_u - f_d} {S_0u - S_0d}$

$f = e^{-rT} (p f_u + (1 - p) f_d)$
where $p = \frac {e^{rT} - d} {u - d}$

**Example**

Put with $K = 52, S_0 = 50, u = 1.2, d=0.8, \delta t = 1, r = 0.05$

$p = \frac {e^{0.05 * 1} - 0.8}{ 1.2 - 0.8} = 0.6282$

|-----------------------72

|---------60 (B)

|---50(A)------------48

|---------40 (C)

|-----------------------32

payoff for put is $max(K - S, 0)$

$B = e^{-0.05 * 1} (0.6282 * 0 + (1-0.6282) * 4) = 1.4147$

$C = e^{-0.05 * 1} (0.6282 * 4 + (1-0.6282) * 20) = 9.4636$

$A = e^{-0.05 * 1} (0.6282 * 1.4147 + (1-0.6282) * 9.4636) =4.1923$

So, the value of the put is 4.1923.





















