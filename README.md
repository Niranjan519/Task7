# Task7
SQLite in Python
 Task 7: Coffee Chain Sales Data Analysis
 Objective
The goal of this project was to demonstrate proficiency in connecting Python to an SQLite database, executing SQL queries to summarize data, and visualizing the results using a bar chart. Specifically, the script calculates the Total Sales Revenue by Product.

Technologies Used
Language: Python 3

Database: SQLite (sqlite3)

Data Handling: Pandas (pandas)

Visualization: Matplotlib (matplotlib)

Dataset
Coffee_Chain_Sales .csv: The primary dataset containing comprehensive sales records for various coffee products.

sales_data.db: SQLite database file created by the script to host the data.

Key Deliverables
The provided script, [your_script_name].py, accomplishes the following:

Database Connection: Creates and connects to sales_data.db.

Data Loading: Imports and loads the Coffee_Chain_Sales .csv data into an SQLite table named sales_table.

SQL Query Execution: Runs a GROUP BY query to aggregate total sales.

Output: Prints the resulting summary table to the console.

Visualization: Generates a basic Matplotlib bar chart and saves it as product_sales_chart.png.

Core SQL Query
The main query used to fulfill the objective:

SQL

SELECT
    Product,
    SUM(Sales) AS Total_Revenue
FROM
    sales_table
GROUP BY
    Product
ORDER BY
    Total_Revenue DESC;
How to Run the Script
Ensure you have Python installed and the necessary libraries:

Bash

pip install pandas matplotlib
Place the provided CSV file (Coffee_Chain_Sales .csv) and the Python script in the same directory.

Execute the script from your terminal:

Bash

python [your_script_name].py
The script will print the revenue table and display the bar chart visualization.
