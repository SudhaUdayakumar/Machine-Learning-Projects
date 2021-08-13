**

## UsedCars-Webscrapping and Model Building using Python

![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/UsedCars/usedcars.jpg?raw=true)



# Summary

**Used cars**

**Webscrapping**

Used live websites to scrape data. Collected close to 10k data from cars24. Also collected 5k from other sites (OLX, Carwale, Carsandbikes). Decided to go with the Cars24 data, as there were duplicates in other data.

**Pre Processing**

1.  Excel Preprocessing: Webscrapped multiple cities and merged them using excel. Also certain operations of adding the type -Sedan/hatchback/SUV etc was done as it didn’t come in the data. It is a very important factor and used google to fill in data.
2.  In Jupyter notebook, we deleted the unwanted columns and used them

**EDA**

EDA gave us some interesting info on the types of car. Sedan and Hatchback was high. Noida had more cars etc.

**Model Building** Was done in 2 ways after finding the Best Random state

<![if !supportLists]>1. <![endif]>Model 1: We have used 7 models and 6 Evaluation Techniques (R2, RMSE, MAE, MSE, Cross validation-R2, Cross validation-RMSE). Also we found the diff of R2 & CV-R2diff, RMSE & RMSECV diff. The scores were not that good.

<![if !supportLists]>2. <![endif]>Random forest was best and we will use that on Hyper Parameter Tuning

**Hyper Parameter Tuning**

<![if !supportLists]>1. <![endif]>Hyper Tuning was done on Random Forest. Random Forest score had improved. So we will use the same and pass it to the Biz

**Saving & Loading**

<![if !supportLists]>1. <![endif]>Random forest model was saved. Later it was loaded and test for a sanity check. The scores matched

<![if !supportLists]>2. <![endif]>We are good to share this saved model to Biz

You can view my Machine Learning book [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/UsedCars/Used%20Cars%20.ipynb) and a sample for one city of webscrapping file [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/UsedCars/Used%20Cars24_Bengaluru.ipynb)
