# Zepto Inventory Analysis (PostgreSQL)

## Business Question
How many products are available or out of stock, and how do pricing, discounts, and pack sizes vary?

## Dataset
Public Kaggle dataset of Zepto product listings. This is publicly available listing data, not Zepto's internal data.

**Dataset link:**  https://www.kaggle.com/datasets/palvi...

## Tools Used
- PostgreSQL
- pgAdmin
- SQL
- VS Code

## Project Steps
1. Imported 3,732 rows from a CSV file into PostgreSQL.
2. Removed one row with a zero price.
3. Converted prices from paise to rupees.
4. Removed duplicate product records, leaving 1,800 records.
5. Used SQL queries to investigate inventory, pricing, discounts, categories, and pack sizes.

## Key Findings
- 12.1% of the 1,800 records were out of stock.
- Weight groups: 1,628 Low (under 1 kg), 149 Medium (1–5 kg), and 23 Bulk (over 5 kg).
- 39 products had an MRP above ₹500 and a discount below 10%.

## Data Limitations
Some products appear under multiple category names. For example, Cooking Essentials and Munchies each contain 514 records in the category count query. Therefore, category-level counts should be interpreted cautiously. Some recorded product weights may also be inaccurate.

## Project Files
- "zepto_analysis.sql" — SQL queries used for the analysis.
- "screenshots/" — Screenshots of selected query results.
