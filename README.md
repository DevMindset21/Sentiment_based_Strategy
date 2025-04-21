**Objective**

In the trading strategy, we buy and sell stock as per the current stock sentiments :
1. Buy a stock when the change in sentiment score (Current sentiment score - previous sentiment score) is greater than .5
2. sell a stock when the change in sentiment score is less than -.5.

Additionally, we check for 15 days moving average while buying and selling and buy or sell in a unit of 100.
Obviusly, there can be many ways to create the trading strategy based in sentiments, by varying the threshold, or changing the number of units based on the initial cash available.

We use lexicon based sentiments for the trading strategy.
