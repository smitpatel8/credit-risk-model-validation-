
## Overview of the Analysis

* Explain the purpose of the analysis.

We will use machine learning in this analysis to examine a dataset containing historical lending activity data from a peer-to-peer lending services company. The goal is to create a model capable of assessing the creditworthiness of borrowers.

* Explain what financial information the data was on and what you needed to predict.

Employing a machine learning approach, we aim to classify loans as either low-risk (healthy) or high-risk (non-healthy) based on the loan status provided by the lending company. The Logistic Regression Algorithm is chosen as the most suitable tool for our machine learning model, as it is commonly utilized to predict the probability of a target variable in classification tasks.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

Using the dataset provided by the lending company, I constructed a logistic regression model that achieved an accuracy score of 95%. Despite the model's high overall accuracy, it exhibits a lower recall value (0.91) for non-healthy loans compared to the recall value (0.99) for healthy loans. This suggests that the model excels at classifying loans as healthy but may have some challenges in correctly identifying non-healthy loans. This imbalance in performance can be attributed to the dataset's inherent class imbalance, where healthy loans significantly outnumber non-healthy loans.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall Scores

According to the model recall scores, the model made 1% of mistakes when predicting healthy loans and 9% of mistakes when predicting non-healthy loans.
The model generated an accuracy score of 95% but could be improved due to the dataset being imbalanced.

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall Scores

According to the model recall scores, the model made 1% of mistakes when predicting healthy loans and 1% of mistakes when predicting non-healthy loans. 
The model generated an accuracy score of 99% due to the dataset being balanced.

## Summary

Summarize the results of the machine learning models and include a recommendation on which model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

The logistic regression model trained on oversampled data exhibited significantly superior performance compared to the model trained on imbalanced data. This improvement is attributed to the balanced nature of the data, resulting in a notably higher accuracy score and enhanced recall. These outcomes indicate that the model is expected to make far fewer errors when categorizing non-healthy loans. Based on the examination of the confusion matrices, there is a significant reduction in the number of false positives, suggesting that the model is likely to accurately classify both healthy and non-healthy loans. Considering this analysis, I would recommend the utilization of Model 2, which is the Logistic Regression Model trained with balanced (oversampled) data.
