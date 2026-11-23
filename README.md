# Retail Sales Exploratory Data Analysis (EDA)

## Project Overview
This project focuses on analyzing retail sales data using Python. The main objective is to explore sales patterns, understand customer purchasing behavior, identify trends, and discover useful business insights through data analysis and visualization.

## Objectives
- Analyze monthly sales trends.
- Understand sales performance across different regions.
- Analyze customer payment method preferences.
- Study monthly order patterns.
- Understand the relationship between quantity and total sales.
- Identify correlations between sales, profit, pricing, and discounts.

## Technologies and Libraries Used
- Python
- Jupyter Notebook
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization

## Exploratory Data Analysis Performed

The following analyses and visualizations were performed:

1. Monthly Sales Trend
2. Total Sales by Region
3. Average Sales by Payment Method
4. Monthly Order Count
5. Number of Orders by Payment Method
6. Quantity vs Total Sales
7. Correlation Heatmap

## Key Findings

- Monthly sales fluctuate throughout the year.
- Sales performance differs across regions.
- UPI is the most frequently used payment method in the analyzed dataset.
- Monthly order counts vary across different months.
- Higher quantities are generally associated with higher total sales.
- Total Sales and Profit show a strong positive correlation of 0.81.
- Unit Price and Total Sales show a positive correlation of 0.78.
- Discount Percentage has a negative correlation with Profit (-0.31).

## Project Structure

```text
Exploratory_Data_Analysis/
│
├── retail_sales_eda.ipynb
├── README.md
└── dataset.csv
```

*Note: Replace `dataset.csv` with the actual name of your dataset file.*

## How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

3. Open the project folder in VS Code.
4. Open `retail_sales_eda.ipynb`.
5. Select the Python kernel.
6. Run the notebook cells to view the analysis and visualizations.

## Conclusion

This project provided practical experience in data cleaning, exploratory data analysis, data visualization, and interpreting business insights using Python.

The analysis helped understand retail sales trends, regional performance, payment preferences, order patterns, and relationships between important sales variables.