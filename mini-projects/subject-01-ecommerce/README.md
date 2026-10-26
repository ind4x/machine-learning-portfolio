# E-Commerce Customer Segmentation: Retail Analytics

This project utilizes unsupervised learning algorithms to partition a retail customer base
into distinct behavioral segments based on annual income, spending scores, and demographic
profiles.

---

## Project Structure

```text
subject-01-ecommerce/
├── README.md                          # Technical specification and segmentation analysis
├── customer-segmentation.ipynb        # Interactive data science notebook
├── customer-segmentation-report.pptx  # Executive briefing and strategic presentation
├── k-means-elbow-method.png           # WCSS inertia curve identifying optimal k=5
├── k-means-clusters-plot.png          # 2D scatter plot of customer clusters
├── hierarchical-dendrogram.png        # Ward linkage tree clustering hierarchy
├── eda-distribution-1.png             # Age distribution histogram
├── eda-distribution-2.png             # Annual income distribution
└── eda-distribution-3.png             # Spending score distribution
```

### File Responsibilities

- **`customer-segmentation.ipynb`**: Complete executable Python pipeline evaluating exploratory distributions, Elbow method inertia curves, silhouette validation scores, K-Means cluster fitting, and Agglomerative Hierarchical Clustering.
- **`customer-segmentation-report.pptx`**: Commercial analysis translating mathematical clusters into marketing personas (e.g., High-Income/High-Spenders vs Budget-Conscious).

---

## Architecture & Segmentation Methodology

```text
Raw Customer Demographic Data
             |
             v
+-------------------------------+
| Preprocessing & Normalization | ---> Null check, Outlier detection, MinMax/StandardScaler
+-------------------------------+
             |
             +---------------------------------------+
             |                                       |
             v                                       v
+-------------------------------+       +-------------------------------+
|      K-Means Clustering       |       |   Hierarchical Clustering     |
| - Elbow Inertia (WCSS)        |       | - Agglomerative bottom-up     |
| - Centroid distance update    |       | - Ward minimum variance       |
| - 5 Distinct Cohorts          |       | - Dendrogram threshold cut    |
+-------------------------------+       +-------------------------------+
             |                                       |
             +-------------------+-------------------+
                                 |
                                 v
+---------------------------------------------------------------+
|                      Customer Personas                        |
|  Cluster 0: Target High Value (High Income, High Spending)    |
|  Cluster 1: Conservative (High Income, Low Spending)          |
|  Cluster 2: Standard Average (Moderate Income & Spending)     |
|  Cluster 3: Careless / Impulsive (Low Income, High Spending)  |
|  Cluster 4: Sensible / Budget (Low Income, Low Spending)      |
+---------------------------------------------------------------+
```

---

## Execution Instructions

Launch Jupyter and open the notebook:

```bash
cd mini-projects/subject-01-ecommerce
jupyter notebook customer-segmentation.ipynb
```

---

## Technology Stack

- **Language:** Python 3
- **Data Engineering:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (`KMeans`, `AgglomerativeClustering`, `silhouette_score`)
- **Visualization:** Matplotlib, Seaborn

---

## Author

- **Author:** Youssef Fellah ([ind4x_](https://github.com/ind4x))
- **Institution:** Mundiapolis University, Engineering Cycle
