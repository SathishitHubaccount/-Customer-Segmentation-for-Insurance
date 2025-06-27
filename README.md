# 📊 Insurance Customer Segmentation using DBSCAN

This project applies **unsupervised clustering** techniques on insurance customer data to identify distinct customer segments. After testing multiple clustering models, **DBSCAN** achieved the highest performance with a **Silhouette Score of 1.000**, indicating very clear and meaningful clusters.

---

## 🔍 Problem Statement

Insurance companies need to understand customer behavior to:
- Personalize offers
- Predict churn
- Optimize risk models

Traditional segmentation methods fail when data has noise or irregular cluster shapes. This project uses **DBSCAN** to uncover hidden structure in complex, real-world insurance data.

---

## 🧠 Key Features in Dataset

| Feature | Description |
|---------|-------------|
| Age | Customer's age |
| Claims_Frequency | Number of claims filed |
| Premium_Amount | Annual premium paid |
| Credit_Score | Customer's creditworthiness |
| Website_Visits | Website interaction frequency |
| Time_to_Conversion | Time taken to convert after first contact |
| Total_Discounts | Combined discounts applied |
| Policy_Type, Region, etc. | Categorical fields |

---

## 🧪 Models Tested

| Model              | Score/Notes |
|--------------------|-------------|
| **K-Means**        | Poor Silhouette Score (0.072) |
| **DBSCAN**         | ⭐ **Best - Silhouette Score: 1.000** |

---

## ✅ DBSCAN Results

- **Perfect cluster separation** (Silhouette Score: 1.000)
- **Outliers detected** and removed (`Cluster -1`)
- Created interpretable customer segments:
  - **Loyal Low-Risk**
  - **High-Claim Young Users**
  - **Inactive Browsers**
  - **Outliers**

---

## 📊 Segment Summary Example

| Cluster | Avg Premium | Avg Claims | Avg Credit Score | Description |
|---------|-------------|------------|------------------|-------------|
| 0       | ₹15,200     | 0.2        | 740              | Loyal & low-risk |
| 1       | ₹8,100      | 2.4        | 610              | High-claim users |
| -1      | —           | —          | —                | Outliers |

---

## 🛠 Tech Stack

- **Python**
- **Scikit-learn**
- **Pandas, NumPy, Matplotlib, Seaborn**
- **DBSCAN, PCA, Silhouette Score**

---

## 📌 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/SathishitHubaccount/-Customer-Segmentation-for-Insurance.git
   cd CustomerSegmentationforInsurancen
