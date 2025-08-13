# Sales Analytics Dashboard — Power BI & BigQuery

## 📌 Project Overview

This project is a real-time business intelligence solution designed to help sales leadership monitor performance, identify trends, and make data-driven decisions. The dashboard consolidates multi-source sales data from disparate systems into a single, unified view with advanced KPIs, interactive visuals, and automated refresh capabilities.

By leveraging **Google BigQuery** for cloud-based storage and query execution, and **Power BI** for visualization and analytics, this solution reduced manual reporting efforts by **12 hours per week** and provided instant, actionable insights to stakeholders.

-----

## 🎯 Objectives

  * Consolidate data from multiple sales databases into a single, interactive dashboard.
  * Automate data refresh for real-time analytics.
  * Provide leadership with key sales performance metrics and actionable insights.
  * Reduce manual report preparation time and improve decision-making speed.

-----

## 📂 Data Sources

The project integrates and transforms data from multiple systems, including:

  * **CRM Database** — Customer and account details.
  * **ERP System** — Transactional sales orders, invoicing, and payment status.
  * **Regional Pricing Data** — For median price comparisons.
  * **Google Sheets / Excel** — Ad-hoc sales target data provided by managers.

All data is ingested into **Google BigQuery** for centralized querying.

-----

## 🛠️ Tools & Technologies

| Category | Tool / Technology |
| :--- | :--- |
| **Cloud Platform** | Google Cloud Platform (GCP) |
| **Database & Query Engine** | Google BigQuery |
| **Visualization Tool** | Power BI Desktop / Power BI Service |
| **Data Transformation** | Power Query |
| **Calculation Language** | DAX (Data Analysis Expressions) |
| **Data Manipulation** | Microsoft Excel |

-----

## ⚙️ Data Processing Workflow

### Data Ingestion

Sales, customer, and pricing data are imported into Google BigQuery from multiple sources (CRM, ERP, spreadsheets) using BigQuery connectors and scheduled ETL jobs.

### Data Transformation

Transformations applied in **Power Query** include:

  * Column renaming and formatting.
  * Null value handling and data type corrections.
  * Merging datasets on customer and order keys.
  * Calculating derived fields (e.g., profit margin %, discount %).

### Data Modeling

A **star schema** design is implemented with:

  * **Fact Table**: Sales transactions.
  * **Dimension Tables**: Customers, Products, Regions, Dates.

Relationship mapping is used for optimal **DAX** performance.

### Metric Calculations (DAX)

Key metrics calculated using DAX include:

  * YOY Sales Growth
  * Regional Median Price
  * Rolling 12-Month Sales Total
  * YTD Performance
  * Average Order Value (AOV), Win Rate, and Sales per Region.

### Visualization & Dashboard Design

Interactive visuals in the dashboard include:

  * KPI cards for high-level metrics.
  * Line charts for sales trends.
  * Bar charts for regional performance.
  * Map visuals for geospatial sales insights.
  * Slicers for product category, date, and region filtering.

### Deployment & Automation

The report is published to the **Power BI Service**. A scheduled refresh is configured via the BigQuery connector for real-time updates. The dashboard is shared with sales leadership through a Power BI app workspace with role-based access.

-----

## 📊 Key Features

  * **Real-time Insights** — Automatic daily data refresh via the BigQuery connector.
  * **Custom DAX Metrics** — Complex KPIs for accurate business tracking.
  * **Interactive Filtering** — Region, product, and date-based drill-downs.
  * **Performance Benchmarking** — YOY, YTD, and rolling totals for trend analysis.
  * **Data Integration** — Consolidates CRM, ERP, and manual inputs into one unified view.

-----

## 📈 Business Impact

  * **12 hours/week** saved in manual report preparation.
  * Improved decision-making with real-time visibility into sales metrics.
  * Enabled data-driven performance reviews at regional and product levels.
  * Enhanced forecasting accuracy through historical trend analysis.

-----

## 📷 Dashboard Preview

-----

## 🚀 How to Run Locally

1.  **Clone the repository**:
    ```bash
    git clone [repository-url]
    ```
2.  **Connect Power BI Desktop**:
    Open the Power BI file (`.pbix`) and connect it to your Google BigQuery instance by updating the data source credentials.
