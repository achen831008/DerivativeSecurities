# Chapter 7 - Swaps

Mechanics of Interest Rate Swaps
================================

LIBOR
-----
The floating rate in most interest rate swap agreements is the London Interbank Offered Rate.

Usage of Swaps
--------------

 1. Transform a Liability
 2. Transform an Asset

Day Count Issues
----------------
6-month LIBOR is quoted on an actual/360 basis.
Fixed rate is usually quoted as actual/365 or 30/360.
> In general, a LIBOR-based floating-rate cash flow on a swap payment date is calculated as LRn/360, where L is the principal, R is the relevant LIBOR rate, and n is the number of days since the last payment date.

 To make approximately comparable, either the 6-month LIBOR rate must be multiplied by 365/360 or the fixed rate must be multiplied by 360/365

Valuation of Interest Rate Swaps
--------------------------------

**Valuation in Terms of Bond Prices**

$V_{swap} = B_{fix} - B_{fl}$

**Example**

> Suppose that a financial institution has agreed to pay 6-month LIBOR and receive 8% per annum on a notional principal of 100 million. The swap has a remaining life of  1.25 years. The LIBOR rates with continuous compounding for 3-month, 9-month, and 15-month maturities are 10%, 10.5%, and 11% respectively. The 6-month LIBOR rate at the last payment date was 10.2%.

The discount factors for these cash flows are $e^{-0.1*0.25}$, $e^{-0.105*0.25}$, $e^{-0.11*0.25}$ respectively.

|Time |$B_{fix}$ cash flow|$B_{fl}$ cash flow|Discount factor|PV($B_{fix}$)|PV($B_{fl}$)|
|-----|-----|-----|------|------|-------|
|0.25 |  4.0|105.1|0.9753| 3.901|102.505|
|0.75 |  4.0|     |0.9243| 3.697|       |
|1.25 |104.0|     |0.8715|90.640|       |
|Total|     |     |      |98.238|102.505|

$V_{swap}$ = 98.238 - 102.505 = -4.267

Currency Swap
=============

Types of currency swaps:

1. fix-for-fix
2. fix-for-floating
3. floating-for-floating

Valuation of Currency Swaps
---------------------------

**Valuation in Terms of Bond Prices**

$V_{swap} = B_D - S_0 B_F$
where $B_F$ is the value, measured in the foreign currency, of the bond defined by the foreign cash flows on the swap and $B_D$ is the value of the bond defined by the domestic cash flows on the swap, and $S_0$ is the spot exchange rate.

**Example**
Suppose that the term structure of LIBOR/swap interest rates is flat in both Japan and the United States. The Japanese rate is 4% per annum and the US rate is 9% per annum (both with continuous compounding). Some time ago a financial institution has entered into a currency swap in which it receives 5% per annum in yen and pays 8% per annum in dollars once a year. The principals in the two currencies are \$10 million and 1,200 million yen. The swap will last for another 3 years, and the current exchange rate is 110 yen ¼ = \$1.

|Time |Cash flows on dollar bond|PV|Cash flows on yen bond|PV|
|-----|----|------|----|-------|
|    1| 0.8|0.7311|  60|  57.65|
|    2| 0.8|0.6682|  60|  55.39|
|    3| 0.8|0.6107|  60|  53.22|
|    3|10.0|7.6338|1200|1064.30|
|Total|    |9.6439|    |1230.55|

Value = 1230.55/110 - 9.6439 = 1.5430 million

