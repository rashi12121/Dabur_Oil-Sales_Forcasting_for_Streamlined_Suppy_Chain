# Dabur Oil-Sales Forcasting for Streamlined Suppy Chain

## 🏢 About the Company

**Dabur Oils** operates four major oil mills located in **Anand, Ahmedabad, Gandhinagar, and Vadodara**. The company produces **six premium oil varieties**, all packaged in convenient 1-liter bottles to ensure quality and freshness. With detailed sales data provided for the months of **June and July**, this project aims to forecast demand for upcoming months and help streamline the supply chain operations.

![Company Screenshot](https://github.com/rashi12121/Dabur_Oil-Sales_Forcasting_for_Streamlined_Suppy_Chain/blob/main/Dabur%20Logo.png)
![Product  Screenshot](https://github.com/rashi12121/Dabur_Oil-Sales_Forcasting_for_Streamlined_Suppy_Chain/blob/main/Dabur%20Products.png)
---

## 🎯 Objective

The goal of this project is to create a **dynamic demand forecasting model** that:
- Allows Dabur Oils to **compare monthly actual sales with forecasted values**.
- Updates forecasts automatically once real data is received from all oil mills.
- Helps in calculating **accurate production requirements** for the upcoming month.
- Assists decision-making across sales, inventory, and production planning.

---

## 🗂️ Data Overview

- **Sales Data**: Available for June and July, segregated by region:
  - Anand
  - Ahmedabad
  - Gandhinagar
  - Vadodara

- **Inventory Data**:
  - July inventory data is provided.
  - Starting August, the company follows a new policy:
    - **6% of forecasted quantity** is planned as inventory for:
      - Groundnut
      - Mustard
      - Sesame
      - Coconut
    - **12% of forecasted quantity** is planned for other oil types.

- **Forecasting Method**:
  - **August Forecast**: Based on July's growth rate.
  - **September Forecast**:
    - If no clear trend exists, apply a **weighted average**, giving more weight to recent data.
    - Otherwise, use the **average growth rate** of past months.

---

## ❓ Questions to Answer

1. What are the consolidated and region-wise sales for June, July, and August?
2. How is the sales growth rate changing month-on-month?
3. What are the forecasted sales for August and September?
4. What are the inventory requirements under the updated policy?
5. What is the production plan for September?
6. Which inventory levels are critically low and need immediate action?

---

## 📊 EDA & Visualization

- **MasterData** tab consolidates June & July data.
- **RegionWise_Sales** and **ConsolidatedSales** track forecast vs actual sales.
- **Inventory tabs** use conditional formatting:
  - 🔴 Red: Inventory = 0
  - 🟡 Yellow: Inventory ≤ 50% of planned stock
  - 🟢 Green: Inventory > 50% of planned stock

---

## 🌟 Key Insights

- Sales growth rates vary regionally; Anand and Ahmedabad show higher volatility.
- Inventory levels can be optimized using category-specific percentages.
- A weighted forecast provides more accuracy during uncertain trends.
- The dashboard gives a holistic view of sales, inventory, and production.

---

## 🛠️ Tools Used

- **Google Sheets** – Data Integration, Formulae, Analysis
- **Excel Functions** – IF, SUMIFS, VLOOKUP, Conditional Formatting
- **CSV Imports** – Real data integration (August Sales & Inventory)
- **Dashboard Design** – For KPIs, trends, and decision support

---

## 📸 Sales/Inventory Dashboard 

![Dashboard Screenshot](https://github.com/rashi12121/Dabur_Oil-Sales_Forcasting_for_Streamlined_Suppy_Chain/blob/main/_Dabur%20Dashboard.png)



---

## 📁 Project Structure

- `MasterData` – Consolidated raw data (June + July)
- `RegionWise_Sales` – Sales, Forecasts, and Actuals
- `ConsolidatedSales` – Total sales for each product across regions
- `Region-wise Inventory` – Planned vs actual stocks with highlights
- `Consolidated_Inventory` – Company-wide stock summary
- `Regionwise_ProductionPlan` – Forecasted production by location
- `Consolidated_ProductionPlan` – Combined national production needs
- `InventoryDetails_August` – Raw inventory data imported from August CSV

---

## 📦 Final Outcome

This project demonstrates how Dabur Oils can automate and scale their forecasting and inventory operations using structured data pipelines and smart forecasting logic.
