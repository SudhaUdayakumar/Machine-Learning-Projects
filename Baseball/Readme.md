
**

## Baseball Win Analysis using Python Machine Learning

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Baseball/baseball-icegif-7.gif?raw=true)

![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Baseball/baseball-2.gif?raw=true)

![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Baseball/baseball-3.gif?raw=true)

##  Summary

<![endif]-->

**Baseball**

**Data Loading**

The data loaded properly and it was a very small dataset of 30 rows and 17 columns. So we might need to be careful before removing any data and use simple models

**Pre Processing**

There were no missing values, Duplicate values , or any column needed to be dropped. So we went directly to do EDA

**EDA**

We did the EDA based on Uni variate, Bi-Variate and Multi Variate analysis. We could clearly find the linear relationship between the “W” and features.

**Outliers & Skewness**

Handled Outliers via Z score and Skewness through Power transformation before moving to Model Building. Since we already did power transformation, our data was scaled and we didn’t have to scale it later.

**Model Building**

Was done in 2 ways after finding the Best Random state

<![if !supportLists]>1. <![endif]>Model 1: We have used 7 models and 5 Evaluation Techniques. Apart from that we have found the diff between R2& CV, and RMSE &CV as well. Simple models like Linear/Ridge/Lasso topped the chart

<![if !supportLists]>2. <![endif]>Model2: PCA: We used PCA and analysed the data. Simple models like Linear/Ridge/Lasso R2 Score dropped. For other models improved but didn’t still match the Linear/Ridge/lasso

<![if !supportLists]>3. <![endif]>Model 3: Feature Engineered Model. Dropped 2columns for which the co-relation was close to “0”. And we found an improvement for Linear/Ridge

**Hyper Parameter Tuning**

<![if !supportLists]>1. <![endif]>Hyper Tuning was done on 3 models and the best was selected. Linear Regression was the highest and saw a improvement in the score !

**Linear Regression Plot**

1.  Visualized how close the predicted where to the actual scores

**Saving & Loading**

1.  The same highest score model- Linear Regression Hyper Tuned model was saved. Later it was loaded and test for a sanity check. The scores matched

2.  We are good to share this saved model to Biz

To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Baseball/Baseball%20case%20study.ipynb) !
