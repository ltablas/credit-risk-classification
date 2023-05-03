# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

  The first model is testing the Accuracy, Precision, and Recall scores of data column "loan_status" using the logistic regression model, with variables set to "healthy loan" (data value 0) and "high-risk loan" (data value 1). The overall accuracy report is measured by a scale of 0 to 1, with 1 meaning 100% accuracy that a loan is accurately classified as being either healthy or high-risk. This particular model has an accuracy score of 0.95 (meaning accuracy is very good), and almost perfect scores for predicting precision and recall scores for healthy loans (1, and 0.99 respectively). High-risk loans are slightly less predictable/accurate than healthy loans with precision and recall scores of 0.85 and 0.91 respectively, but still strong enough to be considered reliable.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  Model 2 in concept is similar to model 1, except that now we're looking at the accuracy, precision, and recall scores using a subset, or sample of the data, versus the original dataset. This type of analysis would be done to see if we could reduce the size of the dataset and still get similar results as the original (ie full) dataset. The oversampled data model has a much higher accuracy score than the original dataset (.99 compared to .95), and much higher recall score (.99 vs .91), meaning it is much more accurate overall, and better able to identify true positives.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best? 

The second model seems to perform best because while it performs the exact same as model 1 in terms of predicting "healthy loans", it does a much better job of predicting "high-risk loans", shown by a higher accuracy, precision, and recall score. What this means is that the 2nd model can more accurately categorize a loan as high-risk, which for an investor could mean mitigating risk by tactics such as denying the loan, or increasing borrowing interest rate. 

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? ) Depends on who the target audience is. If the analysis is done for the person issuing the loan, ie a bank, it would be more important to predict unhealthy loans. In this case, the bank could offer much higher interest rates or choose to deny the loan altogether to mitigate risk. On the other hand, if the target audience is the person applying for the loan, the goal would be predict a higher healthy loan status, as then the person could qualify for more incentives or smaller interest rate.

If you do not recommend any of the models, please justify your reasoning.
