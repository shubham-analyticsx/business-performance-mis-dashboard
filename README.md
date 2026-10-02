# Business Performance MIS & Automated Dashboard

An end-to-end **Business Performance MIS and Management Dashboard** built using **Excel 2021, Power Query, PivotTables, PivotCharts, Slicers, Timeline and VBA automation**.

The project demonstrates how raw transactional sales data can be transformed into a structured, validated and interactive reporting system for management decision-making.

---

## 📌 Project Overview

This portfolio project simulates a retail business reporting environment where management needs to monitor:
- Sales performance
- Profitability
- Regional performance
- Product performance
- Salesperson performance
- Target achievement
- Order status
- Data quality
- Daily sales trends

The solution follows an end-to-end reporting workflow:

**Raw Data → Power Query ETL → Data Quality → Business Calculations → Analysis → PivotTables → Interactive Dashboard → VBA Automation**

---

## 🎯 Business Objectives

The MIS was designed to answer practical business questions such as:

1. What are the total completed sales and profit?
2. Which regions are achieving their sales targets?
3. Which products generate the highest sales?
4. Which salespersons contribute the most sales and profit?
5. What is the overall profit margin?
6. How many orders are cancelled?
7. What is the cancellation rate?
8. How does sales performance change over time?
9. Are there any data-quality problems?
10. Can management refresh the entire reporting system with one click?

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| Excel 2021 | Data analysis and dashboard development |
| Excel Tables | Structured source and target data |
| Power Query | Data cleaning and ETL |
| Advanced Excel Formulas | Business calculations and dynamic analysis |
| PivotTables | Multidimensional analysis |
| PivotCharts | Visual reporting |
| Slicers | Interactive filtering |
| Timeline | Date-based filtering |
| VBA | One-click report refresh automation |

---

## 🔄 Data Preparation & ETL

Power Query was used to create a repeatable data-cleaning and transformation pipeline.

### Transformation steps

- Imported the raw sales table into Power Query
- Added source-row order for traceability
- Trimmed and cleaned text fields
- Corrected data types
- Converted dates using the appropriate regional locale
- Created calculated Profit
- Created Completed Sales
- Created Completed Profit
- Created Completed Quantity
- Added automated data-quality validation
- Loaded the transformed dataset back into Excel

### Data Quality Rules

The transformation layer checks for:

- Missing Order IDs
- Invalid quantities
- Negative sales values
- Negative cost values
- Sales below cost requiring review

The final dataset contained **0 data-quality issues**.

---

## 📊 Key KPIs

The dashboard provides management-level KPIs including:

| KPI | Result |
|---|---:|
| Total Records | 30 |
| Completed Orders | 29 |
| Cancelled Orders | 1 |
| Completed Sales | ₹15,60,000 |
| Completed Profit | ₹4,38,800 |
| Profit Margin | 28.13% |
| Cancellation Rate | 3.33% |
| Completed Quantity | 156 |
| Overall Target | ₹11,80,000 |
| Overall Target Achievement | 132.20% |
| Data Quality Issues | 0 |

---

## 🌎 Regional Performance

Completed sales were compared against regional monthly targets.

| Region | Completed Sales | Target | Achievement |
|---|---:|---:|---:|
| North | ₹4,53,000 | ₹3,50,000 | 129.43% |
| South | ₹4,45,000 | ₹3,00,000 | 148.33% |
| East | ₹3,98,000 | ₹2,50,000 | 159.20% |
| West | ₹2,64,000 | ₹2,80,000 | 94.29% |

This analysis allows management to identify regions performing above target as well as regions requiring additional attention.

---

## 📦 Product Performance

Completed sales analysis by product:

| Product | Sales | Profit | Quantity |
|---|---:|---:|---:|
| Laptop | ₹4,20,000 | ₹1,05,000 | 7 |
| Mobile | ₹4,40,000 | ₹1,10,000 | 22 |
| Office Chair | ₹1,68,000 | ₹56,000 | 14 |
| Desk | ₹1,80,000 | ₹60,000 | 12 |
| Monitor | ₹2,20,000 | ₹55,000 | 11 |
| Keyboard | ₹57,500 | ₹23,000 | 18 |
| Mouse | ₹62,000 | ₹24,800 | 62 |

Cancelled transactions are excluded from completed-sales performance analysis.

---

## 👥 Salesperson Analysis

The reporting model also evaluates sales and profit contribution by salesperson.

| Salesperson | Completed Sales | Completed Profit | Orders |
|---|---:|---:|---:|
| Amit | ₹4,53,000 | ₹1,24,800 | 8 |
| Priya | ₹4,45,000 | ₹1,28,000 | 8 |
| Rahul | ₹3,98,000 | ₹1,12,000 | 8 |
| Neha | ₹2,64,000 | ₹74,000 | 5 |

---

## 📈 Interactive Dashboard

The dashboard includes:

- KPI cards
- Completed Sales
- Completed Profit
- Orders
- Profit Margin
- Cancellation Rate
- Regional performance
- Product performance
- Salesperson performance
- Daily completed-sales trend
- Order-status distribution
- Actual Sales vs Target
- Data-quality summary
- Reporting-period indicator

### Interactive Controls

Users can dynamically filter the report using:

- Region
- Salesperson
- Product
- Category
- Order Status
- Timeline / Date

The PivotTables, PivotCharts and KPI reporting are connected to the interactive filtering layer.

---

## 🎯 Actual Sales vs Target

A dedicated analysis compares completed sales against the monthly target for each region.

The report automatically calculates:

**Achievement % = Completed Sales ÷ Target**

and identifies whether the region has achieved its target.

This provides a simple management view of target performance.

---

## ⚙️ VBA Automation

A VBA refresh macro was developed to simplify the reporting workflow.

The refresh process:

1. Refreshes the Power Query output
2. Refreshes PivotTables
3. Recalculates workbook formulas
4. Updates the dashboard
5. Records the latest refresh timestamp
6. Displays a refresh-success message

This converts a multi-step manual reporting process into a **one-click MIS refresh workflow**.

---

## 🗂️ Project Structure

```text
business-performance-mis-dashboard/
│
├── documentation/
│
├── sample-data/
│   └── Apex_Retail_MIS_Dashboard.xlsm
│
├── screenshots/
│
└── README.md
