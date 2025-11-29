# 🛍️ Customer Purchase Behavior Segmentation (Unsupervised Clustering)

> A complete end-to-end **Machine Learning Project** for identifying customer segments using **unsupervised clustering** techniques.

---

## 📊 Project Overview

In today’s competitive market, understanding customer behavior is crucial for personalized marketing and retention.  
This project uses **unsupervised machine learning** to analyze and segment customers based on their **purchase patterns, income, spending score, and frequency**.

We apply multiple clustering algorithms to create meaningful customer groups and help businesses tailor their strategies for each segment.

---

## 🧠 Objectives

- Understand customer purchase behavior using **EDA & visualization**
- Segment customers using **K-Means**
- Evaluate clustering performance using **Silhouette Score**
- Store and query data using **MySQL**
- Generate actionable business insights for marketing teams

---

## ⚙️ Tech Stack

| Category | Tools / Libraries |
|-----------|------------------|
| **Language** | Python 3 |
| **Libraries** | pandas, numpy, matplotlib, seaborn, scikit-learn, scipy |
| **Database** | MySQL |
| **Visualization** | Matplotlib, Seaborn |
| **Model Evaluation** | Silhouette Score |
| **Data Storage** | CSV, MySQL |

---

## 🧩 Project Workflow

### **1️⃣ Dataset**
- **10,000 customer records**
- 4 true customer groups:
  - **Budget Shoppers**
  - **Regular Buyers**
  - **Premium Loyalists**
  - **Young Impulsives**
- Added **dirty and inconsistent data** for realism:
  - Missing values  
  - Typos & inconsistent formatting  
  - Outliers  
  - Duplicate records  
  - Wrong data types & date formats  

---

### **2️⃣ Data Cleaning**
- Standardized categorical values (e.g. “femail” → “Female”)
- Fixed wrong data types and date formats  
- Removed duplicates and outliers using IQR  
- Filled missing values with median/mode  
- Saved as: `customer_purchase_behavior_cleaned.csv`

---

### **3️⃣ Exploratory Data Analysis**

### **MySQL Integration**
- Stored cleaned dataset in MySQL using `mysql-connector-python`
- Performed SQL analytical queries
  
---

### **EDA with Matplotlib and Seaborn**
  
**Tools:** Pandas, Matplotlib, Seaborn

---

### **4️⃣ Data Preprocessing & Modeling**
- Scaled numerical features with `StandardScaler`
- Applied multiple clustering algorithms:
  - **K-Means**

---

### **5️⃣ Model Evaluation**
| Algorithm | Best Params | Silhouette Score | Comment |
|------------|-------------|------------------|----------|
| KMeans | k=4 | **0.61** | Best performance |

---

### **6️⃣ Business Insights**
| Segment | Description | Behavior |
|----------|--------------|-----------|
| **Budget Shoppers** | Low income, low spending, few purchases | Prefer groceries |
| **Regular Buyers** | Mid income, moderate spending | Loyal, prefer clothing |
| **Premium Loyalists** | High income, high spending, frequent purchases | Prefer electronics & beauty |
| **Young Impulsives** | Young, mid-income, high spending | Prefer sports & fashion |

---

## 🧮 Evaluation Metric: Silhouette Score

| Range | Interpretation |
|--------|----------------|
| 0.5 – 1.0 | Excellent clustering |
| 0.2 – 0.5 | Moderate clustering |
| < 0.2 | Poor clustering |

---
