# Online Retail Exploratory Data Analysis with Python

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
- Dropped records with missing `CustomerID` or `Description` (over 135,000 rows)
- Created a clean dataset of 401,604 rows
- Handled zero unit prices and negative quantities (returns)

### 2. Descriptive Statistics
- Identified skewness in `Quantity` and `UnitPrice` due to extreme outliers
- Highlighted the need for median-based metrics for typical transaction analysis

### 3. Data Visualization
- Histograms, boxplots, and bar charts to analyze:
  - Quantity and price distributions
  - Monthly and weekday sales trends
  - Top-selling products and countries
  - Most returned products

### 4. Time-Based Analysis
- **Peak Sales:** Observed in Q4 (especially November)
- **Slow Months:** February and April
- **No Saturday Data:** Likely due to data collection issue or business operations

### 5. Top Performers
- **Best-Selling Product:** `PAPER CRAFT , LITTLE BIRDIE` (80,995 units)
- **Top Countries (excluding UK):** Netherlands, Ireland (EIRE), Germany, France

### 6. Outliers and Anomalies
- Found outliers with quantities over 80,000 and prices up to £38,970
- Discussed their potential impact on mean, visualizations, and business interpretations

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Insights & Recommendations

- **Maximize Q4 Opportunities:** Invest more in marketing and inventory ahead of holiday season
- **Improve Data Logging:** Investigate missing Saturday sales data
- **Monitor High-Return Products:** Assess quality issues with frequently returned items
- **Refine Data Cleaning Practices:** For more reliable metrics and reporting

## How to Run

Clone this repository and run the notebook:

```bash
git clone https://github.com/yourusername/online-retail-eda-python.git
cd online-retail-eda-python
pip install -r requirements.txt
jupyter notebook notebooks/online_retail_eda.ipynb
