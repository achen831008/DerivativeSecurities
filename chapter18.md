# Chapter 18 - The Greek Letters


Naked and Covered Positions
===========================

Naked Position referred to as financial institution to do nothing.
Covered Position is to buy the underlying asset when you sell it.

Delta Hedging
=============

Delta is the rate of change of the option price with respect to the price of the underlying asset.

delta = 0.6, this means that when the stock price changes by a small amount, the option price changes by about 60% of that amount

When the delta of the stock position offsets the delta of the option position, this is referred to as **delta neutral**.

**Rebalancing** would happen if the delta changes. One would need to buy/sell more shares to be **delta neutral**.

This is referred to as **dynamic hedging**.

Delta of European Stock Options
-------------------------------

**long**

$\delta (call) = N(d_1)$

$\delta (put) = N(d_1) - 1$

**Short**

$\delta (call) = -N(d_1)$

$\delta (put) = 1 - N(d_1)$


Delta is negative, which means that a long position in a put option should be hedged with a long position in the underlying stock, and a short position in a put option should be hedged with a short position in the underlying stock.


Delta of a Portfolio
--------------------

Suppose a financial institution has the following three positions in options on a
stock:
1. A long position in 100,000 call options with strike price \$55 and an expiration date
in 3 months. The delta of each option is 0.533.
2. A short position in 200,000 call options with strike price \$56 and an expiration
date in 5 months. The delta of each option is 0.468.
3. A short position in 50,000 put options with strike price \$56 and an expiration date
in 2 months. The delta of each option is -0.508.

The delta of the whole portfolio is 100,000 * 0.533 - 200,000 * 0.468 - 50,000 * (-0.508) = -14,900


Gamma
=====

The gamma ($\gamma$) of a portfolio of options on an underlying asset is the rate of change of the portfolio's delta with respect to the price of the underlying asset.

If gamma is small, delta changes slowly, and adjustments to keep a portfolio delta neutral need to be made only relatively infrequently.


Making a Portfolio Gamma Neutral
--------------------------------
Suppose that a portfolio is delta neutral and has a gamma of -3,000. The **delta** and **gamma** of a particular traded call option are **0.62** and **1.50**, respectively. The portfolio can be made gamma neutral by including in the portfolio a long position of $\frac {3,000} {1.5} = 2,000$ in the call option. However, the delta of the portfolio will change from zero to $2000 * 0.62 = 1,240$. Therefore, 1,240 unit of underlying asset must be **sold** from the portfolio to keep it **delta neutral**.


Calculation of Gamma
--------------------

$\gamma = \frac {N'(d_1)} {S_0 \sigma \sqrt{T}}$

Consider a call option on a non-dividend-paying stock where the stock price is \$49, the strike price is \$50, the risk-free rate is 5%, the time to maturity is 20 weeks (= 0.3846 years), and the volatility is 20%. In this case, $S_0 = 49, K = 50, r = 0.05, \sigma = 0.2, and T = 0.3846$

The option's gamma is 0.066.


VEGA
====

The vega of a portfolio of derivatives, $\nu$, is the rate of change of the value of the portfolio with respect to the volatility of the underlying asset.

If vega is highly positive or negative, the portfolio's value is very sensitive to small changes in volatility. If it is close to zero, volatility changes have relatively little impact on the value of the portfolio.

$\nu = S_0 \sqrt{T} N'(d_1)$






