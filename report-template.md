# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The primary purpose of this analysis was to evaluate the creditworthiness of potential borrowers using machine learning models. We aimed to classify borrowers into one of two categories: those likely to repay their loans on time (healthy loans) and those at a high risk of defaulting (high-risk loans).
The primary purpose of this analysis was to evaluate the creditworthiness of potential borrowers using machine learning models. We aimed to classify borrowers into one of two categories: those likely to repay their loans on time (healthy loans) and those at a high risk of defaulting (high-risk loans).

**Data Insight:**
The dataset, derived from a peer-to-peer lending company, consisted of historical lending data including personal financial metrics and loan outcomes. Our primary task was to predict the `loan_status` column, which categorizes loans as either "healthy" or "high-risk".

`value_counts` of `loan_status`: 
* Healthy Loans: XX,XXX (or X%)
* High-Risk Loans: X,XXX (or X%)

**Machine Learning Process:**
1. Data Cleaning: Removed any null values and outliers.
2. Data Splitting: Partitioned the data into training and testing sets.
3. Model Creation: Employed a logistic regression model (`LogisticRegression`) due to its efficacy with binary outcomes.
4. Resampling: To address the imbalanced nature of the dataset, resampling methods like oversampling were implemented.
5. Model Evaluation: Assessed the performance of models using metrics such as accuracy, precision, and recall.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * Accuracy: 95% 
  * Precision: 
    * Healthy Loans: 100%
    * High-Risk Loans: 85%
  * Recall: 
    * Healthy Loans: XX%
    * High-Risk Loans: XX%


* Machine Learning Model 2:
  * Accuracy: 99%
  * Precision:
    * Healthy Loans: 100%
    * High-Risk Loans: 84%
  * Recall: 
    * Healthy Loans: XX%
    * High-Risk Loans: XX%

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


Upon a thorough comparison of the two models:

* **Model Performance:**
  * Model 2 (OverSampled Data Model) with an accuracy of 99% outperformed Model 1 (Imbalanced Data Model) which achieved a 95% accuracy.
  * While both models demonstrated impeccable precision in predicting healthy loans, Model 1 slightly edged out Model 2 in predicting high-risk loans by 1%.

* **Best Model:**
  * Although Model 1 has a marginally higher precision for high-risk loans, Model 2's overall higher accuracy and robustness, especially in an oversampled context, make it the preferred choice.

* **Problem Context:**
  * Performance does hinge on our objective. If our prime focus is to minimize the risk of default (i.e., predicting `1`'s or high-risk loans more accurately), Model 1's superior precision for high-risk loans might be more appealing. However, if overall accuracy and balance between the two categories are sought, Model 2 emerges as the winner.

**Recommendation:** 
I would advocate for the implementation of Model 2 (OverSampled Data Model). Its superior accuracy ensures a well-rounded prediction for both healthy and high-risk loans. The marginal 1% compromise on high-risk loan precision seems justified for the comprehensive benefits the model offers.
