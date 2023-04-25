# Advanced Regression Assignment - House price prediction


## Table of Contents
* [About the company](#About-the-company)
* [Problem Statement](#Problem-statement)
* [Conclusions](#Conclusions)   
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## About the company
Surprise Housing is a US-based housing company. They have decided to enter the Australian housing market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

## Problem statement
The company wants to know:
- Which variables are significant in predicting the price of a house, and
- How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression

Model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

Model built using linear regression is having a good r2 score for train data; but for test dat it was giving negative score
- Model performance by Ridge & lasso Regression is giving good r2 scores
- Model performance by Ridge & lasso Regression is giving good RMSE values
- Model built using Ridge regression is having 325 features, whereas the one built using Lasso is having only 53 features
- Lasso regression is helping here to eliminate unwanted features by 0 coeff. This helps to easily identify feature variables and keep it simple and robust
- Following variables are significant in predicting house price

    'GrLivArea', 'OverallQual', 'YearBuilt', 'TotalBsmtSF',
       'OverallCond', 'YearRemodAdd', 'GarageArea', 'BsmtFinSF1',
       'GarageCars', 'LotArea', 'BsmtQual_Ex', 'Neighborhood_Crawfor',
       'BsmtFullBath', 'Fireplaces', 'KitchenQual_Ex',
       'GarageType_Attchd', 'HeatingQC_Ex', 'BsmtFinType1_GLQ',
       'BldgType_1Fam', 'SaleType_New', 'Condition1_Norm',
       'Functional_Typ', 'WoodDeckSF', 'Neighborhood_ClearCr',
       'FireplaceQu_Gd', 'Exterior1st_BrkFace', 'Foundation_PConc',
       'LotConfig_CulDSac', 'GarageFinish_Fin', 'Neighborhood_Somerst',
       'Neighborhood_Veenker', 'Condition1_RRAe', 'Functional_Maj2',
       'PavedDrive_N', 'KitchenQual_TA', 'GarageFinish_Unf',
       'LotFrontage_153.0', 'BldgType_Twnhs', 'ExterQual_TA',
       'Functional_Sev', 'Exterior1st_BrkComm', 'Neighborhood_Edwards',
       'KitchenAbvGr', 'Condition1_Artery', 'LotFrontage_21.0',
       'SaleCondition_Abnorml', 'FireplaceQu_MISSING', 'CentralAir_N',
       'MSZoning_RM', 'MSZoning_C (all)', 'Condition2_PosN',
       'RoofMatl_ClyTile'
- To understand how well those variables describe the price of a house, use the following
log(SalePrice) = C + 0.13*GrLivArea + 0.092*OverallQual + 0.05*YearBuilt + 0.042*TotalBsmtSF + 0.027*OverallCond + 0.027*YearRemodAdd + 0.025*GarageArea + 0.022*BsmtFinSF1 + 0.019*GarageCars + 0.015*LotArea + 0.014*BsmtQual_Ex + 0.013*Neighborhood_Crawfor + 0.012*BsmtFullBath + 0.009*Fireplaces + 0.009*KitchenQual_Ex + 0.007*GarageType_Attchd + 0.006*HeatingQC_Ex + 0.006*BsmtFinType1_GLQ + 0.006*BldgType_1Fam + 0.006*SaleType_New + 0.006*Condition1_Norm + 0.005*Functional_Typ + 0.005*WoodDeckSF + 0.004*Neighborhood_ClearCr + 0.004*FireplaceQu_Gd + 0.004*Exterior1st_BrkFace + 0.003*Foundation_PConc + 0.002*LotConfig_CulDSac + 0.002*GarageFinish_Fin + 0.001*Neighborhood_Somerst + 0.001*Neighborhood_Veenker + -0.001*Condition1_RRAe + -0.001*Functional_Maj2 + -0.001*PavedDrive_N + -0.001*KitchenQual_TA + -0.002*GarageFinish_Unf + -0.002*LotFrontage_153.0 + -0.002*BldgType_Twnhs + -0.003*ExterQual_TA + -0.003*Functional_Sev + -0.004*Exterior1st_BrkComm + -0.004*Neighborhood_Edwards + -0.005*KitchenAbvGr + -0.006*Condition1_Artery + -0.008*LotFrontage_21.0 + -0.009*SaleCondition_Abnorml + -0.011*FireplaceQu_MISSING + -0.011*CentralAir_N + -0.02*MSZoning_RM + -0.024*MSZoning_C (all) + -0.045*Condition2_PosN + -0.06*RoofMatl_ClyTile + Error term(RSS + alpha * (sum of absolute value of coefficients)

## Technologies Used
- python
- pandas library
- matplotlib library
- missingno library
- numpy library
- seaborn library
- sklearn library
- statsmodels library

## Acknowledgements
Give credit here.
- This project was inspired by upGrad's assignment
