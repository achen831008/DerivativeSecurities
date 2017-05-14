# Chapter 2 - Mechanics of Futures Markets

> A trader who agreed to buy has a **long futures position** in one contract

> A trader who agreed to sell has a **short futures position** in one contract

> The price agreed to is the current **futures price**

Closing Out Positions
=====================

Most of the traders choose to close out their positions prior to the delivery period specified in the contract. Closing out a position means entering into the **opposite trade to the original one**.

For example, the New York investor who bought a July corn futures contract on March 5 can close out the position by selling (i.e., shorting) one July corn futures contract on, say, April 20. The Kansas investor who sold (i.e., shorted) a July contract on March 5 can close out the position by buying one July contract on, say, May 25. In each case, the investor’s total gain or loss is determined by the change in the futures price between March 5 and the day when the contract is closed out.

Specification of a Futures Contract
===================================

The exchange must specify:

 - Asset
 - Contract size
 - Delivery arrangements
 - Delivery months
 - Price quotes
 - Price limits and position limits

As a general rule, it is the party with the *short position* that chooses what will happen when alternatives are specified by the exchange. When the party with the *short position* is ready to deliver, it files a *notice of intention to deliver* with the exchange.

Convergence of Futures Price to Spot Price
==========================================

As the delivery period for a futures contract is approached, the futures price converges to the spot price of the underlying asset. When the delivery period is reached, the futures price equals, or is very close to, the spot price.

To see why this is so, we first suppose that the futures price is above the spot price during the delivery period. Traders then have a clear arbitrage opportunity:
1. Sell (i.e., short) a futures contract 
2. Buy the asset
3. Make delivery.
These steps are certain to lead to a profit equal to the amount by which the futures price exceeds the spot price. As traders exploit this arbitrage opportunity, the futures price will fall. 

The Operation of Margins
========================

Daily Settlement
----------------
In general, the broker will require the investor to deposit funds in a margin account. The amount that must be deposited at the time the contract is entered into is known as the **initial margin**.

At the end of each trading day, the margin account is adjusted to reflect the investor's gain or loss. This practice is referred to as **daily settlement** or **marking to market**.

For example, by the end of the first day, the futures price has dropped by \$9 from \$1,250 to \$1,241. (2 contracts, each contract size is 100 ounces) The investor has a loss of \$1,800 (= 200 x \$9), because the 200 ounces of December gold, which the investor contracted to buy at \$1,250, can now be sold for only \$1,241.

**Note:** The balance in the margin account would therefore be reduced by \$1,800 to \$10,200.

To ensure that the balance in the margin account never becomes negative a **maintenance margin**, which is somewhat **lower** than the initial margin, is set. If the balance in the margin account falls **below** the maintenance margin, the investor receives a **margin call** and is expected to top up the margin account to the **initial margin level** by the end of the next day. The extra funds deposited are known as a **variation margin**. 

The Clearing House and Clearing Margins
---------------------------------------

> A **clearing house** acts as an intermediary in futures transactions. It guarantees the performance of the parties to each transaction. The main task of the clearing house is to keep track of all the transactions that take place during a day, so that it can calculate the net position of each of its members.

Market Quotes
========================
Futures quotes are available from exchanges and from several online sources (see, for example, futures.tradingcharts.com/marketquotes).

Prices
------
 - Opening price
 - Highest Price achieved in trading during the day
 - Lowest price achieved in trading during the day

Settlement Price
----------------
This is the price used for calculating daily gains and losses and margin requirements. It is usually calculated as the price at which the contract traded immediately before the end of a day’s trading session (1:30 p.m. for gold).

The Change in the Settlement price is the delta of today's and previous day's settlement price.

Trading Volume and Open Interest
--------------------------------
The **trading volume** is the number of contracts *traded*.
The **open interest** is the number of contracts *outstanding*, that is, the number of long positions, or the number of short positions.

Patterns of Futures Prices
--------------------------
Markets where the futures price is an **increasing** function of the time to maturity are known as **normal markets**. Markets where the futures price **decreases** with the maturity of the futures contract are known as **inverted markets**.

Delivery
========
The decision on **when to deliver** is made by the party with the **short position**, whom we shall refer to as investor A. When investor A decides to deliver, investor A’s broker issues a **notice of intention to deliver** to the exchange clearing house. This notice states how many contracts will be delivered. The exchange then chooses a party with a long position to accept delivery.

Forward vs. Futures Contracts
=============================

**Comparison of forward and futures contracts:**

| Forwards                             | Futures                        |
|--------------------------------------|--------------------------------|
| Private contract between two parties | Traded on an exchange          |
| Not standardized                     | Standardized contract          |
| Usually one specified delivery date  | Range of delivery dates        |
| Settled at end of contract           | Settled daily                  |
| Delivery or final cash settlement    | Contract is usually closed out |
| Usually takes place                  | prior to maturity              |
| Some credit risk                     | Virtually no credit risk       |


Foreign Exchange Quotes
-----------------------

> **Futures prices** where one currency is the USD are always quoted as **the number of USD per unit of the foreign currency**.

> **Forward prices** are always quoted in the same way as spot prices. For `the British pound`, `the euro`, `the Australian dollar`, and `the New Zealand dollar`, the forward quotes show **the number of US dollars per unit of the foreign currency** and are directly comparable with futures quotes. For `other major currencies`, forward quotes show **the number of units of the foreign currency per US dollar** (USD). 

For example, consider the Canadian dollar (CAD). A futures price quote of 0.9500 USD per CAD corresponds to a forward price quote of 1.0526 CAD per USD (1.0526 = 1/0.9500).

