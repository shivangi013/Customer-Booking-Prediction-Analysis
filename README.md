# Customer Booking Prediction Analysis

## Project Overview
This project focuses on analyzing and predicting customer booking completion using a machine learning model. The dataset contains booking information with various features related to customer behavior and flight details.

## Problem Statement
The goal is to predict whether a customer will complete their booking using relevant features. The dataset is highly imbalanced, with approximately 85% of cases where customers do not complete their booking.

## Key Insights
- **Target Variable Distribution:**
  - 85% of bookings are incomplete (booking_complete = 0).
  - Only 15% of customers complete their bookings.
- **Feature Importance:**
  - Significant Features: `Purchase Lead`, `Route`, `Flight Hour`, `Length of Stay`, `Booking Origin`
  - Passenger preferences like `extra baggage`, `preferred seat`, and `in-flight meals` have lesser importance.
  - Strong interaction effect between `Num Passengers` and `Sales Channel`.
- **SHAP Interaction Effects:**
  - Average `Purchase Lead`: 84.94 days before flight.
  - Average `Length of Stay`: 23.04 days.
  - Most flights are scheduled around **9 AM**.
  - **66.9%** passengers carried extra baggage.

## Model Performance
- **Accuracy:** 85.15%
- **Classification Report:**
  - Precision for `booking_complete = 1`: 44%
  - Recall for `booking_complete = 1`: 7%
- **Confusion Matrix:**
  - True Negatives: 1682
  - False Positives: 27
  - False Negatives: 270
  - True Positives: 21

## Tools & Technologies Used
- **Python** for data analysis and modeling
- **Pandas** and **NumPy** for data manipulation
- **Matplotlib** and **Seaborn** for data visualization
- **Scikit-Learn** for model building
- **SHAP** for model interpretability

## Next Steps
- Address class imbalance using SMOTE or other resampling techniques.
- Experiment with alternative models (e.g., XGBoost, SVM).
- Improve feature engineering.

## Contact
For any inquiries, please reach out via GitHub Issues.

---
**Author:** Shivangi Singal


