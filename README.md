# Ecommerce Sales Analytics Pipeline

## Overview
End-to-end data analytics pipeline for e-commerce sales data using Apache PySpark on Databricks.

## Technologies Used
- Apache PySpark
- Databricks Free Edition
- Delta Lake
- Matplotlib
- Python

## Dataset
- Source: Kaggle — Retail Orders Dataset
- Records: 9,994
- Columns: 16

## Pipeline Architecture
orders.csv
↓
Databricks Unity Catalog Volume
↓
PySpark — Data Extraction
↓
PySpark — Data Quality Check
↓
PySpark — Transformations
↓
Business Insights

## Key Insights
- Top Region: West (Revenue: 34,67,409)
- Top Category: Technology (Revenue: 39,34,910)
- Top Sub Category: Chairs (Profit: 1,53,905)
- Best Year: 2023 (Revenue: 56,03,786)

## New Features Engineered
| Column | Logic |
|---|---|
| Sale Price | List Price after Discount |
| Revenue | Sale Price x Quantity |
| Profit | (Sale Price - Cost) x Quantity |
| Order Year | Extracted from Order Date |
| Profit Category | High / Medium / Loss |
Delta Lake Table
↓
Visualizations
