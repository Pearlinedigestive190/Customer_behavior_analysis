🛍️ Customer Shopping Behavior Analysis
📄 Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide data-driven business decisions.

🧰 Tools & Technologies Used
Category	Tools
Data Analysis	Python (Pandas, NumPy, Matplotlib, Seaborn)
Database & SQL	MySQL (Data storage, queries, joins, aggregation)
Business Intelligence	Power BI (Interactive dashboards, KPIs, visuals)
Version Control	Git & GitHub
Data Cleaning & Transformation	Power Query, Python
📊 Dataset Summary

Total Rows: 3,900

Total Columns: 18

Key Features:

Customer Demographics: Age, Gender, Location, Subscription Status

Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color

Shopping Behavior: Discount Applied, Promo Code Used, Frequency of Purchases, Review Rating, Shipping Type

🧮 Data Analysis Workflow
1. Data Preparation (Python)

Imported dataset using pandas

Checked structure and summary statistics using df.info() and df.describe()

Handled missing data (37 nulls in review_rating) using median imputation per category

Standardized column names to snake_case for readability

Feature Engineering:

age_group — binned customer ages

purchase_frequency_days — calculated from purchase history

Dropped redundant columns (promo_code_used)

Loaded cleaned data into MySQL for SQL-based analysis

2. SQL Business Analysis

Performed structured SQL queries to uncover business insights:

Analysis	Description
Revenue by Gender	Compared total revenue from male vs. female customers
Top 5 Products by Rating	Found products with the highest average review ratings
Subscribers vs Non-Subscribers	Compared average spend and total revenue
Shipping Type Comparison	Analyzed purchase amounts between Standard vs Express
Customer Segmentation	Classified customers into New, Returning, and Loyal
Discount-Dependent Products	Identified products often bought with discounts
Top 3 Products per Category	Highlighted top-selling products by category
Repeat Buyers & Subscriptions	Examined subscription likelihood among repeat buyers
3. Dashboard in Power BI

An interactive dashboard was created to visualize:

Total Revenue by Age Group

Gender-based Spending Patterns

Subscription Impact on Revenue

Product Ratings and Discount Analysis

Customer Loyalty Segments

Dashboard Components:

Slicers for Category, Age Group, and Subscription Status

Dynamic Charts (Bar, Pie, Donut, and KPI Cards)

DAX Measures for Revenue, Average Rating, and Discount Usage

💡 Key Insights

High-Spending Discount Users: Customers using discounts still spent above average.

Subscribers: Generate higher lifetime revenue than non-subscribers.

Express Shipping: Linked to higher average purchase amounts.

Top Age Group: Middle-aged customers (30–45) contribute the most to total revenue.

Product Ratings: Correlate positively with repeat purchase rates.

🧭 Business Recommendations

Boost Subscriptions – Promote exclusive perks for subscribers.

Targeted Marketing – Focus campaigns on high-revenue age groups.

Product Positioning – Highlight top-rated and best-selling products.

Customer Loyalty Programs – Reward repeat buyers to encourage loyalty.

Review Discount Policy – Balance sales boosts with profit margins.

📂 Project Structure
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── customer_shopping_data.csv
├── scripts/
│   ├── data_cleaning.ipynb
│   ├── sql_queries.sql
│   └── visualization.pbix
├── README.md
└── requirements.txt

🧠 Learning Outcomes

Data Cleaning & Feature Engineering in Python

SQL Querying for Business Insights

Dashboard Design in Power BI

End-to-End Data Pipeline: Python → MySQL → Power BI

🚀 How to Run This Project

Clone the repository

git clone https://github.com/yourusername/Customer-Shopping-Behavior-Analysis.git
cd Customer-Shopping-Behavior-Analysis


Install dependencies

pip install -r requirements.txt


Run the analysis notebook

jupyter notebook scripts/data_cleaning.ipynb


Import cleaned data to MySQL

Open visualization.pbix in Power BI Desktop to view the dashboard

🧾 Author

[Your Name]
📧 your.email@example.com

📊 Data Analyst | Python | SQL | Power BI | BI Storytelling
