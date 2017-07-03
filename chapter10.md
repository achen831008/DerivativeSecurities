# Chapter 10 - Properties of Stock Options

Factors Affecting Option Prices
===============================

1. The current stock price
2. The strike price
3. The time to expiration
4. The volatility of the stock price
5. The risk-free interest rate
6. The dividends that are expected to be paid

Increase in one variable while keeping all others fixed

| Var | Euro Call | Euro Put | Amer Call | Amer Put|
|--------|---|---|---|---|
|  $S_0$ | + | - | + | - |
|   $K$  | - | + | - | + |
|   $T$  | ? | ? | + | + |
|$\sigma$| + | + | + | + |
|   $r$  | + | - | + | - |
| $Div$  | _ | + | - | + |


Upper and Lower Bounds for Option Prices
========================================

**Upper bound** 

$C = S_0$
$P = Ke^{-rT}$ for European option 
$P = K$ for American option

**Lower bound** 

$C = S_0 - Ke^{-rT}$ for European call option with non-dividend-paying stocks
$C = S_T - Ke^{-rT} - PV(Div)$
$P = Ke^{-rT} - S_0$ for European put option with non-dividend-paying stocks
$P = Ke^{-rT} - S_T + PV(Div)$

**Example**

Consider a European call option on a non-dividend-paying stock when the stock price is \$51, the strike price is \$50, the time to maturity is 6 months, and the risk-free interest rate is 12% per annum.
$51 - 50e^{-0.12 * 0.5} = 3.91$

**Example**

Consider a European put option on a non-dividend-paying stock when the stock price is \$38, the strike price is \$40, the time to maturity is 3 months, and the
risk-free rate of interest is 10% per annum
$40e^{-0.1 * 0.25} - 38 = 1.01$

Put-Call Parity
===============

$Portfolio_A = C + Ke^{-rT} = P + S_0 = Portfolio_B$

If $P_B$ is overpriced relative to $P_A$, an arbitrageur can buy the call and short both the put and the stock.

If $P_A$ is overpriced relative to $P_B$, an arbitrageur can buy both the put and the stock and short the call.

**With Dividend**

$Portfolio_A = C + Ke^{-rT} + PV(Div) = P + S_0 = Portfolio_B$


