# credit-risk-classification

## Code Sources
No additional code sources were used in this challenge.

# Report 

## Overview of the Analysis

The purpose of this analysis is to find which machine learning model can best predict which loans are high-risk versus those that are healthy. To do this, we used our data's features, such as the loan amount, interest rate, debt amount, and number of accounts, to test how these affected the loan's status as either healthy or high-risk. After splitting the data into training and testing sets, we created three different machine learning models--logistic regression, decision tree, and random forest--, fit the training data to each model, and made predictions of how each model would classify the testing data. We then got scores for accuracy, precision, and recall for each model to see which performed the best.


## Results

* Logistic Regression:
    * Accuracy: 99.2%
        * This model correctly predicted which loans were healthy versus high-risk about 99% of the time.
    * Precision: 84.7%
        * Of all the high-risk loans this model labelled, about 85& of them were actually high-risk.
    * Recall: 91.0%
        * Of all the actual high-risk loans, this model labelled 91% of them as high-risk.
* Decision Tree:
    * Accuracy: 99.0%
        * This model correctly predicted which loans were healthy versus high-risk about 99% of the time.
    * Precision: 84.3%
        * Of all the high-risk loans this model labelled, about 84& of them were actually high-risk.
    * Recall: 85.3%
        * Of all the actual high-risk loans, this model labelled about 85% of them as high-risk.
* Random Forest:
    * Accuracy: 99.2%
        * This model correctly predicted which loans were healthy versus high-risk about 99% of the time.
    * Precision: 84.8%
        * Of all the high-risk loans this model labelled, about 85& of them were actually high-risk.
    * Recall: 90.0%
        * Of all the actual high-risk loans, this model labelled 90% of them as high-risk.

## Summary

Overall, all three machine learning models produced very similar results. All three had nearly identical accuracy scores--about 99%, as well as nearly identical precision scores--about 85%. This means that all three models are incredibly good at correctly labelling healthy versus high-risk loans, but have lower scores in classifying a loan as high-risk versus it being a false positive. Their main point of difference is their recall scores. While all close, the logtistic regression model had the highest score, meaning it labelled actual high-risk loans as high-risk the most often. This is extra important since for this data, false-negatives are the most crucial to minimize to avoid incorrectly labelling a high-risk label as healthy. It is for this reason that we would recommend using the logistic regression model.