# BlinkIT Grocery Sales Performance Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

## Project Overview
The goal of this project is to analyze BlinkIT’s grocery sales data to uncover insights on sales trends, item popularity, and performance across different store types and locations. By examining metrics such as item sales, outlet performance, and customer ratings, we aim to provide actionable recommendations for inventory management, promotional strategies, and store operations.

## Data Source
This analysis is based on data from the "BlinkIT Grocery Analysis" Excel file, containing detailed information about grocery items, store attributes, and sales metrics.

## Tools
- **Python (Pandas)**: For data cleaning and preparation
- **Microsoft Excel**: For raw data exploration
- **Markdown**: For report documentation

## Data Cleaning
The following steps were taken to clean and prepare the data for analysis:
1. **Missing Values**: Checked for missing values in key columns and handled them as follows:
   - Used median values for numerical columns (e.g., `Item Weight`) where missing.
   - Imputed categorical columns with the most frequent category.
2. **Data Formatting**: Standardized formats in categorical columns (e.g., `Item Fat Content`).
3. **Outliers**: Detected and managed outliers in `Sales` and `Item Visibility` columns to ensure accurate analysis.
4. **Date Parsing**: Parsed `Outlet Establishment Year` to calculate the age of each outlet.

## Exploratory Data Analysis
The analysis explored the following key questions:
- What are the top-performing item categories in terms of sales?
- How does sales performance vary across outlet types and locations?
- Are there specific trends in customer ratings based on item type or outlet type?
- Which stores have the highest item visibility, and does visibility correlate with sales?

## Results
1. **Top-Performing Categories**: Fruits, vegetables, and beverages emerged as top-sellers.
2. **Sales Trends by Outlet Type**: Supermarkets of Type 1 generally had higher average sales, especially in Tier 1 locations.
3. **Rating and Sales Correlation**: Higher-rated items saw a small increase in sales, suggesting that quality impacts customer choice.
4. **Outlet Age and Performance**: Older outlets had slightly higher sales, possibly due to brand establishment and customer loyalty.

## Recommendations
Based on the findings, the following actions are recommended:
1. **Promotional Strategies**: Increase promotions for high-visibility items in Tier 1 locations.
2. **Inventory Focus**: Prioritize stocking popular categories (e.g., fresh produce, beverages) in high-demand outlets.
3. **Customer Feedback**: Use ratings to adjust inventory for items with consistently high ratings and low returns.
4. **Outlet Expansion**: Consider opening additional stores similar to high-performing locations, particularly in Tier 1 areas.

## Limitations
- **Data Completeness**: Some item weight data was missing, requiring imputation, which may slightly affect accuracy.
- **Visibility Metrics**: The `Item Visibility` metric was difficult to interpret without additional context on store layout.

## References
- [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
- [Data Cleaning Techniques](https://towardsdatascience.com/data-cleaning-techniques)
