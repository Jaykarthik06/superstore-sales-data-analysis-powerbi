# Superstore Sales Data Analysis & Forecasting Dashboard

## 📌 Project Overview

This project focuses on analyzing Superstore sales data using **Power BI** to generate meaningful business insights, track key performance indicators (KPIs), and forecast future sales trends. The dashboard provides an interactive and user-friendly interface that enables stakeholders to make data-driven decisions.

The project incorporates **data cleaning**, **data transformation**, **DAX calculations**, **data visualization**, and **time series forecasting** to evaluate sales performance and predict future sales for the next 15 days.

---

## 🎯 Objective

The primary objective of this project is to contribute to business success by utilizing data analysis techniques and time series forecasting to provide valuable insights and support strategic decision-making.

### Key Goals

* Create an interactive and visually appealing Power BI dashboard.
* Identify and monitor important business KPIs.
* Analyze sales performance across different dimensions.
* Generate accurate sales forecasts using historical sales data.
* Provide actionable insights and recommendations for business growth.

---

## 🛠 Tools & Technologies Used

* **Power BI**
* **Power Query**
* **DAX (Data Analysis Expressions)**
* **Time Series Analysis**
* **Data Visualization**
* **Data Cleaning & Transformation**

---

## 📂 Data Preparation

The following data preprocessing steps were performed before analysis:

1. Verified and corrected data types for all columns.
2. Identified and handled missing/null values.
3. Replaced null values where necessary.
4. Removed unnecessary columns (`ind1`, `ind2`).
5. Created calculated columns and measures using DAX.

### DAX Calculations

#### Average Delivery Time

```DAX
AvgDelivery =
DATEDIFF(
    'SuperStore_Sales'[Order Date],
    'SuperStore_Sales'[Ship Date],
    DAY
)
```

#### Sales Forecast Dataset

```DAX
Salesforecast =
SUMMARIZE(
    'SuperStore_Sales',
    'SuperStore_Sales'[Order Date],
    "Total Sales",
    SUM(SuperStore_Sales[Sales])
)
```

---

## 📊 Dashboard Features
### KPI Monitoring

* Total Sales
* Total Profit
* Total Orders
* Average Delivery Time

### Interactive Visualizations

* Sales Trends Analysis
* Profit Analysis
* Regional Performance Analysis
* Category & Sub-Category Analysis
* Customer Segment Analysis

### Filtering Capabilities

* Region
* Category
* Sub-Category
* Time Period

---

## 📈 Sales Forecasting

A time series forecasting model was implemented using historical sales data to predict sales performance for the next **15 days**.

### Benefits

* Demand Planning
* Inventory Optimization
* Strategic Decision Making
* Performance Monitoring

---

## 🔍 Key Insights

The dashboard helps businesses:

* Identify top-performing products and categories.
* Understand regional sales performance.
* Monitor profit trends and business growth.
* Analyze customer purchasing patterns.
* Make informed decisions based on forecasted sales trends.

---

## 📚 Learning Outcomes

Through this project, the following skills were strengthened:

* Data Cleaning and Transformation
* Business Intelligence Reporting
* Power BI Dashboard Development
* DAX Calculations
* Time Series Analysis
* Data Visualization Best Practices
* Business Insight Generation

---

## 🚀 Future Improvements

* Integrate advanced forecasting models.
* Add customer churn analysis.
* Implement real-time data connectivity.
* Develop automated business alert systems.
* Include advanced profitability and inventory analytics.

---

## 📷 Dashboard Preview

<img width="401" height="223" alt="Screenshot 2026-07-03 175355" src="https://github.com/user-attachments/assets/d3c71c3b-a9e8-4624-bdad-655577299b2e" />


---

## 👨‍💻 Author

**Jayanth L K**

Aspiring Data Analyst passionate about transforming raw data into actionable business insights through analytics, visualization, and forecasting.

---

## ⭐ If you found this project useful, consider giving it a star!

