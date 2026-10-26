# Machine Learning Laboratory Portfolio

This repository hosts practical implementations, predictive modeling pipelines,
and applied intelligence architectures developed for the Machine Learning and
Data Science curriculum at Mundiapolis University.

---

## Laboratory & Project Overview

| Module | Category | Core Methodology | Primary Deliverables | Reference |
| :--- | :--- | :--- | :--- | :--- |
| **[subject-01-ecommerce](./mini-projects/subject-01-ecommerce)** | Business Project | Customer segmentation, K-Means clustering, Agglomerative Hierarchical Clustering (Ward linkage), Elbow heuristic | 5 behavioral segments & dendrograms | [Notebook](./mini-projects/subject-01-ecommerce/customer-segmentation.ipynb) |
| **[subject-02-telecom](./mini-projects/subject-02-telecom)** | Business Project | Supervised churn classification, feature correlation heatmaps, class probability scoring | Churn predictor & executive report | [Notebook](./mini-projects/subject-02-telecom/telecom-churn-prediction.ipynb) |
| **[subject-03-student-success](./mini-projects/subject-03-student-success)** | Capstone Project | Academic risk factor discovery, Random Forest feature importance, PCA, interactive Flask decision tool | Predictive Flask web app | [Notebook](./mini-projects/subject-03-student-success/student-success-analysis.ipynb)<br>[App](./mini-projects/subject-03-student-success/web-app/app.py) |
| **[clustering](./labs-tp/clustering)** | Algorithmic Lab | Unsupervised benchmark comparison: K-Means, Hierarchical (CAH), and DBSCAN density clustering | Multi-model clustering comparison | [Notebooks](./labs-tp/clustering) |
| **[regression](./labs-tp/regression)** | Algorithmic Lab | Analytical Ordinary Least Squares (OLS) vs vectorized Gradient Descent optimization | Convergence curves & loss graphs | [Scripts](./labs-tp/regression) |

---

## General Running Instructions

### Prerequisites

- **Python:** 3.10 or higher
- **Git**
- **Virtual Environment Tooling:** `venv`

### Setup and Environment

1. **Clone the repository:**
   ```bash
   git clone git@github.com:ind4x/machine-learning-portfolio.git
   cd machine-learning-portfolio
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

### Executing Modules

#### Jupyter Notebooks
Launch Jupyter from the repository root:
```bash
jupyter notebook
```
Navigate to any notebook in `mini-projects/` or `labs-tp/` to execute analysis and training cells.

#### Interactive Student Success Web App
```bash
cd mini-projects/subject-03-student-success/web-app
python3 app.py
```
Open `http://127.0.0.1:5000` in a web browser.

---

## Technology Stack

- **Language:** Python 3
- **Data Engineering:** NumPy, Pandas
- **Machine Learning:** Scikit-learn (`KMeans`, `AgglomerativeClustering`, `DBSCAN`, `RandomForestClassifier`, `PCA`)
- **Web App:** Flask
- **Data Visualization:** Matplotlib, Seaborn

---

## Author

- **Author:** Youssef Fellah ([ind4x_](https://github.com/ind4x))
- **Institution:** Mundiapolis University, Engineering Cycle
