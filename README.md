# End-to-End Retail Data Analytics

## 1. Project Overview

This project focuses on analysing real-world retail transaction data to understand sales performance, customer purchasing behaviour, product performance and business trends.

The project uses the UCI Online Retail dataset, which contains historical transactions from a UK-based online retail business.

Python is used to clean, process, analyse and visualize the dataset to extract meaningful business insights.

The main objective is to help businesses make better decisions regarding sales planning, customer retention, inventory management and overall business performance.

## 2. Problem Statement

Retail businesses generate large amounts of transaction data every day. However, understanding customer purchasing behaviour, identifying popular products, analysing sales trends and monitoring product returns can be challenging.

Without proper data analysis, businesses may face difficulties in inventory planning, customer retention and sales improvement.

This project aims to analyse retail transaction data using Python and Exploratory Data Analysis (EDA) to identify meaningful patterns and provide useful business insights.

## 3. Project Objectives

- To analyse real-world retail transaction data.
- To identify and handle missing values and duplicate records.
- To inspect invalid and inconsistent transaction values.
- To calculate total sales revenue, returns and net sales.
- To identify the top-selling products.
- To analyse customer purchasing behaviour.
- To identify the highest-revenue countries.
- To analyse monthly, daily and hourly sales trends.
- To create meaningful data visualizations.
- To generate business insights and recommendations.

## 4. Dataset Description

**Dataset Name:** Online Retail

**Source:** UCI Machine Learning Repository

**Dataset Link:** https://archive.ics.uci.edu/dataset/352/online+retail

The dataset contains historical transactions from an online retail business between December 2010 and December 2011.

### Dataset Features

| Column | Description |
|---|---|
| InvoiceNo | Unique invoice number for each transaction |
| StockCode | Product identification code |
| Description | Product description |
| Quantity | Number of products purchased |
| InvoiceDate | Date and time of transaction |
| UnitPrice | Price per unit |
| CustomerID | Unique customer identification number |
| Country | Customer's country |

**Original dataset shape:** 541,909 rows and 8 columns.

## 5. Technologies and Libraries Used

### Programming Language
- Python

### Libraries
- Pandas – Data manipulation and analysis.
- NumPy – Numerical operations.
- Matplotlib – Data visualization.
- Seaborn – Statistical data visualization.

### Development Environment
- Visual Studio Code
- Jupyter Notebook

## 6. Project Workflow

The project follows these major steps:

1. Dataset collection and loading.
2. Data inspection and understanding.
3. Data cleaning and preprocessing.
4. Exploratory Data Analysis (EDA).
5. Sales and revenue analysis.
6. Customer and product analysis.
7. Data visualization.
8. Business insights and recommendations.
9. Conclusion.

## 7. Data Cleaning and Preprocessing

Data cleaning was performed to improve the quality and reliability of the dataset.

### 7.1 Loading the Dataset

The Excel dataset was loaded into Python using Pandas.

### 7.2 Understanding the Dataset

The following functions were used:

- `data.head()` – Displays the first five records.
- `data.info()` – Displays column information and data types.
- `data.describe()` – Provides statistical summaries.
- `data.shape` – Displays the number of rows and columns.

### 7.3 Removing Duplicate Records

Duplicate records were identified and removed.

- Original records: 541,909
- Duplicate records identified: 5,268
- Records after duplicate removal: 536,641

### 7.4 Handling Missing Values

Missing values were identified in the Description and CustomerID columns.

Missing product descriptions were replaced with "Unknown Product".

Missing CustomerID values were retained because customer identifiers should not be artificially created.

### 7.5 Checking Invalid Values

The dataset was checked for negative and zero values in Quantity and UnitPrice.

Two records with negative unit prices were identified as accounting adjustments and excluded from the sales analysis.

### 7.6 Creating Total Price

A new column named `TotalPrice` was created to calculate the transaction value.

Formula:

`TotalPrice = Quantity × UnitPrice`

### 7.7 Separating Sales and Return Transactions

Transactions with positive quantities were separated as sales transactions.

Transactions with negative quantities were separated as negative-quantity or return/credit transactions for analysis.

## 8. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand the retail dataset and identify important business patterns.

The following analyses were completed:

### 8.1 Overall Sales Analysis

Calculated total sales revenue, return value and net sales.

### 8.2 Product Analysis

Identified the top-selling products based on quantity sold and revenue generated.

### 8.3 Country-wise Sales Analysis

Analysed sales revenue generated by different countries.

### 8.4 Monthly Sales Analysis

Examined monthly sales trends to identify high-performing months.

### 8.5 Day-wise Sales Analysis

