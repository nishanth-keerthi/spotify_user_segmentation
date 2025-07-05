# Spotify User Segmentation and Churn Prediction

This project explores Spotify user behavior using a structured survey dataset of 522 respondents. It covers exploratory analysis, churn prediction, premium subscription modeling, user segmentation, and explainable AI techniques to uncover behavioral insights that can inform business decisions.

---

## 📁 Project Overview

| Module | Description |
|--------|-------------|
| `01_eda.ipynb` | Comprehensive exploratory data analysis including user demographics, listening patterns, content preferences, and subscription behaviors. |
| `02_Churn_Analysis.ipynb` | Predicts which Premium users are likely to churn using models like Logistic Regression and Random Forest with class imbalance handling and feature importance analysis. |
| `03_Premium_Intent_Prediction.ipynb` | Predicts which Free users are likely to upgrade to Premium using models like XGBoost and SVM, with probability segmentation and SHAP-based explainability. |
| `datasets/` | Contains raw survey data, cleaned processed data, label encoding mappings, and model-ready datasets. |
| `dataset_info.md` | Details the original survey dataset, question mappings, and variable descriptions. |

---

## 📊 Dataset Description (Full details in `dataset_info.md`)

- Collected via structured survey of 522 Spotify users.
- Covers age, gender, platform usage, moods, music/podcast habits, subscription type, and willingness to upgrade to Premium.
- Cleaned, encoded, and enriched with additional features for modeling.

**Source**  
- Author: Meera Ajayakumar  
- Dataset: [Spotify User Behavior on Kaggle](https://www.kaggle.com/datasets/meeraajayakumar/spotify-user-behavior-dataset/data)

---

## 🧠 Key Features & Analysis

### ✅ Exploratory Data Analysis (EDA)
- Distribution of users by age, gender, and device
- Preferred content (music vs podcast), genres, and listening time slots
- Subscription plan breakdown (Free vs Premium) and pricing patterns
- Mood-based music behavior and frequency clusters
- Chi-square analysis to assess relationships between predictors and outcomes

### ✅ Churn Analysis (Premium Users)
- Models used: Logistic Regression (with class_weight), Random Forest
- Handled class imbalance using stratification and class weighting
- Precision-recall trade-off evaluated for churner detection
- Feature importance plots and risk segmentation by age group and plan type
- Churn probability prediction with grouping into Low, Medium, High risk segments

### ✅ Premium Subscription Intent Prediction (Free Users)
- Models used: Random Forest, Support Vector Machine (SVM), XGBoost
- Predicts likelihood of a free user upgrading to Premium
- Stratified train-test split with imbalanced classification handled
- Predicted probabilities visualized and segmented into conversion tiers
- Confusion matrix and classification metrics interpreted from a business lens

### ✅ Explainability with SHAP
- Global feature importance via SHAP values for XGBoost model
- SHAP summary and beeswarm plots for behavioral understanding
- Local prediction explanations with waterfall plots for individual users
- Key drivers: plan type, listening frequency, usage lifetime, mood, and exploration method

---

## 📌 Summary of Business Insights

- Users preferring Family plans or dissatisfied with podcasts are more likely to churn.
- Churn risk is elevated for certain age groups and plan types (e.g., Students).
- Free users most likely to convert have distinct listening habits and value personalization.
- Models are optimized for high recall on churners and converters to support intervention strategies.
- SHAP helps uncover transparent explanations of predictions for business stakeholders.

---

## 📈 Results

- Churn Model Accuracy: ~97% (Random Forest), with excellent churner recall
- Premium Intent Model Accuracy: ~80% (XGBoost), with balanced performance
- Feature Importance consistently highlighted pricing sensitivity, plan type, content preference, and engagement patterns

---

## 🚀 Future Work

- Deploy models as REST APIs or dashboards for product teams
- Perform unsupervised clustering for Spotify user personas
- Conduct A/B experiments on predicted High-Risk/High-Intent users
- Extend SHAP to include interaction values or temporal components (if timestamped data is available)
