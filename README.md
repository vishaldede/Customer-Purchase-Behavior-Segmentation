# Customer Purchase Behavior Segmentation  
### Unsupervised Machine Learning Project (KMeans Clustering)

## 📌 Project Overview
This project demonstrates the use of **unsupervised learning techniques** to segment customers based on their **purchase behavior**.  
The goal is to identify meaningful customer groups that can be used for **targeted marketing, personalization, and business strategy**.

A dataset including noise and data quality issues, followed by a complete **data cleaning, preprocessing, clustering, and evaluation pipeline**.

---

## 🎯 Business Objective
- Segment customers based on purchasing behavior
- Identify high-value and low-value customer groups
- Understand customer patterns without using labeled data
- Validate clustering quality using **Silhouette Score**

---

## 🗂 Dataset Description
- **Records:** 10,000
- **Target Variable:** None (Unsupervised)

### Features
| Feature | Description |
|------|------------|
| Annual_Income | Customer yearly income |
| Annual_Spend | Total yearly spending |
| Monthly_Visits | Average monthly store/app visits |
| Avg_Order_Value | Average value per purchase |
| Customer_Tenure_Years | Years as a customer |
| Gender | Customer gender (categorical) |
| Preferred_Channel | Shopping channel |

---

## 🧹 Data Cleaning
The dataset intentionally included real-world issues:
- Missing values
- Duplicate records
- Inconsistent categorical values

### Cleaning Steps
- Removed duplicate records
- Standardized categorical values
- Converted data types safely
- Applied **segment-aware median imputation**
- Treated outliers using **IQR capping**
- Preserved cluster structure for ML modeling

---

## 📊 Exploratory Data Analysis (EDA)

Performed using **Pandas, Matplotlib, Seaborn**

---

## ⚙️ Data Preprocessing
- Careful feature selection for clustering
- Feature scaling using **StandardScaler**

---

## 🤖 Model Used
- **Algorithm:** KMeans Clustering
- **Optimal K Selection:** Elbow Method
- **Validation Metric:** Silhouette Score

### Selected Features for Clustering
- Annual_Income
- Annual_Spend
- Monthly_Visits
- Avg_Order_Value

---

## 📈 Model Evaluation
- **Optimal number of clusters:** 4
- **Silhouette Score:** ~0.50 – 0.65
- Strong intra-cluster similarity
- Clear inter-cluster separation

---

## 🏷 Customer Segments Identified
| Cluster | Segment Name |
|------|-------------|
| 3 | Budget Shoppers |
| 1 | Regular Customers |
| 2 | Premium Customers |
| 0 | Loyal Customers |

Cluster labels were assigned based on **cluster centroids**, not numeric order.

---

## 🚀 Key Learnings
- Importance of feature selection in clustering
- Limitations of KMeans with categorical data
- How Silhouette Score reacts to noise and dimensionality
- Translating clusters into business insights

---

## 🛠 Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## 📌 Future Improvements
- PCA for dimensionality reduction
- Hierarchical clustering comparison

---



