# PowerBI-Finance-DashBoard
Interactive Finance Data Analysis Dashboard developed using Power BI, Power Query and DAX.

## 📌 Project Overview

This project presents an **interactive Finance Data Analysis Dashboard** developed using **Microsoft Power BI**.

The dashboard analyzes financial performance across **sales, profit, products, countries, segments, and discount bands**. It is designed to provide a clear view of business performance and support data-driven decision-making.

---

## 🎯 Project Objectives

* Analyze overall financial performance
* Monitor Sales and Profit
* Understand Profit Margin
* Analyze product-wise performance
* Analyze country-wise performance
* Compare different business segments
* Analyze the impact of discount bands
* Create interactive and user-friendly dashboards
* Practice Power Query, DAX, data modeling, and visualization

---

## 📂 Dataset

The Finance dataset contains the following major fields:

* Segment
* Country
* Product
* Discount Band
* Units Sold
* Manufacturing Price
* Sale Price
* Gross Sales
* Discounts
* Sales
* COGS
* Profit

---

# 📑 Dashboard Pages

## 1️⃣ Finance Overview

The **Finance Overview** page provides a high-level summary of financial performance.

### Key Performance Indicators

* Total Revenue
* EBIT(Profit)
* Total Records
* EBIT Margin %
* Gross Sales
* Units Sold
* Operation Working Capital

### Visualizations

* Sales by Year
* Sales & Profit By Year
* Profit By Country
* Sales By Product
* Sales By Segment

### Interactive Filters

* Year
* Country
* Segment
* Product
* Discount Band
* Month Name

---

## 2️⃣ Sales & Profit Analysis

This page focuses on detailed analysis of **Sales and Profit performance**.

---

## 3️⃣ Product & Country Analysis

This page provides detailed analysis of **product and country performance**.

---

# 🛠️ Tools & Technologies

### Microsoft Power BI

* Power BI Desktop
* Power Query
* DAX
* Data Modeling
* Data Visualization

### Microsoft Excel

* Data preparation
* Source dataset

---

# 📐 DAX Measures

### Total Revenue

```DAX
Total Revenue =
SUM(Finance[Sales])
```

### Total Profit

```DAX
EBIT =
SUM(Finance[Profit])
```

### Total COGS

```DAX
Total COGS =
SUM(Finance[COGS])
```

### Total Units Sold

```DAX
Total Units Sold =
SUM(Finance[Units Sold])
```

### EBIT Margin

```DAX
EBIT Margin % =
DIVIDE(
    [EBIT],
    [Total Revenue],
    0
)
```

```DAX
Selected Country = 
SELECTEDVALUE(Finance[Country], "All Countries")
)
```

### Operating Working Capital
Operating Working Capital = 
VAR _AR = [Accounts Receivable]
VAR _InvDays = 45
VAR _PayableDays = 30

VAR _Inventory = DIVIDE([Total COGS], 365, 0) * _InvDays
VAR _AP = DIVIDE([Total COGS], 365, 0) * _PayableDays

RETURN
(_AR + _Inventory) - _AP

# 🔄 Power BI Features Used

* ✅ Power Query
* ✅ Data Cleaning
* ✅ Data Transformation
* ✅ Data Modeling
* ✅ DAX Measures
* ✅ KPI Cards
* ✅ Slicers
* ✅ Charts
* ✅ Matrix
* ✅ Page Navigation
* ✅ Drill-through
* ✅ Report Tooltips
* ✅ Interactive Filtering

---

# 🧭 Dashboard Navigation

The dashboard contains three main pages:

```text
Finance Overview
       ↓
Sales & Profit Analysis
       ↓
Product & Country Analysis
       ↓
Website



```

Page navigation buttons allow users to move between dashboard pages easily.

---

# 🔎 Drill-through Analysis

Drill-through functionality is used to provide detailed information for selected:

* Countries
* Products

Users can right-click a data point and navigate to the corresponding detail page.

---

# 💡 Key Business Analysis

The dashboard can be used to identify:

* Overall sales performance
* Profitability trends
* Product-level performance
* Country-level performance
* Segment contribution
* Discount-related sales patterns
* Differences between Sales, COGS, and Profit

> **Note:** Specific business insights should be added based on the actual results displayed in the completed Power BI dashboard.

---

# 📸 Dashboard Preview

### Finance Overview

Add your screenshot here:

```markdown
<img width="1319" height="740" alt="Finance_Overview" src="https://github.com/user-attachments/assets/8053e638-483f-42a4-b2f1-2fba806eabb2" />
```

### Sales & Profit Analysis

```markdown
<img width="1329" height="749" alt="Sales Profit_Analysis" src="https://github.com/user-attachments/assets/06530899-ed67-4b29-89f8-e811c246db6a" />
```

### Product & Country Analysis

```markdown
<img width="1319" height="727" alt="Product Country_Analysis" src="https://github.com/user-attachments/assets/a8f2cd11-f078-4702-9c9b-7cf799a8c142" />
```
### Finance Metrics

```markdown
<img width="1319" height="727" alt="Product Country_Analysis" src="https://github.com/user-attachments/assets/a8f2cd11-f078-4702-9c9b-7cf799a8c142" />
```
---


---

# 🚀 Learning Outcomes

Through this project, I practiced:

* Data cleaning and transformation
* Power Query
* Data modeling
* DAX calculations
* KPI development
* Financial analysis
* Interactive dashboard design
* Drill-through analysis
* Report tooltips
* Business data visualization
* Power BI storytelling

---

## Skills Demonstrated

`Power BI` · `Power Query` · `DAX` · `Excel` · `Data Analysis` · `Data Visualization` · `Business Intelligence`

---




