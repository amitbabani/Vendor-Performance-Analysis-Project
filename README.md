📊 Vendor Performance Analysis

This project analyzes vendor performance using Python, SQLite, and Power BI. It focuses on integrating purchase, sales, and inventory data to generate insights on profitability, vendor contribution, and inventory management.

🚀 Project Workflow
1️⃣ get_vendor_summary.py

Extracts and prepares raw vendor data.

Joins key tables: purchases, sales, purchase prices, and invoices.

Creates a vendor_sales_summary table with consolidated metrics.

2️⃣ ingest_db.py

Loads and stores the processed data into a SQLite database.

Ensures efficient storage for large datasets (over 2.2 GB database).

Optimizes schema for faster queries and dashboarding.

3️⃣ EDA.ipynb

Performs Exploratory Data Analysis on the vendor_sales_summary table.

Generates descriptive statistics and correlation heatmaps.

Identifies anomalies such as negative profit margins, unsold inventory, and outliers.

Prepares cleaned datasets for downstream reporting.

4️⃣ Vendor Performance Analysis.ipynb

Builds advanced KPIs:

Gross Profit

Profit Margin

Stock Turnover

Sales-to-Purchase Ratio

Net Profit

Performs statistical tests to compare high vs. low-performing vendors.

Creates Power BI dashboards for visual insights.

📂 Data Files

purchases.xlsx – Purchase transactions.

purchase_prices.xlsx – Product prices by vendor.

sales.xlsx – Large sales file with 1.10+ crore rows (~11M records).

vendor_invoice.xlsx – Vendor-level invoices with freight details.

inventory.db – Final SQLite database (~2.2 GB) containing consolidated data.

📈 Key Insights

Top 10 vendors contribute ~65% of purchases, highlighting dependency risks.

Bulk purchasing reduces unit costs by 72%, improving profitability.

Unsold inventory capital of $2.7M ties up resources.

High-margin but low-sales brands represent untapped growth opportunities.

Statistical validation confirms significant differences between top and low-performing vendors.

🛠️ Tech Stack

Python – Data processing, SQL queries, EDA

SQLite – Database storage & optimization

Power BI – Dashboarding & reporting

Pandas, Matplotlib, Seaborn – Data wrangling and visualization

📌 Next Steps

Automate data ingestion and reporting.

Integrate with cloud services (Azure/BigQuery) for scalability.

Extend analysis to predictive modeling for vendor performance.
