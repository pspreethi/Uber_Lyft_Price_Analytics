# Uber_Lyft_Price_Analytics

# README: Rideshare Data Analysis and Prediction Project

## Overview
This project provides a comprehensive analysis of rideshare data from Uber and Lyft, focusing on their dynamic pricing models and other influential factors such as weather, distance, and time. Using a dataset collected from Boston, the project examines market dynamics, customer behavior, and predictive modeling of ride prices. The primary goal is to understand the factors driving pricing and demand while identifying the most effective models for price prediction.

---

## Table of Contents
1. [Introduction](#introduction)  
2. [Dataset Overview](#dataset-overview)  
3. [Key Features](#key-features)  
4. [Data Preprocessing](#data-preprocessing)  
5. [Exploratory Analysis](#exploratory-analysis)  
6. [Predictive Modeling](#predictive-modeling)  
7. [Key Findings](#key-findings)  
8. [Conclusion](#conclusion)  
9. [References](#references)  

---

## Introduction
Ride-sharing services like Uber and Lyft have transformed urban mobility, providing convenience and flexibility for millions of riders. However, dynamic pricing strategies and environmental factors significantly influence ride prices. This project investigates the rideshare market, with an emphasis on understanding ride distribution, pricing factors, and the effectiveness of different predictive models.

---

## Dataset Overview
The dataset comprises **693,071 records** collected from Boston over November and December. It includes:
- Temporal details (timestamp, hour, day, month)
- Geographic markers (source, destination, latitude, longitude)
- Ride specifics (cab type, price, distance, weather conditions)

Source: [Kaggle Rideshare Dataset - Boston](https://www.kaggle.com/datasets/brllrb/uber-and-lyft-dataset-boston-ma)

---

## Key Features
- **Ride Distribution Analysis**: Distribution of rides across Uber and Lyft services.
- **Weather Impact**: Assessment of how weather conditions like rain and temperature influence pricing and demand.
- **Dynamic Pricing Models**: Exploration of surge pricing and its role in price fluctuations.
- **Predictive Modeling**: Comparison of multiple models, including Decision Trees, Random Forest, Gradient Boosting, and Neural Networks.

---

## Data Preprocessing
Key steps include:
- Cleaning and organizing columns, such as removing irrelevant data and consolidating product IDs.
- Handling missing values, particularly in critical variables like price.
- One-hot encoding of categorical variables (e.g., weather conditions).
- Feature selection using linear regression and backward elimination to identify the most relevant predictors.

---

## Exploratory Analysis
Insights include:
- **Temporal Trends**: Ride frequency peaks during commuting hours and late-night periods.
- **Weather Conditions**: Overcast weather is most common, while rain significantly impacts demand and pricing.
- **Distance and Price**: Longer distances generally result in higher prices, but variability is influenced by factors like surge pricing.

---

## Predictive Modeling
Several machine learning models were implemented and evaluated:
1. **Random Forest Regressor**: Achieved the best performance with high accuracy (R² = 0.965) and low error rates.
2. **Gradient Boosting Regressor**: Comparable performance to Random Forest with slightly better consistency.
3. **Decision Tree**: Moderate performance with higher error rates.
4. **Multilayer Perceptron Regressor**: Poor performance with a negative R² value, indicating overfitting or insufficient model complexity.
5. **Multiple Linear Regression**: Lowest performance due to the dataset's non-linear relationships.

---

## Key Findings
- **Surge Pricing and Distance**: Strongest predictors of ride prices.
- **Weather Impact**: While weather influences ride demand, its direct impact on pricing is minimal compared to other factors.
- **Model Effectiveness**: Ensemble models like Random Forest and Gradient Boosting outperformed simpler models in both accuracy and reliability.
- **Pricing Patterns**: Prices exhibit significant variation during adverse weather and peak hours, emphasizing the importance of dynamic pricing.

---

## Conclusion
This project highlights the complex interplay of factors influencing rideshare prices and demand. The findings demonstrate that ensemble models are the most effective for predicting ride prices in dynamic environments. Understanding these patterns provides valuable insights for both rideshare companies and consumers.

---

## References
1. [Uber Dynamic Pricing Model](https://www.uber.com/en-GB/blog/uber-dynamic-pricing/)  
2. [Kaggle Rideshare Dataset - Boston](https://www.kaggle.com/datasets/brllrb/uber-and-lyft-dataset-boston-ma)  
3. Brodeur, A., & Nield, K. (2018). *An empirical analysis of taxi, Lyft and Uber rides: Evidence from weather shocks in NYC.*  
4. Davis, L. (2024). *Lyft vs. Uber: What’s the Difference?*  

---

## How to Use
1. Clone this repository.  
2. Ensure Python and required libraries (e.g., pandas, sklearn, matplotlib, seaborn) are installed.  
3. Run the provided Jupyter notebooks for data preprocessing, exploratory analysis, and modeling.  
4. Modify the code to explore additional insights or improve model performance.

