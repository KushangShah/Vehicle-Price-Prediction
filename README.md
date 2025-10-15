# Vehicle Price Prediction
<img src="images/banner.png">

###### Project 2: From Unified Mentors [Internship]

## Problem Statement
The objective of this project is to develop a machine learning model capable of accurately predicting the price of vehicles based on various features such as make, model, year, mileage, engine characteristics, fuel type, transmission, body style, and other relevant attributes. Accurate price prediction is crucial for stakeholders in the automotive industry, including dealerships, buyers, and financial institutions, to make informed decisions regarding pricing, inventory management, and valuation.

## Project Summary
This project focused on building a machine learning model to predict vehicle prices using a dataset containing information like make, model, year, price, engine details, fuel type, transmission, and body style.

## Data Preparation & Exploratory Data Analysis (EDA)
- Handled missing values (median for numerical, mode for categorical) and removed duplicates.
- Capped outliers using IQR to prevent skewed results.
- Explored data through visualizations:
  - Numerical feature distributions
  - Popular makes (Jeep, Dodge, RAM)
  - Common body types (SUV, Pickup)
  - Price variations across categories
- Observed weak correlations between most numerical features, except for a moderate positive correlation between price and cylinders.
- Hypothesis testing confirmed a significant negative correlation between mileage and price and an association between fuel type and transmission.

## Feature Engineering & Preprocessing
- Created new features: `price_category`, `brand`, `age`, `engine_cylinders`, and `mileage_year_interaction`.
- Applied one-hot encoding for categorical variables and standard scaling for numerical features.
- Split data into training and testing sets.

## Modeling & Evaluation
- Tested multiple regression models: Linear Regression, Ridge, Lasso, Random Forest, and Gradient Boosting.
- Tuned Ridge and Random Forest using GridSearchCV.
- Best model: Tuned Ridge Regression achieved R² = 0.890 and MAE ≈ 3,898, showing strong predictive performance.

<img src="images/Model performance.png">

## Conclusion
The project successfully built a vehicle price prediction model. Data cleaning, EDA, and feature engineering were crucial in preparing the data. The tuned Ridge model provides accurate price predictions and can be applied in pricing strategies, inventory planning, and financial forecasting.

## License
This project is licensed under the MIT License.