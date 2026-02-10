# DBSCAN Clustering Analysis (Unsupervised Learning)

This project demonstrates **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** using
`scikit-learn`.  
It focuses on clustering without predefined labels, detecting noise points, and evaluating clusters using
standard unsupervised metrics.

---

## 📌 Project Overview

DBSCAN is an unsupervised learning algorithm that:
- Automatically determines the number of clusters
- Identifies arbitrarily shaped clusters
- Detects outliers (noise points)

This project applies DBSCAN on a synthetic dataset and evaluates its performance using multiple clustering metrics.

---

## 🧠 Concepts Covered

- Unsupervised Learning
- Density-Based Clustering
- Feature Scaling
- Noise / Outlier Detection
- Cluster Evaluation Metrics

---

## 📂 Dataset Used

- **Source:** `sklearn.datasets.make_blobs`
- **Type:** Synthetic dataset
- **Samples:** 1000
- **Features:** 2 (for visualization)

The dataset is scaled using **StandardScaler**, which is crucial for DBSCAN performance.

---

## ⚙️ Algorithm Used

### DBSCAN Parameters:
- **eps:** Radius of neighborhood
- **min_samples:** Minimum points required to form a dense region

Noise points are labeled as **-1**.

---

## 📊 Evaluation Metrics

The following unsupervised metrics are used (excluding noise points):

| Metric | Description | Interpretation |
|------|------------|----------------|
| Silhouette Score | Measures cohesion & separation | Higher is better |
| Davies-Bouldin Index | Measures cluster overlap | Lower is better |
| Calinski-Harabasz Score | Ratio of between/within cluster dispersion | Higher is better |

---

## 📈 Visualization

Clusters are visualized using scatter plots:
- Different colors represent different clusters
- Noise points are marked separately

---

## 🛠️ Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-learn

---

## ▶️ How to Run

1. Clone the repository
```bash
git clone https://github.com/your-username/dbscan-clustering-analysis.git
```
Install dependencies

pip install -r requirements.txt


Run the notebook

jupyter notebook DBScan.ipynb
