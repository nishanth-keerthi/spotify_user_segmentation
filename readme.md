# Spotify User Segmentation and Churn Prediction

This project explores user behavior on Spotify using a structured survey dataset collected from 522 individuals. The goal is to generate insights about user preferences, segment behaviors, and build predictive models to support business decisions such as premium subscription targeting and churn management.

## 📂 Project Structure

- **EDA**: Visualizes user demographics, music & podcast preferences, subscription behavior, and engagement patterns.
- **Churn Modeling**: Builds classification models (Logistic Regression, Random Forest) to predict likelihood of premium user churn.
- **Premium Subscription Intent** *(planned)*: Predicts whether users are willing to upgrade to Premium based on behavioral traits.
- **Segmentation & Risk Scoring**: Categorizes users into churn risk levels and visualizes those segments by age group and plan type.
- **Notebook-based workflow**: Clean separation between exploratory and predictive modeling steps for clarity and reproducibility.

## 📊 Dataset Description (View detailed info in dataset_info.md)

- Responses from 522 Spotify users covering age, gender, listening habits, podcast preferences, mood-based behavior, and subscription history.
- Data was collected via structured survey and made publicly available on Kaggle.

**Dataset Source**  
- **Author**: Meera Ajayakumar  
- **Link**: [Spotify User Behavior Dataset (Kaggle)](https://www.kaggle.com/datasets/meeraajayakumar/spotify-user-behavior-dataset/data)  
- **License**: Open for educational and research purposes

## 📌 Highlights

- Cleaned, transformed, and visualized 20+ survey variables
- Handled categorical encoding, null value imputation, and feature engineering
- Performed chi-square analysis to select important predictors
- Built and evaluated churn models using balanced class techniques
- Visualized churn risk distribution by age and plan type for actionable targeting

---

## 🚀 Future Work

- Predict likelihood of subscription upgrade (Premium conversion modeling)
- Explore unsupervised clustering for Spotify user personas
- Deploy churn prediction pipeline as a dashboard or API
