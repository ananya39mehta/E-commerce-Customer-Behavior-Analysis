# EDA, Dimensionality Reduction & Clustering on E-commerce Customer Behavior

This project analyzes user behavior on an e-commerce website using **Exploratory Data Analysis (EDA)**, **Dimensionality Reduction** (PCA, t-SNE), and **Clustering** (KMeans, DBSCAN, Hierarchical). The aim is to segment users based on their interaction with different product categories.

## 📊 Project Overview

The notebook walks through:
- Data Cleaning and Preprocessing
- Exploratory Data Analysis
- Feature Engineering and Scaling
- Dimensionality Reduction using PCA and t-SNE
- Clustering with K-Means, DBSCAN, and Hierarchical Clustering
- Cluster Interpretation and Visualization

## 🧰 Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Yellowbrick
- Plotly

## 📈 Key Insights & Inferences

- **Dimensionality Reduction**:
  - PCA effectively reduced dimensionality while preserving most of the variance, helping in visualizing the underlying structure of the data.
  - t-SNE provided better visual separation between potential clusters but was sensitive to hyperparameters like perplexity.

- **Clustering Results**:
  - **KMeans** identified 3 main customer behavior clusters, aligned with product engagement patterns.
    - Cluster 0: Likely represents customers engaging mostly with sale items.
    - Cluster 1: Customers more interested in specific categories like trousers or skirts.
    - Cluster 2: Users with high engagement across multiple categories.
  - **DBSCAN** struggled with high-dimensional data and produced many noise points.
  - **Hierarchical Clustering** confirmed similar groups as KMeans, indicating stable patterns in user behavior.

- **Customer Behavior Patterns**:
  - Certain countries like the USA, UK, and Germany showed higher engagement.
  - Users preferred specific product positions on the page (e.g., "top middle").
  - Color preferences like black, white, and blue dominated user clicks.

- **Business Impact**:
  - These clusters can be used to tailor product recommendations or marketing strategies.
  - Product page layout and featured color variations could be optimized based on user preferences.
  - Prices and model photography types had a noticeable effect on engagement.

## 📦 Installation

Clone this repository and install dependencies:

```bash
git clone https://github.com/your-username/eda-dim-red-clustering.git
cd eda-dim-red-clustering
pip install -r requirements.txt
```

## 📁 File Description

| File | Description |
|------|-------------|
| `eda-dim-red-clustering.ipynb` | Full Jupyter Notebook with analysis |
| `requirements.txt` | Python dependencies |
| `.gitignore` | Ignored files in GitHub |

## 🧪 Running the Notebook

Use Jupyter Notebook or JupyterLab to open:

```bash
jupyter notebook eda-dim-red-clustering.ipynb
```

## 📜 License

This project is open-source and free to use under the MIT License.
