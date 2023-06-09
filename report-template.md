# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
This analysis is specifically being done to get data that will back future decisions concerning creditworthiness and otherwise.
* Explain what financial information the data was on, and what you needed to predict.
We needed to predict risk associated with credit.  Who to lend to, who is a sufficient candidate and who poses the risks with lended credit.  
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
Tools for creating this data consisted of python and libraries such as sklearn.  Within sklearn we used metrics of balanced accuracy, confusion matrix, classification report imbalanced.  In order to test and train data into datasets train_test_split module from sklearn was implemented.  Other libraries within helped the process as well.
* Describe the stages of the machine learning process you went through as part of this analysis.
Steps in the process consisted of obtain original data, spliting it in to variables, checking initial data such as value count in order to compare with later model data.  The data is again split into training and testing datasets.  Afterwards that data is then place in Model methods such as logistic regression, that follows up with predictions, and then reports.  

To get a better understanding of the data we resample the data in accordance to weak points such as data that arent sampled enough or too much.  So we oversample or undersample for newer results.  With the datasets of the new sample we repeat the steps and then compare the results from both.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
Methods mentioned above.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
                        precision    recall  f1-score   support

               0       1.00      0.99      1.00     18765
               1       0.85      0.91      0.88       619

        accuracy                           0.99     19384
       macro avg       0.92      0.95      0.94     19384
    weighted avg       0.99      0.99      0.99     19384



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
                         pre       rec       spe        f1       geo       iba       sup

              0       1.00      0.99      0.99      1.00      0.99      0.99     18765
              1       0.84      0.99      0.99      0.91      0.99      0.99       619

    avg / total       0.99      0.99      0.99      0.99      0.99      0.99     19384

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

The first difference if that the accuracy score is roughly 5% higher. Based on the amount of data points, it is a positive improvement. There is a 1% change in the precision, so in this case the original model did a point better. The recall had a impressive push of 8% in a positive direction making both class 0 and 1 better at predicting both credit worthiness or not.  I would recommend the Model 2 for clear reasons of more appropriate accuracy.

If you do not recommend any of the models, please justify your reasoning.

Both models would work because they both do not have a stark negative accuracy.  But the second model is better. 