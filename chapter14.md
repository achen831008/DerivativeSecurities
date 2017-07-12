# Chapter 14 - Black-Scholes-Merton Model

Assumptions
-----------
1. The stock price follows the process developed with $\mu$ and $\sigma$ constant
2. The short selling of securities with full use of proceeds is permitted.
3. There are no transactions costs or taxes. All securities are perfectly divisible
4. There are no dividends during the life of the derivative
5. There are no riskless arbitrage opportunities
6. Security trading is continuous
7. The risk-free rate of interest, r, is constant and the same for all maturities

Black-Scholes-Merton Pricing Formulas
-------------------------------------

European call option:

$c = S_0 N(d_1) - Ke^{-rT} N(d_2)$

European put option:

$p = Ke^{-rT} N(-d_2) - S_0 N(-d_1)$

where

$d_1 = \frac{ln(S_0/K)+(r+\sigma^2 / 2) T} {\sigma \sqrt{T}}$

$d_2 = \frac{ln(S_0/K)+(r-\sigma^2 / 2) T} {\sigma \sqrt{T}} = d_1 - \sigma \sqrt{T}$




