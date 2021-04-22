
**

## Mushroom Project Dataset

**

Mushrooms are edible or poisonous but how do we differentiate what makes it edible or poisonous ? Multiple parameters and they are going to be called as features in our dataset. And our target variable would be edible or poisonous

The source for the dataset is from [UCI](https://archive.ics.uci.edu/ml/datasets/mushroom)

our target variable , Edible & Poisonous 
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Mushroom/Mushroom%20Types.png?raw=true)

Features of the Mushroom

![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Mushroom/Mushroom%20Features.jpg?raw=true)

Machine Learning Models used and their evaluation methods and conclusion
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Mushroom/Machine%20Learning%20Models%20and%20their%20evaluation%20score.png?raw=true)

Summary of the Project

1. We got the data and analysed what type of data it was- found it was classification ,  the target column has 2 variables
    and it is a balanced dataset
    
2. Pre-processing the data: Converted the data using Label Encoding, only then we can use it for Machine Learning. 
    Also used the Label Encoded data for EDA. Also checked for any columns needs to be dropped, missing values etc. Since
    this is a classification data, cant handle the Outliers and Skewness
    
3. EDA- Did uni-variate analysis, bi-variate analysis (against the target variable) and multi variate analysis 

4. Model Building- Used various Models to build using 2 methods. Since this is a balanced dataset, used the second method 
    to generate the Accuracy, Cross validation and the diff between accuracy & Cross validation in a table
    
5. Hyper Parameter tuning- After we found DTC is the best model, did hyper parameter tuning for academic reasons. 
    Why academic reasons, coz the accuracy score was already at 100%
    
6. Save & Load the model. Saved the model and before handing over, just loaded & test the model to see if its working fine
    if the accuracy is the same and predictions are coming up. All were working fine 

7. For all the steps the Observation was highlighted in Yellow and the Notes were highlighted in Pink. Also the Table of 
    Contents was added, to have a good view of the flow 
    
This summarizes the steps at a high level and how the DTC model was built

To see my Python Notebook, please click [here](https://nbviewer.jupyter.org/github/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Mushroom/Mushroom_Dataset.ipynb)
