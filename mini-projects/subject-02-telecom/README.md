# Predictive Analysis: Telecom Customer Churn

This project implements an end-to-end predictive classification pipeline to forecast
customer attrition for a telecommunications operator, isolating high-risk customer
cohorts and identifying primary drivers of account churn.

---

## Project Structure

```text
subject-02-telecom/
├── README.md                          # Technical specification and model benchmarks
├── telecom-churn-prediction.ipynb     # Interactive machine learning pipeline notebook
└── telecom-churn-report.pptx          # Executive slides summarizing model accuracy and retention KPIs
```

### File Responsibilities

- **`telecom-churn-prediction.ipynb`**: Complete executable Python notebook implementing data cleaning, tenure feature engineering, exploratory correlation heatmaps, categorical encoding, train/test splitting, and multi-model classification comparison.
- **`telecom-churn-report.pptx`**: Business synthesis presenting customer lifetime value (CLV) retention recommendations.

---

## Architecture & Machine Learning Pipeline

```text
Raw Subscriber Data (Contract Type, Monthly Charges, Tech Support, Tenure)
                               |
                               v
               +-------------------------------+
               | Preprocessing & Encoding      |
               | - Binary & One-Hot Encoding   |
               | - Numerical Feature Scaling   |
               +-------------------------------+
                               |
                               v
               +-------------------------------+
               | Supervised Classification     |
               | - Logistic Regression         |
               | - Random Forest Classifier    |
               | - Gradient Boosting           |
               +-------------------------------+
                               |
                               v
               +-------------------------------+
               | Evaluation & Retention Action |
               | - Precision, Recall, ROC-AUC  |
               | - Churn Probability Scoring   |
               +-------------------------------+
```

---

## Execution Instructions

Launch Jupyter and run the notebook:

```bash
cd mini-projects/subject-02-telecom
jupyter notebook telecom-churn-prediction.ipynb
```

---

## Technology Stack

- **Language:** Python 3
- **Data Engineering:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (`LogisticRegression`, `RandomForestClassifier`, `StandardScaler`, `metrics`)
- **Visualization:** Matplotlib, Seaborn

---

## Author

- **Author:** Youssef Fellah ([ind4x_](https://github.com/ind4x))
- **Institution:** Mundiapolis University, Engineering Cycle
