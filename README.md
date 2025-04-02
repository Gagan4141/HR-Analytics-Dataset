# HR Analytics Dataset

This repository contains an HR dataset (`HR_DATA_Excel.xlsx`) that provides detailed information about employees in a company. The dataset is useful for analyzing workforce trends, predicting attrition, and understanding factors influencing employee satisfaction and performance.

## Table of Contents
1. [Dataset Overview](#dataset-overview)
2. [File Structure](#file-structure)
3. [Key Features](#key-features)
4. [Insights and Observations](#insights-and-observations)
5. [How to Use](#how-to-use)
6. [Licensing](#licensing)
7. [Contributions](#contributions)

---

## Dataset Overview
The dataset contains **1,470 records** of employees, with **14 attributes** per record. It covers demographic details, job-related information, and performance metrics. This data can be used for exploratory analysis, predictive modeling, and deriving actionable insights for HR management.

---

## File Structure
- **HR_DATA_Excel.xlsx**: The main dataset file.
  - Sheet: `HR_Data`
    - Columns: `Employee_ID`, `Age`, `Gender`, `Education_Level`, `Job_Title`, `Department`, `Years_of_Service`, `Performance_Rating`, `Salary`, `Work_Life_Balance`, `Attrition`, `Marital_Status`, `Overtime`, `Distance_From_Home`.

---

## Key Features
- **Demographics**: Includes age, gender, and marital status.
- **Education and Job Details**: Captures education level, job title, department, and years of service.
- **Performance Metrics**: Tracks performance ratings, salary, and work-life balance.
- **Attrition**: Indicates whether an employee has left the company.
- **Work Conditions**: Includes overtime and distance from home.

---

## Insights and Observations
- **Attrition Analysis**: Approximately 16% of employees have left the company. Factors like commute distance and work-life balance appear to influence attrition.
- **Performance and Salary**: Higher performance ratings correlate with higher salaries.
- **Overtime Patterns**: Certain departments (e.g., Sales, Research & Development) report higher overtime rates.
- **Work-Life Balance**: Scores vary significantly across departments, impacting overall satisfaction.

---

## How to Use
1. Download the dataset (`HR_DATA_Excel.xlsx`) from this repository.
2. Load the data into your preferred tool (e.g., Python, R, Excel) for analysis.
3. Explore relationships between variables using visualizations and statistical methods.
4. Build predictive models to forecast attrition or identify key drivers of employee satisfaction.

Example (Python):
```python
import pandas as pd

# Load the dataset
df = pd.read_excel("HR_DATA_Excel.xlsx", sheet_name="HR_Data")

# Display basic information
print(df.info())
print(df.describe())

# Analyze attrition
attrition_rate = df['Attrition'].value_counts(normalize=True)
print(attrition_rate)
