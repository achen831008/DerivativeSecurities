# Chapter 9 - Mechanics of Options Markets

Types of Options
================

**Call** Option - gives the holder of the option the right to **buy** an asset by a certain date for a certain price.

**Put** Option - gives the holder the right to **sell** an asset by a certain date for a certain price.

The date specified in the contract is known as the **expiration** date. The price specified in the contract is known as the **exercise** price or the **strike** price.

**American** Options can be exercised at any time up to the expiration date.

**European** Options can be exercised only on the expiration date itself.

**Note**: Buyer pays seller (writer) fees.

Payoffs
=======

**European call option**

Long position: $max(S_T - K, 0)$

Short position: $min(K - S_T, 0)$

**European put option**

Long position: $max(K - S_T, 0)$

Short position: $min(S_T - K, 0)$

**Upper bound**

$C = S_T$

$P = Ke^{-rT}$ for European option

$P = K$ for American option

**Lower bound**

$C = S_T - Ke^{-rT} - PV(Div)$

$P = Ke^{-rT} - S_T + PV(Div)$

**Factors that would affect Option Value**

An increase in the following list of factor would change the value of option.

|Factors|   C   |   P   |
|-------|-------|-------|
|   K   |  Down |   Up  |
|   S   |   Up  |  Down |
|   T   |   Up  |   Up  |
|   r   |   Up  |  Down |
|  Div  |  Down |   Up  |
|  Vol  |   Up  |   Up  |


Dividends and Stock Splits
==========================

In general,  an n-for-m stock split cause the strike price reduced to m/n of its previous value, and the number of shares covered by one contract is increased to n/m of its previous value.

**Stock Splits Example**
Consider a call option to buy 100 shares of a company for \$30 per share. Suppose the company makes a 2-for-1 stock split. The terms of the option contract are then
changed so that it gives the holder the right to purchase 200 shares for \$15 per share.

**Dividends Example**
Consider a put option to sell 100 shares of a company for \$15 per share. Suppose the company declares a 25\% stock dividend. This is equivalent to a 5-for-4 stock split. The terms of the option contract are changed so that it gives the holder the right to sell 125 shares for $12.

Warrants, Employee Stock Options, and Convertibles
==================================================

**Warrants** are options issued by a financial institution or non-financial corporation. A common use of warrants by a non-financial corporation is at the time of a bond issue. The corporation issues call warrants on its own stock and then attaches them to the bond issue to make it more attractive to investors.

**Note:** warrants give the holder the option to buy shares at certain price.

**Employee stock options** are call options issued to employees by their company to motivate them to act in the best interests of the company's shareholders. They are usually at the money at the time of issue.

Convertible bonds are bonds issued by a company that can be converted into equity at certain times using a predetermined exchange ratio. They are therefore bonds with an embedded call option on the company's stock.













