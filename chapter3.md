# Chapter 3 - Hedging Strategies Using Futures

> A **perfect hedge** is one that completely eliminates the risk.

Basic Principles
================

When an individual or company chooses to use futures markets to hedge a risk, the objective is usually to take a position that **neutralizes the risk** as far as possible.

> A short hedge is a hedge that involves a short position in futures contracts. 

> A long hedge is a hedge that involves a long position in futures contracts.


Basis Risk
==========

Uncertainty of Hedging:

 1. The asset whose price is to be hedged may not be exactly the same as the asset underlying the futures contract.
 2. The hedger may be uncertain as to the exact date when the asset will be bought
or sold.
 3. The hedge may require the futures contract to be closed out before its delivery month. 

These problems give rise to what is termed **basis risk**.

The Basis
---------

    Basis = Spot price of asset to be hedged - Futures price of contract used

To examine the nature of basis risk, we will use the following notation:

 - S1: Spot price at time t1
 - S2: Spot price at time t2
 - F1: Futures price at time t1
 - F2: Futures price at time t2
 - b1: Basis at time t1
 - b2: Basis at time t2

From the definition of the basis, we have

    b1 = S1 - F1 and b2 = S2 - F2

**Note:** basis risk can lead to an improvement or a worsening of a hedger’s position. 

Consider a **short** hedge. If the basis **strengthens** (i.e., increases) unexpectedly, the hedger’s position **improves**; if the basis **weakens** (i.e., decreases) unexpectedly, the hedger’s position **worsens**.

By hedging, a company ensures that the price that will be paid (or received) for the asset is

    S2 + F1 - F2

Choice of Contract
------------------
One key factor affecting basis risk is the choice of the futures contract to be used for hedging. This choice has two components:
1. The choice of the **asset underlying** the futures contract 
2. The choice of the **delivery month**.

In general, basis risk **increases** as the time difference between the hedge expiration and the delivery month **increases**. A good rule of thumb is therefore to choose a delivery month that is **as close as possible** to, but **later** than, the **expiration of the hedge**.


Cross Hedging
=============

**Cross hedging** occurs when the asset underlying the futures contract is **different** from the asset whose price is being hedged.

**Hedge Ratio** is the ratio of the size of the position taken in futures contracts to the size of the exposure.

Calculating the Minimum Variance Hedge Ratio
--------------------------------------------
The minimum variance hedge ratio depends on the relationship between changes in the spot price and changes in the futures price. Define:

 - $\delta$S: Change in spot price, S, during a period of time equal to the life of the hedge
 - $\delta$F: Change in futures price, F, during a period of time equal to the life of the hedge.

We will denote the minimum variance hedge ratio by h*.
The formula for h* is:

> $h^* = p \times \frac {\sigma_S}{\sigma_F} $

where $\sigma_S$ is the standard deviation of $\delta$S, $\sigma_F$ is the standard deviation of $\delta$F, and p is the coefficient of correlation between the two.

Optimal Number of Contracts
---------------------------
To calculate the number of contracts that should be used in hedging, define:

 - $Q_A$: Size of position being hedged (units)
 - $Q_F$: Size of one futures contract (units)
 - N*: Optimal number of futures contracts for hedging.

The futures contracts should be on h*$Q_A$ units of the asset. The number of futures contracts required is therefore given by

> $N^* = \frac{h^* Q_A}{Q_F}$

Tailing the Hedge
-----------------
When futures are used for hedging, a small adjustment, know as **tailing the hedge**, can be made to allow for the impact of daily settlement. In practice this means that:

> $N^* = \frac {h^* V_A}{V_F}$

where $V_A$ is the dollar value of the position being hedged and $V_F$ is the dollar value of one futures contract.

The effect of tailing the hedge is to multiply the hedge ratio by the ratio of the spot price to the futures price.

Stock Index Futures
===================

> A **stock index** tracks changes in the value of a hypothetical portfolio of stocks.

Stock Indices
-------------

The **Dow Jones Industrial Average** is based on a portfolio consisting of 30 blue-chip stocks in the United States. The weights given to the stocks are proportional to their prices.

The **Standard & Poor’s 500** (S&P 500) Index is based on a portfolio of 500 different stocks: 400 industrials, 40 utilities, 20 transportation companies, and 40 financial institutions. The weights of the stocks in the portfolio at any given time are proportional to their market capitalizations.

The **Russell 1000 Index** is an index of the prices of the 1,000 largest capitalization stocks in the United States. The US Dollar Index is a trade-weighted index of the values of six foreign currencies (the euro, yen, pound, Canadian dollar, Swedish krona, and Swiss franc).

Hedging an Equity Portfolio
---------------------------
**Stock index futures** can be used to hedge a well-diversified equity portfolio. Define: 

 - $V_A$: Current value of the portfolio
 - $V_F$: Current value of one futures contract (the futures price times the contract size). 

If the portfolio mirrors the index, the optimal hedge ratio, $h^*$, equals 1.0 and shows that the number of futures contracts that should be shorted is

> $N^* = \frac {V_A}{V_F}$

When the portfolio does not exactly mirror the index, we can use the **capital asset pricing model**. The parameter beta ($\beta$) from the capital asset pricing model is the **slope** of the best-fit line obtained when excess return on the portfolio over the risk-free rate is regressed against the excess return of the index over the risk-free rate.

In general,

> $N^* = \beta \frac {V_A}{V_F}$

This formula assumes that the maturity of the futures contract is close to the maturity of the hedge.


Stack and Roll
--------------
Sometimes the expiration date of the hedge is **later than** the delivery dates of all the futures contracts that can be used. The hedger must then **roll** the hedge forward by **closing out** one futures contract and taking the same position in a futures contract with a later delivery date. Hedges can be rolled forward many times. The procedure is known as **stack and roll**. 
