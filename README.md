# ☕ Aromia Coffee Sales Analysis Dashboard (Power BI)

## Project Overview

This project presents an interactive Power BI dashboard built for **Aromia Coffee Shop** in the UK, analyzing sales performance from **January to March 2025**.

The dashboard transforms raw transactional data into business insights, allowing stakeholders to monitor revenue, sales performance, customer purchasing behavior, store performance, and product trends through interactive visualizations.

---

# Dashboard Preview

## General Overview

<img width="1426" height="800" alt="General Overview" src="https://github.com/user-attachments/assets/ce621696-fc9d-4706-8f1e-32e8df144963" />

## Products & Store Performance

<img width="1423" height="798" alt="Product and Location" src="https://github.com/user-attachments/assets/10cc5dc5-2682-4098-8f3d-b7dd61c4bd2a" />

## Interactive Dashboard

[aromia_revenue_dashboard.html](https://code-with-shahin.github.io/Aromia_Coffee_Sales_Analysis/Dashboard/aromia_revenue_dashboard.html)

---

# Business Objectives

The dashboard answers questions such as:

- Which cities generate the highest revenue?
- Which stores perform best?
- Which products contribute the most revenue?
- What time of day generates the highest sales?
- How does revenue change over time?
- Which product categories drive the business?
- Where are the highest-performing stores located?

---

# Key KPIs

The dashboard includes:

- **Total Revenue**
- **Total Orders**
- **Average Order Value**
- **Total Items Sold**

---

# Dashboard Pages

## 1. Executive Overview

Features:

- KPI Cards
- Revenue by City
- Monthly Revenue Trend
- Revenue Split by Category
- City Filter
- Month Filter

Insights:

- London generated the highest revenue (£2,107).
- Revenue increased consistently between January and March.
- Coffee products account for more than half of total sales.
- March recorded the highest monthly revenue.

---

## 2. Product & Store Analysis

Features:

- Top 5 Best-Selling Products
- Top 5 Stores by Revenue
- Revenue by Time of Day
- Revenue by City (Bubble Map)
- Product Category Filter
- City Filter

Insights:

- Mocha generated the highest revenue.
- Aromia Manchester is the highest-performing store.
- Morning (08:00–10:00) is the busiest sales period.
- Revenue is concentrated in major UK cities.

---

# Data Model

The dashboard uses a relational model consisting of multiple tables.

Tables used:

- Orders
- Order Items
- Calendar
- Products
- Stores

Relationships were created using primary and foreign keys to support efficient DAX calculations and interactive reporting.

---

# Power BI Features Used

- Power Query
- Data Cleaning
- Data Modeling
- Star Schema
- DAX Measures
- Interactive Slicers
- KPI Cards
- Maps
- Line Charts
- Bar Charts
- Donut Charts
- Drill-through Filtering
- Cross-filtering

---

# Main DAX Measures

Examples include:

```DAX
Total Revenue =
SUMX(
    order_items,
    order_items[quantity] * order_items[unit_price]
)

Total Orders =
DISTINCTCOUNT(orders[order_id])

Average Order Value =
DIVIDE([Total Revenue], [Total Orders])

Total Items Sold =
SUM(order_items[quantity])
```

---

# Business Insights

### Revenue

- Total Revenue: **£7,069**
- Total Orders: **1,200**
- Average Order Value: **£5.89**
- Total Items Sold: **2,131**

### Cities

Highest revenue:

1. London
2. Manchester
3. Birmingham

### Categories

Revenue distribution:

- Coffee (51.5%)
- Bakery (20.3%)
- Cold Drinks (20.0%)
- Tea (8.3%)

### Products

Top performers:

- Mocha
- Latte
- Cortado
- Americano
- Macchiato

### Peak Hours

The busiest period is:

**Morning (08:00–10:00)**

followed by

- Afternoon
- Lunch
- Evening

---

# Skills Demonstrated

- Power BI
- Data Visualization
- Dashboard Design
- Power Query
- DAX
- Data Modeling
- Business Intelligence
- KPI Reporting
- Interactive Reporting

---

# Tools Used

- Microsoft Power BI Desktop
- Power Query
- DAX
- Microsoft Excel / CSV

---

# Repository Contents

```
Dashboard/
    Aromia_Coffee_Dashboard.pbix

Data/
    CSV datasets

Images/
    Dashboard screenshots

README.md
```

---

# Future Improvements

Potential enhancements include:

- Customer segmentation
- Profit analysis
- Forecasting future revenue
- Customer lifetime value (CLV)
- Inventory monitoring
- Dynamic tooltips
- Drill-through report pages

---

## Author

**Shahin Amirov**

- Power BI
- Data Analytics
- Business Intelligence