Analysed sales performance across different days of the week.

### 8.6 Hour-wise Sales Analysis

Identified the hours during which the business generated the highest sales.

### 8.7 Customer Analysis

Identified customers based on the number of orders placed and total revenue generated.

### 8.8 Order Value Analysis

Examined the distribution of order values to understand customer spending patterns.

## 9. Data Visualization

The following visualizations were created using Matplotlib and Pandas.

1. Top 10 Countries by Sales: Identifies the countries generating the highest sales revenue.

2. Monthly Sales Trend: Displays sales performance across different months.

3. Top 10 Products by Quantity Sold: Identifies products with the highest sales quantity.

4. Top 10 Products by Revenue: Identifies products generating the highest revenue after excluding the identified postage and manual entries.

5. Sales by Day of the Week: Compares sales revenue across weekdays.

6. Sales by Hour of the Day: Identifies the hours with the highest sales activity.

7. Top 10 Customers by Number of Orders: Identifies customers who placed the highest number of orders.

8. Top 10 Customers by Revenue: Identifies customers generating the highest revenue.

9. Comparison of Sales and Returns: Compares total sales revenue with the value of negative-quantity transactions.

10. Distribution of Order Values: Uses a histogram to understand the distribution of order values, including a logarithmic-scale version.

## 10. Key Business Findings

The following findings were identified through the analysis:

### Overall Sales Performance

- Total sales revenue: 10,642,110.80
- Total return value: 893,979.73
- Net sales: 9,748,131.07
- Return percentage: Approximately 8.4%

### Product Performance

Paper Craft, Little Birdie was the highest-selling product by quantity, with 80,995 units sold.

Regency Cakestand 3 Tier generated the highest product revenue among the filtered product entries, with revenue of 174,156.54.

### Country-wise Performance

The United Kingdom generated the highest sales revenue among the countries analysed.

### Monthly Sales Performance

November 2011 recorded the highest monthly sales in the dataset.

### Day-wise Sales Performance

Thursday recorded the highest sales among the days with recorded transactions.

### Hour-wise Sales Performance

10 AM recorded the highest sales, with approximately 1,444,814.77 in revenue.

### Customer Performance

- Customer 12748 placed the highest number of orders, with 210 orders.
- Customer 14646 generated the highest revenue, with 280,206.02.

### Order Value Analysis

The order value distribution showed that most orders had relatively low values, while a small number of orders had very high values.

## 11. Business Recommendations

Based on the analysis, the following recommendations are suggested:

1. **Inventory Management:** Maintain sufficient stock of popular products to avoid stock shortages.

2. **Customer Retention:** Introduce loyalty rewards, discounts and special offers for frequent customers.

3. **Returns Management:** Investigate reasons for product returns and improve product descriptions, quality checks and packaging.

4. **Sales Planning:** Use monthly sales trends to plan promotional activities during lower-sales periods.

5. **Operational Planning:** Use hourly sales patterns to plan staffing and customer support during busy hours.

6. **Market Expansion:** Strengthen sales in the United Kingdom while exploring opportunities in other countries.

7. **High-Value Customer Analysis:** Study customers generating high revenue and develop strategies to maintain their engagement.

## 12. How to Run the Project

Follow these steps to run the project on your local system.

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
```

### Step 2: Navigate to the Project Folder

```bash
cd Real_World_Retail_Analytics
```

### Step 3: Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn openpyxl jupyter
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Open the Notebook

Open `retail_analytics.ipynb` and execute the cells sequentially.

Make sure the `Online Retail.xlsx` dataset is available in the project directory.

## 13. Project Structure

```text
Real_World_Retail_Analytics/
│
├── Online Retail.xlsx
│
├── retail_analytics.ipynb
│
└── README.md
```

## 14. Conclusion

This project demonstrates an end-to-end retail data analysis workflow using Python.

The analysis included data cleaning, preprocessing, Exploratory Data Analysis, sales analysis, customer analysis, product analysis and data visualization.

The project helped identify important retail business patterns, including top-performing products, customer purchasing behaviour, monthly sales trends, country-wise sales performance and product returns.

The insights generated from this analysis can help retail businesses make informed decisions regarding inventory management, customer retention, sales planning and business improvement.

## 15. Project Learning Outcomes

Through this project, practical experience was gained in:

- Working with real-world datasets.
- Python programming.
- Data cleaning and preprocessing.
- Pandas and NumPy.
- Exploratory Data Analysis.
- Data visualization using Matplotlib.
- Customer and sales analysis.
- Interpreting business insights.
- Preparing data analysis documentation.