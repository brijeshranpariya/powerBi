# Corporate Sales Analysis Dashboard

## Project Overview

This project is a **Sales Analysis Dashboard** developed in **Microsoft
Power BI**. The objective of this project was to transform raw
sales-related data into an interactive business intelligence report that
helps users understand sales performance, customer behavior, product
performance, regional trends, and return analysis.

The dashboard was created by cleaning, transforming, modeling, and
visualizing the provided dataset to generate meaningful insights through
interactive reports.

---

## Tools & Technologies Used

- **Microsoft Power BI**
  - Power Query Editor (Data Cleaning & Transformation)
  - Data Modeling
  - DAX Measures
  - Interactive Visualizations
  - Dashboard Design
- **Microsoft Excel**
  - Source Dataset

---

## Dataset Description

The project dataset contains multiple tables following a dimensional
modeling approach.

### Dimension Tables

### Customer Dimension (`Customer_Dim`)

Contains customer-related information:

- Customer ID
- Customer Name
- Email
- Customer Segment
- Customer Region

Used for analyzing sales based on customer categories and regions.

---

### Product Dimension (`Product_Dim`)

Contains product information:

- Product ID
- Product Name
- Category
- Sub Category
- Product Price

Used for product-level sales and category performance analysis.

---

### Date Dimension (`Date_Dim`)

A dedicated date table was created to support time-based analysis.

Includes:

- Date ID
- Date
- Year
- Month
- Quarter

This table enables:

- Year-wise analysis
- Monthly trends
- Quarterly comparison
- Time intelligence calculations

---

### Region Dimension (`Region_Dim`)

Contains regional information:

- Region ID
- Region Name
- Regional Manager

Used for region-based performance tracking.

---

### Fact Tables

### Sales Fact (`Sales_Fact`)

Contains transaction-level sales data:

- Sale ID
- Customer ID
- Product ID
- Date ID
- Units Sold
- Total Sales Amount

This table is used as the main source for sales calculations.

---

### Returns Fact (`Returns_Fact`)

Contains product return details:

- Return ID
- Sale ID
- Return Reason
- Return Date

Used to analyze returned products and return patterns.

---

# Data Preparation & Transformation

The dataset was imported into Power BI and processed using Power Query.

The following transformations were performed:

- Data type corrections
- Date formatting
- Relationship preparation
- Data validation
- Table structuring
- Creation of a proper data model

A star schema model was implemented where dimension tables connect with
fact tables.

---

# Data Model Design

The dashboard follows a **Star Schema Architecture**.

Relationships created:

- Customer Dimension → Sales Fact
- Product Dimension → Sales Fact
- Date Dimension → Sales Fact
- Region Dimension → Customer/Sales analysis
- Sales Fact → Returns Fact

This structure improves:

- Report performance
- DAX calculations
- Filtering behavior
- Data analysis flexibility

---

# Dashboard Features Implemented

## KPI Analysis

Created KPI cards to display important business metrics such as:

- Total Sales
- Total Units Sold
- Profit/Sales Performance Indicators
- Monthly comparison metrics

These KPIs provide a quick overview of business performance.

---

## Sales Trend Analysis

Implemented time-series visuals to analyze:

- Daily sales movement
- Monthly sales trends
- Year-wise comparison

This helps identify growth patterns and sales fluctuations.

---

## Customer Analysis

The dashboard provides customer-based insights:

- Customer segment performance
- Region-wise customer contribution
- Customer sales distribution

This helps understand which customer groups generate the highest
revenue.

---

## Product Performance Analysis

Product analysis includes:

- Category-wise sales
- Sub-category performance
- Top-performing products
- Product contribution toward revenue

This helps identify high-value products and categories.

---

## Regional Sales Analysis

Regional performance analysis includes:

- Sales by region
- Regional comparison
- Manager-level regional insights

This helps compare business performance across different locations.

---

## Returns Analysis

Return-related analysis includes:

- Return count tracking
- Return reason analysis
- Return trends

This helps identify operational issues affecting customer satisfaction.

---

# Interactive Features

The dashboard includes interactive Power BI features:

- Slicers for filtering data
- Cross-filtering between visuals
- Drill-down capabilities
- Dynamic visual updates
- Interactive charts and cards

Users can explore the report by selecting different:

- Years
- Months
- Regions
- Categories
- Segments

---

# Visualizations Used

The report includes:

- KPI Cards
- Line Charts
- Column Charts
- Donut Charts
- Area Charts
- Tables
- Slicers
- Summary Cards

Each visualization was selected to represent the data in a clear and
meaningful way.

---

# Business Insights Covered

The dashboard helps answer questions like:

- How much revenue is generated over time?
- Which products contribute the most sales?
- Which customer segments perform better?
- Which regions generate higher revenue?
- What are the common return reasons?
- How does business performance change month over month?

---

# Project Outcome

This project demonstrates the complete Power BI reporting workflow:

1.  Importing raw business data
2.  Cleaning and transforming data
3.  Building a relational data model
4.  Creating DAX-based calculations
5.  Designing interactive dashboards
6.  Presenting business insights visually

The final dashboard converts raw sales data into an easy-to-understand
analytical report that supports data-driven decision making.

---

## Author

Created as a Power BI Business Intelligence project.
