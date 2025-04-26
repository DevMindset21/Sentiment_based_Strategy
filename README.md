## Problem Statement
Building a trading strategy that uses NLP to extracts the information inside the news headlines, assigns a sentiment to that and use the sentiments and the information inside the news headlines for a trading strategy.

## Dataset
1. News headlines data compiled from RSS feeds of several news websites: This news headlines data is complied by different news website and contains the most financially relevant news filtered. 
2. Yahoo finance website for the stock return: (The return data can be obtained from other website such as yahoo finance)
3. Kaggle: labelled data of of news sentiments obtained for a classification based sentiment analysis model. This data may not be authentic and is used only for demonstration purpose in this case study.
4. Stock market lexicon created based on stock market conversations in microblogging services.

## Logic

In the trading strategy, we buy and sell stock as per the current stock sentiments :
1. Buy a stock when the change in sentiment score (Current sentiment score - previous sentiment score) is greater than .5
2. sell a stock when the change in sentiment score is less than -.5.

Additionally, we check for 15 days moving average while buying and selling and buy or sell in a unit of 100.

We use lexicon based sentiments for the trading strategy.
