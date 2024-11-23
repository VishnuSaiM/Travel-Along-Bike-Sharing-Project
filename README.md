# Travel-Along-Bike-Sharing-Project  🚴‍♂️
Bike-Sharing Demand Prediction

**# Bike Sharing Demand Prediction**



## 🎯** Overview**
This project focuses on predicting bike-sharing demand for 'Travel Along', a bike-sharing company, using machine learning techniques. The goal is to help the company optimize its operations and improve customer service by accurately forecasting bike rental demand based on various environmental and temporal factors.

## ** 🚲 Problem Statement**
'Travel Along' needs to:
- Predict the number of bikes that will be rented on an hourly basis
- Identify key factors affecting bike rental patterns
- Develop strategies for managing demand surges
- Optimize bike allocation across different stations

**## 📊 Dataset Information**
The dataset contains bike rental information spanning 2 years with the following features:
- Temporal: date, hour, weekday, holiday, working day
- Environmental: weather conditions, temperature, humidity, windspeed
- Target Variable: count of total rental bikes (casual + registered users)

**### Features Description:**
- `dteday`: Date
- `season`: Season (1:spring, 2:summer, 3:fall, 4:winter)
- `yr`: Year (0:2011, 1:2012)
- `mnth`: Month (1-12)
- `hr`: Hour (0-23)
- `holiday`: Whether it's a holiday
- `weekday`: Day of the week
- `workingday`: Working day indicator
- `weathersit`: Weather situation (1: Clear - 4: Heavy Rain)
- `temp`: Normalized temperature in Celsius
- `atemp`: Normalized feeling temperature
- `hum`: Normalized humidity
- `windspeed`: Normalized wind speed
- `casual`: Count of casual users
- `registered`: Count of registered users
- `cnt`: Total count of bikes rented

**## 🛠️ Technical Stack**
- **Programming Language:** Python 3.x
- **Libraries:**
  - Data Manipulation: Pandas, NumPy
  - Visualization: Matplotlib, Seaborn
  - Machine Learning: Scikit-learn
  - Gradient Boosting: XGBoost
- **Models Implemented:**
  - Decision Trees
  - Random Forest
  - AdaBoost
  - Gradient Boosting
  - XGBoost
  - Stacking Regressor



**## 🔍 Key Findings**
1. **Temporal Patterns:**
   - Peak rental hours: Morning (8-9 AM) and Evening (5-6 PM)
   - Higher demand on working days
   - Seasonal variations with peak in summer

2. **Weather Impact:**
   - Clear weather shows highest rental numbers
   - Significant drop during adverse weather conditions
   - Temperature has strong positive correlation with rentals

**## 📈 Model Performance**
Model performance on test data:

| Model | R2 Score | RMSE |
|-------|----------|------|
| Gradient Boost (Tuned) | 95.5% | 39 |
| XGBoost | 94.8% | 41 |
| Stacking Regressor | 94.5% | 42 |

**## 💡 Business Recommendations**
1. **Dynamic Pricing Strategy:**
   - Implement surge pricing during peak hours
   - Offer discounts during off-peak hours

2. **Inventory Management:**
   - Optimize bike distribution based on temporal patterns
   - Maintain larger fleet availability during summer months

3. **Weather-based Planning:**
   - Implement weather-based demand forecasting
   - Develop contingency plans for adverse weather conditions



## 📝 License
This project is licensed under the MIT License -.
