**

## Customer Churn Analysis using Python Machine Learning 

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/CustomerChurn/Customer%20churn.jpeg?raw=true)

##  Summary


**Customer Churn Analysis**

**Data Loading**

Data loaded properly and we see that there are lot of yes/no, male/female values. The customer ID might be dropped.

**Pre Processing**

Customer ID was unique to each customer and we dropped the column. On further analysing we saw that the Total Charges has numerical data, but is shown as Object column. It means, some space or special characters are present. So it was analyzed and the blank spaces were replaced with Nan. Since only 11 values were replaced, we went and directly replaced them with Median data. Now all our columns were set for EDA

**EDA**

EDA gave us some interesting info on who churned more and compared within the ranges of Senior Citizens, Tenure, Gender, Dependents and other Services

**Skewness & Outliers**

Skewness was present in 5 columns and they were categorical in nature. So we did not handle them. Outliers were present again in columns, where we had ordinal values. So didn’t handle them as well

**Ordinal Encoding**

Since there were lot of Ordinal Data present, we used the Ordinal encoding. And then we did re-shape.

**Min Max Scalar**

Used Min Max scalar as the range was low and lot of independent columns were categorical in Nature

**Model Building**

Was done in 2 ways after finding the Best Random state

1.  Model 1: We have used 6 models and 3 Evaluation Techniques (F1 Score, Classification Report & Cross Validation). In the Classification Report we saw the score equal in both classes, which says it is a good model. Decision Tree & Random forest topped the charts
2.  Model2: We have used 6 models and 3 Evaluation Techniques (F1 Score, Cross Validation, diff between F1 Score & Cross Validation). Almost every model the diff was lowest and the top ones were chosen- which again was Decision Tree & Random forest
3.  Model 3: ROC_AUC for model evaluation of 6 models. Random forest topped the charts

**Hyper Parameter Tuning**

1.  Hyper Tuning was done on 2 models (Decision Tree & Random forest) both had the same score of almost 100%. Random Forest being a better algo than Decision Tree, it was used to Save & Load the Model

**Saving & Loading**

1.  Random forest model was saved. Later it was loaded and test for a sanity check. The scores matched
2.  We are good to share this saved model to Biz



To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/CustomerChurn/CustomerChurn.ipynb) !
