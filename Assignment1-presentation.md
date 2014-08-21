How long will your savings last in retirement?
========================================================
author: Brian Greiner
date:  August 20, 2014

INTRODUCTION
========================================================

- When discussing retirement, the big question is "how much can I afford to spend each month without outliving my savings?".
- This program will help to answer this question, taking into account inflation and 
expected rates of return on investment.


```r
# ignoring inflation or rate of return 
initialSavings <- 1000000
timeFrameMonths <- 30 * 12
monthlyWithdrawal <- 3000
amountRemaining <- initialSavings - (timeFrameMonths * monthlyWithdrawal)
amountRemaining
```

```
[1] -80000
```

PROGRAM INPUT
========================================================

The following information is required :
- the amount of savings (in dollars)
- the amount of money to be withdrawn each month (in dollars)
- the yearly rate of return on the savings (in %)
- the yearly rate of inflation (in %)
- the time frame of the calculation (in years) [that is, how long do you expect to live after retirement]

PROGRAM OUTPUT
========================================================
The program calculates :
- a graph of how much of the savings remains for each month of retirement
- the amount left in savings at the end of the assigned time frame

DISCUSSION
========================================================
- the program does not take into account any other sources of income, such as pensions
- the amount of savings is re-calculated each month, taking into account the effects of rate of return and inflation
- it is assumed that the rate of return and rate of inflation will remain constant over the time frame
