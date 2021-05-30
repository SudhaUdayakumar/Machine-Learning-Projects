**

## Temperature Multioutput Regression using Python Machine Learning 

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Temperature_Multioutput/Temperature%20Mutioutput%20Regressor.jpeg?raw=true)


**

## Summary
<![endif]-->

**Temperature Forecast- Multi-output Regression**

**Data Loading**

Data loads and we see a lot of numerical columns. Also we have 2 target columns T_Max & T_Min

**Pre Processing**

Pre-processing there were many missing values and we had to replace them with median. Date was Object column, which we converted to Year/Month/Day Columns

**EDA**

EDA of Tmax & Tmin was similar for month, year, latitude, longitude, slope. However once we move to Co-releation, we see that T_max and T_min have different co-relation

**Skewness & Outliers**

We got 11% outliers, so we will not handle it. Skewness from 14 columns was reduced to 4 columns using power Transform. Since we used Power Transform we didn’t have to use Standard Scalar or Min Max Scalar

**Model Building Preparation**

**2 Target Variables**

We can see that y_train & y_test has 2 columns. Usually only 1 target column is present. This is a Multi-Output Regression Model

We have 2 target columns. So this has to be handled differently

[https://machinelearningmastery.com/multi-output-regression-models-with-python/](https://machinelearningmastery.com/multi-output-regression-models-with-python/)

This Link gives a detailed explanation on how to handle 2 target columns

**Algorithms**

Some regression machine learning algorithms support multiple outputs directly.

This includes most of the popular machine learning algorithms implemented in the scikit-learn library, such as:

1. LinearRegression (and related)

2. KNeighborsRegressor

3. DecisionTreeRegressor

4. RandomForestRegressor (and related)

**MUltioutput**

In this Dataset we fit all the 4 on the multioutput regression dataset, then makes a single prediction with the fit model.

Running dataset with all the 4  algorithim and then makes a prediction for one input, confirming that the model predicted two required values.

**CrossValidation**

Error is reported across both output variables, rather than separate error scores for each output variable.

**Model Building**

1. In **Multi-output Regression** we see 2 values for each Algorithim as expected, as we have 2 target variables in this Dataset

2. **R2** is a good metric to measure and we have got good scores in Random Forest, Bagging Regressor and KNN. Highlighted only the top 2. So based on this we can use these 3 algos for HyperParameter Tuning

3. **RMSE** Scores are high, as the errors are punished higher. The **RMSLE** negates it and we see good low scores on RMSLE as well for Random Forest, Bagging, and KNN. Another reason to use them in finding RMSLE

4. R2 and **Cross Validation** difference is low for Linear Algos (Linear, Lasso, Ridge), however their R2 scores are not that high. So if we remove them, again Random Forest and Bagging tops our chart

We will use the 3 algos which are topping in every column for Hyper Parameter Tuning- Random Forest/KNN/Bagging<

**Hyper Parameter Tuning**

1.  RandomForest- we tuned several Methods and saved the good score
2.  KNN- also we did tuning but our score didn’t improve much
3.  Bagging- GridSearch – Slight Improvement
4.  Bagging-RandomSearch- Slight Improvement

Of all the Hyper Tuning Models, Random Forest had the best score and we saved and shared it to Biz

**Saving & Loading**

1.  Random forest model was saved. Later it was loaded and test for a sanity check. The scores matched
2.  We are good to share this saved model to Biz
**


To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Temperature_Multioutput/Temperature-%20Muti-output%20Regressor.ipynb) !
