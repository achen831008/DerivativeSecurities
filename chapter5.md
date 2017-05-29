# Chapter 5 - Determination of Forward and Futures Prices

> An **investment asset** is an asset that is held for investment purposes by significant numbers of investors. (i.e. stocks and gold)

> A **consumption asset** is an asset that is held primarily for consumption. (i.e. copper, oil, pork bellies)

Short Selling
================

Note: An investor with a short position must pay to the broker any income such as dividends or interest, that would normally be received on the securities that have been shorted.

Assumptions and Notation
========================

We assume the following are all true:

 1. The market participants are subject to no transaction costs when they trade
 2. The market participants are subject to the same tax rate on all net trading profits
 3. The market participants can borrow money at the same risk-free rate of interest as they can lend money
 4. The market participants take advantage of arbitrage opportunities as they occur

The following notation will be used throughout this chapter:

> $T$: Time until delivery date in a forward or futures contract (in years)
> $S_0$: Price of the asset underlying the forward or futures contract today
> $F_0$: Forward or futures price today
> $r$: Zero-coupon risk free rate of interest per annum, expressed with continuous compounding, for an investment maturing at the delivery date

Forward Price For An Investment Asset
=====================================

Consider a forward contract on an investment asset with price $S_0$ that provides no income. Using our notation, $T$ is the time to maturity, $r$ is the risk-free rate, and $F_0$ is the forward price. The relationship between $F_0$ and $S_0$ is

> $F_0 = S_0 e$<sup>rT</sup>

No Income
---------
When forward price is out of line with spot price for asset providing no income. (Asset Price = 40; interest rate = 5%; maturity of forward contract = 3 months.)

**Situation 1: (If Forward Price = \$43)**

*Action Now:*

 - Borrow \$40 at 5% for 3 months
 - Buy one unit of asset
 - Enter into forward contract to sell asset in 3 months for $43

*Action in 3 months:*

 - Sell asset for \$43
 - Use $40.50 to repay loan with interest

**Profit realized = $2.50**

**Situation 2: (If Forward Price = \$39)**

*Action Now:*

 - Short 1 unit of asset to realize $40
 - Invest $40 at 5% for 3 months
 - Enter into forward contract to buy asset in 3 months for $39

*Action in 3 months:*

 - Buy asset for $39
 - Close short position
 - Receive $40.50 from investment

**Profit realized = $1.50**

If $F_0$ > $S_0 e$<sup>rT</sup>, arbitrageurs can buy the asset and short forward contracts on the asset. If $F_0$ < $S_0 e$<sup>rT</sup>, they can short the asset and enter into long forward contracts on it.

Known Income
------------

When an investment asset will provide income with a present value of $I$ during the life of a forward contract, we have

> $F_0 = (S_0 - I) e$ <sup> rT </sup> 

If $F_0$ > $(S_0 - I) e$<sup>rT</sup>, arbitrageurs can buy the asset and short forward contracts on the asset. If $F_0$ < $(S_0 - I) e$<sup>rT</sup>, they can short the asset and enter into long forward contracts on it.

Known Yield
===========

> $F_0 = S_0 e$ <sup> (r-q) T </sup>

where $q$ is the average yield per annum on an asset during the life of a forward contract with continuous compounding.

Valuing Forward Contracts
=========================

> $K$ is the delivery price for a contract that was negotiated some time ago.
> The delivery date is $T$ years from today.
> $r$ is the T-year risk-free interest rate.
> $F_0$ is the forward price that would be applicable if we negotiated the contract today.
> $f$ is the value of forward contract today.

Long forward contracts:

> **No Income:**
> $f = (F_0 - K) e$ <sup>-rT</sup>
> $ = S_0 - Ke$ <sup>-rT</sup>

> **Known Income:**
> $f = S_0 - I - Ke$ <sup>-rT</sup>
> $  = S_0 e$<sup>-qT</sup> $- Ke$ <sup>-rT</sup>

Futures on Commodities
======================

**Income and Storage Costs**

> $F_0 = (S_0 + U)e$<sup>rT</sup>
> $= S_0 e$<sup>(r+u) T</sup>

 - $U$ is the present value of all the storage costs
 - $u$ denotes the storage costs per annum as a proportion of the spot price net of any yield earned on the asset

**Consumption Commodities**

If $F_0 > (S_0 + U)e$<sup>rT</sup>

 1. Borrow an amount $S_0 + U$ at the risk-free rate and use it to purchase one unit of the commodity ad to pay storage costs
 2. Short a futures contract on one unit of the commodity

If $F_0 < (S_0 + U)e$<sup>rT</sup>

 1. Sell the commodity, save the storage costs, and invest the proceeds at the risk-free interest rate
 2. Take a long position in a futures contract

**Convenience Yields**

> $F_0 = S_0 e$<sup>(r + u - y) T</sup>

where y is the convenience yield.

The convenience yield reflects the market's expectations concerning the future availability of the commodity. The greater the possibility that shortages will occur, the higher the convenience yield.


Cost of Carry
=============

> Cost of Carry measures the storage cost plus the interest that is paid to finance the asset less the income earned on the asset.

 1. **Non-dividend-paying stock**: cost of carry is $r$
 2. **Stock Index**: cost of carry is $r - q$
 3. **Currency**: cost of carry is $r - r_f$
 4. **Commodity**: cost of carry is $r - q + u$

> For an investment asset, the futures price is
> $F_0 = S_0 e$<sup>cT</sup>

> For a consumption asset, the futures price is
> $F_0 = S_0 e$<sup>(c - y) T</sup>

where $y$ is the convenience yield and $c$ is the cost of carry.

Futures Prices and Expected Future Spot Prices
==============================================

> $F_0 = E(S_T) e$<sup>(r-k) T</sup>

 - $S_T$ is the price of the asset at time T at the end of the futures contract
 - $k$ is an investor's required return for this investment

| Underlying asset        | Relationship of expected return $k$ from asset to risk-free rate $r$           | Relationship of futures price F to expected future spot price $E(S_T$)  |
| ------------- |:-------------:| -----:|
| No Systematic risk     | $k = r$ | $F_0 = E(S_T)$ |
| Positive systematic risk      | $k > r$      | $F_0 < E(S_T)$  |
| Negative systematic risk | $k < r$      |  $F_0 > E(S_T)$ |

