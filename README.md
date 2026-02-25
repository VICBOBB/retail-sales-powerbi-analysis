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

### Revenue Growth and Retail Performance: 
-Total sales across 2022-2025 are $1.55M, ranging monthly from $37k to $49k. 
-January 2022 made the most sales with $53k, while January 2025 records the lowest with sales as low as $26k. 
-More sales are made online than offline. The difference is minor, if not negligible, with online sales leading by only 2%. 
-The Butchers and Beverages category saw the largest revenue spikes in Q3 of 2022 and Q1 of 2023, respectively.

<img width="715" height="191" alt="Declining Sales" src="https://github.com/user-attachments/assets/a49e900f-349e-4854-bd1c-1ffb426e4a19" />
### Declining Trend in 2025:
-January 2022 made the most sales with $53k, while Jan 2025 records the lowest with sales as low as $26k.
-There are no main drivers of sales or dips in the graph, as most sales sit closely together in revenue earned. 

### Quarterly Insights and Seasonal Trends: 
-The top-performing department is the Butchers department, making sales up to $208k, while the worst-performing product is the milk products, with sales only going as high as $108k, responsible for less than 13% of sales. 
-66.21% of sales made, which account for $1.03M, did not have discount pricing attached to them. Only $0.52M, which accounts for 33.79% of sales, was born of discounted pricing.
-The Butchers and Beverages category saw the largest revenue spikes in Q3 of 2022 and Q1 of 2023, respectively.
-Quarterly and global sales trends do not show any major seasonal trend in sales. However, at the beginning, middle, and end of every year except 2025, there is a sales spike, which is most likely due to the end of the year and summer holidays.

### Key Takeaways & Recommendations: 
-Conduct sanity checks on key dimensions to determine whether there's a clear driver. There was no record of the specific products in each category, making it almost impossible to track which product was responsible.
-Investigate the drop in sales. It could be a seasonal issue, a sales record issue, a marketing issue, or even a product quality issue. 
-Dedicate more resources to raising global sales and diversify locations from just a single store to multiple stores at different locations. This would improve in-store access for many customers and would even improve reach for online customers, thereby improving customer satisfaction.
-More resources should go to ads and promotions for all products, across the board, but keep an eye on beverages and furniture, since they tend to dip more than other products and categories. 

## DATA STRUCTURE AND INITIAL CHECKS(includes Star Schema)
The database structure contains 5 major tables: the date dimension, customer dimension, location dimension, and product dimension, all connected to the fact table, with a total of 11,12575 records.
<img width="759" height="681" alt="Star Schema" src="https://github.com/user-attachments/assets/b7432e2b-98ef-4af3-8361-3ca22d2ec215" />

## INSIGHT DEEP-DIVE
## SALES TREND
<img width="1050" height="125" alt="Sales Summary" src="https://github.com/user-attachments/assets/724fbb2a-2a53-47d4-867d-c72673760039" />
<img width="1278" height="319" alt="Total Sales by Year and Month" src="https://github.com/user-attachments/assets/2b9519fa-9499-4f69-8880-e677d2d85c7e" />

### SALES: 
-Total sales across 2022-2025 are $1.55M, ranging monthly from $37k to $49k, and tanking significantly in 2025 to just $26k. With January 2022 holding the highest number of sales, with numbers up to $53k
-The top-performing department is the Butchers department, selling more online than it did offline. It made sales up to $208k, while the worst performing product is the milk products, with sales only going as high as $108k. The worst-performing category is milk products, accounting for less than 13% of sales.
-Many products are purchased in bulk quantities, especially the Butchers category and Milk products, with MoM growth ranging from 1.59% to 2.22% usually.
-Most categories outperform each other by a margin of $2k - $4k.

<img width="342" height="355" alt="Total Sales by Location" src="https://github.com/user-attachments/assets/28b38d7c-2bc1-4aae-b5a2-c9c1cc996dc3" />
### REVENUE RETENTION, AND LOCATION: 
-More sales are made online than offline. The difference is minor, with online sales leading by only 2%. 
-AOV: AOV across the years stays consistently at $123, indicating relative stability or stagnancy in sales except for in the first quarter of 2025, where AOV decreases to $120. 
-That said, the monthly AOV for each year ranges roughly from $116 to $130, with 2024 recording the highest AOV with $141 in the month of April due to a spike in Beverage sales.

