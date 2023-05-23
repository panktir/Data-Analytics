### SQL Practice Problems

Here, I have attempted to solve various SQL problems for practice.

#### Customers and Orders Schema

**Customers**
- id (int)
- name (varchar)
- email (varchar)

**Orders**
- id (int)
- customer_id (int)
- order_date (date)

**Problem 1: Retrieving Customer Order Counts**

Write a query to retrieve the name, email, and total number of orders for all customers who have placed at least one order in each month of the year 2022. The results should be sorted in ascending order by customer name.

**Solution:**
```sql
SELECT c.name, COUNT(DISTINCT o.id) AS total_orders
FROM Customers c
JOIN Orders o ON c.id = o.customer_id
WHERE YEAR(o.order_date) = 2022
GROUP BY c.name
HAVING COUNT(DISTINCT MONTH(o.order_date)) = 12;
```

**Problem 2: Top Spending Customers**

Write an SQL query to find the top 5 customers who have spent the most money on orders placed in the year 2022, along with the total amount spent by each customer.

**Solution:**
```sql
SELECT c.name, c.email, SUM(o.order_total) AS total_spent
FROM Customers AS c
JOIN Orders AS o ON c.customer_id = o.customer_id
WHERE o.order_date BETWEEN '2022-01-01' AND '2022-12-31'
GROUP BY c.name, c.email
ORDER BY total_spent DESC
LIMIT 5;
```

#### Sales Schema

**Sales**
- id (int)
- salesperson_name (varchar)
- sale_amount (float)
- sale_date (date)

**Problem 1: Top Salespeople**

Write a query to retrieve the name and total sales for the top 3 salespeople in the company. The results should be sorted in descending order by total sales.

**Solution:**
```sql
SELECT salesperson_name, SUM(sale_amount) AS total_sales
FROM Sales
GROUP BY salesperson_name
ORDER BY total_sales DESC
LIMIT 3;
```
