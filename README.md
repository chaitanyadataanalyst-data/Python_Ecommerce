# 🛒 Pandas E-commerce Sales Project

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning%20%26%20Analysis-green?logo=pandas)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 📌 Project Overview
This project demonstrates a complete data pipeline using only Pandas:
- Data Quality Checks  
- Data Cleaning & Validation  
- Merging multiple raw files  
- Business KPI calculations  
- Insights & Recommendations  
- Exporting final reports  

The dataset simulates an E-commerce business with orders, payments, products, and customers.
---
## 📂 Raw Datasets
- orders_raw.csv → Order details (Order ID, Customer ID, Product ID, Quantity, Discount, Order Date)  
- payments_raw.csv → Payment details (Order ID, Payment Mode, Sales Channel)  
- products_raw.csv → Product details (Product ID, Product Name, Category, Unit Price)  
- customers_raw.csv → Customer details (Customer ID, Name, City, State)  
---

## 🧹 Data Cleaning Highlights
- Removed duplicates: Orders (250 final), Customers (120 final), Payments (250 final)  
- Standardized text columns (title case, stripped spaces)  
- Converted dates and numeric columns to correct formats  
- Fixed inconsistent values (e.g.,  Upi  → UPI)  
- Handled missing values carefully (kept as NaN or flagged for review)  
- Validated IDs across datasets  

---

## 📈 Final Business KPIs
- Total Revenue: ₹9,581,450  
- Total Orders: 250  
- Average Order Value (AOV): ₹38,479.72  
- Total Quantity Sold: 1,104 units  
- Number of Customers: 120  
- Number of Products: 25  

---

## 🔎 Revenue Breakdown
-  By City
  - Pune → ₹2,048,750  
  - Delhi → ₹1,694,950  
  - Hyderabad → ₹1,211,650  
  - Nagpur → ₹1,054,800  
  - Thane → ₹1,039,750  
  - Nashik → ₹1,018,250  
  - Mumbai → ₹927,750  
  - Bengaluru → ₹585,550  

-  By Category 
  - Electronics → ₹6,104,550  
  - Furniture → ₹3,163,900  
  - Accessories → ₹294,250  
  - Stationery → ₹18,750  

-  By Product (Top 5)
  - Laptop → ₹2,740,000  
  - Sofa → ₹1,518,150  
  - Smartphone → ₹1,041,200  
  - Tablet → ₹651,250  
  - Table → ₹574,500  

-  By Payment Mode
  - Net Banking → ₹2,287,000  
  - UPI → ₹1,894,050  
  - Debit Card → ₹1,819,750  
  - Credit Card → ₹1,812,450  
  - Cash → ₹1,768,200  

-  By Sales Channel
  - Online → ₹5,459,350  
  - Offline → ₹4,073,150  

---

## 📊 Monthly Sales Trend
- Best Month: March → ₹1,524,350  
- Other strong months: April (₹1,183,800), August (₹1,092,250)  

---

## 👥 Customer Insights
- Top Customer : Pooja → ₹1,438,300 revenue, 27 orders  
-  High Value Customers (≥ ₹500,000) : Pooja, Kavya, Nisha, Raj, Sneha, Akash, Amit  
-  Low Value Customers (< ₹200,000) : Riya (₹185,250), Aditya (₹63,700)  
-  Frequent but Lower-Spending : Raj → 24 orders, ₹663,750 revenue (₹27,656 per order)  
-  High-Spending but Less-Frequent : Vikram, Meera, Karan (avg revenue per order > ₹47,000)  

---

## 🛒 Product Performance
-  High Revenue & High Quantity : Laptop, Sofa, Smartphone, Tablet, Table  
-  Top Quantity Sold : Mouse (98 units), Router (72 units), Bookshelf (66 units)  
-  Revenue per Unit Leader : Laptop → ₹54,800 per unit  
-  Negative Revenue Product : Notebook → -₹1,650 (due to excessive discounts)  

---




## 🚨 Discount & Revenue Quality
-  Suspicious Discounts (>50%)  flagged and reviewed  
-  Negative Revenue Orders : 1.2% of dataset, causing ~2% revenue leakage  

---

## 🏆 Business Winners
-  Best City : Pune → ₹2,048,750  
-  Best Category : Electronics → ₹6,104,550  
-  Best Product : Laptop → ₹2,740,000  
-  Best Sales Channel : Online → ₹5,459,350  
-  Best Month : March → ₹1,524,350  

---

## 🎯 Business Recommendations
1.  Expand in Pune  → Highest revenue city, explore new segments and marketing.  
2.  Focus on Electronics  → Promote laptops, smartphones, and tablets with bundles.  
3.  Promote Laptop-related products  → Cross-sell accessories and electronics.  
4.  Strengthen Online Sales  → Invest in digital marketing and online engagement.  
5.  Retain High-Value Customers  → Loyalty programs, personalized offers, exclusive promotions.  
6.  Monitor Discounts  → Prevent excessive discounts that lead to negative revenue.  

---



## 📂 Exported Reports
All cleaned and aggregated outputs are saved in the `final_reports/` folder:
- `cleaned_sales_data.csv`  
- `city_sales.csv`  
- `category_sales.csv`  
- `product_sales.csv`  
- `monthly_sales.csv`  
- `customer_summary.csv`  
- `negative_orders.csv`  
- `final_insights.csv`  

---

## 🛠️ Tools & Libraries
-  Python 3.x 
-  Pandas 
-  OS (for file handling) 

---

