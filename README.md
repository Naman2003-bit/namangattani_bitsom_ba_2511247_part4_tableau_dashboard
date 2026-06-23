# Retail Executive Performance Dashboard

## Business Problem Summary
Retail leadership requires a centralised dashboard to track business performance across sales, profitability, customer segments, shipping operations, discount effectiveness, and return patterns. The goal is to surface growth opportunities, operational risks, and actionable insights that enable data-driven decision-making.

---

## Dataset Description

The dashboard is built on the following dataset:

**dashboard_sales_data.xlsx**

The dataset contains retail transaction-level records covering:

* Order Date
* Ship Date
* Region
* State
* Customer Segment
* Category
* Sub-Category
* Sales
* Profit
* Discount
* Quantity
* Shipping Mode
* Return Flag
* Customer Rating
* Campaign Channel

The data was analysed in Tableau to produce all visualisations and business insights.

---

## Tableau Workbook Description

**Workbook File:**

**tableau/executive_dashboard.twbx**

The workbook includes the following sheets:

1. KPI_Total_Sales
2. KPI_Total_Profit
3. KPI_Average_Order_Value
4. Sales_Trend
5. Regional_Performance
6. Category_Profitability
7. Customer_Segment
8. Shipping_Performance
9. Discount_vs_Profit
10. Return_Analysis
11. Executive_Dashboard

The dashboard brings all major business performance indicators together into a single executive-level view.

---

## Calculated Fields Created

### 1. Profit Margin

```text
Profit / Sales
```

**Purpose:**
Measures the profitability generated for every dollar of sales revenue.

### 2. Cost

```text
Sales - Profit
```

**Purpose:**
Estimates product cost by removing profit from total sales.

### 3. Average Order Value

```text
SUM(Sales) / COUNTD([Order Id])
```

**Purpose:**
Calculates the average revenue generated per individual order.

### 4. Return Rate

```text
SUM([Return Flag]) / COUNT([Order Id])
```

**Purpose:**
Measures the proportion of orders that were returned.

### 5. Shipping Delay Bucket

```text
IF [Delivery Days] <= 2 THEN "Fast (0-2 Days)"
ELSEIF [Delivery Days] <= 5 THEN "Normal (3-5 Days)"
ELSE "Delayed (6+ Days)"
END
```

**Purpose:**
Groups delivery performance into clearly defined business categories.

---

## Dashboard Components

### KPI Cards

* Total Sales
* Total Profit
* Average Order Value

### Analytical Views

* Monthly Sales Trend by Region
* Regional Sales and Profit Performance
* Category Profitability by Sub-Category
* Sales Performance by Customer Segment
* Discount Impact on Profitability
* Average Delivery Days by Shipping Mode
* Returns by Category and Customer Segment

---

## Filters and Interactions Used

### Filters

* Region
* Category
* Customer Segment

### Dashboard Interactions

* The Region filter refreshes all views across the dashboard.
* The Category filter updates all category-related analyses.
* The Customer Segment filter drives all customer-focused visualisations.
* Action filtering allows users to drill into specific business segments interactively.

---

## Key Business Insights

### Insight 1
The South region records the highest overall sales performance.

### Insight 2
Technology sub-categories deliver the greatest profit contribution.

### Insight 3
Home Office customers generate the largest share of total sales volume.

### Insight 4
Higher discount levels are generally associated with lower profitability.

### Insight 5
Standard Class shipping consistently experiences the longest delivery durations.

### Insight 6
Furniture products account for the highest number of returns.

### Insight 7
Sales performance remains broadly stable throughout the analysis period.

### Insight 8
Reducing return volumes and managing discount levels more carefully can meaningfully improve overall profitability.

---

## Dashboard Story Summary
The dashboard presents a picture of a business that is performing well overall but faces profitability pressures tied to excessive discounting and product returns.

Technology products and the South region stand out as key business strengths, while Furniture returns and shipping delays highlight areas with room for improvement.

The dashboard supports executive decision-making by connecting sales performance, profitability, customer behaviour, logistics efficiency, and return management within a single analytical view.

---

## Assumptions and Limitations

### Assumptions

* Dataset values are assumed to be accurate and complete.
* The Return Flag correctly identifies all returned orders.
* Delivery Days accurately capture the true shipping duration.
* Order IDs uniquely represent individual customer transactions.

### Limitations

* The analysis draws exclusively on historical data.
* External market conditions are not factored into the findings.
* Customer satisfaction data is not available within the dataset.
* Inventory levels and detailed operational cost information are not included.

---

## Screenshots Included

### full_dashboard.png
Complete executive dashboard view.

### sales_trend_view.png
Monthly sales trend analysis.

### regional_performance_view.png
Regional sales and profit comparison.

### category_profitability_view.png
Category and sub-category profitability breakdown.

### filter_interaction_view.png
Demonstration of dashboard filter interactivity in action.

---

## Conclusion
The Retail Executive Performance Dashboard delivers a consolidated view of business performance spanning revenue, profitability, customer behaviour, logistics efficiency, and operational risk. It enables faster, more confident decision-making and helps leadership identify both opportunities for growth and areas that require corrective action.
