# Data-Driven-Price-Intelligence-for-Airbnb-Marrakes

This repository cexplores Airbnb listing data in Marrakesh to understand key factors influencing rental prices and to build predictive models for price estimation. After extensive data cleaning and feature engineering, statistical analyses and machine learning models — particularly tree-based regressors — were applied to uncover insights and forecast listing prices with high accuracy. A Power BI dashboard was also developed to visually communicate pricing trends and market segments, offering valuable intelligence to hosts, investors, and hospitality stakeholders.



## 📌 Project Summary

- **Objective**: Analyze Airbnb data to identify price-influencing features and develop robust predictive models.
- **Tools Used**: Python (Pandas, Scikit-learn, Seaborn, XGBoost), Power BI for visualization
- **Machine Learning**: 17 regression models evaluated, top-performing: ExtraTreesRegressor (R² = 1.0000)
- **Outcome**: Insights into pricing patterns, market segmentation, and a predictive engine with high accuracy.

---

## 📂 Table of Contents

- [Dataset Overview](#dataset-overview)
- [Data Preparation](#data-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Predictive Modeling](#predictive-modeling)
- [Key Findings](#key-findings)
- [Power BI Dashboard](#power-bi-dashboard)
- [How to Run](#how-to-run)
- [Results & Business Insights](#results--business-insights)
- [Future Improvements](#future-improvements)

---

## 📊 Dataset Overview

- **Source**: Airbnb listings dataset for Marrakesh (3,660 records, 29 initial features)
- **Variables**: Includes price, location, reviews, amenities, and descriptive features

---

## 🛠️ Data Preparation

- **Missing Value Handling**: Dropped or imputed based on relevance
- **Outlier Treatment**: Used IQR-based capping for price (above $562.50)
- **Final Feature Set**: 49 features after creation of indicators for:
  - Amenity counts
  - Luxury title flags
  - Pool availability
  - Price tiers
  - Location and property descriptions

---

## 📈 Exploratory Data Analysis

- Distribution: Strong right-skewed price distribution
- Room Type Insights: "Entire home/apt" most common and highest priced
- Capacity vs Price: Positive correlation, especially for 10+ guests
- SuperHost Listings: Slight price premium observed
- Correlation Analysis: High correlation with luxury indicators and pool availability

---

## 🧠 Predictive Modeling

- **Models Tested**: Linear Regression, Ridge, Lasso, RandomForest, GradientBoosting, ExtraTrees, XGBoost, etc.
- **Top Model**: `ExtraTreesRegressor`
  - R²: 1.000
  - MAE: 0.1186
  - MAPE: 0.0007
  - RMSE: 0.3510
- **Model Evaluation**: Tree-based models vastly outperformed linear methods

---

## 📌 Key Findings

- **Property type and capacity** affect market segmentation
- **Hosts with SuperHost status** enjoy moderate price premiums
- **Price prediction is highly reliable** based on physical attributes

---

## 📊 Power BI Dashboard

An interactive Power BI dashboard complements the analysis and provides:
- Price trends by room type and capacity
- Location-based insights
- Price outlier impact visualization
- Amenity-driven filtering and analysis

> **Note**: Power BI `.pbix` file is available upon request or can be added in a separate branch.

---

## ▶️ How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/ZubairKhan87/Data-Driven-Price-Intelligence-for-Airbnb-Marrakes.git
   cd Data-Driven-Price-Intelligence-for-Airbnb-Marrakes
