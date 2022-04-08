# House-Price-Prediction

**Task**: Predict the selling price of each house

**Medium Blog**: https://parisrohan.medium.com/top-3-rank-kaggle-house-prices-advanced-regression-techniques-using-bagging-ensemble-ff2a3f9b70cb

1. **Data Collection**: 
    The kaggle dataset can be downloaded from https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview
    The train data has 1460 records and 81 features.

2. **EDA**:
    2.1. Distribution of right-skewed Target feature
    ![image](https://user-images.githubusercontent.com/49038495/162480861-be579207-f485-4fd9-b67c-84f4b1d1a684.png)
    2.2. Outlier detection

3. **Feature Engineering**:
    3.1. Handle missing data
    
        i. On data exploration we can see that there are few features where having a missing values makes sense. So we will impute the missing value with keyword 'Missing'
        
        ii. Replace the remaining categorical features with the mode of feature to impute missing values.
        
        iii. Impute missing numerical features with mean of the feature.
        
    3.2. Drop the feature 'Id' as it is not required.
    
    3.3. Create the total square footage feature 'TotalFlrSF' which is the addition of '1stFlrSF' and '2ndFlrSF'
    
    3.4. Create 'Total_Bath' feature 
    
    3.5. Find the skewness of data and use log transformation to get a gaussian distribution curve.
    
    3.6. Encode categorical data

4. **Model Building**: Use K-fold cross validation and bagging ensemble to build a model

**Leaderboard Ranking**
![image](https://user-images.githubusercontent.com/49038495/162482532-264269fa-b399-4009-962c-85a2d71b12cc.png)

    
    
