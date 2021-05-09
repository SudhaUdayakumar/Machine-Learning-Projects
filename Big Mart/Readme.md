
**

## Big Mart Dataset Analysis  using Python Machine Learning

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Big%20Mart/BigMart.jpeg?raw=true)

<![endif]-->

**

## BigMart Dataset Summary

**

**Data Loading**

This was an interesting Dataset, where the Train & Test data was split. We can either combine or use them, or use them as is. However if we don’t combine, we might need to do EDA, handling of data in train and test. In case we drop any row,

We need to be careful and drop the same rows. So instead we combine the data and add a column called “Source”, where we know which is train and test, so easier to split during model building

**Missing Values**

Item Weight and Item Size were immediately visible as missing values. However Visibility we had to check and then handle it.

**EDA**

When we have so many columns and rows , the EDA gets interesting and we were able to do lot of Uni Variate and Multi Variate Analysis

**Feature Engineering**

Combining few columns or grouping few data, gave us more and better insights of data

**Skewness**

Skewness was handled before moving to Model Building

**Model Building**

After dropping the unwanted columns and choosing the right Train & Test data, we went to Model building

1.  Used 7 algos and used MAE, MSE, RMSE, R2 and Cross Validation (R2) for evaluation.
2.  PCA: Since the score was not very high, applied PCA to reduce the dimensionality and then ran the 7 algos and MAE, MSE, RMSE, R2 and Cross Validation (R2) for evaluation.
3.  PCA actually decreased the scores, so decided to use the non-PCA for Hyper Parameter Tuning

**Hyper Parameter Tuning**

1.  Used 3 times the Hyper Parameter Tuning.2  on top Algos (RF, Gradient) and on the lowest (KNN)
2.  For all 3 , the performance had improved
3.  Choose the one with the highest score (R2) and it was Gradient Boosting

**Saving & Loading**

1.  The same highest score model- Gradient Hyper Tuned model was saved. Later it was loaded and test for a sanity check. The scores matched
2.  We are good to share this saved model to Biz

To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Big%20Mart/Big%20Data%20Mart%20Sales.ipynb) !
