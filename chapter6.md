# Chapter 6 - Interest Rate Futures

Day Count and Quotation Conventions
===================================

Day Count Conventions:

 1. Actual/actual (in period)
 2. 30/360
 3. Actual/360

Price Quotations of US Treasury Bills
-------------------------------------

$P = \frac{360}{n} * (100 -Y)$

where P is quoted price, Y is cash price, and n is the remaining life of the Treasury bill.

Price Quotations of US Treasury Bonds
-------------------------------------

> Treasury bond prices in US are quoted in dollars and thirty-seconds of a dollar. The quoted price is for a bond with a face value of \$100. Thus a quote of 90-05 indicates that the quoted price for a bond with a face value of \$100,000 is \$90,156.25.

> Quoted price is referred to as the clean price
> Cash price is referred to as the dirty price

Cash price = Quoted price + Accrued interest since last coupon date

**Example**
Today: March 5, 2010
Coupon: 11% annually, paid semiannually
Maturity: July 10, 2018
Quote: 95-16 or $95.50
Last Coupon Date: January 10, 2010
Days Since: 21+28+5 = 54
Total Days: 21+28+31+30+31+30+10 = 181

Accrued Interest = 54/181 * 11%/2 * 100 = $1.64
Cash Price = 95.5 + 1.64 = 97.14

Treasury Bond Futures
=====================

Quotes
------

Treasury bond and Treasury note futures contracts are quoted in dollars and thirty-seconds of a dollar per $100 face value.

Conversion Factors
------------------

> When a particular bond is delivered, a parameter known as its **conversion factor** defines the price received for the bond by the party with the short position.
> The cash received for each $100 face value of the bond delivered is (most recent settlement price * Conversion factor) + Accrued interest

Cheapest-to-Deliver Bond
------------------------

> The cheapest-to-deliver bond is the one for which
`Quoted bond price - (Most recent settlement price * Conversion Factor)`
is least.

Determining the Futures Price
-----------------------------

$F_0 = (S_0 - I){e}^{rT}$

where I is the present value of the coupons during the life of the futures contract, T is the time until the futures contract matures, and r is the risk-free interest rate applicable to a time period of length T

**Example**
Cheapest-to-deliver bond: 12% coupon bond with Conversion Factor of 1.6000
Delivery: in 270 days
Coupons: paid semiannually
Last coupon date: 60 days ago
Next coupon date: 122 days
Coupon date thereafter is in 305 days
Term structure: flat
Interest rate: 10% annually
Quote: \$115
Cash price: 115 + 60/(60+122) * 12% / 2 * 100 = 116.978

A coupon of \$6 will be received after 122 days (= 0.3342 years). The present value of this is
$6{e}^{-0.1*0.3342} = 5.803$

The futures contract lasts for 270 days. The cash futures price, if the contract were written on the 12% bond, would be
$(116.978 - 5.803){e}^{0.1*0.7397} = 119.711$

At delivery, there are 148 days of accrued interest. The quoted futures price is
$119.711 - 6 * \frac{148}{148+35} = 114.859$

The quoted futures price should be
$\frac{114.859}{1.6000} = 71.79$

EuroDollar Futures
==================

> Eurodollar is a dollar deposited in a U.S. or foreign bank outside the U.S.
> Eurodollar interest rate is the rate of interest earned on Eurodollars deposited by one bank with another bank.
> Settlement price is set equal to 100 - R, where R is the actual three-month Eurodollar interest rate.
> One basis point change in the futures quote corresponds to a 0.01% change in the futures interest rate.

Contract price is $10,000 * [100 - 0.25 * (100 - Q)]$

Duration-Based Hedging Strategies Using Futures
==================

Number of contracts required to hedge against a uncertain change in yield, therefore, is 

$N^* = \frac{P D_P}{V_F D_F}$

This is the duration-based hedge ratio (price sensitivity hedge ratio).



