# Human-Age-Prediction
Synthetic Data for Predicting Age Based on Health and Lifestyle Factors

## Overview

This project predicts human life expectancy using a synthetic dataset of demographic, health, and lifestyle factors. The objective is to explore the influence of genetic and environmental factors on longevity. Through rigorous exploratory data analysis (EDA) and modeling, we derived actionable insights for various stakeholders, including healthcare providers, government agencies, and insurance companies.

## Dataset

The dataset used is publicly available on [Kaggle](https://www.kaggle.com/datasets/abdullah0a/human-age-prediction-synthetic-dataset/code). It includes:

- **Target Variable:** Age (in years).
- **Demographics:** Gender, income, education level, BMI, etc.
- **Biometrics:** Blood pressure, cholesterol level, cognitive function, etc.
- **Lifestyle Factors:** Physical activity, smoking status, diet, stress levels, etc.

## Objective

- **Primary Goal:** Predict age based on a combination of features using machine learning models.
- **Secondary Goal:** Evaluate the relative impact of nature (genetic) versus nurture (environmental) factors.

---

## Methods and Workflow

### 1. Data Preprocessing
- **Handling Missing Values:** Interpreted missing values in categorical features as "None."
- **Feature Engineering:** Split combined attributes (e.g., `Blood Pressure (s/d)`) into separate columns.
- **Multicollinearity Check:** Removed correlated features like `Height` and `Weight` to avoid redundancy.
- **Outlier Detection:** Identified outliers using the IQR method but retained them as they represented natural variability.

### 2. Exploratory Data Analysis (EDA)
- Visualized feature distributions and identified skewness.
- Investigated the impact of nature vs. nurture factors on age prediction.

### 3. Modeling
We tested various machine learning models to predict age:
- **Random Forest**: Moderate performance, but prone to overfitting.
- **Gradient Boosting**: Improved performance but computationally intensive.
- **Artificial Neural Networks (ANN)**: Underperformed due to limited dataset size and complexity.
- **Linear Regression**: Best performance with:
  - **R² = 0.94**: Explained 94% of the variability in age.
  - **RMSE = 5.15 years**: Average deviation from actual age.

### 4. Key Insights
- Genetic features (e.g., bone density) were more predictive of age than lifestyle factors.
- However, lifestyle still plays a significant role in modulating health outcomes.

---

## Business Impacts & Insights for Stakeholders
- **Healthcare Providers:** Identify high-risk patients and design preventive programs.
- **Insurance Companies:** Improve underwriting practices and offer tailored wellness incentives.
- **Government Agencies:** Develop targeted public health campaigns based on influential factors.
- **General Public:** Raise awareness about how lifestyle choices influence aging.

---

## Repository Structure
- **Human_Age_Prediction.ipynb**: Main notebook for preprocessing, feature selection, and modeling.
- **Train.csv**: Input dataset.
- **Presentation.pdf**: Summary of project findings and insights.

---

## Future Work

- Explore ensemble models and advanced hyperparameter tuning for better accuracy.
- Incorporate external datasets to improve model robustness.
- Develop an interactive dashboard for real-time analysis and stakeholder engagement.

---

## Acknowledgments

This project was completed as part of the INSY662 course at McGill University, in collaboration with Madeleine Dinh, Alexandra Guion, Juliana Hubacova, and Boyang Wan.


