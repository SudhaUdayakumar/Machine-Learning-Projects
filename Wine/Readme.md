**

## Wine Python Machine Learning Project

**
Predict the wine quality score, using the physiochemical properties

![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Wine/Wine%20Data%20Analysis.png?raw=true)

In this project, we will examine the data and build different machine learning models that will detect the happines score based on the features given.
What might be an interesting thing to do, is to set an arbitrary cutoff for your dependent variable (wine quality) at e.g. 7 or higher getting classified as 'good/1' and the remainder as 'not good/0'.
This allows you to practice with hyper parameter tuning on e.g. decision tree algorithms looking at the ROC curve and the AUC value.

**Conclusion**

Wine Quality could have been done using 2 categories as well. However from the problem statement, it makes 
more meaning to split the Wine Quality using 3 categories

We have used Stratify, so that the data is easily split as per the imbalance %. This helps in good model building

We have built 4 models and since this is an imbalanced dataset, we have used F1score, precision, recall
Also to avoid over fitting and underfiitng issues, we have used Cross Validation and there we have used AUC ROC

After selecting the model, we have chosen the best model and done hyper Parameter tuning on it, to improve the performance.

Then finally we have saved the model and loaded to check if it works fine

To view the details of my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Wine/Quality%20of%20Wine%20Prediction%20using%20ML.ipynb)
