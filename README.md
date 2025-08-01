# Customer-Segmentation

## 📌 Overview

This project implements a **customer segmentation model** using **K-Means clustering** on the **Mall Customers dataset**. The goal is to group customers into distinct segments based on their **Annual Income** and **Spending Score**, which can help businesses better understand customer behavior and improve marketing strategies.

---

## 🗂️ Dataset

- **Source:** [Mall Customer Dataset (Kaggle)](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation)
- **Records:** 200 customers
- **Features:**
  - `Gender`
  - `Age`
  - `Annual Income (k$)`
  - `Spending Score (1-100)`

---

## 🎯 Objectives

- Load and clean the dataset (remove nulls/duplicates)
- Scale the numerical data
- Perform **visual exploratory analysis** (Histogram, Boxplot, Scatter, Heatmap)
- Apply **K-Means Clustering**
- Determine the **optimal number of clusters** using:
  - Elbow Method
  - Silhouette Score
- Visualize the customer clusters in 2D space
- Analyze characteristics of each cluster
- *(Bonus)* Try alternative clustering algorithms (e.g., DBSCAN)
- *(Bonus)* Analyze average spending score per cluster

---

## 🛠️ Tools & Libraries

- **Python**
- **Pandas** – data handling
- **NumPy** – numerical operations
- **Matplotlib / Seaborn** – data visualization
- **Scikit-learn** – machine learning & clustering

---

## 📊 Key Components

### 1. 📥 Data Preprocessing
- Checked for and removed null or duplicate entries
- Scaled `Annual Income` and `Spending Score` for better clustering performance

### 2. 📈 Visual Exploration
- **Histogram** – to observe distributions of Age, Income, and Spending Score
- **Boxplot** – to detect outliers and understand spread
- **Scatter Plot** – to visualize relations between features (e.g., Income vs Spending)
- **Heatmap** – to analyze feature correlations

### 3. 🧠 Clustering
- Applied **K-Means algorithm** on scaled features (`Annual Income`, `Spending Score`)
- Visualized resulting clusters in a 2D scatter plot with centroids
- Interpreted spread, tightness, and separability of clusters

### 4. 🧪 Optimal Cluster Detection
- **Elbow Method** – plotted inertia vs. number of clusters
- **Silhouette Score** – used to evaluate the quality of clustering

### 5. 🎨 Cluster Visualization
- 2D scatter plots colored by cluster labels
- Highlighted cluster centers with distinct markers

### 6. 📊 Cluster Interpretation
- Analyzed each cluster’s:
  - Size (number of customers)
  - Average income
  - Average spending score
  - Demographic patterns (optional)

---

## 🚀 Bonus Work

- 🧪 Tried **DBSCAN** clustering algorithm as an alternative to K-Means
- 📊 Calculated average **Spending Score** per cluster to identify high-value customers

---

## ✅ Covered Topics

- Unsupervised Learning
- Clustering (K-Means, DBSCAN)
- Data Scaling
- Data Visualization
- Evaluation metrics (Inertia, Silhouette Score)

---

## 🏁 Future Improvements

- Include Age and Gender as encoded features to enrich clustering
- Build a dashboard for interactive cluster exploration (e.g., Plotly or Streamlit)
- Extend analysis with **predictive modeling** based on segment behavior

