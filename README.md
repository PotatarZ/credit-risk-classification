# Analysis
## Overview

Data has been provided for around 80 thousand loans that have been labeled as healthy or high-risk.  I was tasked with creating a machine learning model that can accurately predict the status of a loan, given various features such as loan size, income, total debt, et cetera.  I started by spliting the data into training and testing groups.  The training group was used to create a logistic regression model, and that model was tested with the testing group.  I also created another model by using an over sampler on the training data and re-testing it.

## Results
Both models show a 100% accurate prediction of healthy loans. The high-risk classifications differ slightly:
* Regression Model 1:
  * F1:  88% high-risk, 94% overall
  * Precision:  87% high-risk, 94% overall
  * Recall:  89% high-risk, 94% overall
* Regression Model 2 (Over Sampled):
  * F1:  93% high-risk, 96% overall
  * Precision:  87% high-risk, 94% overall
  * Recall:  100% high-risk, 100% overall

## Summary
Both models perform extremely well.  I would recommend the second model, as it has a 99% overall accuracy rating.  Both models avoid flagging innocent accounts, which is extremely important.  The scores being so high would normally set off a red flag for me.  However, I realize that this dataset may be fictitious.
