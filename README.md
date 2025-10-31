🛍️ Customer Shopping Behavior Analysis
📘 Overview

This project analyzes customer shopping patterns to help a retail company improve sales, satisfaction, and loyalty. It combines Python (EDA & cleaning), SQL (query-based insights), and Power BI (visual storytelling) to identify what drives purchases, repeat customers, and overall revenue growth.

📊 Dataset

Source: Company’s transactional dataset

Records: 3,900 rows

Features: 18 columns covering demographics, purchase behavior, and sales data

Demographics: age, gender, location, subscription_status

Purchase info: item_purchased, category, purchase_amount, season, size, color

Behavioral: discount_applied, previous_purchases, review_rating, shipping_type

Missing Data: 37 null values in review_rating, handled using median imputation.

🧰 Tools & Technologies
Category	Tool / Technology
Programming	Python (Pandas, NumPy, Matplotlib, Seaborn)
Database	PostgreSQL / MySQL / SQL Server
Visualization	Power BI
Reporting	Gamma App
Documentation	Jupyter Notebook, Markdown, PDF, PPT
⚙️ Steps Followed
1. Data Loading & Exploration (Python)

Imported dataset with pandas

Checked structure with df.info() and df.describe()

Identified and handled missing values in review_rating

Renamed columns to snake_case for consistency

2. Data Cleaning & Feature Engineering

Created age_group bins from customer ages

Derived purchase_frequency_days to measure buying habits

Dropped redundant features like promo_code_used

Ensured data integrity before database upload

3. SQL Analysis (PostgreSQL/MySQL)

Performed advanced queries to extract actionable insights:

Revenue by gender, age group, and subscription status

High-spending discount users

Top products by review rating

Shipping type comparison (Standard vs. Express)

Loyalty segmentation: New, Returning, and Loyal customers

Discount dependency and product preference analysis

4. Dashboard (Power BI)

Built an interactive Power BI dashboard showing:

Total revenue by demographics & category

Purchase trends across seasons

Discount and subscription impact

Top 5 performing products

Customer segmentation visualizations

5. Report & Presentation (Gamma)

Created a structured report summarizing key insights, recommendations, and trends.

Designed a presentation deck in Gamma to communicate findings clearly to stakeholders.

📈 Key Insights & Recommendations

Promote Subscriptions: Subscribers spend more on average.

Loyalty Programs: Reward repeat buyers to drive retention.

Discount Strategy: Optimize discounts to protect profit margins.

Product Positioning: Highlight top-rated products in campaigns.

Targeted Marketing: Focus on high-value age groups and Express shipping users.

🚀 How to Run
1. Clone Repository
git clone https://github.com/arnabkar07/customer-shopping-behavior.git
cd customer-shopping-behavior

2. Run Python Notebook

Open the Jupyter Notebook:

jupyter notebook Customer_Shopping_Behavior_Analysis.ipynb

3. Configure SQL Database

Create a new database in PostgreSQL/MySQL/SQL Server

Run the SQL scripts in /sql_scripts folder

Update database credentials in the notebook before running SQL cells

4. View Power BI Dashboard

Open the .pbix file in Power BI Desktop

Refresh data connection to your local database

5. View Final Report

Open the Gamma link or PDF under /report

📂 Project Structure
├── data/
│   └── customer_shopping_behavior.csv
├── notebooks/
│   └── Customer_Shopping_Behavior_Analysis.ipynb
├── sql_scripts/
│   └── business_queries.sql
├── dashboard/
│   └── customer_behavior_dashboard.pbix
├── report/
│   └── Customer_Shopping_Behavior_Analysis.pdf
├── presentation/
│   └── Customer_Behavior_Insights.pptx
└── README.md
