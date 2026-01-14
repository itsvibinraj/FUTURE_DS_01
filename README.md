# FUTURE_DS_01
# 📊 Superstore Sales Performance Dashboard

![Power BI](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

## 📖 Project Overview
This project is part of a data analytics internship task to analyze real-world e-commerce sales data. The goal was to build an interactive **Power BI Dashboard** that helps business stakeholders understand sales trends, product performance, and regional distribution.

The dashboard answers critical business questions such as:
* What are the best-selling products?
* When do sales peak during the year?
* Which regions contribute the most to revenue?

## 📂 Data Source
* **Dataset:** Superstore Sales Dataset
* **Source:** Kaggle / Internship Provider
* **Format:** Excel (.xls) / CSV
* **Key Columns:** Order Date, Sales, Profit, Region, Category, Sub-Category.

## 🛠️ Tech Stack & Skills
* **Tool:** Microsoft Power BI Desktop
* **Data Cleaning:** Power Query Editor
* **Analysis:** DAX (Data Analysis Expressions)
* **Visualization:** Clustered Bar Charts, Line Charts, Tree Maps, Slicers.

## 🔍 Steps Followed

### 1. Data Transformation (ETL)
* Imported raw data into Power BI.
* Used **Power Query** to clean the data:
    * Promoted headers.
    * Changed data types (e.g., `Order Date` to Date, `Sales` to Fixed Decimal Number).
    * Removed unused columns to optimize performance.

### 2. Data Modeling & DAX
* Created a dedicated **Date Table** for time-intelligence analysis.
* Created explicit **Measures** for KPIs using DAX:
    ```dax
    Total Sales = SUM(Orders[Sales])
    Total Quantity = SUM(Orders[Quantity])
    Total Transactions = COUNTROWS(Orders)
    ```

### 3. Dashboard Design
* **KPI Cards:** Displayed headline numbers (Total Sales, Profit).
* **Line Chart:** Analyzed monthly sales trends to identify seasonality.
* **Clustered Bar Chart:** Ranked top-performing Sub-Categories (e.g., Phones, Chairs).
* **Tree Map:** Visualized sales distribution across different States and Regions.
* **Slicers:** Added interactivity for users to filter by `Region` and `Year`.


## 💡 Key Insights
1.  **Seasonality:** Sales consistently peak in **November and December**, indicating a strong dependence on holiday shopping.
2.  **Top Products:** **Phones** and **Chairs** are the highest revenue-generating sub-categories.
3.  **Regional Performance:** The **West** region (specifically California) and **East** region (New York) are the top contributors to total sales.
4.  **Strategic Recommendation:** Launch marketing campaigns in Q1 (Jan-Feb) to counteract the significant post-holiday sales dip.

## 🚀 How to Run
1.  Download the `.pbix` file from this repository.
2.  Open it in **Microsoft Power BI Desktop**.
3.  Interact with the slicers to explore different regions and time periods.

---
*Created by Vibin Raj*
