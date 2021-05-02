**

## Abalone Dataset

**
![enter image description here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Abalone/Abalone%20Header.jpeg?raw=true)

Have to predict the rings of each abalone which will lead us to the age of that abalone.

Model Set- Abaolone

1. 1. Pre-Processing: 
    Converted the multiple ranges of "Rings" target column to 3 categories. Also for later model did for "2" categories, to check on Binomial. For regression nothing was done

    2. Skewness 
        Skewness was handled for both types of models (Regression & Classification)
        
    3. EDA:
        We found that with increasing age, the length,height, and weight was increasing
    4. Model Building
        We found the best score, when Rings was in 2 categories. This shows that less complex the data, more acccurate
        The Regression data was also fine, but the Binomial output was much better
        
    5. Hyper Parameter Tuning
        As we mentioned the Binomial class had the best output and the best model in that was choosen for Hyper Parameter 
        tuning and saving the model. It was also loaded and checked
        
    Conclusion: Given a dataset it can be handled with Regression and Classification after handling the data as needed
To view my Jupyter notebook, please click [here](https://github.com/SudhaUdayakumar/Machine-Learning-Projects/blob/main/Abalone/Abalone%20Dataset.ipynb)
