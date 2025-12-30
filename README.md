# Customer Churn Prediction

## Project Overview
Customer churn is a critical business problem where organizations aim to identify customers who are likely to stop using their services. This project focuses on predicting customer churn using machine learning techniques on a telecom dataset. The objective is to help businesses proactively retain customers by identifying churn risks early.

---

## Objectives
- Perform exploratory data analysis (EDA) to understand churn patterns  
- Build and compare classification models  
- Evaluate models using business-relevant metrics  
- Identify key factors influencing customer churn  

---

## Dataset
- **Source:** Telco Customer Churn Dataset  
- **Total Records:** ~7,000 customers  
- **Target Variable:** `Churn` (Yes / No)

### Key Features
- Customer tenure  
- Contract type  
- Monthly and total charges  
- Payment method  
- Service usage information  

---

## Exploratory Data Analysis
Key insights from EDA:
- Customers with month-to-month contracts show significantly higher churn  
- Higher monthly charges are associated with increased churn  
- Long-tenure customers are less likely to churn  

Basic visualizations such as churn distribution and monthly charges comparison were used to identify these trends.

---

## Data Preprocessing
- Converted `TotalCharges` to numeric format  
- Removed missing values  
- Dropped non-informative columns (customer ID)  
- Encoded categorical variables using Label Encoding  
- Applied feature scaling using StandardScaler  

---

## Models Implemented

### Logistic Regression
- Used as a baseline model  
- Simple and interpretable  

### Random Forest Classifier
- Handles non-linear relationships  
- Robust to feature interactions  
- Used as the primary model  

---

## Model Evaluation
Models were evaluated using the following metrics:
- **Accuracy**
- **Recall** (important for identifying churners)
- **ROC-AUC Score**

The Random Forest model outperformed Logistic Regression across all evaluation metrics, making it more suitable for churn prediction.

---

## Results Summary

| Model | Accuracy | Recall | ROC-AUC |
|------|----------|--------|--------|
| Logistic Regression | Moderate | Moderate | Good |
| Random Forest | Higher | Higher | Better |

*Exact metric values may vary slightly due to random state initialization.*

---

## Business Insights
- Contract type and tenure are the strongest predictors of churn  
- Customers on short-term contracts require proactive engagement  
- Pricing strategy plays a crucial role in customer retention  

---

## Conclusion
This project demonstrates how machine learning models can effectively identify customers at risk of churn. The insights generated can assist businesses in designing targeted retention strategies, reducing revenue loss, and improving customer satisfaction.

---

## Future Enhancements
- Hyperparameter tuning with cross-validation  
- Implementation of advanced models such as XGBoost  
- Deployment using Streamlit or Flask  
- Cost-sensitive learning to improve churn recall  

---

## Author
**Gitesh Patil**  
Data Science Intern
