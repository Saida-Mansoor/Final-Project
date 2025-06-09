# 🏠 Airbnb Rental Price Prediction – NYC  
## *Data Science Case Study*

> A machine learning project to predict optimal Airbnb listing prices in New York City using Python, Scikit-learn, and XGBoost.

---

## 🔍 Project Overview

This project aims to develop a predictive machine learning model that helps Airbnb hosts in New York City determine competitive and profitable listing prices. The model leverages features such as property type, room type, location, availability, and guest reviews to make accurate price predictions.

The dataset contains over **27,000 listings** with **23 features**, including host information, property characteristics, geographic coordinates, and review scores.

Several regression models were trained and evaluated:
- Linear Regression
- Lasso & Ridge Regression (with regularization)
- Random Forest Regressor
- XGBoost Regressor

Among these, **XGBoost achieved the best performance with a test R² score of 98%**, indicating strong predictive accuracy.

---

## 📊 Key Features Engineered

| Feature Name             | Description |
|--------------------------|-------------|
| `price_per_person`       | Normalized price per person (`price / accommodates`) |
| `total_sleeping_capacity`| Estimated maximum number of guests (`beds * 2`) |
| `has_reviews`            | Binary flag indicating if the listing has any reviews |
| `distance_to_center`     | Euclidean distance from NYC center |
| `location`               | Combined city and state for geographic grouping |

---

## 🛠️ Tools & Technologies

- **Programming Language**: Python
- **Libraries Used**:
  - `pandas`, `numpy` – For data manipulation
  - `matplotlib`, `seaborn` – For visualization
  - `scikit-learn` – For preprocessing, model training, and evaluation
  - `xgboost` – For implementing the XGBoost regressor
- **Evaluation Metrics**:
  - R² Score
  - Root Mean Squared Error (RMSE)


---

## 📊 Results Summary

| Model              | Training R² | Test R² | RMSE (Test) |
|--------------------|-------------|---------|-------------|
| Linear Regression  | 87.26%      | 86.16%  | 32.26       |
| Lasso Regression   | 87.25%      | 86.16%  | N/A         |
| Ridge Regression   | 87.26%      | 86.16%  | N/A         |
| Random Forest      | 99.30%      | 94.90%  | 19.58       |
| **XGBoost (Best)** | **98.00%**  | **98.00%** | **~10**    |

---

## 📄 Final Report

A comprehensive 1–2 page case study report is included:
- [Final_Project_Report.pdf](Final_Project_Report.pdf)

---

