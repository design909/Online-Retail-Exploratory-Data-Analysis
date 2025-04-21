# Online Retail Exploratory Data Analysis with Python

> 📊 **Presentation Available**: [View EDA Summary Slides (Canva)](https://www.canva.com/design/DAGlO5r_JU8/sIUWNNKbRfKGnFoJ_S-SyQ/edit?utm_content=DAGlO5r_JU8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

Welcome to my portfolio project where I performed Exploratory Data Analysis (EDA) on a real-world online retail dataset using Python. The goal of this project was to uncover key business insights, identify customer behavior patterns, and provide actionable recommendations for decision-making.

## Overview

This project simulates the role of a data analyst in an online retail company. I worked with transactional data from an e-commerce store spanning 2010 to 2011. The dataset includes invoice details, product descriptions, quantities, pricing, timestamps, and customer information across various countries.

Through data cleaning, exploration, visualization, and basic statistical analysis, I answered business-relevant questions such as:

- What are the busiest months and days for sales?
- Which products and countries generate the most revenue?
- What patterns exist in product returns?
- Are there any data quality issues or outliers?

## Dataset

The dataset was sourced from the UCI Machine Learning Repository:  
**[Online Retail Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx)**

It contains 541,909 rows and 8 features:
- `InvoiceNo`
- `StockCode`
- `Description`
- `Quantity`
- `InvoiceDate`
- `UnitPrice`
- `CustomerID`
- `Country`

## Key Steps and Highlights

### 1. Data Cleaning
- Removed 5,268 duplicate rows
- Dropped records with missing `CustomerID` or `Description`
- Cleaned dataset has 401,604 valid transactions
- Handled zero unit prices and negative quantities (returns)

### 2. Descriptive Statistics
- Identified skewness in `Quantity` and `UnitPrice` due to extreme outliers
- Median values were more representative of typical transactions

### 3. Data Visualization
- Histograms and boxplots to analyze distributions
- Line and bar charts for time-series trends
- Bar plots for top-selling products and countries
- Return analysis via most frequently returned items

### 4. Time-Based Analysis
- **Peak Sales:** Q4, especially November
- **Low Sales Periods:** February and April
- **Missing Saturday Data:** Possibly a logging or operational issue

### 5. Top Performers
- **Best-Selling Product:** `PAPER CRAFT , LITTLE BIRDIE` (80,995 units)
- **Top Countries (Excl. UK):** Netherlands, Ireland (EIRE), Germany, France

### 6. Outliers and Anomalies
- Found significant outliers in quantities (up to 80,000) and prices (up to £38,970)
- Discussed their impact on average statistics and visualizations

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Insights & Recommendations

- **Maximize Q4 Opportunities:** Optimize marketing/inventory ahead of peak season
- **Investigate Data Gaps:** Missing Saturdays should be explored further
- **Analyze High Return Items:** Monitor customer feedback and product quality
- **Enhance Data Integrity:** Apply better validation on quantity and pricing fields
- **Capitalize on International Markets:** Focus on strong-performing regions like the Netherlands and Germany

## How to Run

Clone this repository and run the notebook:

```bash
git clone https://github.com/yourusername/online-retail-eda-python.git
cd online-retail-eda-python
pip install -r requirements.txt
jupyter notebook notebooks/online_retail_eda.ipynb
