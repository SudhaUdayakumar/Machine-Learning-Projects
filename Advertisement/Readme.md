
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Advertisement/Advertisement.jpeg?raw=true)
***Advertising Sales Channel Dataset***

 Sales Channel Prediction Case Study
    
1. We have to see which channel has the highest Sales. Radio/Newspaper or TV
2. All our EDA shows TV has the highest sales, through our various plots
3. Processing our data.
    Drop Column. The Unnamed column acts like a serial number so we drop them
    Outlier: Only 2 values in Newspaper have outlier, so we are dropping it. it comes to almost only 1% of data , so we are dropping it
    Skewness: Was only with newspaper, and since there are negative values, used power transform to transform the data (except sales)    
        
4. Model Building:
    We have used 6 models to build our data
    We have used MAE, MSE, RMSE & R2 To evaluate our models
    For CV we have used R2 score as well
    
    After analyzing and finding the diff, we found Random Forest is best
    
5. Hyper Parameter Tuning. 
    Our data is already 97% but with hyper parameter tuning, we were able to get 98% and its a good improvement
    
6. Later we saved and loaded our model to check if it is working fine. We tried to save the model, in 2 ways for academic purpose

To view my notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Advertisement/Advertising%20Sales%20Channel%20Prediction.ipynb)
