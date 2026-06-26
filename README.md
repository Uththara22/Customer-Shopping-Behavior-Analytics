<div align="center">

# 🛒 Customer Shopping Behavior Analytics

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

### 📊 End-to-End Customer Behavior Analytics Project

Transforming transactional data into actionable business insights using Python, PostgreSQL, and Power BI.

</div>

---

## 📖 Project Overview

Customer shopping behavior analytics using Python, PostgreSQL, and Power BI to uncover spending patterns, customer segments, and business insights. Using transactional data from **3,900 purchases** across multiple product categories, the objective is to establish a fully scaled analytics pipeline—handling raw data conditioning, relational database querying, and deploying an interactive dashboard to uncover spending patterns, subscription insights, and purchasing trends.

---

## 🎯 Skills Demonstrated

* 📊 **Exploratory Data Analysis (EDA)** — Data Profiling and Descriptive Statistics via Pandas

* 🧹 **Advanced Data Cleansing** — Handling Missing Values through Category-Wise Median Imputation

* 🏗️ **Feature Engineering** — Generating Custom Age Groups and Numerical Purchase Frequencies

* 🗄️ **Database Integration & SQL Analytics** — Connecting Pipelines to PostgreSQL and Structuring Advanced Subqueries & Window Functions

* 👥 **Advanced Customer Segmentation** — Behavioral Grouping into New, Returning, and Loyal Segments

* 📈 **Business Intelligence & Reporting** — Designing Interactive Dashboards, Button Slicers, and Dynamic KPI Displays

---

## 📊 Dataset Information

| Metric | Value |
|---------|---------|
| 📄 Total Records | 3,900 |
| 📋 Total Features | 18 |
| ⭐ Missing Values | 37 (Review Rating) |

### 🔑 Key Features

#### 👤 Customer Demographics
- Age
- Gender
- Location
- Subscription Status

#### 🛍️ Purchase Information
- Item Purchased
- Category
- Purchase Amount
- Season
- Size
- Color

#### 📈 Shopping Behavior
- Discount Applied
- Previous Purchases
- Purchase Frequency
- Review Rating
- Shipping Type

---

## 🧹 Data Preprocessing & Cleaning

### ✅ Data Exploration
- Loaded dataset using Pandas in Jupyter Notebook
- Inspected data structure and quality using `info()` and `describe(include='all')`

### 🔧 Missing Value Handling
- Identified 37 missing values in the Review Rating column
- Imputed missing values using the median review rating within each specific product category to prevent bias

### 🏗️ Feature Engineering
- Created categorical customer age groups (Young Adult, Adult, Middle-Aged, Senior) using `pd.qcut()`
- Converted textual purchase frequencies (e.g., Weekly, Monthly) into numerical days metrics via a dictionary mapping function

### 📋 Data Standardization
- Standardized all column headers into consistent `snake_case` layout for easier referencing
- Removed the redundant `promo_code_used` column after verifying it contained identical values to `discount_applied`

### 🗄️ Database Integration
- Connected Jupyter Notebook directly to the PostgreSQL database (pgAdmin)
- Successfully loaded the cleaned data frame into a production database table named `customer`

---

## 🔍 Business Analysis Using SQL

### 💰 Revenue Analysis
- **Revenue by Gender:** Evaluating total purchase weight split by demographic gender profiles
- **Revenue by Age Group:** Aggregating transactional volume against custom engineered age brackets

### 👥 Customer Analysis
- **Customer Loyalty Segmentation:** Utilizing SQL `CASE WHEN` statements to partition baseline records into New, Returning, and Loyal segments based on historical counts
- **Subscribers vs Non-Subscribers:** Comparing behavioral metrics, volume profiles, and gross contributions across subscriber segments
- **Repeat Buyers & Subscription Trends:** Investigating the subscription conversion velocity among repeat purchasers

### 🛒 Product Analysis
- **Top 5 Highest Rated Products:** Finding best-selling merchandise across categories with peak average scores
- **Top 3 Products per Category:** Executing advanced SQL Window Functions (`ROW_NUMBER() OVER(PARTITION BY...)`) to extract category leaders
- **Discount-Dependent Products:** Identifying specific items that rely heavily on promotional discounts to drive unit velocity

### 🚚 Shopping Behavior Analysis
- **Shipping Type Comparison:** Reviewing purchase amounts between Standard and Express delivery modes
- **High-Spending Discount Users:** Auditing transactions where consumers applied a discount but still spent above the baseline statistical average

---

## 📊 Power BI Dashboard

Built an interactive, fully integrated Power BI dashboard connected directly to PostgreSQL to visualize:

- 📈 **Revenue Trends:** Tracking performance vectors and financial outcomes
- 👥 **Customer Segmentation:** Providing clear interactive visual breakdowns of customer clusters
- 🛍️ **Product Performance:** Mapping category movements, orders, and product yields
- 💳 **Subscription Insights:** Visualizing customer status percentages using optimized donut charts
- 🚚 **Shipping Preferences & Dynamic KPIs:** Deploying advanced card visual architecture, accent bars, and button slicers for immediate evaluation cross-filtering

---

## 💡 Key Business Recommendations

* 🚀 **Increase Subscription Adoption:** Provide exclusive offers and benefits to encourage more customer subscriptions.
* 🎁 **Strengthen Customer Loyalty:** Reward repeat customers through loyalty programs and personalized incentives.
* 💵 **Optimize Discount Strategies:** Balance discount campaigns with profitability objectives, focusing on discount-dependent products.
* ⭐ **Promote Top-Performing Products:** Feature best-selling and highest-rated products in marketing efforts.
* 🎯 **Target Marketing Campaigns:** Focus on high-value customer segments and revenue-generating age groups.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|----------|
| 🐍 Python | Data Cleaning & Analysis |
| 🐼 Pandas | Data Manipulation & Wrangling |
| 🐘 PostgreSQL | SQL Production Analytics |
| 📊 Power BI | Dashboard Development & BI Reporting |