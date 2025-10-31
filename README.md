🛒 Customer Shopping Behavior Analysis – Retail Insights

Analyzing customer purchase patterns, loyalty, and profitability to drive data-driven marketing and sales strategies using Python, SQL, and Power BI.

📌 Table of Contents

<a href="#overview">Overview</a>

<a href="#business-problem">Business Problem</a>

<a href="#dataset">Dataset</a>

<a href="#tools--technologies">Tools & Technologies</a>

<a href="#project-structure">Project Structure</a>

<a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>

<a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a>

<a href="#sql-analysis">SQL Analysis</a>

<a href="#dashboard">Dashboard</a>

<a href="#how-to-run-this-project">How to Run This Project</a>

<a href="#business-insights--recommendations">Business Insights & Recommendations</a>

<a href="#author--contact">Author & Contact</a>

<h2><a class="anchor" id="overview"></a>Overview</h2>

This project explores consumer shopping behavior using transactional data from a retail company.
The analysis identifies key factors influencing sales, loyalty, and repeat purchases — helping the company design better marketing, pricing, and retention strategies.
It integrates Python (EDA + cleaning), SQL (data analysis), and Power BI (dashboard) for end-to-end insight generation.

<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

Retail management has noticed shifting purchasing trends across demographics and channels.
The core business challenge is:

“How can we leverage customer data to identify trends, improve engagement, and optimize product and marketing strategies?”

This project focuses on:

Understanding spending patterns and loyalty behavior

Analyzing the impact of discounts and subscriptions

Identifying high-value customer segments

Evaluating top-performing products and channels

<h2><a class="anchor" id="dataset"></a>Dataset</h2>

Source: Customer transaction records (3,900 purchases)

Rows: 3,900

Columns: 18

Key Attributes:

Demographics: age, gender, location, subscription_status

Purchase Data: item_purchased, category, purchase_amount, season, size, color

Behavior: discount_applied, promo_code_used, previous_purchases, review_rating, shipping_type

Missing Data: 37 null values in review_rating handled via median imputation

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

Python: Pandas, NumPy, Matplotlib, Seaborn

SQL: PostgreSQL / MySQL / SQL Server

Visualization: Power BI

Presentation: Gamma App

Documentation: Jupyter Notebook, Markdown

<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>
customer-shopping-behavior-analysis/
│
├── README.md
├── .gitignore
├── requirements.txt
│
├── notebooks/
│   └── Customer_Shopping_Behavior_Analysis.ipynb
│
├── sql_scripts/
│   └── business_queries.sql
│
├── dashboard/
│   └── customer_behavior_dashboard.pbix
│
├── report/
│   ├── Customer_Shopping_Behavior_Analysis.pdf
│   └── Business Problem Document.pdf
│
├── presentation/
│   └── Customer_Behavior_Insights.pptx

<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

Loaded dataset using pandas

Checked structure with df.info() and summary with df.describe()

Renamed columns to snake_case for readability

Imputed missing values in review_rating using median per category

Created new features:

age_group (binned ages)

purchase_frequency_days (time between purchases)

Dropped redundant columns (promo_code_used)

Verified data consistency before exporting to SQL

<h2><a class="anchor" id="exploratory-data-analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

Key Observations:

Average Purchase Amount: ₹3,000–₹5,000 range

Majority purchases from female customers aged 25–35

Subscribed users have 25% higher purchase frequency

Positive correlation between discount_applied and purchase volume

Express shipping linked to higher-value transactions

Visuals Generated:

Category-wise revenue distribution

Gender vs. purchase amount

Review ratings vs. discount usage

Heatmap of feature correlations

<h2><a class="anchor" id="sql-analysis"></a>SQL Analysis</h2>

Performed using PostgreSQL to derive structured business insights:

Query	Objective
Revenue by Gender	Compare male vs. female contribution
High-Spending Discount Users	Identify customers spending above average despite discounts
Top 5 Products by Rating	Highlight products with best customer feedback
Shipping Type Analysis	Compare average purchase by shipping mode
Subscription Analysis	Compare spend between subscribers and non-subscribers
Discount-Dependent Products	Find items most influenced by discounts
Customer Segmentation	Classify into New, Returning, and Loyal segments
Age Group Revenue	Measure total contribution by age bucket
<h2><a class="anchor" id="dashboard"></a>Dashboard</h2>

Built in Power BI to visualize:

Customer segmentation & retention trends

Sales by demographics, category, and season

Discount impact on revenue

Product ratings and shipping insights

<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

Clone the Repository

git clone https://github.com/arnabkar07/customer-shopping-behavior.git
cd customer-shopping-behavior


Install Dependencies

pip install -r requirements.txt


Run the Jupyter Notebook

jupyter notebook notebooks/Customer_Shopping_Behavior_Analysis.ipynb


Connect to SQL Database

Create a PostgreSQL/MySQL DB

Run SQL scripts from /sql_scripts/

Update credentials in notebook before execution

View Dashboard

Open Power BI file: dashboard/customer_behavior_dashboard.pbix

Refresh dataset connection

View Final Report

Open PDF or Gamma presentation in /report/

<h2><a class="anchor" id="business-insights--recommendations"></a>Business Insights & Recommendations</h2>

Boost Subscriptions: Subscribers spend 25–30% more — incentivize sign-ups.

Loyalty Programs: Reward repeat buyers to increase retention.

Discount Optimization: Balance volume growth and profit margins.

Product Positioning: Focus marketing on top-rated and top-selling categories.

Target Marketing: Prioritize high-revenue demographics (25–35 age group).

<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

Arnab Kar
📧 Email: arnabk734@gmail.com

🔗 LinkedIn

