# btc-price-prediction-sentiment-analysis

Bitcoin is a digital currency that is getting popular day by day. Bitcoin has been an area
of interest for investors, analysts, and researchers due to its volatile nature and high return
possibility. In the prices of cryptocurrencies such as Bitcoin, significant fluctuations and
inherent risks can be faced. For this reason, predicting Bitcoin price fluctuations is becoming
important for individuals and organizations. Some methods can generate investment ideas
by predicting the movement of Bitcoin prices in the future. One of the methods that can help
in predicting Bitcoin prices is sentiment analysis. Sentiment analysis can be applied in many
areas such as customer service, finance, and marketing. It is also used in the cryptocurrency
industry to get ideas. Sentiment analysis can help predict the market trend of Bitcoin prices.
Therefore, in this project, a prediction model is made using sentiment analysis of how Bitcoin
prices will change tomorrow compared to today.

In this study, two models are built that aim to predict the change in Bitcoin prices for the
next day. Bitcoin-related news data is collected and sentiment analysis is applied. Afterward,
the sentiment classification and prediction models are built. For sentiment analysis, the news
titles are scored using VADER, and the BERT model is trained with the scored data. For
prediction, two different models were trained, one with news headline sentiment and Bitcoin
prices, and the other with news headline sentiment, Bitcoin prices, and financial metrics.
Thus, while the news headline is given in the first model, the news headline and required
financial metrics are given in the second model. Logistic Regression, Random Forest, and
SVM algorithms were applied and compared in both prediction models. In the first prediction
model, the SVM model gives the best results. In the second prediction model, the Random
Forest model gives the best performance.
