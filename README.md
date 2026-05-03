# ISOM835-Amazon-Profitability
Amazon Order Profitability Prediction — ISOM 835
# Amazon Order Profitability Prediction
ISOM 835 — Predictive Analytics and Machine Learning  
Suffolk University | Sawyer Business School

## Project Summary
This project predicts whether an Amazon sales order will be 
profitable or result in a loss using machine learning classification.  
Dataset: Amazonsale_dataset.xlsx — 3,203 orders, Western US, 2011–2015

## Business Problem
Not every Amazon sale is profitable. Heavy discounts and low-margin 
categories erode profits. This model identifies loss-generating orders 
before fulfillment to enable smarter pricing decisions.

## Dataset
| Attribute | Value |
|---|---|
| File | Amazonsale_dataset.xlsx |
| Records | 3,203 orders |
| Features | 16 |
| Date Range | 2011 – 2015 |
| States | 11 (Western US) |
| Target | Profitable (1) / Loss (0) |
| Class Balance | 89.4% Profitable / 10.6% Loss |
| Missing Values | None |

## Google Colab Notebook
[Open Notebook Here](https://colab.research.google.com/drive/1GYIe2Bjb7vOEAFlRhVVi1hQO0Q7SUnQl#scrollTo=M7KfkXFQjLxX)

## Models & Results
| Model | Accuracy | F1-Score | ROC-AUC |
|---|---|---|---|
| Logistic Regression | 89.39% | 0.9440 | 0.537 |
| Random Forest | 90.48% | 0.9493 | 0.878 |
| **Gradient Boosting** | **91.73%** | **0.9550** | **0.923** |

Best Model: Gradient Boosting — Accuracy 91.7%, AUC 0.923

## Key Findings
- Tables (42.2%), Bookcases (40%), Chairs (36.2%) = highest loss rates
- Paper, Art, Appliances, Envelopes = 0% loss rate over 4+ years
- Product Category is the #1 predictor of profitability (25.2%)
- Sales Amount is the #2 predictor (22.7%)

## Tools & Libraries
Python 3, Google Colab, pandas, numpy, scikit-learn, matplotlib, seaborn
