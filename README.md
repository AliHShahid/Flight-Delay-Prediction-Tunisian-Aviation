# AeroDelay Insights ✈️
### *Predicting Flight Delays for Tunisair Aviation (Zindi Competition)*

[![Competition: Zindi](https://img.shields.io/badge/Competition-Zindi-blue)](https://zindi.africa/competitions/tunisair-flight-delay-prediction)
[![Python: 3.10](https://img.shields.io/badge/Python-3.10-green)](https://www.python.org/)
[![ML: CatBoost](https://img.shields.io/badge/Model-CatBoost-orange)](https://catboost.ai/)
[![ML: XGBoost](https://img.shields.io/badge/Model-XGBoost-purple)](https://xgboost.ai/)

**AeroDelay Insights** is a machine learning solution developed to predict the arrival delay of flights for Tunisair. Predicting delays is critical for airline operations, affecting everything from crew scheduling to passenger satisfaction and fuel management.

---

## 📊 The Challenge
The goal was to predict the flight delay time (in minutes) based on historical flight data. 
- **Target Variable:** Arrival Delay (Target).
- **Metric:** Root Mean Squared Error (RMSE).

---

## 🛠️ Feature Engineering Strategy
A Senior Data Scientist's value is in the features. This project implements:
- **Temporal Features:** Extraction of day, month, hour, and day of the week to capture seasonal travel patterns.
- **Flight Categorization:** Grouping flights by airline codes and airport locations to identify "bottleneck" routes.
- **Lag Features:** Analysis of historical delay patterns to predict future occurrences.
- **Handling Missingness:** Sophisticated imputation of missing categorical and numerical flight data.

---

## 🤖 The Model Pipeline
I utilized an ensemble approach to achieve high predictive accuracy:
1. **CatBoost:** Specifically chosen for its superior handling of categorical flight data (Airports, Aircraft IDs).
2. **XGBoost:** Integrated for its gradient boosting efficiency on structured tabular data.
3. **Hyperparameter Tuning:** Optimized using a Randomized Search approach to minimize RMSE.


---

## 📈 Results & Impact
- **RMSE Performance:** Achieved a competitive score on the Zindi Leaderboard.
- **Key Insight:** Departure time and Aircraft age were identified as the highest predictors of arrival delay.

---

## 🚀 How to Run
```bash
# Clone the repo
git clone [https://github.com/AliHShahid/Flight-Delay-Prediction-Tunisian-Aviation.git](https://github.com/AliHShahid/Flight-Delay-Prediction-Tunisian-Aviation.git)

# Install dependencies
pip install pandas scikit-learn catboost xgboost matplotlib seaborn

# Open the Notebook
jupyter notebook Zindi_Flight_Delay_Prediction_Tunisair.ipynb
