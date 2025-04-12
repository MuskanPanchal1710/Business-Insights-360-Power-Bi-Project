# Business Insights 360

AtliQ Hardware, a rapidly growing company, embarked on its first data analytics initiative to gain a competitive edge in the market and embrace data-driven decision-making. This Power BI project was developed to support key stakeholders across various departments—Finance, Sales, Marketing, and Supply Chain—by providing actionable insights through interactive dashboards and reports.

The objective was to transform raw data into meaningful visualizations that help answer critical business questions, identify performance trends, and drive strategic planning across the organization.

# Data Sources

The dashboard integrates data from two main sources:

* **Excel/CSV Files:** Includes targets, market share data, and other related metrics collected from Excel and CSV files.

* **MySQL Database:** Retrieves key fact and dimension tables across all departments to support comprehensive analysis.

# Power BI Skills and Techniques Gained

Throughout this project, I explored a wide range of Power BI features and best practices, gaining hands-on experience in building interactive, dynamic dashboards. Key skills and techniques I learned include:

* Creating calculated columns and measures using DAX language

* Building robust Data models (Data Modeling)

* Implementing bookmarks to toggle between different visuals

* Enabling smooth page navigation using buttons.

* Designing dynamic titles that respond to filters and slicers

* Applying KPI indicators to track performance effectively

* Using conditional formatting with icons or color scales to highlight insights

* Publishing reports to Power BI Service
* Data integration from various sources like Excel/CSV files, MySQL database, etc.

# Business Terminology
* Gross price
* Pre-invoice deductions
* Post-Invoice deductions
* Net Invoice sale
* Gross Margin
* Net sales
* Net profit
* COGC - cost of goods sold
* YTD - Year to Date
* YTG - Year to Go
* Direct
* Retailer
* Distributors
* Consumer
* FY-Fiscal Year
# Dataset Overview
A clear understanding of the available data is crucial before beginning any analysis. The dashboard relies on structured datasets from two main databases: gdb041 (sales and forecasting) and gdb056 (costs and pricing).


🔸 Dimension Tables
dim_customer
Attribute	                               Description
Markets	                                 27 (e.g., India, USA, Spain)
Customers	                               75 unique customers across all markets
Platforms	                               Brick & Mortar, E-commerce (Amazon, Flipkart)
Sales Channels	                         Retailer, Direct, Distributor
dim_market
Attribute	Description
Markets	27 markets
Sub-zones	7 sub-zones
Regions	4 (APAC, EU, LATAM, nan)
dim_product
Attribute	Description
Divisions	P&A (Peripherals, Accessories, PC), N&S (Networking, Storage)
Categories	14 total (e.g., Internal HDD, Keyboard)
Variants	Multiple variants per product
🔹 Fact Tables
fact_forecast_monthly
Attribute	Description
Date Format	Monthly granularity (start date of month)
Purpose	Forecasts customer needs to: improve satisfaction, reduce warehouse costs
Structure	Denormalized for analytics; includes forecasted quantity
fact_sales_monthly
Attribute	Description
Structure	Similar to fact_forecast_monthly
Key Difference	Final column contains actual sold quantity instead of forecasted value
</details>
<details> <summary><strong>🗂️ gdb056: Cost & Pricing Data</strong></summary>
🔸 Cost & Pricing Tables
Table Name	Description
freight_cost	Travel and logistics costs per market and fiscal year
gross_price	Product gross pricing by product code
manufacturing_cost	Yearly manufacturing costs by product
pre_invoice_deductions	Pre-invoice deduction percentages by customer and year
post_invoice_deductions	Post-invoice and other deduction details

