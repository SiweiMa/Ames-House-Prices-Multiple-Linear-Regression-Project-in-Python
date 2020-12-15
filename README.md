# Multiple Linear Regression Project: Ames House Prices
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
||15|BldgType
||16|HouseStyle
|Location|2|MSZoning
||12|Neighborhood
||13|Condition1
||14|Condition2
|Lot|3|LotFrontage
||4|LotArea
	7	LotShape
	10	LotConfig
Roof	21	RoofStyle
	22	RoofMatl
Exterior	23	Exterior1st
	24	Exterior2nd
	25	MasVnrType
	26	MasVnrArea
	27	ExterQual
	28	ExterCond
Foundation:	29	Foundation
Basement	30	BsmtQual
	31	BsmtCond
	32	BsmtExposure
	33	BsmtFinType1
	34	BsmtFinSF1
	35	BsmtFinType2
	36	BsmtFinSF2
	37	BsmtUnfSF
	38	TotalBsmtSF
	47	BsmtFullBath
	48	BsmtHalfBath
Bath	47	BsmtFullBath
	48	BsmtHalfBath
	49	FullBath
	50	HalfBath
Bedroom	51	BedroomAbvGr
Kitchen	52	KitchenAbvGr
	53	KitchenQual
Fireplace	56	Fireplaces
	57	FireplaceQu
Garage	58	GarageType
	59	GarageYrBlt
	60	GarageFinish
	61	GarageCars
	62	GarageArea
	63	GarageQual
	64	GarageCond
Porch	66	WoodDeckSF
	67	OpenPorchSF
	68	EnclosedPorch
	69	3SsnPorch
	70	ScreenPorch
Pool	71	PoolArea
	72	PoolQC
Pavement	5	Street
	6	Alley
	65	PavedDrive
Year	19	YearBuilt
	20	YearRemodAdd
	76	MoSold
	77	YrSold
Indoor	9	Utilities
	39	Heating
	40	HeatingQC
	41	CentralAir
	42	Electrical
Outdoor	8	LandContour
	11	LandSlope
Overall Estimation	17	OverallQual
	18	OverallCond
