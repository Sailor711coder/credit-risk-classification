# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to build and evaluate a machine learning model capable of predicting whether a loan is high-risk or healthy. The dataset contained financial and categorical information about individual borrowers. Our target was the `loan_status` column, where:

- `0` indicates a healthy loan
- `1` indicates a high-risk loan

We followed the standard machine learning pipeline:
- Loaded and explored the data
- Split the dataset into features (`X`) and labels (`y`)
- Applied a train/test split
- Trained a `LogisticRegression` model
- Evaluated the model using accuracy, precision, and recall metrics

## Results

* **Logistic Regression Model**:
  - **Accuracy**: 0.99
  - **Precision**:
    - Class 0 (healthy): 1.00
    - Class 1 (high-risk): 0.84
  - **Recall**:
    - Class 0 (healthy): 0.99
    - Class 1 (high-risk): 0.94

## Summary

The logistic regression model is highly accurate and performs well at identifying both classes. The precision and recall for high-risk loans are particularly important, and this model showed strong results in both:

- It successfully identifies **94% of actual high-risk loans** (recall)
- When it predicts a loan as high-risk, it's correct **84% of the time** (precision)

Given its strong performance and minimal misclassification of risky loans, we recommend this model as a useful tool for credit risk evaluation.
