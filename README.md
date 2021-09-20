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

This analysis echoes the same basic structure of many classification models focused on credit risk or fraud detection. The target variable is the "loan status" column of our data, which holds the binary classifications of each loan described in the dataset. 

The features variables used to train the model were all columns other than the loan staus column present in the lending dataset.


#### Sub-Process: Machine Learning

This analysis builds all of its machine leaning models around a logistic regression algorithm. Logistic regression is a popular method used for classification problems in machine learning, and provides adequate complexity and depth for the given use case. 


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Model 1 Accuracy, Precision, and Recall scores.
  
Balanced Accuracy Score:

0.9520479254722232

* Precision:

    * Group 0:
        * 1.00
    * Group 1:
        * 0.85

* Recall:

   * Group 0:
       * 0.99
   * Group 1:
       * 0.91

* Machine Learning Model 2:
  * Model 2 Accuracy, Precision, and Recall scores.
  
Balanced Accuracy Score:

0.9936781215845847

* Precision:

    * Group 0:
        * 1.00
    * Group 1:
        * 0.84

* Recall:

   * Group 0:
       * 0.99
   * Group 1:
       * 0.99

## Summary

It is important to remember the role of recall when assessing the efficacy of both of the machine learning models outlined in this project. Recall is a particularly important evaluation metric when assessing the performance of models created for the purpose of catching rare, but detrimental, instances of a particular outcome or classification label.

The recall metric displays how adequately a model correctly predicted the class of a certain instance compared to the total number of instances that actually belong to said class. In the case of credit-risk, the recall value of the "unhealthy loan" class (group 1 in this context) needs to be optimal, even if this optimization leads to minor detriments in precision or accuracy. 

For this reason, the second model, which was trained using oversampled data, will perform significantly better than its counterpart that utilizes original and unmodified data for the given use case. The second model eliminates much of the recall error for group 1 that is present in the initial, unmodifed model. Model 2's increase in recall for group 1 means that it will identify credit-risks with a higher degree of reliability than its non-resampled predecessor.

It is important to note that the oversampled (second) model does have a slightly decreased precision value for group 1, but this really is not detrimental given the use case of both models. The decrease in precision is minimal, and the worst outcome this may lead to is a missclassification of a healthy loan. This particular kind of missclassification poses far less financial risk than missclassifying unhealthy loans. 