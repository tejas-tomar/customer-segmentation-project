# Customer Segmentation Analysis (RFM + K-Means)

An end-to-end analytics project that segments customers using **RFM analysis** (Recency, Frequency, Monetary) and **K-means clustering**, then translates those segments into actionable business insights through an interactive Tableau dashboard.

---

## 📊 Tableau Dashboard

View the interactive dashboard:  
https://public.tableau.com/views/CustomerSegmentationDashboardRFMAnalysis_17763658008350/CustomerSegmentationDashboardRFMAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

---

## 🎯 Project Objective

This project answers a key business question:

> How can transactional data be used to segment customers and improve targeting, retention, and revenue strategy?

The goal is to move from raw transaction data → customer segments → business insights.

---

## 🛠 Tech Stack

- **Python** (pandas, NumPy)
- **scikit-learn** (K-means clustering)
- **Matplotlib**
- **Tableau** (data visualization)
- CSV pipeline for dashboard integration

---

## 📁 Dataset

- **Source:** Online Retail transactional dataset  
- **File:** `data/raw/Online Retail.xlsx`  
- Contains customer purchases, timestamps, quantities, and pricing data

---

## ⚙️ Methodology

### 1. Data Cleaning
- Removed missing customer IDs  
- Filtered out canceled orders and negative quantities  
- Created feature: `TotalPrice = Quantity × UnitPrice`  

### 2. Feature Engineering (RFM)
- **Recency:** Days since last purchase  
- **Frequency:** Number of transactions  
- **Monetary:** Total customer spend  

### 3. Modeling
- Scaled RFM features  
- Applied **K-means clustering** to identify customer groups  

### 4. Segmentation
- Translated clusters into business-friendly segments  
- Created structured outputs for analysis and visualization  

### 5. Visualization
- Built an interactive Tableau dashboard showing:
  - Customer distribution  
  - Revenue contribution  
  - Behavioral segmentation  

---

## 👥 Final Customer Segments

- **VIP Customers:** high spend, frequent purchases, recent activity  
- **Loyal Customers:** consistent repeat buyers with strong revenue contribution  
- **Potential Customers:** low-spend but active customers with growth potential  
- **At-Risk Customers:** high recency and low engagement, indicating churn risk  

---

## 🔍 Key Insights

- The dataset includes **4,338 customers** and **~$8.9M in total revenue**  
- **Potential customers** represent ~70% of the customer base but have low average spend  
- **Loyal customers** contribute a significant portion of revenue despite a smaller population  
- **VIP customers** are a small segment but generate the highest value per customer  
- **At-Risk customers** show high recency and low spend, signaling disengagement and retention opportunities  

---

## 💡 Business Impact

This analysis enables companies to:

- Prioritize **high-value customer retention (VIP & Loyal)**  
- Identify **upsell opportunities (Potential customers)**  
- Target **churn prevention strategies (At-Risk customers)**  
- Make **data-driven marketing and revenue decisions**  

---

## 🚀 Project Highlights

- Built a full pipeline from raw data → clustering → dashboard  
- Combined **machine learning + business interpretation**  
- Designed a **clean, interactive Tableau dashboard** for stakeholder use  

---
