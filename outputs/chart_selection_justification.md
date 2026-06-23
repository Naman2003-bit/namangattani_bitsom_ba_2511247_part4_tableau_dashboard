# Chart Selection Justification

## 1. Monthly Sales Trend By Region (2024–2025)

### Business Question
How are sales evolving over time across different regions?

### Chart Type Used
Line Chart

### Why This Chart Is Appropriate
A line chart is the most suitable way to display trends over time. It enables leadership to spot growth patterns, seasonal movements, fluctuations, and performance differences across regions.

### Fields Used

* X-Axis: Order Date (Month)
* Y-Axis: Sales
* Color: Region
* Filter: Region

### Design Principles Applied

* Consistent colour coding per region
* Clear chronological progression
* Minimal visual clutter
* Straightforward cross-region comparison

### Mistake Avoided
Pie charts and stacked bar charts were avoided as they are poorly suited to displaying time-series trends.

---

## 2. Regional Sales and Profit Performance

### Business Question
Which region delivers the highest sales and profit contribution?

### Chart Type Used
Horizontal Bar Chart

### Why This Chart Is Appropriate
Bar charts make it easy to compare values across categories. A horizontal layout improves the readability of region labels and supports quick ranking.

### Fields Used

* Category: Region
* Measure: Sales
* Color: Profit
* Filter: Region

### Design Principles Applied

* Sorted bars for immediate ranking clarity
* Colour intensity used to represent profitability levels
* Clear value labels throughout

### Mistake Avoided
Pie charts were avoided as they make it difficult to accurately compare performance across multiple regions.

---

## 3. Category Profitability by Sub-Category

### Business Question
Which product sub-categories produce the highest profit?

### Chart Type Used
Horizontal Bar Chart

### Why This Chart Is Appropriate
Ranking across sub-categories demands precision. Horizontal bars handle a large number of categories effectively while keeping the visual easy to read.

### Fields Used

* Category: Sub-Category
* Measure: Profit
* Color: Product Category
* Filter: Category

### Design Principles Applied

* Descending sort order for instant prioritisation
* Distinct colours used to differentiate product categories
* Direct data labels for quick reference

### Mistake Avoided
Treemaps were avoided as they can make precise profit comparisons across sub-categories harder to interpret.

---

## 4. Sales Performance by Customer Segment

### Business Question
Which customer segment generates the highest sales volume?

### Chart Type Used
Bar Chart

### Why This Chart Is Appropriate
Bar charts offer a clean and accurate way to compare sales figures across customer segments.

### Fields Used

* Category: Customer Segment
* Measure: Sales
* Color: Profit
* Filter: Customer Segment

### Design Principles Applied

* Consistent formatting throughout
* Simple side-by-side comparison between segments
* Clear and readable labels

### Mistake Avoided
Pie charts were avoided as they can obscure smaller performance differences between segments.

---

## 5. Discount Impact on Profitability

### Business Question
What effect does discounting have on profitability?

### Chart Type Used
Scatter Plot with Trend Line

### Why This Chart Is Appropriate
Scatter plots are well suited to identifying relationships and correlations between two numerical variables. The trend line makes the overall direction of the relationship immediately visible.

### Fields Used

* X-Axis: Discount
* Y-Axis: Profit
* Color: Category
* Detail: Order ID

### Design Principles Applied

* Trend line included to aid interpretation
* Separate colours assigned to each category
* Clear and descriptive axis labels

### Mistake Avoided
Bar charts were avoided as they cannot effectively reveal correlation between two continuous variables.

---

## 6. Average Delivery Days by Shipping Mode

### Business Question
Which shipping method tends to experience the longest delivery times?

### Chart Type Used
Horizontal Bar Chart

### Why This Chart Is Appropriate
A bar chart enables direct comparison of average delivery durations across different shipping modes.

### Fields Used

* Category: Ship Mode
* Measure: Average Delivery Days

### Design Principles Applied

* Values sorted for easy comparison
* Data labels displayed on bars
* Clean and uncluttered layout

### Mistake Avoided
Line charts were avoided because shipping modes are discrete categories rather than time-based data points.

---

## 7. Returns by Category and Customer Segment

### Business Question
Which product categories and customer segments record the highest return volumes?

### Chart Type Used
Stacked Bar Chart

### Why This Chart Is Appropriate
Stacked bars allow the total return count per category to be compared while also revealing how each customer segment contributes to that total.

### Fields Used

* Category: Product Category
* Measure: Return Flag
* Color: Customer Segment

### Design Principles Applied

* Colour differentiation applied across segments
* Cross-category comparison made straightforward
* Return counts clearly labelled

### Mistake Avoided
Pie charts were avoided as displaying multiple categories and segments simultaneously would make comparisons very difficult to follow.

---

## Dashboard Design Principles
The dashboard was built in line with the following visualisation best practices:

* Chart types matched to the specific business question being answered
* Consistent formatting and colour usage applied throughout
* Clear titles and labels on all visuals
* Interactive filters included to support user exploration
* KPI cards placed at the top for immediate executive visibility
* Minimal clutter with no unnecessary visual elements
* Action filters incorporated to enhance interactivity
* Business-driven storytelling prioritised over decorative design choices

These decisions ensure that leadership can quickly identify performance trends, risks, and opportunities to support informed decision-making.
