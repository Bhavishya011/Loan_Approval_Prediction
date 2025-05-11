🏦 Loan Approval Prediction

A machine learning project to predict whether a loan will be approved based on applicant details, financial data, and credit history. We used various models including Random Forest, Decision Tree, Logistic Regression, and its regularized variants to evaluate and compare performance.

---

## 👨‍💻 Team Members

* **Bhavishya Jain**
* **Mehul Shah**
* **Soumya Jain**

---

## 📊 Dataset Overview

The dataset includes:

* Personal information (e.g., gender, marital status, dependents)
* Financial indicators (e.g., applicant income, co-applicant income, loan amount)
* Credit details (e.g., CIBIL score, assets)
* Target variable: `Loan Status` (Approved/Rejected)

---

## 🔍 Key Features Engineered

* **Movable Assets** = bank assets + luxury assets
* **Immovable Assets** = residential assets + commercial assets
* **Net Income** = applicant income + co-applicant income

Categorical variables were label-encoded, and missing values were handled appropriately.

---

## 📈 Exploratory Data Analysis (EDA)

* Boxplots and violin plots for income, CIBIL score, and loan status
* Correlation heatmap of features
* Count plots for categorical variables
* Scatter plots for loan amount vs other financial features

---

## 🤖 Machine Learning Models Used

| Model               | Accuracy   | AUC Score | Log Loss |
| ------------------- | ---------- | --------- | -------- |
| Decision Tree       | Overfitted | \~0.75    | –        |
| Random Forest       | Excellent  | \~0.83    | –        |
| Logistic Regression | Good       | \~0.79    | 0.42     |
| L1 (Lasso)          | Good       | \~0.80    | 0.38     |
| L2 (Ridge)          | Good       | \~0.79    | 0.39     |
| ElasticNet          | Good       | \~0.79    | 0.40     |

---

## 📌 Key Findings

* **Random Forest** performed best with high accuracy and AUC.
* Regularized Logistic Regression models reduced overfitting and gave stable results.
* Feature engineering and data scaling improved model effectiveness.

---

## 🖼️ Visualizations

* Confusion Matrices
* ROC-AUC Curves
* Feature Importance (for Random Forest)
* EDA plots in the `images/` folder

---

## ✅ Conclusion

This project demonstrates that machine learning can be effectively used to automate loan approval predictions. Ensemble models like Random Forest offer strong performance, but regularized logistic models also perform well with proper preprocessing.

---

## 📌 Future Improvements

* Hyperparameter tuning with GridSearchCV
* Use of SMOTE or class balancing techniques
* Integration with a Flask/Django backend for deployment

---

## 📚 Requirements

* Python 3.8+
* scikit-learn
* pandas
* matplotlib
* seaborn
* jupyter

Install dependencies:

```
pip install -r requirements.txt
```

---

For any questions or suggestions, feel free to reach out to any of the team members via GitHub.
