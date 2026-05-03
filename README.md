# 📊 Ultimate One-Click Financial Dashboard (Excel + Power Query + Power Pivot)

![Domain](https://img.shields.io/badge/Domain-Financial%20Modeling%20%7C%20FP%26A-blue)
![Tool](https://img.shields.io/badge/Tool-Excel%20%7C%20Power%20Query%20%7C%20Power%20Pivot-217346?logo=microsoft-excel&logoColor=white)
![Model](https://img.shields.io/badge/Architecture-Data%20Model%20%7C%20DAX-orange)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

A fully dynamic **one-click financial performance dashboard** built entirely in Excel using **Power Query, Power Pivot, DAX measures, and a structured data model**.

This project replicates a real-world FP&A reporting system capable of switching between:

- Budget
- Prior Period
- Prior Year
- YTD
- Trailing 3 / 6 / 12 Months

All with a single slicer selection.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Dashboard Architecture](#dashboard-architecture)
- [Data Engineering (Power Query)](#data-engineering-power-query)
- [Data Model & Relationships (Power Pivot)](#data-model--relationships-power-pivot)
- [Dynamic Period Engine (DAX Measures)](#dynamic-period-engine-dax-measures)
- [Financial Dashboard Outputs](#financial-dashboard-outputs)
- [Key Insights & Capabilities](#key-insights--capabilities)
- [Skills Demonstrated](#skills-demonstrated)

---

## 📋 Project Overview

This project transforms raw departmental P&L exports into a **fully scalable financial reporting system**.

The dashboard supports:

| Analysis Type | Description |
|---------------|-------------|
| Budget vs Actual | Variance analysis with hit/miss visualization |
| Prior Period | Month-over-month comparison |
| Prior Year | YoY comparison |
| Rolling Views | Trailing 3M / 6M / 12M |
| YTD | Year-to-date aggregation |

All calculations are dynamically driven by DAX measures — no manual updates required.

---

# 🏗 Dashboard Architecture

![Financial Dashboard](images/financial_dashboard.png)

The dashboard consists of three major reporting layers:

### 1️⃣ Enterprise Financial Summary
- Revenue & Gross Margin trend
- Opex by Department
- Opex by Cost Type
- Period slicer (2023 / 2024 / YTD / Rolling views)

### 2️⃣ Variance Analysis Framework
- Budget vs Actual
- Prior Period vs Actual
- Prior Year vs Actual
- KPI hit/miss donut visualizations

### 3️⃣ Department & Cost Drilldowns
- Budget / Actual / Variance by Department
- Budget / Actual / Variance by Cost Type
- Fully dynamic pivot-backed tables

---

# 🔄 Data Engineering (Power Query)

Raw departmental P&L files were:

- Converted to named ranges
- Unpivoted into columnar format
- Standardized across departments
- Appended into consolidated Actual & Budget tables

### ETL Steps:
- Unpivot monthly columns into Date column
- Standardize account naming
- Append multiple departments
- Create centralized departmental P&L dataset

Result: Clean tabular data optimized for Power Pivot modeling.

---

# 🧠 Data Model & Relationships (Power Pivot)

A full data model was created including:

### Fact Tables
- Departmental Profit & Loss (Actual)
- Departmental Profit & Loss (Budget)

### Lookup Tables
- Calendar Table (auto-generated date table)
- Account Mapping Table (Section + Summary Grouping)
- Department Table
- Period Selection Table
- Predefined Date Logic Table

Relationships were built between:
- Fact tables ↔ Calendar
- Fact tables ↔ Account Mapping
- Fact tables ↔ Department

This allowed full filtering scalability across:

- Date
- Department
- Summary grouping
- Period selection

---

# ⚙️ Dynamic Period Engine (DAX Measures)

The core innovation of this dashboard is the **dynamic period engine**.

A slicer selection controls all dashboard outputs using:

- SWITCH()
- SUMX()
- FILTER()
- LOOKUPVALUE()
- Date boundary logic

Supported dynamic periods:

- 2023
- 2024
- 2025
- Current Month
- YTD
- Trailing 3 Months
- Trailing 6 Months
- Trailing 12 Months

Changing one slicer updates:

- All pivot tables
- All variance calculations
- All donut charts
- All KPIs
- All summary sections

No manual recalculation required.

---

# 📈 Financial Dashboard Outputs

### 🔹 Revenue & Gross Margin Trend
- Clustered column + smooth line combo
- Dynamic period switching
- Margin visual overlay

### 🔹 Opex by Department
- Stacked column visualization
- Pie chart breakdown
- Real-time filtering

### 🔹 Budget vs Actual Framework
- Dollar variance
- Percentage variance
- Dynamic hit/miss donut charts
- Favorable (green) vs unfavorable (red) visualization

### 🔹 Prior Period & Prior Year Comparisons
- Fully automated rolling comparison logic
- KPI variance engine
- Custom conditional formatting logic

---

# 💡 Key Insights & Capabilities

1. **Single-click reporting engine** — All reporting views update instantly.
2. **Fully scalable model** — Add departments without redesigning dashboard.
3. **Dynamic time intelligence** — Rolling, YTD, and annual views supported.
4. **True FP&A structure** — Mirrors institutional reporting workflows.
5. **Separation of ETL, model, and visualization layers**.
6. **No hard-coded formulas in dashboard layer** — All logic centralized in DAX.

---

# 🧠 Skills Demonstrated

- Advanced Excel Financial Modeling
- Power Query (ETL Design)
- Power Pivot Data Modeling
- DAX Measure Engineering
- Time Intelligence Calculations
- Variance Analysis Framework Design
- Financial KPI Architecture
- Dashboard UX Design
- Enterprise FP&A Reporting Logic

---

## 🚀 Business Impact

This project demonstrates the ability to:

- Design institutional-grade financial reporting tools
- Automate monthly reporting workflows
- Replace static P&L exports with interactive dashboards
- Build scalable financial intelligence systems
- Apply BI engineering concepts inside Excel

---

This project reflects advanced proficiency in Excel-based business intelligence and financial analytics modeling.
