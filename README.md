# customer_behavior
🛍️ Customer Shopping Behavior Analysis
📄 Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The goal is to uncover insights into spending patterns, customer segmentation, product preferences, and subscription trends to support strategic business decisions.
📊 Dataset Summary
Rows: 3,900
Columns: 18
Key Features:
Customer demographics – Age, Gender, Location, Subscription Status
Purchase details – Item Purchased, Category, Purchase Amount, Season, Size, Color
Shopping behavior – Discount Applied, Promo Code Used, Previous Purchases, Frequency, Review Rating, Shipping Type
Missing Data: 37 missing values in the Review Rating column
🧠 Exploratory Data Analysis (Python)
Performed using pandas, numpy, matplotlib, and seaborn.
Steps:
Data Loading: Imported the dataset into Python using pandas.
Initial Exploration: Used .info() and .describe() for data structure and summary statistics.
Missing Data Handling: Imputed missing review ratings using the median rating per product category.
Column Standardization: Converted column names to snake_case format.
Feature Engineering:
Created age_group by binning customer ages.
Derived purchase_frequency_days from purchase timestamps.
Data Consistency Check: Compared discount_applied vs. promo_code_used and dropped redundant columns.
Database Integration: Loaded the cleaned DataFrame into PostgreSQL for SQL-based analysis.

🧮 SQL Analysis (PostgreSQL)

Key business queries and insights include:

Revenue by Gender – Compared total sales by male vs. female customers.

High-Spending Discount Users – Found customers who used discounts but spent above-average amounts.

Top 5 Products by Rating – Identified highest-rated items.

Shipping Type Comparison – Compared spend between Standard and Express shipping.

Subscribers vs. Non-Subscribers – Analyzed revenue and average spend across subscription groups.

Discount-Dependent Products – Highlighted products most often sold with discounts.

Customer Segmentation – Grouped customers as New, Returning, or Loyal.

Top 3 Products per Category – Listed most popular products within each category.

Repeat Buyers & Subscriptions – Tested if frequent buyers are more likely to subscribe.

Revenue by Age Group – Compared contributions by different age segments.

📈 Dashboard (Power BI)

An interactive Power BI dashboard was created to visualize:

Sales and revenue by gender, category, and region

Discount usage and customer segmentation

Ratings, top products, and subscription-based spending

KPI cards and dynamic filters for decision-making

💡 Business Recommendations

Boost Subscriptions: Market exclusive benefits to attract more subscribers.

Loyalty Programs: Reward repeat buyers to enhance retention.

Review Discount Policy: Optimize discount strategy for balanced margins.

Product Positioning: Highlight top-rated and best-selling items.

Targeted Marketing: Focus on high-value demographics and express-shipping users.

🧰 Tools & Technologies
Category	Tools Used
Programming	Python (pandas, numpy, matplotlib, seaborn)
Database	PostgreSQL
Visualization	Power BI
Presentation	Gamma / PowerPoint
🚀 How to Run

Clone this repository or download the .pbix and .ipynb files.

Install dependencies:

pip install pandas numpy matplotlib seaborn psycopg2


Load the dataset and run the Python script for cleaning and EDA.

Execute SQL queries in PostgreSQL to reproduce insights.

Open the Power BI dashboard to explore visual analytics.

🏁 Results Summary

Women generated higher average purchase amounts.

Discounts significantly impacted sales volume.

Loyal customers had the highest lifetime value.

Express shipping correlated with higher order values.ations.
