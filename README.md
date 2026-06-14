# Customer Segmentation using K-Means Clustering

## 📌 Project Overview

Customer segmentation is the process of dividing customers into distinct groups based on common characteristics. This project applies the **K-Means Clustering** algorithm to segment mall customers according to their **Age**, **Annual Income**, and **Spending Score**.

The insights obtained from clustering can help businesses improve marketing campaigns, personalize customer experiences, and increase sales through targeted promotions.

---

## 🎯 Objectives

* Analyze customer behavior using demographic and spending data.
* Identify distinct customer groups using K-Means Clustering.
* Visualize customer segments for better business understanding.
* Predict the segment of new customers based on their characteristics.

---

## 📂 Dataset

The dataset used is **Mall_Customers.csv**, containing information about mall customers.

### Features Used

| Feature                | Description                                        |
| ---------------------- | -------------------------------------------------- |
| Age                    | Customer age                                       |
| Annual Income (k$)     | Annual income in thousand dollars                  |
| Spending Score (1-100) | Score assigned based on customer spending behavior |

### Removed Features

* CustomerID
* Gender

These columns were excluded because they do not significantly contribute to clustering.

---

## 🛠 Technologies and Libraries

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Collections

Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## 📊 Methodology

### 1. Data Preprocessing

* Loaded dataset using Pandas.
* Explored data structure using:

  * `.info()`
  * `.shape`
  * `.head()`
* Removed unnecessary columns.

### 2. Exploratory Data Analysis (EDA)

Performed:

* Box plots for:

  * Age
  * Annual Income
  * Spending Score
* Histogram for Annual Income distribution.

### 3. Finding Optimal Clusters

Used the **Elbow Method** to determine the ideal number of clusters by analyzing the Within-Cluster Sum of Squares (WCSS).

**Optimal Clusters Selected:** 4

### 4. K-Means Clustering

Applied K-Means with:

* Number of clusters = 4
* Random State = 42

Cluster labels were assigned to each customer.

### 5. Cluster Analysis

Examined cluster centers to understand customer characteristics and assigned meaningful names to each segment.

### 6. Visualization

Created scatter plots showing:

* Annual Income vs Spending Score
* Customer clusters
* Cluster centroids

### 7. Prediction

Predicted the segment for new customer data using the trained K-Means model.

---

## 📈 Customer Segments Identified

### Cluster 0 – Average Spenders

* Medium income
* Moderate spending behavior
* Regular customers

### Cluster 1 – High Income, High Spenders

* High annual income
* High spending score
* Premium customers

### Cluster 2 – Young, Low Income, High Spenders

* Younger customers
* Lower income levels
* High spending habits

### Cluster 3 – High Income, Low Spenders

* High income
* Low spending score
* Potential customers for promotional campaigns

---

## 📷 Visualization

### Elbow Method

Used to determine the optimal number of clusters.

### Customer Segmentation Plot

* X-axis: Annual Income (k$)
* Y-axis: Spending Score (1-100)
* Different colors represent different customer segments.
* Cluster centers highlighted for better interpretation.

---

## 📌 Results

The K-Means model successfully segmented **200 mall customers into 4 meaningful groups**. These customer segments can be used to:

* Develop personalized marketing campaigns.
* Recommend products based on customer behavior.
* Improve customer retention strategies.
* Identify high-value customers.

---

## 🔮 Future Enhancements

* Use additional customer attributes.
* Apply Hierarchical Clustering and DBSCAN for comparison.
* Build an interactive dashboard using Power BI or Streamlit.
* Deploy the model as a web application.

---

## 👨‍💻 Author

**Sudharshan Gavvala**

* Aspiring Data Scientist & Machine Learning Enthusiast
* GitHub: https://github.com/SudharshanGavvala/
* LinkedIn: https://www.linkedin.com/in/sudharshangavvala/
