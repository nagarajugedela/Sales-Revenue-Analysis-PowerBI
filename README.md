# 📊 Sales & Revenue Analysis Dashboard

## 📌 Project Overview

The **Sales & Revenue Analysis Dashboard** is an interactive data visualization project developed using Microsoft Power BI. It analyzes sales performance, revenue distribution, regional sales, product performance, and monthly revenue trends.

The dashboard helps users understand business performance through interactive charts, KPI cards, and slicers.

## 🎯 Project Objectives

- Analyze overall sales and revenue performance.
- Track monthly revenue trends.
- Compare sales performance across regions.
- Understand revenue contribution by product category.
- Identify the top-performing products.
- Provide interactive filtering for better analysis.

## 🛠️ Tools & Technologies

- Microsoft Power BI Desktop
- Power BI Service
- Power Query
- DAX (Data Analysis Expressions)
- CSV Dataset

## 📂 Dataset Information

**Dataset:** `sales_data.csv`

The dataset contains the following columns:

| Column | Description |
|---|---|
| Order ID | Unique order identifier |
| Order Date | Date of the order |
| Region | Sales region |
| Category | Product category |
| Product | Product name |
| Quantity | Number of units sold |
| Unit Price | Price per unit |
| Revenue | Total revenue generated |

## 📈 Dashboard Features

### 1. Key Performance Indicators (KPIs)
- Total Revenue
- Total Orders
- Total Quantity Sold
- Average Order Value
- Average Selling Price

### 2. Monthly Revenue Trend
Visualizes revenue performance over time.

### 3. Sales by Region
Compares revenue generated across different regions.

### 4. Revenue by Category
Shows the percentage contribution of each product category.

### 5. Top 5 Products by Revenue
Identifies the five products generating the highest revenue.

### 6. Interactive Slicers
- Region
- Category
- Order Date

## 📊 DAX Measures

**Total Revenue**
```dax
Total Revenue = SUM(sales_data[Revenue])
```

**Total Orders**
```dax
Total Orders = DISTINCTCOUNT(sales_data[Order ID])
```

**Total Quantity**
```dax
Total Quantity = SUM(sales_data[Quantity])
```

**Average Order Value**
```dax
Average Order Value = DIVIDE([Total Revenue], [Total Orders], 0)
```

**Average Selling Price**
```dax
Average Selling Price = DIVIDE([Total Revenue], [Total Quantity], 0)
```

## 🔍 Key Results

| KPI | Result |
|---|---:|
| Total Revenue | 31,090 |
| Total Orders | 40 |
| Total Quantity | 238 |
| Average Order Value | 777.25 |
| Average Selling Price | 130.63 |

*Note: Currency is not specified in the source dataset.*

## 📅 Reporting Period

January 2025 – September 2025

## 🚀 Project Workflow

1. Imported the CSV dataset into Power BI.
2. Performed data inspection and type conversion using Power Query.
3. Created DAX measures for key business metrics.
4. Designed interactive KPI cards and charts.
5. Added slicers for dynamic filtering.
6. Published the report to Power BI Service.

## 📁 Project Files

- `Sales_Revenue_Analysis.pbix` – Power BI dashboard file.
- `sales_data.csv` – Source dataset.
- `README.md` – Project documentation.
- `screenshots/` – Dashboard screenshots.

## 👨‍💻 Author

**Naga Raju Gedela**

Data Analytics | SQL | Excel | Power BI | Python

## ⭐ Acknowledgement

This project was developed as a practical learning project to improve skills in data analysis, data visualization, Power Query, and Power BI dashboard development.
