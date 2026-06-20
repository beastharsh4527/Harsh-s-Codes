# Credit Card Fraud Detection

Detecting fraudulent transactions in a real, highly imbalanced dataset of 284,807 transactions, where only 0.17% were fraud.

## What I did
- Explored the data and found most fraud is very small in value (likely card-testing)
- Ran a statistical t-test: fraud transactions have a significantly higher average amount (p = 0.0036)
- Built a logistic regression model to predict fraud
- Handled the class imbalance using class weighting
- Tuned the decision threshold to balance catching fraud against false alarms

## Key results
- Baseline model: caught 61% of fraud, 86% precision, 15 false alarms
- Balanced model: caught 87% of fraud, but only 6% precision and 1,888 false alarms
- Balanced model with a tuned threshold: caught 80% of fraud, 63% precision, just 71 false alarms

## Takeaway
The hardest part of fraud detection isn't building the model, it's choosing where to sit on the precision/recall tradeoff. 
Tuning the decision threshold found a practical operating point that catches most fraud without overwhelming investigators.
