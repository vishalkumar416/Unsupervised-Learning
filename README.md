# Unsupervised Learning Algorithms – Machine Learning

This repository contains implementations of important **Unsupervised Learning algorithms** using Python and Scikit-learn.
Each algorithm is implemented in a separate Jupyter Notebook with visualization using inbuilt datasets.

The main goal of this project is to understand how machine learning models can **identify hidden patterns in unlabeled data**.

---

# What is Unsupervised Learning?

Unsupervised Learning is a type of **Machine Learning** where algorithms learn patterns from **unlabeled datasets**. Unlike supervised learning, there are **no target labels** provided.

The algorithm automatically discovers **structures, similarities, or clusters** in the data.

## Key Characteristics

* Works with **unlabeled data**
* Identifies **hidden patterns**
* Used for **clustering and dimensionality reduction**
* Useful for **data exploration**

## Applications

* Customer Segmentation
* Recommendation Systems
* Anomaly Detection
* Market Basket Analysis
* Data Compression
* Pattern Recognition

---

# Algorithms Implemented

This repository includes implementations of the following unsupervised learning algorithms:

1. K-Means Clustering
2. Hierarchical Clustering
3. DBSCAN Clustering
4. Gaussian Mixture Model (GMM)
5. PCA (Principal Component Analysis)

Each algorithm is implemented with visualization to better understand clustering and data transformation.

---

# 1. K-Means Clustering

K-Means is a popular clustering algorithm that divides the dataset into **K clusters** based on similarity.

## Working Steps

1. Select the number of clusters (K)
2. Initialize cluster centroids randomly
3. Assign data points to the nearest centroid
4. Update centroids based on assigned points
5. Repeat until centroids stop changing

## Advantages

* Simple and easy to implement
* Efficient for large datasets
* Fast convergence

## Limitations

* Requires predefined K value
* Sensitive to outliers
* Works best with spherical clusters

**Notebook File**

`K-Means Clustering.ipynb`

---

# 2. Hierarchical Clustering

Hierarchical clustering builds clusters in a **tree-like structure called a dendrogram**.

There are two types:

* Agglomerative (Bottom-Up)
* Divisive (Top-Down)

This implementation uses **Agglomerative Clustering**.

## Working Process

1. Each data point starts as a separate cluster
2. The closest clusters are merged
3. Merging continues until only one cluster remains

## Advantages

* No need to specify number of clusters initially
* Provides dendrogram visualization

## Limitations

* Computationally expensive
* Not suitable for very large datasets

**Notebook File**

`Hierarchical Clustering.ipynb`

---

# 3. DBSCAN Clustering

DBSCAN stands for **Density-Based Spatial Clustering of Applications with Noise**.

It groups data based on **density** and can detect **outliers**.

## Important Parameters

* eps → Neighborhood radius
* min_samples → Minimum points required to form a dense region

## Working Steps

1. Identify core points based on density
2. Expand clusters from core points
3. Label remaining points as noise

## Advantages

* Detects clusters of arbitrary shape
* Handles noise effectively
* No need to specify number of clusters

## Limitations

* Sensitive to parameter selection
* Difficult with varying density datasets

**Notebook File**

`DBSCAN Clustering.ipynb`

---

# 4. Gaussian Mixture Model (GMM)

Gaussian Mixture Model is a **probabilistic clustering algorithm** that assumes data points are generated from multiple Gaussian distributions.

Unlike K-Means, it assigns **probability of belonging to each cluster**.

## Working Principle

GMM uses the **Expectation-Maximization (EM) Algorithm**.

### Expectation Step

Calculate probability of each data point belonging to clusters.

### Maximization Step

Update Gaussian parameters to maximize likelihood.

## Advantages

* Can model overlapping clusters
* Flexible cluster shapes
* Provides probability-based clustering

## Limitations

* Slower than K-Means
* Sensitive to initialization

**Notebook File**

`Gaussian Mixture Model.ipynb`

---

# 5. PCA (Principal Component Analysis)

PCA is a **Dimensionality Reduction technique** used to reduce the number of features while preserving most of the important information.

It transforms original features into **principal components**.

## Steps in PCA

1. Standardize the dataset
2. Compute covariance matrix
3. Calculate eigenvalues and eigenvectors
4. Select principal components
5. Transform data into lower dimensional space

## Advantages

* Reduces dimensionality
* Improves visualization
* Removes redundant features

## Limitations

* Reduces interpretability
* Assumes linear relationships

**Notebook File**

`PCA (Dimensionality Reduction).ipynb`

---

# Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

# Installation

Clone the repository

git clone https://github.com/your-username/unsupervised-learning-algorithms.git

Move to project folder

cd unsupervised-learning-algorithms

Install required libraries

pip install numpy pandas matplotlib seaborn scikit-learn

Run Jupyter Notebook

jupyter notebook

---

# Project Structure

```
Unsupervised-Learning-Algorithms
│
├── K-Means Clustering.ipynb
├── Hierarchical Clustering.ipynb
├── DBSCAN Clustering.ipynb
├── Gaussian Mixture Model.ipynb
├── PCA (Dimensionality Reduction).ipynb
└── README.md
```

---

# Results

The notebooks demonstrate how unsupervised learning algorithms can discover patterns and group similar data points without labeled outputs.

Visualizations help understand clustering structures and dimensionality reduction.

---

# Future Improvements

* Apply algorithms on real-world datasets
* Add comparison of clustering performance
* Implement additional algorithms such as:

Mean Shift
Spectral Clustering
t-SNE

---

# Author

**Vishal Kumar**
B-Tech in Artificial Intelligence and Data Science
