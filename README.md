# Sales Management Dashboard

**One-line:** Sales overview dashboard with KPI card, sales by customer & product, budget vs sales line chart and map visualization.

## Features
- Big KPI card showing total sales + budget variance.
- Donut chart for Category split, bar charts for top customers & products.
- Time series for sales vs budget by month.
- Map visualization of sales by customer city.
- Data model with `fact_internetsales`, `dim_customer`, `dim_products`, `dim_calendar`, and `fact_budgets`.

## Tech stack
- Power BI Desktop (.pbix)
- Data: CSVs / Excel extracts
- DAX measures for KPI and variance calculations

## Files
- `reports/SalesManagement.pbix`
- `data/` (sales, customers, products, budgets)
- `screenshots/` (images used in portfolio)

## Key measures (examples)
- `Total Sales = SUM(fact_internetsales[sales_amount])`
- `Budget Amount = SUM(fact_budgets[Budget])`
- `Variance = [Total Sales] - [Budget Amount]`
- `YTD Sales = TOTALYTD([Total Sales], dim_calendar[Date])`

## How to open
1. Clone repo.
2. Open `SalesManagement.pbix` in Power BI Desktop.
3. Update data source paths to `data/` CSV files if necessary.
4. Refresh to load latest data and visuals.

## Publishing
- Publish to Power BI Service to share with stakeholders (or export to PDF).
- For portfolio, export high-quality screenshots and include a brief interactive demo link if available.

## License
MIT (optional)
# Sales-Management-Dashboard
