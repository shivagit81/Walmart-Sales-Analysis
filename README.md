# Walmart-Sales-Analysis
This SQL-driven Walmart data analysis project focuses on identifying top-performing branches and products while optimizing sales strategies using data from Kaggle's Walmart Sales Forecasting Competition.

# Walmart-Sales-Data-Analysis--SQL-Project  

## About  
This project aims to analyze Walmart’s sales data to identify top-performing branches and products, uncover sales patterns, and understand customer behavior. The ultimate goal is to optimize sales strategies and improve overall business performance. The dataset used for this project is sourced from the **Kaggle Walmart Sales Forecasting Competition**.  

## Purposes of the Project  
The primary objective is to extract meaningful insights from Walmart’s sales data, investigating various factors influencing sales across different branches.  

## About Data  
The dataset, obtained from the **Kaggle Walmart Sales Forecasting Competition**, consists of sales transactions from **three Walmart branches** located in **Mandalay, Yangon, and Naypyitaw**.  
It comprises **17 columns and 1000 rows**, detailing invoices, store locations, customer demographics, sales figures, taxes, and ratings.  

| Column            | Description                                    | Data Type        |  
|-------------------|----------------------------------------------|------------------|  
| invoice_id        | Unique identifier for each sale               | VARCHAR(30)      |  
| branch           | Store branch where the transaction occurred    | VARCHAR(5)       |  
| city             | Location of the branch                        | VARCHAR(30)      |  
| customer_type    | Category of customer                         | VARCHAR(30)      |  
| gender           | Gender of the customer                       | VARCHAR(10)      |  
| product_line     | Product category                              | VARCHAR(100)     |  
| unit_price       | Price per unit                                | DECIMAL(10, 2)   |  
| quantity        | Number of items purchased                     | INT              |  
| VAT              | Tax amount on the transaction                 | FLOAT(6, 4)      |  
| total            | Total cost of purchase                        | DECIMAL(12, 4)   |  
| date             | Date of transaction                          | DATETIME         |  
| time             | Time of transaction                          | TIME             |  
| payment         | Payment amount                                | DECIMAL(10, 2)   |  
| cogs             | Cost of Goods Sold (COGS)                     | DECIMAL(10, 2)   |  
| gross_margin_pct | Gross margin percentage                      | FLOAT(11, 9)     |  
| gross_income     | Profit generated                              | DECIMAL(12, 4)   |  
| rating          | Customer rating                               | FLOAT(2, 1)      |  

## Analysis List  

### 1. Product Analysis  
> Investigating different product lines to identify best-sellers and areas for improvement.  

### 2. Sales Analysis  
> Evaluating sales trends and assessing the effectiveness of various sales strategies.  

### 3. Customer Analysis  
> Analyzing customer segments, purchasing patterns, and revenue contributions from different customer groups.  

## Approach Used  

### **1. Data Wrangling**  
In this phase, the dataset is assessed for missing values, and necessary data-cleaning techniques are applied.  
- Create a structured database and import the dataset.  
- Ensure all fields have `NOT NULL` constraints to prevent missing values.  

### **2. Feature Engineering**  
New columns are generated to enhance data analysis and uncover trends.  
- **`time_of_day`**: Categorizes transactions into **Morning, Afternoon, and Evening** to determine peak sales periods.  
- **`day_name`**: Extracts the day of the week (**Mon, Tue, Wed, Thu, Fri**) to identify the busiest days.  
- **`month_name`**: Extracts the month (**Jan, Feb, Mar**) to track revenue and profit trends over time.  

### **3. Exploratory Data Analysis (EDA)**  
EDA is conducted to generate insights, answer business-related questions, and uncover sales trends.  

## Business Questions to Answer  

### **Generic Questions**  
1. How many unique cities are represented in the dataset?  
2. Which city corresponds to each branch?  

### **Product Analysis**  
1. How many distinct product lines exist?  
2. What is the most frequently used payment method?  
3. Which product line has the highest sales volume?  
4. What is the total revenue per month?  
5. Which month recorded the highest **Cost of Goods Sold (COGS)**?  
6. Which product line generates the most revenue?  
7. Which city produces the highest revenue?  
8. Which product line incurs the highest VAT?  
9. Categorize product lines as **"Good"** or **"Bad"** based on sales performance.  
10. Identify branches that sell more than the average product volume.  
11. Which product line is most popular among different genders?  
12. What is the average rating for each product line?  

### **Sales Analysis**  
1. How do sales vary at different times of the day throughout the week?  
2. Which customer type contributes the most to revenue?  
3. Which city has the highest **VAT (Value Added Tax) percentage**?  
4. Which customer type pays the most VAT?  

### **Customer Analysis**  
1. How many unique customer categories are there?  
2. How many distinct payment methods are available?  
3. What is the most common customer type?  
4. Which customer type makes the most purchases?  
5. What is the gender distribution of customers?  
6. How does gender distribution vary by branch?  
7. What time of day receives the most customer ratings?  
8. How do ratings vary by time of day across different branches?  
9. Which weekday receives the highest average ratings?  
10. What is the highest-rated day for each branch?  

This project utilizes **SQL-based data analysis** to extract key insights, enabling **data-driven decision-making** to enhance Walmart’s sales and customer satisfaction. 🚀  

What is the gender distribution of customers?
How does gender distribution vary across branches?
What time of day receives the most customer ratings?
Identify the time of day with the highest ratings per branch.
Which weekday has the best average customer ratings?
Determine the best-rated day for each branch.
This project applies structured SQL queries to extract insights, enabling data-driven decisions to improve Walmart's sales performance and customer satisfaction.
