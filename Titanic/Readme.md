
Titanic Dataset- Python Machine Learning
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Titanic/Titanic.jpeg?raw=true)
Titanic Dataset

1.  We had lot of pre-processing to do as there were missing values. We handled the missing values with mode & median
2.  We then merged the family column and dropped the Cabin Column as it had more than 50% missing values
3.  As we go to EDA, we found that Females survived more.
4.  Also we created Age bins to see the suvival rate. The senior citizens didnt survive much on the harsh conditions
5.  Looks like first class people had more access to lifeboats than people in third class, as more First class people had survivied

Moving on to the Model Building

1.  It was a balanced dataset,, however it was not 50:50, we used stratify for y_train and y_test to balance the test data
2.  RFC was our best model choosen
3.  With Hyper Parameter tuning, our model acccuracy on Cross validtion improved from 80 to 82 %

To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Titanic/Titanic%20Dataset.ipynb)
