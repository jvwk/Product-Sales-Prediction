# Product-Sales-Prediction
Prediction of product sales based on various independent underlying features

***Jaco van Wyk***

<br>
<br>

## Overview

In order to assess future sales, regression techniques were employed based on the available data. The data included:

| Data description |
----- |
|	Unique product ID
|	Weight of product
|	Whether the product is low fat or regular
|	The percentage of total display area of all products in a store allocated to the particular product
|	The category to which the product belongs
|	Maximum Retail Price (list price) of the product
|	Unique store ID
|	The year in which store was established
|	The size of the store in terms of ground area covered
|	The type of area in which the store is located
|	Whether the outlet is a grocery store or some sort of supermarket
|	Sales of the product in the particular store. This is the target variable to be predicted.

<br>
<br>

## Data

From exploratory data analysis it can be seen that the maximum retail price and item outlet sales are positively correlated:

![MRP v IOSales](https://github.com/jvwk/Product-Sales-Prediction/assets/138116044/91f4d5f1-b6d5-4e1c-90fa-d3f46645f413)

Similarly, outlet type is expected to be a predictor of item outlet sales:

![Outlet type v IOSales](https://github.com/jvwk/Product-Sales-Prediction/assets/138116044/255f1cc9-1fd6-4352-90d0-042641378444)

<br>
<br>

## Model

Ultimately a Random Forest model was employed, with hyperparameter tuning. It displayed the following regression metrics for the test data:

Metric | Value
--- | ---:
Mean Absolute Error | 737
Mean Square Error | 1,115,237
Root Mean Square Error | 1,056
R<sup>2</sup> | 0.596

<br>
<br>

## Recommendation

It is recommended that the Random Forest model with hyperparameter tuning is employed for predicting item outlet sales. Continued refinement of the model, and possible alternative models, can be investigated as more data becomes available.
