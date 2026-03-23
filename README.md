# Retail Store Profitability Analysis

## Executive Summary
This project analyzes the profitability of a global retail store across its primary product categories. By extracting raw sales data from a local relational database and utilizing Python for data manipulation and visualization, this analysis identifies the highest and lowest-performing sectors. 

## Technology Stack
* **Database Management:** MySQL, MySQL Workbench
* **Programming Language:** Python 3
* **Data Manipulation:** Pandas
* **Data Visualization:** Matplotlib, Seaborn

## Methodology

### Phase 1: Data Extraction (SQL)
The raw dataset (`global superstore raw`) within the `retail_db` database was queried to calculate business metrics. SQL scripts were used to:
* Aggregate total revenue and profit grouped by major product category to identify which high-level sectors drive the business.
* Drill down into specific sub-categories to find the top 10 strongest performing product groups.
* Filter exclusively for negative profit margins to pinpoint the top 10 individual products generating the most significant financial losses for the store.

### Phase 2: Data Transformation (Python/Pandas)
The query results were exported and securely loaded into a Python workspace. The Pandas library was utilized to read the data into a structured DataFrame, verifying the integrity of the three columns: Category, Total_Revenue, and Total_Profit. The extracted CSV data revealed the following exact metrics:
* **Technology:** $288,803.06 Revenue, $47,824.77 Profit
* **Office Supplies:** $157,965.95 Revenue, $44,664.57 Profit
* **Furniture:** $187,232.04 Revenue, $22,398.52 Profit

### Phase 3: Data Visualization (Seaborn)
To make the data accessible
