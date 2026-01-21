# SQL Query Generator Automation

## Goal
Convert natural language into SQL query.

## Prompt
"Generate SQL to find total sales per product for last month."

## Output
SELECT product, SUM(sales) 
FROM orders 
WHERE order_date >= CURRENT_DATE - INTERVAL '30 days'
GROUP BY product;

## Business Value
Speeds up analyst productivity.
