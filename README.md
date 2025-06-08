# Anomaly Detection

This project explores various unsupervised anomaly detection techniques applied to both real-world and synthetic datasets using Python and scikit-learn.

## 📌 Overview

The objective is to detect outliers using different machine learning approaches and compare their performance across distinct data types.

### Techniques Used
- **Isolation Forest**
- **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**
- **Local Outlier Factor (LOF)**

## 📁 Datasets

1. **Real-world dataset**
   - `healthcare.csv`: Contains healthcare-related data on which Isolation Forest was applied.

2. **Synthetic dataset**
   - Generated using `make_circles(n_samples=1000, noise=0.1, factor=0.3)`
   - Used for both DBSCAN and LOF anomaly detection.

## 🔍 Methods

### 1. Isolation Forest
- Applied to the `healthcare.csv` dataset.
- Detects anomalies by isolating observations that are far from the rest of the data.

### 2. DBSCAN
- Applied on synthetic circular data.
- Identifies anomalies as points not belonging to any dense cluster.

### 3. Local Outlier Factor
- Also applied to the same synthetic circular data.
- Flags samples as outliers based on local density deviation.

## 📊 Visualizations
Plots and graphs are included for:
- Cluster formation (DBSCAN)
- Local density comparisons (LOF)
- Outlier points (all methods)

## 🛠️ Installation

```bash
git clone https://github.com/your-username/anomaly-detection.git
cd anomaly-detection
pip install -r requirements.txt
