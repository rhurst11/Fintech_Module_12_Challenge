# Module 12 Report

## Overview of the Analysis

### Purpose

When using machine learning to predict credit risk, it is critical to understand the near-inevitability of working with imbalanced datasets.

Instances or individuals who pose a high credit risk can be particularly hard for machine learning models to adequately predict, since they will almost always compose the minority label group in an imbalanced dataset.

It is important to try multiple techniques, including resampling techniques, in order to have the most efficacious model for catching instances that pose a high risk. 

This analysis attempts to evaluate the importance of resampling when creating machine learning models that utilize imbalanced datasets, and this work should be able to provide insight that goes beyond the isue of credit risk alone. 

Many of the imbalancing issues present in credit risk data remain prevalent in fraud detection as well. Essentially, any instance where an individual works with a dataset that has a clear majority class in its target variable could find this analysis useful.


### Process

This analysis relies on a dataset of lending data composed of seven columns that outline characteristics of each loan, and one column that classifies each loan. This lending data classifies loans using a binary scale; A label of 0 means that a loan is healthy, whereas a label of 1 means a loan is unhealthy / risky.

This analysis echoes the same basic structure of many classification models focused on credit risk or fraud detection. The target variable is the "loan staus" column of our data, which holds the binary classifications of each loan described in the dataset. 

The features variables used to train the model were all columns other than the loan staus column present in the lending dataset.


#### Sub-Process: Machine Learning

This analysis builds all of its machine leaning models around a logistic regression algorithm. Logistic regression is a popular method used for classification problems in machine learning, and provides adequate complexity and depth for the given use case. 


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
