# Telecommunication Customer Attrition Analysis

This project analyzes customer churn (attrition) in the telecommunications industry using a public dataset and applies a Random Forest classifier to predict which customers are at risk of leaving. The project identifies the most influential features driving churn and offers recommendations for reducing attrition.

---

## 📘 Project Overview

Customer churn is one of the most pressing issues for telecom providers, where high competition and fluctuating pricing can lead to frequent customer turnover. By identifying customers most at risk of churning, telecom companies can proactively improve retention strategies and optimize customer experience.

This project:
- Explores telecom customer behavior using a real-world-style dataset
- Preprocesses and balances the dataset using SMOTE
- Builds a Random Forest classification model
- Evaluates model accuracy and feature importance
- Recommends actionable retention strategies

---

## 🧾 Dataset

- **Source**: [Kaggle – Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Rows**: 7,043  
- **Features**: 21 (demographic + service attributes + churn status)

Each row represents a unique customer, with attributes such as:
- Tenure
- Monthly/Total Charges
- Internet and streaming services
- Payment method and billing type
- Churn (target)

---

## ⚙️ Modeling Workflow

### 1. **Data Cleaning**
- Handled incorrect data types (e.g., converting `TotalCharges` from object to float)
- Dropped null or invalid entries
- Encoded categorical variables using `LabelEncoder`

### 2. **Preprocessing**
- Balanced the training data using **SMOTE** (Synthetic Minority Over-sampling Technique)
- Split the dataset into training and testing sets

### 3. **Model Implementation**
- Used **Random Forest Classifier** from `scikit-learn`
- Trained on oversampled data
- Evaluated on holdout test data

---

## 📊 Results

- **Model Accuracy**: 77% on test data (well above the 70% benchmark for classification models)
- **Top Churn Indicators**:
  - Paperless billing status (most influential)
  - Monthly charges
  - Total charges
  - Gender (not recommended for targeting, but flagged by the model)

### 📈 Feature Importance Chart:
> Visualized which features most influenced the model's churn predictions, guiding retention focus areas.

---

## 💡 Key Insights

- Customers **without paperless billing** were more likely to churn.
- Higher **monthly charges** correlated with higher churn risk.
- Despite its predictive power, **gender** should not be used for decision-making due to ethical considerations.

---

## ✅ Recommendations

- **Promote paperless billing** enrollment via incentives or opt-out policies.
- **Review pricing tiers** for high-charge customers and explore loyalty discounts.
- Avoid using sensitive demographic features like gender in decision-making.

---

## 📚 Learning Outcomes

- Developed a deeper understanding of churn modeling using tree-based classifiers
- Gained hands-on experience with data preprocessing and class imbalance solutions
- Reflected on the ethical implications of feature selection in predictive modeling

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `Telecommunication_Customer_Attrition.ipynb` | Jupyter Notebook with full code for data prep, modeling, and evaluation |
| `Final_White_Paper.pdf` | Full project write-up including rationale, modeling decisions, evaluation results, and recommendations |

---

## 🤝 Author

**Ruben Brionez Jr**  
_M.S. in Data Science candidate at Bellevue University_  
[LinkedIn](https://www.linkedin.com/in/ruben-brionez-jr/)  
[GitHub](https://github.com/rbrionezjr-bellevue)

---

## 📜 License

This project is intended for academic and educational use only.
