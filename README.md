# HR Analytics Dashboard – Power BI

## Project Overview
This project focuses on analyzing employee attrition and workforce trends using Microsoft Power BI.

The dashboard helps HR teams understand employee turnover, identify departments with higher attrition, and analyze workforce demographics.

## Tools & Technologies
- Microsoft Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Microsoft Excel / CSV
- GitHub

## Business Objectives
- Calculate total employees and active employees.
- Calculate employee attrition count and attrition rate.
- Analyze attrition by department.
- Analyze employee attrition by gender and age group.
- Compare average monthly salary by department.
- Analyze employee hiring trends.
- Identify departments with higher attrition rates.

## Key Performance Indicators (KPIs)
1. Total Employees
2. Active Employees
3. Attrition Count
4. Attrition Rate
5. Average Monthly Salary

## Dashboard Features
- Department-wise attrition analysis
- Gender-wise attrition analysis
- Age-group attrition analysis
- Department-wise average salary comparison
- Employee hiring trends
- Interactive department and hire-date filters

## DAX Measures

**Total Employees**
```dax
Total Employees =
DISTINCTCOUNT('HR Data'[EmployeeNumber])
```

**Attrition Count**
```dax
Attrition Count =
CALCULATE(
    [Total Employees],
    'HR Data'[Attrition] = "Yes"
)
```

**Attrition Rate**
```dax
Attrition Rate =
DIVIDE(
    [Attrition Count],
    [Total Employees],
    0
)
```

**Average Salary**
```dax
Average Salary =
AVERAGE('HR Data'[MonthlyIncome])
```

## Project Files
- Dashboard: Power BI PBIX file
- Dataset: HR employee dataset
- Dashboard Screenshot: PNG image
- Dashboard Report: PDF
- DAX Measures: Calculation documentation

## Business Insights
The dashboard helps identify departments with higher employee attrition rates and provides insights into workforce demographics and salary distribution.

## Dataset Disclaimer
This project uses a practice dataset. Any simulated hire dates are for demonstration purposes and do not represent actual historical hiring records.

## Author
Data Analytics Portfolio Project

Skills: Power BI | DAX | Power Query | Data Visualization | Data Analysis

## Dashboard Preview

<img width="925" height="1065" alt="HR_Analytics_Dashboard" src="https://github.com/user-attachments/assets/c6e2258e-42c1-47b6-b244-86c26d1de01f" />

