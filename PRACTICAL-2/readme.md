# Power BI Practical – Sales & Returns Analysis

## Project Overview

This practical demonstrates the complete Power BI workflow using multiple Excel datasets. The project focuses on:

- Importing datasets from Excel files
- Performing data cleaning and transformation using Power Query Editor
- Building a star schema data model
- Creating relationships between fact and dimension tables
- Designing report visuals for business insights

The practical was implemented using Power BI Desktop.

---

# Dataset Information

The following datasets were provided as Excel files:

| Dataset             | Type            | Description                                                           |
| ------------------- | --------------- | --------------------------------------------------------------------- |
| `Sales_Fact.xlsx`   | Fact Table      | Contains sales transactions including quantity, revenue, and discount |
| `Returns_Fact.xlsx` | Fact Table      | Contains product return details and return reasons                    |
| `Customer_Dim.xlsx` | Dimension Table | Customer demographic and segment information                          |
| `Product_Dim.xlsx`  | Dimension Table | Product, category, brand, and subcategory information                 |
| `Region_Dim.xlsx`   | Dimension Table | Country, state, and city information                                  |
| `Date_Dim.xlsx`     | Dimension Table | Date hierarchy including month, quarter, year, and fiscal year        |

---

# Data Import Process

The datasets were imported into Power BI using Excel workbook connections.

Imported tables:

- Sales Fact
- Returns Fact
- Customer Dimension
- Product Dimension
- Region Dimension
- Date Dimension

---

# Power Query Transformations Performed

The following transformation operations were performed using Power Query Editor:

## 1. Data Cleaning

- Verified and corrected column data types
- Checked for null values
- Removed unnecessary inconsistencies
- Ensured numeric columns were properly formatted

## 2. Column Standardization

- Standardized field names for readability
- Maintained consistent naming conventions across datasets

## 3. Data Validation

- Validated relationships between fact and dimension tables
- Ensured keys matched correctly

## 4. Data Preparation for Modeling

- Prepared dimension tables for relationship creation
- Structured fact tables for analysis and reporting

---

# Data Model Design

A star schema model was created in Power BI.

## Fact Tables

### Sales Fact

Contains:

- SalesID
- CustomerID
- ProductID
- RegionID
- DateKey
- Quantity
- Revenue
- Discount

### Returns Fact

Contains:

- ReturnID
- SalesID
- ReturnDateKey
- Reason

## Dimension Tables

### Customer Dimension

Contains customer-related attributes:

- Customer Name
- Age
- Gender
- Segment

### Product Dimension

Contains product-related attributes:

- Product Name
- Category
- Subcategory
- Brand

### Region Dimension

Contains geographic details:

- Country
- State
- City

### Date Dimension

Contains date hierarchy:

- Date
- Month
- Quarter
- Year
- Fiscal Year

---

# Relationships Created

The following relationships were established in the model view:

| From Table   | Column     | To Table           | Column     |
| ------------ | ---------- | ------------------ | ---------- |
| Sales Fact   | CustomerID | Customer Dimension | CustomerID |
| Sales Fact   | ProductID  | Product Dimension  | ProductID  |
| Sales Fact   | RegionID   | Region Dimension   | RegionID   |
| Sales Fact   | DateKey    | Date Dimension     | DateKey    |
| Returns Fact | SalesID    | Sales Fact         | SalesID    |

The model follows a centralized fact table approach for optimized reporting.

---

# Report Visualizations Created

The report page includes multiple table visuals for analysis.

## 1. Product Category Sales Analysis

Visual displays:

- Product Category
- Total Quantity Sold
- Total Revenue
- Country-wise analysis

Purpose:

- Analyze revenue generation across product categories and regions.

---

## 2. Returns Analysis

Visual displays:

- Fiscal Year
- Return Reason

Purpose:

- Understand return patterns and return reasons across fiscal periods.

---

## 3. Customer Segment Revenue Analysis

Visual displays:

- Customer Segment
- Total Revenue

Purpose:

- Identify which customer segments generate the highest revenue.

---

# Key Learning Outcomes

This practical helped in understanding:

- Power BI data import process
- Power Query Editor transformations
- Data cleaning techniques
- Star schema modeling
- Relationship management
- Fact and dimension table concepts
- Report building and visualization
- Business intelligence reporting workflow

---

# Tools & Technologies Used

- Power BI Desktop
- Power Query Editor
- Microsoft Excel

---

# Conclusion

This practical demonstrates the end-to-end implementation of a Power BI reporting solution using multiple Excel datasets. The project covers data preparation, transformation, modeling, and report visualization to generate meaningful business insights from sales and returns data.
