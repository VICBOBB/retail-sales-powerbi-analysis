# <img width="1920" height="1080" alt="Regal Retail" src="https://github.com/user-attachments/assets/9c939bd3-bc33-42b6-ba21-fb5541637fd1" />
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

An interactive PowerBI dashboard can be downloaded ![here]()

The SQL queries utilized to inspect and perform quality checks can be found ![here]()

The SQL queries utilized to clean, organize, and prepare data for the dashboard can be found ![here]()

Targeted SQL queries regarding various business questions can be found ![here]()

# Retail Sales Analytics – Power BI Project

## EXECUTIVE SUMMARY
<img width="1288" height="638" alt="Total Sales by Year" src="https://github.com/user-attachments/assets/8562a1c9-e511-4b48-9860-bc4817eb3776" />

Revenue Growth and Retail Performance: 
Total sales across 2022-2025 are $1.55M, ranging monthly from $37k to $49k. 
January 2022 made the most sales with $53k, while January 2025 records the lowest with sales as low as $26k. 
More sales are made online than offline. The difference is minor, if not negligible, with online sales leading by only 2%. 
The Butchers and Beverages category saw the largest revenue spikes in Q3 of 2022 and Q1 of 2023, respectively.

Declining Trend in 2025:
January 2022 made the most sales with $53k, while Jan 2025 records the lowest with sales as low as $26k.
There are no main drivers of sales or dips in the graph, as most sales sit closely together in revenue earned. 

Quarterly Insights and Seasonal Trends: 
The top-performing department is the Butchers department, making sales up to $208k, while the worst-performing product is the milk products, with sales only going as high as $108k, responsible for less than 13% of sales. 
66.21% of sales made, which account for $1.03M, did not have discount pricing attached to them. Only $0.52M, which accounts for 33.79% of sales, was born of discounted pricing.
The Butchers and Beverages category saw the largest revenue spikes in Q3 of 2022 and Q1 of 2023, respectively.
Quarterly and global sales trends do not show any major seasonal trend in sales. However, at the beginning, middle, and end of every year except 2025, there is a sales spike, which is most likely due to the end of the year and summer holidays.

Key Takeaways & Recommendations: 
Conduct sanity checks on key dimensions to determine whether there's a clear driver. There was no record of the specific products in each category, making it almost impossible to track which product was responsible.
Investigate the drop in sales. It could be a seasonal issue, a sales record issue, a marketing issue, or even a product quality issue. 
Dedicate more resources to raising global sales and diversify locations from just a single store to multiple stores at different locations. This would improve in-store access for many customers and would even improve reach for online customers, thereby improving customer satisfaction.
More resources should go to ads and promotions for all products, across the board, but keep an eye on beverages and furniture, since they tend to dip more than other products and categories. 


## Business Insights Discovered

- The **Butchers category within the dataset generated the highest revenue**, indicating strong customer demand and the need to prioritize inventory and supplier relationships in this segment  
- Discounts contributed only a **small portion of total sales (≈0.34 impact)**, showing that the business is not heavily reliant on promotions to drive revenue  
- Sales patterns were **relatively stable across months**, suggesting consistent demand rather than strong seasonality. Sales were relatively consistent across months.  
- Performance differences across locations highlight opportunities for sharing best practices from top stores.
---


## RECOMMENDATIONS.

### General:
-Do sanity checks on key dimensions to investigate if there's a clear driver. Investigate the drop in sales. Was it a seasonal issue, a marketing issue, or even a product quality issue?
-Dedicate more resources to raising global sales and diversify locations from just a single store to multiple stores at different locations. This would improve in-store access for many customers and even ensure that online orders reach their intended destinations earlier.
-Product variety expansion.
### Prioritize the Butchers category for:
-Inventory availability.  
-Supplier negotiation. 
-Product variety expansion. 
-Push more resources towards the butcher section, electric household essentials, beverages, and furniture(because of the spike). These categories seem to be among the major drivers of all spikes in the total sales graph, compared to other categories.
### Maintain current pricing strategy since:
-Discounts have minimal influence  
-Customers appear value-driven rather than promotion-driven 
### Focus on operational improvements:
-Study high-performing locations  
-Replicate layout and product mix  
-Introduce cross-selling with related categories  
### Next Analytics Steps:
-Add profit and margin data  
-Analyze repeat purchase behavior  
-Introduce forecasting for stock planning
-Lastly, the store appears to be doing well with the data provided. More ads for general revenue growth and fulfillment of Northstar metrics are highly encouraged.

---

## Tools Used

- Power BI  
- DAX  
- Python (Pandas)  
- Data Modeling  
- Business Intelligence Design

---

## CAVEATS AND ASSUMPTIONS:
-Discounts need better recording. Some were missing in store records. Though the numbers were minimal and the impact negligible, it's still better to just have those completed. This is for the sales and finance team to take note of.
-For future reference, please keep a detailed record of the products sold in each category. It would make it easier to pinpoint which product within a category caused the spike in revenue and sales.


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