## ORDER COUNT
-The order count remained relatively stable from 2022 to 2024, then plummeted in 2025, with annual total transactions falling from as high as 4k over 3 consecutive years to only 213 in January of 2025.
-The sales decline was rapid in the first month of 2025, with orders dropping from 376 in December to 216 in January, and High Value Sales were cut by half. -However, the order count is not the only thing greatly affected; sales dropped from $48k to $26k.

## PRODUCT PERFORMANCE
<img width="1284" height="523" alt="Total Sales by Category" src="https://github.com/user-attachments/assets/6f5b1089-49c1-4215-b613-db0b67a7fd1e" />
### Performance detail: 
-The 3 best-performing product categories were Butchers, Electric Household Essentials, and Beverages, with Milk products performing the least. 
-The gap between products' performance is negligible, possibly due to their physical location, as demand for these products in this area is not that different.
-Across the years, each product had relatively similar dips and spikes in revenue, with Furniture having the most contrast between them. These spikes contributed the most to Butchers and Beverages, leading in sales and helping furniture move up the performance ladder, even though most of its sales were relatively average.

<img width="513" height="350" alt="Total Sales by Discount Applied" src="https://github.com/user-attachments/assets/19a66e14-99e2-43aa-9975-540c8ee7fb98" />
### Discounts: 
-Discounts did not greatly affect sales, as the discount sales percentage usually ranges around 0.34%. The Butchers category experienced the most discounts at 4.67%, while Milk Products had the least at 3.89%.

<img width="1295" height="559" alt="Total Sales by Varying Categories" src="https://github.com/user-attachments/assets/51ff1478-d0dd-41dd-8def-33d35b400108" />
### Revenue Spikes: 
-A few categories, namely Butchers, Beverages, and Furniture, experienced the most spikes, greatly impacting their sales performance and being a net positive for the retail store. 
-Ironically, Electric Essentials, the second-best-selling category, didn’t experience significant spikes; it remained fairly consistent. 
-Beverages experienced the most recurring spikes, with sales reaching as high as $2316 and $1827, occurring all in one day in Q1 of 2023 and 2024. This likely occurs due to the high demand for fitness drinks that occurs around Q1 of the year. 
-Most Butcher and Furniture sales happen online; however, most beverage sales occur in person, suggesting a casual pickup-and-go transaction or a lack of online options.


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

## CAVEATS AND ASSUMPTIONS:
-Discounts need better recording. Some were missing in store records. Though the numbers were minimal and the impact negligible, it's still better to just have those completed. This is for the sales and finance team to take note of.
-For future reference, please keep a detailed record of the products sold in each category. It would make it easier to pinpoint which product within a category caused the spike in revenue and sales.


---

## Screenshots

### Retail Sales Performance.
![Overview](<img width="1277" height="716" alt="PAGE 1-Retail Sales Peformance" src="https://github.com/user-attachments/assets/cd8e2dae-ff9f-45c0-aed0-665f91446a77" />)


### Sales Analysis.
![Analysis](<img width="1290" height="724" alt="PAGE 2- Sales Analysis" src="https://github.com/user-attachments/assets/925e7d3d-21e3-4454-8007-c9e8b6baafc1" />)


### Discount and Behaviour.
![Discounts](<img width="1290" height="730" alt="PAGE 3-Discount and Behaviour" src="https://github.com/user-attachments/assets/b215dd96-de28-4be5-9d70-8e250f06e93a" />)

### Revenue Spikes.
![Revenue](<img width="1290" height="725" alt="PAGE 4-Revenue Spikes" src="https://github.com/user-attachments/assets/50d24ae9-5d87-449c-92b7-359a56d19c26" />)

---

## How to Use

1. Download the `.pbix` file  
2. Open with Power BI Desktop  
3. Refresh data from processed CSVs  
4. Explore using slicers and filters
