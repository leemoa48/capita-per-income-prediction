# capita-per-income-prediction
This repository is for predicting the capita per income in Canada. It is a machine learning project that uses linear regression model.

# 📈 Per Capita Income Prediction

This project focuses on predicting **Per Capita Income** over time using a simple regression model. The dataset includes **annual per capita income data** for India from **1970 to 2020**, and the model forecasts income for future years.

---

## Objective

To build a **Linear Regression** model that learns the relationship between **year** and **per capita income**, and use it to predict future income values.

---

## Dataset Overview

- **Features**:
  - `year`: Year (1970–2020)
  - `per capita income (US$)`: Income per person in USD

- **Total Records**: 51 rows

---

## Exploratory Data Analysis (EDA)

### 🔹 Trend

- The data shows a **steady upward trend** in per capita income over time.
- Growth is **nearly linear**, which supports the use of a linear regression model.

### Visualization

- A scatter plot with a regression line shows a **strong positive correlation** between year and income.

---

## Preprocessing

- Converted `year` column into numeric format using `.values.reshape(-1, 1)` to prepare it for model training.
- No missing values or outliers were found.
- Data was clean and required minimal transformation.

---

## Model Used

- **Linear Regression** (from `scikit-learn`)

### Why Linear Regression?

- Due to the linear nature of the income increase over time, linear regression fits the data well with minimal complexity.

---

## Model Evaluation

- **R² score** (coefficient of determination): High, indicating good fit.
- The model was tested by predicting the income for the year **2020**:
   **Actual**: \$1,883.00
   **Predicted**: Close to actual with minimal error

---

## Predictions

- The model can be used to **predict income for future years**, e.g., 2025, 2030, etc.
