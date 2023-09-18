# Housing-price-prediction

This project aims to find the features which affect the house prices in US nationally. 

We have used the S&P Case-Schiller Home Price Index as a proxy for home prices [link](fred.stlouisfed.org/series/CSUSHPISA]

For start, we have taken 6 features (GDP, Mortgage Rate, Unemployment Rate, Federal Funds Rate, Personal Consumption Expenditure, House supply months) into consideration to see their impact on the house prices.

The data contains total 276 rows (12 for each year from 2000 - 2022) and 8 columns (including date and target variable column)

On analysing the data with the help of plots, we found out that PCE(Personal Consumption Expenditure) has a strong linear correlation with the target variable.
To verify this and find other features having high impact on target variable, we used 3 regression techniques namely Linear Regression, Random Forest Regression and Gradient Boosting Regression. 
