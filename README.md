# Retail Store Profitability & Risk Analysis

## Executive Summary
This project analyzes the profitability of a global retail store by extracting raw sales data from a local relational database and utilizing Python for data manipulation and visualization. Beyond identifying macro-level category performance, this analysis drills down into sub-categories to find primary revenue drivers and conducts a strict loss analysis to pinpoint specific products operating at a negative profit margin. The primary finding indicates that while the Technology category drives the highest overall profit, specific individual products are actively bleeding revenue and require immediate business intervention.

## Project Objectives
* **Data Extraction & Exploration:** Query a local MySQL database to understand the dataset schema and aggregate total revenue and profit.
* **Granular Business Intelligence:** Execute drill-down SQL queries to identify top-performing sub-categories and isolate the top 10 loss-making products.
* **Data Transformation & Visualization:** Load the extracted SQL data into a Python environment using the Pandas library, designing professional bar charts to visually communicate profitability gaps to stakeholders.

## Technology Stack
* **Database Management:** MySQL, MySQL Workbench
* **Programming Language:** Python 3
* **Data Manipulation:** Pandas
* **Data Visualization:** Matplotlib, Seaborn

## Methodology

### Phase 1: Relational Database Querying (SQL)
To gather the necessary metrics, the raw dataset (`global superstore raw`) was queried at three different levels of granularity:
1. **Macro-Level:** Aggregating total revenue and profit grouped by the main Category.
2. **Micro-Level:** Drilling down to find the top 10 performing Sub-Category groups.
3. **Risk Mitigation:** Filtering explicitly for negative profit margins (Profit < 0) to identify the top 10 individual product items generating the highest financial losses.

### Phase 2: Data Transformation (Python/Pandas)
The aggregated macro-level query results were exported and securely loaded into a cloud-based Python workspace (Google Colab). The Pandas library was utilized to read the data into a structured DataFrame, verifying the integrity of the data types before plotting.

### Phase 3: Data Visualization (Seaborn)
To make the data accessible for business decision-making, Seaborn and Matplotlib were used to generate a high-resolution bar chart mapping Total Profit against each primary Category.

## Key Findings & Business Insights
* **Technology is the Leading Profit Driver:** At a macro level, the Technology category generated the highest profit, nearing the $50,000 mark.
* **Granular Sub-Category Performance:** Further SQL analysis revealed the top 10 sub-categories, allowing the business to see exactly which specific item types (rather than just broad categories) are keeping the business profitable.
* **Critical Loss Leaders Identified:** The risk mitigation query successfully isolated the bottom 10 products operating at a loss. Despite units being sold, these specific products are actively reducing the company's net profit.

## Strategic Recommendations
* **Audit Loss-Making Products:** Immediately halt or audit the supply chain for the bottom 10 products identified in the SQL loss analysis. The business must determine if the negative margins are due to high shipping costs, supplier pricing, or extreme discounting.
* **Reallocate Marketing Budget:** Shift marketing spend away from the underperforming Furniture sector and heavily promote the top 10 Sub-Categories identified in the micro-level analysis to maximize Return on Ad Spend (ROAS).

---
**Author:** Aditya Singh Tomar
