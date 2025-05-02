# Sales-trend-analysis-using-aggregations-
# Summary of findings
# objective:
sales trend analysis using aggregations on online sales dataset.

# Dataset Used:
sales_data.csv from kaggle (uploded in zip file above) 
#  Tools: MySQL 

# Steps with queries & output:
Created database sales_data 
imported dataset of sales_data.csv in table sales_ data.
# 1).Each row shows:
•The month (e.g., '2023-01-01'),
•The total revenue generated in that month,
•The total quantity of items sold in that month.
•Helps identify trends in sales and volume over time:
•Which months had highest/lowest revenue,
•Which months had highest/lowest units sold.
![1000012854](https://github.com/user-attachments/assets/c503dc62-9afd-47c3-be62-f002dc271430)

# 2).Groups data by Region.
Calculates:
•Total_Sales: total revenue per region.
•Num_Sales_Reps: number of unique sales representatives in each region.

•Orders results by Total_Sales in descending order, so the region with the highest sales appears first.
![1000012851](https://github.com/user-attachments/assets/574d2a41-8499-4cf4-8131-32b2bc249db4)

# 3).total sales and number of unique sales reps per region.
It helps identify which regions are generating the most revenue and how many sales reps are active in each. Results are sorted from highest to lowest total sales.
![1000012863](https://github.com/user-attachments/assets/5afd69df-48f8-4e48-a78b-adba1aa634bd)

# 4).total sales and units sold per product category.
It highlights which categories generate the most revenue and sales volume, with results sorted from highest to lowest total sales—useful for identifying top-performing product lines.
![1000012886](https://github.com/user-attachments/assets/ddaad51b-5de4-40df-871f-b118df1a51a8)
# 5).Shows total sales and number of transactions for each customer type (e.g., new vs. returning).

Helps identify which customer type brings more revenue.
![1000012892](https://github.com/user-attachments/assets/8675a672-fb02-4e01-bacd-393cd08c954f)

# 6).total sales by each payment method and sales channel combo.

Useful for understanding which sales channels and payment types are most profitable.
![1000012893](https://github.com/user-attachments/assets/6d021540-efc0-4939-94e6-ffaf70c89d53)
# 7).monthly revenue and product sales volume for the year 2023.

Tracks trends across months to highlight seasonal peaks.
![1000012894](https://github.com/user-attachments/assets/f4dd534a-f372-41fb-bcf7-d59d1cc4bbd9)

# 8).Monthly Total Sales
•Shows total sales per month (across all years).
•Identifies which months perform best in terms of revenue.
![1000012895](https://github.com/user-attachments/assets/5f7be15e-11f5-4a08-8c61-1b6738cbf5dd)

# 9).Year-Month Sales Summary
•Shows total monthly sales grouped by both year and month.
•Useful for analyzing sales patterns over multiple years.
![1000012896](https://github.com/user-attachments/assets/83608ec3-e686-45e8-9875-fe2ef9306657)

# 10).All Sales Data Ordered by Date
SELECT * FROM sales_data ORDER BY sale_date;
Lists all transactions chronologically.
Useful for reviewing or auditing the raw sales data timeline.
![1000012897](https://github.com/user-attachments/assets/f19a2dc1-08cd-4dfb-b716-82be3593109f)

# 11).Monthly sales summary, grouped by year and month. It shows:

Rev: Total revenue for each month.

Vol: Total number of unique products sold in that month.
![1000012900](https://github.com/user-attachments/assets/a34b2d14-9703-42f6-bfbc-2187f8a6ac5e)

# 12).performance of each sales representative by region, including:
•Total_Sales: Revenue generated.
•Total_Units_Sold: Quantity of products sold.
![1000012903](https://github.com/user-attachments/assets/b64f8ead-d15f-4a8b-bdb7-c7709f097c77)

