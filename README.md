
# Customer Churn Prediction using Machine Learning

## Project Overview

This project analyzes telecom customer data to predict churn using machine learning techniques. It includes data preprocessing, exploratory data analysis (EDA), model building, evaluation, and visualization with Tableau.

---

## 1. Data Loading and Exploration

- Loaded dataset with `pandas`
- Checked dataset structure, null values, and basic statistics
- Cleaned missing values with median/mode imputation
- One-hot encoded categorical features

---

## 2. Exploratory Data Analysis (EDA)

- Visualized churn distribution
- Created correlation matrix to examine relationships
- Identified top correlated features with churn

**Churn Distribution:**  
![Churn Distribution](churn_distribution.png)

**Correlation Matrix:**  
![Correlation Matrix](correlation_matrix.png)

---

## 3. Tableau Dashboards for Business Insights

**Churn by Contract Type**  
Customers on **month-to-month contracts** are more likely to churn.  
![Churn by Contract](https://i.imgur.com/xCoPfbn.png)

**Monthly Charges and Churn**  
Customers with higher **monthly charges** tend to churn more.  
![Monthly Charges](https://i.imgur.com/ldLR8b4.png)

**Tenure and Churn Relationship**  
Customers with **shorter tenure** show a higher churn rate.  
![Tenure and Churn](https://i.imgur.com/k9IYcpD.png)

**Churn vs Service Usage**  
Lack of services like **Tech Support** or **Online Security** increases churn.  
![Service Heatmap](https://i.imgur.com/t6Jk5Hn.png)

> 👉 [View Full Dashboard on Tableau Public](#)

---

## 4. Feature Engineering & Preprocessing

- Handled class imbalance using **SMOTE**
- Scaled features with **StandardScaler**
- Split data into training and testing sets

---

## 5. Model Training & Tuning

Trained and optimized the following models:
- **Logistic Regression** with hyperparameter tuning
- **Random Forest Classifier** with grid search
- **Gradient Boosting Classifier** with tuning

---

## 6. Model Evaluation

Models were evaluated using:
- **Accuracy Score**
- **Confusion Matrix**
- **ROC-AUC Curve**

**Model Accuracy Comparison:**  
![Model Comparison](model_comparison.png)

**Confusion Matrices & ROC Curves:**  
- Logistic Regression: `confusion_matrix_Logistic Regression.png`, `roc_curve_Logistic Regression.png`  
- Random Forest: `confusion_matrix_Random Forest.png`, `roc_curve_Random Forest.png`  
- Gradient Boosting: `confusion_matrix_Gradient Boosting.png`, `roc_curve_Gradient Boosting.png`

---

## 7. Feature Importance

Feature importance from the best-performing model:

**Top 10 Important Features:**  
![Feature Importance](feature_importance.png)

---

## 8. Conclusion

- The best model (Gradient Boosting or Random Forest) achieved ~84% accuracy
- Top churn indicators include `Contract`, `MonthlyCharges`, `TechSupport`, and `Tenure`
- Tableau dashboards provided valuable business insights for stakeholders

---

## Next Steps

1. Deploy the model using Flask or FastAPI
2. Integrate Tableau dashboards in business reporting
3. Monitor model drift and retrain with fresh data
4. Use predictions for targeted customer retention campaigns

---

## Repository Contents

```
churn_prediction_project/
├── churn_prediction.py
├── churn_distribution.png
├── correlation_matrix.png
├── feature_importance.png
├── model_comparison.png
├── confusion_matrix_*.png
├── roc_curve_*.png
├── tableau_dashboards/ (optional)
└── README.md
```

---

## Author
**Your Name**  
📧 your.email@example.com  
🔗 [LinkedIn](#) | [Portfolio](#) | [Tableau Public](#)

---

## License
MIT License
