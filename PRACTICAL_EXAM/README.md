# Student Performance Analytics Dashboard

## Overview

This project is a Power BI dashboard created to analyze student performance, attendance, academic scores, and behavior patterns.

The main goal of this project was to transform raw student data into meaningful insights that can help teachers and administrators understand student progress, identify improvement areas, and track overall academic performance.

The dashboard includes interactive reports for analyzing:

- Student demographics
- Attendance trends
- Subject-wise performance
- Exam performance
- Behavioral records
- Individual student profiles

---

## Project Dataset

The project uses multiple datasets:

### Students Dataset

Contains basic student information such as:

- Student ID
- Name
- Gender
- Class
- Section

This table works as the main student dimension table.

### Attendance Dataset

Contains attendance records of students including:

- Student ID
- Attendance status
- Absence details
- Date information

This data is used to calculate attendance percentage and identify attendance patterns.

### Scores Dataset

Contains academic performance details:

- Student ID
- Subject
- Exam Type
- Term
- Marks obtained

This table is used to analyze student scores and subject-wise performance.

### Behavior Dataset

Contains student activity and behavior records such as:

- Positive behavior
- Late arrivals
- Classroom issues
- Other observations

This helps in understanding student engagement beyond academics.

---

# Data Preparation (Power Query)

Before creating the dashboard, I cleaned and transformed the raw data using Power Query.

The following steps were performed:

- Changed incorrect data types
- Cleaned text values
- Removed unnecessary columns
- Handled missing values
- Standardized category values
- Removed duplicate records
- Prepared tables for reporting

This ensured that the data was consistent and ready for analysis.

---

# Data Model

The report follows a Star Schema design.

The model contains:

### Dimension Tables

- Students
- Date/Calendar (where required)

### Fact Tables

- Attendance
- Scores
- Behavior

Relationships were created using Student ID to allow filtering and interaction between all report pages.

---

# DAX Measures Created

Several DAX calculations were created to support the dashboard.

## Total Students

```DAX
Total Students =
DISTINCTCOUNT(Student[StudentID])
```
