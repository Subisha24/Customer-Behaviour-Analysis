# Customer-Behaviour-Analysis
Project showcased customer behaviour analysis using Python, MySQL, and Power BI.
### 1. Project Overview
This project analyses customer shopping behaviour using transactional data from 3,900 purchases across multiple product categories. 

The goal is to understand:

  •	Who the key customer segments are
  
  •	How discounts, shipping type, and subscriptions affect revenue
  
  •	Which products and categories perform best
  
  •	How customer behaviour translates into actionable business recommendations 

The end-to-end workflow covers Python-based EDA and cleaning, SQL analysis in MySQL, a Power BI dashboard, a written report, and a presentation created using Gamma.

### 2. Dataset

•	Rows: 3,900

•	Columns: 18

•	Type: Transaction-level shopping data

**Key Features**

•	Customer demographics: Age, Gender, Location, Subscription Status

•	Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, Colour

•	Behavioural fields: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

•	Missing data: 37 missing values in the Review Rating field 

Note: This is an anonymised dataset created for analytics and portfolio purposes.

### 3.  Tech Stack & Tools

• **Python (Pandas)**: Data extraction, cleaning, imputation, and feature engineering.

•	**MySQL Workbench**: Database management and structured data analysis (SQL).

•	**Power BI**: Interactive dashboard creation for visual storytelling.

•	**Gamma**: Creation of the final presentation deck.

### 4. Project Steps

**4.1 Data Loading & Initial EDA (Python)**

•	Load CSV dataset using pandas

•	Inspect structure using .info() and .describe()

•	Explore distributions and relationships (age, purchase amount, ratings, etc.) with plots 

**4.2 Data Cleaning & Feature Engineering**

•	Handle missing values in review_rating by imputing median ratings per product category

•	Standardise column names to snake_case

•	Create new features:

       o	age_group (binned age ranges)
   
       o	purchase_frequency_days (derived from purchase dates)

•	Validate and remove redundant fields (e.g., promo_code_used after checking overlap with discount_applied) 

**4.3 Loading Data into MySQL**

•	Create a database and table schema in MySQL

•	Use Python (SQLAlchemy / mysql-connector) to push the cleaned DataFrame into MySQL

•	Validate row and column counts between Python and MySQL

**4.4 Business Analysis in SQL**

Key analyses performed in MySQL Workbench include: 

1.	Revenue by gender

2.	High-spending discount users (discount applied but above-average purchase amount)

3.	Top 5 products by rating

4.	Shipping type analysis (Standard vs Express average spend)

5.	Subscribers vs non-subscribers (avg spend & total revenue)

6.	Discount-dependent products

7.	Customer segmentation (New, Returning, Loyal)

8.	Top 3 products per category

9.	Repeat buyers & subscription uptake

10.	Revenue by age group

**4.5 Power BI Dashboard**

•	Connect Power BI to the cleaned dataset (or MySQL view)

•	Create interactive visuals:

o	KPIs: number of customers, average purchase amount, average review rating

o	Revenue by category and age group

o	Sales by category

o	% customers by subscription status

o	Filters for subscription status, gender, category, and shipping type 

**4.6 Report & Recommendations**

•	Summarise insights from Python, SQL, and Power BI

•	Convert findings into business recommendations (e.g., boosting subscriptions, loyalty programs, discount strategy, targeted marketing) 

**4.7 Gamma Presentation**

•	Import key charts and numbers from Power BI/report

•	Build a structured PPT-style deck in Gamma, including:

     o	Problem statement & objectives

     o	Methodology (Python → SQL → Power BI)

     o	Key insights & charts

     o	Business recommendations & next steps

### 5. Dashboard Highlights

The Customer Behaviour Dashboard in Power BI includes: 

**•	KPIs:**

o	3.9K customers

o	~$59.76 average purchase amount

o	~3.75 average review rating

**•	Visuals:**

o	Revenue and sales by category

o	Revenue and sales by age group

o	Subscription share (% of customers who are subscribers vs non-subscribers)

o	Slicers for gender, subscription status, category, and shipping type

This allows stakeholders to explore how different customer segments and behaviours drive revenue quickly.

### 6. Results & Key Insights

Some example findings from the analysis:

•	Certain **age groups contribute more revenue**, making them a priority for targeted campaigns.

•	**Subscribers** generally have higher engagement and revenue potential than non-subscribers.

•	A subset of customers **uses discounts but still spends above average**, showing an opportunity to design smarter promotions.

•	**Top-rated and best-selling products** can be highlighted in marketing to increase conversion.

•	Customers opting for **Express shipping** may represent a more time-sensitive and higher-value segment.

These insights feed into recommendations on subscriptions, loyalty programs, discount policies, product positioning, and targeted marketing.
________________________________________


________________________________________


________________________________________

