# Housing-price-prediction

This project aims to find the features which affect the house prices in US nationally. 

We have used the S&P Case-Schiller Home Price Index as a proxy for home prices [fred.stlouisfed.org/series/CSUSHPISA]

For start, we have taken 6 features (GDP, Mortgage Rate, Unemployment Rate, Federal Funds Rate, Personal Consumption Expenditure, House supply months) into consideration to see their impact on the house prices. Further the date column was also split into day, month and year columns to see their impact.

The data contains total 276 rows (12 for each year from 2000 - 2022) and 8 columns (including date and target variable column)

On analysing the data with the help of plots and graphs, we found out that PCE(Personal Consumption Expenditure) has a strong linear correlation with the target variable.
To verify this and find other features having high impact on target variable, we used 3 regression techniques namely Linear Regression, Random Forest Regression and Gradient Boosting Regression. 

We have used 80% of the data to train the model and rest 20% for testing purpose. 

GridSearchCV was used to tune the hyperparamaters for Random Forest Regression and Gradient Boosting Regression. 

When all the features were used we got r2 scores for linear regression, Gradient Boosting Regression and Random Forest Regression as 0.7970, 0.9899, 0.9709 respectively.

After dropping 3 features having least importance (namely DFF, UNRATE and MORTGAGE30US) we got r2 score values as 0.7309, 0.9758, 0.9835.

Further dropping 'day' and 'month' column, the r2 scores we get are 0.7643, 0.9599, 0.9832.

With only 3 features namely 'year', 'PCE' and 'UNRATE', we get r2 scores as 0.7738, 0.9878, 0.9761. 

The features were choosen based on backward feature selection technique and the feature importance graph from Random Forest Regressor.


