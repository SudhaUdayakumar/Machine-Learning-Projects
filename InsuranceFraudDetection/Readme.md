
**

## Insurance Fraud Detection using Python Machine Learning 

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/InsuranceFraudDetection/InsuranceFraud.png?raw=true)

##  Summary


**Insurance Fraud Detection**

**Data Loading**

Data loaded properly and we see there are few “?” and na values which needs to be handled.

**Pre Processing**

There were totally 1000 rows of data. So any column which had more than 900 unique values were dropped, as they don’t add value. Also column with no values were dropped. The “?” were replaced as Unknown category

**EDA**

EDA gave us some interesting info on who were the fraud claims more and compared within the profession, city, state, age, profession, type of claims etc. Interesting we see that people with hobbies as Chess and Cross Fittness had the highest fraud claim. Also people with High claims had more fraudulent data

**Skewness & Outliers**

Outliers was less than 2% of data, so we removed them. Skewness was present only in 3 columns and they didn’t had to be handled.

**Ordinal Encoding**

Since there were lot of Ordinal Data present, we used the Ordinal encoding. And then we did re-shape.

**Standard Scalar**

Used Standard Scalar as the range was high and we had to bring everything to one scale

**Model Building**

Was done in 2 ways after finding the Best Random state

1.  Model 1: We have used 6 models and 3 Evaluation Techniques (F1 Score, Classification Report & Cross Validation). In the Classification Report we saw the score equal in both classes, which says it is a good model. Decision Tree & Random forest topped the charts
2.  Model2: We have used 6 models and 3 Evaluation Techniques (F1 Score, Cross Validation, diff between F1 Score & Cross Validation). Almost every model the diff was lowest and the top ones were chosen- which again was Decision Tree & Random forest
3.  Model 3: ROC_AUC for model evaluation of 6 models. Random forest topped the charts

**Hyper Parameter Tuning**

1.  Hyper Tuning was done on Random forest) and had the perfect score 100%. It was used to Save & Load the Model

**Saving & Loading**

1.  Random forest model was saved. Later it was loaded and test for a sanity check. The scores matched
2.  We are good to share this saved model to Biz



To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/InsuranceFraudDetection/InsuranceclaimsFrauddetection.ipynb) !
