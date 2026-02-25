# REGAL RETAIL.
## CLIENT BACKGROUND

Regal Retail is a US-based general retail store founded in 2021. They specialize in selling a variety of products, including meats and beverages, furniture, and everyday essentials like food and milk products, etc. The store has experienced exponential growth and has been a net positive for the community. They have as many as 300 active customers annually and sales records close to 13,000, with total revenue exceeding $1.5M across 3 years and a single quarter. 

The available retail store data spans various dimensions and metrics, including sales, sales by products, discounts applied, AOV, and total sales by location. Discounts are a fair part of their brand's identity, as they are in their early stages. This would be a rundown of their total sales analysis.

An in-depth analysis was conducted to evaluate Regal Retail's performance over the past several years (2022-2024 and Q1 of 2025). This comprehensive review provides valuable insights that internal cross-functional teams will use to streamline processes, enhance Regal Retail’s commercial performance, and help them achieve their NorthStar Metrics.

The key insights and recommendations focus on the following areas:
Northstar Metrics: Customer Lifetime Value(CLV)
The sales trend focuses on the number of sales, revenue retention, and Average Order Value (AOV), among others.
Product performance - Analyzing different product lines, discounts, and revenue spikes.
Sales channels, discounts, and resource allocation for improved sales and customer satisfaction.

An interactive PowerBI dashboard can be downloaded here

The SQL queries utilized to inspect and perform quality checks can be found here

The SQL queries utilized to clean, organize, and prepare data for the dashboard can be found here

Targeted SQL queries regarding various business questions can be found here

# Retail Sales Analytics – Power BI Project

## Business Problem

The company collected retail data but lacked insight into:

- Which locations and categories drive revenue
- How much sales depend on discounts
- Seasonal trends for planning inventory
- Average order behavior across stores

Decisions were being made based on intuition instead of data.

---

## What I Worked on. What I did(Analytics Process)

### 1. Data Cleaning & Preparation
- I profiled raw CSV data for quality issues  
- Removed duplicates and handled missing values  
- I also applied IQR method to detect outliers  
- I converted transaction dates for time intelligence  
- I created dimension tables (product, location, date, customer)

### 2. Data Modeling
- Designed a **star schema** with:
  - Fact table: sales transactions  
  - Dimension tables: product, location, date, customer  
- Built one-to-many relationships  
- And validated filter context behavior

### 3. DAX & Metrics
Created business KPIs:

- Total Sales  
- Total Transactions  
- Average Order Value  
- Discount Contribution  
- High-Value Sales  
- MoM Growth  
- YTD Sales

### 4. Dashboard Design
Built a 3-page interactive report:

1. **Overview** – KPIs, trend, location performance  
2. **Sales Analysis** – category & product insights  
3. **Discount Behavior** – impact of promotions

---

## Business Insights Discovered

- The **Butchers category within the dataset generated the highest revenue**, indicating strong customer demand and the need to prioritize inventory and supplier relationships in this segment  
- Discounts contributed only a **small portion of total sales (≈0.34 impact)**, showing that the business is not heavily reliant on promotions to drive revenue  
- Sales patterns were **relatively stable across months**, suggesting consistent demand rather than strong seasonality. Sales were relatively consistent across months.  
- Performance differences across locations highlight opportunities for sharing best practices from top stores.
---


## Recommendations (Way Forward)

1. Prioritize the Butchers category for:
   - Inventory availability  
   - Supplier negotiation  
   - Product variety expansion  

2. Maintain current pricing strategy since:
   - Discounts have minimal influence  
   - Customers appear value-driven rather than promotion-driven  

3. Focus on operational improvements:
   - Study high-performing locations  
   - Replicate layout and product mix  
   - Introduce cross-selling with related categories  

4. Next Analytics Steps:
   - Add profit and margin data  
   - Analyze repeat purchase behavior  
   - Introduce forecasting for stock planning


---

## Tools Used

- Power BI  
- DAX  
- Python (Pandas)  
- Data Modeling  
- Business Intelligence Design

---

## Skills Demonstrated

- Data Cleaning & Transformation  
- Feature Engineering  
- Star Schema Modeling  
- KPI Development  
- Dashboard Storytelling  
- Business Analysis

---

## Screenshots

### Overview Page
![Overview](screenshots/PAGE_1-Overview_and_Slicers.png)

### Sales Analysis
![Analysis](screenshots/PAGE_2-Category_and_Table.png)

### Discount Analysis
![Discounts](screenshots/PAGE_3-Discount_Visuals.png)

---

## How to Use

1. Download the `.pbix` file  
2. Open with Power BI Desktop  
3. Refresh data from processed CSVs  
4. Explore using slicers and filters

---

## Author

Chika-Ezeagu Victor – Data Analytics and Comp Sci Student
