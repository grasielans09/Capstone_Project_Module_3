# **Customer Lifetime Value Prediction**

## **Project Overview**
This project focuses on building and optimizing machine learning models to predict **Customer Lifetime Value (CLV)**. CLV is an essential metric for businesses to evaluate the potential revenue a customer will generate over time. By leveraging machine learning, this project aims to provide actionable insights that help improve customer retention strategies and maximize profitability.

---

## **Project Objectives**
1. Predict the Customer Lifetime Value (CLV) accurately using machine learning techniques.
2. Identify the key factors that influence CLV using feature importance analysis.
3. Optimize model performance through feature selection and hyperparameter tuning.
4. Evaluate and compare different regression models on metrics like RMSE, MAE, MAPE, and R-squared.
5. Visualize residuals and analyze model biases for better interpretability.

---

## **Features**
- **End-to-End Workflow**:
  - Data preprocessing (handling missing values, encoding categorical data, scaling).
  - Feature engineering (selection based on feature importance).
  - Model training, tuning, and evaluation.
- **Multiple Regression Models**:
  - Random Forest Regressor
  - XGBoost Regressor
  - AdaBoost Regressor
- **Hyperparameter Optimization**:
  - Conducted using `RandomizedSearchCV` for models like Random Forest and XGBoost.
- **Residual Analysis**:
  - Compare model performance before and after feature selection using residual plots.

---

## **Model Performance**
### **Model Evaluation Summary**
| **Model**                                 | **RMSE**  | **MAE**  | **MAPE** | **R-squared (R²)** |
|-------------------------------------------|-----------|----------|----------|--------------------|
| Random Forest Regressor (After Tuning)    | 3989.68   | 1798.11  | 0.1423   | 0.6706             |
| Random Forest with Feature Selection      | 3978.76   | 1821.24  | 0.1474   | 0.6724             |
| XGBoost Regressor (After Tuning)          | 4030.13   | 1812.67  | 0.1494   | 0.6639             |
| AdaBoost Regressor (After Tuning)         | 4048.04   | 1757.52  | 0.1339   | 0.6609             |

### **Key Observations**:
- Random Forest Regressor with feature selection achieved the best R-squared value (0.6724) and lowest RMSE (3978.76), indicating better accuracy and fit.
- Feature selection reduced noise and improved model interpretability while maintaining performance.

---

## **Visualizations**
Residual plots were generated to analyze model errors. The plots show how residuals are distributed across predictions before and after feature selection, providing insights into model bias and variance.

---

## **How to Use**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/customer-lifetime-value.git
   cd customer-lifetime-value
