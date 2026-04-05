HOUSE PRICE PREDICTION

This project walks through a complete machine learning pipeline to predict residential house prices using the California Housing dataset, 
which contains 20,640 records across 9 features including location coordinates, housing age, room counts, household size, and median income. 
The workflow covers data inspection, exploratory data analysis (EDA), feature engineering, preprocessing, and model training. 
Three new features were created from the raw data — rooms per household, bedrooms per room, and population per household — alongside a log-transformation of the target variable to correct for its right-skewed distribution. 
Four models were trained and compared using 5-fold cross-validation: Linear Regression, Ridge Regression, Random Forest, and Gradient Boosting.

Gradient Boosting Regressor was the best, achieving an R² of 0.8316 on the hold-out test set — meaning it explains 83.16% of the variation in house prices — with a Mean Absolute Error of $32,200 and an RMSE of $49,708.
Feature importance analysis revealed that median income alone drives 54.5% of all predictive power, followed by geographic coordinates (longitude and latitude together at ~27%), 
confirming that where a house is and how wealthy its residents are remain the two dominant factors in California housing prices.
The engineered ratio features contributed a meaningful combined ~15%, validating the feature engineering step.
