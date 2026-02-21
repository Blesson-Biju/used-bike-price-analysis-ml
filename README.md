# used-bike-price-analysis-ml
Machine Learning and Power BI analysis on used bike resale pricing.

📌 Used Bike Price Analysis & Prediction
🔍 Project Overview

This project focuses on analyzing used bike resale data and building a machine learning model to predict bike prices based on multiple influencing factors.

The objective was to:

Clean and preprocess raw real-world data

Perform exploratory data analysis (EDA)

Engineer meaningful features

Build and evaluate machine learning models

Develop an interactive Power BI dashboard for business insights

📊 Dataset Information

Total Records: 7,857

Original Features: 8

Raw Dataset Issues:

Missing values

Mixed units (bhp, hp, ps, kw)

Text in numeric columns

Outliers and inconsistent entries

Original Features:

model_name

model_year

kms_driven

owner

location

mileage

power

price

🛠 Data Preprocessing & Feature Engineering

The following steps were performed in Python (Google Colab):

Cleaned and standardized kms_driven

Converted mileage to numeric format

Standardized power values into BHP

Extracted brand from model_name

Extracted engine capacity (CC)

Created new feature: bike_age

Handled missing values

Removed inconsistent records

Final cleaned dataset was prepared for modeling.

📈 Exploratory Data Analysis (EDA)

Key insights discovered:

Newer bikes tend to have higher resale value.

Higher kilometers driven generally reduces price.

Premium brands retain resale value better.

First-owner bikes are priced higher.

Price distribution is positively skewed.

🤖 Machine Learning Model
Target Variable:

price

Data Preparation:

Categorical encoding (One-Hot Encoding)

Train-Test Split (80:20)

Algorithms Used:

Linear Regression

Ridge / Lasso Regression

Random Forest (if used)

Evaluation Metrics:

R² Score

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

The model was evaluated to measure prediction accuracy and generalization performance.

📊 Power BI Dashboard

An interactive Power BI dashboard was created to visualize insights.

Dashboard Features:

Price by Brand

Price by Model Year

Owner Type Distribution

Mileage vs Price (Scatter Plot)

Location-based Filtering

KPI Cards (Average Price, Total Listings)

The dashboard enables dynamic filtering and comparative analysis.

🧰 Tools & Technologies

Python

Pandas

NumPy

Matplotlib / Seaborn

Scikit-learn

Power BI

Google Colab

🚀 Future Improvements

Advanced hyperparameter tuning

Testing additional ML models (XGBoost)

Log transformation for skewed price distribution

Deployment as a web-based prediction tool

Integration with live marketplace data
