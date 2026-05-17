# Data Leverage - Power Query Transformation Project

## Project Overview

This project focuses on performing data transformation and ETL operations using Power BI Power Query. Multiple datasets were imported using different data ingestion methods, followed by cleaning, transformation, merging, appending, and aggregation operations.

The project demonstrates practical Power Query skills commonly used in real-world data analyst workflows.

---

## Datasets Used

### 1. Country Wise Population Dataset

Source:

- [https://www.worldometers.info/world-population/population-by-country](https://www.worldometers.info/world-population/population-by-country)

Imported directly from the web into Power BI.

### 2. Sales Datasets

- Three separate yearly sales datasets were imported using Folder Import.

### 3. Employee Dataset

- Imported from a worksheet inside an Excel workbook.

---

## Import Techniques Used

Different data import methods were utilized in this project:

- Web Import
- Folder Import
- Excel Workbook Sheet Import

---

## Data Cleaning Performed

The following cleaning operations were performed across datasets:

- Renamed columns for better readability
- Removed null values
- Removed duplicate records
- Removed errors from columns
- Corrected incorrect data types

Example:

- Corrected percentage columns in the population dataset

---

## Data Transformations Performed

### Sales Dataset Transformations

- Extracted `OrderMonth` from order date
- Extracted `OrderYear` from order date
- Replaced `%` symbols with empty values to resolve datatype conversion issues

### Employee Dataset Transformations

- Created `BirthYear` column using employee age
- Created conditional column `EmployeeType` based on `ExperienceInDomain`

Example:

- Fresher
- Experienced

### Indexing

- Added both `0-Based Index` and `1-Based Index` columns across datasets

---

## Merging and Appending

### Merge Operation

- Merged Employee and Sales datasets using Index column

### Append Operation

- Appended all three yearly sales datasets into a single consolidated table

---

## Aggregation and Analysis

Used Group By feature in Power Query to:

- Calculate Year-wise Total Sold Quantity

---

## Power BI Features Used

- Power Query Editor
- Web Data Import
- Folder Import
- Excel Workbook Import
- Column Renaming
- Data Type Transformation
- Replace Values
- Conditional Columns
- Extract Transformations
- Merge Queries
- Append Queries
- Group By
- Index Columns
- Error Handling
- Duplicate Removal

---

## Skills Demonstrated

- Data Cleaning
- ETL Operations
- Data Transformation
- Power Query
- Data Integration
- Data Preparation
- Power BI
- Data Aggregation
- Query Optimization
