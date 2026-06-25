# Principal Component Analysis (PCA) for Dimensionality Reduction and Visualization

## Project Overview

This project demonstrates the use of **Principal Component Analysis (PCA)**, one of the most widely used dimensionality reduction techniques in machine learning.

PCA transforms high-dimensional data into a smaller number of principal components while preserving as much information (variance) as possible. This simplifies visualization, reduces computational complexity, and prepares data for downstream machine learning algorithms.

---

# Business Problem

Real-world datasets often contain many correlated features, making visualization and model training difficult.

Principal Component Analysis addresses this challenge by:

- Reducing the number of variables
- Preserving important information
- Eliminating redundancy
- Improving computational efficiency
- Enabling visualization of high-dimensional data

---

# Dataset

**Mall Customers Dataset**

The dataset contains customer demographic and spending information.

Features used:

- Age
- Annual Income (k$)
- Spending Score (1–100)

---

# Project Workflow

## 1. Data Exploration

- Loaded dataset
- Examined dataset dimensions
- Inspected data types
- Generated descriptive statistics
- Checked for missing values

---

## 2. Feature Selection

Selected numerical variables:

- Age
- Annual Income (k$)
- Spending Score (1–100)

---

## 3. Feature Scaling

Applied StandardScaler to normalize the features before PCA.

```python
from sklearn.preprocessing import StandardScaler
```

---

## 4. Principal Component Analysis

Reduced three original features into two principal components.

```python
from sklearn.decomposition import PCA

pca = PCA(n_components=2)
```

---

## 5. Variance Analysis

Measured how much information was preserved after dimensionality reduction.

### Explained Variance

| Component | Variance Explained |
|------------|-------------------:|
| Principal Component 1 | 44.27% |
| Principal Component 2 | 33.31% |

### Total Variance Preserved

```text
77.57%
```

This means that two principal components retained approximately **78% of the original information** contained in the dataset.

---

## 6. PCA Visualization

Visualized customers using:

- Principal Component 1
- Principal Component 2

The resulting scatter plot illustrates how PCA projects multi-dimensional customer information into a two-dimensional space for easier interpretation.

---

## 7. Explained Variance Curve

Generated a cumulative explained variance plot to determine the number of principal components required to retain the majority of the dataset's information.

---

# Key Results

- Successfully reduced the dataset from **3 features to 2 principal components**.
- Preserved approximately **77.57%** of the original variance.
- Produced a two-dimensional representation suitable for visualization.
- Demonstrated how PCA compresses information while minimizing information loss.

---

# Machine Learning Concepts Covered

- Unsupervised Learning
- Feature Engineering
- Dimensionality Reduction
- Principal Component Analysis (PCA)
- Variance Explained
- Feature Scaling
- Data Compression
- Data Visualization

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

# Project Structure

```
PCA_Dimensionality_Reduction_Visualization/
│
├── PCA_Dimensionality_Reduction.ipynb
├── README.md
├── requirements.txt
└── images/
```

---

# Key Takeaways

- PCA reduces dimensionality while preserving the most important information.
- Standardizing features is essential before applying PCA.
- The first principal component captures the highest variance.
- PCA is valuable for visualization, feature compression, noise reduction, and improving machine learning workflows.

---

# Future Improvements

- Apply PCA before clustering algorithms such as K-Means.
- Compare clustering performance with and without PCA.
- Explore 3D PCA using three principal components.
- Apply PCA to larger and higher-dimensional datasets.
- Investigate nonlinear dimensionality reduction techniques such as t-SNE and UMAP.

---

# Author

**Stephen Mariga Ndegwa**

Data Analyst | Machine Learning Engineer | AI Engineer

This project is part of a comprehensive machine learning portfolio covering supervised learning, unsupervised learning, dimensionality reduction, model evaluation, and artificial intelligence.
