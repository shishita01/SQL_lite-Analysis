# Basic Sales Summary Using SQLite and Python



# Project Overview

This project is part of the Data Analyst Internship program.
The objective of this task is to use SQL inside Python to extract basic sales information from a small SQLite database and visualize the results using a simple bar chart.



# Objective

Calculate total quantity sold per product
Calculate total revenue per product
Display results using:
Print statements
A basic matplotlib bar chart



# Tools & Technologies

Python
SQLite (via sqlite3)
Pandas
Matplotlib
Jupyter Notebook



# Dataset Description

A small SQLite database named sales_data.db was created with a single table:

Table: sales
Column	Description
product	Product name
quantity	Quantity sold
price	Price per unit

Sample data was manually inserted as required by the task.




# Approach

Created a SQLite database using Python
Inserted sample sales data
Executed SQL aggregation queries inside Python
Loaded query results into a pandas DataFrame
Printed the results
Visualized revenue by product using a bar chart




# SQL Query Used
SELECT
    product,
    SUM(quantity) AS total_qty,
    SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;



# Output

Tabular summary of total quantity and revenue per product

Bar chart showing Revenue by Product

# Deliverables

Jupyter Notebook (.ipynb)
SQLite database file (sales_data.db)
Printed results
Bar chart visualization

# Conclusion

This task demonstrates the use of SQL queries inside Python, basic data aggregation, and simple data visualization — essential skills for a data analyst.
