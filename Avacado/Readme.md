
**

## Avocado Predicting Price using Python Machine Learning

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Avacado/avacado2.gif?raw=true)

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Avacado/Avacado%203.gif?raw=true)

![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Avacado/name.gif?raw=true)

##  Summary

**Data Loading**

The data loaded properly and we found that it is had a lot of “nan” values. So had to remove the “nan” values. Further analysis we found it is a regression data set and need to handle based on it

**Pre Processing**

After removing the “nan” values, few columns which were redundant were dropped. Also the Date was an object column, had to be converted to DateTime, and we extracted the month from it. We used the month later in our EDA, but dropped it later.

**EDA**

We did the EDA based on timeline, year, months and got some interesting information. Also the places where Avocado was used and least used, was found

**Label Encoding**

Before going to Model Building, we had to do Label Encoding for few columns. Region was Label Encoded. Year was also Label Encoded, as to make sure it doesn’t impact the data coz of the high numerical value

**Outliers & Skewness**

Handled Outliers via Z score and Skewness through log transformation before moving to Model Building

**Standard Scalar**

Standard Scaled and Skewness data were similar at high level but it is a best practice to do Standard Scaling and hence it was used.

**Model Building**

Was done in 2 ways after finding the Best Random state

1.  Model 1: We have used 7 models and 5 Evaluation Techniques. Apart from that we have found the diff between R2& CV, and RMSE &CV as well.Random Forest topped our Chart

2.  Model 2: Feature Engineered Model. Dropped a column for which the co-relation was close to “0”. And we found an improvement for Random Score and major improvement for K-Neighbors.

**Hyper Parameter Tuning**

1.  Hyper Tuning was done on 3 models and the best was selected. Random Forest was the highest and saw a improvement in the score !

**Saving & Loading**

1.  The same highest score model- Random Forest Hyper Tuned model was saved. Later it was loaded and test for a sanity check. The scores matched

2.  We are good to share this saved model to Biz

To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Avacado/Avacado%20Project.ipynb) !
