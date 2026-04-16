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

## Tableau Dashboard
View the interactive dashboard:  
(https://public.tableau.com/views/CustomerSegmentationDashboardRFMAnalysis_17763658008350/CustomerSegmentationDashboardRFMAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Final Segments
- VIP Customers: high spend, frequent purchases, recent activity  
- Loyal Customers: consistent repeat buyers with strong revenue contribution  
- Potential Customers: newer or low-spend customers with room to grow  
- At-Risk Customers: customers with high recency and low recent engagement

## Key Findings
- The dataset contains 4,338 customers and ~$8.9M in total revenue.
- Potential customers make up ~70% of the customer base but contribute less revenue per user.
- Loyal customers contribute a significant portion of revenue despite a smaller share of customers.
- VIP customers represent a very small portion of users but have the highest spending behavior.
- At-Risk customers show high recency and low spending, indicating disengagement.

