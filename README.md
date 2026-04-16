# Customer Segmentation Analysis

A portfolio-ready analytics project that uses **RFM analysis** and **K-means clustering** to segment customers from the Online Retail transactional dataset. The project identifies high-value, core, promising, and at-risk customer groups, then translates those segments into dashboard-ready business insights.

## Project Objective
The goal of this project is to answer a simple business question:

> How can a company use transaction data to group customers into meaningful segments and improve targeting, retention, and revenue strategy?

## Tools Used
- Python
- pandas / NumPy
- scikit-learn
- Matplotlib
- Tableau-ready CSV outputs

## Dataset
- Source: Online Retail transactional dataset
- File used: `data/raw/Online Retail.xlsx`
  
## Methodology
1. Cleaned the raw transactional data
   - removed missing customer IDs
   - removed canceled orders and negative quantities
   - created `TotalPrice = Quantity x UnitPrice`
2. Built **RFM features** for each customer
   - Recency = days since most recent purchase
   - Frequency = number of unique invoices
   - Monetary = total spend
3. Scaled log-transformed RFM data and applied **K-means clustering**
4. Interpreted clusters into business-friendly segment names
5. Exported dashboard-ready outputs for Tableau and created portfolio visuals

## Final Segments
- VIP Loyalists: high spend, frequent purchases, recent activity
- Core Customers: strong repeat buyers with solid revenue contribution
- Promising New Customers: newer customers with room to grow
- At-Risk Customers: older/lapsed customers with low recent engagement

## Key Findings
- The dataset contains **4,338 customers** and **$6.94M** in total modeled revenue.
- **VIP Loyalists** account for roughly **57.0% of total revenue** while representing only **17.0% of customers**.
- **At-Risk Customers** make up the largest share of customers at **36.7%**, but contribute only **7.9% of revenue**.
- **Core Customers** contribute about **28.8% of revenue**, making them the largest growth-retention opportunity after VIP customers.
- The average modeled customer value is **$1,599**, and average recency is **93 days**.

