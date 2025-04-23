# Retail Transaction Analytics (MBA Assignment)

This project showcases insights derived from analyzing retail transaction data using SAS and SQL. Completed as part of the Business Analytics course at Carleton University, this assignment demonstrates practical skills in data manipulation, statistical analysis, and business intelligence.

## Key Highlights
- 67K+ transactions processed
- 23K+ unique customers identified
- Region- and time-based sales insights
- Identification of top products and customer behaviors

## Tools & Techniques Used
- SAS: PROC SQL, DATA Step programming, summarization procedures
- SQL: Filtering, aggregation, joins, ranking

## Files Included
- `Retail_Transaction_Analytics_SAS_SQL_Presentation.pptx`: Slide deck summarizing findings and business insights
- `README.md`: Overview of the project

## Business Insights
- Tuesdays are peak sales days → Plan promotions accordingly
- “Lure Mepps Yellow” was the top-selling item in 1998 → Optimize inventory
- Average of 3 transactions per customer → Focus on retention strategies

# SAS to SQL Conversion

This repository also contains SQL translations of SAS Enterprise Guide queries used in a business analytics assignment.

Each query includes:
- Purpose – what the query aims to analyze
- Explanation – plain English summary of the logic
- SQL Code – optimized SQL syntax based on SAS logic

## Sample Queries

Query 1: Count Unique Transactions
SELECT COUNT(DISTINCT TRANSACTION_ID) FROM SALES_FACT;

Query 12: Top 10 Customers by Spend (1997)
SELECT CUST_ID, SUM(TRANSACTION_AMT)
FROM SALES_FACT
WHERE YEAR = 1997
GROUP BY CUST_ID
ORDER BY SUM(TRANSACTION_AMT) DESC
LIMIT 10;


---

Created by Herman Hui  
MBA in Business Analytics | Data-Driven Storyteller


## Author
Herman Hui  
[GitHub](https://github.com/huiherman)  
