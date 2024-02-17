# Increasing_Revenue_NYC_TLC

# Overview
The goal of this project was to construct a suite of models to improve operations and revenue of the New York City Taxi and Limousine Commission. A multiple linear regression model was developed to predict fare amounts based on ride duration and distance. A random forest model was constructed to predict whether a rider would be a generous tipper (>20% of fare tip). 

# Business Understanding
This NYC TLC consists of many employees. This data coems from 200,000 licensees and over one million trips. With mean one bedroom apartment rent in NYC costing $4100 per month, and mean taxi driver salary at $45,500, this project was designed to increase revenue of the NYC TLC and its drivers, to help drivers better afford necessities of daily living. 

# Data Understanding
The data was collected byt the NYC TLC, and the dataset consists of 408,294 rows, and is part of a larger dataset of about 117 million rows. There are 18 columns, with variables such as pickup and dropoff points, number of passengers, payment type, fare amount, tip amount, pickup time and dropoff time. Somne variables were engineered into new ones, including mean duration and distance for every pickup/dropoff combination, a binary column indicating whether a rider was a generous tipper, and a column indicating whether a ride was during am/pm rush hour or not. 

# Modeling and Evaluation
A linear regression model was built to predict fare amount using features of the dataset. This model achieved an r^2 of 0.87, an MAE of 2.12, and an MSE of 14.2. This model explains 87% of the variation in fare amount. A suite of machine learning models was constructed to see which would most accurately predict those riders who would be a generous tipper. The champion model was an xgboosted forest, which was able to positively classify 82% of all generous tippers in the test dataset. The plot below illustrates the most important features in these predictions.

<a href="url"><img src="https://github.com/bjkoewler/Increasing_Revenue_NYC_TLC/blob/main/images/feature_importances.png" align="justify" height="500" width="500" ></a>

# Conclusion
These models will help to increase the operations and revenue of NYC TLC and its drivers, and will help provide pricing transparency to riders. Recommendations include tracking tipping behavior across rides per rider, investigating why Vendor 2 solicits more generous tips, and using the MLR model to build an algorithm into an app that would allow potential riders to see fare price before calling a cab.
