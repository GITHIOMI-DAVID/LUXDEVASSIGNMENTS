# Jumia Product Performance Dashboard

## 📊 Project Overview
This project focuses on analyzing the performance of products listed on **Jumia**, a leading e-commerce platform. By examining pricing strategies, discount impacts, and customer feedback metrics, this interactive Excel dashboard provides actionable insights into consumer behavior and product engagement.

## 🎯 Project Objective
The goal is to design and build an interactive Excel dashboard that explores how pricing, discounts, and ratings influence customer engagement. This project supports data-driven decision-making for e-commerce optimization.

---

## 📂 Dataset Description
The dataset includes product-level data with the following attributes:
* **Product:** Name of the item.
* **Current Price:** Selling price (KSh).
* **Old Price:** Original price before discount (KSh).
* **Discount:** Percentage reduction applied.
* **Reviews:** Total number of customer reviews.
* **Rating:** Average customer rating (out of 5).

---

## 🛠️ Data Cleaning & Preparation
To ensure data integrity, the following steps were performed:
1.  **Handling Missing Values:** Addressed nulls in the `Reviews` and `Rating` columns.
2.  **Deduplication:** Removed duplicate product entries.
3.  **Data Type Conversion:** * Stripped "KSh" and commas from price columns to convert them to numeric format.
    * Cleaned the `Rating` column (e.g., converting "4.5 out of 5" to `4.5`).
4.  **Formatting:** Standardized the `Discount` column as a percentage.
5.  **Error Correction:** Converted negative review values to positive.

---

## 🧪 Data Enrichment
New calculated columns were created to enhance the analysis:
* **Discount Amount (KSh):** `Old Price - Current Price`
* **Rating Category:** * *Poor:* < 3
    * *Average:* 3 - 4.4
    * *Excellent:* ≥ 4.5
* **Discount Category:** * *Low:* < 20%
    * *Medium:* 20% - 40%
    * *High:* > 40%

---

## 📈 Key Insights & Analysis
### Descriptive Analysis
* Calculation of average pricing, discounts, and ratings across the catalog.
* Identification of price extremes (most and least expensive items).
* Distribution of products across rating and discount tiers.

### Trend & Relationship Analysis
* **Discount vs. Engagement:** Correlation between discount depth and the number of reviews.
* **Rating vs. Volume:** Analyzing if higher-rated products naturally attract more reviews.

### Top Performers
* Ranked lists for the Top 10 most discounted products.
* Ranked lists for the Top 10 most reviewed products.
* Comparative analysis of the Top 5 and Bottom 5 rated items.

---

## 🖥️ Dashboard Features
The final Excel dashboard is a single-page interactive interface featuring:
* **KPI Scorecards:** Total products, average rating, average discount, and total reviews.
* **Interactive Visuals:** * Bar/Column charts for top product performance.
    * Scatter plots for trend analysis (Discount vs. Reviews).
    * Donut charts for category breakdowns.
* **Dynamic Filtering:** Integrated **Slicers** for *Rating Category*, *Discount Category*, and *Price Range*.

---

## 🚀 How to Use
1.  Clone this repository.
2.  Open the `Jumia_Analysis_Dashboard.xlsx` file.
3.  Use the **Slicers** on the right side of the dashboard to filter data dynamically.
4.  If you update the raw data, go to the `Data` tab and click **Refresh All** to update the Pivot Tables and Charts.
