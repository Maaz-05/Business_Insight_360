# Business Insights 360

## Problem Statement

AtliQ Hardware, a global consumer electronics company, was facing challenges in managing and analyzing large volumes of business data using traditional Excel-based reporting. The existing reporting system lacked scalability, interactive visualization, and real-time analytical capabilities, making it difficult for stakeholders to track KPIs, monitor business performance, and make informed strategic decisions across different departments.

---

## Project Objective

The objective of this project was to build an end-to-end Business Intelligence solution that transforms raw business data into meaningful insights for Finance, Sales, Marketing, Supply Chain, Executive, and Product teams. The dashboard was designed to help business leaders monitor KPIs, analyze trends, improve forecasting accuracy, and optimize decision-making through interactive and dynamic reporting.

---

# Live Dashboard

[🔗 View Live Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYmFhZmQzMTctYzNiNS00MzRiLTliY2UtZTMwMGU4MDY4YjQ2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

---

# Dashboard Views

## Home View
- Designed a centralized home page for smooth navigation across different dashboard views.
- Added interactive buttons and navigation icons for better user experience.
- Displayed last refresh date and sales data availability information for report transparency.

### Home View Preview
![Home View]()


---

## Finance View
- Developed Profit & Loss (P&L) reports to analyze revenue, expenses, and profitability trends.
- Created KPI visuals for Net Sales, Gross Margin %, and Net Profit % against benchmark values.
- Built Top & Bottom customer and product analysis based on Net Sales contribution.

### Finance View Preview
![Finance View](images/finance_view.png)

---

## Sales View
- Built customer and product performance dashboards using Net Sales and Gross Margin metrics.
- Created performance matrix visuals to identify high-performing customers and products.
- Designed key metric visualizations for COGS, Gross Margin, and invoice deductions.

### Sales View Preview
![Sales View](images/sales_view.png)

---

## Marketing View
- Analyzed market, region, and customer performance using key profitability metrics.
- Developed profitability matrices and unit economics visuals for strategic marketing insights.
- Built waterfall and donut charts to visualize operational expenses and profit distribution.

### Marketing View Preview
![Marketing View](images/marketing_view.png)

---

## Supply Chain View
- Created dashboards to monitor Forecast Accuracy, Net Error, and ABS Error trends.
- Designed trend analysis visuals for supply chain performance monitoring.
- Generated product-level KPI insights to support operational planning and inventory decisions.

### Supply Chain View Preview
![Supply Chain View](images/supply_chain_view.png)

---

## Executive View
- Developed high-level executive dashboards for business monitoring and KPI tracking.
- Visualized yearly trends for Net Sales, Gross Margin %, Net Profit %, and Market Share %.
- Built revenue distribution reports across divisions, channels, and regions.

### Executive View Preview
![Executive View](images/executive_view.png)

---

## Product View
- Created Top 5 and Bottom 5 product analysis reports using Gross Margin performance.
- Implemented conditional formatting to identify customers achieving target profitability goals.

### Product View Preview
![Product View](images/product_view.png)

---

# Data Source Details

Understanding the available data before analysis was essential for building accurate dashboards and generating meaningful business insights.

## Data Structure
- **Dimension Tables:** Contain static information such as customer and product details.
- **Fact Tables:** Store transactional and business performance data.

---

## Database: gdb041

### dim_customer
- 27 distinct markets (India, USA, Spain, etc.)
- 75 distinct customers across markets
- 2 platform types:
  - Brick & Mortar (Offline stores)
  - E-commerce (Amazon, Flipkart)
- 3 sales channels:
  - Retailer
  - Direct
  - Distributor

### dim_market
- 27 distinct markets
- 7 sub-zones
- 4 regions:
  - APAC
  - EU
  - LATAM
  - NA

### dim_product
- Product divisions:
  - P & A
    - Peripherals
    - Accessories
  - PC
    - Notebook
    - Desktop
  - N & S
    - Networking
    - Storage
- 14 different product categories
- Multiple product variants available

### fact_forecast_monthly
- Used for forecasting customer demand in advance
- Helps reduce warehouse storage costs and improve customer satisfaction
- Contains forecast quantity data for customers

### fact_sales_monthly
- Contains monthly sales transaction data
- Similar to forecast table but stores sold quantity instead of forecast values

---

## Database: gdb056

### freight_cost
- Contains freight and travel costs for each market and fiscal year

### gross_price
- Stores gross price details for products

### manufacturing_cost
- Contains yearly manufacturing cost details

### pre_invoice_deductions
- Contains customer-level pre-invoice deduction percentages

### post_invoice_deductions
- Stores post-invoice deductions and additional deduction details

> Note: Benchmark and target values were available only for Fiscal Year 2022.

---

# Technical Skills Used

- Power BI
- MySQL
- Power Query
- DAX
- Data Modeling
- DAX Studio
- ETL (Extract, Transform, Load)
- Interactive Dashboard Design

---

# Key Business Insights

- Notebook and Peripheral segments generated the highest revenue contribution.
- Amazon, AtliQ Exclusive, and Flipkart were among the top-performing customers based on Net Sales.
- APAC and North America were the strongest performing regions in terms of revenue.
- Forecast analysis helped identify inventory risks including Out of Stock (OOS) and Excess Inventory (EI).

---

# Key Learnings

- Gained practical experience in end-to-end Business Intelligence and analytics workflows.
- Improved understanding of Finance, Sales, Marketing, Executive, and Supply Chain reporting.
- Learned advanced data modeling, KPI analysis, dashboard optimization, and stakeholder-focused reporting.
- Developed the ability to transform complex raw data into interactive and business-driven insights.
