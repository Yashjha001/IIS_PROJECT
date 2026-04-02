# Market Regime Discovery in FAANG Stocks Using K-Means Clustering

## Overview
This project analyzes FAANG stock market data using **unsupervised machine learning** to identify hidden market behavior patterns. Instead of predicting future stock prices, the model focuses on **market regime discovery** by grouping similar historical market conditions into meaningful clusters.

The framework transforms raw stock market data into a representative feature space using **technical indicators** and **engineered financial features**, and then applies **K-Means clustering** to detect interpretable market regimes such as:

- **Bullish Market**
- **Stable / Neutral Market**
- **Bearish / Volatile Market**

This project is designed as an **exploratory financial machine learning system** for understanding stock market structure and behavior.

---

## Objective
The main objective of this project is to discover **hidden patterns in stock market behavior** using clustering techniques. The project aims to:

- Analyze historical FAANG stock data
- Extract meaningful financial and technical features
- Apply K-Means clustering to group similar market conditions
- Interpret the clusters as different stock market regimes
- Visualize and evaluate clustering results

---

## Features Used
The model uses a combination of **raw stock attributes** and **engineered technical indicators**.

### Primary Stock Features
- Open
- High
- Low
- Close
- Volume

### Engineered Features
- Daily Return
- Volatility
- RSI (Relative Strength Index)
- MACD (Moving Average Convergence Divergence)

These features help capture:
- **Price movement**
- **Trend direction**
- **Momentum**
- **Risk / Volatility**

---

## Workflow
The complete workflow of the project is:

1. **Data Collection**
2. **Feature Engineering**
3. **Feature Extraction**
4. **Data Standardization**
5. **K-Means Clustering**
6. **Cluster Evaluation**
7. **Visualization & Interpretation**

---

## Model Used
### K-Means Clustering
K-Means is used as the core unsupervised learning algorithm to group similar market states based on their statistical and behavioral characteristics.

The final output clusters represent:
- **Cluster 0 → Bullish Behavior**
- **Cluster 1 → Stable / Neutral Behavior**
- **Cluster 2 → Bearish / Volatile Behavior**

---

## Evaluation Metrics
Since this is an **unsupervised learning** project, traditional supervised metrics such as accuracy or F1-score are not used.

Instead, clustering performance is evaluated using:

- **WCSS (Within-Cluster Sum of Squares)**
- **Elbow Method**
- **Cluster Compactness**
- **Cluster Separation**
- **Interpretability of Clusters**

---

## Visual Outputs
This project includes visual analysis such as:

- Elbow Curve
- Cluster Scatter Plot
- Feature Distribution Graphs
- Correlation Analysis
- Summary Statistics Tables

These visualizations help in understanding how different market regimes are formed.

---

## Tech Stack
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Jupyter Notebook**

---

## Project Structure
```bash
├── data/
│   └── faang_stock_data.csv
├── notebooks/
│   └── stock_clustering_analysis.ipynb
├── images/
│   ├── workflow_detailed.png
│   ├── elbow_curve.png
│   ├── cluster_plot.png
│   └── feature_distribution.png
├── src/
│   └── preprocessing_and_clustering.py
├── README.md
└── requirements.txt
