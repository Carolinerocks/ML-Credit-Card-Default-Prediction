# ML Credit Card Default Prediction

**1. Project Overview**  

This project aims to predict the probability of customer default payments using data mining techniques. Six machine learning models were implemented and compared based on their predictive accuracy and performance metrics. The dataset focuses on credit card customers in Taiwan.

**2. Dataset**  

The dataset contains information about customers' demographics, payment history, and financial behavior.  

Features:
- Demographic Information: Sex, Education, Marriage, Age
- Financial Data: Credit limit, bill amounts, and payment amounts
- Repayment Status: PAY_0 to PAY_6 (payment delays in months)
- Target Variable: DEFAULT (0 = Non-default, 1 = Default)

**3. Objective**  

To compare the predictive accuracy of six machine learning models and identify the most suitable model for predicting customer default payments.

**4. Tools and Libraries**  
The project was implemented using Python and the following libraries:  
- Data Preprocessing: pandas, numpy, scikit-learn
- Visualization: matplotlib, seaborn
- Modeling:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost
  - Neural Network
  - Support Vector Machine (SVM)

**5. Models Compared**

| **Model**                | **AUC-ROC** | **F1-Score** | **Accuracy** | **Log-Loss** | **Pros**                              | **Cons**                               |
|--------------------------|-------------|-------------|-------------|-------------|---------------------------------------|---------------------------------------|
| **Logistic Regression**  | 0.7216      | 0.4711      | 0.6852      | 0.6099      | Simple, interpretable results         | Limited performance on complex data   |
| **Decision Tree**        | 0.7537      | 0.5234      | 0.7773      | 0.5999      | Easy to interpret, handles non-linearity | Prone to overfitting without pruning |
| **Random Forest**        | 0.7596      | 0.5712      | 0.7675      | 0.5136      | Robust, reduces overfitting           | Slower training for large datasets    |
| **XGBoost**              | 0.7515      | 0.3705      | 0.6205      | 1.5154      | Powerful, effective on imbalanced data| High complexity, longer tuning time   |
| **Neural Network**       | 0.7631      | 0.4626      | 0.8176      | 0.4430      | Captures complex patterns             | Requires more data and tuning         |
| **SVM**                  | 0.7180      | 0.6576      | 0.6980      | 0.6110      | Effective on smaller datasets         | Computationally expensive             |


**6. Results and Conclusion**  

- Random Forest performed the best overall, achieving high accuracy and a balanced AUC-ROC score while avoiding overfitting.
- While the Neural Network showed competitive performance, it lacked interpretability for practical applications.
- Other models like Logistic Regression and Decision Tree offered simplicity but were less effective in predictive accuracy.

Final Recommendation: Random Forest is the optimal model for predicting customer default payments.

