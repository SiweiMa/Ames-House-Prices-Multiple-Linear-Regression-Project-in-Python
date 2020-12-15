# Ames House Prices: Multiple Linear Regression Project in Python
*The repository is a part of final project of course MSDS 601.* 

#### by [Siwei Ma](https://www.linkedin.com/in/siwei-ma-28345856/)


# Executive Summary
Give [Ames Housing dataset](http://jse.amstat.org/v19n3/decock.pdf), the project started with an exploratory data analysis (EDA) to identify the missing values, suspicious data, and redundant variables. Then I performed a mixed stepwise selection to reduce the set of variables and select the best model based on AIC, BIC, and adjust R-squared. With the best model selected, the model assumptions were checked regarding normality, homoscedasticity, collinearity, and linearity between response and predictors. Several solutions were proposed to solve the assumption violation. The model was then tested on unseed data and scored on Root-Mean-Squared-Error (RMSE).

# Data Summary
**Data source**
The data of this project came from [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques). 
**Data Dictionary**
|Category|Index|Name|
|--|--|--|
|Type|1|MSSubClass|
|^|15|BldgType
|^|16|HouseStyle
|Location|2|MSZoning
|^|12|Neighborhood
|^|13|Condition1
|^|14|Condition2
