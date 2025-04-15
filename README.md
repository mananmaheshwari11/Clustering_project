# Clustering project
# 🧠 Customer Segmentation using Clustering

This project applies **unsupervised machine learning** techniques to segment customers based on their **annual income** and **spending score**. The goal is to group similar customers together to better understand purchasing behaviors.

---

## 📌 What is Clustering?

**Clustering** is an unsupervised learning technique used to group data points such that items in the same group (called a cluster) are more similar to each other than to those in other groups.

Clustering is commonly used in:
- Customer segmentation
- Market research
- Image compression
- Anomaly detection

---

## 🧪 Hard vs. Soft Clustering

| Type             | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Hard Clustering** | Each data point is assigned to exactly one cluster.                            |
| **Soft Clustering** | A data point can belong to multiple clusters with a probability distribution. |

---

## 🔍 Algorithms Used

### 📌 1. KMeans Clustering (Hard)

- Divides the dataset into **K non-overlapping clusters**.
- Each point is assigned to the nearest cluster center (centroid).
- Updates centroids iteratively until convergence.

**Pros:**
- Fast and efficient for large datasets.
- Easy to understand and implement.

**Cons:**
- Assumes clusters are spherical and equally sized.
- Requires the number of clusters (`k`) to be defined in advance.

---

### 📌 2. Gaussian Mixture Model (Soft)

- Probabilistic model assuming data is generated from multiple **Gaussian distributions**.
- Each point is assigned a probability of belonging to each cluster.

**Pros:**
- Captures uncertainty in cluster membership.
- Works well when clusters overlap or have different shapes.

**Cons:**
- More computationally intensive than KMeans.
- Can get stuck in local optima without good initialization.

---

### 📌 3. Agglomerative Clustering (Hierarchical)

- A bottom-up approach to clustering.
- Initially treats each point as its own cluster, then merges them step-by-step based on distance metrics (e.g., Euclidean).

**Pros:**
- No need to pre-specify the number of clusters.
- Produces a **dendrogram** showing the hierarchy of clusters.

**Cons:**
- Computationally expensive for large datasets.
- Sensitive to noise and outliers.

---

## 📊 Dataset Used

- **Mall_Customers.csv**
- Columns used: `Annual Income (k$)`, `Spending Score (1-100)`
- Preprocessed using standardization for better performance.

---

## 📈 Visualizations

- Side-by-side scatter plots comparing KMeans and GMM cluster assignments.
- Optionally, a dendrogram for Agglomerative Clustering.

---

## 🧑‍💻 Made by: **Manan**

---

## ✅ Future Enhancements

- Include Age or Gender as clustering features.
- Add interactive visualizations (e.g., using Plotly).
- Implement silhouette analysis or BIC/AIC to determine the optimal number of clusters.

---
