# 🛒 E-Commerce Sales Funnel Analysis (SQL)

Analysis of 100K+ orders from the Olist Brazilian E-Commerce platform to uncover revenue trends, delivery performance, customer behavior, and seller insights using MySQL.

## 📌 Problem Statement
Olist, Brazil's largest e-commerce marketplace, needed visibility into where customers drop off in the sales funnel, which product categories drive revenue, how delivery delays affect customer satisfaction, and which sellers/states perform best. This project answers those questions purely through SQL.

## 📊 Dataset
- **Source:** [Olist Brazilian E-Commerce Public Dataset – Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- **Size:** ~100,000 orders (2016–2018), 9 relational CSV files
- **Tables used:** customers, orders, order_items, order_payments, order_reviews, products, sellers, category_translation

## 🛠️ Tools & Skills
`MySQL 8.0` · `SQL Joins` · `Window Functions` · `Aggregations` · `CTEs` · `Date Functions` · `Business Analytics`

## 🔍 Approach
1. Designed a normalized relational schema (8 tables) matching the Olist data model
2. Imported all CSVs into MySQL
3. Wrote 15 analytical queries covering the full sales funnel — from order placement to delivery to review
4. Interpreted results to surface actionable business insights

## 📈 Key Findings
- **Order funnel:** ~97% of orders reach "delivered" status; cancellation/unavailability is a small but trackable leak point
- **Revenue concentration:** Top 10 product categories account for a disproportionate share of total revenue
- **Delivery performance:** Actual delivery time is well below the estimated delivery window in most cases, but a measurable % of orders still arrive late
- **Payments:** Credit card is the dominant payment method; installment usage varies significantly by payment type
- **Customer base:** The vast majority of customers are one-time buyers — repeat purchase rate is a clear growth opportunity
- **Geography:** Revenue and customer base are heavily concentrated in a handful of states (São Paulo leading)

## 📂 Files
- `ecommerce_sales_funnel_analysis.sql` — full schema + 15 queries

## 🚀 How to Run
1. Download the 9 CSVs from the [Kaggle dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
2. Create the database using the schema in the `.sql` file
3. Import each CSV into its matching table (MySQL Workbench → Table Data Import Wizard, or `LOAD DATA INFILE`)
4. Run the 15 queries to reproduce the analysis

## 👤 Author
**Kiran Garje**
[GitHub](https://github.com/karangarje48) · [LinkedIn](https://linkedin.com/in/kirangarje)
