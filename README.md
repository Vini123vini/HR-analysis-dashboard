# HR-analysis-dashboard
Interactive powerBI Dashboard for Human Resources Analysis
# 💼 HR Analysis Dashboard - Power BI

## 📊 Project Overview
The *HR Analysis Dashboard* is an interactive Power BI project designed to visualize and analyze key *Human Resource metrics* such as employee attrition, department performance, gender diversity, and salary trends.  

This dashboard helps HR departments make *data-driven decisions* by transforming raw HR data into actionable insights through *Power BI visuals* and *DAX formulas*.

---

## 🎯 Objectives
- To monitor and analyze employee data efficiently.
- To identify workforce trends and patterns.
- To support HR decision-making using key performance indicators (KPIs).
- To demonstrate Power BI and DAX capabilities for business insights.

---

## ⚙️ Tools & Technologies
- *Power BI Desktop*
- *DAX (Data Analysis Expressions)*
- *Excel / CSV dataset*
- *Data Modeling (Relationships, Measures, Calculated Columns)*

---

## 📈 Key Insights & Metrics
The dashboard highlights:
- 👥 *Total Employees*
- 📉 *Attrition Rate*
- 💰 *Average Salary*
- 🏢 *Department-wise Employee Count*
- 👨‍💼 *Gender Diversity*
- ⏳ *Age and Experience Distribution*

---

## 🧮 DAX Measures Used
Some key *DAX formulas* applied in this project:

```DAX
Total Employees = COUNTROWS('HR Data')

Attrition Count = CALCULATE(COUNTROWS('HR Data'), 'HR Data'[Attrition] = "Yes")

Attrition Rate = DIVIDE([Attrition Count], [Total Employees]) * 100

Average Salary = AVERAGE('HR Data'[MonthlyIncome])

Avg Age = AVERAGE('HR Data'[Age])

Years of Service = DATEDIFF('HR Data'[HireDate], TODAY(), YEAR)

Visuals Used

KPI Cards (Total Employees, Attrition Rate, Average Salary)

Clustered Bar Chart (Department-wise Attrition)

Pie / Donut Chart (Gender Diversity)

Line Chart (Attrition Trend by Age)

Table (Detailed Employee Information)

Slicers (Department, Gender, Education, Job Role)



🧠 Insights Derived

Most attrition occurs among employees with lower job satisfaction and shorter tenure.

Certain departments show higher salary variations.

The gender ratio reveals potential diversity imbalance.

Experienced employees tend to have higher retention rates.
