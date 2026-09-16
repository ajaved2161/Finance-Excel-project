# Finance-Excel-project
This Excel Finance Dashboard is designed to analyze revenue performance, product pricing distributions, rounding variances, and regional sales trends using Pivot Tables and Pivot Charts.

Key Performance Indicators (KPIs)
Total Sales (₹4,38,968.00): The cumulative revenue generated across all recorded transactions.

Average Sales (₹552.86): The mean ticket size or revenue per order/transaction.

Round Sales Variance (103): Measures the difference or count of discrepancies introduced when sales figures are rounded to the nearest multiple of 5.

Count of Product (794): The total volume of units sold or individual transaction entries analyzed.

Interactive Filters (Slicers)
Weekday: Allows filtering the dashboard by individual days of the week (Monday through Sunday) to spot daily purchasing behavior.

Product ID: Enables filtering by specific SKUs (PIZB0001 through PIZB0006), isolating individual product performance.

Chart Breakdowns
Daily Sales: Total VS Average:
A 100% stacked column chart comparing total revenue contribution against the average transaction value across product IDs (PIZB0001 to PIZB0006). Products PIZB0005 and PIZB0006 exhibit a significantly higher average order value relative to their total volume share.

Actual Sales VS Round Sales (Nearest 5):
A line/area comparison tracking actual sales amounts against figures rounded to the nearest ₹5 across transaction values (ranging roughly from ₹197 to ₹896) to evaluate rounding impact on accounting margins.

Sales Amount by Price Bucket:
A column chart categorizing revenue by price ranges: Below 300, 300–500, 500–700, and 700 Above. The 700 Above tier generates the bulk of total sales (over ₹1,80,000), followed closely by the ₹500–₹700 bracket.

Product Sale by Price Bucket:
Displays the frequency or distribution of products across the same pricing tiers (300–500, 500–700, 700 Above, and Below 300), illustrating how volume correlates with price tiers.

Region Wise Total Sales Amount:
Compares geographical revenue across four zones (East, North, South, and West). North leads overall sales (exceeding ₹1,12,000), followed by South, with East contributing the lowest share (~₹1,07,000).

Technical Implementation
Formulas Likely Used: ROUND(), MROUND(..., 5) (for rounding to nearest 5), and nested IF() / IFS() or VLOOKUP() with approximate match to generate the price bucket tiers.

Architecture: Raw data fed into multiple Pivot Tables, linked to Pivot Charts, and synchronized dynamically using Slicer Connections (Report Connections).
