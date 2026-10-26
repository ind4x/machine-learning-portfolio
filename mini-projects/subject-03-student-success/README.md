# Improving Student Success: Academic Performance Analysis

This capstone project combines deep predictive analytics and unsupervised customer
segmentation with an interactive Flask decision-support web application, identifying
key risk factors influencing student outcomes in high school mathematics and language curricula.

---

## Project Structure

```text
subject-03-student-success/
├── README.md                          # Technical specification and architecture overview
├── student-success-analysis.ipynb     # Interactive exploratory, clustering, and modeling notebook
├── data/                              # Benchmark student performance datasets
│   ├── student-mat.csv                # Mathematics course performance records
│   └── student-por.csv                # Portuguese language course performance records
└── web-app/                           # Interactive pedagogical decision application
    ├── app.py                         # Flask application serving inference endpoints
    ├── run.sh                         # Shell launcher
    ├── requirements.txt               # App-specific dependencies
    ├── templates/                     # Jinja2 HTML interfaces
    │   └── index.html                 # Interactive prediction and student profile dashboard
    ├── student-mat.csv                # Static runtime dataset reference
    └── student-por.csv                # Static runtime dataset reference
```

### File Responsibilities

- **`student-success-analysis.ipynb`**: Complete exploratory data science notebook: correlation analysis, K-Means clustering, Principal Component Analysis (PCA), and Random Forest feature importance calculations.
- **`web-app/app.py`**: Lightweight Flask web application allowing educators to input student behavioral metrics (study time, past failures, family support, absences) and receive immediate real-time risk level predictions.

---

## System Architecture

```text
+-----------------------+
| Educational Datasets  |  (Demographic, Behavioral, Historical Grades)
+-----------------------+
            |
            v
+-----------------------+
|  Analytical Modeling  |  - K-Means Clustering (Identifies student cohorts)
|  & Feature Importance |  - Random Forest Regressor (Ranks failure indicators)
|                       |  - PCA Dimensionality Reduction (2D visualization)
+-----------------------+
            |
            v
+-----------------------+
| Pedagogical Decision  |  - Identifies at-risk students before final evaluations
| Guidance Platform     |  - Prescribes targeted tutoring and intervention plans
+-----------------------+
            |
            v
+-----------------------+
| Flask Web Application |  Interactive UI: http://localhost:5000
+-----------------------+
```

---

## Execution Instructions

### 1. Running the Machine Learning Notebook
```bash
jupyter notebook student-success-analysis.ipynb
```

### 2. Launching the Interactive Web Application
```bash
cd web-app
pip install -r requirements.txt
python3 app.py
```
Open `http://127.0.0.1:5000` in your web browser.

---

## Technology Stack

- **Language:** Python 3
- **Data Engineering:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (`KMeans`, `RandomForestRegressor`, `PCA`)
- **Web App:** Flask, Jinja2, HTML5/CSS3
- **Visualization:** Matplotlib, Seaborn

---

## Author

- **Author:** Youssef Fellah ([ind4x_](https://github.com/ind4x))
- **Institution:** Mundiapolis University, Engineering Cycle
