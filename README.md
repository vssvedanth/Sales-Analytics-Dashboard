Sales Analytics Dashboard — Power BI & BigQuery
📌 Project Overview
The Sales Analytics Dashboard is a real-time business intelligence solution designed to help sales leadership monitor performance, identify trends, and make data-driven decisions.
The project integrates multi-source sales data from disparate systems into a single, unified dashboard with advanced KPIs, interactive visuals, and automated refresh capabilities.

By leveraging Google BigQuery for cloud-based storage and query execution, and Power BI for visualization and analytics, the solution reduced manual reporting efforts by 12 hours per week and provided instant, actionable insights to stakeholders.

🎯 Objectives
Consolidate data from multiple sales databases into a single, interactive dashboard.

Automate data refresh for real-time analytics.

Provide leadership with key sales performance metrics and actionable insights.

Reduce manual report preparation time and improve decision-making speed.

📂 Data Sources
The project integrates and transforms data from multiple systems, including:

CRM Database — Customer and account details.

ERP System — Transactional sales orders, invoicing, and payment status.

Regional Pricing Data — For median price comparisons.

Google Sheets / Excel — Ad-hoc sales target data provided by managers.

Data from all sources is ingested into Google BigQuery for centralized querying.

🛠️ Tools & Technologies
Cloud Platform: Google Cloud Platform (GCP)

Database & Query Engine: Google BigQuery

Visualization Tool: Power BI Desktop / Power BI Service

Data Transformation: Power Query

Calculation Language: DAX (Data Analysis Expressions)

Data Manipulation: Microsoft Excel

⚙️ Data Processing Workflow
Data Ingestion

Sales, customer, and pricing data imported into Google BigQuery from multiple sources (CRM, ERP, spreadsheets).

Data loaded via BigQuery connectors and scheduled ETL jobs.

Data Transformation

Applied transformations in Power Query:

Column renaming and formatting.

Null value handling and data type corrections.

Merging datasets on customer and order keys.

Calculating derived fields (profit margin %, discount %, etc.).

Data Modeling

Star schema design with:

Fact Table: Sales transactions.

Dimension Tables: Customers, Products, Regions, Dates.

Relationship mapping for optimal DAX performance.

Metric Calculations (DAX)

YOY Sales Growth

Regional Median Price

Rolling 12-Month Sales Total

YTD Performance

Average Order Value (AOV), Win Rate, and Sales per Region.

Visualization & Dashboard Design

Interactive visuals including:

KPI cards for high-level metrics.

Line charts for sales trends.

Bar charts for regional performance.

Map visuals for geospatial sales insights.

Slicers for product category, date, and region filtering.

Deployment & Automation

Published report to Power BI Service.

Configured scheduled refresh via BigQuery connector for real-time updates.

Shared with sales leadership via Power BI app workspace with role-based access.

📊 Key Features
Real-time Insights — Automatic daily data refresh via BigQuery connector.

Custom DAX Metrics — Complex KPIs for accurate business tracking.

Interactive Filtering — Region, product, and date-based drill-downs.

Performance Benchmarking — YOY, YTD, and rolling totals for trend analysis.

Data Integration — Consolidates CRM, ERP, and manual inputs into one unified view.

📈 Business Impact
12 hours/week saved in manual report preparation.

Improved decision-making with real-time visibility into sales metrics.

Enabled data-driven performance reviews at regional and product levels.

Enhanced forecasting accuracy through historical trend analysis.

📷 Dashboard Preview


🚀 How to Run Locally
Clone the repository.

Connect your Power BI Desktop file to your Google BigQuery instance.

