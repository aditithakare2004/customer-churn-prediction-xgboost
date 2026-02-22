# customer-churn-prediction-xgboost
End-to-end customer churn prediction using SMOTE and tuned XGBoost with ROC-AUC optimization.


##  Project Overview

This project builds an end-to-end Machine Learning system to predict whether a telecom customer is likely to churn (leave the service). The solution uses advanced preprocessing, class imbalance handling with SMOTE, and a tuned XGBoost model to deliver reliable churn predictions.

The goal is to help businesses identify at-risk customers early and take proactive retention actions.

---

##  Problem Statement

Customer churn is a critical business problem in the telecom industry. Retaining existing customers is significantly more cost-effective than acquiring new ones. This project predicts customer churn using historical customer data.

**Type:** Binary Classification
**Target Variable:** `Churn` (Yes/No)

---

##  Dataset

* **Name:** Telco Customer Churn Dataset
* **Records:** ~7,000 customers
* **Domain:** Telecom
* **Source:** Kaggle

###  Key Features Used

* tenure
* MonthlyCharges
* TotalCharges
* Contract
* InternetService
* gender
* SeniorCitizen

---

##  Machine Learning Pipeline

### ✔ Data Preprocessing

* Handled missing values in `TotalCharges`
* Encoded categorical variables
* Feature alignment for inference

###  Class Imbalance Handling

* Applied **SMOTE** to balance churn classes

###  Model Training

Models experimented:

* Logistic Regression
* Decision Tree
* Random Forest
* **XGBoost (Final Model)** ⭐

###  Hyperparameter Tuning

* Used **GridSearchCV**
* Optimized for ROC-AUC

---

##  Final Model Performance (XGBoost)

| Metric         | Score      |
| -------------- | ---------- |
| Accuracy       | ~0.76      |
| ROC-AUC        | **~0.82**  |
| Recall (Churn) | High       |
| Overfitting    | Controlled |

✅ Balanced performance after SMOTE
✅ Suitable for business use

---

##  ROC Curve

The ROC curve demonstrates strong separability of churn vs non-churn customers using the tuned XGBoost model.

---

## 🚀 How to Run the Project

### 1️⃣ Clone Repository

```bash
git clone https://github.com/aditithakare2004/customer-churn-prediction-xgboost.git
cd customer-churn-prediction-xgboost
```

### 2️⃣ Install Requirements

```bash
pip install -r requirement.txt
```

### 3️⃣ Train Model (Optional)

```bash
python src/train_model.py
```

### 4️⃣ Run Prediction

```bash
python main.py
```

---

##  Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- XGBoost  
- Imbalanced-learn (SMOTE)  
- Matplotlib  
- Seaborn 

##  Project Structure

```
customer-churn-prediction-xgboost/
│
├── data/
├── notebooks/
├── src/
├── models/
├── images/
├── requirements.txt
├── README.md
└── LICENSE
```

---

##  Business Impact

* Early identification of at-risk customers
* Enables targeted retention campaigns
* Reduces revenue loss
* Improves customer lifetime value

---

##  Future Improvements

* Streamlit web deployment
* SHAP explainability
* Real-time API with FastAPI
* Automated retraining pipeline

---

## 👩‍💻 Author

**Aditi Thakare**
B.Tech Computer Science | Machine Learning Enthusiast

---

##  If you found this useful

Give this repo a ⭐ on GitHub!
