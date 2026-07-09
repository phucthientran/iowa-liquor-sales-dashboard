📊 Iowa Liquor Sales Analytics Dashboard
Overview

This project demonstrates an end-to-end Business Intelligence solution built using Google BigQuery, SQL, and Power BI.

The objective is to transform raw Iowa Liquor Sales transaction data into a structured analytical model that enables business users to monitor performance, identify growth opportunities, and make data-driven decisions.

The project covers the complete BI workflow:

Raw Dataset
    ↓
Data Cleaning (SQL)
    ↓
Data Warehouse Modeling
    ↓
Star Schema Design
    ↓
DAX KPI Development
    ↓
Interactive Power BI Dashboard
🎯 Business Objectives

This dashboard was designed to answer key business questions:

How are sales performing over time?
Which vendors generate the most revenue?
Which product categories drive business growth?
What products contribute most to sales volume?
How many orders are being processed each month?
How does current performance compare to previous periods?
🛠 Technology Stack
Technology	Purpose
Google BigQuery	Data Storage & Transformation
SQL	Data Cleaning & Data Modeling
Power BI	Data Visualization
DAX	KPI Calculations
GitHub	Documentation & Version Control
📂 Dataset
Source

Iowa Liquor Sales Dataset

This project uses a 10% sample of the original dataset.

Dataset Includes
Invoice Information
Transaction Date
Store Information
Product Information
Vendor Information
Category Information
Bottles Sold
Sales Amount
Volume Sold
🔄 Data Architecture
Iowa Liquor Sales Dataset
            │
            ▼
      Google BigQuery
            │
            ▼
      Data Cleaning
            │
            ▼
      Star Schema
            │
            ▼
         Power BI
            │
            ▼
   Interactive Dashboard
🧹 Data Cleaning & Transformation

Data preparation was performed in Google BigQuery using SQL.

Cleaning Activities

✅ Data Type Standardization

✅ Missing Value Handling

✅ Duplicate Detection

✅ Revenue Validation

✅ Vendor Consistency Checks

✅ Category Consistency Checks

Example SQL
SELECT *
FROM sales
WHERE sale_dollars IS NOT NULL
🏗 Data Model

A Star Schema model was implemented to optimize query performance and simplify reporting.

Fact Table
Fact_Sales

Measures:

Sales Amount
Bottles Sold
Order Count

Foreign Keys:

Date Key
Vendor Key
Category Key
Store Key
Item Key
Dimension Tables
Dim_Date
Date
Month
Year
Dim_Vendor
Vendor Information
Dim_Category
Category Information
Dim_Store
Store Information
Dim_Item
Product Information
⭐ Star Schema

Benefits
Faster dashboard performance
Simplified DAX calculations
Improved scalability
Better analytical flexibility
📈 KPI Development

Measures were created using DAX to support business analysis.

Sales KPIs
Total Sales
Previous Sales
Sales Growth %
Order KPIs
Total Orders
Previous Orders
Order Growth %
Bottles Sold KPIs
Total Bottles Sold
Previous Bottles Sold
Bottles Sold Growth %
Store KPIs
Total Stores
Previous Stores
Store Growth %
Revenue Metrics
Average Order Value
Previous Average Order Value
AOV Growth %
📊 Dashboard Pages
1. Sales Performance Dashboard

Provides visibility into:

Total Sales
Sales Trend
Top Categories by Sales
Top Vendors by Sales
Top Products by Sales
Month-over-Month Sales Growth

2. Order Analysis Dashboard

Provides visibility into:

Total Orders
Order Trend
Top Categories by Orders
Top Vendors by Orders
Top Products by Orders
Month-over-Month Order Growth

3. Bottles Sold Dashboard

Provides visibility into:

Total Bottles Sold
Volume Trend
Top Categories by Bottles Sold
Top Vendors by Bottles Sold
Top Products by Bottles Sold
Month-over-Month Volume Growth

💡 Key Insights
Revenue
Total sales reached $36.77M.
Revenue decreased 6.6% compared to the previous period.
Product Performance
American Vodka generated the highest revenue.
Tito's Handmade Vodka was the leading product by sales.
Vendor Performance
Diageo was the highest revenue-generating vendor.
Sazerac led bottle volume sales.
Business Trend
Sales and order volume peaked during May 2024.
June 2024 showed a decline across key KPIs.
🚀 Skills Demonstrated
Data Engineering
SQL Data Cleaning
Data Transformation
Data Validation
BigQuery Development
Data Modeling
Star Schema Design
Fact & Dimension Modeling
Relationship Management
Business Intelligence
DAX Development
KPI Design
Dashboard Development
Interactive Reporting
Analytics
Sales Analysis
Product Analysis
Vendor Analysis
Time-Series Analysis
Performance Monitoring
👨‍💻 Author: Tran Thien Phuc
