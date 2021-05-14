**

## HR Analysis on Attrition  using Python Machine Learning

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/HRAnalysis_Attrition/HR%20Attrition.jpeg?raw=true)

<![endif]-->

**

## HR Analysis - on Attrition Dataset Summary

<![endif]-->

HR Attrition

**Data Loading**

The data loaded properly and we found that it is an imbalanced data set. Attrition was at 16% which is around the expected attrition rate in Companies. Since it is a imbalanced dataset we need to do Over Sampling and other techniques as well. For a person to leave a company, it is never one reason. So multiple columns have to be analysied

**Pre Processing**

There were no missing values, .however there were few columns which were redundant and not needed in the model building. So we have dropped them

**EDA**

When we have so many columns and rows , the EDA gets interesting and we were able to do lot of Uni Variate and Bi Variate Analysis. We separated them into Numerical Columns and Categorical columns to do a bi variate analysis for attrition to understand further. The Multi variate analysis was also done, to see which is the closest related column and which is not

**Skewness**

Skewness was handled before moving to Model Building

**Label Encoding**

Before going to Model Building, we had to do Label Encoding for few columns. Already there were many columns, so doing dummies or other forms of encoding would have increased the number of columns. So chose Label Encoding

**Standard Scalar**

Age is a 2 digit but salary would be more than 2 digits. A simple example of how we needed to do Standard Scalar, so that one column doesn’t influence another.

**Over Sampling**

We already saw that it is a imbalanced data. Our split of data wont be normal, so used Oversampling so that our Target data is equally balanced.

**Model Building**

After dropping the unwanted columns and choosing the right Train & Test data from Over Sampling, we went to Model building

1.  Used 6 algos and used F1, Precision , Recall and Cross Validation for evaluation.

2.  Then compared the F1 score with Cross validation and choose the best model which has the least difference. Random Forest stood out than other Algos, and we selected it.

**Hyper Parameter Tuning**

1.  Random Forest on Hyper tuning moved from 98% to 100% and improved our model to a perfect score

**Saving & Loading**

1.  The same highest score model- Random Forest Hyper Tuned model was saved. Later it was loaded and test for a sanity check. The scores matched

2.  We are good to share this saved model to Biz

To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/HRAnalysis_Attrition/HR%20Analytics-%20Attrition.ipynb) !
