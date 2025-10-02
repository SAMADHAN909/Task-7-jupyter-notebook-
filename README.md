
## Objective
Get Basic Sales Summary from a Tiny SQLite Database using Python.

## Tools Used
- Python (sqlite3, pandas, matplotlib)
- SQLite (built-in Python library)
- Jupyter Notebook

## Steps Performed
1. Connected Python to SQLite database (`sales_data.db`).
2. Created a `sales` table with columns: product, quantity, price.
3. Inserted sample data (Pen, Notebook, Pencil, rubber,shopner).
4. Wrote SQL query to calculate total quantity & revenue for each product.
5. Loaded SQL results into Pandas DataFrame.
6. Printed sales summary in tabular format.
7. Created a simple bar chart showing revenue by product.
8. Saved chart as `sales_chart.png`.

## Output
- Printed sales summary table in Jupyter Notebook.
- Revenue bar chart plotted using Matplotlib.

## Sample Query
```sql
SELECT product,
       SUM(quantity) AS total_qty,
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;# Task-7-jupyter-notebook-
