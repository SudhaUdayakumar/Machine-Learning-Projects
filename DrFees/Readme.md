
**

## Doctor Consultation Fees Prediction using Python Machine Learning 

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/DrFees/Dr%20Consultation%20Fees.jpeg?raw=true)

##  Summary


**Predicting Doctor Consultation Fees**

**Data Loading**

Data was split into Train & Test. We combined them to do the Pre-processing and EDA. Then before modelling we went back to the data set of train & test

**Pre Processing**

This dataset had lot of pre-processing to do. It had more text values in its columns and we had to handle one by one. Place column was split into Area & City. Qualification, we retained the top 2 degrees. Miscellaneous Info column had too many missing values we dropped them

**EDA**

EDA gave us some interesting info on which profile doctors charged more. Practice of Dentists are higher as well.

**Model Building**

Was done in 2 ways after finding the Best Random state

Model 1: We have used 7 models and  6 Evaluation Techniques (R2, RMSE, MAE, MSE, Cross validation-R2, Cross validation-RMSE). Also we found the diff of R2 & CV-R2diff, RMSE & RMSECV diff. The scores were not that good.

Model2:  PCA: We used the PCA to use only the top data. Here again We have used 7 models and  6 Evaluation Techniques (R2, RMSE, MAE, MSE, Cross validation-R2, Cross validation-RMSE). Also we found the diff of R2 & CV-R2diff, RMSE & RMSECV diff. The scores were not that good.

Model 3: Feature Engineering. We removed the sub-columns of Qualification. Here again We have used 7 models and  6 Evaluation Techniques (R2, RMSE, MAE, MSE, Cross validation-R2, Cross validation-RMSE). Also we found the diff of R2 & CV-R2diff, RMSE & RMSECV diff. The scores were not that good.

After clear analysis we see that the evaluation metric is not a right choice. So our evaluation has to be changed. RMSE explodes in magnitude as soon as it encounters an outlier. In contrast, even on the introduction of the outlier, the RMSLE error is not affected much. This link clearly says why RMSLE is a better evaluation metric than RMSE when there are outliers. Our data has lot of outliers, and so lets use RMSLE in our model [https://medium.com/analytics-vidhya/root-mean-square-log-error-rmse-vs-rmlse-935c6cc1802a](https://medium.com/analytics-vidhya/root-mean-square-log-error-rmse-vs-rmlse-935c6cc1802a)

Model 4. We added 1 more algo (Bagging Regressor) and one more evaluation technique. RMSLE. Also we found out the Cross validation of RMSLE as well. We found the RMSLE scores have improved.

Model 5. Feature Engineering +RMSLE- Scores improved
Model 6. PCA+ RMSLE- Scores improved.

**Hyper Parameter Tuning**

Hyper Tuning was done on Gradient Boost and Random Forest. Random Forest score had improved. So we will use the same and pass it to the Biz

**Saving & Loading**

1.  Random forest model was saved. Later it was loaded and test for a sanity check. The scores matched

2.  We are good to share this saved model to Biz



To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/DrFees/DoctorFees.ipynb) !
