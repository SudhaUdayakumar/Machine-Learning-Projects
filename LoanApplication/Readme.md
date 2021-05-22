
**

## Loan Application Status prediction using Python Machine Learning

**

![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/LoanApplication/Loan%20Application%20status.jpeg?raw=true)

##  Summary




<![endif]-->

**Loan Prediction**

**Data Loading**

The data loaded properly and it was moderate dataset size. It is a classification imbalanced dataset. So need to be careful while handling outliers and skewness

**Pre Processing**

There were missing values which were replaced with Mode (classification) and median (for numerical data- which were not normally distributed). Also the redundant column of “Loan_ID” was dropped from the dataset.

**EDA**

We did the EDA based on Uni variate, Bi-Variate and Multi Variate analysis. We could find that men, married people took more loan. Also people with 0 dependents had got more loan. People in Semi-Urban, Self-employed, with credit score were the highest people who applied and got the loan as well.

**Outliers & Skewness**

Skewness was handled in columns where it colums. Already columns which were skewed like 30 years loan etc cant be skewed further.

**Oversampling**

Since this is an imbalanced Dataset for classification, we had to do Oversampling, so that data is balanced before moving to Model Building

**Model Building**

Was done in 2 ways after finding the Best Random state

<![if !supportLists]>1. <![endif]>Model 1: We have used 6 models and  3 Evaluation Techniques (F1 Score, Classification Report & Cross Validation). In the Classification Report we saw the score equal in both classes, which says it is a good model. Decision Tree & Random forest topped the charts

<![if !supportLists]>2. <![endif]>Model2:  We have used 6 models and  3 Evaluation Techniques (F1 Score, Cross Validation, diff between F1 Score & Cross Validation). Almost every model the diff was lowest and the top ones were chosen- which again was Decision Tree & Random forest

<![if !supportLists]>3. <![endif]>Model 3: ROC_AUC for model evaluation of 6 models. Random forest topped the charts

**Hyper Parameter Tuning**

<![if !supportLists]>1. <![endif]>Hyper Tuning was done on Random forest and had score of 100%. Random Forest was used to Save & Load the Model

**Saving & Loading**

1.  Random forest model was saved. Later it was loaded and test for a sanity check. The scores matched

2.  We are good to share this saved model to Biz

To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/LoanApplication/LoanApplicationStatus.ipynb) !
