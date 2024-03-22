The dataset I use here was taken from Kaggle. It contains tweets for a basket of stocks from 2021 to 2022.

Steps I took:
1. Classified sentiment using NLTK.
2. Train-test period of 125 days and 250 days respectively.
3. Training period used to set thresholds on positive and negative sentiment scores. Values on the upper quartile were considered as target values for sentiment.
4. Strategy was to buy if positive sentiment threshold is consistently over for 2 days in a row, sell if negative threshold crossed for 2 days in a row.
5. 1 day holding period, 5 units of stock purchased at a signal, shorting constraint considered.
