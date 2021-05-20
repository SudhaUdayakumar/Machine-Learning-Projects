**

## Census Income prediction using Python Machine Learning

**

![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Census/Census.jpeg?raw=true)

##  Summary



**Census**

**Data Loading**

The data loaded properly and it was moderate dataset size.

**Pre Processing**

There were duplicate values, and data contained “?” in it as well. So we have to remove the duplicate values and “?” were replaced with Mode of the respective column. Also we found that it was an imbalanced dataset

**EDA**

We did the EDA based on Uni variate, Bi-Variate and Multi Variate analysis. We could clearly find a good relationship and which was dominating in a feature. E.g. USA as Native_country, Private in workclass etc.

**Outliers & Skewness**

When we tried to handle outliers, through Z score, 15% of data got lost. That is huge data to be lost. Also this being an imbalanced dataset it was expected. So the outliers were not handled and only skewness through Power Transformation. Few columns skewness was still present, but we were good enough to go for model building.

**Oversampling**

Since this is an imbalanced Dataset for classification, we had to do Oversampling, so that data is balanced before moving to Model Building

**Model Building**

Was done in 2 ways after finding the Best Random state

<![if !supportLists]>1. <![endif]>Model 1: We have used 6 models and 3 Evaluation Techniques (F1 Score, Classification Report & Cross Validation). In the Classification Report we saw the score equal in both classes, which says it is a good model. Decision Tree & Random forest topped the charts

<![if !supportLists]>2. <![endif]>Model2:  We have used 6 models and 3 Evaluation Techniques (F1 Score, Cross Validation, diff between F1 Score & Cross Validation). Almost every model the diff was lowest and the top ones were chosen- which again was Decision Tree & Random forest

<![if !supportLists]>3. <![endif]>Model 3: ROC_AUC for model evaluation of 6 models. Decision Tree & Random forest topped the charts

**Hyper Parameter Tuning**

<![if !supportLists]>1. <![endif]>Hyper Tuning was done on 2 models (Decision Tree & Random forest) both had the same score of almost 100%. Random Forest being a better algo than Decision Tree, it was used to Save & Load the Model

**Saving & Loading**

1.  Random forest model was saved. Later it was loaded and test for a sanity check. The scores matched

2.  We are good to share this saved model to Biz

To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Census/Census.ipynb) !
