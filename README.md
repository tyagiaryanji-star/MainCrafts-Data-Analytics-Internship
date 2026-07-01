
# My Data Analytics Journey 📊

Welcome to my Data Analytics portfolio project! This project was completed as part of my **Data Analytics & Business Intelligence Internship at MainCrafts**. 

The primary objective of this task was to take raw, messy data, clean it thoroughly, perform Exploratory Data Analysis (EDA), and build a high-impact dashboard to derive meaningful business insights.

---

## 🖼️ Project Dashboard & Overview

> [!TIP]
> *Yahan par apni image drag and drop kar dena (Niche diye gaye note ko padhein)*

---

## 🛠️ Tools & Skills Used

* **Tools:** Microsoft Excel | SQL | Microsoft Power BI
* **Key Skills:**
    * Data Cleaning & Preparation
    * Exploratory Data Analysis (EDA)
    * Pivot Table Analysis
    * SQL Aggregations
    * Data Visualization
    * Business Insights & Reporting

---

## 🧹 Data Cleaning Steps Followed

Before jumping into analysis, the data was refined using the following pipeline:
1.  **Removed Duplicate Records** to ensure data integrity.
2.  **Handled Missing Values** appropriately without biasing the metrics.
3.  **Standardized Date Formats** for seamless time-series analysis.
4.  **Corrected Data Types** (e.g., converting text numbers to integers).
5.  **Removed Unnecessary Columns** to optimize dashboard performance.
6.  **Cleaned Inconsistent Text Entries** (fixing typos, casing issues).

---

## 📈 Key Business Metrics (KPIs)

* **Total Sales:** $2.30M
* **Total Profit:** $286.40K
* **Total Orders:** 9,994
* **Total Customers:** 793
* **Average Discount:** 15.62%

---

## 🗄️ Sample SQL Queries Used

Here are some of the core SQL queries implemented to aggregate data before visualization:

```sql
-- 1. Calculate Total Sales
SELECT SUM(Sales) AS Total_Sales 
FROM sales;

-- 2. Sales by Category
SELECT Category, SUM(Sales) AS Total_Sales 
FROM sales
GROUP BY Category
ORDER BY Total_Sales DESC;

-- 3. Monthly Sales Trend
SELECT DATE_TRUNC('month', Order_Date) AS Month,
       SUM(Sales) AS Total_Sales
FROM sales
GROUP BY Month
ORDER BY Month;
