# credit-risk-classification
In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.


Credit Risk Analysis Report

Overview of the Analysis:

Credit Risk pertains to the risk that a borrower may default on a loan, leading to potential financial losses for the lender. In this comprehensive analysis, we leveraged Machine Learning to delve into the dataset of past lending activities from a peer-to-peer lending services company. Our primary objective was to construct a model adept at discerning the creditworthiness of borrowers, and to this end, we employed various techniques. Our approach was methodical: We initially partitioned the data into training and testing sets, formulated a logistic regression model from the original data, and subsequently refined this model by integrating resampled training data. The culmination of these efforts is this credit risk analysis report.

Our endeavor was to classify loans as either healthy or high-risk, based on the loan status indicators provided by the lending institution.

Key Results:

The model trained on the Imbalanced data rendered an accuracy of 95%. This performance can be enhanced, given the imbalanced nature of the data.

In contrast, the OverSampled data model outperformed with an accuracy of 99%. This showcases that the OverSampled model is more reliable for analyzing the data in this specific context.

Precision metrics are as follows:

Imbalanced Model: 100% precision for healthy loans and 85% for high-risk loans.
OverSampled Model: 100% precision for healthy loans and 84% for high-risk loans.
Summary and Recommendations:

For a lending company, a pivotal model is one that can consistently and accurately categorize loans as either healthy or high-risk.

Upon comparison, the Logistic Regression model trained on OverSampled data, with its 99% accuracy, outshines the Imbalanced data model which has an accuracy of 95%. The implication here is that the former model, Logistic Regression Model 2, is less prone to false negatives. Yet, based on the confusion matrices of both models, it's noteworthy that Model 2 does indicate a higher rate of false positives, i.e., predicting loans as healthy when they were, in fact, high-risk.

In sum, given its superior overall accuracy, Logistic Regression Model 2 emerges as the recommended choice, despite its slight inclination towards more false positives. The benefits of reduced false negatives, combined with its heightened accuracy, make it the more desirable model for evaluating creditworthiness in this dataset.